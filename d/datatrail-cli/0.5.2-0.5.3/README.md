# Comparing `tmp/datatrail_cli-0.5.2.tar.gz` & `tmp/datatrail_cli-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatrail_cli-0.5.2.tar", max compression
+gzip compressed data, was "datatrail_cli-0.5.3.tar", max compression
```

## Comparing `datatrail_cli-0.5.2.tar` & `datatrail_cli-0.5.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1080 2024-04-09 18:55:51.200617 datatrail_cli-0.5.2/LICENSE
--rw-r--r--   0        0        0     3558 2024-04-09 18:55:51.200617 datatrail_cli-0.5.2/README.md
--rw-r--r--   0        0        0      214 2024-04-09 18:55:51.208618 datatrail_cli-0.5.2/dtcli/__init__.py
--rw-r--r--   0        0        0     4590 2024-04-09 18:55:51.208618 datatrail_cli-0.5.2/dtcli/clear.py
--rw-r--r--   0        0        0     1437 2024-04-09 18:55:51.208618 datatrail_cli-0.5.2/dtcli/cli.py
--rw-r--r--   0        0        0     4037 2024-04-09 18:55:51.208618 datatrail_cli-0.5.2/dtcli/config.py
--rw-r--r--   0        0        0     1062 2024-04-09 18:55:51.208618 datatrail_cli-0.5.2/dtcli/config.yaml
--rw-r--r--   0        0        0     3806 2024-04-09 18:55:51.208618 datatrail_cli-0.5.2/dtcli/ls.py
--rw-r--r--   0        0        0     7846 2024-04-09 18:55:51.208618 datatrail_cli-0.5.2/dtcli/ps.py
--rw-r--r--   0        0        0     4576 2024-04-09 18:55:51.208618 datatrail_cli-0.5.2/dtcli/pull.py
--rw-r--r--   0        0        0    15634 2024-04-09 18:55:51.208618 datatrail_cli-0.5.2/dtcli/src/functions.py
--rw-r--r--   0        0        0     9241 2024-04-09 18:55:51.208618 datatrail_cli-0.5.2/dtcli/utilities/cadcclient.py
--rw-r--r--   0        0        0     3089 2024-04-09 18:55:51.208618 datatrail_cli-0.5.2/dtcli/utilities/utilities.py
--rw-r--r--   0        0        0     1073 2024-04-09 18:55:51.208618 datatrail_cli-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     4522 1970-01-01 00:00:00.000000 datatrail_cli-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-04-24 18:29:31.079116 datatrail_cli-0.5.3/LICENSE
+-rw-r--r--   0        0        0     3558 2024-04-24 18:29:31.079116 datatrail_cli-0.5.3/README.md
+-rw-r--r--   0        0        0      214 2024-04-24 18:29:31.087116 datatrail_cli-0.5.3/dtcli/__init__.py
+-rw-r--r--   0        0        0     4590 2024-04-24 18:29:31.087116 datatrail_cli-0.5.3/dtcli/clear.py
+-rw-r--r--   0        0        0     1437 2024-04-24 18:29:31.087116 datatrail_cli-0.5.3/dtcli/cli.py
+-rw-r--r--   0        0        0     4037 2024-04-24 18:29:31.087116 datatrail_cli-0.5.3/dtcli/config.py
+-rw-r--r--   0        0        0     1062 2024-04-24 18:29:31.087116 datatrail_cli-0.5.3/dtcli/config.yaml
+-rw-r--r--   0        0        0     3924 2024-04-24 18:29:31.087116 datatrail_cli-0.5.3/dtcli/ls.py
+-rw-r--r--   0        0        0     7992 2024-04-24 18:29:31.087116 datatrail_cli-0.5.3/dtcli/ps.py
+-rw-r--r--   0        0        0     4576 2024-04-24 18:29:31.087116 datatrail_cli-0.5.3/dtcli/pull.py
+-rw-r--r--   0        0        0    15784 2024-04-24 18:29:31.087116 datatrail_cli-0.5.3/dtcli/src/functions.py
+-rw-r--r--   0        0        0     9241 2024-04-24 18:29:31.087116 datatrail_cli-0.5.3/dtcli/utilities/cadcclient.py
+-rw-r--r--   0        0        0     3089 2024-04-24 18:29:31.087116 datatrail_cli-0.5.3/dtcli/utilities/utilities.py
+-rw-r--r--   0        0        0     1073 2024-04-24 18:29:31.087116 datatrail_cli-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     4522 1970-01-01 00:00:00.000000 datatrail_cli-0.5.3/PKG-INFO
```

### Comparing `datatrail_cli-0.5.2/LICENSE` & `datatrail_cli-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.2/README.md` & `datatrail_cli-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.2/dtcli/clear.py` & `datatrail_cli-0.5.3/dtcli/clear.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.2/dtcli/cli.py` & `datatrail_cli-0.5.3/dtcli/cli.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.2/dtcli/config.py` & `datatrail_cli-0.5.3/dtcli/config.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.2/dtcli/config.yaml` & `datatrail_cli-0.5.3/dtcli/config.yaml`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.2/dtcli/ls.py` & `datatrail_cli-0.5.3/dtcli/ls.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,16 +71,18 @@
     if "scopes" in results.keys():
         table = Table(
             title="Datatrail: Scopes",
             header_style="magenta",
             title_style="bold magenta",
         )
         table.add_column("Scopes")
-        for s in results["scopes"]:
-            table.add_row(s)
+        for site in ["chime", "kko", "gbo", "hco"]:
+            for s in [_ for _ in results["scopes"] if site in _]:
+                table.add_row(s)
+            table.add_section()
         console.print(table)
 
     if "larger_datasets" in results.keys():
         results["larger_datasets"] = sorted(results["larger_datasets"])
 
         if write:
             with open(f"./larger_datasets_list_{scope}.txt", "w") as file:
```

### Comparing `datatrail_cli-0.5.2/dtcli/ps.py` & `datatrail_cli-0.5.3/dtcli/ps.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,17 +153,20 @@
     policy_table = Table(
         title=f"Datatrail: Policies for {dataset} {scope}",
         header_style="magenta",
         title_style="bold magenta",
         show_footer=True,
         footer_style="bold red",
     )
-    belongs_to = (
-        policies["belongs_to"][0]["name"] if len(policies["belongs_to"]) > 0 else "None"
-    )
+    if len(policies["belongs_to"]) > 1:
+        belongs_to = ", ".join([lgr_ds["name"] for lgr_ds in policies["belongs_to"]])
+    elif len(policies["belongs_to"]) == 1:
+        belongs_to = policies["belongs_to"][0]["name"]
+    else:
+        belongs_to = None
     policy_table.add_column("Policy", style="bold", footer="Belongs to")
     policy_table.add_column("Storage Element", footer=belongs_to)
     policy_table.add_column("Priority")
     policy_table.add_column("Default")
     policy_table.add_column(r"Delete After \[days]")
 
     rp = policies["replication_policy"]
```

### Comparing `datatrail_cli-0.5.2/dtcli/pull.py` & `datatrail_cli-0.5.3/dtcli/pull.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.2/dtcli/src/functions.py` & `datatrail_cli-0.5.3/dtcli/src/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -326,16 +326,20 @@
     # Check if path exists.
     p = Path(path)
     logger.debug(f"Checking if path {path} exists.")
     exists = p.exists()
 
     # Delete files.
     if exists:
-        shutil.rmtree(p)
-        logger.info("Path successfully removed.")
+        if len(p.parents) < 4:
+            logger.critical("Path is a core directory! Cannot delete.")
+            return False
+        else:
+            shutil.rmtree(p)
+            logger.info("Path successfully removed.")
         time.sleep(0.1)
     else:
         logger.info(f"Path {path} not found.")
         return False
 
     # Clear empty parent directories.
     parent = p.parent
```

### Comparing `datatrail_cli-0.5.2/dtcli/utilities/cadcclient.py` & `datatrail_cli-0.5.3/dtcli/utilities/cadcclient.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.2/dtcli/utilities/utilities.py` & `datatrail_cli-0.5.3/dtcli/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.2/pyproject.toml` & `datatrail_cli-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datatrail-cli"
-version = "0.5.2"
+version = "0.5.3"
 description = "CHIME/FRB Datatrail CLI"
 authors = ["CHIME FRB Project Office"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "dtcli" }]
 
 [tool.poetry.dependencies]
```

### Comparing `datatrail_cli-0.5.2/PKG-INFO` & `datatrail_cli-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatrail-cli
-Version: 0.5.2
+Version: 0.5.3
 Summary: CHIME/FRB Datatrail CLI
 License: MIT
 Author: CHIME FRB Project Office
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datatrail-cli Version: 0.5.2 Summary: CHIME/FRB
+Metadata-Version: 2.1 Name: datatrail-cli Version: 0.5.3 Summary: CHIME/FRB
 Datatrail CLI License: MIT Author: CHIME FRB Project Office Requires-Python:
 >=3.8.1,<4.0.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: cadcdata (>=2.5.0,<3.0.0) Requires-Dist: cadctap
 (>=0.9.11,<0.10.0) Requires-Dist: cadcutils (>=1.5.1.1,<2.0.0.0) Requires-Dist:
```

