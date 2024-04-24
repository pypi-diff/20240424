# Comparing `tmp/fiftyone_pipeline_core-4.4.8.0.tar.gz` & `tmp/fiftyone_pipeline_core-4.4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiftyone_pipeline_core-4.4.8.0.tar", last modified: Sun Jul  2 01:56:21 2023, max compression
+gzip compressed data, was "fiftyone_pipeline_core-4.4.9.0.tar", last modified: Fri Jul 14 01:53:27 2023, max compression
```

## Comparing `fiftyone_pipeline_core-4.4.8.0.tar` & `fiftyone_pipeline_core-4.4.9.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:21.366800 fiftyone_pipeline_core-4.4.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-02 01:56:21.366800 fiftyone_pipeline_core-4.4.8.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:21.366800 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/
--rw-r--r--   0 runner    (1001) docker     (123)    16980 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/JavaScriptResource.mustache
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/aspectproperty_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/basiclist_evidence_keyfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/elementdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/elementdata_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/evidence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/evidence_keyfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/flowdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/flowelement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/flowerror.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/javascriptbuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/jsonbundler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/pipelinebuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/sequenceelement.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/setheaderelement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 01:56:21.366800 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-02 01:56:21.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-02 01:56:21.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 01:56:21.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-02 01:56:21.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-02 01:56:21.000000 fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 01:56:21.366800 fiftyone_pipeline_core-4.4.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-07-02 01:56:16.000000 fiftyone_pipeline_core-4.4.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:53:27.698662 fiftyone_pipeline_core-4.4.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-14 01:53:20.000000 fiftyone_pipeline_core-4.4.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-14 01:53:27.698662 fiftyone_pipeline_core-4.4.9.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:53:27.698662 fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/
+-rw-r--r--   0 runner    (1001) docker     (123)    16980 2023-07-14 01:53:20.000000 fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/JavaScriptResource.mustache
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:53:20.000000 fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-14 01:53:20.000000 fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/aspectproperty_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-14 01:53:20.000000 fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/basiclist_evidence_keyfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-14 01:53:20.000000 fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/elementdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-14 01:53:20.000000 fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/elementdata_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-14 01:53:20.000000 fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/evidence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-14 01:53:20.000000 fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/evidence_keyfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-07-14 01:53:20.000000 fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/flowdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-07-14 01:53:20.000000 fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/flowelement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-14 01:53:20.000000 fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/flowerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-07-14 01:53:20.000000 fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/javascriptbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-07-14 01:53:20.000000 fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/jsonbundler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-14 01:53:20.000000 fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-14 01:53:20.000000 fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-07-14 01:53:20.000000 fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-07-14 01:53:20.000000 fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/pipelinebuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-14 01:53:20.000000 fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/sequenceelement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-07-14 01:53:20.000000 fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/setheaderelement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-14 01:53:20.000000 fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 01:53:27.698662 fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-14 01:53:27.000000 fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-14 01:53:27.000000 fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 01:53:27.000000 fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-14 01:53:27.000000 fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 01:53:27.000000 fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 01:53:27.698662 fiftyone_pipeline_core-4.4.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-07-14 01:53:20.000000 fiftyone_pipeline_core-4.4.9.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 01:53:27.000000 fiftyone_pipeline_core-4.4.9.0/version.txt
```

### Comparing `fiftyone_pipeline_core-4.4.8.0/PKG-INFO` & `fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fiftyone_pipeline_core
-Version: 4.4.8.0
+Name: fiftyone-pipeline-core
+Version: 4.4.9.0
 Summary: The 51Degrees Pipeline API is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines). This package definds the essential components of the Pipeline API such as flow elements, flow data and evidence. It also packages together JavaScript served by a pipeline and allows for client side requests for additional data populated by evidence from the client side.
 Home-page: https://51degrees.com/
 Author: 51Degrees
 Author-email: support@51degrees.com
 License: EUPL-1.2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/JavaScriptResource.mustache` & `fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/JavaScriptResource.mustache`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/aspectproperty_value.py` & `fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/aspectproperty_value.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/basiclist_evidence_keyfilter.py` & `fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/basiclist_evidence_keyfilter.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/elementdata.py` & `fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/elementdata.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/elementdata_dictionary.py` & `fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/elementdata_dictionary.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/evidence.py` & `fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/evidence.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/evidence_keyfilter.py` & `fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/evidence_keyfilter.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/flowdata.py` & `fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/flowdata.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/flowelement.py` & `fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/flowelement.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/flowerror.py` & `fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/flowerror.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/javascriptbuilder.py` & `fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/javascriptbuilder.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/jsonbundler.py` & `fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/jsonbundler.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/logger.py` & `fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/logger.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/messages.py` & `fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/messages.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/pipeline.py` & `fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/pipeline.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/pipelinebuilder.py` & `fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/pipelinebuilder.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/sequenceelement.py` & `fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/sequenceelement.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/setheaderelement.py` & `fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/setheaderelement.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core/web.py` & `fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core/web.py`

 * *Files identical despite different names*

### Comparing `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core.egg-info/PKG-INFO` & `fiftyone_pipeline_core-4.4.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fiftyone-pipeline-core
-Version: 4.4.8.0
+Name: fiftyone_pipeline_core
+Version: 4.4.9.0
 Summary: The 51Degrees Pipeline API is a generic web request intelligence and data processing solution with the ability to add a range of 51Degrees and/or custom plug ins (Engines). This package definds the essential components of the Pipeline API such as flow elements, flow data and evidence. It also packages together JavaScript served by a pipeline and allows for client side requests for additional data populated by evidence from the client side.
 Home-page: https://51degrees.com/
 Author: 51Degrees
 Author-email: support@51degrees.com
 License: EUPL-1.2
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fiftyone_pipeline_core-4.4.8.0/fiftyone_pipeline_core.egg-info/SOURCES.txt` & `fiftyone_pipeline_core-4.4.9.0/fiftyone_pipeline_core.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 MANIFEST.in
 setup.py
+version.txt
 fiftyone_pipeline_core/JavaScriptResource.mustache
 fiftyone_pipeline_core/__init__.py
 fiftyone_pipeline_core/aspectproperty_value.py
 fiftyone_pipeline_core/basiclist_evidence_keyfilter.py
 fiftyone_pipeline_core/elementdata.py
 fiftyone_pipeline_core/elementdata_dictionary.py
 fiftyone_pipeline_core/evidence.py
```

### Comparing `fiftyone_pipeline_core-4.4.8.0/setup.py` & `fiftyone_pipeline_core-4.4.9.0/setup.py`

 * *Files identical despite different names*

