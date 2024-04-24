# Comparing `tmp/imgmagic-0.2.7-py3-none-any.whl.zip` & `tmp/imgmagic-0.2.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 11379 bytes, number of entries: 11
+Zip file size: 11385 bytes, number of entries: 11
 -rw-rw-r--  2.0 unx      393 b- defN 24-Apr-23 09:22 imgmagic/__init__.py
 -rw-rw-r--  2.0 unx      673 b- defN 24-Apr-15 08:54 imgmagic/colors.py
 -rw-rw-r--  2.0 unx     1446 b- defN 24-Apr-15 08:54 imgmagic/display.py
 -rw-rw-r--  2.0 unx    11895 b- defN 24-Apr-21 13:26 imgmagic/filter.py
 -rw-rw-r--  2.0 unx    13009 b- defN 24-Apr-23 11:14 imgmagic/fourier.py
 -rw-rw-r--  2.0 unx     3987 b- defN 24-Apr-15 08:54 imgmagic/geometric.py
 -rw-rw-r--  2.0 unx     4352 b- defN 24-Apr-15 08:54 imgmagic/histogram.py
--rw-rw-r--  2.0 unx    11005 b- defN 24-Apr-24 13:44 imgmagic-0.2.7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-24 13:44 imgmagic-0.2.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 24-Apr-24 13:44 imgmagic-0.2.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      837 b- defN 24-Apr-24 13:44 imgmagic-0.2.7.dist-info/RECORD
-11 files, 47698 bytes uncompressed, 9985 bytes compressed:  79.1%
+-rw-rw-r--  2.0 unx    11075 b- defN 24-Apr-24 13:46 imgmagic-0.2.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-24 13:46 imgmagic-0.2.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 24-Apr-24 13:46 imgmagic-0.2.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      837 b- defN 24-Apr-24 13:46 imgmagic-0.2.8.dist-info/RECORD
+11 files, 47768 bytes uncompressed, 9991 bytes compressed:  79.1%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: imgmagic/geometric.py
 Comment: 
 
 Filename: imgmagic/histogram.py
 Comment: 
 
-Filename: imgmagic-0.2.7.dist-info/METADATA
+Filename: imgmagic-0.2.8.dist-info/METADATA
 Comment: 
 
-Filename: imgmagic-0.2.7.dist-info/WHEEL
+Filename: imgmagic-0.2.8.dist-info/WHEEL
 Comment: 
 
-Filename: imgmagic-0.2.7.dist-info/top_level.txt
+Filename: imgmagic-0.2.8.dist-info/top_level.txt
 Comment: 
 
-Filename: imgmagic-0.2.7.dist-info/RECORD
+Filename: imgmagic-0.2.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `imgmagic-0.2.7.dist-info/METADATA` & `imgmagic-0.2.8.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgmagic
-Version: 0.2.7
+Version: 0.2.8
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Requires-Dist: numpy (>=1.23.4)
 Requires-Dist: scipy (>=1.11.4)
@@ -30,25 +30,25 @@
 
 im = Image.fromarray(img2)
 im.save("new.jpeg")
 ```
 
 ### Documentation
 
-imgmagic.display.greyscale(x: numpy.ndarray)<br />
+**imgmagic.display.greyscale(x: numpy.ndarray)**<br />
 Function that converts image into greyscale.<br />
 &emsp;&emsp; **Parameters**:<br />
 &emsp;&emsp;&emsp;&emsp; **x : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Image to convert.<br />
 &emsp;&emsp; **Returns**:<br />
 &emsp;&emsp;&emsp;&emsp; **output : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Returns the greyscale image.<br />
 
 
-imgmagic.geometric.crop(img:numpy.ndarray, x:Tuple[int], width:int, height:int)<br />
+**imgmagic.geometric.crop(img:numpy.ndarray, x:Tuple[int], width:int, height:int)**<br />
  Function that crops an image.<br />
 &emsp;&emsp; **Parameters**:<br />
 &emsp;&emsp;&emsp;&emsp; **img : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Image to crop.<br />
 &emsp;&emsp;&emsp;&emsp; **x : Tuple[int]**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Coordiates of starting point.<br />
 &emsp;&emsp;&emsp;&emsp; **width : int**<br />
@@ -56,107 +56,107 @@
 &emsp;&emsp;&emsp;&emsp; **height : int**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Height of the cropped image.<br />
 &emsp;&emsp; **Returns**:<br />
 &emsp;&emsp;&emsp;&emsp; **output : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Cropped image.<br />
 
     
-imgmagic.geometric.rotate(img:numpy.ndarray, degree:float)<br />
+**imgmagic.geometric.rotate(img:numpy.ndarray, degree:float)**<br />
 Function that rotates an image.<br />
 &emsp;&emsp; **Parameters**:<br />
 &emsp;&emsp;&emsp;&emsp; **img : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Image to rotate.<br />
 &emsp;&emsp;&emsp;&emsp; **degree : int**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Angle of rotaion (degrees). This parameter can be positive or negative.<br />
 &emsp;&emsp; **Returns**:<br />
 &emsp;&emsp;&emsp;&emsp; **output : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Rotated image.<br />
 
-imgmagic.geometric.flipping(img:numpy.ndarray)<br />
+**imgmagic.geometric.flipping(img:numpy.ndarray)**<br />
 Function that flips an image.<br />
 &emsp;&emsp; **Parameters**:<br />
 &emsp;&emsp;&emsp;&emsp; **img : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Image to rotate.<br />
 &emsp;&emsp; **Returns**:<br />
 &emsp;&emsp;&emsp;&emsp; **output : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Flipped image.<br />
 
-imgmagic.geometric.scaling(img:numpy.ndarray, scale:float)<br />
+**imgmagic.geometric.scaling(img:numpy.ndarray, scale:float)**<br />
 Function that scales an image.<br />
 &emsp;&emsp; **Parameters**:<br />
 &emsp;&emsp;&emsp;&emsp; **img : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Image to scale.<br />
 &emsp;&emsp;&emsp;&emsp; **scale : float**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Factor of scaling (ex. 0.5, 1.25, 2...etc).<br />
 &emsp;&emsp; **Returns**:<br />
 &emsp;&emsp;&emsp;&emsp; **output : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Scaled image.<br />
 
 
-imgmagic.geometric.reverse(img:numpy.ndarray)<br />
+**imgmagic.geometric.reverse(img:numpy.ndarray)**<br />
 Function that reverts an image.<br />
 &emsp;&emsp; **Parameters**:<br />
 &emsp;&emsp;&emsp;&emsp; **img : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Image to reverse.<br />
 &emsp;&emsp; **Returns**:<br />
 &emsp;&emsp;&emsp;&emsp; **output : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Reverted image.<br />
 
-imgmagic.histogram.adjustContrast(img:numpy.ndarray)<br />
+**imgmagic.histogram.adjustContrast(img:numpy.ndarray)**<br />
 Function that performs contrast stretching.<br />
 &emsp;&emsp; **Parameters**:<br />
 &emsp;&emsp;&emsp;&emsp; **img : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Input image.<br />
 &emsp;&emsp; **Returns**:<br />
 &emsp;&emsp;&emsp;&emsp; **output : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Image (with contrat stretching).<br />
 
-imgmagic.histogram.equalization(img:numpy.ndarray)<br />
+**imgmagic.histogram.equalization(img:numpy.ndarray)**<br />
 Function that performs histogram equalization.<br />
 &emsp;&emsp; **Parameters**:<br />
 &emsp;&emsp;&emsp;&emsp; **img : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Input image.<br />
 &emsp;&emsp; **Returns**:<br />
 &emsp;&emsp;&emsp;&emsp; **output : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Image (with equalization).<br />
 
-imgmagic.histogram.negative(img:numpy.ndarray)<br />
+**imgmagic.histogram.negative(img:numpy.ndarray)**<br />
 Function that performs computes digital negative of an image.<br />
 &emsp;&emsp;&emsp;&emsp;s = T( r ) = (L – 1) – r<br />
 &emsp;&emsp; **Parameters**:<br />
 &emsp;&emsp;&emsp;&emsp; **img : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Input image.<br />
 &emsp;&emsp; **Returns**:<br />
 &emsp;&emsp;&emsp;&emsp; **output : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Image (negative).<br />
 
-imgmagic.filter.GaussianNoise(img:numpy.ndarray, mean:float, sigma:float)
+**imgmagic.filter.GaussianNoise(img:numpy.ndarray, mean:float, sigma:float)**<br />
 Function that adds gaussian noise to an image.<br />
 &emsp;&emsp; **Parameters**:<br />
 &emsp;&emsp;&emsp;&emsp; **img : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Input image.<br />
 &emsp;&emsp;&emsp;&emsp; **mean, sigma : float**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Parameters for gaussian distribution.<br />
 &emsp;&emsp; **Returns**:<br />
 &emsp;&emsp;&emsp;&emsp; **output : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Image (with noise).<br />
 
 
-imgmagic.filter.SaltnPepperNoise(img:numpy.ndarray, prob:float)<br />
+**imgmagic.filter.SaltnPepperNoise(img:numpy.ndarray, prob:float)**<br />
 Function that adds salt and pepper noise.<br />
 &emsp;&emsp; **Parameters**:<br />
 &emsp;&emsp;&emsp;&emsp; **img : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Input image.<br />
 &emsp;&emsp;&emsp;&emsp; **prob : float**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Probability for salting (ex. 0.01 ...etc).<br />
 &emsp;&emsp; **Returns**:<br />
 &emsp;&emsp;&emsp;&emsp; **output : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Image (with noise).<br />
 
-imgmagic.filter.filtering(img:numpy.ndarray, types:str, mode:str, *args: Tuple[Any])<br />
+**imgmagic.filter.filtering(img:numpy.ndarray, types:str, mode:str, *args: Tuple[Any])**<br />
 Function that perfoms filtering on an image.<br />
 &emsp;&emsp; **Parameters**:<br />
 &emsp;&emsp;&emsp;&emsp; **img : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Input image.<br />
 &emsp;&emsp;&emsp;&emsp; **types : {"lowpass", "highpass", "avg", "gauss"}**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Type of filter.<br />
 &emsp;&emsp;&emsp;&emsp; **mode : {"reflect", "constant", "nearest", "mirror", "wrap"}**<br />
@@ -165,41 +165,41 @@
 &emsp;&emsp;&emsp;&emsp;&emsp; Extra arguments (optional). For instance, it can be:<br />
 &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;  n : size for avg filter<br />
 &emsp;&emsp; **Returns**:<br />
 &emsp;&emsp;&emsp;&emsp; **output : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Image (filtered).<br />
 
 
-imgmagic.filter.sharpening(img:numpy.ndarray, types:str, mode:str)<br />
+**imgmagic.filter.sharpening(img:numpy.ndarray, types:str, mode:str)**<br />
 Function that perfoms sharpening on an image.<br />
 &emsp;&emsp; **Parameters**:<br />
 &emsp;&emsp;&emsp;&emsp; **img : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Input image.<br />
 &emsp;&emsp;&emsp;&emsp; **types : {"laplacian", "sobel", "roberts"}**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Type of filter.<br />
 &emsp;&emsp;&emsp;&emsp; **mode : {"reflect", "constant", "wrap"}**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Type of padding.<br />
 &emsp;&emsp; **Returns**:<br />
 &emsp;&emsp;&emsp;&emsp; **output : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Image (filtered).<br />
 
-imgmagic.filter.crosscorrelation(img:numpy.ndarray, filters:str, sub:numpy.ndarray)<br />
+**imgmagic.filter.crosscorrelation(img:numpy.ndarray, filters:str, sub:numpy.ndarray)**<br />
 Function that find a subimage in an image.<br />
 &emsp;&emsp; **Parameters**:<br />
 &emsp;&emsp;&emsp;&emsp; **img : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Input image.<br />
 &emsp;&emsp;&emsp;&emsp; **filters : {"laplacian", "sobel", "roberts"}**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Type of filter.<br />
 &emsp;&emsp;&emsp;&emsp; **sub : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Subimage image.<br />
 &emsp;&emsp; **Returns**:<br />
 &emsp;&emsp;&emsp;&emsp; **output : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Image (found).<br />
 
-imgmagic.fourier.ftfiltering(img:numpy.ndarray, filters:str, *args: Tuple[Any])<br />
+**imgmagic.fourier.ftfiltering(img:numpy.ndarray, filters:str, *args: Tuple[Any])**<br />
 Function that perfoms sharpening on an image.<br />
 &emsp;&emsp; **Parameters**:<br />
 &emsp;&emsp;&emsp;&emsp; **img : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Input image.<br />
 &emsp;&emsp;&emsp;&emsp; **filters : {"lowpass", "blowpass", "glowpass", "highpass", "bhighpass", "ghighpass", "bandreject", "bandpass", "homomorphic"}**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Type of filter.<br />
 &emsp;&emsp;&emsp;&emsp; **args : float**<br />
@@ -208,15 +208,15 @@
 &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;  D0, n : cutoff frequency, order for Butterworth filter ("blowpass", "bhighpass")<br />
 &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; sigma : cutoff frequency for Gaussian filter ("glowpass", "ghighpass")<br />
 &emsp;&emsp; **Returns**:<br />
 &emsp;&emsp;&emsp;&emsp; **output : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Image (filtered).<br />
 
 
-imgmagic.fourier.UnsharpMasking(img:numpy.ndarray, D0:int, k:int)<br />
+**imgmagic.fourier.UnsharpMasking(img:numpy.ndarray, D0:int, k:int)**<br />
 Function that performs Unsharp Masking and Highboost filtering.<br />
 &emsp;&emsp; **Parameters**:<br />
 &emsp;&emsp;&emsp;&emsp; **img : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Input image.<br />
 &emsp;&emsp;&emsp;&emsp; **k : float**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Parameter:<br />
 &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; k=1 - unsharp masking<br />
```

## Comparing `imgmagic-0.2.7.dist-info/RECORD` & `imgmagic-0.2.8.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 imgmagic/__init__.py,sha256=74QY0Sg9Y4-7YAHku1RYcKdxZL4Pcvjc7a1fPYNPLn4,393
 imgmagic/colors.py,sha256=E4PlcOrASd9V8Gmqg6crHr0wGUcxMtNnq678bo-aPBk,673
 imgmagic/display.py,sha256=OPGVurZCzDMViFTL1PdUk7QZpP1-nvjyWH2AGH-sI7E,1446
 imgmagic/filter.py,sha256=M-sD5BFkmG3c1GHgI2pd-qi9o7UT7s7QXToTP5t8mX4,11895
 imgmagic/fourier.py,sha256=t8-HJDyAWnKJVwETUGaf6I-EUjOdz5lJfRodk9Pwz0E,13009
 imgmagic/geometric.py,sha256=PPGCsIiBtKx6O-NFwJkjbpRuqJWFW7n2h4hZI8fMRgA,3987
 imgmagic/histogram.py,sha256=UAuS9D0_P-5u3YKTlbUWtOoYcWDkmgBzSfybgeoM1F4,4352
-imgmagic-0.2.7.dist-info/METADATA,sha256=LwQj2yEBWNtiCvUJcUMunRCZXOynnGp8mRkVuZucATQ,11005
-imgmagic-0.2.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-imgmagic-0.2.7.dist-info/top_level.txt,sha256=0NkjpAFNl2tXByLndZgmnxt6LKEwAu0X41gVoFXjlmo,9
-imgmagic-0.2.7.dist-info/RECORD,,
+imgmagic-0.2.8.dist-info/METADATA,sha256=h8bgjqhQEfE-5gcOOI5C2EXeY7ltJN5gJAMNM96Q7so,11075
+imgmagic-0.2.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+imgmagic-0.2.8.dist-info/top_level.txt,sha256=0NkjpAFNl2tXByLndZgmnxt6LKEwAu0X41gVoFXjlmo,9
+imgmagic-0.2.8.dist-info/RECORD,,
```

