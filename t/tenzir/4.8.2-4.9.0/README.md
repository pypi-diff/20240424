# Comparing `tmp/tenzir-4.8.2.tar.gz` & `tmp/tenzir-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tenzir-4.8.2.tar", max compression
+gzip compressed data, was "tenzir-4.9.0.tar", max compression
```

## Comparing `tenzir-4.8.2.tar` & `tenzir-4.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1868 2024-01-24 16:47:36.799447 tenzir-4.8.2/README.md
--rw-r--r--   0        0        0     1812 2024-01-24 16:47:36.799447 tenzir-4.8.2/pyproject.toml
--rw-r--r--   0        0        0       77 2024-01-24 16:47:36.799447 tenzir-4.8.2/tenzir/__init__.py
--rw-r--r--   0        0        0       74 2024-01-24 16:47:36.799447 tenzir-4.8.2/tenzir/tenzir/__init__.py
--rw-r--r--   0        0        0     2909 2024-01-24 16:47:36.799447 tenzir-4.8.2/tenzir/tenzir/cli.py
--rw-r--r--   0        0        0     3645 2024-01-24 16:47:36.799447 tenzir-4.8.2/tenzir/tenzir/convert.py
--rw-r--r--   0        0        0     6162 2024-01-24 16:47:36.799447 tenzir-4.8.2/tenzir/tenzir/tenzir.py
--rw-r--r--   0        0        0        0 2024-01-24 16:47:36.799447 tenzir-4.8.2/tenzir/tools/__init__.py
--rw-r--r--   0        0        0    13985 2024-01-24 16:47:36.799447 tenzir-4.8.2/tenzir/tools/python_operator_executor.py
--rw-r--r--   0        0        0    14634 2024-01-24 16:47:36.799447 tenzir-4.8.2/tenzir/utils/arrow.py
--rw-r--r--   0        0        0     2058 2024-01-24 16:47:36.799447 tenzir-4.8.2/tenzir/utils/asyncio.py
--rw-r--r--   0        0        0      740 2024-01-24 16:47:36.799447 tenzir-4.8.2/tenzir/utils/config.py
--rw-r--r--   0        0        0     1863 2024-01-24 16:47:36.799447 tenzir-4.8.2/tenzir/utils/logging.py
--rw-r--r--   0        0        0     2856 1970-01-01 00:00:00.000000 tenzir-4.8.2/setup.py
--rw-r--r--   0        0        0     3332 1970-01-01 00:00:00.000000 tenzir-4.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1868 2024-02-21 12:26:03.748291 tenzir-4.9.0/README.md
+-rw-r--r--   0        0        0     1812 2024-02-21 12:26:03.748291 tenzir-4.9.0/pyproject.toml
+-rw-r--r--   0        0        0       77 2024-02-21 12:26:03.748291 tenzir-4.9.0/tenzir/__init__.py
+-rw-r--r--   0        0        0       74 2024-02-21 12:26:03.748291 tenzir-4.9.0/tenzir/tenzir/__init__.py
+-rw-r--r--   0        0        0     2909 2024-02-21 12:26:03.748291 tenzir-4.9.0/tenzir/tenzir/cli.py
+-rw-r--r--   0        0        0     3645 2024-02-21 12:26:03.748291 tenzir-4.9.0/tenzir/tenzir/convert.py
+-rw-r--r--   0        0        0     6162 2024-02-21 12:26:03.748291 tenzir-4.9.0/tenzir/tenzir/tenzir.py
+-rw-r--r--   0        0        0        0 2024-02-21 12:26:03.748291 tenzir-4.9.0/tenzir/tools/__init__.py
+-rw-r--r--   0        0        0    13985 2024-02-21 12:26:03.748291 tenzir-4.9.0/tenzir/tools/python_operator_executor.py
+-rw-r--r--   0        0        0    14634 2024-02-21 12:26:03.748291 tenzir-4.9.0/tenzir/utils/arrow.py
+-rw-r--r--   0        0        0     2058 2024-02-21 12:26:03.748291 tenzir-4.9.0/tenzir/utils/asyncio.py
+-rw-r--r--   0        0        0      740 2024-02-21 12:26:03.748291 tenzir-4.9.0/tenzir/utils/config.py
+-rw-r--r--   0        0        0     1863 2024-02-21 12:26:03.748291 tenzir-4.9.0/tenzir/utils/logging.py
+-rw-r--r--   0        0        0     2856 1970-01-01 00:00:00.000000 tenzir-4.9.0/setup.py
+-rw-r--r--   0        0        0     3332 1970-01-01 00:00:00.000000 tenzir-4.9.0/PKG-INFO
```

### Comparing `tenzir-4.8.2/README.md` & `tenzir-4.9.0/README.md`

 * *Files identical despite different names*

### Comparing `tenzir-4.8.2/pyproject.toml` & `tenzir-4.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tenzir"
-version = "4.8.2"
+version = "4.9.0"
 description = "A security telemetry engine for detection and response"
 authors = ["Tenzir <engineering@tenzir.com>"]
 maintainers = ["Tenzir <engineering@tenzir.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `tenzir-4.8.2/tenzir/tenzir/cli.py` & `tenzir-4.9.0/tenzir/tenzir/cli.py`

 * *Files identical despite different names*

### Comparing `tenzir-4.8.2/tenzir/tenzir/convert.py` & `tenzir-4.9.0/tenzir/tenzir/convert.py`

 * *Files identical despite different names*

### Comparing `tenzir-4.8.2/tenzir/tenzir/tenzir.py` & `tenzir-4.9.0/tenzir/tenzir/tenzir.py`

 * *Files identical despite different names*

### Comparing `tenzir-4.8.2/tenzir/tools/python_operator_executor.py` & `tenzir-4.9.0/tenzir/tools/python_operator_executor.py`

 * *Files identical despite different names*

### Comparing `tenzir-4.8.2/tenzir/utils/arrow.py` & `tenzir-4.9.0/tenzir/utils/arrow.py`

 * *Files identical despite different names*

### Comparing `tenzir-4.8.2/tenzir/utils/asyncio.py` & `tenzir-4.9.0/tenzir/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `tenzir-4.8.2/tenzir/utils/config.py` & `tenzir-4.9.0/tenzir/utils/config.py`

 * *Files identical despite different names*

### Comparing `tenzir-4.8.2/tenzir/utils/logging.py` & `tenzir-4.9.0/tenzir/utils/logging.py`

 * *Files identical despite different names*

### Comparing `tenzir-4.8.2/setup.py` & `tenzir-4.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 extras_require = \
 {'module': ['numpy>=1.24,<2.0'],
  'operator': ['python-box>=7.0,<8.0', 'pandas>=2.1.3,<3.0.0']}
 
 setup_kwargs = {
     'name': 'tenzir',
-    'version': '4.8.2',
+    'version': '4.9.0',
     'description': 'A security telemetry engine for detection and response',
     'long_description': '# Tenzir Python\n\nThe Python package of Tenzir provides a flexible control plane to integrate Tenzir\nwith other security tools.\n\n> **Note**\n> The Python effort is still highly experimental and subject to rapid change.\n> Please do not consider it for production use.\n\n## Usage\n\nTo get started, clone the Tenzir repository and install the Python package via\n[Poetry](https://python-poetry.org/docs/):\n\n```bash\ngit clone https://github.com/tenzir/tenzir.git\ncd tenzir/python\npoetry install -E module\n```\n\n## Development\n\nWe recommend that you work with an editable installation, which is the default\nfor `poetry install`.\n\n### Unit Tests\n\nRun the unit tests via pytest:\n\n```bash\npoetry run pytest\n```\n\n### Integration Tests\n\nRun the integrations tests via Docker Compose and pytest:\n\n```bash\n./docker-poetry-run.sh pytest -v\n```\n\n## Packaging\n\nThe following instructions concern maintainers who want to publish the Python\npackage to PyPI.\n\n> **Note**\n> Our releasing scripts and CI run these steps automatically. You do not need to\n> intervene anywhere. The instructions below merely document the steps taken.\n\n### Bump the version\n\nPrior to releasing a new version, bump the version, e.g.:\n\n```bash\npoetry version 2.3.1\n```\n\nThis updates the `pyproject.toml` file.\n\n### Publish to Test PyPI\n\n1. Add a Test PyPi repository:\n\n   ```bash\n   poetry config repositories.test-pypi https://test.pypi.org/legacy/\n   ```\n\n2. Get the token from <https://test.pypi.org/manage/account/token/>.\n\n3. Store the token:\n\n  ```bash\n  poetry config pypi-token.test-pypi pypi-XXXXXXXX\n  ```\n\n4. Publish:\n  \n   ```bash\n   poetry publish --build -r test-pypi\n   ```\n\n### Publish to PyPI\n\n1. Get the token from <https://pypi.org/manage/account/token/>.\n\n2. Store the token:\n\n  ```bash\n  poetry config pypi-token.pypi pypi-XXXXXXXX\n  ```\n\n3. Publish\n\n   ```bash\n   poetry publish --build\n   ```\n',
     'author': 'Tenzir',
     'author_email': 'engineering@tenzir.com',
     'maintainer': 'Tenzir',
     'maintainer_email': 'engineering@tenzir.com',
     'url': 'https://tenzir.com',
```

### Comparing `tenzir-4.8.2/PKG-INFO` & `tenzir-4.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tenzir
-Version: 4.8.2
+Version: 4.9.0
 Summary: A security telemetry engine for detection and response
 Home-page: https://tenzir.com
 License: BSD-3-Clause
 Author: Tenzir
 Author-email: engineering@tenzir.com
 Maintainer: Tenzir
 Maintainer-email: engineering@tenzir.com
```

