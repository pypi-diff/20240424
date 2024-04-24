# Comparing `tmp/funcnodes_opencv-0.1.0.tar.gz` & `tmp/funcnodes_opencv-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes_opencv-0.1.0.tar", max compression
+gzip compressed data, was "funcnodes_opencv-0.1.1.tar", max compression
```

## Comparing `funcnodes_opencv-0.1.0.tar` & `funcnodes_opencv-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      101 2024-04-24 11:35:56.585713 funcnodes_opencv-0.1.0/funcnodes_opencv/__init__.py
--rw-r--r--   0        0        0     2822 2024-04-24 11:37:00.653404 funcnodes_opencv-0.1.0/funcnodes_opencv/imageformat.py
--rw-r--r--   0        0        0      361 2024-04-24 11:35:08.340021 funcnodes_opencv-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-24 11:32:57.575895 funcnodes_opencv-0.1.0/README.md
--rw-r--r--   0        0        0      459 1970-01-01 00:00:00.000000 funcnodes_opencv-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      101 2024-04-24 12:04:20.719727 funcnodes_opencv-0.1.1/funcnodes_opencv/__init__.py
+-rw-r--r--   0        0        0     2822 2024-04-24 12:02:15.184275 funcnodes_opencv-0.1.1/funcnodes_opencv/imageformat.py
+-rw-r--r--   0        0        0      361 2024-04-24 12:04:06.134372 funcnodes_opencv-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-24 11:32:57.575895 funcnodes_opencv-0.1.1/README.md
+-rw-r--r--   0        0        0      459 1970-01-01 00:00:00.000000 funcnodes_opencv-0.1.1/PKG-INFO
```

### Comparing `funcnodes_opencv-0.1.0/funcnodes_opencv/imageformat.py` & `funcnodes_opencv-0.1.1/funcnodes_opencv/imageformat.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     def to_jpeg(self, quality=0.75) -> bytes:
         return cv2.imencode(
             ".jpg", self.data, [int(cv2.IMWRITE_JPEG_QUALITY), int(quality * 100)]
         )[1].tobytes()
 
     def to_thumbnail(self, size: tuple) -> "OpenCVImageFormat":
-        cur_x, cur_y = self.data.shape[:2]
+        cur_y, cur_x = self.data.shape[:2]
         ratio = min(size[0] / cur_x, size[1] / cur_y)
         new_x, new_y = int(cur_x * ratio), int(cur_y * ratio)
         return OpenCVImageFormat(
             cv2.resize(
                 self._data,
                 (new_x, new_y),
             )
```

