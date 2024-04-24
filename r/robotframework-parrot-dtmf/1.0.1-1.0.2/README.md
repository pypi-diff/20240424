# Comparing `tmp/robotframework_parrot_dtmf-1.0.1.tar.gz` & `tmp/robotframework_parrot_dtmf-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_parrot_dtmf-1.0.1.tar", last modified: Mon Apr 22 06:28:01 2024, max compression
+gzip compressed data, was "robotframework_parrot_dtmf-1.0.2.tar", last modified: Wed Apr 24 05:45:33 2024, max compression
```

## Comparing `robotframework_parrot_dtmf-1.0.1.tar` & `robotframework_parrot_dtmf-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-22 06:28:01.214660 robotframework_parrot_dtmf-1.0.1/
--rw-rw-r--   0 user      (1000) user      (1000)    11357 2024-04-15 11:33:40.000000 robotframework_parrot_dtmf-1.0.1/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)      788 2024-04-22 06:28:01.214660 robotframework_parrot_dtmf-1.0.1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      316 2024-04-16 10:40:33.000000 robotframework_parrot_dtmf-1.0.1/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-22 06:28:01.214660 robotframework_parrot_dtmf-1.0.1/dtmf/
--rw-rw-r--   0 user      (1000) user      (1000)    10140 2024-04-15 11:31:38.000000 robotframework_parrot_dtmf-1.0.1/dtmf/DTMF.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-15 11:30:30.000000 robotframework_parrot_dtmf-1.0.1/dtmf/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      107 2024-04-15 11:35:06.000000 robotframework_parrot_dtmf-1.0.1/pyproject.toml
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-22 06:28:01.214660 robotframework_parrot_dtmf-1.0.1/robotframework_parrot_dtmf.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      788 2024-04-22 06:28:01.000000 robotframework_parrot_dtmf-1.0.1/robotframework_parrot_dtmf.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      321 2024-04-22 06:28:01.000000 robotframework_parrot_dtmf-1.0.1/robotframework_parrot_dtmf.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-22 06:28:01.000000 robotframework_parrot_dtmf-1.0.1/robotframework_parrot_dtmf.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       27 2024-04-22 06:28:01.000000 robotframework_parrot_dtmf-1.0.1/robotframework_parrot_dtmf.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        5 2024-04-22 06:28:01.000000 robotframework_parrot_dtmf-1.0.1/robotframework_parrot_dtmf.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)      561 2024-04-22 06:28:01.214660 robotframework_parrot_dtmf-1.0.1/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-24 05:45:33.306849 robotframework_parrot_dtmf-1.0.2/
+-rw-rw-r--   0 user      (1000) user      (1000)    11357 2024-04-15 11:33:40.000000 robotframework_parrot_dtmf-1.0.2/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)      788 2024-04-24 05:45:33.306849 robotframework_parrot_dtmf-1.0.2/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      316 2024-04-16 10:40:33.000000 robotframework_parrot_dtmf-1.0.2/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)      107 2024-04-15 11:35:06.000000 robotframework_parrot_dtmf-1.0.2/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)      601 2024-04-24 05:45:33.306849 robotframework_parrot_dtmf-1.0.2/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-24 05:45:33.286849 robotframework_parrot_dtmf-1.0.2/src/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-24 05:45:33.306849 robotframework_parrot_dtmf-1.0.2/src/parrot/
+-rw-rw-r--   0 user      (1000) user      (1000)    10140 2024-04-15 11:31:38.000000 robotframework_parrot_dtmf-1.0.2/src/parrot/DTMF.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-15 11:30:30.000000 robotframework_parrot_dtmf-1.0.2/src/parrot/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-24 05:45:33.306849 robotframework_parrot_dtmf-1.0.2/src/robotframework_parrot_dtmf.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      788 2024-04-24 05:45:33.000000 robotframework_parrot_dtmf-1.0.2/src/robotframework_parrot_dtmf.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      353 2024-04-24 05:45:33.000000 robotframework_parrot_dtmf-1.0.2/src/robotframework_parrot_dtmf.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-24 05:45:33.000000 robotframework_parrot_dtmf-1.0.2/src/robotframework_parrot_dtmf.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       27 2024-04-24 05:45:33.000000 robotframework_parrot_dtmf-1.0.2/src/robotframework_parrot_dtmf.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        7 2024-04-24 05:45:33.000000 robotframework_parrot_dtmf-1.0.2/src/robotframework_parrot_dtmf.egg-info/top_level.txt
```

### Comparing `robotframework_parrot_dtmf-1.0.1/LICENSE` & `robotframework_parrot_dtmf-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_parrot_dtmf-1.0.1/PKG-INFO` & `robotframework_parrot_dtmf-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-parrot-dtmf
-Version: 1.0.1
+Version: 1.0.2
 Summary: DTMF (Dual tone multi frequency) Library used to generate and verify DTMF tone
 Home-page: https://github.com/zilogic-systems/parrot
 Author: Zilogic Systems
 Author-email: code@zilogic.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `robotframework_parrot_dtmf-1.0.1/dtmf/DTMF.py` & `robotframework_parrot_dtmf-1.0.2/src/parrot/DTMF.py`

 * *Files identical despite different names*

### Comparing `robotframework_parrot_dtmf-1.0.1/robotframework_parrot_dtmf.egg-info/PKG-INFO` & `robotframework_parrot_dtmf-1.0.2/src/robotframework_parrot_dtmf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-parrot-dtmf
-Version: 1.0.1
+Version: 1.0.2
 Summary: DTMF (Dual tone multi frequency) Library used to generate and verify DTMF tone
 Home-page: https://github.com/zilogic-systems/parrot
 Author: Zilogic Systems
 Author-email: code@zilogic.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `robotframework_parrot_dtmf-1.0.1/setup.cfg` & `robotframework_parrot_dtmf-1.0.2/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 [metadata]
 name = robotframework-parrot-dtmf
-version = 1.0.1
+version = 1.0.2
 author = Zilogic Systems
 author_email = code@zilogic.com
 description = DTMF (Dual tone multi frequency) Library used to generate and verify DTMF tone
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/zilogic-systems/parrot
 classifiers = 
 	Programming Language :: Python :: 3
 
 [options]
 install_requires = 
 	pydub
 	numpy
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

