# Comparing `tmp/davml-1.1.tar.gz` & `tmp/davml-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "davml-1.1.tar", last modified: Tue Apr 23 18:43:25 2024, max compression
+gzip compressed data, was "davml-1.1.1.tar", last modified: Tue Apr 23 18:45:04 2024, max compression
```

## Comparing `davml-1.1.tar` & `davml-1.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 18:43:25.906337 davml-1.1/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      191 2024-04-23 18:43:25.906337 davml-1.1/PKG-INFO
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 18:43:25.906337 davml-1.1/davml/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 17:31:37.000000 davml-1.1/davml/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      642 2024-04-23 18:00:43.000000 davml-1.1/davml/p1.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1489 2024-04-23 18:00:57.000000 davml-1.1/davml/p2.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1483 2024-04-23 18:01:12.000000 davml-1.1/davml/p3.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1705 2024-04-23 18:01:28.000000 davml-1.1/davml/p4.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1730 2024-04-23 18:01:39.000000 davml-1.1/davml/p5.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4111 2024-04-23 18:01:51.000000 davml-1.1/davml/p6.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2383 2024-04-23 18:02:06.000000 davml-1.1/davml/p7.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    13790 2024-04-23 17:48:59.000000 davml-1.1/davml/program.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1708 2024-04-23 18:42:28.000000 davml-1.1/davml/programs.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 18:43:25.906337 davml-1.1/davml.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      191 2024-04-23 18:43:25.000000 davml-1.1/davml.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      321 2024-04-23 18:43:25.000000 davml-1.1/davml.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2024-04-23 18:43:25.000000 davml-1.1/davml.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       46 2024-04-23 18:43:25.000000 davml-1.1/davml.egg-info/entry_points.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       10 2024-04-23 18:43:25.000000 davml-1.1/davml.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        6 2024-04-23 18:43:25.000000 davml-1.1/davml.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2024-04-23 18:43:25.906337 davml-1.1/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      418 2024-04-23 18:43:14.000000 davml-1.1/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 18:45:04.774243 davml-1.1.1/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      193 2024-04-23 18:45:04.770243 davml-1.1.1/PKG-INFO
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 18:45:04.770243 davml-1.1.1/davml/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 17:31:37.000000 davml-1.1.1/davml/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      642 2024-04-23 18:00:43.000000 davml-1.1.1/davml/p1.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1489 2024-04-23 18:00:57.000000 davml-1.1.1/davml/p2.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1483 2024-04-23 18:01:12.000000 davml-1.1.1/davml/p3.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1705 2024-04-23 18:01:28.000000 davml-1.1.1/davml/p4.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1730 2024-04-23 18:01:39.000000 davml-1.1.1/davml/p5.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4111 2024-04-23 18:01:51.000000 davml-1.1.1/davml/p6.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2383 2024-04-23 18:02:06.000000 davml-1.1.1/davml/p7.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    13790 2024-04-23 17:48:59.000000 davml-1.1.1/davml/program.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1702 2024-04-23 18:44:46.000000 davml-1.1.1/davml/programs.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 18:45:04.770243 davml-1.1.1/davml.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      193 2024-04-23 18:45:04.000000 davml-1.1.1/davml.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      321 2024-04-23 18:45:04.000000 davml-1.1.1/davml.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2024-04-23 18:45:04.000000 davml-1.1.1/davml.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       46 2024-04-23 18:45:04.000000 davml-1.1.1/davml.egg-info/entry_points.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       10 2024-04-23 18:45:04.000000 davml-1.1.1/davml.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        6 2024-04-23 18:45:04.000000 davml-1.1.1/davml.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2024-04-23 18:45:04.774243 davml-1.1.1/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      420 2024-04-23 18:44:53.000000 davml-1.1.1/setup.py
```

### Comparing `davml-1.1/davml/p1.py` & `davml-1.1.1/davml/p1.py`

 * *Files identical despite different names*

### Comparing `davml-1.1/davml/p2.py` & `davml-1.1.1/davml/p2.py`

 * *Files identical despite different names*

### Comparing `davml-1.1/davml/p3.py` & `davml-1.1.1/davml/p3.py`

 * *Files identical despite different names*

### Comparing `davml-1.1/davml/p4.py` & `davml-1.1.1/davml/p4.py`

 * *Files identical despite different names*

### Comparing `davml-1.1/davml/p5.py` & `davml-1.1.1/davml/p5.py`

 * *Files identical despite different names*

### Comparing `davml-1.1/davml/p6.py` & `davml-1.1.1/davml/p6.py`

 * *Files identical despite different names*

### Comparing `davml-1.1/davml/p7.py` & `davml-1.1.1/davml/p7.py`

 * *Files identical despite different names*

### Comparing `davml-1.1/davml/program.py` & `davml-1.1.1/davml/program.py`

 * *Files identical despite different names*

### Comparing `davml-1.1/davml/programs.py` & `davml-1.1.1/davml/programs.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     else:
         try:
             # Argument provided, try to convert it to an integer
             idx = int(sys.argv[1]) - 1
             if 0 <= idx < len(titles):
                 # Valid index provided
                 current_directory = os.path.dirname(os.path.realpath(__file__))
-                file_name = f"program{idx + 1}.py"
+                file_name = f"p{idx + 1}.py"
                 file_path = os.path.join(current_directory, file_name)
                 
                 if len(sys.argv) > 2 and sys.argv[2] == 'p':
                     # Print complete code to terminal
                     with open(file_path, 'r') as file:
                         code = file.read()
                         print(f"Code from {file_name}:\n")
```

