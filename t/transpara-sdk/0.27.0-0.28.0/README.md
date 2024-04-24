# Comparing `tmp/transpara_sdk-0.27.0.tar.gz` & `tmp/transpara_sdk-0.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transpara_sdk-0.27.0.tar", last modified: Wed Apr 17 22:07:02 2024, max compression
+gzip compressed data, was "transpara_sdk-0.28.0.tar", last modified: Wed Apr 24 21:03:09 2024, max compression
```

## Comparing `transpara_sdk-0.27.0.tar` & `transpara_sdk-0.28.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-17 22:07:02.279675 transpara_sdk-0.27.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2024-01-17 13:58:36.000000 transpara_sdk-0.27.0/LICENSE.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      480 2024-04-17 22:07:02.279675 transpara_sdk-0.27.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2175 2023-09-25 15:54:29.000000 transpara_sdk-0.27.0/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      693 2024-04-17 22:06:55.000000 transpara_sdk-0.27.0/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-17 22:07:02.279675 transpara_sdk-0.27.0/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-17 22:07:02.275675 transpara_sdk-0.27.0/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-17 22:07:02.279675 transpara_sdk-0.27.0/src/transpara/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-09-25 15:54:29.000000 transpara_sdk-0.27.0/src/transpara/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-17 22:07:02.279675 transpara_sdk-0.27.0/src/transpara/internal/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3355 2024-01-17 16:45:29.000000 transpara_sdk-0.27.0/src/transpara/internal/settings.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2755 2023-09-25 15:54:29.000000 transpara_sdk-0.27.0/src/transpara/logging_config.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14487 2023-09-25 15:54:29.000000 transpara_sdk-0.27.0/src/transpara/tlogging.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6838 2023-09-25 15:54:29.000000 transpara_sdk-0.27.0/src/transpara/tracing.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-17 22:07:02.279675 transpara_sdk-0.27.0/src/transpara_sdk.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      480 2024-04-17 22:07:02.000000 transpara_sdk-0.27.0/src/transpara_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      399 2024-04-17 22:07:02.000000 transpara_sdk-0.27.0/src/transpara_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-17 22:07:02.000000 transpara_sdk-0.27.0/src/transpara_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      201 2024-04-17 22:07:02.000000 transpara_sdk-0.27.0/src/transpara_sdk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2024-04-17 22:07:02.000000 transpara_sdk-0.27.0/src/transpara_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-17 22:07:02.279675 transpara_sdk-0.27.0/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1036 2023-09-25 17:41:05.000000 transpara_sdk-0.27.0/tests/tests.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 21:03:09.503326 transpara_sdk-0.28.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2024-01-17 13:58:36.000000 transpara_sdk-0.28.0/LICENSE.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      480 2024-04-24 21:03:09.503326 transpara_sdk-0.28.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2175 2023-09-25 15:54:29.000000 transpara_sdk-0.28.0/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      693 2024-04-24 21:02:40.000000 transpara_sdk-0.28.0/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-24 21:03:09.503326 transpara_sdk-0.28.0/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 21:03:09.499326 transpara_sdk-0.28.0/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 21:03:09.499326 transpara_sdk-0.28.0/src/transpara/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-09-25 15:54:29.000000 transpara_sdk-0.28.0/src/transpara/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 21:03:09.499326 transpara_sdk-0.28.0/src/transpara/internal/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3432 2024-04-24 21:02:24.000000 transpara_sdk-0.28.0/src/transpara/internal/settings.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2755 2023-09-25 15:54:29.000000 transpara_sdk-0.28.0/src/transpara/logging_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14487 2023-09-25 15:54:29.000000 transpara_sdk-0.28.0/src/transpara/tlogging.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6838 2023-09-25 15:54:29.000000 transpara_sdk-0.28.0/src/transpara/tracing.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 21:03:09.503326 transpara_sdk-0.28.0/src/transpara_sdk.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      480 2024-04-24 21:03:09.000000 transpara_sdk-0.28.0/src/transpara_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      399 2024-04-24 21:03:09.000000 transpara_sdk-0.28.0/src/transpara_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-24 21:03:09.000000 transpara_sdk-0.28.0/src/transpara_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      201 2024-04-24 21:03:09.000000 transpara_sdk-0.28.0/src/transpara_sdk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2024-04-24 21:03:09.000000 transpara_sdk-0.28.0/src/transpara_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 21:03:09.503326 transpara_sdk-0.28.0/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1036 2023-09-25 17:41:05.000000 transpara_sdk-0.28.0/tests/tests.py
```

### Comparing `transpara_sdk-0.27.0/LICENSE.txt` & `transpara_sdk-0.28.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `transpara_sdk-0.27.0/README.md` & `transpara_sdk-0.28.0/README.md`

 * *Files identical despite different names*

### Comparing `transpara_sdk-0.27.0/pyproject.toml` & `transpara_sdk-0.28.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 author = "Transpara"
 author_email = "arturo.aguilar@transpara.com"
 
 [project]
 name = "transpara-sdk"
-version = "0.27.0"
+version = "0.28.0"
 description = "Transpara Python SDK"
 dependencies = [
     "jsonpickle==1.4.2",
     "asyncio==3.4.3",
     "opentelemetry-api==1.20.0",
     "opentelemetry-sdk==1.20.0",
     "opentelemetry-exporter-otlp==1.20.0",
```

### Comparing `transpara_sdk-0.27.0/src/transpara/internal/settings.py` & `transpara_sdk-0.28.0/src/transpara/internal/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,16 @@
         try:
             return float(v)
         except:
             return v
 
     def load_settings(self):
         try:
-            response = requests.get(f"http://{required_settings.TSYSTEM_HOST}/{required_settings.TSYSTEM_COMPONENT_TYPE}/{required_settings.COMPONENT_ID}")
+            timeout = getenv("TSYSTEM_SETTINGS_TIMEOUT", 1)
+            response = requests.get(f"http://{required_settings.TSYSTEM_HOST}/{required_settings.TSYSTEM_COMPONENT_TYPE}/{required_settings.COMPONENT_ID}", timeout=timeout)
             response.raise_for_status()
             settings: dict = response.json()["settings"]
             for key, value in settings.items():
                 if hasattr(self, key): 
                     setattr(self, key, value)
         except:
```

### Comparing `transpara_sdk-0.27.0/src/transpara/logging_config.py` & `transpara_sdk-0.28.0/src/transpara/logging_config.py`

 * *Files identical despite different names*

### Comparing `transpara_sdk-0.27.0/src/transpara/tlogging.py` & `transpara_sdk-0.28.0/src/transpara/tlogging.py`

 * *Files identical despite different names*

### Comparing `transpara_sdk-0.27.0/src/transpara/tracing.py` & `transpara_sdk-0.28.0/src/transpara/tracing.py`

 * *Files identical despite different names*

### Comparing `transpara_sdk-0.27.0/tests/tests.py` & `transpara_sdk-0.28.0/tests/tests.py`

 * *Files identical despite different names*

