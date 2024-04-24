# Comparing `tmp/seamm_exec-2024.4.22.tar.gz` & `tmp/seamm_exec-2024.4.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seamm_exec-2024.4.22.tar", last modified: Mon Apr 22 20:04:48 2024, max compression
+gzip compressed data, was "seamm_exec-2024.4.24.tar", last modified: Wed Apr 24 21:54:55 2024, max compression
```

## Comparing `seamm_exec-2024.4.22.tar` & `seamm_exec-2024.4.24.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:04:48.022174 seamm_exec-2024.4.22/
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-22 20:04:22.000000 seamm_exec-2024.4.22/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-22 20:04:22.000000 seamm_exec-2024.4.22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-22 20:04:22.000000 seamm_exec-2024.4.22/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-22 20:04:48.022174 seamm_exec-2024.4.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-22 20:04:22.000000 seamm_exec-2024.4.22/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-22 20:04:22.000000 seamm_exec-2024.4.22/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:04:48.022174 seamm_exec-2024.4.22/seamm_exec/
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-22 20:04:22.000000 seamm_exec-2024.4.22/seamm_exec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-22 20:04:47.000000 seamm_exec-2024.4.22/seamm_exec/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-04-22 20:04:22.000000 seamm_exec-2024.4.22/seamm_exec/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-22 20:04:22.000000 seamm_exec-2024.4.22/seamm_exec/computational_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-04-22 20:04:22.000000 seamm_exec-2024.4.22/seamm_exec/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)    27614 2024-04-22 20:04:22.000000 seamm_exec-2024.4.22/seamm_exec/exec_flowchart.py
--rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-04-22 20:04:22.000000 seamm_exec-2024.4.22/seamm_exec/local.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-22 20:04:22.000000 seamm_exec-2024.4.22/seamm_exec/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-22 20:04:22.000000 seamm_exec-2024.4.22/seamm_exec/seamm_exec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:04:48.022174 seamm_exec-2024.4.22/seamm_exec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-22 20:04:48.000000 seamm_exec-2024.4.22/seamm_exec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-22 20:04:48.000000 seamm_exec-2024.4.22/seamm_exec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 20:04:48.000000 seamm_exec-2024.4.22/seamm_exec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-22 20:04:48.000000 seamm_exec-2024.4.22/seamm_exec.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 20:04:30.000000 seamm_exec-2024.4.22/seamm_exec.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-22 20:04:48.000000 seamm_exec-2024.4.22/seamm_exec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-22 20:04:48.000000 seamm_exec-2024.4.22/seamm_exec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-22 20:04:48.022174 seamm_exec-2024.4.22/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:04:48.022174 seamm_exec-2024.4.22/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-22 20:04:22.000000 seamm_exec-2024.4.22/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-22 20:04:22.000000 seamm_exec-2024.4.22/tests/test_seamm_exec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:54:55.698193 seamm_exec-2024.4.24/
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-24 21:54:55.698193 seamm_exec-2024.4.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:54:55.694193 seamm_exec-2024.4.24/seamm_exec/
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/seamm_exec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-24 21:54:55.000000 seamm_exec-2024.4.24/seamm_exec/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12536 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/seamm_exec/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/seamm_exec/computational_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/seamm_exec/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27614 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/seamm_exec/exec_flowchart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/seamm_exec/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/seamm_exec/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/seamm_exec/seamm_exec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:54:55.694193 seamm_exec-2024.4.24/seamm_exec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-24 21:54:55.000000 seamm_exec-2024.4.24/seamm_exec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-24 21:54:55.000000 seamm_exec-2024.4.24/seamm_exec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 21:54:55.000000 seamm_exec-2024.4.24/seamm_exec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-24 21:54:55.000000 seamm_exec-2024.4.24/seamm_exec.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 21:54:50.000000 seamm_exec-2024.4.24/seamm_exec.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-24 21:54:55.000000 seamm_exec-2024.4.24/seamm_exec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-24 21:54:55.000000 seamm_exec-2024.4.24/seamm_exec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-24 21:54:55.698193 seamm_exec-2024.4.24/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:54:55.694193 seamm_exec-2024.4.24/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-24 21:54:47.000000 seamm_exec-2024.4.24/tests/test_seamm_exec.py
```

### Comparing `seamm_exec-2024.4.22/CODE_OF_CONDUCT.md` & `seamm_exec-2024.4.24/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.22/LICENSE` & `seamm_exec-2024.4.24/LICENSE`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.22/PKG-INFO` & `seamm_exec-2024.4.24/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seamm_exec
-Version: 2024.4.22
+Version: 2024.4.24
 Summary: Classes to execute background codes for SEAMM
 Author-email: Paul Saxe <psaxe@molssi.org>
 License: MIT
 Project-URL: Source, https://github.com/molssi-seamm/seamm_exec/
 Project-URL: Documentation, https://molssi-seamm.github.io/
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `seamm_exec-2024.4.22/README.md` & `seamm_exec-2024.4.24/README.md`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.22/pyproject.toml` & `seamm_exec-2024.4.24/pyproject.toml`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.22/seamm_exec/__init__.py` & `seamm_exec-2024.4.24/seamm_exec/__init__.py`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.22/seamm_exec/base.py` & `seamm_exec-2024.4.24/seamm_exec/base.py`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.22/seamm_exec/computational_environment.py` & `seamm_exec-2024.4.24/seamm_exec/computational_environment.py`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.22/seamm_exec/docker.py` & `seamm_exec-2024.4.24/seamm_exec/docker.py`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.22/seamm_exec/exec_flowchart.py` & `seamm_exec-2024.4.24/seamm_exec/exec_flowchart.py`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.22/seamm_exec/local.py` & `seamm_exec-2024.4.24/seamm_exec/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,14 +156,18 @@
                 tmp = command
                 while True:
                     command = tmp.format(**config, **ce)
                     if tmp == command:
                         break
                     tmp = command
 
+                # If running using Docker, we have to munge any paths in the command
+                prefix = str(directory)
+                command = command.replace(prefix, "/home")
+
                 self.logger.debug(
                     f"""
                     result = client.containers.run(
                         command={command},
                         environment={env},
                         image={container},
                         platform={platform},
```

### Comparing `seamm_exec-2024.4.22/seamm_exec/seamm_exec.py` & `seamm_exec-2024.4.24/seamm_exec/seamm_exec.py`

 * *Files identical despite different names*

### Comparing `seamm_exec-2024.4.22/seamm_exec.egg-info/PKG-INFO` & `seamm_exec-2024.4.24/seamm_exec.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seamm_exec
-Version: 2024.4.22
+Version: 2024.4.24
 Summary: Classes to execute background codes for SEAMM
 Author-email: Paul Saxe <psaxe@molssi.org>
 License: MIT
 Project-URL: Source, https://github.com/molssi-seamm/seamm_exec/
 Project-URL: Documentation, https://molssi-seamm.github.io/
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `seamm_exec-2024.4.22/seamm_exec.egg-info/SOURCES.txt` & `seamm_exec-2024.4.24/seamm_exec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

