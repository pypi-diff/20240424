# Comparing `tmp/validio_cli-0.8.0.tar.gz` & `tmp/validio_cli-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validio_cli-0.8.0.tar", max compression
+gzip compressed data, was "validio_cli-0.9.0.tar", max compression
```

## Comparing `validio_cli-0.8.0.tar` & `validio_cli-0.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11340 2023-11-02 13:09:56.144358 validio_cli-0.8.0/LICENSE
--rw-r--r--   0        0        0      227 2023-11-02 13:09:56.144358 validio_cli-0.8.0/README_PUBLIC.md
--rw-r--r--   0        0        0     2169 2023-11-02 13:10:28.633326 validio_cli-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     7151 2023-11-02 13:09:56.145358 validio_cli-0.8.0/validio_cli/__init__.py
--rw-r--r--   0        0        0     2689 2023-11-02 13:09:56.145358 validio_cli-0.8.0/validio_cli/bin/entities/channels.py
--rw-r--r--   0        0        0    14708 2023-11-02 13:09:56.145358 validio_cli-0.8.0/validio_cli/bin/entities/code.py
--rw-r--r--   0        0        0     5010 2023-11-02 13:09:56.145358 validio_cli-0.8.0/validio_cli/bin/entities/config.py
--rw-r--r--   0        0        0     2810 2023-11-02 13:09:56.145358 validio_cli-0.8.0/validio_cli/bin/entities/credentials.py
--rw-r--r--   0        0        0     1807 2023-11-02 13:09:56.145358 validio_cli-0.8.0/validio_cli/bin/entities/dbt.py
--rw-r--r--   0        0        0     7514 2023-11-02 13:09:56.145358 validio_cli-0.8.0/validio_cli/bin/entities/incidents.py
--rw-r--r--   0        0        0     2346 2023-11-02 13:09:56.145358 validio_cli-0.8.0/validio_cli/bin/entities/metrics.py
--rw-r--r--   0        0        0     3221 2023-11-02 13:09:56.145358 validio_cli-0.8.0/validio_cli/bin/entities/notification_rules.py
--rw-r--r--   0        0        0     3317 2023-11-02 13:09:56.145358 validio_cli-0.8.0/validio_cli/bin/entities/recommendations.py
--rw-r--r--   0        0        0     4098 2023-11-02 13:09:56.145358 validio_cli-0.8.0/validio_cli/bin/entities/resources.py
--rw-r--r--   0        0        0     2949 2023-11-02 13:09:56.146358 validio_cli-0.8.0/validio_cli/bin/entities/segmentations.py
--rw-r--r--   0        0        0     1912 2023-11-02 13:09:56.146358 validio_cli-0.8.0/validio_cli/bin/entities/segments.py
--rw-r--r--   0        0        0    37213 2023-11-02 13:09:56.146358 validio_cli-0.8.0/validio_cli/bin/entities/sources.py
--rw-r--r--   0        0        0     1351 2023-11-02 13:09:56.146358 validio_cli-0.8.0/validio_cli/bin/entities/users.py
--rw-r--r--   0        0        0     3802 2023-11-02 13:09:56.146358 validio_cli-0.8.0/validio_cli/bin/entities/validators.py
--rw-r--r--   0        0        0     3139 2023-11-02 13:09:56.146358 validio_cli-0.8.0/validio_cli/bin/entities/windows.py
--rw-r--r--   0        0        0     2374 2023-11-02 13:09:56.146358 validio_cli-0.8.0/validio_cli/bin/main.py
--rw-r--r--   0        0        0     3276 2023-11-02 13:09:56.146358 validio_cli-0.8.0/validio_cli/components.py
--rw-r--r--   0        0        0      272 2023-11-02 13:09:56.146358 validio_cli-0.8.0/validio_cli/metadata.py
--rw-r--r--   0        0        0      630 2023-11-02 13:09:56.146358 validio_cli-0.8.0/validio_cli/namespace.py
--rw-r--r--   0        0        0     1382 2023-11-02 13:09:56.146358 validio_cli-0.8.0/validio_cli/schema.py
--rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 validio_cli-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11340 2023-11-16 20:16:53.917479 validio_cli-0.9.0/LICENSE
+-rw-r--r--   0        0        0      227 2023-11-16 20:16:53.917479 validio_cli-0.9.0/README_PUBLIC.md
+-rw-r--r--   0        0        0     2189 2023-11-16 20:17:17.040456 validio_cli-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     7151 2023-11-16 20:16:53.917479 validio_cli-0.9.0/validio_cli/__init__.py
+-rw-r--r--   0        0        0     2689 2023-11-16 20:16:53.917479 validio_cli-0.9.0/validio_cli/bin/entities/channels.py
+-rw-r--r--   0        0        0    14708 2023-11-16 20:16:53.918479 validio_cli-0.9.0/validio_cli/bin/entities/code.py
+-rw-r--r--   0        0        0     5010 2023-11-16 20:16:53.918479 validio_cli-0.9.0/validio_cli/bin/entities/config.py
+-rw-r--r--   0        0        0     2810 2023-11-16 20:16:53.918479 validio_cli-0.9.0/validio_cli/bin/entities/credentials.py
+-rw-r--r--   0        0        0     1807 2023-11-16 20:16:53.918479 validio_cli-0.9.0/validio_cli/bin/entities/dbt.py
+-rw-r--r--   0        0        0     7540 2023-11-16 20:16:53.918479 validio_cli-0.9.0/validio_cli/bin/entities/incidents.py
+-rw-r--r--   0        0        0     2346 2023-11-16 20:16:53.918479 validio_cli-0.9.0/validio_cli/bin/entities/metrics.py
+-rw-r--r--   0        0        0     3221 2023-11-16 20:16:53.918479 validio_cli-0.9.0/validio_cli/bin/entities/notification_rules.py
+-rw-r--r--   0        0        0     3317 2023-11-16 20:16:53.918479 validio_cli-0.9.0/validio_cli/bin/entities/recommendations.py
+-rw-r--r--   0        0        0     4098 2023-11-16 20:16:53.918479 validio_cli-0.9.0/validio_cli/bin/entities/resources.py
+-rw-r--r--   0        0        0     2949 2023-11-16 20:16:53.918479 validio_cli-0.9.0/validio_cli/bin/entities/segmentations.py
+-rw-r--r--   0        0        0     1912 2023-11-16 20:16:53.918479 validio_cli-0.9.0/validio_cli/bin/entities/segments.py
+-rw-r--r--   0        0        0    36434 2023-11-16 20:16:53.918479 validio_cli-0.9.0/validio_cli/bin/entities/sources.py
+-rw-r--r--   0        0        0     1351 2023-11-16 20:16:53.918479 validio_cli-0.9.0/validio_cli/bin/entities/users.py
+-rw-r--r--   0        0        0     3802 2023-11-16 20:16:53.918479 validio_cli-0.9.0/validio_cli/bin/entities/validators.py
+-rw-r--r--   0        0        0     3139 2023-11-16 20:16:53.918479 validio_cli-0.9.0/validio_cli/bin/entities/windows.py
+-rw-r--r--   0        0        0     2374 2023-11-16 20:16:53.918479 validio_cli-0.9.0/validio_cli/bin/main.py
+-rw-r--r--   0        0        0     3277 2023-11-16 20:16:53.918479 validio_cli-0.9.0/validio_cli/components.py
+-rw-r--r--   0        0        0      273 2023-11-16 20:16:53.918479 validio_cli-0.9.0/validio_cli/metadata.py
+-rw-r--r--   0        0        0      631 2023-11-16 20:16:53.918479 validio_cli-0.9.0/validio_cli/namespace.py
+-rw-r--r--   0        0        0     1382 2023-11-16 20:16:53.918479 validio_cli-0.9.0/validio_cli/schema.py
+-rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 validio_cli-0.9.0/PKG-INFO
```

### Comparing `validio_cli-0.8.0/LICENSE` & `validio_cli-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `validio_cli-0.8.0/pyproject.toml` & `validio_cli-0.9.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "validio-cli"
 # This version does not represent the released version or any tag. For each
 # release we automatically bump this before building and publishing so this
 # should be kept at 0.0.1dev1
-version = "0.8.0"
+version = "0.9.0"
 description = "CLI tool to interact with the Validio platform"
 authors = ["Validio <support@validio.io>"]
 license = "Apache-2.0"
 homepage = "https://validio.io/"
 documentation = "https://docs.validio.io/"
 packages = [{include = "validio_cli"}]
 readme = "README_PUBLIC.md"
@@ -25,14 +25,15 @@
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.263"
 black = "^23.3.0"
 mypy = "^1.2.0"
 validio-sdk = { path = "../validio-sdk", develop = true }
 licensecheck = "^2023.1.1"
+pydantic = "^2.4.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 validio = "validio_cli.bin.main:main"
```

### Comparing `validio_cli-0.8.0/validio_cli/__init__.py` & `validio_cli-0.9.0/validio_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.8.0/validio_cli/bin/entities/channels.py` & `validio_cli-0.9.0/validio_cli/bin/entities/channels.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.8.0/validio_cli/bin/entities/code.py` & `validio_cli-0.9.0/validio_cli/bin/entities/code.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.8.0/validio_cli/bin/entities/config.py` & `validio_cli-0.9.0/validio_cli/bin/entities/config.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.8.0/validio_cli/bin/entities/credentials.py` & `validio_cli-0.9.0/validio_cli/bin/entities/credentials.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.8.0/validio_cli/bin/entities/dbt.py` & `validio_cli-0.9.0/validio_cli/bin/entities/dbt.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.8.0/validio_cli/bin/entities/incidents.py` & `validio_cli-0.9.0/validio_cli/bin/entities/incidents.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,17 +79,20 @@
     if source is not None:
         source_id = await sources.get_source_id(vc, cfg, source, namespace)
         if source_id is None:
             return None
 
     # TODO(UI-2006): These should all support namespace
 
-    incidents: None | list[GetValidatorIncidentsValidatorIncidents] | list[
-        GetValidatorSegmentIncidentsValidatorSegmentIncidents
-    ] | list[GetSegmentIncidentsSegmentIncidents] = None
+    incidents: (
+        None
+        | list[GetValidatorIncidentsValidatorIncidents]
+        | list[GetValidatorSegmentIncidentsValidatorSegmentIncidents]
+        | list[GetSegmentIncidentsSegmentIncidents]
+    ) = None
 
     if validator and segment:
         incidents = await vc.get_validator_segment_incidents(
             ValidatorSegmentIncidentsInput(
                 time_range=TimeRangeInput(
                     start=ended_after,
                     end=ended_before,
```

### Comparing `validio_cli-0.8.0/validio_cli/bin/entities/metrics.py` & `validio_cli-0.9.0/validio_cli/bin/entities/metrics.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.8.0/validio_cli/bin/entities/notification_rules.py` & `validio_cli-0.9.0/validio_cli/bin/entities/notification_rules.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.8.0/validio_cli/bin/entities/recommendations.py` & `validio_cli-0.9.0/validio_cli/bin/entities/recommendations.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.8.0/validio_cli/bin/entities/resources.py` & `validio_cli-0.9.0/validio_cli/bin/entities/resources.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.8.0/validio_cli/bin/entities/segmentations.py` & `validio_cli-0.9.0/validio_cli/bin/entities/segmentations.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.8.0/validio_cli/bin/entities/segments.py` & `validio_cli-0.9.0/validio_cli/bin/entities/segments.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.8.0/validio_cli/bin/entities/sources.py` & `validio_cli-0.9.0/validio_cli/bin/entities/sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,169 +287,159 @@
     if inference_type is None:
         return
 
     match inference_type:
         case "demo":
             await _infer_schema_demo(vc, filename)
         case "kinesis":
-            info = await _multip_prompt(
-                [
-                    (
-                        "Region",
-                        # https://docs.aws.amazon.com/general/latest/gr/ak.html
-                        [
-                            "us-east-2",
-                            "us-east-1",
-                            "us-west-1",
-                            "us-west-2",
-                            "af-south-1",
-                            "ap-east-1",
-                            "ap-south-2",
-                            "ap-southeast-3",
-                            "ap-southeast-4",
-                            "ap-south-1",
-                            "ap-northeast-3",
-                            "ap-northeast-2",
-                            "ap-southeast-1",
-                            "ap-southeast-2",
-                            "ap-northeast-1",
-                            "ca-central-1",
-                            "eu-central-1",
-                            "eu-west-1",
-                            "eu-west-2",
-                            "eu-south-1",
-                            "eu-west-3",
-                            "eu-south-2",
-                            "eu-north-1",
-                            "eu-central-2",
-                            "me-south-1",
-                            "me-central-1",
-                            "sa-east-1",
-                            "us-gov-east-1",
-                            "us-gov-west-1",
-                        ],
-                        "",
-                    ),
-                    ("Stream name", [], ""),
-                    _interactive_message_format_input(),
-                    ("Message schema", [], ""),
-                ]
-            )
+            info = await _multip_prompt([
+                (
+                    "Region",
+                    # https://docs.aws.amazon.com/general/latest/gr/ak.html
+                    [
+                        "us-east-2",
+                        "us-east-1",
+                        "us-west-1",
+                        "us-west-2",
+                        "af-south-1",
+                        "ap-east-1",
+                        "ap-south-2",
+                        "ap-southeast-3",
+                        "ap-southeast-4",
+                        "ap-south-1",
+                        "ap-northeast-3",
+                        "ap-northeast-2",
+                        "ap-southeast-1",
+                        "ap-southeast-2",
+                        "ap-northeast-1",
+                        "ca-central-1",
+                        "eu-central-1",
+                        "eu-west-1",
+                        "eu-west-2",
+                        "eu-south-1",
+                        "eu-west-3",
+                        "eu-south-2",
+                        "eu-north-1",
+                        "eu-central-2",
+                        "me-south-1",
+                        "me-central-1",
+                        "sa-east-1",
+                        "us-gov-east-1",
+                        "us-gov-west-1",
+                    ],
+                    "",
+                ),
+                ("Stream name", [], ""),
+                _interactive_message_format_input(),
+                ("Message schema", [], ""),
+            ])
 
             await _infer_schema_kinesis(
                 vc,
                 filename,
                 credential_id,
                 info.get("region", ""),
                 info.get("stream_name", ""),
                 info.get("message_format", ""),
                 info.get("message_schema", ""),
             )
         case "pubsub":
-            info = await _multip_prompt(
-                [
-                    ("Project", [], ""),
-                    ("Subscription ID", [], ""),
-                    _interactive_message_format_input(),
-                    ("Message schema", [], ""),
-                ]
-            )
+            info = await _multip_prompt([
+                ("Project", [], ""),
+                ("Subscription ID", [], ""),
+                _interactive_message_format_input(),
+                ("Message schema", [], ""),
+            ])
 
             await _infer_schema_pubsub(
                 vc,
                 filename,
                 credential_id,
                 info.get("project", ""),
                 info.get("subscription_id", ""),
                 info.get("message_format", ""),
                 info.get("message_schema", ""),
             )
         case "pubsublite":
-            info = await _multip_prompt(
-                [
-                    ("Project", [], ""),
-                    ("Subscription ID", [], ""),
-                    # https://cloud.google.com/pubsub/lite/docs/locations
-                    (
-                        "Location",
-                        [
-                            "asia-east1",
-                            "asia-east2",
-                            "asia-northeast1",
-                            "asia-northeast2",
-                            "asia-northeast3",
-                            "asia-south1",
-                            "asia-southeast1",
-                            "asia-southeast2",
-                            "australia-southeast1",
-                            "australia-southeast2",
-                            "europe-central2",
-                            "europe-north1",
-                            "europe-west1",
-                            "europe-west2",
-                            "europe-west3",
-                            "europe-west4",
-                            "europe-west6",
-                            "europe-west8",
-                            "europe-west9",
-                            "me-central1",
-                            "northamerica-northeast1",
-                            "me-west1",
-                            "northamerica-northeast2",
-                            "southamerica-east1",
-                            "us-central1",
-                            "us-east1",
-                            "us-east4",
-                            "us-east5",
-                            "us-west1",
-                            "us-west2",
-                            "us-west3",
-                            "us-west4",
-                        ],
-                        "",
-                    ),
-                    _interactive_message_format_input(),
-                    ("Message schema", [], ""),
-                ]
-            )
+            info = await _multip_prompt([
+                ("Project", [], ""),
+                ("Subscription ID", [], ""),
+                # https://cloud.google.com/pubsub/lite/docs/locations
+                (
+                    "Location",
+                    [
+                        "asia-east1",
+                        "asia-east2",
+                        "asia-northeast1",
+                        "asia-northeast2",
+                        "asia-northeast3",
+                        "asia-south1",
+                        "asia-southeast1",
+                        "asia-southeast2",
+                        "australia-southeast1",
+                        "australia-southeast2",
+                        "europe-central2",
+                        "europe-north1",
+                        "europe-west1",
+                        "europe-west2",
+                        "europe-west3",
+                        "europe-west4",
+                        "europe-west6",
+                        "europe-west8",
+                        "europe-west9",
+                        "me-central1",
+                        "northamerica-northeast1",
+                        "me-west1",
+                        "northamerica-northeast2",
+                        "southamerica-east1",
+                        "us-central1",
+                        "us-east1",
+                        "us-east4",
+                        "us-east5",
+                        "us-west1",
+                        "us-west2",
+                        "us-west3",
+                        "us-west4",
+                    ],
+                    "",
+                ),
+                _interactive_message_format_input(),
+                ("Message schema", [], ""),
+            ])
             await _infer_schema_pubsub_lite(
                 vc,
                 filename,
                 credential_id,
                 info.get("project", ""),
                 info.get("subscription_id", ""),
                 info.get("location", ""),
                 info.get("message_format", ""),
                 info.get("message_schema", ""),
             )
         case "kafka":
-            info = await _multip_prompt(
-                [
-                    ("topic", [], ""),
-                    _interactive_message_format_input(),
-                    ("Message schema", [], ""),
-                ]
-            )
+            info = await _multip_prompt([
+                ("topic", [], ""),
+                _interactive_message_format_input(),
+                ("Message schema", [], ""),
+            ])
             await _infer_schema_kafka(
                 vc,
                 filename,
                 credential_id,
                 info.get("topic", ""),
                 info.get("message_format", ""),
                 info.get("message_schema", ""),
             )
         case "s3":
-            info = await _multip_prompt(
-                [
-                    ("Bucket", [], ""),
-                    ("File pattern", [], "*.csv"),
-                    ("Prefix", [], ""),
-                    ("CSV delimiter", [",", "|"], ","),
-                ]
-            )
+            info = await _multip_prompt([
+                ("Bucket", [], ""),
+                ("File pattern", [], "*.csv"),
+                ("Prefix", [], ""),
+                ("CSV delimiter", [",", "|"], ","),
+            ])
 
             print()
             null_marker = await _get_null_marker()
 
             await _infer_schema_s3(
                 vc,
                 filename,
@@ -457,91 +447,81 @@
                 info.get("bucket", ""),
                 info.get("file_pattern", ""),
                 info.get("prefix", ""),
                 info.get("csv_delimiter", ""),
                 null_marker,
             )
         case "postgresql":
-            info = await _multip_prompt(
-                [
-                    ("Schema", [], ""),
-                    ("Database", [], ""),
-                    ("Table", [], ""),
-                ]
-            )
+            info = await _multip_prompt([
+                ("Schema", [], ""),
+                ("Database", [], ""),
+                ("Table", [], ""),
+            ])
             await _infer_schema_postgresql(
                 vc,
                 filename,
                 credential_id,
                 info.get("schema", ""),
                 info.get("database", ""),
                 info.get("table", ""),
             )
         case "redshift":
-            info = await _multip_prompt(
-                [
-                    ("Schema", [], ""),
-                    ("Database", [], ""),
-                    ("Table", [], ""),
-                ]
-            )
+            info = await _multip_prompt([
+                ("Schema", [], ""),
+                ("Database", [], ""),
+                ("Table", [], ""),
+            ])
             await _infer_schema_redshift(
                 vc,
                 filename,
                 credential_id,
                 info.get("schema", ""),
                 info.get("database", ""),
                 info.get("table", ""),
             )
         case "snowflake":
-            info = await _multip_prompt(
-                [
-                    ("Schema", [], ""),
-                    ("Database", [], ""),
-                    ("Table", [], ""),
-                    ("Warehouse", [], ""),
-                    ("Role", [], ""),
-                ]
-            )
+            info = await _multip_prompt([
+                ("Schema", [], ""),
+                ("Database", [], ""),
+                ("Table", [], ""),
+                ("Warehouse", [], ""),
+                ("Role", [], ""),
+            ])
             await _infer_schema_snowflake(
                 vc,
                 filename,
                 credential_id,
                 info.get("schema", ""),
                 info.get("database", ""),
                 info.get("table", ""),
                 info.get("role", ""),
                 info.get("warehouse", ""),
             )
         case "bigquery":
-            info = await _multip_prompt(
-                [
-                    ("Project", [], ""),
-                    ("Dataset", [], ""),
-                    ("Table", [], ""),
-                ]
-            )
+            info = await _multip_prompt([
+                ("Project", [], ""),
+                ("Dataset", [], ""),
+                ("Table", [], ""),
+            ])
             await _infer_schema_bigquery(
                 vc,
                 filename,
                 credential_id,
                 info.get("project", ""),
                 info.get("dataset", ""),
                 info.get("table", ""),
             )
         case "gcs":
-            info = await _multip_prompt(
-                [
-                    ("Project", [], ""),
-                    ("Bucket", [], ""),
-                    ("Folder", [], ""),
-                    ("File pattern", ["*.csv"], "*.csv"),
-                    ("CSV delimiter", [",", "|"], ","),
-                ]
-            )
+            info = await _multip_prompt([
+                ("Project", [], ""),
+                ("Bucket", [], ""),
+                ("Folder", [], ""),
+                ("File pattern", ["*.csv"], "*.csv"),
+                ("CSV delimiter", [",", "|"], ","),
+            ])
 
             print()
             null_marker = await _get_null_marker()
 
             await _infer_schema_gcs(
                 vc,
                 filename,
@@ -959,15 +939,15 @@
     db_schema: str,
     database: str,
     table: str,
 ) -> None:
     schema = await vc.infer_postgre_sql_schema(
         PostgreSqlInferSchemaInput(
             credential_id=credential_id,
-            schema=db_schema,
+            db_schema=db_schema,
             database=database,
             table=table,
         )
     )
     _write_schema(filename, schema)
 
 
@@ -978,15 +958,15 @@
     db_schema: str,
     database: str,
     table: str,
 ) -> None:
     schema = await vc.infer_aws_redshift_schema(
         AwsRedshiftInferSchemaInput(
             credential_id=credential_id,
-            schema=db_schema,
+            db_schema=db_schema,
             database=database,
             table=table,
         )
     )
     _write_schema(filename, schema)
 
 
@@ -999,15 +979,15 @@
     table: str,
     role: str,
     warehouse: str,
 ) -> None:
     schema = await vc.infer_snowflake_schema(
         SnowflakeInferSchemaInput(
             credential_id=credential_id,
-            schema=db_schema,
+            db_schema=db_schema,
             database=database,
             table=table,
             role=role,
             warehouse=warehouse,
         )
     )
     _write_schema(filename, schema)
@@ -1171,17 +1151,17 @@
 
     return resolved_credential_id
 
 
 def _get_message_format_input(
     message_format: str | None, message_schema: str | None
 ) -> StreamingSourceMessageFormatConfigInput | None:
-    if any([message_format, message_schema]) and not all(
-        [message_format, message_schema]
-    ):
+    if any([message_format, message_schema]) and not all([
+        message_format, message_schema
+    ]):
         raise ValidioError(
             "Both message_format and message_schema must be supplied, or neither them"
         )
     if all([message_format, message_schema]):
         return StreamingSourceMessageFormatConfigInput(
             format=cast(str, message_format).upper(), db_schema=message_schema
         )
```

### Comparing `validio_cli-0.8.0/validio_cli/bin/entities/users.py` & `validio_cli-0.9.0/validio_cli/bin/entities/users.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.8.0/validio_cli/bin/entities/validators.py` & `validio_cli-0.9.0/validio_cli/bin/entities/validators.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.8.0/validio_cli/bin/entities/windows.py` & `validio_cli-0.9.0/validio_cli/bin/entities/windows.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.8.0/validio_cli/bin/main.py` & `validio_cli-0.9.0/validio_cli/bin/main.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.8.0/validio_cli/components.py` & `validio_cli-0.9.0/validio_cli/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Components for the CLI."""
+
 from typing import Any
 
 from prompt_toolkit import PromptSession
 from prompt_toolkit.application import Application
 from prompt_toolkit.key_binding import KeyPressEvent
 from prompt_toolkit.key_binding.defaults import load_key_bindings
 from prompt_toolkit.key_binding.key_bindings import KeyBindings, merge_key_bindings
```

### Comparing `validio_cli-0.8.0/validio_cli/namespace.py` & `validio_cli-0.9.0/validio_cli/namespace.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Namepsace management."""
+
 from validio_sdk.config import ValidioConfig
 
 import validio_cli
 
 
 def get_namespace(ns: str | None, cfg: ValidioConfig) -> str:
     """
```

### Comparing `validio_cli-0.8.0/validio_cli/schema.py` & `validio_cli-0.9.0/validio_cli/schema.py`

 * *Files identical despite different names*

### Comparing `validio_cli-0.8.0/PKG-INFO` & `validio_cli-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: validio-cli
-Version: 0.8.0
+Version: 0.9.0
 Summary: CLI tool to interact with the Validio platform
 Home-page: https://validio.io/
 License: Apache-2.0
 Author: Validio
 Author-email: support@validio.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

