# Comparing `tmp/ws_sync-0.6.1.tar.gz` & `tmp/ws_sync-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ws_sync-0.6.1.tar", max compression
+gzip compressed data, was "ws_sync-0.6.3.tar", max compression
```

## Comparing `ws_sync-0.6.1.tar` & `ws_sync-0.6.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     4912 2024-02-20 18:33:05.515422 ws_sync-0.6.1/README.md
--rw-r--r--   0        0        0      374 2024-04-18 01:05:03.783505 ws_sync-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      429 2024-04-03 03:54:28.931620 ws_sync-0.6.1/ws_sync/__init__.py
--rw-r--r--   0        0        0     3484 2024-04-03 03:52:59.911008 ws_sync-0.6.1/ws_sync/decorators.py
--rw-r--r--   0        0        0      842 2024-01-31 22:47:04.922252 ws_sync-0.6.1/ws_sync/id.py
--rw-r--r--   0        0        0     4912 2024-04-18 01:04:18.002636 ws_sync-0.6.1/ws_sync/session.py
--rw-r--r--   0        0        0    16688 2024-04-03 05:19:45.797505 ws_sync-0.6.1/ws_sync/sync.py
--rw-r--r--   0        0        0      705 2024-04-03 03:01:49.284779 ws_sync-0.6.1/ws_sync/utils.py
--rw-r--r--   0        0        0     5548 1970-01-01 00:00:00.000000 ws_sync-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     4912 2024-02-20 18:33:05.515422 ws_sync-0.6.3/README.md
+-rw-r--r--   0        0        0      374 2024-04-24 16:12:00.282742 ws_sync-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0      429 2024-04-03 03:54:28.931620 ws_sync-0.6.3/ws_sync/__init__.py
+-rw-r--r--   0        0        0     3484 2024-04-03 03:52:59.911008 ws_sync-0.6.3/ws_sync/decorators.py
+-rw-r--r--   0        0        0      842 2024-01-31 22:47:04.922252 ws_sync-0.6.3/ws_sync/id.py
+-rw-r--r--   0        0        0     5071 2024-04-24 15:50:52.693591 ws_sync-0.6.3/ws_sync/session.py
+-rw-r--r--   0        0        0    16692 2024-04-19 10:31:36.837688 ws_sync-0.6.3/ws_sync/sync.py
+-rw-r--r--   0        0        0      705 2024-04-03 03:01:49.284779 ws_sync-0.6.3/ws_sync/utils.py
+-rw-r--r--   0        0        0     5548 1970-01-01 00:00:00.000000 ws_sync-0.6.3/PKG-INFO
```

### Comparing `ws_sync-0.6.1/README.md` & `ws_sync-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `ws_sync-0.6.1/ws_sync/decorators.py` & `ws_sync-0.6.3/ws_sync/decorators.py`

 * *Files identical despite different names*

### Comparing `ws_sync-0.6.1/ws_sync/id.py` & `ws_sync-0.6.3/ws_sync/id.py`

 * *Files identical despite different names*

### Comparing `ws_sync-0.6.1/ws_sync/session.py` & `ws_sync-0.6.3/ws_sync/session.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,17 @@
     @property
     def is_connected(self):
         return self.ws is not None
 
     # ===== Low-Level: Register Event Callbacks =====#
     def register_event(self, event: str, callback: Callable):
         if event in self.event_handlers:
-            raise Exception(f"Event {event} already has a subscriber.")
+            # raise Exception(f"Event {event} already has a subscriber.")
+            if self.logger:
+                self.logger.warning(f"Event {event} already has a subscriber.")
         self.event_handlers[event] = callback
 
     def deregister_event(self, event: str):
         if event not in self.event_handlers:
             raise Exception(f"Event {event} has no subscriber.")
         del self.event_handlers[event]
 
@@ -127,12 +129,13 @@
                 self.ws = None
                 await ws.close()
             except:
                 pass
 
     # ===== High-Level: Context Manager =====#
     def __enter__(self):
-        session_context.set(self)
+        self.token = session_context.set(self)
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
-        session_context.reset()
+        session_context.reset(self.token)
+        self.token = None
```

### Comparing `ws_sync-0.6.1/ws_sync/sync.py` & `ws_sync-0.6.3/ws_sync/sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,18 +237,18 @@
             )
 
         # create reverse-lookup for patching
         self.key_to_attr = {key: attr for attr, key in self.sync_attributes.items()}
 
         # ========== Debugging ========== #
         if self.logger:
-            self.logger.info(f"{self.key}: Syncing {self.sync_attributes}")
-            self.logger.info(f"{self.key}: Actions {actions}")
-            self.logger.info(f"{self.key}: Tasks {tasks}")
-            self.logger.info(f"{self.key}: Task Cancels {task_cancels}")
+            self.logger.debug(f"{self.key}: Syncing {self.sync_attributes}")
+            self.logger.debug(f"{self.key}: Actions {actions}")
+            self.logger.debug(f"{self.key}: Tasks {tasks}")
+            self.logger.debug(f"{self.key}: Task Cancels {task_cancels}")
 
         assert include.keys().isdisjoint(exclude), "Attribute in both include & exclude"
         assert all(a in dir(obj) for a in self.sync_attributes), "Attribute not found"
         assert all(e in dir(obj) for e in exclude), "Excluded attribute not found"
         assert (
             len(self.sync_attributes) + expose_running_tasks > 0
         ), "No attributes to sync"
```

### Comparing `ws_sync-0.6.1/ws_sync/utils.py` & `ws_sync-0.6.3/ws_sync/utils.py`

 * *Files identical despite different names*

### Comparing `ws_sync-0.6.1/PKG-INFO` & `ws_sync-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ws-sync
-Version: 0.6.1
+Version: 0.6.3
 Summary: Keep objects synchronized over a persistent WebSocket session
 Author: Joong-Won Seo
 Author-email: joong.won.seo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

