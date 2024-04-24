# Comparing `tmp/allocmd-0.3.8.tar.gz` & `tmp/allocmd-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/allocmd-0.3.8.tar", last modified: Mon Apr 22 18:02:43 2024, max compression
+gzip compressed data, was "dist/allocmd-0.3.9.tar", last modified: Mon Apr 22 18:43:41 2024, max compression
```

## Comparing `allocmd-0.3.8.tar` & `allocmd-0.3.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:02:43.000000 allocmd-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-22 18:02:43.000000 allocmd-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-04-22 18:02:34.000000 allocmd-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:02:43.000000 allocmd-0.3.8/allocmd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 18:02:34.000000 allocmd-0.3.8/allocmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-04-22 18:02:34.000000 allocmd-0.3.8/allocmd/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:02:43.000000 allocmd-0.3.8/allocmd/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 18:02:34.000000 allocmd-0.3.8/allocmd/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 18:02:34.000000 allocmd-0.3.8/allocmd/utilities/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-22 18:02:34.000000 allocmd-0.3.8/allocmd/utilities/typings.py
--rw-r--r--   0 runner    (1001) docker     (127)    23481 2024-04-22 18:02:34.000000 allocmd-0.3.8/allocmd/utilities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:02:43.000000 allocmd-0.3.8/allocmd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-22 18:02:42.000000 allocmd-0.3.8/allocmd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-22 18:02:43.000000 allocmd-0.3.8/allocmd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 18:02:42.000000 allocmd-0.3.8/allocmd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-22 18:02:42.000000 allocmd-0.3.8/allocmd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-22 18:02:42.000000 allocmd-0.3.8/allocmd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 18:02:42.000000 allocmd-0.3.8/allocmd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 18:02:43.000000 allocmd-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-22 18:02:34.000000 allocmd-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:43:41.000000 allocmd-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-22 18:43:41.000000 allocmd-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-04-22 18:43:29.000000 allocmd-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:43:41.000000 allocmd-0.3.9/allocmd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 18:43:29.000000 allocmd-0.3.9/allocmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-04-22 18:43:29.000000 allocmd-0.3.9/allocmd/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:43:41.000000 allocmd-0.3.9/allocmd/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 18:43:29.000000 allocmd-0.3.9/allocmd/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 18:43:29.000000 allocmd-0.3.9/allocmd/utilities/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-22 18:43:29.000000 allocmd-0.3.9/allocmd/utilities/typings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23481 2024-04-22 18:43:29.000000 allocmd-0.3.9/allocmd/utilities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 18:43:41.000000 allocmd-0.3.9/allocmd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-22 18:43:41.000000 allocmd-0.3.9/allocmd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-22 18:43:41.000000 allocmd-0.3.9/allocmd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 18:43:41.000000 allocmd-0.3.9/allocmd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-22 18:43:41.000000 allocmd-0.3.9/allocmd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-22 18:43:41.000000 allocmd-0.3.9/allocmd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 18:43:41.000000 allocmd-0.3.9/allocmd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 18:43:41.000000 allocmd-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-22 18:43:29.000000 allocmd-0.3.9/setup.py
```

### Comparing `allocmd-0.3.8/PKG-INFO` & `allocmd-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allocmd
-Version: 0.3.8
+Version: 0.3.9
 Summary: A CLI tool for creating Allora Chain Worker Nodes
 Home-page: UNKNOWN
 Author: Upshot Technologies
 Author-email: tobi@upshot.xyz
 License: UNKNOWN
 Description: # Building a Worker Node with the allocmd CLI
         ![Docker!](https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white)
```

### Comparing `allocmd-0.3.8/README.md` & `allocmd-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `allocmd-0.3.8/allocmd/cli.py` & `allocmd-0.3.9/allocmd/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,27 +22,27 @@
     """generate scaffolded files and directories depending on the command type passed."""
     pass
 
 @generate.command()
 @click.option('--env', 'environment', required=True, type=click.Choice(['dev', 'prod']), help='Environment to generate for')
 @click.option('--name', required=False, help='Name of the worker.')
 @click.option('--topic', required=False, type=int, help='The topic ID the worker is registered with.')
-def worker(environment, type= BlocklessNodeType.worker, name=None, topic=None):
+def worker(environment, name=None, topic=None):
     """Initialize your Allora Worker Node with necessary boilerplates"""
 
-    blocklessNode(environment, env, type, name, topic)
+    blocklessNode(environment, env, BlocklessNodeType.worker, name, topic)
 
 @generate.command()
 @click.option('--env', 'environment', required=True, type=click.Choice(['dev', 'prod']), help='Environment to generate for')
 @click.option('--name', required=False, help='Name of the reputer.')
 @click.option('--topic', required=False, type=int, help='The topic ID the reputer is registered with.')
-def reputer(environment, type= BlocklessNodeType.reputer, name=None, topic=None):
+def reputer(environment, name=None, topic=None):
     """Initialize your Allora Reputer Node with necessary boilerplates"""
 
-    blocklessNode(environment, env, type, name, topic)
+    blocklessNode(environment, env, BlocklessNodeType.reputer, name, topic)
 
 
 @generate.command()
 @click.option('--name',required=True, help='Name of the validator.')
 @click.option('--network', required=True, type=click.Choice(['testnet', 'edgenet']), help='Your preffered chain network to run the validator on.')
 def validator(name=None, network=None):
     """Initialize your Allora Worker Node with necessary boilerplates"""
```

### Comparing `allocmd-0.3.8/allocmd/utilities/utils.py` & `allocmd-0.3.9/allocmd/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `allocmd-0.3.8/allocmd.egg-info/PKG-INFO` & `allocmd-0.3.9/allocmd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allocmd
-Version: 0.3.8
+Version: 0.3.9
 Summary: A CLI tool for creating Allora Chain Worker Nodes
 Home-page: UNKNOWN
 Author: Upshot Technologies
 Author-email: tobi@upshot.xyz
 License: UNKNOWN
 Description: # Building a Worker Node with the allocmd CLI
         ![Docker!](https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white)
```

### Comparing `allocmd-0.3.8/setup.py` & `allocmd-0.3.9/setup.py`

 * *Files identical despite different names*

