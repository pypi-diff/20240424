# Comparing `tmp/rrtask-0.0.5.tar.gz` & `tmp/rrtask-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rrtask-0.0.5.tar", max compression
+gzip compressed data, was "rrtask-0.0.6.tar", max compression
```

## Comparing `rrtask-0.0.5.tar` & `rrtask-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1063 2024-04-23 08:17:03.738389 rrtask-0.0.5/LICENSE
--rw-r--r--   0        0        0      210 2024-04-24 08:52:17.584490 rrtask-0.0.5/README.md
--rw-r--r--   0        0        0      581 2024-04-24 09:12:48.294029 rrtask-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      133 2024-04-24 09:02:58.172982 rrtask-0.0.5/rrtask/__init__.py
--rw-r--r--   0        0        0      171 2024-04-24 08:30:19.015153 rrtask-0.0.5/rrtask/enums.py
--rw-r--r--   0        0        0     5621 2024-04-24 08:56:57.928565 rrtask-0.0.5/rrtask/rrtask.py
--rw-r--r--   0        0        0      394 2024-04-24 08:50:30.008555 rrtask-0.0.5/rrtask/signals.py
--rw-r--r--   0        0        0      298 2024-04-24 08:50:30.008555 rrtask-0.0.5/rrtask/utils.py
--rw-r--r--   0        0        0       18 2024-04-24 09:12:50.010033 rrtask-0.0.5/rrtask/version.py
--rw-r--r--   0        0        0      701 1970-01-01 00:00:00.000000 rrtask-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-23 08:17:03.738389 rrtask-0.0.6/LICENSE
+-rw-r--r--   0        0        0      210 2024-04-24 08:52:17.584490 rrtask-0.0.6/README.md
+-rw-r--r--   0        0        0      581 2024-04-24 10:13:31.923879 rrtask-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      133 2024-04-24 09:02:58.172982 rrtask-0.0.6/rrtask/__init__.py
+-rw-r--r--   0        0        0      171 2024-04-24 08:30:19.015153 rrtask-0.0.6/rrtask/enums.py
+-rw-r--r--   0        0        0     5567 2024-04-24 10:13:13.927827 rrtask-0.0.6/rrtask/rrtask.py
+-rw-r--r--   0        0        0      394 2024-04-24 08:50:30.008555 rrtask-0.0.6/rrtask/signals.py
+-rw-r--r--   0        0        0      179 2024-04-24 10:11:29.383527 rrtask-0.0.6/rrtask/utils.py
+-rw-r--r--   0        0        0       18 2024-04-24 10:13:33.723884 rrtask-0.0.6/rrtask/version.py
+-rw-r--r--   0        0        0      701 1970-01-01 00:00:00.000000 rrtask-0.0.6/PKG-INFO
```

### Comparing `rrtask-0.0.5/LICENSE` & `rrtask-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rrtask-0.0.5/pyproject.toml` & `rrtask-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rrtask"
-version = "0.0.5"
+version = "0.0.6"
 description = "Round Robin Task"
 authors = ["François Schmidts <francois@schmidts.fr>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "==3.7.*"
```

### Comparing `rrtask-0.0.5/rrtask/rrtask.py` & `rrtask-0.0.6/rrtask/rrtask.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import logging
 from datetime import datetime
 from typing import Generator, Optional, Union
 from uuid import uuid4
 
+from redis import Redis
 from celery import Celery, current_task  # type: ignore
 
 from rrtask import signals
 from rrtask.enums import State
-from rrtask.utils import get_rabbitmq_client, get_redis_conn
+from rrtask.utils import get_rabbitmq_client
 
 logger = logging.getLogger(__name__)
 
 
 class RoundRobinTask:
     shall_loop_in: Optional[Union[float, int]] = None
 
     def __init__(
         self,
         celery_app: Celery,
-        redis_host: str,
-        redis_db: int = 10,
+        redis: Redis,
         queue_prefix: str = "",
     ):
         self._celery_app = celery_app
-        self._redis_conn = get_redis_conn(redis_host, redis_db)
+        self._redis_conn = redis
         self._queue_prefix = queue_prefix
 
         logger.info("Registering %s", self.queue_name)
         self._recurring_task = self.__set_recuring_task()
         self._scheduler_task = self.__set_scheduling_task()
 
     def recurring_task(self, **kwd_params) -> Union[bool, State]:
```

### Comparing `rrtask-0.0.5/PKG-INFO` & `rrtask-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rrtask
-Version: 0.0.5
+Version: 0.0.6
 Summary: Round Robin Task
 License: MIT
 Author: François Schmidts
 Author-email: francois@schmidts.fr
 Requires-Python: ==3.7.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

