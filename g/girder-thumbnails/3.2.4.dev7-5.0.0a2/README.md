# Comparing `tmp/girder-thumbnails-3.2.4.dev7.tar.gz` & `tmp/girder_thumbnails-5a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-thumbnails-3.2.4.dev7.tar", last modified: Wed Apr 24 19:13:53 2024, max compression
+gzip compressed data, was "girder_thumbnails-5a2.tar", last modified: Fri Apr 12 16:32:45 2024, max compression
```

## Comparing `girder-thumbnails-3.2.4.dev7.tar` & `girder_thumbnails-5a2.tar`

### file list

```diff
@@ -1,43 +1,28 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:53.014438 girder-thumbnails-3.2.4.dev7/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      617 2024-04-24 19:13:53.014438 girder-thumbnails-3.2.4.dev7/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:53.010439 girder-thumbnails-3.2.4.dev7/girder_thumbnails/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3080 2024-04-24 19:11:47.000000 girder-thumbnails-3.2.4.dev7/girder_thumbnails/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2346 2024-04-24 19:11:47.000000 girder-thumbnails-3.2.4.dev7/girder_thumbnails/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      664 2024-04-24 19:11:47.000000 girder-thumbnails-3.2.4.dev7/girder_thumbnails/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:53.010439 girder-thumbnails-3.2.4.dev7/girder_thumbnails/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2024-04-24 19:11:47.000000 girder-thumbnails-3.2.4.dev7/girder_thumbnails/web_client/main.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:53.010439 girder-thumbnails-3.2.4.dev7/girder_thumbnails/web_client/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      150 2024-04-24 19:11:47.000000 girder-thumbnails-3.2.4.dev7/girder_thumbnails/web_client/models/ThumbnailModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      537 2024-04-24 19:11:47.000000 girder-thumbnails-3.2.4.dev7/girder_thumbnails/web_client/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:53.010439 girder-thumbnails-3.2.4.dev7/girder_thumbnails/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      496 2024-04-24 19:11:47.000000 girder-thumbnails-3.2.4.dev7/girder_thumbnails/web_client/stylesheets/createThumbnailView.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2024-04-24 19:11:47.000000 girder-thumbnails-3.2.4.dev7/girder_thumbnails/web_client/stylesheets/flowView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:53.014438 girder-thumbnails-3.2.4.dev7/girder_thumbnails/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1510 2024-04-24 19:11:47.000000 girder-thumbnails-3.2.4.dev7/girder_thumbnails/web_client/templates/createThumbnailViewDialog.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)       56 2024-04-24 19:11:47.000000 girder-thumbnails-3.2.4.dev7/girder_thumbnails/web_client/templates/createThumbnailViewTargetDescription.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2024-04-24 19:11:47.000000 girder-thumbnails-3.2.4.dev7/girder_thumbnails/web_client/templates/fileListWidgetCreateButton.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      314 2024-04-24 19:11:47.000000 girder-thumbnails-3.2.4.dev7/girder_thumbnails/web_client/templates/flowView.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2024-04-24 19:11:47.000000 girder-thumbnails-3.2.4.dev7/girder_thumbnails/web_client/templates/itemView.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:53.014438 girder-thumbnails-3.2.4.dev7/girder_thumbnails/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3910 2024-04-24 19:11:47.000000 girder-thumbnails-3.2.4.dev7/girder_thumbnails/web_client/views/CreateThumbnailView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1306 2024-04-24 19:11:47.000000 girder-thumbnails-3.2.4.dev7/girder_thumbnails/web_client/views/FileListWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2021 2024-04-24 19:11:47.000000 girder-thumbnails-3.2.4.dev7/girder_thumbnails/web_client/views/FlowView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1171 2024-04-24 19:11:47.000000 girder-thumbnails-3.2.4.dev7/girder_thumbnails/web_client/views/ItemView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6324 2024-04-24 19:11:47.000000 girder-thumbnails-3.2.4.dev7/girder_thumbnails/worker.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:53.014438 girder-thumbnails-3.2.4.dev7/girder_thumbnails.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      617 2024-04-24 19:13:52.000000 girder-thumbnails-3.2.4.dev7/girder_thumbnails.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1324 2024-04-24 19:13:52.000000 girder-thumbnails-3.2.4.dev7/girder_thumbnails.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:13:52.000000 girder-thumbnails-3.2.4.dev7/girder_thumbnails.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       64 2024-04-24 19:13:52.000000 girder-thumbnails-3.2.4.dev7/girder_thumbnails.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:13:52.000000 girder-thumbnails-3.2.4.dev7/girder_thumbnails.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2024-04-24 19:13:52.000000 girder-thumbnails-3.2.4.dev7/girder_thumbnails.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2024-04-24 19:13:52.000000 girder-thumbnails-3.2.4.dev7/girder_thumbnails.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       55 2024-04-24 19:11:47.000000 girder-thumbnails-3.2.4.dev7/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:53.014438 girder-thumbnails-3.2.4.dev7/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:11:47.000000 girder-thumbnails-3.2.4.dev7/plugin_tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:53.014438 girder-thumbnails-3.2.4.dev7/plugin_tests/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    35946 2024-04-24 19:11:47.000000 girder-thumbnails-3.2.4.dev7/plugin_tests/data/sample_dicom.dcm
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13000 2024-04-24 19:11:47.000000 girder-thumbnails-3.2.4.dev7/plugin_tests/thumbnail_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2213 2024-04-24 19:11:47.000000 girder-thumbnails-3.2.4.dev7/plugin_tests/thumbnailsSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-24 19:13:53.014438 girder-thumbnails-3.2.4.dev7/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1687 2024-04-24 19:11:47.000000 girder-thumbnails-3.2.4.dev7/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:32:45.289472 girder_thumbnails-5a2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      162 2024-04-12 16:27:18.000000 girder_thumbnails-5a2/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      614 2024-04-12 16:32:45.289472 girder_thumbnails-5a2/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:32:45.289472 girder_thumbnails-5a2/girder_thumbnails/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3370 2024-04-12 16:27:18.000000 girder_thumbnails-5a2/girder_thumbnails/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2346 2024-04-12 16:27:18.000000 girder_thumbnails-5a2/girder_thumbnails/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      664 2024-04-12 16:27:18.000000 girder_thumbnails-5a2/girder_thumbnails/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:32:45.285472 girder_thumbnails-5a2/girder_thumbnails/web_client/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:32:45.289472 girder_thumbnails-5a2/girder_thumbnails/web_client/dist/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21094 2024-04-12 16:28:51.000000 girder_thumbnails-5a2/girder_thumbnails/web_client/dist/girder-plugin-thumbnails.umd.cjs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      992 2024-04-12 16:28:51.000000 girder_thumbnails-5a2/girder_thumbnails/web_client/dist/style.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6324 2024-04-12 16:27:18.000000 girder_thumbnails-5a2/girder_thumbnails/worker.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:32:45.289472 girder_thumbnails-5a2/girder_thumbnails.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      614 2024-04-12 16:32:45.000000 girder_thumbnails-5a2/girder_thumbnails.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      634 2024-04-12 16:32:45.000000 girder_thumbnails-5a2/girder_thumbnails.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:32:45.000000 girder_thumbnails-5a2/girder_thumbnails.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       64 2024-04-12 16:32:45.000000 girder_thumbnails-5a2/girder_thumbnails.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:32:45.000000 girder_thumbnails-5a2/girder_thumbnails.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2024-04-12 16:32:45.000000 girder_thumbnails-5a2/girder_thumbnails.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2024-04-12 16:32:45.000000 girder_thumbnails-5a2/girder_thumbnails.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       55 2024-04-12 16:27:18.000000 girder_thumbnails-5a2/plugin.cmake
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:32:45.289472 girder_thumbnails-5a2/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:27:18.000000 girder_thumbnails-5a2/plugin_tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:32:45.289472 girder_thumbnails-5a2/plugin_tests/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    35946 2024-04-12 16:27:18.000000 girder_thumbnails-5a2/plugin_tests/data/sample_dicom.dcm
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12986 2024-04-12 16:27:18.000000 girder_thumbnails-5a2/plugin_tests/thumbnail_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-12 16:32:45.289472 girder_thumbnails-5a2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1687 2024-04-12 16:27:18.000000 girder_thumbnails-5a2/setup.py
```

### Comparing `girder-thumbnails-3.2.4.dev7/PKG-INFO` & `girder_thumbnails-5a2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-thumbnails
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Generate thumbnails from files.
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-thumbnails-3.2.4.dev7/girder_thumbnails/__init__.py` & `girder_thumbnails-5a2/girder_thumbnails/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import json
+from pathlib import Path
+
 from girder import events
 from girder.constants import AccessType
 from girder.models.collection import Collection
 from girder.models.file import File
 from girder.models.folder import Folder
 from girder.models.item import Item
 from girder.models.user import User
-from girder.plugin import getPlugin, GirderPlugin
+from girder.plugin import getPlugin, GirderPlugin, registerPluginStaticContent
 from girder.utility.model_importer import ModelImporter
 from . import rest, utils
 
 
 def removeThumbnails(event):
     """
     When a resource containing thumbnails is about to be deleted, we delete
@@ -81,21 +83,28 @@
     utils.scheduleThumbnailJob(
         file=file, attachToType='item', attachToId=item['_id'], user=event.info['currentUser'],
         width=width, height=height, crop=crop)
 
 
 class ThumbnailsPlugin(GirderPlugin):
     DISPLAY_NAME = 'Thumbnails'
-    CLIENT_SOURCE_PATH = 'web_client'
 
     def load(self, info):
         getPlugin('jobs').load(info)
 
         name = 'thumbnails'
         info['apiRoot'].thumbnail = rest.Thumbnail()
 
         for model in (Item(), Collection(), Folder(), User()):
             model.exposeFields(level=AccessType.READ, fields='_thumbnails')
             events.bind('model.%s.remove' % model.name, name, removeThumbnails)
 
         events.bind('model.file.remove', name, removeThumbnailLink)
         events.bind('data.process', name, _onUpload)
+
+        registerPluginStaticContent(
+            plugin='thumbnails',
+            css=['/style.css'],
+            js=['/girder-plugin-thumbnails.umd.cjs'],
+            staticDir=Path(__file__).parent / 'web_client' / 'dist',
+            tree=info['serverRoot'],
+        )
```

### Comparing `girder-thumbnails-3.2.4.dev7/girder_thumbnails/rest.py` & `girder_thumbnails-5a2/girder_thumbnails/rest.py`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.2.4.dev7/girder_thumbnails/utils.py` & `girder_thumbnails-5a2/girder_thumbnails/utils.py`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.2.4.dev7/girder_thumbnails/worker.py` & `girder_thumbnails-5a2/girder_thumbnails/worker.py`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.2.4.dev7/girder_thumbnails.egg-info/PKG-INFO` & `girder_thumbnails-5a2/girder_thumbnails.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-thumbnails
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Generate thumbnails from files.
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-thumbnails-3.2.4.dev7/plugin_tests/data/sample_dicom.dcm` & `girder_thumbnails-5a2/plugin_tests/data/sample_dicom.dcm`

 * *Files identical despite different names*

### Comparing `girder-thumbnails-3.2.4.dev7/plugin_tests/thumbnail_test.py` & `girder_thumbnails-5a2/plugin_tests/thumbnail_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         folders = Folder().childFolders(parent=self.admin, parentType='user', user=self.admin)
         for folder in folders:
             if folder['public'] is True:
                 self.publicFolder = folder
             else:
                 self.privateFolder = folder
 
-        path = os.path.join(ROOT_DIR, 'girder', 'web_client', 'src', 'assets', 'Girder_Mark.png')
+        path = os.path.join(ROOT_DIR, 'girder', 'web', 'public', 'Girder_Mark.png')
         with open(path, 'rb') as file:
             self.image = file.read()
         events.unbind('thumbnails.create', 'test')
 
     def testThumbnailCreation(self):
         # Upload the Girder logo to the admin's public folder
         resp = self.request(
```

### Comparing `girder-thumbnails-3.2.4.dev7/setup.py` & `girder_thumbnails-5a2/setup.py`

 * *Files identical despite different names*

