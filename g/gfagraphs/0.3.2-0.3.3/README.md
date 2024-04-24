# Comparing `tmp/gfagraphs-0.3.2.tar.gz` & `tmp/gfagraphs-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gfagraphs-0.3.2.tar", last modified: Wed Apr 24 08:12:17 2024, max compression
+gzip compressed data, was "gfagraphs-0.3.3.tar", last modified: Wed Apr 24 13:48:03 2024, max compression
```

## Comparing `gfagraphs-0.3.2.tar` & `gfagraphs-0.3.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-24 08:12:17.086707 gfagraphs-0.3.2/
--rw-r--r--   0 sidubois (669136) genscale (35005)    34521 2023-11-29 09:58:07.000000 gfagraphs-0.3.2/LICENSE
--rw-r--r--   0 sidubois (669136) genscale (35005)     2114 2024-04-24 08:12:17.085707 gfagraphs-0.3.2/PKG-INFO
--rw-r--r--   0 sidubois (669136) genscale (35005)     1491 2024-04-19 14:44:53.000000 gfagraphs-0.3.2/README.md
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-24 08:12:17.085707 gfagraphs-0.3.2/gfagraphs/
--rw-r--r--   0 sidubois (669136) genscale (35005)       58 2024-04-19 08:22:28.000000 gfagraphs-0.3.2/gfagraphs/__init__.py
--rw-r--r--   0 sidubois (669136) genscale (35005)    39616 2024-03-07 16:32:34.000000 gfagraphs-0.3.2/gfagraphs/gfagraphs.py
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-24 08:12:17.085707 gfagraphs-0.3.2/gfagraphs.egg-info/
--rw-r--r--   0 sidubois (669136) genscale (35005)     2114 2024-04-24 08:12:17.000000 gfagraphs-0.3.2/gfagraphs.egg-info/PKG-INFO
--rw-r--r--   0 sidubois (669136) genscale (35005)      351 2024-04-24 08:12:17.000000 gfagraphs-0.3.2/gfagraphs.egg-info/SOURCES.txt
--rw-r--r--   0 sidubois (669136) genscale (35005)        1 2024-04-24 08:12:17.000000 gfagraphs-0.3.2/gfagraphs.egg-info/dependency_links.txt
--rw-r--r--   0 sidubois (669136) genscale (35005)        1 2024-04-19 08:24:53.000000 gfagraphs-0.3.2/gfagraphs.egg-info/not-zip-safe
--rw-r--r--   0 sidubois (669136) genscale (35005)       19 2024-04-24 08:12:17.000000 gfagraphs-0.3.2/gfagraphs.egg-info/top_level.txt
-drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-24 08:12:17.085707 gfagraphs-0.3.2/pgGraphs/
--rw-r--r--   0 sidubois (669136) genscale (35005)      178 2024-04-23 16:35:16.000000 gfagraphs-0.3.2/pgGraphs/__init__.py
--rw-r--r--   0 sidubois (669136) genscale (35005)     2079 2024-04-23 15:21:03.000000 gfagraphs-0.3.2/pgGraphs/abstractions.py
--rw-r--r--   0 sidubois (669136) genscale (35005)    16717 2024-04-23 16:16:09.000000 gfagraphs-0.3.2/pgGraphs/gfaparser.py
--rw-r--r--   0 sidubois (669136) genscale (35005)    30506 2024-04-23 16:17:02.000000 gfagraphs-0.3.2/pgGraphs/graph.py
--rw-r--r--   0 sidubois (669136) genscale (35005)     6217 2024-04-19 09:42:36.000000 gfagraphs-0.3.2/pgGraphs/nx.py
--rw-r--r--   0 sidubois (669136) genscale (35005)      695 2024-04-24 08:12:17.000000 gfagraphs-0.3.2/pyproject.toml
--rw-r--r--   0 sidubois (669136) genscale (35005)       38 2024-04-24 08:12:17.086707 gfagraphs-0.3.2/setup.cfg
--rw-r--r--   0 sidubois (669136) genscale (35005)     2482 2024-04-24 08:12:00.000000 gfagraphs-0.3.2/setup.py
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-24 13:48:03.187340 gfagraphs-0.3.3/
+-rw-r--r--   0 sidubois (669136) genscale (35005)    34521 2023-11-29 09:58:07.000000 gfagraphs-0.3.3/LICENSE
+-rw-r--r--   0 sidubois (669136) genscale (35005)     2114 2024-04-24 13:48:03.186340 gfagraphs-0.3.3/PKG-INFO
+-rw-r--r--   0 sidubois (669136) genscale (35005)     1491 2024-04-19 14:44:53.000000 gfagraphs-0.3.3/README.md
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-24 13:48:03.186340 gfagraphs-0.3.3/gfagraphs/
+-rw-r--r--   0 sidubois (669136) genscale (35005)       58 2024-04-19 08:22:28.000000 gfagraphs-0.3.3/gfagraphs/__init__.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)    39616 2024-03-07 16:32:34.000000 gfagraphs-0.3.3/gfagraphs/gfagraphs.py
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-24 13:48:03.186340 gfagraphs-0.3.3/gfagraphs.egg-info/
+-rw-r--r--   0 sidubois (669136) genscale (35005)     2114 2024-04-24 13:48:03.000000 gfagraphs-0.3.3/gfagraphs.egg-info/PKG-INFO
+-rw-r--r--   0 sidubois (669136) genscale (35005)      351 2024-04-24 13:48:03.000000 gfagraphs-0.3.3/gfagraphs.egg-info/SOURCES.txt
+-rw-r--r--   0 sidubois (669136) genscale (35005)        1 2024-04-24 13:48:03.000000 gfagraphs-0.3.3/gfagraphs.egg-info/dependency_links.txt
+-rw-r--r--   0 sidubois (669136) genscale (35005)        1 2024-04-19 08:24:53.000000 gfagraphs-0.3.3/gfagraphs.egg-info/not-zip-safe
+-rw-r--r--   0 sidubois (669136) genscale (35005)       19 2024-04-24 13:48:03.000000 gfagraphs-0.3.3/gfagraphs.egg-info/top_level.txt
+drwxr-xr-x   0 sidubois (669136) genscale (35005)        0 2024-04-24 13:48:03.186340 gfagraphs-0.3.3/pgGraphs/
+-rw-r--r--   0 sidubois (669136) genscale (35005)      178 2024-04-23 16:35:16.000000 gfagraphs-0.3.3/pgGraphs/__init__.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)     1848 2024-04-24 12:08:52.000000 gfagraphs-0.3.3/pgGraphs/abstractions.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)    16812 2024-04-24 12:47:37.000000 gfagraphs-0.3.3/pgGraphs/gfaparser.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)    31188 2024-04-24 13:23:42.000000 gfagraphs-0.3.3/pgGraphs/graph.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)     6217 2024-04-19 09:42:36.000000 gfagraphs-0.3.3/pgGraphs/nx.py
+-rw-r--r--   0 sidubois (669136) genscale (35005)      695 2024-04-24 13:48:03.000000 gfagraphs-0.3.3/pyproject.toml
+-rw-r--r--   0 sidubois (669136) genscale (35005)       38 2024-04-24 13:48:03.187340 gfagraphs-0.3.3/setup.cfg
+-rw-r--r--   0 sidubois (669136) genscale (35005)     2449 2024-04-24 13:47:52.000000 gfagraphs-0.3.3/setup.py
```

### Comparing `gfagraphs-0.3.2/LICENSE` & `gfagraphs-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.2/PKG-INFO` & `gfagraphs-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gfagraphs
-Version: 0.3.2
+Version: 0.3.3
 Summary: Library to parse, edit and handle in memory GFA graphs
 Home-page: https://github.com/Tharos-ux/gfagraphs
 Author: ('Siegfried Dubois',)
 Author-email: Siegfried Dubois <siegfried.dubois@inria.fr>
 Project-URL: Homepage, https://github.com/Tharos-ux/gfagraphs
 Project-URL: Bug Tracker, https://github.com/Tharos-ux/gfagraphs/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gfagraphs-0.3.2/README.md` & `gfagraphs-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.2/gfagraphs/gfagraphs.py` & `gfagraphs-0.3.3/gfagraphs/gfagraphs.py`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.2/gfagraphs.egg-info/PKG-INFO` & `gfagraphs-0.3.3/gfagraphs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gfagraphs
-Version: 0.3.2
+Version: 0.3.3
 Summary: Library to parse, edit and handle in memory GFA graphs
 Home-page: https://github.com/Tharos-ux/gfagraphs
 Author: ('Siegfried Dubois',)
 Author-email: Siegfried Dubois <siegfried.dubois@inria.fr>
 Project-URL: Homepage, https://github.com/Tharos-ux/gfagraphs
 Project-URL: Bug Tracker, https://github.com/Tharos-ux/gfagraphs/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gfagraphs-0.3.2/pgGraphs/abstractions.py` & `gfagraphs-0.3.3/pgGraphs/abstractions.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,47 +13,33 @@
     """
     FORWARD = '+'
     REVERSE = '-'
     ANY = '?'
     BOTH = '='
 
 
-class EdgeOrientation(Enum):
-    """Describes the way an edge direction is encoded
-
-    Parameters
-    ----------
-    Enum : str
-        One of the following: +/+, +/-, -/+, -/-
-    """
-    FF = '+/+'
-    RR = '-/-'
-    FR = '+/-'
-    RF = '-/+'
-
-
-def reverse(orientation: EdgeOrientation) -> EdgeOrientation:
+def reverse(orientation: Orientation) -> Orientation:
     """Returns the orientation of the reverse edge
 
     Parameters
     ----------
-    orientation : EdgeOrientation
-        _description_
+    orientation : Orientation
+        The orientation the edge is pointing on
 
     Returns
     -------
-    EdgeOrientation
+    Orientation
         The complementary operation
     """
     return {
-        EdgeOrientation.FF: EdgeOrientation.RR,
-        EdgeOrientation.RR: EdgeOrientation.FF,
-        EdgeOrientation.RF: EdgeOrientation.FR,
-        EdgeOrientation.FR: EdgeOrientation.RF,
-    }
+        Orientation.FORWARD: Orientation.REVERSE,
+        Orientation.REVERSE: Orientation.FORWARD,
+        Orientation.ANY: Orientation.ANY,
+        Orientation.BOTH: Orientation.BOTH,
+    }[orientation]
 
 
 class GFAFormat(Enum):
     """Describes the different possible gfa-like formats.
     Please refer to http://gfa-spec.github.io/GFA-spec/GFA1.html for examples and full description of the format.
 
     Parameters
```

### Comparing `gfagraphs-0.3.2/pgGraphs/gfaparser.py` & `gfagraphs-0.3.3/pgGraphs/gfaparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from re import match
 from typing import Callable
 from json import loads, dumps
 from os import path, stat
 from tharospytools.path_tools import path_allocator
-from pgGraphs.abstractions import Orientation, GFALine, GFAFormat, EdgeOrientation
+from pgGraphs.abstractions import Orientation, GFALine, GFAFormat
 from gzip import open as gz_open
 from re import search
 
 
 class GFAParser:
     """This class implements static methods to get informations about the contents of a GFA file, and to parse them.
 
@@ -233,15 +233,15 @@
             a pattern to keep for path names, by default ".*"
         memory_mode : bool, optional
             if additional information should be loaded in the struct, by default True
 
         Returns
         -------
         tuple[str, GFALine, dict]
-            Conatins `id_of_line`, `type_of_line`, `datas_of_line`
+            Contains `id_of_line`, `type_of_line`, `datas_of_line`
         """
         line_datas: dict = dict()
         if not (datas[0].isupper() or len(datas) == 0):
             return (None, None, None)
 
         match (line_type := GFALine(datas[0])):
             case GFALine.SEGMENT:
@@ -250,19 +250,22 @@
                     line_datas["seq"] = datas[2]
                 if memory_mode:
                     return (datas[1], line_type, {**line_datas, **GFAParser.supplementary_datas(datas, 3)})
                 else:
                     return (datas[1], line_type, line_datas)
             case GFALine.LINE:
                 if not memory_mode:
-                    line_datas["orientation"] = {
-                        EdgeOrientation(
-                            f"{datas[2]}/{datas[4]}"
-                        )
-                    }
+                    line_datas["orientation"] = set(
+                        [
+                            (
+                                Orientation(datas[2]),
+                                Orientation(datas[4]),
+                            )
+                        ]
+                    )
                     return ((datas[1], datas[3]), line_type, {**line_datas, **GFAParser.supplementary_datas(datas, 5)})
                 else:
                     return (None, None, None)
             case GFALine.WALK:
                 line_datas["name"] = datas[1]
                 line_datas["id"] = datas[3]
                 line_datas["origin"] = datas[2]
@@ -299,15 +302,15 @@
                         regexp_pattern, datas[1]).group(1).upper()
                 except:
                     label: str = datas[1].upper()
                 return (label, line_type, {**line_datas, **GFAParser.supplementary_datas(datas, 7)})
             case GFALine.HEADER | GFALine.ANY:
                 return (None, line_type, GFAParser.supplementary_datas(datas, 1))
 
-    @staticmethod
+    @ staticmethod
     def save_graph(graph, output_path: str, force_format: GFAFormat | bool = False, minimal_graph: bool = False) -> None:
         """Given a gfa Graph object, saves to a valid gfa file the Graph.
 
         Parameters
         ----------
         graph : Graph
             the graph object loaded in memory
@@ -352,17 +355,17 @@
                         "S\t"+f"{segment_name}\t{segment_datas['seq'] if 'seq' in segment_datas else 'N'*segment_datas['length']}{supplementary_text}\n")
             if graph.lines:
                 for (source, sink), line in graph.lines.items():
                     supplementary_text: str = '' if minimal_graph else "\t" + '\t'.join(
                         [f"{key}:{GFAParser.get_python_type(value)}:{GFAParser.set_gfa_type(GFAParser.get_python_type(value))(value)}" if not key.startswith('ARG') else str(value) for key, value in line.items() if key not in ['orientation', 'start', 'end']])
                     # We accomodate for all alternatives orientation versions that are described in the input graph file to be written back
                     for alt in line['orientation']:
-                        ori1, ori2 = alt.value.split('/')
+                        ori1, ori2 = alt.split('/')
                         gfa_writer.write(
-                            f"L\t"+f"{source}\t{ori1}\t{sink}\t{ori2}\t0M{supplementary_text}\n")
+                            f"L\t"+f"{source}\t{ori1.value}\t{sink}\t{ori2.value}\t0M{supplementary_text}\n")
             if graph.paths:
                 for path_name, path_datas in graph.paths.items():
                     supplementary_text: str = '' if minimal_graph else "\t" + '\t'.join(
                         [f"{key}:{GFAParser.get_python_type(value)}:{GFAParser.set_gfa_type(GFAParser.get_python_type(value))(value)}" if not key.startswith('ARG') else str(value) for key, value in path_datas.items() if key not in ['path', 'start_offset', 'stop_offset', 'origin', 'name', 'id']])
                     if gfa_format == GFAFormat.GFA1:  # P-line
                         strpath: str = ','.join(
                             [node_name+'+' if orient == Orientation.FORWARD else node_name+'-' for node_name, orient in path_datas['path']])
```

### Comparing `gfagraphs-0.3.2/pgGraphs/graph.py` & `gfagraphs-0.3.3/pgGraphs/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 "Modelizes a graph object"
 from itertools import count
-from pgGraphs.abstractions import GFALine, Orientation, EdgeOrientation, reverse
+from pgGraphs.abstractions import GFALine, Orientation, reverse
 from pgGraphs.gfaparser import GFAParser
 from gzip import open as gz_open
 from tharospytools.multithreading import futures_collector
 from tharospytools.bio_tools import revcomp
 from typing import Any, Generator
 
 
@@ -74,22 +74,34 @@
                             self.segments[name] = datas
                         case GFALine.WALK | GFALine.PATH:
                             self.paths[name] = datas
                         case GFALine.LINE:
                             if name not in self.lines:
                                 self.lines[name] = datas
                             else:
-                                self.lines[name]['orientation'] = self.lines[name].get(
-                                    'orientation', set()).add(datas['orientation'])
+                                try:
+                                    self.lines[name]['orientation'] = self.lines[name].get(
+                                        'orientation',
+                                        {}
+                                    ) | datas['orientation']
+                                except TypeError:
+                                    print(name, self.lines[name].get(
+                                        'orientation', {}), datas['orientation'])
                             if with_reverse_edges:
+                                (_ttad,) = datas['orientation']
                                 if name[::-1] not in self.lines:
-                                    self.lines[name[::-1]] = datas
+                                    self.lines[name[::-1]] = {
+                                        'orientation': set(
+                                            [(reverse(_ttad[0]), reverse(_ttad[1]))]
+                                        )
+                                    }
+                                    self.lines[name[::-1]]
                                 else:
                                     self.lines[name[::-1]]['orientation'] = self.lines[name[::-1]].get(
-                                        'orientation', set()).add(reverse(datas['orientation']))
+                                        'orientation', set()) | set([(reverse(_ttad[0]), reverse(_ttad[1]))])
 
                         case GFALine.HEADER:
                             self.headers.append(datas)
                         case _:
                             pass
 
     def __str__(self) -> str:
@@ -294,20 +306,20 @@
                 ori_source = ori_source.value
             except:
                 raise ValueError("Not compatible with GFA format.")
         if (source, sink) not in self.lines:
             self.lines[(source, sink)] = {
                 'start': source,
                 'end': sink,
-                'orientation': set(EdgeOrientation(f"{ori_source}/{ori_sink}")),
+                'orientation': set([Orientation(ori_source), Orientation(ori_sink)]),
                 **metadata
             }
         else:
             self.lines[(source, sink)]['orientation'] = self.lines[(source, sink)].get(
-                'orientation', set()).add(EdgeOrientation(f"{ori_source}/{ori_sink}"))
+                'orientation', set()) | set([Orientation(ori_source), Orientation(ori_sink)])
 
     def add_path(
         self,
         name: str,
         chain: list[tuple[str, Orientation]],
         start: int = 0,
         end: int | None = None,
@@ -405,24 +417,25 @@
         future_segment_name: list,
         position_to_split: list
     ) -> None:
         """Given a segment to split and a series/single new name(s) + position(s),
         breaks the node in multiple nodes and includes splits them in the Graph data
 
         If you want to split the segment A into A,B, ... you must provide
-        self.split_segments(A,[A,B, ...],[(start_A,end_A),(start_B,end_B), ...])
+        self.split_segments(
+            A,[A,B, ...],[(start_A,end_A),(start_B,end_B), ...])
 
         Parameters
         ----------
         segment_name : str
             the node to split
         future_segment_name : list
             the futures names of the nodes. The current name will be used for the first node of the splitting series
         position_to_split : list
-            a list of breakpoints where to split to. 
+            a list of breakpoints where to split to.
 
         Raises
         ------
         ValueError
             the number of specified breakpoints is incompatible with the number of names provided
         """
         # First, we check if input parameters are correct
```

### Comparing `gfagraphs-0.3.2/pgGraphs/nx.py` & `gfagraphs-0.3.3/pgGraphs/nx.py`

 * *Files identical despite different names*

### Comparing `gfagraphs-0.3.2/pyproject.toml` & `gfagraphs-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
     requires = ["setuptools>=61.0"]
     build-backend = "setuptools.build_meta"
 
     [project]
     name = "gfagraphs"
-    version = "0.3.2"
+    version = "0.3.3"
     authors = [
     { name="Siegfried Dubois", email="siegfried.dubois@inria.fr" },
     ]
     description = "Library to parse, edit and handle in memory GFA graphs"
     readme = "README.md"
     requires-python = ">=3.10"
     classifiers = [
```

### Comparing `gfagraphs-0.3.2/setup.py` & `gfagraphs-0.3.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 #!/usr/bin/env python3
 from setuptools import setup, find_packages
-from subprocess import run, PIPE
 from sys import version_info, stderr
 from setuptools import setup
 from pkg_resources import require
 from sys import argv
 
 NAME: str = "gfagraphs"
 AUTHOR: str = "Siegfried Dubois",
 AUTHOR_EMAIL: str = "siegfried.dubois@inria.fr",
 LICENCE: str = "LICENCE"
 DESCRIPTION: str = "Library to parse, edit and handle in memory GFA graphs"
 REQUIRED_PYTHON: tuple = (3, 10)
 OVERRIDE_VN: bool = True
-VN: str = "0.3.2"
+VN: str = "0.3.3"
 URL: str = "https://github.com/Tharos-ux/gfagraphs"
 REQUIREMENTS: list[str] = [
     'networkx',
     'tharos-pytools',
     'matplotlib',
     'mycolorpy',
 ]
```

