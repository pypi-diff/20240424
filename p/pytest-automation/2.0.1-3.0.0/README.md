# Comparing `tmp/pytest-automation-2.0.1.tar.gz` & `tmp/pytest_automation-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-automation-2.0.1.tar", last modified: Fri May 20 23:38:21 2022, max compression
+gzip compressed data, was "pytest_automation-3.0.0.tar", last modified: Wed Apr 24 18:15:24 2024, max compression
```

## Comparing `pytest-automation-2.0.1.tar` & `pytest_automation-3.0.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 23:38:21.309880 pytest-automation-2.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 23:38:21.305880 pytest-automation-2.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 23:38:21.305880 pytest-automation-2.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      679 2022-05-20 23:38:00.000000 pytest-automation-2.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-05-20 23:38:00.000000 pytest-automation-2.0.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-05-20 23:38:00.000000 pytest-automation-2.0.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-05-20 23:38:00.000000 pytest-automation-2.0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 23:38:21.309880 pytest-automation-2.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      685 2022-05-20 23:38:00.000000 pytest-automation-2.0.1/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2467 2022-05-20 23:38:00.000000 pytest-automation-2.0.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-05-20 23:38:00.000000 pytest-automation-2.0.1/.github/workflows/label-prod-pr.yml
--rw-r--r--   0 runner    (1001) docker     (121)      810 2022-05-20 23:38:00.000000 pytest-automation-2.0.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1850 2022-05-20 23:38:00.000000 pytest-automation-2.0.1/.github/workflows/stable-pr-merged.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1810 2022-05-20 23:38:00.000000 pytest-automation-2.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     3954 2022-05-20 23:38:00.000000 pytest-automation-2.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1533 2022-05-20 23:38:00.000000 pytest-automation-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    16183 2022-05-20 23:38:21.309880 pytest-automation-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15288 2022-05-20 23:38:00.000000 pytest-automation-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 23:38:21.309880 pytest-automation-2.0.1/automation/
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-05-20 23:38:00.000000 pytest-automation-2.0.1/automation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10263 2022-05-20 23:38:00.000000 pytest-automation-2.0.1/automation/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3050 2022-05-20 23:38:00.000000 pytest-automation-2.0.1/automation/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     4018 2022-05-20 23:38:00.000000 pytest-automation-2.0.1/automation/yamlfile.py
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-05-20 23:38:00.000000 pytest-automation-2.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 23:38:21.309880 pytest-automation-2.0.1/pytest_automation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    16183 2022-05-20 23:38:20.000000 pytest-automation-2.0.1/pytest_automation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      735 2022-05-20 23:38:21.000000 pytest-automation-2.0.1/pytest_automation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-20 23:38:20.000000 pytest-automation-2.0.1/pytest_automation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-05-20 23:38:20.000000 pytest-automation-2.0.1/pytest_automation.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-05-20 23:38:21.000000 pytest-automation-2.0.1/pytest_automation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-05-20 23:38:21.000000 pytest-automation-2.0.1/pytest_automation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-05-20 23:38:00.000000 pytest-automation-2.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-20 23:38:21.309880 pytest-automation-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-05-20 23:38:00.000000 pytest-automation-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:15:24.866887 pytest_automation-3.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:15:24.862887 pytest_automation-3.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:15:24.862887 pytest_automation-3.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-24 18:15:17.000000 pytest_automation-3.0.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-24 18:15:17.000000 pytest_automation-3.0.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-24 18:15:17.000000 pytest_automation-3.0.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-24 18:15:17.000000 pytest_automation-3.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:15:24.862887 pytest_automation-3.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-24 18:15:17.000000 pytest_automation-3.0.0/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-24 18:15:17.000000 pytest_automation-3.0.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-24 18:15:17.000000 pytest_automation-3.0.0/.github/workflows/label-prod-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-24 18:15:17.000000 pytest_automation-3.0.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-24 18:15:17.000000 pytest_automation-3.0.0/.github/workflows/stable-pr-merged.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-24 18:15:17.000000 pytest_automation-3.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-24 18:15:17.000000 pytest_automation-3.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-24 18:15:17.000000 pytest_automation-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16234 2024-04-24 18:15:24.866887 pytest_automation-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15288 2024-04-24 18:15:17.000000 pytest_automation-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:15:24.862887 pytest_automation-3.0.0/automation/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-24 18:15:17.000000 pytest_automation-3.0.0/automation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10253 2024-04-24 18:15:17.000000 pytest_automation-3.0.0/automation/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-24 18:15:17.000000 pytest_automation-3.0.0/automation/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-24 18:15:17.000000 pytest_automation-3.0.0/automation/yamlfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-24 18:15:17.000000 pytest_automation-3.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:15:24.866887 pytest_automation-3.0.0/pytest_automation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16234 2024-04-24 18:15:24.000000 pytest_automation-3.0.0/pytest_automation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-24 18:15:24.000000 pytest_automation-3.0.0/pytest_automation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 18:15:24.000000 pytest_automation-3.0.0/pytest_automation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-24 18:15:24.000000 pytest_automation-3.0.0/pytest_automation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 18:15:24.000000 pytest_automation-3.0.0/pytest_automation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 18:15:24.000000 pytest_automation-3.0.0/pytest_automation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-24 18:15:17.000000 pytest_automation-3.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 18:15:24.866887 pytest_automation-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-24 18:15:17.000000 pytest_automation-3.0.0/setup.py
```

### Comparing `pytest-automation-2.0.1/.github/ISSUE_TEMPLATE/bug_report.md` & `pytest_automation-3.0.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pytest-automation-2.0.1/.github/ISSUE_TEMPLATE/feature_request.md` & `pytest_automation-3.0.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pytest-automation-2.0.1/.github/workflows/changelog.yml` & `pytest_automation-3.0.0/.github/workflows/changelog.yml`

 * *Files identical despite different names*

### Comparing `pytest-automation-2.0.1/.github/workflows/codeql-analysis.yml` & `pytest_automation-3.0.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `pytest-automation-2.0.1/.github/workflows/pypi-publish.yml` & `pytest_automation-3.0.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `pytest-automation-2.0.1/.github/workflows/stable-pr-merged.yml` & `pytest_automation-3.0.0/.github/workflows/stable-pr-merged.yml`

 * *Files identical despite different names*

### Comparing `pytest-automation-2.0.1/.gitignore` & `pytest_automation-3.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-automation-2.0.1/CHANGELOG.md` & `pytest_automation-3.0.0/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -24,14 +24,24 @@
 ### Removed:
 -
 
 -->
 
 ------
 
+## [v3.0.0](https://github.com/asfadmin/Discovery-PytestAutomation/compare/v2.0.1...v3.0.0)
+
+### Breaking Change:
+- Upgraded to pytest-8. **Plugin will now only work with pytest>=8.0.0**.
+
+### Fixed:
+- Completely removes legacy dependency from requirements.txt (`py` package) per cve advisory https://github.com/advisories/GHSA-w596-4wvx-j9j6
+
+------
+
 ## [v2.0.1](https://github.com/asfadmin/Discovery-PytestAutomation/compare/v2.0.0...v2.0.1)
 
 ### Fixed:
 - Pass **copies** of params into the test, so that they can't modify the params before `repr_failure` is called on test cleanup.
 
 ------
```

### Comparing `pytest-automation-2.0.1/LICENSE` & `pytest_automation-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-automation-2.0.1/PKG-INFO` & `pytest_automation-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-automation
-Version: 2.0.1
+Version: 3.0.0
 Summary: pytest plugin for building a test suite, using YAML files to extend pytest parameterize functionality.
 Home-page: https://github.com/asfadmin/Discovery-PytestAutomation
 Author: Alaska Satellite Facility Discovery Team
 Author-email: uaf-asf-discovery@alaska.edu
 License: BSD
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: BSD License
@@ -14,14 +14,16 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Testing
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pytest>=7.0.0
+Requires-Dist: PyYAML
 
 # Pytest Automation
 
 [![image](https://img.shields.io/pypi/v/pytest-automation.svg)](https://pypi.python.org/pypi/pytest-automation) [![CodeFactor](https://www.codefactor.io/repository/github/asfadmin/discovery-pytestautomation/badge/stable)](https://www.codefactor.io/repository/github/asfadmin/discovery-pytestautomation/overview/stable) [![Join the chat at https://gitter.im/ASFDiscovery/pytest-automation](https://badges.gitter.im/ASFDiscovery/pytest-automation.svg)](https://gitter.im/ASFDiscovery/pytest-automation?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
 For automating test creation. This plugin lets you send a list of tests (arguments defined in yaml's), to python methods. For creating an agile test suite.
```

### Comparing `pytest-automation-2.0.1/README.md` & `pytest_automation-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest-automation-2.0.1/automation/helpers.py` & `pytest_automation-3.0.0/automation/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 # For type hints only:
 from typing import Union
 from types import ModuleType
 from _pytest.config import Config
 
 import os
-import re
 import fnmatch
 
 # Returns true if any "section" (any part between /, "section1/section2/..."),
 # matches any pattern.
 #   For finding if an "excluded" directory exists in a path, so you can remove the path
 #   from the list.
 def pathSectionContainsPattern(path: str, patterns: list=["*"]) -> bool:
```

### Comparing `pytest-automation-2.0.1/automation/plugin.py` & `pytest_automation-3.0.0/automation/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from automation import helpers
 
 import pathlib
 
 # For type hints only:
 from pytest import Session, File
 from _pytest.config.argparsing import Parser
-from py._path.local import LocalPath
 from _pytest.nodes import Collector
 
 # Runs once at the start of everything:
 # pylint: disable=fixme
 #   TODO: Move this to a hook *after* `pytest_collect_file` runs. Can have the collect_file hook look for pytest-config/pytest-managers,
 #   to automatically include the norecursedirs logic when searching for them.
 #   - From here (https://github.com/pytest-dev/pytest/issues/3261#issuecomment-369740536), seems like `pytest_runtestloop` would be the
@@ -42,10 +41,12 @@
         help = "Only run test types that contain this in their name.")
     group.addoption("--dont-run-type", "--dt", action="append", default=None,
         help = "Dont run test types that contain this in their name.")
     group.addoption("--skip-all", action="store_true",
         help = "Skips ALL the tests. (Added for pipeline use).")
 
 # Based on: https://docs.pytest.org/en/6.2.x/example/nonpython.html
-def pytest_collect_file(parent: Collector, path: LocalPath) -> File:
-    if path.ext in [".yml", ".yaml"] and path.basename.startswith("test_"):
-        return yamlfile.YamlFile.from_parent(parent, path=pathlib.Path(path))
+# path is deprecated, using file_path
+# https://docs.pytest.org/en/7.1.x/reference/reference.html#pytest_collect_file
+def pytest_collect_file(parent: Collector, file_path: pathlib.Path) -> File:
+    if file_path.suffix in [".yml", ".yaml"] and file_path.name.startswith("test_"):
+        return yamlfile.YamlFile.from_parent(parent, path=file_path)
```

### Comparing `pytest-automation-2.0.1/automation/yamlfile.py` & `pytest_automation-3.0.0/automation/yamlfile.py`

 * *Files identical despite different names*

### Comparing `pytest-automation-2.0.1/pytest_automation.egg-info/PKG-INFO` & `pytest_automation-3.0.0/pytest_automation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-automation
-Version: 2.0.1
+Version: 3.0.0
 Summary: pytest plugin for building a test suite, using YAML files to extend pytest parameterize functionality.
 Home-page: https://github.com/asfadmin/Discovery-PytestAutomation
 Author: Alaska Satellite Facility Discovery Team
 Author-email: uaf-asf-discovery@alaska.edu
 License: BSD
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: BSD License
@@ -14,14 +14,16 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Testing
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pytest>=7.0.0
+Requires-Dist: PyYAML
 
 # Pytest Automation
 
 [![image](https://img.shields.io/pypi/v/pytest-automation.svg)](https://pypi.python.org/pypi/pytest-automation) [![CodeFactor](https://www.codefactor.io/repository/github/asfadmin/discovery-pytestautomation/badge/stable)](https://www.codefactor.io/repository/github/asfadmin/discovery-pytestautomation/overview/stable) [![Join the chat at https://gitter.im/ASFDiscovery/pytest-automation](https://badges.gitter.im/ASFDiscovery/pytest-automation.svg)](https://gitter.im/ASFDiscovery/pytest-automation?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
 For automating test creation. This plugin lets you send a list of tests (arguments defined in yaml's), to python methods. For creating an agile test suite.
```

### Comparing `pytest-automation-2.0.1/pytest_automation.egg-info/SOURCES.txt` & `pytest_automation-3.0.0/pytest_automation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-automation-2.0.1/setup.py` & `pytest_automation-3.0.0/setup.py`

 * *Files identical despite different names*

