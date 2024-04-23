# Comparing `tmp/pytainer-0.0.2.tar.gz` & `tmp/pytainer-0.0.3.tar.gz`

## Comparing `pytainer-0.0.2.tar` & `pytainer-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytainer-0.0.2/__init__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pytainer-0.0.2/requirements.txt
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pytainer-0.0.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pytainer-0.0.2/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytainer-0.0.2/pytainer/__about__.py
--rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 pytainer-0.0.2/pytainer/__init__.py
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 pytainer-0.0.2/pytainer/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytainer-0.0.2/pytainer/models/__init__.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 pytainer-0.0.2/pytainer/models/gittypes.py
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 pytainer-0.0.2/pytainer/models/portainer.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pytainer-0.0.2/scripts/docker-compose.example.yml
--rwxr-xr-x   0        0        0      296 2020-02-02 00:00:00.000000 pytainer-0.0.2/scripts/run_portainer_ce.sh
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 pytainer-0.0.2/tests/test_pytainer.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 pytainer-0.0.2/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pytainer-0.0.2/LICENSE
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pytainer-0.0.2/README.md
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 pytainer-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 pytainer-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytainer-0.0.3/__init__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pytainer-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pytainer-0.0.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pytainer-0.0.3/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytainer-0.0.3/pytainer/__about__.py
+-rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 pytainer-0.0.3/pytainer/__init__.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 pytainer-0.0.3/pytainer/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytainer-0.0.3/pytainer/models/__init__.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 pytainer-0.0.3/pytainer/models/gittypes.py
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 pytainer-0.0.3/pytainer/models/portainer.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 pytainer-0.0.3/scripts/docker-compose.example.yml
+-rwxr-xr-x   0        0        0      296 2020-02-02 00:00:00.000000 pytainer-0.0.3/scripts/run_portainer_ce.sh
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 pytainer-0.0.3/tests/test_pytainer.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 pytainer-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pytainer-0.0.3/LICENSE
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pytainer-0.0.3/README.md
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 pytainer-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 pytainer-0.0.3/PKG-INFO
```

### Comparing `pytainer-0.0.2/.github/workflows/publish.yml` & `pytainer-0.0.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pytainer-0.0.2/pytainer/__init__.py` & `pytainer-0.0.3/pytainer/__init__.py`

 * *Files identical despite different names*

### Comparing `pytainer-0.0.2/pytainer/cli.py` & `pytainer-0.0.3/pytainer/cli.py`

 * *Files identical despite different names*

### Comparing `pytainer-0.0.2/pytainer/models/portainer.py` & `pytainer-0.0.3/pytainer/models/portainer.py`

 * *Files identical despite different names*

### Comparing `pytainer-0.0.2/tests/test_pytainer.py` & `pytainer-0.0.3/tests/test_pytainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import httpx
 from pytest_httpx import HTTPXMock
 
-from pytainer.pytainer import Pytainer
+from pytainer import Pytainer
 from pytainer.models.portainer import AuthAuthenticateResponse, SystemInfoResponse
 
 
 def test_portainer_init():
     portainer = Pytainer(
         base_url="https://portainer.test/", api_token="debug-auth-token"
     )
```

### Comparing `pytainer-0.0.2/.gitignore` & `pytainer-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pytainer-0.0.2/LICENSE` & `pytainer-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytainer-0.0.2/pyproject.toml` & `pytainer-0.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "pytainer"
 description = ""
 readme = "README.md"
 requires-python = ">=3.9"
 license = "MIT"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name = "Krzysztof Myjak"},
 ]
 classifiers = [
     "Intended Audience :: Information Technology",
     "Intended Audience :: System Administrators",
     "Operating System :: OS Independent",
```

### Comparing `pytainer-0.0.2/PKG-INFO` & `pytainer-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pytainer
-Version: 0.0.2
+Version: 0.0.3
 Author: Krzysztof Myjak
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
```

