# Comparing `tmp/keras_generators-1.4.2-py3-none-any.whl.zip` & `tmp/keras_generators-1.4.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 29153 bytes, number of entries: 16
+Zip file size: 29702 bytes, number of entries: 16
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-08 16:27 examples/__init__.py
 -rw-rw-rw-  2.0 fat     6233 b- defN 23-Apr-13 14:38 examples/predict_stock_price.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-08 16:27 keras_generators/__init__.py
--rw-rw-rw-  2.0 fat     4298 b- defN 24-Apr-22 22:11 keras_generators/callbacks.py
--rw-rw-rw-  2.0 fat      803 b- defN 24-Apr-22 16:08 keras_generators/common.py
+-rw-rw-rw-  2.0 fat     6339 b- defN 24-Apr-23 14:52 keras_generators/callbacks.py
+-rw-rw-rw-  2.0 fat      782 b- defN 24-Apr-23 14:50 keras_generators/common.py
 -rw-rw-rw-  2.0 fat    10842 b- defN 23-Mar-08 16:27 keras_generators/encoders.py
 -rw-rw-rw-  2.0 fat    36073 b- defN 24-Apr-22 16:04 keras_generators/generators.py
 -rw-rw-rw-  2.0 fat     4139 b- defN 23-Mar-08 19:39 keras_generators/splitters.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Mar-08 16:27 keras_generators/model_abstractions/__init__.py
 -rw-rw-rw-  2.0 fat     8063 b- defN 23-Dec-01 13:36 keras_generators/model_abstractions/model_object.py
 -rw-rw-rw-  2.0 fat     3263 b- defN 24-Apr-22 14:58 keras_generators/model_abstractions/model_params.py
--rw-rw-rw-  2.0 fat    11558 b- defN 24-Apr-22 22:18 keras_generators-1.4.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    13558 b- defN 24-Apr-22 22:18 keras_generators-1.4.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-22 22:18 keras_generators-1.4.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       26 b- defN 24-Apr-22 22:18 keras_generators-1.4.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1422 b- defN 24-Apr-22 22:18 keras_generators-1.4.2.dist-info/RECORD
-16 files, 100370 bytes uncompressed, 26767 bytes compressed:  73.3%
+-rw-rw-rw-  2.0 fat    11558 b- defN 24-Apr-23 14:53 keras_generators-1.4.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    13741 b- defN 24-Apr-23 14:53 keras_generators-1.4.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-23 14:53 keras_generators-1.4.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       26 b- defN 24-Apr-23 14:53 keras_generators-1.4.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1422 b- defN 24-Apr-23 14:53 keras_generators-1.4.3.dist-info/RECORD
+16 files, 102573 bytes uncompressed, 27316 bytes compressed:  73.4%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: keras_generators/model_abstractions/model_object.py
 Comment: 
 
 Filename: keras_generators/model_abstractions/model_params.py
 Comment: 
 
-Filename: keras_generators-1.4.2.dist-info/LICENSE
+Filename: keras_generators-1.4.3.dist-info/LICENSE
 Comment: 
 
-Filename: keras_generators-1.4.2.dist-info/METADATA
+Filename: keras_generators-1.4.3.dist-info/METADATA
 Comment: 
 
-Filename: keras_generators-1.4.2.dist-info/WHEEL
+Filename: keras_generators-1.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: keras_generators-1.4.2.dist-info/top_level.txt
+Filename: keras_generators-1.4.3.dist-info/top_level.txt
 Comment: 
 
-Filename: keras_generators-1.4.2.dist-info/RECORD
+Filename: keras_generators-1.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## keras_generators/callbacks.py

```diff
@@ -1,17 +1,19 @@
 import json
 import logging
 import math
 from json import JSONEncoder
 from pathlib import Path
 from typing import Optional
 
+import dill
 import numpy as np
 from tensorflow.python.util.tf_export import keras_export
 from tf_keras.callbacks import Callback, CSVLogger, ReduceLROnPlateau, TensorBoard
+from typing_extensions import Self, override
 
 from keras_generators.common import SerializableKerasObject
 
 
 class EarlyStoppingAtMinLoss(Callback, SerializableKerasObject):
     """Stop training when the loss is at its min, i.e. the loss stops decreasing.
 
@@ -113,13 +115,67 @@
 @keras_export("keras.callbacks.SerializableReduceLROnPlateau")
 class SerializableReduceLROnPlateau(ReduceLROnPlateau, SerializableKerasObject):
     pass
 
 
 @keras_export("keras.callbacks.SerializableTensorBoard")
 class SerializableTensorBoard(TensorBoard, SerializableKerasObject):
-    pass
+    @override
+    def serialize(self) -> bytes:
+        kwargs = {
+            "log_dir": self.log_dir,
+            "histogram_freq": self.histogram_freq,
+            "write_graph": self.write_graph,
+            "write_images": self.write_images,
+            "write_steps_per_second": self.write_steps_per_second,
+            "update_freq": self.update_freq,
+            # "profile_batch" we ignore this parameter as it's not directly saved on the object
+            "embeddings_freq": self.embeddings_freq,
+            "embeddings_metadata": self.embeddings_metadata,
+        }
+        all_state_attrs = self.__dict__.copy()
+        excepted_attrs = set(kwargs.keys()) | {"_writers"}
+        for attr in excepted_attrs:
+            del all_state_attrs[attr]
+
+        return dill.dumps((kwargs, all_state_attrs))
+
+    @override
+    @classmethod
+    def deserialize(cls, buffer: bytes) -> Self:
+        kwargs, state_attrs = dill.loads(buffer)
+        instance = cls(**kwargs)
+        for attr, val in state_attrs.items():
+            setattr(instance, attr, val)
+        return instance
 
 
 @keras_export("keras.callbacks.SerializableCSVLogger")
 class SerializableCSVLogger(CSVLogger, SerializableKerasObject):
-    pass
+    def serialize(self) -> bytes:
+        """
+        self.sep = separator
+        self.filename = io_utils.path_to_string(filename)
+        self.append = append
+
+        :return:
+        """
+        kwargs = {
+            "separator": self.sep,
+            "filename": self.filename,
+            "append": self.append,
+        }
+        all_state_attrs = self.__dict__.copy()
+        excepted_attrs = {"sep", "filename", "append"} | {"writer", "csv_file"}
+        for attr in excepted_attrs:
+            del all_state_attrs[attr]
+
+        return dill.dumps((kwargs, all_state_attrs))
+
+    @override
+    @classmethod
+    def deserialize(cls, buffer: bytes) -> Self:
+        kwargs, state_attrs = dill.loads(buffer)
+        instance = cls(**kwargs)
+        for attr, val in state_attrs.items():
+            setattr(instance, attr, val)
+        return instance
```

## keras_generators/common.py

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # Author: ASU --<andrei.suiu@gmail.com>
 
 from json import JSONEncoder
 
-import cloudpickle
+import dill
 import numpy as np
 from pydantic import Extra
 
 
 class NumpyArrayEncoder(JSONEncoder):
     def default(self, o):
         if isinstance(o, np.ndarray):
@@ -23,13 +23,13 @@
 
 class ArbitraryTypes:
     arbitrary_types_allowed = True
 
 
 class SerializableKerasObject:
     def serialize(self) -> bytes:
-        pickled = cloudpickle.dumps(self)
+        pickled = dill.dumps(self)
         return pickled
 
     @classmethod
     def deserialize(cls, buffer: bytes) -> "SerializableKerasObject":
-        return cloudpickle.loads(buffer)
+        return dill.loads(buffer)
```

## Comparing `keras_generators-1.4.2.dist-info/LICENSE` & `keras_generators-1.4.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `keras_generators-1.4.2.dist-info/METADATA` & `keras_generators-1.4.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-generators
-Version: 1.4.2
+Version: 1.4.3
 Summary: Multi-dimensional/Multi-input/Multi-output Data preprocessing and Batch Generators for Keras models
 Home-page: https://github.com/asuiu/keras-generators
 Author: Andrei Suiu
 Author-email: andrei.suiu@gmail.com
 License: Apache License 2.0
 Keywords: ML,DataGenerators,Keras,tensorflow
 Classifier: Intended Audience :: Developers
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: cloudpickle >=3.0.0
+Requires-Dist: dill >=0.3.8
 Requires-Dist: numpy >=1.20
 Requires-Dist: pip >=22.1.2
 Requires-Dist: pydantic >=2.0
 Requires-Dist: pyxtension >=1.15.0
 Requires-Dist: scikit-learn >=0.22.2
 Requires-Dist: setuptools >=63.4.1
 Requires-Dist: tensorflow >=2.16
@@ -181,14 +181,18 @@
 res_ds = TensorDataSource(name="prediction", tensors=y_pred, encoders=targets_ds.get_encoders())
 unscaled_y_pred = res_ds.decode()[:]
 ```
 
 # Changelog
 
 All notable changes to this project will be documented in this file.
+## [1.4.3] - 2024-04-23
+- fix callbacks to work on TF 2.16
+- added integration tests for callbacks.py module
+- using dill serializer instead of pickle for serialization of the Callbacks
 
 ## [1.4.2] - 2024-04-22
 - Drops support <3.10 in setup.py
 - Upgrade ModelParams to use pydantic>=2.*
 - Proper serialization of Callbacks using cloudpickle + dependency on cloudpickle
 - Added common SerializableKerasObject
 - Use legacy Keras (2.*) instead of the new 3.0 by explicitly importing tf_keras lib
```

## Comparing `keras_generators-1.4.2.dist-info/RECORD` & `keras_generators-1.4.3.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 examples/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 examples/predict_stock_price.py,sha256=OLhlvKkctYf12kGk7QgxSWKVWM61EI6r0NzXwSKOuAY,6233
 keras_generators/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-keras_generators/callbacks.py,sha256=veerVJoKbnLwNjYI7uSWHxHqTokudY00USxkD5_Mr64,4298
-keras_generators/common.py,sha256=dD1g27em-9aBGpjxlepTLN7rLxBDytXnVB-n1UrnOQw,803
+keras_generators/callbacks.py,sha256=mY93NxalXmLDjZ_Fjqv9SYcXjQUjUdPA8I5G0hun7_o,6339
+keras_generators/common.py,sha256=B3V2ypF3sGQtNJK-SB1RXvNlKVYKjjQCybOZvtSgyYA,782
 keras_generators/encoders.py,sha256=WwviJAdT_mYwjSIn9wqzt3-DEjLNl7jbliKC2jjlYik,10842
 keras_generators/generators.py,sha256=ZZXh0c4RPzKui0n-VVvvJQesmhc4ZRu3KIo_MqK0NMU,36073
 keras_generators/splitters.py,sha256=O7AKehcoPiQNjv1kuZWOoax-yvnjTFPuOkwLjox-qMw,4139
 keras_generators/model_abstractions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 keras_generators/model_abstractions/model_object.py,sha256=TkkAcMJQ6S9Onzueret5xNwMZN0eLqqtocbpZEkUZxs,8063
 keras_generators/model_abstractions/model_params.py,sha256=114iJ1gi15XEUhhU5vZnBgvfL1GY2ozhEsIiXf7rwTE,3263
-keras_generators-1.4.2.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-keras_generators-1.4.2.dist-info/METADATA,sha256=QRkbwsc0gJhPHBEQ_w6Mu5VbnduYezy1ai3_yclVNmA,13558
-keras_generators-1.4.2.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-keras_generators-1.4.2.dist-info/top_level.txt,sha256=6h3qtPKTpHlh7dFVHfOuDDRxVzXpjgb3hL-O3LMXK2w,26
-keras_generators-1.4.2.dist-info/RECORD,,
+keras_generators-1.4.3.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+keras_generators-1.4.3.dist-info/METADATA,sha256=9QULxMIcErgJFhREwGhU0qLUBo1PdPvkQeaz0OjkLtA,13741
+keras_generators-1.4.3.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+keras_generators-1.4.3.dist-info/top_level.txt,sha256=6h3qtPKTpHlh7dFVHfOuDDRxVzXpjgb3hL-O3LMXK2w,26
+keras_generators-1.4.3.dist-info/RECORD,,
```

