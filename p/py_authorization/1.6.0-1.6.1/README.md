# Comparing `tmp/py_authorization-1.6.0.tar.gz` & `tmp/py_authorization-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_authorization-1.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "py_authorization-1.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `py_authorization-1.6.0.tar` & `py_authorization-1.6.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      119 2023-11-24 17:36:21.043058 py_authorization-1.6.0/.gitignore
--rw-r--r--   0        0        0       78 2023-11-24 17:36:21.043058 py_authorization-1.6.0/.isort.cfg
--rw-r--r--   0        0        0     1041 2023-11-24 17:36:21.043058 py_authorization-1.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      788 2023-11-24 17:36:21.043058 py_authorization-1.6.0/.vscode/settings.json
--rw-r--r--   0        0        0     1065 2023-11-24 17:36:21.043058 py_authorization-1.6.0/LICENSE
--rw-r--r--   0        0        0       23 2023-11-24 17:36:21.043058 py_authorization-1.6.0/README.md
--rwxr-xr-x   0        0        0      579 2023-11-24 17:36:21.043058 py_authorization-1.6.0/bin/new_line_check.sh
--rwxr-xr-x   0        0        0      481 2023-11-24 17:36:21.043058 py_authorization-1.6.0/bin/pdb_check.sh
--rw-r--r--   0        0        0      555 2023-11-25 18:28:12.820626 py_authorization-1.6.0/py_authorization/__init__.py
--rw-r--r--   0        0        0    10840 2023-11-25 18:16:28.281455 py_authorization-1.6.0/py_authorization/authorization.py
--rw-r--r--   0        0        0      325 2023-11-25 18:16:49.521889 py_authorization-1.6.0/py_authorization/context.py
--rw-r--r--   0        0        0      398 2023-11-25 18:16:46.689831 py_authorization-1.6.0/py_authorization/policy.py
--rw-r--r--   0        0        0      793 2023-11-25 18:16:24.262373 py_authorization-1.6.0/py_authorization/policy_strategy.py
--rw-r--r--   0        0        0      657 2023-11-25 18:16:48.201862 py_authorization-1.6.0/py_authorization/policy_strategy_builder.py
--rw-r--r--   0        0        0        0 2023-11-24 17:36:21.043058 py_authorization-1.6.0/py_authorization/py.typed
--rw-r--r--   0        0        0     5538 2023-11-25 18:16:39.722689 py_authorization-1.6.0/py_authorization/sql_parser.py
--rw-r--r--   0        0        0      128 2023-11-25 18:16:41.242720 py_authorization-1.6.0/py_authorization/user.py
--rw-r--r--   0        0        0      413 2023-11-25 18:16:21.792323 py_authorization-1.6.0/pyproject.toml
--rw-r--r--   0        0        0      177 2023-11-24 17:52:23.813702 py_authorization-1.6.0/requirements.txt
--rw-r--r--   0        0        0      377 2023-11-24 17:36:21.043058 py_authorization-1.6.0/setup.cfg
--rw-r--r--   0        0        0      309 2023-11-24 17:36:21.043058 py_authorization-1.6.0/setup.py
--rw-r--r--   0        0        0      106 2023-11-24 17:36:21.043058 py_authorization-1.6.0/tests/conftest.py
--rw-r--r--   0        0        0     5906 2023-11-24 17:36:21.043058 py_authorization-1.6.0/tests/test_authorization.py
--rw-r--r--   0        0        0     3304 2023-11-24 17:36:21.044058 py_authorization-1.6.0/tests/test_policy_finder.py
--rw-r--r--   0        0        0      235 1970-01-01 00:00:00.000000 py_authorization-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0      119 2023-11-24 17:36:21.043058 py_authorization-1.6.1/.gitignore
+-rw-r--r--   0        0        0       78 2023-11-24 17:36:21.043058 py_authorization-1.6.1/.isort.cfg
+-rw-r--r--   0        0        0     1041 2023-11-24 17:36:21.043058 py_authorization-1.6.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      639 2024-04-24 18:05:04.790648 py_authorization-1.6.1/.vscode/settings.json
+-rw-r--r--   0        0        0     1065 2023-11-24 17:36:21.043058 py_authorization-1.6.1/LICENSE
+-rw-r--r--   0        0        0       23 2023-11-24 17:36:21.043058 py_authorization-1.6.1/README.md
+-rwxr-xr-x   0        0        0      579 2023-11-24 17:36:21.043058 py_authorization-1.6.1/bin/new_line_check.sh
+-rwxr-xr-x   0        0        0      481 2023-11-24 17:36:21.043058 py_authorization-1.6.1/bin/pdb_check.sh
+-rw-r--r--   0        0        0      555 2024-04-24 18:10:36.894196 py_authorization-1.6.1/py_authorization/__init__.py
+-rw-r--r--   0        0        0    10794 2024-04-24 18:05:32.793851 py_authorization-1.6.1/py_authorization/authorization.py
+-rw-r--r--   0        0        0      325 2023-11-25 18:16:49.521889 py_authorization-1.6.1/py_authorization/context.py
+-rw-r--r--   0        0        0      398 2023-11-25 18:16:46.689831 py_authorization-1.6.1/py_authorization/policy.py
+-rw-r--r--   0        0        0      793 2023-11-25 18:16:24.262373 py_authorization-1.6.1/py_authorization/policy_strategy.py
+-rw-r--r--   0        0        0      657 2023-11-25 18:16:48.201862 py_authorization-1.6.1/py_authorization/policy_strategy_builder.py
+-rw-r--r--   0        0        0        0 2023-11-24 17:36:21.043058 py_authorization-1.6.1/py_authorization/py.typed
+-rw-r--r--   0        0        0     5538 2023-11-25 18:16:39.722689 py_authorization-1.6.1/py_authorization/sql_parser.py
+-rw-r--r--   0        0        0      128 2023-11-25 18:16:41.242720 py_authorization-1.6.1/py_authorization/user.py
+-rw-r--r--   0        0        0      413 2023-11-25 18:16:21.792323 py_authorization-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0      177 2023-11-24 17:52:23.813702 py_authorization-1.6.1/requirements.txt
+-rw-r--r--   0        0        0      377 2023-11-24 17:36:21.043058 py_authorization-1.6.1/setup.cfg
+-rw-r--r--   0        0        0      309 2023-11-24 17:36:21.043058 py_authorization-1.6.1/setup.py
+-rw-r--r--   0        0        0      106 2023-11-24 17:36:21.043058 py_authorization-1.6.1/tests/conftest.py
+-rw-r--r--   0        0        0     5906 2023-11-24 17:36:21.043058 py_authorization-1.6.1/tests/test_authorization.py
+-rw-r--r--   0        0        0     3304 2023-11-24 17:36:21.044058 py_authorization-1.6.1/tests/test_policy_finder.py
+-rw-r--r--   0        0        0      235 1970-01-01 00:00:00.000000 py_authorization-1.6.1/PKG-INFO
```

### Comparing `py_authorization-1.6.0/.pre-commit-config.yaml` & `py_authorization-1.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `py_authorization-1.6.0/.vscode/settings.json` & `py_authorization-1.6.1/.vscode/settings.json`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 {
   "editor.rulers": [
     120
   ],
   "editor.tabSize": 4,
-  "python.linting.lintOnSave": true,
-  "python.linting.mypyEnabled": true,
-  "python.linting.flake8Enabled": true,
-  "python.formatting.provider": "none",
   "editor.formatOnSave": true,
   "[python]": {
     "editor.formatOnSave": true,
     "editor.defaultFormatter": "ms-python.black-formatter",
     "editor.codeActionsOnSave": {
-      "source.organizeImports": true
+      "source.organizeImports": "explicit"
     },
   },
   "isort.args": [
     "--profile",
     "black"
   ],
   "python.testing.pytestArgs": [
```

### Comparing `py_authorization-1.6.0/LICENSE` & `py_authorization-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_authorization-1.6.0/bin/new_line_check.sh` & `py_authorization-1.6.1/bin/new_line_check.sh`

 * *Files identical despite different names*

### Comparing `py_authorization-1.6.0/py_authorization/__init__.py` & `py_authorization-1.6.1/py_authorization/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Easily manage authorization complex logic"""
 
-__version__ = "1.6.0"
+__version__ = "1.6.1"
 
 from .authorization import Authorization, CheckResponse
 from .context import Context
 from .policy import Policy, Strategy
 from .policy_strategy import EmptyEntity, PolicyStrategy
 from .policy_strategy_builder import PolicyStrategyBuilder, StrategyMapper
 from .user import User
```

### Comparing `py_authorization-1.6.0/py_authorization/authorization.py` & `py_authorization-1.6.1/py_authorization/authorization.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,14 @@
         strategies_to_apply: list[_ApplicableStrategies] = []
 
         if not resources_to_check:
             entities = all_entities_in_statement(query)
             resources_to_check = entities.keys() or []
 
         self.logger.debug("Resources from queries")
-        self.logger.debug(resources_to_check)
 
         self.logger.debug(f"Entities to look for policies: {resources_to_check}")
         for resource_to_access in resources_to_check:
             self.logger.debug(f"Checking Resource: '{resource_to_access}'")
             policy = self._get_policy(
                 user=user,
                 resource_to_access=resource_to_access,
```

### Comparing `py_authorization-1.6.0/py_authorization/policy_strategy.py` & `py_authorization-1.6.1/py_authorization/policy_strategy.py`

 * *Files identical despite different names*

### Comparing `py_authorization-1.6.0/py_authorization/policy_strategy_builder.py` & `py_authorization-1.6.1/py_authorization/policy_strategy_builder.py`

 * *Files identical despite different names*

### Comparing `py_authorization-1.6.0/py_authorization/sql_parser.py` & `py_authorization-1.6.1/py_authorization/sql_parser.py`

 * *Files identical despite different names*

### Comparing `py_authorization-1.6.0/tests/test_authorization.py` & `py_authorization-1.6.1/tests/test_authorization.py`

 * *Files identical despite different names*

### Comparing `py_authorization-1.6.0/tests/test_policy_finder.py` & `py_authorization-1.6.1/tests/test_policy_finder.py`

 * *Files identical despite different names*

