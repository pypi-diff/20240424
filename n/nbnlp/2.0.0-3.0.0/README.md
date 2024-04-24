# Comparing `tmp/nbnlp-2.0.0.tar.gz` & `tmp/nbnlp-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbnlp-2.0.0.tar", last modified: Fri Apr 19 08:41:26 2024, max compression
+gzip compressed data, was "nbnlp-3.0.0.tar", last modified: Wed Apr 24 08:09:09 2024, max compression
```

## Comparing `nbnlp-2.0.0.tar` & `nbnlp-3.0.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 08:41:26.334383 nbnlp-2.0.0/
--rw-rw-rw-   0        0        0      469 2024-04-14 08:16:37.000000 nbnlp-2.0.0/LICENSE
--rw-rw-rw-   0        0        0       42 2024-04-14 10:43:41.000000 nbnlp-2.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      398 2024-04-19 08:41:26.331014 nbnlp-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       18 2024-04-14 08:05:38.000000 nbnlp-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 08:41:26.290905 nbnlp-2.0.0/nbnlp/
--rw-rw-rw-   0        0        0        0 2024-04-12 16:09:58.000000 nbnlp-2.0.0/nbnlp/__init__.py
--rw-rw-rw-   0        0        0     2157 2024-04-14 10:50:18.000000 nbnlp-2.0.0/nbnlp/api.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:41:26.327273 nbnlp-2.0.0/nbnlp/data/
--rw-rw-rw-   0        0        0      169 2024-04-14 07:54:01.000000 nbnlp-2.0.0/nbnlp/data/test.tsv
--rw-rw-rw-   0        0        0      169 2024-04-14 07:54:01.000000 nbnlp-2.0.0/nbnlp/data/train.tsv
--rw-rw-rw-   0        0        0     2437 2024-04-14 08:06:29.000000 nbnlp-2.0.0/nbnlp/db.py
--rw-rw-rw-   0        0        0     2409 2024-04-14 10:30:51.000000 nbnlp-2.0.0/nbnlp/model.py
--rw-rw-rw-   0        0        0      872 2024-04-19 07:20:01.000000 nbnlp-2.0.0/nbnlp/scheduler.py
--rw-rw-rw-   0        0        0     2465 2024-04-19 08:40:11.000000 nbnlp-2.0.0/nbnlp/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-19 08:41:26.318995 nbnlp-2.0.0/nbnlp.egg-info/
--rw-rw-rw-   0        0        0      398 2024-04-19 08:41:26.000000 nbnlp-2.0.0/nbnlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2024-04-19 08:41:26.000000 nbnlp-2.0.0/nbnlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 08:41:26.000000 nbnlp-2.0.0/nbnlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-19 08:41:26.000000 nbnlp-2.0.0/nbnlp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 08:41:26.336666 nbnlp-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      726 2024-04-19 08:40:57.000000 nbnlp-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 08:09:09.422099 nbnlp-3.0.0/
+-rw-rw-rw-   0        0        0      469 2024-04-14 08:16:37.000000 nbnlp-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0       42 2024-04-14 10:43:41.000000 nbnlp-3.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      398 2024-04-24 08:09:09.419484 nbnlp-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2024-04-24 08:09:06.000000 nbnlp-3.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 08:09:09.391165 nbnlp-3.0.0/nbnlp/
+-rw-rw-rw-   0        0        0        0 2024-04-12 16:09:58.000000 nbnlp-3.0.0/nbnlp/__init__.py
+-rw-rw-rw-   0        0        0     2157 2024-04-14 10:50:18.000000 nbnlp-3.0.0/nbnlp/api.py
+drwxrwxrwx   0        0        0        0 2024-04-24 08:09:09.416186 nbnlp-3.0.0/nbnlp/data/
+-rw-rw-rw-   0        0        0      169 2024-04-14 07:54:01.000000 nbnlp-3.0.0/nbnlp/data/test.tsv
+-rw-rw-rw-   0        0        0      169 2024-04-14 07:54:01.000000 nbnlp-3.0.0/nbnlp/data/train.tsv
+-rw-rw-rw-   0        0        0     2437 2024-04-14 08:06:29.000000 nbnlp-3.0.0/nbnlp/db.py
+-rw-rw-rw-   0        0        0     2409 2024-04-14 10:30:51.000000 nbnlp-3.0.0/nbnlp/model.py
+-rw-rw-rw-   0        0        0     1653 2024-04-24 08:02:31.000000 nbnlp-3.0.0/nbnlp/ner.py
+-rw-rw-rw-   0        0        0      872 2024-04-19 07:20:01.000000 nbnlp-3.0.0/nbnlp/scheduler.py
+-rw-rw-rw-   0        0        0     2524 2024-04-24 07:52:50.000000 nbnlp-3.0.0/nbnlp/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 08:09:09.409337 nbnlp-3.0.0/nbnlp.egg-info/
+-rw-rw-rw-   0        0        0      398 2024-04-24 08:09:09.000000 nbnlp-3.0.0/nbnlp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2024-04-24 08:09:09.000000 nbnlp-3.0.0/nbnlp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 08:09:09.000000 nbnlp-3.0.0/nbnlp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-24 08:09:09.000000 nbnlp-3.0.0/nbnlp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-24 08:09:09.000000 nbnlp-3.0.0/nbnlp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 08:09:09.422099 nbnlp-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      716 2024-04-24 07:08:45.000000 nbnlp-3.0.0/setup.py
+-rw-rw-rw-   0        0        0      274 2024-04-24 08:07:38.000000 nbnlp-3.0.0/upload.md
```

### Comparing `nbnlp-2.0.0/nbnlp/api.py` & `nbnlp-3.0.0/nbnlp/api.py`

 * *Files identical despite different names*

### Comparing `nbnlp-2.0.0/nbnlp/db.py` & `nbnlp-3.0.0/nbnlp/db.py`

 * *Files identical despite different names*

### Comparing `nbnlp-2.0.0/nbnlp/model.py` & `nbnlp-3.0.0/nbnlp/model.py`

 * *Files identical despite different names*

### Comparing `nbnlp-2.0.0/nbnlp/scheduler.py` & `nbnlp-3.0.0/nbnlp/scheduler.py`

 * *Files identical despite different names*

### Comparing `nbnlp-2.0.0/nbnlp/utils.py` & `nbnlp-3.0.0/nbnlp/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,30 @@
+import os
 import json
 from mysql.connector import Error
-from flask import Flask, request, Response
+from flask import Flask, request, jsonify, make_response
 
+# 默认配置
 default_config = {
     'host': '0.0.0.0',
     'port': 8080,
     'debug': False,
 }
 
+# 设置环境变量
+def set_environment_variable(name, value):
+    """
+    设置环境变量。
+
+    参数:
+    - name: 环境变量的名称。
+    - value: 要设置的值。
+    """
+    os.environ[name] = value
+
 # 去除空格
 def trim(data, key, default=""):
     value = data.get(key, default)
     if isinstance(value, str):
         return value.strip()
     return value
 
@@ -76,15 +89,13 @@
 
 # 发送数据
 def send_data(code=0, msg="数据获取成功。", data=None):
     response_content = {"code": code, "msg": msg}
     if data is not None:
         response_content["data"] = data
     status = 200 if code == 0 else code
-    response_json = json.dumps(response_content, ensure_ascii=False)  # 使用json.dumps并设置ensure_ascii=False
-    response = Response(response_json, status=status, mimetype='application/json; charset=utf-8')  # 创建Response对象
-    return response
+    return make_response(jsonify(response_content), status)
 
 # 运行服务
 def run(app, config = default_config):
     final_config = {**default_config, **config}
     app.run(**final_config)
```

### Comparing `nbnlp-2.0.0/setup.py` & `nbnlp-3.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nbnlp',
-    version="2.0.0",
+    version="3.0.0",
     packages=find_packages(),
     include_package_data=True,
     author="xl",
     author_email="123456@qq.com",
     description="A short description of your package",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
@@ -15,14 +15,14 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ],
     package_data={
         'nbnlp': ['data/*', 'model/*'],
     },
     install_requires=[
-        # 'mysql-connector-python',
-        # 'hanlp',
-        # 'Flask',
-        # 'APScheduler',
-        # 'requests'
+        'mysql-connector-python',
+        'hanlp',
+        'Flask',
+        'APScheduler',
+        'requests'
     ]
 )
```

