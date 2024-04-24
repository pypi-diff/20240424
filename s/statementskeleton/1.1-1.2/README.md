# Comparing `tmp/statementskeleton-1.1.tar.gz` & `tmp/statementskeleton-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statementskeleton-1.1.tar", last modified: Wed Apr 24 02:22:15 2024, max compression
+gzip compressed data, was "statementskeleton-1.2.tar", last modified: Wed Apr 24 02:38:36 2024, max compression
```

## Comparing `statementskeleton-1.1.tar` & `statementskeleton-1.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 02:22:15.950202 statementskeleton-1.1/
--rw-rw-rw-   0        0        0    35823 2024-04-24 02:12:24.000000 statementskeleton-1.1/LICENSE
--rw-rw-rw-   0        0        0     3597 2024-04-24 02:22:15.949202 statementskeleton-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2972 2024-04-24 02:21:46.000000 statementskeleton-1.1/README.md
--rw-rw-rw-   0        0        0      716 2024-04-24 02:22:01.000000 statementskeleton-1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-24 02:22:15.950703 statementskeleton-1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-24 02:22:15.925081 statementskeleton-1.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-24 02:22:15.931102 statementskeleton-1.1/src/statementskeleton/
--rw-rw-rw-   0        0        0       51 2024-04-24 02:05:03.000000 statementskeleton-1.1/src/statementskeleton/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 02:22:15.944182 statementskeleton-1.1/src/statementskeleton/elements/
--rw-rw-rw-   0        0        0     1325 2024-04-24 02:05:03.000000 statementskeleton-1.1/src/statementskeleton/elements/Account.py
--rw-rw-rw-   0        0        0      692 2024-04-24 02:05:03.000000 statementskeleton-1.1/src/statementskeleton/elements/Divider.py
--rw-rw-rw-   0        0        0      453 2024-04-24 02:05:03.000000 statementskeleton-1.1/src/statementskeleton/elements/Element.py
--rw-rw-rw-   0        0        0     1918 2024-04-24 02:05:03.000000 statementskeleton-1.1/src/statementskeleton/elements/Header.py
--rw-rw-rw-   0        0        0      504 2024-04-24 02:05:03.000000 statementskeleton-1.1/src/statementskeleton/elements/Spacer.py
--rw-rw-rw-   0        0        0      807 2024-04-24 02:05:03.000000 statementskeleton-1.1/src/statementskeleton/elements/Subtotal.py
--rw-rw-rw-   0        0        0      669 2024-04-24 02:05:03.000000 statementskeleton-1.1/src/statementskeleton/elements/Title.py
--rw-rw-rw-   0        0        0     1057 2024-04-24 02:05:03.000000 statementskeleton-1.1/src/statementskeleton/elements/Total.py
--rw-rw-rw-   0        0        0      187 2024-04-24 02:05:03.000000 statementskeleton-1.1/src/statementskeleton/elements/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 02:22:15.945680 statementskeleton-1.1/src/statementskeleton/skeletons/
--rw-rw-rw-   0        0        0     9273 2024-04-24 02:21:46.000000 statementskeleton-1.1/src/statementskeleton/skeletons/Skeleton.py
--rw-rw-rw-   0        0        0       25 2024-04-24 02:05:03.000000 statementskeleton-1.1/src/statementskeleton/skeletons/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 02:22:15.948197 statementskeleton-1.1/src/statementskeleton.egg-info/
--rw-rw-rw-   0        0        0     3597 2024-04-24 02:22:15.000000 statementskeleton-1.1/src/statementskeleton.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      731 2024-04-24 02:22:15.000000 statementskeleton-1.1/src/statementskeleton.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 02:22:15.000000 statementskeleton-1.1/src/statementskeleton.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-24 02:22:15.000000 statementskeleton-1.1/src/statementskeleton.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-24 02:22:15.946684 statementskeleton-1.1/tests/
--rw-rw-rw-   0        0        0     1121 2024-04-24 02:21:46.000000 statementskeleton-1.1/tests/test_Skeleton.py
+drwxrwxrwx   0        0        0        0 2024-04-24 02:38:36.787866 statementskeleton-1.2/
+-rw-rw-rw-   0        0        0    35823 2024-04-24 02:12:24.000000 statementskeleton-1.2/LICENSE
+-rw-rw-rw-   0        0        0     3597 2024-04-24 02:38:36.786866 statementskeleton-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2972 2024-04-24 02:21:46.000000 statementskeleton-1.2/README.md
+-rw-rw-rw-   0        0        0      716 2024-04-24 02:38:05.000000 statementskeleton-1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-24 02:38:36.787866 statementskeleton-1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-24 02:38:36.766433 statementskeleton-1.2/src/
+-rw-rw-rw-   0        0        0       33 2024-04-24 02:38:05.000000 statementskeleton-1.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 02:38:36.766933 statementskeleton-1.2/src/statementskeleton/
+-rw-rw-rw-   0        0        0       51 2024-04-24 02:05:03.000000 statementskeleton-1.2/src/statementskeleton/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 02:38:36.782358 statementskeleton-1.2/src/statementskeleton/elements/
+-rw-rw-rw-   0        0        0     1325 2024-04-24 02:05:03.000000 statementskeleton-1.2/src/statementskeleton/elements/Account.py
+-rw-rw-rw-   0        0        0      692 2024-04-24 02:05:03.000000 statementskeleton-1.2/src/statementskeleton/elements/Divider.py
+-rw-rw-rw-   0        0        0      453 2024-04-24 02:05:03.000000 statementskeleton-1.2/src/statementskeleton/elements/Element.py
+-rw-rw-rw-   0        0        0     1918 2024-04-24 02:05:03.000000 statementskeleton-1.2/src/statementskeleton/elements/Header.py
+-rw-rw-rw-   0        0        0      504 2024-04-24 02:05:03.000000 statementskeleton-1.2/src/statementskeleton/elements/Spacer.py
+-rw-rw-rw-   0        0        0      807 2024-04-24 02:05:03.000000 statementskeleton-1.2/src/statementskeleton/elements/Subtotal.py
+-rw-rw-rw-   0        0        0      669 2024-04-24 02:05:03.000000 statementskeleton-1.2/src/statementskeleton/elements/Title.py
+-rw-rw-rw-   0        0        0     1057 2024-04-24 02:05:03.000000 statementskeleton-1.2/src/statementskeleton/elements/Total.py
+-rw-rw-rw-   0        0        0      187 2024-04-24 02:05:03.000000 statementskeleton-1.2/src/statementskeleton/elements/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 02:38:36.783861 statementskeleton-1.2/src/statementskeleton/skeletons/
+-rw-rw-rw-   0        0        0     9273 2024-04-24 02:21:46.000000 statementskeleton-1.2/src/statementskeleton/skeletons/Skeleton.py
+-rw-rw-rw-   0        0        0       25 2024-04-24 02:05:03.000000 statementskeleton-1.2/src/statementskeleton/skeletons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 02:38:36.786367 statementskeleton-1.2/src/statementskeleton.egg-info/
+-rw-rw-rw-   0        0        0     3597 2024-04-24 02:38:36.000000 statementskeleton-1.2/src/statementskeleton.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      747 2024-04-24 02:38:36.000000 statementskeleton-1.2/src/statementskeleton.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 02:38:36.000000 statementskeleton-1.2/src/statementskeleton.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-24 02:38:36.000000 statementskeleton-1.2/src/statementskeleton.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 02:38:36.784869 statementskeleton-1.2/tests/
+-rw-rw-rw-   0        0        0     1121 2024-04-24 02:21:46.000000 statementskeleton-1.2/tests/test_Skeleton.py
```

### Comparing `statementskeleton-1.1/LICENSE` & `statementskeleton-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `statementskeleton-1.1/PKG-INFO` & `statementskeleton-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statementskeleton
-Version: 1.1
+Version: 1.2
 Summary: A package for formatting financial statements in the console. Designed for PyActy.
 Author-email: Jacob Zufall <jacobzufall@gmail.com>
 Project-URL: Homepage, https://github.com/JacobZufall/statementskeleton
 Project-URL: Issues, https://github.com/JacobZufall/statementskeleton/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```

### Comparing `statementskeleton-1.1/README.md` & `statementskeleton-1.2/README.md`

 * *Files identical despite different names*

### Comparing `statementskeleton-1.1/pyproject.toml` & `statementskeleton-1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "statementskeleton"
-version = "1.1"
+version = "1.2"
 authors = [
     {name="Jacob Zufall", email="jacobzufall@gmail.com"}
 ]
 description = "A package for formatting financial statements in the console. Designed for PyActy."
 readme = "README.md"
 requires-python= ">3.11"
 dependencies = []
```

### Comparing `statementskeleton-1.1/src/statementskeleton/elements/Account.py` & `statementskeleton-1.2/src/statementskeleton/elements/Account.py`

 * *Files identical despite different names*

### Comparing `statementskeleton-1.1/src/statementskeleton/elements/Divider.py` & `statementskeleton-1.2/src/statementskeleton/elements/Divider.py`

 * *Files identical despite different names*

### Comparing `statementskeleton-1.1/src/statementskeleton/elements/Header.py` & `statementskeleton-1.2/src/statementskeleton/elements/Header.py`

 * *Files identical despite different names*

### Comparing `statementskeleton-1.1/src/statementskeleton/elements/Subtotal.py` & `statementskeleton-1.2/src/statementskeleton/elements/Subtotal.py`

 * *Files identical despite different names*

### Comparing `statementskeleton-1.1/src/statementskeleton/elements/Title.py` & `statementskeleton-1.2/src/statementskeleton/elements/Title.py`

 * *Files identical despite different names*

### Comparing `statementskeleton-1.1/src/statementskeleton/elements/Total.py` & `statementskeleton-1.2/src/statementskeleton/elements/Total.py`

 * *Files identical despite different names*

### Comparing `statementskeleton-1.1/src/statementskeleton/skeletons/Skeleton.py` & `statementskeleton-1.2/src/statementskeleton/skeletons/Skeleton.py`

 * *Files identical despite different names*

### Comparing `statementskeleton-1.1/src/statementskeleton.egg-info/PKG-INFO` & `statementskeleton-1.2/src/statementskeleton.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statementskeleton
-Version: 1.1
+Version: 1.2
 Summary: A package for formatting financial statements in the console. Designed for PyActy.
 Author-email: Jacob Zufall <jacobzufall@gmail.com>
 Project-URL: Homepage, https://github.com/JacobZufall/statementskeleton
 Project-URL: Issues, https://github.com/JacobZufall/statementskeleton/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
```

### Comparing `statementskeleton-1.1/src/statementskeleton.egg-info/SOURCES.txt` & `statementskeleton-1.2/src/statementskeleton.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
+src/__init__.py
 src/statementskeleton/__init__.py
 src/statementskeleton.egg-info/PKG-INFO
 src/statementskeleton.egg-info/SOURCES.txt
 src/statementskeleton.egg-info/dependency_links.txt
 src/statementskeleton.egg-info/top_level.txt
 src/statementskeleton/elements/Account.py
 src/statementskeleton/elements/Divider.py
```

### Comparing `statementskeleton-1.1/tests/test_Skeleton.py` & `statementskeleton-1.2/tests/test_Skeleton.py`

 * *Files identical despite different names*

