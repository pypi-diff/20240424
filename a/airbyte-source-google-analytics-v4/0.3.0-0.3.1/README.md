# Comparing `tmp/airbyte_source_google_analytics_v4-0.3.0.tar.gz` & `tmp/airbyte_source_google_analytics_v4-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_google_analytics_v4-0.3.0.tar", max compression
+gzip compressed data, was "airbyte_source_google_analytics_v4-0.3.1.tar", max compression
```

## Comparing `airbyte_source_google_analytics_v4-0.3.0.tar` & `airbyte_source_google_analytics_v4-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     4730 2024-03-21 01:47:20.477994 airbyte_source_google_analytics_v4-0.3.0/README.md
--rw-r--r--   0        0        0      907 2024-03-21 02:24:18.153404 airbyte_source_google_analytics_v4-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1191 2024-03-21 01:47:20.477994 airbyte_source_google_analytics_v4-0.3.0/source_google_analytics_v4/__init__.py
--rw-r--r--   0        0        0     4180 2024-03-21 01:47:20.477994 airbyte_source_google_analytics_v4-0.3.0/source_google_analytics_v4/custom_reports_validator.py
--rw-r--r--   0        0        0     2445 2024-03-21 01:47:20.477994 airbyte_source_google_analytics_v4-0.3.0/source_google_analytics_v4/defaults/default_reports.json
--rw-r--r--   0        0        0      265 2024-03-21 01:47:20.477994 airbyte_source_google_analytics_v4-0.3.0/source_google_analytics_v4/run.py
--rw-r--r--   0        0        0    26758 2024-03-21 01:47:20.477994 airbyte_source_google_analytics_v4-0.3.0/source_google_analytics_v4/source.py
--rw-r--r--   0        0        0     6378 2024-03-21 01:47:20.477994 airbyte_source_google_analytics_v4-0.3.0/source_google_analytics_v4/spec.json
--rw-r--r--   0        0        0     5575 1970-01-01 00:00:00.000000 airbyte_source_google_analytics_v4-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     4730 2024-04-24 13:37:45.646824 airbyte_source_google_analytics_v4-0.3.1/README.md
+-rw-r--r--   0        0        0      907 2024-04-24 13:45:15.637220 airbyte_source_google_analytics_v4-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1191 2024-04-24 13:37:45.646824 airbyte_source_google_analytics_v4-0.3.1/source_google_analytics_v4/__init__.py
+-rw-r--r--   0        0        0     4180 2024-04-24 13:37:45.646824 airbyte_source_google_analytics_v4-0.3.1/source_google_analytics_v4/custom_reports_validator.py
+-rw-r--r--   0        0        0     2445 2024-04-24 13:37:45.646824 airbyte_source_google_analytics_v4-0.3.1/source_google_analytics_v4/defaults/default_reports.json
+-rw-r--r--   0        0        0      265 2024-04-24 13:37:45.646824 airbyte_source_google_analytics_v4-0.3.1/source_google_analytics_v4/run.py
+-rw-r--r--   0        0        0    26892 2024-04-24 13:37:45.646824 airbyte_source_google_analytics_v4-0.3.1/source_google_analytics_v4/source.py
+-rw-r--r--   0        0        0     6378 2024-04-24 13:37:45.646824 airbyte_source_google_analytics_v4-0.3.1/source_google_analytics_v4/spec.json
+-rw-r--r--   0        0        0     5575 1970-01-01 00:00:00.000000 airbyte_source_google_analytics_v4-0.3.1/PKG-INFO
```

### Comparing `airbyte_source_google_analytics_v4-0.3.0/README.md` & `airbyte_source_google_analytics_v4-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_analytics_v4-0.3.0/pyproject.toml` & `airbyte_source_google_analytics_v4-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.3.0"
+version = "0.3.1"
 name = "airbyte-source-google-analytics-v4"
 description = "Source implementation for Google Analytics V4."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "Elv2"
 readme = "README.md"
```

### Comparing `airbyte_source_google_analytics_v4-0.3.0/source_google_analytics_v4/__init__.py` & `airbyte_source_google_analytics_v4-0.3.1/source_google_analytics_v4/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_analytics_v4-0.3.0/source_google_analytics_v4/custom_reports_validator.py` & `airbyte_source_google_analytics_v4-0.3.1/source_google_analytics_v4/custom_reports_validator.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_analytics_v4-0.3.0/source_google_analytics_v4/defaults/default_reports.json` & `airbyte_source_google_analytics_v4-0.3.1/source_google_analytics_v4/defaults/default_reports.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_analytics_v4-0.3.0/source_google_analytics_v4/source.py` & `airbyte_source_google_analytics_v4-0.3.1/source_google_analytics_v4/source.py`

 * *Files 1% similar despite different names*

```diff
@@ -529,16 +529,16 @@
         signed_jwt = jwt.encode(payload, self.client_secret, headers=headers, algorithm="RS256")
         return {"grant_type": "urn:ietf:params:oauth:grant-type:jwt-bearer", "assertion": str(signed_jwt)}
 
 
 class TestStreamConnection(GoogleAnalyticsV4Stream):
     """
     Test the connectivity and permissions to read the data from the stream.
-    Because of the nature of the connector, the streams are created dynamicaly.
-    We declare the static stream like this to be able to test out the prmissions to read the particular view_id."""
+    Because of the nature of the connector, the streams are created dynamically.
+    We declare the static stream like this to be able to test out the permissions to read the particular view_id."""
 
     page_size = 1
 
     def next_page_token(self, response: requests.Response) -> Optional[Mapping[str, Any]]:
         """For test reading pagination is not required"""
         return None
 
@@ -548,15 +548,19 @@
         """
         start_date = pendulum.parse(self.start_date).date()
         end_date = pendulum.now().date()
         return [{"startDate": self.to_datetime_str(start_date), "endDate": self.to_datetime_str(end_date)}]
 
     def parse_response(self, response: requests.Response, **kwargs: Any) -> Iterable[Mapping]:
         res = response.json()
-        return res.get("reports", {})[0].get("data")
+        try:
+            return res.get("reports", [])[0].get("data")
+        except IndexError:
+            self.logger.warning(f"No reports in response: {res}")
+            return []
 
 
 class SourceGoogleAnalyticsV4(AbstractSource):
     """Google Analytics lets you analyze data about customer engagement with your website or application."""
 
     @staticmethod
     def get_authenticator(config: Mapping) -> Oauth2Authenticator:
```

### Comparing `airbyte_source_google_analytics_v4-0.3.0/source_google_analytics_v4/spec.json` & `airbyte_source_google_analytics_v4-0.3.1/source_google_analytics_v4/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_analytics_v4-0.3.0/PKG-INFO` & `airbyte_source_google_analytics_v4-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-google-analytics-v4
-Version: 0.3.0
+Version: 0.3.1
 Summary: Source implementation for Google Analytics V4.
 Home-page: https://airbyte.com
 License: Elv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

