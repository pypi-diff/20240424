# Comparing `tmp/t2d2-sdk-1.4.9.tar.gz` & `tmp/t2d2-sdk-1.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t2d2-sdk-1.4.9.tar", last modified: Fri Feb  9 21:02:49 2024, max compression
+gzip compressed data, was "t2d2-sdk-1.4.dev1.tar", last modified: Mon Jan 29 02:04:09 2024, max compression
```

## Comparing `t2d2-sdk-1.4.9.tar` & `t2d2-sdk-1.4.dev1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 21:02:49.249213 t2d2-sdk-1.4.9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 21:02:49.249213 t2d2-sdk-1.4.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 21:02:49.249213 t2d2-sdk-1.4.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-02-09 21:02:41.000000 t2d2-sdk-1.4.9/.github/workflows/publish_pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-02-09 21:02:41.000000 t2d2-sdk-1.4.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-02-09 21:02:41.000000 t2d2-sdk-1.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-02-09 21:02:49.249213 t2d2-sdk-1.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-02-09 21:02:41.000000 t2d2-sdk-1.4.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-02-09 21:02:41.000000 t2d2-sdk-1.4.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 21:02:49.249213 t2d2-sdk-1.4.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 21:02:49.249213 t2d2-sdk-1.4.9/src/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-09 21:02:49.000000 t2d2-sdk-1.4.9/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 21:02:49.249213 t2d2-sdk-1.4.9/src/t2d2_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-02-09 21:02:49.000000 t2d2-sdk-1.4.9/src/t2d2_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-02-09 21:02:49.000000 t2d2-sdk-1.4.9/src/t2d2_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 21:02:49.000000 t2d2-sdk-1.4.9/src/t2d2_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-09 21:02:49.000000 t2d2-sdk-1.4.9/src/t2d2_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-09 21:02:49.000000 t2d2-sdk-1.4.9/src/t2d2_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    22847 2024-02-09 21:02:41.000000 t2d2-sdk-1.4.9/src/t2d2_sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 21:02:49.249213 t2d2-sdk-1.4.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-02-09 21:02:41.000000 t2d2-sdk-1.4.9/tests/t2d2_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 02:04:09.030934 t2d2-sdk-1.4.dev1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 02:04:09.026934 t2d2-sdk-1.4.dev1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 02:04:09.030934 t2d2-sdk-1.4.dev1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-01-29 02:04:01.000000 t2d2-sdk-1.4.dev1/.github/workflows/publish_pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-01-29 02:04:01.000000 t2d2-sdk-1.4.dev1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-01-29 02:04:01.000000 t2d2-sdk-1.4.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-01-29 02:04:09.030934 t2d2-sdk-1.4.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-01-29 02:04:01.000000 t2d2-sdk-1.4.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-01-29 02:04:01.000000 t2d2-sdk-1.4.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-29 02:04:09.030934 t2d2-sdk-1.4.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 02:04:09.030934 t2d2-sdk-1.4.dev1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-01-29 02:04:08.000000 t2d2-sdk-1.4.dev1/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 02:04:09.030934 t2d2-sdk-1.4.dev1/src/t2d2_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-01-29 02:04:09.000000 t2d2-sdk-1.4.dev1/src/t2d2_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-01-29 02:04:09.000000 t2d2-sdk-1.4.dev1/src/t2d2_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 02:04:09.000000 t2d2-sdk-1.4.dev1/src/t2d2_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-29 02:04:09.000000 t2d2-sdk-1.4.dev1/src/t2d2_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-29 02:04:09.000000 t2d2-sdk-1.4.dev1/src/t2d2_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16531 2024-01-29 02:04:01.000000 t2d2-sdk-1.4.dev1/src/t2d2_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 02:04:09.030934 t2d2-sdk-1.4.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-01-29 02:04:01.000000 t2d2-sdk-1.4.dev1/tests/t2d2_test.py
```

### Comparing `t2d2-sdk-1.4.9/.github/workflows/publish_pypi.yaml` & `t2d2-sdk-1.4.dev1/.github/workflows/publish_pypi.yaml`

 * *Files identical despite different names*

### Comparing `t2d2-sdk-1.4.9/LICENSE` & `t2d2-sdk-1.4.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `t2d2-sdk-1.4.9/PKG-INFO` & `t2d2-sdk-1.4.dev1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t2d2-sdk
-Version: 1.4.9
+Version: 1.4.dev1
 Summary: T2D2 SDK
 Author-email: Badri Hiriyur <badri@t2d2.ai>
 Project-URL: Homepage, https://t2d2.ai
 Project-URL: Issues, https://github.com/t2d2-ai/t2d2-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `t2d2-sdk-1.4.9/README.md` & `t2d2-sdk-1.4.dev1/README.md`

 * *Files identical despite different names*

### Comparing `t2d2-sdk-1.4.9/pyproject.toml` & `t2d2-sdk-1.4.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `t2d2-sdk-1.4.9/src/t2d2_sdk.egg-info/PKG-INFO` & `t2d2-sdk-1.4.dev1/src/t2d2_sdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t2d2-sdk
-Version: 1.4.9
+Version: 1.4.dev1
 Summary: T2D2 SDK
 Author-email: Badri Hiriyur <badri@t2d2.ai>
 Project-URL: Homepage, https://t2d2.ai
 Project-URL: Issues, https://github.com/t2d2-ai/t2d2-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `t2d2-sdk-1.4.9/src/t2d2_sdk.py` & `t2d2-sdk-1.4.dev1/src/t2d2_sdk.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """T2D2 SDK API wrapper"""
-
-import json
 import os
 import random
 import string
 from enum import Enum, auto
 from urllib.parse import urlencode, urlparse
 
 import boto3
@@ -18,20 +16,14 @@
 ####################################################################################################
 def random_string(length: int = 6) -> str:
     """Generate a random string of fixed length"""
     letters = string.ascii_lowercase
     return "".join(random.choice(letters) for i in range(length))
 
 
-def random_color() -> str:
-    """Generate a random color"""
-    r = lambda: random.randint(0, 255)
-    return "#%02X%02X%02X" % (r(), r(), r())
-
-
 ####################################################################################################
 def download_file(url: str, file_path: str):
     """Download a file from a url to a local path"""
     try:
         s3 = boto3.client("s3")
         parsed_url = urlparse(url)
         bucket = parsed_url.netloc.split(".")[0]
@@ -79,15 +71,14 @@
     headers: dict
     s3_base_url: str
     aws_region: str
     bucket: str
     access_token: str
     api_key: str
     project: dict = None
-    debug: bool = True
 
     def __init__(self, credentials, base_url=BASE_URL):
         """Initialize / login"""
         if not base_url.endswith("/"):
             base_url += "/"
         self.base_url = base_url
         self.headers = {"Content-Type": "application/json"}
@@ -109,62 +100,57 @@
             headers = {}
         if params is None:
             params = {}
         if data is None:
             data = {}
 
         headers.update(self.headers)
-        params_enc = {key: json.dumps(val) for key, val in params.items()}
         if req_type == RequestType.GET:
             res = requests.get(
-                url,
-                headers=headers,
-                params=urlencode(params_enc),
-                timeout=TIMEOUT,
+                url, headers=headers, params=urlencode(params), timeout=TIMEOUT
             )
         elif req_type == RequestType.POST:
             res = requests.post(
                 url,
                 headers=headers,
-                params=urlencode(params_enc),
+                params=urlencode(params),
                 json=data,
                 timeout=TIMEOUT,
             )
         elif req_type == RequestType.PUT:
             res = requests.put(
                 url,
                 headers=headers,
-                params=urlencode(params_enc),
+                params=urlencode(params),
                 json=data,
                 timeout=TIMEOUT,
             )
         elif req_type == RequestType.DELETE:
             res = requests.delete(
                 url,
                 headers=headers,
-                params=urlencode(params_enc),
+                params=urlencode(params),
                 json=data,
                 timeout=TIMEOUT,
             )
         else:
             raise ValueError("Request type not yet supported. Coming soon")
 
-        if res.status_code in (200, 201):
+        if res.status_code == 200:
             try:
                 return res.json()
             except Exception as e:
                 print("JSON Conversion Error: ", e)
                 return {"content": res.content}
         else:
-            if self.debug:
-                print(f"URL: {req_type} {res.url}")
-                print(f"HEADERS: {headers}")
-                print(f"PARAMS: {params}")
-                print(f"DATA: {data}")
-                print(res.status_code, res.content)
+            print(f"URL: {req_type} {url}")
+            print(f"HEADERS: {headers}")
+            print(f"PARAMS: {params}")
+            print(f"DATA: {data}")
+            print(res.status_code, res.content)
             raise ValueError(f"Error code received: {res.status_code}")
 
     def login(self, credentials):
         """Login and update header with authorization credentials"""
 
         if "access_token" in credentials:
             # Directly use token
@@ -183,29 +169,23 @@
             self.headers["x-api-key"] = self.api_key
 
         return
 
     ################################################################################################
     # Project Get/Set
     ################################################################################################
-    def get_project(self, project_id=None):
+    def get_project(self, project_id):
         """Return project list"""
-        if project_id is None:
-            url = "project"
-        else:
-            url = f"project/{project_id}"
+        url = f"project/{project_id}"
         json_data = self.request(url, RequestType.GET)
         return json_data["data"]
 
     def set_project(self, project_id):
         """Set project by project_id"""
         json_data = self.request(f"project/{project_id}", RequestType.GET)
-        if not json_data["success"]:
-            raise ValueError(json_data["message"])
-
         project = json_data["data"]
         self.project = project
 
         self.s3_base_url = project["config"]["s3_base_url"]
         self.aws_region = project["config"]["aws_region"]
         res = urlparse(self.s3_base_url)
         self.bucket = res.netloc.split(".")[0]
@@ -226,15 +206,15 @@
         payload = {"asset_type": asset_type, "asset_ids": asset_ids}
         json_data = self.request(url, RequestType.POST, data=payload)
         return json_data["data"]
 
     def get_images(self, image_ids=None, params=None):
         """Return image list based on specified ids"""
         if not self.project:
-            raise ValueError("Project not set yet")
+            raise ValueError("Project not set")
 
         # all images in project
         if image_ids is None:
             url = f"{self.project['id']}/images"
             json_data = self.request(url, RequestType.GET, params=params)
             results = json_data["data"]["image_list"]
             return results
@@ -288,98 +268,53 @@
         results = []
         for report_id in report_ids:
             url = f"{self.project['id']}/reports/{report_id}"
             json_data = self.request(url, RequestType.GET, params=params)
             results.append(json_data["data"])
         return results
 
-    def download_assets(
-        self, asset_ids, asset_type=1, download_dir="./", original_filename=False
-    ):
-        """Download assets"""
-        if not self.project:
-            raise ValueError("Project not set")
-
-        assets = self.get_assets(asset_type, asset_ids)
-        if len(assets) != len(asset_ids):
-            raise ValueError("Some assets not found")
-
-        output = {}
-        for asset in assets:
-            url = asset["url"]
-            if original_filename:
-                file_name = asset["filename"]
-            else:
-                ext = os.path.splitext(asset["filename"])[1]
-                file_name = f"img_{asset['id']}{ext}"
-            file_path = os.path.join(download_dir, file_name)
-            output[asset["id"]] = file_path
-            response = download_file(url, file_path)
-            if not response["success"]:
-                raise ValueError(response["message"])
-
-        return output
-
-    ################################################################################################
-    # Update methods
-    ################################################################################################
-    def update_images(self, image_ids, payload):
-        """Update images"""
-        if not self.project:
-            raise ValueError("Project not set")
-
-        url = f"{self.project['id']}/images/bulk.update"
-        payload["image_ids"] = image_ids
-        payload["project_id"] = self.project["id"]
-        return self.request(url, RequestType.PUT, data=payload)
-
     ################################################################################################
     # Add / Upload Asset methods
     ################################################################################################
     def add_assets(self, payload):
         """Add assets"""
         url = f"{self.project['id']}/assets/bulk.create"
         return self.request(url, RequestType.POST, data=payload)
 
-    def upload_images(self, image_paths, image_type=1, params=None):
+    def upload_images(self, image_paths, image_type=1):
         """Upload images"""
 
         if not self.project:
             raise ValueError("Project not set")
 
         # Upload images to S3
         assets = []
         for file_path in image_paths:
             base, ext = os.path.splitext(os.path.basename(file_path))
             filename = f"{base}_{random_string(6)}{ext}"
             s3_path = (
                 self.s3_base_url + f"/projects/{self.project['id']}/images/{filename}"
             )
-            result = upload_file(file_path, s3_path)
-            if result.get("success", False):
-                assets.append(
-                    {
-                        "name": base,
-                        "filename": base + ext,
-                        "url": filename,
-                        "size": {"filesize": os.path.getsize(file_path)},
-                    }
-                )
+            upload_file(file_path, s3_path)
+            assets.append(
+                {
+                    "name": base,
+                    "filename": base + ext,
+                    "url": filename,
+                    "size": {"filesize": os.path.getsize(file_path)},
+                }
+            )
 
         # Add images to project
         payload = {
             "project_id": self.project["id"],
             "asset_type": 1,
             "image_type": image_type,
             "assets": assets,
         }
-
-        if params is not None:
-            payload.update(params)
-
         return self.add_assets(payload)
 
     def upload_drawings(self, drawing_paths):
         """Upload drawings"""
 
         if not self.project:
             raise ValueError("Project not set")
@@ -524,87 +459,18 @@
 
         url = "annotation"
         payload = {
             "project_id": self.project["id"],
             "image_id": image_id,
             "annotations": annotations,
         }
-
-        results = self.request(url, RequestType.POST, data=payload)
-
-        return results
-
-    def get_materials(self):
-        """Return material list"""
-        if not self.project:
-            raise ValueError("Project not set")
-
-        url = "material"
-        params = {"project_id": self.project["id"]}
-        json_data = self.request(url, RequestType.GET, params=params)
-        return json_data["data"]
-
-    def get_annotation_classes(self, params=None):
-        """Return annotation class list"""
-        if not self.project:
-            raise ValueError("Project not set")
-
-        url = "annotation-class"
-        params_ = {
-            "project_id": self.project["id"],
-            "scope": "DEFAULT",
-            "sortBy": "id:asc",
-        }
-        if params is not None:
-            params_.update(params)
-
-        print(params_)
-
-        json_data = self.request(url, RequestType.GET, params=params_)
-        return json_data["data"]
-
-    def add_annotation_class(self, name, color=None, materials=None):
-        """Add annotation class"""
-        if not self.project:
-            raise ValueError("Project not set")
-
-        if materials is None:
-            materials = []
-
-        if color is None:
-            color = random_color()
-
-        url = "annotation-class/create-annotation-class"
-        payload = {
-            "project_id": self.project["id"],
-            "name": name,
-            "materials": materials,
-            "color": color,
-        }
         results = self.request(url, RequestType.POST, data=payload)
 
         return results
 
-    def delete_annotation_classes(self, annotation_class_ids):
-        """Delete annotation class"""
-        if not self.project:
-            raise ValueError("Project not set")
-
-        if isinstance(annotation_class_ids, int):
-            annotation_class_ids = [annotation_class_ids]
-
-        if len(annotation_class_ids) == 0:
-            return {"success": False, "message": "No annotation class ids provided"}
-
-        url = f"{self.project['id']}/annotation-class/bulk.delete"
-        payload = {"annotation_class_ids": annotation_class_ids}
-        results = self.request(url, RequestType.DELETE, data=payload)
-
-        return results
-
     ################################################################################################
     # Geotag methods
     ################################################################################################
     def get_geotags(self, drawing_id, params=None):
         """Return annotation list based on specified ids"""
         if drawing_id is None:
             return []
@@ -612,69 +478,7 @@
         if not self.project:
             raise ValueError("Project not set")
 
         url = f"{self.project['id']}/geotags?drawing_id={drawing_id}"
         json_data = self.request(url, RequestType.GET, params=params)
 
         return json_data["data"]
-
-    def add_geotags(self, drawing_id, geotags):
-        """Add geotags"""
-        if not self.project:
-            raise ValueError("Project not set")
-
-        url = f"{self.project['id']}/geotags/bulk.create"
-        payload = {
-            "drawing_id": drawing_id,
-            "geotags": geotags,
-        }
-        results = self.request(url, RequestType.POST, data=payload)
-
-        return results
-
-    def delete_geotags(self, drawing_id, geotag_ids):
-        """Delete geotags"""
-        if not self.project:
-            raise ValueError("Project not set")
-
-        url = f"{self.project['id']}/geotags/bulk.delete"
-        payload = {
-            "drawing_id": drawing_id,
-            "geotag_ids": geotag_ids,
-        }
-        results = self.request(url, RequestType.POST, data=payload)
-
-        return results
-
-    # TODO: Update Geotags
-
-    ################################################################################################
-    # Tag methods
-    ################################################################################################
-    def get_tags(self, params=None):
-        """Return tag list"""
-        if not self.project:
-            raise ValueError("Project not set")
-
-        url = f"{self.project['id']}/tags"
-        json_data = self.request(url, RequestType.GET, params=params)
-        return json_data["data"]
-
-    def add_tags(self, tags):
-        """Add tags"""
-        if not self.project:
-            raise ValueError("Project not set")
-
-        url = f"{self.project['id']}/tags"
-        if isinstance(tags, str):
-            tags = [tags]
-
-        results = []
-        for tag in tags:
-            payload = {"name": tag}
-            try:
-                result = self.request(url, RequestType.POST, data=payload)
-                results.append(result)
-            except Exception as e:
-                print("*WARNING* Tag already exists: ", e)
-
-        return results
```

### Comparing `t2d2-sdk-1.4.9/tests/t2d2_test.py` & `t2d2-sdk-1.4.dev1/tests/t2d2_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,18 +21,18 @@
         points.append([random.random(), random.random()])
     return points
 
 
 def gen_random_box():
     """Return random box points"""
     points = [
-        0.1 + 0.05 * random.random(),
-        0.2 + 0.05 * random.random(),
-        0.4 + 0.05 * random.random(),
-        0.8 + 0.05 * random.random(),
+        0.1 + 0.01 * random.random(),
+        0.2 + 0.01 * random.random(),
+        0.4 + 0.01 * random.random(),
+        0.8 + 0.01 * random.random(),
     ]
     return points
 
 
 def generate_random_annotations(n=10):
     """Generate random annotations"""
     annotations = []
@@ -59,28 +59,17 @@
     def test_random_string(self):
         # Test random_string function
         result = random_string(length=6)
         self.assertEqual(len(result), 6)
 
     def test_project(self):
         # Test project function
-        res = self.t2d2.get_project()
-        project_count = res["total_projects"]
-        # print("Total Projects: ", project_count)
-        self.assertEqual(project_count, 273)
-
         project = self.t2d2.get_project(PROJECT_ID)
         self.assertEqual(project["id"], PROJECT_ID)
 
-    def test_unauthorized(self):
-        # Test unauthorized function
-        t2d2 = T2D2(credentials={"api_key": "test"}, base_url=BASE_URL)
-        t2d2.debug = False
-        self.assertRaises(ValueError, t2d2.get_project, PROJECT_ID)
-
     def test_images(self):
         # Get Images
         images = self.t2d2.get_images(params={"image_types": [1, 2, 4]})
         self.assertEqual(len(images), 205)
 
         # Get Images
         orthos = self.t2d2.get_images(params={"image_types": [3]})
```

