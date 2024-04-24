# Comparing `tmp/amuse-hermite-2023.5.0.tar.gz` & `tmp/amuse-hermite-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amuse-hermite-2023.5.0.tar", last modified: Wed May 17 10:18:54 2023, max compression
+gzip compressed data, was "amuse-hermite-2024.4.0.tar", last modified: Wed Apr 24 16:32:22 2024, max compression
```

## Comparing `amuse-hermite-2023.5.0.tar` & `amuse-hermite-2024.4.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:54.281865 amuse-hermite-2023.5.0/
--rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-hermite-2023.5.0/MANIFEST.in
--rw-r--r--   0 rieder     (501) staff       (20)     1189 2023-05-17 10:18:54.281706 amuse-hermite-2023.5.0/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)       60 2022-11-22 11:55:14.000000 amuse-hermite-2023.5.0/README.md
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:54.278135 amuse-hermite-2023.5.0/amuse_hermite.egg-info/
--rw-r--r--   0 rieder     (501) staff       (20)     1189 2023-05-17 10:18:52.000000 amuse-hermite-2023.5.0/amuse_hermite.egg-info/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)      768 2023-05-17 10:18:54.000000 amuse-hermite-2023.5.0/amuse_hermite.egg-info/SOURCES.txt
--rw-r--r--   0 rieder     (501) staff       (20)        1 2023-05-17 10:18:52.000000 amuse-hermite-2023.5.0/amuse_hermite.egg-info/dependency_links.txt
--rw-r--r--   0 rieder     (501) staff       (20)       16 2023-05-17 10:18:52.000000 amuse-hermite-2023.5.0/amuse_hermite.egg-info/requires.txt
--rw-r--r--   0 rieder     (501) staff       (20)        6 2023-05-17 10:18:52.000000 amuse-hermite-2023.5.0/amuse_hermite.egg-info/top_level.txt
--rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:28.000000 amuse-hermite-2023.5.0/pyproject.toml
--rw-r--r--   0 rieder     (501) staff       (20)       38 2023-05-17 10:18:54.281908 amuse-hermite-2023.5.0/setup.cfg
--rw-r--r--   0 rieder     (501) staff       (20)     1884 2022-11-22 11:55:14.000000 amuse-hermite-2023.5.0/setup.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:54.276524 amuse-hermite-2023.5.0/src/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:54.276576 amuse-hermite-2023.5.0/src/amuse/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:54.276698 amuse-hermite-2023.5.0/src/amuse/community/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:54.279955 amuse-hermite-2023.5.0/src/amuse/community/hermite/
--rw-r--r--   0 rieder     (501) staff       (20)     1428 2023-03-14 13:48:49.000000 amuse-hermite-2023.5.0/src/amuse/community/hermite/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)       31 2022-11-22 11:55:15.000000 amuse-hermite-2023.5.0/src/amuse/community/hermite/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)    48897 2022-11-22 11:55:15.000000 amuse-hermite-2023.5.0/src/amuse/community/hermite/interface.cc
--rw-r--r--   0 rieder     (501) staff       (20)        1 2022-11-22 11:55:15.000000 amuse-hermite-2023.5.0/src/amuse/community/hermite/interface.h
--rw-r--r--   0 rieder     (501) staff       (20)    11097 2023-03-14 13:48:49.000000 amuse-hermite-2023.5.0/src/amuse/community/hermite/interface.py
--rw-r--r--   0 rieder     (501) staff       (20)     6056 2022-11-22 11:55:15.000000 amuse-hermite-2023.5.0/src/amuse/community/hermite/vec3.h
--rw-r--r--   0 rieder     (501) staff       (20)      148 2023-05-17 10:18:52.000000 amuse-hermite-2023.5.0/src/amuse/community/hermite/version.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:54.280199 amuse-hermite-2023.5.0/src/amuse/community/hermite0/
--rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-hermite-2023.5.0/src/amuse/community/hermite0/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)      345 2022-11-22 11:55:15.000000 amuse-hermite-2023.5.0/src/amuse/community/hermite0/interface.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:54.281471 amuse-hermite-2023.5.0/support/
--rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-hermite-2023.5.0/support/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-hermite-2023.5.0/support/classifiers.py
--rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-hermite-2023.5.0/support/config.py
--rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-hermite-2023.5.0/support/generate_main.py
--rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-hermite-2023.5.0/support/getsp.class
--rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-hermite-2023.5.0/support/getsp.java
--rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-hermite-2023.5.0/support/misc.py
--rw-r--r--   0 rieder     (501) staff       (20)    49373 2023-05-17 08:15:41.000000 amuse-hermite-2023.5.0/support/setup_codes.py
--rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-hermite-2023.5.0/support/version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:22.666929 amuse-hermite-2024.4.0/
+-rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-hermite-2024.4.0/MANIFEST.in
+-rw-r--r--   0 rieder     (501) staff       (20)     1220 2024-04-24 16:32:22.666739 amuse-hermite-2024.4.0/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)       60 2022-11-22 11:55:14.000000 amuse-hermite-2024.4.0/README.md
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:22.666486 amuse-hermite-2024.4.0/amuse_hermite.egg-info/
+-rw-r--r--   0 rieder     (501) staff       (20)     1220 2024-04-24 16:32:21.000000 amuse-hermite-2024.4.0/amuse_hermite.egg-info/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)      769 2024-04-24 16:32:22.000000 amuse-hermite-2024.4.0/amuse_hermite.egg-info/SOURCES.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        1 2024-04-24 16:32:21.000000 amuse-hermite-2024.4.0/amuse_hermite.egg-info/dependency_links.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       16 2024-04-24 16:32:21.000000 amuse-hermite-2024.4.0/amuse_hermite.egg-info/requires.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        6 2024-04-24 16:32:21.000000 amuse-hermite-2024.4.0/amuse_hermite.egg-info/top_level.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       93 2024-04-24 16:29:24.000000 amuse-hermite-2024.4.0/pyproject.toml
+-rw-r--r--   0 rieder     (501) staff       (20)       38 2024-04-24 16:32:22.666983 amuse-hermite-2024.4.0/setup.cfg
+-rw-r--r--   0 rieder     (501) staff       (20)     1687 2024-04-24 15:35:29.000000 amuse-hermite-2024.4.0/setup.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:22.662301 amuse-hermite-2024.4.0/src/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:22.662353 amuse-hermite-2024.4.0/src/amuse/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:22.662468 amuse-hermite-2024.4.0/src/amuse/community/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:22.664789 amuse-hermite-2024.4.0/src/amuse/community/hermite/
+-rw-r--r--   0 rieder     (501) staff       (20)     1428 2023-03-14 13:48:49.000000 amuse-hermite-2024.4.0/src/amuse/community/hermite/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)       31 2022-11-22 11:55:15.000000 amuse-hermite-2024.4.0/src/amuse/community/hermite/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      417 2024-04-24 16:32:21.000000 amuse-hermite-2024.4.0/src/amuse/community/hermite/_version.py
+-rw-r--r--   0 rieder     (501) staff       (20)    48589 2024-04-24 15:35:29.000000 amuse-hermite-2024.4.0/src/amuse/community/hermite/interface.cc
+-rw-r--r--   0 rieder     (501) staff       (20)        1 2022-11-22 11:55:15.000000 amuse-hermite-2024.4.0/src/amuse/community/hermite/interface.h
+-rw-r--r--   0 rieder     (501) staff       (20)    11097 2024-04-24 15:35:29.000000 amuse-hermite-2024.4.0/src/amuse/community/hermite/interface.py
+-rw-r--r--   0 rieder     (501) staff       (20)     6056 2022-11-22 11:55:15.000000 amuse-hermite-2024.4.0/src/amuse/community/hermite/vec3.h
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:22.665069 amuse-hermite-2024.4.0/src/amuse/community/hermite0/
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-hermite-2024.4.0/src/amuse/community/hermite0/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      345 2022-11-22 11:55:15.000000 amuse-hermite-2024.4.0/src/amuse/community/hermite0/interface.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:22.666305 amuse-hermite-2024.4.0/support/
+-rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-hermite-2024.4.0/support/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-hermite-2024.4.0/support/classifiers.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-hermite-2024.4.0/support/config.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-hermite-2024.4.0/support/generate_main.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-hermite-2024.4.0/support/getsp.class
+-rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-hermite-2024.4.0/support/getsp.java
+-rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-hermite-2024.4.0/support/misc.py
+-rw-r--r--   0 rieder     (501) staff       (20)    49244 2023-05-26 13:47:38.000000 amuse-hermite-2024.4.0/support/setup_codes.py
+-rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-hermite-2024.4.0/support/version.py
```

### Comparing `amuse-hermite-2023.5.0/PKG-INFO` & `amuse-hermite-2024.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-hermite
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - Hermite
 Home-page: http://www.amusecode.org/
 Author: The AMUSE team
 Author-email: info@amusecode.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -19,11 +19,12 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Fortran
 Classifier: Topic :: Scientific/Engineering :: Astronomy
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: amuse-framework
 
 This package installs the Hermite community code for AMUSE.
```

### Comparing `amuse-hermite-2023.5.0/amuse_hermite.egg-info/PKG-INFO` & `amuse-hermite-2024.4.0/amuse_hermite.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-hermite
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - Hermite
 Home-page: http://www.amusecode.org/
 Author: The AMUSE team
 Author-email: info@amusecode.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -19,11 +19,12 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Fortran
 Classifier: Topic :: Scientific/Engineering :: Astronomy
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: amuse-framework
 
 This package installs the Hermite community code for AMUSE.
```

### Comparing `amuse-hermite-2023.5.0/amuse_hermite.egg-info/SOURCES.txt` & `amuse-hermite-2024.4.0/amuse_hermite.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 amuse_hermite.egg-info/PKG-INFO
 amuse_hermite.egg-info/SOURCES.txt
 amuse_hermite.egg-info/dependency_links.txt
 amuse_hermite.egg-info/requires.txt
 amuse_hermite.egg-info/top_level.txt
 src/amuse/community/hermite/Makefile
 src/amuse/community/hermite/__init__.py
+src/amuse/community/hermite/_version.py
 src/amuse/community/hermite/interface.cc
 src/amuse/community/hermite/interface.h
 src/amuse/community/hermite/interface.py
 src/amuse/community/hermite/vec3.h
-src/amuse/community/hermite/version.py
 src/amuse/community/hermite0/__init__.py
 src/amuse/community/hermite0/interface.py
 support/__init__.py
 support/classifiers.py
 support/config.py
 support/generate_main.py
 support/getsp.class
```

### Comparing `amuse-hermite-2023.5.0/setup.py` & `amuse-hermite-2024.4.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -30,42 +30,35 @@
 ]
 
 package_data = {
 }
 
 mapping_from_command_name_to_command_class = setup_commands()
 
-try:
-    from src.amuse.community.hermite.version import version
-    use_scm_version = False
-    setup_requires = []
-except ImportError:
-    version = False
-    setup_requires = ['setuptools_scm']
-    use_scm_version = {
-        "root": "../..",
-        "relative_to": __file__,
-        "write_to": "src/amuse/community/hermite/version.py",
-    }
+setup_requires = ['setuptools_scm']
+use_scm_version = {
+    "root": "../..",
+    "relative_to": __file__,
+    "version_file": "src/amuse/community/hermite/_version.py",
+}
 
 setup(
     name=name,
     use_scm_version=use_scm_version,
     setup_requires=setup_requires,
-    version=version,
     classifiers=classifiers,
     url=url,
     author_email=author_email,
     author=author,
     license=license_,
     description=description,
     long_description=long_description,
     long_description_content_type=long_description_content_type,
     install_requires=install_requires,
-    python_requires=">=3.5",
+    python_requires=">=3.7",
     cmdclass=mapping_from_command_name_to_command_class,
     ext_modules=extensions,
     package_dir={
         'amuse.community.hermite': 'src/amuse/community/hermite',
         'amuse.community.hermite0': 'src/amuse/community/hermite0',
     },
     packages=packages,
```

### Comparing `amuse-hermite-2023.5.0/src/amuse/community/hermite/Makefile` & `amuse-hermite-2024.4.0/src/amuse/community/hermite/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-hermite-2023.5.0/src/amuse/community/hermite/interface.cc` & `amuse-hermite-2024.4.0/src/amuse/community/hermite/interface.cc`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 static real  t = 0;
 static real t_evolve = t;                // Time requested by evolve.  Control returns
                                 // when t <= t_evolve and t + dt > t_evolve,
                                 // and this is assumed when the state of the
                                 // system is computed by extrapolation.
 static real t_wanted = 0;
 static double begin_time = 0;
-static double end_time_accuracy_factor = 0.5;
+static double end_time_accuracy_factor = 0.0;
 
 static vector<int>  ident;
 static vector<real> mass, radius, potential;
 static vector<vec>  pos, vel, acc, jerk;
 static vector<vec>  acc_reduced, jerk_reduced;
 static vector<real> potential_reduced;
 
@@ -1283,32 +1283,14 @@
     }
   else
     {
       return -2;
     }
 }
 
-int set_acceleration(int id, double ax, double ay, double az)
-{
-  unsigned int i = find(ident.begin(), ident.end(), id) - ident.begin();
-  if (i < ident.size())
-    {
-      acc[i][0] = ax;
-      acc[i][1] = ay;
-      acc[i][2] = az;
-      return 0;
-    }
-  else
-    {
-      return -2;
-    }
-
-  return -3;
-}
-
 int evolve_not_on_root() {
 
 #ifndef NOMPI
     int must_run = 1;
     int mpi_error = MPI_Bcast(&must_run, 1, MPI_INTEGER, 0, WORLD);
     if(mpi_error) {
         return -1;
```

### Comparing `amuse-hermite-2023.5.0/src/amuse/community/hermite/interface.py` & `amuse-hermite-2024.4.0/src/amuse/community/hermite/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,15 @@
             Get the end time accuracy factor:
                 < 0.0  will stop on or before the end time (larger factor, more before)
                   0.0  will stop at exactly the end time
                 > 0.0  will stop on or after the end time
                 
             Valid factors are between -1.0 and 1.0
             """,
-            default_value = 1.0
+            default_value = 0.0
         )
         handler.add_method_parameter(
             "get_dt_dia",
             "set_dt_dia",
             "dt_dia", 
             "time interval between diagnostics output", 
             default_value = 1.0 | nbody_system.time
```

### Comparing `amuse-hermite-2023.5.0/src/amuse/community/hermite/vec3.h` & `amuse-hermite-2024.4.0/src/amuse/community/hermite/vec3.h`

 * *Files identical despite different names*

### Comparing `amuse-hermite-2023.5.0/support/__init__.py` & `amuse-hermite-2024.4.0/support/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-hermite-2023.5.0/support/classifiers.py` & `amuse-hermite-2024.4.0/support/classifiers.py`

 * *Files identical despite different names*

### Comparing `amuse-hermite-2023.5.0/support/config.py` & `amuse-hermite-2024.4.0/support/config.py`

 * *Files identical despite different names*

### Comparing `amuse-hermite-2023.5.0/support/generate_main.py` & `amuse-hermite-2024.4.0/support/generate_main.py`

 * *Files identical despite different names*

### Comparing `amuse-hermite-2023.5.0/support/getsp.class` & `amuse-hermite-2024.4.0/support/getsp.class`

 * *Files identical despite different names*

### Comparing `amuse-hermite-2023.5.0/support/getsp.java` & `amuse-hermite-2024.4.0/support/getsp.java`

 * *Files identical despite different names*

### Comparing `amuse-hermite-2023.5.0/support/misc.py` & `amuse-hermite-2024.4.0/support/misc.py`

 * *Files identical despite different names*

### Comparing `amuse-hermite-2023.5.0/support/setup_codes.py` & `amuse-hermite-2024.4.0/support/setup_codes.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 import configparser
 
 from subprocess import Popen, PIPE, STDOUT
 
 from glob import glob
 
 from distutils.dir_util import create_tree
-# from distutils import log
-import logging
+from distutils import log
 from distutils import spawn
 from distutils import file_util
 from distutils.errors import DistutilsError
 from distutils.command.clean import clean
 from setuptools.command.install import install
 from setuptools import Command
 from setuptools.command.build import build
@@ -556,37 +555,37 @@
         if not os.path.exists(lib_binbuilddir):
             self.mkpath(lib_binbuilddir)
 
         for srcdir in self.makefile_paths(self.codes_src_dir):
             reldir = os.path.relpath(srcdir, self.codes_src_dir)
             temp_builddir = os.path.join(self.codes_dir, reldir)
 
-            self.announce("will copy worker: {0}".format(srcdir), level=logging.INFO)
+            self.announce("will copy worker: {0}".format(srcdir), level=log.INFO)
             lib_builddir = os.path.join(self.build_lib, os.path.relpath(srcdir, os.path.join(self.amuse_src_dir, '..')))
 
             shortname = reldir.lower()
-            self.announce(shortname, level=logging.INFO)
+            self.announce(shortname, level=log.INFO)
 
             for name in os.listdir(temp_builddir):
                 path = os.path.join(temp_builddir, name)
                 stat = os.stat(path)
 
                 if os.path.isfile(path):
                     if worker_so_re.match(name):
                         topath = os.path.join(lib_builddir, name)
                         self.copy_file(path, topath)
                         continue
 
-                # self.announce("will copy worker: {0}".format(name), level = logging.INFO)
+                # self.announce("will copy worker: {0}".format(name), level = log.INFO)
                 if os.path.isfile(path) and os.access(path, os.X_OK):
                     if worker_code_re.match(name):
                         topath = os.path.join(lib_binbuilddir, name)
                         self.copy_file(path, topath)
                     elif not name.endswith('.py'):
-                        self.announce("will not copy executable: {0}, it does not match the worker pattern".format(name), level=logging.WARN)
+                        self.announce("will not copy executable: {0}, it does not match the worker pattern".format(name), level=log.WARN)
             
             # also copy file or dir named data
             path = os.path.join(temp_builddir, 'data')
             topath = os.path.join(lib_builddir, 'data')
             if os.path.isfile(path):
                 self.copy_file(path, topath)
             if os.path.isdir(path):
@@ -599,19 +598,19 @@
             worker_code_re = re.compile(r'(([a-zA-Z0-9]+_)*)?worker(_[a-zA-Z0-9]+)?')
         worker_so_re = re.compile(r'(([a-zA-Z0-9]+_)*)?cython(_[a-zA-Z0-9]+)?.so')
 
         for srcdir in self.makefile_paths(self.codes_src_dir):
             reldir = os.path.relpath(srcdir, self.codes_src_dir)
             temp_builddir = os.path.join(self.codes_dir, reldir)
 
-            self.announce("will copy worker: {0}".format(srcdir), level=logging.INFO)
+            self.announce("will copy worker: {0}".format(srcdir), level=log.INFO)
             lib_builddir = os.path.join(self.build_lib, os.path.relpath(srcdir, os.path.join(self.amuse_src_dir, '..')))
 
             shortname = reldir.lower()
-            self.announce(shortname, level=logging.INFO)
+            self.announce(shortname, level=log.INFO)
 
             for name in os.listdir(temp_builddir):
                 path = os.path.join(temp_builddir, name)
                 stat = os.stat(path)
 
                 if os.path.isfile(path):
                     if worker_so_re.match(name):
@@ -620,15 +619,15 @@
                         continue
 
                 if os.path.isfile(path) and os.access(path, os.X_OK):
                     if worker_code_re.match(name):
                         topath = os.path.join(lib_builddir, name)
                         self.copy_file(path, topath)
                     elif not name.endswith('.py'):
-                        self.announce("will not copy executable: {0}, it does not match the worker pattern".format(name), level=logging.WARN)
+                        self.announce("will not copy executable: {0}, it does not match the worker pattern".format(name), level=log.WARN)
             
             # also copy file or dir named data
             path = os.path.join(temp_builddir, 'data')
             topath = os.path.join(lib_builddir, 'data')
             if os.path.isfile(path):
                 self.copy_file(path, topath)
             if os.path.isdir(path):
@@ -712,15 +711,15 @@
         result = list(set(result))
 
         return result
 
     def call(self, arguments, buildlogfile=None, **keyword_arguments):
         stringio = []
 
-        self.announce(' '.join(arguments), logging.DEBUG)
+        self.announce(' '.join(arguments), log.DEBUG)
 
         process = Popen(
             arguments,
             stdout=PIPE,
             stderr=STDOUT,
             **keyword_arguments
         )
@@ -728,24 +727,24 @@
         while True:
             line = process.stdout.readline()
             if len(line) == 0:
                 break
 
             if buildlogfile is not None:
                 buildlogfile.write(line)
-            self.announce(line[:-1].decode("utf-8"), logging.DEBUG)
+            self.announce(line[:-1].decode("utf-8"), log.DEBUG)
             stringio.append(str(line, 'utf-8'))
 
         result = process.wait()
         content = ''.join(stringio)
 
         if result != 0:
-            self.announce("error in call, tail output:\n", logging.INFO)
-            self.announce(''.join(stringio[-100:]), logging.INFO)
-            self.announce("-"*80, logging.INFO)
+            self.announce("error in call, tail output:\n", log.INFO)
+            self.announce(''.join(stringio[-100:]), log.INFO)
+            self.announce("-"*80, log.INFO)
 
         return result, content
 
     def build_environment(self):
         environment = self.environment.copy()
         environment.update(os.environ)
         path = os.path.join(environment["MUSE_PACKAGE_DIR"], "src")
@@ -880,16 +879,16 @@
         build = list()
         lib_build = list()
         lib_not_build = list()
         environment = self.build_environment()
 
         buildlog = 'build.log'
 
-        self.announce("building libraries and community codes", level=logging.INFO)
-        self.announce("build, for logging, see '{0}'".format(buildlog), level=logging.INFO)
+        self.announce("building libraries and community codes", level=log.INFO)
+        self.announce("build, for logging, see '{0}'".format(buildlog), level=log.INFO)
 
         with open(buildlog, "w") as output:
             output.write('*'*100)
             output.write('\n')
             output.write('Building libraries and codes\n')
             output.write('*'*100)
             output.write('\n')
@@ -898,28 +897,28 @@
             self.copy_build_prereq_to_build_dir()
             self.copy_lib_to_build_dir()
 
         for x in self.makefile_paths(self.lib_dir):
 
             shortname = x[len(self.lib_dir) + 1:] + '-library'
             starttime = datetime.datetime.now()
-            self.announce("[{1:%H:%M:%S}] building {0}".format(shortname, starttime), level=logging.INFO)
+            self.announce("[{1:%H:%M:%S}] building {0}".format(shortname, starttime), level=log.INFO)
             returncode, outputlog = self.run_make_on_directory(shortname, x, 'all', environment)
 
             endtime = datetime.datetime.now()
             if returncode == 2:
-                self.announce("[{2:%H:%M:%S}] building {0}, failed, see {1!r} for error log".format(shortname, buildlog, endtime), level=logging.DEBUG)
+                self.announce("[{2:%H:%M:%S}] building {0}, failed, see {1!r} for error log".format(shortname, buildlog, endtime), level=log.DEBUG)
                 if self.is_download_needed(outputlog):
                     is_download_needed.append(x[len(self.lib_dir) + 1:])
                 elif self.is_cuda_needed(outputlog):
                     is_cuda_needed.append(x[len(self.lib_dir) + 1:])
                 else:
                     lib_not_build.append(shortname)
             else:
-                self.announce("[{1:%H:%M:%S}] building {0}, succeeded".format(shortname, endtime), level=logging.DEBUG)
+                self.announce("[{1:%H:%M:%S}] building {0}, succeeded".format(shortname, endtime), level=log.DEBUG)
                 lib_build.append(shortname)
 
         if not self.codes_dir == self.codes_src_dir:
             self.copy_codes_to_build_dir()
 
         # environment.update(self.environment)
         makefile_paths = list(self.makefile_paths(self.codes_dir))
@@ -933,24 +932,24 @@
             # to distribute mesa, it will make the
             # download size from about 100mb size
             # to > 1Gb size.
             #
             # Could we remove some of the data files from mesa?
             #
             if not self.inplace and shortname == 'mesa':
-                self.announce("[{1:%H:%M:%S}] skipping {0}".format(shortname, starttime), level=logging.INFO)
+                self.announce("[{1:%H:%M:%S}] skipping {0}".format(shortname, starttime), level=log.INFO)
                 continue
 
-            self.announce("[{1:%H:%M:%S}] building {0}".format(shortname, starttime), level=logging.INFO)
+            self.announce("[{1:%H:%M:%S}] building {0}".format(shortname, starttime), level=log.INFO)
             returncode, outputlog = self.run_make_on_directory(shortname, x, 'all', environment)
             endtime = datetime.datetime.now()
             if returncode > 0:
                 self.announce(
                     "[{2:%H:%M:%S}] building {0}, failed, see {1!r} for error log".format(shortname, buildlog, endtime),
-                    level=logging.DEBUG
+                    level=log.DEBUG
                 )
                 if self.is_download_needed(outputlog):
                     is_download_needed.append(shortname)
                 elif self.is_cuda_needed(outputlog):
                     is_cuda_needed.append(shortname)
                 elif self.are_python_imports_needed(outputlog):
                     are_python_imports_needed.append(shortname)
@@ -960,40 +959,40 @@
                 if self.is_mpi_enabled():
                     continue
             else:
                 build.append(shortname)
                 is_built = True
                 self.announce(
                     "[{1:%H:%M:%S}] building {0}, succeeded".format(shortname, endtime),
-                    level=logging.DEBUG
+                    level=log.DEBUG
                 )
 
             if not self.variant:
                 continue
 
             special_targets = self.get_special_targets(shortname, x, environment)
             for target, target_name in special_targets:
                 starttime = datetime.datetime.now()
                 self.announce(
                     "[{2:%H:%M:%S}] building {0} - {1}".format(shortname, target_name, starttime),
-                    level=logging.DEBUG
+                    level=log.DEBUG
                 )
                 returncode, outputlog = self.run_make_on_directory(shortname, x, target, environment)
                 endtime = datetime.datetime.now()
                 if returncode > 0:
                     specials_list = not_build_special.setdefault(shortname,[])
                     specials_list.append(target_name)
                     self.announce(
                         "[{3:%H:%M:%S}] building {0} - {1}, failed, see {2!r} for error log".format(shortname, target_name, buildlog, endtime),
-                        level=logging.DEBUG
+                        level=log.DEBUG
                     )
                 else:
                     build_to_special_targets.setdefault(shortname, list()).append(target_name)
                     self.announce(
-                        "[{2:%H:%M:%S}] building {0} - {1}, succeeded".format(shortname, target_name, endtime), level=logging.DEBUG
+                        "[{2:%H:%M:%S}] building {0} - {1}, succeeded".format(shortname, target_name, endtime), level=log.DEBUG
                     )
 
         # if supportrc["framework_install"]:
         #     self.copy_config_to_build_dir()
 
         if not self.codes_dir == self.codes_src_dir:
             # self.copy_worker_codes_to_build_dir()
@@ -1028,17 +1027,17 @@
             not_build
             or not_build_special
             or is_download_needed
             or is_cuda_needed
             or are_python_imports_needed
         ):
             if not_build:
-                level = logging.WARN
+                level = log.WARN
             else:
-                level = logging.INFO
+                level = log.INFO
             if not_build:
                 self.announce(
                     "Community codes not built (because of errors/ missing libraries):",
                     level=level
                 )
                 self.announce("="*80,  level=level)
                 for x in not_build:
@@ -1061,26 +1060,26 @@
                     self.announce(
                         f' * {x} , make {x}.code DOWNLOAD_CODES=1', level=level
                     )
 
             self.announce("="*80,  level=level)
 
         if build:
-            level = logging.INFO
+            level = log.INFO
             self.announce("Community codes built",  level=level)
             self.announce("="*80,  level=level)
             for x in build:
                 if x in build_to_special_targets:
                     y = build_to_special_targets[x]
                     self.announce('* {0} ({1})'.format(x, ','.join(y)), level=level)
                 else:
                     self.announce('* {0}'.format(x),  level=level)
             self.announce("="*80,  level=level)
 
-        level = logging.INFO
+        level = log.INFO
         self.announce(
             "{0} out of {1} codes built, {2} out of {3} libraries built".format(
                 len(build), 
                 len(build) + len(not_build), 
                 len(lib_build), 
                 len(lib_build) + len(lib_not_build)
             ),
```

