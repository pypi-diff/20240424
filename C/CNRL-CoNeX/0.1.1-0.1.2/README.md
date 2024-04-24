# Comparing `tmp/cnrl_conex-0.1.1.tar.gz` & `tmp/cnrl_conex-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnrl_conex-0.1.1.tar", last modified: Tue Apr 23 14:26:37 2024, max compression
+gzip compressed data, was "cnrl_conex-0.1.2.tar", last modified: Tue Apr 23 14:38:53 2024, max compression
```

## Comparing `cnrl_conex-0.1.1.tar` & `cnrl_conex-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2024-04-23 14:26:37.398850 cnrl_conex-0.1.1/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      359 2024-04-23 14:00:44.000000 cnrl_conex-0.1.1/AUTHORS.rst
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2024-04-23 14:26:37.398850 cnrl_conex-0.1.1/CNRL_CoNeX.egg-info/
--rw-r--r--   0 saeed     (1000) saeed     (1000)      705 2024-04-23 14:26:37.000000 cnrl_conex-0.1.1/CNRL_CoNeX.egg-info/PKG-INFO
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      538 2024-04-23 14:26:37.000000 cnrl_conex-0.1.1/CNRL_CoNeX.egg-info/SOURCES.txt
--rw-rw-r--   0 saeed     (1000) saeed     (1000)        1 2024-04-23 14:26:37.000000 cnrl_conex-0.1.1/CNRL_CoNeX.egg-info/dependency_links.txt
--rw-rw-r--   0 saeed     (1000) saeed     (1000)        1 2024-04-23 14:23:19.000000 cnrl_conex-0.1.1/CNRL_CoNeX.egg-info/not-zip-safe
--rw-rw-r--   0 saeed     (1000) saeed     (1000)       47 2024-04-23 14:26:37.000000 cnrl_conex-0.1.1/CNRL_CoNeX.egg-info/requires.txt
--rw-rw-r--   0 saeed     (1000) saeed     (1000)        6 2024-04-23 14:26:37.000000 cnrl_conex-0.1.1/CNRL_CoNeX.egg-info/top_level.txt
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     3472 2024-04-23 14:00:44.000000 cnrl_conex-0.1.1/CONTRIBUTING.rst
--rw-rw-r--   0 saeed     (1000) saeed     (1000)       24 2024-04-23 14:00:44.000000 cnrl_conex-0.1.1/HISTORY.rst
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     1103 2024-04-23 14:00:44.000000 cnrl_conex-0.1.1/LICENSE
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      262 2024-04-23 14:00:44.000000 cnrl_conex-0.1.1/MANIFEST.in
--rw-r--r--   0 saeed     (1000) saeed     (1000)      705 2024-04-23 14:26:37.398850 cnrl_conex-0.1.1/PKG-INFO
--rw-rw-r--   0 saeed     (1000) saeed     (1000)        7 2024-04-23 14:00:44.000000 cnrl_conex-0.1.1/README.md
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2024-04-23 14:26:37.394850 cnrl_conex-0.1.1/conex/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)       76 2024-04-23 14:25:56.000000 cnrl_conex-0.1.1/conex/__init__.py
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2024-04-23 14:26:37.394850 cnrl_conex-0.1.1/docs/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      606 2024-04-23 14:00:44.000000 cnrl_conex-0.1.1/docs/Makefile
--rw-rw-r--   0 saeed     (1000) saeed     (1000)       28 2024-04-23 14:00:44.000000 cnrl_conex-0.1.1/docs/authors.rst
--rwxrwxr-x   0 saeed     (1000) saeed     (1000)     4928 2024-04-23 14:00:44.000000 cnrl_conex-0.1.1/docs/conf.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)       33 2024-04-23 14:00:44.000000 cnrl_conex-0.1.1/docs/contributing.rst
--rw-rw-r--   0 saeed     (1000) saeed     (1000)       28 2024-04-23 14:00:44.000000 cnrl_conex-0.1.1/docs/documentation.rst
--rw-rw-r--   0 saeed     (1000) saeed     (1000)       28 2024-04-23 14:00:44.000000 cnrl_conex-0.1.1/docs/history.rst
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      311 2024-04-23 14:00:44.000000 cnrl_conex-0.1.1/docs/index.rst
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     1112 2024-04-23 14:00:44.000000 cnrl_conex-0.1.1/docs/installation.rst
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      803 2024-04-23 14:00:44.000000 cnrl_conex-0.1.1/docs/make.bat
--rw-rw-r--   0 saeed     (1000) saeed     (1000)       26 2024-04-23 14:00:44.000000 cnrl_conex-0.1.1/docs/readme.rst
--rw-rw-r--   0 saeed     (1000) saeed     (1000)       18 2024-04-23 14:00:44.000000 cnrl_conex-0.1.1/docs/tutorial.rst
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      422 2024-04-23 14:26:37.398850 cnrl_conex-0.1.1/setup.cfg
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     1165 2024-04-23 14:25:47.000000 cnrl_conex-0.1.1/setup.py
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2024-04-23 14:26:37.398850 cnrl_conex-0.1.1/tests/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)       35 2024-04-23 14:00:44.000000 cnrl_conex-0.1.1/tests/__init__.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      508 2024-04-23 14:00:44.000000 cnrl_conex-0.1.1/tests/test_CoNeX.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:38:53.290560 cnrl_conex-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-23 14:38:48.000000 cnrl_conex-0.1.2/AUTHORS.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:38:53.290560 cnrl_conex-0.1.2/CNRL_CoNeX.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-23 14:38:53.000000 cnrl_conex-0.1.2/CNRL_CoNeX.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-23 14:38:53.000000 cnrl_conex-0.1.2/CNRL_CoNeX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:38:53.000000 cnrl_conex-0.1.2/CNRL_CoNeX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:38:53.000000 cnrl_conex-0.1.2/CNRL_CoNeX.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-23 14:38:53.000000 cnrl_conex-0.1.2/CNRL_CoNeX.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 14:38:53.000000 cnrl_conex-0.1.2/CNRL_CoNeX.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-23 14:38:48.000000 cnrl_conex-0.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 14:38:48.000000 cnrl_conex-0.1.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-23 14:38:48.000000 cnrl_conex-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-23 14:38:48.000000 cnrl_conex-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-23 14:38:53.290560 cnrl_conex-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 14:38:48.000000 cnrl_conex-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:38:53.290560 cnrl_conex-0.1.2/conex/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-23 14:38:48.000000 cnrl_conex-0.1.2/conex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:38:53.290560 cnrl_conex-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-23 14:38:48.000000 cnrl_conex-0.1.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-23 14:38:48.000000 cnrl_conex-0.1.2/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4928 2024-04-23 14:38:48.000000 cnrl_conex-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-23 14:38:48.000000 cnrl_conex-0.1.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-23 14:38:48.000000 cnrl_conex-0.1.2/docs/documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-23 14:38:48.000000 cnrl_conex-0.1.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-23 14:38:48.000000 cnrl_conex-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-23 14:38:48.000000 cnrl_conex-0.1.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-23 14:38:48.000000 cnrl_conex-0.1.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-23 14:38:48.000000 cnrl_conex-0.1.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 14:38:48.000000 cnrl_conex-0.1.2/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-23 14:38:53.290560 cnrl_conex-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-23 14:38:48.000000 cnrl_conex-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:38:53.290560 cnrl_conex-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-23 14:38:48.000000 cnrl_conex-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-23 14:38:48.000000 cnrl_conex-0.1.2/tests/test_CoNeX.py
```

### Comparing `cnrl_conex-0.1.1/CNRL_CoNeX.egg-info/PKG-INFO` & `cnrl_conex-0.1.2/CNRL_CoNeX.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CNRL-CoNeX
-Version: 0.1.1
+Version: 0.1.2
 Summary: Cortical Network for everything!
 Home-page: https://github.com/cnrl/CoNeX
 Author: CNRL
 Author-email: ashenatena@gmail.com
 License: MIT license
 Keywords: CNRL-CoNeX
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `cnrl_conex-0.1.1/CNRL_CoNeX.egg-info/SOURCES.txt` & `cnrl_conex-0.1.2/CNRL_CoNeX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.1/CONTRIBUTING.rst` & `cnrl_conex-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.1/LICENSE` & `cnrl_conex-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.1/PKG-INFO` & `cnrl_conex-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CNRL-CoNeX
-Version: 0.1.1
+Version: 0.1.2
 Summary: Cortical Network for everything!
 Home-page: https://github.com/cnrl/CoNeX
 Author: CNRL
 Author-email: ashenatena@gmail.com
 License: MIT license
 Keywords: CNRL-CoNeX
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `cnrl_conex-0.1.1/docs/Makefile` & `cnrl_conex-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.1/docs/conf.py` & `cnrl_conex-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.1/docs/installation.rst` & `cnrl_conex-0.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.1/docs/make.bat` & `cnrl_conex-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cnrl_conex-0.1.1/setup.py` & `cnrl_conex-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,10 +35,10 @@
     include_package_data=True,
     keywords="CNRL-CoNeX",
     name="CNRL-CoNeX",
     packages=["conex"],
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/cnrl/CoNeX",
-    version="0.1.1",
+    version="0.1.2",
     zip_safe=False,
 )
```

