# Comparing `tmp/imgmagic-0.2.0-py3-none-any.whl.zip` & `tmp/imgmagic-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 11349 bytes, number of entries: 11
+Zip file size: 11353 bytes, number of entries: 11
 -rw-rw-r--  2.0 unx      393 b- defN 24-Apr-23 09:22 imgmagic/__init__.py
 -rw-rw-r--  2.0 unx      673 b- defN 24-Apr-15 08:54 imgmagic/colors.py
 -rw-rw-r--  2.0 unx     1446 b- defN 24-Apr-15 08:54 imgmagic/display.py
 -rw-rw-r--  2.0 unx    11895 b- defN 24-Apr-21 13:26 imgmagic/filter.py
 -rw-rw-r--  2.0 unx    13009 b- defN 24-Apr-23 11:14 imgmagic/fourier.py
 -rw-rw-r--  2.0 unx     3987 b- defN 24-Apr-15 08:54 imgmagic/geometric.py
 -rw-rw-r--  2.0 unx     4352 b- defN 24-Apr-15 08:54 imgmagic/histogram.py
--rw-rw-r--  2.0 unx    10050 b- defN 24-Apr-24 13:23 imgmagic-0.2.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-24 13:23 imgmagic-0.2.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 24-Apr-24 13:23 imgmagic-0.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      837 b- defN 24-Apr-24 13:23 imgmagic-0.2.0.dist-info/RECORD
-11 files, 46743 bytes uncompressed, 9955 bytes compressed:  78.7%
+-rw-rw-r--  2.0 unx    10062 b- defN 24-Apr-24 13:28 imgmagic-0.2.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-24 13:28 imgmagic-0.2.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 24-Apr-24 13:28 imgmagic-0.2.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      837 b- defN 24-Apr-24 13:28 imgmagic-0.2.1.dist-info/RECORD
+11 files, 46755 bytes uncompressed, 9959 bytes compressed:  78.7%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: imgmagic/geometric.py
 Comment: 
 
 Filename: imgmagic/histogram.py
 Comment: 
 
-Filename: imgmagic-0.2.0.dist-info/METADATA
+Filename: imgmagic-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: imgmagic-0.2.0.dist-info/WHEEL
+Filename: imgmagic-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: imgmagic-0.2.0.dist-info/top_level.txt
+Filename: imgmagic-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: imgmagic-0.2.0.dist-info/RECORD
+Filename: imgmagic-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `imgmagic-0.2.0.dist-info/METADATA` & `imgmagic-0.2.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgmagic
-Version: 0.2.0
+Version: 0.2.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Requires-Dist: numpy (>=1.23.4)
 Requires-Dist: scipy (>=1.11.4)
@@ -16,21 +16,23 @@
 Toolbox to perform image processing.
 
 ### Libraries
 * Install numpy, scipy, matplotlib, pillow.
 
 ### Documentation
 ##### imgmagic.display.greyscale(x: numpy.ndarray)
+```bash
 Function that converts image into greyscale.
 &emsp;&emsp; **Parameters**:
 &emsp;&emsp;&emsp;&emsp; **x : numpy.ndarray**
 &emsp;&emsp;&emsp;&emsp;&emsp; Image to convert.
 &emsp;&emsp; **Returns**:
 &emsp;&emsp;&emsp;&emsp; **output : numpy.ndarray**
 &emsp;&emsp;&emsp;&emsp;&emsp; Returns the greyscale image.
+```
 
 ##### imgmagic.geometric.crop(img:numpy.ndarray, x:Tuple[int], width:int, height:int)
  Function that crops an image.
 &emsp;&emsp; **Parameters**:
 &emsp;&emsp;&emsp;&emsp; **img : numpy.ndarray**
 &emsp;&emsp;&emsp;&emsp;&emsp; Image to crop.
 &emsp;&emsp;&emsp;&emsp; **x : Tuple[int]**
```

## Comparing `imgmagic-0.2.0.dist-info/RECORD` & `imgmagic-0.2.1.dist-info/RECORD`

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
-imgmagic-0.2.0.dist-info/METADATA,sha256=5oFxCoS0gT07johDOaI-b3O5ivQdNaTW0iMYI0Jyx48,10050
-imgmagic-0.2.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-imgmagic-0.2.0.dist-info/top_level.txt,sha256=0NkjpAFNl2tXByLndZgmnxt6LKEwAu0X41gVoFXjlmo,9
-imgmagic-0.2.0.dist-info/RECORD,,
+imgmagic-0.2.1.dist-info/METADATA,sha256=18r5LyYgn5n0wxB6LGJW-BobdOs_vVML5XGcQJXzzVE,10062
+imgmagic-0.2.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+imgmagic-0.2.1.dist-info/top_level.txt,sha256=0NkjpAFNl2tXByLndZgmnxt6LKEwAu0X41gVoFXjlmo,9
+imgmagic-0.2.1.dist-info/RECORD,,
```

