# Comparing `tmp/mdxcanvas-0.1.1.tar.gz` & `tmp/mdxcanvas-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdxcanvas-0.1.1.tar", max compression
+gzip compressed data, was "mdxcanvas-0.1.2.tar", max compression
```

## Comparing `mdxcanvas-0.1.1.tar` & `mdxcanvas-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1065 2024-01-31 20:08:12.653583 mdxcanvas-0.1.1/LICENSE
--rw-r--r--   0        0        0      156 2024-02-23 19:51:14.711484 mdxcanvas-0.1.1/mdxcanvas/__init__.py
--rw-r--r--   0        0        0    20788 2024-04-23 21:52:37.729116 mdxcanvas-0.1.1/mdxcanvas/canvas_creator.py
--rw-r--r--   0        0        0      914 2024-04-23 21:43:27.025380 mdxcanvas-0.1.1/mdxcanvas/deploy.py
--rw-r--r--   0        0        0     3392 2024-04-22 22:07:08.576705 mdxcanvas-0.1.1/mdxcanvas/document_schema.py
--rw-r--r--   0        0        0      873 2024-02-26 20:43:38.531257 mdxcanvas-0.1.1/mdxcanvas/extensions.py
--rw-r--r--   0        0        0     2689 2024-04-22 22:07:08.576782 mdxcanvas-0.1.1/mdxcanvas/jinja_parser.py
--rw-r--r--   0        0        0    25486 2024-04-22 22:07:08.577304 mdxcanvas-0.1.1/mdxcanvas/parser.py
--rw-r--r--   0        0        0      559 2024-04-22 22:07:08.577386 mdxcanvas-0.1.1/mdxcanvas/question_schema.py
--rw-r--r--   0        0        0     1878 2024-04-22 22:07:08.577697 mdxcanvas-0.1.1/mdxcanvas/templating.py
--rw-r--r--   0        0        0    15308 2024-04-22 22:07:08.577804 mdxcanvas-0.1.1/mdxcanvas/yaml_parser.py
--rw-r--r--   0        0        0      651 2024-04-23 21:52:48.699614 mdxcanvas-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 mdxcanvas-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-01-31 20:08:12.653583 mdxcanvas-0.1.2/LICENSE
+-rw-r--r--   0        0        0      156 2024-02-23 19:51:14.711484 mdxcanvas-0.1.2/mdxcanvas/__init__.py
+-rw-r--r--   0        0        0    20789 2024-04-23 21:55:26.002491 mdxcanvas-0.1.2/mdxcanvas/canvas_creator.py
+-rw-r--r--   0        0        0      914 2024-04-23 21:43:27.025380 mdxcanvas-0.1.2/mdxcanvas/deploy.py
+-rw-r--r--   0        0        0     3392 2024-04-22 22:07:08.576705 mdxcanvas-0.1.2/mdxcanvas/document_schema.py
+-rw-r--r--   0        0        0      873 2024-02-26 20:43:38.531257 mdxcanvas-0.1.2/mdxcanvas/extensions.py
+-rw-r--r--   0        0        0     2689 2024-04-22 22:07:08.576782 mdxcanvas-0.1.2/mdxcanvas/jinja_parser.py
+-rw-r--r--   0        0        0    25486 2024-04-22 22:07:08.577304 mdxcanvas-0.1.2/mdxcanvas/parser.py
+-rw-r--r--   0        0        0      559 2024-04-22 22:07:08.577386 mdxcanvas-0.1.2/mdxcanvas/question_schema.py
+-rw-r--r--   0        0        0     1878 2024-04-22 22:07:08.577697 mdxcanvas-0.1.2/mdxcanvas/templating.py
+-rw-r--r--   0        0        0    15308 2024-04-22 22:07:08.577804 mdxcanvas-0.1.2/mdxcanvas/yaml_parser.py
+-rw-r--r--   0        0        0      651 2024-04-23 21:55:30.944064 mdxcanvas-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 mdxcanvas-0.1.2/PKG-INFO
```

### Comparing `mdxcanvas-0.1.1/LICENSE` & `mdxcanvas-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.1/mdxcanvas/canvas_creator.py` & `mdxcanvas-0.1.2/mdxcanvas/canvas_creator.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from canvasapi import Canvas
 from canvasapi.assignment import Assignment
 from canvasapi.course import Course
 from canvasapi.module import Module
 from canvasapi.quiz import Quiz
 from markdown.extensions.codehilite import makeExtension as makeCodehiliteExtension
 
-from jinja_parser import process_jinja
+from .jinja_parser import process_jinja
 from .extensions import BlackInlineCodeExtension
 from .parser import DocumentParser, make_iso
 from .yaml_parser import DocumentWalker, parse_yaml
 
 
 def readfile(filepath: Path):
     with open(filepath) as file:
```

### Comparing `mdxcanvas-0.1.1/mdxcanvas/deploy.py` & `mdxcanvas-0.1.2/mdxcanvas/deploy.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.1/mdxcanvas/document_schema.py` & `mdxcanvas-0.1.2/mdxcanvas/document_schema.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.1/mdxcanvas/extensions.py` & `mdxcanvas-0.1.2/mdxcanvas/extensions.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.1/mdxcanvas/jinja_parser.py` & `mdxcanvas-0.1.2/mdxcanvas/jinja_parser.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.1/mdxcanvas/parser.py` & `mdxcanvas-0.1.2/mdxcanvas/parser.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.1/mdxcanvas/question_schema.py` & `mdxcanvas-0.1.2/mdxcanvas/question_schema.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.1/mdxcanvas/templating.py` & `mdxcanvas-0.1.2/mdxcanvas/templating.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.1/mdxcanvas/yaml_parser.py` & `mdxcanvas-0.1.2/mdxcanvas/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.1/pyproject.toml` & `mdxcanvas-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mdxcanvas"
-version = "0.1.1"
+version = "0.1.2"
 description = "A Canvas LMS API wrapper for maintaining content in markdown"
 authors = ["Gordon Bean <gbean@cs.byu.edu>", "Preston Raab <phr23@byu.edu>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Jinja2 = "^3.1.2"
```

### Comparing `mdxcanvas-0.1.1/PKG-INFO` & `mdxcanvas-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdxcanvas
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Canvas LMS API wrapper for maintaining content in markdown
 License: MIT
 Author: Gordon Bean
 Author-email: gbean@cs.byu.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

