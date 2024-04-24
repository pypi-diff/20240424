# Comparing `tmp/fdamages-0.0.8.tar.gz` & `tmp/fdamages-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdamages-0.0.8.tar", last modified: Mon Apr 15 08:32:19 2024, max compression
+gzip compressed data, was "fdamages-0.0.9.tar", last modified: Mon Apr 15 08:44:20 2024, max compression
```

## Comparing `fdamages-0.0.8.tar` & `fdamages-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 08:32:19.989437 fdamages-0.0.8/
--rw-rw-rw-   0        0        0     1091 2024-04-12 09:29:34.000000 fdamages-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      469 2024-04-15 08:32:19.989437 fdamages-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       59 2024-04-12 09:29:34.000000 fdamages-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-15 08:32:19.989437 fdamages-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      852 2024-04-15 08:32:17.000000 fdamages-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 08:32:19.981689 fdamages-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2024-04-15 08:32:19.984689 fdamages-0.0.8/src/fdamages/
--rw-rw-rw-   0        0        0       88 2024-04-15 08:32:15.000000 fdamages-0.0.8/src/fdamages/__init__.py
--rw-rw-rw-   0        0        0     4750 2024-04-15 08:30:58.000000 fdamages-0.0.8/src/fdamages/module_fdamage.py
-drwxrwxrwx   0        0        0        0 2024-04-15 08:32:19.988432 fdamages-0.0.8/src/fdamages.egg-info/
--rw-rw-rw-   0        0        0      469 2024-04-15 08:32:19.000000 fdamages-0.0.8/src/fdamages.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2024-04-15 08:32:19.000000 fdamages-0.0.8/src/fdamages.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 08:32:19.000000 fdamages-0.0.8/src/fdamages.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-15 08:32:19.000000 fdamages-0.0.8/src/fdamages.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-15 08:32:19.000000 fdamages-0.0.8/src/fdamages.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 08:44:20.721533 fdamages-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2024-04-12 09:29:34.000000 fdamages-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      469 2024-04-15 08:44:20.721533 fdamages-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       59 2024-04-12 09:29:34.000000 fdamages-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-15 08:44:20.721533 fdamages-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      866 2024-04-15 08:44:18.000000 fdamages-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:44:20.712012 fdamages-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-15 08:44:20.715518 fdamages-0.0.9/src/fdamages/
+-rw-rw-rw-   0        0        0       88 2024-04-15 08:32:15.000000 fdamages-0.0.9/src/fdamages/__init__.py
+-rw-rw-rw-   0        0        0     4750 2024-04-15 08:30:58.000000 fdamages-0.0.9/src/fdamages/module_fdamage.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:44:20.720529 fdamages-0.0.9/src/fdamages.egg-info/
+-rw-rw-rw-   0        0        0      469 2024-04-15 08:44:20.000000 fdamages-0.0.9/src/fdamages.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2024-04-15 08:44:20.000000 fdamages-0.0.9/src/fdamages.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 08:44:20.000000 fdamages-0.0.9/src/fdamages.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-15 08:44:20.000000 fdamages-0.0.9/src/fdamages.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-15 08:44:20.000000 fdamages-0.0.9/src/fdamages.egg-info/top_level.txt
```

### Comparing `fdamages-0.0.8/LICENSE` & `fdamages-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fdamages-0.0.8/setup.py` & `fdamages-0.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 PACKAGE_NAME = "fdamages"
 AUTHOR = "Valerio Luzzi"
 EMAIL = "valerio.luzzi@gecosistema.com"
 GITHUB = f"https://github.com/valluzzi/{PACKAGE_NAME}.git"
 DESCRIPTION = "A fdamage utility for reading damage functions"
 
 setup(
@@ -22,23 +22,24 @@
         "": ["data/*.json"]
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    install_requires=[ "boto3" ]
+    install_requires=[ "boto3", "requests" ]
 )
 
 
 
 
 
 
 
+
```

### Comparing `fdamages-0.0.8/src/fdamages/module_fdamage.py` & `fdamages-0.0.9/src/fdamages/module_fdamage.py`

 * *Files identical despite different names*

