# Comparing `tmp/github_custom_actions-2.0.0.tar.gz` & `tmp/github_custom_actions-2.0.1.tar.gz`

## Comparing `github_custom_actions-2.0.0.tar` & `github_custom_actions-2.0.1.tar`

### file list

```diff
@@ -1,61 +1,69 @@
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/.coveragerc
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/.flake8
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/.mypy.ini
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/.pylintrc
--rwxr-xr-x   0        0        0     1339 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/activate.sh
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/invoke.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/pytest.ini
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/requirements.dev.in
--rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/requirements.dev.txt
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/requirements.in
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/requirements.txt
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/tasks.py
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/.github/workflows/pip_publish.yml
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/.github/workflows/static.yml
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/mkdocs.yml
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/includes/input_output_typed.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/includes/install_pipx_macos.sh
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/includes/quick_start.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/src/en/github_env_vars.md
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/src/en/index.md
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/src/en/inputs.md
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/src/en/installation.md
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/src/en/outputs.md
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/src/en/reference.md
--rw-r--r--   0        0        0    80255 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/src/en/images/var_ide_hover_docstring.jpg
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/src/ru/github_env_vars.md
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/src/ru/index.md
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/src/ru/inputs.md
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/src/ru/installation.md
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/docs/src/ru/outputs.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/scripts/__init__.py
--rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/scripts/build-docs.sh
--rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/scripts/build.sh
--rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/scripts/docs-render-config.sh
--rwxr-xr-x   0        0        0      243 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/scripts/docstrings.sh
--rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/scripts/include_pyproject_requirements.py
--rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/scripts/upload.sh
--rwxr-xr-x   0        0        0     2522 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/scripts/verup.sh
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/src/github_custom_actions/__about__.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/src/github_custom_actions/__init__.py
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/src/github_custom_actions/action_base.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/src/github_custom_actions/attr_dict_vars.py
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/src/github_custom_actions/env_attr_dict_vars.py
--rw-r--r--   0        0        0     4528 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/src/github_custom_actions/file_attr_dict_vars.py
--rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/src/github_custom_actions/github_vars.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/src/github_custom_actions/inputs_outputs.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/tests/conftest.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/tests/test_action_base.py
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/tests/test_env_attr_dict_vars.py
--rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/tests/test_file_attr_dict_vars.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/tests/test_github_custom_actions.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/tests/test_github_vars.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/tests/test_inputs_outputs.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/LICENSE.txt
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/README.md
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 github_custom_actions-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/.coveragerc
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/.flake8
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/.mypy.ini
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/.pylintrc
+-rwxr-xr-x   0        0        0     1339 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/activate.sh
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/invoke.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/pytest.ini
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/requirements.dev.in
+-rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/requirements.dev.txt
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/requirements.in
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/requirements.txt
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/tasks.py
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/.github/workflows/pip_publish.yml
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/.github/workflows/static.yml
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/docs/mkdocs.yml
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/docs/includes/input_output_typed.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/docs/includes/install_pipx_macos.sh
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/docs/includes/quick_start.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/docs/src/en/base.md
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/docs/src/en/github_env_vars.md
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/docs/src/en/index.md
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/docs/src/en/inputs.md
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/docs/src/en/installation.md
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/docs/src/en/main.md
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/docs/src/en/outputs.md
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/docs/src/en/reference.md
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/docs/src/en/render.md
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/docs/src/en/summary.md
+-rw-r--r--   0        0        0    80255 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/docs/src/en/images/var_ide_hover_docstring.jpg
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/docs/src/ru/base.md
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/docs/src/ru/github_env_vars.md
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/docs/src/ru/index.md
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/docs/src/ru/inputs.md
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/docs/src/ru/installation.md
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/docs/src/ru/main.md
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/docs/src/ru/outputs.md
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/docs/src/ru/render.md
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/docs/src/ru/summary.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/scripts/__init__.py
+-rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/scripts/build-docs.sh
+-rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/scripts/build.sh
+-rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/scripts/docs-render-config.sh
+-rwxr-xr-x   0        0        0      243 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/scripts/docstrings.sh
+-rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/scripts/include_pyproject_requirements.py
+-rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/scripts/upload.sh
+-rwxr-xr-x   0        0        0     2522 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/scripts/verup.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/src/github_custom_actions/__about__.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/src/github_custom_actions/__init__.py
+-rw-r--r--   0        0        0     4138 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/src/github_custom_actions/action_base.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/src/github_custom_actions/attr_dict_vars.py
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/src/github_custom_actions/env_attr_dict_vars.py
+-rw-r--r--   0        0        0     4526 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/src/github_custom_actions/file_attr_dict_vars.py
+-rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/src/github_custom_actions/github_vars.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/src/github_custom_actions/inputs_outputs.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/tests/conftest.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/tests/test_action_base.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/tests/test_env_attr_dict_vars.py
+-rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/tests/test_file_attr_dict_vars.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/tests/test_github_custom_actions.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/tests/test_github_vars.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/tests/test_inputs_outputs.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/README.md
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 github_custom_actions-2.0.1/PKG-INFO
```

### Comparing `github_custom_actions-2.0.0/.pre-commit-config.yaml` & `github_custom_actions-2.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-2.0.0/activate.sh` & `github_custom_actions-2.0.1/activate.sh`

 * *Files identical despite different names*

### Comparing `github_custom_actions-2.0.0/requirements.dev.txt` & `github_custom_actions-2.0.1/requirements.dev.txt`

 * *Files identical despite different names*

### Comparing `github_custom_actions-2.0.0/tasks.py` & `github_custom_actions-2.0.1/tasks.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-2.0.0/.github/workflows/ci.yml` & `github_custom_actions-2.0.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-2.0.0/.github/workflows/docs.yml` & `github_custom_actions-2.0.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-2.0.0/.github/workflows/pip_publish.yml` & `github_custom_actions-2.0.1/.github/workflows/pip_publish.yml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-2.0.0/.github/workflows/static.yml` & `github_custom_actions-2.0.1/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-2.0.0/docs/mkdocs.yml` & `github_custom_actions-2.0.1/docs/mkdocs.yml`

 * *Files 3% similar despite different names*

```diff
@@ -9,17 +9,21 @@
 edit_uri: edit/master/docs
 docs_dir: 'src/LANGUAGE'
 site_dir: '../site/SITE_PREFIX'
 
 nav:
   - index.md
   - installation.md
+  - base.md
   - inputs.md
   - outputs.md
   - github_env_vars.md
+  - main.md
+  - summary.md
+  - render.md
 
 plugins:
   - awesome-pages
   - search:
       lang: LANGUAGE
   - mkdocstrings:
       handlers:
```

### Comparing `github_custom_actions-2.0.0/docs/includes/input_output_typed.py` & `github_custom_actions-2.0.1/docs/includes/input_output_typed.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-2.0.0/docs/src/en/github_env_vars.md` & `github_custom_actions-2.0.1/docs/src/en/github_env_vars.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Github variables 
+
 In the `vars` attribute of the action class, you can access all the environment variables provided by GitHub.
 
 The library provides a full list of 
 [GitHub environment variables](https://docs.github.com/en/actions/learn-github-actions/variables#default-environment-variables), 
 including descriptions.
 
 Paths and files have type Path.
```

### Comparing `github_custom_actions-2.0.0/docs/src/en/index.md` & `github_custom_actions-2.0.1/docs/src/en/index.md`

 * *Files 18% similar despite different names*

```diff
@@ -7,42 +7,43 @@
 
 ### Quick start
 
 ```python
 --8<-- "quick_start.py"
 ```
 
-This example uses the `runner_os` variable from GitHub environment variables. 
+This example uses the [runner_os][github_custom_actions.GithubVars.runner_os] 
+variable from 
+[GitHub environment variables][github_custom_actions.GithubVars]. 
 All variables from the GitHub environment are available in the `env`, 
 with descriptions shown in your IDE on mouse hover:
 ![var_ide_hover_docstring.jpg](images/var_ide_hover_docstring.jpg)
 
-The action gets a value from the `my-input` action input and renders 
-it in the action step summary on the GitHub build summary.
+The action gets a value from the `my-input` [action input](inputs) and renders 
+it in the action [step summary](summary) on the GitHub build summary.
 
-It also returns a value to the `runner-os` action output.
+It also returns a value to the `runner-os` [action output](outputs).
 
-The main block runs the `main()` method of the action with the necessary boilerplate 
-to catch and report exceptions.
+The `run()` in the main block runs the [main()](main) that implements your action.
 
 ### Explicitly defined inputs and outputs
 
 With explicitly defined inputs and outputs, you can use typo-checked code autocompletion:
 
 ```python
 --8<-- "input_output_typed.py"
 ```
 
 Note that you only define the types of inputs and outputs, and instances are created automatically
-upon `MyAction` initialization.
+upon [ActionBase](base) initialization.
 
 Now you can utilize the attributes defined in the `inputs` and `outputs` classes of the action. 
 All attributes names are converted to `kebab-case`, allowing dot notation like `inputs.my_input`
 to replace the `inputs['my-input']`.
 
 Inputs defined as Path will be converted to `Path` objects.
 
 But still can use the `inputs['my-input']` style if you prefer.
 
 ### Example of usage
 
-[Allure Test Report Action](hhttps://github.com/andgineer/allure-report/blob/main/src/allure_generate.py)
+[Allure Test Report Action](https://github.com/andgineer/allure-report/blob/main/src/allure_generate.py)
```

### Comparing `github_custom_actions-2.0.0/docs/src/en/installation.md` & `github_custom_actions-2.0.1/docs/src/en/installation.md`

 * *Files identical despite different names*

### Comparing `github_custom_actions-2.0.0/docs/src/en/images/var_ide_hover_docstring.jpg` & `github_custom_actions-2.0.1/docs/src/en/images/var_ide_hover_docstring.jpg`

 * *Files identical despite different names*

### Comparing `github_custom_actions-2.0.0/docs/src/ru/github_env_vars.md` & `github_custom_actions-2.0.1/docs/src/ru/github_env_vars.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Переменные окружения GitHub
+
 В атрибуте `env` класса действия вы можете получить доступ ко всем переменным окружения, предоставляемым GitHub.
 
 Библиотека предоставляет полный список 
 [переменных окружения GitHub](https://docs.github.com/en/actions/learn-github-actions/variables#default-environment-variables), 
 включая описания.
 
 Пути и файлы имеют тип `Path`.
```

### Comparing `github_custom_actions-2.0.0/docs/src/ru/index.md` & `github_custom_actions-2.0.1/docs/src/ru/index.md`

 * *Files 7% similar despite different names*

```diff
@@ -7,37 +7,38 @@
 
 ### Быстрый старт
 
 ```python
 --8<-- "quick_start.py"
 ```
 
-Этот пример использует переменную `runner_os` из переменных окружения GitHub. 
+Этот пример использует переменную [runner_os][github_custom_actions.GithubVars.runner_os] из 
+[переменных окружения GitHub][runner_os][github_custom_actions.GithubVars]. 
 
 Все переменные из окружения GitHub доступны в `env`, 
 описания которых отображаются в вашей IDE при наведении мыши:
 ![var_ide_hover_docstring.jpg](images/var_ide_hover_docstring.jpg)
 
-Action получает значение из action input `my-input` и отображает его 
-в `step summary` на странице билда GitHub.
+Action получает значение из [action input](inputs) `my-input` и отображает его 
+в [step summary](summary) на странице билда GitHub.
 
-Оно также возвращает значение в action output `runner-os`.
+Оно также возвращает значение в [action output](outputs) `runner-os`.
 
-Основной блок запускает метод `main()` действия с необходимым кодом для перехвата и обработки исключений.
+`run()` в основном блоке запускает метод [main()](main) реализующий вашу Github action.
 
 ### Явно определенные входы и выходы
 
 С явно определенными входами и выходами вы можете использовать автодополнение кода с проверкой на опечатки:
 
 ```python
 --8<-- "input_output_typed.py"
 ```
 
 Обратите внимание, что вы только определяете типы входов и выходов, а экземпляры этих классов создаются автоматически
-при инициализации `MyAction`.
+при инициализации [ActionBase](base).
 
 Теперь вы можете использовать атрибуты, определенные в классах `inputs` и `outputs` действия. 
 Все имена атрибутов преобразуются в `kebab-case`, что позволяет использовать точечную нотацию, например `inputs.my_input`, 
 вместо `inputs['my-input']`.
 
 Если вы определили input как `Path`, он будет преобразован в объект `Path`.
```

### Comparing `github_custom_actions-2.0.0/docs/src/ru/inputs.md` & `github_custom_actions-2.0.1/docs/src/ru/inputs.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,28 @@
-# inputs вашей GitHub Action
-
-Входящие параметры описываются в наследнике 
-[class ActionInputs][github_custom_actions.ActionInputs]
-
-Если вы не создаете наследника, то можете получать входные параметры в стиле словаря.
-Описав же наследника вы получите все преимущества автодополнения и проверки типов.
+Входные переменные GitHub Action (inputs)
 
+Использование:
 ```python
 class MyInputs(ActionInputs):
     my_input: str
 
 action = ActionBase(inputs=MyInputs())
 print(action.inputs.my_input)
-print(action.inputs["my-input"])  # the same as above
+print(action.inputs["my-input"])  # то же самое, что и выше
 ```
 
+Имена атрибутов преобразуются в `kebab-case`.
+Таким образом, `action.inputs.my_input` тоже самое, что и `action.inputs["my-input"]`.
 
-Имена атрибутов преобразуются в `kebab-case`. 
-Таким образом, `action.inputs.my_input` то же самое, что и `action.inputs["my-input"]`.
-
-Если вам нужно получить доступ к входной переменной `my_input`, записанной в `snake_case`, 
-вы должны использовать только доступ через словарь: `action.inputs["my_input"]`. 
-Однако обычно в GitHub Actions имена входных переменных используют `kebab-case`.
-
-По соглашению GitHub, все имена входных переменных для передачи через окружение преобразуются 
-в верхний регистр с добавлением префикса "INPUT_". 
-
-Таким образом, вход `actions.inputs.my_input` или `actions.inputs['my-input']` будет переменной `INPUT_MY-INPUT` в окружении. 
-[ActionInputs][github_custom_actions.ActionInputs] автоматически выполняет преобразование.
-Благодаря этому используя стиль словаря вы можете использовать обращаться к любым переменным окружения,
-в том числе не описанным в атрибутах класса.
-
-Используется ленивая загрузка значений. 
-Таким образом, значение считывается из окружения, только когда оно запрашивается, и только один раз,
-после чего запоминается во внутреннем словаре объекта.
+Если вам нужно получить доступ к входному параметру с именем в `snake_case` `my_input`, вы должны
+использовать стиль словаря: `action.inputs["my_input"]`.
+Но обычно в GitHub Actions имена входных данных используются в `kebab-case`.
+
+По соглашению GitHub все имена входных данных преобразуются в верхний регистр в окружении и имеют 
+префикс "INPUT_".
+Таким образом, `actions.inputs.my_input` или `actions.inputs['my-input']` будет переменной 
+`INPUT_MY-INPUT` в окружении.
+ActionInputs автоматически выполняет преобразование.
+
+Использует ленивую загрузку значений.
+Таким образом, значение считывается из окружения только при доступе к нему и только один раз, 
+и сохраняется во внутреннем словаре объекта.
```

### Comparing `github_custom_actions-2.0.0/docs/src/ru/installation.md` & `github_custom_actions-2.0.1/docs/src/ru/installation.md`

 * *Files identical despite different names*

### Comparing `github_custom_actions-2.0.0/docs/src/ru/outputs.md` & `github_custom_actions-2.0.1/docs/src/ru/outputs.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-# outputs вашей GitHub Action
-
-Выходящие параметры описываются в наследнике 
-[class ActionOutputs][github_custom_actions.ActionOutputs]
-
-Если вы не создаете наследника, то можете получать выходные параметры в стиле словаря.
-Описав же наследника вы получите все преимущества автодополнения и проверки типов.
+Выходные переменные GitHub Action (outputs)
 
+Использование:
 ```python
 class MyOutputs(ActionOutputs):
-    my_output: str
+   my_output: str
 
 action = ActionBase(outputs=MyOutputs())
 action.outputs["my-output"] = "value"
-action.outputs.my_output = "value"  # the same as above
+action.outputs.my_output = "value"  # то же самое, что выше
 ```
 
-Имена атрибутов преобразуются в `kebab-case`. 
-Таким образом, `action.outputs.my_output` эквивалентен `action.outputs["my-output"]`.
-
-Если вам нужно получить доступ к выходным данным с именем в snake_case `my_output`, 
-следует использовать только стиль словаря: `action.outputs["my-output"]`. 
-Но обычно в именах выходных данных GitHub Actions используется kebab-case.
+С атрибутами можно обращаться только к явно объявленным переменным,
+с помощью доступа, подобного словарю, можно обратиться к любой переменной.
+Таким образом, вы можете найти баланс между строго определёнными переменными и гибкостью.
+
+Имена атрибутов преобразуются в `kebab-case`.
+Так что `action.outputs.my_output` тоже самое, что и `action.outputs["my-output"]`.
+
+Если вам нужно обратиться к выходной переменной с именем в `snake_case`, например `my_output`,
+следует использовать только стиль словаря: `action.outputs["my_output"]`.
+Но обычно в именах выходных данных GitHub Actions используется `kebab-case`.
 
-Каждое присваивание переменных выводов изменяет файл выводов Github 
-(путь определяется переменной Github `action.env.github_output`).
+Каждое присвоение выходной переменной изменяет файл выходных данных GitHub
+(путь определяется как `action.env.github_output`).
```

### Comparing `github_custom_actions-2.0.0/scripts/include_pyproject_requirements.py` & `github_custom_actions-2.0.1/scripts/include_pyproject_requirements.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-2.0.0/scripts/verup.sh` & `github_custom_actions-2.0.1/scripts/verup.sh`

 * *Files identical despite different names*

### Comparing `github_custom_actions-2.0.0/src/github_custom_actions/attr_dict_vars.py` & `github_custom_actions-2.0.1/src/github_custom_actions/attr_dict_vars.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-2.0.0/src/github_custom_actions/env_attr_dict_vars.py` & `github_custom_actions-2.0.1/src/github_custom_actions/env_attr_dict_vars.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,32 @@
 from github_custom_actions.attr_dict_vars import AttrDictVars
 
 
 class EnvAttrDictVars(AttrDictVars):
     """Dual access env vars.
 
     Access to env vars as object attributes or as dict items.
-    Do not allow to change vars so this is read-only source of env vars values.
+    Do not allow changing vars, so this is a read-only source of env vars values.
 
-    With attributes, you can only access explicitly declared vars, with dict - any.
+    With attributes, you can only access explicitly declared vars,
+    with dict-like access you can access any var.
     This way you can find your balance between strictly defined vars and flexibility.
 
     Usage:
-        class MyVars(EnvAttrDictVars):
-            documented_var: str
+       ```python
+       class MyVars(EnvAttrDictVars):
+           documented_var: str
+
+       vars = MyVars(prefix="INPUT_")
+       print(vars["undocumented_var"])  # from os.environ["INPUT_UNDOCUMENTED_VAR"]
+       print(vars.documented_var)  # from os.environ["INPUT_DOCUMENTED-VAR"]
+       ```
 
-        vars = MyVars(prefix="INPUT_")
-        print(vars["undocumented_var"])  # from os.environ["INPUT_UNDOCUMENTED_VAR"]
-        print(vars.documented_var)  # from os.environ["INPUT_DOCUMENTED-VAR"]
-
-    Attribute names converted with method `_attr_to_var_name()` - it converts python attribute
-    name from snake_case to kebab-case.
+    Attribute names are converted with the method `_attr_to_var_name()` - it converts Python attribute
+    names from snake_case to kebab-case.
     """
 
     def __getattribute__(self, name: str) -> Any:
         try:
             return super().__getattribute__(name)
         except AttributeError as exc:
             type_hints = self.__class__._get_type_hints()
```

### Comparing `github_custom_actions-2.0.0/src/github_custom_actions/file_attr_dict_vars.py` & `github_custom_actions-2.0.1/src/github_custom_actions/file_attr_dict_vars.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,36 +5,37 @@
 
 
 class FileAttrDictVars(AttrDictVars, MutableMapping):  # type: ignore
     """Dual access vars in a file.
 
     File contains vars as `key=value` lines.
     Access with attributes or as dict.
-    With attributes, you can only access explicitly declared vars, with dict-like access you can access any var.
+
+    With attributes, you can only access explicitly declared vars,
+    with dict-like access you can access any var.
     This way you can find your balance between strictly defined vars and flexibility.
 
     Usage:
-        class MyVars(FileAttrDictVars):
-            documented_var: str
+       class MyVars(FileAttrDictVars):
+           documented_var: str
 
-        vars = MyVars(Path("my_vars.txt"))
-        vars["undocumented_var"] = "value1"
-        vars.documented_var == "value2"
+       vars = MyVars(Path("my_vars.txt"))
+       vars["undocumented_var"] = "value1"
+       vars.documented_var == "value2"
 
-        # Produce "my_vars.txt" with:
-        #    documented-var=value1
-        #    undocumented_var=value2
+       # Produces "my_vars.txt" with:
+       #    documented-var=value2
+       #    undocumented_var=value1
 
 
-    On read / write converts var names with `_name_from_external()` / `_external_name()` methods.
-    They remove / add `_external_name_prefix` to the names.
+    On read/write, it converts var names with `_name_from_external()`/`_external_name()` methods.
+    They remove/add `_external_name_prefix` to the names.
 
-    Attribute access also do `_attr_to_var_name()` - by default it converts python attribute name
+    Attribute access also uses `_attr_to_var_name()` - by default it converts Python attribute names
     from snake_case to kebab-case.
-
     """
 
     def __init__(self, vars_file: Path, *, prefix: str = "") -> None:
         """Init the vars file and prefix."""
         self._external_name_prefix = prefix
         self._vars_file: Path = vars_file
         self._var_keys_cache: Optional[Dict[str, str]] = None
```

### Comparing `github_custom_actions-2.0.0/src/github_custom_actions/github_vars.py` & `github_custom_actions-2.0.1/src/github_custom_actions/github_vars.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-2.0.0/src/github_custom_actions/inputs_outputs.py` & `github_custom_actions-2.0.1/src/github_custom_actions/inputs_outputs.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,54 +22,63 @@
             my_input: str
 
         action = ActionBase(inputs=MyInputs())
         print(action.inputs.my_input)
         print(action.inputs["my-input"])  # the same as above
         ```
 
-    Attribute names converted to `kebab-case`.
+    With attributes, you can only access explicitly declared vars, with dict-like access you can access any var.
+    This way you can find your balance between strictly defined vars and flexibility.
+
+    Attribute names are converted to `kebab-case`.
     So `action.inputs.my_input` is the same as `action.inputs["my-input"]`.
 
-    If you need to access `snake_case` named input `my_input` you should
+    If you need to access a `snake_case` named input `my_input`, you should
     use dict-style only: `action.inputs["my_input"]`.
-    But it's common to use `kebab-case` in GitHub Actions inputs names.
+    But it's common to use `kebab-case` in GitHub Actions input names.
 
-    By github convention all input names are upper-cased in environment and prefixed with "INPUT_".
-    So `actions.inputs.my_input` or `actions.inputs['my-input']` will be variable `INPUT_MY-INPUT` in environment.
+    By GitHub convention, all input names are upper-cased in the environment and prefixed with "INPUT_".
+    So `actions.inputs.my_input` or `actions.inputs['my-input']` will be the variable `INPUT_MY-INPUT`
+    in the environment.
     The ActionInputs does the conversion automatically.
 
-    Use lazy loading of the values.
-    So the value is read from environment only when accessed and only once, and saved in the object internal dict.
-    """
+    Uses lazy loading of the values.
+    So the value is read from the environment only when accessed and only once,
+    and saved in the object's internal dict."""
 
     # pylint: disable=abstract-method  # we want RO implementation that raises NotImplementedError on write
 
     def _external_name(self, name: str) -> str:
         """Convert variable name to the external form."""
         return INPUT_PREFIX + name.upper()
 
 
 class ActionOutputs(FileAttrDictVars):
     """GitHub Actions output variables.
 
     Usage:
-        ```python
-        class MyOutputs(ActionOutputs):
-            my_output: str
-
-        action = ActionBase(outputs=MyOutputs())
-        action.outputs["my-output"] = "value"
-        action.outputs.my_output = "value"  # the same as above
-        ```
+       ```python
+       class MyOutputs(ActionOutputs):
+           my_output: str
+
+       action = ActionBase(outputs=MyOutputs())
+       action.outputs["my-output"] = "value"
+       action.outputs.my_output = "value"  # the same as above
+       ```
+
+    With attributes, you can only access explicitly declared vars,
+    with dict-like access you can access any var.
+    This way you can find your balance between strictly defined vars and flexibility.
 
-    Attribute names converted to `kebab-case`.
+    Attribute names are converted to `kebab-case`.
     So `action.outputs.my_output` is the same as `action.outputs["my-output"]`.
 
-    If you need to access `snake_case` named output `my_output` you should
-    use dict-style only: `action.outputs["my-output"]`.
-    But it's common to use `kebab-case` in GitHub Actions outputs names.
+    If you need to access a `snake_case` named output like `my_output` you should
+    use dict-style only: `action.outputs["my_output"]`.
+    But it's common to use `kebab-case` in GitHub Actions output names.
 
-    Each outputs vars assignment change the Github outputs file (the path is defined as `action.env.github_output`).
+    Each output var assignment changes the GitHub outputs file
+    (the path is defined as `action.env.github_output`).
     """
 
     def __init__(self) -> None:
         super().__init__(Path(os.environ["GITHUB_OUTPUT"]))
```

### Comparing `github_custom_actions-2.0.0/tests/conftest.py` & `github_custom_actions-2.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-2.0.0/tests/test_env_attr_dict_vars.py` & `github_custom_actions-2.0.1/tests/test_env_attr_dict_vars.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-2.0.0/tests/test_file_attr_dict_vars.py` & `github_custom_actions-2.0.1/tests/test_file_attr_dict_vars.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-2.0.0/tests/test_github_vars.py` & `github_custom_actions-2.0.1/tests/test_github_vars.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-2.0.0/tests/test_inputs_outputs.py` & `github_custom_actions-2.0.1/tests/test_inputs_outputs.py`

 * *Files identical despite different names*

### Comparing `github_custom_actions-2.0.0/LICENSE.txt` & `github_custom_actions-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `github_custom_actions-2.0.0/README.md` & `github_custom_actions-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `github_custom_actions-2.0.0/pyproject.toml` & `github_custom_actions-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `github_custom_actions-2.0.0/PKG-INFO` & `github_custom_actions-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: github-custom-actions
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python package for creating custom GitHub Actions.
 Project-URL: Homepage, https://andgineer.github.io/github-custom-actions/
 Project-URL: Documentation, https://andgineer.github.io/github-custom-actions/
 Author-email: Andrey Sorokin <andrey@sorokin.engineer>
 License: Copyright (c) 2024 Andrey Sorokin <andrey@sorokin.engineer>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

