# Comparing `tmp/refract-serving-0.0.7a0.tar.gz` & `tmp/refract-serving-1.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/refract-serving-0.0.7a0.tar", last modified: Wed Apr 24 05:41:30 2024, max compression
+gzip compressed data, was "dist/refract-serving-1.0.1a0.tar", last modified: Fri Jan 12 09:37:44 2024, max compression
```

## Comparing `refract-serving-0.0.7a0.tar` & `refract-serving-1.0.1a0.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxr-xr-x   0 10670132 (130145352) domain^users (130023937)        0 2024-04-24 05:41:30.585582 refract-serving-0.0.7a0/
--rw-r--r--   0 10670132 (130145352) domain^users (130023937)       38 2024-04-24 04:23:40.000000 refract-serving-0.0.7a0/MANIFEST.in
--rw-r--r--   0 10670132 (130145352) domain^users (130023937)      266 2024-04-24 05:41:30.585582 refract-serving-0.0.7a0/PKG-INFO
-drwxr-xr-x   0 10670132 (130145352) domain^users (130023937)        0 2024-04-24 05:41:30.581582 refract-serving-0.0.7a0/refract_serving/
--rw-r--r--   0 10670132 (130145352) domain^users (130023937)     6232 2024-04-24 04:23:40.000000 refract-serving-0.0.7a0/refract_serving/README.md
--rw-r--r--   0 10670132 (130145352) domain^users (130023937)        0 2024-04-24 04:23:40.000000 refract-serving-0.0.7a0/refract_serving/__init__.py
--rw-r--r--   0 10670132 (130145352) domain^users (130023937)    17661 2024-04-24 04:23:40.000000 refract-serving-0.0.7a0/refract_serving/app.py
-drwxr-xr-x   0 10670132 (130145352) domain^users (130023937)        0 2024-04-24 05:41:30.585582 refract-serving-0.0.7a0/refract_serving/batch_serving/
--rw-r--r--   0 10670132 (130145352) domain^users (130023937)        0 2024-04-24 03:31:22.000000 refract-serving-0.0.7a0/refract_serving/batch_serving/__init__.py
--rw-r--r--   0 10670132 (130145352) domain^users (130023937)    10346 2024-04-24 05:17:39.000000 refract-serving-0.0.7a0/refract_serving/batch_serving/app.py
--rw-r--r--   0 10670132 (130145352) domain^users (130023937)     1877 2024-04-24 03:31:22.000000 refract-serving-0.0.7a0/refract_serving/batch_serving/constants.py
--rw-r--r--   0 10670132 (130145352) domain^users (130023937)      240 2024-04-24 04:45:28.000000 refract-serving-0.0.7a0/refract_serving/batch_serving/init_script.sh
--rw-r--r--   0 10670132 (130145352) domain^users (130023937)     1650 2024-04-24 03:31:22.000000 refract-serving-0.0.7a0/refract_serving/batch_serving/utils.py
--rw-r--r--   0 10670132 (130145352) domain^users (130023937)      363 2024-04-24 04:23:40.000000 refract-serving-0.0.7a0/refract_serving/config.py
--rw-r--r--   0 10670132 (130145352) domain^users (130023937)     3786 2024-04-24 04:23:40.000000 refract-serving-0.0.7a0/refract_serving/constants.py
--rw-r--r--   0 10670132 (130145352) domain^users (130023937)     2698 2024-04-24 04:23:40.000000 refract-serving-0.0.7a0/refract_serving/decorators.py
-drwxr-xr-x   0 10670132 (130145352) domain^users (130023937)        0 2024-04-24 05:41:30.585582 refract-serving-0.0.7a0/refract_serving/explainableai/
--rw-r--r--   0 10670132 (130145352) domain^users (130023937)        0 2024-04-24 04:23:40.000000 refract-serving-0.0.7a0/refract_serving/explainableai/__init__.py
--rw-r--r--   0 10670132 (130145352) domain^users (130023937)    15283 2024-04-24 04:23:40.000000 refract-serving-0.0.7a0/refract_serving/explainableai/local_interpretation.py
--rw-r--r--   0 10670132 (130145352) domain^users (130023937)     5096 2024-04-24 04:23:40.000000 refract-serving-0.0.7a0/refract_serving/loader.py
--rw-r--r--   0 10670132 (130145352) domain^users (130023937)     1052 2024-04-24 04:23:40.000000 refract-serving-0.0.7a0/refract_serving/middlewares.py
--rw-r--r--   0 10670132 (130145352) domain^users (130023937)     1007 2024-04-24 04:23:40.000000 refract-serving-0.0.7a0/refract_serving/models.py
--rw-r--r--   0 10670132 (130145352) domain^users (130023937)     1162 2024-04-24 04:23:40.000000 refract-serving-0.0.7a0/refract_serving/schema.py
--rw-r--r--   0 10670132 (130145352) domain^users (130023937)     6120 2024-04-24 04:23:40.000000 refract-serving-0.0.7a0/refract_serving/swagger_template.json
--rw-r--r--   0 10670132 (130145352) domain^users (130023937)    18397 2024-04-24 04:23:40.000000 refract-serving-0.0.7a0/refract_serving/utils.py
-drwxr-xr-x   0 10670132 (130145352) domain^users (130023937)        0 2024-04-24 05:41:30.581582 refract-serving-0.0.7a0/refract_serving.egg-info/
--rw-r--r--   0 10670132 (130145352) domain^users (130023937)      266 2024-04-24 05:41:30.000000 refract-serving-0.0.7a0/refract_serving.egg-info/PKG-INFO
--rw-r--r--   0 10670132 (130145352) domain^users (130023937)      812 2024-04-24 05:41:30.000000 refract-serving-0.0.7a0/refract_serving.egg-info/SOURCES.txt
--rw-r--r--   0 10670132 (130145352) domain^users (130023937)        1 2024-04-24 05:41:30.000000 refract-serving-0.0.7a0/refract_serving.egg-info/dependency_links.txt
--rw-r--r--   0 10670132 (130145352) domain^users (130023937)       16 2024-04-24 05:41:30.000000 refract-serving-0.0.7a0/refract_serving.egg-info/top_level.txt
--rw-r--r--   0 10670132 (130145352) domain^users (130023937)       38 2024-04-24 05:41:30.585582 refract-serving-0.0.7a0/setup.cfg
--rw-r--r--   0 10670132 (130145352) domain^users (130023937)      481 2024-04-24 05:39:39.000000 refract-serving-0.0.7a0/setup.py
+drwxr-xr-x   0 10670132 (130145352) domain^users (130023937)        0 2024-01-12 09:37:44.710557 refract-serving-1.0.1a0/
+-rw-r--r--   0 10670132 (130145352) domain^users (130023937)       38 2024-01-12 09:34:49.000000 refract-serving-1.0.1a0/MANIFEST.in
+-rw-r--r--   0 10670132 (130145352) domain^users (130023937)      266 2024-01-12 09:37:44.710557 refract-serving-1.0.1a0/PKG-INFO
+drwxr-xr-x   0 10670132 (130145352) domain^users (130023937)        0 2024-01-12 09:37:44.702556 refract-serving-1.0.1a0/refract_serving/
+-rw-rw-r--   0 10670132 (130145352) domain^users (130023937)        0 2022-12-06 11:51:37.000000 refract-serving-1.0.1a0/refract_serving/__init__.py
+-rw-r--r--   0 10670132 (130145352) domain^users (130023937)    17661 2024-01-12 07:13:10.000000 refract-serving-1.0.1a0/refract_serving/app.py
+drwxr-xr-x   0 10670132 (130145352) domain^users (130023937)        0 2024-01-12 09:37:44.706557 refract-serving-1.0.1a0/refract_serving/batch_serving/
+-rw-r--r--   0 10670132 (130145352) domain^users (130023937)        0 2024-01-12 06:39:18.000000 refract-serving-1.0.1a0/refract_serving/batch_serving/__init__.py
+-rw-r--r--   0 10670132 (130145352) domain^users (130023937)     7714 2024-01-11 09:32:17.000000 refract-serving-1.0.1a0/refract_serving/batch_serving/app.py
+-rw-r--r--   0 10670132 (130145352) domain^users (130023937)     1877 2024-01-10 06:14:50.000000 refract-serving-1.0.1a0/refract_serving/batch_serving/constants.py
+-rw-r--r--   0 10670132 (130145352) domain^users (130023937)      122 2024-01-11 09:32:17.000000 refract-serving-1.0.1a0/refract_serving/batch_serving/init_script.sh
+-rw-r--r--   0 10670132 (130145352) domain^users (130023937)     1650 2023-09-14 09:44:08.000000 refract-serving-1.0.1a0/refract_serving/batch_serving/utils.py
+-rw-rw-r--   0 10670132 (130145352) domain^users (130023937)      363 2022-12-06 07:13:15.000000 refract-serving-1.0.1a0/refract_serving/config.py
+-rw-r--r--   0 10670132 (130145352) domain^users (130023937)     3786 2023-09-26 07:47:34.000000 refract-serving-1.0.1a0/refract_serving/constants.py
+-rw-r--r--   0 10670132 (130145352) domain^users (130023937)     2698 2023-09-26 07:47:34.000000 refract-serving-1.0.1a0/refract_serving/decorators.py
+drwxr-xr-x   0 10670132 (130145352) domain^users (130023937)        0 2024-01-12 09:37:44.706557 refract-serving-1.0.1a0/refract_serving/explainableai/
+-rw-rw-r--   0 10670132 (130145352) domain^users (130023937)        0 2022-12-06 07:13:15.000000 refract-serving-1.0.1a0/refract_serving/explainableai/__init__.py
+drwxr-xr-x   0 10670132 (130145352) domain^users (130023937)        0 2024-01-12 09:37:44.710557 refract-serving-1.0.1a0/refract_serving/explainableai/__pycache__/
+-rw-rw-r--   0 10670132 (130145352) domain^users (130023937)      172 2022-06-02 12:45:41.000000 refract-serving-1.0.1a0/refract_serving/explainableai/__pycache__/__init__.cpython-37-pytest-7.1.2.pyc
+-rw-rw-r--   0 10670132 (130145352) domain^users (130023937)      172 2022-06-01 13:59:35.000000 refract-serving-1.0.1a0/refract_serving/explainableai/__pycache__/__init__.cpython-37.pyc
+-rw-rw-r--   0 10670132 (130145352) domain^users (130023937)     8987 2022-06-07 11:06:53.000000 refract-serving-1.0.1a0/refract_serving/explainableai/__pycache__/local_interpretation.cpython-37-pytest-7.1.2.pyc
+-rw-rw-r--   0 10670132 (130145352) domain^users (130023937)     8874 2022-11-16 10:14:42.000000 refract-serving-1.0.1a0/refract_serving/explainableai/__pycache__/local_interpretation.cpython-37.pyc
+-rw-rw-r--   0 10670132 (130145352) domain^users (130023937)    15283 2022-12-06 11:51:37.000000 refract-serving-1.0.1a0/refract_serving/explainableai/local_interpretation.py
+-rw-r--r--   0 10670132 (130145352) domain^users (130023937)     5096 2024-01-12 06:44:37.000000 refract-serving-1.0.1a0/refract_serving/loader.py
+-rw-rw-r--   0 10670132 (130145352) domain^users (130023937)     1052 2022-12-06 11:51:37.000000 refract-serving-1.0.1a0/refract_serving/middlewares.py
+-rw-rw-r--   0 10670132 (130145352) domain^users (130023937)     1007 2022-12-06 11:51:37.000000 refract-serving-1.0.1a0/refract_serving/models.py
+-rw-rw-r--   0 10670132 (130145352) domain^users (130023937)     1162 2022-12-06 11:51:37.000000 refract-serving-1.0.1a0/refract_serving/schema.py
+-rw-rw-r--   0 10670132 (130145352) domain^users (130023937)     6120 2022-12-06 07:13:15.000000 refract-serving-1.0.1a0/refract_serving/swagger_template.json
+-rw-r--r--   0 10670132 (130145352) domain^users (130023937)    18397 2024-01-03 06:31:57.000000 refract-serving-1.0.1a0/refract_serving/utils.py
+drwxr-xr-x   0 10670132 (130145352) domain^users (130023937)        0 2024-01-12 09:37:44.706557 refract-serving-1.0.1a0/refract_serving.egg-info/
+-rw-r--r--   0 10670132 (130145352) domain^users (130023937)      266 2024-01-12 09:37:44.000000 refract-serving-1.0.1a0/refract_serving.egg-info/PKG-INFO
+-rw-r--r--   0 10670132 (130145352) domain^users (130023937)     1100 2024-01-12 09:37:44.000000 refract-serving-1.0.1a0/refract_serving.egg-info/SOURCES.txt
+-rw-r--r--   0 10670132 (130145352) domain^users (130023937)        1 2024-01-12 09:37:44.000000 refract-serving-1.0.1a0/refract_serving.egg-info/dependency_links.txt
+-rw-r--r--   0 10670132 (130145352) domain^users (130023937)       16 2024-01-12 09:37:44.000000 refract-serving-1.0.1a0/refract_serving.egg-info/top_level.txt
+-rw-r--r--   0 10670132 (130145352) domain^users (130023937)       38 2024-01-12 09:37:44.710557 refract-serving-1.0.1a0/setup.cfg
+-rw-r--r--   0 10670132 (130145352) domain^users (130023937)      481 2024-01-12 09:35:16.000000 refract-serving-1.0.1a0/setup.py
```

### Comparing `refract-serving-0.0.7a0/refract_serving/app.py` & `refract-serving-1.0.1a0/refract_serving/app.py`

 * *Files identical despite different names*

### Comparing `refract-serving-0.0.7a0/refract_serving/batch_serving/app.py` & `refract-serving-1.0.1a0/refract_serving/batch_serving/app.py`

 * *Files 25% similar despite different names*

```diff
@@ -102,16 +102,21 @@
 
     if source.lower() == 'local data files':
         data, result = file_prediction(model, input_file)
         write_result_file(data, result, write_strategy, input_file, output_path)
     if source.lower() == 'refract datasets':
         data, result = db_prediction(model, scoring_func)
         # write_result_db("not availble in refracio")
-        write_strategy = 'New table' if write_strategy == 'Same table' else write_strategy
-        write_result_db(data, result, write_strategy, input_file, output_path)
+        write_result_file(data, result, write_strategy, input_file, output_path)
+
+    ##################################
+    # import time
+    # print("Slee start")
+    # time.sleep(120)
+    # print("Slee end")
 
     # send notification send notification send notification send notification
 
 
 def file_prediction(model, input_file):
     import joblib
 
@@ -141,39 +146,34 @@
     print("data, predictions -", data, predictions)
 
     return data, predictions
 
 
 def write_result_file(data, predictions, write_strategy, input_file, output_path):
     print("Inside write_result:", write_strategy, output_path)
-    print("data in write_result_file - ", data)
     # Step 5: Create a new DataFrame with the predictions
 
     run_id = output_path.split("/")[-1]
     data['Prediction'] = predictions
     data['Run_id'] = run_id
 
-    try:
-        if write_strategy == 'Same table':
-            path = input_file
-            write_data = data
-        elif write_strategy == 'New table':
-            path = os.path.join(output_path, f"prediction_{datetime.now().strftime('%Y%m%d%H%M%S')}.csv")
-            write_data = data
-        elif write_strategy == 'New prediction table':
-            path = os.path.join(output_path, f"prediction_{datetime.now().strftime('%Y%m%d%H%M%S')}.csv")
-            write_data = pd.DataFrame({'Prediction': predictions, 'Run_id': run_id})
-        else:
-            path = input_file
-            write_data = pd.DataFrame([])
-        print("Final write_data - ", write_data)
-        print("Final path - ", path)
-        write_data.to_csv(path, index=False)
-    except Exception as error:
-        print("Error from write_data block", error)
+    if write_strategy == 'Same table':
+        path = input_file
+        write_data = data
+    elif write_strategy == 'New table':
+        path = os.path.join(output_path, f"prediction_{datetime.now().strftime('%Y%m%d%H%M%S')}.csv")
+        write_data = data
+    elif write_strategy == 'New prediction table':
+        path = os.path.join(output_path, f"prediction_{datetime.now().strftime('%Y%m%d%H%M%S')}.csv")
+        write_data = pd.DataFrame({'Prediction': predictions, 'Run_id': run_id})
+    else:
+        path = input_file
+        write_data = pd.DataFrame([])
+
+    write_data.to_csv(path, index=False)
 
 
 def db_prediction(model, scoring_func):
     # read db_configs
     # conect to db
     # read data
     # run predictions
@@ -183,15 +183,15 @@
     from refractio import snowflake
 
     # To get snowflake connection object with a default snowflake connection created by the user, if available.
     # snowflake.get_connection()
 
     # To read a specific dataset published from a snowflake connection
     data = snowflake.get_dataframe(os.getenv('reference_data_path').upper())
-    print(data)
+    print("Data - ", data)
 
     # Step 2: Load the pre-trained model
     model = model
 
     # Step 3: Create an empty list to store predictions
     predictions = []
 
@@ -203,56 +203,9 @@
     print("predictions", predictions)
     print("predictions type", type(predictions))
     print("data, predictions -", data, predictions)
 
     return data, predictions
 
 
-def write_result_db(data, predictions, write_strategy, input_file, output_path):
-    import requests
-    from snowflake.snowpark.session import Session
-    print("Inside write_result:", write_strategy, output_path)
-    print("data in write_result_file - ", data)
-
-    run_id = output_path.split("/")[-1]
-    data['Prediction'] = predictions
-    data['Run_id'] = run_id
-
-    url = f"http://fdc-project-manager:80/project-manager/connections/api/External/v2/external/getConnConfig/" \
-          f"{input_file}/refract_user/{os.getenv('project_id')}"
-    connection_details = requests.get(url, verify=False).json()
-
-    # connection_parameters = dict(
-    #     user=config.get("snowflake", "user"),
-    #     password=config.get("snowflake", "password"),
-    #     account=config.get("snowflake", "account"),
-    #     warehouse=config.get("snowflake", "warehouse"),
-    #     database=config.get("snowflake", "database"),
-    #     schema=config.get("snowflake", "schema"),
-    #     role=config.get("snowflake", "role"))
-
-    connection_parameters = dict(user=connection_details["params"]["READER"].get("user"),
-                                 password=connection_details["params"]["READER"].get("password"),
-                                 account=connection_details["params"]["READER"].get("accountId"),
-                                 database=connection_details["params"]["READER"].get("database"),
-                                 role=connection_details["params"]["READER"]["role"],
-                                 cloudPlatform=connection_details["params"]["READER"]["cloudPlatform"],
-                                 schema=connection_details["params"]["READER"].get("schema"),
-                                 wareHouse=connection_details["params"]["READER"]["wareHouse"],
-                                 region=connection_details["params"]["READER"]["region"] + ".gcp")
-
-    session = Session.builder.configs(connection_parameters).create()
-
-    if write_strategy == 'New table':
-        write_data = data
-    elif write_strategy == 'New prediction table':
-        write_data = pd.DataFrame({'Prediction': predictions, "Run_id": run_id})
-    else:
-        write_data = data
-
-    # data to snoflake f"{table_name}_prediction"
-    session.write_pandas(write_data, f"{run_id}_{os.getenv('model_id')}_{os.getenv('version_id')}",
-                         auto_create_table=True, overwrite=True)
-
-
 if __name__ == "__main__":
     main()
```

### Comparing `refract-serving-0.0.7a0/refract_serving/batch_serving/constants.py` & `refract-serving-1.0.1a0/refract_serving/batch_serving/constants.py`

 * *Files identical despite different names*

### Comparing `refract-serving-0.0.7a0/refract_serving/batch_serving/utils.py` & `refract-serving-1.0.1a0/refract_serving/batch_serving/utils.py`

 * *Files identical despite different names*

### Comparing `refract-serving-0.0.7a0/refract_serving/constants.py` & `refract-serving-1.0.1a0/refract_serving/constants.py`

 * *Files identical despite different names*

### Comparing `refract-serving-0.0.7a0/refract_serving/decorators.py` & `refract-serving-1.0.1a0/refract_serving/decorators.py`

 * *Files identical despite different names*

### Comparing `refract-serving-0.0.7a0/refract_serving/explainableai/local_interpretation.py` & `refract-serving-1.0.1a0/refract_serving/explainableai/local_interpretation.py`

 * *Files identical despite different names*

### Comparing `refract-serving-0.0.7a0/refract_serving/loader.py` & `refract-serving-1.0.1a0/refract_serving/loader.py`

 * *Files identical despite different names*

### Comparing `refract-serving-0.0.7a0/refract_serving/middlewares.py` & `refract-serving-1.0.1a0/refract_serving/middlewares.py`

 * *Files identical despite different names*

### Comparing `refract-serving-0.0.7a0/refract_serving/models.py` & `refract-serving-1.0.1a0/refract_serving/models.py`

 * *Files identical despite different names*

### Comparing `refract-serving-0.0.7a0/refract_serving/schema.py` & `refract-serving-1.0.1a0/refract_serving/schema.py`

 * *Files identical despite different names*

### Comparing `refract-serving-0.0.7a0/refract_serving/swagger_template.json` & `refract-serving-1.0.1a0/refract_serving/swagger_template.json`

 * *Files identical despite different names*

### Comparing `refract-serving-0.0.7a0/refract_serving/utils.py` & `refract-serving-1.0.1a0/refract_serving/utils.py`

 * *Files identical despite different names*

