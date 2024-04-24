# Comparing `tmp/pyvisjs-0.0.0.dev3.tar.gz` & `tmp/pyvisjs-0.0.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvisjs-0.0.0.dev3.tar", last modified: Tue Apr 23 14:09:49 2024, max compression
+gzip compressed data, was "pyvisjs-0.0.0.dev4.tar", last modified: Wed Apr 24 18:49:31 2024, max compression
```

## Comparing `pyvisjs-0.0.0.dev3.tar` & `pyvisjs-0.0.0.dev4.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 14:09:49.744351 pyvisjs-0.0.0.dev3/
--rw-rw-rw-   0 root         (0) root         (0)     1327 2024-04-23 14:09:33.000000 pyvisjs-0.0.0.dev3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      907 2024-04-23 14:09:33.000000 pyvisjs-0.0.0.dev3/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     3452 2024-04-23 14:09:33.000000 pyvisjs-0.0.0.dev3/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)     1091 2024-04-23 14:09:33.000000 pyvisjs-0.0.0.dev3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3385 2024-04-23 14:09:49.744351 pyvisjs-0.0.0.dev3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1455 2024-04-23 14:09:33.000000 pyvisjs-0.0.0.dev3/README.md
--rw-rw-rw-   0 root         (0) root         (0)      967 2024-04-23 14:09:33.000000 pyvisjs-0.0.0.dev3/example.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 14:09:49.740351 pyvisjs-0.0.0.dev3/examples/
--rw-rw-rw-   0 root         (0) root         (0)      537 2024-04-23 14:09:33.000000 pyvisjs-0.0.0.dev3/examples/main.py
--rw-rw-rw-   0 root         (0) root         (0)      194 2024-04-23 14:09:33.000000 pyvisjs-0.0.0.dev3/examples/readme_usage.py
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-04-23 14:09:33.000000 pyvisjs-0.0.0.dev3/folder_structure.txt
--rw-rw-rw-   0 root         (0) root         (0)      830 2024-04-23 14:09:33.000000 pyvisjs-0.0.0.dev3/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 14:09:49.741351 pyvisjs-0.0.0.dev3/pyvisjs/
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-23 14:09:33.000000 pyvisjs-0.0.0.dev3/pyvisjs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      105 2024-04-23 14:09:33.000000 pyvisjs-0.0.0.dev3/pyvisjs/_version.py
--rw-rw-rw-   0 root         (0) root         (0)      181 2024-04-23 14:09:33.000000 pyvisjs-0.0.0.dev3/pyvisjs/edge.py
--rw-rw-rw-   0 root         (0) root         (0)     1512 2024-04-23 14:09:33.000000 pyvisjs-0.0.0.dev3/pyvisjs/network.py
--rw-rw-rw-   0 root         (0) root         (0)      232 2024-04-23 14:09:33.000000 pyvisjs-0.0.0.dev3/pyvisjs/node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 14:09:49.742351 pyvisjs-0.0.0.dev3/pyvisjs/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1075 2024-04-23 14:09:33.000000 pyvisjs-0.0.0.dev3/pyvisjs/templates/basic.html
--rw-rw-rw-   0 root         (0) root         (0)     1114 2024-04-23 14:09:33.000000 pyvisjs-0.0.0.dev3/pyvisjs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 14:09:49.743351 pyvisjs-0.0.0.dev3/pyvisjs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3385 2024-04-23 14:09:49.000000 pyvisjs-0.0.0.dev3/pyvisjs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      518 2024-04-23 14:09:49.000000 pyvisjs-0.0.0.dev3/pyvisjs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 14:09:49.000000 pyvisjs-0.0.0.dev3/pyvisjs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-04-23 14:09:49.000000 pyvisjs-0.0.0.dev3/pyvisjs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-23 14:09:49.000000 pyvisjs-0.0.0.dev3/pyvisjs.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-04-23 14:09:33.000000 pyvisjs-0.0.0.dev3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 14:09:49.744351 pyvisjs-0.0.0.dev3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 14:09:49.743351 pyvisjs-0.0.0.dev3/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 14:09:33.000000 pyvisjs-0.0.0.dev3/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4344 2024-04-23 14:09:33.000000 pyvisjs-0.0.0.dev3/tests/test_network.py
--rw-rw-rw-   0 root         (0) root         (0)     2507 2024-04-23 14:09:33.000000 pyvisjs-0.0.0.dev3/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 18:49:31.507796 pyvisjs-0.0.0.dev4/
+-rw-rw-rw-   0 root         (0) root         (0)     1355 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1054 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3452 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3384 2024-04-24 18:49:31.507796 pyvisjs-0.0.0.dev4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1454 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 18:49:31.502796 pyvisjs-0.0.0.dev4/examples/
+-rw-rw-rw-   0 root         (0) root         (0)      537 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/examples/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      194 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/examples/readme_usage.py
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/folder_structure.txt
+-rw-rw-rw-   0 root         (0) root         (0)      830 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 18:49:31.504796 pyvisjs-0.0.0.dev4/pyvisjs/
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/pyvisjs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      105 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/pyvisjs/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      371 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/pyvisjs/edge.py
+-rw-rw-rw-   0 root         (0) root         (0)     1786 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/pyvisjs/network.py
+-rw-rw-rw-   0 root         (0) root         (0)      687 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/pyvisjs/node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 18:49:31.505796 pyvisjs-0.0.0.dev4/pyvisjs/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/pyvisjs/templates/basic.html
+-rw-rw-rw-   0 root         (0) root         (0)     1114 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/pyvisjs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 18:49:31.506796 pyvisjs-0.0.0.dev4/pyvisjs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3384 2024-04-24 18:49:31.000000 pyvisjs-0.0.0.dev4/pyvisjs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      543 2024-04-24 18:49:31.000000 pyvisjs-0.0.0.dev4/pyvisjs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 18:49:31.000000 pyvisjs-0.0.0.dev4/pyvisjs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-24 18:49:31.000000 pyvisjs-0.0.0.dev4/pyvisjs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-24 18:49:31.000000 pyvisjs-0.0.0.dev4/pyvisjs.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 18:49:31.507796 pyvisjs-0.0.0.dev4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 18:49:31.506796 pyvisjs-0.0.0.dev4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      778 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/tests/test_edge.py
+-rw-rw-rw-   0 root         (0) root         (0)     5310 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/tests/test_network.py
+-rw-rw-rw-   0 root         (0) root         (0)     1540 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/tests/test_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     2507 2024-04-24 18:49:15.000000 pyvisjs-0.0.0.dev4/tests/test_utils.py
```

### Comparing `pyvisjs-0.0.0.dev3/.gitignore` & `pyvisjs-0.0.0.dev4/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# pyvisjs specific
+/*.html
+
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
```

### Comparing `pyvisjs-0.0.0.dev3/.gitlab-ci.yml` & `pyvisjs-0.0.0.dev4/.gitlab-ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,22 @@
   image: python:latest
   before_script:
     - pip install --upgrade pip
     - pip install -r requirements.txt
     - pip install -e .
   script:
     - pytest --noconftest
+  rules:
+    - when: on_success
+      changes:
+        - "*.py"
+    - when: never
+      changes:
+        - "_version.py"
+        - "examples/**/*"
 #  except:
 #    - dev
 #  only:
 #    - dev
 
 deploy_to_pypi:
   stage: deploy
```

### Comparing `pyvisjs-0.0.0.dev3/CONTRIBUTING.md` & `pyvisjs-0.0.0.dev4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev3/LICENSE` & `pyvisjs-0.0.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev3/PKG-INFO` & `pyvisjs-0.0.0.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisjs
-Version: 0.0.0.dev3
+Version: 0.0.0.dev4
 Summary: A Python wrapper for vis.js Network
 Author-email: Andrey Morozov <andrey@morozov.lv>
 License: MIT License
         
         Copyright (c) 2024 Andrey Morozov (andrey@morozov.lv)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,15 +47,15 @@
 
 - **Integration**: Easily incorporate vis.js network visualizations into your Python projects.
 - **Flexibility**: Leverage the power of Python to manipulate network data and customize visualizations.
 - **Interactivity**: Enable users to interact with network visualizations directly from Python scripts.
 
 ## Installation
 
-You can install PyVis.js via pip:
+You can install PyVisjs via pip:
 
 ```bash
 pip install pyvisjs
 ```
 
 ## Usage
```

### Comparing `pyvisjs-0.0.0.dev3/README.md` & `pyvisjs-0.0.0.dev4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 - **Integration**: Easily incorporate vis.js network visualizations into your Python projects.
 - **Flexibility**: Leverage the power of Python to manipulate network data and customize visualizations.
 - **Interactivity**: Enable users to interact with network visualizations directly from Python scripts.
 
 ## Installation
 
-You can install PyVis.js via pip:
+You can install PyVisjs via pip:
 
 ```bash
 pip install pyvisjs
 ```
 
 ## Usage
```

### Comparing `pyvisjs-0.0.0.dev3/example.html` & `pyvisjs-0.0.0.dev4/pyvisjs/templates/basic.html`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 <html>
 <head>
     <script type="text/javascript" src="https://unpkg.com/vis-network/standalone/umd/vis-network.min.js"></script>
 
     <style type="text/css">
         #visjsnet {
-            width: 600px;
-            height: 400px;
+            width: {{width}};
+            height: {{height}};
             border: 1px solid lightgray;
         }
     </style>
 </head>
 
 <body>
 <div id="visjsnet"></div>
 
 <script type="text/javascript">
     // create an array with nodes
     var nodes = new vis.DataSet([
-    
-        {id: 1, label: '1'},
-    
-        {id: 2, label: '2'},
-    
+    {% for node in data["nodes"] %}
+        {{ node.to_json()|safe }},
+    {%- endfor %}
     ]);
 
     // create an array with edges
     var edges = new vis.DataSet([
-    
-        {from: 1, to: '2'},
-    
+    {% for edge in data["edges"] %}
+        {{ edge.to_json()|safe }},
+    {%- endfor %}
     ]);
 
     // create a network
     var container = document.getElementById('visjsnet');
 
     // provide the data in the vis format
     var data = {
```

### Comparing `pyvisjs-0.0.0.dev3/examples/main.py` & `pyvisjs-0.0.0.dev4/examples/main.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev3/folder_structure.txt` & `pyvisjs-0.0.0.dev4/folder_structure.txt`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev3/pyproject.toml` & `pyvisjs-0.0.0.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev3/pyvisjs/network.py` & `pyvisjs-0.0.0.dev4/pyvisjs/network.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,19 +15,24 @@
             loader=PackageLoader("pyvisjs"),
             autoescape=select_autoescape()
         )
 
     def __repr__(self):
         return f"Network(\'{self.name}\', \'{self.width}\', \'{self.height}\')"
     
-    def add_node(self, node_id):
-        self.data["nodes"].append(Node(node_id))
+    def add_node(self, node_id, label=None):
+        if not [node.id for node in self.data["nodes"] if node.id == node_id]:
+            self.data["nodes"].append(Node(node_id, label))
 
     def add_edge(self, from_id, to_id):
-        self.data["edges"].append(Edge(from_id, to_id))
+        self.add_node(from_id)
+        self.add_node(to_id)
+
+        if not [edge.start for edge in self.data["edges"] if edge.start == from_id and edge.end == to_id]:
+            self.data["edges"].append(Edge(from_id, to_id))
 
     def show(self, file_name):
         self.render_template(open_in_browser=True, output_filename=file_name)
 
     def render_template(self, open_in_browser=False, save_to_output=False, output_filename="default.html", template_filename="basic.html") -> str:
         html_output = self.env \
             .get_template(template_filename) \
```

### Comparing `pyvisjs-0.0.0.dev3/pyvisjs/utils.py` & `pyvisjs-0.0.0.dev4/pyvisjs/utils.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-0.0.0.dev3/pyvisjs.egg-info/PKG-INFO` & `pyvisjs-0.0.0.dev4/pyvisjs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisjs
-Version: 0.0.0.dev3
+Version: 0.0.0.dev4
 Summary: A Python wrapper for vis.js Network
 Author-email: Andrey Morozov <andrey@morozov.lv>
 License: MIT License
         
         Copyright (c) 2024 Andrey Morozov (andrey@morozov.lv)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,15 +47,15 @@
 
 - **Integration**: Easily incorporate vis.js network visualizations into your Python projects.
 - **Flexibility**: Leverage the power of Python to manipulate network data and customize visualizations.
 - **Interactivity**: Enable users to interact with network visualizations directly from Python scripts.
 
 ## Installation
 
-You can install PyVis.js via pip:
+You can install PyVisjs via pip:
 
 ```bash
 pip install pyvisjs
 ```
 
 ## Usage
```

### Comparing `pyvisjs-0.0.0.dev3/pyvisjs.egg-info/SOURCES.txt` & `pyvisjs-0.0.0.dev4/pyvisjs.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 .gitignore
 .gitlab-ci.yml
 CONTRIBUTING.md
 LICENSE
 README.md
-example.html
 folder_structure.txt
 pyproject.toml
 requirements.txt
 examples/main.py
 examples/readme_usage.py
 pyvisjs/__init__.py
 pyvisjs/_version.py
@@ -18,9 +17,11 @@
 pyvisjs.egg-info/PKG-INFO
 pyvisjs.egg-info/SOURCES.txt
 pyvisjs.egg-info/dependency_links.txt
 pyvisjs.egg-info/requires.txt
 pyvisjs.egg-info/top_level.txt
 pyvisjs/templates/basic.html
 tests/__init__.py
+tests/test_edge.py
 tests/test_network.py
+tests/test_node.py
 tests/test_utils.py
```

### Comparing `pyvisjs-0.0.0.dev3/tests/test_utils.py` & `pyvisjs-0.0.0.dev4/tests/test_utils.py`

 * *Files identical despite different names*

