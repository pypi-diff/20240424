# Comparing `tmp/cli-log-0.1.4.tar.gz` & `tmp/cli-log-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli-log-0.1.4.tar", last modified: Wed Apr 24 19:49:36 2024, max compression
+gzip compressed data, was "cli-log-0.1.6.tar", last modified: Wed Apr 24 20:07:43 2024, max compression
```

## Comparing `cli-log-0.1.4.tar` & `cli-log-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 19:49:36.599084 cli-log-0.1.4/
--rw-rw-rw-   0        0        0     1105 2024-04-24 16:19:18.000000 cli-log-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     1138 2024-04-24 19:49:36.599084 cli-log-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      574 2024-04-24 18:27:39.000000 cli-log-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 19:49:36.588564 cli-log-0.1.4/cli/
--rw-rw-rw-   0        0        0      256 2024-04-24 19:48:15.000000 cli-log-0.1.4/cli/__init__.py
--rw-rw-rw-   0        0        0     2256 2024-04-24 19:46:42.000000 cli-log-0.1.4/cli/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 19:49:36.598083 cli-log-0.1.4/cli_log.egg-info/
--rw-rw-rw-   0        0        0     1138 2024-04-24 19:49:36.000000 cli-log-0.1.4/cli_log.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-04-24 19:49:36.000000 cli-log-0.1.4/cli_log.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 19:49:36.000000 cli-log-0.1.4/cli_log.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-24 19:49:36.000000 cli-log-0.1.4/cli_log.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-24 19:49:36.000000 cli-log-0.1.4/cli_log.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-24 19:49:36.600081 cli-log-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      810 2024-04-24 19:49:26.000000 cli-log-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 20:07:43.531525 cli-log-0.1.6/
+-rw-rw-rw-   0        0        0     1105 2024-04-24 16:19:18.000000 cli-log-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     1138 2024-04-24 20:07:43.531525 cli-log-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      574 2024-04-24 18:27:39.000000 cli-log-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 20:07:43.517593 cli-log-0.1.6/cli/
+-rw-rw-rw-   0        0        0      177 2024-04-24 19:59:30.000000 cli-log-0.1.6/cli/__init__.py
+-rw-rw-rw-   0        0        0     2256 2024-04-24 19:46:42.000000 cli-log-0.1.6/cli/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 20:07:43.518599 cli-log-0.1.6/cli/utils/
+-rw-rw-rw-   0        0        0       84 2024-04-24 19:46:56.000000 cli-log-0.1.6/cli/utils/__init__.py
+-rw-rw-rw-   0        0        0      319 2024-04-24 19:46:49.000000 cli-log-0.1.6/cli/utils/time_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 20:07:43.530135 cli-log-0.1.6/cli_log.egg-info/
+-rw-rw-rw-   0        0        0     1138 2024-04-24 20:07:43.000000 cli-log-0.1.6/cli_log.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2024-04-24 20:07:43.000000 cli-log-0.1.6/cli_log.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 20:07:43.000000 cli-log-0.1.6/cli_log.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-24 20:07:43.000000 cli-log-0.1.6/cli_log.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-24 20:07:43.000000 cli-log-0.1.6/cli_log.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-24 20:07:43.533578 cli-log-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      833 2024-04-24 20:07:28.000000 cli-log-0.1.6/setup.py
```

### Comparing `cli-log-0.1.4/LICENSE` & `cli-log-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cli-log-0.1.4/PKG-INFO` & `cli-log-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-log
-Version: 0.1.4
+Version: 0.1.6
 Summary: Command line interface logging.
 Home-page: https://github.com/DeltaBotics/cli-log
 Author: DeltaBotics
 License: MIT
 Project-URL: Source, https://github.com/DeltaBotics/cli-log
 Keywords: logging
 Classifier: Intended Audience :: Developers
```

### Comparing `cli-log-0.1.4/README.md` & `cli-log-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `cli-log-0.1.4/cli/core.py` & `cli-log-0.1.6/cli/core.py`

 * *Files identical despite different names*

### Comparing `cli-log-0.1.4/cli_log.egg-info/PKG-INFO` & `cli-log-0.1.6/cli_log.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-log
-Version: 0.1.4
+Version: 0.1.6
 Summary: Command line interface logging.
 Home-page: https://github.com/DeltaBotics/cli-log
 Author: DeltaBotics
 License: MIT
 Project-URL: Source, https://github.com/DeltaBotics/cli-log
 Keywords: logging
 Classifier: Intended Audience :: Developers
```

### Comparing `cli-log-0.1.4/setup.py` & `cli-log-0.1.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 classifiers = [
     "Intended Audience :: Developers",
     "Topic :: System :: Logging",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
 ]
 
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
     name="cli-log",
-    packages=["cli"],
-    version="0.1.4",
+    packages=find_packages(),
+    version="0.1.6",
     license="MIT",
     description="Command line interface logging.",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="DeltaBotics",
     url="https://github.com/DeltaBotics/cli-log",
     keywords=["logging"],
```

