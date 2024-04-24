# Comparing `tmp/syncari-sdk-1.3.8.tar.gz` & `tmp/syncari-sdk-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncari-sdk-1.3.8.tar", last modified: Mon Jul 10 03:33:59 2023, max compression
+gzip compressed data, was "syncari-sdk-1.3.9.tar", last modified: Tue Feb  6 16:37:53 2024, max compression
```

## Comparing `syncari-sdk-1.3.8.tar` & `syncari-sdk-1.3.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 blesson    (501) staff       (20)        0 2023-07-10 03:33:59.434896 syncari-sdk-1.3.8/
--rw-r--r--   0 blesson    (501) staff       (20)      338 2023-07-10 03:33:59.434789 syncari-sdk-1.3.8/PKG-INFO
--rw-r--r--   0 blesson    (501) staff       (20)       78 2023-05-04 22:58:58.000000 syncari-sdk-1.3.8/README.md
--rw-r--r--   0 blesson    (501) staff       (20)       38 2023-07-10 03:33:59.434934 syncari-sdk-1.3.8/setup.cfg
--rwxr-xr-x   0 blesson    (501) staff       (20)      562 2023-07-07 16:46:08.000000 syncari-sdk-1.3.8/setup.py
-drwxr-xr-x   0 blesson    (501) staff       (20)        0 2023-07-10 03:33:59.432085 syncari-sdk-1.3.8/syncari/
--rw-r--r--   0 blesson    (501) staff       (20)        0 2023-05-04 22:58:58.000000 syncari-sdk-1.3.8/syncari/__init__.py
--rw-r--r--   0 blesson    (501) staff       (20)      699 2023-05-04 22:58:58.000000 syncari-sdk-1.3.8/syncari/logger.py
-drwxr-xr-x   0 blesson    (501) staff       (20)        0 2023-07-10 03:33:59.432877 syncari-sdk-1.3.8/syncari/models/
--rw-r--r--   0 blesson    (501) staff       (20)       64 2023-05-04 22:58:58.000000 syncari-sdk-1.3.8/syncari/models/__init__.py
--rw-r--r--   0 blesson    (501) staff       (20)     3969 2023-07-07 15:56:51.000000 syncari-sdk-1.3.8/syncari/models/core.py
--rw-r--r--   0 blesson    (501) staff       (20)     2505 2023-05-04 22:58:58.000000 syncari-sdk-1.3.8/syncari/models/request.py
--rw-r--r--   0 blesson    (501) staff       (20)     2273 2023-05-04 22:58:58.000000 syncari-sdk-1.3.8/syncari/models/schema.py
-drwxr-xr-x   0 blesson    (501) staff       (20)        0 2023-07-10 03:33:59.433100 syncari-sdk-1.3.8/syncari/rest/
--rw-r--r--   0 blesson    (501) staff       (20)        0 2023-05-04 22:58:58.000000 syncari-sdk-1.3.8/syncari/rest/__init__.py
--rw-r--r--   0 blesson    (501) staff       (20)     3938 2023-06-15 14:32:04.000000 syncari-sdk-1.3.8/syncari/rest/client.py
-drwxr-xr-x   0 blesson    (501) staff       (20)        0 2023-07-10 03:33:59.433409 syncari-sdk-1.3.8/syncari/synapse/
--rw-r--r--   0 blesson    (501) staff       (20)        0 2023-05-04 22:58:58.000000 syncari-sdk-1.3.8/syncari/synapse/__init__.py
--rw-r--r--   0 blesson    (501) staff       (20)    10308 2023-05-04 22:58:58.000000 syncari-sdk-1.3.8/syncari/synapse/abstract_synapse.py
-drwxr-xr-x   0 blesson    (501) staff       (20)        0 2023-07-10 03:33:59.433970 syncari-sdk-1.3.8/syncari_sdk.egg-info/
--rw-r--r--   0 blesson    (501) staff       (20)      338 2023-07-10 03:33:59.000000 syncari-sdk-1.3.8/syncari_sdk.egg-info/PKG-INFO
--rw-r--r--   0 blesson    (501) staff       (20)      569 2023-07-10 03:33:59.000000 syncari-sdk-1.3.8/syncari_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 blesson    (501) staff       (20)        1 2023-07-10 03:33:59.000000 syncari-sdk-1.3.8/syncari_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 blesson    (501) staff       (20)       47 2023-07-10 03:33:59.000000 syncari-sdk-1.3.8/syncari_sdk.egg-info/requires.txt
--rw-r--r--   0 blesson    (501) staff       (20)       19 2023-07-10 03:33:59.000000 syncari-sdk-1.3.8/syncari_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 blesson    (501) staff       (20)        0 2023-07-10 03:33:59.434527 syncari-sdk-1.3.8/unit_tests/
--rw-r--r--   0 blesson    (501) staff       (20)        0 2023-05-04 22:58:58.000000 syncari-sdk-1.3.8/unit_tests/__init__.py
--rw-r--r--   0 blesson    (501) staff       (20)     7319 2023-05-04 22:58:58.000000 syncari-sdk-1.3.8/unit_tests/test_mock_synapse.py
--rw-r--r--   0 blesson    (501) staff       (20)     6299 2023-05-04 22:58:58.000000 syncari-sdk-1.3.8/unit_tests/test_response_validations.py
--rw-r--r--   0 blesson    (501) staff       (20)     2809 2023-06-15 14:32:04.000000 syncari-sdk-1.3.8/unit_tests/test_rest_client.py
+drwxr-xr-x   0 durga      (501) staff       (20)        0 2024-02-06 16:37:53.789598 syncari-sdk-1.3.9/
+-rw-r--r--   0 durga      (501) staff       (20)      406 2024-02-06 16:37:53.789420 syncari-sdk-1.3.9/PKG-INFO
+-rw-r--r--   0 durga      (501) staff       (20)       78 2024-02-06 16:27:15.000000 syncari-sdk-1.3.9/README.md
+-rw-r--r--   0 durga      (501) staff       (20)       38 2024-02-06 16:37:53.789642 syncari-sdk-1.3.9/setup.cfg
+-rwxr-xr-x   0 durga      (501) staff       (20)      562 2024-02-06 16:32:34.000000 syncari-sdk-1.3.9/setup.py
+drwxr-xr-x   0 durga      (501) staff       (20)        0 2024-02-06 16:37:53.785989 syncari-sdk-1.3.9/syncari/
+-rw-r--r--   0 durga      (501) staff       (20)        0 2024-02-06 16:27:15.000000 syncari-sdk-1.3.9/syncari/__init__.py
+-rw-r--r--   0 durga      (501) staff       (20)      699 2024-02-06 16:27:15.000000 syncari-sdk-1.3.9/syncari/logger.py
+drwxr-xr-x   0 durga      (501) staff       (20)        0 2024-02-06 16:37:53.787206 syncari-sdk-1.3.9/syncari/models/
+-rw-r--r--   0 durga      (501) staff       (20)       64 2024-02-06 16:27:15.000000 syncari-sdk-1.3.9/syncari/models/__init__.py
+-rw-r--r--   0 durga      (501) staff       (20)     3987 2024-02-06 16:32:34.000000 syncari-sdk-1.3.9/syncari/models/core.py
+-rw-r--r--   0 durga      (501) staff       (20)     2505 2024-02-06 16:27:15.000000 syncari-sdk-1.3.9/syncari/models/request.py
+-rw-r--r--   0 durga      (501) staff       (20)     2273 2024-02-06 16:27:15.000000 syncari-sdk-1.3.9/syncari/models/schema.py
+drwxr-xr-x   0 durga      (501) staff       (20)        0 2024-02-06 16:37:53.787426 syncari-sdk-1.3.9/syncari/rest/
+-rw-r--r--   0 durga      (501) staff       (20)        0 2024-02-06 16:27:15.000000 syncari-sdk-1.3.9/syncari/rest/__init__.py
+-rw-r--r--   0 durga      (501) staff       (20)     3938 2024-02-06 16:27:15.000000 syncari-sdk-1.3.9/syncari/rest/client.py
+drwxr-xr-x   0 durga      (501) staff       (20)        0 2024-02-06 16:37:53.787648 syncari-sdk-1.3.9/syncari/synapse/
+-rw-r--r--   0 durga      (501) staff       (20)        0 2024-02-06 16:27:15.000000 syncari-sdk-1.3.9/syncari/synapse/__init__.py
+-rw-r--r--   0 durga      (501) staff       (20)    10308 2024-02-06 16:27:15.000000 syncari-sdk-1.3.9/syncari/synapse/abstract_synapse.py
+drwxr-xr-x   0 durga      (501) staff       (20)        0 2024-02-06 16:37:53.789225 syncari-sdk-1.3.9/syncari_sdk.egg-info/
+-rw-r--r--   0 durga      (501) staff       (20)      406 2024-02-06 16:37:53.000000 syncari-sdk-1.3.9/syncari_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 durga      (501) staff       (20)      569 2024-02-06 16:37:53.000000 syncari-sdk-1.3.9/syncari_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 durga      (501) staff       (20)        1 2024-02-06 16:37:53.000000 syncari-sdk-1.3.9/syncari_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 durga      (501) staff       (20)       47 2024-02-06 16:37:53.000000 syncari-sdk-1.3.9/syncari_sdk.egg-info/requires.txt
+-rw-r--r--   0 durga      (501) staff       (20)       19 2024-02-06 16:37:53.000000 syncari-sdk-1.3.9/syncari_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 durga      (501) staff       (20)        0 2024-02-06 16:37:53.789042 syncari-sdk-1.3.9/unit_tests/
+-rw-r--r--   0 durga      (501) staff       (20)        0 2024-02-06 16:27:15.000000 syncari-sdk-1.3.9/unit_tests/__init__.py
+-rw-r--r--   0 durga      (501) staff       (20)     7319 2024-02-06 16:27:15.000000 syncari-sdk-1.3.9/unit_tests/test_mock_synapse.py
+-rw-r--r--   0 durga      (501) staff       (20)     6299 2024-02-06 16:27:15.000000 syncari-sdk-1.3.9/unit_tests/test_response_validations.py
+-rw-r--r--   0 durga      (501) staff       (20)     2809 2024-02-06 16:27:15.000000 syncari-sdk-1.3.9/unit_tests/test_rest_client.py
```

### Comparing `syncari-sdk-1.3.8/setup.py` & `syncari-sdk-1.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name='syncari-sdk',
-    version='1.3.8',
+    version='1.3.9',
     description='Syncari Synapse Development Kit',
     author='Syncari',
     author_email='dev@syncari.com',
     long_description=readme,
     long_description_content_type='text/markdown',
     license='TBD',
     packages=find_packages(exclude=('unittests')),
```

### Comparing `syncari-sdk-1.3.8/syncari/logger.py` & `syncari-sdk-1.3.9/syncari/logger.py`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.8/syncari/models/core.py` & `syncari-sdk-1.3.9/syncari/models/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
         Identifies all auth types
     """
     BASIC_TOKEN = 'UserPasswordToken'
     USER_PWD = 'UserPassword'
     API_KEY = 'ApiKey'
     OAUTH = 'Oauth'
     SIMPLE_OAUTH = 'SimpleOAuth'
+    NONE = 'None'
 
 class AuthField(BaseModel):
     """
         Represents an auth field.
     """
     name: str
     dataType: DataType = DataType.STRING
```

### Comparing `syncari-sdk-1.3.8/syncari/models/request.py` & `syncari-sdk-1.3.9/syncari/models/request.py`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.8/syncari/models/schema.py` & `syncari-sdk-1.3.9/syncari/models/schema.py`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.8/syncari/rest/client.py` & `syncari-sdk-1.3.9/syncari/rest/client.py`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.8/syncari/synapse/abstract_synapse.py` & `syncari-sdk-1.3.9/syncari/synapse/abstract_synapse.py`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.8/syncari_sdk.egg-info/SOURCES.txt` & `syncari-sdk-1.3.9/syncari_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.8/unit_tests/test_mock_synapse.py` & `syncari-sdk-1.3.9/unit_tests/test_mock_synapse.py`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.8/unit_tests/test_response_validations.py` & `syncari-sdk-1.3.9/unit_tests/test_response_validations.py`

 * *Files identical despite different names*

### Comparing `syncari-sdk-1.3.8/unit_tests/test_rest_client.py` & `syncari-sdk-1.3.9/unit_tests/test_rest_client.py`

 * *Files identical despite different names*

