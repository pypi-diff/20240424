# Comparing `tmp/server_templates-0.2.8.tar.gz` & `tmp/server_templates-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "server_templates-0.2.8.tar", last modified: Mon Apr 22 09:33:21 2024, max compression
+gzip compressed data, was "server_templates-0.2.9.tar", last modified: Mon Apr 22 09:45:19 2024, max compression
```

## Comparing `server_templates-0.2.8.tar` & `server_templates-0.2.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 09:33:21.746378 server_templates-0.2.8/
--rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 server_templates-0.2.8/LICENSE
--rw-rw-rw-   0        0        0     1970 2024-04-22 09:33:21.746378 server_templates-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     1115 2024-04-22 09:33:02.000000 server_templates-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 09:33:21.735039 server_templates-0.2.8/server_templates/
--rw-rw-rw-   0        0        0      196 2024-04-17 12:25:31.000000 server_templates-0.2.8/server_templates/__init__.py
--rw-rw-rw-   0        0        0     7623 2024-03-05 15:09:35.000000 server_templates-0.2.8/server_templates/client_requests.py
-drwxrwxrwx   0        0        0        0 2024-04-22 09:33:21.742671 server_templates-0.2.8/server_templates/server_aiohttp/
--rw-rw-rw-   0        0        0       19 2024-01-29 15:35:36.000000 server_templates-0.2.8/server_templates/server_aiohttp/__init__.py
--rw-rw-rw-   0        0        0    10652 2024-03-29 11:33:06.000000 server_templates-0.2.8/server_templates/server_aiohttp/main.py
-drwxrwxrwx   0        0        0        0 2024-04-22 09:33:21.744554 server_templates-0.2.8/server_templates/server_fastapi/
--rw-rw-rw-   0        0        0       19 2024-01-29 15:35:36.000000 server_templates-0.2.8/server_templates/server_fastapi/__init__.py
--rw-rw-rw-   0        0        0    21396 2024-04-22 09:19:01.000000 server_templates-0.2.8/server_templates/server_fastapi/main.py
-drwxrwxrwx   0        0        0        0 2024-04-22 09:33:21.745350 server_templates-0.2.8/server_templates.egg-info/
--rw-rw-rw-   0        0        0     1970 2024-04-22 09:33:21.000000 server_templates-0.2.8/server_templates.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2024-04-22 09:33:21.000000 server_templates-0.2.8/server_templates.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 09:33:21.000000 server_templates-0.2.8/server_templates.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-22 09:33:21.000000 server_templates-0.2.8/server_templates.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 09:33:21.748705 server_templates-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     2092 2024-01-30 06:52:17.000000 server_templates-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 09:45:19.193019 server_templates-0.2.9/
+-rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 server_templates-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0     1970 2024-04-22 09:45:19.193019 server_templates-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1115 2024-04-22 09:45:02.000000 server_templates-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 09:45:19.182577 server_templates-0.2.9/server_templates/
+-rw-rw-rw-   0        0        0      196 2024-04-17 12:25:31.000000 server_templates-0.2.9/server_templates/__init__.py
+-rw-rw-rw-   0        0        0     7623 2024-03-05 15:09:35.000000 server_templates-0.2.9/server_templates/client_requests.py
+drwxrwxrwx   0        0        0        0 2024-04-22 09:45:19.188565 server_templates-0.2.9/server_templates/server_aiohttp/
+-rw-rw-rw-   0        0        0       19 2024-01-29 15:35:36.000000 server_templates-0.2.9/server_templates/server_aiohttp/__init__.py
+-rw-rw-rw-   0        0        0    10652 2024-03-29 11:33:06.000000 server_templates-0.2.9/server_templates/server_aiohttp/main.py
+drwxrwxrwx   0        0        0        0 2024-04-22 09:45:19.190893 server_templates-0.2.9/server_templates/server_fastapi/
+-rw-rw-rw-   0        0        0       19 2024-01-29 15:35:36.000000 server_templates-0.2.9/server_templates/server_fastapi/__init__.py
+-rw-rw-rw-   0        0        0    21476 2024-04-22 09:44:37.000000 server_templates-0.2.9/server_templates/server_fastapi/main.py
+drwxrwxrwx   0        0        0        0 2024-04-22 09:45:19.191990 server_templates-0.2.9/server_templates.egg-info/
+-rw-rw-rw-   0        0        0     1970 2024-04-22 09:45:19.000000 server_templates-0.2.9/server_templates.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2024-04-22 09:45:19.000000 server_templates-0.2.9/server_templates.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 09:45:19.000000 server_templates-0.2.9/server_templates.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-22 09:45:19.000000 server_templates-0.2.9/server_templates.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 09:45:19.194018 server_templates-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     2092 2024-01-30 06:52:17.000000 server_templates-0.2.9/setup.py
```

### Comparing `server_templates-0.2.8/LICENSE` & `server_templates-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `server_templates-0.2.8/PKG-INFO` & `server_templates-0.2.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: server_templates
-Version: 0.2.8
+Version: 0.2.9
 Summary: templates for servers
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/server_templates
 Keywords: api,api server,http server,aiohttp,FastApi
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# server_templates (v0.2.8)
+# server_templates (v0.2.9)
 
 ## DESCRIPTION_SHORT
 templates for servers
 
 ## DESCRIPTION_LONG
 designed for keep all servers templates in one place
```

### Comparing `server_templates-0.2.8/README.md` & `server_templates-0.2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# server_templates (v0.2.8)
+# server_templates (v0.2.9)
 
 ## DESCRIPTION_SHORT
 templates for servers
 
 ## DESCRIPTION_LONG
 designed for keep all servers templates in one place
```

### Comparing `server_templates-0.2.8/server_templates/client_requests.py` & `server_templates-0.2.9/server_templates/client_requests.py`

 * *Files identical despite different names*

### Comparing `server_templates-0.2.8/server_templates/server_aiohttp/main.py` & `server_templates-0.2.9/server_templates/server_aiohttp/main.py`

 * *Files identical despite different names*

### Comparing `server_templates-0.2.8/server_templates/server_fastapi/main.py` & `server_templates-0.2.9/server_templates/server_fastapi/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -511,17 +511,20 @@
     """
     HOST: str = "0.0.0.0"
     PORT: int = 80
 
     data: Any = None
     create_app: Callable[[Any], FastAPI] = create_app__FastApi
 
-    def __init__(self, app: FastAPI = None, *args, **kwargs):
+    def __init__(self, app: FastAPI = None, data: Any = None, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
+        if data is not None:
+            self.data = data
+
         if app is None:
             app = self.create_app(data=self.data)
         self.app = app
 
     def run(self):
         uvicorn.run(self.app, host=self.HOST, port=self.PORT)
```

### Comparing `server_templates-0.2.8/server_templates.egg-info/PKG-INFO` & `server_templates-0.2.9/server_templates.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: server_templates
-Version: 0.2.8
+Version: 0.2.9
 Summary: templates for servers
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/server_templates
 Keywords: api,api server,http server,aiohttp,FastApi
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# server_templates (v0.2.8)
+# server_templates (v0.2.9)
 
 ## DESCRIPTION_SHORT
 templates for servers
 
 ## DESCRIPTION_LONG
 designed for keep all servers templates in one place
```

### Comparing `server_templates-0.2.8/setup.py` & `server_templates-0.2.9/setup.py`

 * *Files identical despite different names*

