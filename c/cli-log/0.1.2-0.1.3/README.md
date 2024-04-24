# Comparing `tmp/cli-log-0.1.2.tar.gz` & `tmp/cli-log-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli-log-0.1.2.tar", last modified: Wed Apr 24 19:15:03 2024, max compression
+gzip compressed data, was "cli-log-0.1.3.tar", last modified: Wed Apr 24 19:22:37 2024, max compression
```

## Comparing `cli-log-0.1.2.tar` & `cli-log-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 19:15:03.755070 cli-log-0.1.2/
--rw-rw-rw-   0        0        0     1105 2024-04-24 16:19:18.000000 cli-log-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     1138 2024-04-24 19:15:03.755070 cli-log-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      574 2024-04-24 18:27:39.000000 cli-log-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 19:15:03.740429 cli-log-0.1.2/cli/
--rw-rw-rw-   0        0        0      177 2024-04-24 18:15:48.000000 cli-log-0.1.2/cli/__init__.py
--rw-rw-rw-   0        0        0     2256 2024-04-24 19:14:50.000000 cli-log-0.1.2/cli/core.py
-drwxrwxrwx   0        0        0        0 2024-04-24 19:15:03.753822 cli-log-0.1.2/cli_log.egg-info/
--rw-rw-rw-   0        0        0     1138 2024-04-24 19:15:03.000000 cli-log-0.1.2/cli_log.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-04-24 19:15:03.000000 cli-log-0.1.2/cli_log.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 19:15:03.000000 cli-log-0.1.2/cli_log.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-24 19:15:03.000000 cli-log-0.1.2/cli_log.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-24 19:15:03.000000 cli-log-0.1.2/cli_log.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-24 19:15:03.755574 cli-log-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      810 2024-04-24 19:14:52.000000 cli-log-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 19:22:37.972974 cli-log-0.1.3/
+-rw-rw-rw-   0        0        0     1105 2024-04-24 16:19:18.000000 cli-log-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1138 2024-04-24 19:22:37.972974 cli-log-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      574 2024-04-24 18:27:39.000000 cli-log-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 19:22:37.962016 cli-log-0.1.3/cli/
+-rw-rw-rw-   0        0        0      177 2024-04-24 18:15:48.000000 cli-log-0.1.3/cli/__init__.py
+-rw-rw-rw-   0        0        0     2256 2024-04-24 19:14:50.000000 cli-log-0.1.3/cli/core.py
+drwxrwxrwx   0        0        0        0 2024-04-24 19:22:37.971809 cli-log-0.1.3/cli_log.egg-info/
+-rw-rw-rw-   0        0        0     1138 2024-04-24 19:22:37.000000 cli-log-0.1.3/cli_log.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-04-24 19:22:37.000000 cli-log-0.1.3/cli_log.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 19:22:37.000000 cli-log-0.1.3/cli_log.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-24 19:22:37.000000 cli-log-0.1.3/cli_log.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-24 19:22:37.000000 cli-log-0.1.3/cli_log.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-24 19:22:37.974488 cli-log-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      810 2024-04-24 19:22:22.000000 cli-log-0.1.3/setup.py
```

### Comparing `cli-log-0.1.2/LICENSE` & `cli-log-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cli-log-0.1.2/PKG-INFO` & `cli-log-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-log
-Version: 0.1.2
+Version: 0.1.3
 Summary: Command line interface logging.
 Home-page: https://github.com/DeltaBotics/cli-log
 Author: DeltaBotics
 License: MIT
 Project-URL: Source, https://github.com/DeltaBotics/cli-log
 Keywords: logging
 Classifier: Intended Audience :: Developers
```

### Comparing `cli-log-0.1.2/README.md` & `cli-log-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cli-log-0.1.2/cli/core.py` & `cli-log-0.1.3/cli/core.py`

 * *Files identical despite different names*

### Comparing `cli-log-0.1.2/cli_log.egg-info/PKG-INFO` & `cli-log-0.1.3/cli_log.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-log
-Version: 0.1.2
+Version: 0.1.3
 Summary: Command line interface logging.
 Home-page: https://github.com/DeltaBotics/cli-log
 Author: DeltaBotics
 License: MIT
 Project-URL: Source, https://github.com/DeltaBotics/cli-log
 Keywords: logging
 Classifier: Intended Audience :: Developers
```

### Comparing `cli-log-0.1.2/setup.py` & `cli-log-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
     name="cli-log",
     packages=["cli"],
-    version="0.1.2",
+    version="0.1.3",
     license="MIT",
     description="Command line interface logging.",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="DeltaBotics",
     url="https://github.com/DeltaBotics/cli-log",
     keywords=["logging"],
```

