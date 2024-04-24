# Comparing `tmp/girder-gravatar-3.2.4.dev7.tar.gz` & `tmp/girder-gravatar-5.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-gravatar-3.2.4.dev7.tar", last modified: Wed Apr 24 19:12:45 2024, max compression
+gzip compressed data, was "girder-gravatar-5.0.0a2.tar", last modified: Fri Apr 12 16:30:27 2024, max compression
```

## Comparing `girder-gravatar-3.2.4.dev7.tar` & `girder-gravatar-5.0.0a2.tar`

### file list

```diff
@@ -1,29 +1,23 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:45.118527 girder-gravatar-3.2.4.dev7/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      609 2024-04-24 19:12:45.118527 girder-gravatar-3.2.4.dev7/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:45.114527 girder-gravatar-3.2.4.dev7/girder_gravatar/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1922 2024-04-24 19:11:47.000000 girder-gravatar-3.2.4.dev7/girder_gravatar/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-04-24 19:11:47.000000 girder-gravatar-3.2.4.dev7/girder_gravatar/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:45.118527 girder-gravatar-3.2.4.dev7/girder_gravatar/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       78 2024-04-24 19:11:47.000000 girder-gravatar-3.2.4.dev7/girder_gravatar/web_client/main.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:45.118527 girder-gravatar-3.2.4.dev7/girder_gravatar/web_client/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      367 2024-04-24 19:11:47.000000 girder-gravatar-3.2.4.dev7/girder_gravatar/web_client/models/UserModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      558 2024-04-24 19:11:47.000000 girder-gravatar-3.2.4.dev7/girder_gravatar/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      422 2024-04-24 19:11:47.000000 girder-gravatar-3.2.4.dev7/girder_gravatar/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:45.118527 girder-gravatar-3.2.4.dev7/girder_gravatar/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      554 2024-04-24 19:11:47.000000 girder-gravatar-3.2.4.dev7/girder_gravatar/web_client/templates/configView.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:45.118527 girder-gravatar-3.2.4.dev7/girder_gravatar/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2103 2024-04-24 19:11:47.000000 girder-gravatar-3.2.4.dev7/girder_gravatar/web_client/views/ConfigView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:45.118527 girder-gravatar-3.2.4.dev7/girder_gravatar.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      609 2024-04-24 19:12:44.000000 girder-gravatar-3.2.4.dev7/girder_gravatar.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      664 2024-04-24 19:12:45.000000 girder-gravatar-3.2.4.dev7/girder_gravatar.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:12:44.000000 girder-gravatar-3.2.4.dev7/girder_gravatar.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2024-04-24 19:12:44.000000 girder-gravatar-3.2.4.dev7/girder_gravatar.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:12:44.000000 girder-gravatar-3.2.4.dev7/girder_gravatar.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-04-24 19:12:44.000000 girder-gravatar-3.2.4.dev7/girder_gravatar.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-04-24 19:12:44.000000 girder-gravatar-3.2.4.dev7/girder_gravatar.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2024-04-24 19:11:47.000000 girder-gravatar-3.2.4.dev7/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:45.118527 girder-gravatar-3.2.4.dev7/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:11:47.000000 girder-gravatar-3.2.4.dev7/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3106 2024-04-24 19:11:47.000000 girder-gravatar-3.2.4.dev7/plugin_tests/gravatar_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-24 19:12:45.118527 girder-gravatar-3.2.4.dev7/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1675 2024-04-24 19:11:47.000000 girder-gravatar-3.2.4.dev7/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:30:27.372477 girder-gravatar-5.0.0a2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      104 2024-04-12 16:27:18.000000 girder-gravatar-5.0.0a2/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      606 2024-04-12 16:30:27.372477 girder-gravatar-5.0.0a2/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:30:27.372477 girder-gravatar-5.0.0a2/girder_gravatar/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2196 2024-04-12 16:27:18.000000 girder-gravatar-5.0.0a2/girder_gravatar/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-04-12 16:27:18.000000 girder-gravatar-5.0.0a2/girder_gravatar/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:30:27.372477 girder-gravatar-5.0.0a2/girder_gravatar/web_client/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:30:27.372477 girder-gravatar-5.0.0a2/girder_gravatar/web_client/dist/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4199 2024-04-12 16:28:13.000000 girder-gravatar-5.0.0a2/girder_gravatar/web_client/dist/girder-plugin-gravatar.umd.cjs
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:30:27.372477 girder-gravatar-5.0.0a2/girder_gravatar.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      606 2024-04-12 16:30:27.000000 girder-gravatar-5.0.0a2/girder_gravatar.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      481 2024-04-12 16:30:27.000000 girder-gravatar-5.0.0a2/girder_gravatar.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:30:27.000000 girder-gravatar-5.0.0a2/girder_gravatar.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2024-04-12 16:30:27.000000 girder-gravatar-5.0.0a2/girder_gravatar.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:30:27.000000 girder-gravatar-5.0.0a2/girder_gravatar.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-04-12 16:30:27.000000 girder-gravatar-5.0.0a2/girder_gravatar.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-04-12 16:30:27.000000 girder-gravatar-5.0.0a2/girder_gravatar.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2024-04-12 16:27:18.000000 girder-gravatar-5.0.0a2/plugin.cmake
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:30:27.372477 girder-gravatar-5.0.0a2/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:27:18.000000 girder-gravatar-5.0.0a2/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3106 2024-04-12 16:27:18.000000 girder-gravatar-5.0.0a2/plugin_tests/gravatar_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-12 16:30:27.372477 girder-gravatar-5.0.0a2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1675 2024-04-12 16:27:18.000000 girder-gravatar-5.0.0a2/setup.py
```

### Comparing `girder-gravatar-3.2.4.dev7/PKG-INFO` & `girder-gravatar-5.0.0a2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-gravatar
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Adds Gravatar URLs for users.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#gravatar-portraits
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `girder-gravatar-3.2.4.dev7/girder_gravatar/__init__.py` & `girder-gravatar-5.0.0a2/girder_gravatar/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-import cherrypy
 import hashlib
+from pathlib import Path
+
+import cherrypy
 
 from girder import events
 from girder.api import access
 from girder.api.describe import Description, autoDescribeRoute
 from girder.models.model_base import AccessType
 from girder.models.setting import Setting
 from girder.models.user import User
-from girder.plugin import GirderPlugin
+from girder.plugin import GirderPlugin, registerPluginStaticContent
 
 from .settings import PluginSettings
 
 
 def computeBaseUrl(user):
     """
     Compute the base gravatar URL for a user and return it. For the moment, the
@@ -45,15 +47,22 @@
     gravatar URL.
     """
     event.info['gravatar_baseUrl'] = computeBaseUrl(event.info)
 
 
 class GravatarPlugin(GirderPlugin):
     DISPLAY_NAME = 'Gravatar Portraits'
-    CLIENT_SOURCE_PATH = 'web_client'
 
     def load(self, info):
         info['apiRoot'].user.route('GET', (':id', 'gravatar'), getGravatar)
 
         User().exposeFields(level=AccessType.READ, fields='gravatar_baseUrl')
 
         events.bind('model.user.save', 'gravatar', _userUpdate)
+
+        registerPluginStaticContent(
+            plugin='gravatar',
+            css=[],
+            js=['/girder-plugin-gravatar.umd.cjs'],
+            staticDir=Path(__file__).parent / 'web_client' / 'dist',
+            tree=info['serverRoot'],
+        )
```

### Comparing `girder-gravatar-3.2.4.dev7/girder_gravatar.egg-info/PKG-INFO` & `girder-gravatar-5.0.0a2/girder_gravatar.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-gravatar
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Adds Gravatar URLs for users.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#gravatar-portraits
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `girder-gravatar-3.2.4.dev7/plugin_tests/gravatar_test.py` & `girder-gravatar-5.0.0a2/plugin_tests/gravatar_test.py`

 * *Files identical despite different names*

### Comparing `girder-gravatar-3.2.4.dev7/setup.py` & `girder-gravatar-5.0.0a2/setup.py`

 * *Files identical despite different names*

