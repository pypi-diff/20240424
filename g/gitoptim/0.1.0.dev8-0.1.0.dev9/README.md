# Comparing `tmp/gitoptim-0.1.0.dev8.tar.gz` & `tmp/gitoptim-0.1.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitoptim-0.1.0.dev8.tar", max compression
+gzip compressed data, was "gitoptim-0.1.0.dev9.tar", max compression
```

## Comparing `gitoptim-0.1.0.dev8.tar` & `gitoptim-0.1.0.dev9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     1181 2024-02-28 13:18:14.167329 gitoptim-0.1.0.dev8/README.md
--rwxr-xr-x   0        0        0        0 2024-02-28 12:58:19.208174 gitoptim-0.1.0.dev8/gitoptim/__init__.py
--rwxr-xr-x   0        0        0       57 2024-03-02 13:59:31.193915 gitoptim-0.1.0.dev8/gitoptim/__main__.py
--rwxr-xr-x   0        0        0       92 2024-03-01 18:01:37.936398 gitoptim-0.1.0.dev8/gitoptim/commands/__init__.py
--rwxr-xr-x   0        0        0       56 2024-03-01 18:45:11.073168 gitoptim-0.1.0.dev8/gitoptim/commands/analyse/__init__.py
--rwxr-xr-x   0        0        0     4466 2024-03-02 14:29:32.477052 gitoptim-0.1.0.dev8/gitoptim/commands/analyse/logs.py
--rwxr-xr-x   0        0        0      313 2024-03-02 13:48:13.894234 gitoptim-0.1.0.dev8/gitoptim/commands/analyse/main.py
--rwxr-xr-x   0        0        0       55 2024-03-01 18:39:48.485767 gitoptim-0.1.0.dev8/gitoptim/commands/memlab.py
--rwxr-xr-x   0        0        0      465 2024-03-02 11:58:55.430577 gitoptim-0.1.0.dev8/gitoptim/commands/tag.py
--rwxr-xr-x   0        0        0      569 2024-03-02 13:49:12.858972 gitoptim-0.1.0.dev8/gitoptim/main.py
--rwxr-xr-x   0        0        0        0 2024-03-02 00:29:07.740287 gitoptim-0.1.0.dev8/gitoptim/schemas/__init__.py
--rwxr-xr-x   0        0        0       84 2024-03-02 00:38:03.228656 gitoptim-0.1.0.dev8/gitoptim/schemas/workflows.py
--rwxr-xr-x   0        0        0        0 2024-03-01 21:15:15.339151 gitoptim-0.1.0.dev8/gitoptim/services/__init__.py
--rwxr-xr-x   0        0        0     1034 2024-03-02 11:48:41.724063 gitoptim-0.1.0.dev8/gitoptim/services/gitlab.py
--rwxr-xr-x   0        0        0      157 2024-03-02 12:50:35.703958 gitoptim-0.1.0.dev8/gitoptim/utils/__init__.py
--rwxr-xr-x   0        0        0      280 2024-03-02 14:11:33.723128 gitoptim-0.1.0.dev8/gitoptim/utils/cli.py
--rwxr-xr-x   0        0        0     2137 2024-03-02 13:13:26.630979 gitoptim-0.1.0.dev8/gitoptim/utils/environment.py
--rwxr-xr-x   0        0        0      598 2024-03-02 01:54:57.995641 gitoptim-0.1.0.dev8/gitoptim/utils/tag.py
--rwxr-xr-x   0        0        0      588 2024-03-02 14:29:49.784888 gitoptim-0.1.0.dev8/pyproject.toml
--rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 gitoptim-0.1.0.dev8/PKG-INFO
+-rwxr-xr-x   0        0        0     1181 2024-02-28 13:18:14.167329 gitoptim-0.1.0.dev9/README.md
+-rwxr-xr-x   0        0        0        0 2024-02-28 12:58:19.208174 gitoptim-0.1.0.dev9/gitoptim/__init__.py
+-rwxr-xr-x   0        0        0       57 2024-03-02 13:59:31.193915 gitoptim-0.1.0.dev9/gitoptim/__main__.py
+-rwxr-xr-x   0        0        0       92 2024-03-01 18:01:37.936398 gitoptim-0.1.0.dev9/gitoptim/commands/__init__.py
+-rwxr-xr-x   0        0        0       56 2024-03-01 18:45:11.073168 gitoptim-0.1.0.dev9/gitoptim/commands/analyse/__init__.py
+-rwxr-xr-x   0        0        0     3588 2024-03-02 14:32:16.501883 gitoptim-0.1.0.dev9/gitoptim/commands/analyse/logs.py
+-rwxr-xr-x   0        0        0      313 2024-03-02 13:48:13.894234 gitoptim-0.1.0.dev9/gitoptim/commands/analyse/main.py
+-rwxr-xr-x   0        0        0       55 2024-03-01 18:39:48.485767 gitoptim-0.1.0.dev9/gitoptim/commands/memlab.py
+-rwxr-xr-x   0        0        0      465 2024-03-02 11:58:55.430577 gitoptim-0.1.0.dev9/gitoptim/commands/tag.py
+-rwxr-xr-x   0        0        0      569 2024-03-02 13:49:12.858972 gitoptim-0.1.0.dev9/gitoptim/main.py
+-rwxr-xr-x   0        0        0        0 2024-03-02 00:29:07.740287 gitoptim-0.1.0.dev9/gitoptim/schemas/__init__.py
+-rwxr-xr-x   0        0        0       84 2024-03-02 00:38:03.228656 gitoptim-0.1.0.dev9/gitoptim/schemas/workflows.py
+-rwxr-xr-x   0        0        0        0 2024-03-01 21:15:15.339151 gitoptim-0.1.0.dev9/gitoptim/services/__init__.py
+-rwxr-xr-x   0        0        0     1034 2024-03-02 11:48:41.724063 gitoptim-0.1.0.dev9/gitoptim/services/gitlab.py
+-rwxr-xr-x   0        0        0      157 2024-03-02 12:50:35.703958 gitoptim-0.1.0.dev9/gitoptim/utils/__init__.py
+-rwxr-xr-x   0        0        0      263 2024-03-02 14:32:20.220485 gitoptim-0.1.0.dev9/gitoptim/utils/cli.py
+-rwxr-xr-x   0        0        0     2137 2024-03-02 13:13:26.630979 gitoptim-0.1.0.dev9/gitoptim/utils/environment.py
+-rwxr-xr-x   0        0        0      598 2024-03-02 01:54:57.995641 gitoptim-0.1.0.dev9/gitoptim/utils/tag.py
+-rwxr-xr-x   0        0        0      588 2024-03-02 14:32:27.973755 gitoptim-0.1.0.dev9/pyproject.toml
+-rw-r--r--   0        0        0     1705 1970-01-01 00:00:00.000000 gitoptim-0.1.0.dev9/PKG-INFO
```

### Comparing `gitoptim-0.1.0.dev8/README.md` & `gitoptim-0.1.0.dev9/README.md`

 * *Files identical despite different names*

### Comparing `gitoptim-0.1.0.dev8/gitoptim/commands/analyse/logs.py` & `gitoptim-0.1.0.dev9/gitoptim/commands/analyse/logs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import sys
-import threading
 import time
 from typing import Annotated
 
 import httpx
 import typer
 
 from gitoptim.schemas.workflows import AnalyseLogsSchema
@@ -13,50 +11,17 @@
 PROMPT_TEMPLATE = (
     "{input}\n\nAbove are displayed logs from Gitlab CI/CD job. Analyse them. If there are no errors and warning "
     "don't do anything. If there are any errors or warning summarize them. If you know how to fix some "
     "errors/warnings or fix is described in the logs include it in your answer. Group errors, warnings and fixes by "
     "command. Commands are prefixed with $ sign.")
 
 
-class FlushThread(threading.Thread):
-    def __init__(self, interval):
-        super().__init__()
-        self.interval = interval
-        self._stop_event = threading.Event()
-
-    def stop(self):
-        self._stop_event.set()
-
-    def run(self):
-        while not self._stop_event.is_set():
-            sys.stdout.flush()
-            sys.stderr.flush()
-            time.sleep(1 / self.interval)
-
-
-class FlushStdoutContextManager:
-    def __init__(self, fps=30):
-        self.fps = fps
-
-    def __enter__(self):
-        self.flush_thread = FlushThread(self.fps)
-        self.flush_thread.start()
-        return self
-
-    def __exit__(self, exc_type, exc_value, traceback):
-        self.flush_thread.stop()
-        self.flush_thread.join()
-
-
 def extract_relevant_logs(api: GitlabAPI, after_last_command: bool):
-    sys.stdout.flush()
-
     retries = 0
     logs = api.get_job_logs()
-
     start_tag_index = logs.find(str(StartTag()))
 
     while start_tag_index == -1:
         retries += 1
 
         if retries > 18:
             error_console.print("Cannot synchronize with Gitlab logs")
@@ -121,16 +86,14 @@
     See:
     `gitoptim tag`
     """
 
     console.print("Running job logs analysis command")
     gitlab_api = GitlabAPI()
 
-    with FlushStdoutContextManager(fps=30), console.status("Synchronizing with Gitlab logs"):
-        relevant_logs = extract_relevant_logs(gitlab_api, after_last_command)
-
-    console.print("test")
+    console.print("Synchronizing with Gitlab logs... (it may take up to 3 minutes)")
+    relevant_logs = extract_relevant_logs(gitlab_api, after_last_command)
 
-    with FlushStdoutContextManager(fps=30), console.status("Starting analysis"):
-        run_workflow_task(relevant_logs)
+    console.print("Starting analysis...")
+    run_workflow_task(relevant_logs)
 
     console.print("Logs analysis started. See [url] for more details.")
```

### Comparing `gitoptim-0.1.0.dev8/gitoptim/main.py` & `gitoptim-0.1.0.dev9/gitoptim/main.py`

 * *Files identical despite different names*

### Comparing `gitoptim-0.1.0.dev8/gitoptim/services/gitlab.py` & `gitoptim-0.1.0.dev9/gitoptim/services/gitlab.py`

 * *Files identical despite different names*

### Comparing `gitoptim-0.1.0.dev8/gitoptim/utils/environment.py` & `gitoptim-0.1.0.dev9/gitoptim/utils/environment.py`

 * *Files identical despite different names*

### Comparing `gitoptim-0.1.0.dev8/gitoptim/utils/tag.py` & `gitoptim-0.1.0.dev9/gitoptim/utils/tag.py`

 * *Files identical despite different names*

### Comparing `gitoptim-0.1.0.dev8/pyproject.toml` & `gitoptim-0.1.0.dev9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gitoptim"
-version = "0.1.0-dev8"
+version = "0.1.0-dev9"
 description = "SDK tool to connect Gitlab pipelines with Workflows"
 authors = ["Łukasz Leszko <leszko.lucas@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 gitoptim = "gitoptim.main:app"
```

### Comparing `gitoptim-0.1.0.dev8/PKG-INFO` & `gitoptim-0.1.0.dev9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitoptim
-Version: 0.1.0.dev8
+Version: 0.1.0.dev9
 Summary: SDK tool to connect Gitlab pipelines with Workflows
 Author: Łukasz Leszko
 Author-email: leszko.lucas@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

