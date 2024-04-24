# Comparing `tmp/girder-hashsum-download-3.2.4.dev7.tar.gz` & `tmp/girder-hashsum-download-5.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-hashsum-download-3.2.4.dev7.tar", last modified: Wed Apr 24 19:13:02 2024, max compression
+gzip compressed data, was "girder-hashsum-download-5.0.0a2.tar", last modified: Fri Apr 12 16:30:40 2024, max compression
```

## Comparing `girder-hashsum-download-3.2.4.dev7.tar` & `girder-hashsum-download-5.0.0a2.tar`

### file list

```diff
@@ -1,31 +1,24 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:02.282506 girder-hashsum-download-3.2.4.dev7/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      614 2024-04-24 19:13:02.282506 girder-hashsum-download-3.2.4.dev7/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:02.278506 girder-hashsum-download-3.2.4.dev7/girder_hashsum_download/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7455 2024-04-24 19:11:47.000000 girder-hashsum-download-3.2.4.dev7/girder_hashsum_download/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      492 2024-04-24 19:11:47.000000 girder-hashsum-download-3.2.4.dev7/girder_hashsum_download/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:02.282506 girder-hashsum-download-3.2.4.dev7/girder_hashsum_download/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      516 2024-04-24 19:11:47.000000 girder-hashsum-download-3.2.4.dev7/girder_hashsum_download/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2024-04-24 19:11:47.000000 girder-hashsum-download-3.2.4.dev7/girder_hashsum_download/web_client/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:02.282506 girder-hashsum-download-3.2.4.dev7/girder_hashsum_download/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      140 2024-04-24 19:11:47.000000 girder-hashsum-download-3.2.4.dev7/girder_hashsum_download/web_client/stylesheets/hashsumDownloadFileInfoWidget.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:02.282506 girder-hashsum-download-3.2.4.dev7/girder_hashsum_download/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      482 2024-04-24 19:11:47.000000 girder-hashsum-download-3.2.4.dev7/girder_hashsum_download/web_client/templates/config.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2024-04-24 19:11:47.000000 girder-hashsum-download-3.2.4.dev7/girder_hashsum_download/web_client/templates/hashsumDownloadFileInfoWidget.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:02.282506 girder-hashsum-download-3.2.4.dev7/girder_hashsum_download/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2070 2024-04-24 19:11:47.000000 girder-hashsum-download-3.2.4.dev7/girder_hashsum_download/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1147 2024-04-24 19:11:47.000000 girder-hashsum-download-3.2.4.dev7/girder_hashsum_download/web_client/views/FileInfoWidget.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:02.282506 girder-hashsum-download-3.2.4.dev7/girder_hashsum_download.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      614 2024-04-24 19:13:02.000000 girder-hashsum-download-3.2.4.dev7/girder_hashsum_download.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      936 2024-04-24 19:13:02.000000 girder-hashsum-download-3.2.4.dev7/girder_hashsum_download.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:13:02.000000 girder-hashsum-download-3.2.4.dev7/girder_hashsum_download.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       81 2024-04-24 19:13:02.000000 girder-hashsum-download-3.2.4.dev7/girder_hashsum_download.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:13:02.000000 girder-hashsum-download-3.2.4.dev7/girder_hashsum_download.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-04-24 19:13:02.000000 girder-hashsum-download-3.2.4.dev7/girder_hashsum_download.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-04-24 19:13:02.000000 girder-hashsum-download-3.2.4.dev7/girder_hashsum_download.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-04-24 19:11:47.000000 girder-hashsum-download-3.2.4.dev7/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:02.282506 girder-hashsum-download-3.2.4.dev7/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:11:47.000000 girder-hashsum-download-3.2.4.dev7/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2371 2024-04-24 19:11:47.000000 girder-hashsum-download-3.2.4.dev7/plugin_tests/hashsumSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13472 2024-04-24 19:11:47.000000 girder-hashsum-download-3.2.4.dev7/plugin_tests/hashsum_download_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-24 19:13:02.282506 girder-hashsum-download-3.2.4.dev7/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1703 2024-04-24 19:11:47.000000 girder-hashsum-download-3.2.4.dev7/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:30:40.032569 girder-hashsum-download-5.0.0a2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      186 2024-04-12 16:27:18.000000 girder-hashsum-download-5.0.0a2/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      611 2024-04-12 16:30:40.032569 girder-hashsum-download-5.0.0a2/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:30:40.028569 girder-hashsum-download-5.0.0a2/girder_hashsum_download/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7498 2024-04-12 16:27:18.000000 girder-hashsum-download-5.0.0a2/girder_hashsum_download/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      492 2024-04-12 16:27:18.000000 girder-hashsum-download-5.0.0a2/girder_hashsum_download/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:30:40.028569 girder-hashsum-download-5.0.0a2/girder_hashsum_download/web_client/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:30:40.028569 girder-hashsum-download-5.0.0a2/girder_hashsum_download/web_client/dist/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9324 2024-04-12 16:28:16.000000 girder-hashsum-download-5.0.0a2/girder_hashsum_download/web_client/dist/girder-plugin-hashsum-download.umd.cjs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2024-04-12 16:28:16.000000 girder-hashsum-download-5.0.0a2/girder_hashsum_download/web_client/dist/style.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:30:40.028569 girder-hashsum-download-5.0.0a2/girder_hashsum_download.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      611 2024-04-12 16:30:39.000000 girder-hashsum-download-5.0.0a2/girder_hashsum_download.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      627 2024-04-12 16:30:40.000000 girder-hashsum-download-5.0.0a2/girder_hashsum_download.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:30:39.000000 girder-hashsum-download-5.0.0a2/girder_hashsum_download.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       81 2024-04-12 16:30:39.000000 girder-hashsum-download-5.0.0a2/girder_hashsum_download.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:30:39.000000 girder-hashsum-download-5.0.0a2/girder_hashsum_download.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-04-12 16:30:39.000000 girder-hashsum-download-5.0.0a2/girder_hashsum_download.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-04-12 16:30:39.000000 girder-hashsum-download-5.0.0a2/girder_hashsum_download.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-04-12 16:27:18.000000 girder-hashsum-download-5.0.0a2/plugin.cmake
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:30:40.028569 girder-hashsum-download-5.0.0a2/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:27:18.000000 girder-hashsum-download-5.0.0a2/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13472 2024-04-12 16:27:18.000000 girder-hashsum-download-5.0.0a2/plugin_tests/hashsum_download_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-12 16:30:40.032569 girder-hashsum-download-5.0.0a2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1703 2024-04-12 16:27:18.000000 girder-hashsum-download-5.0.0a2/setup.py
```

### Comparing `girder-hashsum-download-3.2.4.dev7/PKG-INFO` & `girder-hashsum-download-5.0.0a2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-hashsum-download
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Allows download of a file by its hashsum.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#hashsum-download
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `girder-hashsum-download-3.2.4.dev7/girder_hashsum_download/__init__.py` & `girder-hashsum-download-5.0.0a2/girder_hashsum_download/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 import hashlib
+from pathlib import Path
 
-import girder
 from girder import events
 from girder.api import access
 from girder.api.describe import autoDescribeRoute, Description
 from girder.api.rest import (
     filtermodel, setRawResponse, setResponseHeader, setContentDisposition)
 from girder.api.v1.file import File
 from girder.constants import AccessType, TokenScope
 from girder.exceptions import RestException
 from girder.models.file import File as FileModel
 from girder.models.setting import Setting
-from girder.plugin import GirderPlugin
+from girder.plugin import GirderPlugin, registerPluginStaticContent
 from girder.utility.progress import ProgressContext, noProgress
 
 from .settings import PluginSettings
 
 
 SUPPORTED_ALGORITHMS = {'sha512'}
 _CHUNK_LEN = 65536
 
 
 class HashedFile(File):
-    @property
-    def supportedAlgorithms(self):
-        girder.logger.warning(
-            'HashedFile.supportedAlgorithms is deprecated, use the module-level '
-            'SUPPORTED_ALGORITHMS instead.')
-        return SUPPORTED_ALGORITHMS
-
     def __init__(self, node):
         super().__init__()
 
         node.route('GET', ('hashsum', ':algo', ':hash'), self.getByHash)
         node.route('GET', ('hashsum', ':algo', ':hash', 'download'), self.downloadWithHash)
         node.route('GET', (':id', 'hashsum_file', ':algo'), self.downloadKeyFile)
         node.route('POST', (':id', 'hashsum'), self.computeHashes)
@@ -188,14 +181,21 @@
     }, multi=False)
 
     return digests
 
 
 class HashsumDownloadPlugin(GirderPlugin):
     DISPLAY_NAME = 'Hashsum Download'
-    CLIENT_SOURCE_PATH = 'web_client'
 
     def load(self, info):
         HashedFile(info['apiRoot'].file)
         FileModel().exposeFields(level=AccessType.READ, fields=SUPPORTED_ALGORITHMS)
 
         events.bind('data.process', 'hashsum_download', _computeHashHook)
+
+        registerPluginStaticContent(
+            plugin='hashsum_download',
+            css=['/style.css'],
+            js=['/girder-plugin-hashsum-download.umd.cjs'],
+            staticDir=Path(__file__).parent / 'web_client' / 'dist',
+            tree=info['serverRoot'],
+        )
```

### Comparing `girder-hashsum-download-3.2.4.dev7/girder_hashsum_download.egg-info/PKG-INFO` & `girder-hashsum-download-5.0.0a2/girder_hashsum_download.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-hashsum-download
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Allows download of a file by its hashsum.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#hashsum-download
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `girder-hashsum-download-3.2.4.dev7/plugin_tests/hashsum_download_test.py` & `girder-hashsum-download-5.0.0a2/plugin_tests/hashsum_download_test.py`

 * *Files identical despite different names*

### Comparing `girder-hashsum-download-3.2.4.dev7/setup.py` & `girder-hashsum-download-5.0.0a2/setup.py`

 * *Files identical despite different names*

