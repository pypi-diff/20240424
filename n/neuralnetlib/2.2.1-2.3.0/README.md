# Comparing `tmp/neuralnetlib-2.2.1.tar.gz` & `tmp/neuralnetlib-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralnetlib-2.2.1.tar", last modified: Sun Apr 21 14:20:38 2024, max compression
+gzip compressed data, was "neuralnetlib-2.3.0.tar", last modified: Wed Apr 24 00:56:17 2024, max compression
```

## Comparing `neuralnetlib-2.2.1.tar` & `neuralnetlib-2.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:20:38.959592 neuralnetlib-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-21 14:20:29.000000 neuralnetlib-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-21 14:20:38.959592 neuralnetlib-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-21 14:20:29.000000 neuralnetlib-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:20:38.955592 neuralnetlib-2.2.1/neuralnetlib/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-21 14:20:29.000000 neuralnetlib-2.2.1/neuralnetlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-21 14:20:29.000000 neuralnetlib-2.2.1/neuralnetlib/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)    18200 2024-04-21 14:20:29.000000 neuralnetlib-2.2.1/neuralnetlib/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-21 14:20:29.000000 neuralnetlib-2.2.1/neuralnetlib/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-21 14:20:29.000000 neuralnetlib-2.2.1/neuralnetlib/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7839 2024-04-21 14:20:29.000000 neuralnetlib-2.2.1/neuralnetlib/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7261 2024-04-21 14:20:29.000000 neuralnetlib-2.2.1/neuralnetlib/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-04-21 14:20:29.000000 neuralnetlib-2.2.1/neuralnetlib/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-21 14:20:29.000000 neuralnetlib-2.2.1/neuralnetlib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 14:20:38.959592 neuralnetlib-2.2.1/neuralnetlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-21 14:20:38.000000 neuralnetlib-2.2.1/neuralnetlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-21 14:20:38.000000 neuralnetlib-2.2.1/neuralnetlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 14:20:38.000000 neuralnetlib-2.2.1/neuralnetlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-21 14:20:38.000000 neuralnetlib-2.2.1/neuralnetlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-21 14:20:38.000000 neuralnetlib-2.2.1/neuralnetlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-21 14:20:38.959592 neuralnetlib-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-21 14:20:29.000000 neuralnetlib-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:56:17.175221 neuralnetlib-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 00:55:56.000000 neuralnetlib-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-24 00:56:17.175221 neuralnetlib-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-24 00:55:56.000000 neuralnetlib-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:56:17.175221 neuralnetlib-2.3.0/neuralnetlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-24 00:55:56.000000 neuralnetlib-2.3.0/neuralnetlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-24 00:55:56.000000 neuralnetlib-2.3.0/neuralnetlib/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33635 2024-04-24 00:55:56.000000 neuralnetlib-2.3.0/neuralnetlib/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-24 00:55:56.000000 neuralnetlib-2.3.0/neuralnetlib/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-24 00:55:56.000000 neuralnetlib-2.3.0/neuralnetlib/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10663 2024-04-24 00:55:56.000000 neuralnetlib-2.3.0/neuralnetlib/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7261 2024-04-24 00:55:56.000000 neuralnetlib-2.3.0/neuralnetlib/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-04-24 00:55:56.000000 neuralnetlib-2.3.0/neuralnetlib/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-24 00:55:56.000000 neuralnetlib-2.3.0/neuralnetlib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:56:17.175221 neuralnetlib-2.3.0/neuralnetlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-24 00:56:16.000000 neuralnetlib-2.3.0/neuralnetlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-24 00:56:17.000000 neuralnetlib-2.3.0/neuralnetlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 00:56:16.000000 neuralnetlib-2.3.0/neuralnetlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 00:56:16.000000 neuralnetlib-2.3.0/neuralnetlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 00:56:16.000000 neuralnetlib-2.3.0/neuralnetlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 00:56:17.175221 neuralnetlib-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 00:55:56.000000 neuralnetlib-2.3.0/setup.py
```

### Comparing `neuralnetlib-2.2.1/LICENSE` & `neuralnetlib-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.2.1/PKG-INFO` & `neuralnetlib-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralnetlib
-Version: 2.2.1
+Version: 2.3.0
 Summary: A simple convolutional neural network library with only numpy as dependency
 Home-page: https://github.com/marcpinet/handmade-neuralnetwork
 Author: Marc Pinet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `neuralnetlib-2.2.1/README.md` & `neuralnetlib-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.2.1/neuralnetlib/activations.py` & `neuralnetlib-2.3.0/neuralnetlib/activations.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.2.1/neuralnetlib/losses.py` & `neuralnetlib-2.3.0/neuralnetlib/losses.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.2.1/neuralnetlib/metrics.py` & `neuralnetlib-2.3.0/neuralnetlib/metrics.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.2.1/neuralnetlib/optimizers.py` & `neuralnetlib-2.3.0/neuralnetlib/optimizers.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.2.1/neuralnetlib/utils.py` & `neuralnetlib-2.3.0/neuralnetlib/utils.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.2.1/neuralnetlib.egg-info/PKG-INFO` & `neuralnetlib-2.3.0/neuralnetlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralnetlib
-Version: 2.2.1
+Version: 2.3.0
 Summary: A simple convolutional neural network library with only numpy as dependency
 Home-page: https://github.com/marcpinet/handmade-neuralnetwork
 Author: Marc Pinet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `neuralnetlib-2.2.1/setup.py` & `neuralnetlib-2.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='neuralnetlib',
-    version='2.2.1',
+    version='2.3.0',
     author='Marc Pinet',
     description='A simple convolutional neural network library with only numpy as dependency',
     long_description=open('README.md', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     url='https://github.com/marcpinet/handmade-neuralnetwork',
     packages=find_packages(),
     install_requires=[
```

