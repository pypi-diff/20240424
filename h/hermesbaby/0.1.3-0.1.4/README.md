# Comparing `tmp/hermesbaby-0.1.3.tar.gz` & `tmp/hermesbaby-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermesbaby-0.1.3.tar", max compression
+gzip compressed data, was "hermesbaby-0.1.4.tar", max compression
```

## Comparing `hermesbaby-0.1.3.tar` & `hermesbaby-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      117 2024-04-22 04:05:52.750497 hermesbaby-0.1.3/AUTHORS.rst
--rw-r--r--   0        0        0     1104 2024-04-22 04:07:33.370496 hermesbaby-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0      454 2024-04-24 04:32:01.252082 hermesbaby-0.1.3/README.md
--rw-r--r--   0        0        0      737 2024-04-24 04:44:33.740053 hermesbaby-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        1 2024-04-22 04:34:17.510486 hermesbaby-0.1.3/src/hermesbaby/__init__.py
--rw-r--r--   0        0        0      269 2024-04-23 04:06:33.843538 hermesbaby-0.1.3/src/hermesbaby/cli.py
--rw-r--r--   0        0        0        0 2024-04-24 04:30:38.840085 hermesbaby-0.1.3/src/hermesbaby/cmd/__init_.py
--rw-r--r--   0        0        0      269 2024-04-24 04:30:38.852085 hermesbaby-0.1.3/src/hermesbaby/cmd/hb.py
--rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 hermesbaby-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      117 2024-04-22 04:05:52.750497 hermesbaby-0.1.4/AUTHORS.rst
+-rw-r--r--   0        0        0     1104 2024-04-22 04:07:33.370496 hermesbaby-0.1.4/LICENSE.txt
+-rw-r--r--   0        0        0      691 2024-04-24 04:55:31.172027 hermesbaby-0.1.4/README.md
+-rw-r--r--   0        0        0      737 2024-04-24 04:55:57.872026 hermesbaby-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        1 2024-04-22 04:34:17.510486 hermesbaby-0.1.4/src/hermesbaby/__init__.py
+-rw-r--r--   0        0        0      269 2024-04-23 04:06:33.843538 hermesbaby-0.1.4/src/hermesbaby/cli.py
+-rw-r--r--   0        0        0        0 2024-04-24 04:30:38.840085 hermesbaby-0.1.4/src/hermesbaby/cmd/__init_.py
+-rw-r--r--   0        0        0      269 2024-04-24 04:30:38.852085 hermesbaby-0.1.4/src/hermesbaby/cmd/hb.py
+-rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 hermesbaby-0.1.4/PKG-INFO
```

### Comparing `hermesbaby-0.1.3/LICENSE.txt` & `hermesbaby-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hermesbaby-0.1.3/pyproject.toml` & `hermesbaby-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hermesbaby"
-version = "0.1.3"
+version = "0.1.4"
 description = "The Software Engineers' Typewriter"
 authors = ["Alexander Mann-Wahrenberg (basejumpa) <alexander.mannwahrenberg@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `hermesbaby-0.1.3/PKG-INFO` & `hermesbaby-0.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hermesbaby
-Version: 0.1.3
+Version: 0.1.4
 Summary: The Software Engineers' Typewriter
 License: MIT
 Author: Alexander Mann-Wahrenberg (basejumpa)
 Author-email: alexander.mannwahrenberg@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -36,7 +36,19 @@
     pipx install hermesbaby
     hermesbaby new MyNewProject
     cd MyNewProject
     hermesbaby preview
     # Start editing ./docs/index.rst ...
 ```
 
+See what's possible
+===================
+
+.. code-block:: bash
+
+    cd
+    hermesbaby new SeeWhatsPossible --template showcase
+    cd SeeWhatsPossible
+    hermesbaby preview
+    # Investigate preview in browser and sources in editor
+```
+
```

