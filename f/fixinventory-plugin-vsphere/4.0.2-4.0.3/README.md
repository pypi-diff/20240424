# Comparing `tmp/fixinventory-plugin-vsphere-4.0.2.tar.gz` & `tmp/fixinventory_plugin_vsphere-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventory-plugin-vsphere-4.0.2.tar", last modified: Fri Apr 12 12:17:14 2024, max compression
+gzip compressed data, was "fixinventory_plugin_vsphere-4.0.3.tar", last modified: Wed Apr 24 10:32:26 2024, max compression
```

## Comparing `fixinventory-plugin-vsphere-4.0.2.tar` & `fixinventory_plugin_vsphere-4.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:14.151716 fixinventory-plugin-vsphere-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-04-12 12:14:21.000000 fixinventory-plugin-vsphere-4.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 12:14:21.000000 fixinventory-plugin-vsphere-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13505 2024-04-12 12:17:14.151716 fixinventory-plugin-vsphere-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-12 12:14:21.000000 fixinventory-plugin-vsphere-4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:14.147716 fixinventory-plugin-vsphere-4.0.2/fix_plugin_vsphere/
--rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-04-12 12:14:21.000000 fixinventory-plugin-vsphere-4.0.2/fix_plugin_vsphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-12 12:14:21.000000 fixinventory-plugin-vsphere-4.0.2/fix_plugin_vsphere/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-04-12 12:14:21.000000 fixinventory-plugin-vsphere-4.0.2/fix_plugin_vsphere/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-12 12:14:21.000000 fixinventory-plugin-vsphere-4.0.2/fix_plugin_vsphere/vsphere_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:14.147716 fixinventory-plugin-vsphere-4.0.2/fixinventory_plugin_vsphere.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13505 2024-04-12 12:17:14.000000 fixinventory-plugin-vsphere-4.0.2/fixinventory_plugin_vsphere.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-12 12:17:14.000000 fixinventory-plugin-vsphere-4.0.2/fixinventory_plugin_vsphere.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:17:14.000000 fixinventory-plugin-vsphere-4.0.2/fixinventory_plugin_vsphere.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-12 12:17:14.000000 fixinventory-plugin-vsphere-4.0.2/fixinventory_plugin_vsphere.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:15:27.000000 fixinventory-plugin-vsphere-4.0.2/fixinventory_plugin_vsphere.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-12 12:17:14.000000 fixinventory-plugin-vsphere-4.0.2/fixinventory_plugin_vsphere.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 12:17:14.000000 fixinventory-plugin-vsphere-4.0.2/fixinventory_plugin_vsphere.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-12 12:14:21.000000 fixinventory-plugin-vsphere-4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-12 12:17:14.151716 fixinventory-plugin-vsphere-4.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:14.147716 fixinventory-plugin-vsphere-4.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-12 12:14:21.000000 fixinventory-plugin-vsphere-4.0.2/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:26.068427 fixinventory_plugin_vsphere-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-04-24 10:29:19.000000 fixinventory_plugin_vsphere-4.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 10:29:19.000000 fixinventory_plugin_vsphere-4.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13505 2024-04-24 10:32:26.068427 fixinventory_plugin_vsphere-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-24 10:29:19.000000 fixinventory_plugin_vsphere-4.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:26.064427 fixinventory_plugin_vsphere-4.0.3/fix_plugin_vsphere/
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-04-24 10:29:19.000000 fixinventory_plugin_vsphere-4.0.3/fix_plugin_vsphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-24 10:29:19.000000 fixinventory_plugin_vsphere-4.0.3/fix_plugin_vsphere/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-04-24 10:29:19.000000 fixinventory_plugin_vsphere-4.0.3/fix_plugin_vsphere/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-24 10:29:19.000000 fixinventory_plugin_vsphere-4.0.3/fix_plugin_vsphere/vsphere_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:26.068427 fixinventory_plugin_vsphere-4.0.3/fixinventory_plugin_vsphere.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13505 2024-04-24 10:32:26.000000 fixinventory_plugin_vsphere-4.0.3/fixinventory_plugin_vsphere.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-24 10:32:26.000000 fixinventory_plugin_vsphere-4.0.3/fixinventory_plugin_vsphere.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:32:26.000000 fixinventory_plugin_vsphere-4.0.3/fixinventory_plugin_vsphere.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-24 10:32:26.000000 fixinventory_plugin_vsphere-4.0.3/fixinventory_plugin_vsphere.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:30:34.000000 fixinventory_plugin_vsphere-4.0.3/fixinventory_plugin_vsphere.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-24 10:32:26.000000 fixinventory_plugin_vsphere-4.0.3/fixinventory_plugin_vsphere.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-24 10:32:26.000000 fixinventory_plugin_vsphere-4.0.3/fixinventory_plugin_vsphere.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-24 10:29:19.000000 fixinventory_plugin_vsphere-4.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 10:32:26.068427 fixinventory_plugin_vsphere-4.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:32:26.068427 fixinventory_plugin_vsphere-4.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-24 10:29:19.000000 fixinventory_plugin_vsphere-4.0.3/test/test_config.py
```

### Comparing `fixinventory-plugin-vsphere-4.0.2/LICENSE` & `fixinventory_plugin_vsphere-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-vsphere-4.0.2/PKG-INFO` & `fixinventory_plugin_vsphere-4.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-vsphere
-Version: 4.0.2
+Version: 4.0.3
 Summary: Fix VSphere Collector Plugin
 Author: Some Engineering Inc.
 License: 
                                       Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
@@ -217,15 +217,15 @@
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: fixinventorylib==4.0.2
+Requires-Dist: fixinventorylib==4.0.3
 Requires-Dist: pyvmomi
 
 # fix-plugin-vsphere
 VMWare VSphere Collector Plugin for Fix (Alpha)
 
 ## License
 See [LICENSE](../../LICENSE) for details.
```

### Comparing `fixinventory-plugin-vsphere-4.0.2/fix_plugin_vsphere/__init__.py` & `fixinventory_plugin_vsphere-4.0.3/fix_plugin_vsphere/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,14 +144,30 @@
                 self.graph.add_resource(dcObj, clusterObj)
                 try:
                     rpool = cluster.resourcePool
                     self.resource_pool(rpool, clusterObj)
                 except Exception:
                     log.warning(f"Resourcepool error for cluster {cluster._moId} {cluster.name}")
 
+                # get hosts from a cluster
+                for host in cluster.host:  #
+                    log.debug(f"Found host - {host._moId} - {host.name}")
+                    hostObj = VSphereESXiHost(id=host._moId, name=host.name)
+                    self.graph.add_resource(clusterObj, hostObj)
+                    # get vms for each host and read from the vm list
+                    for vm in host.vm:
+                        if vm._moId in self.instances_dict:
+                            vmObj = self.instances_dict[vm._moId]
+                            log.debug(
+                                f"lookup vm - {vm._moId} - {vmObj.name} and assign to host {host._moId} - {host.name}"
+                            )
+                            self.graph.add_edge(hostObj, vmObj)
+                        else:
+                            log.warning(f"host {host._moId} - {host.name} reports {vm._moId} but instance not found")
+
             for datastore in dc.datastoreFolder.childEntity:
                 if datastore._wsdlName == "Datastore":
                     log.debug(f"Found Datastore - {datastore._moId} - {datastore.name}")
                     dsObj = VSphereDataStore(id=datastore._moId, name=datastore.name)
                     self.graph.add_resource(dcObj, dsObj)
                     for vm in datastore.vm:
                         vmObj = self.instances_dict[vm._moId]
@@ -165,26 +181,10 @@
                         if store._wsdlName == "Datastore":
                             dsObj = VSphereDataStore(id=store._moId, name=store.name)
                             self.graph.add_resource(dcObj, dsObj)
                             for vm in store.vm:
                                 vmObj = self.instances_dict[vm._moId]
                                 self.graph.add_edge(dsObj, vmObj)
 
-            # get hosts from a cluster
-            for host in cluster.host:  #
-                log.debug(f"Found host - {host._moId} - {host.name}")
-                hostObj = VSphereESXiHost(id=host._moId, name=host.name)
-                self.graph.add_resource(clusterObj, hostObj)
-                # get vms for each host and read from the vm list
-                for vm in host.vm:
-                    if vm._moId in self.instances_dict:
-                        vmObj = self.instances_dict[vm._moId]
-                        log.debug(
-                            f"lookup vm - {vm._moId} - {vmObj.name} and assign to host {host._moId} - {host.name}"
-                        )
-                        self.graph.add_edge(hostObj, vmObj)
-                    else:
-                        log.warning(f"host {host._moId} - {host.name} reports {vm._moId} but instance not found")
-
     @staticmethod
     def add_config(config: Config) -> None:
         config.add_config(VSphereConfig)
```

### Comparing `fixinventory-plugin-vsphere-4.0.2/fix_plugin_vsphere/config.py` & `fixinventory_plugin_vsphere-4.0.3/fix_plugin_vsphere/config.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-vsphere-4.0.2/fix_plugin_vsphere/resources.py` & `fixinventory_plugin_vsphere-4.0.3/fix_plugin_vsphere/resources.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-vsphere-4.0.2/fix_plugin_vsphere/vsphere_client.py` & `fixinventory_plugin_vsphere-4.0.3/fix_plugin_vsphere/vsphere_client.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-vsphere-4.0.2/fixinventory_plugin_vsphere.egg-info/PKG-INFO` & `fixinventory_plugin_vsphere-4.0.3/fixinventory_plugin_vsphere.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-vsphere
-Version: 4.0.2
+Version: 4.0.3
 Summary: Fix VSphere Collector Plugin
 Author: Some Engineering Inc.
 License: 
                                       Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
@@ -217,15 +217,15 @@
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: fixinventorylib==4.0.2
+Requires-Dist: fixinventorylib==4.0.3
 Requires-Dist: pyvmomi
 
 # fix-plugin-vsphere
 VMWare VSphere Collector Plugin for Fix (Alpha)
 
 ## License
 See [LICENSE](../../LICENSE) for details.
```

### Comparing `fixinventory-plugin-vsphere-4.0.2/fixinventory_plugin_vsphere.egg-info/SOURCES.txt` & `fixinventory_plugin_vsphere-4.0.3/fixinventory_plugin_vsphere.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-vsphere-4.0.2/pyproject.toml` & `fixinventory_plugin_vsphere-4.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "fixinventory-plugin-vsphere"
 description = "Fix VSphere Collector Plugin"
-version = "4.0.2"
+version = "4.0.3"
 authors = [{name="Some Engineering Inc."}]
 license = {file="LICENSE"}
 requires-python = ">=3.11"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
     # Audience
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "fixinventorylib==4.0.2",
+    "fixinventorylib==4.0.3",
     "pyvmomi",
 ]
 
 [project.entry-points."fix.plugins"]
 vsphere = "fix_plugin_vsphere:VSphereCollectorPlugin"
 
 [project.urls]
```

