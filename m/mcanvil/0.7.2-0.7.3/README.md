# Comparing `tmp/mcanvil-0.7.2.tar.gz` & `tmp/mcanvil-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcanvil-0.7.2.tar", last modified: Wed Mar 13 10:04:55 2024, max compression
+gzip compressed data, was "mcanvil-0.7.3.tar", last modified: Wed Apr 24 20:27:15 2024, max compression
```

## Comparing `mcanvil-0.7.2.tar` & `mcanvil-0.7.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:04:55.775107 mcanvil-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-13 10:04:51.000000 mcanvil-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-03-13 10:04:55.775107 mcanvil-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-03-13 10:04:51.000000 mcanvil-0.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-13 10:04:51.000000 mcanvil-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-03-13 10:04:55.775107 mcanvil-0.7.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:04:55.767107 mcanvil-0.7.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:04:55.767107 mcanvil-0.7.2/src/anvil/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:04:55.771107 mcanvil-0.7.2/src/anvil/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    84786 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/api/actors.py
--rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/api/blockbench.py
--rw-r--r--   0 runner    (1001) docker     (127)    27525 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/api/blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    31039 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/api/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)   227807 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/api/components.py
--rw-r--r--   0 runner    (1001) docker     (127)    30187 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/api/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    38964 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/api/features.py
--rw-r--r--   0 runner    (1001) docker     (127)    34114 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/api/items.py
--rw-r--r--   0 runner    (1001) docker     (127)    95903 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/api/molang.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/api/texture_pack.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/api/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    54579 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/api/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)   251032 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/api/vanilla.py
--rw-r--r--   0 runner    (1001) docker     (127)    18188 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:04:55.775107 mcanvil-0.7.2/src/anvil/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    31644 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/lib/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/lib/format_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8637 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/lib/lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14695 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/lib/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/lib/materials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/lib/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)    21299 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/lib/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/lib/sounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/lib/textures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:04:55.775107 mcanvil-0.7.2/src/anvil/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22412 2024-03-13 10:04:51.000000 mcanvil-0.7.2/src/anvil/tools/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:04:55.775107 mcanvil-0.7.2/src/mcanvil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-03-13 10:04:55.000000 mcanvil-0.7.2/src/mcanvil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-03-13 10:04:55.000000 mcanvil-0.7.2/src/mcanvil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 10:04:55.000000 mcanvil-0.7.2/src/mcanvil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-13 10:04:55.000000 mcanvil-0.7.2/src/mcanvil.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 10:04:55.000000 mcanvil-0.7.2/src/mcanvil.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-13 10:04:55.000000 mcanvil-0.7.2/src/mcanvil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-13 10:04:55.000000 mcanvil-0.7.2/src/mcanvil.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:27:15.532363 mcanvil-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 20:27:11.000000 mcanvil-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-24 20:27:15.532363 mcanvil-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-24 20:27:11.000000 mcanvil-0.7.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 20:27:11.000000 mcanvil-0.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-24 20:27:15.532363 mcanvil-0.7.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:27:15.524363 mcanvil-0.7.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:27:15.524363 mcanvil-0.7.3/src/anvil/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:27:15.528363 mcanvil-0.7.3/src/anvil/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89516 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/api/actors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/api/blockbench.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27515 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/api/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32083 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/api/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)   249766 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/api/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31125 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/api/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40436 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/api/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34447 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/api/items.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96987 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/api/molang.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/api/texture_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/api/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54579 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/api/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)   258421 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/api/vanilla.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18415 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:27:15.532363 mcanvil-0.7.3/src/anvil/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8796 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31965 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/lib/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/lib/format_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8637 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/lib/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15532 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/lib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/lib/materials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/lib/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21533 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/lib/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/lib/sounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/lib/textures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:27:15.532363 mcanvil-0.7.3/src/anvil/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22412 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/tools/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:27:15.532363 mcanvil-0.7.3/src/mcanvil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-24 20:27:15.000000 mcanvil-0.7.3/src/mcanvil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-24 20:27:15.000000 mcanvil-0.7.3/src/mcanvil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 20:27:15.000000 mcanvil-0.7.3/src/mcanvil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-24 20:27:15.000000 mcanvil-0.7.3/src/mcanvil.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 20:27:15.000000 mcanvil-0.7.3/src/mcanvil.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 20:27:15.000000 mcanvil-0.7.3/src/mcanvil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 20:27:15.000000 mcanvil-0.7.3/src/mcanvil.egg-info/top_level.txt
```

### Comparing `mcanvil-0.7.2/LICENSE` & `mcanvil-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mcanvil-0.7.2/PKG-INFO` & `mcanvil-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcanvil
-Version: 0.7.2
+Version: 0.7.3
 Summary: A Minecraft bedrock content development framework.
 Home-page: https://anvil.starktma.net/
 Author: Yasser A. Benfoughal
 Author-email: yasser@starktma.net
 License: GNU GPLv3
 Project-URL: Github, https://github.com/StarkTMA/Anvil
 Project-URL: Website, https://starktma.net
@@ -32,15 +32,15 @@
 Requires-Dist: reportlab
 
 <img src="https://starktma.net/wp-content/uploads/2022/04/logo.png" width="300" alt="Anvil Logo">
 
 # Anvil
 
 ![Python 10](https://img.shields.io/badge/python-3.10%20%20|%20%203.11%20%20|%20%203.12-g.svg)
-![Anvil Version](https://img.shields.io/badge/beta-0.7.2-yellow.svg)
+![Anvil Version](https://img.shields.io/badge/beta-0.7.3-yellow.svg)
 ![OS](https://img.shields.io/badge/OS-Windows-blue.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ---
 
 ## What is Anvil?
```

### Comparing `mcanvil-0.7.2/README.md` & `mcanvil-0.7.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <img src="https://starktma.net/wp-content/uploads/2022/04/logo.png" width="300" alt="Anvil Logo">
 
 # Anvil
 
 ![Python 10](https://img.shields.io/badge/python-3.10%20%20|%20%203.11%20%20|%20%203.12-g.svg)
-![Anvil Version](https://img.shields.io/badge/beta-0.7.2-yellow.svg)
+![Anvil Version](https://img.shields.io/badge/beta-0.7.3-yellow.svg)
 ![OS](https://img.shields.io/badge/OS-Windows-blue.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ---
 
 ## What is Anvil?
```

### Comparing `mcanvil-0.7.2/setup.cfg` & `mcanvil-0.7.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `mcanvil-0.7.2/src/anvil/api/actors.py` & `mcanvil-0.7.3/src/anvil/api/actors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import json
 import os
 from enum import StrEnum
 
 import requests
+from halo import Halo
+from PIL import Image
+
 from anvil import ANVIL, CONFIG
+from anvil.api import vanilla
 from anvil.api.blockbench import Animation, Geometry
 from anvil.api.components import Filter, InstantDespawn, Rideable, _component
 from anvil.api.enums import Difficulty, Population, Target, Vibrations
 from anvil.api.molang import Query, Variable
 from anvil.api.types import Identifier, Molang, event
 from anvil.api.vanilla import ENTITY_LIST, ITEMS_LIST, Entities
 from anvil.lib.lib import MOLANG_PREFIXES, CopyFiles, File, FileExists
 from anvil.lib.reports import ReportType
 from anvil.lib.schemas import AddonObject, JsonSchemes, MinecraftDescription
 from anvil.lib.sounds import EntitySoundEvent, SoundCategory, SoundDescription
-from halo import Halo
-from PIL import Image
 
 __all__ = ["Entity", "Attachable"]
 
 
 class _ActorDescription(MinecraftDescription):
     """Base class for all actor descriptions."""
 
@@ -88,14 +90,74 @@
         self._description["description"]["animations"].update(
             {
                 animation_shortname: f"animation.{CONFIG.NAMESPACE}.{geometry_name}.{animation_shortname}"
             }
         )
 
 
+class _ActorReuseAssets:
+    def __init__(self, client: "_ActorClientDescription") -> None:
+        self.client = client
+
+    def animation(self, shortname: str, animation_name: str, animate: bool = False, condition: str | Molang = None):
+        if animate is True:
+            if condition is None:
+                self.client._animate_append(shortname)
+            else:
+                self.client._animate_append({shortname: condition})
+
+        self.client._description["description"]["animations"].update(
+            {
+                shortname: animation_name
+            }
+        )
+    
+    def animation_controller(self, shortname: str, animation_controller_name: str, animate: bool = False, condition: str | Molang = None):
+        if animate is True:
+            if condition is None:
+                self.client._animate_append(shortname)
+            else:
+                self.client._animate_append({shortname: condition})
+
+        self.client._description["description"]["animations"].update(
+            {
+                shortname: animation_controller_name
+            }
+        )
+
+    def texture(self, shortname: str, texture_name: str):
+        self.client._description["description"]["textures"].update(
+            {shortname: texture_name}
+        )
+    
+    def geometry(self, shortname: str, geometry_name: str):
+        self.client._description["description"]["geometry"].update(
+            {shortname: geometry_name}
+        )
+    
+    def particle_effect(self, shortname: str, particle_name: str):
+        self.client._description["description"]["particle_effects"].update(
+            {shortname: particle_name}
+        )
+
+    def sound_effect(self, shortname: str, sound_name: str):
+        self.client._description["description"]["sound_effects"].update(
+            {shortname: sound_name}
+        )
+    
+    def spawn_egg(self, item_sprite: str, texture_index: int = 0):
+        self.client._description["description"]["spawn_egg"] = {"texture": item_sprite, "texture_index": texture_index}
+
+    def render_controller(self, controller_name: str, condition: str = None):
+        if condition is None:
+            self.client._description["description"]["render_controllers"].append(controller_name)
+        else:
+            self.client._description["description"]["render_controllers"].append({controller_name: condition})
+
+
 class _ActorClientDescription(_ActorDescription):
     _queued_models = set()
     _queued_textures = set()
     _queued_animations = set()
     _queued_animation_controllers = set()
     _type = "entity"
 
@@ -110,14 +172,18 @@
             name (str): The name of the actor.
             is_vanilla (bool, optional): Whether or not the actor is a vanilla actor. Defaults to False.
             type (str, optional): The type of the actor. Defaults to "entity".
         """
         super().__init__(name, is_vanilla)
         if self._type not in ["entity", "attachables"]:
             CONFIG.Logger.client_type_unsupported(self._type, self.identifier)
+        
+        if is_vanilla and ENTITY_LIST.get(self.name) is None:
+            CONFIG.Logger.entity_not_valid_vanilla(self.name)
+
         self._is_vanilla = is_vanilla
         self._animation_controllers = _RP_AnimationControllers(self._name, self._is_vanilla)
         self._render_controllers = _RenderControllers(self._name, self._is_vanilla)
         self._description["description"].update(JsonSchemes.client_description())
 
         self._sounds: list[SoundDescription] = []
 
@@ -239,14 +305,24 @@
 
             _ActorClientDescription._queued_models.add(geometry_name)
 
         self._description["description"]["geometry"].update({geometry_shortname: geo_namespace})
 
         return self
 
+    def queryable_geometry(self, geometry_shortname: str):
+        """This method manages the queryable geometry for an entity.
+
+        Args:
+            geometry_shortname (str): The shortname of the geometry.
+
+        """
+        self._description["description"]["queryable_geometry"] = f"geometry.{CONFIG.NAMESPACE}.{geometry_shortname}"
+        return self
+    
     def texture(self, texture_id: str, texture_name: str):
         """This method manages the textures for an entity.
 
         Args:
             texture_id (str): The id of the texture.
             texture_name (str): The name of the texture.
 
@@ -261,15 +337,15 @@
             {texture_id: os.path.join("textures", CONFIG.NAMESPACE, CONFIG.PROJECT_NAME, "actors", texture_name)}
         )
 
         return self
 
     def script(self, variable: Variable | str, script: Molang | str):
         """This method manages the scripts for an entity."""
-        self._description["description"]["scripts"]["pre_animation"].append(f"{variable}={script};")
+        self._description["description"]["scripts"]["pre_animation"].append(f"{variable}={script};".replace(";;", ";"))
         return self
 
     def init_vars(self, **vars):
         """Initializes variables for an entity.
 
         Examples:
             >>> Entity("example").init_vars(x=0, y=5, z=8)
@@ -284,14 +360,44 @@
 
         Args:
             scale (str | Molang, optional): The scale of the entity. Defaults to "1".
         """
         if not scale == "1":
             self._description["description"]["scripts"].update({"scale": str(scale)})
 
+    def should_update_bones_and_effects_offscreen(self, bool: bool = False):
+        """Sets whether or not the entity should update bones and effects offscreen.
+
+        Args:
+            bool (bool, optional): Whether or not the entity should update bones and effects offscreen. Defaults to False.
+        """
+        self._description["description"]["scripts"]["update_bones_and_effects_offscreen"] = str(int(bool))
+
+    def should_update_effects_offscreen(self, bool: bool = False):
+        """Sets whether or not the entity should update effects offscreen.
+
+        Args:
+            bool (bool, optional): Whether or not the entity should update effects offscreen. Defaults to False.
+        """
+        self._description["description"]["scripts"]["update_effects_offscreen"] = str(int(bool))
+
+
+    def scaleXYZ(self, x: Molang | str = "1", y: Molang | str = "1", z: Molang | str = "1"):
+        """Sets the scale of the entity.
+
+        Args:
+            x (str | Molang, optional): The x scale of the entity. Defaults to "1".
+            y (str | Molang, optional): The y scale of the entity. Defaults to "1".
+            z (str | Molang, optional): The z scale of the entity. Defaults to "1".
+        """
+        if not x == "1" or not y == "1" or not z == "1":
+            self._description["description"]["scripts"]["scalex"] = str(x)
+            self._description["description"]["scripts"]["scaley"] = str(y)
+            self._description["description"]["scripts"]["scalez"] = str(z)
+
     def render_controller(self, controller_name: str, condition: str = None):
         """This method manages the render controllers for an entity.
 
         Args:
             controller_name (str): The name of the render controller.
             condition (str, optional): The condition to render the render controller. Defaults to None.
 
@@ -306,114 +412,100 @@
     def particle_effect(self, particle_name: str):
         """This method manages the particle effects for an entity.
 
         Args:
             particle_name (str): The name of the particle effect.
 
         """
+        from anvil.api.features import Particle
         self._particle_name = particle_name
         self._description["description"]["particle_effects"].update(
             {self._particle_name: f"{CONFIG.NAMESPACE}:{self._particle_name}"}
         )
+        Particle(self._particle_name).queue()
         return self
 
     def sound_effect(
         self,
         sound_name: str,
         sound_reference: str,
         category: SoundCategory = SoundCategory.Neutral,
         max_distance: int = 0,
         min_distance: int = 9999,
     ):
         """This method manages the sound effects for an entity.
 
         Args:
             sound_shortname (str): The shortname of the sound effect.
-            sound_identifier (str): The identifier of the sound effect.
+            sound_reference (str): The identifier of the sound effect.
             category (SoundCategory, optional): The category of the sound effect. Defaults to SoundCategory.Neutral.
 
         """
         self._description["description"]["sound_effects"].update({sound_name: f"{CONFIG.NAMESPACE}:{sound_reference}"})
         sound: SoundDescription = ANVIL.definitions.register_sound_definition(
             sound_reference, category, max_distance=max_distance, min_distance=min_distance
         )
         self._sounds.append(sound)
         return sound
 
     def sound_event(
         self,
-        sound_identifier,
+        sound_reference,
         sound_event: EntitySoundEvent,
         category: SoundCategory = SoundCategory.Neutral,
         volume: float = 1.0,
         pitch: tuple[float, float] = (0.8, 1.2),
         max_distance: int = 0,
         min_distance: int = 9999,
     ):
         """This method manages the sound events for an entity.
 
         Args:
-            sound_identifier (_type_): The identifier of the sound effect.
+            sound_reference (_type_): The identifier of the sound effect.
             sound_event (EntitySoundEvent): The sound event.
             category (SoundCategory, optional): The category of the sound effect. Defaults to SoundCategory.Neutral.
             volume (float, optional): The volume of the sound effect. Defaults to 1.0.
             pitch (tuple[float, float], optional): The pitch of the sound effect. Defaults to (0.8, 1.2).
 
         """
-        ANVIL.definitions.register_sound_event(self.identifier, sound_identifier, sound_event, volume, pitch)
+        ANVIL.definitions.register_entity_sound_event(self.identifier, sound_reference, sound_event, volume, pitch)
 
         sound: SoundDescription = ANVIL.definitions.register_sound_definition(
-            sound_identifier, category, max_distance=max_distance, min_distance=min_distance
+            sound_reference, category, max_distance=max_distance, min_distance=min_distance
         )
         self._sounds.append(sound)
         return sound
 
     @Halo("Retrieving vanilla entity description")
     def get_vanilla(self):
         if self.is_vanilla:
-            cache_path = os.path.join("assets", "cache", f"{self.name}.entity.json")
-            data = {}
-            if FileExists(cache_path):
-                with open(cache_path, "r") as file:
-                    data = json.loads(file.read())
-            else:
-                retrieve = requests.get(
-                    f"https://raw.githubusercontent.com/Mojang/bedrock-samples/main/resource_pack/entity/{self.name}.entity.json"
-                )
-                data = json.loads(retrieve.text)
+            data = ENTITY_LIST.get(self.name).get_vanilla_resource()
             self._description["description"].update(data["minecraft:client_entity"]["description"])
-            File(f"{self.name}.entity.json", data, os.path.join("assets", "cache"), "w", True)
 
     def to_dict(self, directory: str = None):
         """Queues the entity for export.
 
         Args:
             directory (str, optional): The directory to export the entity to. Defaults to None.
 
         Raises:
             RuntimeError: If the entity does not have a geometry, texture, or render controller.
             Exception: If a geometry is reused but the entity it is reused from has not been queued yet.
 
         """
-        from anvil.api.features import Particle
 
         if len(self._description["description"]["geometry"]) == 0:
             CONFIG.Logger.missing_geometry(self.identifier)
 
         if len(self._description["description"]["textures"]) == 0:
             CONFIG.Logger.missing_texture(self.identifier)
 
         if len(self._description["description"]["render_controllers"]) == 0:
             CONFIG.Logger.missing_render_controller(self.identifier)
 
-        # TODO: Replace once a proper particle integration is added.
-        if "particle_effects" in self._description["description"]:
-            for particle in self._description["description"]["particle_effects"]:
-                Particle(particle).queue()
-
         for sound in self._sounds:
             sound._export
 
         self._render_controllers.queue(directory)
         self._animation_controllers.queue(directory)
 
         return super().to_dict
@@ -516,36 +608,40 @@
                 CONFIG.Logger.experimental_not_allowed(self.identifier)
         else:
             CONFIG.Logger.entity_marked_as_experimental(self.identifier)
 
         self._description["description"]["is_experimental"] = True
         return self
 
-    def RuntimeIdentifier(self, entity: Entities.vanilla_entity):
+    def RuntimeIdentifier(self, entity: Entities.VanillaEntity):
         """Sets the runtime identifier of the entity.
 
         Args:
-            entity (Entities.vanilla_entity): The vanilla entity to get the runtime identifier from.
+            entity (Entities.VanillaEntity): The vanilla entity to get the runtime identifier from.
         """
         if CONFIG._TARGET != "addon":
-            if not type(entity) is Entities.vanilla_entity:
+            if not type(entity) is Entities.VanillaEntity:
                 CONFIG.Logger.runtime_entity_error(entity)
             else:
-                if entity._allow_runtime:
+                if entity.allow_runtime:
                     self._description["description"]["runtime_identifier"] = entity.identifier
                 else:
                     CONFIG.Logger.runtime_entity_not_allowed(entity)
         else:
             CONFIG.Logger.runtime_not_allowed(self.identifier)
 
     @property
     def add_property(self):
         """Adds a property to the entity."""
         return self._properties
 
+    def spawn_category(self):
+        """Sets the spawn category of the entity."""
+        self._description["description"]["spawn_category"] = "none"
+
     @property
     def _export(self):
         """Exports the entity description."""
         self._description["description"]["properties"] = self._properties._export
         return super().to_dict
 
 
@@ -576,23 +672,32 @@
 
     @property
     def HideArmor(self):
         """This determines if the armor should be hidden."""
         self._description["description"]["hide_armor"] = True
         return self
 
-    def spawn_egg(self, item_sprite: str):
+    def spawn_egg(self, item_sprite: str, texture_index: int = 0):
         """This method adds a spawn egg texture to the entity.
 
         Args:
             item_sprite (str): The name of the item sprite.
         """
         ANVIL.definitions.register_item_textures(item_sprite, "spawn_eggs", item_sprite)
-        self._description["description"]["spawn_egg"] = {"texture": f"{CONFIG.NAMESPACE}:{item_sprite}"}
+        self._description["description"]["spawn_egg"] = {"texture": f"{CONFIG.NAMESPACE}:{item_sprite}", "texture_index": texture_index if texture_index == 0 else {}}
+
+    def spawn_egg_color(self, base_color: str, overlay_color: str):
+        """This method adds a spawn egg color to the entity.
 
+        Args:
+            base_color (str): The base color of the spawn egg.
+            overlay_color (str): The overlay color of the spawn egg.
+        """
+        self._description["description"]["spawn_egg"] = {"base_color": base_color, "overlay_color": overlay_color}
+        
     def to_dict(self, directory: str):
         """Queues the entity for export.
 
         Args:
             directory (str): The directory to export the entity to.
 
         """
@@ -641,14 +746,19 @@
 
         Args:
             name (str): The name of the attachable.
             is_vanilla (bool, optional): Whether or not the attachable is a vanilla attachable. Defaults to False.
         """
         super().__init__(name, is_vanilla)
 
+    @property
+    def reuse_assets(self):
+        """Whether or not the actor should reuse assets from another actor."""
+        return _ActorReuseAssets(self._description)
+
 
 class _EntityServer(AddonObject):
     """Base class for all server entities."""
 
     _extension = ".behavior.json"
     _path = os.path.join(CONFIG.BP_PATH, "entities")
 
@@ -784,15 +894,15 @@
             if controller.startswith("controller.") and controller not in controllers:
                 cleared_items.append(key)
         
         for item in cleared_items:
             self._description._description["description"]["animations"].pop(item)
             
         if Rideable.component_namespace in json.dumps(self._server_entity):
-            ANVIL.definitions.register_lang(f"action.hint.exit.{self.identifier}", "Hold shift to exit")
+            ANVIL.definitions.register_lang(f"action.hint.exit.{self.identifier}", "Sneak to exit")
 
         super().queue(directory=directory)
 
 
 class _EntityClient(AddonObject):
     """Base class for all client entities."""
 
@@ -813,14 +923,19 @@
 
     @property
     def description(self):
         """Returns the entity description."""
         return self._description
 
     @property
+    def reuse_assets(self):
+        """Whether or not the actor should reuse assets from another actor."""
+        return _ActorReuseAssets(self._description)
+    
+    @property
     def identifier(self) -> str:
         return self.description.identifier
 
     def queue(self, directory: str = None):
         """Queues the entity for export.
 
         Args:
@@ -1166,15 +1281,15 @@
         Returns
         -------
             This state.
 
         """
         particle = {"effect": effect, "locator": locator}
         if pre_anim_script is not None:
-            particle.update({"pre_effect_script": pre_anim_script})
+            particle.update({"pre_effect_script": f"{pre_anim_script};".replace(";;", ";")})
         if bind_to_actor is False:
             particle.update({"bind_to_actor": False})
         self._controller_state[self._state_name]["particle_effects"].append(particle)
         self._default = False
         return self
 
     def sound_effect(self, effect: str):
@@ -2194,15 +2309,16 @@
         self._component_group_name = "components"
         self._components: dict[str, _component] = {}
 
     def _set(self, key: str, value: _component):
         self._components[key] = value
 
     def _remove(self, key: str):
-        self._components.pop(key)
+        if key in self._components.keys():
+            self._components.pop(key)
 
     def _has(self, key: str):
         return key in self._components
 
     def add(self, *components: _component):
         for component in components:
             self._set(component.component_namespace, component)
@@ -2295,21 +2411,21 @@
 class Entity:
     def _validate_name(self, name: str):
         if ":" in name:
             CONFIG.Logger.namespaces_not_allowed(name)
         if not name[0].isalpha():
             CONFIG.Logger.digits_not_allowed(name)
 
-    def __init__(self, name: str) -> None:
-        self._is_vanilla = name in ENTITY_LIST
-        self._name = name if not self._is_vanilla else str(name)
-        self._namespace_format = "minecraft" if self._is_vanilla else CONFIG.NAMESPACE
+    def __init__(self, name: str, is_vanilla: bool = False) -> None:
+        self._is_vanilla = is_vanilla
+        self._name = name if not is_vanilla else str(name)
+        self._namespace_format = "minecraft" if is_vanilla else CONFIG.NAMESPACE
         self._validate_name(self._name)
 
-        if CONFIG._TARGET == "addon" and self._is_vanilla:
+        if CONFIG._TARGET == "addon" and is_vanilla:
             CONFIG.Logger.vanilla_override_error(self._name)
 
         self._server = _EntityServer(self._name, self._is_vanilla)
         self._client = _EntityClient(self._name, self._is_vanilla)
 
     @property
     def Server(self):
```

### Comparing `mcanvil-0.7.2/src/anvil/api/blockbench.py` & `mcanvil-0.7.3/src/anvil/api/blockbench.py`

 * *Files identical despite different names*

### Comparing `mcanvil-0.7.2/src/anvil/api/blocks.py` & `mcanvil-0.7.3/src/anvil/api/blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from enum import StrEnum
 
 from anvil import ANVIL, CONFIG
 from anvil.api.actors import _Components
 from anvil.api.components import _component
-from anvil.api.enums import (BlockCategory, BlockFaces, BlockGroups,
-                             BlockMaterial, PlacementDirectionTrait,
+from anvil.api.enums import (BlockFaces, BlockMaterial, ItemCategory,
+                             ItemGroups, PlacementDirectionTrait,
                              PlacementPositionTrait)
 from anvil.api.types import Molang, coordinates, position
 from anvil.lib.lib import CopyFiles, FileExists, clamp
 from anvil.lib.reports import ReportType
 from anvil.lib.schemas import AddonObject, JsonSchemes, MinecraftDescription
 
 __all__ = [
@@ -508,25 +508,25 @@
 
         """
         if len(range) > 16:
             CONFIG.Logger.block_state_values_out_of_range(self._name, name, len(range))
         self._description["description"]["states"][f"{CONFIG.NAMESPACE}:{name}"] = range
         return self
 
-    def menu_category(self, category: BlockCategory = BlockCategory.none, group: BlockGroups | str = BlockGroups.none, ):
+    def menu_category(self, category: ItemCategory = ItemCategory.none, group: ItemGroups | str = ItemGroups.none, ):
         """Sets the menu category for the block.
 
         Args:
-            category (BlockCategory, optional): The category of the block. Defaults to BlockCategory.none.
+            category (ItemCategory, optional): The category of the block. Defaults to ItemCategory.none.
             group (str, optional): The group of the block. Defaults to None.
 
         """
         self._description["description"]["menu_category"] = {
-            "category": category.value if not category == BlockCategory.none else {},
-            "group": group if not group == BlockGroups.none else {},
+            "category": category.value if not category == ItemCategory.none else {},
+            "group": group if not group == ItemGroups.none else {},
         }
         return self
 
     @property
     def is_hidden_in_commands(self):
         self._description["description"]["is_hidden_in_commands"] = True
         return self
```

### Comparing `mcanvil-0.7.2/src/anvil/api/commands.py` & `mcanvil-0.7.3/src/anvil/api/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import json
 from enum import StrEnum
 from math import inf
 
 from anvil import CONFIG
 from anvil.api.blocks import Block
-from anvil.api.enums import Anchor, CameraEasing, CameraPresets, CameraShakeType, CloneMode, DamageCause, Dimension, Effects, FillMode, Gamemodes, InputPermissions, MaskMode, MusicRepeatMode, RawTextConstructor, ScoreboardOperation, ScoreboardOperator, Selector, Slots, Target, TimeSpec
-from anvil.api.vanilla import Blocks
-from anvil.lib.lib import clamp, normalize_180
+from anvil.api.enums import (Anchor, CameraEasing, CameraPresets,
+                             CameraShakeType, CloneMode, DamageCause,
+                             Dimension, Effects, FillMode, Gamemodes,
+                             HudElement, HudVisibility, InputPermissions,
+                             MaskMode, MusicRepeatMode, RawTextConstructor,
+                             ScoreboardOperation, ScoreboardOperator, Selector,
+                             Slots, Target, TimeSpec)
 from anvil.api.types import (Color, Identifier, Seconds, coordinate,
                              coordinates, event, position, rotation, tick)
-
+from anvil.api.vanilla import Blocks
+from anvil.lib.lib import clamp, normalize_180
 
 
 class Command:
     def __init__(self, prefix: str, *commands) -> None:
         self._prefix = prefix
         self._components = {}
         self._command = f"{self._prefix} {' '.join([str(cmd) for cmd in commands])}"
@@ -437,25 +442,27 @@
         super().__init__("clear", target, itemname, date if not date == -1 else "", max_count if not max_count == -1 else "")
 
 
 class Effect(Command):
     def __init__(self, target: Selector) -> None:
         super().__init__("effect", target)
 
-    @property
     def clear(self):
         self._append_cmd("clear")
         return self
 
     def give(self, effect: Effects, seconds: int, amplifier: int, hide_particles: bool = False):
         self._append_cmd(effect, seconds, amplifier)
         if hide_particles:
             self._append_cmd("true")
         return self
 
+    def remove(self, effect: Effects):
+        self._append_cmd(effect, 0)
+        return self
 
 class Gamemode(Command):
     def __init__(self, target: str, gamemode: Gamemodes):
         super().__init__("gamemode", gamemode, target)
 
 
 class Teleport(Command):
@@ -928,7 +935,24 @@
 
         [Documentation reference]: https://learn.microsoft.com/en-gb/minecraft/creator/commands/commands/stopsound
         """
         super().__init__("stopsound", target)
 
         if not sound == "":
             self._append_cmd(f'"{sound}"')
+
+
+class Hud(Command):
+    def __init__(self, target: Selector | Target, visible: HudVisibility = HudVisibility.Reset, hud_element: HudElement = HudElement.All):
+        """Changes the visibility of HUD elements for a player.
+
+        Args:
+            target (Selector | Target): The player to change the HUD visibility for.
+            visible (HudVisibility, optional): The visibility state to set. Defaults to HudVisibility.Reset.
+            hud_element (HudElement, optional): The HUD element to change the visibility of. Defaults to HudElement.All.
+
+        [Documentation reference]: https://learn.microsoft.com/en-gb/minecraft/creator/commands/commands/hud
+        """
+
+        super().__init__("hud", target, visible, hud_element)
+        return self
+
```

### Comparing `mcanvil-0.7.2/src/anvil/api/components.py` & `mcanvil-0.7.3/src/anvil/api/components.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import math
 from typing import Union
 
 from anvil import ANVIL, CONFIG
-from anvil.api.enums import (Biomes, ControlFlags, DamageCause, Effects,
-                             FilterEquipmentDomain, FilterOperation,
-                             FilterSubject, RawTextConstructor, Selector,
-                             Target, Vibrations)
+from anvil.api.enums import (Biomes, ContainerType, ControlFlags, DamageCause,
+                             Difficulty, Effects, FilterEquipmentDomain,
+                             FilterOperation, FilterSubject,
+                             RawTextConstructor, Selector, Slots, Target,
+                             Vibrations)
 from anvil.api.features import Particle
 from anvil.api.types import (Identifier, Molang, Seconds, coordinates, event,
                              position)
 from anvil.api.vanilla import Blocks
 from anvil.lib.format_versions import ENTITY_SERVER_VERSION
-from anvil.lib.lib import *
+from anvil.lib.lib import clamp
 
 
 class EventObject:
     def __init__(self, event: event, target: Selector | Target) -> None:
         return {"event": event, "target": target}
 
 
@@ -472,14 +473,55 @@
         value: str,
         *,
         subject: FilterSubject = FilterSubject.Self,
         operator: FilterOperation = FilterOperation.Equals,
     ):
         return self._construct_filter("was_last_hurt_by", subject, operator, None, value)
 
+    @classmethod
+    def has_tag(
+        self,
+        value: str,
+        *,
+        subject: FilterSubject = FilterSubject.Self,
+        operator: FilterOperation = FilterOperation.Equals,
+    ):
+        return self._construct_filter("has_tag", subject, operator, None, value)
+
+    @classmethod
+    def is_difficulty(
+        self,
+        value: Difficulty,
+        *,
+        subject: FilterSubject = FilterSubject.Self,
+        operator: FilterOperation = FilterOperation.Equals,
+    ):
+        return self._construct_filter("is_difficulty", subject, operator, None, str(value))
+
+    @classmethod
+    def is_sitting(
+        self,
+        value: bool,
+        *,
+        subject: FilterSubject = FilterSubject.Self,
+        operator: FilterOperation = FilterOperation.Equals,
+    ):
+        return self._construct_filter("is_sitting", subject, operator, None, value)
+   
+    @classmethod
+    def has_damaged_equipment(
+        self,
+        value: str,
+        domain: FilterEquipmentDomain,
+        *,
+        subject: FilterSubject = FilterSubject.Self,
+        operator: FilterOperation = FilterOperation.Equals,
+    ):
+        return self._construct_filter("has_damaged_equipment", subject, operator, domain, value)
+
 # Components ==========================================================================
 
 
 class AddRider(_component):
     component_namespace = "minecraft:addrider"
 
     def __init__(self, entity_type: Identifier, spawn_event: event = None) -> None:
@@ -648,14 +690,15 @@
     def __init__(self, height: float, width: float, pivot: list[float, float, float] = [0, 1, 0]) -> None:
         """List of hitboxes for melee and ranged hits against the entity."""
         super().__init__("custom_hit_test")
         self._component_add_field("hitboxes", [{"width": width, "height": height, "pivot": pivot}])
 
     def add_hitbox(self, height: float, width: float, pivot: list[float, float, float] = [0, 1, 0]):
         self[self.component_namespace]["hitboxes"].append({"width": width, "height": height, "pivot": pivot})
+        return self
 
 
 class CanClimb(_component):
     component_namespace = "minecraft:can_climb"
 
     def __init__(self) -> None:
         """Allows this entity to climb up ladders."""
@@ -674,19 +717,18 @@
         if not effect_name is None:
             self._component_add_field("effect_name", effect_name)
 
 
 class JumpStatic(_component):
     component_namespace = "minecraft:jump.static"
 
-    def __init__(self, jump_power: float = 0.6) -> None:
+    def __init__(self, jump_power: float = 0.42) -> None:
         """Gives the entity the ability to jump."""
         super().__init__("jump.static")
-        if not jump_power == 0.6:
-            self._component_add_field("jump_power", jump_power)
+        self._component_add_field("jump_power", jump_power)
 
 
 class HorseJumpStrength(_component):
     component_namespace = "minecraft:horse.jump_strength"
 
     def __init__(self, range_min: float, range_max: float) -> None:
         """Allows this mob to jump higher when being ridden by a player."""
@@ -737,85 +779,14 @@
 
     def __init__(self, value: int) -> None:
         """Defines how much friction affects this entity."""
         super().__init__("friction_modifier")
         self._component_add_field("value", value)
 
 
-class Breathable(_component):
-    component_namespace = "minecraft:breathable"
-
-    def __init__(
-        self,
-        breathes_air: bool = True,
-        breathes_water: bool = False,
-        total_supply: int = 15,
-        suffocate_time: int = -20,
-        inhale_time: int = 0,
-        generates_bubbles: bool = True,
-    ) -> None:
-        """Defines what blocks this entity can breathe in and gives them the ability to suffocate."""
-        super().__init__("breathable")
-        if not breathes_air:
-            self._component_add_field("breathes_air", breathes_air)
-        if breathes_water:
-            self._component_add_field("breathes_water", breathes_water)
-        if total_supply != 15:
-            self._component_add_field("total_supply", total_supply)
-        if suffocate_time != -20:
-            self._component_add_field("suffocate_time", suffocate_time)
-        if inhale_time != 0:
-            self._component_add_field("inhale_time", inhale_time)
-        if not generates_bubbles:
-            self._component_add_field("generates_bubbles", generates_bubbles)
-
-    @property
-    def breathes_lava(self):
-        self._component_add_field("breathes_lava", True)
-        return self
-
-    @property
-    def breathes_solids(self):
-        self._component_add_field("breathes_solids", True)
-        return self
-
-    @property
-    def breathes_solids(self):
-        self._component_add_field("breathes_solids", True)
-        return self
-
-    def breathe_blocks(self, *blocks: Blocks._MinecraftBlock | str):
-        self._component_add_field(
-            "blocks",
-            [
-                (
-                    block.identifier
-                    if isinstance(block, Blocks._MinecraftBlock)
-                    else block if isinstance(block, str) else CONFIG.Logger.unsupported_block_type(block)
-                )
-                for block in blocks
-            ],
-        )
-        return self
-
-    def non_breathe_blocks(self, *blocks: Blocks._MinecraftBlock | str):
-        self._component_add_field(
-            "non_breathe_blocks",
-            [
-                (
-                    block.identifier
-                    if isinstance(block, Blocks._MinecraftBlock)
-                    else block if isinstance(block, str) else CONFIG.Logger.unsupported_block_type(block)
-                )
-                for block in blocks
-            ],
-        )
-        return self
-
-
 class Variant(_component):
     component_namespace = "minecraft:variant"
 
     def __init__(self, value: int) -> None:
         """Used to differentiate the component group of a variant of an entity from others. (e.g. ocelot, villager)."""
         super().__init__("variant")
         self._component_add_field("value", value)
@@ -2518,15 +2489,15 @@
 
 class Loot(_component):
     component_namespace = "minecraft:loot"
 
     def __init__(self, path) -> None:
         """Sets the loot table for what items this entity drops upon death."""
         super().__init__("loot")
-        self._component_add_field("table", os.path.join("loot_tables", path + ".loot_table.json"))
+        self._component_add_field("table", path)
 
 
 class Float(_ai_goal):
     component_namespace = "minecraft:behavior.float"
 
     def __init__(self, sink_with_passengers: bool = False) -> None:
         """Allows an entity to float on water. Passengers will be kicked out the moment the mob's head goes underwater, which may not happen for tall mobs."""
@@ -2884,27 +2855,14 @@
                 "summon_cap_radius": summon_cap_radius if summon_cap_radius != 0 else {},
                 "target": target,
             }
         )
         return self
 
 
-class Boss(_component):
-    component_namespace = "minecraft:boss"
-
-    def __init__(self, name: str, hud_range: int = 55, should_darken_sky: bool = False) -> None:
-        """Defines the current state of the boss for updating the boss HUD."""
-        super().__init__("boss")
-        self._component_add_field("name", name)
-        if hud_range != 55:
-            self._component_add_field("power", hud_range)
-        if should_darken_sky:
-            self._component_add_field("should_darken_sky", should_darken_sky)
-
-
 class DelayedAttack(_ai_goal):
     component_namespace = "minecraft:behavior.delayed_attack"
 
     def __init__(
         self,
         attack_duration: float = 0.75,
         attack_once: bool = False,
@@ -3207,15 +3165,15 @@
 
 class Equipment(_component):
     component_namespace = "minecraft:equipment"
 
     def __init__(self, path) -> None:
         """Sets the loot table for what items this entity drops upon death."""
         super().__init__("equipment")
-        self._component_add_field("table", os.path.join("loot_tables", path))
+        self._component_add_field("table", path)
 
 
 class _EquipItem(_component):
     component_namespace = "minecraft:equip_item"
 
     def __init__(self) -> None:
         """Compels the entity to equip desired equipment."""
@@ -3325,15 +3283,15 @@
         event: str,
         event_filters: Filter,
         maximum_count: int = -1,
         minimum_count: int = -1,
         require_all: bool = False,
         range: tuple[float, float] = [10, 10],
         cooldown: int = -1,
-    ) -> None:
+    ):
         """A component that initiates an event when a set of conditions are met by other entities within the defined range.
 
         Args:
             event (str): Event to initiate when the conditions are met.
             event_filter (Filter): The set of conditions that must be satisfied to initiate the event.
             maximum_count (int, optional): The maximum number of entities that must pass the filter conditions for the event to send. Defaults to -1.
             minimum_count (int, optional): The minimum number of entities that must pass the filter conditions for the event to send. Defaults to -1.
@@ -3350,15 +3308,15 @@
         if maximum_count != -1:
             sensor["maximum_count"] = maximum_count
         if minimum_count != -1:
             sensor["minimum_count"] = minimum_count
         if require_all:
             sensor["require_all"] = require_all
         if range != (10, 10):
-            sensor["range"] = range
+            sensor["range"] = range if type(range) is list else [range, range]
         if cooldown != -1:
             sensor["cooldown"] = cooldown
 
         self[self.component_namespace]["subsensors"].append(sensor)
 
         return self
 
@@ -4130,15 +4088,15 @@
         """
         super().__init__("behavior.owner_hurt_by_target")
 
         if entity_types != None:
             self._component_add_field("entity_types", {"filters": entity_types})
         if cooldown != 0:
             self._component_add_field("cooldown", cooldown)
-        if not filters != None:
+        if filters != None:
             self._component_add_field("filters", filters)
         if max_dist != 16:
             self._component_add_field("max_dist", max_dist)
         if must_see:
             self._component_add_field("must_see", must_see)
         if must_see_forget_duration != 3.0:
             self._component_add_field("must_see_forget_duration", must_see_forget_duration)
@@ -4182,15 +4140,15 @@
         """
         super().__init__("behavior.owner_hurt_target")
 
         if entity_types != None:
             self._component_add_field("entity_types", {"filters": entity_types})
         if cooldown != 0:
             self._component_add_field("cooldown", cooldown)
-        if not filters != None:
+        if filters != None:
             self._component_add_field("filters", filters)
         if max_dist != 16:
             self._component_add_field("max_dist", max_dist)
         if must_see:
             self._component_add_field("must_see", must_see)
         if must_see_forget_duration != 3.0:
             self._component_add_field("must_see_forget_duration", must_see_forget_duration)
@@ -4417,23 +4375,14 @@
             self._component_add_field("search_range", search_range)
         if speed_multiplier != 1.0:
             self._component_add_field("speed_multiplier", speed_multiplier)
         if stop_distance != 2:
             self._component_add_field("stop_distance", stop_distance)
 
 
-# Unfinished
-class ConditionalBandwidthOptimization(_component):
-    component_namespace = "minecraft:conditional_bandwidth_optimization"
-
-    def __init__(self) -> None:
-        """Defines the Conditional Spatial Update Bandwidth Optimizations of this entity."""
-        super().__init__("conditional_bandwidth_optimization")
-
-
 class RandomSwim(_ai_goal):
     component_namespace = "minecraft:behavior.random_swim"
 
     def __init__(
         self,
         avoid_surface: bool = True,
         interval: int = 120,
@@ -4569,47 +4518,50 @@
     def add_interaction(
         self,
         event: str,
         filter: Filter = None,
         add_items: str = None,
         cooldown: float = 0.0,
         cooldown_after_being_attacked: float = 0.0,
-        drop_item_slot: int = -1,
-        equip_item_slot: int = -1,
+        drop_item_slot: int | Slots = -1,
+        equip_item_slot: int | Slots = -1,
         health_amount: int = 0,
         hurt_item: int = 0,
         interact_text: str = None,
         play_sounds: str = None,
         spawn_entities: Identifier = None,
         spawn_items: str = None,
         swing: bool = False,
         transform_to_item: str = None,
         use_item: bool = False,
         vibration: Vibrations = Vibrations.EntityInteract,
+        repair_entity_item: tuple[Slots, int] = None,
         # entity_act: str = None,
     ):
         """Adds an interaction to the entity.
 
         Args:
             event (str): Event to trigger when the interaction occurs.
             filter (Filter, optional): Filter to determine which entities can interact with this entity. Defaults to None.
             add_items (str, optional): File path, relative to the Behavior Pack's path, to the loot table file. Defaults to None.
             cooldown (float, optional): Time in seconds before this entity can be interacted with again. Defaults to 0.0.
             cooldown_after_being_attacked (float, optional): Time in seconds before this entity can be interacted with after being attacked. Defaults to 0.0.
-            equip_item_slot (int, optional): The entity's equipment slot to equip the item to, if any, upon successful interaction. Defaults to -1.
+            drop_item_slot (int | Slots, optional): Slot from which the item will be dropped when interacting with this entity. Defaults to -1.
+            equip_item_slot (int | Slots, optional): Slot from which the item will be equipped when interacting with this entity. Defaults to -1.
             health_amount (int, optional): The amount of health this entity will recover or hurt when interacting with this item. Negative values will harm the entity. Defaults to 0.
             hurt_item (int, optional): The amount of damage the item will take when used to interact with this entity. A value of 0 means the item won't lose durability. Defaults to 0.
             interact_text (str, optional): Text to show while playing with touch-screen controls when the player is able to interact in this way with this entity. Defaults to None.
             play_sounds (str, optional): One or more sound identifiers to play when the interaction occurs. Defaults to None.
             spawn_entities (str, optional): Entity to spawn when the interaction occurs. Defaults to None.
             spawn_items (str, optional): Loot table with items to drop on the ground upon successful interaction. Defaults to None.
             swing (bool, optional): If true, the player will do the 'swing' animation when interacting with this entity. Defaults to False.
             transform_to_item (str, optional): The item used will transform to this item upon successful interaction. Format: itemName:auxValue. Defaults to None.
             use_item (bool, optional): If true, the interaction will use an item. Defaults to False.
             vibration (str, optional): Vibration to emit when the interaction occurs. Admitted values are entity_interact (used by default), shear, and none (no vibration emitted). Defaults to None.
+            repair_entity_item (tuple[Slots, int], optional): Slot and amount to repair the item used to interact with this entity. Defaults to None.
 
         [Documentation reference]: https://learn.microsoft.com/en-gb/minecraft/creator/reference/content/entityreference/examples/entitycomponents/minecraftcomponent_interact?view=minecraft-bedrock-stable#parameter
         """
 
         interaction = {
             "on_interact": {
                 "filters": filter if not filter is None else {},
@@ -4642,14 +4594,19 @@
             interaction["swing"] = swing
         if not transform_to_item is None:
             interaction["transform_to_item"] = transform_to_item
         if use_item:
             interaction["use_item"] = use_item
         if not vibration is Vibrations.EntityInteract:
             interaction["vibration"] = vibration.value
+        if not repair_entity_item is None:
+            interaction["repair_entity_item"] = {
+                "slot": repair_entity_item[0],
+                "repair_amount": repair_entity_item[1],
+            }
 
         self[self.component_namespace]["interactions"].append(interaction)
         return self
 
     def particle_on_start(
         self,
         particle_type: str,
@@ -5055,15 +5012,15 @@
         super().__init__("tameable")
 
         if probability != 1.0:
             self._component_add_field("probability", probability)
         if not tame_event is None:
             self._component_add_field("tame_event", {"event": tame_event, "target": tame_subject})
         if len(tame_items) > 0:
-            self._component_add_field("tame_items", *tame_items)
+            self._component_add_field("tame_items", [str(i) for i in tame_items])
 
 
 class RunAroundLikeCrazy(_ai_goal):
     component_namespace = "minecraft:behavior.run_around_like_crazy"
 
     def __init__(
         self,
@@ -5105,39 +5062,560 @@
 
 class Ageable(_component):
     component_namespace = "minecraft:ageable"
 
     def __init__(
         self,
         duration: Seconds = 1200.0,
-        drop_items: list[str] = [],
-        feed_items: list[dict[str, Union[str, int]] | str] = [],
-        grow_up: str = None,
+        grow_up_event: str = None,
+        grow_up_target: FilterSubject = FilterSubject.Self,
         interact_filters: Filter = None,
         transform_to_item: str = None,
     ) -> None:
         """Adds a timer for the entity to grow up. The timer can be accelerated by giving the entity items it likes as defined by feed_items.
 
         Args:
             duration (Seconds, optional): Amount of time before the entity grows up, -1 for always a baby. Defaults to 1200.0.
-            drop_items (list[str], optional): List of items the entity drops when it grows up. Defaults to [].
-            feed_items (list[dict[str, Union[str, int]], optional): List of items that can be fed to the entity. Includes 'item' for the item name and 'growth' to define how much time growth is accelerated. Defaults to [].
-            grow_up (str, optional): Event to run when the entity grows up. Defaults to None.
+            grow_up_event (str, optional): Event to initiate when the entity grows up. Defaults to None.
             interact_filters (Filter, optional): A list of conditions to meet for the entity to be fed. Defaults to None.
             transform_to_item (str, optional): The feed item used will transform into this item upon successful interaction. Format: itemName:auxValue. Defaults to None.
 
         [Documentation reference]: https://learn.microsoft.com/en-gb/minecraft/creator/reference/content/entityreference/examples/entitycomponents/minecraftcomponent_ageable
         """
         super().__init__("ageable")
+        self[self.component_namespace]["feed_items"] = []
 
         if duration != 1200.0:
             self._component_add_field("duration", duration)
-        if not drop_items == []:
-            self._component_add_field("drop_items", drop_items)
-        if not feed_items == []:
-            self._component_add_field("feed_items", feed_items)
-        if not grow_up is None:
-            self._component_add_field("grow_up", grow_up)
+        if not grow_up_event is None:
+            self._component_add_field("grow_up", {"event": grow_up_event, "target": grow_up_target})
         if not interact_filters is None:
             self._component_add_field("interact_filters", interact_filters)
         if not transform_to_item is None:
             self._component_add_field("transform_to_item", transform_to_item)
+
+    def drop_item(self, *items: str):
+        """Adds an item to the list of items the entity drops when it grows up.
+
+        Args:
+            item (str): The item to add to the list of items the entity drops when it grows up.
+
+            Returns:
+                Ageable: Returns the Ageable component to allow for method chaining.
+        """
+        self._component_add_field("drop_items", items)
+        return self
+
+    def feed_items(self, *items: str):
+        """Adds an item to the list of items the entity can be fed.
+
+        Args:
+            item (str): The item to add to the list of items the entity can be fed.
+
+            Returns:
+                Ageable: Returns the Ageable component to allow for method chaining.
+        """
+        self[self.component_namespace]["feed_items"].extend([str(i) for i in items])
+        return self
+
+    def feed_item_growth(self, item: str, growth: float):
+        """Adds an item to the list of items the entity can be fed.
+
+        Args:
+            item (str): The item to add to the list of items the entity can be fed.
+            growth (float): The amount of growth to add to the entity when fed this item.
+
+            Returns:
+                Ageable: Returns the Ageable component to allow for method chaining.
+        """
+        self[self.component_namespace]["feed_items"].append({"item": str(item), "growth": clamp(growth, 0, 1)})
+        return self
+
+
+class Inventory(_component):
+    component_namespace = "minecraft:inventory"
+
+    def __init__(
+        self,
+        additional_slots_per_strength: int = 0,
+        can_be_siphoned_from: bool = False,
+        container_type: ContainerType = ContainerType.Inventory,
+        inventory_size: int = 5,
+        private: bool = False,
+        restrict_to_owner: bool = False,
+    ) -> None:
+        """Defines how an entity's inventory is managed.
+
+        Args:
+            additional_slots_per_strength (int, optional): Number of slots that this entity can gain per extra strength. Defaults to 0.
+            can_be_siphoned_from (bool, optional): If true, the contents of this inventory can be removed by a hopper. Defaults to False.
+            container_type (str, optional): Type of container the entity has. Can be horse, minecart_chest, chest_boat, minecart_hopper, inventory, container or hopper. Defaults to inventory.
+            inventory_size (int, optional): Number of slots the container has. Defaults to 5.
+            private (bool, optional): If true, the entity will not drop its inventory on death. Defaults to False.
+            restrict_to_owner (bool, optional): If true, the entity's inventory can only be accessed by its owner or itself. Defaults to False.
+
+        [Documentation reference]: https://learn.microsoft.com/en-gb/minecraft/creator/reference/content/entityreference/examples/entitycomponents/minecraftcomponent_inventory
+        """
+        super().__init__("inventory")
+
+        self._component_add_field("container_type", container_type)
+        if additional_slots_per_strength != 0:
+            self._component_add_field("additional_slots_per_strength", additional_slots_per_strength)
+        if can_be_siphoned_from:
+            self._component_add_field("can_be_siphoned_from", can_be_siphoned_from)
+        if inventory_size != 5:
+            self._component_add_field("inventory_size", inventory_size)
+        if private:
+            self._component_add_field("private", private)
+        if restrict_to_owner:
+            self._component_add_field("restrict_to_owner", restrict_to_owner)
+
+
+class Dash(_component):
+    component_namespace = "minecraft:dash"
+
+    def __init__(
+        self,
+        cooldown_time: Seconds = 1.0,
+        horizontal_momentum: float = 1.0,
+        vertical_momentum: float = 1.0,
+    ) -> None:
+        """Determines a rideable entity's ability to dash.
+
+        Args:
+            cooldown_time (Seconds, optional): The dash cooldown time, in seconds. Defaults to 1.0.
+            horizontal_momentum (float, optional): Horizontal momentum of the dash. Defaults to 1.0.
+            vertical_momentum (float, optional): Vertical momentum of the dash. Defaults to 1.0.
+
+        [Documentation reference]: https://learn.microsoft.com/en-gb/minecraft/creator/reference/content/entityreference/examples/entitycomponents/minecraftcomponent_dash
+        """
+        super().__init__("dash")
+
+        if cooldown_time != 1.0:
+            self._component_add_field("cooldown_time", cooldown_time)
+        if horizontal_momentum != 1.0:
+            self._component_add_field("horizontal_momentum", horizontal_momentum)
+        if vertical_momentum != 1.0:
+            self._component_add_field("vertical_momentum", vertical_momentum)
+
+
+class Breathable(_component):
+    component_namespace = "minecraft:breathable"
+
+    def __init__(
+        self,
+        breathes_air: bool = True,
+        breathes_lava: bool = True,
+        breathes_solids: bool = False,
+        breathes_water: bool = False,
+        generates_bubbles: bool = True,
+        inhale_time: Seconds = 0.0,
+        suffocate_time: int = -20,
+        total_supply: int = 15,
+        breathe_blocks: list[str] = [],
+        non_breathe_blocks: list[str] = [],
+    ) -> None:
+        """Defines which blocks an entity can breathe in and defines the ability to suffocate in those blocks.
+
+        Args:
+            breathe_blocks (list[str], optional): List of blocks the entity can breathe in. Defaults to [].
+            breathes_air (bool, optional): If true, the entity can breathe in air. Defaults to True.
+            breathes_lava (bool, optional): If true, the entity can breathe in lava. Defaults to True.
+            breathes_solids (bool, optional): If true, the entity can breathe in solid blocks. Defaults to False.
+            breathes_water (bool, optional): If true, the entity can breathe in water. Defaults to False.
+            generates_bubbles (bool, optional): If true, the entity will have visible bubbles while in water. Defaults to True.
+            inhale_time (Seconds, optional): Time in seconds to recover breath to maximum. Defaults to 0.0.
+            non_breathe_blocks (list[str], optional): List of blocks the entity can't breathe in, in addition to the other "breathes" parameters. Defaults to [].
+            suffocate_time (int, optional): Time in seconds between suffocation damage. Defaults to -20.
+            total_supply (int, optional): Time in seconds the entity can hold its breath. Defaults to 15.
+
+        [Documentation reference]: https://learn.microsoft.com/en-gb/minecraft/creator/reference/content/entityreference/examples/entitycomponents/minecraftcomponent_breathable
+        """
+        super().__init__("breathable")
+
+        if not breathes_air:
+            self._component_add_field("breathes_air", breathes_air)
+        if not breathes_lava:
+            self._component_add_field("breathes_lava", breathes_lava)
+        if breathes_solids:
+            self._component_add_field("breathes_solids", breathes_solids)
+        if breathes_water:
+            self._component_add_field("breathes_water", breathes_water)
+        if not generates_bubbles:
+            self._component_add_field("generates_bubbles", generates_bubbles)
+        if inhale_time != 0.0:
+            self._component_add_field("inhale_time", inhale_time)
+        if suffocate_time != -20:
+            self._component_add_field("suffocate_time", suffocate_time)
+        if total_supply != 15:
+            self._component_add_field("total_supply", total_supply)
+        if not breathe_blocks == []:
+            self._component_add_field("breathe_blocks", breathe_blocks)
+        if not non_breathe_blocks == []:
+            self._component_add_field("non_breathe_blocks", non_breathe_blocks)
+
+
+class VariableMaxAutoStep(_component):
+    component_namespace = "minecraft:variable_max_auto_step"
+
+    def __init__(
+        self,
+        base_value: float = 0.5625,
+        controlled_value: float = 0.5625,
+        jump_prevented_value: float = 0.5625,
+    ) -> None:
+        """Allows entities have a maximum auto step height that is different depending on whether they are on a block that prevents jumping.
+
+        Args:
+            base_value (float, optional): The maximum auto step height when on any other block. Defaults to 0.5625.
+            controlled_value (float, optional): The maximum auto step height when on any other block and controlled by the player. Defaults to 0.5625.
+            jump_prevented_value (float, optional): The maximum auto step height when on a block that prevents jumping. Defaults to 0.5625.
+
+        [Documentation reference]: https://learn.microsoft.com/en-gb/minecraft/creator/reference/content/entityreference/examples/entitycomponents/minecraftcomponent_variable_max_auto_step
+        """
+        super().__init__("variable_max_auto_step")
+
+        if base_value != 0.5625:
+            self._component_add_field("base_value", base_value)
+        if controlled_value != 0.5625:
+            self._component_add_field("controlled_value", controlled_value)
+        if jump_prevented_value != 0.5625:
+            self._component_add_field("jump_prevented_value", jump_prevented_value)
+
+
+class RiseToLiquidLevel(_ai_goal):
+    component_namespace = "minecraft:behavior.rise_to_liquid_level"
+
+    def __init__(
+        self,
+        liquid_y_offset: float = 0.0,
+        rise_delta: float = 0.0,
+        sink_delta: float = 0.0,
+    ) -> None:
+        """Compels an entity to rise to the top of a liquid block if they are located in one or have spawned under a liquid block.
+
+        Args:
+            liquid_y_offset (float, optional): Vertical offset from the liquid. Defaults to 0.0.
+            priority (int, optional): The higher the priority, the sooner this behavior will be executed as a goal. Defaults to 0.
+            rise_delta (float, optional): Displacement for how much the entity will move up in the vertical axis. Defaults to 0.0.
+            sink_delta (float, optional): Displacement for how much the entity will move down in the vertical axis. Defaults to 0.0.
+
+        [Documentation reference]: https://learn.microsoft.com/en-gb/minecraft/creator/reference/content/entityreference/examples/entitygoals/minecraftbehavior_rise_to_liquid_level
+        """
+        super().__init__("behavior.rise_to_liquid_level")
+
+        if liquid_y_offset != 0.0:
+            self._component_add_field("liquid_y_offset", liquid_y_offset)
+        if rise_delta != 0.0:
+            self._component_add_field("rise_delta", rise_delta)
+        if sink_delta != 0.0:
+            self._component_add_field("sink_delta", sink_delta)
+
+
+class Buoyant(_component):
+    component_namespace = "minecraft:buoyant"
+
+    def __init__(
+        self,
+        liquid_blocks: list[str],
+        apply_gravity: bool = True,
+        base_buoyancy: float = 1.0,
+        big_wave_probability: float = 0.03,
+        big_wave_speed: float = 10.0,
+        drag_down_on_buoyancy_removed: float = 0.0,
+        simulate_waves: bool = True,
+    ) -> None:
+        """Allows an entity to float on the specified liquid blocks.
+
+        Args:
+            liquid_blocks (list[str], optional): List of blocks this entity can float on. Must be a liquid block.
+            apply_gravity (bool, optional): Applies gravity each tick. Causes more of a wave simulation, but will cause more gravity to be applied outside liquids. Defaults to True.
+            base_buoyancy (float, optional): Base buoyancy used to calculate how much the entity will float. Defaults to 1.0.
+            big_wave_probability (float, optional): Probability of a big wave hitting the entity. Only used if simulate_waves is true. Defaults to 0.03.
+            big_wave_speed (float, optional): Multiplier for the speed to make a big wave. Triggered depending on big_wave_probability. Defaults to 10.0.
+            drag_down_on_buoyancy_removed (float, optional): How much an entity will be dragged down when the buoyancy component is removed. Defaults to 0.0.
+            simulate_waves (bool, optional): If true, the movement simulates waves going through. Defaults to True.
+
+        [Documentation reference]: https://learn.microsoft.com/en-gb/minecraft/creator/reference/content/entityreference/examples/entitycomponents/minecraftcomponent_buoyant
+        """
+        super().__init__("buoyant")
+
+        self._component_add_field("liquid_blocks", liquid_blocks)
+        if not apply_gravity:
+            self._component_add_field("apply_gravity", apply_gravity)
+        if base_buoyancy != 1.0:
+            self._component_add_field("base_buoyancy", clamp(base_buoyancy, 0, 1))
+        if big_wave_probability != 0.03:
+            self._component_add_field("big_wave_probability", big_wave_probability)
+        if big_wave_speed != 10.0:
+            self._component_add_field("big_wave_speed", big_wave_speed)
+        if drag_down_on_buoyancy_removed != 0.0:
+            self._component_add_field("drag_down_on_buoyancy_removed", drag_down_on_buoyancy_removed)
+        if not simulate_waves:
+            self._component_add_field("simulate_waves", simulate_waves)
+
+
+class LavaMovement(_component):
+    component_namespace = "minecraft:lava_movement"
+
+    def __init__(self, value: float) -> None:
+        """Defines the speed with which an entity can move through lava."""
+        super().__init__("lava_movement")
+        self._component_add_field("value", value)
+
+
+class ExperienceReward(_component):
+    component_namespace = "minecraft:experience_reward"
+
+    def __init__(
+        self,
+    ) -> None:
+        """Defines the amount of experience rewarded when the entity dies or is successfully bred.
+
+        [Documentation reference]: https://learn.microsoft.com/en-gb/minecraft/creator/reference/content/entityreference/examples/entitycomponents/minecraftcomponent_experience_reward
+        """
+        super().__init__("experience_reward")
+
+    def on_bred(self, on_bred: str | int | Molang):
+        self._component_add_field("on_bred", on_bred)
+        return self
+
+    def on_death(self, on_death: str | int | Molang):
+        self._component_add_field("on_death", on_death)
+        return self
+
+
+class Equippable(_component):
+    component_namespace = "minecraft:equippable"
+
+    def __init__(self) -> None:
+        """Defines an entity's behavior for having items equipped to it."""
+        super().__init__("equippable")
+        self[self.component_namespace]["slots"] = []
+
+    def slot(
+        self,
+        slot: int,
+        item: str,
+        accepted_items: list[str],
+        interact_text: str = None,
+        on_equip: str = None,
+        on_unequip: str = None,
+    ):
+        """Adds a slot to the entity's equippable slots.
+
+        Args:
+            slot (int): The slot number of this slot.
+            item (str): Identifier of the item that can be equipped for the slot.
+            accepted_items (list[str]): The list of items that can fill this slot.
+            interact_text (str, optional): Text to be displayed while playing with touch-screen controls when the entity can be equipped with this item. Defaults to None.
+            on_equip (str, optional): Event to trigger when the entity is equipped with the item. Defaults to None.
+            on_unequip (str, optional): Event to trigger when the item is removed from the entity. Defaults to None.
+
+        Returns:
+            Equippable: Returns the Equippable component to allow for method chaining.
+        """
+        slot_data = {
+            "slot": slot,
+            "item": item,
+            "accepted_items": accepted_items,
+        }
+        if not interact_text is None:
+            t = interact_text.lower().replace(" ", "_")
+            slot_data["interact_text"] = f"action.interact.{t}"
+            ANVIL.definitions.register_lang(f"action.interact.{t}", interact_text)
+        if not on_equip is None:
+            slot_data["on_equip"] = {"event": on_equip}
+        if not on_unequip is None:
+            slot_data["on_unequip"] = {"event": on_unequip}
+
+        self[self.component_namespace]["slots"].append(slot_data)
+        return self
+
+
+class Color(_component):
+    component_namespace = "minecraft:color"
+
+    def __init__(self, value: int) -> None:
+        """Defines the entity's main color.
+
+        Args:
+            value (int): The Palette Color value of the entity.
+
+        [Documentation reference]: https://learn.microsoft.com/en-gb/minecraft/creator/reference/content/entityreference/examples/entitycomponents/minecraftcomponent_color
+        """
+        super().__init__("color")
+        self._component_add_field("value", value)
+
+
+class Color2(_component):
+    component_namespace = "minecraft:color2"
+
+    def __init__(self, value: int) -> None:
+        """Defines the entity's second texture color.
+
+        Args:
+            value (int): The Palette Color value of the entity.
+
+        [Documentation reference]: https://learn.microsoft.com/en-gb/minecraft/creator/reference/content/entityreference/examples/entitycomponents/minecraftcomponent_color2
+        """
+        super().__init__("color2")
+        self._component_add_field("value", value)
+
+
+class BurnsInDaylight(_component):
+    component_namespace = "minecraft:burns_in_daylight"
+
+    def __init__(self) -> None:
+        """Compels an entity to burn when it's daylight.
+
+        [Documentation reference]: https://learn.microsoft.com/en-gb/minecraft/creator/reference/content/entityreference/examples/entitycomponents/minecraftcomponent_burns_in_daylight
+        """
+        super().__init__("burns_in_daylight")
+
+
+class Boss(_component):
+    component_namespace = "minecraft:boss"
+
+    def __init__(
+        self,
+        name: str,
+        hud_range: int = 55,
+        should_darken_sky: bool = False,
+    ) -> None:
+        """Defines the current state of the boss for updating the boss HUD.
+
+        Args:
+            name (str, optional): The name that displays above the boss's health bar.
+            hud_range (int, optional): The max distance from the boss at which the boss's health bar appears on the screen. Defaults to 55.
+            should_darken_sky (bool, optional): Whether the sky should darken in the presence of the boss. Defaults to False.
+
+        [Documentation reference]: https://learn.microsoft.com/en-gb/minecraft/creator/reference/content/entityreference/examples/entitycomponents/minecraftcomponent_boss
+        """
+        super().__init__("boss")
+
+        self._component_add_field("name", name)
+        if hud_range != 55:
+            self._component_add_field("hud_range", hud_range)
+        if should_darken_sky:
+            self._component_add_field("should_darken_sky", should_darken_sky)
+
+
+class Sittable(_component):
+    component_namespace = "minecraft:sittable"
+
+    def __init__(
+        self,
+        sit_event: str = None,
+        stand_event: str = None,
+    ) -> None:
+        """Defines the entity's 'sit' state.
+
+        Args:
+            sit_event (str, optional): Event to run when the entity enters the 'sit' state. Defaults to None.
+            stand_event (str, optional): Event to run when the entity exits the 'sit' state. Defaults to None.
+
+        [Documentation reference]: https://learn.microsoft.com/en-gb/minecraft/creator/reference/content/entityreference/examples/entitycomponents/minecraftcomponent_sittable
+        """
+        super().__init__("sittable")
+
+        if not sit_event is None:
+            self._component_add_field("sit_event", {"event": sit_event})
+        if not stand_event is None:
+            self._component_add_field("stand_event", {"event": stand_event})
+
+
+class FlyingSpeedMeters(_component):
+    component_namespace = "minecraft:flying_speed"
+
+    def __init__(self, value: float, max: float = None) -> None:
+        """A component that defines the entity's flying movement speed in meters per second.
+
+        Args:
+            value (float): Flying movement speed of the entity in meters per second.
+            max (float, optional): Maximum flying movement speed of the entity in meters per second. Defaults to None.
+
+        [Documentation reference]: https://learn.microsoft.com/en-gb/minecraft/creator/reference/content/entityreference/examples/entitycomponents/minecraftcomponent_flying_speed
+        """
+        super().__init__("flying_speed")
+        self._component_add_field("value", round(0.152 * math.sqrt(value), 2))
+        if not max is None:
+            self._component_add_field("max", round(0.152 * math.sqrt(max), 2))
+
+
+class ConditionalBandwidthOptimization(_component):
+    component_namespace = "minecraft:conditional_bandwidth_optimization"
+
+    def __init__(
+        self,
+        max_dropped_ticks: int = 0,
+        max_optimized_distance: int = 0,
+        use_motion_prediction_hints: bool = False,
+    ) -> None:
+        """Defines the Conditional Spatial Update Bandwidth Optimizations of the entity.
+
+        Args:
+            max_dropped_ticks (int): In relation to the optimization value, determines the maximum ticks spatial update packets can be not sent.
+            max_optimized_distance (int): The maximum distance considered during bandwidth optimizations. Any value below the max is interpolated to find optimization, and any value greater than or equal to the max results in max optimization.
+            use_motion_prediction_hints (bool): When set to true, smaller motion packets will be sent during drop packet intervals, resulting in the same amount of packets being sent as without optimizations but with less data being sent. This should be used to prevent visual oddities when entities are traveling quickly or teleporting.
+
+        [Documentation reference]: https://learn.microsoft.com/en-gb/minecraft/creator/reference/content/entityreference/examples/entitycomponents/minecraftcomponent_conditional_bandwidth_optimization
+        """
+        super().__init__("conditional_bandwidth_optimization")
+        a = {}
+        if max_dropped_ticks != 0:
+            a["max_dropped_ticks"] = max_dropped_ticks
+        if max_optimized_distance != 0:
+            a["max_optimized_distance"] = max_optimized_distance
+        if use_motion_prediction_hints:
+            a["use_motion_prediction_hints"] = use_motion_prediction_hints
+
+        self._component_add_field(
+            "default_values",
+            a,
+        )
+
+    def conditional_values(
+        self,
+        max_dropped_ticks: int = 0,
+        max_optimized_distance: int = 0,
+        use_motion_prediction_hints: bool = False,
+    ):
+        a = {}
+        if max_dropped_ticks != 0:
+            a["max_dropped_ticks"] = max_dropped_ticks
+        if max_optimized_distance != 0:
+            a["max_optimized_distance"] = max_optimized_distance
+        if use_motion_prediction_hints:
+            a["use_motion_prediction_hints"] = use_motion_prediction_hints
+
+        self._component_add_field(
+            "conditional_values",
+            a,
+        )
+        return self
+
+
+class ItemHopper(_component):
+    component_namespace = "minecraft:item_hopper"
+
+    def __init__(
+        self,
+    ) -> None:
+        """Allows an entity to function like a hopper block.
+
+        [Documentation reference]: https://learn.microsoft.com/en-gb/minecraft/creator/reference/content/entityreference/examples/entitycomponents/minecraftcomponent_item_hopper
+        """
+        super().__init__("item_hopper")
+
+
+class BodyRotationBlocked(_component):
+    component_namespace = "minecraft:body_rotation_blocked"
+
+    def __init__(
+        self,
+    ) -> None:
+        """When set, the entity will no longer visually rotate their body to match their facing direction.
+
+        [Documentation reference]: https://learn.microsoft.com/en-gb/minecraft/creator/reference/content/entityreference/examples/entitycomponents/minecraftcomponent_body_rotation_blocked
+        """
+        super().__init__("body_rotation_blocked")
```

### Comparing `mcanvil-0.7.2/src/anvil/api/enums.py` & `mcanvil-0.7.3/src/anvil/api/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json
 from enum import StrEnum
 
-from anvil import ANVIL
 from anvil.api.types import Identifier, coordinate, coordinates
 from anvil.lib.lib import clamp, normalize_180
 
 
 class Target(StrEnum):
     """
     Enumeration for the types of targets that can be selected in Minecraft.
@@ -159,14 +158,15 @@
     Enumeration for the different levels of game difficulty.
     """
 
     Peaceful = "peaceful"
     Easy = "easy"
     Normal = "normal"
     Hard = "hard"
+    Hardcore = "hardcore"
 
 
 class DamageCause(StrEnum):
     """
     Enumeration for the different causes of damage in the game.
     """
 
@@ -223,14 +223,15 @@
     Absorption = "absorption"
     Invisibility = "invisibility"
     SlowFalling = "slow_falling"
     Nausea = "nausea"
     NightVision = "night_vision"
     WaterBreathing = "water_breathing"
     ConduitPower = "conduit_power"
+    Resistance = "resistance"
 
 
 class ScoreboardOperation(StrEnum):
     """
     Enumeration for the different operations that can be performed on a scoreboard.
     """
 
@@ -542,14 +543,15 @@
         """Selects targets that have the specified property.
 
         Args:
             property (str): The property to check for.
             value (str): The value of the property.
 
         """
+        from anvil import ANVIL
         property_values = {}
         for property, value in properties.items():
             property_values.update({f"{ANVIL.config.NAMESPACE}:{property}": value})
         self._args(has_property=property_values)
         return self
     
     def __str__(self) -> str:
@@ -737,27 +739,27 @@
     Opaque = "opaque"
     DoubleSided = "double_sided"
     Blend = "blend"
     AlphaTest = "alpha_test"
     AlphaTestSingleSided = "alpha_test_single_sided"
 
 
-class BlockCategory(StrEnum):
+class ItemCategory(StrEnum):
     """
-    Enumeration representing the categories of blocks that can be used in Minecraft.
+    Enumeration representing the categories of blocks and items that can be used in Minecraft.
     """
 
     Construction = "construction"
     Equipment = "equipment"
     Items = "items"
     Nature = "nature"
     none = "none"
 
 
-class BlockGroups(StrEnum):
+class ItemGroups(StrEnum):
     Anvil = "itemGroup.name.anvil"
     Arrow = "itemGroup.name.arrow"
     Axe = "itemGroup.name.axe"
     Banner = "itemGroup.name.banner"
     BannerPattern = "itemGroup.name.banner_pattern"
     Bed = "itemGroup.name.bed"
     Boat = "itemGroup.name.boat"
@@ -1135,7 +1137,46 @@
 
 class SmeltingTags(StrEnum):
     FURNACE = "furnace"
     BLAST_FURNACE = "blast_furnace"
     SMOKER = "smoker"
     CAMPFIRE = "campfire"
     SOUL_CAMPFIRE = "soul_campfire"
+
+
+class ContainerType(StrEnum):
+    Horse = "horse"
+    MinecartChest = "minecart_chest"
+    ChestBoat = "chest_boat"
+    MinecartHopper = "minecart_hopper"
+    Inventory = "inventory"
+    Container = "container"
+    Hopper = "hopper"
+
+
+class EnchantsSlots(StrEnum):
+    ArmorHead = "armor_head"
+    ArmorTorse = "armor_torso"
+    ArmorLegs = "armor_legs"
+    ArmorFeet = "armor_feet"
+
+
+class HudElement(StrEnum):
+    Hunger = "hunger"
+    All = "all"
+    Paperdoll = "paperdoll"
+    Armor = "armor"
+    Tooltips = "tooltips"
+    TouchControls = "touch_controls"
+    Crosshair = "crosshair"
+    Hotbar = "hotbar"
+    Health = "health"
+    ProgressBar = "progress_bar"
+    AirBubbles = "air_bubbles"
+    HorseHealth = "horse_health"
+    StatusEffects = "status_effects"
+    ItemText = "item_text"
+
+
+class HudVisibility(StrEnum):
+    Hide = "hide"
+    Reset = "reset"
```

### Comparing `mcanvil-0.7.2/src/anvil/api/features.py` & `mcanvil-0.7.3/src/anvil/api/features.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+import json
 import os
 from enum import StrEnum
 
+from PIL import Image, ImageDraw, ImageFont
+
 from anvil import CONFIG
 from anvil.api.enums import (CameraPresets, FogCameraLocation, LootPoolType,
                              RawTextConstructor, RenderDistanceType,
                              SmeltingTags)
 from anvil.api.types import Identifier
 from anvil.lib.lib import CopyFiles, File, FileExists, clamp
 from anvil.lib.reports import ReportType
 from anvil.lib.schemas import AddonObject, JsonSchemes, MinecraftDescription
-from PIL import Image, ImageDraw, ImageFont
 
 
 # Dialogue ------------------------------------------------
 class _DialogueButton:
     """Handles dialogue buttons.
 
     Attributes:
@@ -495,16 +497,16 @@
 class SmeltingRecipe(AddonObject):
     _extension = ".recipe.json"
     _path = os.path.join(CONFIG.BP_PATH, "recipes")
 
     def __init__(self, name: str, *tags: SmeltingTags):
         self._name = name
         self._tags = tags
-        self.content(JsonSchemes.smelting_recipe(CONFIG.NAMESPACE, name, tags))
         super().__init__(name)
+        self.content(JsonSchemes.smelting_recipe(CONFIG.NAMESPACE, name, tags))
 
     def input(self, identifier: Identifier):
         self._content["minecraft:recipe_furnace"]["input"] = {"item": identifier}
         return self
 
     def output(self, identifier: Identifier):
         self._content["minecraft:recipe_furnace"]["output"] = identifier
@@ -548,26 +550,36 @@
 
 
 class ShapelessRecipe(AddonObject):
     _extension = ".recipe.json"
     _path = os.path.join(CONFIG.BP_PATH, "recipes")
 
     def __init__(self, name: str):
-        self._name = name
-        self.content(JsonSchemes.shapeless_crafting_recipe(CONFIG.NAMESPACE, name, ["crafting_table"]))
         super().__init__(name)
+        self.content(JsonSchemes.shapeless_crafting_recipe(CONFIG.NAMESPACE, name, ["crafting_table"]))
 
     def ingredients(self, items: list[tuple[Identifier, int]]):
         if len(items) > 9:
             CONFIG.Logger.recipe_max_items(self._name)
-        self._content["minecraft:recipe_shapeless"]["ingredients"] = [{"item": item[0], "data": item[1] if len(item) > 1 else {}} for item in items]
+
+        for i, item in enumerate(items):
+            if not item is None:
+                if not isinstance(item, tuple):
+                    data = {"item": str(item)}
+                else:
+                    data = {"item": str(item[0]), "data": item[1]}
+                self._content["minecraft:recipe_shapeless"]["ingredients"].append(data)
         return self
 
     def result(self, identifier: Identifier, count: int = 1, data: int = 0):
-        self._content["minecraft:recipe_shapeless"]["result"] = {"item": identifier, "count": count, "data": data if data != 0 else {}}
+        self._content["minecraft:recipe_shapeless"]["result"] = {
+            "item": identifier,
+            "count": count,
+            "data": data if data != 0 else {},
+        }
         return self
 
     def priority(self, priority: int):
         self._content["minecraft:recipe_shapeless"]["priority"] = priority
         return self
 
     def queue(self):
@@ -586,19 +598,19 @@
         return super().queue()
 
 
 class ShapedCraftingRecipe(AddonObject):
     _extension = ".recipe.json"
     _path = os.path.join(CONFIG.BP_PATH, "recipes")
 
-    def __init__(self, name: str):
+    def __init__(self, name: str, assume_symmetry: bool = True):
         self._name = name
         self._recipe_exactly = False
         super().__init__(name)
-        self.content(JsonSchemes.shaped_crafting_recipe(CONFIG.NAMESPACE, name, ["crafting_table"]))
+        self.content(JsonSchemes.shaped_crafting_recipe(CONFIG.NAMESPACE, name, assume_symmetry, ["crafting_table"]))
 
     def ingredients(self, items: list[list[tuple[str, int]]], keep_empty_slots: bool = False) -> None:
         max_items = 9
         if len(items) > max_items:
             CONFIG.Logger.recipe_max_items(self._name)
 
         keys = "abcdefghijklmnopqrstuvwxyz"
@@ -633,15 +645,19 @@
             while all(row[-1] == " " for row in pattern):
                 pattern = [row[:-1] for row in pattern]
 
         self._content["minecraft:recipe_shaped"]["pattern"] = pattern
         return self
 
     def result(self, identifier: Identifier, count: int = 1, data: int = 0):
-        self._content["minecraft:recipe_shaped"]["result"] = {"item": identifier, "count": count, "data": data if data != 0 else {}}
+        self._content["minecraft:recipe_shaped"]["result"] = {
+            "item": str(identifier),
+            "count": count,
+            "data": data if data != 0 else {},
+        }
         return self
 
     def priority(self, priority: int):
         self._content["minecraft:recipe_shaped"]["priority"] = priority
         return self
 
     def queue(self):
@@ -759,48 +775,56 @@
 class Particle(AddonObject):
     _extension = ".particle.json"
     _path = os.path.join(CONFIG.BP_PATH, "particles")
 
     def __init__(self, particle_name, use_vanilla_texture: bool = False):
         super().__init__(particle_name)
         self._name = particle_name
-        self._content = ""
         self._use_vanilla_texture = use_vanilla_texture
 
+        if not FileExists(os.path.join("assets", "particles", f"{self._name}.particle.json")):
+            CONFIG.Logger.file_exist_error(f"{self._name}.particle.json", os.path.join("assets", "particles"))
+
+        with open(os.path.join("assets", "particles", f"{self._name}.particle.json"), "r") as file:
+            self._content = json.loads(file.read())
+            if self._content["particle_effect"]["description"]["identifier"] != f"{CONFIG.NAMESPACE}:{self._name}":
+                CONFIG.Logger.namespace_not_valid(self._content["particle_effect"]["description"]["identifier"])
+
     def queue(self):
         CONFIG.Report.add_report(
             ReportType.PARTICLE,
             vanilla=False,
             col0=self._name.replace("_", " ").title(),
             col1=f"{CONFIG.NAMESPACE}:{self._name}",
         )
 
         return super().queue("particles")
 
     def _export(self):
-        if self._content != "":
-            super()._export()
         if not self._use_vanilla_texture:
-            if FileExists(os.path.join("assets", "particles", f"{self._name}.png")):
-                CopyFiles(
-                    os.path.join("assets", "particles"),
-                    os.path.join(CONFIG.RP_PATH, "textures", CONFIG.NAMESPACE, CONFIG.PROJECT_NAME, "particle"),
-                    f"{self._name}.png",
-                )
-            else:
-                CONFIG.Logger.file_exist_error(f"{self._name}.png", os.path.join("assets", "particles"))
+            texture_path = self._content["particle_effect"]["description"]["basic_render_parameters"]["texture"]
+            texture_name = texture_path.split("/")[-1]
+            self._content["particle_effect"]["description"]["basic_render_parameters"]["texture"] = os.path.join(
+                CONFIG.RP_PATH, "textures", CONFIG.NAMESPACE, CONFIG.PROJECT_NAME, "particle", texture_name
+            )
+
+            if not FileExists(os.path.join("assets", "particles", f"{texture_name}.png")):
+                CONFIG.Logger.file_exist_error(f"{texture_name}.png", os.path.join("assets", "particles"))
 
-        if FileExists(os.path.join("assets", "particles", f"{self._name}.particle.json")):
             CopyFiles(
                 os.path.join("assets", "particles"),
-                os.path.join(CONFIG.RP_PATH, "particles"),
-                f"{self._name}.particle.json",
+                os.path.join(CONFIG.RP_PATH, "textures", CONFIG.NAMESPACE, CONFIG.PROJECT_NAME, "particle"),
+                f"{texture_name}.png",
             )
-        else:
-            CONFIG.Logger.file_exist_error(f"{self._name}.particle.json", os.path.join("assets", "particles"))
+
+        CopyFiles(
+            os.path.join("assets", "particles"),
+            os.path.join(CONFIG.RP_PATH, "particles"),
+            f"{self._name}.particle.json",
+        )
 
 
 # Camera Presets ------------------------------------------
 class CameraPreset(AddonObject):
     """A class representing a CameraPreset."""
 
     _extension = ".camera.json"
@@ -861,14 +885,27 @@
 
         Args:
             value (bool): Whether the listener is enabled.
         """
         self._camera_preset["minecraft:camera_preset"]["listener"] = value
         return self
 
+    def extend_player_rendering(self, value: bool = True):
+        """Sets whether the player rendering is extended.
+
+        Args:
+            value (bool): Whether the player rendering is extended.
+        """
+        if self._inherit == CameraPresets.Free:
+            if value == False:
+                self._camera_preset["minecraft:camera_preset"]["extend_player_rendering"] = False
+        else:
+            CONFIG.Logger.extend_player_rendering_not_free(self._name)
+        return self
+    
     @property
     def queue(self):
         """Queues the camera preset to be exported."""
         self.content(self._camera_preset)
         return super().queue()
 
     def __str__(self) -> str:
```

### Comparing `mcanvil-0.7.2/src/anvil/api/items.py` & `mcanvil-0.7.3/src/anvil/api/items.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 
 from anvil import ANVIL, CONFIG
 from anvil.api.actors import Attachable, _Components
 from anvil.api.commands import Effects, Slots
 from anvil.api.components import _component
+from anvil.api.enums import EnchantsSlots, ItemCategory, ItemGroups
 from anvil.api.types import Identifier, Seconds, inf
 from anvil.lib.format_versions import ITEM_SERVER_VERSION
 from anvil.lib.lib import clamp
 from anvil.lib.reports import ReportType
 from anvil.lib.schemas import AddonObject, JsonSchemes, MinecraftDescription
 
 __all__ = [
@@ -73,27 +74,27 @@
             self._component_add_field("movement_modifier", movement_modifier)
 
 
 # Require ITEM_SERVER_VERSION >= 1.20.30
 class ItemEnchantable(_component):
     component_namespace = "minecraft:enchantable"
 
-    def __init__(self, type: str, value: int) -> None:
+    def __init__(self, slot: EnchantsSlots, value: int) -> None:
         """Determines what enchantments can be applied to the item. Not all enchantments will have an effect on all item components.
 
         Args:
             type (str): What enchantments can be applied (ex. Using bow would allow this item to be enchanted as if it were a bow).
             value (int): The value of the enchantment (minimum of 0).
 
         [Documentation reference]: https://learn.microsoft.com/en-gb/minecraft/creator/reference/content/itemreference/examples/itemcomponents/minecraft_enchantable
         """
         super().__init__("enchantable")
         self._enforce_version(ITEM_SERVER_VERSION, "1.20.30")
 
-        self._component_add_field("type", type)
+        self._component_add_field("slot", slot)
         self._component_add_field("value", clamp(value, 0, inf))
 
 
 class ItemFood(_component):
     component_namespace = "minecraft:food"
 
     def __init__(
@@ -110,40 +111,35 @@
         [Documentation reference]: https://learn.microsoft.com/en-gb/minecraft/creator/reference/content/itemreference/examples/itemcomponents/minecraft_food
         """
         super().__init__("food")
         self._enforce_version(ITEM_SERVER_VERSION, "1.20.30")
         self._require_components(ItemUseModifiers)
 
         self._component_add_field("effects", [])
-        if can_always_eat:
-            self._component_add_field("can_always_eat", True)
-
-        if nutrition > 0:
-            self._component_add_field("nutrition", max(1, nutrition))
-
-        if saturation_modifier > 0:
-            self._component_add_field("saturation_modifier", max(0, saturation_modifier))
-
-        if not using_converts_to is None:
+        self._component_add_field("can_always_eat", can_always_eat)
+        self._component_add_field("nutrition", max(0, nutrition))
+        self._component_add_field("saturation_modifier", max(0, saturation_modifier))
+        if using_converts_to:
             self._component_add_field("using_converts_to", using_converts_to)
 
     def effects(self, effect: Effects, chance: float, duration: Seconds, amplifier: int):
-        """Sets the effects of the food item.
+        """# DEPRECATED
+        Sets the effects of the food item.
 
         Args:
             effect (Effects): The effect to apply.
             chance (float): The chance of the effect being applied.
             duration (Seconds): The duration of the effect.
             amplifier (int): The amplifier of the effect.
         """
         self[self.component_namespace]["effects"].append(
             {
-                "name": effect.value,
+                "name": str(effect),
                 "chance": clamp(chance, 0, 1),
-                "duration": duration,
+                "duration": max(0, duration * 20),
                 "amplifier": clamp(amplifier, 0, 255),
             }
         )
         return self
 
 
 class ItemInteractButton(_component):
@@ -215,30 +211,30 @@
         self._component_set_value(value)
 
 
 # Require ITEM_SERVER_VERSION >= 1.20.20
 class ItemWearable(_component):
     component_namespace = "minecraft:wearable"
 
-    def __init__(self, slot: Slots, protection: int = 0, dispensable: bool = True) -> None:
+    def __init__(self, slot: Slots, protection: int = 0) -> None:
         """Sets the wearable item component.
 
         Args:
             slot (Slots): Determines where the item can be worn. If any non-hand slot is chosen, the max stack size is set to 1.
             protection (int, optional): How much protection the wearable has. Defaults to 0.
             dispensable (bool, optional): Whether or not the item can be dispensed from a dispenser. Defaults to True.
 
         [Documentation reference]: https://learn.microsoft.com/en-gb/minecraft/creator/reference/content/itemreference/examples/itemcomponents/minecraft_wearable
         """
         super().__init__("wearable")
-        self._enforce_version(ITEM_SERVER_VERSION, "1.20.20")
+        self._enforce_version(ITEM_SERVER_VERSION, "1.20.70")
 
         self._component_add_field("slot", slot)
         self._component_add_field("protection", protection)
-        self._component_add_field("dispensable", dispensable)
+        #self._component_add_field("dispensable", dispensable)
 
 
 class ItemHandEquipped(_component):
     component_namespace = "minecraft:hand_equipped"
 
     def __init__(self, value: bool) -> None:
         """Determines if an item is rendered like a tool while in-hand.
@@ -247,15 +243,15 @@
             value (bool): Determines if the item is rendered like a tool in-hand.
 
         [Documentation reference]: https://learn.microsoft.com/en-gb/minecraft/creator/reference/content/itemreference/examples/itemcomponents/minecraft_hand_equipped
         """
         super().__init__("hand_equipped")
         self._enforce_version(ITEM_SERVER_VERSION, "1.20.20")
 
-        self._component_set_value(value)
+        self._component_add_field("value", value)
 
 
 class ItemGlint(_component):
     component_namespace = "minecraft:glint"
 
     def __init__(self, value: bool) -> None:
         """Determines whether the item has the enchanted glint render effect on it.
@@ -435,15 +431,15 @@
 
     def add_items(self, repair_amount: int, *repair_items: str):
         """
         Args:
             repair_amount (int): How much durability is repaired.
             repair_items (str): List of repair item entries.
         """
-        self[self.component_namespace]["repair_items"].append({"items": repair_items, "repair_amount": repair_amount})
+        self[self.component_namespace]["repair_items"].append({"items": [str(i) for i in repair_items], "repair_amount": repair_amount})
         return self
 
 
 class ItemMaxStackSize(_component):
     component_namespace = "minecraft:max_stack_size"
 
     def __init__(self, stack_size: int) -> None:
@@ -459,28 +455,32 @@
 
         self._component_set_value(clamp(stack_size, 1, 64))
 
 
 class ItemBlockPlacer(_component):
     component_namespace = "minecraft:block_placer"
 
-    def __init__(self, block: str, *use_on: str) -> None:
+    def __init__(self, block: str) -> None:
         """Sets the item as a Planter item component for blocks. Planter items are items that can be planted into another block.
 
         Args:
             block (str): Set the placement block name for the planter item.
             use_on (str): List of block descriptors that contain blocks that this item can be used on. If left empty, all blocks will be allowed.
 
         [Documentation reference]: https://learn.microsoft.com/en-gb/minecraft/creator/reference/content/itemreference/examples/itemcomponents/minecraft_block_placer
         """
         super().__init__("block_placer")
         self._enforce_version(ITEM_SERVER_VERSION, "1.20.10")
 
         self._component_add_field("block", block)
-        self._component_add_field("use_on", use_on)
+
+    def use_on(self, *blocks: str):
+        """List of block descriptors that contain blocks that this item can be used on."""
+        self._component_add_field("use_on", blocks)
+        return self
 
 
 class ItemRecord(_component):
     component_namespace = "minecraft:record"
 
     def __init__(self, sound_event: str, duration: float, comparator_signal: int = 1) -> None:
         """Used by record items to play music.
@@ -706,34 +706,38 @@
             texture (str): The item texture name to be used.
 
         [Documentation reference]: https://learn.microsoft.com/en-gb/minecraft/creator/reference/content/itemreference/examples/itemcomponents/minecraft_icon
         """
         super().__init__("icon")
         self._enforce_version(ITEM_SERVER_VERSION, "1.19.80")
         ANVIL.definitions.register_item_textures(texture, "", texture)
-        self._component_add_field("texture", f"{CONFIG.NAMESPACE}:{texture}")
+        self[self.component_namespace]["textures"] = {
+            "default": f"{CONFIG.NAMESPACE}:{texture}",
+        }
 
 
 # Items
 class _ItemServerDescription(MinecraftDescription):
     def __init__(self, name, is_vanilla) -> None:
         super().__init__(name, is_vanilla)
         self._description["description"]["properties"] = {}
+        self._description["description"]["menu_category"] = {}
+        
 
-    def group(self, group: str):
-        self._description["description"]["group"] = group
+    def group(self, group: ItemGroups):
+        self._description["description"]["menu_category"]["group"] = str(group)
         return self
 
-    def category(self, category: str):
-        self._description["description"]["category"] = category
+    def category(self, category: ItemCategory):
+        self._description["description"]["menu_category"]["category"] = str(category)
         return self
 
     @property
     def is_hidden_in_commands(self):
-        self._description["description"]["is_hidden_in_commands"] = True
+        self._description["description"]["menu_category"]["is_hidden_in_commands"] = True
         return self
 
     @property
     def to_dict(self):
         return super().to_dict
```

### Comparing `mcanvil-0.7.2/src/anvil/api/molang.py` & `mcanvil-0.7.3/src/anvil/api/molang.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from anvil.api.commands import Scoreboard
 from deprecated import deprecated
 
 from anvil import CONFIG
 from anvil.api.enums import Slots
 from anvil.lib.lib import *
 
 
@@ -83,14 +82,17 @@
 
     def __abs__(self):
         return Math.abs(self)
 
     def __round__(self):
         return Math.round(self)
 
+    def _struct(self, *args):
+        return _molang(f"{self}.{'.'.join(args)}")
+
     def _query(self, qtype, query, *arguments):
         a = f"{qtype}.{query}"
         if len(arguments):
             args = ", ".join(
                 (
                     f"'{arg}'"
                     if isinstance(arg, (str, StrEnum)) and not isinstance(arg, _molang) and not arg.startswith(MOLANG_PREFIXES)
@@ -98,14 +100,54 @@
                 )
                 for arg in arguments
             )
             a += f"({args})"
         return _molang(a)
 
 
+class vec3:
+    def __init__(self, molang: _molang) -> None:
+        self.m = molang
+
+    @property
+    def x(self):
+        return self.m._struct("x")
+
+    @property
+    def y(self):
+        return self.m._struct("y")
+
+    @property
+    def z(self):
+        return self.m._struct("z")
+
+    def __str__(self) -> str:
+        return self.m
+
+
+class _TRS:
+    def __init__(self, molang: _molang) -> None:
+        self.m = molang
+
+    @property
+    def translation(self):
+        return vec3(self.m._struct("t"))
+
+    @property
+    def rotation(self):
+        return vec3(self.m._struct("r"))
+
+    @property
+    def scale(self):
+        return vec3(self.m._struct("s"))
+
+    def __str__(self) -> str:
+        return self.m
+
+
 class Query(_molang):
     handle = "q"
 
     @classmethod
     def AboveTopSolid(self, x: int, z: int):
         """Returns the height of the block immediately above the highest solid block at the input (x,z) position.
 
@@ -2651,29 +2693,29 @@
     @classmethod
     def BoneOrientationTrs(self, bone_name: str):
         """TRS stands for 'Translate/Rotate/Scale.' Takes the name of the bone as an argument. Returns the bone orientation matrix decomposed into the component translation/rotation/scale parts of the desired bone provided it exists in the queryable geometry of the entity, else this returns the identity matrix and throws a content error. The returned value is returned as a variable of type struct with members .t, .r, and .s, each with members .x, .y, and .z, and can be accessed as per this example: v.my_variable = q.bone_orientation_trs('rightarm'); return v.my_variable.r.x;
 
         Returns:
             Molang(_molang): A Molang Instance
         """
-        return self._query(self, self.handle, "bone_orientation_trs", bone_name)
+        return _TRS(self._query(self, self.handle, "bone_orientation_trs", bone_name))
 
     @classmethod
     def BoneOrientationMatrix(self, bone_name: str):
         """Takes the name of the bone as an argument. Returns the bone orientation (as a matrix) of the desired bone provided it exists in the queryable geometry of the entity, else this returns the identity matrix and throws a content error.
 
         Returns:
             Molang(_molang): A Molang Instance
         """
         return self._query(self, self.handle, "bone_orientation_matrix", bone_name)
 
     @classmethod
     def IsAttached(self):
         """### Client Only
-        
+
         Returns 1.0 if the entity is attached to another entity (such as being held or worn), else it will return 0.0.
 
         Returns:
             Molang(_molang): A Molang Instance
         """
         return self._query(self, self.handle, "is_attached")
 
@@ -2681,15 +2723,15 @@
     def HasPlayerRider(self):
         """Returns 1.0 if the entity has a player rider, else it returns 0.0.
 
         Returns:
             Molang(_molang): A Molang Instance
         """
         return self._query(self, self.handle, "has_player_rider")
-    
+
     @classmethod
     def Scoreboard(self, score):
         """### Server Only
         Returns the specified scoreboard value for this entity.
 
         Args:
             score (str): The name of the scoreboard to query.
@@ -2703,33 +2745,33 @@
     def RideBodyXRotation(self):
         """Returns the body pitch world-rotation of the ride an entity, else it returns 0.0.
 
         Returns:
             Molang(_molang): A Molang Instance
         """
         return self._query(self, self.handle, "ride_body_x_rotation")
-    
+
     @classmethod
     def RideBodyYRotation(self):
         """Returns the body pitch world-rotation of a valid rider at the provided index if called on an entity, else it returns 0.0.
 
         Returns:
             Molang(_molang): A Molang Instance
         """
         return self._query(self, self.handle, "ride_body_y_rotation")
-    
+
     @classmethod
     def RideHeadXRotation(self):
         """Returns the head x world-rotation of the ride of an entity, else it returns 0.0.
 
         Returns:
             Molang(_molang): A Molang Instance
         """
         return self._query(self, self.handle, "ride_head_x_rotation")
-    
+
     @classmethod
     def RideHeadYRotation(self, clamp: int = 0):
         """Takes one optional argument as a parameter. Returns the head y world-rotation of the ride of an entity, else it returns 0.0. First parameter only for horses, zombie horses, skeleton horses, donkeys and mules that clamps rotation in degrees.
 
         Returns:
             Molang(_molang): A Molang Instance
         """
@@ -2739,15 +2781,15 @@
     def RiderBodyXRotation(self):
         """Returns the body pitch world-rotation of a valid rider at the provided index if called on an entity, else it returns 0.0.
 
         Returns:
             Molang(_molang): A Molang Instance
         """
         return self._query(self, self.handle, "rider_body_x_rotation")
-    
+
     @classmethod
     def RiderBodyYRotation(self):
         """Returns the body yaw world-rotation of a valid rider at the provided index if called on an entity, else it returns 0.0.
 
         Returns:
             Molang(_molang): A Molang Instance
         """
@@ -2766,15 +2808,25 @@
     def RiderHeadYRotation(self, head: int = 0, clamp: int = 0):
         """Takes one or two arguments as parameters. Returns the head y world-rotation of the rider entity at the provided index, else it returns 0.0. Horses, zombie horses, skeleton horses, donkeys and mules require a second parameter that clamps rotation in degrees.
 
         Returns:
             Molang(_molang): A Molang Instance
         """
         return self._query(self, self.handle, "rider_head_y_rotation", head, clamp)
-    
+
+    @classmethod
+    def ArmorSlotDamage(self, slot: Slots, slot_id: int = 0):
+        """Returns the damage of the item in the specified armor slot name and slot id, else it returns 0.0.
+
+        Returns:
+            Molang(_molang): A Molang Instance
+        """
+        return self._query(self, self.handle, "armor_slot_damage", slot, slot_id)
+
+
 class Context(Query):
     handle = "c"
 
 
 class Variable(_molang):
     handle = "v"
```

### Comparing `mcanvil-0.7.2/src/anvil/api/texture_pack.py` & `mcanvil-0.7.3/src/anvil/api/texture_pack.py`

 * *Files identical despite different names*

### Comparing `mcanvil-0.7.2/src/anvil/api/types.py` & `mcanvil-0.7.3/src/anvil/api/types.py`

 * *Files identical despite different names*

### Comparing `mcanvil-0.7.2/src/anvil/api/ui.py` & `mcanvil-0.7.3/src/anvil/api/ui.py`

 * *Files identical despite different names*

### Comparing `mcanvil-0.7.2/src/anvil/api/vanilla.py` & `mcanvil-0.7.3/src/anvil/api/vanilla.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,182 @@
+import os
 from enum import Enum
 
+import commentjson as json
+import requests
+
 from anvil import ANVIL, CONFIG
 from anvil.api.enums import Dimension
+from anvil.lib.lib import File, FileExists
 
-ENTITY_LIST = []
+ENTITY_LIST: dict[str, "Entities.VanillaEntity"] = {}
 ITEMS_LIST = []
 BLOCK_LIST = []
 
+
+class Entities:
+    class VanillaEntity():
+        def __init__(self, name : str, is_mob: bool = True, is_vanilla: bool = True, allow_runtime: bool = True) -> None:
+            super().__init__()
+            ENTITY_LIST[name] = self
+            self.is_mob = is_mob
+            self.namespace = 'minecraft' if is_vanilla else CONFIG.NAMESPACE
+            self.name = name
+            self.allow_runtime = allow_runtime
+            self._github_name = name
+
+        def _set_github_name(self, name):
+            self._github_name = name
+
+        def get_vanilla_resource(self):
+            cache_path = os.path.join("assets", "cache", f"{self.name}.entity.json")
+            data = {}
+            if FileExists(cache_path):
+                with open(cache_path, "r") as file:
+                    data = json.loads(file.read())
+            else:
+                retrieve = requests.get(
+                    f"https://raw.githubusercontent.com/Mojang/bedrock-samples/main/resource_pack/entity/{self._github_name}.entity.json"
+                )
+                data = json.loads(retrieve.text)
+                File(f"{self.name}.entity.json", data, os.path.join("assets", "cache"), "w", True)
+                
+            return data
+
+        @property
+        def identifier(self):
+            return self.namespace + ':' + self.name
+        
+        def __str__(self) -> str:
+            return self.name
+        
+        def __eq__(self, __value: object) -> bool:
+            return __value == (self.namespace + ':' + self.name)
+
+        def __iter__(self):
+            yield self.name
+    
+    Agent = VanillaEntity("agent", False)
+    Allay = VanillaEntity("allay")
+    ArmorStand = VanillaEntity("armor_stand", False)._set_github_name("armor_stand.v1.0")
+    Arrow = VanillaEntity("arrow", False)
+    Axolotl = VanillaEntity("axolotl")
+    Bat = VanillaEntity("bat")
+    Bed = VanillaEntity("bed", False)
+    Bee = VanillaEntity("bee")
+    Blaze = VanillaEntity("blaze")._set_github_name("blaze.v1.0")
+    Boat = VanillaEntity("boat", False)
+    Camel = VanillaEntity("camel")
+    Cat = VanillaEntity("cat")
+    CaveSpider = VanillaEntity("cave_spider")._set_github_name("cave_spider.v1.0")
+    ChestBoat = VanillaEntity("chest_boat", False)
+    ChestMinecart = VanillaEntity("chest_minecart", False)._set_github_name("chest_minecart.v1.0")
+    Chicken = VanillaEntity("chicken")._set_github_name("chicken.v1.0")
+    Cod = VanillaEntity("cod")
+    CommandBlockMinecart = VanillaEntity("command_block_minecart", False)._set_github_name("command_block_minecart.v1.0")
+    Cow = VanillaEntity("cow")._set_github_name("cow.v1.0")
+    Creeper = VanillaEntity("creeper")._set_github_name("creeper.v1.0")
+    DecoratedPot = VanillaEntity("decorated_pot", False)
+    Dolphin = VanillaEntity("dolphin")
+    Donkey = VanillaEntity("donkey")._set_github_name("donkey_v3")
+    DragonFireball = VanillaEntity("dragon_fireball", False)
+    Drowned = VanillaEntity("drowned")._set_github_name("drowned.v1.0")
+    Egg = VanillaEntity("egg", False)
+    ElderGuardian = VanillaEntity("elder_guardian")
+    EnderCrystal = VanillaEntity("ender_crystal", False)
+    EnderDragon = VanillaEntity("ender_dragon")
+    EnderEye = VanillaEntity("ender_eye", False)
+    EnderPearl = VanillaEntity("ender_pearl", False)
+    Enderman = VanillaEntity("enderman")._set_github_name("enderman.v1.0")
+    Endermite = VanillaEntity("endermite")
+    EvocationFangs = VanillaEntity("evocation_fangs", False)
+    EvocationIllager = VanillaEntity("evocation_illager")._set_github_name("evocation_illager.v1.0")
+    ExperienceBottle = VanillaEntity("experience_bottle", False)
+    ExperienceOrb = VanillaEntity("experience_orb", False)
+    Fireball = VanillaEntity("fireball")
+    FireworkRocket = VanillaEntity("firework_rocket", False)
+    FishingHook = VanillaEntity("fishing_hook")
+    Fox = VanillaEntity("fox")
+    Frog = VanillaEntity("frog")
+    Ghast = VanillaEntity("ghast")
+    GlowSquid = VanillaEntity("glow_squid")
+    Goat = VanillaEntity("goat")
+    Guardian = VanillaEntity("guardian")
+    Hoglin = VanillaEntity("hoglin")
+    HopperMinecart = VanillaEntity("hopper_minecart", False)._set_github_name("hopper_minecart.v1.0")
+    Horse = VanillaEntity("horse")._set_github_name("horse_v3")
+    Husk = VanillaEntity("husk")._set_github_name("husk.v1.0")
+    IronGolem = VanillaEntity("iron_golem")
+    LeashKnot = VanillaEntity("leash_knot", False)
+    LingeringPotion = VanillaEntity("lingering_potion", False)
+    Llama = VanillaEntity("llama")._set_github_name("llama.v1.0")
+    LlamaSpit = VanillaEntity("llama_spit")
+    MagmaCube = VanillaEntity("magma_cube")
+    Minecart = VanillaEntity("minecart", False)._set_github_name("minecart.v1.0")
+    Mooshroom = VanillaEntity("mooshroom")._set_github_name("mooshroom.v1.0")
+    Mule = VanillaEntity("mule")._set_github_name("mule_v3")
+    Npc = VanillaEntity("npc")
+    Ocelot = VanillaEntity("ocelot")._set_github_name("ocelot.v1.0")
+    Panda = VanillaEntity("panda")
+    Parrot = VanillaEntity("parrot")
+    Phantom = VanillaEntity("phantom")
+    Pig = VanillaEntity("pig")._set_github_name("pig.v1.0")
+    Piglin = VanillaEntity("piglin")
+    PiglinBrute = VanillaEntity("piglin_brute")
+    Pillager = VanillaEntity("pillager")
+    Player = VanillaEntity("player")
+    PolarBear = VanillaEntity("polar_bear")
+    Pufferfish = VanillaEntity("pufferfish")._set_github_name("pufferfish.v1.0")
+    Rabbit = VanillaEntity("rabbit")._set_github_name("rabbit.v1.0")
+    Ravager = VanillaEntity("ravager")
+    Salmon = VanillaEntity("salmon")
+    Sheep = VanillaEntity("sheep")._set_github_name("sheep.v1.0")
+    Shulker = VanillaEntity("shulker")._set_github_name("shulker.v1.0")
+    ShulkerBullet = VanillaEntity("shulker_bullet")
+    Silverfish = VanillaEntity("silverfish")
+    Skeleton = VanillaEntity("skeleton")._set_github_name("skeleton.v1.0")
+    SkeletonHorse = VanillaEntity("skeleton_horse")._set_github_name("skeleton_horse_v3")
+    Skull = VanillaEntity("skull", False)
+    Slime = VanillaEntity("slime")
+    SmallFireball = VanillaEntity("small_fireball")
+    Sniffer = VanillaEntity("sniffer")
+    Snowball = VanillaEntity("snowball", False)
+    SnowGolem = VanillaEntity("snow_golem")._set_github_name("snow_golem.v1.0")
+    Spider = VanillaEntity("spider")._set_github_name("spider.v1.0")
+    SplashPotion = VanillaEntity("splash_potion", False)
+    Squid = VanillaEntity("squid")
+    Stray = VanillaEntity("stray")._set_github_name("stray.v1.0")
+    Strider = VanillaEntity("strider")
+    Tadpole = VanillaEntity("tadpole")
+    ThrownTrident = VanillaEntity("thrown_trident")
+    TntMinecart = VanillaEntity("tnt_minecart", False)._set_github_name("tnt_minecart.v1.0")
+    TraderLlama = VanillaEntity("trader_llama")
+    TripodCamera = VanillaEntity("tripod_camera", False)
+    Tropicalfish = VanillaEntity("tropicalfish")
+    Turtle = VanillaEntity("turtle")
+    Vex = VanillaEntity("vex")._set_github_name("vex.v1.0")
+    Villager = VanillaEntity("villager_v2")
+    Vindicator = VanillaEntity("vindicator")._set_github_name("vindicator.v1.0")
+    WanderingTrader = VanillaEntity("wandering_trader")
+    Warden = VanillaEntity("warden")
+    Witch = VanillaEntity("witch")._set_github_name("witch.v1.0")
+    Wither = VanillaEntity("wither")._set_github_name("wither.v1.0")
+    WitherSkeleton = VanillaEntity("wither_skeleton")._set_github_name("wither_skeleton.v1.0")
+    WitherSkull = VanillaEntity("wither_skull")
+    WitherSkullDangeroud = VanillaEntity("wither_skull_dangerous")
+    Wolf = VanillaEntity("wolf")
+    Zoglin = VanillaEntity("zoglin")
+    Zombie = VanillaEntity("zombie")._set_github_name("zombie.v1.0")
+    ZombieHorse = VanillaEntity("zombie_horse")._set_github_name("zombie_horse_v3")
+    ZombieVillager = VanillaEntity("zombie_villager_v2")
+
+    # Added in 1.20.80
+    Armadillo = VanillaEntity("armadillo")
+
+
 # Updated on 05-04-2023
 # Latest Updated release: 1.19.81.01
 class BlockStates:
     class ButtonPressedBit(Enum):
         ENUM0B = "0b"
         ENUM1B = "1b"
 
@@ -1500,134 +1666,16 @@
     ZoglinSpawnEgg = _basic_item('zoglin_spawn_egg')
     ZombieHorseSpawnEgg = _basic_item('zombie_horse_spawn_egg')
     ZombiePigmanSpawnEgg = _basic_item('zombie_pigman_spawn_egg')
     ZombieSpawnEgg = _basic_item('zombie_spawn_egg')
     ZombieVillagerSpawnEgg = _basic_item('zombie_villager_spawn_egg')
     Redstone = _basic_item('redstone')
 
-
-class Entities:
-    class vanilla_entity():
-        def __init__(self, name : str, is_vanilla: bool = True, allow_runtime: bool = True) -> None:
-            super().__init__()
-            ENTITY_LIST.append(self)
-            self._namespace = 'minecraft' if is_vanilla else CONFIG.NAMESPACE
-            self._name = name
-            self._allow_runtime = allow_runtime
-        
-        @property
-        def namespace(self):
-            return self._namespace
-        
-        @property
-        def identifier(self):
-            return self._namespace + ':' + self._name
-        
-        def __str__(self) -> str:
-            return self._name
-        
-        def __eq__(self, __value: object) -> bool:
-            return __value == (self._namespace + ':' + self._name)
-
-        def __iter__(self):
-            yield self._name
-
-    ArmorStand = vanilla_entity("armor_stand")
-    Arrow = vanilla_entity("arrow")
-    Axolotl = vanilla_entity("axolotl")
-    Bat = vanilla_entity("bat")
-    Bee = vanilla_entity("bee")
-    Blaze = vanilla_entity("blaze")
-    Cat = vanilla_entity("cat")
-    CaveSpider = vanilla_entity("cave_spider")
-    Chicken = vanilla_entity("chicken")
-    Cow = vanilla_entity("cow")
-    Creeper = vanilla_entity("creeper")
-    Dolphin = vanilla_entity("dolphin")
-    Donkey = vanilla_entity("donkey")
-    Drowned = vanilla_entity("drowned")
-    ElderGuardian = vanilla_entity("elder_guardian")
-    EnderDragon = vanilla_entity("ender_dragon")
-    Enderman = vanilla_entity("enderman")
-    Endermite = vanilla_entity("endermite")
-    EvocationIllager = vanilla_entity("evocation_illager")
-    Fish = vanilla_entity("fish")
-    FishingHook = vanilla_entity("fishing_hook")
-    Fireball = vanilla_entity("fireball")
-    Fox = vanilla_entity("fox")
-    Ghast = vanilla_entity("ghast")
-    GlowSquid = vanilla_entity("glow_squid")
-    Goat = vanilla_entity("goat")
-    Guardian = vanilla_entity("guardian")
-    Hoglin = vanilla_entity("hoglin")
-    Horse = vanilla_entity("horse")
-    Husk = vanilla_entity("husk")
-    IronGolem = vanilla_entity("iron_golem")
-    Llama = vanilla_entity("llama")
-    LlamaSpit = vanilla_entity("llama_spit")
-    MagmaCube = vanilla_entity("magma_cube")
-    Mooshroom = vanilla_entity("mooshroom")
-    Mule = vanilla_entity("mule")
-    Npc = vanilla_entity("npc")
-    Ocelot = vanilla_entity("ocelot")
-    Panda = vanilla_entity("panda")
-    Parrot = vanilla_entity("parrot")
-    Phantom = vanilla_entity("phantom")
-    Pig = vanilla_entity("pig")
-    PiglinBrute = vanilla_entity("piglin_brute")
-    Piglin = vanilla_entity("piglin")
-    Pillager = vanilla_entity("pillager")
-    Player = vanilla_entity("player")
-    PolarBear = vanilla_entity("polar_bear")
-    Pufferfish = vanilla_entity("pufferfish")
-    Rabbit = vanilla_entity("rabbit")
-    Ravager = vanilla_entity("ravager")
-    Salmon = vanilla_entity("salmon")
-    Sheep = vanilla_entity("sheep")
-    Shulker = vanilla_entity("shulker")
-    ShulkerBullet = vanilla_entity("shulker_bullet")
-    Silverfish = vanilla_entity("silverfish")
-    SkeletonHorse = vanilla_entity("skeleton_horse")
-    Skeleton = vanilla_entity("skeleton")
-    Slime = vanilla_entity("slime")
-    SnowGolem = vanilla_entity("snow_golem")
-    Spider = vanilla_entity("spider")
-    Squid = vanilla_entity("squid")
-    Stray = vanilla_entity("stray")
-    Strider = vanilla_entity("strider")
-    Tropicalfish = vanilla_entity("tropicalfish")
-    ThrownTrident = vanilla_entity("thrown_trident")
-    Turtle = vanilla_entity("turtle")
-    Vex = vanilla_entity("vex")
-    Villager = vanilla_entity("villager_v2")
-    Vindicator = vanilla_entity("vindicator")
-    WanderingTrader = vanilla_entity("wandering_trader")
-    Witch = vanilla_entity("witch")
-    WitherSkull = vanilla_entity("wither_skull")
-    WitherSkullDangeroud = vanilla_entity("wither_skull_dangerous")
-    WitherSkeleton = vanilla_entity("wither_skeleton")
-    Wither = vanilla_entity("wither")
-    Wolf = vanilla_entity("wolf")
-    Zoglin = vanilla_entity("zoglin")
-    ZombieHorse = vanilla_entity("zombie_horse")
-    ZombiePigman = vanilla_entity("zombie_pigman")
-    ZombieVillager = vanilla_entity("zombie_villager_v2")
-    Zombie = vanilla_entity("zombie")
-    Boat = vanilla_entity("boat")
-    Snowball = vanilla_entity("snowball")
-    LightningBolt = vanilla_entity('lightning_bolt')
-    # 1.19.0
-    # Updated on 11-07-2022
-    Warden = vanilla_entity("warden")
-    # 1.19.50.21
-    # Updated on 21-10-2022
-    Camel = vanilla_entity("camel")
-    # 1.19.70.23
-    # Updated on 28-02-2023
-    Sniffer = vanilla_entity("sniffer")
+    ArmadilloScute = _basic_item('armadillo_scute')
+    WolfArmor = _basic_item('wolf_armor')
 
 
 class Blocks:
     class _MinecraftBlock():
         def __init__(self, name: str, is_vanilla: bool = True):
             self._namespace = 'minecraft' if is_vanilla else ANVIL.NAMESPACE
             self._name = name
@@ -2530,26 +2578,14 @@
 
     class CoralBlock(_MinecraftBlock):
         def __init__(self, coral_color:'BlockStates.CoralColor'=None, dead_bit:'BlockStates.DeadBit'=None):
             self._coral_color = coral_color
             self._dead_bit = dead_bit
             super().__init__("coral_block", True)
 
-    class CoralFan(_MinecraftBlock):
-        def __init__(self, coral_color:'BlockStates.CoralColor'=None, coral_fan_direction:'BlockStates.CoralFanDirection'=None):
-            self._coral_color = coral_color
-            self._coral_fan_direction = coral_fan_direction
-            super().__init__("coral_fan", True)
-
-    class CoralFanDead(_MinecraftBlock):
-        def __init__(self, coral_color:'BlockStates.CoralColor'=None, coral_fan_direction:'BlockStates.CoralFanDirection'=None):
-            self._coral_color = coral_color
-            self._coral_fan_direction = coral_fan_direction
-            super().__init__("coral_fan_dead", True)
-
     class CoralFanHang(_MinecraftBlock):
         def __init__(self, coral_direction:'BlockStates.CoralDirection'=None, coral_hang_type_bit:'BlockStates.CoralHangTypeBit'=None, dead_bit:'BlockStates.DeadBit'=None):
             self._coral_direction = coral_direction
             self._coral_hang_type_bit = coral_hang_type_bit
             self._dead_bit = dead_bit
             super().__init__("coral_fan_hang", True)
 
@@ -4895,19 +4931,14 @@
             self._lit = lit
             super().__init__("red_candle_cake", True)
 
     class RedCarpet(_MinecraftBlock):
         def __init__(self, ):
             super().__init__("red_carpet", True)
 
-    class RedFlower(_MinecraftBlock):
-        def __init__(self, flower_type:'BlockStates.FlowerType'=None):
-            self._flower_type = flower_type
-            super().__init__("red_flower", True)
-
     class RedGlazedTerracotta(_MinecraftBlock):
         def __init__(self, facing_direction:'BlockStates.FacingDirection'=None):
             self._facing_direction = facing_direction
             super().__init__("red_glazed_terracotta", True)
 
     class RedMushroom(_MinecraftBlock):
         def __init__(self, ):
@@ -4979,20 +5010,14 @@
 
     class SandstoneStairs(_MinecraftBlock):
         def __init__(self, upside_down_bit:'BlockStates.UpsideDownBit'=None, weirdo_direction:'BlockStates.WeirdoDirection'=None):
             self._upside_down_bit = upside_down_bit
             self._weirdo_direction = weirdo_direction
             super().__init__("sandstone_stairs", True)
 
-    class Sapling(_MinecraftBlock):
-        def __init__(self, age_bit:'BlockStates.AgeBit'=None, sapling_type:'BlockStates.SaplingType'=None):
-            self._age_bit = age_bit
-            self._sapling_type = sapling_type
-            super().__init__("sapling", True)
-
     class Scaffolding(_MinecraftBlock):
         def __init__(self, stability:'BlockStates.Stability'=None, stability_check:'BlockStates.StabilityCheck'=None):
             self._stability = stability
             self._stability_check = stability_check
             super().__init__("scaffolding", True)
 
     class Sculk(_MinecraftBlock):
@@ -6218,15 +6243,15 @@
             
     class BlackConcretePowder(_MinecraftBlock):
         def __init__(self,):
             super().__init__("black_concrete_powder", True)
 
     # Added in 1.20.50
     # Planks
-    class OakPlans(_MinecraftBlock):
+    class OakPlanks(_MinecraftBlock):
         def __init__(self, ):
             super().__init__("oak_planks", True)
 
     class SprucePlanks(_MinecraftBlock):
         def __init__(self, ):
             super().__init__("spruce_planks", True)
 
@@ -6271,11 +6296,140 @@
         def __init__(self, ):
             super().__init__("polished_diorite", True)
 
     class PolishedAndesite(_MinecraftBlock):
         def __init__(self, ):
             super().__init__("polished_andesite", True)
 
+    # Added in 1.20.80
+    #Saplings
+    class OakSapling(_MinecraftBlock):
+        def __init__(self, age_bit:'BlockStates.AgeBit'=None):
+            self._age_bit = age_bit
+            super().__init__("oak_sapling", True)
+
+    class SpruceSapling(_MinecraftBlock):
+        def __init__(self, age_bit:'BlockStates.AgeBit'=None):
+            self._age_bit = age_bit
+            super().__init__("spruce_sapling", True)
+
+    class BirchSapling(_MinecraftBlock):
+        def __init__(self, age_bit:'BlockStates.AgeBit'=None):
+            self._age_bit = age_bit
+            super().__init__("birch_sapling", True)
+
+    class JungleSapling(_MinecraftBlock):
+        def __init__(self, age_bit:'BlockStates.AgeBit'=None):
+            self._age_bit = age_bit
+            super().__init__("jungle_sapling", True)
+
+    class AcaciaSapling(_MinecraftBlock):
+        def __init__(self, age_bit:'BlockStates.AgeBit'=None):
+            self._age_bit = age_bit
+            super().__init__("acacia_sapling", True)
+
+    class DarkOakSapling(_MinecraftBlock):
+        def __init__(self, age_bit:'BlockStates.AgeBit'=None):
+            self._age_bit = age_bit
+            super().__init__("dark_oak_sapling", True)
+
+    #Coral
+    class TubeCoralFan(_MinecraftBlock):
+        def __init__(self, coral_fan_direction:'BlockStates.CoralFanDirection'=None):
+            self._coral_fan_direction = coral_fan_direction
+            super().__init__("tube_coral_fan", True)
+
+    class BrainCoralFan(_MinecraftBlock):
+        def __init__(self, coral_fan_direction:'BlockStates.CoralFanDirection'=None):
+            self._coral_fan_direction = coral_fan_direction
+            super().__init__("brain_coral_fan", True)
+    
+    class BubbleCoralFan(_MinecraftBlock):
+        def __init__(self, coral_fan_direction:'BlockStates.CoralFanDirection'=None):
+            self._coral_fan_direction = coral_fan_direction
+            super().__init__("bubble_coral_fan", True)
+
+    class FireCoralFan(_MinecraftBlock):
+        def __init__(self, coral_fan_direction:'BlockStates.CoralFanDirection'=None):
+            self._coral_fan_direction = coral_fan_direction
+            super().__init__("fire_coral_fan", True)
+
+    class HornCoralFan(_MinecraftBlock):
+        def __init__(self, coral_fan_direction:'BlockStates.CoralFanDirection'=None):
+            self._coral_fan_direction = coral_fan_direction
+            super().__init__("horn_coral_fan", True)
+
+    class DeadTubeCoralFan(_MinecraftBlock):
+        def __init__(self, coral_fan_direction:'BlockStates.CoralFanDirection'=None):
+            self._coral_fan_direction = coral_fan_direction
+            super().__init__("dead_tube_coral_fan", True)
+    
+    class DeadBrainCoralFan(_MinecraftBlock):
+        def __init__(self, coral_fan_direction:'BlockStates.CoralFanDirection'=None):
+            self._coral_fan_direction = coral_fan_direction
+            super().__init__("dead_brain_coral_fan", True)
+
+    class DeadBubbleCoralFan(_MinecraftBlock):
+        def __init__(self, coral_fan_direction:'BlockStates.CoralFanDirection'=None):
+            self._coral_fan_direction = coral_fan_direction
+            super().__init__("dead_bubble_coral_fan", True)
+
+    class DeadFireCoralFan(_MinecraftBlock):
+        def __init__(self, coral_fan_direction:'BlockStates.CoralFanDirection'=None):
+            self._coral_fan_direction = coral_fan_direction
+            super().__init__("dead_fire_coral_fan", True)
+
+    class DeadHornCoralFan(_MinecraftBlock):
+        def __init__(self, coral_fan_direction:'BlockStates.CoralFanDirection'=None):
+            self._coral_fan_direction = coral_fan_direction
+            super().__init__("dead_horn_coral_fan", True)
+
+    class Poppy(_MinecraftBlock):
+        def __init__(self):
+            super().__init__("poppy", True)
+
+    class BlueOrchid(_MinecraftBlock):
+        def __init__(self):
+            super().__init__("blue_orchid", True)
+
+    class Allium(_MinecraftBlock):
+        def __init__(self):
+            super().__init__("allium", True)
+
+    class AzureBluet(_MinecraftBlock):
+        def __init__(self):
+            super().__init__("azure_bluet", True)
+            
+    class RedTulip(_MinecraftBlock):
+        def __init__(self):
+            super().__init__("red_tulip", True)
+
+    class OrangeTulip(_MinecraftBlock):
+        def __init__(self):
+            super().__init__("orange_tulip", True)
+
+    class WhiteTulip(_MinecraftBlock):
+        def __init__(self):
+            super().__init__("white_tulip", True)
+
+    class PinkTulip(_MinecraftBlock):
+        def __init__(self):
+            super().__init__("pink_tulip", True)
+
+    class OxeyeDaisy(_MinecraftBlock):
+        def __init__(self):
+            super().__init__("oxeye_daisy", True)
+
+    class Cornflower(_MinecraftBlock):
+        def __init__(self):
+            super().__init__("cornflower", True)
+
+    class LilyOfTheValley(_MinecraftBlock):
+        def __init__(self):
+            super().__init__("lily_of_the_valley", True)
+
+
+
 # Take all the subclasses of Blocks and add them to BLOCK_LIST
 for block in Blocks.__dict__.values():
     if isinstance(block, type) and issubclass(block, Blocks._MinecraftBlock) and block is not Blocks._MinecraftBlock:
         BLOCK_LIST.append(block())
```

### Comparing `mcanvil-0.7.2/src/anvil/cli.py` & `mcanvil-0.7.3/src/anvil/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -418,14 +418,16 @@
 
     config.add_option(ConfigSection.MINECRAFT, ConfigOption.VANILLA_VERSION, latest_build)
     config.add_option(ConfigSection.PACKAGE, ConfigOption.COMPANY, namespace.title())
     config.add_option(ConfigSection.PACKAGE, ConfigOption.NAMESPACE, namespace)
     config.add_option(ConfigSection.PACKAGE, ConfigOption.PROJECT_NAME, project_name)
     config.add_option(ConfigSection.PACKAGE, ConfigOption.DISPLAY_NAME, display_name)
     config.add_option(ConfigSection.PACKAGE, ConfigOption.PROJECT_DESCRIPTION, f"{display_name} Packs")
+    config.add_option(ConfigSection.PACKAGE, ConfigOption.RESOURCE_DESCRIPTION, f"{display_name} Resource Pack")
+    config.add_option(ConfigSection.PACKAGE, ConfigOption.BEHAVIOR_DESCRIPTION, f"{display_name} Behaviour Pack")
     config.add_option(ConfigSection.PACKAGE, ConfigOption.TARGET, "addon" if addon else "world")
     config.add_option(ConfigSection.PACKAGE, ConfigOption.EXPERIMENTAL, preview)
 
     config.add_option(ConfigSection.BUILD, ConfigOption.RELEASE, "1.0.0")
     config.add_option(ConfigSection.BUILD, ConfigOption.RP_UUID, [str(uuid.uuid4())])
     config.add_option(ConfigSection.BUILD, ConfigOption.BP_UUID, [str(uuid.uuid4())])
     config.add_option(ConfigSection.BUILD, ConfigOption.PACK_UUID, str(uuid.uuid4()))
```

### Comparing `mcanvil-0.7.2/src/anvil/lib/config.py` & `mcanvil-0.7.3/src/anvil/lib/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 class ConfigOption(StrEnum):
     VANILLA_VERSION = "vanilla_version"
     COMPANY = "company"
     NAMESPACE = "namespace"
     PROJECT_NAME = "project_name"
     DISPLAY_NAME = "display_name"
     PROJECT_DESCRIPTION = "project_description"
+    RESOURCE_DESCRIPTION = "resource_description"
+    BEHAVIOR_DESCRIPTION = "behavior_description"
+
     TARGET = "target"
 
     RELEASE = "release"
     BP_UUID = "bp_uuid"
     RP_UUID = "rp_uuid"
     PACK_UUID = "pack_uuid"
 
@@ -47,15 +50,15 @@
 class Config:
     """A class used to read and write to the config.ini file."""
 
     def __init__(self) -> None:
         """Initializes a Config object."""
         self._config = {}
         if FileExists("anvilconfig.json"):
-            with open("anvilconfig.json", "r") as f:
+            with open("anvilconfig.json", "r", encoding='utf-8') as f:
                 self._config = json.loads(f.read())
 
     def save(self):
         """Saves the anvilconfig.json file."""
         with open("anvilconfig.json", "w") as f:
             f.write(json.dumps(self._config, indent=4))
 
@@ -119,14 +122,16 @@
 
 class _AnvilConfig:
     COMPANY: str
     NAMESPACE: str
     PROJECT_NAME: str
     DISPLAY_NAME: str
     PROJECT_DESCRIPTION: str
+    RESOURCE_DESCRIPTION: str
+    BEHAVIOR_DESCRIPTION: str
 
     RP_PATH: str
     BP_PATH: str
 
     _VANILLA_VERSION: str
     _RELEASE: str
     _DEBUG: bool
@@ -166,14 +171,20 @@
         self.COMPANY = self._handle_config(ConfigSection.PACKAGE, ConfigOption.COMPANY, "input")
         self.DISPLAY_NAME = self._handle_config(
             ConfigSection.PACKAGE, ConfigOption.DISPLAY_NAME, "input"
         )
         self.PROJECT_DESCRIPTION = self._handle_config(
             ConfigSection.PACKAGE, ConfigOption.PROJECT_DESCRIPTION, "input"
         )
+        self.BEHAVIOR_DESCRIPTION = self._handle_config(
+            ConfigSection.PACKAGE, ConfigOption.BEHAVIOR_DESCRIPTION, "input"
+        )
+        self.RESOURCE_DESCRIPTION = self._handle_config(
+            ConfigSection.PACKAGE, ConfigOption.RESOURCE_DESCRIPTION, "input"
+        )
         self._DEBUG = self._handle_config(ConfigSection.ANVIL, ConfigOption.DEBUG, False)
         self._PASCAL_PROJECT_NAME = self._handle_config(
             ConfigSection.ANVIL, ConfigOption.PASCAL_PROJECT_NAME, "".join(x[0] for x in self.PROJECT_NAME.split("_")).upper()
         )
 
         self._VANILLA_VERSION = self._handle_config(ConfigSection.MINECRAFT, ConfigOption.VANILLA_VERSION, MANIFEST_BUILD)
         self._TARGET = self._handle_config(ConfigSection.PACKAGE, ConfigOption.TARGET, "world")
```

### Comparing `mcanvil-0.7.2/src/anvil/lib/core.py` & `mcanvil-0.7.3/src/anvil/lib/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Provides the core functionality of the Anvil library."""
+
 import os
 from atexit import register
 from datetime import datetime
 
 import commentjson
 from bs4 import Stylesheet
 from halo import Halo
@@ -78,26 +79,31 @@
             sound_reference,
             category,
             use_legacy_max_distance,
             max_distance,
             min_distance,
         )
 
-    def register_sound_event(
+    def register_entity_sound_event(
         self,
         entity_identifier: Identifier,
         sound_identifier,
         sound_event: EntitySoundEvent,
         volume: float = 1.0,
         pitch: tuple[float, float] = (0.8, 1.2),
     ):
         if self._sound_event_object is None:
             self._sound_event_object = SoundEvent()
         return self._sound_event_object.add_entity_event(entity_identifier, sound_identifier, sound_event, volume, pitch)
 
+    def register_block_sound_event(self):
+        """# TO IMPLEMENT
+        Registers a block sound event."""
+        pass
+
     def register_item_textures(self, item_name: str, directory: str, *item_sprites: str):
         if self._item_textures_object is None:
             self._item_textures_object = ItemTexturesObject()
         return self._item_textures_object.add_item(item_name, directory, *item_sprites)
 
     def register_music(self, music_category: MusicCategory, min_delay: int = 60, max_delay: int = 180):
         """Adds a music to the music definition.
@@ -193,40 +199,45 @@
     def get_new_lang(self):
         id = f"raw_text_{self._raw_text}"
         self._raw_text += 1
         return id
 
     def _export_manifest(self):
         release_list = [int(i) for i in self.config._RELEASE.split(".")]
-        manifest_rp = JsonSchemes.manifest_rp(release_list, self.config._RP_UUID[0], self.config._BP_UUID[0], self.config.COMPANY, self.config._PBR, self.config._TARGET == "addon")
-        manifest_bp = JsonSchemes.manifest_bp(release_list, self.config._BP_UUID[0], self.config._RP_UUID[0], self.config.COMPANY, self.config._SCRIPT_API, self.config._SCRIPT_UI)
-        manifest_world = JsonSchemes.manifest_world(release_list, self.config._PACK_UUID, self.config.COMPANY, self.config._RANDOM_SEED)
-        world_rp_pack = JsonSchemes.world_packs(self.config._RP_UUID, release_list)
-        world_bp_pack = JsonSchemes.world_packs(self.config._BP_UUID, release_list)
-
-        File("manifest.json", manifest_rp, self.config.RP_PATH, "w")
-        File("manifest.json", manifest_bp, self.config.BP_PATH, "w")
-        File("manifest.json", manifest_world, "", "w")
 
-        File("world_resource_packs.json", world_rp_pack, "", "w")
-        File("world_behavior_packs.json", world_bp_pack, "", "w")
+        File("manifest.json", JsonSchemes.manifest_rp(version=release_list), self.config.RP_PATH, "w")
+        File("manifest.json", JsonSchemes.manifest_bp(version=release_list), self.config.BP_PATH, "w")
+        File("manifest.json", JsonSchemes.manifest_world(version=release_list), "", "w")
+
+        File("world_resource_packs.json", JsonSchemes.world_packs(release_list, self.config._RP_UUID), "", "w")
+        File("world_behavior_packs.json", JsonSchemes.world_packs(release_list, self.config._BP_UUID), "", "w")
 
     def _export_language(self):
-        default_langs = JsonSchemes.pack_name_lang(self.config.DISPLAY_NAME, self.config.PROJECT_DESCRIPTION)
+        default_langs = JsonSchemes.pack_name_lang(self.config.DISPLAY_NAME, self.config.RESOURCE_DESCRIPTION)
         langs = default_langs.copy()
         langs.extend([f"{k}={v}" for k, v in self._language.items()])
         langs.sort(reverse=True)
 
         File("languages.json", JsonSchemes.languages(), os.path.join(self.config.BP_PATH, "texts"), "w")
         File("languages.json", JsonSchemes.languages(), os.path.join(self.config.RP_PATH, "texts"), "w")
         File("languages.json", JsonSchemes.languages(), "texts", "w")
 
         File("en_US.lang", "\n".join(langs), os.path.join(self.config.RP_PATH, "texts"), "w")
-        File("en_US.lang", "\n".join(default_langs), os.path.join(self.config.BP_PATH, "texts"), "w")
-        File("en_US.lang", "\n".join(default_langs), "texts", "w")
+        File(
+            "en_US.lang",
+            "\n".join(JsonSchemes.pack_name_lang(self.config.DISPLAY_NAME, self.config.BEHAVIOR_DESCRIPTION)),
+            os.path.join(self.config.BP_PATH, "texts"),
+            "w",
+        )
+        File(
+            "en_US.lang",
+            "\n".join(JsonSchemes.pack_name_lang(self.config.DISPLAY_NAME, self.config.PROJECT_DESCRIPTION)),
+            "texts",
+            "w",
+        )
 
     def _export_scripts(self):
         File(
             "package.json",
             JsonSchemes.packagejson(
                 self.config.PROJECT_NAME, self.config._RELEASE, self.config.PROJECT_DESCRIPTION, self.config.COMPANY
             ),
@@ -297,15 +308,15 @@
             self._terrain_texture_object.queue
         if not self._blocks_object == None:
             self._blocks_object.queue
 
         self._export_manifest()
         self._export_language()
         self._export_helper_functions()
-        
+
         if any([self.config._SCRIPT_API, self.config._SCRIPT_UI]):
             self._export_scripts()
 
 
 class _AnvilCore:
     """A class representing an Anvil instance."""
 
@@ -366,15 +377,15 @@
         Usage:
         ---------
         >>> ANVIL.translate
         """
         from deep_translator import GoogleTranslator
 
         def _to_lang(translator: GoogleTranslator, langs: dict):
-            lang = JsonSchemes.pack_name_lang(self.config.PROJECT_NAME, self.config.PROJECT_NAME)
+            lang = JsonSchemes.pack_name_lang(self.config.DISPLAY_NAME, self.config.PROJECT_DESCRIPTION)
             translated = translator.translate_batch(langs.values())
             for k, v in zip(langs.keys(), translated):
                 lang.append(f"{k}={v}")
             return lang
 
         for language in JsonSchemes.languages():
             destination_language = (
@@ -412,27 +423,35 @@
     def compile(self) -> None:
         """Compiles the project."""
 
         self._definitions.queue
 
         for object in self._objects_list:
             object._export()
-            
+
         from anvil.api.actors import _ActorClientDescription
+
         _ActorClientDescription._export()
 
         from anvil.api.blocks import _PermutationComponents
+
         if _PermutationComponents._count > 10000:
             if self.config._TARGET == "addon":
                 self.config.Logger.too_many_permutations(_PermutationComponents._count)
             else:
                 self.config.Logger.too_many_permutations_warn(_PermutationComponents._count)
 
         if self.config._SCRIPT_API:
-            File("anvilConstants.ts", JsonSchemes.tsconstants(self.config.NAMESPACE, self.config.PROJECT_NAME), os.path.join("assets", "javascript"), "w", False)
+            File(
+                "anvilConstants.ts",
+                JsonSchemes.tsconstants(self.config.NAMESPACE, self.config.PROJECT_NAME),
+                os.path.join("assets", "javascript"),
+                "w",
+                False,
+            )
 
             source = os.path.join("assets", "javascript")
             target = os.path.join(self.config.BP_PATH, "scripts")
 
             do_ts = False
             for subdir, dirname, files in os.walk(source):
                 for file in files:
@@ -533,17 +552,17 @@
                 output_store,
                 (round(original.size[0] * scale_factor), 450),
                 95,
                 72,
             )
 
         else:
-            self.config.Logger.file_exist_warning("panorama.png")
+            self.config.Logger.file_exist_info("panorama.png")
 
-        for i in range(5):
+        for i in range(999):
             if not FileExists(os.path.join(source, f"{i}.png")):
                 if i < 5:
                     self.config.Logger.file_exist_warning(f"{i}.png")
                 break
             else:
                 original = Image.open(os.path.join(source, f"{i}.png"))
                 resize(
@@ -586,49 +605,55 @@
         skip_translation: bool = False,
         apply_overlay: bool = False,
     ) -> None:
         if not self._compiled:
             self.config.Logger.not_compiled()
         self.config.Logger.packaging_zip()
 
-        content_structure = {}
-
         if not skip_translation:
             self.translate()
 
         self._process_art(apply_overlay)
 
-        content_structure.update(
-            {
-                os.path.join("assets", "output", "Store Art"): os.path.join("Store Art"),
-                os.path.join("assets", "output", "Marketing Art"): os.path.join("Marketing Art"),
-                "resource_packs": os.path.join("Content", "world_template", "resource_packs"),
-                "behavior_packs": os.path.join("Content", "world_template", "behavior_packs"),
-                "texts": os.path.join("Content", "world_template", "texts"),
-                "level.dat": os.path.join("Content", "world_template"),
-                "levelname.txt": os.path.join("Content", "world_template"),
-                "manifest.json": os.path.join("Content", "world_template"),
-                "world_icon.jpeg": os.path.join("Content", "world_template"),
-                "world_behavior_packs.json": os.path.join("Content", "world_template"),
-                "world_resource_packs.json": os.path.join("Content", "world_template"),
-            }
-        )
-
-        if not self.config._RANDOM_SEED:
-            content_structure.update(
-                {
-                    "db": os.path.join("Content", "world_template", "db"),
-                }
-            )
+        content_structure = {
+            os.path.join("assets", "output", "Store Art"): os.path.join("Store Art"),
+            os.path.join("assets", "output", "Marketing Art"): os.path.join("Marketing Art"),
+        }
 
         if self.config._TARGET == "addon":
             if len(self.config._RP_UUID) > 1:
                 self.config.Logger.multiple_rp_uuids()
             if len(self.config._BP_UUID) > 1:
                 self.config.Logger.multiple_bp_uuids()
+            
+            content_structure.update({
+                    "resource_packs": os.path.join("Content", "resource_packs"),
+                    "behavior_packs": os.path.join("Content", "behavior_packs"),
+                })
+
+        else:
+            content_structure.update(
+                {
+                    "resource_packs": os.path.join("Content", "world_template", "resource_packs"),
+                    "behavior_packs": os.path.join("Content", "world_template", "behavior_packs"),
+                    "texts": os.path.join("Content", "world_template", "texts"),
+                    "level.dat": os.path.join("Content", "world_template"),
+                    "levelname.txt": os.path.join("Content", "world_template"), 
+                    "manifest.json": os.path.join("Content", "world_template"),
+                    "world_icon.jpeg": os.path.join("Content", "world_template"),
+                    "world_behavior_packs.json": os.path.join("Content", "world_template"),
+                    "world_resource_packs.json": os.path.join("Content", "world_template"),
+                }
+            )
+            if not self.config._RANDOM_SEED:
+                content_structure.update(
+                    {
+                        "db": os.path.join("Content", "world_template", "db"),
+                    }
+                )
 
         zipit(
             os.path.join("assets", "output", f"{self.config.PROJECT_NAME}.zip"),
             content_structure,
         )
 
         RemoveDirectory(os.path.join("assets", "output", "Store Art"))
@@ -759,16 +784,14 @@
             subject=f"{self.config.DISPLAY_NAME} Technical Notes",
             creator=f"Anvil@stark_lg {__version__}",
         )
         styles = getSampleStyleSheet()
         title_style = styles["Heading1"]
         body_style = styles["BodyText"]
         bullet_style = styles["Bullet"]
-        
-
 
         elements = [
             Paragraph(f"{self.config.DISPLAY_NAME}:", title_style),
             Paragraph(f"Developed by: {self.config.COMPANY}", body_style),
             Paragraph(f"Generated with StarkTMA/Anvil {__version__}", body_style),
             Spacer(1, 1 * cm),
             Paragraph("General information:", title_style),
```

### Comparing `mcanvil-0.7.2/src/anvil/lib/format_versions.py` & `mcanvil-0.7.3/src/anvil/lib/format_versions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-MANIFEST_BUILD: str = "1.20.70"  # The build version of the manifest.
+MANIFEST_BUILD: str = "1.20.80"  # The build version of the manifest.
 BLOCK_SERVER_VERSION: str = "1.20.30"  # The version of the block server.
-ENTITY_SERVER_VERSION: str = "1.20.70"  # The version of the entity server.
+ENTITY_SERVER_VERSION: str = "1.20.80"  # The version of the entity server.
 ENTITY_CLIENT_VERSION: str = "1.10.0"  # The version of the entity client.
 BP_ANIMATION_VERSION: str = "1.10.0"  # The version of the behavior pack animation.
 RP_ANIMATION_VERSION: str = "1.8.0"  # The version of the resource pack animation.
 ANIMATION_CONTROLLERS_VERSION: str = "1.10.0"  # The version of the animation controllers.
 SPAWN_RULES_VERSION: str = "1.8.0"  # The version of the spawn rules.
 GEOMETRY_VERSION: str = "1.12.0"  # The version of the geometry.
 RENDER_CONTROLLER_VERSION: str = "1.10.0"  # The version of the render controller.
 SOUND_DEFINITIONS_VERSION: str = "1.20.20"  # The version of the sound definitions.
 DIALOGUE_VERSION: str = "1.18.0"  # The version of the dialogue.
 FOG_VERSION: str = "1.16.100"  # The version of the fog.
 MATERIALS_VERSION: str = "1.0.0"  # The version of the materials.
-ITEM_SERVER_VERSION: str = "1.20.50"  # The version of the item server.
+ITEM_SERVER_VERSION: str = "1.20.70"  # The version of the item server.
 GLOBAL_LIGHTING = "1.0.0"
-CAMERA_PRESET_VERSION = "1.19.50"  # The version of the camera presets.
+CAMERA_PRESET_VERSION = "1.20.80"  # The version of the camera presets.
 BLOCK_JSON_FORMAT_VERSION = "1.1.0"  # The version of the block json format.
 
-MODULE_MINECRAFT_SERVER: str = "1.9.0"  # The version of the Minecraft server module.
+MODULE_MINECRAFT_SERVER: str = "1.10.0"  # The version of the Minecraft server module.
 MODULE_MINECRAFT_SERVER_UI: str = "1.1.0"  # The version of the Minecraft UI module.
 MODULE_MINECRAFT_SERVER_EDITOR: str = "0.1.0"  # The version of the Minecraft UI module.
 MODULE_MINECRAFT_SERVER_GAMETEST: str = "1.0.0"  # The version of the Minecraft UI module.
```

### Comparing `mcanvil-0.7.2/src/anvil/lib/lib.py` & `mcanvil-0.7.3/src/anvil/lib/lib.py`

 * *Files identical despite different names*

### Comparing `mcanvil-0.7.2/src/anvil/lib/logger.py` & `mcanvil-0.7.3/src/anvil/lib/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,20 @@
 
     # Error
     def file_exist_error(self, filename, directory):
         m = f'{filename} could not be found at "{directory}".'
         self.logger.error(m)
         raise FileNotFoundError(self.Red("[ERROR]: " + m))
 
+    # Info
+    def file_exist_info(self, filename):
+        m = f"{filename} does not exist. It is optional but might have been left out unintentionally."
+        self.logger.info(m)
+        click.echo(self.Cyan("[INFO]: " + m))
+
     # Error
     def path_length_error(self, path):
         m = f"Relative file path [{path}] has [{len(path)}] characters, but cannot be more than [80] characters."
         self.logger.error(m)
         raise FileNotFoundError(self.Red("[ERROR]: " + m))
 
     # Error
@@ -285,25 +291,25 @@
         self.logger.error(m)
         raise RuntimeError(self.Red("[ERROR]: " + m))
 
     def missing_render_controller(self, entity):
         m = f"[{entity}] is missing a render_controller"
         self.logger.error(m)
         raise RuntimeError(self.Red("[ERROR]: " + m))
-    
+
     def missing_geometry(self, entity):
         m = f"[{entity}] is missing a geometry"
         self.logger.error(m)
         raise RuntimeError(self.Red("[ERROR]: " + m))
-    
+
     def missing_texture(self, entity):
         m = f"[{entity}] is missing a texture"
         self.logger.error(m)
         raise RuntimeError(self.Red("[ERROR]: " + m))
-    
+
     def lang_error(self, text):
         m = f"Invalid localized string at {text}"
         self.logger.error(m)
         raise RuntimeError(self.Red("[ERROR]: " + m))
 
     def sound_category_error(self):
         m = f"Invalid sound category"
@@ -355,39 +361,39 @@
         raise RuntimeError(self.Red("[ERROR]: " + m))
 
     # Error
     def experimental_not_allowed(self, identifier):
         m = f"Experimental features are not allowed for packages of type : 'addon'. Error at {identifier}."
         self.logger.error(m)
         raise RuntimeError(self.Red("[ERROR]: " + m))
-    
+
     # Warn
     def entity_marked_as_experimental(self, identifier):
         m = f"Entity {identifier} is marked as experimental. This may be unintentional."
         self.logger.warn(m)
         click.echo(self.Yellow("[WARNING]: " + m))
-    
+
     # Error
     def too_many_permutations(self, count):
         m = f"Total Block permutations exceeded 10000 ({count}). For minimal performance impact, reduce the number of permutations."
         self.logger.error(m)
         raise RuntimeError(self.Red("[ERROR]: " + m))
-    
+
     # Warn
     def too_many_permutations_warn(self, count):
         m = f"Total Block permutations exceeded 10000 ({count}). For minimal performance impact, consider reducing the number of permutations."
         self.logger.warn(m)
         click.echo(self.Yellow("[WARNING]: " + m))
 
     # Error
     def multiple_rp_uuids(self, identifier):
         m = f"Multiple resource pack uuids found. Error at {identifier}."
         self.logger.error(m)
         raise RuntimeError(self.Red("[ERROR]: " + m))
-    
+
     # Error
     def multiple_bp_uuids(self, identifier):
         m = f"Multiple behavior pack uuids found. Error at {identifier}."
         self.logger.error(m)
         raise RuntimeError(self.Red("[ERROR]: " + m))
 
     # Error
@@ -409,13 +415,29 @@
         raise RuntimeError(self.Red("[ERROR]: " + m))
 
     # Error
     def component_required(self, identifier, requirer, required):
         m = f"The component {requirer} requires the component {required} to be added to {identifier}."
         self.logger.error(m)
         raise RuntimeError(self.Red("[ERROR]: " + m))
-    
+
     # Error
     def recipe_max_items(self, name):
         m = f"Recipes cannot have more than 9 items. Error at {name}."
         self.logger.error(m)
-        raise RuntimeError(self.Red("[ERROR]: " + m))
+        raise RuntimeError(self.Red("[ERROR]: " + m))
+
+    # Error
+    def entity_not_valid_vanilla(self, name):
+        m = f"{name} is not a valid vanilla entity."
+        self.logger.error(m)
+        raise RuntimeError(self.Red("[ERROR]: " + m))
+
+    def namespace_not_valid(self, namespace):
+        m = f"{namespace} is not a valid namespace."
+        self.logger.error(m)
+        raise RuntimeError(self.Red("[ERROR]: " + m))
+
+    def extend_player_rendering_not_free(self, camera_preset: str):
+        m = f"Extending player component is only supported with the Free preset. Error at {camera_preset}."
+        self.logger.error(m)
+        raise RuntimeError(self.Red("[ERROR]: " + m))
```

### Comparing `mcanvil-0.7.2/src/anvil/lib/materials.py` & `mcanvil-0.7.3/src/anvil/lib/materials.py`

 * *Files identical despite different names*

### Comparing `mcanvil-0.7.2/src/anvil/lib/reports.py` & `mcanvil-0.7.3/src/anvil/lib/reports.py`

 * *Files identical despite different names*

### Comparing `mcanvil-0.7.2/src/anvil/lib/schemas.py` & `mcanvil-0.7.3/src/anvil/lib/schemas.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 import uuid
 
 from anvil import CONFIG
-from anvil.lib.config import _AnvilConfig
 from anvil.lib.format_versions import *
 from anvil.lib.lib import File
 
 
 class JsonSchemes:
     """A class used to read and write to the json_schemes.json file."""
 
@@ -15,29 +14,29 @@
         return [f"pack.name={name}", f"pack.description={description}"]
 
     @staticmethod
     def skin_pack_name_lang(name, display_name):
         return [f"skinpack.{name}={display_name}"]
 
     @staticmethod
-    def manifest_bp(version, uuid1, rpuuid, author, has_script: bool, server_ui: bool):
+    def manifest_bp(version):
         m = {
             "format_version": 2,
             "header": {
                 "description": "pack.description",
                 "name": "pack.name",
-                "uuid": uuid1,
+                "uuid": CONFIG._BP_UUID[0],
                 "version": version,
                 "min_engine_version": [int(i) for i in MANIFEST_BUILD.split(".")],
             },
             "modules": [{"type": "data", "uuid": str(uuid.uuid4()), "version": version}],
-            "dependencies": [{"uuid": rpuuid, "version": version}],
-            "metadata": {"authors": [author]},
+            "dependencies": [{"uuid": CONFIG._RP_UUID[0], "version": version}],
+            "metadata": {"authors": [CONFIG.COMPANY]},
         }
-        if has_script:
+        if CONFIG._SCRIPT_API:
             m["modules"].append(
                 {
                     "uuid": str(uuid.uuid4()),
                     "version": version,
                     "type": "script",
                     "language": "javascript",
                     "entry": "scripts/main.js",
@@ -45,77 +44,84 @@
             )
             m["dependencies"].append(
                 {
                     "module_name": "@minecraft/server",
                     "version": MODULE_MINECRAFT_SERVER,
                 }
             )
-            if server_ui:
+            if CONFIG._SCRIPT_UI:
                 m["dependencies"].append(
                     {
                         "module_name": "@minecraft/server-ui",
                         "version": MODULE_MINECRAFT_SERVER_UI,
                     }
                 )
+        if CONFIG._TARGET == "addon":
+            m["header"]["pack_scope"] = "world"
+            m["metadata"]["product_type"] = "addon"
         return m
 
     @staticmethod
-    def manifest_rp(version, uuid1, bp_uuid, author, has_pbr, addon):
+    def manifest_rp(version):
         m = {
             "format_version": 2,
             "header": {
                 "description": "pack.description",
                 "name": "pack.name",
-                "uuid": uuid1,
+                "uuid": CONFIG._RP_UUID[0],
                 "version": version,
                 "min_engine_version": [int(i) for i in MANIFEST_BUILD.split(".")],
             },
             "modules": [
                 {
                     "type": "resources",
                     "uuid": str(uuid.uuid4()),
                     "version": version,
                 }
             ],
-            "dependencies": [{"uuid": bp_uuid, "version": version}],
-            "metadata": {"authors": [author]},
+            "dependencies": [{"uuid": CONFIG._BP_UUID[0], "version": version}],
+            "metadata": {"authors": [CONFIG.COMPANY]},
         }
-        if has_pbr:
+        if CONFIG._PBR:
             m.update({"capabilities": ["pbr"]})
-        if addon:
+        if CONFIG._TARGET == "addon":
             m["header"]["pack_scope"] = "world"
             m["metadata"]["product_type"] = "addon"
         return m
 
     @staticmethod
-    def manifest_world(version, uuid1, author, seed):
-        return {
+    def manifest_world(version):
+        m = {
             "format_version": 2,
             "header": {
                 "name": "pack.name",
                 "description": "pack.description",
                 "version": version,
-                "uuid": uuid1,
+                "uuid": CONFIG._PACK_UUID,
                 # "platform_locked": False,
                 "lock_template_options": True,
                 "base_game_version": [int(i) for i in MANIFEST_BUILD.split(".")],
-                "allow_random_seed": seed,
             },
             "modules": [
                 {
                     "type": "world_template",
                     "uuid": str(uuid.uuid4()),
                     "version": version,
                 }
             ],
-            "metadata": {"authors": [author]},
+            "metadata": {"authors": [CONFIG.COMPANY]},
         }
 
+        if CONFIG._RANDOM_SEED:
+            m["header"]["allow_random_seed"] = True
+
+        return m
+
     @staticmethod
-    def world_packs(pack_id, version):
+    def world_packs(version, pack_id):
         return [{"pack_id": i, "version": version} for i in pack_id]
 
     @staticmethod
     def code_workspace(name, path1, path2):
         return {
             "folders": [
                 {"name": name, "path": os.path.join(path1, path2)},
@@ -532,20 +538,21 @@
                 "description": {"identifier": f"{namespace}:{name}"},
                 "tags": tags,
                 "ingredients": [],
             },
         }
 
     @staticmethod
-    def shaped_crafting_recipe(namespace: str, name: str, tags: list[str]):
+    def shaped_crafting_recipe(namespace: str, name: str, assume_symmetry: bool, tags: list[str]):
         return {
             "format_version": "1.12",
             "minecraft:recipe_shaped": {
                 "description": {"identifier": f"{namespace}:{name}"},
                 "tags": tags,
+                "assume_symmetry": assume_symmetry,
                 "pattern": [],
                 "key": {},
             },
         }
 
     @staticmethod
     def tsconstants(namespace: str, project_name: str):
```

### Comparing `mcanvil-0.7.2/src/anvil/lib/sounds.py` & `mcanvil-0.7.3/src/anvil/lib/sounds.py`

 * *Files identical despite different names*

### Comparing `mcanvil-0.7.2/src/anvil/lib/textures.py` & `mcanvil-0.7.3/src/anvil/lib/textures.py`

 * *Files identical despite different names*

### Comparing `mcanvil-0.7.2/src/anvil/tools/functions.py` & `mcanvil-0.7.3/src/anvil/tools/functions.py`

 * *Files identical despite different names*

### Comparing `mcanvil-0.7.2/src/mcanvil.egg-info/PKG-INFO` & `mcanvil-0.7.3/src/mcanvil.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcanvil
-Version: 0.7.2
+Version: 0.7.3
 Summary: A Minecraft bedrock content development framework.
 Home-page: https://anvil.starktma.net/
 Author: Yasser A. Benfoughal
 Author-email: yasser@starktma.net
 License: GNU GPLv3
 Project-URL: Github, https://github.com/StarkTMA/Anvil
 Project-URL: Website, https://starktma.net
@@ -32,15 +32,15 @@
 Requires-Dist: reportlab
 
 <img src="https://starktma.net/wp-content/uploads/2022/04/logo.png" width="300" alt="Anvil Logo">
 
 # Anvil
 
 ![Python 10](https://img.shields.io/badge/python-3.10%20%20|%20%203.11%20%20|%20%203.12-g.svg)
-![Anvil Version](https://img.shields.io/badge/beta-0.7.2-yellow.svg)
+![Anvil Version](https://img.shields.io/badge/beta-0.7.3-yellow.svg)
 ![OS](https://img.shields.io/badge/OS-Windows-blue.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ---
 
 ## What is Anvil?
```

### Comparing `mcanvil-0.7.2/src/mcanvil.egg-info/SOURCES.txt` & `mcanvil-0.7.3/src/mcanvil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

