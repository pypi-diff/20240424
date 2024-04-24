# Comparing `tmp/hrcl_jobs-1.6.0.tar.gz` & `tmp/hrcl_jobs-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hrcl_jobs-1.6.0.tar", last modified: Wed Feb 21 17:49:57 2024, max compression
+gzip compressed data, was "/Users/austinwallace/gits/hierarchical_python_jobs/dist/.tmp-rafaxy6q/hrcl_jobs-1.7.0.tar", last modified: Wed Apr 24 19:00:06 2024, max compression
```

## Comparing `hrcl_jobs-1.6.0.tar` & `hrcl_jobs-1.7.0.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 relativity64  (1000) relativity64  (1000)        0 2024-02-21 17:49:57.668854 hrcl_jobs-1.6.0/
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)     1074 2024-02-21 17:31:53.000000 hrcl_jobs-1.6.0/LICENSE
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)     1344 2024-02-21 17:49:57.668854 hrcl_jobs-1.6.0/PKG-INFO
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)      354 2024-02-21 17:31:53.000000 hrcl_jobs-1.6.0/README.md
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)      925 2024-02-21 17:49:43.000000 hrcl_jobs-1.6.0/pyproject.toml
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)      268 2024-02-21 17:49:57.668854 hrcl_jobs-1.6.0/setup.cfg
-drwxr-xr-x   0 relativity64  (1000) relativity64  (1000)        0 2024-02-21 17:49:57.658854 hrcl_jobs-1.6.0/src/
-drwxr-xr-x   0 relativity64  (1000) relativity64  (1000)        0 2024-02-21 17:49:57.668854 hrcl_jobs-1.6.0/src/hrcl_jobs/
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)      618 2024-02-21 17:34:47.000000 hrcl_jobs-1.6.0/src/hrcl_jobs/__init__.py
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)    14403 2024-02-21 17:31:53.000000 hrcl_jobs-1.6.0/src/hrcl_jobs/data.py
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)    11265 2024-02-21 17:31:53.000000 hrcl_jobs-1.6.0/src/hrcl_jobs/dataset.py
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)      968 2024-02-21 17:31:53.000000 hrcl_jobs-1.6.0/src/hrcl_jobs/examples.py
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)      893 2024-02-21 17:31:53.000000 hrcl_jobs-1.6.0/src/hrcl_jobs/jobspec.py
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)    16849 2024-02-21 17:31:53.000000 hrcl_jobs-1.6.0/src/hrcl_jobs/parallel.py
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)     9817 2024-02-21 17:31:53.000000 hrcl_jobs-1.6.0/src/hrcl_jobs/pgsql.py
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)    20138 2024-02-21 17:31:53.000000 hrcl_jobs-1.6.0/src/hrcl_jobs/s22.py
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)     7318 2024-02-21 17:31:53.000000 hrcl_jobs-1.6.0/src/hrcl_jobs/serial.py
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)     9059 2024-02-21 17:31:53.000000 hrcl_jobs-1.6.0/src/hrcl_jobs/setup.py
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)    30828 2024-02-21 17:31:53.000000 hrcl_jobs-1.6.0/src/hrcl_jobs/sqlt.py
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)     2929 2024-02-21 17:31:53.000000 hrcl_jobs-1.6.0/src/hrcl_jobs/tools_og.py
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)     2548 2024-02-21 17:31:53.000000 hrcl_jobs-1.6.0/src/hrcl_jobs/utils.py
-drwxr-xr-x   0 relativity64  (1000) relativity64  (1000)        0 2024-02-21 17:49:57.668854 hrcl_jobs-1.6.0/src/hrcl_jobs.egg-info/
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)     1344 2024-02-21 17:49:57.000000 hrcl_jobs-1.6.0/src/hrcl_jobs.egg-info/PKG-INFO
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)     1131 2024-02-21 17:49:57.000000 hrcl_jobs-1.6.0/src/hrcl_jobs.egg-info/SOURCES.txt
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)        1 2024-02-21 17:49:57.000000 hrcl_jobs-1.6.0/src/hrcl_jobs.egg-info/dependency_links.txt
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)      151 2024-02-21 17:49:57.000000 hrcl_jobs-1.6.0/src/hrcl_jobs.egg-info/requires.txt
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)       78 2024-02-21 17:49:57.000000 hrcl_jobs-1.6.0/src/hrcl_jobs.egg-info/top_level.txt
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)        1 2024-02-21 17:49:57.000000 hrcl_jobs-1.6.0/src/hrcl_jobs.egg-info/zip-safe
-drwxr-xr-x   0 relativity64  (1000) relativity64  (1000)        0 2024-02-21 17:49:57.668854 hrcl_jobs-1.6.0/src/hrcl_jobs_docking/
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)      110 2024-02-21 17:31:53.000000 hrcl_jobs-1.6.0/src/hrcl_jobs_docking/__init__.py
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)     8806 2024-02-21 17:34:47.000000 hrcl_jobs-1.6.0/src/hrcl_jobs_docking/datasets.py
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)    17663 2024-02-21 17:34:47.000000 hrcl_jobs-1.6.0/src/hrcl_jobs_docking/docking_inps.py
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)     1291 2024-02-21 17:34:47.000000 hrcl_jobs-1.6.0/src/hrcl_jobs_docking/jobspec.py
-drwxr-xr-x   0 relativity64  (1000) relativity64  (1000)        0 2024-02-21 17:49:57.668854 hrcl_jobs-1.6.0/src/hrcl_jobs_orca/
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)       24 2024-02-21 17:31:53.000000 hrcl_jobs-1.6.0/src/hrcl_jobs_orca/__init__.py
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)      628 2024-02-21 17:31:53.000000 hrcl_jobs-1.6.0/src/hrcl_jobs_orca/jobspec.py
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)     8196 2024-02-21 17:31:53.000000 hrcl_jobs-1.6.0/src/hrcl_jobs_orca/orca_inps.py
-drwxr-xr-x   0 relativity64  (1000) relativity64  (1000)        0 2024-02-21 17:49:57.668854 hrcl_jobs-1.6.0/src/hrcl_jobs_psi4/
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)     1554 2024-02-21 17:31:53.000000 hrcl_jobs-1.6.0/src/hrcl_jobs_psi4/__init__.py
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)      703 2024-02-21 17:31:53.000000 hrcl_jobs-1.6.0/src/hrcl_jobs_psi4/basis_sets.py
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)        0 2024-02-21 17:31:53.000000 hrcl_jobs-1.6.0/src/hrcl_jobs_psi4/datasets.py
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)     3423 2024-02-21 17:31:53.000000 hrcl_jobs-1.6.0/src/hrcl_jobs_psi4/jobspec.py
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)      615 2024-02-21 17:31:53.000000 hrcl_jobs-1.6.0/src/hrcl_jobs_psi4/methods.py
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)    47792 2024-02-21 17:31:53.000000 hrcl_jobs-1.6.0/src/hrcl_jobs_psi4/psi4_inps.py
-drwxr-xr-x   0 relativity64  (1000) relativity64  (1000)        0 2024-02-21 17:49:57.668854 hrcl_jobs-1.6.0/src/hrcl_jobs_qcfractal/
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)       45 2024-02-21 17:31:53.000000 hrcl_jobs-1.6.0/src/hrcl_jobs_qcfractal/__init__.py
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)     1805 2024-02-21 17:31:53.000000 hrcl_jobs-1.6.0/src/hrcl_jobs_qcfractal/jobspec.py
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)    13655 2024-02-21 17:31:53.000000 hrcl_jobs-1.6.0/src/hrcl_jobs_qcfractal/psi4_inps.py
--rw-r--r--   0 relativity64  (1000) relativity64  (1000)       27 2024-02-21 17:31:53.000000 hrcl_jobs-1.6.0/src/hrcl_jobs_qcfractal/serial.py
+drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2024-04-24 19:00:06.025739 hrcl_jobs-1.7.0/
+-rw-r--r--   0 austinwallace   (501) staff       (20)     1803 2024-04-24 18:52:09.000000 hrcl_jobs-1.7.0/.gitignore
+-rw-r--r--   0 austinwallace   (501) staff       (20)     1074 2023-02-02 20:22:41.000000 hrcl_jobs-1.7.0/LICENSE
+-rw-r--r--   0 austinwallace   (501) staff       (20)     1344 2024-04-24 19:00:06.025466 hrcl_jobs-1.7.0/PKG-INFO
+-rw-r--r--   0 austinwallace   (501) staff       (20)      354 2024-04-24 18:52:09.000000 hrcl_jobs-1.7.0/README.md
+-rw-r--r--   0 austinwallace   (501) staff       (20)      116 2023-03-27 20:06:21.000000 hrcl_jobs-1.7.0/main.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)      925 2024-04-24 18:59:55.000000 hrcl_jobs-1.7.0/pyproject.toml
+-rw-r--r--   0 austinwallace   (501) staff       (20)      268 2024-04-24 19:00:06.026767 hrcl_jobs-1.7.0/setup.cfg
+drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2024-04-24 19:00:05.994343 hrcl_jobs-1.7.0/src/
+drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2024-04-24 19:00:06.008739 hrcl_jobs-1.7.0/src/hrcl_jobs/
+-rw-r--r--   0 austinwallace   (501) staff       (20)      618 2024-04-24 18:52:09.000000 hrcl_jobs-1.7.0/src/hrcl_jobs/__init__.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)    14403 2023-05-18 20:01:58.000000 hrcl_jobs-1.7.0/src/hrcl_jobs/data.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)    11265 2024-04-24 18:52:09.000000 hrcl_jobs-1.7.0/src/hrcl_jobs/dataset.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)      968 2023-05-18 20:01:58.000000 hrcl_jobs-1.7.0/src/hrcl_jobs/examples.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)      893 2023-05-18 20:01:58.000000 hrcl_jobs-1.7.0/src/hrcl_jobs/jobspec.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)    17203 2024-04-24 18:52:09.000000 hrcl_jobs-1.7.0/src/hrcl_jobs/parallel.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)     9849 2024-04-24 18:52:09.000000 hrcl_jobs-1.7.0/src/hrcl_jobs/pgsql.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)    20138 2023-05-18 20:01:58.000000 hrcl_jobs-1.7.0/src/hrcl_jobs/s22.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)     7666 2024-04-24 18:52:09.000000 hrcl_jobs-1.7.0/src/hrcl_jobs/serial.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)     9059 2023-12-17 05:22:13.000000 hrcl_jobs-1.7.0/src/hrcl_jobs/setup.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)    30828 2024-04-24 18:52:09.000000 hrcl_jobs-1.7.0/src/hrcl_jobs/sqlt.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)     2929 2023-03-27 20:06:21.000000 hrcl_jobs-1.7.0/src/hrcl_jobs/tools_og.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)     2548 2024-01-08 18:45:15.000000 hrcl_jobs-1.7.0/src/hrcl_jobs/utils.py
+drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2024-04-24 19:00:06.023581 hrcl_jobs-1.7.0/src/hrcl_jobs.egg-info/
+-rw-r--r--   0 austinwallace   (501) staff       (20)     1344 2024-04-24 19:00:05.000000 hrcl_jobs-1.7.0/src/hrcl_jobs.egg-info/PKG-INFO
+-rw-r--r--   0 austinwallace   (501) staff       (20)     1150 2024-04-24 19:00:05.000000 hrcl_jobs-1.7.0/src/hrcl_jobs.egg-info/SOURCES.txt
+-rw-r--r--   0 austinwallace   (501) staff       (20)        1 2024-04-24 19:00:05.000000 hrcl_jobs-1.7.0/src/hrcl_jobs.egg-info/dependency_links.txt
+-rw-r--r--   0 austinwallace   (501) staff       (20)      151 2024-04-24 19:00:05.000000 hrcl_jobs-1.7.0/src/hrcl_jobs.egg-info/requires.txt
+-rw-r--r--   0 austinwallace   (501) staff       (20)       78 2024-04-24 19:00:05.000000 hrcl_jobs-1.7.0/src/hrcl_jobs.egg-info/top_level.txt
+-rw-r--r--   0 austinwallace   (501) staff       (20)        1 2023-02-02 20:26:18.000000 hrcl_jobs-1.7.0/src/hrcl_jobs.egg-info/zip-safe
+drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2024-04-24 19:00:06.014237 hrcl_jobs-1.7.0/src/hrcl_jobs_docking/
+-rw-r--r--   0 austinwallace   (501) staff       (20)      110 2024-04-24 18:52:09.000000 hrcl_jobs-1.7.0/src/hrcl_jobs_docking/__init__.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)    12147 2024-04-24 18:59:55.000000 hrcl_jobs-1.7.0/src/hrcl_jobs_docking/datasets.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)    22213 2024-04-24 18:59:55.000000 hrcl_jobs-1.7.0/src/hrcl_jobs_docking/docking_inps.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)     1503 2024-04-24 18:52:09.000000 hrcl_jobs-1.7.0/src/hrcl_jobs_docking/jobspec.py
+drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2024-04-24 19:00:06.016221 hrcl_jobs-1.7.0/src/hrcl_jobs_orca/
+-rw-r--r--   0 austinwallace   (501) staff       (20)       24 2023-05-18 20:01:58.000000 hrcl_jobs-1.7.0/src/hrcl_jobs_orca/__init__.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)      628 2023-12-17 05:22:13.000000 hrcl_jobs-1.7.0/src/hrcl_jobs_orca/jobspec.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)     8196 2023-12-17 05:22:13.000000 hrcl_jobs-1.7.0/src/hrcl_jobs_orca/orca_inps.py
+drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2024-04-24 19:00:06.020072 hrcl_jobs-1.7.0/src/hrcl_jobs_psi4/
+-rw-r--r--   0 austinwallace   (501) staff       (20)     1554 2024-04-24 18:52:09.000000 hrcl_jobs-1.7.0/src/hrcl_jobs_psi4/__init__.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)      703 2023-12-17 05:22:13.000000 hrcl_jobs-1.7.0/src/hrcl_jobs_psi4/basis_sets.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)        0 2023-12-17 05:22:13.000000 hrcl_jobs-1.7.0/src/hrcl_jobs_psi4/datasets.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)     3729 2024-04-24 18:59:55.000000 hrcl_jobs-1.7.0/src/hrcl_jobs_psi4/jobspec.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)      615 2024-04-24 18:52:09.000000 hrcl_jobs-1.7.0/src/hrcl_jobs_psi4/methods.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)    51206 2024-04-24 18:59:55.000000 hrcl_jobs-1.7.0/src/hrcl_jobs_psi4/psi4_inps.py
+drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2024-04-24 19:00:06.022767 hrcl_jobs-1.7.0/src/hrcl_jobs_qcfractal/
+-rw-r--r--   0 austinwallace   (501) staff       (20)       45 2023-12-17 05:22:13.000000 hrcl_jobs-1.7.0/src/hrcl_jobs_qcfractal/__init__.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)     1805 2023-12-17 05:22:13.000000 hrcl_jobs-1.7.0/src/hrcl_jobs_qcfractal/jobspec.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)    13655 2023-12-17 05:22:13.000000 hrcl_jobs-1.7.0/src/hrcl_jobs_qcfractal/psi4_inps.py
+-rw-r--r--   0 austinwallace   (501) staff       (20)       27 2023-12-17 05:22:13.000000 hrcl_jobs-1.7.0/src/hrcl_jobs_qcfractal/serial.py
```

### Comparing `hrcl_jobs-1.6.0/LICENSE` & `hrcl_jobs-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.6.0/PKG-INFO` & `hrcl_jobs-1.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hrcl_jobs
-Version: 1.6.0
+Version: 1.7.0
 Summary: Runs python functions on worker threads with main thread communicating with sql db
 Author-email: "Austin M. Wallace" <awallace43@gatech.edu>
 Project-URL: Homepage, https://github.com/Awallace3/hierarchical_python_jobs
 Project-URL: Bug Tracker, https://github.com/Awallace3/hierarchical_python_jobs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hrcl_jobs-1.6.0/pyproject.toml` & `hrcl_jobs-1.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hrcl_jobs"
-version = "1.6.0"
+version = "1.7.0"
 authors = [
   { name="Austin M. Wallace", email="awallace43@gatech.edu" },
 ]
 description = "Runs python functions on worker threads with main thread communicating with sql db"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `hrcl_jobs-1.6.0/src/hrcl_jobs/__init__.py` & `hrcl_jobs-1.7.0/src/hrcl_jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.6.0/src/hrcl_jobs/data.py` & `hrcl_jobs-1.7.0/src/hrcl_jobs/data.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.6.0/src/hrcl_jobs/dataset.py` & `hrcl_jobs-1.7.0/src/hrcl_jobs/dataset.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.6.0/src/hrcl_jobs/examples.py` & `hrcl_jobs-1.7.0/src/hrcl_jobs/examples.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.6.0/src/hrcl_jobs/jobspec.py` & `hrcl_jobs-1.7.0/src/hrcl_jobs/jobspec.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.6.0/src/hrcl_jobs/parallel.py` & `hrcl_jobs-1.7.0/src/hrcl_jobs/parallel.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,22 @@
         self.cores = cores
         self.threads = threads
         self.memory = memory  # Total Memory
         self.memory_per_thread = memory_per_core
         self.omp_threads = omp_threads
 
 
+def truncated_output(lst, max_length_str=30):
+    trunc_lst = []
+    for i in lst:
+        if isinstance(i, str) and len(i) > max_length_str:
+            trunc_lst.append(i[:max_length_str] + "...")
+        else:
+            trunc_lst.append(i)
+    return trunc_lst
 
 
 def ms_sl_extra_info_pg(
     pgsql_op: pgsql.pgsql_operations,
     id_list=[0, 50],
     run_js_job=example_run_js_job,
     extra_info={},  # memory requirements should be set here
@@ -117,15 +125,16 @@
                         os.remove(i)
                     except FileNotFoundError:
                         continue
             pgsql_op.update(conn, output, id_value)
             i2 = time.time() - i1
             insertion_str = ""
             if print_insertion:
-                insertion_str = f", output={output}"
+                tmp = truncated_output(output)
+                insertion_str = f", output={tmp}"
             print(f"\nMAIN: id {id_value} inserted{insertion_str}\n")
         print("\nMAIN CLEANING UP PROCESSES\n")
         for n in range(n_procs - 1):
             output = comm.recv(source=MPI.ANY_SOURCE, tag=2)
             p = glob("psi.*.clean")
             target_proc = output.pop()
             for i in p:
@@ -135,15 +144,16 @@
                     except FileNotFoundError:
                         continue
             id_value = output.pop()
             pgsql_op.update(conn, output, id_value)
             comm.send(0, dest=target_proc, tag=2)
             insertion_str = ""
             if print_insertion:
-                insertion_str = f", output={output}"
+                tmp = truncated_output(output)
+                insertion_str = f", output={tmp}"
             print(f"\nMAIN: id {id_value} inserted{insertion_str}\n")
         print("\nCOMPLETED MAIN\n")
     else:
         js = 1
         req = comm.irecv(source=0, tag=2)
         js = req.wait()
         if js == 0:
```

### Comparing `hrcl_jobs-1.6.0/src/hrcl_jobs/pgsql.py` & `hrcl_jobs-1.7.0/src/hrcl_jobs/pgsql.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,16 @@
             id SERIAL PRIMARY KEY,
             {t1_id} INTEGER REFERENCES {schema_name}.{t1_name}({t1_id}) ON DELETE CASCADE,
             {t2_id} INTEGER REFERENCES {schema_name}.{t2_name}({t2_id}) ON DELETE CASCADE
         );
         """
         )
         print(f"Creating junction table {schema_name}.{new_table_name}")
-    except psycopg2.Error:
+    except psycopg2.Error as e:
+        print("ERROR:", e)
         print(f"Table {schema_name}.{new_table_name} exists")
         conn.rollback()
     conn.commit()
     return
 
 
 def update_by_id(
```

### Comparing `hrcl_jobs-1.6.0/src/hrcl_jobs/s22.py` & `hrcl_jobs-1.7.0/src/hrcl_jobs/s22.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.6.0/src/hrcl_jobs/serial.py` & `hrcl_jobs-1.7.0/src/hrcl_jobs/serial.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,14 +20,23 @@
     """
     example_run_js_job
     """
     v1 = js.val + 1
     v2 = js.val + 2
     return [v1, v2]
 
+def truncated_output(lst, max_length_str=30):
+    trunc_lst = []
+    for i in lst:
+        if isinstance(i, str) and len(i) > max_length_str:
+            trunc_lst.append(i[:max_length_str] + "...")
+        else:
+            trunc_lst.append(i)
+    return trunc_lst
+
 def ms_sl_extra_info_pg(
     pgsql_op: pgsql.pgsql_operations,
     id_list=[0, 50],
     run_js_job=example_run_js_job,
     extra_info={},  # memory requirements should be set here
     js_obj=example_js,
     print_insertion=False,
@@ -36,22 +45,24 @@
     first = True
     conn, cur = pgsql_op.connect_db()
     for n, active_ind in enumerate(id_list):
         js = pgsql_op.job_query(conn, active_ind, js_obj, extra_info)
         output = run_js_job(js)
         insertion_str = ""
         if print_insertion:
-            insertion_str = f", output={output}"
+            tmp = truncated_output(output)
+            insertion_str = f", output={tmp}"
         print(f"\nMAIN: id {active_ind} inserted{insertion_str}\n")
         pgsql_op.update(conn, output, active_ind)
     print((time.time() - start) / 60, "Minutes")
     print("COMPLETED MAIN")
     return
 
 
+
 def ms_sl_extra_info(
     id_list=[0, 50],
     db_path="db/dimers_all.db",
     run_js_job=example_run_js_job,
     update_func=update_by_id,
     extra_info={},
     headers_sql=["main_id", "id", "RA", "RB", "ZA", "ZB", "TQA", "TQB"],
@@ -89,15 +100,16 @@
             id_value=active_ind,
             id_label=id_label,
             table=table_name,
         )
         output = run_js_job(js)
         insertion_str = ""
         if print_insertion:
-            insertion_str = f", output={output}"
+            tmp = truncated_output(output)
+            insertion_str = f", output={tmp}"
         print(f"\nMAIN: id {active_ind} inserted{insertion_str}\n")
         update_func(
             con,
             cur,
             output,
             id_value=active_ind,
             id_label=id_label,
```

### Comparing `hrcl_jobs-1.6.0/src/hrcl_jobs/setup.py` & `hrcl_jobs-1.7.0/src/hrcl_jobs/setup.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.6.0/src/hrcl_jobs/sqlt.py` & `hrcl_jobs-1.7.0/src/hrcl_jobs/sqlt.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.6.0/src/hrcl_jobs/tools_og.py` & `hrcl_jobs-1.7.0/src/hrcl_jobs/tools_og.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.6.0/src/hrcl_jobs/utils.py` & `hrcl_jobs-1.7.0/src/hrcl_jobs/utils.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.6.0/src/hrcl_jobs.egg-info/PKG-INFO` & `hrcl_jobs-1.7.0/src/hrcl_jobs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hrcl_jobs
-Version: 1.6.0
+Version: 1.7.0
 Summary: Runs python functions on worker threads with main thread communicating with sql db
 Author-email: "Austin M. Wallace" <awallace43@gatech.edu>
 Project-URL: Homepage, https://github.com/Awallace3/hierarchical_python_jobs
 Project-URL: Bug Tracker, https://github.com/Awallace3/hierarchical_python_jobs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hrcl_jobs-1.6.0/src/hrcl_jobs.egg-info/SOURCES.txt` & `hrcl_jobs-1.7.0/src/hrcl_jobs.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+.gitignore
 LICENSE
 README.md
+main.py
 pyproject.toml
 setup.cfg
 src/hrcl_jobs/__init__.py
 src/hrcl_jobs/data.py
 src/hrcl_jobs/dataset.py
 src/hrcl_jobs/examples.py
 src/hrcl_jobs/jobspec.py
```

### Comparing `hrcl_jobs-1.6.0/src/hrcl_jobs_docking/docking_inps.py` & `hrcl_jobs-1.7.0/src/hrcl_jobs_docking/docking_inps.py`

 * *Files 16% similar despite different names*

```diff
@@ -112,41 +112,51 @@
     """
     import apnet
     import tensorflow as tf
 
     # tf.config.threading.set_intra_op_parallelism_threads(js.extra_info["n_cpus"])
     # tf.config.threading.set_inter_op_parallelism_threads(js.extra_info["n_cpus"])
     # gpus = tf.config.experimental.list_physical_devices('GPU')
-    physical_cpus = tf.config.experimental.list_physical_devices("CPU")
-    assert physical_cpus, "No CPUs were detected."
+    # physical_cpus = tf.config.experimental.list_physical_devices("CPU")
+    # assert physical_cpus, "No CPUs were detected."
     # memory = compute_memory(js.extra_info["mem_per_process"])
     # assert memory, "No memory was detected."
 
     # tf.config.threading.set_intra_op_parallelism_threads(0)
     # tf.config.threading.set_inter_op_parallelism_threads(0)
 
+    verbose = js.extra_info.get("verbosity", 0)
+    if verbose:
+        pp(js.__dict__)
+
     if js.PRO_PDB is None:
         return [None, None, None, None, None, "PRO_PDB is None"]
-    if js.LIG_PDB is None:
-        return [None, None, None, None, None, "LIG_PDB is None"]
-
     try:
+        if isinstance(js, jobspec.apnet_pdbs_js):
+            lig_universe = mda.Universe(js.LIG_PDB)
+            lig_xyz = mda_selection_to_xyz(lig_universe.atoms)
+        elif isinstance(js, jobspec.apnet_pdb_sf_geom_js):
+            lig_xyz = np.array(js.geometry_xyz)
+            lig_elements = np.array([qcel.periodictable.to_Z(i) for i in js.geometry_ele]
+)
+            lig_xyz = np.concatenate((np.reshape(lig_elements, (-1, 1)), lig_xyz), axis=1)
+        else:
+            raise ValueError("js must be of type apnet_pdbs_js or apnet_pdb_sf_geom_js")
+
         pro_universe = mda.Universe(js.PRO_PDB)
-        lig_universe = mda.Universe(js.LIG_PDB)
         pro_xyz = mda_selection_to_xyz(
             pro_universe.select_atoms("all and not altloc B")
         )
         atom_count_protein = len(pro_xyz)
         max_atoms = js.extra_info.get("atom_max", None)
         if max_atoms is not None and atom_count_protein > max_atoms:
             return [None, None, None, None, None, "atom_count_protein > atom_max"]
-        lig_xyz = mda_selection_to_xyz(lig_universe.atoms)
         pro_cm = [js.PRO_CHARGE, 1]
         lig_cm = [js.LIG_CHARGE, 1]
-        print(f"{pro_universe} {js.PRO_CHARGE} {js.PRO_PDB}", f"{lig_universe} {js.LIG_CHARGE} {js.LIG_PDB}", sep="\n")
+        # print(f"{pro_universe} {js.PRO_CHARGE} {js.PRO_PDB}", f"{lig_universe} {js.LIG_CHARGE} {js.LIG_PDB}", sep="\n")
         mon_a = qm_tools_aw.tools.print_cartesians_pos_carts_symbols(
             pro_xyz[:, 0], pro_xyz[:, 1:], only_results=True
         )
         mon_b = qm_tools_aw.tools.print_cartesians_pos_carts_symbols(
             lig_xyz[:, 0], lig_xyz[:, 1:], only_results=True
         )
         apnet_error = None
@@ -188,26 +198,30 @@
 
 
 def prepare_receptor4(receptor_filename, outputfilename):
     cmd = f"python3 ~/data/gits/apnet_docking/docking_practice/MGLToolsPckgsPy3/prepare_receptor4.py -r receptor_filename -o outputfilename"
     out = subprocess.run(cmd, shell=True, check=True)
 
 
-def run_autodock_vina(js: jobspec.autodock_vina_js, verbose=1) -> []:
+def run_autodock_vina(js: jobspec.autodock_vina_js) -> []:
     """
     User must provide the following in js.extra_info:
     - sf_name: str
     - setup_python_files_path: str
     where sf_name is the name of the scoring function ['vina', 'ad4'] and
     setup_python_files_path is path to ligand_preparation.py and
     receptor_preparation.py
     """
     import docking_tools_amw
-
-    # try:
+    if js.extra_info.get("verbosity", 0) > 0:
+        verbose = 1
+    else:
+        verbose = None
+    if verbose:
+        pp(js.__dict__)
     if "n_poses" in js.extra_info.keys():
         n_poses = js.extra_info["sf_params"]["n_poses"]
     else:
         n_poses = 10
     if "exhaustiveness" in js.extra_info.keys():
         exhaustiveness = js.extra_info["sf_params"]["exhaustiveness"]
     else:
@@ -224,61 +238,56 @@
     if identifier is None:
         identifier = "_0"
     else:
         identifier = f"_{identifier}"
     npts_param = f"npts={npts[0]},{npts[1]},{npts[2]}"
     sf_name = js.extra_info["sf_name"]
     v = Vina(sf_name=sf_name, cpu=js.extra_info["n_cpus"], seed=875234)
-    # TODO: set_weights for vina and ad4
-    # need to run on docked structure single-point energy and collect
-    # v.set_weights([])
+
     if js.PRO_PDB is None:
-        return [None, None, None, None, None, None, None, "PRO_PDBQT is None"]
+        return [None, None, None, None, None, None, None, None, "PRO_PDBQT is None"]
     if js.LIG_PDB is None:
-        return [None, None, None, None, None, None, None, "LIG_PDBQT is None"]
+        return [None, None, None, None, None, None, None, None, "LIG_PDBQT is None"]
 
     PRO_PDBQT = js.PRO_PDB + "qt"
     LIG_PDBQT = js.LIG_PDB + "qt"
-    # WAT_PDBQT = js.WAT_PDB + "qt"
-    # OTH_PDBQT = js.OTH_PDB + "qt"
-    PRO = PRO_PDBQT.replace(".pdbqt", "")
+    PRO_PDBQT = PRO_PDBQT.replace(".pdbqt", f"{identifier}.pdbqt")
+    LIG_PDBQT = LIG_PDBQT.replace(".pdbqt", f"{identifier}.pdbqt")
     def_dir = os.getcwd()
     try:
         if verbose:
             print(PRO_PDBQT, LIG_PDBQT, sep="\n")
-        if not os.path.exists(PRO_PDBQT):
-            docking_tools_amw.prepare_receptor4.prepare_receptor4(
-                receptor_filename=js.PRO_PDB,
-                outputfilename=PRO_PDBQT,
-                # charges_to_add=None,
-            )
-        if not os.path.exists(LIG_PDBQT):
-            docking_tools_amw.prepare_ligand4.prepare_ligand4(
-                ligand_filename=js.LIG_PDB,
-                outputfilename=LIG_PDBQT,
-                repairs="hydrogen",
-            )
+        docking_tools_amw.prepare_receptor4.prepare_receptor4(
+            receptor_filename=js.PRO_PDB,
+            outputfilename=PRO_PDBQT,
+            # charges_to_add=None,
+        )
+        docking_tools_amw.prepare_ligand4.prepare_ligand4(
+            ligand_filename=js.LIG_PDB,
+            outputfilename=LIG_PDBQT,
+            repairs="",
+        )
         # find the center of the binding pocket, for this dataset that is also the center of mass of the ligand
         com = get_com(js.LIG_PDB)
         # set the ligand
         ad_vina_errors = None
-        # if vina or vinardo then set the receptor and computer the vina maps, if autodock then prepare the gpf and autogrid
         # NOTE: receptor must be set before ligand
         if sf_name in ["vina", "vinardo"]:
-            print(sf_name)
             v.set_receptor(PRO_PDBQT)
             v.compute_vina_maps(center=com, box_size=box_size)
         elif sf_name == "ad4":
+            PRO = PRO_PDBQT.replace(".pdbqt", "")
             os.chdir("/".join(PRO.split("/")[:-1]))
             PRO_MAP = PRO.split("/")[-1]
             PRO = PRO_MAP + identifier
 
             PRO_GPF = f"{PRO}.gpf"
             PRO_GLG = f"{PRO}.glg"
-            print(f"{PRO_GPF = }")
+            if verbose:
+                print(f"{PRO_GPF = }")
             PRO_PDBQT = PRO_PDBQT.split("/")[-1]
             LIG_PDBQT = LIG_PDBQT.split("/")[-1]
             docking_tools_amw.prepare_gpf.prepare_gpf(
                 receptor_filename=PRO_PDBQT,
                 ligand_filename=LIG_PDBQT,
                 output_gpf_filename=PRO_GPF,
                 parameters=[npts_param],
@@ -289,50 +298,70 @@
             v.load_maps(PRO)
         else:
             ad_vina_errors = "invalid sf_name"
         v.set_ligand_from_file(LIG_PDBQT)
 
         # docking
         v.dock(exhaustiveness=exhaustiveness, n_poses=n_poses)
-        vina_out = LIG_PDBQT.replace(".pdbqt", f"{js.LIG_NAME.replace(':', '_')}_{js.system}_out.pdb")
-        v.write_poses(vina_out, n_poses=n_poses, overwrite=True)
         energies = v.energies(n_poses=n_poses)
 
+        vina_out = LIG_PDBQT.replace(".pdbqt", f"_{sf_name}_{js.LIG_NAME.replace(':', '_')}_{js.system}_out.pdbqt")
+        obabel_out = vina_out.replace('.pdbqt', '_best.pdb')
+
+        v.write_poses(vina_out, n_poses=10, overwrite=True)
+        with open(vina_out, "r") as f:
+            sf_all_poses_pdbqt_str = f.read()
+        v.write_poses(vina_out, n_poses=1, overwrite=True)
+        obabel_cmd = f"{js.extra_info['obabel_path']} -ipdbqt {vina_out} -opdb -O{obabel_out}"
+        os.system(obabel_cmd)
+        with open(obabel_out, "r") as f:
+            sf_best_pose_pdb_str = f.read()
+        if verbose:
+            print(f"{vina_out = }")
+            print(sf_best_pose_pdb_str)
+        os.system(f"rm {obabel_out} {vina_out} {LIG_PDBQT} {PRO_PDBQT}")
         if sf_name == "ad4":
             cmd = f"rm {PRO_GPF} {PRO_GLG} {PRO}.map*"
             os.system(cmd)
             os.chdir(def_dir)
 
     except Exception as e:
         ad_vina_errors = str(e)
         os.chdir(def_dir)
     if ad_vina_errors == None:
         return [
-            energies[0][0],
-            energies[0][1],
-            energies[0][2],
-            energies[0][3],
-            energies[0][4],
-            vina_out,
-            energies,
+            energies[0][0],         # total
+            energies[0][1],         # inter
+            energies[0][2],         # intra
+            energies[0][3],         # torsion
+            energies[0][4],         # intra_best_pose / minus_intra
+            sf_all_poses_pdbqt_str, # all_poses pdbqt as str
+            energies,               # all poses energies
+            sf_best_pose_pdb_str,   # best pose's pdb as str
             ad_vina_errors,
         ]
     else:
-        return [None, None, None, None, None, None, None, ad_vina_errors]
+        return [None, None, None, None, None, None, None, None, ad_vina_errors]
 
-def run_autodock_vina_components(js: jobspec.autodock_vina_js, verbose=1) -> []:
+def run_autodock_vina_components(js: jobspec.autodock_vina_js) -> []:
     """
     User must provide the following in js.extra_info:
     - sf_name: str
     - setup_python_files_path: str
     where sf_name is the name of the scoring function ['vina', 'ad4'] and
     setup_python_files_path is path to ligand_preparation.py and
     receptor_preparation.py
     """
     import docking_tools_amw
+    if js.extra_info.get("verbosity", 0) > 0:
+        verbose = 1
+    else:
+        verbose = None
+    if verbose:
+        pp(js.__dict__)
 
     # try:
     if "n_poses" in js.extra_info.keys():
         n_poses = js.extra_info["sf_params"]["n_poses"]
     else:
         n_poses = 10
     if "exhaustiveness" in js.extra_info.keys():
@@ -351,121 +380,118 @@
     if identifier is None:
         identifier = "_0"
     else:
         identifier = f"_{identifier}"
     npts_param = f"npts={npts[0]},{npts[1]},{npts[2]}"
     sf_name = js.extra_info["sf_name"]
     v = Vina(sf_name=sf_name, cpu=js.extra_info["n_cpus"], seed=875234)
+
     if js.PRO_PDB is None:
         return [None, None, None, None, None, None, None, "PRO_PDBQT is None"]
     if js.LIG_PDB is None:
         return [None, None, None, None, None, None, None, "LIG_PDBQT is None"]
 
     PRO_PDBQT = js.PRO_PDB + "qt"
     LIG_PDBQT = js.LIG_PDB + "qt"
-    # WAT_PDBQT = js.WAT_PDB + "qt"
-    # OTH_PDBQT = js.OTH_PDB + "qt"
+    PRO_PDBQT = PRO_PDBQT.replace(".pdbqt", f"{identifier}.pdbqt")
+    LIG_PDBQT = LIG_PDBQT.replace(".pdbqt", f"{identifier}.pdbqt")
     PRO = PRO_PDBQT.replace(".pdbqt", "")
     def_dir = os.getcwd()
     try:
         if verbose:
             print(PRO_PDBQT, LIG_PDBQT, sep="\n")
-        if not os.path.exists(PRO_PDBQT):
-            docking_tools_amw.prepare_receptor4.prepare_receptor4(
-                receptor_filename=js.PRO_PDB,
-                outputfilename=PRO_PDBQT,
-                # charges_to_add=None,
-            )
-        # if not os.path.exists(LIG_PDBQT):
-        if os.path.exists(LIG_PDBQT):
-            docking_tools_amw.prepare_ligand4.prepare_ligand4(
-                ligand_filename=js.LIG_PDB,
-                outputfilename=LIG_PDBQT,
-                repairs="",
-                verbose=True,
-            )
-        return
-        u = mda.Universe(js.LIG_PDB)
-        print(u.atoms.positions)
-        print(u.atoms.elements)
+        docking_tools_amw.prepare_receptor4.prepare_receptor4(
+            receptor_filename=js.PRO_PDB,
+            outputfilename=PRO_PDBQT,
+            # charges_to_add=None,
+        )
+        docking_tools_amw.prepare_ligand4.prepare_ligand4(
+            ligand_filename=js.LIG_PDB,
+            outputfilename=LIG_PDBQT,
+            repairs="",
+            verbose=None,
+        )
         # find the center of the binding pocket, for this dataset that is also the center of mass of the ligand
         com = get_com(js.LIG_PDB)
-        # set the ligand
         ad_vina_errors = None
-        # if vina or vinardo then set the receptor and computer the vina maps, if autodock then prepare the gpf and autogrid
         # NOTE: receptor must be set before ligand
         if sf_name in ["vina", "vinardo"]:
-            print(sf_name)
             v.set_receptor(PRO_PDBQT)
             v.compute_vina_maps(center=com, box_size=box_size)
         elif sf_name == "ad4":
             os.chdir("/".join(PRO.split("/")[:-1]))
             PRO_MAP = PRO.split("/")[-1]
             PRO = PRO_MAP + identifier
 
             PRO_GPF = f"{PRO}.gpf"
             PRO_GLG = f"{PRO}.glg"
-            print(f"{PRO_GPF = }")
+            if verbose:
+                print(f"{PRO_GPF = }")
             PRO_PDBQT = PRO_PDBQT.split("/")[-1]
             LIG_PDBQT = LIG_PDBQT.split("/")[-1]
             docking_tools_amw.prepare_gpf.prepare_gpf(
                 receptor_filename=PRO_PDBQT,
                 ligand_filename=LIG_PDBQT,
                 output_gpf_filename=PRO_GPF,
                 parameters=[npts_param],
                 identifier=identifier,
             )
             cmd = f"autogrid4 -p {PRO_GPF} -l {PRO_GLG}"
             os.system(cmd)
             v.load_maps(PRO)
         else:
             ad_vina_errors = "invalid sf_name"
-        v.set_ligand_from_file(LIG_PDBQT)
-
-        # docking
-        v.dock(exhaustiveness=exhaustiveness, n_poses=n_poses)
-        vina_out = LIG_PDBQT.replace(".pdbqt", f"{js.LIG_NAME.replace(':', '_')}_{js.system}_out.pdb")
-        v.write_poses(vina_out, n_poses=n_poses, overwrite=True)
-        poses = v.poses(n_poses=1, coordinates_only=True)
-        print(f"{poses = }")
-        energies = v.energies(n_poses=n_poses)
+        energies = v.energies(n_poses=1)
+        print(f"{energies = }")
 
         weighted_energies = []
-
         if sf_name == "ad4":
             ad4_weights = [0.1662, 0.1209, 0.1406, 0.1322, 50]
             for n, i in enumerate(ad4_weights):
                 new_weighs = [0] * 5
                 new_weighs[n] = i
                 v.set_weights(new_weighs)
+                v.score()
                 e = v.energies(n_poses=1)
                 print(e)
                 weighted_energies.append(e)
             cmd = f"rm {PRO_GPF} {PRO_GLG} {PRO}.map*"
             os.system(cmd)
             os.chdir(def_dir)
         elif sf_name == "vina":
-            vina_weights = [-0.035579, -0.005156, 0.840245, -0.035069, -0.587439, 50, 0.05846]
+            # vina_weights = [gau1, gau2, repulsion, hydrophobic, Hydrogen_bonding, npts?, n_rot, ]
+            # https://onlinelibrary.wiley.com/doi/10.1002/jcc.21334
+            vina_weights = [-0.035579, -0.005156, 0.840245, -0.035069, -0.587439, 0.05846]
             for n, i in enumerate(vina_weights):
-                new_weights = [0] * 7
+                new_weights = [0] * 6
                 new_weights[n] = i
-                print(new_weights)
-                v.set_weights(new_weights)
-                print(v.info())
-                e = v.score()
-                print(e)
-                weighted_energies.append(e)
+                print(f"{new_weights = }")
+                vina_cmd = f"vina --receptor {PRO_PDBQT} --ligand {LIG_PDBQT} --scoring vina --autobox --score_only --cpu {js.extra_info['n_cpus']} --weight_gauss1 {new_weights[0]} --weight_gauss2 {new_weights[1]} --weight_repulsion {new_weights[2]} --weight_hydrophobic {new_weights[3]} --weight_hydrogen {new_weights[4]} --weight_rot {new_weights[5]}"
+
+                vina_cmd = f"vina --receptor {PRO_PDBQT} --ligand {LIG_PDBQT} --autobox --scoring vina --autobox --score_only --cpu {js.extra_info['n_cpus']} --weight_gauss1 {new_weights[0]}"
+                print(vina_cmd)
+                vina_cmd = vina_cmd.split(" ")
+                print(vina_cmd)
+                res = subprocess.call(vina_cmd, shell=True)
+                print(res)
+                # weighted_energies.append(e)
+            # TODO: add remove of pdbqt files
         elif sf_name == 'vinardo':
             vinardo_weights = [-0.045, 0.8, -0.035, -0.6, 50, 0.05846]
             for n, i in enumerate(vinardo_weights):
                 new_weighs = [0] * 6
                 new_weighs[n] = i
                 v.set_weights(new_weighs)
-                e = v.energies(n_poses=1)
+                v.compute_vina_maps(center=com, box_size=box_size)
+                e = v.energies()
                 weighted_energies.append(e)
+            # TODO: add remove of pdbqt files
+        weighted_energies = np.array(weighted_energies)
+        weighted_total_sum = np.sum(weighted_energies[:, 0])
+        print(f"{weighted_total_sum = }")
         print(f"{weighted_energies = }")
 
     except Exception as e:
         ad_vina_errors = str(e)
         print(ad_vina_errors)
         os.chdir(def_dir)
     if ad_vina_errors == None:
@@ -478,16 +504,68 @@
             vina_out,
             energies,
             ad_vina_errors,
         ]
     else:
         return [None, None, None, None, None, None, None, ad_vina_errors]
 
-# return data as a list in the following order (and typing)
-# "vina_total__LIG": "REAL",
-# "vina_inter__LIG": "REAL",
-# "vina_intra__LIG": "REAL",
-# "vina_torsion__LIG": "REAL",
-# "vina_intra_best_pose__LIG": "REAL",
-# "vina_poses_pdbqt__LIG": "TEXT",
-# "vina_all_poses__LIG": "array",
-# "vina_errors__LIG": "TEXT",
+"""
+(apd7) ➜  ~/data/apnet/create_models   git:(main) ✗ vina --help_advanced
+AutoDock Vina b87c493-mod
+
+Input:
+  --receptor arg                        rigid part of the receptor (PDBQT)
+  --flex arg                            flexible side chains, if any (PDBQT)
+  --ligand arg                          ligand (PDBQT)
+  --batch arg                           batch ligand (PDBQT)
+  --scoring arg (=vina)                 scoring function (ad4, vina or vinardo)
+
+Output (optional):
+  --out arg                             output models (PDBQT), the default is
+                                        chosen based on the ligand file name
+  --dir arg                             output directory for batch mode
+  --write_maps arg                      output filename (directory + prefix
+                                        name) for maps. Option
+                                        --force_even_voxels may be needed to
+                                        comply with .map format
+
+Advanced options (see the manual):
+  --score_only                          score only - search space can be
+                                        omitted
+  --unbound_energy arg (=nan)           Explicitly set the Unbound System's
+                                        Energy for --score_only jobs
+                                        --score_only jobs
+  --weight_gauss1 arg (=-0.035579)      gauss_1 weight
+  --weight_gauss2 arg (=-0.005156)      gauss_2 weight
+  --weight_repulsion arg (=0.84024500000000002)
+                                        repulsion weight
+  --weight_hydrophobic arg (=-0.035069000000000003)
+                                        hydrophobic weight
+  --weight_hydrogen arg (=-0.58743900000000004)
+                                        Hydrogen bond weight
+  --weight_rot arg (=0.058459999999999998)
+                                        N_rot weight
+  --weight_vinardo_gauss1 arg (=-0.044999999999999998)
+                                        Vinardo gauss_1 weight
+  --weight_vinardo_repulsion arg (=0.80000000000000004)
+                                        Vinardo repulsion weight
+  --weight_vinardo_hydrophobic arg (=-0.035000000000000003)
+                                        Vinardo hydrophobic weight
+  --weight_vinardo_hydrogen arg (=-0.59999999999999998)
+                                        Vinardo Hydrogen bond weight
+  --weight_vinardo_rot arg (=0.058459999999999998)
+                                        Vinardo N_rot weight
+  --weight_ad4_vdw arg (=0.16619999999999999)
+                                        ad4_vdw weight
+  --weight_ad4_hb arg (=0.12089999999999999)
+                                        ad4_hb weight
+  --weight_ad4_elec arg (=0.1406)       ad4_elec weight
+  --weight_ad4_dsolv arg (=0.13220000000000001)
+                                        ad4_dsolv weight
+  --weight_ad4_rot arg (=0.29830000000000001)
+                                        ad4_rot weight
+  --weight_glue arg (=50)               macrocycle glue weight
+
+  --cpu arg (=0)                        the number of CPUs to use (the default
+                                        is to try to detect the number of CPUs
+                                        or, failing that, use 1)
+"""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hrcl_jobs-1.6.0/src/hrcl_jobs_docking/jobspec.py` & `hrcl_jobs-1.7.0/src/hrcl_jobs_docking/jobspec.py`

 * *Files 17% similar despite different names*

```diff
@@ -44,14 +44,26 @@
     LIG_PDB: str
     PRO_CHARGE: int
     LIG_CHARGE: int
     system: str
     extra_info: {}
     mem: str = None
 
+@dataclass
+class apnet_pdb_sf_geom_js:
+    id_label: int
+    PRO_PDB: str
+    geometry_xyz: []
+    geometry_ele: []
+    PRO_CHARGE: int
+    LIG_CHARGE: int
+    system: str
+    extra_info: {}
+    mem: str = None
+
 
 def apnet_disco_js_headers():
     return [
         "id",
         "PRO_PDB_Hs",
         "LIG_PDB",
         "WAT_PDB",
```

### Comparing `hrcl_jobs-1.6.0/src/hrcl_jobs_orca/jobspec.py` & `hrcl_jobs-1.7.0/src/hrcl_jobs_orca/jobspec.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.6.0/src/hrcl_jobs_orca/orca_inps.py` & `hrcl_jobs-1.7.0/src/hrcl_jobs_orca/orca_inps.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.6.0/src/hrcl_jobs_psi4/__init__.py` & `hrcl_jobs-1.7.0/src/hrcl_jobs_psi4/__init__.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.6.0/src/hrcl_jobs_psi4/basis_sets.py` & `hrcl_jobs-1.7.0/src/hrcl_jobs_psi4/basis_sets.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.6.0/src/hrcl_jobs_psi4/jobspec.py` & `hrcl_jobs-1.7.0/src/hrcl_jobs_psi4/jobspec.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,14 +180,35 @@
         "monAs",
         "monBs",
         "charges",
         # "grac_shift_a",
         # "grac_shift_b",
     ]
 
+@dataclass
+class ccsd_t_CBS_js:
+    id_label: int
+    geometry: np.array
+    monAs: np.array
+    monBs: np.array
+    charges: np.array
+    extra_info: {}
+    mem: str
+
+
+def ccsd_T_CBS_js_headers():
+    return [
+        "id",
+        "Geometry",
+        "monAs",
+        "monBs",
+        "charges",
+    ]
+
+
 
 @dataclass
 class saptdft_mon_grac_js:
     id_label: int
     geometry: np.array
     monNs: np.array
     charges: np.array
```

### Comparing `hrcl_jobs-1.6.0/src/hrcl_jobs_psi4/methods.py` & `hrcl_jobs-1.7.0/src/hrcl_jobs_psi4/methods.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.6.0/src/hrcl_jobs_psi4/psi4_inps.py` & `hrcl_jobs-1.7.0/src/hrcl_jobs_psi4/psi4_inps.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from qm_tools_aw import tools
 import qcelemental as qcel
 from pprint import pprint as pp
 
 """
 /theoryfs2/ds/amwalla3/miniconda3/envs/psi4mpi4py_qcng/lib/python3.8/site-packages/psi4/driver/driver_nbody.py
 """
-
+h2kcalmol = constants.conversion_factor("hartree", "kcal / mol")
 
 class NumpyEncoder(json.JSONEncoder):
     def default(self, obj):
         if isinstance(obj, np.ndarray):
             return obj.tolist()
         return json.JSONEncoder.default(self, obj)
 
@@ -508,32 +508,104 @@
     )
     es = []
     for l in js.extra_info["level_theory"]:
         mol = psi4.geometry(geom)
         js.extra_info["options"]["sapt_dft_grac_shift_a"] = js.grac_shift_a
         js.extra_info["options"]["sapt_dft_grac_shift_b"] = js.grac_shift_b
         handle_hrcl_extra_info_options(js, l)
-
+        do_ddft_d4 = "SAPT_DFT_DO_DDFT" in js.extra_info["options"].keys() and "SAPT_DFT_D4_IE" in js.extra_info["options"].keys()
         try:
             e = psi4.energy(f"{l}")
             e *= constants.conversion_factor("hartree", "kcal / mol")
             ie = psi4.core.variable("SAPT(DFT) TOTAL ENERGY")
             ELST = psi4.core.variable("SAPT ELST ENERGY")
             EXCH = psi4.core.variable("SAPT EXCH ENERGY")
             IND = psi4.core.variable("SAPT IND ENERGY")
             DISP = psi4.core.variable("SAPT DISP ENERGY")
             mult = constants.conversion_factor("hartree", "kcal / mol")
+            if do_ddft_d4:
+                DELTA_HF = psi4.core.variable("SAPT(DFT) DELTA HF") * mult 
+                DDFT = psi4.core.variable("SAPT(DFT) DELTA DFT") * mult 
+                D4_IE = psi4.core.variable("D4 IE") * mult
+                DFT_MONA = psi4.core.variable("DFT MONOMER A ENERGY")
+                DFT_MONB = psi4.core.variable("DFT MONOMER B ENERGY")
+                DFT_DIMER = psi4.core.variable("DFT DIMER ENERGY")
+                DFT_IE = (DFT_DIMER - DFT_MONA - DFT_MONB) * mult 
+                DFTD4_IE = (DFT_DIMER - DFT_MONA - DFT_MONB) * mult + D4_IE
             out_energies = np.array([ie, ELST, EXCH, IND, DISP]) * mult
         except Exception as e:
             print("Exception:", e)
             out_energies = None
         es.append(out_energies)
+        if do_ddft_d4:
+            es.append(DELTA_HF)
+            es.append(DDFT)
+            es.append(D4_IE)
+            es.append(DFT_IE)
         handle_hrcl_psi4_cleanup(js, l)
     return es
 
+def run_sapt2p3(js: jobspec.sapt_js) -> np.array:
+    generate_outputs = "out" in js.extra_info.keys()
+    geom = tools.generate_p4input_from_df(
+        js.geometry, js.charges, js.monAs, js.monBs, units="angstrom"
+    )
+    es = []
+    for l in js.extra_info["level_theory"]:
+        mol = psi4.geometry(geom)
+        print(l)
+        handle_hrcl_extra_info_options(js, l)
+        try:
+            e = psi4.energy(f"{l}")
+            e *= constants.conversion_factor("hartree", "kcal / mol")
+            ie = e
+            # ELST = psi4.core.variable("SAPT ELST ENERGY")
+            # EXCH = psi4.core.variable("SAPT EXCH ENERGY")
+            # IND = psi4.core.variable("SAPT IND ENERGY")
+            # DISP = psi4.core.variable("SAPT DISP ENERGY")
+            mult = constants.conversion_factor("hartree", "kcal / mol")
+            out_energies = np.array([ie]) * mult
+        except Exception as e:
+            print("Exception:", e)
+            out_energies = None
+        es.append(out_energies)
+        handle_hrcl_psi4_cleanup(js, l)
+    return
+
+
+def run_ccsd_t_CBS_IE(js: jobspec.saptdft_js) -> np.array:
+    """
+    Untested
+    """
+    generate_outputs = "out" in js.extra_info.keys()
+    geom = tools.generate_p4input_from_df(
+        js.geometry, js.charges, js.monAs, js.monBs, units="angstrom"
+    )
+    cp = js.extra_info.get("CP", "NOCP")
+    es = []
+    for l in js.extra_info["level_theory"]:
+        mol = psi4.geometry(geom)
+        handle_hrcl_extra_info_options(js, l)
+        try:
+            e = psi4.energy(f"{l}", bsse_type=cp)
+            e *= constants.conversion_factor("hartree", "kcal / mol")
+            # ie = psi4.core.variable("SAPT(DFT) TOTAL ENERGY")
+            # ELST = psi4.core.variable("SAPT ELST ENERGY")
+            # EXCH = psi4.core.variable("SAPT EXCH ENERGY")
+            # IND = psi4.core.variable("SAPT IND ENERGY")
+            # DISP = psi4.core.variable("SAPT DISP ENERGY")
+            mult = constants.conversion_factor("hartree", "kcal / mol")
+            out_energies = np.array([e]) * mult
+        except Exception as e:
+            print("Exception:", e)
+            out_energies = None
+        es.append(out_energies)
+        handle_hrcl_psi4_cleanup(js, l)
+    return
+
 
 def run_psi4_saptdft(
     A: str,
     B: str,
     ppm: str = "4 gb",
     level_theory: [] = ["hf/cc-pvdz"],
     charge_mult: np.array = np.array([[0, 1], [0, 1], [0, 1]]),
@@ -852,18 +924,23 @@
     )
     es = []
     for l in js.extra_info["level_theory"]:
         handle_hrcl_extra_info_options(js, l)
         mol = psi4.geometry(geom)
         e = psi4.energy(f"{l}")
         e *= constants.conversion_factor("hartree", "kcal / mol")
+        pp(psi4.core.variables())
         ELST = psi4.core.variable("SAPT ELST ENERGY")
         EXCH = psi4.core.variable("SAPT EXCH ENERGY")
         IND = psi4.core.variable("SAPT IND ENERGY")
-        DISP = psi4.core.variable("SAPT DISP ENERGY")
+        # NOTE: would need to get 'SAPT-D TOTAL ENERGY' if not doing sum here
+        if 'sapt0-d' in l.lower():
+            DISP = psi4.core.variable("DISPERSION CORRECTION ENERGY")
+        else:
+            DISP = psi4.core.variable("SAPT DISP ENERGY")
         ie = sum([ELST, EXCH, IND, DISP])
         mult = constants.conversion_factor("hartree", "kcal / mol")
         out_energies = np.array([ie, ELST, EXCH, IND, DISP]) * mult
         es.append(out_energies)
         handle_hrcl_psi4_cleanup(js, l)
     return es
 
@@ -1028,29 +1105,29 @@
     if "out" in js.extra_info.keys() and "sub_path" in js.extra_info["out"].keys():
         job_dir += f"/{js.extra_info['out']['sub_path']}"
     if sub_job != 0:
         job_dir += f"/{sub_job}"
     return job_dir
 
 
-def handle_hrcl_extra_info_options(js, l, sub_job=0):
+def handle_hrcl_extra_info_options(js, l, sub_job=0, psi4_quiet=False):
     psi4.set_memory(js.mem)
     psi4.set_options(js.extra_info["options"])
     generate_outputs = "out" in js.extra_info.keys()
     set_scratch = "scratch" in js.extra_info.keys()
     if set_scratch:
         psi4.core.IOManager.shared_object().set_default_path(
             os.path.abspath(os.path.expanduser(js.extra_info["scratch"]["path"]))
         )
     if generate_outputs:
         job_dir = generate_job_dir(js, l, sub_job)
         os.makedirs(job_dir, exist_ok=True)
         psi4.set_output_file(f"{job_dir}/psi4.out", False, loglevel=10)
         psi4.core.print_out(f"{js}")
-    else:
+    elif psi4_quiet:
         psi4.core.be_quiet()
     if "num_threads" in js.extra_info.keys():
         psi4.set_num_threads(js.extra_info["num_threads"])
     return
 
 
 def handle_hrcl_psi4_cleanup(js, l, sub_job=0, psi4_clean_all=True, wfn=None):
```

### Comparing `hrcl_jobs-1.6.0/src/hrcl_jobs_qcfractal/jobspec.py` & `hrcl_jobs-1.7.0/src/hrcl_jobs_qcfractal/jobspec.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.6.0/src/hrcl_jobs_qcfractal/psi4_inps.py` & `hrcl_jobs-1.7.0/src/hrcl_jobs_qcfractal/psi4_inps.py`

 * *Files identical despite different names*

