# Comparing `tmp/torch_kf-0.0.1.tar.gz` & `tmp/torch_kf-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_kf-0.0.1.tar", last modified: Tue Apr 23 22:46:06 2024, max compression
+gzip compressed data, was "torch_kf-0.0.2.tar", last modified: Tue Apr 23 23:31:07 2024, max compression
```

## Comparing `torch_kf-0.0.1.tar` & `torch_kf-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 rreme     (1000) rreme     (1000)        0 2024-04-23 22:46:06.761987 torch_kf-0.0.1/
--rw-rw-r--   0 rreme     (1000) rreme     (1000)     1068 2024-04-21 17:30:39.000000 torch_kf-0.0.1/LICENSE
--rw-r--r--   0 rreme     (1000) rreme     (1000)     5483 2024-04-23 22:46:06.761987 torch_kf-0.0.1/PKG-INFO
--rw-rw-r--   0 rreme     (1000) rreme     (1000)     4616 2024-04-23 22:43:16.000000 torch_kf-0.0.1/README.md
--rw-rw-r--   0 rreme     (1000) rreme     (1000)      139 2024-04-21 17:28:51.000000 torch_kf-0.0.1/pyproject.toml
--rw-rw-r--   0 rreme     (1000) rreme     (1000)     1008 2024-04-23 22:46:06.761987 torch_kf-0.0.1/setup.cfg
--rw-rw-r--   0 rreme     (1000) rreme     (1000)       54 2024-04-21 17:28:51.000000 torch_kf-0.0.1/setup.py
-drwxrwxr-x   0 rreme     (1000) rreme     (1000)        0 2024-04-23 22:46:06.761987 torch_kf-0.0.1/torch_kf/
--rw-rw-r--   0 rreme     (1000) rreme     (1000)      122 2024-04-23 08:52:40.000000 torch_kf-0.0.1/torch_kf/__init__.py
--rw-rw-r--   0 rreme     (1000) rreme     (1000)    17083 2024-04-23 09:55:32.000000 torch_kf-0.0.1/torch_kf/kalman_filter.py
--rw-rw-r--   0 rreme     (1000) rreme     (1000)        0 2024-04-21 17:29:00.000000 torch_kf-0.0.1/torch_kf/py.typed
-drwxrwxr-x   0 rreme     (1000) rreme     (1000)        0 2024-04-23 22:46:06.761987 torch_kf-0.0.1/torch_kf.egg-info/
--rw-r--r--   0 rreme     (1000) rreme     (1000)     5483 2024-04-23 22:46:06.000000 torch_kf-0.0.1/torch_kf.egg-info/PKG-INFO
--rw-rw-r--   0 rreme     (1000) rreme     (1000)      275 2024-04-23 22:46:06.000000 torch_kf-0.0.1/torch_kf.egg-info/SOURCES.txt
--rw-rw-r--   0 rreme     (1000) rreme     (1000)        1 2024-04-23 22:46:06.000000 torch_kf-0.0.1/torch_kf.egg-info/dependency_links.txt
--rw-rw-r--   0 rreme     (1000) rreme     (1000)        6 2024-04-23 22:46:06.000000 torch_kf-0.0.1/torch_kf.egg-info/requires.txt
--rw-rw-r--   0 rreme     (1000) rreme     (1000)        9 2024-04-23 22:46:06.000000 torch_kf-0.0.1/torch_kf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:31:07.097141 torch_kf-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-23 23:31:03.000000 torch_kf-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5483 2024-04-23 23:31:07.097141 torch_kf-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-04-23 23:31:03.000000 torch_kf-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-23 23:31:03.000000 torch_kf-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-23 23:31:07.097141 torch_kf-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-23 23:31:03.000000 torch_kf-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:31:07.093141 torch_kf-0.0.2/torch_kf/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-23 23:31:03.000000 torch_kf-0.0.2/torch_kf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17083 2024-04-23 23:31:03.000000 torch_kf-0.0.2/torch_kf/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 23:31:03.000000 torch_kf-0.0.2/torch_kf/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:31:07.093141 torch_kf-0.0.2/torch_kf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5483 2024-04-23 23:31:07.000000 torch_kf-0.0.2/torch_kf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-23 23:31:07.000000 torch_kf-0.0.2/torch_kf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 23:31:07.000000 torch_kf-0.0.2/torch_kf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 23:31:07.000000 torch_kf-0.0.2/torch_kf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 23:31:07.000000 torch_kf-0.0.2/torch_kf.egg-info/top_level.txt
```

### Comparing `torch_kf-0.0.1/LICENSE` & `torch_kf-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_kf-0.0.1/PKG-INFO` & `torch_kf-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-kf
-Version: 0.0.1
+Version: 0.0.2
 Summary: Kalman Filter implementation with PyTorch
 Home-page: https://github.com/raphaelreme/torch-kf
 Author: Raphael Reme
 Author-email: raphaelreme-dev@protonmail.com
 License: MIT
 Keywords: Kalman filter,statistics,pytorch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `torch_kf-0.0.1/README.md` & `torch_kf-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `torch_kf-0.0.1/setup.cfg` & `torch_kf-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `torch_kf-0.0.1/torch_kf/kalman_filter.py` & `torch_kf-0.0.2/torch_kf/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `torch_kf-0.0.1/torch_kf.egg-info/PKG-INFO` & `torch_kf-0.0.2/torch_kf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-kf
-Version: 0.0.1
+Version: 0.0.2
 Summary: Kalman Filter implementation with PyTorch
 Home-page: https://github.com/raphaelreme/torch-kf
 Author: Raphael Reme
 Author-email: raphaelreme-dev@protonmail.com
 License: MIT
 Keywords: Kalman filter,statistics,pytorch
 Classifier: Development Status :: 4 - Beta
```

