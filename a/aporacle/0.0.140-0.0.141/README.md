# Comparing `tmp/aporacle-0.0.140.tar.gz` & `tmp/aporacle-0.0.141.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aporacle-0.0.140.tar", max compression
+gzip compressed data, was "aporacle-0.0.141.tar", max compression
```

## Comparing `aporacle-0.0.140.tar` & `aporacle-0.0.141.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2024-02-28 04:02:27.389085 aporacle-0.0.140/README.md
--rw-r--r--   0        0        0      265 2024-03-20 16:45:48.348259 aporacle-0.0.140/aporacle/__init__.py
--rw-r--r--   0        0        0     1717 2024-03-26 04:23:06.584243 aporacle-0.0.140/aporacle/broadcast/__init__.py
--rw-r--r--   0        0        0     2834 2024-03-26 04:26:39.150092 aporacle-0.0.140/aporacle/conf/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 16:41:03.985547 aporacle-0.0.140/aporacle/core/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 16:41:11.733621 aporacle-0.0.140/aporacle/core/utils/__init__.py
--rw-r--r--   0        0        0     4383 2024-03-20 16:45:48.336259 aporacle-0.0.140/aporacle/core/utils/async_call_scheduler.py
--rw-r--r--   0        0        0        0 2024-03-10 13:49:56.523746 aporacle-0.0.140/aporacle/data/__init__.py
--rw-r--r--   0        0        0      589 2024-03-11 05:27:14.610597 aporacle-0.0.140/aporacle/data/asset/__init__.py
--rw-r--r--   0        0        0     1543 2024-04-19 13:19:36.337225 aporacle-0.0.140/aporacle/data/combination.py
--rw-r--r--   0        0        0        0 2024-03-10 13:50:08.923807 aporacle-0.0.140/aporacle/data/db/__init__.py
--rw-r--r--   0        0        0      684 2024-03-18 04:25:23.973270 aporacle-0.0.140/aporacle/data/db/crud.py
--rw-r--r--   0        0        0      869 2024-04-19 06:59:59.684489 aporacle-0.0.140/aporacle/data/feed_results.py
--rw-r--r--   0        0        0    10186 2024-04-19 06:26:40.918071 aporacle-0.0.140/aporacle/data/gcp/__init__.py
--rw-r--r--   0        0        0      615 2024-03-18 04:07:19.874287 aporacle-0.0.140/aporacle/data/symbols/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 16:12:22.030426 aporacle-0.0.140/aporacle/execution/__init__.py
--rw-r--r--   0        0        0     5923 2024-04-23 16:47:31.692033 aporacle-0.0.140/aporacle/execution/executables.py
--rw-r--r--   0        0        0        0 2024-03-20 16:39:34.468697 aporacle-0.0.140/aporacle/network/__init__.py
--rw-r--r--   0        0        0     4316 2024-03-12 15:57:25.236568 aporacle-0.0.140/aporacle/network/network_base.py
--rw-r--r--   0        0        0     1583 2024-03-11 12:44:12.298311 aporacle-0.0.140/aporacle/shared_setup.py
--rw-r--r--   0        0        0      399 2024-04-23 16:48:06.696337 aporacle-0.0.140/pyproject.toml
--rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 aporacle-0.0.140/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-28 04:02:27.389085 aporacle-0.0.141/README.md
+-rw-r--r--   0        0        0      265 2024-03-20 16:45:48.348259 aporacle-0.0.141/aporacle/__init__.py
+-rw-r--r--   0        0        0     1717 2024-03-26 04:23:06.584243 aporacle-0.0.141/aporacle/broadcast/__init__.py
+-rw-r--r--   0        0        0     2834 2024-03-26 04:26:39.150092 aporacle-0.0.141/aporacle/conf/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:41:03.985547 aporacle-0.0.141/aporacle/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:41:11.733621 aporacle-0.0.141/aporacle/core/utils/__init__.py
+-rw-r--r--   0        0        0     4383 2024-03-20 16:45:48.336259 aporacle-0.0.141/aporacle/core/utils/async_call_scheduler.py
+-rw-r--r--   0        0        0        0 2024-03-10 13:49:56.523746 aporacle-0.0.141/aporacle/data/__init__.py
+-rw-r--r--   0        0        0      589 2024-03-11 05:27:14.610597 aporacle-0.0.141/aporacle/data/asset/__init__.py
+-rw-r--r--   0        0        0     1543 2024-04-19 13:19:36.337225 aporacle-0.0.141/aporacle/data/combination.py
+-rw-r--r--   0        0        0        0 2024-03-10 13:50:08.923807 aporacle-0.0.141/aporacle/data/db/__init__.py
+-rw-r--r--   0        0        0      684 2024-03-18 04:25:23.973270 aporacle-0.0.141/aporacle/data/db/crud.py
+-rw-r--r--   0        0        0      869 2024-04-19 06:59:59.684489 aporacle-0.0.141/aporacle/data/feed_results.py
+-rw-r--r--   0        0        0    10186 2024-04-19 06:26:40.918071 aporacle-0.0.141/aporacle/data/gcp/__init__.py
+-rw-r--r--   0        0        0      615 2024-03-18 04:07:19.874287 aporacle-0.0.141/aporacle/data/symbols/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-11 16:12:22.030426 aporacle-0.0.141/aporacle/execution/__init__.py
+-rw-r--r--   0        0        0     6135 2024-04-24 12:29:15.753203 aporacle-0.0.141/aporacle/execution/executables.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:39:34.468697 aporacle-0.0.141/aporacle/network/__init__.py
+-rw-r--r--   0        0        0     4316 2024-03-12 15:57:25.236568 aporacle-0.0.141/aporacle/network/network_base.py
+-rw-r--r--   0        0        0     1583 2024-03-11 12:44:12.298311 aporacle-0.0.141/aporacle/shared_setup.py
+-rw-r--r--   0        0        0      399 2024-04-24 12:29:30.925339 aporacle-0.0.141/pyproject.toml
+-rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 aporacle-0.0.141/PKG-INFO
```

### Comparing `aporacle-0.0.140/aporacle/broadcast/__init__.py` & `aporacle-0.0.141/aporacle/broadcast/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.140/aporacle/conf/__init__.py` & `aporacle-0.0.141/aporacle/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.140/aporacle/core/utils/async_call_scheduler.py` & `aporacle-0.0.141/aporacle/core/utils/async_call_scheduler.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.140/aporacle/data/asset/__init__.py` & `aporacle-0.0.141/aporacle/data/asset/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.140/aporacle/data/combination.py` & `aporacle-0.0.141/aporacle/data/combination.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.140/aporacle/data/db/crud.py` & `aporacle-0.0.141/aporacle/data/db/crud.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.140/aporacle/data/feed_results.py` & `aporacle-0.0.141/aporacle/data/feed_results.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.140/aporacle/data/gcp/__init__.py` & `aporacle-0.0.141/aporacle/data/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.140/aporacle/data/symbols/__init__.py` & `aporacle-0.0.141/aporacle/data/symbols/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.140/aporacle/execution/executables.py` & `aporacle-0.0.141/aporacle/execution/executables.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,36 +12,44 @@
 
 class VotingRoundExecutable(KomoBase):
     def __init__(self):
         super().__init__()
 
         self._schedule_queue: asyncio.Queue = asyncio.Queue()
         # self.epoch_schedule: Optional[dict] = {"coston": None, "flare": None, "songbird": None}
-        self.epoch_schedule: Optional[dict] = {"coston": {"voting_round": 0}}
+        self.epoch_schedule: Optional[dict] = {}
 
         self._epoch_scheduler_task: Optional[asyncio.Task] = None
         self._ws_listener_task: Optional[asyncio.Task] = None
 
-        self._ready: bool = False
-
     @property
     def name(self):
         return "voting_round_executable"
 
     def initialize(self):
         pass
 
+    def start_network(self):
+        raise NotImplementedError
+
+    def stop_network(self):
+        raise NotImplementedError
+
     async def start(self):
         self.initialize()
         self._epoch_scheduler_task = safe_ensure_future(self.epoch_scheduling_loop())
-        [safe_ensure_future(self.tso_listener_loop(chain=chain)) for chain in self.epoch_schedule.keys()]
-        self._ready = True
+        [await self.tso_listener_loop(chain=chain) for chain in self.epoch_schedule.keys()]
+
+        self.start_network()
+
+    async def stop(self):
+        self.stop_network()
+
+
 
-    def stop(self):
-        pass
 
     def utilities_message_processor(self, message: dict):
         raise NotImplementedError
 
     def epoch_schedule_processor(self, message: dict):
         raise NotImplementedError
 
@@ -60,14 +68,17 @@
 
                 if message["voting_round"] <= self.epoch_schedule[message["chain"]]["voting_round"]:
                     self.log_with_clock(log_level=logging.WARNING,
                                         msg=f"Voting round {message['voting_round']} for chain {message['chain']} "
                                             f"has already been scheduled. ")
                     continue
 
+                if message["chain"] not in self.epoch_schedule:
+                    self.epoch_schedule.update({message["chain"]: {}})
+
                 self.epoch_schedule[message["chain"]] = {
                     "chain": message["chain"],
                     "reward_epoch": message['reward_epoch'],
                     "voting_round": message['voting_round'],
                     "start_time": message["voting_round_start"],
                 }
```

### Comparing `aporacle-0.0.140/aporacle/network/network_base.py` & `aporacle-0.0.141/aporacle/network/network_base.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.140/aporacle/shared_setup.py` & `aporacle-0.0.141/aporacle/shared_setup.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.140/PKG-INFO` & `aporacle-0.0.141/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aporacle
-Version: 0.0.140
+Version: 0.0.141
 Summary: 
 Author: Makhosonke Morafo
 Author-email: makhosonke@komokun.org
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

