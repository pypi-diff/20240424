# Comparing `tmp/tensorrt-9.3.0.post11.dev1.tar.gz` & `tmp/tensorrt-9.3.0.post12.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorrt-9.3.0.post11.dev1.tar", last modified: Wed Jan 31 22:02:29 2024, max compression
+gzip compressed data, was "tensorrt-9.3.0.post12.dev1.tar", last modified: Wed Jan 31 22:21:28 2024, max compression
```

## Comparing `tensorrt-9.3.0.post11.dev1.tar` & `tensorrt-9.3.0.post12.dev1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2024-01-31 22:02:29.397499 tensorrt-9.3.0.post11.dev1/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      455 2024-01-31 22:02:29.000000 tensorrt-9.3.0.post11.dev1/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2024-01-06 03:22:49.000000 tensorrt-9.3.0.post11.dev1/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        8 2024-01-31 22:02:29.000000 tensorrt-9.3.0.post11.dev1/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1629 2024-01-31 22:02:29.397499 tensorrt-9.3.0.post11.dev1/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      244 2024-01-31 22:02:29.000000 tensorrt-9.3.0.post11.dev1/README.rst
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2024-01-31 22:02:29.397499 tensorrt-9.3.0.post11.dev1/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4864 2024-01-06 03:22:49.000000 tensorrt-9.3.0.post11.dev1/setup.py
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2024-01-31 22:02:29.397499 tensorrt-9.3.0.post11.dev1/tensorrt.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1629 2024-01-31 22:02:29.000000 tensorrt-9.3.0.post11.dev1/tensorrt.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      181 2024-01-31 22:02:29.000000 tensorrt-9.3.0.post11.dev1/tensorrt.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2024-01-31 22:02:29.000000 tensorrt-9.3.0.post11.dev1/tensorrt.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2024-01-31 22:02:29.000000 tensorrt-9.3.0.post11.dev1/tensorrt.egg-info/top_level.txt
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2024-01-31 22:21:28.889889 tensorrt-9.3.0.post12.dev1/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      455 2024-01-31 22:21:28.000000 tensorrt-9.3.0.post12.dev1/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2024-01-06 03:22:49.000000 tensorrt-9.3.0.post12.dev1/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        8 2024-01-31 22:21:28.000000 tensorrt-9.3.0.post12.dev1/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1629 2024-01-31 22:21:28.889889 tensorrt-9.3.0.post12.dev1/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      244 2024-01-31 22:21:28.000000 tensorrt-9.3.0.post12.dev1/README.rst
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2024-01-31 22:21:28.889889 tensorrt-9.3.0.post12.dev1/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4864 2024-01-06 03:22:49.000000 tensorrt-9.3.0.post12.dev1/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2024-01-31 22:21:28.889889 tensorrt-9.3.0.post12.dev1/tensorrt.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1629 2024-01-31 22:21:28.000000 tensorrt-9.3.0.post12.dev1/tensorrt.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      181 2024-01-31 22:21:28.000000 tensorrt-9.3.0.post12.dev1/tensorrt.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2024-01-31 22:21:28.000000 tensorrt-9.3.0.post12.dev1/tensorrt.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2024-01-31 22:21:28.000000 tensorrt-9.3.0.post12.dev1/tensorrt.egg-info/top_level.txt
```

### Comparing `tensorrt-9.3.0.post11.dev1/LICENSE.md` & `tensorrt-9.3.0.post12.dev1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tensorrt-9.3.0.post11.dev1/PKG-INFO` & `tensorrt-9.3.0.post12.dev1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorrt
-Version: 9.3.0.post11.dev1
+Version: 9.3.0.post12.dev1
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `tensorrt-9.3.0.post11.dev1/setup.py` & `tensorrt-9.3.0.post12.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `tensorrt-9.3.0.post11.dev1/tensorrt.egg-info/PKG-INFO` & `tensorrt-9.3.0.post12.dev1/tensorrt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorrt
-Version: 9.3.0.post11.dev1
+Version: 9.3.0.post12.dev1
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

