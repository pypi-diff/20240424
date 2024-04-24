# Comparing `tmp/dataidea-0.2.4.tar.gz` & `tmp/dataidea-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataidea-0.2.4.tar", max compression
+gzip compressed data, was "dataidea-0.2.5.tar", max compression
```

## Comparing `dataidea-0.2.4.tar` & `dataidea-0.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     8646 2024-04-21 19:27:31.509014 dataidea-0.2.4/README.md
--rw-r--r--   0        0        0      229 2024-04-19 06:31:05.013813 dataidea-0.2.4/dataidea/datasets/cluster.csv
--rw-r--r--   0        0        0     4645 2024-04-19 06:33:56.213774 dataidea-0.2.4/dataidea/datasets/demo.csv
--rw-r--r--   0        0        0    47391 2024-04-19 06:31:05.017817 dataidea-0.2.4/dataidea/datasets/fpl.csv
--rw-r--r--   0        0        0      370 2024-04-19 06:31:05.021821 dataidea-0.2.4/dataidea/datasets/homeprices.csv
--rw-r--r--   0        0        0  2091239 2024-04-19 06:31:05.025825 dataidea-0.2.4/dataidea/datasets/melbourne.csv
--rw-r--r--   0        0        0      302 2024-04-19 06:31:05.029829 dataidea-0.2.4/dataidea/datasets/music.csv
--rw-r--r--   0        0        0      656 2024-04-19 06:31:05.029829 dataidea-0.2.4/dataidea/datasets/salaries.csv
--rw-r--r--   0        0        0   108285 2024-04-19 06:31:05.029829 dataidea-0.2.4/dataidea/datasets/titanic.csv
--rw-r--r--   0        0        0  1355781 2024-04-19 06:31:05.033833 dataidea-0.2.4/dataidea/datasets/vgsales.csv
--rw-r--r--   0        0        0      217 2024-04-19 06:31:05.033833 dataidea-0.2.4/dataidea/datasets/weather.csv
--rw-r--r--   0        0        0     3767 2024-04-21 10:09:01.374308 dataidea-0.2.4/dataidea/datasets.py
--rw-r--r--   0        0        0      210 2024-04-19 05:07:03.723401 dataidea-0.2.4/dataidea/feature_selection.py
--rw-r--r--   0        0        0     2816 2024-04-21 19:11:14.394771 dataidea-0.2.4/dataidea/models.py
--rw-r--r--   0        0        0      167 2024-04-21 19:28:54.845536 dataidea-0.2.4/dataidea/packages.py
--rw-r--r--   0        0        0      284 2024-04-20 15:08:51.951883 dataidea-0.2.4/dataidea/statistics.py
--rw-r--r--   0        0        0       96 2024-04-20 14:03:53.712195 dataidea-0.2.4/dataidea/tabular.py
--rw-r--r--   0        0        0      481 2024-04-21 19:28:23.018071 dataidea-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     9445 1970-01-01 00:00:00.000000 dataidea-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     7496 2024-04-21 19:53:53.642815 dataidea-0.2.5/README.md
+-rw-r--r--   0        0        0      229 2024-04-19 06:31:05.013813 dataidea-0.2.5/dataidea/datasets/cluster.csv
+-rw-r--r--   0        0        0     4645 2024-04-19 06:33:56.213774 dataidea-0.2.5/dataidea/datasets/demo.csv
+-rw-r--r--   0        0        0    47391 2024-04-19 06:31:05.017817 dataidea-0.2.5/dataidea/datasets/fpl.csv
+-rw-r--r--   0        0        0      370 2024-04-19 06:31:05.021821 dataidea-0.2.5/dataidea/datasets/homeprices.csv
+-rw-r--r--   0        0        0  2091239 2024-04-19 06:31:05.025825 dataidea-0.2.5/dataidea/datasets/melbourne.csv
+-rw-r--r--   0        0        0      302 2024-04-19 06:31:05.029829 dataidea-0.2.5/dataidea/datasets/music.csv
+-rw-r--r--   0        0        0      656 2024-04-19 06:31:05.029829 dataidea-0.2.5/dataidea/datasets/salaries.csv
+-rw-r--r--   0        0        0   108285 2024-04-19 06:31:05.029829 dataidea-0.2.5/dataidea/datasets/titanic.csv
+-rw-r--r--   0        0        0  1355781 2024-04-19 06:31:05.033833 dataidea-0.2.5/dataidea/datasets/vgsales.csv
+-rw-r--r--   0        0        0      217 2024-04-19 06:31:05.033833 dataidea-0.2.5/dataidea/datasets/weather.csv
+-rw-r--r--   0        0        0     3767 2024-04-21 10:09:01.374308 dataidea-0.2.5/dataidea/datasets.py
+-rw-r--r--   0        0        0      210 2024-04-19 05:07:03.723401 dataidea-0.2.5/dataidea/feature_selection.py
+-rw-r--r--   0        0        0     2816 2024-04-21 19:11:14.394771 dataidea-0.2.5/dataidea/models.py
+-rw-r--r--   0        0        0      167 2024-04-21 19:28:54.845536 dataidea-0.2.5/dataidea/packages.py
+-rw-r--r--   0        0        0      284 2024-04-20 15:08:51.951883 dataidea-0.2.5/dataidea/statistics.py
+-rw-r--r--   0        0        0      129 2024-04-23 19:34:49.942481 dataidea-0.2.5/dataidea/tabular.py
+-rw-r--r--   0        0        0      481 2024-04-23 19:35:34.466480 dataidea-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     8295 1970-01-01 00:00:00.000000 dataidea-0.2.5/PKG-INFO
```

### Comparing `dataidea-0.2.4/README.md` & `dataidea-0.2.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: dataidea
+Version: 0.2.5
+Summary: Package to ease data analysis for DATAIDEA students
+License: MIT
+Author: jumashafara
+Author-email: jumashafara0@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: matplotlib (>=3.8.4,<4.0.0)
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: pandas (>=2.2.2,<3.0.0)
+Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
+Requires-Dist: scipy (>=1.13.0,<2.0.0)
+Requires-Dist: seaborn (>=0.13.2,<0.14.0)
+Requires-Dist: statsmodels (>=0.14.2,<0.15.0)
+Description-Content-Type: text/markdown
+
 ## What is the `dataidea` package?
 
 This is a package we are currently developing to help new and old data analysists (especially DATAIDEA students) walk around some repetitive and sometimes disturbing tasks that a data analyst does day to day
 
 This library currently extends and depends on majorly numpy, pandas as sklearn and these, among a few others will be installed once you install dataidea
 
 ## Installing `dataidea`
@@ -27,15 +49,15 @@
 ```python
 from dataidea.tabular import *
 ```
 
 `dataidea`'s applications all use the same basic steps and code:
 
 - Create appropriate DataLoaders
-- Create a Learner
+- Create a Trainer
 - Call a fit method
 - Make predictions or view results.
 
 In this quick start, we’ll show these steps for classification and regression. As you’ll see, the code in each case is extremely similar, despite the very different models and data being used.
 
 ## Loading datasets
 
@@ -50,28 +72,14 @@
 We can see some values inside by using our usual `pandas` dataframe methods like `sample()`, `head()`, `tail()` etc
 
 ```python
 music_data.sample(n=5)
 ```
 
 <div>
-<style scoped>
-    .dataframe tbody tr th:only-of-type {
-        vertical-align: middle;
-    }
-
-    .dataframe tbody tr th {
-        vertical-align: top;
-    }
-
-    .dataframe thead th {
-        text-align: right;
-    }
-
-</style>
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th></th>
       <th>age</th>
       <th>gender</th>
       <th>genre</th>
@@ -129,28 +137,14 @@
 ```
 
 ```python
 transformed_data[0].head()
 ```
 
 <div>
-<style scoped>
-    .dataframe tbody tr th:only-of-type {
-        vertical-align: middle;
-    }
-
-    .dataframe tbody tr th {
-        vertical-align: top;
-    }
-
-    .dataframe thead th {
-        text-align: right;
-    }
-
-</style>
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th></th>
       <th>num__  age</th>
       <th>cat__gender_0</th>
       <th>cat__gender_1</th>
@@ -216,28 +210,14 @@
 ```
 
 ```python
 classification_report
 ```
 
 <div>
-<style scoped>
-    .dataframe tbody tr th:only-of-type {
-        vertical-align: middle;
-    }
-
-    .dataframe tbody tr th {
-        vertical-align: top;
-    }
-
-    .dataframe thead th {
-        text-align: right;
-    }
-
-</style>
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th></th>
       <th>precision</th>
       <th>recall</th>
       <th>f1-score</th>
@@ -312,28 +292,14 @@
         'gender': [1, 0]
     })
 
 data_to_predict
 ```
 
 <div>
-<style scoped>
-    .dataframe tbody tr th:only-of-type {
-        vertical-align: middle;
-    }
-
-    .dataframe tbody tr th {
-        vertical-align: top;
-    }
-
-    .dataframe thead th {
-        text-align: right;
-    }
-
-</style>
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th></th>
       <th>age</th>
       <th>gender</th>
     </tr>
@@ -362,28 +328,14 @@
 ```
 
 ```python
 data_to_predict
 ```
 
 <div>
-<style scoped>
-    .dataframe tbody tr th:only-of-type {
-        vertical-align: middle;
-    }
-
-    .dataframe tbody tr th {
-        vertical-align: top;
-    }
-
-    .dataframe thead th {
-        text-align: right;
-    }
-
-</style>
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th></th>
       <th>age</th>
       <th>gender</th>
       <th>predicted</th>
@@ -405,7 +357,8 @@
   </tbody>
 </table>
 </div>
 
 ```python
 
 ```
+
```

### Comparing `dataidea-0.2.4/dataidea/datasets/demo.csv` & `dataidea-0.2.5/dataidea/datasets/demo.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.2.4/dataidea/datasets/fpl.csv` & `dataidea-0.2.5/dataidea/datasets/fpl.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.2.4/dataidea/datasets/melbourne.csv` & `dataidea-0.2.5/dataidea/datasets/melbourne.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.2.4/dataidea/datasets/salaries.csv` & `dataidea-0.2.5/dataidea/datasets/salaries.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.2.4/dataidea/datasets/titanic.csv` & `dataidea-0.2.5/dataidea/datasets/titanic.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.2.4/dataidea/datasets/vgsales.csv` & `dataidea-0.2.5/dataidea/datasets/vgsales.csv`

 * *Files identical despite different names*

### Comparing `dataidea-0.2.4/dataidea/datasets.py` & `dataidea-0.2.5/dataidea/datasets.py`

 * *Files identical despite different names*

### Comparing `dataidea-0.2.4/dataidea/models.py` & `dataidea-0.2.5/dataidea/models.py`

 * *Files identical despite different names*

