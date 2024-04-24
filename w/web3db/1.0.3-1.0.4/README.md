# Comparing `tmp/web3db-1.0.3.tar.gz` & `tmp/web3db-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3db-1.0.3.tar", max compression
+gzip compressed data, was "web3db-1.0.4.tar", max compression
```

## Comparing `web3db-1.0.3.tar` & `web3db-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      660 2024-04-18 19:30:47.356765 web3db-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       51 2024-02-26 15:25:35.563030 web3db-1.0.3/web3db/__init__.py
--rw-r--r--   0        0        0    15788 2024-04-18 17:41:03.447775 web3db-1.0.3/web3db/core.py
--rw-r--r--   0        0        0      194 2024-02-26 15:25:35.549029 web3db-1.0.3/web3db/models/__init__.py
--rw-r--r--   0        0        0       88 2024-01-19 19:11:12.418624 web3db-1.0.3/web3db/models/base.py
--rw-r--r--   0        0        0      867 2024-01-21 14:45:55.501349 web3db-1.0.3/web3db/models/discord.py
--rw-r--r--   0        0        0     1026 2024-04-18 16:33:29.904944 web3db-1.0.3/web3db/models/email.py
--rw-r--r--   0        0        0      779 2024-02-04 17:48:00.969984 web3db-1.0.3/web3db/models/github.py
--rw-r--r--   0        0        0     2690 2024-02-26 16:52:49.709378 web3db-1.0.3/web3db/models/mixins.py
--rw-r--r--   0        0        0     1974 2024-03-24 21:27:16.492192 web3db-1.0.3/web3db/models/profile.py
--rw-r--r--   0        0        0      763 2024-02-27 20:23:16.946158 web3db-1.0.3/web3db/models/proxy.py
--rw-r--r--   0        0        0     1078 2024-02-18 00:57:20.977221 web3db-1.0.3/web3db/models/twitter.py
--rw-r--r--   0        0        0      205 2024-01-20 14:29:59.965637 web3db-1.0.3/web3db/utils/__init__.py
--rw-r--r--   0        0        0      922 2024-03-29 13:15:22.001268 web3db-1.0.3/web3db/utils/encrypt_private.py
--rw-r--r--   0        0        0      713 2024-02-10 15:01:20.600084 web3db-1.0.3/web3db/utils/logger.py
--rw-r--r--   0        0        0      861 1970-01-01 00:00:00.000000 web3db-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      660 2024-04-24 07:21:51.453772 web3db-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0       51 2024-02-26 15:25:35.563030 web3db-1.0.4/web3db/__init__.py
+-rw-r--r--   0        0        0    15788 2024-04-18 17:41:03.447775 web3db-1.0.4/web3db/core.py
+-rw-r--r--   0        0        0      194 2024-02-26 15:25:35.549029 web3db-1.0.4/web3db/models/__init__.py
+-rw-r--r--   0        0        0       88 2024-01-19 19:11:12.418624 web3db-1.0.4/web3db/models/base.py
+-rw-r--r--   0        0        0      867 2024-01-21 14:45:55.501349 web3db-1.0.4/web3db/models/discord.py
+-rw-r--r--   0        0        0     1026 2024-04-18 16:33:29.904944 web3db-1.0.4/web3db/models/email.py
+-rw-r--r--   0        0        0      779 2024-02-04 17:48:00.969984 web3db-1.0.4/web3db/models/github.py
+-rw-r--r--   0        0        0     2690 2024-02-26 16:52:49.709378 web3db-1.0.4/web3db/models/mixins.py
+-rw-r--r--   0        0        0     1974 2024-03-24 21:27:16.492192 web3db-1.0.4/web3db/models/profile.py
+-rw-r--r--   0        0        0      763 2024-02-27 20:23:16.946158 web3db-1.0.4/web3db/models/proxy.py
+-rw-r--r--   0        0        0     1078 2024-02-18 00:57:20.977221 web3db-1.0.4/web3db/models/twitter.py
+-rw-r--r--   0        0        0       75 2024-04-24 07:20:40.664893 web3db-1.0.4/web3db/utils/__init__.py
+-rw-r--r--   0        0        0      605 2024-04-24 07:21:51.446492 web3db-1.0.4/web3db/utils/encrypt_private.py
+-rw-r--r--   0        0        0      713 2024-02-10 15:01:20.600084 web3db-1.0.4/web3db/utils/logger.py
+-rw-r--r--   0        0        0      861 1970-01-01 00:00:00.000000 web3db-1.0.4/PKG-INFO
```

### Comparing `web3db-1.0.3/pyproject.toml` & `web3db-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "web3db"
-version = "1.0.3"
+version = "1.0.4"
 description = "Database for web3"
 authors = ["timertimertimer <timerkhan2002@gmail.com>"]
 repository = "https://github.com/timertimertimer/web3db"
 packages = [{include = "web3db"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `web3db-1.0.3/web3db/core.py` & `web3db-1.0.4/web3db/core.py`

 * *Files identical despite different names*

### Comparing `web3db-1.0.3/web3db/models/discord.py` & `web3db-1.0.4/web3db/models/discord.py`

 * *Files identical despite different names*

### Comparing `web3db-1.0.3/web3db/models/email.py` & `web3db-1.0.4/web3db/models/email.py`

 * *Files identical despite different names*

### Comparing `web3db-1.0.3/web3db/models/github.py` & `web3db-1.0.4/web3db/models/github.py`

 * *Files identical despite different names*

### Comparing `web3db-1.0.3/web3db/models/mixins.py` & `web3db-1.0.4/web3db/models/mixins.py`

 * *Files identical despite different names*

### Comparing `web3db-1.0.3/web3db/models/profile.py` & `web3db-1.0.4/web3db/models/profile.py`

 * *Files identical despite different names*

### Comparing `web3db-1.0.3/web3db/models/proxy.py` & `web3db-1.0.4/web3db/models/proxy.py`

 * *Files identical despite different names*

### Comparing `web3db-1.0.3/web3db/models/twitter.py` & `web3db-1.0.4/web3db/models/twitter.py`

 * *Files identical despite different names*

### Comparing `web3db-1.0.3/web3db/utils/logger.py` & `web3db-1.0.4/web3db/utils/logger.py`

 * *Files identical despite different names*

### Comparing `web3db-1.0.3/PKG-INFO` & `web3db-1.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web3db
-Version: 1.0.3
+Version: 1.0.4
 Summary: Database for web3
 Home-page: https://github.com/timertimertimer/web3db
 Author: timertimertimer
 Author-email: timerkhan2002@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

