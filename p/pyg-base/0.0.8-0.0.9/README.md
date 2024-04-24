# Comparing `tmp/pyg-base-0.0.8.tar.gz` & `tmp/pyg-base-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyg-base-0.0.8.tar", last modified: Fri Jan  7 18:50:58 2022, max compression
+gzip compressed data, was "pyg-base-0.0.9.tar", last modified: Fri Jan 21 00:09:10 2022, max compression
```

## Comparing `pyg-base-0.0.8.tar` & `pyg-base-0.0.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2022-01-07 18:50:58.875037 pyg-base-0.0.8/
--rw-rw-rw-   0        0        0     1091 2021-12-07 01:05:04.000000 pyg-base-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1125 2022-01-07 18:50:58.876034 pyg-base-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      540 2021-12-09 01:32:13.000000 pyg-base-0.0.8/README.md
--rw-rw-rw-   0        0        0      108 2021-12-07 00:38:43.000000 pyg-base-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      758 2022-01-07 18:50:58.886011 pyg-base-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-01-07 18:50:58.788275 pyg-base-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2022-01-07 18:50:58.866062 pyg-base-0.0.8/src/pyg_base/
--rw-rw-rw-   0        0        0     2909 2022-01-06 14:31:48.000000 pyg-base-0.0.8/src/pyg_base/__init__.py
--rw-rw-rw-   0        0        0     9063 2021-12-06 23:15:36.000000 pyg-base-0.0.8/src/pyg_base/_acell.py
--rw-rw-rw-   0        0        0     1081 2021-12-06 23:15:35.000000 pyg-base-0.0.8/src/pyg_base/_as_float.py
--rw-rw-rw-   0        0        0     4961 2021-12-06 23:15:33.000000 pyg-base-0.0.8/src/pyg_base/_as_list.py
--rw-rw-rw-   0        0        0     2657 2021-12-07 00:29:56.000000 pyg-base-0.0.8/src/pyg_base/_cache.py
--rw-rw-rw-   0        0        0    29407 2021-12-09 00:19:28.000000 pyg-base-0.0.8/src/pyg_base/_cell.py
--rw-rw-rw-   0        0        0     1186 2022-01-03 22:26:33.000000 pyg-base-0.0.8/src/pyg_base/_cfg.py
--rw-rw-rw-   0        0        0     7218 2022-01-06 14:40:23.000000 pyg-base-0.0.8/src/pyg_base/_dag.py
--rw-rw-rw-   0        0        0    16701 2022-01-07 18:39:30.000000 pyg-base-0.0.8/src/pyg_base/_dates.py
--rw-rw-rw-   0        0        0    10699 2022-01-06 14:41:31.000000 pyg-base-0.0.8/src/pyg_base/_decorators.py
--rw-rw-rw-   0        0        0    15737 2021-12-06 23:15:22.000000 pyg-base-0.0.8/src/pyg_base/_dict.py
--rw-rw-rw-   0        0        0    41191 2021-12-06 23:15:20.000000 pyg-base-0.0.8/src/pyg_base/_dictable.py
--rw-rw-rw-   0        0        0     9918 2022-01-06 14:36:36.000000 pyg-base-0.0.8/src/pyg_base/_dictattr.py
--rw-rw-rw-   0        0        0    28466 2021-12-23 11:37:33.000000 pyg-base-0.0.8/src/pyg_base/_drange.py
--rw-rw-rw-   0        0        0     8288 2021-12-07 19:42:03.000000 pyg-base-0.0.8/src/pyg_base/_encode.py
--rw-rw-rw-   0        0        0     4452 2021-02-15 15:59:03.000000 pyg-base-0.0.8/src/pyg_base/_eq.py
--rw-rw-rw-   0        0        0      764 2022-01-06 14:29:14.000000 pyg-base-0.0.8/src/pyg_base/_file.py
--rw-rw-rw-   0        0        0     3130 2021-12-06 23:14:47.000000 pyg-base-0.0.8/src/pyg_base/_getitem.py
--rw-rw-rw-   0        0        0     9583 2021-11-15 18:28:36.000000 pyg-base-0.0.8/src/pyg_base/_inspect.py
--rw-rw-rw-   0        0        0     1516 2021-02-11 21:51:36.000000 pyg-base-0.0.8/src/pyg_base/_logger.py
--rw-rw-rw-   0        0        0    10799 2021-12-06 23:15:12.000000 pyg-base-0.0.8/src/pyg_base/_loop.py
--rw-rw-rw-   0        0        0     8122 2021-12-06 23:15:50.000000 pyg-base-0.0.8/src/pyg_base/_named_dict.py
--rw-rw-rw-   0        0        0    42295 2021-12-29 04:20:49.000000 pyg-base-0.0.8/src/pyg_base/_pandas.py
--rw-rw-rw-   0        0        0     3439 2022-01-06 14:41:28.000000 pyg-base-0.0.8/src/pyg_base/_parquet.py
--rw-rw-rw-   0        0        0    16882 2021-12-06 23:16:27.000000 pyg-base-0.0.8/src/pyg_base/_perdictable.py
--rw-rw-rw-   0        0        0     2280 2021-12-06 23:16:34.000000 pyg-base-0.0.8/src/pyg_base/_reducer.py
--rw-rw-rw-   0        0        0     8328 2022-01-02 23:18:07.000000 pyg-base-0.0.8/src/pyg_base/_sort.py
--rw-rw-rw-   0        0        0     2661 2021-12-06 23:16:58.000000 pyg-base-0.0.8/src/pyg_base/_tree.py
--rw-rw-rw-   0        0        0     2541 2021-12-06 23:16:50.000000 pyg-base-0.0.8/src/pyg_base/_tree_repr.py
--rw-rw-rw-   0        0        0     8103 2021-12-06 23:17:06.000000 pyg-base-0.0.8/src/pyg_base/_txt.py
--rw-rw-rw-   0        0        0     5063 2021-12-06 23:17:14.000000 pyg-base-0.0.8/src/pyg_base/_types.py
--rw-rw-rw-   0        0        0     2376 2021-12-06 23:17:23.000000 pyg-base-0.0.8/src/pyg_base/_ulist.py
--rw-rw-rw-   0        0        0     2855 2021-12-06 23:17:31.000000 pyg-base-0.0.8/src/pyg_base/_waiter.py
--rw-rw-rw-   0        0        0     2021 2021-12-06 23:17:42.000000 pyg-base-0.0.8/src/pyg_base/_zip.py
-drwxrwxrwx   0        0        0        0 2022-01-07 18:50:58.875037 pyg-base-0.0.8/src/pyg_base.egg-info/
--rw-rw-rw-   0        0        0     1125 2022-01-07 18:50:58.000000 pyg-base-0.0.8/src/pyg_base.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1125 2021-12-23 20:18:04.000000 pyg-base-0.0.8/src/pyg_base.egg-info/PKG-INFO (DESKTOP-27SMATF's conflicted copy 2022-01-03)
--rw-rw-rw-   0        0        0     1110 2022-01-07 18:50:58.000000 pyg-base-0.0.8/src/pyg_base.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-07 18:50:58.000000 pyg-base-0.0.8/src/pyg_base.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2022-01-07 18:50:58.000000 pyg-base-0.0.8/src/pyg_base.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-01-07 18:50:58.000000 pyg-base-0.0.8/src/pyg_base.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-01-21 00:09:10.614687 pyg-base-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2021-12-07 01:05:04.000000 pyg-base-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1125 2022-01-21 00:09:10.615684 pyg-base-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      540 2021-12-09 01:32:13.000000 pyg-base-0.0.9/README.md
+-rw-rw-rw-   0        0        0      108 2021-12-07 00:38:43.000000 pyg-base-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      758 2022-01-21 00:09:10.617679 pyg-base-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-01-21 00:09:10.517945 pyg-base-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2022-01-21 00:09:10.584782 pyg-base-0.0.9/src/pyg_base/
+-rw-rw-rw-   0        0        0     2909 2022-01-06 14:31:48.000000 pyg-base-0.0.9/src/pyg_base/__init__.py
+-rw-rw-rw-   0        0        0     9063 2021-12-06 23:15:36.000000 pyg-base-0.0.9/src/pyg_base/_acell.py
+-rw-rw-rw-   0        0        0     1686 2022-01-08 23:54:00.000000 pyg-base-0.0.9/src/pyg_base/_as_float.py
+-rw-rw-rw-   0        0        0     4961 2021-12-06 23:15:33.000000 pyg-base-0.0.9/src/pyg_base/_as_list.py
+-rw-rw-rw-   0        0        0     2657 2021-12-07 00:29:56.000000 pyg-base-0.0.9/src/pyg_base/_cache.py
+-rw-rw-rw-   0        0        0    29807 2022-01-20 23:57:42.000000 pyg-base-0.0.9/src/pyg_base/_cell.py
+-rw-rw-rw-   0        0        0     1186 2022-01-03 22:26:33.000000 pyg-base-0.0.9/src/pyg_base/_cfg.py
+-rw-rw-rw-   0        0        0     7218 2022-01-06 14:40:23.000000 pyg-base-0.0.9/src/pyg_base/_dag.py
+-rw-rw-rw-   0        0        0    16701 2022-01-07 18:39:30.000000 pyg-base-0.0.9/src/pyg_base/_dates.py
+-rw-rw-rw-   0        0        0    10699 2022-01-06 14:41:31.000000 pyg-base-0.0.9/src/pyg_base/_decorators.py
+-rw-rw-rw-   0        0        0    15737 2021-12-06 23:15:22.000000 pyg-base-0.0.9/src/pyg_base/_dict.py
+-rw-rw-rw-   0        0        0    42604 2022-01-21 00:06:36.000000 pyg-base-0.0.9/src/pyg_base/_dictable.py
+-rw-rw-rw-   0        0        0     9918 2022-01-06 14:36:36.000000 pyg-base-0.0.9/src/pyg_base/_dictattr.py
+-rw-rw-rw-   0        0        0    28466 2021-12-23 11:37:33.000000 pyg-base-0.0.9/src/pyg_base/_drange.py
+-rw-rw-rw-   0        0        0     8288 2021-12-07 19:42:03.000000 pyg-base-0.0.9/src/pyg_base/_encode.py
+-rw-rw-rw-   0        0        0     4452 2021-02-15 15:59:03.000000 pyg-base-0.0.9/src/pyg_base/_eq.py
+-rw-rw-rw-   0        0        0      764 2022-01-06 14:29:14.000000 pyg-base-0.0.9/src/pyg_base/_file.py
+-rw-rw-rw-   0        0        0     3130 2021-12-06 23:14:47.000000 pyg-base-0.0.9/src/pyg_base/_getitem.py
+-rw-rw-rw-   0        0        0     9583 2021-11-15 18:28:36.000000 pyg-base-0.0.9/src/pyg_base/_inspect.py
+-rw-rw-rw-   0        0        0     1516 2021-02-11 21:51:36.000000 pyg-base-0.0.9/src/pyg_base/_logger.py
+-rw-rw-rw-   0        0        0    10799 2021-12-06 23:15:12.000000 pyg-base-0.0.9/src/pyg_base/_loop.py
+-rw-rw-rw-   0        0        0     8122 2021-12-06 23:15:50.000000 pyg-base-0.0.9/src/pyg_base/_named_dict.py
+-rw-rw-rw-   0        0        0    42277 2022-01-20 15:27:25.000000 pyg-base-0.0.9/src/pyg_base/_pandas.py
+-rw-rw-rw-   0        0        0     3439 2022-01-06 14:41:28.000000 pyg-base-0.0.9/src/pyg_base/_parquet.py
+-rw-rw-rw-   0        0        0    16882 2021-12-06 23:16:27.000000 pyg-base-0.0.9/src/pyg_base/_perdictable.py
+-rw-rw-rw-   0        0        0     2280 2021-12-06 23:16:34.000000 pyg-base-0.0.9/src/pyg_base/_reducer.py
+-rw-rw-rw-   0        0        0     8328 2022-01-02 23:18:07.000000 pyg-base-0.0.9/src/pyg_base/_sort.py
+-rw-rw-rw-   0        0        0     2661 2021-12-06 23:16:58.000000 pyg-base-0.0.9/src/pyg_base/_tree.py
+-rw-rw-rw-   0        0        0     2541 2021-12-06 23:16:50.000000 pyg-base-0.0.9/src/pyg_base/_tree_repr.py
+-rw-rw-rw-   0        0        0     8103 2021-12-06 23:17:06.000000 pyg-base-0.0.9/src/pyg_base/_txt.py
+-rw-rw-rw-   0        0        0     5063 2021-12-06 23:17:14.000000 pyg-base-0.0.9/src/pyg_base/_types.py
+-rw-rw-rw-   0        0        0     2376 2021-12-06 23:17:23.000000 pyg-base-0.0.9/src/pyg_base/_ulist.py
+-rw-rw-rw-   0        0        0     2855 2021-12-06 23:17:31.000000 pyg-base-0.0.9/src/pyg_base/_waiter.py
+-rw-rw-rw-   0        0        0     2021 2021-12-06 23:17:42.000000 pyg-base-0.0.9/src/pyg_base/_zip.py
+drwxrwxrwx   0        0        0        0 2022-01-21 00:09:10.613690 pyg-base-0.0.9/src/pyg_base.egg-info/
+-rw-rw-rw-   0        0        0     1125 2022-01-21 00:09:10.000000 pyg-base-0.0.9/src/pyg_base.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1125 2021-12-23 20:18:04.000000 pyg-base-0.0.9/src/pyg_base.egg-info/PKG-INFO (DESKTOP-27SMATF's conflicted copy 2022-01-03)
+-rw-rw-rw-   0        0        0     1110 2022-01-21 00:09:10.000000 pyg-base-0.0.9/src/pyg_base.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-01-21 00:09:10.000000 pyg-base-0.0.9/src/pyg_base.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2022-01-21 00:09:10.000000 pyg-base-0.0.9/src/pyg_base.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2022-01-21 00:09:10.000000 pyg-base-0.0.9/src/pyg_base.egg-info/top_level.txt
```

### Comparing `pyg-base-0.0.8/LICENSE` & `pyg-base-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/PKG-INFO` & `pyg-base-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyg-base
-Version: 0.0.8
+Version: 0.0.9
 Summary: Utilities for data manipulation including creation of DAGs and tables
 Home-page: https://github.com/gityoav/pyg-base
 Author: Yoav Git
 Author-email: yoav.git@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/gityoav/pyg-base/issues
 Platform: UNKNOWN
```

### Comparing `pyg-base-0.0.8/README.md` & `pyg-base-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/setup.cfg` & `pyg-base-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7967 2d62 6173 650d 0a76 6572   = pyg-base..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e38 0d0a 6175  sion = 0.0.8..au
+00000020: 7369 6f6e 203d 2030 2e30 2e39 0d0a 6175  sion = 0.0.9..au
 00000030: 7468 6f72 203d 2059 6f61 7620 4769 740d  thor = Yoav Git.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 796f 6176 2e67 6974 4067 6d61 696c 2e63  yoav.git@gmail.c
 00000060: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
 00000070: 3d20 5574 696c 6974 6965 7320 666f 7220  = Utilities for 
 00000080: 6461 7461 206d 616e 6970 756c 6174 696f  data manipulatio
 00000090: 6e20 696e 636c 7564 696e 6720 6372 6561  n including crea
```

### Comparing `pyg-base-0.0.8/src/pyg_base/__init__.py` & `pyg-base-0.0.9/src/pyg_base/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base/_acell.py` & `pyg-base-0.0.9/src/pyg_base/_acell.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base/_as_float.py` & `pyg-base-0.0.9/src/pyg_base/_as_float.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 _k = {0 : '', 3 : 'k', 6:'m', 9:'b', 12: 't', -2 : '%'}
 _n = {v: 10**k for k,v in _k.items()}
 
 __all__ = ['as_float']
 
 @loop(list, tuple, dict)
-def as_float(value):
+def _as_float(value):
     """
     converts a string to float
 
     :Parameters:
     ----------
     value : string
         number in string format.
@@ -35,13 +35,38 @@
             return None
         if txt[-1] in _n:
             mult = _n[txt[-1]]
             txt = txt[:-1]
         else:
             mult = 1
         try:
-            return mult * float(txt)
+            res = mult * float(txt)
+            res = round(res, len(txt)+2)
+            return res
         except ValueError:
             return None
     else:
         return value
 
+def as_float(value):
+    """
+    converts a string to float allowing for commas, percentages etc.
+
+    :Parameters:
+    ----------
+    value : string
+        number in string format.
+
+    :Returns:
+    -------
+    float
+
+    :Example:
+    --------
+    >>> from pyg import *
+    >>> assert as_float('1.3k') == 1300
+    >>> assert as_float('1.4m') == 1400000
+    >>> assert as_float('100%') == 1
+    >>> assert as_float('1,234') == 1234
+    >>> assert as_float('-1,234k') == -1234000
+    """
+    return _as_float(value)
```

### Comparing `pyg-base-0.0.8/src/pyg_base/_as_list.py` & `pyg-base-0.0.9/src/pyg_base/_as_list.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base/_cache.py` & `pyg-base-0.0.9/src/pyg_base/_cache.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base/_cell.py` & `pyg-base-0.0.9/src/pyg_base/_cell.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,28 +57,26 @@
                 return tree_getitem(value, key)
             else:
                 try:
                     return value[output[0]]
                 except KeyError:
                     return tree_getitem(value, key)
     else:
+        if not key_before_data:
+            if _data == output[0]:
+                return value[_data]
         if key is not None:
             try:
                 return tree_getitem(value, key)
             except Exception:
-                if _data == output[0]:
-                    return value[_data]
-                else:
-                    return Dict(value)[output]
-        else:
-            if _data == output[0]:
-                return value[_data]
-            else:            
-                return Dict(value)[output]
-            
+                pass
+        if _data == output[0]:
+            return value[_data]
+        else:            
+            return Dict(value)[output]
         
 
 def cell_clear(value):
     """
     cell_clear clears a cell of its output so that it contains only the essentil stuff to do its calculations.
     This will be used when we save the cell or we want to recalculate it.
     
@@ -108,40 +106,45 @@
         return type(value)([cell_clear(v) for v in value])
     elif isinstance(value, dict):
         return type(value)(**{k : cell_clear(v) for k, v in value.items()})
     else:
         return value
 
 
-def cell_item(value, key = None):
+def cell_item(value, key = None, key_before_data = False):
     """
     returns an item from a cell (if not cell, returns back the value).
     If no key is provided, will return the output of the cell
     
     :Parameters:
     ------------------
     value : cell or object or list of cells/objects
         cell
     key : str, optional
         The key within cell we are interested in. Note that key is treated as GUIDANCE only. 
         Our strong preference is to return valid output from cell_output(cell)
 
+    key_before_data: bool
+        We usually give preference to reserved keyword 'data' when we grab a cell, even if a key is provided
+        So if a cell contains both the data and the key, we will return cell[data] by default
+        Set key_before_data = True to search for key values first
+        
     :Example: non cells
     ---------------------------------
     >>> assert cell_item(1) == 1
     >>> assert cell_item(dict(a=1,b=2)) == dict(a=1,b=2)
 
     :Example: cells, simple
     ----------------------------
     >>> c = cell(lambda a, b: a+b, a = 1, b = 2)
     >>> assert cell_item(c) is None
     >>> assert cell_item(c.go()) == 3
 
     """
-    return _cell_item(value, key = key)
+    return _cell_item(value, key = key, key_before_data = key_before_data)
 
 @loop(list, tuple)
 def _cell_go(value, go, mode = 0):
     if isinstance(value, cell):
         if value._awaitable:
             return value
         else:
@@ -419,17 +422,20 @@
         ---------
         >>> c = cell(lambda x: x+1, x = 1)
         >>> assert c.run()
         >>> c = c()
         >>> assert c.data == 2 and not c.run()
         """
         output = cell_output(self)
-        for o in output:
-            if self.get(o) is None:
-                return True
+        if _data in output:
+            return self.get(_data) is None
+        else:
+            for o in output:
+                if self.get(o) is None:
+                    return True
         return False
     
     def save(self):
         """
         Saves the cell for persistency. For an in-memory cell, this is implemented by storing cell._address in the GRAPH
 
         :Returns:
```

### Comparing `pyg-base-0.0.8/src/pyg_base/_cfg.py` & `pyg-base-0.0.9/src/pyg_base/_cfg.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base/_dag.py` & `pyg-base-0.0.9/src/pyg_base/_dag.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base/_dates.py` & `pyg-base-0.0.9/src/pyg_base/_dates.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base/_decorators.py` & `pyg-base-0.0.9/src/pyg_base/_decorators.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base/_dict.py` & `pyg-base-0.0.9/src/pyg_base/_dict.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base/_dictable.py` & `pyg-base-0.0.9/src/pyg_base/_dictable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 from _collections_abc import dict_keys, dict_values
 from pyg_base._as_list import as_list, as_tuple
+from pyg_base._as_float import as_float
 from pyg_base._dict import Dict
 from pyg_base._zip import zipper, lens
 from pyg_base._types import is_str, is_strs, is_arr, is_df, is_dicts, is_int, is_ints, is_tuple, is_bools, is_nan
 from pyg_base._tree import is_tree, tree_to_table
 from pyg_base._inspect import getargs
-from pyg_base._decorators import kwargs_support, try_none
+from pyg_base._decorators import kwargs_support, try_none, try_back
+from pyg_base._dates import ndt
 from pyg_base._sort import sort, cmp
 from pyg_base._encode import _encode, _obj
 from pyg_base._file import read_csv
 from functools import reduce
 import pandas as pd
 import re
 
 __all__ = ['dict_concat', 'dictable', 'is_dictable']
 
 
+def nan2none(v):
+    return None if is_nan(v) or (is_str(v) and (len(v.strip()) == 0 or v[0] == '#' or v == 'n/a')) else v
+
+
 def dict_concat(*dicts):
     """
     A method of turning a list of dicts into one happy dict sharing its keys
 
     :Parameters:
     ----------------
     *dicts : list of dicts
@@ -89,23 +95,26 @@
         data = list(data)
     if data is None or (isinstance(data, list) and data == []):
         return {}
     elif isinstance(data, dict):
         return dict_concat(tree_to_table(data, columns)) if is_tree(columns) else dict(data)
     if columns is not None:
         if is_str(columns):
-            return {columns : data}
+            if (is_str(data) and '.xls' in data) or isinstance(data, pd.io.excel.ExcelFile):
+                return dict(dictable.read_excel(data, columns))
+            else:
+                return {columns : data}
         else:
             return dict(zipper(columns, zipper(*data)))
     else:
         if is_str(data):
             if data.endswith('.csv'):
                 data = read_csv(data)
             elif 'xls' in data:
-                data = pd.ExcelFile(data).parse()
+                data = dict(dictable.read_excel(data))
             else:
                 return dict(data = data)
         if is_df(data):
             if data.index.name is not None:
                 data = data.reset_index()
             return data.to_dict('list')
         tp = str(type(data)).lower()        
@@ -249,15 +258,15 @@
 
     Full details are below.
     """
     def __init__(self, data = None, columns = None, **kwargs):
         kwargs = {key :_value(value) for key, value in kwargs.items()}
         data_kwargs = {key: _value(value) for key, value in _data_columns_as_dict(data, columns).items()}
         kwargs.update(data_kwargs)
-        if is_strs(columns) and not is_tree(columns):
+        if is_strs(columns) and (len(data_kwargs) == 0 or not is_str(columns)):
             kwargs = {key : kwargs.get(key, [None]) for key in columns} if len(kwargs)>0 else {key : [] for key in columns}
         n = lens(*kwargs.values())
         kwargs = {str(key) if is_int(key) else key : value * n if len(value)==1 else value for key, value in kwargs.items()}
         super(dictable, self).__init__(kwargs)
         
     def __len__(self):
         return lens(*self.values())
@@ -690,14 +699,40 @@
         if len(by) == 0:
             return dictable({key: [value] for key, value in dict(self).items()})
         xs, ids = self._listby(by)
         rtn = dictable(xs, by)
         rtn.update({k: [[self[k][i] for i in y] for y in ids] for k in self.keys() if k not in by})
         return rtn
     
+    @classmethod
+    def read_excel(cls, io, sheet_name = None, floats = None, ints = None, dates = None, no_none = None):
+        if is_str(io):
+            io = io.lower()
+            if '!' in io and sheet_name is None: ## handling input like: ExcelFile.xlsx!SheetName
+                io, sheet_name = io.split('!')
+            if not '.xls' in io:
+                io = io + '.xlsx'
+            io = pd.ExcelFile(io)
+        if sheet_name is None:
+            sheet_name = 0
+        df = io.parse(sheet_name)
+        res = cls(df)
+        res = res.relabel(lambda v: v.strip().replace(' ', '_'))
+        res = res.do(nan2none)
+        if floats:
+            res = res.do(try_back(as_float), floats)
+        if ints:
+            res = res.do(try_back(int), ints)
+        if dates:
+            res = res.do(try_back(ndt), dates)
+        if no_none:
+            for col in as_list(no_none):
+                res = res.exc(**{col : None})
+        return res
+    
     def unlist(self):
         """
         undoes listby...
         
         :Example:
         -------
         >>> x = dictable(a = [1,2,3,4], b= [1,0,1,0])
```

### Comparing `pyg-base-0.0.8/src/pyg_base/_dictattr.py` & `pyg-base-0.0.9/src/pyg_base/_dictattr.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base/_drange.py` & `pyg-base-0.0.9/src/pyg_base/_drange.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base/_encode.py` & `pyg-base-0.0.9/src/pyg_base/_encode.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base/_eq.py` & `pyg-base-0.0.9/src/pyg_base/_eq.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base/_file.py` & `pyg-base-0.0.9/src/pyg_base/_file.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base/_getitem.py` & `pyg-base-0.0.9/src/pyg_base/_getitem.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base/_inspect.py` & `pyg-base-0.0.9/src/pyg_base/_inspect.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base/_logger.py` & `pyg-base-0.0.9/src/pyg_base/_logger.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base/_loop.py` & `pyg-base-0.0.9/src/pyg_base/_loop.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base/_named_dict.py` & `pyg-base-0.0.9/src/pyg_base/_named_dict.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base/_pandas.py` & `pyg-base-0.0.9/src/pyg_base/_pandas.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from pyg_base._loop import loop
 from pyg_base._dates import dt
 import pandas as pd
 import numpy as np
 from copy import copy
 import inspect
 import datetime
-from operator import add, mul
 
 
 __all__ = ['df_fillna', 'df_index', 'df_reindex', 'df_columns', 'presync', 'np_reindex', 'nona', 'df_slice', 'df_unslice', 'min_', 'max_', 'add_', 'mul_', 'sub_', 'div_', 'pow_']
 
 def _list(values):
     """
     >>> assert _list([1,2,[3,4,5,[6,7]],dict(a =[8,9], b=[10,[11,12]])])  == [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12]  
@@ -470,15 +469,15 @@
     >>> 5  2.0  NaN
     >>> 6  3.0  NaN    
 
     """
     if isinstance(objs, dict):
         columns = list(objs.keys())
         objs = list(objs.values())
-    if isinstance(objs, list):
+    if isinstance(objs, (list, tuple)):
         df_objs = [o for o in objs if is_pd(o)]
         res = pd.concat(df_objs, axis = axis, join = join)
         if len(df_objs) < len(objs):
             df_objs = [o if is_pd(o) else pd.Series(o, res.index) for o in objs]
             res = pd.concat(df_objs, axis = axis, join = join)            
     elif isinstance(objs, pd.DataFrame):
         res = objs.copy() if columns is not None else objs
@@ -1132,8 +1131,9 @@
 
     """
     n = df.shape[1] if is_df(df) else 1
     res = dictable(ub = ub, lb = [None] + ub[:-1], i = range(len(ub)))
     res = res(ts = lambda lb, ub: df_slice(df, lb, ub, '(]'))
     res = res(rs = lambda i, ts: dictable(u = ub[i: i+n], j = range(len(ub[i: i+n])))(ts = lambda j: ts[j]))
     rs = dictable.concat(res.rs).listby('u').do([pd.concat, nona], 'ts')
-    return dict(rs['u', 'ts'])
+    return dict(rs['u', 'ts'])
+
```

### Comparing `pyg-base-0.0.8/src/pyg_base/_parquet.py` & `pyg-base-0.0.9/src/pyg_base/_parquet.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base/_perdictable.py` & `pyg-base-0.0.9/src/pyg_base/_perdictable.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base/_reducer.py` & `pyg-base-0.0.9/src/pyg_base/_reducer.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base/_sort.py` & `pyg-base-0.0.9/src/pyg_base/_sort.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base/_tree.py` & `pyg-base-0.0.9/src/pyg_base/_tree.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base/_tree_repr.py` & `pyg-base-0.0.9/src/pyg_base/_tree_repr.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base/_txt.py` & `pyg-base-0.0.9/src/pyg_base/_txt.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base/_types.py` & `pyg-base-0.0.9/src/pyg_base/_types.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base/_ulist.py` & `pyg-base-0.0.9/src/pyg_base/_ulist.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base/_waiter.py` & `pyg-base-0.0.9/src/pyg_base/_waiter.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base/_zip.py` & `pyg-base-0.0.9/src/pyg_base/_zip.py`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base.egg-info/PKG-INFO` & `pyg-base-0.0.9/src/pyg_base.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyg-base
-Version: 0.0.8
+Version: 0.0.9
 Summary: Utilities for data manipulation including creation of DAGs and tables
 Home-page: https://github.com/gityoav/pyg-base
 Author: Yoav Git
 Author-email: yoav.git@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/gityoav/pyg-base/issues
 Platform: UNKNOWN
```

### Comparing `pyg-base-0.0.8/src/pyg_base.egg-info/PKG-INFO (DESKTOP-27SMATF's conflicted copy 2022-01-03)` & `pyg-base-0.0.9/src/pyg_base.egg-info/PKG-INFO (DESKTOP-27SMATF's conflicted copy 2022-01-03)`

 * *Files identical despite different names*

### Comparing `pyg-base-0.0.8/src/pyg_base.egg-info/SOURCES.txt` & `pyg-base-0.0.9/src/pyg_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

