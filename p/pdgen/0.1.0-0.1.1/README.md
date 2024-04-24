# Comparing `tmp/pdgen-0.1.0.tar.gz` & `tmp/pdgen-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdgen-0.1.0.tar", last modified: Wed Apr 24 21:06:25 2024, max compression
+gzip compressed data, was "pdgen-0.1.1.tar", last modified: Wed Apr 24 21:24:45 2024, max compression
```

## Comparing `pdgen-0.1.0.tar` & `pdgen-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 21:06:25.359739 pdgen-0.1.0/
--rw-rw-rw-   0        0        0      628 2024-04-24 21:06:25.358594 pdgen-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      712 2024-04-24 21:06:20.000000 pdgen-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-24 21:06:25.359739 pdgen-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-24 21:06:25.345249 pdgen-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-24 21:06:25.357607 pdgen-0.1.0/src/pdgen.egg-info/
--rw-rw-rw-   0        0        0      628 2024-04-24 21:06:25.000000 pdgen-0.1.0/src/pdgen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      146 2024-04-24 21:06:25.000000 pdgen-0.1.0/src/pdgen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 21:06:25.000000 pdgen-0.1.0/src/pdgen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 21:06:25.000000 pdgen-0.1.0/src/pdgen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 21:24:45.506537 pdgen-0.1.1/
+-rw-rw-rw-   0        0        0      628 2024-04-24 21:24:45.505272 pdgen-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      712 2024-04-24 21:24:39.000000 pdgen-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-24 21:24:45.506537 pdgen-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-24 21:24:45.485240 pdgen-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-24 21:24:45.488762 pdgen-0.1.1/src/pdgen/
+-rw-rw-rw-   0        0        0        0 2024-04-24 11:05:29.000000 pdgen-0.1.1/src/pdgen/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 21:24:45.503246 pdgen-0.1.1/src/pdgen/decorators/
+-rw-rw-rw-   0        0        0        0 2024-04-24 18:00:32.000000 pdgen-0.1.1/src/pdgen/decorators/__init__.py
+-rw-rw-rw-   0        0        0      687 2024-04-24 20:15:43.000000 pdgen-0.1.1/src/pdgen/decorators/decorators.py
+-rw-rw-rw-   0        0        0     2185 2024-04-24 20:33:14.000000 pdgen-0.1.1/src/pdgen/decorators/generation.py
+-rw-rw-rw-   0        0        0       82 2024-04-24 19:01:39.000000 pdgen-0.1.1/src/pdgen/decorators/store.py
+-rw-rw-rw-   0        0        0     6590 2024-04-24 19:56:04.000000 pdgen-0.1.1/src/pdgen/decorators/uml_types.py
+-rw-rw-rw-   0        0        0      730 2024-04-24 20:32:14.000000 pdgen-0.1.1/src/pdgen/diagram.py
+drwxrwxrwx   0        0        0        0 2024-04-24 21:24:45.504288 pdgen-0.1.1/src/pdgen.egg-info/
+-rw-rw-rw-   0        0        0      628 2024-04-24 21:24:45.000000 pdgen-0.1.1/src/pdgen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2024-04-24 21:24:45.000000 pdgen-0.1.1/src/pdgen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 21:24:45.000000 pdgen-0.1.1/src/pdgen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-24 21:24:45.000000 pdgen-0.1.1/src/pdgen.egg-info/top_level.txt
```

### Comparing `pdgen-0.1.0/PKG-INFO` & `pdgen-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdgen
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package for generating UML diagrams from Python code using PlantUML.
 Author-email: Tobias Bück <tab@softoft.de>
 Project-URL: Bug Reports, https://github.com/Softoft/pdgen/issues
 Project-URL: Source, https://github.com/Softoft/pdgen/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pdgen-0.1.0/pyproject.toml` & `pdgen-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pdgen"
-version = "0.1.0"
+version = "0.1.1"
 authors = [{name="Tobias Bück", email="tab@softoft.de"}]
 description = "A Python package for generating UML diagrams from Python code using PlantUML."
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

### Comparing `pdgen-0.1.0/src/pdgen.egg-info/PKG-INFO` & `pdgen-0.1.1/src/pdgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdgen
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package for generating UML diagrams from Python code using PlantUML.
 Author-email: Tobias Bück <tab@softoft.de>
 Project-URL: Bug Reports, https://github.com/Softoft/pdgen/issues
 Project-URL: Source, https://github.com/Softoft/pdgen/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

