# Comparing `tmp/sinarax-1.1.5.tar.gz` & `tmp/sinarax-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinarax-1.1.5.tar", max compression
+gzip compressed data, was "sinarax-1.1.6.tar", max compression
```

## Comparing `sinarax-1.1.5.tar` & `sinarax-1.1.6.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0    11357 2024-03-25 17:50:13.307495 sinarax-1.1.5/LICENSE
--rw-r--r--   0        0        0     2222 2024-03-25 17:50:13.307495 sinarax-1.1.5/README.md
--rw-r--r--   0        0        0     1129 2024-03-25 17:50:13.307495 sinarax-1.1.5/pyproject.toml
--rw-r--r--   0        0        0       61 2024-03-25 17:50:13.307495 sinarax-1.1.5/sinaraX/__init__.py
--rw-r--r--   0        0        0      428 2024-03-25 17:50:13.307495 sinarax-1.1.5/sinaraX/__main__.py
--rw-r--r--   0        0        0       93 2024-03-25 17:50:13.307495 sinarax-1.1.5/sinaraX/_version.py
--rw-r--r--   0        0        0      134 2024-03-25 17:50:13.307495 sinarax-1.1.5/sinaraX/screens/__init__.py
--rw-r--r--   0        0        0       68 2024-03-25 17:50:13.307495 sinarax-1.1.5/sinaraX/screens/file_screen/__init__.py
--rw-r--r--   0        0        0     3416 2024-03-25 17:50:13.307495 sinarax-1.1.5/sinaraX/screens/file_screen/file_tree.py
--rw-r--r--   0        0        0     6490 2024-03-25 17:50:13.307495 sinarax-1.1.5/sinaraX/screens/main.py
--rw-r--r--   0        0        0     6076 2024-03-25 17:50:13.307495 sinarax-1.1.5/sinaraX/screens/running.py
--rw-r--r--   0        0        0    13858 2024-03-25 17:50:13.307495 sinarax-1.1.5/sinaraX/screens/server.py
--rw-r--r--   0        0        0     2846 2024-03-25 17:50:13.307495 sinarax-1.1.5/sinaraX/screens/server_cfg.py
--rw-r--r--   0        0        0      963 2024-03-25 17:50:13.307495 sinarax-1.1.5/sinaraX/screens/style.css
--rw-r--r--   0        0        0     2349 2024-03-25 17:50:13.307495 sinarax-1.1.5/sinaraX/screens/update.py
--rw-r--r--   0        0        0      250 2024-03-25 17:50:13.307495 sinarax-1.1.5/sinaraX/screens/utils/__init__.py
--rw-r--r--   0        0        0     4607 2024-03-25 17:50:13.307495 sinarax-1.1.5/sinaraX/screens/utils/config.py
--rw-r--r--   0        0        0     5224 2024-03-25 17:50:13.307495 sinarax-1.1.5/sinaraX/screens/utils/infra.py
--rw-r--r--   0        0        0     1564 2024-03-25 17:50:13.307495 sinarax-1.1.5/sinaraX/screens/utils/process.py
--rw-r--r--   0        0        0     3224 1970-01-01 00:00:00.000000 sinarax-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-24 12:32:33.411542 sinarax-1.1.6/LICENSE
+-rw-r--r--   0        0        0     2212 2024-04-24 12:32:33.411542 sinarax-1.1.6/README.md
+-rw-r--r--   0        0        0     1129 2024-04-24 12:32:33.411542 sinarax-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0       61 2024-04-24 12:32:33.411542 sinarax-1.1.6/sinaraX/__init__.py
+-rw-r--r--   0        0        0      428 2024-04-24 12:32:33.411542 sinarax-1.1.6/sinaraX/__main__.py
+-rw-r--r--   0        0        0       93 2024-04-24 12:32:33.411542 sinarax-1.1.6/sinaraX/_version.py
+-rw-r--r--   0        0        0      134 2024-04-24 12:32:33.411542 sinarax-1.1.6/sinaraX/screens/__init__.py
+-rw-r--r--   0        0        0       68 2024-04-24 12:32:33.411542 sinarax-1.1.6/sinaraX/screens/file_screen/__init__.py
+-rw-r--r--   0        0        0     3416 2024-04-24 12:32:33.411542 sinarax-1.1.6/sinaraX/screens/file_screen/file_tree.py
+-rw-r--r--   0        0        0     6544 2024-04-24 12:32:33.411542 sinarax-1.1.6/sinaraX/screens/main.py
+-rw-r--r--   0        0        0     6278 2024-04-24 12:32:33.411542 sinarax-1.1.6/sinaraX/screens/running.py
+-rw-r--r--   0        0        0    13814 2024-04-24 12:32:33.411542 sinarax-1.1.6/sinaraX/screens/server.py
+-rw-r--r--   0        0        0     2948 2024-04-24 12:32:33.411542 sinarax-1.1.6/sinaraX/screens/server_cfg.py
+-rw-r--r--   0        0        0      963 2024-04-24 12:32:33.411542 sinarax-1.1.6/sinaraX/screens/style.css
+-rw-r--r--   0        0        0     2403 2024-04-24 12:32:33.411542 sinarax-1.1.6/sinaraX/screens/update.py
+-rw-r--r--   0        0        0      507 2024-04-24 12:32:33.411542 sinarax-1.1.6/sinaraX/screens/utils/__init__.py
+-rw-r--r--   0        0        0     4609 2024-04-24 12:32:33.411542 sinarax-1.1.6/sinaraX/screens/utils/config.py
+-rw-r--r--   0        0        0     5721 2024-04-24 12:32:33.411542 sinarax-1.1.6/sinaraX/screens/utils/infra.py
+-rw-r--r--   0        0        0     1564 2024-04-24 12:32:33.411542 sinarax-1.1.6/sinaraX/screens/utils/process.py
+-rw-r--r--   0        0        0      847 2024-04-24 12:32:33.415542 sinarax-1.1.6/sinaraX/screens/utils/sinara_server_utils.py
+-rw-r--r--   0        0        0     3214 1970-01-01 00:00:00.000000 sinarax-1.1.6/PKG-INFO
```

### Comparing `sinarax-1.1.5/LICENSE` & `sinarax-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sinarax-1.1.5/README.md` & `sinarax-1.1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SinaraX is a TUI for the [sinaraml](https://github.com/4-DS/sinaraml) library
-[![license](https://img.shields.io/github/license/open-mmlab/mmdetection.svg)](https://github.com/open-mmlab/mmdetection/blob/main/LICENSE)
+[![license](https://img.shields.io/github/license/MiXaiLL76/sinaraX.svg)](https://github.com/MiXaiLL76/sinaraX/blob/main/LICENSE)
 
 | lib      | pypy                                                                                     |
 | -------- | ---------------------------------------------------------------------------------------- |
 | SinaraX  | [![SinaraX](https://img.shields.io/pypi/v/sinarax)](https://pypi.org/project/sinarax)    |
 | sinaraml | [![sinaraml](https://img.shields.io/pypi/v/sinaraml)](https://pypi.org/project/sinaraml) |
 | textual  | [![textual](https://img.shields.io/pypi/v/textual)](https://pypi.org/project/textual)    |
```

### Comparing `sinarax-1.1.5/pyproject.toml` & `sinarax-1.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sinaraX"
-version = "1.1.5"
+version = "1.1.6"
 readme = "README.md"
 authors = ["MiXaiLL76 <mike.milos@yandex.ru>"]
 description = "sinaraX - TUI for sinaraml clin"
 keywords = ["sinaraX", "tui", "cli", "sinaraml", "sinara"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
@@ -17,15 +17,15 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 packages = [{ include = "sinaraX" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-textual = { version = ">=0.52.0" }
+textual = { version = ">=0.57.1" }
 requests = { version = "*" }
 sinaraml = { version = ">=2024.3.12" }
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sinarax-1.1.5/sinaraX/screens/file_screen/file_tree.py` & `sinarax-1.1.6/sinaraX/screens/file_screen/file_tree.py`

 * *Files identical despite different names*

### Comparing `sinarax-1.1.5/sinaraX/screens/main.py` & `sinarax-1.1.6/sinaraX/screens/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     }
 
     BINDINGS = [
         ("escape", "exit", "Exit"),
         ("s", "server", "Server"),
         ("u", "update", "Update"),
         ("ctrl+s", "save_screen"),
+        ("f6", "copy_logs", "Copy log to clipboard"),
     ]
 
     def action_server(self):
         self.server_screen_start()
 
     def action_update(self):
         self.update_screen_start()
```

### Comparing `sinarax-1.1.5/sinaraX/screens/running.py` & `sinarax-1.1.6/sinaraX/screens/running.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,57 @@
 from pathlib import Path
 
 import docker.errors as docker_errors
 from textual import on, work
 from textual.containers import Horizontal, ScrollableContainer
 from textual.screen import ModalScreen
-from textual.widgets import Button, Collapsible, DataTable, Label, Log, Static
+from textual.widgets import (
+    Button,
+    Collapsible,
+    DataTable,
+    Footer,
+    Label,
+    Log,
+    Static,
+)
 
 from .server_cfg import BaseFunctions
 from .utils.infra import get_instanse_token, get_sinara_servers
 from .utils.process import decode_lines
 
 
 class RunningScreen(ModalScreen, BaseFunctions):
     CSS_PATH = "style.css"
 
     BINDINGS = [
         ("escape", "app.pop_screen", "Back to main."),
         ("ctrl+s", "save_screen", "Save screenshot"),
+        ("f6", "copy_logs", "Copy log to clipboard"),
+        ("u", ""),
+        ("s", ""),
     ]
 
     def action_save_screen(self):
         image_folder = Path("./images/")
         image_folder.mkdir(exist_ok=True)
         self.app.save_screenshot(image_folder.joinpath("running.svg"))
 
     def compose(self):
         self.selected_uid = None
-
+        yield Footer()
         with ScrollableContainer():
             yield Label("Running servers:")
             yield Static("Click on server for inspect server url.")
             yield DataTable(cursor_type="row")
 
             yield Static()
 
-            with Collapsible(title="not supported by sinaraml"):
+            with Collapsible(
+                title="not supported by sinaraml", collapsed=False
+            ):
                 yield Static("Select server in click!")
                 self.sudo_button = Button(
                     "install sudo",
                     id="install_sudo",
                     classes="button",
                     disabled=True,
                 )
@@ -103,15 +116,15 @@
         port = row[2]
         try:
             server_url = get_instanse_token(instanceName, port)
             out_string = f"{instanceName} running on: {server_url}\n"
             self.log_window.write_line(out_string)
             self.log_window.write_line("-----")
         except docker_errors.APIError:
-            self.log_window.write_line("server not running")
+            self.log_window.write_line("Server not running")
             self.log_window.write_line("-----")
 
     @on(DataTable.RowSelected)
     def on_row_selected(self, event: DataTable.RowSelected):
         row = event.data_table.get_row_at(event.cursor_row)
         self.select_server(row)
         self.sudo_button.disabled = False
```

### Comparing `sinarax-1.1.5/sinaraX/screens/server.py` & `sinarax-1.1.6/sinaraX/screens/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from pathlib import Path
 
-from sinaraml.server import SinaraServer
 from textual import on
 from textual.containers import Horizontal, Vertical
 from textual.events import Mount
 from textual.screen import ModalScreen
 from textual.widgets import (
     Button,
     Checkbox,
@@ -17,29 +16,34 @@
     Static,
     TabbedContent,
     TabPane,
 )
 
 from .file_screen import FilePickButton
 from .server_cfg import ServerFunctions
-from .utils import FilteredConfigTree
+from .utils import (
+    FilteredConfigTree,
+    get_cpu_cores_limit,
+    get_memory_size_limit,
+)
 
 
 class ServerScreen(ModalScreen, ServerFunctions):
     CSS_PATH = "style.css"
     config_dict = {}
 
     BINDINGS = [
         ("escape", "app.pop_screen"),
         ("ctrl+s", "save_screen"),
         ("f1", "load_config", "Load cfg"),
         ("f2", "create_server", "Server Create"),
         ("f3", "start_server", "Start"),
         ("f4", "stop_server", "Stop"),
         ("f5", "stop_remove", "Remove"),
+        ("f6", "copy_logs", "Copy log to clipboard"),
         ("u", ""),
         ("s", ""),
     ]
 
     def action_save_screen(self):
         image_folder = Path("./images/")
         image_folder.mkdir(exist_ok=True)
@@ -122,15 +126,15 @@
                 with TabbedContent(initial="base"):
                     with TabPane("Base", id="base"):
                         with Collapsible(
                             title="Sinara server container and config name",
                             collapsed=False,
                         ):
                             yield Input(
-                                value=SinaraServer.container_name,
+                                value="jovyan-single-use",
                                 name="instanceName",
                             )
 
                         with Horizontal():
                             with Vertical():
                                 with Collapsible(
                                     title="Host where the server is run",
@@ -146,18 +150,15 @@
                                 ):
                                     with RadioSet(name="sinara_image_num"):
                                         yield RadioButton("CV", value=True)
                                         yield RadioButton("ML")
 
                     with TabPane("Resource", id="resource"):
                         sinara_mem = (
-                            SinaraServer.get_memory_size_limit()
-                            // 1024
-                            // 1024
-                            // 1024
+                            get_memory_size_limit() // 1024 // 1024 // 1024
                         )
                         base_shm_size = sinara_mem // 6
                         if base_shm_size < 1:
                             base_shm_size = 1
 
                         with Collapsible(title="Memory", collapsed=False):
                             yield Static(
@@ -181,15 +182,15 @@
 
                         with Collapsible(title="Cpu", collapsed=False):
                             yield Static(
                                 " Number of CPU cores to use for"
                                 " server container"
                             )
                             yield Input(
-                                value=str(SinaraServer.get_cpu_cores_limit()),
+                                value=str(get_cpu_cores_limit()),
                                 type="number",
                                 name="cpuLimit",
                             )
 
                     with TabPane("Extra", id="extra"):
                         with Collapsible(
                             title="Server config", collapsed=False
```

### Comparing `sinarax-1.1.5/sinaraX/screens/server_cfg.py` & `sinarax-1.1.6/sinaraX/screens/server_cfg.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,17 @@
     decode_lines,
     generate_from_screen,
     load_from_file,
 )
 
 
 class BaseFunctions:
+    def action_copy_logs(self):
+        self.app.copy_to_clipboard("\n".join(self.log_window.lines))
+
     def write_log_lines(self, lines):
         self.log_window.clear()
 
         if type(lines) is list:
             self.log_window.write_lines(lines)
 
         elif type(lines) is str:
```

### Comparing `sinarax-1.1.5/sinaraX/screens/style.css` & `sinarax-1.1.6/sinaraX/screens/style.css`

 * *Files identical despite different names*

### Comparing `sinarax-1.1.5/sinaraX/screens/update.py` & `sinarax-1.1.6/sinaraX/screens/update.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     CSS_PATH = "style.css"
 
     BINDINGS = [
         ("escape", "app.pop_screen", "Back to main."),
         ("ctrl+s", "save_screen"),
         ("u", "update_all", "Update ALL"),
         ("s", ""),
+        ("f6", "copy_logs", "Copy log to clipboard"),
     ]
 
     def action_update_all(self):
         self.cmd("pip install sinaraml sinaraX --upgrade")
 
     def action_save_screen(self):
         image_folder = Path("./images/")
```

### Comparing `sinarax-1.1.5/sinaraX/screens/utils/config.py` & `sinarax-1.1.6/sinaraX/screens/utils/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import argparse
 import json
 from pathlib import Path
 from typing import Iterable
 
-from sinaraml.server import SinaraServer
 from textual.widgets import DirectoryTree, RadioSet
 
+from .sinara_server_utils import get_memory_size_limit
+
 
 class AppConfig(argparse.Namespace):
     pass
 
 
 class FilteredConfigTree(DirectoryTree):
     def filter_paths(self, paths: Iterable[Path]) -> Iterable[Path]:
@@ -52,15 +53,15 @@
         else:
             memLimit = str(_dict["memLimit"])
             if "g" in memLimit:
                 memLimit = int(memLimit.replace("g", ""))
             elif "m" in memLimit:
                 memLimit = float(memLimit.replace("m", "")) / 1024
             elif type(_dict["memLimit"]) is int:
-                max_mem = SinaraServer.get_memory_size_limit()
+                max_mem = get_memory_size_limit()
                 if int(memLimit) > max_mem:
                     memLimit = max_mem
 
                 memLimit = int(memLimit) // 1024 // 1024 // 1024
             else:
                 memLimit = None
                 del _dict["memLimit"]
```

### Comparing `sinarax-1.1.5/sinaraX/screens/utils/infra.py` & `sinarax-1.1.6/sinaraX/screens/utils/infra.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import getpass
 import importlib.metadata
 import json
 import platform
+import re
 
 import requests
-from sinaraml.server import SinaraServer
 
 from .process import start_cmd
 
 
 def check_docker():
     check_docker_cmd = "docker info -f json"
     lines = []
@@ -126,50 +126,86 @@
             if index not in label_row:
                 label_row.append(index)
         rows.append(list(row.values()))
 
     return [label_row] + rows
 
 
+def get_server_url(instance):
+    url = None
+    commands = [
+        "jupyter lab list",
+        "jupyter server list",
+        "jupyter notebook list",
+    ]
+    for cmd in commands:
+        if url:
+            continue
+
+        for line in start_cmd(f"docker exec {instance} {cmd}"):
+            if url:
+                continue
+
+            if any(x in line for x in ["http://", "https://"]):
+                m = re.search(r"(http[^\s]+)", line)
+                url = m.group(1) if m else None
+
+    return url
+
+
+def get_server_token(server_url):
+    m = re.search(r"token=([a-f0-9-][^\s]+)", server_url)
+    return m.group(1) if m else None
+
+
+def get_server_protocol(server_url):
+    m = re.search(r"^(http:|https:)", server_url)
+    return str(m.group(1))[:-1] if m else None
+
+
 def get_instanse_token(instanceName, host_port):
-    url = SinaraServer.get_server_url(instanceName)
-    token = SinaraServer.get_server_token(url)
+    url = get_server_url(instanceName)
+
+    try:
+        token = get_server_token(url)
+    except TypeError:
+        token = None
+
     token_str = f"?token={token}" if token else ""
-    protocol = SinaraServer.get_server_protocol(url)
 
-    platform = SinaraServer.get_server_platform(instanceName)
-    server_ip = SinaraServer.get_server_ip(platform)
+    try:
+        protocol = get_server_protocol(url)
+    except TypeError:
+        protocol = "http"
+
+    server_ip = "localhost"
     server_url = f"{protocol}://{server_ip}:{host_port}/{token_str}"
     return server_url
 
 
 def check_last_version(name: str):
     try:
-        local_version = (name + "-" + importlib.metadata.version(name)).lower()
+        local_version = str(importlib.metadata.version(name)).lower()
 
-        url = f"https://pypi.org/simple/{name}/"
+        url = f"https://pypi.org/pypi/{name}/json"
         resp = requests.get(url)
         if resp.status_code == 200:
-            text = resp.text.lower()
-            lines = text.split("\n")
-            lines = [line for line in lines if ".tar.gz" in line]
-            version_idx = -1
-            for idx, line in enumerate(lines):
-                start_idx = line.find(">") + 1
-                if start_idx == -1:
-                    continue
-
-                end_idx = line.find(".tar.gz", start_idx)
-
-                lines[idx] = line[start_idx:end_idx].lower()
-                if local_version == lines[idx]:
-                    version_idx = idx
+            package_data = resp.json()
+
+            last_version = (
+                package_data.get("info", {})
+                .get("version", "not found!")
+                .lower()
+            )
 
-            if version_idx < idx:
-                return False, f"Available new! [{lines[idx]}]"
+            if last_version != local_version:
+                return (
+                    False,
+                    f"Available new! [{local_version}] < [{last_version}]",
+                )
         else:
             return False, "Pypi not available from this env!"
     except UnboundLocalError:
         return False, "UnboundLocalError!"
     except ImportError:
         return False, "ImportError!"
```

### Comparing `sinarax-1.1.5/sinaraX/screens/utils/process.py` & `sinarax-1.1.6/sinaraX/screens/utils/process.py`

 * *Files identical despite different names*

### Comparing `sinarax-1.1.5/PKG-INFO` & `sinarax-1.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinaraX
-Version: 1.1.5
+Version: 1.1.6
 Summary: sinaraX - TUI for sinaraml clin
 Keywords: sinaraX,tui,cli,sinaraml,sinara
 Author: MiXaiLL76
 Author-email: mike.milos@yandex.ru
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,20 +15,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: requests
 Requires-Dist: sinaraml (>=2024.3.12)
-Requires-Dist: textual (>=0.52.0)
+Requires-Dist: textual (>=0.57.1)
 Project-URL: Homepage, https://github.com/MiXaiLL76/sinaraX
 Description-Content-Type: text/markdown
 
 # SinaraX is a TUI for the [sinaraml](https://github.com/4-DS/sinaraml) library
-[![license](https://img.shields.io/github/license/open-mmlab/mmdetection.svg)](https://github.com/open-mmlab/mmdetection/blob/main/LICENSE)
+[![license](https://img.shields.io/github/license/MiXaiLL76/sinaraX.svg)](https://github.com/MiXaiLL76/sinaraX/blob/main/LICENSE)
 
 | lib      | pypy                                                                                     |
 | -------- | ---------------------------------------------------------------------------------------- |
 | SinaraX  | [![SinaraX](https://img.shields.io/pypi/v/sinarax)](https://pypi.org/project/sinarax)    |
 | sinaraml | [![sinaraml](https://img.shields.io/pypi/v/sinaraml)](https://pypi.org/project/sinaraml) |
 | textual  | [![textual](https://img.shields.io/pypi/v/textual)](https://pypi.org/project/textual)    |
```

