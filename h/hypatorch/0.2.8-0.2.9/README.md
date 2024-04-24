# Comparing `tmp/hypatorch-0.2.8.tar.gz` & `tmp/hypatorch-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypatorch-0.2.8.tar", last modified: Thu Apr 11 08:48:39 2024, max compression
+gzip compressed data, was "hypatorch-0.2.9.tar", last modified: Tue Apr 16 14:00:25 2024, max compression
```

## Comparing `hypatorch-0.2.8.tar` & `hypatorch-0.2.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 paulkrug   (502) staff       (20)        0 2024-04-11 08:48:39.324014 hypatorch-0.2.8/
--rw-r--r--   0 paulkrug   (502) staff       (20)    11357 2024-03-18 15:51:00.000000 hypatorch-0.2.8/LICENSE
--rw-r--r--   0 paulkrug   (502) staff       (20)      779 2024-04-11 08:48:39.323787 hypatorch-0.2.8/PKG-INFO
--rw-r--r--   0 paulkrug   (502) staff       (20)      403 2024-03-18 20:05:31.000000 hypatorch-0.2.8/README.md
-drwxr-xr-x   0 paulkrug   (502) staff       (20)        0 2024-04-11 08:48:39.322178 hypatorch-0.2.8/hypatorch/
--rw-r--r--   0 paulkrug   (502) staff       (20)      258 2024-04-11 08:47:38.000000 hypatorch-0.2.8/hypatorch/__init__.py
--rw-r--r--   0 paulkrug   (502) staff       (20)     4816 2024-04-11 08:47:29.000000 hypatorch-0.2.8/hypatorch/assessments.py
--rw-r--r--   0 paulkrug   (502) staff       (20)    25337 2024-04-11 08:47:29.000000 hypatorch-0.2.8/hypatorch/core.py
--rw-r--r--   0 paulkrug   (502) staff       (20)     2544 2024-03-18 20:05:31.000000 hypatorch-0.2.8/hypatorch/losses.py
--rw-r--r--   0 paulkrug   (502) staff       (20)     7427 2024-04-11 08:47:29.000000 hypatorch-0.2.8/hypatorch/utils.py
-drwxr-xr-x   0 paulkrug   (502) staff       (20)        0 2024-04-11 08:48:39.323524 hypatorch-0.2.8/hypatorch.egg-info/
--rw-r--r--   0 paulkrug   (502) staff       (20)      779 2024-04-11 08:48:39.000000 hypatorch-0.2.8/hypatorch.egg-info/PKG-INFO
--rw-r--r--   0 paulkrug   (502) staff       (20)      294 2024-04-11 08:48:39.000000 hypatorch-0.2.8/hypatorch.egg-info/SOURCES.txt
--rw-r--r--   0 paulkrug   (502) staff       (20)        1 2024-04-11 08:48:39.000000 hypatorch-0.2.8/hypatorch.egg-info/dependency_links.txt
--rw-r--r--   0 paulkrug   (502) staff       (20)       37 2024-04-11 08:48:39.000000 hypatorch-0.2.8/hypatorch.egg-info/requires.txt
--rw-r--r--   0 paulkrug   (502) staff       (20)       10 2024-04-11 08:48:39.000000 hypatorch-0.2.8/hypatorch.egg-info/top_level.txt
--rw-r--r--   0 paulkrug   (502) staff       (20)       38 2024-04-11 08:48:39.324073 hypatorch-0.2.8/setup.cfg
--rw-r--r--   0 paulkrug   (502) staff       (20)      807 2024-03-19 10:48:19.000000 hypatorch-0.2.8/setup.py
+drwxr-xr-x   0 paulkrug   (502) staff       (20)        0 2024-04-16 14:00:25.499584 hypatorch-0.2.9/
+-rw-r--r--   0 paulkrug   (502) staff       (20)    11357 2024-03-18 15:51:00.000000 hypatorch-0.2.9/LICENSE
+-rw-r--r--   0 paulkrug   (502) staff       (20)      779 2024-04-16 14:00:25.499332 hypatorch-0.2.9/PKG-INFO
+-rw-r--r--   0 paulkrug   (502) staff       (20)      403 2024-03-18 20:05:31.000000 hypatorch-0.2.9/README.md
+drwxr-xr-x   0 paulkrug   (502) staff       (20)        0 2024-04-16 14:00:25.497950 hypatorch-0.2.9/hypatorch/
+-rw-r--r--   0 paulkrug   (502) staff       (20)      258 2024-04-16 13:59:22.000000 hypatorch-0.2.9/hypatorch/__init__.py
+-rw-r--r--   0 paulkrug   (502) staff       (20)     4816 2024-04-11 08:47:29.000000 hypatorch-0.2.9/hypatorch/assessments.py
+-rw-r--r--   0 paulkrug   (502) staff       (20)    25337 2024-04-11 08:47:29.000000 hypatorch-0.2.9/hypatorch/core.py
+-rw-r--r--   0 paulkrug   (502) staff       (20)     2544 2024-03-18 20:05:31.000000 hypatorch-0.2.9/hypatorch/losses.py
+-rw-r--r--   0 paulkrug   (502) staff       (20)     7739 2024-04-16 13:58:46.000000 hypatorch-0.2.9/hypatorch/utils.py
+drwxr-xr-x   0 paulkrug   (502) staff       (20)        0 2024-04-16 14:00:25.499029 hypatorch-0.2.9/hypatorch.egg-info/
+-rw-r--r--   0 paulkrug   (502) staff       (20)      779 2024-04-16 14:00:25.000000 hypatorch-0.2.9/hypatorch.egg-info/PKG-INFO
+-rw-r--r--   0 paulkrug   (502) staff       (20)      294 2024-04-16 14:00:25.000000 hypatorch-0.2.9/hypatorch.egg-info/SOURCES.txt
+-rw-r--r--   0 paulkrug   (502) staff       (20)        1 2024-04-16 14:00:25.000000 hypatorch-0.2.9/hypatorch.egg-info/dependency_links.txt
+-rw-r--r--   0 paulkrug   (502) staff       (20)       37 2024-04-16 14:00:25.000000 hypatorch-0.2.9/hypatorch.egg-info/requires.txt
+-rw-r--r--   0 paulkrug   (502) staff       (20)       10 2024-04-16 14:00:25.000000 hypatorch-0.2.9/hypatorch.egg-info/top_level.txt
+-rw-r--r--   0 paulkrug   (502) staff       (20)       38 2024-04-16 14:00:25.499631 hypatorch-0.2.9/setup.cfg
+-rw-r--r--   0 paulkrug   (502) staff       (20)      807 2024-03-19 10:48:19.000000 hypatorch-0.2.9/setup.py
```

### Comparing `hypatorch-0.2.8/LICENSE` & `hypatorch-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hypatorch-0.2.8/PKG-INFO` & `hypatorch-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypatorch
-Version: 0.2.8
+Version: 0.2.9
 Summary: HypaTorch: A library for abstract and visual model configuration
 Home-page: https://github.com/Altavo/hypatorch/
 Author: Altavo GmbH
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
```

### Comparing `hypatorch-0.2.8/hypatorch/assessments.py` & `hypatorch-0.2.9/hypatorch/assessments.py`

 * *Files identical despite different names*

### Comparing `hypatorch-0.2.8/hypatorch/core.py` & `hypatorch-0.2.9/hypatorch/core.py`

 * *Files identical despite different names*

### Comparing `hypatorch-0.2.8/hypatorch/losses.py` & `hypatorch-0.2.9/hypatorch/losses.py`

 * *Files identical despite different names*

### Comparing `hypatorch-0.2.8/hypatorch/utils.py` & `hypatorch-0.2.9/hypatorch/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,16 +40,25 @@
             f"""
             The function must have a single return statement,
             but passed function has {return_part.count("return ")}
             return statements.
             """
             )
     
+    # Remove leading and trailing "(" and ")"
+    return_part = return_part.strip("()")
+    # Remove new line chars
+    return_part = return_part.replace("\n", "")
+    # Remove all whitespaces
+    return_part = return_part.replace(" ", "")
+    # Remove trailing commas
+    return_part = return_part.rstrip(",")
     # Split by commas and clean up the code
     returned_variables = return_part.split(",")
+
     returned_variables = [var.strip() for var in returned_variables]
     
     return returned_variables
 
 def make_iterable(
         x,
         make_none_iterable = False,
```

### Comparing `hypatorch-0.2.8/hypatorch.egg-info/PKG-INFO` & `hypatorch-0.2.9/hypatorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypatorch
-Version: 0.2.8
+Version: 0.2.9
 Summary: HypaTorch: A library for abstract and visual model configuration
 Home-page: https://github.com/Altavo/hypatorch/
 Author: Altavo GmbH
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
```

### Comparing `hypatorch-0.2.8/setup.py` & `hypatorch-0.2.9/setup.py`

 * *Files identical despite different names*

