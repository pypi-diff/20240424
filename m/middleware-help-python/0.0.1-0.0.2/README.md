# Comparing `tmp/middleware-help-python-0.0.1.tar.gz` & `tmp/middleware-help-python-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "middleware-help-python-0.0.1.tar", last modified: Wed Apr 24 08:01:14 2024, max compression
+gzip compressed data, was "middleware-help-python-0.0.2.tar", last modified: Wed Apr 24 08:22:00 2024, max compression
```

## Comparing `middleware-help-python-0.0.1.tar` & `middleware-help-python-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 08:01:14.721090 middleware-help-python-0.0.1/
--rw-rw-rw-   0        0        0    11558 2024-04-24 07:47:20.000000 middleware-help-python-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      513 2024-04-24 08:01:14.719097 middleware-help-python-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       24 2024-04-24 07:47:20.000000 middleware-help-python-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 08:01:14.717101 middleware-help-python-0.0.1/middleware_help_python.egg-info/
--rw-rw-rw-   0        0        0      513 2024-04-24 08:01:14.000000 middleware-help-python-0.0.1/middleware_help_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2024-04-24 08:01:14.000000 middleware-help-python-0.0.1/middleware_help_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 08:01:14.000000 middleware-help-python-0.0.1/middleware_help_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-04-24 08:01:14.000000 middleware-help-python-0.0.1/middleware_help_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-24 08:01:14.000000 middleware-help-python-0.0.1/middleware_help_python.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-24 08:01:14.714109 middleware-help-python-0.0.1/middleware_helper/
--rw-rw-rw-   0        0        0      480 2024-04-24 07:50:59.000000 middleware-help-python-0.0.1/middleware_helper/__init__.py
--rw-rw-rw-   0        0        0     3289 2024-04-24 07:57:37.000000 middleware-help-python-0.0.1/middleware_helper/mysql.py
--rw-rw-rw-   0        0        0     1000 2024-04-24 07:56:34.000000 middleware-help-python-0.0.1/middleware_helper/redis.py
--rw-rw-rw-   0        0        0       42 2024-04-24 08:01:14.721090 middleware-help-python-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1136 2024-04-24 07:59:45.000000 middleware-help-python-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 08:22:00.548479 middleware-help-python-0.0.2/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 07:47:20.000000 middleware-help-python-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      513 2024-04-24 08:22:00.546485 middleware-help-python-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2024-04-24 07:47:20.000000 middleware-help-python-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 08:22:00.545511 middleware-help-python-0.0.2/middleware_help_python.egg-info/
+-rw-rw-rw-   0        0        0      513 2024-04-24 08:22:00.000000 middleware-help-python-0.0.2/middleware_help_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2024-04-24 08:22:00.000000 middleware-help-python-0.0.2/middleware_help_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 08:22:00.000000 middleware-help-python-0.0.2/middleware_help_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-04-24 08:22:00.000000 middleware-help-python-0.0.2/middleware_help_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-24 08:22:00.000000 middleware-help-python-0.0.2/middleware_help_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 08:22:00.543493 middleware-help-python-0.0.2/middleware_helper/
+-rw-rw-rw-   0        0        0      480 2024-04-24 07:50:59.000000 middleware-help-python-0.0.2/middleware_helper/__init__.py
+-rw-rw-rw-   0        0        0     3289 2024-04-24 07:57:37.000000 middleware-help-python-0.0.2/middleware_helper/mysql.py
+-rw-rw-rw-   0        0        0     1036 2024-04-24 08:21:48.000000 middleware-help-python-0.0.2/middleware_helper/redis.py
+-rw-rw-rw-   0        0        0       42 2024-04-24 08:22:00.548479 middleware-help-python-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1136 2024-04-24 08:21:37.000000 middleware-help-python-0.0.2/setup.py
```

### Comparing `middleware-help-python-0.0.1/LICENSE` & `middleware-help-python-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `middleware-help-python-0.0.1/PKG-INFO` & `middleware-help-python-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: middleware-help-python
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is my middleware help package
 Home-page: https://github.com/ckf10000/middleware-help-python
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `middleware-help-python-0.0.1/middleware_help_python.egg-info/PKG-INFO` & `middleware-help-python-0.0.2/middleware_help_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: middleware-help-python
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is my middleware help package
 Home-page: https://github.com/ckf10000/middleware-help-python
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `middleware-help-python-0.0.1/middleware_helper/mysql.py` & `middleware-help-python-0.0.2/middleware_helper/mysql.py`

 * *Files identical despite different names*

### Comparing `middleware-help-python-0.0.1/middleware_helper/redis.py` & `middleware-help-python-0.0.2/middleware_helper/redis.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,10 +18,10 @@
         password=redis_params_map.get("password"),
         port=redis_params_map.get("port"),
         db=redis_params_map.get("db"),
         max_connections=redis_params_map.get("max_connections")
     )
 
 
-def get_redis_connection() -> Redis:
+def get_redis_connection(**redis_params_map) -> Redis:
     # 使用连接池创建 Redis 客户端
-    return Redis(connection_pool=get_redis_pool())
+    return Redis(connection_pool=get_redis_pool(**redis_params_map))
```

### Comparing `middleware-help-python-0.0.1/setup.py` & `middleware-help-python-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='middleware-help-python',
-    version='0.0.1',
+    version='0.0.2',
     description='This is my middleware help package',
     long_description='This is my middleware help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/middleware-help-python',
     packages=find_packages(),
     install_requires=[
```

