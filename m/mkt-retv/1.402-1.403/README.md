# Comparing `tmp/mkt-retv-1.402.tar.gz` & `tmp/mkt-retv-1.403.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkt-retv-1.402.tar", last modified: Tue Jan 30 11:26:24 2024, max compression
+gzip compressed data, was "mkt-retv-1.403.tar", last modified: Wed Apr 24 14:07:53 2024, max compression
```

## Comparing `mkt-retv-1.402.tar` & `mkt-retv-1.403.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-01-30 11:26:24.458390 mkt-retv-1.402/
--rw-rw-rw-   0        0        0      697 2024-01-30 11:26:24.458390 mkt-retv-1.402/PKG-INFO
--rw-rw-rw-   0        0        0     1637 2024-01-28 21:55:38.000000 mkt-retv-1.402/README.md
-drwxrwxrwx   0        0        0        0 2024-01-30 11:26:24.294386 mkt-retv-1.402/market_research/
--rw-rw-rw-   0        0        0        2 2023-11-21 12:45:19.000000 mkt-retv-1.402/market_research/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-30 11:26:24.332487 mkt-retv-1.402/market_research/analysis/
--rw-rw-rw-   0        0        0      167 2024-01-28 14:21:17.000000 mkt-retv-1.402/market_research/analysis/__init__.py
--rw-rw-rw-   0        0        0     1285 2023-11-23 12:49:10.000000 mkt-retv-1.402/market_research/analysis/_analysis_scheme.py
--rw-rw-rw-   0        0        0    10414 2024-01-30 11:22:46.000000 mkt-retv-1.402/market_research/analysis/imgemanger.py
--rw-rw-rw-   0        0        0    11047 2023-12-02 10:26:16.000000 mkt-retv-1.402/market_research/analysis/sentimentmanager.py
--rw-rw-rw-   0        0        0     4939 2024-01-28 14:17:23.000000 mkt-retv-1.402/market_research/analysis/textmanager.py
-drwxrwxrwx   0        0        0        0 2024-01-30 11:26:24.348139 mkt-retv-1.402/market_research/scraper/
--rw-rw-rw-   0        0        0      451 2024-01-24 12:15:44.000000 mkt-retv-1.402/market_research/scraper/__init__.py
--rw-rw-rw-   0        0        0     2145 2023-11-21 13:39:46.000000 mkt-retv-1.402/market_research/scraper/_scaper_scheme.py
--rw-rw-rw-   0        0        0      497 2023-11-21 16:22:41.000000 mkt-retv-1.402/market_research/scraper/_visualizer_scheme.py
-drwxrwxrwx   0        0        0        0 2024-01-30 11:26:24.348139 mkt-retv-1.402/market_research/scraper/models/
--rw-rw-rw-   0        0        0        0 2023-11-21 12:44:57.000000 mkt-retv-1.402/market_research/scraper/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-30 11:26:24.364078 mkt-retv-1.402/market_research/scraper/models/pana/
--rw-rw-rw-   0        0        0        0 2023-11-21 12:44:12.000000 mkt-retv-1.402/market_research/scraper/models/pana/__init__.py
--rw-rw-rw-   0        0        0     6484 2024-01-24 12:45:30.000000 mkt-retv-1.402/market_research/scraper/models/pana/spec_p.py
--rw-rw-rw-   0        0        0    12563 2024-01-24 13:16:23.000000 mkt-retv-1.402/market_research/scraper/models/pana/spec_pjp.py
-drwxrwxrwx   0        0        0        0 2024-01-30 11:26:24.382713 mkt-retv-1.402/market_research/scraper/models/sony/
--rw-rw-rw-   0        0        0        4 2023-11-21 12:44:57.000000 mkt-retv-1.402/market_research/scraper/models/sony/__init__.py
--rw-rw-rw-   0        0        0     5209 2023-11-29 13:09:13.000000 mkt-retv-1.402/market_research/scraper/models/sony/cleanup_s.py
--rw-rw-rw-   0        0        0    10226 2024-01-24 12:45:30.000000 mkt-retv-1.402/market_research/scraper/models/sony/sepc_sjp.py
--rw-rw-rw-   0        0        0    11976 2024-01-24 12:45:38.000000 mkt-retv-1.402/market_research/scraper/models/sony/spec_s.py
--rw-rw-rw-   0        0        0     3774 2023-11-29 13:22:50.000000 mkt-retv-1.402/market_research/scraper/models/sony/visualizer_s.py
-drwxrwxrwx   0        0        0        0 2024-01-30 11:26:24.398460 mkt-retv-1.402/market_research/scraper/rtings/
--rw-rw-rw-   0        0        0      106 2023-11-19 08:24:51.000000 mkt-retv-1.402/market_research/scraper/rtings/__init__.py
--rw-rw-rw-   0        0        0    10290 2023-11-23 09:57:43.000000 mkt-retv-1.402/market_research/scraper/rtings/rtings.py
--rw-rw-rw-   0        0        0     6309 2023-11-26 10:28:52.000000 mkt-retv-1.402/market_research/scraper/rtings/rurlsearcher.py
--rw-rw-rw-   0        0        0    13793 2023-11-23 12:05:59.000000 mkt-retv-1.402/market_research/scraper/rtings/rvisualizer.py
-drwxrwxrwx   0        0        0        0 2024-01-30 11:26:24.411504 mkt-retv-1.402/market_research/tools/
--rw-rw-rw-   0        0        0      206 2023-11-16 08:38:53.000000 mkt-retv-1.402/market_research/tools/__init__.py
--rw-rw-rw-   0        0        0     1003 2023-11-18 14:03:46.000000 mkt-retv-1.402/market_research/tools/aimanager.py
--rw-rw-rw-   0        0        0     3371 2023-11-19 12:13:44.000000 mkt-retv-1.402/market_research/tools/filemanager.py
--rw-rw-rw-   0        0        0     3818 2023-11-14 14:05:22.000000 mkt-retv-1.402/market_research/tools/installer.py
--rw-rw-rw-   0        0        0     5509 2023-11-15 11:16:47.000000 mkt-retv-1.402/market_research/tools/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-01-30 11:26:24.458390 mkt-retv-1.402/mkt_retv.egg-info/
--rw-rw-rw-   0        0        0      697 2024-01-30 11:26:24.000000 mkt-retv-1.402/mkt_retv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1351 2024-01-30 11:26:24.000000 mkt-retv-1.402/mkt_retv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-30 11:26:24.000000 mkt-retv-1.402/mkt_retv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-01-30 11:26:24.000000 mkt-retv-1.402/mkt_retv.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      129 2024-01-30 11:26:24.000000 mkt-retv-1.402/mkt_retv.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-01-30 11:26:24.000000 mkt-retv-1.402/mkt_retv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-30 11:26:24.458390 mkt-retv-1.402/setup.cfg
--rw-rw-rw-   0        0        0      959 2024-01-30 11:25:53.000000 mkt-retv-1.402/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:53.610451 mkt-retv-1.403/
+-rw-rw-rw-   0        0        0      697 2024-04-24 14:07:53.610451 mkt-retv-1.403/PKG-INFO
+-rw-rw-rw-   0        0        0     1637 2024-01-28 21:55:38.000000 mkt-retv-1.403/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:53.070608 mkt-retv-1.403/market_research/
+-rw-rw-rw-   0        0        0        2 2023-11-21 12:45:19.000000 mkt-retv-1.403/market_research/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:53.158369 mkt-retv-1.403/market_research/analysis/
+-rw-rw-rw-   0        0        0      167 2024-01-28 14:21:17.000000 mkt-retv-1.403/market_research/analysis/__init__.py
+-rw-rw-rw-   0        0        0     1285 2023-11-23 12:49:10.000000 mkt-retv-1.403/market_research/analysis/_analysis_scheme.py
+-rw-rw-rw-   0        0        0    10414 2024-01-30 11:22:46.000000 mkt-retv-1.403/market_research/analysis/imgemanger.py
+-rw-rw-rw-   0        0        0    11047 2023-12-02 10:26:16.000000 mkt-retv-1.403/market_research/analysis/sentimentmanager.py
+-rw-rw-rw-   0        0        0     4939 2024-01-28 14:17:23.000000 mkt-retv-1.403/market_research/analysis/textmanager.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:53.202025 mkt-retv-1.403/market_research/scraper/
+-rw-rw-rw-   0        0        0      451 2024-01-24 12:15:44.000000 mkt-retv-1.403/market_research/scraper/__init__.py
+-rw-rw-rw-   0        0        0     2145 2023-11-21 13:39:46.000000 mkt-retv-1.403/market_research/scraper/_scaper_scheme.py
+-rw-rw-rw-   0        0        0      497 2023-11-21 16:22:41.000000 mkt-retv-1.403/market_research/scraper/_visualizer_scheme.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:53.202025 mkt-retv-1.403/market_research/scraper/models/
+-rw-rw-rw-   0        0        0        0 2023-11-21 12:44:57.000000 mkt-retv-1.403/market_research/scraper/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:53.258423 mkt-retv-1.403/market_research/scraper/models/pana/
+-rw-rw-rw-   0        0        0        0 2023-11-21 12:44:12.000000 mkt-retv-1.403/market_research/scraper/models/pana/__init__.py
+-rw-rw-rw-   0        0        0     6484 2024-01-24 12:45:30.000000 mkt-retv-1.403/market_research/scraper/models/pana/spec_p.py
+-rw-rw-rw-   0        0        0    12563 2024-01-24 13:16:23.000000 mkt-retv-1.403/market_research/scraper/models/pana/spec_pjp.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:53.358827 mkt-retv-1.403/market_research/scraper/models/sony/
+-rw-rw-rw-   0        0        0        4 2023-11-21 12:44:57.000000 mkt-retv-1.403/market_research/scraper/models/sony/__init__.py
+-rw-rw-rw-   0        0        0     5203 2024-04-24 13:43:17.000000 mkt-retv-1.403/market_research/scraper/models/sony/cleanup_s.py
+-rw-rw-rw-   0        0        0    10226 2024-01-24 12:45:30.000000 mkt-retv-1.403/market_research/scraper/models/sony/sepc_sjp.py
+-rw-rw-rw-   0        0        0    11943 2024-04-24 13:28:28.000000 mkt-retv-1.403/market_research/scraper/models/sony/spec_s.py
+-rw-rw-rw-   0        0        0     4147 2024-04-24 14:06:33.000000 mkt-retv-1.403/market_research/scraper/models/sony/visualizer_s.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:53.436978 mkt-retv-1.403/market_research/scraper/rtings/
+-rw-rw-rw-   0        0        0      106 2023-11-19 08:24:51.000000 mkt-retv-1.403/market_research/scraper/rtings/__init__.py
+-rw-rw-rw-   0        0        0    10290 2023-11-23 09:57:43.000000 mkt-retv-1.403/market_research/scraper/rtings/rtings.py
+-rw-rw-rw-   0        0        0     6309 2023-11-26 10:28:52.000000 mkt-retv-1.403/market_research/scraper/rtings/rurlsearcher.py
+-rw-rw-rw-   0        0        0    13793 2023-11-23 12:05:59.000000 mkt-retv-1.403/market_research/scraper/rtings/rvisualizer.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:53.531289 mkt-retv-1.403/market_research/tools/
+-rw-rw-rw-   0        0        0      206 2023-11-16 08:38:53.000000 mkt-retv-1.403/market_research/tools/__init__.py
+-rw-rw-rw-   0        0        0     1003 2023-11-18 14:03:46.000000 mkt-retv-1.403/market_research/tools/aimanager.py
+-rw-rw-rw-   0        0        0     3371 2023-11-19 12:13:44.000000 mkt-retv-1.403/market_research/tools/filemanager.py
+-rw-rw-rw-   0        0        0     3818 2023-11-14 14:05:22.000000 mkt-retv-1.403/market_research/tools/installer.py
+-rw-rw-rw-   0        0        0     5509 2023-11-15 11:16:47.000000 mkt-retv-1.403/market_research/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:53.607149 mkt-retv-1.403/mkt_retv.egg-info/
+-rw-rw-rw-   0        0        0      697 2024-04-24 14:07:52.000000 mkt-retv-1.403/mkt_retv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1351 2024-04-24 14:07:52.000000 mkt-retv-1.403/mkt_retv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 14:07:52.000000 mkt-retv-1.403/mkt_retv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-04-24 14:07:52.000000 mkt-retv-1.403/mkt_retv.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      129 2024-04-24 14:07:52.000000 mkt-retv-1.403/mkt_retv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-24 14:07:52.000000 mkt-retv-1.403/mkt_retv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 14:07:53.614519 mkt-retv-1.403/setup.cfg
+-rw-rw-rw-   0        0        0      959 2024-04-24 14:07:47.000000 mkt-retv-1.403/setup.py
```

### Comparing `mkt-retv-1.402/PKG-INFO` & `mkt-retv-1.403/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkt-retv
-Version: 1.402
+Version: 1.403
 Summary: market research TV 
 Home-page: https://github.com/xikest/research_market_tv
 Author: xikest
 Project-URL: Source, https://github.com/xikest/research_market_tv
 Project-URL: Bug Tracker, https://github.com/xikest/research_market_tv/issues
 Requires-Python: >=3.7
 Requires-Dist: numpy
```

### Comparing `mkt-retv-1.402/README.md` & `mkt-retv-1.403/README.md`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.402/market_research/analysis/_analysis_scheme.py` & `mkt-retv-1.403/market_research/analysis/_analysis_scheme.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.402/market_research/analysis/imgemanger.py` & `mkt-retv-1.403/market_research/analysis/imgemanger.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.402/market_research/analysis/sentimentmanager.py` & `mkt-retv-1.403/market_research/analysis/sentimentmanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.402/market_research/analysis/textmanager.py` & `mkt-retv-1.403/market_research/analysis/textmanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.402/market_research/scraper/_scaper_scheme.py` & `mkt-retv-1.403/market_research/scraper/_scaper_scheme.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.402/market_research/scraper/models/pana/spec_p.py` & `mkt-retv-1.403/market_research/scraper/models/pana/spec_p.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.402/market_research/scraper/models/pana/spec_pjp.py` & `mkt-retv-1.403/market_research/scraper/models/pana/spec_pjp.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.402/market_research/scraper/models/sony/cleanup_s.py` & `mkt-retv-1.403/market_research/scraper/models/sony/cleanup_s.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,17 +30,19 @@
                            "wallmount", "mic", "network", "android", "ios", "miracast",
                            "operating", "store", "clock", "rs-232c", "menu", "mute", "4:3", "hdcp",
                            "built", "tuners", "demo", "presence", "switch", "reader", "face", "surround", "phase",
                            "batteries", "info", "Parental", "setup", "aspect", "dashboard", "formats", "accessibility",
                            "ci+",
                            "bass", "master", "shut", "sorplas", "volume", "wireless", "china",
                            "hole", "program", "manual", "latency",
-                           "inversion","twin","h x v","bravia","motion", "netflix","calman","rate"]
+                           "inversion","twin","h x v","bravia", "motion","calman","rate"]
         return stop_words_list
 
+
+
     def _preprocess_df(self):
         self.df = self.df.sort_values(["year", "series", "size", "grade"], axis=0, ascending=False)
         self.df = (self.df.map(lambda x: x.replace("  ", " ") if isinstance(x, str) else x)  # 공백 2개는 하나로 변경
                    .map(lambda x: x.replace("™", "") if isinstance(x, str) else x)  # ™ 제거
                    .map(lambda x: x.replace("®", "") if isinstance(x, str) else x)  # ® 제거
                    .map(lambda x: x.replace("\n\n", "\n ") if isinstance(x, str) else x)
                    .map(lambda x: x.replace(" \n", "\n ") if isinstance(x, str) else x)
```

### Comparing `mkt-retv-1.402/market_research/scraper/models/sony/sepc_sjp.py` & `mkt-retv-1.403/market_research/scraper/models/sony/sepc_sjp.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.402/market_research/scraper/models/sony/spec_s.py` & `mkt-retv-1.403/market_research/scraper/models/sony/spec_s.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,26 +227,24 @@
         dict_info = {}
         dict_info["year"] = model.split("-")[1][-1]
         dict_info["series"] = model.split("-")[1][2:-1]
         dict_info["size"] = model.split("-")[1][:2]
         dict_info["grade"] = model.split("-")[0]
 
         year_mapping = {
-            "N": 2025,
-            "M": 2024,
             'L': 2023,
             'K': 2022,
             'J': 2021,
             # Add additional mappings as needed
         }
 
         try:
             dict_info["year"] = year_mapping.get(dict_info.get("year"))
         except:
-            dict_info["year"] = ""
+            dict_info["year"] = "2024_" ## 임시
 
         return dict_info
 
     def _soup_to_dict(self, soup):
         """
         Convert BeautifulSoup soup to dictionary.
         """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mkt-retv-1.402/market_research/scraper/models/sony/visualizer_s.py` & `mkt-retv-1.403/market_research/scraper/models/sony/visualizer_s.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,29 +40,33 @@
         # cividis
         # inferno
         # magma
         # coolwarm
         # Blues
         """
         if col_selected is None:
-            col_selected = [
-                            'contrast enhancement', 'peak luminance', 'pixel contrast booster',
-                             'color enhancement', 'triluminos', 'smoothing', 'live colour technology',
-                             'clarity enhancement', 'dual database processing', 'video processing',
-                             'object-based super resolution',
+            col_selected = ['Display Type', 'Backlight type', 'Backlight dimming type'
+                            'High Peak Luminance','peak luminance',
+                            'contrast enhancement', 'pixel contrast booster', 'Dynamic Contrast Enhancer','XR Backlight Master Drive',
+                             'color enhancement', 'triluminos',
+                            # 'live colour technology',
+                             # 'clarity enhancement', 'dual database processing', 'video processing',
+                             # 'object-based super resolution',
                              'viewing angle (x-wide angle)', 'x-wide angle',
                              'anti reflection (x-anti reflection)', 'x-anti reflection',
                              'picture processor', '4k processor',
-                             'color space',
-                             'eco friendly',
+                             # 'color space',
+                             # 'eco friendly',
+                             'SONY PICTURES CORE Calibrated mode', 'NETFLIX CALIBRATED MODE','Prime Video Calibrated mode',
                              'auto genre picture mode',
                              'features for playstation5 auto genre picture mode',
                              'auto hdr tone mapping',
                              'features for playstation5 auto hdr tone mapping',
                              'multi-view',
+                             'Rated Power Consumption'
                              ]
 
 
         data_df = self.dc.get_df_cleaned()
         data_df = data_df[col_selected]
         if display_types is not None:
             condition = data_df.index.get_level_values('display type').str.contains('|'.join(display_types), case=False, na=False)
```

### Comparing `mkt-retv-1.402/market_research/scraper/rtings/rtings.py` & `mkt-retv-1.403/market_research/scraper/rtings/rtings.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.402/market_research/scraper/rtings/rurlsearcher.py` & `mkt-retv-1.403/market_research/scraper/rtings/rurlsearcher.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.402/market_research/scraper/rtings/rvisualizer.py` & `mkt-retv-1.403/market_research/scraper/rtings/rvisualizer.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.402/market_research/tools/aimanager.py` & `mkt-retv-1.403/market_research/tools/aimanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.402/market_research/tools/filemanager.py` & `mkt-retv-1.403/market_research/tools/filemanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.402/market_research/tools/installer.py` & `mkt-retv-1.403/market_research/tools/installer.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.402/market_research/tools/webdriver.py` & `mkt-retv-1.403/market_research/tools/webdriver.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.402/mkt_retv.egg-info/PKG-INFO` & `mkt-retv-1.403/mkt_retv.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkt-retv
-Version: 1.402
+Version: 1.403
 Summary: market research TV 
 Home-page: https://github.com/xikest/research_market_tv
 Author: xikest
 Project-URL: Source, https://github.com/xikest/research_market_tv
 Project-URL: Bug Tracker, https://github.com/xikest/research_market_tv/issues
 Requires-Python: >=3.7
 Requires-Dist: numpy
```

### Comparing `mkt-retv-1.402/mkt_retv.egg-info/SOURCES.txt` & `mkt-retv-1.403/mkt_retv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.402/setup.py` & `mkt-retv-1.403/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mkt-retv',
-    version='1.402',
+    version='1.403',
     author='xikest',
     description='market research TV ',
     packages=find_packages(),
     python_requires='>=3.7',
     install_requires=[
         'numpy', 'pandas',
         'selenium','beautifulsoup4','requests',
```

