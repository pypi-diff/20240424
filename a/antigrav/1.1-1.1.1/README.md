# Comparing `tmp/antigrav-1.1.tar.gz` & `tmp/antigrav-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antigrav-1.1.tar", last modified: Wed Apr 24 12:41:15 2024, max compression
+gzip compressed data, was "antigrav-1.1.1.tar", last modified: Wed Apr 24 12:44:05 2024, max compression
```

## Comparing `antigrav-1.1.tar` & `antigrav-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 12:41:15.964174 antigrav-1.1/
--rw-rw-rw-   0        0        0      181 2024-04-24 12:34:49.000000 antigrav-1.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0       25 2024-01-25 13:25:38.000000 antigrav-1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1466 2024-04-24 12:41:15.963175 antigrav-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1002 2024-03-16 13:04:35.000000 antigrav-1.1/README.txt
-drwxrwxrwx   0        0        0        0 2024-04-24 12:41:15.942147 antigrav-1.1/antigrav/
--rw-rw-rw-   0        0        0    12121 2024-04-24 12:37:00.000000 antigrav-1.1/antigrav/__init__.py
--rw-rw-rw-   0        0        0    12994 2024-04-24 12:36:13.000000 antigrav-1.1/antigrav/decoder.py
--rw-rw-rw-   0        0        0    16957 2024-03-16 12:44:30.000000 antigrav-1.1/antigrav/encoder.py
--rw-rw-rw-   0        0        0     3342 2024-04-24 12:14:42.000000 antigrav-1.1/antigrav/scanner.py
--rw-rw-rw-   0        0        0     3480 2024-03-16 12:36:38.000000 antigrav-1.1/antigrav/tool.py
-drwxrwxrwx   0        0        0        0 2024-04-24 12:41:15.962160 antigrav-1.1/antigrav.egg-info/
--rw-rw-rw-   0        0        0     1466 2024-04-24 12:41:15.000000 antigrav-1.1/antigrav.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2024-04-24 12:41:15.000000 antigrav-1.1/antigrav.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 12:41:15.000000 antigrav-1.1/antigrav.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-24 12:41:15.000000 antigrav-1.1/antigrav.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 12:41:15.964174 antigrav-1.1/setup.cfg
--rw-rw-rw-   0        0        0      699 2024-04-24 12:41:02.000000 antigrav-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 12:44:05.641247 antigrav-1.1.1/
+-rw-rw-rw-   0        0        0      222 2024-04-24 12:43:30.000000 antigrav-1.1.1/CHANGELOG.txt
+-rw-rw-rw-   0        0        0       25 2024-01-25 13:25:38.000000 antigrav-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1468 2024-04-24 12:44:05.640249 antigrav-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1002 2024-03-16 13:04:35.000000 antigrav-1.1.1/README.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 12:44:05.621254 antigrav-1.1.1/antigrav/
+-rw-rw-rw-   0        0        0    12125 2024-04-24 12:43:19.000000 antigrav-1.1.1/antigrav/__init__.py
+-rw-rw-rw-   0        0        0    12994 2024-04-24 12:36:13.000000 antigrav-1.1.1/antigrav/decoder.py
+-rw-rw-rw-   0        0        0    16957 2024-03-16 12:44:30.000000 antigrav-1.1.1/antigrav/encoder.py
+-rw-rw-rw-   0        0        0     3342 2024-04-24 12:14:42.000000 antigrav-1.1.1/antigrav/scanner.py
+-rw-rw-rw-   0        0        0     3480 2024-03-16 12:36:38.000000 antigrav-1.1.1/antigrav/tool.py
+drwxrwxrwx   0        0        0        0 2024-04-24 12:44:05.637728 antigrav-1.1.1/antigrav.egg-info/
+-rw-rw-rw-   0        0        0     1468 2024-04-24 12:44:05.000000 antigrav-1.1.1/antigrav.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2024-04-24 12:44:05.000000 antigrav-1.1.1/antigrav.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 12:44:05.000000 antigrav-1.1.1/antigrav.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-24 12:44:05.000000 antigrav-1.1.1/antigrav.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 12:44:05.641247 antigrav-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      701 2024-04-24 12:43:57.000000 antigrav-1.1.1/setup.py
```

### Comparing `antigrav-1.1/PKG-INFO` & `antigrav-1.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antigrav
-Version: 1.1
+Version: 1.1.1
 Summary: antigrav is basically JSON but supports complex numbers
 Home-page: 
 Author: tema5002
 Author-email: xtema5002x@gmail.com
 Keywords: kreisi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

### Comparing `antigrav-1.1/README.txt` & `antigrav-1.1.1/README.txt`

 * *Files identical despite different names*

### Comparing `antigrav-1.1/antigrav/__init__.py` & `antigrav-1.1.1/antigrav/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 __json_version__ = '2.0.9'
 __all__ = [
     'dump', 'dumps', 'load', 'loads',
     'ANTIGRAVDecoder', 'ANTIGRAVDecodeError', 'ANTIGRAVEncoder',
 ]
 
 __author__ = "tema5002 <tema5002@gmail.com>"
-__version__ = "1.1"
+__version__ = "1.1.1"
 __short_description__ = "antigrav is basically JSON but supports complex numbers"
 
-from decoder import ANTIGRAVDecoder, ANTIGRAVDecodeError
-from encoder import ANTIGRAVEncoder
+from .decoder import ANTIGRAVDecoder, ANTIGRAVDecodeError
+from .encoder import ANTIGRAVEncoder
 import codecs
 
 _default_encoder = ANTIGRAVEncoder(
     skipkeys=False,
     ensure_ascii=True,
     check_circular=True,
     allow_nan=True,
```

### Comparing `antigrav-1.1/antigrav/decoder.py` & `antigrav-1.1.1/antigrav/decoder.py`

 * *Files identical despite different names*

### Comparing `antigrav-1.1/antigrav/encoder.py` & `antigrav-1.1.1/antigrav/encoder.py`

 * *Files identical despite different names*

### Comparing `antigrav-1.1/antigrav/scanner.py` & `antigrav-1.1.1/antigrav/scanner.py`

 * *Files identical despite different names*

### Comparing `antigrav-1.1/antigrav/tool.py` & `antigrav-1.1.1/antigrav/tool.py`

 * *Files identical despite different names*

### Comparing `antigrav-1.1/antigrav.egg-info/PKG-INFO` & `antigrav-1.1.1/antigrav.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antigrav
-Version: 1.1
+Version: 1.1.1
 Summary: antigrav is basically JSON but supports complex numbers
 Home-page: 
 Author: tema5002
 Author-email: xtema5002x@gmail.com
 Keywords: kreisi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

### Comparing `antigrav-1.1/setup.py` & `antigrav-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "Intended Audience :: Education",
     "Operating System :: Microsoft :: Windows :: Windows 11",
     "Programming Language :: Python :: 3"
 ]
 
 setup(
     name="antigrav",
-    version="1.1",
+    version="1.1.1",
     description="antigrav is basically JSON but supports complex numbers",
     long_description=open("README.txt").read(),
     url="",
     author="tema5002",
     author_email="xtema5002x@gmail.com",
     license="",
     classifiers=classifiers,
```

