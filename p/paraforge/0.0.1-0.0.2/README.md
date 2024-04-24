# Comparing `tmp/paraforge-0.0.1.tar.gz` & `tmp/paraforge-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paraforge-0.0.1.tar", last modified: Wed Apr 24 06:05:14 2024, max compression
+gzip compressed data, was "paraforge-0.0.2.tar", last modified: Wed Apr 24 06:22:19 2024, max compression
```

## Comparing `paraforge-0.0.1.tar` & `paraforge-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 den-antares  (1000) den-antares  (1000)        0 2024-04-24 06:05:14.068880 paraforge-0.0.1/
--rw-r--r--   0 den-antares  (1000) den-antares  (1000)       34 2024-04-24 06:03:24.000000 paraforge-0.0.1/MANIFEST.in
--rw-r--r--   0 den-antares  (1000) den-antares  (1000)      528 2024-04-24 06:05:14.068880 paraforge-0.0.1/PKG-INFO
--rw-r--r--   0 den-antares  (1000) den-antares  (1000)       89 2024-04-18 23:18:28.000000 paraforge-0.0.1/README.md
-drwxr-xr-x   0 den-antares  (1000) den-antares  (1000)        0 2024-04-24 06:05:14.066880 paraforge-0.0.1/paraforge/
--rw-r--r--   0 den-antares  (1000) den-antares  (1000)     1128 2024-04-24 05:42:05.000000 paraforge-0.0.1/paraforge/__init__.py
--rwxr-xr-x   0 den-antares  (1000) den-antares  (1000)   422984 2024-04-24 05:27:49.000000 paraforge-0.0.1/paraforge/libparaforge.so
-drwxr-xr-x   0 den-antares  (1000) den-antares  (1000)        0 2024-04-24 06:05:14.067880 paraforge-0.0.1/paraforge.egg-info/
--rw-r--r--   0 den-antares  (1000) den-antares  (1000)      528 2024-04-24 06:05:14.000000 paraforge-0.0.1/paraforge.egg-info/PKG-INFO
--rw-r--r--   0 den-antares  (1000) den-antares  (1000)      210 2024-04-24 06:05:14.000000 paraforge-0.0.1/paraforge.egg-info/SOURCES.txt
--rw-r--r--   0 den-antares  (1000) den-antares  (1000)        1 2024-04-24 06:05:14.000000 paraforge-0.0.1/paraforge.egg-info/dependency_links.txt
--rw-r--r--   0 den-antares  (1000) den-antares  (1000)       10 2024-04-24 06:05:14.000000 paraforge-0.0.1/paraforge.egg-info/top_level.txt
--rw-r--r--   0 den-antares  (1000) den-antares  (1000)       38 2024-04-24 06:05:14.068880 paraforge-0.0.1/setup.cfg
--rw-r--r--   0 den-antares  (1000) den-antares  (1000)      750 2024-04-24 06:05:09.000000 paraforge-0.0.1/setup.py
+drwxr-xr-x   0 den-antares  (1000) den-antares  (1000)        0 2024-04-24 06:22:19.683053 paraforge-0.0.2/
+-rw-r--r--   0 den-antares  (1000) den-antares  (1000)       34 2024-04-24 06:20:57.000000 paraforge-0.0.2/MANIFEST.in
+-rw-r--r--   0 den-antares  (1000) den-antares  (1000)      548 2024-04-24 06:22:19.683053 paraforge-0.0.2/PKG-INFO
+-rw-r--r--   0 den-antares  (1000) den-antares  (1000)       89 2024-04-24 06:20:57.000000 paraforge-0.0.2/README.md
+drwxr-xr-x   0 den-antares  (1000) den-antares  (1000)        0 2024-04-24 06:22:19.682053 paraforge-0.0.2/paraforge/
+-rw-r--r--   0 den-antares  (1000) den-antares  (1000)     1135 2024-04-24 06:20:57.000000 paraforge-0.0.2/paraforge/__init__.py
+drwxr-xr-x   0 den-antares  (1000) den-antares  (1000)        0 2024-04-24 06:22:19.683053 paraforge-0.0.2/paraforge.egg-info/
+-rw-r--r--   0 den-antares  (1000) den-antares  (1000)      548 2024-04-24 06:22:19.000000 paraforge-0.0.2/paraforge.egg-info/PKG-INFO
+-rw-r--r--   0 den-antares  (1000) den-antares  (1000)      216 2024-04-24 06:22:19.000000 paraforge-0.0.2/paraforge.egg-info/SOURCES.txt
+-rw-r--r--   0 den-antares  (1000) den-antares  (1000)        1 2024-04-24 06:22:19.000000 paraforge-0.0.2/paraforge.egg-info/dependency_links.txt
+-rw-r--r--   0 den-antares  (1000) den-antares  (1000)        5 2024-04-24 06:22:19.000000 paraforge-0.0.2/paraforge.egg-info/requires.txt
+-rw-r--r--   0 den-antares  (1000) den-antares  (1000)       10 2024-04-24 06:22:19.000000 paraforge-0.0.2/paraforge.egg-info/top_level.txt
+-rw-r--r--   0 den-antares  (1000) den-antares  (1000)       38 2024-04-24 06:22:19.683053 paraforge-0.0.2/setup.cfg
+-rw-r--r--   0 den-antares  (1000) den-antares  (1000)      796 2024-04-24 06:20:57.000000 paraforge-0.0.2/setup.py
```

### Comparing `paraforge-0.0.1/PKG-INFO` & `paraforge-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: paraforge
-Version: 0.0.1
+Version: 0.0.2
 Summary: Evaluation of a Python-Rust architecture for a parametric modeling project
 Home-page: https://github.com/Densaugeo/paraforge
 Author: Densaugeo
 Author-email: author@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Rust
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
+Requires-Dist: cffi
 
 # Paraforge
 
 Evaluation of a Python-Rust architecture for a parametric modeling project.
```

### Comparing `paraforge-0.0.1/paraforge/__init__.py` & `paraforge-0.0.2/paraforge/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-import cffi, ctypes, os, enum
+import ctypes, os, enum
+
+import cffi
 
 
 class ErrorCode(enum.Enum):
     None_ = 0
     Mutex = 1
     Generation = 2
     NotImplemented = 3
```

### Comparing `paraforge-0.0.1/paraforge.egg-info/PKG-INFO` & `paraforge-0.0.2/paraforge.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: paraforge
-Version: 0.0.1
+Version: 0.0.2
 Summary: Evaluation of a Python-Rust architecture for a parametric modeling project
 Home-page: https://github.com/Densaugeo/paraforge
 Author: Densaugeo
 Author-email: author@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Rust
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
+Requires-Dist: cffi
 
 # Paraforge
 
 Evaluation of a Python-Rust architecture for a parametric modeling project.
```

### Comparing `paraforge-0.0.1/setup.py` & `paraforge-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='paraforge',
-    version='0.0.1',
+    version='0.0.2',
     author='Densaugeo',
     author_email='author@example.com',
     description='Evaluation of a Python-Rust architecture for a parametric modeling project',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Densaugeo/paraforge',
     packages=['paraforge'],
@@ -19,8 +19,11 @@
     classifiers=[
         'Programming Language :: Python :: 3',
         'Programming Language :: Rust',
         #'License :: TBD',
         'Operating System :: POSIX :: Linux',
     ],
     python_requires='>=3.12',
+    install_requires=[
+        'cffi',
+    ],
 )
```

