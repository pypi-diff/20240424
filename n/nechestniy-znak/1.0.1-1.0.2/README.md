# Comparing `tmp/nechestniy_znak-1.0.1.tar.gz` & `tmp/nechestniy_znak-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nechestniy_znak-1.0.1.tar", last modified: Tue Apr 23 19:33:57 2024, max compression
+gzip compressed data, was "nechestniy_znak-1.0.2.tar", last modified: Wed Apr 24 14:52:14 2024, max compression
```

## Comparing `nechestniy_znak-1.0.1.tar` & `nechestniy_znak-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:33:57.559353 nechestniy_znak-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-23 19:33:53.000000 nechestniy_znak-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-23 19:33:57.559353 nechestniy_znak-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-23 19:33:53.000000 nechestniy_znak-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-23 19:33:53.000000 nechestniy_znak-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:33:57.559353 nechestniy_znak-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:33:57.555353 nechestniy_znak-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:33:57.555353 nechestniy_znak-1.0.1/src/nechestniy_znak/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 19:33:53.000000 nechestniy_znak-1.0.1/src/nechestniy_znak/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-23 19:33:53.000000 nechestniy_znak-1.0.1/src/nechestniy_znak/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:33:57.559353 nechestniy_znak-1.0.1/src/nechestniy_znak.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-23 19:33:57.000000 nechestniy_znak-1.0.1/src/nechestniy_znak.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-23 19:33:57.000000 nechestniy_znak-1.0.1/src/nechestniy_znak.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:33:57.000000 nechestniy_znak-1.0.1/src/nechestniy_znak.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 19:33:57.000000 nechestniy_znak-1.0.1/src/nechestniy_znak.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 19:33:57.000000 nechestniy_znak-1.0.1/src/nechestniy_znak.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:52:14.570920 nechestniy_znak-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-24 14:52:06.000000 nechestniy_znak-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-24 14:52:14.570920 nechestniy_znak-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-24 14:52:06.000000 nechestniy_znak-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-24 14:52:06.000000 nechestniy_znak-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 14:52:14.570920 nechestniy_znak-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:52:14.566920 nechestniy_znak-1.0.2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 14:52:06.000000 nechestniy_znak-1.0.2/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:52:14.566920 nechestniy_znak-1.0.2/src/nechestniy_znak/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-24 14:52:06.000000 nechestniy_znak-1.0.2/src/nechestniy_znak/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-24 14:52:06.000000 nechestniy_znak-1.0.2/src/nechestniy_znak/crpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-24 14:52:06.000000 nechestniy_znak-1.0.2/src/nechestniy_znak/egais.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:52:14.570920 nechestniy_znak-1.0.2/src/nechestniy_znak.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-24 14:52:14.000000 nechestniy_znak-1.0.2/src/nechestniy_znak.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-24 14:52:14.000000 nechestniy_znak-1.0.2/src/nechestniy_znak.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:52:14.000000 nechestniy_znak-1.0.2/src/nechestniy_znak.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 14:52:14.000000 nechestniy_znak-1.0.2/src/nechestniy_znak.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 14:52:14.000000 nechestniy_znak-1.0.2/src/nechestniy_znak.egg-info/top_level.txt
```

### Comparing `nechestniy_znak-1.0.1/LICENSE` & `nechestniy_znak-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nechestniy_znak-1.0.1/pyproject.toml` & `nechestniy_znak-1.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nechestniy_znak"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
     { name="li0ard", email="li0ard@proton.me" },
 ]
 maintainers = [
     {name = "li0ard", email = "li0ard@proton.me"}
 ]
 description = "Библеотека обертка для API ГИС МТ “Честный Знак”"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 4 - Beta",
-    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "requests",
 ]
```

### Comparing `nechestniy_znak-1.0.1/src/nechestniy_znak/lib.py` & `nechestniy_znak-1.0.2/src/nechestniy_znak/crpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 from typing import Union
 
 
-class Lib:
+class Crpt:
     def __init__(self):
         pass
 
     def _get(self, content: str, type: str) -> Union[list, dict]:
         return requests.get(f"https://mobile.api.crpt.ru/mobile/check?code={content}&codeType={type}").json()
 
     def _post(self, data: Union[dict, list]) -> Union[list, dict]:
```

