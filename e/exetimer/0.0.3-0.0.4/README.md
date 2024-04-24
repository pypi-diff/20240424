# Comparing `tmp/exetimer-0.0.3.tar.gz` & `tmp/exetimer-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exetimer-0.0.3.tar", last modified: Wed Apr 24 00:34:40 2024, max compression
+gzip compressed data, was "exetimer-0.0.4.tar", last modified: Wed Apr 24 00:37:45 2024, max compression
```

## Comparing `exetimer-0.0.3.tar` & `exetimer-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ricovanderhallen   (501) staff       (20)        0 2024-04-24 00:34:40.271271 exetimer-0.0.3/
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)     1073 2024-04-24 00:11:22.000000 exetimer-0.0.3/LICENSE
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)      641 2024-04-24 00:34:40.271019 exetimer-0.0.3/PKG-INFO
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)       83 2024-04-24 00:11:15.000000 exetimer-0.0.3/README.md
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)      538 2024-04-24 00:34:23.000000 exetimer-0.0.3/pyproject.toml
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)       38 2024-04-24 00:34:40.271342 exetimer-0.0.3/setup.cfg
-drwxr-xr-x   0 ricovanderhallen   (501) staff       (20)        0 2024-04-24 00:34:40.268654 exetimer-0.0.3/src/
-drwxr-xr-x   0 ricovanderhallen   (501) staff       (20)        0 2024-04-24 00:34:40.269826 exetimer-0.0.3/src/exetimer/
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)       15 2024-04-24 00:27:54.000000 exetimer-0.0.3/src/exetimer/__init__.py
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)      218 2024-04-24 00:21:58.000000 exetimer-0.0.3/src/exetimer/exetimer.py
-drwxr-xr-x   0 ricovanderhallen   (501) staff       (20)        0 2024-04-24 00:34:40.270784 exetimer-0.0.3/src/exetimer.egg-info/
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)      641 2024-04-24 00:34:40.000000 exetimer-0.0.3/src/exetimer.egg-info/PKG-INFO
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)      226 2024-04-24 00:34:40.000000 exetimer-0.0.3/src/exetimer.egg-info/SOURCES.txt
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)        1 2024-04-24 00:34:40.000000 exetimer-0.0.3/src/exetimer.egg-info/dependency_links.txt
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)        9 2024-04-24 00:34:40.000000 exetimer-0.0.3/src/exetimer.egg-info/top_level.txt
+drwxr-xr-x   0 ricovanderhallen   (501) staff       (20)        0 2024-04-24 00:37:45.991418 exetimer-0.0.4/
+-rw-r--r--   0 ricovanderhallen   (501) staff       (20)     1073 2024-04-24 00:11:22.000000 exetimer-0.0.4/LICENSE
+-rw-r--r--   0 ricovanderhallen   (501) staff       (20)      641 2024-04-24 00:37:45.991114 exetimer-0.0.4/PKG-INFO
+-rw-r--r--   0 ricovanderhallen   (501) staff       (20)       83 2024-04-24 00:11:15.000000 exetimer-0.0.4/README.md
+-rw-r--r--   0 ricovanderhallen   (501) staff       (20)      538 2024-04-24 00:37:38.000000 exetimer-0.0.4/pyproject.toml
+-rw-r--r--   0 ricovanderhallen   (501) staff       (20)       38 2024-04-24 00:37:45.991476 exetimer-0.0.4/setup.cfg
+drwxr-xr-x   0 ricovanderhallen   (501) staff       (20)        0 2024-04-24 00:37:45.989176 exetimer-0.0.4/src/
+drwxr-xr-x   0 ricovanderhallen   (501) staff       (20)        0 2024-04-24 00:37:45.989950 exetimer-0.0.4/src/exetimer/
+-rw-r--r--   0 ricovanderhallen   (501) staff       (20)        0 2024-04-24 00:37:30.000000 exetimer-0.0.4/src/exetimer/__init__.py
+-rw-r--r--   0 ricovanderhallen   (501) staff       (20)      218 2024-04-24 00:21:58.000000 exetimer-0.0.4/src/exetimer/exetimer.py
+drwxr-xr-x   0 ricovanderhallen   (501) staff       (20)        0 2024-04-24 00:37:45.990838 exetimer-0.0.4/src/exetimer.egg-info/
+-rw-r--r--   0 ricovanderhallen   (501) staff       (20)      641 2024-04-24 00:37:45.000000 exetimer-0.0.4/src/exetimer.egg-info/PKG-INFO
+-rw-r--r--   0 ricovanderhallen   (501) staff       (20)      226 2024-04-24 00:37:45.000000 exetimer-0.0.4/src/exetimer.egg-info/SOURCES.txt
+-rw-r--r--   0 ricovanderhallen   (501) staff       (20)        1 2024-04-24 00:37:45.000000 exetimer-0.0.4/src/exetimer.egg-info/dependency_links.txt
+-rw-r--r--   0 ricovanderhallen   (501) staff       (20)        9 2024-04-24 00:37:45.000000 exetimer-0.0.4/src/exetimer.egg-info/top_level.txt
```

### Comparing `exetimer-0.0.3/LICENSE` & `exetimer-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `exetimer-0.0.3/PKG-INFO` & `exetimer-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exetimer
-Version: 0.0.3
+Version: 0.0.4
 Summary: A lightweight module that prints the execution time at the end of a python program.
 Author-email: Clevrthings <info@clevrthings.com>
 Project-URL: Homepage, https://github.com/clevrthings/exetimer
 Project-URL: Issues, https://github.com/celvrthings/exetimer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `exetimer-0.0.3/pyproject.toml` & `exetimer-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "exetimer"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Clevrthings", email="info@clevrthings.com" },
 ]
 description = "A lightweight module that prints the execution time at the end of a python program."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `exetimer-0.0.3/src/exetimer.egg-info/PKG-INFO` & `exetimer-0.0.4/src/exetimer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exetimer
-Version: 0.0.3
+Version: 0.0.4
 Summary: A lightweight module that prints the execution time at the end of a python program.
 Author-email: Clevrthings <info@clevrthings.com>
 Project-URL: Homepage, https://github.com/clevrthings/exetimer
 Project-URL: Issues, https://github.com/celvrthings/exetimer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

