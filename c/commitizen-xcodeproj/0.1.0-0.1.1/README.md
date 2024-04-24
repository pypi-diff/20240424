# Comparing `tmp/commitizen_xcodeproj-0.1.0.tar.gz` & `tmp/commitizen_xcodeproj-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commitizen_xcodeproj-0.1.0.tar", max compression
+gzip compressed data, was "commitizen_xcodeproj-0.1.1.tar", max compression
```

## Comparing `commitizen_xcodeproj-0.1.0.tar` & `commitizen_xcodeproj-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1088 2024-04-23 22:52:45.087323 commitizen_xcodeproj-0.1.0/LICENSE
--rw-r--r--   0        0        0     1458 2024-04-23 22:52:45.104238 commitizen_xcodeproj-0.1.0/README.md
--rw-r--r--   0        0        0      909 2024-04-23 22:52:45.108179 commitizen_xcodeproj-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-23 22:52:45.083167 commitizen_xcodeproj-0.1.0/src/commitizen_xcodeproj/__init__.py
--rw-r--r--   0        0        0     1310 2024-04-23 22:52:45.100557 commitizen_xcodeproj-0.1.0/src/commitizen_xcodeproj/xcodeproj_version_provider.py
--rw-r--r--   0        0        0     1831 1970-01-01 00:00:00.000000 commitizen_xcodeproj-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1088 2024-04-23 22:52:45.087323 commitizen_xcodeproj-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1458 2024-04-23 22:52:45.104238 commitizen_xcodeproj-0.1.1/README.md
+-rw-r--r--   0        0        0      909 2024-04-24 08:53:10.641117 commitizen_xcodeproj-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-23 22:52:45.083167 commitizen_xcodeproj-0.1.1/src/commitizen_xcodeproj/__init__.py
+-rw-r--r--   0        0        0     1310 2024-04-23 22:52:45.100557 commitizen_xcodeproj-0.1.1/src/commitizen_xcodeproj/xcodeproj_version_provider.py
+-rw-r--r--   0        0        0     1933 1970-01-01 00:00:00.000000 commitizen_xcodeproj-0.1.1/PKG-INFO
```

### Comparing `commitizen_xcodeproj-0.1.0/LICENSE` & `commitizen_xcodeproj-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `commitizen_xcodeproj-0.1.0/README.md` & `commitizen_xcodeproj-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `commitizen_xcodeproj-0.1.0/pyproject.toml` & `commitizen_xcodeproj-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "commitizen-xcodeproj"
-version = "0.1.0"
+version = "0.1.1"
 description = "Commitizen version provider for Xcode projects."
 authors = ["Karsten Silkenbäumer <993392+kassi@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "commitizen_xcodeproj", from = "src"}]
 
 [tool.poetry.dependencies]
-python = "^3.12"
+python = "^3.10"
 
 [tool.poetry.group.dev.dependencies]
 commitizen = "^3.24.0"
 pytest = "^8.1.1"
 pytest-watcher = "^0.4.2"
 pytest-mock = "^3.14.0"
```

### Comparing `commitizen_xcodeproj-0.1.0/src/commitizen_xcodeproj/xcodeproj_version_provider.py` & `commitizen_xcodeproj-0.1.1/src/commitizen_xcodeproj/xcodeproj_version_provider.py`

 * *Files identical despite different names*

### Comparing `commitizen_xcodeproj-0.1.0/PKG-INFO` & `commitizen_xcodeproj-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: commitizen-xcodeproj
-Version: 0.1.0
+Version: 0.1.1
 Summary: Commitizen version provider for Xcode projects.
 Author: Karsten Silkenbäumer
 Author-email: 993392+kassi@users.noreply.github.com
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 # Commitizen Xcode Project Version Provider
 
 A commitizen version provider for Xcode project files, which store the version in the `MARKETING_VERSION` field.
```

