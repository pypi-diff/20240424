# Comparing `tmp/brynq_sdk_leapsome-1.0.2.tar.gz` & `tmp/brynq_sdk_leapsome-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/brynq_sdk_leapsome-1.0.2.tar", last modified: Wed Apr 24 13:00:59 2024, max compression
+gzip compressed data, was "dist/brynq_sdk_leapsome-1.0.3.tar", last modified: Wed Apr 24 13:05:36 2024, max compression
```

## Comparing `brynq_sdk_leapsome-1.0.2.tar` & `brynq_sdk_leapsome-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:00:59.000000 brynq_sdk_leapsome-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      246 2024-04-24 13:00:59.000000 brynq_sdk_leapsome-1.0.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:00:59.000000 brynq_sdk_leapsome-1.0.2/brynq_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:00:59.000000 brynq_sdk_leapsome-1.0.2/brynq_sdk/leapsome/
--rw-rw-rw-   0 root         (0) root         (0)      117 2024-04-24 13:00:40.000000 brynq_sdk_leapsome-1.0.2/brynq_sdk/leapsome/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4714 2024-04-24 13:00:40.000000 brynq_sdk_leapsome-1.0.2/brynq_sdk/leapsome/api_interface.py
--rw-rw-rw-   0 root         (0) root         (0)     3832 2024-04-24 13:00:40.000000 brynq_sdk_leapsome-1.0.2/brynq_sdk/leapsome/sftp_interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:00:59.000000 brynq_sdk_leapsome-1.0.2/brynq_sdk_leapsome.egg-info/
--rw-r--r--   0 root         (0) root         (0)      246 2024-04-24 13:00:59.000000 brynq_sdk_leapsome-1.0.2/brynq_sdk_leapsome.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      362 2024-04-24 13:00:59.000000 brynq_sdk_leapsome-1.0.2/brynq_sdk_leapsome.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 13:00:59.000000 brynq_sdk_leapsome-1.0.2/brynq_sdk_leapsome.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 13:00:59.000000 brynq_sdk_leapsome-1.0.2/brynq_sdk_leapsome.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       76 2024-04-24 13:00:59.000000 brynq_sdk_leapsome-1.0.2/brynq_sdk_leapsome.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-24 13:00:59.000000 brynq_sdk_leapsome-1.0.2/brynq_sdk_leapsome.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 13:00:59.000000 brynq_sdk_leapsome-1.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      494 2024-04-24 13:00:40.000000 brynq_sdk_leapsome-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:05:36.000000 brynq_sdk_leapsome-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      246 2024-04-24 13:05:36.000000 brynq_sdk_leapsome-1.0.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:05:36.000000 brynq_sdk_leapsome-1.0.3/brynq_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:05:36.000000 brynq_sdk_leapsome-1.0.3/brynq_sdk/leapsome/
+-rw-rw-rw-   0 root         (0) root         (0)      117 2024-04-24 13:05:15.000000 brynq_sdk_leapsome-1.0.3/brynq_sdk/leapsome/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4714 2024-04-24 13:05:15.000000 brynq_sdk_leapsome-1.0.3/brynq_sdk/leapsome/api_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)     3832 2024-04-24 13:05:15.000000 brynq_sdk_leapsome-1.0.3/brynq_sdk/leapsome/sftp_interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:05:36.000000 brynq_sdk_leapsome-1.0.3/brynq_sdk_leapsome.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      246 2024-04-24 13:05:36.000000 brynq_sdk_leapsome-1.0.3/brynq_sdk_leapsome.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      362 2024-04-24 13:05:36.000000 brynq_sdk_leapsome-1.0.3/brynq_sdk_leapsome.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 13:05:36.000000 brynq_sdk_leapsome-1.0.3/brynq_sdk_leapsome.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 13:05:36.000000 brynq_sdk_leapsome-1.0.3/brynq_sdk_leapsome.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       76 2024-04-24 13:05:36.000000 brynq_sdk_leapsome-1.0.3/brynq_sdk_leapsome.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-24 13:05:36.000000 brynq_sdk_leapsome-1.0.3/brynq_sdk_leapsome.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 13:05:36.000000 brynq_sdk_leapsome-1.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      494 2024-04-24 13:05:15.000000 brynq_sdk_leapsome-1.0.3/setup.py
```

### Comparing `brynq_sdk_leapsome-1.0.2/brynq_sdk/leapsome/api_interface.py` & `brynq_sdk_leapsome-1.0.3/brynq_sdk/leapsome/api_interface.py`

 * *Files identical despite different names*

### Comparing `brynq_sdk_leapsome-1.0.2/brynq_sdk/leapsome/sftp_interface.py` & `brynq_sdk_leapsome-1.0.3/brynq_sdk/leapsome/sftp_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pandas as pd
 from typing import Union, List
 import requests
 import datetime
 import json
 from io import StringIO
 import paramiko
-from brynq_sdk.bryng import BrynQ
+from brynq_sdk.brynq import BrynQ
 
 
 class SFTPInterface(BrynQ):
 
     def __init__(self, label: Union[str, List], local_file_directory: str, debug: bool = False):
         """
         For the full documentation, see: https://leapsome.zendesk.com/hc/en-us/articles/4414678642193-SFTP-integration-
```

