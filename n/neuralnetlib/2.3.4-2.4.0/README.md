# Comparing `tmp/neuralnetlib-2.3.4.tar.gz` & `tmp/neuralnetlib-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralnetlib-2.3.4.tar", last modified: Wed Apr 24 02:54:07 2024, max compression
+gzip compressed data, was "neuralnetlib-2.4.0.tar", last modified: Wed Apr 24 02:56:02 2024, max compression
```

## Comparing `neuralnetlib-2.3.4.tar` & `neuralnetlib-2.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:54:07.648475 neuralnetlib-2.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 02:53:55.000000 neuralnetlib-2.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-24 02:54:07.648475 neuralnetlib-2.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-24 02:53:55.000000 neuralnetlib-2.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:54:07.648475 neuralnetlib-2.3.4/neuralnetlib/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-24 02:53:55.000000 neuralnetlib-2.3.4/neuralnetlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-24 02:53:55.000000 neuralnetlib-2.3.4/neuralnetlib/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-24 02:53:55.000000 neuralnetlib-2.3.4/neuralnetlib/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    42004 2024-04-24 02:53:55.000000 neuralnetlib-2.3.4/neuralnetlib/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-24 02:53:55.000000 neuralnetlib-2.3.4/neuralnetlib/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-24 02:53:55.000000 neuralnetlib-2.3.4/neuralnetlib/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-04-24 02:53:55.000000 neuralnetlib-2.3.4/neuralnetlib/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7261 2024-04-24 02:53:55.000000 neuralnetlib-2.3.4/neuralnetlib/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-04-24 02:53:55.000000 neuralnetlib-2.3.4/neuralnetlib/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-24 02:53:55.000000 neuralnetlib-2.3.4/neuralnetlib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:54:07.648475 neuralnetlib-2.3.4/neuralnetlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-24 02:54:07.000000 neuralnetlib-2.3.4/neuralnetlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-24 02:54:07.000000 neuralnetlib-2.3.4/neuralnetlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:54:07.000000 neuralnetlib-2.3.4/neuralnetlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 02:54:07.000000 neuralnetlib-2.3.4/neuralnetlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 02:54:07.000000 neuralnetlib-2.3.4/neuralnetlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 02:54:07.648475 neuralnetlib-2.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 02:53:55.000000 neuralnetlib-2.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:56:02.487735 neuralnetlib-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 02:55:51.000000 neuralnetlib-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-24 02:56:02.487735 neuralnetlib-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-24 02:55:51.000000 neuralnetlib-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:56:02.487735 neuralnetlib-2.4.0/neuralnetlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-24 02:55:51.000000 neuralnetlib-2.4.0/neuralnetlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-24 02:55:51.000000 neuralnetlib-2.4.0/neuralnetlib/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-24 02:55:51.000000 neuralnetlib-2.4.0/neuralnetlib/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42004 2024-04-24 02:55:51.000000 neuralnetlib-2.4.0/neuralnetlib/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-24 02:55:51.000000 neuralnetlib-2.4.0/neuralnetlib/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-24 02:55:51.000000 neuralnetlib-2.4.0/neuralnetlib/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9681 2024-04-24 02:55:51.000000 neuralnetlib-2.4.0/neuralnetlib/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7261 2024-04-24 02:55:51.000000 neuralnetlib-2.4.0/neuralnetlib/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-04-24 02:55:51.000000 neuralnetlib-2.4.0/neuralnetlib/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-24 02:55:51.000000 neuralnetlib-2.4.0/neuralnetlib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:56:02.487735 neuralnetlib-2.4.0/neuralnetlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-24 02:56:02.000000 neuralnetlib-2.4.0/neuralnetlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-24 02:56:02.000000 neuralnetlib-2.4.0/neuralnetlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:56:02.000000 neuralnetlib-2.4.0/neuralnetlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 02:56:02.000000 neuralnetlib-2.4.0/neuralnetlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 02:56:02.000000 neuralnetlib-2.4.0/neuralnetlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 02:56:02.487735 neuralnetlib-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 02:55:51.000000 neuralnetlib-2.4.0/setup.py
```

### Comparing `neuralnetlib-2.3.4/LICENSE` & `neuralnetlib-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.4/PKG-INFO` & `neuralnetlib-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralnetlib
-Version: 2.3.4
+Version: 2.4.0
 Summary: A simple convolutional neural network library with only numpy as dependency
 Home-page: https://github.com/marcpinet/handmade-neuralnetwork
 Author: Marc Pinet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `neuralnetlib-2.3.4/README.md` & `neuralnetlib-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.4/neuralnetlib/activations.py` & `neuralnetlib-2.4.0/neuralnetlib/activations.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.4/neuralnetlib/callbacks.py` & `neuralnetlib-2.4.0/neuralnetlib/callbacks.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.4/neuralnetlib/layers.py` & `neuralnetlib-2.4.0/neuralnetlib/layers.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.4/neuralnetlib/losses.py` & `neuralnetlib-2.4.0/neuralnetlib/losses.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.4/neuralnetlib/metrics.py` & `neuralnetlib-2.4.0/neuralnetlib/metrics.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.4/neuralnetlib/model.py` & `neuralnetlib-2.4.0/neuralnetlib/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
                 for callback in callbacks:
                     if callback.stop_training:
                         break
                     if callback.on_epoch_end(self, metrics_values):
                         break
                     
                 if any(callback.stop_training for callback in callbacks):
-                                break
+                    break
 
             if verbose:
                 print()
 
         if verbose:
             print()
```

### Comparing `neuralnetlib-2.3.4/neuralnetlib/optimizers.py` & `neuralnetlib-2.4.0/neuralnetlib/optimizers.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.4/neuralnetlib/preprocessing.py` & `neuralnetlib-2.4.0/neuralnetlib/preprocessing.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.4/neuralnetlib/utils.py` & `neuralnetlib-2.4.0/neuralnetlib/utils.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.4/neuralnetlib.egg-info/PKG-INFO` & `neuralnetlib-2.4.0/neuralnetlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralnetlib
-Version: 2.3.4
+Version: 2.4.0
 Summary: A simple convolutional neural network library with only numpy as dependency
 Home-page: https://github.com/marcpinet/handmade-neuralnetwork
 Author: Marc Pinet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `neuralnetlib-2.3.4/setup.py` & `neuralnetlib-2.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='neuralnetlib',
-    version='2.3.4',
+    version='2.4.0',
     author='Marc Pinet',
     description='A simple convolutional neural network library with only numpy as dependency',
     long_description=open('README.md', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     url='https://github.com/marcpinet/handmade-neuralnetwork',
     packages=find_packages(),
     install_requires=[
```

