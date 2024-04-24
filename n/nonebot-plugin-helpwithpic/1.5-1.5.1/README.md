# Comparing `tmp/nonebot_plugin_helpwithpic-1.5.tar.gz` & `tmp/nonebot_plugin_helpwithpic-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_helpwithpic-1.5.tar", last modified: Tue Apr 23 08:10:49 2024, max compression
+gzip compressed data, was "nonebot_plugin_helpwithpic-1.5.1.tar", last modified: Wed Apr 24 09:46:24 2024, max compression
```

## Comparing `nonebot_plugin_helpwithpic-1.5.tar` & `nonebot_plugin_helpwithpic-1.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:10:49.502632 nonebot_plugin_helpwithpic-1.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-23 08:10:39.000000 nonebot_plugin_helpwithpic-1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    44311 2024-04-23 08:10:49.502632 nonebot_plugin_helpwithpic-1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-23 08:10:39.000000 nonebot_plugin_helpwithpic-1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:10:49.498632 nonebot_plugin_helpwithpic-1.5/nonebot_plugin_helpwithpic/
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-23 08:10:39.000000 nonebot_plugin_helpwithpic-1.5/nonebot_plugin_helpwithpic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-23 08:10:39.000000 nonebot_plugin_helpwithpic-1.5/nonebot_plugin_helpwithpic/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8200 2024-04-23 08:10:39.000000 nonebot_plugin_helpwithpic-1.5/nonebot_plugin_helpwithpic/draw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-23 08:10:39.000000 nonebot_plugin_helpwithpic-1.5/nonebot_plugin_helpwithpic/draw_contect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-23 08:10:39.000000 nonebot_plugin_helpwithpic-1.5/nonebot_plugin_helpwithpic/hwp_main.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-23 08:10:39.000000 nonebot_plugin_helpwithpic-1.5/nonebot_plugin_helpwithpic/jsondata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-23 08:10:39.000000 nonebot_plugin_helpwithpic-1.5/nonebot_plugin_helpwithpic/plugins_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:10:49.502632 nonebot_plugin_helpwithpic-1.5/nonebot_plugin_helpwithpic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44311 2024-04-23 08:10:49.000000 nonebot_plugin_helpwithpic-1.5/nonebot_plugin_helpwithpic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-23 08:10:49.000000 nonebot_plugin_helpwithpic-1.5/nonebot_plugin_helpwithpic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 08:10:49.000000 nonebot_plugin_helpwithpic-1.5/nonebot_plugin_helpwithpic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-23 08:10:49.000000 nonebot_plugin_helpwithpic-1.5/nonebot_plugin_helpwithpic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-23 08:10:49.000000 nonebot_plugin_helpwithpic-1.5/nonebot_plugin_helpwithpic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-23 08:10:39.000000 nonebot_plugin_helpwithpic-1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 08:10:49.502632 nonebot_plugin_helpwithpic-1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:46:24.367210 nonebot_plugin_helpwithpic-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 09:46:20.000000 nonebot_plugin_helpwithpic-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    44334 2024-04-24 09:46:24.363210 nonebot_plugin_helpwithpic-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-24 09:46:20.000000 nonebot_plugin_helpwithpic-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:46:24.363210 nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic/
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-24 09:46:20.000000 nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-24 09:46:20.000000 nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8200 2024-04-24 09:46:20.000000 nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-24 09:46:20.000000 nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic/draw_contect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-24 09:46:20.000000 nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic/hwp_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-24 09:46:20.000000 nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic/jsondata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-24 09:46:20.000000 nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic/plugins_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:46:24.363210 nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44334 2024-04-24 09:46:24.000000 nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-24 09:46:24.000000 nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 09:46:24.000000 nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-24 09:46:24.000000 nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-24 09:46:24.000000 nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-24 09:46:20.000000 nonebot_plugin_helpwithpic-1.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 09:46:24.367210 nonebot_plugin_helpwithpic-1.5.1/setup.cfg
```

### Comparing `nonebot_plugin_helpwithpic-1.5/LICENSE` & `nonebot_plugin_helpwithpic-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helpwithpic-1.5/PKG-INFO` & `nonebot_plugin_helpwithpic-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-helpwithpic
-Version: 1.5
+Version: 1.5.1
 Summary: nonebot插件-动态帮助图片制作
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -683,14 +683,15 @@
 Keywords: egg,bacon,sausage,tomatoes,Lobster Thermidor
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
+Requires-Dist: anyio
 Requires-Dist: nonebot-adapter-onebot
 Requires-Dist: nonebot-plugin-localstore
 Requires-Dist: aiohttp
 Requires-Dist: pil_utils
 Requires-Dist: pillow
 
 <div align="center">
```

### Comparing `nonebot_plugin_helpwithpic-1.5/README.md` & `nonebot_plugin_helpwithpic-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helpwithpic-1.5/nonebot_plugin_helpwithpic/__init__.py` & `nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helpwithpic-1.5/nonebot_plugin_helpwithpic/config.py` & `nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helpwithpic-1.5/nonebot_plugin_helpwithpic/draw.py` & `nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helpwithpic-1.5/nonebot_plugin_helpwithpic/draw_contect.py` & `nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic/draw_contect.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helpwithpic-1.5/nonebot_plugin_helpwithpic/hwp_main.py` & `nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic/hwp_main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helpwithpic-1.5/nonebot_plugin_helpwithpic/jsondata.py` & `nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic/jsondata.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helpwithpic-1.5/nonebot_plugin_helpwithpic/plugins_data.py` & `nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic/plugins_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helpwithpic-1.5/nonebot_plugin_helpwithpic.egg-info/PKG-INFO` & `nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-helpwithpic
-Version: 1.5
+Version: 1.5.1
 Summary: nonebot插件-动态帮助图片制作
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -683,14 +683,15 @@
 Keywords: egg,bacon,sausage,tomatoes,Lobster Thermidor
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
+Requires-Dist: anyio
 Requires-Dist: nonebot-adapter-onebot
 Requires-Dist: nonebot-plugin-localstore
 Requires-Dist: aiohttp
 Requires-Dist: pil_utils
 Requires-Dist: pillow
 
 <div align="center">
```

### Comparing `nonebot_plugin_helpwithpic-1.5/nonebot_plugin_helpwithpic.egg-info/SOURCES.txt` & `nonebot_plugin_helpwithpic-1.5.1/nonebot_plugin_helpwithpic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_helpwithpic-1.5/pyproject.toml` & `nonebot_plugin_helpwithpic-1.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-helpwithpic"
-version = "1.5"
+version = "1.5.1"
 description = "nonebot插件-动态帮助图片制作"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 keywords = ["egg", "bacon", "sausage", "tomatoes", "Lobster Thermidor"]
 authors = [
   {email = "cub_staryow@outlook.com"},
@@ -13,14 +13,15 @@
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python"
 ]
 
 dependencies = [
   "nonebot2",
+  "anyio",
   "nonebot-adapter-onebot",
   "nonebot-plugin-localstore",
   "aiohttp",
   "pil_utils",
   "pillow"
 ]
```

