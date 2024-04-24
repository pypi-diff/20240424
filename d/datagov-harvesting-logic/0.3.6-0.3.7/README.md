# Comparing `tmp/datagov_harvesting_logic-0.3.6.tar.gz` & `tmp/datagov_harvesting_logic-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datagov_harvesting_logic-0.3.6.tar", max compression
+gzip compressed data, was "datagov_harvesting_logic-0.3.7.tar", max compression
```

## Comparing `datagov_harvesting_logic-0.3.6.tar` & `datagov_harvesting_logic-0.3.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1878 2024-04-03 22:04:24.163847 datagov_harvesting_logic-0.3.6/LICENSE.md
--rw-r--r--   0        0        0     5031 2024-04-03 22:04:24.163847 datagov_harvesting_logic-0.3.6/README.md
--rw-r--r--   0        0        0      162 2024-04-03 22:04:24.167847 datagov_harvesting_logic-0.3.6/harvester/__init__.py
--rw-r--r--   0        0        0     4489 2024-04-03 22:04:24.167847 datagov_harvesting_logic-0.3.6/harvester/ckan_utils.py
--rw-r--r--   0        0        0     4464 2024-04-03 22:04:24.167847 datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/arm.data.json
--rw-r--r--   0        0        0     7830 2024-04-03 22:04:24.167847 datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/collection-1-parent-2-children.data.json
--rw-r--r--   0        0        0    14027 2024-04-03 22:04:24.167847 datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/collection-2-parent-4-children.data.json
--rw-r--r--   0        0        0     7454 2024-04-03 22:04:24.167847 datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/geospatial.data.json
--rw-r--r--   0        0        0   310979 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/large-spatial.data.json
--rw-r--r--   0        0        0      918 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/missing-catalog.data.json
--rw-r--r--   0        0        0     1059 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/missing-dataset-fields.data.json
--rw-r--r--   0        0        0     3259 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/missing-identifier-title.data.json
--rw-r--r--   0        0        0     1292 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/numerical-title.data.json
--rw-r--r--   0        0        0     2520 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/ny.data.json
--rw-r--r--   0        0        0     1314 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/reserved-title.data.json
--rw-r--r--   0        0        0     9562 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/usda.gov.data.json
--rw-r--r--   0        0        0     1604 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/harvester/data/dcatus/schemas/catalog.json
--rw-r--r--   0        0        0    23811 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/harvester/data/dcatus/schemas/dataset.json
--rw-r--r--   0        0        0     2200 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/harvester/exceptions.py
--rw-r--r--   0        0        0    25444 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/harvester/harvest.py
--rw-r--r--   0        0        0      589 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/harvester/logger_config.py
--rw-r--r--   0        0        0     3632 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/harvester/utils.py
--rw-r--r--   0        0        0     2212 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     6296 1970-01-01 00:00:00.000000 datagov_harvesting_logic-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1878 2024-04-24 14:59:01.131058 datagov_harvesting_logic-0.3.7/LICENSE.md
+-rw-r--r--   0        0        0     5265 2024-04-24 14:59:01.131058 datagov_harvesting_logic-0.3.7/README.md
+-rw-r--r--   0        0        0      162 2024-04-24 14:59:01.135058 datagov_harvesting_logic-0.3.7/harvester/__init__.py
+-rw-r--r--   0        0        0     4489 2024-04-24 14:59:01.135058 datagov_harvesting_logic-0.3.7/harvester/ckan_utils.py
+-rw-r--r--   0        0        0     4464 2024-04-24 14:59:01.135058 datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/arm.data.json
+-rw-r--r--   0        0        0     7830 2024-04-24 14:59:01.135058 datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/collection-1-parent-2-children.data.json
+-rw-r--r--   0        0        0    14027 2024-04-24 14:59:01.135058 datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/collection-2-parent-4-children.data.json
+-rw-r--r--   0        0        0     7454 2024-04-24 14:59:01.135058 datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/geospatial.data.json
+-rw-r--r--   0        0        0   310979 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/large-spatial.data.json
+-rw-r--r--   0        0        0      918 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/missing-catalog.data.json
+-rw-r--r--   0        0        0     1059 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/missing-dataset-fields.data.json
+-rw-r--r--   0        0        0     3259 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/missing-identifier-title.data.json
+-rw-r--r--   0        0        0     1292 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/numerical-title.data.json
+-rw-r--r--   0        0        0     2520 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/ny.data.json
+-rw-r--r--   0        0        0     1314 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/reserved-title.data.json
+-rw-r--r--   0        0        0     9562 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/usda.gov.data.json
+-rw-r--r--   0        0        0     1604 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/harvester/data/dcatus/schemas/catalog.json
+-rw-r--r--   0        0        0    23811 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/harvester/data/dcatus/schemas/dataset.json
+-rw-r--r--   0        0        0     2158 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/harvester/exceptions.py
+-rw-r--r--   0        0        0    25444 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/harvester/harvest.py
+-rw-r--r--   0        0        0      589 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/harvester/logger_config.py
+-rw-r--r--   0        0        0     3632 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/harvester/utils.py
+-rw-r--r--   0        0        0     2241 2024-04-24 14:59:01.139058 datagov_harvesting_logic-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     6582 1970-01-01 00:00:00.000000 datagov_harvesting_logic-0.3.7/PKG-INFO
```

### Comparing `datagov_harvesting_logic-0.3.6/LICENSE.md` & `datagov_harvesting_logic-0.3.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.6/README.md` & `datagov_harvesting_logic-0.3.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,19 @@
 
 ### Harvester testing
 
 - These tests are found in `extract`, and `validate`. Some of them rely on services in the `docker-compose.yml`. Run using docker `docker compose up -d` and with the command `poetry run pytest --ignore=./tests/load/ckan`.
 
 If you followed the instructions for `CKAN load testing` and `Harvester testing` you can simply run `poetry run pytest` to run all tests.
 
+### Integration testing
+- to run integration tests locally add the following env variables to your .env file in addition to their appropriate values
+  - CF_SERVICE_USER = "put username here"
+  - CF_SERVICE_AUTH = "put password here"
+
 ## Comparison
 
 - `./tests/harvest_sources/ckan_datasets_resp.json`
   - Represents what ckan would respond with after querying for the harvest source name
 - `./tests/harvest_sources/dcatus_compare.json`
   - Represents a changed harvest source
   - Created:
@@ -106,17 +111,17 @@
    ```
 
    This will start the necessary services and execute the test.
 
 3. when there are database DDL changes, use following steps to generate migration scripts and update database:
 
     ```bash
-    docker-compose db up
-    docker-compose run app flask db migrate -m "migration description"
-    docker-compose run app flask db upgrade
+    docker compose db up
+    docker compose run app flask db migrate -m "migration description"
+    docker compose run app flask db upgrade
     ```
 
 ### Deployment to cloud.gov
 
 #### Database Service Setup
 
 A database service is required for use on cloud.gov.
```

### Comparing `datagov_harvesting_logic-0.3.6/harvester/ckan_utils.py` & `datagov_harvesting_logic-0.3.7/harvester/ckan_utils.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/arm.data.json` & `datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/arm.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/collection-1-parent-2-children.data.json` & `datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/collection-1-parent-2-children.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/collection-2-parent-4-children.data.json` & `datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/collection-2-parent-4-children.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/geospatial.data.json` & `datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/geospatial.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/large-spatial.data.json` & `datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/large-spatial.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/missing-catalog.data.json` & `datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/missing-catalog.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/missing-dataset-fields.data.json` & `datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/missing-dataset-fields.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/missing-identifier-title.data.json` & `datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/missing-identifier-title.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/numerical-title.data.json` & `datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/numerical-title.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/ny.data.json` & `datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/ny.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/reserved-title.data.json` & `datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/reserved-title.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/usda.gov.data.json` & `datagov_harvesting_logic-0.3.7/harvester/data/dcatus/jsons/usda.gov.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.6/harvester/data/dcatus/schemas/catalog.json` & `datagov_harvesting_logic-0.3.7/harvester/data/dcatus/schemas/catalog.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.6/harvester/data/dcatus/schemas/dataset.json` & `datagov_harvesting_logic-0.3.7/harvester/data/dcatus/schemas/dataset.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.6/harvester/exceptions.py` & `datagov_harvesting_logic-0.3.7/harvester/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             "harvest_job_id": self.harvest_job_id,
             "message": self.msg,
             "severity": self.severity,
             "type": self.type,
             "date_created": datetime.utcnow(),
         }
 
-        self.db_interface.add_harvest_error(error_data, self.harvest_job_id)
+        self.db_interface.add_harvest_error(error_data)
         self.logger.critical(self.msg, exc_info=True)
 
 
 class ExtractHarvestSourceException(HarvestCriticalException):
     pass
 
 
@@ -59,15 +59,15 @@
             "message": self.msg,
             "severity": self.severity,
             "type": self.type,
             "date_created": datetime.utcnow(),
             "harvest_record_id": self.title # to-do 
         }
 
-        self.db_interface.add_harvest_error(error_data, self.harvest_job_id)
+        self.db_interface.add_harvest_error(error_data)
         self.logger.error(self.msg, exc_info=True)
 
 
 class ValidationException(HarvestNonCriticalException):
     pass
```

### Comparing `datagov_harvesting_logic-0.3.6/harvester/harvest.py` & `datagov_harvesting_logic-0.3.7/harvester/harvest.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.6/harvester/logger_config.py` & `datagov_harvesting_logic-0.3.7/harvester/logger_config.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.6/harvester/utils.py` & `datagov_harvesting_logic-0.3.7/harvester/utils.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.6/pyproject.toml` & `datagov_harvesting_logic-0.3.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datagov-harvesting-logic"
-version = "0.3.6"
+version = "0.3.7"
 description = ""
 # authors = [
 #     {name = "Jin Sun", email = "jin.sun@gsa.gov"},
 #     {name = "Tyler Burton", email = "tyler.burton@gsa.gov"},
 # ]
 authors = [
     "Datagov Team <datagov@gsa.gov>",
@@ -29,14 +29,15 @@
 boto3 = "^1.34.29"
 sqlalchemy = "^2.0.25"
 flask = "^3.0.2"
 psycopg2-binary = "^2.9.9"
 flask-sqlalchemy = "^3.1.1"
 flask-wtf = "^1.2.1"
 flask-migrate = "^4.0.7"
+flask-bootstrap = "^3.3.7.1"
 cloudfoundry-client = "^1.36.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.0"
 ruff = "^0.0.261"
 pytest-cov = "^4.0.0"
```

### Comparing `datagov_harvesting_logic-0.3.6/PKG-INFO` & `datagov_harvesting_logic-0.3.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datagov-harvesting-logic
-Version: 0.3.6
+Version: 0.3.7
 Summary: 
 Home-page: https://github.com/GSA/datagov-harvesting-logic
 License: LICENSE.md
 Author: Datagov Team
 Author-email: datagov@gsa.gov
 Maintainer: Datagov Team
 Maintainer-email: datagov@gsa.gov
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: boto3 (>=1.34.29,<2.0.0)
 Requires-Dist: ckanapi (>=4.7)
 Requires-Dist: cloudfoundry-client (>=1.36.0,<2.0.0)
 Requires-Dist: deepdiff (>=6)
 Requires-Dist: flask (>=3.0.2,<4.0.0)
+Requires-Dist: flask-bootstrap (>=3.3.7.1,<4.0.0.0)
 Requires-Dist: flask-migrate (>=4.0.7,<5.0.0)
 Requires-Dist: flask-sqlalchemy (>=3.1.1,<4.0.0)
 Requires-Dist: flask-wtf (>=1.2.1,<2.0.0)
 Requires-Dist: jsonschema (>=4)
 Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0)
 Requires-Dist: pytest (>=7.3.2)
 Requires-Dist: python-dotenv (>=1)
@@ -69,14 +70,19 @@
 
 ### Harvester testing
 
 - These tests are found in `extract`, and `validate`. Some of them rely on services in the `docker-compose.yml`. Run using docker `docker compose up -d` and with the command `poetry run pytest --ignore=./tests/load/ckan`.
 
 If you followed the instructions for `CKAN load testing` and `Harvester testing` you can simply run `poetry run pytest` to run all tests.
 
+### Integration testing
+- to run integration tests locally add the following env variables to your .env file in addition to their appropriate values
+  - CF_SERVICE_USER = "put username here"
+  - CF_SERVICE_AUTH = "put password here"
+
 ## Comparison
 
 - `./tests/harvest_sources/ckan_datasets_resp.json`
   - Represents what ckan would respond with after querying for the harvest source name
 - `./tests/harvest_sources/dcatus_compare.json`
   - Represents a changed harvest source
   - Created:
@@ -140,17 +146,17 @@
    ```
 
    This will start the necessary services and execute the test.
 
 3. when there are database DDL changes, use following steps to generate migration scripts and update database:
 
     ```bash
-    docker-compose db up
-    docker-compose run app flask db migrate -m "migration description"
-    docker-compose run app flask db upgrade
+    docker compose db up
+    docker compose run app flask db migrate -m "migration description"
+    docker compose run app flask db upgrade
     ```
 
 ### Deployment to cloud.gov
 
 #### Database Service Setup
 
 A database service is required for use on cloud.gov.
```

