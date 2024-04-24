# Comparing `tmp/imgmagic-0.2.1-py3-none-any.whl.zip` & `tmp/imgmagic-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 11353 bytes, number of entries: 11
+Zip file size: 11386 bytes, number of entries: 11
 -rw-rw-r--  2.0 unx      393 b- defN 24-Apr-23 09:22 imgmagic/__init__.py
 -rw-rw-r--  2.0 unx      673 b- defN 24-Apr-15 08:54 imgmagic/colors.py
 -rw-rw-r--  2.0 unx     1446 b- defN 24-Apr-15 08:54 imgmagic/display.py
 -rw-rw-r--  2.0 unx    11895 b- defN 24-Apr-21 13:26 imgmagic/filter.py
 -rw-rw-r--  2.0 unx    13009 b- defN 24-Apr-23 11:14 imgmagic/fourier.py
 -rw-rw-r--  2.0 unx     3987 b- defN 24-Apr-15 08:54 imgmagic/geometric.py
 -rw-rw-r--  2.0 unx     4352 b- defN 24-Apr-15 08:54 imgmagic/histogram.py
--rw-rw-r--  2.0 unx    10062 b- defN 24-Apr-24 13:28 imgmagic-0.2.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-24 13:28 imgmagic-0.2.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 24-Apr-24 13:28 imgmagic-0.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      837 b- defN 24-Apr-24 13:28 imgmagic-0.2.1.dist-info/RECORD
-11 files, 46755 bytes uncompressed, 9959 bytes compressed:  78.7%
+-rw-rw-r--  2.0 unx    10121 b- defN 24-Apr-24 13:31 imgmagic-0.2.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-24 13:31 imgmagic-0.2.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 24-Apr-24 13:31 imgmagic-0.2.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      837 b- defN 24-Apr-24 13:31 imgmagic-0.2.2.dist-info/RECORD
+11 files, 46814 bytes uncompressed, 9992 bytes compressed:  78.7%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: imgmagic/geometric.py
 Comment: 
 
 Filename: imgmagic/histogram.py
 Comment: 
 
-Filename: imgmagic-0.2.1.dist-info/METADATA
+Filename: imgmagic-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: imgmagic-0.2.1.dist-info/WHEEL
+Filename: imgmagic-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: imgmagic-0.2.1.dist-info/top_level.txt
+Filename: imgmagic-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: imgmagic-0.2.1.dist-info/RECORD
+Filename: imgmagic-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `imgmagic-0.2.1.dist-info/METADATA` & `imgmagic-0.2.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: imgmagic
-Version: 0.2.1
+Version: 0.2.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Requires-Dist: numpy (>=1.23.4)
 Requires-Dist: scipy (>=1.11.4)
 Requires-Dist: matplotlib (>=3.5.1)
 Requires-Dist: pillow (>=9.0.1)
 Requires-Dist: protobuf (<4)
 
-# Image Processing
 Toolbox to perform image processing.
 
 ### Libraries
 * Install numpy, scipy, matplotlib, pillow.
 
 ### Documentation
 ##### imgmagic.display.greyscale(x: numpy.ndarray)
@@ -27,27 +26,27 @@
 &emsp;&emsp;&emsp;&emsp;&emsp; Image to convert.
 &emsp;&emsp; **Returns**:
 &emsp;&emsp;&emsp;&emsp; **output : numpy.ndarray**
 &emsp;&emsp;&emsp;&emsp;&emsp; Returns the greyscale image.
 ```
 
 ##### imgmagic.geometric.crop(img:numpy.ndarray, x:Tuple[int], width:int, height:int)
- Function that crops an image.
-&emsp;&emsp; **Parameters**:
-&emsp;&emsp;&emsp;&emsp; **img : numpy.ndarray**
-&emsp;&emsp;&emsp;&emsp;&emsp; Image to crop.
-&emsp;&emsp;&emsp;&emsp; **x : Tuple[int]**
-&emsp;&emsp;&emsp;&emsp;&emsp; Coordiates of starting point.
-&emsp;&emsp;&emsp;&emsp; **width : int**
-&emsp;&emsp;&emsp;&emsp;&emsp; Width of the cropped image.
-&emsp;&emsp;&emsp;&emsp; **height : int**
-&emsp;&emsp;&emsp;&emsp;&emsp; Height of the cropped image.
-&emsp;&emsp; **Returns**:
-&emsp;&emsp;&emsp;&emsp; **output : numpy.ndarray**
-&emsp;&emsp;&emsp;&emsp;&emsp; Cropped image.
+ Function that crops an image.<br />
+&emsp;&emsp; **Parameters**:<br />
+&emsp;&emsp;&emsp;&emsp; **img : numpy.ndarray**<br />
+&emsp;&emsp;&emsp;&emsp;&emsp; Image to crop.<br />
+&emsp;&emsp;&emsp;&emsp; **x : Tuple[int]**<br />
+&emsp;&emsp;&emsp;&emsp;&emsp; Coordiates of starting point.<br />
+&emsp;&emsp;&emsp;&emsp; **width : int**<br />
+&emsp;&emsp;&emsp;&emsp;&emsp; Width of the cropped image.<br />
+&emsp;&emsp;&emsp;&emsp; **height : int**<br />
+&emsp;&emsp;&emsp;&emsp;&emsp; Height of the cropped image.<br />
+&emsp;&emsp; **Returns**:<br />
+&emsp;&emsp;&emsp;&emsp; **output : numpy.ndarray**<br />
+&emsp;&emsp;&emsp;&emsp;&emsp; Cropped image.<br />
 
     
 ##### imgmagic.geometric.rotate(img:numpy.ndarray, degree:float)
 Function that rotates an image.
 &emsp;&emsp; **Parameters**:
 &emsp;&emsp;&emsp;&emsp; **img : numpy.ndarray**
 &emsp;&emsp;&emsp;&emsp;&emsp; Image to rotate.
```

