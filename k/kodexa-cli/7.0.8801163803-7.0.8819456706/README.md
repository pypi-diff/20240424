# Comparing `tmp/kodexa_cli-7.0.8801163803.tar.gz` & `tmp/kodexa_cli-7.0.8819456706.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa_cli-7.0.8801163803.tar", max compression
+gzip compressed data, was "kodexa_cli-7.0.8819456706.tar", max compression
```

## Comparing `kodexa_cli-7.0.8801163803.tar` & `kodexa_cli-7.0.8819456706.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    11357 2024-04-23 13:19:49.403059 kodexa_cli-7.0.8801163803/LICENSE
--rw-r--r--   0        0        0     2101 2024-04-23 13:19:49.403059 kodexa_cli-7.0.8801163803/README.md
--rw-r--r--   0        0        0       64 2024-04-23 13:19:49.407059 kodexa_cli-7.0.8801163803/kodexa_cli/__init__.py
--rw-r--r--   0        0        0      349 2024-04-23 13:19:49.407059 kodexa_cli-7.0.8801163803/kodexa_cli/charts/extension-pack/.helmignore
--rw-r--r--   0        0        0      146 2024-04-23 13:19:49.407059 kodexa_cli-7.0.8801163803/kodexa_cli/charts/extension-pack/Chart.yaml
--rw-r--r--   0        0        0        0 2024-04-23 13:19:49.407059 kodexa_cli-7.0.8801163803/kodexa_cli/charts/extension-pack/resources/.gitkeep
--rw-r--r--   0        0        0       38 2024-04-23 13:19:49.407059 kodexa_cli-7.0.8801163803/kodexa_cli/charts/extension-pack/templates/NOTES.txt
--rw-r--r--   0        0        0     1852 2024-04-23 13:19:49.407059 kodexa_cli-7.0.8801163803/kodexa_cli/charts/extension-pack/templates/_helpers.tpl
--rw-r--r--   0        0        0      324 2024-04-23 13:19:49.407059 kodexa_cli-7.0.8801163803/kodexa_cli/charts/extension-pack/templates/configmap.yaml
--rw-r--r--   0        0        0      250 2024-04-23 13:19:49.407059 kodexa_cli-7.0.8801163803/kodexa_cli/charts/extension-pack/values.yaml
--rw-r--r--   0        0        0      402 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/charts/resource-container/Dockerfile
--rw-r--r--   0        0        0      174 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/charts/resource-container/health-check.conf
--rw-r--r--   0        0        0        0 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/charts/resource-container/index.html
--rw-r--r--   0        0        0      349 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/charts/resource-pack/.helmignore
--rw-r--r--   0        0        0      140 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/charts/resource-pack/Chart.yaml
--rw-r--r--   0        0        0     1528 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/charts/resource-pack/templates/_helpers.tpl
--rw-r--r--   0        0        0     1791 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/charts/resource-pack/templates/deployment.yaml
--rw-r--r--   0        0        0      410 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/charts/resource-pack/templates/service.yaml
--rw-r--r--   0        0        0      330 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/charts/resource-pack/values.yaml
--rw-r--r--   0        0        0    49226 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/cli.py
--rw-r--r--   0        0        0     7641 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/documentation.py
--rw-r--r--   0        0        0      134 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/templates/action.jinja2
--rw-r--r--   0        0        0     1356 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/templates/assistant.jinja2
--rw-r--r--   0        0        0     1021 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/templates/content-taxon.jinja2
--rw-r--r--   0        0        0      328 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/templates/data-store.jinja2
--rw-r--r--   0        0        0      707 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/templates/document-store.jinja2
--rw-r--r--   0        0        0       30 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/templates/extension-pack.jinja2
--rw-r--r--   0        0        0      818 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/templates/header.jinja2
--rw-r--r--   0        0        0      343 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/templates/index.jinja2
--rw-r--r--   0        0        0       30 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/templates/model-runtime.jinja2
--rw-r--r--   0        0        0     2999 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/templates/model.jinja2
--rw-r--r--   0        0        0     1137 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/templates/options.jinja2
--rw-r--r--   0        0        0        0 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/templates/overview.jinja2
--rw-r--r--   0        0        0      722 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/templates/processing-taxon.jinja2
--rw-r--r--   0        0        0       30 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/templates/project-template.jinja2
--rw-r--r--   0        0        0       30 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/templates/store.jinja2
--rw-r--r--   0        0        0      492 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/templates/taxon.jinja2
--rw-r--r--   0        0        0      273 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/templates/taxonomy-labels.jinja2
--rw-r--r--   0        0        0      534 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/templates/taxonomy-structure.jinja2
--rw-r--r--   0        0        0      269 2024-04-23 13:19:49.411059 kodexa_cli-7.0.8801163803/kodexa_cli/templates/taxonomy.jinja2
--rw-r--r--   0        0        0      808 2024-04-23 13:19:58.103111 kodexa_cli-7.0.8801163803/pyproject.toml
--rw-r--r--   0        0        0     2711 1970-01-01 00:00:00.000000 kodexa_cli-7.0.8801163803/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-24 15:49:18.124251 kodexa_cli-7.0.8819456706/LICENSE
+-rw-r--r--   0        0        0     2101 2024-04-24 15:49:18.124251 kodexa_cli-7.0.8819456706/README.md
+-rw-r--r--   0        0        0       64 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/__init__.py
+-rw-r--r--   0        0        0      349 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/charts/extension-pack/.helmignore
+-rw-r--r--   0        0        0      146 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/charts/extension-pack/Chart.yaml
+-rw-r--r--   0        0        0        0 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/charts/extension-pack/resources/.gitkeep
+-rw-r--r--   0        0        0       38 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/charts/extension-pack/templates/NOTES.txt
+-rw-r--r--   0        0        0     1852 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/charts/extension-pack/templates/_helpers.tpl
+-rw-r--r--   0        0        0      324 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/charts/extension-pack/templates/configmap.yaml
+-rw-r--r--   0        0        0      250 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/charts/extension-pack/values.yaml
+-rw-r--r--   0        0        0      402 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/charts/resource-container/Dockerfile
+-rw-r--r--   0        0        0      174 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/charts/resource-container/health-check.conf
+-rw-r--r--   0        0        0        0 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/charts/resource-container/index.html
+-rw-r--r--   0        0        0      349 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/charts/resource-pack/.helmignore
+-rw-r--r--   0        0        0      140 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/charts/resource-pack/Chart.yaml
+-rw-r--r--   0        0        0     1528 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/charts/resource-pack/templates/_helpers.tpl
+-rw-r--r--   0        0        0     1791 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/charts/resource-pack/templates/deployment.yaml
+-rw-r--r--   0        0        0      410 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/charts/resource-pack/templates/service.yaml
+-rw-r--r--   0        0        0      330 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/charts/resource-pack/values.yaml
+-rw-r--r--   0        0        0    49833 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/cli.py
+-rw-r--r--   0        0        0     7641 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/documentation.py
+-rw-r--r--   0        0        0      134 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/templates/action.jinja2
+-rw-r--r--   0        0        0     1356 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/templates/assistant.jinja2
+-rw-r--r--   0        0        0     1021 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/templates/content-taxon.jinja2
+-rw-r--r--   0        0        0      328 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/templates/data-store.jinja2
+-rw-r--r--   0        0        0      707 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/templates/document-store.jinja2
+-rw-r--r--   0        0        0       30 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/templates/extension-pack.jinja2
+-rw-r--r--   0        0        0      818 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/templates/header.jinja2
+-rw-r--r--   0        0        0      343 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/templates/index.jinja2
+-rw-r--r--   0        0        0       30 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/templates/model-runtime.jinja2
+-rw-r--r--   0        0        0     2999 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/templates/model.jinja2
+-rw-r--r--   0        0        0     1137 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/templates/options.jinja2
+-rw-r--r--   0        0        0        0 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/templates/overview.jinja2
+-rw-r--r--   0        0        0      722 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/templates/processing-taxon.jinja2
+-rw-r--r--   0        0        0       30 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/templates/project-template.jinja2
+-rw-r--r--   0        0        0       30 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/templates/store.jinja2
+-rw-r--r--   0        0        0      492 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/templates/taxon.jinja2
+-rw-r--r--   0        0        0      273 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/templates/taxonomy-labels.jinja2
+-rw-r--r--   0        0        0      534 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/templates/taxonomy-structure.jinja2
+-rw-r--r--   0        0        0      269 2024-04-24 15:49:18.128252 kodexa_cli-7.0.8819456706/kodexa_cli/templates/taxonomy.jinja2
+-rw-r--r--   0        0        0      808 2024-04-24 15:49:26.892239 kodexa_cli-7.0.8819456706/pyproject.toml
+-rw-r--r--   0        0        0     2711 1970-01-01 00:00:00.000000 kodexa_cli-7.0.8819456706/PKG-INFO
```

### Comparing `kodexa_cli-7.0.8801163803/LICENSE` & `kodexa_cli-7.0.8819456706/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8801163803/README.md` & `kodexa_cli-7.0.8819456706/README.md`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8801163803/kodexa_cli/charts/extension-pack/templates/_helpers.tpl` & `kodexa_cli-7.0.8819456706/kodexa_cli/charts/extension-pack/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8801163803/kodexa_cli/charts/resource-pack/templates/_helpers.tpl` & `kodexa_cli-7.0.8819456706/kodexa_cli/charts/resource-pack/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8801163803/kodexa_cli/charts/resource-pack/templates/deployment.yaml` & `kodexa_cli-7.0.8819456706/kodexa_cli/charts/resource-pack/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8801163803/kodexa_cli/cli.py` & `kodexa_cli-7.0.8819456706/kodexa_cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 from datetime import datetime
 from getpass import getpass
 from pathlib import Path
 from shutil import copyfile
 from typing import Optional
 
 import click
+import pkg_resources
+import requests
 import yaml
 from functional import seq
 from kodexa.model import ModelContentMetadata
 from kodexa.platform.client import (
     ModelStoreEndpoint,
     PageDocumentFamilyEndpoint,
     DocumentFamilyEndpoint,
@@ -210,14 +212,29 @@
     global GLOBAL_IGNORE_COMPLETE
     GLOBAL_IGNORE_COMPLETE = False
     print("")
     try:
         # Record the starting time of the function execution
         start_time = datetime.now().replace(microsecond=0)
 
+        cli_version = pkg_resources.get_distribution("kodexa").version
+
+        # Check Pypi for the latest version
+        try:
+            latest_version = seq(["https://pypi.org/pypi/kodexa/json"]).map(
+                lambda url: json.loads(requests.get(url).text)
+            ).map(lambda data: data["info"]["version"]).first()
+
+            if latest_version != cli_version:
+                print(
+                    f"New version of Kodexa CLI available: {latest_version} (you have {cli_version})"
+                )
+        except:
+            print("Unable to check for latest version")
+
         try:
             print(f"Using profile {get_current_kodexa_profile()} @ {get_current_kodexa_url()}\n")
         except:
             print("Unable to load profile")
 
         # Call the cli() function
         cli()
@@ -1157,16 +1174,14 @@
 @cli.command()
 @pass_info
 def version(_: Info):
     """
     Get the version of the CLI
 
     """
-    import pkg_resources
-
     print("Kodexa Version:", pkg_resources.get_distribution("kodexa").version)
 
 
 @cli.command()
 @click.option(
     "--path",
     default=os.getcwd(),
```

### Comparing `kodexa_cli-7.0.8801163803/kodexa_cli/documentation.py` & `kodexa_cli-7.0.8819456706/kodexa_cli/documentation.py`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8801163803/kodexa_cli/templates/assistant.jinja2` & `kodexa_cli-7.0.8819456706/kodexa_cli/templates/assistant.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8801163803/kodexa_cli/templates/content-taxon.jinja2` & `kodexa_cli-7.0.8819456706/kodexa_cli/templates/content-taxon.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8801163803/kodexa_cli/templates/document-store.jinja2` & `kodexa_cli-7.0.8819456706/kodexa_cli/templates/document-store.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8801163803/kodexa_cli/templates/header.jinja2` & `kodexa_cli-7.0.8819456706/kodexa_cli/templates/header.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8801163803/kodexa_cli/templates/model.jinja2` & `kodexa_cli-7.0.8819456706/kodexa_cli/templates/model.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8801163803/kodexa_cli/templates/options.jinja2` & `kodexa_cli-7.0.8819456706/kodexa_cli/templates/options.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8801163803/kodexa_cli/templates/processing-taxon.jinja2` & `kodexa_cli-7.0.8819456706/kodexa_cli/templates/processing-taxon.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8801163803/kodexa_cli/templates/taxonomy-structure.jinja2` & `kodexa_cli-7.0.8819456706/kodexa_cli/templates/taxonomy-structure.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8801163803/pyproject.toml` & `kodexa_cli-7.0.8819456706/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa-cli"
-version = "7.0.08801163803"
+version = "7.0.08819456706"
 description = "Command Line Tools for Kodexa"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>", "John Patrick Sese <jp@kodexa.com>"]
 readme = "README.md"
 packages = [{include = "kodexa_cli"}]
 
 [tool.poetry.scripts]
 kodexa = 'kodexa_cli.cli:safe_entry_point'
```

### Comparing `kodexa_cli-7.0.8801163803/PKG-INFO` & `kodexa_cli-7.0.8819456706/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa-cli
-Version: 7.0.8801163803
+Version: 7.0.8819456706
 Summary: Command Line Tools for Kodexa
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

