# Comparing `tmp/anaconda_cloud_auth-0.5.0.tar.gz` & `tmp/anaconda_cloud_auth-0.5.1.tar.gz`

## Comparing `anaconda_cloud_auth-0.5.0.tar` & `anaconda_cloud_auth-0.5.1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/Makefile
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/environment-dev.yml
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/_version.py
--rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/actions.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/cli.py
--rw-r--r--   0        0        0     7913 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/client.py
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/config.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/console.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/exceptions.py
--rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/handlers.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/jwt.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/panel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/py.typed
--rw-r--r--   0        0        0     9118 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/token.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/_conda/__init__.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/_conda/auth_handler.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/_conda/plugins.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0     8708 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/tests/conftest.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/tests/mock-cert.csr
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/tests/mock-cert.key
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/tests/mock-cert.pem
--rw-r--r--   0        0        0     5856 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/tests/test_auth.py
--rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/tests/test_client.py
--rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/tests/test_conda_plugins.py
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/tests/test_config.py
--rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/tests/test_handler.py
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/tests/test_token.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/.gitignore
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/LICENSE
--rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/README.md
--rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/Makefile
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/environment-dev.yml
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/src/anaconda_cloud_auth/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/src/anaconda_cloud_auth/_version.py
+-rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/src/anaconda_cloud_auth/actions.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/src/anaconda_cloud_auth/cli.py
+-rw-r--r--   0        0        0     7913 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/src/anaconda_cloud_auth/client.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/src/anaconda_cloud_auth/config.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/src/anaconda_cloud_auth/console.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/src/anaconda_cloud_auth/exceptions.py
+-rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/src/anaconda_cloud_auth/handlers.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/src/anaconda_cloud_auth/jwt.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/src/anaconda_cloud_auth/panel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/src/anaconda_cloud_auth/py.typed
+-rw-r--r--   0        0        0     9118 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/src/anaconda_cloud_auth/token.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/src/anaconda_cloud_auth/_conda/__init__.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/src/anaconda_cloud_auth/_conda/auth_handler.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/src/anaconda_cloud_auth/_conda/entrypoint.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/src/anaconda_cloud_auth/_conda/plugins.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/tests/__init__.py
+-rw-r--r--   0        0        0     8708 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/tests/conftest.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/tests/mock-cert.csr
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/tests/mock-cert.key
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/tests/mock-cert.pem
+-rw-r--r--   0        0        0     5856 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/tests/test_auth.py
+-rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/tests/test_client.py
+-rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/tests/test_conda_plugins.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/tests/test_config.py
+-rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/tests/test_handler.py
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/tests/test_token.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/.gitignore
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/LICENSE
+-rw-r--r--   0        0        0     9148 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/README.md
+-rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0    10092 2020-02-02 00:00:00.000000 anaconda_cloud_auth-0.5.1/PKG-INFO
```

### Comparing `anaconda_cloud_auth-0.5.0/Makefile` & `anaconda_cloud_auth-0.5.1/Makefile`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/actions.py` & `anaconda_cloud_auth-0.5.1/src/anaconda_cloud_auth/actions.py`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/client.py` & `anaconda_cloud_auth-0.5.1/src/anaconda_cloud_auth/client.py`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/config.py` & `anaconda_cloud_auth-0.5.1/src/anaconda_cloud_auth/config.py`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/console.py` & `anaconda_cloud_auth-0.5.1/src/anaconda_cloud_auth/console.py`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/handlers.py` & `anaconda_cloud_auth-0.5.1/src/anaconda_cloud_auth/handlers.py`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/jwt.py` & `anaconda_cloud_auth-0.5.1/src/anaconda_cloud_auth/jwt.py`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/panel.py` & `anaconda_cloud_auth-0.5.1/src/anaconda_cloud_auth/panel.py`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/token.py` & `anaconda_cloud_auth-0.5.1/src/anaconda_cloud_auth/token.py`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/_conda/__init__.py` & `anaconda_cloud_auth-0.5.1/src/anaconda_cloud_auth/_conda/__init__.py`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/_conda/auth_handler.py` & `anaconda_cloud_auth-0.5.1/src/anaconda_cloud_auth/_conda/auth_handler.py`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.5.0/src/anaconda_cloud_auth/_conda/plugins.py` & `anaconda_cloud_auth-0.5.1/src/anaconda_cloud_auth/_conda/plugins.py`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.5.0/tests/conftest.py` & `anaconda_cloud_auth-0.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.5.0/tests/mock-cert.csr` & `anaconda_cloud_auth-0.5.1/tests/mock-cert.csr`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.5.0/tests/mock-cert.key` & `anaconda_cloud_auth-0.5.1/tests/mock-cert.key`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.5.0/tests/mock-cert.pem` & `anaconda_cloud_auth-0.5.1/tests/mock-cert.pem`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.5.0/tests/test_auth.py` & `anaconda_cloud_auth-0.5.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.5.0/tests/test_client.py` & `anaconda_cloud_auth-0.5.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.5.0/tests/test_conda_plugins.py` & `anaconda_cloud_auth-0.5.1/tests/test_conda_plugins.py`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.5.0/tests/test_config.py` & `anaconda_cloud_auth-0.5.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.5.0/tests/test_handler.py` & `anaconda_cloud_auth-0.5.1/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.5.0/tests/test_token.py` & `anaconda_cloud_auth-0.5.1/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.5.0/.gitignore` & `anaconda_cloud_auth-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.5.0/LICENSE` & `anaconda_cloud_auth-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.5.0/README.md` & `anaconda_cloud_auth-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `anaconda_cloud_auth-0.5.0/pyproject.toml` & `anaconda_cloud_auth-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 dynamic = ["version"]
 license = {text = "BSD-3-Clause"}
 name = "anaconda-cloud-auth"
 readme = "README.md"
 requires-python = ">=3.8"
 
 [project.entry-points.conda]
-anaconda-cloud-auth = "anaconda_cloud_auth._conda.plugins"
+anaconda-cloud-auth = "anaconda_cloud_auth._conda.entrypoint"
 
 [project.entry-points."panel.auth"]
 anaconda_cloud = "anaconda_cloud_auth.panel:AnacondaCloudLoginHandler"
 
 [project.optional-dependencies]
 cli = ["anaconda-cloud-cli"]
 dev = [
```

### Comparing `anaconda_cloud_auth-0.5.0/PKG-INFO` & `anaconda_cloud_auth-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: anaconda-cloud-auth
-Version: 0.5.0
+Version: 0.5.1
 Summary: A client auth library for Anaconda.cloud APIs
 License: BSD-3-Clause
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: cryptography>=3.4.0
 Requires-Dist: keyring
 Requires-Dist: pkce
```

