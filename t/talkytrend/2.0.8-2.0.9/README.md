# Comparing `tmp/talkytrend-2.0.8.tar.gz` & `tmp/talkytrend-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-2.0.8.tar", max compression
+gzip compressed data, was "talkytrend-2.0.9.tar", max compression
```

## Comparing `talkytrend-2.0.8.tar` & `talkytrend-2.0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2024-03-28 21:10:01.095648 talkytrend-2.0.8/LICENSE
--rw-r--r--   0        0        0     2941 2024-03-28 21:10:01.095648 talkytrend-2.0.8/README.md
--rw-r--r--   0        0        0     3690 2024-03-28 21:10:24.967872 talkytrend-2.0.8/pyproject.toml
--rw-r--r--   0        0        0      116 2024-03-28 21:10:24.967872 talkytrend-2.0.8/talkytrend/__init__.py
--rw-r--r--   0        0        0      724 2024-03-28 21:10:01.099648 talkytrend-2.0.8/talkytrend/config.py
--rw-r--r--   0        0        0     1922 2024-03-28 21:10:01.099648 talkytrend-2.0.8/talkytrend/default_settings.toml
--rw-r--r--   0        0        0    12076 2024-03-28 21:10:01.099648 talkytrend-2.0.8/talkytrend/main.py
--rw-r--r--   0        0        0     4075 1970-01-01 00:00:00.000000 talkytrend-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-17 04:28:15.092200 talkytrend-2.0.9/LICENSE
+-rw-r--r--   0        0        0     2941 2024-04-17 04:28:15.092200 talkytrend-2.0.9/README.md
+-rw-r--r--   0        0        0     3692 2024-04-17 04:28:39.112408 talkytrend-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0      116 2024-04-17 04:28:39.112408 talkytrend-2.0.9/talkytrend/__init__.py
+-rw-r--r--   0        0        0      724 2024-04-17 04:28:15.096200 talkytrend-2.0.9/talkytrend/config.py
+-rw-r--r--   0        0        0     1922 2024-04-17 04:28:15.096200 talkytrend-2.0.9/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0    12076 2024-04-17 04:28:15.096200 talkytrend-2.0.9/talkytrend/main.py
+-rw-r--r--   0        0        0     4075 1970-01-01 00:00:00.000000 talkytrend-2.0.9/PKG-INFO
```

### Comparing `talkytrend-2.0.8/LICENSE` & `talkytrend-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-2.0.8/README.md` & `talkytrend-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `talkytrend-2.0.8/pyproject.toml` & `talkytrend-2.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "talkytrend"
-version = "2.0.8"
+version = "2.0.9"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
@@ -96,14 +96,15 @@
 
 
 
 
 
 
 
+
 [tool.poetry.group.test.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.23.0"
 pytest-mock = "^3.11.1"
 pytest-loguru = "^0.3.0"
 
@@ -141,19 +142,20 @@
 
 
 
 
 
 
 
+
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "7.2.6"
+sphinx = "7.3.1"
 pydata-sphinx-theme = "^0.15.0"
 sphinx-hoverxref = "^1.3.0"
 sphinx_design = "^0.5.0"
 sphinx_copybutton = "^0.5.2"
 myst_parser = "^2.0.0"
 
 [tool.semantic_release]
```

### Comparing `talkytrend-2.0.8/talkytrend/config.py` & `talkytrend-2.0.9/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-2.0.8/talkytrend/default_settings.toml` & `talkytrend-2.0.9/talkytrend/default_settings.toml`

 * *Files identical despite different names*

### Comparing `talkytrend-2.0.8/talkytrend/main.py` & `talkytrend-2.0.9/talkytrend/main.py`

 * *Files identical despite different names*

### Comparing `talkytrend-2.0.8/PKG-INFO` & `talkytrend-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 2.0.8
+Version: 2.0.9
 Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: talkytrend Version: 2.0.8 Summary: A python package
+Metadata-Version: 2.1 Name: talkytrend Version: 2.0.9 Summary: A python package
 to retrieve economic data such as Trend for any financial symbol. License: MIT
 Keywords: finance,crypto,bot,trend,economic Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: aiohttp (>=3.8.4,<4.0.0) Requires-
```

