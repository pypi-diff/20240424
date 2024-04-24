# Comparing `tmp/zyte-common-items-0.8.0.tar.gz` & `tmp/zyte-common-items-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zyte-common-items-0.8.0.tar", last modified: Thu Jul 27 12:13:01 2023, max compression
+gzip compressed data, was "zyte-common-items-0.9.0.tar", last modified: Thu Aug  3 15:30:50 2023, max compression
```

## Comparing `zyte-common-items-0.8.0.tar` & `zyte-common-items-0.9.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:13:01.701554 zyte-common-items-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 12:13:01.701554 zyte-common-items-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 12:13:01.701554 zyte-common-items-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:13:01.697554 zyte-common-items-0.8.0/zyte_common_items/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/zyte_common_items/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/zyte_common_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/zyte_common_items/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/zyte_common_items/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13652 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/zyte_common_items/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    38188 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/zyte_common_items/items.py
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/zyte_common_items/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/zyte_common_items/processors.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/zyte_common_items/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/zyte_common_items/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:13:01.697554 zyte-common-items-0.8.0/zyte_common_items.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 12:13:01.000000 zyte-common-items-0.8.0/zyte_common_items.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-27 12:13:01.000000 zyte-common-items-0.8.0/zyte_common_items.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:13:01.000000 zyte-common-items-0.8.0/zyte_common_items.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-27 12:13:01.000000 zyte-common-items-0.8.0/zyte_common_items.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 12:13:01.000000 zyte-common-items-0.8.0/zyte_common_items.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:30:50.068385 zyte-common-items-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-03 15:30:40.000000 zyte-common-items-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-03 15:30:40.000000 zyte-common-items-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-08-03 15:30:50.068385 zyte-common-items-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-08-03 15:30:40.000000 zyte-common-items-0.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-03 15:30:40.000000 zyte-common-items-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 15:30:50.068385 zyte-common-items-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-08-03 15:30:40.000000 zyte-common-items-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:30:50.064386 zyte-common-items-0.9.0/zyte_common_items/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 15:30:40.000000 zyte-common-items-0.9.0/zyte_common_items/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-03 15:30:40.000000 zyte-common-items-0.9.0/zyte_common_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-08-03 15:30:40.000000 zyte-common-items-0.9.0/zyte_common_items/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-08-03 15:30:40.000000 zyte-common-items-0.9.0/zyte_common_items/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13652 2023-08-03 15:30:40.000000 zyte-common-items-0.9.0/zyte_common_items/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38188 2023-08-03 15:30:40.000000 zyte-common-items-0.9.0/zyte_common_items/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6058 2023-08-03 15:30:40.000000 zyte-common-items-0.9.0/zyte_common_items/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-08-03 15:30:40.000000 zyte-common-items-0.9.0/zyte_common_items/processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 15:30:40.000000 zyte-common-items-0.9.0/zyte_common_items/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-08-03 15:30:40.000000 zyte-common-items-0.9.0/zyte_common_items/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 15:30:50.064386 zyte-common-items-0.9.0/zyte_common_items.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-08-03 15:30:50.000000 zyte-common-items-0.9.0/zyte_common_items.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-03 15:30:50.000000 zyte-common-items-0.9.0/zyte_common_items.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 15:30:50.000000 zyte-common-items-0.9.0/zyte_common_items.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-03 15:30:50.000000 zyte-common-items-0.9.0/zyte_common_items.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-03 15:30:50.000000 zyte-common-items-0.9.0/zyte_common_items.egg-info/top_level.txt
```

### Comparing `zyte-common-items-0.8.0/LICENSE` & `zyte-common-items-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zyte-common-items-0.8.0/PKG-INFO` & `zyte-common-items-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zyte-common-items
-Version: 0.8.0
+Version: 0.9.0
 Summary: Item definitions for Zyte API schema
 Home-page: https://github.com/zytedata/zyte-common-items
 Author: Zyte Group Ltd
 Author-email: info@zyte.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `zyte-common-items-0.8.0/README.rst` & `zyte-common-items-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `zyte-common-items-0.8.0/setup.py` & `zyte-common-items-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,18 +18,19 @@
         exclude=[
             "tests",
         ]
     ),
     package_data={
         "zyte_common_items": ["py.typed", "VERSION"],
     },
+    # needs to be in sync with the tox.ini min env
     install_requires=[
         "attrs>=22.1.0",
         "itemadapter>=0.8.0",
-        "web-poet>=0.9.0",
+        "web-poet>=0.14.0",
         "zyte-parsers>=0.2.0",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
```

### Comparing `zyte-common-items-0.8.0/zyte_common_items/__init__.py` & `zyte-common-items-0.9.0/zyte_common_items/__init__.py`

 * *Files identical despite different names*

### Comparing `zyte-common-items-0.8.0/zyte_common_items/adapter.py` & `zyte-common-items-0.9.0/zyte_common_items/adapter.py`

 * *Files identical despite different names*

### Comparing `zyte-common-items-0.8.0/zyte_common_items/base.py` & `zyte-common-items-0.9.0/zyte_common_items/base.py`

 * *Files identical despite different names*

### Comparing `zyte-common-items-0.8.0/zyte_common_items/components.py` & `zyte-common-items-0.9.0/zyte_common_items/components.py`

 * *Files identical despite different names*

### Comparing `zyte-common-items-0.8.0/zyte_common_items/items.py` & `zyte-common-items-0.9.0/zyte_common_items/items.py`

 * *Files identical despite different names*

### Comparing `zyte-common-items-0.8.0/zyte_common_items/pages.py` & `zyte-common-items-0.9.0/zyte_common_items/pages.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from datetime import datetime
-from typing import Generic, Type, TypeVar, get_args
+from typing import Generic, Optional, Type, TypeVar
 
 import attrs
 from web_poet import ItemPage, RequestUrl, Returns, WebPage, field
 from web_poet.pages import ItemT
+from web_poet.utils import get_generic_param
 
 from .components import (
     ArticleListMetadata,
     ArticleMetadata,
     ArticleNavigationMetadata,
     BusinessPlaceMetadata,
     JobPostingMetadata,
@@ -40,50 +41,47 @@
 
 
 class HasMetadata(Generic[MetadataT]):
     """Inherit from this generic mixin to set the metadata class used by a page
     class."""
 
     @property
-    def metadata_cls(self) -> Type[MetadataT]:
+    def metadata_cls(self) -> Optional[Type[MetadataT]]:
         """Metadata class."""
-        return _get_metadata_class(self)
+        return _get_metadata_class(type(self))
 
 
-def _get_metadata_class(obj):
-    for base in getattr(obj.__class__, "__orig_bases__", []):
-        origin = getattr(base, "__origin__", None)
-        if not origin:
-            continue
-        if origin != HasMetadata:
-            continue
-        return get_args(base)[0]
-    return None
+def _get_metadata_class(cls: type) -> Optional[Type[MetadataT]]:
+    return get_generic_param(cls, HasMetadata)
 
 
 class _BasePage(ItemPage[ItemT], HasMetadata[MetadataT]):
     class Processors:
         metadata = [metadata_processor]
 
     @field
     def metadata(self) -> MetadataT:
+        if self.metadata_cls is None:
+            raise ValueError(f"{type(self)} doesn'have a metadata class configured.")
         value = self.metadata_cls()
         attributes = dir(value)
         if "dateDownloaded" in attributes:
             value.dateDownloaded = _date_downloaded_now()  # type: ignore
         if "probability" in attributes:
             value.probability = 1.0  # type: ignore
         return value
 
     def no_item_found(self) -> ItemT:
         """Return an item with the current url and probability=0,
         indicating that the passed URL doesn't contain the expected item.
 
         Use it in your .validate_input implementation.
         """
+        if self.metadata_cls is None:
+            raise ValueError(f"{type(self)} doesn'have a metadata class configured.")
         metadata = self.metadata_cls()
         metadata_attributes = dir(metadata)
         if "dateDownloaded" in metadata_attributes:
             metadata.dateDownloaded = _date_downloaded_now()  # type: ignore
         if "probability" in metadata_attributes:
             metadata.probability = 0.0  # type: ignore
         return self.item_cls(  # type: ignore
```

### Comparing `zyte-common-items-0.8.0/zyte_common_items/processors.py` & `zyte-common-items-0.9.0/zyte_common_items/processors.py`

 * *Files identical despite different names*

### Comparing `zyte-common-items-0.8.0/zyte_common_items/util.py` & `zyte-common-items-0.9.0/zyte_common_items/util.py`

 * *Files identical despite different names*

### Comparing `zyte-common-items-0.8.0/zyte_common_items.egg-info/PKG-INFO` & `zyte-common-items-0.9.0/zyte_common_items.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zyte-common-items
-Version: 0.8.0
+Version: 0.9.0
 Summary: Item definitions for Zyte API schema
 Home-page: https://github.com/zytedata/zyte-common-items
 Author: Zyte Group Ltd
 Author-email: info@zyte.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `zyte-common-items-0.8.0/zyte_common_items.egg-info/SOURCES.txt` & `zyte-common-items-0.9.0/zyte_common_items.egg-info/SOURCES.txt`

 * *Files identical despite different names*

