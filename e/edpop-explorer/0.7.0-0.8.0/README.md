# Comparing `tmp/edpop-explorer-0.7.0.tar.gz` & `tmp/edpop_explorer-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edpop-explorer-0.7.0.tar", last modified: Wed Dec  6 12:54:40 2023, max compression
+gzip compressed data, was "edpop_explorer-0.8.0.tar", last modified: Wed Apr 24 08:37:42 2024, max compression
```

## Comparing `edpop-explorer-0.7.0.tar` & `edpop_explorer-0.8.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 tijmen    (1000) tijmen    (1000)        0 2023-12-06 12:54:40.445299 edpop-explorer-0.7.0/
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     1512 2023-01-26 17:59:00.000000 edpop-explorer-0.7.0/LICENSE
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)       38 2023-03-17 12:01:49.000000 edpop-explorer-0.7.0/MANIFEST.in
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     5800 2023-12-06 12:54:40.441966 edpop-explorer-0.7.0/PKG-INFO
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     4625 2023-10-17 19:06:55.000000 edpop-explorer-0.7.0/README.md
-drwxr-xr-x   0 tijmen    (1000) tijmen    (1000)        0 2023-12-06 12:54:40.438633 edpop-explorer-0.7.0/docs/
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     1844 2023-10-02 12:37:18.000000 edpop-explorer-0.7.0/docs/conf.py
-drwxr-xr-x   0 tijmen    (1000) tijmen    (1000)        0 2023-12-06 12:54:40.438633 edpop-explorer-0.7.0/edpop_explorer/
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     6656 2023-03-17 12:01:49.000000 edpop-explorer-0.7.0/edpop_explorer/M21_fields.csv
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     1209 2023-12-06 12:54:10.000000 edpop-explorer-0.7.0/edpop_explorer/__init__.py
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)      666 2023-08-07 12:16:01.000000 edpop-explorer-0.7.0/edpop_explorer/__main__.py
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     8767 2023-12-06 12:54:10.000000 edpop-explorer-0.7.0/edpop_explorer/edpopxshell.py
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     6766 2023-10-17 19:06:55.000000 edpop-explorer-0.7.0/edpop_explorer/fields.py
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)      649 2023-09-04 18:02:52.000000 edpop-explorer-0.7.0/edpop_explorer/rdf.py
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     6190 2023-12-06 12:54:10.000000 edpop-explorer-0.7.0/edpop_explorer/reader.py
-drwxr-xr-x   0 tijmen    (1000) tijmen    (1000)        0 2023-12-06 12:54:40.441966 edpop-explorer-0.7.0/edpop_explorer/readers/
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     1220 2023-12-06 12:54:10.000000 edpop-explorer-0.7.0/edpop_explorer/readers/__init__.py
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)      804 2023-12-06 12:54:10.000000 edpop-explorer-0.7.0/edpop_explorer/readers/bibliopolis.py
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     1330 2023-12-06 12:54:10.000000 edpop-explorer-0.7.0/edpop_explorer/readers/bnf.py
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     3475 2023-12-06 12:54:10.000000 edpop-explorer-0.7.0/edpop_explorer/readers/cerl_thesaurus.py
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     5429 2023-12-06 12:54:10.000000 edpop-explorer-0.7.0/edpop_explorer/readers/fbtee.py
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     5291 2023-12-06 12:54:10.000000 edpop-explorer-0.7.0/edpop_explorer/readers/gallica.py
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     1506 2023-12-06 12:54:10.000000 edpop-explorer-0.7.0/edpop_explorer/readers/hpb.py
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     3171 2023-12-06 12:54:10.000000 edpop-explorer-0.7.0/edpop_explorer/readers/kb.py
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     5103 2023-12-06 12:54:10.000000 edpop-explorer-0.7.0/edpop_explorer/readers/sbtireader.py
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     3829 2023-12-06 12:54:10.000000 edpop-explorer-0.7.0/edpop_explorer/readers/stcn.py
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     4883 2023-12-06 12:54:10.000000 edpop-explorer-0.7.0/edpop_explorer/readers/ustc.py
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     3262 2023-12-06 12:54:10.000000 edpop-explorer-0.7.0/edpop_explorer/readers/vd.py
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)    10201 2023-12-06 12:54:10.000000 edpop-explorer-0.7.0/edpop_explorer/record.py
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     5119 2023-12-06 12:54:10.000000 edpop-explorer-0.7.0/edpop_explorer/sparqlreader.py
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)      221 2023-12-06 12:54:10.000000 edpop-explorer-0.7.0/edpop_explorer/sql.py
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)    10876 2023-10-02 12:37:18.000000 edpop-explorer-0.7.0/edpop_explorer/srumarc21reader.py
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     3272 2023-12-06 12:54:10.000000 edpop-explorer-0.7.0/edpop_explorer/srureader.py
-drwxr-xr-x   0 tijmen    (1000) tijmen    (1000)        0 2023-12-06 12:54:40.441966 edpop-explorer-0.7.0/edpop_explorer.egg-info/
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     5800 2023-12-06 12:54:40.000000 edpop-explorer-0.7.0/edpop_explorer.egg-info/PKG-INFO
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     1157 2023-12-06 12:54:40.000000 edpop-explorer-0.7.0/edpop_explorer.egg-info/SOURCES.txt
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)        1 2023-12-06 12:54:40.000000 edpop-explorer-0.7.0/edpop_explorer.egg-info/dependency_links.txt
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)       56 2023-12-06 12:54:40.000000 edpop-explorer-0.7.0/edpop_explorer.egg-info/entry_points.txt
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)      185 2023-12-06 12:54:40.000000 edpop-explorer-0.7.0/edpop_explorer.egg-info/requires.txt
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)       40 2023-12-06 12:54:40.000000 edpop-explorer-0.7.0/edpop_explorer.egg-info/top_level.txt
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     1312 2023-12-06 12:54:10.000000 edpop-explorer-0.7.0/pyproject.toml
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)       38 2023-12-06 12:54:40.445299 edpop-explorer-0.7.0/setup.cfg
-drwxr-xr-x   0 tijmen    (1000) tijmen    (1000)        0 2023-12-06 12:54:40.441966 edpop-explorer-0.7.0/tests/
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)        0 2023-03-17 12:01:49.000000 edpop-explorer-0.7.0/tests/__init__.py
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)      304 2023-12-06 12:54:10.000000 edpop-explorer-0.7.0/tests/conftest.py
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     2353 2023-12-06 12:54:10.000000 edpop-explorer-0.7.0/tests/test_allreaders.py
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     3435 2023-10-17 19:06:55.000000 edpop-explorer-0.7.0/tests/test_field.py
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     2952 2023-12-06 12:54:10.000000 edpop-explorer-0.7.0/tests/test_reader.py
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     3167 2023-12-06 12:54:10.000000 edpop-explorer-0.7.0/tests/test_record.py
--rw-r--r--   0 tijmen    (1000) tijmen    (1000)     1742 2023-12-06 12:54:10.000000 edpop-explorer-0.7.0/tests/test_srureader.py
+drwxr-xr-x   0 tijmen    (1000) tijmen    (1000)        0 2024-04-24 08:37:42.064523 edpop_explorer-0.8.0/
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)     1512 2023-01-26 17:59:00.000000 edpop_explorer-0.8.0/LICENSE
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)       38 2023-03-17 12:01:49.000000 edpop_explorer-0.8.0/MANIFEST.in
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)     5833 2024-04-24 08:37:42.064523 edpop_explorer-0.8.0/PKG-INFO
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)     4625 2023-10-17 19:06:55.000000 edpop_explorer-0.8.0/README.md
+drwxr-xr-x   0 tijmen    (1000) tijmen    (1000)        0 2024-04-24 08:37:42.061190 edpop_explorer-0.8.0/docs/
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)     1844 2023-10-02 12:37:18.000000 edpop_explorer-0.8.0/docs/conf.py
+drwxr-xr-x   0 tijmen    (1000) tijmen    (1000)        0 2024-04-24 08:37:42.061190 edpop_explorer-0.8.0/edpop_explorer/
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)     6656 2023-03-17 12:01:49.000000 edpop_explorer-0.8.0/edpop_explorer/M21_fields.csv
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)     1217 2024-04-24 08:35:18.000000 edpop_explorer-0.8.0/edpop_explorer/__init__.py
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)      666 2023-08-07 12:16:01.000000 edpop_explorer-0.8.0/edpop_explorer/__main__.py
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)     8772 2024-04-24 08:35:18.000000 edpop_explorer-0.8.0/edpop_explorer/edpopxshell.py
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)     6766 2023-10-17 19:06:55.000000 edpop_explorer-0.8.0/edpop_explorer/fields.py
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)      649 2023-09-04 18:02:52.000000 edpop_explorer-0.8.0/edpop_explorer/rdf.py
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)    12114 2024-04-24 08:35:18.000000 edpop_explorer-0.8.0/edpop_explorer/reader.py
+drwxr-xr-x   0 tijmen    (1000) tijmen    (1000)        0 2024-04-24 08:37:42.064523 edpop_explorer-0.8.0/edpop_explorer/readers/
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)     1220 2023-12-06 12:54:10.000000 edpop_explorer-0.8.0/edpop_explorer/readers/__init__.py
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)      804 2023-12-06 12:54:10.000000 edpop_explorer-0.8.0/edpop_explorer/readers/bibliopolis.py
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)     1330 2023-12-06 12:54:10.000000 edpop_explorer-0.8.0/edpop_explorer/readers/bnf.py
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)     3475 2023-12-06 12:54:10.000000 edpop_explorer-0.8.0/edpop_explorer/readers/cerl_thesaurus.py
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)     5683 2024-04-24 08:35:18.000000 edpop_explorer-0.8.0/edpop_explorer/readers/fbtee.py
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)     5291 2024-01-03 12:55:04.000000 edpop_explorer-0.8.0/edpop_explorer/readers/gallica.py
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)     1506 2023-12-06 12:54:10.000000 edpop_explorer-0.8.0/edpop_explorer/readers/hpb.py
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)     3171 2023-12-06 12:54:10.000000 edpop_explorer-0.8.0/edpop_explorer/readers/kb.py
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)     5034 2024-04-24 08:35:18.000000 edpop_explorer-0.8.0/edpop_explorer/readers/sbtireader.py
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)     3828 2024-04-24 08:35:18.000000 edpop_explorer-0.8.0/edpop_explorer/readers/stcn.py
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)     4929 2024-04-24 08:35:18.000000 edpop_explorer-0.8.0/edpop_explorer/readers/ustc.py
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)     3262 2023-12-06 12:54:10.000000 edpop_explorer-0.8.0/edpop_explorer/readers/vd.py
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)    10202 2024-04-24 08:35:18.000000 edpop_explorer-0.8.0/edpop_explorer/record.py
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)     5376 2024-04-24 08:35:18.000000 edpop_explorer-0.8.0/edpop_explorer/sparqlreader.py
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)      229 2024-04-24 08:35:18.000000 edpop_explorer-0.8.0/edpop_explorer/sql.py
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)    10876 2023-10-02 12:37:18.000000 edpop_explorer-0.8.0/edpop_explorer/srumarc21reader.py
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)     3559 2024-04-24 08:35:18.000000 edpop_explorer-0.8.0/edpop_explorer/srureader.py
+drwxr-xr-x   0 tijmen    (1000) tijmen    (1000)        0 2024-04-24 08:37:42.064523 edpop_explorer-0.8.0/edpop_explorer.egg-info/
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)     5833 2024-04-24 08:37:42.000000 edpop_explorer-0.8.0/edpop_explorer.egg-info/PKG-INFO
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)     1157 2024-04-24 08:37:42.000000 edpop_explorer-0.8.0/edpop_explorer.egg-info/SOURCES.txt
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)        1 2024-04-24 08:37:42.000000 edpop_explorer-0.8.0/edpop_explorer.egg-info/dependency_links.txt
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)       56 2024-04-24 08:37:42.000000 edpop_explorer-0.8.0/edpop_explorer.egg-info/entry_points.txt
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)      203 2024-04-24 08:37:42.000000 edpop_explorer-0.8.0/edpop_explorer.egg-info/requires.txt
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)       37 2024-04-24 08:37:42.000000 edpop_explorer-0.8.0/edpop_explorer.egg-info/top_level.txt
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)     1335 2024-04-24 08:35:26.000000 edpop_explorer-0.8.0/pyproject.toml
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)       38 2024-04-24 08:37:42.064523 edpop_explorer-0.8.0/setup.cfg
+drwxr-xr-x   0 tijmen    (1000) tijmen    (1000)        0 2024-04-24 08:37:42.064523 edpop_explorer-0.8.0/tests/
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)        0 2023-03-17 12:01:49.000000 edpop_explorer-0.8.0/tests/__init__.py
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)      304 2023-12-06 12:54:10.000000 edpop_explorer-0.8.0/tests/conftest.py
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)     3891 2024-04-24 08:35:18.000000 edpop_explorer-0.8.0/tests/test_allreaders.py
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)     3435 2023-10-17 19:06:55.000000 edpop_explorer-0.8.0/tests/test_field.py
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)     5095 2024-04-24 08:35:18.000000 edpop_explorer-0.8.0/tests/test_reader.py
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)     3167 2023-12-06 12:54:10.000000 edpop_explorer-0.8.0/tests/test_record.py
+-rw-r--r--   0 tijmen    (1000) tijmen    (1000)     1742 2023-12-06 12:54:10.000000 edpop_explorer-0.8.0/tests/test_srureader.py
```

### Comparing `edpop-explorer-0.7.0/LICENSE` & `edpop_explorer-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edpop-explorer-0.7.0/PKG-INFO` & `edpop_explorer-0.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edpop-explorer
-Version: 0.7.0
+Version: 0.8.0
 Summary: Common interface to multiple library catalogues and bibliographical databases
 Author-email: "Utrecht University, Centre for Digital Humanities - Research Software Lab" <cdh@uu.nl>
 Project-URL: Homepage, https://github.com/UUDigitalHumanitieslab/edpop-explorer
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -20,14 +20,15 @@
 Requires-Dist: pyreadline3; platform_system == "Windows"
 Requires-Dist: colorama; platform_system == "Windows"
 Requires-Dist: cmd2
 Requires-Dist: pyyaml
 Requires-Dist: rdflib<8,>=7.0.0
 Requires-Dist: Pygments
 Requires-Dist: xmltodict>=0.13.0
+Requires-Dist: typing_extensions
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 
 [![PyPI Version](https://img.shields.io/pypi/v/edpop-explorer)](https://pypi.org/project/edpop-explorer/) [![Tests](https://github.com/UUDigitalHumanitieslab/edpop-explorer/actions/workflows/test.yml/badge.svg)](https://github.com/UUDigitalHumanitieslab/edpop-explorer/actions/workflows/test.yml) [![Read the Docs](https://readthedocs.org/projects/edpop-explorer/badge/?version=latest&style=flat)](https://edpop-explorer.readthedocs.io/en/latest/)
```

### Comparing `edpop-explorer-0.7.0/README.md` & `edpop_explorer-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `edpop-explorer-0.7.0/docs/conf.py` & `edpop_explorer-0.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `edpop-explorer-0.7.0/edpop_explorer/M21_fields.csv` & `edpop_explorer-0.8.0/edpop_explorer/M21_fields.csv`

 * *Files identical despite different names*

### Comparing `edpop-explorer-0.7.0/edpop_explorer/__init__.py` & `edpop_explorer-0.8.0/edpop_explorer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __all__ = [
     'EDPOPREC', 'RELATORS', 'bind_common_namespaces',
     'Field', 'FieldError', 'LocationField',
     'Reader', 'ReaderError', 'NotFoundError',
-    'GetByIdBasedOnQueryMixin', 'PreparedQuery', 'PreparedQueryType',
+    'GetByIdBasedOnQueryMixin', 'BasePreparedQuery', 'PreparedQueryType',
     'Record', 'RawData', 'RecordError', 'BibliographicalRecord',
     'BiographicalRecord', 'LazyRecordMixin',
     'SRUReader',
     'Marc21Data', 'Marc21Field', 'Marc21BibliographicalRecord',
     'Marc21DataMixin', 'SRUMarc21Reader', 'SRUMarc21BibliographicalReader',
     'BIBLIOGRAPHICAL', 'BIOGRAPHICAL'
 ]
@@ -15,15 +15,15 @@
 # ruff: noqa
 BIBLIOGRAPHICAL = "bibliographical"
 BIOGRAPHICAL = "biographical"
 
 from .rdf import EDPOPREC, RELATORS, bind_common_namespaces
 from .fields import Field, FieldError, LocationField
 from .reader import (
-    Reader, ReaderError, GetByIdBasedOnQueryMixin, PreparedQuery,
+    Reader, ReaderError, GetByIdBasedOnQueryMixin, BasePreparedQuery,
     PreparedQueryType, NotFoundError
 )
 from .record import (
     Record, RawData, RecordError, BibliographicalRecord, BiographicalRecord,
     LazyRecordMixin
 )
 from .srureader import SRUReader
```

### Comparing `edpop-explorer-0.7.0/edpop_explorer/__main__.py` & `edpop_explorer-0.8.0/edpop_explorer/__main__.py`

 * *Files identical despite different names*

### Comparing `edpop-explorer-0.7.0/edpop_explorer/edpopxshell.py` & `edpop_explorer-0.8.0/edpop_explorer/edpopxshell.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             return
         assert self.reader.number_of_results is not None
         assert self.reader.number_fetched is not None
         if self.shown >= self.reader.number_of_results:
             self.perror('All records have been shown')
         else:
             if self.reader.number_fetched - self.shown < self.RECORDS_PER_PAGE:
-                self.reader.fetch_next()
+                self.reader.fetch()
             self.shown += self._show_records(self.reader.records,
                                              self.shown,
                                              self.RECORDS_PER_PAGE)
 
     def do_show(self, args) -> None:
         '''Show a normalized version of the record with the given number.'''
         record = self.get_record_from_argument(args)
@@ -191,15 +191,15 @@
         'Universal Short Title Catalogue'
         self._query(USTCReader, args)
     
     def do_kb(self, args) -> None:
         'Koninklijke Bibliotheek'
         self._query(KBReader, args)
 
-    def _show_records(self, records: List[Record],
+    def _show_records(self, records: List[Optional[Record]],
                       start: int,
                       limit=math.inf) -> int:
         """Show the records from start, with limit as the maximum number
         of records to show. Return the number of records shown."""
         total = len(records)
         remaining = total - start
         if remaining < 1:
```

### Comparing `edpop-explorer-0.7.0/edpop_explorer/fields.py` & `edpop_explorer-0.8.0/edpop_explorer/fields.py`

 * *Files identical despite different names*

### Comparing `edpop-explorer-0.7.0/edpop_explorer/rdf.py` & `edpop_explorer-0.8.0/edpop_explorer/rdf.py`

 * *Files identical despite different names*

### Comparing `edpop-explorer-0.7.0/edpop_explorer/readers/__init__.py` & `edpop_explorer-0.8.0/edpop_explorer/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `edpop-explorer-0.7.0/edpop_explorer/readers/bibliopolis.py` & `edpop_explorer-0.8.0/edpop_explorer/readers/bibliopolis.py`

 * *Files identical despite different names*

### Comparing `edpop-explorer-0.7.0/edpop_explorer/readers/bnf.py` & `edpop_explorer-0.8.0/edpop_explorer/readers/bnf.py`

 * *Files identical despite different names*

### Comparing `edpop-explorer-0.7.0/edpop_explorer/readers/cerl_thesaurus.py` & `edpop_explorer-0.8.0/edpop_explorer/readers/cerl_thesaurus.py`

 * *Files identical despite different names*

### Comparing `edpop-explorer-0.7.0/edpop_explorer/readers/fbtee.py` & `edpop_explorer-0.8.0/edpop_explorer/readers/fbtee.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 from pathlib import Path
 import sqlite3
 from rdflib import URIRef
 import requests
 from appdirs import AppDirs
-from typing import List, Optional
+from typing import Optional
 
 from edpop_explorer import (
     Reader, BibliographicalRecord, ReaderError, Field, BIBLIOGRAPHICAL
 )
 from edpop_explorer.reader import GetByIdBasedOnQueryMixin
 from edpop_explorer.sql import SQLPreparedQuery
 
 
 class FBTEEReader(GetByIdBasedOnQueryMixin, Reader):
     DATABASE_URL = 'https://dhstatic.hum.uu.nl/edpop/cl.sqlite3'
     DATABASE_LICENSE = 'https://dhstatic.hum.uu.nl/edpop/LICENSE.txt'
     FBTEE_LINK = 'http://fbtee.uws.edu.au/stn/interface/browse.php?t=book&' \
         'id={}'
-    records: List[BibliographicalRecord]
     READERTYPE = BIBLIOGRAPHICAL
     CATALOG_URIREF = URIRef(
         'https://edpop.hum.uu.nl/readers/fbtee'
     )
     IRI_PREFIX = "https://edpop.hum.uu.nl/readers/fbtee/"
     prepared_query: Optional[SQLPreparedQuery] = None
+    FETCH_ALL_AT_ONCE = True
 
     def __init__(self):
+        super().__init__()
         self.database_file = Path(
             AppDirs('edpop-explorer', 'cdh').user_data_dir
         ) / 'cl.sqlite3'
 
     def prepare_data(self):
         if not self.database_file.exists():
             self._download_database()
@@ -88,52 +89,54 @@
         if publisher:
             record.publisher_or_printer = Field(publisher)
         record.contributors = []
         for author in record.data['authors']:
             # author is tuple of author code and author name
             record.contributors.append(Field(author[1]))
 
-    def fetch(self) -> None:
+    def fetch_range(self, range_to_fetch: range) -> range:
+        # This method always fetches all data at once. This could be avoided,
+        # but it is inexpensive because the data is locally available and
+        # the dataset is small.
         self.prepare_data()
         if not self.prepared_query:
             raise ReaderError('First call prepare_query method')
-
+        if self.fetching_exhausted:
+            return range(0)
         cur = self.con.cursor()
         columns = [x[1] for x in cur.execute('PRAGMA table_info(books)')]
         res = cur.execute(
             'SELECT B.*, BA.author_code, A.author_name FROM books B '
             'LEFT OUTER JOIN books_authors BA on B.book_code=BA.book_code '
             'JOIN authors A on BA.author_code=A.author_code '
             f'{self.prepared_query.where_statement} '
             'ORDER BY B.book_code',
             self.prepared_query.arguments
         )
-        self.records = []
         last_book_code = ''
+        i = -1
         for row in res:
             # Since we are joining with another table, a book may be repeated,
             # so check if this is a new item
             book_code: str = row[columns.index('book_code')]
             if last_book_code != book_code:
+                # We have a new book, so update i
+                i += 1
                 record = BibliographicalRecord(self.__class__)
                 record.data = {}
-                for i in range(len(columns)):
-                    record.data[columns[i]] = row[i]
+                for j in range(len(columns)):
+                    record.data[columns[j]] = row[j]
                 record.identifier = book_code
                 record.link = self.FBTEE_LINK.format(book_code)
                 record.data['authors'] = []
-                self.records.append(record)
+                self.records[i] = record
                 last_book_code = book_code
             # Add author_code and author_name to the last record
             assert len(self.records) > 0
             author_code = row[len(columns)]
             author_name = row[len(columns) + 1]
-            assert isinstance(self.records[-1].data, dict)
-            self.records[-1].data['authors'].append((author_code, author_name))
+            assert isinstance(self.records[i].data, dict)
+            self.records[i].data['authors'].append((author_code, author_name))
         for record in self.records:
             self._add_fields(record)
         self.number_of_results = len(self.records)
-        self.number_fetched = self.number_of_results
-        self.fetching_exhausted = True
-
-    def fetch_next(self):
-        pass
+        return range(0, len(self.records))
```

### Comparing `edpop-explorer-0.7.0/edpop_explorer/readers/gallica.py` & `edpop_explorer-0.8.0/edpop_explorer/readers/gallica.py`

 * *Files identical despite different names*

### Comparing `edpop-explorer-0.7.0/edpop_explorer/readers/hpb.py` & `edpop_explorer-0.8.0/edpop_explorer/readers/hpb.py`

 * *Files identical despite different names*

### Comparing `edpop-explorer-0.7.0/edpop_explorer/readers/kb.py` & `edpop_explorer-0.8.0/edpop_explorer/readers/kb.py`

 * *Files identical despite different names*

### Comparing `edpop-explorer-0.7.0/edpop_explorer/readers/sbtireader.py` & `edpop_explorer-0.8.0/edpop_explorer/readers/sbtireader.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 import requests
 from typing import List, Dict, Optional
 
 from edpop_explorer import (
     Reader, Record, ReaderError, BiographicalRecord, Field
 )
 
-RECORDS_PER_PAGE = 10
-
 
 class SBTIReader(Reader):
     api_url = 'https://data.cerl.org/sbti/_search'
     api_by_id_base_url = 'https://data.cerl.org/sbti/'
     link_base_url = 'https://data.cerl.org/sbti/'
     fetching_exhausted: bool = False
     additional_params: Optional[Dict[str, str]] = None
     CATALOG_URIREF = URIRef(
         'https://edpop.hum.uu.nl/readers/sbti'
     )
     IRI_PREFIX = "https://edpop.hum.uu.nl/readers/sbti/"
+    DEFAULT_RECORDS_PER_PAGE = 10
 
     @classmethod
     def _get_name_field(cls, data: dict) -> Optional[Field]:
         field = None
         firstname = data.get("firstname", None)
         name = data.get("name", None)
         if firstname and name:
@@ -76,22 +75,25 @@
                 name = place.get("name", None)
                 if name:
                     field = Field(name)
                     record.places_of_activity.append(field)
 
         return record
 
-    def _perform_query(self, start_record: int) -> List[Record]:
+    def _perform_query(self, start_record: int, maximum_records: Optional[int]) -> List[Record]:
+        assert isinstance(self.prepared_query, str)
+        if maximum_records is None:
+            maximum_records = self.DEFAULT_RECORDS_PER_PAGE
         try:
             response = requests.get(
                 self.api_url,
                 params={
                     'query': self.prepared_query,
                     'from': start_record,
-                    'size': RECORDS_PER_PAGE,
+                    'size': maximum_records,
                     'mode': 'default',
                     'sort': 'default'
                 },
                 headers={
                     'Accept': 'application/json'
                 }
             ).json()
@@ -121,27 +123,19 @@
         return records
 
     @classmethod
     def transform_query(cls, query) -> str:
         # No transformation needed
         return query
 
-    def fetch(self) -> None:
-        self.records = []
+    def fetch_range(self, range_to_fetch: range) -> range:
         if self.prepared_query is None:
             raise ReaderError('First call prepare_query')
-        results = self._perform_query(0)
-        self.records.extend(results)
-        self.number_fetched = len(self.records)
-        if self.number_fetched == self.number_of_results:
-            self.fetching_exhausted = True
-
-    def fetch_next(self) -> None:
-        # TODO: can be merged with fetch method
         if self.fetching_exhausted:
-            return
-        start_record = len(self.records) + 1
-        results = self._perform_query(start_record)
-        self.records.extend(results)
-        self.number_fetched = len(self.records)
-        if self.number_fetched == self.number_of_results:
-            self.fetching_exhausted = True
+            return range(0)
+        start_record = range_to_fetch.start
+        number_to_fetch = range_to_fetch.stop - start_record
+        results = self._perform_query(start_record, number_to_fetch)
+        for i, result in enumerate(results):
+            self.records[i] = result
+        return range(start_record, start_record + len(results))
+
```

### Comparing `edpop-explorer-0.7.0/edpop_explorer/readers/stcn.py` & `edpop_explorer-0.8.0/edpop_explorer/readers/stcn.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     )
     IRI_PREFIX = "https://edpop.hum.uu.nl/readers/stcn/"
 
     def __init__(self):
         super().__init__()
 
     @classmethod
-    def _convert_record(
+    def convert_record(
         cls, graph: Graph, record: BibliographicalRDFRecord
     ) -> None:
         SCHEMA = Namespace('http://schema.org/')
         # First get the title and languages fields, which are simple
         # properties
         assert record.identifier is not None
         subject_node = URIRef(record.identifier)
```

### Comparing `edpop-explorer-0.7.0/edpop_explorer/readers/ustc.py` & `edpop_explorer-0.8.0/edpop_explorer/readers/ustc.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,16 +16,18 @@
     USTC_LINK = 'https://www.ustc.ac.uk/editions/{}'
     READERTYPE = BIBLIOGRAPHICAL
     CATALOG_URIREF = URIRef(
         'https://edpop.hum.uu.nl/readers/ustc'
     )
     IRI_PREFIX = "https://edpop.hum.uu.nl/readers/ustc/"
     prepared_query: Optional[SQLPreparedQuery] = None
+    FETCH_ALL_AT_ONCE = True
 
     def __init__(self):
+        super().__init__()
         self.database_file = Path(
             AppDirs('edpop-explorer', 'cdh').user_data_dir
         ) / self.DATABASE_FILENAME
 
     def prepare_data(self):
         if not self.database_file.exists():
             # Find database dir with .resolve() because on Windows it is
@@ -62,47 +64,44 @@
         except ValueError:
             raise ReaderError(f"Identifier {identifier} is not an integer")
         return SQLPreparedQuery(
             where_statement="WHERE E.sn = ?",
             arguments=[identifier_int]
         )
 
-    def fetch(self) -> None:
+    def fetch_range(self, range_to_fetch: range) -> range:
         self.prepare_data()
 
         # This method fetches all records immediately, because the data is
         # locally stored.
 
         if not self.prepared_query:
             raise ReaderError('No query has been set')
+        if self.fetching_exhausted:
+            return range(0)
 
         cur = self.con.cursor()
         columns = [x[1] for x in cur.execute('PRAGMA table_info(editions)')]
         # This kind of query is far from ideal, but the alternative is to
         # implement SQLite full text search which is probably too much work
         # for our current goal (i.e. getting insight in the data structures)
         res = cur.execute(
             'SELECT E.* FROM editions E '
             + self.prepared_query.where_statement
             + ' ORDER BY E.id',
             self.prepared_query.arguments,
         )
-        self.records = []
-        for row in res:
+        for i, row in enumerate(res):
             data = {}
-            for i in range(len(columns)):
-                data[columns[i]] = row[i]
+            for j in range(len(columns)):
+                data[columns[j]] = row[j]
             record = self._convert_record(data)
-            self.records.append(record)
+            self.records[i] = record
         self.number_of_results = len(self.records)
-        self.number_fetched = self.number_of_results
-        self.fetching_exhausted = True
-
-    def fetch_next(self):
-        pass
+        return range(0, len(self.records))
 
     def _convert_record(self, data: dict) -> BibliographicalRecord:
         record = BibliographicalRecord(from_reader=self.__class__)
         record.data = data
         record.identifier = data['sn']
         record.link = self.USTC_LINK.format(data['sn'])
         record.title = Field(data['std_title'])
```

### Comparing `edpop-explorer-0.7.0/edpop_explorer/readers/vd.py` & `edpop_explorer-0.8.0/edpop_explorer/readers/vd.py`

 * *Files identical despite different names*

### Comparing `edpop-explorer-0.7.0/edpop_explorer/record.py` & `edpop_explorer-0.8.0/edpop_explorer/record.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     """Python representation of edpoprec:Record.
 
     This base class provides some basic attributes, an infrastructure
     to define fields and a method to convert the record to RDF.
     While this is a non-abstract base class, no fields are
     defined here -- these should be added in subclasses. ``Record``
     and its subclasses should be created by calling the constructor
-    with the ``Reader`` class as the ``from_reader`` argument
+    with the ``Reader`` class as the ``from_reader`` parameter
     and by setting the ``data``, ``link``, ``identifier`` and
     ``subject_node`` attributes (all are optional but recommended),
     as well as the fields that are defined by the subclass.
     fields are set using the attribute with the same name:
     set them to an instance of ``Field`` or to ``None``. The
     basic attributes and the fields are ``None`` by default.
```

### Comparing `edpop-explorer-0.7.0/edpop_explorer/sparqlreader.py` & `edpop_explorer-0.8.0/edpop_explorer/sparqlreader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import Optional, Type
 from rdflib import Graph
 import json
 from SPARQLWrapper import SPARQLWrapper, SPARQLExceptions, JSON as JSONFormat
 from abc import abstractmethod
 
+from typing_extensions import override
+
 from edpop_explorer import (
     Reader, Record, BibliographicalRecord, ReaderError, RecordError,
     LazyRecordMixin
 )
 
 PREFIXES = {
     'rdf': 'http://www.w3.org/1999/02/22-rdf-syntax-ns#',
@@ -99,55 +101,59 @@
 
 
 class SparqlReader(Reader):
     endpoint: str
     name_predicate: str
     filter: Optional[str] = None
     prepared_query: Optional[str]
+    FETCH_ALL_AT_ONCE = True
 
     @classmethod
+    @override
     def transform_query(cls, query: str):
         return prepare_listing_query(
             name_predicate=cls.name_predicate,
             filter=cls.filter,
             query=query
         )
 
     @classmethod
+    @override
     def get_by_id(cls, identifier: str) -> Record:
         return cls._create_lazy_record(identifier)
 
-    def fetch(self):
+    @override
+    def fetch_range(self, range_to_fetch: range) -> range:
+        # Fetch all records at one, because this is an expensive operation.
         if not self.prepared_query:
             raise ReaderError('First call prepare_query method')
+        if self.fetching_exhausted:
+            return range(0, 0)
         wrapper = SPARQLWrapper(self.endpoint)
         wrapper.setReturnFormat(JSONFormat)
         wrapper.setQuery(self.prepared_query)
         try:
             response = wrapper.queryAndConvert()
         except SPARQLExceptions.QueryBadFormed as err:
             raise ReaderError(
                 'Malformed SPARQL query: {}'.format(err)
             )
         assert isinstance(response, dict)
         results = response['results']['bindings']
-        self.records = []
+        self.records = {}
         self.number_of_results = len(results)
-        for result in results:
+        for i, result in enumerate(results):
             iri = result['s']['value']
             name = result['name']['value']
-            self.records.append(self._create_lazy_record(iri, name))
-        self.number_fetched = self.number_of_results
-
-    def fetch_next(self):
-        pass
+            self.records[i] = self._create_lazy_record(iri, name)
+        return range(0, self.number_of_results)
 
     @classmethod
     @abstractmethod
-    def _convert_record(cls, graph: Graph, record: Record) -> None:
+    def convert_record(cls, graph: Graph, record: Record) -> None:
         '''Convert data from an RDF graph to Fields in a Record. The 
         Record is changed in-place.'''
         pass
 
     @classmethod
     @abstractmethod
     def _create_lazy_record(cls, iri: str, name: Optional[str]=None) -> Record:
```

### Comparing `edpop-explorer-0.7.0/edpop_explorer/srumarc21reader.py` & `edpop_explorer-0.8.0/edpop_explorer/srumarc21reader.py`

 * *Files identical despite different names*

### Comparing `edpop-explorer-0.7.0/edpop_explorer/srureader.py` & `edpop_explorer-0.8.0/edpop_explorer/srureader.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 import requests
 from abc import abstractmethod
 from typing import List, Optional
 
 from edpop_explorer import Reader, Record, ReaderError
 from edpop_explorer.reader import GetByIdBasedOnQueryMixin
 
-RECORDS_PER_PAGE = 10
-
 
 class SRUReader(GetByIdBasedOnQueryMixin, Reader):
     '''Subclass of ``Reader`` that adds basic SRU functionality
     using the ``sruthi`` library.
 
     This class is still abstract and subclasses should implement
     the ``transform_query()`` and ``_convert_record()`` methods
@@ -30,14 +28,15 @@
     session: requests.Session
     '''The ``Session`` object of the ``requests`` library.'''
 
     def __init__(self):
         # Set a session to allow reuse of HTTP sessions and to set additional
         # parameters and settings, which some SRU APIs require -
         # see https://github.com/metaodi/sruthi#custom-parameters-and-settings
+        super().__init__()
         self.session = requests.Session()
 
     @classmethod
     @abstractmethod
     def transform_query(cls, query: str) -> str:
         pass
 
@@ -48,49 +47,49 @@
         (a subclass of) ``Record``.'''
         pass
 
     @classmethod
     def _prepare_get_by_id_query(cls, identifier: str) -> str:
         return cls.transform_query(identifier)
 
-    def _perform_query(self, start_record: int) -> List[Record]:
+    def _perform_query(self, start_record: int, maximum_records: Optional[int]) -> List[Record]:
+        if maximum_records is None:
+            maximum_records = self.DEFAULT_RECORDS_PER_PAGE
         try:
             response = sruthi.searchretrieve(
                 self.sru_url,
                 self.prepared_query,
                 start_record=start_record,
-                maximum_records=RECORDS_PER_PAGE,
+                maximum_records=maximum_records,
                 sru_version=self.sru_version,
                 session=self.session
             )
         except (
             sruthi.errors.SruError
         ) as err:
             raise ReaderError('Server returned error: ' + str(err))
 
         self.number_of_results = response.count
 
         records: List[Record] = []
-        for sruthirecord in response[0:RECORDS_PER_PAGE]:
+        for sruthirecord in response[0:maximum_records]:
             records.append(self._convert_record(sruthirecord))
 
         return records
 
     def prepare_query(self, query) -> None:
         self.prepared_query = self.transform_query(query)
 
-    def fetch(self) -> None:
-        self.records = []
+    def fetch_range(self, range_to_fetch: range) -> range:
+        # SRU provides paged retrieve using a start record (that starts at
+        # 1, while we start at 0) and a maximum number of results.
+        if self.fetching_exhausted:
+            return range(0, 0)
         if self.prepared_query is None:
             raise ReaderError('First call prepare_query')
-        results = self._perform_query(1)
-        self.records.extend(results)
-        self.number_fetched = len(self.records)
-
-    def fetch_next(self) -> None:
-        # TODO: can be merged with fetch method
-        if self.number_of_results == self.number_fetched:
-            return
-        start_record = len(self.records) + 1
-        results = self._perform_query(start_record)
-        self.records.extend(results)
-        self.number_fetched = len(self.records)
+        start_number = range_to_fetch.start
+        start_number_sru = start_number + 1  # SRU starts at 1
+        records_to_fetch = range_to_fetch.stop - range_to_fetch.start
+        results = self._perform_query(start_number_sru, records_to_fetch)
+        for i, result in enumerate(results):
+            self.records[i + start_number] = result
+        return range(start_number, start_number + len(results))
```

### Comparing `edpop-explorer-0.7.0/edpop_explorer.egg-info/PKG-INFO` & `edpop_explorer-0.8.0/edpop_explorer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edpop-explorer
-Version: 0.7.0
+Version: 0.8.0
 Summary: Common interface to multiple library catalogues and bibliographical databases
 Author-email: "Utrecht University, Centre for Digital Humanities - Research Software Lab" <cdh@uu.nl>
 Project-URL: Homepage, https://github.com/UUDigitalHumanitieslab/edpop-explorer
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -20,14 +20,15 @@
 Requires-Dist: pyreadline3; platform_system == "Windows"
 Requires-Dist: colorama; platform_system == "Windows"
 Requires-Dist: cmd2
 Requires-Dist: pyyaml
 Requires-Dist: rdflib<8,>=7.0.0
 Requires-Dist: Pygments
 Requires-Dist: xmltodict>=0.13.0
+Requires-Dist: typing_extensions
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 
 [![PyPI Version](https://img.shields.io/pypi/v/edpop-explorer)](https://pypi.org/project/edpop-explorer/) [![Tests](https://github.com/UUDigitalHumanitieslab/edpop-explorer/actions/workflows/test.yml/badge.svg)](https://github.com/UUDigitalHumanitieslab/edpop-explorer/actions/workflows/test.yml) [![Read the Docs](https://readthedocs.org/projects/edpop-explorer/badge/?version=latest&style=flat)](https://edpop-explorer.readthedocs.io/en/latest/)
```

### Comparing `edpop-explorer-0.7.0/edpop_explorer.egg-info/SOURCES.txt` & `edpop_explorer-0.8.0/edpop_explorer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edpop-explorer-0.7.0/pyproject.toml` & `edpop_explorer-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "edpop-explorer"
-version = "0.7.0"
+version = "0.8.0"
 authors = [
   {name="Utrecht University, Centre for Digital Humanities - Research Software Lab", email="cdh@uu.nl"}
 ]
 dependencies = [
   "sruthi>=2.0.0,<3",
   "termcolor",
   "appdirs",
@@ -16,14 +16,15 @@
   'pyreadline3 ; platform_system == "Windows"',
   'colorama ; platform_system == "Windows"',
   'cmd2',
   'pyyaml',
   'rdflib>=7.0.0,<8',
   'Pygments',
   'xmltodict>=0.13.0',
+  'typing_extensions',
 ]
 
 description = "Common interface to multiple library catalogues and bibliographical databases"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   'Development Status :: 2 - Pre-Alpha',
```

### Comparing `edpop-explorer-0.7.0/tests/test_field.py` & `edpop_explorer-0.8.0/tests/test_field.py`

 * *Files identical despite different names*

### Comparing `edpop-explorer-0.7.0/tests/test_record.py` & `edpop_explorer-0.8.0/tests/test_record.py`

 * *Files identical despite different names*

### Comparing `edpop-explorer-0.7.0/tests/test_srureader.py` & `edpop_explorer-0.8.0/tests/test_srureader.py`

 * *Files identical despite different names*

