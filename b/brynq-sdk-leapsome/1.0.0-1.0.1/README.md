# Comparing `tmp/brynq_sdk_leapsome-1.0.0.tar.gz` & `tmp/brynq_sdk_leapsome-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/brynq_sdk_leapsome-1.0.0.tar", last modified: Wed Apr 24 12:37:11 2024, max compression
+gzip compressed data, was "dist/brynq_sdk_leapsome-1.0.1.tar", last modified: Wed Apr 24 12:41:09 2024, max compression
```

## Comparing `brynq_sdk_leapsome-1.0.0.tar` & `brynq_sdk_leapsome-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:37:11.000000 brynq_sdk_leapsome-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      246 2024-04-24 12:37:11.000000 brynq_sdk_leapsome-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:37:11.000000 brynq_sdk_leapsome-1.0.0/brynq_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:37:11.000000 brynq_sdk_leapsome-1.0.0/brynq_sdk/leapsome/
--rw-rw-rw-   0 root         (0) root         (0)      127 2024-04-24 12:36:53.000000 brynq_sdk_leapsome-1.0.0/brynq_sdk/leapsome/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4714 2024-04-24 12:36:53.000000 brynq_sdk_leapsome-1.0.0/brynq_sdk/leapsome/api_interface.py
--rw-rw-rw-   0 root         (0) root         (0)     3832 2024-04-24 12:36:53.000000 brynq_sdk_leapsome-1.0.0/brynq_sdk/leapsome/sftp_interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:37:11.000000 brynq_sdk_leapsome-1.0.0/brynq_sdk_leapsome.egg-info/
--rw-r--r--   0 root         (0) root         (0)      246 2024-04-24 12:37:11.000000 brynq_sdk_leapsome-1.0.0/brynq_sdk_leapsome.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      362 2024-04-24 12:37:11.000000 brynq_sdk_leapsome-1.0.0/brynq_sdk_leapsome.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 12:37:11.000000 brynq_sdk_leapsome-1.0.0/brynq_sdk_leapsome.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 12:37:11.000000 brynq_sdk_leapsome-1.0.0/brynq_sdk_leapsome.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       84 2024-04-24 12:37:11.000000 brynq_sdk_leapsome-1.0.0/brynq_sdk_leapsome.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-24 12:37:11.000000 brynq_sdk_leapsome-1.0.0/brynq_sdk_leapsome.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 12:37:11.000000 brynq_sdk_leapsome-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      502 2024-04-24 12:36:53.000000 brynq_sdk_leapsome-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:41:09.000000 brynq_sdk_leapsome-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)      246 2024-04-24 12:41:09.000000 brynq_sdk_leapsome-1.0.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:41:09.000000 brynq_sdk_leapsome-1.0.1/brynq_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:41:09.000000 brynq_sdk_leapsome-1.0.1/brynq_sdk/leapsome/
+-rw-rw-rw-   0 root         (0) root         (0)      127 2024-04-24 12:40:54.000000 brynq_sdk_leapsome-1.0.1/brynq_sdk/leapsome/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4714 2024-04-24 12:40:54.000000 brynq_sdk_leapsome-1.0.1/brynq_sdk/leapsome/api_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)     3832 2024-04-24 12:40:54.000000 brynq_sdk_leapsome-1.0.1/brynq_sdk/leapsome/sftp_interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:41:09.000000 brynq_sdk_leapsome-1.0.1/brynq_sdk_leapsome.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      246 2024-04-24 12:41:09.000000 brynq_sdk_leapsome-1.0.1/brynq_sdk_leapsome.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      362 2024-04-24 12:41:09.000000 brynq_sdk_leapsome-1.0.1/brynq_sdk_leapsome.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 12:41:09.000000 brynq_sdk_leapsome-1.0.1/brynq_sdk_leapsome.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 12:41:09.000000 brynq_sdk_leapsome-1.0.1/brynq_sdk_leapsome.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       76 2024-04-24 12:41:09.000000 brynq_sdk_leapsome-1.0.1/brynq_sdk_leapsome.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-24 12:41:09.000000 brynq_sdk_leapsome-1.0.1/brynq_sdk_leapsome.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 12:41:09.000000 brynq_sdk_leapsome-1.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      494 2024-04-24 12:40:54.000000 brynq_sdk_leapsome-1.0.1/setup.py
```

### Comparing `brynq_sdk_leapsome-1.0.0/brynq_sdk/leapsome/api_interface.py` & `brynq_sdk_leapsome-1.0.1/brynq_sdk/leapsome/api_interface.py`

 * *Files identical despite different names*

### Comparing `brynq_sdk_leapsome-1.0.0/brynq_sdk/leapsome/sftp_interface.py` & `brynq_sdk_leapsome-1.0.1/brynq_sdk/leapsome/sftp_interface.py`

 * *Files identical despite different names*

