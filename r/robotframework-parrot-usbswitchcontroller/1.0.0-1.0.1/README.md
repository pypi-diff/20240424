# Comparing `tmp/robotframework_parrot_usbswitchcontroller-1.0.0.tar.gz` & `tmp/robotframework_parrot_usbswitchcontroller-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_parrot_usbswitchcontroller-1.0.0.tar", last modified: Mon Apr 22 06:33:29 2024, max compression
+gzip compressed data, was "robotframework_parrot_usbswitchcontroller-1.0.1.tar", last modified: Wed Apr 24 05:53:55 2024, max compression
```

## Comparing `robotframework_parrot_usbswitchcontroller-1.0.0.tar` & `robotframework_parrot_usbswitchcontroller-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-22 06:33:29.936781 robotframework_parrot_usbswitchcontroller-1.0.0/
--rw-rw-r--   0 user      (1000) user      (1000)    11357 2024-04-10 06:17:16.000000 robotframework_parrot_usbswitchcontroller-1.0.0/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)      747 2024-04-22 06:33:29.936781 robotframework_parrot_usbswitchcontroller-1.0.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      335 2024-04-22 06:32:35.000000 robotframework_parrot_usbswitchcontroller-1.0.0/README.md
--rw-rw-r--   0 user      (1000) user      (1000)      107 2024-04-15 10:24:47.000000 robotframework_parrot_usbswitchcontroller-1.0.0/pyproject.toml
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-22 06:33:29.936781 robotframework_parrot_usbswitchcontroller-1.0.0/robotframework_parrot_usbswitchcontroller.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      747 2024-04-22 06:33:29.000000 robotframework_parrot_usbswitchcontroller-1.0.0/robotframework_parrot_usbswitchcontroller.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      415 2024-04-22 06:33:29.000000 robotframework_parrot_usbswitchcontroller-1.0.0/robotframework_parrot_usbswitchcontroller.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-22 06:33:29.000000 robotframework_parrot_usbswitchcontroller-1.0.0/robotframework_parrot_usbswitchcontroller.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       24 2024-04-22 06:33:29.000000 robotframework_parrot_usbswitchcontroller-1.0.0/robotframework_parrot_usbswitchcontroller.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        7 2024-04-22 06:33:29.000000 robotframework_parrot_usbswitchcontroller-1.0.0/robotframework_parrot_usbswitchcontroller.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)      515 2024-04-22 06:33:29.936781 robotframework_parrot_usbswitchcontroller-1.0.0/setup.cfg
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-22 06:33:29.936781 robotframework_parrot_usbswitchcontroller-1.0.0/switch/
--rw-rw-r--   0 user      (1000) user      (1000)     6425 2024-04-15 10:10:34.000000 robotframework_parrot_usbswitchcontroller-1.0.0/switch/USBSwitchController.py
--rw-rw-r--   0 user      (1000) user      (1000)       26 2024-04-15 10:25:10.000000 robotframework_parrot_usbswitchcontroller-1.0.0/switch/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-24 05:53:55.806935 robotframework_parrot_usbswitchcontroller-1.0.1/
+-rw-rw-r--   0 user      (1000) user      (1000)    11357 2024-04-10 06:17:16.000000 robotframework_parrot_usbswitchcontroller-1.0.1/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)      747 2024-04-24 05:53:55.806935 robotframework_parrot_usbswitchcontroller-1.0.1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      335 2024-04-22 06:32:35.000000 robotframework_parrot_usbswitchcontroller-1.0.1/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)      107 2024-04-15 10:24:47.000000 robotframework_parrot_usbswitchcontroller-1.0.1/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)      555 2024-04-24 05:53:55.806935 robotframework_parrot_usbswitchcontroller-1.0.1/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-24 05:53:55.806935 robotframework_parrot_usbswitchcontroller-1.0.1/src/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-24 05:53:55.806935 robotframework_parrot_usbswitchcontroller-1.0.1/src/parrot/
+-rw-rw-r--   0 user      (1000) user      (1000)     6425 2024-04-15 10:10:34.000000 robotframework_parrot_usbswitchcontroller-1.0.1/src/parrot/USBSwitchController.py
+-rw-rw-r--   0 user      (1000) user      (1000)       26 2024-04-15 10:25:10.000000 robotframework_parrot_usbswitchcontroller-1.0.1/src/parrot/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-24 05:53:55.806935 robotframework_parrot_usbswitchcontroller-1.0.1/src/robotframework_parrot_usbswitchcontroller.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      747 2024-04-24 05:53:55.000000 robotframework_parrot_usbswitchcontroller-1.0.1/src/robotframework_parrot_usbswitchcontroller.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      443 2024-04-24 05:53:55.000000 robotframework_parrot_usbswitchcontroller-1.0.1/src/robotframework_parrot_usbswitchcontroller.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-24 05:53:55.000000 robotframework_parrot_usbswitchcontroller-1.0.1/src/robotframework_parrot_usbswitchcontroller.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       24 2024-04-24 05:53:55.000000 robotframework_parrot_usbswitchcontroller-1.0.1/src/robotframework_parrot_usbswitchcontroller.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        7 2024-04-24 05:53:55.000000 robotframework_parrot_usbswitchcontroller-1.0.1/src/robotframework_parrot_usbswitchcontroller.egg-info/top_level.txt
```

### Comparing `robotframework_parrot_usbswitchcontroller-1.0.0/LICENSE` & `robotframework_parrot_usbswitchcontroller-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_parrot_usbswitchcontroller-1.0.0/PKG-INFO` & `robotframework_parrot_usbswitchcontroller-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-parrot-usbswitchcontroller
-Version: 1.0.0
+Version: 1.0.1
 Summary: USB Switch Controller
 Home-page: https://github.com/zilogic-systems/parrot
 Author: Zilogic Systems
 Author-email: code@zilogic.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `robotframework_parrot_usbswitchcontroller-1.0.0/robotframework_parrot_usbswitchcontroller.egg-info/PKG-INFO` & `robotframework_parrot_usbswitchcontroller-1.0.1/src/robotframework_parrot_usbswitchcontroller.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-parrot-usbswitchcontroller
-Version: 1.0.0
+Version: 1.0.1
 Summary: USB Switch Controller
 Home-page: https://github.com/zilogic-systems/parrot
 Author: Zilogic Systems
 Author-email: code@zilogic.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `robotframework_parrot_usbswitchcontroller-1.0.0/switch/USBSwitchController.py` & `robotframework_parrot_usbswitchcontroller-1.0.1/src/parrot/USBSwitchController.py`

 * *Files identical despite different names*

