# Comparing `tmp/cnspy_timestamp_association-0.1.1.tar.gz` & `tmp/cnspy_timestamp_association-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/jungr/workspace/CNS/VIO_Evaluation_Framework/py3_pkgs/cnspy_eco_system_test/pkgs/c_timestamp_association/dist/tmpoxq50ajf", last modified: Sat Mar 20 14:23:37 2021, max compression
+gzip compressed data, was "cnspy_timestamp_association-0.2.0.tar", last modified: Wed Apr 24 12:16:43 2024, max compression
```

## Comparing `cnspy_timestamp_association-0.1.1.tar` & `cnspy_timestamp_association-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 14:23:37.685984 cnspy_timestamp_association-0.1.1/
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     1775 2021-03-20 14:23:37.685984 cnspy_timestamp_association-0.1.1/PKG-INFO
--rw-rw-r--   0 jungr     (1000) jungr     (1000)      858 2021-03-20 14:21:27.000000 cnspy_timestamp_association-0.1.1/README.md
-drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 14:23:37.685984 cnspy_timestamp_association-0.1.1/cnspy_timestamp_association/
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)     2759 2021-03-20 12:20:48.000000 cnspy_timestamp_association-0.1.1/cnspy_timestamp_association/TimestampAssociation.py
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 12:20:48.000000 cnspy_timestamp_association-0.1.1/cnspy_timestamp_association/__init__.py
-drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 14:23:37.685984 cnspy_timestamp_association-0.1.1/cnspy_timestamp_association.egg-info/
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     1775 2021-03-20 14:23:37.000000 cnspy_timestamp_association-0.1.1/cnspy_timestamp_association.egg-info/PKG-INFO
--rw-rw-r--   0 jungr     (1000) jungr     (1000)      415 2021-03-20 14:23:37.000000 cnspy_timestamp_association-0.1.1/cnspy_timestamp_association.egg-info/SOURCES.txt
--rw-rw-r--   0 jungr     (1000) jungr     (1000)        1 2021-03-20 14:23:37.000000 cnspy_timestamp_association-0.1.1/cnspy_timestamp_association.egg-info/dependency_links.txt
--rw-rw-r--   0 jungr     (1000) jungr     (1000)        6 2021-03-20 14:23:37.000000 cnspy_timestamp_association-0.1.1/cnspy_timestamp_association.egg-info/requires.txt
--rw-rw-r--   0 jungr     (1000) jungr     (1000)       33 2021-03-20 14:23:37.000000 cnspy_timestamp_association-0.1.1/cnspy_timestamp_association.egg-info/top_level.txt
--rw-rw-r--   0 jungr     (1000) jungr     (1000)       38 2021-03-20 14:23:37.685984 cnspy_timestamp_association-0.1.1/setup.cfg
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     1266 2021-03-20 14:21:27.000000 cnspy_timestamp_association-0.1.1/setup.py
-drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 14:23:37.685984 cnspy_timestamp_association-0.1.1/test/
--rwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2021-03-20 12:20:48.000000 cnspy_timestamp_association-0.1.1/test/__init__.py
--rw-rw-r--   0 jungr     (1000) jungr     (1000)     2633 2021-03-20 12:20:48.000000 cnspy_timestamp_association-0.1.1/test/test_TimestampAssociation.py
+drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2024-04-24 12:16:43.441220 cnspy_timestamp_association-0.2.0/
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)    35149 2022-05-30 14:10:28.000000 cnspy_timestamp_association-0.2.0/LICENCE
+-rw-r--r--   0 jungr     (1000) jungr     (1000)     1690 2024-04-24 12:16:43.441220 cnspy_timestamp_association-0.2.0/PKG-INFO
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     1002 2022-05-30 14:10:28.000000 cnspy_timestamp_association-0.2.0/README.md
+drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2024-04-24 12:16:43.441220 cnspy_timestamp_association-0.2.0/cnspy_timestamp_association/
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)     3557 2024-04-24 11:45:25.000000 cnspy_timestamp_association-0.2.0/cnspy_timestamp_association/TimestampAssociation.py
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2022-05-30 14:10:28.000000 cnspy_timestamp_association-0.2.0/cnspy_timestamp_association/__init__.py
+drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2024-04-24 12:16:43.441220 cnspy_timestamp_association-0.2.0/cnspy_timestamp_association.egg-info/
+-rw-r--r--   0 jungr     (1000) jungr     (1000)     1690 2024-04-24 12:16:43.000000 cnspy_timestamp_association-0.2.0/cnspy_timestamp_association.egg-info/PKG-INFO
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)      423 2024-04-24 12:16:43.000000 cnspy_timestamp_association-0.2.0/cnspy_timestamp_association.egg-info/SOURCES.txt
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)        1 2024-04-24 12:16:43.000000 cnspy_timestamp_association-0.2.0/cnspy_timestamp_association.egg-info/dependency_links.txt
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)        6 2024-04-24 12:16:43.000000 cnspy_timestamp_association-0.2.0/cnspy_timestamp_association.egg-info/requires.txt
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)       33 2024-04-24 12:16:43.000000 cnspy_timestamp_association-0.2.0/cnspy_timestamp_association.egg-info/top_level.txt
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)       38 2024-04-24 12:16:43.441220 cnspy_timestamp_association-0.2.0/setup.cfg
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     1266 2022-05-30 14:10:28.000000 cnspy_timestamp_association-0.2.0/setup.py
+drwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2024-04-24 12:16:43.441220 cnspy_timestamp_association-0.2.0/test/
+-rwxrwxr-x   0 jungr     (1000) jungr     (1000)        0 2022-05-30 14:10:28.000000 cnspy_timestamp_association-0.2.0/test/__init__.py
+-rw-rw-r--   0 jungr     (1000) jungr     (1000)     2633 2022-05-30 14:10:28.000000 cnspy_timestamp_association-0.2.0/test/test_TimestampAssociation.py
```

### Comparing `cnspy_timestamp_association-0.1.1/PKG-INFO` & `cnspy_timestamp_association-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 Metadata-Version: 2.1
 Name: cnspy_timestamp_association
-Version: 0.1.1
+Version: 0.2.0
 Summary: Associates vectors of timestamps.
 Home-page: https://github.com/aau-cns/cnspy_timestamp_association/
 Author: Roland Jung
 Author-email: roland.jung@aau.at
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/aau-cns/cnspy_timestamp_association/issues
-Description: # cnspy_timestamp_association
-        
-        The class `TimestampAssociation` finds correspondences between to vectors, in our case containing timestamps. The aim is to find timestamp pairs with a configurable  `max_difference`.
-        
-        ## Installation
-        
-        Install the current code base from GitHub and pip install a link to that cloned copy
-        ```
-        git clone https://github.com/aau-cns/cnspy_timestamp_association.git
-        cd cnspy_timestamp_association
-        pip install -e .
-        ```
-        
-        ## Dependencies
-        
-        It is part of the [cnspy eco-system](hhttps://github.com/aau-cns/cnspy_eco_system_test) of the [cns-github](https://github.com/aau-cns) group.  
-        
-        * [numpy]()
-        
-        ## Examples
-        
-        Please refer to the unit-test section in `TimestampAssociation.py`.
-        
-        ## License
-        
-        Software License Agreement (GNU GPLv3  License), refer to the LICENSE file.
-        
-        *Sharing is caring!* - [Roland Jung](https://github.com/jungr-ait)
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENCE
+Requires-Dist: numpy
+
+# cnspy_timestamp_association
+
+The class `TimestampAssociation` finds correspondences between to vectors, in our case containing timestamps. The aim is to find timestamp pairs with a configurable  `max_difference`.
+
+## Installation
+
+Install the current code base from GitHub and pip install a link to that cloned copy
+```
+git clone https://github.com/aau-cns/cnspy_timestamp_association.git
+cd cnspy_timestamp_association
+pip install -e .
+```
+or the [official package](https://pypi.org/project/cnspy-timestamp-association/) via
+```commandline
+pip install cnspy-timestamp-association
+```
+
+## Dependencies
+
+It is part of the [cnspy eco-system](hhttps://github.com/aau-cns/cnspy_eco_system_test) of the [cns-github](https://github.com/aau-cns) group.  
+
+* [numpy]()
+
+## Examples
+
+Please refer to the unit-test section in `TimestampAssociation.py`.
+
+## License
+
+Software License Agreement (GNU GPLv3  License), refer to the LICENSE file.
+
+*Sharing is caring!* - [Roland Jung](https://github.com/jungr-ait)
```

### Comparing `cnspy_timestamp_association-0.1.1/README.md` & `cnspy_timestamp_association-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 
 Install the current code base from GitHub and pip install a link to that cloned copy
 ```
 git clone https://github.com/aau-cns/cnspy_timestamp_association.git
 cd cnspy_timestamp_association
 pip install -e .
 ```
+or the [official package](https://pypi.org/project/cnspy-timestamp-association/) via
+```commandline
+pip install cnspy-timestamp-association
+```
 
 ## Dependencies
 
 It is part of the [cnspy eco-system](hhttps://github.com/aau-cns/cnspy_eco_system_test) of the [cns-github](https://github.com/aau-cns) group.  
 
 * [numpy]()
```

### Comparing `cnspy_timestamp_association-0.1.1/cnspy_timestamp_association/TimestampAssociation.py` & `cnspy_timestamp_association-0.2.0/cnspy_timestamp_association/TimestampAssociation.py`

 * *Files 26% similar despite different names*

```diff
@@ -38,34 +38,52 @@
         prev_idx_is_less = ((idxs == len(array)) | (np.fabs(values - array[np.maximum(idxs - 1, 0)]) < np.fabs(
             values - array[np.minimum(idxs, len(array) - 1)])))
         idxs[prev_idx_is_less] -= 1
 
         return array[idxs], idxs
 
     @staticmethod
-    def associate_timestamps(t_est, t_gt, offset=0.0, max_difference=0.02):
+    def associate_timestamps(t_est, t_gt, offset=0.0, max_difference=0.02, round_decimals=9, unique_timestamps=True):
         # returns idx_est, idx_gt, t_est_matched, t_gt_matched
         swapped = False
         if len(t_est) > len(t_gt):
             t_vec1 = t_est + offset
             t_vec2 = t_gt
             swapped = True
         else:
             t_vec1 = t_gt
             t_vec2 = t_est + offset
 
-        closest_t_vec1, idx1 = TimestampAssociation.get_closest(t_vec1.transpose().ravel(), t_vec2.transpose().ravel())
-        idx2 = np.arange(0, len(idx1), dtype=np.int32)
-        diff = np.abs(closest_t_vec1 - np.array(t_vec2.ravel()))
-        mask_greater = np.where(diff >= max_difference)[0]
-        idx_1 = np.delete(idx1, mask_greater, axis=0)
-        idx_2 = np.delete(idx2, mask_greater, axis=0)
-        vec_1_matched = t_vec1[idx_1]
-        vec_2_matched = t_vec2[idx_2]
+        # round the timestamp arrays by N-decimals
+        t_vec1 = np.round(t_vec1, decimals=round_decimals)
+        t_vec2 = np.round(t_vec2, decimals=round_decimals)
+
+        closest_t_vec1, idx_1 = TimestampAssociation.get_closest(t_vec1.transpose().ravel(), t_vec2.transpose().ravel())
+        idx_2 = np.arange(0, len(idx_1), dtype=np.int32)
+
+        if max_difference > 0:
+            diff = np.abs(closest_t_vec1 - np.array(t_vec2.ravel()))
+            mask_greater = np.where(diff >= max_difference)[0]
+            idx_1 = np.delete(idx_1, mask_greater, axis=0)
+            idx_2 = np.delete(idx_2, mask_greater, axis=0)
+
+        t_vec_1_matched = t_vec1[idx_1]
+        t_vec_2_matched = t_vec2[idx_2]
+
+        # find uniques in both matched sets of timestamps
+        if unique_timestamps:
+            vec_1_matched_unique, unique_idx_1 = np.unique(t_vec_1_matched, return_index=True)
+            vec_2_matched_unique, unique_idx_2 = np.unique(t_vec_2_matched, return_index=True)
+            common_indices = np.intersect1d(unique_idx_1, unique_idx_2)
+
+            idx_1 = idx_1[common_indices]
+            idx_2 = idx_2[common_indices]
+            t_vec_1_matched = t_vec1[idx_1]
+            t_vec_2_matched = t_vec2[idx_2]
 
         # returns idx_est, idx_gt, t_est_matched, t_gt_matched
-        if not swapped:
-            return idx_2, idx_1, vec_2_matched, vec_1_matched
+        if swapped:
+            return idx_1, idx_2, t_vec_1_matched, t_vec_2_matched
         else:
-            return idx_1, idx_2, vec_1_matched, vec_2_matched
+            return idx_2, idx_1, t_vec_2_matched, t_vec_1_matched
```

### Comparing `cnspy_timestamp_association-0.1.1/cnspy_timestamp_association.egg-info/PKG-INFO` & `cnspy_timestamp_association-0.2.0/cnspy_timestamp_association.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 Metadata-Version: 2.1
-Name: cnspy-timestamp-association
-Version: 0.1.1
+Name: cnspy_timestamp_association
+Version: 0.2.0
 Summary: Associates vectors of timestamps.
 Home-page: https://github.com/aau-cns/cnspy_timestamp_association/
 Author: Roland Jung
 Author-email: roland.jung@aau.at
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/aau-cns/cnspy_timestamp_association/issues
-Description: # cnspy_timestamp_association
-        
-        The class `TimestampAssociation` finds correspondences between to vectors, in our case containing timestamps. The aim is to find timestamp pairs with a configurable  `max_difference`.
-        
-        ## Installation
-        
-        Install the current code base from GitHub and pip install a link to that cloned copy
-        ```
-        git clone https://github.com/aau-cns/cnspy_timestamp_association.git
-        cd cnspy_timestamp_association
-        pip install -e .
-        ```
-        
-        ## Dependencies
-        
-        It is part of the [cnspy eco-system](hhttps://github.com/aau-cns/cnspy_eco_system_test) of the [cns-github](https://github.com/aau-cns) group.  
-        
-        * [numpy]()
-        
-        ## Examples
-        
-        Please refer to the unit-test section in `TimestampAssociation.py`.
-        
-        ## License
-        
-        Software License Agreement (GNU GPLv3  License), refer to the LICENSE file.
-        
-        *Sharing is caring!* - [Roland Jung](https://github.com/jungr-ait)
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENCE
+Requires-Dist: numpy
+
+# cnspy_timestamp_association
+
+The class `TimestampAssociation` finds correspondences between to vectors, in our case containing timestamps. The aim is to find timestamp pairs with a configurable  `max_difference`.
+
+## Installation
+
+Install the current code base from GitHub and pip install a link to that cloned copy
+```
+git clone https://github.com/aau-cns/cnspy_timestamp_association.git
+cd cnspy_timestamp_association
+pip install -e .
+```
+or the [official package](https://pypi.org/project/cnspy-timestamp-association/) via
+```commandline
+pip install cnspy-timestamp-association
+```
+
+## Dependencies
+
+It is part of the [cnspy eco-system](hhttps://github.com/aau-cns/cnspy_eco_system_test) of the [cns-github](https://github.com/aau-cns) group.  
+
+* [numpy]()
+
+## Examples
+
+Please refer to the unit-test section in `TimestampAssociation.py`.
+
+## License
+
+Software License Agreement (GNU GPLv3  License), refer to the LICENSE file.
+
+*Sharing is caring!* - [Roland Jung](https://github.com/jungr-ait)
```

### Comparing `cnspy_timestamp_association-0.1.1/setup.py` & `cnspy_timestamp_association-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `cnspy_timestamp_association-0.1.1/test/test_TimestampAssociation.py` & `cnspy_timestamp_association-0.2.0/test/test_TimestampAssociation.py`

 * *Files identical despite different names*

