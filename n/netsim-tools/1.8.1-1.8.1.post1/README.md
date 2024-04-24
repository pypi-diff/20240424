# Comparing `tmp/netsim-tools-1.8.1.tar.gz` & `tmp/netsim_tools-1.8.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsim-tools-1.8.1.tar", last modified: Mon Apr  8 09:31:08 2024, max compression
+gzip compressed data, was "netsim_tools-1.8.1.post1.tar", last modified: Wed Apr 24 08:34:00 2024, max compression
```

## Comparing `netsim-tools-1.8.1.tar` & `netsim_tools-1.8.1.post1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:31:08.900160 netsim-tools-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-08 09:31:08.900160 netsim-tools-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-08 09:30:50.000000 netsim-tools-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:31:08.900160 netsim-tools-1.8.1/netsim_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-08 09:31:08.000000 netsim-tools-1.8.1/netsim_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-08 09:31:08.000000 netsim-tools-1.8.1/netsim_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:31:08.000000 netsim-tools-1.8.1/netsim_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-08 09:31:08.000000 netsim-tools-1.8.1/netsim_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:31:08.000000 netsim-tools-1.8.1/netsim_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 09:31:08.900160 netsim-tools-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-08 09:30:50.000000 netsim-tools-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:34:00.702518 netsim_tools-1.8.1.post1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-24 08:34:00.702518 netsim_tools-1.8.1.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-24 08:33:44.000000 netsim_tools-1.8.1.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:34:00.698518 netsim_tools-1.8.1.post1/netsim_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-24 08:34:00.000000 netsim_tools-1.8.1.post1/netsim_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-24 08:34:00.000000 netsim_tools-1.8.1.post1/netsim_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:34:00.000000 netsim_tools-1.8.1.post1/netsim_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 08:34:00.000000 netsim_tools-1.8.1.post1/netsim_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:34:00.000000 netsim_tools-1.8.1.post1/netsim_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 08:34:00.702518 netsim_tools-1.8.1.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-24 08:33:44.000000 netsim_tools-1.8.1.post1/setup.py
```

### Comparing `netsim-tools-1.8.1/PKG-INFO` & `netsim_tools-1.8.1.post1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: netsim-tools
-Version: 1.8.1
+Version: 1.8.1.post1
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
-Requires-Python: >=3.7
-Requires-Dist: networklab>=1.8.1
+Requires-Python: >=3.8
+Requires-Dist: networklab>=1.8.1-post1
 
 netsim-tools has been renamed to netlab in August 2022.
 
 The Python package netsim-tools has been renamed to networklab and is
 installed as a dependency of netsim-tools every time you install or
 upgrade netsim-tools, but we won't keep that dependency active foreer.
```

### Comparing `netsim-tools-1.8.1/netsim_tools.egg-info/PKG-INFO` & `netsim_tools-1.8.1.post1/netsim_tools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: netsim-tools
-Version: 1.8.1
+Version: 1.8.1.post1
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
-Requires-Python: >=3.7
-Requires-Dist: networklab>=1.8.1
+Requires-Python: >=3.8
+Requires-Dist: networklab>=1.8.1-post1
 
 netsim-tools has been renamed to netlab in August 2022.
 
 The Python package netsim-tools has been renamed to networklab and is
 installed as a dependency of netsim-tools every time you install or
 upgrade netsim-tools, but we won't keep that dependency active foreer.
```

### Comparing `netsim-tools-1.8.1/setup.py` & `netsim_tools-1.8.1.post1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ redirect netsim-tools to networklab """
 import sys
 from setuptools import setup, find_packages
 from pathlib import Path
 
 sys.path.append('..')
 
-version="1.8.1"
+version="1.8.1-post1"
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
   name="netsim-tools",
   version=version,
   packages=[],
@@ -19,13 +19,16 @@
   long_description=long_description,
   install_requires=[f"networklab>={version}"],
   classifiers=[
     "Topic :: Utilities",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS",
   ],
   url="https://github.com/ipspace/netlab",
-  python_requires='>=3.7',  # Due to e.g. 'capture_output' in subprocess.run
+  python_requires='>=3.8',  # Due to e.g. 'capture_output' in subprocess.run
 )
```

