# Comparing `tmp/robotframework_rpycremote-0.0.2.tar.gz` & `tmp/robotframework_rpycremote-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_rpycremote-0.0.2.tar", last modified: Mon Apr 22 16:42:49 2024, max compression
+gzip compressed data, was "robotframework_rpycremote-0.0.3.tar", last modified: Wed Apr 24 21:14:26 2024, max compression
```

## Comparing `robotframework_rpycremote-0.0.2.tar` & `robotframework_rpycremote-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:42:49.760967 robotframework_rpycremote-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:42:49.756967 robotframework_rpycremote-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:42:49.756967 robotframework_rpycremote-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-22 16:42:43.000000 robotframework_rpycremote-0.0.2/.github/workflows/pipeline.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-22 16:42:43.000000 robotframework_rpycremote-0.0.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-22 16:42:43.000000 robotframework_rpycremote-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-22 16:42:43.000000 robotframework_rpycremote-0.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-22 16:42:49.760967 robotframework_rpycremote-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-22 16:42:43.000000 robotframework_rpycremote-0.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:42:49.756967 robotframework_rpycremote-0.0.2/RPyCRobotRemote/
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-22 16:42:43.000000 robotframework_rpycremote-0.0.2/RPyCRobotRemote/RPyCRobotRemoteClient.py
--rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-04-22 16:42:43.000000 robotframework_rpycremote-0.0.2/RPyCRobotRemote/RPyCRobotRemoteServer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-22 16:42:43.000000 robotframework_rpycremote-0.0.2/RPyCRobotRemote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-22 16:42:49.000000 robotframework_rpycremote-0.0.2/RPyCRobotRemote/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-22 16:42:43.000000 robotframework_rpycremote-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:42:49.760967 robotframework_rpycremote-0.0.2/robotframework_rpycremote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-22 16:42:49.000000 robotframework_rpycremote-0.0.2/robotframework_rpycremote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-22 16:42:49.000000 robotframework_rpycremote-0.0.2/robotframework_rpycremote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 16:42:49.000000 robotframework_rpycremote-0.0.2/robotframework_rpycremote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-22 16:42:49.000000 robotframework_rpycremote-0.0.2/robotframework_rpycremote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-22 16:42:49.000000 robotframework_rpycremote-0.0.2/robotframework_rpycremote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 16:42:49.760967 robotframework_rpycremote-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-22 16:42:43.000000 robotframework_rpycremote-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:42:49.760967 robotframework_rpycremote-0.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-22 16:42:43.000000 robotframework_rpycremote-0.0.2/test/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-22 16:42:43.000000 robotframework_rpycremote-0.0.2/test/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-22 16:42:43.000000 robotframework_rpycremote-0.0.2/test/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-22 16:42:43.000000 robotframework_rpycremote-0.0.2/test/test.robot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:14:26.417055 robotframework_rpycremote-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:14:26.413055 robotframework_rpycremote-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:14:26.417055 robotframework_rpycremote-0.0.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:14:26.417055 robotframework_rpycremote-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/.github/workflows/pipeline.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-24 21:14:26.417055 robotframework_rpycremote-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:14:26.417055 robotframework_rpycremote-0.0.3/RPyCRobotRemote/
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/RPyCRobotRemote/RPyCRobotRemoteClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/RPyCRobotRemote/RPyCRobotRemoteServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/RPyCRobotRemote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-24 21:14:26.000000 robotframework_rpycremote-0.0.3/RPyCRobotRemote/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:14:26.417055 robotframework_rpycremote-0.0.3/robotframework_rpycremote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-24 21:14:26.000000 robotframework_rpycremote-0.0.3/robotframework_rpycremote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-24 21:14:26.000000 robotframework_rpycremote-0.0.3/robotframework_rpycremote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 21:14:26.000000 robotframework_rpycremote-0.0.3/robotframework_rpycremote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-24 21:14:26.000000 robotframework_rpycremote-0.0.3/robotframework_rpycremote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 21:14:26.000000 robotframework_rpycremote-0.0.3/robotframework_rpycremote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 21:14:26.417055 robotframework_rpycremote-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:14:26.417055 robotframework_rpycremote-0.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/test/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/test/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/test/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-24 21:14:20.000000 robotframework_rpycremote-0.0.3/test/test.robot
```

### Comparing `robotframework_rpycremote-0.0.2/.github/workflows/pipeline.yml` & `robotframework_rpycremote-0.0.3/.github/workflows/pipeline.yml`

 * *Files identical despite different names*

### Comparing `robotframework_rpycremote-0.0.2/.github/workflows/publish-to-pypi.yml` & `robotframework_rpycremote-0.0.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `robotframework_rpycremote-0.0.2/LICENSE.txt` & `robotframework_rpycremote-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotframework_rpycremote-0.0.2/PKG-INFO` & `robotframework_rpycremote-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-rpycremote
-Version: 0.0.2
+Version: 0.0.3
 Summary: Robot Framework Remote Library based on RPyC
 Author-email: René Lehfeld <54720674+rlehfeld@users.noreply.github.com>
 License: MIT
 Project-URL: Homepage, https://github.com/rlehfeld/robotframework-rpycremote
 Project-URL: Bug Reports, https://github.com/rlehfeld/robotframework-rpycremote/issues
 Project-URL: Source, https://github.com/rlehfeld/robotframework-rpycremote/
 Keywords: robotframework,robot-framework,rpyc
```

### Comparing `robotframework_rpycremote-0.0.2/README.rst` & `robotframework_rpycremote-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `robotframework_rpycremote-0.0.2/RPyCRobotRemote/RPyCRobotRemoteClient.py` & `robotframework_rpycremote-0.0.3/RPyCRobotRemote/RPyCRobotRemoteClient.py`

 * *Files identical despite different names*

### Comparing `robotframework_rpycremote-0.0.2/RPyCRobotRemote/RPyCRobotRemoteServer.py` & `robotframework_rpycremote-0.0.3/RPyCRobotRemote/RPyCRobotRemoteServer.py`

 * *Files identical despite different names*

### Comparing `robotframework_rpycremote-0.0.2/pyproject.toml` & `robotframework_rpycremote-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotframework_rpycremote-0.0.2/robotframework_rpycremote.egg-info/PKG-INFO` & `robotframework_rpycremote-0.0.3/robotframework_rpycremote.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-rpycremote
-Version: 0.0.2
+Version: 0.0.3
 Summary: Robot Framework Remote Library based on RPyC
 Author-email: René Lehfeld <54720674+rlehfeld@users.noreply.github.com>
 License: MIT
 Project-URL: Homepage, https://github.com/rlehfeld/robotframework-rpycremote
 Project-URL: Bug Reports, https://github.com/rlehfeld/robotframework-rpycremote/issues
 Project-URL: Source, https://github.com/rlehfeld/robotframework-rpycremote/
 Keywords: robotframework,robot-framework,rpyc
```

### Comparing `robotframework_rpycremote-0.0.2/robotframework_rpycremote.egg-info/SOURCES.txt` & `robotframework_rpycremote-0.0.3/robotframework_rpycremote.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 .gitignore
 LICENSE.txt
 README.rst
 pyproject.toml
 setup.py
+.github/ISSUE_TEMPLATE/bug_report.md
+.github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/pipeline.yml
 .github/workflows/publish-to-pypi.yml
 RPyCRobotRemote/RPyCRobotRemoteClient.py
 RPyCRobotRemote/RPyCRobotRemoteServer.py
 RPyCRobotRemote/__init__.py
 RPyCRobotRemote/_version.py
 robotframework_rpycremote.egg-info/PKG-INFO
```

### Comparing `robotframework_rpycremote-0.0.2/test/provider.py` & `robotframework_rpycremote-0.0.3/test/provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,19 @@
 
     class Dummy:
         """dummy class"""
         def __init__(self):
             self._value = 1
             self.value2 = 5
 
+        def __getattribute__(self, attr):
+            if attr in ('__class__'):
+                raise AttributeError(f'catched {attr}')
+            return super().__getattribute__(attr)
+
         @property
         def value(self):
             """value getter"""
             print('called value getter')
             return self._value
 
         @value.setter
@@ -72,14 +77,18 @@
         print(f'from remote {b} {args=}')
         return a, c
 
     def get_region(self):
         """keyword which return a region"""
         return Region(1, 2, 3, 4)
 
+    def get_dictionary(self):
+        """keyword which return a region"""
+        return {"first": 1, "second": 2}
+
     def raise_error(self):
         """keyword which raises an error"""
         raise RuntimeError('error')
 
     def get_question(self):
         """keyword which returns a string"""
         return "what is the airspeed velocity of an unladen swallow?"
```

### Comparing `robotframework_rpycremote-0.0.2/test/server.py` & `robotframework_rpycremote-0.0.3/test/server.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import sys
 import logging
 import logging.config
 import yaml
 from provider import Provider
 import RPyCRobotRemote
 
-
 LOGCONFIG = """
 version: 1
 formatters:
   simple:
     format: '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
 handlers:
   console:
@@ -33,14 +32,15 @@
 logging.config.dictConfig(
     yaml.load(
         LOGCONFIG,
         Loader=yaml.SafeLoader
     ),
 )
 
+
 server = RPyCRobotRemote.Server(
     Provider(),
     serve=False,
     # port=0,
     port_file=sys.stdout,
     server=RPyCRobotRemote.SingleServer
 )
```

