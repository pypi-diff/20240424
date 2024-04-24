# Comparing `tmp/svdi-1.0.0.tar.gz` & `tmp/svdi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svdi-1.0.0.tar", max compression
+gzip compressed data, was "svdi-1.0.1.tar", max compression
```

## Comparing `svdi-1.0.0.tar` & `svdi-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1061 2024-04-24 00:56:29.315066 svdi-1.0.0/LICENCE
--rw-r--r--   0        0        0     2166 2024-04-24 00:56:29.315066 svdi-1.0.0/README.md
--rw-r--r--   0        0        0      578 2024-04-24 00:56:29.327067 svdi-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-24 00:56:29.327067 svdi-1.0.0/svdi/__init__.py
--rw-r--r--   0        0        0     2196 2024-04-24 00:56:29.327067 svdi-1.0.0/svdi/cli.py
--rw-r--r--   0        0        0       72 2024-04-24 00:56:29.327067 svdi-1.0.0/svdi/constant.py
--rw-r--r--   0        0        0        0 2024-04-24 00:56:29.327067 svdi-1.0.0/svdi/file/__init__.py
--rw-r--r--   0        0        0     1275 2024-04-24 00:56:29.327067 svdi-1.0.0/svdi/file/format.py
--rw-r--r--   0        0        0     1855 2024-04-24 00:56:29.327067 svdi-1.0.0/svdi/main.py
--rw-r--r--   0        0        0        0 2024-04-24 00:56:29.327067 svdi-1.0.0/svdi/svd/__init__.py
--rw-r--r--   0        0        0      762 2024-04-24 00:56:29.327067 svdi-1.0.0/svdi/svd/basic_rSVD.py
--rw-r--r--   0        0        0      180 2024-04-24 00:56:29.327067 svdi-1.0.0/svdi/svd/numpy_default.py
--rw-r--r--   0        0        0      964 2024-04-24 00:56:29.327067 svdi-1.0.0/svdi/svd/pcafast.py
--rw-r--r--   0        0        0     1358 2024-04-24 00:56:29.327067 svdi-1.0.0/svdi/svd/power_iterations.py
--rw-r--r--   0        0        0       91 2024-04-24 00:56:29.327067 svdi-1.0.0/svdi/svd/result.py
--rw-r--r--   0        0        0     2831 1970-01-01 00:00:00.000000 svdi-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-04-24 01:27:22.094553 svdi-1.0.1/LICENCE
+-rw-r--r--   0        0        0     2163 2024-04-24 01:27:22.094553 svdi-1.0.1/README.md
+-rw-r--r--   0        0        0      578 2024-04-24 01:27:22.106553 svdi-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-24 01:27:22.106553 svdi-1.0.1/svdi/__init__.py
+-rw-r--r--   0        0        0     2213 2024-04-24 01:27:22.106553 svdi-1.0.1/svdi/cli.py
+-rw-r--r--   0        0        0       72 2024-04-24 01:27:22.106553 svdi-1.0.1/svdi/constant.py
+-rw-r--r--   0        0        0        0 2024-04-24 01:27:22.106553 svdi-1.0.1/svdi/file/__init__.py
+-rw-r--r--   0        0        0     1275 2024-04-24 01:27:22.106553 svdi-1.0.1/svdi/file/format.py
+-rw-r--r--   0        0        0     1855 2024-04-24 01:27:22.106553 svdi-1.0.1/svdi/main.py
+-rw-r--r--   0        0        0        0 2024-04-24 01:27:22.106553 svdi-1.0.1/svdi/svd/__init__.py
+-rw-r--r--   0        0        0      762 2024-04-24 01:27:22.106553 svdi-1.0.1/svdi/svd/basic_rSVD.py
+-rw-r--r--   0        0        0      180 2024-04-24 01:27:22.106553 svdi-1.0.1/svdi/svd/numpy_default.py
+-rw-r--r--   0        0        0      964 2024-04-24 01:27:22.106553 svdi-1.0.1/svdi/svd/pcafast.py
+-rw-r--r--   0        0        0     1358 2024-04-24 01:27:22.106553 svdi-1.0.1/svdi/svd/power_iterations.py
+-rw-r--r--   0        0        0       91 2024-04-24 01:27:22.106553 svdi-1.0.1/svdi/svd/result.py
+-rw-r--r--   0        0        0     2828 1970-01-01 00:00:00.000000 svdi-1.0.1/PKG-INFO
```

### Comparing `svdi-1.0.0/LICENCE` & `svdi-1.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `svdi-1.0.0/README.md` & `svdi-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# SVD image compression and decompression tool
+# Image compression and decompression using SVD
 
 ## Installation
 Install CLI using pipx:
 ```bash
 pipx install git+https://github.com/toadharvard/svdi-cli.git
 ```
 Or
 ```bash
-pipx install svdi-cli
+pipx install svdi
 ```
 
 ## Usage example
 ```bash
 svdi compress --in-file=images/rafiq.bmp --out-file=images/liquidated.svdi --compression=3 --method=numpy
 
 svdi decompress --in-file=images/liquidated.svdi --out-file=images/rafiq2.bmp
```

### Comparing `svdi-1.0.0/pyproject.toml` & `svdi-1.0.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "svdi"
-version = "1.0.0"
+version = "1.0.1"
 description = "Image compression and decompression tool using SVD"
 authors = ["Vadim Yakshigulov <toadharvard@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10"
```

### Comparing `svdi-1.0.0/svdi/cli.py` & `svdi-1.0.1/svdi/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from enum import StrEnum, auto
+from enum import Enum
 import os
 import typer
 from pathlib import Path
 from PIL import Image
 
 from svdi.svd import basic_rSVD, numpy_default, pcafast
 from svdi.svd import power_iterations as pi
@@ -12,24 +12,24 @@
 app = typer.Typer(
     no_args_is_help=True,
     help="Image compression and decompression using SVD",
     pretty_exceptions_show_locals=False,
 )
 
 
-class Method(StrEnum):
-    numpy = auto()
-    pi = auto()
-    rSVD = auto()
-    pcafast = auto()
+class Method(str, Enum):
+    numpy = "numpy"
+    pi = "pi"
+    rSVD = "rSVD"
+    pcafast = "pcafast"
 
 
 @app.command(no_args_is_help=True)
 def compress(
-    method: Method = typer.Option(Method.numpy, help="Compression method"),
+    method: Method = typer.Option(Method.numpy, help="Compression method", case_sensitive=False),
     compression: float = typer.Option(2, min=1, help="Compression factor"),
     in_file: Path = typer.Option(..., help="Path to image file"),
     out_file: Path = typer.Option(..., help="Path to .svdi file to be created"),
     power_iterations: int = typer.Option(
         100,
         min=0,
         help="Number of power iterations. Applicable only to rSVD and pcafast methods",
```

### Comparing `svdi-1.0.0/svdi/file/format.py` & `svdi-1.0.1/svdi/file/format.py`

 * *Files identical despite different names*

### Comparing `svdi-1.0.0/svdi/main.py` & `svdi-1.0.1/svdi/main.py`

 * *Files identical despite different names*

### Comparing `svdi-1.0.0/svdi/svd/basic_rSVD.py` & `svdi-1.0.1/svdi/svd/basic_rSVD.py`

 * *Files identical despite different names*

### Comparing `svdi-1.0.0/svdi/svd/pcafast.py` & `svdi-1.0.1/svdi/svd/pcafast.py`

 * *Files identical despite different names*

### Comparing `svdi-1.0.0/svdi/svd/power_iterations.py` & `svdi-1.0.1/svdi/svd/power_iterations.py`

 * *Files identical despite different names*

### Comparing `svdi-1.0.0/PKG-INFO` & `svdi-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svdi
-Version: 1.0.0
+Version: 1.0.1
 Summary: Image compression and decompression tool using SVD
 License: MIT
 Author: Vadim Yakshigulov
 Author-email: toadharvard@gmail.com
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,24 +13,24 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pillow (>=10.3.0,<11.0.0)
 Requires-Dist: scipy (>=1.13.0,<2.0.0)
 Requires-Dist: typer[all] (>=0.12.3,<0.13.0)
 Description-Content-Type: text/markdown
 
-# SVD image compression and decompression tool
+# Image compression and decompression using SVD
 
 ## Installation
 Install CLI using pipx:
 ```bash
 pipx install git+https://github.com/toadharvard/svdi-cli.git
 ```
 Or
 ```bash
-pipx install svdi-cli
+pipx install svdi
 ```
 
 ## Usage example
 ```bash
 svdi compress --in-file=images/rafiq.bmp --out-file=images/liquidated.svdi --compression=3 --method=numpy
 
 svdi decompress --in-file=images/liquidated.svdi --out-file=images/rafiq2.bmp
```

