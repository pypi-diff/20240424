# Comparing `tmp/buttercms-python-1.3.tar.gz` & `tmp/buttercms-python-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/buttercms-python-1.3.tar", last modified: Wed Sep  1 14:32:16 2021, max compression
+gzip compressed data, was "buttercms-python-2.0.tar", last modified: Wed Apr 24 17:13:36 2024, max compression
```

## Comparing `buttercms-python-1.3.tar` & `buttercms-python-2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jakelumetta   (501) staff       (20)        0 2021-09-01 14:32:16.626218 buttercms-python-1.3/
--rw-r--r--   0 jakelumetta   (501) staff       (20)     1076 2020-04-16 17:30:21.000000 buttercms-python-1.3/LICENSE
--rw-r--r--   0 jakelumetta   (501) staff       (20)       25 2020-04-16 17:30:21.000000 buttercms-python-1.3/MANIFEST.in
--rw-r--r--   0 jakelumetta   (501) staff       (20)     6608 2021-09-01 14:32:16.626316 buttercms-python-1.3/PKG-INFO
--rw-r--r--   0 jakelumetta   (501) staff       (20)     4135 2021-09-01 13:37:24.000000 buttercms-python-1.3/README.md
-drwxr-xr-x   0 jakelumetta   (501) staff       (20)        0 2021-09-01 14:32:16.625480 buttercms-python-1.3/butter_cms/
--rw-r--r--   0 jakelumetta   (501) staff       (20)      565 2020-04-16 17:30:21.000000 buttercms-python-1.3/butter_cms/__init__.py
--rw-r--r--   0 jakelumetta   (501) staff       (20)       20 2021-09-01 13:37:24.000000 buttercms-python-1.3/butter_cms/__version__.py
--rw-r--r--   0 jakelumetta   (501) staff       (20)      253 2020-04-16 17:30:21.000000 buttercms-python-1.3/butter_cms/author.py
--rw-r--r--   0 jakelumetta   (501) staff       (20)      260 2020-04-16 17:30:21.000000 buttercms-python-1.3/butter_cms/category.py
--rw-r--r--   0 jakelumetta   (501) staff       (20)      922 2020-04-16 17:34:03.000000 buttercms-python-1.3/butter_cms/client.py
--rw-r--r--   0 jakelumetta   (501) staff       (20)      363 2020-04-16 17:30:21.000000 buttercms-python-1.3/butter_cms/content_field.py
--rw-r--r--   0 jakelumetta   (501) staff       (20)      171 2020-04-16 17:30:21.000000 buttercms-python-1.3/butter_cms/feed.py
--rw-r--r--   0 jakelumetta   (501) staff       (20)      754 2021-09-01 13:37:24.000000 buttercms-python-1.3/butter_cms/page.py
--rw-r--r--   0 jakelumetta   (501) staff       (20)      620 2021-09-01 13:37:24.000000 buttercms-python-1.3/butter_cms/post.py
--rw-r--r--   0 jakelumetta   (501) staff       (20)      244 2020-04-16 17:30:21.000000 buttercms-python-1.3/butter_cms/tag.py
--rw-r--r--   0 jakelumetta   (501) staff       (20)     4738 2021-09-01 13:37:24.000000 buttercms-python-1.3/butter_cms/unit_tests.py
-drwxr-xr-x   0 jakelumetta   (501) staff       (20)        0 2021-09-01 14:32:16.626112 buttercms-python-1.3/buttercms_python.egg-info/
--rw-r--r--   0 jakelumetta   (501) staff       (20)     6608 2021-09-01 14:32:16.000000 buttercms-python-1.3/buttercms_python.egg-info/PKG-INFO
--rw-r--r--   0 jakelumetta   (501) staff       (20)      489 2021-09-01 14:32:16.000000 buttercms-python-1.3/buttercms_python.egg-info/SOURCES.txt
--rw-r--r--   0 jakelumetta   (501) staff       (20)        1 2021-09-01 14:32:16.000000 buttercms-python-1.3/buttercms_python.egg-info/dependency_links.txt
--rw-r--r--   0 jakelumetta   (501) staff       (20)        9 2021-09-01 14:32:16.000000 buttercms-python-1.3/buttercms_python.egg-info/requires.txt
--rw-r--r--   0 jakelumetta   (501) staff       (20)       11 2021-09-01 14:32:16.000000 buttercms-python-1.3/buttercms_python.egg-info/top_level.txt
--rw-r--r--   0 jakelumetta   (501) staff       (20)       67 2021-09-01 14:32:16.626582 buttercms-python-1.3/setup.cfg
--rw-r--r--   0 jakelumetta   (501) staff       (20)     1683 2020-04-16 17:44:29.000000 buttercms-python-1.3/setup.py
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-04-24 17:13:36.310475 buttercms-python-2.0/
+-rw-rw-r--   0 maria     (1000) maria     (1000)     1076 2023-09-14 13:51:45.000000 buttercms-python-2.0/LICENSE
+-rw-rw-r--   0 maria     (1000) maria     (1000)       25 2023-09-14 13:51:45.000000 buttercms-python-2.0/MANIFEST.in
+-rw-r--r--   0 maria     (1000) maria     (1000)     4958 2024-04-24 17:13:36.310475 buttercms-python-2.0/PKG-INFO
+-rw-rw-r--   0 maria     (1000) maria     (1000)     4135 2023-09-14 13:51:45.000000 buttercms-python-2.0/README.md
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-04-24 17:13:36.306475 buttercms-python-2.0/butter_cms/
+-rw-rw-r--   0 maria     (1000) maria     (1000)      565 2023-09-14 13:51:45.000000 buttercms-python-2.0/butter_cms/__init__.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)       20 2023-09-14 13:51:45.000000 buttercms-python-2.0/butter_cms/__version__.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)      253 2023-09-14 13:51:45.000000 buttercms-python-2.0/butter_cms/author.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)      260 2023-09-14 13:51:45.000000 buttercms-python-2.0/butter_cms/category.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)     1425 2024-04-24 17:10:33.000000 buttercms-python-2.0/butter_cms/client.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)      363 2023-09-14 13:51:45.000000 buttercms-python-2.0/butter_cms/content_field.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)      171 2023-09-14 13:51:45.000000 buttercms-python-2.0/butter_cms/feed.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)      754 2023-09-14 13:51:45.000000 buttercms-python-2.0/butter_cms/page.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)      620 2023-09-14 13:51:45.000000 buttercms-python-2.0/butter_cms/post.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)      244 2023-09-14 13:51:45.000000 buttercms-python-2.0/butter_cms/tag.py
+-rw-rw-r--   0 maria     (1000) maria     (1000)     4738 2023-09-14 13:51:45.000000 buttercms-python-2.0/butter_cms/unit_tests.py
+drwxrwxr-x   0 maria     (1000) maria     (1000)        0 2024-04-24 17:13:36.310475 buttercms-python-2.0/buttercms_python.egg-info/
+-rw-r--r--   0 maria     (1000) maria     (1000)     4958 2024-04-24 17:13:36.000000 buttercms-python-2.0/buttercms_python.egg-info/PKG-INFO
+-rw-rw-r--   0 maria     (1000) maria     (1000)      489 2024-04-24 17:13:36.000000 buttercms-python-2.0/buttercms_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 maria     (1000) maria     (1000)        1 2024-04-24 17:13:36.000000 buttercms-python-2.0/buttercms_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 maria     (1000) maria     (1000)        9 2024-04-24 17:13:36.000000 buttercms-python-2.0/buttercms_python.egg-info/requires.txt
+-rw-rw-r--   0 maria     (1000) maria     (1000)       11 2024-04-24 17:13:36.000000 buttercms-python-2.0/buttercms_python.egg-info/top_level.txt
+-rw-rw-r--   0 maria     (1000) maria     (1000)       67 2024-04-24 17:13:36.310475 buttercms-python-2.0/setup.cfg
+-rw-rw-r--   0 maria     (1000) maria     (1000)     1866 2024-04-24 17:10:33.000000 buttercms-python-2.0/setup.py
```

### Comparing `buttercms-python-1.3/LICENSE` & `buttercms-python-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `buttercms-python-1.3/README.md` & `buttercms-python-2.0/README.md`

 * *Files identical despite different names*

### Comparing `buttercms-python-1.3/butter_cms/__init__.py` & `buttercms-python-2.0/butter_cms/__init__.py`

 * *Files identical despite different names*

### Comparing `buttercms-python-1.3/butter_cms/client.py` & `buttercms-python-2.0/butter_cms/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import requests
 
 from .__version__ import __version__
+from requests.exceptions import HTTPError
 
 
 class Client(object):
     """Client"""
     def __init__(self, auth_token):
         self.auth_token = auth_token
         self.url = 'https://api.buttercms.com/v2/'
@@ -22,16 +23,26 @@
         }
 
         if path_override:
             path = path_override
         else:
             path = self.path
 
-        response = requests.get(
-            url=self.url + path + str(slug),
-            params=payload,
-            headers=headers,
-        )
+        try:
+            response = requests.get(
+                url=self.url + path + str(slug),
+                params=payload,
+                headers=headers,
+                timeout=10,
+            )
+        except requests.exceptions.Timeout:
+            raise
+
+        # We are not using response.raise_for_status(), as it only raises errors for definite error codes; we want to raise errors for any status other than 200.  
+        # more info here: https://github.com/ButterCMS/buttercms-python/issues/5
+        if response.status_code != 200: 
+            raise HTTPError(response.status_code)
+
         return response.json()
 
     def get(self, slug='', params=None):
         return self.api_get(slug=slug, params=params)
```

### Comparing `buttercms-python-1.3/butter_cms/page.py` & `buttercms-python-2.0/butter_cms/page.py`

 * *Files identical despite different names*

### Comparing `buttercms-python-1.3/butter_cms/post.py` & `buttercms-python-2.0/butter_cms/post.py`

 * *Files identical despite different names*

### Comparing `buttercms-python-1.3/butter_cms/unit_tests.py` & `buttercms-python-2.0/butter_cms/unit_tests.py`

 * *Files identical despite different names*

### Comparing `buttercms-python-1.3/setup.py` & `buttercms-python-2.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import sys
-
-from butter_cms.__version__ import __version__
+import os
 
 try:
-    from setuptools import setup
+    from setuptools import setup, find_packages
 except ImportError:
     from distutils.core import setup
 
 with open('README.md', 'r') as f:
     readme = f.read()
 
 
@@ -18,19 +17,26 @@
         'Please take a few seconds to upgrade to Python 2.7.9 and try again.\n'
         'https://www.python.org/downloads/')
     # TODO: Add support for < Python 2.7.9
     # install_requires.append('requests[security]')
 else:
     install_requires.append('requests')
 
+package_root = os.path.abspath(os.path.dirname(__file__))
+version = {}
+
+with open(os.path.join(package_root, "butter_cms/__version__.py")) as fp:
+    exec(fp.read(), version)
+
+version = version["__version__"]
 
 setup(
     name = 'buttercms-python',
-    packages = ['butter_cms'],
-    version = __version__,
+    packages = find_packages(),
+    version = version,
     description = 'API First Blogging and CMS platform built for developers',
     long_description=readme,
     long_description_content_type="text/markdown",
     author = 'Adam Yala',
     author_email = 'adam@adamyala.com',
     url = 'https://github.com/buttercms/buttercms-python',
     download_url = 'https://github.com/buttercms/buttercms-python/tarball/0.1',
```

