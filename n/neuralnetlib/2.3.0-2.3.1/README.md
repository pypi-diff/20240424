# Comparing `tmp/neuralnetlib-2.3.0.tar.gz` & `tmp/neuralnetlib-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralnetlib-2.3.0.tar", last modified: Wed Apr 24 00:56:17 2024, max compression
+gzip compressed data, was "neuralnetlib-2.3.1.tar", last modified: Wed Apr 24 01:14:28 2024, max compression
```

## Comparing `neuralnetlib-2.3.0.tar` & `neuralnetlib-2.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:56:17.175221 neuralnetlib-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 00:55:56.000000 neuralnetlib-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-24 00:56:17.175221 neuralnetlib-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-24 00:55:56.000000 neuralnetlib-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:56:17.175221 neuralnetlib-2.3.0/neuralnetlib/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-24 00:55:56.000000 neuralnetlib-2.3.0/neuralnetlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-24 00:55:56.000000 neuralnetlib-2.3.0/neuralnetlib/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)    33635 2024-04-24 00:55:56.000000 neuralnetlib-2.3.0/neuralnetlib/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-24 00:55:56.000000 neuralnetlib-2.3.0/neuralnetlib/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-24 00:55:56.000000 neuralnetlib-2.3.0/neuralnetlib/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10663 2024-04-24 00:55:56.000000 neuralnetlib-2.3.0/neuralnetlib/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7261 2024-04-24 00:55:56.000000 neuralnetlib-2.3.0/neuralnetlib/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-04-24 00:55:56.000000 neuralnetlib-2.3.0/neuralnetlib/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-24 00:55:56.000000 neuralnetlib-2.3.0/neuralnetlib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:56:17.175221 neuralnetlib-2.3.0/neuralnetlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-24 00:56:16.000000 neuralnetlib-2.3.0/neuralnetlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-24 00:56:17.000000 neuralnetlib-2.3.0/neuralnetlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 00:56:16.000000 neuralnetlib-2.3.0/neuralnetlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 00:56:16.000000 neuralnetlib-2.3.0/neuralnetlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 00:56:16.000000 neuralnetlib-2.3.0/neuralnetlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 00:56:17.175221 neuralnetlib-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 00:55:56.000000 neuralnetlib-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:14:28.779139 neuralnetlib-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 01:14:15.000000 neuralnetlib-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-24 01:14:28.779139 neuralnetlib-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-24 01:14:15.000000 neuralnetlib-2.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:14:28.779139 neuralnetlib-2.3.1/neuralnetlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-24 01:14:15.000000 neuralnetlib-2.3.1/neuralnetlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-24 01:14:15.000000 neuralnetlib-2.3.1/neuralnetlib/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40301 2024-04-24 01:14:15.000000 neuralnetlib-2.3.1/neuralnetlib/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-24 01:14:15.000000 neuralnetlib-2.3.1/neuralnetlib/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-24 01:14:15.000000 neuralnetlib-2.3.1/neuralnetlib/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-04-24 01:14:15.000000 neuralnetlib-2.3.1/neuralnetlib/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7261 2024-04-24 01:14:15.000000 neuralnetlib-2.3.1/neuralnetlib/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-04-24 01:14:15.000000 neuralnetlib-2.3.1/neuralnetlib/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-24 01:14:15.000000 neuralnetlib-2.3.1/neuralnetlib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:14:28.779139 neuralnetlib-2.3.1/neuralnetlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-24 01:14:28.000000 neuralnetlib-2.3.1/neuralnetlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-24 01:14:28.000000 neuralnetlib-2.3.1/neuralnetlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 01:14:28.000000 neuralnetlib-2.3.1/neuralnetlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 01:14:28.000000 neuralnetlib-2.3.1/neuralnetlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 01:14:28.000000 neuralnetlib-2.3.1/neuralnetlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 01:14:28.779139 neuralnetlib-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 01:14:15.000000 neuralnetlib-2.3.1/setup.py
```

### Comparing `neuralnetlib-2.3.0/LICENSE` & `neuralnetlib-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.0/PKG-INFO` & `neuralnetlib-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralnetlib
-Version: 2.3.0
+Version: 2.3.1
 Summary: A simple convolutional neural network library with only numpy as dependency
 Home-page: https://github.com/marcpinet/handmade-neuralnetwork
 Author: Marc Pinet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -31,15 +31,15 @@
 
 Remember that this library is not optimized for performance, but for learning purposes (although I tried to make it as fast as possible).
 
 I intend to improve the neural networks and add more features in the future.
 
 ## 📦 Features
 
-- Many layers (input, activation, dense, dropout, conv2d, maxpooling2d, flatten) 🧠
+- Many layers (input, activation, dense, dropout, conv1d/2d, maxpooling1d/2d, flatten, embedding, batchnormalization, and more) 🧠
 - Many activation functions (sigmoid, tanh, relu, leaky relu, softmax, linear, elu, selu) 📈
 - Many loss functions (mean squared error, mean absolute error, categorical crossentropy, binary crossentropy, huber loss) 📉
 - Many optimizers (sgd, momentum, rmsprop, adam) 📊
 - Supports binary classification, multiclass classification and regression 📖
 - Save and load models 📁
 - Simple to use 📚
```

### Comparing `neuralnetlib-2.3.0/README.md` & `neuralnetlib-2.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 Remember that this library is not optimized for performance, but for learning purposes (although I tried to make it as fast as possible).
 
 I intend to improve the neural networks and add more features in the future.
 
 ## 📦 Features
 
-- Many layers (input, activation, dense, dropout, conv2d, maxpooling2d, flatten) 🧠
+- Many layers (input, activation, dense, dropout, conv1d/2d, maxpooling1d/2d, flatten, embedding, batchnormalization, and more) 🧠
 - Many activation functions (sigmoid, tanh, relu, leaky relu, softmax, linear, elu, selu) 📈
 - Many loss functions (mean squared error, mean absolute error, categorical crossentropy, binary crossentropy, huber loss) 📉
 - Many optimizers (sgd, momentum, rmsprop, adam) 📊
 - Supports binary classification, multiclass classification and regression 📖
 - Save and load models 📁
 - Simple to use 📚
```

### Comparing `neuralnetlib-2.3.0/neuralnetlib/activations.py` & `neuralnetlib-2.3.1/neuralnetlib/activations.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.0/neuralnetlib/layers.py` & `neuralnetlib-2.3.1/neuralnetlib/layers.py`

 * *Files 12% similar despite different names*

```diff
@@ -794,8 +794,172 @@
 
     @staticmethod
     def from_config(config: dict):
         layer = BatchNormalization(config['momentum'], config['epsilon'])
         if config['gamma'] is not None:
             layer.gamma = np.array(config['gamma'])
             layer.beta = np.array(config['beta'])
-        return layer
+        return layer
+    
+    
+class AveragePooling2D(Layer):
+    def __init__(self, pool_size: tuple | int, stride: tuple = None, padding: str = 'valid'):
+        if isinstance(pool_size, int):
+            self.pool_size = (pool_size, pool_size)
+        else:
+            self.pool_size = pool_size
+        self.stride = stride if stride is not None else self.pool_size
+        self.padding = padding
+
+    def __str__(self):
+        return f'AveragePooling2D(pool_size={self.pool_size}, stride={self.stride}, padding={self.padding})'
+
+    def forward_pass(self, input_data: np.ndarray) -> np.ndarray:
+        assert len(input_data.shape) == 4, f"AveragePooling2D input must be 4D (batch_size, channels, height, width), got {input_data.shape}"
+        self.input = input_data
+        output = self._pool(self.input, self.pool_size, self.stride, self.padding)
+        return output
+
+    def backward_pass(self, output_error: np.ndarray) -> np.ndarray:
+        input_error = self._pool_backward(output_error, self.input, self.pool_size, self.stride, self.padding)
+        return input_error
+
+    def get_config(self) -> dict:
+        return {
+            'name': self.__class__.__name__,
+            'pool_size': self.pool_size,
+            'stride': self.stride,
+            'padding': self.padding
+        }
+
+    @staticmethod
+    def from_config(config: dict):
+        return AveragePooling2D(config['pool_size'], config['stride'], config['padding'])
+
+    @staticmethod
+    def _pool(input_data: np.ndarray, pool_size: tuple, stride: tuple, padding: str) -> np.ndarray:
+        batch_size, channels, in_height, in_width = input_data.shape
+
+        if padding == 'same':
+            pad_height = ((in_height - 1) * stride[0] + pool_size[0] - in_height) // 2
+            pad_width = ((in_width - 1) * stride[1] + pool_size[1] - in_width) // 2
+        else:
+            pad_height, pad_width = 0, 0
+
+        padded_input = np.pad(input_data, ((0, 0), (0, 0), (pad_height, pad_height), (pad_width, pad_width)),
+                              mode='constant')
+
+        out_height = (in_height + 2 * pad_height - pool_size[0]) // stride[0] + 1
+        out_width = (in_width + 2 * pad_width - pool_size[1]) // stride[1] + 1
+
+        output = np.zeros((batch_size, channels, out_height, out_width))
+
+        for i in range(out_height):
+            for j in range(out_width):
+                input_slice = padded_input[:, :, i * stride[0]:i * stride[0] + pool_size[0],
+                              j * stride[1]:j * stride[1] + pool_size[1]]
+                output[:, :, i, j] = np.mean(input_slice, axis=(2, 3))
+
+        return output
+
+    @staticmethod
+    def _pool_backward(output_error: np.ndarray, input_data: np.ndarray, pool_size: tuple, stride: tuple,
+                       padding: str) -> np.ndarray:
+        batch_size, channels, in_height, in_width = input_data.shape
+        _, _, out_height, out_width = output_error.shape
+
+        if padding == 'same':
+            pad_height = ((in_height - 1) * stride[0] + pool_size[0] - in_height) // 2
+            pad_width = ((in_width - 1) * stride[1] + pool_size[1] - in_width) // 2
+        else:
+            pad_height, pad_width = 0, 0
+
+        padded_input = np.pad(input_data, ((0, 0), (0, 0), (pad_height, pad_height), (pad_width, pad_width)),
+                              mode='constant')
+
+        d_input = np.zeros_like(padded_input)
+
+        for i in range(out_height):
+            for j in range(out_width):
+                d_input[:, :, i * stride[0]:i * stride[0] + pool_size[0],
+                j * stride[1]:j * stride[1] + pool_size[1]] += output_error[:, :, i, j][:, :, np.newaxis, np.newaxis] / np.prod(pool_size)
+
+        if padding == 'same':
+            d_input = d_input[:, :, pad_height:-pad_height, pad_width:-pad_width]
+
+        return d_input
+
+
+class AveragePooling1D(Layer):
+    def __init__(self, pool_size: int, stride: int = None, padding: str = 'valid'):
+        self.pool_size = pool_size
+        self.stride = stride if stride is not None else pool_size
+        self.padding = padding
+
+    def __str__(self):
+        return f'AveragePooling1D(pool_size={self.pool_size}, stride={self.stride}, padding={self.padding})'
+
+    def forward_pass(self, input_data: np.ndarray) -> np.ndarray:
+        assert len(input_data.shape) == 3, f"AveragePooling1D input must be 3D (batch_size, steps, features), got {input_data.shape}"
+        self.input = input_data
+        output = self._pool(self.input, self.pool_size, self.stride, self.padding)
+        return output
+
+    def backward_pass(self, output_error: np.ndarray) -> np.ndarray:
+        input_error = self._pool_backward(output_error, self.input, self.pool_size, self.stride, self.padding)
+        return input_error
+
+    def get_config(self) -> dict:
+        return {
+            'name': self.__class__.__name__,
+            'pool_size': self.pool_size,
+            'stride': self.stride,
+            'padding': self.padding
+        }
+
+    @staticmethod
+    def from_config(config: dict):
+        return AveragePooling1D(config['pool_size'], config['stride'], config['padding'])
+
+    @staticmethod
+    def _pool(input_data: np.ndarray, pool_size: int, stride: int, padding: str) -> np.ndarray:
+        batch_size, steps, features = input_data.shape
+
+        if padding == 'same':
+            pad_steps = ((steps - 1) * stride + pool_size - steps) // 2
+        else:
+            pad_steps = 0
+
+        padded_input = np.pad(input_data, ((0, 0), (pad_steps, pad_steps), (0, 0)), mode='constant')
+
+        out_steps = (steps + 2 * pad_steps - pool_size) // stride + 1
+
+        output = np.zeros((batch_size, out_steps, features))
+
+        for i in range(out_steps):
+            input_slice = padded_input[:, i * stride:i * stride + pool_size, :]
+            output[:, i, :] = np.mean(input_slice, axis=1)
+
+        return output
+
+    @staticmethod
+    def _pool_backward(output_error: np.ndarray, input_data: np.ndarray, pool_size: int, stride: int,
+                       padding: str) -> np.ndarray:
+        batch_size, steps, features = input_data.shape
+        _, out_steps, _ = output_error.shape
+
+        if padding == 'same':
+            pad_steps = ((steps - 1) * stride + pool_size - steps) // 2
+        else:
+            pad_steps = 0
+
+        padded_input = np.pad(input_data, ((0, 0), (pad_steps, pad_steps), (0, 0)), mode='constant')
+
+        d_input = np.zeros_like(padded_input)
+
+        for i in range(out_steps):
+            d_input[:, i * stride:i * stride + pool_size, :] += output_error[:, i, :][:, np.newaxis, :] / pool_size
+
+        if padding == 'same':
+            d_input = d_input[:, pad_steps:-pad_steps, :]
+
+        return d_input
```

### Comparing `neuralnetlib-2.3.0/neuralnetlib/losses.py` & `neuralnetlib-2.3.1/neuralnetlib/losses.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.0/neuralnetlib/metrics.py` & `neuralnetlib-2.3.1/neuralnetlib/metrics.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.0/neuralnetlib/model.py` & `neuralnetlib-2.3.1/neuralnetlib/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import time
 
 import numpy as np
 
-from neuralnetlib.layers import Layer, Input, Dense, Activation, Conv2D, MaxPooling2D, Conv1D, MaxPooling1D, Flatten, Dropout, Embedding, BatchNormalization
+from neuralnetlib.layers import Layer, Input, Dense, Activation, Conv2D, MaxPooling2D, Conv1D, MaxPooling1D, AveragePooling2D, AveragePooling1D, Flatten, Dropout, Embedding, BatchNormalization
 from neuralnetlib.losses import LossFunction, CategoricalCrossentropy
 from neuralnetlib.optimizers import Optimizer
 from neuralnetlib.utils import shuffle, progress_bar
 from neuralnetlib.metrics import accuracy_score
 
 
 class Model:
@@ -34,45 +34,47 @@
 
     def add(self, layer: Layer):
         if not self.layers:
             if not isinstance(layer, Input):
                 raise ValueError("The first layer must be an Input layer.")
         else:
             previous_layer = self.layers[-1]
-
             if isinstance(previous_layer, Input):
                 if not isinstance(layer, (Dense, Conv2D, Conv1D, Embedding)):
                     raise ValueError("Input layer can only be followed by Dense, Conv2D, Conv1D, or Embedding.")
             elif isinstance(previous_layer, Dense):
                 if not isinstance(layer, (Dense, Activation, Dropout, BatchNormalization)):
                     raise ValueError("Dense layer can only be followed by Dense, Activation, BatchNormalization, or Dropout.")
             elif isinstance(previous_layer, Activation):
-                if not isinstance(layer, (Dense, Conv2D, Conv1D, MaxPooling2D, MaxPooling1D, Flatten, Dropout)):
-                    raise ValueError("Activation layer can only be followed by Dense, Conv2D, Conv1D, MaxPooling2D, MaxPooling1D, Flatten, or Dropout.")
+                if not isinstance(layer, (Dense, Conv2D, Conv1D, MaxPooling2D, AveragePooling2D, MaxPooling1D, AveragePooling1D, Flatten, Dropout)):
+                    raise ValueError("Activation layer can only be followed by Dense, Conv2D, Conv1D, MaxPooling2D, AveragePooling2D, MaxPooling1D, AveragePooling1D, Flatten, or Dropout.")
             elif isinstance(previous_layer, Conv2D):
-                if not isinstance(layer, (Conv2D, MaxPooling2D, Activation, Dropout, Flatten, BatchNormalization)):
-                    raise ValueError("Conv2D layer can only be followed by Conv2D, MaxPooling2D, Activation, Dropout, BatchNormalization, or Flatten.")
-            elif isinstance(previous_layer, MaxPooling2D):
-                if not isinstance(layer, (Conv2D, MaxPooling2D, Flatten)):
-                    raise ValueError("MaxPooling2D layer can only be followed by Conv2D, MaxPooling2D, or Flatten.")
+                if not isinstance(layer, (Conv2D, MaxPooling2D, AveragePooling2D, Activation, Dropout, Flatten, BatchNormalization)):
+                    raise ValueError("Conv2D layer can only be followed by Conv2D, MaxPooling2D, AveragePooling2D, Activation, Dropout, BatchNormalization, or Flatten.")
+            elif isinstance(previous_layer, MaxPooling2D) or isinstance(previous_layer, AveragePooling2D):
+                if not isinstance(layer, (Conv2D, MaxPooling2D, AveragePooling2D, Flatten)):
+                    raise ValueError("MaxPooling2D or AveragePooling2D layer can only be followed by Conv2D, MaxPooling2D, AveragePooling2D, or Flatten.")
             elif isinstance(previous_layer, Conv1D):
-                if not isinstance(layer, (Conv1D, MaxPooling1D, Activation, Dropout, Flatten, BatchNormalization)):
-                    raise ValueError("Conv1D layer can only be followed by Conv1D, MaxPooling1D, Activation, Dropout, BatchNormalization, or Flatten.")
-            elif isinstance(previous_layer, MaxPooling1D):
-                if not isinstance(layer, (Conv1D, MaxPooling1D, Flatten)):
-                    raise ValueError("MaxPooling1D layer can only be followed by Conv1D, MaxPooling1D, or Flatten.")
+                if not isinstance(layer, (Conv1D, MaxPooling1D, AveragePooling1D, Activation, Dropout, Flatten, BatchNormalization)):
+                    raise ValueError("Conv1D layer can only be followed by Conv1D, MaxPooling1D, AveragePooling1D, Activation, Dropout, BatchNormalization, or Flatten.")
+            elif isinstance(previous_layer, MaxPooling1D) or isinstance(previous_layer, AveragePooling1D):
+                if not isinstance(layer, (Conv1D, MaxPooling1D, AveragePooling1D, Flatten)):
+                    raise ValueError("MaxPooling1D or AveragePooling1D layer can only be followed by Conv1D, MaxPooling1D, AveragePooling1D, or Flatten.")
             elif isinstance(previous_layer, Flatten):
                 if not isinstance(layer, (Dense, Dropout)):
                     raise ValueError("Flatten layer can only be followed by Dense or Dropout.")
             elif isinstance(previous_layer, Dropout):
                 if not isinstance(layer, (Dense, Conv2D, Conv1D, Activation)):
                     raise ValueError("Dropout layer can only be followed by Dense, Conv2D, Conv1D, or Activation.")
             elif isinstance(previous_layer, Embedding):
                 if not isinstance(layer, (Conv1D, Flatten, Dense)):
                     raise ValueError("Embedding layer can only be followed by Conv1D, Flatten, or Dense.")
+            elif isinstance(previous_layer, BatchNormalization):
+                if not isinstance(layer, (Dense, Conv2D, Conv1D, Activation)):
+                    raise ValueError("BatchNormalization layer can only be followed by Dense, Conv2D, Conv1D, or Activation.")
         
         self.layers.append(layer)
 
     def compile(self, loss_function: LossFunction, optimizer: Optimizer, verbose: bool = False):
         self.loss_function = loss_function
         self.optimizer = optimizer
         if verbose:
```

### Comparing `neuralnetlib-2.3.0/neuralnetlib/optimizers.py` & `neuralnetlib-2.3.1/neuralnetlib/optimizers.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.0/neuralnetlib/preprocessing.py` & `neuralnetlib-2.3.1/neuralnetlib/preprocessing.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.0/neuralnetlib/utils.py` & `neuralnetlib-2.3.1/neuralnetlib/utils.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.0/neuralnetlib.egg-info/PKG-INFO` & `neuralnetlib-2.3.1/neuralnetlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralnetlib
-Version: 2.3.0
+Version: 2.3.1
 Summary: A simple convolutional neural network library with only numpy as dependency
 Home-page: https://github.com/marcpinet/handmade-neuralnetwork
 Author: Marc Pinet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -31,15 +31,15 @@
 
 Remember that this library is not optimized for performance, but for learning purposes (although I tried to make it as fast as possible).
 
 I intend to improve the neural networks and add more features in the future.
 
 ## 📦 Features
 
-- Many layers (input, activation, dense, dropout, conv2d, maxpooling2d, flatten) 🧠
+- Many layers (input, activation, dense, dropout, conv1d/2d, maxpooling1d/2d, flatten, embedding, batchnormalization, and more) 🧠
 - Many activation functions (sigmoid, tanh, relu, leaky relu, softmax, linear, elu, selu) 📈
 - Many loss functions (mean squared error, mean absolute error, categorical crossentropy, binary crossentropy, huber loss) 📉
 - Many optimizers (sgd, momentum, rmsprop, adam) 📊
 - Supports binary classification, multiclass classification and regression 📖
 - Save and load models 📁
 - Simple to use 📚
```

### Comparing `neuralnetlib-2.3.0/setup.py` & `neuralnetlib-2.3.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='neuralnetlib',
-    version='2.3.0',
+    version='2.3.1',
     author='Marc Pinet',
     description='A simple convolutional neural network library with only numpy as dependency',
     long_description=open('README.md', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     url='https://github.com/marcpinet/handmade-neuralnetwork',
     packages=find_packages(),
     install_requires=[
```

