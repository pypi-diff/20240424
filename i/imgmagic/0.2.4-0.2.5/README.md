# Comparing `tmp/imgmagic-0.2.4-py3-none-any.whl.zip` & `tmp/imgmagic-0.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 11378 bytes, number of entries: 11
+Zip file size: 11381 bytes, number of entries: 11
 -rw-rw-r--  2.0 unx      393 b- defN 24-Apr-23 09:22 imgmagic/__init__.py
 -rw-rw-r--  2.0 unx      673 b- defN 24-Apr-15 08:54 imgmagic/colors.py
 -rw-rw-r--  2.0 unx     1446 b- defN 24-Apr-15 08:54 imgmagic/display.py
 -rw-rw-r--  2.0 unx    11895 b- defN 24-Apr-21 13:26 imgmagic/filter.py
 -rw-rw-r--  2.0 unx    13009 b- defN 24-Apr-23 11:14 imgmagic/fourier.py
 -rw-rw-r--  2.0 unx     3987 b- defN 24-Apr-15 08:54 imgmagic/geometric.py
 -rw-rw-r--  2.0 unx     4352 b- defN 24-Apr-15 08:54 imgmagic/histogram.py
--rw-rw-r--  2.0 unx    11086 b- defN 24-Apr-24 13:40 imgmagic-0.2.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-24 13:40 imgmagic-0.2.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 24-Apr-24 13:40 imgmagic-0.2.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      837 b- defN 24-Apr-24 13:40 imgmagic-0.2.4.dist-info/RECORD
-11 files, 47779 bytes uncompressed, 9984 bytes compressed:  79.1%
+-rw-rw-r--  2.0 unx    11088 b- defN 24-Apr-24 13:41 imgmagic-0.2.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-24 13:41 imgmagic-0.2.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 24-Apr-24 13:41 imgmagic-0.2.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      837 b- defN 24-Apr-24 13:41 imgmagic-0.2.5.dist-info/RECORD
+11 files, 47781 bytes uncompressed, 9987 bytes compressed:  79.1%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: imgmagic/geometric.py
 Comment: 
 
 Filename: imgmagic/histogram.py
 Comment: 
 
-Filename: imgmagic-0.2.4.dist-info/METADATA
+Filename: imgmagic-0.2.5.dist-info/METADATA
 Comment: 
 
-Filename: imgmagic-0.2.4.dist-info/WHEEL
+Filename: imgmagic-0.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: imgmagic-0.2.4.dist-info/top_level.txt
+Filename: imgmagic-0.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: imgmagic-0.2.4.dist-info/RECORD
+Filename: imgmagic-0.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `imgmagic-0.2.4.dist-info/METADATA` & `imgmagic-0.2.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imgmagic
-Version: 0.2.4
+Version: 0.2.5
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Requires-Dist: numpy (>=1.23.4)
 Requires-Dist: scipy (>=1.11.4)
@@ -29,15 +29,15 @@
 img2 = imgmagic.filter.filtering(img1, "avg", "wrap", 9)
 
 im = Image.fromarray(img2)
 im.save("new.jpeg")
 ```
 
 ### Documentation
-##### imgmagic.display.greyscale(x: numpy.ndarray)
+####### imgmagic.display.greyscale(x: numpy.ndarray)
 Function that converts image into greyscale.<br />
 &emsp;&emsp; **Parameters**:<br />
 &emsp;&emsp;&emsp;&emsp; **x : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Image to convert.<br />
 &emsp;&emsp; **Returns**:<br />
 &emsp;&emsp;&emsp;&emsp; **output : numpy.ndarray**<br />
 &emsp;&emsp;&emsp;&emsp;&emsp; Returns the greyscale image.<br />
```

## Comparing `imgmagic-0.2.4.dist-info/RECORD` & `imgmagic-0.2.5.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 imgmagic/__init__.py,sha256=74QY0Sg9Y4-7YAHku1RYcKdxZL4Pcvjc7a1fPYNPLn4,393
 imgmagic/colors.py,sha256=E4PlcOrASd9V8Gmqg6crHr0wGUcxMtNnq678bo-aPBk,673
 imgmagic/display.py,sha256=OPGVurZCzDMViFTL1PdUk7QZpP1-nvjyWH2AGH-sI7E,1446
 imgmagic/filter.py,sha256=M-sD5BFkmG3c1GHgI2pd-qi9o7UT7s7QXToTP5t8mX4,11895
 imgmagic/fourier.py,sha256=t8-HJDyAWnKJVwETUGaf6I-EUjOdz5lJfRodk9Pwz0E,13009
 imgmagic/geometric.py,sha256=PPGCsIiBtKx6O-NFwJkjbpRuqJWFW7n2h4hZI8fMRgA,3987
 imgmagic/histogram.py,sha256=UAuS9D0_P-5u3YKTlbUWtOoYcWDkmgBzSfybgeoM1F4,4352
-imgmagic-0.2.4.dist-info/METADATA,sha256=6VFeh2ak3G_T-hzfBGwETBPPfqM3D4oYNMWu4or4HB0,11086
-imgmagic-0.2.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-imgmagic-0.2.4.dist-info/top_level.txt,sha256=0NkjpAFNl2tXByLndZgmnxt6LKEwAu0X41gVoFXjlmo,9
-imgmagic-0.2.4.dist-info/RECORD,,
+imgmagic-0.2.5.dist-info/METADATA,sha256=1ey_llfZD2SWQ_49fBkABKmTUrn_TQpYLD70yJmnoss,11088
+imgmagic-0.2.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+imgmagic-0.2.5.dist-info/top_level.txt,sha256=0NkjpAFNl2tXByLndZgmnxt6LKEwAu0X41gVoFXjlmo,9
+imgmagic-0.2.5.dist-info/RECORD,,
```

