# Comparing `tmp/qbraid_cli-0.8.0.dev6.tar.gz` & `tmp/qbraid_cli-0.8.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbraid_cli-0.8.0.dev6.tar", last modified: Tue Apr 23 22:44:33 2024, max compression
+gzip compressed data, was "qbraid_cli-0.8.0.dev7.tar", last modified: Wed Apr 24 00:37:19 2024, max compression
```

## Comparing `qbraid_cli-0.8.0.dev6.tar` & `qbraid_cli-0.8.0.dev7.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.734693 qbraid_cli-0.8.0.dev6/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/.env.example
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.706693 qbraid_cli-0.8.0.dev6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.710693 qbraid_cli-0.8.0.dev6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.710693 qbraid_cli-0.8.0.dev6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/.github/workflows/test-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/MANIFEST.IN
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-04-23 22:44:33.734693 qbraid_cli-0.8.0.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.710693 qbraid_cli-0.8.0.dev6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.710693 qbraid_cli-0.8.0.dev6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    30522 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/docs/_static/api-key.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.714693 qbraid_cli-0.8.0.dev6/docs/_static/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/docs/_static/cards/jupyter.png
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/docs/_static/cards/python.png
--rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/docs/_static/cards/terminal.png
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.714693 qbraid_cli-0.8.0.dev6/docs/_static/style/
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/docs/_static/style/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/docs/_static/style/s4defs-roles.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.714693 qbraid_cli-0.8.0.dev6/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/docs/cli/configure.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/docs/cli/credits.rst
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/docs/cli/devices-list.rst
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/docs/cli/devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/docs/cli/envs-activate.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/docs/cli/envs-list.rst
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/docs/cli/envs-uninstall.rst
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/docs/cli/envs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/docs/cli/jobs-add.rst
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/docs/cli/jobs-disable.rst
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/docs/cli/jobs-enable.rst
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/docs/cli/jobs-list.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/docs/cli/jobs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/docs/cli/kernels.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/docs/cli/qbraid.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.714693 qbraid_cli-0.8.0.dev6/docs/guide/
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/docs/guide/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.718693 qbraid_cli-0.8.0.dev6/qbraid_cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/qbraid_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-23 22:44:33.000000 qbraid_cli-0.8.0.dev6/qbraid_cli/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.718693 qbraid_cli-0.8.0.dev6/qbraid_cli/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/qbraid_cli/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/qbraid_cli/admin/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     6667 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/qbraid_cli/admin/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/qbraid_cli/admin/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.718693 qbraid_cli-0.8.0.dev6/qbraid_cli/configure/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/qbraid_cli/configure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/qbraid_cli/configure/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/qbraid_cli/configure/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.718693 qbraid_cli-0.8.0.dev6/qbraid_cli/credits/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/qbraid_cli/credits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/qbraid_cli/credits/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.722693 qbraid_cli-0.8.0.dev6/qbraid_cli/devices/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/qbraid_cli/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/qbraid_cli/devices/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/qbraid_cli/devices/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.722693 qbraid_cli-0.8.0.dev6/qbraid_cli/envs/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/qbraid_cli/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/qbraid_cli/envs/activate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/qbraid_cli/envs/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/qbraid_cli/envs/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/qbraid_cli/envs/data_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/qbraid_cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/qbraid_cli/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.722693 qbraid_cli-0.8.0.dev6/qbraid_cli/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/qbraid_cli/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/qbraid_cli/jobs/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/qbraid_cli/jobs/toggle_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/qbraid_cli/jobs/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.722693 qbraid_cli-0.8.0.dev6/qbraid_cli/kernels/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/qbraid_cli/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/qbraid_cli/kernels/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/qbraid_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.730693 qbraid_cli-0.8.0.dev6/qbraid_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-04-23 22:44:33.000000 qbraid_cli-0.8.0.dev6/qbraid_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-23 22:44:33.000000 qbraid_cli-0.8.0.dev6/qbraid_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 22:44:33.000000 qbraid_cli-0.8.0.dev6/qbraid_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-23 22:44:33.000000 qbraid_cli-0.8.0.dev6/qbraid_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-23 22:44:33.000000 qbraid_cli-0.8.0.dev6/qbraid_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 22:44:33.000000 qbraid_cli-0.8.0.dev6/qbraid_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 22:44:33.734693 qbraid_cli-0.8.0.dev6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.722693 qbraid_cli-0.8.0.dev6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.722693 qbraid_cli-0.8.0.dev6/tests/test_configure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_configure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_configure/test_configure_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_configure/test_prompt_for_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_configure/test_validate_input.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.722693 qbraid_cli-0.8.0.dev6/tests/test_credits/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_credits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_credits/test_credits_value.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.726693 qbraid_cli-0.8.0.dev6/tests/test_devices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_devices/test_devices_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_devices/test_validations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.726693 qbraid_cli-0.8.0.dev6/tests/test_envs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_envs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.726693 qbraid_cli-0.8.0.dev6/tests/test_envs/test_activate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_envs/test_activate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_envs/test_activate/test_activate_pyenv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_envs/test_activate/test_find_shell_rc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_envs/test_activate/test_print_activate_command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.726693 qbraid_cli-0.8.0.dev6/tests/test_envs/test_app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_envs/test_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_envs/test_app/test_envs_activate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_envs/test_app/test_envs_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_envs/test_app/test_envs_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_envs/test_app/test_envs_remove.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.726693 qbraid_cli-0.8.0.dev6/tests/test_envs/test_create/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_envs/test_create/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_envs/test_create/test_create_qbraid_env_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_envs/test_create/test_replace_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_envs/test_create/test_update_state_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.726693 qbraid_cli-0.8.0.dev6/tests/test_envs/test_data_handling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_envs/test_data_handling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_envs/test_data_handling/test_installed_envs_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_envs/test_data_handling/test_is_valid_env_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_envs/test_data_handling/test_request_delete_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_envs/test_data_handling/test_validate_env_name.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.726693 qbraid_cli-0.8.0.dev6/tests/test_jobs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_jobs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.730693 qbraid_cli-0.8.0.dev6/tests/test_jobs/test_app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_jobs/test_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_jobs/test_app/test_jobs_disable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_jobs/test_app/test_jobs_enable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_jobs/test_app/test_jobs_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_jobs/test_app/test_jobs_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.730693 qbraid_cli-0.8.0.dev6/tests/test_jobs/test_toggle_braket/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_jobs/test_toggle_braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_jobs/test_toggle_braket/test_confirm_updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_jobs/test_toggle_braket/test_disable_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_jobs/test_toggle_braket/test_enable_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_jobs/test_toggle_braket/test_get_package_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.730693 qbraid_cli-0.8.0.dev6/tests/test_jobs/test_validation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_jobs/test_validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_jobs/test_validation/test_get_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_jobs/test_validation/test_handle_jobs_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_jobs/test_validation/test_run_progress_get_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_jobs/test_validation/test_validate_library.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.730693 qbraid_cli-0.8.0.dev6/tests/test_kernels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tests/test_kernels/test_kernels_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 22:44:33.730693 qbraid_cli-0.8.0.dev6/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tools/split_rst.py
--rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-04-23 22:44:25.000000 qbraid_cli-0.8.0.dev6/tools/verify_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.736724 qbraid_cli-0.8.0.dev7/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/.env.example
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.712723 qbraid_cli-0.8.0.dev7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.712723 qbraid_cli-0.8.0.dev7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.712723 qbraid_cli-0.8.0.dev7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/.github/workflows/test-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/MANIFEST.IN
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-04-24 00:37:19.736724 qbraid_cli-0.8.0.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.712723 qbraid_cli-0.8.0.dev7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.712723 qbraid_cli-0.8.0.dev7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    30522 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/docs/_static/api-key.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.716723 qbraid_cli-0.8.0.dev7/docs/_static/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/docs/_static/cards/jupyter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/docs/_static/cards/python.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/docs/_static/cards/terminal.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.716723 qbraid_cli-0.8.0.dev7/docs/_static/style/
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/docs/_static/style/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/docs/_static/style/s4defs-roles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.716723 qbraid_cli-0.8.0.dev7/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/docs/cli/configure.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/docs/cli/credits.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/docs/cli/devices-list.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/docs/cli/devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/docs/cli/envs-activate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/docs/cli/envs-list.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/docs/cli/envs-uninstall.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/docs/cli/envs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/docs/cli/jobs-add.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/docs/cli/jobs-disable.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/docs/cli/jobs-enable.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/docs/cli/jobs-list.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/docs/cli/jobs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/docs/cli/kernels.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/docs/cli/qbraid.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.720723 qbraid_cli-0.8.0.dev7/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/docs/guide/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.720723 qbraid_cli-0.8.0.dev7/qbraid_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/qbraid_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-24 00:37:19.000000 qbraid_cli-0.8.0.dev7/qbraid_cli/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.720723 qbraid_cli-0.8.0.dev7/qbraid_cli/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/qbraid_cli/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/qbraid_cli/admin/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6667 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/qbraid_cli/admin/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/qbraid_cli/admin/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.720723 qbraid_cli-0.8.0.dev7/qbraid_cli/configure/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/qbraid_cli/configure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/qbraid_cli/configure/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/qbraid_cli/configure/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.724723 qbraid_cli-0.8.0.dev7/qbraid_cli/credits/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/qbraid_cli/credits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/qbraid_cli/credits/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.724723 qbraid_cli-0.8.0.dev7/qbraid_cli/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/qbraid_cli/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/qbraid_cli/devices/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/qbraid_cli/devices/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.724723 qbraid_cli-0.8.0.dev7/qbraid_cli/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/qbraid_cli/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/qbraid_cli/envs/activate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/qbraid_cli/envs/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/qbraid_cli/envs/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/qbraid_cli/envs/data_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/qbraid_cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/qbraid_cli/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.724723 qbraid_cli-0.8.0.dev7/qbraid_cli/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/qbraid_cli/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/qbraid_cli/jobs/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/qbraid_cli/jobs/toggle_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/qbraid_cli/jobs/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.724723 qbraid_cli-0.8.0.dev7/qbraid_cli/kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/qbraid_cli/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/qbraid_cli/kernels/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/qbraid_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.732724 qbraid_cli-0.8.0.dev7/qbraid_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-04-24 00:37:19.000000 qbraid_cli-0.8.0.dev7/qbraid_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-24 00:37:19.000000 qbraid_cli-0.8.0.dev7/qbraid_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 00:37:19.000000 qbraid_cli-0.8.0.dev7/qbraid_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 00:37:19.000000 qbraid_cli-0.8.0.dev7/qbraid_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-24 00:37:19.000000 qbraid_cli-0.8.0.dev7/qbraid_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 00:37:19.000000 qbraid_cli-0.8.0.dev7/qbraid_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 00:37:19.736724 qbraid_cli-0.8.0.dev7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.724723 qbraid_cli-0.8.0.dev7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.724723 qbraid_cli-0.8.0.dev7/tests/test_configure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_configure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_configure/test_configure_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_configure/test_prompt_for_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_configure/test_validate_input.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.728723 qbraid_cli-0.8.0.dev7/tests/test_credits/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_credits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_credits/test_credits_value.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.728723 qbraid_cli-0.8.0.dev7/tests/test_devices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_devices/test_devices_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_devices/test_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.728723 qbraid_cli-0.8.0.dev7/tests/test_envs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_envs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.728723 qbraid_cli-0.8.0.dev7/tests/test_envs/test_activate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_envs/test_activate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_envs/test_activate/test_activate_pyenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_envs/test_activate/test_find_shell_rc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_envs/test_activate/test_print_activate_command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.728723 qbraid_cli-0.8.0.dev7/tests/test_envs/test_app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_envs/test_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_envs/test_app/test_envs_activate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_envs/test_app/test_envs_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_envs/test_app/test_envs_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_envs/test_app/test_envs_remove.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.728723 qbraid_cli-0.8.0.dev7/tests/test_envs/test_create/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_envs/test_create/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_envs/test_create/test_create_qbraid_env_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_envs/test_create/test_replace_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_envs/test_create/test_update_state_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.732724 qbraid_cli-0.8.0.dev7/tests/test_envs/test_data_handling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_envs/test_data_handling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_envs/test_data_handling/test_installed_envs_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_envs/test_data_handling/test_is_valid_env_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_envs/test_data_handling/test_request_delete_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_envs/test_data_handling/test_validate_env_name.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.732724 qbraid_cli-0.8.0.dev7/tests/test_jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_jobs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.732724 qbraid_cli-0.8.0.dev7/tests/test_jobs/test_app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_jobs/test_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_jobs/test_app/test_jobs_disable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_jobs/test_app/test_jobs_enable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_jobs/test_app/test_jobs_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_jobs/test_app/test_jobs_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.732724 qbraid_cli-0.8.0.dev7/tests/test_jobs/test_toggle_braket/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_jobs/test_toggle_braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_jobs/test_toggle_braket/test_confirm_updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_jobs/test_toggle_braket/test_disable_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_jobs/test_toggle_braket/test_enable_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_jobs/test_toggle_braket/test_get_package_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.732724 qbraid_cli-0.8.0.dev7/tests/test_jobs/test_validation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_jobs/test_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_jobs/test_validation/test_get_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_jobs/test_validation/test_handle_jobs_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_jobs/test_validation/test_run_progress_get_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_jobs/test_validation/test_validate_library.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.732724 qbraid_cli-0.8.0.dev7/tests/test_kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tests/test_kernels/test_kernels_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:37:19.732724 qbraid_cli-0.8.0.dev7/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tools/split_rst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-04-24 00:37:07.000000 qbraid_cli-0.8.0.dev7/tools/verify_headers.py
```

### Comparing `qbraid_cli-0.8.0.dev6/.github/ISSUE_TEMPLATE/bug_report.yml` & `qbraid_cli-0.8.0.dev7/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/.github/ISSUE_TEMPLATE/feature_request.yml` & `qbraid_cli-0.8.0.dev7/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/.github/workflows/docs.yml` & `qbraid_cli-0.8.0.dev7/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/.github/workflows/format.yml` & `qbraid_cli-0.8.0.dev7/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/.github/workflows/main.yml` & `qbraid_cli-0.8.0.dev7/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/.github/workflows/publish.yml` & `qbraid_cli-0.8.0.dev7/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/.github/workflows/test-publish.yml` & `qbraid_cli-0.8.0.dev7/.github/workflows/test-publish.yml`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/.gitignore` & `qbraid_cli-0.8.0.dev7/.gitignore`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/.readthedocs.yml` & `qbraid_cli-0.8.0.dev7/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/CONTRIBUTING.md` & `qbraid_cli-0.8.0.dev7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/Makefile` & `qbraid_cli-0.8.0.dev7/Makefile`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/PKG-INFO` & `qbraid_cli-0.8.0.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-cli
-Version: 0.8.0.dev6
+Version: 0.8.0.dev7
 Summary: Command Line Interface for interacting with all parts of the qBraid platform.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
```

### Comparing `qbraid_cli-0.8.0.dev6/README.md` & `qbraid_cli-0.8.0.dev7/README.md`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/docs/Makefile` & `qbraid_cli-0.8.0.dev7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/docs/_static/api-key.png` & `qbraid_cli-0.8.0.dev7/docs/_static/api-key.png`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/docs/_static/cards/jupyter.png` & `qbraid_cli-0.8.0.dev7/docs/_static/cards/jupyter.png`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/docs/_static/cards/python.png` & `qbraid_cli-0.8.0.dev7/docs/_static/cards/python.png`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/docs/_static/cards/terminal.png` & `qbraid_cli-0.8.0.dev7/docs/_static/cards/terminal.png`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/docs/_static/favicon.ico` & `qbraid_cli-0.8.0.dev7/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/docs/_static/logo.png` & `qbraid_cli-0.8.0.dev7/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/docs/_static/style/custom.css` & `qbraid_cli-0.8.0.dev7/docs/_static/style/custom.css`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/docs/_static/style/s4defs-roles.css` & `qbraid_cli-0.8.0.dev7/docs/_static/style/s4defs-roles.css`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/docs/cli/configure.rst` & `qbraid_cli-0.8.0.dev7/docs/cli/configure.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/docs/cli/devices-list.rst` & `qbraid_cli-0.8.0.dev7/docs/cli/devices-list.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/docs/cli/envs-activate.rst` & `qbraid_cli-0.8.0.dev7/docs/cli/envs-activate.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/docs/cli/envs-list.rst` & `qbraid_cli-0.8.0.dev7/docs/cli/envs-list.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/docs/cli/envs-uninstall.rst` & `qbraid_cli-0.8.0.dev7/docs/cli/envs-uninstall.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/docs/cli/envs.rst` & `qbraid_cli-0.8.0.dev7/docs/cli/envs.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/docs/cli/jobs-add.rst` & `qbraid_cli-0.8.0.dev7/docs/cli/jobs-add.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/docs/cli/jobs-disable.rst` & `qbraid_cli-0.8.0.dev7/docs/cli/jobs-disable.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/docs/cli/jobs-enable.rst` & `qbraid_cli-0.8.0.dev7/docs/cli/jobs-enable.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/docs/cli/jobs-list.rst` & `qbraid_cli-0.8.0.dev7/docs/cli/jobs-list.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/docs/cli/jobs.rst` & `qbraid_cli-0.8.0.dev7/docs/cli/jobs.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/docs/cli/kernels.rst` & `qbraid_cli-0.8.0.dev7/docs/cli/kernels.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/docs/cli/qbraid.rst` & `qbraid_cli-0.8.0.dev7/docs/cli/qbraid.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/docs/conf.py` & `qbraid_cli-0.8.0.dev7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/docs/guide/overview.rst` & `qbraid_cli-0.8.0.dev7/docs/guide/overview.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/docs/index.rst` & `qbraid_cli-0.8.0.dev7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/docs/make.bat` & `qbraid_cli-0.8.0.dev7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/pyproject.toml` & `qbraid_cli-0.8.0.dev7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qbraid-cli"
-version = "0.8.0.dev6"
+version = "0.8.0.dev7"
 description = "Command Line Interface for interacting with all parts of the qBraid platform."
 readme = "README.md"
 authors = [{ name = "qBraid Development Team", email = "contact@qbraid.com" }]
 license = { text = "Proprietary" }
 keywords = ["qbraid", "cli", "quantum", "cloud"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `qbraid_cli-0.8.0.dev6/qbraid_cli/admin/app.py` & `qbraid_cli-0.8.0.dev7/qbraid_cli/admin/app.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/qbraid_cli/admin/headers.py` & `qbraid_cli-0.8.0.dev7/qbraid_cli/admin/headers.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/qbraid_cli/admin/validation.py` & `qbraid_cli-0.8.0.dev7/qbraid_cli/admin/validation.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/qbraid_cli/configure/actions.py` & `qbraid_cli-0.8.0.dev7/qbraid_cli/configure/actions.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/qbraid_cli/configure/app.py` & `qbraid_cli-0.8.0.dev7/qbraid_cli/configure/app.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 """
 Module defining commands in the 'qbraid configure' namespace.
 
 """
 
 import typer
+from rich.console import Console
 
 from qbraid_cli.configure.actions import default_action
 
 # disable pretty_exceptions_show_locals to avoid printing sensative information in the traceback
 configure_app = typer.Typer(
     help="Configure qBraid CLI options.", pretty_exceptions_show_locals=False
 )
@@ -50,20 +51,27 @@
 
     save_config(config)
     typer.echo("Configuration updated successfully.")
 
 
 @configure_app.command(name="magic")
 def configure_magic():
-    """Configure qBraid IPython magic commands."""
+    """Enable qBraid IPython magic commands."""
     # pylint: disable-next=import-outside-toplevel
     from qbraid_core.services.environments import add_magic_config
 
     add_magic_config()
 
-    typer.echo("Successfully configured qBraid IPython magic commands.")
-    typer.echo("You can now use the qBraid-CLI from inside a Jupyter notebook as follows:")
-    typer.echo("\n\n\t[ ] %load_ext qbraid_magic\n\n\t[ ] %qbraid")
+    console = Console()
+
+    in_1 = (
+        "[green]In [[/green][yellow]1[/yellow][green]]:[/green] [blue]%[/blue]load_ext qbraid_magic"
+    )
+    in_2 = "[green]In [[/green][yellow]2[/yellow][green]]:[/green] [blue]%[/blue]qbraid"
+
+    console.print("\nSuccessfully configured qBraid IPython magic commands.\n")
+    console.print("You can now use the qBraid-CLI from inside a Jupyter notebook as follows:")
+    console.print(f"\n\t{in_1}\n\n\t{in_2}\n")
 
 
 if __name__ == "__main__":
     configure_app()
```

### Comparing `qbraid_cli-0.8.0.dev6/qbraid_cli/credits/app.py` & `qbraid_cli-0.8.0.dev7/qbraid_cli/credits/app.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/qbraid_cli/devices/app.py` & `qbraid_cli-0.8.0.dev7/qbraid_cli/devices/app.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/qbraid_cli/devices/validation.py` & `qbraid_cli-0.8.0.dev7/qbraid_cli/devices/validation.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/qbraid_cli/envs/activate.py` & `qbraid_cli-0.8.0.dev7/qbraid_cli/envs/activate.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/qbraid_cli/envs/app.py` & `qbraid_cli-0.8.0.dev7/qbraid_cli/envs/app.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/qbraid_cli/envs/create.py` & `qbraid_cli-0.8.0.dev7/qbraid_cli/envs/create.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/qbraid_cli/envs/data_handling.py` & `qbraid_cli-0.8.0.dev7/qbraid_cli/envs/data_handling.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/qbraid_cli/exceptions.py` & `qbraid_cli-0.8.0.dev7/qbraid_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/qbraid_cli/handlers.py` & `qbraid_cli-0.8.0.dev7/qbraid_cli/handlers.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/qbraid_cli/jobs/app.py` & `qbraid_cli-0.8.0.dev7/qbraid_cli/jobs/app.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/qbraid_cli/jobs/toggle_braket.py` & `qbraid_cli-0.8.0.dev7/qbraid_cli/jobs/toggle_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/qbraid_cli/jobs/validation.py` & `qbraid_cli-0.8.0.dev7/qbraid_cli/jobs/validation.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/qbraid_cli/kernels/app.py` & `qbraid_cli-0.8.0.dev7/qbraid_cli/kernels/app.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/qbraid_cli/main.py` & `qbraid_cli-0.8.0.dev7/qbraid_cli/main.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/qbraid_cli.egg-info/PKG-INFO` & `qbraid_cli-0.8.0.dev7/qbraid_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-cli
-Version: 0.8.0.dev6
+Version: 0.8.0.dev7
 Summary: Command Line Interface for interacting with all parts of the qBraid platform.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/cli/en/stable/guide/overview.html
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
```

### Comparing `qbraid_cli-0.8.0.dev6/qbraid_cli.egg-info/SOURCES.txt` & `qbraid_cli-0.8.0.dev7/qbraid_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_configure/test_configure_set.py` & `qbraid_cli-0.8.0.dev7/tests/test_configure/test_configure_set.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_configure/test_prompt_for_config.py` & `qbraid_cli-0.8.0.dev7/tests/test_configure/test_prompt_for_config.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_configure/test_validate_input.py` & `qbraid_cli-0.8.0.dev7/tests/test_configure/test_validate_input.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_credits/test_credits_value.py` & `qbraid_cli-0.8.0.dev7/tests/test_credits/test_credits_value.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_devices/test_devices_list.py` & `qbraid_cli-0.8.0.dev7/tests/test_devices/test_devices_list.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_devices/test_validations.py` & `qbraid_cli-0.8.0.dev7/tests/test_devices/test_validations.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_envs/test_activate/test_activate_pyenv.py` & `qbraid_cli-0.8.0.dev7/tests/test_envs/test_activate/test_activate_pyenv.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_envs/test_activate/test_find_shell_rc.py` & `qbraid_cli-0.8.0.dev7/tests/test_envs/test_activate/test_find_shell_rc.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_envs/test_activate/test_print_activate_command.py` & `qbraid_cli-0.8.0.dev7/tests/test_envs/test_activate/test_print_activate_command.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_envs/test_app/test_envs_activate.py` & `qbraid_cli-0.8.0.dev7/tests/test_envs/test_app/test_envs_activate.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_envs/test_app/test_envs_create.py` & `qbraid_cli-0.8.0.dev7/tests/test_envs/test_app/test_envs_create.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_envs/test_app/test_envs_list.py` & `qbraid_cli-0.8.0.dev7/tests/test_envs/test_app/test_envs_list.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_envs/test_app/test_envs_remove.py` & `qbraid_cli-0.8.0.dev7/tests/test_envs/test_app/test_envs_remove.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_envs/test_create/test_create_qbraid_env_assets.py` & `qbraid_cli-0.8.0.dev7/tests/test_envs/test_create/test_create_qbraid_env_assets.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_envs/test_create/test_replace_str.py` & `qbraid_cli-0.8.0.dev7/tests/test_envs/test_create/test_replace_str.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_envs/test_create/test_update_state_json.py` & `qbraid_cli-0.8.0.dev7/tests/test_envs/test_create/test_update_state_json.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_envs/test_data_handling/test_installed_envs_data.py` & `qbraid_cli-0.8.0.dev7/tests/test_envs/test_data_handling/test_installed_envs_data.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_envs/test_data_handling/test_is_valid_env_name.py` & `qbraid_cli-0.8.0.dev7/tests/test_envs/test_data_handling/test_is_valid_env_name.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_envs/test_data_handling/test_request_delete_env.py` & `qbraid_cli-0.8.0.dev7/tests/test_envs/test_data_handling/test_request_delete_env.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_envs/test_data_handling/test_validate_env_name.py` & `qbraid_cli-0.8.0.dev7/tests/test_envs/test_data_handling/test_validate_env_name.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_jobs/test_app/test_jobs_disable.py` & `qbraid_cli-0.8.0.dev7/tests/test_jobs/test_app/test_jobs_disable.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_jobs/test_app/test_jobs_enable.py` & `qbraid_cli-0.8.0.dev7/tests/test_jobs/test_app/test_jobs_enable.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_jobs/test_app/test_jobs_list.py` & `qbraid_cli-0.8.0.dev7/tests/test_jobs/test_app/test_jobs_list.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_jobs/test_app/test_jobs_state.py` & `qbraid_cli-0.8.0.dev7/tests/test_jobs/test_app/test_jobs_state.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_jobs/test_toggle_braket/test_confirm_updates.py` & `qbraid_cli-0.8.0.dev7/tests/test_jobs/test_toggle_braket/test_confirm_updates.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_jobs/test_toggle_braket/test_disable_braket.py` & `qbraid_cli-0.8.0.dev7/tests/test_jobs/test_toggle_braket/test_disable_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_jobs/test_toggle_braket/test_enable_braket.py` & `qbraid_cli-0.8.0.dev7/tests/test_jobs/test_toggle_braket/test_enable_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_jobs/test_toggle_braket/test_get_package_data.py` & `qbraid_cli-0.8.0.dev7/tests/test_jobs/test_toggle_braket/test_get_package_data.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_jobs/test_validation/test_get_state.py` & `qbraid_cli-0.8.0.dev7/tests/test_jobs/test_validation/test_get_state.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_jobs/test_validation/test_handle_jobs_state.py` & `qbraid_cli-0.8.0.dev7/tests/test_jobs/test_validation/test_handle_jobs_state.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_jobs/test_validation/test_run_progress_get_state.py` & `qbraid_cli-0.8.0.dev7/tests/test_jobs/test_validation/test_run_progress_get_state.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_jobs/test_validation/test_validate_library.py` & `qbraid_cli-0.8.0.dev7/tests/test_jobs/test_validation/test_validate_library.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tests/test_kernels/test_kernels_list.py` & `qbraid_cli-0.8.0.dev7/tests/test_kernels/test_kernels_list.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tools/split_rst.py` & `qbraid_cli-0.8.0.dev7/tools/split_rst.py`

 * *Files identical despite different names*

### Comparing `qbraid_cli-0.8.0.dev6/tools/verify_headers.py` & `qbraid_cli-0.8.0.dev7/tools/verify_headers.py`

 * *Files identical despite different names*

