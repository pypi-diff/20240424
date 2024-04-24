# Comparing `tmp/fluxlib-0.0.8.tar.gz` & `tmp/fluxlib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\fluxlib-0.0.8.tar", last modified: Fri Jul 17 08:08:17 2020, max compression
+gzip compressed data, was "dist\fluxlib-0.0.9.tar", last modified: Thu Aug 20 08:31:18 2020, max compression
```

## Comparing `fluxlib-0.0.8.tar` & `fluxlib-0.0.9.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxrwx   0        0        0        0 2020-07-17 08:08:17.000000 fluxlib-0.0.8/
--rw-rw-rw-   0        0        0      317 2020-07-17 08:08:17.000000 fluxlib-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      191 2020-07-14 08:38:11.000000 fluxlib-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2020-07-17 08:08:17.000000 fluxlib-0.0.8/fluxlib/
--rw-rw-rw-   0        0        0      322 2020-07-15 08:35:02.000000 fluxlib-0.0.8/fluxlib/__init__.py
--rw-rw-rw-   0        0        0     6979 2020-07-04 21:44:37.000000 fluxlib-0.0.8/fluxlib/fluxnet.py
-drwxrwxrwx   0        0        0        0 2020-07-17 08:08:17.000000 fluxlib-0.0.8/fluxlib/funcs/
--rw-rw-rw-   0        0        0       53 2020-07-14 11:06:53.000000 fluxlib-0.0.8/fluxlib/funcs/__init__.py
--rw-rw-rw-   0        0        0      518 2020-07-15 10:19:21.000000 fluxlib-0.0.8/fluxlib/funcs/cal_vpd.py
-drwxrwxrwx   0        0        0        0 2020-07-17 08:08:17.000000 fluxlib-0.0.8/fluxlib/gapfill/
--rw-rw-rw-   0        0        0      223 2020-07-10 07:17:55.000000 fluxlib-0.0.8/fluxlib/gapfill/__init__.py
--rw-rw-rw-   0        0        0     4144 2020-07-09 21:01:46.000000 fluxlib-0.0.8/fluxlib/gapfill/auxfill_xgb.py
--rw-rw-rw-   0        0        0     2944 2020-07-17 08:06:30.000000 fluxlib-0.0.8/fluxlib/gapfill/dataloader.py
--rw-rw-rw-   0        0        0    21346 2020-05-19 11:43:14.000000 fluxlib-0.0.8/fluxlib/gapfill/gapfill_candi.py
--rw-rw-rw-   0        0        0     8494 2020-07-10 09:35:58.000000 fluxlib-0.0.8/fluxlib/gapfill/gapfill_rfr.py
--rw-rw-rw-   0        0        0    11863 2020-07-10 12:55:31.000000 fluxlib-0.0.8/fluxlib/gapfill/ggapfill.py
--rw-rw-rw-   0        0        0     1861 2020-07-10 11:03:38.000000 fluxlib-0.0.8/fluxlib/gapfill/utils.py
-drwxrwxrwx   0        0        0        0 2020-07-17 08:08:17.000000 fluxlib-0.0.8/fluxlib/partitioning/
--rw-rw-rw-   0        0        0      117 2020-07-13 10:21:42.000000 fluxlib-0.0.8/fluxlib/partitioning/__init__.py
-drwxrwxrwx   0        0        0        0 2020-07-17 08:08:17.000000 fluxlib-0.0.8/fluxlib/partitioning/const/
--rw-rw-rw-   0        0        0      542 2020-07-10 13:42:55.000000 fluxlib-0.0.8/fluxlib/partitioning/const/__init__.py
--rw-rw-rw-   0        0        0     5391 2020-07-10 13:42:55.000000 fluxlib-0.0.8/fluxlib/partitioning/const/const.py
-drwxrwxrwx   0        0        0        0 2020-07-17 08:08:17.000000 fluxlib-0.0.8/fluxlib/partitioning/functions/
--rw-rw-rw-   0        0        0     1062 2020-07-10 13:42:56.000000 fluxlib-0.0.8/fluxlib/partitioning/functions/__init__.py
--rw-rw-rw-   0        0        0    39341 2020-07-10 13:42:56.000000 fluxlib-0.0.8/fluxlib/partitioning/functions/fit_functions.py
--rw-rw-rw-   0        0        0     2493 2020-07-10 13:42:56.000000 fluxlib-0.0.8/fluxlib/partitioning/functions/general_functions.py
--rw-rw-rw-   0        0        0    14277 2020-07-10 13:42:56.000000 fluxlib-0.0.8/fluxlib/partitioning/functions/logistic_function.py
--rw-rw-rw-   0        0        0     5458 2020-07-10 13:42:56.000000 fluxlib-0.0.8/fluxlib/partitioning/functions/opti_test_functions.py
--rw-rw-rw-   0        0        0    20563 2020-07-10 13:42:56.000000 fluxlib-0.0.8/fluxlib/partitioning/functions/sa_test_functions.py
--rw-rw-rw-   0        0        0    13671 2020-07-07 20:35:04.000000 fluxlib-0.0.8/fluxlib/partitioning/mad.py
--rw-rw-rw-   0        0        0    42886 2020-07-07 20:35:04.000000 fluxlib-0.0.8/fluxlib/partitioning/nee2gpp.py
--rw-rw-rw-   0        0        0      612 2020-07-13 10:19:54.000000 fluxlib-0.0.8/fluxlib/partitioning/partitioning.py
-drwxrwxrwx   0        0        0        0 2020-07-17 08:08:17.000000 fluxlib-0.0.8/fluxlib/preprocessing/
--rw-rw-rw-   0        0        0      104 2020-07-09 15:16:54.000000 fluxlib-0.0.8/fluxlib/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     5358 2020-07-09 16:11:05.000000 fluxlib-0.0.8/fluxlib/preprocessing/formatize.py
--rw-rw-rw-   0        0        0      682 2020-07-09 15:30:58.000000 fluxlib-0.0.8/fluxlib/preprocessing/share_drivers.py
--rw-rw-rw-   0        0        0      713 2020-07-01 17:39:58.000000 fluxlib-0.0.8/fluxlib/run_fluxnet.py
-drwxrwxrwx   0        0        0        0 2020-07-17 08:08:17.000000 fluxlib-0.0.8/fluxlib.egg-info/
--rw-rw-rw-   0        0        0      317 2020-07-17 08:08:17.000000 fluxlib-0.0.8/fluxlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1075 2020-07-17 08:08:17.000000 fluxlib-0.0.8/fluxlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-07-17 08:08:17.000000 fluxlib-0.0.8/fluxlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2020-07-17 08:08:17.000000 fluxlib-0.0.8/fluxlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-07-17 08:08:17.000000 fluxlib-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      750 2020-07-17 08:07:46.000000 fluxlib-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2020-08-20 08:31:18.000000 fluxlib-0.0.9/
+-rw-rw-rw-   0        0        0      317 2020-08-20 08:31:18.000000 fluxlib-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2020-07-14 08:38:11.000000 fluxlib-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2020-08-20 08:31:18.000000 fluxlib-0.0.9/fluxlib/
+-rw-rw-rw-   0        0        0      322 2020-07-15 08:35:02.000000 fluxlib-0.0.9/fluxlib/__init__.py
+-rw-rw-rw-   0        0        0     6979 2020-07-04 21:44:37.000000 fluxlib-0.0.9/fluxlib/fluxnet.py
+drwxrwxrwx   0        0        0        0 2020-08-20 08:31:18.000000 fluxlib-0.0.9/fluxlib/funcs/
+-rw-rw-rw-   0        0        0       53 2020-07-14 11:06:53.000000 fluxlib-0.0.9/fluxlib/funcs/__init__.py
+-rw-rw-rw-   0        0        0      518 2020-07-15 10:19:21.000000 fluxlib-0.0.9/fluxlib/funcs/cal_vpd.py
+drwxrwxrwx   0        0        0        0 2020-08-20 08:31:18.000000 fluxlib-0.0.9/fluxlib/gapfill/
+-rw-rw-rw-   0        0        0      223 2020-07-10 07:17:55.000000 fluxlib-0.0.9/fluxlib/gapfill/__init__.py
+-rw-rw-rw-   0        0        0     4144 2020-07-09 21:01:46.000000 fluxlib-0.0.9/fluxlib/gapfill/auxfill_xgb.py
+-rw-rw-rw-   0        0        0     2944 2020-07-17 08:06:30.000000 fluxlib-0.0.9/fluxlib/gapfill/dataloader.py
+-rw-rw-rw-   0        0        0    21346 2020-05-19 11:43:14.000000 fluxlib-0.0.9/fluxlib/gapfill/gapfill_candi.py
+-rw-rw-rw-   0        0        0     8494 2020-07-10 09:35:58.000000 fluxlib-0.0.9/fluxlib/gapfill/gapfill_rfr.py
+-rw-rw-rw-   0        0        0    11863 2020-07-10 12:55:31.000000 fluxlib-0.0.9/fluxlib/gapfill/ggapfill.py
+-rw-rw-rw-   0        0        0     1861 2020-07-10 11:03:38.000000 fluxlib-0.0.9/fluxlib/gapfill/utils.py
+drwxrwxrwx   0        0        0        0 2020-08-20 08:31:18.000000 fluxlib-0.0.9/fluxlib/partitioning/
+-rw-rw-rw-   0        0        0      117 2020-07-13 10:21:42.000000 fluxlib-0.0.9/fluxlib/partitioning/__init__.py
+drwxrwxrwx   0        0        0        0 2020-08-20 08:31:18.000000 fluxlib-0.0.9/fluxlib/partitioning/const/
+-rw-rw-rw-   0        0        0      542 2020-07-10 13:42:55.000000 fluxlib-0.0.9/fluxlib/partitioning/const/__init__.py
+-rw-rw-rw-   0        0        0     5391 2020-07-10 13:42:55.000000 fluxlib-0.0.9/fluxlib/partitioning/const/const.py
+drwxrwxrwx   0        0        0        0 2020-08-20 08:31:18.000000 fluxlib-0.0.9/fluxlib/partitioning/functions/
+-rw-rw-rw-   0        0        0     1062 2020-07-10 13:42:56.000000 fluxlib-0.0.9/fluxlib/partitioning/functions/__init__.py
+-rw-rw-rw-   0        0        0    39341 2020-07-10 13:42:56.000000 fluxlib-0.0.9/fluxlib/partitioning/functions/fit_functions.py
+-rw-rw-rw-   0        0        0     2493 2020-07-10 13:42:56.000000 fluxlib-0.0.9/fluxlib/partitioning/functions/general_functions.py
+-rw-rw-rw-   0        0        0    14277 2020-07-10 13:42:56.000000 fluxlib-0.0.9/fluxlib/partitioning/functions/logistic_function.py
+-rw-rw-rw-   0        0        0     5458 2020-07-10 13:42:56.000000 fluxlib-0.0.9/fluxlib/partitioning/functions/opti_test_functions.py
+-rw-rw-rw-   0        0        0    20563 2020-07-10 13:42:56.000000 fluxlib-0.0.9/fluxlib/partitioning/functions/sa_test_functions.py
+-rw-rw-rw-   0        0        0    13671 2020-07-07 20:35:04.000000 fluxlib-0.0.9/fluxlib/partitioning/mad.py
+-rw-rw-rw-   0        0        0    42886 2020-07-07 20:35:04.000000 fluxlib-0.0.9/fluxlib/partitioning/nee2gpp.py
+-rw-rw-rw-   0        0        0      612 2020-07-13 10:19:54.000000 fluxlib-0.0.9/fluxlib/partitioning/partitioning.py
+drwxrwxrwx   0        0        0        0 2020-08-20 08:31:18.000000 fluxlib-0.0.9/fluxlib/preprocessing/
+-rw-rw-rw-   0        0        0      143 2020-08-20 08:30:12.000000 fluxlib-0.0.9/fluxlib/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     4015 2020-08-20 08:29:36.000000 fluxlib-0.0.9/fluxlib/preprocessing/ec_raw_reader.py
+-rw-rw-rw-   0        0        0     5358 2020-07-09 16:11:05.000000 fluxlib-0.0.9/fluxlib/preprocessing/formatize.py
+-rw-rw-rw-   0        0        0      682 2020-07-09 15:30:58.000000 fluxlib-0.0.9/fluxlib/preprocessing/share_drivers.py
+-rw-rw-rw-   0        0        0      713 2020-07-01 17:39:58.000000 fluxlib-0.0.9/fluxlib/run_fluxnet.py
+drwxrwxrwx   0        0        0        0 2020-08-20 08:31:18.000000 fluxlib-0.0.9/fluxlib.egg-info/
+-rw-rw-rw-   0        0        0      317 2020-08-20 08:31:18.000000 fluxlib-0.0.9/fluxlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1114 2020-08-20 08:31:18.000000 fluxlib-0.0.9/fluxlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-08-20 08:31:18.000000 fluxlib-0.0.9/fluxlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2020-08-20 08:31:18.000000 fluxlib-0.0.9/fluxlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2020-08-20 08:31:18.000000 fluxlib-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      750 2020-08-20 08:30:48.000000 fluxlib-0.0.9/setup.py
```

### Comparing `fluxlib-0.0.8/fluxlib/fluxnet.py` & `fluxlib-0.0.9/fluxlib/fluxnet.py`

 * *Files identical despite different names*

### Comparing `fluxlib-0.0.8/fluxlib/funcs/cal_vpd.py` & `fluxlib-0.0.9/fluxlib/funcs/cal_vpd.py`

 * *Files identical despite different names*

### Comparing `fluxlib-0.0.8/fluxlib/gapfill/auxfill_xgb.py` & `fluxlib-0.0.9/fluxlib/gapfill/auxfill_xgb.py`

 * *Files identical despite different names*

### Comparing `fluxlib-0.0.8/fluxlib/gapfill/dataloader.py` & `fluxlib-0.0.9/fluxlib/gapfill/dataloader.py`

 * *Files identical despite different names*

### Comparing `fluxlib-0.0.8/fluxlib/gapfill/gapfill_candi.py` & `fluxlib-0.0.9/fluxlib/gapfill/gapfill_candi.py`

 * *Files identical despite different names*

### Comparing `fluxlib-0.0.8/fluxlib/gapfill/gapfill_rfr.py` & `fluxlib-0.0.9/fluxlib/gapfill/gapfill_rfr.py`

 * *Files identical despite different names*

### Comparing `fluxlib-0.0.8/fluxlib/gapfill/ggapfill.py` & `fluxlib-0.0.9/fluxlib/gapfill/ggapfill.py`

 * *Files identical despite different names*

### Comparing `fluxlib-0.0.8/fluxlib/gapfill/utils.py` & `fluxlib-0.0.9/fluxlib/gapfill/utils.py`

 * *Files identical despite different names*

### Comparing `fluxlib-0.0.8/fluxlib/partitioning/const/__init__.py` & `fluxlib-0.0.9/fluxlib/partitioning/const/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxlib-0.0.8/fluxlib/partitioning/const/const.py` & `fluxlib-0.0.9/fluxlib/partitioning/const/const.py`

 * *Files identical despite different names*

### Comparing `fluxlib-0.0.8/fluxlib/partitioning/functions/__init__.py` & `fluxlib-0.0.9/fluxlib/partitioning/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxlib-0.0.8/fluxlib/partitioning/functions/fit_functions.py` & `fluxlib-0.0.9/fluxlib/partitioning/functions/fit_functions.py`

 * *Files identical despite different names*

### Comparing `fluxlib-0.0.8/fluxlib/partitioning/functions/general_functions.py` & `fluxlib-0.0.9/fluxlib/partitioning/functions/general_functions.py`

 * *Files identical despite different names*

### Comparing `fluxlib-0.0.8/fluxlib/partitioning/functions/logistic_function.py` & `fluxlib-0.0.9/fluxlib/partitioning/functions/logistic_function.py`

 * *Files identical despite different names*

### Comparing `fluxlib-0.0.8/fluxlib/partitioning/functions/opti_test_functions.py` & `fluxlib-0.0.9/fluxlib/partitioning/functions/opti_test_functions.py`

 * *Files identical despite different names*

### Comparing `fluxlib-0.0.8/fluxlib/partitioning/functions/sa_test_functions.py` & `fluxlib-0.0.9/fluxlib/partitioning/functions/sa_test_functions.py`

 * *Files identical despite different names*

### Comparing `fluxlib-0.0.8/fluxlib/partitioning/mad.py` & `fluxlib-0.0.9/fluxlib/partitioning/mad.py`

 * *Files identical despite different names*

### Comparing `fluxlib-0.0.8/fluxlib/partitioning/nee2gpp.py` & `fluxlib-0.0.9/fluxlib/partitioning/nee2gpp.py`

 * *Files identical despite different names*

### Comparing `fluxlib-0.0.8/fluxlib/partitioning/partitioning.py` & `fluxlib-0.0.9/fluxlib/partitioning/partitioning.py`

 * *Files identical despite different names*

### Comparing `fluxlib-0.0.8/fluxlib/preprocessing/formatize.py` & `fluxlib-0.0.9/fluxlib/preprocessing/formatize.py`

 * *Files identical despite different names*

### Comparing `fluxlib-0.0.8/fluxlib/preprocessing/share_drivers.py` & `fluxlib-0.0.9/fluxlib/preprocessing/share_drivers.py`

 * *Files identical despite different names*

### Comparing `fluxlib-0.0.8/fluxlib/run_fluxnet.py` & `fluxlib-0.0.9/fluxlib/run_fluxnet.py`

 * *Files identical despite different names*

### Comparing `fluxlib-0.0.8/fluxlib.egg-info/SOURCES.txt` & `fluxlib-0.0.9/fluxlib.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -25,9 +25,10 @@
 fluxlib/partitioning/functions/__init__.py
 fluxlib/partitioning/functions/fit_functions.py
 fluxlib/partitioning/functions/general_functions.py
 fluxlib/partitioning/functions/logistic_function.py
 fluxlib/partitioning/functions/opti_test_functions.py
 fluxlib/partitioning/functions/sa_test_functions.py
 fluxlib/preprocessing/__init__.py
+fluxlib/preprocessing/ec_raw_reader.py
 fluxlib/preprocessing/formatize.py
 fluxlib/preprocessing/share_drivers.py
```

### Comparing `fluxlib-0.0.8/setup.py` & `fluxlib-0.0.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #############################################
 
 
 from setuptools import setup, find_packages
 
 setup(
 	name = "fluxlib",
-	version = "0.0.8",
+	version = "0.0.9",
 	keywords = ("eddy covariance postprocessing, gapfilling and partitioning", "flux"),
 	description = "left blank",
 	long_description = "left blank",
 	license = "MIT Licence",
 
 	url = "https://github.com/soonyenju/fluxlib",
 	author = "Songyan Zhu",
```

