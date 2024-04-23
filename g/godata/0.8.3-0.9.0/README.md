# Comparing `tmp/godata-0.8.3.tar.gz` & `tmp/godata-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "godata-0.8.3.tar", max compression
+gzip compressed data, was "godata-0.9.0.tar", max compression
```

## Comparing `godata-0.8.3.tar` & `godata-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0        0 2024-01-26 22:51:27.659110 godata-0.8.3/README.md
--rw-r--r--   0        0        0      477 2024-01-26 22:51:27.659110 godata-0.8.3/godata/__init__.py
--rw-r--r--   0        0        0      443 2024-01-26 22:51:27.659110 godata-0.8.3/godata/cli/cli.py
--rw-r--r--   0        0        0      912 2024-01-26 22:51:27.659110 godata-0.8.3/godata/cli/ie.py
--rw-r--r--   0        0        0     2806 2024-01-26 22:51:27.659110 godata-0.8.3/godata/cli/project.py
--rw-r--r--   0        0        0      723 2024-01-26 22:51:27.659110 godata-0.8.3/godata/cli/server.py
--rw-r--r--   0        0        0      335 2024-01-26 22:51:27.659110 godata-0.8.3/godata/cli/utils.py
--rw-r--r--   0        0        0        0 2024-01-26 22:51:27.659110 godata-0.8.3/godata/client/__init__.py
--rw-r--r--   0        0        0     9847 2024-01-26 22:51:27.659110 godata-0.8.3/godata/client/client.py
--rw-r--r--   0        0        0     2873 2024-01-26 22:51:27.659110 godata-0.8.3/godata/client/unixsocket.py
--rw-r--r--   0        0        0       62 2024-01-26 22:51:27.659110 godata-0.8.3/godata/files/__init__.py
--rw-r--r--   0        0        0      443 2024-01-26 22:51:27.659110 godata-0.8.3/godata/files/utils.py
--rw-r--r--   0        0        0     3811 2024-01-26 22:51:27.659110 godata-0.8.3/godata/ie.py
--rw-r--r--   0        0        0     5394 2024-01-26 22:51:27.659110 godata-0.8.3/godata/io/__init__.py
--rw-r--r--   0        0        0      371 2024-01-26 22:51:27.659110 godata-0.8.3/godata/io/jsonio.py
--rw-r--r--   0        0        0      401 2024-01-26 22:51:27.659110 godata-0.8.3/godata/io/numpyio.py
--rw-r--r--   0        0        0     1022 2024-01-26 22:51:27.659110 godata-0.8.3/godata/io/pandasio.py
--rw-r--r--   0        0        0      430 2024-01-26 22:51:27.659110 godata-0.8.3/godata/io/polarsio.py
--rw-r--r--   0        0        0    14154 2024-01-26 22:51:27.659110 godata-0.8.3/godata/project.py
--rw-r--r--   0        0        0     1166 2024-01-26 22:51:27.659110 godata-0.8.3/godata/server/__init__.py
--rw-r--r--   0        0        0     2570 2024-01-26 22:51:27.663110 godata-0.8.3/godata/server/install.py
--rw-r--r--   0        0        0     2067 2024-01-26 22:51:27.663110 godata-0.8.3/godata/utils.py
--rw-r--r--   0        0        0      796 2024-01-26 22:51:27.663110 godata-0.8.3/pyproject.toml
--rw-r--r--   0        0        0      670 1970-01-01 00:00:00.000000 godata-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-01-31 21:50:16.587896 godata-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3310 2024-01-31 21:50:16.587896 godata-0.9.0/README.md
+-rw-r--r--   0        0        0      477 2024-01-31 21:50:16.587896 godata-0.9.0/godata/__init__.py
+-rw-r--r--   0        0        0      443 2024-01-31 21:50:16.587896 godata-0.9.0/godata/cli/cli.py
+-rw-r--r--   0        0        0      912 2024-01-31 21:50:16.587896 godata-0.9.0/godata/cli/ie.py
+-rw-r--r--   0        0        0     2806 2024-01-31 21:50:16.587896 godata-0.9.0/godata/cli/project.py
+-rw-r--r--   0        0        0     1405 2024-01-31 21:50:16.587896 godata-0.9.0/godata/cli/server.py
+-rw-r--r--   0        0        0      335 2024-01-31 21:50:16.587896 godata-0.9.0/godata/cli/utils.py
+-rw-r--r--   0        0        0        0 2024-01-31 21:50:16.587896 godata-0.9.0/godata/client/__init__.py
+-rw-r--r--   0        0        0    10128 2024-01-31 21:50:16.587896 godata-0.9.0/godata/client/client.py
+-rw-r--r--   0        0        0     2873 2024-01-31 21:50:16.587896 godata-0.9.0/godata/client/unixsocket.py
+-rw-r--r--   0        0        0       62 2024-01-31 21:50:16.587896 godata-0.9.0/godata/files/__init__.py
+-rw-r--r--   0        0        0      443 2024-01-31 21:50:16.587896 godata-0.9.0/godata/files/utils.py
+-rw-r--r--   0        0        0     3992 2024-01-31 21:50:16.587896 godata-0.9.0/godata/ie.py
+-rw-r--r--   0        0        0     5394 2024-01-31 21:50:16.591896 godata-0.9.0/godata/io/__init__.py
+-rw-r--r--   0        0        0      386 2024-01-31 21:50:16.591896 godata-0.9.0/godata/io/fitsio.py
+-rw-r--r--   0        0        0      371 2024-01-31 21:50:16.591896 godata-0.9.0/godata/io/jsonio.py
+-rw-r--r--   0        0        0      401 2024-01-31 21:50:16.591896 godata-0.9.0/godata/io/numpyio.py
+-rw-r--r--   0        0        0     1022 2024-01-31 21:50:16.591896 godata-0.9.0/godata/io/pandasio.py
+-rw-r--r--   0        0        0      430 2024-01-31 21:50:16.591896 godata-0.9.0/godata/io/polarsio.py
+-rw-r--r--   0        0        0    14154 2024-01-31 21:50:16.591896 godata-0.9.0/godata/project.py
+-rw-r--r--   0        0        0     2529 2024-01-31 21:50:16.591896 godata-0.9.0/godata/server/__init__.py
+-rw-r--r--   0        0        0     2653 2024-01-31 21:50:16.591896 godata-0.9.0/godata/server/install.py
+-rw-r--r--   0        0        0     2067 2024-01-31 21:50:16.591896 godata-0.9.0/godata/utils.py
+-rw-r--r--   0        0        0      996 2024-01-31 21:50:16.591896 godata-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3891 1970-01-01 00:00:00.000000 godata-0.9.0/PKG-INFO
```

### Comparing `godata-0.8.3/godata/cli/ie.py` & `godata-0.9.0/godata/cli/ie.py`

 * *Files identical despite different names*

### Comparing `godata-0.8.3/godata/cli/project.py` & `godata-0.9.0/godata/cli/project.py`

 * *Files identical despite different names*

### Comparing `godata-0.8.3/godata/client/client.py` & `godata-0.9.0/godata/client/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from functools import cache
 from pathlib import Path
 from urllib import parse
 
 import requests
 from packaging import version
+from requests.adapters import HTTPAdapter
 
 from godata import server
 
 from .unixsocket import UnixHTTPAdapter
 
 """
 The client connects to the godata server and communicates with it on behalf of the 
@@ -14,18 +16,14 @@
 REST-ish API. Windows is not supported at this time, but will probalby just have 
 to use a TCP socket instead of a unix socket.
 
 The client is stateless, so it's just a bunch of functions.
 
 I need to think a bit about how to properly reuse the client sesion.
 """
-SERVER_PATH = str(Path.home() / ".godata.sock")
-SERVER_URL = f"http+unix://{parse.quote(SERVER_PATH, safe='')}"
-CLIENT = requests.Session()
-CLIENT.mount("http+unix://", UnixHTTPAdapter(SERVER_PATH))
 
 
 class NotFound(Exception):
     pass
 
 
 class AlreadyExists(Exception):
@@ -36,91 +34,107 @@
     pass
 
 
 class GodataClientError(Exception):
     pass
 
 
-def check_server():
+def check_server(client, url):
     from godata import __minimum_server_version__
 
-    server_version = version.parse(get_version(CLIENT))
+    server_version = version.parse(get_version(client, url))
     minium_version = version.parse(__minimum_server_version__)
 
     if server_version < minium_version:
         raise GodataClientError(
             f"Server version {server_version} is less than minimum version "
             f"{minium_version}. Please upgrade the server."
         )
     return True
 
 
+@cache
 def get_client():
-    if not hasattr(get_client, "has_run"):
-        try:
-            check_server()
-        except requests.exceptions.ConnectionError:
-            server.start()
-            check_server()
-        get_client.has_run = True
-    return CLIENT
+    try:
+        with open(Path.home() / ".godata_server", "r") as f:
+            SERVER_URL = f.read().strip()
+    except FileNotFoundError:
+        SERVER_URL = None
+
+    if not SERVER_URL:
+        server.start()
+        return get_client()
+
+    elif SERVER_URL.startswith("http+unix://"):
+        SERVER_PATH = parse.unquote(SERVER_URL.split("://")[1])
+        ADAPTER = UnixHTTPAdapter(SERVER_PATH)
+    else:
+        ADAPTER = HTTPAdapter()
+
+    CLIENT = requests.Session()
+    CLIENT.mount(SERVER_URL, ADAPTER)
+
+    try:
+        check_server(CLIENT, SERVER_URL)
+        return (CLIENT, SERVER_URL)
+    except requests.exceptions.ConnectionError:
+        server.start()
+        return get_client()
 
 
-def get_version(client):
-    resp = client.get(f"{SERVER_URL}/version")
+def get_version(client, url):
+    resp = client.get(f"{url}/version")
     if resp.status_code == 200:
         return resp.json()
 
 
 def list_collections(show_hidden=False):
-    client = get_client()
+    client, url = get_client()
     payload = {"show_hidden": str(show_hidden).lower()}
-    result = client.get(f"{SERVER_URL}/collections", params=payload)
+    result = client.get(f"{url}/collections", params=payload)
     return result.json()
 
 
 def list_projects(collection_name: str, show_hidden: bool = False):
-    client = get_client()
+    client, url = get_client()
     payload = {"show_hidden": str(show_hidden).lower()}
-    resp = client.get(f"{SERVER_URL}/projects/{collection_name}", params=payload)
+    resp = client.get(f"{url}/projects/{collection_name}", params=payload)
     if resp.status_code == 200:
         return resp.json()
     elif resp.status_code == 404:
         raise NotFound(f"{resp.json()}")
     else:
         raise GodataClientError(f"{resp.status_code}: {resp.text}")
 
 
 def create_project(
     collection_name: str,
     project_name: str,
     force: bool = False,
     storage_location: str = None,
 ):
-    client = get_client()
+    client, url = get_client()
     args = {"force": str(force).lower()}
     if storage_location:
         args["storage_location"] = storage_location
 
-    result = client.post(
-        f"{SERVER_URL}/create/{collection_name}/{project_name}", params=args
-    )
+    result = client.post(f"{url}/create/{collection_name}/{project_name}", params=args)
     if result.status_code == 201:
         return result.json()
     elif result.status_code == 409:
         raise AlreadyExists(f"{result.json()}")
     else:
         raise GodataClientError(f"{result.status_code}: {result.text}")
 
 
 def delete_project(collection_name: str, project_name: str, force: bool = False):
-    client = get_client()
+    client, url = get_client()
     payload = {"force": str(force).lower()}
     resp = client.delete(
-        f"{SERVER_URL}/projects/{collection_name}/{project_name}", params=payload
+        f"{url}/projects/{collection_name}/{project_name}", params=payload
     )
     if resp.status_code == 200:
         return resp.json()
     elif resp.status_code == 404:
         raise NotFound(f"{resp.json()}")
     elif resp.status_code == 403:
         raise Forbidden(f"{resp.json()}")
@@ -128,47 +142,47 @@
         raise GodataClientError(f"{resp.status_code}: {resp.text}")
 
 
 def load_project(collection_name: str, project_name: str):
     """
     Load a project into the server memory if it is not already loaded.
     """
-    client = get_client()
-    resp = client.post(f"{SERVER_URL}/load/{collection_name}/{project_name}")
+    client, url = get_client()
+    resp = client.post(f"{url}/load/{collection_name}/{project_name}")
     if resp.status_code == 200:
         print(resp.json())
         return True
     elif resp.status_code == 404:
         raise NotFound(f"{resp.json()}")
     else:
         raise GodataClientError(f"{resp.status_code}: {resp.text}")
 
 
 def drop_project(collection_name: str, project_name: str):
     """
     Signals to the server this client is done with this project. This may or may not
     actually drop the project from memory, depending on if other clients are using it.
     """
-    client = get_client()
+    client, url = get_client()
     try:
-        resp = client.post(f"{SERVER_URL}/drop/{collection_name}/{project_name}")
+        resp = client.post(f"{url}/drop/{collection_name}/{project_name}")
     except requests.exceptions.ConnectionError:
         # The server is probably down, so this operation doesn't really matter
         return {}
     if resp.status_code == 200:
         return resp.json()
     else:
         raise GodataClientError(f"{resp.status_code}: {resp.text}")
 
 
 def path_exists(collection_name: str, project_name: str, project_path: str):
-    client = get_client()
+    client, url = get_client()
     params = {"project_path": project_path}
     resp = client.get(
-        f"{SERVER_URL}/projects/{collection_name}/{project_name}/exists", params=params
+        f"{url}/projects/{collection_name}/{project_name}/exists", params=params
     )
     if resp.status_code == 200:
         return resp.json()
     else:
         raise GodataClientError(f"{resp.status_code}: {resp.text}")
 
 
@@ -176,15 +190,15 @@
     collection_name: str,
     project_name: str,
     project_path: str,
     file_path: str,
     metadata: dict = {},
     force: bool = False,
 ):
-    client = get_client()
+    client, url = get_client()
     params = {
         "project_path": project_path,
         "real_path": file_path,
         "force": str(force).lower(),
     }
     if set(metadata.keys()).intersection(set(params.keys())):
         raise GodataClientError(
@@ -196,15 +210,15 @@
             params.update({str(k): str(v)})
         except TypeError:
             raise GodataClientError(
                 "Metadata keys and values must be convertible strings."
             ) from None
 
     resp = client.post(
-        f"{SERVER_URL}/projects/{collection_name}/{project_name}/files", params=params
+        f"{url}/projects/{collection_name}/{project_name}/files", params=params
     )
     if resp.status_code == 201:
         return resp.json()
     elif resp.status_code == 409:
         raise AlreadyExists(f"{resp.json()}")
     else:
         raise GodataClientError(f"{resp.status_code}: {resp.text}")
@@ -213,23 +227,23 @@
 def link_folder(
     collection_name: str,
     project_name: str,
     project_path: str,
     folder_path: str,
     recursive: bool = False,
 ):
-    client = get_client()
+    client, url = get_client()
     params = {
         "project_path": project_path,
         "real_path": folder_path,
         "type": "folder",
         "recursive": str(recursive).lower(),
     }
     resp = client.post(
-        f"{SERVER_URL}/projects/{collection_name}/{project_name}/files", params=params
+        f"{url}/projects/{collection_name}/{project_name}/files", params=params
     )
     if resp.status_code == 201:
         return resp.json()
     elif resp.status_code == 409:
         raise AlreadyExists(f"{resp.json()}")
     else:
         raise GodataClientError(f"{resp.status_code}: {resp.text}")
@@ -237,90 +251,86 @@
 
 def list_project_contents(
     collection_name: str,
     project_name: str,
     project_path=None,
     show_hidden: bool = False,
 ):
-    client = get_client()
+    client, url = get_client()
     params = {"show_hidden": str(show_hidden).lower()}
     if project_path:
         params["project_path"] = project_path
 
     resp = client.get(
-        f"{SERVER_URL}/projects/{collection_name}/{project_name}/list", params=params
+        f"{url}/projects/{collection_name}/{project_name}/list", params=params
     )
     if resp.status_code == 200:
         return resp.json()
     elif resp.status_code == 404:
         raise NotFound(f"{resp.json()}")
     else:
         raise GodataClientError(f"{resp.status_code}: {resp.text}")
 
 
 def get_file(collection_name: str, project_name: str, project_path: str):
-    client = get_client()
+    client, url = get_client()
     params = {"project_path": project_path}
     resp = client.get(
-        f"{SERVER_URL}/projects/{collection_name}/{project_name}/files", params=params
+        f"{url}/projects/{collection_name}/{project_name}/files", params=params
     )
     if resp.status_code == 200:
         return resp.json()
     else:
         raise NotFound(f"{resp.json()}")
 
 
 def generate_path(collection_name: str, project_name: str, project_path: str):
-    client = get_client()
+    client, url = get_client()
     params = {"project_path": project_path}
     resp = client.get(
-        f"{SERVER_URL}/projects/{collection_name}/{project_name}/generate",
+        f"{url}/projects/{collection_name}/{project_name}/generate",
         params=params,
     )
     if resp.status_code == 200:
         return resp.json()
     elif resp.status_code == 404:
         raise NotFound(f"{resp.json()}")
     else:
         raise GodataClientError(f"{resp.status_code}: {resp.text}")
 
 
 def remove_file(collection_name: str, project_name: str, project_path: str):
-    client = get_client()
+    client, url = get_client()
     params = {"project_path": project_path}
     resp = client.delete(
-        f"{SERVER_URL}/projects/{collection_name}/{project_name}/files", params=params
+        f"{url}/projects/{collection_name}/{project_name}/files", params=params
     )
     if resp.status_code == 200:
         return resp.json()
     elif resp.status_code == 404:
         raise NotFound(f"{resp.json()}")
     else:
         raise GodataClientError(f"{resp.status_code}: {resp.text}")
 
 
 def export_tree(collection_name: str, project_name: str, output_path: Path):
-    client = get_client()
+    client, url = get_client()
     params = {"output_path": str(output_path)}
-    resp = client.get(
-        f"{SERVER_URL}/export/{collection_name}/{project_name}", params=params
-    )
+    resp = client.get(f"{url}/export/{collection_name}/{project_name}", params=params)
     if resp.status_code == 200:
         return resp.json()
     elif resp.status_code == 404:
         raise NotFound(f"{resp.json()}")
     else:
         raise GodataClientError(f"{resp.status_code}: {resp.text}")
 
 
 def import_tree(collection_name: str, project_name: str, input_path: Path):
-    client = get_client()
+    client, url = get_client()
     params = {"input_path": str(input_path)}
-    resp = client.get(
-        f"{SERVER_URL}/import/{collection_name}/{project_name}", params=params
-    )
+    resp = client.get(f"{url}/import/{collection_name}/{project_name}", params=params)
     if resp.status_code == 200:
         return resp.json()
     elif resp.status_code == 404:
         raise NotFound(f"{resp.json()}")
     else:
         raise GodataClientError(f"{resp.status_code}: {resp.text}")
```

### Comparing `godata-0.8.3/godata/client/unixsocket.py` & `godata-0.9.0/godata/client/unixsocket.py`

 * *Files identical despite different names*

### Comparing `godata-0.8.3/godata/ie.py` & `godata-0.9.0/godata/ie.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,21 +35,24 @@
     if not output_location:
         output_location = Path.cwd()
 
     source_project = load_project(project_name, collection_name)
     target_project = create_project(
         project_name, ".temp", storage_location=output_location
     )
+    print("Duplicating project for export")
     export_helper(source_project, target_project)
     # Now, zip up the temporary project
     zip_path = output_location / f"{project_name}.zip"
     expected_location = output_location / f".temp.{project_name}"
     if not expected_location.exists():
         raise RuntimeError("Something went wrong with the export")
+    print("Exporting project file tree...")
     export_tree(collection_name, project_name, expected_location)
+    print("Zipping up project...")
     with zipfile.ZipFile(zip_path, "w") as zip_file:
         # Recursively add all files in the temp project
         for f in expected_location.glob("**/*"):
             zip_file.write(f, f.relative_to(expected_location))
     # Clean up the temp project
     del target_project
     delete_project(project_name, ".temp", True)
@@ -57,23 +60,24 @@
 
 
 def export_helper(
     source_project: GodataProject,
     destination_project: GodataProject,
     project_path: str = None,
 ) -> None:
+    print(f"Working on {project_path}...")
     folder_contents = source_project.list(project_path)
     files = folder_contents["files"]
     folders = folder_contents["folders"]
     if not project_path:
         project_path = ""
     for f in files:
         file_project_path = f"{project_path}/{f}"
         file_real_path = source_project.get(file_project_path, as_path=True)
-        destination_project.store(file_real_path, file_project_path)
+        destination_project.store(file_real_path, file_project_path, verbose=False)
     for f in folders:
         export_helper(source_project, destination_project, f"{project_path}/{f}")
 
 
 def import_project(
     zip_path: Path,
     project_name: str = None,
```

### Comparing `godata-0.8.3/godata/io/__init__.py` & `godata-0.9.0/godata/io/__init__.py`

 * *Files identical despite different names*

### Comparing `godata-0.8.3/godata/io/pandasio.py` & `godata-0.9.0/godata/io/pandasio.py`

 * *Files identical despite different names*

### Comparing `godata-0.8.3/godata/project.py` & `godata-0.9.0/godata/project.py`

 * *Files identical despite different names*

### Comparing `godata-0.8.3/godata/server/__init__.py` & `godata-0.9.0/godata/cli/server.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,68 @@
-import os
-import signal
-import subprocess
-import time
+from pathlib import Path
 
-import requests
+import click
 
-from godata.client import client
+from godata import server as srv
 
-from .install import SERVER_INSTALL_PATH, install, upgrade
 
-
-def start():
-    try:
-        client.check_server()
-    except client.GodataClientError as e:
-        # Server is running, but client has a bad version
-        print(e)
-        return
-    except requests.exceptions.ConnectionError:
-        is_running = False
-    else:
-        is_running = True
-    if is_running:
-        print("Server is already running.")
-        return
-
-    try:
-        subprocess.Popen([f"{SERVER_INSTALL_PATH}"], close_fds=True, shell=True)
-    except FileNotFoundError:
-        raise FileNotFoundError(
-            "Unable to start godata server: could not find the server binary. "
-            "Please run `godata server install` first."
-        )
-    time.sleep(0.5)
-    return True
+# top level godata command
+@click.group()
+def server():
+    pass
+
+
+# server subcommand
+@server.command()
+@click.option(
+    "--port",
+    "-p",
+    help="Port to start the server on. Default is 8000",
+    type=int,
+)
+def start(port: int = None):
+    """
+    Start the godata server. This will start the server in the background. By default,
+    the server will be started on a unix socker, unless the --port option is used,
+    in which case the server will be started on a TCP socket. If running on Windows,
+    the server will always be started on a TCP socket.
+    """
+    srv.start(port=port)
 
 
+@server.command()
 def stop():
+    """
+    Stop the godata server if it is running.
+    """
     try:
-        server_pid = subprocess.check_output(["pgrep", "godata_server"])
-    except subprocess.CalledProcessError:
-        print("Server is not running.")
-        return
+        srv.stop()
+    except Exception as e:
+        print(e)
 
-    os.kill(int(server_pid), signal.SIGINT)
+
+@server.command()
+@click.option(
+    "--upgrade",
+    "-u",
+    is_flag=True,
+    help="Upgrade the server to the latest version.",
+)
+@click.option(
+    "--path",
+    "-p",
+    help="Path to install the server binary.",
+    type=click.Path(file_okay=False, resolve_path=True, path_type=Path),
+    default=srv.get_server_location(),
+)
+def install(upgrade: bool, path: Path):
+    print(f"Installing server at {path}")
+    srv.set_server_location(path)
+    if upgrade:
+        srv.upgrade()
+    else:
+        srv.install()
 
 
-__all__ = ["start", "stop", "install", "upgrade"]
+@server.command()
+def uninstall():
+    pass
```

### Comparing `godata-0.8.3/godata/server/install.py` & `godata-0.9.0/godata/server/install.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # from . import SERVER_INSTALL_PATH
 import os
 import platform
 import shutil
 import subprocess
 import zipfile
+from pathlib import Path
 
 import requests
 
 from godata import server
 
 ENDPOINT = "https://sqm13wjyaf.execute-api.us-west-2.amazonaws.com/godata/download"
-SERVER_INSTALL_PATH = "/usr/local/bin/godata_server"
+DEFAULT_SERVER_INSTALL_LOCATION = Path.home() / ".local" / "bin"
 
 
 def install(upgrade=False, version=None):
     """Install the godata server binary to /usr/local/bin/godata_server."""
     # detect the os this script is running on
     if upgrade and version is None:
         raise ValueError("Must specify the current version when upgrading.")
@@ -47,19 +48,21 @@
 
     with open("godata_server.zip", "wb") as f:
         f.write(result.content)
     # unzip the file
     with zipfile.ZipFile("godata_server.zip", "r") as zip_ref:
         zip_ref.extractall()
     # move the binary to the install path
-    shutil.move("godata_server", SERVER_INSTALL_PATH)
+    install_path = server.get_server_path()
+
+    shutil.move("godata_server", install_path)
     # remove the zip file
     os.remove("godata_server.zip")
     # make the binary executable
-    os.chmod(SERVER_INSTALL_PATH, 0o755)
+    os.chmod(install_path, 0o755)
     print("Restarting server...")
     server.start()
     if version is None:
         print(f"Successfully installed godata server version {response['version']}")
     else:
         print(
             f"Successfully upgraded godata server to version {response['version']} "
@@ -70,16 +73,15 @@
 def upgrade():
     """Upgrade the godata server binary to the latest version."""
     current_version = get_version().strip("\n")
     install(upgrade=True, version=current_version)
 
 
 def get_version():
+    install_path = server.get_server_path()
     try:
-        return subprocess.check_output([f"{SERVER_INSTALL_PATH}", "--version"]).decode(
-            "utf-8"
-        )
+        return subprocess.check_output([f"{install_path}", "--version"]).decode("utf-8")
     except FileNotFoundError:
         raise FileNotFoundError(
             "Unable to get godata server version: could not find the server binary. "
             "Please run `godata server install` first."
         )
```

### Comparing `godata-0.8.3/godata/utils.py` & `godata-0.9.0/godata/utils.py`

 * *Files identical despite different names*

### Comparing `godata-0.8.3/pyproject.toml` & `godata-0.9.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "godata"
-version = "0.8.3"
+version = "0.9.0"
 description = ""
 authors = ["Patrick Wells <pwells@ucdavis.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 loguru = "^0.7.2"
@@ -18,25 +18,37 @@
 portalocker = "^2.8.2"
 appdirs = "^1.4.4"
 packaging = "^23.2"
 
 [tool.poetry.scripts]
 godata = "godata.cli.cli:main"
 
+[tool.poetry.group.dev]
+optional = true
+
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.4.3"
 ruff = "^0.1.7"
 black = "^23.11.0"
 isort = "^5.13.0"
+
+[tool.poetry.group.test]
+optional = true
+
+[tool.poetry.group.test.dependencies]
+pytest = "^7.4.3"
 numpy = "^1.26.2"
 pandas = "^2.1.4"
 toml = "^0.10.2"
 polars = "^0.20.5"
 pyarrow = "^14.0.2"
+astropy = "^6.0.0"
+
 
+[tool.poetry.group.tests.dependencies]
+astropy = "^6.0.0"
 
 [tool.isort]
 profile = "black"
 
 [tool.black]
 extend-exclude = '''
 (
```

