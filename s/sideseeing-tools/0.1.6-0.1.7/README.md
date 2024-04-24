# Comparing `tmp/sideseeing_tools-0.1.6.tar.gz` & `tmp/sideseeing_tools-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sideseeing_tools-0.1.6.tar", last modified: Mon Apr 22 21:43:43 2024, max compression
+gzip compressed data, was "sideseeing_tools-0.1.7.tar", last modified: Wed Apr 24 17:52:24 2024, max compression
```

## Comparing `sideseeing_tools-0.1.6.tar` & `sideseeing_tools-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-22 21:43:43.012475 sideseeing_tools-0.1.6/
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     1088 2024-04-22 21:02:32.000000 sideseeing_tools-0.1.6/LICENSE
--rw-r--r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     4410 2024-04-22 21:43:43.012475 sideseeing_tools-0.1.6/PKG-INFO
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     3531 2024-04-22 21:31:25.000000 sideseeing_tools-0.1.6/README.md
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      878 2024-04-22 21:03:07.000000 sideseeing_tools-0.1.6/pyproject.toml
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)       38 2024-04-22 21:43:43.012475 sideseeing_tools-0.1.6/setup.cfg
-drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-22 21:43:43.012475 sideseeing_tools-0.1.6/src/
-drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-22 21:43:43.012475 sideseeing_tools-0.1.6/src/sideseeing_tools/
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-22 21:02:32.000000 sideseeing_tools-0.1.6/src/sideseeing_tools/__init__.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      962 2024-04-22 21:02:32.000000 sideseeing_tools-0.1.6/src/sideseeing_tools/constants.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      206 2024-04-22 21:02:32.000000 sideseeing_tools-0.1.6/src/sideseeing_tools/exceptions.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     2341 2024-04-22 21:02:32.000000 sideseeing_tools-0.1.6/src/sideseeing_tools/media.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)    15261 2024-04-22 21:11:00.000000 sideseeing_tools-0.1.6/src/sideseeing_tools/plot.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     8628 2024-04-22 21:43:38.000000 sideseeing_tools-0.1.6/src/sideseeing_tools/sideseeing.py
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     7397 2024-04-22 21:27:31.000000 sideseeing_tools-0.1.6/src/sideseeing_tools/utils.py
-drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-22 21:43:43.012475 sideseeing_tools-0.1.6/src/sideseeing_tools.egg-info/
--rw-r--r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     4410 2024-04-22 21:43:43.000000 sideseeing_tools-0.1.6/src/sideseeing_tools.egg-info/PKG-INFO
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      477 2024-04-22 21:43:43.000000 sideseeing_tools-0.1.6/src/sideseeing_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)        1 2024-04-22 21:43:43.000000 sideseeing_tools-0.1.6/src/sideseeing_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      134 2024-04-22 21:43:43.000000 sideseeing_tools-0.1.6/src/sideseeing_tools.egg-info/requires.txt
--rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)       17 2024-04-22 21:43:43.000000 sideseeing_tools-0.1.6/src/sideseeing_tools.egg-info/top_level.txt
+drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-24 17:52:24.971136 sideseeing_tools-0.1.7/
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     1088 2024-04-22 21:02:32.000000 sideseeing_tools-0.1.7/LICENSE
+-rw-r--r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     5582 2024-04-24 17:52:24.971136 sideseeing_tools-0.1.7/PKG-INFO
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     4670 2024-04-24 17:50:34.000000 sideseeing_tools-0.1.7/README.md
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      901 2024-04-24 16:06:08.000000 sideseeing_tools-0.1.7/pyproject.toml
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)       38 2024-04-24 17:52:24.971136 sideseeing_tools-0.1.7/setup.cfg
+drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-24 17:52:24.971136 sideseeing_tools-0.1.7/src/
+drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-24 17:52:24.971136 sideseeing_tools-0.1.7/src/sideseeing_tools/
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-22 21:02:32.000000 sideseeing_tools-0.1.7/src/sideseeing_tools/__init__.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      962 2024-04-22 21:02:32.000000 sideseeing_tools-0.1.7/src/sideseeing_tools/constants.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      206 2024-04-22 21:02:32.000000 sideseeing_tools-0.1.7/src/sideseeing_tools/exceptions.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     3655 2024-04-24 17:31:46.000000 sideseeing_tools-0.1.7/src/sideseeing_tools/media.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)    15261 2024-04-22 21:11:00.000000 sideseeing_tools-0.1.7/src/sideseeing_tools/plot.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     8748 2024-04-24 17:02:21.000000 sideseeing_tools-0.1.7/src/sideseeing_tools/sideseeing.py
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     7397 2024-04-22 21:27:31.000000 sideseeing_tools-0.1.7/src/sideseeing_tools/utils.py
+drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-24 17:52:24.971136 sideseeing_tools-0.1.7/src/sideseeing_tools.egg-info/
+-rw-r--r--   0 rafaeljpd  (1000) rafaeljpd  (1000)     5582 2024-04-24 17:52:24.000000 sideseeing_tools-0.1.7/src/sideseeing_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      497 2024-04-24 17:52:24.000000 sideseeing_tools-0.1.7/src/sideseeing_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)        1 2024-04-24 17:52:24.000000 sideseeing_tools-0.1.7/src/sideseeing_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      152 2024-04-24 17:52:24.000000 sideseeing_tools-0.1.7/src/sideseeing_tools.egg-info/requires.txt
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)       17 2024-04-24 17:52:24.000000 sideseeing_tools-0.1.7/src/sideseeing_tools.egg-info/top_level.txt
+drwxrwxr-x   0 rafaeljpd  (1000) rafaeljpd  (1000)        0 2024-04-24 17:52:24.971136 sideseeing_tools-0.1.7/tests/
+-rw-rw-r--   0 rafaeljpd  (1000) rafaeljpd  (1000)      114 2024-04-24 16:01:51.000000 sideseeing_tools-0.1.7/tests/test_media.py
```

### Comparing `sideseeing_tools-0.1.6/LICENSE` & `sideseeing_tools-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sideseeing_tools-0.1.6/PKG-INFO` & `sideseeing_tools-0.1.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: sideseeing-tools
-Version: 0.1.6
-Summary: A set of tools to load, preprocess and analyze data collected through the MultiSensor Data Collection App
-Author-email: "Rafael J. P. Damaceno" <rafael.damaceno@ime.usp.br>
-Project-URL: Homepage, https://github.com/rafaelpezzuto/sideseeing-tools
-Project-URL: Issues, https://github.com/rafaelpezzuto/sideseeing-tools/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: folium~=0.13.0
-Requires-Dist: imageio~=2.5.0
-Requires-Dist: librosa~=0.10.0
-Requires-Dist: moviepy~=1.0.3
-Requires-Dist: numpy~=1.25.0
-Requires-Dist: opencv-python~=4.7.0.68
-Requires-Dist: pandas~=2.0.3
-Requires-Dist: reverse-geocode==1.6
-
 # SideSeeing Tools
 
 SideSeeing Tools is a collection of scripts designed to load, preprocess, and analyze data gathered through the MultiSensor Data Collection App.
 
 ## Installation
 
 ```bash
@@ -40,15 +18,31 @@
 
 # Available iterators
 #   .instances  // Tip: dictionary of instances (key=instance_name, value=SideSeeingInstance)
 #   .iterator   // Tip: for i in ds.iterator: i.instance_name
 
 # Available attributes and methods
 #   .metadata() // Tip: generates and prints the dataset metadata
-#   .size       // Tip: number of instances  
+#   .size       // Tip: shows the number of instances  
+#   .sensors    // Tip: lists the names of the available sensors
+```
+
+__Get a random sample from the dataset__
+```python
+my_sample = ds.instance
+```
+
+__Extract accelerometer data from the sample__
+```python
+my_accel_data = ds.instance['sensors3']['Accelerometer']
+```
+
+__Show available sensors in the dataset__
+```python
+ds.sensors
 ```
 
 __Iterating over the samples__
 
 ```python
 for i in ds.iterator:
     print(i.instance_name, i.video)
@@ -87,14 +81,27 @@
 #   .plot_instance_map()
 #   .plot_instance_sensors3_and_audio()
 #   .plot_instance_video_frames_at_times()
 #   .plot_instance_video_frames()
 #   .generate_video_sensor3()
 ```
 
+__Media tools__
+```python
+from sideseeing_tools import media
+
+# Extract a 15-second snippet from the video, beginning at the 3-second mark and ending at the 18-second mark
+media.extract_video_snippet(
+    source_path=my_sample.video # Tip: path to a mp4 file
+    start_second=3,
+    end_second=18,
+    output_path='my_snippet.mp4'
+)
+```
+
 __Suggested dataset folder structure__
 
 `ds = sideseeing.SideSeeingDS('/home/user/my-project', subdir='data', name='MyDataset')`
 
 ```text
 my-project/
 ├─ data/
@@ -113,16 +120,27 @@
 │  ├─ place02/
 │  ├─ place03/
 ├─ metadata.csv
 ├─ taxonomy.csv
 ```
 
 
-## Documentation
-Under construction.
+## Sensors variables
+
+### 3-axis sensors (accelerometer, gyroscope, among others)
+| N | Column          | Description      |
+|---|-----------------|----------------|
+| 1 | timestamp_nano  | Timestamp in nanoseconds |
+| 2 | datetime_utc    | Date/time in Coordinated Universal Time (UTC) |
+| 3 | name            | Sensor name |
+| 4 | axis_x          | Value of axis X |
+| 5 | axis_y          | Value of axis Y |
+| 6 | axis_z          | Value of axis Z |
+| 7 | accuracy        | Sensor accuracy |
+
 
 ## Author
 
 [Rafael J P Damaceno](https://github.com/rafaelpezzuto)
 
 
 ## About us
```

### Comparing `sideseeing_tools-0.1.6/pyproject.toml` & `sideseeing_tools-0.1.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [project]
 name = "sideseeing-tools"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   {name="Rafael J. P. Damaceno", email="rafael.damaceno@ime.usp.br"},
 ]
 description = "A set of tools to load, preprocess and analyze data collected through the MultiSensor Data Collection App"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
   "folium~=0.13.0",
   "imageio~=2.5.0",
   "librosa~=0.10.0",
+  "matplotlib~=3.8.4",
   "moviepy~=1.0.3",
   "numpy~=1.25.0",
   "opencv-python~=4.7.0.68",
   "pandas~=2.0.3",
   "reverse-geocode==1.6",
 ]
 classifiers = [
```

### Comparing `sideseeing_tools-0.1.6/src/sideseeing_tools/constants.py` & `sideseeing_tools-0.1.7/src/sideseeing_tools/constants.py`

 * *Files identical despite different names*

### Comparing `sideseeing_tools-0.1.6/src/sideseeing_tools/plot.py` & `sideseeing_tools-0.1.7/src/sideseeing_tools/plot.py`

 * *Files identical despite different names*

### Comparing `sideseeing_tools-0.1.6/src/sideseeing_tools/sideseeing.py` & `sideseeing_tools-0.1.7/src/sideseeing_tools/sideseeing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import datetime
 import json
 import os
+import random
 
 from sideseeing_tools import (
     constants, 
     exceptions,
     media,
     utils,
 )
@@ -15,30 +16,30 @@
             self, 
             root_dir,
             subdir_data='.',
             name='MyDataset', 
             generate_metadata=True,
             extract_media=True,
         ):
+        print('INFO. Loading data.')
         self.name = name
         
         if not os.path.isdir(root_dir):
             raise exceptions.RootDirIsNotADirectoryError()
 
         if not os.path.exists(root_dir):
             raise exceptions.RootDirDoesNotExistError()
 
         self.root_dir = root_dir if root_dir.endswith(os.path.sep) else f'{root_dir}{os.path.sep}'
         self.data_dir = os.path.join(self.root_dir, subdir_data)
         self.setup(extract_media)
 
         if generate_metadata:
             self.metadata(generate_metadata)
-
-        self.sensors = self.discover_sensors()
+        print('INFO. Done.')
 
     def setup(self, extract_media):
         self.instances = {}
         for root, _, files in os.walk(self.data_dir):
             for f in files:
                 if f not in constants.SUPPORTED_FILES:
                     print(f'WARNING. {os.path.join(root, f)} has been ignored.')
@@ -52,28 +53,28 @@
                                 ssf.instance_path,
                             )
                     self.instances[ssf.instance_name].add_file(ssf)
 
         for key in self.instances.keys():
             self.instances[key].setup(extract_media)
 
-    def discover_sensors(self):
-        sns = set()
-
+        self.sensors = set()
         for i in self.iterator:
             for name in i.sensors1.keys():
-                sns.add(name)
+                self.sensors.add(name)
 
             for name in i.sensors3.keys():
-                sns.add(name)
+                self.sensors.add(name)
 
             for name in i.sensors6.keys():
-                sns.add(name)
-        
-        return sns
+                self.sensors.add(name)
+
+    @property
+    def instance(self):
+        return self.instances[random.choice(list(self.instances.keys()))]
 
     @property
     def size(self):
         return len(self.instances)
 
     @property
     def iterator(self):
```

### Comparing `sideseeing_tools-0.1.6/src/sideseeing_tools/utils.py` & `sideseeing_tools-0.1.7/src/sideseeing_tools/utils.py`

 * *Files identical despite different names*

### Comparing `sideseeing_tools-0.1.6/src/sideseeing_tools.egg-info/PKG-INFO` & `sideseeing_tools-0.1.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: sideseeing-tools
-Version: 0.1.6
+Version: 0.1.7
 Summary: A set of tools to load, preprocess and analyze data collected through the MultiSensor Data Collection App
 Author-email: "Rafael J. P. Damaceno" <rafael.damaceno@ime.usp.br>
 Project-URL: Homepage, https://github.com/rafaelpezzuto/sideseeing-tools
 Project-URL: Issues, https://github.com/rafaelpezzuto/sideseeing-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: folium~=0.13.0
 Requires-Dist: imageio~=2.5.0
 Requires-Dist: librosa~=0.10.0
+Requires-Dist: matplotlib~=3.8.4
 Requires-Dist: moviepy~=1.0.3
 Requires-Dist: numpy~=1.25.0
 Requires-Dist: opencv-python~=4.7.0.68
 Requires-Dist: pandas~=2.0.3
 Requires-Dist: reverse-geocode==1.6
 
 # SideSeeing Tools
@@ -40,15 +41,31 @@
 
 # Available iterators
 #   .instances  // Tip: dictionary of instances (key=instance_name, value=SideSeeingInstance)
 #   .iterator   // Tip: for i in ds.iterator: i.instance_name
 
 # Available attributes and methods
 #   .metadata() // Tip: generates and prints the dataset metadata
-#   .size       // Tip: number of instances  
+#   .size       // Tip: shows the number of instances  
+#   .sensors    // Tip: lists the names of the available sensors
+```
+
+__Get a random sample from the dataset__
+```python
+my_sample = ds.instance
+```
+
+__Extract accelerometer data from the sample__
+```python
+my_accel_data = ds.instance['sensors3']['Accelerometer']
+```
+
+__Show available sensors in the dataset__
+```python
+ds.sensors
 ```
 
 __Iterating over the samples__
 
 ```python
 for i in ds.iterator:
     print(i.instance_name, i.video)
@@ -87,14 +104,27 @@
 #   .plot_instance_map()
 #   .plot_instance_sensors3_and_audio()
 #   .plot_instance_video_frames_at_times()
 #   .plot_instance_video_frames()
 #   .generate_video_sensor3()
 ```
 
+__Media tools__
+```python
+from sideseeing_tools import media
+
+# Extract a 15-second snippet from the video, beginning at the 3-second mark and ending at the 18-second mark
+media.extract_video_snippet(
+    source_path=my_sample.video # Tip: path to a mp4 file
+    start_second=3,
+    end_second=18,
+    output_path='my_snippet.mp4'
+)
+```
+
 __Suggested dataset folder structure__
 
 `ds = sideseeing.SideSeeingDS('/home/user/my-project', subdir='data', name='MyDataset')`
 
 ```text
 my-project/
 ├─ data/
@@ -113,16 +143,27 @@
 │  ├─ place02/
 │  ├─ place03/
 ├─ metadata.csv
 ├─ taxonomy.csv
 ```
 
 
-## Documentation
-Under construction.
+## Sensors variables
+
+### 3-axis sensors (accelerometer, gyroscope, among others)
+| N | Column          | Description      |
+|---|-----------------|----------------|
+| 1 | timestamp_nano  | Timestamp in nanoseconds |
+| 2 | datetime_utc    | Date/time in Coordinated Universal Time (UTC) |
+| 3 | name            | Sensor name |
+| 4 | axis_x          | Value of axis X |
+| 5 | axis_y          | Value of axis Y |
+| 6 | axis_z          | Value of axis Z |
+| 7 | accuracy        | Sensor accuracy |
+
 
 ## Author
 
 [Rafael J P Damaceno](https://github.com/rafaelpezzuto)
 
 
 ## About us
```

