# Comparing `tmp/jaxutils-nightly-0.0.8.dev20240422.tar.gz` & `tmp/jaxutils-nightly-0.0.8.dev20240423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jaxutils-nightly-0.0.8.dev20240422.tar", last modified: Mon Apr 22 00:06:33 2024, max compression
+gzip compressed data, was "dist/jaxutils-nightly-0.0.8.dev20240423.tar", last modified: Tue Apr 23 00:06:33 2024, max compression
```

## Comparing `jaxutils-nightly-0.0.8.dev20240422.tar` & `jaxutils-nightly-0.0.8.dev20240423.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-22 00:06:33.150836 jaxutils-nightly-0.0.8.dev20240422/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2024-04-22 00:06:33.150836 jaxutils-nightly-0.0.8.dev20240422/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3004 2024-04-22 00:06:25.000000 jaxutils-nightly-0.0.8.dev20240422/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-22 00:06:33.150836 jaxutils-nightly-0.0.8.dev20240422/jaxutils/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1701 2024-04-22 00:06:25.000000 jaxutils-nightly-0.0.8.dev20240422/jaxutils/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      509 2024-04-22 00:06:33.150836 jaxutils-nightly-0.0.8.dev20240422/jaxutils/_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4944 2024-04-22 00:06:25.000000 jaxutils-nightly-0.0.8.dev20240422/jaxutils/config.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3831 2024-04-22 00:06:25.000000 jaxutils-nightly-0.0.8.dev20240422/jaxutils/data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3536 2024-04-22 00:06:25.000000 jaxutils-nightly-0.0.8.dev20240422/jaxutils/dict.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13713 2024-04-22 00:06:25.000000 jaxutils-nightly-0.0.8.dev20240422/jaxutils/parameters.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2802 2024-04-22 00:06:25.000000 jaxutils-nightly-0.0.8.dev20240422/jaxutils/pytree.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-22 00:06:33.150836 jaxutils-nightly-0.0.8.dev20240422/jaxutils_nightly.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2024-04-22 00:06:33.000000 jaxutils-nightly-0.0.8.dev20240422/jaxutils_nightly.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2024-04-22 00:06:33.000000 jaxutils-nightly-0.0.8.dev20240422/jaxutils_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-04-22 00:06:33.000000 jaxutils-nightly-0.0.8.dev20240422/jaxutils_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2024-04-22 00:06:33.000000 jaxutils-nightly-0.0.8.dev20240422/jaxutils_nightly.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2024-04-22 00:06:33.000000 jaxutils-nightly-0.0.8.dev20240422/jaxutils_nightly.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      233 2024-04-22 00:06:33.150836 jaxutils-nightly-0.0.8.dev20240422/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2389 2024-04-22 00:06:25.000000 jaxutils-nightly-0.0.8.dev20240422/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    83607 2024-04-22 00:06:25.000000 jaxutils-nightly-0.0.8.dev20240422/versioneer.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-23 00:06:33.774547 jaxutils-nightly-0.0.8.dev20240423/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2024-04-23 00:06:33.774547 jaxutils-nightly-0.0.8.dev20240423/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3004 2024-04-23 00:06:26.000000 jaxutils-nightly-0.0.8.dev20240423/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-23 00:06:33.778547 jaxutils-nightly-0.0.8.dev20240423/jaxutils/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1701 2024-04-23 00:06:26.000000 jaxutils-nightly-0.0.8.dev20240423/jaxutils/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      509 2024-04-23 00:06:33.778547 jaxutils-nightly-0.0.8.dev20240423/jaxutils/_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4944 2024-04-23 00:06:26.000000 jaxutils-nightly-0.0.8.dev20240423/jaxutils/config.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3831 2024-04-23 00:06:26.000000 jaxutils-nightly-0.0.8.dev20240423/jaxutils/data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3536 2024-04-23 00:06:26.000000 jaxutils-nightly-0.0.8.dev20240423/jaxutils/dict.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13713 2024-04-23 00:06:26.000000 jaxutils-nightly-0.0.8.dev20240423/jaxutils/parameters.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2802 2024-04-23 00:06:26.000000 jaxutils-nightly-0.0.8.dev20240423/jaxutils/pytree.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2024-04-23 00:06:33.774547 jaxutils-nightly-0.0.8.dev20240423/jaxutils_nightly.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4582 2024-04-23 00:06:33.000000 jaxutils-nightly-0.0.8.dev20240423/jaxutils_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      378 2024-04-23 00:06:33.000000 jaxutils-nightly-0.0.8.dev20240423/jaxutils_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2024-04-23 00:06:33.000000 jaxutils-nightly-0.0.8.dev20240423/jaxutils_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2024-04-23 00:06:33.000000 jaxutils-nightly-0.0.8.dev20240423/jaxutils_nightly.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        9 2024-04-23 00:06:33.000000 jaxutils-nightly-0.0.8.dev20240423/jaxutils_nightly.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      233 2024-04-23 00:06:33.778547 jaxutils-nightly-0.0.8.dev20240423/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2389 2024-04-23 00:06:26.000000 jaxutils-nightly-0.0.8.dev20240423/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    83607 2024-04-23 00:06:26.000000 jaxutils-nightly-0.0.8.dev20240423/versioneer.py
```

### Comparing `jaxutils-nightly-0.0.8.dev20240422/PKG-INFO` & `jaxutils-nightly-0.0.8.dev20240423/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxutils-nightly
-Version: 0.0.8.dev20240422
+Version: 0.0.8.dev20240423
 Summary: Utility functions for JaxGaussianProcesses
 Home-page: UNKNOWN
 Author: Daniel Dodd and Thomas Pinder
 Author-email: tompinder@live.co.uk
 License: LICENSE
 Project-URL: Documentation, https://JaxUitls.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/JaxGaussianProcesses/JaxUitls
```

### Comparing `jaxutils-nightly-0.0.8.dev20240422/README.md` & `jaxutils-nightly-0.0.8.dev20240423/README.md`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20240422/jaxutils/__init__.py` & `jaxutils-nightly-0.0.8.dev20240423/jaxutils/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20240422/jaxutils/config.py` & `jaxutils-nightly-0.0.8.dev20240423/jaxutils/config.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20240422/jaxutils/data.py` & `jaxutils-nightly-0.0.8.dev20240423/jaxutils/data.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20240422/jaxutils/dict.py` & `jaxutils-nightly-0.0.8.dev20240423/jaxutils/dict.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20240422/jaxutils/parameters.py` & `jaxutils-nightly-0.0.8.dev20240423/jaxutils/parameters.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20240422/jaxutils/pytree.py` & `jaxutils-nightly-0.0.8.dev20240423/jaxutils/pytree.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20240422/jaxutils_nightly.egg-info/PKG-INFO` & `jaxutils-nightly-0.0.8.dev20240423/jaxutils_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxutils-nightly
-Version: 0.0.8.dev20240422
+Version: 0.0.8.dev20240423
 Summary: Utility functions for JaxGaussianProcesses
 Home-page: UNKNOWN
 Author: Daniel Dodd and Thomas Pinder
 Author-email: tompinder@live.co.uk
 License: LICENSE
 Project-URL: Documentation, https://JaxUitls.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/JaxGaussianProcesses/JaxUitls
```

### Comparing `jaxutils-nightly-0.0.8.dev20240422/setup.py` & `jaxutils-nightly-0.0.8.dev20240423/setup.py`

 * *Files identical despite different names*

### Comparing `jaxutils-nightly-0.0.8.dev20240422/versioneer.py` & `jaxutils-nightly-0.0.8.dev20240423/versioneer.py`

 * *Files identical despite different names*

