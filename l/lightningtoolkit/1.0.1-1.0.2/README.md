# Comparing `tmp/lightningtoolkit-1.0.1.tar.gz` & `tmp/lightningtoolkit-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightningtoolkit-1.0.1.tar", last modified: Sun Apr 21 09:37:16 2024, max compression
+gzip compressed data, was "lightningtoolkit-1.0.2.tar", last modified: Wed Apr 24 12:34:53 2024, max compression
```

## Comparing `lightningtoolkit-1.0.1.tar` & `lightningtoolkit-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-21 09:37:16.002533 lightningtoolkit-1.0.1/
--rw-rw-r--   0 gqx       (1000) gqx       (1000)     1070 2024-04-20 12:35:42.000000 lightningtoolkit-1.0.1/LICENSE
--rw-r--r--   0 gqx       (1000) gqx       (1000)     1909 2024-04-21 09:37:16.002533 lightningtoolkit-1.0.1/PKG-INFO
--rwx------   0 gqx       (1000) gqx       (1000)      697 2024-04-20 13:21:44.000000 lightningtoolkit-1.0.1/README.md
-drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-21 09:37:16.002533 lightningtoolkit-1.0.1/lightningtoolkit.egg-info/
--rw-r--r--   0 gqx       (1000) gqx       (1000)     1909 2024-04-21 09:37:15.000000 lightningtoolkit-1.0.1/lightningtoolkit.egg-info/PKG-INFO
--rw-rw-r--   0 gqx       (1000) gqx       (1000)      186 2024-04-21 09:37:15.000000 lightningtoolkit-1.0.1/lightningtoolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 gqx       (1000) gqx       (1000)        1 2024-04-21 09:37:15.000000 lightningtoolkit-1.0.1/lightningtoolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 gqx       (1000) gqx       (1000)        1 2024-04-21 09:37:15.000000 lightningtoolkit-1.0.1/lightningtoolkit.egg-info/top_level.txt
--rw-rw-r--   0 gqx       (1000) gqx       (1000)       38 2024-04-21 09:37:16.002533 lightningtoolkit-1.0.1/setup.cfg
--rw-rw-r--   0 gqx       (1000) gqx       (1000)     1424 2024-04-21 09:36:25.000000 lightningtoolkit-1.0.1/setup.py
+drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-24 12:34:53.821962 lightningtoolkit-1.0.2/
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)     1070 2024-04-21 10:28:28.000000 lightningtoolkit-1.0.2/LICENSE
+-rw-r--r--   0 gqx       (1000) gqx       (1000)     3462 2024-04-24 12:34:53.821962 lightningtoolkit-1.0.2/PKG-INFO
+-rwx------   0 gqx       (1000) gqx       (1000)     2210 2024-04-24 12:07:15.000000 lightningtoolkit-1.0.2/README.md
+drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-24 12:34:53.821962 lightningtoolkit-1.0.2/lightningtoolkit/
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)       32 2024-04-24 12:13:50.000000 lightningtoolkit-1.0.2/lightningtoolkit/__init__.py
+-rwx------   0 gqx       (1000) gqx       (1000)     9067 2024-04-24 12:00:03.000000 lightningtoolkit-1.0.2/lightningtoolkit/run.py
+drwxrwxr-x   0 gqx       (1000) gqx       (1000)        0 2024-04-24 12:34:53.821962 lightningtoolkit-1.0.2/lightningtoolkit.egg-info/
+-rw-r--r--   0 gqx       (1000) gqx       (1000)     3462 2024-04-24 12:34:53.000000 lightningtoolkit-1.0.2/lightningtoolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)      239 2024-04-24 12:34:53.000000 lightningtoolkit-1.0.2/lightningtoolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)        1 2024-04-24 12:34:53.000000 lightningtoolkit-1.0.2/lightningtoolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)       17 2024-04-24 12:34:53.000000 lightningtoolkit-1.0.2/lightningtoolkit.egg-info/top_level.txt
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)       38 2024-04-24 12:34:53.821962 lightningtoolkit-1.0.2/setup.cfg
+-rw-rw-r--   0 gqx       (1000) gqx       (1000)     1353 2024-04-24 12:34:30.000000 lightningtoolkit-1.0.2/setup.py
```

### Comparing `lightningtoolkit-1.0.1/LICENSE` & `lightningtoolkit-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lightningtoolkit-1.0.1/setup.py` & `lightningtoolkit-1.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 from setuptools import setup,find_packages
 with open("README.md", "r", encoding="utf-8") as fh:
     description = fh.read()
 setup(
-    name = "lightningtoolkit",
-    version = "1.0.1",
-    author = "GQX",
-    author_email = "kill114514251@outlook.com",
-    packages = find_packages(),
-    description = "A toolkit that combines many functions",
-    long_description = description,
-    url = "https://github.com/BinaryGuo/Lightning_Toolkit",
-    classifiers = [
-        "Intended Audience :: End Users/Desktop",
-        "Development Status :: 5 - Production/Stable",
-        "Natural Language :: English",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.13",
-        "Programming Language :: Python :: 3.12",
-        "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.4",
-        "Programming Language :: Python :: 3.3",
-        "Programming Language :: Python :: 3.2",
-        "Programming Language :: Python :: 3.1",
-        "Programming Language :: Python :: 3"
-    ],
-    python_requires=">=3.0"
+name = "lightningtoolkit",
+version = "1.0.2",
+author = "GQX",
+author_email = "kill114514251@outlook.com",
+packages = find_packages(),
+description = "A toolkit that combines many functions",
+long_description_content_type = "text/markdown",
+long_description = description,
+url = "https://github.com/BinaryGuo/Lightning_Toolkit",
+classifiers = [
+    "Intended Audience :: End Users/Desktop",
+    "Development Status :: 5 - Production/Stable",
+    "Natural Language :: English",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3.13",
+    "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.6",
+    "Programming Language :: Python :: 3.5",
+    "Programming Language :: Python :: 3.4",
+    "Programming Language :: Python :: 3.3",
+    "Programming Language :: Python :: 3.2",
+    "Programming Language :: Python :: 3.1",
+    "Programming Language :: Python :: 3"
+],
+python_requires=">=3.0"
 )
```

