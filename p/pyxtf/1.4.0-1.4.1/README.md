# Comparing `tmp/pyxtf-1.4.0.tar.gz` & `tmp/pyxtf-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxtf-1.4.0.tar", last modified: Fri Dec  1 14:17:41 2023, max compression
+gzip compressed data, was "pyxtf-1.4.1.tar", last modified: Wed Apr 24 19:02:52 2024, max compression
```

## Comparing `pyxtf-1.4.0.tar` & `pyxtf-1.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 14:17:41.065253 pyxtf-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-12-01 14:17:18.000000 pyxtf-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2023-12-01 14:17:41.065253 pyxtf-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2023-12-01 14:17:18.000000 pyxtf-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-12-01 14:17:18.000000 pyxtf-1.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 14:17:41.061253 pyxtf-1.4.0/pyxtf/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-12-01 14:17:18.000000 pyxtf-1.4.0/pyxtf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7461 2023-12-01 14:17:18.000000 pyxtf-1.4.0/pyxtf/enumerations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 14:17:41.065253 pyxtf-1.4.0/pyxtf/vendors/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-01 14:17:18.000000 pyxtf-1.4.0/pyxtf/vendors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8887 2023-12-01 14:17:18.000000 pyxtf-1.4.0/pyxtf/vendors/kongsberg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5582 2023-12-01 14:17:18.000000 pyxtf-1.4.0/pyxtf/vendors/kongsberg.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    38574 2023-12-01 14:17:18.000000 pyxtf-1.4.0/pyxtf/xtf_ctypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    37164 2023-12-01 14:17:18.000000 pyxtf-1.4.0/pyxtf/xtf_ctypes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9876 2023-12-01 14:17:18.000000 pyxtf-1.4.0/pyxtf/xtf_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2023-12-01 14:17:18.000000 pyxtf-1.4.0/pyxtf/xtf_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 14:17:41.065253 pyxtf-1.4.0/pyxtf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2023-12-01 14:17:41.000000 pyxtf-1.4.0/pyxtf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      381 2023-12-01 14:17:41.000000 pyxtf-1.4.0/pyxtf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-01 14:17:41.000000 pyxtf-1.4.0/pyxtf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-01 14:17:41.000000 pyxtf-1.4.0/pyxtf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-01 14:17:41.000000 pyxtf-1.4.0/pyxtf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-01 14:17:41.065253 pyxtf-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2023-12-01 14:17:18.000000 pyxtf-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:02:52.004667 pyxtf-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-24 19:02:39.000000 pyxtf-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-24 19:02:52.004667 pyxtf-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-24 19:02:39.000000 pyxtf-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-24 19:02:39.000000 pyxtf-1.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:02:52.000667 pyxtf-1.4.1/pyxtf/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-24 19:02:39.000000 pyxtf-1.4.1/pyxtf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7461 2024-04-24 19:02:39.000000 pyxtf-1.4.1/pyxtf/enumerations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:02:52.000667 pyxtf-1.4.1/pyxtf/vendors/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 19:02:39.000000 pyxtf-1.4.1/pyxtf/vendors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8887 2024-04-24 19:02:39.000000 pyxtf-1.4.1/pyxtf/vendors/kongsberg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-04-24 19:02:39.000000 pyxtf-1.4.1/pyxtf/vendors/kongsberg.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    38491 2024-04-24 19:02:39.000000 pyxtf-1.4.1/pyxtf/xtf_ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37164 2024-04-24 19:02:39.000000 pyxtf-1.4.1/pyxtf/xtf_ctypes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-04-24 19:02:39.000000 pyxtf-1.4.1/pyxtf/xtf_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-24 19:02:39.000000 pyxtf-1.4.1/pyxtf/xtf_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:02:52.000667 pyxtf-1.4.1/pyxtf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-24 19:02:51.000000 pyxtf-1.4.1/pyxtf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-24 19:02:51.000000 pyxtf-1.4.1/pyxtf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:02:51.000000 pyxtf-1.4.1/pyxtf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-24 19:02:51.000000 pyxtf-1.4.1/pyxtf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 19:02:51.000000 pyxtf-1.4.1/pyxtf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:02:52.004667 pyxtf-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-24 19:02:39.000000 pyxtf-1.4.1/setup.py
```

### Comparing `pyxtf-1.4.0/LICENSE` & `pyxtf-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxtf-1.4.0/PKG-INFO` & `pyxtf-1.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxtf
-Version: 1.4.0
+Version: 1.4.1
 Summary: eXtended Triton Format (XTF) file interface
 Home-page: https://github.com/oysstu/pyxtf
 Author: Oystein Sture
 Author-email: oysstu@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/oysstu/pyxtf/issues
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyxtf-1.4.0/README.md` & `pyxtf-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pyxtf-1.4.0/pyxtf/enumerations.py` & `pyxtf-1.4.1/pyxtf/enumerations.py`

 * *Files identical despite different names*

### Comparing `pyxtf-1.4.0/pyxtf/vendors/kongsberg.py` & `pyxtf-1.4.1/pyxtf/vendors/kongsberg.py`

 * *Files identical despite different names*

### Comparing `pyxtf-1.4.0/pyxtf/vendors/kongsberg.pyi` & `pyxtf-1.4.1/pyxtf/vendors/kongsberg.pyi`

 * *Files identical despite different names*

### Comparing `pyxtf-1.4.0/pyxtf/xtf_ctypes.py` & `pyxtf-1.4.1/pyxtf/xtf_ctypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -734,17 +734,16 @@
     _pack_ = 1
     _fields_ = [
         ('Id', ctypes.c_int),
         ('Intensity', ctypes.c_double),
         ('Quality', ctypes.c_int),
         ('TwoWayTravelTime', ctypes.c_double),
         ('DeltaTime', ctypes.c_double),
-        ('OffsetX', ctypes.c_double),  # Number of bytes without padding (header+data)
-        ('OffsetY', ctypes.c_double),
-        ('OffsetZ', ctypes.c_double),
+        ('BeamAngle', ctypes.c_double),
+        ('TiltAngle', ctypes.c_double),
         ('Reserved', ctypes.c_float * 4)
     ]
 
 
 class XTFRawCustomHeader(XTFPacket):
     _pack_ = 1
     _fields_ = [
```

### Comparing `pyxtf-1.4.0/pyxtf/xtf_ctypes.pyi` & `pyxtf-1.4.1/pyxtf/xtf_ctypes.pyi`

 * *Files identical despite different names*

### Comparing `pyxtf-1.4.0/pyxtf/xtf_io.py` & `pyxtf-1.4.1/pyxtf/xtf_io.py`

 * *Files identical despite different names*

### Comparing `pyxtf-1.4.0/pyxtf/xtf_util.py` & `pyxtf-1.4.1/pyxtf/xtf_util.py`

 * *Files identical despite different names*

### Comparing `pyxtf-1.4.0/pyxtf.egg-info/PKG-INFO` & `pyxtf-1.4.1/pyxtf.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxtf
-Version: 1.4.0
+Version: 1.4.1
 Summary: eXtended Triton Format (XTF) file interface
 Home-page: https://github.com/oysstu/pyxtf
 Author: Oystein Sture
 Author-email: oysstu@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/oysstu/pyxtf/issues
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyxtf-1.4.0/setup.py` & `pyxtf-1.4.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     # read the contents of README file
     this_directory = path.abspath(path.dirname(__file__))
     with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
         long_description = f.read()
 
     # Run setup script
     setup(name='pyxtf',
-          version='1.4.0',
+          version='1.4.1',
           description='eXtended Triton Format (XTF) file interface',
           long_description=long_description,
           long_description_content_type='text/markdown',
           author='Oystein Sture',
           author_email='oysstu@gmail.com',
           url='https://github.com/oysstu/pyxtf',
           project_urls={
```

