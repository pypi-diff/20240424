# Comparing `tmp/lazyad-0.0.8.tar.gz` & `tmp/lazyad-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyad-0.0.8.tar", last modified: Thu Apr 11 07:23:16 2024, max compression
+gzip compressed data, was "lazyad-0.0.9.tar", last modified: Thu Apr 11 09:06:09 2024, max compression
```

## Comparing `lazyad-0.0.8.tar` & `lazyad-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-11 07:23:16.775597 lazyad-0.0.8/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1693 2024-04-11 07:23:16.775420 lazyad-0.0.8/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1311 2024-03-14 02:37:12.000000 lazyad-0.0.8/README.md
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-11 07:23:16.773053 lazyad-0.0.8/lazyad/
--rw-r--r--   0 zeroseeker   (501) staff       (20)       41 2024-04-11 06:24:40.000000 lazyad-0.0.8/lazyad/__init__.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-11 07:23:16.774733 lazyad-0.0.8/lazyad/crawlers/
--rw-r--r--   0 zeroseeker   (501) staff       (20)       68 2024-03-19 07:34:32.000000 lazyad-0.0.8/lazyad/crawlers/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1482 2024-03-19 07:35:06.000000 lazyad-0.0.8/lazyad/crawlers/chuangliang.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     4540 2024-03-15 02:44:05.000000 lazyad-0.0.8/lazyad/crawlers/oceanengine.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     3060 2024-03-24 01:42:41.000000 lazyad-0.0.8/lazyad/crawlers/qq.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-11 07:23:16.775130 lazyad-0.0.8/lazyad/open/
--rw-r--r--   0 zeroseeker   (501) staff       (20)        0 2024-04-11 06:24:12.000000 lazyad-0.0.8/lazyad/open/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     2886 2024-04-11 07:22:45.000000 lazyad-0.0.8/lazyad/open/qq.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-11 07:23:16.773706 lazyad-0.0.8/lazyad.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1693 2024-04-11 07:23:16.000000 lazyad-0.0.8/lazyad.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      340 2024-04-11 07:23:16.000000 lazyad-0.0.8/lazyad.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2024-04-11 07:23:16.000000 lazyad-0.0.8/lazyad.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       16 2024-04-11 07:23:16.000000 lazyad-0.0.8/lazyad.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        7 2024-04-11 07:23:16.000000 lazyad-0.0.8/lazyad.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2024-04-11 07:23:16.775637 lazyad-0.0.8/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)      893 2024-04-11 07:22:45.000000 lazyad-0.0.8/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-11 09:06:09.640488 lazyad-0.0.9/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1693 2024-04-11 09:06:09.640298 lazyad-0.0.9/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1311 2024-03-14 02:37:12.000000 lazyad-0.0.9/README.md
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-11 09:06:09.637986 lazyad-0.0.9/lazyad/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       41 2024-04-11 06:24:40.000000 lazyad-0.0.9/lazyad/__init__.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-11 09:06:09.639657 lazyad-0.0.9/lazyad/crawlers/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       68 2024-03-19 07:34:32.000000 lazyad-0.0.9/lazyad/crawlers/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1482 2024-03-19 07:35:06.000000 lazyad-0.0.9/lazyad/crawlers/chuangliang.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     4540 2024-03-15 02:44:05.000000 lazyad-0.0.9/lazyad/crawlers/oceanengine.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     3060 2024-03-24 01:42:41.000000 lazyad-0.0.9/lazyad/crawlers/qq.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-11 09:06:09.639979 lazyad-0.0.9/lazyad/open/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        0 2024-04-11 06:24:12.000000 lazyad-0.0.9/lazyad/open/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     2895 2024-04-11 09:05:28.000000 lazyad-0.0.9/lazyad/open/qq.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-04-11 09:06:09.638697 lazyad-0.0.9/lazyad.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1693 2024-04-11 09:06:09.000000 lazyad-0.0.9/lazyad.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      340 2024-04-11 09:06:09.000000 lazyad-0.0.9/lazyad.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2024-04-11 09:06:09.000000 lazyad-0.0.9/lazyad.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       16 2024-04-11 09:06:09.000000 lazyad-0.0.9/lazyad.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        7 2024-04-11 09:06:09.000000 lazyad-0.0.9/lazyad.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2024-04-11 09:06:09.640543 lazyad-0.0.9/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      893 2024-04-11 09:05:52.000000 lazyad-0.0.9/setup.py
```

### Comparing `lazyad-0.0.8/PKG-INFO` & `lazyad-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyad
-Version: 0.0.8
+Version: 0.0.9
 Summary: 基于Python的懒人包-适用于广告投放模块
 Home-page: https://gitee.com/ZeroSeeker/lazyad
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `lazyad-0.0.8/README.md` & `lazyad-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `lazyad-0.0.8/lazyad/crawlers/chuangliang.py` & `lazyad-0.0.9/lazyad/crawlers/chuangliang.py`

 * *Files identical despite different names*

### Comparing `lazyad-0.0.8/lazyad/crawlers/oceanengine.py` & `lazyad-0.0.9/lazyad/crawlers/oceanengine.py`

 * *Files identical despite different names*

### Comparing `lazyad-0.0.8/lazyad/crawlers/qq.py` & `lazyad-0.0.9/lazyad/crawlers/qq.py`

 * *Files identical despite different names*

### Comparing `lazyad-0.0.8/lazyad/open/qq.py` & `lazyad-0.0.9/lazyad/open/qq.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     )
 
 
 def oauth_token3(
         access_token,
         app_id,
         app_secret,
-        redirect_uri,
+        redirect_uri=None,
         grant_type='authorization_code',
         auth_code=None,
         refresh_token=None,
 ):
     """
     获取/刷新token
     相关文档：https://developers.e.qq.com/v3.0/docs/api/oauth/token
@@ -79,15 +79,14 @@
     :param app_id:
     :param app_secret:
     :param grant_type: 请求的类型，可选值：authorization_code（授权码方式获取 token）、refresh_token（刷新 token）
     :param refresh_token:
     :param redirect_uri: 回调地址
     :return:
     """
-    redirect_uri = f'{redirect_uri}?app_id={app_id}'
     url = 'https://api.e.qq.com/v3.0/oauth/token'
     params = {
         'access_token': access_token,
         'timestamp': int(time.time()),
         'nonce': make_nonce,
 
         'client_id': app_id,
@@ -95,14 +94,15 @@
         'grant_type': grant_type
     }
     if auth_code:
         params['authorization_code'] = auth_code
     if refresh_token:
         params['refresh_token'] = refresh_token
     if redirect_uri:
+        redirect_uri = f'{redirect_uri}?app_id={app_id}'
         params['redirect_uri'] = redirect_uri
 
     for k in params:
         if type(params[k]) is not str:
             params[k] = json.dumps(params[k])
 
     return lazyrequests.lazy_requests(
```

### Comparing `lazyad-0.0.8/lazyad.egg-info/PKG-INFO` & `lazyad-0.0.9/lazyad.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazyad
-Version: 0.0.8
+Version: 0.0.9
 Summary: 基于Python的懒人包-适用于广告投放模块
 Home-page: https://gitee.com/ZeroSeeker/lazyad
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `lazyad-0.0.8/setup.py` & `lazyad-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lazyad",
-    version="0.0.8",
+    version="0.0.9",
     description="基于Python的懒人包-适用于广告投放模块",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
     url="https://gitee.com/ZeroSeeker/lazyad",
     packages=setuptools.find_packages(),
```

