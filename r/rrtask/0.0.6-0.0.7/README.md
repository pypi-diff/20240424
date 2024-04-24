# Comparing `tmp/rrtask-0.0.6.tar.gz` & `tmp/rrtask-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rrtask-0.0.6.tar", max compression
+gzip compressed data, was "rrtask-0.0.7.tar", max compression
```

## Comparing `rrtask-0.0.6.tar` & `rrtask-0.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1063 2024-04-23 08:17:03.738389 rrtask-0.0.6/LICENSE
--rw-r--r--   0        0        0      210 2024-04-24 08:52:17.584490 rrtask-0.0.6/README.md
--rw-r--r--   0        0        0      581 2024-04-24 10:13:31.923879 rrtask-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      133 2024-04-24 09:02:58.172982 rrtask-0.0.6/rrtask/__init__.py
--rw-r--r--   0        0        0      171 2024-04-24 08:30:19.015153 rrtask-0.0.6/rrtask/enums.py
--rw-r--r--   0        0        0     5567 2024-04-24 10:13:13.927827 rrtask-0.0.6/rrtask/rrtask.py
--rw-r--r--   0        0        0      394 2024-04-24 08:50:30.008555 rrtask-0.0.6/rrtask/signals.py
--rw-r--r--   0        0        0      179 2024-04-24 10:11:29.383527 rrtask-0.0.6/rrtask/utils.py
--rw-r--r--   0        0        0       18 2024-04-24 10:13:33.723884 rrtask-0.0.6/rrtask/version.py
--rw-r--r--   0        0        0      701 1970-01-01 00:00:00.000000 rrtask-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-23 08:17:03.738389 rrtask-0.0.7/LICENSE
+-rw-r--r--   0        0        0      210 2024-04-24 08:52:17.584490 rrtask-0.0.7/README.md
+-rw-r--r--   0        0        0      581 2024-04-24 12:07:42.120789 rrtask-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      133 2024-04-24 09:02:58.172982 rrtask-0.0.7/rrtask/__init__.py
+-rw-r--r--   0        0        0      195 2024-04-24 12:06:28.840639 rrtask-0.0.7/rrtask/enums.py
+-rw-r--r--   0        0        0     5617 2024-04-24 12:22:24.327022 rrtask-0.0.7/rrtask/rrtask.py
+-rw-r--r--   0        0        0      394 2024-04-24 08:50:30.008555 rrtask-0.0.7/rrtask/signals.py
+-rw-r--r--   0        0        0      179 2024-04-24 10:11:29.383527 rrtask-0.0.7/rrtask/utils.py
+-rw-r--r--   0        0        0       18 2024-04-24 12:26:55.715653 rrtask-0.0.7/rrtask/version.py
+-rw-r--r--   0        0        0      701 1970-01-01 00:00:00.000000 rrtask-0.0.7/PKG-INFO
```

### Comparing `rrtask-0.0.6/LICENSE` & `rrtask-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rrtask-0.0.6/pyproject.toml` & `rrtask-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rrtask"
-version = "0.0.6"
+version = "0.0.7"
 description = "Round Robin Task"
 authors = ["François Schmidts <francois@schmidts.fr>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "==3.7.*"
```

### Comparing `rrtask-0.0.6/rrtask/rrtask.py` & `rrtask-0.0.7/rrtask/rrtask.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 import logging
-from datetime import datetime
 from typing import Generator, Optional, Union
-from uuid import uuid4
 
 from redis import Redis
 from celery import Celery, current_task  # type: ignore
 
 from rrtask import signals
 from rrtask.enums import State
 from rrtask.utils import get_rabbitmq_client
 
 logger = logging.getLogger(__name__)
 
 
 class RoundRobinTask:
     shall_loop_in: Optional[Union[float, int]] = None
+    _lock_expire = 10 * 60
 
     def __init__(
         self,
-        celery_app: Celery,
+        celery: Celery,
         redis: Redis,
         queue_prefix: str = "",
     ):
-        self._celery_app = celery_app
-        self._redis_conn = redis
+        self._celery = celery
+        self._redis = redis
         self._queue_prefix = queue_prefix
 
         logger.info("Registering %s", self.queue_name)
         self._recurring_task = self.__set_recuring_task()
         self._scheduler_task = self.__set_scheduling_task()
 
     def recurring_task(self, **kwd_params) -> Union[bool, State]:
@@ -38,92 +37,98 @@
 
     def reschedule_params(self) -> Generator[dict, None, None]:
         """This method should return an iterable. Each element of this iterable
         is a valid argument for the true task (aka self.recurring_task).
         """
         raise NotImplementedError("should be overridden")
 
+    @property
+    def queue_name(self):
+        if self._queue_prefix:
+            return f"{self._queue_prefix}.{self.__class__.__name__}"
+        return self.__class__.__name__
+
+    @property
     def is_queue_empty(self) -> int:
-        rabbitmq_conn = self._celery_app.broker_connection()
+        rabbitmq_conn = self._celery.broker_connection()
         rabbitmq_client = get_rabbitmq_client(
             rabbitmq_conn.host, rabbitmq_conn.userid, rabbitmq_conn.password
         )
         queue_depth = rabbitmq_client.get_queue_depth(
             rabbitmq_conn.virtual_host, self.queue_name
         )
         return queue_depth == 0
 
+    def is_rescheduling_allowed(self, force: bool = False) -> bool:
+        lock_key = f"{self.queue_name}.lock"
+        if not self._redis.setnx(lock_key, 1):
+            return False
+        self._redis.expire(lock_key, self._lock_expire)
+        try:
+            uuid = current_task.request.id
+        except AttributeError:
+            uuid = None
+        if uuid and self._redis.delete(f"{self.queue_name}.{uuid}"):
+            self._redis.delete(lock_key)
+            return True
+        if force:
+            self._redis.delete(lock_key)
+            return True
+        if self.is_queue_empty:
+            self._redis.delete(lock_key)
+            return True
+        return False
+
+    def mark_for_scheduling(self, schedule_id: str):
+        self._redis.set(f"{self.queue_name}.{schedule_id}", 1)
+
     def __set_recuring_task(self):
         task_name = f"{self.queue_name}.recurring_task"
 
-        @self._celery_app.task(
-            queue=self.queue_name,
-            ignore_result=True,
-            name=task_name,
+        @self._celery.task(
+            queue=self.queue_name, ignore_result=True, name=task_name
         )
         def __recurring_task(**kwd_params):
             sigload = {
                 "task_name": task_name,
                 "queue_name": self.queue_name,
                 "task_kwargs": kwd_params,
             }
             signals.task.send(current_task, status=State.STARTING, **sigload)
-            task_state = State.SKIPPED
+            status = State.SKIPPED
             try:
                 result = self.recurring_task(**kwd_params)
                 if isinstance(result, State):
-                    task_state = result
+                    status = result
                 elif result is True:
-                    task_state = State.FINISHED
+                    status = State.FINISHED
+                else:
+                    status = State.UNKNOWN
             except Exception:
-                task_state = State.ERRORED
+                status = State.ERRORED
                 raise
-            signals.task.send(current_task, status=task_state, **sigload)
-            return task_state.value
+            signals.task.send(current_task, status=status, **sigload)
+            return status.value
 
         return __recurring_task
 
-    def is_rescheduling_allowed(
-        self, task_name: str, uuid: Optional[str], force: bool
-    ) -> bool:
-        slot_freed = False
-        if uuid:
-            slot_freed = bool(self._redis_conn.delete(f"{task_name}.{uuid}"))
-            if slot_freed:
-                return True
-        if force:
-            return True
-        if self.is_queue_empty():
-            return True
-        return False
-
-    def mark_for_scheduling(self, task_name: str, uuid: str):
-        self._redis_conn.set(
-            f"{task_name}.{uuid}", datetime.utcnow().isoformat()
-        )
-
     def __set_scheduling_task(self):
         task_name = f"{self.queue_name}.scheduler_task"
 
-        @self._celery_app.task(
-            queue=self.queue_name,
-            ignore_result=True,
-            name=task_name,
+        @self._celery.task(
+            queue=self.queue_name, ignore_result=True, name=task_name
         )
-        def __scheduler_task(
-            schedule_id: Optional[str] = None, force: bool = False
-        ):
+        def __scheduler_task(force: bool = False):
             sigload = {
                 "task_name": task_name,
                 "queue_name": self.queue_name,
-                "schedule_id": schedule_id,
                 "force": force,
             }
             signals.task.send(current_task, status=State.STARTING, **sigload)
-            if not self.is_rescheduling_allowed(task_name, schedule_id, force):
+            if not self.is_rescheduling_allowed(force):
                 status = State.SKIPPED
                 signals.task.send(current_task, status=status, **sigload)
                 return status
 
             # Push all other stuff in queue
             params_list = list(self.reschedule_params())
             task_count = len(params_list)
@@ -139,22 +144,18 @@
                 self._recurring_task.apply_async(
                     kwargs=params,
                     countdown=int(i * delay_between_task) or None,
                 )
 
             # push yourself
             logger.info("Rescheduling %s", self.queue_name)
-            reschedule_id = str(uuid4())
-            self._scheduler_task.apply_async(
-                args=[reschedule_id], countdown=self.shall_loop_in
+            async_res = self._scheduler_task.apply_async(
+                countdown=self.shall_loop_in or None
             )
-            self.mark_for_scheduling(task_name, reschedule_id)
+            self.mark_for_scheduling(async_res.id)
             signals.task.send(current_task, status=State.FINISHED, **sigload)
             return State.FINISHED
 
         return __scheduler_task
 
-    @property
-    def queue_name(self):
-        if self._queue_prefix:
-            return f"{self._queue_prefix}.{self.__class__.__name__}"
-        return self.__class__.__name__
+    def start(self):
+        self._scheduler_task()
```

### Comparing `rrtask-0.0.6/PKG-INFO` & `rrtask-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rrtask
-Version: 0.0.6
+Version: 0.0.7
 Summary: Round Robin Task
 License: MIT
 Author: François Schmidts
 Author-email: francois@schmidts.fr
 Requires-Python: ==3.7.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

