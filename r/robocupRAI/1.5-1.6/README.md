# Comparing `tmp/robocuprai-1.5.tar.gz` & `tmp/robocuprai-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocuprai-1.5.tar", last modified: Mon Apr 22 21:36:42 2024, max compression
+gzip compressed data, was "robocuprai-1.6.tar", last modified: Wed Apr 24 10:40:23 2024, max compression
```

## Comparing `robocuprai-1.5.tar` & `robocuprai-1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 21:36:42.368974 robocuprai-1.5/
--rw-rw-rw-   0        0        0     1077 2024-04-22 21:07:36.000000 robocuprai-1.5/LICENSE.txt
--rw-rw-rw-   0        0        0      508 2024-04-22 21:36:42.365697 robocuprai-1.5/PKG-INFO
--rw-rw-rw-   0        0        0       12 2024-04-22 21:07:36.000000 robocuprai-1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 21:36:42.345570 robocuprai-1.5/robocupRAI/
--rw-rw-rw-   0        0        0       96 2024-04-22 21:07:36.000000 robocuprai-1.5/robocupRAI/__init__.py
--rw-rw-rw-   0        0        0       28 2024-04-22 21:07:36.000000 robocuprai-1.5/robocupRAI/config.py
--rw-rw-rw-   0        0        0     5197 2024-04-22 21:33:38.000000 robocuprai-1.5/robocupRAI/insert.py
--rw-rw-rw-   0        0        0     1597 2024-04-22 21:07:36.000000 robocuprai-1.5/robocupRAI/query.py
-drwxrwxrwx   0        0        0        0 2024-04-22 21:36:42.362581 robocuprai-1.5/robocupRAI.egg-info/
--rw-rw-rw-   0        0        0      508 2024-04-22 21:36:42.000000 robocuprai-1.5/robocupRAI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2024-04-22 21:36:42.000000 robocuprai-1.5/robocupRAI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 21:36:42.000000 robocuprai-1.5/robocupRAI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-04-22 21:36:42.000000 robocuprai-1.5/robocupRAI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-22 21:36:42.000000 robocuprai-1.5/robocupRAI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 21:36:42.368974 robocuprai-1.5/setup.cfg
--rw-rw-rw-   0        0        0      651 2024-04-22 21:36:35.000000 robocuprai-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:40:23.158116 robocuprai-1.6/
+-rw-rw-rw-   0        0        0     1077 2024-04-24 10:34:05.000000 robocuprai-1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      508 2024-04-24 10:40:23.154611 robocuprai-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2024-04-24 10:34:05.000000 robocuprai-1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 10:40:23.127589 robocuprai-1.6/robocupRAI/
+-rw-rw-rw-   0        0        0       96 2024-04-24 10:34:05.000000 robocuprai-1.6/robocupRAI/__init__.py
+-rw-rw-rw-   0        0        0       28 2024-04-24 10:34:05.000000 robocuprai-1.6/robocupRAI/config.py
+-rw-rw-rw-   0        0        0     5363 2024-04-24 10:39:35.000000 robocuprai-1.6/robocupRAI/insert.py
+-rw-rw-rw-   0        0        0     1597 2024-04-24 10:34:05.000000 robocuprai-1.6/robocupRAI/query.py
+drwxrwxrwx   0        0        0        0 2024-04-24 10:40:23.150443 robocuprai-1.6/robocupRAI.egg-info/
+-rw-rw-rw-   0        0        0      508 2024-04-24 10:40:23.000000 robocuprai-1.6/robocupRAI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2024-04-24 10:40:23.000000 robocuprai-1.6/robocupRAI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 10:40:23.000000 robocuprai-1.6/robocupRAI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-24 10:40:23.000000 robocuprai-1.6/robocupRAI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-24 10:40:23.000000 robocuprai-1.6/robocupRAI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 10:40:23.158116 robocuprai-1.6/setup.cfg
+-rw-rw-rw-   0        0        0      651 2024-04-24 10:40:15.000000 robocuprai-1.6/setup.py
```

### Comparing `robocuprai-1.5/LICENSE.txt` & `robocuprai-1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robocuprai-1.5/robocupRAI/insert.py` & `robocuprai-1.6/robocupRAI/insert.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,24 +156,27 @@
     collection = client['robocup']['target_station']
     
     data = {
         'name': name,
         'type': name[2:4],
         'zone': zone,
         'rotation': int(rotation),
-        'state': False,
+        'state': '',
     }
 
     try:
         result = collection.insert_one(data)
         client.close()
         return True
     except:
         client.close()
         return False
+ 
+def updateTargetStation(host= '10.26.11.13', name= '', state= ''):
+    directUpdate(host, collection='target_station', key= {'name': name}, data= {'state': state})
     
 def resetTargetStation(host= '10.26.11.13'):
     client = pymongo.MongoClient(f'mongodb://{host}:27017/')
     collection = client['robocup']['target_station']
     
     try:
         collection.delete_many({})
```

### Comparing `robocuprai-1.5/robocupRAI/query.py` & `robocuprai-1.6/robocupRAI/query.py`

 * *Files identical despite different names*

### Comparing `robocuprai-1.5/setup.py` & `robocuprai-1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="robocupRAI",
-    version="1.5",
+    version="1.6",
     author="whaly",
     author_email="whalykj@gmail.com",
     description="A small example package MongoDB Robo",
     long_description='long_description',
     long_description_content_type="text/markdown",
     url="https://github.com/whaly-w/robocup",
     packages=setuptools.find_packages(),
```

