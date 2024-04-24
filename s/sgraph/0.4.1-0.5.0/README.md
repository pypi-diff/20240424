# Comparing `tmp/sgraph-0.4.1.tar.gz` & `tmp/sgraph-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sgraph-0.4.1.tar", last modified: Mon Mar 25 12:45:57 2024, max compression
+gzip compressed data, was "sgraph-0.5.0.tar", last modified: Wed Apr 24 21:31:31 2024, max compression
```

## Comparing `sgraph-0.4.1.tar` & `sgraph-0.5.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxr-x   0 ville     (1001) ville     (1001)        0 2024-03-25 12:45:57.664832 sgraph-0.4.1/
--rw-rw-r--   0 ville     (1001) ville     (1001)     1054 2021-05-06 19:05:39.000000 sgraph-0.4.1/LICENSE
--rw-rw-r--   0 ville     (1001) ville     (1001)       42 2023-03-01 16:27:00.000000 sgraph-0.4.1/MANIFEST.in
--rw-rw-r--   0 ville     (1001) ville     (1001)     4286 2024-03-25 12:45:57.664832 sgraph-0.4.1/PKG-INFO
--rw-rw-r--   0 ville     (1001) ville     (1001)     3584 2024-02-08 14:16:11.000000 sgraph-0.4.1/README.md
--rw-rw-r--   0 ville     (1001) ville     (1001)      880 2024-03-25 12:45:57.664832 sgraph-0.4.1/setup.cfg
--rw-rw-r--   0 ville     (1001) ville     (1001)       36 2023-01-25 23:13:09.000000 sgraph-0.4.1/setup.py
-drwxrwxr-x   0 ville     (1001) ville     (1001)        0 2024-03-25 12:45:57.652832 sgraph-0.4.1/src/
-drwxrwxr-x   0 ville     (1001) ville     (1001)        0 2024-03-25 12:45:57.656832 sgraph-0.4.1/src/sgraph/
--rw-rw-r--   0 ville     (1001) ville     (1001)      285 2023-04-20 22:26:43.000000 sgraph-0.4.1/src/sgraph/__init__.py
-drwxrwxr-x   0 ville     (1001) ville     (1001)        0 2024-03-25 12:45:57.656832 sgraph-0.4.1/src/sgraph/algorithms/
--rw-rw-r--   0 ville     (1001) ville     (1001)        0 2023-04-20 22:26:44.000000 sgraph-0.4.1/src/sgraph/algorithms/__init__.py
--rw-rw-r--   0 ville     (1001) ville     (1001)        1 2023-04-20 22:26:45.000000 sgraph-0.4.1/src/sgraph/algorithms/graphutils.py
--rw-rw-r--   0 ville     (1001) ville     (1001)      452 2023-04-20 22:26:52.000000 sgraph-0.4.1/src/sgraph/algorithms/selementutils.py
--rw-rw-r--   0 ville     (1001) ville     (1001)     4663 2024-02-08 14:16:29.000000 sgraph-0.4.1/src/sgraph/algorithms/sgraphanalysis.py
--rw-rw-r--   0 ville     (1001) ville     (1001)     3195 2024-02-08 14:16:29.000000 sgraph-0.4.1/src/sgraph/algorithms/sgraphfiltering.py
-drwxrwxr-x   0 ville     (1001) ville     (1001)        0 2024-03-25 12:45:57.660832 sgraph-0.4.1/src/sgraph/attributes/
--rw-rw-r--   0 ville     (1001) ville     (1001)        0 2023-04-20 22:26:55.000000 sgraph-0.4.1/src/sgraph/attributes/__init__.py
--rw-rw-r--   0 ville     (1001) ville     (1001)    19473 2024-02-08 14:16:29.000000 sgraph-0.4.1/src/sgraph/attributes/attributequeries.py
-drwxrwxr-x   0 ville     (1001) ville     (1001)        0 2024-03-25 12:45:57.660832 sgraph-0.4.1/src/sgraph/cli/
--rw-rw-r--   0 ville     (1001) ville     (1001)        0 2023-04-20 22:27:44.000000 sgraph-0.4.1/src/sgraph/cli/__init__.py
--rw-rw-r--   0 ville     (1001) ville     (1001)     2733 2023-04-20 22:27:44.000000 sgraph-0.4.1/src/sgraph/cli/filter_deps.py
--rw-rw-r--   0 ville     (1001) ville     (1001)     2172 2023-04-20 22:27:45.000000 sgraph-0.4.1/src/sgraph/cli/modelinfo_prettyprinter.py
--rw-rw-r--   0 ville     (1001) ville     (1001)     1850 2023-04-20 22:27:46.000000 sgraph-0.4.1/src/sgraph/cli/show_model.py
-drwxrwxr-x   0 ville     (1001) ville     (1001)        0 2024-03-25 12:45:57.660832 sgraph-0.4.1/src/sgraph/compare/
--rw-rw-r--   0 ville     (1001) ville     (1001)        0 2023-04-20 22:27:46.000000 sgraph-0.4.1/src/sgraph/compare/__init__.py
--rw-rw-r--   0 ville     (1001) ville     (1001)      194 2023-04-20 22:27:47.000000 sgraph-0.4.1/src/sgraph/compare/comparegraphattrs.py
--rw-rw-r--   0 ville     (1001) ville     (1001)    42258 2024-02-08 14:16:29.000000 sgraph-0.4.1/src/sgraph/compare/modelcompare.py
-drwxrwxr-x   0 ville     (1001) ville     (1001)        0 2024-03-25 12:45:57.664832 sgraph-0.4.1/src/sgraph/converters/
--rw-rw-r--   0 ville     (1001) ville     (1001)        0 2023-04-20 22:27:48.000000 sgraph-0.4.1/src/sgraph/converters/__init__.py
--rw-rw-r--   0 ville     (1001) ville     (1001)      344 2023-04-20 22:27:49.000000 sgraph-0.4.1/src/sgraph/converters/deps_to_xml.py
--rw-rw-r--   0 ville     (1001) ville     (1001)    19855 2023-08-28 15:38:52.000000 sgraph-0.4.1/src/sgraph/converters/graphml.py
--rw-rw-r--   0 ville     (1001) ville     (1001)      372 2023-04-20 22:27:50.000000 sgraph-0.4.1/src/sgraph/converters/graphml_to_xml.py
--rw-rw-r--   0 ville     (1001) ville     (1001)    13276 2024-02-08 14:16:29.000000 sgraph-0.4.1/src/sgraph/converters/sbom_cyclonedx_generator.py
--rw-rw-r--   0 ville     (1001) ville     (1001)     1998 2024-02-08 14:16:29.000000 sgraph-0.4.1/src/sgraph/converters/sgraph_json.py
--rw-rw-r--   0 ville     (1001) ville     (1001)     2773 2024-02-08 14:16:29.000000 sgraph-0.4.1/src/sgraph/converters/sgraph_to_cytoscape.py
--rw-rw-r--   0 ville     (1001) ville     (1001)     1472 2024-02-08 14:16:29.000000 sgraph-0.4.1/src/sgraph/converters/xml_to_3dforcegraph.py
--rw-rw-r--   0 ville     (1001) ville     (1001)      344 2023-04-20 22:27:52.000000 sgraph-0.4.1/src/sgraph/converters/xml_to_deps.py
--rw-rw-r--   0 ville     (1001) ville     (1001)     1295 2023-04-20 22:27:52.000000 sgraph-0.4.1/src/sgraph/converters/xml_to_dot.py
--rw-rw-r--   0 ville     (1001) ville     (1001)      167 2023-04-20 22:27:53.000000 sgraph-0.4.1/src/sgraph/converters/xml_to_graphml.py
--rw-rw-r--   0 ville     (1001) ville     (1001)      163 2024-02-08 14:16:29.000000 sgraph-0.4.1/src/sgraph/converters/xml_to_hierarchical_json.py
--rw-rw-r--   0 ville     (1001) ville     (1001)     3382 2024-02-08 14:16:29.000000 sgraph-0.4.1/src/sgraph/converters/xml_to_json.py
--rw-rw-r--   0 ville     (1001) ville     (1001)      348 2023-04-20 22:27:54.000000 sgraph-0.4.1/src/sgraph/converters/xml_to_plantuml.py
--rw-rw-r--   0 ville     (1001) ville     (1001)      233 2023-04-20 22:27:54.000000 sgraph-0.4.1/src/sgraph/exceptions.py
--rw-rw-r--   0 ville     (1001) ville     (1001)     2424 2023-04-20 22:27:55.000000 sgraph-0.4.1/src/sgraph/graphdataservice.py
-drwxrwxr-x   0 ville     (1001) ville     (1001)        0 2024-03-25 12:45:57.664832 sgraph-0.4.1/src/sgraph/loader/
--rw-rw-r--   0 ville     (1001) ville     (1001)      108 2023-04-20 22:27:55.000000 sgraph-0.4.1/src/sgraph/loader/__init__.py
--rw-rw-r--   0 ville     (1001) ville     (1001)     2110 2023-04-20 22:27:56.000000 sgraph-0.4.1/src/sgraph/loader/attributeloader.py
--rw-rw-r--   0 ville     (1001) ville     (1001)     4371 2023-08-28 15:38:52.000000 sgraph-0.4.1/src/sgraph/loader/modelloader.py
--rw-rw-r--   0 ville     (1001) ville     (1001)     5644 2023-08-28 15:38:52.000000 sgraph-0.4.1/src/sgraph/metricsapi.py
--rw-rw-r--   0 ville     (1001) ville     (1001)    10928 2024-02-08 14:16:29.000000 sgraph-0.4.1/src/sgraph/modelapi.py
--rw-rw-r--   0 ville     (1001) ville     (1001)    22984 2024-02-08 14:16:29.000000 sgraph-0.4.1/src/sgraph/selement.py
--rw-rw-r--   0 ville     (1001) ville     (1001)     5592 2023-08-28 15:38:52.000000 sgraph-0.4.1/src/sgraph/selementassociation.py
--rw-rw-r--   0 ville     (1001) ville     (1001)    39570 2024-03-25 12:40:33.000000 sgraph-0.4.1/src/sgraph/sgraph.py
-drwxrwxr-x   0 ville     (1001) ville     (1001)        0 2024-03-25 12:45:57.656832 sgraph-0.4.1/src/sgraph.egg-info/
--rw-rw-r--   0 ville     (1001) ville     (1001)     4286 2024-03-25 12:45:57.000000 sgraph-0.4.1/src/sgraph.egg-info/PKG-INFO
--rw-rw-r--   0 ville     (1001) ville     (1001)     1584 2024-03-25 12:45:57.000000 sgraph-0.4.1/src/sgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 ville     (1001) ville     (1001)        1 2024-03-25 12:45:57.000000 sgraph-0.4.1/src/sgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 ville     (1001) ville     (1001)       39 2024-03-25 12:45:57.000000 sgraph-0.4.1/src/sgraph.egg-info/requires.txt
--rw-rw-r--   0 ville     (1001) ville     (1001)        7 2024-03-25 12:45:57.000000 sgraph-0.4.1/src/sgraph.egg-info/top_level.txt
+drwxrwxr-x   0 ville     (1001) ville     (1001)        0 2024-04-24 21:31:31.019332 sgraph-0.5.0/
+-rw-rw-r--   0 ville     (1001) ville     (1001)     1054 2021-05-06 19:05:39.000000 sgraph-0.5.0/LICENSE
+-rw-rw-r--   0 ville     (1001) ville     (1001)       42 2023-03-01 16:27:00.000000 sgraph-0.5.0/MANIFEST.in
+-rw-rw-r--   0 ville     (1001) ville     (1001)     4286 2024-04-24 21:31:31.019332 sgraph-0.5.0/PKG-INFO
+-rw-rw-r--   0 ville     (1001) ville     (1001)     3584 2024-02-08 14:16:11.000000 sgraph-0.5.0/README.md
+-rw-rw-r--   0 ville     (1001) ville     (1001)      880 2024-04-24 21:31:31.019332 sgraph-0.5.0/setup.cfg
+-rw-rw-r--   0 ville     (1001) ville     (1001)       36 2023-01-25 23:13:09.000000 sgraph-0.5.0/setup.py
+drwxrwxr-x   0 ville     (1001) ville     (1001)        0 2024-04-24 21:31:31.003332 sgraph-0.5.0/src/
+drwxrwxr-x   0 ville     (1001) ville     (1001)        0 2024-04-24 21:31:31.007332 sgraph-0.5.0/src/sgraph/
+-rw-rw-r--   0 ville     (1001) ville     (1001)      285 2023-04-20 22:26:43.000000 sgraph-0.5.0/src/sgraph/__init__.py
+drwxrwxr-x   0 ville     (1001) ville     (1001)        0 2024-04-24 21:31:31.011332 sgraph-0.5.0/src/sgraph/algorithms/
+-rw-rw-r--   0 ville     (1001) ville     (1001)        0 2023-04-20 22:26:44.000000 sgraph-0.5.0/src/sgraph/algorithms/__init__.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)        1 2023-04-20 22:26:45.000000 sgraph-0.5.0/src/sgraph/algorithms/graphutils.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)      452 2023-04-20 22:26:52.000000 sgraph-0.5.0/src/sgraph/algorithms/selementutils.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)     4663 2024-02-08 14:16:29.000000 sgraph-0.5.0/src/sgraph/algorithms/sgraphanalysis.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)     3195 2024-02-08 14:16:29.000000 sgraph-0.5.0/src/sgraph/algorithms/sgraphfiltering.py
+drwxrwxr-x   0 ville     (1001) ville     (1001)        0 2024-04-24 21:31:31.011332 sgraph-0.5.0/src/sgraph/attributes/
+-rw-rw-r--   0 ville     (1001) ville     (1001)        0 2023-04-20 22:26:55.000000 sgraph-0.5.0/src/sgraph/attributes/__init__.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)    19473 2024-02-08 14:16:29.000000 sgraph-0.5.0/src/sgraph/attributes/attributequeries.py
+drwxrwxr-x   0 ville     (1001) ville     (1001)        0 2024-04-24 21:31:31.011332 sgraph-0.5.0/src/sgraph/cli/
+-rw-rw-r--   0 ville     (1001) ville     (1001)        0 2023-04-20 22:27:44.000000 sgraph-0.5.0/src/sgraph/cli/__init__.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)     2733 2023-04-20 22:27:44.000000 sgraph-0.5.0/src/sgraph/cli/filter_deps.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)     2172 2023-04-20 22:27:45.000000 sgraph-0.5.0/src/sgraph/cli/modelinfo_prettyprinter.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)     1850 2023-04-20 22:27:46.000000 sgraph-0.5.0/src/sgraph/cli/show_model.py
+drwxrwxr-x   0 ville     (1001) ville     (1001)        0 2024-04-24 21:31:31.011332 sgraph-0.5.0/src/sgraph/compare/
+-rw-rw-r--   0 ville     (1001) ville     (1001)        0 2023-04-20 22:27:46.000000 sgraph-0.5.0/src/sgraph/compare/__init__.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)      194 2023-04-20 22:27:47.000000 sgraph-0.5.0/src/sgraph/compare/comparegraphattrs.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)    42258 2024-02-08 14:16:29.000000 sgraph-0.5.0/src/sgraph/compare/modelcompare.py
+drwxrwxr-x   0 ville     (1001) ville     (1001)        0 2024-04-24 21:31:31.019332 sgraph-0.5.0/src/sgraph/converters/
+-rw-rw-r--   0 ville     (1001) ville     (1001)        0 2023-04-20 22:27:48.000000 sgraph-0.5.0/src/sgraph/converters/__init__.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)      344 2023-04-20 22:27:49.000000 sgraph-0.5.0/src/sgraph/converters/deps_to_xml.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)    19855 2023-08-28 15:38:52.000000 sgraph-0.5.0/src/sgraph/converters/graphml.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)      372 2023-04-20 22:27:50.000000 sgraph-0.5.0/src/sgraph/converters/graphml_to_xml.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)    13276 2024-02-08 14:16:29.000000 sgraph-0.5.0/src/sgraph/converters/sbom_cyclonedx_generator.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)     1998 2024-02-08 14:16:29.000000 sgraph-0.5.0/src/sgraph/converters/sgraph_json.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)     2773 2024-02-08 14:16:29.000000 sgraph-0.5.0/src/sgraph/converters/sgraph_to_cytoscape.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)     1472 2024-02-08 14:16:29.000000 sgraph-0.5.0/src/sgraph/converters/xml_to_3dforcegraph.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)      344 2023-04-20 22:27:52.000000 sgraph-0.5.0/src/sgraph/converters/xml_to_deps.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)     1295 2023-04-20 22:27:52.000000 sgraph-0.5.0/src/sgraph/converters/xml_to_dot.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)      167 2023-04-20 22:27:53.000000 sgraph-0.5.0/src/sgraph/converters/xml_to_graphml.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)      163 2024-02-08 14:16:29.000000 sgraph-0.5.0/src/sgraph/converters/xml_to_hierarchical_json.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)     3382 2024-02-08 14:16:29.000000 sgraph-0.5.0/src/sgraph/converters/xml_to_json.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)      348 2023-04-20 22:27:54.000000 sgraph-0.5.0/src/sgraph/converters/xml_to_plantuml.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)      233 2023-04-20 22:27:54.000000 sgraph-0.5.0/src/sgraph/exceptions.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)     2424 2023-04-20 22:27:55.000000 sgraph-0.5.0/src/sgraph/graphdataservice.py
+drwxrwxr-x   0 ville     (1001) ville     (1001)        0 2024-04-24 21:31:31.019332 sgraph-0.5.0/src/sgraph/loader/
+-rw-rw-r--   0 ville     (1001) ville     (1001)      108 2023-04-20 22:27:55.000000 sgraph-0.5.0/src/sgraph/loader/__init__.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)     2135 2024-04-24 21:28:26.000000 sgraph-0.5.0/src/sgraph/loader/attributeloader.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)     4371 2023-08-28 15:38:52.000000 sgraph-0.5.0/src/sgraph/loader/modelloader.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)     5644 2023-08-28 15:38:52.000000 sgraph-0.5.0/src/sgraph/metricsapi.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)    10928 2024-02-08 14:16:29.000000 sgraph-0.5.0/src/sgraph/modelapi.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)    22984 2024-02-08 14:16:29.000000 sgraph-0.5.0/src/sgraph/selement.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)     5592 2023-08-28 15:38:52.000000 sgraph-0.5.0/src/sgraph/selementassociation.py
+-rw-rw-r--   0 ville     (1001) ville     (1001)    39002 2024-04-24 21:28:26.000000 sgraph-0.5.0/src/sgraph/sgraph.py
+drwxrwxr-x   0 ville     (1001) ville     (1001)        0 2024-04-24 21:31:31.007332 sgraph-0.5.0/src/sgraph.egg-info/
+-rw-rw-r--   0 ville     (1001) ville     (1001)     4286 2024-04-24 21:31:30.000000 sgraph-0.5.0/src/sgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 ville     (1001) ville     (1001)     1584 2024-04-24 21:31:30.000000 sgraph-0.5.0/src/sgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 ville     (1001) ville     (1001)        1 2024-04-24 21:31:30.000000 sgraph-0.5.0/src/sgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 ville     (1001) ville     (1001)       39 2024-04-24 21:31:30.000000 sgraph-0.5.0/src/sgraph.egg-info/requires.txt
+-rw-rw-r--   0 ville     (1001) ville     (1001)        7 2024-04-24 21:31:30.000000 sgraph-0.5.0/src/sgraph.egg-info/top_level.txt
```

### Comparing `sgraph-0.4.1/LICENSE` & `sgraph-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sgraph-0.4.1/PKG-INFO` & `sgraph-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgraph
-Version: 0.4.1
+Version: 0.5.0
 Summary: sgraph hierarchic graph data structure, format and algorithms
 Home-page: https://github.com/softagram/sgraph
 Author: Ville Laitila
 Author-email: ville.laitila@softagram.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/softagram/sgraph/issues
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sgraph-0.4.1/README.md` & `sgraph-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `sgraph-0.4.1/setup.cfg` & `sgraph-0.5.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sgraph
-version = 0.4.1
+version = 0.5.0
 description = sgraph hierarchic graph data structure, format and algorithms
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/softagram/sgraph
 author = Ville Laitila
 author_email = ville.laitila@softagram.com
 license = MIT
```

### Comparing `sgraph-0.4.1/src/sgraph/algorithms/sgraphanalysis.py` & `sgraph-0.5.0/src/sgraph/algorithms/sgraphanalysis.py`

 * *Files identical despite different names*

### Comparing `sgraph-0.4.1/src/sgraph/algorithms/sgraphfiltering.py` & `sgraph-0.5.0/src/sgraph/algorithms/sgraphfiltering.py`

 * *Files identical despite different names*

### Comparing `sgraph-0.4.1/src/sgraph/attributes/attributequeries.py` & `sgraph-0.5.0/src/sgraph/attributes/attributequeries.py`

 * *Files identical despite different names*

### Comparing `sgraph-0.4.1/src/sgraph/cli/filter_deps.py` & `sgraph-0.5.0/src/sgraph/cli/filter_deps.py`

 * *Files identical despite different names*

### Comparing `sgraph-0.4.1/src/sgraph/cli/modelinfo_prettyprinter.py` & `sgraph-0.5.0/src/sgraph/cli/modelinfo_prettyprinter.py`

 * *Files identical despite different names*

### Comparing `sgraph-0.4.1/src/sgraph/cli/show_model.py` & `sgraph-0.5.0/src/sgraph/cli/show_model.py`

 * *Files identical despite different names*

### Comparing `sgraph-0.4.1/src/sgraph/compare/modelcompare.py` & `sgraph-0.5.0/src/sgraph/compare/modelcompare.py`

 * *Files identical despite different names*

### Comparing `sgraph-0.4.1/src/sgraph/converters/graphml.py` & `sgraph-0.5.0/src/sgraph/converters/graphml.py`

 * *Files identical despite different names*

### Comparing `sgraph-0.4.1/src/sgraph/converters/sbom_cyclonedx_generator.py` & `sgraph-0.5.0/src/sgraph/converters/sbom_cyclonedx_generator.py`

 * *Files identical despite different names*

### Comparing `sgraph-0.4.1/src/sgraph/converters/sgraph_json.py` & `sgraph-0.5.0/src/sgraph/converters/sgraph_json.py`

 * *Files identical despite different names*

### Comparing `sgraph-0.4.1/src/sgraph/converters/sgraph_to_cytoscape.py` & `sgraph-0.5.0/src/sgraph/converters/sgraph_to_cytoscape.py`

 * *Files identical despite different names*

### Comparing `sgraph-0.4.1/src/sgraph/converters/xml_to_3dforcegraph.py` & `sgraph-0.5.0/src/sgraph/converters/xml_to_3dforcegraph.py`

 * *Files identical despite different names*

### Comparing `sgraph-0.4.1/src/sgraph/converters/xml_to_dot.py` & `sgraph-0.5.0/src/sgraph/converters/xml_to_dot.py`

 * *Files identical despite different names*

### Comparing `sgraph-0.4.1/src/sgraph/converters/xml_to_json.py` & `sgraph-0.5.0/src/sgraph/converters/xml_to_json.py`

 * *Files identical despite different names*

### Comparing `sgraph-0.4.1/src/sgraph/graphdataservice.py` & `sgraph-0.5.0/src/sgraph/graphdataservice.py`

 * *Files identical despite different names*

### Comparing `sgraph-0.4.1/src/sgraph/loader/attributeloader.py` & `sgraph-0.5.0/src/sgraph/loader/attributeloader.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 
     # noinspection PyMethodMayBeStatic
     def load_attrfile(self, filepath, model: SGraph):
         columns, entries = attributequeries.read_attrs_generic(filepath)
         for elem_path, attrs in entries:
             if isinstance(elem_path, int):
                 raise Exception(f'Invalid attribute file {filepath} as id {elem_path} is numeric..')
+            elem = model.createOrGetElementFromPath(elem_path)
             for c in columns:
                 val = attrs[c]
                 if not isinstance(val, str):
                     val = '' if math.isnan(val) else val
-                model.createOrGetElementFromPath(elem_path).addAttribute(c, val)
+
+                elem.addAttribute(c, val)
 
         return model
 
     def load_all_files(self, model, filepath_of_model_root):
 
         attrfiles = ['attr_temporary.csv', 'git/attr_git_propagated.csv',
                      'git/attr_analysis_state.csv', 'content/loc/attr_loc_propagated.csv',
```

### Comparing `sgraph-0.4.1/src/sgraph/loader/modelloader.py` & `sgraph-0.5.0/src/sgraph/loader/modelloader.py`

 * *Files identical despite different names*

### Comparing `sgraph-0.4.1/src/sgraph/metricsapi.py` & `sgraph-0.5.0/src/sgraph/metricsapi.py`

 * *Files identical despite different names*

### Comparing `sgraph-0.4.1/src/sgraph/modelapi.py` & `sgraph-0.5.0/src/sgraph/modelapi.py`

 * *Files identical despite different names*

### Comparing `sgraph-0.4.1/src/sgraph/selement.py` & `sgraph-0.5.0/src/sgraph/selement.py`

 * *Files identical despite different names*

### Comparing `sgraph-0.4.1/src/sgraph/selementassociation.py` & `sgraph-0.5.0/src/sgraph/selementassociation.py`

 * *Files identical despite different names*

### Comparing `sgraph-0.4.1/src/sgraph/sgraph.py` & `sgraph-0.5.0/src/sgraph/sgraph.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 import sys
 import uuid
 import xml.sax.handler
 import zipfile
 from typing import Optional
 from xml.sax import parseString
 
-import deprecation
-
 from .selement import SElement
 from .selementassociation import SElementAssociation
 
 
 def addEA(deptype, info, id1, id2, egm):
     e1 = None
     if not id1.startswith('generate dependency'):
@@ -63,27 +61,14 @@
         self.metaAttrs = {}
         self.propagateActions = []
         self.totalModel = None
 
     def addPropagateAction(self, a, v):
         self.propagateActions.append((a, v))
 
-    @deprecation.deprecated(deprecated_in="0.4.1", removed_in="0.5",
-                            current_version=deprecation.__version__,
-                            details="Use either findElementFromPath or createOrGetElementFromPath instead of this.")
-    def getElementFromPath(self, i):
-        if i.startswith('/'):
-            i = i[1:]
-        if '/' not in i:
-            return self.rootNode.getChildByName(i)
-        elif len(i) > 0:
-            e = self.rootNode.createOrGetElement(i)
-            return e
-        return self.rootNode
-
     def createOrGetElementFromPath(self, path: str):
         """
         Create or get existing element based on element path.
         """
         if path.startswith('/'):
             path = path[1:]
         if '/' not in path:
```

### Comparing `sgraph-0.4.1/src/sgraph.egg-info/PKG-INFO` & `sgraph-0.5.0/src/sgraph.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgraph
-Version: 0.4.1
+Version: 0.5.0
 Summary: sgraph hierarchic graph data structure, format and algorithms
 Home-page: https://github.com/softagram/sgraph
 Author: Ville Laitila
 Author-email: ville.laitila@softagram.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/softagram/sgraph/issues
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sgraph-0.4.1/src/sgraph.egg-info/SOURCES.txt` & `sgraph-0.5.0/src/sgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

