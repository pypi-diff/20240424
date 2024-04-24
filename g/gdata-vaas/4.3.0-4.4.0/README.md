# Comparing `tmp/gdata-vaas-4.3.0.tar.gz` & `tmp/gdata_vaas-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdata-vaas-4.3.0.tar", last modified: Wed Mar 13 14:31:10 2024, max compression
+gzip compressed data, was "gdata_vaas-4.4.0.tar", last modified: Wed Apr 24 12:12:05 2024, max compression
```

## Comparing `gdata-vaas-4.3.0.tar` & `gdata_vaas-4.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:31:10.459214 gdata-vaas-4.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-13 14:30:29.000000 gdata-vaas-4.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-03-13 14:31:10.459214 gdata-vaas-4.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-03-13 14:30:29.000000 gdata-vaas-4.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-13 14:30:29.000000 gdata-vaas-4.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-13 14:31:10.459214 gdata-vaas-4.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-13 14:30:29.000000 gdata-vaas-4.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:31:10.455214 gdata-vaas-4.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:31:10.459214 gdata-vaas-4.3.0/src/gdata_vaas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-03-13 14:31:10.000000 gdata-vaas-4.3.0/src/gdata_vaas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-13 14:31:10.000000 gdata-vaas-4.3.0/src/gdata_vaas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 14:31:10.000000 gdata-vaas-4.3.0/src/gdata_vaas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-13 14:31:10.000000 gdata-vaas-4.3.0/src/gdata_vaas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-13 14:31:10.000000 gdata-vaas-4.3.0/src/gdata_vaas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:31:10.459214 gdata-vaas-4.3.0/src/vaas/
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-13 14:30:29.000000 gdata-vaas-4.3.0/src/vaas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-13 14:30:29.000000 gdata-vaas-4.3.0/src/vaas/client_credentials_grant_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-03-13 14:30:29.000000 gdata-vaas-4.3.0/src/vaas/resource_owner_password_grant_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14739 2024-03-13 14:30:29.000000 gdata-vaas-4.3.0/src/vaas/vaas.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-13 14:30:29.000000 gdata-vaas-4.3.0/src/vaas/vaas_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:31:10.459214 gdata-vaas-4.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-03-13 14:30:29.000000 gdata-vaas-4.3.0/tests/test_client_credentials_grant_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-03-13 14:30:29.000000 gdata-vaas-4.3.0/tests/test_resource_owner_password_grant_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11931 2024-03-13 14:30:29.000000 gdata-vaas-4.3.0/tests/test_vaas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:12:05.144325 gdata_vaas-4.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-24 12:11:06.000000 gdata_vaas-4.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-04-24 12:12:05.144325 gdata_vaas-4.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-24 12:11:06.000000 gdata_vaas-4.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-24 12:11:06.000000 gdata_vaas-4.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-24 12:12:05.148325 gdata_vaas-4.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-24 12:11:06.000000 gdata_vaas-4.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:12:05.140325 gdata_vaas-4.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:12:05.144325 gdata_vaas-4.4.0/src/gdata_vaas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-04-24 12:12:05.000000 gdata_vaas-4.4.0/src/gdata_vaas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-24 12:12:05.000000 gdata_vaas-4.4.0/src/gdata_vaas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 12:12:05.000000 gdata_vaas-4.4.0/src/gdata_vaas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-24 12:12:05.000000 gdata_vaas-4.4.0/src/gdata_vaas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 12:12:05.000000 gdata_vaas-4.4.0/src/gdata_vaas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:12:05.144325 gdata_vaas-4.4.0/src/vaas/
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-24 12:11:06.000000 gdata_vaas-4.4.0/src/vaas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-24 12:11:06.000000 gdata_vaas-4.4.0/src/vaas/client_credentials_grant_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-24 12:11:06.000000 gdata_vaas-4.4.0/src/vaas/resource_owner_password_grant_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14646 2024-04-24 12:11:06.000000 gdata_vaas-4.4.0/src/vaas/vaas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-24 12:11:06.000000 gdata_vaas-4.4.0/src/vaas/vaas_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:12:05.144325 gdata_vaas-4.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-24 12:11:06.000000 gdata_vaas-4.4.0/tests/test_client_credentials_grant_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-24 12:11:06.000000 gdata_vaas-4.4.0/tests/test_resource_owner_password_grant_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11931 2024-04-24 12:11:06.000000 gdata_vaas-4.4.0/tests/test_vaas.py
```

### Comparing `gdata-vaas-4.3.0/LICENSE` & `gdata_vaas-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdata-vaas-4.3.0/PKG-INFO` & `gdata_vaas-4.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdata-vaas
-Version: 4.3.0
+Version: 4.4.0
 Summary: gdata-vaas is a Python library for the VaaS-API.
 Home-page: https://github.com/GDATASoftwareAG/vaas/tree/main/python
 Author: G DATA CyberDefense AG
 Author-email: oem@gdata.de
 Project-URL: Bug Tracker, https://github.com/GDATASoftwareAG/vaas/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gdata-vaas-4.3.0/README.md` & `gdata_vaas-4.4.0/README.md`

 * *Files identical despite different names*

### Comparing `gdata-vaas-4.3.0/setup.cfg` & `gdata_vaas-4.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gdata-vaas
-version = 4.3.0
+version = 4.4.0
 author = G DATA CyberDefense AG
 author_email = oem@gdata.de
 description = gdata-vaas is a Python library for the VaaS-API.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/GDATASoftwareAG/vaas/tree/main/python
 project_urls =
```

### Comparing `gdata-vaas-4.3.0/src/gdata_vaas.egg-info/PKG-INFO` & `gdata_vaas-4.4.0/src/gdata_vaas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdata-vaas
-Version: 4.3.0
+Version: 4.4.0
 Summary: gdata-vaas is a Python library for the VaaS-API.
 Home-page: https://github.com/GDATASoftwareAG/vaas/tree/main/python
 Author: G DATA CyberDefense AG
 Author-email: oem@gdata.de
 Project-URL: Bug Tracker, https://github.com/GDATASoftwareAG/vaas/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gdata-vaas-4.3.0/src/gdata_vaas.egg-info/SOURCES.txt` & `gdata_vaas-4.4.0/src/gdata_vaas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gdata-vaas-4.3.0/src/vaas/__init__.py` & `gdata_vaas-4.4.0/src/vaas/__init__.py`

 * *Files identical despite different names*

### Comparing `gdata-vaas-4.3.0/src/vaas/client_credentials_grant_authenticator.py` & `gdata_vaas-4.4.0/src/vaas/client_credentials_grant_authenticator.py`

 * *Files identical despite different names*

### Comparing `gdata-vaas-4.3.0/src/vaas/resource_owner_password_grant_authenticator.py` & `gdata_vaas-4.4.0/src/vaas/resource_owner_password_grant_authenticator.py`

 * *Files identical despite different names*

### Comparing `gdata-vaas-4.3.0/src/vaas/vaas.py` & `gdata_vaas-4.4.0/src/vaas/vaas.py`

 * *Files 0% similar despite different names*

```diff
@@ -357,22 +357,20 @@
                 )
 
         return map_response(verdict_response)
 
     async def __upload(self, token, upload_uri, buffer_or_file, content_length):
         jwt = PyJWT()
         decoded_token = jwt.decode(token, options={"verify_signature": False})
-        trace_id = decoded_token.get("traceId")
         try:
             await self.httpx_client.put(
                 url=upload_uri,
                 content=buffer_or_file,
                 headers={
                     "Authorization": token,
-                    "traceParent": trace_id,
                     "Content-Length": str(content_length),
                 },
                 timeout=UPLOAD_TIMEOUT,
             )
         except httpx.TimeoutException as ex:
             self.tracing.trace_upload_timeout(content_length)
             raise VaasTimeoutError() from ex
```

### Comparing `gdata-vaas-4.3.0/src/vaas/vaas_errors.py` & `gdata_vaas-4.4.0/src/vaas/vaas_errors.py`

 * *Files identical despite different names*

### Comparing `gdata-vaas-4.3.0/tests/test_client_credentials_grant_authenticator.py` & `gdata_vaas-4.4.0/tests/test_client_credentials_grant_authenticator.py`

 * *Files identical despite different names*

### Comparing `gdata-vaas-4.3.0/tests/test_resource_owner_password_grant_authenticator.py` & `gdata_vaas-4.4.0/tests/test_resource_owner_password_grant_authenticator.py`

 * *Files identical despite different names*

### Comparing `gdata-vaas-4.3.0/tests/test_vaas.py` & `gdata_vaas-4.4.0/tests/test_vaas.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,20 +54,20 @@
     async def test_connects(self):
         async with await create_and_connect():
             pass
 
     async def test_for_sha256_returns_clean_for_clean_sha256(self):
         async with await create_and_connect() as vaas:
             verdict = await vaas.for_sha256(
-                "3A78F382E8E2968EC201B33178102E06DB72E4F2D1505E058A4613C1E977825C"
+                "cd617c5c1b1ff1c94a52ab8cf07192654f271a3f8bad49490288131ccb9efc1e"
             )
             self.assertEqual(verdict["Verdict"], "Clean")
             self.assertEqual(
                 verdict["Sha256"].casefold(),
-                "3A78F382E8E2968EC201B33178102E06DB72E4F2D1505E058A4613C1E977825C".casefold(),
+                "cd617c5c1b1ff1c94a52ab8cf07192654f271a3f8bad49490288131ccb9efc1e".casefold(),
             )
 
     async def test_use_for_sha256_when_connection_already_closed(self):
         authenticator = ClientCredentialsGrantAuthenticator(
             CLIENT_ID, CLIENT_SECRET, TOKEN_URL, SSL_VERIFICATION
         )
         vaas = Vaas(tracing=VaasTracing(), options=VaasOptions(), url=VAAS_URL)
```

