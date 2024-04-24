# Comparing `tmp/xagpy-0.2.tar.gz` & `tmp/xagpy-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xagpy-0.2.tar", last modified: Sat Apr 20 13:26:39 2024, max compression
+gzip compressed data, was "xagpy-0.3.tar", last modified: Wed Apr 24 14:55:42 2024, max compression
```

## Comparing `xagpy-0.2.tar` & `xagpy-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:26:39.267424 xagpy-0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-20 13:26:35.000000 xagpy-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-20 13:26:39.267424 xagpy-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-20 13:26:35.000000 xagpy-0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 13:26:39.267424 xagpy-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-20 13:26:35.000000 xagpy-0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:26:39.267424 xagpy-0.2/xagpy/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-20 13:26:35.000000 xagpy-0.2/xagpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-20 13:26:35.000000 xagpy-0.2/xagpy/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 13:26:39.267424 xagpy-0.2/xagpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-20 13:26:39.000000 xagpy-0.2/xagpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-20 13:26:39.000000 xagpy-0.2/xagpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 13:26:39.000000 xagpy-0.2/xagpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 13:26:39.000000 xagpy-0.2/xagpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-20 13:26:39.000000 xagpy-0.2/xagpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:55:42.145764 xagpy-0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-24 14:55:36.000000 xagpy-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-24 14:55:42.145764 xagpy-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-24 14:55:36.000000 xagpy-0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 14:55:42.145764 xagpy-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-24 14:55:36.000000 xagpy-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:55:42.145764 xagpy-0.3/xagpy/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-24 14:55:36.000000 xagpy-0.3/xagpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-24 14:55:36.000000 xagpy-0.3/xagpy/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:55:42.145764 xagpy-0.3/xagpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-24 14:55:42.000000 xagpy-0.3/xagpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-24 14:55:42.000000 xagpy-0.3/xagpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:55:42.000000 xagpy-0.3/xagpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 14:55:42.000000 xagpy-0.3/xagpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 14:55:42.000000 xagpy-0.3/xagpy.egg-info/top_level.txt
```

### Comparing `xagpy-0.2/LICENSE` & `xagpy-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xagpy-0.2/PKG-INFO` & `xagpy-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xagpy
-Version: 0.2
+Version: 0.3
 Summary: Api wrapper for the Xag(Xbox account generator) api
 Home-page: https://github.com/dropalways/xagpy
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
```

### Comparing `xagpy-0.2/README.md` & `xagpy-0.3/README.md`

 * *Files identical despite different names*

### Comparing `xagpy-0.2/xagpy/api.py` & `xagpy-0.3/xagpy/api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import requests
 
 
 class xagpy:
-    def __init__(self, api_token):
+    def __init__(self, api_token) -> None:
         if api_token is None or api_token == "":
             raise ValueError("API token is invalid")
         self.api_token = api_token
         self.base_url = "https://xag.fly.dev/api"
         try:
             response = requests.get(f"{self.base_url}/stock", timeout=3)
-        except Exception as e:
-            if response.status_code == 200:  # probably works i havent tested too much
+        except Exception as e:  # probably works i havent tested too much
+            if response.status_code == 200:
                 pass
             else:
                 print(
                     "Error has occurred while connecting to the API. It's likely that the API is offline, or you are offline.\n", e)
 
     def _handle_response(self, response):
         try:
@@ -26,36 +26,43 @@
                 429: "You have sent too many requests. | 429",
                 401: "Unauthorised. | 401",
                 400: "Bad request. | 400",
 
 
             }
             error_message = error_messages.get(
-                status_code, "Unexpected response | Status Code:")
+                status_code, f"Unexpected response | Status Code: {status_code} | Error Message: {response.json}")
             if status_code == 200:
                 pass
             else:
-                print(error_message, status_code)
+                print(error_message)
             if status_code == 200:
                 return response.json()
         except requests.exceptions.HTTPError as e:
             print("HTTP error occurred:", e)
         return None
 
-    def generate_account(self, test_mode=False, timeout=3):
-        url = f"{self.base_url}/generate?type=xbox"
+    def generate_account(self, test_mode=False, timeout=3, xag_plus=False) -> object:
+        if xag_plus:
+            url = f"{self.base_url}/generate?type=xbox_plus"
+        elif not xag_plus:
+            url = f"{self.base_url}/generate?type=xbox"
+        else:
+            # this never should happen if this happens, we are all doomed.
+            url = f"{self.base_url}/generate?type=xbox"
+            print("wtf happend heere this code shoudl-d work??!?!?!!")
         if test_mode:
             url += "&test_mode"
         headers = {"api-token": self.api_token}
         response = requests.post(url, headers=headers, timeout=timeout)
         return self._handle_response(response)
 
-    def get_stock(self, timeout=3):
+    def get_stock(self, timeout=3) -> object:
         url = f"{self.base_url}/stock"
         response = requests.get(url, timeout=timeout)
         return self._handle_response(response)
 
-    def get_coins(self, timeout=3):
+    def get_coins(self, timeout=3) -> object:
         url = f"{self.base_url}/coins"
         headers = {"api-token": self.api_token}
         response = requests.get(url, headers=headers, timeout=timeout)
         return self._handle_response(response)
```

### Comparing `xagpy-0.2/xagpy.egg-info/PKG-INFO` & `xagpy-0.3/xagpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xagpy
-Version: 0.2
+Version: 0.3
 Summary: Api wrapper for the Xag(Xbox account generator) api
 Home-page: https://github.com/dropalways/xagpy
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
```

