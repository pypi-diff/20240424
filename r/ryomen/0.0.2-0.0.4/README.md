# Comparing `tmp/ryomen-0.0.2.tar.gz` & `tmp/ryomen-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryomen-0.0.2.tar", last modified: Tue Apr 16 15:40:32 2024, max compression
+gzip compressed data, was "ryomen-0.0.4.tar", last modified: Tue Apr 23 23:02:40 2024, max compression
```

## Comparing `ryomen-0.0.2.tar` & `ryomen-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-16 15:40:32.573307 ryomen-0.0.2/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)     5481 2024-04-16 15:40:32.573218 ryomen-0.0.2/PKG-INFO
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-16 15:40:32.571179 ryomen-0.0.2/ryomen/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)       31 2024-04-15 17:56:53.000000 ryomen-0.0.2/ryomen/__init__.py
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)    12999 2024-04-16 14:21:26.000000 ryomen-0.0.2/ryomen/main.py
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-16 15:40:32.572421 ryomen-0.0.2/ryomen.egg-info/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)     5481 2024-04-16 15:40:32.000000 ryomen-0.0.2/ryomen.egg-info/PKG-INFO
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)      218 2024-04-16 15:40:32.000000 ryomen-0.0.2/ryomen.egg-info/SOURCES.txt
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)        1 2024-04-16 15:40:32.000000 ryomen-0.0.2/ryomen.egg-info/dependency_links.txt
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)        7 2024-04-16 15:40:32.000000 ryomen-0.0.2/ryomen.egg-info/top_level.txt
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)        1 2024-04-16 13:55:45.000000 ryomen-0.0.2/ryomen.egg-info/zip-safe
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)      260 2024-04-16 15:40:32.573650 ryomen-0.0.2/setup.cfg
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)      396 2024-04-16 14:03:09.000000 ryomen-0.0.2/setup.py
-drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-16 15:40:32.572763 ryomen-0.0.2/tests/
--rw-r--r--   0 chrisbuswinka   (501) staff       (20)     7377 2024-04-16 14:15:13.000000 ryomen-0.0.2/tests/test_ryomen.py
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-23 23:02:40.149716 ryomen-0.0.4/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)     1064 2024-04-16 15:51:46.000000 ryomen-0.0.4/LICENSE
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)     5654 2024-04-23 23:02:40.149616 ryomen-0.0.4/PKG-INFO
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-23 23:02:40.147634 ryomen-0.0.4/ryomen/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)       31 2024-04-15 17:56:53.000000 ryomen-0.0.4/ryomen/__init__.py
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)    22085 2024-04-23 22:57:56.000000 ryomen-0.0.4/ryomen/main.py
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-23 23:02:40.148735 ryomen-0.0.4/ryomen.egg-info/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)     5654 2024-04-23 23:02:40.000000 ryomen-0.0.4/ryomen.egg-info/PKG-INFO
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)      226 2024-04-23 23:02:40.000000 ryomen-0.0.4/ryomen.egg-info/SOURCES.txt
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)        1 2024-04-23 23:02:40.000000 ryomen-0.0.4/ryomen.egg-info/dependency_links.txt
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)        7 2024-04-23 23:02:40.000000 ryomen-0.0.4/ryomen.egg-info/top_level.txt
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)        1 2024-04-16 13:55:45.000000 ryomen-0.0.4/ryomen.egg-info/zip-safe
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)      260 2024-04-23 23:02:40.150035 ryomen-0.0.4/setup.cfg
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)      396 2024-04-16 14:03:09.000000 ryomen-0.0.4/setup.py
+drwxr-xr-x   0 chrisbuswinka   (501) staff       (20)        0 2024-04-23 23:02:40.148985 ryomen-0.0.4/tests/
+-rw-r--r--   0 chrisbuswinka   (501) staff       (20)     8560 2024-04-17 20:42:38.000000 ryomen-0.0.4/tests/test_ryomen.py
```

### Comparing `ryomen-0.0.2/PKG-INFO` & `ryomen-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: ryomen
-Version: 0.0.2
+Version: 0.0.4
 Summary: Ryomen
 Home-page: https://github.com/buswinka/ryomen
 Author: Chris Buswinka
 Author-email: buswinka@g.harvard.edu
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Ryomen
 ## For slicing up large microscopy images
 
 Ryomen is a lightweight, no dependency utility for working with large biological microscopy images. 
 
 
@@ -46,20 +47,20 @@
 
 ```python
 import skimage.io as io
 import numpy as np
 import zarr
 from ryomen import Slicer
 
-image = io.imread("really_huge_8bit_3d_image.tif")  # Shape of [3, 10000, 10000] 
-c, x, y, z = image.shape
+image = io.imread("really_huge_8bit_2d_image.tif")  # Shape of [3, 10000, 10000] 
+c, x, y = image.shape
 output: zarr.Array = zarr.open(
     'really_huge_output_on_disk.zarr',
     mode="w",
-    shape=(c, x, y, z),
+    shape=(c, x, y),
     dtype="|f2",
 )
 
 expensive_fn = lambda x: x + 1  # might be a ML model, or anything else
 
 crop_size = (512, 512)
 overlap = (64, 64)
@@ -70,15 +71,15 @@
     
     # Slot the crop into an output array, excluding the overlap
     output[destination] = crop[source]  
 
 ```
 
 You can apply arbitrary functions to a crop after it has been extracted from the large image. This is useful for working 
-with a large uint8 image that might need to be a cast to float for a ML model. 
+with a large uint8 image that might need to be cast to float for a ML model. 
 
 ```python
 import skimage.io as io
 import numpy as np
 import zarr
 from ryomen import Slicer
 
@@ -140,21 +141,29 @@
 slices = Slicer(image, 
                 crop_size=crop_size, 
                 overlap=overlap, 
                 output_transform=output_transform, 
                 batch_size=64,
                 collate=collate)
 
-pytorch_model = lambda x: nn.Conv2d(3, 1, kernel_size=3)
+pytorch_model = lambda x: nn.Conv3d(3, 1, kernel_size=3)
 
 for crop, source, destination in slices:
     assert crop.ndim == 4  # crop shape is -> [B=64, 3, 512, 512]
     
     # Run the expensive fn on a crop of the whole image
     crop = pytorch_model(crop)
     
     # Slot the batched crop into an output array, excluding the overlap
     for b, (_source, _destination) in enumerate(zip(source, destination)):
         output[_destination] = crop[b, ...][_source]  
 ```
 
-Ryomen is names after the first name of the main antagonist of JJK who slices up everything.
+### Change Log
+#### 0.0.4
+    - padding now works with pure indexing, for reflections. Tested up to 3D with numpy. 
+
+
+#### 0.0.3
+    - First working version
+
+Ryomen is titled after the first name of the main antagonist of JJK who slices up everything.
```

### Comparing `ryomen-0.0.2/ryomen.egg-info/PKG-INFO` & `ryomen-0.0.4/ryomen.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: ryomen
-Version: 0.0.2
+Version: 0.0.4
 Summary: Ryomen
 Home-page: https://github.com/buswinka/ryomen
 Author: Chris Buswinka
 Author-email: buswinka@g.harvard.edu
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Ryomen
 ## For slicing up large microscopy images
 
 Ryomen is a lightweight, no dependency utility for working with large biological microscopy images. 
 
 
@@ -46,20 +47,20 @@
 
 ```python
 import skimage.io as io
 import numpy as np
 import zarr
 from ryomen import Slicer
 
-image = io.imread("really_huge_8bit_3d_image.tif")  # Shape of [3, 10000, 10000] 
-c, x, y, z = image.shape
+image = io.imread("really_huge_8bit_2d_image.tif")  # Shape of [3, 10000, 10000] 
+c, x, y = image.shape
 output: zarr.Array = zarr.open(
     'really_huge_output_on_disk.zarr',
     mode="w",
-    shape=(c, x, y, z),
+    shape=(c, x, y),
     dtype="|f2",
 )
 
 expensive_fn = lambda x: x + 1  # might be a ML model, or anything else
 
 crop_size = (512, 512)
 overlap = (64, 64)
@@ -70,15 +71,15 @@
     
     # Slot the crop into an output array, excluding the overlap
     output[destination] = crop[source]  
 
 ```
 
 You can apply arbitrary functions to a crop after it has been extracted from the large image. This is useful for working 
-with a large uint8 image that might need to be a cast to float for a ML model. 
+with a large uint8 image that might need to be cast to float for a ML model. 
 
 ```python
 import skimage.io as io
 import numpy as np
 import zarr
 from ryomen import Slicer
 
@@ -140,21 +141,29 @@
 slices = Slicer(image, 
                 crop_size=crop_size, 
                 overlap=overlap, 
                 output_transform=output_transform, 
                 batch_size=64,
                 collate=collate)
 
-pytorch_model = lambda x: nn.Conv2d(3, 1, kernel_size=3)
+pytorch_model = lambda x: nn.Conv3d(3, 1, kernel_size=3)
 
 for crop, source, destination in slices:
     assert crop.ndim == 4  # crop shape is -> [B=64, 3, 512, 512]
     
     # Run the expensive fn on a crop of the whole image
     crop = pytorch_model(crop)
     
     # Slot the batched crop into an output array, excluding the overlap
     for b, (_source, _destination) in enumerate(zip(source, destination)):
         output[_destination] = crop[b, ...][_source]  
 ```
 
-Ryomen is names after the first name of the main antagonist of JJK who slices up everything.
+### Change Log
+#### 0.0.4
+    - padding now works with pure indexing, for reflections. Tested up to 3D with numpy. 
+
+
+#### 0.0.3
+    - First working version
+
+Ryomen is titled after the first name of the main antagonist of JJK who slices up everything.
```

### Comparing `ryomen-0.0.2/tests/test_ryomen.py` & `ryomen-0.0.4/tests/test_ryomen.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,98 @@
 import pytest
 from ryomen.main import Slicer, _nd_generator
 import numpy as np
 
 
+def test_that_nd_gen_finishes():
+    max = 10000
+    counter = 0
+    for ind, xyz in _nd_generator(
+        crop=[10, 10, 10], overlap=[2, 2, 2], shape=(100, 100, 10), pad=False
+    ):
+        counter += 1
+        assert counter < max
+
+    # now do it with padding
+    max = 10000
+    counter = 0
+    for ind, xyz in _nd_generator(
+        crop=[10, 10, 10], overlap=[2, 2, 2], shape=(100, 100, 10), pad=True
+    ):
+        counter += 1
+        assert counter < max
+
+
 def test_non_array_input():
     with pytest.raises(ValueError):
-        Slicer(image=[[1,2,3,4], [1,2,3,4, 5], [1, 2, 3, 4, 5]], crop_size=(2,), overlap=(0,0))
-
+        Slicer(
+            image=[[1, 2, 3, 4], [1, 2, 3, 4, 5], [1, 2, 3, 4, 5]],
+            crop_size=(2,),
+            overlap=(0, 0),
+        )
 
 
 def test_total_3d_ind_coverage():
     image = np.zeros((100, 100, 10))
     for ind, xyz in _nd_generator(
-        crop=[10, 10, 10], overlap=[2, 2, 2], shape=image.shape
+        crop=[10, 10, 10], overlap=[2, 2, 2], shape=image.shape, pad=False
     ):
         image[tuple(ind)] = 1
     assert np.all(image == 1)
 
 
 def test_total_2d_ind_coverage():
 
     image = np.zeros((100, 100))
-    for ind, xyz in _nd_generator(crop=[30, 30], overlap=[10, 10], shape=image.shape):
+    for ind, xyz in _nd_generator(
+        crop=[30, 30], overlap=[10, 10], shape=image.shape, pad=False
+    ):
         image[tuple(ind)] = 1
     assert np.all(image == 1)
 
 
 def test_total_5d_ind_coverage():
 
     image = np.zeros((30, 30, 30, 30, 30))
     for ind, xyz in _nd_generator(
-        crop=[10, 10, 10, 10, 10], overlap=[2,] * 5, shape=image.shape
+        crop=[10, 10, 10, 10, 10], overlap=[2,] * 5, shape=image.shape, pad=False
     ):
         image[tuple(ind)] = 1
     assert np.all(image == 1)
 
+
 def test_source_destination():
     image = np.random.randn(1, 100, 100, 100)
     output = np.random.randn(1, 100, 100, 100)
     crop = (10, 10, 10)
     overlap = [2, 2, 2]
 
     crop_iterator = Slicer(image, crop_size=crop, overlap=overlap)
     for crop, source, destination in crop_iterator:
         a = output[destination]
         b = crop[source]
         assert a.shape == b.shape, source
 
+
 def test_all_crops_same_size():
     image = np.random.randn(100, 100, 100)
     output = np.random.randn(100, 100, 100)
     cropsize = (10, 10, 10)
     overlap = [2, 2, 2]
 
     def same_size(t1, t2):
         return all(a == b for a, b in zip(t1, t2))
 
     crop_iterator = Slicer(image, crop_size=cropsize, overlap=overlap)
     crops = []
     for crop, source, destination in crop_iterator:
         crops.append(crop)
-    assert all([same_size(c.shape, cropsize) for c in crops]), f'{source=}, {destination=}'
+    assert all(
+        [same_size(c.shape, cropsize) for c in crops]
+    ), f"{source=}, {destination=}"
 
 
 def test_nonfunctional_runtime():
     image = np.random.randn(1, 100, 100, 100)
     crop = (10, 10, 10)
     overlap = [2, 2, 2]
 
@@ -118,17 +146,16 @@
     output = np.empty_like(image)
     crop = (5, 5, 5)
     overlap = [0, 0, 0]
 
     crop_iterator = Slicer(image, crop_size=crop, overlap=overlap)
     for crop, source, destination in crop_iterator:
         output[destination] = crop[source]
-    
-    assert np.allclose(image, output)
 
+    assert np.allclose(image, output)
 
 
 def test_strangely_large_crop():
     image = np.random.randn(1, 100, 100, 100)
     crop = (1000, 1000, 1000)
     overlap = [10, 10, 10]
 
@@ -154,14 +181,15 @@
     with pytest.raises(TypeError):
         Slicer(image, (10, 10, 10), (2, 2, 2), batch_size=float("inf"))
     with pytest.raises(TypeError):
         Slicer(image, (10, 10, 10), (2, 2, 2), batch_size=float("nan"))
     with pytest.raises(TypeError):
         Slicer(image, (10, 10, 10), (2, 2, 2), batch_size=0.2)
 
+
 def test_batch_size():
     image = np.random.randn(100, 100, 90)
     output = np.empty_like(image)
     crop = (10, 10, 10)
     overlap = [0, 0, 0]
 
     crop_iterator = Slicer(image, crop_size=crop, overlap=overlap, batch_size=10)
@@ -173,34 +201,60 @@
     image = np.random.randn(100, 100, 90)
     output = np.empty_like(image)
     crop = (10, 10, 10)
     overlap = [0, 0, 0]
 
     collate = lambda x: np.stack(x, axis=0)
 
-    crop_iterator = Slicer(image, crop_size=crop, overlap=overlap, collate=collate, batch_size=10)
+    crop_iterator = Slicer(
+        image, crop_size=crop, overlap=overlap, collate=collate, batch_size=10
+    )
     for crop, source, destination in crop_iterator:
         assert crop.shape[0] == 10
 
 
 def test_batched_source_destination_agreement():
     image = np.random.randn(20, 10, 10)
     output = np.empty_like(image)
     crop = (10, 10, 10)
     overlap = [0, 0, 0]
 
     def fn(x):
         return x * 100 - 3
 
-    crop_iterator = Slicer(image, crop_size=crop, overlap=overlap, output_transform=fn, batch_size=10)
+    crop_iterator = Slicer(
+        image, crop_size=crop, overlap=overlap, output_transform=fn, batch_size=10
+    )
     for crop, source, destination in crop_iterator:
         for _crop, _source, _destination in zip(crop, source, destination):
             output[_destination] = _crop[_source]
             assert np.allclose(_crop[_source], image[_destination] * 100 - 3)
 
+
+def test_batched_source_destination_agreement_with_pad():
+    image = np.random.randn(20, 10, 10)
+    output = np.empty_like(image)
+    crop = (10, 10, 10)
+    overlap = [2, 2, 2]
+
+    def fn(x):
+        return x * 100 - 3
+
+    crop_iterator = Slicer(
+        image,
+        crop_size=crop,
+        overlap=overlap,
+        output_transform=fn,
+        batch_size=10,
+        pad=True,
+    )
+    for crop, source, destination in crop_iterator:
+        for _crop, _source, _destination in zip(crop, source, destination):
+            output[_destination] = _crop[_source]
+
     assert np.allclose((image * 100) - 3, output)
 
 
 def test_src_dest_zero_overlap():
     image = np.random.randn(20, 100, 100)
     output = np.empty_like(image)
     crop = (10, 10, 10)
@@ -208,14 +262,15 @@
 
     crop_iterator = Slicer(image, crop_size=crop, overlap=overlap)
     for crop, source, destination in crop_iterator:
         output[destination] = crop[source]
 
     assert np.allclose(image, output)
 
+
 def test_source_destination_identity_agreement():
     import numpy as np
 
     image = np.random.randn(20, 10, 10)
     output = np.empty_like(image)
     crop = (10, 10, 10)
     overlap = [0, 0, 0]
@@ -224,22 +279,23 @@
         return x
 
     crop_iterator = Slicer(image, crop_size=crop, overlap=overlap, output_transform=fn)
     for crop, source, destination in crop_iterator:
         output[destination] = crop[source]
         assert np.allclose(crop[source], image[destination])
 
+
 def test_output_fn():
     image = np.random.randn(20, 10, 10)
     output = np.empty_like(image)
     crop = (10, 10, 10)
     overlap = [0, 0, 0]
 
     def fn(x):
         return x * 100 - 3
 
     crop_iterator = Slicer(image, crop_size=crop, overlap=overlap, output_transform=fn)
     for crop, source, destination in crop_iterator:
         output[destination] = crop[source]
         assert np.allclose(crop[source], image[destination] * 100 - 3)
 
-    assert np.allclose((image * 100) - 3, output)
+    assert np.allclose((image * 100) - 3, output)
```

