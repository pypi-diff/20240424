# Comparing `tmp/tensorrt_dispatch-9.3.0.post11.dev1.tar.gz` & `tmp/tensorrt_dispatch-9.3.0.post12.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorrt_dispatch-9.3.0.post11.dev1.tar", last modified: Wed Jan 31 22:16:05 2024, max compression
+gzip compressed data, was "tensorrt_dispatch-9.3.0.post12.dev1.tar", last modified: Wed Jan 31 22:35:05 2024, max compression
```

## Comparing `tensorrt_dispatch-9.3.0.post11.dev1.tar` & `tensorrt_dispatch-9.3.0.post12.dev1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2024-01-31 22:16:05.122169 tensorrt_dispatch-9.3.0.post11.dev1/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      464 2024-01-31 22:16:05.000000 tensorrt_dispatch-9.3.0.post11.dev1/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2024-01-06 03:22:49.000000 tensorrt_dispatch-9.3.0.post11.dev1/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       17 2024-01-31 22:16:05.000000 tensorrt_dispatch-9.3.0.post11.dev1/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1665 2024-01-31 22:16:05.118169 tensorrt_dispatch-9.3.0.post11.dev1/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      271 2024-01-31 22:16:05.000000 tensorrt_dispatch-9.3.0.post11.dev1/README.rst
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2024-01-31 22:16:05.122169 tensorrt_dispatch-9.3.0.post11.dev1/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4864 2024-01-06 03:22:49.000000 tensorrt_dispatch-9.3.0.post11.dev1/setup.py
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2024-01-31 22:16:05.118169 tensorrt_dispatch-9.3.0.post11.dev1/tensorrt_dispatch.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1665 2024-01-31 22:16:05.000000 tensorrt_dispatch-9.3.0.post11.dev1/tensorrt_dispatch.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      217 2024-01-31 22:16:05.000000 tensorrt_dispatch-9.3.0.post11.dev1/tensorrt_dispatch.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2024-01-31 22:16:05.000000 tensorrt_dispatch-9.3.0.post11.dev1/tensorrt_dispatch.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2024-01-31 22:16:05.000000 tensorrt_dispatch-9.3.0.post11.dev1/tensorrt_dispatch.egg-info/top_level.txt
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2024-01-31 22:35:05.515653 tensorrt_dispatch-9.3.0.post12.dev1/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      464 2024-01-31 22:35:05.000000 tensorrt_dispatch-9.3.0.post12.dev1/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2024-01-06 03:22:49.000000 tensorrt_dispatch-9.3.0.post12.dev1/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       17 2024-01-31 22:35:05.000000 tensorrt_dispatch-9.3.0.post12.dev1/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1665 2024-01-31 22:35:05.515653 tensorrt_dispatch-9.3.0.post12.dev1/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      271 2024-01-31 22:35:05.000000 tensorrt_dispatch-9.3.0.post12.dev1/README.rst
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2024-01-31 22:35:05.515653 tensorrt_dispatch-9.3.0.post12.dev1/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4864 2024-01-06 03:22:49.000000 tensorrt_dispatch-9.3.0.post12.dev1/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2024-01-31 22:35:05.515653 tensorrt_dispatch-9.3.0.post12.dev1/tensorrt_dispatch.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1665 2024-01-31 22:35:05.000000 tensorrt_dispatch-9.3.0.post12.dev1/tensorrt_dispatch.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      217 2024-01-31 22:35:05.000000 tensorrt_dispatch-9.3.0.post12.dev1/tensorrt_dispatch.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2024-01-31 22:35:05.000000 tensorrt_dispatch-9.3.0.post12.dev1/tensorrt_dispatch.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2024-01-31 22:35:05.000000 tensorrt_dispatch-9.3.0.post12.dev1/tensorrt_dispatch.egg-info/top_level.txt
```

### Comparing `tensorrt_dispatch-9.3.0.post11.dev1/LICENSE.md` & `tensorrt_dispatch-9.3.0.post12.dev1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tensorrt_dispatch-9.3.0.post11.dev1/PKG-INFO` & `tensorrt_dispatch-9.3.0.post12.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorrt_dispatch
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

### Comparing `tensorrt_dispatch-9.3.0.post11.dev1/setup.py` & `tensorrt_dispatch-9.3.0.post12.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `tensorrt_dispatch-9.3.0.post11.dev1/tensorrt_dispatch.egg-info/PKG-INFO` & `tensorrt_dispatch-9.3.0.post12.dev1/tensorrt_dispatch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorrt-dispatch
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

