# Comparing `tmp/robotframework_parrot_ocrlib-1.0.2.tar.gz` & `tmp/robotframework_parrot_ocrlib-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_parrot_ocrlib-1.0.2.tar", last modified: Mon Apr 22 06:24:18 2024, max compression
+gzip compressed data, was "robotframework_parrot_ocrlib-1.0.3.tar", last modified: Wed Apr 24 05:48:01 2024, max compression
```

## Comparing `robotframework_parrot_ocrlib-1.0.2.tar` & `robotframework_parrot_ocrlib-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-22 06:24:18.364442 robotframework_parrot_ocrlib-1.0.2/
--rw-rw-r--   0 user      (1000) user      (1000)    11357 2024-04-10 06:17:16.000000 robotframework_parrot_ocrlib-1.0.2/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)      962 2024-04-22 06:24:18.364442 robotframework_parrot_ocrlib-1.0.2/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      486 2024-04-22 06:11:01.000000 robotframework_parrot_ocrlib-1.0.2/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-22 06:24:18.364442 robotframework_parrot_ocrlib-1.0.2/ocr/
--rw-rw-r--   0 user      (1000) user      (1000)     2042 2024-04-10 06:17:16.000000 robotframework_parrot_ocrlib-1.0.2/ocr/OCRLib.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-15 11:22:39.000000 robotframework_parrot_ocrlib-1.0.2/ocr/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      107 2024-04-10 12:39:25.000000 robotframework_parrot_ocrlib-1.0.2/pyproject.toml
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-22 06:24:18.364442 robotframework_parrot_ocrlib-1.0.2/robotframework_parrot_ocrlib.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      962 2024-04-22 06:24:18.000000 robotframework_parrot_ocrlib-1.0.2/robotframework_parrot_ocrlib.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      331 2024-04-22 06:24:18.000000 robotframework_parrot_ocrlib-1.0.2/robotframework_parrot_ocrlib.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-22 06:24:18.000000 robotframework_parrot_ocrlib-1.0.2/robotframework_parrot_ocrlib.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       40 2024-04-22 06:24:18.000000 robotframework_parrot_ocrlib-1.0.2/robotframework_parrot_ocrlib.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        4 2024-04-22 06:24:18.000000 robotframework_parrot_ocrlib-1.0.2/robotframework_parrot_ocrlib.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)      551 2024-04-22 06:24:18.364442 robotframework_parrot_ocrlib-1.0.2/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-24 05:48:01.438964 robotframework_parrot_ocrlib-1.0.3/
+-rw-rw-r--   0 user      (1000) user      (1000)    11357 2024-04-10 06:17:16.000000 robotframework_parrot_ocrlib-1.0.3/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)      962 2024-04-24 05:48:01.438964 robotframework_parrot_ocrlib-1.0.3/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      486 2024-04-22 06:11:01.000000 robotframework_parrot_ocrlib-1.0.3/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)      107 2024-04-10 12:39:25.000000 robotframework_parrot_ocrlib-1.0.3/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)      591 2024-04-24 05:48:01.438964 robotframework_parrot_ocrlib-1.0.3/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-24 05:48:01.414964 robotframework_parrot_ocrlib-1.0.3/src/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-24 05:48:01.434964 robotframework_parrot_ocrlib-1.0.3/src/parrot/
+-rw-rw-r--   0 user      (1000) user      (1000)     2042 2024-04-10 06:17:16.000000 robotframework_parrot_ocrlib-1.0.3/src/parrot/OCRLib.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-15 11:22:39.000000 robotframework_parrot_ocrlib-1.0.3/src/parrot/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-24 05:48:01.438964 robotframework_parrot_ocrlib-1.0.3/src/robotframework_parrot_ocrlib.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      962 2024-04-24 05:48:01.000000 robotframework_parrot_ocrlib-1.0.3/src/robotframework_parrot_ocrlib.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      365 2024-04-24 05:48:01.000000 robotframework_parrot_ocrlib-1.0.3/src/robotframework_parrot_ocrlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-24 05:48:01.000000 robotframework_parrot_ocrlib-1.0.3/src/robotframework_parrot_ocrlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       40 2024-04-24 05:48:01.000000 robotframework_parrot_ocrlib-1.0.3/src/robotframework_parrot_ocrlib.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        7 2024-04-24 05:48:01.000000 robotframework_parrot_ocrlib-1.0.3/src/robotframework_parrot_ocrlib.egg-info/top_level.txt
```

### Comparing `robotframework_parrot_ocrlib-1.0.2/LICENSE` & `robotframework_parrot_ocrlib-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_parrot_ocrlib-1.0.2/PKG-INFO` & `robotframework_parrot_ocrlib-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-parrot-ocrlib
-Version: 1.0.2
+Version: 1.0.3
 Summary: OCR Library to recognize text within a digital image
 Home-page: https://github.com/zilogic-systems/parrot
 Author: Zilogic Systems
 Author-email: code@zilogic.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `robotframework_parrot_ocrlib-1.0.2/ocr/OCRLib.py` & `robotframework_parrot_ocrlib-1.0.3/src/parrot/OCRLib.py`

 * *Files identical despite different names*

### Comparing `robotframework_parrot_ocrlib-1.0.2/robotframework_parrot_ocrlib.egg-info/PKG-INFO` & `robotframework_parrot_ocrlib-1.0.3/src/robotframework_parrot_ocrlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-parrot-ocrlib
-Version: 1.0.2
+Version: 1.0.3
 Summary: OCR Library to recognize text within a digital image
 Home-page: https://github.com/zilogic-systems/parrot
 Author: Zilogic Systems
 Author-email: code@zilogic.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `robotframework_parrot_ocrlib-1.0.2/setup.cfg` & `robotframework_parrot_ocrlib-1.0.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = robotframework-parrot-ocrlib
-version = 1.0.2
+version = 1.0.3
 author = Zilogic Systems
 author_email = code@zilogic.com
 description = OCR Library to recognize text within a digital image
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/zilogic-systems/parrot
 classifiers = 
@@ -12,15 +12,19 @@
 
 [options]
 install_requires = 
 	pillow
 	pytesseract
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

