# Comparing `tmp/dosview-0.1.5.tar.gz` & `tmp/dosview-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dosview-0.1.5.tar", last modified: Sat Apr 20 10:36:50 2024, max compression
+gzip compressed data, was "dosview-0.1.8.tar", last modified: Wed Apr 24 01:24:57 2024, max compression
```

## Comparing `dosview-0.1.5.tar` & `dosview-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:36:50.380837 dosview-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-20 10:36:50.380837 dosview-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-20 10:36:24.000000 dosview-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:36:50.380837 dosview-0.1.5/dosview/
--rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-04-20 10:36:24.000000 dosview-0.1.5/dosview/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:36:50.380837 dosview-0.1.5/dosview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-20 10:36:50.000000 dosview-0.1.5/dosview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-20 10:36:50.000000 dosview-0.1.5/dosview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 10:36:50.000000 dosview-0.1.5/dosview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-20 10:36:50.000000 dosview-0.1.5/dosview.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-20 10:36:50.000000 dosview-0.1.5/dosview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 10:36:50.000000 dosview-0.1.5/dosview.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 10:36:50.380837 dosview-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-20 10:36:24.000000 dosview-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:24:57.006067 dosview-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-24 01:24:57.002067 dosview-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-24 01:24:29.000000 dosview-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:24:57.002067 dosview-0.1.8/dosview/
+-rw-r--r--   0 runner    (1001) docker     (127)    17677 2024-04-24 01:24:29.000000 dosview-0.1.8/dosview/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:24:57.002067 dosview-0.1.8/dosview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-24 01:24:56.000000 dosview-0.1.8/dosview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-24 01:24:56.000000 dosview-0.1.8/dosview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 01:24:56.000000 dosview-0.1.8/dosview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-24 01:24:56.000000 dosview-0.1.8/dosview.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 01:24:56.000000 dosview-0.1.8/dosview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 01:24:56.000000 dosview-0.1.8/dosview.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 01:24:57.006067 dosview-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-24 01:24:29.000000 dosview-0.1.8/setup.py
```

### Comparing `dosview-0.1.5/PKG-INFO` & `dosview-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dosview
-Version: 0.1.5
+Version: 0.1.8
 Summary: A .dos file viewer
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -18,15 +18,15 @@
 Requires-Dist: pyqtgraph
 
 # Dosview
 
 ## Overview
 **Dosview** is a lightweight, efficient log viewer written in Python3, utilizing the Qt framework for its graphical interface. It is designed to facilitate quick viewing and analysis of log files directly from the command line.
 
-![obrazek](https://github.com/UniversalScientificTechnologies/dosview/assets/5196729/7279580d-4de3-4dfe-9a29-1a9149133691)
+![obrazek](doc/img/screenshot.png)
 
 
 
 ## Features
 - **Command Line Interface**: Start viewing logs with a simple command.
 - **Fast Performance**: Optimized for quick loading and smooth scrolling through large log files.
 - **Cross-Platform Compatibility**: Works on any platform that supports Python and Qt.
```

### Comparing `dosview-0.1.5/README.md` & `dosview-0.1.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Dosview
 
 ## Overview
 **Dosview** is a lightweight, efficient log viewer written in Python3, utilizing the Qt framework for its graphical interface. It is designed to facilitate quick viewing and analysis of log files directly from the command line.
 
-![obrazek](https://github.com/UniversalScientificTechnologies/dosview/assets/5196729/7279580d-4de3-4dfe-9a29-1a9149133691)
+![obrazek](doc/img/screenshot.png)
 
 
 
 ## Features
 - **Command Line Interface**: Start viewing logs with a simple command.
 - **Fast Performance**: Optimized for quick loading and smooth scrolling through large log files.
 - **Cross-Platform Compatibility**: Works on any platform that supports Python and Qt.
```

### Comparing `dosview-0.1.5/dosview.egg-info/PKG-INFO` & `dosview-0.1.8/dosview.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dosview
-Version: 0.1.5
+Version: 0.1.8
 Summary: A .dos file viewer
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -18,15 +18,15 @@
 Requires-Dist: pyqtgraph
 
 # Dosview
 
 ## Overview
 **Dosview** is a lightweight, efficient log viewer written in Python3, utilizing the Qt framework for its graphical interface. It is designed to facilitate quick viewing and analysis of log files directly from the command line.
 
-![obrazek](https://github.com/UniversalScientificTechnologies/dosview/assets/5196729/7279580d-4de3-4dfe-9a29-1a9149133691)
+![obrazek](doc/img/screenshot.png)
 
 
 
 ## Features
 - **Command Line Interface**: Start viewing logs with a simple command.
 - **Fast Performance**: Optimized for quick loading and smooth scrolling through large log files.
 - **Cross-Platform Compatibility**: Works on any platform that supports Python and Qt.
```

### Comparing `dosview-0.1.5/setup.py` & `dosview-0.1.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from shutil import copyfile
 import os
+import subprocess
 
 # Read requirements.txt
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 # Read README.md for the long description
 with open('README.md', 'r', encoding='utf-8') as f:
@@ -22,17 +23,20 @@
             os.makedirs('/usr/local/share/applications')
         copyfile('dosview.desktop', '/usr/local/share/applications/dosview.desktop')
         
         if not os.path.exists('/usr/local/share/icons'):
             os.makedirs('/usr/local/share/icons')
         copyfile('media/icon_ust.png', '/usr/local/share/icons/icon_ust.png')
 
+# Get the commit hash
+#commit_hash = subprocess.check_output(['git', 'rev-parse', 'HEAD']).decode().strip()
+
 setup(
     name='dosview',
-    version='0.1.5',
+    version=f'0.1.8',
     description='A .dos file viewer', 
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'dosview = dosview:main',
```

