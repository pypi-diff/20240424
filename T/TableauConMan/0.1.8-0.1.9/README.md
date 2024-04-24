# Comparing `tmp/TableauConMan-0.1.8.tar.gz` & `tmp/TableauConMan-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TableauConMan-0.1.8.tar", last modified: Thu Oct 26 13:17:41 2023, max compression
+gzip compressed data, was "TableauConMan-0.1.9.tar", last modified: Fri Oct 27 12:37:39 2023, max compression
```

## Comparing `TableauConMan-0.1.8.tar` & `TableauConMan-0.1.9.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-26 13:17:40.999784 TableauConMan-0.1.8/
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/AUTHORS.rst
--rw-rw-rw-   0 root         (0) root         (0)     3589 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/HISTORY.rst
--rw-rw-rw-   0 root         (0) root         (0)     1073 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      311 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      744 2023-10-26 13:17:40.999784 TableauConMan-0.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2763 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-26 13:17:40.990783 TableauConMan-0.1.8/TableauConMan/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/TableauConMan/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14604 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/TableauConMan/api.py
--rw-rw-rw-   0 root         (0) root         (0)     3126 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/TableauConMan/assets_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-26 13:17:40.992783 TableauConMan-0.1.8/TableauConMan/cli/
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/TableauConMan/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/TableauConMan/cli/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      272 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/TableauConMan/cli/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     5277 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/TableauConMan/cli/provisioning.py
--rw-rw-rw-   0 root         (0) root         (0)    11935 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/TableauConMan/data_sources_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     4290 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/TableauConMan/dev.py
--rw-rw-rw-   0 root         (0) root         (0)    10635 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/TableauConMan/group_provisioning.py
--rw-rw-rw-   0 root         (0) root         (0)     9027 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/TableauConMan/groups_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-26 13:17:40.993783 TableauConMan-0.1.8/TableauConMan/helpers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/TableauConMan/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2211 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/TableauConMan/helpers/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3701 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/TableauConMan/plan.py
--rw-rw-rw-   0 root         (0) root         (0)    18937 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/TableauConMan/project_provisioning.py
--rw-rw-rw-   0 root         (0) root         (0)    38071 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/TableauConMan/projects_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-26 13:17:40.994783 TableauConMan-0.1.8/TableauConMan/schemas/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/TableauConMan/schemas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      473 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/TableauConMan/schemas/graphQL_result.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/TableauConMan/schemas/plan.py
--rw-rw-rw-   0 root         (0) root         (0)     6102 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/TableauConMan/schemas/spec.py
--rw-rw-rw-   0 root         (0) root         (0)     2343 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/TableauConMan/server_connector.py
--rw-rw-rw-   0 root         (0) root         (0)     3930 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/TableauConMan/specification.py
--rw-rw-rw-   0 root         (0) root         (0)     3097 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/TableauConMan/update_credentails.py
--rw-rw-rw-   0 root         (0) root         (0)     7418 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/TableauConMan/workbooks_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2123 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/TableauConMan/yaml_connector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-26 13:17:40.991783 TableauConMan-0.1.8/TableauConMan.egg-info/
--rw-r--r--   0 root         (0) root         (0)      744 2023-10-26 13:17:40.000000 TableauConMan-0.1.8/TableauConMan.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1503 2023-10-26 13:17:40.000000 TableauConMan-0.1.8/TableauConMan.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-26 13:17:40.000000 TableauConMan-0.1.8/TableauConMan.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2023-10-26 13:17:40.000000 TableauConMan-0.1.8/TableauConMan.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-26 13:17:40.000000 TableauConMan-0.1.8/TableauConMan.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      247 2023-10-26 13:17:40.000000 TableauConMan-0.1.8/TableauConMan.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-10-26 13:17:40.000000 TableauConMan-0.1.8/TableauConMan.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-26 13:17:40.997784 TableauConMan-0.1.8/docs/
--rw-rw-rw-   0 root         (0) root         (0)      614 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/docs/authors.rst
--rwxrwxrwx   0 root         (0) root         (0)     4859 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/docs/contributing.rst
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/docs/history.rst
--rw-rw-rw-   0 root         (0) root         (0)      310 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1174 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/docs/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)      775 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       97 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/docs/modules.rst
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/docs/readme.rst
--rw-rw-rw-   0 root         (0) root         (0)      142 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/docs/tabpy_ConMan.rst
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/docs/usage.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-26 13:17:40.998783 TableauConMan-0.1.8/requirements/
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/requirements/ci.txt
--rw-rw-rw-   0 root         (0) root         (0)      132 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/requirements/prod.txt
--rw-rw-rw-   0 root         (0) root         (0)       96 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/requirements/test.txt
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-10-26 13:17:41.000784 TableauConMan-0.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2071 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-26 13:17:40.999784 TableauConMan-0.1.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/tests/test_connectors.py
--rw-rw-rw-   0 root         (0) root         (0)     8449 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/tests/test_spec.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1009 2023-10-26 13:17:16.000000 TableauConMan-0.1.8/tests/test_tabpy_ConMan.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-27 12:37:39.501495 TableauConMan-0.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/AUTHORS.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3589 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/HISTORY.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      311 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      744 2023-10-27 12:37:39.501495 TableauConMan-0.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2763 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-27 12:37:39.494161 TableauConMan-0.1.9/TableauConMan/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/TableauConMan/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14604 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/TableauConMan/api.py
+-rw-rw-rw-   0 root         (0) root         (0)     3126 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/TableauConMan/assets_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-27 12:37:39.495995 TableauConMan-0.1.9/TableauConMan/cli/
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/TableauConMan/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/TableauConMan/cli/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      272 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/TableauConMan/cli/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     5277 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/TableauConMan/cli/provisioning.py
+-rw-rw-rw-   0 root         (0) root         (0)    11935 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/TableauConMan/data_sources_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     4290 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/TableauConMan/dev.py
+-rw-rw-rw-   0 root         (0) root         (0)    10635 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/TableauConMan/group_provisioning.py
+-rw-rw-rw-   0 root         (0) root         (0)     9027 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/TableauConMan/groups_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-27 12:37:39.496911 TableauConMan-0.1.9/TableauConMan/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/TableauConMan/helpers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2211 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/TableauConMan/helpers/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4426 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/TableauConMan/plan.py
+-rw-rw-rw-   0 root         (0) root         (0)    18937 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/TableauConMan/project_provisioning.py
+-rw-rw-rw-   0 root         (0) root         (0)    38071 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/TableauConMan/projects_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-27 12:37:39.497828 TableauConMan-0.1.9/TableauConMan/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/TableauConMan/schemas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      473 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/TableauConMan/schemas/graphQL_result.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/TableauConMan/schemas/plan.py
+-rw-rw-rw-   0 root         (0) root         (0)     6102 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/TableauConMan/schemas/spec.py
+-rw-rw-rw-   0 root         (0) root         (0)     2343 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/TableauConMan/server_connector.py
+-rw-rw-rw-   0 root         (0) root         (0)     3930 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/TableauConMan/specification.py
+-rw-rw-rw-   0 root         (0) root         (0)     3097 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/TableauConMan/update_credentails.py
+-rw-rw-rw-   0 root         (0) root         (0)     7418 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/TableauConMan/workbooks_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2123 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/TableauConMan/yaml_connector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-27 12:37:39.495078 TableauConMan-0.1.9/TableauConMan.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      744 2023-10-27 12:37:39.000000 TableauConMan-0.1.9/TableauConMan.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1503 2023-10-27 12:37:39.000000 TableauConMan-0.1.9/TableauConMan.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-27 12:37:39.000000 TableauConMan-0.1.9/TableauConMan.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2023-10-27 12:37:39.000000 TableauConMan-0.1.9/TableauConMan.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-27 12:37:39.000000 TableauConMan-0.1.9/TableauConMan.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      247 2023-10-27 12:37:39.000000 TableauConMan-0.1.9/TableauConMan.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-10-27 12:37:39.000000 TableauConMan-0.1.9/TableauConMan.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-27 12:37:39.499661 TableauConMan-0.1.9/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      614 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/docs/authors.rst
+-rwxrwxrwx   0 root         (0) root         (0)     4859 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/docs/contributing.rst
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/docs/history.rst
+-rw-rw-rw-   0 root         (0) root         (0)      310 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1174 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/docs/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      775 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/docs/modules.rst
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/docs/readme.rst
+-rw-rw-rw-   0 root         (0) root         (0)      142 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/docs/tabpy_ConMan.rst
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/docs/usage.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-27 12:37:39.500578 TableauConMan-0.1.9/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/requirements/ci.txt
+-rw-rw-rw-   0 root         (0) root         (0)      132 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/requirements/prod.txt
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/requirements/test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-10-27 12:37:39.503328 TableauConMan-0.1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2071 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-27 12:37:39.501495 TableauConMan-0.1.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/tests/test_connectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     8449 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/tests/test_spec.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1009 2023-10-27 12:37:14.000000 TableauConMan-0.1.9/tests/test_tabpy_ConMan.py
```

### Comparing `TableauConMan-0.1.8/CONTRIBUTING.rst` & `TableauConMan-0.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `TableauConMan-0.1.8/LICENSE` & `TableauConMan-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `TableauConMan-0.1.8/PKG-INFO` & `TableauConMan-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TableauConMan
-Version: 0.1.8
+Version: 0.1.9
 Summary: UNKNOWN
 Home-page: https://gitlab.com/gitlab-data/TableauConMan
 Author: GitLab data team
 Author-email: analyticsapi@gitlab.com
 License: MIT license
 Keywords: TableauConMan
 Platform: UNKNOWN
```

### Comparing `TableauConMan-0.1.8/README.rst` & `TableauConMan-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `TableauConMan-0.1.8/TableauConMan/api.py` & `TableauConMan-0.1.9/TableauConMan/api.py`

 * *Files identical despite different names*

### Comparing `TableauConMan-0.1.8/TableauConMan/assets_manager.py` & `TableauConMan-0.1.9/TableauConMan/assets_manager.py`

 * *Files identical despite different names*

### Comparing `TableauConMan-0.1.8/TableauConMan/cli/provisioning.py` & `TableauConMan-0.1.9/TableauConMan/cli/provisioning.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -51,16 +51,16 @@
     plan.load_plan(raw_plan.get_yaml())
     logger.info("Loaded plan")
 
     provision_groups(plan)
 
 
 def migrate_datasources(migrate_plan: Plan):
-    logger.info("Processing Datasources")
     datasources = DataSourcesManager(migrate_plan)
+    logger.info("Processing Datasources")
     datasources.populate_datasources()
     logger.info("Populated datasources")
     # logger.debug(datasources.reference_datasources)
 
     datasource_options = datasources.get_datasource_options()
 
     to_update, to_add, to_remove = datasources.get_datasource_changes()
```

### Comparing `TableauConMan-0.1.8/TableauConMan/data_sources_manager.py` & `TableauConMan-0.1.9/TableauConMan/data_sources_manager.py`

 * *Files identical despite different names*

### Comparing `TableauConMan-0.1.8/TableauConMan/dev.py` & `TableauConMan-0.1.9/TableauConMan/dev.py`

 * *Files identical despite different names*

### Comparing `TableauConMan-0.1.8/TableauConMan/group_provisioning.py` & `TableauConMan-0.1.9/TableauConMan/group_provisioning.py`

 * *Files identical despite different names*

### Comparing `TableauConMan-0.1.8/TableauConMan/groups_manager.py` & `TableauConMan-0.1.9/TableauConMan/groups_manager.py`

 * *Files identical despite different names*

### Comparing `TableauConMan-0.1.8/TableauConMan/helpers/utils.py` & `TableauConMan-0.1.9/TableauConMan/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `TableauConMan-0.1.8/TableauConMan/plan.py` & `TableauConMan-0.1.9/TableauConMan/plan.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Module management of provided plans"""
+import os
+
 import tableauserverclient as TSC
 from TableauConMan.server_connector import ServerConnector
 from TableauConMan.yaml_connector import YamlConnector
 from TableauConMan.specification import Specification
-
+from loguru import logger
 
 class Plan:
     """Class for reading and formatting configs and options from the provided plan"""
 
     def __init__(self):
         self.target: str = None
         self.reference: str = None
@@ -24,15 +26,17 @@
 
         :param raw_plan:
         """
         if not isinstance(raw_plan, dict):
             raise TypeError("The raw plan must be a dictionary")
 
         self.target = self.format_connection(raw_plan.get("target"))
+        logger.info(self.target)
         self.reference = self.format_connection(raw_plan.get("reference"))
+        logger.info(self.reference)
         self.target_selection_rules = self.format_rule(
             raw_plan.get("target_selection_rules")
         )
         self.reference_selection_rules = self.format_rule(
             raw_plan.get("reference_selection_rules")
         )
         self.assets = list(raw_plan.get("assets"))
@@ -76,28 +80,35 @@
 
     def format_server(self, connection):
         """
 
         :param connection:
         :return:
         """
-        token_name, token_secret, server_url, site_name = self.get_server_secrets(
+        token_name, token_secret, server_url, site_name = self.get_server_secrets_from_env(
             connection
         )
 
         server = ServerConnector(site_name, server_url, token_name, token_secret)
 
         return server
 
     def format_spec(self, connection):
-        """ """
+        """
 
+        :param connection:
+        :return:
+        """
+        logger.info("connection")
+        logger.info(connection)
         spec_file_path = connection.get("file_path")
 
         raw_spec = YamlConnector(spec_file_path)
+        logger.info("raw_spec")
+        logger.info(raw_spec)
 
         spec = Specification()
         spec.load_spec(raw_spec.get_yaml())
 
         return spec
 
     @staticmethod
@@ -110,14 +121,27 @@
         token_name = server.get("token_name")
         token_secret = server.get("token_secret")
         server_url = server.get("server_url")
         site_name = server.get("site_name")
 
         return token_name, token_secret, server_url, site_name
 
+    def get_server_secrets_from_env(self, server):
+        """
+
+        :param server:
+        :return:
+        """
+        token_name = os.environ.get(server.get("token_name"))
+        token_secret = os.environ.get(server.get("token_secret"))
+        server_url = os.environ.get(server.get("server_url"))
+        site_name = os.environ.get(server.get("site_name"))
+
+        return token_name, token_secret, server_url, site_name
+
     @staticmethod
     def get_connection_secretes(connection):
         """
 
         :param connection:
         :return:
         """
```

### Comparing `TableauConMan-0.1.8/TableauConMan/project_provisioning.py` & `TableauConMan-0.1.9/TableauConMan/project_provisioning.py`

 * *Files identical despite different names*

### Comparing `TableauConMan-0.1.8/TableauConMan/projects_manager.py` & `TableauConMan-0.1.9/TableauConMan/projects_manager.py`

 * *Files identical despite different names*

### Comparing `TableauConMan-0.1.8/TableauConMan/schemas/spec.py` & `TableauConMan-0.1.9/TableauConMan/schemas/spec.py`

 * *Files identical despite different names*

### Comparing `TableauConMan-0.1.8/TableauConMan/server_connector.py` & `TableauConMan-0.1.9/TableauConMan/server_connector.py`

 * *Files identical despite different names*

### Comparing `TableauConMan-0.1.8/TableauConMan/specification.py` & `TableauConMan-0.1.9/TableauConMan/specification.py`

 * *Files identical despite different names*

### Comparing `TableauConMan-0.1.8/TableauConMan/update_credentails.py` & `TableauConMan-0.1.9/TableauConMan/update_credentails.py`

 * *Files identical despite different names*

### Comparing `TableauConMan-0.1.8/TableauConMan/workbooks_manager.py` & `TableauConMan-0.1.9/TableauConMan/workbooks_manager.py`

 * *Files identical despite different names*

### Comparing `TableauConMan-0.1.8/TableauConMan/yaml_connector.py` & `TableauConMan-0.1.9/TableauConMan/yaml_connector.py`

 * *Files identical despite different names*

### Comparing `TableauConMan-0.1.8/TableauConMan.egg-info/PKG-INFO` & `TableauConMan-0.1.9/TableauConMan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TableauConMan
-Version: 0.1.8
+Version: 0.1.9
 Summary: UNKNOWN
 Home-page: https://gitlab.com/gitlab-data/TableauConMan
 Author: GitLab data team
 Author-email: analyticsapi@gitlab.com
 License: MIT license
 Keywords: TableauConMan
 Platform: UNKNOWN
```

### Comparing `TableauConMan-0.1.8/TableauConMan.egg-info/SOURCES.txt` & `TableauConMan-0.1.9/TableauConMan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TableauConMan-0.1.8/docs/Makefile` & `TableauConMan-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `TableauConMan-0.1.8/docs/conf.py` & `TableauConMan-0.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `TableauConMan-0.1.8/docs/installation.rst` & `TableauConMan-0.1.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `TableauConMan-0.1.8/docs/make.bat` & `TableauConMan-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `TableauConMan-0.1.8/setup.py` & `TableauConMan-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `TableauConMan-0.1.8/tests/test_connectors.py` & `TableauConMan-0.1.9/tests/test_connectors.py`

 * *Files identical despite different names*

### Comparing `TableauConMan-0.1.8/tests/test_spec.yaml` & `TableauConMan-0.1.9/tests/test_spec.yaml`

 * *Files identical despite different names*

### Comparing `TableauConMan-0.1.8/tests/test_tabpy_ConMan.py` & `TableauConMan-0.1.9/tests/test_tabpy_ConMan.py`

 * *Files identical despite different names*

