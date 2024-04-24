# Comparing `tmp/mojo_credentials-1.3.3.tar.gz` & `tmp/mojo_credentials-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_credentials-1.3.3.tar", max compression
+gzip compressed data, was "mojo_credentials-1.3.4.tar", max compression
```

## Comparing `mojo_credentials-1.3.3.tar` & `mojo_credentials-1.3.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1083 2024-01-26 02:55:48.527481 mojo_credentials-1.3.3/LICENSE.txt
--rw-r--r--   0        0        0      811 2024-01-26 02:55:48.527658 mojo_credentials-1.3.3/README.rst
--rw-r--r--   0        0        0      674 2024-04-05 03:43:56.366778 mojo_credentials-1.3.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-26 02:55:48.529247 mojo_credentials-1.3.3/source/packages/mojo/credentials/__init__.py
--rw-r--r--   0        0        0     3308 2024-01-26 02:55:48.529375 mojo_credentials-1.3.3/source/packages/mojo/credentials/azureclientsecretcredential.py
--rw-r--r--   0        0        0     1906 2024-01-26 02:55:48.529507 mojo_credentials-1.3.3/source/packages/mojo/credentials/basecredential.py
--rw-r--r--   0        0        0     3224 2024-01-26 02:55:48.529591 mojo_credentials-1.3.3/source/packages/mojo/credentials/basiccredential.py
--rw-r--r--   0        0        0     9472 2024-04-05 03:43:50.656225 mojo_credentials-1.3.3/source/packages/mojo/credentials/credentialmanager.py
--rw-r--r--   0        0        0     5478 2024-01-26 02:55:48.529790 mojo_credentials-1.3.3/source/packages/mojo/credentials/sshcredential.py
--rw-r--r--   0        0        0     3324 2024-01-26 02:55:48.529980 mojo_credentials-1.3.3/source/packages/mojo/credentials/wifichoicecredential.py
--rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 mojo_credentials-1.3.3/setup.py
--rw-r--r--   0        0        0     1457 1970-01-01 00:00:00.000000 mojo_credentials-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-01-26 02:55:48.527481 mojo_credentials-1.3.4/LICENSE.txt
+-rw-r--r--   0        0        0      811 2024-01-26 02:55:48.527658 mojo_credentials-1.3.4/README.rst
+-rw-r--r--   0        0        0      674 2024-04-24 03:53:49.663267 mojo_credentials-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-26 02:55:48.529247 mojo_credentials-1.3.4/source/packages/mojo/credentials/__init__.py
+-rw-r--r--   0        0        0     3308 2024-01-26 02:55:48.529375 mojo_credentials-1.3.4/source/packages/mojo/credentials/azureclientsecretcredential.py
+-rw-r--r--   0        0        0     1906 2024-01-26 02:55:48.529507 mojo_credentials-1.3.4/source/packages/mojo/credentials/basecredential.py
+-rw-r--r--   0        0        0     3224 2024-01-26 02:55:48.529591 mojo_credentials-1.3.4/source/packages/mojo/credentials/basiccredential.py
+-rw-r--r--   0        0        0     9472 2024-04-05 03:43:50.656225 mojo_credentials-1.3.4/source/packages/mojo/credentials/credentialmanager.py
+-rw-r--r--   0        0        0     5478 2024-01-26 02:55:48.529790 mojo_credentials-1.3.4/source/packages/mojo/credentials/sshcredential.py
+-rw-r--r--   0        0        0     3324 2024-01-26 02:55:48.529980 mojo_credentials-1.3.4/source/packages/mojo/credentials/wifichoicecredential.py
+-rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 mojo_credentials-1.3.4/setup.py
+-rw-r--r--   0        0        0     1457 1970-01-01 00:00:00.000000 mojo_credentials-1.3.4/PKG-INFO
```

### Comparing `mojo_credentials-1.3.3/LICENSE.txt` & `mojo_credentials-1.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mojo_credentials-1.3.3/README.rst` & `mojo_credentials-1.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `mojo_credentials-1.3.3/pyproject.toml` & `mojo_credentials-1.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mojo-credentials"
 description = "Automation Mojo Credentials Package"
-version = "1.3.3"
+version = "1.3.4"
 authors = []
 readme = "README.rst"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX"
```

### Comparing `mojo_credentials-1.3.3/source/packages/mojo/credentials/azureclientsecretcredential.py` & `mojo_credentials-1.3.4/source/packages/mojo/credentials/azureclientsecretcredential.py`

 * *Files identical despite different names*

### Comparing `mojo_credentials-1.3.3/source/packages/mojo/credentials/basecredential.py` & `mojo_credentials-1.3.4/source/packages/mojo/credentials/basecredential.py`

 * *Files identical despite different names*

### Comparing `mojo_credentials-1.3.3/source/packages/mojo/credentials/basiccredential.py` & `mojo_credentials-1.3.4/source/packages/mojo/credentials/basiccredential.py`

 * *Files identical despite different names*

### Comparing `mojo_credentials-1.3.3/source/packages/mojo/credentials/credentialmanager.py` & `mojo_credentials-1.3.4/source/packages/mojo/credentials/credentialmanager.py`

 * *Files identical despite different names*

### Comparing `mojo_credentials-1.3.3/source/packages/mojo/credentials/sshcredential.py` & `mojo_credentials-1.3.4/source/packages/mojo/credentials/sshcredential.py`

 * *Files identical despite different names*

### Comparing `mojo_credentials-1.3.3/source/packages/mojo/credentials/wifichoicecredential.py` & `mojo_credentials-1.3.4/source/packages/mojo/credentials/wifichoicecredential.py`

 * *Files identical despite different names*

### Comparing `mojo_credentials-1.3.3/setup.py` & `mojo_credentials-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['mojo', 'mojo.credentials']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'mojo-credentials',
-    'version': '1.3.3',
+    'version': '1.3.4',
     'description': 'Automation Mojo Credentials Package',
     'long_description': "=======================\nmojo-credentials\n=======================\nThis is a package used for managing different types of credentials.\n\n=================\nCode Organization\n=================\n* .vscode - Common tasks\n* development - This is where the runtime environment scripts are located\n* repository-setup - Scripts for homing your repository and to your checkout and machine setup\n* userguide - Where you put your user guide\n* source/packages - Put your root folder here 'source/packages/(root-module-folder)'\n* source/sphinx - This is the Sphinx documentation folder\n* workspaces - This is where you add VSCode workspaces templates and where workspaces show up when homed.\n\n==========\nReferences\n==========\n\n- `User Guide <userguide/userguide.rst>`\n- `Coding Standards <userguide/10-00-coding-standards.rst>`\n",
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mojo_credentials-1.3.3/PKG-INFO` & `mojo_credentials-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mojo-credentials
-Version: 1.3.3
+Version: 1.3.4
 Summary: Automation Mojo Credentials Package
 License: LICENSE.txt
 Keywords: python
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX
```

