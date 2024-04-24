# Comparing `tmp/coloralf-0.2.tar.gz` & `tmp/coloralf-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coloralf-0.2.tar", last modified: Wed Apr 24 13:37:51 2024, max compression
+gzip compressed data, was "coloralf-0.3.tar", last modified: Wed Apr 24 13:53:17 2024, max compression
```

## Comparing `coloralf-0.2.tar` & `coloralf-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 13:37:51.831097 coloralf-0.2/
--rw-rw-rw-   0        0        0     2836 2024-04-24 13:37:51.830082 coloralf-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2740 2024-04-24 13:37:34.000000 coloralf-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 13:37:51.818637 coloralf-0.2/coloralf/
--rw-rw-rw-   0        0        0     1232 2024-04-24 11:51:00.000000 coloralf-0.2/coloralf/Color.py
--rw-rw-rw-   0        0        0     2144 2024-04-24 12:54:00.000000 coloralf-0.2/coloralf/__init__.py
--rw-rw-rw-   0        0        0     2078 2024-04-24 12:45:21.000000 coloralf-0.2/coloralf/func.py
--rw-rw-rw-   0        0        0     1983 2024-04-24 12:45:21.000000 coloralf-0.2/coloralf/loc.py
-drwxrwxrwx   0        0        0        0 2024-04-24 13:37:51.830082 coloralf-0.2/coloralf.egg-info/
--rw-rw-rw-   0        0        0     2836 2024-04-24 13:37:51.000000 coloralf-0.2/coloralf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-04-24 13:37:51.000000 coloralf-0.2/coloralf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 13:37:51.000000 coloralf-0.2/coloralf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-24 13:37:51.000000 coloralf-0.2/coloralf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 13:37:51.831097 coloralf-0.2/setup.cfg
--rw-rw-rw-   0        0        0      273 2024-04-24 13:37:50.000000 coloralf-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:53:17.994936 coloralf-0.3/
+-rw-rw-rw-   0        0        0     2981 2024-04-24 13:53:17.994936 coloralf-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2740 2024-04-24 13:37:34.000000 coloralf-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 13:53:17.979972 coloralf-0.3/coloralf/
+-rw-rw-rw-   0        0        0     1232 2024-04-24 11:51:00.000000 coloralf-0.3/coloralf/Color.py
+-rw-rw-rw-   0        0        0     2144 2024-04-24 12:54:00.000000 coloralf-0.3/coloralf/__init__.py
+-rw-rw-rw-   0        0        0     2078 2024-04-24 12:45:21.000000 coloralf-0.3/coloralf/func.py
+-rw-rw-rw-   0        0        0     1983 2024-04-24 12:45:21.000000 coloralf-0.3/coloralf/loc.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:53:17.993920 coloralf-0.3/coloralf.egg-info/
+-rw-rw-rw-   0        0        0     2981 2024-04-24 13:53:17.000000 coloralf-0.3/coloralf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-04-24 13:53:17.000000 coloralf-0.3/coloralf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 13:53:17.000000 coloralf-0.3/coloralf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-24 13:53:17.000000 coloralf-0.3/coloralf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 13:53:17.994936 coloralf-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      431 2024-04-24 13:53:02.000000 coloralf-0.3/setup.py
```

### Comparing `coloralf-0.2/PKG-INFO` & `coloralf-0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 Metadata-Version: 2.1
 Name: coloralf
-Version: 0.2
+Version: 0.3
+Summary: Simple package to easy color & transform your console string and output
+Author: Aexeos - Angelo LF
+Author-email: aexeos413@gmail.com
 Description-Content-Type: text/markdown
 
 # coloralf
 
 ## Info :
 
 This package is all you need for transform and colored your print in the console.
```

### Comparing `coloralf-0.2/README.md` & `coloralf-0.3/README.md`

 * *Files identical despite different names*

### Comparing `coloralf-0.2/coloralf/Color.py` & `coloralf-0.3/coloralf/Color.py`

 * *Files identical despite different names*

### Comparing `coloralf-0.2/coloralf/__init__.py` & `coloralf-0.3/coloralf/__init__.py`

 * *Files identical despite different names*

### Comparing `coloralf-0.2/coloralf/func.py` & `coloralf-0.3/coloralf/func.py`

 * *Files identical despite different names*

### Comparing `coloralf-0.2/coloralf/loc.py` & `coloralf-0.3/coloralf/loc.py`

 * *Files identical despite different names*

### Comparing `coloralf-0.2/coloralf.egg-info/PKG-INFO` & `coloralf-0.3/coloralf.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 Metadata-Version: 2.1
 Name: coloralf
-Version: 0.2
+Version: 0.3
+Summary: Simple package to easy color & transform your console string and output
+Author: Aexeos - Angelo LF
+Author-email: aexeos413@gmail.com
 Description-Content-Type: text/markdown
 
 # coloralf
 
 ## Info :
 
 This package is all you need for transform and colored your print in the console.
```

