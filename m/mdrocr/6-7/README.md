# Comparing `tmp/mdrocr-6.tar.gz` & `tmp/mdrocr-7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdrocr-6.tar", last modified: Thu Apr 11 16:49:42 2024, max compression
+gzip compressed data, was "mdrocr-7.tar", last modified: Wed Apr 24 16:45:45 2024, max compression
```

## Comparing `mdrocr-6.tar` & `mdrocr-7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2024-04-11 16:49:42.759487 mdrocr-6/
--rw-rw-r--   0 j         (1000) j         (1000)       30 2024-03-20 16:50:35.000000 mdrocr-6/.gitignore
--rw-rw-r--   0 j         (1000) j         (1000)      458 2024-04-11 16:49:42.759487 mdrocr-6/PKG-INFO
--rw-rw-r--   0 j         (1000) j         (1000)       89 2024-03-20 16:55:05.000000 mdrocr-6/README.md
--rwxrwxr-x   0 j         (1000) j         (1000)     2483 2024-04-11 16:49:15.000000 mdrocr-6/mdrocr
-drwxrwxr-x   0 j         (1000) j         (1000)        0 2024-04-11 16:49:42.759487 mdrocr-6/mdrocr.egg-info/
--rw-rw-r--   0 j         (1000) j         (1000)      458 2024-04-11 16:49:42.000000 mdrocr-6/mdrocr.egg-info/PKG-INFO
--rw-rw-r--   0 j         (1000) j         (1000)      167 2024-04-11 16:49:42.000000 mdrocr-6/mdrocr.egg-info/SOURCES.txt
--rw-rw-r--   0 j         (1000) j         (1000)        1 2024-04-11 16:49:42.000000 mdrocr-6/mdrocr.egg-info/dependency_links.txt
--rw-rw-r--   0 j         (1000) j         (1000)        1 2024-04-11 16:49:42.000000 mdrocr-6/mdrocr.egg-info/top_level.txt
--rwxr-xr-x   0 j         (1000) j         (1000)      291 2024-03-20 16:56:34.000000 mdrocr-6/release.sh
--rw-rw-r--   0 j         (1000) j         (1000)       38 2024-04-11 16:49:42.759487 mdrocr-6/setup.cfg
--rw-rw-r--   0 j         (1000) j         (1000)      924 2024-04-11 16:49:41.000000 mdrocr-6/setup.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2024-04-24 16:45:45.323872 mdrocr-7/
+-rw-rw-r--   0 j         (1000) j         (1000)       30 2024-03-20 16:50:35.000000 mdrocr-7/.gitignore
+-rw-rw-r--   0 j         (1000) j         (1000)      458 2024-04-24 16:45:45.323872 mdrocr-7/PKG-INFO
+-rw-rw-r--   0 j         (1000) j         (1000)       89 2024-03-20 16:55:05.000000 mdrocr-7/README.md
+-rwxrwxr-x   0 j         (1000) j         (1000)     2502 2024-04-24 16:45:04.000000 mdrocr-7/mdrocr
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2024-04-24 16:45:45.323872 mdrocr-7/mdrocr.egg-info/
+-rw-rw-r--   0 j         (1000) j         (1000)      458 2024-04-24 16:45:44.000000 mdrocr-7/mdrocr.egg-info/PKG-INFO
+-rw-rw-r--   0 j         (1000) j         (1000)      167 2024-04-24 16:45:45.000000 mdrocr-7/mdrocr.egg-info/SOURCES.txt
+-rw-rw-r--   0 j         (1000) j         (1000)        1 2024-04-24 16:45:44.000000 mdrocr-7/mdrocr.egg-info/dependency_links.txt
+-rw-rw-r--   0 j         (1000) j         (1000)        1 2024-04-24 16:45:44.000000 mdrocr-7/mdrocr.egg-info/top_level.txt
+-rwxr-xr-x   0 j         (1000) j         (1000)      291 2024-03-20 16:56:34.000000 mdrocr-7/release.sh
+-rw-rw-r--   0 j         (1000) j         (1000)       38 2024-04-24 16:45:45.323872 mdrocr-7/setup.cfg
+-rw-rw-r--   0 j         (1000) j         (1000)      924 2024-04-24 16:45:43.000000 mdrocr-7/setup.py
```

### Comparing `mdrocr-6/mdrocr` & `mdrocr-7/mdrocr`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import shutil
 import subprocess
 import sys
 import tempfile
 
 
 def sorted_list(l):
-    convert = lambda text: float(text) if text.isdigit() else text
+    convert = lambda text: float(text) if text.replace(".", "").isnumeric() else text
     alphanum = lambda key: [
         convert(c) for c in re.split(r"([-+]?[0-9]*\.?[0-9]*)", key)
     ]
     l.sort(key=alphanum)
     return l
```

### Comparing `mdrocr-6/setup.py` & `mdrocr-7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 from setuptools import setup
 
 
 def get_version():
-    return 6 #import subprocess
+    return 7 #import subprocess
     cmd = ['git', 'rev-list', 'HEAD', '--count']
     p = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     stdout, stderr = p.communicate()
     rev = int(stdout)
     return u'%s' % rev
```

