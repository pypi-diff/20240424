# Comparing `tmp/airbyte_source_marketo-1.3.0.tar.gz` & `tmp/airbyte_source_marketo-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_marketo-1.3.0.tar", max compression
+gzip compressed data, was "airbyte_source_marketo-1.3.2.tar", max compression
```

## Comparing `airbyte_source_marketo-1.3.0.tar` & `airbyte_source_marketo-1.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     4514 2024-03-21 01:47:20.565994 airbyte_source_marketo-1.3.0/README.md
--rw-r--r--   0        0        0      772 2024-03-21 02:05:25.195585 airbyte_source_marketo-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     1171 2024-03-21 01:47:20.565994 airbyte_source_marketo-1.3.0/source_marketo/__init__.py
--rw-r--r--   0        0        0      233 2024-03-21 01:47:20.565994 airbyte_source_marketo-1.3.0/source_marketo/run.py
--rw-r--r--   0        0        0      789 2024-03-21 01:47:20.565994 airbyte_source_marketo-1.3.0/source_marketo/schemas/activity_types.json
--rw-r--r--   0        0        0      726 2024-03-21 01:47:20.565994 airbyte_source_marketo-1.3.0/source_marketo/schemas/campaigns.json
--rw-r--r--   0        0        0     5898 2024-03-21 01:47:20.565994 airbyte_source_marketo-1.3.0/source_marketo/schemas/leads.json
--rw-r--r--   0        0        0      617 2024-03-21 01:47:20.565994 airbyte_source_marketo-1.3.0/source_marketo/schemas/lists.json
--rw-r--r--   0        0        0     1124 2024-03-21 01:47:20.565994 airbyte_source_marketo-1.3.0/source_marketo/schemas/programs.json
--rw-r--r--   0        0        0      888 2024-03-21 01:47:20.565994 airbyte_source_marketo-1.3.0/source_marketo/schemas/segmentations.json
--rw-r--r--   0        0        0    23327 2024-03-21 01:47:20.565994 airbyte_source_marketo-1.3.0/source_marketo/source.py
--rw-r--r--   0        0        0     1803 2024-03-21 01:47:20.565994 airbyte_source_marketo-1.3.0/source_marketo/spec.json
--rw-r--r--   0        0        0     2069 2024-03-21 01:47:20.565994 airbyte_source_marketo-1.3.0/source_marketo/utils.py
--rw-r--r--   0        0        0     5218 1970-01-01 00:00:00.000000 airbyte_source_marketo-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     4514 2024-04-24 19:26:18.579111 airbyte_source_marketo-1.3.2/README.md
+-rw-r--r--   0        0        0      776 2024-04-24 19:29:40.282623 airbyte_source_marketo-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1171 2024-04-24 19:26:18.579111 airbyte_source_marketo-1.3.2/source_marketo/__init__.py
+-rw-r--r--   0        0        0      233 2024-04-24 19:26:18.579111 airbyte_source_marketo-1.3.2/source_marketo/run.py
+-rw-r--r--   0        0        0     1542 2024-04-24 19:26:18.579111 airbyte_source_marketo-1.3.2/source_marketo/schemas/activity_types.json
+-rw-r--r--   0        0        0     1471 2024-04-24 19:26:18.579111 airbyte_source_marketo-1.3.2/source_marketo/schemas/campaigns.json
+-rw-r--r--   0        0        0    11717 2024-04-24 19:26:18.579111 airbyte_source_marketo-1.3.2/source_marketo/schemas/leads.json
+-rw-r--r--   0        0        0     1158 2024-04-24 19:26:18.579111 airbyte_source_marketo-1.3.2/source_marketo/schemas/lists.json
+-rw-r--r--   0        0        0     2254 2024-04-24 19:26:18.579111 airbyte_source_marketo-1.3.2/source_marketo/schemas/programs.json
+-rw-r--r--   0        0        0     1620 2024-04-24 19:26:18.579111 airbyte_source_marketo-1.3.2/source_marketo/schemas/segmentations.json
+-rw-r--r--   0        0        0    23327 2024-04-24 19:26:18.579111 airbyte_source_marketo-1.3.2/source_marketo/source.py
+-rw-r--r--   0        0        0     1803 2024-04-24 19:26:18.579111 airbyte_source_marketo-1.3.2/source_marketo/spec.json
+-rw-r--r--   0        0        0     2069 2024-04-24 19:26:18.579111 airbyte_source_marketo-1.3.2/source_marketo/utils.py
+-rw-r--r--   0        0        0     5220 1970-01-01 00:00:00.000000 airbyte_source_marketo-1.3.2/PKG-INFO
```

### Comparing `airbyte_source_marketo-1.3.0/README.md` & `airbyte_source_marketo-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_marketo-1.3.0/pyproject.toml` & `airbyte_source_marketo-1.3.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "1.3.0"
+version = "1.3.2"
 name = "airbyte-source-marketo"
 description = "Source implementation for Marketo."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_marketo" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "^0"
+airbyte-cdk = "0.80.0"
 
 [tool.poetry.scripts]
 source-marketo = "source_marketo.run:run"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.1"
 requests-mock = "^1.11.0"
```

### Comparing `airbyte_source_marketo-1.3.0/source_marketo/__init__.py` & `airbyte_source_marketo-1.3.2/source_marketo/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_marketo-1.3.0/source_marketo/schemas/programs.json` & `airbyte_source_marketo-1.3.2/source_marketo/schemas/activity_types.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7453703703703702%*

 * *Differences: {"'properties'": "{'id': {'type': {insert: [(1, 'integer')], delete: [0]}, 'description': 'The "*

 * *                 "unique identifier of the activity type.'}, 'name': {'type': {insert: [(1, "*

 * *                 "'string')], delete: [0]}, 'description': 'The name of the activity type.'}, "*

 * *                 "'description': {'description': 'A description of the activity type.'}, "*

 * *                 "'primaryAttribute': OrderedDict([('description', 'The primary attribute of the "*

 * *                 "activity, which c […]*

```diff
@@ -1,109 +1,83 @@
 {
     "additionalProperties": true,
     "properties": {
-        "channel": {
+        "attributes": {
+            "description": "An array containing the activity attributes including details like type, value, timestamp, etc.",
+            "items": {
+                "description": "Properties related to a specific activity attribute.",
+                "properties": {
+                    "dataType": {
+                        "description": "The data type of the attribute.",
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    },
+                    "name": {
+                        "description": "The name of the attribute.",
+                        "type": [
+                            "null",
+                            "string"
+                        ]
+                    }
+                },
+                "type": [
+                    "null",
+                    "object"
+                ]
+            },
+            "type": [
+                "null",
+                "array"
+            ]
+        },
+        "description": {
+            "description": "A description of the activity type.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "createdAt": {
-            "format": "date-time",
+        "id": {
+            "description": "The unique identifier of the activity type.",
             "type": [
-                "string",
-                "null"
+                "null",
+                "integer"
             ]
         },
-        "description": {
+        "name": {
+            "description": "The name of the activity type.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "folder": {
+        "primaryAttribute": {
+            "description": "The primary attribute of the activity, which could be the most essential or relevant data point.",
             "properties": {
-                "folderName": {
+                "dataType": {
+                    "description": "The data type of the primary attribute.",
                     "type": [
                         "null",
                         "string"
                     ]
                 },
-                "type": {
+                "name": {
+                    "description": "The name of the primary attribute.",
                     "type": [
                         "null",
                         "string"
                     ]
-                },
-                "value": {
-                    "type": [
-                        "null",
-                        "integer"
-                    ]
                 }
             },
             "type": [
-                "object",
-                "null"
-            ]
-        },
-        "headStart": {
-            "type": [
                 "null",
-                "boolean"
-            ]
-        },
-        "id": {
-            "type": [
-                "integer",
-                "null"
-            ]
-        },
-        "isHeadStart": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "name": {
-            "type": [
-                "string",
-                "null"
-            ]
-        },
-        "status": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "type": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "updatedAt": {
-            "format": "date-time",
-            "type": [
-                "string",
-                "null"
-            ]
-        },
-        "url": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "workspace": {
-            "type": [
-                "null",
-                "string"
+                "object"
             ]
         }
     },
     "type": [
-        "object",
-        "null"
+        "null",
+        "object"
     ]
 }
```

### Comparing `airbyte_source_marketo-1.3.0/source_marketo/source.py` & `airbyte_source_marketo-1.3.2/source_marketo/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_marketo-1.3.0/source_marketo/spec.json` & `airbyte_source_marketo-1.3.2/source_marketo/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_marketo-1.3.0/source_marketo/utils.py` & `airbyte_source_marketo-1.3.2/source_marketo/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_marketo-1.3.0/PKG-INFO` & `airbyte_source_marketo-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-marketo
-Version: 1.3.0
+Version: 1.3.2
 Summary: Source implementation for Marketo.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (>=0,<1)
+Requires-Dist: airbyte-cdk (==0.80.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/marketo
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Marketo source connector
```

