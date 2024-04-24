# Comparing `tmp/pygformula-1.0.4.tar.gz` & `tmp/pygformula-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygformula-1.0.4.tar", last modified: Sun Apr 21 19:07:37 2024, max compression
+gzip compressed data, was "pygformula-1.0.5.tar", last modified: Wed Apr 24 19:58:37 2024, max compression
```

## Comparing `pygformula-1.0.4.tar` & `pygformula-1.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 19:07:37.359888 pygformula-1.0.4/
--rw-rw-rw-   0        0        0     1122 2024-04-18 20:33:45.000000 pygformula-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     1453 2024-04-21 19:07:37.358888 pygformula-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1203 2024-04-21 02:57:27.000000 pygformula-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 19:07:37.310880 pygformula-1.0.4/pygformula/
--rw-rw-rw-   0        0        0       53 2024-04-18 18:44:20.000000 pygformula-1.0.4/pygformula/__init__.py
--rw-rw-rw-   0        0        0    14167 2024-04-18 20:33:45.000000 pygformula-1.0.4/pygformula/comparisons.py
--rw-rw-rw-   0        0        0     9610 2024-04-18 20:32:39.000000 pygformula-1.0.4/pygformula/data.py
-drwxrwxrwx   0        0        0        0 2024-04-21 19:07:37.345895 pygformula-1.0.4/pygformula/parametric_gformula/
--rw-rw-rw-   0        0        0       55 2024-02-09 07:11:15.000000 pygformula-1.0.4/pygformula/parametric_gformula/__init__.py
--rw-rw-rw-   0        0        0    17447 2024-04-18 20:33:45.000000 pygformula-1.0.4/pygformula/parametric_gformula/bootstrap.py
--rw-rw-rw-   0        0        0    21378 2024-04-18 20:33:45.000000 pygformula-1.0.4/pygformula/parametric_gformula/fit.py
--rw-rw-rw-   0        0        0     8385 2024-04-18 20:33:45.000000 pygformula-1.0.4/pygformula/parametric_gformula/histories.py
--rw-rw-rw-   0        0        0    12355 2024-04-18 20:33:45.000000 pygformula-1.0.4/pygformula/parametric_gformula/interventions.py
--rw-rw-rw-   0        0        0    44695 2024-04-18 20:33:45.000000 pygformula-1.0.4/pygformula/parametric_gformula/parametric_gformula.py
--rw-rw-rw-   0        0        0    25088 2024-04-18 20:33:45.000000 pygformula-1.0.4/pygformula/parametric_gformula/simulate.py
--rw-rw-rw-   0        0        0    19939 2024-04-18 20:33:45.000000 pygformula-1.0.4/pygformula/plot.py
-drwxrwxrwx   0        0        0        0 2024-04-21 19:07:37.355888 pygformula-1.0.4/pygformula/utils/
--rw-rw-rw-   0        0        0        0 2024-04-18 20:33:45.000000 pygformula-1.0.4/pygformula/utils/__init__.py
--rw-rw-rw-   0        0        0     7677 2024-04-18 20:33:45.000000 pygformula-1.0.4/pygformula/utils/helper.py
--rw-rw-rw-   0        0        0    39548 2024-04-18 20:33:45.000000 pygformula-1.0.4/pygformula/utils/util.py
-drwxrwxrwx   0        0        0        0 2024-04-21 19:07:37.320878 pygformula-1.0.4/pygformula.egg-info/
--rw-rw-rw-   0        0        0     1453 2024-04-21 19:07:37.000000 pygformula-1.0.4/pygformula.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      644 2024-04-21 19:07:37.000000 pygformula-1.0.4/pygformula.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 19:07:37.000000 pygformula-1.0.4/pygformula.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-21 19:07:37.000000 pygformula-1.0.4/pygformula.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 19:07:37.359888 pygformula-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      421 2024-04-21 02:54:57.000000 pygformula-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 19:58:37.417611 pygformula-1.0.5/
+-rw-rw-rw-   0        0        0     1122 2024-04-18 20:33:45.000000 pygformula-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1453 2024-04-24 19:58:37.416611 pygformula-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1203 2024-04-24 19:58:04.000000 pygformula-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 19:58:37.376628 pygformula-1.0.5/pygformula/
+-rw-rw-rw-   0        0        0       53 2024-04-18 18:44:20.000000 pygformula-1.0.5/pygformula/__init__.py
+-rw-rw-rw-   0        0        0    14167 2024-04-18 20:33:45.000000 pygformula-1.0.5/pygformula/comparisons.py
+-rw-rw-rw-   0        0        0     9610 2024-04-18 20:32:39.000000 pygformula-1.0.5/pygformula/data.py
+drwxrwxrwx   0        0        0        0 2024-04-24 19:58:37.405610 pygformula-1.0.5/pygformula/parametric_gformula/
+-rw-rw-rw-   0        0        0       55 2024-02-09 07:11:15.000000 pygformula-1.0.5/pygformula/parametric_gformula/__init__.py
+-rw-rw-rw-   0        0        0    17447 2024-04-18 20:33:45.000000 pygformula-1.0.5/pygformula/parametric_gformula/bootstrap.py
+-rw-rw-rw-   0        0        0    21378 2024-04-18 20:33:45.000000 pygformula-1.0.5/pygformula/parametric_gformula/fit.py
+-rw-rw-rw-   0        0        0     8385 2024-04-18 20:33:45.000000 pygformula-1.0.5/pygformula/parametric_gformula/histories.py
+-rw-rw-rw-   0        0        0    12355 2024-04-18 20:33:45.000000 pygformula-1.0.5/pygformula/parametric_gformula/interventions.py
+-rw-rw-rw-   0        0        0    44695 2024-04-18 20:33:45.000000 pygformula-1.0.5/pygformula/parametric_gformula/parametric_gformula.py
+-rw-rw-rw-   0        0        0    25088 2024-04-18 20:33:45.000000 pygformula-1.0.5/pygformula/parametric_gformula/simulate.py
+-rw-rw-rw-   0        0        0    19939 2024-04-18 20:33:45.000000 pygformula-1.0.5/pygformula/plot.py
+drwxrwxrwx   0        0        0        0 2024-04-24 19:58:37.411610 pygformula-1.0.5/pygformula/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-18 20:33:45.000000 pygformula-1.0.5/pygformula/utils/__init__.py
+-rw-rw-rw-   0        0        0     7677 2024-04-18 20:33:45.000000 pygformula-1.0.5/pygformula/utils/helper.py
+-rw-rw-rw-   0        0        0    39587 2024-04-24 19:56:21.000000 pygformula-1.0.5/pygformula/utils/util.py
+drwxrwxrwx   0        0        0        0 2024-04-24 19:58:37.387610 pygformula-1.0.5/pygformula.egg-info/
+-rw-rw-rw-   0        0        0     1453 2024-04-24 19:58:37.000000 pygformula-1.0.5/pygformula.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      644 2024-04-24 19:58:37.000000 pygformula-1.0.5/pygformula.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 19:58:37.000000 pygformula-1.0.5/pygformula.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-24 19:58:37.000000 pygformula-1.0.5/pygformula.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 19:58:37.417611 pygformula-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      421 2024-04-24 19:58:32.000000 pygformula-1.0.5/setup.py
```

### Comparing `pygformula-1.0.4/LICENSE` & `pygformula-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pygformula-1.0.4/PKG-INFO` & `pygformula-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygformula
-Version: 1.0.4
+Version: 1.0.5
 Summary: A python implementation of the parametric g-formula
 Maintainer: Jing Li
 Maintainer-email: jing_li@hsph.harvard.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pygformula: a python implementation of the parametric g-formula
```

### Comparing `pygformula-1.0.4/README.md` & `pygformula-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pygformula-1.0.4/pygformula/comparisons.py` & `pygformula-1.0.5/pygformula/comparisons.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.0.4/pygformula/data.py` & `pygformula-1.0.5/pygformula/data.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.0.4/pygformula/parametric_gformula/bootstrap.py` & `pygformula-1.0.5/pygformula/parametric_gformula/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.0.4/pygformula/parametric_gformula/fit.py` & `pygformula-1.0.5/pygformula/parametric_gformula/fit.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.0.4/pygformula/parametric_gformula/histories.py` & `pygformula-1.0.5/pygformula/parametric_gformula/histories.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.0.4/pygformula/parametric_gformula/interventions.py` & `pygformula-1.0.5/pygformula/parametric_gformula/interventions.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.0.4/pygformula/parametric_gformula/parametric_gformula.py` & `pygformula-1.0.5/pygformula/parametric_gformula/parametric_gformula.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.0.4/pygformula/parametric_gformula/simulate.py` & `pygformula-1.0.5/pygformula/parametric_gformula/simulate.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.0.4/pygformula/plot.py` & `pygformula-1.0.5/pygformula/plot.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.0.4/pygformula/utils/helper.py` & `pygformula-1.0.5/pygformula/utils/helper.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.0.4/pygformula/utils/util.py` & `pygformula-1.0.5/pygformula/utils/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 def read_intervention_input(interventions, int_descript):
 
     intervention_dicts = {}
     for intervention_key, intervention in interventions.items():
         prefix = intervention_key.split('_', 1)[0]  # Get the prefix (e.g., 'Intervention1', 'Intervention2')
         intervention_id = int(prefix[12:])  # Get id
         intervention_name = int_descript[intervention_id - 1]
-        treatment_name = intervention_key.split('_')[1]  # Get the treatment name
+        index = intervention_key.find('_') # Get the treatment name
+        treatment_name = intervention_key[index+1:]
 
         intervention.insert(0, treatment_name)
         if intervention_name not in intervention_dicts:
             intervention_dicts[intervention_name] = []
         intervention_dicts[intervention_name].append(intervention)
 
     return intervention_dicts
```

### Comparing `pygformula-1.0.4/pygformula.egg-info/PKG-INFO` & `pygformula-1.0.5/pygformula.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygformula
-Version: 1.0.4
+Version: 1.0.5
 Summary: A python implementation of the parametric g-formula
 Maintainer: Jing Li
 Maintainer-email: jing_li@hsph.harvard.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pygformula: a python implementation of the parametric g-formula
```

### Comparing `pygformula-1.0.4/pygformula.egg-info/SOURCES.txt` & `pygformula-1.0.5/pygformula.egg-info/SOURCES.txt`

 * *Files identical despite different names*

