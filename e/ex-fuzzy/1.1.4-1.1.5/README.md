# Comparing `tmp/ex_fuzzy-1.1.4.tar.gz` & `tmp/ex_fuzzy-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ex_fuzzy-1.1.4.tar", last modified: Wed Apr 24 13:51:01 2024, max compression
+gzip compressed data, was "ex_fuzzy-1.1.5.tar", last modified: Wed Apr 24 14:44:20 2024, max compression
```

## Comparing `ex_fuzzy-1.1.4.tar` & `ex_fuzzy-1.1.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 13:51:01.501254 ex_fuzzy-1.1.4/
--rw-rw-rw-   0        0        0    35184 2024-04-10 13:18:52.000000 ex_fuzzy-1.1.4/LICENSE
--rw-rw-rw-   0        0        0     4333 2024-04-24 13:51:01.494273 ex_fuzzy-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     3284 2024-04-22 14:14:00.000000 ex_fuzzy-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 13:51:01.369252 ex_fuzzy-1.1.4/ex_fuzzy/
-drwxrwxrwx   0        0        0        0 2024-04-24 13:51:01.469252 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/
--rw-rw-rw-   0        0        0      282 2024-04-05 15:43:34.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/__init__.py
--rw-rw-rw-   0        0        0     6197 2024-01-31 12:48:36.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/centroid.py
--rw-rw-rw-   0        0        0    11027 2024-04-11 15:17:33.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/classifiers.py
--rw-rw-rw-   0        0        0     7433 2024-01-30 16:48:50.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/cognitive_maps.py
--rw-rw-rw-   0        0        0    15878 2024-04-18 15:39:28.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/eval_rules.py
--rw-rw-rw-   0        0        0     2693 2024-04-24 13:08:01.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/eval_tools.py
--rw-rw-rw-   0        0        0    43114 2024-04-24 13:36:10.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/evolutionary_fit.py
--rw-rw-rw-   0        0        0    17306 2024-04-05 15:07:12.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/fuzzy_sets.py
--rw-rw-rw-   0        0        0     6160 2024-04-03 14:16:49.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/maintenance.py
--rw-rw-rw-   0        0        0     3677 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/persistence.py
--rw-rw-rw-   0        0        0    11420 2024-04-05 16:05:24.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/rule_mining.py
--rw-rw-rw-   0        0        0    41199 2024-04-23 15:06:45.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/rules.py
--rw-rw-rw-   0        0        0    27001 2024-01-31 15:05:05.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/temporal.py
--rw-rw-rw-   0        0        0    25751 2024-04-05 15:33:36.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/utils.py
--rw-rw-rw-   0        0        0    16166 2024-04-24 13:41:44.000000 ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/vis_rules.py
-drwxrwxrwx   0        0        0        0 2024-04-24 13:51:01.400254 ex_fuzzy-1.1.4/ex_fuzzy.egg-info/
--rw-rw-rw-   0        0        0     4333 2024-04-24 13:51:01.000000 ex_fuzzy-1.1.4/ex_fuzzy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      785 2024-04-24 13:51:01.000000 ex_fuzzy-1.1.4/ex_fuzzy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 13:51:01.000000 ex_fuzzy-1.1.4/ex_fuzzy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-04-24 13:51:01.000000 ex_fuzzy-1.1.4/ex_fuzzy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-24 13:51:01.000000 ex_fuzzy-1.1.4/ex_fuzzy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 13:51:01.502251 ex_fuzzy-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1773 2024-04-24 13:50:10.000000 ex_fuzzy-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-24 13:51:01.491252 ex_fuzzy-1.1.4/tests/
--rw-rw-rw-   0        0        0     1261 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.4/tests/test_centroids.py
--rw-rw-rw-   0        0        0     1963 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.4/tests/test_classification.py
--rw-rw-rw-   0        0        0      797 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.4/tests/test_eval_tools.py
--rw-rw-rw-   0        0        0     1821 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.4/tests/test_fuzzy_sets.py
--rw-rw-rw-   0        0        0     4189 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.4/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:44:20.570669 ex_fuzzy-1.1.5/
+-rw-rw-rw-   0        0        0    35184 2024-04-10 13:18:52.000000 ex_fuzzy-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0     4333 2024-04-24 14:44:20.563668 ex_fuzzy-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3284 2024-04-22 14:14:00.000000 ex_fuzzy-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 14:44:20.446658 ex_fuzzy-1.1.5/ex_fuzzy/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:44:20.536666 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/
+-rw-rw-rw-   0        0        0      282 2024-04-05 15:43:34.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/__init__.py
+-rw-rw-rw-   0        0        0     6197 2024-01-31 12:48:36.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/centroid.py
+-rw-rw-rw-   0        0        0    11027 2024-04-11 15:17:33.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/classifiers.py
+-rw-rw-rw-   0        0        0     7433 2024-01-30 16:48:50.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/cognitive_maps.py
+-rw-rw-rw-   0        0        0    15878 2024-04-18 15:39:28.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/eval_rules.py
+-rw-rw-rw-   0        0        0     2693 2024-04-24 13:08:01.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/eval_tools.py
+-rw-rw-rw-   0        0        0    43114 2024-04-24 13:36:10.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/evolutionary_fit.py
+-rw-rw-rw-   0        0        0    17306 2024-04-05 15:07:12.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/fuzzy_sets.py
+-rw-rw-rw-   0        0        0     6160 2024-04-03 14:16:49.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/maintenance.py
+-rw-rw-rw-   0        0        0     3677 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/persistence.py
+-rw-rw-rw-   0        0        0    11420 2024-04-05 16:05:24.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/rule_mining.py
+-rw-rw-rw-   0        0        0    41199 2024-04-23 15:06:45.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/rules.py
+-rw-rw-rw-   0        0        0    27001 2024-01-31 15:05:05.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/temporal.py
+-rw-rw-rw-   0        0        0    25751 2024-04-05 15:33:36.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/utils.py
+-rw-rw-rw-   0        0        0    16171 2024-04-24 14:42:34.000000 ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/vis_rules.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:44:20.478662 ex_fuzzy-1.1.5/ex_fuzzy.egg-info/
+-rw-rw-rw-   0        0        0     4333 2024-04-24 14:44:20.000000 ex_fuzzy-1.1.5/ex_fuzzy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      785 2024-04-24 14:44:20.000000 ex_fuzzy-1.1.5/ex_fuzzy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 14:44:20.000000 ex_fuzzy-1.1.5/ex_fuzzy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-04-24 14:44:20.000000 ex_fuzzy-1.1.5/ex_fuzzy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-24 14:44:20.000000 ex_fuzzy-1.1.5/ex_fuzzy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 14:44:20.572668 ex_fuzzy-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1773 2024-04-24 14:44:15.000000 ex_fuzzy-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:44:20.555672 ex_fuzzy-1.1.5/tests/
+-rw-rw-rw-   0        0        0     1261 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.5/tests/test_centroids.py
+-rw-rw-rw-   0        0        0     1963 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.5/tests/test_classification.py
+-rw-rw-rw-   0        0        0      797 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.5/tests/test_eval_tools.py
+-rw-rw-rw-   0        0        0     1821 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.5/tests/test_fuzzy_sets.py
+-rw-rw-rw-   0        0        0     4189 2024-01-30 16:48:51.000000 ex_fuzzy-1.1.5/tests/test_utils.py
```

### Comparing `ex_fuzzy-1.1.4/LICENSE` & `ex_fuzzy-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.4/PKG-INFO` & `ex_fuzzy-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ex_fuzzy
-Version: 1.1.4
+Version: 1.1.5
 Summary: Library to perform explainable AI using fuzzy logic.
 Home-page: https://github.com/Fuminides/ex-fuzzy
 Download-URL: https://pypi.org/project/ex-fuzzy/
 Maintainer: Javier Fumanal Idocin
 Maintainer-email: javierfumanalidocin@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ex_fuzzy-1.1.4/README.md` & `ex_fuzzy-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/centroid.py` & `ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/centroid.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/classifiers.py` & `ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/classifiers.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/cognitive_maps.py` & `ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/cognitive_maps.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/eval_rules.py` & `ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/eval_rules.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/eval_tools.py` & `ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/eval_tools.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/evolutionary_fit.py` & `ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/evolutionary_fit.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/fuzzy_sets.py` & `ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/fuzzy_sets.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/maintenance.py` & `ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/maintenance.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/persistence.py` & `ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/persistence.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/rule_mining.py` & `ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/rule_mining.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/rules.py` & `ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/rules.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/temporal.py` & `ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/temporal.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/utils.py` & `ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/utils.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.4/ex_fuzzy/ex_fuzzy/vis_rules.py` & `ex_fuzzy-1.1.5/ex_fuzzy/ex_fuzzy/vis_rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     :return: List of list of pandas dataframes with the connections in adjacency matrix format.
     '''
     res = []
     for ix, rule_base in enumerate(mrule_base.rule_bases):
         try:
             res.append(connect_rulebase(rule_base))
         except:
-            print('Error in the visualization of the rule base: "' + mrule_base.get_consequents_names()[ix] + '", probably because there are no rules in the rule base.')
+            print('Error in the visualization of the rule base: "' + str(mrule_base.get_consequents_names()[ix]) + '", probably because there are no rules in the rule base.')
 
     return res
 
 
 def visualize_rulebase(mrule_base: rules.MasterRuleBase, export_path: str=None) -> None:
     '''
     Visualize a rule base using low, medium and high partitions with 1 rule in common -> 1 edge connections.
```

### Comparing `ex_fuzzy-1.1.4/ex_fuzzy.egg-info/PKG-INFO` & `ex_fuzzy-1.1.5/ex_fuzzy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ex-fuzzy
-Version: 1.1.4
+Version: 1.1.5
 Summary: Library to perform explainable AI using fuzzy logic.
 Home-page: https://github.com/Fuminides/ex-fuzzy
 Download-URL: https://pypi.org/project/ex-fuzzy/
 Maintainer: Javier Fumanal Idocin
 Maintainer-email: javierfumanalidocin@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ex_fuzzy-1.1.4/ex_fuzzy.egg-info/SOURCES.txt` & `ex_fuzzy-1.1.5/ex_fuzzy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.4/setup.py` & `ex_fuzzy-1.1.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 DISTNAME = "ex_fuzzy"
 DESCRIPTION = "Library to perform explainable AI using fuzzy logic."
 MAINTAINER = "Javier Fumanal Idocin"
 MAINTAINER_EMAIL = "javierfumanalidocin@gmail.com"
 URL = "https://github.com/Fuminides/ex-fuzzy"
 LICENSE = "GPL-3.0"
 DOWNLOAD_URL = "https://pypi.org/project/ex-fuzzy/"
-VERSION = "1.1.4"
+VERSION = "1.1.5"
 INSTALL_REQUIRES = ["numpy", "networkx", "matplotlib", "pymoo", "pandas", "scikit-learn"]
 CLASSIFIERS = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.7",
```

### Comparing `ex_fuzzy-1.1.4/tests/test_centroids.py` & `ex_fuzzy-1.1.5/tests/test_centroids.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.4/tests/test_classification.py` & `ex_fuzzy-1.1.5/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.4/tests/test_eval_tools.py` & `ex_fuzzy-1.1.5/tests/test_eval_tools.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.4/tests/test_fuzzy_sets.py` & `ex_fuzzy-1.1.5/tests/test_fuzzy_sets.py`

 * *Files identical despite different names*

### Comparing `ex_fuzzy-1.1.4/tests/test_utils.py` & `ex_fuzzy-1.1.5/tests/test_utils.py`

 * *Files identical despite different names*

