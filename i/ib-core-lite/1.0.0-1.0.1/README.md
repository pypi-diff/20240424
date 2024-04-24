# Comparing `tmp/ib_core_lite-1.0.0.tar.gz` & `tmp/ib_core_lite-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ib_core_lite-1.0.0.tar", last modified: Sun Apr  7 20:09:19 2024, max compression
+gzip compressed data, was "ib_core_lite-1.0.1.tar", last modified: Wed Apr 24 12:35:46 2024, max compression
```

## Comparing `ib_core_lite-1.0.0.tar` & `ib_core_lite-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 20:09:19.939117 ib_core_lite-1.0.0/
--rw-rw-rw-   0        0        0     1087 2024-04-07 13:25:09.000000 ib_core_lite-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1423 2024-04-07 20:09:19.939117 ib_core_lite-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      755 2024-04-07 20:03:16.000000 ib_core_lite-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 20:09:19.930470 ib_core_lite-1.0.0/ib_core_lite/
--rw-rw-rw-   0        0        0        0 2024-04-06 20:43:41.000000 ib_core_lite-1.0.0/ib_core_lite/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 20:09:19.939117 ib_core_lite-1.0.0/ib_core_lite/authorization/
--rw-rw-rw-   0        0        0        0 2024-04-06 20:43:41.000000 ib_core_lite-1.0.0/ib_core_lite/authorization/__init__.py
--rw-rw-rw-   0        0        0     5930 2024-04-07 19:57:15.000000 ib_core_lite-1.0.0/ib_core_lite/authorization/models.py
--rw-rw-rw-   0        0        0      257 2024-04-06 20:43:41.000000 ib_core_lite-1.0.0/ib_core_lite/authorization/types.py
--rw-rw-rw-   0        0        0     1561 2024-04-07 19:56:11.000000 ib_core_lite-1.0.0/ib_core_lite/authorization/utils.py
--rw-rw-rw-   0        0        0     6507 2024-04-07 20:03:16.000000 ib_core_lite-1.0.0/ib_core_lite/helpers.py
--rw-rw-rw-   0        0        0      229 2024-04-06 20:49:35.000000 ib_core_lite-1.0.0/ib_core_lite/settings.py
-drwxrwxrwx   0        0        0        0 2024-04-07 20:09:19.939117 ib_core_lite-1.0.0/ib_core_lite/types/
--rw-rw-rw-   0        0        0      279 2024-04-06 20:43:41.000000 ib_core_lite-1.0.0/ib_core_lite/types/__init__.py
--rw-rw-rw-   0        0        0     2419 2024-04-07 20:03:16.000000 ib_core_lite-1.0.0/ib_core_lite/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-07 20:09:19.930470 ib_core_lite-1.0.0/ib_core_lite.egg-info/
--rw-rw-rw-   0        0        0     1423 2024-04-07 20:09:19.000000 ib_core_lite-1.0.0/ib_core_lite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      495 2024-04-07 20:09:19.000000 ib_core_lite-1.0.0/ib_core_lite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 20:09:19.000000 ib_core_lite-1.0.0/ib_core_lite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-04-07 20:09:19.000000 ib_core_lite-1.0.0/ib_core_lite.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-07 20:09:19.000000 ib_core_lite-1.0.0/ib_core_lite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      363 2024-04-07 20:05:35.000000 ib_core_lite-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-07 20:09:19.939117 ib_core_lite-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1099 2024-04-07 20:08:16.000000 ib_core_lite-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 12:35:46.656003 ib_core_lite-1.0.1/
+-rw-rw-rw-   0        0        0     1087 2024-04-24 08:38:05.000000 ib_core_lite-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1423 2024-04-24 12:35:46.656003 ib_core_lite-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2024-04-24 08:38:05.000000 ib_core_lite-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 12:35:46.649891 ib_core_lite-1.0.1/ib_core_lite/
+-rw-rw-rw-   0        0        0        0 2024-04-24 08:38:05.000000 ib_core_lite-1.0.1/ib_core_lite/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 12:35:46.653891 ib_core_lite-1.0.1/ib_core_lite/authorization/
+-rw-rw-rw-   0        0        0        0 2024-04-24 08:38:05.000000 ib_core_lite-1.0.1/ib_core_lite/authorization/__init__.py
+-rw-rw-rw-   0        0        0     5930 2024-04-24 08:38:05.000000 ib_core_lite-1.0.1/ib_core_lite/authorization/models.py
+-rw-rw-rw-   0        0        0      257 2024-04-24 08:38:05.000000 ib_core_lite-1.0.1/ib_core_lite/authorization/types.py
+-rw-rw-rw-   0        0        0     1561 2024-04-24 08:38:05.000000 ib_core_lite-1.0.1/ib_core_lite/authorization/utils.py
+-rw-rw-rw-   0        0        0     6507 2024-04-24 08:38:05.000000 ib_core_lite-1.0.1/ib_core_lite/helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-24 12:35:46.654891 ib_core_lite-1.0.1/ib_core_lite/logging/
+-rw-rw-rw-   0        0        0        0 2024-04-24 09:31:23.000000 ib_core_lite-1.0.1/ib_core_lite/logging/__init__.py
+-rw-rw-rw-   0        0        0      567 2024-04-24 12:33:00.000000 ib_core_lite-1.0.1/ib_core_lite/logging/utils.py
+-rw-rw-rw-   0        0        0      229 2024-04-24 08:38:05.000000 ib_core_lite-1.0.1/ib_core_lite/settings.py
+drwxrwxrwx   0        0        0        0 2024-04-24 12:35:46.654891 ib_core_lite-1.0.1/ib_core_lite/types/
+-rw-rw-rw-   0        0        0      279 2024-04-24 08:38:05.000000 ib_core_lite-1.0.1/ib_core_lite/types/__init__.py
+-rw-rw-rw-   0        0        0     2419 2024-04-24 08:38:05.000000 ib_core_lite-1.0.1/ib_core_lite/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 12:35:46.652891 ib_core_lite-1.0.1/ib_core_lite.egg-info/
+-rw-rw-rw-   0        0        0     1423 2024-04-24 12:35:46.000000 ib_core_lite-1.0.1/ib_core_lite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      558 2024-04-24 12:35:46.000000 ib_core_lite-1.0.1/ib_core_lite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 12:35:46.000000 ib_core_lite-1.0.1/ib_core_lite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-24 12:35:46.000000 ib_core_lite-1.0.1/ib_core_lite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-24 12:35:46.000000 ib_core_lite-1.0.1/ib_core_lite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      363 2024-04-24 08:38:05.000000 ib_core_lite-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-24 12:35:46.657005 ib_core_lite-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1099 2024-04-24 12:33:54.000000 ib_core_lite-1.0.1/setup.py
```

### Comparing `ib_core_lite-1.0.0/LICENSE` & `ib_core_lite-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ib_core_lite-1.0.0/PKG-INFO` & `ib_core_lite-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ib_core_lite
-Version: 1.0.0
+Version: 1.0.1
 Summary: Integration Bus fastapi-applications core
 Home-page: https://gitlab.it-psg.com/ib-elp-it-psg/ib_core_lite
 Download-URL: https://gitlab.it-psg.com/ib-elp-it-psg/ib_core_lite.git
 Author: Damir Fatkhullin
 Author-email: damir.f@it-psg.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ib_core_lite-1.0.0/README.md` & `ib_core_lite-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ib_core_lite-1.0.0/ib_core_lite/authorization/models.py` & `ib_core_lite-1.0.1/ib_core_lite/authorization/models.py`

 * *Files identical despite different names*

### Comparing `ib_core_lite-1.0.0/ib_core_lite/authorization/utils.py` & `ib_core_lite-1.0.1/ib_core_lite/authorization/utils.py`

 * *Files identical despite different names*

### Comparing `ib_core_lite-1.0.0/ib_core_lite/helpers.py` & `ib_core_lite-1.0.1/ib_core_lite/helpers.py`

 * *Files identical despite different names*

### Comparing `ib_core_lite-1.0.0/ib_core_lite/utils.py` & `ib_core_lite-1.0.1/ib_core_lite/utils.py`

 * *Files identical despite different names*

### Comparing `ib_core_lite-1.0.0/ib_core_lite.egg-info/PKG-INFO` & `ib_core_lite-1.0.1/ib_core_lite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ib-core-lite
-Version: 1.0.0
+Version: 1.0.1
 Summary: Integration Bus fastapi-applications core
 Home-page: https://gitlab.it-psg.com/ib-elp-it-psg/ib_core_lite
 Download-URL: https://gitlab.it-psg.com/ib-elp-it-psg/ib_core_lite.git
 Author: Damir Fatkhullin
 Author-email: damir.f@it-psg.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ib_core_lite-1.0.0/setup.py` & `ib_core_lite-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='ib_core_lite',
-    version='1.0.0',
+    version='1.0.1',
     author='Damir Fatkhullin',
     author_email='damir.f@it-psg.com',
     url='https://gitlab.it-psg.com/ib-elp-it-psg/ib_core_lite',
     description='Integration Bus fastapi-applications core',
     download_url='https://gitlab.it-psg.com/ib-elp-it-psg/ib_core_lite.git',
     license='MIT',
     packages=find_packages(),
```

