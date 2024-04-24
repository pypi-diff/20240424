# Comparing `tmp/neuralnetlib-2.3.1.tar.gz` & `tmp/neuralnetlib-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralnetlib-2.3.1.tar", last modified: Wed Apr 24 01:14:28 2024, max compression
+gzip compressed data, was "neuralnetlib-2.3.2.tar", last modified: Wed Apr 24 01:23:52 2024, max compression
```

## Comparing `neuralnetlib-2.3.1.tar` & `neuralnetlib-2.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:14:28.779139 neuralnetlib-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 01:14:15.000000 neuralnetlib-2.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-24 01:14:28.779139 neuralnetlib-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-24 01:14:15.000000 neuralnetlib-2.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:14:28.779139 neuralnetlib-2.3.1/neuralnetlib/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-24 01:14:15.000000 neuralnetlib-2.3.1/neuralnetlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-24 01:14:15.000000 neuralnetlib-2.3.1/neuralnetlib/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)    40301 2024-04-24 01:14:15.000000 neuralnetlib-2.3.1/neuralnetlib/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-24 01:14:15.000000 neuralnetlib-2.3.1/neuralnetlib/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-24 01:14:15.000000 neuralnetlib-2.3.1/neuralnetlib/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-04-24 01:14:15.000000 neuralnetlib-2.3.1/neuralnetlib/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7261 2024-04-24 01:14:15.000000 neuralnetlib-2.3.1/neuralnetlib/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-04-24 01:14:15.000000 neuralnetlib-2.3.1/neuralnetlib/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-24 01:14:15.000000 neuralnetlib-2.3.1/neuralnetlib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:14:28.779139 neuralnetlib-2.3.1/neuralnetlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-24 01:14:28.000000 neuralnetlib-2.3.1/neuralnetlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-24 01:14:28.000000 neuralnetlib-2.3.1/neuralnetlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 01:14:28.000000 neuralnetlib-2.3.1/neuralnetlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 01:14:28.000000 neuralnetlib-2.3.1/neuralnetlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 01:14:28.000000 neuralnetlib-2.3.1/neuralnetlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 01:14:28.779139 neuralnetlib-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 01:14:15.000000 neuralnetlib-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:23:52.241866 neuralnetlib-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 01:23:41.000000 neuralnetlib-2.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-24 01:23:52.241866 neuralnetlib-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-24 01:23:41.000000 neuralnetlib-2.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:23:52.241866 neuralnetlib-2.3.2/neuralnetlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-24 01:23:41.000000 neuralnetlib-2.3.2/neuralnetlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-24 01:23:41.000000 neuralnetlib-2.3.2/neuralnetlib/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41351 2024-04-24 01:23:41.000000 neuralnetlib-2.3.2/neuralnetlib/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-24 01:23:41.000000 neuralnetlib-2.3.2/neuralnetlib/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-24 01:23:41.000000 neuralnetlib-2.3.2/neuralnetlib/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-04-24 01:23:41.000000 neuralnetlib-2.3.2/neuralnetlib/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7261 2024-04-24 01:23:41.000000 neuralnetlib-2.3.2/neuralnetlib/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-04-24 01:23:41.000000 neuralnetlib-2.3.2/neuralnetlib/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-24 01:23:41.000000 neuralnetlib-2.3.2/neuralnetlib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:23:52.241866 neuralnetlib-2.3.2/neuralnetlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-24 01:23:52.000000 neuralnetlib-2.3.2/neuralnetlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-24 01:23:52.000000 neuralnetlib-2.3.2/neuralnetlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 01:23:52.000000 neuralnetlib-2.3.2/neuralnetlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 01:23:52.000000 neuralnetlib-2.3.2/neuralnetlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 01:23:52.000000 neuralnetlib-2.3.2/neuralnetlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 01:23:52.241866 neuralnetlib-2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 01:23:41.000000 neuralnetlib-2.3.2/setup.py
```

### Comparing `neuralnetlib-2.3.1/LICENSE` & `neuralnetlib-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.1/PKG-INFO` & `neuralnetlib-2.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralnetlib
-Version: 2.3.1
+Version: 2.3.2
 Summary: A simple convolutional neural network library with only numpy as dependency
 Home-page: https://github.com/marcpinet/handmade-neuralnetwork
 Author: Marc Pinet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `neuralnetlib-2.3.1/README.md` & `neuralnetlib-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.1/neuralnetlib/activations.py` & `neuralnetlib-2.3.2/neuralnetlib/activations.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.1/neuralnetlib/layers.py` & `neuralnetlib-2.3.2/neuralnetlib/layers.py`

 * *Files 6% similar despite different names*

```diff
@@ -959,7 +959,27 @@
         for i in range(out_steps):
             d_input[:, i * stride:i * stride + pool_size, :] += output_error[:, i, :][:, np.newaxis, :] / pool_size
 
         if padding == 'same':
             d_input = d_input[:, pad_steps:-pad_steps, :]
 
         return d_input
+    
+
+# --------------------------------------------------------------------------------------------------------------
+
+
+compatibility_dict = {
+    Input: [Dense, Conv2D, Conv1D, Embedding],
+    Dense: [Dense, Activation, Dropout, BatchNormalization],
+    Activation: [Dense, Conv2D, Conv1D, MaxPooling2D, AveragePooling2D, MaxPooling1D, AveragePooling1D, Flatten, Dropout],
+    Conv2D: [Conv2D, MaxPooling2D, AveragePooling2D, Activation, Dropout, Flatten, BatchNormalization],
+    MaxPooling2D: [Conv2D, MaxPooling2D, AveragePooling2D, Flatten],
+    AveragePooling2D: [Conv2D, MaxPooling2D, AveragePooling2D, Flatten],
+    Conv1D: [Conv1D, MaxPooling1D, AveragePooling1D, Activation, Dropout, Flatten, BatchNormalization],
+    MaxPooling1D: [Conv1D, MaxPooling1D, AveragePooling1D, Flatten],
+    AveragePooling1D: [Conv1D, MaxPooling1D, AveragePooling1D, Flatten],
+    Flatten: [Dense, Dropout],
+    Dropout: [Dense, Conv2D, Conv1D, Activation],
+    Embedding: [Conv1D, Flatten, Dense],
+    BatchNormalization: [Dense, Conv2D, Conv1D, Activation]
+}
```

### Comparing `neuralnetlib-2.3.1/neuralnetlib/losses.py` & `neuralnetlib-2.3.2/neuralnetlib/losses.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.1/neuralnetlib/metrics.py` & `neuralnetlib-2.3.2/neuralnetlib/metrics.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.1/neuralnetlib/optimizers.py` & `neuralnetlib-2.3.2/neuralnetlib/optimizers.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.1/neuralnetlib/preprocessing.py` & `neuralnetlib-2.3.2/neuralnetlib/preprocessing.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.1/neuralnetlib/utils.py` & `neuralnetlib-2.3.2/neuralnetlib/utils.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.1/neuralnetlib.egg-info/PKG-INFO` & `neuralnetlib-2.3.2/neuralnetlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralnetlib
-Version: 2.3.1
+Version: 2.3.2
 Summary: A simple convolutional neural network library with only numpy as dependency
 Home-page: https://github.com/marcpinet/handmade-neuralnetwork
 Author: Marc Pinet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `neuralnetlib-2.3.1/setup.py` & `neuralnetlib-2.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='neuralnetlib',
-    version='2.3.1',
+    version='2.3.2',
     author='Marc Pinet',
     description='A simple convolutional neural network library with only numpy as dependency',
     long_description=open('README.md', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     url='https://github.com/marcpinet/handmade-neuralnetwork',
     packages=find_packages(),
     install_requires=[
```

