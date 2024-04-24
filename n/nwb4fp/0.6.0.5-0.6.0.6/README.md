# Comparing `tmp/nwb4fp-0.6.0.5.tar.gz` & `tmp/nwb4fp-0.6.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwb4fp-0.6.0.5.tar", last modified: Tue Apr 23 18:36:39 2024, max compression
+gzip compressed data, was "nwb4fp-0.6.0.6.tar", last modified: Wed Apr 24 08:35:10 2024, max compression
```

## Comparing `nwb4fp-0.6.0.5.tar` & `nwb4fp-0.6.0.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 18:36:39.394041 nwb4fp-0.6.0.5/
--rw-rw-rw-   0        0        0     1089 2024-02-24 13:06:48.000000 nwb4fp-0.6.0.5/LICENSE
--rw-rw-rw-   0        0        0     5780 2024-04-23 18:36:39.385038 nwb4fp-0.6.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     6901 2024-03-27 14:22:15.000000 nwb4fp-0.6.0.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-23 18:36:39.414995 nwb4fp-0.6.0.5/setup.cfg
--rw-rw-rw-   0        0        0      877 2024-04-23 18:36:36.000000 nwb4fp-0.6.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:36:39.005009 nwb4fp-0.6.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-23 18:36:39.024012 nwb4fp-0.6.0.5/src/nwb4fp/
--rw-rw-rw-   0        0        0        0 2024-03-03 17:04:21.000000 nwb4fp-0.6.0.5/src/nwb4fp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:36:39.015007 nwb4fp-0.6.0.5/src/nwb4fp/main/
--rw-rw-rw-   0        0        0        0 2024-03-08 16:12:29.000000 nwb4fp-0.6.0.5/src/nwb4fp/main/__init__.py
--rw-rw-rw-   0        0        0     3593 2024-03-29 11:35:18.000000 nwb4fp-0.6.0.5/src/nwb4fp/main/main_create_nwb.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:36:39.019995 nwb4fp-0.6.0.5/src/nwb4fp/postprocess/
--rw-rw-rw-   0        0        0    15551 2024-03-27 11:37:25.000000 nwb4fp-0.6.0.5/src/nwb4fp/postprocess/Get_positions.py
--rw-rw-rw-   0        0        0        0 2024-02-15 18:06:22.000000 nwb4fp-0.6.0.5/src/nwb4fp/postprocess/__init__.py
--rw-rw-rw-   0        0        0     1639 2024-04-23 18:17:23.000000 nwb4fp-0.6.0.5/src/nwb4fp/postprocess/add_wfcor.py
--rw-rw-rw-   0        0        0      470 2024-03-24 12:00:57.000000 nwb4fp-0.6.0.5/src/nwb4fp/postprocess/dlc_kinematic.py
--rw-rw-rw-   0        0        0     2485 2024-03-29 14:47:19.000000 nwb4fp-0.6.0.5/src/nwb4fp/postprocess/extract_wf.py
--rw-rw-rw-   0        0        0     1343 2024-04-23 15:19:46.000000 nwb4fp-0.6.0.5/src/nwb4fp/postprocess/get_potential_merge.py
--rw-rw-rw-   0        0        0    17067 2024-04-04 14:46:56.000000 nwb4fp-0.6.0.5/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
--rw-rw-rw-   0        0        0    12897 2024-04-23 18:36:02.000000 nwb4fp-0.6.0.5/src/nwb4fp/postprocess/quality_metrix.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:36:39.330001 nwb4fp-0.6.0.5/src/nwb4fp/preprocess/
--rw-rw-rw-   0        0        0        0 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.5/src/nwb4fp/preprocess/__init__.py
--rw-rw-rw-   0        0        0      459 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.5/src/nwb4fp/preprocess/copy_file.py
--rw-rw-rw-   0        0        0      620 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.5/src/nwb4fp/preprocess/down_sample.py
--rw-rw-rw-   0        0        0     6762 2024-03-05 12:39:24.000000 nwb4fp-0.6.0.5/src/nwb4fp/preprocess/down_sample_lfp.py
--rw-rw-rw-   0        0        0     3712 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.5/src/nwb4fp/preprocess/extract_lfp.py
--rw-rw-rw-   0        0        0      148 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.5/src/nwb4fp/preprocess/get_path.py
--rw-rw-rw-   0        0        0     1203 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.5/src/nwb4fp/preprocess/load_data.py
--rw-rw-rw-   0        0        0      244 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.5/src/nwb4fp/preprocess/run_phy.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:36:39.033010 nwb4fp-0.6.0.5/src/nwb4fp/test/
-drwxrwxrwx   0        0        0        0 2024-04-23 18:36:39.033010 nwb4fp-0.6.0.5/src/nwb4fp/test/run_scripts/
--rw-rw-rw-   0        0        0     1552 2024-04-03 09:55:04.000000 nwb4fp-0.6.0.5/src/nwb4fp/test/run_scripts/readnwb.py
--rw-rw-rw-   0        0        0     1428 2024-04-23 16:33:31.000000 nwb4fp-0.6.0.5/src/nwb4fp/test/run_scripts/readnwb_09PC.py
--rw-rw-rw-   0        0        0        0 2024-03-13 14:23:55.000000 nwb4fp-0.6.0.5/src/nwb4fp/test/run_scripts/test.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:36:39.130005 nwb4fp-0.6.0.5/src/nwb4fp.egg-info/
--rw-rw-rw-   0        0        0     5780 2024-04-23 18:36:38.000000 nwb4fp-0.6.0.5/src/nwb4fp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1000 2024-04-23 18:36:38.000000 nwb4fp-0.6.0.5/src/nwb4fp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 18:36:38.000000 nwb4fp-0.6.0.5/src/nwb4fp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2910 2024-04-23 18:36:38.000000 nwb4fp-0.6.0.5/src/nwb4fp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-23 18:36:38.000000 nwb4fp-0.6.0.5/src/nwb4fp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 08:35:11.083603 nwb4fp-0.6.0.6/
+-rw-rw-rw-   0        0        0     1089 2024-02-24 13:06:48.000000 nwb4fp-0.6.0.6/LICENSE
+-rw-rw-rw-   0        0        0     5746 2024-04-24 08:35:11.060613 nwb4fp-0.6.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6901 2024-03-27 14:22:15.000000 nwb4fp-0.6.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 08:35:11.085589 nwb4fp-0.6.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      877 2024-04-24 08:35:05.000000 nwb4fp-0.6.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 08:35:10.369578 nwb4fp-0.6.0.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-24 08:35:10.473610 nwb4fp-0.6.0.6/src/nwb4fp/
+-rw-rw-rw-   0        0        0        0 2024-03-03 17:04:21.000000 nwb4fp-0.6.0.6/src/nwb4fp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 08:35:10.556590 nwb4fp-0.6.0.6/src/nwb4fp/main/
+-rw-rw-rw-   0        0        0        0 2024-03-08 16:12:29.000000 nwb4fp-0.6.0.6/src/nwb4fp/main/__init__.py
+-rw-rw-rw-   0        0        0     3593 2024-03-29 11:35:18.000000 nwb4fp-0.6.0.6/src/nwb4fp/main/main_create_nwb.py
+drwxrwxrwx   0        0        0        0 2024-04-24 08:35:10.673570 nwb4fp-0.6.0.6/src/nwb4fp/postprocess/
+-rw-rw-rw-   0        0        0    15551 2024-03-27 11:37:25.000000 nwb4fp-0.6.0.6/src/nwb4fp/postprocess/Get_positions.py
+-rw-rw-rw-   0        0        0        0 2024-02-15 18:06:22.000000 nwb4fp-0.6.0.6/src/nwb4fp/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     1639 2024-04-23 18:17:23.000000 nwb4fp-0.6.0.6/src/nwb4fp/postprocess/add_wfcor.py
+-rw-rw-rw-   0        0        0      470 2024-03-24 12:00:57.000000 nwb4fp-0.6.0.6/src/nwb4fp/postprocess/dlc_kinematic.py
+-rw-rw-rw-   0        0        0     2485 2024-03-29 14:47:19.000000 nwb4fp-0.6.0.6/src/nwb4fp/postprocess/extract_wf.py
+-rw-rw-rw-   0        0        0     1343 2024-04-23 15:19:46.000000 nwb4fp-0.6.0.6/src/nwb4fp/postprocess/get_potential_merge.py
+-rw-rw-rw-   0        0        0    17067 2024-04-04 14:46:56.000000 nwb4fp-0.6.0.6/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
+-rw-rw-rw-   0        0        0    12897 2024-04-23 18:36:02.000000 nwb4fp-0.6.0.6/src/nwb4fp/postprocess/quality_metrix.py
+drwxrwxrwx   0        0        0        0 2024-04-24 08:35:10.385595 nwb4fp-0.6.0.6/src/nwb4fp/preprocess/
+-rw-rw-rw-   0        0        0        0 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.6/src/nwb4fp/preprocess/__init__.py
+-rw-rw-rw-   0        0        0      459 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.6/src/nwb4fp/preprocess/copy_file.py
+-rw-rw-rw-   0        0        0      620 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.6/src/nwb4fp/preprocess/down_sample.py
+-rw-rw-rw-   0        0        0     6762 2024-03-05 12:39:24.000000 nwb4fp-0.6.0.6/src/nwb4fp/preprocess/down_sample_lfp.py
+-rw-rw-rw-   0        0        0     3712 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.6/src/nwb4fp/preprocess/extract_lfp.py
+-rw-rw-rw-   0        0        0      148 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.6/src/nwb4fp/preprocess/get_path.py
+-rw-rw-rw-   0        0        0     1203 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.6/src/nwb4fp/preprocess/load_data.py
+-rw-rw-rw-   0        0        0      244 2024-02-27 13:40:23.000000 nwb4fp-0.6.0.6/src/nwb4fp/preprocess/run_phy.py
+drwxrwxrwx   0        0        0        0 2024-04-24 08:35:10.394575 nwb4fp-0.6.0.6/src/nwb4fp/test/
+drwxrwxrwx   0        0        0        0 2024-04-24 08:35:10.394575 nwb4fp-0.6.0.6/src/nwb4fp/test/run_scripts/
+-rw-rw-rw-   0        0        0     1552 2024-04-03 09:55:04.000000 nwb4fp-0.6.0.6/src/nwb4fp/test/run_scripts/readnwb.py
+-rw-rw-rw-   0        0        0     1428 2024-04-23 16:33:31.000000 nwb4fp-0.6.0.6/src/nwb4fp/test/run_scripts/readnwb_09PC.py
+-rw-rw-rw-   0        0        0        0 2024-03-13 14:23:55.000000 nwb4fp-0.6.0.6/src/nwb4fp/test/run_scripts/test.py
+drwxrwxrwx   0        0        0        0 2024-04-24 08:35:10.533586 nwb4fp-0.6.0.6/src/nwb4fp.egg-info/
+-rw-rw-rw-   0        0        0     5746 2024-04-24 08:35:09.000000 nwb4fp-0.6.0.6/src/nwb4fp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1000 2024-04-24 08:35:10.000000 nwb4fp-0.6.0.6/src/nwb4fp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 08:35:10.000000 nwb4fp-0.6.0.6/src/nwb4fp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2892 2024-04-24 08:35:10.000000 nwb4fp-0.6.0.6/src/nwb4fp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-24 08:35:10.000000 nwb4fp-0.6.0.6/src/nwb4fp.egg-info/top_level.txt
```

### Comparing `nwb4fp-0.6.0.5/LICENSE` & `nwb4fp-0.6.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.5/PKG-INFO` & `nwb4fp-0.6.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.6.0.5
+Version: 0.6.0.6
 Summary: Description of my package
 Home-page: https://github.com/sachuriga283/nwb4fp
 Author: sachuriga283
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
@@ -84,15 +84,15 @@
 Requires-Dist: natsort==8.4.0
 Requires-Dist: nbclient==0.9.0
 Requires-Dist: nbconvert==7.16.1
 Requires-Dist: nbformat==5.9.2
 Requires-Dist: ndindex==1.8
 Requires-Dist: neo==0.13.0
 Requires-Dist: nest-asyncio==1.6.0
-Requires-Dist: neuroconv==0.4.6
+Requires-Dist: neuroconv==0.4.8
 Requires-Dist: nh3==0.2.15
 Requires-Dist: notebook==7.1.1
 Requires-Dist: notebook_shim==0.2.4
 Requires-Dist: numba==0.59.0
 Requires-Dist: numcodecs==0.11.0
 Requires-Dist: numexpr==2.9.0
 Requires-Dist: numpy==1.26.4
@@ -109,15 +109,14 @@
 Requires-Dist: probeinterface==0.2.21
 Requires-Dist: prometheus_client==0.20.0
 Requires-Dist: prompt-toolkit==3.0.43
 Requires-Dist: psutil==5.9.8
 Requires-Dist: pure-eval==0.2.2
 Requires-Dist: py-cpuinfo==9.0.0
 Requires-Dist: pycparser==2.21
-Requires-Dist: pydantic==1.10.14
 Requires-Dist: Pygments==2.17.2
 Requires-Dist: pynwb==2.6.0
 Requires-Dist: pyopenephys==1.2.0
 Requires-Dist: pyparsing==3.1.1
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: python-json-logger==2.0.7
 Requires-Dist: pytz==2024.1
```

### Comparing `nwb4fp-0.6.0.5/README.md` & `nwb4fp-0.6.0.6/README.md`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.5/setup.py` & `nwb4fp-0.6.0.6/setup.py`

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
-    version='0.6.0.5',
+    version='0.6.0.6',
     url='https://github.com/sachuriga283/nwb4fp',
     author='sachuriga283',
     author_email='sachuriga.sachuriga@ntnu.no',
     description='Description of my package',
     #packages=find_packages(./src/),    
     install_requires=read_requirements(),
 )
```

### Comparing `nwb4fp-0.6.0.5/src/nwb4fp/main/main_create_nwb.py` & `nwb4fp-0.6.0.6/src/nwb4fp/main/main_create_nwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.5/src/nwb4fp/postprocess/Get_positions.py` & `nwb4fp-0.6.0.6/src/nwb4fp/postprocess/Get_positions.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.5/src/nwb4fp/postprocess/add_wfcor.py` & `nwb4fp-0.6.0.6/src/nwb4fp/postprocess/add_wfcor.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.5/src/nwb4fp/postprocess/extract_wf.py` & `nwb4fp-0.6.0.6/src/nwb4fp/postprocess/extract_wf.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.5/src/nwb4fp/postprocess/get_potential_merge.py` & `nwb4fp-0.6.0.6/src/nwb4fp/postprocess/get_potential_merge.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.5/src/nwb4fp/postprocess/nwbPHYnOPHYS.py` & `nwb4fp-0.6.0.6/src/nwb4fp/postprocess/nwbPHYnOPHYS.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.5/src/nwb4fp/postprocess/quality_metrix.py` & `nwb4fp-0.6.0.6/src/nwb4fp/postprocess/quality_metrix.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.5/src/nwb4fp/preprocess/down_sample.py` & `nwb4fp-0.6.0.6/src/nwb4fp/preprocess/down_sample.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.5/src/nwb4fp/preprocess/down_sample_lfp.py` & `nwb4fp-0.6.0.6/src/nwb4fp/preprocess/down_sample_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.5/src/nwb4fp/preprocess/extract_lfp.py` & `nwb4fp-0.6.0.6/src/nwb4fp/preprocess/extract_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.5/src/nwb4fp/preprocess/load_data.py` & `nwb4fp-0.6.0.6/src/nwb4fp/preprocess/load_data.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.5/src/nwb4fp/test/run_scripts/readnwb.py` & `nwb4fp-0.6.0.6/src/nwb4fp/test/run_scripts/readnwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.5/src/nwb4fp/test/run_scripts/readnwb_09PC.py` & `nwb4fp-0.6.0.6/src/nwb4fp/test/run_scripts/readnwb_09PC.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.5/src/nwb4fp.egg-info/PKG-INFO` & `nwb4fp-0.6.0.6/src/nwb4fp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.6.0.5
+Version: 0.6.0.6
 Summary: Description of my package
 Home-page: https://github.com/sachuriga283/nwb4fp
 Author: sachuriga283
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
@@ -84,15 +84,15 @@
 Requires-Dist: natsort==8.4.0
 Requires-Dist: nbclient==0.9.0
 Requires-Dist: nbconvert==7.16.1
 Requires-Dist: nbformat==5.9.2
 Requires-Dist: ndindex==1.8
 Requires-Dist: neo==0.13.0
 Requires-Dist: nest-asyncio==1.6.0
-Requires-Dist: neuroconv==0.4.6
+Requires-Dist: neuroconv==0.4.8
 Requires-Dist: nh3==0.2.15
 Requires-Dist: notebook==7.1.1
 Requires-Dist: notebook_shim==0.2.4
 Requires-Dist: numba==0.59.0
 Requires-Dist: numcodecs==0.11.0
 Requires-Dist: numexpr==2.9.0
 Requires-Dist: numpy==1.26.4
@@ -109,15 +109,14 @@
 Requires-Dist: probeinterface==0.2.21
 Requires-Dist: prometheus_client==0.20.0
 Requires-Dist: prompt-toolkit==3.0.43
 Requires-Dist: psutil==5.9.8
 Requires-Dist: pure-eval==0.2.2
 Requires-Dist: py-cpuinfo==9.0.0
 Requires-Dist: pycparser==2.21
-Requires-Dist: pydantic==1.10.14
 Requires-Dist: Pygments==2.17.2
 Requires-Dist: pynwb==2.6.0
 Requires-Dist: pyopenephys==1.2.0
 Requires-Dist: pyparsing==3.1.1
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: python-json-logger==2.0.7
 Requires-Dist: pytz==2024.1
```

### Comparing `nwb4fp-0.6.0.5/src/nwb4fp.egg-info/SOURCES.txt` & `nwb4fp-0.6.0.6/src/nwb4fp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.0.5/src/nwb4fp.egg-info/requires.txt` & `nwb4fp-0.6.0.6/src/nwb4fp.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 natsort==8.4.0
 nbclient==0.9.0
 nbconvert==7.16.1
 nbformat==5.9.2
 ndindex==1.8
 neo==0.13.0
 nest-asyncio==1.6.0
-neuroconv==0.4.6
+neuroconv==0.4.8
 nh3==0.2.15
 notebook==7.1.1
 notebook_shim==0.2.4
 numba==0.59.0
 numcodecs==0.11.0
 numexpr==2.9.0
 numpy==1.26.4
@@ -101,15 +101,14 @@
 probeinterface==0.2.21
 prometheus_client==0.20.0
 prompt-toolkit==3.0.43
 psutil==5.9.8
 pure-eval==0.2.2
 py-cpuinfo==9.0.0
 pycparser==2.21
-pydantic==1.10.14
 Pygments==2.17.2
 pynwb==2.6.0
 pyopenephys==1.2.0
 pyparsing==3.1.1
 python-dateutil==2.8.2
 python-json-logger==2.0.7
 pytz==2024.1
```

