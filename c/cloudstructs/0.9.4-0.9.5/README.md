# Comparing `tmp/cloudstructs-0.9.4.tar.gz` & `tmp/cloudstructs-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudstructs-0.9.4.tar", last modified: Thu Apr  4 14:19:38 2024, max compression
+gzip compressed data, was "cloudstructs-0.9.5.tar", last modified: Wed Apr 24 08:52:57 2024, max compression
```

## Comparing `cloudstructs-0.9.4.tar` & `cloudstructs-0.9.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:19:38.373109 cloudstructs-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-04 14:19:26.000000 cloudstructs-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-04 14:19:26.000000 cloudstructs-0.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-04 14:19:38.373109 cloudstructs-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-04 14:19:26.000000 cloudstructs-0.9.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-04 14:19:26.000000 cloudstructs-0.9.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 14:19:38.373109 cloudstructs-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-04 14:19:26.000000 cloudstructs-0.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:19:38.369109 cloudstructs-0.9.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:19:38.369109 cloudstructs-0.9.4/src/cloudstructs/
--rw-r--r--   0 runner    (1001) docker     (127)   184196 2024-04-04 14:19:26.000000 cloudstructs-0.9.4/src/cloudstructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:19:38.369109 cloudstructs-0.9.4/src/cloudstructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-04 14:19:26.000000 cloudstructs-0.9.4/src/cloudstructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  3235913 2024-04-04 14:19:26.000000 cloudstructs-0.9.4/src/cloudstructs/_jsii/cloudstructs@0.9.4.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:19:26.000000 cloudstructs-0.9.4/src/cloudstructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:19:38.369109 cloudstructs-0.9.4/src/cloudstructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-04 14:19:38.000000 cloudstructs-0.9.4/src/cloudstructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-04 14:19:38.000000 cloudstructs-0.9.4/src/cloudstructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:19:38.000000 cloudstructs-0.9.4/src/cloudstructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-04 14:19:38.000000 cloudstructs-0.9.4/src/cloudstructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-04 14:19:38.000000 cloudstructs-0.9.4/src/cloudstructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:52:57.896037 cloudstructs-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-24 08:52:39.000000 cloudstructs-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-24 08:52:39.000000 cloudstructs-0.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-24 08:52:57.896037 cloudstructs-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-24 08:52:39.000000 cloudstructs-0.9.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-24 08:52:39.000000 cloudstructs-0.9.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 08:52:57.896037 cloudstructs-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-24 08:52:39.000000 cloudstructs-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:52:57.888037 cloudstructs-0.9.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:52:57.892037 cloudstructs-0.9.5/src/cloudstructs/
+-rw-r--r--   0 runner    (1001) docker     (127)   184196 2024-04-24 08:52:39.000000 cloudstructs-0.9.5/src/cloudstructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:52:57.892037 cloudstructs-0.9.5/src/cloudstructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-24 08:52:39.000000 cloudstructs-0.9.5/src/cloudstructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  3242102 2024-04-24 08:52:39.000000 cloudstructs-0.9.5/src/cloudstructs/_jsii/cloudstructs@0.9.5.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:52:39.000000 cloudstructs-0.9.5/src/cloudstructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:52:57.892037 cloudstructs-0.9.5/src/cloudstructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-24 08:52:57.000000 cloudstructs-0.9.5/src/cloudstructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-24 08:52:57.000000 cloudstructs-0.9.5/src/cloudstructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:52:57.000000 cloudstructs-0.9.5/src/cloudstructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-24 08:52:57.000000 cloudstructs-0.9.5/src/cloudstructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 08:52:57.000000 cloudstructs-0.9.5/src/cloudstructs.egg-info/top_level.txt
```

### Comparing `cloudstructs-0.9.4/LICENSE` & `cloudstructs-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudstructs-0.9.4/PKG-INFO` & `cloudstructs-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudstructs
-Version: 0.9.4
+Version: 0.9.5
 Summary: High-level constructs for AWS CDK
 Home-page: https://github.com/jogold/cloudstructs.git
 Author: Jonathan Goldwasser<jonathan.goldwasser@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/jogold/cloudstructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudstructs-0.9.4/README.md` & `cloudstructs-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `cloudstructs-0.9.4/setup.py` & `cloudstructs-0.9.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudstructs",
-    "version": "0.9.4",
+    "version": "0.9.5",
     "description": "High-level constructs for AWS CDK",
     "license": "Apache-2.0",
     "url": "https://github.com/jogold/cloudstructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Jonathan Goldwasser<jonathan.goldwasser@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cloudstructs",
         "cloudstructs._jsii"
     ],
     "package_data": {
         "cloudstructs._jsii": [
-            "cloudstructs@0.9.4.jsii.tgz"
+            "cloudstructs@0.9.5.jsii.tgz"
         ],
         "cloudstructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.133.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.96.0, <2.0.0",
+        "jsii>=1.97.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cloudstructs-0.9.4/src/cloudstructs/__init__.py` & `cloudstructs-0.9.5/src/cloudstructs/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudstructs-0.9.4/src/cloudstructs.egg-info/PKG-INFO` & `cloudstructs-0.9.5/src/cloudstructs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudstructs
-Version: 0.9.4
+Version: 0.9.5
 Summary: High-level constructs for AWS CDK
 Home-page: https://github.com/jogold/cloudstructs.git
 Author: Jonathan Goldwasser<jonathan.goldwasser@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/jogold/cloudstructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

