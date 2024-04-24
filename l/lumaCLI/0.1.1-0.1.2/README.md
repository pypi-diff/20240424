# Comparing `tmp/lumacli-0.1.1.tar.gz` & `tmp/lumacli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumacli-0.1.1.tar", max compression
+gzip compressed data, was "lumacli-0.1.2.tar", max compression
```

## Comparing `lumacli-0.1.1.tar` & `lumacli-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1064 2024-04-19 09:55:55.389014 lumacli-0.1.1/LICENSE
--rw-r--r--   0        0        0      399 2024-04-19 09:55:55.389014 lumacli-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-19 09:55:55.389014 lumacli-0.1.1/lumaCLI/__init__.py
--rw-r--r--   0        0        0     2618 2024-04-19 09:55:55.389014 lumacli-0.1.1/lumaCLI/commands/config.py
--rw-r--r--   0        0        0     6352 2024-04-19 09:55:55.389014 lumacli-0.1.1/lumaCLI/commands/dbt.py
--rw-r--r--   0        0        0     2177 2024-04-19 09:55:55.389014 lumacli-0.1.1/lumaCLI/commands/postgres.py
--rw-r--r--   0        0        0     2505 2024-04-19 09:55:55.389014 lumacli-0.1.1/lumaCLI/main.py
--rw-r--r--   0        0        0       98 2024-04-19 09:55:55.389014 lumacli-0.1.1/lumaCLI/models/__init__.py
--rw-r--r--   0        0        0     8892 2024-04-19 09:55:55.389014 lumacli-0.1.1/lumaCLI/models/config_info.py
--rw-r--r--   0        0        0     7922 2024-04-19 09:55:55.389014 lumacli-0.1.1/lumaCLI/models/dbt.py
--rw-r--r--   0        0        0     2047 2024-04-19 09:55:55.389014 lumacli-0.1.1/lumaCLI/models/request_info.py
--rw-r--r--   0        0        0        0 2024-04-19 09:55:55.389014 lumacli-0.1.1/lumaCLI/tests/__init__.py
--rw-r--r--   0        0        0     8087 2024-04-19 09:55:55.389014 lumacli-0.1.1/lumaCLI/tests/assets/dbt_v1.3/catalog.json
--rw-r--r--   0        0        0      260 2024-04-19 09:55:55.389014 lumacli-0.1.1/lumaCLI/tests/assets/dbt_v1.3/invalid_json.json
--rw-r--r--   0        0        0   173474 2024-04-19 09:55:55.389014 lumacli-0.1.1/lumaCLI/tests/assets/dbt_v1.3/manifest.json
--rw-r--r--   0        0        0    10271 2024-04-19 09:55:55.389014 lumacli-0.1.1/lumaCLI/tests/assets/dbt_v1.3/run_results.json
--rw-r--r--   0        0        0     9716 2024-04-19 09:55:55.389014 lumacli-0.1.1/lumaCLI/tests/assets/dbt_v1.3/sources.json
--rw-r--r--   0        0        0        0 2024-04-19 09:55:55.389014 lumacli-0.1.1/lumaCLI/tests/assets/dbt_v1.3/test_non_json_file.txt
--rw-r--r--   0        0        0     6277 2024-04-19 09:55:55.389014 lumacli-0.1.1/lumaCLI/tests/assets/dbt_v1.7/model_metadata/catalog.json
--rw-r--r--   0        0        0  1063666 2024-04-19 09:55:55.393014 lumacli-0.1.1/lumaCLI/tests/assets/dbt_v1.7/model_metadata/manifest.json
--rw-r--r--   0        0        0     2002 2024-04-19 09:55:55.393014 lumacli-0.1.1/lumaCLI/tests/assets/dbt_v1.7/model_run_metadata/run_results.json
--rw-r--r--   0        0        0     6811 2024-04-19 09:55:55.393014 lumacli-0.1.1/lumaCLI/tests/conftest.py
--rw-r--r--   0        0        0      441 2024-04-19 09:55:55.393014 lumacli-0.1.1/lumaCLI/tests/integration/test_dbt.py
--rw-r--r--   0        0        0      319 2024-04-19 09:55:55.393014 lumacli-0.1.1/lumaCLI/tests/integration/test_luma.py
--rw-r--r--   0        0        0     5109 2024-04-19 09:55:55.393014 lumacli-0.1.1/lumaCLI/tests/postgres_dump_file.sql
--rw-r--r--   0        0        0       90 2024-04-19 09:55:55.393014 lumacli-0.1.1/lumaCLI/tests/requirements.txt
--rw-r--r--   0        0        0     2524 2024-04-19 09:55:55.393014 lumacli-0.1.1/lumaCLI/tests/unit/test_config.py
--rw-r--r--   0        0        0     3752 2024-04-19 09:55:55.393014 lumacli-0.1.1/lumaCLI/tests/unit/test_dbt.py
--rw-r--r--   0        0        0     1208 2024-04-19 09:55:55.393014 lumacli-0.1.1/lumaCLI/tests/unit/test_postgres.py
--rw-r--r--   0        0        0     4258 2024-04-19 09:55:55.393014 lumacli-0.1.1/lumaCLI/tests/unit/test_postgres_utils.py
--rw-r--r--   0        0        0      478 2024-04-19 09:55:55.393014 lumacli-0.1.1/lumaCLI/utils/__init__.py
--rw-r--r--   0        0        0    15023 2024-04-19 09:55:55.397014 lumacli-0.1.1/lumaCLI/utils/luma_utils.py
--rw-r--r--   0        0        0     4177 2024-04-19 09:55:55.397014 lumacli-0.1.1/lumaCLI/utils/options.py
--rw-r--r--   0        0        0    10546 2024-04-19 09:55:55.397014 lumacli-0.1.1/lumaCLI/utils/postgres_utils.py
--rw-r--r--   0        0        0     1612 2024-04-19 09:55:55.397014 lumacli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1394 1970-01-01 00:00:00.000000 lumacli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-24 13:54:30.920741 lumacli-0.1.2/LICENSE
+-rw-r--r--   0        0        0      399 2024-04-24 13:54:30.920741 lumacli-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-24 13:54:30.920741 lumacli-0.1.2/lumaCLI/__init__.py
+-rw-r--r--   0        0        0     2618 2024-04-24 13:54:30.920741 lumacli-0.1.2/lumaCLI/commands/config.py
+-rw-r--r--   0        0        0     6352 2024-04-24 13:54:30.920741 lumacli-0.1.2/lumaCLI/commands/dbt.py
+-rw-r--r--   0        0        0     2177 2024-04-24 13:54:30.920741 lumacli-0.1.2/lumaCLI/commands/postgres.py
+-rw-r--r--   0        0        0     2505 2024-04-24 13:54:30.920741 lumacli-0.1.2/lumaCLI/main.py
+-rw-r--r--   0        0        0       98 2024-04-24 13:54:30.920741 lumacli-0.1.2/lumaCLI/models/__init__.py
+-rw-r--r--   0        0        0     9011 2024-04-24 13:54:30.920741 lumacli-0.1.2/lumaCLI/models/config_info.py
+-rw-r--r--   0        0        0     7922 2024-04-24 13:54:30.924741 lumacli-0.1.2/lumaCLI/models/dbt.py
+-rw-r--r--   0        0        0     2047 2024-04-24 13:54:30.924741 lumacli-0.1.2/lumaCLI/models/request_info.py
+-rw-r--r--   0        0        0        0 2024-04-24 13:54:30.924741 lumacli-0.1.2/lumaCLI/tests/__init__.py
+-rw-r--r--   0        0        0     8087 2024-04-24 13:54:30.924741 lumacli-0.1.2/lumaCLI/tests/assets/dbt_v1.3/catalog.json
+-rw-r--r--   0        0        0      260 2024-04-24 13:54:30.924741 lumacli-0.1.2/lumaCLI/tests/assets/dbt_v1.3/invalid_json.json
+-rw-r--r--   0        0        0   173474 2024-04-24 13:54:30.924741 lumacli-0.1.2/lumaCLI/tests/assets/dbt_v1.3/manifest.json
+-rw-r--r--   0        0        0    10271 2024-04-24 13:54:30.924741 lumacli-0.1.2/lumaCLI/tests/assets/dbt_v1.3/run_results.json
+-rw-r--r--   0        0        0     9716 2024-04-24 13:54:30.924741 lumacli-0.1.2/lumaCLI/tests/assets/dbt_v1.3/sources.json
+-rw-r--r--   0        0        0        0 2024-04-24 13:54:30.924741 lumacli-0.1.2/lumaCLI/tests/assets/dbt_v1.3/test_non_json_file.txt
+-rw-r--r--   0        0        0     6277 2024-04-24 13:54:30.924741 lumacli-0.1.2/lumaCLI/tests/assets/dbt_v1.7/model_metadata/catalog.json
+-rw-r--r--   0        0        0  1063666 2024-04-24 13:54:30.928741 lumacli-0.1.2/lumaCLI/tests/assets/dbt_v1.7/model_metadata/manifest.json
+-rw-r--r--   0        0        0     2002 2024-04-24 13:54:30.928741 lumacli-0.1.2/lumaCLI/tests/assets/dbt_v1.7/model_run_metadata/run_results.json
+-rw-r--r--   0        0        0     6829 2024-04-24 13:54:30.928741 lumacli-0.1.2/lumaCLI/tests/conftest.py
+-rw-r--r--   0        0        0      441 2024-04-24 13:54:30.928741 lumacli-0.1.2/lumaCLI/tests/integration/test_dbt.py
+-rw-r--r--   0        0        0      319 2024-04-24 13:54:30.928741 lumacli-0.1.2/lumaCLI/tests/integration/test_luma.py
+-rw-r--r--   0        0        0     5109 2024-04-24 13:54:30.928741 lumacli-0.1.2/lumaCLI/tests/postgres_dump_file.sql
+-rw-r--r--   0        0        0       90 2024-04-24 13:54:30.928741 lumacli-0.1.2/lumaCLI/tests/requirements.txt
+-rw-r--r--   0        0        0     2524 2024-04-24 13:54:30.928741 lumacli-0.1.2/lumaCLI/tests/unit/test_config.py
+-rw-r--r--   0        0        0     3752 2024-04-24 13:54:30.928741 lumacli-0.1.2/lumaCLI/tests/unit/test_dbt.py
+-rw-r--r--   0        0        0     1208 2024-04-24 13:54:30.928741 lumacli-0.1.2/lumaCLI/tests/unit/test_postgres.py
+-rw-r--r--   0        0        0     4258 2024-04-24 13:54:30.928741 lumacli-0.1.2/lumaCLI/tests/unit/test_postgres_utils.py
+-rw-r--r--   0        0        0      478 2024-04-24 13:54:30.928741 lumacli-0.1.2/lumaCLI/utils/__init__.py
+-rw-r--r--   0        0        0    15043 2024-04-24 13:54:30.928741 lumacli-0.1.2/lumaCLI/utils/luma_utils.py
+-rw-r--r--   0        0        0     4177 2024-04-24 13:54:30.928741 lumacli-0.1.2/lumaCLI/utils/options.py
+-rw-r--r--   0        0        0    10546 2024-04-24 13:54:30.928741 lumacli-0.1.2/lumaCLI/utils/postgres_utils.py
+-rw-r--r--   0        0        0     1612 2024-04-24 13:54:30.928741 lumacli-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1394 1970-01-01 00:00:00.000000 lumacli-0.1.2/PKG-INFO
```

### Comparing `lumacli-0.1.1/LICENSE` & `lumacli-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lumacli-0.1.1/lumaCLI/commands/config.py` & `lumacli-0.1.2/lumaCLI/commands/config.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.1.1/lumaCLI/commands/dbt.py` & `lumacli-0.1.2/lumaCLI/commands/dbt.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.1.1/lumaCLI/commands/postgres.py` & `lumacli-0.1.2/lumaCLI/commands/postgres.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.1.1/lumaCLI/main.py` & `lumacli-0.1.2/lumaCLI/main.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.1.1/lumaCLI/models/config_info.py` & `lumacli-0.1.2/lumaCLI/models/config_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -307,25 +307,27 @@
         slug (str): A slug for the group, used in URLs or as an identifier.
         label_plural (str): The plural label for the group.
         label_singular (str): The singular label for the group.
         icon (Optional[str]): An optional icon for the group. Must be one of the allowed
             icons.
         in_sidebar (bool, optional): Whether the group should be displayed in the
             sidebar.
+        visible (bool, optional): Whether the group should be displayed in Luma UI.
 
     Methods:
         icon_validator: Validates that the provided icon (if any) is in the allowed set.
     """
 
     meta_key: str
     slug: str
     label_plural: str
     label_singular: str
     icon: Optional[str]
     in_sidebar: Optional[bool] = True
+    visible: Optional[bool] = True
 
     @validator("icon")
     def icon_validator(cls, v):
         """Validates the icon attribute.
 
         Ensures that if an icon is provided, it is one of the pre-approved icons.
```

### Comparing `lumacli-0.1.1/lumaCLI/models/dbt.py` & `lumacli-0.1.2/lumaCLI/models/dbt.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.1.1/lumaCLI/models/request_info.py` & `lumacli-0.1.2/lumaCLI/models/request_info.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.1.1/lumaCLI/tests/assets/dbt_v1.3/catalog.json` & `lumacli-0.1.2/lumaCLI/tests/assets/dbt_v1.3/catalog.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.1.1/lumaCLI/tests/assets/dbt_v1.3/manifest.json` & `lumacli-0.1.2/lumaCLI/tests/assets/dbt_v1.3/manifest.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.1.1/lumaCLI/tests/assets/dbt_v1.3/run_results.json` & `lumacli-0.1.2/lumaCLI/tests/assets/dbt_v1.3/run_results.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.1.1/lumaCLI/tests/assets/dbt_v1.3/sources.json` & `lumacli-0.1.2/lumaCLI/tests/assets/dbt_v1.3/sources.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.1.1/lumaCLI/tests/assets/dbt_v1.7/model_metadata/catalog.json` & `lumacli-0.1.2/lumaCLI/tests/assets/dbt_v1.7/model_metadata/catalog.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.1.1/lumaCLI/tests/assets/dbt_v1.7/model_metadata/manifest.json` & `lumacli-0.1.2/lumaCLI/tests/assets/dbt_v1.7/model_metadata/manifest.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.1.1/lumaCLI/tests/assets/dbt_v1.7/model_run_metadata/run_results.json` & `lumacli-0.1.2/lumaCLI/tests/assets/dbt_v1.7/model_run_metadata/run_results.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.1.1/lumaCLI/tests/conftest.py` & `lumacli-0.1.2/lumaCLI/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
             """groups:
   - meta_key: "domain"
     slug: "domains"
     label_plural: "Domains"
     label_singular: "Domain"
     icon: "Cube"
     in_sidebar: true
+    visible: true
   - meta_key: "true_source"
     slug: "sources"
     label_plural: "Sources"
     label_singular: "Source"
     icon: "Cloud"
     in_sidebar: false
 """
```

### Comparing `lumacli-0.1.1/lumaCLI/tests/postgres_dump_file.sql` & `lumacli-0.1.2/lumaCLI/tests/postgres_dump_file.sql`

 * *Files identical despite different names*

### Comparing `lumacli-0.1.1/lumaCLI/tests/unit/test_config.py` & `lumacli-0.1.2/lumaCLI/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.1.1/lumaCLI/tests/unit/test_dbt.py` & `lumacli-0.1.2/lumaCLI/tests/unit/test_dbt.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.1.1/lumaCLI/tests/unit/test_postgres.py` & `lumacli-0.1.2/lumaCLI/tests/unit/test_postgres.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.1.1/lumaCLI/tests/unit/test_postgres_utils.py` & `lumacli-0.1.2/lumaCLI/tests/unit/test_postgres_utils.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.1.1/lumaCLI/utils/luma_utils.py` & `lumacli-0.1.2/lumaCLI/utils/luma_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 # groups:
 #   - meta_key: "domain"
 #     slug: "domains"
 #     label_plural: "Domains"
 #     label_singular: "Domain"
 #     icon: "Cube"
 #     in_sidebar: true
+#     visible: true
 #   - meta_key: "true_source"
 #     slug: "sources"
 #     label_plural: "Sources"
 #     label_singular: "Source"
 #     icon: "Cloud"
 #     in_sidebar: true
 """
```

### Comparing `lumacli-0.1.1/lumaCLI/utils/options.py` & `lumacli-0.1.2/lumaCLI/utils/options.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.1.1/lumaCLI/utils/postgres_utils.py` & `lumacli-0.1.2/lumaCLI/utils/postgres_utils.py`

 * *Files identical despite different names*

### Comparing `lumacli-0.1.1/pyproject.toml` & `lumacli-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lumaCLI"
-version = "0.1.1"
+version = "0.1.2"
 description = "A CLI tool for managing the data catalog platform."
 authors = ["Facundo Goiriz <fgoiriz@dyvenia.com>"]
 readme = "README.md"
 license = "MIT"
 
 packages = [{ include = "lumaCLI" }]
```

### Comparing `lumacli-0.1.1/PKG-INFO` & `lumacli-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumaCLI
-Version: 0.1.1
+Version: 0.1.2
 Summary: A CLI tool for managing the data catalog platform.
 License: MIT
 Keywords: cli,dbt,luma,data,catalog
 Author: Facundo Goiriz
 Author-email: fgoiriz@dyvenia.com
 Requires-Python: >=3.8,<4
 Classifier: Development Status :: 3 - Alpha
```

