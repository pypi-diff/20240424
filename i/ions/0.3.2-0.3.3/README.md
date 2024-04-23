# Comparing `tmp/ions-0.3.2.tar.gz` & `tmp/ions-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ions-0.3.2.tar", last modified: Mon Apr 22 21:10:34 2024, max compression
+gzip compressed data, was "ions-0.3.3.tar", last modified: Tue Apr 23 21:54:56 2024, max compression
```

## Comparing `ions-0.3.2.tar` & `ions-0.3.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-22 21:10:34.691674 ions-0.3.2/
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1074 2023-10-31 13:23:17.000000 ions-0.3.2/LICENSE
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)      206 2023-11-21 18:10:05.000000 ions-0.3.2/MANIFEST.in
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    12151 2024-04-22 21:10:34.691184 ions-0.3.2/PKG-INFO
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    11435 2024-04-04 13:33:19.000000 ions-0.3.2/README.md
-drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-22 21:10:34.682670 ions-0.3.2/ions/
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)       32 2023-12-28 10:50:17.000000 ions-0.3.2/ions/__init__.py
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    10237 2024-04-16 11:59:59.000000 ions-0.3.2/ions/calculators.py
-drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-22 21:10:34.688639 ions-0.3.2/ions/data/
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     5337 2023-11-09 08:42:48.000000 ions-0.3.2/ions/data/Li2O_mp-1960.cif
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1770 2023-11-19 14:10:41.000000 ions-0.3.2/ions/data/bvparam_1991.yaml
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    43938 2023-11-16 11:52:28.000000 ions-0.3.2/ions/data/bvparams2020-average.json
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    62564 2023-11-16 11:52:28.000000 ions-0.3.2/ions/data/bvparams2020-average.pickle
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    22301 2023-11-16 11:52:28.000000 ions-0.3.2/ions/data/bvparams_averaged2020.csv
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    96425 2023-11-14 16:11:16.000000 ions-0.3.2/ions/data/bvparm2020.cif
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    94027 2023-11-14 16:29:49.000000 ions-0.3.2/ions/data/bvparm2020_edit.txt
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    48466 2023-11-16 11:52:28.000000 ions-0.3.2/ions/data/bvse_data.json
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    56330 2023-11-16 11:52:28.000000 ions-0.3.2/ions/data/bvse_data.pickle
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)      971 2023-11-19 14:35:25.000000 ions-0.3.2/ions/data/elneg_data.json
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    34095 2023-11-19 14:58:05.000000 ions-0.3.2/ions/data/icsd_bv.yaml
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)        1 2023-11-19 15:13:12.000000 ions-0.3.2/ions/data/icsd_bv_data.json
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3217 2022-11-10 13:13:57.000000 ions-0.3.2/ions/data/quantum_n.pkl
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3845 2023-11-16 11:52:28.000000 ions-0.3.2/ions/data/shannon-data-crystal.json
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3121 2023-11-16 11:52:28.000000 ions-0.3.2/ions/data/shannon-data-crystal.pickle
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3882 2023-11-16 11:52:28.000000 ions-0.3.2/ions/data/shannon-data-ionic.json
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3121 2023-11-16 11:52:28.000000 ions-0.3.2/ions/data/shannon-data-ionic.pickle
--rw-rw-r--   0 artemdembitskiy   (501) staff       (20)    37813 2014-07-16 19:56:01.000000 ions-0.3.2/ions/data/shannon-radii.json
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    20356 2023-11-16 11:52:28.000000 ions-0.3.2/ions/data/shannon-radii.pickle
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1307 2023-11-20 19:21:33.000000 ions-0.3.2/ions/data.py
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    10438 2024-04-04 13:35:35.000000 ions-0.3.2/ions/decorator.py
-drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-22 21:10:34.688813 ions-0.3.2/ions/featurizers/
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)       44 2024-04-01 14:09:37.000000 ions-0.3.2/ions/featurizers/__init__.py
-drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-22 21:10:34.689497 ions-0.3.2/ions/geom/
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)       43 2024-04-16 10:55:19.000000 ions-0.3.2/ions/geom/__init__.py
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     2398 2024-04-17 09:40:16.000000 ions-0.3.2/ions/geom/box.py
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     5256 2024-04-18 12:25:27.000000 ions-0.3.2/ions/geom/edge.py
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1799 2024-04-22 21:08:32.000000 ions-0.3.2/ions/geom/utils.py
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     4631 2024-04-08 08:34:14.000000 ions-0.3.2/ions/potential.py
-drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-22 21:10:34.690689 ions-0.3.2/ions/tools/
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)       74 2024-04-16 10:55:28.000000 ions-0.3.2/ions/tools/__init__.py
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    15102 2024-04-04 13:01:13.000000 ions-0.3.2/ions/tools/percolator.py
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     2968 2024-04-16 11:58:30.000000 ions-0.3.2/ions/tools/saddle_finder.py
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     4742 2024-04-04 06:53:48.000000 ions-0.3.2/ions/utils.py
-drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-22 21:10:34.684958 ions-0.3.2/ions.egg-info/
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)    12151 2024-04-22 21:10:34.000000 ions-0.3.2/ions.egg-info/PKG-INFO
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1035 2024-04-22 21:10:34.000000 ions-0.3.2/ions.egg-info/SOURCES.txt
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)        1 2024-04-22 21:10:34.000000 ions-0.3.2/ions.egg-info/dependency_links.txt
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)       49 2024-04-22 21:10:34.000000 ions-0.3.2/ions.egg-info/requires.txt
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)        5 2024-04-22 21:10:34.000000 ions-0.3.2/ions.egg-info/top_level.txt
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)       38 2024-04-22 21:10:34.691747 ions-0.3.2/setup.cfg
--rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1537 2024-04-16 12:32:21.000000 ions-0.3.2/setup.py
+drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-23 21:54:56.197114 ions-0.3.3/
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1074 2023-10-31 13:23:17.000000 ions-0.3.3/LICENSE
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)      206 2023-11-21 18:10:05.000000 ions-0.3.3/MANIFEST.in
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    12151 2024-04-23 21:54:56.196854 ions-0.3.3/PKG-INFO
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    11435 2024-04-04 13:33:19.000000 ions-0.3.3/README.md
+drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-23 21:54:56.180790 ions-0.3.3/ions/
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)       32 2023-12-28 10:50:17.000000 ions-0.3.3/ions/__init__.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    10237 2024-04-16 11:59:59.000000 ions-0.3.3/ions/calculators.py
+drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-23 21:54:56.194406 ions-0.3.3/ions/data/
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     5337 2023-11-09 08:42:48.000000 ions-0.3.3/ions/data/Li2O_mp-1960.cif
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1770 2023-11-19 14:10:41.000000 ions-0.3.3/ions/data/bvparam_1991.yaml
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    43938 2023-11-16 11:52:28.000000 ions-0.3.3/ions/data/bvparams2020-average.json
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    62564 2023-11-16 11:52:28.000000 ions-0.3.3/ions/data/bvparams2020-average.pickle
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    22301 2023-11-16 11:52:28.000000 ions-0.3.3/ions/data/bvparams_averaged2020.csv
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    96425 2023-11-14 16:11:16.000000 ions-0.3.3/ions/data/bvparm2020.cif
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    94027 2023-11-14 16:29:49.000000 ions-0.3.3/ions/data/bvparm2020_edit.txt
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    48466 2023-11-16 11:52:28.000000 ions-0.3.3/ions/data/bvse_data.json
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    56330 2023-11-16 11:52:28.000000 ions-0.3.3/ions/data/bvse_data.pickle
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)      971 2023-11-19 14:35:25.000000 ions-0.3.3/ions/data/elneg_data.json
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    34095 2023-11-19 14:58:05.000000 ions-0.3.3/ions/data/icsd_bv.yaml
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)        1 2023-11-19 15:13:12.000000 ions-0.3.3/ions/data/icsd_bv_data.json
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3217 2022-11-10 13:13:57.000000 ions-0.3.3/ions/data/quantum_n.pkl
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3845 2023-11-16 11:52:28.000000 ions-0.3.3/ions/data/shannon-data-crystal.json
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3121 2023-11-16 11:52:28.000000 ions-0.3.3/ions/data/shannon-data-crystal.pickle
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3882 2023-11-16 11:52:28.000000 ions-0.3.3/ions/data/shannon-data-ionic.json
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     3121 2023-11-16 11:52:28.000000 ions-0.3.3/ions/data/shannon-data-ionic.pickle
+-rw-rw-r--   0 artemdembitskiy   (501) staff       (20)    37813 2014-07-16 19:56:01.000000 ions-0.3.3/ions/data/shannon-radii.json
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    20356 2023-11-16 11:52:28.000000 ions-0.3.3/ions/data/shannon-radii.pickle
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1307 2023-11-20 19:21:33.000000 ions-0.3.3/ions/data.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    10438 2024-04-04 13:35:35.000000 ions-0.3.3/ions/decorator.py
+drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-23 21:54:56.194954 ions-0.3.3/ions/featurizers/
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)       44 2024-04-01 14:09:37.000000 ions-0.3.3/ions/featurizers/__init__.py
+drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-23 21:54:56.195736 ions-0.3.3/ions/geom/
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)       43 2024-04-23 15:07:12.000000 ions-0.3.3/ions/geom/__init__.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     2398 2024-04-23 12:00:59.000000 ions-0.3.3/ions/geom/box.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     5369 2024-04-23 20:36:28.000000 ions-0.3.3/ions/geom/edge.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     5687 2024-04-23 21:54:09.000000 ions-0.3.3/ions/geom/utils.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     4631 2024-04-08 08:34:14.000000 ions-0.3.3/ions/potential.py
+drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-23 21:54:56.196369 ions-0.3.3/ions/tools/
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)       74 2024-04-16 10:55:28.000000 ions-0.3.3/ions/tools/__init__.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    15102 2024-04-04 13:01:13.000000 ions-0.3.3/ions/tools/percolator.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     2968 2024-04-16 11:58:30.000000 ions-0.3.3/ions/tools/saddle_finder.py
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     4888 2024-04-23 20:30:14.000000 ions-0.3.3/ions/utils.py
+drwxr-xr-x   0 artemdembitskiy   (501) staff       (20)        0 2024-04-23 21:54:56.182473 ions-0.3.3/ions.egg-info/
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)    12151 2024-04-23 21:54:56.000000 ions-0.3.3/ions.egg-info/PKG-INFO
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1035 2024-04-23 21:54:56.000000 ions-0.3.3/ions.egg-info/SOURCES.txt
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)        1 2024-04-23 21:54:56.000000 ions-0.3.3/ions.egg-info/dependency_links.txt
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)       49 2024-04-23 21:54:56.000000 ions-0.3.3/ions.egg-info/requires.txt
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)        5 2024-04-23 21:54:56.000000 ions-0.3.3/ions.egg-info/top_level.txt
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)       38 2024-04-23 21:54:56.197187 ions-0.3.3/setup.cfg
+-rw-r--r--   0 artemdembitskiy   (501) staff       (20)     1537 2024-04-23 21:54:25.000000 ions-0.3.3/setup.py
```

### Comparing `ions-0.3.2/LICENSE` & `ions-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ions-0.3.2/PKG-INFO` & `ions-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ions
-Version: 0.3.2
+Version: 0.3.3
 Summary: A python library for studying percolation in solids
 Home-page: https://github.com/dembart/ions
 Author: Artem Dembitskiy
 Author-email: art.dembitskiy@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `ions-0.3.2/README.md` & `ions-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `ions-0.3.2/ions/calculators.py` & `ions-0.3.3/ions/calculators.py`

 * *Files identical despite different names*

### Comparing `ions-0.3.2/ions/data/Li2O_mp-1960.cif` & `ions-0.3.3/ions/data/Li2O_mp-1960.cif`

 * *Files identical despite different names*

### Comparing `ions-0.3.2/ions/data/bvparam_1991.yaml` & `ions-0.3.3/ions/data/bvparam_1991.yaml`

 * *Files identical despite different names*

### Comparing `ions-0.3.2/ions/data/bvparams2020-average.json` & `ions-0.3.3/ions/data/bvparams2020-average.json`

 * *Files identical despite different names*

### Comparing `ions-0.3.2/ions/data/bvparams2020-average.pickle` & `ions-0.3.3/ions/data/bvparams2020-average.pickle`

 * *Files identical despite different names*

### Comparing `ions-0.3.2/ions/data/bvparams_averaged2020.csv` & `ions-0.3.3/ions/data/bvparams_averaged2020.csv`

 * *Files identical despite different names*

### Comparing `ions-0.3.2/ions/data/bvparm2020.cif` & `ions-0.3.3/ions/data/bvparm2020.cif`

 * *Files identical despite different names*

### Comparing `ions-0.3.2/ions/data/bvparm2020_edit.txt` & `ions-0.3.3/ions/data/bvparm2020_edit.txt`

 * *Files identical despite different names*

### Comparing `ions-0.3.2/ions/data/bvse_data.json` & `ions-0.3.3/ions/data/bvse_data.json`

 * *Files identical despite different names*

### Comparing `ions-0.3.2/ions/data/bvse_data.pickle` & `ions-0.3.3/ions/data/bvse_data.pickle`

 * *Files identical despite different names*

### Comparing `ions-0.3.2/ions/data/elneg_data.json` & `ions-0.3.3/ions/data/elneg_data.json`

 * *Files identical despite different names*

### Comparing `ions-0.3.2/ions/data/icsd_bv.yaml` & `ions-0.3.3/ions/data/icsd_bv.yaml`

 * *Files identical despite different names*

### Comparing `ions-0.3.2/ions/data/quantum_n.pkl` & `ions-0.3.3/ions/data/quantum_n.pkl`

 * *Files identical despite different names*

### Comparing `ions-0.3.2/ions/data/shannon-data-crystal.json` & `ions-0.3.3/ions/data/shannon-data-crystal.json`

 * *Files identical despite different names*

### Comparing `ions-0.3.2/ions/data/shannon-data-crystal.pickle` & `ions-0.3.3/ions/data/shannon-data-crystal.pickle`

 * *Files identical despite different names*

### Comparing `ions-0.3.2/ions/data/shannon-data-ionic.json` & `ions-0.3.3/ions/data/shannon-data-ionic.json`

 * *Files identical despite different names*

### Comparing `ions-0.3.2/ions/data/shannon-data-ionic.pickle` & `ions-0.3.3/ions/data/shannon-data-ionic.pickle`

 * *Files identical despite different names*

### Comparing `ions-0.3.2/ions/data/shannon-radii.json` & `ions-0.3.3/ions/data/shannon-radii.json`

 * *Files identical despite different names*

### Comparing `ions-0.3.2/ions/data/shannon-radii.pickle` & `ions-0.3.3/ions/data/shannon-radii.pickle`

 * *Files identical despite different names*

### Comparing `ions-0.3.2/ions/data.py` & `ions-0.3.3/ions/data.py`

 * *Files identical despite different names*

### Comparing `ions-0.3.2/ions/decorator.py` & `ions-0.3.3/ions/decorator.py`

 * *Files identical despite different names*

### Comparing `ions-0.3.2/ions/geom/box.py` & `ions-0.3.3/ions/geom/box.py`

 * *Files identical despite different names*

### Comparing `ions-0.3.2/ions/geom/edge.py` & `ions-0.3.3/ions/geom/edge.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self.p2 = np.dot(self.offset, self.cell) + self.atoms.positions[self.target]
         self.wrapped_target = self._wrapped_target()
 
     @property
     def length(self):
         return np.linalg.norm(self.p1 - self.p2)
     
-    #@property
+    
     def _wrapped_target(self):
         p2_scaled = self.cell.scaled_positions(self.p2).round(10) # rounding for a safer wrapping
         p2_scaled[:]%=1.0
         p2_wrapped = self.cell.cartesian_positions(p2_scaled)
         target_specie = self.atoms.numbers[self.target]
         specie_ids = np.argwhere(self.atoms.numbers == target_specie).ravel()
         atoms = self.atoms.copy()
@@ -52,26 +52,28 @@
         target = int(specie_ids[index])
         if distance > 1e-8:
             print('target was not properly wrapped', distance)
             raise
         assert self.atoms.numbers[self.target] == self.atoms.numbers[target] # not needed
         return target
 
-    #@property
     def nn(self, r_cut = None):
         if r_cut == None:
             r_cut = 2 * self.length # this is heuristics but should work well
         edge = self.superedge(r_cut, center = True)
+        #edge.atoms.wrap()
         frame_ids = np.array([i for i in range(len(edge.atoms)) if i not in [edge.source, edge.wrapped_target]])
         p = edge.atoms.positions[frame_ids]
         a = edge.atoms.positions[edge.source]
-        b = edge.atoms.positions[edge.wrapped_target]
+        b = edge.atoms.positions[edge.target] + np.dot(edge.offset, edge.cell)
         dd = lineseg_dists(p, a, b)
         nn_id = frame_ids[np.where(dd == dd.min())[0][0]]
-        return {'min_dist': dd.min(), 'nn': nn_id, 'nnp': self._project_point_on_edge(p[nn_id])}
+        image = edge.atoms.copy()
+        image.append('Pd')
+        return {'min_dist': dd.min(), 'nn': nn_id, 'nnp': edge._project_point_on_edge(p[nn_id])}
     
 
     def _project_point_on_edge(self, p):
         ap = p-self.p1
         ab = self.p2 - self.p1
         result = self.p1 + np.dot(ap,ab)/np.dot(ab,ab) * ab
         return result
@@ -86,14 +88,15 @@
             p2 = supercell.positions[self.target] + np.dot(self.offset, self.cell)
             d = np.linalg.norm(p1 - p2)
             assert abs(d - self.length) < 1e-10
             centroid = (p1 + p2) / 2
             box_center = np.dot([0.5, 0.5, 0.5], supercell.cell)
             shift = box_center - centroid
             supercell.positions += shift
+        supercell.wrap()
         offset = self.offset / scale
         return Edge(supercell, self.source, self.target, offset)
     
 
     @property
     def centroid(self):
         return (self.p1 +  self.p2) / 2
```

### Comparing `ions-0.3.2/ions/potential.py` & `ions-0.3.3/ions/potential.py`

 * *Files identical despite different names*

### Comparing `ions-0.3.2/ions/tools/percolator.py` & `ions-0.3.3/ions/tools/percolator.py`

 * *Files identical despite different names*

### Comparing `ions-0.3.2/ions/tools/saddle_finder.py` & `ions-0.3.3/ions/tools/saddle_finder.py`

 * *Files identical despite different names*

### Comparing `ions-0.3.2/ions/utils.py` & `ions-0.3.3/ions/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import itertools
 import numpy as np
 from scipy.spatial.distance import cdist, euclidean
+
 from scipy.optimize import minimize
 from ase.data import atomic_numbers, covalent_radii
 from ions.data import bvse_data, principle_number
 
+
+
 def collect_bvse_params(atoms, symbol, charge, self_interaction = True):
     
     s1 = symbol
     z1 = atomic_numbers[symbol]
     q1 = charge
     n1 = principle_number[z1]
     rc1 = covalent_radii[z1]
@@ -137,8 +140,17 @@
     if np.all(a == b):
         return np.linalg.norm(p - a, axis=1)
     d = np.divide(b - a, np.linalg.norm(b - a))
     s = np.dot(a - p, d)
     t = np.dot(p - b, d)
     h = np.maximum.reduce([s, t, np.zeros(len(p))])
     c = np.cross(p - a, d)
-    return np.hypot(h, np.linalg.norm(c, axis = 1))
+    return np.hypot(h, np.linalg.norm(c, axis = 1))
+
+
+def project_point_on_edge(p, p1, p2):
+    ap = p-p1
+    ab = p2 - p1
+    result = p1 + np.dot(ap,ab)/np.dot(ab,ab) * ab
+    return result
+
+
```

### Comparing `ions-0.3.2/ions.egg-info/PKG-INFO` & `ions-0.3.3/ions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ions
-Version: 0.3.2
+Version: 0.3.3
 Summary: A python library for studying percolation in solids
 Home-page: https://github.com/dembart/ions
 Author: Artem Dembitskiy
 Author-email: art.dembitskiy@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `ions-0.3.2/ions.egg-info/SOURCES.txt` & `ions-0.3.3/ions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ions-0.3.2/setup.py` & `ions-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='ions',  
-     version='0.3.2',
+     version='0.3.3',
      py_modules = ["ions"],
      install_requires = [
                          "ase>=3.22.1",
                          "numpy",
 			             "spglib",
                          "networkx",
                          "scipy",
```

