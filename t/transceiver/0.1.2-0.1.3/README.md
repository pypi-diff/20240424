# Comparing `tmp/transceiver-0.1.2.tar.gz` & `tmp/transceiver-0.1.3.tar.gz`

## Comparing `transceiver-0.1.2.tar` & `transceiver-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,14 @@
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 transceiver-0.1.2/.gitmodules
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 transceiver-0.1.2/.python-version
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 transceiver-0.1.2/make.py
--rwxr-xr-x   0        0        0       79 2020-02-02 00:00:00.000000 transceiver-0.1.2/make.sh
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 transceiver-0.1.2/repositories/ComfyUI-Annotations/.git
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 transceiver-0.1.2/repositories/ComfyUI-Annotations/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 transceiver-0.1.2/repositories/ComfyUI-Annotations/LICENSE
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 transceiver-0.1.2/repositories/ComfyUI-Annotations/__init__.py
--rw-r--r--   0        0        0    17164 2020-02-02 00:00:00.000000 transceiver-0.1.2/repositories/ComfyUI-Annotations/comfy_annotations.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 transceiver-0.1.2/repositories/ComfyUI-Annotations/pyproject.toml
--rw-r--r--   0        0        0     7377 2020-02-02 00:00:00.000000 transceiver-0.1.2/repositories/ComfyUI-Annotations/readme.md
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 transceiver-0.1.2/repositories/ComfyUI-Annotations/example/__init__.py
--rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 transceiver-0.1.2/repositories/ComfyUI-Annotations/example/example_nodes.py
--rw-r--r--   0        0        0    15204 2020-02-02 00:00:00.000000 transceiver-0.1.2/repositories/ComfyUI-Annotations/example/example_workflow.json
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 transceiver-0.1.2/src/transceiver/__init__.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 transceiver-0.1.2/src/transceiver/pyarrow_example.py
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 transceiver-0.1.2/src/transceiver/save_image_mem.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transceiver-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 transceiver-0.1.2/tests/test_null.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 transceiver-0.1.2/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 transceiver-0.1.2/LICENSE
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 transceiver-0.1.2/README.md
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 transceiver-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 transceiver-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transceiver-0.1.3/.gitmodules
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 transceiver-0.1.3/.python-version
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 transceiver-0.1.3/make.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transceiver-0.1.3/src/transceiver/__init__.py
+-rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 transceiver-0.1.3/src/transceiver/core.py
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 transceiver-0.1.3/src/transceiver/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transceiver-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 transceiver-0.1.3/tests/test_core.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 transceiver-0.1.3/tests/test_utils.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 transceiver-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 transceiver-0.1.3/LICENSE
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 transceiver-0.1.3/README.md
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 transceiver-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 transceiver-0.1.3/PKG-INFO
```

### Comparing `transceiver-0.1.2/make.py` & `transceiver-0.1.3/make.py`

 * *Files identical despite different names*

### Comparing `transceiver-0.1.2/.gitignore` & `transceiver-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `transceiver-0.1.2/LICENSE` & `transceiver-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `transceiver-0.1.2/README.md` & `transceiver-0.1.3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,25 @@
-# transceiver
+# Transceiver📡
 
-transceiver is a Python library that swiftly exchanges complex data structures such as numpy arrays and PIL images between processes, optimizing AI inference tasks that utilize ComfyUI.
+Please see [**comfyui-transceiver**](https://github.com/nat-chan/comfyui-transceiver),  the ComfyUI custom nodes binding of the "transceiver" library.
 
-## why?
+
+"transceiver" is a python library that swiftly exchanges fundamental data structures, specifically numpy arrays, between processes, optimizing AI inference tasks that utilize ComfyUI.
+
+## Why?
 
 When processing a large number of requests, the SaveImage and LoadImage nodes may be IO-limited, and using shared memory improves performance by passing images only through memory access, not through IO.
 
-## install
+## Installation
 
+The "transceiver" is indexed by PyPI. You can easily integrate it into any project.
+
+```bash
+pip install transceiver
 ```
-cd /path/to/ComfyUI
-source venv/bin/activate
-cd custom_nodes
-git clone https://github.com/nat-chan/comfyui-in-memory-transceiver
-cd comfyui-in-memory-transceiver
-pip install -e .
-cd ../.. # cd /path/to/ComfyUI
-python main.py # launch
-```
-## features
 
-### SaveImageMem
+## Features
 
-todo
 
-### LoadImageMem
+UNDER CONSTRUCTION
 
-todo
+See [core.py](/src/transceiver/core.py) doc
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `transceiver-0.1.2/pyproject.toml` & `transceiver-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "transceiver"
-version = "0.1.2"
-description = "transceiver is a Python library that swiftly exchanges complex data structures such as numpy arrays and PIL images between processes, optimizing AI inference tasks that utilize ComfyUI."
-dependencies = [ "fs>=2.4.16", "numpy>=1.26.4", "pyarrow>=16.0.0",]
+version = "0.1.3"
+description = "Transceiver is a python library that swiftly exchanges fundamental data structures, specifically numpy arrays, between processes, optimizing AI inference tasks that utilize ComfyUI."
+dependencies = [ "numpy>=1.26.4",]
 readme = "README.md"
 requires-python = ">= 3.10"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
 [[project.authors]]
 name = "nat-chan"
 email = "ogino.natsuki.tm@alumni.tsukuba.ac.jp"
 
@@ -16,24 +16,21 @@
 
 [project.urls]
 Homepage = "https://github.com/nat-chan/transceiver"
 Issues = "https://github.com/nat-chan/transceiver/issues"
 
 [tool.rye]
 managed = true
-dev-dependencies = [ "ipykernel>=6.29.4", "ruff", "mypy", "pydantic", "pytest", "build>=1.2.1", "twine>=5.0.0", "toml>=0.10.2",]
+dev-dependencies = [ "ipykernel>=6.29.4", "ruff", "mypy", "pydantic", "pytest", "build>=1.2.1", "twine>=5.0.0", "toml>=0.10.2", "grip>=4.6.2",]
 
 [tool.ruff]
 line-length = 88
 indent-width = 4
 target-version = "py310"
 
-[tool.rye.workspace]
-members = [ "repositories/**/*",]
-
 [tool.ruff.lint]
 exclude = [ ".venv",]
 select = [ "B", "C4", "E", "G", "W", "F", "I", "UP", "EXE", "F", "SIM1", "LOG", "NPY", "PERF", "PGH004", "PIE794", "PIE800", "PIE804", "PIE807", "PIE810", "PLC0131", "PLC0132", "PLC0205", "PLE", "PLR0133", "PLR0206", "PLR1722", "PLW0129", "PLW0406", "PLW0711", "PLW1509", "PLW3301", "PT006", "PT022", "PT023", "PT024", "PT025", "PT026", "PYI", "RUF008", "RUF015", "RUF016", "RUF017", "TRY200", "TRY302",]
 
 [tool.hatch.metadata]
 allow-direct-references = true
```

### Comparing `transceiver-0.1.2/PKG-INFO` & `transceiver-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,40 @@
 Metadata-Version: 2.3
 Name: transceiver
-Version: 0.1.2
-Summary: transceiver is a Python library that swiftly exchanges complex data structures such as numpy arrays and PIL images between processes, optimizing AI inference tasks that utilize ComfyUI.
+Version: 0.1.3
+Summary: Transceiver is a python library that swiftly exchanges fundamental data structures, specifically numpy arrays, between processes, optimizing AI inference tasks that utilize ComfyUI.
 Project-URL: Homepage, https://github.com/nat-chan/transceiver
 Project-URL: Issues, https://github.com/nat-chan/transceiver/issues
 Author-email: nat-chan <ogino.natsuki.tm@alumni.tsukuba.ac.jp>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
-Requires-Dist: fs>=2.4.16
 Requires-Dist: numpy>=1.26.4
-Requires-Dist: pyarrow>=16.0.0
 Description-Content-Type: text/markdown
 
-# transceiver
+# Transceiver📡
 
-transceiver is a Python library that swiftly exchanges complex data structures such as numpy arrays and PIL images between processes, optimizing AI inference tasks that utilize ComfyUI.
+Please see [**comfyui-transceiver**](https://github.com/nat-chan/comfyui-transceiver),  the ComfyUI custom nodes binding of the "transceiver" library.
 
-## why?
+
+"transceiver" is a python library that swiftly exchanges fundamental data structures, specifically numpy arrays, between processes, optimizing AI inference tasks that utilize ComfyUI.
+
+## Why?
 
 When processing a large number of requests, the SaveImage and LoadImage nodes may be IO-limited, and using shared memory improves performance by passing images only through memory access, not through IO.
 
-## install
+## Installation
 
+The "transceiver" is indexed by PyPI. You can easily integrate it into any project.
+
+```bash
+pip install transceiver
 ```
-cd /path/to/ComfyUI
-source venv/bin/activate
-cd custom_nodes
-git clone https://github.com/nat-chan/comfyui-in-memory-transceiver
-cd comfyui-in-memory-transceiver
-pip install -e .
-cd ../.. # cd /path/to/ComfyUI
-python main.py # launch
-```
-## features
 
-### SaveImageMem
+## Features
 
-todo
 
-### LoadImageMem
+UNDER CONSTRUCTION
 
-todo
+See [core.py](/src/transceiver/core.py) doc
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

