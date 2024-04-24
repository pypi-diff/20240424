# Comparing `tmp/mure-1.0.0a3.tar.gz` & `tmp/mure-1.0.0a4.tar.gz`

## Comparing `mure-1.0.0a3.tar` & `mure-1.0.0a4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 mure-1.0.0a3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 mure-1.0.0a3/requirements-dev.lock
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 mure-1.0.0a3/requirements.lock
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 mure-1.0.0a3/.github/workflows/main.yml
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 mure-1.0.0a3/examples/example.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mure-1.0.0a3/mure/__init__.py
--rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 mure-1.0.0a3/mure/core.py
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 mure-1.0.0a3/mure/dtos.py
--rw-r--r--   0        0        0     8732 2020-02-02 00:00:00.000000 mure-1.0.0a3/mure/iterator.py
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 mure-1.0.0a3/mure/logging.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 mure-1.0.0a3/tests/test_mure.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 mure-1.0.0a3/.gitignore
--rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 mure-1.0.0a3/LICENSE
--rw-r--r--   0        0        0     6526 2020-02-02 00:00:00.000000 mure-1.0.0a3/README.md
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 mure-1.0.0a3/pyproject.toml
--rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 mure-1.0.0a3/PKG-INFO
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 mure-1.0.0a4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 mure-1.0.0a4/requirements-dev.lock
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 mure-1.0.0a4/requirements.lock
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 mure-1.0.0a4/.github/workflows/main.yml
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 mure-1.0.0a4/examples/example.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 mure-1.0.0a4/mure/__init__.py
+-rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 mure-1.0.0a4/mure/core.py
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 mure-1.0.0a4/mure/dtos.py
+-rw-r--r--   0        0        0     8833 2020-02-02 00:00:00.000000 mure-1.0.0a4/mure/iterator.py
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 mure-1.0.0a4/mure/logging.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 mure-1.0.0a4/tests/test_mure.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 mure-1.0.0a4/.gitignore
+-rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 mure-1.0.0a4/LICENSE
+-rw-r--r--   0        0        0     6526 2020-02-02 00:00:00.000000 mure-1.0.0a4/README.md
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 mure-1.0.0a4/pyproject.toml
+-rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 mure-1.0.0a4/PKG-INFO
```

### Comparing `mure-1.0.0a3/requirements-dev.lock` & `mure-1.0.0a4/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a3/.github/workflows/main.yml` & `mure-1.0.0a4/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a3/examples/example.py` & `mure-1.0.0a4/examples/example.py`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a3/mure/core.py` & `mure-1.0.0a4/mure/core.py`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a3/mure/dtos.py` & `mure-1.0.0a4/mure/dtos.py`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a3/mure/iterator.py` & `mure-1.0.0a4/mure/iterator.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,15 +206,17 @@
         """Fetch responses concurrently.
 
         Yields
         ------
         Response
             The server's response.
         """
-        async with ClientSession() as session:
+        session = ClientSession()
+
+        try:
             # create tasks (lazy)
             tasks = self._create_tasks(session)
 
             # process first batch of tasks
             self._process_batch(tasks)
 
             for event in self._events:
@@ -229,14 +231,18 @@
 
                 # process next batch of tasks
                 self._process_batch(tasks)
 
                 yield response
                 self._queue.task_done()
                 self.pending -= 1
+        except GeneratorExit:
+            return
+        finally:
+            await session.close()
 
     async def _afetch(self, session: ClientSession, resource: HTTPResource) -> Response:
         """Perform a HTTP request.
 
         Parameters
         ----------
         session : ClientSession
```

### Comparing `mure-1.0.0a3/mure/logging.py` & `mure-1.0.0a4/mure/logging.py`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a3/tests/test_mure.py` & `mure-1.0.0a4/tests/test_mure.py`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a3/.gitignore` & `mure-1.0.0a4/.gitignore`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a3/LICENSE` & `mure-1.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a3/README.md` & `mure-1.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `mure-1.0.0a3/pyproject.toml` & `mure-1.0.0a4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "mure"
-version = "1.0.0a3"
+version = "1.0.0a4"
 description = "Perform multiple HTTP requests in parallel – without writing boilerplate code or worrying about async functions."
 authors = [{ name = "Severin Simmler", email = "s.simmler@snapaddy.com" }]
 dependencies = ["aiohttp>=3.9.3", "chardet>=5.2.0"]
 readme = "README.md"
-requires-python = ">= 3.11"
+requires-python = ">= 3.11, <= 3.12"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 managed = true
```

### Comparing `mure-1.0.0a3/PKG-INFO` & `mure-1.0.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.3
 Name: mure
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: Perform multiple HTTP requests in parallel – without writing boilerplate code or worrying about async functions.
 Author-email: Severin Simmler <s.simmler@snapaddy.com>
 License-File: LICENSE
-Requires-Python: >=3.11
+Requires-Python: <=3.12,>=3.11
 Requires-Dist: aiohttp>=3.9.3
 Requires-Dist: chardet>=5.2.0
 Description-Content-Type: text/markdown
 
 # mure
 
 [![downloads](https://static.pepy.tech/personalized-badge/mure?period=total&units=international_system&left_color=black&right_color=black&left_text=downloads)](https://pepy.tech/project/mure)
```

