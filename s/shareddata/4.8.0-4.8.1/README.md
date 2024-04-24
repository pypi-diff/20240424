# Comparing `tmp/shareddata-4.8.0.tar.gz` & `tmp/shareddata-4.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shareddata-4.8.0.tar", last modified: Thu Sep 28 10:02:41 2023, max compression
+gzip compressed data, was "shareddata-4.8.1.tar", last modified: Thu Sep 28 13:32:43 2023, max compression
```

## Comparing `shareddata-4.8.0.tar` & `shareddata-4.8.1.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-09-28 10:02:41.269636 shareddata-4.8.0/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-4.8.0/LICENSE
--rw-r--r--   0 jcooloj   (1000) jcooloj   (1000)     1407 2023-09-28 10:02:41.269636 shareddata-4.8.0/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-4.8.0/README.md
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-09-23 21:18:30.000000 shareddata-4.8.0/pyproject.toml
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      750 2023-09-28 10:02:41.269636 shareddata-4.8.0/setup.cfg
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-09-28 10:02:41.265636 shareddata-4.8.0/src/
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-09-28 10:02:41.269636 shareddata-4.8.0/src/SharedData/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    16628 2023-09-06 22:57:53.000000 shareddata-4.8.0/src/SharedData/AWSKinesis.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5671 2023-08-23 18:07:33.000000 shareddata-4.8.0/src/SharedData/AWSS3.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10669 2023-08-23 18:07:33.000000 shareddata-4.8.0/src/SharedData/DataFrame.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1726 2023-08-23 18:07:33.000000 shareddata-4.8.0/src/SharedData/Defaults.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     3604 2023-08-23 18:07:33.000000 shareddata-4.8.0/src/SharedData/Logger.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11495 2023-09-18 02:54:35.000000 shareddata-4.8.0/src/SharedData/Metadata.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     7479 2023-09-16 01:09:40.000000 shareddata-4.8.0/src/SharedData/MultiProc.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8507 2023-08-24 14:32:51.000000 shareddata-4.8.0/src/SharedData/RealTime.py
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-09-28 10:02:41.269636 shareddata-4.8.0/src/SharedData/Routines/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1360 2023-08-27 23:22:47.000000 shareddata-4.8.0/src/SharedData/Routines/ReadLogs.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    19316 2023-09-22 10:42:43.000000 shareddata-4.8.0/src/SharedData/Routines/Schedule.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1517 2023-09-04 02:39:57.000000 shareddata-4.8.0/src/SharedData/Routines/Scheduler.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      729 2023-08-31 13:01:50.000000 shareddata-4.8.0/src/SharedData/Routines/SendCommand.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1301 2023-09-08 14:48:55.000000 shareddata-4.8.0/src/SharedData/Routines/Server.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2152 2023-09-07 08:48:12.000000 shareddata-4.8.0/src/SharedData/Routines/Worker.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    22492 2023-09-14 14:10:18.000000 shareddata-4.8.0/src/SharedData/Routines/WorkerLib.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-09 17:28:44.000000 shareddata-4.8.0/src/SharedData/Routines/__init__.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     7861 2023-09-27 07:18:37.000000 shareddata-4.8.0/src/SharedData/SharedData.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11452 2023-09-27 11:06:58.000000 shareddata-4.8.0/src/SharedData/SharedNumpy.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    34293 2023-09-27 11:05:09.000000 shareddata-4.8.0/src/SharedData/Table.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14815 2023-09-24 15:28:30.000000 shareddata-4.8.0/src/SharedData/TableIndex.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    39530 2023-09-11 15:04:51.000000 shareddata-4.8.0/src/SharedData/TableIndexJit.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    13325 2023-08-31 12:47:12.000000 shareddata-4.8.0/src/SharedData/TimeSeries.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    16610 2023-09-06 22:57:53.000000 shareddata-4.8.0/src/SharedData/TimeseriesContainer.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1150 2023-09-28 09:32:16.000000 shareddata-4.8.0/src/SharedData/Utils.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-4.8.0/src/SharedData/__init__.py
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-09-28 10:02:41.269636 shareddata-4.8.0/src/shareddata.egg-info/
--rw-r--r--   0 jcooloj   (1000) jcooloj   (1000)     1407 2023-09-28 10:02:41.000000 shareddata-4.8.0/src/shareddata.egg-info/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      997 2023-09-28 10:02:41.000000 shareddata-4.8.0/src/shareddata.egg-info/SOURCES.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-09-28 10:02:41.000000 shareddata-4.8.0/src/shareddata.egg-info/dependency_links.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      231 2023-09-28 10:02:41.000000 shareddata-4.8.0/src/shareddata.egg-info/requires.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-09-28 10:02:41.000000 shareddata-4.8.0/src/shareddata.egg-info/top_level.txt
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-09-28 13:32:43.268725 shareddata-4.8.1/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-4.8.1/LICENSE
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       26 2023-09-28 13:24:29.000000 shareddata-4.8.1/MANIFEST.in
+-rw-r--r--   0 jcooloj   (1000) jcooloj   (1000)     1326 2023-09-28 13:32:43.268725 shareddata-4.8.1/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-4.8.1/README.md
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-09-23 21:18:30.000000 shareddata-4.8.1/pyproject.toml
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      690 2023-09-28 13:32:43.268725 shareddata-4.8.1/setup.cfg
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    21504 2023-09-28 13:26:12.000000 shareddata-4.8.1/sharedmutexwin.pyd
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-09-28 13:32:43.264725 shareddata-4.8.1/src/
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-09-28 13:32:43.268725 shareddata-4.8.1/src/SharedData/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    16628 2023-09-06 22:57:53.000000 shareddata-4.8.1/src/SharedData/AWSKinesis.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5671 2023-08-23 18:07:33.000000 shareddata-4.8.1/src/SharedData/AWSS3.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10669 2023-08-23 18:07:33.000000 shareddata-4.8.1/src/SharedData/DataFrame.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1726 2023-08-23 18:07:33.000000 shareddata-4.8.1/src/SharedData/Defaults.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     3604 2023-08-23 18:07:33.000000 shareddata-4.8.1/src/SharedData/Logger.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11495 2023-09-18 02:54:35.000000 shareddata-4.8.1/src/SharedData/Metadata.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     7479 2023-09-16 01:09:40.000000 shareddata-4.8.1/src/SharedData/MultiProc.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8507 2023-08-24 14:32:51.000000 shareddata-4.8.1/src/SharedData/RealTime.py
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-09-28 13:32:43.268725 shareddata-4.8.1/src/SharedData/Routines/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1360 2023-08-27 23:22:47.000000 shareddata-4.8.1/src/SharedData/Routines/ReadLogs.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    19316 2023-09-22 10:42:43.000000 shareddata-4.8.1/src/SharedData/Routines/Schedule.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1517 2023-09-04 02:39:57.000000 shareddata-4.8.1/src/SharedData/Routines/Scheduler.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      729 2023-08-31 13:01:50.000000 shareddata-4.8.1/src/SharedData/Routines/SendCommand.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1301 2023-09-08 14:48:55.000000 shareddata-4.8.1/src/SharedData/Routines/Server.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2152 2023-09-07 08:48:12.000000 shareddata-4.8.1/src/SharedData/Routines/Worker.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    22492 2023-09-14 14:10:18.000000 shareddata-4.8.1/src/SharedData/Routines/WorkerLib.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-09 17:28:44.000000 shareddata-4.8.1/src/SharedData/Routines/__init__.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     7861 2023-09-27 07:18:37.000000 shareddata-4.8.1/src/SharedData/SharedData.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11452 2023-09-27 11:06:58.000000 shareddata-4.8.1/src/SharedData/SharedNumpy.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    34293 2023-09-27 11:05:09.000000 shareddata-4.8.1/src/SharedData/Table.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14815 2023-09-24 15:28:30.000000 shareddata-4.8.1/src/SharedData/TableIndex.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    39530 2023-09-11 15:04:51.000000 shareddata-4.8.1/src/SharedData/TableIndexJit.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    13325 2023-08-31 12:47:12.000000 shareddata-4.8.1/src/SharedData/TimeSeries.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    16610 2023-09-06 22:57:53.000000 shareddata-4.8.1/src/SharedData/TimeseriesContainer.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1150 2023-09-28 09:32:16.000000 shareddata-4.8.1/src/SharedData/Utils.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-4.8.1/src/SharedData/__init__.py
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-09-28 13:32:43.268725 shareddata-4.8.1/src/shareddata.egg-info/
+-rw-r--r--   0 jcooloj   (1000) jcooloj   (1000)     1326 2023-09-28 13:32:43.000000 shareddata-4.8.1/src/shareddata.egg-info/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1028 2023-09-28 13:32:43.000000 shareddata-4.8.1/src/shareddata.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-09-28 13:32:43.000000 shareddata-4.8.1/src/shareddata.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      198 2023-09-28 13:32:43.000000 shareddata-4.8.1/src/shareddata.egg-info/requires.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-09-28 13:32:43.000000 shareddata-4.8.1/src/shareddata.egg-info/top_level.txt
```

### Comparing `shareddata-4.8.0/LICENSE` & `shareddata-4.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shareddata-4.8.0/PKG-INFO` & `shareddata-4.8.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 4.8.0
+Version: 4.8.1
 Summary: Shared Memory Database with S3 repository
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,16 +16,14 @@
 Requires-Dist: numpy==1.24.3
 Requires-Dist: pandas==2.0.2
 Requires-Dist: XlsxWriter==3.1.2
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: tqdm==4.65.0
 Requires-Dist: cffi==1.15.1
 Requires-Dist: tzlocal==5.0.1
-Provides-Extra: windows
-Requires-Dist: sharedmutexwin==2.0.0; extra == "windows"
 
 # Instalation Instructions
 
 ### create virtual environment
 <ul>
 <li>enter command: pip -m venv venv</li>
 <li>activate virtual environnment (venv\Scripts\activate.bat)</li>
```

### Comparing `shareddata-4.8.0/README.md` & `shareddata-4.8.1/README.md`

 * *Files identical despite different names*

### Comparing `shareddata-4.8.0/src/SharedData/AWSKinesis.py` & `shareddata-4.8.1/src/SharedData/AWSKinesis.py`

 * *Files identical despite different names*

### Comparing `shareddata-4.8.0/src/SharedData/AWSS3.py` & `shareddata-4.8.1/src/SharedData/AWSS3.py`

 * *Files identical despite different names*

### Comparing `shareddata-4.8.0/src/SharedData/DataFrame.py` & `shareddata-4.8.1/src/SharedData/DataFrame.py`

 * *Files identical despite different names*

### Comparing `shareddata-4.8.0/src/SharedData/Defaults.py` & `shareddata-4.8.1/src/SharedData/Defaults.py`

 * *Files identical despite different names*

### Comparing `shareddata-4.8.0/src/SharedData/Logger.py` & `shareddata-4.8.1/src/SharedData/Logger.py`

 * *Files identical despite different names*

### Comparing `shareddata-4.8.0/src/SharedData/Metadata.py` & `shareddata-4.8.1/src/SharedData/Metadata.py`

 * *Files identical despite different names*

### Comparing `shareddata-4.8.0/src/SharedData/MultiProc.py` & `shareddata-4.8.1/src/SharedData/MultiProc.py`

 * *Files identical despite different names*

### Comparing `shareddata-4.8.0/src/SharedData/RealTime.py` & `shareddata-4.8.1/src/SharedData/RealTime.py`

 * *Files identical despite different names*

### Comparing `shareddata-4.8.0/src/SharedData/Routines/ReadLogs.py` & `shareddata-4.8.1/src/SharedData/Routines/ReadLogs.py`

 * *Files identical despite different names*

### Comparing `shareddata-4.8.0/src/SharedData/Routines/Schedule.py` & `shareddata-4.8.1/src/SharedData/Routines/Schedule.py`

 * *Files identical despite different names*

### Comparing `shareddata-4.8.0/src/SharedData/Routines/Scheduler.py` & `shareddata-4.8.1/src/SharedData/Routines/Scheduler.py`

 * *Files identical despite different names*

### Comparing `shareddata-4.8.0/src/SharedData/Routines/SendCommand.py` & `shareddata-4.8.1/src/SharedData/Routines/SendCommand.py`

 * *Files identical despite different names*

### Comparing `shareddata-4.8.0/src/SharedData/Routines/Server.py` & `shareddata-4.8.1/src/SharedData/Routines/Server.py`

 * *Files identical despite different names*

### Comparing `shareddata-4.8.0/src/SharedData/Routines/Worker.py` & `shareddata-4.8.1/src/SharedData/Routines/Worker.py`

 * *Files identical despite different names*

### Comparing `shareddata-4.8.0/src/SharedData/Routines/WorkerLib.py` & `shareddata-4.8.1/src/SharedData/Routines/WorkerLib.py`

 * *Files identical despite different names*

### Comparing `shareddata-4.8.0/src/SharedData/SharedData.py` & `shareddata-4.8.1/src/SharedData/SharedData.py`

 * *Files identical despite different names*

### Comparing `shareddata-4.8.0/src/SharedData/SharedNumpy.py` & `shareddata-4.8.1/src/SharedData/SharedNumpy.py`

 * *Files identical despite different names*

### Comparing `shareddata-4.8.0/src/SharedData/Table.py` & `shareddata-4.8.1/src/SharedData/Table.py`

 * *Files identical despite different names*

### Comparing `shareddata-4.8.0/src/SharedData/TableIndex.py` & `shareddata-4.8.1/src/SharedData/TableIndex.py`

 * *Files identical despite different names*

### Comparing `shareddata-4.8.0/src/SharedData/TableIndexJit.py` & `shareddata-4.8.1/src/SharedData/TableIndexJit.py`

 * *Files identical despite different names*

### Comparing `shareddata-4.8.0/src/SharedData/TimeSeries.py` & `shareddata-4.8.1/src/SharedData/TimeSeries.py`

 * *Files identical despite different names*

### Comparing `shareddata-4.8.0/src/SharedData/TimeseriesContainer.py` & `shareddata-4.8.1/src/SharedData/TimeseriesContainer.py`

 * *Files identical despite different names*

### Comparing `shareddata-4.8.0/src/SharedData/Utils.py` & `shareddata-4.8.1/src/SharedData/Utils.py`

 * *Files identical despite different names*

### Comparing `shareddata-4.8.0/src/shareddata.egg-info/PKG-INFO` & `shareddata-4.8.1/src/shareddata.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 4.8.0
+Version: 4.8.1
 Summary: Shared Memory Database with S3 repository
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,16 +16,14 @@
 Requires-Dist: numpy==1.24.3
 Requires-Dist: pandas==2.0.2
 Requires-Dist: XlsxWriter==3.1.2
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: tqdm==4.65.0
 Requires-Dist: cffi==1.15.1
 Requires-Dist: tzlocal==5.0.1
-Provides-Extra: windows
-Requires-Dist: sharedmutexwin==2.0.0; extra == "windows"
 
 # Instalation Instructions
 
 ### create virtual environment
 <ul>
 <li>enter command: pip -m venv venv</li>
 <li>activate virtual environnment (venv\Scripts\activate.bat)</li>
```

### Comparing `shareddata-4.8.0/src/shareddata.egg-info/SOURCES.txt` & `shareddata-4.8.1/src/shareddata.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
+sharedmutexwin.pyd
 src/SharedData/AWSKinesis.py
 src/SharedData/AWSS3.py
 src/SharedData/DataFrame.py
 src/SharedData/Defaults.py
 src/SharedData/Logger.py
 src/SharedData/Metadata.py
 src/SharedData/MultiProc.py
```

