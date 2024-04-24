# Comparing `tmp/robotframework-parrot-adbcontroller-1.0.0.tar.gz` & `tmp/robotframework_parrot_adbcontroller-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-parrot-adbcontroller-1.0.0.tar", last modified: Fri Apr 12 10:34:36 2024, max compression
+gzip compressed data, was "robotframework_parrot_adbcontroller-1.0.1.tar", last modified: Wed Apr 24 05:37:59 2024, max compression
```

## Comparing `robotframework-parrot-adbcontroller-1.0.0.tar` & `robotframework_parrot_adbcontroller-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-12 10:34:36.389650 robotframework-parrot-adbcontroller-1.0.0/
--rw-rw-r--   0 user      (1000) user      (1000)    11357 2024-04-10 06:17:16.000000 robotframework-parrot-adbcontroller-1.0.0/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)      800 2024-04-12 10:34:36.389650 robotframework-parrot-adbcontroller-1.0.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      326 2024-04-12 10:32:58.000000 robotframework-parrot-adbcontroller-1.0.0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-12 10:34:36.389650 robotframework-parrot-adbcontroller-1.0.0/adb/
--rw-rw-r--   0 user      (1000) user      (1000)    24441 2024-04-10 06:17:16.000000 robotframework-parrot-adbcontroller-1.0.0/adb/ADBController.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-12 10:18:06.000000 robotframework-parrot-adbcontroller-1.0.0/adb/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      107 2024-04-12 10:33:22.000000 robotframework-parrot-adbcontroller-1.0.0/pyproject.toml
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-12 10:34:36.389650 robotframework-parrot-adbcontroller-1.0.0/robotframework_parrot_adbcontroller.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      800 2024-04-12 10:34:36.000000 robotframework-parrot-adbcontroller-1.0.0/robotframework_parrot_adbcontroller.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      373 2024-04-12 10:34:36.000000 robotframework-parrot-adbcontroller-1.0.0/robotframework_parrot_adbcontroller.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-12 10:34:36.000000 robotframework-parrot-adbcontroller-1.0.0/robotframework_parrot_adbcontroller.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       15 2024-04-12 10:34:36.000000 robotframework-parrot-adbcontroller-1.0.0/robotframework_parrot_adbcontroller.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        4 2024-04-12 10:34:36.000000 robotframework-parrot-adbcontroller-1.0.0/robotframework_parrot_adbcontroller.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)      568 2024-04-12 10:34:36.393650 robotframework-parrot-adbcontroller-1.0.0/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-24 05:37:59.189622 robotframework_parrot_adbcontroller-1.0.1/
+-rw-rw-r--   0 user      (1000) user      (1000)    11357 2024-04-10 06:17:16.000000 robotframework_parrot_adbcontroller-1.0.1/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)      702 2024-04-24 05:37:59.189622 robotframework_parrot_adbcontroller-1.0.1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      326 2024-04-12 10:32:58.000000 robotframework_parrot_adbcontroller-1.0.1/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)      107 2024-04-12 10:33:22.000000 robotframework_parrot_adbcontroller-1.0.1/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)      532 2024-04-24 05:37:59.189622 robotframework_parrot_adbcontroller-1.0.1/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-24 05:37:59.185622 robotframework_parrot_adbcontroller-1.0.1/src/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-24 05:37:59.185622 robotframework_parrot_adbcontroller-1.0.1/src/parrot/
+-rw-rw-r--   0 user      (1000) user      (1000)    24441 2024-04-10 06:17:16.000000 robotframework_parrot_adbcontroller-1.0.1/src/parrot/ADBController.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-12 10:18:06.000000 robotframework_parrot_adbcontroller-1.0.1/src/parrot/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-24 05:37:59.189622 robotframework_parrot_adbcontroller-1.0.1/src/robotframework_parrot_adbcontroller.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      702 2024-04-24 05:37:59.000000 robotframework_parrot_adbcontroller-1.0.1/src/robotframework_parrot_adbcontroller.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      407 2024-04-24 05:37:59.000000 robotframework_parrot_adbcontroller-1.0.1/src/robotframework_parrot_adbcontroller.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-24 05:37:59.000000 robotframework_parrot_adbcontroller-1.0.1/src/robotframework_parrot_adbcontroller.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       15 2024-04-24 05:37:59.000000 robotframework_parrot_adbcontroller-1.0.1/src/robotframework_parrot_adbcontroller.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        7 2024-04-24 05:37:59.000000 robotframework_parrot_adbcontroller-1.0.1/src/robotframework_parrot_adbcontroller.egg-info/top_level.txt
```

### Comparing `robotframework-parrot-adbcontroller-1.0.0/LICENSE` & `robotframework_parrot_adbcontroller-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-parrot-adbcontroller-1.0.0/PKG-INFO` & `robotframework_parrot_adbcontroller-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: robotframework-parrot-adbcontroller
-Version: 1.0.0
+Version: 1.0.1
 Summary: ADB Controller
 Home-page: https://github.com/zilogic-systems/parrot
 Author: Zilogic Systems
 Author-email: code@zilogic.com
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: robotframework
 
 # ADB Controller
```

### Comparing `robotframework-parrot-adbcontroller-1.0.0/adb/ADBController.py` & `robotframework_parrot_adbcontroller-1.0.1/src/parrot/ADBController.py`

 * *Files identical despite different names*

### Comparing `robotframework-parrot-adbcontroller-1.0.0/robotframework_parrot_adbcontroller.egg-info/PKG-INFO` & `robotframework_parrot_adbcontroller-1.0.1/src/robotframework_parrot_adbcontroller.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: robotframework-parrot-adbcontroller
-Version: 1.0.0
+Version: 1.0.1
 Summary: ADB Controller
 Home-page: https://github.com/zilogic-systems/parrot
 Author: Zilogic Systems
 Author-email: code@zilogic.com
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: robotframework
 
 # ADB Controller
```

### Comparing `robotframework-parrot-adbcontroller-1.0.0/setup.cfg` & `robotframework_parrot_adbcontroller-1.0.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [metadata]
 name = robotframework-parrot-adbcontroller
-version = 1.0.0
+version = 1.0.1
 author = Zilogic Systems
 author_email = code@zilogic.com
 description = ADB Controller
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/zilogic-systems/parrot
 classifiers = 
 	Programming Language :: Python :: 3
-	License :: OSI Approved :: MIT License
-	Operating System :: OS Independent
 
 [options]
 install_requires = 
 	robotframework
-packages = find:
+package_dir = 
+	=src
+packages = find_namespace:
 python_requires = >=3.6
-include_package_data = True
+
+[options.packages.find]
+where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

