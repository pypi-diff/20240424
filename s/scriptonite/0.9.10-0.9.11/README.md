# Comparing `tmp/scriptonite-0.9.10.tar.gz` & `tmp/scriptonite-0.9.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scriptonite-0.9.10.tar", max compression
+gzip compressed data, was "scriptonite-0.9.11.tar", max compression
```

## Comparing `scriptonite-0.9.10.tar` & `scriptonite-0.9.11.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      990 2024-04-23 07:23:07.955150 scriptonite-0.9.10/README.md
--rw-r--r--   0        0        0      549 2024-04-23 07:28:40.165018 scriptonite-0.9.10/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-22 09:43:15.887610 scriptonite-0.9.10/scriptonite/__init__.py
--rw-r--r--   0        0        0     5796 2024-04-22 13:55:09.652200 scriptonite-0.9.10/scriptonite/configuration.py
--rw-r--r--   0        0        0     2605 2024-04-22 13:26:38.591687 scriptonite-0.9.10/scriptonite/logging.py
--rw-r--r--   0        0        0     2080 2024-04-22 13:50:06.718720 scriptonite-0.9.10/scriptonite/utilities.py
--rw-r--r--   0        0        0     1596 1970-01-01 00:00:00.000000 scriptonite-0.9.10/PKG-INFO
+-rw-r--r--   0        0        0     1006 2024-04-24 07:19:42.027260 scriptonite-0.9.11/README.md
+-rw-r--r--   0        0        0      566 2024-04-24 11:07:56.176095 scriptonite-0.9.11/pyproject.toml
+-rw-r--r--   0        0        0      132 2024-04-24 10:20:40.388982 scriptonite-0.9.11/scriptonite/__init__.py
+-rw-r--r--   0        0        0     6681 2024-04-24 09:46:50.049014 scriptonite-0.9.11/scriptonite/configuration.py
+-rw-r--r--   0        0        0     3601 2024-04-24 09:48:01.049660 scriptonite-0.9.11/scriptonite/email.py
+-rw-r--r--   0        0        0     4719 2024-04-24 11:01:25.170127 scriptonite-0.9.11/scriptonite/logging.py
+-rw-r--r--   0        0        0     2144 2024-04-24 09:48:17.236143 scriptonite-0.9.11/scriptonite/utilities.py
+-rw-r--r--   0        0        0     1612 1970-01-01 00:00:00.000000 scriptonite-0.9.11/PKG-INFO
```

### Comparing `scriptonite-0.9.10/README.md` & `scriptonite-0.9.11/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ## SCRIPTONITE
 
-A Python toolkit for scripting
+An opinionated Python toolkit for scripting
 
 ## Introduction
 
 When writing python utilites and CLI scripts there are some parts that need to be implented each time, like
 
 - logging;
 - configuration parsing;
 - other nice to have;
 
-We wrote some standard implementations, that gives enough flexibility, but reduce the effort required to start writing the core parts of our script.
+We wrote some opinionated implementations, that gives enough flexibility, but reduce the effort required to start writing the core parts of our script.
 
 More details on each submodule can be found in the `docs/` directory of the original repository.
 
 ### Install
 
 ```
 pip intall scriptonite
```

### Comparing `scriptonite-0.9.10/pyproject.toml` & `scriptonite-0.9.11/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "scriptonite"
-version = "0.9.10"
+version = "0.9.11"
 description = "A toolkit for scripting in Python"
 authors = ["Andrea Mistrali <andrea@mistrali.pw>"]
 maintainers = ["Andrea Mistrali <andrea@mistrali.pw>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^8.23.0"
 poetry = "^1.8.2"
+pdoc = "^14.4.0"
 
 [tool.pyright]
 reportOptionalSubscript = false
 reportAttributeAccessIssue = false
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `scriptonite-0.9.10/scriptonite/configuration.py` & `scriptonite-0.9.11/scriptonite/configuration.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,25 +26,25 @@
                  env_prefix: str | None = None,
                  configfile: str | None = None,
                  file_loader: t.Callable[[t.IO[t.Any]],
                                          t.Mapping[str, t.Any]] = yaml_load):
         """
         Create a configuration, as a dict.
         Can create it from:
-            - a default dict passed at init;
-            - environment variables, prefixed with a specific string;
-            - a yaml or json file;
-
-        Methods:
-            - from_environ: reads config from environment variables;
-            - from_file: loads and parses a file;
-            - from_mapping: update the dict with a mapping (dict);
-
-            - from_json: calls from_file using json parser;
-            - from_yaml: calls from_file using yaml parser;
+        - a default dict passed at init;
+        - environment variables, prefixed with a specific string;
+        - a yaml or json file;
+
+        Parameters:
+        - **defaults**: a dict of initial values
+        - **env_prefix**: the prefix to use to look up environment variables
+        - **configfile**: a configuration file to read
+        - **file_loader**: the loader to use to parse the config file,
+                       defaults to `yaml_load` function, you can use
+                       `json.load` or `toml.load` to parse other formats
         """
         super().__init__(defaults or {})
 
         if env_prefix:
             self.from_environ(prefix=env_prefix)
 
         if configfile:
@@ -56,14 +56,21 @@
                      loads: t.Callable[[str], t.Any] = json.loads) -> bool:
         """
         Loads configuration parsing environment variables.
         Prefix is the prefix of the variables (that will be stripped).
         Variables can build structures, using `__` as separator
         between the levels.
 
+        Parameters:
+        - **prefix**: the environment prefix
+        - **loads**: a function to parse and normalize environment variables
+                 values, best to use is `json.load` that will convert
+                 numeric values to numbers and string like "true" or "false"
+                 to python boolean
+
         Examples:
             - `PREFIX_ANSWER=42` -> `answer`: 42
             - `PREFIX_A__B=1` -> `{'a': {'b': 1}}`
         """
         prefix = f"{prefix}_"
         len_prefix = len(prefix)
 
@@ -100,24 +107,32 @@
                   load: t.Callable[[t.IO[t.Any]], t.Mapping[str, t.Any]],
                   silent: bool = False,
                   text: bool = True,) -> bool:
         """
         Loads and parses a file, updating the config with the content.
         Wants a `load` method to use to parse the file.
 
-        - `silent`: do not stop if file does not exist;
-        - `text`: open file as text if True, as binary if False
+        Parameters:
+        - **filename**: the file to load
+        - **silent**: do not stop if file does not exist;
+        - **text**: open file as text if True, as binary if False
+        - **load**: a function to parse the file, we have `yaml_load` to load
+                YAML files, you can use `json.load` or `toml.load` to load
+                other formats.
 
         Example:
-            conf.from_file('conf.json', load=json.load)
-        NOTE:
-            to open YAML file, we can use yaml.load, but that requires an extra
-            parameter `Loader`.
-            We have a simple function called `load_yaml` to use,
-            so you can use `conf=c.from_file('config.yaml', load=yaml_load)`
+        ```
+        conf.from_file('conf.json', load=json.load)
+        ```
+
+        **NOTE**:
+        >> to open YAML file, we can use yaml.load, but that requires an extra
+        parameter `Loader`.
+        We have a simple function called `load_yaml` to use,
+        so you can use `conf=c.from_file('config.yaml', load=yaml_load)`
         """
 
         try:
             with open(filename, "r" if text else "rb") as f:
                 obj = load(f)
         except OSError as e:
             if silent and e.errno in (errno.ENOENT, errno.EISDIR):
@@ -129,38 +144,41 @@
 
     def from_yaml(self,
                   filename: str | os.PathLike[str],
                   silent: bool = False,
                   text: bool = True) -> bool:
         """
         Syntax sugar to load a YAML file
+        Parameters are the same as `from_file`, apart for the `load` parameter
+        that is hardcoded to `yaml_load`
         """
         return self.from_file(filename,
                               silent=silent,
                               text=text,
                               load=yaml_load)
 
     def from_json(self,
                   filename: str | os.PathLike[str],
                   silent: bool = False,
                   text: bool = True) -> bool:
         """
         Syntax sugar to load a JSON file
+        Parameters are the same ad `from_file`, apart for the `load` parameter
+        that is hardcoded to `json.load`
         """
         return self.from_file(filename,
                               silent=silent,
                               text=text,
                               load=json.load)
 
     def from_mapping(
         self, mapping: t.Mapping[str, t.Any] | None = None, **kwargs: t.Any
     ) -> bool:
-        """Updates the config like :meth:`update`
-
-        :return: Always returns ``True``.
+        """
+        Updates the config like :meth:`update` of dict object
 
         """
         mappings: dict[str, t.Any] = {}
         if mapping is not None:
             mappings.update(mapping)
         mappings.update(kwargs)
         self.update(mappings)
```

### Comparing `scriptonite-0.9.10/scriptonite/utilities.py` & `scriptonite-0.9.11/scriptonite/utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,23 @@
 """
 from functools import singledispatchmethod
 from typing import Any
 
 
 class dictObj(dict):
     """
-    The usual dict on steroids
+    A dict on steroids
     You can access keys as attributes
+
+    Example:
     c=Config({'a': 1, 'b': 2})
     c.a == c['a'] -> True
+
+    Parameters:
+    - **init**: a dict of initial values
     """
 
     def __init__(self, init: dict | None) -> None:
         if init:
             for key, value in init.items():
                 self.__parse_value(key, value)
```

### Comparing `scriptonite-0.9.10/PKG-INFO` & `scriptonite-0.9.11/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scriptonite
-Version: 0.9.10
+Version: 0.9.11
 Summary: A toolkit for scripting in Python
 License: GPL-3.0-or-later
 Author: Andrea Mistrali
 Author-email: andrea@mistrali.pw
 Maintainer: Andrea Mistrali
 Maintainer-email: andrea@mistrali.pw
 Requires-Python: >=3.10,<4.0
@@ -13,25 +13,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 ## SCRIPTONITE
 
-A Python toolkit for scripting
+An opinionated Python toolkit for scripting
 
 ## Introduction
 
 When writing python utilites and CLI scripts there are some parts that need to be implented each time, like
 
 - logging;
 - configuration parsing;
 - other nice to have;
 
-We wrote some standard implementations, that gives enough flexibility, but reduce the effort required to start writing the core parts of our script.
+We wrote some opinionated implementations, that gives enough flexibility, but reduce the effort required to start writing the core parts of our script.
 
 More details on each submodule can be found in the `docs/` directory of the original repository.
 
 ### Install
 
 ```
 pip intall scriptonite
```

