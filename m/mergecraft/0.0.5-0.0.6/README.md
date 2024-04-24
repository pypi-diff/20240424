# Comparing `tmp/mergecraft-0.0.5.tar.gz` & `tmp/mergecraft-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mergecraft-0.0.5.tar", last modified: Wed Apr 24 10:06:15 2024, max compression
+gzip compressed data, was "mergecraft-0.0.6.tar", last modified: Wed Apr 24 10:12:25 2024, max compression
```

## Comparing `mergecraft-0.0.5.tar` & `mergecraft-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:06:15.279684 mergecraft-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-24 10:06:03.000000 mergecraft-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-24 10:06:15.279684 mergecraft-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-24 10:06:03.000000 mergecraft-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:06:15.279684 mergecraft-0.0.5/mergecraft/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:06:03.000000 mergecraft-0.0.5/mergecraft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-04-24 10:06:03.000000 mergecraft-0.0.5/mergecraft/mergecraft.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:06:15.279684 mergecraft-0.0.5/mergecraft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-24 10:06:15.000000 mergecraft-0.0.5/mergecraft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-24 10:06:15.000000 mergecraft-0.0.5/mergecraft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:06:15.000000 mergecraft-0.0.5/mergecraft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 10:06:15.000000 mergecraft-0.0.5/mergecraft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 10:06:15.000000 mergecraft-0.0.5/mergecraft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 10:06:15.000000 mergecraft-0.0.5/mergecraft.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 10:06:15.279684 mergecraft-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-24 10:06:03.000000 mergecraft-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:12:25.077340 mergecraft-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-24 10:12:15.000000 mergecraft-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-24 10:12:25.077340 mergecraft-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-24 10:12:15.000000 mergecraft-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:12:25.077340 mergecraft-0.0.6/mergecraft/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:12:15.000000 mergecraft-0.0.6/mergecraft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-04-24 10:12:15.000000 mergecraft-0.0.6/mergecraft/mergecraft.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:12:25.077340 mergecraft-0.0.6/mergecraft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-24 10:12:25.000000 mergecraft-0.0.6/mergecraft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-24 10:12:25.000000 mergecraft-0.0.6/mergecraft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:12:25.000000 mergecraft-0.0.6/mergecraft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 10:12:25.000000 mergecraft-0.0.6/mergecraft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 10:12:25.000000 mergecraft-0.0.6/mergecraft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 10:12:25.000000 mergecraft-0.0.6/mergecraft.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 10:12:25.077340 mergecraft-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-24 10:12:15.000000 mergecraft-0.0.6/setup.py
```

### Comparing `mergecraft-0.0.5/LICENSE` & `mergecraft-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mergecraft-0.0.5/PKG-INFO` & `mergecraft-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mergecraft
-Version: 0.0.5
+Version: 0.0.6
 Summary: A command-line tool to merge files into a temporary file and open in VS Code. Designed to support AI-driven development.
 Home-page: https://github.com/josenerydev/mergecraft
 Author: José Nery
 Author-email: josenerydev@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -42,14 +42,22 @@
 
 To set up the `mergecraft` tool, you can now install it directly from PyPI:
 
 ```bash
 pip install mergecraft
 ```
 
+### ⬆️ Upgrading mergecraft
+
+To upgrade to the latest version of `mergecraft`, you can use the following command:
+
+```bash
+pip install --upgrade mergecraft
+```
+
 ### 📦 Install Locally
 
 Alternatively, if you need to install from the source for the latest features or development purposes:
 
 ```bash
 # Clone the repository
 git clone https://github.com/your-username/mergecraft.git
```

### Comparing `mergecraft-0.0.5/README.md` & `mergecraft-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,22 @@
 
 To set up the `mergecraft` tool, you can now install it directly from PyPI:
 
 ```bash
 pip install mergecraft
 ```
 
+### ⬆️ Upgrading mergecraft
+
+To upgrade to the latest version of `mergecraft`, you can use the following command:
+
+```bash
+pip install --upgrade mergecraft
+```
+
 ### 📦 Install Locally
 
 Alternatively, if you need to install from the source for the latest features or development purposes:
 
 ```bash
 # Clone the repository
 git clone https://github.com/your-username/mergecraft.git
```

### Comparing `mergecraft-0.0.5/mergecraft/mergecraft.py` & `mergecraft-0.0.6/mergecraft/mergecraft.py`

 * *Files identical despite different names*

### Comparing `mergecraft-0.0.5/mergecraft.egg-info/PKG-INFO` & `mergecraft-0.0.6/mergecraft.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mergecraft
-Version: 0.0.5
+Version: 0.0.6
 Summary: A command-line tool to merge files into a temporary file and open in VS Code. Designed to support AI-driven development.
 Home-page: https://github.com/josenerydev/mergecraft
 Author: José Nery
 Author-email: josenerydev@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -42,14 +42,22 @@
 
 To set up the `mergecraft` tool, you can now install it directly from PyPI:
 
 ```bash
 pip install mergecraft
 ```
 
+### ⬆️ Upgrading mergecraft
+
+To upgrade to the latest version of `mergecraft`, you can use the following command:
+
+```bash
+pip install --upgrade mergecraft
+```
+
 ### 📦 Install Locally
 
 Alternatively, if you need to install from the source for the latest features or development purposes:
 
 ```bash
 # Clone the repository
 git clone https://github.com/your-username/mergecraft.git
```

### Comparing `mergecraft-0.0.5/setup.py` & `mergecraft-0.0.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="mergecraft",
-    version="0.0.5",
+    version="0.0.6",
     description="A command-line tool to merge files into a temporary file and open in VS Code. Designed to support AI-driven development.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="José Nery",
     author_email="josenerydev@gmail.com",
     url="https://github.com/josenerydev/mergecraft",
     packages=find_packages(),
```

