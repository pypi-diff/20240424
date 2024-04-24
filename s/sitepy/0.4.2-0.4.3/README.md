# Comparing `tmp/sitepy-0.4.2.tar.gz` & `tmp/sitepy-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitepy-0.4.2.tar", last modified: Wed Apr 24 14:52:31 2024, max compression
+gzip compressed data, was "sitepy-0.4.3.tar", last modified: Wed Apr 24 15:04:25 2024, max compression
```

## Comparing `sitepy-0.4.2.tar` & `sitepy-0.4.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-24 14:52:31.102659 sitepy-0.4.2/
--rw-r--r--   0 lewis-family   (501) staff       (20)      554 2024-04-24 14:29:53.000000 sitepy-0.4.2/LICENSE
--rw-r--r--   0 lewis-family   (501) staff       (20)     2389 2024-04-24 14:52:31.101019 sitepy-0.4.2/PKG-INFO
--rw-r--r--   0 lewis-family   (501) staff       (20)      875 2024-04-24 14:30:00.000000 sitepy-0.4.2/README.md
--rw-r--r--   0 lewis-family   (501) staff       (20)       38 2024-04-24 14:52:31.102975 sitepy-0.4.2/setup.cfg
--rw-r--r--   0 lewis-family   (501) staff       (20)     1057 2024-04-24 14:51:27.000000 sitepy-0.4.2/setup.py
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-24 14:52:31.096821 sitepy-0.4.2/sitepy/
--rw-r--r--   0 lewis-family   (501) staff       (20)      103 2024-04-24 14:31:25.000000 sitepy-0.4.2/sitepy/__init__.py
--rw-r--r--   0 lewis-family   (501) staff       (20)    11709 2024-04-24 14:30:00.000000 sitepy-0.4.2/sitepy/core.py
--rw-r--r--   0 lewis-family   (501) staff       (20)      227 2024-04-24 14:30:00.000000 sitepy-0.4.2/sitepy/gpt.py
--rw-r--r--   0 lewis-family   (501) staff       (20)     2631 2024-04-24 14:30:00.000000 sitepy-0.4.2/sitepy/log.py
--rw-r--r--   0 lewis-family   (501) staff       (20)      332 2024-04-24 14:51:31.000000 sitepy-0.4.2/sitepy/profanity.py
--rw-r--r--   0 lewis-family   (501) staff       (20)      306 2024-04-24 14:30:00.000000 sitepy-0.4.2/sitepy/recaptcha.py
--rw-r--r--   0 lewis-family   (501) staff       (20)    26817 2024-04-24 14:37:08.000000 sitepy-0.4.2/sitepy/word_list.py
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-24 14:52:31.099895 sitepy-0.4.2/sitepy.egg-info/
--rw-r--r--   0 lewis-family   (501) staff       (20)     2389 2024-04-24 14:52:30.000000 sitepy-0.4.2/sitepy.egg-info/PKG-INFO
--rw-r--r--   0 lewis-family   (501) staff       (20)      268 2024-04-24 14:52:31.000000 sitepy-0.4.2/sitepy.egg-info/SOURCES.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-04-24 14:52:30.000000 sitepy-0.4.2/sitepy.egg-info/dependency_links.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)        7 2024-04-24 14:52:30.000000 sitepy-0.4.2/sitepy.egg-info/top_level.txt
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-24 15:04:25.568878 sitepy-0.4.3/
+-rw-r--r--   0 lewis-family   (501) staff       (20)      554 2024-04-24 14:29:53.000000 sitepy-0.4.3/LICENSE
+-rw-r--r--   0 lewis-family   (501) staff       (20)     2389 2024-04-24 15:04:25.567279 sitepy-0.4.3/PKG-INFO
+-rw-r--r--   0 lewis-family   (501) staff       (20)      875 2024-04-24 14:30:00.000000 sitepy-0.4.3/README.md
+-rw-r--r--   0 lewis-family   (501) staff       (20)       38 2024-04-24 15:04:25.569139 sitepy-0.4.3/setup.cfg
+-rw-r--r--   0 lewis-family   (501) staff       (20)     1057 2024-04-24 15:04:12.000000 sitepy-0.4.3/setup.py
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-24 15:04:25.562107 sitepy-0.4.3/sitepy/
+-rw-r--r--   0 lewis-family   (501) staff       (20)      103 2024-04-24 14:31:25.000000 sitepy-0.4.3/sitepy/__init__.py
+-rw-r--r--   0 lewis-family   (501) staff       (20)    11628 2024-04-24 15:04:09.000000 sitepy-0.4.3/sitepy/core.py
+-rw-r--r--   0 lewis-family   (501) staff       (20)      227 2024-04-24 14:30:00.000000 sitepy-0.4.3/sitepy/gpt.py
+-rw-r--r--   0 lewis-family   (501) staff       (20)     2631 2024-04-24 14:30:00.000000 sitepy-0.4.3/sitepy/log.py
+-rw-r--r--   0 lewis-family   (501) staff       (20)      332 2024-04-24 14:51:31.000000 sitepy-0.4.3/sitepy/profanity.py
+-rw-r--r--   0 lewis-family   (501) staff       (20)      306 2024-04-24 14:30:00.000000 sitepy-0.4.3/sitepy/recaptcha.py
+-rw-r--r--   0 lewis-family   (501) staff       (20)    26817 2024-04-24 14:37:08.000000 sitepy-0.4.3/sitepy/word_list.py
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-24 15:04:25.566190 sitepy-0.4.3/sitepy.egg-info/
+-rw-r--r--   0 lewis-family   (501) staff       (20)     2389 2024-04-24 15:04:25.000000 sitepy-0.4.3/sitepy.egg-info/PKG-INFO
+-rw-r--r--   0 lewis-family   (501) staff       (20)      268 2024-04-24 15:04:25.000000 sitepy-0.4.3/sitepy.egg-info/SOURCES.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-04-24 15:04:25.000000 sitepy-0.4.3/sitepy.egg-info/dependency_links.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)        7 2024-04-24 15:04:25.000000 sitepy-0.4.3/sitepy.egg-info/top_level.txt
```

### Comparing `sitepy-0.4.2/LICENSE` & `sitepy-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sitepy-0.4.2/PKG-INFO` & `sitepy-0.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitepy
-Version: 0.4.2
+Version: 0.4.3
 Summary: A simple web framework.
 Home-page: https://github.com/WolfTheDeveloper/sitepy
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 License: Copyright [2024] [WolfTheDev]
         
         Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `sitepy-0.4.2/README.md` & `sitepy-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `sitepy-0.4.2/setup.py` & `sitepy-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sitepy',
-    version='0.4.2',
+    version='0.4.3',
     description='A simple web framework.',
     author='WolfTheDev',
     author_email='wolfthedev@gmail.com',
     url='https://github.com/WolfTheDeveloper/sitepy',
     license=open('LICENSE').read(),
     packages=find_packages(),
     long_description=open('README.md').read(),
```

### Comparing `sitepy-0.4.2/sitepy/core.py` & `sitepy-0.4.3/sitepy/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,18 +377,16 @@
         try:
             path = environ["PATH_INFO"]
             method = environ["REQUEST_METHOD"]
             for middleware in self.middleware:
                 middleware(environ)
             handler = None
             for route, methods in self.routes.keys():
-                match = route.match(path)
-                if match and method in methods:
+                if route == path and method in methods:
                     handler = self.routes[(route, methods)]
-                    params = match.groupdict()
                     break
             if handler:
                 try:
                     request_body_size = int(environ.get("CONTENT_LENGTH", 0))
                 except ValueError:
                     request_body_size = 0
                 request_body = environ["wsgi.input"].read(request_body_size)
```

### Comparing `sitepy-0.4.2/sitepy/log.py` & `sitepy-0.4.3/sitepy/log.py`

 * *Files identical despite different names*

### Comparing `sitepy-0.4.2/sitepy/word_list.py` & `sitepy-0.4.3/sitepy/word_list.py`

 * *Files identical despite different names*

### Comparing `sitepy-0.4.2/sitepy.egg-info/PKG-INFO` & `sitepy-0.4.3/sitepy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitepy
-Version: 0.4.2
+Version: 0.4.3
 Summary: A simple web framework.
 Home-page: https://github.com/WolfTheDeveloper/sitepy
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 License: Copyright [2024] [WolfTheDev]
         
         Licensed under the Apache License, Version 2.0 (the "License");
```

