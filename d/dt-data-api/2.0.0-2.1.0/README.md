# Comparing `tmp/dt-data-api-2.0.0.tar.gz` & `tmp/dt-data-api-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dt-data-api-2.0.0.tar", last modified: Wed Nov  1 22:41:48 2023, max compression
+gzip compressed data, was "dt-data-api-2.1.0.tar", last modified: Wed Apr 24 15:59:06 2024, max compression
```

## Comparing `dt-data-api-2.0.0.tar` & `dt-data-api-2.1.0.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-11-01 22:41:48.209187 dt-data-api-2.0.0/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      415 2023-11-01 22:41:48.209187 dt-data-api-2.0.0/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-11-01 22:41:48.209187 dt-data-api-2.0.0/setup.cfg
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      408 2023-06-07 13:19:06.000000 dt-data-api-2.0.0/setup.json
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2132 2023-09-29 18:53:06.000000 dt-data-api-2.0.0/setup.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-11-01 22:41:48.201187 dt-data-api-2.0.0/src/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-11-01 22:41:48.205186 dt-data-api-2.0.0/src/dt_data_api/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      539 2023-11-01 22:41:17.000000 dt-data-api-2.0.0/src/dt_data_api/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2824 2023-05-30 04:43:20.000000 dt-data-api-2.0.0/src/dt_data_api/api.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1995 2023-04-19 19:49:18.000000 dt-data-api-2.0.0/src/dt_data_api/client.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      529 2023-06-07 13:21:51.000000 dt-data-api-2.0.0/src/dt_data_api/constants.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      519 2023-04-19 19:49:18.000000 dt-data-api-2.0.0/src/dt_data_api/exceptions.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1024 2023-06-07 13:19:06.000000 dt-data-api-2.0.0/src/dt_data_api/item.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      127 2023-05-30 04:42:56.000000 dt-data-api-2.0.0/src/dt_data_api/logging.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    20068 2023-06-07 13:19:06.000000 dt-data-api-2.0.0/src/dt_data_api/storage.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    15644 2023-06-07 13:19:06.000000 dt-data-api-2.0.0/src/dt_data_api/utils.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-11-01 22:41:48.209187 dt-data-api-2.0.0/src/dt_data_api.egg-info/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      415 2023-11-01 22:41:48.000000 dt-data-api-2.0.0/src/dt_data_api.egg-info/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      494 2023-11-01 22:41:48.000000 dt-data-api-2.0.0/src/dt_data_api.egg-info/SOURCES.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-11-01 22:41:48.000000 dt-data-api-2.0.0/src/dt_data_api.egg-info/dependency_links.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       20 2023-11-01 22:41:48.000000 dt-data-api-2.0.0/src/dt_data_api.egg-info/entry_points.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       47 2023-11-01 22:41:48.000000 dt-data-api-2.0.0/src/dt_data_api.egg-info/requires.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       30 2023-11-01 22:41:48.000000 dt-data-api-2.0.0/src/dt_data_api.egg-info/top_level.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-24 15:59:06.779595 dt-data-api-2.1.0/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      468 2024-04-24 15:59:06.779595 dt-data-api-2.1.0/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2024-04-24 15:59:06.779595 dt-data-api-2.1.0/setup.cfg
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      408 2023-03-22 21:05:02.000000 dt-data-api-2.1.0/setup.json
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2132 2024-04-24 15:58:47.000000 dt-data-api-2.1.0/setup.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-24 15:59:06.779595 dt-data-api-2.1.0/src/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-24 15:59:06.779595 dt-data-api-2.1.0/src/dt_data_api/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      539 2024-04-24 15:59:01.000000 dt-data-api-2.1.0/src/dt_data_api/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2917 2024-04-24 15:58:47.000000 dt-data-api-2.1.0/src/dt_data_api/api.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1995 2023-03-22 21:05:02.000000 dt-data-api-2.1.0/src/dt_data_api/client.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      529 2024-04-24 15:58:47.000000 dt-data-api-2.1.0/src/dt_data_api/constants.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      519 2023-03-22 21:05:02.000000 dt-data-api-2.1.0/src/dt_data_api/exceptions.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1024 2023-03-22 21:05:02.000000 dt-data-api-2.1.0/src/dt_data_api/item.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      127 2023-03-22 21:05:02.000000 dt-data-api-2.1.0/src/dt_data_api/logging.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    20068 2023-03-22 21:05:02.000000 dt-data-api-2.1.0/src/dt_data_api/storage.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    15644 2023-03-22 21:05:02.000000 dt-data-api-2.1.0/src/dt_data_api/utils.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2024-04-24 15:59:06.779595 dt-data-api-2.1.0/src/dt_data_api.egg-info/
+-rw-r--r--   0 afdaniele  (1000) afdaniele  (1000)      468 2024-04-24 15:59:06.000000 dt-data-api-2.1.0/src/dt_data_api.egg-info/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      452 2024-04-24 15:59:06.000000 dt-data-api-2.1.0/src/dt_data_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2024-04-24 15:59:06.000000 dt-data-api-2.1.0/src/dt_data_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       47 2024-04-24 15:59:06.000000 dt-data-api-2.1.0/src/dt_data_api.egg-info/requires.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       30 2024-04-24 15:59:06.000000 dt-data-api-2.1.0/src/dt_data_api.egg-info/top_level.txt
```

### Comparing `dt-data-api-2.0.0/setup.py` & `dt-data-api-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `dt-data-api-2.0.0/src/dt_data_api/__init__.py` & `dt-data-api-2.1.0/src/dt_data_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.0.0"
+__version__ = "2.1.0"
 
 from .logging import logger
 from .client import DataClient
 from .storage import Storage
 from .utils import TransferStatus, TransferProgress, TransferHandler
 from .exceptions import APIError, TransferError, ConfigurationError
 from .item import Item
```

### Comparing `dt-data-api-2.0.0/src/dt_data_api/api.py` & `dt-data-api-2.1.0/src/dt_data_api/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 from typing import Dict
 
 from dt_authentication import DuckietownToken
 from .constants import DATA_API_URL
 from .exceptions import APIError
 
+URL = str
+
 
 class DataAPI(object):
     """
     Provides an interface to the RESTful Data API service. The RESTful Data API service
     generates signed URLs that allow you to perform operations on files on the DCSS.
 
     You should not use this class yourself, the DataClient will do it for you.
@@ -35,18 +37,19 @@
         return self._uid
 
     @property
     def token(self) -> str:
         """The given token"""
         return self._token
 
-    def authorize_request(self, action: str, bucket: str, obj: str, headers: Dict[str, str] = None):
+    def authorize_request(self, action: str, bucket: str, obj: str, headers: Dict[str, str] = None) -> URL:
         """
         Authorizes the request to perform a given ``action`` on a given object ``obj``
-        in the storage space ``bucket``.
+        in the storage space ``bucket``. Returns the presigned URL (``str``) to use to perform
+        the request.
 
         Args:
             action (:obj:`str`):        Action to perform on the object. Allowed values are listed
                                         `here <https://docs.aws.amazon.com/AmazonS3/latest/API/
                                         API_Operations_Amazon_Simple_Storage_Service.html>`_.
 
             bucket (:obj:`str`):        Name of the target storage space (e.g., ``public``).
```

### Comparing `dt-data-api-2.0.0/src/dt_data_api/client.py` & `dt-data-api-2.1.0/src/dt_data_api/client.py`

 * *Files identical despite different names*

### Comparing `dt-data-api-2.0.0/src/dt_data_api/constants.py` & `dt-data-api-2.1.0/src/dt_data_api/constants.py`

 * *Files identical despite different names*

### Comparing `dt-data-api-2.0.0/src/dt_data_api/exceptions.py` & `dt-data-api-2.1.0/src/dt_data_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `dt-data-api-2.0.0/src/dt_data_api/item.py` & `dt-data-api-2.1.0/src/dt_data_api/item.py`

 * *Files identical despite different names*

### Comparing `dt-data-api-2.0.0/src/dt_data_api/storage.py` & `dt-data-api-2.1.0/src/dt_data_api/storage.py`

 * *Files identical despite different names*

### Comparing `dt-data-api-2.0.0/src/dt_data_api/utils.py` & `dt-data-api-2.1.0/src/dt_data_api/utils.py`

 * *Files identical despite different names*

