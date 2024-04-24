# Comparing `tmp/cli-log-0.1.tar.gz` & `tmp/cli-log-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli-log-0.1.tar", last modified: Wed Apr 24 18:50:15 2024, max compression
+gzip compressed data, was "cli-log-0.1.1.tar", last modified: Wed Apr 24 19:07:47 2024, max compression
```

## Comparing `cli-log-0.1.tar` & `cli-log-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 18:50:15.344652 cli-log-0.1/
--rw-rw-rw-   0        0        0     1105 2024-04-24 16:19:18.000000 cli-log-0.1/LICENSE
--rw-rw-rw-   0        0        0     1192 2024-04-24 18:50:15.344652 cli-log-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      574 2024-04-24 18:27:39.000000 cli-log-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 18:50:15.326390 cli-log-0.1/cli-log/
--rw-rw-rw-   0        0        0      177 2024-04-24 18:15:48.000000 cli-log-0.1/cli-log/__init__.py
--rw-rw-rw-   0        0        0     2256 2024-04-24 16:19:18.000000 cli-log-0.1/cli-log/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 18:50:15.343641 cli-log-0.1/cli_log.egg-info/
--rw-rw-rw-   0        0        0     1192 2024-04-24 18:50:15.000000 cli-log-0.1/cli_log.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2024-04-24 18:50:15.000000 cli-log-0.1/cli_log.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 18:50:15.000000 cli-log-0.1/cli_log.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-24 18:50:15.000000 cli-log-0.1/cli_log.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-24 18:50:15.000000 cli-log-0.1/cli_log.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-24 18:50:15.346018 cli-log-0.1/setup.cfg
--rw-rw-rw-   0        0        0      880 2024-04-24 18:41:32.000000 cli-log-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 19:07:47.762436 cli-log-0.1.1/
+-rw-rw-rw-   0        0        0     1105 2024-04-24 16:19:18.000000 cli-log-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1194 2024-04-24 19:07:47.762436 cli-log-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      574 2024-04-24 18:27:39.000000 cli-log-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 19:07:47.745641 cli-log-0.1.1/cli_log/
+-rw-rw-rw-   0        0        0      177 2024-04-24 18:15:48.000000 cli-log-0.1.1/cli_log/__init__.py
+-rw-rw-rw-   0        0        0     2256 2024-04-24 16:19:18.000000 cli-log-0.1.1/cli_log/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 19:07:47.760928 cli-log-0.1.1/cli_log.egg-info/
+-rw-rw-rw-   0        0        0     1194 2024-04-24 19:07:47.000000 cli-log-0.1.1/cli_log.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2024-04-24 19:07:47.000000 cli-log-0.1.1/cli_log.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 19:07:47.000000 cli-log-0.1.1/cli_log.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-24 19:07:47.000000 cli-log-0.1.1/cli_log.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-24 19:07:47.000000 cli-log-0.1.1/cli_log.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-24 19:07:47.763950 cli-log-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      882 2024-04-24 19:07:38.000000 cli-log-0.1.1/setup.py
```

### Comparing `cli-log-0.1/LICENSE` & `cli-log-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cli-log-0.1/PKG-INFO` & `cli-log-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-log
-Version: 0.1
+Version: 0.1.1
 Summary: Command line interface logging.
 Home-page: https://github.com/DeltaBotics/cli-log
 Author: DeltaBotics
 License: MIT
 Project-URL: Source, https://github.com/DeltaBotics/cli-log
 Keywords: logging,terminal logging,cli logging,terminal logger,cli logger
 Classifier: Intended Audience :: Developers
```

### Comparing `cli-log-0.1/README.md` & `cli-log-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cli-log-0.1/cli-log/core.py` & `cli-log-0.1.1/cli_log/core.py`

 * *Files identical despite different names*

### Comparing `cli-log-0.1/cli_log.egg-info/PKG-INFO` & `cli-log-0.1.1/cli_log.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-log
-Version: 0.1
+Version: 0.1.1
 Summary: Command line interface logging.
 Home-page: https://github.com/DeltaBotics/cli-log
 Author: DeltaBotics
 License: MIT
 Project-URL: Source, https://github.com/DeltaBotics/cli-log
 Keywords: logging,terminal logging,cli logging,terminal logger,cli logger
 Classifier: Intended Audience :: Developers
```

### Comparing `cli-log-0.1/setup.py` & `cli-log-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 ]
 
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
     name="cli-log",
-    packages=["cli-log"],
-    version="0.1",
+    packages=["cli_log"],
+    version="0.1.1",
     license="MIT",
     description="Command line interface logging.",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="DeltaBotics",
     url="https://github.com/DeltaBotics/cli-log",
     keywords=["logging", "terminal logging", "cli logging", "terminal logger", "cli logger"],
```

