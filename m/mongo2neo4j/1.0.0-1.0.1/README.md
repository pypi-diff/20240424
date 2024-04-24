# Comparing `tmp/mongo2neo4j-1.0.0.tar.gz` & `tmp/mongo2neo4j-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo2neo4j-1.0.0.tar", last modified: Fri Apr 19 14:06:08 2024, max compression
+gzip compressed data, was "mongo2neo4j-1.0.1.tar", last modified: Wed Apr 24 15:56:56 2024, max compression
```

## Comparing `mongo2neo4j-1.0.0.tar` & `mongo2neo4j-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 luther     (501) staff       (20)        0 2024-04-19 14:06:08.839669 mongo2neo4j-1.0.0/
--rw-r--r--   0 luther     (501) staff       (20)    35821 2023-08-05 21:05:58.000000 mongo2neo4j-1.0.0/LICENSE
--rw-r--r--   0 luther     (501) staff       (20)    46256 2024-04-19 14:06:08.839076 mongo2neo4j-1.0.0/PKG-INFO
--rw-r--r--   0 luther     (501) staff       (20)     4347 2023-09-28 10:35:23.000000 mongo2neo4j-1.0.0/README.md
--rw-r--r--   0 luther     (501) staff       (20)     6987 2024-02-12 16:48:54.000000 mongo2neo4j-1.0.0/pyproject.toml
--rw-r--r--   0 luther     (501) staff       (20)      170 2024-04-19 13:47:32.000000 mongo2neo4j-1.0.0/requirements-dev.txt
--rw-r--r--   0 luther     (501) staff       (20)       29 2024-04-16 11:28:39.000000 mongo2neo4j-1.0.0/requirements.txt
--rw-r--r--   0 luther     (501) staff       (20)       38 2024-04-19 14:06:08.839778 mongo2neo4j-1.0.0/setup.cfg
-drwxr-xr-x   0 luther     (501) staff       (20)        0 2024-04-19 14:06:08.828159 mongo2neo4j-1.0.0/src/
-drwxr-xr-x   0 luther     (501) staff       (20)        0 2024-04-19 14:06:08.831901 mongo2neo4j-1.0.0/src/mongo2neo4j/
--rw-rw-r--   0 luther     (501) staff       (20)    49265 2024-04-17 14:33:29.000000 mongo2neo4j-1.0.0/src/mongo2neo4j/__init__.py
--rw-rw-r--   0 luther     (501) staff       (20)      138 2024-04-12 10:37:13.000000 mongo2neo4j-1.0.0/src/mongo2neo4j/__main__.py
--rw-rw-r--   0 luther     (501) staff       (20)        0 2023-08-10 06:05:58.000000 mongo2neo4j-1.0.0/src/mongo2neo4j/py.typed
-drwxr-xr-x   0 luther     (501) staff       (20)        0 2024-04-19 14:06:08.836621 mongo2neo4j-1.0.0/src/mongo2neo4j.egg-info/
--rw-r--r--   0 luther     (501) staff       (20)    46256 2024-04-19 14:06:08.000000 mongo2neo4j-1.0.0/src/mongo2neo4j.egg-info/PKG-INFO
--rw-r--r--   0 luther     (501) staff       (20)      441 2024-04-19 14:06:08.000000 mongo2neo4j-1.0.0/src/mongo2neo4j.egg-info/SOURCES.txt
--rw-r--r--   0 luther     (501) staff       (20)        1 2024-04-19 14:06:08.000000 mongo2neo4j-1.0.0/src/mongo2neo4j.egg-info/dependency_links.txt
--rw-r--r--   0 luther     (501) staff       (20)       57 2024-04-19 14:06:08.000000 mongo2neo4j-1.0.0/src/mongo2neo4j.egg-info/entry_points.txt
--rw-r--r--   0 luther     (501) staff       (20)      206 2024-04-19 14:06:08.000000 mongo2neo4j-1.0.0/src/mongo2neo4j.egg-info/requires.txt
--rw-r--r--   0 luther     (501) staff       (20)       12 2024-04-19 14:06:08.000000 mongo2neo4j-1.0.0/src/mongo2neo4j.egg-info/top_level.txt
-drwxr-xr-x   0 luther     (501) staff       (20)        0 2024-04-19 14:06:08.835596 mongo2neo4j-1.0.0/tests/
--rw-rw-r--   0 luther     (501) staff       (20)       41 2023-07-06 07:53:53.000000 mongo2neo4j-1.0.0/tests/test_basic.py
--rw-rw-r--   0 luther     (501) staff       (20)     9949 2023-10-15 11:38:33.000000 mongo2neo4j-1.0.0/tests/test_flatten_and_cleanse.py
+drwxr-xr-x   0 luther     (501) staff       (20)        0 2024-04-24 15:56:56.776553 mongo2neo4j-1.0.1/
+-rw-r--r--   0 luther     (501) staff       (20)    35821 2023-08-05 21:05:58.000000 mongo2neo4j-1.0.1/LICENSE
+-rw-r--r--   0 luther     (501) staff       (20)    46256 2024-04-24 15:56:56.775457 mongo2neo4j-1.0.1/PKG-INFO
+-rw-r--r--   0 luther     (501) staff       (20)     4347 2023-09-28 10:35:23.000000 mongo2neo4j-1.0.1/README.md
+-rw-r--r--   0 luther     (501) staff       (20)     6987 2024-04-22 12:53:21.000000 mongo2neo4j-1.0.1/pyproject.toml
+-rw-r--r--   0 luther     (501) staff       (20)      170 2024-04-19 13:47:32.000000 mongo2neo4j-1.0.1/requirements-dev.txt
+-rw-r--r--   0 luther     (501) staff       (20)       29 2024-04-16 11:28:39.000000 mongo2neo4j-1.0.1/requirements.txt
+-rw-r--r--   0 luther     (501) staff       (20)       38 2024-04-24 15:56:56.776751 mongo2neo4j-1.0.1/setup.cfg
+drwxr-xr-x   0 luther     (501) staff       (20)        0 2024-04-24 15:56:56.758468 mongo2neo4j-1.0.1/src/
+drwxr-xr-x   0 luther     (501) staff       (20)        0 2024-04-24 15:56:56.762651 mongo2neo4j-1.0.1/src/mongo2neo4j/
+-rw-rw-r--   0 luther     (501) staff       (20)    50723 2024-04-24 15:56:27.000000 mongo2neo4j-1.0.1/src/mongo2neo4j/__init__.py
+-rw-rw-r--   0 luther     (501) staff       (20)      138 2024-04-19 14:06:59.000000 mongo2neo4j-1.0.1/src/mongo2neo4j/__main__.py
+-rw-rw-r--   0 luther     (501) staff       (20)        0 2023-08-10 06:05:58.000000 mongo2neo4j-1.0.1/src/mongo2neo4j/py.typed
+drwxr-xr-x   0 luther     (501) staff       (20)        0 2024-04-24 15:56:56.770164 mongo2neo4j-1.0.1/src/mongo2neo4j.egg-info/
+-rw-r--r--   0 luther     (501) staff       (20)    46256 2024-04-24 15:56:56.000000 mongo2neo4j-1.0.1/src/mongo2neo4j.egg-info/PKG-INFO
+-rw-r--r--   0 luther     (501) staff       (20)      441 2024-04-24 15:56:56.000000 mongo2neo4j-1.0.1/src/mongo2neo4j.egg-info/SOURCES.txt
+-rw-r--r--   0 luther     (501) staff       (20)        1 2024-04-24 15:56:56.000000 mongo2neo4j-1.0.1/src/mongo2neo4j.egg-info/dependency_links.txt
+-rw-r--r--   0 luther     (501) staff       (20)       57 2024-04-24 15:56:56.000000 mongo2neo4j-1.0.1/src/mongo2neo4j.egg-info/entry_points.txt
+-rw-r--r--   0 luther     (501) staff       (20)      206 2024-04-24 15:56:56.000000 mongo2neo4j-1.0.1/src/mongo2neo4j.egg-info/requires.txt
+-rw-r--r--   0 luther     (501) staff       (20)       12 2024-04-24 15:56:56.000000 mongo2neo4j-1.0.1/src/mongo2neo4j.egg-info/top_level.txt
+drwxr-xr-x   0 luther     (501) staff       (20)        0 2024-04-24 15:56:56.768847 mongo2neo4j-1.0.1/tests/
+-rw-rw-r--   0 luther     (501) staff       (20)       41 2023-07-06 07:53:53.000000 mongo2neo4j-1.0.1/tests/test_basic.py
+-rw-rw-r--   0 luther     (501) staff       (20)     9949 2023-10-15 11:38:33.000000 mongo2neo4j-1.0.1/tests/test_flatten_and_cleanse.py
```

### Comparing `mongo2neo4j-1.0.0/LICENSE` & `mongo2neo4j-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mongo2neo4j-1.0.0/PKG-INFO` & `mongo2neo4j-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo2neo4j
-Version: 1.0.0
+Version: 1.0.1
 Summary: Imports object structures generated by MongoDB object relation mappers (like Mongoose) into Neo4j for exploration with SemSpect
 Author: Marko Luther, Paul Holleis, Thorsten Liebig, Vincent Vialard
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -681,15 +681,15 @@
 Project-URL: Homepage, https://makomo.github.io/mongo2neo4j/
 Project-URL: Issue Tracker, https://github.com/MAKOMO/mongo2neo4j/issues
 Keywords: MongoDB,Neo4j,Mongoose,SemSpect,exploration,conversion
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Other/Nonlisted Topic
-Requires-Python: >=3.11
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pymongo>=4.6.3
 Requires-Dist: neo4j>=5.19.0
 Provides-Extra: dev
 Requires-Dist: mypy>=1.9.0; extra == "dev"
 Requires-Dist: pyright>=1.1.359; extra == "dev"
```

### Comparing `mongo2neo4j-1.0.0/README.md` & `mongo2neo4j-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mongo2neo4j-1.0.0/pyproject.toml` & `mongo2neo4j-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
   { name="Marko Luther" },
   { name="Paul Holleis" },
   { name="Thorsten Liebig" },
   { name="Vincent Vialard" }
 ]
 license = {file = 'LICENSE'}
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.12"
 keywords = ['MongoDB', 'Neo4j', 'Mongoose', 'SemSpect', 'exploration', 'conversion']
 classifiers = [
     "Programming Language :: Python :: 3 :: Only",
     'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
     "Operating System :: OS Independent",
     'Topic :: Other/Nonlisted Topic'
 ]
@@ -70,15 +70,15 @@
 ]
 
 # Use multiple processes to speed up Pylint. Specifying 0 will auto-detect the
 # number of processors available to use.
 jobs = "0"
 
 # Minimum supported python version
-py-version = "3.11"
+py-version = "3.12"
 
 # Pickle collected data for later comparisons.
 persistent = "no"
 
 [tool.pylint.'MESSAGES CONTROL']
 
 # Disable the message, report, category or checker with the given id(s). You
@@ -131,15 +131,15 @@
 enable='''c-extension-no-member,'''
 
 
 ## mypy conf
 
 [tool.mypy]
 files = ["src/mongo2neo4j/*.py"]
-python_version = "3.11"
+python_version = "3.12"
 
 # Ensure full coverage
 check_untyped_defs = true
 disallow_incomplete_defs = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
 disallow_untyped_decorators = true
@@ -183,28 +183,28 @@
 
 # Never enforce `E501` (line length violations).
 lint.ignore = ["E402", "E501", "E741", "PLR0913", "PLR2004", "COM812", "PLR0912", "PLR0915", "PLW0603", "PLR0911", "SIM105", "SIM114"]
 
 # Exclude a variety of commonly ignored directories.
 exclude = ["dist", "build", "proto", ".pytype", ".mypy_cache", ".git"]
 
-# Assume Python 3.11
-target-version = "py311"
+# Assume Python 3.12
+target-version = "py312"
 
 
 
 ## pyright conf
 
 [tool.pyright]
 include = ["src/mongo2neo4j"]
 
 reportMissingImports = true
 reportMissingTypeStubs = false
 
-pythonVersion = "3.11"
+pythonVersion = "3.12"
 pythonPlatform = "All"
 
 #typeCheckingMode = "strict" # "off", "basic", "strict"
 
 # strict disabled checks # "error", "warning", false, true
 #reportUnboundVariable = "error"
 #reportUnknownParameterType = false
```

### Comparing `mongo2neo4j-1.0.0/src/mongo2neo4j/__init__.py` & `mongo2neo4j-1.0.1/src/mongo2neo4j/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 #!/usr/bin/env python3
 """Imports object structures generated by the ORM Mongoose <https://mongoosejs.com/> and
 stored in MongoDB <https://www.mongodb.com/> into Neo4j <https://neo4j.com/> for exploration with
 SemSpect <https://www.semspect.de/>.
 """
 
 # Changelog:
+#  v1.0.1 (04/22/2024) :
+#     - adds <super_label> to sublabel spec to play nice with SemSpects subtree facets
+#     - escapes single quites in sublabels
+#     - renames attrib to field to correspond to the MongoDB terminology
+#     - moved to Python 3.12
 #  v1.0.0 (04/12/2024) : minor rework and lib updates
 #  v0.5.0 (09/28/2023) : makes import idempotent
 #  v0.4.0 (09/26/2023) : pytests, fixes
 #  v0.3.0 (08/16/2023) : src layout, pypip package
 #  v0.2.0 (08/10/2023) :
 #     - adds recursive processing of list of objects
 #     - adds options to link nodes via relations on matching field values that are not MongoDB ObjectIds
@@ -37,126 +42,132 @@
 from neo4j.exceptions import Neo4jError, AuthError
 
 if TYPE_CHECKING:
     from pymongo.database import Database
     from pymongo.cursor import Cursor
     from neo4j import ManagedTransaction
 
-__author__ = "Marko Luther, Paul Holleis, Thorsten Liebig, Vincent Vialard, Maximilian Wenzel"
-__license__ = "GPLv3 <https://www.gnu.org/licenses/gpl-3.0.html>"
-__version__ = "1.0.0"
+__author__ = 'Marko Luther, Paul Holleis, Thorsten Liebig, Vincent Vialard, Maximilian Wenzel'
+__license__ = 'GPLv3 <https://www.gnu.org/licenses/gpl-3.0.html>'
+__version__ = '1.0.1'
 
 
 # Types
 
 Item = dict[str, Any]
 Items = list[Item]
 Link = tuple[str, str]  # holds source and target IDs
 Links = set[Link]
 Relations = dict[str, Links]  # associates relation name to Links
 Collections = set[str]
 Fields = set[str]
 NodeLabels = dict[str, str]  # associating node IDs to labels
 LabelRelations = dict[str, Relations]  # associates labels to relations
 SubLabel = tuple[
-    str, str, str, str
-]  # collection, field, sublabel postfix, OTHERS-sublabel (last two can be the empty string)
+    str, str, str, str, str
+]  # collection, field, sublabel postfix, super_label, OTHERS-sublabel (last three can be the empty string)
 SubLabels = list[SubLabel]
 CollectionField = tuple[str, str]  # collection and field
 RelationSpecification = tuple[
     CollectionField, CollectionField
-]  # source collection-attrib tuple & target collection-attrib tuple
+]  # source collection-field tuple & target collection-field tuple
 RelationSpecifications = list[RelationSpecification]
 
 
 class SubSpec(TypedDict):
     """A subtype specification."""
 
     discriminator: str
     value_type: type  # one of {str, list, bool}
     postfix: str  # empty string by default
+    super_label: str # empty string by default
     others: str  # empty string by default
     distinct_values: NotRequired[
         set[str]
     ]  # if value_type is bool, distinct_values is not available
 
 
 # Globals
 
 # default MongoDB documents ID field
-mid: str = "_id"
+mid: str = '_id'
 
 default_fields_to_remove: Fields = {
-    "__v"  # the document version will always be ignored and never transferred
+    '__v'  # the document version will always be ignored and never transferred
 }
 
-default_exclude_collections: Collections = {"system.*"}
+default_exclude_collections: Collections = {'system.*'}
 
 
 # Utility functions
 
 
 def split_excludes(suppress: Fields) -> tuple[Fields, Fields, Fields]:
     """Splits the given exclude field specifications into equal, startswith and endswith field suppress matchers"""
     res_suppress: Fields = set()
     res_suppress_startswith: Fields = set()
     res_suppress_endswith: Fields = set()
     for sup in suppress:
-        if sup.startswith("*"):
+        if sup.startswith('*'):
             res_suppress_endswith.add(sup[1:])
-        elif sup.endswith("*"):
+        elif sup.endswith('*'):
             res_suppress_startswith.add(sup[:-1])
         else:
             res_suppress.add(sup)
     return res_suppress, res_suppress_startswith, res_suppress_endswith
 
 
 def match_collection(collection: str, excluded_collections: Collections) -> bool:
     """Returns True if the given <collection> matches any pattern in <excluded_collections>"""
     return any(
         xc == collection
-        or xc.startswith("*")
+        or xc.startswith('*')
         and collection.endswith(xc[1:])
-        or xc.endswith("*")
+        or xc.endswith('*')
         and collection.startswith(xc[:-1])
         for xc in excluded_collections
     )
 
 
 def remove_excluded_collections(
     collections: Collections, excluded_collections: Collections
 ) -> Collections:
     """Removes all collections from the given <collections> that matches any pattern in excluded_collections"""
     return {c for c in collections if not match_collection(c, excluded_collections)}
 
 
 def strlist2subLabels(sl: list[str]) -> SubLabels:
-    """Takes a list of sublabel string specifications of the form <collection>.<field>[.<postfix>][,<others>] and turns it into a SubLabels specification <label=collection, discriminator=field, postfix=postfix, others=others>."""
+    """Takes a list of sublabel string specifications of the form <collection>.<field>[.<postfix>][:<super_label>][,<others>] and turns it into a SubLabels specification <label=collection, discriminator=field, postfix=postfix, super_label=super_label, others=others>."""
     sublabels: SubLabels = []
     for subl in sl:
-        el: list[str] = subl.split(",")[:2]
-        others: str = ""
+        el: list[str] = subl.split(',')[:2]
+        others: str = ''
         if len(el) > 1:
             others = el[1]
         if len(el) > 0:
-            parts: list[str] = el[0].split(".")[:3]
-            if len(parts) == 2:
-                parts += [""]
-            if len(parts) == 3:
-                sublabels.append((parts[0], parts[1], parts[2], others))
+            remaining: list[str] = el[0].split(':')[:2]
+            super_label: str = ''
+            if len(remaining) > 1:
+                super_label = remaining[1]
+            if len(remaining) > 0:
+                parts: list[str] = remaining[0].split('.')[:3]
+                if len(parts) == 2:
+                    parts += ['']
+                if len(parts) == 3:
+                    sublabels.append((parts[0], parts[1], parts[2], super_label, others))
     return sublabels
 
 
 def strlist2relationSpecifications(rl: list[str]) -> RelationSpecifications:
     relationspecs: RelationSpecifications = []
     for rel in rl:
-        rels: list[str] = rel.split(",")[:2]
+        rels: list[str] = rel.split(',')[:2]
         if len(rels) == 2:
-            source = rels[0].split(".")[:2]
-            target = rels[1].split(".")[:2]
+            source = rels[0].split('.')[:2]
+            target = rels[1].split('.')[:2]
             if len(source) == 2 and len(target) == 2:
                 source_cf: CollectionField = (source[0], source[1])
                 target_cf: CollectionField = (target[0], target[1])
                 rel_spec: RelationSpecification = (source_cf, target_cf)
                 relationspecs.append(rel_spec)
     return relationspecs
 
@@ -170,15 +181,15 @@
         if x[-1] is fillvalue:
             yield x[: bisect(x, False, key=lambda v: v is fillvalue)]  # Python 3.10+ only!
         else:
             yield x
 
 
 # see https://stackoverflow.com/questions/54815892/pymongo-cursor-batch-size
-def yield_rows(cursor: "Cursor[Any]", chunk_size: int) -> Iterator[Items]:
+def yield_rows(cursor: 'Cursor[Any]', chunk_size: int) -> Iterator[Items]:
     """Generator to yield chunks from cursor
     :param cursor:
     :param chunk_size:
     :return:
     """
     chunk: Items = []
     for i, row in enumerate(cursor):
@@ -238,57 +249,57 @@
 # converts ObjectId(_) to string
 def flatten_and_cleanse(  # pylint: disable=too-complex, too-many-arguments, too-many-locals
     collection: str,
     dictionary: MutableMapping[str, Any],
     suppress: Fields,
     suppress_startswith: Fields,
     suppress_endswith: Fields,
-    parent_key: str = "",
-    node_id: str = "",
-    separator: str = "_",
+    parent_key: str = '',
+    node_id: str = '',
+    separator: str = '_',
 ) -> tuple[Item, Relations, Fields, dict[str, Items]]:
     """Returns the given dictionary with sub dictionaries flattened,
     objectId(_) converted to strings and keys in the 'suppress', 'suppress_startswith', 'suppress_endswith' sets
     removed. As second result a dictionary associating relation names
     with list of tuples of source and target node ids.
-    As third result a set of attributes of type list.
+    As third result a set of fields of type list.
     As last result a dict associating labels with additional objects created."""
     res: Item = {}
     relations: Relations = {}
     array_fields: Fields = set()
     additional_objects: dict[str, Items] = {}  # additional objects associated to new labels
 
-    if parent_key == "" and mid in dictionary:
+    if parent_key == '' and mid in dictionary:
         node_id = str(dictionary[mid])
 
     for key, value in dictionary.items():
         if (
             key not in suppress
             and not key.startswith(tuple(suppress_startswith))
             and not key.endswith(tuple(suppress_endswith))
             and value is not None
-            and value != ""
+            and value != ''
             and value != []
         ):
             uuid_hex: str
             new_key = parent_key + separator + key if parent_key else key
             if isinstance(value, MutableMapping):
                 if mid in value:
                     uuid_hex = str(value[mid])
                     value[mid] = uuid_hex
-                    new_label = f"{collection}_{new_key}"
+                    new_label = f'{collection}_{new_key}'
                     # we create a new object and link it
                     rec_res, rec_relations, rec_array_fields, rec_objects = flatten_and_cleanse(
                         new_label,
                         value,
                         suppress,
                         suppress_startswith,
                         suppress_endswith,
-                        "",
-                        "",
+                        '',
+                        '',
                         separator,
                     )
                     add_object(additional_objects, new_label, [rec_res])
                     update_relations(relations, rec_relations)
                     array_fields.update(rec_array_fields)
                     update_objects(additional_objects, rec_objects)
                     add_relation(relations, key, (node_id, uuid_hex))
@@ -306,15 +317,15 @@
                     )
                     res.update(rec_res)
                     update_relations(relations, rec_relations)
                     array_fields.update(rec_array_fields)
                     update_objects(additional_objects, rec_objects)
             elif isinstance(value, ObjectId):
                 id_str: str = str(value)
-                if new_key != mid and node_id != "":
+                if new_key != mid and node_id != '':
                     add_relation(relations, new_key, (node_id, id_str))
                 else:
                     res[new_key] = id_str
             elif isinstance(value, MutableSequence):
                 if all(isinstance(v, str) for v in value):
                     # homogeneous list of strings
                     res[new_key] = value
@@ -323,36 +334,36 @@
                     )  # mark as field of type array, to have sublabels generated correctly on demand
                 elif all(isinstance(v, int) for v in value) or all(
                     isinstance(v, float) for v in value
                 ):
                     # homogeneous list of numbers (not marked as field of type array, to have field ignored on sublabel generation)
                     res[new_key] = value
                 elif (
-                    all(isinstance(v, ObjectId) for v in value) and new_key != mid and node_id != ""
+                    all(isinstance(v, ObjectId) for v in value) and new_key != mid and node_id != ''
                 ):
                     # homogeneous list of ObjectIds
                     # we discard the field, but establish the relations
                     add_relations(relations, new_key, {(node_id, str(v)) for v in value})
                 elif all(isinstance(v, MutableMapping) for v in value):
                     # list of objects
-                    new_label = f"{collection}_{new_key}"
+                    new_label = f'{collection}_{new_key}'
                     uuids = []
                     for i, v in enumerate(value):
                         # if there is no unique object id we generate one
-                        uuid_hex = str(v[mid]) if mid in v else f"{node_id}{new_label}{i}"
+                        uuid_hex = str(v[mid]) if mid in v else f'{node_id}{new_label}{i}'
                         uuids.append(uuid_hex)
                         v[mid] = uuid_hex
                         rec_res, rec_relations, rec_array_fields, rec_objects = flatten_and_cleanse(
                             new_label,
                             v,
                             suppress,
                             suppress_startswith,
                             suppress_endswith,
-                            "",
-                            "",
+                            '',
+                            '',
                             separator,
                         )
                         add_object(additional_objects, new_label, [rec_res])
                         update_relations(relations, rec_relations)
                         array_fields.update(rec_array_fields)
                         update_objects(additional_objects, rec_objects)
                     # add relations between this object and all generated ids
@@ -360,15 +371,15 @@
                         add_relation(relations, new_key, (node_id, uuid_hex))
             else:
                 res[new_key] = value
     return res, relations, array_fields, additional_objects
 
 
 def split_attributes(dictionary: Item) -> tuple[Item, Item]:
-    """Splits the given attributes into those with primitive values and those with \
+    """Splits the given fields into those with primitive values and those with \
         non-primitive ones"""
     primitive: Item = {}
     non_primitive: Item = {}
     for key, value in dictionary.items():
         if isinstance(value, list) and not all(
             isinstance(e, (str | bool | int | float)) for e in value
         ):
@@ -379,71 +390,71 @@
 
 
 # see https://stackoverflow.com/a/34325723
 # Progress Bar Printing Function
 def printProgressBar(  # pylint: disable=too-many-arguments
     iteration: int,
     total: int = 100,
-    prefix: str = "",
-    suffix: str = "",
+    prefix: str = '',
+    suffix: str = '',
     decimals: int = 1,
     length: int = 70,
-    fill: str = "█",
-    printEnd: str = "\r",
+    fill: str = '█',
+    printEnd: str = '\r',
 ) -> None:
     """Outputs a progress bar to stdout"""
-    percent = f"{100 * (iteration / float(total)):.{decimals}f}"
+    percent = f'{100 * (iteration / float(total)):.{decimals}f}'
     filledLength = int(length * iteration // total)
-    progbar = fill * filledLength + "-" * (length - filledLength)
-    print(f"\r{prefix} |{progbar}| {percent}% {suffix}", end=printEnd)
+    progbar = fill * filledLength + '-' * (length - filledLength)
+    print(f'\r{prefix} |{progbar}| {percent}% {suffix}', end=printEnd)
 
 
 # Neo4j communication
 
 
 def render_value(value: Any) -> str:
     """Render given value as str"""
     if isinstance(value, DateTime):
         return f"datetime('{value}')"
     if isinstance(value, datetime.datetime):
-        value_as_isoformat_datetime: str = value.isoformat(sep="T")
+        value_as_isoformat_datetime: str = value.isoformat(sep='T')
         return f"datetime('{value_as_isoformat_datetime}')"
     if isinstance(value, bool):
         return str(value).lower()
     if isinstance(value, (int | float)):
         return str(value)
     return f"'{value}'"
 
 
 def neo4j_output_query(query: str, **kwargs: Any) -> None:
     """Outputs the given Cypher query to stdout."""
     result = query
     for key, value in kwargs.items():
-        result = result.replace(f"${key}", render_value(value))
+        result = result.replace(f'${key}', render_value(value))
     print(result)
 
 
 def neo4j_run_read_query(session: None | Session, verbose: bool, query: str, **kwargs: Any) -> None:
     """Sends the given query to Neo4j and outputs it to stdout if verbose is True."""
 
-    def work(tx: "ManagedTransaction") -> Any:  # pylint: disable=invalid-name
+    def work(tx: 'ManagedTransaction') -> Any:  # pylint: disable=invalid-name
         return tx.run(query, **kwargs)  # pyright:ignore[reportGeneralTypeIssues, reportArgumentType]
 
     if verbose:
         neo4j_output_query(query, **kwargs)  # pyright:ignore[reportGeneralTypeIssues, reportArgumentType]
     if session is not None:
         session.execute_read(work)
 
 
 def neo4j_run_write_query(
     session: None | Session, verbose: bool, query: str, **kwargs: Any
 ) -> None:
     """Sends the given query to Neo4j and outputs it to stdout if verbose is True."""
 
-    def work(tx: "ManagedTransaction") -> Any:  # pylint: disable=invalid-name
+    def work(tx: 'ManagedTransaction') -> Any:  # pylint: disable=invalid-name
         return tx.run(query, **kwargs)  # pyright:ignore[reportGeneralTypeIssues, reportArgumentType]
 
     if verbose:
         neo4j_output_query(query, **kwargs)
     if session is not None:
         session.execute_write(work)
 
@@ -473,32 +484,35 @@
     apoc_installed: bool,
     create: bool,
     source: CollectionField,
     target: CollectionField,
     list_source: bool = False,
 ) -> None:
     match_clause: str = (
-        f"MATCH (a:`{source[0]}`), (b:`{target[0]}`) "
+        f'MATCH (a:`{source[0]}`), (b:`{target[0]}`) '
         f'WHERE b.`{target[1]}` {"IN" if list_source else "="} a.`{source[1]}`'
     )
     create_clause: str = f'{("CREATE" if create else "MERGE")} (a)-[:`{source[1]}`]->(b)'
     if apoc_installed:
         neo4j_run_write_query(
             session,
             verbose,
             (
                 f'CALL apoc.periodic.iterate("{match_clause} RETURN a, b",'
                 f'"{create_clause}",'
-                f"{{batchSize:{chunk_size}, parallel:true}})"
+                f'{{batchSize:{chunk_size}, parallel:true}})'
             ),
         )
     else:
-        query = f"{match_clause} {create_clause}"
+        query = f'{match_clause} {create_clause}'
         neo4j_run_write_query(session, verbose, query)
 
+def escape_neo4j_label(label:str) -> str:
+    translations: dict[str, str | int | None] = {"'":  "\\\\'"}
+    return label.translate(str.maketrans(translations))
 
 def neo4j_add_sublabel(  # pylint: disable=too-many-arguments
     session: None | Session,
     verbose: bool,
     chunk_size: int,
     apoc_installed: bool,
     label: str,
@@ -507,63 +521,63 @@
     sublabels: list[str],
     isarray: bool = False,
 ) -> None:
     """Adds <sublabel> to nodes in <label> where <value> is in list of <field> field values if isarray is True,
     or if isarray is False and <field> value equals <value>."""
     if len(sublabels) > 0:
         if isarray:
-            match_clause = f"MATCH (n:`{label}`) WHERE {value} IN n.`{field}`"
+            match_clause = f'MATCH (n:`{label}`) WHERE {value} IN n.`{field}`'
         else:
-            match_clause = f"MATCH (n:`{label}` {{`{field}`: {value}}})"
-        quoted_sublabels = [f"`{sub}`" for sub in sublabels]
+            match_clause = f'MATCH (n:`{label}` {{`{field}`: {value}}})'
+        quoted_sublabels = [f'`{sub}`' for sub in sublabels]
         set_clause = f'SET n:{":".join(quoted_sublabels)}'
         if apoc_installed:
             neo4j_run_write_query(
                 session,
                 verbose,
                 (
                     f'CALL apoc.periodic.iterate("{match_clause} RETURN n",'
                     f'"{set_clause}",'
-                    f"{{batchSize:{chunk_size}, parallel:true}})"
+                    f'{{batchSize:{chunk_size}, parallel:true}})'
                 ),
             )
         else:
-            neo4j_run_write_query(session, verbose, f"{match_clause} {set_clause}")
+            neo4j_run_write_query(session, verbose, f'{match_clause} {set_clause}')
 
 
 def neo4j_add_sublabel_other(  # pylint: disable=too-many-arguments
     session: None | Session,
     verbose: bool,
     chunk_size: int,
     apoc_installed: bool,
     label: str,
     field: str,
     others: str,
 ) -> None:
     """Adds sublabel <others> to nodes in <label> where <value> of <field> is NULL"""
-    if others != "":
-        match_clause = f"MATCH (n:`{label}`) WHERE n.`{field}` is NULL"
-        set_clause = f"SET n:{others}"
+    if others != '':
+        match_clause = f'MATCH (n:`{label}`) WHERE n.`{field}` is NULL'
+        set_clause = f'SET n:{others}'
         if apoc_installed:
             neo4j_run_write_query(
                 session,
                 verbose,
                 (
                     f'CALL apoc.periodic.iterate("{match_clause} RETURN n",'
                     f'"{set_clause}",'
-                    f"{{batchSize:{chunk_size}, parallel:true}})"
+                    f'{{batchSize:{chunk_size}, parallel:true}})'
                 ),
             )
         else:
-            neo4j_run_write_query(session, verbose, f"{match_clause} {set_clause}")
+            neo4j_run_write_query(session, verbose, f'{match_clause} {set_clause}')
 
 
 # pylint: disable=too-many-arguments
 def process_data(  # pylint: disable=too-complex,too-many-locals
-    database: "Database[Any]",
+    database: 'Database[Any]',
     session: None | Session,
     collections: Collections,
     excluded_collections: Collections,
     excluded_fields: Fields,
     sublabels: SubLabels,
     additional_relations: RelationSpecifications,
     additional_list_relations: RelationSpecifications,
@@ -591,34 +605,34 @@
     suppress_endswith: Fields
 
     suppress, suppress_startswith, suppress_endswith = split_excludes(excluded_fields)
 
     apoc_installed: bool = False
     if session is not None:
         try:
-            neo4j_run_read_query(session, verbose, "RETURN apoc.version() AS output")
+            neo4j_run_read_query(session, verbose, 'RETURN apoc.version() AS output')
             apoc_installed = True
-            print("Neo4j APOC plugin installed")
+            print('Neo4j APOC plugin installed')
         except Neo4jError:
-            print("Neo4j APOC plugin NOT installed")
+            print('Neo4j APOC plugin NOT installed')
 
     # add nodes
 
     additional_objects: dict[str, Items] = (
         {}
     )  # additional internal objects associated to new labels
 
     for collection in active_collections:
         if (item_count := database[collection].count_documents({})) > 0:
             print(f"*** processing {item_count} nodes of collection '{collection}'")
             relations = {}
             cursor: Cursor[Any] = database[collection].find({}, batch_size=chunk_size)
             chunk: Items
 
-            # Establish constraints on '_id' attribute of label 'collection'
+            # Establish constraints on '_id' fields of label 'collection'
             # NOTE: the use of $ query parameters for constraint name and label
             #       does not work here, so we use Python fstring substitution
             neo4j_create_constraint(session, verbose, collection, mid)
 
             # Initial Progress Bar Call
             printProgressBar(0, item_count)
             cnt: int = 0
@@ -637,15 +651,15 @@
                     else:
                         cleansed_data.append(obj_data)
                         update_relations(relations, obj_relations)
                         node_label[node_id] = collection
                         array_fields.update(obj_array_fields)
                         update_objects(additional_objects, obj_objects)
                 # create the nodes per chunk
-                data: dict[str, Items] = {"batch": cleansed_data}
+                data: dict[str, Items] = {'batch': cleansed_data}
                 query = f"UNWIND $batch as row {('CREATE' if create else 'MERGE')} (n:`{collection}` {{{mid}: row.{mid}}}) SET n += row"
                 neo4j_run_write_query(session, verbose, query, **data)
                 # Update Progress Bar
                 printProgressBar(cnt, item_count)
             # print new line on complete
             print()
             all_relations[collection] = relations
@@ -664,15 +678,15 @@
             if (item_count := len(new_objects)) > 0:
                 neo4j_create_constraint(session, verbose, ao_label, mid)
                 print(f"*** processing {item_count} {ao_label} additional internal nodes'")
                 printProgressBar(0, item_count)
                 cnt = 0
                 for chunk in chunker(chunk_size, new_objects):
                     cnt += len(chunk)
-                    data = {"batch": chunk}
+                    data = {'batch': chunk}
                     query = f"UNWIND $batch as row {('CREATE' if create else 'MERGE')} (n:`{ao_label}` {{{mid}: row.{mid}}}) SET n += row"
                     neo4j_run_write_query(session, verbose, query, **data)
                     # Update Progress Bar
                     printProgressBar(cnt, item_count)
                 # print new line on complete
                 print()
 
@@ -681,23 +695,23 @@
     for collection, relations in all_relations.items():
         # create relations (also per chunk)
         for rel, all_links in relations.items():
             # collected links by source and target label indexed by '<source_label>$<target_label>' with $ not allowed in MongoDB collection names
             links_by_labels: dict[str, Links] = {}
             for l in all_links:
                 if l[0] in node_label and l[1] in node_label:
-                    if (idx := f"{node_label[l[0]]}${node_label[l[1]]}") in links_by_labels:
+                    if (idx := f'{node_label[l[0]]}${node_label[l[1]]}') in links_by_labels:
                         links_by_labels[idx].add(l)
                     else:
                         links_by_labels[idx] = {l}
                 elif l[0] not in node_label:
                     print(f'missing source object: ObjectId("{l[0]}")')
                 elif l[1] not in node_label:
                     print(
-                        f'missing object linked from {node_label[l[0]]} ObjectId("{l[0]}") by attribute "{rel}": ObjectId("{l[1]}")'
+                        f'missing object linked from {node_label[l[0]]} ObjectId("{l[0]}") by field "{rel}": ObjectId("{l[1]}")'
                     )
             for links in links_by_labels.values():
                 if (item_count := len(links)) > 0:
                     # Initial Progress Bar Call
                     printProgressBar(0, item_count)
                     cnt = 0
                     # assuming same source and target labels for all links
@@ -707,31 +721,31 @@
 
                     print(
                         f"*** processing {item_count} {rel} relation ({source_label}, {target_label}) of collection '{collection}'"
                     )
 
                     for links_chunk in chunker(chunk_size, links):
                         cnt += len(links_chunk)
-                        data = {"links": links_chunk}
+                        data = {'links': links_chunk}
                         query = (
-                            f"UNWIND $links as row MATCH (a:`{source_label}`), (b:`{target_label}`) "
+                            f'UNWIND $links as row MATCH (a:`{source_label}`), (b:`{target_label}`) '
                             f"WHERE a.{mid} = row[0] and b.{mid} = row[1] {('CREATE' if create else 'MERGE')} (a)-[:`{rel}`]->(b)"
                         )
                         neo4j_run_write_query(session, verbose, query, **data)
                         # Update Progress Bar
                         printProgressBar(cnt, item_count)
                     # print new line on complete
                     print()
 
     # add specified relations
 
     # create indices on sources and uniqueness constraint on targets of additional relations
     if additional_relations:
         item_count = len(additional_relations)
-        print(f"*** processing {item_count} additional relations")
+        print(f'*** processing {item_count} additional relations')
         # Initial Progress Bar Call
         printProgressBar(0, item_count)
         cnt = 0
         for rel_source, rel_target in additional_relations:
             cnt += 1
             if rel_source[0] in node_label.values() and rel_target[0] in node_label.values():
                 # only process additional relation if nodes in source and target labels exist
@@ -743,15 +757,15 @@
             # Update Progress Bar
             printProgressBar(cnt, item_count)
         # print new line on complete
         print()
 
     if additional_list_relations:
         item_count = len(additional_list_relations)
-        print(f"*** processing {item_count} additional list relations")
+        print(f'*** processing {item_count} additional list relations')
         # Initial Progress Bar Call
         printProgressBar(0, item_count)
         cnt = 0
         for rel_source, rel_target in additional_list_relations:
             cnt += 1
             if rel_source[0] in node_label.values() and rel_target[0] in node_label.values():
                 # only process additional list relation if nodes in source and target labels exist
@@ -775,133 +789,142 @@
     # add sublabels
 
     # we only generate sublabels for active collections
     sublabels = [sl for sl in sublabels if sl[0] in active_collections]
     if len(sublabels) > 0:
         established_sublabels: set[str] = set()
         sub_label_specs: dict[str, list[SubSpec]] = {}
-        # extract distinct values, type and postfix per sublabel item and associate it with label in sub_label_spec
-        for label, discriminator, postfix, others in sublabels:
+        # extract distinct values, type , postfix, and super_label per sublabel item and associate it with label in sub_label_spec
+        for label, discriminator, postfix, super_label, others in sublabels:
             # distinct values, without None and the empty string
             distinct_values: set[Any] = set(database[label].distinct(discriminator)).difference(
-                {None, ""}
+                {None, ''}
             )
             sub_label_spec_item: None | SubSpec = None
             if all(isinstance(item, bool) for item in distinct_values) and True in distinct_values:
                 discriminator_postfix: str = discriminator + postfix
                 if (
                     discriminator_postfix not in active_collections
                     and discriminator_postfix not in established_sublabels
                 ):
                     # we use only the discriminator+prefix as sublabel for boolean typed discriminators
                     sub_label_spec_item = SubSpec(
-                        discriminator=discriminator, postfix=postfix, others=others, value_type=bool
+                        discriminator=discriminator, postfix=postfix, super_label=super_label, others=others, value_type=bool
                     )
                     # remember newly created (sub-)label
                     established_sublabels.add(discriminator_postfix)
                 else:
                     print(
                         f'sublabel {label}.{discriminator}{("" if postfix == "" else "."+postfix)} skipped'
                     )
-            elif 1 < len(distinct_values) < 150 and all(
+            elif 1 < len(distinct_values) < 300 and all(
                 isinstance(item, str) for item in distinct_values
             ):
                 distinct_values_postfix: list[str] = [str(s) + postfix for s in distinct_values]
                 if not active_collections.intersection(
                     distinct_values_postfix
                 ) and not established_sublabels.intersection(distinct_values_postfix):
                     sub_label_spec_item = SubSpec(
                         discriminator=discriminator,
                         postfix=postfix,
+                        super_label=super_label,
                         others=others,
                         value_type=(list if (discriminator in array_fields) else str),
                         distinct_values=distinct_values,
                     )
                     # remember newly created (sub-)label
                     new_sublabels: list[str] = [
                         item
                         for sublist in [
-                            [f"{l}{postfix}" for l in sl.split("#")] for sl in distinct_values
+                            [f'{l}{postfix}' for l in sl.split('#')] for sl in distinct_values
                         ]
                         for item in sublist
                     ]
                     new_sublabels.append(discriminator)
                     established_sublabels.update(new_sublabels)
                 else:
                     print(
                         f'sublabel {label}.{discriminator}{("" if postfix == "" else "."+postfix)} skipped'
                     )
+            elif len(distinct_values) > 150:
+                print(
+                    f'sublabel {label}.{discriminator}{("" if postfix == "" else "."+postfix)} skipped (): to many distinct values ({len(distinct_values)} > 300)'
+                )
             if sub_label_spec_item is not None:
                 if label in sub_label_specs:
                     sub_label_specs[label].append(sub_label_spec_item)
                 else:
                     sub_label_specs[label] = [sub_label_spec_item]
 
         if (item_count := len(sub_label_specs.items())) > 0:
-            print(f"*** processing {item_count} sublabels")
+            print(f'*** processing {item_count} sublabels')
             # Initial Progress Bar Call
             printProgressBar(0, item_count)
             cnt = 0
             for label, sub_specs in sub_label_specs.items():
                 cnt += 1
                 for sub_spec in sub_specs:
-                    if sub_spec["value_type"] is bool:
-                        discriminator = sub_spec["discriminator"]
+                    if sub_spec['value_type'] is bool:
+                        discriminator = sub_spec['discriminator']
                         neo4j_create_index(session, verbose, label, discriminator)
                         neo4j_add_sublabel(
                             session,
                             verbose,
                             chunk_size,
                             apoc_installed,
                             label,
                             discriminator,
-                            "true",
+                            'true',
                             [f'{discriminator}{sub_spec["postfix"]}'],
                         )
                         neo4j_add_sublabel_other(
                             session,
                             verbose,
                             chunk_size,
                             apoc_installed,
                             label,
                             discriminator,
-                            sub_spec["others"],
+                            sub_spec['others'],
                         )
-                    elif sub_spec["value_type"] in [str, list]:
+                    elif sub_spec['value_type'] in [str, list]:
                         # first establish index on the discriminator
-                        isarray: bool = sub_spec["value_type"] is list
-                        discriminator = sub_spec["discriminator"]
+                        isarray: bool = sub_spec['value_type'] is list
+                        discriminator = sub_spec['discriminator']
                         if not isarray:
                             # for fields of type list the index is not effective
                             neo4j_create_index(session, verbose, label, discriminator)
-                        if "distinct_values" in sub_spec:
-                            for sl in sub_spec["distinct_values"]:
+                        if 'distinct_values' in sub_spec:
+                            for sl in sub_spec['distinct_values']:
+                                sl_escaped = escape_neo4j_label(sl)
                                 # add sublabels
                                 labels: list[str] = [
-                                    f'{l}{sub_spec["postfix"]}' for l in sl.split("#")
+                                    f'{l}{sub_spec["postfix"]}' for l in sl.split('#')
                                 ]
+                                # add the specified <super_label> label if any
+                                if sub_spec['super_label']:
+                                    labels.append(sub_spec['super_label'])
                                 neo4j_add_sublabel(
                                     session,
                                     verbose,
                                     chunk_size,
                                     apoc_installed,
                                     label,
                                     discriminator,
-                                    f"'{sl}'",
+                                    f"'{sl_escaped}'",
                                     labels,
                                     isarray,
                                 )
                             neo4j_add_sublabel_other(
                                 session,
                                 verbose,
                                 chunk_size,
                                 apoc_installed,
                                 label,
                                 discriminator,
-                                sub_spec["others"],
+                                sub_spec['others'],
                             )
                 # Update Progress Bar
                 printProgressBar(cnt, item_count)
             # print new line on complete
             print()
 
 
@@ -923,22 +946,22 @@
     relations: RelationSpecifications,
     list_relations: RelationSpecifications,
     create: bool = False,
     verbose: bool = False,
     simulate: bool = False,
 ) -> int:
     """The main mongo2neo4j function that takes MongoDB credential and DB name, Neo4j credentials \
-        and DB name and a specification which MongoDB collections and attributes should be \
+        and DB name and a specification which MongoDB collections and fields should be \
         transferred to Neo4j, if the Cypher queries should be printed to stdout (verbose=True) \
         and if the Neo4j engine should be connected to or not (simulate=True)."""
 
     # connect to MongDB
     mongo_client: MongoClient[Any] = MongoClient(mongo_host, mongo_port)
     # get MongoDB DB
-    database: "Database[Any]" = mongo_client[mongo_db]
+    database: 'Database[Any]' = mongo_client[mongo_db]
 
     try:
         db_collections: list[str] = database.list_collection_names()
         collections: Collections = (
             set(db_collections)
             if included_collections is None
             else set(included_collections).intersection(db_collections)
@@ -957,15 +980,15 @@
                 create,
                 verbose,
                 chunk_size,
             )
         else:
             driver: Driver
             with GraphDatabase.driver(  # pylint: disable=not-context-manager
-                f"neo4j://{neo4j_host}:{neo4j_port}",
+                f'neo4j://{neo4j_host}:{neo4j_port}',
                 auth=(neo4j_user, neo4j_password),
                 telemetry_disabled=True,
             ) as driver:
                 session: Session
                 with driver.session(database=neo4j_db) as session:
                     process_data(
                         database,
@@ -978,179 +1001,179 @@
                         list_relations,
                         create,
                         verbose,
                         chunk_size,
                     )
         return 0
     except AuthError:
-        print("Neo4j authentication failed")
+        print('Neo4j authentication failed')
     except ServerSelectionTimeoutError:
-        print("MongoDB connection error")
+        print('MongoDB connection error')
     except PyMongoError as e:
-        print("MongoDB error", e)
+        print('MongoDB error', e)
     except Neo4jError as e:
-        print("Neo4j error", e)
+        print('Neo4j error', e)
     return -1
 
 
 def console_main() -> int:  # pylint: disable=too-complex
     """The CLI entry point of mongo2neo4j.
 
     This function is not meant for programmable use; use `main()` instead.
     """
     # https://docs.python.org/3/library/signal.html#note-on-sigpipe
     try:
-        parser = argparse.ArgumentParser(description=f"mongo2neo4j v{__version__}: {__doc__}")
-        mongo_group = parser.add_argument_group("MongoDB connection")
+        parser = argparse.ArgumentParser(description=f'mongo2neo4j v{__version__}: {__doc__}')
+        mongo_group = parser.add_argument_group('MongoDB connection')
         mongo_group.add_argument(
-            "-mh",
-            "--mongo_host",
-            dest="mongo_host",
+            '-mh',
+            '--mongo_host',
+            dest='mongo_host',
             type=str,
-            default="localhost",
-            help="MongoDB simple hostname or a full MongoDB URI of the form mongodb://<user>:<password>@<host>:<port>. Unix domain sockets with percent encoded socket path in the URI.",
+            default='localhost',
+            help='MongoDB simple hostname or a full MongoDB URI of the form mongodb://<user>:<password>@<host>:<port>. Unix domain sockets with percent encoded socket path in the URI.',
         )
         mongo_group.add_argument(
-            "-mp", "--mongo_port", dest="mongo_port", type=int, default="27017", help="MongoDB port"
+            '-mp', '--mongo_port', dest='mongo_port', type=int, default='27017', help='MongoDB port'
         )
 
-        neo4j_group = parser.add_argument_group("Neo4j connection")
+        neo4j_group = parser.add_argument_group('Neo4j connection')
         neo4j_group.add_argument(
-            "-nh",
-            "--neo4j_host",
-            dest="neo4j_host",
+            '-nh',
+            '--neo4j_host',
+            dest='neo4j_host',
             type=str,
-            default="localhost",
-            help="Neo4j hostname",
+            default='localhost',
+            help='Neo4j hostname',
         )
         neo4j_group.add_argument(
-            "-np", "--neo4j_port", dest="neo4j_port", type=int, default="7687", help="Neo4j port"
+            '-np', '--neo4j_port', dest='neo4j_port', type=int, default='7687', help='Neo4j port'
         )
         neo4j_group.add_argument(
-            "-nu", "--neo4j_user", dest="neo4j_user", type=str, default="neo4j", help="Neo4j user"
+            '-nu', '--neo4j_user', dest='neo4j_user', type=str, default='neo4j', help='Neo4j user'
         )
         neo4j_group.add_argument(
-            "-npw", "--neo4j_password", dest="neo4j_password", type=str, help="Neo4j password"
+            '-npw', '--neo4j_password', dest='neo4j_password', type=str, help='Neo4j password'
         )
         neo4j_group.add_argument(
-            "-nd", "--neo4j_db", dest="neo4j_db", type=str, help="Neo4j DB to import into"
+            '-nd', '--neo4j_db', dest='neo4j_db', type=str, help='Neo4j DB to import into'
         )
 
-        mapping_group = parser.add_argument_group("Mapping")
+        mapping_group = parser.add_argument_group('Mapping')
         mapping_group.add_argument(
-            "-i",
-            "--include",
-            dest="included_collections",
-            action="append",
-            help="Comma separated collections to be transferred. If not specified, transfer all not excluded ones",
+            '-i',
+            '--include',
+            dest='included_collections',
+            action='append',
+            help='Comma separated collections to be transferred. If not specified, transfer all not excluded ones',
         )
         mapping_group.add_argument(
-            "-x",
-            "--exclude",
-            dest="excluded_collections",
-            action="append",
+            '-x',
+            '--exclude',
+            dest='excluded_collections',
+            action='append',
             default=[],
-            help="Comma separated collections to be excluded. Collection names can have a * at the begin or end to match multiple collections.",
+            help='Comma separated collections to be excluded. Collection names can have a * at the begin or end to match multiple collections.',
         )
         mapping_group.add_argument(
-            "-f",
-            "--exclude_fields",
-            dest="excluded_fields",
-            action="append",
+            '-f',
+            '--exclude_fields',
+            dest='excluded_fields',
+            action='append',
             default=[],
-            help="Comma separated fields to be ignored. Field names can have a * at the begin or end to match multiple fields.",
+            help='Comma separated fields to be ignored. Field names can have a * at the begin or end to match multiple fields.',
         )
         mapping_group.add_argument(
-            "-sl",
-            "--sublabels",
-            dest="sublabels",
-            action="append",
+            '-sl',
+            '--sublabels',
+            dest='sublabels',
+            action='append',
             default=[],
-            help="List of <collection>.<attrib>[.<postfix>][,<others>] fields of type string or list of strings to create sublabels. The optional <postfix> is added to the generated sublabel and if <others> is given it is used to collect nodes without proper value.",
+            help='List of <collection>.<field>[.<postfix>][:<super_label>][,<others>] fields of type string or list of strings to create sublabels. The optional <postfix> is added to the generated sublabel, the optional <super_label> is assigned to all items and if <others> is given it is used to collect the nodes without proper value.',
         )
         mapping_group.add_argument(
-            "-r",
-            "--relations",
-            dest="relations",
-            action="append",
+            '-r',
+            '--relations',
+            dest='relations',
+            action='append',
             default=[],
-            help="List of <Collection>.<attrib>,<collection>.<attrib> tuples to relations between nodes of equal str/number values",
+            help='List of <Collection>.<field>,<collection>.<field> tuples to relations between nodes of equal str/number values',
         )
         mapping_group.add_argument(
-            "-lr",
-            "--list_relations",
-            dest="list_relations",
-            action="append",
+            '-lr',
+            '--list_relations',
+            dest='list_relations',
+            action='append',
             default=[],
-            help="List of <collection>.<attrib>,<collection>.<attrib> tuples to relations between nodes of list of str/number values and str/number values",
+            help='List of <collection>.<field>,<collection>.<field> tuples to relations between nodes of list of str/number values and str/number values',
         )
 
-        parser.add_argument("--conf_export", action="store_true", help="Dump config and exit")
-        parser.add_argument("--conf", action="append", help="Read config file")
-        parser.add_argument("-v", "--verbose", action="store_true", help="Output Cypher")
-        parser.add_argument("-s", "--simulate", action="store_true", help="Don't connect to Neo4j")
+        parser.add_argument('--conf_export', action='store_true', help='Dump config and exit')
+        parser.add_argument('--conf', action='append', help='Read config file')
+        parser.add_argument('-v', '--verbose', action='store_true', help='Output Cypher')
+        parser.add_argument('-s', '--simulate', action='store_true', help="Don't connect to Neo4j")
         parser.add_argument(
-            "-c",
-            "--create",
-            action="store_true",
-            help="Use CREATE instead of MERGE to create objects in Neo4j",
+            '-c',
+            '--create',
+            action='store_true',
+            help='Use CREATE instead of MERGE to create objects in Neo4j',
         )
 
         parser.add_argument(
-            "-k",
-            "--chunk_size",
-            dest="chunk_size",
+            '-k',
+            '--chunk_size',
+            dest='chunk_size',
             type=int,
-            default="500",
-            help="processing objects chunk size",
+            default='500',
+            help='processing objects chunk size',
         )
 
-        parser.add_argument("mongo_db", help="MongoDB DB to be imported")
+        parser.add_argument('mongo_db', help='MongoDB DB to be imported')
         args = parser.parse_args()
 
-        print(f"mongo2neo4j v{__version__}")
+        print(f'mongo2neo4j v{__version__}')
 
         # load config file
-        if args.conf is None and os.path.isfile("mongo2neo4j.conf"):
+        if args.conf is None and os.path.isfile('mongo2neo4j.conf'):
             # by default we load a config from mongo2neo4j.conf if nothing else is specified and that file exists
-            args.conf = ["mongo2neo4j.conf"]
+            args.conf = ['mongo2neo4j.conf']
         if args.conf is not None:
             for conf_fname in args.conf:
                 try:
-                    with open(conf_fname, encoding="utf-8") as f:
+                    with open(conf_fname, encoding='utf-8') as f:
                         parser.set_defaults(**json.load(f))
                 except FileNotFoundError:
                     print(f'config file "{conf_fname}" not found')
                     sys.exit(-1)
 
         # Reload arguments to override config file values with command line values
         args = parser.parse_args()
 
         # dump config
         if args.conf_export:
             tmp_args = vars(args).copy()
-            del tmp_args["conf_export"]  # Do not dump value of conf_export flag
-            del tmp_args["conf"]  # Values already loaded
+            del tmp_args['conf_export']  # Do not dump value of conf_export flag
+            del tmp_args['conf']  # Values already loaded
             print(json.dumps(tmp_args, indent=4, sort_keys=True))
             sys.exit(-1)
 
         requested_collections: None | Collections = None
         if args.included_collections is not None:
             requested_collections = set()
             for c in args.included_collections:
-                for s in c.split(","):
+                for s in c.split(','):
                     requested_collections.add(s)
         args_excluded_collections: Collections = default_exclude_collections
         for c in args.excluded_collections:
-            for s in c.split(","):
+            for s in c.split(','):
                 args_excluded_collections.add(s)
         args_excluded_fields: Fields = default_fields_to_remove
         if args.excluded_fields is not None:
             for fields in args.excluded_fields:
-                for f in fields.split(","):
+                for f in fields.split(','):
                     args_excluded_fields.add(str(f))
 
         start = time.perf_counter()
         res = main(
             args.mongo_host,
             args.mongo_port,
             args.mongo_db,
@@ -1180,9 +1203,9 @@
         # Python flushes standard streams on exit; redirect remaining output
         # to devnull to avoid another BrokenPipeError at shutdown
         devnull = os.open(os.devnull, os.O_WRONLY)
         os.dup2(devnull, sys.stdout.fileno())
         return 1  # Python exits with error code 1 on EPIPE
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     sys.exit(console_main())
```

### Comparing `mongo2neo4j-1.0.0/src/mongo2neo4j.egg-info/PKG-INFO` & `mongo2neo4j-1.0.1/src/mongo2neo4j.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongo2neo4j
-Version: 1.0.0
+Version: 1.0.1
 Summary: Imports object structures generated by MongoDB object relation mappers (like Mongoose) into Neo4j for exploration with SemSpect
 Author: Marko Luther, Paul Holleis, Thorsten Liebig, Vincent Vialard
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -681,15 +681,15 @@
 Project-URL: Homepage, https://makomo.github.io/mongo2neo4j/
 Project-URL: Issue Tracker, https://github.com/MAKOMO/mongo2neo4j/issues
 Keywords: MongoDB,Neo4j,Mongoose,SemSpect,exploration,conversion
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Other/Nonlisted Topic
-Requires-Python: >=3.11
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pymongo>=4.6.3
 Requires-Dist: neo4j>=5.19.0
 Provides-Extra: dev
 Requires-Dist: mypy>=1.9.0; extra == "dev"
 Requires-Dist: pyright>=1.1.359; extra == "dev"
```

### Comparing `mongo2neo4j-1.0.0/tests/test_flatten_and_cleanse.py` & `mongo2neo4j-1.0.1/tests/test_flatten_and_cleanse.py`

 * *Files identical despite different names*

