# Comparing `tmp/pluto_rt-0.7.1.tar.gz` & `tmp/pluto_rt-0.7.2.tar.gz`

## Comparing `pluto_rt-0.7.1.tar` & `pluto_rt-0.7.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/MANIFEST.in
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/Dockerfile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/__init__.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/asgi.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/compose.yaml
--rwxr-xr-x   0        0        0      701 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/manage.py
--rw-r--r--   0        0        0  2281154 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/pluto_rt_demo.gif
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/requirements.txt
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/settings.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/tasks.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/urls.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/views.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/wsgi.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/templates/demo/demo_index.html
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/templates/demo/demo_list.html
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/templates/demo/demo_messages.html
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/templates/demo/demo_progress.html
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/templates/pluto_rt/list_item.html
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/templates/pluto_rt/progress_item.html
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/demo/templates/pluto_rt/toast_item.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/src/pluto_rt/__init__.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/src/pluto_rt/apps.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/src/pluto_rt/ops.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/src/pluto_rt/urls.py
--rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/src/pluto_rt/views.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/src/pluto_rt/templates/pluto_rt/polling.html
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/src/pluto_rt/templates/pluto_rt/sse.html
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/src/pluto_rt/templates/pluto_rt/table.html
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/src/pluto_rt/templates/pluto_rt/table_item.html
--rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/src/pluto_rt.egg-info/PKG-INFO
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/src/pluto_rt.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/src/pluto_rt.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/src/pluto_rt.egg-info/top_level.txt
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/tests/tests.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/.gitignore
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/LICENSE
--rw-r--r--   0        0        0     6945 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/README.md
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 pluto_rt-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/MANIFEST.in
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/demo/Dockerfile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/demo/__init__.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/demo/asgi.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/demo/compose.yaml
+-rwxr-xr-x   0        0        0      701 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/demo/manage.py
+-rw-r--r--   0        0        0  2281154 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/demo/pluto_rt_demo.gif
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/demo/requirements.txt
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/demo/settings.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/demo/tasks.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/demo/urls.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/demo/views.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/demo/wsgi.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/demo/templates/demo/demo_index.html
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/demo/templates/demo/demo_list.html
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/demo/templates/demo/demo_messages.html
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/demo/templates/demo/demo_progress.html
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/demo/templates/pluto_rt/list_item.html
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/demo/templates/pluto_rt/progress_item.html
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/demo/templates/pluto_rt/toast_item.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/src/pluto_rt/__init__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/src/pluto_rt/apps.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/src/pluto_rt/ops.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/src/pluto_rt/urls.py
+-rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/src/pluto_rt/views.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/src/pluto_rt/templates/pluto_rt/polling.html
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/src/pluto_rt/templates/pluto_rt/sse.html
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/src/pluto_rt/templates/pluto_rt/table.html
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/src/pluto_rt/templates/pluto_rt/table_item.html
+-rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/src/pluto_rt.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/src/pluto_rt.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/src/pluto_rt.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/src/pluto_rt.egg-info/top_level.txt
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/tests/tests.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/.gitignore
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/LICENSE
+-rw-r--r--   0        0        0     7297 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/README.md
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     7912 2020-02-02 00:00:00.000000 pluto_rt-0.7.2/PKG-INFO
```

### Comparing `pluto_rt-0.7.1/demo/compose.yaml` & `pluto_rt-0.7.2/demo/compose.yaml`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.7.1/demo/manage.py` & `pluto_rt-0.7.2/demo/manage.py`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.7.1/demo/pluto_rt_demo.gif` & `pluto_rt-0.7.2/demo/pluto_rt_demo.gif`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.7.1/demo/settings.py` & `pluto_rt-0.7.2/demo/settings.py`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.7.1/demo/tasks.py` & `pluto_rt-0.7.2/demo/tasks.py`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.7.1/demo/views.py` & `pluto_rt-0.7.2/demo/views.py`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.7.1/demo/templates/demo/demo_index.html` & `pluto_rt-0.7.2/demo/templates/demo/demo_index.html`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.7.1/demo/templates/demo/demo_list.html` & `pluto_rt-0.7.2/demo/templates/demo/demo_list.html`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.7.1/demo/templates/demo/demo_messages.html` & `pluto_rt-0.7.2/demo/templates/demo/demo_messages.html`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.7.1/demo/templates/demo/demo_progress.html` & `pluto_rt-0.7.2/demo/templates/demo/demo_progress.html`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.7.1/src/pluto_rt/ops.py` & `pluto_rt-0.7.2/src/pluto_rt/ops.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,22 +13,24 @@
 
     QUEUE_EXHAUSTED = '"_queue_exhausted_"'
 
     def __init__(self, name: str, **kwargs):
         self.name = name
         self.redis = get_redis_connection("default")
 
-    def complete(self, clear_delay: int = 5):
-        """Mark the queue as complete, wait a few seconds and then purge the queue
-        purging can be skipped if clear_delay is 0
+    def complete(self, clear_delay: int | None = None):
+        """Mark the queue as complete, usually wait a few seconds and then purge the queue
+        default purging is 5 seconds unless specified in settings or specified in argument
+        using a delay of 0 will omit the sleep
         """
         self.push(self.QUEUE_EXHAUSTED)
+        clear_delay = int(clear_delay or getattr(settings, "PLUTO_RT_CLEAR_DELAY", 5))
         if clear_delay:
             time.sleep(clear_delay)
-            self.redis.delete(self.name)
+        self.redis.delete(self.name)
 
     def push(self, message: dict):
         message = pickle.dumps(message)
         self.redis.rpush(self.name, message)
 
     def pop(self) -> dict | None:
         raw_message = self.redis.lpop(self.name)
```

### Comparing `pluto_rt-0.7.1/src/pluto_rt/urls.py` & `pluto_rt-0.7.2/src/pluto_rt/urls.py`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.7.1/src/pluto_rt/views.py` & `pluto_rt-0.7.2/src/pluto_rt/views.py`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.7.1/src/pluto_rt/templates/pluto_rt/table.html` & `pluto_rt-0.7.2/src/pluto_rt/templates/pluto_rt/table.html`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.7.1/src/pluto_rt.egg-info/PKG-INFO` & `pluto_rt-0.7.2/src/pluto_rt.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `pluto_rt-0.7.1/README.md` & `pluto_rt-0.7.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -132,14 +132,17 @@
 We require the path to contain "pluto_rt" as a security measure. Frankly there is little chance that any data might be exposed via a template (the context contains only the `item` variable), but it makes security a little tidier. You can use a path named "pluto_rt", or include it in the template file name.
 
 ## Stop polling
 
 If you call `complete()` on the queue, the view will return a message that tells htmx to stop polling. So in your processing function, be sure
 to call that function when the work is done.
 
+The default delay between calling `complete()` and having the queue purged is 5 seconds. This can be overridden by passing an int argument (seconds) to `complete()`,
+ or via the optional django setting `PLUTO_RT_CLEAR_DELAY`. For testing, this setting should be 0 to prevent slow pytests.
+
 ## Distribution and license
 
 Creating this as a private ES github repo first, for re-usability,
 with intention to secure permission to open source it in the future.
 
 When this is pip-installed, it will install the wheel, which means you need to recompile the wheel after making changes.
 
@@ -174,7 +177,9 @@
 0.5.0 Mar 3, 2024: Improved template inclusion, added demos
 
 0.6.0 Mar 9, 2024: Use modes, add replace
 
 0.7.0 Apr 9, 2024: Support multiple consumers
 
 0.7.1 Apr 19, 20204: Keepalive every 10 seconds
+
+0.7.2 Apr 23, 20204: Use setting to avoid sleep (for pytest)
```

### Comparing `pluto_rt-0.7.1/pyproject.toml` & `pluto_rt-0.7.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pluto_rt"
-version = "0.7.1"
+version = "0.7.2"
 authors = [
   { name="Scot Hacker", email="shacker@energy-solution.com" },
   { name="Rob Harvey", email="rharvey@energy-solution.com" },
 ]
 description = "A reusable Django app providing a kit for storing and displaying messages from a background processor into a web view in real time, as the processor works."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `pluto_rt-0.7.1/PKG-INFO` & `pluto_rt-0.7.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pluto_rt
-Version: 0.7.1
+Version: 0.7.2
 Summary: A reusable Django app providing a kit for storing and displaying messages from a background processor into a web view in real time, as the processor works.
 Project-URL: Homepage, https://github.com/energy-solution/pluto-rt
 Author-email: Scot Hacker <shacker@energy-solution.com>, Rob Harvey <rharvey@energy-solution.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -145,14 +145,17 @@
 We require the path to contain "pluto_rt" as a security measure. Frankly there is little chance that any data might be exposed via a template (the context contains only the `item` variable), but it makes security a little tidier. You can use a path named "pluto_rt", or include it in the template file name.
 
 ## Stop polling
 
 If you call `complete()` on the queue, the view will return a message that tells htmx to stop polling. So in your processing function, be sure
 to call that function when the work is done.
 
+The default delay between calling `complete()` and having the queue purged is 5 seconds. This can be overridden by passing an int argument (seconds) to `complete()`,
+ or via the optional django setting `PLUTO_RT_CLEAR_DELAY`. For testing, this setting should be 0 to prevent slow pytests.
+
 ## Distribution and license
 
 Creating this as a private ES github repo first, for re-usability,
 with intention to secure permission to open source it in the future.
 
 When this is pip-installed, it will install the wheel, which means you need to recompile the wheel after making changes.
 
@@ -187,7 +190,9 @@
 0.5.0 Mar 3, 2024: Improved template inclusion, added demos
 
 0.6.0 Mar 9, 2024: Use modes, add replace
 
 0.7.0 Apr 9, 2024: Support multiple consumers
 
 0.7.1 Apr 19, 20204: Keepalive every 10 seconds
+
+0.7.2 Apr 23, 20204: Use setting to avoid sleep (for pytest)
```

