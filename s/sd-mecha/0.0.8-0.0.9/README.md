# Comparing `tmp/sd-mecha-0.0.8.tar.gz` & `tmp/sd-mecha-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd-mecha-0.0.8.tar", last modified: Sat Mar 16 22:35:55 2024, max compression
+gzip compressed data, was "sd-mecha-0.0.9.tar", last modified: Mon Mar 25 01:45:30 2024, max compression
```

## Comparing `sd-mecha-0.0.8.tar` & `sd-mecha-0.0.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-03-16 22:35:55.382947 sd-mecha-0.0.8/
--rw-rw-rw-   0        0        0     1083 2024-02-13 02:37:42.000000 sd-mecha-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     6700 2024-03-16 22:35:55.382947 sd-mecha-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     6127 2024-03-16 22:29:31.000000 sd-mecha-0.0.8/README.md
--rw-rw-rw-   0        0        0      868 2024-03-16 22:35:28.000000 sd-mecha-0.0.8/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-03-16 22:35:55.361947 sd-mecha-0.0.8/sd_mecha/
--rw-rw-rw-   0        0        0     7994 2024-03-05 08:23:10.000000 sd-mecha-0.0.8/sd_mecha/__init__.py
--rw-rw-rw-   0        0        0     6894 2024-02-28 03:16:46.000000 sd-mecha-0.0.8/sd_mecha/__main__.py
--rw-rw-rw-   0        0        0      253 2024-02-28 03:16:46.000000 sd-mecha-0.0.8/sd_mecha/builtin_model_archs.py
--rw-rw-rw-   0        0        0     3254 2024-03-05 08:23:10.000000 sd-mecha-0.0.8/sd_mecha/builtin_model_types.py
-drwxrwxrwx   0        0        0        0 2024-03-16 22:35:55.378949 sd-mecha-0.0.8/sd_mecha/extensions/
--rw-rw-rw-   0        0        0       52 2024-02-28 03:16:46.000000 sd-mecha-0.0.8/sd_mecha/extensions/__init__.py
--rw-rw-rw-   0        0        0     9126 2024-03-16 22:29:31.000000 sd-mecha-0.0.8/sd_mecha/extensions/merge_method.py
--rw-rw-rw-   0        0        0     4921 2024-02-28 03:16:46.000000 sd-mecha-0.0.8/sd_mecha/extensions/model_arch.py
--rw-rw-rw-   0        0        0     5022 2024-03-05 08:23:10.000000 sd-mecha-0.0.8/sd_mecha/extensions/model_type.py
--rw-rw-rw-   0        0        0     5786 2024-03-05 08:23:10.000000 sd-mecha-0.0.8/sd_mecha/hypers.py
-drwxrwxrwx   0        0        0        0 2024-03-16 22:35:55.379948 sd-mecha-0.0.8/sd_mecha/lora/
--rw-rw-rw-   0        0        0    37233 2024-02-28 03:16:46.000000 sd-mecha-0.0.8/sd_mecha/lora/sd1_ldm_to_lora.json
--rw-rw-rw-   0        0        0    19137 2024-03-16 22:29:52.000000 sd-mecha-0.0.8/sd_mecha/merge_methods.py
--rw-rw-rw-   0        0        0       96 2024-02-28 03:16:46.000000 sd-mecha-0.0.8/sd_mecha/merge_space.py
--rw-rw-rw-   0        0        0     7020 2024-03-05 08:23:10.000000 sd-mecha-0.0.8/sd_mecha/model_detection.py
-drwxrwxrwx   0        0        0        0 2024-03-16 22:35:55.381947 sd-mecha-0.0.8/sd_mecha/models/
--rw-rw-rw-   0        0        0     1089 2024-02-28 03:16:46.000000 sd-mecha-0.0.8/sd_mecha/models/sd1_ldm.yaml
--rw-rw-rw-   0        0        0    74404 2024-02-28 03:16:47.000000 sd-mecha-0.0.8/sd_mecha/models/sd1_ldm_keys.txt
--rw-rw-rw-   0        0        0     1334 2024-02-28 03:16:47.000000 sd-mecha-0.0.8/sd_mecha/models/sdxl_sgm.yaml
--rw-rw-rw-   0        0        0   182143 2024-02-28 03:16:47.000000 sd-mecha-0.0.8/sd_mecha/models/sdxl_sgm_keys.txt
--rw-rw-rw-   0        0        0     7908 2024-03-05 08:23:10.000000 sd-mecha-0.0.8/sd_mecha/recipe_merger.py
--rw-rw-rw-   0        0        0     5990 2024-03-05 08:23:10.000000 sd-mecha-0.0.8/sd_mecha/recipe_nodes.py
--rw-rw-rw-   0        0        0     6472 2024-03-16 22:29:52.000000 sd-mecha-0.0.8/sd_mecha/recipe_serializer.py
--rw-rw-rw-   0        0        0    10302 2024-02-28 03:16:47.000000 sd-mecha-0.0.8/sd_mecha/streaming.py
--rw-rw-rw-   0        0        0       39 2024-02-17 22:56:26.000000 sd-mecha-0.0.8/sd_mecha/user_error.py
-drwxrwxrwx   0        0        0        0 2024-03-16 22:35:55.382947 sd-mecha-0.0.8/sd_mecha.egg-info/
--rw-rw-rw-   0        0        0     6700 2024-03-16 22:35:55.000000 sd-mecha-0.0.8/sd_mecha.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      817 2024-03-16 22:35:55.000000 sd-mecha-0.0.8/sd_mecha.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-16 22:35:55.000000 sd-mecha-0.0.8/sd_mecha.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-03-16 22:35:55.000000 sd-mecha-0.0.8/sd_mecha.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-16 22:35:55.000000 sd-mecha-0.0.8/sd_mecha.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-16 22:35:55.383946 sd-mecha-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-03-25 01:45:30.223717 sd-mecha-0.0.9/
+-rw-rw-rw-   0        0        0     1083 2024-02-13 02:37:42.000000 sd-mecha-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     6700 2024-03-25 01:45:30.223717 sd-mecha-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6127 2024-03-25 01:35:54.000000 sd-mecha-0.0.9/README.md
+-rw-rw-rw-   0        0        0      868 2024-03-25 01:45:14.000000 sd-mecha-0.0.9/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-03-25 01:45:30.207716 sd-mecha-0.0.9/sd_mecha/
+-rw-rw-rw-   0        0        0     7994 2024-03-05 08:23:10.000000 sd-mecha-0.0.9/sd_mecha/__init__.py
+-rw-rw-rw-   0        0        0     6894 2024-02-28 03:16:46.000000 sd-mecha-0.0.9/sd_mecha/__main__.py
+-rw-rw-rw-   0        0        0      253 2024-02-28 03:16:46.000000 sd-mecha-0.0.9/sd_mecha/builtin_model_archs.py
+-rw-rw-rw-   0        0        0     3254 2024-03-25 01:35:54.000000 sd-mecha-0.0.9/sd_mecha/builtin_model_types.py
+drwxrwxrwx   0        0        0        0 2024-03-25 01:45:30.219716 sd-mecha-0.0.9/sd_mecha/extensions/
+-rw-rw-rw-   0        0        0       52 2024-02-28 03:16:46.000000 sd-mecha-0.0.9/sd_mecha/extensions/__init__.py
+-rw-rw-rw-   0        0        0     9126 2024-03-25 01:35:54.000000 sd-mecha-0.0.9/sd_mecha/extensions/merge_method.py
+-rw-rw-rw-   0        0        0     4921 2024-03-25 01:35:54.000000 sd-mecha-0.0.9/sd_mecha/extensions/model_arch.py
+-rw-rw-rw-   0        0        0     5022 2024-03-05 08:23:10.000000 sd-mecha-0.0.9/sd_mecha/extensions/model_type.py
+-rw-rw-rw-   0        0        0     5786 2024-03-25 01:35:54.000000 sd-mecha-0.0.9/sd_mecha/hypers.py
+drwxrwxrwx   0        0        0        0 2024-03-25 01:45:30.219716 sd-mecha-0.0.9/sd_mecha/lora/
+-rw-rw-rw-   0        0        0    37233 2024-02-28 03:16:46.000000 sd-mecha-0.0.9/sd_mecha/lora/sd1_ldm_to_lora.json
+-rw-rw-rw-   0        0        0    19137 2024-03-22 14:32:59.000000 sd-mecha-0.0.9/sd_mecha/merge_methods.py
+-rw-rw-rw-   0        0        0       96 2024-02-28 03:16:46.000000 sd-mecha-0.0.9/sd_mecha/merge_space.py
+-rw-rw-rw-   0        0        0     7020 2024-03-05 08:23:10.000000 sd-mecha-0.0.9/sd_mecha/model_detection.py
+drwxrwxrwx   0        0        0        0 2024-03-25 01:45:30.222716 sd-mecha-0.0.9/sd_mecha/models/
+-rw-rw-rw-   0        0        0     1089 2024-02-28 03:16:46.000000 sd-mecha-0.0.9/sd_mecha/models/sd1_ldm.yaml
+-rw-rw-rw-   0        0        0    74404 2024-02-28 03:16:47.000000 sd-mecha-0.0.9/sd_mecha/models/sd1_ldm_keys.txt
+-rw-rw-rw-   0        0        0     1331 2024-03-25 01:35:57.000000 sd-mecha-0.0.9/sd_mecha/models/sdxl_sgm.yaml
+-rw-rw-rw-   0        0        0   182143 2024-02-28 03:16:47.000000 sd-mecha-0.0.9/sd_mecha/models/sdxl_sgm_keys.txt
+-rw-rw-rw-   0        0        0     7908 2024-03-05 08:23:10.000000 sd-mecha-0.0.9/sd_mecha/recipe_merger.py
+-rw-rw-rw-   0        0        0     5990 2024-03-05 08:23:10.000000 sd-mecha-0.0.9/sd_mecha/recipe_nodes.py
+-rw-rw-rw-   0        0        0     6472 2024-03-25 01:35:54.000000 sd-mecha-0.0.9/sd_mecha/recipe_serializer.py
+-rw-rw-rw-   0        0        0    10302 2024-02-28 03:16:47.000000 sd-mecha-0.0.9/sd_mecha/streaming.py
+-rw-rw-rw-   0        0        0       39 2024-02-17 22:56:26.000000 sd-mecha-0.0.9/sd_mecha/user_error.py
+drwxrwxrwx   0        0        0        0 2024-03-25 01:45:30.222716 sd-mecha-0.0.9/sd_mecha.egg-info/
+-rw-rw-rw-   0        0        0     6700 2024-03-25 01:45:30.000000 sd-mecha-0.0.9/sd_mecha.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      817 2024-03-25 01:45:30.000000 sd-mecha-0.0.9/sd_mecha.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-25 01:45:30.000000 sd-mecha-0.0.9/sd_mecha.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-03-25 01:45:30.000000 sd-mecha-0.0.9/sd_mecha.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-03-25 01:45:30.000000 sd-mecha-0.0.9/sd_mecha.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-03-25 01:45:30.223717 sd-mecha-0.0.9/setup.cfg
```

### Comparing `sd-mecha-0.0.8/LICENSE` & `sd-mecha-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sd-mecha-0.0.8/PKG-INFO` & `sd-mecha-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd-mecha
-Version: 0.0.8
+Version: 0.0.9
 Summary: Stable Diffusion recipe merger
 Author: ljleb
 Project-URL: Homepage, https://github.com/ljleb/sd-mecha
 Project-URL: Issues, https://github.com/ljleb/sd-mecha/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

### Comparing `sd-mecha-0.0.8/README.md` & `sd-mecha-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sd-mecha-0.0.8/pyproject.toml` & `sd-mecha-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sd-mecha"
-version = "0.0.8"
+version = "0.0.9"
 description = "Stable Diffusion recipe merger"
 readme = "README.md"
 authors = [{ name = "ljleb" }]
 requires-python = ">=3.10"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

### Comparing `sd-mecha-0.0.8/sd_mecha/__init__.py` & `sd-mecha-0.0.9/sd_mecha/__init__.py`

 * *Files identical despite different names*

### Comparing `sd-mecha-0.0.8/sd_mecha/__main__.py` & `sd-mecha-0.0.9/sd_mecha/__main__.py`

 * *Files identical despite different names*

### Comparing `sd-mecha-0.0.8/sd_mecha/builtin_model_types.py` & `sd-mecha-0.0.9/sd_mecha/builtin_model_types.py`

 * *Files identical despite different names*

### Comparing `sd-mecha-0.0.8/sd_mecha/extensions/merge_method.py` & `sd-mecha-0.0.9/sd_mecha/extensions/merge_method.py`

 * *Files identical despite different names*

### Comparing `sd-mecha-0.0.8/sd_mecha/extensions/model_arch.py` & `sd-mecha-0.0.9/sd_mecha/extensions/model_arch.py`

 * *Files identical despite different names*

### Comparing `sd-mecha-0.0.8/sd_mecha/extensions/model_type.py` & `sd-mecha-0.0.9/sd_mecha/extensions/model_type.py`

 * *Files identical despite different names*

### Comparing `sd-mecha-0.0.8/sd_mecha/hypers.py` & `sd-mecha-0.0.9/sd_mecha/hypers.py`

 * *Files identical despite different names*

### Comparing `sd-mecha-0.0.8/sd_mecha/lora/sd1_ldm_to_lora.json` & `sd-mecha-0.0.9/sd_mecha/lora/sd1_ldm_to_lora.json`

 * *Files identical despite different names*

### Comparing `sd-mecha-0.0.8/sd_mecha/merge_methods.py` & `sd-mecha-0.0.9/sd_mecha/merge_methods.py`

 * *Files identical despite different names*

### Comparing `sd-mecha-0.0.8/sd_mecha/model_detection.py` & `sd-mecha-0.0.9/sd_mecha/model_detection.py`

 * *Files identical despite different names*

### Comparing `sd-mecha-0.0.8/sd_mecha/models/sd1_ldm.yaml` & `sd-mecha-0.0.9/sd_mecha/models/sd1_ldm.yaml`

 * *Files identical despite different names*

### Comparing `sd-mecha-0.0.8/sd_mecha/models/sd1_ldm_keys.txt` & `sd-mecha-0.0.9/sd_mecha/models/sd1_ldm_keys.txt`

 * *Files identical despite different names*

### Comparing `sd-mecha-0.0.8/sd_mecha/models/sdxl_sgm.yaml` & `sd-mecha-0.0.9/sd_mecha/models/sdxl_sgm.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,17 @@
       in6:
       - input_blocks.6.#
       - input_blocks.6.#.transformer_blocks.#
       mid:
       - middle_block.#
       - middle_block.#.transformer_blocks.#
       - time_embed
-      out11:
-      - output_blocks.11.#
-      - output_blocks.11.#.transformer_blocks.#
+      out8:
+      - output_blocks.8.#
+      - output_blocks.8.#.transformer_blocks.#
       - time_embed
       - out
       in*:
       - input_blocks.*.#
       - input_blocks.*.#.transformer_blocks.#
       - time_embed
       out*:
```

### Comparing `sd-mecha-0.0.8/sd_mecha/models/sdxl_sgm_keys.txt` & `sd-mecha-0.0.9/sd_mecha/models/sdxl_sgm_keys.txt`

 * *Files identical despite different names*

### Comparing `sd-mecha-0.0.8/sd_mecha/recipe_merger.py` & `sd-mecha-0.0.9/sd_mecha/recipe_merger.py`

 * *Files identical despite different names*

### Comparing `sd-mecha-0.0.8/sd_mecha/recipe_nodes.py` & `sd-mecha-0.0.9/sd_mecha/recipe_nodes.py`

 * *Files identical despite different names*

### Comparing `sd-mecha-0.0.8/sd_mecha/recipe_serializer.py` & `sd-mecha-0.0.9/sd_mecha/recipe_serializer.py`

 * *Files identical despite different names*

### Comparing `sd-mecha-0.0.8/sd_mecha/streaming.py` & `sd-mecha-0.0.9/sd_mecha/streaming.py`

 * *Files identical despite different names*

### Comparing `sd-mecha-0.0.8/sd_mecha.egg-info/PKG-INFO` & `sd-mecha-0.0.9/sd_mecha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd-mecha
-Version: 0.0.8
+Version: 0.0.9
 Summary: Stable Diffusion recipe merger
 Author: ljleb
 Project-URL: Homepage, https://github.com/ljleb/sd-mecha
 Project-URL: Issues, https://github.com/ljleb/sd-mecha/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

### Comparing `sd-mecha-0.0.8/sd_mecha.egg-info/SOURCES.txt` & `sd-mecha-0.0.9/sd_mecha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

