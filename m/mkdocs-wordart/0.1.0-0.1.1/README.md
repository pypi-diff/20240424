# Comparing `tmp/mkdocs-wordart-0.1.0.tar.gz` & `tmp/mkdocs_wordart-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-wordart-0.1.0.tar", last modified: Wed Apr  3 15:33:27 2024, max compression
+gzip compressed data, was "mkdocs_wordart-0.1.1.tar", last modified: Wed Apr 24 14:15:37 2024, max compression
```

## Comparing `mkdocs-wordart-0.1.0.tar` & `mkdocs_wordart-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:33:27.480343 mkdocs-wordart-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-03 15:33:16.000000 mkdocs-wordart-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-03 15:33:27.480343 mkdocs-wordart-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-03 15:33:16.000000 mkdocs-wordart-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-03 15:33:16.000000 mkdocs-wordart-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 15:33:27.480343 mkdocs-wordart-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:33:27.476343 mkdocs-wordart-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:33:27.480343 mkdocs-wordart-0.1.0/src/mkdocs_wordart/
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-03 15:33:16.000000 mkdocs-wordart-0.1.0/src/mkdocs_wordart/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:33:27.480343 mkdocs-wordart-0.1.0/src/mkdocs_wordart.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-03 15:33:27.000000 mkdocs-wordart-0.1.0/src/mkdocs_wordart.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-03 15:33:27.000000 mkdocs-wordart-0.1.0/src/mkdocs_wordart.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:33:27.000000 mkdocs-wordart-0.1.0/src/mkdocs_wordart.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-03 15:33:27.000000 mkdocs-wordart-0.1.0/src/mkdocs_wordart.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 15:33:27.000000 mkdocs-wordart-0.1.0/src/mkdocs_wordart.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 15:33:27.000000 mkdocs-wordart-0.1.0/src/mkdocs_wordart.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:15:37.080925 mkdocs_wordart-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 14:15:27.000000 mkdocs_wordart-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-24 14:15:27.000000 mkdocs_wordart-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-24 14:15:37.080925 mkdocs_wordart-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-24 14:15:27.000000 mkdocs_wordart-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-24 14:15:27.000000 mkdocs_wordart-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 14:15:37.080925 mkdocs_wordart-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:15:37.076925 mkdocs_wordart-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:15:37.076925 mkdocs_wordart-0.1.1/src/mkdocs_wordart/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:15:37.076925 mkdocs_wordart-0.1.1/src/mkdocs_wordart/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   243780 2024-04-24 14:15:27.000000 mkdocs_wordart-0.1.1/src/mkdocs_wordart/assets/wordart.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-24 14:15:27.000000 mkdocs_wordart-0.1.1/src/mkdocs_wordart/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:15:37.080925 mkdocs_wordart-0.1.1/src/mkdocs_wordart/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-24 14:15:27.000000 mkdocs_wordart-0.1.1/src/mkdocs_wordart/templates/wordart.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:15:37.080925 mkdocs_wordart-0.1.1/src/mkdocs_wordart.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-24 14:15:37.000000 mkdocs_wordart-0.1.1/src/mkdocs_wordart.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-24 14:15:37.000000 mkdocs_wordart-0.1.1/src/mkdocs_wordart.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:15:37.000000 mkdocs_wordart-0.1.1/src/mkdocs_wordart.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-24 14:15:37.000000 mkdocs_wordart-0.1.1/src/mkdocs_wordart.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 14:15:37.000000 mkdocs_wordart-0.1.1/src/mkdocs_wordart.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-24 14:15:37.000000 mkdocs_wordart-0.1.1/src/mkdocs_wordart.egg-info/top_level.txt
```

### Comparing `mkdocs-wordart-0.1.0/LICENSE` & `mkdocs_wordart-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-wordart-0.1.0/PKG-INFO` & `mkdocs_wordart-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-wordart
-Version: 0.1.0
+Version: 0.1.1
 Summary: A MkDocs plugin that makes wordart available again.
 Author-email: Useless DevLab <useless.devlab@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Useless DevLab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mkdocs-wordart-0.1.0/pyproject.toml` & `mkdocs_wordart-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mkdocs-wordart"
-version = "0.1.0"
+version = "0.1.1"
 description = "A MkDocs plugin that makes wordart available again."
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["mkdocs", "documentation", "wordart"]
 authors = [
   {name = "Useless DevLab", email = "useless.devlab@gmail.com"}
 ]
```

### Comparing `mkdocs-wordart-0.1.0/src/mkdocs_wordart/plugin.py` & `mkdocs_wordart-0.1.1/src/mkdocs_wordart/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-wordart-0.1.0/src/mkdocs_wordart.egg-info/PKG-INFO` & `mkdocs_wordart-0.1.1/src/mkdocs_wordart.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-wordart
-Version: 0.1.0
+Version: 0.1.1
 Summary: A MkDocs plugin that makes wordart available again.
 Author-email: Useless DevLab <useless.devlab@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Useless DevLab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

