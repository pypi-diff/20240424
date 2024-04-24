# Comparing `tmp/sequrekey_pkg-0.0.1.tar.gz` & `tmp/sequrekey_pkg-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequrekey_pkg-0.0.1.tar", last modified: Sun Apr 21 14:48:44 2024, max compression
+gzip compressed data, was "sequrekey_pkg-0.0.2.tar", last modified: Wed Apr 24 15:48:07 2024, max compression
```

## Comparing `sequrekey_pkg-0.0.1.tar` & `sequrekey_pkg-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 wxh        (501) staff       (20)        0 2024-04-21 14:48:44.986266 sequrekey_pkg-0.0.1/
--rw-r--r--   0 wxh        (501) staff       (20)      270 2024-04-21 14:48:44.986046 sequrekey_pkg-0.0.1/PKG-INFO
--rw-r--r--   0 wxh        (501) staff       (20)       13 2024-04-21 14:42:59.000000 sequrekey_pkg-0.0.1/README.md
-drwxr-xr-x   0 wxh        (501) staff       (20)        0 2024-04-21 14:48:44.984951 sequrekey_pkg-0.0.1/sequrekey_pkg/
--rw-r--r--   0 wxh        (501) staff       (20)      294 2024-04-14 14:29:58.000000 sequrekey_pkg-0.0.1/sequrekey_pkg/__init__.py
--rw-r--r--   0 wxh        (501) staff       (20)      856 2024-04-14 14:29:58.000000 sequrekey_pkg-0.0.1/sequrekey_pkg/cipher.py
--rw-r--r--   0 wxh        (501) staff       (20)      871 2024-04-14 14:29:58.000000 sequrekey_pkg-0.0.1/sequrekey_pkg/dss.py
--rw-r--r--   0 wxh        (501) staff       (20)     1374 2024-04-14 14:29:58.000000 sequrekey_pkg-0.0.1/sequrekey_pkg/errors.py
--rw-r--r--   0 wxh        (501) staff       (20)      793 2024-04-14 14:29:58.000000 sequrekey_pkg-0.0.1/sequrekey_pkg/kdf.py
--rw-r--r--   0 wxh        (501) staff       (20)      724 2024-04-14 14:29:58.000000 sequrekey_pkg-0.0.1/sequrekey_pkg/kem.py
--rw-r--r--   0 wxh        (501) staff       (20)      649 2024-04-14 14:29:58.000000 sequrekey_pkg-0.0.1/sequrekey_pkg/utils.py
-drwxr-xr-x   0 wxh        (501) staff       (20)        0 2024-04-21 14:48:44.985782 sequrekey_pkg-0.0.1/sequrekey_pkg.egg-info/
--rw-r--r--   0 wxh        (501) staff       (20)      270 2024-04-21 14:48:44.000000 sequrekey_pkg-0.0.1/sequrekey_pkg.egg-info/PKG-INFO
--rw-r--r--   0 wxh        (501) staff       (20)      326 2024-04-21 14:48:44.000000 sequrekey_pkg-0.0.1/sequrekey_pkg.egg-info/SOURCES.txt
--rw-r--r--   0 wxh        (501) staff       (20)        1 2024-04-21 14:48:44.000000 sequrekey_pkg-0.0.1/sequrekey_pkg.egg-info/dependency_links.txt
--rw-r--r--   0 wxh        (501) staff       (20)       14 2024-04-21 14:48:44.000000 sequrekey_pkg-0.0.1/sequrekey_pkg.egg-info/top_level.txt
--rw-r--r--   0 wxh        (501) staff       (20)       38 2024-04-21 14:48:44.986339 sequrekey_pkg-0.0.1/setup.cfg
--rw-r--r--   0 wxh        (501) staff       (20)      455 2024-04-21 14:48:43.000000 sequrekey_pkg-0.0.1/setup.py
+drwxr-xr-x   0 wxh        (501) staff       (20)        0 2024-04-24 15:48:07.455450 sequrekey_pkg-0.0.2/
+-rw-r--r--   0 wxh        (501) staff       (20)      270 2024-04-24 15:48:07.455300 sequrekey_pkg-0.0.2/PKG-INFO
+-rw-r--r--   0 wxh        (501) staff       (20)       13 2024-04-21 14:42:59.000000 sequrekey_pkg-0.0.2/README.md
+drwxr-xr-x   0 wxh        (501) staff       (20)        0 2024-04-24 15:48:07.454527 sequrekey_pkg-0.0.2/sequrekey_pkg/
+-rw-r--r--   0 wxh        (501) staff       (20)      294 2024-04-14 14:29:58.000000 sequrekey_pkg-0.0.2/sequrekey_pkg/__init__.py
+-rw-r--r--   0 wxh        (501) staff       (20)      856 2024-04-14 14:29:58.000000 sequrekey_pkg-0.0.2/sequrekey_pkg/cipher.py
+-rw-r--r--   0 wxh        (501) staff       (20)      871 2024-04-14 14:29:58.000000 sequrekey_pkg-0.0.2/sequrekey_pkg/dss.py
+-rw-r--r--   0 wxh        (501) staff       (20)     1374 2024-04-14 14:29:58.000000 sequrekey_pkg-0.0.2/sequrekey_pkg/errors.py
+-rw-r--r--   0 wxh        (501) staff       (20)      793 2024-04-14 14:29:58.000000 sequrekey_pkg-0.0.2/sequrekey_pkg/kdf.py
+-rw-r--r--   0 wxh        (501) staff       (20)      724 2024-04-14 14:29:58.000000 sequrekey_pkg-0.0.2/sequrekey_pkg/kem.py
+-rw-r--r--   0 wxh        (501) staff       (20)      649 2024-04-14 14:29:58.000000 sequrekey_pkg-0.0.2/sequrekey_pkg/utils.py
+drwxr-xr-x   0 wxh        (501) staff       (20)        0 2024-04-24 15:48:07.455081 sequrekey_pkg-0.0.2/sequrekey_pkg.egg-info/
+-rw-r--r--   0 wxh        (501) staff       (20)      270 2024-04-24 15:48:07.000000 sequrekey_pkg-0.0.2/sequrekey_pkg.egg-info/PKG-INFO
+-rw-r--r--   0 wxh        (501) staff       (20)      326 2024-04-24 15:48:07.000000 sequrekey_pkg-0.0.2/sequrekey_pkg.egg-info/SOURCES.txt
+-rw-r--r--   0 wxh        (501) staff       (20)        1 2024-04-24 15:48:07.000000 sequrekey_pkg-0.0.2/sequrekey_pkg.egg-info/dependency_links.txt
+-rw-r--r--   0 wxh        (501) staff       (20)       14 2024-04-24 15:48:07.000000 sequrekey_pkg-0.0.2/sequrekey_pkg.egg-info/top_level.txt
+-rw-r--r--   0 wxh        (501) staff       (20)       38 2024-04-24 15:48:07.455505 sequrekey_pkg-0.0.2/setup.cfg
+-rw-r--r--   0 wxh        (501) staff       (20)      464 2024-04-24 15:48:02.000000 sequrekey_pkg-0.0.2/setup.py
```

### Comparing `sequrekey_pkg-0.0.1/sequrekey_pkg/cipher.py` & `sequrekey_pkg-0.0.2/sequrekey_pkg/cipher.py`

 * *Files identical despite different names*

### Comparing `sequrekey_pkg-0.0.1/sequrekey_pkg/dss.py` & `sequrekey_pkg-0.0.2/sequrekey_pkg/dss.py`

 * *Files identical despite different names*

### Comparing `sequrekey_pkg-0.0.1/sequrekey_pkg/errors.py` & `sequrekey_pkg-0.0.2/sequrekey_pkg/errors.py`

 * *Files identical despite different names*

### Comparing `sequrekey_pkg-0.0.1/sequrekey_pkg/kdf.py` & `sequrekey_pkg-0.0.2/sequrekey_pkg/kdf.py`

 * *Files identical despite different names*

### Comparing `sequrekey_pkg-0.0.1/sequrekey_pkg/kem.py` & `sequrekey_pkg-0.0.2/sequrekey_pkg/kem.py`

 * *Files identical despite different names*

### Comparing `sequrekey_pkg-0.0.1/sequrekey_pkg/utils.py` & `sequrekey_pkg-0.0.2/sequrekey_pkg/utils.py`

 * *Files identical despite different names*

