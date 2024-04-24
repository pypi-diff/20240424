# Comparing `tmp/mo_dots-9.600.24114.tar.gz` & `tmp/mo_dots-9.601.24115.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo_dots-9.600.24114.tar", last modified: Tue Apr 23 01:01:38 2024, max compression
+gzip compressed data, was "mo_dots-9.601.24115.tar", last modified: Wed Apr 24 08:54:35 2024, max compression
```

## Comparing `mo_dots-9.600.24114.tar` & `mo_dots-9.601.24115.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 01:01:38.646871 mo_dots-9.600.24114/
--rw-rw-rw-   0        0        0    16725 2022-02-13 20:11:16.000000 mo_dots-9.600.24114/LICENSE
--rw-rw-rw-   0        0        0     5055 2024-04-23 01:01:38.645592 mo_dots-9.600.24114/PKG-INFO
--rw-rw-rw-   0        0        0     3549 2024-04-04 03:46:45.000000 mo_dots-9.600.24114/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 01:01:38.633351 mo_dots-9.600.24114/mo_dots/
--rw-rw-rw-   0        0        0    14004 2024-04-22 09:12:18.000000 mo_dots-9.600.24114/mo_dots/__init__.py
--rw-rw-rw-   0        0        0    16489 2024-04-23 01:01:31.000000 mo_dots-9.600.24114/mo_dots/datas.py
--rw-rw-rw-   0        0        0     4283 2024-04-21 15:00:21.000000 mo_dots-9.600.24114/mo_dots/fields.py
--rw-rw-rw-   0        0        0    10399 2024-04-21 15:00:21.000000 mo_dots-9.600.24114/mo_dots/lists.py
--rw-rw-rw-   0        0        0     6663 2024-04-21 15:00:21.000000 mo_dots-9.600.24114/mo_dots/nones.py
--rw-rw-rw-   0        0        0     5357 2024-04-21 16:31:40.000000 mo_dots-9.600.24114/mo_dots/objects.py
--rw-rw-rw-   0        0        0     1423 2024-04-21 15:00:21.000000 mo_dots-9.600.24114/mo_dots/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-23 01:01:38.643505 mo_dots-9.600.24114/mo_dots.egg-info/
--rw-rw-rw-   0        0        0     5055 2024-04-23 01:01:38.000000 mo_dots-9.600.24114/mo_dots.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2024-04-23 01:01:38.000000 mo_dots-9.600.24114/mo_dots.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 01:01:38.000000 mo_dots-9.600.24114/mo_dots.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-21 02:12:28.000000 mo_dots-9.600.24114/mo_dots.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      241 2024-04-23 01:01:38.000000 mo_dots-9.600.24114/mo_dots.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-23 01:01:38.000000 mo_dots-9.600.24114/mo_dots.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 01:01:38.646871 mo_dots-9.600.24114/setup.cfg
--rw-rw-rw-   0        0        0     4937 2024-04-23 01:01:33.000000 mo_dots-9.600.24114/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 08:54:35.703057 mo_dots-9.601.24115/
+-rw-rw-rw-   0        0        0    16725 2022-02-13 20:11:16.000000 mo_dots-9.601.24115/LICENSE
+-rw-rw-rw-   0        0        0     5055 2024-04-24 08:54:35.701931 mo_dots-9.601.24115/PKG-INFO
+-rw-rw-rw-   0        0        0     3549 2024-04-04 03:46:45.000000 mo_dots-9.601.24115/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 08:54:35.690191 mo_dots-9.601.24115/mo_dots/
+-rw-rw-rw-   0        0        0    13476 2024-04-24 08:54:27.000000 mo_dots-9.601.24115/mo_dots/__init__.py
+-rw-rw-rw-   0        0        0    16609 2024-04-24 08:54:27.000000 mo_dots-9.601.24115/mo_dots/datas.py
+-rw-rw-rw-   0        0        0     4283 2024-04-21 15:00:21.000000 mo_dots-9.601.24115/mo_dots/fields.py
+-rw-rw-rw-   0        0        0    10432 2024-04-24 08:54:27.000000 mo_dots-9.601.24115/mo_dots/lists.py
+-rw-rw-rw-   0        0        0     7076 2024-04-24 08:54:27.000000 mo_dots-9.601.24115/mo_dots/nones.py
+-rw-rw-rw-   0        0        0     5473 2024-04-24 08:54:27.000000 mo_dots-9.601.24115/mo_dots/objects.py
+-rw-rw-rw-   0        0        0     1423 2024-04-21 15:00:21.000000 mo_dots-9.601.24115/mo_dots/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 08:54:35.698693 mo_dots-9.601.24115/mo_dots.egg-info/
+-rw-rw-rw-   0        0        0     5055 2024-04-24 08:54:35.000000 mo_dots-9.601.24115/mo_dots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2024-04-24 08:54:35.000000 mo_dots-9.601.24115/mo_dots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 08:54:35.000000 mo_dots-9.601.24115/mo_dots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-03-21 02:12:28.000000 mo_dots-9.601.24115/mo_dots.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      241 2024-04-24 08:54:35.000000 mo_dots-9.601.24115/mo_dots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-24 08:54:35.000000 mo_dots-9.601.24115/mo_dots.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 08:54:35.703057 mo_dots-9.601.24115/setup.cfg
+-rw-rw-rw-   0        0        0     4937 2024-04-24 08:54:30.000000 mo_dots-9.601.24115/setup.py
```

### Comparing `mo_dots-9.600.24114/LICENSE` & `mo_dots-9.601.24115/LICENSE`

 * *Files identical despite different names*

### Comparing `mo_dots-9.600.24114/PKG-INFO` & `mo_dots-9.601.24115/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-dots
-Version: 9.600.24114
+Version: 9.601.24115
 Summary: More Dots! Dot-access to Python dicts like Javascript
 Home-page: https://github.com/klahnakoski/mo-dots
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `mo_dots-9.600.24114/README.md` & `mo_dots-9.601.24115/README.md`

 * *Files identical despite different names*

### Comparing `mo_dots-9.600.24114/mo_dots/__init__.py` & `mo_dots-9.601.24115/mo_dots/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -471,39 +471,14 @@
         return tuple()
     elif is_many(value):
         return tuple(tuplewrap(v) if is_sequence(v) else v for v in value)
     else:
         return (from_data(value),)
 
 
-def is_null(t):
-    # RETURN True IF EFFECTIVELY NOTHING
-    class_ = t.__class__
-    if class_ in null_types:
-        return True
-    else:
-        try:
-            return t == None
-        except Exception:
-            return False
-
-
-def is_not_null(t):
-    # RETURN True IF EFFECTIVELY SOMETHING
-    class_ = t.__class__
-    if class_ in null_types:
-        return False
-    elif class_ in datas._data_types:
-        return True
-    elif class_ in finite_types and t:
-        return True
-    else:
-        return t != None
-
-
 datawrap = object_to_data
 
 
 # EXPORT
 export("mo_dots.datas", to_data)
 export("mo_dots.datas", from_data)
 export("mo_dots.datas", coalesce)
```

### Comparing `mo_dots-9.600.24114/mo_dots/datas.py` & `mo_dots-9.601.24115/mo_dots/datas.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     MutableMapping,
     OrderedDict,
     first,
 )
 from mo_imports import expect
 
 from mo_dots.fields import split_field, literal_field, concat_field
-from mo_dots.nones import Null, NullType, null_types
+from mo_dots.nones import Null, NullType, null_types, is_null
 from mo_dots.utils import CLASS, SLOT
 from mo_dots.utils import get_logger
 
 (
     _getdefault,
     coalesce,
     listwrap,
@@ -128,15 +128,15 @@
                 else:
                     d = _getdefault(d, n)  # EVERYTHING ELSE TREATS n AS LITERAL
 
             return to_data(d)
         else:
             o = d.get(key)
 
-        if o == None:
+        if is_null(o):
             return NullType(d, key)
         return to_data(o)
 
     def __setitem__(self, key, value):
         if key == "":
             get_logger().error("key is empty string.  Probably a bad idea")
         if key == None:
@@ -419,35 +419,39 @@
     SEE leaves_to_data FOR THE INVERSE
 
     :param value: THE Mapping TO TRAVERSE
     :param prefix:  OPTIONAL PREFIX GIVEN TO EACH KEY
     :return: Data, WHICH EACH KEY BEING A PATH INTO value TREE
     """
     if not prefix:
-        yield from _leaves(".", value)
+        yield from _leaves(".", value, tuple())
     else:
-        for k, v in _leaves(".", value):
+        for k, v in _leaves(".", value, tuple()):
             yield prefix + k, v
 
 
-def _leaves(parent, value):
-    value = from_data(value)
-    obj = object_to_data(value)
-    if obj is value or is_many(value):
+def _leaves(parent, value, path):
+    val = from_data(value)
+    _id = id(val)
+    if _id in path:
+        yield parent, value
+        return
+    obj = object_to_data(val)
+    if obj is val or is_many(val):
         yield parent, value
         return
 
     for k in get_keys(obj):
         try:
             v = obj[literal_field(k)]
             if is_missing(v):
                 continue
             kk = concat_field(parent, literal_field(k))
             vv = object_to_data(v)
-            yield from _leaves(kk, vv)
+            yield from _leaves(kk, vv, path+(_id,))
         except Exception as cause:
             get_logger().error("Do not know how to handle", cause=cause)
 
 
 def _split_field(field):
     """
     SIMPLE SPLIT, NO CHECKS
```

### Comparing `mo_dots-9.600.24114/mo_dots/fields.py` & `mo_dots-9.601.24115/mo_dots/fields.py`

 * *Files identical despite different names*

### Comparing `mo_dots-9.600.24114/mo_dots/lists.py` & `mo_dots-9.601.24115/mo_dots/lists.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,7 +384,8 @@
 export("mo_dots.datas", is_list)
 export("mo_dots.datas", list_to_data)
 export("mo_dots.datas", FlatList)
 export("mo_dots.datas", is_sequence)
 export("mo_dots.datas", is_many)
 
 export("mo_dots.nones", is_sequence)
+export("mo_dots.nones", FlatList)
```

### Comparing `mo_dots-9.600.24114/mo_dots/nones.py` & `mo_dots-9.601.24115/mo_dots/nones.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 from mo_future import none_type
 from mo_imports import expect
 
 from mo_dots.utils import CLASS, KEY, SLOT
 
-to_data, get_attr, is_sequence = expect("to_data", "get_attr", "is_sequence")
+to_data, get_attr, is_sequence, FlatList = expect("to_data", "get_attr", "is_sequence", "FlatList")
 
 _get = object.__getattribute__
 _set = object.__setattr__
 _zero_list = []
 _null_hash = hash(None)
 
 
@@ -281,14 +281,33 @@
                 obj[path0] = old_value = {}
 
         _assign_to_null(old_value, path[1:], value)
     except Exception as e:
         raise e
 
 
+def is_null(value):
+    # RETURN True IF EFFECTIVELY NOTHING
+    _class = _get(value, CLASS)
+    if _class in null_types:
+        return True
+    if _class is FlatList:
+        return not value
+    return False
+
+
+def is_not_null(value):
+    _class = _get(value, CLASS)
+    if _class in null_types:
+        return False
+    if _class is FlatList:
+        return bool(value)
+    return True
+
+
 def _split_field(field):
     """
     SIMPLE SPLIT, NO CHECKS
     """
     if field == ".":
         return []
     else:
```

### Comparing `mo_dots-9.600.24114/mo_dots/objects.py` & `mo_dots-9.601.24115/mo_dots/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 _new = object.__new__
 _get = object.__getattribute__
 _set = object.__setattr__
 
 WRAPPED_CLASSES = set()
 known_types = {}  #  map from type to field names
+ignored_attributes = set(dir(object)) | set(dir(dict.values.__class__))
 
 
 class DataObject(Mapping):
     """
     TREAT AN OBJECT LIKE DATA
     """
 
@@ -122,25 +123,25 @@
     try:
         return obj.__dict__.keys()
     except Exception:
         pass
 
     _type = obj.__class__
     keys = known_types.get(_type)
-    if keys:
+    if keys is not None:
         return keys
 
     try:
         keys = known_types[_type] = _type.__slots__
         return keys
     except Exception:
         pass
 
     keys = known_types[_type] = tuple(
-        k for k in dir(_type) if getattr(_type, k).__class__.__name__ in ["member_descriptor", "getset_descriptor"]
+        k for k in dir(_type) if k not in ignored_attributes and getattr(_type, k).__class__.__name__ in ["member_descriptor", "getset_descriptor"]
     )
     return keys
 
 
 def object_to_data(v):
     try:
         if v == None:
@@ -148,15 +149,15 @@
     except Exception:
         pass
 
     if is_primitive(v):
         return v
 
     type_ = _get(v, CLASS)
-    if type_ is (dict, OrderedDict):
+    if type_ in (dict, OrderedDict):
         m = _new(Data)
         _set(m, SLOT, v)
         return m
     elif type_ is tuple:
         return list_to_data(v)
     elif type_ is list:
         return list_to_data(v)
```

### Comparing `mo_dots-9.600.24114/mo_dots/utils.py` & `mo_dots-9.601.24115/mo_dots/utils.py`

 * *Files identical despite different names*

### Comparing `mo_dots-9.600.24114/mo_dots.egg-info/PKG-INFO` & `mo_dots-9.601.24115/mo_dots.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-dots
-Version: 9.600.24114
+Version: 9.601.24115
 Summary: More Dots! Dot-access to Python dicts like Javascript
 Home-page: https://github.com/klahnakoski/mo-dots
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `mo_dots-9.600.24114/setup.py` & `mo_dots-9.601.24115/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,10 +11,10 @@
     install_requires=["mo-future==7.584.24095","mo-imports==7.584.24095"],
     license='MPL 2.0',
     long_description='\n# More Dots!\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-dots.svg)](https://pypi.org/project/mo-dots/)\n[![Build Status](https://github.com/klahnakoski/mo-dots/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-dots/actions/workflows/build.yml)\n[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-dots/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-dots?branch=dev)\n[![Downloads](https://pepy.tech/badge/mo-dots/month)](https://pepy.tech/project/mo-dots)\n\n#### Changes in version 9.x.x\n\nEscaping a literal dot (`.`) is no longer (`\\\\.`) rather double-dot (`..`). Escaping a literal dot can still be done with bell (`\\b`) \n\n#### Changes in version 5.x.x\n\nThe `Data()` constructor only accepts keyword parameters. It no longer accepts a dict, nor does it attempt to clean the input.  Replace `Data(my_var)` with `to_data(my_var)`\n  \n\n## Overview\n\nThis library defines a `Data` class that can serve as a replacement for `dict`, and acts much like a null-safe dataclass.\n\n> See the [full documentation](https://github.com/klahnakoski/mo-dots/tree/dev/docs) for all the features of `mo-dots`\n\n### Create instances\n\nDefine `Data` using named parameters, just like you would a `dict`\n\n    >>> from mo_dots import Data\n    >>> Data(b=42, c="hello world")\n    Data({\'b\': 42, \'c\': \'hello world\'})\n\nYou can also wrap existing `dict`s so they can be used like `Data`\n\n    >>> from mo_dots import to_data\n    >>> to_data({\'b\': 42, \'c\': \'hello world\'})\n    Data({\'b\': 42, \'c\': \'hello world\'})\n\n### Dot Access\n\nAccess properties with attribute dots: `a.b == a["b"]`. You have probably seen this before.\n\n### Path Access\n\nAccess properties by dot-delimited path.\n\n\t>>> a = to_data({"b": {"c": 42}})\n\t>>> a["b.c"] == 42\n\tTrue\n\n### Safe Access\n\nIf a property does not exist then return `Null` rather than raising an error.\n\n\t>>> a = Data()\n\t>>> a.b == None\n\tTrue\n\t>>> a.b.c == None\n\tTrue\n\t>>> a[None] == None\n\tTrue\n\n### Path assignment\n\nNo need to make intermediate `dicts`\n\n    >>> a = Data()\n    >>> a["b.c"] = 42   # same as a.b.c = 42\n    a == {"b": {"c": 42}}\n\n### Path accumulation\n\nUse `+=` to add to a property; default zero (`0`)\n\n    >>> a = Data()\n    a == {}\n    >>> a.b.c += 1\n    a == {"b": {"c": 1}}\n    >>> a.b.c += 42\n    a == {"b": {"c": 43}}\n\nUse `+=` with a list (`[]`) to append to a list; default empty list (`[]`)\n\n    >>> a = Data()\n    a == {}\n    >>> a.b.c += [1]\n    a == {"b": {"c": [1]}}\n    >>> a.b.c += [42]\n    a == {"b": {"c": [1, 42]}}\n\n## Serializing to JSON\n\nThe standard Python JSON library does not recognize `Data` as serializable.  You may overcome this by providing `default=from_data`; which converts the data structures in this module into Python primitives of the same. \n\n    from mo_dots import from_data, to_data\n    \n    s = to_data({"a": ["b", 1]})\n    result = json.dumps(s, default=from_data)  \n\nAlternatively, you may consider [mo-json](https://pypi.org/project/mo-json/) which has a function `value2json` that converts a larger number of data structures into JSON.\n\n\n## Summary\n\nThis library is the basis for a data transformation algebra: We want a succinct way of transforming data in Python. We want operations on data to result in yet more data. We do not want data operations to raise exceptions. This library is solves Python\'s lack of consistency (lack of closure) under the dot (`.`) and slice `[::]` operators when operating on data objects. \n\n[Full documentation](https://github.com/klahnakoski/mo-dots/tree/dev/docs)\n',
     long_description_content_type='text/markdown',
     name='mo-dots',
     packages=["mo_dots"],
     url='https://github.com/klahnakoski/mo-dots',
-    version='9.600.24114',
+    version='9.601.24115',
     zip_safe=False
 )
```

