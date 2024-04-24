# Comparing `tmp/confme-2.0.2.tar.gz` & `tmp/confme-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confme-2.0.2.tar", max compression
+gzip compressed data, was "confme-2.0.3.tar", max compression
```

## Comparing `confme-2.0.2.tar` & `confme-2.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1085 2023-07-10 16:22:35.041099 confme-2.0.2/LICENSE
--rw-r--r--   0        0        0     9849 2023-07-10 16:22:35.041099 confme-2.0.2/README.md
--rw-r--r--   0        0        0      173 2023-07-10 16:22:35.041099 confme-2.0.2/confme/__init__.py
--rw-r--r--   0        0        0      746 2023-07-10 16:22:35.041099 confme-2.0.2/confme/annotation.py
--rw-r--r--   0        0        0        0 2023-07-10 16:22:35.041099 confme-2.0.2/confme/core/__init__.py
--rw-r--r--   0        0        0     1091 2023-07-10 16:22:35.045099 confme-2.0.2/confme/core/argument_overwrite.py
--rw-r--r--   0        0        0     6859 2023-07-10 16:22:35.045099 confme-2.0.2/confme/core/base_config.py
--rw-r--r--   0        0        0      743 2023-07-10 16:22:35.045099 confme-2.0.2/confme/core/env_overwrite.py
--rw-r--r--   0        0        0    18170 2023-07-10 16:22:35.045099 confme-2.0.2/confme/pylintrc
--rw-r--r--   0        0        0      841 2023-07-10 16:22:35.045099 confme-2.0.2/confme/source_backend/__init__.py
--rw-r--r--   0        0        0      728 2023-07-10 16:22:35.045099 confme-2.0.2/confme/source_backend/backend_base.py
--rw-r--r--   0        0        0      847 2023-07-10 16:22:35.045099 confme-2.0.2/confme/source_backend/backend_yaml.py
--rw-r--r--   0        0        0        0 2023-07-10 16:22:35.045099 confme-2.0.2/confme/utils/__init__.py
--rw-r--r--   0        0        0      121 2023-07-10 16:22:35.045099 confme-2.0.2/confme/utils/base_exception.py
--rw-r--r--   0        0        0      974 2023-07-10 16:22:35.045099 confme-2.0.2/confme/utils/deprecated.py
--rw-r--r--   0        0        0     1099 2023-07-10 16:22:35.045099 confme-2.0.2/confme/utils/dict_util.py
--rw-r--r--   0        0        0      763 2023-07-10 16:22:35.045099 confme-2.0.2/confme/utils/typing.py
--rw-r--r--   0        0        0     1355 2023-07-10 16:22:35.045099 confme-2.0.2/pyproject.toml
--rw-r--r--   0        0        0    11088 1970-01-01 00:00:00.000000 confme-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-04-24 13:20:26.683281 confme-2.0.3/LICENSE
+-rw-r--r--   0        0        0     9849 2024-04-24 13:20:26.683281 confme-2.0.3/README.md
+-rw-r--r--   0        0        0      173 2024-04-24 13:20:26.683281 confme-2.0.3/confme/__init__.py
+-rw-r--r--   0        0        0      746 2024-04-24 13:20:26.683281 confme-2.0.3/confme/annotation.py
+-rw-r--r--   0        0        0        0 2024-04-24 13:20:26.683281 confme-2.0.3/confme/core/__init__.py
+-rw-r--r--   0        0        0     1091 2024-04-24 13:20:26.683281 confme-2.0.3/confme/core/argument_overwrite.py
+-rw-r--r--   0        0        0     6859 2024-04-24 13:20:26.683281 confme-2.0.3/confme/core/base_config.py
+-rw-r--r--   0        0        0      743 2024-04-24 13:20:26.683281 confme-2.0.3/confme/core/env_overwrite.py
+-rw-r--r--   0        0        0    18170 2024-04-24 13:20:26.683281 confme-2.0.3/confme/pylintrc
+-rw-r--r--   0        0        0      841 2024-04-24 13:20:26.683281 confme-2.0.3/confme/source_backend/__init__.py
+-rw-r--r--   0        0        0      728 2024-04-24 13:20:26.683281 confme-2.0.3/confme/source_backend/backend_base.py
+-rw-r--r--   0        0        0      847 2024-04-24 13:20:26.683281 confme-2.0.3/confme/source_backend/backend_yaml.py
+-rw-r--r--   0        0        0        0 2024-04-24 13:20:26.683281 confme-2.0.3/confme/utils/__init__.py
+-rw-r--r--   0        0        0      121 2024-04-24 13:20:26.683281 confme-2.0.3/confme/utils/base_exception.py
+-rw-r--r--   0        0        0      974 2024-04-24 13:20:26.683281 confme-2.0.3/confme/utils/deprecated.py
+-rw-r--r--   0        0        0     1099 2024-04-24 13:20:26.687281 confme-2.0.3/confme/utils/dict_util.py
+-rw-r--r--   0        0        0      763 2024-04-24 13:20:26.687281 confme-2.0.3/confme/utils/typing.py
+-rw-r--r--   0        0        0     1436 2024-04-24 13:20:26.687281 confme-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0    11280 1970-01-01 00:00:00.000000 confme-2.0.3/PKG-INFO
```

### Comparing `confme-2.0.2/LICENSE` & `confme-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `confme-2.0.2/README.md` & `confme-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `confme-2.0.2/confme/annotation.py` & `confme-2.0.3/confme/annotation.py`

 * *Files identical despite different names*

### Comparing `confme-2.0.2/confme/core/argument_overwrite.py` & `confme-2.0.3/confme/core/argument_overwrite.py`

 * *Files identical despite different names*

### Comparing `confme-2.0.2/confme/core/base_config.py` & `confme-2.0.3/confme/core/base_config.py`

 * *Files identical despite different names*

### Comparing `confme-2.0.2/confme/core/env_overwrite.py` & `confme-2.0.3/confme/core/env_overwrite.py`

 * *Files identical despite different names*

### Comparing `confme-2.0.2/confme/pylintrc` & `confme-2.0.3/confme/pylintrc`

 * *Files identical despite different names*

### Comparing `confme-2.0.2/confme/source_backend/__init__.py` & `confme-2.0.3/confme/source_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `confme-2.0.2/confme/source_backend/backend_base.py` & `confme-2.0.3/confme/source_backend/backend_base.py`

 * *Files identical despite different names*

### Comparing `confme-2.0.2/confme/source_backend/backend_yaml.py` & `confme-2.0.3/confme/source_backend/backend_yaml.py`

 * *Files identical despite different names*

### Comparing `confme-2.0.2/confme/utils/deprecated.py` & `confme-2.0.3/confme/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `confme-2.0.2/confme/utils/dict_util.py` & `confme-2.0.3/confme/utils/dict_util.py`

 * *Files identical despite different names*

### Comparing `confme-2.0.2/confme/utils/typing.py` & `confme-2.0.3/confme/utils/typing.py`

 * *Files identical despite different names*

### Comparing `confme-2.0.2/pyproject.toml` & `confme-2.0.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "confme"
-version = "2.0.2"
+version = "2.0.3"
 description = "Easy configuration management in python"
 authors = ["Iwan Silvan Bolzern <iwan.bolzern@roche.com>"]
 license = "LICENSE"
 readme = "README.md"
 homepage = "https://github.com/iwanbolzern/confme"
 repository = "https://github.com/iwanbolzern/confme"
 classifiers = [
@@ -25,18 +25,22 @@
 ]
 packages = [
     { include = "confme" },
 ]
 
 
 [tool.poetry.dependencies]
-python = "^3.7.2"
+python = "^3.8"
 pyyaml = ">=5.3"
 pydantic = "^2.0"
+pydantic-core = "^2.0.0"
+annotated-types = "^0.6.0"
 tabulate = ">=0.8.9"
+typing-extensions = "^4.11.0"
+
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.1.2"
 pylint = "^2.17.4"
 sphinx = "^3.2.1"
 recommonmark = "^0.6.0"
 pytest-cov = "^2.11.1"
```

### Comparing `confme-2.0.2/PKG-INFO` & `confme-2.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
 Name: confme
-Version: 2.0.2
+Version: 2.0.3
 Summary: Easy configuration management in python
 Home-page: https://github.com/iwanbolzern/confme
 License: LICENSE
 Author: Iwan Silvan Bolzern
 Author-email: iwan.bolzern@roche.com
-Requires-Python: >=3.7.2,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: annotated-types (>=0.6.0,<0.7.0)
 Requires-Dist: pydantic (>=2.0,<3.0)
+Requires-Dist: pydantic-core (>=2.0.0,<3.0.0)
 Requires-Dist: pyyaml (>=5.3)
 Requires-Dist: tabulate (>=0.8.9)
+Requires-Dist: typing-extensions (>=4.11.0,<5.0.0)
 Project-URL: Repository, https://github.com/iwanbolzern/confme
 Description-Content-Type: text/markdown
 
 # ConfMe: Configuration Made Easy 💖
 
 [![image](https://img.shields.io/pypi/v/confme?color=blue)](https://pypi.org/project/confme/) [![image](https://img.shields.io/pypi/l/confme)](https://pypi.org/project/confme/) [![image](https://github.com/iwanbolzern/ConfMe/workflows/Test/badge.svg?branch=master)](https://pypi.org/project/confme/)
 [![image](https://img.shields.io/pypi/pyversions/confme?color=blue)](https://pypi.org/project/confme/)
```

