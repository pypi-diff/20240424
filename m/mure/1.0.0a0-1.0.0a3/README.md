# Comparing `tmp/mure-1.0.0a0.tar.gz` & `tmp/mure-1.0.0a3.tar.gz`

## Comparing `mure-1.0.0a0.tar` & `mure-1.0.0a3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 mure-1.0.0a0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 mure-1.0.0a0/requirements-dev.lock
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 mure-1.0.0a0/requirements.lock
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 mure-1.0.0a0/.github/workflows/main.yml
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 mure-1.0.0a0/examples/example.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mure-1.0.0a0/mure/__init__.py
--rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 mure-1.0.0a0/mure/core.py
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 mure-1.0.0a0/mure/dtos.py
--rw-r--r--   0        0        0     8559 2020-02-02 00:00:00.000000 mure-1.0.0a0/mure/iterator.py
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 mure-1.0.0a0/mure/logging.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 mure-1.0.0a0/tests/test_mure.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 mure-1.0.0a0/.gitignore
--rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 mure-1.0.0a0/LICENSE
--rw-r--r--   0        0        0     6526 2020-02-02 00:00:00.000000 mure-1.0.0a0/README.md
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 mure-1.0.0a0/pyproject.toml
--rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 mure-1.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 mure-1.0.0a3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 mure-1.0.0a3/requirements-dev.lock
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 mure-1.0.0a3/requirements.lock
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 mure-1.0.0a3/.github/workflows/main.yml
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 mure-1.0.0a3/examples/example.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mure-1.0.0a3/mure/__init__.py
+-rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 mure-1.0.0a3/mure/core.py
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 mure-1.0.0a3/mure/dtos.py
+-rw-r--r--   0        0        0     8732 2020-02-02 00:00:00.000000 mure-1.0.0a3/mure/iterator.py
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 mure-1.0.0a3/mure/logging.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 mure-1.0.0a3/tests/test_mure.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 mure-1.0.0a3/.gitignore
+-rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 mure-1.0.0a3/LICENSE
+-rw-r--r--   0        0        0     6526 2020-02-02 00:00:00.000000 mure-1.0.0a3/README.md
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 mure-1.0.0a3/pyproject.toml
+-rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 mure-1.0.0a3/PKG-INFO
```

### Comparing `mure-1.0.0a0/requirements-dev.lock` & `mure-1.0.0a3/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a0/.github/workflows/main.yml` & `mure-1.0.0a3/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a0/examples/example.py` & `mure-1.0.0a3/examples/example.py`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a0/mure/core.py` & `mure-1.0.0a3/mure/core.py`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a0/mure/dtos.py` & `mure-1.0.0a3/mure/dtos.py`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a0/mure/iterator.py` & `mure-1.0.0a3/mure/iterator.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,18 +94,23 @@
         """Cancel open tasks (if any) and close the event loop."""
         if self._loop.is_closed():
             return
 
         if self._generator:
             self._loop.run_until_complete(self._generator.aclose())
 
-        if self._tasks:
-            for task in self._tasks:
+        # cancel pending tasks (if any)
+        if tasks := {
+            task
+            for task in self._tasks | asyncio.all_tasks(self._loop)
+            if not task.done() or task.cancelled()
+        }:
+            for task in tasks:
                 task.cancel()
-            self._loop.run_until_complete(asyncio.gather(*self._tasks, return_exceptions=True))
+            self._loop.run_until_complete(asyncio.gather(*tasks, return_exceptions=True))
 
         if not self._loop.is_closed():
             self._loop.close()
             asyncio.set_event_loop(None)
 
     def _fetch_responses(self) -> Iterator[Response]:
         """Fetch responses concurrently.
@@ -216,15 +221,15 @@
                 # wait for the specific event to be set to preserve order of the resources
                 await event.wait()
 
                 # process next batch of tasks
                 self._process_batch(tasks)
 
                 # get response from the queue
-                i, response = await self._queue.get()
+                _, response = await self._queue.get()
 
                 # process next batch of tasks
                 self._process_batch(tasks)
 
                 yield response
                 self._queue.task_done()
                 self.pending -= 1
```

### Comparing `mure-1.0.0a0/mure/logging.py` & `mure-1.0.0a3/mure/logging.py`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a0/tests/test_mure.py` & `mure-1.0.0a3/tests/test_mure.py`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a0/.gitignore` & `mure-1.0.0a3/.gitignore`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a0/LICENSE` & `mure-1.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a0/README.md` & `mure-1.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a0/pyproject.toml` & `mure-1.0.0a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mure"
-version = "1.0.0a0"
+version = "1.0.0a3"
 description = "Perform multiple HTTP requests in parallel – without writing boilerplate code or worrying about async functions."
 authors = [{ name = "Severin Simmler", email = "s.simmler@snapaddy.com" }]
 dependencies = ["aiohttp>=3.9.3", "chardet>=5.2.0"]
 readme = "README.md"
 requires-python = ">= 3.11"
 
 [build-system]
```

### Comparing `mure-1.0.0a0/PKG-INFO` & `mure-1.0.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mure
-Version: 1.0.0a0
+Version: 1.0.0a3
 Summary: Perform multiple HTTP requests in parallel – without writing boilerplate code or worrying about async functions.
 Author-email: Severin Simmler <s.simmler@snapaddy.com>
 License-File: LICENSE
 Requires-Python: >=3.11
 Requires-Dist: aiohttp>=3.9.3
 Requires-Dist: chardet>=5.2.0
 Description-Content-Type: text/markdown
```

