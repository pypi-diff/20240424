# Comparing `tmp/smartboiler-0.0.3.0.0.7.2.tar.gz` & `tmp/smartboiler-0.0.3.0.0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartboiler-0.0.3.0.0.7.2.tar", last modified: Tue Apr 23 19:24:11 2024, max compression
+gzip compressed data, was "smartboiler-0.0.3.0.0.7.3.tar", last modified: Tue Apr 23 19:56:28 2024, max compression
```

## Comparing `smartboiler-0.0.3.0.0.7.2.tar` & `smartboiler-0.0.3.0.0.7.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:24:11.660982 smartboiler-0.0.3.0.0.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-23 19:24:11.660982 smartboiler-0.0.3.0.0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-23 19:24:08.000000 smartboiler-0.0.3.0.0.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:24:11.660982 smartboiler-0.0.3.0.0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-23 19:24:09.000000 smartboiler-0.0.3.0.0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:24:11.656982 smartboiler-0.0.3.0.0.7.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:24:11.660982 smartboiler-0.0.3.0.0.7.2/src/smartboiler/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-23 19:24:08.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-04-23 19:24:08.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler/boiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    13097 2024-04-23 19:24:08.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    22920 2024-04-23 19:24:08.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-23 19:24:08.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler/event_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    14704 2024-04-23 19:24:08.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-23 19:24:08.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler/fotovoltaics.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:24:08.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    17340 2024-04-23 19:24:08.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler/retrieve_hass.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-23 19:24:08.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-23 19:24:08.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler/time_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    14501 2024-04-23 19:24:08.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler/week_planner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:24:11.660982 smartboiler-0.0.3.0.0.7.2/src/smartboiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-23 19:24:11.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-23 19:24:11.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:24:11.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 19:24:11.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-23 19:24:11.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 19:24:11.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:56:28.492168 smartboiler-0.0.3.0.0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-23 19:56:28.492168 smartboiler-0.0.3.0.0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-23 19:56:07.000000 smartboiler-0.0.3.0.0.7.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:56:28.492168 smartboiler-0.0.3.0.0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-23 19:56:22.000000 smartboiler-0.0.3.0.0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:56:28.492168 smartboiler-0.0.3.0.0.7.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:56:28.492168 smartboiler-0.0.3.0.0.7.3/src/smartboiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-23 19:56:07.000000 smartboiler-0.0.3.0.0.7.3/src/smartboiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-04-23 19:56:07.000000 smartboiler-0.0.3.0.0.7.3/src/smartboiler/boiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13097 2024-04-23 19:56:07.000000 smartboiler-0.0.3.0.0.7.3/src/smartboiler/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22920 2024-04-23 19:56:07.000000 smartboiler-0.0.3.0.0.7.3/src/smartboiler/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-23 19:56:07.000000 smartboiler-0.0.3.0.0.7.3/src/smartboiler/event_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14668 2024-04-23 19:56:07.000000 smartboiler-0.0.3.0.0.7.3/src/smartboiler/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-23 19:56:07.000000 smartboiler-0.0.3.0.0.7.3/src/smartboiler/fotovoltaics.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:56:07.000000 smartboiler-0.0.3.0.0.7.3/src/smartboiler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17340 2024-04-23 19:56:07.000000 smartboiler-0.0.3.0.0.7.3/src/smartboiler/retrieve_hass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-23 19:56:07.000000 smartboiler-0.0.3.0.0.7.3/src/smartboiler/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-23 19:56:07.000000 smartboiler-0.0.3.0.0.7.3/src/smartboiler/time_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14501 2024-04-23 19:56:07.000000 smartboiler-0.0.3.0.0.7.3/src/smartboiler/week_planner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:56:28.492168 smartboiler-0.0.3.0.0.7.3/src/smartboiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-23 19:56:28.000000 smartboiler-0.0.3.0.0.7.3/src/smartboiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-23 19:56:28.000000 smartboiler-0.0.3.0.0.7.3/src/smartboiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:56:28.000000 smartboiler-0.0.3.0.0.7.3/src/smartboiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 19:56:28.000000 smartboiler-0.0.3.0.0.7.3/src/smartboiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-23 19:56:28.000000 smartboiler-0.0.3.0.0.7.3/src/smartboiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 19:56:28.000000 smartboiler-0.0.3.0.0.7.3/src/smartboiler.egg-info/top_level.txt
```

### Comparing `smartboiler-0.0.3.0.0.7.2/PKG-INFO` & `smartboiler-0.0.3.0.0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 0.0.3.0.0.7.2
+Version: 0.0.3.0.0.7.3
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-0.0.3.0.0.7.2/README.md` & `smartboiler-0.0.3.0.0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.7.2/setup.py` & `smartboiler-0.0.3.0.0.7.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name='smartboiler',  # Required
-    version='0.0.3.0.0.7.2',  # Required
+    version='0.0.3.0.0.7.3',  # Required
     description='Smart boiling of household',  # Optional
     long_description=long_description,  # Optional
     long_description_content_type='text/markdown',  # Optional (see note above)
     url='https://github.com/grinwi/smartboiler',  # Optional
     author='Adam GRUNWALD',  # Optional
     author_email='grunwald.adam24@gmail.com',  # Optional
     classifiers=[  # Optional
```

### Comparing `smartboiler-0.0.3.0.0.7.2/src/smartboiler/boiler.py` & `smartboiler-0.0.3.0.0.7.3/src/smartboiler/boiler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.7.2/src/smartboiler/controller.py` & `smartboiler-0.0.3.0.0.7.3/src/smartboiler/controller.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.7.2/src/smartboiler/data_handler.py` & `smartboiler-0.0.3.0.0.7.3/src/smartboiler/data_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.7.2/src/smartboiler/event_checker.py` & `smartboiler-0.0.3.0.0.7.3/src/smartboiler/event_checker.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.7.2/src/smartboiler/forecast.py` & `smartboiler-0.0.3.0.0.7.3/src/smartboiler/forecast.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from distutils.command import build
 from pathlib import Path
 
 print("Running" if __name__ == "__main__" else "Importing", Path(__file__).resolve())
 from datetime import timedelta, datetime
 from sklearn.preprocessing import MinMaxScaler, RobustScaler
 from tensorflow.keras.models import Sequential
 from tensorflow.keras.callbacks import ReduceLROnPlateau
```

### Comparing `smartboiler-0.0.3.0.0.7.2/src/smartboiler/fotovoltaics.py` & `smartboiler-0.0.3.0.0.7.3/src/smartboiler/fotovoltaics.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.7.2/src/smartboiler/retrieve_hass.py` & `smartboiler-0.0.3.0.0.7.3/src/smartboiler/retrieve_hass.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.7.2/src/smartboiler/switch.py` & `smartboiler-0.0.3.0.0.7.3/src/smartboiler/switch.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.7.2/src/smartboiler/time_handler.py` & `smartboiler-0.0.3.0.0.7.3/src/smartboiler/time_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.7.2/src/smartboiler/week_planner.py` & `smartboiler-0.0.3.0.0.7.3/src/smartboiler/week_planner.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.7.2/src/smartboiler.egg-info/PKG-INFO` & `smartboiler-0.0.3.0.0.7.3/src/smartboiler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 0.0.3.0.0.7.2
+Version: 0.0.3.0.0.7.3
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-0.0.3.0.0.7.2/src/smartboiler.egg-info/SOURCES.txt` & `smartboiler-0.0.3.0.0.7.3/src/smartboiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

