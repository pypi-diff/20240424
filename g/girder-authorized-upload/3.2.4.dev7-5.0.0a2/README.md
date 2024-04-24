# Comparing `tmp/girder-authorized-upload-3.2.4.dev7.tar.gz` & `tmp/girder-authorized-upload-5.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-authorized-upload-3.2.4.dev7.tar", last modified: Wed Apr 24 19:12:09 2024, max compression
+gzip compressed data, was "girder-authorized-upload-5.0.0a2.tar", last modified: Fri Apr 12 16:29:32 2024, max compression
```

## Comparing `girder-authorized-upload-3.2.4.dev7.tar` & `girder-authorized-upload-5.0.0a2.tar`

### file list

```diff
@@ -1,37 +1,27 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:09.482569 girder-authorized-upload-3.2.4.dev7/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      667 2024-04-24 19:12:09.482569 girder-authorized-upload-3.2.4.dev7/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:09.478569 girder-authorized-upload-3.2.4.dev7/girder_authorized_upload/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4605 2024-04-24 19:11:47.000000 girder-authorized-upload-3.2.4.dev7/girder_authorized_upload/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       52 2024-04-24 19:11:47.000000 girder-authorized-upload-3.2.4.dev7/girder_authorized_upload/constants.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:09.478569 girder-authorized-upload-3.2.4.dev7/girder_authorized_upload/mail_templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      281 2024-04-24 19:11:47.000000 girder-authorized-upload-3.2.4.dev7/girder_authorized_upload/mail_templates/authorized_upload.uploadFinished.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1712 2024-04-24 19:11:47.000000 girder-authorized-upload-3.2.4.dev7/girder_authorized_upload/rest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:09.478569 girder-authorized-upload-3.2.4.dev7/girder_authorized_upload/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      707 2024-04-24 19:11:47.000000 girder-authorized-upload-3.2.4.dev7/girder_authorized_upload/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      664 2024-04-24 19:11:47.000000 girder-authorized-upload-3.2.4.dev7/girder_authorized_upload/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      905 2024-04-24 19:11:47.000000 girder-authorized-upload-3.2.4.dev7/girder_authorized_upload/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:09.478569 girder-authorized-upload-3.2.4.dev7/girder_authorized_upload/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       35 2024-04-24 19:11:47.000000 girder-authorized-upload-3.2.4.dev7/girder_authorized_upload/web_client/stylesheets/authorizeUpload.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      966 2024-04-24 19:11:47.000000 girder-authorized-upload-3.2.4.dev7/girder_authorized_upload/web_client/stylesheets/authorizedUpload.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:09.478569 girder-authorized-upload-3.2.4.dev7/girder_authorized_upload/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      827 2024-04-24 19:11:47.000000 girder-authorized-upload-3.2.4.dev7/girder_authorized_upload/web_client/templates/authorizeUpload.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      766 2024-04-24 19:11:47.000000 girder-authorized-upload-3.2.4.dev7/girder_authorized_upload/web_client/templates/authorizedUpload.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      137 2024-04-24 19:11:47.000000 girder-authorized-upload-3.2.4.dev7/girder_authorized_upload/web_client/templates/folderActions.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:09.482569 girder-authorized-upload-3.2.4.dev7/girder_authorized_upload/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2024-04-24 19:11:47.000000 girder-authorized-upload-3.2.4.dev7/girder_authorized_upload/web_client/views/AuthorizeUploadView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1544 2024-04-24 19:11:47.000000 girder-authorized-upload-3.2.4.dev7/girder_authorized_upload/web_client/views/AuthorizedUploadView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:09.482569 girder-authorized-upload-3.2.4.dev7/girder_authorized_upload.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      667 2024-04-24 19:12:09.000000 girder-authorized-upload-3.2.4.dev7/girder_authorized_upload.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1240 2024-04-24 19:12:09.000000 girder-authorized-upload-3.2.4.dev7/girder_authorized_upload.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:12:09.000000 girder-authorized-upload-3.2.4.dev7/girder_authorized_upload.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       84 2024-04-24 19:12:09.000000 girder-authorized-upload-3.2.4.dev7/girder_authorized_upload.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:12:09.000000 girder-authorized-upload-3.2.4.dev7/girder_authorized_upload.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-04-24 19:12:09.000000 girder-authorized-upload-3.2.4.dev7/girder_authorized_upload.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2024-04-24 19:12:09.000000 girder-authorized-upload-3.2.4.dev7/girder_authorized_upload.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2024-04-24 19:11:47.000000 girder-authorized-upload-3.2.4.dev7/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:12:09.482569 girder-authorized-upload-3.2.4.dev7/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:11:47.000000 girder-authorized-upload-3.2.4.dev7/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3124 2024-04-24 19:11:47.000000 girder-authorized-upload-3.2.4.dev7/plugin_tests/authorizedUploadSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4600 2024-04-24 19:11:47.000000 girder-authorized-upload-3.2.4.dev7/plugin_tests/upload_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-24 19:12:09.482569 girder-authorized-upload-3.2.4.dev7/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1766 2024-04-24 19:11:47.000000 girder-authorized-upload-3.2.4.dev7/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:29:32.288034 girder-authorized-upload-5.0.0a2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2024-04-12 16:27:18.000000 girder-authorized-upload-5.0.0a2/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      664 2024-04-12 16:29:32.288034 girder-authorized-upload-5.0.0a2/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:29:32.284034 girder-authorized-upload-5.0.0a2/girder_authorized_upload/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4908 2024-04-12 16:27:18.000000 girder-authorized-upload-5.0.0a2/girder_authorized_upload/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       52 2024-04-12 16:27:18.000000 girder-authorized-upload-5.0.0a2/girder_authorized_upload/constants.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:29:32.284034 girder-authorized-upload-5.0.0a2/girder_authorized_upload/mail_templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      281 2024-04-12 16:27:18.000000 girder-authorized-upload-5.0.0a2/girder_authorized_upload/mail_templates/authorized_upload.uploadFinished.mako
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1712 2024-04-12 16:27:18.000000 girder-authorized-upload-5.0.0a2/girder_authorized_upload/rest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:29:32.284034 girder-authorized-upload-5.0.0a2/girder_authorized_upload/web_client/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:29:32.284034 girder-authorized-upload-5.0.0a2/girder_authorized_upload/web_client/dist/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15067 2024-04-12 16:28:05.000000 girder-authorized-upload-5.0.0a2/girder_authorized_upload/web_client/dist/girder-plugin-authorized-upload.umd.cjs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1300 2024-04-12 16:28:05.000000 girder-authorized-upload-5.0.0a2/girder_authorized_upload/web_client/dist/style.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:29:32.288034 girder-authorized-upload-5.0.0a2/girder_authorized_upload.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      664 2024-04-12 16:29:32.000000 girder-authorized-upload-5.0.0a2/girder_authorized_upload.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      741 2024-04-12 16:29:32.000000 girder-authorized-upload-5.0.0a2/girder_authorized_upload.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:29:32.000000 girder-authorized-upload-5.0.0a2/girder_authorized_upload.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       84 2024-04-12 16:29:32.000000 girder-authorized-upload-5.0.0a2/girder_authorized_upload.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:29:32.000000 girder-authorized-upload-5.0.0a2/girder_authorized_upload.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-04-12 16:29:32.000000 girder-authorized-upload-5.0.0a2/girder_authorized_upload.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2024-04-12 16:29:32.000000 girder-authorized-upload-5.0.0a2/girder_authorized_upload.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2024-04-12 16:27:18.000000 girder-authorized-upload-5.0.0a2/plugin.cmake
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:29:32.288034 girder-authorized-upload-5.0.0a2/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:27:18.000000 girder-authorized-upload-5.0.0a2/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4600 2024-04-12 16:27:18.000000 girder-authorized-upload-5.0.0a2/plugin_tests/upload_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-12 16:29:32.288034 girder-authorized-upload-5.0.0a2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1766 2024-04-12 16:27:18.000000 girder-authorized-upload-5.0.0a2/setup.py
```

### Comparing `girder-authorized-upload-3.2.4.dev7/PKG-INFO` & `girder-authorized-upload-5.0.0a2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-authorized-upload
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Allows registered users to authorize file uploads on their behalf via a secure one-use URL.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#authorized-uploads
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `girder-authorized-upload-3.2.4.dev7/girder_authorized_upload/__init__.py` & `girder-authorized-upload-5.0.0a2/girder_authorized_upload/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import os
+from pathlib import Path
 
 from bson.objectid import ObjectId
 from bson.errors import InvalidId
 from girder import events
 from girder.api import access
 from girder.api.rest import getCurrentToken, setCurrentUser
 from girder.models.item import Item
 from girder.models.token import Token
 from girder.models.user import User
-from girder.plugin import GirderPlugin
+from girder.plugin import GirderPlugin, registerPluginStaticContent
 from girder.utility import mail_utils
 
 from .constants import TOKEN_SCOPE_AUTHORIZED_UPLOAD
 from .rest import AuthorizedUpload
 
 _HERE = os.path.abspath(os.path.dirname(__file__))
 
@@ -99,22 +100,29 @@
         })
         mail_utils.sendMail('Authorized upload complete', text, [user['email']])
         Token().remove(token)
 
 
 class AuthorizedUploadPlugin(GirderPlugin):
     DISPLAY_NAME = 'Authorized Uploads'
-    CLIENT_SOURCE_PATH = 'web_client'
 
     def load(self, info):
         name = 'authorized_upload'
 
         mail_utils.addTemplateDirectory(os.path.join(_HERE, 'mail_templates'))
 
         events.bind('rest.post.file.before', name, _authorizeInitUpload)
         events.bind('rest.post.file.after', name, _storeUploadId)
         events.bind('rest.post.file/chunk.before', name, _authorizeUploadStep)
         events.bind('rest.post.file/completion.before', name, _authorizeUploadStep)
         events.bind('rest.get.file/offset.before', name, _authorizeUploadStep)
         events.bind('model.file.finalizeUpload.after', name, _uploadComplete)
 
         info['apiRoot'].authorized_upload = AuthorizedUpload()
+
+        registerPluginStaticContent(
+            plugin='authorized_upload',
+            css=['/style.css'],
+            js=['/girder-plugin-authorized-upload.umd.cjs'],
+            staticDir=Path(__file__).parent / 'web_client' / 'dist',
+            tree=info['serverRoot'],
+        )
```

### Comparing `girder-authorized-upload-3.2.4.dev7/girder_authorized_upload/rest.py` & `girder-authorized-upload-5.0.0a2/girder_authorized_upload/rest.py`

 * *Files identical despite different names*

### Comparing `girder-authorized-upload-3.2.4.dev7/girder_authorized_upload.egg-info/PKG-INFO` & `girder-authorized-upload-5.0.0a2/girder_authorized_upload.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-authorized-upload
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Allows registered users to authorize file uploads on their behalf via a secure one-use URL.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#authorized-uploads
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `girder-authorized-upload-3.2.4.dev7/girder_authorized_upload.egg-info/SOURCES.txt` & `girder-authorized-upload-5.0.0a2/girder_authorized_upload.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,18 @@
+MANIFEST.in
 plugin.cmake
 setup.py
 girder_authorized_upload/__init__.py
 girder_authorized_upload/constants.py
 girder_authorized_upload/rest.py
 girder_authorized_upload.egg-info/PKG-INFO
 girder_authorized_upload.egg-info/SOURCES.txt
 girder_authorized_upload.egg-info/dependency_links.txt
 girder_authorized_upload.egg-info/entry_points.txt
 girder_authorized_upload.egg-info/not-zip-safe
 girder_authorized_upload.egg-info/requires.txt
 girder_authorized_upload.egg-info/top_level.txt
 girder_authorized_upload/mail_templates/authorized_upload.uploadFinished.mako
-girder_authorized_upload/web_client/main.js
-girder_authorized_upload/web_client/package.json
-girder_authorized_upload/web_client/routes.js
-girder_authorized_upload/web_client/stylesheets/authorizeUpload.styl
-girder_authorized_upload/web_client/stylesheets/authorizedUpload.styl
-girder_authorized_upload/web_client/templates/authorizeUpload.pug
-girder_authorized_upload/web_client/templates/authorizedUpload.pug
-girder_authorized_upload/web_client/templates/folderActions.pug
-girder_authorized_upload/web_client/views/AuthorizeUploadView.js
-girder_authorized_upload/web_client/views/AuthorizedUploadView.js
+girder_authorized_upload/web_client/dist/girder-plugin-authorized-upload.umd.cjs
+girder_authorized_upload/web_client/dist/style.css
 plugin_tests/__init__.py
-plugin_tests/authorizedUploadSpec.js
 plugin_tests/upload_test.py
```

### Comparing `girder-authorized-upload-3.2.4.dev7/plugin_tests/upload_test.py` & `girder-authorized-upload-5.0.0a2/plugin_tests/upload_test.py`

 * *Files identical despite different names*

### Comparing `girder-authorized-upload-3.2.4.dev7/setup.py` & `girder-authorized-upload-5.0.0a2/setup.py`

 * *Files identical despite different names*

