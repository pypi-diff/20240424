# Comparing `tmp/robotframework_parrot_relaycontroller-1.0.0.tar.gz` & `tmp/robotframework_parrot_relaycontroller-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_parrot_relaycontroller-1.0.0.tar", last modified: Tue Apr 16 10:44:02 2024, max compression
+gzip compressed data, was "robotframework_parrot_relaycontroller-1.0.1.tar", last modified: Wed Apr 24 05:52:00 2024, max compression
```

## Comparing `robotframework_parrot_relaycontroller-1.0.0.tar` & `robotframework_parrot_relaycontroller-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-16 10:44:02.117074 robotframework_parrot_relaycontroller-1.0.0/
--rw-rw-r--   0 user      (1000) user      (1000)    11357 2024-04-10 06:17:16.000000 robotframework_parrot_relaycontroller-1.0.0/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)      734 2024-04-16 10:44:02.117074 robotframework_parrot_relaycontroller-1.0.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      330 2024-04-10 12:07:10.000000 robotframework_parrot_relaycontroller-1.0.0/README.md
--rw-rw-r--   0 user      (1000) user      (1000)      107 2024-04-10 12:08:58.000000 robotframework_parrot_relaycontroller-1.0.0/pyproject.toml
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-16 10:44:02.117074 robotframework_parrot_relaycontroller-1.0.0/relay/
--rw-rw-r--   0 user      (1000) user      (1000)     6425 2024-04-10 06:17:16.000000 robotframework_parrot_relaycontroller-1.0.0/relay/RelayController.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-10 12:04:22.000000 robotframework_parrot_relaycontroller-1.0.0/relay/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-16 10:44:02.117074 robotframework_parrot_relaycontroller-1.0.0/robotframework_parrot_relaycontroller.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      734 2024-04-16 10:44:02.000000 robotframework_parrot_relaycontroller-1.0.0/robotframework_parrot_relaycontroller.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      389 2024-04-16 10:44:02.000000 robotframework_parrot_relaycontroller-1.0.0/robotframework_parrot_relaycontroller.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-16 10:44:02.000000 robotframework_parrot_relaycontroller-1.0.0/robotframework_parrot_relaycontroller.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       24 2024-04-16 10:44:02.000000 robotframework_parrot_relaycontroller-1.0.0/robotframework_parrot_relaycontroller.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        6 2024-04-16 10:44:02.000000 robotframework_parrot_relaycontroller-1.0.0/robotframework_parrot_relaycontroller.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)      506 2024-04-16 10:44:02.117074 robotframework_parrot_relaycontroller-1.0.0/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-24 05:52:00.490980 robotframework_parrot_relaycontroller-1.0.1/
+-rw-rw-r--   0 user      (1000) user      (1000)    11357 2024-04-10 06:17:16.000000 robotframework_parrot_relaycontroller-1.0.1/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)      734 2024-04-24 05:52:00.490980 robotframework_parrot_relaycontroller-1.0.1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      330 2024-04-10 12:07:10.000000 robotframework_parrot_relaycontroller-1.0.1/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)      107 2024-04-10 12:08:58.000000 robotframework_parrot_relaycontroller-1.0.1/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)      546 2024-04-24 05:52:00.490980 robotframework_parrot_relaycontroller-1.0.1/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-24 05:52:00.490980 robotframework_parrot_relaycontroller-1.0.1/src/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-24 05:52:00.490980 robotframework_parrot_relaycontroller-1.0.1/src/parrot/
+-rw-rw-r--   0 user      (1000) user      (1000)     6425 2024-04-10 06:17:16.000000 robotframework_parrot_relaycontroller-1.0.1/src/parrot/RelayController.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-04-10 12:04:22.000000 robotframework_parrot_relaycontroller-1.0.1/src/parrot/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-24 05:52:00.490980 robotframework_parrot_relaycontroller-1.0.1/src/robotframework_parrot_relaycontroller.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      734 2024-04-24 05:52:00.000000 robotframework_parrot_relaycontroller-1.0.1/src/robotframework_parrot_relaycontroller.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      419 2024-04-24 05:52:00.000000 robotframework_parrot_relaycontroller-1.0.1/src/robotframework_parrot_relaycontroller.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-24 05:52:00.000000 robotframework_parrot_relaycontroller-1.0.1/src/robotframework_parrot_relaycontroller.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       24 2024-04-24 05:52:00.000000 robotframework_parrot_relaycontroller-1.0.1/src/robotframework_parrot_relaycontroller.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        7 2024-04-24 05:52:00.000000 robotframework_parrot_relaycontroller-1.0.1/src/robotframework_parrot_relaycontroller.egg-info/top_level.txt
```

### Comparing `robotframework_parrot_relaycontroller-1.0.0/LICENSE` & `robotframework_parrot_relaycontroller-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_parrot_relaycontroller-1.0.0/PKG-INFO` & `robotframework_parrot_relaycontroller-1.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-parrot-relaycontroller
-Version: 1.0.0
+Version: 1.0.1
 Summary: Relay Controller
 Home-page: https://github.com/zilogic-systems/parrot
 Author: Zilogic Systems
 Author-email: code@zilogic.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `robotframework_parrot_relaycontroller-1.0.0/relay/RelayController.py` & `robotframework_parrot_relaycontroller-1.0.1/src/parrot/RelayController.py`

 * *Files identical despite different names*

### Comparing `robotframework_parrot_relaycontroller-1.0.0/robotframework_parrot_relaycontroller.egg-info/PKG-INFO` & `robotframework_parrot_relaycontroller-1.0.1/src/robotframework_parrot_relaycontroller.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-parrot-relaycontroller
-Version: 1.0.0
+Version: 1.0.1
 Summary: Relay Controller
 Home-page: https://github.com/zilogic-systems/parrot
 Author: Zilogic Systems
 Author-email: code@zilogic.com
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

