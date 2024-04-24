# Comparing `tmp/utype-0.5.1.tar.gz` & `tmp/utype-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utype-0.5.1.tar", last modified: Tue Apr 16 02:45:21 2024, max compression
+gzip compressed data, was "utype-0.5.2.tar", last modified: Wed Apr 24 14:42:52 2024, max compression
```

## Comparing `utype-0.5.1.tar` & `utype-0.5.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 02:45:21.745885 utype-0.5.1/
--rw-rw-rw-   0        0        0      588 2022-11-30 10:26:26.000000 utype-0.5.1/LICENSE
--rw-rw-rw-   0        0        0    10191 2024-04-16 02:45:21.745885 utype-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     8759 2024-01-09 06:17:39.000000 utype-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 02:45:21.706990 utype-0.5.1/examples/
--rw-rw-rw-   0        0        0        0 2024-01-27 10:18:42.000000 utype-0.5.1/examples/__init__.py
--rw-rw-rw-   0        0        0       42 2024-04-16 02:45:21.745885 utype-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1824 2022-12-16 10:42:48.000000 utype-0.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 02:45:21.708985 utype-0.5.1/utype/
--rw-rw-rw-   0        0        0     1231 2024-04-16 02:36:41.000000 utype-0.5.1/utype/__init__.py
--rw-rw-rw-   0        0        0     6219 2023-02-18 08:54:07.000000 utype-0.5.1/utype/decorator.py
-drwxrwxrwx   0        0        0        0 2024-04-16 02:45:21.728931 utype-0.5.1/utype/parser/
--rw-rw-rw-   0        0        0        0 2022-12-02 05:43:17.000000 utype-0.5.1/utype/parser/__init__.py
--rw-rw-rw-   0        0        0    23012 2024-02-22 10:40:50.000000 utype-0.5.1/utype/parser/base.py
--rw-rw-rw-   0        0        0    22768 2024-03-28 04:21:05.000000 utype-0.5.1/utype/parser/cls.py
--rw-rw-rw-   0        0        0    48651 2024-03-29 04:45:00.000000 utype-0.5.1/utype/parser/field.py
--rw-rw-rw-   0        0        0    36928 2023-12-19 13:21:17.000000 utype-0.5.1/utype/parser/func.py
--rw-rw-rw-   0        0        0    16412 2023-04-08 06:18:37.000000 utype-0.5.1/utype/parser/options.py
--rw-rw-rw-   0        0        0    67750 2024-04-16 02:41:01.000000 utype-0.5.1/utype/parser/rule.py
--rw-rw-rw-   0        0        0    18029 2024-02-22 10:45:55.000000 utype-0.5.1/utype/schema.py
-drwxrwxrwx   0        0        0        0 2024-04-16 02:45:21.729928 utype-0.5.1/utype/specs/
--rw-rw-rw-   0        0        0        0 2022-11-30 10:26:26.000000 utype-0.5.1/utype/specs/__init__.py
--rw-rw-rw-   0        0        0    14933 2024-03-31 08:20:40.000000 utype-0.5.1/utype/specs/json_schema.py
--rw-rw-rw-   0        0        0     5515 2024-04-03 15:29:32.000000 utype-0.5.1/utype/types.py
-drwxrwxrwx   0        0        0        0 2024-04-16 02:45:21.744894 utype-0.5.1/utype/utils/
--rw-rw-rw-   0        0        0        0 2022-11-30 10:26:26.000000 utype-0.5.1/utype/utils/__init__.py
--rw-rw-rw-   0        0        0     3676 2023-03-04 11:33:54.000000 utype-0.5.1/utype/utils/base.py
--rw-rw-rw-   0        0        0     3381 2024-04-16 02:41:01.000000 utype-0.5.1/utype/utils/compat.py
--rw-rw-rw-   0        0        0     2017 2022-12-16 09:30:29.000000 utype-0.5.1/utype/utils/datastructures.py
--rw-rw-rw-   0        0        0     3928 2024-04-04 11:29:24.000000 utype-0.5.1/utype/utils/encode.py
--rw-rw-rw-   0        0        0     7863 2024-02-22 10:54:09.000000 utype-0.5.1/utype/utils/example.py
--rw-rw-rw-   0        0        0     8483 2024-01-03 07:03:53.000000 utype-0.5.1/utype/utils/exceptions.py
--rw-rw-rw-   0        0        0     1621 2023-06-30 09:41:30.000000 utype-0.5.1/utype/utils/functional.py
--rw-rw-rw-   0        0        0     6219 2022-12-16 09:43:52.000000 utype-0.5.1/utype/utils/style.py
--rw-rw-rw-   0        0        0    24094 2024-01-03 08:18:27.000000 utype-0.5.1/utype/utils/transform.py
-drwxrwxrwx   0        0        0        0 2024-04-16 02:45:21.724945 utype-0.5.1/utype.egg-info/
--rw-rw-rw-   0        0        0    10191 2024-04-16 02:45:21.000000 utype-0.5.1/utype.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      703 2024-04-16 02:45:21.000000 utype-0.5.1/utype.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 02:45:21.000000 utype-0.5.1/utype.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-16 02:45:21.000000 utype-0.5.1/utype.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-16 02:45:21.000000 utype-0.5.1/utype.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 14:42:52.012967 utype-0.5.2/
+-rw-rw-rw-   0        0        0      588 2022-11-30 10:26:26.000000 utype-0.5.2/LICENSE
+-rw-rw-rw-   0        0        0    10191 2024-04-24 14:42:52.011970 utype-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8759 2024-01-09 06:17:39.000000 utype-0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 14:42:51.978014 utype-0.5.2/examples/
+-rw-rw-rw-   0        0        0        0 2024-01-27 10:18:42.000000 utype-0.5.2/examples/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-24 14:42:52.012967 utype-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1824 2022-12-16 10:42:48.000000 utype-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:42:51.989033 utype-0.5.2/utype/
+-rw-rw-rw-   0        0        0     1231 2024-04-24 14:39:20.000000 utype-0.5.2/utype/__init__.py
+-rw-rw-rw-   0        0        0     6219 2023-02-18 08:54:07.000000 utype-0.5.2/utype/decorator.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:42:52.003991 utype-0.5.2/utype/parser/
+-rw-rw-rw-   0        0        0        0 2022-12-02 05:43:17.000000 utype-0.5.2/utype/parser/__init__.py
+-rw-rw-rw-   0        0        0    23012 2024-02-22 10:40:50.000000 utype-0.5.2/utype/parser/base.py
+-rw-rw-rw-   0        0        0    22768 2024-03-28 04:21:05.000000 utype-0.5.2/utype/parser/cls.py
+-rw-rw-rw-   0        0        0    48651 2024-03-29 04:45:00.000000 utype-0.5.2/utype/parser/field.py
+-rw-rw-rw-   0        0        0    36928 2023-12-19 13:21:17.000000 utype-0.5.2/utype/parser/func.py
+-rw-rw-rw-   0        0        0    16412 2023-04-08 06:18:37.000000 utype-0.5.2/utype/parser/options.py
+-rw-rw-rw-   0        0        0    67750 2024-04-16 02:41:01.000000 utype-0.5.2/utype/parser/rule.py
+-rw-rw-rw-   0        0        0    18029 2024-02-22 10:45:55.000000 utype-0.5.2/utype/schema.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:42:52.004988 utype-0.5.2/utype/specs/
+-rw-rw-rw-   0        0        0        0 2022-11-30 10:26:26.000000 utype-0.5.2/utype/specs/__init__.py
+-rw-rw-rw-   0        0        0    15234 2024-04-24 14:39:20.000000 utype-0.5.2/utype/specs/json_schema.py
+-rw-rw-rw-   0        0        0     5515 2024-04-03 15:29:32.000000 utype-0.5.2/utype/types.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:42:52.010973 utype-0.5.2/utype/utils/
+-rw-rw-rw-   0        0        0        0 2022-11-30 10:26:26.000000 utype-0.5.2/utype/utils/__init__.py
+-rw-rw-rw-   0        0        0     3676 2023-03-04 11:33:54.000000 utype-0.5.2/utype/utils/base.py
+-rw-rw-rw-   0        0        0     3381 2024-04-16 02:41:01.000000 utype-0.5.2/utype/utils/compat.py
+-rw-rw-rw-   0        0        0     2017 2022-12-16 09:30:29.000000 utype-0.5.2/utype/utils/datastructures.py
+-rw-rw-rw-   0        0        0     3928 2024-04-04 11:29:24.000000 utype-0.5.2/utype/utils/encode.py
+-rw-rw-rw-   0        0        0     7863 2024-02-22 10:54:09.000000 utype-0.5.2/utype/utils/example.py
+-rw-rw-rw-   0        0        0     8889 2024-04-23 11:52:38.000000 utype-0.5.2/utype/utils/exceptions.py
+-rw-rw-rw-   0        0        0     1621 2023-06-30 09:41:30.000000 utype-0.5.2/utype/utils/functional.py
+-rw-rw-rw-   0        0        0     6219 2022-12-16 09:43:52.000000 utype-0.5.2/utype/utils/style.py
+-rw-rw-rw-   0        0        0    24094 2024-01-03 08:18:27.000000 utype-0.5.2/utype/utils/transform.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:42:52.000002 utype-0.5.2/utype.egg-info/
+-rw-rw-rw-   0        0        0    10191 2024-04-24 14:42:51.000000 utype-0.5.2/utype.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      703 2024-04-24 14:42:51.000000 utype-0.5.2/utype.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 14:42:51.000000 utype-0.5.2/utype.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-24 14:42:51.000000 utype-0.5.2/utype.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-24 14:42:51.000000 utype-0.5.2/utype.egg-info/top_level.txt
```

### Comparing `utype-0.5.1/LICENSE` & `utype-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `utype-0.5.1/PKG-INFO` & `utype-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utype
-Version: 0.5.1
+Version: 0.5.2
 Summary: Declare & parse types / dataclasses / functions based on Python type annotations
 Home-page: https://utype.io
 Author: XuLin Zhou
 Author-email: zxl@utilmeta.com
 License: Apache 2.0
 Project-URL: Project Home, https://utype.io
 Project-URL: Documentation, https://utype.io
```

### Comparing `utype-0.5.1/README.md` & `utype-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `utype-0.5.1/setup.py` & `utype-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.1/utype/__init__.py` & `utype-0.5.2/utype/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .utils.transform import (TypeTransformer, type_transform)
 from .utils.datastructures import unprovided
 from .specs.json_schema import JsonSchemaGenerator
 
 register_transformer = TypeTransformer.registry.register
 
 
-VERSION = (0, 5, 1, None)
+VERSION = (0, 5, 2, None)
 
 
 def _get_version():
     pre_release = VERSION[3] if len(VERSION) > 3 else ""
     version = ".".join([str(v) for v in VERSION[:3]])
     if pre_release:
         version += f"-{pre_release}"
```

### Comparing `utype-0.5.1/utype/decorator.py` & `utype-0.5.2/utype/decorator.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.1/utype/parser/base.py` & `utype-0.5.2/utype/parser/base.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.1/utype/parser/cls.py` & `utype-0.5.2/utype/parser/cls.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.1/utype/parser/field.py` & `utype-0.5.2/utype/parser/field.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.1/utype/parser/func.py` & `utype-0.5.2/utype/parser/func.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.1/utype/parser/options.py` & `utype-0.5.2/utype/parser/options.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.1/utype/parser/rule.py` & `utype-0.5.2/utype/parser/rule.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.1/utype/schema.py` & `utype-0.5.2/utype/schema.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.1/utype/specs/json_schema.py` & `utype-0.5.2/utype/specs/json_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,15 +273,20 @@
     def get_def_name(self, t: type):
         if t in self.defs:
             for k, v in self.names.items():
                 if v == t:
                     return k
         return None
 
-    def set_def(self, name: str, t: type, data: dict):
+    def set_def(self, name: str, t: type, data: dict = None):
+        if t in self.defs:
+            if data is not None:
+                # name already set
+                self.defs[t] = data
+            return name
         n = 0
         while True:
             _name = name + (f'_{n}' if n else '')
             if _name in self.names:
                 n += 1
                 continue
             name = _name
@@ -348,14 +353,17 @@
         if self.output and not parser.in_out_identical:
             cls_name += '_O'
 
         if isinstance(self.defs, dict):
             def_name = self.get_def_name(t)
             if def_name:
                 return {"$ref": f"{self.ref_prefix}{def_name}"}
+            cls_name = self.set_def(cls_name, t, data=None)
+            # set data to None:
+            # avoid cascade references
 
         data = {"type": "object"}
         required = []
         properties = {}
 
         for name, field in parser.fields.items():
             value = self.generate_for_field(field, options=parser.options)
```

### Comparing `utype-0.5.1/utype/types.py` & `utype-0.5.2/utype/types.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.1/utype/utils/base.py` & `utype-0.5.2/utype/utils/base.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.1/utype/utils/compat.py` & `utype-0.5.2/utype/utils/compat.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.1/utype/utils/datastructures.py` & `utype-0.5.2/utype/utils/datastructures.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.1/utype/utils/encode.py` & `utype-0.5.2/utype/utils/encode.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.1/utype/utils/example.py` & `utype-0.5.2/utype/utils/example.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.1/utype/utils/exceptions.py` & `utype-0.5.2/utype/utils/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,18 +18,21 @@
         msg: str = None,
         *,
         field=None,
         origin_exc: Exception = None,
     ):
         self.msg = msg
         self.field = field
-        self.origin = origin_exc
+        self.origin_exc = origin_exc
 
         super().__init__(msg)
 
+        if isinstance(self.origin_exc, Exception):
+            self.__traceback__ = self.origin_exc.__traceback__
+
 
 class UpdateError(FieldError):
     pass
 
 
 class DeleteError(FieldError):
     pass
@@ -56,19 +59,24 @@
         self.value = value
         self.type = type
         self.item = item
         self.field = field
         self.routes = routes
         super().__init__(self.formatted_message)
 
+        if isinstance(self.origin_exc, Exception):
+            self.__traceback__ = self.origin_exc.__traceback__
+
     @property
     def formatted_message(self):
         msg = self.msg
         if self.item:
             msg = f"parse item: [{repr(self.item)}] failed: {msg}"
+        if isinstance(self.origin_exc, Exception) and not isinstance(self.origin_exc, ParseError):
+            msg = f'{self.origin_exc.__class__.__name__}: {msg}'
         return msg
 
     def get_detail(self) -> dict:
         from ..specs.json_schema import JsonSchemaGenerator
         origin = None
         if self.origin_exc:
             if isinstance(self.origin_exc, ParseError) and self.origin_exc.field:
```

### Comparing `utype-0.5.1/utype/utils/functional.py` & `utype-0.5.2/utype/utils/functional.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.1/utype/utils/style.py` & `utype-0.5.2/utype/utils/style.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.1/utype/utils/transform.py` & `utype-0.5.2/utype/utils/transform.py`

 * *Files identical despite different names*

### Comparing `utype-0.5.1/utype.egg-info/PKG-INFO` & `utype-0.5.2/utype.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utype
-Version: 0.5.1
+Version: 0.5.2
 Summary: Declare & parse types / dataclasses / functions based on Python type annotations
 Home-page: https://utype.io
 Author: XuLin Zhou
 Author-email: zxl@utilmeta.com
 License: Apache 2.0
 Project-URL: Project Home, https://utype.io
 Project-URL: Documentation, https://utype.io
```

### Comparing `utype-0.5.1/utype.egg-info/SOURCES.txt` & `utype-0.5.2/utype.egg-info/SOURCES.txt`

 * *Files identical despite different names*

