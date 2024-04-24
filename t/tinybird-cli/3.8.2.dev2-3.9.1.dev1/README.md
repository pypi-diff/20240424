# Comparing `tmp/tinybird-cli-3.8.2.dev2.tar.gz` & `tmp/tinybird-cli-3.9.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinybird-cli-3.8.2.dev2.tar", last modified: Thu Apr 18 13:33:49 2024, max compression
+gzip compressed data, was "tinybird-cli-3.9.1.dev1.tar", last modified: Wed Apr 24 06:19:04 2024, max compression
```

## Comparing `tinybird-cli-3.8.2.dev2.tar` & `tinybird-cli-3.9.1.dev1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 13:33:49.780388 tinybird-cli-3.8.2.dev2/
--rw-r--r--   0 root         (0) root         (0)    68437 2024-04-18 13:33:49.779389 tinybird-cli-3.8.2.dev2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 13:33:49.780388 tinybird-cli-3.8.2.dev2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 13:33:49.777388 tinybird-cli-3.8.2.dev2/tinybird/
--rw-rw-rw-   0 root         (0) root         (0)      254 2024-04-18 13:33:48.000000 tinybird-cli-3.8.2.dev2/tinybird/__cli__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 13:33:49.777388 tinybird-cli-3.8.2.dev2/tinybird/ch_utils/
--rw-rw-rw-   0 root         (0) root         (0)     3657 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/ch_utils/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    39699 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/ch_utils/engine.py
--rw-rw-rw-   0 root         (0) root         (0)      975 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/check_pypi.py
--rw-rw-rw-   0 root         (0) root         (0)    46735 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/client.py
--rw-rw-rw-   0 root         (0) root         (0)     2003 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/config.py
--rw-rw-rw-   0 root         (0) root         (0)    15244 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/connectors.py
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/context.py
--rw-rw-rw-   0 root         (0) root         (0)   212510 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/datafile.py
--rw-rw-rw-   0 root         (0) root         (0)     7060 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/datatypes.py
--rw-rw-rw-   0 root         (0) root         (0)    59114 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/feedback_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     4707 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/git_settings.py
--rw-rw-rw-   0 root         (0) root         (0)    41181 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/sql.py
--rw-rw-rw-   0 root         (0) root         (0)    80819 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/sql_template.py
--rw-rw-rw-   0 root         (0) root         (0)    10196 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/sql_template_fmt.py
--rw-rw-rw-   0 root         (0) root         (0)    11568 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/sql_toolset.py
--rw-rw-rw-   0 root         (0) root         (0)    27763 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/syncasync.py
--rw-rw-rw-   0 root         (0) root         (0)      674 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/tb_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 13:33:49.779389 tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/
--rw-rw-rw-   0 root         (0) root         (0)     8601 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    37863 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/branch.py
--rw-rw-rw-   0 root         (0) root         (0)    14087 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/cicd.py
--rw-rw-rw-   0 root         (0) root         (0)    64868 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    78344 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/common.py
--rw-rw-rw-   0 root         (0) root         (0)    11484 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/config.py
--rw-rw-rw-   0 root         (0) root         (0)    30927 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/connection.py
--rw-rw-rw-   0 root         (0) root         (0)    31944 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/datasource.py
--rw-rw-rw-   0 root         (0) root         (0)     3367 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2964 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/job.py
--rw-rw-rw-   0 root         (0) root         (0)    26155 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/pipe.py
--rw-rw-rw-   0 root         (0) root         (0)     2010 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/regions.py
--rw-rw-rw-   0 root         (0) root         (0)    10490 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/telemetry.py
--rw-rw-rw-   0 root         (0) root         (0)     4223 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 13:33:49.779389 tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/tinyunit/
--rw-rw-rw-   0 root         (0) root         (0)    11667 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/tinyunit/tinyunit.py
--rw-rw-rw-   0 root         (0) root         (0)     1868 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py
--rw-rw-rw-   0 root         (0) root         (0)     4383 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/token.py
--rw-rw-rw-   0 root         (0) root         (0)    10081 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/workspace.py
--rw-rw-rw-   0 root         (0) root         (0)     8268 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/workspace_members.py
--rw-rw-rw-   0 root         (0) root         (0)    41982 2024-04-18 13:33:43.000000 tinybird-cli-3.8.2.dev2/tinybird/tornado_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 13:33:49.779389 tinybird-cli-3.8.2.dev2/tinybird_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)    68437 2024-04-18 13:33:49.000000 tinybird-cli-3.8.2.dev2/tinybird_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1348 2024-04-18 13:33:49.000000 tinybird-cli-3.8.2.dev2/tinybird_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 13:33:49.000000 tinybird-cli-3.8.2.dev2/tinybird_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-04-18 13:33:49.000000 tinybird-cli-3.8.2.dev2/tinybird_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      732 2024-04-18 13:33:49.000000 tinybird-cli-3.8.2.dev2/tinybird_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       45 2024-04-18 13:33:49.000000 tinybird-cli-3.8.2.dev2/tinybird_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:19:04.494391 tinybird-cli-3.9.1.dev1/
+-rw-r--r--   0 root         (0) root         (0)    68385 2024-04-24 06:19:04.493391 tinybird-cli-3.9.1.dev1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 06:19:04.494391 tinybird-cli-3.9.1.dev1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:19:04.491391 tinybird-cli-3.9.1.dev1/tinybird/
+-rw-rw-rw-   0 root         (0) root         (0)      254 2024-04-24 06:19:03.000000 tinybird-cli-3.9.1.dev1/tinybird/__cli__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:19:04.491391 tinybird-cli-3.9.1.dev1/tinybird/ch_utils/
+-rw-rw-rw-   0 root         (0) root         (0)     3657 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/ch_utils/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    39699 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/ch_utils/engine.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/check_pypi.py
+-rw-rw-rw-   0 root         (0) root         (0)    46735 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2003 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15244 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/connectors.py
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/context.py
+-rw-rw-rw-   0 root         (0) root         (0)   212510 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/datafile.py
+-rw-rw-rw-   0 root         (0) root         (0)     7060 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/datatypes.py
+-rw-rw-rw-   0 root         (0) root         (0)    59114 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/feedback_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     4707 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/git_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    41181 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/sql.py
+-rw-rw-rw-   0 root         (0) root         (0)    81435 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/sql_template.py
+-rw-rw-rw-   0 root         (0) root         (0)    10196 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/sql_template_fmt.py
+-rw-rw-rw-   0 root         (0) root         (0)    11568 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/sql_toolset.py
+-rw-rw-rw-   0 root         (0) root         (0)    27763 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/syncasync.py
+-rw-rw-rw-   0 root         (0) root         (0)      674 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:19:04.493391 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/
+-rw-rw-rw-   0 root         (0) root         (0)     8601 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    37863 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/branch.py
+-rw-rw-rw-   0 root         (0) root         (0)    14087 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/cicd.py
+-rw-rw-rw-   0 root         (0) root         (0)    64868 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    78344 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/common.py
+-rw-rw-rw-   0 root         (0) root         (0)    11484 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    30927 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)    31944 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/datasource.py
+-rw-rw-rw-   0 root         (0) root         (0)     3367 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2964 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/job.py
+-rw-rw-rw-   0 root         (0) root         (0)    26155 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/pipe.py
+-rw-rw-rw-   0 root         (0) root         (0)     2010 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/regions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10490 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/telemetry.py
+-rw-rw-rw-   0 root         (0) root         (0)     4223 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:19:04.493391 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/tinyunit/
+-rw-rw-rw-   0 root         (0) root         (0)    11667 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/tinyunit/tinyunit.py
+-rw-rw-rw-   0 root         (0) root         (0)     1868 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     4383 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/token.py
+-rw-rw-rw-   0 root         (0) root         (0)    10081 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/workspace.py
+-rw-rw-rw-   0 root         (0) root         (0)     8268 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/workspace_members.py
+-rw-rw-rw-   0 root         (0) root         (0)    41982 2024-04-24 06:18:59.000000 tinybird-cli-3.9.1.dev1/tinybird/tornado_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 06:19:04.493391 tinybird-cli-3.9.1.dev1/tinybird_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    68385 2024-04-24 06:19:04.000000 tinybird-cli-3.9.1.dev1/tinybird_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1348 2024-04-24 06:19:04.000000 tinybird-cli-3.9.1.dev1/tinybird_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 06:19:04.000000 tinybird-cli-3.9.1.dev1/tinybird_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-24 06:19:04.000000 tinybird-cli-3.9.1.dev1/tinybird_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      732 2024-04-24 06:19:04.000000 tinybird-cli-3.9.1.dev1/tinybird_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2024-04-24 06:19:04.000000 tinybird-cli-3.9.1.dev1/tinybird_cli.egg-info/top_level.txt
```

### Comparing `tinybird-cli-3.8.2.dev2/PKG-INFO` & `tinybird-cli-3.9.1.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinybird-cli
-Version: 3.8.2.dev2
+Version: 3.9.1.dev1
 Summary: Tinybird Command Line Tool
 Home-page: https://www.tinybird.co/docs/cli/introduction.html
 Author: Tinybird
 Author-email: support@tinybird.co
 Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/x-rst
 Provides-Extra: bigquery
@@ -14,27 +14,19 @@
 =============
 
 The Tinybird command-line tool allows you to use all the Tinybird functionality directly from the command line. Additionally, it includes several functions to create and manage data projects easily.
 
 Changelog
 ---------
 
-3.8.2.dev2
-************
-
-- `Added` New `--policy` option for `create s3_iamrole` command that will generate different hints depending on the case
-
-3.8.2.dev1
+3.9.0
 ************
 
 - `Added` Support for connection names when doing `tb connection rm`
-
-3.8.1
-************
-
+- `Added` New `--policy` option for `create s3_iamrole` command that will generate different hints depending on the case
 - `Fixed` Avoid system vars evaluation when doing `tb fmt`
 - `Fixed` environment variables substitution for Data Source engine parameters.
 
 
 3.8.0
 ************
```

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/ch_utils/constants.py` & `tinybird-cli-3.9.1.dev1/tinybird/ch_utils/constants.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/ch_utils/engine.py` & `tinybird-cli-3.9.1.dev1/tinybird/ch_utils/engine.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/check_pypi.py` & `tinybird-cli-3.9.1.dev1/tinybird/check_pypi.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/client.py` & `tinybird-cli-3.9.1.dev1/tinybird/client.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/config.py` & `tinybird-cli-3.9.1.dev1/tinybird/config.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/connectors.py` & `tinybird-cli-3.9.1.dev1/tinybird/connectors.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/context.py` & `tinybird-cli-3.9.1.dev1/tinybird/context.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/datafile.py` & `tinybird-cli-3.9.1.dev1/tinybird/datafile.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/datatypes.py` & `tinybird-cli-3.9.1.dev1/tinybird/datatypes.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/feedback_manager.py` & `tinybird-cli-3.9.1.dev1/tinybird/feedback_manager.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/git_settings.py` & `tinybird-cli-3.9.1.dev1/tinybird/git_settings.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/sql.py` & `tinybird-cli-3.9.1.dev1/tinybird/sql.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/sql_template.py` & `tinybird-cli-3.9.1.dev1/tinybird/sql_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1558,15 +1558,28 @@
                 )
                 is_reserved_name = node.id in reserved_vars or node.id in function_list or node.id in _namespace
                 if (not isinstance(node.parent, ast.Call) and not is_cast) and not is_reserved_name:
                     vars[node.id] = {"type": "String", "default": None}
 
         return vars
 
-    parsed = ast.parse(content)
+    def parse_content(content, retries=0):
+        try:
+            parsed = ast.parse(content)
+            return parsed
+        except Exception as e:
+            if "AST constructor recursion depth mismatch" not in str(e):
+                raise e
+            retries += 1
+            if retries > 3:
+                raise e
+            return parse_content(content, retries)
+
+    parsed = parse_content(content)
+
     # calculate parents for each node for later checks
     for node in ast.walk(parsed):
         for child in ast.iter_child_nodes(node):
             child.parent = node
     vars = _w(parsed)
 
     return [dict(name=k, **v) for k, v in vars.items()]
@@ -1996,14 +2009,18 @@
     ("%  SELECT test as aa, ['1','2'] as test, '1,,,2' as a ", {})
     >>> render_sql_template("% {% if defined(test) %}{% set _groupByCSV = ','.join(test) %} SELECT test as aa, {{Array(test, 'String')}} as test, {{_groupByCSV}} as a {% end %}", {"test": ["1","2"]})
     ("%  SELECT test as aa, ['1','2'] as test, '1,2' as a ", {})
     >>> render_sql_template("% {% if defined(test) %}{% set _total = sum(test) %} SELECT test as aa, {{Array(test, 'Int32')}} as test, {{_total}} as a {% end %}", {"test": "1,2"})
     Traceback (most recent call last):
     ...
     ValueError: unsupported operand type(s) for +: 'int' and 'str'
+    >>> render_sql_template("% SELECT {% if defined(x) %} x, 1", preprocess_variables_flag=True)
+    Traceback (most recent call last):
+    ...
+    tinybird.tornado_template.UnClosedIfError: Missing {% end %} block for if at line 1
     """
 
     t, template_variables = get_template_and_variables(sql, name)
 
     if preprocess_variables_flag and variables is not None:
         processed_variables = preprocess_variables(variables, t)
         variables.update(processed_variables)
```

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/sql_template_fmt.py` & `tinybird-cli-3.9.1.dev1/tinybird/sql_template_fmt.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/sql_toolset.py` & `tinybird-cli-3.9.1.dev1/tinybird/sql_toolset.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/syncasync.py` & `tinybird-cli-3.9.1.dev1/tinybird/syncasync.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/tb_cli.py` & `tinybird-cli-3.9.1.dev1/tinybird/tb_cli.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/auth.py` & `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/auth.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/branch.py` & `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/branch.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/cicd.py` & `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/cicd.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/cli.py` & `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/cli.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/common.py` & `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/common.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/config.py` & `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/config.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/connection.py` & `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/connection.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/datasource.py` & `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/datasource.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/exceptions.py` & `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/exceptions.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/job.py` & `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/job.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/pipe.py` & `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/pipe.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/regions.py` & `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/regions.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/telemetry.py` & `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/telemetry.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/test.py` & `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/test.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/tinyunit/tinyunit.py` & `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/tinyunit/tinyunit.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py` & `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/token.py` & `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/token.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/workspace.py` & `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/workspace.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/tb_cli_modules/workspace_members.py` & `tinybird-cli-3.9.1.dev1/tinybird/tb_cli_modules/workspace_members.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird/tornado_template.py` & `tinybird-cli-3.9.1.dev1/tinybird/tornado_template.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird_cli.egg-info/PKG-INFO` & `tinybird-cli-3.9.1.dev1/tinybird_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinybird-cli
-Version: 3.8.2.dev2
+Version: 3.9.1.dev1
 Summary: Tinybird Command Line Tool
 Home-page: https://www.tinybird.co/docs/cli/introduction.html
 Author: Tinybird
 Author-email: support@tinybird.co
 Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/x-rst
 Provides-Extra: bigquery
@@ -14,27 +14,19 @@
 =============
 
 The Tinybird command-line tool allows you to use all the Tinybird functionality directly from the command line. Additionally, it includes several functions to create and manage data projects easily.
 
 Changelog
 ---------
 
-3.8.2.dev2
-************
-
-- `Added` New `--policy` option for `create s3_iamrole` command that will generate different hints depending on the case
-
-3.8.2.dev1
+3.9.0
 ************
 
 - `Added` Support for connection names when doing `tb connection rm`
-
-3.8.1
-************
-
+- `Added` New `--policy` option for `create s3_iamrole` command that will generate different hints depending on the case
 - `Fixed` Avoid system vars evaluation when doing `tb fmt`
 - `Fixed` environment variables substitution for Data Source engine parameters.
 
 
 3.8.0
 ************
```

### Comparing `tinybird-cli-3.8.2.dev2/tinybird_cli.egg-info/SOURCES.txt` & `tinybird-cli-3.9.1.dev1/tinybird_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.8.2.dev2/tinybird_cli.egg-info/requires.txt` & `tinybird-cli-3.9.1.dev1/tinybird_cli.egg-info/requires.txt`

 * *Files identical despite different names*

