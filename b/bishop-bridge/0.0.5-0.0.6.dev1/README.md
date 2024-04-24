# Comparing `tmp/bishop-bridge-0.0.5.tar.gz` & `tmp/bishop_bridge-0.0.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bishop-bridge-0.0.5.tar", last modified: Thu Dec  7 01:03:41 2023, max compression
+gzip compressed data, was "bishop_bridge-0.0.6.dev1.tar", last modified: Wed Apr 24 19:28:49 2024, max compression
```

## Comparing `bishop-bridge-0.0.5.tar` & `bishop_bridge-0.0.6.dev1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 01:03:41.277763 bishop-bridge-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2023-12-07 01:03:27.000000 bishop-bridge-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      553 2023-12-07 01:03:41.277763 bishop-bridge-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-07 01:03:27.000000 bishop-bridge-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 01:03:41.277763 bishop-bridge-0.0.5/bishop_bridge/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-12-07 01:03:27.000000 bishop-bridge-0.0.5/bishop_bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2023-12-07 01:03:27.000000 bishop-bridge-0.0.5/bishop_bridge/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 01:03:41.277763 bishop-bridge-0.0.5/bishop_bridge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2023-12-07 01:03:41.000000 bishop-bridge-0.0.5/bishop_bridge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2023-12-07 01:03:41.000000 bishop-bridge-0.0.5/bishop_bridge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-07 01:03:41.000000 bishop-bridge-0.0.5/bishop_bridge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-07 01:03:41.000000 bishop-bridge-0.0.5/bishop_bridge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-07 01:03:41.000000 bishop-bridge-0.0.5/bishop_bridge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      508 2023-12-07 01:03:27.000000 bishop-bridge-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-07 01:03:41.277763 bishop-bridge-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:28:49.566896 bishop_bridge-0.0.6.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-24 19:28:43.000000 bishop_bridge-0.0.6.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-24 19:28:49.566896 bishop_bridge-0.0.6.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:28:43.000000 bishop_bridge-0.0.6.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:28:49.566896 bishop_bridge-0.0.6.dev1/bishop_bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-24 19:28:43.000000 bishop_bridge-0.0.6.dev1/bishop_bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-24 19:28:43.000000 bishop_bridge-0.0.6.dev1/bishop_bridge/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:28:49.566896 bishop_bridge-0.0.6.dev1/bishop_bridge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-24 19:28:49.000000 bishop_bridge-0.0.6.dev1/bishop_bridge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-24 19:28:49.000000 bishop_bridge-0.0.6.dev1/bishop_bridge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:28:49.000000 bishop_bridge-0.0.6.dev1/bishop_bridge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 19:28:49.000000 bishop_bridge-0.0.6.dev1/bishop_bridge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 19:28:49.000000 bishop_bridge-0.0.6.dev1/bishop_bridge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-24 19:28:43.000000 bishop_bridge-0.0.6.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:28:49.566896 bishop_bridge-0.0.6.dev1/setup.cfg
```

### Comparing `bishop-bridge-0.0.5/LICENSE` & `bishop_bridge-0.0.6.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `bishop-bridge-0.0.5/PKG-INFO` & `bishop_bridge-0.0.6.dev1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bishop-bridge
-Version: 0.0.5
+Version: 0.0.6.dev1
 Summary: A package for creating a Bishop bridge
 Author-email: Noah Hunn <nhunn@calvaryrobotics.com>
 Project-URL: Homepage, https://github.com/CalvaryDesign/bishop-bridge
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `bishop-bridge-0.0.5/bishop_bridge/bridge.py` & `bishop_bridge-0.0.6.dev1/bishop_bridge/bridge.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,20 +74,24 @@
         """
         if path == "/":
             return self.data
 
         keys = path.strip("/").split("/")
         current_dict = self.data
 
-        for key in keys:
-            if key in current_dict:
-                current_dict = current_dict[key]
-            else:
-                return None
-        return current_dict
+        try:
+            for key in keys:
+                if key in current_dict:
+                    current_dict = current_dict[key]
+                else:
+                    return None
+            return current_dict
+        except TypeError:
+            print("Error: path must be a string")
+            return None
 
     def set_data(self, path: str, value: any):
         """
         Set the data at the given path to the given value.
         """
         keys = path.strip("/").split("/")
         current_dict = self.data
```

### Comparing `bishop-bridge-0.0.5/bishop_bridge.egg-info/PKG-INFO` & `bishop_bridge-0.0.6.dev1/bishop_bridge.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bishop-bridge
-Version: 0.0.5
+Version: 0.0.6.dev1
 Summary: A package for creating a Bishop bridge
 Author-email: Noah Hunn <nhunn@calvaryrobotics.com>
 Project-URL: Homepage, https://github.com/CalvaryDesign/bishop-bridge
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

