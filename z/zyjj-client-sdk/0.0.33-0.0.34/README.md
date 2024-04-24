# Comparing `tmp/zyjj_client_sdk-0.0.33.tar.gz` & `tmp/zyjj_client_sdk-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zyjj_client_sdk-0.0.33.tar", last modified: Mon Mar 18 00:16:06 2024, max compression
+gzip compressed data, was "zyjj_client_sdk-0.0.34.tar", last modified: Tue Apr 23 14:13:43 2024, max compression
```

## Comparing `zyjj_client_sdk-0.0.33.tar` & `zyjj_client_sdk-0.0.34.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 00:16:06.601290 zyjj_client_sdk-0.0.33/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-18 00:16:06.601290 zyjj_client_sdk-0.0.33/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 00:16:06.601290 zyjj_client_sdk-0.0.33/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-18 00:16:02.000000 zyjj_client_sdk-0.0.33/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 00:16:06.597290 zyjj_client_sdk-0.0.33/zyjj_client_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     8495 2024-03-18 00:16:02.000000 zyjj_client_sdk-0.0.33/zyjj_client_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 00:16:06.601290 zyjj_client_sdk-0.0.33/zyjj_client_sdk/api/
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-03-18 00:16:02.000000 zyjj_client_sdk-0.0.33/zyjj_client_sdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-18 00:16:02.000000 zyjj_client_sdk-0.0.33/zyjj_client_sdk/api/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 00:16:06.601290 zyjj_client_sdk-0.0.33/zyjj_client_sdk/base/
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-03-18 00:16:02.000000 zyjj_client_sdk-0.0.33/zyjj_client_sdk/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 00:16:06.601290 zyjj_client_sdk-0.0.33/zyjj_client_sdk/client/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-18 00:16:02.000000 zyjj_client_sdk-0.0.33/zyjj_client_sdk/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-03-18 00:16:02.000000 zyjj_client_sdk-0.0.33/zyjj_client_sdk/client/mqtt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 00:16:06.601290 zyjj_client_sdk-0.0.33/zyjj_client_sdk/decorate/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-18 00:16:02.000000 zyjj_client_sdk-0.0.33/zyjj_client_sdk/decorate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 00:16:06.601290 zyjj_client_sdk-0.0.33/zyjj_client_sdk/entity/
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-03-18 00:16:02.000000 zyjj_client_sdk-0.0.33/zyjj_client_sdk/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-03-18 00:16:02.000000 zyjj_client_sdk-0.0.33/zyjj_client_sdk/entity/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 00:16:06.601290 zyjj_client_sdk-0.0.33/zyjj_client_sdk/ffmpeg_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-03-18 00:16:02.000000 zyjj_client_sdk-0.0.33/zyjj_client_sdk/ffmpeg_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 00:16:06.601290 zyjj_client_sdk-0.0.33/zyjj_client_sdk/storage/
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-03-18 00:16:02.000000 zyjj_client_sdk-0.0.33/zyjj_client_sdk/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 00:16:06.601290 zyjj_client_sdk-0.0.33/zyjj_client_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-18 00:16:06.000000 zyjj_client_sdk-0.0.33/zyjj_client_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-18 00:16:06.000000 zyjj_client_sdk-0.0.33/zyjj_client_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 00:16:06.000000 zyjj_client_sdk-0.0.33/zyjj_client_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-18 00:16:06.000000 zyjj_client_sdk-0.0.33/zyjj_client_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-18 00:16:06.000000 zyjj_client_sdk-0.0.33/zyjj_client_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:13:43.833072 zyjj_client_sdk-0.0.34/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-23 14:13:43.833072 zyjj_client_sdk-0.0.34/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:13:43.833072 zyjj_client_sdk-0.0.34/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-23 14:13:40.000000 zyjj_client_sdk-0.0.34/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:13:43.829072 zyjj_client_sdk-0.0.34/zyjj_client_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-23 14:13:40.000000 zyjj_client_sdk-0.0.34/zyjj_client_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:13:43.829072 zyjj_client_sdk-0.0.34/zyjj_client_sdk/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-23 14:13:40.000000 zyjj_client_sdk-0.0.34/zyjj_client_sdk/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-23 14:13:40.000000 zyjj_client_sdk-0.0.34/zyjj_client_sdk/base/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-23 14:13:40.000000 zyjj_client_sdk-0.0.34/zyjj_client_sdk/base/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-23 14:13:40.000000 zyjj_client_sdk-0.0.34/zyjj_client_sdk/base/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-23 14:13:40.000000 zyjj_client_sdk-0.0.34/zyjj_client_sdk/base/mqtt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:13:43.829072 zyjj_client_sdk-0.0.34/zyjj_client_sdk/flow/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-23 14:13:40.000000 zyjj_client_sdk-0.0.34/zyjj_client_sdk/flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-23 14:13:40.000000 zyjj_client_sdk-0.0.34/zyjj_client_sdk/flow/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-04-23 14:13:40.000000 zyjj_client_sdk-0.0.34/zyjj_client_sdk/flow/flow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:13:43.833072 zyjj_client_sdk-0.0.34/zyjj_client_sdk/flow/node/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-23 14:13:40.000000 zyjj_client_sdk-0.0.34/zyjj_client_sdk/flow/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-23 14:13:40.000000 zyjj_client_sdk-0.0.34/zyjj_client_sdk/flow/node/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-04-23 14:13:40.000000 zyjj_client_sdk-0.0.34/zyjj_client_sdk/flow/node/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:13:43.833072 zyjj_client_sdk-0.0.34/zyjj_client_sdk/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-23 14:13:40.000000 zyjj_client_sdk-0.0.34/zyjj_client_sdk/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-23 14:13:40.000000 zyjj_client_sdk-0.0.34/zyjj_client_sdk/lib/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-23 14:13:40.000000 zyjj_client_sdk-0.0.34/zyjj_client_sdk/lib/oss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:13:43.833072 zyjj_client_sdk-0.0.34/zyjj_client_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-23 14:13:43.000000 zyjj_client_sdk-0.0.34/zyjj_client_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-23 14:13:43.000000 zyjj_client_sdk-0.0.34/zyjj_client_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:13:43.000000 zyjj_client_sdk-0.0.34/zyjj_client_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-23 14:13:43.000000 zyjj_client_sdk-0.0.34/zyjj_client_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 14:13:43.000000 zyjj_client_sdk-0.0.34/zyjj_client_sdk.egg-info/top_level.txt
```

### Comparing `zyjj_client_sdk-0.0.33/setup.py` & `zyjj_client_sdk-0.0.34/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='zyjj_client_sdk',
-    version='0.0.33',
+    version='0.0.34',
     description='智游剪辑客户端sdk包',
     url='https://github.com/zyjj-cc/zyjj-client-sdk',
     author='zyjj',
     author_email='zyjj.cc@foxmail.com',
     license='MIT',
     long_description="智游剪辑客户端sdk包",
     packages=find_packages(),
```

### Comparing `zyjj_client_sdk-0.0.33/zyjj_client_sdk/api/__init__.py` & `zyjj_client_sdk-0.0.34/zyjj_client_sdk/base/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import json
 import logging
-
 import requests
-from zyjj_client_sdk.base import Base
-from zyjj_client_sdk.api.model import TaskStatus
+from zyjj_client_sdk.base.base import Base
+from zyjj_client_sdk.base.entity import TaskStatus
 
 
-class Api:
+class ApiService:
     def __init__(self, base: Base):
         self.__header = {
             "x-username": base.username,
             "x-password": base.password,
             "Content-Type": "application/json"
         }
         self.__base = f"{base.host}/api/v1/client"
@@ -56,14 +55,18 @@
     def cloud_get_mqtt(self):
         return self.__request("get", f"cloud/mqtt/task")
 
     # 拉取任务
     def task_pull_task(self):
         return self.__request("get", "task/pull")
 
+    # 拉取任务流程
+    def task_pull_flow(self, task_type: int):
+        return self.__request("get", f"flow/{task_type}")
+
     # 更新任务状态
     def task_update_task(
             self,
             task_id: str,
             status: TaskStatus = None,
             point_cost: float = None,
             output: str = None,
@@ -82,14 +85,16 @@
 
     # 获取用户积分
     def get_user_point(self, uid: str) -> int:
         return self.__request("get", f"point/user/{uid}", {})
 
     # 扣除用户积分
     def use_user_point(self, uid: str, name: str, point: float, desc='') -> bool:
+        if len(desc) > 20:
+            desc = f'{desc[:20]}...'
         logging.info("[api] {} use point {}".format(uid, int(point)))
         try:
             self.__request("post", "point/deducting", {
                 "uid": uid,
                 "name": name,
                 "point": int(point),
                 "desc": desc,
```

### Comparing `zyjj_client_sdk-0.0.33/zyjj_client_sdk/base/__init__.py` & `zyjj_client_sdk-0.0.34/zyjj_client_sdk/base/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,11 +22,7 @@
     # 生成一个临时文件
     def generate_local_file(self, extend: str) -> str:
         return f"{self.tmp_dir}/{str(uuid.uuid4())}.{extend}"
 
     # 根据路径生成一个新的同名文件
     def generate_file_with_path(self, path: str) -> str:
         return self.generate_local_file(path.split(".")[-1])
-
-    # 获取配置文件
-    def get_config_data(self, key: str):
-        return self.__config[key]
```

### Comparing `zyjj_client_sdk-0.0.33/zyjj_client_sdk/client/mqtt.py` & `zyjj_client_sdk-0.0.34/zyjj_client_sdk/base/mqtt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import json
 import logging
 import threading
 from enum import Enum
 from typing import Callable
 
-from zyjj_client_sdk.api import Api
+from zyjj_client_sdk.base.api import ApiService
 import paho.mqtt.client as mqtt
 
 
 class MqttEventType(Enum):
     Start = 1  # 开始任务
     Progress = 2  # 进度事件
     Success = 3  # 成功
     Fail = 4  # 失败
 
 
 class MqttServer:
-    def __init__(self, api: Api):
+    def __init__(self, api: ApiService):
         self.__close = False
         self.__subscribe = {}
         # 获取客户端信息
         info = api.cloud_get_mqtt()
         host, client_id, username, password = (info['host'], info['client_id'], info['username'], info['password'])
         print(host, client_id, username, password)
         self.__client = mqtt.Client(client_id=client_id, protocol=mqtt.MQTTv311)
```

### Comparing `zyjj_client_sdk-0.0.33/zyjj_client_sdk/ffmpeg_sdk/__init__.py` & `zyjj_client_sdk-0.0.34/zyjj_client_sdk/lib/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `zyjj_client_sdk-0.0.33/zyjj_client_sdk/storage/__init__.py` & `zyjj_client_sdk-0.0.34/zyjj_client_sdk/lib/oss.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,94 +1,71 @@
-import json
 import logging
 
-from zyjj_client_sdk.api import Api
+from zyjj_client_sdk.base.api import ApiService
 from zyjj_client_sdk.base import Base
 from qcloud_cos import CosConfig
 from qcloud_cos import CosS3Client
 from typing import Callable
 
 
 def _callback(i: float):
     logging.info(f"[storage] current progress {i}")
 
 
-class Storage:
-    def __init__(self, base: Base, api: Api):
+class OSSService:
+    def __init__(self, base: Base, api: ApiService):
         self.__base = base
         self.__api = api
         self.__auth = None
 
     def __get_auth(self):
         if self.__auth is None:
             self.__auth = self.__api.could_get_tencent_cos()
         return self.__auth
 
-    # 下载文件
-    def download_file(self, key: str) -> str:
-        path = self.__base.generate_file_with_path(key)
-        self.__tencent_download_file(key, path, _callback)
-        return path
-
-    # 上传文件
-    def upload_file(self, path: str, uid: str, source: int) -> dict:
-        key = self.__tencent_upload_file(path, uid, _callback)
-        return {
-            "name": path.split("/")[-1],
-            "path": key,
-            "source": source
-        }
-
-    # 原始下载文件
-    def tencent_get_path_by_key(self, key: str) -> str:
-        path = self.__base.generate_file_with_path(key)
-        self.__tencent_download_file(key, path, _callback)
-        return path
-
-    # 直接上传文件
-    def tencent_get_key_by_path(self, path: str, uid: str) -> str:
-        return self.__tencent_upload_file(path, uid, _callback)
-
     def __tencent_get_client(self) -> CosS3Client:
         auth = self.__get_auth()
         token = auth["token"]
         config = CosConfig(
             Region=auth["region"],
             SecretId=token["TmpSecretId"],
             SecretKey=token["TmpSecretKey"],
             Token=token["Token"],
             Scheme="https",
         )
         return CosS3Client(config)
 
     # 下载腾讯存储文件
-    def __tencent_download_file(self, key: str, path: str, callback: Callable[[float], None] = _callback):
+    def tencent_download_file_by_key(self, key: str) -> str:
         client = self.__tencent_get_client()
+        path = self.__base.generate_file_with_path(key)
         client.download_file(
             Bucket=self.__auth["bucket"],
             Key=key,
             DestFilePath=path,
-            progress_callback=lambda finish, total: callback((finish / total) * 100),
+            # progress_callback=lambda finish, total: callback((finish / total) * 100),
         )
+        return path
 
-    def __tencent_upload_file(self, path: str, uid: str, callback: Callable[[float], None] = _callback) -> str:
+    # 本地路径上传文件
+    def tencent_upload_by_local_path(self, uid: str, path: str) -> str:
         client = self.__tencent_get_client()
-        key = f"tmp/{uid}/{self.__base.generate_file_with_path(path).split('/')[-1]}"
+        key = f"tmp/{uid}/{self.__base.generate_filename(path.split('.')[-1])}"
         client.upload_file(
             Bucket=self.__auth["bucket"],
             Key=key,
             LocalFilePath=path,
-            progress_callback=lambda finish, total: callback((finish / total) * 100),
+            # progress_callback=lambda finish, total: callback((finish / total) * 100),
         )
         return key
 
     # 上传二进制数据
-    def tencent_get_key_by_bytes(self, uid: str, key: str, data: bytes) -> str:
+    def tencent_upload_by_bytes(self, uid: str, data: bytes, ext: str) -> str:
         client = self.__tencent_get_client()
-        key = f"tmp/{uid}/{key}"
+        key = f"tmp/{uid}/{self.__base.generate_filename(ext)}"
 
         class TmpBody:
             def __init__(self, _data: bytes):
                 self.__data = _data
 
             def read(self, n: int) -> bytes:
                 if n >= len(self.__data):
@@ -105,16 +82,18 @@
             Key=key,
             Body=TmpBody(data),
         )
         return key
 
     def tencent_get_url_by_key(self, key: str, expired=180) -> str:
         client = self.__tencent_get_client()
-        return client.get_presigned_download_url(
-            Bucket=self.__auth["bucket"],
+        bucket = self.__auth["bucket"]
+        url = client.get_presigned_download_url(
+            Bucket=bucket,
             Key=key,
             Expired=expired,
+            SignHost=False,
             Params={
-                "x-cos-security-token":
-                    self.__auth["token"]["Token"]
+                "x-cos-security-token": self.__auth["token"]["Token"]
             }
         )
+        return str(url).replace(f'{bucket}.cos.{self.__auth["region"]}.myqcloud.com', 'cos-origin.zyjj.cc')
```

### Comparing `zyjj_client_sdk-0.0.33/zyjj_client_sdk.egg-info/SOURCES.txt` & `zyjj_client_sdk-0.0.34/zyjj_client_sdk.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 setup.py
 zyjj_client_sdk/__init__.py
 zyjj_client_sdk.egg-info/PKG-INFO
 zyjj_client_sdk.egg-info/SOURCES.txt
 zyjj_client_sdk.egg-info/dependency_links.txt
 zyjj_client_sdk.egg-info/requires.txt
 zyjj_client_sdk.egg-info/top_level.txt
-zyjj_client_sdk/api/__init__.py
-zyjj_client_sdk/api/model.py
 zyjj_client_sdk/base/__init__.py
-zyjj_client_sdk/client/__init__.py
-zyjj_client_sdk/client/mqtt.py
-zyjj_client_sdk/decorate/__init__.py
-zyjj_client_sdk/entity/__init__.py
-zyjj_client_sdk/entity/model.py
-zyjj_client_sdk/ffmpeg_sdk/__init__.py
-zyjj_client_sdk/storage/__init__.py
+zyjj_client_sdk/base/api.py
+zyjj_client_sdk/base/base.py
+zyjj_client_sdk/base/entity.py
+zyjj_client_sdk/base/mqtt.py
+zyjj_client_sdk/flow/__init__.py
+zyjj_client_sdk/flow/base.py
+zyjj_client_sdk/flow/flow.py
+zyjj_client_sdk/flow/node/__init__.py
+zyjj_client_sdk/flow/node/base.py
+zyjj_client_sdk/flow/node/tool.py
+zyjj_client_sdk/lib/__init__.py
+zyjj_client_sdk/lib/ffmpeg.py
+zyjj_client_sdk/lib/oss.py
```

