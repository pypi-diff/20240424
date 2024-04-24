# Comparing `tmp/pyrobird-0.0.1.tar.gz` & `tmp/pyrobird-0.0.2.tar.gz`

## Comparing `pyrobird-0.0.1.tar` & `pyrobird-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0      122 2020-02-02 00:00:00.000000 pyrobird-0.0.1/src/pyrobird/__about__.py
--rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 pyrobird-0.0.1/src/pyrobird/__init__.py
--rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 pyrobird-0.0.1/src/pyrobird/__main__.py
--rwxr-xr-x   0        0        0      371 2020-02-02 00:00:00.000000 pyrobird-0.0.1/src/pyrobird/cli/__init__.py
--rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 pyrobird-0.0.1/tests/__init__.py
--rwxr-xr-x   0        0        0     2177 2020-02-02 00:00:00.000000 pyrobird-0.0.1/.gitignore
--rwxr-xr-x   0        0        0     7651 2020-02-02 00:00:00.000000 pyrobird-0.0.1/LICENSE.LGPL3.txt
--rwxr-xr-x   0        0        0      478 2020-02-02 00:00:00.000000 pyrobird-0.0.1/README.md
--rwxr-xr-x   0        0        0     1941 2020-02-02 00:00:00.000000 pyrobird-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 pyrobird-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0      122 2020-02-02 00:00:00.000000 pyrobird-0.0.2/src/pyrobird/__about__.py
+-rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 pyrobird-0.0.2/src/pyrobird/__init__.py
+-rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 pyrobird-0.0.2/src/pyrobird/__main__.py
+-rwxr-xr-x   0        0        0      366 2020-02-02 00:00:00.000000 pyrobird-0.0.2/src/pyrobird/cli/__init__.py
+-rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 pyrobird-0.0.2/tests/__init__.py
+-rwxr-xr-x   0        0        0     2177 2020-02-02 00:00:00.000000 pyrobird-0.0.2/.gitignore
+-rwxr-xr-x   0        0        0     7651 2020-02-02 00:00:00.000000 pyrobird-0.0.2/LICENSE.txt
+-rwxr-xr-x   0        0        0      478 2020-02-02 00:00:00.000000 pyrobird-0.0.2/README.md
+-rwxr-xr-x   0        0        0     2071 2020-02-02 00:00:00.000000 pyrobird-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 pyrobird-0.0.2/PKG-INFO
```

### Comparing `pyrobird-0.0.1/.gitignore` & `pyrobird-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyrobird-0.0.1/LICENSE.LGPL3.txt` & `pyrobird-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyrobird-0.0.1/pyproject.toml` & `pyrobird-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 [project]
 name = "pyrobird"
 dynamic = ["version"]
 description = ''
 readme = "README.md"
 requires-python = ">=3.8"
-license = "MIT"
+license = "LGPL-3.0-or-later"
 keywords = []
 authors = [
-  { name = "U.N. Owen", email = "void@some.where" },
+  { name = "Dmitry Romanov", email = "romanovda@gmail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
@@ -25,20 +25,20 @@
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "click",
 ]
 
 [project.urls]
-Documentation = "https://github.com/unknown/pyrobird#readme"
-Issues = "https://github.com/unknown/pyrobird/issues"
-Source = "https://github.com/unknown/pyrobird"
+Documentation = "https://github.com/eic/firebird#readme"
+Issues = "https://github.com/eic/firebird/issues"
+Source = "https://github.com/eic/firebird"
 
 [project.scripts]
-pyrobird = "pyrobird.cli:pyrobird"
+fbd = "pyrobird.cli:pyrobird"
 
 [tool.hatch.version]
 path = "src/pyrobird/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
@@ -80,7 +80,15 @@
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
+
+[tool.hatch.publish.index]
+disable = true
+
+[tool.hatch.publish.index.repos.main]
+url = "https://upload.pypi.org/legacy/"
+
+
```

### Comparing `pyrobird-0.0.1/PKG-INFO` & `pyrobird-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.3
 Name: pyrobird
-Version: 0.0.1
-Project-URL: Documentation, https://github.com/unknown/pyrobird#readme
-Project-URL: Issues, https://github.com/unknown/pyrobird/issues
-Project-URL: Source, https://github.com/unknown/pyrobird
-Author-email: "U.N. Owen" <void@some.where>
-License-Expression: MIT
-License-File: LICENSE.LGPL3.txt
+Version: 0.0.2
+Project-URL: Documentation, https://github.com/eic/firebird#readme
+Project-URL: Issues, https://github.com/eic/firebird/issues
+Project-URL: Source, https://github.com/eic/firebird
+Author-email: Dmitry Romanov <romanovda@gmail.com>
+License-Expression: LGPL-3.0-or-later
+License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

