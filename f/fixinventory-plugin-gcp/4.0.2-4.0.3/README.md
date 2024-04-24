# Comparing `tmp/fixinventory-plugin-gcp-4.0.2.tar.gz` & `tmp/fixinventory_plugin_gcp-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventory-plugin-gcp-4.0.2.tar", last modified: Fri Apr 12 12:19:21 2024, max compression
+gzip compressed data, was "fixinventory_plugin_gcp-4.0.3.tar", last modified: Wed Apr 24 10:34:02 2024, max compression
```

## Comparing `fixinventory-plugin-gcp-4.0.2.tar` & `fixinventory_plugin_gcp-4.0.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:19:21.084606 fixinventory-plugin-gcp-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-12 12:19:21.084606 fixinventory-plugin-gcp-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:19:21.080606 fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7564 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/gcp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:19:21.080606 fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25511 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    16036 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/resources/billing.py
--rw-r--r--   0 runner    (1001) docker     (127)   364421 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/resources/compute.py
--rw-r--r--   0 runner    (1001) docker     (127)    69260 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/resources/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    52716 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/resources/sqladmin.py
--rw-r--r--   0 runner    (1001) docker     (127)    20501 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/resources/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:19:21.084606 fixinventory-plugin-gcp-4.0.2/fixinventory_plugin_gcp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-12 12:19:21.000000 fixinventory-plugin-gcp-4.0.2/fixinventory_plugin_gcp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-12 12:19:21.000000 fixinventory-plugin-gcp-4.0.2/fixinventory_plugin_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:19:21.000000 fixinventory-plugin-gcp-4.0.2/fixinventory_plugin_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-12 12:19:21.000000 fixinventory-plugin-gcp-4.0.2/fixinventory_plugin_gcp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:15:33.000000 fixinventory-plugin-gcp-4.0.2/fixinventory_plugin_gcp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-12 12:19:21.000000 fixinventory-plugin-gcp-4.0.2/fixinventory_plugin_gcp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 12:19:21.000000 fixinventory-plugin-gcp-4.0.2/fixinventory_plugin_gcp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-12 12:19:21.084606 fixinventory-plugin-gcp-4.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:19:21.084606 fixinventory-plugin-gcp-4.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    12025 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/test/random_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/test/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/test/test_billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/test/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)    12951 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/test/test_compute.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/test/test_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/test/test_sqladmin.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-12 12:14:22.000000 fixinventory-plugin-gcp-4.0.2/test/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:34:02.220003 fixinventory_plugin_gcp-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 10:29:14.000000 fixinventory_plugin_gcp-4.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-24 10:34:02.220003 fixinventory_plugin_gcp-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-24 10:29:14.000000 fixinventory_plugin_gcp-4.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:34:02.212003 fixinventory_plugin_gcp-4.0.3/fix_plugin_gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-04-24 10:29:14.000000 fixinventory_plugin_gcp-4.0.3/fix_plugin_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-04-24 10:29:14.000000 fixinventory_plugin_gcp-4.0.3/fix_plugin_gcp/collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-24 10:29:14.000000 fixinventory_plugin_gcp-4.0.3/fix_plugin_gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7564 2024-04-24 10:29:14.000000 fixinventory_plugin_gcp-4.0.3/fix_plugin_gcp/gcp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:34:02.216003 fixinventory_plugin_gcp-4.0.3/fix_plugin_gcp/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:29:14.000000 fixinventory_plugin_gcp-4.0.3/fix_plugin_gcp/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25931 2024-04-24 10:29:14.000000 fixinventory_plugin_gcp-4.0.3/fix_plugin_gcp/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16036 2024-04-24 10:29:14.000000 fixinventory_plugin_gcp-4.0.3/fix_plugin_gcp/resources/billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)   364421 2024-04-24 10:29:14.000000 fixinventory_plugin_gcp-4.0.3/fix_plugin_gcp/resources/compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69260 2024-04-24 10:29:14.000000 fixinventory_plugin_gcp-4.0.3/fix_plugin_gcp/resources/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52716 2024-04-24 10:29:14.000000 fixinventory_plugin_gcp-4.0.3/fix_plugin_gcp/resources/sqladmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20501 2024-04-24 10:29:14.000000 fixinventory_plugin_gcp-4.0.3/fix_plugin_gcp/resources/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-04-24 10:29:14.000000 fixinventory_plugin_gcp-4.0.3/fix_plugin_gcp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:34:02.220003 fixinventory_plugin_gcp-4.0.3/fixinventory_plugin_gcp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-24 10:34:02.000000 fixinventory_plugin_gcp-4.0.3/fixinventory_plugin_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-24 10:34:02.000000 fixinventory_plugin_gcp-4.0.3/fixinventory_plugin_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:34:02.000000 fixinventory_plugin_gcp-4.0.3/fixinventory_plugin_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-24 10:34:02.000000 fixinventory_plugin_gcp-4.0.3/fixinventory_plugin_gcp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:30:18.000000 fixinventory_plugin_gcp-4.0.3/fixinventory_plugin_gcp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-24 10:34:02.000000 fixinventory_plugin_gcp-4.0.3/fixinventory_plugin_gcp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-24 10:34:02.000000 fixinventory_plugin_gcp-4.0.3/fixinventory_plugin_gcp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-24 10:29:14.000000 fixinventory_plugin_gcp-4.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-24 10:34:02.220003 fixinventory_plugin_gcp-4.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:34:02.220003 fixinventory_plugin_gcp-4.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:29:14.000000 fixinventory_plugin_gcp-4.0.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-24 10:29:14.000000 fixinventory_plugin_gcp-4.0.3/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12025 2024-04-24 10:29:14.000000 fixinventory_plugin_gcp-4.0.3/test/random_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-24 10:29:14.000000 fixinventory_plugin_gcp-4.0.3/test/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-24 10:29:14.000000 fixinventory_plugin_gcp-4.0.3/test/test_billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-24 10:29:14.000000 fixinventory_plugin_gcp-4.0.3/test/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12951 2024-04-24 10:29:14.000000 fixinventory_plugin_gcp-4.0.3/test/test_compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-24 10:29:14.000000 fixinventory_plugin_gcp-4.0.3/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-24 10:29:14.000000 fixinventory_plugin_gcp-4.0.3/test/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-24 10:29:14.000000 fixinventory_plugin_gcp-4.0.3/test/test_sqladmin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-24 10:29:14.000000 fixinventory_plugin_gcp-4.0.3/test/test_storage.py
```

### Comparing `fixinventory-plugin-gcp-4.0.2/PKG-INFO` & `fixinventory_plugin_gcp-4.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-gcp
-Version: 4.0.2
+Version: 4.0.3
 Summary: Fix GCP Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/gcp
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
@@ -15,15 +15,16 @@
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: fixinventorylib==4.0.2
+Requires-Dist: fixinventorylib==4.0.3
+Requires-Dist: fixinventorydata
 Requires-Dist: google-api-python-client
 Requires-Dist: oauth2client
 Requires-Dist: retrying
 Requires-Dist: tenacity
 
 # fix-plugin-gcp
 An GCP collector plugin for Fix.
```

### Comparing `fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/__init__.py` & `fixinventory_plugin_gcp-4.0.3/fix_plugin_gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/collector.py` & `fixinventory_plugin_gcp-4.0.3/fix_plugin_gcp/collector.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/config.py` & `fixinventory_plugin_gcp-4.0.3/fix_plugin_gcp/config.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/gcp_client.py` & `fixinventory_plugin_gcp-4.0.3/fix_plugin_gcp/gcp_client.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/resources/base.py` & `fixinventory_plugin_gcp-4.0.3/fix_plugin_gcp/resources/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from fixlib.config import Config
 from fixlib.core.actions import CoreFeedback
 from fixlib.graph import Graph, EdgeKey
 from fixlib.json import from_json as from_js, value_in_path
 from fixlib.json_bender import bend, Bender, S, Bend, MapDict, F
 from fixlib.threading import ExecutorQueue
 from fixlib.types import Json
+from fixinventorydata.cloud import regions as cloud_region_data
 
 log = logging.getLogger("fix.plugins.gcp")
 
 
 T = TypeVar("T")
 
 
@@ -520,14 +521,20 @@
     }
     reference_kinds: ClassVar[ModelReference] = {"successors": {"default": ["gcp_zone"]}}
     description: Optional[str] = field(default=None)
     status: Optional[str] = field(default=None)
     region_deprecated: Optional[GcpDeprecationStatus] = field(default=None)
     region_supports_pzs: Optional[bool] = field(default=None)
 
+    def __attrs_post_init__(self) -> None:
+        super().__attrs_post_init__()
+        self.long_name = cloud_region_data.get("gcp", {}).get(self.id, {}).get("long_name")
+        self.latitude = cloud_region_data.get("gcp", {}).get(self.id, {}).get("latitude")
+        self.longitude = cloud_region_data.get("gcp", {}).get(self.id, {}).get("longitude")
+
     @classmethod
     def fallback_global_region(cls: Type[GcpRegion], project: GcpProject) -> GcpRegion:
         return cls(id="global", tags={}, name="global", account=project)
 
     def post_process(self, graph_builder: GraphBuilder, source: Json) -> None:
         region_quota = GcpRegionQuota.from_api(source)
         graph_builder.add_node(region_quota, source)
```

### Comparing `fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/resources/billing.py` & `fixinventory_plugin_gcp-4.0.3/fix_plugin_gcp/resources/billing.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/resources/compute.py` & `fixinventory_plugin_gcp-4.0.3/fix_plugin_gcp/resources/compute.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/resources/container.py` & `fixinventory_plugin_gcp-4.0.3/fix_plugin_gcp/resources/container.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/resources/sqladmin.py` & `fixinventory_plugin_gcp-4.0.3/fix_plugin_gcp/resources/sqladmin.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/resources/storage.py` & `fixinventory_plugin_gcp-4.0.3/fix_plugin_gcp/resources/storage.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.2/fix_plugin_gcp/utils.py` & `fixinventory_plugin_gcp-4.0.3/fix_plugin_gcp/utils.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.2/fixinventory_plugin_gcp.egg-info/PKG-INFO` & `fixinventory_plugin_gcp-4.0.3/fixinventory_plugin_gcp.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-gcp
-Version: 4.0.2
+Version: 4.0.3
 Summary: Fix GCP Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/gcp
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
@@ -15,15 +15,16 @@
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: fixinventorylib==4.0.2
+Requires-Dist: fixinventorylib==4.0.3
+Requires-Dist: fixinventorydata
 Requires-Dist: google-api-python-client
 Requires-Dist: oauth2client
 Requires-Dist: retrying
 Requires-Dist: tenacity
 
 # fix-plugin-gcp
 An GCP collector plugin for Fix.
```

### Comparing `fixinventory-plugin-gcp-4.0.2/fixinventory_plugin_gcp.egg-info/SOURCES.txt` & `fixinventory_plugin_gcp-4.0.3/fixinventory_plugin_gcp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.2/pyproject.toml` & `fixinventory_plugin_gcp-4.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "fixinventory-plugin-gcp"
 description = "Fix GCP Collector Plugin"
-version = "4.0.2"
+version = "4.0.3"
 authors = [{name="Some Engineering Inc."}]
 license = { text="AGPLv3" }
 requires-python = ">=3.11"
 classifiers = [
     # Current project status
     "Development Status :: 5 - Production/Stable",
     # Audience
@@ -23,15 +23,16 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "fixinventorylib==4.0.2",
+    "fixinventorylib==4.0.3",
+    "fixinventorydata",
     "google-api-python-client",
     "oauth2client",
     "retrying",
     "tenacity",
 ]
 
 [project.entry-points."fix.plugins"]
```

### Comparing `fixinventory-plugin-gcp-4.0.2/test/conftest.py` & `fixinventory_plugin_gcp-4.0.3/test/conftest.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.2/test/random_client.py` & `fixinventory_plugin_gcp-4.0.3/test/random_client.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.2/test/test_base.py` & `fixinventory_plugin_gcp-4.0.3/test/test_base.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.2/test/test_billing.py` & `fixinventory_plugin_gcp-4.0.3/test/test_billing.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.2/test/test_collector.py` & `fixinventory_plugin_gcp-4.0.3/test/test_collector.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.2/test/test_compute.py` & `fixinventory_plugin_gcp-4.0.3/test/test_compute.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.2/test/test_config.py` & `fixinventory_plugin_gcp-4.0.3/test/test_config.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.2/test/test_container.py` & `fixinventory_plugin_gcp-4.0.3/test/test_container.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-gcp-4.0.2/test/test_sqladmin.py` & `fixinventory_plugin_gcp-4.0.3/test/test_sqladmin.py`

 * *Files identical despite different names*

