# Comparing `tmp/aporacle-0.0.139.tar.gz` & `tmp/aporacle-0.0.140.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aporacle-0.0.139.tar", max compression
+gzip compressed data, was "aporacle-0.0.140.tar", max compression
```

## Comparing `aporacle-0.0.139.tar` & `aporacle-0.0.140.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2024-02-28 04:02:27.389085 aporacle-0.0.139/README.md
--rw-r--r--   0        0        0      265 2024-03-20 16:45:48.348259 aporacle-0.0.139/aporacle/__init__.py
--rw-r--r--   0        0        0     1717 2024-03-26 04:23:06.584243 aporacle-0.0.139/aporacle/broadcast/__init__.py
--rw-r--r--   0        0        0     2834 2024-03-26 04:26:39.150092 aporacle-0.0.139/aporacle/conf/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 16:41:03.985547 aporacle-0.0.139/aporacle/core/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 16:41:11.733621 aporacle-0.0.139/aporacle/core/utils/__init__.py
--rw-r--r--   0        0        0     4383 2024-03-20 16:45:48.336259 aporacle-0.0.139/aporacle/core/utils/async_call_scheduler.py
--rw-r--r--   0        0        0        0 2024-03-10 13:49:56.523746 aporacle-0.0.139/aporacle/data/__init__.py
--rw-r--r--   0        0        0      589 2024-03-11 05:27:14.610597 aporacle-0.0.139/aporacle/data/asset/__init__.py
--rw-r--r--   0        0        0     1543 2024-04-19 13:19:36.337225 aporacle-0.0.139/aporacle/data/combination.py
--rw-r--r--   0        0        0        0 2024-03-10 13:50:08.923807 aporacle-0.0.139/aporacle/data/db/__init__.py
--rw-r--r--   0        0        0      684 2024-03-18 04:25:23.973270 aporacle-0.0.139/aporacle/data/db/crud.py
--rw-r--r--   0        0        0      869 2024-04-19 06:59:59.684489 aporacle-0.0.139/aporacle/data/feed_results.py
--rw-r--r--   0        0        0    10186 2024-04-19 06:26:40.918071 aporacle-0.0.139/aporacle/data/gcp/__init__.py
--rw-r--r--   0        0        0      615 2024-03-18 04:07:19.874287 aporacle-0.0.139/aporacle/data/symbols/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 16:12:22.030426 aporacle-0.0.139/aporacle/execution/__init__.py
--rw-r--r--   0        0        0     5666 2024-03-27 10:53:43.099151 aporacle-0.0.139/aporacle/execution/executables.py
--rw-r--r--   0        0        0        0 2024-03-20 16:39:34.468697 aporacle-0.0.139/aporacle/network/__init__.py
--rw-r--r--   0        0        0     4316 2024-03-12 15:57:25.236568 aporacle-0.0.139/aporacle/network/network_base.py
--rw-r--r--   0        0        0     1583 2024-03-11 12:44:12.298311 aporacle-0.0.139/aporacle/shared_setup.py
--rw-r--r--   0        0        0      399 2024-04-19 13:19:36.333225 aporacle-0.0.139/pyproject.toml
--rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 aporacle-0.0.139/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-28 04:02:27.389085 aporacle-0.0.140/README.md
+-rw-r--r--   0        0        0      265 2024-03-20 16:45:48.348259 aporacle-0.0.140/aporacle/__init__.py
+-rw-r--r--   0        0        0     1717 2024-03-26 04:23:06.584243 aporacle-0.0.140/aporacle/broadcast/__init__.py
+-rw-r--r--   0        0        0     2834 2024-03-26 04:26:39.150092 aporacle-0.0.140/aporacle/conf/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:41:03.985547 aporacle-0.0.140/aporacle/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:41:11.733621 aporacle-0.0.140/aporacle/core/utils/__init__.py
+-rw-r--r--   0        0        0     4383 2024-03-20 16:45:48.336259 aporacle-0.0.140/aporacle/core/utils/async_call_scheduler.py
+-rw-r--r--   0        0        0        0 2024-03-10 13:49:56.523746 aporacle-0.0.140/aporacle/data/__init__.py
+-rw-r--r--   0        0        0      589 2024-03-11 05:27:14.610597 aporacle-0.0.140/aporacle/data/asset/__init__.py
+-rw-r--r--   0        0        0     1543 2024-04-19 13:19:36.337225 aporacle-0.0.140/aporacle/data/combination.py
+-rw-r--r--   0        0        0        0 2024-03-10 13:50:08.923807 aporacle-0.0.140/aporacle/data/db/__init__.py
+-rw-r--r--   0        0        0      684 2024-03-18 04:25:23.973270 aporacle-0.0.140/aporacle/data/db/crud.py
+-rw-r--r--   0        0        0      869 2024-04-19 06:59:59.684489 aporacle-0.0.140/aporacle/data/feed_results.py
+-rw-r--r--   0        0        0    10186 2024-04-19 06:26:40.918071 aporacle-0.0.140/aporacle/data/gcp/__init__.py
+-rw-r--r--   0        0        0      615 2024-03-18 04:07:19.874287 aporacle-0.0.140/aporacle/data/symbols/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-11 16:12:22.030426 aporacle-0.0.140/aporacle/execution/__init__.py
+-rw-r--r--   0        0        0     5923 2024-04-23 16:47:31.692033 aporacle-0.0.140/aporacle/execution/executables.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:39:34.468697 aporacle-0.0.140/aporacle/network/__init__.py
+-rw-r--r--   0        0        0     4316 2024-03-12 15:57:25.236568 aporacle-0.0.140/aporacle/network/network_base.py
+-rw-r--r--   0        0        0     1583 2024-03-11 12:44:12.298311 aporacle-0.0.140/aporacle/shared_setup.py
+-rw-r--r--   0        0        0      399 2024-04-23 16:48:06.696337 aporacle-0.0.140/pyproject.toml
+-rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 aporacle-0.0.140/PKG-INFO
```

### Comparing `aporacle-0.0.139/aporacle/broadcast/__init__.py` & `aporacle-0.0.140/aporacle/broadcast/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.139/aporacle/conf/__init__.py` & `aporacle-0.0.140/aporacle/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.139/aporacle/core/utils/async_call_scheduler.py` & `aporacle-0.0.140/aporacle/core/utils/async_call_scheduler.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.139/aporacle/data/asset/__init__.py` & `aporacle-0.0.140/aporacle/data/asset/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.139/aporacle/data/combination.py` & `aporacle-0.0.140/aporacle/data/combination.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.139/aporacle/data/db/crud.py` & `aporacle-0.0.140/aporacle/data/db/crud.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.139/aporacle/data/feed_results.py` & `aporacle-0.0.140/aporacle/data/feed_results.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.139/aporacle/data/gcp/__init__.py` & `aporacle-0.0.140/aporacle/data/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.139/aporacle/data/symbols/__init__.py` & `aporacle-0.0.140/aporacle/data/symbols/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.139/aporacle/execution/executables.py` & `aporacle-0.0.140/aporacle/execution/executables.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,14 +67,17 @@
                 self.epoch_schedule[message["chain"]] = {
                     "chain": message["chain"],
                     "reward_epoch": message['reward_epoch'],
                     "voting_round": message['voting_round'],
                     "start_time": message["voting_round_start"],
                 }
 
+                self.log_with_clock(log_level=logging.WARNING,
+                                    msg=f"Scheduling voting round {message['voting_round']} for {message['chain']}. ")
+
                 self.epoch_schedule_processor(message=self.epoch_schedule[message["chain"]])
             except NotImplementedError as nie:
                 self.log_with_clock(log_level=logging.WARNING, msg=f"Epoch schedule processor not implemented. {nie}")
             except Exception as e:
                 self.log_with_clock(log_level=logging.ERROR, msg=f"Exception. {e}")
 
     async def tso_listener_loop(self, chain: str):
@@ -91,38 +94,40 @@
                     SubscribeRequest(type='subscribe', topics=conf.tso_utility_topics).model_dump_json())
 
                 while True:
                     try:
                         # print("Waiting for message")
                         data = await websocket.recv()
                         message = json.loads(data)
-                        # print(message)
+                        print(message)
                         if 'success' in message:
                             continue
 
-                        if message['event'] in ['new_voting_round_initiated']:
+                        if message['event'] in ['voting_round_initiated']:
                             self.log_with_clock(log_level=logging.INFO,
                                                 msg=f"Got new schedule message for round {message['voting_round']}. ")
 
                             safe_ensure_future(self._schedule_queue.put(message))
                             self.log_with_clock(log_level=logging.INFO,
                                                 msg=f"Waiting for the next TSO schedule message. ")
                             continue
 
-                        # print(message)
+                        print(message)
                         self.utilities_message_processor(message=message)
 
                     except websockets.ConnectionClosed as cc:
                         self.log_with_clock(log_level=logging.ERROR,
                                             msg=f"Connection to {url} was closed. {cc}. Will re-establish connection. ")
-                        await asyncio.sleep(1)
+                        await asyncio.sleep(5)
                         safe_ensure_future(self.tso_listener_loop(chain=chain))
 
                     except Exception as e:
                         self.log_with_clock(log_level=logging.ERROR,
                                             msg=f"Failed to connect to {url}. On message - {e}. ")
+                        await asyncio.sleep(5)
                         safe_ensure_future(self.tso_listener_loop(chain=chain))
 
         except Exception as e:
             self.log_with_clock(log_level=logging.ERROR,
                                 msg=f"Failed to connect to {url}. On message - {e}. ")
+            await asyncio.sleep(5)
             safe_ensure_future(self.tso_listener_loop(chain=chain))
```

### Comparing `aporacle-0.0.139/aporacle/network/network_base.py` & `aporacle-0.0.140/aporacle/network/network_base.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.139/aporacle/shared_setup.py` & `aporacle-0.0.140/aporacle/shared_setup.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.139/PKG-INFO` & `aporacle-0.0.140/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aporacle
-Version: 0.0.139
+Version: 0.0.140
 Summary: 
 Author: Makhosonke Morafo
 Author-email: makhosonke@komokun.org
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

