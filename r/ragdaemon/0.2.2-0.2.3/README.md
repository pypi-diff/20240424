# Comparing `tmp/ragdaemon-0.2.2.tar.gz` & `tmp/ragdaemon-0.2.3.tar.gz`

## Comparing `ragdaemon-0.2.2.tar` & `ragdaemon-0.2.3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/tutorial.ipynb
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/__main__.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/app.py
--rw-r--r--   0        0        0     8808 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/context.py
--rw-r--r--   0        0        0     6047 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/errors.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/get_paths.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/graph.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/llm.py
--rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/utils.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/annotators/chunker.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/annotators/chunker_line.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/annotators/chunker_llm.py
--rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/database/database.py
--rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/tests/conftest.py
--rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/tests/test_comments.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/tests/test_context.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/tests/test_daemon.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/tests/test_database.py
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/tests/test_get_paths.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/tests/test_sample.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/tests/data/context_message.txt
--rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/tests/data/diff_graph.json
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/README.md
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    13747 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tutorial.ipynb
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/app.py
+-rw-r--r--   0        0        0     8808 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/context.py
+-rw-r--r--   0        0        0     6150 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/errors.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/get_paths.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/graph.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/llm.py
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/utils.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/annotators/chunker.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/annotators/chunker_line.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/annotators/chunker_llm.py
+-rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/conftest.py
+-rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/test_comments.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/test_context.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/test_daemon.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/test_database.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/test_get_paths.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/test_sample.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/data/context_message.txt
+-rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/README.md
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.2.3/PKG-INFO
```

### Comparing `ragdaemon-0.2.2/.github/workflows/run-tests.yml` & `ragdaemon-0.2.3/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/ragdaemon/app.py` & `ragdaemon-0.2.3/ragdaemon/app.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/ragdaemon/context.py` & `ragdaemon-0.2.3/ragdaemon/context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/ragdaemon/daemon.py` & `ragdaemon-0.2.3/ragdaemon/daemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from ragdaemon.annotators import Annotator, annotators_map
 from ragdaemon.context import ContextBuilder
 from ragdaemon.database import DEFAULT_EMBEDDING_MODEL, Database, get_db
 from ragdaemon.get_paths import get_paths_for_directory
 from ragdaemon.graph import KnowledgeGraph
 from ragdaemon.llm import DEFAULT_COMPLETION_MODEL
+from ragdaemon.utils import mentat_dir_path
 
 
 def default_annotators():
     return {
         "hierarchy": {},
         "chunker_line": {"lines_per_chunk": 30},
         "diff": {},
@@ -40,15 +41,17 @@
         provider: Optional[str] = None,
     ):
         self.cwd = cwd
         self.verbose = verbose
         if graph_path is not None:
             self.graph_path = (cwd / graph_path).resolve()
         else:
-            self.graph_path = self.cwd / ".ragdaemon" / "graph.json"
+            self.graph_path = (
+                mentat_dir_path / "ragdaemon" / f"ragdaemon-{self.cwd.name}.json"
+            )
         self.graph_path.parent.mkdir(exist_ok=True)
         if spice_client is None:
             spice_client = Spice(
                 default_text_model=DEFAULT_COMPLETION_MODEL,
                 default_embeddings_model=model,
             )
         self.spice_client = spice_client
```

### Comparing `ragdaemon-0.2.2/ragdaemon/get_paths.py` & `ragdaemon-0.2.3/ragdaemon/get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/ragdaemon/graph.py` & `ragdaemon-0.2.3/ragdaemon/graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/ragdaemon/utils.py` & `ragdaemon-0.2.3/ragdaemon/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     elif type in {"file", "chunk"}:
         path, lines = parse_path_ref(ref)
         if lines:
             text = ""
             with open(cwd / path, "r") as f:
                 file_lines = f.read().split("\n")
             for line in sorted(lines):
-                text += f"{line}:{file_lines[line - 1]}\n"
+                text += f"{file_lines[line - 1]}\n"
         else:
             try:
                 with open(cwd / path, "r") as f:
                     text = f.read()
             except UnicodeDecodeError:
                 raise RagdaemonError(f"Not a text file: {path}")
     else:
```

### Comparing `ragdaemon-0.2.2/ragdaemon/annotators/__init__.py` & `ragdaemon-0.2.3/ragdaemon/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.2.3/ragdaemon/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/ragdaemon/annotators/chunker.py` & `ragdaemon-0.2.3/ragdaemon/annotators/chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/ragdaemon/annotators/chunker_line.py` & `ragdaemon-0.2.3/ragdaemon/annotators/chunker_line.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/ragdaemon/annotators/chunker_llm.py` & `ragdaemon-0.2.3/ragdaemon/annotators/chunker_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/ragdaemon/annotators/diff.py` & `ragdaemon-0.2.3/ragdaemon/annotators/diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.2.3/ragdaemon/annotators/hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.2.3/ragdaemon/annotators/layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/ragdaemon/database/__init__.py` & `ragdaemon-0.2.3/ragdaemon/database/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/ragdaemon/database/chroma_database.py` & `ragdaemon-0.2.3/ragdaemon/database/chroma_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/ragdaemon/database/database.py` & `ragdaemon-0.2.3/ragdaemon/database/database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/ragdaemon/database/lite_database.py` & `ragdaemon-0.2.3/ragdaemon/database/lite_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/ragdaemon/static/favicon.ico` & `ragdaemon-0.2.3/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.2.3/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/ragdaemon/static/js/main.js` & `ragdaemon-0.2.3/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.2.3/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/ragdaemon/static/js/three/node.js` & `ragdaemon-0.2.3/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.2.3/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/ragdaemon/templates/index.html` & `ragdaemon-0.2.3/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/tests/conftest.py` & `ragdaemon-0.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/tests/test_comments.py` & `ragdaemon-0.2.3/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/tests/test_context.py` & `ragdaemon-0.2.3/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/tests/test_daemon.py` & `ragdaemon-0.2.3/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/tests/test_get_paths.py` & `ragdaemon-0.2.3/tests/test_get_paths.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,13 @@
 
     is_git_repo = get_git_root_for_path(git_history, raise_error=False)
     assert not is_git_repo, "Is a git repository"
 
     paths = get_paths_for_directory(git_history)
     assert paths == {
         Path(".gitignore"),
-        Path(".ragdaemon/graph.json"),  # Generated by other tests and ignored
         Path("README.md"),
         Path("hello.py"),
         Path("src/__init__.py"),
         Path("src/interface.py"),
         Path("src/operations.py"),
     }, "Paths are not equal"
```

### Comparing `ragdaemon-0.2.2/tests/test_sample.py` & `ragdaemon-0.2.3/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/tests/annotators/test_chunker.py` & `ragdaemon-0.2.3/tests/annotators/test_chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/tests/annotators/test_diff.py` & `ragdaemon-0.2.3/tests/annotators/test_diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/tests/annotators/test_hierarchy.py` & `ragdaemon-0.2.3/tests/annotators/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.2.3/tests/annotators/test_layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/tests/data/chunker_graph.json` & `ragdaemon-0.2.3/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/tests/data/context_message.txt` & `ragdaemon-0.2.3/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/tests/data/diff_graph.json` & `ragdaemon-0.2.3/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/tests/data/hierarchy_graph.json` & `ragdaemon-0.2.3/tests/data/hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.2.3/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/tests/sample/src/interface.py` & `ragdaemon-0.2.3/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/LICENSE` & `ragdaemon-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/README.md` & `ragdaemon-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.2/pyproject.toml` & `ragdaemon-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.2.2"
+version = "0.2.3"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
     "chromadb==0.4.24",
     "dict2xml==1.7.5",
     "fastapi==0.109.2",
     "Jinja2==3.1.3",
     "networkx==3.2.1",
     "spiceai~=0.2.0",
     "starlette==0.36.3",
     "tqdm==4.66.2",
-    "uvicorn==0.27.1",
+    "uvicorn==0.29.0",
 ]
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `ragdaemon-0.2.2/PKG-INFO` & `ragdaemon-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.2.2
+Version: 0.2.3
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
@@ -12,15 +12,15 @@
 Requires-Dist: dict2xml==1.7.5
 Requires-Dist: fastapi==0.109.2
 Requires-Dist: jinja2==3.1.3
 Requires-Dist: networkx==3.2.1
 Requires-Dist: spiceai~=0.2.0
 Requires-Dist: starlette==0.36.3
 Requires-Dist: tqdm==4.66.2
-Requires-Dist: uvicorn==0.27.1
+Requires-Dist: uvicorn==0.29.0
 Provides-Extra: dev
 Requires-Dist: pyright; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-asyncio; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Description-Content-Type: text/markdown
```

