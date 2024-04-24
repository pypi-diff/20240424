# Comparing `tmp/girder-ldap-3.2.4.dev7.tar.gz` & `tmp/girder-ldap-5.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-ldap-3.2.4.dev7.tar", last modified: Wed Apr 24 19:13:34 2024, max compression
+gzip compressed data, was "girder-ldap-5.0.0a2.tar", last modified: Fri Apr 12 16:31:27 2024, max compression
```

## Comparing `girder-ldap-3.2.4.dev7.tar` & `girder-ldap-5.0.0a2.tar`

### file list

```diff
@@ -1,31 +1,24 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:34.102464 girder-ldap-3.2.4.dev7/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      574 2024-04-24 19:13:34.102464 girder-ldap-3.2.4.dev7/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:34.098464 girder-ldap-3.2.4.dev7/girder_ldap/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6318 2024-04-24 19:11:47.000000 girder-ldap-3.2.4.dev7/girder_ldap/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2076 2024-04-24 19:11:47.000000 girder-ldap-3.2.4.dev7/girder_ldap/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:34.102464 girder-ldap-3.2.4.dev7/girder_ldap/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2024-04-24 19:11:47.000000 girder-ldap-3.2.4.dev7/girder_ldap/web_client/main.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      561 2024-04-24 19:11:47.000000 girder-ldap-3.2.4.dev7/girder_ldap/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      406 2024-04-24 19:11:47.000000 girder-ldap-3.2.4.dev7/girder_ldap/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:34.102464 girder-ldap-3.2.4.dev7/girder_ldap/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-04-24 19:11:47.000000 girder-ldap-3.2.4.dev7/girder_ldap/web_client/stylesheets/configView.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:34.102464 girder-ldap-3.2.4.dev7/girder_ldap/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1438 2024-04-24 19:11:47.000000 girder-ldap-3.2.4.dev7/girder_ldap/web_client/templates/configView.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2592 2024-04-24 19:11:47.000000 girder-ldap-3.2.4.dev7/girder_ldap/web_client/templates/editServerMixin.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-04-24 19:11:47.000000 girder-ldap-3.2.4.dev7/girder_ldap/web_client/templates/newServerTemplate.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:34.102464 girder-ldap-3.2.4.dev7/girder_ldap/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4955 2024-04-24 19:11:47.000000 girder-ldap-3.2.4.dev7/girder_ldap/web_client/views/ConfigView.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:34.102464 girder-ldap-3.2.4.dev7/girder_ldap.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      574 2024-04-24 19:13:33.000000 girder-ldap-3.2.4.dev7/girder_ldap.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      716 2024-04-24 19:13:34.000000 girder-ldap-3.2.4.dev7/girder_ldap.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:13:33.000000 girder-ldap-3.2.4.dev7/girder_ldap.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       46 2024-04-24 19:13:33.000000 girder-ldap-3.2.4.dev7/girder_ldap.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:13:33.000000 girder-ldap-3.2.4.dev7/girder_ldap.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       17 2024-04-24 19:13:33.000000 girder-ldap-3.2.4.dev7/girder_ldap.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2024-04-24 19:13:33.000000 girder-ldap-3.2.4.dev7/girder_ldap.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2024-04-24 19:11:47.000000 girder-ldap-3.2.4.dev7/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:34.102464 girder-ldap-3.2.4.dev7/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:11:47.000000 girder-ldap-3.2.4.dev7/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9007 2024-04-24 19:11:47.000000 girder-ldap-3.2.4.dev7/plugin_tests/ldap_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-24 19:13:34.102464 girder-ldap-3.2.4.dev7/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1615 2024-04-24 19:11:47.000000 girder-ldap-3.2.4.dev7/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:31:27.360912 girder-ldap-5.0.0a2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      138 2024-04-12 16:27:18.000000 girder-ldap-5.0.0a2/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      571 2024-04-12 16:31:27.360912 girder-ldap-5.0.0a2/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:31:27.356912 girder-ldap-5.0.0a2/girder_ldap/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6596 2024-04-12 16:27:18.000000 girder-ldap-5.0.0a2/girder_ldap/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2076 2024-04-12 16:27:18.000000 girder-ldap-5.0.0a2/girder_ldap/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:31:27.356912 girder-ldap-5.0.0a2/girder_ldap/web_client/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:31:27.360912 girder-ldap-5.0.0a2/girder_ldap/web_client/dist/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    44338 2024-04-12 16:28:36.000000 girder-ldap-5.0.0a2/girder_ldap/web_client/dist/girder-plugin-ldap.umd.cjs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      325 2024-04-12 16:28:36.000000 girder-ldap-5.0.0a2/girder_ldap/web_client/dist/style.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:31:27.360912 girder-ldap-5.0.0a2/girder_ldap.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      571 2024-04-12 16:31:27.000000 girder-ldap-5.0.0a2/girder_ldap.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      471 2024-04-12 16:31:27.000000 girder-ldap-5.0.0a2/girder_ldap.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:31:27.000000 girder-ldap-5.0.0a2/girder_ldap.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       46 2024-04-12 16:31:27.000000 girder-ldap-5.0.0a2/girder_ldap.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:31:27.000000 girder-ldap-5.0.0a2/girder_ldap.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       17 2024-04-12 16:31:27.000000 girder-ldap-5.0.0a2/girder_ldap.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2024-04-12 16:31:27.000000 girder-ldap-5.0.0a2/girder_ldap.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2024-04-12 16:27:18.000000 girder-ldap-5.0.0a2/plugin.cmake
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:31:27.360912 girder-ldap-5.0.0a2/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:27:18.000000 girder-ldap-5.0.0a2/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9007 2024-04-12 16:27:18.000000 girder-ldap-5.0.0a2/plugin_tests/ldap_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-12 16:31:27.360912 girder-ldap-5.0.0a2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1615 2024-04-12 16:27:18.000000 girder-ldap-5.0.0a2/setup.py
```

### Comparing `girder-ldap-3.2.4.dev7/PKG-INFO` & `girder-ldap-5.0.0a2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-ldap
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Authenticate user credentials against LDAP or Active Directory servers.
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-ldap-3.2.4.dev7/girder_ldap/__init__.py` & `girder-ldap-5.0.0a2/girder_ldap/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+from pathlib import Path
+
 import ldap
 
 from girder import events
 from girder.api import access
 from girder.api.describe import autoDescribeRoute, Description
 from girder.api.rest import boundHandler
 from girder.exceptions import ValidationException, RestException
 from girder.models.setting import Setting
 from girder.models.user import User
-from girder.plugin import GirderPlugin
+from girder.plugin import GirderPlugin, registerPluginStaticContent
 
 from .settings import PluginSettings
 
 _LDAP_ATTRS = ('uid', 'mail', 'cn', 'sn', 'givenName', 'distinguishedName')
 _MAX_NAME_ATTEMPTS = 10
 _CONNECT_TIMEOUT = 4  # seconds
 
@@ -159,12 +161,19 @@
     finally:
         if conn:
             conn.unbind_s()
 
 
 class LDAPPlugin(GirderPlugin):
     DISPLAY_NAME = 'LDAP Authentication'
-    CLIENT_SOURCE_PATH = 'web_client'
 
     def load(self, info):
         events.bind('model.user.authenticate', 'ldap', _ldapAuth)
         info['apiRoot'].system.route('GET', ('ldap_server', 'status'), _ldapServerTest)
+
+        registerPluginStaticContent(
+            plugin='ldap',
+            css=['/style.css'],
+            js=['/girder-plugin-ldap.umd.cjs'],
+            staticDir=Path(__file__).parent / 'web_client' / 'dist',
+            tree=info['serverRoot'],
+        )
```

### Comparing `girder-ldap-3.2.4.dev7/girder_ldap/settings.py` & `girder-ldap-5.0.0a2/girder_ldap/settings.py`

 * *Files identical despite different names*

### Comparing `girder-ldap-3.2.4.dev7/girder_ldap.egg-info/PKG-INFO` & `girder-ldap-5.0.0a2/girder_ldap.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-ldap
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: Authenticate user credentials against LDAP or Active Directory servers.
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `girder-ldap-3.2.4.dev7/plugin_tests/ldap_test.py` & `girder-ldap-5.0.0a2/plugin_tests/ldap_test.py`

 * *Files identical despite different names*

### Comparing `girder-ldap-3.2.4.dev7/setup.py` & `girder-ldap-5.0.0a2/setup.py`

 * *Files identical despite different names*

