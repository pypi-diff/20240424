# Comparing `tmp/linkture-2.5.3.tar.gz` & `tmp/linkture-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkture-2.5.3.tar", last modified: Wed Apr 24 00:27:08 2024, max compression
+gzip compressed data, was "linkture-2.5.4.tar", last modified: Wed Apr 24 11:58:19 2024, max compression
```

## Comparing `linkture-2.5.3.tar` & `linkture-2.5.4.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1064 2022-02-12 23:12:44.228988 linkture-2.5.3/LICENSE
--rw-r--r--   0        0        0     9941 2024-02-12 21:07:04.115612 linkture-2.5.3/README.md
--rw-r--r--   0        0        0     1031 2024-04-24 00:27:08.549810 linkture-2.5.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-23 19:22:30.399279 linkture-2.5.3/src/linkture/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 19:22:30.399279 linkture-2.5.3/tests/__init__.py
--rw-r--r--   0        0        0    10815 1970-01-01 00:00:00.000000 linkture-2.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-24 11:58:06.254156 linkture-2.5.4/LICENSE
+-rw-r--r--   0        0        0     9850 2024-04-24 11:58:06.254156 linkture-2.5.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-24 11:58:06.254156 linkture-2.5.4/__init__.py
+-rwxr-xr-x   0        0        0    29080 2024-04-24 11:58:06.254156 linkture-2.5.4/linkture.py
+-rw-r--r--   0        0        0     1292 2024-04-24 11:58:19.218121 linkture-2.5.4/pyproject.toml
+-rw-r--r--   0        0        0     1491 2024-04-24 11:58:06.258156 linkture-2.5.4/setup.py
+-rw-r--r--   0        0        0    11015 1970-01-01 00:00:00.000000 linkture-2.5.4/PKG-INFO
```

### Comparing `linkture-2.5.3/LICENSE` & `linkture-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `linkture-2.5.3/README.md` & `linkture-2.5.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 The parser tries to deal "intelligently" with different notations, but there are simply too many "edge-cases". If something isn't being parsed properly, try to rewrite the original reference(s) in a standard way or use {{ }} to force the detection.
 
 A couple of auxiliary functions provide a verse number lookup (either by BCV reference or integer). These can be useful to calculate the number of verses between two references, etc.
 
 ____
 ## Installation
 
-Download [latest source](https://github.com/erykjj/linkture/releases/latest) and `python3 -m pip install linkture-*.tar.gz`.
+`python3 -m pip install linkture`
 
 ____
 ## Command-line usage
 
 ```
 > python3 linkture.py -h
 usage: linkture.py [-h] [-v] [-q] [-f in-file | -r reference] [-o out-file]
```

### Comparing `linkture-2.5.3/pyproject.toml` & `linkture-2.5.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 [project]
 name = "linkture"
-version = "2.5.3"
+version = "2.5.4"
 description = "PARSE and PROCESS BIBLE SCRIPTURE REFERENCES: extract, tag, link, rewrite, translate, BCV-encode and decode"
 authors = [
     { name = "Eryk J.", email = "infiniti@inventati.org" },
 ]
 dependencies = [
     "setuptools>=59.6.0",
     "argparse>=1.4.0",
     "regex>=2023.8.8",
     "unidecode>=1.3.8",
-    "pathlib",
+    "pathlib>=1.0.1",
     "pandas==2.2.2",
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
+    "Topic :: Religion",
+    "Topic :: Text Processing :: General",
+    "Topic :: Text Processing :: Linguistic",
 ]
 keywords = [
     "bible",
     "scriptures",
     "scripture-references",
     "scripture-translation",
     "scripture-parser",
```

### Comparing `linkture-2.5.3/PKG-INFO` & `linkture-2.5.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 Metadata-Version: 2.1
 Name: linkture
-Version: 2.5.3
+Version: 2.5.4
 Summary: PARSE and PROCESS BIBLE SCRIPTURE REFERENCES: extract, tag, link, rewrite, translate, BCV-encode and decode
 Keywords: bible,scriptures,scripture-references,scripture-translation,scripture-parser,scripture-linker
 Author-Email: "Eryk J." <infiniti@inventati.org>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
+Classifier: Topic :: Religion
+Classifier: Topic :: Text Processing :: General
+Classifier: Topic :: Text Processing :: Linguistic
 Project-URL: Homepage, https://github.com/erykjj/linkture
 Requires-Python: >=3.9
 Requires-Dist: setuptools>=59.6.0
 Requires-Dist: argparse>=1.4.0
 Requires-Dist: regex>=2023.8.8
 Requires-Dist: unidecode>=1.3.8
-Requires-Dist: pathlib
+Requires-Dist: pathlib>=1.0.1
 Requires-Dist: pandas==2.2.2
 Description-Content-Type: text/markdown
 
 # linkture
 
 
 ## Purpose
@@ -36,15 +42,15 @@
 The parser tries to deal "intelligently" with different notations, but there are simply too many "edge-cases". If something isn't being parsed properly, try to rewrite the original reference(s) in a standard way or use {{ }} to force the detection.
 
 A couple of auxiliary functions provide a verse number lookup (either by BCV reference or integer). These can be useful to calculate the number of verses between two references, etc.
 
 ____
 ## Installation
 
-Download [latest source](https://github.com/erykjj/linkture/releases/latest) and `python3 -m pip install linkture-*.tar.gz`.
+`python3 -m pip install linkture`
 
 ____
 ## Command-line usage
 
 ```
 > python3 linkture.py -h
 usage: linkture.py [-h] [-v] [-q] [-f in-file | -r reference] [-o out-file]
```

