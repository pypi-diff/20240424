# Comparing `tmp/memory_graph-0.2.4.tar.gz` & `tmp/memory_graph-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memory_graph-0.2.4.tar", last modified: Thu Apr 11 20:42:56 2024, max compression
+gzip compressed data, was "memory_graph-0.2.5.tar", last modified: Wed Apr 24 17:48:19 2024, max compression
```

## Comparing `memory_graph-0.2.4.tar` & `memory_graph-0.2.5.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2024-04-11 20:42:56.456853 memory_graph-0.2.4/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1314 2024-02-16 13:16:53.000000 memory_graph-0.2.4/LICENSE.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       25 2024-02-16 13:16:53.000000 memory_graph-0.2.4/MANIFEST.in
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)    20745 2024-04-11 20:42:56.456853 memory_graph-0.2.4/PKG-INFO
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)    20098 2024-04-11 20:38:36.000000 memory_graph-0.2.4/README.md
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2024-04-11 20:42:56.456853 memory_graph-0.2.4/memory_graph/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     5038 2024-04-07 17:46:45.000000 memory_graph-0.2.4/memory_graph/HTML_Table.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3430 2024-04-07 17:46:45.000000 memory_graph-0.2.4/memory_graph/Memory_Graph.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3430 2024-04-08 20:46:55.000000 memory_graph-0.2.4/memory_graph/Memory_Visitor.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3131 2024-04-11 17:51:04.000000 memory_graph-0.2.4/memory_graph/Node.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      847 2024-04-11 17:52:51.000000 memory_graph-0.2.4/memory_graph/Node_Hidden.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4254 2024-04-11 18:14:00.000000 memory_graph-0.2.4/memory_graph/Node_Key_Value.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     2481 2024-04-11 17:52:34.000000 memory_graph-0.2.4/memory_graph/Node_Linear.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3462 2024-04-11 17:53:02.000000 memory_graph-0.2.4/memory_graph/Node_Table.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4134 2024-04-11 18:12:31.000000 memory_graph-0.2.4/memory_graph/Sliced.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     6586 2024-04-07 17:46:45.000000 memory_graph-0.2.4/memory_graph/Slicer.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     6542 2024-04-11 20:41:47.000000 memory_graph-0.2.4/memory_graph/__init__.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      327 2024-04-08 20:50:18.000000 memory_graph-0.2.4/memory_graph/config.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3231 2024-04-08 21:10:10.000000 memory_graph-0.2.4/memory_graph/config_default.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     2400 2024-04-07 17:46:45.000000 memory_graph-0.2.4/memory_graph/config_helpers.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1340 2024-04-07 17:46:45.000000 memory_graph-0.2.4/memory_graph/extension_numpy.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      660 2024-04-07 17:46:45.000000 memory_graph-0.2.4/memory_graph/extension_pandas.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       24 2024-04-08 20:16:22.000000 memory_graph-0.2.4/memory_graph/special_types.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4909 2024-04-08 21:05:52.000000 memory_graph-0.2.4/memory_graph/test.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      536 2024-04-08 19:52:20.000000 memory_graph-0.2.4/memory_graph/test_memory_graph.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      286 2024-04-07 17:46:45.000000 memory_graph-0.2.4/memory_graph/test_memory_visitor.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1944 2024-04-07 17:46:45.000000 memory_graph-0.2.4/memory_graph/utils.py
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2024-04-11 20:42:56.456853 memory_graph-0.2.4/memory_graph.egg-info/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)    20745 2024-04-11 20:42:56.000000 memory_graph-0.2.4/memory_graph.egg-info/PKG-INFO
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      807 2024-04-11 20:42:56.000000 memory_graph-0.2.4/memory_graph.egg-info/SOURCES.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        1 2024-04-11 20:42:56.000000 memory_graph-0.2.4/memory_graph.egg-info/dependency_links.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        9 2024-04-11 20:42:56.000000 memory_graph-0.2.4/memory_graph.egg-info/requires.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       13 2024-04-11 20:42:56.000000 memory_graph-0.2.4/memory_graph.egg-info/top_level.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       38 2024-04-11 20:42:56.456853 memory_graph-0.2.4/setup.cfg
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1037 2024-04-11 20:41:52.000000 memory_graph-0.2.4/setup.py
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2024-04-24 17:48:19.614964 memory_graph-0.2.5/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1314 2024-04-24 17:31:01.000000 memory_graph-0.2.5/LICENSE.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       25 2024-04-24 17:31:01.000000 memory_graph-0.2.5/MANIFEST.in
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)    20745 2024-04-24 17:48:19.614964 memory_graph-0.2.5/PKG-INFO
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)    20098 2024-04-24 17:31:01.000000 memory_graph-0.2.5/README.md
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2024-04-24 17:48:19.614964 memory_graph-0.2.5/memory_graph/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     6717 2024-04-24 17:46:59.000000 memory_graph-0.2.5/memory_graph/__init__.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      327 2024-04-24 17:43:04.000000 memory_graph-0.2.5/memory_graph/config.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3231 2024-04-24 17:43:04.000000 memory_graph-0.2.5/memory_graph/config_default.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     2400 2024-04-24 17:43:04.000000 memory_graph-0.2.5/memory_graph/config_helpers.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1340 2024-04-24 17:43:04.000000 memory_graph-0.2.5/memory_graph/extension_numpy.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      660 2024-04-24 17:43:04.000000 memory_graph-0.2.5/memory_graph/extension_pandas.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     5038 2024-04-24 17:43:04.000000 memory_graph-0.2.5/memory_graph/html_table.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3430 2024-04-24 17:43:04.000000 memory_graph-0.2.5/memory_graph/memory_graph.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3430 2024-04-24 17:43:04.000000 memory_graph-0.2.5/memory_graph/memory_visitor.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3131 2024-04-24 17:43:04.000000 memory_graph-0.2.5/memory_graph/node.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      847 2024-04-24 17:43:04.000000 memory_graph-0.2.5/memory_graph/node_hidden.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4254 2024-04-24 17:43:04.000000 memory_graph-0.2.5/memory_graph/node_key_value.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     2481 2024-04-24 17:43:04.000000 memory_graph-0.2.5/memory_graph/node_linear.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3462 2024-04-24 17:43:04.000000 memory_graph-0.2.5/memory_graph/node_table.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4134 2024-04-24 17:43:04.000000 memory_graph-0.2.5/memory_graph/sliced.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     6586 2024-04-24 17:43:04.000000 memory_graph-0.2.5/memory_graph/slicer.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4909 2024-04-24 17:43:04.000000 memory_graph-0.2.5/memory_graph/test.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      536 2024-04-24 17:43:04.000000 memory_graph-0.2.5/memory_graph/test_memory_graph.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      286 2024-04-24 17:43:04.000000 memory_graph-0.2.5/memory_graph/test_memory_visitor.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1944 2024-04-24 17:43:04.000000 memory_graph-0.2.5/memory_graph/utils.py
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2024-04-24 17:48:19.614964 memory_graph-0.2.5/memory_graph.egg-info/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)    20745 2024-04-24 17:48:19.000000 memory_graph-0.2.5/memory_graph.egg-info/PKG-INFO
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      777 2024-04-24 17:48:19.000000 memory_graph-0.2.5/memory_graph.egg-info/SOURCES.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        1 2024-04-24 17:48:19.000000 memory_graph-0.2.5/memory_graph.egg-info/dependency_links.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        9 2024-04-24 17:48:19.000000 memory_graph-0.2.5/memory_graph.egg-info/requires.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       13 2024-04-24 17:48:19.000000 memory_graph-0.2.5/memory_graph.egg-info/top_level.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       38 2024-04-24 17:48:19.614964 memory_graph-0.2.5/setup.cfg
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1037 2024-04-24 17:47:09.000000 memory_graph-0.2.5/setup.py
```

### Comparing `memory_graph-0.2.4/LICENSE.txt` & `memory_graph-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.4/PKG-INFO` & `memory_graph-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memory_graph
-Version: 0.2.4
+Version: 0.2.5
 Summary: Draws a graph of your data to analyze its structure.
 Home-page: https://github.com/bterwijn/memory_graph
 Author: Bas Terwijn
 Author-email: bterwijn@gmail.com
 License: BSD 2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `memory_graph-0.2.4/README.md` & `memory_graph-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.4/memory_graph/HTML_Table.py` & `memory_graph-0.2.5/memory_graph/html_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from memory_graph.Node import Node 
+from memory_graph.node import Node 
 
 import memory_graph.config as config
 
 import html
 
 def outer_html_table(s, border, color):
     """ Helper function to add the outer HTML table tags to the string s setting the 'border' and 'color'. """
```

### Comparing `memory_graph-0.2.4/memory_graph/Memory_Graph.py` & `memory_graph-0.2.5/memory_graph/memory_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from memory_graph.Memory_Visitor import Memory_Visitor
+from memory_graph.memory_visitor import Memory_Visitor
 
 import memory_graph.config_helpers as config_helpers
 
 import graphviz
 
 class Memory_Graph:
     """
```

### Comparing `memory_graph-0.2.4/memory_graph/Memory_Visitor.py` & `memory_graph-0.2.5/memory_graph/memory_visitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from memory_graph.Node import Node
-from memory_graph.Node_Linear import Node_Linear
-from memory_graph.Node_Key_Value import Node_Key_Value
+from memory_graph.node import Node
+from memory_graph.node_linear import Node_Linear
+from memory_graph.node_key_value import Node_Key_Value
 
 import memory_graph.utils as utils    
 import memory_graph.config as config
 import memory_graph.config_helpers as config_helpers
 
 def default_backtrack_callback(node):
     print('backtrack_callback:', node)
```

### Comparing `memory_graph-0.2.4/memory_graph/Node.py` & `memory_graph-0.2.5/memory_graph/node.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         """
         return f'node{self.node_id}'
     
     def get_html_table(self):
         """
         Return the HTML_Table object that determines how the node is visualized in the graph.
         """
-        from memory_graph.HTML_Table import HTML_Table
+        from memory_graph.html_table import HTML_Table
         html_table = HTML_Table()
         if self.children is None:
             html_table.add_string(f'{self.data}')
         elif self.children.has_data():
             self.fill_html_table(html_table)
         return html_table
```

### Comparing `memory_graph-0.2.4/memory_graph/Node_Hidden.py` & `memory_graph-0.2.5/memory_graph/node_hidden.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from memory_graph.Node import Node
+from memory_graph.node import Node
 
 class Node_Hidden(Node):
     """
     Node_Hidden (subclass of Node) is a node that represents a node that is not shown 
     in the graph. This is used for the children of Node_Key_Value to hide the separate 
     tuples Nodes and visualize the key-value pairs in the Node_Key_Value instead.
     """
```

### Comparing `memory_graph-0.2.4/memory_graph/Node_Key_Value.py` & `memory_graph-0.2.5/memory_graph/node_key_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from memory_graph.Node import Node
-from memory_graph.Node_Hidden import Node_Hidden
-from memory_graph.Slicer import Slicer
+from memory_graph.node import Node
+from memory_graph.node_hidden import Node_Hidden
+from memory_graph.slicer import Slicer
 
 import memory_graph.config_helpers as config_helpers
 import memory_graph.utils as utils
 
 def transform_node_hidden(node_hidden, fun):
     """
     Helper function to forward the transform to the children of the Node_Hidden node.
```

### Comparing `memory_graph-0.2.4/memory_graph/Node_Linear.py` & `memory_graph-0.2.5/memory_graph/node_linear.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from memory_graph.Node import Node
-from memory_graph.Slicer import Slicer
+from memory_graph.node import Node
+from memory_graph.slicer import Slicer
 
 import memory_graph.config_helpers as config_helpers
 
 class Node_Linear(Node):
     """
     Node_Linear (subclass of Node) is a node that represents a linear sequence 
     of data used for most iterable type like list, tuple, set, etc.
```

### Comparing `memory_graph-0.2.4/memory_graph/Node_Table.py` & `memory_graph-0.2.5/memory_graph/node_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from memory_graph.Node import Node
-from memory_graph.Slicer import Slicer
+from memory_graph.node import Node
+from memory_graph.slicer import Slicer
 
 import memory_graph.config_helpers as config_helpers
 
 import math
 
 def add_name_or_index(html_table, index, names):
     """
```

### Comparing `memory_graph-0.2.4/memory_graph/Sliced.py` & `memory_graph-0.2.5/memory_graph/sliced.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from memory_graph.Node import Node
+from memory_graph.node import Node
 
 import memory_graph.utils as utils
 
 class Slice:
     """ Represents a slice of data with its starting index. """
     def __init__(self, index, data):
         self.index = index
```

### Comparing `memory_graph-0.2.4/memory_graph/Slicer.py` & `memory_graph-0.2.5/memory_graph/slicer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from memory_graph.Sliced import Sliced
+from memory_graph.sliced import Sliced
 
 import memory_graph.utils as utils
 
 import math
 
 def make_sliceable(data):
     """ Helper function to convert data to a sliceable type if it is not already. """
```

### Comparing `memory_graph-0.2.4/memory_graph/__init__.py` & `memory_graph-0.2.5/memory_graph/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from memory_graph.Memory_Graph import Memory_Graph
+from memory_graph.memory_graph import Memory_Graph
 
 import memory_graph.config_default as config_default
 import memory_graph.utils as utils
 
 import inspect
 import sys
 
-__version__ = "0.2.04"
+__version__ = "0.2.05"
 __author__ = 'Bas Terwijn'
 
 log_file=sys.stdout
 press_enter_text="press <ENTER> to continue..."
 
 def get_source_location(stack_index):
     """ Helper function to get the source location of the stack with 'stack_index' of the call stack. """
@@ -29,32 +29,35 @@
                  colors = None,
                  vertical_orientations = None,
                  slicers = None):
     """ Creates and returns a memory graph from 'data'. """
     memory_graph = Memory_Graph(data, colors, vertical_orientations, slicers)
     return memory_graph.get_graph()
 
-def show(data,block=False,
+def show(data=None ,block=False, stack_index=2,
                  colors = None,
                  vertical_orientations = None,
                  slicers = None):
     """ Shows the graph of 'data' and optionally blocks. """
+    if data is None:
+        data=get_locals_from_calling_frame(stack_index)
     graph = create_graph(data, colors, vertical_orientations, slicers)
-    #print('graph:',graph)
     graph.view()
     if block:
         input(f"showing '{graph.filename}', {get_source_location(2)}, {press_enter_text}")
 
-def render(data, output_filename=None, block=False,
+def render(data=None, output_filename=None, block=False, stack_index=2,
                  colors = None,
                  vertical_orientations = None,
                  slicers = None):
     """ Renders the graph of 'data' to 'output_filename' and optionally blocks. """
+    if data is None:
+        data=get_locals_from_calling_frame(stack_index)
     graph = create_graph(data, colors, vertical_orientations, slicers)
-    filename = output_filename if output_filename else graph.filename
+    filename = output_filename if output_filename else graph.filename+".pdf"
     graph.render(outfile=filename)
     if block:
         input(f"rendering '{filename}', {get_source_location(2)}, {press_enter_text}")
 
 def to_str(data):
     try:
         return str(data)
```

### Comparing `memory_graph-0.2.4/memory_graph/config_default.py` & `memory_graph-0.2.5/memory_graph/config_default.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ Sets the default configuration values for the memory graph. """
-from memory_graph.Node import Node
-from memory_graph.Node_Linear import Node_Linear
-from memory_graph.Node_Key_Value import Node_Key_Value
-from memory_graph.Node_Hidden import Node_Hidden
-from memory_graph.Node_Table import Node_Table
-from memory_graph.Slicer import Slicer
+from memory_graph.node import Node
+from memory_graph.node_linear import Node_Linear
+from memory_graph.node_key_value import Node_Key_Value
+from memory_graph.node_hidden import Node_Hidden
+from memory_graph.node_table import Node_Table
+from memory_graph.slicer import Slicer
 
 import memory_graph.config as config
 import memory_graph.utils as utils
 
 import types
 
 """ The maxium number of Nodes shown in the graph. When the graph gets too big set this to a smaller number to analyze the problem. A `★` symbol indictes where the gra[h is cut short.  """
```

### Comparing `memory_graph-0.2.4/memory_graph/config_helpers.py` & `memory_graph-0.2.5/memory_graph/config_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """ This module provides helper functions to access the configuration of the memory graph. """
-from memory_graph.Slicer import Slicer
+from memory_graph.slicer import Slicer
 
 import memory_graph.config as config
 import memory_graph.utils as utils
 
 type_to_color = None
 type_to_vertical_orientation = None
 type_to_slicer = None
```

### Comparing `memory_graph-0.2.4/memory_graph/extension_numpy.py` & `memory_graph-0.2.5/memory_graph/extension_numpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ Extension to add the memory graph configuration for Numpy types. """
-from memory_graph.Node_Linear import Node_Linear
-from memory_graph.Node_Table import Node_Table
+from memory_graph.node_linear import Node_Linear
+from memory_graph.node_table import Node_Table
 
 import memory_graph.config as config
 
 import numpy as np
 
 config.no_reference_types |= {
     np.int8 : lambda d : d,
```

### Comparing `memory_graph-0.2.4/memory_graph/extension_pandas.py` & `memory_graph-0.2.5/memory_graph/extension_pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ Extension to add the memory graph configuration for Pandas type. """
-from memory_graph.Node_Linear import Node_Linear
-from memory_graph.Node_Table import Node_Table
+from memory_graph.node_linear import Node_Linear
+from memory_graph.node_table import Node_Table
 
 import memory_graph.config as config
 
 import pandas as pd
 
 config.type_to_node[pd.DataFrame] = lambda data : (
     Node_Table(data,
```

### Comparing `memory_graph-0.2.4/memory_graph/test.py` & `memory_graph-0.2.5/memory_graph/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import memory_graph.config as config
 
 import numpy as np
 import pandas as pd
 import memory_graph.extension_numpy
 import memory_graph.extension_pandas
 
-from memory_graph.Node_Table import Node_Table
-from memory_graph.Memory_Graph import Memory_Graph
+from memory_graph.node_table import Node_Table
+from memory_graph.memory_graph import Memory_Graph
 
 def test_singular(fun):
     data = 100
     fun(data)
 
 def test_linear(fun):
     data = [None, True, 1, 2.2, complex(3,4), 'hello this is a very long string that should be cut off at some point.']
```

### Comparing `memory_graph-0.2.4/memory_graph/utils.py` & `memory_graph-0.2.5/memory_graph/utils.py`

 * *Files identical despite different names*

### Comparing `memory_graph-0.2.4/memory_graph.egg-info/PKG-INFO` & `memory_graph-0.2.5/memory_graph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memory-graph
-Version: 0.2.4
+Version: 0.2.5
 Summary: Draws a graph of your data to analyze its structure.
 Home-page: https://github.com/bterwijn/memory_graph
 Author: Bas Terwijn
 Author-email: bterwijn@gmail.com
 License: BSD 2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `memory_graph-0.2.4/memory_graph.egg-info/SOURCES.txt` & `memory_graph-0.2.5/memory_graph.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 setup.py
-memory_graph/HTML_Table.py
-memory_graph/Memory_Graph.py
-memory_graph/Memory_Visitor.py
-memory_graph/Node.py
-memory_graph/Node_Hidden.py
-memory_graph/Node_Key_Value.py
-memory_graph/Node_Linear.py
-memory_graph/Node_Table.py
-memory_graph/Sliced.py
-memory_graph/Slicer.py
 memory_graph/__init__.py
 memory_graph/config.py
 memory_graph/config_default.py
 memory_graph/config_helpers.py
 memory_graph/extension_numpy.py
 memory_graph/extension_pandas.py
-memory_graph/special_types.py
+memory_graph/html_table.py
+memory_graph/memory_graph.py
+memory_graph/memory_visitor.py
+memory_graph/node.py
+memory_graph/node_hidden.py
+memory_graph/node_key_value.py
+memory_graph/node_linear.py
+memory_graph/node_table.py
+memory_graph/sliced.py
+memory_graph/slicer.py
 memory_graph/test.py
 memory_graph/test_memory_graph.py
 memory_graph/test_memory_visitor.py
 memory_graph/utils.py
 memory_graph.egg-info/PKG-INFO
 memory_graph.egg-info/SOURCES.txt
 memory_graph.egg-info/dependency_links.txt
```

### Comparing `memory_graph-0.2.4/setup.py` & `memory_graph-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description_from_readme = (this_directory / "README.md").read_text()
 
 setup(
     name = 'memory_graph',
-    version = '0.2.04',
+    version = '0.2.05',
     description = 'Draws a graph of your data to analyze its structure.',
     long_description = long_description_from_readme,
     long_description_content_type = 'text/markdown',
     readme = 'README.md',
     url = 'https://github.com/bterwijn/memory_graph',
     author = 'Bas Terwijn',
     author_email = 'bterwijn@gmail.com',
```

