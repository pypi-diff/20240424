# Comparing `tmp/python_binexport-0.3.2.tar.gz` & `tmp/python_binexport-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_binexport-0.3.2.tar", last modified: Wed Apr 24 12:03:40 2024, max compression
+gzip compressed data, was "python_binexport-0.3.3.tar", last modified: Wed Apr 24 13:16:57 2024, max compression
```

## Comparing `python_binexport-0.3.2.tar` & `python_binexport-0.3.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:03:40.278426 python_binexport-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 12:03:31.000000 python_binexport-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-24 12:03:40.278426 python_binexport-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-24 12:03:31.000000 python_binexport-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-24 12:03:31.000000 python_binexport-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 12:03:40.278426 python_binexport-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:03:40.274426 python_binexport-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:03:40.278426 python_binexport-0.3.2/src/binexport/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-24 12:03:31.000000 python_binexport-0.3.2/src/binexport/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3579 2024-04-24 12:03:31.000000 python_binexport-0.3.2/src/binexport/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-04-24 12:03:31.000000 python_binexport-0.3.2/src/binexport/basic_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     8996 2024-04-24 12:03:31.000000 python_binexport-0.3.2/src/binexport/binexport2_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-04-24 12:03:31.000000 python_binexport-0.3.2/src/binexport/expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-04-24 12:03:31.000000 python_binexport-0.3.2/src/binexport/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-24 12:03:31.000000 python_binexport-0.3.2/src/binexport/instruction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-24 12:03:31.000000 python_binexport-0.3.2/src/binexport/operand.py
--rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-04-24 12:03:31.000000 python_binexport-0.3.2/src/binexport/program.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-24 12:03:31.000000 python_binexport-0.3.2/src/binexport/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-24 12:03:31.000000 python_binexport-0.3.2/src/binexport/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:03:40.278426 python_binexport-0.3.2/src/python_binexport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-24 12:03:40.000000 python_binexport-0.3.2/src/python_binexport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-24 12:03:40.000000 python_binexport-0.3.2/src/python_binexport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 12:03:40.000000 python_binexport-0.3.2/src/python_binexport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-24 12:03:40.000000 python_binexport-0.3.2/src/python_binexport.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-24 12:03:40.000000 python_binexport-0.3.2/src/python_binexport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 12:03:40.000000 python_binexport-0.3.2/src/python_binexport.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:16:57.972730 python_binexport-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 13:16:52.000000 python_binexport-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-24 13:16:57.972730 python_binexport-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-24 13:16:52.000000 python_binexport-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-24 13:16:52.000000 python_binexport-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:16:57.972730 python_binexport-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:16:57.968730 python_binexport-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:16:57.972730 python_binexport-0.3.3/src/binexport/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-24 13:16:52.000000 python_binexport-0.3.3/src/binexport/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3579 2024-04-24 13:16:52.000000 python_binexport-0.3.3/src/binexport/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-04-24 13:16:52.000000 python_binexport-0.3.3/src/binexport/basic_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8996 2024-04-24 13:16:52.000000 python_binexport-0.3.3/src/binexport/binexport2_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-04-24 13:16:52.000000 python_binexport-0.3.3/src/binexport/expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-04-24 13:16:52.000000 python_binexport-0.3.3/src/binexport/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-24 13:16:52.000000 python_binexport-0.3.3/src/binexport/instruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-24 13:16:52.000000 python_binexport-0.3.3/src/binexport/operand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-04-24 13:16:52.000000 python_binexport-0.3.3/src/binexport/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-24 13:16:52.000000 python_binexport-0.3.3/src/binexport/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-24 13:16:52.000000 python_binexport-0.3.3/src/binexport/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:16:57.972730 python_binexport-0.3.3/src/python_binexport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-24 13:16:57.000000 python_binexport-0.3.3/src/python_binexport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-24 13:16:57.000000 python_binexport-0.3.3/src/python_binexport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:16:57.000000 python_binexport-0.3.3/src/python_binexport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-24 13:16:57.000000 python_binexport-0.3.3/src/python_binexport.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-24 13:16:57.000000 python_binexport-0.3.3/src/python_binexport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 13:16:57.000000 python_binexport-0.3.3/src/python_binexport.egg-info/top_level.txt
```

### Comparing `python_binexport-0.3.2/LICENSE` & `python_binexport-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_binexport-0.3.2/PKG-INFO` & `python_binexport-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-binexport
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python wrapper to manipulate binexport files (protobuf)
 Author-email: Quarkslab <diffing@quarkslab.com>
 License: AGPL-3.0
 Project-URL: Homepage, https://github.com/quarkslab/python-binexport
 Project-URL: Repository, https://github.com/quarkslab/python-binexport
 Project-URL: Documentation, https://quarkslab.github.io/diffing-portal/exporter/binexport.html#python-binexport
 Project-URL: Bug Tracker, https://github.com/quarkslab/python-binexport/issues
```

### Comparing `python_binexport-0.3.2/README.md` & `python_binexport-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `python_binexport-0.3.2/pyproject.toml` & `python_binexport-0.3.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-binexport"
-version = "0.3.2"
+version = "0.3.3"
 description = "Python wrapper to manipulate binexport files (protobuf)"
 readme = { file = "README.md", content-type = "text/markdown" }
 authors = [{ name = "Quarkslab", email = "diffing@quarkslab.com" }]
 license = {text = "AGPL-3.0"}
 requires-python = ">=3.9"
 dependencies = [
     "python-magic; os_name!='nt'",
```

### Comparing `python_binexport-0.3.2/src/binexport/__main__.py` & `python_binexport-0.3.3/src/binexport/__main__.py`

 * *Files identical despite different names*

### Comparing `python_binexport-0.3.2/src/binexport/basic_block.py` & `python_binexport-0.3.3/src/binexport/basic_block.py`

 * *Files identical despite different names*

### Comparing `python_binexport-0.3.2/src/binexport/binexport2_pb2.py` & `python_binexport-0.3.3/src/binexport/binexport2_pb2.py`

 * *Files identical despite different names*

### Comparing `python_binexport-0.3.2/src/binexport/expression.py` & `python_binexport-0.3.3/src/binexport/expression.py`

 * *Files identical despite different names*

### Comparing `python_binexport-0.3.2/src/binexport/function.py` & `python_binexport-0.3.3/src/binexport/function.py`

 * *Files identical despite different names*

### Comparing `python_binexport-0.3.2/src/binexport/instruction.py` & `python_binexport-0.3.3/src/binexport/instruction.py`

 * *Files identical despite different names*

### Comparing `python_binexport-0.3.2/src/binexport/operand.py` & `python_binexport-0.3.3/src/binexport/operand.py`

 * *Files identical despite different names*

### Comparing `python_binexport-0.3.2/src/binexport/program.py` & `python_binexport-0.3.3/src/binexport/program.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,17 @@
     def __init__(self, file: pathlib.Path | str):
         """
         :param file: BinExport file path
         """
         super(ProgramBinExport, self).__init__()
 
         self._pb = BinExport2()
+
+        self.path: pathlib.Path = pathlib.Path(file)  #: Binexport file path
+
         with open(file, "rb") as f:
             self._pb.ParseFromString(f.read())
         self.mask = 0xFFFFFFFF if self.architecture.endswith("32") else 0xFFFFFFFFFFFFFFFF
         self.fun_names: dict[str, FunctionBinExport] = {}  #: dictionary function name -> name
         self.callgraph: networkx.DiGraph = networkx.DiGraph()  #: program callgraph (as Digraph)
 
         # Make the data refs map {instruction index -> address referred}
```

### Comparing `python_binexport-0.3.2/src/binexport/types.py` & `python_binexport-0.3.3/src/binexport/types.py`

 * *Files identical despite different names*

### Comparing `python_binexport-0.3.2/src/binexport/utils.py` & `python_binexport-0.3.3/src/binexport/utils.py`

 * *Files identical despite different names*

### Comparing `python_binexport-0.3.2/src/python_binexport.egg-info/PKG-INFO` & `python_binexport-0.3.3/src/python_binexport.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-binexport
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python wrapper to manipulate binexport files (protobuf)
 Author-email: Quarkslab <diffing@quarkslab.com>
 License: AGPL-3.0
 Project-URL: Homepage, https://github.com/quarkslab/python-binexport
 Project-URL: Repository, https://github.com/quarkslab/python-binexport
 Project-URL: Documentation, https://quarkslab.github.io/diffing-portal/exporter/binexport.html#python-binexport
 Project-URL: Bug Tracker, https://github.com/quarkslab/python-binexport/issues
```

### Comparing `python_binexport-0.3.2/src/python_binexport.egg-info/SOURCES.txt` & `python_binexport-0.3.3/src/python_binexport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

