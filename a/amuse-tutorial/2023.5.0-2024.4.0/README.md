# Comparing `tmp/amuse-tutorial-2023.5.0.tar.gz` & `tmp/amuse-tutorial-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amuse-tutorial-2023.5.0.tar", last modified: Wed May 17 10:19:55 2023, max compression
+gzip compressed data, was "amuse-tutorial-2024.4.0.tar", last modified: Wed Apr 24 16:33:02 2024, max compression
```

## Comparing `amuse-tutorial-2023.5.0.tar` & `amuse-tutorial-2024.4.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:55.001588 amuse-tutorial-2023.5.0/
--rw-r--r--   0 rieder     (501) staff       (20)      207 2022-11-22 11:55:14.000000 amuse-tutorial-2023.5.0/MANIFEST.in
--rw-r--r--   0 rieder     (501) staff       (20)     1231 2023-05-17 10:19:55.001437 amuse-tutorial-2023.5.0/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)      100 2022-11-22 11:55:14.000000 amuse-tutorial-2023.5.0/README.md
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:54.995320 amuse-tutorial-2023.5.0/amuse_tutorial.egg-info/
--rw-r--r--   0 rieder     (501) staff       (20)     1231 2023-05-17 10:19:53.000000 amuse-tutorial-2023.5.0/amuse_tutorial.egg-info/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)      959 2023-05-17 10:19:54.000000 amuse-tutorial-2023.5.0/amuse_tutorial.egg-info/SOURCES.txt
--rw-r--r--   0 rieder     (501) staff       (20)        1 2023-05-17 10:19:53.000000 amuse-tutorial-2023.5.0/amuse_tutorial.egg-info/dependency_links.txt
--rw-r--r--   0 rieder     (501) staff       (20)       92 2023-05-17 10:19:53.000000 amuse-tutorial-2023.5.0/amuse_tutorial.egg-info/requires.txt
--rw-r--r--   0 rieder     (501) staff       (20)        1 2023-05-17 10:19:53.000000 amuse-tutorial-2023.5.0/amuse_tutorial.egg-info/top_level.txt
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:54.995608 amuse-tutorial-2023.5.0/bin/
--rwxr-xr-x   0 rieder     (501) staff       (20)      328 2022-11-22 11:55:13.000000 amuse-tutorial-2023.5.0/bin/amuse-tutorial
--rw-r--r--   0 rieder     (501) staff       (20)      728 2022-11-22 11:55:13.000000 amuse-tutorial-2023.5.0/bin/amusifier.in
--rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:29.000000 amuse-tutorial-2023.5.0/pyproject.toml
--rw-r--r--   0 rieder     (501) staff       (20)       38 2023-05-17 10:19:55.001639 amuse-tutorial-2023.5.0/setup.cfg
--rw-r--r--   0 rieder     (501) staff       (20)     1633 2022-11-22 11:55:14.000000 amuse-tutorial-2023.5.0/setup.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:54.996924 amuse-tutorial-2023.5.0/support/
--rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-tutorial-2023.5.0/support/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-tutorial-2023.5.0/support/classifiers.py
--rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-tutorial-2023.5.0/support/config.py
--rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-tutorial-2023.5.0/support/generate_main.py
--rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-tutorial-2023.5.0/support/getsp.class
--rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-tutorial-2023.5.0/support/getsp.java
--rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-tutorial-2023.5.0/support/misc.py
--rw-r--r--   0 rieder     (501) staff       (20)    49373 2023-05-17 08:15:41.000000 amuse-tutorial-2023.5.0/support/setup_codes.py
--rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-tutorial-2023.5.0/support/version.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:19:55.001201 amuse-tutorial-2023.5.0/tutorial/
--rw-r--r--   0 rieder     (501) staff       (20)     6415 2023-03-14 13:48:48.000000 amuse-tutorial-2023.5.0/tutorial/00-Welcome.ipynb
--rw-r--r--   0 rieder     (501) staff       (20)    13511 2023-03-14 13:48:48.000000 amuse-tutorial-2023.5.0/tutorial/01-Loading_AMUSE.ipynb
--rw-r--r--   0 rieder     (501) staff       (20)     8479 2023-03-14 13:48:48.000000 amuse-tutorial-2023.5.0/tutorial/02-Quantities_with_units.ipynb
--rw-r--r--   0 rieder     (501) staff       (20)     8566 2023-03-14 13:48:48.000000 amuse-tutorial-2023.5.0/tutorial/03-Generic_units.ipynb
--rw-r--r--   0 rieder     (501) staff       (20)     9087 2023-03-14 13:48:48.000000 amuse-tutorial-2023.5.0/tutorial/04-Collections_of_Particles.ipynb
--rw-r--r--   0 rieder     (501) staff       (20)     9580 2023-03-14 13:48:48.000000 amuse-tutorial-2023.5.0/tutorial/05-Attributes_and_functions_on_particle_collections.ipynb
--rw-r--r--   0 rieder     (501) staff       (20)    11166 2023-03-14 13:48:48.000000 amuse-tutorial-2023.5.0/tutorial/06-Using_a_community_code.ipynb
--rw-r--r--   0 rieder     (501) staff       (20)     8150 2023-03-14 13:48:48.000000 amuse-tutorial-2023.5.0/tutorial/07-Channels.ipynb
--rw-r--r--   0 rieder     (501) staff       (20)     5199 2023-03-14 13:48:48.000000 amuse-tutorial-2023.5.0/tutorial/08-Grids.ipynb
--rw-r--r--   0 rieder     (501) staff       (20)     6646 2023-03-14 13:48:48.000000 amuse-tutorial-2023.5.0/tutorial/09-Units_and_functions.ipynb
--rw-r--r--   0 rieder     (501) staff       (20)     8023 2023-03-14 13:48:48.000000 amuse-tutorial-2023.5.0/tutorial/10-Radiative_transfer.ipynb
--rw-r--r--   0 rieder     (501) staff       (20)      977 2022-11-22 11:55:13.000000 amuse-tutorial-2023.5.0/tutorial/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)       34 2022-11-22 11:55:13.000000 amuse-tutorial-2023.5.0/tutorial/amuserc
--rw-r--r--   0 rieder     (501) staff       (20)      449 2022-11-22 11:55:13.000000 amuse-tutorial-2023.5.0/tutorial/create_title.py
--rw-r--r--   0 rieder     (501) staff       (20)     1304 2022-11-22 11:55:13.000000 amuse-tutorial-2023.5.0/tutorial/index.rst
--rw-r--r--   0 rieder     (501) staff       (20)      148 2023-05-17 10:19:53.000000 amuse-tutorial-2023.5.0/tutorial/version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:33:02.593401 amuse-tutorial-2024.4.0/
+-rw-r--r--   0 rieder     (501) staff       (20)      207 2022-11-22 11:55:14.000000 amuse-tutorial-2024.4.0/MANIFEST.in
+-rw-r--r--   0 rieder     (501) staff       (20)     1428 2024-04-24 16:33:02.593171 amuse-tutorial-2024.4.0/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)      100 2022-11-22 11:55:14.000000 amuse-tutorial-2024.4.0/README.md
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:33:02.592814 amuse-tutorial-2024.4.0/amuse_tutorial.egg-info/
+-rw-r--r--   0 rieder     (501) staff       (20)     1428 2024-04-24 16:33:01.000000 amuse-tutorial-2024.4.0/amuse_tutorial.egg-info/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)      960 2024-04-24 16:33:02.000000 amuse-tutorial-2024.4.0/amuse_tutorial.egg-info/SOURCES.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        1 2024-04-24 16:33:01.000000 amuse-tutorial-2024.4.0/amuse_tutorial.egg-info/dependency_links.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       92 2024-04-24 16:33:01.000000 amuse-tutorial-2024.4.0/amuse_tutorial.egg-info/requires.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        1 2024-04-24 16:33:01.000000 amuse-tutorial-2024.4.0/amuse_tutorial.egg-info/top_level.txt
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:33:02.587325 amuse-tutorial-2024.4.0/bin/
+-rwxr-xr-x   0 rieder     (501) staff       (20)      328 2022-11-22 11:55:13.000000 amuse-tutorial-2024.4.0/bin/amuse-tutorial
+-rw-r--r--   0 rieder     (501) staff       (20)      728 2022-11-22 11:55:13.000000 amuse-tutorial-2024.4.0/bin/amusifier.in
+-rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:29.000000 amuse-tutorial-2024.4.0/pyproject.toml
+-rw-r--r--   0 rieder     (501) staff       (20)       38 2024-04-24 16:33:02.593458 amuse-tutorial-2024.4.0/setup.cfg
+-rw-r--r--   0 rieder     (501) staff       (20)     1455 2024-04-24 15:35:29.000000 amuse-tutorial-2024.4.0/setup.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:33:02.589262 amuse-tutorial-2024.4.0/support/
+-rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-tutorial-2024.4.0/support/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-tutorial-2024.4.0/support/classifiers.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-tutorial-2024.4.0/support/config.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-tutorial-2024.4.0/support/generate_main.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-tutorial-2024.4.0/support/getsp.class
+-rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-tutorial-2024.4.0/support/getsp.java
+-rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-tutorial-2024.4.0/support/misc.py
+-rw-r--r--   0 rieder     (501) staff       (20)    49244 2023-05-26 13:47:38.000000 amuse-tutorial-2024.4.0/support/setup_codes.py
+-rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-tutorial-2024.4.0/support/version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:33:02.592587 amuse-tutorial-2024.4.0/tutorial/
+-rw-r--r--   0 rieder     (501) staff       (20)     6415 2023-03-14 13:48:48.000000 amuse-tutorial-2024.4.0/tutorial/00-Welcome.ipynb
+-rw-r--r--   0 rieder     (501) staff       (20)    13511 2023-03-14 13:48:48.000000 amuse-tutorial-2024.4.0/tutorial/01-Loading_AMUSE.ipynb
+-rw-r--r--   0 rieder     (501) staff       (20)     8479 2023-03-14 13:48:48.000000 amuse-tutorial-2024.4.0/tutorial/02-Quantities_with_units.ipynb
+-rw-r--r--   0 rieder     (501) staff       (20)     8566 2023-03-14 13:48:48.000000 amuse-tutorial-2024.4.0/tutorial/03-Generic_units.ipynb
+-rw-r--r--   0 rieder     (501) staff       (20)     9087 2023-03-14 13:48:48.000000 amuse-tutorial-2024.4.0/tutorial/04-Collections_of_Particles.ipynb
+-rw-r--r--   0 rieder     (501) staff       (20)     9580 2023-03-14 13:48:48.000000 amuse-tutorial-2024.4.0/tutorial/05-Attributes_and_functions_on_particle_collections.ipynb
+-rw-r--r--   0 rieder     (501) staff       (20)    11166 2023-03-14 13:48:48.000000 amuse-tutorial-2024.4.0/tutorial/06-Using_a_community_code.ipynb
+-rw-r--r--   0 rieder     (501) staff       (20)     8150 2023-03-14 13:48:48.000000 amuse-tutorial-2024.4.0/tutorial/07-Channels.ipynb
+-rw-r--r--   0 rieder     (501) staff       (20)     5199 2023-03-14 13:48:48.000000 amuse-tutorial-2024.4.0/tutorial/08-Grids.ipynb
+-rw-r--r--   0 rieder     (501) staff       (20)     6646 2023-03-14 13:48:48.000000 amuse-tutorial-2024.4.0/tutorial/09-Units_and_functions.ipynb
+-rw-r--r--   0 rieder     (501) staff       (20)     8023 2023-03-14 13:48:48.000000 amuse-tutorial-2024.4.0/tutorial/10-Radiative_transfer.ipynb
+-rw-r--r--   0 rieder     (501) staff       (20)      977 2022-11-22 11:55:13.000000 amuse-tutorial-2024.4.0/tutorial/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)      417 2024-04-24 16:33:01.000000 amuse-tutorial-2024.4.0/tutorial/_version.py
+-rw-r--r--   0 rieder     (501) staff       (20)       34 2022-11-22 11:55:13.000000 amuse-tutorial-2024.4.0/tutorial/amuserc
+-rw-r--r--   0 rieder     (501) staff       (20)      449 2022-11-22 11:55:13.000000 amuse-tutorial-2024.4.0/tutorial/create_title.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1304 2022-11-22 11:55:13.000000 amuse-tutorial-2024.4.0/tutorial/index.rst
```

### Comparing `amuse-tutorial-2023.5.0/PKG-INFO` & `amuse-tutorial-2024.4.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-tutorial
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - tutorial
 Home-page: http://www.amusecode.org/
 Author: The AMUSE team
 Author-email: info@amusecode.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -19,11 +19,18 @@
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
+Requires-Dist: matplotlib>=2.2
+Requires-Dist: amuse-framework
+Requires-Dist: amuse-bhtree
+Requires-Dist: amuse-hermite
+Requires-Dist: amuse-seba
+Requires-Dist: amuse-sphray
+Requires-Dist: notebook
 
 This package installs the tutorial for the Astrophysical Multipurpose Software Environment (AMUSE).
```

### Comparing `amuse-tutorial-2023.5.0/amuse_tutorial.egg-info/PKG-INFO` & `amuse-tutorial-2024.4.0/amuse_tutorial.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-tutorial
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - tutorial
 Home-page: http://www.amusecode.org/
 Author: The AMUSE team
 Author-email: info@amusecode.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -19,11 +19,18 @@
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
+Requires-Dist: matplotlib>=2.2
+Requires-Dist: amuse-framework
+Requires-Dist: amuse-bhtree
+Requires-Dist: amuse-hermite
+Requires-Dist: amuse-seba
+Requires-Dist: amuse-sphray
+Requires-Dist: notebook
 
 This package installs the tutorial for the Astrophysical Multipurpose Software Environment (AMUSE).
```

### Comparing `amuse-tutorial-2023.5.0/amuse_tutorial.egg-info/SOURCES.txt` & `amuse-tutorial-2024.4.0/amuse_tutorial.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,11 +26,11 @@
 tutorial/05-Attributes_and_functions_on_particle_collections.ipynb
 tutorial/06-Using_a_community_code.ipynb
 tutorial/07-Channels.ipynb
 tutorial/08-Grids.ipynb
 tutorial/09-Units_and_functions.ipynb
 tutorial/10-Radiative_transfer.ipynb
 tutorial/Makefile
+tutorial/_version.py
 tutorial/amuserc
 tutorial/create_title.py
-tutorial/index.rst
-tutorial/version.py
+tutorial/index.rst
```

### Comparing `amuse-tutorial-2023.5.0/bin/amusifier.in` & `amuse-tutorial-2024.4.0/bin/amusifier.in`

 * *Files identical despite different names*

### Comparing `amuse-tutorial-2023.5.0/setup.py` & `amuse-tutorial-2024.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,40 +23,33 @@
     long_description = fh.read()
 long_description_content_type = "text/markdown"
 
 all_data_files = find_data_files(
     'tutorial', 'share/amuse/tutorial', '*', recursive=True
 )
 
-try:
-    from tutorial.version import version
-    use_scm_version = False
-    setup_requires = []
-except ImportError:
-    version = False
-    setup_requires = ['setuptools_scm']
-    use_scm_version = {
-        "root": "../..",
-        "relative_to": __file__,
-        "write_to": "tutorial/version.py",
-    }
+setup_requires = ['setuptools_scm']
+use_scm_version = {
+    "root": "../..",
+    "relative_to": __file__,
+    "version_file": "tutorial/_version.py",
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
     # cmdclass=mapping_from_command_name_to_command_class,
     data_files=all_data_files,
     scripts=["bin/amuse-tutorial"],
     packages=[],
 )
```

### Comparing `amuse-tutorial-2023.5.0/support/__init__.py` & `amuse-tutorial-2024.4.0/support/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-tutorial-2023.5.0/support/classifiers.py` & `amuse-tutorial-2024.4.0/support/classifiers.py`

 * *Files identical despite different names*

### Comparing `amuse-tutorial-2023.5.0/support/config.py` & `amuse-tutorial-2024.4.0/support/config.py`

 * *Files identical despite different names*

### Comparing `amuse-tutorial-2023.5.0/support/generate_main.py` & `amuse-tutorial-2024.4.0/support/generate_main.py`

 * *Files identical despite different names*

### Comparing `amuse-tutorial-2023.5.0/support/getsp.class` & `amuse-tutorial-2024.4.0/support/getsp.class`

 * *Files identical despite different names*

### Comparing `amuse-tutorial-2023.5.0/support/getsp.java` & `amuse-tutorial-2024.4.0/support/getsp.java`

 * *Files identical despite different names*

### Comparing `amuse-tutorial-2023.5.0/support/misc.py` & `amuse-tutorial-2024.4.0/support/misc.py`

 * *Files identical despite different names*

### Comparing `amuse-tutorial-2023.5.0/support/setup_codes.py` & `amuse-tutorial-2024.4.0/support/setup_codes.py`

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

### Comparing `amuse-tutorial-2023.5.0/tutorial/00-Welcome.ipynb` & `amuse-tutorial-2024.4.0/tutorial/00-Welcome.ipynb`

 * *Files identical despite different names*

### Comparing `amuse-tutorial-2023.5.0/tutorial/01-Loading_AMUSE.ipynb` & `amuse-tutorial-2024.4.0/tutorial/01-Loading_AMUSE.ipynb`

 * *Files identical despite different names*

### Comparing `amuse-tutorial-2023.5.0/tutorial/02-Quantities_with_units.ipynb` & `amuse-tutorial-2024.4.0/tutorial/02-Quantities_with_units.ipynb`

 * *Files identical despite different names*

### Comparing `amuse-tutorial-2023.5.0/tutorial/03-Generic_units.ipynb` & `amuse-tutorial-2024.4.0/tutorial/03-Generic_units.ipynb`

 * *Files identical despite different names*

### Comparing `amuse-tutorial-2023.5.0/tutorial/04-Collections_of_Particles.ipynb` & `amuse-tutorial-2024.4.0/tutorial/04-Collections_of_Particles.ipynb`

 * *Files identical despite different names*

### Comparing `amuse-tutorial-2023.5.0/tutorial/05-Attributes_and_functions_on_particle_collections.ipynb` & `amuse-tutorial-2024.4.0/tutorial/05-Attributes_and_functions_on_particle_collections.ipynb`

 * *Files identical despite different names*

### Comparing `amuse-tutorial-2023.5.0/tutorial/06-Using_a_community_code.ipynb` & `amuse-tutorial-2024.4.0/tutorial/06-Using_a_community_code.ipynb`

 * *Files identical despite different names*

### Comparing `amuse-tutorial-2023.5.0/tutorial/07-Channels.ipynb` & `amuse-tutorial-2024.4.0/tutorial/07-Channels.ipynb`

 * *Files identical despite different names*

### Comparing `amuse-tutorial-2023.5.0/tutorial/08-Grids.ipynb` & `amuse-tutorial-2024.4.0/tutorial/08-Grids.ipynb`

 * *Files identical despite different names*

### Comparing `amuse-tutorial-2023.5.0/tutorial/09-Units_and_functions.ipynb` & `amuse-tutorial-2024.4.0/tutorial/09-Units_and_functions.ipynb`

 * *Files identical despite different names*

### Comparing `amuse-tutorial-2023.5.0/tutorial/10-Radiative_transfer.ipynb` & `amuse-tutorial-2024.4.0/tutorial/10-Radiative_transfer.ipynb`

 * *Files identical despite different names*

### Comparing `amuse-tutorial-2023.5.0/tutorial/Makefile` & `amuse-tutorial-2024.4.0/tutorial/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-tutorial-2023.5.0/tutorial/index.rst` & `amuse-tutorial-2024.4.0/tutorial/index.rst`

 * *Files identical despite different names*

