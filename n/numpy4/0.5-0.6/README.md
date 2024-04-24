# Comparing `tmp/numpy4-0.5.tar.gz` & `tmp/numpy4-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpy4-0.5.tar", last modified: Tue Apr 23 14:17:39 2024, max compression
+gzip compressed data, was "numpy4-0.6.tar", last modified: Wed Apr 24 16:26:11 2024, max compression
```

## Comparing `numpy4-0.5.tar` & `numpy4-0.6.tar`

### file list

```diff
@@ -1,31 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 14:17:39.979862 numpy4-0.5/
--rw-rw-rw-   0        0        0      213 2024-04-23 14:17:39.977862 numpy4-0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-23 14:17:39.950841 numpy4-0.5/numpy4/
--rw-rw-rw-   0        0        0     2549 2024-04-23 14:09:01.000000 numpy4-0.5/numpy4/ADS_DataCleaning.py
--rw-rw-rw-   0        0        0     2187 2024-04-22 09:37:22.000000 numpy4-0.5/numpy4/ADS_SMOTE.py
--rw-rw-rw-   0        0        0     3969 2024-04-22 09:42:33.000000 numpy4-0.5/numpy4/ADS_inferentialStats.py
--rw-rw-rw-   0        0        0     1286 2024-04-22 09:30:31.000000 numpy4-0.5/numpy4/ADS_outlierDetection.py
--rw-rw-rw-   0        0        0     1707 2024-04-23 14:08:35.000000 numpy4-0.5/numpy4/ADS_stats.py
--rw-rw-rw-   0        0        0     6252 2024-04-23 14:09:44.000000 numpy4-0.5/numpy4/ADS_superviseEval.py
--rw-rw-rw-   0        0        0     2235 2024-04-22 09:26:56.000000 numpy4-0.5/numpy4/ADS_timeSeries.py
--rw-rw-rw-   0        0        0      996 2024-04-22 09:22:47.000000 numpy4-0.5/numpy4/ADS_unsuperviseEval.py
--rw-rw-rw-   0        0        0     2456 2024-04-23 14:09:25.000000 numpy4-0.5/numpy4/ADS_visualization.py
--rw-rw-rw-   0        0        0     2082 2024-04-22 12:25:11.000000 numpy4-0.5/numpy4/DC_Bankers.py
--rw-rw-rw-   0        0        0     1260 2024-04-22 12:23:48.000000 numpy4-0.5/numpy4/DC_Berkley.py
--rw-rw-rw-   0        0        0     2479 2024-04-22 12:24:14.000000 numpy4-0.5/numpy4/DC_Bully.py
--rw-rw-rw-   0        0        0     1903 2024-04-22 12:24:33.000000 numpy4-0.5/numpy4/DC_RaymondTree.py
--rw-rw-rw-   0        0        0      985 2024-04-22 12:24:45.000000 numpy4-0.5/numpy4/DC_RicartAgrawala.py
--rw-rw-rw-   0        0        0     3564 2024-04-22 12:22:21.000000 numpy4-0.5/numpy4/DC_gc.py
--rw-rw-rw-   0        0        0     1383 2024-04-22 12:22:55.000000 numpy4-0.5/numpy4/DC_globalAvg.py
--rw-rw-rw-   0        0        0     1762 2024-04-22 12:19:22.000000 numpy4-0.5/numpy4/DC_ipc.py
--rw-rw-rw-   0        0        0     2541 2024-04-22 12:25:26.000000 numpy4-0.5/numpy4/DC_loadBalancing.py
--rw-rw-rw-   0        0        0       34 2024-04-22 12:25:53.000000 numpy4-0.5/numpy4/DC_multithreading.py
--rw-rw-rw-   0        0        0        0 2023-04-26 18:17:37.000000 numpy4-0.5/numpy4/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 14:17:39.976861 numpy4-0.5/numpy4.egg-info/
--rw-rw-rw-   0        0        0      213 2024-04-23 14:17:39.000000 numpy4-0.5/numpy4.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      641 2024-04-23 14:17:39.000000 numpy4-0.5/numpy4.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 14:17:39.000000 numpy4-0.5/numpy4.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-23 14:17:39.000000 numpy4-0.5/numpy4.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-23 14:17:39.000000 numpy4-0.5/numpy4.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 14:17:39.979862 numpy4-0.5/setup.cfg
--rw-rw-rw-   0        0        0      312 2024-04-23 14:16:51.000000 numpy4-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:26:11.124743 numpy4-0.6/
+-rw-rw-rw-   0        0        0      213 2024-04-24 16:26:11.118922 numpy4-0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-24 16:26:11.039765 numpy4-0.6/numpy4/
+-rw-rw-rw-   0        0        0     2549 2024-04-23 14:09:01.000000 numpy4-0.6/numpy4/ADS_DataCleaning.py
+-rw-rw-rw-   0        0        0     2187 2024-04-22 09:37:22.000000 numpy4-0.6/numpy4/ADS_SMOTE.py
+-rw-rw-rw-   0        0        0     3969 2024-04-22 09:42:33.000000 numpy4-0.6/numpy4/ADS_inferentialStats.py
+-rw-rw-rw-   0        0        0     1286 2024-04-22 09:30:31.000000 numpy4-0.6/numpy4/ADS_outlierDetection.py
+-rw-rw-rw-   0        0        0     1707 2024-04-23 14:08:35.000000 numpy4-0.6/numpy4/ADS_stats.py
+-rw-rw-rw-   0        0        0     6252 2024-04-23 14:09:44.000000 numpy4-0.6/numpy4/ADS_superviseEval.py
+-rw-rw-rw-   0        0        0     2235 2024-04-22 09:26:56.000000 numpy4-0.6/numpy4/ADS_timeSeries.py
+-rw-rw-rw-   0        0        0      996 2024-04-22 09:22:47.000000 numpy4-0.6/numpy4/ADS_unsuperviseEval.py
+-rw-rw-rw-   0        0        0     2456 2024-04-23 14:09:25.000000 numpy4-0.6/numpy4/ADS_visualization.py
+-rw-rw-rw-   0        0        0     2082 2024-04-22 12:25:11.000000 numpy4-0.6/numpy4/DC_Bankers.py
+-rw-rw-rw-   0        0        0     1260 2024-04-22 12:23:48.000000 numpy4-0.6/numpy4/DC_Berkley.py
+-rw-rw-rw-   0        0        0     2479 2024-04-22 12:24:14.000000 numpy4-0.6/numpy4/DC_Bully.py
+-rw-rw-rw-   0        0        0     1903 2024-04-22 12:24:33.000000 numpy4-0.6/numpy4/DC_RaymondTree.py
+-rw-rw-rw-   0        0        0      985 2024-04-22 12:24:45.000000 numpy4-0.6/numpy4/DC_RicartAgrawala.py
+-rw-rw-rw-   0        0        0     3564 2024-04-22 12:22:21.000000 numpy4-0.6/numpy4/DC_gc.py
+-rw-rw-rw-   0        0        0     1383 2024-04-22 12:22:55.000000 numpy4-0.6/numpy4/DC_globalAvg.py
+-rw-rw-rw-   0        0        0     1762 2024-04-22 12:19:22.000000 numpy4-0.6/numpy4/DC_ipc.py
+-rw-rw-rw-   0        0        0     2541 2024-04-22 12:25:26.000000 numpy4-0.6/numpy4/DC_loadBalancing.py
+-rw-rw-rw-   0        0        0       34 2024-04-22 12:25:53.000000 numpy4-0.6/numpy4/DC_multithreading.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 18:17:37.000000 numpy4-0.6/numpy4/__init__.py
+-rw-rw-rw-   0        0        0     1877 2024-04-24 16:24:55.000000 numpy4-0.6/numpy4/sma_10_community_prac_exam.py
+-rw-rw-rw-   0        0        0     8906 2024-04-24 16:22:12.000000 numpy4-0.6/numpy4/sma_1_topic_keyword_prac_exam.py
+-rw-rw-rw-   0        0        0     2207 2024-04-24 16:22:21.000000 numpy4-0.6/numpy4/sma_2_location_prac_exam.py
+-rw-rw-rw-   0        0        0     2052 2024-04-24 16:23:20.000000 numpy4-0.6/numpy4/sma_3_trends_prac_exam.py
+-rw-rw-rw-   0        0        0     3176 2024-04-24 16:23:25.000000 numpy4-0.6/numpy4/sma_4_hashtag_prac_exam.py
+-rw-rw-rw-   0        0        0     2195 2024-04-24 16:23:31.000000 numpy4-0.6/numpy4/sma_5_sentiment_prac_exam.py
+-rw-rw-rw-   0        0        0     2387 2024-04-24 16:23:37.000000 numpy4-0.6/numpy4/sma_6_user_engagement_prac_exam.py
+-rw-rw-rw-   0        0        0     1686 2024-04-24 16:24:38.000000 numpy4-0.6/numpy4/sma_7_eda_visualization_prac_exam (1).py
+-rw-rw-rw-   0        0        0     2199 2024-04-24 16:24:27.000000 numpy4-0.6/numpy4/sma_7_eda_visualization_prac_exam.py
+-rw-rw-rw-   0        0        0     1602 2024-04-24 16:24:42.000000 numpy4-0.6/numpy4/sma_8_brand_prac_exam.py
+-rw-rw-rw-   0        0        0     2322 2024-04-24 16:24:48.000000 numpy4-0.6/numpy4/sma_9_competitor_prac_exam.py
+drwxrwxrwx   0        0        0        0 2024-04-24 16:26:11.113272 numpy4-0.6/numpy4.egg-info/
+-rw-rw-rw-   0        0        0      213 2024-04-24 16:26:10.000000 numpy4-0.6/numpy4.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1059 2024-04-24 16:26:10.000000 numpy4-0.6/numpy4.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 16:26:10.000000 numpy4-0.6/numpy4.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-24 16:26:10.000000 numpy4-0.6/numpy4.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-24 16:26:10.000000 numpy4-0.6/numpy4.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 16:26:11.125738 numpy4-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      312 2024-04-24 16:26:07.000000 numpy4-0.6/setup.py
```

### Comparing `numpy4-0.5/numpy4/ADS_DataCleaning.py` & `numpy4-0.6/numpy4/ADS_DataCleaning.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.5/numpy4/ADS_SMOTE.py` & `numpy4-0.6/numpy4/ADS_SMOTE.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.5/numpy4/ADS_inferentialStats.py` & `numpy4-0.6/numpy4/ADS_inferentialStats.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.5/numpy4/ADS_outlierDetection.py` & `numpy4-0.6/numpy4/ADS_outlierDetection.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.5/numpy4/ADS_stats.py` & `numpy4-0.6/numpy4/ADS_stats.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.5/numpy4/ADS_superviseEval.py` & `numpy4-0.6/numpy4/ADS_superviseEval.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.5/numpy4/ADS_timeSeries.py` & `numpy4-0.6/numpy4/ADS_timeSeries.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.5/numpy4/ADS_unsuperviseEval.py` & `numpy4-0.6/numpy4/ADS_unsuperviseEval.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.5/numpy4/ADS_visualization.py` & `numpy4-0.6/numpy4/ADS_visualization.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.5/numpy4/DC_Bankers.py` & `numpy4-0.6/numpy4/DC_Bankers.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.5/numpy4/DC_Berkley.py` & `numpy4-0.6/numpy4/DC_Berkley.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.5/numpy4/DC_Bully.py` & `numpy4-0.6/numpy4/DC_Bully.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.5/numpy4/DC_RaymondTree.py` & `numpy4-0.6/numpy4/DC_RaymondTree.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.5/numpy4/DC_RicartAgrawala.py` & `numpy4-0.6/numpy4/DC_RicartAgrawala.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.5/numpy4/DC_gc.py` & `numpy4-0.6/numpy4/DC_gc.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.5/numpy4/DC_globalAvg.py` & `numpy4-0.6/numpy4/DC_globalAvg.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.5/numpy4/DC_ipc.py` & `numpy4-0.6/numpy4/DC_ipc.py`

 * *Files identical despite different names*

### Comparing `numpy4-0.5/numpy4/DC_loadBalancing.py` & `numpy4-0.6/numpy4/DC_loadBalancing.py`

 * *Files identical despite different names*

