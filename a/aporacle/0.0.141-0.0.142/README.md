# Comparing `tmp/aporacle-0.0.141.tar.gz` & `tmp/aporacle-0.0.142.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aporacle-0.0.141.tar", max compression
+gzip compressed data, was "aporacle-0.0.142.tar", max compression
```

## Comparing `aporacle-0.0.141.tar` & `aporacle-0.0.142.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2024-02-28 04:02:27.389085 aporacle-0.0.141/README.md
--rw-r--r--   0        0        0      265 2024-03-20 16:45:48.348259 aporacle-0.0.141/aporacle/__init__.py
--rw-r--r--   0        0        0     1717 2024-03-26 04:23:06.584243 aporacle-0.0.141/aporacle/broadcast/__init__.py
--rw-r--r--   0        0        0     2834 2024-03-26 04:26:39.150092 aporacle-0.0.141/aporacle/conf/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 16:41:03.985547 aporacle-0.0.141/aporacle/core/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 16:41:11.733621 aporacle-0.0.141/aporacle/core/utils/__init__.py
--rw-r--r--   0        0        0     4383 2024-03-20 16:45:48.336259 aporacle-0.0.141/aporacle/core/utils/async_call_scheduler.py
--rw-r--r--   0        0        0        0 2024-03-10 13:49:56.523746 aporacle-0.0.141/aporacle/data/__init__.py
--rw-r--r--   0        0        0      589 2024-03-11 05:27:14.610597 aporacle-0.0.141/aporacle/data/asset/__init__.py
--rw-r--r--   0        0        0     1543 2024-04-19 13:19:36.337225 aporacle-0.0.141/aporacle/data/combination.py
--rw-r--r--   0        0        0        0 2024-03-10 13:50:08.923807 aporacle-0.0.141/aporacle/data/db/__init__.py
--rw-r--r--   0        0        0      684 2024-03-18 04:25:23.973270 aporacle-0.0.141/aporacle/data/db/crud.py
--rw-r--r--   0        0        0      869 2024-04-19 06:59:59.684489 aporacle-0.0.141/aporacle/data/feed_results.py
--rw-r--r--   0        0        0    10186 2024-04-19 06:26:40.918071 aporacle-0.0.141/aporacle/data/gcp/__init__.py
--rw-r--r--   0        0        0      615 2024-03-18 04:07:19.874287 aporacle-0.0.141/aporacle/data/symbols/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 16:12:22.030426 aporacle-0.0.141/aporacle/execution/__init__.py
--rw-r--r--   0        0        0     6135 2024-04-24 12:29:15.753203 aporacle-0.0.141/aporacle/execution/executables.py
--rw-r--r--   0        0        0        0 2024-03-20 16:39:34.468697 aporacle-0.0.141/aporacle/network/__init__.py
--rw-r--r--   0        0        0     4316 2024-03-12 15:57:25.236568 aporacle-0.0.141/aporacle/network/network_base.py
--rw-r--r--   0        0        0     1583 2024-03-11 12:44:12.298311 aporacle-0.0.141/aporacle/shared_setup.py
--rw-r--r--   0        0        0      399 2024-04-24 12:29:30.925339 aporacle-0.0.141/pyproject.toml
--rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 aporacle-0.0.141/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-28 04:02:27.389085 aporacle-0.0.142/README.md
+-rw-r--r--   0        0        0      265 2024-03-20 16:45:48.348259 aporacle-0.0.142/aporacle/__init__.py
+-rw-r--r--   0        0        0     1717 2024-03-26 04:23:06.584243 aporacle-0.0.142/aporacle/broadcast/__init__.py
+-rw-r--r--   0        0        0     2834 2024-03-26 04:26:39.150092 aporacle-0.0.142/aporacle/conf/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:41:03.985547 aporacle-0.0.142/aporacle/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:41:11.733621 aporacle-0.0.142/aporacle/core/utils/__init__.py
+-rw-r--r--   0        0        0     4383 2024-03-20 16:45:48.336259 aporacle-0.0.142/aporacle/core/utils/async_call_scheduler.py
+-rw-r--r--   0        0        0        0 2024-03-10 13:49:56.523746 aporacle-0.0.142/aporacle/data/__init__.py
+-rw-r--r--   0        0        0      589 2024-03-11 05:27:14.610597 aporacle-0.0.142/aporacle/data/asset/__init__.py
+-rw-r--r--   0        0        0     1543 2024-04-19 13:19:36.337225 aporacle-0.0.142/aporacle/data/combination.py
+-rw-r--r--   0        0        0        0 2024-03-10 13:50:08.923807 aporacle-0.0.142/aporacle/data/db/__init__.py
+-rw-r--r--   0        0        0      684 2024-03-18 04:25:23.973270 aporacle-0.0.142/aporacle/data/db/crud.py
+-rw-r--r--   0        0        0      869 2024-04-19 06:59:59.684489 aporacle-0.0.142/aporacle/data/feed_results.py
+-rw-r--r--   0        0        0    10186 2024-04-19 06:26:40.918071 aporacle-0.0.142/aporacle/data/gcp/__init__.py
+-rw-r--r--   0        0        0      615 2024-03-18 04:07:19.874287 aporacle-0.0.142/aporacle/data/symbols/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-11 16:12:22.030426 aporacle-0.0.142/aporacle/execution/__init__.py
+-rw-r--r--   0        0        0     6086 2024-04-24 12:49:52.772335 aporacle-0.0.142/aporacle/execution/executables.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:39:34.468697 aporacle-0.0.142/aporacle/network/__init__.py
+-rw-r--r--   0        0        0     4316 2024-03-12 15:57:25.236568 aporacle-0.0.142/aporacle/network/network_base.py
+-rw-r--r--   0        0        0     1583 2024-03-11 12:44:12.298311 aporacle-0.0.142/aporacle/shared_setup.py
+-rw-r--r--   0        0        0      399 2024-04-24 12:49:15.231999 aporacle-0.0.142/pyproject.toml
+-rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 aporacle-0.0.142/PKG-INFO
```

### Comparing `aporacle-0.0.141/aporacle/broadcast/__init__.py` & `aporacle-0.0.142/aporacle/broadcast/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.141/aporacle/conf/__init__.py` & `aporacle-0.0.142/aporacle/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.141/aporacle/core/utils/async_call_scheduler.py` & `aporacle-0.0.142/aporacle/core/utils/async_call_scheduler.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.141/aporacle/data/asset/__init__.py` & `aporacle-0.0.142/aporacle/data/asset/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.141/aporacle/data/combination.py` & `aporacle-0.0.142/aporacle/data/combination.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.141/aporacle/data/db/crud.py` & `aporacle-0.0.142/aporacle/data/db/crud.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.141/aporacle/data/feed_results.py` & `aporacle-0.0.142/aporacle/data/feed_results.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.141/aporacle/data/gcp/__init__.py` & `aporacle-0.0.142/aporacle/data/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.141/aporacle/data/symbols/__init__.py` & `aporacle-0.0.142/aporacle/data/symbols/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.141/aporacle/execution/executables.py` & `aporacle-0.0.142/aporacle/execution/executables.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,50 +7,45 @@
 import websockets
 from komoutils.core import KomoBase, safe_ensure_future, SubscribeRequest
 
 from aporacle import conf
 
 
 class VotingRoundExecutable(KomoBase):
-    def __init__(self):
+    def __init__(self, chains: list):
         super().__init__()
-
-        self._schedule_queue: asyncio.Queue = asyncio.Queue()
-        # self.epoch_schedule: Optional[dict] = {"coston": None, "flare": None, "songbird": None}
+        self.chains = chains
         self.epoch_schedule: Optional[dict] = {}
-
+        self._schedule_queue: asyncio.Queue = asyncio.Queue()
         self._epoch_scheduler_task: Optional[asyncio.Task] = None
         self._ws_listener_task: Optional[asyncio.Task] = None
 
     @property
     def name(self):
         return "voting_round_executable"
 
     def initialize(self):
         pass
 
     def start_network(self):
-        raise NotImplementedError
+        pass
 
     def stop_network(self):
-        raise NotImplementedError
+        pass
 
     async def start(self):
-        self.initialize()
+        assert len(self.chains) > 0, "No chains provided. Please provide at least one chain."
         self._epoch_scheduler_task = safe_ensure_future(self.epoch_scheduling_loop())
-        [await self.tso_listener_loop(chain=chain) for chain in self.epoch_schedule.keys()]
+        [await self.tso_listener_loop(chain=chain) for chain in self.chains]
 
         self.start_network()
 
     async def stop(self):
         self.stop_network()
 
-
-
-
     def utilities_message_processor(self, message: dict):
         raise NotImplementedError
 
     def epoch_schedule_processor(self, message: dict):
         raise NotImplementedError
 
     async def epoch_scheduling_loop(self):
```

### Comparing `aporacle-0.0.141/aporacle/network/network_base.py` & `aporacle-0.0.142/aporacle/network/network_base.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.141/aporacle/shared_setup.py` & `aporacle-0.0.142/aporacle/shared_setup.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.141/PKG-INFO` & `aporacle-0.0.142/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aporacle
-Version: 0.0.141
+Version: 0.0.142
 Summary: 
 Author: Makhosonke Morafo
 Author-email: makhosonke@komokun.org
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

