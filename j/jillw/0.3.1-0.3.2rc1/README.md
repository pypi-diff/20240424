# Comparing `tmp/jillw-0.3.1.tar.gz` & `tmp/jillw-0.3.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jillw-0.3.1.tar", max compression
+gzip compressed data, was "jillw-0.3.2rc1.tar", max compression
```

## Comparing `jillw-0.3.1.tar` & `jillw-0.3.2rc1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2517 2023-11-13 05:08:16.419996 jillw-0.3.1/jillw/__init__.py
--rw-r--r--   0        0        0     3935 2023-11-13 05:09:40.532758 jillw-0.3.1/jillw/cli.py
--rw-r--r--   0        0        0     3246 2023-11-13 05:08:16.422996 jillw-0.3.1/jillw/configloader.py
--rw-r--r--   0        0        0     1103 2023-11-13 04:07:09.890085 jillw-0.3.1/LICENSE.md
--rw-r--r--   0        0        0      504 2023-11-13 04:43:36.741832 jillw-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2827 2023-11-13 04:07:09.890085 jillw-0.3.1/README.md
--rw-r--r--   0        0        0     3418 1970-01-01 00:00:00.000000 jillw-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1103 2024-04-24 00:34:28.309322 jillw-0.3.2rc1/LICENSE.md
+-rw-r--r--   0        0        0     3446 2024-04-24 00:34:28.309322 jillw-0.3.2rc1/README.md
+-rw-r--r--   0        0        0     2571 2024-04-24 00:34:28.309322 jillw-0.3.2rc1/jillw/__init__.py
+-rw-r--r--   0        0        0     3913 2024-04-24 00:34:28.309322 jillw-0.3.2rc1/jillw/cli.py
+-rw-r--r--   0        0        0     3391 2024-04-24 00:34:28.309322 jillw-0.3.2rc1/jillw/configloader.py
+-rw-r--r--   0        0        0      925 2024-04-24 00:34:28.309322 jillw-0.3.2rc1/pyproject.toml
+-rw-r--r--   0        0        0     4084 1970-01-01 00:00:00.000000 jillw-0.3.2rc1/PKG-INFO
```

### Comparing `jillw-0.3.1/jillw/__init__.py` & `jillw-0.3.2rc1/jillw/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from __future__ import annotations
-import venv
-import wisepy2
-import shutil
+
 import json
+import shutil
 import sys
+import venv
 from pathlib import Path
+from typing import Any, Dict, Union
+
+import wisepy2
 
 root = Path("~/.jlenvs").expanduser()
 
 
 class Ops:
     @staticmethod
-    def get_config(new_conf: "dict | None" = None) -> dict:
+    def get_config(new_conf: "dict | None" = None) -> Union[Dict, Any]:
         root.mkdir(mode=0o755, parents=True, exist_ok=True)
         config_file = root.joinpath("config.json")
         if config_file.exists():
             if new_conf is None:
                 return json.load(config_file.open("r", encoding="utf-8"))
             json.dump(new_conf, config_file.open("w", encoding="utf-8"), indent=4)
             return new_conf
@@ -44,15 +47,15 @@
         install_julia(
             version=version or name,
             install_dir=envdir.joinpath("julia").as_posix(),
             confirm=confirm,
             upstream=upstream,
             unstable=unstable,
             skip_symlinks=True,
-            reinstall=True
+            reinstall=True,
         )
         print(wisepy2.Green(f"Environment {name} created at {envdir.as_posix()}."))
 
     @staticmethod
     def env(name: str):
         Ops.get_config()
         envdir = root.joinpath(name)
```

### Comparing `jillw-0.3.1/jillw/cli.py` & `jillw-0.3.2rc1/jillw/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import annotations
-from jillw import Ops
-from wisepy2 import wise
-from pathlib import Path
-import os
+
 import contextlib
 import io
-import sys
+import os
+import shlex
 import subprocess
+import sys
+from pathlib import Path
+
 import wisepy2
-import shlex
+from wisepy2 import wise
+
+from jillw import Ops
 
 
 def find_julia_binary_dir(env: Path):
     found = next(env.joinpath("julia").iterdir(), None)
     if found is None:
         raise IOError(f"No Julia installation found at {env}")
     return found.joinpath("bin")
@@ -33,19 +36,18 @@
     try:
         with contextlib.redirect_stdout(sio):
             yield
     finally:
         msg = sio.getvalue()
         print(wisepy2.Red(msg))
 
+
 def append_PATH(PATH: str, *paths: Path):
-    return os.pathsep.join([
-        *map(os.path.normpath, paths),
-        *PATH.split(os.pathsep)
-    ])
+    return os.pathsep.join([*map(os.path.normpath, paths), *PATH.split(os.pathsep)])
+
 
 def run_with_activated_env(cmd: list[str]):
     config = Ops.get_config()
     current: str | None = config["current"]
 
     if current is None:
         print(wisepy2.Yellow("No activated environment"))
@@ -63,26 +65,29 @@
     if os.name == "nt":
         envdict = os.environ.copy()
         envdict["VIRTUAL_ENV"] = str(env)
         try:
             del envdict["PYTHONHOME"]
         except KeyError:
             pass
-        envdict['PATH'] = append_PATH(os.environ["PATH"], jlbindir, env, env / "Scripts")
+        envdict["PATH"] = append_PATH(
+            os.environ["PATH"], jlbindir, env, env / "Scripts"
+        )
     else:
         envdict = os.environ.copy()
         envdict["VIRTUAL_ENV"] = str(env)
         try:
             del envdict["PYTHONHOME"]
         except KeyError:
             pass
-        envdict['PATH'] = append_PATH(os.environ["PATH"], jlbindir, env, env / "bin")
+        envdict["PATH"] = append_PATH(os.environ["PATH"], jlbindir, env, env / "bin")
 
     subprocess.run(cmd, env=envdict, shell=False)
 
+
 class Main:
     @staticmethod
     def switch(name: str):
         """Switch to the specified environment"""
         with cmd_session():
             env = Ops.env(name)
             config = Ops.get_config()
@@ -99,46 +104,46 @@
     def create(
         name: str,
         version: str = "",
         upstream: str = "",
         confirm: bool = False,
         unstable: bool = False,
     ):
-        """Create a new Julia environment
-        """
+        """Create a new Julia environment"""
         with cmd_session():
             Ops.create_(name, upstream, version, confirm, unstable)
 
     @staticmethod
     def remove(name: str):
-        """Remove a Julia environment
-        """
+        """Remove a Julia environment"""
         with cmd_session():
             Ops.remove_(name)
 
     @staticmethod
     def list():
-        """List all Julia environments
-        """
+        """List all Julia environments"""
         with cmd_session():
             for each in Ops.list():
                 print(wisepy2.Purple(each.name, "=>", each.as_posix(), sep=" "))
 
     @staticmethod
     def devhere():
-        """Create a Development.toml at the current directory.
-        """
+        """Create a Development.toml at the current directory."""
         with cmd_session():
-            from . configloader import write_empty_config_
+            from .configloader import write_empty_config_
+
             write_empty_config_()
 
+
 def main():
     wise(Main)()
 
+
 def julia():
     extra_options: list[str] = []
 
     if os.environ.get("DEV", "").strip():
         from jillw.configloader import get_options
+
         extra_options = get_options()
 
     run_with_activated_env(["julia", *extra_options, *sys.argv[1:]])
```

### Comparing `jillw-0.3.1/jillw/configloader.py` & `jillw-0.3.2rc1/jillw/configloader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
-import tomli
+
+import json
 import os
 import pathlib
+from typing import Any, List, Union
+
+import tomli
 import wisepy2
-import json
 
-EMPTY_CONFIG = \
-r"""
+EMPTY_CONFIG = r"""
 [julia]
 min-latency = false
 quiet-start = false
 no-startup-file = false
 interactive = true
 
 # activate the specified project
@@ -22,95 +24,106 @@
 # start Julia with loading these modules
 using = []
 
 # start Julia with executing these files
 files = []
 """
 
+
 def get_bool(conf: dict, name: str) -> bool | None:
     if conf.get(name, name):
         var = conf[name]
         if not isinstance(var, bool):
             raise ValueError("'{}' must be a boolean".format(name))
         return var
+    return None
+
 
 def get_int(conf: dict, name: str) -> int | None:
     if conf.get(name, name):
         var = conf[name]
         if not isinstance(var, int):
             raise ValueError("'{}' must be a int".format(name))
         return var
+    return None
+
 
-def get_str_list(conf: dict, name: str) -> list[str] | None:
+def get_str_list(conf: dict, name: str) -> Union[List[str], Any]:
     if conf.get(name, name):
         var = conf[name]
         if not isinstance(var, list) and not (all(isinstance(e, str) for e in var)):
             raise ValueError("'{}' must be a string list".format(name))
         return var
+    return None
+
 
 def get_str(conf: dict, name: str) -> str | None:
     if conf.get(name, name):
         var = conf[name]
         if not isinstance(var, str):
             raise ValueError("'{}' must be a string".format(name))
         return var
+    return None
+
 
 def write_empty_config_():
     cwd = pathlib.Path(os.getcwd())
     dev = cwd / "Development.toml"
     if dev.is_file():
         print(wisepy2.Yellow("Warning: Development.toml already exists"))
         return
     else:
         with dev.open("w", encoding="utf-8") as f:
             f.write(EMPTY_CONFIG)
 
-def get_options() -> list[str]:
+
+def get_options() -> List[str]:
     cwd = pathlib.Path(os.getcwd())
     dev = cwd / "Development.toml"
     if dev.is_file():
-        io = dev.open('rb')
-        conf = tomli.load(io) # type: ignore
+        io = dev.open("rb")
+        conf = tomli.load(io)
         if not isinstance(conf, dict):
             return []
-        conf = conf.get("julia")
-        if not isinstance(conf, dict):
+        julia_conf = conf.get("julia")
+        if not isinstance(julia_conf, dict):
             return []
     else:
         return []
-    opts: list[str] = []
+    opts: List = []
 
-    if get_bool(conf, 'min-latency'):
+    if get_bool(julia_conf, "min-latency"):
         opts.append("--compile=min")
         opts.append("-O0")
 
-    if project := get_str(conf, "project"):
+    if project := get_str(julia_conf, "project"):
         opts.append("--project={}".format(project))
 
     if get_bool(conf, "interactive"):
         opts.append("-i")
 
-    if get_bool(conf, 'quiet-start'):
+    if get_bool(conf, "quiet-start"):
         opts.append("--quiet")
 
     if sysimage := get_str(conf, "sysimage"):
         opts.append("--sysimage")
         opts.append(sysimage)
 
     if get_bool(conf, "no-startup-file"):
         opts.append("--startup-file=no")
 
-    if preload_modules := get_str_list(conf, 'using'):
+    if preload_modules := get_str_list(conf, "using"):
         for each in preload_modules:
             opts.append("-e")
             opts.append("using {}".format(each))
 
-    if preincluded_files := get_str_list(conf, 'files'):
+    if preincluded_files := get_str_list(conf, "files"):
         for file in preincluded_files:
             opts.append("-e")
             opts.append(
-                'include(' +
-                'raw' +json.dumps(str(cwd / file), ensure_ascii=False) +
-                ')'
+                "include("
+                + "raw"
+                + json.dumps(str(cwd / file), ensure_ascii=False)
+                + ")"
             )
 
     return opts
```

### Comparing `jillw-0.3.1/LICENSE.md` & `jillw-0.3.2rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jillw-0.3.1/README.md` & `jillw-0.3.2rc1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # JILL Wrapper
 
+[![CI](https://github.com/Suzhou-Tongyuan/jillw/actions/workflows/ci.yml/badge.svg)](https://github.com/Suzhou-Tongyuan/jillw/actions/workflows/ci.yml)
+[![codecov](https://codecov.io/gh/Suzhou-Tongyuan/jillw/branch/master/graph/badge.svg)](https://codecov.io/gh/Suzhou-Tongyuan/jillw)
+[![versions](https://img.shields.io/pypi/pyversions/jillw.svg)](https://pypi.org/project/jillw/#history)
+[![pypi](https://img.shields.io/pypi/v/jillw.svg)](https://pypi.org/project/jillw/)
+[![License](https://img.shields.io/badge/License-MIT--Clause-green.svg)](https://github.com/Suzhou-Tongyuan/jillw/blob/main/LICENSE.md)
+
+
 JILL Wrapper (`jillw`) is a lightweight and cross-platform Julia version manager. This work is based on [johnnychen94/jill.py](https://github.com/johnnychen94/jill.py) and [Python venv](https://docs.python.org/3/library/venv.html).
 
 `jillw` targets several different use cases:
 
 1. cross-platform julia installation
 2. cross-platform julia version management (create, switch, remove, etc.)
 3. providing the "one Julia, one Python" installation
```

### Comparing `jillw-0.3.1/PKG-INFO` & `jillw-0.3.2rc1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 Metadata-Version: 2.1
 Name: jillw
-Version: 0.3.1
+Version: 0.3.2rc1
 Summary: The wrapper for jill.py and manage Julia environments with Python virtualenv
 License: MIT
 Author: Suzhou-tongyuan
 Author-email: support@tongyuan.cc
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: jill (>=0.11.1,<0.12.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: wisepy2 (>=1.3,<2.0)
 Description-Content-Type: text/markdown
 
 # JILL Wrapper
 
+[![CI](https://github.com/Suzhou-Tongyuan/jillw/actions/workflows/ci.yml/badge.svg)](https://github.com/Suzhou-Tongyuan/jillw/actions/workflows/ci.yml)
+[![codecov](https://codecov.io/gh/Suzhou-Tongyuan/jillw/branch/master/graph/badge.svg)](https://codecov.io/gh/Suzhou-Tongyuan/jillw)
+[![versions](https://img.shields.io/pypi/pyversions/jillw.svg)](https://pypi.org/project/jillw/#history)
+[![pypi](https://img.shields.io/pypi/v/jillw.svg)](https://pypi.org/project/jillw/)
+[![License](https://img.shields.io/badge/License-MIT--Clause-green.svg)](https://github.com/Suzhou-Tongyuan/jillw/blob/main/LICENSE.md)
+
+
 JILL Wrapper (`jillw`) is a lightweight and cross-platform Julia version manager. This work is based on [johnnychen94/jill.py](https://github.com/johnnychen94/jill.py) and [Python venv](https://docs.python.org/3/library/venv.html).
 
 `jillw` targets several different use cases:
 
 1. cross-platform julia installation
 2. cross-platform julia version management (create, switch, remove, etc.)
 3. providing the "one Julia, one Python" installation
```

