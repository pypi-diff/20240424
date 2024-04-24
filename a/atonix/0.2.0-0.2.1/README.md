# Comparing `tmp/atonix-0.2.0.tar.gz` & `tmp/atonix-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atonix-0.2.0.tar", last modified: Wed Mar 27 17:25:36 2024, max compression
+gzip compressed data, was "atonix-0.2.1.tar", last modified: Wed Apr 24 17:01:37 2024, max compression
```

## Comparing `atonix-0.2.0.tar` & `atonix-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 17:25:36.517278 atonix-0.2.0/
--rw-rw-rw-   0        0        0     1088 2024-02-20 23:06:22.000000 atonix-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      655 2024-03-27 17:25:36.517278 atonix-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-02-20 23:06:22.000000 atonix-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-27 17:25:36.494547 atonix-0.2.0/atonix/
--rw-rw-rw-   0        0        0      123 2024-03-27 17:22:16.000000 atonix-0.2.0/atonix/__init__.py
--rw-rw-rw-   0        0        0     4099 2024-03-26 22:07:21.000000 atonix-0.2.0/atonix/actions.py
--rw-rw-rw-   0        0        0     1144 2024-03-27 17:20:23.000000 atonix-0.2.0/atonix/api.py
--rw-rw-rw-   0        0        0     1197 2024-03-27 17:20:23.000000 atonix-0.2.0/atonix/api_india.py
--rw-rw-rw-   0        0        0     4773 2024-03-27 16:57:34.000000 atonix-0.2.0/atonix/assets.py
--rw-rw-rw-   0        0        0     5698 2024-03-26 22:07:21.000000 atonix-0.2.0/atonix/auth_helper.py
--rw-rw-rw-   0        0        0     6293 2024-03-26 22:07:21.000000 atonix-0.2.0/atonix/issues.py
--rw-rw-rw-   0        0        0     6344 2024-03-26 22:07:21.000000 atonix-0.2.0/atonix/models.py
--rw-rw-rw-   0        0        0    16339 2024-03-26 22:07:21.000000 atonix-0.2.0/atonix/processdata.py
-drwxrwxrwx   0        0        0        0 2024-03-27 17:25:36.517278 atonix-0.2.0/atonix.egg-info/
--rw-rw-rw-   0        0        0      655 2024-03-27 17:25:36.000000 atonix-0.2.0/atonix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2024-03-27 17:25:36.000000 atonix-0.2.0/atonix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 17:25:36.000000 atonix-0.2.0/atonix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-03-27 17:25:36.000000 atonix-0.2.0/atonix.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      624 2024-03-27 17:22:16.000000 atonix-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-27 17:25:36.517278 atonix-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      568 2024-03-27 17:22:16.000000 atonix-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 17:01:37.244682 atonix-0.2.1/
+-rw-rw-rw-   0        0        0     1088 2024-04-02 20:28:32.000000 atonix-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      655 2024-04-24 17:01:37.244682 atonix-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-02 20:28:32.000000 atonix-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 17:01:37.218922 atonix-0.2.1/atonix/
+-rw-rw-rw-   0        0        0      123 2024-04-24 16:55:29.000000 atonix-0.2.1/atonix/__init__.py
+-rw-rw-rw-   0        0        0     4101 2024-04-24 16:46:39.000000 atonix-0.2.1/atonix/actions.py
+-rw-rw-rw-   0        0        0     1144 2024-04-02 20:28:32.000000 atonix-0.2.1/atonix/api.py
+-rw-rw-rw-   0        0        0     1197 2024-04-24 16:50:51.000000 atonix-0.2.1/atonix/api_india.py
+-rw-rw-rw-   0        0        0     4773 2024-04-24 16:50:51.000000 atonix-0.2.1/atonix/assets.py
+-rw-rw-rw-   0        0        0     5698 2024-04-02 20:28:32.000000 atonix-0.2.1/atonix/auth_helper.py
+-rw-rw-rw-   0        0        0     6293 2024-04-24 16:50:51.000000 atonix-0.2.1/atonix/issues.py
+-rw-rw-rw-   0        0        0     6344 2024-04-24 16:50:51.000000 atonix-0.2.1/atonix/models.py
+-rw-rw-rw-   0        0        0    16339 2024-04-24 16:50:51.000000 atonix-0.2.1/atonix/processdata.py
+drwxrwxrwx   0        0        0        0 2024-04-24 17:01:37.244682 atonix-0.2.1/atonix.egg-info/
+-rw-rw-rw-   0        0        0      655 2024-04-24 17:01:37.000000 atonix-0.2.1/atonix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2024-04-24 17:01:37.000000 atonix-0.2.1/atonix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 17:01:37.000000 atonix-0.2.1/atonix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-24 17:01:37.000000 atonix-0.2.1/atonix.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      624 2024-04-24 16:55:29.000000 atonix-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-24 17:01:37.260450 atonix-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      568 2024-04-24 16:55:29.000000 atonix-0.2.1/setup.py
```

### Comparing `atonix-0.2.0/LICENSE` & `atonix-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atonix-0.2.0/PKG-INFO` & `atonix-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atonix
-Version: 0.2.0
+Version: 0.2.1
 Summary: A user friendly client to retrieve data from the AtonixOI system.
 Author: Kolton Stimpert
 Author-email: Kolton Stimpert <stimpertk@bv.com>
 Project-URL: Homepage, https://github.com/kstimp/atonix
 Project-URL: Bug Tracker, https://github.com/kstimp/atonix/issues
 Platform: Python 3.8
 Platform: Python 3.9
```

### Comparing `atonix-0.2.0/atonix/actions.py` & `atonix-0.2.1/atonix/actions.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             query_params = {'skip': skip,
                             'take': 500,
                             'changedAfter': changedAfter}
             if skip != 0:
                 time.sleep(0.21)
             response = handle_atx_request(
                 self.base_url,
-                self.api_key,
+                self.user_key,
                 self.private_key,
                 resource,
                 http_method,
                 query_params,
                 request_body,
                 headers)
 
@@ -99,15 +99,15 @@
                             'skip': skip,
                             'take': 500,
                             }
             if skip != 0:
                 time.sleep(0.21)
             response = handle_atx_request(
                 self.base_url,
-                self.api_key,
+                self.user_key,
                 self.private_key,
                 resource,
                 http_method,
                 query_params,
                 request_body,
                 headers)
```

### Comparing `atonix-0.2.0/atonix/api.py` & `atonix-0.2.1/atonix/api.py`

 * *Files identical despite different names*

### Comparing `atonix-0.2.0/atonix/api_india.py` & `atonix-0.2.1/atonix/api_india.py`

 * *Files identical despite different names*

### Comparing `atonix-0.2.0/atonix/assets.py` & `atonix-0.2.1/atonix/assets.py`

 * *Files identical despite different names*

### Comparing `atonix-0.2.0/atonix/auth_helper.py` & `atonix-0.2.1/atonix/auth_helper.py`

 * *Files identical despite different names*

### Comparing `atonix-0.2.0/atonix/issues.py` & `atonix-0.2.1/atonix/issues.py`

 * *Files identical despite different names*

### Comparing `atonix-0.2.0/atonix/models.py` & `atonix-0.2.1/atonix/models.py`

 * *Files identical despite different names*

### Comparing `atonix-0.2.0/atonix/processdata.py` & `atonix-0.2.1/atonix/processdata.py`

 * *Files identical despite different names*

### Comparing `atonix-0.2.0/atonix.egg-info/PKG-INFO` & `atonix-0.2.1/atonix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atonix
-Version: 0.2.0
+Version: 0.2.1
 Summary: A user friendly client to retrieve data from the AtonixOI system.
 Author: Kolton Stimpert
 Author-email: Kolton Stimpert <stimpertk@bv.com>
 Project-URL: Homepage, https://github.com/kstimp/atonix
 Project-URL: Bug Tracker, https://github.com/kstimp/atonix/issues
 Platform: Python 3.8
 Platform: Python 3.9
```

### Comparing `atonix-0.2.0/pyproject.toml` & `atonix-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=66.1.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "atonix"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Kolton Stimpert", email="stimpertk@bv.com" },
 ]
 description = "A user friendly client to retrieve data from the AtonixOI system."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `atonix-0.2.0/setup.py` & `atonix-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
   name='atonix',
-  version='0.2.0',
+  version='0.2.1',
   author='Kolton Stimpert',
   author_email='stimpertk@bv.com',
   description='A package, providing an easy to use interface for the AtonixOI web APIs.',
   platforms=['Python 3.8', 'Python 3.9', 'Python 3.10', 'Python 3.11'],
   packages=['atonix'],
   install_requires=['cryptography>=42.0.0',
                     'setuptools>=66.1.1',
```

