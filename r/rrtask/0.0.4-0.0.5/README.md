# Comparing `tmp/rrtask-0.0.4.tar.gz` & `tmp/rrtask-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rrtask-0.0.4.tar", max compression
+gzip compressed data, was "rrtask-0.0.5.tar", max compression
```

## Comparing `rrtask-0.0.4.tar` & `rrtask-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1063 2024-04-23 08:17:03.738389 rrtask-0.0.4/LICENSE
--rw-r--r--   0        0        0      210 2024-04-24 08:52:17.584490 rrtask-0.0.4/README.md
--rw-r--r--   0        0        0      605 2024-04-24 09:05:31.069223 rrtask-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      133 2024-04-24 09:02:58.172982 rrtask-0.0.4/rrtask/__init__.py
--rw-r--r--   0        0        0      171 2024-04-24 08:30:19.015153 rrtask-0.0.4/rrtask/enums.py
--rw-r--r--   0        0        0     5621 2024-04-24 08:56:57.928565 rrtask-0.0.4/rrtask/rrtask.py
--rw-r--r--   0        0        0      394 2024-04-24 08:50:30.008555 rrtask-0.0.4/rrtask/signals.py
--rw-r--r--   0        0        0      298 2024-04-24 08:50:30.008555 rrtask-0.0.4/rrtask/utils.py
--rw-r--r--   0        0        0       18 2024-04-24 09:05:34.229229 rrtask-0.0.4/rrtask/version.py
--rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 rrtask-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-23 08:17:03.738389 rrtask-0.0.5/LICENSE
+-rw-r--r--   0        0        0      210 2024-04-24 08:52:17.584490 rrtask-0.0.5/README.md
+-rw-r--r--   0        0        0      581 2024-04-24 09:12:48.294029 rrtask-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      133 2024-04-24 09:02:58.172982 rrtask-0.0.5/rrtask/__init__.py
+-rw-r--r--   0        0        0      171 2024-04-24 08:30:19.015153 rrtask-0.0.5/rrtask/enums.py
+-rw-r--r--   0        0        0     5621 2024-04-24 08:56:57.928565 rrtask-0.0.5/rrtask/rrtask.py
+-rw-r--r--   0        0        0      394 2024-04-24 08:50:30.008555 rrtask-0.0.5/rrtask/signals.py
+-rw-r--r--   0        0        0      298 2024-04-24 08:50:30.008555 rrtask-0.0.5/rrtask/utils.py
+-rw-r--r--   0        0        0       18 2024-04-24 09:12:50.010033 rrtask-0.0.5/rrtask/version.py
+-rw-r--r--   0        0        0      701 1970-01-01 00:00:00.000000 rrtask-0.0.5/PKG-INFO
```

### Comparing `rrtask-0.0.4/LICENSE` & `rrtask-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rrtask-0.0.4/pyproject.toml` & `rrtask-0.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [tool.poetry]
 name = "rrtask"
-version = "0.0.4"
+version = "0.0.5"
 description = "Round Robin Task"
 authors = ["François Schmidts <francois@schmidts.fr>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "3.7.*"
-celery = "4.4.7"
-redis = "2.10.5"
-pyrabbit = "1.1.0"
-threaded-context = "==1.*"
+python = "==3.7.*"
+celery = "==4.4.*"
+redis = "==2.*"
+pyrabbit = "==1.*"
 blinker = "==1.*"
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 isort = "*"
 ipdb = "*"
 pylint = "*"
```

### Comparing `rrtask-0.0.4/rrtask/rrtask.py` & `rrtask-0.0.5/rrtask/rrtask.py`

 * *Files identical despite different names*

### Comparing `rrtask-0.0.4/PKG-INFO` & `rrtask-0.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: rrtask
-Version: 0.0.4
+Version: 0.0.5
 Summary: Round Robin Task
 License: MIT
 Author: François Schmidts
 Author-email: francois@schmidts.fr
 Requires-Python: ==3.7.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Dist: blinker (==1.*)
-Requires-Dist: celery (==4.4.7)
-Requires-Dist: pyrabbit (==1.1.0)
-Requires-Dist: redis (==2.10.5)
-Requires-Dist: threaded-context (==1.*)
+Requires-Dist: celery (==4.4.*)
+Requires-Dist: pyrabbit (==1.*)
+Requires-Dist: redis (==2.*)
 Description-Content-Type: text/markdown
 
 # Basic Usage
 
 ```python3
 >>> import rrtask
 ```
```

