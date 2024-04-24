# Comparing `tmp/collider_dashboard-1.3.0.0.tar.gz` & `tmp/collider_dashboard-1.3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collider_dashboard-1.3.0.0.tar", max compression
+gzip compressed data, was "collider_dashboard-1.3.1.0.tar", max compression
```

## Comparing `collider_dashboard-1.3.0.0.tar` & `collider_dashboard-1.3.1.0.tar`

### file list

```diff
@@ -1,37 +1,36 @@
--rw-r--r--   0        0        0     1071 2023-10-24 11:48:04.875018 collider_dashboard-1.3.0.0/LICENSE
--rw-r--r--   0        0        0     3581 2024-04-23 15:22:44.060082 collider_dashboard-1.3.0.0/README.md
--rw-r--r--   0        0        0     1362 2023-11-15 08:57:20.035624 collider_dashboard-1.3.0.0/collider_dashboard/__init__.py
--rw-r--r--   0        0        0     4449 2024-04-23 15:21:15.025736 collider_dashboard-1.3.0.0/collider_dashboard/__main__.py
--rw-r--r--   0        0        0   263006 2023-07-12 14:17:34.166444 collider_dashboard-1.3.0.0/collider_dashboard/assets/favicon.ico
--rw-r--r--   0        0        0     3741 2023-07-12 14:17:34.166444 collider_dashboard-1.3.0.0/collider_dashboard/assets/style.css
--rw-r--r--   0        0        0        0 2023-10-31 10:48:04.031937 collider_dashboard-1.3.0.0/collider_dashboard/backend/__init__.py
--rw-r--r--   0        0        0    23874 2024-04-23 15:18:16.757038 collider_dashboard-1.3.0.0/collider_dashboard/backend/compute_globals.py
--rw-r--r--   0        0        0       71 2023-11-07 10:48:49.664970 collider_dashboard-1.3.0.0/collider_dashboard/backend/fillingpatterns/__init__.py
--rw-r--r--   0        0        0    24744 2023-11-07 10:48:49.680971 collider_dashboard-1.3.0.0/collider_dashboard/backend/fillingpatterns/bbFunctions.py
--rw-r--r--   0        0        0      214 2023-11-07 10:55:40.460126 collider_dashboard-1.3.0.0/collider_dashboard/backend/fillingpatterns/disclaimer.md
--rw-r--r--   0        0        0     1458 2023-11-07 10:48:49.680971 collider_dashboard-1.3.0.0/collider_dashboard/backend/fillingpatterns/dotdict.py
--rw-r--r--   0        0        0    11712 2023-11-07 10:48:49.680971 collider_dashboard-1.3.0.0/collider_dashboard/backend/fillingpatterns/filling_pattern.py
--rw-r--r--   0        0        0    14291 2023-11-07 10:48:49.680971 collider_dashboard-1.3.0.0/collider_dashboard/backend/fillingpatterns/mystyle.py
--rw-r--r--   0        0        0    58560 2023-11-20 13:42:41.003136 collider_dashboard-1.3.0.0/collider_dashboard/backend/plot.py
--rw-r--r--   0        0        0     6799 2023-10-30 15:41:06.612463 collider_dashboard-1.3.0.0/collider_dashboard/backend/resonance.py
--rw-r--r--   0        0        0    12620 2024-04-23 15:15:30.012642 collider_dashboard-1.3.0.0/collider_dashboard/callbacks.py
--rw-r--r--   0        0        0     1716 2024-04-23 15:18:45.249790 collider_dashboard-1.3.0.0/collider_dashboard/dashboard.py
--rw-r--r--   0        0        0    21406 2023-11-02 15:35:17.252062 collider_dashboard-1.3.0.0/collider_dashboard/data/25ns_2464b_2452_1842_1821_236bpi_12inj_hybrid_converted.json
--rw-r--r--   0        0        0    21406 2024-02-21 12:52:56.845294 collider_dashboard-1.3.0.0/collider_dashboard/data/8b4e_1972b_1960_1178_1886_224bpi_12inj_800ns_bs200ns.json
--rw-r--r--   0        0        0 31122700 2024-01-24 09:55:11.869415 collider_dashboard-1.3.0.0/collider_dashboard/data/collider.json
--rw-r--r--   0        0        0      764 2023-11-20 14:22:51.013393 collider_dashboard-1.3.0.0/collider_dashboard/layout/__init__.py
--rw-r--r--   0        0        0     1990 2023-11-20 14:12:59.127295 collider_dashboard-1.3.0.0/collider_dashboard/layout/configuration.py
--rw-r--r--   0        0        0     1822 2023-10-30 14:14:19.025522 collider_dashboard-1.3.0.0/collider_dashboard/layout/filling.py
--rw-r--r--   0        0        0     5185 2023-10-30 14:14:34.581925 collider_dashboard-1.3.0.0/collider_dashboard/layout/footprint.py
--rw-r--r--   0        0        0     3896 2023-11-20 14:38:34.671795 collider_dashboard-1.3.0.0/collider_dashboard/layout/header.py
--rw-r--r--   0        0        0     2220 2023-11-20 14:30:08.139717 collider_dashboard-1.3.0.0/collider_dashboard/layout/knob.py
--rw-r--r--   0        0        0     1546 2023-10-30 14:43:13.835252 collider_dashboard-1.3.0.0/collider_dashboard/layout/main.py
--rw-r--r--   0        0        0     2385 2023-10-30 14:49:30.513242 collider_dashboard-1.3.0.0/collider_dashboard/layout/optics.py
--rw-r--r--   0        0        0    11401 2024-04-23 15:13:00.436694 collider_dashboard-1.3.0.0/collider_dashboard/layout/sanity.py
--rw-r--r--   0        0        0     3931 2023-10-30 14:51:24.176257 collider_dashboard-1.3.0.0/collider_dashboard/layout/separation.py
--rw-r--r--   0        0        0     4588 2023-11-08 10:41:12.594720 collider_dashboard-1.3.0.0/collider_dashboard/layout/separation_3D.py
--rw-r--r--   0        0        0     5274 2023-10-30 14:51:51.948994 collider_dashboard-1.3.0.0/collider_dashboard/layout/survey.py
--rw-r--r--   0        0        0     1586 2023-10-30 15:05:24.770559 collider_dashboard-1.3.0.0/collider_dashboard/layout/tables.py
--rw-r--r--   0        0        0        0 2023-07-12 14:17:34.166444 collider_dashboard-1.3.0.0/collider_dashboard/temp/.gitkeep
--rw-r--r--   0        0        0     1111 2024-04-23 15:23:35.413434 collider_dashboard-1.3.0.0/pyproject.toml
--rw-r--r--   0        0        0     4686 1970-01-01 00:00:00.000000 collider_dashboard-1.3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-10-24 11:48:04.875018 collider_dashboard-1.3.1.0/LICENSE
+-rw-r--r--   0        0        0     3581 2024-04-23 15:22:44.060082 collider_dashboard-1.3.1.0/README.md
+-rw-r--r--   0        0        0     1362 2023-11-15 08:57:20.035624 collider_dashboard-1.3.1.0/collider_dashboard/__init__.py
+-rw-r--r--   0        0        0     4449 2024-04-24 12:21:44.886368 collider_dashboard-1.3.1.0/collider_dashboard/__main__.py
+-rw-r--r--   0        0        0   263006 2023-07-12 14:17:34.166444 collider_dashboard-1.3.1.0/collider_dashboard/assets/favicon.ico
+-rw-r--r--   0        0        0     3741 2023-07-12 14:17:34.166444 collider_dashboard-1.3.1.0/collider_dashboard/assets/style.css
+-rw-r--r--   0        0        0        0 2023-10-31 10:48:04.031937 collider_dashboard-1.3.1.0/collider_dashboard/backend/__init__.py
+-rw-r--r--   0        0        0    23873 2024-04-24 12:43:07.264226 collider_dashboard-1.3.1.0/collider_dashboard/backend/compute_globals.py
+-rw-r--r--   0        0        0       71 2023-11-07 10:48:49.664970 collider_dashboard-1.3.1.0/collider_dashboard/backend/fillingpatterns/__init__.py
+-rw-r--r--   0        0        0    24744 2023-11-07 10:48:49.680971 collider_dashboard-1.3.1.0/collider_dashboard/backend/fillingpatterns/bbFunctions.py
+-rw-r--r--   0        0        0      214 2023-11-07 10:55:40.460126 collider_dashboard-1.3.1.0/collider_dashboard/backend/fillingpatterns/disclaimer.md
+-rw-r--r--   0        0        0     1458 2023-11-07 10:48:49.680971 collider_dashboard-1.3.1.0/collider_dashboard/backend/fillingpatterns/dotdict.py
+-rw-r--r--   0        0        0    11712 2023-11-07 10:48:49.680971 collider_dashboard-1.3.1.0/collider_dashboard/backend/fillingpatterns/filling_pattern.py
+-rw-r--r--   0        0        0    14291 2023-11-07 10:48:49.680971 collider_dashboard-1.3.1.0/collider_dashboard/backend/fillingpatterns/mystyle.py
+-rw-r--r--   0        0        0    58560 2023-11-20 13:42:41.003136 collider_dashboard-1.3.1.0/collider_dashboard/backend/plot.py
+-rw-r--r--   0        0        0     6799 2023-10-30 15:41:06.612463 collider_dashboard-1.3.1.0/collider_dashboard/backend/resonance.py
+-rw-r--r--   0        0        0    12620 2024-04-23 15:15:30.012642 collider_dashboard-1.3.1.0/collider_dashboard/callbacks.py
+-rw-r--r--   0        0        0     1716 2024-04-23 15:18:45.249790 collider_dashboard-1.3.1.0/collider_dashboard/dashboard.py
+-rw-r--r--   0        0        0    14277 2024-04-24 12:17:34.807763 collider_dashboard-1.3.1.0/collider_dashboard/data/25ns_2556b_2544_2211_2327_3x48bpi_20inj.json
+-rw-r--r--   0        0        0 59716547 2024-04-24 12:15:38.644694 collider_dashboard-1.3.1.0/collider_dashboard/data/collider.json
+-rw-r--r--   0        0        0      764 2023-11-20 14:22:51.013393 collider_dashboard-1.3.1.0/collider_dashboard/layout/__init__.py
+-rw-r--r--   0        0        0     1990 2023-11-20 14:12:59.127295 collider_dashboard-1.3.1.0/collider_dashboard/layout/configuration.py
+-rw-r--r--   0        0        0     1822 2023-10-30 14:14:19.025522 collider_dashboard-1.3.1.0/collider_dashboard/layout/filling.py
+-rw-r--r--   0        0        0     5185 2023-10-30 14:14:34.581925 collider_dashboard-1.3.1.0/collider_dashboard/layout/footprint.py
+-rw-r--r--   0        0        0     3896 2023-11-20 14:38:34.671795 collider_dashboard-1.3.1.0/collider_dashboard/layout/header.py
+-rw-r--r--   0        0        0     2220 2023-11-20 14:30:08.139717 collider_dashboard-1.3.1.0/collider_dashboard/layout/knob.py
+-rw-r--r--   0        0        0     1546 2023-10-30 14:43:13.835252 collider_dashboard-1.3.1.0/collider_dashboard/layout/main.py
+-rw-r--r--   0        0        0     2385 2023-10-30 14:49:30.513242 collider_dashboard-1.3.1.0/collider_dashboard/layout/optics.py
+-rw-r--r--   0        0        0    11401 2024-04-23 15:13:00.436694 collider_dashboard-1.3.1.0/collider_dashboard/layout/sanity.py
+-rw-r--r--   0        0        0     3931 2023-10-30 14:51:24.176257 collider_dashboard-1.3.1.0/collider_dashboard/layout/separation.py
+-rw-r--r--   0        0        0     4588 2023-11-08 10:41:12.594720 collider_dashboard-1.3.1.0/collider_dashboard/layout/separation_3D.py
+-rw-r--r--   0        0        0     5274 2023-10-30 14:51:51.948994 collider_dashboard-1.3.1.0/collider_dashboard/layout/survey.py
+-rw-r--r--   0        0        0     1586 2023-10-30 15:05:24.770559 collider_dashboard-1.3.1.0/collider_dashboard/layout/tables.py
+-rw-r--r--   0        0        0        0 2023-07-12 14:17:34.166444 collider_dashboard-1.3.1.0/collider_dashboard/temp/.gitkeep
+-rw-r--r--   0        0        0     1111 2024-04-24 12:52:03.970029 collider_dashboard-1.3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4686 1970-01-01 00:00:00.000000 collider_dashboard-1.3.1.0/PKG-INFO
```

### Comparing `collider_dashboard-1.3.0.0/LICENSE` & `collider_dashboard-1.3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.3.0.0/README.md` & `collider_dashboard-1.3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.3.0.0/collider_dashboard/__init__.py` & `collider_dashboard-1.3.1.0/collider_dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.3.0.0/collider_dashboard/__main__.py` & `collider_dashboard-1.3.1.0/collider_dashboard/__main__.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.3.0.0/collider_dashboard/assets/favicon.ico` & `collider_dashboard-1.3.1.0/collider_dashboard/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.3.0.0/collider_dashboard/assets/style.css` & `collider_dashboard-1.3.1.0/collider_dashboard/assets/style.css`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.3.0.0/collider_dashboard/backend/compute_globals.py` & `collider_dashboard-1.3.1.0/collider_dashboard/backend/compute_globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -442,15 +442,15 @@
         df_elements_corrected.at[index, "knl"] = (
             df_elements_corrected.loc[index, "knl"] + np.array(df_elements.loc[i]["knl"])
             if not isinstance(df_elements.loc[i]["knl"], float)
             else df_elements.loc[i]["knl"]
         )
 
         # Replace order
-        df_elements_corrected.at[index, "_order"] = df_elements.loc[i]["_order"]
+        df_elements_corrected.at[index, "_order"] = df_elements.loc[i]["order"]
 
     # Drop all duplicate rows
     df_elements_corrected.drop(index=df_tw_duplicated_elements.index, inplace=True)
 
     return df_elements_corrected
```

### Comparing `collider_dashboard-1.3.0.0/collider_dashboard/backend/fillingpatterns/bbFunctions.py` & `collider_dashboard-1.3.1.0/collider_dashboard/backend/fillingpatterns/bbFunctions.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.3.0.0/collider_dashboard/backend/fillingpatterns/dotdict.py` & `collider_dashboard-1.3.1.0/collider_dashboard/backend/fillingpatterns/dotdict.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.3.0.0/collider_dashboard/backend/fillingpatterns/filling_pattern.py` & `collider_dashboard-1.3.1.0/collider_dashboard/backend/fillingpatterns/filling_pattern.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.3.0.0/collider_dashboard/backend/fillingpatterns/mystyle.py` & `collider_dashboard-1.3.1.0/collider_dashboard/backend/fillingpatterns/mystyle.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.3.0.0/collider_dashboard/backend/plot.py` & `collider_dashboard-1.3.1.0/collider_dashboard/backend/plot.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.3.0.0/collider_dashboard/backend/resonance.py` & `collider_dashboard-1.3.1.0/collider_dashboard/backend/resonance.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.3.0.0/collider_dashboard/callbacks.py` & `collider_dashboard-1.3.1.0/collider_dashboard/callbacks.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.3.0.0/collider_dashboard/dashboard.py` & `collider_dashboard-1.3.1.0/collider_dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.3.0.0/collider_dashboard/layout/__init__.py` & `collider_dashboard-1.3.1.0/collider_dashboard/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.3.0.0/collider_dashboard/layout/configuration.py` & `collider_dashboard-1.3.1.0/collider_dashboard/layout/configuration.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.3.0.0/collider_dashboard/layout/filling.py` & `collider_dashboard-1.3.1.0/collider_dashboard/layout/filling.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.3.0.0/collider_dashboard/layout/footprint.py` & `collider_dashboard-1.3.1.0/collider_dashboard/layout/footprint.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.3.0.0/collider_dashboard/layout/header.py` & `collider_dashboard-1.3.1.0/collider_dashboard/layout/header.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.3.0.0/collider_dashboard/layout/knob.py` & `collider_dashboard-1.3.1.0/collider_dashboard/layout/knob.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.3.0.0/collider_dashboard/layout/main.py` & `collider_dashboard-1.3.1.0/collider_dashboard/layout/main.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.3.0.0/collider_dashboard/layout/optics.py` & `collider_dashboard-1.3.1.0/collider_dashboard/layout/optics.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.3.0.0/collider_dashboard/layout/sanity.py` & `collider_dashboard-1.3.1.0/collider_dashboard/layout/sanity.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.3.0.0/collider_dashboard/layout/separation.py` & `collider_dashboard-1.3.1.0/collider_dashboard/layout/separation.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.3.0.0/collider_dashboard/layout/separation_3D.py` & `collider_dashboard-1.3.1.0/collider_dashboard/layout/separation_3D.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.3.0.0/collider_dashboard/layout/survey.py` & `collider_dashboard-1.3.1.0/collider_dashboard/layout/survey.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.3.0.0/collider_dashboard/layout/tables.py` & `collider_dashboard-1.3.1.0/collider_dashboard/layout/tables.py`

 * *Files identical despite different names*

### Comparing `collider_dashboard-1.3.0.0/pyproject.toml` & `collider_dashboard-1.3.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "collider-dashboard"
-version = "1.3.0.0"
+version = "1.3.1.0"
 description = "A Dash application to visualize the observables and parameters of a collider built and configured with Xsuite."
 authors = ["Colas Droin <colas.noe.droin@cern.ch>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ColasDroin/simulation-dashboard"
 packages = [
     { include = "collider_dashboard" },
@@ -16,15 +16,15 @@
 numpy = "^1.26.1"
 pandas = "^2.1.2"
 xsuite = "^0.6.0"
 dash-mantine-components = "^0.12.1"
 seaborn = "^0.13.0"
 dash-iconify = "^0.1.2"
 argparse = "^1.4.0"
-collider-check = "^0.1.7"
+collider-check = "^0.2.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
 black = "^23.10.1"
```

### Comparing `collider_dashboard-1.3.0.0/PKG-INFO` & `collider_dashboard-1.3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: collider-dashboard
-Version: 1.3.0.0
+Version: 1.3.1.0
 Summary: A Dash application to visualize the observables and parameters of a collider built and configured with Xsuite.
 Home-page: https://github.com/ColasDroin/simulation-dashboard
 License: MIT
 Author: Colas Droin
 Author-email: colas.noe.droin@cern.ch
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: argparse (>=1.4.0,<2.0.0)
-Requires-Dist: collider-check (>=0.1.7,<0.2.0)
+Requires-Dist: collider-check (>=0.2.0,<0.3.0)
 Requires-Dist: dash (>=2.14.1,<3.0.0)
 Requires-Dist: dash-iconify (>=0.1.2,<0.2.0)
 Requires-Dist: dash-mantine-components (>=0.12.1,<0.13.0)
 Requires-Dist: numpy (>=1.26.1,<2.0.0)
 Requires-Dist: pandas (>=2.1.2,<3.0.0)
 Requires-Dist: seaborn (>=0.13.0,<0.14.0)
 Requires-Dist: xsuite (>=0.6.0,<0.7.0)
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: collider-dashboard Version: 1.3.0.0 Summary: A Dash
+Metadata-Version: 2.1 Name: collider-dashboard Version: 1.3.1.0 Summary: A Dash
 application to visualize the observables and parameters of a collider built and
 configured with Xsuite. Home-page: https://github.com/ColasDroin/simulation-
 dashboard License: MIT Author: Colas Droin Author-email:
 colas.noe.droin@cern.ch Requires-Python: >=3.10,<3.13 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: argparse (>=1.4.0,<2.0.0) Requires-Dist: collider-check
-(>=0.1.7,<0.2.0) Requires-Dist: dash (>=2.14.1,<3.0.0) Requires-Dist: dash-
+(>=0.2.0,<0.3.0) Requires-Dist: dash (>=2.14.1,<3.0.0) Requires-Dist: dash-
 iconify (>=0.1.2,<0.2.0) Requires-Dist: dash-mantine-components
 (>=0.12.1,<0.13.0) Requires-Dist: numpy (>=1.26.1,<2.0.0) Requires-Dist: pandas
 (>=2.1.2,<3.0.0) Requires-Dist: seaborn (>=0.13.0,<0.14.0) Requires-Dist:
 xsuite (>=0.6.0,<0.7.0) Project-URL: Repository, https://github.com/ColasDroin/
 simulation-dashboard Description-Content-Type: text/markdown # Collider
 Dashboard
     _[_h_t_t_p_s_:_/_/_b_a_d_g_e_n_._n_e_t_/_s_t_a_t_i_c_/_l_i_c_e_n_s_e_/_M_I_T_/_b_l_u_e_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_n_._n_e_t_/_s_t_a_t_i_c_/
```

