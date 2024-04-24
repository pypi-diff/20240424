# Comparing `tmp/pronto-2.5.6.tar.gz` & `tmp/pronto-2.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pronto-2.5.6.tar", last modified: Wed Feb 21 16:27:12 2024, max compression
+gzip compressed data, was "pronto-2.5.7.tar", last modified: Wed Apr 24 13:39:38 2024, max compression
```

## Comparing `pronto-2.5.6.tar` & `pronto-2.5.7.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 16:27:12.254152 pronto-2.5.6/
--rw-r--r--   0 runner    (1001) docker     (127)    18523 2024-02-21 16:27:04.000000 pronto-2.5.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-02-21 16:27:04.000000 pronto-2.5.6/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-21 16:27:04.000000 pronto-2.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-02-21 16:27:12.254152 pronto-2.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7807 2024-02-21 16:27:04.000000 pronto-2.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 16:27:12.246152 pronto-2.5.6/pronto/
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/definition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 16:27:12.250152 pronto-2.5.6/pronto/entity/
--rw-r--r--   0 runner    (1001) docker     (127)    24216 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/entity/attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 16:27:12.250152 pronto-2.5.6/pronto/logic/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12712 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/logic/lineage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    20624 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/ontology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 16:27:12.250152 pronto-2.5.6/pronto/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19357 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/parsers/_fastobo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/parsers/obo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/parsers/obojson.py
--rw-r--r--   0 runner    (1001) docker     (127)    37690 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/parsers/rdfxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/pv.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    19543 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/relationship.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 16:27:12.250152 pronto-2.5.6/pronto/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13392 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/serializers/_fastobo.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/serializers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/serializers/obo.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/serializers/obojson.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/serializers/ofn.py
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/synonym.py
--rw-r--r--   0 runner    (1001) docker     (127)    15010 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/term.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 16:27:12.250152 pronto-2.5.6/pronto/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/utils/iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/utils/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/utils/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/utils/warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-02-21 16:27:04.000000 pronto-2.5.6/pronto/xref.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 16:27:12.250152 pronto-2.5.6/pronto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-02-21 16:27:12.000000 pronto-2.5.6/pronto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-02-21 16:27:12.000000 pronto-2.5.6/pronto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 16:27:12.000000 pronto-2.5.6/pronto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-21 16:27:12.000000 pronto-2.5.6/pronto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-21 16:27:12.000000 pronto-2.5.6/pronto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 16:27:12.000000 pronto-2.5.6/pronto.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-02-21 16:27:12.254152 pronto-2.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-21 16:27:04.000000 pronto-2.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:39:38.490252 pronto-2.5.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    18782 2024-04-24 13:39:29.000000 pronto-2.5.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-24 13:39:29.000000 pronto-2.5.7/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-24 13:39:29.000000 pronto-2.5.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-04-24 13:39:38.490252 pronto-2.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7807 2024-04-24 13:39:29.000000 pronto-2.5.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:39:38.486252 pronto-2.5.7/pronto/
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:39:38.486252 pronto-2.5.7/pronto/entity/
+-rw-r--r--   0 runner    (1001) docker     (127)    24216 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/entity/attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:39:38.486252 pronto-2.5.7/pronto/logic/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12712 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/logic/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20624 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/ontology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:39:38.486252 pronto-2.5.7/pronto/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19357 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/parsers/_fastobo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/parsers/obo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/parsers/obojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37887 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/parsers/rdfxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/pv.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    19543 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/relationship.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:39:38.490252 pronto-2.5.7/pronto/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13392 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/serializers/_fastobo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/serializers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/serializers/obo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/serializers/obojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/serializers/ofn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/synonym.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15010 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/term.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:39:38.490252 pronto-2.5.7/pronto/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/utils/iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/utils/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/utils/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/utils/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-24 13:39:29.000000 pronto-2.5.7/pronto/xref.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:39:38.490252 pronto-2.5.7/pronto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-04-24 13:39:38.000000 pronto-2.5.7/pronto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-24 13:39:38.000000 pronto-2.5.7/pronto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:39:38.000000 pronto-2.5.7/pronto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 13:39:38.000000 pronto-2.5.7/pronto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 13:39:38.000000 pronto-2.5.7/pronto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:39:38.000000 pronto-2.5.7/pronto.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-24 13:39:38.490252 pronto-2.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-24 13:39:29.000000 pronto-2.5.7/setup.py
```

### Comparing `pronto-2.5.6/CHANGELOG.md` & `pronto-2.5.7/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
-[Unreleased]: https://github.com/althonos/pronto/compare/v2.5.6...HEAD
+[Unreleased]: https://github.com/althonos/pronto/compare/v2.5.7...HEAD
+
+## [v2.5.7] - 2024-04-24
+[v2.5.7]: https://github.com/althonos/pronto/compare/v2.5.6...v2.5.7
+### Fixed
+- Handling of RDF datatypes in RDF/XML parser ([#223](https://github.com/althonos/pronto/pull/223], by [@chrishmorris](https://github.com/chrishmorris)).
 
 ## [v2.5.6] - 2024-02-21
 [v2.5.6]: https://github.com/althonos/pronto/compare/v2.5.5...v2.5.6
 ### Added
 - Explicit support for Python 3.12.
 ### Fixed
 - Synonym types not being properly extracted by RDF/XML parser ([#218](https://github.com/althonos/pronto/issues/218)).
```

### Comparing `pronto-2.5.6/COPYING` & `pronto-2.5.7/COPYING`

 * *Files identical despite different names*

### Comparing `pronto-2.5.6/PKG-INFO` & `pronto-2.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pronto
-Version: 2.5.6
+Version: 2.5.7
 Summary: Python frontend to ontologies.
 Home-page: https://github.com/althonos/pronto
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/althonos/pronto/issues
 Project-URL: Changelog, https://pronto.readthedocs.io/en/latest/changes.html
```

### Comparing `pronto-2.5.6/README.md` & `pronto-2.5.7/README.md`

 * *Files identical despite different names*

### Comparing `pronto-2.5.6/pronto/__init__.py` & `pronto-2.5.7/pronto/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     LiteralPropertyValue.__name__,
     ResourcePropertyValue.__name__,
     Xref.__name__,
 ]
 
 __author__ = "Martin Larralde <martin.larralde@embl.de>"
 __license__ = "MIT"
-__version__ = "2.5.6"
+__version__ = "2.5.7"
 
 # Update the docstring with a link to the right version of the documentation
 # instead of the latest.
 if __doc__ is not None:
     __doc__ += f"""See Also:
     Online documentation for this version of the library on
     `Read The Docs <https://pronto.readthedocs.io/en/v{__version__}/>`_
```

### Comparing `pronto-2.5.6/pronto/definition.py` & `pronto-2.5.7/pronto/definition.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.6/pronto/entity/__init__.py` & `pronto-2.5.7/pronto/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.6/pronto/entity/attributes.py` & `pronto-2.5.7/pronto/entity/attributes.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.6/pronto/logic/lineage.py` & `pronto-2.5.7/pronto/logic/lineage.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.6/pronto/metadata.py` & `pronto-2.5.7/pronto/metadata.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.6/pronto/ontology.py` & `pronto-2.5.7/pronto/ontology.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.6/pronto/parsers/_fastobo.py` & `pronto-2.5.7/pronto/parsers/_fastobo.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.6/pronto/parsers/base.py` & `pronto-2.5.7/pronto/parsers/base.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.6/pronto/parsers/obo.py` & `pronto-2.5.7/pronto/parsers/obo.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.6/pronto/parsers/obojson.py` & `pronto-2.5.7/pronto/parsers/obojson.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.6/pronto/parsers/rdfxml.py` & `pronto-2.5.7/pronto/parsers/rdfxml.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,24 +169,27 @@
         if match is not None:
             return ":".join(match.groups())
         if self.ont.metadata.ontology is not None:
             id_ = self.ont.metadata.ontology
             match = re.match(f"^http://purl.obolibrary.org/obo/{id_}#(.*)$", iri)
             if match is not None:
                 return match.group(1)
-        return iri
+        return iri 
 
     def _compact_datatype(self, iri: str) -> str:
         match = re.match("^http://www.w3.org/2001/XMLSchema#(.*)$", iri)
         if match is not None:
             return f"xsd:{match.group(1)}"
         match = re.match("^http://www.w3.org/2000/01/rdf-schema#(.*)$", iri)
         if match is not None:
             return f"rdfs:{match.group(1)}"
-        raise iri
+        match = re.match("^http://www.w3.org/1999/02/22-rdf-syntax-ns#(.*)", iri)
+        if match is not None:
+            return f"rdf:{match.group(1)}"
+        raise ValueError(f"Invalid datatype IRI: {iri!r}")
 
     def _extract_term_relationship(
         self, elem: etree.Element
     ) -> Tuple[Optional[str], Optional[str]]:
         """Extract the relationship info from a `owl:Restriction` element.
 
         This only handles the simplest case of `owl:someValuesFrom` annotation
```

### Comparing `pronto-2.5.6/pronto/pv.py` & `pronto-2.5.7/pronto/pv.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.6/pronto/relationship.py` & `pronto-2.5.7/pronto/relationship.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.6/pronto/serializers/_fastobo.py` & `pronto-2.5.7/pronto/serializers/_fastobo.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.6/pronto/serializers/obo.py` & `pronto-2.5.7/pronto/serializers/obo.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.6/pronto/synonym.py` & `pronto-2.5.7/pronto/synonym.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.6/pronto/term.py` & `pronto-2.5.7/pronto/term.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.6/pronto/utils/io.py` & `pronto-2.5.7/pronto/utils/io.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.6/pronto/utils/iter.py` & `pronto-2.5.7/pronto/utils/iter.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.6/pronto/utils/meta.py` & `pronto-2.5.7/pronto/utils/meta.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.6/pronto/utils/pool.py` & `pronto-2.5.7/pronto/utils/pool.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.6/pronto/utils/warnings.py` & `pronto-2.5.7/pronto/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.6/pronto/xref.py` & `pronto-2.5.7/pronto/xref.py`

 * *Files identical despite different names*

### Comparing `pronto-2.5.6/pronto.egg-info/PKG-INFO` & `pronto-2.5.7/pronto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pronto
-Version: 2.5.6
+Version: 2.5.7
 Summary: Python frontend to ontologies.
 Home-page: https://github.com/althonos/pronto
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/althonos/pronto/issues
 Project-URL: Changelog, https://pronto.readthedocs.io/en/latest/changes.html
```

### Comparing `pronto-2.5.6/pronto.egg-info/SOURCES.txt` & `pronto-2.5.7/pronto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pronto-2.5.6/setup.cfg` & `pronto-2.5.7/setup.cfg`

 * *Files identical despite different names*

