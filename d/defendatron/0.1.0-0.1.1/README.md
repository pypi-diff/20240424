# Comparing `tmp/defendatron-0.1.0.tar.gz` & `tmp/defendatron-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defendatron-0.1.0.tar", last modified: Wed Apr 24 01:26:36 2024, max compression
+gzip compressed data, was "defendatron-0.1.1.tar", last modified: Wed Apr 24 02:16:10 2024, max compression
```

## Comparing `defendatron-0.1.0.tar` & `defendatron-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:26:36.901012 defendatron-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-24 01:26:36.901012 defendatron-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-24 01:26:31.000000 defendatron-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 01:26:36.901012 defendatron-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-24 01:26:31.000000 defendatron-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:26:36.897012 defendatron-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:26:36.901012 defendatron-0.1.0/src/defendatron/
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-24 01:26:31.000000 defendatron-0.1.0/src/defendatron/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:26:36.901012 defendatron-0.1.0/src/defendatron.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-24 01:26:36.000000 defendatron-0.1.0/src/defendatron.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-24 01:26:36.000000 defendatron-0.1.0/src/defendatron.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-24 01:26:36.000000 defendatron-0.1.0/src/defendatron.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 01:26:36.000000 defendatron-0.1.0/src/defendatron.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:16:10.158920 defendatron-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-24 02:16:10.158920 defendatron-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-24 02:16:05.000000 defendatron-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 02:16:10.158920 defendatron-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-24 02:16:05.000000 defendatron-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:16:10.154920 defendatron-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:16:10.154920 defendatron-0.1.1/src/defendatron/
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-24 02:16:05.000000 defendatron-0.1.1/src/defendatron/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:16:10.158920 defendatron-0.1.1/src/defendatron.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-24 02:16:10.000000 defendatron-0.1.1/src/defendatron.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-24 02:16:10.000000 defendatron-0.1.1/src/defendatron.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:16:10.000000 defendatron-0.1.1/src/defendatron.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-24 02:16:10.000000 defendatron-0.1.1/src/defendatron.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 02:16:10.000000 defendatron-0.1.1/src/defendatron.egg-info/top_level.txt
```

### Comparing `defendatron-0.1.0/PKG-INFO` & `defendatron-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,17 @@
-Metadata-Version: 2.1
-Name: defendatron
-Version: 0.1.0
-Home-page: https://github.com/Capsize-Games/defendatron
-Author: Capsize LLC
-Author-email: contact@capsizegames.com
-License: GPL-3.0
-Requires-Python: >=3.10.0
-Description-Content-Type: text/markdown
-
 # Defendatron
 
 Defendatron is a simple coordinator for `Protectbots`, Python modules that provide security features for your applications.
 
-
 ---
 
 ![img_1.png](img.png)
 
+[![Upload Python Package](https://github.com/Capsize-Games/defendatron/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Capsize-Games/defendatron/actions/workflows/python-publish.yml)
+
 ---
 
 ## Installation
 
 ```bash
 pip install defendatron
 ```
@@ -35,29 +26,29 @@
 
 # Deactivate defendatron (all protectbots)
 defendatron.deactivate()
 
 # Activate specific protectbots
 defendatron.nullscream.activate()
 defendatron.shadowlogger.activate()
-defendatron.lockdown.activate()
+defendatron.darklock.activate()
 
 # Deactivate specific protectbots
 defendatron.nullscream.deactivate()
 defendatron.shadowlogger.deactivate()
-defendatron.lockdown.deactivate()
+defendatron.darklock.deactivate()
 ```
 
 See `src/defendatron/__init__.py` for more advanced usage.
 
 ## When Protecbots assemble, they create DEFENDATRON
 ![img_2.png](img_1.png)
 
 ---
 
 Defendatron is built with `Protectbots`, Python modules that provide security features for your applications. 
 Each `Protectbot` is designed to defend against specific threats and vulnerabilities, 
 helping to provide another layer of protection for your code. 
 
 - [NULLSCREAM](https://github.com/Capsize-Games/nullscream) Responsible for masquerading as other libraries in order to cancel out their operations. Useful when you are unable to modify the code of a library that you are using, but you want to prevent it from performing certain operations.
-- [LOCKDOWN](https://github.com/Capsize-Games/lockdown) Responsible for locking down your application and preventing it from performing certain operations.
+- [DARKLOCK](https://github.com/Capsize-Games/darklock) Responsible for locking down your application and preventing it from performing certain operations.
 - [SHADOWLOGGER](https://github.com/Capsize-Games/shadowlogger) Intercepts all logs and shadows them, preventing sensitive information from being leaked.
```

### Comparing `defendatron-0.1.0/setup.py` & `defendatron-0.1.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name="defendatron",
-    version="0.1.0",
+    version="0.1.1",
     author="Capsize LLC",
     description="",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="",
     license="GPL-3.0",
     author_email="contact@capsizegames.com",
     url="https://github.com/Capsize-Games/defendatron",
     package_dir={"": "src"},
     packages=find_packages("src"),
     python_requires=">=3.10.0",
     install_requires=[
-    ],
-    dependency_links=[
         "nullscream==0.1.0",
-        "lockdown==0.1.0",
+        "darklock==0.1.0",
         "shadowlogger==0.1.0",
     ],
+    dependency_links=[
+    ],
 )
```

### Comparing `defendatron-0.1.0/src/defendatron.egg-info/PKG-INFO` & `defendatron-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: defendatron
-Version: 0.1.0
+Version: 0.1.1
 Home-page: https://github.com/Capsize-Games/defendatron
 Author: Capsize LLC
 Author-email: contact@capsizegames.com
 License: GPL-3.0
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
+Requires-Dist: nullscream==0.1.0
+Requires-Dist: darklock==0.1.0
+Requires-Dist: shadowlogger==0.1.0
 
 # Defendatron
 
 Defendatron is a simple coordinator for `Protectbots`, Python modules that provide security features for your applications.
 
-
 ---
 
 ![img_1.png](img.png)
 
+[![Upload Python Package](https://github.com/Capsize-Games/defendatron/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Capsize-Games/defendatron/actions/workflows/python-publish.yml)
+
 ---
 
 ## Installation
 
 ```bash
 pip install defendatron
 ```
@@ -35,29 +39,29 @@
 
 # Deactivate defendatron (all protectbots)
 defendatron.deactivate()
 
 # Activate specific protectbots
 defendatron.nullscream.activate()
 defendatron.shadowlogger.activate()
-defendatron.lockdown.activate()
+defendatron.darklock.activate()
 
 # Deactivate specific protectbots
 defendatron.nullscream.deactivate()
 defendatron.shadowlogger.deactivate()
-defendatron.lockdown.deactivate()
+defendatron.darklock.deactivate()
 ```
 
 See `src/defendatron/__init__.py` for more advanced usage.
 
 ## When Protecbots assemble, they create DEFENDATRON
 ![img_2.png](img_1.png)
 
 ---
 
 Defendatron is built with `Protectbots`, Python modules that provide security features for your applications. 
 Each `Protectbot` is designed to defend against specific threats and vulnerabilities, 
 helping to provide another layer of protection for your code. 
 
 - [NULLSCREAM](https://github.com/Capsize-Games/nullscream) Responsible for masquerading as other libraries in order to cancel out their operations. Useful when you are unable to modify the code of a library that you are using, but you want to prevent it from performing certain operations.
-- [LOCKDOWN](https://github.com/Capsize-Games/lockdown) Responsible for locking down your application and preventing it from performing certain operations.
+- [DARKLOCK](https://github.com/Capsize-Games/darklock) Responsible for locking down your application and preventing it from performing certain operations.
 - [SHADOWLOGGER](https://github.com/Capsize-Games/shadowlogger) Intercepts all logs and shadows them, preventing sensitive information from being leaked.
```

