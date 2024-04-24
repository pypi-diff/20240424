# Comparing `tmp/kmt-0.3.1.tar.gz` & `tmp/kmt-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmt-0.3.1.tar", last modified: Tue Apr 23 01:59:27 2024, max compression
+gzip compressed data, was "kmt-0.3.2.tar", last modified: Tue Apr 23 23:49:38 2024, max compression
```

## Comparing `kmt-0.3.1.tar` & `kmt-0.3.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:59:27.634597 kmt-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-23 01:59:13.000000 kmt-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-23 01:59:27.634597 kmt-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 01:59:13.000000 kmt-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 01:59:27.634597 kmt-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-23 01:59:13.000000 kmt-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:59:27.630597 kmt-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:59:27.630597 kmt-0.3.1/src/kmt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 01:59:13.000000 kmt-0.3.1/src/kmt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 01:59:13.000000 kmt-0.3.1/src/kmt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-23 01:59:13.000000 kmt-0.3.1/src/kmt/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    24412 2024-04-23 01:59:13.000000 kmt-0.3.1/src/kmt/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-23 01:59:13.000000 kmt-0.3.1/src/kmt/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-23 01:59:13.000000 kmt-0.3.1/src/kmt/j2support.py
--rw-r--r--   0 runner    (1001) docker     (127)    11927 2024-04-23 01:59:13.000000 kmt-0.3.1/src/kmt/pipeline_support.py
--rw-r--r--   0 runner    (1001) docker     (127)    12658 2024-04-23 01:59:13.000000 kmt-0.3.1/src/kmt/step_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-04-23 01:59:13.000000 kmt-0.3.1/src/kmt/step_support.py
--rw-r--r--   0 runner    (1001) docker     (127)    13115 2024-04-23 01:59:13.000000 kmt-0.3.1/src/kmt/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     7336 2024-04-23 01:59:13.000000 kmt-0.3.1/src/kmt/yaml_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:59:27.634597 kmt-0.3.1/src/kmt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-23 01:59:27.000000 kmt-0.3.1/src/kmt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-23 01:59:27.000000 kmt-0.3.1/src/kmt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 01:59:27.000000 kmt-0.3.1/src/kmt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-23 01:59:27.000000 kmt-0.3.1/src/kmt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-23 01:59:27.000000 kmt-0.3.1/src/kmt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-23 01:59:27.000000 kmt-0.3.1/src/kmt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:49:38.624118 kmt-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-23 23:49:19.000000 kmt-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-23 23:49:38.620118 kmt-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 23:49:19.000000 kmt-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 23:49:38.624118 kmt-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-23 23:49:19.000000 kmt-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:49:38.620118 kmt-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:49:38.620118 kmt-0.3.2/src/kmt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 23:49:19.000000 kmt-0.3.2/src/kmt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 23:49:19.000000 kmt-0.3.2/src/kmt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-23 23:49:19.000000 kmt-0.3.2/src/kmt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24412 2024-04-23 23:49:19.000000 kmt-0.3.2/src/kmt/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-23 23:49:19.000000 kmt-0.3.2/src/kmt/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-23 23:49:19.000000 kmt-0.3.2/src/kmt/j2support.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12795 2024-04-23 23:49:19.000000 kmt-0.3.2/src/kmt/pipeline_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12658 2024-04-23 23:49:19.000000 kmt-0.3.2/src/kmt/step_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-04-23 23:49:19.000000 kmt-0.3.2/src/kmt/step_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13115 2024-04-23 23:49:19.000000 kmt-0.3.2/src/kmt/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7336 2024-04-23 23:49:19.000000 kmt-0.3.2/src/kmt/yaml_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:49:38.620118 kmt-0.3.2/src/kmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-23 23:49:38.000000 kmt-0.3.2/src/kmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-23 23:49:38.000000 kmt-0.3.2/src/kmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 23:49:38.000000 kmt-0.3.2/src/kmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-23 23:49:38.000000 kmt-0.3.2/src/kmt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-23 23:49:38.000000 kmt-0.3.2/src/kmt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-23 23:49:38.000000 kmt-0.3.2/src/kmt.egg-info/top_level.txt
```

### Comparing `kmt-0.3.1/LICENSE` & `kmt-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kmt-0.3.1/setup.py` & `kmt-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `kmt-0.3.1/src/kmt/cli.py` & `kmt-0.3.2/src/kmt/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import kmt.step_handlers as step_handlers
 import kmt.step_support as step_support
 import kmt.pipeline_support as pipeline_support
 import kmt.j2support as j2support
 
 logger = logging.getLogger(__name__)
 
-def process_args() -> int:
+def main():
     """
     Processes kmt command line arguments, initialises and runs the pipeline to perform text processing
     """
 
     # Create parser for command line arguments
     parser = argparse.ArgumentParser(
         prog="kmt", description="Kubernetes Manifest Transform", exit_on_error=False
@@ -49,31 +49,31 @@
         # Start executing the pipeline
         manifests = pipeline.run()
 
         logger.debug(f"Received {len(manifests)} manifests from the pipeline")
         for manifest in manifests:
             print(manifest)
 
+    except BrokenPipeError as e:
+        try:
+            print("Broken Pipe", file=sys.stderr)
+            if not sys.stderr.closed:
+                sys.stderr.close()
+        except:
+            pass
+
+        sys.exit(1)
+
     except Exception as e:  # pylint: disable=broad-exception-caught
         if debug:
             logger.error(e, exc_info=True, stack_info=True)
         else:
             logger.error(e)
-        return 1
-
-    return 0
 
+        sys.exit(1)
 
-def main():
-    """
-    Entrypoint for the module.
-    Minor exception handling is performed, along with return code processing and
-    flushing of stdout on program exit.
-    """
     try:
-        ret = process_args()
-        sys.stdout.flush()
-        sys.exit(ret)
-    except Exception as e:  # pylint: disable=broad-exception-caught
-        logging.getLogger(__name__).exception(e)
         sys.stdout.flush()
+    except Exception as e:
         sys.exit(1)
+
+    sys.exit(0)
```

### Comparing `kmt-0.3.1/src/kmt/core.py` & `kmt-0.3.2/src/kmt/core.py`

 * *Files identical despite different names*

### Comparing `kmt-0.3.1/src/kmt/exception.py` & `kmt-0.3.2/src/kmt/exception.py`

 * *Files identical despite different names*

### Comparing `kmt-0.3.1/src/kmt/j2support.py` & `kmt-0.3.2/src/kmt/j2support.py`

 * *Files identical despite different names*

### Comparing `kmt-0.3.1/src/kmt/pipeline_support.py` & `kmt-0.3.2/src/kmt/pipeline_support.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,34 +15,46 @@
 
     def post(self):
 
         # Don't bother sorting unless we're on a top level pipeline
         if not self.pipeline.root_pipeline:
             return
 
+        working = self.pipeline.manifests
+        working = sorted(working, key=lambda x: x.spec.get("name", ""))
+        working = sorted(working, key=lambda x: x.spec.get("namespace", ""))
+        working = sorted(working, key=lambda x: x.spec.get("kind", ""))
+        working = sorted(working, key=lambda x: x.spec.get("version", ""))
+        working = sorted(working, key=lambda x: x.spec.get("group", ""))
+        working = sorted(
+            working,
+            key=lambda x: x.spec.get("kind", "").casefold() != "configmap" and x.spec.get("kind", "").casefold() != "secret"
+        )
+        working = sorted(working, key=lambda x: x.spec.get("kind", "").casefold() != "namespace" )
+
+        self.pipeline.manifests = working
+
+        # Display sorted order
         def _get_metadata_str(manifest):
             keys = [
                 "group",
                 "version",
                 "kind",
                 "namespace",
                 "name",
             ]
 
             info = manifest.get_info(default_value="")
 
             return ":".join([info.get(key, "") for key in keys])
 
+        logger.debug("Sorted order:")
         for manifest in self.pipeline.manifests:
             logger.debug(f"metadata: {_get_metadata_str(manifest)}")
 
-        # Don't need a particular ordering, just consistency in output
-        # to allow for easy diff comparison
-        self.pipeline.manifests = sorted(self.pipeline.manifests, key=lambda x: _get_metadata_str(x))
-
 class PipelineSupportRenameHash(core.PipelineSupportHandler):
     def pre(self):
         pass
 
     def post(self):
 
         # Only run when we're operating on a root/top level pipeline
@@ -283,11 +295,19 @@
         for manifest in self.pipeline.manifests:
             annotations = manifest.get_annotations()
 
             for key in annotations_list:
                 if key in annotations:
                     annotations.pop(key)
 
+            metadata = manifest.get_metadata()
+
+            if "annotations" in metadata and len(metadata["annotations"]) < 1:
+                metadata.pop("annotations")
+
+            if "labels" in metadata and len(metadata["labels"]) < 1:
+                metadata.pop("labels")
+
 core.default_pipeline_support_handlers.append(PipelineSupportOrdering)
 core.default_pipeline_support_handlers.append(PipelineSupportRenameHash)
 core.default_pipeline_support_handlers.append(PipelineSupportResolveTags)
 core.default_pipeline_support_handlers.append(PipelineSupportCleanup)
```

### Comparing `kmt-0.3.1/src/kmt/step_handlers.py` & `kmt-0.3.2/src/kmt/step_handlers.py`

 * *Files identical despite different names*

### Comparing `kmt-0.3.1/src/kmt/step_support.py` & `kmt-0.3.2/src/kmt/step_support.py`

 * *Files identical despite different names*

### Comparing `kmt-0.3.1/src/kmt/util.py` & `kmt-0.3.2/src/kmt/util.py`

 * *Files identical despite different names*

### Comparing `kmt-0.3.1/src/kmt/yaml_types.py` & `kmt-0.3.2/src/kmt/yaml_types.py`

 * *Files identical despite different names*

