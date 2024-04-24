# Comparing `tmp/pyqqq_cli-0.2.6.tar.gz` & `tmp/pyqqq_cli-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq_cli-0.2.6.tar", max compression
+gzip compressed data, was "pyqqq_cli-0.2.7.tar", max compression
```

## Comparing `pyqqq_cli-0.2.6.tar` & `pyqqq_cli-0.2.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      937 2024-03-26 03:56:47.680900 pyqqq_cli-0.2.6/README.md
--rw-r--r--   0        0        0      655 2024-04-22 08:16:49.081048 pyqqq_cli-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      358 2024-04-12 09:23:39.993237 pyqqq_cli-0.2.6/qupiato/cli/config.py
--rw-r--r--   0        0        0     8659 2024-04-22 08:15:00.066397 pyqqq_cli-0.2.6/qupiato/cli/main.py
--rw-r--r--   0        0        0     5675 2024-04-22 08:12:36.529460 pyqqq_cli-0.2.6/qupiato/cli/utils.py
--rw-r--r--   0        0        0     1809 1970-01-01 00:00:00.000000 pyqqq_cli-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-24 00:29:15.273727 pyqqq_cli-0.2.7/README.md
+-rw-r--r--   0        0        0      655 2024-04-24 00:29:44.448434 pyqqq_cli-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      358 2024-03-29 03:28:42.002454 pyqqq_cli-0.2.7/qupiato/cli/config.py
+-rw-r--r--   0        0        0     8659 2024-04-24 00:29:15.274392 pyqqq_cli-0.2.7/qupiato/cli/main.py
+-rw-r--r--   0        0        0     5675 2024-04-24 00:29:15.274530 pyqqq_cli-0.2.7/qupiato/cli/utils.py
+-rw-r--r--   0        0        0     1936 1970-01-01 00:00:00.000000 pyqqq_cli-0.2.7/PKG-INFO
```

### Comparing `pyqqq_cli-0.2.6/README.md` & `pyqqq_cli-0.2.7/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 
 #### Commands
 
 - `deploy`: Deploy a strategy.
 - `delete`: Delete a deployed strategy.
 - `list`: List deployed strategies.
 - `logs`: Show logs of a deployed strategy.
+- `pull`: Download an strategy from the registry.
+- `run`: Run a strategy.
+- `search`: Search for stock investment strategies.
 - `version`: Show version number and quit.
 
 ### Example
 
 ```bash
 qqq deploy my_strategy_name
 ```
```

### Comparing `pyqqq_cli-0.2.6/pyproject.toml` & `pyqqq_cli-0.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "pyqqq-cli"
-version = "0.2.6"
+version = "0.2.7"
 description = "CLI tool for controlling strategies deployed on the PyQQQ platform."
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "qupiato"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.1.7"
 websockets = "^12.0"
 python-dotenv = "^1.0.1"
 requests = "^2.31.0"
-pyqqq = "^0.8.0"
+pyqqq = "^0.8.7"
 pyyaml = "^6.0.1"
 
 [tool.poetry.scripts]
 qqq = 'qupiato.cli.main:main'
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `pyqqq_cli-0.2.6/qupiato/cli/main.py` & `pyqqq_cli-0.2.7/qupiato/cli/main.py`

 * *Files identical despite different names*

### Comparing `pyqqq_cli-0.2.6/qupiato/cli/utils.py` & `pyqqq_cli-0.2.7/qupiato/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pyqqq_cli-0.2.6/PKG-INFO` & `pyqqq_cli-0.2.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pyqqq-cli
-Version: 0.2.6
+Version: 0.2.7
 Summary: CLI tool for controlling strategies deployed on the PyQQQ platform.
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: pyqqq (>=0.8.0,<0.9.0)
+Requires-Dist: pyqqq (>=0.8.7,<0.9.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: websockets (>=12.0,<13.0)
 Project-URL: Documentation, https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io
 Description-Content-Type: text/markdown
 
@@ -44,14 +44,17 @@
 
 #### Commands
 
 - `deploy`: Deploy a strategy.
 - `delete`: Delete a deployed strategy.
 - `list`: List deployed strategies.
 - `logs`: Show logs of a deployed strategy.
+- `pull`: Download an strategy from the registry.
+- `run`: Run a strategy.
+- `search`: Search for stock investment strategies.
 - `version`: Show version number and quit.
 
 ### Example
 
 ```bash
 qqq deploy my_strategy_name
 ```
```

