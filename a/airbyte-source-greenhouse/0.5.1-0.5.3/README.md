# Comparing `tmp/airbyte_source_greenhouse-0.5.1.tar.gz` & `tmp/airbyte_source_greenhouse-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_greenhouse-0.5.1.tar", max compression
+gzip compressed data, was "airbyte_source_greenhouse-0.5.3.tar", max compression
```

## Comparing `airbyte_source_greenhouse-0.5.1.tar` & `airbyte_source_greenhouse-0.5.3.tar`

### file list

```diff
@@ -1,45 +1,9 @@
--rw-r--r--   0        0        0     4568 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/README.md
--rw-r--r--   0        0        0      797 2024-03-14 15:23:24.579668 airbyte_source_greenhouse-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      130 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/__init__.py
--rw-r--r--   0        0        0     6505 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/components.py
--rw-r--r--   0        0        0    13946 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/manifest.yaml
--rw-r--r--   0        0        0      242 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/run.py
--rw-r--r--   0        0        0     3573 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/activity_feed.json
--rw-r--r--   0        0        0     2836 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/applications.json
--rw-r--r--   0        0        0      614 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/applications_demographics_answers.json
--rw-r--r--   0        0        0     2287 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/applications_interviews.json
--rw-r--r--   0        0        0     1997 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/approvals.json
--rw-r--r--   0        0        0     5296 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/candidates.json
--rw-r--r--   0        0        0      188 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/close_reasons.json
--rw-r--r--   0        0        0     1550 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/custom_fields.json
--rw-r--r--   0        0        0      298 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/degrees.json
--rw-r--r--   0        0        0      693 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/demographics_answer_options.json
--rw-r--r--   0        0        0      614 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/demographics_answers.json
--rw-r--r--   0        0        0      693 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/demographics_answers_answer_options.json
--rw-r--r--   0        0        0      317 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/demographics_question_sets.json
--rw-r--r--   0        0        0      696 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/demographics_question_sets_questions.json
--rw-r--r--   0        0        0      696 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/demographics_questions.json
--rw-r--r--   0        0        0      504 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/departments.json
--rw-r--r--   0        0        0      299 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/disciplines.json
--rw-r--r--   0        0        0     1242 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/eeoc.json
--rw-r--r--   0        0        0      866 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/email_templates.json
--rw-r--r--   0        0        0     2287 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/interviews.json
--rw-r--r--   0        0        0     1898 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/job_posts.json
--rw-r--r--   0        0        0     1418 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/job_stages.json
--rw-r--r--   0        0        0     3852 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/jobs.json
--rw-r--r--   0        0        0     1760 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/jobs_openings.json
--rw-r--r--   0        0        0     1418 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/jobs_stages.json
--rw-r--r--   0        0        0     1764 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/offers.json
--rw-r--r--   0        0        0      929 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/offices.json
--rw-r--r--   0        0        0      567 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/prospect_pools.json
--rw-r--r--   0        0        0      413 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/rejection_reasons.json
--rw-r--r--   0        0        0      299 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/schools.json
--rw-r--r--   0        0        0     2635 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/scorecards.json
--rw-r--r--   0        0        0      413 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/sources.json
--rw-r--r--   0        0        0      240 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/tags.json
--rw-r--r--   0        0        0      274 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/user_permissions.json
--rw-r--r--   0        0        0      262 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/user_roles.json
--rw-r--r--   0        0        0     2474 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/schemas/users.json
--rw-r--r--   0        0        0      478 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/source.py
--rw-r--r--   0        0        0      636 2024-03-14 14:37:10.000000 airbyte_source_greenhouse-0.5.1/source_greenhouse/spec.json
--rw-r--r--   0        0        0     5331 1970-01-01 00:00:00.000000 airbyte_source_greenhouse-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     4568 2024-04-23 22:51:09.297891 airbyte_source_greenhouse-0.5.3/README.md
+-rw-r--r--   0        0        0      801 2024-04-23 22:53:50.953833 airbyte_source_greenhouse-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      130 2024-04-23 22:51:09.297891 airbyte_source_greenhouse-0.5.3/source_greenhouse/__init__.py
+-rw-r--r--   0        0        0     6505 2024-04-23 22:51:09.297891 airbyte_source_greenhouse-0.5.3/source_greenhouse/components.py
+-rw-r--r--   0        0        0   119276 2024-04-23 22:51:09.301891 airbyte_source_greenhouse-0.5.3/source_greenhouse/manifest.yaml
+-rw-r--r--   0        0        0      242 2024-04-23 22:51:09.301891 airbyte_source_greenhouse-0.5.3/source_greenhouse/run.py
+-rw-r--r--   0        0        0      478 2024-04-23 22:51:09.301891 airbyte_source_greenhouse-0.5.3/source_greenhouse/source.py
+-rw-r--r--   0        0        0      636 2024-04-23 22:51:09.301891 airbyte_source_greenhouse-0.5.3/source_greenhouse/spec.json
+-rw-r--r--   0        0        0     5333 1970-01-01 00:00:00.000000 airbyte_source_greenhouse-0.5.3/PKG-INFO
```

### Comparing `airbyte_source_greenhouse-0.5.1/README.md` & `airbyte_source_greenhouse-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_greenhouse-0.5.1/pyproject.toml` & `airbyte_source_greenhouse-0.5.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.5.1"
+version = "0.5.3"
 name = "airbyte-source-greenhouse"
 description = "Source implementation for Greenhouse."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_greenhouse" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "^0"
+airbyte-cdk = "0.80.0"
 dataclasses-jsonschema = "==2.15.1"
 
 [tool.poetry.scripts]
 source-greenhouse = "source_greenhouse.run:run"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.1"
```

### Comparing `airbyte_source_greenhouse-0.5.1/source_greenhouse/components.py` & `airbyte_source_greenhouse-0.5.3/source_greenhouse/components.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_greenhouse-0.5.1/source_greenhouse/spec.json` & `airbyte_source_greenhouse-0.5.3/source_greenhouse/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_greenhouse-0.5.1/PKG-INFO` & `airbyte_source_greenhouse-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-greenhouse
-Version: 0.5.1
+Version: 0.5.3
 Summary: Source implementation for Greenhouse.
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
 Requires-Dist: dataclasses-jsonschema (==2.15.1)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/greenhouse
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Greenhouse source connector
```

