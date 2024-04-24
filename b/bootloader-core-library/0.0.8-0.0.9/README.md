# Comparing `tmp/bootloader_core_library-0.0.8.tar.gz` & `tmp/bootloader_core_library-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bootloader_core_library-0.0.8.tar", max compression
+gzip compressed data, was "bootloader_core_library-0.0.9.tar", max compression
```

## Comparing `bootloader_core_library-0.0.8.tar` & `bootloader_core_library-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1102 2023-08-02 02:26:54.265696 bootloader_core_library-0.0.8/CHANGELOG.md
--rw-r--r--   0        0        0      761 2023-03-31 11:22:24.297536 bootloader_core_library-0.0.8/LICENSE.md
--rw-r--r--   0        0        0      138 2023-08-01 09:48:11.340859 bootloader_core_library-0.0.8/README.md
--rw-r--r--   0        0        0      905 2023-08-02 02:25:47.178772 bootloader_core_library-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 bootloader_core_library-0.0.8/src/bootloader/__init__.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.992853 bootloader_core_library-0.0.8/src/bootloader/ue/__init__.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 bootloader_core_library-0.0.8/src/bootloader/ue/constant/__init__.py
--rw-r--r--   0        0        0    17232 2023-08-01 14:15:12.075340 bootloader_core_library-0.0.8/src/bootloader/ue/constant/ue_asset.py
--rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 bootloader_core_library-0.0.8/src/bootloader/ue/model/__init__.py
--rw-r--r--   0        0        0    15962 2023-08-02 02:25:57.190457 bootloader_core_library-0.0.8/src/bootloader/ue/model/ue_asset.py
--rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 bootloader_core_library-0.0.8/setup.py
--rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 bootloader_core_library-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1199 2023-08-02 03:29:41.616696 bootloader_core_library-0.0.9/CHANGELOG.md
+-rw-r--r--   0        0        0      761 2023-03-31 11:22:24.297536 bootloader_core_library-0.0.9/LICENSE.md
+-rw-r--r--   0        0        0      138 2023-08-01 09:48:11.340859 bootloader_core_library-0.0.9/README.md
+-rw-r--r--   0        0        0      905 2023-08-02 03:29:48.222238 bootloader_core_library-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.979756 bootloader_core_library-0.0.9/src/bootloader/__init__.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.992853 bootloader_core_library-0.0.9/src/bootloader/ue/__init__.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 bootloader_core_library-0.0.9/src/bootloader/ue/constant/__init__.py
+-rw-r--r--   0        0        0    17232 2023-08-01 14:15:12.075340 bootloader_core_library-0.0.9/src/bootloader/ue/constant/ue_asset.py
+-rw-r--r--   0        0        0      859 2023-03-31 11:21:05.975392 bootloader_core_library-0.0.9/src/bootloader/ue/model/__init__.py
+-rw-r--r--   0        0        0    16003 2023-08-02 03:29:17.793044 bootloader_core_library-0.0.9/src/bootloader/ue/model/ue_asset.py
+-rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 bootloader_core_library-0.0.9/setup.py
+-rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 bootloader_core_library-0.0.9/PKG-INFO
```

### Comparing `bootloader_core_library-0.0.8/CHANGELOG.md` & `bootloader_core_library-0.0.9/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,21 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), 
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 
+## [0.0.9] - 2024-08-02
+### Fixed
+- Add missing attribute "asset_id" in the JSON serialization
+
 ## [0.0.8] - 2024-08-02
 ### Fixed
-- Fix the method "to_json" to include the complete list of the asset's attribute
+- Fix the method "to_json" to include the complete list of the asset's attributes
 
 ## [0.0.7] - 2024-08-02
 ### Added
 - Add the method "__str__" to stringify the representation of an asset or an asset file
 
 ## [0.0.6] - 2024-08-02
 ### Added
```

### Comparing `bootloader_core_library-0.0.8/LICENSE.md` & `bootloader_core_library-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.8/pyproject.toml` & `bootloader_core_library-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 keywords = ["core", "library"]
 license = "SEE LICENSE IN <LICENSE.md>"
 name = "bootloader-core-library"
 packages = [{include = "bootloader", from = "src"}]
 readme = "README.md"
 repository = "https://github.com/bootloader-studio/bootloader-core-python-library"
-version = "0.0.8"
+version = "0.0.9"
 
 [tool.poetry.dependencies]
 perseus-core-library = "^1.19.4"
 python = "^3.10"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `bootloader_core_library-0.0.8/src/bootloader/__init__.py` & `bootloader_core_library-0.0.9/src/bootloader/__init__.py`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.8/src/bootloader/ue/__init__.py` & `bootloader_core_library-0.0.9/src/bootloader/ue/__init__.py`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.8/src/bootloader/ue/constant/__init__.py` & `bootloader_core_library-0.0.9/src/bootloader/ue/constant/__init__.py`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.8/src/bootloader/ue/constant/ue_asset.py` & `bootloader_core_library-0.0.9/src/bootloader/ue/constant/ue_asset.py`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.8/src/bootloader/ue/model/__init__.py` & `bootloader_core_library-0.0.9/src/bootloader/ue/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bootloader_core_library-0.0.8/src/bootloader/ue/model/ue_asset.py` & `bootloader_core_library-0.0.9/src/bootloader/ue/model/ue_asset.py`

 * *Files 0% similar despite different names*

```diff
@@ -280,14 +280,15 @@
         """
         Serialize the asset's information to a JSON expression.
 
 
         :return: A JSON expression representing the asset's information.
         """
         return {
+            'asset_id': self.__asset_id,
             'asset_name': self.__asset_name,
             'asset_class_path': self.__asset_class_path,
             'dependencies': self.__dependencies,
             'object_status': self.__object_status,
             'package_name': self.__package_name,
             'references': self.__references,
             'tags': self.__tags,
```

### Comparing `bootloader_core_library-0.0.8/setup.py` & `bootloader_core_library-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['perseus-core-library>=1.19.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'bootloader-core-library',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Repository of reusable Python components to be shared by Python projects using the Bootloader services',
     'long_description': '# Bootloader Core Python Library\n\nRepository of reusable Python components to be shared by Python projects using the Bootloader services.\n',
     'author': 'Daniel CAUNE',
     'author_email': 'daniel@bootloader.studio',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bootloader-studio/bootloader-core-python-library',
```

### Comparing `bootloader_core_library-0.0.8/PKG-INFO` & `bootloader_core_library-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bootloader-core-library
-Version: 0.0.8
+Version: 0.0.9
 Summary: Repository of reusable Python components to be shared by Python projects using the Bootloader services
 Home-page: https://github.com/bootloader-studio/bootloader-core-python-library
 License: SEE LICENSE IN <LICENSE.md>
 Keywords: core,library
 Author: Daniel CAUNE
 Author-email: daniel@bootloader.studio
 Requires-Python: >=3.10,<4.0
```

