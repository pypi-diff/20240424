# Comparing `tmp/ctrip-app-ui-0.0.2.tar.gz` & `tmp/ctrip-app-ui-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-app-ui-0.0.2.tar", last modified: Wed Apr 24 10:24:49 2024, max compression
+gzip compressed data, was "ctrip-app-ui-0.0.3.tar", last modified: Wed Apr 24 15:32:07 2024, max compression
```

## Comparing `ctrip-app-ui-0.0.2.tar` & `ctrip-app-ui-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 10:24:49.410220 ctrip-app-ui-0.0.2/
--rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      474 2024-04-24 10:24:49.409222 ctrip-app-ui-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 10:24:49.394264 ctrip-app-ui-0.0.2/capp_ui/
--rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.0.2/capp_ui/__init__.py
--rw-rw-rw-   0        0        0     3028 2024-04-24 09:35:36.000000 ctrip-app-ui-0.0.2/capp_ui/date_extend.py
--rw-rw-rw-   0        0        0     1191 2024-04-24 09:24:00.000000 ctrip-app-ui-0.0.2/capp_ui/device.py
--rw-rw-rw-   0        0        0     1263 2024-04-24 09:31:47.000000 ctrip-app-ui-0.0.2/capp_ui/dir.py
--rw-rw-rw-   0        0        0    49360 2024-04-24 10:21:33.000000 ctrip-app-ui-0.0.2/capp_ui/domain_service.py
--rw-rw-rw-   0        0        0     2270 2024-04-24 09:34:43.000000 ctrip-app-ui-0.0.2/capp_ui/libs.py
--rw-rw-rw-   0        0        0    23814 2024-04-24 09:32:32.000000 ctrip-app-ui-0.0.2/capp_ui/mobile_terminals.py
--rw-rw-rw-   0        0        0     1799 2024-04-24 09:24:12.000000 ctrip-app-ui-0.0.2/capp_ui/platforms.py
--rw-rw-rw-   0        0        0     5563 2024-04-24 09:33:04.000000 ctrip-app-ui-0.0.2/capp_ui/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-24 10:24:49.407228 ctrip-app-ui-0.0.2/ctrip_app_ui.egg-info/
--rw-rw-rw-   0        0        0      474 2024-04-24 10:24:49.000000 ctrip-app-ui-0.0.2/ctrip_app_ui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      389 2024-04-24 10:24:49.000000 ctrip-app-ui-0.0.2/ctrip_app_ui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 10:24:49.000000 ctrip-app-ui-0.0.2/ctrip_app_ui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-24 10:24:49.000000 ctrip-app-ui-0.0.2/ctrip_app_ui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-24 10:24:49.000000 ctrip-app-ui-0.0.2/ctrip_app_ui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 10:24:49.411217 ctrip-app-ui-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-04-24 10:24:37.000000 ctrip-app-ui-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:32:07.378896 ctrip-app-ui-0.0.3/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 09:02:35.000000 ctrip-app-ui-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-04-24 15:32:07.376898 ctrip-app-ui-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       47 2024-04-24 09:02:35.000000 ctrip-app-ui-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 15:32:07.363960 ctrip-app-ui-0.0.3/capp_ui/
+-rw-rw-rw-   0        0        0      470 2024-04-24 09:06:21.000000 ctrip-app-ui-0.0.3/capp_ui/__init__.py
+-rw-rw-rw-   0        0        0     3028 2024-04-24 09:35:36.000000 ctrip-app-ui-0.0.3/capp_ui/date_extend.py
+-rw-rw-rw-   0        0        0     1191 2024-04-24 09:24:00.000000 ctrip-app-ui-0.0.3/capp_ui/device.py
+-rw-rw-rw-   0        0        0     1263 2024-04-24 09:31:47.000000 ctrip-app-ui-0.0.3/capp_ui/dir.py
+-rw-rw-rw-   0        0        0    49360 2024-04-24 10:21:33.000000 ctrip-app-ui-0.0.3/capp_ui/domain_service.py
+-rw-rw-rw-   0        0        0      613 2024-04-24 15:31:00.000000 ctrip-app-ui-0.0.3/capp_ui/fee.py
+-rw-rw-rw-   0        0        0     2270 2024-04-24 09:34:43.000000 ctrip-app-ui-0.0.3/capp_ui/libs.py
+-rw-rw-rw-   0        0        0    23814 2024-04-24 09:32:32.000000 ctrip-app-ui-0.0.3/capp_ui/mobile_terminals.py
+-rw-rw-rw-   0        0        0     1799 2024-04-24 09:24:12.000000 ctrip-app-ui-0.0.3/capp_ui/platforms.py
+-rw-rw-rw-   0        0        0     5563 2024-04-24 09:33:04.000000 ctrip-app-ui-0.0.3/capp_ui/utils.py
+-rw-rw-rw-   0        0        0     2676 2024-04-24 15:31:32.000000 ctrip-app-ui-0.0.3/capp_ui/validators.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:32:07.374905 ctrip-app-ui-0.0.3/ctrip_app_ui.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-04-24 15:32:07.000000 ctrip-app-ui-0.0.3/ctrip_app_ui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      426 2024-04-24 15:32:07.000000 ctrip-app-ui-0.0.3/ctrip_app_ui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 15:32:07.000000 ctrip-app-ui-0.0.3/ctrip_app_ui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-24 15:32:07.000000 ctrip-app-ui-0.0.3/ctrip_app_ui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-24 15:32:07.000000 ctrip-app-ui-0.0.3/ctrip_app_ui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 15:32:07.378896 ctrip-app-ui-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-04-24 15:31:59.000000 ctrip-app-ui-0.0.3/setup.py
```

### Comparing `ctrip-app-ui-0.0.2/LICENSE` & `ctrip-app-ui-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.2/capp_ui/date_extend.py` & `ctrip-app-ui-0.0.3/capp_ui/date_extend.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.2/capp_ui/device.py` & `ctrip-app-ui-0.0.3/capp_ui/device.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.2/capp_ui/dir.py` & `ctrip-app-ui-0.0.3/capp_ui/dir.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.2/capp_ui/domain_service.py` & `ctrip-app-ui-0.0.3/capp_ui/domain_service.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.2/capp_ui/libs.py` & `ctrip-app-ui-0.0.3/capp_ui/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.2/capp_ui/mobile_terminals.py` & `ctrip-app-ui-0.0.3/capp_ui/mobile_terminals.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.2/capp_ui/platforms.py` & `ctrip-app-ui-0.0.3/capp_ui/platforms.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.2/capp_ui/utils.py` & `ctrip-app-ui-0.0.3/capp_ui/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-app-ui-0.0.2/setup.py` & `ctrip-app-ui-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-app-ui',
-    version='0.0.2',
+    version='0.0.3',
     description='This is my ctrip app ui package',
     long_description='This is my ctrip app ui package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-app-ui',
     packages=find_packages(),
     install_requires=[
```

