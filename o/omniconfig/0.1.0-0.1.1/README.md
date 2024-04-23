# Comparing `tmp/omniconfig-0.1.0.tar.gz` & `tmp/omniconfig-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniconfig-0.1.0.tar", max compression
+gzip compressed data, was "omniconfig-0.1.1.tar", max compression
```

## Comparing `omniconfig-0.1.0.tar` & `omniconfig-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    34523 2024-04-22 18:56:40.046281 omniconfig-0.1.0/LICENSE
--rw-r--r--   0        0        0     6488 2024-04-23 22:52:57.920077 omniconfig-0.1.0/README.md
--rw-r--r--   0        0        0      371 2024-04-22 18:56:55.342364 omniconfig-0.1.0/omniconfig/__init__.py
--rw-r--r--   0        0        0    17446 2024-04-22 19:39:16.088184 omniconfig-0.1.0/omniconfig/args.py
--rw-r--r--   0        0        0    13422 2024-04-23 21:56:49.634348 omniconfig-0.1.0/omniconfig/configclass.py
--rw-r--r--   0        0        0    10024 2024-04-22 19:43:02.785418 omniconfig-0.1.0/omniconfig/parser.py
--rw-r--r--   0        0        0     6474 2024-04-23 22:16:21.488513 omniconfig-0.1.0/omniconfig/utils.py
--rw-r--r--   0        0        0       90 2024-04-22 18:56:55.354364 omniconfig-0.1.0/omniconfig/version.py
--rw-r--r--   0        0        0      858 2024-04-23 23:15:04.879061 omniconfig-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7137 1970-01-01 00:00:00.000000 omniconfig-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-22 18:56:40.046281 omniconfig-0.1.1/LICENSE
+-rw-r--r--   0        0        0     6476 2024-04-23 23:25:40.582406 omniconfig-0.1.1/README.md
+-rw-r--r--   0        0        0      371 2024-04-22 18:56:55.342364 omniconfig-0.1.1/omniconfig/__init__.py
+-rw-r--r--   0        0        0    17446 2024-04-22 19:39:16.088184 omniconfig-0.1.1/omniconfig/args.py
+-rw-r--r--   0        0        0    13422 2024-04-23 21:56:49.634348 omniconfig-0.1.1/omniconfig/configclass.py
+-rw-r--r--   0        0        0    10024 2024-04-22 19:43:02.785418 omniconfig-0.1.1/omniconfig/parser.py
+-rw-r--r--   0        0        0     6474 2024-04-23 22:16:21.488513 omniconfig-0.1.1/omniconfig/utils.py
+-rw-r--r--   0        0        0       90 2024-04-23 23:26:53.546790 omniconfig-0.1.1/omniconfig/version.py
+-rw-r--r--   0        0        0      858 2024-04-23 23:26:46.062751 omniconfig-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7125 1970-01-01 00:00:00.000000 omniconfig-0.1.1/PKG-INFO
```

### Comparing `omniconfig-0.1.0/LICENSE` & `omniconfig-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `omniconfig-0.1.0/README.md` & `omniconfig-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-# configparse
+# omniconfig
 
 Python package for parsing configurations from YAML and command-line interface.
 
 ## Usage
 
-Decorator `configclass` in `configparse` package can help build argument parser from `dataclass` in `dataclasses`. Here is an example:
+Decorator `configclass` in `omniconfig` package can help build argument parser from `dataclass` in `dataclasses`. Here is an example:
 
 ```python
 from dataclasses import dataclass, field
 from typing import Any, Callable
 
-import configparse
+import omniconfig
 
 
-@configparse.configclass
+@omniconfig.configclass
 @dataclass
 class EvalConfig:
     """Evaluation Config class.
 
     Attributes:
         num_gpus (int): the number of GPUs. Defaults to ``8``.
     """
 
     num_gpus: int = 8
 
 
-@configparse.configclass
+@omniconfig.configclass
 @dataclass
 class QuantConfig:
     """Quantization config class.
 
     Attributes:
         dtype (str): Quantization data type. Defaults to ``"torch.float16"``.
         group_shape (list[int]): Quantization group shape. Defaults to ``(1, -1)``.
@@ -57,15 +57,15 @@
                 default=defaults.get("group_shape", (1, -1)),
                 help="Quantization group shape",
             ),
         )
         return overwrites, defaults
 
 
-@configparse.configclass
+@omniconfig.configclass
 @dataclass
 class ModelConfig:
     """Model Config class.
 
     Attributes:
         name (str): the model name.
         group (str): the model family.
@@ -74,29 +74,29 @@
     name: str
     family: str = field(init=False, default="")
 
     def __post_init__(self):
         self.family = self.name.split("-")[0]
 
 
-@configparse.configclass
+@omniconfig.configclass
 @dataclass
 class QuantizedModelConfig(ModelConfig):
     """Quantized Model Config class.
 
     Attributes:
         name (str): the model name.
         group (str): the model group.
         quant (QuantConfig): quantization configuration. Defaults to ``None``.
     """
 
     quant: QuantConfig | None = None
 
 
-@configparse.configclass
+@omniconfig.configclass
 @dataclass
 class Config:
     """Config class.
 
     Attributes:
         model (QuantizedModelConfig): the quantized model config.
         eval (EvalConfig): the evaluation config.
@@ -112,28 +112,28 @@
         Args:
             args (list[str], optional): Arguments to parse. Defaults to ``None``.
 
         Returns:
             tuple[Config, dict[str, dict], list[str]]: Configs from the parsed arguments,
                                                        parsed yaml configs, and unknown arguments.
         """
-        parser = configparse.ConfigParser("Evaluate Quantized Model")
+        parser = omniconfig.omniconfigr("Evaluate Quantized Model")
         parser.add_config(Config)
         config, parsed_args, unknown_args = parser.parse_known_args(args)
         assert isinstance(config, Config)
         return config, parsed_args, unknown_args
 
     @staticmethod
     def dump_default(path: str = "default.yaml") -> None:
         """Dump default configuration to a yaml file.
 
         Args:
             path (str, optional): The path to save the default configuration. Defaults to ``"default.yaml"``.
         """
-        parser = configparse.ConfigParser("Evaluate Quantized Model")
+        parser = omniconfig.omniconfigr("Evaluate Quantized Model")
         parser.add_config(Config)
         if path.endswith(("yaml", "yml")):
             parser.dump_yaml(path)
         elif path.endswith("toml"):
             parser.dump_toml(path)
         else:
             raise ValueError(f"Unsupported file format: {path}")
```

### Comparing `omniconfig-0.1.0/omniconfig/args.py` & `omniconfig-0.1.1/omniconfig/args.py`

 * *Files identical despite different names*

### Comparing `omniconfig-0.1.0/omniconfig/configclass.py` & `omniconfig-0.1.1/omniconfig/configclass.py`

 * *Files identical despite different names*

### Comparing `omniconfig-0.1.0/omniconfig/parser.py` & `omniconfig-0.1.1/omniconfig/parser.py`

 * *Files identical despite different names*

### Comparing `omniconfig-0.1.0/omniconfig/utils.py` & `omniconfig-0.1.1/omniconfig/utils.py`

 * *Files identical despite different names*

### Comparing `omniconfig-0.1.0/pyproject.toml` & `omniconfig-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omniconfig"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python package for parsing configurations from YAML and TOML and command-line interface."
 authors = ["Yujun(Xavier) Lin"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10 <4.0"
```

### Comparing `omniconfig-0.1.0/PKG-INFO` & `omniconfig-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 Metadata-Version: 2.1
 Name: omniconfig
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python package for parsing configurations from YAML and TOML and command-line interface.
 License: AGPL-3.0-only
 Author: Yujun(Xavier) Lin
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyYAML (>=6.0)
 Requires-Dist: docstring-parser (>=0.15)
 Requires-Dist: toml (>=0.10)
 Description-Content-Type: text/markdown
 
-# configparse
+# omniconfig
 
 Python package for parsing configurations from YAML and command-line interface.
 
 ## Usage
 
-Decorator `configclass` in `configparse` package can help build argument parser from `dataclass` in `dataclasses`. Here is an example:
+Decorator `configclass` in `omniconfig` package can help build argument parser from `dataclass` in `dataclasses`. Here is an example:
 
 ```python
 from dataclasses import dataclass, field
 from typing import Any, Callable
 
-import configparse
+import omniconfig
 
 
-@configparse.configclass
+@omniconfig.configclass
 @dataclass
 class EvalConfig:
     """Evaluation Config class.
 
     Attributes:
         num_gpus (int): the number of GPUs. Defaults to ``8``.
     """
 
     num_gpus: int = 8
 
 
-@configparse.configclass
+@omniconfig.configclass
 @dataclass
 class QuantConfig:
     """Quantization config class.
 
     Attributes:
         dtype (str): Quantization data type. Defaults to ``"torch.float16"``.
         group_shape (list[int]): Quantization group shape. Defaults to ``(1, -1)``.
@@ -74,15 +74,15 @@
                 default=defaults.get("group_shape", (1, -1)),
                 help="Quantization group shape",
             ),
         )
         return overwrites, defaults
 
 
-@configparse.configclass
+@omniconfig.configclass
 @dataclass
 class ModelConfig:
     """Model Config class.
 
     Attributes:
         name (str): the model name.
         group (str): the model family.
@@ -91,29 +91,29 @@
     name: str
     family: str = field(init=False, default="")
 
     def __post_init__(self):
         self.family = self.name.split("-")[0]
 
 
-@configparse.configclass
+@omniconfig.configclass
 @dataclass
 class QuantizedModelConfig(ModelConfig):
     """Quantized Model Config class.
 
     Attributes:
         name (str): the model name.
         group (str): the model group.
         quant (QuantConfig): quantization configuration. Defaults to ``None``.
     """
 
     quant: QuantConfig | None = None
 
 
-@configparse.configclass
+@omniconfig.configclass
 @dataclass
 class Config:
     """Config class.
 
     Attributes:
         model (QuantizedModelConfig): the quantized model config.
         eval (EvalConfig): the evaluation config.
@@ -129,28 +129,28 @@
         Args:
             args (list[str], optional): Arguments to parse. Defaults to ``None``.
 
         Returns:
             tuple[Config, dict[str, dict], list[str]]: Configs from the parsed arguments,
                                                        parsed yaml configs, and unknown arguments.
         """
-        parser = configparse.ConfigParser("Evaluate Quantized Model")
+        parser = omniconfig.omniconfigr("Evaluate Quantized Model")
         parser.add_config(Config)
         config, parsed_args, unknown_args = parser.parse_known_args(args)
         assert isinstance(config, Config)
         return config, parsed_args, unknown_args
 
     @staticmethod
     def dump_default(path: str = "default.yaml") -> None:
         """Dump default configuration to a yaml file.
 
         Args:
             path (str, optional): The path to save the default configuration. Defaults to ``"default.yaml"``.
         """
-        parser = configparse.ConfigParser("Evaluate Quantized Model")
+        parser = omniconfig.omniconfigr("Evaluate Quantized Model")
         parser.add_config(Config)
         if path.endswith(("yaml", "yml")):
             parser.dump_yaml(path)
         elif path.endswith("toml"):
             parser.dump_toml(path)
         else:
             raise ValueError(f"Unsupported file format: {path}")
```

