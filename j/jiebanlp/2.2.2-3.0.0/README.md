# Comparing `tmp/jiebanlp-2.2.2.tar.gz` & `tmp/jiebanlp-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiebanlp-2.2.2.tar", last modified: Tue Apr 16 10:10:58 2024, max compression
+gzip compressed data, was "jiebanlp-3.0.0.tar", last modified: Wed Apr 24 08:31:48 2024, max compression
```

## Comparing `jiebanlp-2.2.2.tar` & `jiebanlp-3.0.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 10:10:58.517235 jiebanlp-2.2.2/
--rw-rw-rw-   0        0        0      469 2024-04-14 08:16:37.000000 jiebanlp-2.2.2/LICENSE
--rw-rw-rw-   0        0        0        0 2024-04-15 03:10:57.000000 jiebanlp-2.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0      404 2024-04-16 10:10:58.516235 jiebanlp-2.2.2/PKG-INFO
--rw-rw-rw-   0        0        0       21 2024-04-15 03:10:31.000000 jiebanlp-2.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 10:10:58.494064 jiebanlp-2.2.2/jiebanlp/
--rw-rw-rw-   0        0        0        0 2024-04-12 16:09:58.000000 jiebanlp-2.2.2/jiebanlp/__init__.py
--rw-rw-rw-   0        0        0      569 2024-04-15 03:16:25.000000 jiebanlp-2.2.2/jiebanlp/constant.py
--rw-rw-rw-   0        0        0     1660 2024-04-16 10:03:24.000000 jiebanlp-2.2.2/jiebanlp/manager.py
--rw-rw-rw-   0        0        0      290 2024-04-15 03:21:31.000000 jiebanlp-2.2.2/jiebanlp/predict.py
--rw-rw-rw-   0        0        0      296 2024-04-15 05:10:11.000000 jiebanlp-2.2.2/jiebanlp/scheduler.py
--rw-rw-rw-   0        0        0     1456 2024-04-16 10:09:30.000000 jiebanlp-2.2.2/jiebanlp/service.py
-drwxrwxrwx   0        0        0        0 2024-04-16 10:10:58.511211 jiebanlp-2.2.2/jiebanlp.egg-info/
--rw-rw-rw-   0        0        0      404 2024-04-16 10:10:58.000000 jiebanlp-2.2.2/jiebanlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2024-04-16 10:10:58.000000 jiebanlp-2.2.2/jiebanlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 10:10:58.000000 jiebanlp-2.2.2/jiebanlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-16 10:10:58.000000 jiebanlp-2.2.2/jiebanlp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 10:10:58.518960 jiebanlp-2.2.2/setup.cfg
--rw-rw-rw-   0        0        0      646 2024-04-16 10:10:10.000000 jiebanlp-2.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 08:31:48.883202 jiebanlp-3.0.0/
+-rw-rw-rw-   0        0        0      469 2024-04-14 08:16:37.000000 jiebanlp-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0        0 2024-04-15 03:10:57.000000 jiebanlp-3.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      404 2024-04-24 08:31:48.882205 jiebanlp-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       21 2024-04-15 03:10:31.000000 jiebanlp-3.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 08:31:48.857535 jiebanlp-3.0.0/jiebanlp/
+-rw-rw-rw-   0        0        0        0 2024-04-12 16:09:58.000000 jiebanlp-3.0.0/jiebanlp/__init__.py
+-rw-rw-rw-   0        0        0      569 2024-04-15 03:16:25.000000 jiebanlp-3.0.0/jiebanlp/constant.py
+-rw-rw-rw-   0        0        0     1660 2024-04-16 10:03:24.000000 jiebanlp-3.0.0/jiebanlp/manager.py
+-rw-rw-rw-   0        0        0      290 2024-04-15 03:21:31.000000 jiebanlp-3.0.0/jiebanlp/predict.py
+-rw-rw-rw-   0        0        0      296 2024-04-15 05:10:11.000000 jiebanlp-3.0.0/jiebanlp/scheduler.py
+-rw-rw-rw-   0        0        0     1456 2024-04-16 10:09:30.000000 jiebanlp-3.0.0/jiebanlp/service.py
+drwxrwxrwx   0        0        0        0 2024-04-24 08:31:48.877670 jiebanlp-3.0.0/jiebanlp.egg-info/
+-rw-rw-rw-   0        0        0      404 2024-04-24 08:31:48.000000 jiebanlp-3.0.0/jiebanlp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2024-04-24 08:31:48.000000 jiebanlp-3.0.0/jiebanlp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 08:31:48.000000 jiebanlp-3.0.0/jiebanlp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-04-24 08:31:48.000000 jiebanlp-3.0.0/jiebanlp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-24 08:31:48.000000 jiebanlp-3.0.0/jiebanlp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 08:31:48.884205 jiebanlp-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      634 2024-04-24 08:31:34.000000 jiebanlp-3.0.0/setup.py
```

### Comparing `jiebanlp-2.2.2/jiebanlp/constant.py` & `jiebanlp-3.0.0/jiebanlp/constant.py`

 * *Files identical despite different names*

### Comparing `jiebanlp-2.2.2/jiebanlp/manager.py` & `jiebanlp-3.0.0/jiebanlp/manager.py`

 * *Files identical despite different names*

### Comparing `jiebanlp-2.2.2/jiebanlp/service.py` & `jiebanlp-3.0.0/jiebanlp/service.py`

 * *Files identical despite different names*

