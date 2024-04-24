# Comparing `tmp/botocore-a-la-carte-iotevents-1.34.89.tar.gz` & `tmp/botocore-a-la-carte-iotevents-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-iotevents-1.34.89.tar", last modified: Tue Apr 23 01:01:59 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-iotevents-1.34.9.tar", last modified: Thu Dec 28 01:06:43 2023, max compression
```

## Comparing `botocore-a-la-carte-iotevents-1.34.89.tar` & `botocore-a-la-carte-iotevents-1.34.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:01:59.805818 botocore-a-la-carte-iotevents-1.34.89/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-23 01:01:59.000000 botocore-a-la-carte-iotevents-1.34.89/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-23 01:01:59.805818 botocore-a-la-carte-iotevents-1.34.89/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:01:59.805818 botocore-a-la-carte-iotevents-1.34.89/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:01:59.805818 botocore-a-la-carte-iotevents-1.34.89/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:01:59.805818 botocore-a-la-carte-iotevents-1.34.89/botocore/data/iotevents/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:01:59.805818 botocore-a-la-carte-iotevents-1.34.89/botocore/data/iotevents/2018-07-27/
--rw-r--r--   0 runner    (1001) docker     (127)    13738 2024-04-23 01:01:45.000000 botocore-a-la-carte-iotevents-1.34.89/botocore/data/iotevents/2018-07-27/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 01:01:45.000000 botocore-a-la-carte-iotevents-1.34.89/botocore/data/iotevents/2018-07-27/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-23 01:01:45.000000 botocore-a-la-carte-iotevents-1.34.89/botocore/data/iotevents/2018-07-27/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   126424 2024-04-23 01:01:45.000000 botocore-a-la-carte-iotevents-1.34.89/botocore/data/iotevents/2018-07-27/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:01:59.805818 botocore-a-la-carte-iotevents-1.34.89/botocore_a_la_carte_iotevents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-23 01:01:59.000000 botocore-a-la-carte-iotevents-1.34.89/botocore_a_la_carte_iotevents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-23 01:01:59.000000 botocore-a-la-carte-iotevents-1.34.89/botocore_a_la_carte_iotevents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 01:01:59.000000 botocore-a-la-carte-iotevents-1.34.89/botocore_a_la_carte_iotevents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 01:01:59.000000 botocore-a-la-carte-iotevents-1.34.89/botocore_a_la_carte_iotevents.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 01:01:59.805818 botocore-a-la-carte-iotevents-1.34.89/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-23 01:01:59.000000 botocore-a-la-carte-iotevents-1.34.89/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:43.222290 botocore-a-la-carte-iotevents-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:42.000000 botocore-a-la-carte-iotevents-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2023-12-28 01:06:43.222290 botocore-a-la-carte-iotevents-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:43.218290 botocore-a-la-carte-iotevents-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:43.218290 botocore-a-la-carte-iotevents-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:43.218290 botocore-a-la-carte-iotevents-1.34.9/botocore/data/iotevents/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:43.218290 botocore-a-la-carte-iotevents-1.34.9/botocore/data/iotevents/2018-07-27/
+-rw-r--r--   0 runner    (1001) docker     (127)    13738 2023-12-28 01:06:26.000000 botocore-a-la-carte-iotevents-1.34.9/botocore/data/iotevents/2018-07-27/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-28 01:06:26.000000 botocore-a-la-carte-iotevents-1.34.9/botocore/data/iotevents/2018-07-27/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-28 01:06:26.000000 botocore-a-la-carte-iotevents-1.34.9/botocore/data/iotevents/2018-07-27/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   126421 2023-12-28 01:06:26.000000 botocore-a-la-carte-iotevents-1.34.9/botocore/data/iotevents/2018-07-27/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:43.222290 botocore-a-la-carte-iotevents-1.34.9/botocore_a_la_carte_iotevents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2023-12-28 01:06:43.000000 botocore-a-la-carte-iotevents-1.34.9/botocore_a_la_carte_iotevents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2023-12-28 01:06:43.000000 botocore-a-la-carte-iotevents-1.34.9/botocore_a_la_carte_iotevents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:43.000000 botocore-a-la-carte-iotevents-1.34.9/botocore_a_la_carte_iotevents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:43.000000 botocore-a-la-carte-iotevents-1.34.9/botocore_a_la_carte_iotevents.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:43.222290 botocore-a-la-carte-iotevents-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2023-12-28 01:06:42.000000 botocore-a-la-carte-iotevents-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-iotevents-1.34.89/LICENSE.txt` & `botocore-a-la-carte-iotevents-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-iotevents-1.34.89/PKG-INFO` & `botocore-a-la-carte-iotevents-1.34.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-iotevents
-Version: 1.34.89
+Version: 1.34.9
 Summary: iotevents data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-iotevents-1.34.89/botocore/data/iotevents/2018-07-27/endpoint-rule-set-1.json` & `botocore-a-la-carte-iotevents-1.34.9/botocore/data/iotevents/2018-07-27/endpoint-rule-set-1.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999991069387288%*

 * *Differences: {"'rules'": "{1: {'rules': {0: {'rules': {1: {'rules': {0: {'conditions': {0: {'argv': {insert: "*

 * *            "[(1, OrderedDict([('fn', 'getAttr'), ('argv', [OrderedDict([('ref', "*

 * *            "'PartitionResult')]), 'supportsFIPS'])]))], delete: [0]}}}}}}}}}}}"}*

```diff
@@ -198,24 +198,24 @@
                                 }
                             ],
                             "rules": [
                                 {
                                     "conditions": [
                                         {
                                             "argv": [
+                                                true,
                                                 {
                                                     "argv": [
                                                         {
                                                             "ref": "PartitionResult"
                                                         },
                                                         "supportsFIPS"
                                                     ],
                                                     "fn": "getAttr"
-                                                },
-                                                true
+                                                }
                                             ],
                                             "fn": "booleanEquals"
                                         }
                                     ],
                                     "rules": [
                                         {
                                             "conditions": [],
```

### Comparing `botocore-a-la-carte-iotevents-1.34.89/botocore/data/iotevents/2018-07-27/service-2.json` & `botocore-a-la-carte-iotevents-1.34.9/botocore/data/iotevents/2018-07-27/service-2.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998318385650224%*

 * *Differences: {"'shapes'": "{'AlarmModelDescription': {'max': 128}, 'DetectorModelDescription': {'max': 128}, "*

 * *             "'InputDescription': {'max': 128}}"}*

```diff
@@ -993,15 +993,15 @@
             },
             "type": "structure"
         },
         "AlarmModelArn": {
             "type": "string"
         },
         "AlarmModelDescription": {
-            "max": 1024,
+            "max": 128,
             "type": "string"
         },
         "AlarmModelName": {
             "max": 128,
             "min": 1,
             "pattern": "^[a-zA-Z0-9_-]+$",
             "type": "string"
@@ -1825,15 +1825,15 @@
             "required": [
                 "states",
                 "initialStateName"
             ],
             "type": "structure"
         },
         "DetectorModelDescription": {
-            "max": 1024,
+            "max": 128,
             "type": "string"
         },
         "DetectorModelName": {
             "max": 128,
             "min": 1,
             "pattern": "^[a-zA-Z0-9_-]+$",
             "type": "string"
@@ -2249,15 +2249,15 @@
             },
             "required": [
                 "attributes"
             ],
             "type": "structure"
         },
         "InputDescription": {
-            "max": 1024,
+            "max": 128,
             "type": "string"
         },
         "InputIdentifier": {
             "documentation": "<p> The identifer of the input. </p>",
             "members": {
                 "iotEventsInputIdentifier": {
                     "documentation": "<p> The identifier of the input routed to AWS IoT Events. </p>",
```

### Comparing `botocore-a-la-carte-iotevents-1.34.89/botocore_a_la_carte_iotevents.egg-info/PKG-INFO` & `botocore-a-la-carte-iotevents-1.34.9/botocore_a_la_carte_iotevents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-iotevents
-Version: 1.34.89
+Version: 1.34.9
 Summary: iotevents data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-iotevents-1.34.89/setup.py` & `botocore-a-la-carte-iotevents-1.34.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-iotevents',
-    version="1.34.89",
+    version="1.34.9",
     description='iotevents data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/iotevents/*/*.json'],
```

