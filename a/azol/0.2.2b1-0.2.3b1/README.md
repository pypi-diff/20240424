# Comparing `tmp/azol-0.2.2b1.tar.gz` & `tmp/azol-0.2.3b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azol-0.2.2b1.tar", last modified: Tue Apr 16 22:16:19 2024, max compression
+gzip compressed data, was "azol-0.2.3b1.tar", last modified: Wed Apr 24 13:15:28 2024, max compression
```

## Comparing `azol-0.2.2b1.tar` & `azol-0.2.3b1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:19.431204 azol-0.2.2b1/
--rw-r--r--   0 runner    (1001) docker     (127)    35801 2024-04-16 22:16:08.000000 azol-0.2.2b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-16 22:16:19.427204 azol-0.2.2b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-16 22:16:08.000000 azol-0.2.2b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:19.423204 azol-0.2.2b1/azol/
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:19.423204 azol-0.2.2b1/azol/caches/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/caches/azol_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/caches/in_memory_token_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/caches/local_token_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:19.423204 azol-0.2.2b1/azol/clients/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44625 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/clients/arm_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    29419 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/clients/graph_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/clients/key_vault_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10352 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/clients/oauth_http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    41909 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:19.427204 azol-0.2.2b1/azol/credentials/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/credentials/access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/credentials/application_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/credentials/credential.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/credentials/entraid_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/credentials/service_principal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/credentials/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:19.427204 azol-0.2.2b1/azol/models/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/models/generic_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/models/sp_login_init_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:19.427204 azol-0.2.2b1/azol/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/providers/file_secret_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/providers/key_vault_secret_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:19.427204 azol-0.2.2b1/azol/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   270913 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/resources/graph_delegated_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)   182559 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/resources/graph_permissions_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    32330 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/resources/rbac_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:19.427204 azol-0.2.2b1/azol/services/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24848 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/services/token_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    44361 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/services/token_service_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:19.427204 azol-0.2.2b1/azol/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/utils/auth_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-16 22:16:08.000000 azol-0.2.2b1/azol/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 22:16:19.427204 azol-0.2.2b1/azol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-16 22:16:19.000000 azol-0.2.2b1/azol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-16 22:16:19.000000 azol-0.2.2b1/azol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 22:16:19.000000 azol-0.2.2b1/azol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-16 22:16:19.000000 azol-0.2.2b1/azol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-16 22:16:19.000000 azol-0.2.2b1/azol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-16 22:16:08.000000 azol-0.2.2b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 22:16:19.431204 azol-0.2.2b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-16 22:16:08.000000 azol-0.2.2b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:15:28.497771 azol-0.2.3b1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35801 2024-04-24 13:15:11.000000 azol-0.2.3b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-24 13:15:28.497771 azol-0.2.3b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-24 13:15:11.000000 azol-0.2.3b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:15:28.489771 azol-0.2.3b1/azol/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:15:28.489771 azol-0.2.3b1/azol/caches/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/caches/azol_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/caches/in_memory_token_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/caches/local_token_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:15:28.489771 azol-0.2.3b1/azol/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44625 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/clients/arm_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33149 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/clients/graph_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/clients/key_vault_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10352 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/clients/oauth_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41909 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:15:28.493771 azol-0.2.3b1/azol/credentials/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/credentials/access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/credentials/application_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/credentials/credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/credentials/entraid_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/credentials/service_principal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/credentials/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:15:28.493771 azol-0.2.3b1/azol/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/models/generic_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/models/sp_login_init_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:15:28.493771 azol-0.2.3b1/azol/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/providers/file_secret_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/providers/key_vault_secret_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:15:28.493771 azol-0.2.3b1/azol/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   270913 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/resources/graph_delegated_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)   182559 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/resources/graph_permissions_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32330 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/resources/rbac_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:15:28.493771 azol-0.2.3b1/azol/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24848 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/services/token_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44361 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/services/token_service_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:15:28.497771 azol-0.2.3b1/azol/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/utils/auth_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-24 13:15:11.000000 azol-0.2.3b1/azol/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:15:28.497771 azol-0.2.3b1/azol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-24 13:15:28.000000 azol-0.2.3b1/azol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-24 13:15:28.000000 azol-0.2.3b1/azol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:15:28.000000 azol-0.2.3b1/azol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-24 13:15:28.000000 azol-0.2.3b1/azol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 13:15:28.000000 azol-0.2.3b1/azol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-24 13:15:11.000000 azol-0.2.3b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:15:28.497771 azol-0.2.3b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-24 13:15:11.000000 azol-0.2.3b1/setup.py
```

### Comparing `azol-0.2.2b1/LICENSE` & `azol-0.2.3b1/LICENSE`

 * *Files identical despite different names*

### Comparing `azol-0.2.2b1/PKG-INFO` & `azol-0.2.3b1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azol
-Version: 0.2.2b1
+Version: 0.2.3b1
 Summary: A python-based pentesting library for Azure and Entra ID
 Home-page: https://github.com/cdburkard/azol
 Author: Cody Burkard
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 Requires-Dist: dataclasses==0.6
```

### Comparing `azol-0.2.2b1/README.md` & `azol-0.2.3b1/README.md`

 * *Files identical despite different names*

### Comparing `azol-0.2.2b1/azol/__init__.py` & `azol-0.2.3b1/azol/__init__.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.2b1/azol/caches/azol_cache.py` & `azol-0.2.3b1/azol/caches/azol_cache.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.2b1/azol/caches/local_token_cache.py` & `azol-0.2.3b1/azol/caches/local_token_cache.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.2b1/azol/clients/arm_client.py` & `azol-0.2.3b1/azol/clients/arm_client.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.2b1/azol/clients/graph_client.py` & `azol-0.2.3b1/azol/clients/graph_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -58,43 +58,84 @@
         """
         response = self._send_request( "/roleManagement/directory/roleDefinitions?"
                                        "$select=displayName,id,isBuiltIn" )
         if response:
             return self._get_all_graph_objects(response)
         raise GraphRequestFailedException()
 
-    def get_active_pim_sessions( self ):
+    def get_current_pim_eligibility( self ):
+        """Get pim eligibility of the current principal.
+
+        Returns:
+            A list of dictionaries containing the pim eligibility of the current principal.
+
+        Raises:
+            GraphRequestFailedException: An error occurred accessing the Graph API
+
+        """
+        response = self._send_request( "/roleManagement/directory/roleEligibilitySchedules/"
+                                       "filterByCurrentUser(on='principal')?"
+                                       "$expand=principal,roleDefinition($select=displayName,id,templateId)"
+                                       "&$select=principal,roleDefinition,scheduleInfo,memberType,appScopeId,"
+                                       "directoryScopeId,createdDateTime" )
+        if response:
+            return self._get_all_graph_objects(response)
+        raise GraphRequestFailedException()
+
+    def get_current_pim_activations( self ):
+        """Get pim activations of the current principal.
+
+        Returns:
+            A list of dictionaries containing the pim activations of the current principal.
+
+        Raises:
+            GraphRequestFailedException: An error occurred accessing the Graph API
+
+        """
+        response = self._send_request( "/roleManagement/directory/roleAssignmentSchedules/"
+                                       "filterByCurrentUser(on='principal')?"
+                                       "$expand=principal,roleDefinition($select=displayName,id,templateId)"
+                                       "&$select=principal,roleDefinition,scheduleInfo,memberType,appScopeId,"
+                                       "directoryScopeId,createdDateTime" )
+        if response:
+            return self._get_all_graph_objects(response)
+        raise GraphRequestFailedException()
+
+    def get_active_pim_assignments( self ):
         """Get all active PIM sessions.
         
         Returns:
             A list of dictionaries containing the active PIM sessions in the directory.
 
         Raises:
             GraphRequestFailedException: An error occurred accessing the Graph API
 
         """
         response = self._send_request( "/roleManagement/directory/roleAssignmentSchedules?"
-                                      "$select=roleDefinitionId,principalId,"
-                                      "directoryScopeId,scheduleInfo,scheduleInfo" )
+                                       "$expand=principal,roleDefinition($select=displayName,id,templateId)"
+                                       "&$select=principal,roleDefinition,scheduleInfo,memberType,appScopeId,"
+                                       "directoryScopeId,createdDateTime" )
         if response:
             return self._get_all_graph_objects(response)
         raise GraphRequestFailedException()
 
-
-    def get_eligible_pim_sessions( self ):
-        """Get all eligible PIM sessions.
+    def get_eligible_pim_assignments( self ):
+        """Get all eligible PIM assignments.
         
         Returns:
-            A list of dictionaries containing the eligible PIM sessions in the directory.
+            A list of dictionaries containing the eligible PIM assignments in the directory.
 
         Raises:
             GraphRequestFailedException: An error occurred accessing the Graph API
 
         """
-        response = self._send_request( "/roleManagement/directory/roleEligibilitySchedules" )
+        response = self._send_request( "/roleManagement/directory/roleEligibilitySchedules?"
+                                       "$expand=principal,roleDefinition($select=displayName,id,templateId)"
+                                       "&$select=principal,roleDefinition,scheduleInfo,memberType,appScopeId,"
+                                       "directoryScopeId,createdDateTime" )
         if response:
             return self._get_all_graph_objects(response)
         raise GraphRequestFailedException()
 
     def get_transitive_group_memberships( self, group_id ):
         """Get transitive group memberships of a specific group.
         
@@ -109,80 +150,96 @@
 
         """
         response = self._send_request( f"/groups/{group_id}/transitiveMembers" )
         if response:
             return self._get_all_graph_objects(response)
         raise GraphRequestFailedException()
 
-    def get_all_users( self, abbreviate=True ):
+    def get_all_users( self, select=[] ):
         """Get all users in the directory.
 
+        Args:
+            select - (list) - a list of json attributes that should be returned from all group.
+                    if this is None, the select query parameter will not be used in the request
         Returns:
             A list of objects containing object id and displayName of all users
 
         Raises:
             GraphRequestFailedException: An error occurred accessing the Graph API
         """
-
-        if abbreviate:
-            url_with_filter = "/users?$select=id,displayName"
+        if select == []:
+            path_and_params="/users?$select=id,displayName"
+        elif select == None:
+            path_and_params="/users"
         else:
-            url_with_filter = "/users"
-
-        response = self._send_request( url_with_filter )
+            path_and_params="/users?$select="+",".join(select)
+        response = self._send_request( path_and_params )
         if response:
             return self._get_all_graph_objects(response)
         raise GraphRequestFailedException()
 
-    def get_all_service_principals( self, abbreviate=True ):
+    def get_all_service_principals( self, select=[] ):
         """Get all service principals in the directory.
 
+        Args:
+            select - (list) - a list of json attributes that should be returned from all group.
+                    if this is None, the select query parameter will not be used in the request
         Returns:
             A list of objects containing object id and displayName of all service principals
 
         Raises:
             GraphRequestFailedException: An error occurred accessing the Graph API
         """
-        
-        if abbreviate:
-            url_with_filter = "/servicePrincipals?$select=id,displayName"
+        if select == []:
+            path_and_params="/servicePrincipals?$select=id,displayName"
+        elif select == None:
+            path_and_params="/servicePrincipals"
         else:
-            url_with_filter = "/servicePrincipals"
+            path_and_params="/servicePrincipals?$select="+",".join(select)
         
-        response = self._send_request( url_with_filter )
+        response = self._send_request( path_and_params )
         if response:
             return self._get_all_graph_objects(response)
         raise GraphRequestFailedException()
 
-    def get_all_applications( self ):
+    def get_all_applications( self, select=[] ):
         """Get all application objects in the directory.
 
         Returns:
             A list of objects containing object id and displayName of all application objects
 
         Raises:
             GraphRequestFailedException: An error occurred accessing the Graph API
         """
-        response = self._send_request( "/applications?$select=id,displayName" )
+        if select == []:
+            path_and_params="/applications?$select=id,displayName"
+        elif select == None:
+            path_and_params="/applications"
+        else:
+            path_and_params="/applications?$select="+",".join(select)
+        response = self._send_request( path_and_params )
         if response:
             return self._get_all_graph_objects(response)
         raise GraphRequestFailedException()
 
-    def get_directory_role_assignments( self ):
+    def get_directory_role_assignments( self, object=None ):
         """Get directory role assignments.
 
         Get all Entra ID role assignments in the directory, ignoring assignments through PIM
 
         Returns:
             A list of dictionaries containing role assignment metadata
 
         Raises:
             GraphRequestFailedException: An error occurred accessing the Graph API
         """
-        response = self._send_request( "/roleManagement/directory/roleAssignments" )
+        if object is None:
+            response = self._send_request( "/roleManagement/directory/roleAssignments" )
+        else:
+            response = self._send_request( f"/roleManagement/directory/roleAssignments?$count=true&$filter=principalId eq '{object}'" )
         if response:
             return self._get_all_graph_objects(response)
         raise GraphRequestFailedException()
 
     def delete_directory_role_assignments( self, assignment_id ):
         """Remove an Entra ID role from a principal in the directory.
 
@@ -217,15 +274,15 @@
         body = {
             "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
             "roleDefinitionId": role_definition_id,
             "principalId": principal_id,
             "directoryScopeId": "/"
         }
         response = self._send_request( "/roleManagement/directory/roleAssignments",
-                                       method="POST", json=body )
+                                       method="POST", success_code=201, json=body )
         if response:
             return response.json()
         raise GraphRequestFailedException()
 
     def add_app_owner( self, app_object_id, principal_id ):
         """Add an owner to an application object.
 
@@ -320,26 +377,36 @@
         """
         response = self._send_request( "/groups?$expand=memberOf($select=id,displayName)"
                                        "&$select=memberOf,id,displayName" )
         if response:
             return self._get_all_graph_objects(response)
         raise GraphRequestFailedException()
 
-    def get_all_groups( self ):
+    def get_all_groups( self, select=[] ):
         """Get all group ids and displaynames in Entra Id.
 
         Calls the graph API get get all groups, and nested memberships.
 
+        Args:
+            select - (list) - a list of json attributes that should be returned from all group.
+                    if this is None, the select query parameter will not be used in the request
+
         Returns:
             A list of dictionaries, containing group ids and names
 
         Raises:
             GraphRequestFailedException: An error occurred accessing the Graph API
         """
-        response = self._send_request( "/groups?$select=id,displayName" )
+        if select == []:
+            path_and_params="/groups?$select=id,displayName"
+        elif select == None:
+            path_and_params="/groups"
+        else:
+            path_and_params="/groups?$select="+",".join(select)
+        response = self._send_request( path_and_params )
         if response:
             return self._get_all_graph_objects(response)
         raise GraphRequestFailedException()
 
     def get_all_groups_and_owners( self ):
         """Get all group owners in all Entra ID groups.
```

### Comparing `azol-0.2.2b1/azol/clients/key_vault_client.py` & `azol-0.2.3b1/azol/clients/key_vault_client.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.2b1/azol/clients/oauth_http_client.py` & `azol-0.2.3b1/azol/clients/oauth_http_client.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.2b1/azol/constants.py` & `azol-0.2.3b1/azol/constants.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.2b1/azol/credentials/access_token.py` & `azol-0.2.3b1/azol/credentials/access_token.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.2b1/azol/credentials/application_object.py` & `azol-0.2.3b1/azol/credentials/application_object.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.2b1/azol/credentials/credential.py` & `azol-0.2.3b1/azol/credentials/credential.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.2b1/azol/credentials/service_principal.py` & `azol-0.2.3b1/azol/credentials/service_principal.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.2b1/azol/credentials/user.py` & `azol-0.2.3b1/azol/credentials/user.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.2b1/azol/models/generic_resource.py` & `azol-0.2.3b1/azol/models/generic_resource.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.2b1/azol/providers/file_secret_provider.py` & `azol-0.2.3b1/azol/providers/file_secret_provider.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,29 +5,21 @@
 from azol.constants import AZOLSECRETPROVIDERFOLDER
 
 class FileSecretProvider( object ):
     """
         A local file secret provider for the azol token service
     """
 
-    def __init__( self, azol_id=None ):
+    def __init__( self, file=None, directory=AZOLSECRETPROVIDERFOLDER ):
 
-        if azol_id is None:
-            azol_id = uuid.uuid4()
-        self._id = azol_id
-        self.file_path=AZOLSECRETPROVIDERFOLDER + "/" + self._id
-        Path(AZOLSECRETPROVIDERFOLDER).mkdir(parents=True, exist_ok=True)
-
-    def get_id( self ):
-        """
-            Get the azol id of the file secret provider
-
-            Returns string - azol id
-        """
-        return self._id
+        if file is None:
+            file = uuid.uuid4()
+        self.file = file
+        self.file_path=directory + "/" + self.file
+        Path(directory).mkdir(parents=True, exist_ok=True)
 
     def get_secret( self, secret_reference ):
         """
             Get a secret value based on its reference name
 
             Args:
                 - secretReference - (string) The secret reference name
```

### Comparing `azol-0.2.2b1/azol/providers/key_vault_secret_provider.py` & `azol-0.2.3b1/azol/providers/key_vault_secret_provider.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.2b1/azol/resources/graph_delegated_permissions.py` & `azol-0.2.3b1/azol/resources/graph_delegated_permissions.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.2b1/azol/resources/graph_permissions_map.py` & `azol-0.2.3b1/azol/resources/graph_permissions_map.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.2b1/azol/resources/rbac_roles.py` & `azol-0.2.3b1/azol/resources/rbac_roles.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.2b1/azol/services/token_service.py` & `azol-0.2.3b1/azol/services/token_service.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.2b1/azol/services/token_service_helpers.py` & `azol-0.2.3b1/azol/services/token_service_helpers.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.2b1/azol/utils/auth_utils.py` & `azol-0.2.3b1/azol/utils/auth_utils.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.2b1/azol/utils/utils.py` & `azol-0.2.3b1/azol/utils/utils.py`

 * *Files identical despite different names*

### Comparing `azol-0.2.2b1/azol.egg-info/PKG-INFO` & `azol-0.2.3b1/azol.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azol
-Version: 0.2.2b1
+Version: 0.2.3b1
 Summary: A python-based pentesting library for Azure and Entra ID
 Home-page: https://github.com/cdburkard/azol
 Author: Cody Burkard
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 Requires-Dist: dataclasses==0.6
```

### Comparing `azol-0.2.2b1/azol.egg-info/SOURCES.txt` & `azol-0.2.3b1/azol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azol-0.2.2b1/setup.py` & `azol-0.2.3b1/setup.py`

 * *Files identical despite different names*

