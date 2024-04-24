# Comparing `tmp/misleep-0.2.3b0.tar.gz` & `tmp/misleep-0.2.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misleep-0.2.3b0.tar", last modified: Sun Apr 21 09:38:41 2024, max compression
+gzip compressed data, was "misleep-0.2.4b0.tar", last modified: Wed Apr 24 09:48:37 2024, max compression
```

## Comparing `misleep-0.2.3b0.tar` & `misleep-0.2.4b0.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 09:38:41.908608 misleep-0.2.3b0/
--rw-rw-rw-   0        0        0     1549 2024-03-05 06:19:17.000000 misleep-0.2.3b0/LICENSE
--rw-rw-rw-   0        0        0     3058 2024-04-21 09:38:41.907609 misleep-0.2.3b0/PKG-INFO
--rw-rw-rw-   0        0        0     1960 2024-04-17 11:42:46.000000 misleep-0.2.3b0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 09:38:41.885995 misleep-0.2.3b0/misleep/
--rw-rw-rw-   0        0        0      215 2024-03-27 05:19:22.000000 misleep-0.2.3b0/misleep/__init__.py
--rw-rw-rw-   0        0        0      167 2024-04-15 03:11:05.000000 misleep-0.2.3b0/misleep/__main__.py
--rw-rw-rw-   0        0        0      528 2024-04-21 09:33:59.000000 misleep-0.2.3b0/misleep/config.ini
-drwxrwxrwx   0        0        0        0 2024-04-21 09:38:41.891604 misleep-0.2.3b0/misleep/gui/
--rw-rw-rw-   0        0        0      334 2024-04-15 03:11:05.000000 misleep-0.2.3b0/misleep/gui/__init__.py
--rw-rw-rw-   0        0        0      808 2024-04-01 05:02:43.000000 misleep-0.2.3b0/misleep/gui/about.py
--rw-rw-rw-   0        0        0     7542 2024-04-21 09:29:39.000000 misleep-0.2.3b0/misleep/gui/dialog.py
--rw-rw-rw-   0        0        0    56484 2024-04-17 11:23:33.000000 misleep-0.2.3b0/misleep/gui/main_window.py
-drwxrwxrwx   0        0        0        0 2024-04-21 09:38:41.894608 misleep-0.2.3b0/misleep/gui/resources/
--rw-rw-rw-   0        0        0       47 2024-04-15 03:11:05.000000 misleep-0.2.3b0/misleep/gui/resources/__init__.py
--rw-rw-rw-   0        0        0     9826 2024-03-13 06:17:48.000000 misleep-0.2.3b0/misleep/gui/resources/entire_logo.png
--rw-rw-rw-   0        0        0     2670 2024-03-13 06:17:48.000000 misleep-0.2.3b0/misleep/gui/resources/logo.png
--rw-rw-rw-   0        0        0    54154 2024-04-02 09:29:51.000000 misleep-0.2.3b0/misleep/gui/resources/misleep.py
--rw-rw-rw-   0        0        0      121 2024-03-13 06:17:48.000000 misleep-0.2.3b0/misleep/gui/resources/misleep.qrc
--rw-rw-rw-   0        0        0      476 2024-04-15 10:19:04.000000 misleep-0.2.3b0/misleep/gui/show.py
--rw-rw-rw-   0        0        0     5893 2024-04-15 03:11:05.000000 misleep-0.2.3b0/misleep/gui/spec_window.py
--rw-rw-rw-   0        0        0     3177 2024-04-15 03:11:05.000000 misleep-0.2.3b0/misleep/gui/thread.py
-drwxrwxrwx   0        0        0        0 2024-04-21 09:38:41.896607 misleep-0.2.3b0/misleep/gui/uis/
--rw-rw-rw-   0        0        0      228 2024-03-13 06:17:48.000000 misleep-0.2.3b0/misleep/gui/uis/__init__.py
--rw-rw-rw-   0        0        0     2921 2024-03-13 06:17:48.000000 misleep-0.2.3b0/misleep/gui/uis/about_ui.py
--rw-rw-rw-   0        0        0     2207 2024-04-01 05:02:43.000000 misleep-0.2.3b0/misleep/gui/uis/label_dialog_ui.py
--rw-rw-rw-   0        0        0    24912 2024-04-17 03:11:18.000000 misleep-0.2.3b0/misleep/gui/uis/main_window_ui.py
--rw-rw-rw-   0        0        0     2371 2024-04-15 03:11:05.000000 misleep-0.2.3b0/misleep/gui/uis/save_data_dialog_ui.py
--rw-rw-rw-   0        0        0     4466 2024-04-15 03:11:05.000000 misleep-0.2.3b0/misleep/gui/uis/spec_window_ui.py
--rw-rw-rw-   0        0        0     4884 2024-04-17 11:15:15.000000 misleep-0.2.3b0/misleep/gui/uis/transfer_result_dialog_ui.py
--rw-rw-rw-   0        0        0     3441 2024-04-15 03:11:05.000000 misleep-0.2.3b0/misleep/gui/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-21 09:38:41.899607 misleep-0.2.3b0/misleep/io/
--rw-rw-rw-   0        0        0      215 2024-03-06 08:30:45.000000 misleep-0.2.3b0/misleep/io/__init__.py
--rw-rw-rw-   0        0        0     7578 2024-04-21 09:27:40.000000 misleep-0.2.3b0/misleep/io/annotation_io.py
--rw-rw-rw-   0        0        0    14995 2024-04-15 03:11:05.000000 misleep-0.2.3b0/misleep/io/base.py
--rw-rw-rw-   0        0        0     5027 2024-04-17 08:38:52.000000 misleep-0.2.3b0/misleep/io/signal_io.py
-drwxrwxrwx   0        0        0        0 2024-04-21 09:38:41.901607 misleep-0.2.3b0/misleep/preprocessing/
--rw-rw-rw-   0        0        0      163 2024-03-05 07:42:23.000000 misleep-0.2.3b0/misleep/preprocessing/__init__.py
--rw-rw-rw-   0        0        0      338 2024-03-05 07:42:23.000000 misleep-0.2.3b0/misleep/preprocessing/channel.py
--rw-rw-rw-   0        0        0      458 2024-04-15 10:35:14.000000 misleep-0.2.3b0/misleep/preprocessing/signals.py
--rw-rw-rw-   0        0        0     4898 2024-03-31 07:18:43.000000 misleep-0.2.3b0/misleep/preprocessing/spectral.py
-drwxrwxrwx   0        0        0        0 2024-04-21 09:38:41.902607 misleep-0.2.3b0/misleep/utils/
--rw-rw-rw-   0        0        0      187 2024-03-06 08:30:45.000000 misleep-0.2.3b0/misleep/utils/__init__.py
--rw-rw-rw-   0        0        0     4394 2024-04-15 03:11:05.000000 misleep-0.2.3b0/misleep/utils/annotation.py
--rw-rw-rw-   0        0        0     2324 2024-03-13 06:17:48.000000 misleep-0.2.3b0/misleep/utils/signals.py
-drwxrwxrwx   0        0        0        0 2024-04-21 09:38:41.903607 misleep-0.2.3b0/misleep/viz/
--rw-rw-rw-   0        0        0      211 2024-03-06 08:30:45.000000 misleep-0.2.3b0/misleep/viz/__init__.py
--rw-rw-rw-   0        0        0     1164 2024-03-07 13:29:48.000000 misleep-0.2.3b0/misleep/viz/hypnogram.py
--rw-rw-rw-   0        0        0     1668 2024-03-07 13:29:48.000000 misleep-0.2.3b0/misleep/viz/signals.py
--rw-rw-rw-   0        0        0     1508 2024-03-13 06:17:48.000000 misleep-0.2.3b0/misleep/viz/spectral.py
-drwxrwxrwx   0        0        0        0 2024-04-21 09:38:41.887995 misleep-0.2.3b0/misleep.egg-info/
--rw-rw-rw-   0        0        0     3058 2024-04-21 09:38:41.000000 misleep-0.2.3b0/misleep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1401 2024-04-21 09:38:41.000000 misleep-0.2.3b0/misleep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 09:38:41.000000 misleep-0.2.3b0/misleep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-04-21 09:38:41.000000 misleep-0.2.3b0/misleep.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-21 09:38:41.000000 misleep-0.2.3b0/misleep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 09:38:41.908608 misleep-0.2.3b0/setup.cfg
--rw-rw-rw-   0        0        0     2154 2024-04-21 09:34:06.000000 misleep-0.2.3b0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 09:38:41.907609 misleep-0.2.3b0/test/
--rw-rw-rw-   0        0        0      473 2024-03-06 08:30:45.000000 misleep-0.2.3b0/test/test_annotation_io.py
--rw-rw-rw-   0        0        0      143 2024-04-15 03:11:05.000000 misleep-0.2.3b0/test/test_loadmat73.py
--rw-rw-rw-   0        0        0     1828 2024-03-13 06:17:48.000000 misleep-0.2.3b0/test/test_midata.py
--rw-rw-rw-   0        0        0      275 2024-03-28 08:11:15.000000 misleep-0.2.3b0/test/test_show.py
--rw-rw-rw-   0        0        0     1488 2024-04-15 03:11:05.000000 misleep-0.2.3b0/test/test_signal_io.py
--rw-rw-rw-   0        0        0      603 2024-03-07 13:29:48.000000 misleep-0.2.3b0/test/test_signals_viz.py
--rw-rw-rw-   0        0        0     1253 2024-03-06 08:30:45.000000 misleep-0.2.3b0/test/test_spectral_viz.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:48:37.709402 misleep-0.2.4b0/
+-rw-rw-rw-   0        0        0     1549 2024-03-05 06:19:17.000000 misleep-0.2.4b0/LICENSE
+-rw-rw-rw-   0        0        0     3079 2024-04-24 09:48:37.708402 misleep-0.2.4b0/PKG-INFO
+-rw-rw-rw-   0        0        0     1960 2024-04-17 11:42:46.000000 misleep-0.2.4b0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 09:48:37.684402 misleep-0.2.4b0/misleep/
+-rw-rw-rw-   0        0        0      215 2024-03-27 05:19:22.000000 misleep-0.2.4b0/misleep/__init__.py
+-rw-rw-rw-   0        0        0      167 2024-04-15 03:11:05.000000 misleep-0.2.4b0/misleep/__main__.py
+-rw-rw-rw-   0        0        0      528 2024-04-24 09:48:01.000000 misleep-0.2.4b0/misleep/config.ini
+drwxrwxrwx   0        0        0        0 2024-04-24 09:48:37.691402 misleep-0.2.4b0/misleep/gui/
+-rw-rw-rw-   0        0        0      334 2024-04-15 03:11:05.000000 misleep-0.2.4b0/misleep/gui/__init__.py
+-rw-rw-rw-   0        0        0      808 2024-04-01 05:02:43.000000 misleep-0.2.4b0/misleep/gui/about.py
+-rw-rw-rw-   0        0        0    13965 2024-04-24 09:46:39.000000 misleep-0.2.4b0/misleep/gui/dialog.py
+-rw-rw-rw-   0        0        0    57175 2024-04-24 08:12:38.000000 misleep-0.2.4b0/misleep/gui/main_window.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:48:37.694403 misleep-0.2.4b0/misleep/gui/resources/
+-rw-rw-rw-   0        0        0       47 2024-04-15 03:11:05.000000 misleep-0.2.4b0/misleep/gui/resources/__init__.py
+-rw-rw-rw-   0        0        0     9826 2024-03-13 06:17:48.000000 misleep-0.2.4b0/misleep/gui/resources/entire_logo.png
+-rw-rw-rw-   0        0        0     2670 2024-03-13 06:17:48.000000 misleep-0.2.4b0/misleep/gui/resources/logo.png
+-rw-rw-rw-   0        0        0    54154 2024-04-02 09:29:51.000000 misleep-0.2.4b0/misleep/gui/resources/misleep.py
+-rw-rw-rw-   0        0        0      121 2024-03-13 06:17:48.000000 misleep-0.2.4b0/misleep/gui/resources/misleep.qrc
+-rw-rw-rw-   0        0        0      476 2024-04-15 10:19:04.000000 misleep-0.2.4b0/misleep/gui/show.py
+-rw-rw-rw-   0        0        0     5893 2024-04-15 03:11:05.000000 misleep-0.2.4b0/misleep/gui/spec_window.py
+-rw-rw-rw-   0        0        0     3177 2024-04-24 08:07:23.000000 misleep-0.2.4b0/misleep/gui/thread.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:48:37.697402 misleep-0.2.4b0/misleep/gui/uis/
+-rw-rw-rw-   0        0        0      228 2024-03-13 06:17:48.000000 misleep-0.2.4b0/misleep/gui/uis/__init__.py
+-rw-rw-rw-   0        0        0     2921 2024-03-13 06:17:48.000000 misleep-0.2.4b0/misleep/gui/uis/about_ui.py
+-rw-rw-rw-   0        0        0     2207 2024-04-01 05:02:43.000000 misleep-0.2.4b0/misleep/gui/uis/label_dialog_ui.py
+-rw-rw-rw-   0        0        0    25023 2024-04-24 06:10:23.000000 misleep-0.2.4b0/misleep/gui/uis/main_window_ui.py
+-rw-rw-rw-   0        0        0     2371 2024-04-15 03:11:05.000000 misleep-0.2.4b0/misleep/gui/uis/save_data_dialog_ui.py
+-rw-rw-rw-   0        0        0     4466 2024-04-15 03:11:05.000000 misleep-0.2.4b0/misleep/gui/uis/spec_window_ui.py
+-rw-rw-rw-   0        0        0     4513 2024-04-24 09:43:30.000000 misleep-0.2.4b0/misleep/gui/uis/state_spectral_dialog_ui.py
+-rw-rw-rw-   0        0        0     3917 2024-04-24 06:08:06.000000 misleep-0.2.4b0/misleep/gui/uis/transfer_result_dialog_ui.py
+-rw-rw-rw-   0        0        0     5126 2024-04-24 08:00:47.000000 misleep-0.2.4b0/misleep/gui/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:48:37.699402 misleep-0.2.4b0/misleep/io/
+-rw-rw-rw-   0        0        0      215 2024-03-06 08:30:45.000000 misleep-0.2.4b0/misleep/io/__init__.py
+-rw-rw-rw-   0        0        0     7578 2024-04-21 09:27:40.000000 misleep-0.2.4b0/misleep/io/annotation_io.py
+-rw-rw-rw-   0        0        0    14995 2024-04-15 03:11:05.000000 misleep-0.2.4b0/misleep/io/base.py
+-rw-rw-rw-   0        0        0     5027 2024-04-17 08:38:52.000000 misleep-0.2.4b0/misleep/io/signal_io.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:48:37.700402 misleep-0.2.4b0/misleep/preprocessing/
+-rw-rw-rw-   0        0        0      163 2024-03-05 07:42:23.000000 misleep-0.2.4b0/misleep/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0      338 2024-03-05 07:42:23.000000 misleep-0.2.4b0/misleep/preprocessing/channel.py
+-rw-rw-rw-   0        0        0     2175 2024-04-24 09:42:26.000000 misleep-0.2.4b0/misleep/preprocessing/signals.py
+-rw-rw-rw-   0        0        0     4898 2024-03-31 07:18:43.000000 misleep-0.2.4b0/misleep/preprocessing/spectral.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:48:37.701402 misleep-0.2.4b0/misleep/utils/
+-rw-rw-rw-   0        0        0      187 2024-03-06 08:30:45.000000 misleep-0.2.4b0/misleep/utils/__init__.py
+-rw-rw-rw-   0        0        0     4394 2024-04-15 03:11:05.000000 misleep-0.2.4b0/misleep/utils/annotation.py
+-rw-rw-rw-   0        0        0     2324 2024-03-13 06:17:48.000000 misleep-0.2.4b0/misleep/utils/signals.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:48:37.704403 misleep-0.2.4b0/misleep/viz/
+-rw-rw-rw-   0        0        0      211 2024-03-06 08:30:45.000000 misleep-0.2.4b0/misleep/viz/__init__.py
+-rw-rw-rw-   0        0        0     1164 2024-03-07 13:29:48.000000 misleep-0.2.4b0/misleep/viz/hypnogram.py
+-rw-rw-rw-   0        0        0     1668 2024-03-07 13:29:48.000000 misleep-0.2.4b0/misleep/viz/signals.py
+-rw-rw-rw-   0        0        0     1508 2024-03-13 06:17:48.000000 misleep-0.2.4b0/misleep/viz/spectral.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:48:37.686402 misleep-0.2.4b0/misleep.egg-info/
+-rw-rw-rw-   0        0        0     3079 2024-04-24 09:48:37.000000 misleep-0.2.4b0/misleep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1445 2024-04-24 09:48:37.000000 misleep-0.2.4b0/misleep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 09:48:37.000000 misleep-0.2.4b0/misleep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2024-04-24 09:48:37.000000 misleep-0.2.4b0/misleep.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-24 09:48:37.000000 misleep-0.2.4b0/misleep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 09:48:37.709402 misleep-0.2.4b0/setup.cfg
+-rw-rw-rw-   0        0        0     2167 2024-04-24 09:47:56.000000 misleep-0.2.4b0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:48:37.708402 misleep-0.2.4b0/test/
+-rw-rw-rw-   0        0        0      473 2024-03-06 08:30:45.000000 misleep-0.2.4b0/test/test_annotation_io.py
+-rw-rw-rw-   0        0        0      143 2024-04-15 03:11:05.000000 misleep-0.2.4b0/test/test_loadmat73.py
+-rw-rw-rw-   0        0        0     1828 2024-03-13 06:17:48.000000 misleep-0.2.4b0/test/test_midata.py
+-rw-rw-rw-   0        0        0      275 2024-03-28 08:11:15.000000 misleep-0.2.4b0/test/test_show.py
+-rw-rw-rw-   0        0        0     1488 2024-04-15 03:11:05.000000 misleep-0.2.4b0/test/test_signal_io.py
+-rw-rw-rw-   0        0        0      603 2024-03-07 13:29:48.000000 misleep-0.2.4b0/test/test_signals_viz.py
+-rw-rw-rw-   0        0        0     1253 2024-03-06 08:30:45.000000 misleep-0.2.4b0/test/test_spectral_viz.py
```

### Comparing `misleep-0.2.3b0/LICENSE` & `misleep-0.2.4b0/LICENSE`

 * *Files identical despite different names*

### Comparing `misleep-0.2.3b0/PKG-INFO` & `misleep-0.2.4b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misleep
-Version: 0.2.3b0
+Version: 0.2.4b0
 Summary: MiSleep: Mice Sleep EEG/EMG visualization, scoring and analysis.
 Home-page: https://github.com/BryanWang0702/MiSleep/
 Download-URL: https://github.com/BryanWang0702/MiSleep/
 Author: Xueqiang Wang
 Author-email: swang@gmail.com
 Maintainer: Xueqiang Wang
 Maintainer-email: swang@gmail.com
@@ -25,14 +25,15 @@
 Requires-Dist: scipy
 Requires-Dist: pyedflib
 Requires-Dist: hdf5storage
 Requires-Dist: pyqt5
 Requires-Dist: mat73
 Requires-Dist: pandas
 Requires-Dist: openpyxl
+Requires-Dist: yasa
 
 # MiSleep
 MiSleep is for EEG/EMG signal processing and visualization
 
 ![logo](resources/entire_logo.png)
 
 ## Get start
```

### Comparing `misleep-0.2.3b0/README.md` & `misleep-0.2.4b0/README.md`

 * *Files identical despite different names*

### Comparing `misleep-0.2.3b0/misleep/config.ini` & `misleep-0.2.4b0/misleep/config.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [gui]
-version = v0.2.3 Beta
+version = v0.2.4 Beta
 updatetime = 2024/04/01
 marker = ['pat', 'add water', 'third']
 startend = ['SWA', 'SWA', 'start end label', 'start end label', 'start end label', 'start end label', 'start end label']
 statemap = {"1": "NREM", "2": "REM", "3": "Wake", "4": "INIT"}
 statecolor = {"1": "orange", "2": "skyblue", "3": "red", "4": "white"}
 statecolorbgalpha = 0.1
 markerlinecolor = "red"
```

### Comparing `misleep-0.2.3b0/misleep/gui/about.py` & `misleep-0.2.4b0/misleep/gui/about.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.3b0/misleep/gui/main_window.py` & `misleep-0.2.4b0/misleep/gui/main_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from misleep.preprocessing.spectral import spectrogram
 from misleep.io.base import MiData, MiAnnotation
 from misleep.io.signal_io import load_mat, load_edf
 from misleep.io.annotation_io import load_misleep_anno, load_bio_anno
 from misleep.gui.utils import create_new_mianno
 from misleep.utils.annotation import lst2group
 from misleep.gui.about import about_dialog
-from misleep.gui.dialog import label_dialog, transferResult_dialog
+from misleep.gui.dialog import label_dialog, transferResult_dialog, stateSpectral_dialog
 from misleep.gui.spec_window import SpecWindow
 from misleep.gui.uis.main_window_ui import Ui_MiSleep
 from misleep.preprocessing.spectral import spectrogram, spectrum, band_power
 from misleep.gui.thread import SaveThread
 
 
 class main_window(QMainWindow, Ui_MiSleep):
@@ -117,14 +117,17 @@
         self.spec_window = SpecWindow()
         # Initial label dialog
         self.label_dialog = label_dialog(config=self.config)
 
         # Initial transfer result dialog
         self.transfer_result_dialog = transferResult_dialog()
 
+        # Initial state spectral dialog
+        self.state_spectral_dialog = stateSpectral_dialog()
+
         # Check wheher operation done and saved or not
         self.is_saved = True
 
         # Timer to auto save annotations
         self.save_timer = QTimer()
         self.save_timer.timeout.connect(self.auto_save)
 
@@ -1342,27 +1345,40 @@
         if signal.text() == "Save Data":
             self.save_data()
         if signal.text() == "Save Annotation":
             self.save_anno()
 
     def tool_bar_dispatcher(self, signal):
         """Triggered by ToolBar action, transfer result"""
+        if signal.text() == "State Spectral":
+            self.state_spectral()
         if signal.text() == "Transfer Result":
             self.transfer_result()
 
     def transfer_result(self):
         """Transfer result into file"""
         self.transfer_result_dialog.ACTimeEditor.setDateTime(self.ac_time)
         self.transfer_result_dialog.TransferStartTimeEdit.setDateTime(self.ac_time)
-        self.transfer_result_dialog.exec_()
-        if self.label_dialog.closed:
+        self.transfer_result_dialog.exec()
+        if self.transfer_result_dialog.closed:
             return
         self.transfer_result_dialog.transfer(config=self.config,
                                              mianno=self.mianno,
                                              ac_time=self.midata.time)
+        
+    def state_spectral(self):
+        """Analyze state spectral"""
+        self.state_spectral_dialog.dialog_show(channels=self.midata.channels)
+        self.state_spectral_dialog.exec()
+        if self.state_spectral_dialog.closed:
+            return
+        self.state_spectral_dialog.spectral_analysis(midata=self.midata,
+                                            mianno=self.mianno,
+                                            config=self.config)
+
 
     def save_anno(self):
         """Save annotation into file"""
         save_thread = SaveThread(file=[self.mianno, self.midata], 
                                  file_path=self.anno_path)
         saved = save_thread.save_anno()
         if saved:
```

### Comparing `misleep-0.2.3b0/misleep/gui/resources/entire_logo.png` & `misleep-0.2.4b0/misleep/gui/resources/entire_logo.png`

 * *Files identical despite different names*

### Comparing `misleep-0.2.3b0/misleep/gui/resources/logo.png` & `misleep-0.2.4b0/misleep/gui/resources/logo.png`

 * *Files identical despite different names*

### Comparing `misleep-0.2.3b0/misleep/gui/resources/misleep.py` & `misleep-0.2.4b0/misleep/gui/resources/misleep.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.3b0/misleep/gui/spec_window.py` & `misleep-0.2.4b0/misleep/gui/spec_window.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.3b0/misleep/gui/thread.py` & `misleep-0.2.4b0/misleep/gui/thread.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.3b0/misleep/gui/uis/about_ui.py` & `misleep-0.2.4b0/misleep/gui/uis/about_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.3b0/misleep/gui/uis/label_dialog_ui.py` & `misleep-0.2.4b0/misleep/gui/uis/label_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.3b0/misleep/gui/uis/main_window_ui.py` & `misleep-0.2.4b0/misleep/gui/uis/main_window_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,30 +323,30 @@
         self.actionShow.setObjectName("actionShow")
         self.actionSave_data = QtWidgets.QAction(MiSleep)
         self.actionSave_data.setObjectName("actionSave_data")
         self.actionSave_Annotation = QtWidgets.QAction(MiSleep)
         self.actionSave_Annotation.setObjectName("actionSave_Annotation")
         self.actionAbout = QtWidgets.QAction(MiSleep)
         self.actionAbout.setObjectName("actionAbout")
-        self.actionMerge_Data = QtWidgets.QAction(MiSleep)
-        self.actionMerge_Data.setObjectName("actionMerge_Data")
+        self.actionState_Spectral = QtWidgets.QAction(MiSleep)
+        self.actionState_Spectral.setObjectName("actionState_Spectral")
         self.actionTransfer_Result = QtWidgets.QAction(MiSleep)
         self.actionTransfer_Result.setObjectName("actionTransfer_Result")
         self.LoadBar.addAction(self.actionLoad_Data)
         self.LoadBar.addSeparator()
         self.LoadBar.addAction(self.actionLoad_Annotation)
         self.LoadBar.addSeparator()
         self.LoadBar.addAction(self.actionShow)
         self.LoadBar.addSeparator()
         self.SaveBar.addAction(self.actionSave_data)
         self.SaveBar.addSeparator()
         self.SaveBar.addAction(self.actionSave_Annotation)
         self.SaveBar.addSeparator()
         self.AboutBar.addAction(self.actionAbout)
-        self.ToolBar.addAction(self.actionMerge_Data)
+        self.ToolBar.addAction(self.actionState_Spectral)
         self.ToolBar.addSeparator()
         self.ToolBar.addAction(self.actionTransfer_Result)
         self.ToolBar.addSeparator()
 
         self.retranslateUi(MiSleep)
         QtCore.QMetaObject.connectSlotsByName(MiSleep)
 
@@ -400,11 +400,12 @@
         self.ToolBar.setWindowTitle(_translate("MiSleep", "toolBar"))
         self.actionLoad_Data.setText(_translate("MiSleep", "Load Data"))
         self.actionLoad_Annotation.setText(_translate("MiSleep", "Load Annotation"))
         self.actionShow.setText(_translate("MiSleep", "Show"))
         self.actionSave_data.setText(_translate("MiSleep", "Save Data"))
         self.actionSave_Annotation.setText(_translate("MiSleep", "Save Annotation"))
         self.actionAbout.setText(_translate("MiSleep", "About"))
-        self.actionMerge_Data.setText(_translate("MiSleep", "Merge Data"))
+        self.actionState_Spectral.setText(_translate("MiSleep", "State Spectral"))
+        self.actionState_Spectral.setToolTip(_translate("MiSleep", "State Spectral"))
         self.actionTransfer_Result.setText(_translate("MiSleep", "Transfer Result"))
         self.actionTransfer_Result.setToolTip(_translate("MiSleep", "Transfer Result"))
 from misleep.gui.resources import misleep
```

### Comparing `misleep-0.2.3b0/misleep/gui/uis/save_data_dialog_ui.py` & `misleep-0.2.4b0/misleep/gui/uis/save_data_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.3b0/misleep/gui/uis/spec_window_ui.py` & `misleep-0.2.4b0/misleep/gui/uis/spec_window_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.3b0/misleep/gui/uis/transfer_result_dialog_ui.py` & `misleep-0.2.4b0/misleep/gui/uis/state_spectral_dialog_ui.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,76 +1,82 @@
 # -*- coding: utf-8 -*-
 
-# Form implementation generated from reading ui file 'misleep/gui/uis/transfer_result_dialog.ui'
+# Form implementation generated from reading ui file 'misleep/gui/uis/state_spectral_dialog.ui'
 #
 # Created by: PyQt5 UI code generator 5.15.10
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
-class Ui_TransferResultDialog(object):
-    def setupUi(self, TransferResultDialog):
-        TransferResultDialog.setObjectName("TransferResultDialog")
-        TransferResultDialog.resize(278, 290)
-        self.verticalLayout = QtWidgets.QVBoxLayout(TransferResultDialog)
-        self.verticalLayout.setObjectName("verticalLayout")
-        self.groupBox = QtWidgets.QGroupBox(TransferResultDialog)
+class Ui_StateSpectralDialog(object):
+    def setupUi(self, StateSpectralDialog):
+        StateSpectralDialog.setObjectName("StateSpectralDialog")
+        StateSpectralDialog.resize(261, 255)
+        self.gridLayout_2 = QtWidgets.QGridLayout(StateSpectralDialog)
+        self.gridLayout_2.setObjectName("gridLayout_2")
+        self.groupBox = QtWidgets.QGroupBox(StateSpectralDialog)
         self.groupBox.setObjectName("groupBox")
         self.gridLayout = QtWidgets.QGridLayout(self.groupBox)
+        self.gridLayout.setSpacing(10)
         self.gridLayout.setObjectName("gridLayout")
-        self.line = QtWidgets.QFrame(self.groupBox)
-        self.line.setFrameShape(QtWidgets.QFrame.HLine)
-        self.line.setFrameShadow(QtWidgets.QFrame.Sunken)
-        self.line.setObjectName("line")
-        self.gridLayout.addWidget(self.line, 5, 0, 1, 2)
+        self.label = QtWidgets.QLabel(self.groupBox)
+        self.label.setObjectName("label")
+        self.gridLayout.addWidget(self.label, 0, 0, 1, 1)
+        self.BPHigh = QtWidgets.QDoubleSpinBox(self.groupBox)
+        self.BPHigh.setDecimals(1)
+        self.BPHigh.setMaximum(10000.0)
+        self.BPHigh.setSingleStep(0.1)
+        self.BPHigh.setProperty("value", 30.0)
+        self.BPHigh.setObjectName("BPHigh")
+        self.gridLayout.addWidget(self.BPHigh, 5, 1, 1, 1)
+        self.BPFilterCheckBox = QtWidgets.QCheckBox(self.groupBox)
+        self.BPFilterCheckBox.setObjectName("BPFilterCheckBox")
+        self.gridLayout.addWidget(self.BPFilterCheckBox, 4, 0, 1, 1)
+        self.ChannelSelector = QtWidgets.QComboBox(self.groupBox)
+        self.ChannelSelector.setObjectName("ChannelSelector")
+        self.gridLayout.addWidget(self.ChannelSelector, 1, 0, 1, 2)
+        self.BPLow = QtWidgets.QDoubleSpinBox(self.groupBox)
+        self.BPLow.setDecimals(1)
+        self.BPLow.setMaximum(100000.0)
+        self.BPLow.setSingleStep(0.1)
+        self.BPLow.setProperty("value", 0.5)
+        self.BPLow.setObjectName("BPLow")
+        self.gridLayout.addWidget(self.BPLow, 5, 0, 1, 1)
         self.RejectArtifactCheckBox = QtWidgets.QCheckBox(self.groupBox)
         self.RejectArtifactCheckBox.setObjectName("RejectArtifactCheckBox")
         self.gridLayout.addWidget(self.RejectArtifactCheckBox, 7, 0, 1, 1)
-        self.ContainEventsCheckBox = QtWidgets.QCheckBox(self.groupBox)
-        self.ContainEventsCheckBox.setObjectName("ContainEventsCheckBox")
-        self.gridLayout.addWidget(self.ContainEventsCheckBox, 4, 0, 1, 1)
-        self.StateSpecAnalysisCheckBox = QtWidgets.QCheckBox(self.groupBox)
-        self.StateSpecAnalysisCheckBox.setObjectName("StateSpecAnalysisCheckBox")
-        self.gridLayout.addWidget(self.StateSpecAnalysisCheckBox, 6, 0, 1, 1)
-        self.ACTimeEditor = QtWidgets.QDateTimeEdit(self.groupBox)
-        self.ACTimeEditor.setObjectName("ACTimeEditor")
-        self.gridLayout.addWidget(self.ACTimeEditor, 1, 0, 1, 1)
-        self.ResetTimeCheckBox = QtWidgets.QCheckBox(self.groupBox)
-        self.ResetTimeCheckBox.setObjectName("ResetTimeCheckBox")
-        self.gridLayout.addWidget(self.ResetTimeCheckBox, 0, 0, 1, 1)
-        self.ResetTransferStartTimeCheckBox = QtWidgets.QCheckBox(self.groupBox)
-        self.ResetTransferStartTimeCheckBox.setObjectName("ResetTransferStartTimeCheckBox")
-        self.gridLayout.addWidget(self.ResetTransferStartTimeCheckBox, 2, 0, 1, 1)
-        spacerItem = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
-        self.gridLayout.addItem(spacerItem, 1, 1, 1, 1)
-        self.TransferStartTimeEdit = QtWidgets.QDateTimeEdit(self.groupBox)
-        self.TransferStartTimeEdit.setObjectName("TransferStartTimeEdit")
-        self.gridLayout.addWidget(self.TransferStartTimeEdit, 3, 0, 1, 1)
-        spacerItem1 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
-        self.gridLayout.addItem(spacerItem1, 3, 1, 1, 1)
-        self.verticalLayout.addWidget(self.groupBox)
-        self.buttonBox = QtWidgets.QDialogButtonBox(TransferResultDialog)
-        self.buttonBox.setOrientation(QtCore.Qt.Horizontal)
-        self.buttonBox.setStandardButtons(QtWidgets.QDialogButtonBox.Cancel|QtWidgets.QDialogButtonBox.Ok)
-        self.buttonBox.setObjectName("buttonBox")
-        self.verticalLayout.addWidget(self.buttonBox)
-
-        self.retranslateUi(TransferResultDialog)
-        self.buttonBox.accepted.connect(TransferResultDialog.accept) # type: ignore
-        self.buttonBox.rejected.connect(TransferResultDialog.reject) # type: ignore
-        QtCore.QMetaObject.connectSlotsByName(TransferResultDialog)
+        self.RelativeCheckBox = QtWidgets.QCheckBox(self.groupBox)
+        self.RelativeCheckBox.setObjectName("RelativeCheckBox")
+        self.gridLayout.addWidget(self.RelativeCheckBox, 6, 0, 1, 1)
+        self.MergeDataCheckBox = QtWidgets.QCheckBox(self.groupBox)
+        self.MergeDataCheckBox.setObjectName("MergeDataCheckBox")
+        self.gridLayout.addWidget(self.MergeDataCheckBox, 8, 0, 1, 1)
+        self.ArtThresholdSpinBox = QtWidgets.QDoubleSpinBox(self.groupBox)
+        self.ArtThresholdSpinBox.setDecimals(1)
+        self.ArtThresholdSpinBox.setObjectName("ArtThresholdSpinBox")
+        self.gridLayout.addWidget(self.ArtThresholdSpinBox, 7, 1, 1, 1)
+        self.gridLayout_2.addWidget(self.groupBox, 0, 0, 1, 2)
+        self.OKBt = QtWidgets.QPushButton(StateSpectralDialog)
+        self.OKBt.setObjectName("OKBt")
+        self.gridLayout_2.addWidget(self.OKBt, 1, 0, 1, 1)
+        self.CancelBt = QtWidgets.QPushButton(StateSpectralDialog)
+        self.CancelBt.setObjectName("CancelBt")
+        self.gridLayout_2.addWidget(self.CancelBt, 1, 1, 1, 1)
 
-    def retranslateUi(self, TransferResultDialog):
+        self.retranslateUi(StateSpectralDialog)
+        QtCore.QMetaObject.connectSlotsByName(StateSpectralDialog)
+
+    def retranslateUi(self, StateSpectralDialog):
         _translate = QtCore.QCoreApplication.translate
-        TransferResultDialog.setWindowTitle(_translate("TransferResultDialog", "Dialog"))
-        self.groupBox.setTitle(_translate("TransferResultDialog", "Transfer result options"))
-        self.RejectArtifactCheckBox.setText(_translate("TransferResultDialog", "Reject artifact"))
-        self.ContainEventsCheckBox.setText(_translate("TransferResultDialog", "Contain Start-End events"))
-        self.StateSpecAnalysisCheckBox.setText(_translate("TransferResultDialog", "State spectral analysis"))
-        self.ACTimeEditor.setDisplayFormat(_translate("TransferResultDialog", "yyyy/MM/dd HH:mm:ss"))
-        self.ResetTimeCheckBox.setText(_translate("TransferResultDialog", "Reset acquisition time"))
-        self.ResetTransferStartTimeCheckBox.setText(_translate("TransferResultDialog", "Reset transfer start time"))
-        self.TransferStartTimeEdit.setDisplayFormat(_translate("TransferResultDialog", "yyyy/MM/dd HH:mm:ss"))
+        StateSpectralDialog.setWindowTitle(_translate("StateSpectralDialog", "Dialog"))
+        self.groupBox.setTitle(_translate("StateSpectralDialog", "State spectral analysis options"))
+        self.label.setText(_translate("StateSpectralDialog", "Channel:"))
+        self.BPFilterCheckBox.setText(_translate("StateSpectralDialog", "Bandpass filter"))
+        self.RejectArtifactCheckBox.setText(_translate("StateSpectralDialog", "Reject artifact"))
+        self.RelativeCheckBox.setText(_translate("StateSpectralDialog", "Relative"))
+        self.MergeDataCheckBox.setText(_translate("StateSpectralDialog", "Merge data"))
+        self.OKBt.setText(_translate("StateSpectralDialog", "OK"))
+        self.CancelBt.setText(_translate("StateSpectralDialog", "Cancel"))
```

### Comparing `misleep-0.2.3b0/misleep/io/annotation_io.py` & `misleep-0.2.4b0/misleep/io/annotation_io.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.3b0/misleep/io/base.py` & `misleep-0.2.4b0/misleep/io/base.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.3b0/misleep/io/signal_io.py` & `misleep-0.2.4b0/misleep/io/signal_io.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.3b0/misleep/preprocessing/spectral.py` & `misleep-0.2.4b0/misleep/preprocessing/spectral.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.3b0/misleep/utils/annotation.py` & `misleep-0.2.4b0/misleep/utils/annotation.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.3b0/misleep/utils/signals.py` & `misleep-0.2.4b0/misleep/utils/signals.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.3b0/misleep/viz/hypnogram.py` & `misleep-0.2.4b0/misleep/viz/hypnogram.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.3b0/misleep/viz/signals.py` & `misleep-0.2.4b0/misleep/viz/signals.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.3b0/misleep/viz/spectral.py` & `misleep-0.2.4b0/misleep/viz/spectral.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.3b0/misleep.egg-info/PKG-INFO` & `misleep-0.2.4b0/misleep.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misleep
-Version: 0.2.3b0
+Version: 0.2.4b0
 Summary: MiSleep: Mice Sleep EEG/EMG visualization, scoring and analysis.
 Home-page: https://github.com/BryanWang0702/MiSleep/
 Download-URL: https://github.com/BryanWang0702/MiSleep/
 Author: Xueqiang Wang
 Author-email: swang@gmail.com
 Maintainer: Xueqiang Wang
 Maintainer-email: swang@gmail.com
@@ -25,14 +25,15 @@
 Requires-Dist: scipy
 Requires-Dist: pyedflib
 Requires-Dist: hdf5storage
 Requires-Dist: pyqt5
 Requires-Dist: mat73
 Requires-Dist: pandas
 Requires-Dist: openpyxl
+Requires-Dist: yasa
 
 # MiSleep
 MiSleep is for EEG/EMG signal processing and visualization
 
 ![logo](resources/entire_logo.png)
 
 ## Get start
```

### Comparing `misleep-0.2.3b0/misleep.egg-info/SOURCES.txt` & `misleep-0.2.4b0/misleep.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 misleep/gui/resources/misleep.qrc
 misleep/gui/uis/__init__.py
 misleep/gui/uis/about_ui.py
 misleep/gui/uis/label_dialog_ui.py
 misleep/gui/uis/main_window_ui.py
 misleep/gui/uis/save_data_dialog_ui.py
 misleep/gui/uis/spec_window_ui.py
+misleep/gui/uis/state_spectral_dialog_ui.py
 misleep/gui/uis/transfer_result_dialog_ui.py
 misleep/io/__init__.py
 misleep/io/annotation_io.py
 misleep/io/base.py
 misleep/io/signal_io.py
 misleep/preprocessing/__init__.py
 misleep/preprocessing/channel.py
```

### Comparing `misleep-0.2.3b0/setup.py` & `misleep-0.2.4b0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,26 +7,27 @@
 
 DISTNAME = "misleep"
 MAINTAINER = "Xueqiang Wang"
 MAINTAINER_EMAIL = "swang@gmail.com"
 URL = "https://github.com/BryanWang0702/MiSleep/"
 LICENSE = "BSD (3-clause)"
 DOWNLOAD_URL = "https://github.com/BryanWang0702/MiSleep/"
-VERSION = "0.2.3b0"
+VERSION = "0.2.4b0"
 
 INSTALL_REQUIRES = [
     "numpy>=1.18.1",
     "matplotlib",
     "scipy",
     "pyedflib",
     "hdf5storage",
     "pyqt5",
     "mat73",
     "pandas",
-    "openpyxl"
+    "openpyxl",
+    "yasa"
 ]
 
 PACKAGES = [
     "misleep",
 ]
 
 CLASSIFIERS = [
```

### Comparing `misleep-0.2.3b0/test/test_midata.py` & `misleep-0.2.4b0/test/test_midata.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.3b0/test/test_signal_io.py` & `misleep-0.2.4b0/test/test_signal_io.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.3b0/test/test_signals_viz.py` & `misleep-0.2.4b0/test/test_signals_viz.py`

 * *Files identical despite different names*

### Comparing `misleep-0.2.3b0/test/test_spectral_viz.py` & `misleep-0.2.4b0/test/test_spectral_viz.py`

 * *Files identical despite different names*

