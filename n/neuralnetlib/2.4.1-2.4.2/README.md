# Comparing `tmp/neuralnetlib-2.4.1.tar.gz` & `tmp/neuralnetlib-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralnetlib-2.4.1.tar", last modified: Wed Apr 24 11:10:45 2024, max compression
+gzip compressed data, was "neuralnetlib-2.4.2.tar", last modified: Wed Apr 24 13:49:03 2024, max compression
```

## Comparing `neuralnetlib-2.4.1.tar` & `neuralnetlib-2.4.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:10:45.257758 neuralnetlib-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 11:10:35.000000 neuralnetlib-2.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-24 11:10:45.257758 neuralnetlib-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-24 11:10:35.000000 neuralnetlib-2.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:10:45.257758 neuralnetlib-2.4.1/neuralnetlib/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-24 11:10:35.000000 neuralnetlib-2.4.1/neuralnetlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-24 11:10:35.000000 neuralnetlib-2.4.1/neuralnetlib/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-24 11:10:35.000000 neuralnetlib-2.4.1/neuralnetlib/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    42004 2024-04-24 11:10:35.000000 neuralnetlib-2.4.1/neuralnetlib/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-24 11:10:35.000000 neuralnetlib-2.4.1/neuralnetlib/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-24 11:10:35.000000 neuralnetlib-2.4.1/neuralnetlib/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9681 2024-04-24 11:10:35.000000 neuralnetlib-2.4.1/neuralnetlib/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7261 2024-04-24 11:10:35.000000 neuralnetlib-2.4.1/neuralnetlib/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-04-24 11:10:35.000000 neuralnetlib-2.4.1/neuralnetlib/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-24 11:10:35.000000 neuralnetlib-2.4.1/neuralnetlib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:10:45.257758 neuralnetlib-2.4.1/neuralnetlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-24 11:10:45.000000 neuralnetlib-2.4.1/neuralnetlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-24 11:10:45.000000 neuralnetlib-2.4.1/neuralnetlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 11:10:45.000000 neuralnetlib-2.4.1/neuralnetlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 11:10:45.000000 neuralnetlib-2.4.1/neuralnetlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 11:10:45.000000 neuralnetlib-2.4.1/neuralnetlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 11:10:45.257758 neuralnetlib-2.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 11:10:35.000000 neuralnetlib-2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:49:03.441216 neuralnetlib-2.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 13:48:53.000000 neuralnetlib-2.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-24 13:49:03.441216 neuralnetlib-2.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-24 13:48:53.000000 neuralnetlib-2.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:49:03.437216 neuralnetlib-2.4.2/neuralnetlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-24 13:48:53.000000 neuralnetlib-2.4.2/neuralnetlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-24 13:48:53.000000 neuralnetlib-2.4.2/neuralnetlib/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-24 13:48:53.000000 neuralnetlib-2.4.2/neuralnetlib/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42004 2024-04-24 13:48:53.000000 neuralnetlib-2.4.2/neuralnetlib/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-24 13:48:53.000000 neuralnetlib-2.4.2/neuralnetlib/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-24 13:48:53.000000 neuralnetlib-2.4.2/neuralnetlib/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9681 2024-04-24 13:48:53.000000 neuralnetlib-2.4.2/neuralnetlib/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7261 2024-04-24 13:48:53.000000 neuralnetlib-2.4.2/neuralnetlib/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-04-24 13:48:53.000000 neuralnetlib-2.4.2/neuralnetlib/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-24 13:48:53.000000 neuralnetlib-2.4.2/neuralnetlib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:49:03.441216 neuralnetlib-2.4.2/neuralnetlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-24 13:49:03.000000 neuralnetlib-2.4.2/neuralnetlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-24 13:49:03.000000 neuralnetlib-2.4.2/neuralnetlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:49:03.000000 neuralnetlib-2.4.2/neuralnetlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 13:49:03.000000 neuralnetlib-2.4.2/neuralnetlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 13:49:03.000000 neuralnetlib-2.4.2/neuralnetlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 13:49:03.441216 neuralnetlib-2.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 13:48:53.000000 neuralnetlib-2.4.2/setup.py
```

### Comparing `neuralnetlib-2.4.1/LICENSE` & `neuralnetlib-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.4.1/PKG-INFO` & `neuralnetlib-2.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralnetlib
-Version: 2.4.1
+Version: 2.4.2
 Summary: A simple convolutional neural network library with only numpy as dependency
 Home-page: https://github.com/marcpinet/handmade-neuralnetwork
 Author: Marc Pinet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `neuralnetlib-2.4.1/README.md` & `neuralnetlib-2.4.2/README.md`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.4.1/neuralnetlib/activations.py` & `neuralnetlib-2.4.2/neuralnetlib/activations.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.4.1/neuralnetlib/callbacks.py` & `neuralnetlib-2.4.2/neuralnetlib/callbacks.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.4.1/neuralnetlib/layers.py` & `neuralnetlib-2.4.2/neuralnetlib/layers.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.4.1/neuralnetlib/losses.py` & `neuralnetlib-2.4.2/neuralnetlib/losses.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.4.1/neuralnetlib/metrics.py` & `neuralnetlib-2.4.2/neuralnetlib/metrics.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.4.1/neuralnetlib/model.py` & `neuralnetlib-2.4.2/neuralnetlib/model.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.4.1/neuralnetlib/optimizers.py` & `neuralnetlib-2.4.2/neuralnetlib/optimizers.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.4.1/neuralnetlib/preprocessing.py` & `neuralnetlib-2.4.2/neuralnetlib/preprocessing.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.4.1/neuralnetlib/utils.py` & `neuralnetlib-2.4.2/neuralnetlib/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,16 +16,18 @@
     """Converts all lists in a dictionary to numpy arrays. This is useful for deserializing the dictionary from JSON."""
     for k, v in d.items():
         if isinstance(v, list):
             d[k] = np.array(v)
     return d
 
 
-def shuffle(x, y, random_state: int = None) -> tuple:
+def shuffle(x: np.ndarray, y: np.ndarray, random_state: int = None) -> tuple:
     """Shuffles the data along the first axis."""
+    x = np.array(x)
+    y = np.array(y)
     rng = np.random.default_rng(random_state if random_state is not None else int(time.time_ns()))
     indices = rng.permutation(len(x))
     return x[indices], y[indices]
 
 
 def progress_bar(current: int, total: int, width: int = 30, message: str = "") -> None:
     """
@@ -40,27 +42,32 @@
     progress = current / total
     bar = '=' * int(width * progress) + '-' * (width - int(width * progress))
     percent = int(100 * progress)
     sys.stdout.write(f'\r[{bar}] {percent}% {message}')
     sys.stdout.flush()
 
 
-def train_test_split(x, y, test_size: float = 0.2, random_state: int = None) -> tuple:
+def train_test_split(x: np.ndarray, y: np.ndarray, test_size: float = 0.2, random_state: int = None) -> tuple:
     """
     Splits the data into training and test sets.
 
     Args:
-        x (np.ndarray): input data
-        y (np.ndarray): target data
+        x (np.ndarray or list): input data
+        y (np.ndarray or list): target data
         test_size (float): the proportion of the dataset to include in the test split
         random_state (int): seed for the random number generator
 
     Returns:
-        tuple: x_train, x_test, y_train, y_test
+        tuple: (x_train, x_test, y_train, y_test)
     """
+    x = np.array(x)
+    y = np.array(y)
     rng = np.random.default_rng(random_state if random_state is not None else int(time.time_ns()))
     indices = np.arange(len(x))
     rng.shuffle(indices)
     split_index = int(len(x) * (1 - test_size))
-    x_train, x_test = x[indices[:split_index]], x[indices[split_index:]]
-    y_train, y_test = y[indices[:split_index]], y[indices[split_index:]]
+    x_train = x[indices[:split_index]]
+    x_test = x[indices[split_index:]]
+    y_train = y[indices[:split_index]]
+    y_test = y[indices[split_index:]]
     return x_train, x_test, y_train, y_test
+
```

### Comparing `neuralnetlib-2.4.1/neuralnetlib.egg-info/PKG-INFO` & `neuralnetlib-2.4.2/neuralnetlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralnetlib
-Version: 2.4.1
+Version: 2.4.2
 Summary: A simple convolutional neural network library with only numpy as dependency
 Home-page: https://github.com/marcpinet/handmade-neuralnetwork
 Author: Marc Pinet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `neuralnetlib-2.4.1/setup.py` & `neuralnetlib-2.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='neuralnetlib',
-    version='2.4.1',
+    version='2.4.2',
     author='Marc Pinet',
     description='A simple convolutional neural network library with only numpy as dependency',
     long_description=open('README.md', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     url='https://github.com/marcpinet/handmade-neuralnetwork',
     packages=find_packages(),
     install_requires=[
```

