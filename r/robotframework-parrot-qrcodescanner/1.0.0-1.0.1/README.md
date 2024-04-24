# Comparing `tmp/robotframework_parrot_qrcodescanner-1.0.0.tar.gz` & `tmp/robotframework_parrot_qrcodescanner-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_parrot_qrcodescanner-1.0.0.tar", last modified: Mon Apr 15 08:08:13 2024, max compression
+gzip compressed data, was "robotframework_parrot_qrcodescanner-1.0.1.tar", last modified: Wed Apr 24 05:49:54 2024, max compression
```

## Comparing `robotframework_parrot_qrcodescanner-1.0.0.tar` & `robotframework_parrot_qrcodescanner-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-15 08:08:13.212980 robotframework_parrot_qrcodescanner-1.0.0/
--rw-rw-r--   0 user      (1000) user      (1000)    11358 2024-04-02 07:20:32.000000 robotframework_parrot_qrcodescanner-1.0.0/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)      768 2024-04-15 08:08:13.212980 robotframework_parrot_qrcodescanner-1.0.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      325 2024-04-05 13:33:06.000000 robotframework_parrot_qrcodescanner-1.0.0/README.md
--rw-rw-r--   0 user      (1000) user      (1000)      107 2024-04-05 13:36:14.000000 robotframework_parrot_qrcodescanner-1.0.0/pyproject.toml
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-15 08:08:13.208980 robotframework_parrot_qrcodescanner-1.0.0/qrcode/
--rw-rw-r--   0 user      (1000) user      (1000)     3177 2024-04-01 12:48:57.000000 robotframework_parrot_qrcodescanner-1.0.0/qrcode/QRCode.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-02 07:01:57.000000 robotframework_parrot_qrcodescanner-1.0.0/qrcode/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-15 08:08:13.212980 robotframework_parrot_qrcodescanner-1.0.0/robotframework_parrot_qrcodescanner.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      768 2024-04-15 08:08:13.000000 robotframework_parrot_qrcodescanner-1.0.0/robotframework_parrot_qrcodescanner.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      372 2024-04-15 08:08:13.000000 robotframework_parrot_qrcodescanner-1.0.0/robotframework_parrot_qrcodescanner.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-15 08:08:13.000000 robotframework_parrot_qrcodescanner-1.0.0/robotframework_parrot_qrcodescanner.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       29 2024-04-15 08:08:13.000000 robotframework_parrot_qrcodescanner-1.0.0/robotframework_parrot_qrcodescanner.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        7 2024-04-15 08:08:13.000000 robotframework_parrot_qrcodescanner-1.0.0/robotframework_parrot_qrcodescanner.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)      531 2024-04-15 08:08:13.212980 robotframework_parrot_qrcodescanner-1.0.0/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-24 05:49:54.022993 robotframework_parrot_qrcodescanner-1.0.1/
+-rw-rw-r--   0 user      (1000) user      (1000)    11358 2024-04-02 07:20:32.000000 robotframework_parrot_qrcodescanner-1.0.1/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)      768 2024-04-24 05:49:54.022993 robotframework_parrot_qrcodescanner-1.0.1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      325 2024-04-05 13:33:06.000000 robotframework_parrot_qrcodescanner-1.0.1/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)      107 2024-04-05 13:36:14.000000 robotframework_parrot_qrcodescanner-1.0.1/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)      571 2024-04-24 05:49:54.022993 robotframework_parrot_qrcodescanner-1.0.1/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-24 05:49:54.022993 robotframework_parrot_qrcodescanner-1.0.1/src/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-24 05:49:54.022993 robotframework_parrot_qrcodescanner-1.0.1/src/parrot/
+-rw-rw-r--   0 user      (1000) user      (1000)     3177 2024-04-01 12:48:57.000000 robotframework_parrot_qrcodescanner-1.0.1/src/parrot/QRCode.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-02 07:01:57.000000 robotframework_parrot_qrcodescanner-1.0.1/src/parrot/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-24 05:49:54.022993 robotframework_parrot_qrcodescanner-1.0.1/src/robotframework_parrot_qrcodescanner.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      768 2024-04-24 05:49:54.000000 robotframework_parrot_qrcodescanner-1.0.1/src/robotframework_parrot_qrcodescanner.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      400 2024-04-24 05:49:54.000000 robotframework_parrot_qrcodescanner-1.0.1/src/robotframework_parrot_qrcodescanner.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-24 05:49:54.000000 robotframework_parrot_qrcodescanner-1.0.1/src/robotframework_parrot_qrcodescanner.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       29 2024-04-24 05:49:54.000000 robotframework_parrot_qrcodescanner-1.0.1/src/robotframework_parrot_qrcodescanner.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        7 2024-04-24 05:49:54.000000 robotframework_parrot_qrcodescanner-1.0.1/src/robotframework_parrot_qrcodescanner.egg-info/top_level.txt
```

### Comparing `robotframework_parrot_qrcodescanner-1.0.0/LICENSE` & `robotframework_parrot_qrcodescanner-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_parrot_qrcodescanner-1.0.0/PKG-INFO` & `robotframework_parrot_qrcodescanner-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-parrot-qrcodescanner
-Version: 1.0.0
+Version: 1.0.1
 Summary: QR Code Scanner to scan the QR images
 Home-page: https://github.com/zilogic-systems/parrot
 Author: Zilogic Systems
 Author-email: code@zilogic.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `robotframework_parrot_qrcodescanner-1.0.0/qrcode/QRCode.py` & `robotframework_parrot_qrcodescanner-1.0.1/src/parrot/QRCode.py`

 * *Files identical despite different names*

### Comparing `robotframework_parrot_qrcodescanner-1.0.0/robotframework_parrot_qrcodescanner.egg-info/PKG-INFO` & `robotframework_parrot_qrcodescanner-1.0.1/src/robotframework_parrot_qrcodescanner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-parrot-qrcodescanner
-Version: 1.0.0
+Version: 1.0.1
 Summary: QR Code Scanner to scan the QR images
 Home-page: https://github.com/zilogic-systems/parrot
 Author: Zilogic Systems
 Author-email: code@zilogic.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `robotframework_parrot_qrcodescanner-1.0.0/setup.cfg` & `robotframework_parrot_qrcodescanner-1.0.1/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 [metadata]
 name = robotframework-parrot-qrcodescanner
-version = 1.0.0
+version = 1.0.1
 author = Zilogic Systems
 author_email = code@zilogic.com
 description = QR Code Scanner to scan the QR images
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/zilogic-systems/parrot
 classifiers = 
 	Programming Language :: Python :: 3
 
 [options]
 install_requires = 
 	pyzbar
 	pillow
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
