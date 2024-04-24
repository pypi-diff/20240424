# Comparing `tmp/flytekitplugins-airflow-1.12.0b5.tar.gz` & `tmp/flytekitplugins_airflow-1.12.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-airflow-1.12.0b5.tar", last modified: Wed Apr 10 17:16:48 2024, max compression
+gzip compressed data, was "flytekitplugins_airflow-1.12.0b6.tar", last modified: Wed Apr 24 18:30:31 2024, max compression
```

## Comparing `flytekitplugins-airflow-1.12.0b5.tar` & `flytekitplugins_airflow-1.12.0b6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:48.163315 flytekitplugins-airflow-1.12.0b5/
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-10 17:16:48.163315 flytekitplugins-airflow-1.12.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-10 17:16:22.000000 flytekitplugins-airflow-1.12.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:48.159315 flytekitplugins-airflow-1.12.0b5/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:48.159315 flytekitplugins-airflow-1.12.0b5/flytekitplugins/airflow/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-10 17:16:22.000000 flytekitplugins-airflow-1.12.0b5/flytekitplugins/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7959 2024-04-10 17:16:22.000000 flytekitplugins-airflow-1.12.0b5/flytekitplugins/airflow/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     9131 2024-04-10 17:16:22.000000 flytekitplugins-airflow-1.12.0b5/flytekitplugins/airflow/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:48.159315 flytekitplugins-airflow-1.12.0b5/flytekitplugins_airflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-10 17:16:48.000000 flytekitplugins-airflow-1.12.0b5/flytekitplugins_airflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-10 17:16:48.000000 flytekitplugins-airflow-1.12.0b5/flytekitplugins_airflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:16:48.000000 flytekitplugins-airflow-1.12.0b5/flytekitplugins_airflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-10 17:16:48.000000 flytekitplugins-airflow-1.12.0b5/flytekitplugins_airflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 17:16:48.000000 flytekitplugins-airflow-1.12.0b5/flytekitplugins_airflow.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-10 17:16:48.000000 flytekitplugins-airflow-1.12.0b5/flytekitplugins_airflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 17:16:48.000000 flytekitplugins-airflow-1.12.0b5/flytekitplugins_airflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 17:16:48.163315 flytekitplugins-airflow-1.12.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-10 17:16:47.000000 flytekitplugins-airflow-1.12.0b5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:48.159315 flytekitplugins-airflow-1.12.0b5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-10 17:16:22.000000 flytekitplugins-airflow-1.12.0b5/tests/test_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-04-10 17:16:22.000000 flytekitplugins-airflow-1.12.0b5/tests/test_task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:31.957186 flytekitplugins_airflow-1.12.0b6/
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-24 18:30:31.953186 flytekitplugins_airflow-1.12.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-24 18:30:04.000000 flytekitplugins_airflow-1.12.0b6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:31.953186 flytekitplugins_airflow-1.12.0b6/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:31.953186 flytekitplugins_airflow-1.12.0b6/flytekitplugins/airflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-24 18:30:04.000000 flytekitplugins_airflow-1.12.0b6/flytekitplugins/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7959 2024-04-24 18:30:04.000000 flytekitplugins_airflow-1.12.0b6/flytekitplugins/airflow/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9131 2024-04-24 18:30:04.000000 flytekitplugins_airflow-1.12.0b6/flytekitplugins/airflow/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:31.953186 flytekitplugins_airflow-1.12.0b6/flytekitplugins_airflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-24 18:30:31.000000 flytekitplugins_airflow-1.12.0b6/flytekitplugins_airflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-24 18:30:31.000000 flytekitplugins_airflow-1.12.0b6/flytekitplugins_airflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 18:30:31.000000 flytekitplugins_airflow-1.12.0b6/flytekitplugins_airflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-24 18:30:31.000000 flytekitplugins_airflow-1.12.0b6/flytekitplugins_airflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 18:30:31.000000 flytekitplugins_airflow-1.12.0b6/flytekitplugins_airflow.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 18:30:31.000000 flytekitplugins_airflow-1.12.0b6/flytekitplugins_airflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 18:30:31.000000 flytekitplugins_airflow-1.12.0b6/flytekitplugins_airflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 18:30:31.957186 flytekitplugins_airflow-1.12.0b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-24 18:30:31.000000 flytekitplugins_airflow-1.12.0b6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:31.953186 flytekitplugins_airflow-1.12.0b6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-24 18:30:04.000000 flytekitplugins_airflow-1.12.0b6/tests/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-04-24 18:30:04.000000 flytekitplugins_airflow-1.12.0b6/tests/test_task.py
```

### Comparing `flytekitplugins-airflow-1.12.0b5/PKG-INFO` & `flytekitplugins_airflow-1.12.0b6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-airflow
-Version: 1.12.0b5
+Version: 1.12.0b6
 Summary: This package holds the Airflow plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-airflow-1.12.0b5/README.md` & `flytekitplugins_airflow-1.12.0b6/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-airflow-1.12.0b5/flytekitplugins/airflow/agent.py` & `flytekitplugins_airflow-1.12.0b6/flytekitplugins/airflow/agent.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-airflow-1.12.0b5/flytekitplugins/airflow/task.py` & `flytekitplugins_airflow-1.12.0b6/flytekitplugins/airflow/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-airflow-1.12.0b5/flytekitplugins_airflow.egg-info/PKG-INFO` & `flytekitplugins_airflow-1.12.0b6/flytekitplugins_airflow.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-airflow
-Version: 1.12.0b5
+Version: 1.12.0b6
 Summary: This package holds the Airflow plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-airflow-1.12.0b5/setup.py` & `flytekitplugins_airflow-1.12.0b6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 plugin_requires = [
     "apache-airflow",
     "flytekit>1.10.7",
     "flyteidl>1.10.7",
 ]
 
-__version__ = "1.12.0b5"
+__version__ = "1.12.0b6"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package holds the Airflow plugins for flytekit",
```

### Comparing `flytekitplugins-airflow-1.12.0b5/tests/test_agent.py` & `flytekitplugins_airflow-1.12.0b6/tests/test_agent.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-airflow-1.12.0b5/tests/test_task.py` & `flytekitplugins_airflow-1.12.0b6/tests/test_task.py`

 * *Files identical despite different names*

