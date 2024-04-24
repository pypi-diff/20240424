# Comparing `tmp/nautobot_plugin_nornir-2.0.0.tar.gz` & `tmp/nautobot_plugin_nornir-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_plugin_nornir-2.0.0.tar", max compression
+gzip compressed data, was "nautobot_plugin_nornir-2.0.1.tar", max compression
```

## Comparing `nautobot_plugin_nornir-2.0.0.tar` & `nautobot_plugin_nornir-2.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      591 2023-10-01 22:31:07.004213 nautobot_plugin_nornir-2.0.0/LICENSE
--rw-r--r--   0        0        0     4629 2023-10-01 22:31:07.004213 nautobot_plugin_nornir-2.0.0/README.md
--rw-r--r--   0        0        0     3553 2023-10-01 22:31:07.012213 nautobot_plugin_nornir-2.0.0/nautobot_plugin_nornir/__init__.py
--rw-r--r--   0        0        0      862 2023-10-01 22:31:07.012213 nautobot_plugin_nornir-2.0.0/nautobot_plugin_nornir/constants.py
--rw-r--r--   0        0        0       29 2023-10-01 22:31:07.012213 nautobot_plugin_nornir-2.0.0/nautobot_plugin_nornir/plugins/__init__.py
--rw-r--r--   0        0        0       33 2023-10-01 22:31:07.012213 nautobot_plugin_nornir-2.0.0/nautobot_plugin_nornir/plugins/credentials/__init__.py
--rw-r--r--   0        0        0     1210 2023-10-01 22:31:07.012213 nautobot_plugin_nornir-2.0.0/nautobot_plugin_nornir/plugins/credentials/env_vars.py
--rw-r--r--   0        0        0     1409 2023-10-01 22:31:07.012213 nautobot_plugin_nornir-2.0.0/nautobot_plugin_nornir/plugins/credentials/nautobot_orm.py
--rw-r--r--   0        0        0     2396 2023-10-01 22:31:07.012213 nautobot_plugin_nornir-2.0.0/nautobot_plugin_nornir/plugins/credentials/nautobot_secrets.py
--rw-r--r--   0        0        0     1078 2023-10-01 22:31:07.012213 nautobot_plugin_nornir-2.0.0/nautobot_plugin_nornir/plugins/credentials/settings_vars.py
--rw-r--r--   0        0        0       45 2023-10-01 22:31:07.012213 nautobot_plugin_nornir-2.0.0/nautobot_plugin_nornir/plugins/inventory/__init__.py
--rw-r--r--   0        0        0    12468 2023-10-01 22:31:07.012213 nautobot_plugin_nornir-2.0.0/nautobot_plugin_nornir/plugins/inventory/nautobot_orm.py
--rw-r--r--   0        0        0       45 2023-10-01 22:31:07.012213 nautobot_plugin_nornir-2.0.0/nautobot_plugin_nornir/tests/__init__.py
--rw-r--r--   0        0        0     1041 2023-10-01 22:31:07.012213 nautobot_plugin_nornir-2.0.0/nautobot_plugin_nornir/tests/test_basic.py
--rw-r--r--   0        0        0     4846 2023-10-01 22:31:07.012213 nautobot_plugin_nornir-2.0.0/nautobot_plugin_nornir/tests/test_nautobot_orm.py
--rw-r--r--   0        0        0      393 2023-10-01 22:31:07.012213 nautobot_plugin_nornir-2.0.0/nautobot_plugin_nornir/utils.py
--rw-r--r--   0        0        0     3698 2023-10-01 22:31:17.116277 nautobot_plugin_nornir-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     5829 1970-01-01 00:00:00.000000 nautobot_plugin_nornir-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      591 2024-03-12 16:48:05.796743 nautobot_plugin_nornir-2.0.1/LICENSE
+-rw-r--r--   0        0        0     4629 2024-03-12 16:48:05.796743 nautobot_plugin_nornir-2.0.1/README.md
+-rw-r--r--   0        0        0     3695 2024-03-12 16:48:05.804743 nautobot_plugin_nornir-2.0.1/nautobot_plugin_nornir/__init__.py
+-rw-r--r--   0        0        0      862 2024-03-12 16:48:05.804743 nautobot_plugin_nornir-2.0.1/nautobot_plugin_nornir/constants.py
+-rw-r--r--   0        0        0       29 2024-03-12 16:48:05.804743 nautobot_plugin_nornir-2.0.1/nautobot_plugin_nornir/plugins/__init__.py
+-rw-r--r--   0        0        0       33 2024-03-12 16:48:05.804743 nautobot_plugin_nornir-2.0.1/nautobot_plugin_nornir/plugins/credentials/__init__.py
+-rw-r--r--   0        0        0     1210 2024-03-12 16:48:05.804743 nautobot_plugin_nornir-2.0.1/nautobot_plugin_nornir/plugins/credentials/env_vars.py
+-rw-r--r--   0        0        0     1409 2024-03-12 16:48:05.804743 nautobot_plugin_nornir-2.0.1/nautobot_plugin_nornir/plugins/credentials/nautobot_orm.py
+-rw-r--r--   0        0        0     6055 2024-03-12 16:48:05.804743 nautobot_plugin_nornir-2.0.1/nautobot_plugin_nornir/plugins/credentials/nautobot_secrets.py
+-rw-r--r--   0        0        0     1078 2024-03-12 16:48:05.804743 nautobot_plugin_nornir-2.0.1/nautobot_plugin_nornir/plugins/credentials/settings_vars.py
+-rw-r--r--   0        0        0       45 2024-03-12 16:48:05.804743 nautobot_plugin_nornir-2.0.1/nautobot_plugin_nornir/plugins/inventory/__init__.py
+-rw-r--r--   0        0        0    12468 2024-03-12 16:48:05.804743 nautobot_plugin_nornir-2.0.1/nautobot_plugin_nornir/plugins/inventory/nautobot_orm.py
+-rw-r--r--   0        0        0       52 2024-03-12 16:48:05.804743 nautobot_plugin_nornir-2.0.1/nautobot_plugin_nornir/tests/__init__.py
+-rw-r--r--   0        0        0     1041 2024-03-12 16:48:05.804743 nautobot_plugin_nornir-2.0.1/nautobot_plugin_nornir/tests/test_basic.py
+-rw-r--r--   0        0        0     4846 2024-03-12 16:48:05.804743 nautobot_plugin_nornir-2.0.1/nautobot_plugin_nornir/tests/test_nautobot_orm.py
+-rw-r--r--   0        0        0      393 2024-03-12 16:48:05.804743 nautobot_plugin_nornir-2.0.1/nautobot_plugin_nornir/utils.py
+-rw-r--r--   0        0        0     3538 2024-03-12 16:48:13.816686 nautobot_plugin_nornir-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5782 1970-01-01 00:00:00.000000 nautobot_plugin_nornir-2.0.1/PKG-INFO
```

### Comparing `nautobot_plugin_nornir-2.0.0/LICENSE` & `nautobot_plugin_nornir-2.0.1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Apache Software License 2.0
 
-Copyright (c) 2021, Network to Code, LLC
+Copyright (c) 2023, Network to Code, LLC
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
 http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `nautobot_plugin_nornir-2.0.0/README.md` & `nautobot_plugin_nornir-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `nautobot_plugin_nornir-2.0.0/nautobot_plugin_nornir/__init__.py` & `nautobot_plugin_nornir-2.0.1/nautobot_plugin_nornir/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """Plugin declaration for nautobot_plugin_nornir."""
-
+# Metadata is inherited from Nautobot. If not including Nautobot in the environment, this should be added
 from importlib import metadata
 
-
 __version__ = metadata.version(__name__)
 
-from nautobot.extras.plugins import PluginConfig
+from nautobot.extras.plugins import NautobotAppConfig
 from nautobot_plugin_nornir.utils import verify_setting
 
 
-class NornirConfig(PluginConfig):
+class NautobotPluginNornirConfig(NautobotAppConfig):
     """Plugin configuration for nautobot_plugin_nornir."""
 
     name = "nautobot_plugin_nornir"
     verbose_name = "Nautobot Plugin for Nornir"
     version = __version__
     author = "Network to Code, LLC"
     description = (
@@ -65,8 +64,8 @@
         # verify_setting(plugin_settings, "nornir_settings.password", "The `password` key should NOT be within the `nornir_settings` dictionary")
         # verify_setting(plugin_settings, "nornir_settings.secret", "The `secret` key should NOT be within the `nornir_settings` dictionary")
         # verify_setting(plugin_settings, "nornir_settings.connection_secret_path", "The `connection_secret_path` key should NOT be within the `nornir_settings` dictionary")
         # verify_setting(plugin_settings, "nornir_settings.secret_access_type", "The `secret_access_type` key should NOT be within the `nornir_settings` dictionary")
         super().ready()
 
 
-config = NornirConfig  # pylint:disable=invalid-name
+config = NautobotPluginNornirConfig  # pylint:disable=invalid-name
```

### Comparing `nautobot_plugin_nornir-2.0.0/nautobot_plugin_nornir/constants.py` & `nautobot_plugin_nornir-2.0.1/nautobot_plugin_nornir/constants.py`

 * *Files identical despite different names*

### Comparing `nautobot_plugin_nornir-2.0.0/nautobot_plugin_nornir/plugins/credentials/env_vars.py` & `nautobot_plugin_nornir-2.0.1/nautobot_plugin_nornir/plugins/credentials/env_vars.py`

 * *Files identical despite different names*

### Comparing `nautobot_plugin_nornir-2.0.0/nautobot_plugin_nornir/plugins/credentials/nautobot_orm.py` & `nautobot_plugin_nornir-2.0.1/nautobot_plugin_nornir/plugins/credentials/nautobot_orm.py`

 * *Files identical despite different names*

### Comparing `nautobot_plugin_nornir-2.0.0/nautobot_plugin_nornir/plugins/credentials/settings_vars.py` & `nautobot_plugin_nornir-2.0.1/nautobot_plugin_nornir/plugins/credentials/settings_vars.py`

 * *Files identical despite different names*

### Comparing `nautobot_plugin_nornir-2.0.0/nautobot_plugin_nornir/plugins/inventory/nautobot_orm.py` & `nautobot_plugin_nornir-2.0.1/nautobot_plugin_nornir/plugins/inventory/nautobot_orm.py`

 * *Files identical despite different names*

### Comparing `nautobot_plugin_nornir-2.0.0/nautobot_plugin_nornir/tests/test_basic.py` & `nautobot_plugin_nornir-2.0.1/nautobot_plugin_nornir/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `nautobot_plugin_nornir-2.0.0/nautobot_plugin_nornir/tests/test_nautobot_orm.py` & `nautobot_plugin_nornir-2.0.1/nautobot_plugin_nornir/tests/test_nautobot_orm.py`

 * *Files identical despite different names*

### Comparing `nautobot_plugin_nornir-2.0.0/pyproject.toml` & `nautobot_plugin_nornir-2.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,76 +1,73 @@
 [tool.poetry]
 name = "nautobot-plugin-nornir"
-version = "v2.0.0"
+version = "v2.0.1"
 description = "Nautobot Nornir plugin."
 authors = ["Network to Code, LLC <info@networktocode.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/nautobot/nautobot-plugin-nornir"
 repository = "https://github.com/nautobot/nautobot-plugin-nornir"
 keywords = ["nautobot", "nautobot-plugin"]
-include = [
-    "LICENSE",
-    "README.md",
-]
 classifiers = [
     "Intended Audience :: Developers",
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
+include = [
+    "LICENSE",
+    "README.md",
+]
 packages = [
     { include = "nautobot_plugin_nornir" },
 ]
 
 [tool.poetry.urls]
 "Changelog" = "https://docs.nautobot.com/projects/plugin-nornir/en/latest/admin/release_notes/"
 "Bug Tracker" = "https://github.com/nautobot/nautobot-plugin-nornir/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
+# Used for local development
 nautobot = "^2.0.0"
 nornir-nautobot = "^3.0.0"
 netutils = ">=1.6.0"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "*"
 black = "*"
 coverage = "*"
 django-debug-toolbar = "*"
-# we need to pin flake8 because of package dependencies that cause it to downgrade and
-# therefore cause issues with linting since older versions do not take .flake8 as config
-flake8 = "^3.9.2"
+flake8 = "*"
 invoke = "*"
 ipython = "*"
 pydocstyle = "*"
 pylint = "*"
 pylint-django = "*"
 pylint-nautobot = "*"
-pytest = "*"
 yamllint = "*"
-Markdown = "*"
 toml = "*"
+Markdown = "*"
 # Rendering docs to HTML
 mkdocs = "1.5.2"
 # Material for MkDocs theme
 mkdocs-material = "9.2.4"
+# Render custom markdown for version added/changed/remove notes
+mkdocs-version-annotations = "1.0.0"
 # Automatic documentation from sources, for MkDocs
 mkdocstrings = "0.22.0"
 mkdocstrings-python = "1.5.2"
 
-[tool.poetry.extras]
-nautobot = ["nautobot"]
-
 [tool.black]
 line-length = 120
-target-version = ['py37']
+target-version = ['py38', 'py39', 'py310', 'py311']
 include = '\.pyi?$'
 exclude = '''
 (
   /(
       \.eggs         # exclude a few common directories in the
     | \.git          # root of the project
     | \.hg
@@ -85,15 +82,15 @@
   | settings.py     # This is where you define files that should not be stylized by black
                      # the root of the project
 )
 '''
 
 [tool.pylint.master]
 # Include the pylint_django plugin to avoid spurious warnings about Django patterns
-load-plugins="pylint_django,pylint_nautobot"
+load-plugins="pylint_django, pylint_nautobot"
 ignore=".venv"
 
 [tool.pylint.basic]
 # No docstrings required for private methods (Pylint default), or for test_ functions, or for inner Meta classes.
 no-docstring-rgx="^(_|test_|Meta$)"
 
 [tool.pylint.messages_control]
@@ -106,14 +103,19 @@
 [tool.pylint.miscellaneous]
 # Don't flag TODO as a failure, let us commit with things that still need to be done in the code
 notes = """,
     FIXME,
     XXX,
     """
 
+[tool.pylint-nautobot]
+supported_nautobot_versions = [
+    "2.0.0"
+]
+
 [tool.pydocstyle]
 convention = "google"
 inherit = false
 match = "(?!__init__).*\\.py"
 match-dir = "(?!tests|migrations|development)[^\\.].*"
 # D212 is enabled by default in google convention, and complains if we have a docstring like:
 # """
@@ -121,15 +123,7 @@
 # """
 # We've discussed and concluded that we consider this to be a valid style choice.
 add_ignore = "D212"
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
-
-[tool.pytest.ini_options]
-testpaths = [
-    "tests"
-]
-addopts = "-vv --doctest-modules"
-[tool.pylint-nautobot]
-supported_nautobot_versions = ["2"]
```

### Comparing `nautobot_plugin_nornir-2.0.0/PKG-INFO` & `nautobot_plugin_nornir-2.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautobot-plugin-nornir
-Version: 2.0.0
+Version: 2.0.1
 Summary: Nautobot Nornir plugin.
 Home-page: https://github.com/nautobot/nautobot-plugin-nornir
 License: Apache-2.0
 Keywords: nautobot,nautobot-plugin
 Author: Network to Code, LLC
 Author-email: info@networktocode.com
 Requires-Python: >=3.8,<3.12
@@ -12,16 +12,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: nautobot
-Requires-Dist: nautobot (>=2.0.0,<3.0.0) ; extra == "nautobot"
+Requires-Dist: nautobot (>=2.0.0,<3.0.0)
 Requires-Dist: netutils (>=1.6.0)
 Requires-Dist: nornir-nautobot (>=3.0.0,<4.0.0)
 Project-URL: Bug Tracker, https://github.com/nautobot/nautobot-plugin-nornir/issues
 Project-URL: Changelog, https://docs.nautobot.com/projects/plugin-nornir/en/latest/admin/release_notes/
 Project-URL: Repository, https://github.com/nautobot/nautobot-plugin-nornir
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: nautobot-plugin-nornir Version: 2.0.0 Summary:
+Metadata-Version: 2.1 Name: nautobot-plugin-nornir Version: 2.0.1 Summary:
 Nautobot Nornir plugin. Home-page: https://github.com/nautobot/nautobot-plugin-
 nornir License: Apache-2.0 Keywords: nautobot,nautobot-plugin Author: Network
 to Code, LLC Author-email: info@networktocode.com Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Provides-Extra: nautobot Requires-Dist: nautobot
-(>=2.0.0,<3.0.0) ; extra == "nautobot" Requires-Dist: netutils (>=1.6.0)
-Requires-Dist: nornir-nautobot (>=3.0.0,<4.0.0) Project-URL: Bug Tracker,
-https://github.com/nautobot/nautobot-plugin-nornir/issues Project-URL:
-Changelog, https://docs.nautobot.com/projects/plugin-nornir/en/latest/admin/
-release_notes/ Project-URL: Repository, https://github.com/nautobot/nautobot-
-plugin-nornir Description-Content-Type: text/markdown # Nautobot Plugin Nornir
+Language :: Python :: 3.11 Requires-Dist: nautobot (>=2.0.0,<3.0.0) Requires-
+Dist: netutils (>=1.6.0) Requires-Dist: nornir-nautobot (>=3.0.0,<4.0.0)
+Project-URL: Bug Tracker, https://github.com/nautobot/nautobot-plugin-nornir/
+issues Project-URL: Changelog, https://docs.nautobot.com/projects/plugin-
+nornir/en/latest/admin/release_notes/ Project-URL: Repository, https://
+github.com/nautobot/nautobot-plugin-nornir Description-Content-Type: text/
+markdown # Nautobot Plugin Nornir
   [https://raw.githubusercontent.com/nautobot/nautobot-plugin-nornir/develop/
                   docs/images/icon-NautobotPluginNornir.png]
  _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_n_a_u_t_o_b_o_t_/_n_a_u_t_o_b_o_t_-_p_l_u_g_i_n_-_n_o_r_n_i_r_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_c_i_._y_m_l_/
 _b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_m_a_i_n_]_[_h_t_t_p_s_:_/_/_r_e_a_d_t_h_e_d_o_c_s_._o_r_g_/_p_r_o_j_e_c_t_s_/_n_a_u_t_o_b_o_t_-_p_l_u_g_i_n_-_n_o_r_n_i_r_/
     _b_a_d_g_e_/_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_n_a_u_t_o_b_o_t_-_p_l_u_g_i_n_-_n_o_r_n_i_r_]_[_h_t_t_p_s_:_/_/
                 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_d_m_/_n_a_u_t_o_b_o_t_-_p_l_u_g_i_n_-_n_o_r_n_i_r_]
                              An App for _N_a_u_t_o_b_o_t.
```

