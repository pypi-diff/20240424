# Comparing `tmp/lifx-photons-interactor-0.9.0.tar.gz` & `tmp/lifx-photons-interactor-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifx-photons-interactor-0.9.0.tar", last modified: Sun Aug 15 01:33:15 2021, max compression
+gzip compressed data, was "lifx-photons-interactor-0.9.1.tar", last modified: Sun Aug 15 01:53:54 2021, max compression
```

## Comparing `lifx-photons-interactor-0.9.0.tar` & `lifx-photons-interactor-0.9.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 01:33:15.558247 lifx-photons-interactor-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1081 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      100 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      769 2021-08-15 01:33:15.558247 lifx-photons-interactor-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      342 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 01:33:15.550247 lifx-photons-interactor-0.9.0/interactor/
--rw-r--r--   0 runner    (1001) docker     (121)      525 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3317 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/addon.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 01:33:15.550247 lifx-photons-interactor-0.9.0/interactor/commander/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/commander/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5349 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/commander/animations.py
--rw-r--r--   0 runner    (1001) docker     (121)     2829 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/commander/command.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 01:33:15.558247 lifx-photons-interactor-0.9.0/interactor/commander/commands/
--rw-r--r--   0 runner    (1001) docker     (121)      221 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/commander/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3611 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/commander/commands/animations.py
--rw-r--r--   0 runner    (1001) docker     (121)     1819 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/commander/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5096 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/commander/commands/control.py
--rw-r--r--   0 runner    (1001) docker     (121)     5393 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/commander/commands/effects.py
--rw-r--r--   0 runner    (1001) docker     (121)    10640 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/commander/commands/scenes.py
--rw-r--r--   0 runner    (1001) docker     (121)      396 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/commander/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     7859 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/commander/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2060 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/commander/spec_description.py
--rw-r--r--   0 runner    (1001) docker     (121)      255 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/commander/store.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 01:33:15.558247 lifx-photons-interactor-0.9.0/interactor/database/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8293 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/database/connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     3327 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/database/database.py
--rw-r--r--   0 runner    (1001) docker     (121)     3094 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/database/db_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 01:33:15.558247 lifx-photons-interactor-0.9.0/interactor/database/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)      494 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/database/migrations/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 01:33:15.558247 lifx-photons-interactor-0.9.0/interactor/database/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (121)     1212 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/database/migrations/versions/119f5f1434f7_add_scenes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1039 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/database/migrations/versions/aab549c5cdbd_add_scene_info.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 01:33:15.558247 lifx-photons-interactor-0.9.0/interactor/database/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/database/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1732 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/database/models/scene.py
--rw-r--r--   0 runner    (1001) docker     (121)      494 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/database/models/scene_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     6351 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/database/models/scene_spec.py
--rw-r--r--   0 runner    (1001) docker     (121)       98 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      978 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/options.py
--rw-r--r--   0 runner    (1001) docker     (121)     2981 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/request_handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)     5968 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/interactor/server.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 01:33:15.558247 lifx-photons-interactor-0.9.0/lifx_photons_interactor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      769 2021-08-15 01:33:15.000000 lifx-photons-interactor-0.9.0/lifx_photons_interactor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1412 2021-08-15 01:33:15.000000 lifx-photons-interactor-0.9.0/lifx_photons_interactor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-15 01:33:15.000000 lifx-photons-interactor-0.9.0/lifx_photons_interactor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-08-15 01:33:15.000000 lifx-photons-interactor-0.9.0/lifx_photons_interactor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      109 2021-08-15 01:33:15.000000 lifx-photons-interactor-0.9.0/lifx_photons_interactor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-08-15 01:33:15.000000 lifx-photons-interactor-0.9.0/lifx_photons_interactor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-15 01:33:15.558247 lifx-photons-interactor-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      964 2021-08-15 01:33:06.000000 lifx-photons-interactor-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 01:53:54.504020 lifx-photons-interactor-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)     1081 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      769 2021-08-15 01:53:54.504020 lifx-photons-interactor-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      342 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 01:53:54.500020 lifx-photons-interactor-0.9.1/interactor/
+-rw-r--r--   0 runner    (1001) docker     (121)      525 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3317 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/addon.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 01:53:54.500020 lifx-photons-interactor-0.9.1/interactor/commander/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/commander/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5349 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/commander/animations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2829 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/commander/command.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 01:53:54.500020 lifx-photons-interactor-0.9.1/interactor/commander/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)      221 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/commander/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3611 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/commander/commands/animations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1819 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/commander/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5096 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/commander/commands/control.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5393 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/commander/commands/effects.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10640 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/commander/commands/scenes.py
+-rw-r--r--   0 runner    (1001) docker     (121)      396 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/commander/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7859 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/commander/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2060 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/commander/spec_description.py
+-rw-r--r--   0 runner    (1001) docker     (121)      255 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/commander/store.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 01:53:54.500020 lifx-photons-interactor-0.9.1/interactor/database/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8293 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/database/connection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3327 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3094 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/database/db_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 01:53:54.504020 lifx-photons-interactor-0.9.1/interactor/database/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)      494 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/database/migrations/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 01:53:54.504020 lifx-photons-interactor-0.9.1/interactor/database/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (121)     1212 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/database/migrations/versions/119f5f1434f7_add_scenes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1039 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/database/migrations/versions/aab549c5cdbd_add_scene_info.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 01:53:54.504020 lifx-photons-interactor-0.9.1/interactor/database/models/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/database/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1732 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/database/models/scene.py
+-rw-r--r--   0 runner    (1001) docker     (121)      494 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/database/models/scene_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6463 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/database/models/scene_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)      978 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/options.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2981 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/request_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5968 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/interactor/server.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-15 01:53:54.504020 lifx-photons-interactor-0.9.1/lifx_photons_interactor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      769 2021-08-15 01:53:54.000000 lifx-photons-interactor-0.9.1/lifx_photons_interactor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1412 2021-08-15 01:53:54.000000 lifx-photons-interactor-0.9.1/lifx_photons_interactor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-15 01:53:54.000000 lifx-photons-interactor-0.9.1/lifx_photons_interactor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2021-08-15 01:53:54.000000 lifx-photons-interactor-0.9.1/lifx_photons_interactor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2021-08-15 01:53:54.000000 lifx-photons-interactor-0.9.1/lifx_photons_interactor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2021-08-15 01:53:54.000000 lifx-photons-interactor-0.9.1/lifx_photons_interactor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-15 01:53:54.504020 lifx-photons-interactor-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      964 2021-08-15 01:53:44.000000 lifx-photons-interactor-0.9.1/setup.py
```

### Comparing `lifx-photons-interactor-0.9.0/LICENSE` & `lifx-photons-interactor-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lifx-photons-interactor-0.9.0/PKG-INFO` & `lifx-photons-interactor-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: lifx-photons-interactor
-Version: 0.9.0
+Version: 0.9.1
 Summary: A server for interacting with LIFX lights over the LAN
 Home-page: http://github.com/delfick/photons/apps/interactor
 Author: Stephen Moore
 Author-email: github@delfick.com
 License: MIT
 Description: Photons Interactor
         ==================
```

### Comparing `lifx-photons-interactor-0.9.0/interactor/__init__.py` & `lifx-photons-interactor-0.9.1/interactor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-VERSION = "0.9.0"
+VERSION = "0.9.1"
 
 
 def run_pytest():
     import pytest
     import sys
 
     class EditConfig:
```

### Comparing `lifx-photons-interactor-0.9.0/interactor/addon.py` & `lifx-photons-interactor-0.9.1/interactor/addon.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-interactor-0.9.0/interactor/commander/animations.py` & `lifx-photons-interactor-0.9.1/interactor/commander/animations.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-interactor-0.9.0/interactor/commander/command.py` & `lifx-photons-interactor-0.9.1/interactor/commander/command.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-interactor-0.9.0/interactor/commander/commands/animations.py` & `lifx-photons-interactor-0.9.1/interactor/commander/commands/animations.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-interactor-0.9.0/interactor/commander/commands/base.py` & `lifx-photons-interactor-0.9.1/interactor/commander/commands/base.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-interactor-0.9.0/interactor/commander/commands/control.py` & `lifx-photons-interactor-0.9.1/interactor/commander/commands/control.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-interactor-0.9.0/interactor/commander/commands/effects.py` & `lifx-photons-interactor-0.9.1/interactor/commander/commands/effects.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-interactor-0.9.0/interactor/commander/commands/scenes.py` & `lifx-photons-interactor-0.9.1/interactor/commander/commands/scenes.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-interactor-0.9.0/interactor/commander/helpers.py` & `lifx-photons-interactor-0.9.1/interactor/commander/helpers.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-interactor-0.9.0/interactor/commander/spec_description.py` & `lifx-photons-interactor-0.9.1/interactor/commander/spec_description.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-interactor-0.9.0/interactor/database/connection.py` & `lifx-photons-interactor-0.9.1/interactor/database/connection.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-interactor-0.9.0/interactor/database/database.py` & `lifx-photons-interactor-0.9.1/interactor/database/database.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-interactor-0.9.0/interactor/database/db_queue.py` & `lifx-photons-interactor-0.9.1/interactor/database/db_queue.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-interactor-0.9.0/interactor/database/migrations/versions/119f5f1434f7_add_scenes.py` & `lifx-photons-interactor-0.9.1/interactor/database/migrations/versions/119f5f1434f7_add_scenes.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-interactor-0.9.0/interactor/database/migrations/versions/aab549c5cdbd_add_scene_info.py` & `lifx-photons-interactor-0.9.1/interactor/database/migrations/versions/aab549c5cdbd_add_scene_info.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-interactor-0.9.0/interactor/database/models/scene.py` & `lifx-photons-interactor-0.9.1/interactor/database/models/scene.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-interactor-0.9.0/interactor/database/models/scene_spec.py` & `lifx-photons-interactor-0.9.1/interactor/database/models/scene_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 class hsbk(sb.Spec):
     def __init__(self):
         self.specs = [
             range_spec(0, 360),
             range_spec(0, 1),
             range_spec(0, 1),
-            range_spec(2500, 9000, spec=sb.integer_spec()),
+            range_spec(1500, 9000, spec=sb.integer_spec()),
         ]
 
     def normalise_filled(self, meta, val):
         val = sized_list_spec(sb.any_spec(), 4).normalise(meta, val)
         res = []
         for i, (v, s) in enumerate(zip(val, self.specs)):
             res.append(s.normalise(meta.at(i), v))
@@ -162,19 +162,24 @@
                 power_message = self.power_message(overrides)
                 if power_message:
                     yield power_message
 
                 duration = self.determine_duration(overrides)
                 for i, lst in enumerate(self.chain):
                     colors = self.colors_from_hsbks(lst, overrides)
+
+                    width = 8
+                    if len(colors) == 30:
+                        width = 5
+
                     yield TileMessages.Set64(
                         tile_index=i,
                         length=1,
                         x=0,
                         y=0,
-                        width=8,
+                        width=width,
                         duration=duration,
                         colors=colors,
                         res_required=False,
                     )
 
     return Fields.FieldSpec()
```

### Comparing `lifx-photons-interactor-0.9.0/interactor/options.py` & `lifx-photons-interactor-0.9.1/interactor/options.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-interactor-0.9.0/interactor/request_handlers.py` & `lifx-photons-interactor-0.9.1/interactor/request_handlers.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-interactor-0.9.0/interactor/server.py` & `lifx-photons-interactor-0.9.1/interactor/server.py`

 * *Files identical despite different names*

### Comparing `lifx-photons-interactor-0.9.0/lifx_photons_interactor.egg-info/PKG-INFO` & `lifx-photons-interactor-0.9.1/lifx_photons_interactor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: lifx-photons-interactor
-Version: 0.9.0
+Version: 0.9.1
 Summary: A server for interacting with LIFX lights over the LAN
 Home-page: http://github.com/delfick/photons/apps/interactor
 Author: Stephen Moore
 Author-email: github@delfick.com
 License: MIT
 Description: Photons Interactor
         ==================
```

### Comparing `lifx-photons-interactor-0.9.0/lifx_photons_interactor.egg-info/SOURCES.txt` & `lifx-photons-interactor-0.9.1/lifx_photons_interactor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lifx-photons-interactor-0.9.0/setup.py` & `lifx-photons-interactor-0.9.1/setup.py`

 * *Files identical despite different names*

