# Comparing `tmp/multidst-0.0.3.tar.gz` & `tmp/multidst-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidst-0.0.3.tar", last modified: Wed Apr 17 18:42:00 2024, max compression
+gzip compressed data, was "multidst-0.1.2.tar", last modified: Wed Apr 24 08:20:39 2024, max compression
```

## Comparing `multidst-0.0.3.tar` & `multidst-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 18:42:00.605052 multidst-0.0.3/
--rw-rw-rw-   0        0        0      698 2024-04-17 18:42:00.604064 multidst-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      388 2024-04-05 18:29:30.000000 multidst-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 18:42:00.544254 multidst-0.0.3/multidst/
--rw-rw-rw-   0        0        0       80 2024-04-07 20:03:31.000000 multidst-0.0.3/multidst/__init__.py
--rw-rw-rw-   0        0        0     3121 2024-04-17 18:02:26.000000 multidst-0.0.3/multidst/functions.py
-drwxrwxrwx   0        0        0        0 2024-04-17 18:42:00.590056 multidst-0.0.3/multidst/methods/
--rw-rw-rw-   0        0        0      560 2024-04-05 18:55:56.000000 multidst-0.0.3/multidst/methods/BH.py
--rw-rw-rw-   0        0        0      553 2024-04-05 18:26:19.000000 multidst-0.0.3/multidst/methods/BY.py
--rw-rw-rw-   0        0        0      175 2024-04-07 09:51:41.000000 multidst-0.0.3/multidst/methods/__init__.py
--rw-rw-rw-   0        0        0      616 2024-04-05 18:55:56.000000 multidst-0.0.3/multidst/methods/bonf.py
--rw-rw-rw-   0        0        0      980 2024-04-05 18:26:26.000000 multidst-0.0.3/multidst/methods/holm_bonf.py
--rw-rw-rw-   0        0        0     3122 2024-04-11 12:09:21.000000 multidst-0.0.3/multidst/methods/qval.py
--rw-rw-rw-   0        0        0     1339 2024-04-05 18:27:20.000000 multidst-0.0.3/multidst/methods/sgof.py
-drwxrwxrwx   0        0        0        0 2024-04-17 18:42:00.600029 multidst-0.0.3/multidst/utils/
--rw-rw-rw-   0        0        0       97 2024-04-07 16:43:17.000000 multidst-0.0.3/multidst/utils/__init__.py
--rw-rw-rw-   0        0        0     3472 2024-04-17 18:04:08.000000 multidst-0.0.3/multidst/utils/common_indices.py
--rw-rw-rw-   0        0        0    13712 2024-04-17 18:04:24.000000 multidst-0.0.3/multidst/utils/visualization.py
--rw-rw-rw-   0        0        0     7548 2024-04-17 18:07:25.000000 multidst-0.0.3/multidst/utils/weighting.py
-drwxrwxrwx   0        0        0        0 2024-04-17 18:42:00.601031 multidst-0.0.3/multidst.egg-info/
--rw-rw-rw-   0        0        0      698 2024-04-17 18:42:00.000000 multidst-0.0.3/multidst.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2024-04-17 18:42:00.000000 multidst-0.0.3/multidst.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 18:42:00.000000 multidst-0.0.3/multidst.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-04-17 18:42:00.000000 multidst-0.0.3/multidst.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-17 18:42:00.000000 multidst-0.0.3/multidst.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 18:42:00.606016 multidst-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      567 2024-04-17 18:41:45.000000 multidst-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 08:20:39.641897 multidst-0.1.2/
+-rw-rw-rw-   0        0        0      698 2024-04-24 08:20:39.641897 multidst-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2024-04-05 18:29:30.000000 multidst-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 08:20:39.568023 multidst-0.1.2/multidst/
+-rw-rw-rw-   0        0        0       80 2024-04-24 08:18:39.000000 multidst-0.1.2/multidst/__init__.py
+-rw-rw-rw-   0        0        0     3107 2024-04-24 08:17:26.000000 multidst-0.1.2/multidst/functions.py
+drwxrwxrwx   0        0        0        0 2024-04-24 08:20:39.625234 multidst-0.1.2/multidst/methods/
+-rw-rw-rw-   0        0        0      560 2024-04-05 18:55:56.000000 multidst-0.1.2/multidst/methods/BH.py
+-rw-rw-rw-   0        0        0      553 2024-04-05 18:26:19.000000 multidst-0.1.2/multidst/methods/BY.py
+-rw-rw-rw-   0        0        0      175 2024-04-07 09:51:41.000000 multidst-0.1.2/multidst/methods/__init__.py
+-rw-rw-rw-   0        0        0      616 2024-04-05 18:55:56.000000 multidst-0.1.2/multidst/methods/bonf.py
+-rw-rw-rw-   0        0        0      980 2024-04-05 18:26:26.000000 multidst-0.1.2/multidst/methods/holm_bonf.py
+-rw-rw-rw-   0        0        0     3122 2024-04-24 08:17:01.000000 multidst-0.1.2/multidst/methods/qval.py
+-rw-rw-rw-   0        0        0     1339 2024-04-05 18:27:20.000000 multidst-0.1.2/multidst/methods/sgof.py
+drwxrwxrwx   0        0        0        0 2024-04-24 08:20:39.636309 multidst-0.1.2/multidst/utils/
+-rw-rw-rw-   0        0        0       97 2024-04-07 16:43:17.000000 multidst-0.1.2/multidst/utils/__init__.py
+-rw-rw-rw-   0        0        0     3472 2024-04-17 18:04:08.000000 multidst-0.1.2/multidst/utils/common_indices.py
+-rw-rw-rw-   0        0        0    13712 2024-04-24 08:18:20.000000 multidst-0.1.2/multidst/utils/visualization.py
+-rw-rw-rw-   0        0        0     7548 2024-04-17 18:07:25.000000 multidst-0.1.2/multidst/utils/weighting.py
+drwxrwxrwx   0        0        0        0 2024-04-24 08:20:39.638815 multidst-0.1.2/multidst.egg-info/
+-rw-rw-rw-   0        0        0      698 2024-04-24 08:20:39.000000 multidst-0.1.2/multidst.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2024-04-24 08:20:39.000000 multidst-0.1.2/multidst.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 08:20:39.000000 multidst-0.1.2/multidst.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-04-24 08:20:39.000000 multidst-0.1.2/multidst.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-24 08:20:39.000000 multidst-0.1.2/multidst.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 08:20:39.641897 multidst-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      567 2024-04-24 08:20:17.000000 multidst-0.1.2/setup.py
```

### Comparing `multidst-0.0.3/PKG-INFO` & `multidst-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidst
-Version: 0.0.3
+Version: 0.1.2
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: statsmodels
 Requires-Dist: matplotlib
```

### Comparing `multidst-0.0.3/multidst/functions.py` & `multidst-0.1.2/multidst/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     # 5 - BY
     by_results = BY_method(p_values, alpha=alpha)
     by_p, sig_by_p = by_results[0], by_results[1]
     # by_count = len(sig_by_p)
 
     # 6 - Qval
-    q_results = q_value(p_values, alpha=0.05)
+    q_results = q_value(p_values, alpha=alpha)
     q, sig_q,pi0_est = q_results[0], q_results[1],q_results[2]
     # q_count = len(sig_q)
 
     if sigplot == True:
         methods = ['Bonferroni', 'Holm', 'SGoF', 'BH', 'BY', 'Q value']
         sig_indices = [sig_bonf_p, sig_holm_p, sig_sgof_p, sig_bh_p, sig_by_p, sig_q]
         sigindex_plot(methods, sig_indices, title="Significant Index Plot")
@@ -82,14 +82,13 @@
         }
       
       sig_df = pd.DataFrame(sig_len_dict, index=[0])
       print("\n",sig_df, "\n")
 
     return sig_dict
 
-import random
 
 # p_values = [random.uniform(0,1) for i in range(1000)]
 # multitest(p_values, alpha=0.05, sigplot=True, results = True)
 # multitest(p_values, alpha=0.05, sigplot=False, results=True)
```

### Comparing `multidst-0.0.3/multidst/methods/BH.py` & `multidst-0.1.2/multidst/methods/BH.py`

 * *Files identical despite different names*

### Comparing `multidst-0.0.3/multidst/methods/BY.py` & `multidst-0.1.2/multidst/methods/BY.py`

 * *Files identical despite different names*

### Comparing `multidst-0.0.3/multidst/methods/bonf.py` & `multidst-0.1.2/multidst/methods/bonf.py`

 * *Files identical despite different names*

### Comparing `multidst-0.0.3/multidst/methods/holm_bonf.py` & `multidst-0.1.2/multidst/methods/holm_bonf.py`

 * *Files identical despite different names*

### Comparing `multidst-0.0.3/multidst/methods/qval.py` & `multidst-0.1.2/multidst/methods/qval.py`

 * *Files identical despite different names*

### Comparing `multidst-0.0.3/multidst/methods/sgof.py` & `multidst-0.1.2/multidst/methods/sgof.py`

 * *Files identical despite different names*

### Comparing `multidst-0.0.3/multidst/utils/common_indices.py` & `multidst-0.1.2/multidst/utils/common_indices.py`

 * *Files identical despite different names*

### Comparing `multidst-0.0.3/multidst/utils/visualization.py` & `multidst-0.1.2/multidst/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `multidst-0.0.3/multidst/utils/weighting.py` & `multidst-0.1.2/multidst/utils/weighting.py`

 * *Files identical despite different names*

### Comparing `multidst-0.0.3/multidst.egg-info/PKG-INFO` & `multidst-0.1.2/multidst.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidst
-Version: 0.0.3
+Version: 0.1.2
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: statsmodels
 Requires-Dist: matplotlib
```

### Comparing `multidst-0.0.3/multidst.egg-info/SOURCES.txt` & `multidst-0.1.2/multidst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multidst-0.0.3/setup.py` & `multidst-0.1.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name='multidst',
-    version='0.0.3',
+    version='0.1.2',
     packages=find_packages(),  # Automatically find all packages and subpackages
     install_requires=[
         'numpy', 
         'pandas',
         'scipy',
         'statsmodels',
         'matplotlib'
```

