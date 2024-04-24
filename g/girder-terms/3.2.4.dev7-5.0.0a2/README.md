# Comparing `tmp/girder-terms-3.2.4.dev7.tar.gz` & `tmp/girder-terms-5.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-terms-3.2.4.dev7.tar", last modified: Wed Apr 24 19:13:49 2024, max compression
+gzip compressed data, was "girder-terms-5.0.0a2.tar", last modified: Fri Apr 12 16:32:30 2024, max compression
```

## Comparing `girder-terms-3.2.4.dev7.tar` & `girder-terms-5.0.0a2.tar`

### file list

```diff
@@ -1,37 +1,23 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:49.658443 girder-terms-3.2.4.dev7/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      640 2024-04-24 19:13:49.658443 girder-terms-3.2.4.dev7/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:49.654443 girder-terms-3.2.4.dev7/girder_terms/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3384 2024-04-24 19:11:47.000000 girder-terms-3.2.4.dev7/girder_terms/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:49.658443 girder-terms-3.2.4.dev7/girder_terms/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-04-24 19:11:47.000000 girder-terms-3.2.4.dev7/girder_terms/web_client/main.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:49.658443 girder-terms-3.2.4.dev7/girder_terms/web_client/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3270 2024-04-24 19:11:47.000000 girder-terms-3.2.4.dev7/girder_terms/web_client/models/CollectionModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      655 2024-04-24 19:11:47.000000 girder-terms-3.2.4.dev7/girder_terms/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3087 2024-04-24 19:11:47.000000 girder-terms-3.2.4.dev7/girder_terms/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:49.658443 girder-terms-3.2.4.dev7/girder_terms/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      118 2024-04-24 19:11:47.000000 girder-terms-3.2.4.dev7/girder_terms/web_client/stylesheets/collectionInfoWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)       67 2024-04-24 19:11:47.000000 girder-terms-3.2.4.dev7/girder_terms/web_client/stylesheets/editCollectionTermsWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2024-04-24 19:11:47.000000 girder-terms-3.2.4.dev7/girder_terms/web_client/stylesheets/termsAcceptance.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:49.658443 girder-terms-3.2.4.dev7/girder_terms/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2024-04-24 19:11:47.000000 girder-terms-3.2.4.dev7/girder_terms/web_client/templates/collectionInfoWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      291 2024-04-24 19:11:47.000000 girder-terms-3.2.4.dev7/girder_terms/web_client/templates/editCollectionTermsWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      266 2024-04-24 19:11:47.000000 girder-terms-3.2.4.dev7/girder_terms/web_client/templates/termsAcceptance.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:49.658443 girder-terms-3.2.4.dev7/girder_terms/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      717 2024-04-24 19:11:47.000000 girder-terms-3.2.4.dev7/girder_terms/web_client/views/CollectionInfoWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2413 2024-04-24 19:11:47.000000 girder-terms-3.2.4.dev7/girder_terms/web_client/views/EditCollectionWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1495 2024-04-24 19:11:47.000000 girder-terms-3.2.4.dev7/girder_terms/web_client/views/TermsAcceptanceView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:49.658443 girder-terms-3.2.4.dev7/girder_terms.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      640 2024-04-24 19:13:49.000000 girder-terms-3.2.4.dev7/girder_terms.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1054 2024-04-24 19:13:49.000000 girder-terms-3.2.4.dev7/girder_terms.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:13:49.000000 girder-terms-3.2.4.dev7/girder_terms.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2024-04-24 19:13:49.000000 girder-terms-3.2.4.dev7/girder_terms.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:13:49.000000 girder-terms-3.2.4.dev7/girder_terms.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-04-24 19:13:49.000000 girder-terms-3.2.4.dev7/girder_terms.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-24 19:13:49.000000 girder-terms-3.2.4.dev7/girder_terms.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2024-04-24 19:11:47.000000 girder-terms-3.2.4.dev7/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:49.658443 girder-terms-3.2.4.dev7/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:11:47.000000 girder-terms-3.2.4.dev7/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14763 2024-04-24 19:11:47.000000 girder-terms-3.2.4.dev7/plugin_tests/termsSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6081 2024-04-24 19:11:47.000000 girder-terms-3.2.4.dev7/plugin_tests/terms_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-24 19:13:49.658443 girder-terms-3.2.4.dev7/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1704 2024-04-24 19:11:47.000000 girder-terms-3.2.4.dev7/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:32:30.953370 girder-terms-5.0.0a2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      142 2024-04-12 16:27:18.000000 girder-terms-5.0.0a2/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      637 2024-04-12 16:32:30.953370 girder-terms-5.0.0a2/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:32:30.949370 girder-terms-5.0.0a2/girder_terms/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3663 2024-04-12 16:27:18.000000 girder-terms-5.0.0a2/girder_terms/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:32:30.949370 girder-terms-5.0.0a2/girder_terms/web_client/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:32:30.953370 girder-terms-5.0.0a2/girder_terms/web_client/dist/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10746 2024-04-12 16:28:48.000000 girder-terms-5.0.0a2/girder_terms/web_client/dist/girder-plugin-terms.umd.cjs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2024-04-12 16:28:48.000000 girder-terms-5.0.0a2/girder_terms/web_client/dist/style.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:32:30.953370 girder-terms-5.0.0a2/girder_terms.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      637 2024-04-12 16:32:30.000000 girder-terms-5.0.0a2/girder_terms.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      459 2024-04-12 16:32:30.000000 girder-terms-5.0.0a2/girder_terms.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:32:30.000000 girder-terms-5.0.0a2/girder_terms.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2024-04-12 16:32:30.000000 girder-terms-5.0.0a2/girder_terms.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:32:30.000000 girder-terms-5.0.0a2/girder_terms.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-04-12 16:32:30.000000 girder-terms-5.0.0a2/girder_terms.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-12 16:32:30.000000 girder-terms-5.0.0a2/girder_terms.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2024-04-12 16:27:18.000000 girder-terms-5.0.0a2/plugin.cmake
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:32:30.953370 girder-terms-5.0.0a2/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:27:18.000000 girder-terms-5.0.0a2/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6081 2024-04-12 16:27:18.000000 girder-terms-5.0.0a2/plugin_tests/terms_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-12 16:32:30.953370 girder-terms-5.0.0a2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1704 2024-04-12 16:27:18.000000 girder-terms-5.0.0a2/setup.py
```

### Comparing `girder-terms-3.2.4.dev7/PKG-INFO` & `girder-terms-5.0.0a2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-terms
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Allows Girder collections to require users to accept terms of use before browsing.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#terms-of-use
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `girder-terms-3.2.4.dev7/girder_terms/__init__.py` & `girder-terms-5.0.0a2/girder_terms/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import datetime
 import hashlib
+from pathlib import Path
 
 from girder import events
 from girder.api import access
 from girder.api.describe import Description, autoDescribeRoute
 from girder.api.rest import boundHandler
 from girder.api.v1.collection import Collection
 from girder.constants import AccessType, TokenScope
 from girder.exceptions import RestException
 from girder.models.collection import Collection as CollectionModel
 from girder.models.user import User
-from girder.plugin import GirderPlugin
+from girder.plugin import GirderPlugin, registerPluginStaticContent
 
 
 @access.user(scope=TokenScope.DATA_READ)
 @boundHandler
 @autoDescribeRoute(
     Description("Accept a collection's Terms of Use for the current user.")
     .modelParam('id', model=CollectionModel, level=AccessType.READ)
@@ -59,15 +60,14 @@
 
         collectionResponse['terms'] = terms
         event.addResponse(collectionResponse)
 
 
 class TermsPlugin(GirderPlugin):
     DISPLAY_NAME = 'Terms of Use'
-    CLIENT_SOURCE_PATH = 'web_client'
 
     def load(self, info):
         # Augment the collection creation and edit routes to accept a terms field
         events.bind('rest.post.collection.after', 'terms', afterPostPutCollection)
         events.bind('rest.put.collection/:id.after', 'terms', afterPostPutCollection)
         for handler in [
             Collection.createCollection,
@@ -80,7 +80,15 @@
         CollectionModel().exposeFields(level=AccessType.READ, fields={'terms'})
 
         # Add endpoint for registered users to accept terms
         info['apiRoot'].collection.route('POST', (':id', 'acceptTerms'), acceptCollectionTerms)
 
         # Expose the terms field on all users
         User().exposeFields(level=AccessType.ADMIN, fields={'terms'})
+
+        registerPluginStaticContent(
+            plugin='terms',
+            css=['/style.css'],
+            js=['/girder-plugin-terms.umd.cjs'],
+            staticDir=Path(__file__).parent / 'web_client' / 'dist',
+            tree=info['serverRoot'],
+        )
```

### Comparing `girder-terms-3.2.4.dev7/girder_terms.egg-info/PKG-INFO` & `girder-terms-5.0.0a2/girder_terms.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-terms
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Allows Girder collections to require users to accept terms of use before browsing.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#terms-of-use
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `girder-terms-3.2.4.dev7/plugin_tests/terms_test.py` & `girder-terms-5.0.0a2/plugin_tests/terms_test.py`

 * *Files identical despite different names*

### Comparing `girder-terms-3.2.4.dev7/setup.py` & `girder-terms-5.0.0a2/setup.py`

 * *Files identical despite different names*

