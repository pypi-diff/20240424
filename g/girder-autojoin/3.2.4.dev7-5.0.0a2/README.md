# Comparing `tmp/girder-autojoin-3.2.4.dev7.tar.gz` & `tmp/girder-autojoin-5.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-autojoin-3.2.4.dev7.tar", last modified: Wed Apr 24 19:12:13 2024, max compression
+gzip compressed data, was "girder-autojoin-5.0.0a2.tar", last modified: Fri Apr 12 16:29:48 2024, max compression
```

## Comparing `girder-autojoin-3.2.4.dev7.tar` & `girder-autojoin-5.0.0a2.tar`

### file list

```diff
@@ -1,30 +1,24 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:13.214565 girder-autojoin-3.2.4.dev7/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2024-04-24 19:12:13.214565 girder-autojoin-3.2.4.dev7/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:13.214565 girder-autojoin-3.2.4.dev7/girder_autojoin/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      905 2024-04-24 19:11:47.000000 girder-autojoin-3.2.4.dev7/girder_autojoin/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2024-04-24 19:11:47.000000 girder-autojoin-3.2.4.dev7/girder_autojoin/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:13.214565 girder-autojoin-3.2.4.dev7/girder_autojoin/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2024-04-24 19:11:47.000000 girder-autojoin-3.2.4.dev7/girder_autojoin/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      588 2024-04-24 19:11:47.000000 girder-autojoin-3.2.4.dev7/girder_autojoin/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      422 2024-04-24 19:11:47.000000 girder-autojoin-3.2.4.dev7/girder_autojoin/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:13.214565 girder-autojoin-3.2.4.dev7/girder_autojoin/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       92 2024-04-24 19:11:47.000000 girder-autojoin-3.2.4.dev7/girder_autojoin/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:13.214565 girder-autojoin-3.2.4.dev7/girder_autojoin/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1805 2024-04-24 19:11:47.000000 girder-autojoin-3.2.4.dev7/girder_autojoin/web_client/templates/configView.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:13.214565 girder-autojoin-3.2.4.dev7/girder_autojoin/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3781 2024-04-24 19:11:47.000000 girder-autojoin-3.2.4.dev7/girder_autojoin/web_client/views/ConfigView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:13.214565 girder-autojoin-3.2.4.dev7/girder_autojoin.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      626 2024-04-24 19:12:13.000000 girder-autojoin-3.2.4.dev7/girder_autojoin.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      701 2024-04-24 19:12:13.000000 girder-autojoin-3.2.4.dev7/girder_autojoin.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:12:13.000000 girder-autojoin-3.2.4.dev7/girder_autojoin.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2024-04-24 19:12:13.000000 girder-autojoin-3.2.4.dev7/girder_autojoin.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:12:13.000000 girder-autojoin-3.2.4.dev7/girder_autojoin.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-04-24 19:12:13.000000 girder-autojoin-3.2.4.dev7/girder_autojoin.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-04-24 19:12:13.000000 girder-autojoin-3.2.4.dev7/girder_autojoin.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2024-04-24 19:11:47.000000 girder-autojoin-3.2.4.dev7/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:13.214565 girder-autojoin-3.2.4.dev7/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:11:47.000000 girder-autojoin-3.2.4.dev7/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3790 2024-04-24 19:11:47.000000 girder-autojoin-3.2.4.dev7/plugin_tests/autojoinSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2418 2024-04-24 19:11:47.000000 girder-autojoin-3.2.4.dev7/plugin_tests/autojoin_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-24 19:12:13.214565 girder-autojoin-3.2.4.dev7/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1692 2024-04-24 19:11:47.000000 girder-autojoin-3.2.4.dev7/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:29:48.408151 girder-autojoin-5.0.0a2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      154 2024-04-12 16:27:18.000000 girder-autojoin-5.0.0a2/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      623 2024-04-12 16:29:48.408151 girder-autojoin-5.0.0a2/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:29:48.404151 girder-autojoin-5.0.0a2/girder_autojoin/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1191 2024-04-12 16:27:18.000000 girder-autojoin-5.0.0a2/girder_autojoin/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2024-04-12 16:27:18.000000 girder-autojoin-5.0.0a2/girder_autojoin/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:29:48.404151 girder-autojoin-5.0.0a2/girder_autojoin/web_client/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:29:48.404151 girder-autojoin-5.0.0a2/girder_autojoin/web_client/dist/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16089 2024-04-12 16:28:08.000000 girder-autojoin-5.0.0a2/girder_autojoin/web_client/dist/girder-plugin-autojoin.umd.cjs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2024-04-12 16:28:08.000000 girder-autojoin-5.0.0a2/girder_autojoin/web_client/dist/style.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:29:48.408151 girder-autojoin-5.0.0a2/girder_autojoin.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      623 2024-04-12 16:29:48.000000 girder-autojoin-5.0.0a2/girder_autojoin.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      523 2024-04-12 16:29:48.000000 girder-autojoin-5.0.0a2/girder_autojoin.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:29:48.000000 girder-autojoin-5.0.0a2/girder_autojoin.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2024-04-12 16:29:48.000000 girder-autojoin-5.0.0a2/girder_autojoin.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:29:48.000000 girder-autojoin-5.0.0a2/girder_autojoin.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-04-12 16:29:48.000000 girder-autojoin-5.0.0a2/girder_autojoin.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-04-12 16:29:48.000000 girder-autojoin-5.0.0a2/girder_autojoin.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2024-04-12 16:27:18.000000 girder-autojoin-5.0.0a2/plugin.cmake
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:29:48.404151 girder-autojoin-5.0.0a2/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:27:18.000000 girder-autojoin-5.0.0a2/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2418 2024-04-12 16:27:18.000000 girder-autojoin-5.0.0a2/plugin_tests/autojoin_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-12 16:29:48.408151 girder-autojoin-5.0.0a2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1692 2024-04-12 16:27:18.000000 girder-autojoin-5.0.0a2/setup.py
```

### Comparing `girder-autojoin-3.2.4.dev7/PKG-INFO` & `girder-autojoin-5.0.0a2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-autojoin
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Automatically assign new users to groups based on their email domain
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#auto-join
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `girder-autojoin-3.2.4.dev7/girder_autojoin/__init__.py` & `girder-autojoin-5.0.0a2/girder_autojoin/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from pathlib import Path
+
 from girder import events
 from girder.models.group import Group
 from girder.models.setting import Setting
-from girder.plugin import GirderPlugin
+from girder.plugin import GirderPlugin, registerPluginStaticContent
 
 from .settings import PluginSettings
 
 
 def userCreated(event):
     """
     Check auto join rules when a new user is created. If a match is found,
@@ -20,11 +22,18 @@
         group = Group().load(rule['groupId'], force=True)
         if group:
             Group().addUser(group, user, rule['level'])
 
 
 class AutojoinPlugin(GirderPlugin):
     DISPLAY_NAME = 'Auto Join'
-    CLIENT_SOURCE_PATH = 'web_client'
 
     def load(self, info):
         events.bind('model.user.save.created', 'autojoin', userCreated)
+
+        registerPluginStaticContent(
+            plugin='autojoin',
+            css=['/style.css'],
+            js=['/girder-plugin-autojoin.umd.cjs'],
+            staticDir=Path(__file__).parent / 'web_client' / 'dist',
+            tree=info['serverRoot'],
+        )
```

### Comparing `girder-autojoin-3.2.4.dev7/girder_autojoin/settings.py` & `girder-autojoin-5.0.0a2/girder_autojoin/settings.py`

 * *Files identical despite different names*

### Comparing `girder-autojoin-3.2.4.dev7/girder_autojoin.egg-info/PKG-INFO` & `girder-autojoin-5.0.0a2/girder_autojoin.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-autojoin
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Automatically assign new users to groups based on their email domain
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#auto-join
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `girder-autojoin-3.2.4.dev7/plugin_tests/autojoin_test.py` & `girder-autojoin-5.0.0a2/plugin_tests/autojoin_test.py`

 * *Files identical despite different names*

### Comparing `girder-autojoin-3.2.4.dev7/setup.py` & `girder-autojoin-5.0.0a2/setup.py`

 * *Files identical despite different names*

