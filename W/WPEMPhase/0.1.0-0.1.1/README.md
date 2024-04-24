# Comparing `tmp/WPEMPhase-0.1.0.tar.gz` & `tmp/WPEMPhase-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WPEMPhase-0.1.0.tar", last modified: Sun Apr 21 06:11:18 2024, max compression
+gzip compressed data, was "WPEMPhase-0.1.1.tar", last modified: Wed Apr 24 02:24:43 2024, max compression
```

## Comparing `WPEMPhase-0.1.0.tar` & `WPEMPhase-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-04-21 06:11:18.016148 WPEMPhase-0.1.0/
--rw-r--r--   0 jacob      (501) staff       (20)     1023 2024-04-21 06:11:18.015950 WPEMPhase-0.1.0/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      271 2024-01-27 12:03:25.000000 WPEMPhase-0.1.0/README.md
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-04-21 06:11:18.014078 WPEMPhase-0.1.0/WPEMPhase/
--rw-r--r--   0 jacob      (501) staff       (20)     9815 2024-04-21 06:10:33.000000 WPEMPhase-0.1.0/WPEMPhase/CPICANN.py
--rwxr-xr-x   0 jacob      (501) staff       (20)      215 2024-01-27 11:51:36.000000 WPEMPhase-0.1.0/WPEMPhase/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-04-21 06:11:18.014806 WPEMPhase-0.1.0/WPEMPhase/config/
--rw-rw-r--   0 jacob      (501) staff       (20)  1948136 2024-01-04 15:16:16.000000 WPEMPhase-0.1.0/WPEMPhase/config/strucs.csv
--rw-rw-r--   0 jacob      (501) staff       (20)     1749 2024-01-04 15:16:16.000000 WPEMPhase-0.1.0/WPEMPhase/data_format.py
--rw-rw-r--   0 jacob      (501) staff       (20)     7927 2024-01-27 11:11:48.000000 WPEMPhase-0.1.0/WPEMPhase/model.py
--rw-r--r--   0 jacob      (501) staff       (20)      954 2024-01-27 13:38:08.000000 WPEMPhase-0.1.0/WPEMPhase/plot.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-04-21 06:11:18.014686 WPEMPhase-0.1.0/WPEMPhase.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     1023 2024-04-21 06:11:17.000000 WPEMPhase-0.1.0/WPEMPhase.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      315 2024-04-21 06:11:17.000000 WPEMPhase-0.1.0/WPEMPhase.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2024-04-21 06:11:17.000000 WPEMPhase-0.1.0/WPEMPhase.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       48 2024-04-21 06:11:17.000000 WPEMPhase-0.1.0/WPEMPhase.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)       10 2024-04-21 06:11:17.000000 WPEMPhase-0.1.0/WPEMPhase.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)       38 2024-04-21 06:11:18.016191 WPEMPhase-0.1.0/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1179 2024-04-21 06:05:17.000000 WPEMPhase-0.1.0/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-04-24 02:24:43.374176 WPEMPhase-0.1.1/
+-rw-r--r--   0 jacob      (501) staff       (20)     1023 2024-04-24 02:24:43.373970 WPEMPhase-0.1.1/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      271 2024-01-27 12:03:25.000000 WPEMPhase-0.1.1/README.md
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-04-24 02:24:43.372012 WPEMPhase-0.1.1/WPEMPhase/
+-rw-r--r--   0 jacob      (501) staff       (20)     9815 2024-04-24 02:22:04.000000 WPEMPhase-0.1.1/WPEMPhase/CPICANN.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)      215 2024-01-27 11:51:36.000000 WPEMPhase-0.1.1/WPEMPhase/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-04-24 02:24:43.372732 WPEMPhase-0.1.1/WPEMPhase/config/
+-rw-rw-r--   0 jacob      (501) staff       (20)  1948136 2024-01-04 15:16:16.000000 WPEMPhase-0.1.1/WPEMPhase/config/strucs.csv
+-rw-rw-r--   0 jacob      (501) staff       (20)     1749 2024-01-04 15:16:16.000000 WPEMPhase-0.1.1/WPEMPhase/data_format.py
+-rw-rw-r--   0 jacob      (501) staff       (20)     7927 2024-01-27 11:11:48.000000 WPEMPhase-0.1.1/WPEMPhase/model.py
+-rw-r--r--   0 jacob      (501) staff       (20)      954 2024-01-27 13:38:08.000000 WPEMPhase-0.1.1/WPEMPhase/plot.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-04-24 02:24:43.372616 WPEMPhase-0.1.1/WPEMPhase.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     1023 2024-04-24 02:24:43.000000 WPEMPhase-0.1.1/WPEMPhase.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      315 2024-04-24 02:24:43.000000 WPEMPhase-0.1.1/WPEMPhase.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2024-04-24 02:24:43.000000 WPEMPhase-0.1.1/WPEMPhase.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       48 2024-04-24 02:24:43.000000 WPEMPhase-0.1.1/WPEMPhase.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       10 2024-04-24 02:24:43.000000 WPEMPhase-0.1.1/WPEMPhase.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2024-04-24 02:24:43.374218 WPEMPhase-0.1.1/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1179 2024-04-24 02:24:33.000000 WPEMPhase-0.1.1/setup.py
```

### Comparing `WPEMPhase-0.1.0/PKG-INFO` & `WPEMPhase-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WPEMPhase
-Version: 0.1.0
+Version: 0.1.1
 Summary: Crystallographic Phase Identifier of Convolutional self-Attention Neural Network
 Home-page: https://github.com/Bin-Cao/Bgolearn
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `WPEMPhase-0.1.0/WPEMPhase/CPICANN.py` & `WPEMPhase-0.1.1/WPEMPhase/CPICANN.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     extract_to_folder = pkg_resources.get_distribution('WPEMPhase').location
     loc = os.path.join(extract_to_folder, 'WPEMPhase')
     # supply CIF files
     if os.path.isdir(os.path.join(loc, 'strucs')) and os.path.isdir(os.path.join(loc, 'pretrained')):
         pass
     else:
         print("This is the first time CPICANN is being executed on your computer, configuring...")
-        file_url = "https://figshare.com/ndownloader/files/45772149"
+        file_url = "https://figshare.com/ndownloader/files/45822066"
         _dir = os.path.join(loc, 'SystemFiles.zip')
         wget.download(file_url, _dir, bar=bar_progress)
         zipfile.ZipFile(_dir).extractall(loc)
         prefix_dir = os.path.join(loc, 'SystemFiles')
         zipfile.ZipFile(os.path.join(prefix_dir, 'strucs.zip')).extractall(loc)
         zipfile.ZipFile(os.path.join(prefix_dir, 'pretrained.zip')).extractall(loc)
```

### Comparing `WPEMPhase-0.1.0/WPEMPhase/config/strucs.csv` & `WPEMPhase-0.1.1/WPEMPhase/config/strucs.csv`

 * *Files identical despite different names*

### Comparing `WPEMPhase-0.1.0/WPEMPhase/data_format.py` & `WPEMPhase-0.1.1/WPEMPhase/data_format.py`

 * *Files identical despite different names*

### Comparing `WPEMPhase-0.1.0/WPEMPhase/model.py` & `WPEMPhase-0.1.1/WPEMPhase/model.py`

 * *Files identical despite different names*

### Comparing `WPEMPhase-0.1.0/WPEMPhase/plot.py` & `WPEMPhase-0.1.1/WPEMPhase/plot.py`

 * *Files identical despite different names*

### Comparing `WPEMPhase-0.1.0/WPEMPhase.egg-info/PKG-INFO` & `WPEMPhase-0.1.1/WPEMPhase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WPEMPhase
-Version: 0.1.0
+Version: 0.1.1
 Summary: Crystallographic Phase Identifier of Convolutional self-Attention Neural Network
 Home-page: https://github.com/Bin-Cao/Bgolearn
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `WPEMPhase-0.1.0/setup.py` & `WPEMPhase-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='WPEMPhase',
-    version='0.1.0',
+    version='0.1.1',
     description="Crystallographic Phase Identifier of Convolutional self-Attention Neural Network",
     long_description=open('README.md', encoding='utf-8').read(),
     include_package_data=True,
     author='CaoBin',
     author_email='bcao@shu.edu.com',
     maintainer='CaoBin',
     maintainer_email='binjacobcao@gmail.com',
```

