# Comparing `tmp/diffedit-0.0.2rc1.tar.gz` & `tmp/diffedit-0.0.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffedit-0.0.2rc1.tar", max compression
+gzip compressed data, was "diffedit-0.0.2rc2.tar", max compression
```

## Comparing `diffedit-0.0.2rc1.tar` & `diffedit-0.0.2rc2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11357 2024-04-24 19:07:57.389129 diffedit-0.0.2rc1/LICENSE
--rw-r--r--   0        0        0     5073 2024-04-24 19:07:57.389129 diffedit-0.0.2rc1/README.md
--rw-r--r--   0        0        0     5088 2024-04-24 19:07:57.389129 diffedit-0.0.2rc1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-24 19:07:57.393129 diffedit-0.0.2rc1/src/diff_edit/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 19:07:57.393129 diffedit-0.0.2rc1/src/diff_edit/model/__init__.py
--rw-r--r--   0        0        0       57 2024-04-24 19:07:57.393129 diffedit-0.0.2rc1/src/diff_edit/model/constants.py
--rw-r--r--   0        0        0    10994 2024-04-24 19:07:57.393129 diffedit-0.0.2rc1/src/diff_edit/model/diff_edit_model.py
--rw-r--r--   0        0        0     2243 2024-04-24 19:07:57.393129 diffedit-0.0.2rc1/src/diff_edit/model/image_processing.py
--rw-r--r--   0        0        0     8789 2024-04-24 19:07:57.393129 diffedit-0.0.2rc1/src/diff_edit/model/mask_generation.py
--rw-r--r--   0        0        0      852 2024-04-24 19:07:57.393129 diffedit-0.0.2rc1/src/diff_edit/model/mask_inpainting.py
--rw-r--r--   0        0        0     3833 2024-04-24 19:07:57.393129 diffedit-0.0.2rc1/src/diff_edit/model/model_composer.py
--rw-r--r--   0        0        0     7551 2024-04-24 19:07:57.393129 diffedit-0.0.2rc1/src/diff_edit/scripts/image_edit.py
--rw-r--r--   0        0        0   434756 2024-04-24 19:07:57.393129 diffedit-0.0.2rc1/src/diff_edit/scripts/mask.png
--rw-r--r--   0        0        0   491401 2024-04-24 19:07:57.393129 diffedit-0.0.2rc1/src/diff_edit/scripts/result.png
--rw-r--r--   0        0        0     6576 1970-01-01 00:00:00.000000 diffedit-0.0.2rc1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-24 19:12:49.942078 diffedit-0.0.2rc2/LICENSE
+-rw-r--r--   0        0        0     5073 2024-04-24 19:12:49.942078 diffedit-0.0.2rc2/README.md
+-rw-r--r--   0        0        0     5088 2024-04-24 19:12:49.946078 diffedit-0.0.2rc2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-24 19:12:49.946078 diffedit-0.0.2rc2/src/diff_edit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 19:12:49.946078 diffedit-0.0.2rc2/src/diff_edit/model/__init__.py
+-rw-r--r--   0        0        0       57 2024-04-24 19:12:49.946078 diffedit-0.0.2rc2/src/diff_edit/model/constants.py
+-rw-r--r--   0        0        0    10994 2024-04-24 19:12:49.946078 diffedit-0.0.2rc2/src/diff_edit/model/diff_edit_model.py
+-rw-r--r--   0        0        0     2243 2024-04-24 19:12:49.946078 diffedit-0.0.2rc2/src/diff_edit/model/image_processing.py
+-rw-r--r--   0        0        0     8789 2024-04-24 19:12:49.946078 diffedit-0.0.2rc2/src/diff_edit/model/mask_generation.py
+-rw-r--r--   0        0        0      852 2024-04-24 19:12:49.946078 diffedit-0.0.2rc2/src/diff_edit/model/mask_inpainting.py
+-rw-r--r--   0        0        0     3833 2024-04-24 19:12:49.946078 diffedit-0.0.2rc2/src/diff_edit/model/model_composer.py
+-rw-r--r--   0        0        0     7551 2024-04-24 19:12:49.946078 diffedit-0.0.2rc2/src/diff_edit/scripts/image_edit.py
+-rw-r--r--   0        0        0   434756 2024-04-24 19:12:49.946078 diffedit-0.0.2rc2/src/diff_edit/scripts/mask.png
+-rw-r--r--   0        0        0   491401 2024-04-24 19:12:49.946078 diffedit-0.0.2rc2/src/diff_edit/scripts/result.png
+-rw-r--r--   0        0        0     6576 1970-01-01 00:00:00.000000 diffedit-0.0.2rc2/PKG-INFO
```

### Comparing `diffedit-0.0.2rc1/LICENSE` & `diffedit-0.0.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc1/README.md` & `diffedit-0.0.2rc2/README.md`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc1/pyproject.toml` & `diffedit-0.0.2rc2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "DiffEdit"
 # version_pattern = "MAJOR.MINOR.PATCH"
-version = "0.0.2rc1"
+version = "0.0.2rc2"
 description = "An implementation of the DiffEdit algorithm for prompt-based mask creation and inpating. For more information, see the Readme file."
 authors = ["Gennaro Farina"]
 readme = "README.md"
 packages = [
     { include = "diff_edit", from = "src" },
 ]
 license = "Apache-2.0"
```

### Comparing `diffedit-0.0.2rc1/src/diff_edit/model/diff_edit_model.py` & `diffedit-0.0.2rc2/src/diff_edit/model/diff_edit_model.py`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc1/src/diff_edit/model/image_processing.py` & `diffedit-0.0.2rc2/src/diff_edit/model/image_processing.py`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc1/src/diff_edit/model/mask_generation.py` & `diffedit-0.0.2rc2/src/diff_edit/model/mask_generation.py`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc1/src/diff_edit/model/mask_inpainting.py` & `diffedit-0.0.2rc2/src/diff_edit/model/mask_inpainting.py`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc1/src/diff_edit/model/model_composer.py` & `diffedit-0.0.2rc2/src/diff_edit/model/model_composer.py`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc1/src/diff_edit/scripts/image_edit.py` & `diffedit-0.0.2rc2/src/diff_edit/scripts/image_edit.py`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc1/src/diff_edit/scripts/mask.png` & `diffedit-0.0.2rc2/src/diff_edit/scripts/mask.png`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc1/src/diff_edit/scripts/result.png` & `diffedit-0.0.2rc2/src/diff_edit/scripts/result.png`

 * *Files identical despite different names*

### Comparing `diffedit-0.0.2rc1/PKG-INFO` & `diffedit-0.0.2rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DiffEdit
-Version: 0.0.2rc1
+Version: 0.0.2rc2
 Summary: An implementation of the DiffEdit algorithm for prompt-based mask creation and inpating. For more information, see the Readme file.
 License: Apache-2.0
 Author: Gennaro Farina
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: DiffEdit Version: 0.0.2rc1 Summary: An
+Metadata-Version: 2.1 Name: DiffEdit Version: 0.0.2rc2 Summary: An
 implementation of the DiffEdit algorithm for prompt-based mask creation and
 inpating. For more information, see the Readme file. License: Apache-2.0
 Author: Gennaro Farina Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: dev Provides-Extra: test Requires-Dist: accelerate (==0.26.1)
```

