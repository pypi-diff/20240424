# Comparing `tmp/qbraid_core-0.1.4.dev1.tar.gz` & `tmp/qbraid_core-0.1.4.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbraid_core-0.1.4.dev1.tar", last modified: Fri Apr 19 19:46:16 2024, max compression
+gzip compressed data, was "qbraid_core-0.1.4.dev2.tar", last modified: Tue Apr 23 21:27:41 2024, max compression
```

## Comparing `qbraid_core-0.1.4.dev1.tar` & `qbraid_core-0.1.4.dev2.tar`

### file list

```diff
@@ -1,111 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.931794 qbraid_core-0.1.4.dev1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.915794 qbraid_core-0.1.4.dev1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.915794 qbraid_core-0.1.4.dev1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.915794 qbraid_core-0.1.4.dev1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/.github/workflows/test-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-19 19:46:16.931794 qbraid_core-0.1.4.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.919793 qbraid_core-0.1.4.dev1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.919793 qbraid_core-0.1.4.dev1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.919793 qbraid_core-0.1.4.dev1/docs/_static/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/docs/_static/cards/jupyter.png
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/docs/_static/cards/python.png
--rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/docs/_static/cards/terminal.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.919793 qbraid_core-0.1.4.dev1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/docs/_static/css/s4defs-roles.css
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.919793 qbraid_core-0.1.4.dev1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/docs/api/qbraid_core.rst
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/docs/api/qbraid_core.services.rst
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/docs/api/qbraid_core.system.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.923793 qbraid_core-0.1.4.dev1/qbraid_core/
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-19 19:46:16.000000 qbraid_core-0.1.4.dev1/qbraid_core/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.923793 qbraid_core-0.1.4.dev1/qbraid_core/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.923793 qbraid_core-0.1.4.dev1/qbraid_core/services/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/admin/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.923793 qbraid_core-0.1.4.dev1/qbraid_core/services/environments/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/environments/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/environments/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/environments/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/environments/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/environments/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/environments/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.923793 qbraid_core-0.1.4.dev1/qbraid_core/services/quantum/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/quantum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/quantum/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/quantum/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/quantum/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/quantum/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/services/quantum/proxy_braket.py
--rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/sessions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.923793 qbraid_core-0.1.4.dev1/qbraid_core/system/
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/system/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/system/executables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/system/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     8519 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/system/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/system/threader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/qbraid_core/system/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.927794 qbraid_core-0.1.4.dev1/qbraid_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-19 19:46:16.000000 qbraid_core-0.1.4.dev1/qbraid_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-19 19:46:16.000000 qbraid_core-0.1.4.dev1/qbraid_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:46:16.000000 qbraid_core-0.1.4.dev1/qbraid_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-19 19:46:16.000000 qbraid_core-0.1.4.dev1/qbraid_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 19:46:16.000000 qbraid_core-0.1.4.dev1/qbraid_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:46:16.931794 qbraid_core-0.1.4.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.923793 qbraid_core-0.1.4.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.927794 qbraid_core-0.1.4.dev1/tests/environments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/environments/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.927794 qbraid_core-0.1.4.dev1/tests/environments/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/environments/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/environments/fixtures/environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/environments/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/environments/test_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/environments/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/environments/test_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/environments/test_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.927794 qbraid_core-0.1.4.dev1/tests/quantum/
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/quantum/test_aws_configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/quantum/test_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.927794 qbraid_core-0.1.4.dev1/tests/system/
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/system/test_executables.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/system/test_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/system/test_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/system/test_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.927794 qbraid_core-0.1.4.dev1/tests/top_level/
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/top_level/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/top_level/test_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/top_level/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tests/top_level/test_sessions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:46:16.927794 qbraid_core-0.1.4.dev1/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-19 19:46:13.000000 qbraid_core-0.1.4.dev1/tools/verify_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:27:41.223374 qbraid_core-0.1.4.dev2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:27:41.203374 qbraid_core-0.1.4.dev2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:27:41.203374 qbraid_core-0.1.4.dev2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:27:41.207374 qbraid_core-0.1.4.dev2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/.github/workflows/test-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-04-23 21:27:41.223374 qbraid_core-0.1.4.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:27:41.207374 qbraid_core-0.1.4.dev2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:27:41.207374 qbraid_core-0.1.4.dev2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:27:41.207374 qbraid_core-0.1.4.dev2/docs/_static/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/docs/_static/cards/jupyter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/docs/_static/cards/python.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/docs/_static/cards/terminal.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:27:41.207374 qbraid_core-0.1.4.dev2/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/docs/_static/css/s4defs-roles.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:27:41.207374 qbraid_core-0.1.4.dev2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/docs/api/qbraid_core.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/docs/api/qbraid_core.services.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/docs/api/qbraid_core.system.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:27:41.211374 qbraid_core-0.1.4.dev2/qbraid_core/
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-23 21:27:41.000000 qbraid_core-0.1.4.dev2/qbraid_core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:27:41.211374 qbraid_core-0.1.4.dev2/qbraid_core/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:27:41.211374 qbraid_core-0.1.4.dev2/qbraid_core/services/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/services/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/services/admin/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:27:41.215374 qbraid_core-0.1.4.dev2/qbraid_core/services/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/services/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/services/environments/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/services/environments/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/services/environments/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/services/environments/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/services/environments/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/services/environments/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/services/environments/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:27:41.215374 qbraid_core-0.1.4.dev2/qbraid_core/services/quantum/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/services/quantum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/services/quantum/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/services/quantum/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/services/quantum/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/services/quantum/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/services/quantum/proxy_braket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/sessions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:27:41.215374 qbraid_core-0.1.4.dev2/qbraid_core/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/system/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/system/executables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/system/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:27:41.215374 qbraid_core-0.1.4.dev2/qbraid_core/system/magic/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/system/magic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/system/magic/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/system/magic/qbraid_magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/system/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/system/threader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/qbraid_core/system/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:27:41.219374 qbraid_core-0.1.4.dev2/qbraid_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-04-23 21:27:41.000000 qbraid_core-0.1.4.dev2/qbraid_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-23 21:27:41.000000 qbraid_core-0.1.4.dev2/qbraid_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 21:27:41.000000 qbraid_core-0.1.4.dev2/qbraid_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-23 21:27:41.000000 qbraid_core-0.1.4.dev2/qbraid_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 21:27:41.000000 qbraid_core-0.1.4.dev2/qbraid_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 21:27:41.223374 qbraid_core-0.1.4.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:27:41.215374 qbraid_core-0.1.4.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:27:41.219374 qbraid_core-0.1.4.dev2/tests/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/tests/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/tests/environments/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:27:41.219374 qbraid_core-0.1.4.dev2/tests/environments/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/tests/environments/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/tests/environments/fixtures/environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/tests/environments/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/tests/environments/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/tests/environments/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/tests/environments/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/tests/environments/test_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:27:41.219374 qbraid_core-0.1.4.dev2/tests/quantum/
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/tests/quantum/test_aws_configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/tests/quantum/test_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:27:41.219374 qbraid_core-0.1.4.dev2/tests/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/tests/system/test_executables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/tests/system/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/tests/system/test_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/tests/system/test_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:27:41.219374 qbraid_core-0.1.4.dev2/tests/top_level/
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/tests/top_level/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/tests/top_level/test_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/tests/top_level/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/tests/top_level/test_sessions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:27:41.219374 qbraid_core-0.1.4.dev2/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-23 21:27:35.000000 qbraid_core-0.1.4.dev2/tools/verify_headers.py
```

### Comparing `qbraid_core-0.1.4.dev1/.github/ISSUE_TEMPLATE/bug_report.yml` & `qbraid_core-0.1.4.dev2/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/.github/ISSUE_TEMPLATE/feature_request.yml` & `qbraid_core-0.1.4.dev2/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/.github/workflows/docs.yml` & `qbraid_core-0.1.4.dev2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/.github/workflows/format.yml` & `qbraid_core-0.1.4.dev2/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/.github/workflows/main.yml` & `qbraid_core-0.1.4.dev2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/.github/workflows/publish.yml` & `qbraid_core-0.1.4.dev2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/.github/workflows/test-publish.yml` & `qbraid_core-0.1.4.dev2/.github/workflows/test-publish.yml`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/.gitignore` & `qbraid_core-0.1.4.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/LICENSE` & `qbraid_core-0.1.4.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/PKG-INFO` & `qbraid_core-0.1.4.dev2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-core
-Version: 0.1.4.dev1
+Version: 0.1.4.dev2
 Summary: Python library with core abstractions for software development in the qBraid ecosystem.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/core/en/latest/
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: urllib3
+Requires-Dist: ipython
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx~=7.2.6; extra == "docs"
```

### Comparing `qbraid_core-0.1.4.dev1/README.md` & `qbraid_core-0.1.4.dev2/README.md`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/docs/Makefile` & `qbraid_core-0.1.4.dev2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/docs/_static/cards/jupyter.png` & `qbraid_core-0.1.4.dev2/docs/_static/cards/jupyter.png`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/docs/_static/cards/python.png` & `qbraid_core-0.1.4.dev2/docs/_static/cards/python.png`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/docs/_static/cards/terminal.png` & `qbraid_core-0.1.4.dev2/docs/_static/cards/terminal.png`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/docs/_static/css/custom.css` & `qbraid_core-0.1.4.dev2/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/docs/_static/css/s4defs-roles.css` & `qbraid_core-0.1.4.dev2/docs/_static/css/s4defs-roles.css`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/docs/_static/favicon.ico` & `qbraid_core-0.1.4.dev2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/docs/_static/logo.png` & `qbraid_core-0.1.4.dev2/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/docs/conf.py` & `qbraid_core-0.1.4.dev2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/docs/index.rst` & `qbraid_core-0.1.4.dev2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/docs/make.bat` & `qbraid_core-0.1.4.dev2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/pyproject.toml` & `qbraid_core-0.1.4.dev2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qbraid-core"
-version = "0.1.4.dev1"
+version = "0.1.4.dev2"
 authors = [
     {name = "qBraid Development Team", email = "contact@qbraid.com"},
 ]
 description = "Python library with core abstractions for software development in the qBraid ecosystem."
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["qbraid", "quantum", "cloud"]
@@ -21,15 +21,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
-dependencies = ["requests", "urllib3"]
+dependencies = ["requests", "urllib3", "ipython"]
 
 [project.urls]
 Homepage = "https://www.qbraid.com/"
 Documentation = "https://docs.qbraid.com/projects/core/en/latest/"
 "Bug Tracker" = "https://github.com/qBraid/qBraid-Lab/issues"
 Discord = "https://discord.gg/KugF6Cnncm"
 "Launch on Lab" = "https://account.qbraid.com/?gitHubUrl=https://github.com/qBraid/qBraid-Lab.git"
```

### Comparing `qbraid_core-0.1.4.dev1/qbraid_core/__init__.py` & `qbraid_core-0.1.4.dev2/qbraid_core/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/qbraid_core/_compat.py` & `qbraid_core-0.1.4.dev2/qbraid_core/_compat.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/qbraid_core/client.py` & `qbraid_core-0.1.4.dev2/qbraid_core/client.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/qbraid_core/config.py` & `qbraid_core-0.1.4.dev2/qbraid_core/config.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/qbraid_core/exceptions.py` & `qbraid_core-0.1.4.dev2/qbraid_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/qbraid_core/registry.py` & `qbraid_core-0.1.4.dev2/qbraid_core/registry.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/qbraid_core/retry.py` & `qbraid_core-0.1.4.dev2/qbraid_core/retry.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/qbraid_core/services/admin/client.py` & `qbraid_core-0.1.4.dev2/qbraid_core/services/admin/client.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/qbraid_core/services/environments/__init__.py` & `qbraid_core-0.1.4.dev2/qbraid_core/services/environments/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,28 +26,31 @@
    get_default_envs_paths
    get_env_path
    get_tmp_dir_names
    get_next_tmpn
    which_python
    is_valid_env_name
    is_valid_slug
+   add_magic_config
+   remove_magic_config
 
 Exceptions
 ------------
 
 .. autosummary::
    :toctree: ../stubs/
 
    EnvironmentServiceRequestError
    EnvironmentServiceRuntimeError
 
 """
 from .client import EnvironmentManagerClient
 from .create import create_local_venv
 from .exceptions import EnvironmentServiceRequestError, EnvironmentServiceRuntimeError
+from .magic import add_magic_config, remove_magic_config
 from .paths import (
     get_default_envs_paths,
     get_env_path,
     get_next_tmpn,
     get_tmp_dir_names,
     which_python,
 )
```

### Comparing `qbraid_core-0.1.4.dev1/qbraid_core/services/environments/client.py` & `qbraid_core-0.1.4.dev2/qbraid_core/services/environments/client.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/qbraid_core/services/environments/create.py` & `qbraid_core-0.1.4.dev2/qbraid_core/services/environments/create.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/qbraid_core/services/environments/paths.py` & `qbraid_core-0.1.4.dev2/qbraid_core/services/environments/paths.py`

 * *Files identical despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) 2024, qBraid Development Team
 # All rights reserved.
 
 """
-Module for serving environment information.
+Module for serving environment paths information.
 
 """
 
 import json
 import logging
 import os
 import re
```

### Comparing `qbraid_core-0.1.4.dev1/qbraid_core/services/environments/state.py` & `qbraid_core-0.1.4.dev2/qbraid_core/services/environments/state.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/qbraid_core/services/environments/validate.py` & `qbraid_core-0.1.4.dev2/qbraid_core/services/environments/validate.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/qbraid_core/services/quantum/__init__.py` & `qbraid_core-0.1.4.dev2/qbraid_core/services/quantum/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/qbraid_core/services/quantum/adapter.py` & `qbraid_core-0.1.4.dev2/qbraid_core/services/quantum/adapter.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/qbraid_core/services/quantum/client.py` & `qbraid_core-0.1.4.dev2/qbraid_core/services/quantum/client.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/qbraid_core/services/quantum/proxy.py` & `qbraid_core-0.1.4.dev2/qbraid_core/services/quantum/proxy.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/qbraid_core/services/quantum/proxy_braket.py` & `qbraid_core-0.1.4.dev2/qbraid_core/services/quantum/proxy_braket.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/qbraid_core/sessions.py` & `qbraid_core-0.1.4.dev2/qbraid_core/sessions.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/qbraid_core/system/__init__.py` & `qbraid_core-0.1.4.dev2/qbraid_core/system/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,29 +16,31 @@
 
 Functions
 ----------
 
 .. autosummary::
    :toctree: ../stubs/
 
-   echo_log
    extract_version
    is_exe
    is_valid_python
    is_valid_semantic_version
    get_python_version_from_cfg
    get_python_version_from_exe
    get_venv_site_packages_path
    get_active_site_packages_path
    get_active_python_path
    get_local_package_path
    get_local_package_version
    get_latest_package_version
    python_paths_equivalent
+   add_config_path_to_site_packages
+   remove_config_path_from_site_packages
    replace_str
+   echo_log
 
 
 Exceptions
 ------------
 
 .. autosummary::
    :toctree: ../stubs/
@@ -61,15 +63,20 @@
     get_python_version_from_exe,
     is_exe,
     is_valid_python,
     python_paths_equivalent,
 )
 from .generic import echo_log, replace_str
 from .packages import (
+    add_config_path_to_site_packages,
     get_active_site_packages_path,
-    get_latest_package_version,
     get_local_package_path,
-    get_local_package_version,
     get_venv_site_packages_path,
+    remove_config_path_from_site_packages,
 )
 from .threader import FileManager
-from .versions import extract_version, is_valid_semantic_version
+from .versions import (
+    extract_version,
+    get_latest_package_version,
+    get_local_package_version,
+    is_valid_semantic_version,
+)
```

### Comparing `qbraid_core-0.1.4.dev1/qbraid_core/system/exceptions.py` & `qbraid_core-0.1.4.dev2/qbraid_core/system/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/qbraid_core/system/executables.py` & `qbraid_core-0.1.4.dev2/qbraid_core/system/executables.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/qbraid_core/system/generic.py` & `qbraid_core-0.1.4.dev2/qbraid_core/system/generic.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/qbraid_core/system/packages.py` & `qbraid_core-0.1.4.dev2/qbraid_core/system/packages.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,47 +6,49 @@
 
 """
 import ast
 import logging
 import site
 import subprocess
 import sys
-from importlib.metadata import PackageNotFoundError, version
+from importlib.metadata import PackageNotFoundError
 from pathlib import Path
 from typing import Optional, Union
 
-import requests
+from qbraid_core.config import USER_CONFIG_PATH
 
-from .exceptions import QbraidSystemError, VersionNotFoundError
+from .exceptions import QbraidSystemError
 from .executables import (
     get_active_python_path,
     get_python_version_from_cfg,
     get_python_version_from_exe,
     python_paths_equivalent,
 )
 
 logger = logging.getLogger(__name__)
 
 
-def get_venv_site_packages_path(venv_path: Path) -> Path:
+def get_venv_site_packages_path(venv_path: Union[str, Path]) -> Path:
     """
     Determines the site-packages directory for a given virtual environment in an OS-agnostic manner.
     Automatically selects the Python version if a single version is present in the 'lib' directory.
     If multiple versions are detected, it attempts to determine the correct version through
     configuration files or the Python executable.
 
     Args:
-        venv_path (pathlib.Path): The path to the virtual environment directory.
+        venv_path (Union[str, pathlib.Path]): The path to the virtual environment directory.
 
     Returns:
         A Path object pointing to the site-packages directory, or None if unable to determine.
 
     Raises:
         QbraidSystemError: If an error occurs while determining the site-packages path.
     """
+    venv_path = Path(venv_path)
+
     if sys.platform == "win32":
         return venv_path / "Lib" / "site-packages"
 
     python_dirs = sorted(venv_path.glob("lib/python*"))
     if not python_dirs:
         raise QbraidSystemError("No Python directories found in the virtual environment.")
 
@@ -121,75 +123,14 @@
     try:
         site_packages_path = get_active_site_packages_path()
         return site_packages_path / package
     except (PackageNotFoundError, ModuleNotFoundError) as err:
         raise QbraidSystemError(f"{package} not found in the current environment.") from err
 
 
-def get_local_package_version(package: str, python_path: Optional[Union[str, Path]] = None) -> str:
-    """Retrieves the local version of a package."""
-    if python_path:
-        try:
-            result = subprocess.run(
-                [
-                    str(python_path),
-                    "-c",
-                    f"import importlib.metadata; print(importlib.metadata.version('{package}'))",
-                ],
-                capture_output=True,
-                text=True,
-                check=True,
-            )
-            return result.stdout.strip()
-        except subprocess.CalledProcessError as err:
-            raise QbraidSystemError(f"{package} not found in the current environment.") from err
-        except FileNotFoundError as err:
-            raise QbraidSystemError(f"Python executable not found at {python_path}.") from err
-
-    try:
-        return version(package)
-    except PackageNotFoundError as err:
-        raise QbraidSystemError(f"{package} not found in the current environment.") from err
-
-
-def get_latest_package_version(package: str, prerelease: bool = False) -> str:
-    """Retrieves the latest version of package from PyPI."""
-    url = f"https://pypi.org/pypi/{package}/json"
-    try:
-        response = requests.get(url, timeout=5)
-        response.raise_for_status()
-    except requests.RequestException as err:
-        raise VersionNotFoundError(
-            f"Failed to retrieve latest {package} version from PyPI."
-        ) from err
-
-    data = response.json()
-
-    if not prerelease:
-        try:
-            return data["info"]["version"]
-        except KeyError as err:
-            raise QbraidSystemError(
-                f"Failed to extract version from {package} package metadata."
-            ) from err
-
-    try:
-        all_versions = list(data["releases"].keys())
-    except KeyError as err:
-        raise QbraidSystemError(
-            f"Failed to extract version from {package} package metadata."
-        ) from err
-
-    if len(all_versions) == 0:
-        raise VersionNotFoundError(f"No versions found for {package}")
-
-    latest_version = all_versions[-1]
-    return latest_version
-
-
 def extract_include_sys_site_pkgs_value(file_path: Union[str, Path]) -> Optional[bool]:
     """Extracts the value of the 'include-system-site-packages' setting from a file."""
     try:
         with open(file_path, "r", encoding="utf-8") as file:
             for line in file:
                 if line.startswith("include-system-site-packages"):
                     parts = line.strip().split("=")
@@ -230,7 +171,56 @@
         with open(file_path, "w", encoding="utf-8") as file:
             file.writelines(lines)
 
     except FileNotFoundError as err:
         raise FileNotFoundError("The specified file was not found.") from err
     except Exception as err:
         raise QbraidSystemError("An error occurred while updating the file") from err
+
+
+def add_config_path_to_site_packages(site_packages_path: Optional[Union[str, Path]] = None) -> None:
+    """
+    Adds the parent directory of the USER_CONFIG_PATH to the Python site-packages
+    via a .pth file, allowing Python to recognize custom modules located in this directory.
+
+    Raises:
+        QbraidSystemError: If the .pth file cannot be written.
+    """
+    directory_path = str(Path(USER_CONFIG_PATH).parent)
+
+    site_packages_path = site_packages_path or get_active_site_packages_path()
+
+    pth_file = Path(site_packages_path) / "qbraid_config.pth"
+
+    try:
+        with open(pth_file, "w", encoding="utf-8") as file:
+            file.write(directory_path + "\n")
+
+        logger.info("Successfully wrote path %s to %s", directory_path, pth_file)
+    except Exception as err:
+        raise QbraidSystemError(f"Failed to write path to {pth_file}.") from err
+
+
+def remove_config_path_from_site_packages(
+    site_packages_path: Optional[Union[str, Path]] = None
+) -> None:
+    """
+    Removes the custom .pth file from the Python site-packages directory,
+    effectively undoing the addition of a custom module directory to Python's search path.
+
+    Raises:
+        FileNotFoundError: If the .pth file does not exist in the site-packages directory.
+        QbraidSystemError: For other unforeseen errors that may occur during file deletion.
+    """
+    site_packages_path = site_packages_path or get_active_site_packages_path()
+
+    pth_file = Path(site_packages_path) / "qbraid_config.pth"
+
+    try:
+        if pth_file.exists():
+            pth_file.unlink()
+            logger.info("Successfully removed %s", pth_file)
+        else:
+            raise FileNotFoundError(f"{pth_file} does not exist.")
+
+    except Exception as err:
+        raise QbraidSystemError(f"Failed to remove {pth_file}.") from err
```

### Comparing `qbraid_core-0.1.4.dev1/qbraid_core/system/threader.py` & `qbraid_core-0.1.4.dev2/qbraid_core/system/threader.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/qbraid_core/system/versions.py` & `qbraid_core-0.1.4.dev2/qbraid_core/system/versions.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,21 +2,25 @@
 # All rights reserved.
 
 """
 Module for extracting version information from package metadata.
 
 """
 
+import importlib.metadata
 import json
 import pathlib
 import re
+import subprocess
 import sys
-from typing import Union
+from typing import Optional, Union
 
-from .exceptions import InvalidVersionError, VersionNotFoundError
+import requests
+
+from .exceptions import InvalidVersionError, QbraidSystemError, VersionNotFoundError
 
 if sys.version_info >= (3, 11):
     import tomllib
 
     MODE = "rb"
 else:
     try:
@@ -32,27 +36,27 @@
     """
     Returns True if given string represents a valid
     semantic version, False otherwise.
 
     """
     try:
         # pylint: disable-next=import-outside-toplevel
-        from packaging import version
+        from packaging.version import InvalidVersion, Version
 
-        version.Version(v)
+        Version(v)
         return True
     except ImportError:
         # Fallback to regex matching if packaging is not installed
         semantic_version_pattern = re.compile(
             r"^(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)"
             r"(-([0-9A-Za-z-]+(\.[0-9A-Za-z-]+)*))?"
             r"(\+([0-9A-Za-z-]+(\.[0-9A-Za-z-]+)*))?$"
         )
         return bool(semantic_version_pattern.match(v))
-    except version.InvalidVersion:
+    except InvalidVersion:
         return False
 
 
 def _get_version_from_json(package_json_path: Union[str, pathlib.Path]) -> str:
     """Get the version from the package.json file."""
     try:
         with open(package_json_path, "r", encoding="utf-8") as file:
@@ -129,7 +133,70 @@
     if shorten_prerelease:
         version = version.replace("-alpha.", "a").replace("-beta.", "b").replace("-rc.", "rc")
 
     if check and not is_valid_semantic_version(version):
         raise InvalidVersionError(f"Invalid semantic version: {version}")
 
     return version
+
+
+def get_latest_package_version(package: str, prerelease: bool = False) -> str:
+    """Retrieves the latest version of package from PyPI."""
+    url = f"https://pypi.org/pypi/{package}/json"
+    try:
+        response = requests.get(url, timeout=5)
+        response.raise_for_status()
+    except requests.RequestException as err:
+        raise VersionNotFoundError(
+            f"Failed to retrieve latest {package} version from PyPI."
+        ) from err
+
+    data = response.json()
+
+    if not prerelease:
+        try:
+            return data["info"]["version"]
+        except KeyError as err:
+            raise QbraidSystemError(
+                f"Failed to extract version from {package} package metadata."
+            ) from err
+
+    try:
+        all_versions = list(data["releases"].keys())
+    except KeyError as err:
+        raise QbraidSystemError(
+            f"Failed to extract version from {package} package metadata."
+        ) from err
+
+    if len(all_versions) == 0:
+        raise VersionNotFoundError(f"No versions found for {package}")
+
+    latest_version = all_versions[-1]
+    return latest_version
+
+
+def get_local_package_version(
+    package: str, python_path: Optional[Union[str, pathlib.Path]] = None
+) -> str:
+    """Retrieves the local version of a package."""
+    if python_path:
+        try:
+            result = subprocess.run(
+                [
+                    str(python_path),
+                    "-c",
+                    f"import importlib.metadata; print(importlib.metadata.version('{package}'))",
+                ],
+                capture_output=True,
+                text=True,
+                check=True,
+            )
+            return result.stdout.strip()
+        except subprocess.CalledProcessError as err:
+            raise QbraidSystemError(f"{package} not found in the current environment.") from err
+        except FileNotFoundError as err:
+            raise QbraidSystemError(f"Python executable not found at {python_path}.") from err
+
+    try:
+        return importlib.metadata.version(package)
+    except importlib.metadata.PackageNotFoundError as err:
+        raise QbraidSystemError(f"{package} not found in the current environment.") from err
```

### Comparing `qbraid_core-0.1.4.dev1/qbraid_core.egg-info/PKG-INFO` & `qbraid_core-0.1.4.dev2/qbraid_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-core
-Version: 0.1.4.dev1
+Version: 0.1.4.dev2
 Summary: Python library with core abstractions for software development in the qBraid ecosystem.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/core/en/latest/
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: urllib3
+Requires-Dist: ipython
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx~=7.2.6; extra == "docs"
```

### Comparing `qbraid_core-0.1.4.dev1/qbraid_core.egg-info/SOURCES.txt` & `qbraid_core-0.1.4.dev2/qbraid_core.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 qbraid_core/services/__init__.py
 qbraid_core/services/admin/__init__.py
 qbraid_core/services/admin/client.py
 qbraid_core/services/environments/__init__.py
 qbraid_core/services/environments/client.py
 qbraid_core/services/environments/create.py
 qbraid_core/services/environments/exceptions.py
+qbraid_core/services/environments/magic.py
 qbraid_core/services/environments/paths.py
 qbraid_core/services/environments/state.py
 qbraid_core/services/environments/validate.py
 qbraid_core/services/quantum/__init__.py
 qbraid_core/services/quantum/adapter.py
 qbraid_core/services/quantum/client.py
 qbraid_core/services/quantum/exceptions.py
@@ -59,14 +60,17 @@
 qbraid_core/system/__init__.py
 qbraid_core/system/exceptions.py
 qbraid_core/system/executables.py
 qbraid_core/system/generic.py
 qbraid_core/system/packages.py
 qbraid_core/system/threader.py
 qbraid_core/system/versions.py
+qbraid_core/system/magic/__init__.py
+qbraid_core/system/magic/manager.py
+qbraid_core/system/magic/qbraid_magic.py
 tests/__init__.py
 tests/environments/__init__.py
 tests/environments/conftest.py
 tests/environments/test_client.py
 tests/environments/test_create.py
 tests/environments/test_paths.py
 tests/environments/test_state.py
```

### Comparing `qbraid_core-0.1.4.dev1/tests/environments/fixtures/environments.py` & `qbraid_core-0.1.4.dev2/tests/environments/fixtures/environments.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/tests/environments/test_client.py` & `qbraid_core-0.1.4.dev2/tests/environments/test_client.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/tests/environments/test_create.py` & `qbraid_core-0.1.4.dev2/tests/environments/test_create.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/tests/environments/test_paths.py` & `qbraid_core-0.1.4.dev2/tests/environments/test_paths.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/tests/environments/test_state.py` & `qbraid_core-0.1.4.dev2/tests/environments/test_state.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/tests/environments/test_validate.py` & `qbraid_core-0.1.4.dev2/tests/environments/test_validate.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/tests/quantum/test_aws_configure.py` & `qbraid_core-0.1.4.dev2/tests/quantum/test_aws_configure.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/tests/quantum/test_proxy.py` & `qbraid_core-0.1.4.dev2/tests/quantum/test_proxy.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/tests/system/test_executables.py` & `qbraid_core-0.1.4.dev2/tests/system/test_executables.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/tests/system/test_generic.py` & `qbraid_core-0.1.4.dev2/tests/system/test_generic.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/tests/system/test_packages.py` & `qbraid_core-0.1.4.dev2/tests/system/test_packages.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 # Copyright (c) 2024, qBraid Development Team
 # All rights reserved.
 
 """
 Unit tests for qBraid core helper functions related to system site-packages.
 
 """
-import sys
 from pathlib import Path
 from unittest.mock import MagicMock, mock_open, patch
 
 import pytest
 
 from qbraid_core.exceptions import QbraidException
 from qbraid_core.system.exceptions import QbraidSystemError
 from qbraid_core.system.packages import (
     extract_include_sys_site_pkgs_value,
     get_active_site_packages_path,
-    get_latest_package_version,
     get_local_package_path,
-    get_local_package_version,
     set_include_sys_site_pkgs_value,
 )
 
 # pylint: disable=unused-argument
 
 
 def test_active_site_pkgs_from_sys_exe():
@@ -116,48 +113,14 @@
 def test_get_local_package_path_error(mock_get_active_site_packages_path):
     """Test get_local_package_path function raises exception when site-packages not found."""
     package_name = "nonexistent_package"
     with pytest.raises(QbraidException):
         get_local_package_path(package_name)
 
 
-def test_get_latest_version_raises():
-    """Test the _get_latest_version function when an error occurs."""
-    with pytest.raises(QbraidException):
-        get_latest_package_version("nonexistent_package")
-
-
-@pytest.mark.parametrize(
-    "package,python_path", [("not_a_package", None), ("not_a_package", sys.executable)]
-)
-def test_get_local_version_raises_for_bad_package(package, python_path):
-    """Test the _get_local_version function when an error occurs."""
-    with pytest.raises(QbraidException) as exc_info:
-        get_local_package_version(package, python_path=python_path)
-    assert f"{package} not found in the current environment." in str(exc_info)
-
-
-def test_get_local_version_raises_for_():
-    """Test the _get_local_version function when an error occurs."""
-    package = "pytest"  # valid package guaranteed to be installed
-    python_path = "/bad/python/path"  # invalid python path
-    with pytest.raises(QbraidException) as exc_info:
-        get_local_package_version(package, python_path=python_path)
-    assert f"Python executable not found at {python_path}." in str(exc_info)
-
-
-@pytest.mark.parametrize("python_path", [None, Path(sys.executable), sys.executable])
-def test_get_local_package_version_alt_python(python_path):
-    """Test the get_latest_package_version function with an alternative Python path."""
-    python_path = Path(sys.executable)
-    with patch("subprocess.run") as mock_run:
-        mock_run.return_value = MagicMock(stdout="2.31.0\n")
-        assert get_local_package_version("requests", python_path=python_path) == "2.31.0"
-
-
 def test_extract_true_value():
     """Test extract_include_sys_site_pkgs_value function with 'true' value."""
     with patch("builtins.open", mock_open(read_data="include-system-site-packages = true")):
         assert extract_include_sys_site_pkgs_value("fake_path") is True
 
 
 def test_extract_false_value():
```

### Comparing `qbraid_core-0.1.4.dev1/tests/system/test_versions.py` & `qbraid_core-0.1.4.dev2/tests/system/test_versions.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,22 +2,26 @@
 # All rights reserved.
 
 """
 Unit tests for qBraid core helper functions related to package versions.
 
 """
 import sys
-from unittest.mock import mock_open, patch
+from pathlib import Path
+from unittest.mock import MagicMock, mock_open, patch
 
 import pytest
 
+from qbraid_core.exceptions import QbraidException
 from qbraid_core.system.exceptions import InvalidVersionError, VersionNotFoundError
 from qbraid_core.system.versions import (
     _simple_toml_version_extractor,
     extract_version,
+    get_latest_package_version,
+    get_local_package_version,
     is_valid_semantic_version,
 )
 
 try:
     if sys.version_info >= (3, 11):
         import tomllib
     else:
@@ -130,7 +134,41 @@
 def test_simple_toml_version_extractor_io_error():
     """Test the _simple_toml_version_extractor function raises VersionNotFoundError when file cannot be read."""
     with patch("builtins.open", side_effect=IOError):
         with pytest.raises(
             VersionNotFoundError, match="An error occurred while reading the TOML file."
         ):
             _simple_toml_version_extractor("pyproject.toml")
+
+
+def test_get_latest_version_raises():
+    """Test the _get_latest_version function when an error occurs."""
+    with pytest.raises(VersionNotFoundError):
+        get_latest_package_version("nonexistent_package")
+
+
+@pytest.mark.parametrize(
+    "package,python_path", [("not_a_package", None), ("not_a_package", sys.executable)]
+)
+def test_get_local_version_raises_for_bad_package(package, python_path):
+    """Test the _get_local_version function when an error occurs."""
+    with pytest.raises(QbraidException) as exc_info:
+        get_local_package_version(package, python_path=python_path)
+    assert f"{package} not found in the current environment." in str(exc_info)
+
+
+def test_get_local_version_raises_for_():
+    """Test the _get_local_version function when an error occurs."""
+    package = "pytest"  # valid package guaranteed to be installed
+    python_path = "/bad/python/path"  # invalid python path
+    with pytest.raises(QbraidException) as exc_info:
+        get_local_package_version(package, python_path=python_path)
+    assert f"Python executable not found at {python_path}." in str(exc_info)
+
+
+@pytest.mark.parametrize("python_path", [None, Path(sys.executable), sys.executable])
+def test_get_local_package_version_alt_python(python_path):
+    """Test the get_latest_package_version function with an alternative Python path."""
+    python_path = Path(sys.executable)
+    with patch("subprocess.run") as mock_run:
+        mock_run.return_value = MagicMock(stdout="2.31.0\n")
+        assert get_local_package_version("requests", python_path=python_path) == "2.31.0"
```

### Comparing `qbraid_core-0.1.4.dev1/tests/top_level/test_client.py` & `qbraid_core-0.1.4.dev2/tests/top_level/test_client.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/tests/top_level/test_compat.py` & `qbraid_core-0.1.4.dev2/tests/top_level/test_compat.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/tests/top_level/test_config.py` & `qbraid_core-0.1.4.dev2/tests/top_level/test_config.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/tests/top_level/test_sessions.py` & `qbraid_core-0.1.4.dev2/tests/top_level/test_sessions.py`

 * *Files identical despite different names*

### Comparing `qbraid_core-0.1.4.dev1/tools/verify_headers.py` & `qbraid_core-0.1.4.dev2/tools/verify_headers.py`

 * *Files identical despite different names*

