# Comparing `tmp/wwpdb.utils.emdb-1.8.tar.gz` & `tmp/wwpdb_utils_emdb-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.utils.emdb-1.8.tar", last modified: Wed Apr 10 17:17:09 2024, max compression
+gzip compressed data, was "wwpdb_utils_emdb-1.8.1.tar", last modified: Wed Apr 24 16:17:20 2024, max compression
```

## Comparing `wwpdb.utils.emdb-1.8.tar` & `wwpdb_utils_emdb-1.8.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 17:17:09.298135 wwpdb.utils.emdb-1.8/
--rw-r--r--   0 vsts      (1001) docker     (127)      106 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)      958 2024-04-10 17:17:09.298135 wwpdb.utils.emdb-1.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-10 17:17:09.298135 wwpdb.utils.emdb-1.8/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2310 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 17:17:09.290135 wwpdb.utils.emdb-1.8/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 17:17:09.290135 wwpdb.utils.emdb-1.8/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 17:17:09.290135 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/
--rw-r--r--   0 vsts      (1001) docker     (127)      322 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/EmdbSchema.py
--rw-r--r--   0 vsts      (1001) docker     (127)      143 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 17:17:09.290135 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/atomcheck/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/atomcheck/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7031 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/atomcheck/atomcheck.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 17:17:09.290135 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/checkemupload/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/checkemupload/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16058 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/checkemupload/checkemupload.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 17:17:09.298135 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/cif_emdb_translator/
--rwxr-xr-x   0 vsts      (1001) docker     (127)      139 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/cif_emdb_translator/README.md
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/cif_emdb_translator/__init__.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)   676892 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py
--rw-r--r--   0 vsts      (1001) docker     (127)  2304974 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/cif_emdb_translator/emdb.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)     1196 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2490 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 17:17:09.298135 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/data/
--rw-r--r--   0 vsts      (1001) docker     (127)   221515 2024-04-10 17:16:08.000000 wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/data/emdb-v3.xsd
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 17:17:09.298135 wwpdb.utils.emdb-1.8/wwpdb.utils.emdb.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)      958 2024-04-10 17:17:09.000000 wwpdb.utils.emdb-1.8/wwpdb.utils.emdb.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      947 2024-04-10 17:17:09.000000 wwpdb.utils.emdb-1.8/wwpdb.utils.emdb.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-10 17:17:09.000000 wwpdb.utils.emdb-1.8/wwpdb.utils.emdb.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       87 2024-04-10 17:17:09.000000 wwpdb.utils.emdb-1.8/wwpdb.utils.emdb.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-10 17:16:52.000000 wwpdb.utils.emdb-1.8/wwpdb.utils.emdb.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      101 2024-04-10 17:17:09.000000 wwpdb.utils.emdb-1.8/wwpdb.utils.emdb.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-10 17:17:09.000000 wwpdb.utils.emdb-1.8/wwpdb.utils.emdb.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 16:17:20.121608 wwpdb_utils_emdb-1.8.1/
+-rw-r--r--   0 vsts      (1001) docker     (127)      106 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)      960 2024-04-24 16:17:20.121608 wwpdb_utils_emdb-1.8.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-24 16:17:20.121608 wwpdb_utils_emdb-1.8.1/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2310 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 16:17:20.113608 wwpdb_utils_emdb-1.8.1/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 16:17:20.117608 wwpdb_utils_emdb-1.8.1/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 16:17:20.117608 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)      322 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/EmdbSchema.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      145 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 16:17:20.117608 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/atomcheck/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/atomcheck/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7031 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/atomcheck/atomcheck.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 16:17:20.117608 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/checkemupload/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/checkemupload/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16398 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/checkemupload/checkemupload.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 16:17:20.121608 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/cif_emdb_translator/
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      139 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/cif_emdb_translator/README.md
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/cif_emdb_translator/__init__.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)   676892 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)  2304974 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/cif_emdb_translator/emdb.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     1196 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2490 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 16:17:20.121608 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/data/
+-rw-r--r--   0 vsts      (1001) docker     (127)   221515 2024-04-24 16:16:22.000000 wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/data/emdb-v3.xsd
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 16:17:20.121608 wwpdb_utils_emdb-1.8.1/wwpdb.utils.emdb.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)      960 2024-04-24 16:17:20.000000 wwpdb_utils_emdb-1.8.1/wwpdb.utils.emdb.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      947 2024-04-24 16:17:20.000000 wwpdb_utils_emdb-1.8.1/wwpdb.utils.emdb.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-24 16:17:20.000000 wwpdb_utils_emdb-1.8.1/wwpdb.utils.emdb.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       87 2024-04-24 16:17:20.000000 wwpdb_utils_emdb-1.8.1/wwpdb.utils.emdb.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-24 16:17:05.000000 wwpdb_utils_emdb-1.8.1/wwpdb.utils.emdb.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      101 2024-04-24 16:17:20.000000 wwpdb_utils_emdb-1.8.1/wwpdb.utils.emdb.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-24 16:17:20.000000 wwpdb_utils_emdb-1.8.1/wwpdb.utils.emdb.egg-info/top_level.txt
```

### Comparing `wwpdb.utils.emdb-1.8/PKG-INFO` & `wwpdb_utils_emdb-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.emdb
-Version: 1.8
+Version: 1.8.1
 Summary: wwPDB EMDB to XML converter
 Home-page: https://github.com/rcsb/py-wwpdb_utils_config
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.emdb-1.8/setup.py` & `wwpdb_utils_emdb-1.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/atomcheck/atomcheck.py` & `wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/atomcheck/atomcheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/checkemupload/checkemupload.py` & `wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/checkemupload/checkemupload.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,26 +184,34 @@
 
         Args:
             path2model (str): Path to the MMCIF file.
         """
         # Extracting atom coordinates from the MMCIF file
         mmcif_dict = MMCIF2Dict(path2model)
         self.file = path2model
-        self.structure = [
-            (float(x), float(y), float(z))
-            for x, y, z in zip(
-                mmcif_dict['_atom_site.Cartn_x'],
-                mmcif_dict['_atom_site.Cartn_y'],
-                mmcif_dict['_atom_site.Cartn_z']
-            )
-        ] if (
-            '_atom_site.Cartn_x' in mmcif_dict
-            and '_atom_site.Cartn_y' in mmcif_dict
-            and '_atom_site.Cartn_z' in mmcif_dict
-        ) else None
+        # Zhe edit 24042024
+        #
+        # While the coordinate file has been validated to contain floats,
+        # BioPython does not deal with multiple data blocks properly.
+        # The second and subsequent data blocks are misparsed.
+        # Therefore, the try/except handles the misfeature - rejecting
+        # "bad" data
+        structure = []
+        x = mmcif_dict['_atom_site.Cartn_x']
+        y = mmcif_dict['_atom_site.Cartn_y']
+        z = mmcif_dict['_atom_site.Cartn_z']
+        for x, y, z in zip(x, y, z):
+            try:
+                newx = float(x)
+                newy = float(y)
+                newz = float(z)
+                structure.append((newx, newy, newz))
+            except ValueError:
+                continue
+        self.structure = structure
 
 
 class Validator:
     """
     Class for validating and comparing EM maps and models.
     """
```

### Comparing `wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py` & `wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/cif_emdb_translator/emdb.py` & `wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/cif_emdb_translator/emdb.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py` & `wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py` & `wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.8/wwpdb/utils/emdb/data/emdb-v3.xsd` & `wwpdb_utils_emdb-1.8.1/wwpdb/utils/emdb/data/emdb-v3.xsd`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.8/wwpdb.utils.emdb.egg-info/PKG-INFO` & `wwpdb_utils_emdb-1.8.1/wwpdb.utils.emdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.emdb
-Version: 1.8
+Version: 1.8.1
 Summary: wwPDB EMDB to XML converter
 Home-page: https://github.com/rcsb/py-wwpdb_utils_config
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.emdb-1.8/wwpdb.utils.emdb.egg-info/SOURCES.txt` & `wwpdb_utils_emdb-1.8.1/wwpdb.utils.emdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

