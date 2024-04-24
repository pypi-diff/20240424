# Comparing `tmp/funcnodes_opencv-0.1.1.tar.gz` & `tmp/funcnodes_opencv-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes_opencv-0.1.1.tar", max compression
+gzip compressed data, was "funcnodes_opencv-0.1.2.tar", max compression
```

## Comparing `funcnodes_opencv-0.1.1.tar` & `funcnodes_opencv-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      101 2024-04-24 12:04:20.719727 funcnodes_opencv-0.1.1/funcnodes_opencv/__init__.py
--rw-r--r--   0        0        0     2822 2024-04-24 12:02:15.184275 funcnodes_opencv-0.1.1/funcnodes_opencv/imageformat.py
--rw-r--r--   0        0        0      361 2024-04-24 12:04:06.134372 funcnodes_opencv-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-24 11:32:57.575895 funcnodes_opencv-0.1.1/README.md
--rw-r--r--   0        0        0      459 1970-01-01 00:00:00.000000 funcnodes_opencv-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      101 2024-04-24 13:02:24.215736 funcnodes_opencv-0.1.2/funcnodes_opencv/__init__.py
+-rw-r--r--   0        0        0     2956 2024-04-24 13:02:03.732194 funcnodes_opencv-0.1.2/funcnodes_opencv/imageformat.py
+-rw-r--r--   0        0        0      361 2024-04-24 13:03:24.333088 funcnodes_opencv-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-24 11:32:57.575895 funcnodes_opencv-0.1.2/README.md
+-rw-r--r--   0        0        0      459 1970-01-01 00:00:00.000000 funcnodes_opencv-0.1.2/PKG-INFO
```

### Comparing `funcnodes_opencv-0.1.1/funcnodes_opencv/imageformat.py` & `funcnodes_opencv-0.1.2/funcnodes_opencv/imageformat.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,7 +82,11 @@
 
 def cv2_to_pil(cv2_img: OpenCVImageFormat) -> PillowImageFormat:
     return cv2_img.to_np().to_img()
 
 
 def pil_to_cv2(pil_img: PillowImageFormat) -> OpenCVImageFormat:
     return pil_img.to_np().to_cv2()
+
+
+OpenCVImageFormat.add_to_converter(PillowImageFormat, cv2_to_pil)
+OpenCVImageFormat.add_to_converter(PillowImageFormat, pil_to_cv2)
```

