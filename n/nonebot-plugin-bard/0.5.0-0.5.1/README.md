# Comparing `tmp/nonebot_plugin_bard-0.5.0.tar.gz` & `tmp/nonebot_plugin_bard-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bard-0.5.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_bard-0.5.1.tar", max compression
```

## Comparing `nonebot_plugin_bard-0.5.0.tar` & `nonebot_plugin_bard-0.5.1.tar`

### file list

```diff
@@ -1,8 +1,17 @@
--rw-r--r--   0        0        0     2405 2024-04-23 03:28:09.973333 nonebot_plugin_bard-0.5.0/README.md
--rw-r--r--   0        0        0     5123 2024-04-23 03:26:35.474716 nonebot_plugin_bard-0.5.0/nonebot_plugin_bard/__init__.py
--rw-r--r--   0        0        0      539 2024-04-23 03:26:54.720592 nonebot_plugin_bard-0.5.0/nonebot_plugin_bard/config.py
--rw-r--r--   0        0        0   188156 2024-04-23 03:25:58.592485 nonebot_plugin_bard-0.5.0/nonebot_plugin_bard/images/demo1.jpg
--rw-r--r--   0        0        0   120205 2024-04-23 03:25:58.593504 nonebot_plugin_bard-0.5.0/nonebot_plugin_bard/images/demo2.jpg
--rw-r--r--   0        0        0   147000 2024-04-23 03:25:58.594370 nonebot_plugin_bard-0.5.0/nonebot_plugin_bard/images/demo3.jpg
--rw-r--r--   0        0        0      525 2024-04-23 03:28:32.466457 nonebot_plugin_bard-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3035 1970-01-01 00:00:00.000000 nonebot_plugin_bard-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     2405 2024-04-24 11:10:11.460100 nonebot_plugin_bard-0.5.1/README.md
+-rw-r--r--   0        0        0     5123 2024-04-24 11:10:11.462727 nonebot_plugin_bard-0.5.1/nonebot_plugin_bard/__init__.py
+-rw-r--r--   0        0        0      539 2024-04-24 11:10:11.462859 nonebot_plugin_bard-0.5.1/nonebot_plugin_bard/config.py
+-rw-r--r--   0        0        0      147 2024-04-24 11:10:11.460397 nonebot_plugin_bard-0.5.1/nonebot_plugin_bard/gemini_webapi/__init__.py
+-rw-r--r--   0        0        0    15769 2024-04-24 11:11:20.886368 nonebot_plugin_bard-0.5.1/nonebot_plugin_bard/gemini_webapi/client.py
+-rw-r--r--   0        0        0      405 2024-04-24 11:10:11.461387 nonebot_plugin_bard-0.5.1/nonebot_plugin_bard/gemini_webapi/constant.py
+-rw-r--r--   0        0        0      548 2024-04-24 11:10:11.461683 nonebot_plugin_bard-0.5.1/nonebot_plugin_bard/gemini_webapi/exceptions.py
+-rw-r--r--   0        0        0      163 2024-04-24 11:10:11.462138 nonebot_plugin_bard-0.5.1/nonebot_plugin_bard/gemini_webapi/types/__init__.py
+-rw-r--r--   0        0        0     1111 2024-04-24 11:10:11.462263 nonebot_plugin_bard-0.5.1/nonebot_plugin_bard/gemini_webapi/types/candidate.py
+-rw-r--r--   0        0        0     4786 2024-04-24 11:10:11.462367 nonebot_plugin_bard-0.5.1/nonebot_plugin_bard/gemini_webapi/types/image.py
+-rw-r--r--   0        0        0     1121 2024-04-24 11:10:11.462453 nonebot_plugin_bard-0.5.1/nonebot_plugin_bard/gemini_webapi/types/modeloutput.py
+-rw-r--r--   0        0        0      992 2024-04-24 11:10:11.462547 nonebot_plugin_bard-0.5.1/nonebot_plugin_bard/gemini_webapi/utils.py
+-rw-r--r--   0        0        0   188156 2024-04-24 11:10:11.463670 nonebot_plugin_bard-0.5.1/nonebot_plugin_bard/images/demo1.jpg
+-rw-r--r--   0        0        0   120205 2024-04-24 11:10:11.464762 nonebot_plugin_bard-0.5.1/nonebot_plugin_bard/images/demo2.jpg
+-rw-r--r--   0        0        0   147000 2024-04-24 11:10:11.465517 nonebot_plugin_bard-0.5.1/nonebot_plugin_bard/images/demo3.jpg
+-rw-r--r--   0        0        0      525 2024-04-24 11:11:38.918981 nonebot_plugin_bard-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3035 1970-01-01 00:00:00.000000 nonebot_plugin_bard-0.5.1/PKG-INFO
```

### Comparing `nonebot_plugin_bard-0.5.0/README.md` & `nonebot_plugin_bard-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bard-0.5.0/nonebot_plugin_bard/__init__.py` & `nonebot_plugin_bard-0.5.1/nonebot_plugin_bard/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bard-0.5.0/nonebot_plugin_bard/config.py` & `nonebot_plugin_bard-0.5.1/nonebot_plugin_bard/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bard-0.5.0/nonebot_plugin_bard/images/demo1.jpg` & `nonebot_plugin_bard-0.5.1/nonebot_plugin_bard/images/demo1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bard-0.5.0/nonebot_plugin_bard/images/demo2.jpg` & `nonebot_plugin_bard-0.5.1/nonebot_plugin_bard/images/demo2.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bard-0.5.0/nonebot_plugin_bard/images/demo3.jpg` & `nonebot_plugin_bard-0.5.1/nonebot_plugin_bard/images/demo3.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bard-0.5.0/pyproject.toml` & `nonebot_plugin_bard-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-bard"
-version = "0.5.0"
+version = "0.5.1"
 description = "A nonebot plugin for Bard"
 authors = ["Alpaca <alpaca@bupt.edu.cn>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `nonebot_plugin_bard-0.5.0/PKG-INFO` & `nonebot_plugin_bard-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bard
-Version: 0.5.0
+Version: 0.5.1
 Summary: A nonebot plugin for Bard
 License: MIT
 Author: Alpaca
 Author-email: alpaca@bupt.edu.cn
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bard Version: 0.5.0 Summary: A
+Metadata-Version: 2.1 Name: nonebot-plugin-bard Version: 0.5.1 Summary: A
 nonebot plugin for Bard License: MIT Author: Alpaca Author-email:
 alpaca@bupt.edu.cn Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: nonebot-adapter-onebot (>=2.2.1,<3.0.0) Requires-Dist: nonebot2
 (>=2.0.0rc3,<3.0.0) Requires-Dist: websocket-client (>=1.6.1,<2.0.0)
```

