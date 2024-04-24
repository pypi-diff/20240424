# Comparing `tmp/pyneople-0.2.3.tar.gz` & `tmp/pyneople-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneople-0.2.3.tar", last modified: Tue Apr 23 03:53:13 2024, max compression
+gzip compressed data, was "pyneople-0.2.4.tar", last modified: Wed Apr 24 12:54:41 2024, max compression
```

## Comparing `pyneople-0.2.3.tar` & `pyneople-0.2.4.tar`

### file list

```diff
@@ -1,28 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:53:13.915385 pyneople-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-23 03:53:03.000000 pyneople-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-23 03:53:13.915385 pyneople-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-23 03:53:03.000000 pyneople-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-23 03:53:03.000000 pyneople-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 03:53:13.915385 pyneople-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-23 03:53:03.000000 pyneople-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:53:13.911385 pyneople-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:53:13.911385 pyneople-0.2.3/src/pyneople/
--rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-04-23 03:53:03.000000 pyneople-0.2.3/src/pyneople/METADATA.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 03:53:03.000000 pyneople-0.2.3/src/pyneople/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-23 03:53:03.000000 pyneople-0.2.3/src/pyneople/avatars.py
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-23 03:53:03.000000 pyneople-0.2.3/src/pyneople/buff.py
--rw-r--r--   0 runner    (1001) docker     (127)    33657 2024-04-23 03:53:03.000000 pyneople-0.2.3/src/pyneople/character.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-23 03:53:03.000000 pyneople-0.2.3/src/pyneople/character_fame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-23 03:53:03.000000 pyneople-0.2.3/src/pyneople/character_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-23 03:53:03.000000 pyneople-0.2.3/src/pyneople/character_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-04-23 03:53:03.000000 pyneople-0.2.3/src/pyneople/database_connecter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7593 2024-04-23 03:53:03.000000 pyneople-0.2.3/src/pyneople/equipments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-04-23 03:53:03.000000 pyneople-0.2.3/src/pyneople/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-04-23 03:53:03.000000 pyneople-0.2.3/src/pyneople/others.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-23 03:53:03.000000 pyneople-0.2.3/src/pyneople/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-23 03:53:03.000000 pyneople-0.2.3/src/pyneople/timeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:53:13.915385 pyneople-0.2.3/src/pyneople.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-23 03:53:13.000000 pyneople-0.2.3/src/pyneople.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-23 03:53:13.000000 pyneople-0.2.3/src/pyneople.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 03:53:13.000000 pyneople-0.2.3/src/pyneople.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 03:53:13.000000 pyneople-0.2.3/src/pyneople.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:54:41.292426 pyneople-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-24 12:54:30.000000 pyneople-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-24 12:54:41.292426 pyneople-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-24 12:54:30.000000 pyneople-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-24 12:54:30.000000 pyneople-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 12:54:41.292426 pyneople-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-24 12:54:30.000000 pyneople-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:54:41.288426 pyneople-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:54:41.288426 pyneople-0.2.4/src/pyneople/
+-rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-04-24 12:54:30.000000 pyneople-0.2.4/src/pyneople/METADATA.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 12:54:30.000000 pyneople-0.2.4/src/pyneople/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33657 2024-04-24 12:54:30.000000 pyneople-0.2.4/src/pyneople/character.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-04-24 12:54:30.000000 pyneople-0.2.4/src/pyneople/database_connecter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-04-24 12:54:30.000000 pyneople-0.2.4/src/pyneople/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:54:41.292426 pyneople-0.2.4/src/pyneople.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-24 12:54:41.000000 pyneople-0.2.4/src/pyneople.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-24 12:54:41.000000 pyneople-0.2.4/src/pyneople.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 12:54:41.000000 pyneople-0.2.4/src/pyneople.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 12:54:41.000000 pyneople-0.2.4/src/pyneople.egg-info/top_level.txt
```

### Comparing `pyneople-0.2.3/LICENSE` & `pyneople-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneople-0.2.3/PKG-INFO` & `pyneople-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneople
-Version: 0.2.3
+Version: 0.2.4
 Summary: Neople Open API wrapper for data analyst
 Home-page: https://github.com/ippo252525/pyneople
 Author: ippo252525
 Author-email: ippo252525@gmail.com
 Project-URL: Bug Tracker, https://github.com/ippo252525/pyneople/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyneople-0.2.3/setup.py` & `pyneople-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyneople",
-    version="0.2.3",
+    version="0.2.4",
     author="ippo252525",
     author_email="ippo252525@gmail.com",
     description="Neople Open API wrapper for data analyst",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ippo252525/pyneople",
     project_urls={
```

### Comparing `pyneople-0.2.3/src/pyneople/METADATA.py` & `pyneople-0.2.4/src/pyneople/METADATA.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.2.3/src/pyneople/character.py` & `pyneople-0.2.4/src/pyneople/character.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.2.3/src/pyneople/database_connecter.py` & `pyneople-0.2.4/src/pyneople/database_connecter.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.2.3/src/pyneople/functions.py` & `pyneople-0.2.4/src/pyneople/functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 import json
 import requests
 from .METADATA import JOBCLASS
 from .METADATA import SETTINGS
 
 __all__ = ['change_settings', 'get_request', 'jobname_equalize', 'get_job_info', 'system_maintenance']
 
+class PyneopleError(Exception):
+    def __init__(self, *args: object) -> None:
+        super().__init__(*args)
+
+class ServerMaintenanceError(Exception):
+    def __init__(self, *args: object) -> None:
+        super().__init__(*args)
+
 def change_settings(arg_time_out : int = 5, arg_time_sleep : float = 0.0015):
     """
     request에 필요한 설정 값을 바꾸는 함수
 
     초기 설정 값은 각각 5초, 0.0015초
         Args :
             arg_time_out(int) : 해당 시간동안 응답이 없으면 에러 처리한다
@@ -27,15 +35,18 @@
             arg_url(str) : 원하는 url 주소
     """
     start_time = time.time()
     data = requests.get(arg_url, timeout = SETTINGS['request_time_out'])
     data = json.loads(data.text)
     # Neople Open API 상에서 규정된 에러가 발생할 경우 에러를 발생시킨다.
     if data.get("error"):
-        raise Exception(data.get("error"))
+        if data.get("error").get('status') == 503:
+            raise ServerMaintenanceError
+        else:
+            raise PyneopleError(data.get("error"))
     elapsed_time = time.time() - start_time
     if elapsed_time < SETTINGS['request_time_sleep']:
         time.sleep(SETTINGS['request_time_sleep'] - elapsed_time)
     return data
 
 def _next(arg_dict : dict, arg_list : list):
     """
```

### Comparing `pyneople-0.2.3/src/pyneople.egg-info/PKG-INFO` & `pyneople-0.2.4/src/pyneople.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneople
-Version: 0.2.3
+Version: 0.2.4
 Summary: Neople Open API wrapper for data analyst
 Home-page: https://github.com/ippo252525/pyneople
 Author: ippo252525
 Author-email: ippo252525@gmail.com
 Project-URL: Bug Tracker, https://github.com/ippo252525/pyneople/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

