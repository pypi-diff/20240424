# Comparing `tmp/dynafile-0.1.2.tar.gz` & `tmp/dynafile-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynafile-0.1.2.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `dynafile-0.1.2.tar` & `dynafile-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,22 @@
--rw-r--r--   0        0        0     1071 2021-09-26 22:04:03.907067 dynafile-0.1.2/LICENSE
--rw-r--r--   0        0        0     3808 2022-04-27 05:42:29.850435 dynafile-0.1.2/README.md
--rw-r--r--   0        0        0     9949 2022-04-27 19:22:52.787671 dynafile-0.1.2/dynafile/__init__.py
--rw-r--r--   0        0        0      580 2022-04-27 05:09:08.592523 dynafile-0.1.2/dynafile/dispatcher.py
--rw-r--r--   0        0        0     1408 2022-04-27 19:24:59.093850 dynafile-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4806 2022-04-27 19:27:05.165961 dynafile-0.1.2/setup.py
--rw-r--r--   0        0        0     5064 2022-04-27 19:27:05.166367 dynafile-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 dynafile-0.1.3/.python-version
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 dynafile-0.1.3/DEVELOPMENT.md
+-rw-r--r--   0        0        0    49033 2020-02-02 00:00:00.000000 dynafile-0.1.3/architecture.png
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 dynafile-0.1.3/architecture.puml
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 dynafile-0.1.3/pytest.ini
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 dynafile-0.1.3/requirements-dev.lock
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 dynafile-0.1.3/requirements.lock
+-rw-r--r--   0        0        0     9953 2020-02-02 00:00:00.000000 dynafile-0.1.3/src/dynafile/__init__.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 dynafile-0.1.3/src/dynafile/dispatcher.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dynafile-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 dynafile-0.1.3/tests/test_deletion.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 dynafile-0.1.3/tests/test_event_hooks.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 dynafile-0.1.3/tests/test_peformance.py
+-rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 dynafile-0.1.3/tests/test_query.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 dynafile-0.1.3/tests/test_scan.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 dynafile-0.1.3/tests/test_store_and_load.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 dynafile-0.1.3/tests/test_ttl.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 dynafile-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 dynafile-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3856 2020-02-02 00:00:00.000000 dynafile-0.1.3/README.md
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 dynafile-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5095 2020-02-02 00:00:00.000000 dynafile-0.1.3/PKG-INFO
```

### Comparing `dynafile-0.1.2/LICENSE` & `dynafile-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dynafile-0.1.2/README.md` & `dynafile-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -45,25 +45,25 @@
 - batch writer
 - atomic file write
 - event stream hooks (put, delete)
 - TTL
 
 ## Roadmap
 
-- GSI - global secondary index
-- update item
-- batch get
-- thread safeness
-- LSI - local secondary index
-- split partitions
-- parallel scans - pre defined scan segments
-- transactions
-- optimise disc load time (cache partitions in memory, invalidate on file change)
-- conditional put item
-- improve file consistency (options: acidfile)
+- [ ] GSI - global secondary index
+- [ ] update item
+- [ ] batch get
+- [ ] thread safeness
+- [ ] ~~LSI - local secondary index~~
+- [ ] split partitions
+- [ ] parallel scans - pre defined scan segments
+- [ ] transactions
+- [ ] optimise disc load time (cache partitions in memory, invalidate on file change)
+- [ ] conditional put item
+- [ ] improve file consistency (options: acidfile)
 
 ## API
 
 ```python
 from dynafile import *
 
 # init DB interface
```

### Comparing `dynafile-0.1.2/dynafile/__init__.py` & `dynafile-0.1.3/src/dynafile/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,15 +307,15 @@
                 yield item
 
     def __parse_filter(self, _filter: Optional[Filter]) -> Callable:
         if _filter is None:
             return bool
         elif callable(_filter):
             return _filter
-        elif type(_filter) is str:
+        elif isinstance(_filter, str):
             try:
                 import filtration
 
                 return filtration.Expression.parseString(_filter)
             except ImportError as e:
                 raise Exception(
                     "String filter expressions only available if `filtration` is installed."
```

### Comparing `dynafile-0.1.2/dynafile/dispatcher.py` & `dynafile-0.1.3/src/dynafile/dispatcher.py`

 * *Files identical despite different names*

### Comparing `dynafile-0.1.2/pyproject.toml` & `dynafile-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-[tool.poetry]
+[project]
 name = "dynafile"
-version = "0.1.2"
+version = "0.1.3"
 description = "NoSQLDB following the Dynamo concept, but for a filebased embedded db."
-authors = ["Maic Siemering <maic@siemering.tech>"]
+authors = [{name = "Maic Siemering", email = "maic@siemering.tech"}]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/eruvanos/dynafile"
 keywords = ["database", "nosql"]
 
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -15,35 +15,47 @@
     "License :: OSI Approved :: MIT License",
     "Topic :: Database",
     "Topic :: Utilities",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Operating System :: OS Independent",
     "Typing :: Typed",
 ]
 
-packages = [
-    { include = "dynafile" }
+dependencies = [
+    "sortedcontainers>=2.4.0",
+    "atomicwrites>=1.4.1",
 ]
+requires-python = ">= 3.8"
+
+[project.optional-dependencies]
+filter = [
+    "filtration>=2.3.0",
+]
+
+[tool.rye.scripts]
 
-[tool.poetry.dependencies]
-python = "^3.8"
-sortedcontainers = "^2.4.0"
-atomicwrites = "^1.4.0"
-filtration = {version = "^2.3.0", optional = true}
-
-[tool.poetry.extras]
-filter = ["filtration"]
-
-[tool.poetry.dev-dependencies]
-pytest = "^7.1.2"
-pytest-benchmark = "^3.4.1"
-time-machine = "^2.6.0"
-black = {version = "^22.3.0", optional = true}
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[tool.rye]
+managed = true
+dev-dependencies = [
+    "pytest>=8.1.1",
+    "pytest-benchmark>=4.0.0",
+    "time-machine>=2.14.1",
+    "ruff>=0.4.1",
+]
+
+[tool.hatch.metadata]
+allow-direct-references = true
+
+[tool.hatch.build.targets.wheel]
+packages = ["src/dynafile"]
```

### Comparing `dynafile-0.1.2/PKG-INFO` & `dynafile-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: dynafile
-Version: 0.1.2
+Version: 0.1.3
 Summary: NoSQLDB following the Dynamo concept, but for a filebased embedded db.
-Home-page: https://github.com/eruvanos/dynafile
-License: MIT
+Author-email: Maic Siemering <maic@siemering.tech>
+License-Expression: MIT
+License-File: LICENSE
 Keywords: database,nosql
-Author: Maic Siemering
-Author-email: maic@siemering.tech
-Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Database
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
+Requires-Python: >=3.8
+Requires-Dist: atomicwrites>=1.4.1
+Requires-Dist: sortedcontainers>=2.4.0
 Provides-Extra: filter
-Requires-Dist: atomicwrites (>=1.4.0,<2.0.0)
-Requires-Dist: filtration (>=2.3.0,<3.0.0); extra == "filter"
-Requires-Dist: sortedcontainers (>=2.4.0,<3.0.0)
-Project-URL: Repository, https://github.com/eruvanos/dynafile
+Requires-Dist: filtration>=2.3.0; extra == 'filter'
 Description-Content-Type: text/markdown
 
 > Consider the project as a proof of concept! Definitely not production ready!
 
 # Dynafile
 
 Embedded pure Python NoSQL database following DynamoDB concepts.
@@ -76,25 +76,25 @@
 - batch writer
 - atomic file write
 - event stream hooks (put, delete)
 - TTL
 
 ## Roadmap
 
-- GSI - global secondary index
-- update item
-- batch get
-- thread safeness
-- LSI - local secondary index
-- split partitions
-- parallel scans - pre defined scan segments
-- transactions
-- optimise disc load time (cache partitions in memory, invalidate on file change)
-- conditional put item
-- improve file consistency (options: acidfile)
+- [ ] GSI - global secondary index
+- [ ] update item
+- [ ] batch get
+- [ ] thread safeness
+- [ ] ~~LSI - local secondary index~~
+- [ ] split partitions
+- [ ] parallel scans - pre defined scan segments
+- [ ] transactions
+- [ ] optimise disc load time (cache partitions in memory, invalidate on file change)
+- [ ] conditional put item
+- [ ] improve file consistency (options: acidfile)
 
 ## API
 
 ```python
 from dynafile import *
 
 # init DB interface
@@ -195,8 +195,8 @@
 
 --- GSI ---
 |- _gsi-<gsi-name>/
     |- _partitions/
         |- <hash>/
             |- data.pickle - Contains partition data by sort key (SortedDict)
 
-```
+```
```

