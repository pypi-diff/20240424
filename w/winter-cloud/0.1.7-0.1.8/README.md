# Comparing `tmp/winter_cloud-0.1.7.tar.gz` & `tmp/winter_cloud-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winter_cloud-0.1.7.tar", max compression
+gzip compressed data, was "winter_cloud-0.1.8.tar", max compression
```

## Comparing `winter_cloud-0.1.7.tar` & `winter_cloud-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       22 2024-01-25 08:05:23.586024 winter_cloud-0.1.7/README.md
--rw-r--r--   0        0        0      609 2024-01-30 06:10:59.833835 winter_cloud-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-25 08:05:23.587356 winter_cloud-0.1.7/src/winter/__init__.py
--rw-r--r--   0        0        0      213 2024-01-25 08:05:23.587678 winter_cloud-0.1.7/src/winter/_utils.py
--rw-r--r--   0        0        0     3585 2024-01-25 08:05:23.587813 winter_cloud-0.1.7/src/winter/authentication.py
--rw-r--r--   0        0        0        0 2024-01-25 08:05:23.587923 winter_cloud-0.1.7/src/winter/common/__init__.py
--rw-r--r--   0        0        0     2283 2024-01-30 06:07:32.921012 winter_cloud-0.1.7/src/winter/common/dao.py
--rw-r--r--   0        0        0      382 2024-01-30 06:07:32.921243 winter_cloud-0.1.7/src/winter/common/decorators.py
--rw-r--r--   0        0        0     2316 2024-01-25 08:05:23.588270 winter_cloud-0.1.7/src/winter/common/exception.py
--rw-r--r--   0        0        0     1794 2024-01-25 08:05:23.588378 winter_cloud-0.1.7/src/winter/common/ordering.py
--rw-r--r--   0        0        0     1692 2024-01-25 08:05:23.588492 winter_cloud-0.1.7/src/winter/common/pagination.py
--rw-r--r--   0        0        0      413 2024-01-25 08:05:23.588610 winter_cloud-0.1.7/src/winter/common/schema.py
--rw-r--r--   0        0        0        0 2024-01-25 08:05:23.589867 winter_cloud-0.1.7/src/winter/core/__init__.py
--rw-r--r--   0        0        0     1092 2024-01-25 08:05:23.590257 winter_cloud-0.1.7/src/winter/core/depends.py
--rw-r--r--   0        0        0      414 2024-01-25 08:05:23.590433 winter_cloud-0.1.7/src/winter/core/register/__init__.py
--rw-r--r--   0        0        0      268 2024-01-25 08:05:23.590550 winter_cloud-0.1.7/src/winter/core/register/auth.py
--rw-r--r--   0        0        0      716 2024-01-25 08:05:23.590662 winter_cloud-0.1.7/src/winter/core/register/exception.py
--rw-r--r--   0        0        0      430 2024-01-25 08:05:23.590778 winter_cloud-0.1.7/src/winter/core/register/logger.py
--rw-r--r--   0        0        0      240 2024-01-25 08:05:23.590926 winter_cloud-0.1.7/src/winter/core/register/mysql.py
--rw-r--r--   0        0        0     2072 2024-01-25 08:05:23.591053 winter_cloud-0.1.7/src/winter/core/register/nacos.py
--rw-r--r--   0        0        0     1946 2024-01-25 08:05:23.591187 winter_cloud-0.1.7/src/winter/winter.py
--rw-r--r--   0        0        0      707 1970-01-01 00:00:00.000000 winter_cloud-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       22 2024-01-25 08:05:23.586024 winter_cloud-0.1.8/README.md
+-rw-r--r--   0        0        0      610 2024-04-24 10:33:24.906334 winter_cloud-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-25 08:05:23.587356 winter_cloud-0.1.8/src/winter/__init__.py
+-rw-r--r--   0        0        0      213 2024-01-25 08:05:23.587678 winter_cloud-0.1.8/src/winter/_utils.py
+-rw-r--r--   0        0        0     3585 2024-01-25 08:05:23.587813 winter_cloud-0.1.8/src/winter/authentication.py
+-rw-r--r--   0        0        0        0 2024-01-25 08:05:23.587923 winter_cloud-0.1.8/src/winter/common/__init__.py
+-rw-r--r--   0        0        0     2283 2024-01-30 06:07:32.921012 winter_cloud-0.1.8/src/winter/common/dao.py
+-rw-r--r--   0        0        0      382 2024-01-30 06:07:32.921243 winter_cloud-0.1.8/src/winter/common/decorators.py
+-rw-r--r--   0        0        0     2316 2024-01-25 08:05:23.588270 winter_cloud-0.1.8/src/winter/common/exception.py
+-rw-r--r--   0        0        0     1794 2024-01-25 08:05:23.588378 winter_cloud-0.1.8/src/winter/common/ordering.py
+-rw-r--r--   0        0        0     1692 2024-01-25 08:05:23.588492 winter_cloud-0.1.8/src/winter/common/pagination.py
+-rw-r--r--   0        0        0      413 2024-01-25 08:05:23.588610 winter_cloud-0.1.8/src/winter/common/schema.py
+-rw-r--r--   0        0        0        0 2024-01-25 08:05:23.589867 winter_cloud-0.1.8/src/winter/core/__init__.py
+-rw-r--r--   0        0        0     1092 2024-01-25 08:05:23.590257 winter_cloud-0.1.8/src/winter/core/depends.py
+-rw-r--r--   0        0        0      414 2024-01-25 08:05:23.590433 winter_cloud-0.1.8/src/winter/core/register/__init__.py
+-rw-r--r--   0        0        0      268 2024-01-25 08:05:23.590550 winter_cloud-0.1.8/src/winter/core/register/auth.py
+-rw-r--r--   0        0        0      716 2024-01-25 08:05:23.590662 winter_cloud-0.1.8/src/winter/core/register/exception.py
+-rw-r--r--   0        0        0      430 2024-01-25 08:05:23.590778 winter_cloud-0.1.8/src/winter/core/register/logger.py
+-rw-r--r--   0        0        0      240 2024-01-25 08:05:23.590926 winter_cloud-0.1.8/src/winter/core/register/mysql.py
+-rw-r--r--   0        0        0     2072 2024-01-25 08:05:23.591053 winter_cloud-0.1.8/src/winter/core/register/nacos.py
+-rw-r--r--   0        0        0     1946 2024-01-25 08:05:23.591187 winter_cloud-0.1.8/src/winter/winter.py
+-rw-r--r--   0        0        0      716 1970-01-01 00:00:00.000000 winter_cloud-0.1.8/PKG-INFO
```

### Comparing `winter_cloud-0.1.7/pyproject.toml` & `winter_cloud-0.1.8/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "winter-cloud"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["miclon <jcnd@163.com>"]
 readme = "README.md"
 packages = [
     { include = "winter", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-fastapi = { extras = ["all"], version = "0.105.0" }
+fastapi = { extras = ["all"], version = "~0.109.1" }
 sqlmodel = "0.0.14"
 dynaconf = "3.2.4"
 loguru = "0.7.2"
 aiomysql = "0.2.0"
 fastapi-async-sqlalchemy = "0.6.0"
 fastapi-pagination = "0.12.14"
 use-nacos = "^0.1.5"
```

### Comparing `winter_cloud-0.1.7/src/winter/authentication.py` & `winter_cloud-0.1.8/src/winter/authentication.py`

 * *Files identical despite different names*

### Comparing `winter_cloud-0.1.7/src/winter/common/dao.py` & `winter_cloud-0.1.8/src/winter/common/dao.py`

 * *Files identical despite different names*

### Comparing `winter_cloud-0.1.7/src/winter/common/exception.py` & `winter_cloud-0.1.8/src/winter/common/exception.py`

 * *Files identical despite different names*

### Comparing `winter_cloud-0.1.7/src/winter/common/ordering.py` & `winter_cloud-0.1.8/src/winter/common/ordering.py`

 * *Files identical despite different names*

### Comparing `winter_cloud-0.1.7/src/winter/common/pagination.py` & `winter_cloud-0.1.8/src/winter/common/pagination.py`

 * *Files identical despite different names*

### Comparing `winter_cloud-0.1.7/src/winter/core/depends.py` & `winter_cloud-0.1.8/src/winter/core/depends.py`

 * *Files identical despite different names*

### Comparing `winter_cloud-0.1.7/src/winter/core/register/exception.py` & `winter_cloud-0.1.8/src/winter/core/register/exception.py`

 * *Files identical despite different names*

### Comparing `winter_cloud-0.1.7/src/winter/core/register/nacos.py` & `winter_cloud-0.1.8/src/winter/core/register/nacos.py`

 * *Files identical despite different names*

### Comparing `winter_cloud-0.1.7/src/winter/winter.py` & `winter_cloud-0.1.8/src/winter/winter.py`

 * *Files identical despite different names*

### Comparing `winter_cloud-0.1.7/PKG-INFO` & `winter_cloud-0.1.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: winter-cloud
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: miclon
 Author-email: jcnd@163.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiomysql (==0.2.0)
 Requires-Dist: dynaconf (==3.2.4)
 Requires-Dist: fastapi-async-sqlalchemy (==0.6.0)
 Requires-Dist: fastapi-pagination (==0.12.14)
-Requires-Dist: fastapi[all] (==0.105.0)
+Requires-Dist: fastapi[all] (>=0.109.1,<0.110.0)
 Requires-Dist: loguru (==0.7.2)
 Requires-Dist: sqlmodel (==0.0.14)
 Requires-Dist: use-logger (>=0.1.9,<0.2.0)
 Requires-Dist: use-nacos (>=0.1.5,<0.2.0)
 Description-Content-Type: text/markdown
 
 # Winter
```

