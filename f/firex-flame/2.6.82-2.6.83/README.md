# Comparing `tmp/firex_flame-2.6.82.tar.gz` & `tmp/firex_flame-2.6.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firex_flame-2.6.82.tar", last modified: Wed Feb 28 08:25:17 2024, max compression
+gzip compressed data, was "firex_flame-2.6.83.tar", last modified: Wed Apr 24 13:55:28 2024, max compression
```

## Comparing `firex_flame-2.6.82.tar` & `firex_flame-2.6.83.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-02-28 08:25:17.598697 firex_flame-2.6.82/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1505 2024-02-28 08:24:54.000000 firex_flame-2.6.82/LICENSE
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      103 2024-02-28 08:24:54.000000 firex_flame-2.6.82/MANIFEST.in
--rw-r--r--   0 firex      (101) nogroup  (65533)      286 2024-02-28 08:25:17.598697 firex_flame-2.6.82/PKG-INFO
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1642 2024-02-28 08:24:54.000000 firex_flame-2.6.82/README.md
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     4042 2024-02-28 08:24:54.000000 firex_flame-2.6.82/fastentrypoints.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-02-28 08:25:17.599697 firex_flame-2.6.82/firex_flame/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       92 2024-02-28 08:24:54.000000 firex_flame-2.6.82/firex_flame/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     8928 2024-02-28 08:24:54.000000 firex_flame-2.6.82/firex_flame/__main__.py
--rw-r--r--   0 firex      (101) nogroup  (65533)      498 2024-02-28 08:25:17.599697 firex_flame-2.6.82/firex_flame/_version.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    15302 2024-02-28 08:24:54.000000 firex_flame-2.6.82/firex_flame/api.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    18364 2024-02-28 08:24:54.000000 firex_flame-2.6.82/firex_flame/controller.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     7418 2024-02-28 08:24:54.000000 firex_flame-2.6.82/firex_flame/event_broker_processor.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3440 2024-02-28 08:24:54.000000 firex_flame-2.6.82/firex_flame/event_file_processor.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6365 2024-02-28 08:24:54.000000 firex_flame-2.6.82/firex_flame/flame_helper.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    42993 2024-02-28 08:24:54.000000 firex_flame-2.6.82/firex_flame/flame_task_graph.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     9330 2024-02-28 08:24:54.000000 firex_flame-2.6.82/firex_flame/launcher.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     2866 2024-02-28 08:24:54.000000 firex_flame-2.6.82/firex_flame/main_app.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6008 2024-02-28 08:24:54.000000 firex_flame-2.6.82/firex_flame/model_dumper.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-02-28 08:25:17.598697 firex_flame-2.6.82/firex_flame/templates/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     2530 2024-02-28 08:24:54.000000 firex_flame-2.6.82/firex_flame/templates/index.html
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     8171 2024-02-28 08:24:54.000000 firex_flame-2.6.82/firex_flame/web_app.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-02-28 08:25:17.598697 firex_flame-2.6.82/firex_flame.egg-info/
--rw-r--r--   0 firex      (101) nogroup  (65533)      286 2024-02-28 08:25:17.000000 firex_flame-2.6.82/firex_flame.egg-info/PKG-INFO
--rw-r--r--   0 firex      (101) nogroup  (65533)      706 2024-02-28 08:25:17.000000 firex_flame-2.6.82/firex_flame.egg-info/SOURCES.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2024-02-28 08:25:17.000000 firex_flame-2.6.82/firex_flame.egg-info/dependency_links.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)      137 2024-02-28 08:25:17.000000 firex_flame-2.6.82/firex_flame.egg-info/entry_points.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)      172 2024-02-28 08:25:17.000000 firex_flame-2.6.82/firex_flame.egg-info/requires.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)       12 2024-02-28 08:25:17.000000 firex_flame-2.6.82/firex_flame.egg-info/top_level.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2024-02-28 08:25:17.000000 firex_flame-2.6.82/firex_flame.egg-info/zip-safe
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      277 2024-02-28 08:25:17.599697 firex_flame-2.6.82/setup.cfg
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1675 2024-02-28 08:24:54.000000 firex_flame-2.6.82/setup.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2024-02-28 08:24:54.000000 firex_flame-2.6.82/versioneer.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-04-24 13:55:28.766620 firex_flame-2.6.83/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1505 2024-04-24 13:55:04.000000 firex_flame-2.6.83/LICENSE
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      103 2024-04-24 13:55:04.000000 firex_flame-2.6.83/MANIFEST.in
+-rw-r--r--   0 firex      (101) nogroup  (65533)      286 2024-04-24 13:55:28.766620 firex_flame-2.6.83/PKG-INFO
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1642 2024-04-24 13:55:04.000000 firex_flame-2.6.83/README.md
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     4042 2024-04-24 13:55:04.000000 firex_flame-2.6.83/fastentrypoints.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-04-24 13:55:28.767620 firex_flame-2.6.83/firex_flame/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       92 2024-04-24 13:55:04.000000 firex_flame-2.6.83/firex_flame/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     8928 2024-04-24 13:55:04.000000 firex_flame-2.6.83/firex_flame/__main__.py
+-rw-r--r--   0 firex      (101) nogroup  (65533)      498 2024-04-24 13:55:28.767620 firex_flame-2.6.83/firex_flame/_version.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    15302 2024-04-24 13:55:04.000000 firex_flame-2.6.83/firex_flame/api.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    18364 2024-04-24 13:55:04.000000 firex_flame-2.6.83/firex_flame/controller.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     7418 2024-04-24 13:55:04.000000 firex_flame-2.6.83/firex_flame/event_broker_processor.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3440 2024-04-24 13:55:04.000000 firex_flame-2.6.83/firex_flame/event_file_processor.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6365 2024-04-24 13:55:04.000000 firex_flame-2.6.83/firex_flame/flame_helper.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    43510 2024-04-24 13:55:04.000000 firex_flame-2.6.83/firex_flame/flame_task_graph.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     9330 2024-04-24 13:55:04.000000 firex_flame-2.6.83/firex_flame/launcher.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     2866 2024-04-24 13:55:04.000000 firex_flame-2.6.83/firex_flame/main_app.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6008 2024-04-24 13:55:04.000000 firex_flame-2.6.83/firex_flame/model_dumper.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-04-24 13:55:28.766620 firex_flame-2.6.83/firex_flame/templates/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     2530 2024-04-24 13:55:04.000000 firex_flame-2.6.83/firex_flame/templates/index.html
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     8171 2024-04-24 13:55:04.000000 firex_flame-2.6.83/firex_flame/web_app.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-04-24 13:55:28.766620 firex_flame-2.6.83/firex_flame.egg-info/
+-rw-r--r--   0 firex      (101) nogroup  (65533)      286 2024-04-24 13:55:28.000000 firex_flame-2.6.83/firex_flame.egg-info/PKG-INFO
+-rw-r--r--   0 firex      (101) nogroup  (65533)      706 2024-04-24 13:55:28.000000 firex_flame-2.6.83/firex_flame.egg-info/SOURCES.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2024-04-24 13:55:28.000000 firex_flame-2.6.83/firex_flame.egg-info/dependency_links.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)      137 2024-04-24 13:55:28.000000 firex_flame-2.6.83/firex_flame.egg-info/entry_points.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)      172 2024-04-24 13:55:28.000000 firex_flame-2.6.83/firex_flame.egg-info/requires.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)       12 2024-04-24 13:55:28.000000 firex_flame-2.6.83/firex_flame.egg-info/top_level.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2024-04-24 13:55:28.000000 firex_flame-2.6.83/firex_flame.egg-info/zip-safe
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      277 2024-04-24 13:55:28.767620 firex_flame-2.6.83/setup.cfg
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1675 2024-04-24 13:55:04.000000 firex_flame-2.6.83/setup.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2024-04-24 13:55:04.000000 firex_flame-2.6.83/versioneer.py
```

### Comparing `firex_flame-2.6.82/LICENSE` & `firex_flame-2.6.83/LICENSE`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.82/README.md` & `firex_flame-2.6.83/README.md`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.82/fastentrypoints.py` & `firex_flame-2.6.83/fastentrypoints.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.82/firex_flame/__main__.py` & `firex_flame-2.6.83/firex_flame/__main__.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.82/firex_flame/api.py` & `firex_flame-2.6.83/firex_flame/api.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.82/firex_flame/controller.py` & `firex_flame-2.6.83/firex_flame/controller.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.82/firex_flame/event_broker_processor.py` & `firex_flame-2.6.83/firex_flame/event_broker_processor.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.82/firex_flame/event_file_processor.py` & `firex_flame-2.6.83/firex_flame/event_file_processor.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.82/firex_flame/flame_helper.py` & `firex_flame-2.6.83/firex_flame/flame_helper.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.82/firex_flame/flame_task_graph.py` & `firex_flame-2.6.83/firex_flame/flame_task_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import dataclasses
 import os
 import tarfile
 from pathlib import Path
 from enum import Enum
 import json
 import time
+import shutil
+import subprocess
 
 from firexkit.task import FIREX_REVOKE_COMPLETE_EVENT_TYPE
 from firexapp.events.model import ADDITIONAL_CHILDREN_KEY, EXTERNAL_COMMANDS_KEY
 from firexapp.events.event_aggregator import event_type_to_task_state, REVOKED_EVENT_TYPE
 from firexapp.events.model import ADDITIONAL_CHILDREN_KEY
 from firex_flame.flame_helper import flatten, deep_merge
 from firex_flame.model_dumper import get_all_tasks_dir, get_tasks_slim_file, get_run_metadata_file, \
@@ -229,19 +231,14 @@
         if field_names is None:
             field_names = self.unloadable_field_names()
         return any(
             getattr(self, f) == _TaskFieldSentile.UNLOADED
             for f in field_names
         )
 
-    def maybe_set_unloaded_values(self, other: dict):
-        for update_key, update_value in other.items():
-            if self.any_unloaded([update_key]):
-                setattr(self, update_key, update_value)
-
     def unload_fields(self):
         for field_name in self.unloadable_field_names():
             field_val = getattr(self, field_name)
             if not isinstance(field_val, _TaskFieldSentile):
                 # allow this field's value to be garbage collected by unreferencing it.
                 setattr(self, field_name, _TaskFieldSentile.UNLOADED)
                 del field_val
@@ -1043,54 +1040,75 @@
         if dump_task_jsons:
             # Write JSON file with minimum amount of info to render graph.
             self.dump_slim_tasks(task_graph.get_slim_tasks_by_uuid())
 
             # Write one JSON file per task.
             for uuid, task in task_graph.get_full_tasks_by_uuid().items():
                 self.dump_full_task(uuid, task)
+            logger.info("Completed dumping Flame tasks.")
 
         paths_to_compress = [self.slim_tasks_file, self.full_tasks_dir]
         if run_metadata:
             # Write metadata file.
             # Note that since a flame can terminate (e.g. via timeout) before a run, there is no guarantee
             # that the run_metadata model file will ever have root_complete: true.
             root_uuid = task_graph.root_uuid
             root_complete = task_graph.is_root_complete()
             run_metadata_with_root = {**run_metadata, 'root_uuid': root_uuid}
             metadata_model_file = self.dump_metadata(run_metadata_with_root, root_complete, flame_complete=True)
             paths_to_compress.append(metadata_model_file)
 
-        # TODO: use shutil.which to find out of there is a native tar command, and use that when present to speedup
-        #  shutdown.
         # Write a tar.gz file containing all the files dumped above.
-        with tarfile.open(os.path.join(self.root_model_dir, 'full-run-state.tar.gz'), "w:gz") as tar:
-            for path in paths_to_compress:
-                tar.add(path, arcname=os.path.basename(path))
+        _dump_full_task_state_archive(self.root_model_dir, paths_to_compress)
 
         Path(get_model_complete_file(root_model_dir=self.root_model_dir)).touch()
         logger.info("Finished dumping complete Flame model.")
 
     def dump_task_representation(
         self,
         model_file_name: str,
         tasks_representation: dict[str, Any],
         force=False,
         min_age_change=0,
     ):
 
         out_file = os.path.join(self.root_model_dir, model_file_name)
 
-
         try:
             should_write = (
                 force
                 or not os.path.exists(out_file)
                 or time.time() - os.path.getmtime(out_file) > min_age_change
             )
             if should_write:
                 logger.info(f"Starting to dump task representation of: {model_file_name}.")
                 atomic_write_json(out_file, tasks_representation)
                 logger.info(f"Finished dumping {len(tasks_representation)} task representation of {model_file_name} to {out_file}.")
         except Exception as ex:
             # Don't interfere with shutdown even if extra representation dumping fails.
             logger.error(f"Failed to dump representation of {model_file_name}.")
             logger.exception(ex)
+
+
+def _dump_full_task_state_archive(
+    root_model_dir,
+    paths_to_compress
+):
+    logger.info("Starting to create full task state archive.")
+    full_state_gz_basename = 'full-run-state.tar.gz'
+    tar_bin = shutil.which('tar')
+    if tar_bin:
+        rel_paths_to_compress = [os.path.relpath(p, root_model_dir) for p in paths_to_compress]
+        try:
+            subprocess.run(
+                [tar_bin, 'czf', full_state_gz_basename] + rel_paths_to_compress,
+                cwd=root_model_dir,
+                timeout=5*60,
+                check=False,
+            )
+        except subprocess.TimeoutExpired:
+            pass
+    else:
+        with tarfile.open(os.path.join(root_model_dir, full_state_gz_basename), "w:gz") as tar:
+            for path in paths_to_compress:
+                tar.add(path, arcname=os.path.basename(path))
+    logger.info("Completed creating full task state archive.")
```

### Comparing `firex_flame-2.6.82/firex_flame/launcher.py` & `firex_flame-2.6.83/firex_flame/launcher.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.82/firex_flame/main_app.py` & `firex_flame-2.6.83/firex_flame/main_app.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.82/firex_flame/model_dumper.py` & `firex_flame-2.6.83/firex_flame/model_dumper.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.82/firex_flame/templates/index.html` & `firex_flame-2.6.83/firex_flame/templates/index.html`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.82/firex_flame/web_app.py` & `firex_flame-2.6.83/firex_flame/web_app.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.82/firex_flame.egg-info/SOURCES.txt` & `firex_flame-2.6.83/firex_flame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.82/setup.py` & `firex_flame-2.6.83/setup.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.82/versioneer.py` & `firex_flame-2.6.83/versioneer.py`

 * *Files identical despite different names*

