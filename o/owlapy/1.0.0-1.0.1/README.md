# Comparing `tmp/owlapy-1.0.0.tar.gz` & `tmp/owlapy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owlapy-1.0.0.tar", last modified: Fri Apr 19 11:40:23 2024, max compression
+gzip compressed data, was "owlapy-1.0.1.tar", last modified: Wed Apr 24 11:41:15 2024, max compression
```

## Comparing `owlapy-1.0.0.tar` & `owlapy-1.0.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 11:40:23.397060 owlapy-1.0.0/
--rw-rw-rw-   0        0        0     1077 2023-05-27 17:20:12.000000 owlapy-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3808 2024-04-19 11:40:23.396046 owlapy-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3144 2024-04-17 13:17:23.000000 owlapy-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-19 11:40:23.375542 owlapy-1.0.0/owlapy/
--rw-rw-rw-   0        0        0      216 2024-04-18 12:50:47.000000 owlapy-1.0.0/owlapy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 11:40:23.384502 owlapy-1.0.0/owlapy/class_expression/
--rw-rw-rw-   0        0        0     2258 2024-04-17 12:42:17.000000 owlapy-1.0.0/owlapy/class_expression/__init__.py
--rw-rw-rw-   0        0        0     3657 2024-04-17 14:23:56.000000 owlapy-1.0.0/owlapy/class_expression/class_expression.py
--rw-rw-rw-   0        0        0     1889 2024-04-15 18:25:40.000000 owlapy-1.0.0/owlapy/class_expression/nary_boolean_expression.py
--rw-rw-rw-   0        0        0     1653 2024-04-17 12:30:02.000000 owlapy-1.0.0/owlapy/class_expression/owl_class.py
--rw-rw-rw-   0        0        0    31671 2024-04-17 14:23:56.000000 owlapy-1.0.0/owlapy/class_expression/restriction.py
--rw-rw-rw-   0        0        0    24825 2024-04-17 11:25:38.000000 owlapy-1.0.0/owlapy/converter.py
-drwxrwxrwx   0        0        0        0 2024-04-19 11:40:23.386542 owlapy-1.0.0/owlapy/entities/
--rw-rw-rw-   0        0        0      493 2024-04-10 12:11:02.000000 owlapy-1.0.0/owlapy/entities/__init__.py
--rw-rw-rw-   0        0        0     5514 2024-04-17 12:42:17.000000 owlapy-1.0.0/owlapy/iri.py
--rw-rw-rw-   0        0        0     2094 2024-04-17 12:42:17.000000 owlapy-1.0.0/owlapy/meta_classes.py
--rw-rw-rw-   0        0        0     1501 2024-04-11 16:18:42.000000 owlapy-1.0.0/owlapy/namespaces.py
--rw-rw-rw-   0        0        0     1518 2024-04-17 11:21:40.000000 owlapy-1.0.0/owlapy/owl_annotation.py
--rw-rw-rw-   0        0        0    56408 2024-04-17 12:10:21.000000 owlapy-1.0.0/owlapy/owl_axiom.py
--rw-rw-rw-   0        0        0     3402 2024-04-17 14:26:54.000000 owlapy-1.0.0/owlapy/owl_data_ranges.py
--rw-rw-rw-   0        0        0     1396 2024-04-17 14:23:56.000000 owlapy-1.0.0/owlapy/owl_datatype.py
--rw-rw-rw-   0        0        0     1306 2024-04-17 12:30:02.000000 owlapy-1.0.0/owlapy/owl_individual.py
--rw-rw-rw-   0        0        0    16664 2024-04-17 12:48:36.000000 owlapy-1.0.0/owlapy/owl_literal.py
--rw-rw-rw-   0        0        0     2548 2024-04-17 12:48:36.000000 owlapy-1.0.0/owlapy/owl_object.py
--rw-rw-rw-   0        0        0     8206 2024-04-17 11:21:41.000000 owlapy-1.0.0/owlapy/owl_ontology.py
--rw-rw-rw-   0        0        0     5102 2024-04-17 14:11:30.000000 owlapy-1.0.0/owlapy/owl_ontology_manager.py
--rw-rw-rw-   0        0        0     6334 2024-04-18 14:19:00.000000 owlapy-1.0.0/owlapy/owl_property.py
--rw-rw-rw-   0        0        0    19537 2024-04-15 19:10:09.000000 owlapy-1.0.0/owlapy/owl_reasoner.py
--rw-rw-rw-   0        0        0    37465 2024-04-17 14:23:56.000000 owlapy-1.0.0/owlapy/parser.py
--rw-rw-rw-   0        0        0     2882 2024-04-15 19:24:04.000000 owlapy-1.0.0/owlapy/providers.py
--rw-rw-rw-   0        0        0    16389 2024-04-17 14:23:56.000000 owlapy-1.0.0/owlapy/render.py
--rw-rw-rw-   0        0        0    22897 2024-04-17 14:23:56.000000 owlapy-1.0.0/owlapy/util.py
--rw-rw-rw-   0        0        0     4601 2024-04-17 12:10:21.000000 owlapy-1.0.0/owlapy/vocab.py
-drwxrwxrwx   0        0        0        0 2024-04-19 11:40:23.394013 owlapy-1.0.0/owlapy.egg-info/
--rw-rw-rw-   0        0        0     3808 2024-04-19 11:40:23.000000 owlapy-1.0.0/owlapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1064 2024-04-19 11:40:23.000000 owlapy-1.0.0/owlapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 11:40:23.000000 owlapy-1.0.0/owlapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-04-19 11:40:23.000000 owlapy-1.0.0/owlapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-19 11:40:23.000000 owlapy-1.0.0/owlapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2023-11-14 15:09:44.000000 owlapy-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-19 11:40:23.397060 owlapy-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      885 2024-04-18 12:44:58.000000 owlapy-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-19 11:40:23.392823 owlapy-1.0.0/tests/
--rw-rw-rw-   0        0        0     1045 2024-04-15 19:24:04.000000 owlapy-1.0.0/tests/test_class_expression_semantics.py
--rw-rw-rw-   0        0        0     1318 2024-04-15 19:24:04.000000 owlapy-1.0.0/tests/test_examples.py
--rw-rw-rw-   0        0        0     1693 2024-04-15 19:50:32.000000 owlapy-1.0.0/tests/test_owlapy.py
--rw-rw-rw-   0        0        0    11461 2024-04-15 19:50:32.000000 owlapy-1.0.0/tests/test_owlapy_cnf_dnf.py
--rw-rw-rw-   0        0        0    18720 2024-04-17 14:24:48.000000 owlapy-1.0.0/tests/test_owlapy_nnf.py
--rw-rw-rw-   0        0        0    30821 2024-04-17 14:24:48.000000 owlapy-1.0.0/tests/test_owlapy_parser.py
--rw-rw-rw-   0        0        0     8940 2024-04-17 14:24:48.000000 owlapy-1.0.0/tests/test_owlapy_render.py
+drwxrwxrwx   0        0        0        0 2024-04-24 11:41:15.490144 owlapy-1.0.1/
+-rw-rw-rw-   0        0        0     1077 2023-05-27 17:20:12.000000 owlapy-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     3808 2024-04-24 11:41:15.489143 owlapy-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3144 2024-04-17 13:17:23.000000 owlapy-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 11:41:15.468271 owlapy-1.0.1/owlapy/
+-rw-rw-rw-   0        0        0      216 2024-04-18 12:50:47.000000 owlapy-1.0.1/owlapy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 11:41:15.477849 owlapy-1.0.1/owlapy/class_expression/
+-rw-rw-rw-   0        0        0     2258 2024-04-17 12:42:17.000000 owlapy-1.0.1/owlapy/class_expression/__init__.py
+-rw-rw-rw-   0        0        0     3657 2024-04-17 14:23:56.000000 owlapy-1.0.1/owlapy/class_expression/class_expression.py
+-rw-rw-rw-   0        0        0     1889 2024-04-15 18:25:40.000000 owlapy-1.0.1/owlapy/class_expression/nary_boolean_expression.py
+-rw-rw-rw-   0        0        0     1653 2024-04-17 12:30:02.000000 owlapy-1.0.1/owlapy/class_expression/owl_class.py
+-rw-rw-rw-   0        0        0    31689 2024-04-23 13:32:17.000000 owlapy-1.0.1/owlapy/class_expression/restriction.py
+-rw-rw-rw-   0        0        0    24825 2024-04-17 11:25:38.000000 owlapy-1.0.1/owlapy/converter.py
+drwxrwxrwx   0        0        0        0 2024-04-24 11:41:15.479075 owlapy-1.0.1/owlapy/entities/
+-rw-rw-rw-   0        0        0      493 2024-04-10 12:11:02.000000 owlapy-1.0.1/owlapy/entities/__init__.py
+-rw-rw-rw-   0        0        0     5514 2024-04-17 12:42:17.000000 owlapy-1.0.1/owlapy/iri.py
+-rw-rw-rw-   0        0        0     2094 2024-04-17 12:42:17.000000 owlapy-1.0.1/owlapy/meta_classes.py
+-rw-rw-rw-   0        0        0     1501 2024-04-11 16:18:42.000000 owlapy-1.0.1/owlapy/namespaces.py
+-rw-rw-rw-   0        0        0     1518 2024-04-17 11:21:40.000000 owlapy-1.0.1/owlapy/owl_annotation.py
+-rw-rw-rw-   0        0        0    56484 2024-04-23 13:32:17.000000 owlapy-1.0.1/owlapy/owl_axiom.py
+-rw-rw-rw-   0        0        0     3402 2024-04-17 14:26:54.000000 owlapy-1.0.1/owlapy/owl_data_ranges.py
+-rw-rw-rw-   0        0        0     1396 2024-04-17 14:23:56.000000 owlapy-1.0.1/owlapy/owl_datatype.py
+-rw-rw-rw-   0        0        0     1306 2024-04-17 12:30:02.000000 owlapy-1.0.1/owlapy/owl_individual.py
+-rw-rw-rw-   0        0        0    16664 2024-04-17 12:48:36.000000 owlapy-1.0.1/owlapy/owl_literal.py
+-rw-rw-rw-   0        0        0     2548 2024-04-17 12:48:36.000000 owlapy-1.0.1/owlapy/owl_object.py
+-rw-rw-rw-   0        0        0     8206 2024-04-17 11:21:41.000000 owlapy-1.0.1/owlapy/owl_ontology.py
+-rw-rw-rw-   0        0        0     5102 2024-04-17 14:11:30.000000 owlapy-1.0.1/owlapy/owl_ontology_manager.py
+-rw-rw-rw-   0        0        0     6334 2024-04-18 14:19:00.000000 owlapy-1.0.1/owlapy/owl_property.py
+-rw-rw-rw-   0        0        0    19537 2024-04-15 19:10:09.000000 owlapy-1.0.1/owlapy/owl_reasoner.py
+-rw-rw-rw-   0        0        0    37465 2024-04-17 14:23:56.000000 owlapy-1.0.1/owlapy/parser.py
+-rw-rw-rw-   0        0        0     2882 2024-04-15 19:24:04.000000 owlapy-1.0.1/owlapy/providers.py
+-rw-rw-rw-   0        0        0    16389 2024-04-17 14:23:56.000000 owlapy-1.0.1/owlapy/render.py
+-rw-rw-rw-   0        0        0    22897 2024-04-17 14:23:56.000000 owlapy-1.0.1/owlapy/util.py
+-rw-rw-rw-   0        0        0     4601 2024-04-17 12:10:21.000000 owlapy-1.0.1/owlapy/vocab.py
+drwxrwxrwx   0        0        0        0 2024-04-24 11:41:15.488148 owlapy-1.0.1/owlapy.egg-info/
+-rw-rw-rw-   0        0        0     3808 2024-04-24 11:41:15.000000 owlapy-1.0.1/owlapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1064 2024-04-24 11:41:15.000000 owlapy-1.0.1/owlapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 11:41:15.000000 owlapy-1.0.1/owlapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-24 11:41:15.000000 owlapy-1.0.1/owlapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-24 11:41:15.000000 owlapy-1.0.1/owlapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       82 2023-11-14 15:09:44.000000 owlapy-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-24 11:41:15.490144 owlapy-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      885 2024-04-23 13:34:11.000000 owlapy-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 11:41:15.486135 owlapy-1.0.1/tests/
+-rw-rw-rw-   0        0        0     1045 2024-04-15 19:24:04.000000 owlapy-1.0.1/tests/test_class_expression_semantics.py
+-rw-rw-rw-   0        0        0     1318 2024-04-15 19:24:04.000000 owlapy-1.0.1/tests/test_examples.py
+-rw-rw-rw-   0        0        0     1693 2024-04-15 19:50:32.000000 owlapy-1.0.1/tests/test_owlapy.py
+-rw-rw-rw-   0        0        0    11461 2024-04-15 19:50:32.000000 owlapy-1.0.1/tests/test_owlapy_cnf_dnf.py
+-rw-rw-rw-   0        0        0    18720 2024-04-17 14:24:48.000000 owlapy-1.0.1/tests/test_owlapy_nnf.py
+-rw-rw-rw-   0        0        0    30821 2024-04-17 14:24:48.000000 owlapy-1.0.1/tests/test_owlapy_parser.py
+-rw-rw-rw-   0        0        0     8940 2024-04-17 14:24:48.000000 owlapy-1.0.1/tests/test_owlapy_render.py
```

### Comparing `owlapy-1.0.0/LICENSE` & `owlapy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/PKG-INFO` & `owlapy-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owlapy
-Version: 1.0.0
+Version: 1.0.1
 Summary: OWLAPY is a Python Framework for creating and manipulating OWL Ontologies.
 Home-page: https://github.com/dice-group/owlapy
 Author: Caglar Demir
 Author-email: caglardemir8@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `owlapy-1.0.0/README.md` & `owlapy-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/owlapy/class_expression/__init__.py` & `owlapy-1.0.1/owlapy/class_expression/__init__.py`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/owlapy/class_expression/class_expression.py` & `owlapy-1.0.1/owlapy/class_expression/class_expression.py`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/owlapy/class_expression/nary_boolean_expression.py` & `owlapy-1.0.1/owlapy/class_expression/nary_boolean_expression.py`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/owlapy/class_expression/owl_class.py` & `owlapy-1.0.1/owlapy/class_expression/owl_class.py`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/owlapy/class_expression/restriction.py` & `owlapy-1.0.1/owlapy/class_expression/restriction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """OWL Restrictions"""
 from abc import ABCMeta, abstractmethod
 from ..meta_classes import HasFiller, HasCardinality, HasOperands
 from typing import TypeVar, Generic, Final, Sequence, Union, Iterable
-from .nary_boolean_expression import OWLObjectIntersectionOf
+from .nary_boolean_expression import OWLObjectIntersectionOf, OWLObjectUnionOf
 from .class_expression import OWLAnonymousClassExpression, OWLClassExpression
 from ..owl_property import OWLPropertyExpression, OWLObjectPropertyExpression, OWLDataPropertyExpression
 from ..owl_data_ranges import OWLPropertyRange, OWLDataRange
 from ..owl_literal import OWLLiteral
 from ..owl_individual import OWLIndividual
 from ..owl_datatype import OWLDatatype
 from ..owl_object import OWLObject
```

### Comparing `owlapy-1.0.0/owlapy/converter.py` & `owlapy-1.0.1/owlapy/converter.py`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/owlapy/iri.py` & `owlapy-1.0.1/owlapy/iri.py`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/owlapy/meta_classes.py` & `owlapy-1.0.1/owlapy/meta_classes.py`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/owlapy/namespaces.py` & `owlapy-1.0.1/owlapy/namespaces.py`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/owlapy/owl_annotation.py` & `owlapy-1.0.1/owlapy/owl_annotation.py`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/owlapy/owl_axiom.py` & `owlapy-1.0.1/owlapy/owl_axiom.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """OWL Axioms"""
 from abc import ABCMeta, abstractmethod
+from itertools import combinations
 
 from typing import TypeVar, List, Optional, Iterable, Generic, Final, Union
 from .owl_property import OWLDataPropertyExpression, OWLObjectPropertyExpression
 from .owl_object import OWLObject, OWLEntity
 from .owl_datatype import OWLDatatype, OWLDataRange
 from .meta_classes import HasOperands
 from .owl_property import OWLPropertyExpression, OWLProperty
-from .class_expression import OWLClassExpression, OWLClass
+from .class_expression import OWLClassExpression, OWLClass, OWLNothing, OWLThing, OWLObjectUnionOf
 from .owl_individual import OWLIndividual
 from .iri import IRI
 from owlapy.owl_annotation import OWLAnnotationSubject, OWLAnnotationValue
 from .owl_literal import OWLLiteral
 
 _C = TypeVar('_C', bound='OWLObject')  #:
 _P = TypeVar('_P', bound='OWLPropertyExpression')  #:
```

### Comparing `owlapy-1.0.0/owlapy/owl_data_ranges.py` & `owlapy-1.0.1/owlapy/owl_data_ranges.py`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/owlapy/owl_datatype.py` & `owlapy-1.0.1/owlapy/owl_datatype.py`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/owlapy/owl_individual.py` & `owlapy-1.0.1/owlapy/owl_individual.py`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/owlapy/owl_literal.py` & `owlapy-1.0.1/owlapy/owl_literal.py`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/owlapy/owl_object.py` & `owlapy-1.0.1/owlapy/owl_object.py`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/owlapy/owl_ontology.py` & `owlapy-1.0.1/owlapy/owl_ontology.py`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/owlapy/owl_ontology_manager.py` & `owlapy-1.0.1/owlapy/owl_ontology_manager.py`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/owlapy/owl_property.py` & `owlapy-1.0.1/owlapy/owl_property.py`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/owlapy/owl_reasoner.py` & `owlapy-1.0.1/owlapy/owl_reasoner.py`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/owlapy/parser.py` & `owlapy-1.0.1/owlapy/parser.py`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/owlapy/providers.py` & `owlapy-1.0.1/owlapy/providers.py`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/owlapy/render.py` & `owlapy-1.0.1/owlapy/render.py`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/owlapy/util.py` & `owlapy-1.0.1/owlapy/util.py`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/owlapy/vocab.py` & `owlapy-1.0.1/owlapy/vocab.py`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/owlapy.egg-info/PKG-INFO` & `owlapy-1.0.1/owlapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owlapy
-Version: 1.0.0
+Version: 1.0.1
 Summary: OWLAPY is a Python Framework for creating and manipulating OWL Ontologies.
 Home-page: https://github.com/dice-group/owlapy
 Author: Caglar Demir
 Author-email: caglardemir8@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `owlapy-1.0.0/owlapy.egg-info/SOURCES.txt` & `owlapy-1.0.1/owlapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/setup.py` & `owlapy-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 setup(
     name="owlapy",
     description="OWLAPY is a Python Framework for creating and manipulating OWL Ontologies.",
-    version="1.0.0",
+    version="1.0.1",
     packages=find_packages(),
     install_requires=[
         "pandas>=1.5.0",
         "rdflib>=6.0.2",
         "parsimonious>=0.8.1",
         "pytest>=8.1.1"],
     author='Caglar Demir',
```

### Comparing `owlapy-1.0.0/tests/test_class_expression_semantics.py` & `owlapy-1.0.1/tests/test_class_expression_semantics.py`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/tests/test_examples.py` & `owlapy-1.0.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/tests/test_owlapy.py` & `owlapy-1.0.1/tests/test_owlapy.py`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/tests/test_owlapy_cnf_dnf.py` & `owlapy-1.0.1/tests/test_owlapy_cnf_dnf.py`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/tests/test_owlapy_nnf.py` & `owlapy-1.0.1/tests/test_owlapy_nnf.py`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/tests/test_owlapy_parser.py` & `owlapy-1.0.1/tests/test_owlapy_parser.py`

 * *Files identical despite different names*

### Comparing `owlapy-1.0.0/tests/test_owlapy_render.py` & `owlapy-1.0.1/tests/test_owlapy_render.py`

 * *Files identical despite different names*

