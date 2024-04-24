# Comparing `tmp/template_dict-0.1.1-py3-none-any.whl.zip` & `tmp/template_dict-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 7122 bytes, number of entries: 8
--rw-r--r--  2.0 unx      182 b- defN 24-Apr-13 14:19 template_dict/__init__.py
--rw-r--r--  2.0 unx     9928 b- defN 24-Apr-13 14:19 template_dict/templates.py
--rw-r--r--  2.0 unx     1624 b- defN 24-Apr-13 14:19 template_dict/utils.py
--rw-r--r--  2.0 unx     1069 b- defN 24-Apr-13 14:20 template_dict-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3547 b- defN 24-Apr-13 14:20 template_dict-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-13 14:20 template_dict-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 24-Apr-13 14:20 template_dict-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      659 b- defN 24-Apr-13 14:20 template_dict-0.1.1.dist-info/RECORD
-8 files, 17115 bytes uncompressed, 5968 bytes compressed:  65.1%
+Zip file size: 7367 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      243 b- defN 24-Apr-24 18:55 template_dict/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 18:55 template_dict/py.typed
+-rw-r--r--  2.0 unx    10002 b- defN 24-Apr-24 18:55 template_dict/templates.py
+-rw-r--r--  2.0 unx     1661 b- defN 24-Apr-24 18:55 template_dict/utils.py
+-rw-r--r--  2.0 unx     1069 b- defN 24-Apr-24 18:55 template_dict-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3574 b- defN 24-Apr-24 18:55 template_dict-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-24 18:55 template_dict-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 24-Apr-24 18:55 template_dict-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      736 b- defN 24-Apr-24 18:55 template_dict-0.1.2.dist-info/RECORD
+9 files, 17391 bytes uncompressed, 6093 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -1,25 +1,28 @@
 Filename: template_dict/__init__.py
 Comment: 
 
+Filename: template_dict/py.typed
+Comment: 
+
 Filename: template_dict/templates.py
 Comment: 
 
 Filename: template_dict/utils.py
 Comment: 
 
-Filename: template_dict-0.1.1.dist-info/LICENSE
+Filename: template_dict-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: template_dict-0.1.1.dist-info/METADATA
+Filename: template_dict-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: template_dict-0.1.1.dist-info/WHEEL
+Filename: template_dict-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: template_dict-0.1.1.dist-info/top_level.txt
+Filename: template_dict-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: template_dict-0.1.1.dist-info/RECORD
+Filename: template_dict-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## template_dict/__init__.py

```diff
@@ -1,7 +1,9 @@
+"""Python dictionary templates and dictionary functions."""
+
 from template_dict.templates import *
 from template_dict.utils import *
 
 __python_version__ = "3.8"
 __author__ = "violetblackdev@gmail.com"
 __license__ = "MIT"
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

## template_dict/templates.py

```diff
@@ -1,7 +1,9 @@
+"""Templates classes and operators."""
+
 from abc import ABC, abstractmethod
 from ast import literal_eval
 from contextlib import suppress
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, Callable, Dict, Iterable, List, Mapping, Optional, Type, Union
 from uuid import uuid4
@@ -48,15 +50,14 @@
 
         This method should contain operator-specific evaluation logic.
 
         :param args: a tuple of already evaluated arguments
         :param data: dynamic data
         :returns: evaluated operator value
         """
-        ...
 
     def _eval_args(self, data: Mapping[str, Any], /):
         for arg in self.args:
             if isinstance(arg, Operator):
                 arg = arg(data)
             yield arg
 
@@ -287,15 +288,15 @@
             value = tuple(self._parse_value(v, keys, key=key) for v in value)
         return value
 
     def _parse_string(self, s: str, keys: List[str], key: Optional[str] = None) -> Union["Operator", str]:
         if not s:
             return s
 
-        bl, br = self.definitions.operator_brackets
+        bl, br = self.definitions.operator_brackets[0], self.definitions.operator_brackets[1]
         bls, blr = s[0] == bl, s[-1] == br
 
         if not bls and not blr:
             if s[0] == self.definitions.escape_quote and s[-1] == self.definitions.escape_quote:
                 s = s[1:-1]
             return s
         elif not bls or not blr:
@@ -326,10 +327,10 @@
         if isinstance(args[0], str) and args[0].startswith(self.definitions.operator_sign):
             op = args[0][1:]
             args = args[1:]
         else:
             op = self.definitions.default_operator
 
         op_obj = self.operators[op](self, tuple(args))
-        if type(op_obj) is OperatorSelect:
+        if isinstance(op_obj, OperatorSelect):
             keys.extend(arg for arg in args if type(arg) is str)
         return op_obj
```

## template_dict/utils.py

```diff
@@ -1,13 +1,15 @@
+"""Dictionary utility functions."""
+
 from typing import Any, List, Union
 
-__all__ = ['get_field']
+__all__ = ["get_field"]
 
 
-def get_field(__obj, __key: Union[str, List[str]], *, default: Union[Exception, Any] = KeyError, delimiter: str = '.'):
+def get_field(__obj, __key: Union[str, List[str]], *, default: Union[Exception, Any] = KeyError, delimiter: str = "."):
     """Get a field from a nested dict using a flattened key.
 
     >>> get_field({'a': {'b': [1], 'c': 2}}, 'a.b')
     [1]
 
     using a custom delimiter:
```

## Comparing `template_dict-0.1.1.dist-info/LICENSE` & `template_dict-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `template_dict-0.1.1.dist-info/METADATA` & `template_dict-0.1.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: template-dict
-Version: 0.1.1
+Version: 0.1.2
 Summary: Data templates for Python - dynamically fill complex dictionaries with values
 Home-page: https://github.com/violet-black/template-dict
 Author: violetblackdev@gmail.com
 License: MIT
+Keywords: templates,config
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

## Comparing `template_dict-0.1.1.dist-info/RECORD` & `template_dict-0.1.2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-template_dict/__init__.py,sha256=91q6LHZXu3f_PJAddV6J69iAf0pm8EY3kQzL84-mwPY,182
-template_dict/templates.py,sha256=-SW4W4HeJHTdXo529H8Hcs-Xq8DfqddQ48Y7_q9L6hc,9928
-template_dict/utils.py,sha256=5SnHi5zs8g_-c7eS-CZAEfti1DZRpH6pk2Xz4rKYn24,1624
-template_dict-0.1.1.dist-info/LICENSE,sha256=VikX3YBzWiCgZEgI93vz50l4NdJDPjkmxFbYK9IogJ8,1069
-template_dict-0.1.1.dist-info/METADATA,sha256=KbrgRMS5RO2SeE6T_DjdRPI_hbkfVx59NGTLVA4ApLU,3547
-template_dict-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-template_dict-0.1.1.dist-info/top_level.txt,sha256=chh96b_OBgEGknyALRDHkHbpU0qwO0tYeriMi6Bg7Hc,14
-template_dict-0.1.1.dist-info/RECORD,,
+template_dict/__init__.py,sha256=pEBfMxZWHmSBwmlBM-plmm7M6ICY95kyLP8ug6KpaOI,243
+template_dict/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+template_dict/templates.py,sha256=pmtTtc_lW6l8m5yt3bHdcAHnCEDXlPNJt5uuwgy4l74,10002
+template_dict/utils.py,sha256=nqOvzoZYBfvhRLKI_7DaT-kcvK39vyBPYKvPXrtFM5s,1661
+template_dict-0.1.2.dist-info/LICENSE,sha256=VikX3YBzWiCgZEgI93vz50l4NdJDPjkmxFbYK9IogJ8,1069
+template_dict-0.1.2.dist-info/METADATA,sha256=bZVMhR_w_tVs6t7kfTVYA6YjovA5WW4fw_D0xlIgHYc,3574
+template_dict-0.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+template_dict-0.1.2.dist-info/top_level.txt,sha256=chh96b_OBgEGknyALRDHkHbpU0qwO0tYeriMi6Bg7Hc,14
+template_dict-0.1.2.dist-info/RECORD,,
```

