# Comparing `tmp/robotframework-xlibrary-11.0.3.tar.gz` & `tmp/robotframework-xlibrary-11.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\robotframework-xlibrary-11.0.3.tar", last modified: Mon Apr 22 17:32:53 2024, max compression
+gzip compressed data, was "dist\robotframework-xlibrary-11.0.4.tar", last modified: Tue Apr 23 10:13:28 2024, max compression
```

## Comparing `robotframework-xlibrary-11.0.3.tar` & `robotframework-xlibrary-11.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 17:32:53.000000 robotframework-xlibrary-11.0.3/
--rw-rw-rw-   0        0        0        0 2024-03-13 03:39:44.000000 robotframework-xlibrary-11.0.3/LICENSE
--rw-rw-rw-   0        0        0     2269 2024-04-22 17:32:53.000000 robotframework-xlibrary-11.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1777 2024-04-22 17:31:21.000000 robotframework-xlibrary-11.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-22 17:32:53.000000 robotframework-xlibrary-11.0.3/setup.cfg
--rw-rw-rw-   0        0        0      779 2024-04-22 17:30:19.000000 robotframework-xlibrary-11.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 17:32:53.000000 robotframework-xlibrary-11.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-22 17:32:53.000000 robotframework-xlibrary-11.0.3/src/XLibrary/
--rw-rw-rw-   0        0        0     1114 2024-04-17 07:26:57.000000 robotframework-xlibrary-11.0.3/src/XLibrary/__init__.py
--rw-rw-rw-   0        0        0      235 2024-03-18 09:34:26.000000 robotframework-xlibrary-11.0.3/src/XLibrary/main.py
-drwxrwxrwx   0        0        0        0 2024-04-22 17:32:53.000000 robotframework-xlibrary-11.0.3/src/XLibrary/submodule1/
--rw-rw-rw-   0        0        0      108 2024-03-18 09:34:30.000000 robotframework-xlibrary-11.0.3/src/XLibrary/submodule1/__init__.py
--rw-rw-rw-   0        0        0     1421 2024-04-18 05:25:30.000000 robotframework-xlibrary-11.0.3/src/XLibrary/submodule1/module1.py
--rw-rw-rw-   0        0        0     6598 2024-04-22 17:27:05.000000 robotframework-xlibrary-11.0.3/src/XLibrary/submodule1/module2.py
-drwxrwxrwx   0        0        0        0 2024-04-22 17:32:53.000000 robotframework-xlibrary-11.0.3/src/XLibrary/submodule2/
--rw-rw-rw-   0        0        0      114 2024-03-18 09:34:30.000000 robotframework-xlibrary-11.0.3/src/XLibrary/submodule2/__init__.py
--rw-rw-rw-   0        0        0     1774 2024-04-13 12:59:03.000000 robotframework-xlibrary-11.0.3/src/XLibrary/submodule2/module1.py
--rw-rw-rw-   0        0        0      261 2024-04-22 17:28:01.000000 robotframework-xlibrary-11.0.3/src/XLibrary/submodule2/module2.py
-drwxrwxrwx   0        0        0        0 2024-04-22 17:32:53.000000 robotframework-xlibrary-11.0.3/src/robotframework_xlibrary.egg-info/
--rw-rw-rw-   0        0        0     2269 2024-04-22 17:32:53.000000 robotframework-xlibrary-11.0.3/src/robotframework_xlibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      538 2024-04-22 17:32:53.000000 robotframework-xlibrary-11.0.3/src/robotframework_xlibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 17:32:53.000000 robotframework-xlibrary-11.0.3/src/robotframework_xlibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-22 17:32:53.000000 robotframework-xlibrary-11.0.3/src/robotframework_xlibrary.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-22 17:32:53.000000 robotframework-xlibrary-11.0.3/src/robotframework_xlibrary.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 10:13:28.000000 robotframework-xlibrary-11.0.4/
+-rw-rw-rw-   0        0        0        0 2024-03-13 03:39:44.000000 robotframework-xlibrary-11.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2269 2024-04-23 10:13:28.000000 robotframework-xlibrary-11.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1777 2024-04-22 17:31:21.000000 robotframework-xlibrary-11.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-23 10:13:28.000000 robotframework-xlibrary-11.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      779 2024-04-23 10:08:25.000000 robotframework-xlibrary-11.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 10:13:28.000000 robotframework-xlibrary-11.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-23 10:13:28.000000 robotframework-xlibrary-11.0.4/src/XLibrary/
+-rw-rw-rw-   0        0        0     1114 2024-04-17 07:26:57.000000 robotframework-xlibrary-11.0.4/src/XLibrary/__init__.py
+-rw-rw-rw-   0        0        0      235 2024-03-18 09:34:26.000000 robotframework-xlibrary-11.0.4/src/XLibrary/main.py
+drwxrwxrwx   0        0        0        0 2024-04-23 10:13:28.000000 robotframework-xlibrary-11.0.4/src/XLibrary/submodule1/
+-rw-rw-rw-   0        0        0      108 2024-03-18 09:34:30.000000 robotframework-xlibrary-11.0.4/src/XLibrary/submodule1/__init__.py
+-rw-rw-rw-   0        0        0     1421 2024-04-18 05:25:30.000000 robotframework-xlibrary-11.0.4/src/XLibrary/submodule1/module1.py
+-rw-rw-rw-   0        0        0     7948 2024-04-23 09:32:37.000000 robotframework-xlibrary-11.0.4/src/XLibrary/submodule1/module2.py
+drwxrwxrwx   0        0        0        0 2024-04-23 10:13:28.000000 robotframework-xlibrary-11.0.4/src/XLibrary/submodule2/
+-rw-rw-rw-   0        0        0      114 2024-03-18 09:34:30.000000 robotframework-xlibrary-11.0.4/src/XLibrary/submodule2/__init__.py
+-rw-rw-rw-   0        0        0     1774 2024-04-13 12:59:03.000000 robotframework-xlibrary-11.0.4/src/XLibrary/submodule2/module1.py
+-rw-rw-rw-   0        0        0      261 2024-04-22 17:28:01.000000 robotframework-xlibrary-11.0.4/src/XLibrary/submodule2/module2.py
+drwxrwxrwx   0        0        0        0 2024-04-23 10:13:28.000000 robotframework-xlibrary-11.0.4/src/robotframework_xlibrary.egg-info/
+-rw-rw-rw-   0        0        0     2269 2024-04-23 10:13:28.000000 robotframework-xlibrary-11.0.4/src/robotframework_xlibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2024-04-23 10:13:28.000000 robotframework-xlibrary-11.0.4/src/robotframework_xlibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 10:13:28.000000 robotframework-xlibrary-11.0.4/src/robotframework_xlibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-23 10:13:28.000000 robotframework-xlibrary-11.0.4/src/robotframework_xlibrary.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-23 10:13:28.000000 robotframework-xlibrary-11.0.4/src/robotframework_xlibrary.egg-info/top_level.txt
```

### Comparing `robotframework-xlibrary-11.0.3/PKG-INFO` & `robotframework-xlibrary-11.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-xlibrary
-Version: 11.0.3
+Version: 11.0.4
 Summary: Custom Library for MyAIS 2.0 Automation
 Home-page: https://github.com/Khrx1999/robotframework-xlibrary.git
 Author: Tassana Khrueawan
 Author-email: tassana.khr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `robotframework-xlibrary-11.0.3/README.md` & `robotframework-xlibrary-11.0.4/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-xlibrary-11.0.3/setup.py` & `robotframework-xlibrary-11.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="robotframework-xlibrary",
-    version="11.0.3",
+    version="11.0.4",
     author="Tassana Khrueawan",
     author_email="tassana.khr@gmail.com",
     description="Custom Library for MyAIS 2.0 Automation",
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Khrx1999/robotframework-xlibrary.git",
     package_dir={'': 'src'},
```

### Comparing `robotframework-xlibrary-11.0.3/src/XLibrary/__init__.py` & `robotframework-xlibrary-11.0.4/src/XLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-xlibrary-11.0.3/src/XLibrary/submodule1/module1.py` & `robotframework-xlibrary-11.0.4/src/XLibrary/submodule1/module1.py`

 * *Files identical despite different names*

### Comparing `robotframework-xlibrary-11.0.3/src/XLibrary/submodule1/module2.py` & `robotframework-xlibrary-11.0.4/src/XLibrary/submodule1/module2.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 #submodule1/module2.py
 # -*- coding: utf-8 -*-
 from robot.api.deco import keyword
 import ast
 import pymongo
 import logging
+import bson
+
+
 
 class XDrint:
 
     def __init__(self):
         self._dbconnection = None
 
 
@@ -41,15 +44,14 @@
             logging.error("| Fail: การเชื่อมต่อ MongoDB ล้มเหลว เนื่องจาก TimeOut | %s |" % str(e))
             raise Exception("การเชื่อมต่อ MongoDB ล้มเหลว เนื่องจาก TimeOut")
         except Exception as e:
             logging.error("| Fail: การเชื่อมต่อ MongoDB ล้มเหลว | %s |" % str(e))
             raise Exception("การเชื่อมต่อ MongoDB ล้มเหลว: " + str(e))
         
 
-    
     @keyword("XQuery MongoDB")
     def query_mongodb(self, database_name, collection_name, query, limit=None, sort=None):
         """
         ***|    Description     |***
         |   *`Query MongoDB`*   |   เป็น Keyword สำหรับ Query ข้อมูลใน Collection พร้อมกับการกำหนดจำนวนข้อมูลสูงสุดและการเรียงลำดับข้อมูล |
 
         
@@ -139,7 +141,30 @@
             for doc in result:
                 if isinstance(doc, dict) and field_name in doc:
                     results.append(doc[field_name])
         else:
             results = result.get(field_name, None)
 
         return results
+
+
+    @keyword("XConvert BSON Document to JSON Object")
+    def bson_to_json_object(self, bson_data):
+        """
+        แปลงข้อมูล BSON เป็นอ็อบเจกต์ Python (dictionary หรือ list) โดยไม่ต้องแปลงเป็นสตริง JSON
+
+        พารามิเตอร์:
+        - bson_data: ข้อมูล BSON ในรูปแบบไบต์สตริงหรือดิกชันนารี
+
+        ผลลัพธ์ที่ได้:
+        - อ็อบเจกต์ Python ซึ่งอาจเป็นดิกชันนารีหรือลิสต์ของดิกชันนารีที่แสดงถึงข้อมูล BSON
+
+        ตัวอย่างการใช้งาน:
+        | ${json_object} = | Convert BSON Document to JSON Object | ${bson_data} |
+        """
+        try:
+            if isinstance(bson_data, bytes):
+                bson_data = bson.loads(bson_data)
+            # Convert BSON directly to a Python object without converting to a JSON string
+            return bson_data  # This returns a Python dictionary or list of dictionaries
+        except Exception as e:
+            return f"Failed to convert BSON to JSON object: {str(e)}"
```

### Comparing `robotframework-xlibrary-11.0.3/src/XLibrary/submodule2/module1.py` & `robotframework-xlibrary-11.0.4/src/XLibrary/submodule2/module1.py`

 * *Files identical despite different names*

### Comparing `robotframework-xlibrary-11.0.3/src/robotframework_xlibrary.egg-info/PKG-INFO` & `robotframework-xlibrary-11.0.4/src/robotframework_xlibrary.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-xlibrary
-Version: 11.0.3
+Version: 11.0.4
 Summary: Custom Library for MyAIS 2.0 Automation
 Home-page: https://github.com/Khrx1999/robotframework-xlibrary.git
 Author: Tassana Khrueawan
 Author-email: tassana.khr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `robotframework-xlibrary-11.0.3/src/robotframework_xlibrary.egg-info/SOURCES.txt` & `robotframework-xlibrary-11.0.4/src/robotframework_xlibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

