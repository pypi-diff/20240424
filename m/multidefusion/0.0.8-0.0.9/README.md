# Comparing `tmp/multidefusion-0.0.8.tar.gz` & `tmp/multidefusion-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidefusion-0.0.8.tar", last modified: Wed Apr 10 15:32:03 2024, max compression
+gzip compressed data, was "multidefusion-0.0.9.tar", last modified: Fri Apr 12 09:35:41 2024, max compression
```

## Comparing `multidefusion-0.0.8.tar` & `multidefusion-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 15:32:03.924305 multidefusion-0.0.8/
--rw-rw-rw-   0        0        0      175 2024-04-10 14:26:29.000000 multidefusion-0.0.8/AUTHORS.rst
--rw-rw-rw-   0        0        0     1094 2024-04-10 14:26:29.000000 multidefusion-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      129 2024-04-10 14:26:29.000000 multidefusion-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1594 2024-04-10 15:32:03.924305 multidefusion-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      614 2024-04-10 14:26:29.000000 multidefusion-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 15:32:03.911775 multidefusion-0.0.8/multidefusion/
--rw-rw-rw-   0        0        0      142 2024-04-10 14:26:29.000000 multidefusion-0.0.8/multidefusion/__init__.py
--rw-rw-rw-   0        0        0    19053 2024-04-10 14:43:27.000000 multidefusion-0.0.8/multidefusion/datainterface.py
--rw-rw-rw-   0        0        0     1705 2024-04-10 14:42:56.000000 multidefusion-0.0.8/multidefusion/fusion.py
--rw-rw-rw-   0        0        0    26603 2024-04-10 14:43:21.000000 multidefusion-0.0.8/multidefusion/integration.py
--rw-rw-rw-   0        0        0       20 2024-04-10 14:26:29.000000 multidefusion-0.0.8/multidefusion/multidefusion.py
--rw-rw-rw-   0        0        0    45552 2024-04-10 14:43:34.000000 multidefusion-0.0.8/multidefusion/results.py
-drwxrwxrwx   0        0        0        0 2024-04-10 15:32:03.922304 multidefusion-0.0.8/multidefusion.egg-info/
--rw-rw-rw-   0        0        0     1594 2024-04-10 15:32:03.000000 multidefusion-0.0.8/multidefusion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2024-04-10 15:32:03.000000 multidefusion-0.0.8/multidefusion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       70 2024-04-10 15:32:03.000000 multidefusion-0.0.8/multidefusion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-10 14:55:46.000000 multidefusion-0.0.8/multidefusion.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       70 2024-04-10 15:32:03.000000 multidefusion-0.0.8/multidefusion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-10 15:32:03.000000 multidefusion-0.0.8/multidefusion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       73 2024-04-10 14:50:44.000000 multidefusion-0.0.8/requirements.txt
--rw-rw-rw-   0        0        0      421 2024-04-10 15:32:03.925305 multidefusion-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1830 2024-04-10 15:31:02.000000 multidefusion-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 15:32:03.921297 multidefusion-0.0.8/tests/
--rw-rw-rw-   0        0        0      438 2024-04-10 14:26:29.000000 multidefusion-0.0.8/tests/test_multidefusion.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:35:41.437199 multidefusion-0.0.9/
+-rw-rw-rw-   0        0        0      175 2024-04-10 14:26:29.000000 multidefusion-0.0.9/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1094 2024-04-10 14:26:29.000000 multidefusion-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      129 2024-04-10 14:26:29.000000 multidefusion-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1594 2024-04-12 09:35:41.437199 multidefusion-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      614 2024-04-10 14:26:29.000000 multidefusion-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 09:35:41.423573 multidefusion-0.0.9/multidefusion/
+-rw-rw-rw-   0        0        0      142 2024-04-10 14:26:29.000000 multidefusion-0.0.9/multidefusion/__init__.py
+-rw-rw-rw-   0        0        0    19053 2024-04-10 14:43:27.000000 multidefusion-0.0.9/multidefusion/datainterface.py
+-rw-rw-rw-   0        0        0     1705 2024-04-10 14:42:56.000000 multidefusion-0.0.9/multidefusion/fusion.py
+-rw-rw-rw-   0        0        0    26603 2024-04-10 14:43:21.000000 multidefusion-0.0.9/multidefusion/integration.py
+-rw-rw-rw-   0        0        0       20 2024-04-10 14:26:29.000000 multidefusion-0.0.9/multidefusion/multidefusion.py
+-rw-rw-rw-   0        0        0    45552 2024-04-10 14:43:34.000000 multidefusion-0.0.9/multidefusion/results.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:35:41.437199 multidefusion-0.0.9/multidefusion.egg-info/
+-rw-rw-rw-   0        0        0     1594 2024-04-12 09:35:41.000000 multidefusion-0.0.9/multidefusion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2024-04-12 09:35:41.000000 multidefusion-0.0.9/multidefusion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       70 2024-04-12 09:35:41.000000 multidefusion-0.0.9/multidefusion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-10 14:55:46.000000 multidefusion-0.0.9/multidefusion.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       70 2024-04-12 09:35:41.000000 multidefusion-0.0.9/multidefusion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-12 09:35:41.000000 multidefusion-0.0.9/multidefusion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       73 2024-04-10 14:50:44.000000 multidefusion-0.0.9/requirements.txt
+-rw-rw-rw-   0        0        0      421 2024-04-12 09:35:41.437199 multidefusion-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1830 2024-04-12 09:35:15.000000 multidefusion-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:35:41.437199 multidefusion-0.0.9/tests/
+-rw-rw-rw-   0        0        0      438 2024-04-10 14:26:29.000000 multidefusion-0.0.9/tests/test_multidefusion.py
```

### Comparing `multidefusion-0.0.8/LICENSE` & `multidefusion-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `multidefusion-0.0.8/PKG-INFO` & `multidefusion-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidefusion
-Version: 0.0.8
+Version: 0.0.9
 Summary: Perform data fusion and analysis of the ground deformations for multiple stations.
 Home-page: https://github.com/damiantondas/multidefusion
 Author: Damian Tondas
 Author-email: damian.tondas@gmail.com
 License: MIT license
 Keywords: multidefusion
 Classifier: Intended Audience :: Developers
```

### Comparing `multidefusion-0.0.8/README.md` & `multidefusion-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `multidefusion-0.0.8/multidefusion/datainterface.py` & `multidefusion-0.0.9/multidefusion/datainterface.py`

 * *Files identical despite different names*

### Comparing `multidefusion-0.0.8/multidefusion/fusion.py` & `multidefusion-0.0.9/multidefusion/fusion.py`

 * *Files identical despite different names*

### Comparing `multidefusion-0.0.8/multidefusion/integration.py` & `multidefusion-0.0.9/multidefusion/integration.py`

 * *Files identical despite different names*

### Comparing `multidefusion-0.0.8/multidefusion/results.py` & `multidefusion-0.0.9/multidefusion/results.py`

 * *Files identical despite different names*

### Comparing `multidefusion-0.0.8/multidefusion.egg-info/PKG-INFO` & `multidefusion-0.0.9/multidefusion.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidefusion
-Version: 0.0.8
+Version: 0.0.9
 Summary: Perform data fusion and analysis of the ground deformations for multiple stations.
 Home-page: https://github.com/damiantondas/multidefusion
 Author: Damian Tondas
 Author-email: damian.tondas@gmail.com
 License: MIT license
 Keywords: multidefusion
 Classifier: Intended Audience :: Developers
```

### Comparing `multidefusion-0.0.8/setup.py` & `multidefusion-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='multidefusion',
     name='multidefusion',
     packages=find_packages(include=['multidefusion', 'multidefusion.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/damiantondas/multidefusion',
-    version='0.0.8',
+    version='0.0.9',
     zip_safe=False,
 )
```

