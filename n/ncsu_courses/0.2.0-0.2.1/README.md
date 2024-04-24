# Comparing `tmp/ncsu_courses-0.2.0.tar.gz` & `tmp/ncsu_courses-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncsu_courses-0.2.0.tar", max compression
+gzip compressed data, was "ncsu_courses-0.2.1.tar", max compression
```

## Comparing `ncsu_courses-0.2.0.tar` & `ncsu_courses-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1060 2024-04-22 19:59:58.379640 ncsu_courses-0.2.0/LICENSE
--rw-r--r--   0        0        0     1534 2024-04-22 19:59:58.379640 ncsu_courses-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-04-22 19:59:58.379640 ncsu_courses-0.2.0/ncsu_courses/__init__.py
--rw-r--r--   0        0        0     2392 2024-04-22 19:59:58.379640 ncsu_courses-0.2.0/ncsu_courses/courses.py
--rw-r--r--   0        0        0     8004 2024-04-22 19:59:58.379640 ncsu_courses-0.2.0/ncsu_courses/sections.py
--rw-r--r--   0        0        0      451 2024-04-22 19:59:58.379640 ncsu_courses-0.2.0/ncsu_courses/subjects.py
--rw-r--r--   0        0        0      759 2024-04-22 19:59:58.379640 ncsu_courses-0.2.0/ncsu_courses/term.py
--rw-r--r--   0        0        0     1654 2024-04-22 19:59:58.379640 ncsu_courses-0.2.0/ncsu_courses/util.py
--rw-r--r--   0        0        0      467 2024-04-22 19:59:58.383640 ncsu_courses-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2155 1970-01-01 00:00:00.000000 ncsu_courses-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-04-23 21:21:15.741104 ncsu_courses-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1534 2024-04-23 21:21:15.741104 ncsu_courses-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-23 21:21:15.741104 ncsu_courses-0.2.1/ncsu_courses/__init__.py
+-rw-r--r--   0        0        0     2392 2024-04-23 21:21:15.741104 ncsu_courses-0.2.1/ncsu_courses/courses.py
+-rw-r--r--   0        0        0     8004 2024-04-23 21:21:15.741104 ncsu_courses-0.2.1/ncsu_courses/sections.py
+-rw-r--r--   0        0        0      451 2024-04-23 21:21:15.741104 ncsu_courses-0.2.1/ncsu_courses/subjects.py
+-rw-r--r--   0        0        0      759 2024-04-23 21:21:15.741104 ncsu_courses-0.2.1/ncsu_courses/term.py
+-rw-r--r--   0        0        0     1654 2024-04-23 21:21:15.741104 ncsu_courses-0.2.1/ncsu_courses/util.py
+-rw-r--r--   0        0        0      467 2024-04-23 21:21:15.745104 ncsu_courses-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2155 1970-01-01 00:00:00.000000 ncsu_courses-0.2.1/PKG-INFO
```

### Comparing `ncsu_courses-0.2.0/LICENSE` & `ncsu_courses-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ncsu_courses-0.2.0/README.md` & `ncsu_courses-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ncsu_courses-0.2.0/ncsu_courses/courses.py` & `ncsu_courses-0.2.1/ncsu_courses/courses.py`

 * *Files identical despite different names*

### Comparing `ncsu_courses-0.2.0/ncsu_courses/sections.py` & `ncsu_courses-0.2.1/ncsu_courses/sections.py`

 * *Files identical despite different names*

### Comparing `ncsu_courses-0.2.0/ncsu_courses/term.py` & `ncsu_courses-0.2.1/ncsu_courses/term.py`

 * *Files identical despite different names*

### Comparing `ncsu_courses-0.2.0/ncsu_courses/util.py` & `ncsu_courses-0.2.1/ncsu_courses/util.py`

 * *Files identical despite different names*

### Comparing `ncsu_courses-0.2.0/PKG-INFO` & `ncsu_courses-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncsu_courses
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python library for retrieving data about NCSU's course offerings and sections
 License: MIT
 Author: Brendon Hablutzel
 Author-email: booklvrbren@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

