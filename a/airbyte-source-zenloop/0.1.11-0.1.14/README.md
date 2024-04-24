# Comparing `tmp/airbyte_source_zenloop-0.1.11.tar.gz` & `tmp/airbyte_source_zenloop-0.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_zenloop-0.1.11.tar", max compression
+gzip compressed data, was "airbyte_source_zenloop-0.1.14.tar", max compression
```

## Comparing `airbyte_source_zenloop-0.1.11.tar` & `airbyte_source_zenloop-0.1.14.tar`

### file list

```diff
@@ -1,15 +1,10 @@
--rw-r--r--   0        0        0     4514 2024-04-11 00:00:39.049145 airbyte_source_zenloop-0.1.11/README.md
--rw-r--r--   0        0        0      768 2024-04-11 00:03:22.366728 airbyte_source_zenloop-0.1.11/pyproject.toml
--rw-r--r--   0        0        0      126 2024-04-11 00:00:39.053145 airbyte_source_zenloop-0.1.11/source_zenloop/__init__.py
--rw-r--r--   0        0        0     1176 2024-04-11 00:00:39.053145 airbyte_source_zenloop-0.1.11/source_zenloop/components.py
--rw-r--r--   0        0        0     4222 2024-04-11 00:00:39.053145 airbyte_source_zenloop-0.1.11/source_zenloop/manifest.yaml
--rw-r--r--   0        0        0      233 2024-04-11 00:00:39.053145 airbyte_source_zenloop-0.1.11/source_zenloop/run.py
--rw-r--r--   0        0        0     1636 2024-04-11 00:00:39.053145 airbyte_source_zenloop-0.1.11/source_zenloop/schemas/answers.json
--rw-r--r--   0        0        0     1303 2024-04-11 00:00:39.053145 airbyte_source_zenloop-0.1.11/source_zenloop/schemas/answers_survey_group.json
--rw-r--r--   0        0        0      272 2024-04-11 00:00:39.053145 airbyte_source_zenloop-0.1.11/source_zenloop/schemas/properties.json
--rw-r--r--   0        0        0      777 2024-04-11 00:00:39.053145 airbyte_source_zenloop-0.1.11/source_zenloop/schemas/survey_groups.json
--rw-r--r--   0        0        0      376 2024-04-11 00:00:39.053145 airbyte_source_zenloop-0.1.11/source_zenloop/schemas/surveys.json
--rw-r--r--   0        0        0      468 2024-04-11 00:00:39.053145 airbyte_source_zenloop-0.1.11/source_zenloop/source.py
--rw-r--r--   0        0        0     1278 2024-04-11 00:00:39.053145 airbyte_source_zenloop-0.1.11/source_zenloop/spec.json
--rw-r--r--   0        0        0     8926 2024-04-11 00:00:39.053145 airbyte_source_zenloop-0.1.11/source_zenloop/streams.py
--rw-r--r--   0        0        0     5220 1970-01-01 00:00:00.000000 airbyte_source_zenloop-0.1.11/PKG-INFO
+-rw-r--r--   0        0        0     4514 2024-04-24 21:17:52.893670 airbyte_source_zenloop-0.1.14/README.md
+-rw-r--r--   0        0        0      772 2024-04-24 21:20:55.665573 airbyte_source_zenloop-0.1.14/pyproject.toml
+-rw-r--r--   0        0        0      126 2024-04-24 21:17:52.893670 airbyte_source_zenloop-0.1.14/source_zenloop/__init__.py
+-rw-r--r--   0        0        0     1176 2024-04-24 21:17:52.893670 airbyte_source_zenloop-0.1.14/source_zenloop/components.py
+-rw-r--r--   0        0        0    14462 2024-04-24 21:17:52.893670 airbyte_source_zenloop-0.1.14/source_zenloop/manifest.yaml
+-rw-r--r--   0        0        0      233 2024-04-24 21:17:52.893670 airbyte_source_zenloop-0.1.14/source_zenloop/run.py
+-rw-r--r--   0        0        0      468 2024-04-24 21:17:52.893670 airbyte_source_zenloop-0.1.14/source_zenloop/source.py
+-rw-r--r--   0        0        0     1278 2024-04-24 21:17:52.893670 airbyte_source_zenloop-0.1.14/source_zenloop/spec.json
+-rw-r--r--   0        0        0     8926 2024-04-24 21:17:52.893670 airbyte_source_zenloop-0.1.14/source_zenloop/streams.py
+-rw-r--r--   0        0        0     5222 1970-01-01 00:00:00.000000 airbyte_source_zenloop-0.1.14/PKG-INFO
```

### Comparing `airbyte_source_zenloop-0.1.11/README.md` & `airbyte_source_zenloop-0.1.14/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_zenloop-0.1.11/pyproject.toml` & `airbyte_source_zenloop-0.1.14/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.1.11"
+version = "0.1.14"
 name = "airbyte-source-zenloop"
 description = "Source implementation for Zenloop."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,17 +18,17 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_zenloop" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "^0"
+airbyte-cdk = "0.80.0"
 
 [tool.poetry.scripts]
 source-zenloop = "source_zenloop.run:run"
 
 [tool.poetry.group.dev.dependencies]
+pytest-mock = "^3.6.1"
 requests-mock = "^1.9.3"
-responses = "^0.13.3"
 pytest = "^6.1"
-pytest-mock = "^3.6.1"
+responses = "^0.13.3"
```

### Comparing `airbyte_source_zenloop-0.1.11/source_zenloop/components.py` & `airbyte_source_zenloop-0.1.14/source_zenloop/components.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_zenloop-0.1.11/source_zenloop/spec.json` & `airbyte_source_zenloop-0.1.14/source_zenloop/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_zenloop-0.1.11/source_zenloop/streams.py` & `airbyte_source_zenloop-0.1.14/source_zenloop/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_zenloop-0.1.11/PKG-INFO` & `airbyte_source_zenloop-0.1.14/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-zenloop
-Version: 0.1.11
+Version: 0.1.14
 Summary: Source implementation for Zenloop.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (>=0,<1)
+Requires-Dist: airbyte-cdk (==0.80.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/zenloop
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Zenloop source connector
```

