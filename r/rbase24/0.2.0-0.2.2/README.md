# Comparing `tmp/rbase24-0.2.0.tar.gz` & `tmp/rbase24-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rbase24-0.2.0.tar", last modified: Tue Apr 23 08:37:04 2024, max compression
+gzip compressed data, was "rbase24-0.2.2.tar", last modified: Wed Apr 24 17:34:54 2024, max compression
```

## Comparing `rbase24-0.2.0.tar` & `rbase24-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     1047 2024-04-23 08:36:57.386175 rbase24-0.2.0/README.md
--rw-r--r--   0        0        0      882 2024-04-23 08:37:04.790211 rbase24-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-23 08:36:57.390175 rbase24-0.2.0/src/rbase24/__init__.py
--rw-r--r--   0        0        0       87 2024-04-23 08:36:57.390175 rbase24-0.2.0/src/rbase24/__main__.py
--rw-r--r--   0        0        0     2128 2024-04-23 08:36:57.390175 rbase24-0.2.0/src/rbase24/cli.py
--rw-r--r--   0        0        0     1813 2024-04-23 08:36:57.390175 rbase24-0.2.0/src/rbase24/color.py
--rw-r--r--   0        0        0     2030 2024-04-23 08:36:57.390175 rbase24-0.2.0/src/rbase24/config.py
--rw-r--r--   0        0        0     1931 2024-04-23 08:36:57.390175 rbase24-0.2.0/src/rbase24/scheme.py
--rw-r--r--   0        0        0      858 2024-04-23 08:36:57.390175 rbase24-0.2.0/src/rbase24/typedefs.py
--rw-r--r--   0        0        0        0 2024-04-23 08:36:57.390175 rbase24-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0       31 2024-04-23 08:36:57.390175 rbase24-0.2.0/tests/config.ini
--rwxr-xr-x   0        0        0      573 2024-04-23 08:36:57.390175 rbase24-0.2.0/tests/schemes/base16/gruvbox-dark-hard.yaml
--rwxr-xr-x   0        0        0      575 2024-04-23 08:36:57.390175 rbase24-0.2.0/tests/schemes/base16/gruvbox-light-hard.yaml
--rwxr-xr-x   0        0        0      500 2024-04-23 08:36:57.390175 rbase24-0.2.0/tests/schemes/base16/gruvbox-material-dark-hard.yaml
--rwxr-xr-x   0        0        0      504 2024-04-23 08:36:57.390175 rbase24-0.2.0/tests/schemes/base16/gruvbox-material-light-medium.yaml
--rwxr-xr-x   0        0        0      425 2024-04-23 08:36:57.390175 rbase24-0.2.0/tests/schemes/base16/horizon-dark.yaml
--rwxr-xr-x   0        0        0      427 2024-04-23 08:36:57.390175 rbase24-0.2.0/tests/schemes/base16/horizon-light.yaml
--rwxr-xr-x   0        0        0      434 2024-04-23 08:36:57.390175 rbase24-0.2.0/tests/schemes/base16/horizon-terminal-dark.yaml
--rwxr-xr-x   0        0        0      436 2024-04-23 08:36:57.390175 rbase24-0.2.0/tests/schemes/base16/horizon-terminal-light.yaml
--rw-r--r--   0        0        0      576 2024-04-23 08:36:57.390175 rbase24-0.2.0/tests/schemes/base24/brogrammer.yaml
--rw-r--r--   0        0        0      886 2024-04-23 08:36:57.390175 rbase24-0.2.0/tests/test_config.py
--rw-r--r--   0        0        0     1016 2024-04-23 08:36:57.390175 rbase24-0.2.0/tests/test_scheme.py
--rw-r--r--   0        0        0     1394 1970-01-01 00:00:00.000000 rbase24-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-24 17:34:44.212158 rbase24-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1137 2024-04-24 17:34:44.212158 rbase24-0.2.2/README.md
+-rw-r--r--   0        0        0      895 2024-04-24 17:34:54.552082 rbase24-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-24 17:34:44.212158 rbase24-0.2.2/src/rbase24/__init__.py
+-rw-r--r--   0        0        0       87 2024-04-24 17:34:44.212158 rbase24-0.2.2/src/rbase24/__main__.py
+-rw-r--r--   0        0        0     2128 2024-04-24 17:34:44.212158 rbase24-0.2.2/src/rbase24/cli.py
+-rw-r--r--   0        0        0     1813 2024-04-24 17:34:44.212158 rbase24-0.2.2/src/rbase24/color.py
+-rw-r--r--   0        0        0     2073 2024-04-24 17:34:44.212158 rbase24-0.2.2/src/rbase24/config.py
+-rw-r--r--   0        0        0     1931 2024-04-24 17:34:44.212158 rbase24-0.2.2/src/rbase24/scheme.py
+-rw-r--r--   0        0        0      858 2024-04-24 17:34:44.212158 rbase24-0.2.2/src/rbase24/typedefs.py
+-rw-r--r--   0        0        0        0 2024-04-24 17:34:44.212158 rbase24-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0       31 2024-04-24 17:34:44.212158 rbase24-0.2.2/tests/config.ini
+-rwxr-xr-x   0        0        0      573 2024-04-24 17:34:44.212158 rbase24-0.2.2/tests/schemes/base16/gruvbox-dark-hard.yaml
+-rwxr-xr-x   0        0        0      575 2024-04-24 17:34:44.212158 rbase24-0.2.2/tests/schemes/base16/gruvbox-light-hard.yaml
+-rwxr-xr-x   0        0        0      500 2024-04-24 17:34:44.212158 rbase24-0.2.2/tests/schemes/base16/gruvbox-material-dark-hard.yaml
+-rwxr-xr-x   0        0        0      504 2024-04-24 17:34:44.212158 rbase24-0.2.2/tests/schemes/base16/gruvbox-material-light-medium.yaml
+-rwxr-xr-x   0        0        0      425 2024-04-24 17:34:44.212158 rbase24-0.2.2/tests/schemes/base16/horizon-dark.yaml
+-rwxr-xr-x   0        0        0      427 2024-04-24 17:34:44.216158 rbase24-0.2.2/tests/schemes/base16/horizon-light.yaml
+-rwxr-xr-x   0        0        0      434 2024-04-24 17:34:44.216158 rbase24-0.2.2/tests/schemes/base16/horizon-terminal-dark.yaml
+-rwxr-xr-x   0        0        0      436 2024-04-24 17:34:44.216158 rbase24-0.2.2/tests/schemes/base16/horizon-terminal-light.yaml
+-rw-r--r--   0        0        0      576 2024-04-24 17:34:44.216158 rbase24-0.2.2/tests/schemes/base24/brogrammer.yaml
+-rw-r--r--   0        0        0      886 2024-04-24 17:34:44.216158 rbase24-0.2.2/tests/test_config.py
+-rw-r--r--   0        0        0     1016 2024-04-24 17:34:44.216158 rbase24-0.2.2/tests/test_scheme.py
+-rw-r--r--   0        0        0     1497 1970-01-01 00:00:00.000000 rbase24-0.2.2/PKG-INFO
```

### Comparing `rbase24-0.2.0/pyproject.toml` & `rbase24-0.2.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "rbase24"
-version = "0.2.0"
-description = "base16/base24 terminal viewer"
+version = "0.2.2"
+description = "base16/base24 color scheme terminal viewer"
 authors = [
     { name = "Simon Kennedy", email = "sffjunkie+code@gmail.com" },
 ]
 dependencies = [
     "rich>=13.7.1",
     "pyyaml>=6.0.1",
     "unicode-slugify>=0.1.5",
```

### Comparing `rbase24-0.2.0/src/rbase24/cli.py` & `rbase24-0.2.2/src/rbase24/cli.py`

 * *Files identical despite different names*

### Comparing `rbase24-0.2.0/src/rbase24/color.py` & `rbase24-0.2.2/src/rbase24/color.py`

 * *Files identical despite different names*

### Comparing `rbase24-0.2.0/src/rbase24/config.py` & `rbase24-0.2.2/src/rbase24/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,20 +15,21 @@
         return self._scheme_dir
 
     def _get_scheme_dir(self, config_file: Path | None = None) -> Path:
         scheme_dir = os.environ.get("BASE24_SCHEME_DIR", None)
         if scheme_dir is not None:
             return Path(scheme_dir)
 
-        cfg = None
+        if config_file is None:
+            config_file = Base24ViewerConfig.default_config_path()
+
         try:
-            if config_file is not None:
-                cfg = self._read_config(config_file)
+            cfg = self._read_config(config_file)
         except IOError:
-            pass
+            cfg = None
 
         if cfg is None:
             return Base24ViewerConfig.default_scheme_dir()
 
         scheme_dir = cfg.get("rbase24", "scheme_dir")
         if scheme_dir is not None:
             return Path(scheme_dir)
```

### Comparing `rbase24-0.2.0/src/rbase24/scheme.py` & `rbase24-0.2.2/src/rbase24/scheme.py`

 * *Files identical despite different names*

### Comparing `rbase24-0.2.0/src/rbase24/typedefs.py` & `rbase24-0.2.2/src/rbase24/typedefs.py`

 * *Files identical despite different names*

### Comparing `rbase24-0.2.0/tests/schemes/base16/gruvbox-dark-hard.yaml` & `rbase24-0.2.2/tests/schemes/base16/gruvbox-dark-hard.yaml`

 * *Files identical despite different names*

### Comparing `rbase24-0.2.0/tests/schemes/base16/gruvbox-light-hard.yaml` & `rbase24-0.2.2/tests/schemes/base16/gruvbox-light-hard.yaml`

 * *Files identical despite different names*

### Comparing `rbase24-0.2.0/tests/schemes/base24/brogrammer.yaml` & `rbase24-0.2.2/tests/schemes/base24/brogrammer.yaml`

 * *Files identical despite different names*

### Comparing `rbase24-0.2.0/tests/test_config.py` & `rbase24-0.2.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rbase24-0.2.0/tests/test_scheme.py` & `rbase24-0.2.2/tests/test_scheme.py`

 * *Files identical despite different names*

### Comparing `rbase24-0.2.0/PKG-INFO` & `rbase24-0.2.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: rbase24
-Version: 0.2.0
-Summary: base16/base24 terminal viewer
+Version: 0.2.2
+Summary: base16/base24 color scheme terminal viewer
 Author-Email: Simon Kennedy <sffjunkie+code@gmail.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: rich>=13.7.1
 Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: unicode-slugify>=0.1.5
 Requires-Dist: typer>=0.12.3
@@ -13,30 +13,34 @@
 
 # rbase24
 
 A command line tool to print base16/base24 color schemes to the terminal.
 
 Best installed using [`pipx`](https://pypi.org/project/pipx/) or your Python installer of choice.
 
+```sh
+pipx install rbase24
+```
+
 To specify the location of the color scheme files either...
 
 1. Set the `BASE24_SCHEME_DIR` environment variable to point to the directory
    containing the scheme files.
 2. Create a `config.ini` file in `$HOME/.config/rbase24` with a single entry
-   
+
    ```ini
    [rbase24]
    scheme_dir = "<scheme file directory>"
    ```
 
 Run the `rbase24` command passing an optional filespec to filter the list of
 files.
 
 The filespec will have `*` and `.yaml` added if necessary so
-`gruvbox`, `gruvbox*` and `gruvbox*.yaml` mean the same.
+`gruvbox`, `gruvbox*` and `gruvbox*.yaml` will find the same schemes. Schemes are searhced for in all subdirectories.
 
 ```bash
 rbase24 primer
 ```
 
 Displays the following
```

