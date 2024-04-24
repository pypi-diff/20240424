# Comparing `tmp/cook_builder-0.1.2.tar.gz` & `tmp/cook_builder-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cook_builder-0.1.2.tar", last modified: Tue Apr 23 18:17:07 2024, max compression
+gzip compressed data, was "cook_builder-0.1.3.tar", last modified: Tue Apr 23 18:59:54 2024, max compression
```

## Comparing `cook_builder-0.1.2.tar` & `cook_builder-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-23 18:17:07.876594 cook_builder-0.1.2/
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1072 2024-02-10 12:14:36.000000 cook_builder-0.1.2/LICENSE
--rw-r--r--   0 seweryn   (1000) seweryn   (1000)     3006 2024-04-23 18:17:07.876594 cook_builder-0.1.2/PKG-INFO
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      877 2024-04-19 18:55:28.000000 cook_builder-0.1.2/README.md
-drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-23 18:17:07.876594 cook_builder-0.1.2/cook/
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       35 2024-04-20 08:35:09.000000 cook_builder-0.1.2/cook/__init__.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1204 2024-04-20 08:24:26.000000 cook_builder-0.1.2/cook/build.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2609 2024-04-23 18:16:32.000000 cook_builder-0.1.2/cook/cli.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     4851 2024-04-20 08:51:37.000000 cook_builder-0.1.2/cook/configuration.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     3050 2024-04-22 20:22:09.000000 cook_builder-0.1.2/cook/cook.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      150 2024-04-16 14:39:30.000000 cook_builder-0.1.2/cook/exception.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2407 2024-04-23 16:22:15.000000 cook_builder-0.1.2/cook/executors.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      984 2024-04-22 20:26:52.000000 cook_builder-0.1.2/cook/logger.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1840 2024-04-23 18:11:15.000000 cook_builder-0.1.2/cook/main.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1030 2024-04-22 19:33:15.000000 cook_builder-0.1.2/cook/recipe.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2310 2024-04-22 20:00:03.000000 cook_builder-0.1.2/cook/rsync.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1383 2024-04-20 08:25:29.000000 cook_builder-0.1.2/cook/sync.py
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      381 2024-04-20 09:09:37.000000 cook_builder-0.1.2/cook/watchers.py
-drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-23 18:17:07.876594 cook_builder-0.1.2/cook_builder.egg-info/
--rw-r--r--   0 seweryn   (1000) seweryn   (1000)     3006 2024-04-23 18:17:07.000000 cook_builder-0.1.2/cook_builder.egg-info/PKG-INFO
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      451 2024-04-23 18:17:07.000000 cook_builder-0.1.2/cook_builder.egg-info/SOURCES.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        1 2024-04-23 18:17:07.000000 cook_builder-0.1.2/cook_builder.egg-info/dependency_links.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       38 2024-04-23 18:17:07.000000 cook_builder-0.1.2/cook_builder.egg-info/entry_points.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       27 2024-04-23 18:17:07.000000 cook_builder-0.1.2/cook_builder.egg-info/requires.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        5 2024-04-23 18:17:07.000000 cook_builder-0.1.2/cook_builder.egg-info/top_level.txt
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1141 2024-04-23 18:16:47.000000 cook_builder-0.1.2/pyproject.toml
--rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       38 2024-04-23 18:17:07.876594 cook_builder-0.1.2/setup.cfg
+drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-23 18:59:54.512913 cook_builder-0.1.3/
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1072 2024-02-10 12:14:36.000000 cook_builder-0.1.3/LICENSE
+-rw-r--r--   0 seweryn   (1000) seweryn   (1000)     3040 2024-04-23 18:59:54.512913 cook_builder-0.1.3/PKG-INFO
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      877 2024-04-19 18:55:28.000000 cook_builder-0.1.3/README.md
+drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-23 18:59:54.512913 cook_builder-0.1.3/cook/
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       36 2024-04-23 18:58:25.000000 cook_builder-0.1.3/cook/__init__.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1204 2024-04-20 08:24:26.000000 cook_builder-0.1.3/cook/build.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     3023 2024-04-23 18:57:39.000000 cook_builder-0.1.3/cook/cli.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     4851 2024-04-20 08:51:37.000000 cook_builder-0.1.3/cook/configuration.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     3050 2024-04-22 20:22:09.000000 cook_builder-0.1.3/cook/cook.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      150 2024-04-16 14:39:30.000000 cook_builder-0.1.3/cook/exception.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2407 2024-04-23 16:22:15.000000 cook_builder-0.1.3/cook/executors.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      985 2024-04-23 18:19:22.000000 cook_builder-0.1.3/cook/logger.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2170 2024-04-23 18:36:05.000000 cook_builder-0.1.3/cook/main.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1030 2024-04-22 19:33:15.000000 cook_builder-0.1.3/cook/recipe.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     2310 2024-04-22 20:00:03.000000 cook_builder-0.1.3/cook/rsync.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1383 2024-04-20 08:25:29.000000 cook_builder-0.1.3/cook/sync.py
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      381 2024-04-20 09:09:37.000000 cook_builder-0.1.3/cook/watchers.py
+drwxrwxr-x   0 seweryn   (1000) seweryn   (1000)        0 2024-04-23 18:59:54.512913 cook_builder-0.1.3/cook_builder.egg-info/
+-rw-r--r--   0 seweryn   (1000) seweryn   (1000)     3040 2024-04-23 18:59:54.000000 cook_builder-0.1.3/cook_builder.egg-info/PKG-INFO
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)      451 2024-04-23 18:59:54.000000 cook_builder-0.1.3/cook_builder.egg-info/SOURCES.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        1 2024-04-23 18:59:54.000000 cook_builder-0.1.3/cook_builder.egg-info/dependency_links.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       38 2024-04-23 18:59:54.000000 cook_builder-0.1.3/cook_builder.egg-info/entry_points.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       46 2024-04-23 18:59:54.000000 cook_builder-0.1.3/cook_builder.egg-info/requires.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)        5 2024-04-23 18:59:54.000000 cook_builder-0.1.3/cook_builder.egg-info/top_level.txt
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)     1165 2024-04-23 18:59:38.000000 cook_builder-0.1.3/pyproject.toml
+-rw-rw-r--   0 seweryn   (1000) seweryn   (1000)       38 2024-04-23 18:59:54.512913 cook_builder-0.1.3/setup.cfg
```

### Comparing `cook_builder-0.1.2/LICENSE` & `cook_builder-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.2/PKG-INFO` & `cook_builder-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cook_builder
-Version: 0.1.2
+Version: 0.1.3
 Summary: Build script aggregator and remote executor
 Author: Seweryn Rusecki
 License: MIT License
         
         Copyright (c) 2024 Seweryn Rusecki
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,14 +38,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fabric==3.2.2
 Requires-Dist: rich==13.7.1
+Requires-Dist: questionary==2.0.1
 
 # Cook
 
 Build script aggregator and remote executor.
 
 # Getting started
```

### Comparing `cook_builder-0.1.2/README.md` & `cook_builder-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.2/cook/build.py` & `cook_builder-0.1.3/cook/build.py`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.2/cook/cli.py` & `cook_builder-0.1.3/cook/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import argparse
 import pathlib
 
+import questionary
+
 from .main import Main
 
 
 class Settings:
     def __init__(self):
         self.args = {}
         self.flags = []
@@ -40,16 +42,19 @@
 
     parser.add_argument('-r', '--recipe_path', default='.', help='Path to directory containing `recipe.py` file.')
     parser.add_argument('-b', '--build_server', help='Build server to use. Uses value of `default_build_server` if left unspecified.')
     parser.add_argument('-f', '--format', action='store_true', help='Format output using Rich.')
     parser.add_argument('-t', '--targets', action='store_true', help='List available projects.')
     parser.add_argument('-d', '--dry', action='store_true', help='Dry run.')
     parser.add_argument('-q', '--quiet', action='store_true', help='Suppress stdout.')
-    parser.add_argument('-u', '--user_args', nargs='*', default=[], help='User arguments. Can be used in recipe file. Format either `key=value` or `flag`.')
+    parser.add_argument(
+        '-u', '--user_args', nargs='*', default=[], help='User arguments. Can be used in recipe file. Format either `key=value` or `flag`.'
+    )
     parser.add_argument('-p', '--project', default=None, help='Project to build. Uses value of `default_project` if left unspecified.')
+    parser.add_argument('-i', '--interactive', action='store_true', help='Interactive project selection.')
 
     args = parser.parse_args()
 
     recipe_base_path = (pathlib.Path.cwd() / args.recipe_path).resolve()
     build_server = args.build_server
     project = args.project
 
@@ -59,19 +64,28 @@
 
     rich_output = args.format
     quiet = args.quiet
 
     list_targets = args.targets
     dry_run = args.dry
 
-    main_program = Main(recipe_base_path, project, build_server, rich_output=rich_output, quiet=quiet)
+    main_program = Main(recipe_base_path)
     main_program.initialize()
 
     if list_targets:
         projects, default_project = main_program.get_projects()
         recipe_path = main_program.get_recipe_path()
         print(f'Projects defined in {recipe_path}:')
         for project in projects:
             print('  ' + project, '<- default' if project == default_project else '')
         return
 
+    if args.interactive:
+        projects, default_project = main_program.get_projects()
+        project = questionary.select('Project', choices=projects, default=default_project).ask()
+        if project is None:
+            exit(1)
+
+    main_program.configure(project, build_server)
+    main_program.set_output(rich_output, quiet)
+
     main_program.run(dry_run=dry_run)
```

### Comparing `cook_builder-0.1.2/cook/configuration.py` & `cook_builder-0.1.3/cook/configuration.py`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.2/cook/cook.py` & `cook_builder-0.1.3/cook/cook.py`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.2/cook/executors.py` & `cook_builder-0.1.3/cook/executors.py`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.2/cook/logger.py` & `cook_builder-0.1.3/cook/logger.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -32,8 +32,8 @@
         else:
             print(message, end='')
 
     def use_rich_output(self):
         return self.rich_output
 
     def is_quiet(self):
-        return self.quiet
+        return self.quiet
```

### Comparing `cook_builder-0.1.2/cook/recipe.py` & `cook_builder-0.1.3/cook/recipe.py`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.2/cook/rsync.py` & `cook_builder-0.1.3/cook/rsync.py`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.2/cook/sync.py` & `cook_builder-0.1.3/cook/sync.py`

 * *Files identical despite different names*

### Comparing `cook_builder-0.1.2/cook_builder.egg-info/PKG-INFO` & `cook_builder-0.1.3/cook_builder.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cook_builder
-Version: 0.1.2
+Version: 0.1.3
 Summary: Build script aggregator and remote executor
 Author: Seweryn Rusecki
 License: MIT License
         
         Copyright (c) 2024 Seweryn Rusecki
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,14 +38,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fabric==3.2.2
 Requires-Dist: rich==13.7.1
+Requires-Dist: questionary==2.0.1
 
 # Cook
 
 Build script aggregator and remote executor.
 
 # Getting started
```

### Comparing `cook_builder-0.1.2/pyproject.toml` & `cook_builder-0.1.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cook_builder"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
   "fabric==3.2.2",
   "rich==13.7.1",
+  "questionary==2.0.1",
 ]
 requires-python = ">=3.10"
 authors = [
   { name="Seweryn Rusecki" },
 ]
 description = "Build script aggregator and remote executor"
 readme = "README.md"
```

