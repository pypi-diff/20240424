# Comparing `tmp/gfagraphs-0.3.0.tar.gz` & `tmp/gfagraphs-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gfagraphs-0.3.0.tar", last modified: Fri Apr 19 08:42:21 2024, max compression
+gzip compressed data, was "gfagraphs-0.3.1.tar", last modified: Tue Apr 23 16:25:03 2024, max compression
```

## Comparing `gfagraphs-0.3.0.tar` & `gfagraphs-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-19 08:42:21.746106 gfagraphs-0.3.0/
--rw-r--r--   0 sidubois (669136) genscale (35005)    34521 2023-11-29 09:58:07.000000 gfagraphs-0.3.0/LICENSE
--rw-r--r--   0 sidubois (669136) genscale (35005)     2038 2024-04-19 08:42:21.746106 gfagraphs-0.3.0/PKG-INFO
--rw-r--r--   0 sidubois (669136) genscale (35005)     1415 2024-04-19 08:32:43.000000 gfagraphs-0.3.0/README.md
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-19 08:42:21.745107 gfagraphs-0.3.0/gfagraphs/
--rw-r--r--   0 sidubois (669136) genscale (35005)       58 2024-04-19 08:22:28.000000 gfagraphs-0.3.0/gfagraphs/__init__.py
--rw-r--r--   0 sidubois (669136) genscale (35005)    39616 2024-03-07 16:32:34.000000 gfagraphs-0.3.0/gfagraphs/gfagraphs.py
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-19 08:42:21.746106 gfagraphs-0.3.0/gfagraphs.egg-info/
--rw-r--r--   0 sidubois (669136) genscale (35005)     2038 2024-04-19 08:42:21.000000 gfagraphs-0.3.0/gfagraphs.egg-info/PKG-INFO
--rw-r--r--   0 sidubois (669136) genscale (35005)      357 2024-04-19 08:42:21.000000 gfagraphs-0.3.0/gfagraphs.egg-info/SOURCES.txt
--rw-r--r--   0 sidubois (669136) genscale (35005)        1 2024-04-19 08:42:21.000000 gfagraphs-0.3.0/gfagraphs.egg-info/dependency_links.txt
--rw-r--r--   0 sidubois (669136) genscale (35005)        1 2024-04-19 08:24:53.000000 gfagraphs-0.3.0/gfagraphs.egg-info/not-zip-safe
--rw-r--r--   0 sidubois (669136) genscale (35005)       19 2024-04-19 08:42:21.000000 gfagraphs-0.3.0/gfagraphs.egg-info/top_level.txt
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-19 08:42:21.746106 gfagraphs-0.3.0/pgGraphs/
--rw-r--r--   0 sidubois (669136) genscale (35005)      184 2024-01-25 14:21:38.000000 gfagraphs-0.3.0/pgGraphs/__init__.py
--rw-r--r--   0 sidubois (669136) genscale (35005)      548 2024-02-19 09:05:35.000000 gfagraphs-0.3.0/pgGraphs/abstractions.py
--rw-r--r--   0 sidubois (669136) genscale (35005)    15566 2024-04-16 12:23:19.000000 gfagraphs-0.3.0/pgGraphs/gfaparser.py
--rw-r--r--   0 sidubois (669136) genscale (35005)    29827 2024-04-18 09:35:46.000000 gfagraphs-0.3.0/pgGraphs/graph.py
--rw-r--r--   0 sidubois (669136) genscale (35005)     5261 2024-04-08 10:15:17.000000 gfagraphs-0.3.0/pgGraphs/networkx.py
--rw-r--r--   0 sidubois (669136) genscale (35005)      695 2024-04-19 08:42:21.000000 gfagraphs-0.3.0/pyproject.toml
--rw-r--r--   0 sidubois (669136) genscale (35005)       38 2024-04-19 08:42:21.746106 gfagraphs-0.3.0/setup.cfg
--rw-r--r--   0 sidubois (669136) genscale (35005)     2489 2024-04-19 08:32:52.000000 gfagraphs-0.3.0/setup.py
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-23 16:25:03.309799 gfagraphs-0.3.1/
+-rw-r--r--   0 sidubois (669136) genscale (35005)    34521 2023-11-29 09:58:07.000000 gfagraphs-0.3.1/LICENSE
+-rw-r--r--   0 sidubois (669136) genscale (35005)     2114 2024-04-23 16:25:03.308799 gfagraphs-0.3.1/PKG-INFO
+-rw-r--r--   0 sidubois (669136) genscale (35005)     1491 2024-04-19 14:44:53.000000 gfagraphs-0.3.1/README.md
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-23 16:25:03.308799 gfagraphs-0.3.1/gfagraphs/
+-rw-r--r--   0 sidubois (669136) genscale (35005)       58 2024-04-19 08:22:28.000000 gfagraphs-0.3.1/gfagraphs/__init__.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)    39616 2024-03-07 16:32:34.000000 gfagraphs-0.3.1/gfagraphs/gfagraphs.py
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-23 16:25:03.308799 gfagraphs-0.3.1/gfagraphs.egg-info/
+-rw-r--r--   0 sidubois (669136) genscale (35005)     2114 2024-04-23 16:25:03.000000 gfagraphs-0.3.1/gfagraphs.egg-info/PKG-INFO
+-rw-r--r--   0 sidubois (669136) genscale (35005)      357 2024-04-23 16:25:03.000000 gfagraphs-0.3.1/gfagraphs.egg-info/SOURCES.txt
+-rw-r--r--   0 sidubois (669136) genscale (35005)        1 2024-04-23 16:25:03.000000 gfagraphs-0.3.1/gfagraphs.egg-info/dependency_links.txt
+-rw-r--r--   0 sidubois (669136) genscale (35005)        1 2024-04-19 08:24:53.000000 gfagraphs-0.3.1/gfagraphs.egg-info/not-zip-safe
+-rw-r--r--   0 sidubois (669136) genscale (35005)       19 2024-04-23 16:25:03.000000 gfagraphs-0.3.1/gfagraphs.egg-info/top_level.txt
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-23 16:25:03.308799 gfagraphs-0.3.1/pgGraphs/
+-rw-r--r--   0 sidubois (669136) genscale (35005)      184 2024-01-25 14:21:38.000000 gfagraphs-0.3.1/pgGraphs/__init__.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)     2079 2024-04-23 15:21:03.000000 gfagraphs-0.3.1/pgGraphs/abstractions.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)    16717 2024-04-23 16:16:09.000000 gfagraphs-0.3.1/pgGraphs/gfaparser.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)    30506 2024-04-23 16:17:02.000000 gfagraphs-0.3.1/pgGraphs/graph.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)     6217 2024-04-19 09:42:36.000000 gfagraphs-0.3.1/pgGraphs/networkx.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)      695 2024-04-23 16:25:03.000000 gfagraphs-0.3.1/pyproject.toml
+-rw-r--r--   0 sidubois (669136) genscale (35005)       38 2024-04-23 16:25:03.309799 gfagraphs-0.3.1/setup.cfg
+-rw-r--r--   0 sidubois (669136) genscale (35005)     2482 2024-04-23 16:06:05.000000 gfagraphs-0.3.1/setup.py
```

### Comparing `gfagraphs-0.3.0/LICENSE` & `gfagraphs-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.0/PKG-INFO` & `gfagraphs-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gfagraphs
-Version: 0.3.0
+Version: 0.3.1
 Summary: Library to parse, edit and handle in memory GFA graphs
 Home-page: https://github.com/Tharos-ux/gfagraphs
 Author: ('Siegfried Dubois',)
 Author-email: Siegfried Dubois <siegfried.dubois@inria.fr>
 Project-URL: Homepage, https://github.com/Tharos-ux/gfagraphs
 Project-URL: Bug Tracker, https://github.com/Tharos-ux/gfagraphs/issues
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![](https://img.shields.io/badge/Python-3.10-blue.svg)]()
 [![](https://img.shields.io/badge/Python-3.11-blue.svg)]()
 [![](https://img.shields.io/badge/Python-3.12-blue.svg)]()
-[![](https://img.shields.io/badge/documentation-unfinished-orange.svg)]()
+[![Documentation Status](https://readthedocs.org/projects/gfagraphs/badge/?version=latest)](https://gfagraphs.readthedocs.io/en/latest/?badge=latest)
 
 # GFAGraphs - A Python GFA library
 
 > [!WARNING]\
 > A paper is in preparation about this work. If you consider to use this tool, please contact the author for attribution.
 
 This Python library aims to be an abstraction layer for GFA file format.
```

### Comparing `gfagraphs-0.3.0/README.md` & `gfagraphs-0.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [![](https://img.shields.io/badge/Python-3.10-blue.svg)]()
 [![](https://img.shields.io/badge/Python-3.11-blue.svg)]()
 [![](https://img.shields.io/badge/Python-3.12-blue.svg)]()
-[![](https://img.shields.io/badge/documentation-unfinished-orange.svg)]()
+[![Documentation Status](https://readthedocs.org/projects/gfagraphs/badge/?version=latest)](https://gfagraphs.readthedocs.io/en/latest/?badge=latest)
 
 # GFAGraphs - A Python GFA library
 
 > [!WARNING]\
 > A paper is in preparation about this work. If you consider to use this tool, please contact the author for attribution.
 
 This Python library aims to be an abstraction layer for GFA file format.
```

### Comparing `gfagraphs-0.3.0/gfagraphs/gfagraphs.py` & `gfagraphs-0.3.1/gfagraphs/gfagraphs.py`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.0/gfagraphs.egg-info/PKG-INFO` & `gfagraphs-0.3.1/gfagraphs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gfagraphs
-Version: 0.3.0
+Version: 0.3.1
 Summary: Library to parse, edit and handle in memory GFA graphs
 Home-page: https://github.com/Tharos-ux/gfagraphs
 Author: ('Siegfried Dubois',)
 Author-email: Siegfried Dubois <siegfried.dubois@inria.fr>
 Project-URL: Homepage, https://github.com/Tharos-ux/gfagraphs
 Project-URL: Bug Tracker, https://github.com/Tharos-ux/gfagraphs/issues
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![](https://img.shields.io/badge/Python-3.10-blue.svg)]()
 [![](https://img.shields.io/badge/Python-3.11-blue.svg)]()
 [![](https://img.shields.io/badge/Python-3.12-blue.svg)]()
-[![](https://img.shields.io/badge/documentation-unfinished-orange.svg)]()
+[![Documentation Status](https://readthedocs.org/projects/gfagraphs/badge/?version=latest)](https://gfagraphs.readthedocs.io/en/latest/?badge=latest)
 
 # GFAGraphs - A Python GFA library
 
 > [!WARNING]\
 > A paper is in preparation about this work. If you consider to use this tool, please contact the author for attribution.
 
 This Python library aims to be an abstraction layer for GFA file format.
```

### Comparing `gfagraphs-0.3.0/pgGraphs/gfaparser.py` & `gfagraphs-0.3.1/pgGraphs/gfaparser.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,62 @@
-"Abstract class for parsing and saving GFA file format"
 from re import match
 from typing import Callable
 from json import loads, dumps
 from os import path, stat
 from tharospytools.path_tools import path_allocator
-from pgGraphs.abstractions import Orientation, GFALine, GFAFormat
+from pgGraphs.abstractions import Orientation, GFALine, GFAFormat, EdgeOrientation
 from gzip import open as gz_open
 from re import search
 
 
 class GFAParser:
     """This class implements static methods to get informations about the contents of a GFA file, and to parse them.
 
-    Raises:
-        OSError: _description_
-        IOError: _description_
-        IOError: _description_
-        NotImplementedError: _description_
-        ValueError: _description_
-        ValueError: _description_
-
+    Returns
+    -------
+    None
+        Methods are static and should be used passing arguments.
+
+    Raises
+    ------
+    OSError
+        The file does not exists
+    IOError
+        File is empty
+    IOError
+        File descriptor is invalid
+    NotImplementedError
+        Byte-array or array is saved to GFA
+    ValueError
+        Data format not in GFA standards
     """
 
     @staticmethod
     def get_gfa_format(gfa_file_path: str | list[str]) -> str | list[str]:
-        """Given a file, or more, returns the gfa subtypes, and raises error if file is invalid or does not exists
-
-        Args:
-            gfa_file_path (str | list[str]): one or more file paths
+        """Given a file, or more, returns the gfa subtypes, and raises error if file is invalid or does not exists.
+        Objective is to asses GFA subformat on files for pre-processing purposes, or algorithm choices.
 
-        Returns:
-            str | list[str]: a gfa subtype descriptor per input file
-
-        Raises:
-            OSError: The file does not exists
-            IOError: The file descriptor is invalid
-            IOError: The file is empty
+        Parameters
+        ----------
+        gfa_file_path : str | list[str]
+            a series of paths, or a single one
+
+        Returns
+        -------
+        str | list[str]
+            per path, a tag identifying the gfa type
+
+        Raises
+        ------
+        OSError
+            Specified file does not exists
+        IOError
+            File descriptor is invalid
+        IOError
+            File is empty
         """
         styles: list[str] = list()
         if isinstance(gfa_file_path, str):
             gfa_file_path = [gfa_file_path]
         for gfa_file in gfa_file_path:
             # Checking if path exists
             if not path.exists(gfa_file):
@@ -80,25 +97,34 @@
                         styles.append('rGFA')
         if len(styles) == 1:
             return styles[0]
         return styles
 
     @staticmethod
     def get_gfa_type(tag_type: str) -> type | Callable:
-        """Interprets tags of GFA as a Python-compatible format
-
-        Args:
-            tag_type (str): the letter that identifies the GFA data type
-
-        Raises:
-            NotImplementedError: happens if its an array or byte array (needs doc)
-            ValueError: happens if format is not in GFA standards
-
-        Returns:
-            type | Callable: the cast method or type to apply
+        """Interprets tags of GFA as a Python-compatible format.
+        Given a letter used as a tag in the GFA standard, return the type or function to cast the data to.
+        This function is used in input scenarios, to read a file from disk and interpret its content
+
+        Parameters
+        ----------
+        tag_type : str
+            a GFA tag
+
+        Returns
+        -------
+        type | Callable
+            a cast descriptor to use on the data
+
+        Raises
+        ------
+        NotImplementedError
+            Byte-array or array
+        ValueError
+            Type identifer is not in the GFA-spec
         """
         if tag_type == 'i':
             return int
         elif tag_type == 'f':
             return float
         elif tag_type == 'A' or tag_type == 'Z':
             return str
@@ -107,44 +133,52 @@
         elif tag_type == 'H' or tag_type == 'B':
             raise NotImplementedError()
         raise ValueError(
             f"Type identifier {tag_type} is not in the GFA standard")
 
     @staticmethod
     def set_gfa_type(tag_type: str) -> type | Callable:
-        """Interprets tags of GFA as a Python-compatible format
-
-        Args:
-            tag_type (str): the letter that identifies the GFA data type
-
-        Raises:
-            NotImplementedError: happens if its an array or byte array (needs doc)
-            ValueError: happens if format is not in GFA standards
-
-        Returns:
-            type | Callable: the cast method or type to apply
+        """Interprets tags of GFA as a Python-compatible format.
+        Given a letter used as a tag in the GFA standard, return the type or function to cast the data to.
+        This function is used in output scenarios, to write a file to disk.
+
+        Parameters
+        ----------
+        tag_type : str
+            a GFA tag
+
+        Returns
+        -------
+        type | Callable
+            a cast descriptor to use on the data
         """
         if tag_type == 'J':
             return dumps
         else:
             return str
 
     @staticmethod
     def get_python_type(data: object) -> str:
-        """Interprets tags of GFA as a Python-compatible format
-
-        Args:
-            tag_type (str): the letter that identifies the GFA data type
+        """From a python variable, tries to identify the best suiting tag, and validates it.
+        See http://gfa-spec.github.io/GFA-spec/GFA1.html#optional-fields for more details.
 
-        Raises:
-            NotImplementedError: happens if its an array or byte array (needs doc)
-            ValueError: happens if format is not in GFA standards
-
-        Returns:
-            type | Callable: the cast method or type to apply
+        Parameters
+        ----------
+        data : object
+            the data we try to add to the GFA file
+
+        Returns
+        -------
+        str
+            a one-letter code for an optional filed of the GFA-spec
+
+        Raises
+        ------
+        ValueError
+            data type could not be encoded in the GFA-spec
         """
         if isinstance(data, int):
             return 'i'
         elif isinstance(data, float):
             return 'f'
         elif isinstance(data, str):
             return 'Z'
@@ -154,22 +188,27 @@
                 return 'J'
             except (TypeError, OverflowError) as exc:
                 raise ValueError(
                     f"Data {data} of type {type(data)} is not in the GFA standard") from exc
 
     @staticmethod
     def supplementary_datas(datas: list, length_condition: int) -> dict:
-        """Computes the optional tags of a gfa line and returns them as a dict
-
-        Args:
-            datas (list): parsed data line
-            length_condition (int): last position of positional field
+        """Computes the optional tags of a gfa line and returns them as a dict.
 
-        Returns:
-            dict: mapping tag:value
+        Parameters
+        ----------
+        datas : list
+            a list of tags and their values
+        length_condition : int
+            the tags that are mandatory (and already processed)
+
+        Returns
+        -------
+        dict
+            interpreted tags in their right types
         """
         mapping: dict = dict()
         nargs: int = length_condition
         if len(datas) > length_condition:  # we happen to have additional tags to our line
             for additional_tag in datas[length_condition:]:
                 if match('[A-Z]{2}:[a-zA-Z]{1}:', additional_tag):  # matches start of the line
                     mapping[additional_tag[:2]] = GFAParser.get_gfa_type(
@@ -177,24 +216,32 @@
                 else:
                     mapping[f"ARG{nargs}"] = additional_tag
                     nargs += 1
         return mapping
 
     @staticmethod
     def read_gfa_line(datas: list[str], load_sequence_in_memory: bool = True, regexp_pattern: str = ".*", memory_mode: bool = True) -> tuple[str, GFALine, dict]:
-        """Calls methods to parse a GFA line,
-        accordingly to it's fields described in the GFAspec github.
+        """Calls methods to parse a GFA line, accordingly to it's fields described in the GFAspec github.
+        Parses a single line and return the information it contains
 
-        Args:
-            datas (list): a list of the fileds in the line
-            load_sequence_in_memory (bool): if the line is a segment, ask to load its sequence
-            memory_mode (bool): if the strict minimum in information should be inserted
-
-        Returns:
-            tuple[str, GFALine, dict]: datas of the line in Python-compatible formats.
+        Parameters
+        ----------
+        datas : list[str]
+            the list of tab-separated elements of the GFA line.
+        load_sequence_in_memory : bool, optional
+            if it is a node, if the sequance should be or not loaded, by default True
+        regexp_pattern : str, optional
+            a pattern to keep for path names, by default ".*"
+        memory_mode : bool, optional
+            if additional information should be loaded in the struct, by default True
+
+        Returns
+        -------
+        tuple[str, GFALine, dict]
+            Conatins `id_of_line`, `type_of_line`, `datas_of_line`
         """
         line_datas: dict = dict()
         if not (datas[0].isupper() or len(datas) == 0):
             return (None, None, None)
 
         match (line_type := GFALine(datas[0])):
             case GFALine.SEGMENT:
@@ -202,19 +249,21 @@
                 if load_sequence_in_memory:
                     line_datas["seq"] = datas[2]
                 if memory_mode:
                     return (datas[1], line_type, {**line_datas, **GFAParser.supplementary_datas(datas, 3)})
                 else:
                     return (datas[1], line_type, line_datas)
             case GFALine.LINE:
-                if memory_mode:
-                    line_datas["start"] = datas[1]
-                    line_datas["end"] = datas[3]
-                    line_datas["orientation"] = f"{datas[2]}/{datas[4]}"
-                    return ((line_datas['start'], line_datas['end']), line_type, {**line_datas, **GFAParser.supplementary_datas(datas, 5)})
+                if not memory_mode:
+                    line_datas["orientation"] = {
+                        EdgeOrientation(
+                            f"{datas[2]}/{datas[4]}"
+                        )
+                    }
+                    return ((datas[1], datas[3]), line_type, {**line_datas, **GFAParser.supplementary_datas(datas, 5)})
                 else:
                     return (None, None, None)
             case GFALine.WALK:
                 line_datas["name"] = datas[1]
                 line_datas["id"] = datas[3]
                 line_datas["origin"] = datas[2]
                 line_datas["start_offset"] = datas[4]
@@ -254,19 +303,25 @@
             case GFALine.HEADER | GFALine.ANY:
                 return (None, line_type, GFAParser.supplementary_datas(datas, 1))
 
     @staticmethod
     def save_graph(graph, output_path: str, force_format: GFAFormat | bool = False, minimal_graph: bool = False) -> None:
         """Given a gfa Graph object, saves to a valid gfa file the Graph.
 
-        Args:
-            output_path (str): a path on disk where to save
-            force_format (GfaFormat|bool): a format to choose for output.
-                if False, default graph format will be used.
-            minimal_graph (bool) if only necessary info should be kept in output gfa
+        Parameters
+        ----------
+        graph : Graph
+            the graph object loaded in memory
+        output_path : str
+            a path to an existing (or not) dile on the disk
+        force_format : GFAFormat | bool, optional
+            the output gfa subformat, by default False
+        minimal_graph : bool, optional
+            if only mandatory tags should be kept, by default False
+
         """
         # Haplotype number serves when we convert GFA1 to GFA1.1 for W-lines
         haplotype_number: int = 0
         gfa_format: GFAFormat = graph.metadata['version'] if not force_format else force_format
 
         with open(path_allocator(output_path), 'w', encoding='utf-8') as gfa_writer:
             if graph.headers and gfa_format != GFAFormat.RGFA:
@@ -292,24 +347,22 @@
                 # Whichever the format, those should be written
                 for segment_name, segment_datas in graph.segments.items():
                     supplementary_text: str = '' if minimal_graph else "\t" + '\t'.join(
                         [f"{key}:{GFAParser.get_python_type(value)}:{GFAParser.set_gfa_type(GFAParser.get_python_type(value))(value)}" if not key.startswith('ARG') else str(value) for key, value in segment_datas.items() if key not in ['length', 'seq']])
                     gfa_writer.write(
                         "S\t"+f"{segment_name}\t{segment_datas['seq'] if 'seq' in segment_datas else 'N'*segment_datas['length']}{supplementary_text}\n")
             if graph.lines:
-                for line in graph.lines.values():
+                for (source, sink), line in graph.lines.items():
                     supplementary_text: str = '' if minimal_graph else "\t" + '\t'.join(
                         [f"{key}:{GFAParser.get_python_type(value)}:{GFAParser.set_gfa_type(GFAParser.get_python_type(value))(value)}" if not key.startswith('ARG') else str(value) for key, value in line.items() if key not in ['orientation', 'start', 'end']])
                     # We accomodate for all alternatives orientation versions that are described in the input graph file to be written back
-                    all_alternates = line.pop(
-                        'alternates', []) + [line['orientation']]
-                    for alt in all_alternates:
-                        ori1, ori2 = alt.split('/')
+                    for alt in line['orientation']:
+                        ori1, ori2 = alt.value.split('/')
                         gfa_writer.write(
-                            f"L\t"+f"{line['start']}\t{ori1}\t{line['end']}\t{ori2}\t0M{supplementary_text}\n")
+                            f"L\t"+f"{source}\t{ori1}\t{sink}\t{ori2}\t0M{supplementary_text}\n")
             if graph.paths:
                 for path_name, path_datas in graph.paths.items():
                     supplementary_text: str = '' if minimal_graph else "\t" + '\t'.join(
                         [f"{key}:{GFAParser.get_python_type(value)}:{GFAParser.set_gfa_type(GFAParser.get_python_type(value))(value)}" if not key.startswith('ARG') else str(value) for key, value in path_datas.items() if key not in ['path', 'start_offset', 'stop_offset', 'origin', 'name', 'id']])
                     if gfa_format == GFAFormat.GFA1:  # P-line
                         strpath: str = ','.join(
                             [node_name+'+' if orient == Orientation.FORWARD else node_name+'-' for node_name, orient in path_datas['path']])
```

### Comparing `gfagraphs-0.3.0/pgGraphs/graph.py` & `gfagraphs-0.3.1/pgGraphs/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 "Modelizes a graph object"
 from itertools import count
-from pgGraphs.abstractions import GFALine, Orientation
+from pgGraphs.abstractions import GFALine, Orientation, EdgeOrientation, reverse
 from pgGraphs.gfaparser import GFAParser
 from gzip import open as gz_open
 from tharospytools.multithreading import futures_collector
 from tharospytools.bio_tools import revcomp
 from typing import Any, Generator
 
 
@@ -25,26 +25,29 @@
     ]
 
     def __init__(
         self,
         gfa_file: str | None = None,
         with_sequence: bool = True,
         low_memory: bool = False,
+        with_reverse_edges: bool = False,
         regexp: str = ".*",
     ) -> None:
         """Constructor for GFA Graph object.
 
         Parameters
         ----------
         gfa_file : str | None, optional
             A file path to a valid GFA file, by default None
         with_sequence : bool, optional
             If sequence should be included in nodes. Consumes more memory with huge graphs, by default True
         low_memory : bool, optional
             If the minimal number of information should be loaded or not. If yes, will only load length of the nodes and the paths but not the edges, by default False
+        with_reverse_edges : bool, optional
+            If loading the graph should include computation of each reverse edge
         regexp : str, optional
             Regular expression to keep from the paths names (used to standardize/reduce them), by default ".*"
         """
         # Declaring format attributes, generators...
         self.metadata: dict = {
             'version': GFAParser.get_gfa_format(gfa_file_path=gfa_file) if gfa_file and not low_memory else 'unknown',
             'next_node_name': (x for x in count(start=1) if str(x) not in self.segments) if not low_memory else 'unknown',
@@ -71,16 +74,23 @@
                             self.segments[name] = datas
                         case GFALine.WALK | GFALine.PATH:
                             self.paths[name] = datas
                         case GFALine.LINE:
                             if name not in self.lines:
                                 self.lines[name] = datas
                             else:
-                                self.lines[name]['alternates'] = self.lines[name].get(
-                                    'alternates', []) + [datas['orientation']]
+                                self.lines[name]['orientation'] = self.lines[name].get(
+                                    'orientation', set()).add(datas['orientation'])
+                            if with_reverse_edges:
+                                if name[::-1] not in self.lines:
+                                    self.lines[name[::-1]] = datas
+                                else:
+                                    self.lines[name[::-1]]['orientation'] = self.lines[name[::-1]].get(
+                                        'orientation', set()).add(reverse(datas['orientation']))
+
                         case GFALine.HEADER:
                             self.headers.append(datas)
                         case _:
                             pass
 
     def __str__(self) -> str:
         """Returns a textual description of the object.
@@ -284,20 +294,20 @@
                 ori_source = ori_source.value
             except:
                 raise ValueError("Not compatible with GFA format.")
         if (source, sink) not in self.lines:
             self.lines[(source, sink)] = {
                 'start': source,
                 'end': sink,
-                'orientation': f"{ori_source}/{ori_sink}",
+                'orientation': set(EdgeOrientation(f"{ori_source}/{ori_sink}")),
                 **metadata
             }
         else:
-            self.lines[(source, sink)]['alternates'] = self.lines[(source, sink)].get(
-                'alternates', []) + [f"{ori_source}/{ori_sink}"]
+            self.lines[(source, sink)]['orientation'] = self.lines[(source, sink)].get(
+                'orientation', set()).add(EdgeOrientation(f"{ori_source}/{ori_sink}"))
 
     def add_path(
         self,
         name: str,
         chain: list[tuple[str, Orientation]],
         start: int = 0,
         end: int | None = None,
@@ -430,19 +440,19 @@
             node_to_split['length']
 
         # Get incomming and exuting edges
         edges_of_node: list[tuple[tuple[str, str], dict]
                             ] = self.get_edges(segment_name)
         for (_, edge) in edges_of_node:
             if edge['start'] == segment_name:
-                orient: str = edge.datas['orientation'].split('/')[0]
+                orient: str = edge.datas['orientation'].value.split('/')[0]
                 # Edge is output, should be changed
                 edge['start'] = future_segment_name[-1]
             else:
-                orient: str = edge['orientation'].split('/')[-1]
+                orient: str = edge['orientation'].value.split('/')[-1]
                 # Edge is incomming edge, should be kept
 
         # Edit first node
         node_to_split['seq'] = node_to_split['seq'][:position_to_split[0][1]
                                                     ] if 'seq' in node_to_split else 'N'*position_to_split[0][1]
 
         for i, positions in enumerate(position_to_split):
```

### Comparing `gfagraphs-0.3.0/pgGraphs/networkx.py` & `gfagraphs-0.3.1/pgGraphs/networkx.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,38 @@
-"Abstract class for visualization and modelization of GFA in a NetworkX object"
 from networkx import MultiDiGraph, DiGraph
 from pgGraphs.graph import Graph
 from tharospytools.matplotlib_tools import get_palette
 
 
 class GFANetwork:
+    """Abstract class for visualization and modelization of GFA in a NetworkX object
+
+    Returns
+    -------
+    None
+        Methods are static and should be used passing arguments.
+    """
 
     @staticmethod
     def compute_backbone(
         graph: Graph
     ) -> DiGraph:
-        """Computes a networkx representation of the graph, for computing purposes
-
-        Returns:
-            DiGraph: a networkx graph featuring the backbone of the pangenome graph
+        """Computes a networkx representation of the graph, for computing purposes.
+        This backbone contains the exact information of paths, nodes, edges... that is described in the loaded structure.
+        Allows to use every method of networkx library on the graph to perform traversal, neighborhood...
+
+        Parameters
+        ----------
+        graph : Graph
+            a gfa graph loaded in memory using this library
+
+        Returns
+        -------
+        DiGraph
+            a networkx object, in the form of a directed graph.
         """
         backbone: DiGraph = DiGraph()
 
         for node_name, node_datas in graph.segments.items():
             backbone.add_node(
                 node_name,
                 offsets=node_datas['PO'] if 'PO' in node_datas else None,
@@ -41,19 +56,29 @@
                 501, 1000], [1001, 10000], [10001, float('inf')]
         ),
         start_stop_ref: tuple | bool = False,
     ) -> MultiDiGraph:
         """Computes the networkx representation of the GFA.
         This function is intended to be used for graphical representation purposes, and not for computing metrics on the graph.
 
-        Args:
-            node_prefix (str): a prefix used when displaying multiple graphs to prevent node name collisions
-
-        Returns:
-            MultiDiGraph: a networkx graph featuring the maximum of information
+        Parameters
+        ----------
+        graph : Graph
+            a gfa graph loaded in memory using this library
+        node_prefix : str | None, optional
+            a name to put before every node, by default None
+        node_size_classes : tuple[list], optional
+            classes of size for coloring nodes, by default ( [0, 1], [2, 10], [11, 50], [51, 200], [201, 500], [ 501, 1000], [1001, 10000], [10001, float('inf')] )
+        start_stop_ref : tuple | bool, optional
+            defines starting and ending offset on the reference, by default False
+
+        Returns
+        -------
+        MultiDiGraph
+            a networkx object, in the form of a bidirected graph.
         """
         if start_stop_ref:
             graph.sequence_offsets(recalculate=True)
             start, stop, ref = start_stop_ref
         # Define empty graph
         nx_graph: MultiDiGraph = MultiDiGraph()
         # Creating the palette for node class colors
@@ -119,12 +144,14 @@
                 )
         return nx_graph
 
     def get_most_external_nodes(self) -> list[str]:
         """Get nodes that are on the edges of the graph (starting and ending nodes)
         Those are characterized by their in/out degree : one of those has to be 0.
 
-        Returns:
-            list[str]: nodes names matching the condition.
+        Returns
+        -------
+        list[str]
+            nodes matching the criterion.
         """
         bone: DiGraph = self.compute_backbone()
         return [x for x in bone.nodes() if bone.out_degree(x) == 0 or bone.in_degree(x) == 0]
```

### Comparing `gfagraphs-0.3.0/pyproject.toml` & `gfagraphs-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
     requires = ["setuptools>=61.0"]
     build-backend = "setuptools.build_meta"
 
     [project]
     name = "gfagraphs"
-    version = "0.3.0"
+    version = "0.3.1"
     authors = [
     { name="Siegfried Dubois", email="siegfried.dubois@inria.fr" },
     ]
     description = "Library to parse, edit and handle in memory GFA graphs"
     readme = "README.md"
     requires-python = ">=3.10"
     classifiers = [
```

### Comparing `gfagraphs-0.3.0/setup.py` & `gfagraphs-0.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,22 +9,21 @@
 NAME: str = "gfagraphs"
 AUTHOR: str = "Siegfried Dubois",
 AUTHOR_EMAIL: str = "siegfried.dubois@inria.fr",
 LICENCE: str = "LICENCE"
 DESCRIPTION: str = "Library to parse, edit and handle in memory GFA graphs"
 REQUIRED_PYTHON: tuple = (3, 10)
 OVERRIDE_VN: bool = True
-VN: str = "0.3.0"
+VN: str = "0.3.1"
 URL: str = "https://github.com/Tharos-ux/gfagraphs"
 REQUIREMENTS: list[str] = [
     'networkx',
     'tharos-pytools',
     'matplotlib',
     'mycolorpy',
-    ''
 ]
 
 
 if argv[1] in ('install', 'sdist', 'bdist_wheel'):
     # Checking if Python version is correct
     if version_info[:2] < REQUIRED_PYTHON:
         stderr.write(
```

