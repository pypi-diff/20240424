# Comparing `tmp/efinance-0.5.1.tar.gz` & `tmp/efinance-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efinance-0.5.1.tar", last modified: Sun Mar 24 12:05:55 2024, max compression
+gzip compressed data, was "efinance-0.5.2.tar", last modified: Wed Apr 24 12:40:11 2024, max compression
```

## Comparing `efinance-0.5.1.tar` & `efinance-0.5.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 sheep      (997) sheep      (997)        0 2024-03-24 12:05:55.079759 efinance-0.5.1/
--rw-rw-r--   0 sheep      (997) sheep      (997)     1068 2024-03-04 13:52:44.000000 efinance-0.5.1/LICENSE
--rw-r--r--   0 sheep      (997) sheep      (997)    41485 2024-03-24 12:05:55.079759 efinance-0.5.1/PKG-INFO
--rw-rw-r--   0 sheep      (997) sheep      (997)    40481 2024-03-04 13:52:44.000000 efinance-0.5.1/README.md
-drwxrwxr-x   0 sheep      (997) sheep      (997)        0 2024-03-24 12:05:54.995759 efinance-0.5.1/efinance/
--rw-rw-r--   0 sheep      (997) sheep      (997)      240 2024-03-04 13:52:44.000000 efinance-0.5.1/efinance/__init__.py
--rw-rw-r--   0 sheep      (997) sheep      (997)      457 2024-03-04 13:52:44.000000 efinance-0.5.1/efinance/__version__.py
-drwxrwxr-x   0 sheep      (997) sheep      (997)        0 2024-03-24 12:05:54.995759 efinance-0.5.1/efinance/api/
--rw-rw-r--   0 sheep      (997) sheep      (997)      124 2024-03-04 13:52:44.000000 efinance-0.5.1/efinance/api/__init__.py
-drwxrwxr-x   0 sheep      (997) sheep      (997)        0 2024-03-24 12:05:55.027759 efinance-0.5.1/efinance/bond/
--rw-rw-r--   0 sheep      (997) sheep      (997)      399 2024-03-04 13:52:44.000000 efinance-0.5.1/efinance/bond/__init__.py
--rw-rw-r--   0 sheep      (997) sheep      (997)      607 2024-03-04 13:52:44.000000 efinance-0.5.1/efinance/bond/config.py
--rw-rw-r--   0 sheep      (997) sheep      (997)    19125 2024-03-04 13:52:44.000000 efinance-0.5.1/efinance/bond/getter.py
-drwxrwxr-x   0 sheep      (997) sheep      (997)        0 2024-03-24 12:05:55.035759 efinance-0.5.1/efinance/common/
--rw-rw-r--   0 sheep      (997) sheep      (997)      196 2024-03-04 13:52:44.000000 efinance-0.5.1/efinance/common/__init__.py
--rw-rw-r--   0 sheep      (997) sheep      (997)     5131 2024-03-04 13:52:44.000000 efinance-0.5.1/efinance/common/config.py
--rw-rw-r--   0 sheep      (997) sheep      (997)    17341 2024-03-04 13:52:44.000000 efinance-0.5.1/efinance/common/getter.py
-drwxrwxr-x   0 sheep      (997) sheep      (997)        0 2024-03-24 12:05:55.035759 efinance-0.5.1/efinance/config/
--rw-rw-r--   0 sheep      (997) sheep      (997)      301 2024-03-04 13:52:44.000000 efinance-0.5.1/efinance/config/__init__.py
-drwxrwxr-x   0 sheep      (997) sheep      (997)        0 2024-03-24 12:05:55.043759 efinance-0.5.1/efinance/fund/
--rw-rw-r--   0 sheep      (997) sheep      (997)      649 2024-03-04 13:52:44.000000 efinance-0.5.1/efinance/fund/__init__.py
--rw-rw-r--   0 sheep      (997) sheep      (997)      937 2024-03-04 13:52:44.000000 efinance-0.5.1/efinance/fund/config.py
--rw-rw-r--   0 sheep      (997) sheep      (997)    30247 2024-03-04 13:52:44.000000 efinance-0.5.1/efinance/fund/getter.py
--rw-rw-r--   0 sheep      (997) sheep      (997)        0 2024-03-04 13:52:44.000000 efinance-0.5.1/efinance/fund/utils.py
-drwxrwxr-x   0 sheep      (997) sheep      (997)        0 2024-03-24 12:05:55.067759 efinance-0.5.1/efinance/futures/
--rw-rw-r--   0 sheep      (997) sheep      (997)      239 2024-03-04 13:52:44.000000 efinance-0.5.1/efinance/futures/__init__.py
--rw-rw-r--   0 sheep      (997) sheep      (997)      709 2024-03-04 13:52:44.000000 efinance-0.5.1/efinance/futures/config.py
--rw-rw-r--   0 sheep      (997) sheep      (997)    11117 2024-03-04 13:52:44.000000 efinance-0.5.1/efinance/futures/getter.py
--rw-rw-r--   0 sheep      (997) sheep      (997)        0 2024-03-04 13:52:44.000000 efinance-0.5.1/efinance/futures/utils.py
-drwxrwxr-x   0 sheep      (997) sheep      (997)        0 2024-03-24 12:05:55.067759 efinance-0.5.1/efinance/shared/
--rw-rw-r--   0 sheep      (997) sheep      (997)     1114 2024-03-04 13:52:44.000000 efinance-0.5.1/efinance/shared/__init__.py
-drwxrwxr-x   0 sheep      (997) sheep      (997)        0 2024-03-24 12:05:55.075759 efinance-0.5.1/efinance/stock/
--rw-rw-r--   0 sheep      (997) sheep      (997)      845 2024-03-04 13:52:44.000000 efinance-0.5.1/efinance/stock/__init__.py
--rw-rw-r--   0 sheep      (997) sheep      (997)     1125 2024-03-04 13:52:44.000000 efinance-0.5.1/efinance/stock/config.py
--rw-rw-r--   0 sheep      (997) sheep      (997)    76852 2024-03-04 13:52:44.000000 efinance-0.5.1/efinance/stock/getter.py
--rw-rw-r--   0 sheep      (997) sheep      (997)        0 2024-03-04 13:52:44.000000 efinance-0.5.1/efinance/stock/utils.py
-drwxrwxr-x   0 sheep      (997) sheep      (997)        0 2024-03-24 12:05:55.075759 efinance-0.5.1/efinance/utils/
--rw-rw-r--   0 sheep      (997) sheep      (997)    10599 2024-03-04 13:52:44.000000 efinance-0.5.1/efinance/utils/__init__.py
-drwxrwxr-x   0 sheep      (997) sheep      (997)        0 2024-03-24 12:05:55.075759 efinance-0.5.1/efinance.egg-info/
--rw-r--r--   0 sheep      (997) sheep      (997)    41485 2024-03-24 12:05:54.000000 efinance-0.5.1/efinance.egg-info/PKG-INFO
--rw-rw-r--   0 sheep      (997) sheep      (997)      799 2024-03-24 12:05:54.000000 efinance-0.5.1/efinance.egg-info/SOURCES.txt
--rw-rw-r--   0 sheep      (997) sheep      (997)        1 2024-03-24 12:05:54.000000 efinance-0.5.1/efinance.egg-info/dependency_links.txt
--rw-rw-r--   0 sheep      (997) sheep      (997)       54 2024-03-24 12:05:54.000000 efinance-0.5.1/efinance.egg-info/requires.txt
--rw-rw-r--   0 sheep      (997) sheep      (997)        9 2024-03-24 12:05:54.000000 efinance-0.5.1/efinance.egg-info/top_level.txt
--rw-rw-r--   0 sheep      (997) sheep      (997)       38 2024-03-24 12:05:55.079759 efinance-0.5.1/setup.cfg
--rw-rw-r--   0 sheep      (997) sheep      (997)     1258 2024-03-04 13:52:44.000000 efinance-0.5.1/setup.py
+drwxrwxr-x   0 sheep      (997) sheep      (997)        0 2024-04-24 12:40:11.919419 efinance-0.5.2/
+-rw-rw-r--   0 sheep      (997) sheep      (997)     1068 2024-03-04 13:52:44.000000 efinance-0.5.2/LICENSE
+-rw-r--r--   0 sheep      (997) sheep      (997)    41504 2024-04-24 12:40:11.919419 efinance-0.5.2/PKG-INFO
+-rw-rw-r--   0 sheep      (997) sheep      (997)    40481 2024-03-04 13:52:44.000000 efinance-0.5.2/README.md
+drwxrwxr-x   0 sheep      (997) sheep      (997)        0 2024-04-24 12:40:11.915419 efinance-0.5.2/efinance/
+-rw-rw-r--   0 sheep      (997) sheep      (997)      240 2024-03-04 13:52:44.000000 efinance-0.5.2/efinance/__init__.py
+-rw-rw-r--   0 sheep      (997) sheep      (997)      457 2024-04-24 12:37:41.000000 efinance-0.5.2/efinance/__version__.py
+drwxrwxr-x   0 sheep      (997) sheep      (997)        0 2024-04-24 12:40:11.915419 efinance-0.5.2/efinance/api/
+-rw-rw-r--   0 sheep      (997) sheep      (997)      124 2024-03-04 13:52:44.000000 efinance-0.5.2/efinance/api/__init__.py
+drwxrwxr-x   0 sheep      (997) sheep      (997)        0 2024-04-24 12:40:11.915419 efinance-0.5.2/efinance/bond/
+-rw-rw-r--   0 sheep      (997) sheep      (997)      399 2024-03-04 13:52:44.000000 efinance-0.5.2/efinance/bond/__init__.py
+-rw-rw-r--   0 sheep      (997) sheep      (997)      607 2024-03-04 13:52:44.000000 efinance-0.5.2/efinance/bond/config.py
+-rw-rw-r--   0 sheep      (997) sheep      (997)    19125 2024-03-04 13:52:44.000000 efinance-0.5.2/efinance/bond/getter.py
+drwxrwxr-x   0 sheep      (997) sheep      (997)        0 2024-04-24 12:40:11.915419 efinance-0.5.2/efinance/common/
+-rw-rw-r--   0 sheep      (997) sheep      (997)      196 2024-03-04 13:52:44.000000 efinance-0.5.2/efinance/common/__init__.py
+-rw-rw-r--   0 sheep      (997) sheep      (997)     5131 2024-03-04 13:52:44.000000 efinance-0.5.2/efinance/common/config.py
+-rw-rw-r--   0 sheep      (997) sheep      (997)    17341 2024-03-04 13:52:44.000000 efinance-0.5.2/efinance/common/getter.py
+drwxrwxr-x   0 sheep      (997) sheep      (997)        0 2024-04-24 12:40:11.915419 efinance-0.5.2/efinance/config/
+-rw-rw-r--   0 sheep      (997) sheep      (997)      301 2024-03-04 13:52:44.000000 efinance-0.5.2/efinance/config/__init__.py
+drwxrwxr-x   0 sheep      (997) sheep      (997)        0 2024-04-24 12:40:11.915419 efinance-0.5.2/efinance/fund/
+-rw-rw-r--   0 sheep      (997) sheep      (997)      649 2024-03-04 13:52:44.000000 efinance-0.5.2/efinance/fund/__init__.py
+-rw-rw-r--   0 sheep      (997) sheep      (997)      937 2024-03-04 13:52:44.000000 efinance-0.5.2/efinance/fund/config.py
+-rw-rw-r--   0 sheep      (997) sheep      (997)    30247 2024-03-04 13:52:44.000000 efinance-0.5.2/efinance/fund/getter.py
+-rw-rw-r--   0 sheep      (997) sheep      (997)        0 2024-03-04 13:52:44.000000 efinance-0.5.2/efinance/fund/utils.py
+drwxrwxr-x   0 sheep      (997) sheep      (997)        0 2024-04-24 12:40:11.919419 efinance-0.5.2/efinance/futures/
+-rw-rw-r--   0 sheep      (997) sheep      (997)      239 2024-03-04 13:52:44.000000 efinance-0.5.2/efinance/futures/__init__.py
+-rw-rw-r--   0 sheep      (997) sheep      (997)      709 2024-03-04 13:52:44.000000 efinance-0.5.2/efinance/futures/config.py
+-rw-rw-r--   0 sheep      (997) sheep      (997)    11117 2024-03-04 13:52:44.000000 efinance-0.5.2/efinance/futures/getter.py
+-rw-rw-r--   0 sheep      (997) sheep      (997)        0 2024-03-04 13:52:44.000000 efinance-0.5.2/efinance/futures/utils.py
+drwxrwxr-x   0 sheep      (997) sheep      (997)        0 2024-04-24 12:40:11.919419 efinance-0.5.2/efinance/shared/
+-rw-rw-r--   0 sheep      (997) sheep      (997)     1114 2024-03-04 13:52:44.000000 efinance-0.5.2/efinance/shared/__init__.py
+drwxrwxr-x   0 sheep      (997) sheep      (997)        0 2024-04-24 12:40:11.919419 efinance-0.5.2/efinance/stock/
+-rw-rw-r--   0 sheep      (997) sheep      (997)      845 2024-03-04 13:52:44.000000 efinance-0.5.2/efinance/stock/__init__.py
+-rw-rw-r--   0 sheep      (997) sheep      (997)     1125 2024-03-04 13:52:44.000000 efinance-0.5.2/efinance/stock/config.py
+-rw-rw-r--   0 sheep      (997) sheep      (997)    76852 2024-03-04 13:52:44.000000 efinance-0.5.2/efinance/stock/getter.py
+-rw-rw-r--   0 sheep      (997) sheep      (997)        0 2024-03-04 13:52:44.000000 efinance-0.5.2/efinance/stock/utils.py
+drwxrwxr-x   0 sheep      (997) sheep      (997)        0 2024-04-24 12:40:11.919419 efinance-0.5.2/efinance/utils/
+-rw-rw-r--   0 sheep      (997) sheep      (997)    10599 2024-03-04 13:52:44.000000 efinance-0.5.2/efinance/utils/__init__.py
+drwxrwxr-x   0 sheep      (997) sheep      (997)        0 2024-04-24 12:40:11.919419 efinance-0.5.2/efinance.egg-info/
+-rw-r--r--   0 sheep      (997) sheep      (997)    41504 2024-04-24 12:40:11.000000 efinance-0.5.2/efinance.egg-info/PKG-INFO
+-rw-rw-r--   0 sheep      (997) sheep      (997)      799 2024-04-24 12:40:11.000000 efinance-0.5.2/efinance.egg-info/SOURCES.txt
+-rw-rw-r--   0 sheep      (997) sheep      (997)        1 2024-04-24 12:40:11.000000 efinance-0.5.2/efinance.egg-info/dependency_links.txt
+-rw-rw-r--   0 sheep      (997) sheep      (997)       58 2024-04-24 12:40:11.000000 efinance-0.5.2/efinance.egg-info/requires.txt
+-rw-rw-r--   0 sheep      (997) sheep      (997)        9 2024-04-24 12:40:11.000000 efinance-0.5.2/efinance.egg-info/top_level.txt
+-rw-rw-r--   0 sheep      (997) sheep      (997)       38 2024-04-24 12:40:11.919419 efinance-0.5.2/setup.cfg
+-rw-rw-r--   0 sheep      (997) sheep      (997)     1265 2024-04-24 12:35:26.000000 efinance-0.5.2/setup.py
```

### Comparing `efinance-0.5.1/LICENSE` & `efinance-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `efinance-0.5.1/PKG-INFO` & `efinance-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efinance
-Version: 0.5.1
+Version: 0.5.2
 Summary: A finance tool to get stock,fund and futures data base on eastmoney
 Home-page: https://github.com/Micro-sheep/efinance
 Author: micro sheep
 Author-email: micro-sheep@outlook.com
 License: MIT
 Project-URL: Documentation, https://efinance.readthedocs.io
 Project-URL: Source, https://github.com/Micro-sheep/efinance
@@ -22,14 +22,15 @@
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: jsonpath
 Requires-Dist: pandas
 Requires-Dist: tqdm
 Requires-Dist: retry
 Requires-Dist: multitasking
+Requires-Dist: bs4
 
 ## Introduction
 
 [![Python Version](https://img.shields.io/badge/python-3.6+-blue.svg?style=flat)](https://pypi.python.org/pypi/efinance)
 [![Pypi Package](https://img.shields.io/pypi/v/efinance.svg?maxAge=60)](https://pypi.python.org/pypi/efinance)
 [![Pypi-Install](https://img.shields.io/pypi/dm/efinance.svg?maxAge=2592000&label=installs&color=%2327B1FF)](https://pypi.python.org/pypi/efinance)
 [![Docs](https://readthedocs.org/projects/efinance/badge/?version=latest)](https://efinance.readthedocs.io)
```

### Comparing `efinance-0.5.1/README.md` & `efinance-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `efinance-0.5.1/efinance/bond/config.py` & `efinance-0.5.2/efinance/bond/config.py`

 * *Files identical despite different names*

### Comparing `efinance-0.5.1/efinance/bond/getter.py` & `efinance-0.5.2/efinance/bond/getter.py`

 * *Files identical despite different names*

### Comparing `efinance-0.5.1/efinance/common/config.py` & `efinance-0.5.2/efinance/common/config.py`

 * *Files identical despite different names*

### Comparing `efinance-0.5.1/efinance/common/getter.py` & `efinance-0.5.2/efinance/common/getter.py`

 * *Files identical despite different names*

### Comparing `efinance-0.5.1/efinance/fund/__init__.py` & `efinance-0.5.2/efinance/fund/__init__.py`

 * *Files identical despite different names*

### Comparing `efinance-0.5.1/efinance/fund/config.py` & `efinance-0.5.2/efinance/fund/config.py`

 * *Files identical despite different names*

### Comparing `efinance-0.5.1/efinance/fund/getter.py` & `efinance-0.5.2/efinance/fund/getter.py`

 * *Files identical despite different names*

### Comparing `efinance-0.5.1/efinance/futures/config.py` & `efinance-0.5.2/efinance/futures/config.py`

 * *Files identical despite different names*

### Comparing `efinance-0.5.1/efinance/futures/getter.py` & `efinance-0.5.2/efinance/futures/getter.py`

 * *Files identical despite different names*

### Comparing `efinance-0.5.1/efinance/shared/__init__.py` & `efinance-0.5.2/efinance/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `efinance-0.5.1/efinance/stock/__init__.py` & `efinance-0.5.2/efinance/stock/__init__.py`

 * *Files identical despite different names*

### Comparing `efinance-0.5.1/efinance/stock/config.py` & `efinance-0.5.2/efinance/stock/config.py`

 * *Files identical despite different names*

### Comparing `efinance-0.5.1/efinance/stock/getter.py` & `efinance-0.5.2/efinance/stock/getter.py`

 * *Files identical despite different names*

### Comparing `efinance-0.5.1/efinance/utils/__init__.py` & `efinance-0.5.2/efinance/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `efinance-0.5.1/efinance.egg-info/PKG-INFO` & `efinance-0.5.2/efinance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efinance
-Version: 0.5.1
+Version: 0.5.2
 Summary: A finance tool to get stock,fund and futures data base on eastmoney
 Home-page: https://github.com/Micro-sheep/efinance
 Author: micro sheep
 Author-email: micro-sheep@outlook.com
 License: MIT
 Project-URL: Documentation, https://efinance.readthedocs.io
 Project-URL: Source, https://github.com/Micro-sheep/efinance
@@ -22,14 +22,15 @@
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: jsonpath
 Requires-Dist: pandas
 Requires-Dist: tqdm
 Requires-Dist: retry
 Requires-Dist: multitasking
+Requires-Dist: bs4
 
 ## Introduction
 
 [![Python Version](https://img.shields.io/badge/python-3.6+-blue.svg?style=flat)](https://pypi.python.org/pypi/efinance)
 [![Pypi Package](https://img.shields.io/pypi/v/efinance.svg?maxAge=60)](https://pypi.python.org/pypi/efinance)
 [![Pypi-Install](https://img.shields.io/pypi/dm/efinance.svg?maxAge=2592000&label=installs&color=%2327B1FF)](https://pypi.python.org/pypi/efinance)
 [![Docs](https://readthedocs.org/projects/efinance/badge/?version=latest)](https://efinance.readthedocs.io)
```

### Comparing `efinance-0.5.1/efinance.egg-info/SOURCES.txt` & `efinance-0.5.2/efinance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `efinance-0.5.1/setup.py` & `efinance-0.5.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 
 from setuptools import find_packages, setup
 
 here = pathlib.Path(__file__).parent
 # require = (here / "requirements.txt").read_text(encoding='utf-8').split()
-require = ['requests', 'rich', 'jsonpath', 'pandas', 'tqdm', 'retry', 'multitasking']
+require = ['requests', 'rich', 'jsonpath', 'pandas', 'tqdm', 'retry', 'multitasking', 'bs4']
 readme = (here / "README.md").read_text(encoding='utf-8')
 about = {}
 exec((here / 'efinance' / '__version__.py').read_text(encoding='utf-8'), about)
 setup(
     name=about['__title__'],
     version=about['__version__'],
     description=about['__description__'],
```

