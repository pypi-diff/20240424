# Comparing `tmp/PetsisDevUtils-0.1.tar.gz` & `tmp/PetsisDevUtils-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PetsisDevUtils-0.1.tar", last modified: Wed Apr 24 04:18:57 2024, max compression
+gzip compressed data, was "PetsisDevUtils-0.2.tar", last modified: Wed Apr 24 04:23:29 2024, max compression
```

## Comparing `PetsisDevUtils-0.1.tar` & `PetsisDevUtils-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 04:18:57.405907 PetsisDevUtils-0.1/
--rw-rw-rw-   0        0        0      619 2024-04-24 04:18:57.390282 PetsisDevUtils-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-24 04:18:57.390282 PetsisDevUtils-0.1/PetsisDevUtils.egg-info/
--rw-rw-rw-   0        0        0      619 2024-04-24 04:18:57.000000 PetsisDevUtils-0.1/PetsisDevUtils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-04-24 04:18:57.000000 PetsisDevUtils-0.1/PetsisDevUtils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 04:18:57.000000 PetsisDevUtils-0.1/PetsisDevUtils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-24 04:18:57.000000 PetsisDevUtils-0.1/PetsisDevUtils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-04-24 03:31:53.000000 PetsisDevUtils-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 04:18:57.390282 PetsisDevUtils-0.1/package/
--rw-rw-rw-   0        0        0       20 2024-04-24 04:18:13.000000 PetsisDevUtils-0.1/package/__init__.py
--rw-rw-rw-   0        0        0       63 2024-04-24 04:18:13.000000 PetsisDevUtils-0.1/package/funcs.py
--rw-rw-rw-   0        0        0       48 2024-04-24 03:34:20.000000 PetsisDevUtils-0.1/package/module1.py
--rw-rw-rw-   0        0        0       34 2024-04-24 03:34:49.000000 PetsisDevUtils-0.1/package/module2.py
--rw-rw-rw-   0        0        0       42 2024-04-24 04:18:57.405907 PetsisDevUtils-0.1/setup.cfg
--rw-rw-rw-   0        0        0      793 2024-04-24 04:18:13.000000 PetsisDevUtils-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 04:23:28.998078 PetsisDevUtils-0.2/
+-rw-rw-rw-   0        0        0      619 2024-04-24 04:23:28.998078 PetsisDevUtils-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-24 04:23:28.993075 PetsisDevUtils-0.2/PetsisDevUtils.egg-info/
+-rw-rw-rw-   0        0        0      619 2024-04-24 04:23:28.000000 PetsisDevUtils-0.2/PetsisDevUtils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-04-24 04:23:28.000000 PetsisDevUtils-0.2/PetsisDevUtils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 04:23:28.000000 PetsisDevUtils-0.2/PetsisDevUtils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-24 04:23:28.000000 PetsisDevUtils-0.2/PetsisDevUtils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-04-24 03:31:53.000000 PetsisDevUtils-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 04:23:28.996081 PetsisDevUtils-0.2/package/
+-rw-rw-rw-   0        0        0       20 2024-04-24 04:18:13.000000 PetsisDevUtils-0.2/package/__init__.py
+-rw-rw-rw-   0        0        0       78 2024-04-24 04:20:48.000000 PetsisDevUtils-0.2/package/funcs.py
+-rw-rw-rw-   0        0        0       48 2024-04-24 03:34:20.000000 PetsisDevUtils-0.2/package/module1.py
+-rw-rw-rw-   0        0        0       34 2024-04-24 03:34:49.000000 PetsisDevUtils-0.2/package/module2.py
+-rw-rw-rw-   0        0        0       42 2024-04-24 04:23:28.998078 PetsisDevUtils-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      793 2024-04-24 04:21:22.000000 PetsisDevUtils-0.2/setup.py
```

### Comparing `PetsisDevUtils-0.1/PKG-INFO` & `PetsisDevUtils-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PetsisDevUtils
-Version: 0.1
+Version: 0.2
 Summary: A short description of your package
 Author: PetsisDev
 Author-email: petsis_dev@proton.me
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PetsisDevUtils-0.1/PetsisDevUtils.egg-info/PKG-INFO` & `PetsisDevUtils-0.2/PetsisDevUtils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PetsisDevUtils
-Version: 0.1
+Version: 0.2
 Summary: A short description of your package
 Author: PetsisDev
 Author-email: petsis_dev@proton.me
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PetsisDevUtils-0.1/setup.py` & `PetsisDevUtils-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PetsisDevUtils',
-    version='0.1',
+    version='0.2',
     description='A short description of your package',
     long_description='A longer description of your package',
     author='PetsisDev', 
     author_email='petsis_dev@proton.me',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

