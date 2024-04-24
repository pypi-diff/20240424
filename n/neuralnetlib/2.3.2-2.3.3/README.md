# Comparing `tmp/neuralnetlib-2.3.2.tar.gz` & `tmp/neuralnetlib-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralnetlib-2.3.2.tar", last modified: Wed Apr 24 01:23:52 2024, max compression
+gzip compressed data, was "neuralnetlib-2.3.3.tar", last modified: Wed Apr 24 02:51:31 2024, max compression
```

## Comparing `neuralnetlib-2.3.2.tar` & `neuralnetlib-2.3.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:23:52.241866 neuralnetlib-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 01:23:41.000000 neuralnetlib-2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-24 01:23:52.241866 neuralnetlib-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-24 01:23:41.000000 neuralnetlib-2.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:23:52.241866 neuralnetlib-2.3.2/neuralnetlib/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-24 01:23:41.000000 neuralnetlib-2.3.2/neuralnetlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-24 01:23:41.000000 neuralnetlib-2.3.2/neuralnetlib/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)    41351 2024-04-24 01:23:41.000000 neuralnetlib-2.3.2/neuralnetlib/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-24 01:23:41.000000 neuralnetlib-2.3.2/neuralnetlib/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-24 01:23:41.000000 neuralnetlib-2.3.2/neuralnetlib/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8117 2024-04-24 01:23:41.000000 neuralnetlib-2.3.2/neuralnetlib/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7261 2024-04-24 01:23:41.000000 neuralnetlib-2.3.2/neuralnetlib/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-04-24 01:23:41.000000 neuralnetlib-2.3.2/neuralnetlib/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-24 01:23:41.000000 neuralnetlib-2.3.2/neuralnetlib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:23:52.241866 neuralnetlib-2.3.2/neuralnetlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-24 01:23:52.000000 neuralnetlib-2.3.2/neuralnetlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-24 01:23:52.000000 neuralnetlib-2.3.2/neuralnetlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 01:23:52.000000 neuralnetlib-2.3.2/neuralnetlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 01:23:52.000000 neuralnetlib-2.3.2/neuralnetlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 01:23:52.000000 neuralnetlib-2.3.2/neuralnetlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 01:23:52.241866 neuralnetlib-2.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 01:23:41.000000 neuralnetlib-2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:51:31.955064 neuralnetlib-2.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 02:51:23.000000 neuralnetlib-2.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-24 02:51:31.955064 neuralnetlib-2.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-24 02:51:23.000000 neuralnetlib-2.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:51:31.955064 neuralnetlib-2.3.3/neuralnetlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-24 02:51:23.000000 neuralnetlib-2.3.3/neuralnetlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-24 02:51:23.000000 neuralnetlib-2.3.3/neuralnetlib/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-24 02:51:23.000000 neuralnetlib-2.3.3/neuralnetlib/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42004 2024-04-24 02:51:23.000000 neuralnetlib-2.3.3/neuralnetlib/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-24 02:51:23.000000 neuralnetlib-2.3.3/neuralnetlib/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-24 02:51:23.000000 neuralnetlib-2.3.3/neuralnetlib/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9653 2024-04-24 02:51:23.000000 neuralnetlib-2.3.3/neuralnetlib/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7261 2024-04-24 02:51:23.000000 neuralnetlib-2.3.3/neuralnetlib/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-04-24 02:51:23.000000 neuralnetlib-2.3.3/neuralnetlib/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-24 02:51:23.000000 neuralnetlib-2.3.3/neuralnetlib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:51:31.955064 neuralnetlib-2.3.3/neuralnetlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-24 02:51:31.000000 neuralnetlib-2.3.3/neuralnetlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-24 02:51:31.000000 neuralnetlib-2.3.3/neuralnetlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:51:31.000000 neuralnetlib-2.3.3/neuralnetlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 02:51:31.000000 neuralnetlib-2.3.3/neuralnetlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 02:51:31.000000 neuralnetlib-2.3.3/neuralnetlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 02:51:31.955064 neuralnetlib-2.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 02:51:23.000000 neuralnetlib-2.3.3/setup.py
```

### Comparing `neuralnetlib-2.3.2/LICENSE` & `neuralnetlib-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.2/PKG-INFO` & `neuralnetlib-2.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralnetlib
-Version: 2.3.2
+Version: 2.3.3
 Summary: A simple convolutional neural network library with only numpy as dependency
 Home-page: https://github.com/marcpinet/handmade-neuralnetwork
 Author: Marc Pinet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `neuralnetlib-2.3.2/README.md` & `neuralnetlib-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.2/neuralnetlib/activations.py` & `neuralnetlib-2.3.3/neuralnetlib/activations.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.2/neuralnetlib/layers.py` & `neuralnetlib-2.3.3/neuralnetlib/layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,16 @@
 
     @staticmethod
     def from_config(config: dict):
         return Dropout(config['rate'], config['seed'])
 
 
 class Conv2D(Layer):
-    def __init__(self, filters: int, kernel_size: int | tuple, stride: int | tuple = 1, padding: str = 'valid', weights_init: str = "default", bias_init: str = "default", random_state: int = None):
+    def __init__(self, filters: int, kernel_size: int | tuple, stride: int | tuple = 1, padding: str = 'valid',
+                 weights_init: str = "default", bias_init: str = "default", random_state: int = None):
         self.filters = filters
         self.kernel_size = (kernel_size, kernel_size) if isinstance(kernel_size, int) else kernel_size
         self.stride = (stride, stride) if isinstance(stride, int) else stride
         self.padding = padding
 
         self.weights = None
         self.bias = None
@@ -237,17 +238,19 @@
         self.random_state = random_state
 
     def initialize_weights(self, input_shape: tuple):
         in_channels, _, _ = input_shape
 
         self.rng = np.random.default_rng(self.random_state if self.random_state is not None else int(time.time_ns()))
         if self.weights_init == "xavier":
-            self.weights = self.rng.normal(0, np.sqrt(2 / (np.prod(self.kernel_size) * in_channels)), (self.filters, in_channels, *self.kernel_size))
+            self.weights = self.rng.normal(0, np.sqrt(2 / (np.prod(self.kernel_size) * in_channels)),
+                                           (self.filters, in_channels, *self.kernel_size))
         elif self.weights_init == "he":
-            self.weights = self.rng.normal(0, np.sqrt(2 / (in_channels * np.prod(self.kernel_size))), (self.filters, in_channels, *self.kernel_size))
+            self.weights = self.rng.normal(0, np.sqrt(2 / (in_channels * np.prod(self.kernel_size))),
+                                           (self.filters, in_channels, *self.kernel_size))
         elif self.weights_init == "default":
             self.weights = self.rng.normal(0, 0.01, (self.filters, in_channels, *self.kernel_size))
         else:
             raise ValueError("Invalid weights_init value. Possible values are 'xavier', 'he', and 'default'.")
 
         if self.bias_init == "default":
             self.bias = np.zeros((1, self.filters))
@@ -264,23 +267,25 @@
         self.d_bias = np.zeros_like(self.bias)
 
     def __str__(self):
         return f'Conv2D(num_filters={self.filters}, kernel_size={self.kernel_size}, stride={self.stride}, padding={self.padding})'
 
     def forward_pass(self, input_data: np.ndarray) -> np.ndarray:
         if self.weights is None:
-            assert len(input_data.shape) == 4, f"Conv2D input must be 4D (batch_size, channels, height, width), got {input_data.shape}"
+            assert len(
+                input_data.shape) == 4, f"Conv2D input must be 4D (batch_size, channels, height, width), got {input_data.shape}"
             self.initialize_weights(input_data.shape[1:])
 
         self.input = input_data
         output = self._convolve(self.input, self.weights, self.bias, self.stride, self.padding)
         return output
 
     def backward_pass(self, output_error: np.ndarray) -> np.ndarray:
-        input_error, self.d_weights, self.d_bias = self._convolve_backward(output_error, self.input, self.weights, self.stride, self.padding)
+        input_error, self.d_weights, self.d_bias = self._convolve_backward(output_error, self.input, self.weights,
+                                                                           self.stride, self.padding)
         return input_error
 
     def get_config(self) -> dict:
         return {
             'name': self.__class__.__name__,
             'weights': self.weights.tolist() if self.weights is not None else None,
             'bias': self.bias.tolist() if self.bias is not None else None,
@@ -363,15 +368,16 @@
         self.stride = stride if stride is not None else self.pool_size
         self.padding = padding
 
     def __str__(self):
         return f'MaxPooling2D(pool_size={self.pool_size}, stride={self.stride}, padding={self.padding})'
 
     def forward_pass(self, input_data: np.ndarray) -> np.ndarray:
-        assert len(input_data.shape) == 4, f"MaxPooling2D input must be 4D (batch_size, channels, height, width), got {input_data.shape}"
+        assert len(
+            input_data.shape) == 4, f"MaxPooling2D input must be 4D (batch_size, channels, height, width), got {input_data.shape}"
         self.input = input_data
         output = self._pool(self.input, self.pool_size, self.stride, self.padding)
         return output
 
     def backward_pass(self, output_error: np.ndarray) -> np.ndarray:
         input_error = self._pool_backward(output_error, self.input, self.pool_size, self.stride, self.padding)
         return input_error
@@ -463,15 +469,16 @@
 
     @staticmethod
     def from_config(config: dict):
         return Flatten()
 
 
 class Conv1D(Layer):
-    def __init__(self, filters: int, kernel_size: int, stride: int = 1, padding: str = 'valid', weights_init: str = "default", bias_init: str = "default", random_state: int = None):
+    def __init__(self, filters: int, kernel_size: int, stride: int = 1, padding: str = 'valid',
+                 weights_init: str = "default", bias_init: str = "default", random_state: int = None):
         self.filters = filters
         self.kernel_size = kernel_size
         self.stride = stride
         self.padding = padding
 
         self.weights = None
         self.bias = None
@@ -483,17 +490,19 @@
         self.random_state = random_state
 
     def initialize_weights(self, input_shape: tuple):
         in_channels = input_shape[0]
 
         self.rng = np.random.default_rng(self.random_state if self.random_state is not None else int(time.time_ns()))
         if self.weights_init == "xavier":
-            self.weights = self.rng.normal(0, np.sqrt(2 / (self.kernel_size * in_channels)), (self.filters, in_channels, self.kernel_size))
+            self.weights = self.rng.normal(0, np.sqrt(2 / (self.kernel_size * in_channels)),
+                                           (self.filters, in_channels, self.kernel_size))
         elif self.weights_init == "he":
-            self.weights = self.rng.normal(0, np.sqrt(2 / (in_channels * self.kernel_size)), (self.filters, in_channels, self.kernel_size))
+            self.weights = self.rng.normal(0, np.sqrt(2 / (in_channels * self.kernel_size)),
+                                           (self.filters, in_channels, self.kernel_size))
         elif self.weights_init == "default":
             self.weights = self.rng.normal(0, 0.01, (self.filters, in_channels, self.kernel_size))
         else:
             raise ValueError("Invalid weights_init value. Possible values are 'xavier', 'he', and 'default'.")
 
         if self.bias_init == "default":
             self.bias = np.zeros((1, self.filters))
@@ -510,23 +519,25 @@
         self.d_bias = np.zeros_like(self.bias)
 
     def __str__(self):
         return f'Conv1D(num_filters={self.filters}, kernel_size={self.kernel_size}, stride={self.stride}, padding={self.padding})'
 
     def forward_pass(self, input_data: np.ndarray) -> np.ndarray:
         if self.weights is None:
-            assert len(input_data.shape) == 3, f"Conv1D input must be 3D (batch_size, steps, features), got {input_data.shape}"
+            assert len(
+                input_data.shape) == 3, f"Conv1D input must be 3D (batch_size, steps, features), got {input_data.shape}"
             self.initialize_weights(input_data.shape[1:])
 
         self.input = input_data
         output = self._convolve(self.input, self.weights, self.bias, self.stride, self.padding)
         return output
 
     def backward_pass(self, output_error: np.ndarray) -> np.ndarray:
-        input_error, self.d_weights, self.d_bias = self._convolve_backward(output_error, self.input, self.weights, self.stride, self.padding)
+        input_error, self.d_weights, self.d_bias = self._convolve_backward(output_error, self.input, self.weights,
+                                                                           self.stride, self.padding)
         return input_error
 
     def get_config(self) -> dict:
         return {
             'name': self.__class__.__name__,
             'weights': self.weights.tolist() if self.weights is not None else None,
             'bias': self.bias.tolist() if self.bias is not None else None,
@@ -603,15 +614,16 @@
         self.stride = stride if stride is not None else pool_size
         self.padding = padding
 
     def __str__(self):
         return f'MaxPooling1D(pool_size={self.pool_size}, stride={self.stride}, padding={self.padding})'
 
     def forward_pass(self, input_data: np.ndarray) -> np.ndarray:
-        assert len(input_data.shape) == 3, f"MaxPooling1D input must be 3D (batch_size, steps, features), got {input_data.shape}"
+        assert len(
+            input_data.shape) == 3, f"MaxPooling1D input must be 3D (batch_size, steps, features), got {input_data.shape}"
         self.input = input_data
         output = self._pool(self.input, self.pool_size, self.stride, self.padding)
         return output
 
     def backward_pass(self, output_error: np.ndarray) -> np.ndarray:
         input_error = self._pool_backward(output_error, self.input, self.pool_size, self.stride, self.padding)
         return input_error
@@ -672,39 +684,42 @@
         if padding == 'same':
             d_input = d_input[:, :, pad_length:-pad_length]
 
         return d_input
 
 
 class Embedding(Layer):
-    def __init__(self, input_dim: int, output_dim: int, input_length: int = None, weights_init: str = "default", random_state: int = None):
+    def __init__(self, input_dim: int, output_dim: int, input_length: int = None, weights_init: str = "default",
+                 random_state: int = None):
         self.input_dim = input_dim
         self.output_dim = output_dim
         self.input_length = input_length
         self.weights = None
         self.weights_init = weights_init
         self.random_state = random_state
 
     def initialize_weights(self):
         self.rng = np.random.default_rng(self.random_state if self.random_state is not None else int(time.time_ns()))
         if self.weights_init == "xavier":
-            self.weights = self.rng.normal(0, np.sqrt(2 / (self.input_dim + self.output_dim)), (self.input_dim, self.output_dim))
+            self.weights = self.rng.normal(0, np.sqrt(2 / (self.input_dim + self.output_dim)),
+                                           (self.input_dim, self.output_dim))
         elif self.weights_init == "he":
             self.weights = self.rng.normal(0, np.sqrt(2 / self.input_dim), (self.input_dim, self.output_dim))
         elif self.weights_init == "default":
             self.weights = self.rng.normal(0, 0.01, (self.input_dim, self.output_dim))
         else:
             raise ValueError("Invalid weights_init value. Possible values are 'xavier', 'he', and 'default'.")
 
     def __str__(self):
         return f'Embedding(input_dim={self.input_dim}, output_dim={self.output_dim}, input_length={self.input_length})'
 
     def forward_pass(self, input_data: np.ndarray) -> np.ndarray:
         if self.weights is None:
-            assert len(input_data.shape) == 2, f"Embedding input must be 2D (batch_size, sequence_length), got {input_data.shape}"
+            assert len(
+                input_data.shape) == 2, f"Embedding input must be 2D (batch_size, sequence_length), got {input_data.shape}"
             self.initialize_weights()
 
         self.input = input_data
         output = self.weights[input_data]
         return output
 
     def backward_pass(self, output_error: np.ndarray) -> np.ndarray:
@@ -723,20 +738,21 @@
             'input_length': self.input_length,
             'weights_init': self.weights_init,
             'random_state': self.random_state
         }
 
     @staticmethod
     def from_config(config: dict):
-        layer = Embedding(config['input_dim'], config['output_dim'], config['input_length'], config['weights_init'], config['random_state'])
+        layer = Embedding(config['input_dim'], config['output_dim'], config['input_length'], config['weights_init'],
+                          config['random_state'])
         if config['weights'] is not None:
             layer.weights = np.array(config['weights'])
         return layer
-    
-    
+
+
 class BatchNormalization(Layer):
     def __init__(self, momentum: float = 0.99, epsilon: float = 1e-8):
         self.gamma = None
         self.beta = None
         self.d_gamma = None
         self.d_beta = None
         self.momentum = momentum
@@ -774,17 +790,20 @@
 
     def backward_pass(self, output_error: np.ndarray) -> np.ndarray:
         N = output_error.shape[0]
         self.d_gamma = np.sum(output_error * self.input_normalized, axis=0)
         self.d_beta = np.sum(output_error, axis=0)
 
         d_input_normalized = output_error * self.gamma
-        d_var = np.sum(d_input_normalized * self.input_centered, axis=0) * -0.5 * (self.input_centered / (self.input_centered.var(axis=0) + self.epsilon) ** 1.5)
-        d_mean = np.sum(d_input_normalized, axis=0) * -1 / np.sqrt(self.input_centered.var(axis=0) + self.epsilon) - 2 * d_var * np.mean(self.input_centered, axis=0)
-        d_input = d_input_normalized / np.sqrt(self.input_centered.var(axis=0) + self.epsilon) + 2 * d_var * self.input_centered / N + d_mean / N
+        d_var = np.sum(d_input_normalized * self.input_centered, axis=0) * -0.5 * (
+                    self.input_centered / (self.input_centered.var(axis=0) + self.epsilon) ** 1.5)
+        d_mean = np.sum(d_input_normalized, axis=0) * -1 / np.sqrt(
+            self.input_centered.var(axis=0) + self.epsilon) - 2 * d_var * np.mean(self.input_centered, axis=0)
+        d_input = d_input_normalized / np.sqrt(
+            self.input_centered.var(axis=0) + self.epsilon) + 2 * d_var * self.input_centered / N + d_mean / N
         return d_input
 
     def get_config(self) -> dict:
         return {
             'name': self.__class__.__name__,
             'gamma': self.gamma.tolist() if self.gamma is not None else None,
             'beta': self.beta.tolist() if self.beta is not None else None,
@@ -795,30 +814,31 @@
     @staticmethod
     def from_config(config: dict):
         layer = BatchNormalization(config['momentum'], config['epsilon'])
         if config['gamma'] is not None:
             layer.gamma = np.array(config['gamma'])
             layer.beta = np.array(config['beta'])
         return layer
-    
-    
+
+
 class AveragePooling2D(Layer):
     def __init__(self, pool_size: tuple | int, stride: tuple = None, padding: str = 'valid'):
         if isinstance(pool_size, int):
             self.pool_size = (pool_size, pool_size)
         else:
             self.pool_size = pool_size
         self.stride = stride if stride is not None else self.pool_size
         self.padding = padding
 
     def __str__(self):
         return f'AveragePooling2D(pool_size={self.pool_size}, stride={self.stride}, padding={self.padding})'
 
     def forward_pass(self, input_data: np.ndarray) -> np.ndarray:
-        assert len(input_data.shape) == 4, f"AveragePooling2D input must be 4D (batch_size, channels, height, width), got {input_data.shape}"
+        assert len(
+            input_data.shape) == 4, f"AveragePooling2D input must be 4D (batch_size, channels, height, width), got {input_data.shape}"
         self.input = input_data
         output = self._pool(self.input, self.pool_size, self.stride, self.padding)
         return output
 
     def backward_pass(self, output_error: np.ndarray) -> np.ndarray:
         input_error = self._pool_backward(output_error, self.input, self.pool_size, self.stride, self.padding)
         return input_error
@@ -877,15 +897,16 @@
                               mode='constant')
 
         d_input = np.zeros_like(padded_input)
 
         for i in range(out_height):
             for j in range(out_width):
                 d_input[:, :, i * stride[0]:i * stride[0] + pool_size[0],
-                j * stride[1]:j * stride[1] + pool_size[1]] += output_error[:, :, i, j][:, :, np.newaxis, np.newaxis] / np.prod(pool_size)
+                j * stride[1]:j * stride[1] + pool_size[1]] += output_error[:, :, i, j][:, :, np.newaxis,
+                                                               np.newaxis] / np.prod(pool_size)
 
         if padding == 'same':
             d_input = d_input[:, :, pad_height:-pad_height, pad_width:-pad_width]
 
         return d_input
 
 
@@ -895,15 +916,16 @@
         self.stride = stride if stride is not None else pool_size
         self.padding = padding
 
     def __str__(self):
         return f'AveragePooling1D(pool_size={self.pool_size}, stride={self.stride}, padding={self.padding})'
 
     def forward_pass(self, input_data: np.ndarray) -> np.ndarray:
-        assert len(input_data.shape) == 3, f"AveragePooling1D input must be 3D (batch_size, steps, features), got {input_data.shape}"
+        assert len(
+            input_data.shape) == 3, f"AveragePooling1D input must be 3D (batch_size, steps, features), got {input_data.shape}"
         self.input = input_data
         output = self._pool(self.input, self.pool_size, self.stride, self.padding)
         return output
 
     def backward_pass(self, output_error: np.ndarray) -> np.ndarray:
         input_error = self._pool_backward(output_error, self.input, self.pool_size, self.stride, self.padding)
         return input_error
@@ -959,27 +981,28 @@
         for i in range(out_steps):
             d_input[:, i * stride:i * stride + pool_size, :] += output_error[:, i, :][:, np.newaxis, :] / pool_size
 
         if padding == 'same':
             d_input = d_input[:, pad_steps:-pad_steps, :]
 
         return d_input
-    
+
 
 # --------------------------------------------------------------------------------------------------------------
 
 
 compatibility_dict = {
     Input: [Dense, Conv2D, Conv1D, Embedding],
     Dense: [Dense, Activation, Dropout, BatchNormalization],
-    Activation: [Dense, Conv2D, Conv1D, MaxPooling2D, AveragePooling2D, MaxPooling1D, AveragePooling1D, Flatten, Dropout],
+    Activation: [Dense, Conv2D, Conv1D, MaxPooling2D, AveragePooling2D, MaxPooling1D, AveragePooling1D, Flatten,
+                 Dropout],
     Conv2D: [Conv2D, MaxPooling2D, AveragePooling2D, Activation, Dropout, Flatten, BatchNormalization],
     MaxPooling2D: [Conv2D, MaxPooling2D, AveragePooling2D, Flatten],
     AveragePooling2D: [Conv2D, MaxPooling2D, AveragePooling2D, Flatten],
     Conv1D: [Conv1D, MaxPooling1D, AveragePooling1D, Activation, Dropout, Flatten, BatchNormalization],
     MaxPooling1D: [Conv1D, MaxPooling1D, AveragePooling1D, Flatten],
     AveragePooling1D: [Conv1D, MaxPooling1D, AveragePooling1D, Flatten],
     Flatten: [Dense, Dropout],
     Dropout: [Dense, Conv2D, Conv1D, Activation],
     Embedding: [Conv1D, Flatten, Dense],
     BatchNormalization: [Dense, Conv2D, Conv1D, Activation]
-}
+}
```

### Comparing `neuralnetlib-2.3.2/neuralnetlib/losses.py` & `neuralnetlib-2.3.3/neuralnetlib/losses.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.2/neuralnetlib/metrics.py` & `neuralnetlib-2.3.3/neuralnetlib/metrics.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.2/neuralnetlib/model.py` & `neuralnetlib-2.3.3/neuralnetlib/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 import time
 
 import numpy as np
 
 from neuralnetlib.layers import Layer, Input, Activation, Dropout, compatibility_dict
 from neuralnetlib.losses import LossFunction, CategoricalCrossentropy
+from neuralnetlib.metrics import accuracy_score
 from neuralnetlib.optimizers import Optimizer
 from neuralnetlib.utils import shuffle, progress_bar
-from neuralnetlib.metrics import accuracy_score
 
 
 class Model:
     def __init__(self):
         self.layers = []
         self.loss_function = None
         self.optimizer = None
@@ -24,27 +24,27 @@
         for i, layer in enumerate(self.layers):
             model_summary += f'Layer {i + 1}: {str(layer)}\n'
         model_summary += '-------------------------------------------------\n'
         model_summary += f'Loss function: {str(self.loss_function)}\n'
         model_summary += f'Optimizer: {str(self.optimizer)}\n'
         model_summary += '-------------------------------------------------\n'
         return model_summary
-    
+
     def summary(self):
         print(str(self))
 
     def add(self, layer: Layer):
         if not self.layers:
             if not isinstance(layer, Input):
                 raise ValueError("The first layer must be an Input layer.")
         else:
             previous_layer = self.layers[-1]
             if type(layer) not in compatibility_dict[type(previous_layer)]:
                 raise ValueError(f"{type(layer).__name__} layer cannot follow {type(previous_layer).__name__} layer.")
-        
+
         self.layers.append(layer)
 
     def compile(self, loss_function: LossFunction, optimizer: Optimizer, verbose: bool = False):
         self.loss_function = loss_function
         self.optimizer = optimizer
         if verbose:
             print(str(self))
@@ -65,15 +65,15 @@
                 error = self.predictions - self.y_true
             else:
                 error = layer.backward_pass(error)
 
             if hasattr(layer, 'weights'):
                 if hasattr(layer, 'd_weights') and hasattr(layer, 'd_bias'):
                     self.optimizer.update(len(self.layers) - 1 - i, layer.weights, layer.d_weights, layer.bias,
-                                        layer.d_bias)
+                                          layer.d_bias)
                 elif hasattr(layer, 'd_weights'):
                     self.optimizer.update(len(self.layers) - 1 - i, layer.weights, layer.d_weights)
 
     def train_on_batch(self, x_batch: np.ndarray, y_batch: np.ndarray) -> float:
         self.y_true = y_batch
         self.predictions = self.forward_pass(x_batch)
         predictions = self.predictions.copy()
@@ -83,28 +83,46 @@
         if error.ndim == 1:
             error = error[:, None]
 
         self.backward_pass(error)
         return loss
 
     def fit(self, x_train: np.ndarray, y_train: np.ndarray, epochs: int, batch_size: int = None,
-            verbose: bool = True, metrics: list = None, random_state: int = None, validation_data: tuple = None):
+            verbose: bool = True, metrics: list = None, random_state: int = None, validation_data: tuple = None,
+            callbacks: list = None):
         """
         Fit the model to the training data.
 
         Args:
             x_train: Training data
             y_train: Training labels
             epochs: Number of epochs to train the model
             batch_size: Number of samples per gradient update
             verbose: Whether to print training progress
             metrics: List of metrics to evaluate the model (functions from neuralnetlib.metrics module)
             random_state: Random seed for shuffling the data
             validation_data: Tuple of validation data and labels
+            callbacks: List of callback objects (e.g., EarlyStopping)
         """
+        
+        if callbacks:
+            callback_metrics = set()
+            for callback in callbacks:
+                if hasattr(callback, 'monitor') and callback.monitor is not None:
+                    callback_metrics.update(callback.monitor)
+
+            if metrics is None:
+                metrics = list(callback_metrics)
+            else:
+                metrics = set(metrics)
+                missing_metrics = callback_metrics - metrics
+                if missing_metrics:
+                    raise ValueError(f"The following metrics to monitor provided in callbacks are not provided in the fit method: {', '.join(str(metric) for metric in missing_metrics)}")
+
+        
         for i in range(epochs):
             start_time = time.time()
 
             # Shuffling the data to avoid overfitting
             x_train_shuffled, y_train_shuffled = shuffle(x_train, y_train, random_state=random_state)
 
             error = 0
@@ -127,41 +145,61 @@
                     if verbose:
                         metrics_str = ''
                         if metrics is not None:
                             for metric in metrics:
                                 metric_value = metric(np.vstack(predictions_list), np.vstack(y_true_list))
                                 metrics_str += f'{metric.__name__}: {metric_value:.4f} - '
                         progress_bar(j / batch_size + 1, num_batches,
-                                     message=f'Epoch {i + 1}/{epochs} - loss: {error / (j / batch_size + 1):.4f} - {metrics_str[:-3]} - {time.time() - start_time:.2f}s')
+                                    message=f'Epoch {i + 1}/{epochs} - loss: {error / (j / batch_size + 1):.4f} - {metrics_str[:-3]} - {time.time() - start_time:.2f}s')
 
                 error /= num_batches
             else:
                 error = self.train_on_batch(x_train, y_train)
                 predictions_list.append(self.predictions)
                 y_true_list.append(y_train)
 
                 if verbose:
                     metrics_str = ''
                     if metrics is not None:
                         for metric in metrics:
                             metric_value = metric(np.vstack(predictions_list), np.vstack(y_true_list))
                             metrics_str += f'{metric.__name__}: {metric_value:.4f} - '
                     progress_bar(1, 1,
-                                 message=f'Epoch {i + 1}/{epochs} - loss: {error:.4f} - {metrics_str[:-3]} - {time.time() - start_time:.2f}s')
+                                message=f'Epoch {i + 1}/{epochs} - loss: {error:.4f} - {metrics_str[:-3]} - {time.time() - start_time:.2f}s')
 
             if validation_data is not None:
                 x_test, y_test = validation_data
                 val_predictions = self.predict(x_test)
                 val_accuracy = accuracy_score(val_predictions, y_test)
                 if verbose:
                     print(f' - val_accuracy: {val_accuracy:.4f}', end='')
 
+            if callbacks:
+                metrics_values = []
+                if metrics is not None:
+                    metrics_values.extend(
+                        [metric(np.vstack(predictions_list), np.vstack(y_true_list)) for metric in metrics])
+                else:
+                    # If no metrics are provided, use the loss value by default
+                    metrics_values.append(error)
+                for callback in callbacks:
+                    if callback.stop_training:
+                        break
+                    if callback.on_epoch_end(self, metrics_values):
+                        break
+
             if verbose:
                 print()
 
+            if any(callback.stop_training for callback in callbacks):
+                break
+
+        if verbose:
+            print()
+
     def evaluate(self, x_test: np.ndarray, y_test: np.ndarray) -> float:
         predictions = self.forward_pass(x_test)
         loss = self.loss_function(y_test, predictions)
         return loss
 
     def predict(self, X: np.ndarray) -> np.ndarray:
         return self.forward_pass(X, training=False)
```

### Comparing `neuralnetlib-2.3.2/neuralnetlib/optimizers.py` & `neuralnetlib-2.3.3/neuralnetlib/optimizers.py`

 * *Files identical despite different names*

### Comparing `neuralnetlib-2.3.2/neuralnetlib/preprocessing.py` & `neuralnetlib-2.3.3/neuralnetlib/preprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,17 +44,17 @@
     if isinstance(stride, int):
         stride_h, stride_w = stride, stride
     else:
         stride_h, stride_w = stride
 
     # Make sure that the convolution can be executed
     assert (
-                       H + 2 * pad_h - filter_h) % stride_h == 0, f'invalid parameters, (H + 2 * pad_h - filter_h) % stride_h != 0, got H={H}, pad_h={pad_h}, filter_h={filter_h}, stride_h={stride_h}'
+                   H + 2 * pad_h - filter_h) % stride_h == 0, f'invalid parameters, (H + 2 * pad_h - filter_h) % stride_h != 0, got H={H}, pad_h={pad_h}, filter_h={filter_h}, stride_h={stride_h}'
     assert (
-                       W + 2 * pad_w - filter_w) % stride_w == 0, f'invalid parameters, (W + 2 * pad_w - filter_w) % stride_w != 0, got W={W}, pad_w={pad_w}, filter_w={filter_w}, stride_w={stride_w}'
+                   W + 2 * pad_w - filter_w) % stride_w == 0, f'invalid parameters, (W + 2 * pad_w - filter_w) % stride_w != 0, got W={W}, pad_w={pad_w}, filter_w={filter_w}, stride_w={stride_w}'
 
     out_h = (H + 2 * pad_h - filter_h) // stride_h + 1
     out_w = (W + 2 * pad_w - filter_w) // stride_w + 1
 
     padded_input = np.pad(input_data, ((0, 0), (0, 0), (pad_h, pad_h), (pad_w, pad_w)), mode='constant')
 
     col = np.zeros((N, C, filter_h, filter_w, out_h, out_w))
@@ -155,17 +155,17 @@
     if isinstance(stride, int):
         stride_h, stride_w = stride, stride
     else:
         stride_h, stride_w = stride
 
     # Make sure that the convolution can be executed
     assert (
-                       H + 2 * pad_h - filter_h) % stride_h == 0, f'invalid parameters, (H + 2 * pad_h - filter_h) % stride_h != 0, got H={H}, pad_h={pad_h}, filter_h={filter_h}, stride_h={stride_h}'
+                   H + 2 * pad_h - filter_h) % stride_h == 0, f'invalid parameters, (H + 2 * pad_h - filter_h) % stride_h != 0, got H={H}, pad_h={pad_h}, filter_h={filter_h}, stride_h={stride_h}'
     assert (
-                       W + 2 * pad_w - filter_w) % stride_w == 0, f'invalid parameters, (W + 2 * pad_w - filter_w) % stride_w != 0, got W={W}, pad_w={pad_w}, filter_w={filter_w}, stride_w={stride_w}'
+                   W + 2 * pad_w - filter_w) % stride_w == 0, f'invalid parameters, (W + 2 * pad_w - filter_w) % stride_w != 0, got W={W}, pad_w={pad_w}, filter_w={filter_w}, stride_w={stride_w}'
 
     out_h = (H + 2 * pad_h - filter_h) // stride_h + 1
     out_w = (W + 2 * pad_w - filter_w) // stride_w + 1
 
     col = col.reshape(N, out_h, out_w, C, filter_h, filter_w).transpose(0, 3, 4, 5, 1, 2)
 
     image = np.zeros((N, C, H + 2 * pad_h + stride_h - 1, W + 2 * pad_w + stride_w - 1))
@@ -223,16 +223,16 @@
         self.fit(X)
         return self.transform(X)
 
     def inverse_transform(self, X):
         if self.mean_ is None or self.scale_ is None:
             raise ValueError("StandardScaler has not been fitted yet.")
         return X * self.scale_ + self.mean_
-    
-    
+
+
 class MinMaxScaler:
     def __init__(self, feature_range=(0, 1)):
         self.feature_range = feature_range
         self.min_ = None
         self.scale_ = None
 
     def fit(self, X):
```

### Comparing `neuralnetlib-2.3.2/neuralnetlib/utils.py` & `neuralnetlib-2.3.3/neuralnetlib/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -59,8 +59,8 @@
     """
     rng = np.random.default_rng(random_state if random_state is not None else int(time.time_ns()))
     indices = np.arange(len(x))
     rng.shuffle(indices)
     split_index = int(len(x) * (1 - test_size))
     x_train, x_test = x[indices[:split_index]], x[indices[split_index:]]
     y_train, y_test = y[indices[:split_index]], y[indices[split_index:]]
-    return x_train, x_test, y_train, y_test
+    return x_train, x_test, y_train, y_test
```

### Comparing `neuralnetlib-2.3.2/neuralnetlib.egg-info/PKG-INFO` & `neuralnetlib-2.3.3/neuralnetlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralnetlib
-Version: 2.3.2
+Version: 2.3.3
 Summary: A simple convolutional neural network library with only numpy as dependency
 Home-page: https://github.com/marcpinet/handmade-neuralnetwork
 Author: Marc Pinet
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `neuralnetlib-2.3.2/setup.py` & `neuralnetlib-2.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='neuralnetlib',
-    version='2.3.2',
+    version='2.3.3',
     author='Marc Pinet',
     description='A simple convolutional neural network library with only numpy as dependency',
     long_description=open('README.md', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     url='https://github.com/marcpinet/handmade-neuralnetwork',
     packages=find_packages(),
     install_requires=[
```

