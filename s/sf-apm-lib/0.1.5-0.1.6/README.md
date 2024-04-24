# Comparing `tmp/sf_apm_lib-0.1.5.tar.gz` & `tmp/sf_apm_lib-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sf_apm_lib-0.1.5.tar", last modified: Tue Nov 28 07:04:01 2023, max compression
+gzip compressed data, was "sf_apm_lib-0.1.6.tar", last modified: Wed Apr 24 07:39:05 2024, max compression
```

## Comparing `sf_apm_lib-0.1.5.tar` & `sf_apm_lib-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 07:04:01.123884 sf_apm_lib-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-11-28 07:03:55.000000 sf_apm_lib-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2023-11-28 07:04:01.123884 sf_apm_lib-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      924 2023-11-28 07:03:55.000000 sf_apm_lib-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-28 07:04:01.123884 sf_apm_lib-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2023-11-28 07:03:55.000000 sf_apm_lib-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 07:04:01.123884 sf_apm_lib-0.1.5/sf_apm_lib/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-11-28 07:03:55.000000 sf_apm_lib-0.1.5/sf_apm_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5173 2023-11-28 07:03:55.000000 sf_apm_lib-0.1.5/sf_apm_lib/snappyflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 07:04:01.123884 sf_apm_lib-0.1.5/sf_apm_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2023-11-28 07:04:01.000000 sf_apm_lib-0.1.5/sf_apm_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      264 2023-11-28 07:04:01.000000 sf_apm_lib-0.1.5/sf_apm_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 07:04:01.000000 sf_apm_lib-0.1.5/sf_apm_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-28 07:04:01.000000 sf_apm_lib-0.1.5/sf_apm_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-28 07:04:01.000000 sf_apm_lib-0.1.5/sf_apm_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 07:04:01.123884 sf_apm_lib-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-11-28 07:03:55.000000 sf_apm_lib-0.1.5/tests/test_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:39:05.555196 sf_apm_lib-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-24 07:39:01.000000 sf_apm_lib-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-24 07:39:05.555196 sf_apm_lib-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-24 07:39:01.000000 sf_apm_lib-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 07:39:05.555196 sf_apm_lib-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-24 07:39:01.000000 sf_apm_lib-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:39:05.555196 sf_apm_lib-0.1.6/sf_apm_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-24 07:39:01.000000 sf_apm_lib-0.1.6/sf_apm_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-24 07:39:01.000000 sf_apm_lib-0.1.6/sf_apm_lib/snappyflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:39:05.555196 sf_apm_lib-0.1.6/sf_apm_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-24 07:39:05.000000 sf_apm_lib-0.1.6/sf_apm_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-24 07:39:05.000000 sf_apm_lib-0.1.6/sf_apm_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 07:39:05.000000 sf_apm_lib-0.1.6/sf_apm_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-24 07:39:05.000000 sf_apm_lib-0.1.6/sf_apm_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 07:39:05.000000 sf_apm_lib-0.1.6/sf_apm_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:39:05.555196 sf_apm_lib-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-24 07:39:01.000000 sf_apm_lib-0.1.6/tests/test_sample.py
```

### Comparing `sf_apm_lib-0.1.5/LICENSE` & `sf_apm_lib-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sf_apm_lib-0.1.5/PKG-INFO` & `sf_apm_lib-0.1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sf_apm_lib
-Version: 0.1.5
+Version: 0.1.6
 Summary: Snappyflow pip package
 Home-page: https://github.com/snappyflow/py_snappyflow
 Author: Maplelabs
 Author-email: pradeep.jaiswar@maplelabs.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sf_apm_lib-0.1.5/README.md` & `sf_apm_lib-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `sf_apm_lib-0.1.5/setup.py` & `sf_apm_lib-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     text_type = type(u"")
     with io.open(filename, mode="r", encoding='utf-8') as fd:
         return re.sub(text_type(r':[a-z]+:`~?(.*?)`'), text_type(r'``\1``'), fd.read())
 
 
 setup(
     name="sf_apm_lib",
-    version="0.1.5",
+    version="0.1.6",
     url="https://github.com/snappyflow/py_snappyflow",
     license='MIT',
 
     author="Maplelabs",
     author_email="pradeep.jaiswar@maplelabs.com",
 
     description="Snappyflow pip package",
```

### Comparing `sf_apm_lib-0.1.5/sf_apm_lib/snappyflow.py` & `sf_apm_lib-0.1.6/sf_apm_lib/snappyflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,16 @@
         response (obj): Contains http response information from User
     Returns:
         nil
 
     """
     path_info = request.httprequest.environ.get("PATH_INFO")
     name = path_info
+    if not hasattr(request, 'params'):
+        request.params = {}
     for key in ["model", "method", "signal"]:
         val = request.params.get(key)
         if val and val not in name:
             name += " {}: {}".format(key, val)
     elasticapm.set_context(lambda: get_data_from_request(elasticapm, request), "request")
     try:
         code = response.status_code
```

### Comparing `sf_apm_lib-0.1.5/sf_apm_lib.egg-info/PKG-INFO` & `sf_apm_lib-0.1.6/sf_apm_lib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sf-apm-lib
-Version: 0.1.5
+Name: sf_apm_lib
+Version: 0.1.6
 Summary: Snappyflow pip package
 Home-page: https://github.com/snappyflow/py_snappyflow
 Author: Maplelabs
 Author-email: pradeep.jaiswar@maplelabs.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

