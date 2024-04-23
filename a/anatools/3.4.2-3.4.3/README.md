# Comparing `tmp/anatools-3.4.2.tar.gz` & `tmp/anatools-3.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anatools-3.4.2.tar", last modified: Tue Mar 26 23:31:01 2024, max compression
+gzip compressed data, was "anatools-3.4.3.tar", last modified: Tue Apr 23 23:33:07 2024, max compression
```

## Comparing `anatools-3.4.2.tar` & `anatools-3.4.3.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 23:31:01.441648 anatools-3.4.2/
--rw-rw-rw-   0 root         (0) root         (0)     1072 2024-03-26 23:30:48.000000 anatools-3.4.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-03-26 23:30:48.000000 anatools-3.4.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8010 2024-03-26 23:31:01.441648 anatools-3.4.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7474 2024-03-26 23:30:48.000000 anatools-3.4.2/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 23:31:01.429648 anatools-3.4.2/anatools/
--rw-rw-rw-   0 root         (0) root         (0)      953 2024-03-26 23:30:51.000000 anatools-3.4.2/anatools/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 23:31:01.433648 anatools-3.4.2/anatools/anaclient/
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16050 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/anaclient.py
--rw-rw-rw-   0 root         (0) root         (0)     3581 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/analytics.py
--rw-rw-rw-   0 root         (0) root         (0)     9824 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/annotations.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 23:31:01.433648 anatools-3.4.2/anatools/anaclient/api/
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2910 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/api/analytics.py
--rw-rw-rw-   0 root         (0) root         (0)     8143 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/api/annotations.py
--rw-rw-rw-   0 root         (0) root         (0)     4416 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/api/api.py
--rw-rw-rw-   0 root         (0) root         (0)     3060 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/api/api_keys.py
--rw-rw-rw-   0 root         (0) root         (0)     9040 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/api/channels.py
--rw-rw-rw-   0 root         (0) root         (0)     8002 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/api/datasets.py
--rw-rw-rw-   0 root         (0) root         (0)     8955 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/api/gan.py
--rw-rw-rw-   0 root         (0) root         (0)     4206 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/api/graphs.py
--rw-rw-rw-   0 root         (0) root         (0)     1224 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/api/handlers.py
--rw-rw-rw-   0 root         (0) root         (0)     3133 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/api/llm.py
--rw-rw-rw-   0 root         (0) root         (0)     3679 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/api/members.py
--rw-rw-rw-   0 root         (0) root         (0)     1375 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/api/organizations.py
--rw-rw-rw-   0 root         (0) root         (0)     2440 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/api/umap.py
--rw-rw-rw-   0 root         (0) root         (0)     7519 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/api/volumes.py
--rw-rw-rw-   0 root         (0) root         (0)     3202 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/api/workspaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2401 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/api_keys.py
--rw-rw-rw-   0 root         (0) root         (0)    17769 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/channels.py
--rw-rw-rw-   0 root         (0) root         (0)     9203 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/datasets.py
--rw-rw-rw-   0 root         (0) root         (0)     8397 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/gan.py
--rw-rw-rw-   0 root         (0) root         (0)     6300 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/graphs.py
--rw-rw-rw-   0 root         (0) root         (0)     1980 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/llm.py
--rw-rw-rw-   0 root         (0) root         (0)     7310 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/organizations.py
--rw-rw-rw-   0 root         (0) root         (0)     2033 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/umap.py
--rw-rw-rw-   0 root         (0) root         (0)    16454 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/volumes.py
--rw-rw-rw-   0 root         (0) root         (0)     5827 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anaclient/workspaces.py
--rw-rw-rw-   0 root         (0) root         (0)     5622 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/anacreate.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 23:31:01.437648 anatools-3.4.2/anatools/annotations/
--rw-rw-rw-   0 root         (0) root         (0)       63 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/annotations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7460 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/annotations/annotations.py
--rw-rw-rw-   0 root         (0) root         (0)     3751 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/annotations/convert_coco.py
--rw-rw-rw-   0 root         (0) root         (0)     7173 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/annotations/convert_kitti.py
--rw-rw-rw-   0 root         (0) root         (0)     3381 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/annotations/convert_pascal.py
--rw-rw-rw-   0 root         (0) root         (0)     4468 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/annotations/convert_sagemaker.py
--rw-rw-rw-   0 root         (0) root         (0)     2727 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/annotations/convert_yolo.py
--rw-rw-rw-   0 root         (0) root         (0)     7548 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/annotations/draw.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 23:31:01.437648 anatools-3.4.2/anatools/bin/
--rw-rw-rw-   0 root         (0) root         (0)     4523 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/bin/ana
--rw-rw-rw-   0 root         (0) root         (0)     9659 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/bin/anadeploy
--rw-rw-rw-   0 root         (0) root         (0)     7692 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/bin/anamount
--rw-rw-rw-   0 root         (0) root         (0)     4935 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/bin/anautils
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 23:31:01.437648 anatools-3.4.2/anatools/lib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6974 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/lib/ana_object.py
--rw-rw-rw-   0 root         (0) root         (0)     7114 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/lib/bbox.py
--rw-rw-rw-   0 root         (0) root         (0)     2149 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/lib/blender_main.py
--rw-rw-rw-   0 root         (0) root         (0)     4923 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/lib/camera_checks.py
--rw-rw-rw-   0 root         (0) root         (0)    14524 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/lib/channel.py
--rw-rw-rw-   0 root         (0) root         (0)     1777 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/lib/context.py
--rw-rw-rw-   0 root         (0) root         (0)     1490 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/lib/directory_object.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/lib/download.py
--rw-rw-rw-   0 root         (0) root         (0)     4198 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/lib/file_handlers.py
--rw-rw-rw-   0 root         (0) root         (0)     1308 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/lib/file_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)      748 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/lib/file_object.py
--rw-rw-rw-   0 root         (0) root         (0)     9556 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/lib/generator.py
--rw-rw-rw-   0 root         (0) root         (0)     5670 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/lib/interp.py
--rw-rw-rw-   0 root         (0) root         (0)     2244 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/lib/load.py
--rw-rw-rw-   0 root         (0) root         (0)    10556 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/lib/node.py
--rw-rw-rw-   0 root         (0) root         (0)     1430 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/lib/object_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1702 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/lib/package_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      209 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/lib/print.py
--rw-rw-rw-   0 root         (0) root         (0)     1918 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/lib/python_main.py
--rw-rw-rw-   0 root         (0) root         (0)     3200 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/lib/rigged_object.py
--rw-rw-rw-   0 root         (0) root         (0)     8111 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/lib/scene.py
--rw-rw-rw-   0 root         (0) root         (0)     3757 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/lib/search_utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 23:31:01.441648 anatools-3.4.2/anatools/nodes/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/nodes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1115 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/nodes/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1228 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/nodes/constants.yml
--rw-rw-rw-   0 root         (0) root         (0)     2635 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/nodes/generators.py
--rw-rw-rw-   0 root         (0) root         (0)     2183 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/nodes/generators.yml
--rw-rw-rw-   0 root         (0) root         (0)     1592 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/nodes/logic.py
--rw-rw-rw-   0 root         (0) root         (0)     1567 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/nodes/logic.yml
--rw-rw-rw-   0 root         (0) root         (0)     5381 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/nodes/random_generator.py
--rw-rw-rw-   0 root         (0) root         (0)     8429 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/nodes/random_generator.yml
--rw-rw-rw-   0 root         (0) root         (0)     1321 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/nodes/sweep_arange.py
--rw-rw-rw-   0 root         (0) root         (0)     1509 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/nodes/sweep_arange.yml
--rw-rw-rw-   0 root         (0) root         (0)     1306 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/nodes/sweep_linspace.py
--rw-rw-rw-   0 root         (0) root         (0)     1549 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/nodes/sweep_linspace.yml
--rw-rw-rw-   0 root         (0) root         (0)     1224 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/nodes/vectors.py
--rw-rw-rw-   0 root         (0) root         (0)     1922 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/nodes/vectors.yml
--rw-rw-rw-   0 root         (0) root         (0)     1246 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/nodes/volume_directory.py
--rw-rw-rw-   0 root         (0) root         (0)      901 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/nodes/volume_directory.yml
--rw-rw-rw-   0 root         (0) root         (0)      557 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/nodes/volume_file.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2024-03-26 23:30:48.000000 anatools-3.4.2/anatools/nodes/volume_file.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-26 23:31:01.441648 anatools-3.4.2/anatools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8010 2024-03-26 23:31:01.000000 anatools-3.4.2/anatools.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2844 2024-03-26 23:31:01.000000 anatools-3.4.2/anatools.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-26 23:31:01.000000 anatools-3.4.2/anatools.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       54 2024-03-26 23:31:01.000000 anatools-3.4.2/anatools.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)       72 2024-03-26 23:31:01.000000 anatools-3.4.2/anatools.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2024-03-26 23:31:01.000000 anatools-3.4.2/anatools.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      103 2024-03-26 23:30:48.000000 anatools-3.4.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       71 2024-03-26 23:30:48.000000 anatools-3.4.2/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-03-26 23:31:01.441648 anatools-3.4.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1230 2024-03-26 23:30:48.000000 anatools-3.4.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-23 23:33:07.820212 anatools-3.4.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2024-04-23 23:32:44.000000 anatools-3.4.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-04-23 23:32:44.000000 anatools-3.4.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8010 2024-04-23 23:33:07.820212 anatools-3.4.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7474 2024-04-23 23:32:44.000000 anatools-3.4.3/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-23 23:33:07.804212 anatools-3.4.3/anatools/
+-rw-rw-rw-   0 root         (0) root         (0)      953 2024-04-23 23:32:49.000000 anatools-3.4.3/anatools/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-23 23:33:07.812212 anatools-3.4.3/anatools/anaclient/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16050 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/anaclient.py
+-rw-rw-rw-   0 root         (0) root         (0)     3581 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/analytics.py
+-rw-rw-rw-   0 root         (0) root         (0)     9824 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/annotations.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-23 23:33:07.812212 anatools-3.4.3/anatools/anaclient/api/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2910 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/api/analytics.py
+-rw-rw-rw-   0 root         (0) root         (0)     8143 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/api/annotations.py
+-rw-rw-rw-   0 root         (0) root         (0)     4416 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/api/api.py
+-rw-rw-rw-   0 root         (0) root         (0)     3060 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/api/api_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)     9040 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/api/channels.py
+-rw-rw-rw-   0 root         (0) root         (0)     8002 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/api/datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)     8955 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/api/gan.py
+-rw-rw-rw-   0 root         (0) root         (0)     4206 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/api/graphs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1224 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/api/handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)     3133 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/api/llm.py
+-rw-rw-rw-   0 root         (0) root         (0)     3679 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/api/members.py
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/api/organizations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2440 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/api/umap.py
+-rw-rw-rw-   0 root         (0) root         (0)     7519 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/api/volumes.py
+-rw-rw-rw-   0 root         (0) root         (0)     3202 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/api/workspaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2401 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/api_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)    17769 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/channels.py
+-rw-rw-rw-   0 root         (0) root         (0)     9203 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)     8397 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/gan.py
+-rw-rw-rw-   0 root         (0) root         (0)     6300 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/graphs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1980 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/llm.py
+-rw-rw-rw-   0 root         (0) root         (0)     7310 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/organizations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2033 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/umap.py
+-rw-rw-rw-   0 root         (0) root         (0)    16454 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/volumes.py
+-rw-rw-rw-   0 root         (0) root         (0)     5827 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anaclient/workspaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     5622 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/anacreate.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-23 23:33:07.812212 anatools-3.4.3/anatools/annotations/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/annotations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7460 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/annotations/annotations.py
+-rw-rw-rw-   0 root         (0) root         (0)     4331 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/annotations/convert_coco.py
+-rw-rw-rw-   0 root         (0) root         (0)     7173 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/annotations/convert_kitti.py
+-rw-rw-rw-   0 root         (0) root         (0)     3381 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/annotations/convert_pascal.py
+-rw-rw-rw-   0 root         (0) root         (0)     4468 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/annotations/convert_sagemaker.py
+-rw-rw-rw-   0 root         (0) root         (0)     2727 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/annotations/convert_yolo.py
+-rw-rw-rw-   0 root         (0) root         (0)     7548 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/annotations/draw.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-23 23:33:07.816212 anatools-3.4.3/anatools/bin/
+-rw-rw-rw-   0 root         (0) root         (0)     4523 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/bin/ana
+-rw-rw-rw-   0 root         (0) root         (0)     9659 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/bin/anadeploy
+-rw-rw-rw-   0 root         (0) root         (0)     7692 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/bin/anamount
+-rw-rw-rw-   0 root         (0) root         (0)     4935 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/bin/anautils
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-23 23:33:07.816212 anatools-3.4.3/anatools/lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6974 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/lib/ana_object.py
+-rw-rw-rw-   0 root         (0) root         (0)     7114 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/lib/bbox.py
+-rw-rw-rw-   0 root         (0) root         (0)     2149 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/lib/blender_main.py
+-rw-rw-rw-   0 root         (0) root         (0)     4923 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/lib/camera_checks.py
+-rw-rw-rw-   0 root         (0) root         (0)    14524 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/lib/channel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1777 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/lib/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     1490 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/lib/directory_object.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/lib/download.py
+-rw-rw-rw-   0 root         (0) root         (0)     4198 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/lib/file_handlers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1308 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/lib/file_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)      748 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/lib/file_object.py
+-rw-rw-rw-   0 root         (0) root         (0)     9556 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/lib/generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     5670 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/lib/interp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2244 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/lib/load.py
+-rw-rw-rw-   0 root         (0) root         (0)    10556 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/lib/node.py
+-rw-rw-rw-   0 root         (0) root         (0)     1430 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/lib/object_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1702 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/lib/package_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      209 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/lib/print.py
+-rw-rw-rw-   0 root         (0) root         (0)     1918 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/lib/python_main.py
+-rw-rw-rw-   0 root         (0) root         (0)     3200 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/lib/rigged_object.py
+-rw-rw-rw-   0 root         (0) root         (0)     8111 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/lib/scene.py
+-rw-rw-rw-   0 root         (0) root         (0)     3757 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/lib/search_utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-23 23:33:07.820212 anatools-3.4.3/anatools/nodes/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/nodes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/nodes/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1228 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/nodes/constants.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2635 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/nodes/generators.py
+-rw-rw-rw-   0 root         (0) root         (0)     2183 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/nodes/generators.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1592 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/nodes/logic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/nodes/logic.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5381 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/nodes/random_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)     8429 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/nodes/random_generator.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1321 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/nodes/sweep_arange.py
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/nodes/sweep_arange.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1306 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/nodes/sweep_linspace.py
+-rw-rw-rw-   0 root         (0) root         (0)     1549 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/nodes/sweep_linspace.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1224 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/nodes/vectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1922 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/nodes/vectors.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1246 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/nodes/volume_directory.py
+-rw-rw-rw-   0 root         (0) root         (0)      901 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/nodes/volume_directory.yml
+-rw-rw-rw-   0 root         (0) root         (0)      557 2024-04-23 23:32:44.000000 anatools-3.4.3/anatools/nodes/volume_file.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-04-23 23:32:45.000000 anatools-3.4.3/anatools/nodes/volume_file.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-23 23:33:07.820212 anatools-3.4.3/anatools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8010 2024-04-23 23:33:07.000000 anatools-3.4.3/anatools.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2844 2024-04-23 23:33:07.000000 anatools-3.4.3/anatools.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-23 23:33:07.000000 anatools-3.4.3/anatools.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       54 2024-04-23 23:33:07.000000 anatools-3.4.3/anatools.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)       72 2024-04-23 23:33:07.000000 anatools-3.4.3/anatools.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2024-04-23 23:33:07.000000 anatools-3.4.3/anatools.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-04-23 23:32:45.000000 anatools-3.4.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       71 2024-04-23 23:32:45.000000 anatools-3.4.3/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-23 23:33:07.820212 anatools-3.4.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2024-04-23 23:32:45.000000 anatools-3.4.3/setup.py
```

### Comparing `anatools-3.4.2/LICENSE` & `anatools-3.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/PKG-INFO` & `anatools-3.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anatools
-Version: 3.4.2
+Version: 3.4.3
 Summary: Tools for development with the Rendered.ai Platform.
 Home-page: https://rendered.ai
 Author: Rendered AI, Inc
 Author-email: support@rendered.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

### Comparing `anatools-3.4.2/README.md` & `anatools-3.4.3/README.md`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/__init__.py` & `anatools-3.4.3/anatools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,8 @@
         https://support.rendered.ai/gc/Introduction-to-Rendered.ai.1577812005.html
 
 """
 
 from .anaclient.anaclient import client
 from .annotations.annotations import annotations
 
-__version__ = '3.4.2'
+__version__ = '3.4.3'
```

### Comparing `anatools-3.4.2/anatools/anaclient/anaclient.py` & `anatools-3.4.3/anatools/anaclient/anaclient.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/anaclient/analytics.py` & `anatools-3.4.3/anatools/anaclient/analytics.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/anaclient/annotations.py` & `anatools-3.4.3/anatools/anaclient/annotations.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/anaclient/api/analytics.py` & `anatools-3.4.3/anatools/anaclient/api/analytics.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/anaclient/api/annotations.py` & `anatools-3.4.3/anatools/anaclient/api/annotations.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/anaclient/api/api.py` & `anatools-3.4.3/anatools/anaclient/api/api.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/anaclient/api/api_keys.py` & `anatools-3.4.3/anatools/anaclient/api/api_keys.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/anaclient/api/channels.py` & `anatools-3.4.3/anatools/anaclient/api/channels.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/anaclient/api/datasets.py` & `anatools-3.4.3/anatools/anaclient/api/datasets.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/anaclient/api/gan.py` & `anatools-3.4.3/anatools/anaclient/api/gan.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/anaclient/api/graphs.py` & `anatools-3.4.3/anatools/anaclient/api/graphs.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/anaclient/api/handlers.py` & `anatools-3.4.3/anatools/anaclient/api/handlers.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/anaclient/api/llm.py` & `anatools-3.4.3/anatools/anaclient/api/llm.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/anaclient/api/members.py` & `anatools-3.4.3/anatools/anaclient/api/members.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/anaclient/api/organizations.py` & `anatools-3.4.3/anatools/anaclient/api/organizations.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/anaclient/api/umap.py` & `anatools-3.4.3/anatools/anaclient/api/umap.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/anaclient/api/volumes.py` & `anatools-3.4.3/anatools/anaclient/api/volumes.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/anaclient/api/workspaces.py` & `anatools-3.4.3/anatools/anaclient/api/workspaces.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/anaclient/api_keys.py` & `anatools-3.4.3/anatools/anaclient/api_keys.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/anaclient/channels.py` & `anatools-3.4.3/anatools/anaclient/channels.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/anaclient/datasets.py` & `anatools-3.4.3/anatools/anaclient/datasets.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/anaclient/gan.py` & `anatools-3.4.3/anatools/anaclient/gan.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/anaclient/graphs.py` & `anatools-3.4.3/anatools/anaclient/graphs.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/anaclient/llm.py` & `anatools-3.4.3/anatools/anaclient/llm.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/anaclient/organizations.py` & `anatools-3.4.3/anatools/anaclient/organizations.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/anaclient/umap.py` & `anatools-3.4.3/anatools/anaclient/umap.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/anaclient/volumes.py` & `anatools-3.4.3/anatools/anaclient/volumes.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/anaclient/workspaces.py` & `anatools-3.4.3/anatools/anaclient/workspaces.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/anacreate.py` & `anatools-3.4.3/anatools/anacreate.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/annotations/annotations.py` & `anatools-3.4.3/anatools/annotations/annotations.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/annotations/convert_coco.py` & `anatools-3.4.3/anatools/annotations/convert_coco.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,77 +15,85 @@
         "date_created": datetime.datetime.now().isoformat()}
     cocodata['licenses'] = [{
         "id":   0,
         "url":  "https://rendered.ai/",     # "url": "https://creativecommons.org/licenses/by-nc-nd/4.0/",
         "name": "Rendered.AI License"}]     # "name": "Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License"}]
     cocodata['images'] = list()
     cocodata['categories'] = list()
-    cocodata['annotations'] = list()
     return cocodata
 
 
 def convert_coco(datadir, outdir, mapping):
 
     annsdir = os.path.join(datadir, "annotations")
     metadir = os.path.join(datadir, "metadata")
     imgdir = os.path.join(datadir, "images")
     annsfiles = os.listdir(annsdir)
     
     cocodata = create_cocodata()
-    annotations = []
-    categories = []
     cats = {}
     imgid = 0
     annid = 0
-        
-     # for each interpretation, gather annotations and map categories
-    for f in sorted(annsfiles):
-        if not f.endswith('.json'):
-            continue
-        with open(os.path.join(annsdir,f), 'r') as af: anns = json.load(af)
-        with open(os.path.join(metadir,f.replace('ana','metadata')), 'r') as mf: metadata = json.load(mf)
-        
-        # for each object in the metadata file, check if any of the properties are true
-        for obj in metadata['objects']:
-            for prop in mapping['properties']:
-                if eval(prop):
-                    for ann in anns['annotations']:
-                        if ann['id'] == obj['id']: 
-                            class_num = mapping['properties'][prop]
-                            cats[class_num] = mapping['classes'][class_num]
-                            annotation = {}
-                            annotation['id'] = annid
-                            annotation['image_id'] = imgid
-                            annotation['category_id'] = class_num
-                            annotation['segmentation'] = ann['segmentation']
-                            annotation['area'] = ann['bbox'][2] * ann['bbox'][3]
-                            annotation['bbox'] = ann['bbox']
-                            annotation['iscrowd'] = 0
-                            annid += 1
-                            cocodata['annotations'].append(annotation)
-                            break
-        imgdata = {
-            'id':               imgid, 
-            'file_name':        metadata['filename'], 
-            'date_captured':    metadata['date'], 
-            'license':          0 }
-        if 'sensor' in metadata:
-            imgdata['width'] =  metadata['sensor']['resolution'][0]
-            imgdata['height']=  metadata['sensor']['resolution'][1]
-            if 'frame' in metadata['sensor']: metadata['frame'] = metadata['sensor']['frame']
-        else:
-            im = Image.open(os.path.join(imgdir, anns['filename']))
-            width, height = im.size
-            imgdata['width'] =  width
-            imgdata['height']=  height
-        cocodata['images'].append(imgdata)
-        imgid += 1
-    sorted_cats = dict(sorted(cats.items()))
-    for class_num, cat in sorted_cats.items():
-        cocodata['categories'].append({
-            'id':               class_num, 
-            'name':             cat[-1],
-            'supercategory':    cat[0]
-        })
 
     with open(os.path.join(outdir,'coco.json'), 'w+') as of:
-        json.dump(cocodata,of)
+        of.write('{"annotations": [')
+        first = True
+
+        # for each interpretation, gather annotations and map categories
+        for f in sorted(annsfiles):
+            if not f.endswith('.json'):
+                continue
+            with open(os.path.join(annsdir,f), 'r') as af: anns = json.load(af)
+            with open(os.path.join(metadir,f.replace('ana','metadata')), 'r') as mf: metadata = json.load(mf)
+            
+            # for each object in the metadata file, check if any of the properties are true
+            for obj in metadata['objects']:
+                for prop in mapping['properties']:
+                    if eval(prop):
+                        for ann in anns['annotations']:
+                            if ann['id'] == obj['id']: 
+                                class_num = mapping['properties'][prop]
+                                cats[class_num] = mapping['classes'][class_num]
+                                annotation = {}
+                                annotation['id'] = annid
+                                annotation['image_id'] = imgid
+                                annotation['category_id'] = class_num
+                                annotation['segmentation'] = ann['segmentation']
+                                annotation['area'] = ann['bbox'][2] * ann['bbox'][3]
+                                annotation['bbox'] = ann['bbox']
+                                annotation['iscrowd'] = 0
+                                annid += 1
+                                if not first:
+                                    of.write(', ')
+                                json.dump(annotation, of)
+                                first = False
+                                break
+            imgdata = {
+                'id':               imgid, 
+                'file_name':        metadata['filename'], 
+                'date_captured':    metadata['date'], 
+                'license':          0 }
+            if 'sensor' in metadata:
+                imgdata['width'] =  metadata['sensor']['resolution'][0]
+                imgdata['height']=  metadata['sensor']['resolution'][1]
+                if 'frame' in metadata['sensor']: metadata['frame'] = metadata['sensor']['frame']
+            else:
+                im = Image.open(os.path.join(imgdir, anns['filename']))
+                width, height = im.size
+                imgdata['width'] =  width
+                imgdata['height']=  height
+            cocodata['images'].append(imgdata)
+            imgid += 1
+        sorted_cats = dict(sorted(cats.items()))
+        for class_num, cat in sorted_cats.items():
+            cocodata['categories'].append({
+                'id':               class_num, 
+                'name':             cat[-1],
+                'supercategory':    cat[0]
+            })
+
+        of.write('], ')
+        of.write(f'"info": {json.dumps(cocodata["info"])}, ')
+        of.write(f'"licenses": {json.dumps(cocodata["licenses"])}, ')
+        of.write(f'"images": {json.dumps(cocodata["images"])}, ')
+        of.write(f'"categories": {json.dumps(cocodata["categories"])}')
+        of.write('}')
```

### Comparing `anatools-3.4.2/anatools/annotations/convert_kitti.py` & `anatools-3.4.3/anatools/annotations/convert_kitti.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/annotations/convert_pascal.py` & `anatools-3.4.3/anatools/annotations/convert_pascal.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/annotations/convert_sagemaker.py` & `anatools-3.4.3/anatools/annotations/convert_sagemaker.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/annotations/convert_yolo.py` & `anatools-3.4.3/anatools/annotations/convert_yolo.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/annotations/draw.py` & `anatools-3.4.3/anatools/annotations/draw.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/bin/ana` & `anatools-3.4.3/anatools/bin/ana`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/bin/anadeploy` & `anatools-3.4.3/anatools/bin/anadeploy`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/bin/anamount` & `anatools-3.4.3/anatools/bin/anamount`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/bin/anautils` & `anatools-3.4.3/anatools/bin/anautils`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/lib/ana_object.py` & `anatools-3.4.3/anatools/lib/ana_object.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/lib/bbox.py` & `anatools-3.4.3/anatools/lib/bbox.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/lib/blender_main.py` & `anatools-3.4.3/anatools/lib/blender_main.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/lib/camera_checks.py` & `anatools-3.4.3/anatools/lib/camera_checks.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/lib/channel.py` & `anatools-3.4.3/anatools/lib/channel.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/lib/context.py` & `anatools-3.4.3/anatools/lib/context.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/lib/directory_object.py` & `anatools-3.4.3/anatools/lib/directory_object.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/lib/file_handlers.py` & `anatools-3.4.3/anatools/lib/file_handlers.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/lib/file_metadata.py` & `anatools-3.4.3/anatools/lib/file_metadata.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/lib/file_object.py` & `anatools-3.4.3/anatools/lib/file_object.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/lib/generator.py` & `anatools-3.4.3/anatools/lib/generator.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/lib/interp.py` & `anatools-3.4.3/anatools/lib/interp.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/lib/load.py` & `anatools-3.4.3/anatools/lib/load.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/lib/node.py` & `anatools-3.4.3/anatools/lib/node.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/lib/object_utils.py` & `anatools-3.4.3/anatools/lib/object_utils.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/lib/package_utils.py` & `anatools-3.4.3/anatools/lib/package_utils.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/lib/python_main.py` & `anatools-3.4.3/anatools/lib/python_main.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/lib/rigged_object.py` & `anatools-3.4.3/anatools/lib/rigged_object.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/lib/scene.py` & `anatools-3.4.3/anatools/lib/scene.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/lib/search_utils.py` & `anatools-3.4.3/anatools/lib/search_utils.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/nodes/constants.py` & `anatools-3.4.3/anatools/nodes/constants.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/nodes/constants.yml` & `anatools-3.4.3/anatools/nodes/constants.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/nodes/generators.py` & `anatools-3.4.3/anatools/nodes/generators.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/nodes/generators.yml` & `anatools-3.4.3/anatools/nodes/generators.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/nodes/logic.py` & `anatools-3.4.3/anatools/nodes/logic.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/nodes/logic.yml` & `anatools-3.4.3/anatools/nodes/logic.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/nodes/random_generator.py` & `anatools-3.4.3/anatools/nodes/random_generator.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/nodes/random_generator.yml` & `anatools-3.4.3/anatools/nodes/random_generator.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/nodes/sweep_arange.py` & `anatools-3.4.3/anatools/nodes/sweep_arange.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/nodes/sweep_arange.yml` & `anatools-3.4.3/anatools/nodes/sweep_arange.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/nodes/sweep_linspace.py` & `anatools-3.4.3/anatools/nodes/sweep_linspace.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/nodes/sweep_linspace.yml` & `anatools-3.4.3/anatools/nodes/sweep_linspace.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/nodes/vectors.py` & `anatools-3.4.3/anatools/nodes/vectors.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/nodes/vectors.yml` & `anatools-3.4.3/anatools/nodes/vectors.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/nodes/volume_directory.py` & `anatools-3.4.3/anatools/nodes/volume_directory.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/nodes/volume_directory.yml` & `anatools-3.4.3/anatools/nodes/volume_directory.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/nodes/volume_file.py` & `anatools-3.4.3/anatools/nodes/volume_file.py`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools/nodes/volume_file.yml` & `anatools-3.4.3/anatools/nodes/volume_file.yml`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/anatools.egg-info/PKG-INFO` & `anatools-3.4.3/anatools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anatools
-Version: 3.4.2
+Version: 3.4.3
 Summary: Tools for development with the Rendered.ai Platform.
 Home-page: https://rendered.ai
 Author: Rendered AI, Inc
 Author-email: support@rendered.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
```

### Comparing `anatools-3.4.2/anatools.egg-info/SOURCES.txt` & `anatools-3.4.3/anatools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anatools-3.4.2/setup.py` & `anatools-3.4.3/setup.py`

 * *Files identical despite different names*

