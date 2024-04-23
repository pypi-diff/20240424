# Comparing `tmp/thoughtful-3.0.0.tar.gz` & `tmp/thoughtful-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thoughtful-3.0.0.tar", max compression
+gzip compressed data, was "thoughtful-3.0.1.tar", max compression
```

## Comparing `thoughtful-3.0.0.tar` & `thoughtful-3.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11358 2023-09-07 18:37:51.725925 thoughtful-3.0.0/LICENSE
--rw-r--r--   0        0        0     2992 2023-09-07 18:37:51.725925 thoughtful-3.0.0/README.md
--rw-r--r--   0        0        0     1935 2023-09-07 18:37:51.725925 thoughtful-3.0.0/pyproject.toml
--rw-r--r--   0        0        0      222 2023-09-07 18:37:51.725925 thoughtful-3.0.0/thoughtful/__init__.py
--rw-r--r--   0        0        0       54 2023-09-07 18:37:51.725925 thoughtful-3.0.0/thoughtful/__version__.py
--rw-r--r--   0        0        0     1070 2023-09-07 18:37:51.725925 thoughtful-3.0.0/thoughtful/environment_variables.py
--rw-r--r--   0        0        0      143 2023-09-07 18:37:51.725925 thoughtful-3.0.0/thoughtful/supervisor/__init__.py
--rw-r--r--   0        0        0     6846 2023-09-07 18:37:51.725925 thoughtful-3.0.0/thoughtful/supervisor/default_instances.py
--rw-r--r--   0        0        0     1074 2023-09-07 18:37:51.725925 thoughtful-3.0.0/thoughtful/supervisor/event_bus.py
--rw-r--r--   0        0        0     8756 2023-09-07 18:37:51.729925 thoughtful-3.0.0/thoughtful/supervisor/main_context.py
--rw-r--r--   0        0        0    10567 2023-09-07 18:37:51.729925 thoughtful-3.0.0/thoughtful/supervisor/manifest.py
--rw-r--r--   0        0        0        0 2023-09-07 18:37:51.729925 thoughtful-3.0.0/thoughtful/supervisor/py.typed
--rw-r--r--   0        0        0        0 2023-09-07 18:37:51.729925 thoughtful-3.0.0/thoughtful/supervisor/reporting/__init__.py
--rw-r--r--   0        0        0     3037 2023-09-07 18:37:51.729925 thoughtful-3.0.0/thoughtful/supervisor/reporting/record.py
--rw-r--r--   0        0        0     1189 2023-09-07 18:37:51.729925 thoughtful-3.0.0/thoughtful/supervisor/reporting/record_report.py
--rw-r--r--   0        0        0     2066 2023-09-07 18:37:51.729925 thoughtful-3.0.0/thoughtful/supervisor/reporting/report.py
--rw-r--r--   0        0        0    12297 2023-09-07 18:37:51.729925 thoughtful-3.0.0/thoughtful/supervisor/reporting/report_builder.py
--rw-r--r--   0        0        0      660 2023-09-07 18:37:51.729925 thoughtful-3.0.0/thoughtful/supervisor/reporting/status.py
--rw-r--r--   0        0        0      876 2023-09-07 18:37:51.729925 thoughtful-3.0.0/thoughtful/supervisor/reporting/step_report.py
--rw-r--r--   0        0        0     1541 2023-09-07 18:37:51.729925 thoughtful-3.0.0/thoughtful/supervisor/reporting/timed_report.py
--rw-r--r--   0        0        0     1754 2023-09-07 18:37:51.729925 thoughtful-3.0.0/thoughtful/supervisor/reporting/timer.py
--rw-r--r--   0        0        0     8097 2023-09-07 18:37:51.729925 thoughtful-3.0.0/thoughtful/supervisor/step_context.py
--rw-r--r--   0        0        0     6713 2023-09-07 18:37:51.729925 thoughtful-3.0.0/thoughtful/supervisor/step_decorator_factory.py
--rw-r--r--   0        0        0        0 2023-09-07 18:37:51.729925 thoughtful-3.0.0/thoughtful/supervisor/streaming/__init__.py
--rw-r--r--   0        0        0      736 2023-09-07 18:37:51.729925 thoughtful-3.0.0/thoughtful/supervisor/streaming/action.py
--rw-r--r--   0        0        0     1386 2023-09-07 18:37:51.729925 thoughtful-3.0.0/thoughtful/supervisor/streaming/jwt_auth.py
--rw-r--r--   0        0        0     3124 2023-09-07 18:37:51.729925 thoughtful-3.0.0/thoughtful/supervisor/streaming/payloads.py
--rw-r--r--   0        0        0     4752 2023-09-07 18:37:51.729925 thoughtful-3.0.0/thoughtful/supervisor/streaming/streamer.py
--rw-r--r--   0        0        0     1352 2023-09-07 18:37:51.729925 thoughtful-3.0.0/thoughtful/supervisor/streaming/token.py
--rw-r--r--   0        0        0     4578 1970-01-01 00:00:00.000000 thoughtful-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-09-12 19:32:12.901194 thoughtful-3.0.1/LICENSE
+-rw-r--r--   0        0        0     2992 2023-09-12 19:32:12.901194 thoughtful-3.0.1/README.md
+-rw-r--r--   0        0        0     1935 2023-09-12 19:32:12.905194 thoughtful-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0      222 2023-09-12 19:32:12.905194 thoughtful-3.0.1/thoughtful/__init__.py
+-rw-r--r--   0        0        0       54 2023-09-12 19:32:12.905194 thoughtful-3.0.1/thoughtful/__version__.py
+-rw-r--r--   0        0        0     1070 2023-09-12 19:32:12.905194 thoughtful-3.0.1/thoughtful/environment_variables.py
+-rw-r--r--   0        0        0      143 2023-09-12 19:32:12.905194 thoughtful-3.0.1/thoughtful/supervisor/__init__.py
+-rw-r--r--   0        0        0     6963 2023-09-12 19:32:12.905194 thoughtful-3.0.1/thoughtful/supervisor/default_instances.py
+-rw-r--r--   0        0        0     1074 2023-09-12 19:32:12.905194 thoughtful-3.0.1/thoughtful/supervisor/event_bus.py
+-rw-r--r--   0        0        0     8756 2023-09-12 19:32:12.905194 thoughtful-3.0.1/thoughtful/supervisor/main_context.py
+-rw-r--r--   0        0        0    10567 2023-09-12 19:32:12.905194 thoughtful-3.0.1/thoughtful/supervisor/manifest.py
+-rw-r--r--   0        0        0        0 2023-09-12 19:32:12.905194 thoughtful-3.0.1/thoughtful/supervisor/py.typed
+-rw-r--r--   0        0        0        0 2023-09-12 19:32:12.905194 thoughtful-3.0.1/thoughtful/supervisor/reporting/__init__.py
+-rw-r--r--   0        0        0     3037 2023-09-12 19:32:12.905194 thoughtful-3.0.1/thoughtful/supervisor/reporting/record.py
+-rw-r--r--   0        0        0     1189 2023-09-12 19:32:12.905194 thoughtful-3.0.1/thoughtful/supervisor/reporting/record_report.py
+-rw-r--r--   0        0        0     2066 2023-09-12 19:32:12.905194 thoughtful-3.0.1/thoughtful/supervisor/reporting/report.py
+-rw-r--r--   0        0        0    12297 2023-09-12 19:32:12.905194 thoughtful-3.0.1/thoughtful/supervisor/reporting/report_builder.py
+-rw-r--r--   0        0        0      660 2023-09-12 19:32:12.905194 thoughtful-3.0.1/thoughtful/supervisor/reporting/status.py
+-rw-r--r--   0        0        0      876 2023-09-12 19:32:12.905194 thoughtful-3.0.1/thoughtful/supervisor/reporting/step_report.py
+-rw-r--r--   0        0        0     1541 2023-09-12 19:32:12.905194 thoughtful-3.0.1/thoughtful/supervisor/reporting/timed_report.py
+-rw-r--r--   0        0        0     1754 2023-09-12 19:32:12.905194 thoughtful-3.0.1/thoughtful/supervisor/reporting/timer.py
+-rw-r--r--   0        0        0     8097 2023-09-12 19:32:12.905194 thoughtful-3.0.1/thoughtful/supervisor/step_context.py
+-rw-r--r--   0        0        0     6713 2023-09-12 19:32:12.905194 thoughtful-3.0.1/thoughtful/supervisor/step_decorator_factory.py
+-rw-r--r--   0        0        0        0 2023-09-12 19:32:12.905194 thoughtful-3.0.1/thoughtful/supervisor/streaming/__init__.py
+-rw-r--r--   0        0        0      736 2023-09-12 19:32:12.905194 thoughtful-3.0.1/thoughtful/supervisor/streaming/action.py
+-rw-r--r--   0        0        0     1547 2023-09-12 19:32:12.905194 thoughtful-3.0.1/thoughtful/supervisor/streaming/jwt_auth.py
+-rw-r--r--   0        0        0     3124 2023-09-12 19:32:12.905194 thoughtful-3.0.1/thoughtful/supervisor/streaming/payloads.py
+-rw-r--r--   0        0        0     4913 2023-09-12 19:32:12.905194 thoughtful-3.0.1/thoughtful/supervisor/streaming/streamer.py
+-rw-r--r--   0        0        0     1352 2023-09-12 19:32:12.905194 thoughtful-3.0.1/thoughtful/supervisor/streaming/token.py
+-rw-r--r--   0        0        0     4578 1970-01-01 00:00:00.000000 thoughtful-3.0.1/PKG-INFO
```

### Comparing `thoughtful-3.0.0/LICENSE` & `thoughtful-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `thoughtful-3.0.0/README.md` & `thoughtful-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `thoughtful-3.0.0/pyproject.toml` & `thoughtful-3.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thoughtful"
-version = "3.0.0"
+version = "3.0.1"
 description = "Thoughtful is a python package by Thoughtful for helping manage automations with helpful packages like supervisor"
 authors = ["Thoughtful Automation <care@thoughtful.ai>"]
 license = "Apache-2.0"
 readme = 'README.md'
 homepage = "https://thoughtful.ai"
 repository = "https://github.com/thoughtful-automation/thoughtful"
 documentation = "https://thoughtful-supervisor.readthedocs-hosted.com/en/latest/index.html"
```

### Comparing `thoughtful-3.0.0/thoughtful/environment_variables.py` & `thoughtful-3.0.1/thoughtful/environment_variables.py`

 * *Files identical despite different names*

### Comparing `thoughtful-3.0.0/thoughtful/supervisor/default_instances.py` & `thoughtful-3.0.1/thoughtful/supervisor/default_instances.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,17 @@
     run_id = EnvironmentVariables().run_id
     logger.info(f"Run ID required: {run_id}")
     if not run_id:
         warnings.warn(
             "No run ID found in environment variables, so I can't stream" "to Fabric."
         )
         return
-
+    logger.info(
+        f"Connecting to Fabric, {webhook_url}, {access_token}, {refresh_token}, {refresh_url}"
+    )
     fabric_auth = JWTAuth(
         access_token=Token(encoded_value=access_token),
         refresh_token=Token(encoded_value=refresh_token),
         refresh_url=refresh_url,
     )
     logger.info(
         "Connecting to Fabric with run ID %s and callback_url %s", run_id, webhook_url
```

### Comparing `thoughtful-3.0.0/thoughtful/supervisor/event_bus.py` & `thoughtful-3.0.1/thoughtful/supervisor/event_bus.py`

 * *Files identical despite different names*

### Comparing `thoughtful-3.0.0/thoughtful/supervisor/main_context.py` & `thoughtful-3.0.1/thoughtful/supervisor/main_context.py`

 * *Files identical despite different names*

### Comparing `thoughtful-3.0.0/thoughtful/supervisor/manifest.py` & `thoughtful-3.0.1/thoughtful/supervisor/manifest.py`

 * *Files identical despite different names*

### Comparing `thoughtful-3.0.0/thoughtful/supervisor/reporting/record.py` & `thoughtful-3.0.1/thoughtful/supervisor/reporting/record.py`

 * *Files identical despite different names*

### Comparing `thoughtful-3.0.0/thoughtful/supervisor/reporting/record_report.py` & `thoughtful-3.0.1/thoughtful/supervisor/reporting/record_report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-3.0.0/thoughtful/supervisor/reporting/report.py` & `thoughtful-3.0.1/thoughtful/supervisor/reporting/report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-3.0.0/thoughtful/supervisor/reporting/report_builder.py` & `thoughtful-3.0.1/thoughtful/supervisor/reporting/report_builder.py`

 * *Files identical despite different names*

### Comparing `thoughtful-3.0.0/thoughtful/supervisor/reporting/status.py` & `thoughtful-3.0.1/thoughtful/supervisor/reporting/status.py`

 * *Files identical despite different names*

### Comparing `thoughtful-3.0.0/thoughtful/supervisor/reporting/step_report.py` & `thoughtful-3.0.1/thoughtful/supervisor/reporting/step_report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-3.0.0/thoughtful/supervisor/reporting/timed_report.py` & `thoughtful-3.0.1/thoughtful/supervisor/reporting/timed_report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-3.0.0/thoughtful/supervisor/reporting/timer.py` & `thoughtful-3.0.1/thoughtful/supervisor/reporting/timer.py`

 * *Files identical despite different names*

### Comparing `thoughtful-3.0.0/thoughtful/supervisor/step_context.py` & `thoughtful-3.0.1/thoughtful/supervisor/step_context.py`

 * *Files identical despite different names*

### Comparing `thoughtful-3.0.0/thoughtful/supervisor/step_decorator_factory.py` & `thoughtful-3.0.1/thoughtful/supervisor/step_decorator_factory.py`

 * *Files identical despite different names*

### Comparing `thoughtful-3.0.0/thoughtful/supervisor/streaming/action.py` & `thoughtful-3.0.1/thoughtful/supervisor/streaming/action.py`

 * *Files identical despite different names*

### Comparing `thoughtful-3.0.0/thoughtful/supervisor/streaming/jwt_auth.py` & `thoughtful-3.0.1/thoughtful/supervisor/streaming/jwt_auth.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,17 +16,20 @@
 @dataclass
 class JWTAuth(AuthBase):
     access_token: Token
     refresh_token: Token
     refresh_url: str
 
     def __call__(self, r: requests.Request) -> requests.Request:
-        logger.info("JWT auth called")
         self.refresh()
         r.headers["Authorization"] = f"Bearer {self.access_token}"
+        logger.info(f"JWT auth called with request: {r}")
+        logger.debug(f"JWT auth called with token {self.access_token}")
+        logger.warning(f"JWT auth called with headers: {r.headers}")
+
         return r
 
     def refresh(self) -> None:
         if not self.access_token.is_expired:
             return
 
         logger.info("Access token expired, refreshing")
```

### Comparing `thoughtful-3.0.0/thoughtful/supervisor/streaming/payloads.py` & `thoughtful-3.0.1/thoughtful/supervisor/streaming/payloads.py`

 * *Files identical despite different names*

### Comparing `thoughtful-3.0.0/thoughtful/supervisor/streaming/streamer.py` & `thoughtful-3.0.1/thoughtful/supervisor/streaming/streamer.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,14 +47,17 @@
         refresh_token: str,
         refresh_url: str,
     ) -> Streamer:
         """
         Convenience constructor for creating an instance from the string
         (encoded) JWT tokens.
         """
+        logger.info(
+            f"JWT Auth: {access_token}, {refresh_token}, {refresh_url}, {callback_url}"
+        )
         new_auth = JWTAuth(
             access_token=Token(access_token) if access_token else None,
             refresh_token=Token(refresh_token) if refresh_token else None,
             refresh_url=refresh_url,
         )
         return cls(
             run_id=run_id,
@@ -112,15 +115,17 @@
             )
         except Exception:
             # A failed stream message shouldn't break a bot, so catch any possible
             # exception and log it
             logger.exception("Could not post step payload to endpoint")
             return
 
-        logger.info(f"Received response: ({response.status_code}): {response.text}")
+        logger.info(
+            f"Received response: ({response.status_code}): {response.text}, {response.headers}"
+        )
 
         return response
 
 
 if __name__ == "__main__":
     at = "xxxxxx"
     rt = "yyyyyy"
```

### Comparing `thoughtful-3.0.0/thoughtful/supervisor/streaming/token.py` & `thoughtful-3.0.1/thoughtful/supervisor/streaming/token.py`

 * *Files identical despite different names*

### Comparing `thoughtful-3.0.0/PKG-INFO` & `thoughtful-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thoughtful
-Version: 3.0.0
+Version: 3.0.1
 Summary: Thoughtful is a python package by Thoughtful for helping manage automations with helpful packages like supervisor
 Home-page: https://thoughtful.ai
 License: Apache-2.0
 Keywords: rpa,robot-framework,robocorp,automation
 Author: Thoughtful Automation
 Author-email: care@thoughtful.ai
 Requires-Python: >=3.8,<3.12
```

