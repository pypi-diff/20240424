# Comparing `tmp/abst-2.3.8.tar.gz` & `tmp/abst-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abst-2.3.8.tar", last modified: Tue Nov 21 11:14:29 2023, max compression
+gzip compressed data, was "abst-2.3.9.tar", last modified: Tue Nov 21 12:44:20 2023, max compression
```

## Comparing `abst-2.3.8.tar` & `abst-2.3.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:14:29.878259 abst-2.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-11-21 11:14:17.000000 abst-2.3.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2023-11-21 11:14:29.878259 abst-2.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2023-11-21 11:14:17.000000 abst-2.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:14:29.870259 abst-2.3.8/abst/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 11:14:17.000000 abst-2.3.8/abst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2023-11-21 11:14:17.000000 abst-2.3.8/abst/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:14:29.874259 abst-2.3.8/abst/bastion_support/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 11:14:17.000000 abst-2.3.8/abst/bastion_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6764 2023-11-21 11:14:17.000000 abst-2.3.8/abst/bastion_support/bastion_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    28047 2023-11-21 11:14:17.000000 abst-2.3.8/abst/bastion_support/oci_bastion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2023-11-21 11:14:17.000000 abst-2.3.8/abst/cfg_func.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:14:29.874259 abst-2.3.8/abst/cli_commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 11:14:17.000000 abst-2.3.8/abst/cli_commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:14:29.874259 abst-2.3.8/abst/cli_commands/config_cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 11:14:17.000000 abst-2.3.8/abst/cli_commands/config_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2023-11-21 11:14:17.000000 abst-2.3.8/abst/cli_commands/config_cli/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:14:29.874259 abst-2.3.8/abst/cli_commands/context/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 11:14:17.000000 abst-2.3.8/abst/cli_commands/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2023-11-21 11:14:17.000000 abst-2.3.8/abst/cli_commands/context/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:14:29.874259 abst-2.3.8/abst/cli_commands/cp_cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 11:14:17.000000 abst-2.3.8/abst/cli_commands/cp_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2023-11-21 11:14:17.000000 abst-2.3.8/abst/cli_commands/cp_cli/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:14:29.874259 abst-2.3.8/abst/cli_commands/create_cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 11:14:17.000000 abst-2.3.8/abst/cli_commands/create_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2023-11-21 11:14:17.000000 abst-2.3.8/abst/cli_commands/create_cli/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:14:29.874259 abst-2.3.8/abst/cli_commands/helm_cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 11:14:17.000000 abst-2.3.8/abst/cli_commands/helm_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2023-11-21 11:14:17.000000 abst-2.3.8/abst/cli_commands/helm_cli/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:14:29.874259 abst-2.3.8/abst/cli_commands/kubectl_cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 11:14:17.000000 abst-2.3.8/abst/cli_commands/kubectl_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2023-11-21 11:14:17.000000 abst-2.3.8/abst/cli_commands/kubectl_cli/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:14:29.874259 abst-2.3.8/abst/cli_commands/parallel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 11:14:17.000000 abst-2.3.8/abst/cli_commands/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2023-11-21 11:14:17.000000 abst-2.3.8/abst/cli_commands/parallel/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2023-11-21 11:14:17.000000 abst-2.3.8/abst/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2023-11-21 11:14:17.000000 abst-2.3.8/abst/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2023-11-21 11:14:17.000000 abst-2.3.8/abst/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:14:29.874259 abst-2.3.8/abst/notifier/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 11:14:17.000000 abst-2.3.8/abst/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2023-11-21 11:14:17.000000 abst-2.3.8/abst/notifier/version_notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2023-11-21 11:14:17.000000 abst-2.3.8/abst/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:14:29.878259 abst-2.3.8/abst/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 11:14:17.000000 abst-2.3.8/abst/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2023-11-21 11:14:17.000000 abst-2.3.8/abst/utils/misc_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2023-11-21 11:14:17.000000 abst-2.3.8/abst/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:14:29.878259 abst-2.3.8/abst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2023-11-21 11:14:29.000000 abst-2.3.8/abst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2023-11-21 11:14:29.000000 abst-2.3.8/abst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 11:14:29.000000 abst-2.3.8/abst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-11-21 11:14:29.000000 abst-2.3.8/abst.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-11-21 11:14:29.000000 abst-2.3.8/abst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-21 11:14:29.000000 abst-2.3.8/abst.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 11:14:29.000000 abst-2.3.8/abst.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-21 11:14:29.878259 abst-2.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2023-11-21 11:14:17.000000 abst-2.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 11:14:29.878259 abst-2.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2023-11-21 11:14:17.000000 abst-2.3.8/tests/test_sample_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 12:44:20.239627 abst-2.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-11-21 12:44:08.000000 abst-2.3.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2023-11-21 12:44:20.239627 abst-2.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2023-11-21 12:44:08.000000 abst-2.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 12:44:20.235628 abst-2.3.9/abst/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 12:44:08.000000 abst-2.3.9/abst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2023-11-21 12:44:08.000000 abst-2.3.9/abst/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 12:44:20.235628 abst-2.3.9/abst/bastion_support/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 12:44:08.000000 abst-2.3.9/abst/bastion_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6764 2023-11-21 12:44:08.000000 abst-2.3.9/abst/bastion_support/bastion_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28047 2023-11-21 12:44:08.000000 abst-2.3.9/abst/bastion_support/oci_bastion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2023-11-21 12:44:08.000000 abst-2.3.9/abst/cfg_func.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 12:44:20.235628 abst-2.3.9/abst/cli_commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 12:44:08.000000 abst-2.3.9/abst/cli_commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 12:44:20.235628 abst-2.3.9/abst/cli_commands/config_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 12:44:08.000000 abst-2.3.9/abst/cli_commands/config_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2023-11-21 12:44:08.000000 abst-2.3.9/abst/cli_commands/config_cli/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 12:44:20.235628 abst-2.3.9/abst/cli_commands/context/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 12:44:08.000000 abst-2.3.9/abst/cli_commands/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2023-11-21 12:44:08.000000 abst-2.3.9/abst/cli_commands/context/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 12:44:20.239627 abst-2.3.9/abst/cli_commands/cp_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 12:44:08.000000 abst-2.3.9/abst/cli_commands/cp_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2023-11-21 12:44:08.000000 abst-2.3.9/abst/cli_commands/cp_cli/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 12:44:20.239627 abst-2.3.9/abst/cli_commands/create_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 12:44:08.000000 abst-2.3.9/abst/cli_commands/create_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2023-11-21 12:44:08.000000 abst-2.3.9/abst/cli_commands/create_cli/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 12:44:20.239627 abst-2.3.9/abst/cli_commands/helm_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 12:44:08.000000 abst-2.3.9/abst/cli_commands/helm_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2023-11-21 12:44:08.000000 abst-2.3.9/abst/cli_commands/helm_cli/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 12:44:20.239627 abst-2.3.9/abst/cli_commands/kubectl_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 12:44:08.000000 abst-2.3.9/abst/cli_commands/kubectl_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2023-11-21 12:44:08.000000 abst-2.3.9/abst/cli_commands/kubectl_cli/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 12:44:20.239627 abst-2.3.9/abst/cli_commands/parallel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 12:44:08.000000 abst-2.3.9/abst/cli_commands/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2023-11-21 12:44:08.000000 abst-2.3.9/abst/cli_commands/parallel/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2023-11-21 12:44:08.000000 abst-2.3.9/abst/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2023-11-21 12:44:08.000000 abst-2.3.9/abst/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2023-11-21 12:44:08.000000 abst-2.3.9/abst/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 12:44:20.239627 abst-2.3.9/abst/notifier/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 12:44:08.000000 abst-2.3.9/abst/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2023-11-21 12:44:08.000000 abst-2.3.9/abst/notifier/version_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2023-11-21 12:44:08.000000 abst-2.3.9/abst/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 12:44:20.239627 abst-2.3.9/abst/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 12:44:08.000000 abst-2.3.9/abst/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2023-11-21 12:44:08.000000 abst-2.3.9/abst/utils/misc_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2023-11-21 12:44:08.000000 abst-2.3.9/abst/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 12:44:20.239627 abst-2.3.9/abst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2023-11-21 12:44:20.000000 abst-2.3.9/abst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2023-11-21 12:44:20.000000 abst-2.3.9/abst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 12:44:20.000000 abst-2.3.9/abst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2023-11-21 12:44:20.000000 abst-2.3.9/abst.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2023-11-21 12:44:20.000000 abst-2.3.9/abst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-21 12:44:20.000000 abst-2.3.9/abst.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 12:44:20.000000 abst-2.3.9/abst.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-21 12:44:20.239627 abst-2.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2023-11-21 12:44:08.000000 abst-2.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 12:44:20.239627 abst-2.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2023-11-21 12:44:08.000000 abst-2.3.9/tests/test_sample_dict.py
```

### Comparing `abst-2.3.8/LICENSE.md` & `abst-2.3.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `abst-2.3.8/PKG-INFO` & `abst-2.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abst
-Version: 2.3.8
+Version: 2.3.9
 Summary: CLI Command making OCI Bastion and kubernetes usage simple and fast
 Home-page: https://github.com/jiri-otoupal/abst
 Author: Jiri Otoupal
 Author-email: jiri-otoupal@ips-database.eu
 License: MIT
 Keywords: Auto OCI Bastion
 Classifier: Development Status :: 4 - Beta
```

### Comparing `abst-2.3.8/README.md` & `abst-2.3.9/README.md`

 * *Files identical despite different names*

### Comparing `abst-2.3.8/abst/bastion_support/bastion_scheduler.py` & `abst-2.3.9/abst/bastion_support/bastion_scheduler.py`

 * *Files identical despite different names*

### Comparing `abst-2.3.8/abst/bastion_support/oci_bastion.py` & `abst-2.3.9/abst/bastion_support/oci_bastion.py`

 * *Files identical despite different names*

### Comparing `abst-2.3.8/abst/cfg_func.py` & `abst-2.3.9/abst/cfg_func.py`

 * *Files identical despite different names*

### Comparing `abst-2.3.8/abst/cli_commands/config_cli/commands.py` & `abst-2.3.9/abst/cli_commands/config_cli/commands.py`

 * *Files identical despite different names*

### Comparing `abst-2.3.8/abst/cli_commands/context/commands.py` & `abst-2.3.9/abst/cli_commands/context/commands.py`

 * *Files identical despite different names*

### Comparing `abst-2.3.8/abst/cli_commands/cp_cli/commands.py` & `abst-2.3.9/abst/cli_commands/cp_cli/commands.py`

 * *Files identical despite different names*

### Comparing `abst-2.3.8/abst/cli_commands/create_cli/commands.py` & `abst-2.3.9/abst/cli_commands/create_cli/commands.py`

 * *Files identical despite different names*

### Comparing `abst-2.3.8/abst/cli_commands/helm_cli/commands.py` & `abst-2.3.9/abst/cli_commands/helm_cli/commands.py`

 * *Files identical despite different names*

### Comparing `abst-2.3.8/abst/cli_commands/kubectl_cli/commands.py` & `abst-2.3.9/abst/cli_commands/kubectl_cli/commands.py`

 * *Files identical despite different names*

### Comparing `abst-2.3.8/abst/cli_commands/parallel/commands.py` & `abst-2.3.9/abst/cli_commands/parallel/commands.py`

 * *Files identical despite different names*

### Comparing `abst-2.3.8/abst/config.py` & `abst-2.3.9/abst/config.py`

 * *Files identical despite different names*

### Comparing `abst-2.3.8/abst/dialogs.py` & `abst-2.3.9/abst/dialogs.py`

 * *Files identical despite different names*

### Comparing `abst-2.3.8/abst/main.py` & `abst-2.3.9/abst/main.py`

 * *Files identical despite different names*

### Comparing `abst-2.3.8/abst/notifier/version_notifier.py` & `abst-2.3.9/abst/notifier/version_notifier.py`

 * *Files identical despite different names*

### Comparing `abst-2.3.8/abst/tools.py` & `abst-2.3.9/abst/tools.py`

 * *Files identical despite different names*

### Comparing `abst-2.3.8/abst/utils/misc_funcs.py` & `abst-2.3.9/abst/utils/misc_funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,16 @@
 
 
 def copy_file_alt_kubectl(data: list, dest_path: str, local_path: Path, pod_name_precise: str, tries=4):
     kubectl_alt_copy_cmd = (f"cat \"{local_path}\" |"
                             f" kubectl exec -i {pod_name_precise} -n {data[0]} -- tee \"{dest_path}\" > /dev/null")
     logging.info(f"Executing {kubectl_alt_copy_cmd}")
     exit_code = subprocess.call(kubectl_alt_copy_cmd, shell=True)
-    rich.print(f"   [green]{local_path.name} ({local_path.stat().st_size / 1000} kB) successfully copied![/green]")
+    rich.print(
+        f"   [green]{local_path if type(local_path) == str else local_path.name} ({local_path.stat().st_size / 1000} kB) successfully copied![/green]")
     if exit_code != 0 and tries < 0:
         rich.print("[red]Failed to copy.[/red]")
         exit(1)
     elif exit_code != 0 and tries > 0:
         rich.print(f"Failed to copy will try again, try {tries}/4")
         sleep(5)
         copy_file_alt_kubectl(data, dest_path, local_path, pod_name_precise, tries - 1)
```

### Comparing `abst-2.3.8/abst/wrappers.py` & `abst-2.3.9/abst/wrappers.py`

 * *Files identical despite different names*

### Comparing `abst-2.3.8/abst.egg-info/PKG-INFO` & `abst-2.3.9/abst.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abst
-Version: 2.3.8
+Version: 2.3.9
 Summary: CLI Command making OCI Bastion and kubernetes usage simple and fast
 Home-page: https://github.com/jiri-otoupal/abst
 Author: Jiri Otoupal
 Author-email: jiri-otoupal@ips-database.eu
 License: MIT
 Keywords: Auto OCI Bastion
 Classifier: Development Status :: 4 - Beta
```

### Comparing `abst-2.3.8/abst.egg-info/SOURCES.txt` & `abst-2.3.9/abst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `abst-2.3.8/setup.py` & `abst-2.3.9/setup.py`

 * *Files identical despite different names*

