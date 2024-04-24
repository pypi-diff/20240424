# Comparing `tmp/mypy-boto3-ssm-1.34.61.tar.gz` & `tmp/mypy_boto3_ssm-1.34.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ssm-1.34.61.tar", last modified: Tue Mar 12 19:21:13 2024, max compression
+gzip compressed data, was "mypy_boto3_ssm-1.34.91.tar", last modified: Wed Apr 24 19:19:07 2024, max compression
```

## Comparing `mypy-boto3-ssm-1.34.61.tar` & `mypy_boto3_ssm-1.34.91.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:21:13.915058 mypy-boto3-ssm-1.34.61/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-12 19:20:55.000000 mypy-boto3-ssm-1.34.61/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21097 2024-03-12 19:21:13.915058 mypy-boto3-ssm-1.34.61/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19558 2024-03-12 19:20:55.000000 mypy-boto3-ssm-1.34.61/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:21:13.915058 mypy-boto3-ssm-1.34.61/mypy_boto3_ssm/
--rw-r--r--   0 runner    (1001) docker     (127)    12702 2024-03-12 19:20:55.000000 mypy-boto3-ssm-1.34.61/mypy_boto3_ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12702 2024-03-12 19:20:55.000000 mypy-boto3-ssm-1.34.61/mypy_boto3_ssm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-12 19:20:55.000000 mypy-boto3-ssm-1.34.61/mypy_boto3_ssm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   132524 2024-03-12 19:20:57.000000 mypy-boto3-ssm-1.34.61/mypy_boto3_ssm/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   132521 2024-03-12 19:20:56.000000 mypy-boto3-ssm-1.34.61/mypy_boto3_ssm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    28862 2024-03-12 19:20:58.000000 mypy-boto3-ssm-1.34.61/mypy_boto3_ssm/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    28862 2024-03-12 19:20:58.000000 mypy-boto3-ssm-1.34.61/mypy_boto3_ssm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    59455 2024-03-12 19:20:57.000000 mypy-boto3-ssm-1.34.61/mypy_boto3_ssm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    59407 2024-03-12 19:20:57.000000 mypy-boto3-ssm-1.34.61/mypy_boto3_ssm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 19:20:55.000000 mypy-boto3-ssm-1.34.61/mypy_boto3_ssm/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   192240 2024-03-12 19:21:01.000000 mypy-boto3-ssm-1.34.61/mypy_boto3_ssm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   192240 2024-03-12 19:21:00.000000 mypy-boto3-ssm-1.34.61/mypy_boto3_ssm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-12 19:20:55.000000 mypy-boto3-ssm-1.34.61/mypy_boto3_ssm/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-03-12 19:20:57.000000 mypy-boto3-ssm-1.34.61/mypy_boto3_ssm/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-03-12 19:20:57.000000 mypy-boto3-ssm-1.34.61/mypy_boto3_ssm/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:21:13.915058 mypy-boto3-ssm-1.34.61/mypy_boto3_ssm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21097 2024-03-12 19:21:13.000000 mypy-boto3-ssm-1.34.61/mypy_boto3_ssm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-12 19:21:13.000000 mypy-boto3-ssm-1.34.61/mypy_boto3_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 19:21:13.000000 mypy-boto3-ssm-1.34.61/mypy_boto3_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 19:21:13.000000 mypy-boto3-ssm-1.34.61/mypy_boto3_ssm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-12 19:21:13.000000 mypy-boto3-ssm-1.34.61/mypy_boto3_ssm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-12 19:21:13.000000 mypy-boto3-ssm-1.34.61/mypy_boto3_ssm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 19:21:13.915058 mypy-boto3-ssm-1.34.61/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-03-12 19:20:55.000000 mypy-boto3-ssm-1.34.61/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:06.999879 mypy_boto3_ssm-1.34.91/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-24 19:18:47.000000 mypy_boto3_ssm-1.34.91/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21275 2024-04-24 19:19:06.999879 mypy_boto3_ssm-1.34.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19736 2024-04-24 19:18:47.000000 mypy_boto3_ssm-1.34.91/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:06.995879 mypy_boto3_ssm-1.34.91/mypy_boto3_ssm/
+-rw-r--r--   0 runner    (1001) docker     (127)    12966 2024-04-24 19:18:47.000000 mypy_boto3_ssm-1.34.91/mypy_boto3_ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12966 2024-04-24 19:18:47.000000 mypy_boto3_ssm-1.34.91/mypy_boto3_ssm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-24 19:18:47.000000 mypy_boto3_ssm-1.34.91/mypy_boto3_ssm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   133996 2024-04-24 19:18:48.000000 mypy_boto3_ssm-1.34.91/mypy_boto3_ssm/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   133993 2024-04-24 19:18:47.000000 mypy_boto3_ssm-1.34.91/mypy_boto3_ssm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    29529 2024-04-24 19:18:50.000000 mypy_boto3_ssm-1.34.91/mypy_boto3_ssm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29529 2024-04-24 19:18:49.000000 mypy_boto3_ssm-1.34.91/mypy_boto3_ssm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    60844 2024-04-24 19:18:49.000000 mypy_boto3_ssm-1.34.91/mypy_boto3_ssm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60795 2024-04-24 19:18:49.000000 mypy_boto3_ssm-1.34.91/mypy_boto3_ssm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:18:47.000000 mypy_boto3_ssm-1.34.91/mypy_boto3_ssm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   195405 2024-04-24 19:18:53.000000 mypy_boto3_ssm-1.34.91/mypy_boto3_ssm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   195405 2024-04-24 19:18:52.000000 mypy_boto3_ssm-1.34.91/mypy_boto3_ssm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-24 19:18:47.000000 mypy_boto3_ssm-1.34.91/mypy_boto3_ssm/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-24 19:18:49.000000 mypy_boto3_ssm-1.34.91/mypy_boto3_ssm/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-24 19:18:49.000000 mypy_boto3_ssm-1.34.91/mypy_boto3_ssm/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:06.999879 mypy_boto3_ssm-1.34.91/mypy_boto3_ssm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21275 2024-04-24 19:19:06.000000 mypy_boto3_ssm-1.34.91/mypy_boto3_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-24 19:19:06.000000 mypy_boto3_ssm-1.34.91/mypy_boto3_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:19:06.000000 mypy_boto3_ssm-1.34.91/mypy_boto3_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:19:06.000000 mypy_boto3_ssm-1.34.91/mypy_boto3_ssm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-24 19:19:06.000000 mypy_boto3_ssm-1.34.91/mypy_boto3_ssm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-24 19:19:06.000000 mypy_boto3_ssm-1.34.91/mypy_boto3_ssm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:19:06.999879 mypy_boto3_ssm-1.34.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-24 19:18:47.000000 mypy_boto3_ssm-1.34.91/setup.py
```

### Comparing `mypy-boto3-ssm-1.34.61/LICENSE` & `mypy_boto3_ssm-1.34.91/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.34.61/PKG-INFO` & `mypy_boto3_ssm-1.34.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm
-Version: 1.34.61
-Summary: Type annotations for boto3.SSM 1.34.61 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.91
+Summary: Type annotations for boto3.SSM 1.34.91 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm)](https://pepy.tech/project/mypy-boto3-ssm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSM 1.34.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
+[boto3.SSM 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -293,14 +293,15 @@
     DescribeEffectiveInstanceAssociationsPaginator,
     DescribeEffectivePatchesForPatchBaselinePaginator,
     DescribeInstanceAssociationsStatusPaginator,
     DescribeInstanceInformationPaginator,
     DescribeInstancePatchStatesPaginator,
     DescribeInstancePatchStatesForPatchGroupPaginator,
     DescribeInstancePatchesPaginator,
+    DescribeInstancePropertiesPaginator,
     DescribeInventoryDeletionsPaginator,
     DescribeMaintenanceWindowExecutionTaskInvocationsPaginator,
     DescribeMaintenanceWindowExecutionTasksPaginator,
     DescribeMaintenanceWindowExecutionsPaginator,
     DescribeMaintenanceWindowSchedulePaginator,
     DescribeMaintenanceWindowTargetsPaginator,
     DescribeMaintenanceWindowTasksPaginator,
@@ -372,14 +373,17 @@
 )
 describe_instance_patch_states_for_patch_group_paginator: (
     DescribeInstancePatchStatesForPatchGroupPaginator
 ) = client.get_paginator("describe_instance_patch_states_for_patch_group")
 describe_instance_patches_paginator: DescribeInstancePatchesPaginator = client.get_paginator(
     "describe_instance_patches"
 )
+describe_instance_properties_paginator: DescribeInstancePropertiesPaginator = client.get_paginator(
+    "describe_instance_properties"
+)
 describe_inventory_deletions_paginator: DescribeInventoryDeletionsPaginator = client.get_paginator(
     "describe_inventory_deletions"
 )
 describe_maintenance_window_execution_task_invocations_paginator: (
     DescribeMaintenanceWindowExecutionTaskInvocationsPaginator
 ) = client.get_paginator("describe_maintenance_window_execution_task_invocations")
 describe_maintenance_window_execution_tasks_paginator: (
```

### Comparing `mypy-boto3-ssm-1.34.61/README.md` & `mypy_boto3_ssm-1.34.91/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm)](https://pepy.tech/project/mypy-boto3-ssm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSM 1.34.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
+[boto3.SSM 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -260,14 +260,15 @@
     DescribeEffectiveInstanceAssociationsPaginator,
     DescribeEffectivePatchesForPatchBaselinePaginator,
     DescribeInstanceAssociationsStatusPaginator,
     DescribeInstanceInformationPaginator,
     DescribeInstancePatchStatesPaginator,
     DescribeInstancePatchStatesForPatchGroupPaginator,
     DescribeInstancePatchesPaginator,
+    DescribeInstancePropertiesPaginator,
     DescribeInventoryDeletionsPaginator,
     DescribeMaintenanceWindowExecutionTaskInvocationsPaginator,
     DescribeMaintenanceWindowExecutionTasksPaginator,
     DescribeMaintenanceWindowExecutionsPaginator,
     DescribeMaintenanceWindowSchedulePaginator,
     DescribeMaintenanceWindowTargetsPaginator,
     DescribeMaintenanceWindowTasksPaginator,
@@ -339,14 +340,17 @@
 )
 describe_instance_patch_states_for_patch_group_paginator: (
     DescribeInstancePatchStatesForPatchGroupPaginator
 ) = client.get_paginator("describe_instance_patch_states_for_patch_group")
 describe_instance_patches_paginator: DescribeInstancePatchesPaginator = client.get_paginator(
     "describe_instance_patches"
 )
+describe_instance_properties_paginator: DescribeInstancePropertiesPaginator = client.get_paginator(
+    "describe_instance_properties"
+)
 describe_inventory_deletions_paginator: DescribeInventoryDeletionsPaginator = client.get_paginator(
     "describe_inventory_deletions"
 )
 describe_maintenance_window_execution_task_invocations_paginator: (
     DescribeMaintenanceWindowExecutionTaskInvocationsPaginator
 ) = client.get_paginator("describe_maintenance_window_execution_task_invocations")
 describe_maintenance_window_execution_tasks_paginator: (
```

### Comparing `mypy-boto3-ssm-1.34.61/mypy_boto3_ssm/__init__.py` & `mypy_boto3_ssm-1.34.91/mypy_boto3_ssm/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         DescribeEffectiveInstanceAssociationsPaginator,
         DescribeEffectivePatchesForPatchBaselinePaginator,
         DescribeInstanceAssociationsStatusPaginator,
         DescribeInstanceInformationPaginator,
         DescribeInstancePatchStatesForPatchGroupPaginator,
         DescribeInstancePatchStatesPaginator,
         DescribeInstancePatchesPaginator,
+        DescribeInstancePropertiesPaginator,
         DescribeInventoryDeletionsPaginator,
         DescribeMaintenanceWindowExecutionTaskInvocationsPaginator,
         DescribeMaintenanceWindowExecutionTasksPaginator,
         DescribeMaintenanceWindowExecutionsPaginator,
         DescribeMaintenanceWindowSchedulePaginator,
         DescribeMaintenanceWindowTargetsPaginator,
         DescribeMaintenanceWindowTasksPaginator,
@@ -72,14 +73,15 @@
     describe_effective_instance_associations_paginator: DescribeEffectiveInstanceAssociationsPaginator = client.get_paginator("describe_effective_instance_associations")
     describe_effective_patches_for_patch_baseline_paginator: DescribeEffectivePatchesForPatchBaselinePaginator = client.get_paginator("describe_effective_patches_for_patch_baseline")
     describe_instance_associations_status_paginator: DescribeInstanceAssociationsStatusPaginator = client.get_paginator("describe_instance_associations_status")
     describe_instance_information_paginator: DescribeInstanceInformationPaginator = client.get_paginator("describe_instance_information")
     describe_instance_patch_states_paginator: DescribeInstancePatchStatesPaginator = client.get_paginator("describe_instance_patch_states")
     describe_instance_patch_states_for_patch_group_paginator: DescribeInstancePatchStatesForPatchGroupPaginator = client.get_paginator("describe_instance_patch_states_for_patch_group")
     describe_instance_patches_paginator: DescribeInstancePatchesPaginator = client.get_paginator("describe_instance_patches")
+    describe_instance_properties_paginator: DescribeInstancePropertiesPaginator = client.get_paginator("describe_instance_properties")
     describe_inventory_deletions_paginator: DescribeInventoryDeletionsPaginator = client.get_paginator("describe_inventory_deletions")
     describe_maintenance_window_execution_task_invocations_paginator: DescribeMaintenanceWindowExecutionTaskInvocationsPaginator = client.get_paginator("describe_maintenance_window_execution_task_invocations")
     describe_maintenance_window_execution_tasks_paginator: DescribeMaintenanceWindowExecutionTasksPaginator = client.get_paginator("describe_maintenance_window_execution_tasks")
     describe_maintenance_window_executions_paginator: DescribeMaintenanceWindowExecutionsPaginator = client.get_paginator("describe_maintenance_window_executions")
     describe_maintenance_window_schedule_paginator: DescribeMaintenanceWindowSchedulePaginator = client.get_paginator("describe_maintenance_window_schedule")
     describe_maintenance_window_targets_paginator: DescribeMaintenanceWindowTargetsPaginator = client.get_paginator("describe_maintenance_window_targets")
     describe_maintenance_window_tasks_paginator: DescribeMaintenanceWindowTasksPaginator = client.get_paginator("describe_maintenance_window_tasks")
@@ -124,14 +126,15 @@
     DescribeEffectiveInstanceAssociationsPaginator,
     DescribeEffectivePatchesForPatchBaselinePaginator,
     DescribeInstanceAssociationsStatusPaginator,
     DescribeInstanceInformationPaginator,
     DescribeInstancePatchesPaginator,
     DescribeInstancePatchStatesForPatchGroupPaginator,
     DescribeInstancePatchStatesPaginator,
+    DescribeInstancePropertiesPaginator,
     DescribeInventoryDeletionsPaginator,
     DescribeMaintenanceWindowExecutionsPaginator,
     DescribeMaintenanceWindowExecutionTaskInvocationsPaginator,
     DescribeMaintenanceWindowExecutionTasksPaginator,
     DescribeMaintenanceWindowSchedulePaginator,
     DescribeMaintenanceWindowsForTargetPaginator,
     DescribeMaintenanceWindowsPaginator,
@@ -179,14 +182,15 @@
     "DescribeEffectiveInstanceAssociationsPaginator",
     "DescribeEffectivePatchesForPatchBaselinePaginator",
     "DescribeInstanceAssociationsStatusPaginator",
     "DescribeInstanceInformationPaginator",
     "DescribeInstancePatchStatesForPatchGroupPaginator",
     "DescribeInstancePatchStatesPaginator",
     "DescribeInstancePatchesPaginator",
+    "DescribeInstancePropertiesPaginator",
     "DescribeInventoryDeletionsPaginator",
     "DescribeMaintenanceWindowExecutionTaskInvocationsPaginator",
     "DescribeMaintenanceWindowExecutionTasksPaginator",
     "DescribeMaintenanceWindowExecutionsPaginator",
     "DescribeMaintenanceWindowSchedulePaginator",
     "DescribeMaintenanceWindowTargetsPaginator",
     "DescribeMaintenanceWindowTasksPaginator",
```

### Comparing `mypy-boto3-ssm-1.34.61/mypy_boto3_ssm/__init__.pyi` & `mypy_boto3_ssm-1.34.91/mypy_boto3_ssm/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         DescribeEffectiveInstanceAssociationsPaginator,
         DescribeEffectivePatchesForPatchBaselinePaginator,
         DescribeInstanceAssociationsStatusPaginator,
         DescribeInstanceInformationPaginator,
         DescribeInstancePatchStatesForPatchGroupPaginator,
         DescribeInstancePatchStatesPaginator,
         DescribeInstancePatchesPaginator,
+        DescribeInstancePropertiesPaginator,
         DescribeInventoryDeletionsPaginator,
         DescribeMaintenanceWindowExecutionTaskInvocationsPaginator,
         DescribeMaintenanceWindowExecutionTasksPaginator,
         DescribeMaintenanceWindowExecutionsPaginator,
         DescribeMaintenanceWindowSchedulePaginator,
         DescribeMaintenanceWindowTargetsPaginator,
         DescribeMaintenanceWindowTasksPaginator,
@@ -72,14 +73,15 @@
     describe_effective_instance_associations_paginator: DescribeEffectiveInstanceAssociationsPaginator = client.get_paginator("describe_effective_instance_associations")
     describe_effective_patches_for_patch_baseline_paginator: DescribeEffectivePatchesForPatchBaselinePaginator = client.get_paginator("describe_effective_patches_for_patch_baseline")
     describe_instance_associations_status_paginator: DescribeInstanceAssociationsStatusPaginator = client.get_paginator("describe_instance_associations_status")
     describe_instance_information_paginator: DescribeInstanceInformationPaginator = client.get_paginator("describe_instance_information")
     describe_instance_patch_states_paginator: DescribeInstancePatchStatesPaginator = client.get_paginator("describe_instance_patch_states")
     describe_instance_patch_states_for_patch_group_paginator: DescribeInstancePatchStatesForPatchGroupPaginator = client.get_paginator("describe_instance_patch_states_for_patch_group")
     describe_instance_patches_paginator: DescribeInstancePatchesPaginator = client.get_paginator("describe_instance_patches")
+    describe_instance_properties_paginator: DescribeInstancePropertiesPaginator = client.get_paginator("describe_instance_properties")
     describe_inventory_deletions_paginator: DescribeInventoryDeletionsPaginator = client.get_paginator("describe_inventory_deletions")
     describe_maintenance_window_execution_task_invocations_paginator: DescribeMaintenanceWindowExecutionTaskInvocationsPaginator = client.get_paginator("describe_maintenance_window_execution_task_invocations")
     describe_maintenance_window_execution_tasks_paginator: DescribeMaintenanceWindowExecutionTasksPaginator = client.get_paginator("describe_maintenance_window_execution_tasks")
     describe_maintenance_window_executions_paginator: DescribeMaintenanceWindowExecutionsPaginator = client.get_paginator("describe_maintenance_window_executions")
     describe_maintenance_window_schedule_paginator: DescribeMaintenanceWindowSchedulePaginator = client.get_paginator("describe_maintenance_window_schedule")
     describe_maintenance_window_targets_paginator: DescribeMaintenanceWindowTargetsPaginator = client.get_paginator("describe_maintenance_window_targets")
     describe_maintenance_window_tasks_paginator: DescribeMaintenanceWindowTasksPaginator = client.get_paginator("describe_maintenance_window_tasks")
@@ -124,14 +126,15 @@
     DescribeEffectiveInstanceAssociationsPaginator,
     DescribeEffectivePatchesForPatchBaselinePaginator,
     DescribeInstanceAssociationsStatusPaginator,
     DescribeInstanceInformationPaginator,
     DescribeInstancePatchesPaginator,
     DescribeInstancePatchStatesForPatchGroupPaginator,
     DescribeInstancePatchStatesPaginator,
+    DescribeInstancePropertiesPaginator,
     DescribeInventoryDeletionsPaginator,
     DescribeMaintenanceWindowExecutionsPaginator,
     DescribeMaintenanceWindowExecutionTaskInvocationsPaginator,
     DescribeMaintenanceWindowExecutionTasksPaginator,
     DescribeMaintenanceWindowSchedulePaginator,
     DescribeMaintenanceWindowsForTargetPaginator,
     DescribeMaintenanceWindowsPaginator,
@@ -179,14 +182,15 @@
     "DescribeEffectiveInstanceAssociationsPaginator",
     "DescribeEffectivePatchesForPatchBaselinePaginator",
     "DescribeInstanceAssociationsStatusPaginator",
     "DescribeInstanceInformationPaginator",
     "DescribeInstancePatchStatesForPatchGroupPaginator",
     "DescribeInstancePatchStatesPaginator",
     "DescribeInstancePatchesPaginator",
+    "DescribeInstancePropertiesPaginator",
     "DescribeInventoryDeletionsPaginator",
     "DescribeMaintenanceWindowExecutionTaskInvocationsPaginator",
     "DescribeMaintenanceWindowExecutionTasksPaginator",
     "DescribeMaintenanceWindowExecutionsPaginator",
     "DescribeMaintenanceWindowSchedulePaginator",
     "DescribeMaintenanceWindowTargetsPaginator",
     "DescribeMaintenanceWindowTasksPaginator",
```

### Comparing `mypy-boto3-ssm-1.34.61/mypy_boto3_ssm/__main__.py` & `mypy_boto3_ssm-1.34.91/mypy_boto3_ssm/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SSM 1.34.61\n"
-        "Version:         1.34.61\n"
+        "Type annotations for boto3.SSM 1.34.91\n"
+        "Version:         1.34.91\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.61")
+    print("1.34.91")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ssm-1.34.61/mypy_boto3_ssm/client.py` & `mypy_boto3_ssm-1.34.91/mypy_boto3_ssm/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     DescribeEffectiveInstanceAssociationsPaginator,
     DescribeEffectivePatchesForPatchBaselinePaginator,
     DescribeInstanceAssociationsStatusPaginator,
     DescribeInstanceInformationPaginator,
     DescribeInstancePatchesPaginator,
     DescribeInstancePatchStatesForPatchGroupPaginator,
     DescribeInstancePatchStatesPaginator,
+    DescribeInstancePropertiesPaginator,
     DescribeInventoryDeletionsPaginator,
     DescribeMaintenanceWindowExecutionsPaginator,
     DescribeMaintenanceWindowExecutionTaskInvocationsPaginator,
     DescribeMaintenanceWindowExecutionTasksPaginator,
     DescribeMaintenanceWindowSchedulePaginator,
     DescribeMaintenanceWindowsForTargetPaginator,
     DescribeMaintenanceWindowsPaginator,
@@ -138,14 +139,15 @@
     DescribeEffectiveInstanceAssociationsResultTypeDef,
     DescribeEffectivePatchesForPatchBaselineResultTypeDef,
     DescribeInstanceAssociationsStatusResultTypeDef,
     DescribeInstanceInformationResultTypeDef,
     DescribeInstancePatchesResultTypeDef,
     DescribeInstancePatchStatesForPatchGroupResultTypeDef,
     DescribeInstancePatchStatesResultTypeDef,
+    DescribeInstancePropertiesResultTypeDef,
     DescribeInventoryDeletionsResultTypeDef,
     DescribeMaintenanceWindowExecutionsResultTypeDef,
     DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef,
     DescribeMaintenanceWindowExecutionTasksResultTypeDef,
     DescribeMaintenanceWindowScheduleResultTypeDef,
     DescribeMaintenanceWindowsForTargetResultTypeDef,
     DescribeMaintenanceWindowsResultTypeDef,
@@ -187,14 +189,16 @@
     GetPatchBaselineResultTypeDef,
     GetResourcePoliciesResponseTypeDef,
     GetServiceSettingResultTypeDef,
     InstanceAssociationOutputLocationTypeDef,
     InstanceInformationFilterTypeDef,
     InstanceInformationStringFilterTypeDef,
     InstancePatchStateFilterTypeDef,
+    InstancePropertyFilterTypeDef,
+    InstancePropertyStringFilterTypeDef,
     InventoryAggregatorTypeDef,
     InventoryFilterTypeDef,
     InventoryItemTypeDef,
     LabelParameterVersionResultTypeDef,
     ListAssociationsResultTypeDef,
     ListAssociationVersionsResultTypeDef,
     ListCommandInvocationsResultTypeDef,
@@ -338,14 +342,15 @@
     InvalidDocumentVersion: Type[BotocoreClientError]
     InvalidFilter: Type[BotocoreClientError]
     InvalidFilterKey: Type[BotocoreClientError]
     InvalidFilterOption: Type[BotocoreClientError]
     InvalidFilterValue: Type[BotocoreClientError]
     InvalidInstanceId: Type[BotocoreClientError]
     InvalidInstanceInformationFilterValue: Type[BotocoreClientError]
+    InvalidInstancePropertyFilterValue: Type[BotocoreClientError]
     InvalidInventoryGroupException: Type[BotocoreClientError]
     InvalidInventoryItemContextException: Type[BotocoreClientError]
     InvalidInventoryRequestException: Type[BotocoreClientError]
     InvalidItemContentException: Type[BotocoreClientError]
     InvalidKeyId: Type[BotocoreClientError]
     InvalidNextToken: Type[BotocoreClientError]
     InvalidNotificationConfig: Type[BotocoreClientError]
@@ -1073,14 +1078,31 @@
         state relative to the patch baseline being used for the
         node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_patches)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#describe_instance_patches)
         """
 
+    def describe_instance_properties(
+        self,
+        *,
+        InstancePropertyFilterList: Sequence[InstancePropertyFilterTypeDef] = ...,
+        FiltersWithOperator: Sequence[InstancePropertyStringFilterTypeDef] = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...,
+    ) -> DescribeInstancePropertiesResultTypeDef:
+        """
+        An API operation used by the Systems Manager console to display information
+        about Systems Manager managed
+        nodes.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_properties)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#describe_instance_properties)
+        """
+
     def describe_inventory_deletions(
         self, *, DeletionId: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> DescribeInventoryDeletionsResultTypeDef:
         """
         Describes a specific delete inventory operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_inventory_deletions)
@@ -2550,14 +2572,23 @@
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["describe_instance_properties"]
+    ) -> DescribeInstancePropertiesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["describe_inventory_deletions"]
     ) -> DescribeInventoryDeletionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-ssm-1.34.61/mypy_boto3_ssm/client.pyi` & `mypy_boto3_ssm-1.34.91/mypy_boto3_ssm/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     DescribeEffectiveInstanceAssociationsPaginator,
     DescribeEffectivePatchesForPatchBaselinePaginator,
     DescribeInstanceAssociationsStatusPaginator,
     DescribeInstanceInformationPaginator,
     DescribeInstancePatchesPaginator,
     DescribeInstancePatchStatesForPatchGroupPaginator,
     DescribeInstancePatchStatesPaginator,
+    DescribeInstancePropertiesPaginator,
     DescribeInventoryDeletionsPaginator,
     DescribeMaintenanceWindowExecutionsPaginator,
     DescribeMaintenanceWindowExecutionTaskInvocationsPaginator,
     DescribeMaintenanceWindowExecutionTasksPaginator,
     DescribeMaintenanceWindowSchedulePaginator,
     DescribeMaintenanceWindowsForTargetPaginator,
     DescribeMaintenanceWindowsPaginator,
@@ -138,14 +139,15 @@
     DescribeEffectiveInstanceAssociationsResultTypeDef,
     DescribeEffectivePatchesForPatchBaselineResultTypeDef,
     DescribeInstanceAssociationsStatusResultTypeDef,
     DescribeInstanceInformationResultTypeDef,
     DescribeInstancePatchesResultTypeDef,
     DescribeInstancePatchStatesForPatchGroupResultTypeDef,
     DescribeInstancePatchStatesResultTypeDef,
+    DescribeInstancePropertiesResultTypeDef,
     DescribeInventoryDeletionsResultTypeDef,
     DescribeMaintenanceWindowExecutionsResultTypeDef,
     DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef,
     DescribeMaintenanceWindowExecutionTasksResultTypeDef,
     DescribeMaintenanceWindowScheduleResultTypeDef,
     DescribeMaintenanceWindowsForTargetResultTypeDef,
     DescribeMaintenanceWindowsResultTypeDef,
@@ -187,14 +189,16 @@
     GetPatchBaselineResultTypeDef,
     GetResourcePoliciesResponseTypeDef,
     GetServiceSettingResultTypeDef,
     InstanceAssociationOutputLocationTypeDef,
     InstanceInformationFilterTypeDef,
     InstanceInformationStringFilterTypeDef,
     InstancePatchStateFilterTypeDef,
+    InstancePropertyFilterTypeDef,
+    InstancePropertyStringFilterTypeDef,
     InventoryAggregatorTypeDef,
     InventoryFilterTypeDef,
     InventoryItemTypeDef,
     LabelParameterVersionResultTypeDef,
     ListAssociationsResultTypeDef,
     ListAssociationVersionsResultTypeDef,
     ListCommandInvocationsResultTypeDef,
@@ -336,14 +340,15 @@
     InvalidDocumentVersion: Type[BotocoreClientError]
     InvalidFilter: Type[BotocoreClientError]
     InvalidFilterKey: Type[BotocoreClientError]
     InvalidFilterOption: Type[BotocoreClientError]
     InvalidFilterValue: Type[BotocoreClientError]
     InvalidInstanceId: Type[BotocoreClientError]
     InvalidInstanceInformationFilterValue: Type[BotocoreClientError]
+    InvalidInstancePropertyFilterValue: Type[BotocoreClientError]
     InvalidInventoryGroupException: Type[BotocoreClientError]
     InvalidInventoryItemContextException: Type[BotocoreClientError]
     InvalidInventoryRequestException: Type[BotocoreClientError]
     InvalidItemContentException: Type[BotocoreClientError]
     InvalidKeyId: Type[BotocoreClientError]
     InvalidNextToken: Type[BotocoreClientError]
     InvalidNotificationConfig: Type[BotocoreClientError]
@@ -1070,14 +1075,31 @@
         state relative to the patch baseline being used for the
         node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_patches)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#describe_instance_patches)
         """
 
+    def describe_instance_properties(
+        self,
+        *,
+        InstancePropertyFilterList: Sequence[InstancePropertyFilterTypeDef] = ...,
+        FiltersWithOperator: Sequence[InstancePropertyStringFilterTypeDef] = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...,
+    ) -> DescribeInstancePropertiesResultTypeDef:
+        """
+        An API operation used by the Systems Manager console to display information
+        about Systems Manager managed
+        nodes.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_instance_properties)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#describe_instance_properties)
+        """
+
     def describe_inventory_deletions(
         self, *, DeletionId: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> DescribeInventoryDeletionsResultTypeDef:
         """
         Describes a specific delete inventory operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.describe_inventory_deletions)
@@ -2547,14 +2569,23 @@
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["describe_instance_properties"]
+    ) -> DescribeInstancePropertiesPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["describe_inventory_deletions"]
     ) -> DescribeInventoryDeletionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-ssm-1.34.61/mypy_boto3_ssm/literals.py` & `mypy_boto3_ssm-1.34.91/mypy_boto3_ssm/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     "DescribeEffectiveInstanceAssociationsPaginatorName",
     "DescribeEffectivePatchesForPatchBaselinePaginatorName",
     "DescribeInstanceAssociationsStatusPaginatorName",
     "DescribeInstanceInformationPaginatorName",
     "DescribeInstancePatchStatesForPatchGroupPaginatorName",
     "DescribeInstancePatchStatesPaginatorName",
     "DescribeInstancePatchesPaginatorName",
+    "DescribeInstancePropertiesPaginatorName",
     "DescribeInventoryDeletionsPaginatorName",
     "DescribeMaintenanceWindowExecutionTaskInvocationsPaginatorName",
     "DescribeMaintenanceWindowExecutionTasksPaginatorName",
     "DescribeMaintenanceWindowExecutionsPaginatorName",
     "DescribeMaintenanceWindowSchedulePaginatorName",
     "DescribeMaintenanceWindowTargetsPaginatorName",
     "DescribeMaintenanceWindowTasksPaginatorName",
@@ -90,14 +91,16 @@
     "GetInventorySchemaPaginatorName",
     "GetOpsSummaryPaginatorName",
     "GetParameterHistoryPaginatorName",
     "GetParametersByPathPaginatorName",
     "GetResourcePoliciesPaginatorName",
     "InstanceInformationFilterKeyType",
     "InstancePatchStateOperatorTypeType",
+    "InstancePropertyFilterKeyType",
+    "InstancePropertyFilterOperatorType",
     "InventoryAttributeDataTypeType",
     "InventoryDeletionStatusType",
     "InventoryQueryOperatorTypeType",
     "InventorySchemaDeleteOptionType",
     "LastResourceDataSyncStatusType",
     "ListAssociationVersionsPaginatorName",
     "ListAssociationsPaginatorName",
@@ -255,14 +258,15 @@
 DescribeInstanceAssociationsStatusPaginatorName = Literal["describe_instance_associations_status"]
 DescribeInstanceInformationPaginatorName = Literal["describe_instance_information"]
 DescribeInstancePatchStatesForPatchGroupPaginatorName = Literal[
     "describe_instance_patch_states_for_patch_group"
 ]
 DescribeInstancePatchStatesPaginatorName = Literal["describe_instance_patch_states"]
 DescribeInstancePatchesPaginatorName = Literal["describe_instance_patches"]
+DescribeInstancePropertiesPaginatorName = Literal["describe_instance_properties"]
 DescribeInventoryDeletionsPaginatorName = Literal["describe_inventory_deletions"]
 DescribeMaintenanceWindowExecutionTaskInvocationsPaginatorName = Literal[
     "describe_maintenance_window_execution_task_invocations"
 ]
 DescribeMaintenanceWindowExecutionTasksPaginatorName = Literal[
     "describe_maintenance_window_execution_tasks"
 ]
@@ -322,14 +326,28 @@
     "IamRole",
     "InstanceIds",
     "PingStatus",
     "PlatformTypes",
     "ResourceType",
 ]
 InstancePatchStateOperatorTypeType = Literal["Equal", "GreaterThan", "LessThan", "NotEqual"]
+InstancePropertyFilterKeyType = Literal[
+    "ActivationIds",
+    "AgentVersion",
+    "AssociationStatus",
+    "DocumentName",
+    "IamRole",
+    "InstanceIds",
+    "PingStatus",
+    "PlatformTypes",
+    "ResourceType",
+]
+InstancePropertyFilterOperatorType = Literal[
+    "BeginWith", "Equal", "GreaterThan", "LessThan", "NotEqual"
+]
 InventoryAttributeDataTypeType = Literal["number", "string"]
 InventoryDeletionStatusType = Literal["Complete", "InProgress"]
 InventoryQueryOperatorTypeType = Literal[
     "BeginWith", "Equal", "Exists", "GreaterThan", "LessThan", "NotEqual"
 ]
 InventorySchemaDeleteOptionType = Literal["DeleteSchema", "DisableSchema"]
 LastResourceDataSyncStatusType = Literal["Failed", "InProgress", "Successful"]
@@ -589,14 +607,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -609,24 +628,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -687,15 +708,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -824,14 +844,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -875,14 +896,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
@@ -925,14 +947,15 @@
     "describe_effective_instance_associations",
     "describe_effective_patches_for_patch_baseline",
     "describe_instance_associations_status",
     "describe_instance_information",
     "describe_instance_patch_states",
     "describe_instance_patch_states_for_patch_group",
     "describe_instance_patches",
+    "describe_instance_properties",
     "describe_inventory_deletions",
     "describe_maintenance_window_execution_task_invocations",
     "describe_maintenance_window_execution_tasks",
     "describe_maintenance_window_executions",
     "describe_maintenance_window_schedule",
     "describe_maintenance_window_targets",
     "describe_maintenance_window_tasks",
```

### Comparing `mypy-boto3-ssm-1.34.61/mypy_boto3_ssm/literals.pyi` & `mypy_boto3_ssm-1.34.91/mypy_boto3_ssm/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     "DescribeEffectiveInstanceAssociationsPaginatorName",
     "DescribeEffectivePatchesForPatchBaselinePaginatorName",
     "DescribeInstanceAssociationsStatusPaginatorName",
     "DescribeInstanceInformationPaginatorName",
     "DescribeInstancePatchStatesForPatchGroupPaginatorName",
     "DescribeInstancePatchStatesPaginatorName",
     "DescribeInstancePatchesPaginatorName",
+    "DescribeInstancePropertiesPaginatorName",
     "DescribeInventoryDeletionsPaginatorName",
     "DescribeMaintenanceWindowExecutionTaskInvocationsPaginatorName",
     "DescribeMaintenanceWindowExecutionTasksPaginatorName",
     "DescribeMaintenanceWindowExecutionsPaginatorName",
     "DescribeMaintenanceWindowSchedulePaginatorName",
     "DescribeMaintenanceWindowTargetsPaginatorName",
     "DescribeMaintenanceWindowTasksPaginatorName",
@@ -90,14 +91,16 @@
     "GetInventorySchemaPaginatorName",
     "GetOpsSummaryPaginatorName",
     "GetParameterHistoryPaginatorName",
     "GetParametersByPathPaginatorName",
     "GetResourcePoliciesPaginatorName",
     "InstanceInformationFilterKeyType",
     "InstancePatchStateOperatorTypeType",
+    "InstancePropertyFilterKeyType",
+    "InstancePropertyFilterOperatorType",
     "InventoryAttributeDataTypeType",
     "InventoryDeletionStatusType",
     "InventoryQueryOperatorTypeType",
     "InventorySchemaDeleteOptionType",
     "LastResourceDataSyncStatusType",
     "ListAssociationVersionsPaginatorName",
     "ListAssociationsPaginatorName",
@@ -255,14 +258,15 @@
 DescribeInstanceAssociationsStatusPaginatorName = Literal["describe_instance_associations_status"]
 DescribeInstanceInformationPaginatorName = Literal["describe_instance_information"]
 DescribeInstancePatchStatesForPatchGroupPaginatorName = Literal[
     "describe_instance_patch_states_for_patch_group"
 ]
 DescribeInstancePatchStatesPaginatorName = Literal["describe_instance_patch_states"]
 DescribeInstancePatchesPaginatorName = Literal["describe_instance_patches"]
+DescribeInstancePropertiesPaginatorName = Literal["describe_instance_properties"]
 DescribeInventoryDeletionsPaginatorName = Literal["describe_inventory_deletions"]
 DescribeMaintenanceWindowExecutionTaskInvocationsPaginatorName = Literal[
     "describe_maintenance_window_execution_task_invocations"
 ]
 DescribeMaintenanceWindowExecutionTasksPaginatorName = Literal[
     "describe_maintenance_window_execution_tasks"
 ]
@@ -322,14 +326,28 @@
     "IamRole",
     "InstanceIds",
     "PingStatus",
     "PlatformTypes",
     "ResourceType",
 ]
 InstancePatchStateOperatorTypeType = Literal["Equal", "GreaterThan", "LessThan", "NotEqual"]
+InstancePropertyFilterKeyType = Literal[
+    "ActivationIds",
+    "AgentVersion",
+    "AssociationStatus",
+    "DocumentName",
+    "IamRole",
+    "InstanceIds",
+    "PingStatus",
+    "PlatformTypes",
+    "ResourceType",
+]
+InstancePropertyFilterOperatorType = Literal[
+    "BeginWith", "Equal", "GreaterThan", "LessThan", "NotEqual"
+]
 InventoryAttributeDataTypeType = Literal["number", "string"]
 InventoryDeletionStatusType = Literal["Complete", "InProgress"]
 InventoryQueryOperatorTypeType = Literal[
     "BeginWith", "Equal", "Exists", "GreaterThan", "LessThan", "NotEqual"
 ]
 InventorySchemaDeleteOptionType = Literal["DeleteSchema", "DisableSchema"]
 LastResourceDataSyncStatusType = Literal["Failed", "InProgress", "Successful"]
@@ -589,14 +607,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -609,24 +628,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -687,15 +708,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -824,14 +844,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -875,14 +896,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
@@ -925,14 +947,15 @@
     "describe_effective_instance_associations",
     "describe_effective_patches_for_patch_baseline",
     "describe_instance_associations_status",
     "describe_instance_information",
     "describe_instance_patch_states",
     "describe_instance_patch_states_for_patch_group",
     "describe_instance_patches",
+    "describe_instance_properties",
     "describe_inventory_deletions",
     "describe_maintenance_window_execution_task_invocations",
     "describe_maintenance_window_execution_tasks",
     "describe_maintenance_window_executions",
     "describe_maintenance_window_schedule",
     "describe_maintenance_window_targets",
     "describe_maintenance_window_tasks",
```

### Comparing `mypy-boto3-ssm-1.34.61/mypy_boto3_ssm/paginator.py` & `mypy_boto3_ssm-1.34.91/mypy_boto3_ssm/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         DescribeEffectiveInstanceAssociationsPaginator,
         DescribeEffectivePatchesForPatchBaselinePaginator,
         DescribeInstanceAssociationsStatusPaginator,
         DescribeInstanceInformationPaginator,
         DescribeInstancePatchStatesPaginator,
         DescribeInstancePatchStatesForPatchGroupPaginator,
         DescribeInstancePatchesPaginator,
+        DescribeInstancePropertiesPaginator,
         DescribeInventoryDeletionsPaginator,
         DescribeMaintenanceWindowExecutionTaskInvocationsPaginator,
         DescribeMaintenanceWindowExecutionTasksPaginator,
         DescribeMaintenanceWindowExecutionsPaginator,
         DescribeMaintenanceWindowSchedulePaginator,
         DescribeMaintenanceWindowTargetsPaginator,
         DescribeMaintenanceWindowTasksPaginator,
@@ -71,14 +72,15 @@
     describe_effective_instance_associations_paginator: DescribeEffectiveInstanceAssociationsPaginator = client.get_paginator("describe_effective_instance_associations")
     describe_effective_patches_for_patch_baseline_paginator: DescribeEffectivePatchesForPatchBaselinePaginator = client.get_paginator("describe_effective_patches_for_patch_baseline")
     describe_instance_associations_status_paginator: DescribeInstanceAssociationsStatusPaginator = client.get_paginator("describe_instance_associations_status")
     describe_instance_information_paginator: DescribeInstanceInformationPaginator = client.get_paginator("describe_instance_information")
     describe_instance_patch_states_paginator: DescribeInstancePatchStatesPaginator = client.get_paginator("describe_instance_patch_states")
     describe_instance_patch_states_for_patch_group_paginator: DescribeInstancePatchStatesForPatchGroupPaginator = client.get_paginator("describe_instance_patch_states_for_patch_group")
     describe_instance_patches_paginator: DescribeInstancePatchesPaginator = client.get_paginator("describe_instance_patches")
+    describe_instance_properties_paginator: DescribeInstancePropertiesPaginator = client.get_paginator("describe_instance_properties")
     describe_inventory_deletions_paginator: DescribeInventoryDeletionsPaginator = client.get_paginator("describe_inventory_deletions")
     describe_maintenance_window_execution_task_invocations_paginator: DescribeMaintenanceWindowExecutionTaskInvocationsPaginator = client.get_paginator("describe_maintenance_window_execution_task_invocations")
     describe_maintenance_window_execution_tasks_paginator: DescribeMaintenanceWindowExecutionTasksPaginator = client.get_paginator("describe_maintenance_window_execution_tasks")
     describe_maintenance_window_executions_paginator: DescribeMaintenanceWindowExecutionsPaginator = client.get_paginator("describe_maintenance_window_executions")
     describe_maintenance_window_schedule_paginator: DescribeMaintenanceWindowSchedulePaginator = client.get_paginator("describe_maintenance_window_schedule")
     describe_maintenance_window_targets_paginator: DescribeMaintenanceWindowTargetsPaginator = client.get_paginator("describe_maintenance_window_targets")
     describe_maintenance_window_tasks_paginator: DescribeMaintenanceWindowTasksPaginator = client.get_paginator("describe_maintenance_window_tasks")
@@ -140,14 +142,15 @@
     DescribeEffectiveInstanceAssociationsResultTypeDef,
     DescribeEffectivePatchesForPatchBaselineResultTypeDef,
     DescribeInstanceAssociationsStatusResultTypeDef,
     DescribeInstanceInformationResultTypeDef,
     DescribeInstancePatchesResultTypeDef,
     DescribeInstancePatchStatesForPatchGroupResultTypeDef,
     DescribeInstancePatchStatesResultTypeDef,
+    DescribeInstancePropertiesResultTypeDef,
     DescribeInventoryDeletionsResultTypeDef,
     DescribeMaintenanceWindowExecutionsResultTypeDef,
     DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef,
     DescribeMaintenanceWindowExecutionTasksResultPaginatorTypeDef,
     DescribeMaintenanceWindowScheduleResultTypeDef,
     DescribeMaintenanceWindowsForTargetResultTypeDef,
     DescribeMaintenanceWindowsResultTypeDef,
@@ -166,14 +169,16 @@
     GetOpsSummaryResultTypeDef,
     GetParameterHistoryResultTypeDef,
     GetParametersByPathResultTypeDef,
     GetResourcePoliciesResponseTypeDef,
     InstanceInformationFilterTypeDef,
     InstanceInformationStringFilterTypeDef,
     InstancePatchStateFilterTypeDef,
+    InstancePropertyFilterTypeDef,
+    InstancePropertyStringFilterTypeDef,
     InventoryAggregatorTypeDef,
     InventoryFilterTypeDef,
     ListAssociationsResultPaginatorTypeDef,
     ListAssociationVersionsResultPaginatorTypeDef,
     ListCommandInvocationsResultTypeDef,
     ListCommandsResultPaginatorTypeDef,
     ListComplianceItemsResultTypeDef,
@@ -213,14 +218,15 @@
     "DescribeEffectiveInstanceAssociationsPaginator",
     "DescribeEffectivePatchesForPatchBaselinePaginator",
     "DescribeInstanceAssociationsStatusPaginator",
     "DescribeInstanceInformationPaginator",
     "DescribeInstancePatchStatesPaginator",
     "DescribeInstancePatchStatesForPatchGroupPaginator",
     "DescribeInstancePatchesPaginator",
+    "DescribeInstancePropertiesPaginator",
     "DescribeInventoryDeletionsPaginator",
     "DescribeMaintenanceWindowExecutionTaskInvocationsPaginator",
     "DescribeMaintenanceWindowExecutionTasksPaginator",
     "DescribeMaintenanceWindowExecutionsPaginator",
     "DescribeMaintenanceWindowSchedulePaginator",
     "DescribeMaintenanceWindowTargetsPaginator",
     "DescribeMaintenanceWindowTasksPaginator",
@@ -489,14 +495,33 @@
     ) -> _PageIterator[DescribeInstancePatchesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstancepatchespaginator)
         """
 
 
+class DescribeInstancePropertiesPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstanceProperties)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstancepropertiespaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        InstancePropertyFilterList: Sequence[InstancePropertyFilterTypeDef] = ...,
+        FiltersWithOperator: Sequence[InstancePropertyStringFilterTypeDef] = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[DescribeInstancePropertiesResultTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstanceProperties.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstancepropertiespaginator)
+        """
+
+
 class DescribeInventoryDeletionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInventoryDeletions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinventorydeletionspaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-ssm-1.34.61/mypy_boto3_ssm/paginator.pyi` & `mypy_boto3_ssm-1.34.91/mypy_boto3_ssm/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         DescribeEffectiveInstanceAssociationsPaginator,
         DescribeEffectivePatchesForPatchBaselinePaginator,
         DescribeInstanceAssociationsStatusPaginator,
         DescribeInstanceInformationPaginator,
         DescribeInstancePatchStatesPaginator,
         DescribeInstancePatchStatesForPatchGroupPaginator,
         DescribeInstancePatchesPaginator,
+        DescribeInstancePropertiesPaginator,
         DescribeInventoryDeletionsPaginator,
         DescribeMaintenanceWindowExecutionTaskInvocationsPaginator,
         DescribeMaintenanceWindowExecutionTasksPaginator,
         DescribeMaintenanceWindowExecutionsPaginator,
         DescribeMaintenanceWindowSchedulePaginator,
         DescribeMaintenanceWindowTargetsPaginator,
         DescribeMaintenanceWindowTasksPaginator,
@@ -71,14 +72,15 @@
     describe_effective_instance_associations_paginator: DescribeEffectiveInstanceAssociationsPaginator = client.get_paginator("describe_effective_instance_associations")
     describe_effective_patches_for_patch_baseline_paginator: DescribeEffectivePatchesForPatchBaselinePaginator = client.get_paginator("describe_effective_patches_for_patch_baseline")
     describe_instance_associations_status_paginator: DescribeInstanceAssociationsStatusPaginator = client.get_paginator("describe_instance_associations_status")
     describe_instance_information_paginator: DescribeInstanceInformationPaginator = client.get_paginator("describe_instance_information")
     describe_instance_patch_states_paginator: DescribeInstancePatchStatesPaginator = client.get_paginator("describe_instance_patch_states")
     describe_instance_patch_states_for_patch_group_paginator: DescribeInstancePatchStatesForPatchGroupPaginator = client.get_paginator("describe_instance_patch_states_for_patch_group")
     describe_instance_patches_paginator: DescribeInstancePatchesPaginator = client.get_paginator("describe_instance_patches")
+    describe_instance_properties_paginator: DescribeInstancePropertiesPaginator = client.get_paginator("describe_instance_properties")
     describe_inventory_deletions_paginator: DescribeInventoryDeletionsPaginator = client.get_paginator("describe_inventory_deletions")
     describe_maintenance_window_execution_task_invocations_paginator: DescribeMaintenanceWindowExecutionTaskInvocationsPaginator = client.get_paginator("describe_maintenance_window_execution_task_invocations")
     describe_maintenance_window_execution_tasks_paginator: DescribeMaintenanceWindowExecutionTasksPaginator = client.get_paginator("describe_maintenance_window_execution_tasks")
     describe_maintenance_window_executions_paginator: DescribeMaintenanceWindowExecutionsPaginator = client.get_paginator("describe_maintenance_window_executions")
     describe_maintenance_window_schedule_paginator: DescribeMaintenanceWindowSchedulePaginator = client.get_paginator("describe_maintenance_window_schedule")
     describe_maintenance_window_targets_paginator: DescribeMaintenanceWindowTargetsPaginator = client.get_paginator("describe_maintenance_window_targets")
     describe_maintenance_window_tasks_paginator: DescribeMaintenanceWindowTasksPaginator = client.get_paginator("describe_maintenance_window_tasks")
@@ -140,14 +142,15 @@
     DescribeEffectiveInstanceAssociationsResultTypeDef,
     DescribeEffectivePatchesForPatchBaselineResultTypeDef,
     DescribeInstanceAssociationsStatusResultTypeDef,
     DescribeInstanceInformationResultTypeDef,
     DescribeInstancePatchesResultTypeDef,
     DescribeInstancePatchStatesForPatchGroupResultTypeDef,
     DescribeInstancePatchStatesResultTypeDef,
+    DescribeInstancePropertiesResultTypeDef,
     DescribeInventoryDeletionsResultTypeDef,
     DescribeMaintenanceWindowExecutionsResultTypeDef,
     DescribeMaintenanceWindowExecutionTaskInvocationsResultTypeDef,
     DescribeMaintenanceWindowExecutionTasksResultPaginatorTypeDef,
     DescribeMaintenanceWindowScheduleResultTypeDef,
     DescribeMaintenanceWindowsForTargetResultTypeDef,
     DescribeMaintenanceWindowsResultTypeDef,
@@ -166,14 +169,16 @@
     GetOpsSummaryResultTypeDef,
     GetParameterHistoryResultTypeDef,
     GetParametersByPathResultTypeDef,
     GetResourcePoliciesResponseTypeDef,
     InstanceInformationFilterTypeDef,
     InstanceInformationStringFilterTypeDef,
     InstancePatchStateFilterTypeDef,
+    InstancePropertyFilterTypeDef,
+    InstancePropertyStringFilterTypeDef,
     InventoryAggregatorTypeDef,
     InventoryFilterTypeDef,
     ListAssociationsResultPaginatorTypeDef,
     ListAssociationVersionsResultPaginatorTypeDef,
     ListCommandInvocationsResultTypeDef,
     ListCommandsResultPaginatorTypeDef,
     ListComplianceItemsResultTypeDef,
@@ -213,14 +218,15 @@
     "DescribeEffectiveInstanceAssociationsPaginator",
     "DescribeEffectivePatchesForPatchBaselinePaginator",
     "DescribeInstanceAssociationsStatusPaginator",
     "DescribeInstanceInformationPaginator",
     "DescribeInstancePatchStatesPaginator",
     "DescribeInstancePatchStatesForPatchGroupPaginator",
     "DescribeInstancePatchesPaginator",
+    "DescribeInstancePropertiesPaginator",
     "DescribeInventoryDeletionsPaginator",
     "DescribeMaintenanceWindowExecutionTaskInvocationsPaginator",
     "DescribeMaintenanceWindowExecutionTasksPaginator",
     "DescribeMaintenanceWindowExecutionsPaginator",
     "DescribeMaintenanceWindowSchedulePaginator",
     "DescribeMaintenanceWindowTargetsPaginator",
     "DescribeMaintenanceWindowTasksPaginator",
@@ -474,14 +480,32 @@
         PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeInstancePatchesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstancePatches.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstancepatchespaginator)
         """
 
+class DescribeInstancePropertiesPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstanceProperties)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstancepropertiespaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        InstancePropertyFilterList: Sequence[InstancePropertyFilterTypeDef] = ...,
+        FiltersWithOperator: Sequence[InstancePropertyStringFilterTypeDef] = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[DescribeInstancePropertiesResultTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInstanceProperties.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinstancepropertiespaginator)
+        """
+
 class DescribeInventoryDeletionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Paginator.DescribeInventoryDeletions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/paginators/#describeinventorydeletionspaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-ssm-1.34.61/mypy_boto3_ssm/type_defs.py` & `mypy_boto3_ssm-1.34.91/mypy_boto3_ssm/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,16 @@
     DocumentStatusType,
     DocumentTypeType,
     ExecutionModeType,
     ExternalAlarmStateType,
     FaultType,
     InstanceInformationFilterKeyType,
     InstancePatchStateOperatorTypeType,
+    InstancePropertyFilterKeyType,
+    InstancePropertyFilterOperatorType,
     InventoryAttributeDataTypeType,
     InventoryDeletionStatusType,
     InventoryQueryOperatorTypeType,
     InventorySchemaDeleteOptionType,
     LastResourceDataSyncStatusType,
     MaintenanceWindowExecutionStatusType,
     MaintenanceWindowResourceTypeType,
@@ -177,14 +179,16 @@
     "DescribeInstanceAssociationsStatusRequestRequestTypeDef",
     "InstanceInformationFilterTypeDef",
     "InstanceInformationStringFilterTypeDef",
     "InstancePatchStateFilterTypeDef",
     "InstancePatchStateTypeDef",
     "DescribeInstancePatchStatesRequestRequestTypeDef",
     "PatchComplianceDataTypeDef",
+    "InstancePropertyFilterTypeDef",
+    "InstancePropertyStringFilterTypeDef",
     "DescribeInventoryDeletionsRequestRequestTypeDef",
     "MaintenanceWindowFilterTypeDef",
     "MaintenanceWindowExecutionTaskInvocationIdentityTypeDef",
     "MaintenanceWindowExecutionTypeDef",
     "ScheduledWindowExecutionTypeDef",
     "MaintenanceWindowIdentityForTargetTypeDef",
     "MaintenanceWindowIdentityTypeDef",
@@ -408,14 +412,16 @@
     "DescribeInstanceInformationRequestDescribeInstanceInformationPaginateTypeDef",
     "DescribeInstanceInformationRequestRequestTypeDef",
     "DescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef",
     "DescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef",
     "DescribeInstancePatchStatesForPatchGroupResultTypeDef",
     "DescribeInstancePatchStatesResultTypeDef",
     "DescribeInstancePatchesResultTypeDef",
+    "DescribeInstancePropertiesRequestDescribeInstancePropertiesPaginateTypeDef",
+    "DescribeInstancePropertiesRequestRequestTypeDef",
     "DescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef",
     "DescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef",
     "DescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef",
     "DescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef",
     "DescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef",
     "DescribeMaintenanceWindowExecutionsRequestRequestTypeDef",
     "DescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef",
@@ -456,14 +462,15 @@
     "GetParameterResultTypeDef",
     "GetParametersByPathResultTypeDef",
     "GetParametersResultTypeDef",
     "GetResourcePoliciesResponseTypeDef",
     "GetServiceSettingResultTypeDef",
     "ResetServiceSettingResultTypeDef",
     "InstanceInformationTypeDef",
+    "InstancePropertyTypeDef",
     "InstanceAssociationOutputLocationTypeDef",
     "InstanceAssociationOutputUrlTypeDef",
     "InventoryDeletionSummaryTypeDef",
     "InventoryItemSchemaTypeDef",
     "PutInventoryRequestRequestTypeDef",
     "InventoryResultEntityTypeDef",
     "ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef",
@@ -515,14 +522,15 @@
     "UpdateDocumentResultTypeDef",
     "DocumentMetadataResponseInfoTypeDef",
     "UpdateDocumentMetadataRequestRequestTypeDef",
     "DescribeEffectivePatchesForPatchBaselineResultTypeDef",
     "InventoryAggregatorTypeDef",
     "GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef",
     "DescribeInstanceInformationResultTypeDef",
+    "DescribeInstancePropertiesResultTypeDef",
     "InstanceAssociationStatusInfoTypeDef",
     "DeleteInventoryResultTypeDef",
     "InventoryDeletionStatusItemTypeDef",
     "GetInventorySchemaResultTypeDef",
     "GetInventoryResultTypeDef",
     "GetOpsSummaryResultTypeDef",
     "ListOpsItemEventsResponseTypeDef",
@@ -1182,14 +1190,29 @@
         "Classification": str,
         "Severity": str,
         "State": PatchComplianceDataStateType,
         "InstalledTime": datetime,
         "CVEIds": NotRequired[str],
     },
 )
+InstancePropertyFilterTypeDef = TypedDict(
+    "InstancePropertyFilterTypeDef",
+    {
+        "key": InstancePropertyFilterKeyType,
+        "valueSet": Sequence[str],
+    },
+)
+InstancePropertyStringFilterTypeDef = TypedDict(
+    "InstancePropertyStringFilterTypeDef",
+    {
+        "Key": str,
+        "Values": Sequence[str],
+        "Operator": NotRequired[InstancePropertyFilterOperatorType],
+    },
+)
 DescribeInventoryDeletionsRequestRequestTypeDef = TypedDict(
     "DescribeInventoryDeletionsRequestRequestTypeDef",
     {
         "DeletionId": NotRequired[str],
         "NextToken": NotRequired[str],
         "MaxResults": NotRequired[int],
     },
@@ -3298,14 +3321,31 @@
     "DescribeInstancePatchesResultTypeDef",
     {
         "Patches": List[PatchComplianceDataTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DescribeInstancePropertiesRequestDescribeInstancePropertiesPaginateTypeDef = TypedDict(
+    "DescribeInstancePropertiesRequestDescribeInstancePropertiesPaginateTypeDef",
+    {
+        "InstancePropertyFilterList": NotRequired[Sequence[InstancePropertyFilterTypeDef]],
+        "FiltersWithOperator": NotRequired[Sequence[InstancePropertyStringFilterTypeDef]],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
+DescribeInstancePropertiesRequestRequestTypeDef = TypedDict(
+    "DescribeInstancePropertiesRequestRequestTypeDef",
+    {
+        "InstancePropertyFilterList": NotRequired[Sequence[InstancePropertyFilterTypeDef]],
+        "FiltersWithOperator": NotRequired[Sequence[InstancePropertyStringFilterTypeDef]],
+        "MaxResults": NotRequired[int],
+        "NextToken": NotRequired[str],
+    },
+)
 DescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef = TypedDict(
     "DescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
         "Filters": NotRequired[Sequence[MaintenanceWindowFilterTypeDef]],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
@@ -3749,14 +3789,45 @@
         "LastAssociationExecutionDate": NotRequired[datetime],
         "LastSuccessfulAssociationExecutionDate": NotRequired[datetime],
         "AssociationOverview": NotRequired[InstanceAggregatedAssociationOverviewTypeDef],
         "SourceId": NotRequired[str],
         "SourceType": NotRequired[SourceTypeType],
     },
 )
+InstancePropertyTypeDef = TypedDict(
+    "InstancePropertyTypeDef",
+    {
+        "Name": NotRequired[str],
+        "InstanceId": NotRequired[str],
+        "InstanceType": NotRequired[str],
+        "InstanceRole": NotRequired[str],
+        "KeyName": NotRequired[str],
+        "InstanceState": NotRequired[str],
+        "Architecture": NotRequired[str],
+        "IPAddress": NotRequired[str],
+        "LaunchTime": NotRequired[datetime],
+        "PingStatus": NotRequired[PingStatusType],
+        "LastPingDateTime": NotRequired[datetime],
+        "AgentVersion": NotRequired[str],
+        "PlatformType": NotRequired[PlatformTypeType],
+        "PlatformName": NotRequired[str],
+        "PlatformVersion": NotRequired[str],
+        "ActivationId": NotRequired[str],
+        "IamRole": NotRequired[str],
+        "RegistrationDate": NotRequired[datetime],
+        "ResourceType": NotRequired[str],
+        "ComputerName": NotRequired[str],
+        "AssociationStatus": NotRequired[str],
+        "LastAssociationExecutionDate": NotRequired[datetime],
+        "LastSuccessfulAssociationExecutionDate": NotRequired[datetime],
+        "AssociationOverview": NotRequired[InstanceAggregatedAssociationOverviewTypeDef],
+        "SourceId": NotRequired[str],
+        "SourceType": NotRequired[SourceTypeType],
+    },
+)
 InstanceAssociationOutputLocationTypeDef = TypedDict(
     "InstanceAssociationOutputLocationTypeDef",
     {
         "S3Location": NotRequired[S3OutputLocationTypeDef],
     },
 )
 InstanceAssociationOutputUrlTypeDef = TypedDict(
@@ -4388,14 +4459,22 @@
     "DescribeInstanceInformationResultTypeDef",
     {
         "InstanceInformationList": List[InstanceInformationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DescribeInstancePropertiesResultTypeDef = TypedDict(
+    "DescribeInstancePropertiesResultTypeDef",
+    {
+        "InstanceProperties": List[InstancePropertyTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 InstanceAssociationStatusInfoTypeDef = TypedDict(
     "InstanceAssociationStatusInfoTypeDef",
     {
         "AssociationId": NotRequired[str],
         "Name": NotRequired[str],
         "DocumentVersion": NotRequired[str],
         "AssociationVersion": NotRequired[str],
```

### Comparing `mypy-boto3-ssm-1.34.61/mypy_boto3_ssm/type_defs.pyi` & `mypy_boto3_ssm-1.34.91/mypy_boto3_ssm/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,16 @@
     DocumentStatusType,
     DocumentTypeType,
     ExecutionModeType,
     ExternalAlarmStateType,
     FaultType,
     InstanceInformationFilterKeyType,
     InstancePatchStateOperatorTypeType,
+    InstancePropertyFilterKeyType,
+    InstancePropertyFilterOperatorType,
     InventoryAttributeDataTypeType,
     InventoryDeletionStatusType,
     InventoryQueryOperatorTypeType,
     InventorySchemaDeleteOptionType,
     LastResourceDataSyncStatusType,
     MaintenanceWindowExecutionStatusType,
     MaintenanceWindowResourceTypeType,
@@ -177,14 +179,16 @@
     "DescribeInstanceAssociationsStatusRequestRequestTypeDef",
     "InstanceInformationFilterTypeDef",
     "InstanceInformationStringFilterTypeDef",
     "InstancePatchStateFilterTypeDef",
     "InstancePatchStateTypeDef",
     "DescribeInstancePatchStatesRequestRequestTypeDef",
     "PatchComplianceDataTypeDef",
+    "InstancePropertyFilterTypeDef",
+    "InstancePropertyStringFilterTypeDef",
     "DescribeInventoryDeletionsRequestRequestTypeDef",
     "MaintenanceWindowFilterTypeDef",
     "MaintenanceWindowExecutionTaskInvocationIdentityTypeDef",
     "MaintenanceWindowExecutionTypeDef",
     "ScheduledWindowExecutionTypeDef",
     "MaintenanceWindowIdentityForTargetTypeDef",
     "MaintenanceWindowIdentityTypeDef",
@@ -408,14 +412,16 @@
     "DescribeInstanceInformationRequestDescribeInstanceInformationPaginateTypeDef",
     "DescribeInstanceInformationRequestRequestTypeDef",
     "DescribeInstancePatchStatesForPatchGroupRequestDescribeInstancePatchStatesForPatchGroupPaginateTypeDef",
     "DescribeInstancePatchStatesForPatchGroupRequestRequestTypeDef",
     "DescribeInstancePatchStatesForPatchGroupResultTypeDef",
     "DescribeInstancePatchStatesResultTypeDef",
     "DescribeInstancePatchesResultTypeDef",
+    "DescribeInstancePropertiesRequestDescribeInstancePropertiesPaginateTypeDef",
+    "DescribeInstancePropertiesRequestRequestTypeDef",
     "DescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef",
     "DescribeMaintenanceWindowExecutionTaskInvocationsRequestRequestTypeDef",
     "DescribeMaintenanceWindowExecutionTasksRequestDescribeMaintenanceWindowExecutionTasksPaginateTypeDef",
     "DescribeMaintenanceWindowExecutionTasksRequestRequestTypeDef",
     "DescribeMaintenanceWindowExecutionsRequestDescribeMaintenanceWindowExecutionsPaginateTypeDef",
     "DescribeMaintenanceWindowExecutionsRequestRequestTypeDef",
     "DescribeMaintenanceWindowTargetsRequestDescribeMaintenanceWindowTargetsPaginateTypeDef",
@@ -456,14 +462,15 @@
     "GetParameterResultTypeDef",
     "GetParametersByPathResultTypeDef",
     "GetParametersResultTypeDef",
     "GetResourcePoliciesResponseTypeDef",
     "GetServiceSettingResultTypeDef",
     "ResetServiceSettingResultTypeDef",
     "InstanceInformationTypeDef",
+    "InstancePropertyTypeDef",
     "InstanceAssociationOutputLocationTypeDef",
     "InstanceAssociationOutputUrlTypeDef",
     "InventoryDeletionSummaryTypeDef",
     "InventoryItemSchemaTypeDef",
     "PutInventoryRequestRequestTypeDef",
     "InventoryResultEntityTypeDef",
     "ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef",
@@ -515,14 +522,15 @@
     "UpdateDocumentResultTypeDef",
     "DocumentMetadataResponseInfoTypeDef",
     "UpdateDocumentMetadataRequestRequestTypeDef",
     "DescribeEffectivePatchesForPatchBaselineResultTypeDef",
     "InventoryAggregatorTypeDef",
     "GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef",
     "DescribeInstanceInformationResultTypeDef",
+    "DescribeInstancePropertiesResultTypeDef",
     "InstanceAssociationStatusInfoTypeDef",
     "DeleteInventoryResultTypeDef",
     "InventoryDeletionStatusItemTypeDef",
     "GetInventorySchemaResultTypeDef",
     "GetInventoryResultTypeDef",
     "GetOpsSummaryResultTypeDef",
     "ListOpsItemEventsResponseTypeDef",
@@ -1182,14 +1190,29 @@
         "Classification": str,
         "Severity": str,
         "State": PatchComplianceDataStateType,
         "InstalledTime": datetime,
         "CVEIds": NotRequired[str],
     },
 )
+InstancePropertyFilterTypeDef = TypedDict(
+    "InstancePropertyFilterTypeDef",
+    {
+        "key": InstancePropertyFilterKeyType,
+        "valueSet": Sequence[str],
+    },
+)
+InstancePropertyStringFilterTypeDef = TypedDict(
+    "InstancePropertyStringFilterTypeDef",
+    {
+        "Key": str,
+        "Values": Sequence[str],
+        "Operator": NotRequired[InstancePropertyFilterOperatorType],
+    },
+)
 DescribeInventoryDeletionsRequestRequestTypeDef = TypedDict(
     "DescribeInventoryDeletionsRequestRequestTypeDef",
     {
         "DeletionId": NotRequired[str],
         "NextToken": NotRequired[str],
         "MaxResults": NotRequired[int],
     },
@@ -3298,14 +3321,31 @@
     "DescribeInstancePatchesResultTypeDef",
     {
         "Patches": List[PatchComplianceDataTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DescribeInstancePropertiesRequestDescribeInstancePropertiesPaginateTypeDef = TypedDict(
+    "DescribeInstancePropertiesRequestDescribeInstancePropertiesPaginateTypeDef",
+    {
+        "InstancePropertyFilterList": NotRequired[Sequence[InstancePropertyFilterTypeDef]],
+        "FiltersWithOperator": NotRequired[Sequence[InstancePropertyStringFilterTypeDef]],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
+DescribeInstancePropertiesRequestRequestTypeDef = TypedDict(
+    "DescribeInstancePropertiesRequestRequestTypeDef",
+    {
+        "InstancePropertyFilterList": NotRequired[Sequence[InstancePropertyFilterTypeDef]],
+        "FiltersWithOperator": NotRequired[Sequence[InstancePropertyStringFilterTypeDef]],
+        "MaxResults": NotRequired[int],
+        "NextToken": NotRequired[str],
+    },
+)
 DescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef = TypedDict(
     "DescribeMaintenanceWindowExecutionTaskInvocationsRequestDescribeMaintenanceWindowExecutionTaskInvocationsPaginateTypeDef",
     {
         "WindowExecutionId": str,
         "TaskId": str,
         "Filters": NotRequired[Sequence[MaintenanceWindowFilterTypeDef]],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
@@ -3749,14 +3789,45 @@
         "LastAssociationExecutionDate": NotRequired[datetime],
         "LastSuccessfulAssociationExecutionDate": NotRequired[datetime],
         "AssociationOverview": NotRequired[InstanceAggregatedAssociationOverviewTypeDef],
         "SourceId": NotRequired[str],
         "SourceType": NotRequired[SourceTypeType],
     },
 )
+InstancePropertyTypeDef = TypedDict(
+    "InstancePropertyTypeDef",
+    {
+        "Name": NotRequired[str],
+        "InstanceId": NotRequired[str],
+        "InstanceType": NotRequired[str],
+        "InstanceRole": NotRequired[str],
+        "KeyName": NotRequired[str],
+        "InstanceState": NotRequired[str],
+        "Architecture": NotRequired[str],
+        "IPAddress": NotRequired[str],
+        "LaunchTime": NotRequired[datetime],
+        "PingStatus": NotRequired[PingStatusType],
+        "LastPingDateTime": NotRequired[datetime],
+        "AgentVersion": NotRequired[str],
+        "PlatformType": NotRequired[PlatformTypeType],
+        "PlatformName": NotRequired[str],
+        "PlatformVersion": NotRequired[str],
+        "ActivationId": NotRequired[str],
+        "IamRole": NotRequired[str],
+        "RegistrationDate": NotRequired[datetime],
+        "ResourceType": NotRequired[str],
+        "ComputerName": NotRequired[str],
+        "AssociationStatus": NotRequired[str],
+        "LastAssociationExecutionDate": NotRequired[datetime],
+        "LastSuccessfulAssociationExecutionDate": NotRequired[datetime],
+        "AssociationOverview": NotRequired[InstanceAggregatedAssociationOverviewTypeDef],
+        "SourceId": NotRequired[str],
+        "SourceType": NotRequired[SourceTypeType],
+    },
+)
 InstanceAssociationOutputLocationTypeDef = TypedDict(
     "InstanceAssociationOutputLocationTypeDef",
     {
         "S3Location": NotRequired[S3OutputLocationTypeDef],
     },
 )
 InstanceAssociationOutputUrlTypeDef = TypedDict(
@@ -4388,14 +4459,22 @@
     "DescribeInstanceInformationResultTypeDef",
     {
         "InstanceInformationList": List[InstanceInformationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DescribeInstancePropertiesResultTypeDef = TypedDict(
+    "DescribeInstancePropertiesResultTypeDef",
+    {
+        "InstanceProperties": List[InstancePropertyTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 InstanceAssociationStatusInfoTypeDef = TypedDict(
     "InstanceAssociationStatusInfoTypeDef",
     {
         "AssociationId": NotRequired[str],
         "Name": NotRequired[str],
         "DocumentVersion": NotRequired[str],
         "AssociationVersion": NotRequired[str],
```

### Comparing `mypy-boto3-ssm-1.34.61/mypy_boto3_ssm/waiter.py` & `mypy_boto3_ssm-1.34.91/mypy_boto3_ssm/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.34.61/mypy_boto3_ssm/waiter.pyi` & `mypy_boto3_ssm-1.34.91/mypy_boto3_ssm/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.34.61/mypy_boto3_ssm.egg-info/PKG-INFO` & `mypy_boto3_ssm-1.34.91/mypy_boto3_ssm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm
-Version: 1.34.61
-Summary: Type annotations for boto3.SSM 1.34.61 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.91
+Summary: Type annotations for boto3.SSM 1.34.91 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm)](https://pepy.tech/project/mypy-boto3-ssm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSM 1.34.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
+[boto3.SSM 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -293,14 +293,15 @@
     DescribeEffectiveInstanceAssociationsPaginator,
     DescribeEffectivePatchesForPatchBaselinePaginator,
     DescribeInstanceAssociationsStatusPaginator,
     DescribeInstanceInformationPaginator,
     DescribeInstancePatchStatesPaginator,
     DescribeInstancePatchStatesForPatchGroupPaginator,
     DescribeInstancePatchesPaginator,
+    DescribeInstancePropertiesPaginator,
     DescribeInventoryDeletionsPaginator,
     DescribeMaintenanceWindowExecutionTaskInvocationsPaginator,
     DescribeMaintenanceWindowExecutionTasksPaginator,
     DescribeMaintenanceWindowExecutionsPaginator,
     DescribeMaintenanceWindowSchedulePaginator,
     DescribeMaintenanceWindowTargetsPaginator,
     DescribeMaintenanceWindowTasksPaginator,
@@ -372,14 +373,17 @@
 )
 describe_instance_patch_states_for_patch_group_paginator: (
     DescribeInstancePatchStatesForPatchGroupPaginator
 ) = client.get_paginator("describe_instance_patch_states_for_patch_group")
 describe_instance_patches_paginator: DescribeInstancePatchesPaginator = client.get_paginator(
     "describe_instance_patches"
 )
+describe_instance_properties_paginator: DescribeInstancePropertiesPaginator = client.get_paginator(
+    "describe_instance_properties"
+)
 describe_inventory_deletions_paginator: DescribeInventoryDeletionsPaginator = client.get_paginator(
     "describe_inventory_deletions"
 )
 describe_maintenance_window_execution_task_invocations_paginator: (
     DescribeMaintenanceWindowExecutionTaskInvocationsPaginator
 ) = client.get_paginator("describe_maintenance_window_execution_task_invocations")
 describe_maintenance_window_execution_tasks_paginator: (
```

### Comparing `mypy-boto3-ssm-1.34.61/mypy_boto3_ssm.egg-info/SOURCES.txt` & `mypy_boto3_ssm-1.34.91/mypy_boto3_ssm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.34.61/setup.py` & `mypy_boto3_ssm-1.34.91/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ssm",
-    version="1.34.61",
+    version="1.34.91",
     packages=["mypy_boto3_ssm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.SSM 1.34.61 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.SSM 1.34.91 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

