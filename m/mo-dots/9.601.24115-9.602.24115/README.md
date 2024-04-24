# Comparing `tmp/mo_dots-9.601.24115.tar.gz` & `tmp/mo_dots-9.602.24115.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo_dots-9.601.24115.tar", last modified: Wed Apr 24 08:54:35 2024, max compression
+gzip compressed data, was "mo_dots-9.602.24115.tar", last modified: Wed Apr 24 10:11:23 2024, max compression
```

## Comparing `mo_dots-9.601.24115.tar` & `mo_dots-9.602.24115.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 08:54:35.703057 mo_dots-9.601.24115/
--rw-rw-rw-   0        0        0    16725 2022-02-13 20:11:16.000000 mo_dots-9.601.24115/LICENSE
--rw-rw-rw-   0        0        0     5055 2024-04-24 08:54:35.701931 mo_dots-9.601.24115/PKG-INFO
--rw-rw-rw-   0        0        0     3549 2024-04-04 03:46:45.000000 mo_dots-9.601.24115/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 08:54:35.690191 mo_dots-9.601.24115/mo_dots/
--rw-rw-rw-   0        0        0    13476 2024-04-24 08:54:27.000000 mo_dots-9.601.24115/mo_dots/__init__.py
--rw-rw-rw-   0        0        0    16609 2024-04-24 08:54:27.000000 mo_dots-9.601.24115/mo_dots/datas.py
--rw-rw-rw-   0        0        0     4283 2024-04-21 15:00:21.000000 mo_dots-9.601.24115/mo_dots/fields.py
--rw-rw-rw-   0        0        0    10432 2024-04-24 08:54:27.000000 mo_dots-9.601.24115/mo_dots/lists.py
--rw-rw-rw-   0        0        0     7076 2024-04-24 08:54:27.000000 mo_dots-9.601.24115/mo_dots/nones.py
--rw-rw-rw-   0        0        0     5473 2024-04-24 08:54:27.000000 mo_dots-9.601.24115/mo_dots/objects.py
--rw-rw-rw-   0        0        0     1423 2024-04-21 15:00:21.000000 mo_dots-9.601.24115/mo_dots/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-24 08:54:35.698693 mo_dots-9.601.24115/mo_dots.egg-info/
--rw-rw-rw-   0        0        0     5055 2024-04-24 08:54:35.000000 mo_dots-9.601.24115/mo_dots.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2024-04-24 08:54:35.000000 mo_dots-9.601.24115/mo_dots.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 08:54:35.000000 mo_dots-9.601.24115/mo_dots.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-21 02:12:28.000000 mo_dots-9.601.24115/mo_dots.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      241 2024-04-24 08:54:35.000000 mo_dots-9.601.24115/mo_dots.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-24 08:54:35.000000 mo_dots-9.601.24115/mo_dots.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 08:54:35.703057 mo_dots-9.601.24115/setup.cfg
--rw-rw-rw-   0        0        0     4937 2024-04-24 08:54:30.000000 mo_dots-9.601.24115/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:11:23.836866 mo_dots-9.602.24115/
+-rw-rw-rw-   0        0        0    16725 2022-02-13 20:11:16.000000 mo_dots-9.602.24115/LICENSE
+-rw-rw-rw-   0        0        0     5055 2024-04-24 10:11:23.835581 mo_dots-9.602.24115/PKG-INFO
+-rw-rw-rw-   0        0        0     3549 2024-04-04 03:46:45.000000 mo_dots-9.602.24115/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 10:11:23.820639 mo_dots-9.602.24115/mo_dots/
+-rw-rw-rw-   0        0        0    13479 2024-04-24 10:11:14.000000 mo_dots-9.602.24115/mo_dots/__init__.py
+-rw-rw-rw-   0        0        0    16615 2024-04-24 10:11:14.000000 mo_dots-9.602.24115/mo_dots/datas.py
+-rw-rw-rw-   0        0        0     4324 2024-04-24 10:11:14.000000 mo_dots-9.602.24115/mo_dots/fields.py
+-rw-rw-rw-   0        0        0    10450 2024-04-24 10:11:14.000000 mo_dots-9.602.24115/mo_dots/lists.py
+-rw-rw-rw-   0        0        0     7076 2024-04-24 08:54:27.000000 mo_dots-9.602.24115/mo_dots/nones.py
+-rw-rw-rw-   0        0        0     5476 2024-04-24 10:11:14.000000 mo_dots-9.602.24115/mo_dots/objects.py
+-rw-rw-rw-   0        0        0     1423 2024-04-24 10:04:39.000000 mo_dots-9.602.24115/mo_dots/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:11:23.830968 mo_dots-9.602.24115/mo_dots.egg-info/
+-rw-rw-rw-   0        0        0     5055 2024-04-24 10:11:23.000000 mo_dots-9.602.24115/mo_dots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2024-04-24 10:11:23.000000 mo_dots-9.602.24115/mo_dots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 10:11:23.000000 mo_dots-9.602.24115/mo_dots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-03-21 02:12:28.000000 mo_dots-9.602.24115/mo_dots.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      241 2024-04-24 10:11:23.000000 mo_dots-9.602.24115/mo_dots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-24 10:11:23.000000 mo_dots-9.602.24115/mo_dots.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 10:11:23.836866 mo_dots-9.602.24115/setup.cfg
+-rw-rw-rw-   0        0        0     4937 2024-04-24 10:11:18.000000 mo_dots-9.602.24115/setup.py
```

### Comparing `mo_dots-9.601.24115/LICENSE` & `mo_dots-9.602.24115/LICENSE`

 * *Files identical despite different names*

### Comparing `mo_dots-9.601.24115/PKG-INFO` & `mo_dots-9.602.24115/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-dots
-Version: 9.601.24115
+Version: 9.602.24115
 Summary: More Dots! Dot-access to Python dicts like Javascript
 Home-page: https://github.com/klahnakoski/mo-dots
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `mo_dots-9.601.24115/README.md` & `mo_dots-9.602.24115/README.md`

 * *Files identical despite different names*

### Comparing `mo_dots-9.601.24115/mo_dots/__init__.py` & `mo_dots-9.602.24115/mo_dots/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
     except Exception as f:
         pass
 
     if is_sequence(obj):
         return [_getdefault(o, key) for o in obj]
 
     try:
-        if obj.__class__ is not dict:
+        if _get(obj, CLASS) is not dict:
             return getattr(obj, key)
     except Exception as f:
         pass
 
     try:
         if float(key) == round(float(key), 0):
             return obj[int(key)]
```

### Comparing `mo_dots-9.601.24115/mo_dots/datas.py` & `mo_dots-9.602.24115/mo_dots/datas.py`

 * *Files 0% similar despite different names*

```diff
@@ -534,20 +534,20 @@
 
 
 def is_data(d):
     """
     :param d:
     :return: True IF d IS A TYPE THAT HOLDS DATA
     """
-    return d.__class__ in _data_types
+    return _get(d, CLASS) in _data_types
 
 
 def is_missing(t) -> bool:
     # RETURN True IF EFFECTIVELY NOTHING
-    class_ = t.__class__
+    class_ = _get(t, CLASS)
     if class_ in null_types:
         return True
     elif class_ in _data_types:
         return False
     elif class_ in finite_types and not t:
         return True
     elif class_ is text and not t:
```

### Comparing `mo_dots-9.601.24115/mo_dots/fields.py` & `mo_dots-9.602.24115/mo_dots/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import re
 import sys
 
 from mo_future import generator_types, flatten
 
-from mo_dots.utils import get_logger
+from mo_dots.utils import get_logger, CLASS
 
 _module_type = type(sys.modules[__name__])
 _builtin_zip = zip
+_get = object.__getattribute__
 
 
 ESCAPE_DOTS1 = re.compile(r"(^\.|\.$)")  # DOTS AT START/END
 ESCAPE_DOTS2 = re.compile(r"(?<!^)\.(?!$)")  # INTERNAL DOTS
 ILLEGAL_DOTS = re.compile(r"[^.]\.(?:\.\.)+")  # ODD DOTS ARE NOT ALLOWED
 SPLIT_DOTS = re.compile(r"(?<!\.)\.(?!\.)")  # SINGLE DOTS
 UNESCAPE_DOTS = re.compile(r"\x08|(?:\.\.)")  # ENCODED DOTS
@@ -69,15 +70,15 @@
         return [UNESCAPE_DOTS.sub(".", k) for k in SPLIT_DOTS.split(field) if k]
 
 
 def join_field(path):
     """
     RETURN field SEQUENCE AS STRING
     """
-    if path.__class__ in generator_types:
+    if _get(path, CLASS) in generator_types:
         path = list(path)
 
     if not path:
         return "."
 
     prefix = ""
     while True:
```

### Comparing `mo_dots-9.601.24115/mo_dots/lists.py` & `mo_dots-9.602.24115/mo_dots/lists.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     __slots__ = [SLOT]
 
     def __init__(self, vals=None):
         """ USE THE vals, NOT A COPY """
         # list.__init__(self)
         if vals == None:
             _set(self, SLOT, [])
-        elif vals.__class__ is FlatList:
+        elif _get(vals, CLASS) is FlatList:
             _set(self, SLOT, vals.list)
         else:
             _set(self, SLOT, vals)
 
     def __getitem__(self, index):
         if index == ".":
             return self
@@ -326,40 +326,40 @@
 
 # ITERATORS THAT ARE CONSIDERED PRIMITIVE
 not_many_names = ("str", "unicode", "binary", "NullType", "NoneType", "dict", "Data")
 
 
 def is_list(l):
     # ORDERED, AND CAN CHANGE CONTENTS
-    return l.__class__ in list_types
+    return _get(l, CLASS) in list_types
 
 
 def is_container(l):
     # CAN ADD AND REMOVE ELEMENTS
-    return l.__class__ in container_types
+    return _get(l, CLASS) in container_types
 
 
 def is_sequence(l):
     # HAS AN ORDER, INCLUDES GENERATORS
-    return l.__class__ in sequence_types
+    return _get(l, CLASS) in sequence_types
 
 
 def is_finite(l):
     # CAN PERFORM len(l); NOT A GENERATOR
-    return l.__class__ in finite_types
+    return _get(l, CLASS) in finite_types
 
 
 def is_many(value):
     # REPRESENTS MULTIPLE VALUES
     # TODO: CLEAN UP THIS LOGIC
     # THIS IS COMPLICATED BECAUSE I AM UNSURE ABOUT ALL THE "PRIMITIVE TYPES"
     # I WOULD LIKE TO POSITIVELY CATCH many_types, BUT MAYBE IT IS EASIER TO DETECT: Iterable, BUT NOT PRIMITIVE
     # UNTIL WE HAVE A COMPLETE SLOT, WE KEEP ALL THIS warning() CODE
     global _many_types
-    type_ = value.__class__
+    type_ = _get(value, CLASS)
     if type_ in _many_types:
         return True
 
     if issubclass(type_, types.GeneratorType):
         _many_types = _many_types + (type_,)
         Log.warning("is_many() can not detect generator {{type}}", type=type_.__name__)
         return True
```

### Comparing `mo_dots-9.601.24115/mo_dots/nones.py` & `mo_dots-9.602.24115/mo_dots/nones.py`

 * *Files identical despite different names*

### Comparing `mo_dots-9.601.24115/mo_dots/objects.py` & `mo_dots-9.602.24115/mo_dots/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         return obj.keys()
 
     try:
         return obj.__dict__.keys()
     except Exception:
         pass
 
-    _type = obj.__class__
+    _type = _get(obj, CLASS)
     keys = known_types.get(_type)
     if keys is not None:
         return keys
 
     try:
         keys = known_types[_type] = _type.__slots__
         return keys
```

### Comparing `mo_dots-9.601.24115/mo_dots/utils.py` & `mo_dots-9.602.24115/mo_dots/utils.py`

 * *Files identical despite different names*

### Comparing `mo_dots-9.601.24115/mo_dots.egg-info/PKG-INFO` & `mo_dots-9.602.24115/mo_dots.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-dots
-Version: 9.601.24115
+Version: 9.602.24115
 Summary: More Dots! Dot-access to Python dicts like Javascript
 Home-page: https://github.com/klahnakoski/mo-dots
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `mo_dots-9.601.24115/setup.py` & `mo_dots-9.602.24115/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,10 +11,10 @@
     install_requires=["mo-future==7.584.24095","mo-imports==7.584.24095"],
     license='MPL 2.0',
     long_description='\n# More Dots!\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-dots.svg)](https://pypi.org/project/mo-dots/)\n[![Build Status](https://github.com/klahnakoski/mo-dots/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-dots/actions/workflows/build.yml)\n[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-dots/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-dots?branch=dev)\n[![Downloads](https://pepy.tech/badge/mo-dots/month)](https://pepy.tech/project/mo-dots)\n\n#### Changes in version 9.x.x\n\nEscaping a literal dot (`.`) is no longer (`\\\\.`) rather double-dot (`..`). Escaping a literal dot can still be done with bell (`\\b`) \n\n#### Changes in version 5.x.x\n\nThe `Data()` constructor only accepts keyword parameters. It no longer accepts a dict, nor does it attempt to clean the input.  Replace `Data(my_var)` with `to_data(my_var)`\n  \n\n## Overview\n\nThis library defines a `Data` class that can serve as a replacement for `dict`, and acts much like a null-safe dataclass.\n\n> See the [full documentation](https://github.com/klahnakoski/mo-dots/tree/dev/docs) for all the features of `mo-dots`\n\n### Create instances\n\nDefine `Data` using named parameters, just like you would a `dict`\n\n    >>> from mo_dots import Data\n    >>> Data(b=42, c="hello world")\n    Data({\'b\': 42, \'c\': \'hello world\'})\n\nYou can also wrap existing `dict`s so they can be used like `Data`\n\n    >>> from mo_dots import to_data\n    >>> to_data({\'b\': 42, \'c\': \'hello world\'})\n    Data({\'b\': 42, \'c\': \'hello world\'})\n\n### Dot Access\n\nAccess properties with attribute dots: `a.b == a["b"]`. You have probably seen this before.\n\n### Path Access\n\nAccess properties by dot-delimited path.\n\n\t>>> a = to_data({"b": {"c": 42}})\n\t>>> a["b.c"] == 42\n\tTrue\n\n### Safe Access\n\nIf a property does not exist then return `Null` rather than raising an error.\n\n\t>>> a = Data()\n\t>>> a.b == None\n\tTrue\n\t>>> a.b.c == None\n\tTrue\n\t>>> a[None] == None\n\tTrue\n\n### Path assignment\n\nNo need to make intermediate `dicts`\n\n    >>> a = Data()\n    >>> a["b.c"] = 42   # same as a.b.c = 42\n    a == {"b": {"c": 42}}\n\n### Path accumulation\n\nUse `+=` to add to a property; default zero (`0`)\n\n    >>> a = Data()\n    a == {}\n    >>> a.b.c += 1\n    a == {"b": {"c": 1}}\n    >>> a.b.c += 42\n    a == {"b": {"c": 43}}\n\nUse `+=` with a list (`[]`) to append to a list; default empty list (`[]`)\n\n    >>> a = Data()\n    a == {}\n    >>> a.b.c += [1]\n    a == {"b": {"c": [1]}}\n    >>> a.b.c += [42]\n    a == {"b": {"c": [1, 42]}}\n\n## Serializing to JSON\n\nThe standard Python JSON library does not recognize `Data` as serializable.  You may overcome this by providing `default=from_data`; which converts the data structures in this module into Python primitives of the same. \n\n    from mo_dots import from_data, to_data\n    \n    s = to_data({"a": ["b", 1]})\n    result = json.dumps(s, default=from_data)  \n\nAlternatively, you may consider [mo-json](https://pypi.org/project/mo-json/) which has a function `value2json` that converts a larger number of data structures into JSON.\n\n\n## Summary\n\nThis library is the basis for a data transformation algebra: We want a succinct way of transforming data in Python. We want operations on data to result in yet more data. We do not want data operations to raise exceptions. This library is solves Python\'s lack of consistency (lack of closure) under the dot (`.`) and slice `[::]` operators when operating on data objects. \n\n[Full documentation](https://github.com/klahnakoski/mo-dots/tree/dev/docs)\n',
     long_description_content_type='text/markdown',
     name='mo-dots',
     packages=["mo_dots"],
     url='https://github.com/klahnakoski/mo-dots',
-    version='9.601.24115',
+    version='9.602.24115',
     zip_safe=False
 )
```

