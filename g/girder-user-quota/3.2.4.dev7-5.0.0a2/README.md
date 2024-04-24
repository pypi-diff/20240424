# Comparing `tmp/girder-user-quota-3.2.4.dev7.tar.gz` & `tmp/girder_user_quota-5a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-user-quota-3.2.4.dev7.tar", last modified: Wed Apr 24 19:13:58 2024, max compression
+gzip compressed data, was "girder_user_quota-5a2.tar", last modified: Fri Apr 12 16:32:58 2024, max compression
```

## Comparing `girder-user-quota-3.2.4.dev7.tar` & `girder_user_quota-5a2.tar`

### file list

```diff
@@ -1,45 +1,25 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:58.778430 girder-user-quota-3.2.4.dev7/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      616 2024-04-24 19:13:58.778430 girder-user-quota-3.2.4.dev7/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:58.774430 girder-user-quota-3.2.4.dev7/girder_user_quota/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      874 2024-04-24 19:11:47.000000 girder-user-quota-3.2.4.dev7/girder_user_quota/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16648 2024-04-24 19:11:47.000000 girder-user-quota-3.2.4.dev7/girder_user_quota/quota.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      735 2024-04-24 19:11:47.000000 girder-user-quota-3.2.4.dev7/girder_user_quota/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:58.774430 girder-user-quota-3.2.4.dev7/girder_user_quota/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      295 2024-04-24 19:11:47.000000 girder-user-quota-3.2.4.dev7/girder_user_quota/web_client/main.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:58.774430 girder-user-quota-3.2.4.dev7/girder_user_quota/web_client/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      154 2024-04-24 19:11:47.000000 girder-user-quota-3.2.4.dev7/girder_user_quota/web_client/models/CollectionModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2024-04-24 19:11:47.000000 girder-user-quota-3.2.4.dev7/girder_user_quota/web_client/models/UserModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3788 2024-04-24 19:11:47.000000 girder-user-quota-3.2.4.dev7/girder_user_quota/web_client/models/extendModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      559 2024-04-24 19:11:47.000000 girder-user-quota-3.2.4.dev7/girder_user_quota/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      429 2024-04-24 19:11:47.000000 girder-user-quota-3.2.4.dev7/girder_user_quota/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:58.774430 girder-user-quota-3.2.4.dev7/girder_user_quota/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      394 2024-04-24 19:11:47.000000 girder-user-quota-3.2.4.dev7/girder_user_quota/web_client/stylesheets/userQuota.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:58.774430 girder-user-quota-3.2.4.dev7/girder_user_quota/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2024-04-24 19:11:47.000000 girder-user-quota-3.2.4.dev7/girder_user_quota/web_client/templates/collectionViewPoliciesMenu.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1337 2024-04-24 19:11:47.000000 girder-user-quota-3.2.4.dev7/girder_user_quota/web_client/templates/configView.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3480 2024-04-24 19:11:47.000000 girder-user-quota-3.2.4.dev7/girder_user_quota/web_client/templates/quotaPoliciesWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      228 2024-04-24 19:11:47.000000 girder-user-quota-3.2.4.dev7/girder_user_quota/web_client/templates/userViewPoliciesMenu.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:58.774430 girder-user-quota-3.2.4.dev7/girder_user_quota/web_client/utilities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2168 2024-04-24 19:11:47.000000 girder-user-quota-3.2.4.dev7/girder_user_quota/web_client/utilities/Conversions.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:58.778430 girder-user-quota-3.2.4.dev7/girder_user_quota/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      283 2024-04-24 19:11:47.000000 girder-user-quota-3.2.4.dev7/girder_user_quota/web_client/views/CollectionView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3357 2024-04-24 19:11:47.000000 girder-user-quota-3.2.4.dev7/girder_user_quota/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6817 2024-04-24 19:11:47.000000 girder-user-quota-3.2.4.dev7/girder_user_quota/web_client/views/QuotaPoliciesWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      677 2024-04-24 19:11:47.000000 girder-user-quota-3.2.4.dev7/girder_user_quota/web_client/views/UploadWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      241 2024-04-24 19:11:47.000000 girder-user-quota-3.2.4.dev7/girder_user_quota/web_client/views/UserView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1609 2024-04-24 19:11:47.000000 girder-user-quota-3.2.4.dev7/girder_user_quota/web_client/views/extendView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:58.778430 girder-user-quota-3.2.4.dev7/girder_user_quota.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      616 2024-04-24 19:13:58.000000 girder-user-quota-3.2.4.dev7/girder_user_quota.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1424 2024-04-24 19:13:58.000000 girder-user-quota-3.2.4.dev7/girder_user_quota.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:13:58.000000 girder-user-quota-3.2.4.dev7/girder_user_quota.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2024-04-24 19:13:58.000000 girder-user-quota-3.2.4.dev7/girder_user_quota.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:13:58.000000 girder-user-quota-3.2.4.dev7/girder_user_quota.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-04-24 19:13:58.000000 girder-user-quota-3.2.4.dev7/girder_user_quota.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2024-04-24 19:13:58.000000 girder-user-quota-3.2.4.dev7/girder_user_quota.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       55 2024-04-24 19:11:47.000000 girder-user-quota-3.2.4.dev7/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:58.778430 girder-user-quota-3.2.4.dev7/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:11:47.000000 girder-user-quota-3.2.4.dev7/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16489 2024-04-24 19:11:47.000000 girder-user-quota-3.2.4.dev7/plugin_tests/userQuotaSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21142 2024-04-24 19:11:47.000000 girder-user-quota-3.2.4.dev7/plugin_tests/user_quota_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-24 19:13:58.778430 girder-user-quota-3.2.4.dev7/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1694 2024-04-24 19:11:47.000000 girder-user-quota-3.2.4.dev7/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:32:58.437561 girder_user_quota-5a2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      162 2024-04-12 16:27:18.000000 girder_user_quota-5a2/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      613 2024-04-12 16:32:58.433561 girder_user_quota-5a2/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:32:58.433561 girder_user_quota-5a2/girder_user_quota/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1164 2024-04-12 16:27:18.000000 girder_user_quota-5a2/girder_user_quota/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16674 2024-04-12 16:27:18.000000 girder_user_quota-5a2/girder_user_quota/quota.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      735 2024-04-12 16:27:18.000000 girder_user_quota-5a2/girder_user_quota/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:32:58.429561 girder_user_quota-5a2/girder_user_quota/web_client/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:32:58.433561 girder_user_quota-5a2/girder_user_quota/web_client/dist/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    40917 2024-04-12 16:28:54.000000 girder_user_quota-5a2/girder_user_quota/web_client/dist/girder-plugin-user-quota.umd.cjs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      680 2024-04-12 16:28:54.000000 girder_user_quota-5a2/girder_user_quota/web_client/dist/style.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:32:58.433561 girder_user_quota-5a2/girder_user_quota.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      613 2024-04-12 16:32:58.000000 girder_user_quota-5a2/girder_user_quota.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      576 2024-04-12 16:32:58.000000 girder_user_quota-5a2/girder_user_quota.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:32:58.000000 girder_user_quota-5a2/girder_user_quota.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       63 2024-04-12 16:32:58.000000 girder_user_quota-5a2/girder_user_quota.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:32:58.000000 girder_user_quota-5a2/girder_user_quota.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-04-12 16:32:58.000000 girder_user_quota-5a2/girder_user_quota.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2024-04-12 16:32:58.000000 girder_user_quota-5a2/girder_user_quota.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       55 2024-04-12 16:27:18.000000 girder_user_quota-5a2/plugin.cmake
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:32:58.433561 girder_user_quota-5a2/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:27:18.000000 girder_user_quota-5a2/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21225 2024-04-12 16:27:18.000000 girder_user_quota-5a2/plugin_tests/user_quota_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-12 16:32:58.437561 girder_user_quota-5a2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1694 2024-04-12 16:27:18.000000 girder_user_quota-5a2/setup.py
```

### Comparing `girder-user-quota-3.2.4.dev7/PKG-INFO` & `girder_user_quota-5a2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-user-quota
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Limits total file size stored for individual users and collections and can direct all files to a specific assetstore
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-user-quota-3.2.4.dev7/girder_user_quota/quota.py` & `girder_user_quota-5a2/girder_user_quota/quota.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+import logging
+
 from bson.objectid import ObjectId, InvalidId
-from girder import logger
 from girder.api import access
 from girder.api.describe import Description, autoDescribeRoute
 from girder.api.rest import Resource
 from girder.constants import AccessType
 from girder.exceptions import GirderException, ValidationException, RestException
 from girder.models.assetstore import Assetstore
 from girder.models.collection import Collection
@@ -14,16 +15,16 @@
 from girder.models.user import User
 from girder.utility import assetstore_utilities
 from girder.utility.model_importer import ModelImporter
 from girder.utility.system import formatSize
 
 from .settings import PluginSettings
 
-
 QUOTA_FIELD = 'quota'
+logger = logging.getLogger(__name__)
 
 
 def ValidateSizeQuota(value):
     """
     Validate a quota value.  This may be blank or a non-negative integer.
 
     :param value: The proposed value.
```

### Comparing `girder-user-quota-3.2.4.dev7/girder_user_quota/settings.py` & `girder_user_quota-5a2/girder_user_quota/settings.py`

 * *Files identical despite different names*

### Comparing `girder-user-quota-3.2.4.dev7/girder_user_quota.egg-info/PKG-INFO` & `girder_user_quota-5a2/girder_user_quota.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-user-quota
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Limits total file size stored for individual users and collections and can direct all files to a specific assetstore
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-user-quota-3.2.4.dev7/plugin_tests/user_quota_test.py` & `girder_user_quota-5a2/plugin_tests/user_quota_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import datetime
 import json
 import os
+import tempfile
 
 from tests import base
 from girder.constants import AssetstoreType
 from girder.exceptions import ValidationException
 from girder.models.assetstore import Assetstore
 from girder.models.collection import Collection
 from girder.models.folder import Folder
@@ -348,44 +349,44 @@
 
     def testAssetstorePolicy(self):
         """
         Test assetstore policies for a user and a collection.
         """
         # We want three assetstores for testing, one of which is unreachable.
         # We already have one, which is the current assetstore.
-        base.dropGridFSDatabase('girder_test_user_quota_assetstore')
-        params = {
-            'name': 'Non-current Store',
-            'type': AssetstoreType.GRIDFS,
-            'db': 'girder_test_user_quota_assetstore'
-        }
-        resp = self.request(path='/assetstore', method='POST', user=self.admin,
-                            params=params)
-        self.assertStatusOk(resp)
-
-        # Create a broken assetstore. (Must bypass validation since it should
-        # not let us create an assetstore in a broken state).
-        Assetstore().save({
-            'name': 'Broken Store',
-            'type': AssetstoreType.FILESYSTEM,
-            'root': '/dev/null',
-            'created': datetime.datetime.utcnow()
-        }, validate=False)
-
-        # Now get the assetstores and save their ids for later
-        resp = self.request(path='/assetstore', method='GET', user=self.admin,
-                            params={'sort': 'created'})
-        self.assertStatusOk(resp)
-        assetstores = resp.json
-        self.assertEqual(len(assetstores), 3)
-        self.currentAssetstore = assetstores[0]
-        self.alternateAssetstore = assetstores[1]
-        self.brokenAssetstore = assetstores[2]
-        self._testAssetstores('user', self.user, self.admin)
-        self._testAssetstores('collection', self.collection, self.admin)
+        with tempfile.TemporaryDirectory() as root:
+            params = {
+                'name': 'Non-current Store',
+                'type': AssetstoreType.FILESYSTEM,
+                'root': root,
+            }
+            resp = self.request(path='/assetstore', method='POST', user=self.admin,
+                                params=params)
+            self.assertStatusOk(resp)
+
+            # Create a broken assetstore. (Must bypass validation since it should
+            # not let us create an assetstore in a broken state).
+            Assetstore().save({
+                'name': 'Broken Store',
+                'type': AssetstoreType.FILESYSTEM,
+                'root': '/dev/null',
+                'created': datetime.datetime.utcnow()
+            }, validate=False)
+
+            # Now get the assetstores and save their ids for later
+            resp = self.request(path='/assetstore', method='GET', user=self.admin,
+                                params={'sort': 'created'})
+            self.assertStatusOk(resp)
+            assetstores = resp.json
+            self.assertEqual(len(assetstores), 3)
+            self.currentAssetstore = assetstores[0]
+            self.alternateAssetstore = assetstores[1]
+            self.brokenAssetstore = assetstores[2]
+            self._testAssetstores('user', self.user, self.admin)
+            self._testAssetstores('collection', self.collection, self.admin)
 
     def testQuotaPolicy(self):
         """
         Test quota policies for a user and a collection.
         """
         self._testQuota('user', self.user, self.admin)
         self._testQuota('collection', self.collection, self.admin)
```

### Comparing `girder-user-quota-3.2.4.dev7/setup.py` & `girder_user_quota-5a2/setup.py`

 * *Files identical despite different names*

