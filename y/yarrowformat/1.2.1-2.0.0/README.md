# Comparing `tmp/yarrowformat-1.2.1.tar.gz` & `tmp/yarrowformat-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yarrowformat-1.2.1.tar", last modified: Wed Aug  2 16:21:33 2023, max compression
+gzip compressed data, was "dist/yarrowformat-2.0.0.tar", last modified: Wed Apr 24 07:55:30 2024, max compression
```

## Comparing `yarrowformat-1.2.1.tar` & `yarrowformat-2.0.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (122)      889 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2037 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)    11380 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     2392 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    81180 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/src/yarrowformat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/src/yarrowformat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      601 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/src/yarrowformat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/src/yarrowformat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)     2392 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/src/yarrowformat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/src/yarrowformat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/src/yarrowformat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      123 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/src/yarrowformat.egg-info/requires.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/src/yarrow/
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/src/yarrow/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)    29560 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/src/yarrow/yarrow_cls.py
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/src/yarrow/main.py
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/src/yarrow/_yarrow_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 16:21:33.000000 yarrowformat-1.2.1/src/yarrow/cli/
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/src/yarrow/cli/save.py
--rw-r--r--   0 runner    (1001) docker     (122)      850 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/src/yarrow/cli/open.py
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/src/yarrow/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1243 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/src/yarrow/cli/check.py
--rw-r--r--   0 runner    (1001) docker     (122)    13733 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/src/yarrow/yarrow.py
--rw-r--r--   0 runner    (1001) docker     (122)     6466 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/src/yarrow/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-08-02 16:21:29.000000 yarrowformat-1.2.1/src/yarrow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:55:30.000000 yarrowformat-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:55:30.000000 yarrowformat-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:55:30.000000 yarrowformat-2.0.0/src/yarrow/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-24 07:55:20.000000 yarrowformat-2.0.0/src/yarrow/_yarrow_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-24 07:55:20.000000 yarrowformat-2.0.0/src/yarrow/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14038 2024-04-24 07:55:20.000000 yarrowformat-2.0.0/src/yarrow/yarrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-04-24 07:55:20.000000 yarrowformat-2.0.0/src/yarrow/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-24 07:55:20.000000 yarrowformat-2.0.0/src/yarrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-24 07:55:30.000000 yarrowformat-2.0.0/src/yarrow/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29567 2024-04-24 07:55:20.000000 yarrowformat-2.0.0/src/yarrow/yarrow_cls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:55:30.000000 yarrowformat-2.0.0/src/yarrow/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-24 07:55:20.000000 yarrowformat-2.0.0/src/yarrow/cli/save.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-24 07:55:20.000000 yarrowformat-2.0.0/src/yarrow/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-24 07:55:20.000000 yarrowformat-2.0.0/src/yarrow/cli/open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-24 07:55:20.000000 yarrowformat-2.0.0/src/yarrow/cli/check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:55:30.000000 yarrowformat-2.0.0/src/yarrowformat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-24 07:55:30.000000 yarrowformat-2.0.0/src/yarrowformat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 07:55:30.000000 yarrowformat-2.0.0/src/yarrowformat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-24 07:55:30.000000 yarrowformat-2.0.0/src/yarrowformat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 07:55:30.000000 yarrowformat-2.0.0/src/yarrowformat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 07:55:30.000000 yarrowformat-2.0.0/src/yarrowformat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-24 07:55:30.000000 yarrowformat-2.0.0/src/yarrowformat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-24 07:55:30.000000 yarrowformat-2.0.0/src/yarrowformat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-24 07:55:20.000000 yarrowformat-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11380 2024-04-24 07:55:20.000000 yarrowformat-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    81180 2024-04-24 07:55:20.000000 yarrowformat-2.0.0/versioneer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-24 07:55:30.000000 yarrowformat-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-24 07:55:20.000000 yarrowformat-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-24 07:55:30.000000 yarrowformat-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-24 07:55:20.000000 yarrowformat-2.0.0/setup.py
```

### Comparing `yarrowformat-1.2.1/setup.cfg` & `yarrowformat-2.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 author = Mathieu Pichon
 author_email = mathieu.pichon_ext@michelin.com
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >= 3.6
+python_requires = >= 3.7
 install_requires = 
 	setuptools
 	wheel
-	pydantic >= 1.8,<2.0
+	pydantic >= 2.0
 	numpy >= 1.19
 	click
 zip_safe = False
 include_package_data = True
 
 [options.extras_require]
 dev =
```

### Comparing `yarrowformat-1.2.1/README.md` & `yarrowformat-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `yarrowformat-1.2.1/LICENSE` & `yarrowformat-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yarrowformat-1.2.1/PKG-INFO` & `yarrowformat-2.0.0/src/yarrowformat.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: yarrowformat
-Version: 1.2.1
+Version: 2.0.0
 Summary: Yarrow Format parsing lib
 Home-page: https://github.com/michelin/YarrowFormat
 Author: Mathieu Pichon
 Author-email: mathieu.pichon_ext@michelin.com
 License: UNKNOWN
 Platform: UNKNOWN
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Yarrow: a data format for computer vision
 
 ---------------
```

### Comparing `yarrowformat-1.2.1/versioneer.py` & `yarrowformat-2.0.0/versioneer.py`

 * *Files identical despite different names*

### Comparing `yarrowformat-1.2.1/src/yarrowformat.egg-info/SOURCES.txt` & `yarrowformat-2.0.0/src/yarrowformat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yarrowformat-1.2.1/src/yarrowformat.egg-info/PKG-INFO` & `yarrowformat-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: yarrowformat
-Version: 1.2.1
+Version: 2.0.0
 Summary: Yarrow Format parsing lib
 Home-page: https://github.com/michelin/YarrowFormat
 Author: Mathieu Pichon
 Author-email: mathieu.pichon_ext@michelin.com
 License: UNKNOWN
 Platform: UNKNOWN
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Yarrow: a data format for computer vision
 
 ---------------
```

### Comparing `yarrowformat-1.2.1/src/yarrow/yarrow_cls.py` & `yarrowformat-2.0.0/src/yarrow/yarrow_cls.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,14 @@
     img_as_dict = img_pydantic.dict() # now you have a dict
 
 """
 from copy import copy
 from datetime import datetime
 from warnings import warn
 
-from pydantic import StrBytes
-
 from .yarrow import *
 
 
 class Image:
     def __init__(
         self,
         width: int,
@@ -728,15 +726,15 @@
                     meta=multilayer.meta,
                     id=multilayer.id,
                 )
             )
 
         annot_list = []
         for annot in annot_list_source:
-            annot_param = annot.dict(exclude_unset=True)
+            annot_param = annot.model_dump(exclude_unset=True)
 
             # Get contributor from its id
             contr = next(
                 (contr for contr in contrib_list if contr.id == annot.contributor_id),
                 None,
             )
             if contr is None:
@@ -782,16 +780,19 @@
             confidential=conf_list,
             categories=cat_list,
             multilayer_images=multilayer_list,
         )
 
     @classmethod
     def parse_file(cls, path, **kwargs) -> "YarrowDataset":
-        return cls.from_yarrow(YarrowDataset_pydantic.parse_file(path, **kwargs))
+        with open(path, "rb") as jsf:
+            yar_dict = json.load(jsf)
+            return cls.parse_obj(yar_dict)
 
     @classmethod
     def parse_obj(cls, obj: dict, **kwargs) -> "YarrowDataset":
-        return cls.from_yarrow(YarrowDataset_pydantic.parse_obj(obj))
+        return cls.from_yarrow(YarrowDataset_pydantic.model_validate(obj))
 
     @classmethod
-    def parse_raw(cls, raw: StrBytes, **kwargs) -> "YarrowDataset":
-        return cls.from_yarrow(YarrowDataset_pydantic.parse_raw(raw, **kwargs))
+    def parse_raw(cls, raw: bytes, **kwargs) -> "YarrowDataset":
+        yar_dict = json.load(raw)
+        return cls.parse_obj(yar_dict)
```

### Comparing `yarrowformat-1.2.1/src/yarrow/cli/save.py` & `yarrowformat-2.0.0/src/yarrow/cli/save.py`

 * *Files identical despite different names*

### Comparing `yarrowformat-1.2.1/src/yarrow/cli/open.py` & `yarrowformat-2.0.0/src/yarrow/cli/open.py`

 * *Files identical despite different names*

### Comparing `yarrowformat-1.2.1/src/yarrow/cli/check.py` & `yarrowformat-2.0.0/src/yarrow/cli/check.py`

 * *Files identical despite different names*

### Comparing `yarrowformat-1.2.1/src/yarrow/yarrow.py` & `yarrowformat-2.0.0/src/yarrow/yarrow.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 import json
 import uuid
 from datetime import datetime
 from typing import Any, List, Optional, Union
 from warnings import warn
 
 import numpy as np
-from pydantic import BaseModel, Field, Json
+from pydantic import BaseModel, ConfigDict, Field, Json
 
 from ._yarrow_version import _yarrow_version
 
 
 def uuid_init():
     return uuid.uuid4().hex
 
 
 class Info(BaseModel):
     # fmt: off
     version         : str = _yarrow_version
     source          : Union[str, dict]
     date_created    : datetime
-    destination     : Optional[dict]
-    meta            : Optional[dict]
+    destination     : Optional[dict] = None
+    meta            : Optional[dict] = None
     # fmt: on
 
 
 class Layer(BaseModel):
     # fmt: off
     id              : str = Field(default_factory=uuid_init)
     frame_id        : int
-    width           : Optional[int]
-    height          : Optional[int]
+    width           : Optional[int] = None
+    height          : Optional[int] = None
     name            : Optional[str] = ""
-    meta            : Optional[dict]
+    meta            : Optional[dict] = None
     # fmt: on
 
     def __hash__(self) -> int:
         return hash((self.frame_id, self.width, self.height, self.name))
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, Layer):
@@ -53,21 +53,21 @@
 class Image_pydantic(BaseModel):
     # fmt: off
     id              : str = Field(default_factory=uuid_init)
     width           : int
     height          : int
     file_name       : str
     date_captured   : datetime
-    azure_url       : Optional[str]
-    confidential_id : Optional[str]
-    meta            : Optional[Union[dict, Json]]
-    comment         : Optional[str]
-    asset_id        : Optional[str]
-    layers          : Optional[List[Layer]]
-    split           : Optional[str]
+    azure_url       : Optional[str] = None
+    confidential_id : Optional[str] = None
+    meta            : Optional[Union[dict, Json]] = None
+    comment         : Optional[str] = None
+    asset_id        : Optional[str] = None
+    layers          : Optional[List[Layer]] = None
+    split           : Optional[str] = None
     # fmt: on
 
     def __eq__(self, other) -> bool:
         if isinstance(other, Image_pydantic):
             return all(
                 (
                     self.file_name == other.file_name,
@@ -88,16 +88,16 @@
     YarrowDataset
     """
 
     # fmt: off
     id              : str = Field(default_factory=uuid_init)
     image_id        : List[str] = Field(default_factory=list)
     name            : Optional[str] = ""
-    meta            : Optional[dict]
-    split           : Optional[str]
+    meta            : Optional[dict] = None
+    split           : Optional[str] = None
     # fmt: on
 
     def __hash__(self) -> int:
         warn("Multilayer_image.__hash__ is only well defined inside a YarrowDataset")
         return hash((*sorted(self.image_id), self.name))
 
     def __eq__(self, other: Any) -> bool:
@@ -145,18 +145,18 @@
         return NotImplemented
 
 
 class Category(BaseModel):
     # fmt: off
     id              : str = Field(default_factory=uuid_init)
     name            : str
-    value           : Optional[str]
-    super_category  : Optional[str]
-    keypoints       : Optional[List[str]]
-    skeleton        : Optional[List[Edge]]
+    value           : Optional[str] = None
+    super_category  : Optional[str] = None
+    keypoints       : Optional[List[str]] = None
+    skeleton        : Optional[List[Edge]] = None
     # fmt: on
 
     def __eq__(self, other) -> bool:
         if isinstance(other, Category):
             return all(
                 (
                     self.name == other.name,
@@ -235,28 +235,28 @@
 
 class Annotation_pydantic(BaseModel):
     # fmt: off
     id              : str = Field(default_factory=uuid_init)
     image_id        : Union[str, List[str]]
     category_id     : Union[str, List[str]]
     contributor_id  : str
-    name            : Optional[str]
-    comment         : Optional[str]
-    segmentation    : Optional[Union[List[List[float]], RLE]] = Field(deprecated=True)
+    name            : Optional[str] = None
+    comment         : Optional[str] = None
+    segmentation    : Optional[Union[List[List[float]], RLE]] = Field(deprecated=True,default=None)
     is_crowd        : Optional[int] = Field(default=0, deprecated=True)
-    mask            : Optional[RLE]
-    polygon         : Optional[List[List[float]]]
-    polyline        : Optional[List[List[float]]]
-    area            : Optional[float]
-    bbox            : Optional[List[float]]
-    keypoints       : Optional[List[List[float]]]
-    num_keypoints   : Optional[int]
-    weight          : Optional[float]
-    date_captured   : Optional[datetime]
-    meta            : Optional[dict]
+    mask            : Optional[RLE] = None
+    polygon         : Optional[List[List[float]]] = None
+    polyline        : Optional[List[List[float]]] = None 
+    area            : Optional[float] = None
+    bbox            : Optional[List[float]] = None
+    keypoints       : Optional[List[List[float]]] = None
+    num_keypoints   : Optional[int] = None
+    weight          : Optional[float] = None
+    date_captured   : Optional[datetime] = None
+    meta            : Optional[dict] = None
     # fmt: on
 
     def __eq__(self, other) -> bool:
         if isinstance(other, Annotation_pydantic):
             return all(
                 (
                     self.name == other.name,
@@ -267,20 +267,21 @@
                     self.mask == other.mask,
                 )
             )
         return NotImplemented
 
 
 class Contributor(BaseModel):
+    model_config = ConfigDict(protected_namespaces=())
     # fmt: off
     id              : str = Field(default_factory=uuid_init)
     human           : bool
     name            : str
-    model_id        : Optional[str]
-    human_id        : Optional[str]
+    model_id        : Optional[str] = None
+    human_id        : Optional[str] = None
     # fmt: on
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, Contributor):
             return all((self.name == other.name, self.human == other.human))
         return NotImplemented
```

### Comparing `yarrowformat-1.2.1/src/yarrow/utils.py` & `yarrowformat-2.0.0/src/yarrow/utils.py`

 * *Files identical despite different names*

