# Comparing `tmp/temper_std-0.2.0.tar.gz` & `tmp/temper_std-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temper_std-0.2.0.tar", max compression
+gzip compressed data, was "temper_std-0.2.1.tar", max compression
```

## Comparing `temper_std-0.2.0.tar` & `temper_std-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      998 2024-04-18 16:39:36.052472 temper_std-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       95 2024-04-18 16:39:36.022472 temper_std-0.2.0/temper_std/__init__.py
--rw-r--r--   0        0        0      106 2024-04-18 16:39:36.032472 temper_std-0.2.0/temper_std/__init__.py.map
--rw-r--r--   0        0        0    28586 2024-04-18 16:39:36.422473 temper_std-0.2.0/temper_std/regex.py
--rw-r--r--   0        0        0    50476 2024-04-18 16:39:36.452473 temper_std-0.2.0/temper_std/regex.py.map
--rw-r--r--   0        0        0     1974 2024-04-18 16:39:36.112473 temper_std-0.2.0/temper_std/temporal.py
--rw-r--r--   0        0        0     7395 2024-04-18 16:39:36.112473 temper_std-0.2.0/temper_std/temporal.py.map
--rw-r--r--   0        0        0     7174 2024-04-18 16:39:36.192473 temper_std-0.2.0/temper_std/testing.py
--rw-r--r--   0        0        0    14155 2024-04-18 16:39:36.222473 temper_std-0.2.0/temper_std/testing.py.map
--rw-r--r--   0        0        0      651 1970-01-01 00:00:00.000000 temper_std-0.2.0/setup.py
--rw-r--r--   0        0        0      632 1970-01-01 00:00:00.000000 temper_std-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      998 2024-04-23 22:22:20.795323 temper_std-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       95 2024-04-23 22:22:20.805323 temper_std-0.2.1/temper_std/__init__.py
+-rw-r--r--   0        0        0      106 2024-04-23 22:22:20.805323 temper_std-0.2.1/temper_std/__init__.py.map
+-rw-r--r--   0        0        0    28586 2024-04-23 22:22:22.875323 temper_std-0.2.1/temper_std/regex.py
+-rw-r--r--   0        0        0    50476 2024-04-23 22:22:23.085323 temper_std-0.2.1/temper_std/regex.py.map
+-rw-r--r--   0        0        0     1974 2024-04-23 22:22:21.305323 temper_std-0.2.1/temper_std/temporal.py
+-rw-r--r--   0        0        0     7395 2024-04-23 22:22:21.425323 temper_std-0.2.1/temper_std/temporal.py.map
+-rw-r--r--   0        0        0     7174 2024-04-23 22:22:21.635323 temper_std-0.2.1/temper_std/testing.py
+-rw-r--r--   0        0        0    14155 2024-04-23 22:22:21.935323 temper_std-0.2.1/temper_std/testing.py.map
+-rw-r--r--   0        0        0      651 1970-01-01 00:00:00.000000 temper_std-0.2.1/setup.py
+-rw-r--r--   0        0        0      632 1970-01-01 00:00:00.000000 temper_std-0.2.1/PKG-INFO
```

### Comparing `temper_std-0.2.0/pyproject.toml` & `temper_std-0.2.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 [project]
 name = "temper-std"
-version = "0.2.0"
+version = "0.2.1"
 description = "Optional support library provided with Temper"
 readme = ""
 requires-python = "~=3.8"
 license = {text = "Apache-2.0"}
 authors = [ "Temper Contributors" ]
 homepage = "https://temperlang.dev/"
 repository = "https://github.com/temperlang/temper"
 maintainers = [ ]
 keywords = [ ]
 classifiers = [ ]
 urls = { }
 dependencies = [
-    "temper-core == 0.2.0"
+    "temper-core == 0.2.1"
 ]
 
 [project.scripts]
 
 [project.gui-scripts]
 
 [project.entry-points]
 
 
 [tool.poetry]
 name = "temper-std"
-version = "0.2.0"
+version = "0.2.1"
 license = "Apache-2.0"
 description = "Optional support library provided with Temper"
 authors = [ "Temper Contributors" ]
 homepage = "https://temperlang.dev/"
 repository = "https://github.com/temperlang/temper"
 packages = [{ include = "temper_std" }]
 include = ["temper_std/**/*", "./**/*.pyd", "./**/*.so"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-temper-core = "0.2.0"
+temper-core = "0.2.1"
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `temper_std-0.2.0/temper_std/regex.py` & `temper_std-0.2.1/temper_std/regex.py`

 * *Files identical despite different names*

### Comparing `temper_std-0.2.0/temper_std/regex.py.map` & `temper_std-0.2.1/temper_std/regex.py.map`

 * *Files identical despite different names*

### Comparing `temper_std-0.2.0/temper_std/temporal.py` & `temper_std-0.2.1/temper_std/temporal.py`

 * *Files identical despite different names*

### Comparing `temper_std-0.2.0/temper_std/temporal.py.map` & `temper_std-0.2.1/temper_std/temporal.py.map`

 * *Files identical despite different names*

### Comparing `temper_std-0.2.0/temper_std/testing.py` & `temper_std-0.2.1/temper_std/testing.py`

 * *Files identical despite different names*

### Comparing `temper_std-0.2.0/temper_std/testing.py.map` & `temper_std-0.2.1/temper_std/testing.py.map`

 * *Files identical despite different names*

### Comparing `temper_std-0.2.0/setup.py` & `temper_std-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['temper_std']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['temper-core==0.2.0']
+['temper-core==0.2.1']
 
 setup_kwargs = {
     'name': 'temper-std',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Optional support library provided with Temper',
     'long_description': 'None',
     'author': 'Temper Contributors',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://temperlang.dev/',
```

### Comparing `temper_std-0.2.0/PKG-INFO` & `temper_std-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: temper-std
-Version: 0.2.0
+Version: 0.2.1
 Summary: Optional support library provided with Temper
 Home-page: https://temperlang.dev/
 License: Apache-2.0
 Author: Temper Contributors
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: temper-core (==0.2.0)
+Requires-Dist: temper-core (==0.2.1)
 Project-URL: Repository, https://github.com/temperlang/temper
```

