# Comparing `tmp/litdata-0.2.4.tar.gz` & `tmp/litdata-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litdata-0.2.4.tar", last modified: Wed Apr 24 16:14:16 2024, max compression
+gzip compressed data, was "litdata-0.2.5.tar", last modified: Wed Apr 24 16:31:13 2024, max compression
```

## Comparing `litdata-0.2.4.tar` & `litdata-0.2.5.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:14:16.085019 litdata-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-24 16:14:06.000000 litdata-0.2.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-04-24 16:14:06.000000 litdata-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-24 16:14:06.000000 litdata-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20638 2024-04-24 16:14:16.085019 litdata-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18917 2024-04-24 16:14:06.000000 litdata-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-24 16:14:06.000000 litdata-0.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 16:14:16.085019 litdata-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-24 16:14:06.000000 litdata-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:14:16.077019 litdata-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:14:16.081019 litdata-0.2.4/src/litdata/
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/imports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:14:16.081019 litdata-0.2.4/src/litdata/processing/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42470 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/processing/data_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    17078 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/processing/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/processing/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/processing/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:14:16.085019 litdata-0.2.4/src/litdata/streaming/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/combined.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/compression.py
--rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    25796 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8731 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/item_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    12365 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     9749 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    14520 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/shuffle.py
--rw-r--r--   0 runner    (1001) docker     (127)    17993 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/streaming/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:14:16.085019 litdata-0.2.4/src/litdata/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52973 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/utilities/_pytree.py
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/utilities/broadcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/utilities/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/utilities/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/utilities/packing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-24 16:14:06.000000 litdata-0.2.4/src/litdata/utilities/shuffle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:14:16.085019 litdata-0.2.4/src/litdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20638 2024-04-24 16:14:16.000000 litdata-0.2.4/src/litdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-24 16:14:16.000000 litdata-0.2.4/src/litdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:14:16.000000 litdata-0.2.4/src/litdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:14:16.000000 litdata-0.2.4/src/litdata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-24 16:14:16.000000 litdata-0.2.4/src/litdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 16:14:16.000000 litdata-0.2.4/src/litdata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:31:13.262665 litdata-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-24 16:31:03.000000 litdata-0.2.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-04-24 16:31:03.000000 litdata-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-24 16:31:03.000000 litdata-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    20631 2024-04-24 16:31:13.262665 litdata-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18917 2024-04-24 16:31:03.000000 litdata-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-24 16:31:03.000000 litdata-0.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 16:31:13.262665 litdata-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-24 16:31:03.000000 litdata-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:31:13.250665 litdata-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:31:13.254665 litdata-0.2.5/src/litdata/
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/imports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:31:13.254665 litdata-0.2.5/src/litdata/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42470 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/processing/data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17078 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/processing/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/processing/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/processing/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:31:13.258665 litdata-0.2.5/src/litdata/streaming/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/streaming/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/streaming/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/streaming/combined.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/streaming/compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/streaming/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25796 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/streaming/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/streaming/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/streaming/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8731 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/streaming/item_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/streaming/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12365 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/streaming/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9749 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/streaming/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14520 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/streaming/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/streaming/shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17993 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/streaming/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:31:13.258665 litdata-0.2.5/src/litdata/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52973 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/utilities/_pytree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/utilities/broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/utilities/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/utilities/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/utilities/packing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-24 16:31:03.000000 litdata-0.2.5/src/litdata/utilities/shuffle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:31:13.258665 litdata-0.2.5/src/litdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20631 2024-04-24 16:31:13.000000 litdata-0.2.5/src/litdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-24 16:31:13.000000 litdata-0.2.5/src/litdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:31:13.000000 litdata-0.2.5/src/litdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:31:13.000000 litdata-0.2.5/src/litdata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-24 16:31:13.000000 litdata-0.2.5/src/litdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 16:31:13.000000 litdata-0.2.5/src/litdata.egg-info/top_level.txt
```

### Comparing `litdata-0.2.4/LICENSE` & `litdata-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/MANIFEST.in` & `litdata-0.2.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/PKG-INFO` & `litdata-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litdata
-Version: 0.2.4
+Version: 0.2.5
 Summary: The Deep Learning framework to train, deploy, and ship AI products Lightning fast.
 Home-page: https://github.com/Lightning-AI/lit-data
 Download-URL: https://github.com/Lightning-AI/litdata
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/litdata/issues
@@ -22,21 +22,21 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: torch>=2.1.0
+Requires-Dist: torch
 Requires-Dist: filelock
 Requires-Dist: numpy
 Requires-Dist: boto3[crt]
 Requires-Dist: requests
 Provides-Extra: extras
-Requires-Dist: lightning-cloud==0.5.65; extra == "extras"
+Requires-Dist: lightning-cloud==0.5.68; extra == "extras"
 Requires-Dist: pillow; extra == "extras"
 Requires-Dist: pyarrow; extra == "extras"
 Requires-Dist: torchvision; extra == "extras"
 Requires-Dist: tqdm; extra == "extras"
 Requires-Dist: viztracer; extra == "extras"
 
 <div align="center">
```

### Comparing `litdata-0.2.4/README.md` & `litdata-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/setup.py` & `litdata-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/__about__.py` & `litdata-0.2.5/src/litdata/__about__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import time
 
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 __author__ = "Lightning AI et al."
 __author_email__ = "pytorch@lightning.ai"
 __license__ = "Apache-2.0"
 __copyright__ = f"Copyright (c) 2023-{time.strftime('%Y')}, {__author__}."
 __homepage__ = "https://github.com/Lightning-AI/lit-data"
 __docs_url__ = "https://lightning.ai/docs/pytorch/stable/"
 # this has to be simple string, see: https://github.com/pypa/twine/issues/522
```

### Comparing `litdata-0.2.4/src/litdata/__init__.py` & `litdata-0.2.5/src/litdata/__init__.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/constants.py` & `litdata-0.2.5/src/litdata/constants.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/imports.py` & `litdata-0.2.5/src/litdata/imports.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/processing/__init__.py` & `litdata-0.2.5/src/litdata/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/processing/data_processor.py` & `litdata-0.2.5/src/litdata/processing/data_processor.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/processing/functions.py` & `litdata-0.2.5/src/litdata/processing/functions.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/processing/readers.py` & `litdata-0.2.5/src/litdata/processing/readers.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/processing/utilities.py` & `litdata-0.2.5/src/litdata/processing/utilities.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/streaming/__init__.py` & `litdata-0.2.5/src/litdata/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/streaming/cache.py` & `litdata-0.2.5/src/litdata/streaming/cache.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/streaming/client.py` & `litdata-0.2.5/src/litdata/streaming/client.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/streaming/combined.py` & `litdata-0.2.5/src/litdata/streaming/combined.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/streaming/compression.py` & `litdata-0.2.5/src/litdata/streaming/compression.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/streaming/config.py` & `litdata-0.2.5/src/litdata/streaming/config.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/streaming/dataloader.py` & `litdata-0.2.5/src/litdata/streaming/dataloader.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/streaming/dataset.py` & `litdata-0.2.5/src/litdata/streaming/dataset.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/streaming/downloader.py` & `litdata-0.2.5/src/litdata/streaming/downloader.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/streaming/item_loader.py` & `litdata-0.2.5/src/litdata/streaming/item_loader.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/streaming/reader.py` & `litdata-0.2.5/src/litdata/streaming/reader.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/streaming/resolver.py` & `litdata-0.2.5/src/litdata/streaming/resolver.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/streaming/sampler.py` & `litdata-0.2.5/src/litdata/streaming/sampler.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/streaming/serializers.py` & `litdata-0.2.5/src/litdata/streaming/serializers.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/streaming/shuffle.py` & `litdata-0.2.5/src/litdata/streaming/shuffle.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/streaming/writer.py` & `litdata-0.2.5/src/litdata/streaming/writer.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/utilities/__init__.py` & `litdata-0.2.5/src/litdata/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/utilities/_pytree.py` & `litdata-0.2.5/src/litdata/utilities/_pytree.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/utilities/broadcast.py` & `litdata-0.2.5/src/litdata/utilities/broadcast.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/utilities/env.py` & `litdata-0.2.5/src/litdata/utilities/env.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/utilities/format.py` & `litdata-0.2.5/src/litdata/utilities/format.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/utilities/packing.py` & `litdata-0.2.5/src/litdata/utilities/packing.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata/utilities/shuffle.py` & `litdata-0.2.5/src/litdata/utilities/shuffle.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.4/src/litdata.egg-info/PKG-INFO` & `litdata-0.2.5/src/litdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litdata
-Version: 0.2.4
+Version: 0.2.5
 Summary: The Deep Learning framework to train, deploy, and ship AI products Lightning fast.
 Home-page: https://github.com/Lightning-AI/lit-data
 Download-URL: https://github.com/Lightning-AI/litdata
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/litdata/issues
@@ -22,21 +22,21 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: torch>=2.1.0
+Requires-Dist: torch
 Requires-Dist: filelock
 Requires-Dist: numpy
 Requires-Dist: boto3[crt]
 Requires-Dist: requests
 Provides-Extra: extras
-Requires-Dist: lightning-cloud==0.5.65; extra == "extras"
+Requires-Dist: lightning-cloud==0.5.68; extra == "extras"
 Requires-Dist: pillow; extra == "extras"
 Requires-Dist: pyarrow; extra == "extras"
 Requires-Dist: torchvision; extra == "extras"
 Requires-Dist: tqdm; extra == "extras"
 Requires-Dist: viztracer; extra == "extras"
 
 <div align="center">
```

### Comparing `litdata-0.2.4/src/litdata.egg-info/SOURCES.txt` & `litdata-0.2.5/src/litdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

