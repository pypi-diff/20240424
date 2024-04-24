# Comparing `tmp/gearsllm-0.1.8.tar.gz` & `tmp/gearsllm-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gearsllm-0.1.8.tar", max compression
+gzip compressed data, was "gearsllm-0.1.9.tar", max compression
```

## Comparing `gearsllm-0.1.8.tar` & `gearsllm-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1062 2023-07-22 21:52:20.719532 gearsllm-0.1.8/LICENSE
--rw-r--r--   0        0        0      318 2023-07-23 22:37:37.759113 gearsllm-0.1.8/README.md
--rw-r--r--   0        0        0      141 2023-07-23 22:07:23.763584 gearsllm-0.1.8/gears/__init__.py
--rw-r--r--   0        0        0     2108 2023-07-25 17:57:17.857188 gearsllm-0.1.8/gears/gear.py
--rw-r--r--   0        0        0     2592 2023-07-24 03:10:17.813919 gearsllm-0.1.8/gears/history.py
--rw-r--r--   0        0        0      141 2023-07-25 19:38:23.801725 gearsllm-0.1.8/gears/llms/__init__.py
--rw-r--r--   0        0        0      234 2023-07-23 07:06:32.890807 gearsllm-0.1.8/gears/llms/base.py
--rw-r--r--   0        0        0      930 2023-07-23 22:12:06.460243 gearsllm-0.1.8/gears/llms/echo.py
--rw-r--r--   0        0        0     5556 2023-07-25 19:40:27.492346 gearsllm-0.1.8/gears/llms/oai.py
--rw-r--r--   0        0        0     1307 2023-07-23 22:33:03.565128 gearsllm-0.1.8/gears/utils.py
--rw-r--r--   0        0        0      676 2023-07-25 19:41:27.026735 gearsllm-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 gearsllm-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-22 21:52:20.719532 gearsllm-0.1.9/LICENSE
+-rw-r--r--   0        0        0      318 2023-07-23 22:37:37.759113 gearsllm-0.1.9/README.md
+-rw-r--r--   0        0        0      141 2023-07-23 22:07:23.763584 gearsllm-0.1.9/gears/__init__.py
+-rw-r--r--   0        0        0     2384 2023-07-25 20:00:01.439998 gearsllm-0.1.9/gears/gear.py
+-rw-r--r--   0        0        0     2592 2023-07-24 03:10:17.813919 gearsllm-0.1.9/gears/history.py
+-rw-r--r--   0        0        0      141 2023-07-25 19:38:23.801725 gearsllm-0.1.9/gears/llms/__init__.py
+-rw-r--r--   0        0        0      234 2023-07-23 07:06:32.890807 gearsllm-0.1.9/gears/llms/base.py
+-rw-r--r--   0        0        0      930 2023-07-23 22:12:06.460243 gearsllm-0.1.9/gears/llms/echo.py
+-rw-r--r--   0        0        0     5556 2023-07-25 19:40:27.492346 gearsllm-0.1.9/gears/llms/oai.py
+-rw-r--r--   0        0        0     1307 2023-07-23 22:33:03.565128 gearsllm-0.1.9/gears/utils.py
+-rw-r--r--   0        0        0      676 2023-07-25 20:01:59.734651 gearsllm-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 gearsllm-0.1.9/PKG-INFO
```

### Comparing `gearsllm-0.1.8/LICENSE` & `gearsllm-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.8/gears/gear.py` & `gearsllm-0.1.9/gears/gear.py`

 * *Files 20% similar despite different names*

```diff
@@ -54,15 +54,22 @@
                 )
         except NotImplementedError:
             pass
 
         # Load which other gear to run, if any
         try:
             child = self.switch(response)
-            return await child.run(response, history, **kwargs)
+            if isinstance(child, Gear):
+                return await child.run(response, history, **kwargs)
+            elif not child:
+                logger.info("No child gear to run. Returning response.")
+                return response
+            else:
+                raise TypeError(f"Switch must return a Gear instance or None.")
+
         except NotImplementedError:
             pass
 
         # If there is no child, return the response
         return response
 
     def template(self) -> str:
```

### Comparing `gearsllm-0.1.8/gears/history.py` & `gearsllm-0.1.9/gears/history.py`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.8/gears/llms/echo.py` & `gearsllm-0.1.9/gears/llms/echo.py`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.8/gears/llms/oai.py` & `gearsllm-0.1.9/gears/llms/oai.py`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.8/gears/utils.py` & `gearsllm-0.1.9/gears/utils.py`

 * *Files identical despite different names*

### Comparing `gearsllm-0.1.8/pyproject.toml` & `gearsllm-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gearsllm"
-version = "0.1.8"
+version = "0.1.9"
 description = "Lightweight library for building LLM-based control flow."
 authors = ["Shreya Shankar <ss.shankar505@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "gears"}]
 
 [tool.poetry.dependencies]
```

### Comparing `gearsllm-0.1.8/PKG-INFO` & `gearsllm-0.1.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gearsllm
-Version: 0.1.8
+Version: 0.1.9
 Summary: Lightweight library for building LLM-based control flow.
 License: MIT
 Author: Shreya Shankar
 Author-email: ss.shankar505@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

