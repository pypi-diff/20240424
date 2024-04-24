# Comparing `tmp/SleepHarmonizer-0.1.2.tar.gz` & `tmp/SleepHarmonizer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SleepHarmonizer-0.1.2.tar", last modified: Fri Apr 12 11:22:06 2024, max compression
+gzip compressed data, was "SleepHarmonizer-0.1.3.tar", last modified: Wed Apr 24 08:32:26 2024, max compression
```

## Comparing `SleepHarmonizer-0.1.2.tar` & `SleepHarmonizer-0.1.3.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 11:22:06.127721 SleepHarmonizer-0.1.2/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2024-04-12 11:21:29.000000 SleepHarmonizer-0.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     9049 2024-04-12 11:22:06.127721 SleepHarmonizer-0.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     8562 2024-04-12 11:21:29.000000 SleepHarmonizer-0.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 11:22:06.123721 SleepHarmonizer-0.1.2/SleepHarmonizer/
--rw-rw-rw-   0 root         (0) root         (0)     4184 2024-04-12 11:21:29.000000 SleepHarmonizer-0.1.2/SleepHarmonizer/EDFWriter.py
--rw-rw-rw-   0 root         (0) root         (0)     3961 2024-04-12 11:21:29.000000 SleepHarmonizer-0.1.2/SleepHarmonizer/PSGEventManager.py
--rw-rw-rw-   0 root         (0) root         (0)     1012 2024-04-12 11:21:29.000000 SleepHarmonizer-0.1.2/SleepHarmonizer/Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     6744 2024-04-12 11:21:29.000000 SleepHarmonizer-0.1.2/SleepHarmonizer/SignalPreprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-12 11:21:29.000000 SleepHarmonizer-0.1.2/SleepHarmonizer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      515 2024-04-12 11:21:29.000000 SleepHarmonizer-0.1.2/SleepHarmonizer/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 11:22:06.125721 SleepHarmonizer-0.1.2/SleepHarmonizer/recordloaders/
--rwxrwxrwx   0 root         (0) root         (0)    12683 2024-04-12 11:21:29.000000 SleepHarmonizer-0.1.2/SleepHarmonizer/recordloaders/AliceRMLLoader.py
--rw-rw-rw-   0 root         (0) root         (0)    11246 2024-04-12 11:21:29.000000 SleepHarmonizer-0.1.2/SleepHarmonizer/recordloaders/AliceTextReportLoader.py
--rw-rw-rw-   0 root         (0) root         (0)     4568 2024-04-12 11:21:29.000000 SleepHarmonizer-0.1.2/SleepHarmonizer/recordloaders/DominoAnnotationLoader.py
--rw-rw-rw-   0 root         (0) root         (0)     8335 2024-04-12 11:21:29.000000 SleepHarmonizer-0.1.2/SleepHarmonizer/recordloaders/DominoAnnotationWriter.py
--rw-rw-rw-   0 root         (0) root         (0)     8269 2024-04-12 11:21:29.000000 SleepHarmonizer-0.1.2/SleepHarmonizer/recordloaders/DominoErgLoader.py
--rw-rw-rw-   0 root         (0) root         (0)     7126 2024-04-12 11:21:29.000000 SleepHarmonizer-0.1.2/SleepHarmonizer/recordloaders/RecordLoaderAlice.py
--rw-rw-rw-   0 root         (0) root         (0)     5374 2024-04-12 11:21:29.000000 SleepHarmonizer-0.1.2/SleepHarmonizer/recordloaders/RecordLoaderDomino.py
--rw-rw-rw-   0 root         (0) root         (0)     1219 2024-04-12 11:21:29.000000 SleepHarmonizer-0.1.2/SleepHarmonizer/recordloaders/RecordLoaderTest.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 11:21:29.000000 SleepHarmonizer-0.1.2/SleepHarmonizer/recordloaders/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 11:22:06.124721 SleepHarmonizer-0.1.2/SleepHarmonizer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9049 2024-04-12 11:22:06.000000 SleepHarmonizer-0.1.2/SleepHarmonizer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1056 2024-04-12 11:22:06.000000 SleepHarmonizer-0.1.2/SleepHarmonizer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 11:22:06.000000 SleepHarmonizer-0.1.2/SleepHarmonizer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      153 2024-04-12 11:22:06.000000 SleepHarmonizer-0.1.2/SleepHarmonizer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-12 11:22:06.000000 SleepHarmonizer-0.1.2/SleepHarmonizer.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      371 2024-04-12 11:21:29.000000 SleepHarmonizer-0.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 11:22:06.127721 SleepHarmonizer-0.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1056 2024-04-12 11:21:31.000000 SleepHarmonizer-0.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 11:22:06.126721 SleepHarmonizer-0.1.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 11:21:29.000000 SleepHarmonizer-0.1.2/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      383 2024-04-12 11:21:29.000000 SleepHarmonizer-0.1.2/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 11:22:06.126721 SleepHarmonizer-0.1.2/tests/unit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 11:21:29.000000 SleepHarmonizer-0.1.2/tests/unit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-12 11:21:29.000000 SleepHarmonizer-0.1.2/tests/unit/test_Export.py
--rw-rw-rw-   0 root         (0) root         (0)     1194 2024-04-12 11:21:29.000000 SleepHarmonizer-0.1.2/tests/unit/test_LoadData.py
--rw-rw-rw-   0 root         (0) root         (0)      294 2024-04-12 11:21:29.000000 SleepHarmonizer-0.1.2/tests/unit/test_Setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1177 2024-04-12 11:21:29.000000 SleepHarmonizer-0.1.2/tests/unit/test_SignalPreprocessing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 08:32:26.132346 SleepHarmonizer-0.1.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2024-04-24 08:31:47.000000 SleepHarmonizer-0.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9049 2024-04-24 08:32:26.132346 SleepHarmonizer-0.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     8562 2024-04-24 08:31:47.000000 SleepHarmonizer-0.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 08:32:26.127347 SleepHarmonizer-0.1.3/SleepHarmonizer/
+-rw-rw-rw-   0 root         (0) root         (0)     4184 2024-04-24 08:31:47.000000 SleepHarmonizer-0.1.3/SleepHarmonizer/EDFWriter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3961 2024-04-24 08:31:47.000000 SleepHarmonizer-0.1.3/SleepHarmonizer/PSGEventManager.py
+-rw-rw-rw-   0 root         (0) root         (0)      935 2024-04-24 08:31:47.000000 SleepHarmonizer-0.1.3/SleepHarmonizer/Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     6744 2024-04-24 08:31:47.000000 SleepHarmonizer-0.1.3/SleepHarmonizer/SignalPreprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-24 08:31:47.000000 SleepHarmonizer-0.1.3/SleepHarmonizer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      515 2024-04-24 08:31:47.000000 SleepHarmonizer-0.1.3/SleepHarmonizer/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 08:32:26.130347 SleepHarmonizer-0.1.3/SleepHarmonizer/recordloaders/
+-rwxrwxrwx   0 root         (0) root         (0)    12683 2024-04-24 08:31:47.000000 SleepHarmonizer-0.1.3/SleepHarmonizer/recordloaders/AliceRMLLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)    11246 2024-04-24 08:31:47.000000 SleepHarmonizer-0.1.3/SleepHarmonizer/recordloaders/AliceTextReportLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)     4568 2024-04-24 08:31:47.000000 SleepHarmonizer-0.1.3/SleepHarmonizer/recordloaders/DominoAnnotationLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)     8335 2024-04-24 08:31:47.000000 SleepHarmonizer-0.1.3/SleepHarmonizer/recordloaders/DominoAnnotationWriter.py
+-rw-rw-rw-   0 root         (0) root         (0)     8269 2024-04-24 08:31:47.000000 SleepHarmonizer-0.1.3/SleepHarmonizer/recordloaders/DominoErgLoader.py
+-rw-rw-rw-   0 root         (0) root         (0)     7126 2024-04-24 08:31:47.000000 SleepHarmonizer-0.1.3/SleepHarmonizer/recordloaders/RecordLoaderAlice.py
+-rw-rw-rw-   0 root         (0) root         (0)     5374 2024-04-24 08:31:47.000000 SleepHarmonizer-0.1.3/SleepHarmonizer/recordloaders/RecordLoaderDomino.py
+-rw-rw-rw-   0 root         (0) root         (0)     1219 2024-04-24 08:31:47.000000 SleepHarmonizer-0.1.3/SleepHarmonizer/recordloaders/RecordLoaderTest.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 08:31:47.000000 SleepHarmonizer-0.1.3/SleepHarmonizer/recordloaders/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 08:32:26.128347 SleepHarmonizer-0.1.3/SleepHarmonizer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9049 2024-04-24 08:32:26.000000 SleepHarmonizer-0.1.3/SleepHarmonizer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1082 2024-04-24 08:32:26.000000 SleepHarmonizer-0.1.3/SleepHarmonizer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 08:32:26.000000 SleepHarmonizer-0.1.3/SleepHarmonizer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      153 2024-04-24 08:32:26.000000 SleepHarmonizer-0.1.3/SleepHarmonizer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-24 08:32:26.000000 SleepHarmonizer-0.1.3/SleepHarmonizer.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      371 2024-04-24 08:31:47.000000 SleepHarmonizer-0.1.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 08:32:26.132346 SleepHarmonizer-0.1.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2024-04-24 08:31:49.000000 SleepHarmonizer-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 08:32:26.131347 SleepHarmonizer-0.1.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 08:31:47.000000 SleepHarmonizer-0.1.3/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      383 2024-04-24 08:31:47.000000 SleepHarmonizer-0.1.3/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 08:32:26.132346 SleepHarmonizer-0.1.3/tests/unit/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 08:31:47.000000 SleepHarmonizer-0.1.3/tests/unit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-24 08:31:47.000000 SleepHarmonizer-0.1.3/tests/unit/test_Export.py
+-rw-rw-rw-   0 root         (0) root         (0)     1194 2024-04-24 08:31:47.000000 SleepHarmonizer-0.1.3/tests/unit/test_LoadData.py
+-rwxrwxrwx   0 root         (0) root         (0)     1016 2024-04-24 08:31:47.000000 SleepHarmonizer-0.1.3/tests/unit/test_Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)      294 2024-04-24 08:31:47.000000 SleepHarmonizer-0.1.3/tests/unit/test_Setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1177 2024-04-24 08:31:47.000000 SleepHarmonizer-0.1.3/tests/unit/test_SignalPreprocessing.py
```

### Comparing `SleepHarmonizer-0.1.2/LICENSE` & `SleepHarmonizer-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.2/PKG-INFO` & `SleepHarmonizer-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SleepHarmonizer
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Plugin and stand alone tool to harmonize sleep related data
 Home-page: https://gitlab.com/sleep-is-all-you-need/sleep-harmonizer
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -126,15 +126,15 @@
     emg: 200
     mic: 200
   filterQuery: ahi < 15 and tst > 5 # filter by metada query (compatible with pandas.Dataframe query)
 ```
 
 
 
-### Declear available Channels and Annotations
+### Declare available Channels and Annotations
 
 To determine what channels and annotations you want in you edf files you can use the `extract` options:
 
 - `annotations`: The main groups `apnea`, `arousal`, `limb`, `sleepstage` and `ligt` or any subgroup such as `resp_obstructiveapnea` A complete list can be found in `SleepHarmonizer/PSGEventManager.py`.
 - `channels`: Each entry is a list of channel names, the final channel name is the first channel specified in the list. The first existing channel will be used for the EDF file
 
 ```yaml
```

### Comparing `SleepHarmonizer-0.1.2/README.md` & `SleepHarmonizer-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     emg: 200
     mic: 200
   filterQuery: ahi < 15 and tst > 5 # filter by metada query (compatible with pandas.Dataframe query)
 ```
 
 
 
-### Declear available Channels and Annotations
+### Declare available Channels and Annotations
 
 To determine what channels and annotations you want in you edf files you can use the `extract` options:
 
 - `annotations`: The main groups `apnea`, `arousal`, `limb`, `sleepstage` and `ligt` or any subgroup such as `resp_obstructiveapnea` A complete list can be found in `SleepHarmonizer/PSGEventManager.py`.
 - `channels`: Each entry is a list of channel names, the final channel name is the first channel specified in the list. The first existing channel will be used for the EDF file
 
 ```yaml
```

### Comparing `SleepHarmonizer-0.1.2/SleepHarmonizer/EDFWriter.py` & `SleepHarmonizer-0.1.3/SleepHarmonizer/EDFWriter.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.2/SleepHarmonizer/PSGEventManager.py` & `SleepHarmonizer-0.1.3/SleepHarmonizer/PSGEventManager.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.2/SleepHarmonizer/SignalPreprocessing.py` & `SleepHarmonizer-0.1.3/SleepHarmonizer/SignalPreprocessing.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.2/SleepHarmonizer/config.yaml` & `SleepHarmonizer-0.1.3/SleepHarmonizer/config.yaml`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.2/SleepHarmonizer/recordloaders/AliceRMLLoader.py` & `SleepHarmonizer-0.1.3/SleepHarmonizer/recordloaders/AliceRMLLoader.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.2/SleepHarmonizer/recordloaders/AliceTextReportLoader.py` & `SleepHarmonizer-0.1.3/SleepHarmonizer/recordloaders/AliceTextReportLoader.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.2/SleepHarmonizer/recordloaders/DominoAnnotationLoader.py` & `SleepHarmonizer-0.1.3/SleepHarmonizer/recordloaders/DominoAnnotationLoader.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.2/SleepHarmonizer/recordloaders/DominoAnnotationWriter.py` & `SleepHarmonizer-0.1.3/SleepHarmonizer/recordloaders/DominoAnnotationWriter.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.2/SleepHarmonizer/recordloaders/DominoErgLoader.py` & `SleepHarmonizer-0.1.3/SleepHarmonizer/recordloaders/DominoErgLoader.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.2/SleepHarmonizer/recordloaders/RecordLoaderAlice.py` & `SleepHarmonizer-0.1.3/SleepHarmonizer/recordloaders/RecordLoaderAlice.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.2/SleepHarmonizer/recordloaders/RecordLoaderDomino.py` & `SleepHarmonizer-0.1.3/SleepHarmonizer/recordloaders/RecordLoaderDomino.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.2/SleepHarmonizer/recordloaders/RecordLoaderTest.py` & `SleepHarmonizer-0.1.3/SleepHarmonizer/recordloaders/RecordLoaderTest.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.2/SleepHarmonizer.egg-info/PKG-INFO` & `SleepHarmonizer-0.1.3/SleepHarmonizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SleepHarmonizer
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Plugin and stand alone tool to harmonize sleep related data
 Home-page: https://gitlab.com/sleep-is-all-you-need/sleep-harmonizer
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -126,15 +126,15 @@
     emg: 200
     mic: 200
   filterQuery: ahi < 15 and tst > 5 # filter by metada query (compatible with pandas.Dataframe query)
 ```
 
 
 
-### Declear available Channels and Annotations
+### Declare available Channels and Annotations
 
 To determine what channels and annotations you want in you edf files you can use the `extract` options:
 
 - `annotations`: The main groups `apnea`, `arousal`, `limb`, `sleepstage` and `ligt` or any subgroup such as `resp_obstructiveapnea` A complete list can be found in `SleepHarmonizer/PSGEventManager.py`.
 - `channels`: Each entry is a list of channel names, the final channel name is the first channel specified in the list. The first existing channel will be used for the EDF file
 
 ```yaml
```

### Comparing `SleepHarmonizer-0.1.2/SleepHarmonizer.egg-info/SOURCES.txt` & `SleepHarmonizer-0.1.3/SleepHarmonizer.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -23,9 +23,10 @@
 SleepHarmonizer/recordloaders/RecordLoaderTest.py
 SleepHarmonizer/recordloaders/__init__.py
 tests/__init__.py
 tests/conftest.py
 tests/unit/__init__.py
 tests/unit/test_Export.py
 tests/unit/test_LoadData.py
+tests/unit/test_Plugin.py
 tests/unit/test_Setup.py
 tests/unit/test_SignalPreprocessing.py
```

### Comparing `SleepHarmonizer-0.1.2/setup.py` & `SleepHarmonizer-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SleepHarmonizer",
-    version="v0.1.2"[1:],
+    version="v0.1.3"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="A Plugin and stand alone tool to harmonize sleep related data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/sleep-is-all-you-need/sleep-harmonizer",
     packages=setuptools.find_packages(),
```

### Comparing `SleepHarmonizer-0.1.2/tests/unit/test_Export.py` & `SleepHarmonizer-0.1.3/tests/unit/test_Export.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.2/tests/unit/test_LoadData.py` & `SleepHarmonizer-0.1.3/tests/unit/test_LoadData.py`

 * *Files identical despite different names*

### Comparing `SleepHarmonizer-0.1.2/tests/unit/test_SignalPreprocessing.py` & `SleepHarmonizer-0.1.3/tests/unit/test_SignalPreprocessing.py`

 * *Files identical despite different names*

