# Comparing `tmp/skip_pydjamodb-0.1.0.tar.gz` & `tmp/skip_pydjamodb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip_pydjamodb-0.1.0.tar", last modified: Thu Apr 18 13:57:38 2024, max compression
+gzip compressed data, was "skip_pydjamodb-0.1.1.tar", last modified: Wed Apr 24 07:10:34 2024, max compression
```

## Comparing `skip_pydjamodb-0.1.0.tar` & `skip_pydjamodb-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:57:38.177944 skip_pydjamodb-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-18 13:57:34.000000 skip_pydjamodb-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-18 13:57:34.000000 skip_pydjamodb-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-18 13:57:38.177944 skip_pydjamodb-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-18 13:57:34.000000 skip_pydjamodb-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:57:38.173944 skip_pydjamodb-0.1.0/pydjamodb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:57:34.000000 skip_pydjamodb-0.1.0/pydjamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-18 13:57:34.000000 skip_pydjamodb-0.1.0/pydjamodb/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-04-18 13:57:34.000000 skip_pydjamodb-0.1.0/pydjamodb/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-18 13:57:34.000000 skip_pydjamodb-0.1.0/pydjamodb/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     8555 2024-04-18 13:57:34.000000 skip_pydjamodb-0.1.0/pydjamodb/queryset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-04-18 13:57:34.000000 skip_pydjamodb-0.1.0/pydjamodb/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:57:38.177944 skip_pydjamodb-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-18 13:57:34.000000 skip_pydjamodb-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:57:38.177944 skip_pydjamodb-0.1.0/skip_pydjamodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-18 13:57:38.000000 skip_pydjamodb-0.1.0/skip_pydjamodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-18 13:57:38.000000 skip_pydjamodb-0.1.0/skip_pydjamodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:57:38.000000 skip_pydjamodb-0.1.0/skip_pydjamodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:57:38.000000 skip_pydjamodb-0.1.0/skip_pydjamodb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 13:57:38.000000 skip_pydjamodb-0.1.0/skip_pydjamodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 13:57:38.000000 skip_pydjamodb-0.1.0/skip_pydjamodb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:10:34.690712 skip_pydjamodb-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-24 07:10:29.000000 skip_pydjamodb-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-24 07:10:29.000000 skip_pydjamodb-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-24 07:10:34.686712 skip_pydjamodb-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-24 07:10:29.000000 skip_pydjamodb-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:10:34.686712 skip_pydjamodb-0.1.1/pydjamodb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 07:10:29.000000 skip_pydjamodb-0.1.1/pydjamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-24 07:10:29.000000 skip_pydjamodb-0.1.1/pydjamodb/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-04-24 07:10:29.000000 skip_pydjamodb-0.1.1/pydjamodb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-24 07:10:29.000000 skip_pydjamodb-0.1.1/pydjamodb/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8555 2024-04-24 07:10:29.000000 skip_pydjamodb-0.1.1/pydjamodb/queryset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-24 07:10:29.000000 skip_pydjamodb-0.1.1/pydjamodb/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 07:10:34.690712 skip_pydjamodb-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-24 07:10:29.000000 skip_pydjamodb-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:10:34.686712 skip_pydjamodb-0.1.1/skip_pydjamodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-24 07:10:34.000000 skip_pydjamodb-0.1.1/skip_pydjamodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-24 07:10:34.000000 skip_pydjamodb-0.1.1/skip_pydjamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 07:10:34.000000 skip_pydjamodb-0.1.1/skip_pydjamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 07:10:34.000000 skip_pydjamodb-0.1.1/skip_pydjamodb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 07:10:34.000000 skip_pydjamodb-0.1.1/skip_pydjamodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 07:10:34.000000 skip_pydjamodb-0.1.1/skip_pydjamodb.egg-info/top_level.txt
```

### Comparing `skip_pydjamodb-0.1.0/LICENSE` & `skip_pydjamodb-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skip_pydjamodb-0.1.0/PKG-INFO` & `skip_pydjamodb-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-pydjamodb
-Version: 0.1.0
+Version: 0.1.1
 Summary: Django interface to PyDjamoDB.
 Home-page: https://github.com/skip-pay/pydjamodb
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: MIT
 Keywords: django,DynamoDB,PyDjamoDB
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `skip_pydjamodb-0.1.0/README.md` & `skip_pydjamodb-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `skip_pydjamodb-0.1.0/pydjamodb/attributes.py` & `skip_pydjamodb-0.1.1/pydjamodb/attributes.py`

 * *Files identical despite different names*

### Comparing `skip_pydjamodb-0.1.0/pydjamodb/connection.py` & `skip_pydjamodb-0.1.1/pydjamodb/connection.py`

 * *Files identical despite different names*

### Comparing `skip_pydjamodb-0.1.0/pydjamodb/models.py` & `skip_pydjamodb-0.1.1/pydjamodb/models.py`

 * *Files identical despite different names*

### Comparing `skip_pydjamodb-0.1.0/pydjamodb/queryset.py` & `skip_pydjamodb-0.1.1/pydjamodb/queryset.py`

 * *Files identical despite different names*

### Comparing `skip_pydjamodb-0.1.0/pydjamodb/test_runner.py` & `skip_pydjamodb-0.1.1/pydjamodb/test_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         model_class._connection.post_test_clean(model_class)
 
 
 class DynamoDBTestSuiteMixin:
 
     parallel_test_suite = DynamoDBParallelTestSuite
 
-    def log(self, msg):
+    def log(self, msg, level=None):
         sys.stderr.write(msg + os.linesep)
 
     def _teardown_pynamodb_database(self, prefix=None):
         init_pynamodb_test_prefix(prefix)
         table_names = []
         for model_class in dynamodb_model_classes:
             table_names.append(model_class._connection.table_name)
```

### Comparing `skip_pydjamodb-0.1.0/setup.py` & `skip_pydjamodb-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='skip-pydjamodb',
-    version='0.1.0',
+    version='0.1.1',
     description="Django interface to PyDjamoDB.",
     keywords='django, DynamoDB, PyDjamoDB',
     author='Lubos Matl',
     author_email='matllubos@gmail.com',
     url='https://github.com/skip-pay/pydjamodb',
     license='MIT',
     package_dir={'pydjamodb': 'pydjamodb'},
```

### Comparing `skip_pydjamodb-0.1.0/skip_pydjamodb.egg-info/PKG-INFO` & `skip_pydjamodb-0.1.1/skip_pydjamodb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-pydjamodb
-Version: 0.1.0
+Version: 0.1.1
 Summary: Django interface to PyDjamoDB.
 Home-page: https://github.com/skip-pay/pydjamodb
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: MIT
 Keywords: django,DynamoDB,PyDjamoDB
 Classifier: Development Status :: 3 - Alpha
```

