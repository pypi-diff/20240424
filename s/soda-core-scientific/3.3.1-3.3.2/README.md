# Comparing `tmp/soda-core-scientific-3.3.1.tar.gz` & `tmp/soda_core_scientific-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-scientific-3.3.1.tar", last modified: Sun Mar 24 04:29:32 2024, max compression
+gzip compressed data, was "soda_core_scientific-3.3.2.tar", last modified: Wed Apr 24 15:26:32 2024, max compression
```

## Comparing `soda-core-scientific-3.3.1.tar` & `soda_core_scientific-3.3.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:32.813356 soda-core-scientific-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-24 04:29:32.813356 soda-core-scientific-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 04:29:32.813356 soda-core-scientific-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:32.809356 soda-core-scientific-3.3.1/soda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:32.809356 soda-core-scientific-3.3.1/soda/scientific/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:32.809356 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection/
--rw-r--r--   0 runner    (1001) docker     (127)     9902 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection/anomaly_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection/detector_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection/feedback_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:32.809356 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21073 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection/models/prophet_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:32.813356 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/
--rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/anomaly_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/detector_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10904 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/feedback_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7819 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/frequency_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:32.813356 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    19919 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/models/prophet_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/pydantic_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:32.813356 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/simulate/
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/simulate/anomaly_detection_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11697 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/simulate/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:32.813356 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/simulate/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/simulate/assets/SODA.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/simulate/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/simulate/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/simulate/pydantic_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/simulate/visualisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:32.813356 soda-core-scientific-3.3.1/soda/scientific/common/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/soda/scientific/common/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:32.813356 soda-core-scientific-3.3.1/soda/scientific/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)    15870 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/soda/scientific/distribution/comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/soda/scientific/distribution/generate_dro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-03-24 04:28:40.000000 soda-core-scientific-3.3.1/soda/scientific/distribution/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 04:29:32.813356 soda-core-scientific-3.3.1/soda_core_scientific.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-24 04:29:32.000000 soda-core-scientific-3.3.1/soda_core_scientific.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-03-24 04:29:32.000000 soda-core-scientific-3.3.1/soda_core_scientific.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 04:29:32.000000 soda-core-scientific-3.3.1/soda_core_scientific.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-24 04:29:32.000000 soda-core-scientific-3.3.1/soda_core_scientific.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-24 04:29:32.000000 soda-core-scientific-3.3.1/soda_core_scientific.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:32.559829 soda_core_scientific-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-24 15:26:32.559829 soda_core_scientific-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:26:32.559829 soda_core_scientific-3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:32.551829 soda_core_scientific-3.3.2/soda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:32.551829 soda_core_scientific-3.3.2/soda/scientific/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:32.551829 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)     9902 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection/anomaly_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection/detector_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection/feedback_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:32.555829 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21073 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection/models/prophet_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:32.555829 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     7965 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/anomaly_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/detector_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10904 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/feedback_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7819 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/frequency_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:32.555829 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19919 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/models/prophet_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/pydantic_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:32.555829 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/simulate/
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/simulate/anomaly_detection_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11697 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/simulate/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:32.555829 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/simulate/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/simulate/assets/SODA.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/simulate/assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/simulate/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/simulate/pydantic_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/simulate/visualisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:32.555829 soda_core_scientific-3.3.2/soda/scientific/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/soda/scientific/common/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:32.555829 soda_core_scientific-3.3.2/soda/scientific/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)    15870 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/soda/scientific/distribution/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/soda/scientific/distribution/generate_dro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-24 15:25:40.000000 soda_core_scientific-3.3.2/soda/scientific/distribution/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:26:32.559829 soda_core_scientific-3.3.2/soda_core_scientific.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-24 15:26:32.000000 soda_core_scientific-3.3.2/soda_core_scientific.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-24 15:26:32.000000 soda_core_scientific-3.3.2/soda_core_scientific.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:26:32.000000 soda_core_scientific-3.3.2/soda_core_scientific.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-24 15:26:32.000000 soda_core_scientific-3.3.2/soda_core_scientific.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 15:26:32.000000 soda_core_scientific-3.3.2/soda_core_scientific.egg-info/top_level.txt
```

### Comparing `soda-core-scientific-3.3.1/LICENSE` & `soda_core_scientific-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.3.1/PKG-INFO` & `soda_core_scientific-3.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: soda-core-scientific
-Version: 3.3.1
+Version: 3.3.2
 License-File: LICENSE
-Requires-Dist: soda-core==3.3.1
+Requires-Dist: soda-core==3.3.2
 Requires-Dist: pandas<2.0.0
 Requires-Dist: wheel
 Requires-Dist: pydantic<3.0.0,>=2.0.0
 Requires-Dist: scipy>=1.8.0
 Requires-Dist: numpy<2.0.0,>=1.23.3
 Requires-Dist: inflection==0.5.1
 Requires-Dist: httpx<2.0.0,>=0.18.1
```

### Comparing `soda-core-scientific-3.3.1/setup.py` & `soda_core_scientific-3.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import find_namespace_packages, setup
 
 package_name = "soda-core-scientific"
-package_version = "3.3.1"
+package_version = "3.3.2"
 description = "Soda Core Scientific Package"
 requires = [
     f"soda-core=={package_version}",
     "pandas<2.0.0",
     "wheel",
     "pydantic>=2.0.0, <3.0.0",
     "scipy>=1.8.0",
```

### Comparing `soda-core-scientific-3.3.1/soda/scientific/anomaly_detection/anomaly_detector.py` & `soda_core_scientific-3.3.2/soda/scientific/anomaly_detection/anomaly_detector.py`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.3.1/soda/scientific/anomaly_detection/detector_config.yaml` & `soda_core_scientific-3.3.2/soda/scientific/anomaly_detection/detector_config.yaml`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.3.1/soda/scientific/anomaly_detection/feedback_processor.py` & `soda_core_scientific-3.3.2/soda/scientific/anomaly_detection/feedback_processor.py`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.3.1/soda/scientific/anomaly_detection/models/base.py` & `soda_core_scientific-3.3.2/soda/scientific/anomaly_detection/models/base.py`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.3.1/soda/scientific/anomaly_detection/models/prophet_model.py` & `soda_core_scientific-3.3.2/soda/scientific/anomaly_detection/models/prophet_model.py`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/anomaly_detector.py` & `soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/anomaly_detector.py`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/detector_config.yaml` & `soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/detector_config.yaml`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/exceptions.py` & `soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/exceptions.py`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/feedback_processor.py` & `soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/feedback_processor.py`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/frequency_detector.py` & `soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/frequency_detector.py`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/globals.py` & `soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/globals.py`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/models/base.py` & `soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/models/base.py`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/models/prophet_model.py` & `soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/models/prophet_model.py`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/pydantic_models.py` & `soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/simulate/anomaly_detection_dataset.py` & `soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/simulate/anomaly_detection_dataset.py`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/simulate/app.py` & `soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/simulate/app.py`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/simulate/assets/SODA.svg` & `soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/simulate/assets/SODA.svg`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/simulate/assets/favicon.ico` & `soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/simulate/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/simulate/pydantic_models.py` & `soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/simulate/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/simulate/visualisation.py` & `soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/simulate/visualisation.py`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.3.1/soda/scientific/anomaly_detection_v2/utils.py` & `soda_core_scientific-3.3.2/soda/scientific/anomaly_detection_v2/utils.py`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.3.1/soda/scientific/distribution/comparison.py` & `soda_core_scientific-3.3.2/soda/scientific/distribution/comparison.py`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.3.1/soda/scientific/distribution/generate_dro.py` & `soda_core_scientific-3.3.2/soda/scientific/distribution/generate_dro.py`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.3.1/soda/scientific/distribution/utils.py` & `soda_core_scientific-3.3.2/soda/scientific/distribution/utils.py`

 * *Files identical despite different names*

### Comparing `soda-core-scientific-3.3.1/soda_core_scientific.egg-info/PKG-INFO` & `soda_core_scientific-3.3.2/soda_core_scientific.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: soda-core-scientific
-Version: 3.3.1
+Version: 3.3.2
 License-File: LICENSE
-Requires-Dist: soda-core==3.3.1
+Requires-Dist: soda-core==3.3.2
 Requires-Dist: pandas<2.0.0
 Requires-Dist: wheel
 Requires-Dist: pydantic<3.0.0,>=2.0.0
 Requires-Dist: scipy>=1.8.0
 Requires-Dist: numpy<2.0.0,>=1.23.3
 Requires-Dist: inflection==0.5.1
 Requires-Dist: httpx<2.0.0,>=0.18.1
```

### Comparing `soda-core-scientific-3.3.1/soda_core_scientific.egg-info/SOURCES.txt` & `soda_core_scientific-3.3.2/soda_core_scientific.egg-info/SOURCES.txt`

 * *Files identical despite different names*

