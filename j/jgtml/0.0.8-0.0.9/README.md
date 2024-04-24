# Comparing `tmp/jgtml-0.0.8.tar.gz` & `tmp/jgtml-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jgtml-0.0.8.tar", last modified: Fri Feb 23 18:38:11 2024, max compression
+gzip compressed data, was "jgtml-0.0.9.tar", last modified: Fri Feb 23 19:10:02 2024, max compression
```

## Comparing `jgtml-0.0.8.tar` & `jgtml-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-02-23 18:38:11.516238 jgtml-0.0.8/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1086 2024-02-23 16:41:10.000000 jgtml-0.0.8/LICENSE
--rw-r--r--   0 jgi       (1000) jgi       (1000)     1858 2024-02-23 18:38:11.516238 jgtml-0.0.8/PKG-INFO
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       14 2024-02-23 16:41:10.000000 jgtml-0.0.8/README.md
--rwxrwxr-x   0 jgi       (1000) jgi       (1000)      212 2024-02-23 16:55:21.000000 jgtml-0.0.8/README.rst
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-02-23 18:38:11.512238 jgtml-0.0.8/jgtml/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      411 2024-02-23 18:38:02.000000 jgtml-0.0.8/jgtml/__init__.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     8255 2024-02-23 18:36:08.000000 jgtml-0.0.8/jgtml/jtc.py
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-02-23 18:38:11.512238 jgtml-0.0.8/jgtml.egg-info/
--rw-r--r--   0 jgi       (1000) jgi       (1000)     1858 2024-02-23 18:38:11.000000 jgtml-0.0.8/jgtml.egg-info/PKG-INFO
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      315 2024-02-23 18:38:11.000000 jgtml-0.0.8/jgtml.egg-info/SOURCES.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)        1 2024-02-23 18:38:11.000000 jgtml-0.0.8/jgtml.egg-info/dependency_links.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       45 2024-02-23 18:38:11.000000 jgtml-0.0.8/jgtml.egg-info/entry_points.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      479 2024-02-23 18:38:11.000000 jgtml-0.0.8/jgtml.egg-info/requires.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)        6 2024-02-23 18:38:11.000000 jgtml-0.0.8/jgtml.egg-info/top_level.txt
--rwxrwxr-x   0 jgi       (1000) jgi       (1000)      771 2024-02-23 18:38:02.000000 jgtml-0.0.8/pyproject.toml
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       38 2024-02-23 18:38:11.516238 jgtml-0.0.8/setup.cfg
--rwxrwxr-x   0 jgi       (1000) jgi       (1000)     1888 2024-02-23 17:12:31.000000 jgtml-0.0.8/setup.py
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-02-23 18:38:11.512238 jgtml-0.0.8/tests/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      551 2024-02-23 18:05:11.000000 jgtml-0.0.8/tests/test-calc-targets-2.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1473 2024-02-23 17:25:54.000000 jgtml-0.0.8/tests/test-calc-targets.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-02-23 19:10:02.114279 jgtml-0.0.9/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1086 2024-02-23 16:41:10.000000 jgtml-0.0.9/LICENSE
+-rw-r--r--   0 jgi       (1000) jgi       (1000)     1858 2024-02-23 19:10:02.114279 jgtml-0.0.9/PKG-INFO
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       14 2024-02-23 16:41:10.000000 jgtml-0.0.9/README.md
+-rwxrwxr-x   0 jgi       (1000) jgi       (1000)      212 2024-02-23 16:55:21.000000 jgtml-0.0.9/README.rst
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-02-23 19:10:02.106279 jgtml-0.0.9/jgtml/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      411 2024-02-23 19:09:53.000000 jgtml-0.0.9/jgtml/__init__.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     2338 2024-02-23 19:09:35.000000 jgtml-0.0.9/jgtml/jgtmlcli.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     8255 2024-02-23 18:36:08.000000 jgtml-0.0.9/jgtml/jtc.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-02-23 19:10:02.110279 jgtml-0.0.9/jgtml.egg-info/
+-rw-r--r--   0 jgi       (1000) jgi       (1000)     1858 2024-02-23 19:10:02.000000 jgtml-0.0.9/jgtml.egg-info/PKG-INFO
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      333 2024-02-23 19:10:02.000000 jgtml-0.0.9/jgtml.egg-info/SOURCES.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)        1 2024-02-23 19:10:02.000000 jgtml-0.0.9/jgtml.egg-info/dependency_links.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       49 2024-02-23 19:10:02.000000 jgtml-0.0.9/jgtml.egg-info/entry_points.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      479 2024-02-23 19:10:02.000000 jgtml-0.0.9/jgtml.egg-info/requires.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)        6 2024-02-23 19:10:02.000000 jgtml-0.0.9/jgtml.egg-info/top_level.txt
+-rwxrwxr-x   0 jgi       (1000) jgi       (1000)      771 2024-02-23 19:09:53.000000 jgtml-0.0.9/pyproject.toml
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       38 2024-02-23 19:10:02.114279 jgtml-0.0.9/setup.cfg
+-rwxrwxr-x   0 jgi       (1000) jgi       (1000)     1892 2024-02-23 19:05:36.000000 jgtml-0.0.9/setup.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-02-23 19:10:02.110279 jgtml-0.0.9/tests/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      551 2024-02-23 18:05:11.000000 jgtml-0.0.9/tests/test-calc-targets-2.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1473 2024-02-23 17:25:54.000000 jgtml-0.0.9/tests/test-calc-targets.py
```

### Comparing `jgtml-0.0.8/LICENSE` & `jgtml-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jgtml-0.0.8/PKG-INFO` & `jgtml-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jgtml
-Version: 0.0.8
+Version: 0.0.9
 Summary: JGT Ml - Machine Learning Tools
 Home-page: https://github.com/jgwill/jgtml
 Author: GUillaume Isabelle
 Author-email: Guillaume Isabelle <jgi@jgwill.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jgwill/jgtml
 Project-URL: Bug Tracker, https://github.com/jgwill/jgtml/issues
```

### Comparing `jgtml-0.0.8/jgtml/jtc.py` & `jgtml-0.0.9/jgtml/jtc.py`

 * *Files identical despite different names*

### Comparing `jgtml-0.0.8/jgtml.egg-info/PKG-INFO` & `jgtml-0.0.9/jgtml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jgtml
-Version: 0.0.8
+Version: 0.0.9
 Summary: JGT Ml - Machine Learning Tools
 Home-page: https://github.com/jgwill/jgtml
 Author: GUillaume Isabelle
 Author-email: Guillaume Isabelle <jgi@jgwill.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jgwill/jgtml
 Project-URL: Bug Tracker, https://github.com/jgwill/jgtml/issues
```

### Comparing `jgtml-0.0.8/pyproject.toml` & `jgtml-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.8.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jgtml"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Guillaume Isabelle", email="jgi@jgwill.com" },
 ]
 
 description = "JGT Ml - Machine Learning Tools"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `jgtml-0.0.8/setup.py` & `jgtml-0.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     author="GUillaume Isabelle",
     author_email="jgi@jgwill.com",
     url="https://github.com/jgwill/jgtml",
     packages=find_packages(include=["jgtml"], exclude=["*test*"]),
     # packages=find_packages(include=['jgtml', 'jgtml.forexconnect', 'jgtml.forexconnect.lib', 'jgtml.forexconnect.lib.windows', 'jgtml.forexconnect.lib.linux'], exclude=['*test*']),
     install_requires=INSTALL_REQUIRES,
     entry_points={
-        "console_scripts": ["jgtcli=jgtml.jgtcli:main"],
+        "console_scripts": ["jgtmlcli=jgtml.jgtmlcli:main"],
     },
     extras_require={
         "dev": (EXTRAS_DEV_LINT + EXTRAS_DEV_TEST + EXTRAS_DEV_DOCS),
         "dev-lint": EXTRAS_DEV_LINT,
         "dev-test": EXTRAS_DEV_TEST,
         "dev-docs": EXTRAS_DEV_DOCS,
     },
```

### Comparing `jgtml-0.0.8/tests/test-calc-targets-2.py` & `jgtml-0.0.9/tests/test-calc-targets-2.py`

 * *Files identical despite different names*

### Comparing `jgtml-0.0.8/tests/test-calc-targets.py` & `jgtml-0.0.9/tests/test-calc-targets.py`

 * *Files identical despite different names*

