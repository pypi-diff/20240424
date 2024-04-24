# Comparing `tmp/aikicore-1.0.0a0.tar.gz` & `tmp/aikicore-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aikicore-1.0.0a0.tar", last modified: Tue Apr 23 23:18:09 2024, max compression
+gzip compressed data, was "aikicore-1.0.0a1.tar", last modified: Tue Apr 23 23:53:17 2024, max compression
```

## Comparing `aikicore-1.0.0a0.tar` & `aikicore-1.0.0a1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-23 23:18:09.445520 aikicore-1.0.0a0/
--rw-r--r--   0 ashatz     (501) staff       (20)     1509 2024-04-23 22:54:22.000000 aikicore-1.0.0a0/LICENSE
--rw-r--r--   0 ashatz     (501) staff       (20)      391 2024-04-23 23:18:09.445241 aikicore-1.0.0a0/PKG-INFO
-drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-23 23:18:09.443083 aikicore-1.0.0a0/aikicore/
--rw-r--r--   0 ashatz     (501) staff       (20)     2452 2024-04-23 22:57:31.000000 aikicore-1.0.0a0/aikicore/__init__.py
--rw-r--r--   0 ashatz     (501) staff       (20)       55 2024-04-23 22:57:31.000000 aikicore-1.0.0a0/aikicore/activity.py
-drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-23 23:18:09.444554 aikicore-1.0.0a0/aikicore/config/
--rw-r--r--   0 ashatz     (501) staff       (20)     3127 2024-04-23 22:57:31.000000 aikicore-1.0.0a0/aikicore/config/__init__.py
--rw-r--r--   0 ashatz     (501) staff       (20)      306 2024-04-23 22:57:31.000000 aikicore-1.0.0a0/aikicore/config/json.py
--rw-r--r--   0 ashatz     (501) staff       (20)      407 2024-04-23 22:57:31.000000 aikicore-1.0.0a0/aikicore/config/yaml.py
--rw-r--r--   0 ashatz     (501) staff       (20)      334 2024-04-23 22:57:31.000000 aikicore-1.0.0a0/aikicore/constants.py
--rw-r--r--   0 ashatz     (501) staff       (20)     2397 2024-04-23 22:57:31.000000 aikicore-1.0.0a0/aikicore/containers.py
--rw-r--r--   0 ashatz     (501) staff       (20)      395 2024-04-23 22:57:31.000000 aikicore-1.0.0a0/aikicore/domain.py
--rw-r--r--   0 ashatz     (501) staff       (20)     1571 2024-04-23 22:57:31.000000 aikicore-1.0.0a0/aikicore/error.py
--rw-r--r--   0 ashatz     (501) staff       (20)     5667 2024-04-23 22:57:31.000000 aikicore-1.0.0a0/aikicore/routing.py
-drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-23 23:18:09.444898 aikicore-1.0.0a0/aikicore.egg-info/
--rw-r--r--   0 ashatz     (501) staff       (20)      391 2024-04-23 23:18:09.000000 aikicore-1.0.0a0/aikicore.egg-info/PKG-INFO
--rw-r--r--   0 ashatz     (501) staff       (20)      395 2024-04-23 23:18:09.000000 aikicore-1.0.0a0/aikicore.egg-info/SOURCES.txt
--rw-r--r--   0 ashatz     (501) staff       (20)        1 2024-04-23 23:18:09.000000 aikicore-1.0.0a0/aikicore.egg-info/dependency_links.txt
--rw-r--r--   0 ashatz     (501) staff       (20)       32 2024-04-23 23:18:09.000000 aikicore-1.0.0a0/aikicore.egg-info/requires.txt
--rw-r--r--   0 ashatz     (501) staff       (20)        9 2024-04-23 23:18:09.000000 aikicore-1.0.0a0/aikicore.egg-info/top_level.txt
--rw-r--r--   0 ashatz     (501) staff       (20)       38 2024-04-23 23:18:09.445583 aikicore-1.0.0a0/setup.cfg
--rw-r--r--   0 ashatz     (501) staff       (20)      655 2024-04-23 23:12:52.000000 aikicore-1.0.0a0/setup.py
+drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-23 23:53:17.588173 aikicore-1.0.0a1/
+-rw-r--r--   0 ashatz     (501) staff       (20)     1509 2024-04-23 22:54:22.000000 aikicore-1.0.0a1/LICENSE
+-rw-r--r--   0 ashatz     (501) staff       (20)      391 2024-04-23 23:53:17.587933 aikicore-1.0.0a1/PKG-INFO
+drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-23 23:53:17.585932 aikicore-1.0.0a1/aikicore/
+-rw-r--r--   0 ashatz     (501) staff       (20)     2474 2024-04-23 23:51:15.000000 aikicore-1.0.0a1/aikicore/__init__.py
+-rw-r--r--   0 ashatz     (501) staff       (20)       55 2024-04-23 22:57:31.000000 aikicore-1.0.0a1/aikicore/activity.py
+drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-23 23:53:17.587448 aikicore-1.0.0a1/aikicore/config/
+-rw-r--r--   0 ashatz     (501) staff       (20)     3127 2024-04-23 22:57:31.000000 aikicore-1.0.0a1/aikicore/config/__init__.py
+-rw-r--r--   0 ashatz     (501) staff       (20)      306 2024-04-23 22:57:31.000000 aikicore-1.0.0a1/aikicore/config/json.py
+-rw-r--r--   0 ashatz     (501) staff       (20)      407 2024-04-23 22:57:31.000000 aikicore-1.0.0a1/aikicore/config/yaml.py
+-rw-r--r--   0 ashatz     (501) staff       (20)      334 2024-04-23 22:57:31.000000 aikicore-1.0.0a1/aikicore/constants.py
+-rw-r--r--   0 ashatz     (501) staff       (20)     2397 2024-04-23 22:57:31.000000 aikicore-1.0.0a1/aikicore/containers.py
+-rw-r--r--   0 ashatz     (501) staff       (20)      395 2024-04-23 22:57:31.000000 aikicore-1.0.0a1/aikicore/domain.py
+-rw-r--r--   0 ashatz     (501) staff       (20)     1571 2024-04-23 22:57:31.000000 aikicore-1.0.0a1/aikicore/error.py
+-rw-r--r--   0 ashatz     (501) staff       (20)     5667 2024-04-23 22:57:31.000000 aikicore-1.0.0a1/aikicore/routing.py
+drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-23 23:53:17.587687 aikicore-1.0.0a1/aikicore.egg-info/
+-rw-r--r--   0 ashatz     (501) staff       (20)      391 2024-04-23 23:53:17.000000 aikicore-1.0.0a1/aikicore.egg-info/PKG-INFO
+-rw-r--r--   0 ashatz     (501) staff       (20)      395 2024-04-23 23:53:17.000000 aikicore-1.0.0a1/aikicore.egg-info/SOURCES.txt
+-rw-r--r--   0 ashatz     (501) staff       (20)        1 2024-04-23 23:53:17.000000 aikicore-1.0.0a1/aikicore.egg-info/dependency_links.txt
+-rw-r--r--   0 ashatz     (501) staff       (20)       32 2024-04-23 23:53:17.000000 aikicore-1.0.0a1/aikicore.egg-info/requires.txt
+-rw-r--r--   0 ashatz     (501) staff       (20)        9 2024-04-23 23:53:17.000000 aikicore-1.0.0a1/aikicore.egg-info/top_level.txt
+-rw-r--r--   0 ashatz     (501) staff       (20)       38 2024-04-23 23:53:17.588223 aikicore-1.0.0a1/setup.cfg
+-rw-r--r--   0 ashatz     (501) staff       (20)      657 2024-04-23 23:52:54.000000 aikicore-1.0.0a1/setup.py
```

### Comparing `aikicore-1.0.0a0/LICENSE` & `aikicore-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `aikicore-1.0.0a0/aikicore/__init__.py` & `aikicore-1.0.0a1/aikicore/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Dict
 
 from .constants import APP_CONFIGURATION_FILE
 from .config import load_app_config_reader, AppConfigurationReader, AppConfiguration
 from .error import *
 from .containers import *
 from .routing import *
+from .domain import *
 
 
 class AppContext():
 
     name: str = None
     interface: str = None
     container_config: ContainerConfiguration = None
```

### Comparing `aikicore-1.0.0a0/aikicore/config/__init__.py` & `aikicore-1.0.0a1/aikicore/config/__init__.py`

 * *Files identical despite different names*

### Comparing `aikicore-1.0.0a0/aikicore/containers.py` & `aikicore-1.0.0a1/aikicore/containers.py`

 * *Files identical despite different names*

### Comparing `aikicore-1.0.0a0/aikicore/error.py` & `aikicore-1.0.0a1/aikicore/error.py`

 * *Files identical despite different names*

### Comparing `aikicore-1.0.0a0/aikicore/routing.py` & `aikicore-1.0.0a1/aikicore/routing.py`

 * *Files identical despite different names*

### Comparing `aikicore-1.0.0a0/setup.py` & `aikicore-1.0.0a1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 config = {
     'description': 'The Core Library for the Spirit of Harmony',
     'author': 'Andrew Shatz',
     'url': r'https://github.com/Great-Strength-Studios/aikicore',
     'download_url': r'https://github.com/Great-Strength-Studios/aikicore',
     'author_email': 'andrew@greatstrength.me',
-    'version': '1.0.0-alpha',
+    'version': '1.0.0-alpha.1',
     'license': 'BSD 3',
     'install_requires': [
         'schematics>=2.1.1',
         'pyyaml>=6.0.1'
     ],
     'packages': [
         'aikicore',
```

