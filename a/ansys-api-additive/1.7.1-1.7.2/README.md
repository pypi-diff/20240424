# Comparing `tmp/ansys_api_additive-1.7.1.tar.gz` & `tmp/ansys_api_additive-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_api_additive-1.7.1.tar", last modified: Thu Apr 18 15:18:36 2024, max compression
+gzip compressed data, was "ansys_api_additive-1.7.2.tar", last modified: Wed Apr 24 21:40:41 2024, max compression
```

## Comparing `ansys_api_additive-1.7.1.tar` & `ansys_api_additive-1.7.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:18:36.623108 ansys_api_additive-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-18 15:18:28.000000 ansys_api_additive-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-04-18 15:18:36.623108 ansys_api_additive-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-18 15:18:28.000000 ansys_api_additive-1.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:18:36.619108 ansys_api_additive-1.7.1/ansys/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:18:36.619108 ansys_api_additive-1.7.1/ansys/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:18:36.619108 ansys_api_additive-1.7.1/ansys/api/additive/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-18 15:18:28.000000 ansys_api_additive-1.7.1/ansys/api/additive/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-18 15:18:28.000000 ansys_api_additive-1.7.1/ansys/api/additive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:18:28.000000 ansys_api_additive-1.7.1/ansys/api/additive/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:18:36.623108 ansys_api_additive-1.7.1/ansys/api/additive/v0/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-18 15:18:28.000000 ansys_api_additive-1.7.1/ansys/api/additive/v0/about.proto
--rw-r--r--   0 runner    (1001) docker     (127)     8503 2024-04-18 15:18:28.000000 ansys_api_additive-1.7.1/ansys/api/additive/v0/additive_domain.proto
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-18 15:18:28.000000 ansys_api_additive-1.7.1/ansys/api/additive/v0/additive_materials.proto
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-18 15:18:28.000000 ansys_api_additive-1.7.1/ansys/api/additive/v0/additive_simulation.proto
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:18:36.623108 ansys_api_additive-1.7.1/ansys_api_additive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-04-18 15:18:36.000000 ansys_api_additive-1.7.1/ansys_api_additive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-18 15:18:36.000000 ansys_api_additive-1.7.1/ansys_api_additive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:18:36.000000 ansys_api_additive-1.7.1/ansys_api_additive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-18 15:18:36.000000 ansys_api_additive-1.7.1/ansys_api_additive.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-18 15:18:36.000000 ansys_api_additive-1.7.1/ansys_api_additive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 15:18:36.000000 ansys_api_additive-1.7.1/ansys_api_additive.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:18:36.619108 ansys_api_additive-1.7.1/google/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:18:36.623108 ansys_api_additive-1.7.1/google/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-18 15:18:28.000000 ansys_api_additive-1.7.1/google/api/annotations.proto
--rw-r--r--   0 runner    (1001) docker     (127)    15144 2024-04-18 15:18:28.000000 ansys_api_additive-1.7.1/google/api/http.proto
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-18 15:18:28.000000 ansys_api_additive-1.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 15:18:36.623108 ansys_api_additive-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-18 15:18:28.000000 ansys_api_additive-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:40:41.016648 ansys_api_additive-1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-24 21:40:32.000000 ansys_api_additive-1.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-04-24 21:40:41.016648 ansys_api_additive-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-24 21:40:32.000000 ansys_api_additive-1.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:40:41.012648 ansys_api_additive-1.7.2/ansys/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:40:41.012648 ansys_api_additive-1.7.2/ansys/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:40:41.016648 ansys_api_additive-1.7.2/ansys/api/additive/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 21:40:32.000000 ansys_api_additive-1.7.2/ansys/api/additive/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-24 21:40:32.000000 ansys_api_additive-1.7.2/ansys/api/additive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:40:32.000000 ansys_api_additive-1.7.2/ansys/api/additive/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:40:41.016648 ansys_api_additive-1.7.2/ansys/api/additive/v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-24 21:40:32.000000 ansys_api_additive-1.7.2/ansys/api/additive/v0/about.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     8494 2024-04-24 21:40:32.000000 ansys_api_additive-1.7.2/ansys/api/additive/v0/additive_domain.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-24 21:40:32.000000 ansys_api_additive-1.7.2/ansys/api/additive/v0/additive_materials.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-24 21:40:32.000000 ansys_api_additive-1.7.2/ansys/api/additive/v0/additive_simulation.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:40:41.016648 ansys_api_additive-1.7.2/ansys_api_additive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-04-24 21:40:41.000000 ansys_api_additive-1.7.2/ansys_api_additive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-24 21:40:41.000000 ansys_api_additive-1.7.2/ansys_api_additive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 21:40:41.000000 ansys_api_additive-1.7.2/ansys_api_additive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-24 21:40:41.000000 ansys_api_additive-1.7.2/ansys_api_additive.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-24 21:40:41.000000 ansys_api_additive-1.7.2/ansys_api_additive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 21:40:41.000000 ansys_api_additive-1.7.2/ansys_api_additive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:40:41.012648 ansys_api_additive-1.7.2/google/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:40:41.016648 ansys_api_additive-1.7.2/google/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-24 21:40:32.000000 ansys_api_additive-1.7.2/google/api/annotations.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    15144 2024-04-24 21:40:32.000000 ansys_api_additive-1.7.2/google/api/http.proto
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-24 21:40:32.000000 ansys_api_additive-1.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 21:40:41.016648 ansys_api_additive-1.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-24 21:40:32.000000 ansys_api_additive-1.7.2/setup.py
```

### Comparing `ansys_api_additive-1.7.1/LICENSE` & `ansys_api_additive-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_api_additive-1.7.1/PKG-INFO` & `ansys_api_additive-1.7.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-additive
-Version: 1.7.1
-Summary: Autogenerated python gRPC interface package for ansys-api-additive, built on 15:18:36 on 18 April 2024
+Version: 1.7.2
+Summary: Autogenerated python gRPC interface package for ansys-api-additive, built on 21:40:40 on 24 April 2024
 Home-page: https://github.com/ansys/ansys-api-additive
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
 Maintainer-email: pyansys.core@ansys.com
 License: MIT
 Project-URL: Documentation, https://github.com/ansys/ansys-api-additive/#readme
```

### Comparing `ansys_api_additive-1.7.1/README.md` & `ansys_api_additive-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `ansys_api_additive-1.7.1/ansys/api/additive/v0/additive_domain.proto` & `ansys_api_additive-1.7.2/ansys/api/additive/v0/additive_domain.proto`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     double reference_width = 5;
     double depth = 6;
     double reference_depth = 7;
 }
 
 message MeltPool {
     repeated MeltPoolTimeStep time_steps = 1;
-    repeated bytes thermal_history_vtk = 2;
+    bytes thermal_history_vtk = 2;
 }
 
 message AdditiveMaterial {
     double hardening_factor = 1;
     double strain_scaling_factor = 2;
     double support_yield_strength_ratio = 3;
     double poisson_ratio = 4;
```

### Comparing `ansys_api_additive-1.7.1/ansys/api/additive/v0/additive_materials.proto` & `ansys_api_additive-1.7.2/ansys/api/additive/v0/additive_materials.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_additive-1.7.1/ansys/api/additive/v0/additive_simulation.proto` & `ansys_api_additive-1.7.2/ansys/api/additive/v0/additive_simulation.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_additive-1.7.1/ansys_api_additive.egg-info/PKG-INFO` & `ansys_api_additive-1.7.2/ansys_api_additive.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-additive
-Version: 1.7.1
-Summary: Autogenerated python gRPC interface package for ansys-api-additive, built on 15:18:36 on 18 April 2024
+Version: 1.7.2
+Summary: Autogenerated python gRPC interface package for ansys-api-additive, built on 21:40:40 on 24 April 2024
 Home-page: https://github.com/ansys/ansys-api-additive
 Author: ANSYS, Inc.
 Author-email: pyansys.core@ansys.com
 Maintainer: ANSYS, Inc.
 Maintainer-email: pyansys.core@ansys.com
 License: MIT
 Project-URL: Documentation, https://github.com/ansys/ansys-api-additive/#readme
```

### Comparing `ansys_api_additive-1.7.1/ansys_api_additive.egg-info/SOURCES.txt` & `ansys_api_additive-1.7.2/ansys_api_additive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansys_api_additive-1.7.1/google/api/annotations.proto` & `ansys_api_additive-1.7.2/google/api/annotations.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_additive-1.7.1/google/api/http.proto` & `ansys_api_additive-1.7.2/google/api/http.proto`

 * *Files identical despite different names*

### Comparing `ansys_api_additive-1.7.1/setup.py` & `ansys_api_additive-1.7.2/setup.py`

 * *Files identical despite different names*

