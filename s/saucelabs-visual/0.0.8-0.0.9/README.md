# Comparing `tmp/saucelabs_visual-0.0.8.tar.gz` & `tmp/saucelabs_visual-0.0.9.tar.gz`

## Comparing `saucelabs_visual-0.0.8.tar` & `saucelabs_visual-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.8/requirements.txt
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.8/requirements/build.txt
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.8/requirements/dev.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.8/requirements/user.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.8/src/saucelabs_visual/__init__.py
--rw-r--r--   0        0        0     9389 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.8/src/saucelabs_visual/client.py
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.8/src/saucelabs_visual/regions.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.8/src/saucelabs_visual/typing.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.8/src/saucelabs_visual/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.8/src/saucelabs_visual/frameworks/__init__.py
--rw-r--r--   0        0        0     7705 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.8/src/saucelabs_visual/frameworks/robot.py
--rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.8/.gitignore
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.8/README.md
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.9/requirements.txt
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.9/requirements/build.txt
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.9/requirements/dev.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.9/requirements/user.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.9/src/saucelabs_visual/__init__.py
+-rw-r--r--   0        0        0     9414 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.9/src/saucelabs_visual/client.py
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.9/src/saucelabs_visual/regions.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.9/src/saucelabs_visual/typing.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.9/src/saucelabs_visual/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.9/src/saucelabs_visual/frameworks/__init__.py
+-rw-r--r--   0        0        0     8673 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.9/src/saucelabs_visual/frameworks/robot.py
+-rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.9/.gitignore
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.9/README.md
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 saucelabs_visual-0.0.9/PKG-INFO
```

### Comparing `saucelabs_visual-0.0.8/src/saucelabs_visual/client.py` & `saucelabs_visual-0.0.9/src/saucelabs_visual/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,40 +8,40 @@
 from requests.auth import HTTPBasicAuth
 
 from saucelabs_visual.regions import Region
 from saucelabs_visual.typing import IgnoreRegion, FullPageConfig, DiffingMethod, BuildStatus
 
 
 class SauceLabsVisual:
-    client: Client = None
+    _client: Client = None
     build_id: Union[str, None] = None
     build_url: Union[str, None] = None
     meta_cache: dict = {}
     region: Region = None
 
-    def __init__(self):
-        self._create_client()
+    @property
+    def client(self):
+        if self._client is None:
+            self._client = self._create_client()
+        return self._client
 
     def _create_client(self):
         username = environ.get("SAUCE_USERNAME")
         access_key = environ.get("SAUCE_ACCESS_KEY")
 
         if username is None or access_key is None:
-            raise Exception(
+            raise RuntimeError(
                 'Sauce Labs credentials not set. Please check that you set correctly your '
                 '`SAUCE_USERNAME` and `SAUCE_ACCESS_KEY` environment variables.'
             )
 
         self.region = Region.from_name(environ.get("SAUCE_REGION") or 'us-west-1')
         region_url = self.region.graphql_endpoint
         transport = RequestsHTTPTransport(url=region_url, auth=HTTPBasicAuth(username, access_key))
-        self.client = Client(transport=transport, execute_timeout=90)
-
-    def get_client(self) -> Client:
-        return self.client
+        return Client(transport=transport, execute_timeout=90)
 
     def create_build(
             self,
             name: Union[str, None] = environ.get('SAUCE_VISUAL_BUILD_NAME'),
             project: Union[str, None] = environ.get('SAUCE_VISUAL_PROJECT'),
             branch: Union[str, None] = environ.get('SAUCE_VISUAL_BRANCH'),
             default_branch: Union[str, None] = environ.get('SAUCE_VISUAL_DEFAULT_BRANCH'),
```

### Comparing `saucelabs_visual-0.0.8/src/saucelabs_visual/regions.py` & `saucelabs_visual-0.0.9/src/saucelabs_visual/regions.py`

 * *Files identical despite different names*

### Comparing `saucelabs_visual-0.0.8/src/saucelabs_visual/typing.py` & `saucelabs_visual-0.0.9/src/saucelabs_visual/typing.py`

 * *Files identical despite different names*

### Comparing `saucelabs_visual-0.0.8/src/saucelabs_visual/utils.py` & `saucelabs_visual-0.0.9/src/saucelabs_visual/utils.py`

 * *Files identical despite different names*

### Comparing `saucelabs_visual-0.0.8/src/saucelabs_visual/frameworks/robot.py` & `saucelabs_visual-0.0.9/src/saucelabs_visual/frameworks/robot.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,21 +12,44 @@
 from saucelabs_visual.typing import IgnoreRegion, FullPageConfig, DiffingMethod
 from saucelabs_visual.utils import ignore_region_from_dict, is_valid_ignore_region, \
     create_table_from_build_status, is_build_errored, is_build_failed
 
 
 @library(scope='GLOBAL')
 class SauceLabsVisual:
-    client: Client = None
+    _client: Client = None
+    selenium_library_key: Union[str, None] = None
 
-    def __init__(self):
-        self.client = Client()
+    @property
+    def client(self):
+        if self._client is None:
+            self._client = Client()
+        return self._client
 
     def _get_selenium_library(self) -> SeleniumLibrary:
-        return BuiltIn().get_library_instance('SeleniumLibrary')
+        all_libraries: dict = BuiltIn().get_library_instance(all=True)
+
+        # SeleniumLibrary may be imported under another name if an alias is provided -- ex:
+        #
+        # Library           SeleniumLibrary    AS    slib
+        #
+        # Instead of importing by static name, we'll get all imported libraries and iterate over
+        # them to find the instance of SeleniumLibrary and cache that key.
+        if self.selenium_library_key is None:
+            for key, value in all_libraries.items():
+                if type(value) is SeleniumLibrary:
+                    self.selenium_library_key = key
+                    break
+
+        if self.selenium_library_key is None:
+            raise RuntimeError(
+                'SeleniumLibrary instance not found in Robot. Is it imported in your project?'
+            )
+
+        return BuiltIn().get_library_instance(self.selenium_library_key)
 
     def _get_selenium_id(self) -> str:
         return self._get_selenium_library().get_session_id()
 
     def _parse_full_page_config(self, value: str) -> Union[FullPageConfig, None]:
         """
         Parses the value from the 'Visual Snapshot' keyword to allow optional values and defaults
```

### Comparing `saucelabs_visual-0.0.8/.gitignore` & `saucelabs_visual-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `saucelabs_visual-0.0.8/pyproject.toml` & `saucelabs_visual-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "saucelabs_visual"
-version = "0.0.8"
+version = "0.0.9"
 description = "Python bindings for Sauce Labs Visual"
 dependencies=[
     "requests",
     "requests-toolbelt",
     "gql",
     "tabulate",
 ]
```

### Comparing `saucelabs_visual-0.0.8/PKG-INFO` & `saucelabs_visual-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: saucelabs_visual
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python bindings for Sauce Labs Visual
 Project-URL: Homepage, https://github.com/saucelabs/visual-sdks/tree/main/visual-python
 Project-URL: Issues, https://github.com/saucelabs/visual-sdks/issues
 Requires-Dist: gql
 Requires-Dist: requests
 Requires-Dist: requests-toolbelt
 Requires-Dist: tabulate
```

