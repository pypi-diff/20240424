# Comparing `tmp/girder-oauth-3.2.4.dev7.tar.gz` & `tmp/girder-oauth-5.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-oauth-3.2.4.dev7.tar", last modified: Wed Apr 24 19:13:38 2024, max compression
+gzip compressed data, was "girder-oauth-5.0.0a2.tar", last modified: Fri Apr 12 16:31:39 2024, max compression
```

## Comparing `girder-oauth-3.2.4.dev7.tar` & `girder-oauth-5.0.0a2.tar`

### file list

```diff
@@ -1,45 +1,35 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:38.002459 girder-oauth-3.2.4.dev7/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      669 2024-04-24 19:13:38.002459 girder-oauth-3.2.4.dev7/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:37.994459 girder-oauth-3.2.4.dev7/girder_oauth/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1749 2024-04-24 19:11:47.000000 girder-oauth-3.2.4.dev7/girder_oauth/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:37.998459 girder-oauth-3.2.4.dev7/girder_oauth/providers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      480 2024-04-24 19:11:47.000000 girder-oauth-3.2.4.dev7/girder_oauth/providers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9083 2024-04-24 19:11:47.000000 girder-oauth-3.2.4.dev7/girder_oauth/providers/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3526 2024-04-24 19:11:47.000000 girder-oauth-3.2.4.dev7/girder_oauth/providers/bitbucket.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2503 2024-04-24 19:11:47.000000 girder-oauth-3.2.4.dev7/girder_oauth/providers/box.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3253 2024-04-24 19:11:47.000000 girder-oauth-3.2.4.dev7/girder_oauth/providers/github.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2746 2024-04-24 19:11:47.000000 girder-oauth-3.2.4.dev7/girder_oauth/providers/globus.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2980 2024-04-24 19:11:47.000000 girder-oauth-3.2.4.dev7/girder_oauth/providers/google.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2951 2024-04-24 19:11:47.000000 girder-oauth-3.2.4.dev7/girder_oauth/providers/linkedin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3018 2024-04-24 19:11:47.000000 girder-oauth-3.2.4.dev7/girder_oauth/providers/microsoft.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5347 2024-04-24 19:11:47.000000 girder-oauth-3.2.4.dev7/girder_oauth/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3127 2024-04-24 19:11:47.000000 girder-oauth-3.2.4.dev7/girder_oauth/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:37.998459 girder-oauth-3.2.4.dev7/girder_oauth/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      766 2024-04-24 19:11:47.000000 girder-oauth-3.2.4.dev7/girder_oauth/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      568 2024-04-24 19:11:47.000000 girder-oauth-3.2.4.dev7/girder_oauth/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      410 2024-04-24 19:11:47.000000 girder-oauth-3.2.4.dev7/girder_oauth/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:37.998459 girder-oauth-3.2.4.dev7/girder_oauth/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      458 2024-04-24 19:11:47.000000 girder-oauth-3.2.4.dev7/girder_oauth/web_client/stylesheets/configView.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2668 2024-04-24 19:11:47.000000 girder-oauth-3.2.4.dev7/girder_oauth/web_client/stylesheets/oauthLoginView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:37.998459 girder-oauth-3.2.4.dev7/girder_oauth/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2762 2024-04-24 19:11:47.000000 girder-oauth-3.2.4.dev7/girder_oauth/web_client/templates/configView.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      392 2024-04-24 19:11:47.000000 girder-oauth-3.2.4.dev7/girder_oauth/web_client/templates/oauthLoginView.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:38.002459 girder-oauth-3.2.4.dev7/girder_oauth/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8557 2024-04-24 19:11:47.000000 girder-oauth-3.2.4.dev7/girder_oauth/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      416 2024-04-24 19:11:47.000000 girder-oauth-3.2.4.dev7/girder_oauth/web_client/views/LoginView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2770 2024-04-24 19:11:47.000000 girder-oauth-3.2.4.dev7/girder_oauth/web_client/views/OAuthLoginView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      607 2024-04-24 19:11:47.000000 girder-oauth-3.2.4.dev7/girder_oauth/web_client/views/RegisterView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:38.002459 girder-oauth-3.2.4.dev7/girder_oauth.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      669 2024-04-24 19:13:37.000000 girder-oauth-3.2.4.dev7/girder_oauth.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1193 2024-04-24 19:13:37.000000 girder-oauth-3.2.4.dev7/girder_oauth.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:13:37.000000 girder-oauth-3.2.4.dev7/girder_oauth.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2024-04-24 19:13:37.000000 girder-oauth-3.2.4.dev7/girder_oauth.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:13:37.000000 girder-oauth-3.2.4.dev7/girder_oauth.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       27 2024-04-24 19:13:37.000000 girder-oauth-3.2.4.dev7/girder_oauth.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-24 19:13:37.000000 girder-oauth-3.2.4.dev7/girder_oauth.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2024-04-24 19:11:47.000000 girder-oauth-3.2.4.dev7/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:38.002459 girder-oauth-3.2.4.dev7/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:11:47.000000 girder-oauth-3.2.4.dev7/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    65626 2024-04-24 19:11:47.000000 girder-oauth-3.2.4.dev7/plugin_tests/oauth_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-24 19:13:38.002459 girder-oauth-3.2.4.dev7/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1733 2024-04-24 19:11:47.000000 girder-oauth-3.2.4.dev7/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:31:39.264999 girder-oauth-5.0.0a2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      142 2024-04-12 16:27:18.000000 girder-oauth-5.0.0a2/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      666 2024-04-12 16:31:39.264999 girder-oauth-5.0.0a2/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:31:39.260999 girder-oauth-5.0.0a2/girder_oauth/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2029 2024-04-12 16:27:18.000000 girder-oauth-5.0.0a2/girder_oauth/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:31:39.260999 girder-oauth-5.0.0a2/girder_oauth/providers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      480 2024-04-12 16:27:18.000000 girder-oauth-5.0.0a2/girder_oauth/providers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9083 2024-04-12 16:27:18.000000 girder-oauth-5.0.0a2/girder_oauth/providers/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3526 2024-04-12 16:27:18.000000 girder-oauth-5.0.0a2/girder_oauth/providers/bitbucket.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2503 2024-04-12 16:27:18.000000 girder-oauth-5.0.0a2/girder_oauth/providers/box.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3253 2024-04-12 16:27:18.000000 girder-oauth-5.0.0a2/girder_oauth/providers/github.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2746 2024-04-12 16:27:18.000000 girder-oauth-5.0.0a2/girder_oauth/providers/globus.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2980 2024-04-12 16:27:18.000000 girder-oauth-5.0.0a2/girder_oauth/providers/google.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2951 2024-04-12 16:27:18.000000 girder-oauth-5.0.0a2/girder_oauth/providers/linkedin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3018 2024-04-12 16:27:18.000000 girder-oauth-5.0.0a2/girder_oauth/providers/microsoft.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5347 2024-04-12 16:27:18.000000 girder-oauth-5.0.0a2/girder_oauth/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3127 2024-04-12 16:27:18.000000 girder-oauth-5.0.0a2/girder_oauth/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:31:39.260999 girder-oauth-5.0.0a2/girder_oauth/web_client/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:31:39.260999 girder-oauth-5.0.0a2/girder_oauth/web_client/dist/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    30187 2024-04-12 16:28:40.000000 girder-oauth-5.0.0a2/girder_oauth/web_client/dist/girder-plugin-oauth.umd.cjs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2550 2024-04-12 16:28:40.000000 girder-oauth-5.0.0a2/girder_oauth/web_client/dist/style.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:31:39.260999 girder-oauth-5.0.0a2/girder_oauth.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      666 2024-04-12 16:31:39.000000 girder-oauth-5.0.0a2/girder_oauth.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      807 2024-04-12 16:31:39.000000 girder-oauth-5.0.0a2/girder_oauth.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:31:39.000000 girder-oauth-5.0.0a2/girder_oauth.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2024-04-12 16:31:39.000000 girder-oauth-5.0.0a2/girder_oauth.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:31:39.000000 girder-oauth-5.0.0a2/girder_oauth.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       27 2024-04-12 16:31:39.000000 girder-oauth-5.0.0a2/girder_oauth.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-12 16:31:39.000000 girder-oauth-5.0.0a2/girder_oauth.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2024-04-12 16:27:18.000000 girder-oauth-5.0.0a2/plugin.cmake
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:31:39.260999 girder-oauth-5.0.0a2/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:27:18.000000 girder-oauth-5.0.0a2/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    65626 2024-04-12 16:27:18.000000 girder-oauth-5.0.0a2/plugin_tests/oauth_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-12 16:31:39.264999 girder-oauth-5.0.0a2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1733 2024-04-12 16:27:18.000000 girder-oauth-5.0.0a2/setup.py
```

### Comparing `girder-oauth-3.2.4.dev7/PKG-INFO` & `girder-oauth-5.0.0a2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-oauth
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Allow users to login via supported OAuth2 providers.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#oauth-login
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `girder-oauth-3.2.4.dev7/girder_oauth/__init__.py` & `girder-oauth-5.0.0a2/girder_oauth/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from pathlib import Path
+
 from girder import events
 from girder.constants import SortDir
 from girder.exceptions import ValidationException
 from girder.models.user import User
-from girder.plugin import GirderPlugin
+from girder.plugin import GirderPlugin, registerPluginStaticContent
 
 from . import rest, providers
 
 
 def checkOauthUser(event):
     """
     If an OAuth2 user without a password tries to log in with a password, we
@@ -35,17 +37,24 @@
 
         raise ValidationException(
             "You don't have a password. %s" % helpMessage)
 
 
 class OAuthPlugin(GirderPlugin):
     DISPLAY_NAME = 'OAuth2 Login'
-    CLIENT_SOURCE_PATH = 'web_client'
 
     def load(self, info):
         User().ensureIndex((
             (('oauth.provider', SortDir.ASCENDING),
              ('oauth.id', SortDir.ASCENDING)), {}))
 
         events.bind('no_password_login_attempt', 'oauth', checkOauthUser)
 
         info['apiRoot'].oauth = rest.OAuth()
+
+        registerPluginStaticContent(
+            plugin='oauth',
+            css=['/style.css'],
+            js=['/girder-plugin-oauth.umd.cjs'],
+            staticDir=Path(__file__).parent / 'web_client' / 'dist',
+            tree=info['serverRoot'],
+        )
```

### Comparing `girder-oauth-3.2.4.dev7/girder_oauth/providers/base.py` & `girder-oauth-5.0.0a2/girder_oauth/providers/base.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.4.dev7/girder_oauth/providers/bitbucket.py` & `girder-oauth-5.0.0a2/girder_oauth/providers/bitbucket.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.4.dev7/girder_oauth/providers/box.py` & `girder-oauth-5.0.0a2/girder_oauth/providers/box.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.4.dev7/girder_oauth/providers/github.py` & `girder-oauth-5.0.0a2/girder_oauth/providers/github.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.4.dev7/girder_oauth/providers/globus.py` & `girder-oauth-5.0.0a2/girder_oauth/providers/globus.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.4.dev7/girder_oauth/providers/google.py` & `girder-oauth-5.0.0a2/girder_oauth/providers/google.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.4.dev7/girder_oauth/providers/linkedin.py` & `girder-oauth-5.0.0a2/girder_oauth/providers/linkedin.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.4.dev7/girder_oauth/providers/microsoft.py` & `girder-oauth-5.0.0a2/girder_oauth/providers/microsoft.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.4.dev7/girder_oauth/rest.py` & `girder-oauth-5.0.0a2/girder_oauth/rest.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.4.dev7/girder_oauth/settings.py` & `girder-oauth-5.0.0a2/girder_oauth/settings.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.4.dev7/girder_oauth.egg-info/PKG-INFO` & `girder-oauth-5.0.0a2/girder_oauth.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-oauth
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Allow users to login via supported OAuth2 providers.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#oauth-login
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `girder-oauth-3.2.4.dev7/plugin_tests/oauth_test.py` & `girder-oauth-5.0.0a2/plugin_tests/oauth_test.py`

 * *Files identical despite different names*

### Comparing `girder-oauth-3.2.4.dev7/setup.py` & `girder-oauth-5.0.0a2/setup.py`

 * *Files identical despite different names*

