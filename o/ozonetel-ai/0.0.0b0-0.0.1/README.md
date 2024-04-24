# Comparing `tmp/ozonetel-ai-0.0.0b0.tar.gz` & `tmp/ozonetel-ai-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ozonetel-ai-0.0.0b0.tar", last modified: Tue Apr 23 07:18:54 2024, max compression
+gzip compressed data, was "ozonetel-ai-0.0.1.tar", last modified: Wed Apr 24 07:17:28 2024, max compression
```

## Comparing `ozonetel-ai-0.0.0b0.tar` & `ozonetel-ai-0.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:18:54.298155 ozonetel-ai-0.0.0b0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-23 07:18:47.000000 ozonetel-ai-0.0.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-23 07:18:54.298155 ozonetel-ai-0.0.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-23 07:18:47.000000 ozonetel-ai-0.0.0b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:18:54.294155 ozonetel-ai-0.0.0b0/ozoneai/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-23 07:18:47.000000 ozonetel-ai-0.0.0b0/ozoneai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-23 07:18:47.000000 ozonetel-ai-0.0.0b0/ozoneai/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-23 07:18:47.000000 ozonetel-ai-0.0.0b0/ozoneai/embeder.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-23 07:18:47.000000 ozonetel-ai-0.0.0b0/ozoneai/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-23 07:18:47.000000 ozonetel-ai-0.0.0b0/ozoneai/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:18:54.298155 ozonetel-ai-0.0.0b0/ozonetel_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-23 07:18:54.000000 ozonetel-ai-0.0.0b0/ozonetel_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-23 07:18:54.000000 ozonetel-ai-0.0.0b0/ozonetel_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 07:18:54.000000 ozonetel-ai-0.0.0b0/ozonetel_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-23 07:18:54.000000 ozonetel-ai-0.0.0b0/ozonetel_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 07:18:54.000000 ozonetel-ai-0.0.0b0/ozonetel_ai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 07:18:54.298155 ozonetel-ai-0.0.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-23 07:18:47.000000 ozonetel-ai-0.0.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:17:28.727607 ozonetel-ai-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-24 07:15:51.000000 ozonetel-ai-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-24 07:17:28.727607 ozonetel-ai-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-24 07:15:51.000000 ozonetel-ai-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:17:28.727607 ozonetel-ai-0.0.1/ozoneai/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-24 07:15:51.000000 ozonetel-ai-0.0.1/ozoneai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-24 07:15:51.000000 ozonetel-ai-0.0.1/ozoneai/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-04-24 07:15:51.000000 ozonetel-ai-0.0.1/ozoneai/embeder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-24 07:15:51.000000 ozonetel-ai-0.0.1/ozoneai/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-24 07:15:51.000000 ozonetel-ai-0.0.1/ozoneai/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:17:28.727607 ozonetel-ai-0.0.1/ozonetel_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-24 07:17:28.000000 ozonetel-ai-0.0.1/ozonetel_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-24 07:17:28.000000 ozonetel-ai-0.0.1/ozonetel_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 07:17:28.000000 ozonetel-ai-0.0.1/ozonetel_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-24 07:17:28.000000 ozonetel-ai-0.0.1/ozonetel_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 07:17:28.000000 ozonetel-ai-0.0.1/ozonetel_ai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 07:17:28.727607 ozonetel-ai-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-24 07:15:51.000000 ozonetel-ai-0.0.1/setup.py
```

### Comparing `ozonetel-ai-0.0.0b0/LICENSE` & `ozonetel-ai-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ozonetel-ai-0.0.0b0/PKG-INFO` & `ozonetel-ai-0.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ozonetel-ai
-Version: 0.0.0b0
+Version: 0.0.1
 Summary: The Ozonetel AI Library is a powerful tool developed by Ozonetel Communications Pvt Ltd, designed to empower developers with state-of-the-art Artificial Intelligence capabilities. This library provides seamless integration of advanced AI models into your projects, allowing you to leverage the latest in AI technology to enhance your applications.
 Home-page: 
 Author: Biswajit Satapathy
 Author-email: biswajit@ozonetel.com
 License: MIT License
 Keywords: Machine Learning,Artificial Intellegence,Neural Network,Indexing,Searching
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ozonetel-ai-0.0.0b0/ozoneai/connector.py` & `ozonetel-ai-0.0.1/ozoneai/connector.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from requests.compat import urljoin
 
 from .exception import AuthenticationError
 
 class EmbeddingEndpoints:
     baseurl = "https://speech-kws.ozonetel.com"
     root = urljoin(baseurl, "embeddings/")
-    get_embedding = urljoin(root, "text/get_embeddings/")
+    get_embedding = urljoin(root, "text/embedding/get/")
+    quantize = urljoin(root, "text/embedding/quantize/")
     url_details = parse_url(baseurl)
     max_retries = 3
     backoff_factor = 0.3
 
 # Embedder Client
 class EmbeddingConnector(object):
     """Ozone Embedder Client Application"""
```

### Comparing `ozonetel-ai-0.0.0b0/ozonetel_ai.egg-info/PKG-INFO` & `ozonetel-ai-0.0.1/ozonetel_ai.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ozonetel-ai
-Version: 0.0.0b0
+Version: 0.0.1
 Summary: The Ozonetel AI Library is a powerful tool developed by Ozonetel Communications Pvt Ltd, designed to empower developers with state-of-the-art Artificial Intelligence capabilities. This library provides seamless integration of advanced AI models into your projects, allowing you to leverage the latest in AI technology to enhance your applications.
 Home-page: 
 Author: Biswajit Satapathy
 Author-email: biswajit@ozonetel.com
 License: MIT License
 Keywords: Machine Learning,Artificial Intellegence,Neural Network,Indexing,Searching
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ozonetel-ai-0.0.0b0/setup.py` & `ozonetel-ai-0.0.1/setup.py`

 * *Files identical despite different names*

