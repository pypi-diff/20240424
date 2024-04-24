# Comparing `tmp/climb_onyx_client-4.2.0.tar.gz` & `tmp/climb_onyx_client-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climb_onyx_client-4.2.0.tar", last modified: Tue Apr 16 11:16:14 2024, max compression
+gzip compressed data, was "climb_onyx_client-4.3.0.tar", last modified: Wed Apr 24 15:15:25 2024, max compression
```

## Comparing `climb_onyx_client-4.2.0.tar` & `climb_onyx_client-4.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:16:14.711441 climb_onyx_client-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-16 11:16:10.000000 climb_onyx_client-4.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-16 11:16:14.711441 climb_onyx_client-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-16 11:16:10.000000 climb_onyx_client-4.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:16:14.707441 climb_onyx_client-4.2.0/climb_onyx_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-16 11:16:14.000000 climb_onyx_client-4.2.0/climb_onyx_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-16 11:16:14.000000 climb_onyx_client-4.2.0/climb_onyx_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 11:16:14.000000 climb_onyx_client-4.2.0/climb_onyx_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-16 11:16:14.000000 climb_onyx_client-4.2.0/climb_onyx_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-16 11:16:14.000000 climb_onyx_client-4.2.0/climb_onyx_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-16 11:16:14.000000 climb_onyx_client-4.2.0/climb_onyx_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:16:14.707441 climb_onyx_client-4.2.0/onyx/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-16 11:16:10.000000 climb_onyx_client-4.2.0/onyx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    76127 2024-04-16 11:16:10.000000 climb_onyx_client-4.2.0/onyx/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    32218 2024-04-16 11:16:10.000000 climb_onyx_client-4.2.0/onyx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-16 11:16:10.000000 climb_onyx_client-4.2.0/onyx/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-16 11:16:10.000000 climb_onyx_client-4.2.0/onyx/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-04-16 11:16:10.000000 climb_onyx_client-4.2.0/onyx/field.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 11:16:10.000000 climb_onyx_client-4.2.0/onyx/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 11:16:14.711441 climb_onyx_client-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-16 11:16:10.000000 climb_onyx_client-4.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:16:14.707441 climb_onyx_client-4.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    50429 2024-04-16 11:16:10.000000 climb_onyx_client-4.2.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-16 11:16:10.000000 climb_onyx_client-4.2.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-16 11:16:10.000000 climb_onyx_client-4.2.0/tests/test_field.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:25.332217 climb_onyx_client-4.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 15:15:21.000000 climb_onyx_client-4.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-24 15:15:25.332217 climb_onyx_client-4.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-24 15:15:21.000000 climb_onyx_client-4.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:25.332217 climb_onyx_client-4.3.0/climb_onyx_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-24 15:15:25.000000 climb_onyx_client-4.3.0/climb_onyx_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-24 15:15:25.000000 climb_onyx_client-4.3.0/climb_onyx_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:15:25.000000 climb_onyx_client-4.3.0/climb_onyx_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-24 15:15:25.000000 climb_onyx_client-4.3.0/climb_onyx_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-24 15:15:25.000000 climb_onyx_client-4.3.0/climb_onyx_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 15:15:25.000000 climb_onyx_client-4.3.0/climb_onyx_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:25.332217 climb_onyx_client-4.3.0/onyx/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-24 15:15:21.000000 climb_onyx_client-4.3.0/onyx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76687 2024-04-24 15:15:21.000000 climb_onyx_client-4.3.0/onyx/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32879 2024-04-24 15:15:21.000000 climb_onyx_client-4.3.0/onyx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-24 15:15:21.000000 climb_onyx_client-4.3.0/onyx/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-24 15:15:21.000000 climb_onyx_client-4.3.0/onyx/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-04-24 15:15:21.000000 climb_onyx_client-4.3.0/onyx/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 15:15:21.000000 climb_onyx_client-4.3.0/onyx/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:15:25.332217 climb_onyx_client-4.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-24 15:15:21.000000 climb_onyx_client-4.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:25.332217 climb_onyx_client-4.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    50827 2024-04-24 15:15:21.000000 climb_onyx_client-4.3.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-24 15:15:21.000000 climb_onyx_client-4.3.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-24 15:15:21.000000 climb_onyx_client-4.3.0/tests/test_field.py
```

### Comparing `climb_onyx_client-4.2.0/LICENSE` & `climb_onyx_client-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `climb_onyx_client-4.2.0/PKG-INFO` & `climb_onyx_client-4.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climb-onyx-client
-Version: 4.2.0
+Version: 4.3.0
 Summary: Client program for interacting with Onyx.
 Home-page: https://github.com/CLIMB-TRE/onyx-client
 Author: Thomas Brier
 Author-email: t.brier@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -60,21 +60,24 @@
 │                           [default: None]                                                 │
 │ --password  -p      TEXT  Password for authenticating with Onyx. [env var: ONYX_PASSWORD] │
 │                           [default: None]                                                 │
 │ --version   -v            Show the client version number and exit.                        │
 │ --help      -h            Show this message and exit.                                     │
 ╰───────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ────────────────────────────────────────────────────────────────────────────────╮
-│ projects       View available projects.                                                   │
-│ fields         View the field specification for a project.                                │
-│ choices        View options for a choice field.                                           │
-│ get            Get a record from a project.                                               │
-│ filter         Filter multiple records from a project.                                    │
-│ identify       Get the anonymised identifier for a value on a field.                      │
-│ profile        View profile information.                                                  │
-│ siteusers      View users from the same site.                                             │
-│ auth           Authentication commands.                                                   │
-│ admin          Admin commands.                                                            │
+│ projects    View available projects.                                                      │
+│ types       View available field types.                                                   │
+│ lookups     View available lookups.                                                       │
+│ fields      View the field specification for a project.                                   │
+│ choices     View options for a choice field in a project.                                 │
+│ get         Get a record from a project.                                                  │
+│ filter      Filter multiple records from a project.                                       │
+│ history     View the history of a record in a project.                                    │
+│ identify    Get the anonymised identifier for a value on a field.                         │
+│ profile     View profile information.                                                     │
+│ siteusers   View users from the same site.                                                │
+│ auth        Authentication commands.                                                      │
+│ admin       Admin commands.                                                               │
 ╰───────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
 For more information, check out the [documentation](https://climb-tre.github.io/onyx-client/).
```

### Comparing `climb_onyx_client-4.2.0/README.md` & `climb_onyx_client-4.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -44,21 +44,24 @@
 │                           [default: None]                                                 │
 │ --password  -p      TEXT  Password for authenticating with Onyx. [env var: ONYX_PASSWORD] │
 │                           [default: None]                                                 │
 │ --version   -v            Show the client version number and exit.                        │
 │ --help      -h            Show this message and exit.                                     │
 ╰───────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ────────────────────────────────────────────────────────────────────────────────╮
-│ projects       View available projects.                                                   │
-│ fields         View the field specification for a project.                                │
-│ choices        View options for a choice field.                                           │
-│ get            Get a record from a project.                                               │
-│ filter         Filter multiple records from a project.                                    │
-│ identify       Get the anonymised identifier for a value on a field.                      │
-│ profile        View profile information.                                                  │
-│ siteusers      View users from the same site.                                             │
-│ auth           Authentication commands.                                                   │
-│ admin          Admin commands.                                                            │
+│ projects    View available projects.                                                      │
+│ types       View available field types.                                                   │
+│ lookups     View available lookups.                                                       │
+│ fields      View the field specification for a project.                                   │
+│ choices     View options for a choice field in a project.                                 │
+│ get         Get a record from a project.                                                  │
+│ filter      Filter multiple records from a project.                                       │
+│ history     View the history of a record in a project.                                    │
+│ identify    Get the anonymised identifier for a value on a field.                         │
+│ profile     View profile information.                                                     │
+│ siteusers   View users from the same site.                                                │
+│ auth        Authentication commands.                                                      │
+│ admin       Admin commands.                                                               │
 ╰───────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
 For more information, check out the [documentation](https://climb-tre.github.io/onyx-client/).
```

### Comparing `climb_onyx_client-4.2.0/climb_onyx_client.egg-info/PKG-INFO` & `climb_onyx_client-4.3.0/climb_onyx_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climb-onyx-client
-Version: 4.2.0
+Version: 4.3.0
 Summary: Client program for interacting with Onyx.
 Home-page: https://github.com/CLIMB-TRE/onyx-client
 Author: Thomas Brier
 Author-email: t.brier@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -60,21 +60,24 @@
 │                           [default: None]                                                 │
 │ --password  -p      TEXT  Password for authenticating with Onyx. [env var: ONYX_PASSWORD] │
 │                           [default: None]                                                 │
 │ --version   -v            Show the client version number and exit.                        │
 │ --help      -h            Show this message and exit.                                     │
 ╰───────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Commands ────────────────────────────────────────────────────────────────────────────────╮
-│ projects       View available projects.                                                   │
-│ fields         View the field specification for a project.                                │
-│ choices        View options for a choice field.                                           │
-│ get            Get a record from a project.                                               │
-│ filter         Filter multiple records from a project.                                    │
-│ identify       Get the anonymised identifier for a value on a field.                      │
-│ profile        View profile information.                                                  │
-│ siteusers      View users from the same site.                                             │
-│ auth           Authentication commands.                                                   │
-│ admin          Admin commands.                                                            │
+│ projects    View available projects.                                                      │
+│ types       View available field types.                                                   │
+│ lookups     View available lookups.                                                       │
+│ fields      View the field specification for a project.                                   │
+│ choices     View options for a choice field in a project.                                 │
+│ get         Get a record from a project.                                                  │
+│ filter      Filter multiple records from a project.                                       │
+│ history     View the history of a record in a project.                                    │
+│ identify    Get the anonymised identifier for a value on a field.                         │
+│ profile     View profile information.                                                     │
+│ siteusers   View users from the same site.                                                │
+│ auth        Authentication commands.                                                      │
+│ admin       Admin commands.                                                               │
 ╰───────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
 For more information, check out the [documentation](https://climb-tre.github.io/onyx-client/).
```

### Comparing `climb_onyx_client-4.2.0/onyx/api.py` & `climb_onyx_client-4.3.0/onyx/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1173,24 +1173,24 @@
         """
 
         response = super().fields(project)
         response.raise_for_status()
         return response.json()["data"]
 
     @onyx_errors
-    def choices(self, project: str, field: str) -> List[str]:
+    def choices(self, project: str, field: str) -> Dict[str, Dict[str, Any]]:
         """
         View choices for a field.
 
         Args:
             project: Name of the project.
             field: Choice field on the project.
 
         Returns:
-            List of choices for the field.
+            Dictionary mapping choices to information about the choice.
 
         Examples:
             ```python
             import os
             from onyx import OnyxConfig, OnyxEnv, OnyxClient
 
             config = OnyxConfig(
@@ -1199,15 +1199,32 @@
             )
 
             with OnyxClient(config) as client:
                 choices = client.choices("project", "country")
             ```
             ```python
             >>> choices
-            ["ENG", "WALES", "SCOT", "NI"]
+            {
+                "ENG": {
+                    "description": "England",
+                    "is_active" : True,
+                },
+                "WALES": {
+                    "description": "Wales",
+                    "is_active" : True,
+                },
+                "SCOT": {
+                    "description": "Scotland",
+                    "is_active" : True,
+                },
+                "NI": {
+                    "description": "Northern Ireland",
+                    "is_active" : True,
+                },
+            }
             ```
         """
 
         response = super().choices(project, field)
         response.raise_for_status()
         return response.json()["data"]
```

### Comparing `climb_onyx_client-4.2.0/onyx/cli.py` & `climb_onyx_client-4.3.0/onyx/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,14 +260,19 @@
     FILTER = "[bold magenta]filter[/]"
     IDENTIFY = "[bold white]identify[/]"
     ADD = "[bold green]add[/]"
     CHANGE = "[bold yellow]change[/]"
     DELETE = "[bold red]delete[/]"
 
 
+class ActiveStatus(enum.Enum):
+    ACTIVE = "[bold green]active[/]"
+    INACTIVE = "[bold red]inactive[/]"
+
+
 def format_action(action: str) -> str:
     """
     Format an action and apply its colour.
 
     Args:
         action: The action to format.
 
@@ -623,17 +628,31 @@
         field = parse_extra_option([field])[0]
         choices = api.client.choices(project, field)
 
         if format == InfoFormats.TABLE:
             table = Table(
                 show_lines=True,
             )
-            table.add_column("Field")
-            table.add_column("Values")
-            table.add_row(field, ", ".join(choices))
+            table.add_column("Choice")
+            table.add_column("Description")
+            table.add_column("Status")
+            for choice, choice_info in choices.items():
+                active_status = choice_info.get("is_active")
+                if active_status == True:
+                    active_status = ActiveStatus.ACTIVE.value
+                elif active_status == False:
+                    active_status = ActiveStatus.INACTIVE.value
+                else:
+                    active_status = ""
+
+                table.add_row(
+                    choice,
+                    choice_info.get("description", ""),
+                    active_status,
+                )
             console.print(table)
         else:
             typer.echo(json_dump_pretty(choices))
     except Exception as e:
         handle_error(e)
```

### Comparing `climb_onyx_client-4.2.0/onyx/config.py` & `climb_onyx_client-4.3.0/onyx/config.py`

 * *Files identical despite different names*

### Comparing `climb_onyx_client-4.2.0/onyx/exceptions.py` & `climb_onyx_client-4.3.0/onyx/exceptions.py`

 * *Files identical despite different names*

### Comparing `climb_onyx_client-4.2.0/onyx/field.py` & `climb_onyx_client-4.3.0/onyx/field.py`

 * *Files identical despite different names*

### Comparing `climb_onyx_client-4.2.0/setup.py` & `climb_onyx_client-4.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `climb_onyx_client-4.2.0/tests/test_api.py` & `climb_onyx_client-4.3.0/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,18 +133,32 @@
     },
 }
 CHOICE_FIELD = "country"
 CHOICES_DATA = {
     "status": "success",
     "code": 200,
     "data": [
-        "England",
-        "N. Ireland",
-        "Scotland",
-        "Wales",
+        {
+            "eng": {
+                "description": "England",
+                "is_active": True,
+            },
+            "ni": {
+                "description": "N. Ireland",
+                "is_active": True,
+            },
+            "scot": {
+                "description": "Scotland",
+                "is_active": True,
+            },
+            "wales": {
+                "description": "Wales",
+                "is_active": True,
+            },
+        }
     ],
 }
 CLIMB_ID = "C-0123456789"
 GET_DATA = {
     "status": "success",
     "code": 200,
     "data": {
```

### Comparing `climb_onyx_client-4.2.0/tests/test_config.py` & `climb_onyx_client-4.3.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `climb_onyx_client-4.2.0/tests/test_field.py` & `climb_onyx_client-4.3.0/tests/test_field.py`

 * *Files identical despite different names*

