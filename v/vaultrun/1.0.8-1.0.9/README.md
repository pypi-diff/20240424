# Comparing `tmp/vaultrun-1.0.8.tar.gz` & `tmp/vaultrun-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vaultrun-1.0.8.tar", max compression
+gzip compressed data, was "vaultrun-1.0.9.tar", max compression
```

## Comparing `vaultrun-1.0.8.tar` & `vaultrun-1.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      412 2024-01-28 09:48:17.866431 vaultrun-1.0.8/README.md
--rw-r--r--   0        0        0        0 2024-01-28 09:48:17.866431 vaultrun-1.0.8/app/__init__.py
--rw-r--r--   0        0        0     2305 2024-01-28 09:48:17.866431 vaultrun-1.0.8/app/login.py
--rw-r--r--   0        0        0     1814 2024-01-28 09:48:17.866431 vaultrun-1.0.8/app/utils.py
--rw-r--r--   0        0        0     1871 2024-01-28 09:48:17.866431 vaultrun-1.0.8/app/vaultrun.py
--rw-r--r--   0        0        0     1024 2024-01-28 09:48:22.401387 vaultrun-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 vaultrun-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0      412 2024-02-01 14:30:18.564146 vaultrun-1.0.9/README.md
+-rw-r--r--   0        0        0        0 2024-02-01 14:30:18.564146 vaultrun-1.0.9/app/__init__.py
+-rw-r--r--   0        0        0     2305 2024-02-01 14:30:18.564146 vaultrun-1.0.9/app/login.py
+-rw-r--r--   0        0        0     1814 2024-02-01 14:30:18.565146 vaultrun-1.0.9/app/utils.py
+-rw-r--r--   0        0        0     1871 2024-02-01 14:30:18.565146 vaultrun-1.0.9/app/vaultrun.py
+-rw-r--r--   0        0        0     1024 2024-02-01 14:30:23.085126 vaultrun-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 vaultrun-1.0.9/PKG-INFO
```

### Comparing `vaultrun-1.0.8/app/login.py` & `vaultrun-1.0.9/app/login.py`

 * *Files identical despite different names*

### Comparing `vaultrun-1.0.8/app/utils.py` & `vaultrun-1.0.9/app/utils.py`

 * *Files identical despite different names*

### Comparing `vaultrun-1.0.8/app/vaultrun.py` & `vaultrun-1.0.9/app/vaultrun.py`

 * *Files identical despite different names*

### Comparing `vaultrun-1.0.8/pyproject.toml` & `vaultrun-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 output-format = "grouped"
 
 [tool.ruff.format]
 exclude = [".git", ".venv", ".mypy_cache", ".tox", "__pycache__"]
 
 [tool.poetry]
 name = "vaultrun"
-version = "1.0.8"
+version = "1.0.9"
 description = "Rofi/Dmenu to interact with vault."
 authors = ["Meni Yakove", "Ruth Netser"]
 readme = "README.md"
 repository = "https://github.com/RedHatQE/vaultrun"
 
 packages = [
     { include = "app" },
```

### Comparing `vaultrun-1.0.8/PKG-INFO` & `vaultrun-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vaultrun
-Version: 1.0.8
+Version: 1.0.9
 Summary: Rofi/Dmenu to interact with vault.
 Home-page: https://github.com/RedHatQE/vaultrun
 Author: Meni Yakove
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

