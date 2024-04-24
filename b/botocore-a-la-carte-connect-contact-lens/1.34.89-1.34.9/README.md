# Comparing `tmp/botocore-a-la-carte-connect-contact-lens-1.34.89.tar.gz` & `tmp/botocore-a-la-carte-connect-contact-lens-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-connect-contact-lens-1.34.89.tar", last modified: Tue Apr 23 01:01:53 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-connect-contact-lens-1.34.9.tar", last modified: Thu Dec 28 01:06:37 2023, max compression
```

## Comparing `botocore-a-la-carte-connect-contact-lens-1.34.89.tar` & `botocore-a-la-carte-connect-contact-lens-1.34.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:01:53.849852 botocore-a-la-carte-connect-contact-lens-1.34.89/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-23 01:01:53.000000 botocore-a-la-carte-connect-contact-lens-1.34.89/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-23 01:01:53.849852 botocore-a-la-carte-connect-contact-lens-1.34.89/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:01:53.849852 botocore-a-la-carte-connect-contact-lens-1.34.89/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:01:53.849852 botocore-a-la-carte-connect-contact-lens-1.34.89/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:01:53.849852 botocore-a-la-carte-connect-contact-lens-1.34.89/botocore/data/connect-contact-lens/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:01:53.849852 botocore-a-la-carte-connect-contact-lens-1.34.89/botocore/data/connect-contact-lens/2020-08-21/
--rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-04-23 01:01:45.000000 botocore-a-la-carte-connect-contact-lens-1.34.89/botocore/data/connect-contact-lens/2020-08-21/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 01:01:45.000000 botocore-a-la-carte-connect-contact-lens-1.34.89/botocore/data/connect-contact-lens/2020-08-21/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-23 01:01:45.000000 botocore-a-la-carte-connect-contact-lens-1.34.89/botocore/data/connect-contact-lens/2020-08-21/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    11742 2024-04-23 01:01:45.000000 botocore-a-la-carte-connect-contact-lens-1.34.89/botocore/data/connect-contact-lens/2020-08-21/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:01:53.849852 botocore-a-la-carte-connect-contact-lens-1.34.89/botocore_a_la_carte_connect_contact_lens.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-23 01:01:53.000000 botocore-a-la-carte-connect-contact-lens-1.34.89/botocore_a_la_carte_connect_contact_lens.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-23 01:01:53.000000 botocore-a-la-carte-connect-contact-lens-1.34.89/botocore_a_la_carte_connect_contact_lens.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 01:01:53.000000 botocore-a-la-carte-connect-contact-lens-1.34.89/botocore_a_la_carte_connect_contact_lens.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 01:01:53.000000 botocore-a-la-carte-connect-contact-lens-1.34.89/botocore_a_la_carte_connect_contact_lens.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 01:01:53.849852 botocore-a-la-carte-connect-contact-lens-1.34.89/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-23 01:01:53.000000 botocore-a-la-carte-connect-contact-lens-1.34.89/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:37.902249 botocore-a-la-carte-connect-contact-lens-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:37.000000 botocore-a-la-carte-connect-contact-lens-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2023-12-28 01:06:37.902249 botocore-a-la-carte-connect-contact-lens-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:37.902249 botocore-a-la-carte-connect-contact-lens-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:37.902249 botocore-a-la-carte-connect-contact-lens-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:37.902249 botocore-a-la-carte-connect-contact-lens-1.34.9/botocore/data/connect-contact-lens/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:37.902249 botocore-a-la-carte-connect-contact-lens-1.34.9/botocore/data/connect-contact-lens/2020-08-21/
+-rw-r--r--   0 runner    (1001) docker     (127)    13750 2023-12-28 01:06:26.000000 botocore-a-la-carte-connect-contact-lens-1.34.9/botocore/data/connect-contact-lens/2020-08-21/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-28 01:06:26.000000 botocore-a-la-carte-connect-contact-lens-1.34.9/botocore/data/connect-contact-lens/2020-08-21/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-28 01:06:26.000000 botocore-a-la-carte-connect-contact-lens-1.34.9/botocore/data/connect-contact-lens/2020-08-21/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11742 2023-12-28 01:06:26.000000 botocore-a-la-carte-connect-contact-lens-1.34.9/botocore/data/connect-contact-lens/2020-08-21/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:37.902249 botocore-a-la-carte-connect-contact-lens-1.34.9/botocore_a_la_carte_connect_contact_lens.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2023-12-28 01:06:37.000000 botocore-a-la-carte-connect-contact-lens-1.34.9/botocore_a_la_carte_connect_contact_lens.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2023-12-28 01:06:37.000000 botocore-a-la-carte-connect-contact-lens-1.34.9/botocore_a_la_carte_connect_contact_lens.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:37.000000 botocore-a-la-carte-connect-contact-lens-1.34.9/botocore_a_la_carte_connect_contact_lens.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:37.000000 botocore-a-la-carte-connect-contact-lens-1.34.9/botocore_a_la_carte_connect_contact_lens.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:37.902249 botocore-a-la-carte-connect-contact-lens-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2023-12-28 01:06:37.000000 botocore-a-la-carte-connect-contact-lens-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-connect-contact-lens-1.34.89/LICENSE.txt` & `botocore-a-la-carte-connect-contact-lens-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-connect-contact-lens-1.34.89/PKG-INFO` & `botocore-a-la-carte-connect-contact-lens-1.34.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-connect-contact-lens
-Version: 1.34.89
+Version: 1.34.9
 Summary: connect-contact-lens data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-connect-contact-lens-1.34.89/botocore/data/connect-contact-lens/2020-08-21/endpoint-rule-set-1.json` & `botocore-a-la-carte-connect-contact-lens-1.34.9/botocore/data/connect-contact-lens/2020-08-21/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-connect-contact-lens-1.34.89/botocore/data/connect-contact-lens/2020-08-21/service-2.json` & `botocore-a-la-carte-connect-contact-lens-1.34.9/botocore/data/connect-contact-lens/2020-08-21/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-connect-contact-lens-1.34.89/botocore_a_la_carte_connect_contact_lens.egg-info/PKG-INFO` & `botocore-a-la-carte-connect-contact-lens-1.34.9/botocore_a_la_carte_connect_contact_lens.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-connect-contact-lens
-Version: 1.34.89
+Version: 1.34.9
 Summary: connect-contact-lens data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-connect-contact-lens-1.34.89/botocore_a_la_carte_connect_contact_lens.egg-info/SOURCES.txt` & `botocore-a-la-carte-connect-contact-lens-1.34.9/botocore_a_la_carte_connect_contact_lens.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-connect-contact-lens-1.34.89/setup.py` & `botocore-a-la-carte-connect-contact-lens-1.34.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-connect-contact-lens',
-    version="1.34.89",
+    version="1.34.9",
     description='connect-contact-lens data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/connect-contact-lens/*/*.json'],
```

