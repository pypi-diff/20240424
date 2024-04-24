# Comparing `tmp/nwb4fp-0.6.0.3.tar.gz` & `tmp/nwb4fp-0.6.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwb4fp-0.6.0.3.tar", last modified: Tue Apr 23 18:25:01 2024, max compression
+gzip compressed data, was "nwb4fp-0.6.0.5.tar", last modified: Tue Apr 23 18:36:39 2024, max compression
```

## Comparing `nwb4fp-0.6.0.3.tar` & `nwb4fp-0.6.0.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 18:25:01.785047 nwb4fp-0.6.0.3/
--rw-rw-rw-   0        0        0     1089 2024-02-24 13:06:48.000000 nwb4fp-0.6.0.3/LICENSE
--rw-rw-rw-   0        0        0     5780 2024-04-23 18:25:01.762045 nwb4fp-0.6.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     6901 2024-03-27 14:22:15.000000 nwb4fp-0.6.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-23 18:25:01.786049 nwb4fp-0.6.0.3/setup.cfg
--rw-rw-rw-   0        0        0      877 2024-04-23 18:24:55.000000 nwb4fp-0.6.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:25:01.175045 nwb4fp-0.6.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-23 18:25:01.255051 nwb4fp-0.6.0.3/src/nwb4fp/
--rw-rw-rw-   0        0        0        0 2024-03-03 17:04:21.000000 nwb4fp-0.6.0.3/src/nwb4fp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:25:01.374053 nwb4fp-0.6.0.3/src/nwb4fp/main/
--rw-rw-rw-   0        0        0        0 2024-03-08 16:12:29.000000 nwb4fp-0.6.0.3/src/nwb4fp/main/__init__.py
--rw-rw-rw-   0        0        0     3593 2024-03-29 11:35:18.000000 nwb4fp-0.6.0.3/src/nwb4fp/main/main_create_nwb.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:25:01.513042 nwb4fp-0.6.0.3/src/nwb4fp/postprocess/
--rw-rw-rw-   0        0        0    15551 2024-03-27 11:37:25.000000 nwb4fp-0.6.0.3/src/nwb4fp/postprocess/Get_positions.py
--rw-rw-rw-   0        0        0        0 2024-02-15 18:06:22.000000 nwb4fp-0.6.0.3/src/nwb4fp/postprocess/__init__.py
--rw-rw-rw-   0        0        0     1639 2024-04-23 18:17:23.000000 nwb4fp-0.6.0.3/src/nwb4fp/postprocess/add_wfcor.py
--rw-rw-rw-   0        0        0      470 2024-03-24 12:00:57.000000 nwb4fp-0.6.0.3/src/nwb4fp/postprocess/dlc_kinematic.py
--rw-rw-rw-   0        0        0     2485 2024-03-29 14:47:19.000000 nwb4fp-0.6.0.3/src/nwb4fp/postprocess/extract_wf.py
--rw-rw-rw-   0        0        0     1343 2024-04-23 15:19:46.000000 nwb4fp-0.6.0.3/src/nwb4fp/postprocess/get_potential_merge.py
--rw-rw-rw-   0        0        0    17067 2024-04-04 14:46:56.000000 nwb4fp-0.6.0.3/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
--rw-rw-rw-   0        0        0    12880 2024-04-23 18:24:43.000000 nwb4fp-0.6.0.3/src/nwb4fp/postprocess/quality_metrix.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:25:01.667056 nwb4fp-0.6.0.3/src/nwb4fp/preprocess/
--rw-rw-rw-   0        0        0        0 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.3/src/nwb4fp/preprocess/__init__.py
--rw-rw-rw-   0        0        0      459 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.3/src/nwb4fp/preprocess/copy_file.py
--rw-rw-rw-   0        0        0      620 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.3/src/nwb4fp/preprocess/down_sample.py
--rw-rw-rw-   0        0        0     6762 2024-03-05 12:39:24.000000 nwb4fp-0.6.0.3/src/nwb4fp/preprocess/down_sample_lfp.py
--rw-rw-rw-   0        0        0     3712 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.3/src/nwb4fp/preprocess/extract_lfp.py
--rw-rw-rw-   0        0        0      148 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.3/src/nwb4fp/preprocess/get_path.py
--rw-rw-rw-   0        0        0     1203 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.3/src/nwb4fp/preprocess/load_data.py
--rw-rw-rw-   0        0        0      244 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.3/src/nwb4fp/preprocess/run_phy.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:25:01.198055 nwb4fp-0.6.0.3/src/nwb4fp/test/
-drwxrwxrwx   0        0        0        0 2024-04-23 18:25:01.734059 nwb4fp-0.6.0.3/src/nwb4fp/test/run_scripts/
--rw-rw-rw-   0        0        0     1552 2024-04-03 09:55:04.000000 nwb4fp-0.6.0.3/src/nwb4fp/test/run_scripts/readnwb.py
--rw-rw-rw-   0        0        0     1428 2024-04-23 16:33:31.000000 nwb4fp-0.6.0.3/src/nwb4fp/test/run_scripts/readnwb_09PC.py
--rw-rw-rw-   0        0        0        0 2024-03-13 14:23:55.000000 nwb4fp-0.6.0.3/src/nwb4fp/test/run_scripts/test.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:25:01.342048 nwb4fp-0.6.0.3/src/nwb4fp.egg-info/
--rw-rw-rw-   0        0        0     5780 2024-04-23 18:25:00.000000 nwb4fp-0.6.0.3/src/nwb4fp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1000 2024-04-23 18:25:01.000000 nwb4fp-0.6.0.3/src/nwb4fp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 18:25:00.000000 nwb4fp-0.6.0.3/src/nwb4fp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2910 2024-04-23 18:25:00.000000 nwb4fp-0.6.0.3/src/nwb4fp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-23 18:25:00.000000 nwb4fp-0.6.0.3/src/nwb4fp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 18:36:39.394041 nwb4fp-0.6.0.5/
+-rw-rw-rw-   0        0        0     1089 2024-02-24 13:06:48.000000 nwb4fp-0.6.0.5/LICENSE
+-rw-rw-rw-   0        0        0     5780 2024-04-23 18:36:39.385038 nwb4fp-0.6.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6901 2024-03-27 14:22:15.000000 nwb4fp-0.6.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-23 18:36:39.414995 nwb4fp-0.6.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      877 2024-04-23 18:36:36.000000 nwb4fp-0.6.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:36:39.005009 nwb4fp-0.6.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-23 18:36:39.024012 nwb4fp-0.6.0.5/src/nwb4fp/
+-rw-rw-rw-   0        0        0        0 2024-03-03 17:04:21.000000 nwb4fp-0.6.0.5/src/nwb4fp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:36:39.015007 nwb4fp-0.6.0.5/src/nwb4fp/main/
+-rw-rw-rw-   0        0        0        0 2024-03-08 16:12:29.000000 nwb4fp-0.6.0.5/src/nwb4fp/main/__init__.py
+-rw-rw-rw-   0        0        0     3593 2024-03-29 11:35:18.000000 nwb4fp-0.6.0.5/src/nwb4fp/main/main_create_nwb.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:36:39.019995 nwb4fp-0.6.0.5/src/nwb4fp/postprocess/
+-rw-rw-rw-   0        0        0    15551 2024-03-27 11:37:25.000000 nwb4fp-0.6.0.5/src/nwb4fp/postprocess/Get_positions.py
+-rw-rw-rw-   0        0        0        0 2024-02-15 18:06:22.000000 nwb4fp-0.6.0.5/src/nwb4fp/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     1639 2024-04-23 18:17:23.000000 nwb4fp-0.6.0.5/src/nwb4fp/postprocess/add_wfcor.py
+-rw-rw-rw-   0        0        0      470 2024-03-24 12:00:57.000000 nwb4fp-0.6.0.5/src/nwb4fp/postprocess/dlc_kinematic.py
+-rw-rw-rw-   0        0        0     2485 2024-03-29 14:47:19.000000 nwb4fp-0.6.0.5/src/nwb4fp/postprocess/extract_wf.py
+-rw-rw-rw-   0        0        0     1343 2024-04-23 15:19:46.000000 nwb4fp-0.6.0.5/src/nwb4fp/postprocess/get_potential_merge.py
+-rw-rw-rw-   0        0        0    17067 2024-04-04 14:46:56.000000 nwb4fp-0.6.0.5/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
+-rw-rw-rw-   0        0        0    12897 2024-04-23 18:36:02.000000 nwb4fp-0.6.0.5/src/nwb4fp/postprocess/quality_metrix.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:36:39.330001 nwb4fp-0.6.0.5/src/nwb4fp/preprocess/
+-rw-rw-rw-   0        0        0        0 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.5/src/nwb4fp/preprocess/__init__.py
+-rw-rw-rw-   0        0        0      459 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.5/src/nwb4fp/preprocess/copy_file.py
+-rw-rw-rw-   0        0        0      620 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.5/src/nwb4fp/preprocess/down_sample.py
+-rw-rw-rw-   0        0        0     6762 2024-03-05 12:39:24.000000 nwb4fp-0.6.0.5/src/nwb4fp/preprocess/down_sample_lfp.py
+-rw-rw-rw-   0        0        0     3712 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.5/src/nwb4fp/preprocess/extract_lfp.py
+-rw-rw-rw-   0        0        0      148 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.5/src/nwb4fp/preprocess/get_path.py
+-rw-rw-rw-   0        0        0     1203 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.5/src/nwb4fp/preprocess/load_data.py
+-rw-rw-rw-   0        0        0      244 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.5/src/nwb4fp/preprocess/run_phy.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:36:39.033010 nwb4fp-0.6.0.5/src/nwb4fp/test/
+drwxrwxrwx   0        0        0        0 2024-04-23 18:36:39.033010 nwb4fp-0.6.0.5/src/nwb4fp/test/run_scripts/
+-rw-rw-rw-   0        0        0     1552 2024-04-03 09:55:04.000000 nwb4fp-0.6.0.5/src/nwb4fp/test/run_scripts/readnwb.py
+-rw-rw-rw-   0        0        0     1428 2024-04-23 16:33:31.000000 nwb4fp-0.6.0.5/src/nwb4fp/test/run_scripts/readnwb_09PC.py
+-rw-rw-rw-   0        0        0        0 2024-03-13 14:23:55.000000 nwb4fp-0.6.0.5/src/nwb4fp/test/run_scripts/test.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:36:39.130005 nwb4fp-0.6.0.5/src/nwb4fp.egg-info/
+-rw-rw-rw-   0        0        0     5780 2024-04-23 18:36:38.000000 nwb4fp-0.6.0.5/src/nwb4fp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1000 2024-04-23 18:36:38.000000 nwb4fp-0.6.0.5/src/nwb4fp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 18:36:38.000000 nwb4fp-0.6.0.5/src/nwb4fp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2910 2024-04-23 18:36:38.000000 nwb4fp-0.6.0.5/src/nwb4fp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-23 18:36:38.000000 nwb4fp-0.6.0.5/src/nwb4fp.egg-info/top_level.txt
```

### Comparing `nwb4fp-0.6.0.3/LICENSE` & `nwb4fp-0.6.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.3/PKG-INFO` & `nwb4fp-0.6.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.6.0.3
+Version: 0.6.0.5
 Summary: Description of my package
 Home-page: https://github.com/sachuriga283/nwb4fp
 Author: sachuriga283
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.6.0.3/README.md` & `nwb4fp-0.6.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.3/setup.py` & `nwb4fp-0.6.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         with open('requirements.txt', encoding='utf-8-sig') as req:
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
     except UnicodeDecodeError:
         with open('requirements.txt', encoding='utf-16') as req:
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
 setup(
     name='nwb4fp',
-    version='0.6.0.3',
+    version='0.6.0.5',
     url='https://github.com/sachuriga283/nwb4fp',
     author='sachuriga283',
     author_email='sachuriga.sachuriga@ntnu.no',
     description='Description of my package',
     #packages=find_packages(./src/),    
     install_requires=read_requirements(),
 )
```

### Comparing `nwb4fp-0.6.0.3/src/nwb4fp/main/main_create_nwb.py` & `nwb4fp-0.6.0.5/src/nwb4fp/main/main_create_nwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.3/src/nwb4fp/postprocess/Get_positions.py` & `nwb4fp-0.6.0.5/src/nwb4fp/postprocess/Get_positions.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.3/src/nwb4fp/postprocess/add_wfcor.py` & `nwb4fp-0.6.0.5/src/nwb4fp/postprocess/add_wfcor.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.3/src/nwb4fp/postprocess/extract_wf.py` & `nwb4fp-0.6.0.5/src/nwb4fp/postprocess/extract_wf.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.3/src/nwb4fp/postprocess/get_potential_merge.py` & `nwb4fp-0.6.0.5/src/nwb4fp/postprocess/get_potential_merge.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.3/src/nwb4fp/postprocess/nwbPHYnOPHYS.py` & `nwb4fp-0.6.0.5/src/nwb4fp/postprocess/nwbPHYnOPHYS.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.3/src/nwb4fp/postprocess/quality_metrix.py` & `nwb4fp-0.6.0.5/src/nwb4fp/postprocess/quality_metrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,15 @@
     we = analyzer1.compute("quality_metrics")
     ccg = analyzer1.compute(input="correlograms",
                             window_ms=1000.0,
                             bin_ms=10.0,
                             method="auto")
     sim = analyzer1.compute("template_similarity", method="cosine_similarity")
     unit_locations = analyzer1.compute(input="unit_locations", method="monopolar_triangulation")
-    qm_ext = analyzer1.compute(input={"pca": dict(n_components=5, mode="by_channel_local"),
+    qm_ext = analyzer1.compute(input={"principal_components": dict(n_components=5, mode="by_channel_local"),
                                 "quality_metrics": dict(skip_pc_metrics=False)})
     # print(sort_merge.get_property_keys())
     # print(f"get times for merge sorts{sort_merge.get_times()}")
     # wfm = si.extract_waveforms(rec_save, sort_merge, folder=fr"{temp_folder}", overwrite=True, 
     #                           sparse=True, method="by_property",by_property="group",max_spikes_per_unit=None)
     # post.compute_unit_locations(waveform_extractor=wfm,
     #                             method= 'monopolar_triangulation',
```

### Comparing `nwb4fp-0.6.0.3/src/nwb4fp/preprocess/down_sample.py` & `nwb4fp-0.6.0.5/src/nwb4fp/preprocess/down_sample.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.3/src/nwb4fp/preprocess/down_sample_lfp.py` & `nwb4fp-0.6.0.5/src/nwb4fp/preprocess/down_sample_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.3/src/nwb4fp/preprocess/extract_lfp.py` & `nwb4fp-0.6.0.5/src/nwb4fp/preprocess/extract_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.3/src/nwb4fp/preprocess/load_data.py` & `nwb4fp-0.6.0.5/src/nwb4fp/preprocess/load_data.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.3/src/nwb4fp/test/run_scripts/readnwb.py` & `nwb4fp-0.6.0.5/src/nwb4fp/test/run_scripts/readnwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.3/src/nwb4fp/test/run_scripts/readnwb_09PC.py` & `nwb4fp-0.6.0.5/src/nwb4fp/test/run_scripts/readnwb_09PC.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.3/src/nwb4fp.egg-info/PKG-INFO` & `nwb4fp-0.6.0.5/src/nwb4fp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.6.0.3
+Version: 0.6.0.5
 Summary: Description of my package
 Home-page: https://github.com/sachuriga283/nwb4fp
 Author: sachuriga283
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.6.0.3/src/nwb4fp.egg-info/SOURCES.txt` & `nwb4fp-0.6.0.5/src/nwb4fp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.3/src/nwb4fp.egg-info/requires.txt` & `nwb4fp-0.6.0.5/src/nwb4fp.egg-info/requires.txt`

 * *Files identical despite different names*

