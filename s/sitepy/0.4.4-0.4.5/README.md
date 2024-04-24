# Comparing `tmp/sitepy-0.4.4.tar.gz` & `tmp/sitepy-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitepy-0.4.4.tar", last modified: Wed Apr 24 15:22:29 2024, max compression
+gzip compressed data, was "sitepy-0.4.5.tar", last modified: Wed Apr 24 15:26:56 2024, max compression
```

## Comparing `sitepy-0.4.4.tar` & `sitepy-0.4.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-24 15:22:29.206635 sitepy-0.4.4/
--rw-r--r--   0 lewis-family   (501) staff       (20)      554 2024-04-24 14:29:53.000000 sitepy-0.4.4/LICENSE
--rw-r--r--   0 lewis-family   (501) staff       (20)     2389 2024-04-24 15:22:29.205402 sitepy-0.4.4/PKG-INFO
--rw-r--r--   0 lewis-family   (501) staff       (20)      875 2024-04-24 14:30:00.000000 sitepy-0.4.4/README.md
--rw-r--r--   0 lewis-family   (501) staff       (20)       38 2024-04-24 15:22:29.206859 sitepy-0.4.4/setup.cfg
--rw-r--r--   0 lewis-family   (501) staff       (20)     1057 2024-04-24 15:22:17.000000 sitepy-0.4.4/setup.py
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-24 15:22:29.201726 sitepy-0.4.4/sitepy/
--rw-r--r--   0 lewis-family   (501) staff       (20)      103 2024-04-24 14:31:25.000000 sitepy-0.4.4/sitepy/__init__.py
--rw-r--r--   0 lewis-family   (501) staff       (20)    11621 2024-04-24 15:22:01.000000 sitepy-0.4.4/sitepy/core.py
--rw-r--r--   0 lewis-family   (501) staff       (20)      227 2024-04-24 14:30:00.000000 sitepy-0.4.4/sitepy/gpt.py
--rw-r--r--   0 lewis-family   (501) staff       (20)     2631 2024-04-24 14:30:00.000000 sitepy-0.4.4/sitepy/log.py
--rw-r--r--   0 lewis-family   (501) staff       (20)      332 2024-04-24 14:51:31.000000 sitepy-0.4.4/sitepy/profanity.py
--rw-r--r--   0 lewis-family   (501) staff       (20)      306 2024-04-24 14:30:00.000000 sitepy-0.4.4/sitepy/recaptcha.py
--rw-r--r--   0 lewis-family   (501) staff       (20)    26817 2024-04-24 14:37:08.000000 sitepy-0.4.4/sitepy/word_list.py
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-24 15:22:29.204589 sitepy-0.4.4/sitepy.egg-info/
--rw-r--r--   0 lewis-family   (501) staff       (20)     2389 2024-04-24 15:22:29.000000 sitepy-0.4.4/sitepy.egg-info/PKG-INFO
--rw-r--r--   0 lewis-family   (501) staff       (20)      268 2024-04-24 15:22:29.000000 sitepy-0.4.4/sitepy.egg-info/SOURCES.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-04-24 15:22:29.000000 sitepy-0.4.4/sitepy.egg-info/dependency_links.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)        7 2024-04-24 15:22:29.000000 sitepy-0.4.4/sitepy.egg-info/top_level.txt
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-24 15:26:56.249705 sitepy-0.4.5/
+-rw-r--r--   0 lewis-family   (501) staff       (20)      554 2024-04-24 14:29:53.000000 sitepy-0.4.5/LICENSE
+-rw-r--r--   0 lewis-family   (501) staff       (20)     2389 2024-04-24 15:26:56.248700 sitepy-0.4.5/PKG-INFO
+-rw-r--r--   0 lewis-family   (501) staff       (20)      875 2024-04-24 14:30:00.000000 sitepy-0.4.5/README.md
+-rw-r--r--   0 lewis-family   (501) staff       (20)       38 2024-04-24 15:26:56.249891 sitepy-0.4.5/setup.cfg
+-rw-r--r--   0 lewis-family   (501) staff       (20)     1057 2024-04-24 15:26:43.000000 sitepy-0.4.5/setup.py
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-24 15:26:56.245673 sitepy-0.4.5/sitepy/
+-rw-r--r--   0 lewis-family   (501) staff       (20)      103 2024-04-24 14:31:25.000000 sitepy-0.4.5/sitepy/__init__.py
+-rw-r--r--   0 lewis-family   (501) staff       (20)    11699 2024-04-24 15:26:35.000000 sitepy-0.4.5/sitepy/core.py
+-rw-r--r--   0 lewis-family   (501) staff       (20)      227 2024-04-24 14:30:00.000000 sitepy-0.4.5/sitepy/gpt.py
+-rw-r--r--   0 lewis-family   (501) staff       (20)     2631 2024-04-24 14:30:00.000000 sitepy-0.4.5/sitepy/log.py
+-rw-r--r--   0 lewis-family   (501) staff       (20)      332 2024-04-24 14:51:31.000000 sitepy-0.4.5/sitepy/profanity.py
+-rw-r--r--   0 lewis-family   (501) staff       (20)      306 2024-04-24 14:30:00.000000 sitepy-0.4.5/sitepy/recaptcha.py
+-rw-r--r--   0 lewis-family   (501) staff       (20)    26817 2024-04-24 14:37:08.000000 sitepy-0.4.5/sitepy/word_list.py
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-24 15:26:56.247960 sitepy-0.4.5/sitepy.egg-info/
+-rw-r--r--   0 lewis-family   (501) staff       (20)     2389 2024-04-24 15:26:56.000000 sitepy-0.4.5/sitepy.egg-info/PKG-INFO
+-rw-r--r--   0 lewis-family   (501) staff       (20)      268 2024-04-24 15:26:56.000000 sitepy-0.4.5/sitepy.egg-info/SOURCES.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-04-24 15:26:56.000000 sitepy-0.4.5/sitepy.egg-info/dependency_links.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)        7 2024-04-24 15:26:56.000000 sitepy-0.4.5/sitepy.egg-info/top_level.txt
```

### Comparing `sitepy-0.4.4/LICENSE` & `sitepy-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sitepy-0.4.4/PKG-INFO` & `sitepy-0.4.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitepy
-Version: 0.4.4
+Version: 0.4.5
 Summary: A simple web framework.
 Home-page: https://github.com/WolfTheDeveloper/sitepy
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 License: Copyright [2024] [WolfTheDev]
         
         Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `sitepy-0.4.4/README.md` & `sitepy-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `sitepy-0.4.4/setup.py` & `sitepy-0.4.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sitepy',
-    version='0.4.4',
+    version='0.4.5',
     description='A simple web framework.',
     author='WolfTheDev',
     author_email='wolfthedev@gmail.com',
     url='https://github.com/WolfTheDeveloper/sitepy',
     license=open('LICENSE').read(),
     packages=find_packages(),
     long_description=open('README.md').read(),
```

### Comparing `sitepy-0.4.4/sitepy/core.py` & `sitepy-0.4.5/sitepy/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -442,20 +442,20 @@
                     if self.custom_500_page
                     else f00.encode()
                 )
             ]
     
     def tojson(self, data):
         import json
-        response_body = json.dumps(data)
+        response_body = json.dumps(data).encode()  # encode the JSON string, not the function
         def response(start_response):
             status = "200 OK"
             headers = [("Content-type", "application/json")]
             start_response(status, headers)
-            return [response_body.encode()]
+            return [response_body]  # return the encoded JSON string
         return response
 
     def run(self, host="localhost", port=8080):
         try:
             server = make_server(host, port, self)
             print(f"Serving on {host}:{port}")
             server.serve_forever()
```

### Comparing `sitepy-0.4.4/sitepy/log.py` & `sitepy-0.4.5/sitepy/log.py`

 * *Files identical despite different names*

### Comparing `sitepy-0.4.4/sitepy/word_list.py` & `sitepy-0.4.5/sitepy/word_list.py`

 * *Files identical despite different names*

### Comparing `sitepy-0.4.4/sitepy.egg-info/PKG-INFO` & `sitepy-0.4.5/sitepy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitepy
-Version: 0.4.4
+Version: 0.4.5
 Summary: A simple web framework.
 Home-page: https://github.com/WolfTheDeveloper/sitepy
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 License: Copyright [2024] [WolfTheDev]
         
         Licensed under the Apache License, Version 2.0 (the "License");
```

