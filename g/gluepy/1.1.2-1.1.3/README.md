# Comparing `tmp/gluepy-1.1.2.tar.gz` & `tmp/gluepy-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gluepy-1.1.2.tar", last modified: Fri Apr  5 16:47:04 2024, max compression
+gzip compressed data, was "gluepy-1.1.3.tar", last modified: Wed Apr 24 12:48:37 2024, max compression
```

## Comparing `gluepy-1.1.2.tar` & `gluepy-1.1.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:47:04.308121 gluepy-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-05 16:46:53.000000 gluepy-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:46:53.000000 gluepy-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-05 16:47:04.304121 gluepy-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-05 16:46:53.000000 gluepy-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:47:04.300121 gluepy-1.1.2/gluepy/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:47:04.300121 gluepy-1.1.2/gluepy/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/bin/gluepy-cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:47:04.300121 gluepy-1.1.2/gluepy/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/commands/airflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/commands/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/commands/gluepy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/commands/startmodule.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/commands/startproject.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:47:04.300121 gluepy-1.1.2/gluepy/conf/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/conf/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/conf/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:47:04.304121 gluepy-1.1.2/gluepy/exec/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/exec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/exec/boot.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/exec/dags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/exec/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:47:04.304121 gluepy-1.1.2/gluepy/files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:47:04.304121 gluepy-1.1.2/gluepy/files/data/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/files/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/files/data/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/files/data/pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:47:04.304121 gluepy-1.1.2/gluepy/files/storages/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/files/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/files/storages/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/files/storages/google.py
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/files/storages/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/files/storages/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/files/storages/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:47:04.304121 gluepy-1.1.2/gluepy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/utils/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-05 16:46:53.000000 gluepy-1.1.2/gluepy/utils/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:47:04.304121 gluepy-1.1.2/gluepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-05 16:47:04.000000 gluepy-1.1.2/gluepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-05 16:47:04.000000 gluepy-1.1.2/gluepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 16:47:04.000000 gluepy-1.1.2/gluepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 16:47:04.000000 gluepy-1.1.2/gluepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-05 16:47:04.000000 gluepy-1.1.2/gluepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 16:47:04.000000 gluepy-1.1.2/gluepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 16:47:04.308121 gluepy-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-05 16:46:53.000000 gluepy-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 16:47:04.304121 gluepy-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-05 16:46:53.000000 gluepy-1.1.2/tests/test_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:48:37.639013 gluepy-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-24 12:48:27.000000 gluepy-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:48:27.000000 gluepy-1.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-24 12:48:37.639013 gluepy-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-24 12:48:27.000000 gluepy-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:48:37.631013 gluepy-1.1.3/gluepy/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:48:37.635013 gluepy-1.1.3/gluepy/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/bin/gluepy-cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:48:37.635013 gluepy-1.1.3/gluepy/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/commands/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/commands/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/commands/gluepy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/commands/startmodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/commands/startproject.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:48:37.635013 gluepy-1.1.3/gluepy/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/conf/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/conf/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:48:37.635013 gluepy-1.1.3/gluepy/exec/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/exec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/exec/boot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/exec/dags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/exec/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:48:37.635013 gluepy-1.1.3/gluepy/files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:48:37.635013 gluepy-1.1.3/gluepy/files/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/files/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/files/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/files/data/pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:48:37.639013 gluepy-1.1.3/gluepy/files/storages/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/files/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/files/storages/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/files/storages/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/files/storages/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/files/storages/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/files/storages/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:48:37.639013 gluepy-1.1.3/gluepy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-24 12:48:27.000000 gluepy-1.1.3/gluepy/utils/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:48:37.639013 gluepy-1.1.3/gluepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-24 12:48:37.000000 gluepy-1.1.3/gluepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-24 12:48:37.000000 gluepy-1.1.3/gluepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 12:48:37.000000 gluepy-1.1.3/gluepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 12:48:37.000000 gluepy-1.1.3/gluepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-24 12:48:37.000000 gluepy-1.1.3/gluepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 12:48:37.000000 gluepy-1.1.3/gluepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 12:48:37.639013 gluepy-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-24 12:48:27.000000 gluepy-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:48:37.639013 gluepy-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 12:48:27.000000 gluepy-1.1.3/tests/test_sample.py
```

### Comparing `gluepy-1.1.2/LICENSE` & `gluepy-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.2/PKG-INFO` & `gluepy-1.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gluepy
-Version: 1.1.2
+Version: 1.1.3
 Summary: A framework for data scientists
 Home-page: https://github.com/gluepy/gluepy
 Author: Marcus Lind
 Author-email: marcuslind90@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gluepy-1.1.2/gluepy/commands/airflow.py` & `gluepy-1.1.3/gluepy/commands/airflow.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.2/gluepy/commands/base.py` & `gluepy-1.1.3/gluepy/commands/base.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.2/gluepy/commands/dag.py` & `gluepy-1.1.3/gluepy/commands/dag.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.2/gluepy/commands/gluepy.py` & `gluepy-1.1.3/gluepy/commands/gluepy.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.2/gluepy/conf/context.py` & `gluepy-1.1.3/gluepy/conf/context.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.2/gluepy/exec/dags.py` & `gluepy-1.1.3/gluepy/exec/dags.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.2/gluepy/exec/tasks.py` & `gluepy-1.1.3/gluepy/exec/tasks.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.2/gluepy/files/data/pandas.py` & `gluepy-1.1.3/gluepy/files/data/pandas.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.2/gluepy/files/storages/base.py` & `gluepy-1.1.3/gluepy/files/storages/base.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.2/gluepy/files/storages/google.py` & `gluepy-1.1.3/gluepy/files/storages/google.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.2/gluepy/files/storages/local.py` & `gluepy-1.1.3/gluepy/files/storages/local.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.2/gluepy/files/storages/s3.py` & `gluepy-1.1.3/gluepy/files/storages/s3.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.2/gluepy/utils/dict.py` & `gluepy-1.1.3/gluepy/utils/dict.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.2/gluepy/utils/loading.py` & `gluepy-1.1.3/gluepy/utils/loading.py`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.2/gluepy.egg-info/PKG-INFO` & `gluepy-1.1.3/gluepy.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gluepy
-Version: 1.1.2
+Version: 1.1.3
 Summary: A framework for data scientists
 Home-page: https://github.com/gluepy/gluepy
 Author: Marcus Lind
 Author-email: marcuslind90@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gluepy-1.1.2/gluepy.egg-info/SOURCES.txt` & `gluepy-1.1.3/gluepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gluepy-1.1.2/setup.py` & `gluepy-1.1.3/setup.py`

 * *Files identical despite different names*

