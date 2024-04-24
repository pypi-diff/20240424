# Comparing `tmp/mpu6050-0.0.1.tar.gz` & `tmp/mpu6050-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpu6050-0.0.1.tar", last modified: Tue Apr 23 15:38:40 2024, max compression
+gzip compressed data, was "mpu6050-0.0.2.tar", last modified: Wed Apr 24 21:21:45 2024, max compression
```

## Comparing `mpu6050-0.0.1.tar` & `mpu6050-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 15:38:40.978474 mpu6050-0.0.1/
--rw-rw-rw-   0        0        0     1082 2024-03-27 20:06:00.000000 mpu6050-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2004 2024-04-23 15:38:40.976478 mpu6050-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1315 2024-04-23 08:06:54.000000 mpu6050-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 15:38:40.937582 mpu6050-0.0.1/mpu6050/
--rw-rw-rw-   0        0        0    40489 2024-04-16 22:19:38.000000 mpu6050-0.0.1/mpu6050/MPU6050.py
--rw-rw-rw-   0        0        0    32538 2024-04-16 21:53:09.000000 mpu6050-0.0.1/mpu6050/MPUConstants.py
--rw-rw-rw-   0        0        0       51 2024-04-23 08:00:05.000000 mpu6050-0.0.1/mpu6050/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 15:38:40.975480 mpu6050-0.0.1/mpu6050.egg-info/
--rw-rw-rw-   0        0        0     2004 2024-04-23 15:38:40.000000 mpu6050-0.0.1/mpu6050.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2024-04-23 15:38:40.000000 mpu6050-0.0.1/mpu6050.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 15:38:40.000000 mpu6050-0.0.1/mpu6050.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-23 15:38:40.000000 mpu6050-0.0.1/mpu6050.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-23 15:38:40.000000 mpu6050-0.0.1/mpu6050.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 15:38:40.978474 mpu6050-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1283 2024-04-23 15:35:57.000000 mpu6050-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 21:21:45.051225 mpu6050-0.0.2/
+-rw-rw-rw-   0        0        0     1082 2024-03-27 20:06:00.000000 mpu6050-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     4582 2024-04-24 21:21:45.051225 mpu6050-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3839 2024-04-23 20:19:47.000000 mpu6050-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 21:21:45.019982 mpu6050-0.0.2/mpu6050/
+-rw-rw-rw-   0        0        0    40489 2024-04-23 21:19:16.000000 mpu6050-0.0.2/mpu6050/MPU6050.py
+-rw-rw-rw-   0        0        0    32538 2024-04-16 21:53:09.000000 mpu6050-0.0.2/mpu6050/MPUConstants.py
+-rw-rw-rw-   0        0        0       22 2024-04-24 21:18:09.000000 mpu6050-0.0.2/mpu6050/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 21:21:45.051225 mpu6050-0.0.2/mpu6050.egg-info/
+-rw-rw-rw-   0        0        0     4582 2024-04-24 21:21:44.000000 mpu6050-0.0.2/mpu6050.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2024-04-24 21:21:44.000000 mpu6050-0.0.2/mpu6050.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 21:21:44.000000 mpu6050-0.0.2/mpu6050.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-24 21:21:44.000000 mpu6050-0.0.2/mpu6050.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-24 21:21:44.000000 mpu6050-0.0.2/mpu6050.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 21:21:45.051225 mpu6050-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1299 2024-04-24 21:21:41.000000 mpu6050-0.0.2/setup.py
```

### Comparing `mpu6050-0.0.1/LICENSE.txt` & `mpu6050-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mpu6050-0.0.1/mpu6050/MPU6050.py` & `mpu6050-0.0.2/mpu6050/MPU6050.py`

 * *Files identical despite different names*

### Comparing `mpu6050-0.0.1/mpu6050/MPUConstants.py` & `mpu6050-0.0.2/mpu6050/MPUConstants.py`

 * *Files identical despite different names*

### Comparing `mpu6050-0.0.1/setup.py` & `mpu6050-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'A Python Library for Efficient MPU6050 DMP Access.'
 LONG_DESCRIPTION = 'This library aims to simplify the use of digital motion processor (DMP) inside inertial motion unit (IMU), along with other motion data.'
 
 # Setting up
 setup(
     name="mpu6050",
     version=VERSION,
     author="Majid Alekasir",
     author_email="<majid.alekasir@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
+    url='https://github.com/OmidAlek/mpu6050',
     packages=find_packages(),
-    install_requires=['quat'],
+    install_requires=['quat', 'smbus'],
     keywords=['python', 'quaternion', 'vector', 'XYZVector', 'IMU', 'DMP', 'INS', 'Accelometer', 'Gyrometer', 'MPU6050', 'Fusion', 'EKF', 'Kalman Filter'],
     classifiers=[
-        "Development Status :: 1 - Planning",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.10",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Microsoft :: Windows",
     ]
 )
```

