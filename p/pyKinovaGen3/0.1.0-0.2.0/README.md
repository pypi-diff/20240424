# Comparing `tmp/pyKinovaGen3-0.1.0.tar.gz` & `tmp/pykinovagen3-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyKinovaGen3-0.1.0.tar", last modified: Thu Mar 14 10:37:16 2024, max compression
+gzip compressed data, was "pykinovagen3-0.2.0.tar", last modified: Wed Apr 24 11:50:02 2024, max compression
```

## Comparing `pyKinovaGen3-0.1.0.tar` & `pykinovagen3-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 10:37:16.989113 pyKinovaGen3-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-14 10:37:11.000000 pyKinovaGen3-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-14 10:37:16.989113 pyKinovaGen3-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-14 10:37:11.000000 pyKinovaGen3-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 10:37:16.985113 pyKinovaGen3-0.1.0/kinova_gen3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 10:37:11.000000 pyKinovaGen3-0.1.0/kinova_gen3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 10:37:16.985113 pyKinovaGen3-0.1.0/kinova_gen3/dynamics/
--rw-r--r--   0 runner    (1001) docker     (127)   105422 2024-03-14 10:37:11.000000 pyKinovaGen3-0.1.0/kinova_gen3/dynamics/coriolis.py
--rw-r--r--   0 runner    (1001) docker     (127)    13110 2024-03-14 10:37:11.000000 pyKinovaGen3-0.1.0/kinova_gen3/dynamics/gravity.py
--rw-r--r--   0 runner    (1001) docker     (127)   139635 2024-03-14 10:37:11.000000 pyKinovaGen3-0.1.0/kinova_gen3/dynamics/mass_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 10:37:16.989113 pyKinovaGen3-0.1.0/kinova_gen3/kinematics/
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-03-14 10:37:11.000000 pyKinovaGen3-0.1.0/kinova_gen3/kinematics/forward_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-03-14 10:37:11.000000 pyKinovaGen3-0.1.0/kinova_gen3/kinematics/inverse_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7117 2024-03-14 10:37:11.000000 pyKinovaGen3-0.1.0/kinova_gen3/kinematics/jacobian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 10:37:16.989113 pyKinovaGen3-0.1.0/kinova_gen3/performance_criteria/
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-14 10:37:11.000000 pyKinovaGen3-0.1.0/kinova_gen3/performance_criteria/joint_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-03-14 10:37:11.000000 pyKinovaGen3-0.1.0/kinova_gen3/performance_criteria/manipulability.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 10:37:16.989113 pyKinovaGen3-0.1.0/pyKinovaGen3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-14 10:37:16.000000 pyKinovaGen3-0.1.0/pyKinovaGen3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-14 10:37:16.000000 pyKinovaGen3-0.1.0/pyKinovaGen3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 10:37:16.000000 pyKinovaGen3-0.1.0/pyKinovaGen3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-14 10:37:16.000000 pyKinovaGen3-0.1.0/pyKinovaGen3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-14 10:37:16.000000 pyKinovaGen3-0.1.0/pyKinovaGen3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-03-14 10:37:11.000000 pyKinovaGen3-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 10:37:16.989113 pyKinovaGen3-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 10:37:16.989113 pyKinovaGen3-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-03-14 10:37:11.000000 pyKinovaGen3-0.1.0/tests/test_forward_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-14 10:37:11.000000 pyKinovaGen3-0.1.0/tests/test_gravity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:50:02.273230 pykinovagen3-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-24 11:49:55.000000 pykinovagen3-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-24 11:50:02.273230 pykinovagen3-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-24 11:49:55.000000 pykinovagen3-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:50:02.269230 pykinovagen3-0.2.0/kinova_gen3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:49:55.000000 pykinovagen3-0.2.0/kinova_gen3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:50:02.269230 pykinovagen3-0.2.0/kinova_gen3/dynamics/
+-rw-r--r--   0 runner    (1001) docker     (127)   105422 2024-04-24 11:49:55.000000 pykinovagen3-0.2.0/kinova_gen3/dynamics/coriolis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13110 2024-04-24 11:49:55.000000 pykinovagen3-0.2.0/kinova_gen3/dynamics/gravity.py
+-rw-r--r--   0 runner    (1001) docker     (127)   139635 2024-04-24 11:49:55.000000 pykinovagen3-0.2.0/kinova_gen3/dynamics/mass_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:50:02.269230 pykinovagen3-0.2.0/kinova_gen3/kinematics/
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-24 11:49:55.000000 pykinovagen3-0.2.0/kinova_gen3/kinematics/forward_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-04-24 11:49:55.000000 pykinovagen3-0.2.0/kinova_gen3/kinematics/inverse_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24174 2024-04-24 11:49:55.000000 pykinovagen3-0.2.0/kinova_gen3/kinematics/jacobian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:50:02.269230 pykinovagen3-0.2.0/kinova_gen3/performance_criteria/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-24 11:49:55.000000 pykinovagen3-0.2.0/kinova_gen3/performance_criteria/joint_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-24 11:49:55.000000 pykinovagen3-0.2.0/kinova_gen3/performance_criteria/manipulability.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:50:02.273230 pykinovagen3-0.2.0/pyKinovaGen3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-24 11:50:02.000000 pykinovagen3-0.2.0/pyKinovaGen3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-24 11:50:02.000000 pykinovagen3-0.2.0/pyKinovaGen3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 11:50:02.000000 pykinovagen3-0.2.0/pyKinovaGen3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 11:50:02.000000 pykinovagen3-0.2.0/pyKinovaGen3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 11:50:02.000000 pykinovagen3-0.2.0/pyKinovaGen3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-24 11:49:55.000000 pykinovagen3-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 11:50:02.273230 pykinovagen3-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:50:02.273230 pykinovagen3-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-24 11:49:55.000000 pykinovagen3-0.2.0/tests/test_forward_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-24 11:49:55.000000 pykinovagen3-0.2.0/tests/test_gravity.py
```

### Comparing `pyKinovaGen3-0.1.0/LICENSE` & `pykinovagen3-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyKinovaGen3-0.1.0/PKG-INFO` & `pykinovagen3-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyKinovaGen3
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python package for the kinematics and dynamics of Kinova Gen3
 Author-email: Ozan Tokatli <ozan.tokatli@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Documentation, https://pykinovagen3.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyKinovaGen3-0.1.0/kinova_gen3/dynamics/coriolis.py` & `pykinovagen3-0.2.0/kinova_gen3/dynamics/coriolis.py`

 * *Files identical despite different names*

### Comparing `pyKinovaGen3-0.1.0/kinova_gen3/dynamics/gravity.py` & `pykinovagen3-0.2.0/kinova_gen3/dynamics/gravity.py`

 * *Files identical despite different names*

### Comparing `pyKinovaGen3-0.1.0/kinova_gen3/dynamics/mass_matrix.py` & `pykinovagen3-0.2.0/kinova_gen3/dynamics/mass_matrix.py`

 * *Files identical despite different names*

### Comparing `pyKinovaGen3-0.1.0/kinova_gen3/kinematics/forward_kinematics.py` & `pykinovagen3-0.2.0/kinova_gen3/kinematics/forward_kinematics.py`

 * *Files identical despite different names*

### Comparing `pyKinovaGen3-0.1.0/kinova_gen3/kinematics/inverse_kinematics.py` & `pykinovagen3-0.2.0/kinova_gen3/kinematics/inverse_kinematics.py`

 * *Files identical despite different names*

### Comparing `pyKinovaGen3-0.1.0/kinova_gen3/performance_criteria/joint_limits.py` & `pykinovagen3-0.2.0/kinova_gen3/performance_criteria/joint_limits.py`

 * *Files identical despite different names*

### Comparing `pyKinovaGen3-0.1.0/kinova_gen3/performance_criteria/manipulability.py` & `pykinovagen3-0.2.0/kinova_gen3/performance_criteria/manipulability.py`

 * *Files identical despite different names*

### Comparing `pyKinovaGen3-0.1.0/pyKinovaGen3.egg-info/PKG-INFO` & `pykinovagen3-0.2.0/pyKinovaGen3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyKinovaGen3
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python package for the kinematics and dynamics of Kinova Gen3
 Author-email: Ozan Tokatli <ozan.tokatli@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Documentation, https://pykinovagen3.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyKinovaGen3-0.1.0/pyKinovaGen3.egg-info/SOURCES.txt` & `pykinovagen3-0.2.0/pyKinovaGen3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyKinovaGen3-0.1.0/pyproject.toml` & `pykinovagen3-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyKinovaGen3"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="Ozan Tokatli", email="ozan.tokatli@gmail.com" },
 ]
 description = "Python package for the kinematics and dynamics of Kinova Gen3"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `pyKinovaGen3-0.1.0/tests/test_forward_kinematics.py` & `pykinovagen3-0.2.0/tests/test_forward_kinematics.py`

 * *Files identical despite different names*

### Comparing `pyKinovaGen3-0.1.0/tests/test_gravity.py` & `pykinovagen3-0.2.0/tests/test_gravity.py`

 * *Files identical despite different names*

