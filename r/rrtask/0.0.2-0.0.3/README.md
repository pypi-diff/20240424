# Comparing `tmp/rrtask-0.0.2.tar.gz` & `tmp/rrtask-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rrtask-0.0.2.tar", max compression
+gzip compressed data, was "rrtask-0.0.3.tar", max compression
```

## Comparing `rrtask-0.0.2.tar` & `rrtask-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1063 2024-04-23 08:17:03.738389 rrtask-0.0.2/LICENSE
--rw-r--r--   0        0        0      210 2024-04-24 08:51:24.908514 rrtask-0.0.2/README.md
--rw-r--r--   0        0        0      605 2024-04-24 08:51:55.456498 rrtask-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-23 08:32:27.303989 rrtask-0.0.2/rrtask/__init__.py
--rw-r--r--   0        0        0      171 2024-04-24 08:30:19.015153 rrtask-0.0.2/rrtask/enums.py
--rw-r--r--   0        0        0     5558 2024-04-24 08:50:30.008555 rrtask-0.0.2/rrtask/rrtask.py
--rw-r--r--   0        0        0      394 2024-04-24 08:50:30.008555 rrtask-0.0.2/rrtask/signals.py
--rw-r--r--   0        0        0      298 2024-04-24 08:50:30.008555 rrtask-0.0.2/rrtask/utils.py
--rw-r--r--   0        0        0       18 2024-04-24 08:52:01.472496 rrtask-0.0.2/rrtask/version.py
--rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 rrtask-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-23 08:17:03.738389 rrtask-0.0.3/LICENSE
+-rw-r--r--   0        0        0      210 2024-04-24 08:52:17.584490 rrtask-0.0.3/README.md
+-rw-r--r--   0        0        0      605 2024-04-24 08:58:37.864653 rrtask-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-23 08:32:27.303989 rrtask-0.0.3/rrtask/__init__.py
+-rw-r--r--   0        0        0      171 2024-04-24 08:30:19.015153 rrtask-0.0.3/rrtask/enums.py
+-rw-r--r--   0        0        0     5621 2024-04-24 08:56:57.928565 rrtask-0.0.3/rrtask/rrtask.py
+-rw-r--r--   0        0        0      394 2024-04-24 08:50:30.008555 rrtask-0.0.3/rrtask/signals.py
+-rw-r--r--   0        0        0      298 2024-04-24 08:50:30.008555 rrtask-0.0.3/rrtask/utils.py
+-rw-r--r--   0        0        0       18 2024-04-24 08:58:43.296658 rrtask-0.0.3/rrtask/version.py
+-rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 rrtask-0.0.3/PKG-INFO
```

### Comparing `rrtask-0.0.2/LICENSE` & `rrtask-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rrtask-0.0.2/pyproject.toml` & `rrtask-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rrtask"
-version = "0.0.2"
+version = "0.0.3"
 description = "Round Robin Task"
 authors = ["François Schmidts <francois@schmidts.fr>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "3.7.*"
```

### Comparing `rrtask-0.0.2/rrtask/rrtask.py` & `rrtask-0.0.3/rrtask/rrtask.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,18 +139,19 @@
                 self._recurring_task.apply_async(
                     kwargs=params,
                     countdown=int(i * delay_between_task) or None,
                 )
 
             # push yourself
             logger.info("Rescheduling %s", self.queue_name)
-            schedule_uuid = str(uuid4())
+            reschedule_id = str(uuid4())
             self._scheduler_task.apply_async(
-                args=[schedule_uuid], countdown=self.shall_loop_in
+                args=[reschedule_id], countdown=self.shall_loop_in
             )
+            self.mark_for_scheduling(task_name, reschedule_id)
             signals.task.send(current_task, status=State.FINISHED, **sigload)
             return State.FINISHED
 
         return __scheduler_task
 
     @property
     def queue_name(self):
```

### Comparing `rrtask-0.0.2/PKG-INFO` & `rrtask-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rrtask
-Version: 0.0.2
+Version: 0.0.3
 Summary: Round Robin Task
 License: MIT
 Author: François Schmidts
 Author-email: francois@schmidts.fr
 Requires-Python: ==3.7.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

