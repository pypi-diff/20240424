# Comparing `tmp/netlify_dns_manager-0.1.tar.gz` & `tmp/netlify_dns_manager-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netlify_dns_manager-0.1.tar", last modified: Wed Apr 24 09:42:55 2024, max compression
+gzip compressed data, was "netlify_dns_manager-0.2.tar", last modified: Wed Apr 24 10:30:56 2024, max compression
```

## Comparing `netlify_dns_manager-0.1.tar` & `netlify_dns_manager-0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:42:55.711592 netlify_dns_manager-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-24 09:42:44.000000 netlify_dns_manager-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-24 09:42:55.711592 netlify_dns_manager-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-24 09:42:44.000000 netlify_dns_manager-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:42:55.707592 netlify_dns_manager-0.1/netlify_dns_manage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:42:44.000000 netlify_dns_manager-0.1/netlify_dns_manage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-24 09:42:44.000000 netlify_dns_manager-0.1/netlify_dns_manage/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-24 09:42:44.000000 netlify_dns_manager-0.1/netlify_dns_manage/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-24 09:42:44.000000 netlify_dns_manager-0.1/netlify_dns_manage/netlify_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-24 09:42:44.000000 netlify_dns_manager-0.1/netlify_dns_manage/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-24 09:42:44.000000 netlify_dns_manager-0.1/netlify_dns_manage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:42:55.711592 netlify_dns_manager-0.1/netlify_dns_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-24 09:42:55.000000 netlify_dns_manager-0.1/netlify_dns_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-24 09:42:55.000000 netlify_dns_manager-0.1/netlify_dns_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 09:42:55.000000 netlify_dns_manager-0.1/netlify_dns_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-24 09:42:55.000000 netlify_dns_manager-0.1/netlify_dns_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-24 09:42:55.000000 netlify_dns_manager-0.1/netlify_dns_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 09:42:55.000000 netlify_dns_manager-0.1/netlify_dns_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 09:42:55.711592 netlify_dns_manager-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-24 09:42:44.000000 netlify_dns_manager-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:42:55.711592 netlify_dns_manager-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:42:44.000000 netlify_dns_manager-0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:42:44.000000 netlify_dns_manager-0.1/tests/test_netlify_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:42:44.000000 netlify_dns_manager-0.1/tests/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:30:56.916249 netlify_dns_manager-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-24 10:30:44.000000 netlify_dns_manager-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-24 10:30:56.916249 netlify_dns_manager-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-24 10:30:44.000000 netlify_dns_manager-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:30:56.916249 netlify_dns_manager-0.2/netlify_dns_manage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:30:44.000000 netlify_dns_manager-0.2/netlify_dns_manage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-24 10:30:44.000000 netlify_dns_manager-0.2/netlify_dns_manage/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-24 10:30:44.000000 netlify_dns_manager-0.2/netlify_dns_manage/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-24 10:30:44.000000 netlify_dns_manager-0.2/netlify_dns_manage/netlify_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-24 10:30:44.000000 netlify_dns_manager-0.2/netlify_dns_manage/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-24 10:30:44.000000 netlify_dns_manager-0.2/netlify_dns_manage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:30:56.916249 netlify_dns_manager-0.2/netlify_dns_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-24 10:30:56.000000 netlify_dns_manager-0.2/netlify_dns_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-24 10:30:56.000000 netlify_dns_manager-0.2/netlify_dns_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:30:56.000000 netlify_dns_manager-0.2/netlify_dns_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-24 10:30:56.000000 netlify_dns_manager-0.2/netlify_dns_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-24 10:30:56.000000 netlify_dns_manager-0.2/netlify_dns_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 10:30:56.000000 netlify_dns_manager-0.2/netlify_dns_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 10:30:56.916249 netlify_dns_manager-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-24 10:30:44.000000 netlify_dns_manager-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:30:56.916249 netlify_dns_manager-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:30:44.000000 netlify_dns_manager-0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:30:44.000000 netlify_dns_manager-0.2/tests/test_netlify_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:30:44.000000 netlify_dns_manager-0.2/tests/test_parser.py
```

### Comparing `netlify_dns_manager-0.1/LICENSE` & `netlify_dns_manager-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `netlify_dns_manager-0.1/PKG-INFO` & `netlify_dns_manager-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netlify-dns-manager
-Version: 0.1
+Version: 0.2
 Summary: It provides a command line interface to manage DNS records of a domain hosted on Netlify.
 Home-page: https://github.com/sumansaurabh/netlify-dns-manager
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `netlify_dns_manager-0.1/README.md` & `netlify_dns_manager-0.2/README.md`

 * *Files identical despite different names*

### Comparing `netlify_dns_manager-0.1/netlify_dns_manage/driver.py` & `netlify_dns_manager-0.2/netlify_dns_manage/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .parser import parse_zone_file
 from .netlify_api import NetlifyAPI
 
 def sync_dns_records(domain_name, zone_file_path, access_token):
     # Parse local DNS zone file
-    local_records = parse_zone_file(zone_file_path)
+    local_records = parse_zone_file(domain_name, zone_file_path)
     if not local_records:
         print("No records found in the zone file.")
     netlify = NetlifyAPI(access_token)
     # Fetch existing DNS records from Netlify
     zone_id = netlify.get_dns_zone(domain_name)
     existing_records = netlify.list_dns_records(zone_id)
```

### Comparing `netlify_dns_manager-0.1/netlify_dns_manage/main.py` & `netlify_dns_manager-0.2/netlify_dns_manage/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from .parser import parse_zone_file
-from .netlify_api import NetlifyAPI
 import argparse
 from .driver import sync_dns_records, convert_to_zone_file
             
 def main():
     # Create a parser with a description of the script's purpose
     parser = argparse.ArgumentParser(description="Sync DNS records from a local zone file to Netlify or export Netlify records to a zone file.")
```

### Comparing `netlify_dns_manager-0.1/netlify_dns_manage/netlify_api.py` & `netlify_dns_manager-0.2/netlify_dns_manage/netlify_api.py`

 * *Files identical despite different names*

### Comparing `netlify_dns_manager-0.1/netlify_dns_manage/utils.py` & `netlify_dns_manager-0.2/netlify_dns_manage/utils.py`

 * *Files identical despite different names*

### Comparing `netlify_dns_manager-0.1/netlify_dns_manager.egg-info/PKG-INFO` & `netlify_dns_manager-0.2/netlify_dns_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netlify-dns-manager
-Version: 0.1
+Version: 0.2
 Summary: It provides a command line interface to manage DNS records of a domain hosted on Netlify.
 Home-page: https://github.com/sumansaurabh/netlify-dns-manager
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `netlify_dns_manager-0.1/netlify_dns_manager.egg-info/SOURCES.txt` & `netlify_dns_manager-0.2/netlify_dns_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netlify_dns_manager-0.1/setup.py` & `netlify_dns_manager-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='netlify-dns-manager',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     description="It provides a command line interface to manage DNS records of a domain hosted on Netlify.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     install_requires=[
         'requests',
         'dnspython',
```

