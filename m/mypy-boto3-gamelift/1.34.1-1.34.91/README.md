# Comparing `tmp/mypy-boto3-gamelift-1.34.1.tar.gz` & `tmp/mypy_boto3_gamelift-1.34.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-gamelift-1.34.1.tar", last modified: Thu Dec 14 20:49:25 2023, max compression
+gzip compressed data, was "mypy_boto3_gamelift-1.34.91.tar", last modified: Wed Apr 24 19:19:06 2024, max compression
```

## Comparing `mypy-boto3-gamelift-1.34.1.tar` & `mypy_boto3_gamelift-1.34.91.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 20:49:25.549065 mypy-boto3-gamelift-1.34.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-14 20:47:11.000000 mypy-boto3-gamelift-1.34.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15902 2023-12-14 20:49:25.549065 mypy-boto3-gamelift-1.34.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14365 2023-12-14 20:47:11.000000 mypy-boto3-gamelift-1.34.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 20:49:25.549065 mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift/
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2023-12-14 20:47:12.000000 mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2023-12-14 20:47:11.000000 mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      909 2023-12-14 20:47:12.000000 mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    85206 2023-12-14 20:47:12.000000 mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    85202 2023-12-14 20:47:12.000000 mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    22492 2023-12-14 20:47:12.000000 mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    22490 2023-12-14 20:47:12.000000 mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    26542 2023-12-14 20:47:12.000000 mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    26518 2023-12-14 20:47:12.000000 mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-14 20:47:12.000000 mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    89696 2023-12-14 20:47:14.000000 mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    89695 2023-12-14 20:47:14.000000 mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-14 20:47:11.000000 mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-14 20:49:25.549065 mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15902 2023-12-14 20:49:25.000000 mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      699 2023-12-14 20:49:25.000000 mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-14 20:49:25.000000 mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-14 20:49:25.000000 mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-14 20:49:25.000000 mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-14 20:49:25.000000 mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-14 20:49:25.549065 mypy-boto3-gamelift-1.34.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2023-12-14 20:47:11.000000 mypy-boto3-gamelift-1.34.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:06.623885 mypy_boto3_gamelift-1.34.91/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-24 19:18:41.000000 mypy_boto3_gamelift-1.34.91/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16119 2024-04-24 19:19:06.623885 mypy_boto3_gamelift-1.34.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14560 2024-04-24 19:18:41.000000 mypy_boto3_gamelift-1.34.91/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:06.623885 mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift/
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-24 19:18:41.000000 mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-24 19:18:41.000000 mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-24 19:18:41.000000 mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91112 2024-04-24 19:18:42.000000 mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91109 2024-04-24 19:18:41.000000 mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    23284 2024-04-24 19:18:42.000000 mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23284 2024-04-24 19:18:42.000000 mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    27941 2024-04-24 19:18:42.000000 mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27917 2024-04-24 19:18:42.000000 mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:18:41.000000 mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   101398 2024-04-24 19:18:45.000000 mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101398 2024-04-24 19:18:44.000000 mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-24 19:18:41.000000 mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:06.623885 mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16119 2024-04-24 19:19:06.000000 mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-24 19:19:06.000000 mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:19:06.000000 mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:19:06.000000 mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-24 19:19:06.000000 mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-24 19:19:06.000000 mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:19:06.623885 mypy_boto3_gamelift-1.34.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-24 19:18:41.000000 mypy_boto3_gamelift-1.34.91/setup.py
```

### Comparing `mypy-boto3-gamelift-1.34.1/LICENSE` & `mypy_boto3_gamelift-1.34.91/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-gamelift-1.34.1/PKG-INFO` & `mypy_boto3_gamelift-1.34.91/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-gamelift
-Version: 1.34.1
-Summary: Type annotations for boto3.GameLift 1.34.1 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.91
+Summary: Type annotations for boto3.GameLift 1.34.91 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-gamelift"></a>
 
 # mypy-boto3-gamelift
 
 [![PyPI - mypy-boto3-gamelift](https://img.shields.io/pypi/v/mypy-boto3-gamelift.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamelift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-gamelift.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamelift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-gamelift)](https://pepy.tech/project/mypy-boto3-gamelift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GameLift 1.34.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
+[boto3.GameLift 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-gamelift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -296,14 +296,15 @@
     DescribeMatchmakingConfigurationsPaginator,
     DescribeMatchmakingRuleSetsPaginator,
     DescribePlayerSessionsPaginator,
     DescribeScalingPoliciesPaginator,
     ListAliasesPaginator,
     ListBuildsPaginator,
     ListComputePaginator,
+    ListContainerGroupDefinitionsPaginator,
     ListFleetsPaginator,
     ListGameServerGroupsPaginator,
     ListGameServersPaginator,
     ListLocationsPaginator,
     ListScriptsPaginator,
     SearchGameSessionsPaginator,
 )
@@ -350,14 +351,17 @@
 )
 describe_scaling_policies_paginator: DescribeScalingPoliciesPaginator = client.get_paginator(
     "describe_scaling_policies"
 )
 list_aliases_paginator: ListAliasesPaginator = client.get_paginator("list_aliases")
 list_builds_paginator: ListBuildsPaginator = client.get_paginator("list_builds")
 list_compute_paginator: ListComputePaginator = client.get_paginator("list_compute")
+list_container_group_definitions_paginator: ListContainerGroupDefinitionsPaginator = (
+    client.get_paginator("list_container_group_definitions")
+)
 list_fleets_paginator: ListFleetsPaginator = client.get_paginator("list_fleets")
 list_game_server_groups_paginator: ListGameServerGroupsPaginator = client.get_paginator(
     "list_game_server_groups"
 )
 list_game_servers_paginator: ListGameServersPaginator = client.get_paginator("list_game_servers")
 list_locations_paginator: ListLocationsPaginator = client.get_paginator("list_locations")
 list_scripts_paginator: ListScriptsPaginator = client.get_paginator("list_scripts")
```

### Comparing `mypy-boto3-gamelift-1.34.1/README.md` & `mypy_boto3_gamelift-1.34.91/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-gamelift.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamelift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-gamelift)](https://pepy.tech/project/mypy-boto3-gamelift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GameLift 1.34.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
+[boto3.GameLift 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-gamelift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -263,14 +263,15 @@
     DescribeMatchmakingConfigurationsPaginator,
     DescribeMatchmakingRuleSetsPaginator,
     DescribePlayerSessionsPaginator,
     DescribeScalingPoliciesPaginator,
     ListAliasesPaginator,
     ListBuildsPaginator,
     ListComputePaginator,
+    ListContainerGroupDefinitionsPaginator,
     ListFleetsPaginator,
     ListGameServerGroupsPaginator,
     ListGameServersPaginator,
     ListLocationsPaginator,
     ListScriptsPaginator,
     SearchGameSessionsPaginator,
 )
@@ -317,14 +318,17 @@
 )
 describe_scaling_policies_paginator: DescribeScalingPoliciesPaginator = client.get_paginator(
     "describe_scaling_policies"
 )
 list_aliases_paginator: ListAliasesPaginator = client.get_paginator("list_aliases")
 list_builds_paginator: ListBuildsPaginator = client.get_paginator("list_builds")
 list_compute_paginator: ListComputePaginator = client.get_paginator("list_compute")
+list_container_group_definitions_paginator: ListContainerGroupDefinitionsPaginator = (
+    client.get_paginator("list_container_group_definitions")
+)
 list_fleets_paginator: ListFleetsPaginator = client.get_paginator("list_fleets")
 list_game_server_groups_paginator: ListGameServerGroupsPaginator = client.get_paginator(
     "list_game_server_groups"
 )
 list_game_servers_paginator: ListGameServersPaginator = client.get_paginator("list_game_servers")
 list_locations_paginator: ListLocationsPaginator = client.get_paginator("list_locations")
 list_scripts_paginator: ListScriptsPaginator = client.get_paginator("list_scripts")
```

### Comparing `mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift/__init__.py` & `mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         DescribeMatchmakingRuleSetsPaginator,
         DescribePlayerSessionsPaginator,
         DescribeScalingPoliciesPaginator,
         GameLiftClient,
         ListAliasesPaginator,
         ListBuildsPaginator,
         ListComputePaginator,
+        ListContainerGroupDefinitionsPaginator,
         ListFleetsPaginator,
         ListGameServerGroupsPaginator,
         ListGameServersPaginator,
         ListLocationsPaginator,
         ListScriptsPaginator,
         SearchGameSessionsPaginator,
     )
@@ -47,14 +48,15 @@
     describe_matchmaking_configurations_paginator: DescribeMatchmakingConfigurationsPaginator = client.get_paginator("describe_matchmaking_configurations")
     describe_matchmaking_rule_sets_paginator: DescribeMatchmakingRuleSetsPaginator = client.get_paginator("describe_matchmaking_rule_sets")
     describe_player_sessions_paginator: DescribePlayerSessionsPaginator = client.get_paginator("describe_player_sessions")
     describe_scaling_policies_paginator: DescribeScalingPoliciesPaginator = client.get_paginator("describe_scaling_policies")
     list_aliases_paginator: ListAliasesPaginator = client.get_paginator("list_aliases")
     list_builds_paginator: ListBuildsPaginator = client.get_paginator("list_builds")
     list_compute_paginator: ListComputePaginator = client.get_paginator("list_compute")
+    list_container_group_definitions_paginator: ListContainerGroupDefinitionsPaginator = client.get_paginator("list_container_group_definitions")
     list_fleets_paginator: ListFleetsPaginator = client.get_paginator("list_fleets")
     list_game_server_groups_paginator: ListGameServerGroupsPaginator = client.get_paginator("list_game_server_groups")
     list_game_servers_paginator: ListGameServersPaginator = client.get_paginator("list_game_servers")
     list_locations_paginator: ListLocationsPaginator = client.get_paginator("list_locations")
     list_scripts_paginator: ListScriptsPaginator = client.get_paginator("list_scripts")
     search_game_sessions_paginator: SearchGameSessionsPaginator = client.get_paginator("search_game_sessions")
     ```
@@ -74,25 +76,25 @@
     DescribeMatchmakingConfigurationsPaginator,
     DescribeMatchmakingRuleSetsPaginator,
     DescribePlayerSessionsPaginator,
     DescribeScalingPoliciesPaginator,
     ListAliasesPaginator,
     ListBuildsPaginator,
     ListComputePaginator,
+    ListContainerGroupDefinitionsPaginator,
     ListFleetsPaginator,
     ListGameServerGroupsPaginator,
     ListGameServersPaginator,
     ListLocationsPaginator,
     ListScriptsPaginator,
     SearchGameSessionsPaginator,
 )
 
 Client = GameLiftClient
 
-
 __all__ = (
     "Client",
     "DescribeFleetAttributesPaginator",
     "DescribeFleetCapacityPaginator",
     "DescribeFleetEventsPaginator",
     "DescribeFleetUtilizationPaginator",
     "DescribeGameServerInstancesPaginator",
@@ -104,14 +106,15 @@
     "DescribeMatchmakingRuleSetsPaginator",
     "DescribePlayerSessionsPaginator",
     "DescribeScalingPoliciesPaginator",
     "GameLiftClient",
     "ListAliasesPaginator",
     "ListBuildsPaginator",
     "ListComputePaginator",
+    "ListContainerGroupDefinitionsPaginator",
     "ListFleetsPaginator",
     "ListGameServerGroupsPaginator",
     "ListGameServersPaginator",
     "ListLocationsPaginator",
     "ListScriptsPaginator",
     "SearchGameSessionsPaginator",
 )
```

### Comparing `mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift/__init__.pyi` & `mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift/__init__.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         DescribeMatchmakingRuleSetsPaginator,
         DescribePlayerSessionsPaginator,
         DescribeScalingPoliciesPaginator,
         GameLiftClient,
         ListAliasesPaginator,
         ListBuildsPaginator,
         ListComputePaginator,
+        ListContainerGroupDefinitionsPaginator,
         ListFleetsPaginator,
         ListGameServerGroupsPaginator,
         ListGameServersPaginator,
         ListLocationsPaginator,
         ListScriptsPaginator,
         SearchGameSessionsPaginator,
     )
@@ -47,14 +48,15 @@
     describe_matchmaking_configurations_paginator: DescribeMatchmakingConfigurationsPaginator = client.get_paginator("describe_matchmaking_configurations")
     describe_matchmaking_rule_sets_paginator: DescribeMatchmakingRuleSetsPaginator = client.get_paginator("describe_matchmaking_rule_sets")
     describe_player_sessions_paginator: DescribePlayerSessionsPaginator = client.get_paginator("describe_player_sessions")
     describe_scaling_policies_paginator: DescribeScalingPoliciesPaginator = client.get_paginator("describe_scaling_policies")
     list_aliases_paginator: ListAliasesPaginator = client.get_paginator("list_aliases")
     list_builds_paginator: ListBuildsPaginator = client.get_paginator("list_builds")
     list_compute_paginator: ListComputePaginator = client.get_paginator("list_compute")
+    list_container_group_definitions_paginator: ListContainerGroupDefinitionsPaginator = client.get_paginator("list_container_group_definitions")
     list_fleets_paginator: ListFleetsPaginator = client.get_paginator("list_fleets")
     list_game_server_groups_paginator: ListGameServerGroupsPaginator = client.get_paginator("list_game_server_groups")
     list_game_servers_paginator: ListGameServersPaginator = client.get_paginator("list_game_servers")
     list_locations_paginator: ListLocationsPaginator = client.get_paginator("list_locations")
     list_scripts_paginator: ListScriptsPaginator = client.get_paginator("list_scripts")
     search_game_sessions_paginator: SearchGameSessionsPaginator = client.get_paginator("search_game_sessions")
     ```
@@ -74,14 +76,15 @@
     DescribeMatchmakingConfigurationsPaginator,
     DescribeMatchmakingRuleSetsPaginator,
     DescribePlayerSessionsPaginator,
     DescribeScalingPoliciesPaginator,
     ListAliasesPaginator,
     ListBuildsPaginator,
     ListComputePaginator,
+    ListContainerGroupDefinitionsPaginator,
     ListFleetsPaginator,
     ListGameServerGroupsPaginator,
     ListGameServersPaginator,
     ListLocationsPaginator,
     ListScriptsPaginator,
     SearchGameSessionsPaginator,
 )
@@ -103,14 +106,15 @@
     "DescribeMatchmakingRuleSetsPaginator",
     "DescribePlayerSessionsPaginator",
     "DescribeScalingPoliciesPaginator",
     "GameLiftClient",
     "ListAliasesPaginator",
     "ListBuildsPaginator",
     "ListComputePaginator",
+    "ListContainerGroupDefinitionsPaginator",
     "ListFleetsPaginator",
     "ListGameServerGroupsPaginator",
     "ListGameServersPaginator",
     "ListLocationsPaginator",
     "ListScriptsPaginator",
     "SearchGameSessionsPaginator",
 )
```

### Comparing `mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift/client.py` & `mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from .literals import (
     AcceptanceTypeType,
     BackfillModeType,
     BalancingStrategyType,
     BuildStatusType,
     ComparisonOperatorTypeType,
     ComputeTypeType,
+    ContainerSchedulingStrategyType,
     EC2InstanceTypeType,
     FleetTypeType,
     FlexMatchModeType,
     GameServerGroupDeleteOptionType,
     GameServerProtectionPolicyType,
     GameServerUtilizationStatusType,
     LocationFilterType,
@@ -56,29 +57,33 @@
     DescribeMatchmakingConfigurationsPaginator,
     DescribeMatchmakingRuleSetsPaginator,
     DescribePlayerSessionsPaginator,
     DescribeScalingPoliciesPaginator,
     ListAliasesPaginator,
     ListBuildsPaginator,
     ListComputePaginator,
+    ListContainerGroupDefinitionsPaginator,
     ListFleetsPaginator,
     ListGameServerGroupsPaginator,
     ListGameServersPaginator,
     ListLocationsPaginator,
     ListScriptsPaginator,
     SearchGameSessionsPaginator,
 )
 from .type_defs import (
     AnywhereConfigurationTypeDef,
     BlobTypeDef,
     CertificateConfigurationTypeDef,
     ClaimFilterOptionTypeDef,
     ClaimGameServerOutputTypeDef,
+    ContainerDefinitionInputTypeDef,
+    ContainerGroupsConfigurationTypeDef,
     CreateAliasOutputTypeDef,
     CreateBuildOutputTypeDef,
+    CreateContainerGroupDefinitionOutputTypeDef,
     CreateFleetLocationsOutputTypeDef,
     CreateFleetOutputTypeDef,
     CreateGameServerGroupOutputTypeDef,
     CreateGameSessionOutputTypeDef,
     CreateGameSessionQueueOutputTypeDef,
     CreateLocationOutputTypeDef,
     CreateMatchmakingConfigurationOutputTypeDef,
@@ -88,14 +93,15 @@
     CreateScriptOutputTypeDef,
     CreateVpcPeeringAuthorizationOutputTypeDef,
     DeleteFleetLocationsOutputTypeDef,
     DeleteGameServerGroupOutputTypeDef,
     DescribeAliasOutputTypeDef,
     DescribeBuildOutputTypeDef,
     DescribeComputeOutputTypeDef,
+    DescribeContainerGroupDefinitionOutputTypeDef,
     DescribeEC2InstanceLimitsOutputTypeDef,
     DescribeFleetAttributesOutputTypeDef,
     DescribeFleetCapacityOutputTypeDef,
     DescribeFleetEventsOutputTypeDef,
     DescribeFleetLocationAttributesOutputTypeDef,
     DescribeFleetLocationCapacityOutputTypeDef,
     DescribeFleetLocationUtilizationOutputTypeDef,
@@ -130,14 +136,15 @@
     GetInstanceAccessOutputTypeDef,
     InstanceDefinitionTypeDef,
     IpPermissionTypeDef,
     LaunchTemplateSpecificationTypeDef,
     ListAliasesOutputTypeDef,
     ListBuildsOutputTypeDef,
     ListComputeOutputTypeDef,
+    ListContainerGroupDefinitionsOutputTypeDef,
     ListFleetsOutputTypeDef,
     ListGameServerGroupsOutputTypeDef,
     ListGameServersOutputTypeDef,
     ListLocationsOutputTypeDef,
     ListScriptsOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     LocationConfigurationTypeDef,
@@ -182,15 +189,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("GameLiftClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -206,14 +212,15 @@
     IdempotentParameterMismatchException: Type[BotocoreClientError]
     InternalServiceException: Type[BotocoreClientError]
     InvalidFleetStatusException: Type[BotocoreClientError]
     InvalidGameSessionStatusException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
+    NotReadyException: Type[BotocoreClientError]
     OutOfCapacityException: Type[BotocoreClientError]
     TaggingFailedException: Type[BotocoreClientError]
     TerminalRoutingStrategyException: Type[BotocoreClientError]
     UnauthorizedException: Type[BotocoreClientError]
     UnsupportedRegionException: Type[BotocoreClientError]
 
 
@@ -254,15 +261,15 @@
 
     def claim_game_server(
         self,
         *,
         GameServerGroupName: str,
         GameServerId: str = ...,
         GameServerData: str = ...,
-        FilterOption: ClaimFilterOptionTypeDef = ...
+        FilterOption: ClaimFilterOptionTypeDef = ...,
     ) -> ClaimGameServerOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Locates an available game server and temporarily reserves it
         to host gameplay and
         players.
 
@@ -280,15 +287,15 @@
 
     def create_alias(
         self,
         *,
         Name: str,
         RoutingStrategy: RoutingStrategyTypeDef,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAliasOutputTypeDef:
         """
         Creates an alias for a fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#create_alias)
         """
@@ -297,23 +304,45 @@
         self,
         *,
         Name: str = ...,
         Version: str = ...,
         StorageLocation: S3LocationTypeDef = ...,
         OperatingSystem: OperatingSystemType = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ServerSdkVersion: str = ...
+        ServerSdkVersion: str = ...,
     ) -> CreateBuildOutputTypeDef:
         """
         Creates a new Amazon GameLift build resource for your game server binary files.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_build)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#create_build)
         """
 
+    def create_container_group_definition(
+        self,
+        *,
+        Name: str,
+        TotalMemoryLimit: int,
+        TotalCpuLimit: int,
+        ContainerDefinitions: Sequence[ContainerDefinitionInputTypeDef],
+        OperatingSystem: Literal["AMAZON_LINUX_2023"],
+        SchedulingStrategy: ContainerSchedulingStrategyType = ...,
+        Tags: Sequence[TagTypeDef] = ...,
+    ) -> CreateContainerGroupDefinitionOutputTypeDef:
+        """
+        **This operation is used with the Amazon GameLift containers feature, which is
+        currently in public preview.** Creates a `ContainerGroupDefinition` resource
+        that describes a set of containers for hosting your game server with Amazon
+        GameLift managed EC2
+        hosting.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_container_group_definition)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#create_container_group_definition)
+        """
+
     def create_fleet(
         self,
         *,
         Name: str,
         Description: str = ...,
         BuildId: str = ...,
         ScriptId: str = ...,
@@ -331,31 +360,34 @@
         FleetType: FleetTypeType = ...,
         InstanceRoleArn: str = ...,
         CertificateConfiguration: CertificateConfigurationTypeDef = ...,
         Locations: Sequence[LocationConfigurationTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ComputeType: ComputeTypeType = ...,
         AnywhereConfiguration: AnywhereConfigurationTypeDef = ...,
-        InstanceRoleCredentialsProvider: Literal["SHARED_CREDENTIAL_FILE"] = ...
+        InstanceRoleCredentialsProvider: Literal["SHARED_CREDENTIAL_FILE"] = ...,
+        ContainerGroupsConfiguration: ContainerGroupsConfigurationTypeDef = ...,
     ) -> CreateFleetOutputTypeDef:
         """
-        Creates a fleet of Amazon Elastic Compute Cloud (Amazon EC2) instances to host
-        your custom game server or Realtime
-        Servers.
+        **This operation has been expanded to use with the Amazon GameLift containers
+        feature, which is currently in public preview.** Creates a fleet of compute
+        resources to host your game
+        servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_fleet)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#create_fleet)
         """
 
     def create_fleet_locations(
         self, *, FleetId: str, Locations: Sequence[LocationConfigurationTypeDef]
     ) -> CreateFleetLocationsOutputTypeDef:
         """
-        Adds remote locations to a fleet and begins populating the new locations with
-        EC2
+        **This operation has been expanded to use with the Amazon GameLift containers
+        feature, which is currently in public preview.** Adds remote locations to an
+        EC2 or container fleet and begins populating the new locations with
         instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_fleet_locations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#create_fleet_locations)
         """
 
     def create_game_server_group(
@@ -367,15 +399,15 @@
         MaxSize: int,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef,
         InstanceDefinitions: Sequence[InstanceDefinitionTypeDef],
         AutoScalingPolicy: GameServerGroupAutoScalingPolicyTypeDef = ...,
         BalancingStrategy: BalancingStrategyType = ...,
         GameServerProtectionPolicy: GameServerProtectionPolicyType = ...,
         VpcSubnets: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateGameServerGroupOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Creates a Amazon GameLift FleetIQ game server group for
         managing game hosting on a collection of Amazon Elastic Compute Cloud instances
         for game
         hosting.
@@ -392,15 +424,15 @@
         AliasId: str = ...,
         Name: str = ...,
         GameProperties: Sequence[GamePropertyTypeDef] = ...,
         CreatorId: str = ...,
         GameSessionId: str = ...,
         IdempotencyToken: str = ...,
         GameSessionData: str = ...,
-        Location: str = ...
+        Location: str = ...,
     ) -> CreateGameSessionOutputTypeDef:
         """
         Creates a multiplayer game session for players in a specific fleet location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_game_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#create_game_session)
         """
@@ -412,15 +444,15 @@
         TimeoutInSeconds: int = ...,
         PlayerLatencyPolicies: Sequence[PlayerLatencyPolicyTypeDef] = ...,
         Destinations: Sequence[GameSessionQueueDestinationTypeDef] = ...,
         FilterConfiguration: FilterConfigurationTypeDef = ...,
         PriorityConfiguration: PriorityConfigurationTypeDef = ...,
         CustomEventData: str = ...,
         NotificationTarget: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateGameSessionQueueOutputTypeDef:
         """
         Creates a placement queue that processes requests for new game sessions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_game_session_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#create_game_session_queue)
         """
@@ -448,15 +480,15 @@
         NotificationTarget: str = ...,
         AdditionalPlayerCount: int = ...,
         CustomEventData: str = ...,
         GameProperties: Sequence[GamePropertyTypeDef] = ...,
         GameSessionData: str = ...,
         BackfillMode: BackfillModeType = ...,
         FlexMatchMode: FlexMatchModeType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMatchmakingConfigurationOutputTypeDef:
         """
         Defines a new matchmaking configuration for use with FlexMatch.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_matchmaking_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#create_matchmaking_configuration)
         """
@@ -482,15 +514,15 @@
         """
 
     def create_player_sessions(
         self,
         *,
         GameSessionId: str,
         PlayerIds: Sequence[str],
-        PlayerDataMap: Mapping[str, str] = ...
+        PlayerDataMap: Mapping[str, str] = ...,
     ) -> CreatePlayerSessionsOutputTypeDef:
         """
         Reserves open slots in a game session for a group of players.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_player_sessions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#create_player_sessions)
         """
@@ -498,15 +530,15 @@
     def create_script(
         self,
         *,
         Name: str = ...,
         Version: str = ...,
         StorageLocation: S3LocationTypeDef = ...,
         ZipFile: BlobTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateScriptOutputTypeDef:
         """
         Creates a new script record for your Realtime Servers script.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_script)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#create_script)
         """
@@ -548,17 +580,29 @@
         """
         Deletes a build.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.delete_build)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#delete_build)
         """
 
+    def delete_container_group_definition(self, *, Name: str) -> EmptyResponseMetadataTypeDef:
+        """
+        **This operation is used with the Amazon GameLift containers feature, which is
+        currently in public preview.** Deletes a container group definition
+        resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.delete_container_group_definition)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#delete_container_group_definition)
+        """
+
     def delete_fleet(self, *, FleetId: str) -> EmptyResponseMetadataTypeDef:
         """
-        Deletes all resources and information related a fleet.
+        Deletes all resources and information related to a fleet and shuts down any
+        currently running fleet instances, including those in remote
+        locations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.delete_fleet)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#delete_fleet)
         """
 
     def delete_fleet_locations(
         self, *, FleetId: str, Locations: Sequence[str]
@@ -649,15 +693,18 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.delete_vpc_peering_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#delete_vpc_peering_connection)
         """
 
     def deregister_compute(self, *, FleetId: str, ComputeName: str) -> Dict[str, Any]:
         """
-        Removes a compute resource from an Amazon GameLift Anywhere fleet.
+        **This operation has been expanded to use with the Amazon GameLift containers
+        feature, which is currently in public preview.** Removes a compute resource
+        from an Amazon GameLift Anywhere fleet or container
+        fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.deregister_compute)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#deregister_compute)
         """
 
     def deregister_game_server(
         self, *, GameServerGroupName: str, GameServerId: str
@@ -685,20 +732,36 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_build)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_build)
         """
 
     def describe_compute(self, *, FleetId: str, ComputeName: str) -> DescribeComputeOutputTypeDef:
         """
-        Retrieves properties for a compute resource in an Amazon GameLift fleet.
+        **This operation has been expanded to use with the Amazon GameLift containers
+        feature, which is currently in public preview.** Retrieves properties for a
+        compute resource in an Amazon GameLift
+        fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_compute)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_compute)
         """
 
+    def describe_container_group_definition(
+        self, *, Name: str
+    ) -> DescribeContainerGroupDefinitionOutputTypeDef:
+        """
+        **This operation is used with the Amazon GameLift containers feature, which is
+        currently in public preview.** Retrieves the properties of a container group
+        definition, including all container definitions in the
+        group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_container_group_definition)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_container_group_definition)
+        """
+
     def describe_ec2_instance_limits(
         self, *, EC2InstanceType: EC2InstanceTypeType = ..., Location: str = ...
     ) -> DescribeEC2InstanceLimitsOutputTypeDef:
         """
         Retrieves the instance limits and current utilization for an Amazon Web
         Services Region or
         location.
@@ -707,55 +770,59 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_ec2_instance_limits)
         """
 
     def describe_fleet_attributes(
         self, *, FleetIds: Sequence[str] = ..., Limit: int = ..., NextToken: str = ...
     ) -> DescribeFleetAttributesOutputTypeDef:
         """
-        Retrieves core fleet-wide properties, including the computing hardware and
-        deployment configuration for all instances in the
-        fleet.
+        **This operation has been expanded to use with the Amazon GameLift containers
+        feature, which is currently in public preview.** Retrieves core fleet-wide
+        properties for fleets in an Amazon Web Services
+        Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_fleet_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_fleet_attributes)
         """
 
     def describe_fleet_capacity(
         self, *, FleetIds: Sequence[str] = ..., Limit: int = ..., NextToken: str = ...
     ) -> DescribeFleetCapacityOutputTypeDef:
         """
-        Retrieves the resource capacity settings for one or more fleets.
+        **This operation has been expanded to use with the Amazon GameLift containers
+        feature, which is currently in public preview.** Retrieves the resource
+        capacity settings for one or more
+        fleets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_fleet_capacity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_fleet_capacity)
         """
 
     def describe_fleet_events(
         self,
         *,
         FleetId: str,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeFleetEventsOutputTypeDef:
         """
         Retrieves entries from a fleet's event log.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_fleet_events)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_fleet_events)
         """
 
     def describe_fleet_location_attributes(
         self,
         *,
         FleetId: str,
         Locations: Sequence[str] = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeFleetLocationAttributesOutputTypeDef:
         """
         Retrieves information on a fleet's remote locations, including life-cycle
         status and any suspended fleet
         activity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_fleet_location_attributes)
@@ -828,15 +895,15 @@
 
     def describe_game_server_instances(
         self,
         *,
         GameServerGroupName: str,
         InstanceIds: Sequence[str] = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeGameServerInstancesOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Retrieves status information about the Amazon EC2 instances
         associated with a Amazon GameLift FleetIQ game server
         group.
 
@@ -849,15 +916,15 @@
         *,
         FleetId: str = ...,
         GameSessionId: str = ...,
         AliasId: str = ...,
         Location: str = ...,
         StatusFilter: str = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeGameSessionDetailsOutputTypeDef:
         """
         Retrieves additional game session properties, including the game session
         protection policy in force, a set of one or more game sessions in a specific
         fleet
         location.
 
@@ -891,15 +958,15 @@
         *,
         FleetId: str = ...,
         GameSessionId: str = ...,
         AliasId: str = ...,
         Location: str = ...,
         StatusFilter: str = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeGameSessionsOutputTypeDef:
         """
         Retrieves a set of one or more game sessions in a specific fleet location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_game_sessions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_game_sessions)
         """
@@ -907,15 +974,15 @@
     def describe_instances(
         self,
         *,
         FleetId: str,
         InstanceId: str = ...,
         Limit: int = ...,
         NextToken: str = ...,
-        Location: str = ...
+        Location: str = ...,
     ) -> DescribeInstancesOutputTypeDef:
         """
         Retrieves information about the EC2 instances in an Amazon GameLift managed
         fleet, including instance ID, connection data, and
         status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_instances)
@@ -932,15 +999,15 @@
 
     def describe_matchmaking_configurations(
         self,
         *,
         Names: Sequence[str] = ...,
         RuleSetName: str = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeMatchmakingConfigurationsOutputTypeDef:
         """
         Retrieves the details of FlexMatch matchmaking configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_matchmaking_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_matchmaking_configurations)
         """
@@ -959,15 +1026,15 @@
         self,
         *,
         GameSessionId: str = ...,
         PlayerId: str = ...,
         PlayerSessionId: str = ...,
         PlayerSessionStatusFilter: str = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribePlayerSessionsOutputTypeDef:
         """
         Retrieves properties for one or more player sessions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_player_sessions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_player_sessions)
         """
@@ -985,15 +1052,15 @@
     def describe_scaling_policies(
         self,
         *,
         FleetId: str,
         StatusFilter: ScalingStatusTypeType = ...,
         Limit: int = ...,
         NextToken: str = ...,
-        Location: str = ...
+        Location: str = ...,
     ) -> DescribeScalingPoliciesOutputTypeDef:
         """
         Retrieves all scaling policies applied to a fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_scaling_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_scaling_policies)
         """
@@ -1040,28 +1107,29 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#generate_presigned_url)
         """
 
     def get_compute_access(
         self, *, FleetId: str, ComputeName: str
     ) -> GetComputeAccessOutputTypeDef:
         """
-        Requests authorization to remotely connect to a compute resource in an Amazon
-        GameLift
+        **This operation has been expanded to use with the Amazon GameLift containers
+        feature, which is currently in public preview.** Requests authorization to
+        remotely connect to a hosting resource in a Amazon GameLift managed
         fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.get_compute_access)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#get_compute_access)
         """
 
     def get_compute_auth_token(
         self, *, FleetId: str, ComputeName: str
     ) -> GetComputeAuthTokenOutputTypeDef:
         """
-        Requests an authentication token from Amazon GameLift for a registered compute
-        in an Anywhere
+        Requests an authentication token from Amazon GameLift for a compute resource in
+        an Amazon GameLift Anywhere fleet or container
         fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.get_compute_auth_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#get_compute_auth_token)
         """
 
     def get_game_session_log_url(self, *, GameSessionId: str) -> GetGameSessionLogUrlOutputTypeDef:
@@ -1088,15 +1156,15 @@
 
     def list_aliases(
         self,
         *,
         RoutingStrategyType: RoutingStrategyTypeType = ...,
         Name: str = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAliasesOutputTypeDef:
         """
         Retrieves all aliases for this Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.list_aliases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#list_aliases)
         """
@@ -1113,25 +1181,55 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#list_builds)
         """
 
     def list_compute(
         self, *, FleetId: str, Location: str = ..., Limit: int = ..., NextToken: str = ...
     ) -> ListComputeOutputTypeDef:
         """
-        Retrieves the compute resources in an Amazon GameLift fleet.
+        **This operation has been expanded to use with the Amazon GameLift containers
+        feature, which is currently in public preview.** Retrieves information on the
+        compute resources in an Amazon GameLift
+        fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.list_compute)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#list_compute)
         """
 
+    def list_container_group_definitions(
+        self,
+        *,
+        SchedulingStrategy: ContainerSchedulingStrategyType = ...,
+        Limit: int = ...,
+        NextToken: str = ...,
+    ) -> ListContainerGroupDefinitionsOutputTypeDef:
+        """
+        **This operation is used with the Amazon GameLift containers feature, which is
+        currently in public preview.** Retrieves all container group definitions for
+        the Amazon Web Services account and Amazon Web Services Region that are
+        currently in
+        use.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.list_container_group_definitions)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#list_container_group_definitions)
+        """
+
     def list_fleets(
-        self, *, BuildId: str = ..., ScriptId: str = ..., Limit: int = ..., NextToken: str = ...
+        self,
+        *,
+        BuildId: str = ...,
+        ScriptId: str = ...,
+        ContainerGroupDefinitionName: str = ...,
+        Limit: int = ...,
+        NextToken: str = ...,
     ) -> ListFleetsOutputTypeDef:
         """
-        Retrieves a collection of fleet resources in an Amazon Web Services Region.
+        **This operation has been expanded to use with the Amazon GameLift containers
+        feature, which is currently in public preview.** Retrieves a collection of
+        fleet resources in an Amazon Web Services
+        Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.list_fleets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#list_fleets)
         """
 
     def list_game_server_groups(
         self, *, Limit: int = ..., NextToken: str = ...
@@ -1145,15 +1243,15 @@
 
     def list_game_servers(
         self,
         *,
         GameServerGroupName: str,
         SortOrder: SortOrderType = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListGameServersOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Retrieves information on all game servers that are currently
         active in a specified game server
         group.
 
@@ -1197,15 +1295,15 @@
         MetricName: MetricNameType,
         ScalingAdjustment: int = ...,
         ScalingAdjustmentType: ScalingAdjustmentTypeType = ...,
         Threshold: float = ...,
         ComparisonOperator: ComparisonOperatorTypeType = ...,
         EvaluationPeriods: int = ...,
         PolicyType: PolicyTypeType = ...,
-        TargetConfiguration: TargetConfigurationTypeDef = ...
+        TargetConfiguration: TargetConfigurationTypeDef = ...,
     ) -> PutScalingPolicyOutputTypeDef:
         """
         Creates or updates a scaling policy for a fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.put_scaling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#put_scaling_policy)
         """
@@ -1214,31 +1312,34 @@
         self,
         *,
         FleetId: str,
         ComputeName: str,
         CertificatePath: str = ...,
         DnsName: str = ...,
         IpAddress: str = ...,
-        Location: str = ...
+        Location: str = ...,
     ) -> RegisterComputeOutputTypeDef:
         """
-        Registers a compute resource to an Amazon GameLift Anywhere fleet.
+        **This operation has been expanded to use with the Amazon GameLift containers
+        feature, which is currently in public preview.** Registers a compute resource
+        in an Amazon GameLift
+        fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.register_compute)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#register_compute)
         """
 
     def register_game_server(
         self,
         *,
         GameServerGroupName: str,
         GameServerId: str,
         InstanceId: str,
         ConnectionInfo: str = ...,
-        GameServerData: str = ...
+        GameServerData: str = ...,
     ) -> RegisterGameServerOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Creates a new game server resource and notifies Amazon
         GameLift FleetIQ that the game server is ready to host gameplay and
         players.
 
@@ -1254,25 +1355,25 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.request_upload_credentials)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#request_upload_credentials)
         """
 
     def resolve_alias(self, *, AliasId: str) -> ResolveAliasOutputTypeDef:
         """
-        Retrieves the fleet ID that an alias is currently pointing to.
+        Attempts to retrieve a fleet ID that is associated with an alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.resolve_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#resolve_alias)
         """
 
     def resume_game_server_group(
         self,
         *,
         GameServerGroupName: str,
-        ResumeActions: Sequence[Literal["REPLACE_INSTANCE_TYPES"]]
+        ResumeActions: Sequence[Literal["REPLACE_INSTANCE_TYPES"]],
     ) -> ResumeGameServerGroupOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Reinstates activity on a game server group after it has been
         suspended.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.resume_game_server_group)
@@ -1284,15 +1385,15 @@
         *,
         FleetId: str = ...,
         AliasId: str = ...,
         Location: str = ...,
         FilterExpression: str = ...,
         SortExpression: str = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> SearchGameSessionsOutputTypeDef:
         """
         Retrieves all active game sessions that match a set of search criteria and
         sorts them into a specified
         order.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.search_game_sessions)
@@ -1316,30 +1417,30 @@
         PlacementId: str,
         GameSessionQueueName: str,
         MaximumPlayerSessionCount: int,
         GameProperties: Sequence[GamePropertyTypeDef] = ...,
         GameSessionName: str = ...,
         PlayerLatencies: Sequence[PlayerLatencyTypeDef] = ...,
         DesiredPlayerSessions: Sequence[DesiredPlayerSessionTypeDef] = ...,
-        GameSessionData: str = ...
+        GameSessionData: str = ...,
     ) -> StartGameSessionPlacementOutputTypeDef:
         """
         Places a request for a new game session in a queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.start_game_session_placement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#start_game_session_placement)
         """
 
     def start_match_backfill(
         self,
         *,
         ConfigurationName: str,
         Players: Sequence[PlayerTypeDef],
         TicketId: str = ...,
-        GameSessionArn: str = ...
+        GameSessionArn: str = ...,
     ) -> StartMatchBackfillOutputTypeDef:
         """
         Finds new players to fill open slots in currently running game sessions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.start_match_backfill)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#start_match_backfill)
         """
@@ -1385,15 +1486,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#stop_matchmaking)
         """
 
     def suspend_game_server_group(
         self,
         *,
         GameServerGroupName: str,
-        SuspendActions: Sequence[Literal["REPLACE_INSTANCE_TYPES"]]
+        SuspendActions: Sequence[Literal["REPLACE_INSTANCE_TYPES"]],
     ) -> SuspendGameServerGroupOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Temporarily stops activity on a game server group without
         terminating instances or the game server
         group.
 
@@ -1419,15 +1520,15 @@
 
     def update_alias(
         self,
         *,
         AliasId: str,
         Name: str = ...,
         Description: str = ...,
-        RoutingStrategy: RoutingStrategyTypeDef = ...
+        RoutingStrategy: RoutingStrategyTypeDef = ...,
     ) -> UpdateAliasOutputTypeDef:
         """
         Updates properties for an alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_alias)
         """
@@ -1447,65 +1548,68 @@
         *,
         FleetId: str,
         Name: str = ...,
         Description: str = ...,
         NewGameSessionProtectionPolicy: ProtectionPolicyType = ...,
         ResourceCreationLimitPolicy: ResourceCreationLimitPolicyTypeDef = ...,
         MetricGroups: Sequence[str] = ...,
-        AnywhereConfiguration: AnywhereConfigurationTypeDef = ...
+        AnywhereConfiguration: AnywhereConfigurationTypeDef = ...,
     ) -> UpdateFleetAttributesOutputTypeDef:
         """
-        Updates a fleet's mutable attributes, including game session protection and
+        Updates a fleet's mutable attributes, such as game session protection and
         resource creation
         limits.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_fleet_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_fleet_attributes)
         """
 
     def update_fleet_capacity(
         self,
         *,
         FleetId: str,
         DesiredInstances: int = ...,
         MinSize: int = ...,
         MaxSize: int = ...,
-        Location: str = ...
+        Location: str = ...,
     ) -> UpdateFleetCapacityOutputTypeDef:
         """
-        Updates capacity settings for a fleet.
+        **This operation has been expanded to use with the Amazon GameLift containers
+        feature, which is currently in public preview.** Updates capacity settings for
+        a managed EC2 fleet or container
+        fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_fleet_capacity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_fleet_capacity)
         """
 
     def update_fleet_port_settings(
         self,
         *,
         FleetId: str,
         InboundPermissionAuthorizations: Sequence[IpPermissionTypeDef] = ...,
-        InboundPermissionRevocations: Sequence[IpPermissionTypeDef] = ...
+        InboundPermissionRevocations: Sequence[IpPermissionTypeDef] = ...,
     ) -> UpdateFleetPortSettingsOutputTypeDef:
         """
-        Updates permissions that allow inbound traffic to connect to game sessions that
-        are being hosted on instances in the
+        Updates permissions that allow inbound traffic to connect to game sessions in
+        the
         fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_fleet_port_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_fleet_port_settings)
         """
 
     def update_game_server(
         self,
         *,
         GameServerGroupName: str,
         GameServerId: str,
         GameServerData: str = ...,
         UtilizationStatus: GameServerUtilizationStatusType = ...,
-        HealthCheck: Literal["HEALTHY"] = ...
+        HealthCheck: Literal["HEALTHY"] = ...,
     ) -> UpdateGameServerOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Updates information about a registered game server to help
         Amazon GameLift FleetIQ track game server
         availability.
 
@@ -1516,15 +1620,15 @@
     def update_game_server_group(
         self,
         *,
         GameServerGroupName: str,
         RoleArn: str = ...,
         InstanceDefinitions: Sequence[InstanceDefinitionTypeDef] = ...,
         GameServerProtectionPolicy: GameServerProtectionPolicyType = ...,
-        BalancingStrategy: BalancingStrategyType = ...
+        BalancingStrategy: BalancingStrategyType = ...,
     ) -> UpdateGameServerGroupOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Updates Amazon GameLift FleetIQ-specific properties for a game
         server
         group.
 
@@ -1536,15 +1640,15 @@
         self,
         *,
         GameSessionId: str,
         MaximumPlayerSessionCount: int = ...,
         Name: str = ...,
         PlayerSessionCreationPolicy: PlayerSessionCreationPolicyType = ...,
         ProtectionPolicy: ProtectionPolicyType = ...,
-        GameProperties: Sequence[GamePropertyTypeDef] = ...
+        GameProperties: Sequence[GamePropertyTypeDef] = ...,
     ) -> UpdateGameSessionOutputTypeDef:
         """
         Updates the mutable properties of a game session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_game_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_game_session)
         """
@@ -1555,15 +1659,15 @@
         Name: str,
         TimeoutInSeconds: int = ...,
         PlayerLatencyPolicies: Sequence[PlayerLatencyPolicyTypeDef] = ...,
         Destinations: Sequence[GameSessionQueueDestinationTypeDef] = ...,
         FilterConfiguration: FilterConfigurationTypeDef = ...,
         PriorityConfiguration: PriorityConfigurationTypeDef = ...,
         CustomEventData: str = ...,
-        NotificationTarget: str = ...
+        NotificationTarget: str = ...,
     ) -> UpdateGameSessionQueueOutputTypeDef:
         """
         Updates the configuration of a game session queue, which determines how the
         queue processes new game session
         requests.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_game_session_queue)
@@ -1582,43 +1686,41 @@
         RuleSetName: str = ...,
         NotificationTarget: str = ...,
         AdditionalPlayerCount: int = ...,
         CustomEventData: str = ...,
         GameProperties: Sequence[GamePropertyTypeDef] = ...,
         GameSessionData: str = ...,
         BackfillMode: BackfillModeType = ...,
-        FlexMatchMode: FlexMatchModeType = ...
+        FlexMatchMode: FlexMatchModeType = ...,
     ) -> UpdateMatchmakingConfigurationOutputTypeDef:
         """
         Updates settings for a FlexMatch matchmaking configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_matchmaking_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_matchmaking_configuration)
         """
 
     def update_runtime_configuration(
         self, *, FleetId: str, RuntimeConfiguration: RuntimeConfigurationTypeDef
     ) -> UpdateRuntimeConfigurationOutputTypeDef:
         """
-        Updates the current runtime configuration for the specified fleet, which tells
-        Amazon GameLift how to launch server processes on all instances in the
-        fleet.
+        Updates the runtime configuration for the specified fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_runtime_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_runtime_configuration)
         """
 
     def update_script(
         self,
         *,
         ScriptId: str,
         Name: str = ...,
         Version: str = ...,
         StorageLocation: S3LocationTypeDef = ...,
-        ZipFile: BlobTypeDef = ...
+        ZipFile: BlobTypeDef = ...,
     ) -> UpdateScriptOutputTypeDef:
         """
         Updates Realtime script metadata and content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_script)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_script)
         """
@@ -1768,14 +1870,23 @@
     def get_paginator(self, operation_name: Literal["list_compute"]) -> ListComputePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#get_paginator)
         """
 
     @overload
+    def get_paginator(
+        self, operation_name: Literal["list_container_group_definitions"]
+    ) -> ListContainerGroupDefinitionsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#get_paginator)
+        """
+
+    @overload
     def get_paginator(self, operation_name: Literal["list_fleets"]) -> ListFleetsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#get_paginator)
         """
 
     @overload
```

### Comparing `mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift/client.pyi` & `mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from .literals import (
     AcceptanceTypeType,
     BackfillModeType,
     BalancingStrategyType,
     BuildStatusType,
     ComparisonOperatorTypeType,
     ComputeTypeType,
+    ContainerSchedulingStrategyType,
     EC2InstanceTypeType,
     FleetTypeType,
     FlexMatchModeType,
     GameServerGroupDeleteOptionType,
     GameServerProtectionPolicyType,
     GameServerUtilizationStatusType,
     LocationFilterType,
@@ -56,29 +57,33 @@
     DescribeMatchmakingConfigurationsPaginator,
     DescribeMatchmakingRuleSetsPaginator,
     DescribePlayerSessionsPaginator,
     DescribeScalingPoliciesPaginator,
     ListAliasesPaginator,
     ListBuildsPaginator,
     ListComputePaginator,
+    ListContainerGroupDefinitionsPaginator,
     ListFleetsPaginator,
     ListGameServerGroupsPaginator,
     ListGameServersPaginator,
     ListLocationsPaginator,
     ListScriptsPaginator,
     SearchGameSessionsPaginator,
 )
 from .type_defs import (
     AnywhereConfigurationTypeDef,
     BlobTypeDef,
     CertificateConfigurationTypeDef,
     ClaimFilterOptionTypeDef,
     ClaimGameServerOutputTypeDef,
+    ContainerDefinitionInputTypeDef,
+    ContainerGroupsConfigurationTypeDef,
     CreateAliasOutputTypeDef,
     CreateBuildOutputTypeDef,
+    CreateContainerGroupDefinitionOutputTypeDef,
     CreateFleetLocationsOutputTypeDef,
     CreateFleetOutputTypeDef,
     CreateGameServerGroupOutputTypeDef,
     CreateGameSessionOutputTypeDef,
     CreateGameSessionQueueOutputTypeDef,
     CreateLocationOutputTypeDef,
     CreateMatchmakingConfigurationOutputTypeDef,
@@ -88,14 +93,15 @@
     CreateScriptOutputTypeDef,
     CreateVpcPeeringAuthorizationOutputTypeDef,
     DeleteFleetLocationsOutputTypeDef,
     DeleteGameServerGroupOutputTypeDef,
     DescribeAliasOutputTypeDef,
     DescribeBuildOutputTypeDef,
     DescribeComputeOutputTypeDef,
+    DescribeContainerGroupDefinitionOutputTypeDef,
     DescribeEC2InstanceLimitsOutputTypeDef,
     DescribeFleetAttributesOutputTypeDef,
     DescribeFleetCapacityOutputTypeDef,
     DescribeFleetEventsOutputTypeDef,
     DescribeFleetLocationAttributesOutputTypeDef,
     DescribeFleetLocationCapacityOutputTypeDef,
     DescribeFleetLocationUtilizationOutputTypeDef,
@@ -130,14 +136,15 @@
     GetInstanceAccessOutputTypeDef,
     InstanceDefinitionTypeDef,
     IpPermissionTypeDef,
     LaunchTemplateSpecificationTypeDef,
     ListAliasesOutputTypeDef,
     ListBuildsOutputTypeDef,
     ListComputeOutputTypeDef,
+    ListContainerGroupDefinitionsOutputTypeDef,
     ListFleetsOutputTypeDef,
     ListGameServerGroupsOutputTypeDef,
     ListGameServersOutputTypeDef,
     ListLocationsOutputTypeDef,
     ListScriptsOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     LocationConfigurationTypeDef,
@@ -203,14 +210,15 @@
     IdempotentParameterMismatchException: Type[BotocoreClientError]
     InternalServiceException: Type[BotocoreClientError]
     InvalidFleetStatusException: Type[BotocoreClientError]
     InvalidGameSessionStatusException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
+    NotReadyException: Type[BotocoreClientError]
     OutOfCapacityException: Type[BotocoreClientError]
     TaggingFailedException: Type[BotocoreClientError]
     TerminalRoutingStrategyException: Type[BotocoreClientError]
     UnauthorizedException: Type[BotocoreClientError]
     UnsupportedRegionException: Type[BotocoreClientError]
 
 class GameLiftClient(BaseClient):
@@ -250,15 +258,15 @@
 
     def claim_game_server(
         self,
         *,
         GameServerGroupName: str,
         GameServerId: str = ...,
         GameServerData: str = ...,
-        FilterOption: ClaimFilterOptionTypeDef = ...
+        FilterOption: ClaimFilterOptionTypeDef = ...,
     ) -> ClaimGameServerOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Locates an available game server and temporarily reserves it
         to host gameplay and
         players.
 
@@ -276,15 +284,15 @@
 
     def create_alias(
         self,
         *,
         Name: str,
         RoutingStrategy: RoutingStrategyTypeDef,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAliasOutputTypeDef:
         """
         Creates an alias for a fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#create_alias)
         """
@@ -293,23 +301,45 @@
         self,
         *,
         Name: str = ...,
         Version: str = ...,
         StorageLocation: S3LocationTypeDef = ...,
         OperatingSystem: OperatingSystemType = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ServerSdkVersion: str = ...
+        ServerSdkVersion: str = ...,
     ) -> CreateBuildOutputTypeDef:
         """
         Creates a new Amazon GameLift build resource for your game server binary files.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_build)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#create_build)
         """
 
+    def create_container_group_definition(
+        self,
+        *,
+        Name: str,
+        TotalMemoryLimit: int,
+        TotalCpuLimit: int,
+        ContainerDefinitions: Sequence[ContainerDefinitionInputTypeDef],
+        OperatingSystem: Literal["AMAZON_LINUX_2023"],
+        SchedulingStrategy: ContainerSchedulingStrategyType = ...,
+        Tags: Sequence[TagTypeDef] = ...,
+    ) -> CreateContainerGroupDefinitionOutputTypeDef:
+        """
+        **This operation is used with the Amazon GameLift containers feature, which is
+        currently in public preview.** Creates a `ContainerGroupDefinition` resource
+        that describes a set of containers for hosting your game server with Amazon
+        GameLift managed EC2
+        hosting.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_container_group_definition)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#create_container_group_definition)
+        """
+
     def create_fleet(
         self,
         *,
         Name: str,
         Description: str = ...,
         BuildId: str = ...,
         ScriptId: str = ...,
@@ -327,31 +357,34 @@
         FleetType: FleetTypeType = ...,
         InstanceRoleArn: str = ...,
         CertificateConfiguration: CertificateConfigurationTypeDef = ...,
         Locations: Sequence[LocationConfigurationTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ComputeType: ComputeTypeType = ...,
         AnywhereConfiguration: AnywhereConfigurationTypeDef = ...,
-        InstanceRoleCredentialsProvider: Literal["SHARED_CREDENTIAL_FILE"] = ...
+        InstanceRoleCredentialsProvider: Literal["SHARED_CREDENTIAL_FILE"] = ...,
+        ContainerGroupsConfiguration: ContainerGroupsConfigurationTypeDef = ...,
     ) -> CreateFleetOutputTypeDef:
         """
-        Creates a fleet of Amazon Elastic Compute Cloud (Amazon EC2) instances to host
-        your custom game server or Realtime
-        Servers.
+        **This operation has been expanded to use with the Amazon GameLift containers
+        feature, which is currently in public preview.** Creates a fleet of compute
+        resources to host your game
+        servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_fleet)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#create_fleet)
         """
 
     def create_fleet_locations(
         self, *, FleetId: str, Locations: Sequence[LocationConfigurationTypeDef]
     ) -> CreateFleetLocationsOutputTypeDef:
         """
-        Adds remote locations to a fleet and begins populating the new locations with
-        EC2
+        **This operation has been expanded to use with the Amazon GameLift containers
+        feature, which is currently in public preview.** Adds remote locations to an
+        EC2 or container fleet and begins populating the new locations with
         instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_fleet_locations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#create_fleet_locations)
         """
 
     def create_game_server_group(
@@ -363,15 +396,15 @@
         MaxSize: int,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef,
         InstanceDefinitions: Sequence[InstanceDefinitionTypeDef],
         AutoScalingPolicy: GameServerGroupAutoScalingPolicyTypeDef = ...,
         BalancingStrategy: BalancingStrategyType = ...,
         GameServerProtectionPolicy: GameServerProtectionPolicyType = ...,
         VpcSubnets: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateGameServerGroupOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Creates a Amazon GameLift FleetIQ game server group for
         managing game hosting on a collection of Amazon Elastic Compute Cloud instances
         for game
         hosting.
@@ -388,15 +421,15 @@
         AliasId: str = ...,
         Name: str = ...,
         GameProperties: Sequence[GamePropertyTypeDef] = ...,
         CreatorId: str = ...,
         GameSessionId: str = ...,
         IdempotencyToken: str = ...,
         GameSessionData: str = ...,
-        Location: str = ...
+        Location: str = ...,
     ) -> CreateGameSessionOutputTypeDef:
         """
         Creates a multiplayer game session for players in a specific fleet location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_game_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#create_game_session)
         """
@@ -408,15 +441,15 @@
         TimeoutInSeconds: int = ...,
         PlayerLatencyPolicies: Sequence[PlayerLatencyPolicyTypeDef] = ...,
         Destinations: Sequence[GameSessionQueueDestinationTypeDef] = ...,
         FilterConfiguration: FilterConfigurationTypeDef = ...,
         PriorityConfiguration: PriorityConfigurationTypeDef = ...,
         CustomEventData: str = ...,
         NotificationTarget: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateGameSessionQueueOutputTypeDef:
         """
         Creates a placement queue that processes requests for new game sessions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_game_session_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#create_game_session_queue)
         """
@@ -444,15 +477,15 @@
         NotificationTarget: str = ...,
         AdditionalPlayerCount: int = ...,
         CustomEventData: str = ...,
         GameProperties: Sequence[GamePropertyTypeDef] = ...,
         GameSessionData: str = ...,
         BackfillMode: BackfillModeType = ...,
         FlexMatchMode: FlexMatchModeType = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMatchmakingConfigurationOutputTypeDef:
         """
         Defines a new matchmaking configuration for use with FlexMatch.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_matchmaking_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#create_matchmaking_configuration)
         """
@@ -478,15 +511,15 @@
         """
 
     def create_player_sessions(
         self,
         *,
         GameSessionId: str,
         PlayerIds: Sequence[str],
-        PlayerDataMap: Mapping[str, str] = ...
+        PlayerDataMap: Mapping[str, str] = ...,
     ) -> CreatePlayerSessionsOutputTypeDef:
         """
         Reserves open slots in a game session for a group of players.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_player_sessions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#create_player_sessions)
         """
@@ -494,15 +527,15 @@
     def create_script(
         self,
         *,
         Name: str = ...,
         Version: str = ...,
         StorageLocation: S3LocationTypeDef = ...,
         ZipFile: BlobTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateScriptOutputTypeDef:
         """
         Creates a new script record for your Realtime Servers script.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.create_script)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#create_script)
         """
@@ -544,17 +577,29 @@
         """
         Deletes a build.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.delete_build)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#delete_build)
         """
 
+    def delete_container_group_definition(self, *, Name: str) -> EmptyResponseMetadataTypeDef:
+        """
+        **This operation is used with the Amazon GameLift containers feature, which is
+        currently in public preview.** Deletes a container group definition
+        resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.delete_container_group_definition)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#delete_container_group_definition)
+        """
+
     def delete_fleet(self, *, FleetId: str) -> EmptyResponseMetadataTypeDef:
         """
-        Deletes all resources and information related a fleet.
+        Deletes all resources and information related to a fleet and shuts down any
+        currently running fleet instances, including those in remote
+        locations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.delete_fleet)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#delete_fleet)
         """
 
     def delete_fleet_locations(
         self, *, FleetId: str, Locations: Sequence[str]
@@ -645,15 +690,18 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.delete_vpc_peering_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#delete_vpc_peering_connection)
         """
 
     def deregister_compute(self, *, FleetId: str, ComputeName: str) -> Dict[str, Any]:
         """
-        Removes a compute resource from an Amazon GameLift Anywhere fleet.
+        **This operation has been expanded to use with the Amazon GameLift containers
+        feature, which is currently in public preview.** Removes a compute resource
+        from an Amazon GameLift Anywhere fleet or container
+        fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.deregister_compute)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#deregister_compute)
         """
 
     def deregister_game_server(
         self, *, GameServerGroupName: str, GameServerId: str
@@ -681,20 +729,36 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_build)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_build)
         """
 
     def describe_compute(self, *, FleetId: str, ComputeName: str) -> DescribeComputeOutputTypeDef:
         """
-        Retrieves properties for a compute resource in an Amazon GameLift fleet.
+        **This operation has been expanded to use with the Amazon GameLift containers
+        feature, which is currently in public preview.** Retrieves properties for a
+        compute resource in an Amazon GameLift
+        fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_compute)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_compute)
         """
 
+    def describe_container_group_definition(
+        self, *, Name: str
+    ) -> DescribeContainerGroupDefinitionOutputTypeDef:
+        """
+        **This operation is used with the Amazon GameLift containers feature, which is
+        currently in public preview.** Retrieves the properties of a container group
+        definition, including all container definitions in the
+        group.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_container_group_definition)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_container_group_definition)
+        """
+
     def describe_ec2_instance_limits(
         self, *, EC2InstanceType: EC2InstanceTypeType = ..., Location: str = ...
     ) -> DescribeEC2InstanceLimitsOutputTypeDef:
         """
         Retrieves the instance limits and current utilization for an Amazon Web
         Services Region or
         location.
@@ -703,55 +767,59 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_ec2_instance_limits)
         """
 
     def describe_fleet_attributes(
         self, *, FleetIds: Sequence[str] = ..., Limit: int = ..., NextToken: str = ...
     ) -> DescribeFleetAttributesOutputTypeDef:
         """
-        Retrieves core fleet-wide properties, including the computing hardware and
-        deployment configuration for all instances in the
-        fleet.
+        **This operation has been expanded to use with the Amazon GameLift containers
+        feature, which is currently in public preview.** Retrieves core fleet-wide
+        properties for fleets in an Amazon Web Services
+        Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_fleet_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_fleet_attributes)
         """
 
     def describe_fleet_capacity(
         self, *, FleetIds: Sequence[str] = ..., Limit: int = ..., NextToken: str = ...
     ) -> DescribeFleetCapacityOutputTypeDef:
         """
-        Retrieves the resource capacity settings for one or more fleets.
+        **This operation has been expanded to use with the Amazon GameLift containers
+        feature, which is currently in public preview.** Retrieves the resource
+        capacity settings for one or more
+        fleets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_fleet_capacity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_fleet_capacity)
         """
 
     def describe_fleet_events(
         self,
         *,
         FleetId: str,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeFleetEventsOutputTypeDef:
         """
         Retrieves entries from a fleet's event log.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_fleet_events)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_fleet_events)
         """
 
     def describe_fleet_location_attributes(
         self,
         *,
         FleetId: str,
         Locations: Sequence[str] = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeFleetLocationAttributesOutputTypeDef:
         """
         Retrieves information on a fleet's remote locations, including life-cycle
         status and any suspended fleet
         activity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_fleet_location_attributes)
@@ -824,15 +892,15 @@
 
     def describe_game_server_instances(
         self,
         *,
         GameServerGroupName: str,
         InstanceIds: Sequence[str] = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeGameServerInstancesOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Retrieves status information about the Amazon EC2 instances
         associated with a Amazon GameLift FleetIQ game server
         group.
 
@@ -845,15 +913,15 @@
         *,
         FleetId: str = ...,
         GameSessionId: str = ...,
         AliasId: str = ...,
         Location: str = ...,
         StatusFilter: str = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeGameSessionDetailsOutputTypeDef:
         """
         Retrieves additional game session properties, including the game session
         protection policy in force, a set of one or more game sessions in a specific
         fleet
         location.
 
@@ -887,15 +955,15 @@
         *,
         FleetId: str = ...,
         GameSessionId: str = ...,
         AliasId: str = ...,
         Location: str = ...,
         StatusFilter: str = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeGameSessionsOutputTypeDef:
         """
         Retrieves a set of one or more game sessions in a specific fleet location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_game_sessions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_game_sessions)
         """
@@ -903,15 +971,15 @@
     def describe_instances(
         self,
         *,
         FleetId: str,
         InstanceId: str = ...,
         Limit: int = ...,
         NextToken: str = ...,
-        Location: str = ...
+        Location: str = ...,
     ) -> DescribeInstancesOutputTypeDef:
         """
         Retrieves information about the EC2 instances in an Amazon GameLift managed
         fleet, including instance ID, connection data, and
         status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_instances)
@@ -928,15 +996,15 @@
 
     def describe_matchmaking_configurations(
         self,
         *,
         Names: Sequence[str] = ...,
         RuleSetName: str = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeMatchmakingConfigurationsOutputTypeDef:
         """
         Retrieves the details of FlexMatch matchmaking configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_matchmaking_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_matchmaking_configurations)
         """
@@ -955,15 +1023,15 @@
         self,
         *,
         GameSessionId: str = ...,
         PlayerId: str = ...,
         PlayerSessionId: str = ...,
         PlayerSessionStatusFilter: str = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribePlayerSessionsOutputTypeDef:
         """
         Retrieves properties for one or more player sessions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_player_sessions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_player_sessions)
         """
@@ -981,15 +1049,15 @@
     def describe_scaling_policies(
         self,
         *,
         FleetId: str,
         StatusFilter: ScalingStatusTypeType = ...,
         Limit: int = ...,
         NextToken: str = ...,
-        Location: str = ...
+        Location: str = ...,
     ) -> DescribeScalingPoliciesOutputTypeDef:
         """
         Retrieves all scaling policies applied to a fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.describe_scaling_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#describe_scaling_policies)
         """
@@ -1036,28 +1104,29 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#generate_presigned_url)
         """
 
     def get_compute_access(
         self, *, FleetId: str, ComputeName: str
     ) -> GetComputeAccessOutputTypeDef:
         """
-        Requests authorization to remotely connect to a compute resource in an Amazon
-        GameLift
+        **This operation has been expanded to use with the Amazon GameLift containers
+        feature, which is currently in public preview.** Requests authorization to
+        remotely connect to a hosting resource in a Amazon GameLift managed
         fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.get_compute_access)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#get_compute_access)
         """
 
     def get_compute_auth_token(
         self, *, FleetId: str, ComputeName: str
     ) -> GetComputeAuthTokenOutputTypeDef:
         """
-        Requests an authentication token from Amazon GameLift for a registered compute
-        in an Anywhere
+        Requests an authentication token from Amazon GameLift for a compute resource in
+        an Amazon GameLift Anywhere fleet or container
         fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.get_compute_auth_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#get_compute_auth_token)
         """
 
     def get_game_session_log_url(self, *, GameSessionId: str) -> GetGameSessionLogUrlOutputTypeDef:
@@ -1084,15 +1153,15 @@
 
     def list_aliases(
         self,
         *,
         RoutingStrategyType: RoutingStrategyTypeType = ...,
         Name: str = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAliasesOutputTypeDef:
         """
         Retrieves all aliases for this Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.list_aliases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#list_aliases)
         """
@@ -1109,25 +1178,55 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#list_builds)
         """
 
     def list_compute(
         self, *, FleetId: str, Location: str = ..., Limit: int = ..., NextToken: str = ...
     ) -> ListComputeOutputTypeDef:
         """
-        Retrieves the compute resources in an Amazon GameLift fleet.
+        **This operation has been expanded to use with the Amazon GameLift containers
+        feature, which is currently in public preview.** Retrieves information on the
+        compute resources in an Amazon GameLift
+        fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.list_compute)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#list_compute)
         """
 
+    def list_container_group_definitions(
+        self,
+        *,
+        SchedulingStrategy: ContainerSchedulingStrategyType = ...,
+        Limit: int = ...,
+        NextToken: str = ...,
+    ) -> ListContainerGroupDefinitionsOutputTypeDef:
+        """
+        **This operation is used with the Amazon GameLift containers feature, which is
+        currently in public preview.** Retrieves all container group definitions for
+        the Amazon Web Services account and Amazon Web Services Region that are
+        currently in
+        use.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.list_container_group_definitions)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#list_container_group_definitions)
+        """
+
     def list_fleets(
-        self, *, BuildId: str = ..., ScriptId: str = ..., Limit: int = ..., NextToken: str = ...
+        self,
+        *,
+        BuildId: str = ...,
+        ScriptId: str = ...,
+        ContainerGroupDefinitionName: str = ...,
+        Limit: int = ...,
+        NextToken: str = ...,
     ) -> ListFleetsOutputTypeDef:
         """
-        Retrieves a collection of fleet resources in an Amazon Web Services Region.
+        **This operation has been expanded to use with the Amazon GameLift containers
+        feature, which is currently in public preview.** Retrieves a collection of
+        fleet resources in an Amazon Web Services
+        Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.list_fleets)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#list_fleets)
         """
 
     def list_game_server_groups(
         self, *, Limit: int = ..., NextToken: str = ...
@@ -1141,15 +1240,15 @@
 
     def list_game_servers(
         self,
         *,
         GameServerGroupName: str,
         SortOrder: SortOrderType = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListGameServersOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Retrieves information on all game servers that are currently
         active in a specified game server
         group.
 
@@ -1193,15 +1292,15 @@
         MetricName: MetricNameType,
         ScalingAdjustment: int = ...,
         ScalingAdjustmentType: ScalingAdjustmentTypeType = ...,
         Threshold: float = ...,
         ComparisonOperator: ComparisonOperatorTypeType = ...,
         EvaluationPeriods: int = ...,
         PolicyType: PolicyTypeType = ...,
-        TargetConfiguration: TargetConfigurationTypeDef = ...
+        TargetConfiguration: TargetConfigurationTypeDef = ...,
     ) -> PutScalingPolicyOutputTypeDef:
         """
         Creates or updates a scaling policy for a fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.put_scaling_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#put_scaling_policy)
         """
@@ -1210,31 +1309,34 @@
         self,
         *,
         FleetId: str,
         ComputeName: str,
         CertificatePath: str = ...,
         DnsName: str = ...,
         IpAddress: str = ...,
-        Location: str = ...
+        Location: str = ...,
     ) -> RegisterComputeOutputTypeDef:
         """
-        Registers a compute resource to an Amazon GameLift Anywhere fleet.
+        **This operation has been expanded to use with the Amazon GameLift containers
+        feature, which is currently in public preview.** Registers a compute resource
+        in an Amazon GameLift
+        fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.register_compute)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#register_compute)
         """
 
     def register_game_server(
         self,
         *,
         GameServerGroupName: str,
         GameServerId: str,
         InstanceId: str,
         ConnectionInfo: str = ...,
-        GameServerData: str = ...
+        GameServerData: str = ...,
     ) -> RegisterGameServerOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Creates a new game server resource and notifies Amazon
         GameLift FleetIQ that the game server is ready to host gameplay and
         players.
 
@@ -1250,25 +1352,25 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.request_upload_credentials)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#request_upload_credentials)
         """
 
     def resolve_alias(self, *, AliasId: str) -> ResolveAliasOutputTypeDef:
         """
-        Retrieves the fleet ID that an alias is currently pointing to.
+        Attempts to retrieve a fleet ID that is associated with an alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.resolve_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#resolve_alias)
         """
 
     def resume_game_server_group(
         self,
         *,
         GameServerGroupName: str,
-        ResumeActions: Sequence[Literal["REPLACE_INSTANCE_TYPES"]]
+        ResumeActions: Sequence[Literal["REPLACE_INSTANCE_TYPES"]],
     ) -> ResumeGameServerGroupOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Reinstates activity on a game server group after it has been
         suspended.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.resume_game_server_group)
@@ -1280,15 +1382,15 @@
         *,
         FleetId: str = ...,
         AliasId: str = ...,
         Location: str = ...,
         FilterExpression: str = ...,
         SortExpression: str = ...,
         Limit: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> SearchGameSessionsOutputTypeDef:
         """
         Retrieves all active game sessions that match a set of search criteria and
         sorts them into a specified
         order.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.search_game_sessions)
@@ -1312,30 +1414,30 @@
         PlacementId: str,
         GameSessionQueueName: str,
         MaximumPlayerSessionCount: int,
         GameProperties: Sequence[GamePropertyTypeDef] = ...,
         GameSessionName: str = ...,
         PlayerLatencies: Sequence[PlayerLatencyTypeDef] = ...,
         DesiredPlayerSessions: Sequence[DesiredPlayerSessionTypeDef] = ...,
-        GameSessionData: str = ...
+        GameSessionData: str = ...,
     ) -> StartGameSessionPlacementOutputTypeDef:
         """
         Places a request for a new game session in a queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.start_game_session_placement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#start_game_session_placement)
         """
 
     def start_match_backfill(
         self,
         *,
         ConfigurationName: str,
         Players: Sequence[PlayerTypeDef],
         TicketId: str = ...,
-        GameSessionArn: str = ...
+        GameSessionArn: str = ...,
     ) -> StartMatchBackfillOutputTypeDef:
         """
         Finds new players to fill open slots in currently running game sessions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.start_match_backfill)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#start_match_backfill)
         """
@@ -1381,15 +1483,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#stop_matchmaking)
         """
 
     def suspend_game_server_group(
         self,
         *,
         GameServerGroupName: str,
-        SuspendActions: Sequence[Literal["REPLACE_INSTANCE_TYPES"]]
+        SuspendActions: Sequence[Literal["REPLACE_INSTANCE_TYPES"]],
     ) -> SuspendGameServerGroupOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Temporarily stops activity on a game server group without
         terminating instances or the game server
         group.
 
@@ -1415,15 +1517,15 @@
 
     def update_alias(
         self,
         *,
         AliasId: str,
         Name: str = ...,
         Description: str = ...,
-        RoutingStrategy: RoutingStrategyTypeDef = ...
+        RoutingStrategy: RoutingStrategyTypeDef = ...,
     ) -> UpdateAliasOutputTypeDef:
         """
         Updates properties for an alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_alias)
         """
@@ -1443,65 +1545,68 @@
         *,
         FleetId: str,
         Name: str = ...,
         Description: str = ...,
         NewGameSessionProtectionPolicy: ProtectionPolicyType = ...,
         ResourceCreationLimitPolicy: ResourceCreationLimitPolicyTypeDef = ...,
         MetricGroups: Sequence[str] = ...,
-        AnywhereConfiguration: AnywhereConfigurationTypeDef = ...
+        AnywhereConfiguration: AnywhereConfigurationTypeDef = ...,
     ) -> UpdateFleetAttributesOutputTypeDef:
         """
-        Updates a fleet's mutable attributes, including game session protection and
+        Updates a fleet's mutable attributes, such as game session protection and
         resource creation
         limits.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_fleet_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_fleet_attributes)
         """
 
     def update_fleet_capacity(
         self,
         *,
         FleetId: str,
         DesiredInstances: int = ...,
         MinSize: int = ...,
         MaxSize: int = ...,
-        Location: str = ...
+        Location: str = ...,
     ) -> UpdateFleetCapacityOutputTypeDef:
         """
-        Updates capacity settings for a fleet.
+        **This operation has been expanded to use with the Amazon GameLift containers
+        feature, which is currently in public preview.** Updates capacity settings for
+        a managed EC2 fleet or container
+        fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_fleet_capacity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_fleet_capacity)
         """
 
     def update_fleet_port_settings(
         self,
         *,
         FleetId: str,
         InboundPermissionAuthorizations: Sequence[IpPermissionTypeDef] = ...,
-        InboundPermissionRevocations: Sequence[IpPermissionTypeDef] = ...
+        InboundPermissionRevocations: Sequence[IpPermissionTypeDef] = ...,
     ) -> UpdateFleetPortSettingsOutputTypeDef:
         """
-        Updates permissions that allow inbound traffic to connect to game sessions that
-        are being hosted on instances in the
+        Updates permissions that allow inbound traffic to connect to game sessions in
+        the
         fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_fleet_port_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_fleet_port_settings)
         """
 
     def update_game_server(
         self,
         *,
         GameServerGroupName: str,
         GameServerId: str,
         GameServerData: str = ...,
         UtilizationStatus: GameServerUtilizationStatusType = ...,
-        HealthCheck: Literal["HEALTHY"] = ...
+        HealthCheck: Literal["HEALTHY"] = ...,
     ) -> UpdateGameServerOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Updates information about a registered game server to help
         Amazon GameLift FleetIQ track game server
         availability.
 
@@ -1512,15 +1617,15 @@
     def update_game_server_group(
         self,
         *,
         GameServerGroupName: str,
         RoleArn: str = ...,
         InstanceDefinitions: Sequence[InstanceDefinitionTypeDef] = ...,
         GameServerProtectionPolicy: GameServerProtectionPolicyType = ...,
-        BalancingStrategy: BalancingStrategyType = ...
+        BalancingStrategy: BalancingStrategyType = ...,
     ) -> UpdateGameServerGroupOutputTypeDef:
         """
         **This operation is used with the Amazon GameLift FleetIQ solution and game
         server groups.** Updates Amazon GameLift FleetIQ-specific properties for a game
         server
         group.
 
@@ -1532,15 +1637,15 @@
         self,
         *,
         GameSessionId: str,
         MaximumPlayerSessionCount: int = ...,
         Name: str = ...,
         PlayerSessionCreationPolicy: PlayerSessionCreationPolicyType = ...,
         ProtectionPolicy: ProtectionPolicyType = ...,
-        GameProperties: Sequence[GamePropertyTypeDef] = ...
+        GameProperties: Sequence[GamePropertyTypeDef] = ...,
     ) -> UpdateGameSessionOutputTypeDef:
         """
         Updates the mutable properties of a game session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_game_session)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_game_session)
         """
@@ -1551,15 +1656,15 @@
         Name: str,
         TimeoutInSeconds: int = ...,
         PlayerLatencyPolicies: Sequence[PlayerLatencyPolicyTypeDef] = ...,
         Destinations: Sequence[GameSessionQueueDestinationTypeDef] = ...,
         FilterConfiguration: FilterConfigurationTypeDef = ...,
         PriorityConfiguration: PriorityConfigurationTypeDef = ...,
         CustomEventData: str = ...,
-        NotificationTarget: str = ...
+        NotificationTarget: str = ...,
     ) -> UpdateGameSessionQueueOutputTypeDef:
         """
         Updates the configuration of a game session queue, which determines how the
         queue processes new game session
         requests.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_game_session_queue)
@@ -1578,43 +1683,41 @@
         RuleSetName: str = ...,
         NotificationTarget: str = ...,
         AdditionalPlayerCount: int = ...,
         CustomEventData: str = ...,
         GameProperties: Sequence[GamePropertyTypeDef] = ...,
         GameSessionData: str = ...,
         BackfillMode: BackfillModeType = ...,
-        FlexMatchMode: FlexMatchModeType = ...
+        FlexMatchMode: FlexMatchModeType = ...,
     ) -> UpdateMatchmakingConfigurationOutputTypeDef:
         """
         Updates settings for a FlexMatch matchmaking configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_matchmaking_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_matchmaking_configuration)
         """
 
     def update_runtime_configuration(
         self, *, FleetId: str, RuntimeConfiguration: RuntimeConfigurationTypeDef
     ) -> UpdateRuntimeConfigurationOutputTypeDef:
         """
-        Updates the current runtime configuration for the specified fleet, which tells
-        Amazon GameLift how to launch server processes on all instances in the
-        fleet.
+        Updates the runtime configuration for the specified fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_runtime_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_runtime_configuration)
         """
 
     def update_script(
         self,
         *,
         ScriptId: str,
         Name: str = ...,
         Version: str = ...,
         StorageLocation: S3LocationTypeDef = ...,
-        ZipFile: BlobTypeDef = ...
+        ZipFile: BlobTypeDef = ...,
     ) -> UpdateScriptOutputTypeDef:
         """
         Updates Realtime script metadata and content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.update_script)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#update_script)
         """
@@ -1764,14 +1867,23 @@
     def get_paginator(self, operation_name: Literal["list_compute"]) -> ListComputePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#get_paginator)
         """
 
     @overload
+    def get_paginator(
+        self, operation_name: Literal["list_container_group_definitions"]
+    ) -> ListContainerGroupDefinitionsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#get_paginator)
+        """
+
+    @overload
     def get_paginator(self, operation_name: Literal["list_fleets"]) -> ListFleetsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/client/#get_paginator)
         """
 
     @overload
```

### Comparing `mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift/literals.py` & `mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,24 +15,27 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AcceptanceTypeType",
     "BackfillModeType",
     "BalancingStrategyType",
     "BuildStatusType",
     "CertificateTypeType",
     "ComparisonOperatorTypeType",
     "ComputeStatusType",
     "ComputeTypeType",
+    "ContainerDependencyConditionType",
+    "ContainerGroupDefinitionStatusType",
+    "ContainerOperatingSystemType",
+    "ContainerSchedulingStrategyType",
     "DescribeFleetAttributesPaginatorName",
     "DescribeFleetCapacityPaginatorName",
     "DescribeFleetEventsPaginatorName",
     "DescribeFleetUtilizationPaginatorName",
     "DescribeGameServerInstancesPaginatorName",
     "DescribeGameSessionDetailsPaginatorName",
     "DescribeGameSessionQueuesPaginatorName",
@@ -63,14 +66,15 @@
     "GameSessionStatusType",
     "InstanceRoleCredentialsProviderType",
     "InstanceStatusType",
     "IpProtocolType",
     "ListAliasesPaginatorName",
     "ListBuildsPaginatorName",
     "ListComputePaginatorName",
+    "ListContainerGroupDefinitionsPaginatorName",
     "ListFleetsPaginatorName",
     "ListGameServerGroupsPaginatorName",
     "ListGameServersPaginatorName",
     "ListLocationsPaginatorName",
     "ListScriptsPaginatorName",
     "LocationFilterType",
     "LocationUpdateStatusType",
@@ -90,28 +94,31 @@
     "GameLiftServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AcceptanceTypeType = Literal["ACCEPT", "REJECT"]
 BackfillModeType = Literal["AUTOMATIC", "MANUAL"]
 BalancingStrategyType = Literal["ON_DEMAND_ONLY", "SPOT_ONLY", "SPOT_PREFERRED"]
 BuildStatusType = Literal["FAILED", "INITIALIZED", "READY"]
 CertificateTypeType = Literal["DISABLED", "GENERATED"]
 ComparisonOperatorTypeType = Literal[
     "GreaterThanOrEqualToThreshold",
     "GreaterThanThreshold",
     "LessThanOrEqualToThreshold",
     "LessThanThreshold",
 ]
 ComputeStatusType = Literal["ACTIVE", "PENDING", "TERMINATING"]
-ComputeTypeType = Literal["ANYWHERE", "EC2"]
+ComputeTypeType = Literal["ANYWHERE", "CONTAINER", "EC2"]
+ContainerDependencyConditionType = Literal["COMPLETE", "HEALTHY", "START", "SUCCESS"]
+ContainerGroupDefinitionStatusType = Literal["COPYING", "FAILED", "READY"]
+ContainerOperatingSystemType = Literal["AMAZON_LINUX_2023"]
+ContainerSchedulingStrategyType = Literal["DAEMON", "REPLICA"]
 DescribeFleetAttributesPaginatorName = Literal["describe_fleet_attributes"]
 DescribeFleetCapacityPaginatorName = Literal["describe_fleet_capacity"]
 DescribeFleetEventsPaginatorName = Literal["describe_fleet_events"]
 DescribeFleetUtilizationPaginatorName = Literal["describe_fleet_utilization"]
 DescribeGameServerInstancesPaginatorName = Literal["describe_game_server_instances"]
 DescribeGameSessionDetailsPaginatorName = Literal["describe_game_session_details"]
 DescribeGameSessionQueuesPaginatorName = Literal["describe_game_session_queues"]
@@ -455,14 +462,15 @@
 GameSessionStatusType = Literal["ACTIVATING", "ACTIVE", "ERROR", "TERMINATED", "TERMINATING"]
 InstanceRoleCredentialsProviderType = Literal["SHARED_CREDENTIAL_FILE"]
 InstanceStatusType = Literal["ACTIVE", "PENDING", "TERMINATING"]
 IpProtocolType = Literal["TCP", "UDP"]
 ListAliasesPaginatorName = Literal["list_aliases"]
 ListBuildsPaginatorName = Literal["list_builds"]
 ListComputePaginatorName = Literal["list_compute"]
+ListContainerGroupDefinitionsPaginatorName = Literal["list_container_group_definitions"]
 ListFleetsPaginatorName = Literal["list_fleets"]
 ListGameServerGroupsPaginatorName = Literal["list_game_server_groups"]
 ListGameServersPaginatorName = Literal["list_game_servers"]
 ListLocationsPaginatorName = Literal["list_locations"]
 ListScriptsPaginatorName = Literal["list_scripts"]
 LocationFilterType = Literal["AWS", "CUSTOM"]
 LocationUpdateStatusType = Literal["PENDING_UPDATE"]
@@ -528,14 +536,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -546,14 +555,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -571,14 +581,15 @@
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
@@ -591,24 +602,26 @@
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
@@ -669,15 +682,14 @@
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
@@ -753,14 +765,15 @@
     "mturk",
     "mwaa",
     "neptune",
     "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -805,14 +818,15 @@
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
@@ -850,19 +864,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
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
@@ -908,14 +924,15 @@
     "describe_matchmaking_configurations",
     "describe_matchmaking_rule_sets",
     "describe_player_sessions",
     "describe_scaling_policies",
     "list_aliases",
     "list_builds",
     "list_compute",
+    "list_container_group_definitions",
     "list_fleets",
     "list_game_server_groups",
     "list_game_servers",
     "list_locations",
     "list_scripts",
     "search_game_sessions",
 ]
```

### Comparing `mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift/literals.pyi` & `mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,18 @@
     "BackfillModeType",
     "BalancingStrategyType",
     "BuildStatusType",
     "CertificateTypeType",
     "ComparisonOperatorTypeType",
     "ComputeStatusType",
     "ComputeTypeType",
+    "ContainerDependencyConditionType",
+    "ContainerGroupDefinitionStatusType",
+    "ContainerOperatingSystemType",
+    "ContainerSchedulingStrategyType",
     "DescribeFleetAttributesPaginatorName",
     "DescribeFleetCapacityPaginatorName",
     "DescribeFleetEventsPaginatorName",
     "DescribeFleetUtilizationPaginatorName",
     "DescribeGameServerInstancesPaginatorName",
     "DescribeGameSessionDetailsPaginatorName",
     "DescribeGameSessionQueuesPaginatorName",
@@ -62,14 +66,15 @@
     "GameSessionStatusType",
     "InstanceRoleCredentialsProviderType",
     "InstanceStatusType",
     "IpProtocolType",
     "ListAliasesPaginatorName",
     "ListBuildsPaginatorName",
     "ListComputePaginatorName",
+    "ListContainerGroupDefinitionsPaginatorName",
     "ListFleetsPaginatorName",
     "ListGameServerGroupsPaginatorName",
     "ListGameServersPaginatorName",
     "ListLocationsPaginatorName",
     "ListScriptsPaginatorName",
     "LocationFilterType",
     "LocationUpdateStatusType",
@@ -101,15 +106,19 @@
 ComparisonOperatorTypeType = Literal[
     "GreaterThanOrEqualToThreshold",
     "GreaterThanThreshold",
     "LessThanOrEqualToThreshold",
     "LessThanThreshold",
 ]
 ComputeStatusType = Literal["ACTIVE", "PENDING", "TERMINATING"]
-ComputeTypeType = Literal["ANYWHERE", "EC2"]
+ComputeTypeType = Literal["ANYWHERE", "CONTAINER", "EC2"]
+ContainerDependencyConditionType = Literal["COMPLETE", "HEALTHY", "START", "SUCCESS"]
+ContainerGroupDefinitionStatusType = Literal["COPYING", "FAILED", "READY"]
+ContainerOperatingSystemType = Literal["AMAZON_LINUX_2023"]
+ContainerSchedulingStrategyType = Literal["DAEMON", "REPLICA"]
 DescribeFleetAttributesPaginatorName = Literal["describe_fleet_attributes"]
 DescribeFleetCapacityPaginatorName = Literal["describe_fleet_capacity"]
 DescribeFleetEventsPaginatorName = Literal["describe_fleet_events"]
 DescribeFleetUtilizationPaginatorName = Literal["describe_fleet_utilization"]
 DescribeGameServerInstancesPaginatorName = Literal["describe_game_server_instances"]
 DescribeGameSessionDetailsPaginatorName = Literal["describe_game_session_details"]
 DescribeGameSessionQueuesPaginatorName = Literal["describe_game_session_queues"]
@@ -453,14 +462,15 @@
 GameSessionStatusType = Literal["ACTIVATING", "ACTIVE", "ERROR", "TERMINATED", "TERMINATING"]
 InstanceRoleCredentialsProviderType = Literal["SHARED_CREDENTIAL_FILE"]
 InstanceStatusType = Literal["ACTIVE", "PENDING", "TERMINATING"]
 IpProtocolType = Literal["TCP", "UDP"]
 ListAliasesPaginatorName = Literal["list_aliases"]
 ListBuildsPaginatorName = Literal["list_builds"]
 ListComputePaginatorName = Literal["list_compute"]
+ListContainerGroupDefinitionsPaginatorName = Literal["list_container_group_definitions"]
 ListFleetsPaginatorName = Literal["list_fleets"]
 ListGameServerGroupsPaginatorName = Literal["list_game_server_groups"]
 ListGameServersPaginatorName = Literal["list_game_servers"]
 ListLocationsPaginatorName = Literal["list_locations"]
 ListScriptsPaginatorName = Literal["list_scripts"]
 LocationFilterType = Literal["AWS", "CUSTOM"]
 LocationUpdateStatusType = Literal["PENDING_UPDATE"]
@@ -526,14 +536,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -544,14 +555,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -569,14 +581,15 @@
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
@@ -589,24 +602,26 @@
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
@@ -667,15 +682,14 @@
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
@@ -751,14 +765,15 @@
     "mturk",
     "mwaa",
     "neptune",
     "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -803,14 +818,15 @@
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
@@ -848,19 +864,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
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
@@ -906,14 +924,15 @@
     "describe_matchmaking_configurations",
     "describe_matchmaking_rule_sets",
     "describe_player_sessions",
     "describe_scaling_policies",
     "list_aliases",
     "list_builds",
     "list_compute",
+    "list_container_group_definitions",
     "list_fleets",
     "list_game_server_groups",
     "list_game_servers",
     "list_locations",
     "list_scripts",
     "search_game_sessions",
 ]
```

### Comparing `mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift/paginator.py` & `mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         DescribeMatchmakingConfigurationsPaginator,
         DescribeMatchmakingRuleSetsPaginator,
         DescribePlayerSessionsPaginator,
         DescribeScalingPoliciesPaginator,
         ListAliasesPaginator,
         ListBuildsPaginator,
         ListComputePaginator,
+        ListContainerGroupDefinitionsPaginator,
         ListFleetsPaginator,
         ListGameServerGroupsPaginator,
         ListGameServersPaginator,
         ListLocationsPaginator,
         ListScriptsPaginator,
         SearchGameSessionsPaginator,
     )
@@ -49,14 +50,15 @@
     describe_matchmaking_configurations_paginator: DescribeMatchmakingConfigurationsPaginator = client.get_paginator("describe_matchmaking_configurations")
     describe_matchmaking_rule_sets_paginator: DescribeMatchmakingRuleSetsPaginator = client.get_paginator("describe_matchmaking_rule_sets")
     describe_player_sessions_paginator: DescribePlayerSessionsPaginator = client.get_paginator("describe_player_sessions")
     describe_scaling_policies_paginator: DescribeScalingPoliciesPaginator = client.get_paginator("describe_scaling_policies")
     list_aliases_paginator: ListAliasesPaginator = client.get_paginator("list_aliases")
     list_builds_paginator: ListBuildsPaginator = client.get_paginator("list_builds")
     list_compute_paginator: ListComputePaginator = client.get_paginator("list_compute")
+    list_container_group_definitions_paginator: ListContainerGroupDefinitionsPaginator = client.get_paginator("list_container_group_definitions")
     list_fleets_paginator: ListFleetsPaginator = client.get_paginator("list_fleets")
     list_game_server_groups_paginator: ListGameServerGroupsPaginator = client.get_paginator("list_game_server_groups")
     list_game_servers_paginator: ListGameServersPaginator = client.get_paginator("list_game_servers")
     list_locations_paginator: ListLocationsPaginator = client.get_paginator("list_locations")
     list_scripts_paginator: ListScriptsPaginator = client.get_paginator("list_scripts")
     search_game_sessions_paginator: SearchGameSessionsPaginator = client.get_paginator("search_game_sessions")
     ```
@@ -64,14 +66,15 @@
 
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     BuildStatusType,
+    ContainerSchedulingStrategyType,
     LocationFilterType,
     RoutingStrategyTypeType,
     ScalingStatusTypeType,
     SortOrderType,
 )
 from .type_defs import (
     DescribeFleetAttributesOutputTypeDef,
@@ -86,14 +89,15 @@
     DescribeMatchmakingConfigurationsOutputTypeDef,
     DescribeMatchmakingRuleSetsOutputTypeDef,
     DescribePlayerSessionsOutputTypeDef,
     DescribeScalingPoliciesOutputTypeDef,
     ListAliasesOutputTypeDef,
     ListBuildsOutputTypeDef,
     ListComputeOutputTypeDef,
+    ListContainerGroupDefinitionsOutputPaginatorTypeDef,
     ListFleetsOutputTypeDef,
     ListGameServerGroupsOutputTypeDef,
     ListGameServersOutputTypeDef,
     ListLocationsOutputTypeDef,
     ListScriptsOutputTypeDef,
     PaginatorConfigTypeDef,
     SearchGameSessionsOutputTypeDef,
@@ -113,23 +117,23 @@
     "DescribeMatchmakingConfigurationsPaginator",
     "DescribeMatchmakingRuleSetsPaginator",
     "DescribePlayerSessionsPaginator",
     "DescribeScalingPoliciesPaginator",
     "ListAliasesPaginator",
     "ListBuildsPaginator",
     "ListComputePaginator",
+    "ListContainerGroupDefinitionsPaginator",
     "ListFleetsPaginator",
     "ListGameServerGroupsPaginator",
     "ListGameServersPaginator",
     "ListLocationsPaginator",
     "ListScriptsPaginator",
     "SearchGameSessionsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -174,15 +178,15 @@
 
     def paginate(
         self,
         *,
         FleetId: str,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeFleetEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeFleetEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#describefleeteventspaginator)
         """
 
 
@@ -208,15 +212,15 @@
     """
 
     def paginate(
         self,
         *,
         GameServerGroupName: str,
         InstanceIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeGameServerInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeGameServerInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#describegameserverinstancespaginator)
         """
 
 
@@ -230,15 +234,15 @@
         self,
         *,
         FleetId: str = ...,
         GameSessionId: str = ...,
         AliasId: str = ...,
         Location: str = ...,
         StatusFilter: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeGameSessionDetailsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeGameSessionDetails.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#describegamesessiondetailspaginator)
         """
 
 
@@ -267,15 +271,15 @@
         self,
         *,
         FleetId: str = ...,
         GameSessionId: str = ...,
         AliasId: str = ...,
         Location: str = ...,
         StatusFilter: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeGameSessionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeGameSessions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#describegamesessionspaginator)
         """
 
 
@@ -287,15 +291,15 @@
 
     def paginate(
         self,
         *,
         FleetId: str,
         InstanceId: str = ...,
         Location: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#describeinstancespaginator)
         """
 
 
@@ -306,15 +310,15 @@
     """
 
     def paginate(
         self,
         *,
         Names: Sequence[str] = ...,
         RuleSetName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeMatchmakingConfigurationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeMatchmakingConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#describematchmakingconfigurationspaginator)
         """
 
 
@@ -342,15 +346,15 @@
     def paginate(
         self,
         *,
         GameSessionId: str = ...,
         PlayerId: str = ...,
         PlayerSessionId: str = ...,
         PlayerSessionStatusFilter: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribePlayerSessionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribePlayerSessions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#describeplayersessionspaginator)
         """
 
 
@@ -362,15 +366,15 @@
 
     def paginate(
         self,
         *,
         FleetId: str,
         StatusFilter: ScalingStatusTypeType = ...,
         Location: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeScalingPoliciesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeScalingPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#describescalingpoliciespaginator)
         """
 
 
@@ -381,15 +385,15 @@
     """
 
     def paginate(
         self,
         *,
         RoutingStrategyType: RoutingStrategyTypeType = ...,
         Name: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListAliasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListAliases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#listaliasespaginator)
         """
 
 
@@ -419,26 +423,45 @@
     ) -> _PageIterator[ListComputeOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListCompute.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#listcomputepaginator)
         """
 
 
+class ListContainerGroupDefinitionsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListContainerGroupDefinitions)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#listcontainergroupdefinitionspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        SchedulingStrategy: ContainerSchedulingStrategyType = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[ListContainerGroupDefinitionsOutputPaginatorTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListContainerGroupDefinitions.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#listcontainergroupdefinitionspaginator)
+        """
+
+
 class ListFleetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListFleets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#listfleetspaginator)
     """
 
     def paginate(
         self,
         *,
         BuildId: str = ...,
         ScriptId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        ContainerGroupDefinitionName: str = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListFleetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListFleets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#listfleetspaginator)
         """
 
 
@@ -464,15 +487,15 @@
     """
 
     def paginate(
         self,
         *,
         GameServerGroupName: str,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListGameServersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListGameServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#listgameserverspaginator)
         """
 
 
@@ -482,15 +505,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#listlocationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[LocationFilterType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListLocationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListLocations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#listlocationspaginator)
         """
 
 
@@ -519,13 +542,13 @@
         self,
         *,
         FleetId: str = ...,
         AliasId: str = ...,
         Location: str = ...,
         FilterExpression: str = ...,
         SortExpression: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[SearchGameSessionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.SearchGameSessions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#searchgamesessionspaginator)
         """
```

### Comparing `mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift/paginator.pyi` & `mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         DescribeMatchmakingConfigurationsPaginator,
         DescribeMatchmakingRuleSetsPaginator,
         DescribePlayerSessionsPaginator,
         DescribeScalingPoliciesPaginator,
         ListAliasesPaginator,
         ListBuildsPaginator,
         ListComputePaginator,
+        ListContainerGroupDefinitionsPaginator,
         ListFleetsPaginator,
         ListGameServerGroupsPaginator,
         ListGameServersPaginator,
         ListLocationsPaginator,
         ListScriptsPaginator,
         SearchGameSessionsPaginator,
     )
@@ -49,14 +50,15 @@
     describe_matchmaking_configurations_paginator: DescribeMatchmakingConfigurationsPaginator = client.get_paginator("describe_matchmaking_configurations")
     describe_matchmaking_rule_sets_paginator: DescribeMatchmakingRuleSetsPaginator = client.get_paginator("describe_matchmaking_rule_sets")
     describe_player_sessions_paginator: DescribePlayerSessionsPaginator = client.get_paginator("describe_player_sessions")
     describe_scaling_policies_paginator: DescribeScalingPoliciesPaginator = client.get_paginator("describe_scaling_policies")
     list_aliases_paginator: ListAliasesPaginator = client.get_paginator("list_aliases")
     list_builds_paginator: ListBuildsPaginator = client.get_paginator("list_builds")
     list_compute_paginator: ListComputePaginator = client.get_paginator("list_compute")
+    list_container_group_definitions_paginator: ListContainerGroupDefinitionsPaginator = client.get_paginator("list_container_group_definitions")
     list_fleets_paginator: ListFleetsPaginator = client.get_paginator("list_fleets")
     list_game_server_groups_paginator: ListGameServerGroupsPaginator = client.get_paginator("list_game_server_groups")
     list_game_servers_paginator: ListGameServersPaginator = client.get_paginator("list_game_servers")
     list_locations_paginator: ListLocationsPaginator = client.get_paginator("list_locations")
     list_scripts_paginator: ListScriptsPaginator = client.get_paginator("list_scripts")
     search_game_sessions_paginator: SearchGameSessionsPaginator = client.get_paginator("search_game_sessions")
     ```
@@ -64,14 +66,15 @@
 
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     BuildStatusType,
+    ContainerSchedulingStrategyType,
     LocationFilterType,
     RoutingStrategyTypeType,
     ScalingStatusTypeType,
     SortOrderType,
 )
 from .type_defs import (
     DescribeFleetAttributesOutputTypeDef,
@@ -86,14 +89,15 @@
     DescribeMatchmakingConfigurationsOutputTypeDef,
     DescribeMatchmakingRuleSetsOutputTypeDef,
     DescribePlayerSessionsOutputTypeDef,
     DescribeScalingPoliciesOutputTypeDef,
     ListAliasesOutputTypeDef,
     ListBuildsOutputTypeDef,
     ListComputeOutputTypeDef,
+    ListContainerGroupDefinitionsOutputPaginatorTypeDef,
     ListFleetsOutputTypeDef,
     ListGameServerGroupsOutputTypeDef,
     ListGameServersOutputTypeDef,
     ListLocationsOutputTypeDef,
     ListScriptsOutputTypeDef,
     PaginatorConfigTypeDef,
     SearchGameSessionsOutputTypeDef,
@@ -113,14 +117,15 @@
     "DescribeMatchmakingConfigurationsPaginator",
     "DescribeMatchmakingRuleSetsPaginator",
     "DescribePlayerSessionsPaginator",
     "DescribeScalingPoliciesPaginator",
     "ListAliasesPaginator",
     "ListBuildsPaginator",
     "ListComputePaginator",
+    "ListContainerGroupDefinitionsPaginator",
     "ListFleetsPaginator",
     "ListGameServerGroupsPaginator",
     "ListGameServersPaginator",
     "ListLocationsPaginator",
     "ListScriptsPaginator",
     "SearchGameSessionsPaginator",
 )
@@ -169,15 +174,15 @@
 
     def paginate(
         self,
         *,
         FleetId: str,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeFleetEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeFleetEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#describefleeteventspaginator)
         """
 
 class DescribeFleetUtilizationPaginator(Paginator):
@@ -201,15 +206,15 @@
     """
 
     def paginate(
         self,
         *,
         GameServerGroupName: str,
         InstanceIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeGameServerInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeGameServerInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#describegameserverinstancespaginator)
         """
 
 class DescribeGameSessionDetailsPaginator(Paginator):
@@ -222,15 +227,15 @@
         self,
         *,
         FleetId: str = ...,
         GameSessionId: str = ...,
         AliasId: str = ...,
         Location: str = ...,
         StatusFilter: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeGameSessionDetailsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeGameSessionDetails.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#describegamesessiondetailspaginator)
         """
 
 class DescribeGameSessionQueuesPaginator(Paginator):
@@ -257,15 +262,15 @@
         self,
         *,
         FleetId: str = ...,
         GameSessionId: str = ...,
         AliasId: str = ...,
         Location: str = ...,
         StatusFilter: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeGameSessionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeGameSessions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#describegamesessionspaginator)
         """
 
 class DescribeInstancesPaginator(Paginator):
@@ -276,15 +281,15 @@
 
     def paginate(
         self,
         *,
         FleetId: str,
         InstanceId: str = ...,
         Location: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#describeinstancespaginator)
         """
 
 class DescribeMatchmakingConfigurationsPaginator(Paginator):
@@ -294,15 +299,15 @@
     """
 
     def paginate(
         self,
         *,
         Names: Sequence[str] = ...,
         RuleSetName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeMatchmakingConfigurationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeMatchmakingConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#describematchmakingconfigurationspaginator)
         """
 
 class DescribeMatchmakingRuleSetsPaginator(Paginator):
@@ -328,15 +333,15 @@
     def paginate(
         self,
         *,
         GameSessionId: str = ...,
         PlayerId: str = ...,
         PlayerSessionId: str = ...,
         PlayerSessionStatusFilter: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribePlayerSessionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribePlayerSessions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#describeplayersessionspaginator)
         """
 
 class DescribeScalingPoliciesPaginator(Paginator):
@@ -347,15 +352,15 @@
 
     def paginate(
         self,
         *,
         FleetId: str,
         StatusFilter: ScalingStatusTypeType = ...,
         Location: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeScalingPoliciesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.DescribeScalingPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#describescalingpoliciespaginator)
         """
 
 class ListAliasesPaginator(Paginator):
@@ -365,15 +370,15 @@
     """
 
     def paginate(
         self,
         *,
         RoutingStrategyType: RoutingStrategyTypeType = ...,
         Name: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListAliasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListAliases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#listaliasespaginator)
         """
 
 class ListBuildsPaginator(Paginator):
@@ -400,26 +405,44 @@
         self, *, FleetId: str, Location: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListComputeOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListCompute.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#listcomputepaginator)
         """
 
+class ListContainerGroupDefinitionsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListContainerGroupDefinitions)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#listcontainergroupdefinitionspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        SchedulingStrategy: ContainerSchedulingStrategyType = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[ListContainerGroupDefinitionsOutputPaginatorTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListContainerGroupDefinitions.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#listcontainergroupdefinitionspaginator)
+        """
+
 class ListFleetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListFleets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#listfleetspaginator)
     """
 
     def paginate(
         self,
         *,
         BuildId: str = ...,
         ScriptId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        ContainerGroupDefinitionName: str = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListFleetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListFleets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#listfleetspaginator)
         """
 
 class ListGameServerGroupsPaginator(Paginator):
@@ -443,15 +466,15 @@
     """
 
     def paginate(
         self,
         *,
         GameServerGroupName: str,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListGameServersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListGameServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#listgameserverspaginator)
         """
 
 class ListLocationsPaginator(Paginator):
@@ -460,15 +483,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#listlocationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[LocationFilterType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListLocationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.ListLocations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#listlocationspaginator)
         """
 
 class ListScriptsPaginator(Paginator):
@@ -495,13 +518,13 @@
         self,
         *,
         FleetId: str = ...,
         AliasId: str = ...,
         Location: str = ...,
         FilterExpression: str = ...,
         SortExpression: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[SearchGameSessionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift.Paginator.SearchGameSessions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/paginators/#searchgamesessionspaginator)
         """
```

### Comparing `mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift/type_defs.py` & `mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift/type_defs.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,14 +23,17 @@
     BackfillModeType,
     BalancingStrategyType,
     BuildStatusType,
     CertificateTypeType,
     ComparisonOperatorTypeType,
     ComputeStatusType,
     ComputeTypeType,
+    ContainerDependencyConditionType,
+    ContainerGroupDefinitionStatusType,
+    ContainerSchedulingStrategyType,
     EC2InstanceTypeType,
     EventCodeType,
     FilterInstanceStatusType,
     FleetStatusType,
     FleetTypeType,
     FlexMatchModeType,
     GameServerGroupDeleteOptionType,
@@ -67,28 +70,36 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptMatchInputRequestTypeDef",
     "RoutingStrategyTypeDef",
     "AnywhereConfigurationTypeDef",
     "AttributeValueTypeDef",
     "AwsCredentialsTypeDef",
     "BlobTypeDef",
     "BuildTypeDef",
     "CertificateConfigurationTypeDef",
     "ClaimFilterOptionTypeDef",
     "GameServerTypeDef",
     "ResponseMetadataTypeDef",
-    "ComputeTypeDef",
+    "ConnectionPortRangeTypeDef",
+    "ContainerPortMappingTypeDef",
+    "ContainerDependencyTypeDef",
+    "ContainerEnvironmentTypeDef",
+    "ContainerHealthCheckTypeDef",
+    "ContainerMemoryLimitsTypeDef",
+    "ContainerHealthCheckPaginatorTypeDef",
+    "ContainerGroupDefinitionPropertyTypeDef",
+    "ContainerGroupsPerInstanceTypeDef",
+    "ContainerPortRangeTypeDef",
     "TagTypeDef",
     "S3LocationTypeDef",
     "IpPermissionTypeDef",
     "LocationConfigurationTypeDef",
     "ResourceCreationLimitPolicyTypeDef",
     "LocationStateTypeDef",
     "InstanceDefinitionTypeDef",
@@ -104,14 +115,15 @@
     "PlayerSessionTypeDef",
     "CreatePlayerSessionsInputRequestTypeDef",
     "CreateVpcPeeringAuthorizationInputRequestTypeDef",
     "VpcPeeringAuthorizationTypeDef",
     "CreateVpcPeeringConnectionInputRequestTypeDef",
     "DeleteAliasInputRequestTypeDef",
     "DeleteBuildInputRequestTypeDef",
+    "DeleteContainerGroupDefinitionInputRequestTypeDef",
     "DeleteFleetInputRequestTypeDef",
     "DeleteFleetLocationsInputRequestTypeDef",
     "DeleteGameServerGroupInputRequestTypeDef",
     "DeleteGameSessionQueueInputRequestTypeDef",
     "DeleteLocationInputRequestTypeDef",
     "DeleteMatchmakingConfigurationInputRequestTypeDef",
     "DeleteMatchmakingRuleSetInputRequestTypeDef",
@@ -120,14 +132,15 @@
     "DeleteVpcPeeringAuthorizationInputRequestTypeDef",
     "DeleteVpcPeeringConnectionInputRequestTypeDef",
     "DeregisterComputeInputRequestTypeDef",
     "DeregisterGameServerInputRequestTypeDef",
     "DescribeAliasInputRequestTypeDef",
     "DescribeBuildInputRequestTypeDef",
     "DescribeComputeInputRequestTypeDef",
+    "DescribeContainerGroupDefinitionInputRequestTypeDef",
     "DescribeEC2InstanceLimitsInputRequestTypeDef",
     "EC2InstanceLimitTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeFleetAttributesInputRequestTypeDef",
     "DescribeFleetCapacityInputRequestTypeDef",
     "TimestampTypeDef",
     "EventTypeDef",
@@ -154,27 +167,29 @@
     "DescribeRuntimeConfigurationInputRequestTypeDef",
     "DescribeScalingPoliciesInputRequestTypeDef",
     "DescribeScriptInputRequestTypeDef",
     "DescribeVpcPeeringConnectionsInputRequestTypeDef",
     "DesiredPlayerSessionTypeDef",
     "EC2InstanceCountsTypeDef",
     "FilterConfigurationPaginatorTypeDef",
+    "ReplicaContainerGroupCountsTypeDef",
     "TargetTrackingConfigurationTypeDef",
     "MatchedPlayerSessionTypeDef",
     "PlacedPlayerSessionTypeDef",
     "PlayerLatencyTypeDef",
     "PriorityConfigurationPaginatorTypeDef",
     "GetComputeAccessInputRequestTypeDef",
     "GetComputeAuthTokenInputRequestTypeDef",
     "GetGameSessionLogUrlInputRequestTypeDef",
     "GetInstanceAccessInputRequestTypeDef",
     "InstanceCredentialsTypeDef",
     "ListAliasesInputRequestTypeDef",
     "ListBuildsInputRequestTypeDef",
     "ListComputeInputRequestTypeDef",
+    "ListContainerGroupDefinitionsInputRequestTypeDef",
     "ListFleetsInputRequestTypeDef",
     "ListGameServerGroupsInputRequestTypeDef",
     "ListGameServersInputRequestTypeDef",
     "ListLocationsInputRequestTypeDef",
     "ListScriptsInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TargetConfigurationTypeDef",
@@ -217,32 +232,33 @@
     "StopFleetActionsOutputTypeDef",
     "UpdateBuildOutputTypeDef",
     "UpdateFleetAttributesOutputTypeDef",
     "UpdateFleetCapacityOutputTypeDef",
     "UpdateFleetPortSettingsOutputTypeDef",
     "UpdateGameServerOutputTypeDef",
     "ValidateMatchmakingRuleSetOutputTypeDef",
-    "DescribeComputeOutputTypeDef",
-    "ListComputeOutputTypeDef",
-    "RegisterComputeOutputTypeDef",
+    "ContainerGroupsConfigurationTypeDef",
+    "ContainerAttributesTypeDef",
+    "ContainerGroupsAttributesTypeDef",
+    "ContainerPortConfigurationPaginatorTypeDef",
+    "ContainerPortConfigurationTypeDef",
     "CreateAliasInputRequestTypeDef",
     "CreateLocationInputRequestTypeDef",
     "CreateMatchmakingRuleSetInputRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateBuildInputRequestTypeDef",
     "CreateBuildOutputTypeDef",
     "CreateScriptInputRequestTypeDef",
     "RequestUploadCredentialsOutputTypeDef",
     "ScriptTypeDef",
     "UpdateScriptInputRequestTypeDef",
     "DescribeFleetPortSettingsOutputTypeDef",
     "UpdateFleetPortSettingsInputRequestTypeDef",
     "CreateFleetLocationsInputRequestTypeDef",
-    "FleetAttributesTypeDef",
     "UpdateFleetAttributesInputRequestTypeDef",
     "CreateFleetLocationsOutputTypeDef",
     "DeleteFleetLocationsOutputTypeDef",
     "LocationAttributesTypeDef",
     "GameServerGroupTypeDef",
     "UpdateGameServerGroupInputRequestTypeDef",
     "CreateGameSessionInputRequestTypeDef",
@@ -275,14 +291,15 @@
     "DescribeMatchmakingConfigurationsInputDescribeMatchmakingConfigurationsPaginateTypeDef",
     "DescribeMatchmakingRuleSetsInputDescribeMatchmakingRuleSetsPaginateTypeDef",
     "DescribePlayerSessionsInputDescribePlayerSessionsPaginateTypeDef",
     "DescribeScalingPoliciesInputDescribeScalingPoliciesPaginateTypeDef",
     "ListAliasesInputListAliasesPaginateTypeDef",
     "ListBuildsInputListBuildsPaginateTypeDef",
     "ListComputeInputListComputePaginateTypeDef",
+    "ListContainerGroupDefinitionsInputListContainerGroupDefinitionsPaginateTypeDef",
     "ListFleetsInputListFleetsPaginateTypeDef",
     "ListGameServerGroupsInputListGameServerGroupsPaginateTypeDef",
     "ListGameServersInputListGameServersPaginateTypeDef",
     "ListLocationsInputListLocationsPaginateTypeDef",
     "ListScriptsInputListScriptsPaginateTypeDef",
     "SearchGameSessionsInputSearchGameSessionsPaginateTypeDef",
     "DescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef",
@@ -305,20 +322,23 @@
     "VpcPeeringConnectionTypeDef",
     "CreateAliasOutputTypeDef",
     "DescribeAliasOutputTypeDef",
     "ListAliasesOutputTypeDef",
     "UpdateAliasOutputTypeDef",
     "StartMatchBackfillInputRequestTypeDef",
     "StartMatchmakingInputRequestTypeDef",
+    "ComputeTypeDef",
+    "FleetAttributesTypeDef",
+    "ContainerDefinitionPaginatorTypeDef",
+    "ContainerDefinitionInputTypeDef",
+    "ContainerDefinitionTypeDef",
     "CreateScriptOutputTypeDef",
     "DescribeScriptOutputTypeDef",
     "ListScriptsOutputTypeDef",
     "UpdateScriptOutputTypeDef",
-    "CreateFleetOutputTypeDef",
-    "DescribeFleetAttributesOutputTypeDef",
     "DescribeFleetLocationAttributesOutputTypeDef",
     "CreateGameServerGroupOutputTypeDef",
     "DeleteGameServerGroupOutputTypeDef",
     "DescribeGameServerGroupOutputTypeDef",
     "ListGameServerGroupsOutputTypeDef",
     "ResumeGameServerGroupOutputTypeDef",
     "SuspendGameServerGroupOutputTypeDef",
@@ -345,18 +365,30 @@
     "GetInstanceAccessOutputTypeDef",
     "DescribeScalingPoliciesOutputTypeDef",
     "CreateFleetInputRequestTypeDef",
     "DescribeRuntimeConfigurationOutputTypeDef",
     "UpdateRuntimeConfigurationInputRequestTypeDef",
     "UpdateRuntimeConfigurationOutputTypeDef",
     "DescribeVpcPeeringConnectionsOutputTypeDef",
+    "DescribeComputeOutputTypeDef",
+    "ListComputeOutputTypeDef",
+    "RegisterComputeOutputTypeDef",
+    "CreateFleetOutputTypeDef",
+    "DescribeFleetAttributesOutputTypeDef",
+    "ContainerGroupDefinitionPaginatorTypeDef",
+    "CreateContainerGroupDefinitionInputRequestTypeDef",
+    "ContainerGroupDefinitionTypeDef",
     "DescribeGameSessionDetailsOutputTypeDef",
     "DescribeMatchmakingOutputTypeDef",
     "StartMatchBackfillOutputTypeDef",
     "StartMatchmakingOutputTypeDef",
+    "ListContainerGroupDefinitionsOutputPaginatorTypeDef",
+    "CreateContainerGroupDefinitionOutputTypeDef",
+    "DescribeContainerGroupDefinitionOutputTypeDef",
+    "ListContainerGroupDefinitionsOutputTypeDef",
 )
 
 AcceptMatchInputRequestTypeDef = TypedDict(
     "AcceptMatchInputRequestTypeDef",
     {
         "TicketId": str,
         "PlayerIds": Sequence[str],
@@ -437,35 +469,96 @@
         "LastHealthCheckTime": NotRequired[datetime],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
-ComputeTypeDef = TypedDict(
-    "ComputeTypeDef",
+ConnectionPortRangeTypeDef = TypedDict(
+    "ConnectionPortRangeTypeDef",
     {
-        "FleetId": NotRequired[str],
-        "FleetArn": NotRequired[str],
-        "ComputeName": NotRequired[str],
-        "ComputeArn": NotRequired[str],
-        "IpAddress": NotRequired[str],
-        "DnsName": NotRequired[str],
-        "ComputeStatus": NotRequired[ComputeStatusType],
-        "Location": NotRequired[str],
-        "CreationTime": NotRequired[datetime],
-        "OperatingSystem": NotRequired[OperatingSystemType],
-        "Type": NotRequired[EC2InstanceTypeType],
-        "GameLiftServiceSdkEndpoint": NotRequired[str],
+        "FromPort": int,
+        "ToPort": int,
+    },
+)
+ContainerPortMappingTypeDef = TypedDict(
+    "ContainerPortMappingTypeDef",
+    {
+        "ContainerPort": NotRequired[int],
+        "ConnectionPort": NotRequired[int],
+        "Protocol": NotRequired[IpProtocolType],
+    },
+)
+ContainerDependencyTypeDef = TypedDict(
+    "ContainerDependencyTypeDef",
+    {
+        "ContainerName": str,
+        "Condition": ContainerDependencyConditionType,
+    },
+)
+ContainerEnvironmentTypeDef = TypedDict(
+    "ContainerEnvironmentTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
+)
+ContainerHealthCheckTypeDef = TypedDict(
+    "ContainerHealthCheckTypeDef",
+    {
+        "Command": Sequence[str],
+        "Interval": NotRequired[int],
+        "Timeout": NotRequired[int],
+        "Retries": NotRequired[int],
+        "StartPeriod": NotRequired[int],
+    },
+)
+ContainerMemoryLimitsTypeDef = TypedDict(
+    "ContainerMemoryLimitsTypeDef",
+    {
+        "SoftLimit": NotRequired[int],
+        "HardLimit": NotRequired[int],
+    },
+)
+ContainerHealthCheckPaginatorTypeDef = TypedDict(
+    "ContainerHealthCheckPaginatorTypeDef",
+    {
+        "Command": List[str],
+        "Interval": NotRequired[int],
+        "Timeout": NotRequired[int],
+        "Retries": NotRequired[int],
+        "StartPeriod": NotRequired[int],
+    },
+)
+ContainerGroupDefinitionPropertyTypeDef = TypedDict(
+    "ContainerGroupDefinitionPropertyTypeDef",
+    {
+        "SchedulingStrategy": NotRequired[ContainerSchedulingStrategyType],
+        "ContainerGroupDefinitionName": NotRequired[str],
+    },
+)
+ContainerGroupsPerInstanceTypeDef = TypedDict(
+    "ContainerGroupsPerInstanceTypeDef",
+    {
+        "DesiredReplicaContainerGroupsPerInstance": NotRequired[int],
+        "MaxReplicaContainerGroupsPerInstance": NotRequired[int],
+    },
+)
+ContainerPortRangeTypeDef = TypedDict(
+    "ContainerPortRangeTypeDef",
+    {
+        "FromPort": int,
+        "ToPort": int,
+        "Protocol": IpProtocolType,
     },
 )
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -639,14 +732,20 @@
 )
 DeleteBuildInputRequestTypeDef = TypedDict(
     "DeleteBuildInputRequestTypeDef",
     {
         "BuildId": str,
     },
 )
+DeleteContainerGroupDefinitionInputRequestTypeDef = TypedDict(
+    "DeleteContainerGroupDefinitionInputRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
 DeleteFleetInputRequestTypeDef = TypedDict(
     "DeleteFleetInputRequestTypeDef",
     {
         "FleetId": str,
     },
 )
 DeleteFleetLocationsInputRequestTypeDef = TypedDict(
@@ -743,14 +842,20 @@
 DescribeComputeInputRequestTypeDef = TypedDict(
     "DescribeComputeInputRequestTypeDef",
     {
         "FleetId": str,
         "ComputeName": str,
     },
 )
+DescribeContainerGroupDefinitionInputRequestTypeDef = TypedDict(
+    "DescribeContainerGroupDefinitionInputRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
 DescribeEC2InstanceLimitsInputRequestTypeDef = TypedDict(
     "DescribeEC2InstanceLimitsInputRequestTypeDef",
     {
         "EC2InstanceType": NotRequired[EC2InstanceTypeType],
         "Location": NotRequired[str],
     },
 )
@@ -793,14 +898,15 @@
     {
         "EventId": NotRequired[str],
         "ResourceId": NotRequired[str],
         "EventCode": NotRequired[EventCodeType],
         "Message": NotRequired[str],
         "EventTime": NotRequired[datetime],
         "PreSignedLogUrl": NotRequired[str],
+        "Count": NotRequired[int],
     },
 )
 DescribeFleetLocationAttributesInputRequestTypeDef = TypedDict(
     "DescribeFleetLocationAttributesInputRequestTypeDef",
     {
         "FleetId": str,
         "Locations": NotRequired[Sequence[str]],
@@ -1026,14 +1132,23 @@
 )
 FilterConfigurationPaginatorTypeDef = TypedDict(
     "FilterConfigurationPaginatorTypeDef",
     {
         "AllowedLocations": NotRequired[List[str]],
     },
 )
+ReplicaContainerGroupCountsTypeDef = TypedDict(
+    "ReplicaContainerGroupCountsTypeDef",
+    {
+        "PENDING": NotRequired[int],
+        "ACTIVE": NotRequired[int],
+        "IDLE": NotRequired[int],
+        "TERMINATING": NotRequired[int],
+    },
+)
 TargetTrackingConfigurationTypeDef = TypedDict(
     "TargetTrackingConfigurationTypeDef",
     {
         "TargetValue": float,
     },
 )
 MatchedPlayerSessionTypeDef = TypedDict(
@@ -1121,19 +1236,28 @@
     {
         "FleetId": str,
         "Location": NotRequired[str],
         "Limit": NotRequired[int],
         "NextToken": NotRequired[str],
     },
 )
+ListContainerGroupDefinitionsInputRequestTypeDef = TypedDict(
+    "ListContainerGroupDefinitionsInputRequestTypeDef",
+    {
+        "SchedulingStrategy": NotRequired[ContainerSchedulingStrategyType],
+        "Limit": NotRequired[int],
+        "NextToken": NotRequired[str],
+    },
+)
 ListFleetsInputRequestTypeDef = TypedDict(
     "ListFleetsInputRequestTypeDef",
     {
         "BuildId": NotRequired[str],
         "ScriptId": NotRequired[str],
+        "ContainerGroupDefinitionName": NotRequired[str],
         "Limit": NotRequired[int],
         "NextToken": NotRequired[str],
     },
 )
 ListGameServerGroupsInputRequestTypeDef = TypedDict(
     "ListGameServerGroupsInputRequestTypeDef",
     {
@@ -1390,14 +1514,15 @@
     "GetComputeAccessOutputTypeDef",
     {
         "FleetId": str,
         "FleetArn": str,
         "ComputeName": str,
         "ComputeArn": str,
         "Credentials": AwsCredentialsTypeDef,
+        "Target": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetComputeAuthTokenOutputTypeDef = TypedDict(
     "GetComputeAuthTokenOutputTypeDef",
     {
         "FleetId": str,
@@ -1520,34 +1645,48 @@
 ValidateMatchmakingRuleSetOutputTypeDef = TypedDict(
     "ValidateMatchmakingRuleSetOutputTypeDef",
     {
         "Valid": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-DescribeComputeOutputTypeDef = TypedDict(
-    "DescribeComputeOutputTypeDef",
+ContainerGroupsConfigurationTypeDef = TypedDict(
+    "ContainerGroupsConfigurationTypeDef",
     {
-        "Compute": ComputeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ContainerGroupDefinitionNames": Sequence[str],
+        "ConnectionPortRange": ConnectionPortRangeTypeDef,
+        "DesiredReplicaContainerGroupsPerInstance": NotRequired[int],
     },
 )
-ListComputeOutputTypeDef = TypedDict(
-    "ListComputeOutputTypeDef",
+ContainerAttributesTypeDef = TypedDict(
+    "ContainerAttributesTypeDef",
     {
-        "ComputeList": List[ComputeTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ContainerPortMappings": NotRequired[List[ContainerPortMappingTypeDef]],
     },
 )
-RegisterComputeOutputTypeDef = TypedDict(
-    "RegisterComputeOutputTypeDef",
+ContainerGroupsAttributesTypeDef = TypedDict(
+    "ContainerGroupsAttributesTypeDef",
     {
-        "Compute": ComputeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ContainerGroupDefinitionProperties": NotRequired[
+            List[ContainerGroupDefinitionPropertyTypeDef]
+        ],
+        "ConnectionPortRange": NotRequired[ConnectionPortRangeTypeDef],
+        "ContainerGroupsPerInstance": NotRequired[ContainerGroupsPerInstanceTypeDef],
+    },
+)
+ContainerPortConfigurationPaginatorTypeDef = TypedDict(
+    "ContainerPortConfigurationPaginatorTypeDef",
+    {
+        "ContainerPortRanges": List[ContainerPortRangeTypeDef],
+    },
+)
+ContainerPortConfigurationTypeDef = TypedDict(
+    "ContainerPortConfigurationTypeDef",
+    {
+        "ContainerPortRanges": Sequence[ContainerPortRangeTypeDef],
     },
 )
 CreateAliasInputRequestTypeDef = TypedDict(
     "CreateAliasInputRequestTypeDef",
     {
         "Name": str,
         "RoutingStrategy": RoutingStrategyTypeDef,
@@ -1666,45 +1805,14 @@
 CreateFleetLocationsInputRequestTypeDef = TypedDict(
     "CreateFleetLocationsInputRequestTypeDef",
     {
         "FleetId": str,
         "Locations": Sequence[LocationConfigurationTypeDef],
     },
 )
-FleetAttributesTypeDef = TypedDict(
-    "FleetAttributesTypeDef",
-    {
-        "FleetId": NotRequired[str],
-        "FleetArn": NotRequired[str],
-        "FleetType": NotRequired[FleetTypeType],
-        "InstanceType": NotRequired[EC2InstanceTypeType],
-        "Description": NotRequired[str],
-        "Name": NotRequired[str],
-        "CreationTime": NotRequired[datetime],
-        "TerminationTime": NotRequired[datetime],
-        "Status": NotRequired[FleetStatusType],
-        "BuildId": NotRequired[str],
-        "BuildArn": NotRequired[str],
-        "ScriptId": NotRequired[str],
-        "ScriptArn": NotRequired[str],
-        "ServerLaunchPath": NotRequired[str],
-        "ServerLaunchParameters": NotRequired[str],
-        "LogPaths": NotRequired[List[str]],
-        "NewGameSessionProtectionPolicy": NotRequired[ProtectionPolicyType],
-        "OperatingSystem": NotRequired[OperatingSystemType],
-        "ResourceCreationLimitPolicy": NotRequired[ResourceCreationLimitPolicyTypeDef],
-        "MetricGroups": NotRequired[List[str]],
-        "StoppedActions": NotRequired[List[Literal["AUTO_SCALING"]]],
-        "InstanceRoleArn": NotRequired[str],
-        "CertificateConfiguration": NotRequired[CertificateConfigurationTypeDef],
-        "ComputeType": NotRequired[ComputeTypeType],
-        "AnywhereConfiguration": NotRequired[AnywhereConfigurationTypeDef],
-        "InstanceRoleCredentialsProvider": NotRequired[Literal["SHARED_CREDENTIAL_FILE"]],
-    },
-)
 UpdateFleetAttributesInputRequestTypeDef = TypedDict(
     "UpdateFleetAttributesInputRequestTypeDef",
     {
         "FleetId": str,
         "Name": NotRequired[str],
         "Description": NotRequired[str],
         "NewGameSessionProtectionPolicy": NotRequired[ProtectionPolicyType],
@@ -2111,19 +2219,27 @@
     "ListComputeInputListComputePaginateTypeDef",
     {
         "FleetId": str,
         "Location": NotRequired[str],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+ListContainerGroupDefinitionsInputListContainerGroupDefinitionsPaginateTypeDef = TypedDict(
+    "ListContainerGroupDefinitionsInputListContainerGroupDefinitionsPaginateTypeDef",
+    {
+        "SchedulingStrategy": NotRequired[ContainerSchedulingStrategyType],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
 ListFleetsInputListFleetsPaginateTypeDef = TypedDict(
     "ListFleetsInputListFleetsPaginateTypeDef",
     {
         "BuildId": NotRequired[str],
         "ScriptId": NotRequired[str],
+        "ContainerGroupDefinitionName": NotRequired[str],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListGameServerGroupsInputListGameServerGroupsPaginateTypeDef = TypedDict(
     "ListGameServerGroupsInputListGameServerGroupsPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
@@ -2223,14 +2339,15 @@
     "FleetCapacityTypeDef",
     {
         "FleetId": NotRequired[str],
         "FleetArn": NotRequired[str],
         "InstanceType": NotRequired[EC2InstanceTypeType],
         "InstanceCounts": NotRequired[EC2InstanceCountsTypeDef],
         "Location": NotRequired[str],
+        "ReplicaContainerGroupCounts": NotRequired[ReplicaContainerGroupCountsTypeDef],
     },
 )
 GameServerGroupAutoScalingPolicyTypeDef = TypedDict(
     "GameServerGroupAutoScalingPolicyTypeDef",
     {
         "TargetTrackingConfiguration": TargetTrackingConfigurationTypeDef,
         "EstimatedInstanceWarmup": NotRequired[int],
@@ -2402,14 +2519,119 @@
     "StartMatchmakingInputRequestTypeDef",
     {
         "ConfigurationName": str,
         "Players": Sequence[PlayerTypeDef],
         "TicketId": NotRequired[str],
     },
 )
+ComputeTypeDef = TypedDict(
+    "ComputeTypeDef",
+    {
+        "FleetId": NotRequired[str],
+        "FleetArn": NotRequired[str],
+        "ComputeName": NotRequired[str],
+        "ComputeArn": NotRequired[str],
+        "IpAddress": NotRequired[str],
+        "DnsName": NotRequired[str],
+        "ComputeStatus": NotRequired[ComputeStatusType],
+        "Location": NotRequired[str],
+        "CreationTime": NotRequired[datetime],
+        "OperatingSystem": NotRequired[OperatingSystemType],
+        "Type": NotRequired[EC2InstanceTypeType],
+        "GameLiftServiceSdkEndpoint": NotRequired[str],
+        "GameLiftAgentEndpoint": NotRequired[str],
+        "InstanceId": NotRequired[str],
+        "ContainerAttributes": NotRequired[ContainerAttributesTypeDef],
+    },
+)
+FleetAttributesTypeDef = TypedDict(
+    "FleetAttributesTypeDef",
+    {
+        "FleetId": NotRequired[str],
+        "FleetArn": NotRequired[str],
+        "FleetType": NotRequired[FleetTypeType],
+        "InstanceType": NotRequired[EC2InstanceTypeType],
+        "Description": NotRequired[str],
+        "Name": NotRequired[str],
+        "CreationTime": NotRequired[datetime],
+        "TerminationTime": NotRequired[datetime],
+        "Status": NotRequired[FleetStatusType],
+        "BuildId": NotRequired[str],
+        "BuildArn": NotRequired[str],
+        "ScriptId": NotRequired[str],
+        "ScriptArn": NotRequired[str],
+        "ServerLaunchPath": NotRequired[str],
+        "ServerLaunchParameters": NotRequired[str],
+        "LogPaths": NotRequired[List[str]],
+        "NewGameSessionProtectionPolicy": NotRequired[ProtectionPolicyType],
+        "OperatingSystem": NotRequired[OperatingSystemType],
+        "ResourceCreationLimitPolicy": NotRequired[ResourceCreationLimitPolicyTypeDef],
+        "MetricGroups": NotRequired[List[str]],
+        "StoppedActions": NotRequired[List[Literal["AUTO_SCALING"]]],
+        "InstanceRoleArn": NotRequired[str],
+        "CertificateConfiguration": NotRequired[CertificateConfigurationTypeDef],
+        "ComputeType": NotRequired[ComputeTypeType],
+        "AnywhereConfiguration": NotRequired[AnywhereConfigurationTypeDef],
+        "InstanceRoleCredentialsProvider": NotRequired[Literal["SHARED_CREDENTIAL_FILE"]],
+        "ContainerGroupsAttributes": NotRequired[ContainerGroupsAttributesTypeDef],
+    },
+)
+ContainerDefinitionPaginatorTypeDef = TypedDict(
+    "ContainerDefinitionPaginatorTypeDef",
+    {
+        "ContainerName": str,
+        "ImageUri": str,
+        "ResolvedImageDigest": NotRequired[str],
+        "MemoryLimits": NotRequired[ContainerMemoryLimitsTypeDef],
+        "PortConfiguration": NotRequired[ContainerPortConfigurationPaginatorTypeDef],
+        "Cpu": NotRequired[int],
+        "HealthCheck": NotRequired[ContainerHealthCheckPaginatorTypeDef],
+        "Command": NotRequired[List[str]],
+        "Essential": NotRequired[bool],
+        "EntryPoint": NotRequired[List[str]],
+        "WorkingDirectory": NotRequired[str],
+        "Environment": NotRequired[List[ContainerEnvironmentTypeDef]],
+        "DependsOn": NotRequired[List[ContainerDependencyTypeDef]],
+    },
+)
+ContainerDefinitionInputTypeDef = TypedDict(
+    "ContainerDefinitionInputTypeDef",
+    {
+        "ContainerName": str,
+        "ImageUri": str,
+        "MemoryLimits": NotRequired[ContainerMemoryLimitsTypeDef],
+        "PortConfiguration": NotRequired[ContainerPortConfigurationTypeDef],
+        "Cpu": NotRequired[int],
+        "HealthCheck": NotRequired[ContainerHealthCheckTypeDef],
+        "Command": NotRequired[Sequence[str]],
+        "Essential": NotRequired[bool],
+        "EntryPoint": NotRequired[Sequence[str]],
+        "WorkingDirectory": NotRequired[str],
+        "Environment": NotRequired[Sequence[ContainerEnvironmentTypeDef]],
+        "DependsOn": NotRequired[Sequence[ContainerDependencyTypeDef]],
+    },
+)
+ContainerDefinitionTypeDef = TypedDict(
+    "ContainerDefinitionTypeDef",
+    {
+        "ContainerName": str,
+        "ImageUri": str,
+        "ResolvedImageDigest": NotRequired[str],
+        "MemoryLimits": NotRequired[ContainerMemoryLimitsTypeDef],
+        "PortConfiguration": NotRequired[ContainerPortConfigurationTypeDef],
+        "Cpu": NotRequired[int],
+        "HealthCheck": NotRequired[ContainerHealthCheckTypeDef],
+        "Command": NotRequired[List[str]],
+        "Essential": NotRequired[bool],
+        "EntryPoint": NotRequired[List[str]],
+        "WorkingDirectory": NotRequired[str],
+        "Environment": NotRequired[List[ContainerEnvironmentTypeDef]],
+        "DependsOn": NotRequired[List[ContainerDependencyTypeDef]],
+    },
+)
 CreateScriptOutputTypeDef = TypedDict(
     "CreateScriptOutputTypeDef",
     {
         "Script": ScriptTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2431,30 +2653,14 @@
 UpdateScriptOutputTypeDef = TypedDict(
     "UpdateScriptOutputTypeDef",
     {
         "Script": ScriptTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CreateFleetOutputTypeDef = TypedDict(
-    "CreateFleetOutputTypeDef",
-    {
-        "FleetAttributes": FleetAttributesTypeDef,
-        "LocationStates": List[LocationStateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeFleetAttributesOutputTypeDef = TypedDict(
-    "DescribeFleetAttributesOutputTypeDef",
-    {
-        "FleetAttributes": List[FleetAttributesTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 DescribeFleetLocationAttributesOutputTypeDef = TypedDict(
     "DescribeFleetLocationAttributesOutputTypeDef",
     {
         "FleetId": str,
         "FleetArn": str,
         "LocationAttributes": List[LocationAttributesTypeDef],
         "NextToken": str,
@@ -2705,14 +2911,15 @@
         "InstanceRoleArn": NotRequired[str],
         "CertificateConfiguration": NotRequired[CertificateConfigurationTypeDef],
         "Locations": NotRequired[Sequence[LocationConfigurationTypeDef]],
         "Tags": NotRequired[Sequence[TagTypeDef]],
         "ComputeType": NotRequired[ComputeTypeType],
         "AnywhereConfiguration": NotRequired[AnywhereConfigurationTypeDef],
         "InstanceRoleCredentialsProvider": NotRequired[Literal["SHARED_CREDENTIAL_FILE"]],
+        "ContainerGroupsConfiguration": NotRequired[ContainerGroupsConfigurationTypeDef],
     },
 )
 DescribeRuntimeConfigurationOutputTypeDef = TypedDict(
     "DescribeRuntimeConfigurationOutputTypeDef",
     {
         "RuntimeConfiguration": RuntimeConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2735,14 +2942,94 @@
 DescribeVpcPeeringConnectionsOutputTypeDef = TypedDict(
     "DescribeVpcPeeringConnectionsOutputTypeDef",
     {
         "VpcPeeringConnections": List[VpcPeeringConnectionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DescribeComputeOutputTypeDef = TypedDict(
+    "DescribeComputeOutputTypeDef",
+    {
+        "Compute": ComputeTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ListComputeOutputTypeDef = TypedDict(
+    "ListComputeOutputTypeDef",
+    {
+        "ComputeList": List[ComputeTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+RegisterComputeOutputTypeDef = TypedDict(
+    "RegisterComputeOutputTypeDef",
+    {
+        "Compute": ComputeTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+CreateFleetOutputTypeDef = TypedDict(
+    "CreateFleetOutputTypeDef",
+    {
+        "FleetAttributes": FleetAttributesTypeDef,
+        "LocationStates": List[LocationStateTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DescribeFleetAttributesOutputTypeDef = TypedDict(
+    "DescribeFleetAttributesOutputTypeDef",
+    {
+        "FleetAttributes": List[FleetAttributesTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ContainerGroupDefinitionPaginatorTypeDef = TypedDict(
+    "ContainerGroupDefinitionPaginatorTypeDef",
+    {
+        "ContainerGroupDefinitionArn": NotRequired[str],
+        "CreationTime": NotRequired[datetime],
+        "OperatingSystem": NotRequired[Literal["AMAZON_LINUX_2023"]],
+        "Name": NotRequired[str],
+        "SchedulingStrategy": NotRequired[ContainerSchedulingStrategyType],
+        "TotalMemoryLimit": NotRequired[int],
+        "TotalCpuLimit": NotRequired[int],
+        "ContainerDefinitions": NotRequired[List[ContainerDefinitionPaginatorTypeDef]],
+        "Status": NotRequired[ContainerGroupDefinitionStatusType],
+        "StatusReason": NotRequired[str],
+    },
+)
+CreateContainerGroupDefinitionInputRequestTypeDef = TypedDict(
+    "CreateContainerGroupDefinitionInputRequestTypeDef",
+    {
+        "Name": str,
+        "TotalMemoryLimit": int,
+        "TotalCpuLimit": int,
+        "ContainerDefinitions": Sequence[ContainerDefinitionInputTypeDef],
+        "OperatingSystem": Literal["AMAZON_LINUX_2023"],
+        "SchedulingStrategy": NotRequired[ContainerSchedulingStrategyType],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+    },
+)
+ContainerGroupDefinitionTypeDef = TypedDict(
+    "ContainerGroupDefinitionTypeDef",
+    {
+        "ContainerGroupDefinitionArn": NotRequired[str],
+        "CreationTime": NotRequired[datetime],
+        "OperatingSystem": NotRequired[Literal["AMAZON_LINUX_2023"]],
+        "Name": NotRequired[str],
+        "SchedulingStrategy": NotRequired[ContainerSchedulingStrategyType],
+        "TotalMemoryLimit": NotRequired[int],
+        "TotalCpuLimit": NotRequired[int],
+        "ContainerDefinitions": NotRequired[List[ContainerDefinitionTypeDef]],
+        "Status": NotRequired[ContainerGroupDefinitionStatusType],
+        "StatusReason": NotRequired[str],
+    },
+)
 DescribeGameSessionDetailsOutputTypeDef = TypedDict(
     "DescribeGameSessionDetailsOutputTypeDef",
     {
         "GameSessionDetails": List[GameSessionDetailTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2764,7 +3051,37 @@
 StartMatchmakingOutputTypeDef = TypedDict(
     "StartMatchmakingOutputTypeDef",
     {
         "MatchmakingTicket": MatchmakingTicketTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ListContainerGroupDefinitionsOutputPaginatorTypeDef = TypedDict(
+    "ListContainerGroupDefinitionsOutputPaginatorTypeDef",
+    {
+        "ContainerGroupDefinitions": List[ContainerGroupDefinitionPaginatorTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+CreateContainerGroupDefinitionOutputTypeDef = TypedDict(
+    "CreateContainerGroupDefinitionOutputTypeDef",
+    {
+        "ContainerGroupDefinition": ContainerGroupDefinitionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DescribeContainerGroupDefinitionOutputTypeDef = TypedDict(
+    "DescribeContainerGroupDefinitionOutputTypeDef",
+    {
+        "ContainerGroupDefinition": ContainerGroupDefinitionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ListContainerGroupDefinitionsOutputTypeDef = TypedDict(
+    "ListContainerGroupDefinitionsOutputTypeDef",
+    {
+        "ContainerGroupDefinitions": List[ContainerGroupDefinitionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift/type_defs.pyi` & `mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift/type_defs.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -23,14 +23,17 @@
     BackfillModeType,
     BalancingStrategyType,
     BuildStatusType,
     CertificateTypeType,
     ComparisonOperatorTypeType,
     ComputeStatusType,
     ComputeTypeType,
+    ContainerDependencyConditionType,
+    ContainerGroupDefinitionStatusType,
+    ContainerSchedulingStrategyType,
     EC2InstanceTypeType,
     EventCodeType,
     FilterInstanceStatusType,
     FleetStatusType,
     FleetTypeType,
     FlexMatchModeType,
     GameServerGroupDeleteOptionType,
@@ -79,15 +82,24 @@
     "AwsCredentialsTypeDef",
     "BlobTypeDef",
     "BuildTypeDef",
     "CertificateConfigurationTypeDef",
     "ClaimFilterOptionTypeDef",
     "GameServerTypeDef",
     "ResponseMetadataTypeDef",
-    "ComputeTypeDef",
+    "ConnectionPortRangeTypeDef",
+    "ContainerPortMappingTypeDef",
+    "ContainerDependencyTypeDef",
+    "ContainerEnvironmentTypeDef",
+    "ContainerHealthCheckTypeDef",
+    "ContainerMemoryLimitsTypeDef",
+    "ContainerHealthCheckPaginatorTypeDef",
+    "ContainerGroupDefinitionPropertyTypeDef",
+    "ContainerGroupsPerInstanceTypeDef",
+    "ContainerPortRangeTypeDef",
     "TagTypeDef",
     "S3LocationTypeDef",
     "IpPermissionTypeDef",
     "LocationConfigurationTypeDef",
     "ResourceCreationLimitPolicyTypeDef",
     "LocationStateTypeDef",
     "InstanceDefinitionTypeDef",
@@ -103,14 +115,15 @@
     "PlayerSessionTypeDef",
     "CreatePlayerSessionsInputRequestTypeDef",
     "CreateVpcPeeringAuthorizationInputRequestTypeDef",
     "VpcPeeringAuthorizationTypeDef",
     "CreateVpcPeeringConnectionInputRequestTypeDef",
     "DeleteAliasInputRequestTypeDef",
     "DeleteBuildInputRequestTypeDef",
+    "DeleteContainerGroupDefinitionInputRequestTypeDef",
     "DeleteFleetInputRequestTypeDef",
     "DeleteFleetLocationsInputRequestTypeDef",
     "DeleteGameServerGroupInputRequestTypeDef",
     "DeleteGameSessionQueueInputRequestTypeDef",
     "DeleteLocationInputRequestTypeDef",
     "DeleteMatchmakingConfigurationInputRequestTypeDef",
     "DeleteMatchmakingRuleSetInputRequestTypeDef",
@@ -119,14 +132,15 @@
     "DeleteVpcPeeringAuthorizationInputRequestTypeDef",
     "DeleteVpcPeeringConnectionInputRequestTypeDef",
     "DeregisterComputeInputRequestTypeDef",
     "DeregisterGameServerInputRequestTypeDef",
     "DescribeAliasInputRequestTypeDef",
     "DescribeBuildInputRequestTypeDef",
     "DescribeComputeInputRequestTypeDef",
+    "DescribeContainerGroupDefinitionInputRequestTypeDef",
     "DescribeEC2InstanceLimitsInputRequestTypeDef",
     "EC2InstanceLimitTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeFleetAttributesInputRequestTypeDef",
     "DescribeFleetCapacityInputRequestTypeDef",
     "TimestampTypeDef",
     "EventTypeDef",
@@ -153,27 +167,29 @@
     "DescribeRuntimeConfigurationInputRequestTypeDef",
     "DescribeScalingPoliciesInputRequestTypeDef",
     "DescribeScriptInputRequestTypeDef",
     "DescribeVpcPeeringConnectionsInputRequestTypeDef",
     "DesiredPlayerSessionTypeDef",
     "EC2InstanceCountsTypeDef",
     "FilterConfigurationPaginatorTypeDef",
+    "ReplicaContainerGroupCountsTypeDef",
     "TargetTrackingConfigurationTypeDef",
     "MatchedPlayerSessionTypeDef",
     "PlacedPlayerSessionTypeDef",
     "PlayerLatencyTypeDef",
     "PriorityConfigurationPaginatorTypeDef",
     "GetComputeAccessInputRequestTypeDef",
     "GetComputeAuthTokenInputRequestTypeDef",
     "GetGameSessionLogUrlInputRequestTypeDef",
     "GetInstanceAccessInputRequestTypeDef",
     "InstanceCredentialsTypeDef",
     "ListAliasesInputRequestTypeDef",
     "ListBuildsInputRequestTypeDef",
     "ListComputeInputRequestTypeDef",
+    "ListContainerGroupDefinitionsInputRequestTypeDef",
     "ListFleetsInputRequestTypeDef",
     "ListGameServerGroupsInputRequestTypeDef",
     "ListGameServersInputRequestTypeDef",
     "ListLocationsInputRequestTypeDef",
     "ListScriptsInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TargetConfigurationTypeDef",
@@ -216,32 +232,33 @@
     "StopFleetActionsOutputTypeDef",
     "UpdateBuildOutputTypeDef",
     "UpdateFleetAttributesOutputTypeDef",
     "UpdateFleetCapacityOutputTypeDef",
     "UpdateFleetPortSettingsOutputTypeDef",
     "UpdateGameServerOutputTypeDef",
     "ValidateMatchmakingRuleSetOutputTypeDef",
-    "DescribeComputeOutputTypeDef",
-    "ListComputeOutputTypeDef",
-    "RegisterComputeOutputTypeDef",
+    "ContainerGroupsConfigurationTypeDef",
+    "ContainerAttributesTypeDef",
+    "ContainerGroupsAttributesTypeDef",
+    "ContainerPortConfigurationPaginatorTypeDef",
+    "ContainerPortConfigurationTypeDef",
     "CreateAliasInputRequestTypeDef",
     "CreateLocationInputRequestTypeDef",
     "CreateMatchmakingRuleSetInputRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateBuildInputRequestTypeDef",
     "CreateBuildOutputTypeDef",
     "CreateScriptInputRequestTypeDef",
     "RequestUploadCredentialsOutputTypeDef",
     "ScriptTypeDef",
     "UpdateScriptInputRequestTypeDef",
     "DescribeFleetPortSettingsOutputTypeDef",
     "UpdateFleetPortSettingsInputRequestTypeDef",
     "CreateFleetLocationsInputRequestTypeDef",
-    "FleetAttributesTypeDef",
     "UpdateFleetAttributesInputRequestTypeDef",
     "CreateFleetLocationsOutputTypeDef",
     "DeleteFleetLocationsOutputTypeDef",
     "LocationAttributesTypeDef",
     "GameServerGroupTypeDef",
     "UpdateGameServerGroupInputRequestTypeDef",
     "CreateGameSessionInputRequestTypeDef",
@@ -274,14 +291,15 @@
     "DescribeMatchmakingConfigurationsInputDescribeMatchmakingConfigurationsPaginateTypeDef",
     "DescribeMatchmakingRuleSetsInputDescribeMatchmakingRuleSetsPaginateTypeDef",
     "DescribePlayerSessionsInputDescribePlayerSessionsPaginateTypeDef",
     "DescribeScalingPoliciesInputDescribeScalingPoliciesPaginateTypeDef",
     "ListAliasesInputListAliasesPaginateTypeDef",
     "ListBuildsInputListBuildsPaginateTypeDef",
     "ListComputeInputListComputePaginateTypeDef",
+    "ListContainerGroupDefinitionsInputListContainerGroupDefinitionsPaginateTypeDef",
     "ListFleetsInputListFleetsPaginateTypeDef",
     "ListGameServerGroupsInputListGameServerGroupsPaginateTypeDef",
     "ListGameServersInputListGameServersPaginateTypeDef",
     "ListLocationsInputListLocationsPaginateTypeDef",
     "ListScriptsInputListScriptsPaginateTypeDef",
     "SearchGameSessionsInputSearchGameSessionsPaginateTypeDef",
     "DescribeFleetEventsInputDescribeFleetEventsPaginateTypeDef",
@@ -304,20 +322,23 @@
     "VpcPeeringConnectionTypeDef",
     "CreateAliasOutputTypeDef",
     "DescribeAliasOutputTypeDef",
     "ListAliasesOutputTypeDef",
     "UpdateAliasOutputTypeDef",
     "StartMatchBackfillInputRequestTypeDef",
     "StartMatchmakingInputRequestTypeDef",
+    "ComputeTypeDef",
+    "FleetAttributesTypeDef",
+    "ContainerDefinitionPaginatorTypeDef",
+    "ContainerDefinitionInputTypeDef",
+    "ContainerDefinitionTypeDef",
     "CreateScriptOutputTypeDef",
     "DescribeScriptOutputTypeDef",
     "ListScriptsOutputTypeDef",
     "UpdateScriptOutputTypeDef",
-    "CreateFleetOutputTypeDef",
-    "DescribeFleetAttributesOutputTypeDef",
     "DescribeFleetLocationAttributesOutputTypeDef",
     "CreateGameServerGroupOutputTypeDef",
     "DeleteGameServerGroupOutputTypeDef",
     "DescribeGameServerGroupOutputTypeDef",
     "ListGameServerGroupsOutputTypeDef",
     "ResumeGameServerGroupOutputTypeDef",
     "SuspendGameServerGroupOutputTypeDef",
@@ -344,18 +365,30 @@
     "GetInstanceAccessOutputTypeDef",
     "DescribeScalingPoliciesOutputTypeDef",
     "CreateFleetInputRequestTypeDef",
     "DescribeRuntimeConfigurationOutputTypeDef",
     "UpdateRuntimeConfigurationInputRequestTypeDef",
     "UpdateRuntimeConfigurationOutputTypeDef",
     "DescribeVpcPeeringConnectionsOutputTypeDef",
+    "DescribeComputeOutputTypeDef",
+    "ListComputeOutputTypeDef",
+    "RegisterComputeOutputTypeDef",
+    "CreateFleetOutputTypeDef",
+    "DescribeFleetAttributesOutputTypeDef",
+    "ContainerGroupDefinitionPaginatorTypeDef",
+    "CreateContainerGroupDefinitionInputRequestTypeDef",
+    "ContainerGroupDefinitionTypeDef",
     "DescribeGameSessionDetailsOutputTypeDef",
     "DescribeMatchmakingOutputTypeDef",
     "StartMatchBackfillOutputTypeDef",
     "StartMatchmakingOutputTypeDef",
+    "ListContainerGroupDefinitionsOutputPaginatorTypeDef",
+    "CreateContainerGroupDefinitionOutputTypeDef",
+    "DescribeContainerGroupDefinitionOutputTypeDef",
+    "ListContainerGroupDefinitionsOutputTypeDef",
 )
 
 AcceptMatchInputRequestTypeDef = TypedDict(
     "AcceptMatchInputRequestTypeDef",
     {
         "TicketId": str,
         "PlayerIds": Sequence[str],
@@ -436,35 +469,96 @@
         "LastHealthCheckTime": NotRequired[datetime],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
-ComputeTypeDef = TypedDict(
-    "ComputeTypeDef",
+ConnectionPortRangeTypeDef = TypedDict(
+    "ConnectionPortRangeTypeDef",
     {
-        "FleetId": NotRequired[str],
-        "FleetArn": NotRequired[str],
-        "ComputeName": NotRequired[str],
-        "ComputeArn": NotRequired[str],
-        "IpAddress": NotRequired[str],
-        "DnsName": NotRequired[str],
-        "ComputeStatus": NotRequired[ComputeStatusType],
-        "Location": NotRequired[str],
-        "CreationTime": NotRequired[datetime],
-        "OperatingSystem": NotRequired[OperatingSystemType],
-        "Type": NotRequired[EC2InstanceTypeType],
-        "GameLiftServiceSdkEndpoint": NotRequired[str],
+        "FromPort": int,
+        "ToPort": int,
+    },
+)
+ContainerPortMappingTypeDef = TypedDict(
+    "ContainerPortMappingTypeDef",
+    {
+        "ContainerPort": NotRequired[int],
+        "ConnectionPort": NotRequired[int],
+        "Protocol": NotRequired[IpProtocolType],
+    },
+)
+ContainerDependencyTypeDef = TypedDict(
+    "ContainerDependencyTypeDef",
+    {
+        "ContainerName": str,
+        "Condition": ContainerDependencyConditionType,
+    },
+)
+ContainerEnvironmentTypeDef = TypedDict(
+    "ContainerEnvironmentTypeDef",
+    {
+        "Name": str,
+        "Value": str,
+    },
+)
+ContainerHealthCheckTypeDef = TypedDict(
+    "ContainerHealthCheckTypeDef",
+    {
+        "Command": Sequence[str],
+        "Interval": NotRequired[int],
+        "Timeout": NotRequired[int],
+        "Retries": NotRequired[int],
+        "StartPeriod": NotRequired[int],
+    },
+)
+ContainerMemoryLimitsTypeDef = TypedDict(
+    "ContainerMemoryLimitsTypeDef",
+    {
+        "SoftLimit": NotRequired[int],
+        "HardLimit": NotRequired[int],
+    },
+)
+ContainerHealthCheckPaginatorTypeDef = TypedDict(
+    "ContainerHealthCheckPaginatorTypeDef",
+    {
+        "Command": List[str],
+        "Interval": NotRequired[int],
+        "Timeout": NotRequired[int],
+        "Retries": NotRequired[int],
+        "StartPeriod": NotRequired[int],
+    },
+)
+ContainerGroupDefinitionPropertyTypeDef = TypedDict(
+    "ContainerGroupDefinitionPropertyTypeDef",
+    {
+        "SchedulingStrategy": NotRequired[ContainerSchedulingStrategyType],
+        "ContainerGroupDefinitionName": NotRequired[str],
+    },
+)
+ContainerGroupsPerInstanceTypeDef = TypedDict(
+    "ContainerGroupsPerInstanceTypeDef",
+    {
+        "DesiredReplicaContainerGroupsPerInstance": NotRequired[int],
+        "MaxReplicaContainerGroupsPerInstance": NotRequired[int],
+    },
+)
+ContainerPortRangeTypeDef = TypedDict(
+    "ContainerPortRangeTypeDef",
+    {
+        "FromPort": int,
+        "ToPort": int,
+        "Protocol": IpProtocolType,
     },
 )
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
@@ -638,14 +732,20 @@
 )
 DeleteBuildInputRequestTypeDef = TypedDict(
     "DeleteBuildInputRequestTypeDef",
     {
         "BuildId": str,
     },
 )
+DeleteContainerGroupDefinitionInputRequestTypeDef = TypedDict(
+    "DeleteContainerGroupDefinitionInputRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
 DeleteFleetInputRequestTypeDef = TypedDict(
     "DeleteFleetInputRequestTypeDef",
     {
         "FleetId": str,
     },
 )
 DeleteFleetLocationsInputRequestTypeDef = TypedDict(
@@ -742,14 +842,20 @@
 DescribeComputeInputRequestTypeDef = TypedDict(
     "DescribeComputeInputRequestTypeDef",
     {
         "FleetId": str,
         "ComputeName": str,
     },
 )
+DescribeContainerGroupDefinitionInputRequestTypeDef = TypedDict(
+    "DescribeContainerGroupDefinitionInputRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
 DescribeEC2InstanceLimitsInputRequestTypeDef = TypedDict(
     "DescribeEC2InstanceLimitsInputRequestTypeDef",
     {
         "EC2InstanceType": NotRequired[EC2InstanceTypeType],
         "Location": NotRequired[str],
     },
 )
@@ -792,14 +898,15 @@
     {
         "EventId": NotRequired[str],
         "ResourceId": NotRequired[str],
         "EventCode": NotRequired[EventCodeType],
         "Message": NotRequired[str],
         "EventTime": NotRequired[datetime],
         "PreSignedLogUrl": NotRequired[str],
+        "Count": NotRequired[int],
     },
 )
 DescribeFleetLocationAttributesInputRequestTypeDef = TypedDict(
     "DescribeFleetLocationAttributesInputRequestTypeDef",
     {
         "FleetId": str,
         "Locations": NotRequired[Sequence[str]],
@@ -1025,14 +1132,23 @@
 )
 FilterConfigurationPaginatorTypeDef = TypedDict(
     "FilterConfigurationPaginatorTypeDef",
     {
         "AllowedLocations": NotRequired[List[str]],
     },
 )
+ReplicaContainerGroupCountsTypeDef = TypedDict(
+    "ReplicaContainerGroupCountsTypeDef",
+    {
+        "PENDING": NotRequired[int],
+        "ACTIVE": NotRequired[int],
+        "IDLE": NotRequired[int],
+        "TERMINATING": NotRequired[int],
+    },
+)
 TargetTrackingConfigurationTypeDef = TypedDict(
     "TargetTrackingConfigurationTypeDef",
     {
         "TargetValue": float,
     },
 )
 MatchedPlayerSessionTypeDef = TypedDict(
@@ -1120,19 +1236,28 @@
     {
         "FleetId": str,
         "Location": NotRequired[str],
         "Limit": NotRequired[int],
         "NextToken": NotRequired[str],
     },
 )
+ListContainerGroupDefinitionsInputRequestTypeDef = TypedDict(
+    "ListContainerGroupDefinitionsInputRequestTypeDef",
+    {
+        "SchedulingStrategy": NotRequired[ContainerSchedulingStrategyType],
+        "Limit": NotRequired[int],
+        "NextToken": NotRequired[str],
+    },
+)
 ListFleetsInputRequestTypeDef = TypedDict(
     "ListFleetsInputRequestTypeDef",
     {
         "BuildId": NotRequired[str],
         "ScriptId": NotRequired[str],
+        "ContainerGroupDefinitionName": NotRequired[str],
         "Limit": NotRequired[int],
         "NextToken": NotRequired[str],
     },
 )
 ListGameServerGroupsInputRequestTypeDef = TypedDict(
     "ListGameServerGroupsInputRequestTypeDef",
     {
@@ -1389,14 +1514,15 @@
     "GetComputeAccessOutputTypeDef",
     {
         "FleetId": str,
         "FleetArn": str,
         "ComputeName": str,
         "ComputeArn": str,
         "Credentials": AwsCredentialsTypeDef,
+        "Target": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetComputeAuthTokenOutputTypeDef = TypedDict(
     "GetComputeAuthTokenOutputTypeDef",
     {
         "FleetId": str,
@@ -1519,34 +1645,48 @@
 ValidateMatchmakingRuleSetOutputTypeDef = TypedDict(
     "ValidateMatchmakingRuleSetOutputTypeDef",
     {
         "Valid": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-DescribeComputeOutputTypeDef = TypedDict(
-    "DescribeComputeOutputTypeDef",
+ContainerGroupsConfigurationTypeDef = TypedDict(
+    "ContainerGroupsConfigurationTypeDef",
     {
-        "Compute": ComputeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ContainerGroupDefinitionNames": Sequence[str],
+        "ConnectionPortRange": ConnectionPortRangeTypeDef,
+        "DesiredReplicaContainerGroupsPerInstance": NotRequired[int],
     },
 )
-ListComputeOutputTypeDef = TypedDict(
-    "ListComputeOutputTypeDef",
+ContainerAttributesTypeDef = TypedDict(
+    "ContainerAttributesTypeDef",
     {
-        "ComputeList": List[ComputeTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ContainerPortMappings": NotRequired[List[ContainerPortMappingTypeDef]],
     },
 )
-RegisterComputeOutputTypeDef = TypedDict(
-    "RegisterComputeOutputTypeDef",
+ContainerGroupsAttributesTypeDef = TypedDict(
+    "ContainerGroupsAttributesTypeDef",
     {
-        "Compute": ComputeTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ContainerGroupDefinitionProperties": NotRequired[
+            List[ContainerGroupDefinitionPropertyTypeDef]
+        ],
+        "ConnectionPortRange": NotRequired[ConnectionPortRangeTypeDef],
+        "ContainerGroupsPerInstance": NotRequired[ContainerGroupsPerInstanceTypeDef],
+    },
+)
+ContainerPortConfigurationPaginatorTypeDef = TypedDict(
+    "ContainerPortConfigurationPaginatorTypeDef",
+    {
+        "ContainerPortRanges": List[ContainerPortRangeTypeDef],
+    },
+)
+ContainerPortConfigurationTypeDef = TypedDict(
+    "ContainerPortConfigurationTypeDef",
+    {
+        "ContainerPortRanges": Sequence[ContainerPortRangeTypeDef],
     },
 )
 CreateAliasInputRequestTypeDef = TypedDict(
     "CreateAliasInputRequestTypeDef",
     {
         "Name": str,
         "RoutingStrategy": RoutingStrategyTypeDef,
@@ -1665,45 +1805,14 @@
 CreateFleetLocationsInputRequestTypeDef = TypedDict(
     "CreateFleetLocationsInputRequestTypeDef",
     {
         "FleetId": str,
         "Locations": Sequence[LocationConfigurationTypeDef],
     },
 )
-FleetAttributesTypeDef = TypedDict(
-    "FleetAttributesTypeDef",
-    {
-        "FleetId": NotRequired[str],
-        "FleetArn": NotRequired[str],
-        "FleetType": NotRequired[FleetTypeType],
-        "InstanceType": NotRequired[EC2InstanceTypeType],
-        "Description": NotRequired[str],
-        "Name": NotRequired[str],
-        "CreationTime": NotRequired[datetime],
-        "TerminationTime": NotRequired[datetime],
-        "Status": NotRequired[FleetStatusType],
-        "BuildId": NotRequired[str],
-        "BuildArn": NotRequired[str],
-        "ScriptId": NotRequired[str],
-        "ScriptArn": NotRequired[str],
-        "ServerLaunchPath": NotRequired[str],
-        "ServerLaunchParameters": NotRequired[str],
-        "LogPaths": NotRequired[List[str]],
-        "NewGameSessionProtectionPolicy": NotRequired[ProtectionPolicyType],
-        "OperatingSystem": NotRequired[OperatingSystemType],
-        "ResourceCreationLimitPolicy": NotRequired[ResourceCreationLimitPolicyTypeDef],
-        "MetricGroups": NotRequired[List[str]],
-        "StoppedActions": NotRequired[List[Literal["AUTO_SCALING"]]],
-        "InstanceRoleArn": NotRequired[str],
-        "CertificateConfiguration": NotRequired[CertificateConfigurationTypeDef],
-        "ComputeType": NotRequired[ComputeTypeType],
-        "AnywhereConfiguration": NotRequired[AnywhereConfigurationTypeDef],
-        "InstanceRoleCredentialsProvider": NotRequired[Literal["SHARED_CREDENTIAL_FILE"]],
-    },
-)
 UpdateFleetAttributesInputRequestTypeDef = TypedDict(
     "UpdateFleetAttributesInputRequestTypeDef",
     {
         "FleetId": str,
         "Name": NotRequired[str],
         "Description": NotRequired[str],
         "NewGameSessionProtectionPolicy": NotRequired[ProtectionPolicyType],
@@ -2110,19 +2219,27 @@
     "ListComputeInputListComputePaginateTypeDef",
     {
         "FleetId": str,
         "Location": NotRequired[str],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+ListContainerGroupDefinitionsInputListContainerGroupDefinitionsPaginateTypeDef = TypedDict(
+    "ListContainerGroupDefinitionsInputListContainerGroupDefinitionsPaginateTypeDef",
+    {
+        "SchedulingStrategy": NotRequired[ContainerSchedulingStrategyType],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
 ListFleetsInputListFleetsPaginateTypeDef = TypedDict(
     "ListFleetsInputListFleetsPaginateTypeDef",
     {
         "BuildId": NotRequired[str],
         "ScriptId": NotRequired[str],
+        "ContainerGroupDefinitionName": NotRequired[str],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListGameServerGroupsInputListGameServerGroupsPaginateTypeDef = TypedDict(
     "ListGameServerGroupsInputListGameServerGroupsPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
@@ -2222,14 +2339,15 @@
     "FleetCapacityTypeDef",
     {
         "FleetId": NotRequired[str],
         "FleetArn": NotRequired[str],
         "InstanceType": NotRequired[EC2InstanceTypeType],
         "InstanceCounts": NotRequired[EC2InstanceCountsTypeDef],
         "Location": NotRequired[str],
+        "ReplicaContainerGroupCounts": NotRequired[ReplicaContainerGroupCountsTypeDef],
     },
 )
 GameServerGroupAutoScalingPolicyTypeDef = TypedDict(
     "GameServerGroupAutoScalingPolicyTypeDef",
     {
         "TargetTrackingConfiguration": TargetTrackingConfigurationTypeDef,
         "EstimatedInstanceWarmup": NotRequired[int],
@@ -2401,14 +2519,119 @@
     "StartMatchmakingInputRequestTypeDef",
     {
         "ConfigurationName": str,
         "Players": Sequence[PlayerTypeDef],
         "TicketId": NotRequired[str],
     },
 )
+ComputeTypeDef = TypedDict(
+    "ComputeTypeDef",
+    {
+        "FleetId": NotRequired[str],
+        "FleetArn": NotRequired[str],
+        "ComputeName": NotRequired[str],
+        "ComputeArn": NotRequired[str],
+        "IpAddress": NotRequired[str],
+        "DnsName": NotRequired[str],
+        "ComputeStatus": NotRequired[ComputeStatusType],
+        "Location": NotRequired[str],
+        "CreationTime": NotRequired[datetime],
+        "OperatingSystem": NotRequired[OperatingSystemType],
+        "Type": NotRequired[EC2InstanceTypeType],
+        "GameLiftServiceSdkEndpoint": NotRequired[str],
+        "GameLiftAgentEndpoint": NotRequired[str],
+        "InstanceId": NotRequired[str],
+        "ContainerAttributes": NotRequired[ContainerAttributesTypeDef],
+    },
+)
+FleetAttributesTypeDef = TypedDict(
+    "FleetAttributesTypeDef",
+    {
+        "FleetId": NotRequired[str],
+        "FleetArn": NotRequired[str],
+        "FleetType": NotRequired[FleetTypeType],
+        "InstanceType": NotRequired[EC2InstanceTypeType],
+        "Description": NotRequired[str],
+        "Name": NotRequired[str],
+        "CreationTime": NotRequired[datetime],
+        "TerminationTime": NotRequired[datetime],
+        "Status": NotRequired[FleetStatusType],
+        "BuildId": NotRequired[str],
+        "BuildArn": NotRequired[str],
+        "ScriptId": NotRequired[str],
+        "ScriptArn": NotRequired[str],
+        "ServerLaunchPath": NotRequired[str],
+        "ServerLaunchParameters": NotRequired[str],
+        "LogPaths": NotRequired[List[str]],
+        "NewGameSessionProtectionPolicy": NotRequired[ProtectionPolicyType],
+        "OperatingSystem": NotRequired[OperatingSystemType],
+        "ResourceCreationLimitPolicy": NotRequired[ResourceCreationLimitPolicyTypeDef],
+        "MetricGroups": NotRequired[List[str]],
+        "StoppedActions": NotRequired[List[Literal["AUTO_SCALING"]]],
+        "InstanceRoleArn": NotRequired[str],
+        "CertificateConfiguration": NotRequired[CertificateConfigurationTypeDef],
+        "ComputeType": NotRequired[ComputeTypeType],
+        "AnywhereConfiguration": NotRequired[AnywhereConfigurationTypeDef],
+        "InstanceRoleCredentialsProvider": NotRequired[Literal["SHARED_CREDENTIAL_FILE"]],
+        "ContainerGroupsAttributes": NotRequired[ContainerGroupsAttributesTypeDef],
+    },
+)
+ContainerDefinitionPaginatorTypeDef = TypedDict(
+    "ContainerDefinitionPaginatorTypeDef",
+    {
+        "ContainerName": str,
+        "ImageUri": str,
+        "ResolvedImageDigest": NotRequired[str],
+        "MemoryLimits": NotRequired[ContainerMemoryLimitsTypeDef],
+        "PortConfiguration": NotRequired[ContainerPortConfigurationPaginatorTypeDef],
+        "Cpu": NotRequired[int],
+        "HealthCheck": NotRequired[ContainerHealthCheckPaginatorTypeDef],
+        "Command": NotRequired[List[str]],
+        "Essential": NotRequired[bool],
+        "EntryPoint": NotRequired[List[str]],
+        "WorkingDirectory": NotRequired[str],
+        "Environment": NotRequired[List[ContainerEnvironmentTypeDef]],
+        "DependsOn": NotRequired[List[ContainerDependencyTypeDef]],
+    },
+)
+ContainerDefinitionInputTypeDef = TypedDict(
+    "ContainerDefinitionInputTypeDef",
+    {
+        "ContainerName": str,
+        "ImageUri": str,
+        "MemoryLimits": NotRequired[ContainerMemoryLimitsTypeDef],
+        "PortConfiguration": NotRequired[ContainerPortConfigurationTypeDef],
+        "Cpu": NotRequired[int],
+        "HealthCheck": NotRequired[ContainerHealthCheckTypeDef],
+        "Command": NotRequired[Sequence[str]],
+        "Essential": NotRequired[bool],
+        "EntryPoint": NotRequired[Sequence[str]],
+        "WorkingDirectory": NotRequired[str],
+        "Environment": NotRequired[Sequence[ContainerEnvironmentTypeDef]],
+        "DependsOn": NotRequired[Sequence[ContainerDependencyTypeDef]],
+    },
+)
+ContainerDefinitionTypeDef = TypedDict(
+    "ContainerDefinitionTypeDef",
+    {
+        "ContainerName": str,
+        "ImageUri": str,
+        "ResolvedImageDigest": NotRequired[str],
+        "MemoryLimits": NotRequired[ContainerMemoryLimitsTypeDef],
+        "PortConfiguration": NotRequired[ContainerPortConfigurationTypeDef],
+        "Cpu": NotRequired[int],
+        "HealthCheck": NotRequired[ContainerHealthCheckTypeDef],
+        "Command": NotRequired[List[str]],
+        "Essential": NotRequired[bool],
+        "EntryPoint": NotRequired[List[str]],
+        "WorkingDirectory": NotRequired[str],
+        "Environment": NotRequired[List[ContainerEnvironmentTypeDef]],
+        "DependsOn": NotRequired[List[ContainerDependencyTypeDef]],
+    },
+)
 CreateScriptOutputTypeDef = TypedDict(
     "CreateScriptOutputTypeDef",
     {
         "Script": ScriptTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2430,30 +2653,14 @@
 UpdateScriptOutputTypeDef = TypedDict(
     "UpdateScriptOutputTypeDef",
     {
         "Script": ScriptTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CreateFleetOutputTypeDef = TypedDict(
-    "CreateFleetOutputTypeDef",
-    {
-        "FleetAttributes": FleetAttributesTypeDef,
-        "LocationStates": List[LocationStateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeFleetAttributesOutputTypeDef = TypedDict(
-    "DescribeFleetAttributesOutputTypeDef",
-    {
-        "FleetAttributes": List[FleetAttributesTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 DescribeFleetLocationAttributesOutputTypeDef = TypedDict(
     "DescribeFleetLocationAttributesOutputTypeDef",
     {
         "FleetId": str,
         "FleetArn": str,
         "LocationAttributes": List[LocationAttributesTypeDef],
         "NextToken": str,
@@ -2704,14 +2911,15 @@
         "InstanceRoleArn": NotRequired[str],
         "CertificateConfiguration": NotRequired[CertificateConfigurationTypeDef],
         "Locations": NotRequired[Sequence[LocationConfigurationTypeDef]],
         "Tags": NotRequired[Sequence[TagTypeDef]],
         "ComputeType": NotRequired[ComputeTypeType],
         "AnywhereConfiguration": NotRequired[AnywhereConfigurationTypeDef],
         "InstanceRoleCredentialsProvider": NotRequired[Literal["SHARED_CREDENTIAL_FILE"]],
+        "ContainerGroupsConfiguration": NotRequired[ContainerGroupsConfigurationTypeDef],
     },
 )
 DescribeRuntimeConfigurationOutputTypeDef = TypedDict(
     "DescribeRuntimeConfigurationOutputTypeDef",
     {
         "RuntimeConfiguration": RuntimeConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2734,14 +2942,94 @@
 DescribeVpcPeeringConnectionsOutputTypeDef = TypedDict(
     "DescribeVpcPeeringConnectionsOutputTypeDef",
     {
         "VpcPeeringConnections": List[VpcPeeringConnectionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DescribeComputeOutputTypeDef = TypedDict(
+    "DescribeComputeOutputTypeDef",
+    {
+        "Compute": ComputeTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ListComputeOutputTypeDef = TypedDict(
+    "ListComputeOutputTypeDef",
+    {
+        "ComputeList": List[ComputeTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+RegisterComputeOutputTypeDef = TypedDict(
+    "RegisterComputeOutputTypeDef",
+    {
+        "Compute": ComputeTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+CreateFleetOutputTypeDef = TypedDict(
+    "CreateFleetOutputTypeDef",
+    {
+        "FleetAttributes": FleetAttributesTypeDef,
+        "LocationStates": List[LocationStateTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DescribeFleetAttributesOutputTypeDef = TypedDict(
+    "DescribeFleetAttributesOutputTypeDef",
+    {
+        "FleetAttributes": List[FleetAttributesTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ContainerGroupDefinitionPaginatorTypeDef = TypedDict(
+    "ContainerGroupDefinitionPaginatorTypeDef",
+    {
+        "ContainerGroupDefinitionArn": NotRequired[str],
+        "CreationTime": NotRequired[datetime],
+        "OperatingSystem": NotRequired[Literal["AMAZON_LINUX_2023"]],
+        "Name": NotRequired[str],
+        "SchedulingStrategy": NotRequired[ContainerSchedulingStrategyType],
+        "TotalMemoryLimit": NotRequired[int],
+        "TotalCpuLimit": NotRequired[int],
+        "ContainerDefinitions": NotRequired[List[ContainerDefinitionPaginatorTypeDef]],
+        "Status": NotRequired[ContainerGroupDefinitionStatusType],
+        "StatusReason": NotRequired[str],
+    },
+)
+CreateContainerGroupDefinitionInputRequestTypeDef = TypedDict(
+    "CreateContainerGroupDefinitionInputRequestTypeDef",
+    {
+        "Name": str,
+        "TotalMemoryLimit": int,
+        "TotalCpuLimit": int,
+        "ContainerDefinitions": Sequence[ContainerDefinitionInputTypeDef],
+        "OperatingSystem": Literal["AMAZON_LINUX_2023"],
+        "SchedulingStrategy": NotRequired[ContainerSchedulingStrategyType],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+    },
+)
+ContainerGroupDefinitionTypeDef = TypedDict(
+    "ContainerGroupDefinitionTypeDef",
+    {
+        "ContainerGroupDefinitionArn": NotRequired[str],
+        "CreationTime": NotRequired[datetime],
+        "OperatingSystem": NotRequired[Literal["AMAZON_LINUX_2023"]],
+        "Name": NotRequired[str],
+        "SchedulingStrategy": NotRequired[ContainerSchedulingStrategyType],
+        "TotalMemoryLimit": NotRequired[int],
+        "TotalCpuLimit": NotRequired[int],
+        "ContainerDefinitions": NotRequired[List[ContainerDefinitionTypeDef]],
+        "Status": NotRequired[ContainerGroupDefinitionStatusType],
+        "StatusReason": NotRequired[str],
+    },
+)
 DescribeGameSessionDetailsOutputTypeDef = TypedDict(
     "DescribeGameSessionDetailsOutputTypeDef",
     {
         "GameSessionDetails": List[GameSessionDetailTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2763,7 +3051,37 @@
 StartMatchmakingOutputTypeDef = TypedDict(
     "StartMatchmakingOutputTypeDef",
     {
         "MatchmakingTicket": MatchmakingTicketTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ListContainerGroupDefinitionsOutputPaginatorTypeDef = TypedDict(
+    "ListContainerGroupDefinitionsOutputPaginatorTypeDef",
+    {
+        "ContainerGroupDefinitions": List[ContainerGroupDefinitionPaginatorTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+CreateContainerGroupDefinitionOutputTypeDef = TypedDict(
+    "CreateContainerGroupDefinitionOutputTypeDef",
+    {
+        "ContainerGroupDefinition": ContainerGroupDefinitionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DescribeContainerGroupDefinitionOutputTypeDef = TypedDict(
+    "DescribeContainerGroupDefinitionOutputTypeDef",
+    {
+        "ContainerGroupDefinition": ContainerGroupDefinitionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ListContainerGroupDefinitionsOutputTypeDef = TypedDict(
+    "ListContainerGroupDefinitionsOutputTypeDef",
+    {
+        "ContainerGroupDefinitions": List[ContainerGroupDefinitionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift.egg-info/PKG-INFO` & `mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-gamelift
-Version: 1.34.1
-Summary: Type annotations for boto3.GameLift 1.34.1 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.91
+Summary: Type annotations for boto3.GameLift 1.34.91 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-gamelift"></a>
 
 # mypy-boto3-gamelift
 
 [![PyPI - mypy-boto3-gamelift](https://img.shields.io/pypi/v/mypy-boto3-gamelift.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamelift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-gamelift.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamelift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-gamelift)](https://pepy.tech/project/mypy-boto3-gamelift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GameLift 1.34.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
+[boto3.GameLift 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#GameLift)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-gamelift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -296,14 +296,15 @@
     DescribeMatchmakingConfigurationsPaginator,
     DescribeMatchmakingRuleSetsPaginator,
     DescribePlayerSessionsPaginator,
     DescribeScalingPoliciesPaginator,
     ListAliasesPaginator,
     ListBuildsPaginator,
     ListComputePaginator,
+    ListContainerGroupDefinitionsPaginator,
     ListFleetsPaginator,
     ListGameServerGroupsPaginator,
     ListGameServersPaginator,
     ListLocationsPaginator,
     ListScriptsPaginator,
     SearchGameSessionsPaginator,
 )
@@ -350,14 +351,17 @@
 )
 describe_scaling_policies_paginator: DescribeScalingPoliciesPaginator = client.get_paginator(
     "describe_scaling_policies"
 )
 list_aliases_paginator: ListAliasesPaginator = client.get_paginator("list_aliases")
 list_builds_paginator: ListBuildsPaginator = client.get_paginator("list_builds")
 list_compute_paginator: ListComputePaginator = client.get_paginator("list_compute")
+list_container_group_definitions_paginator: ListContainerGroupDefinitionsPaginator = (
+    client.get_paginator("list_container_group_definitions")
+)
 list_fleets_paginator: ListFleetsPaginator = client.get_paginator("list_fleets")
 list_game_server_groups_paginator: ListGameServerGroupsPaginator = client.get_paginator(
     "list_game_server_groups"
 )
 list_game_servers_paginator: ListGameServersPaginator = client.get_paginator("list_game_servers")
 list_locations_paginator: ListLocationsPaginator = client.get_paginator("list_locations")
 list_scripts_paginator: ListScriptsPaginator = client.get_paginator("list_scripts")
```

### Comparing `mypy-boto3-gamelift-1.34.1/mypy_boto3_gamelift.egg-info/SOURCES.txt` & `mypy_boto3_gamelift-1.34.91/mypy_boto3_gamelift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamelift-1.34.1/setup.py` & `mypy_boto3_gamelift-1.34.91/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,48 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-gamelift",
-    version="1.34.1",
+    version="1.34.91",
     packages=["mypy_boto3_gamelift"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.GameLift 1.34.1 service generated with mypy-boto3-builder"
-        " 7.21.0"
-    ),
+    description="Type annotations for boto3.GameLift 1.34.91 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Typing :: Typed",
+        "Typing :: Stubs Only",
     ],
     keywords="boto3 gamelift type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_gamelift": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamelift/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

