# Comparing `tmp/shareyourcloning_linkml-0.1.0a0.tar.gz` & `tmp/shareyourcloning_linkml-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shareyourcloning_linkml-0.1.0a0.tar", max compression
+gzip compressed data, was "shareyourcloning_linkml-0.1.1a0.tar", max compression
```

## Comparing `shareyourcloning_linkml-0.1.0a0.tar` & `shareyourcloning_linkml-0.1.1a0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1087 2024-04-24 14:51:46.818483 shareyourcloning_linkml-0.1.0a0/LICENSE
--rw-r--r--   0        0        0      923 2024-04-24 14:51:46.818483 shareyourcloning_linkml-0.1.0a0/README.md
--rw-r--r--   0        0        0    15882 2024-04-24 14:51:46.818483 shareyourcloning_linkml-0.1.0a0/project/excel/shareyourcloning_linkml.xlsx
--rw-r--r--   0        0        0     3623 2024-04-24 14:51:46.818483 shareyourcloning_linkml-0.1.0a0/project/graphql/shareyourcloning_linkml.graphql
--rw-r--r--   0        0        0     6281 2024-04-24 14:51:46.818483 shareyourcloning_linkml-0.1.0a0/project/jsonld/shareyourcloning_linkml.context.jsonld
--rw-r--r--   0        0        0    67794 2024-04-24 14:51:46.818483 shareyourcloning_linkml-0.1.0a0/project/jsonld/shareyourcloning_linkml.jsonld
--rw-r--r--   0        0        0    36392 2024-04-24 14:51:46.818483 shareyourcloning_linkml-0.1.0a0/project/jsonschema/shareyourcloning_linkml.schema.json
--rw-r--r--   0        0        0    46328 2024-04-24 14:51:46.822483 shareyourcloning_linkml-0.1.0a0/project/owl/shareyourcloning_linkml.owl.ttl
--rw-r--r--   0        0        0      400 2024-04-24 14:51:46.822483 shareyourcloning_linkml-0.1.0a0/project/prefixmap/shareyourcloning_linkml.yaml
--rw-r--r--   0        0        0     5299 2024-04-24 14:51:46.822483 shareyourcloning_linkml-0.1.0a0/project/protobuf/shareyourcloning_linkml.proto
--rw-r--r--   0        0        0    38377 2024-04-24 14:51:46.822483 shareyourcloning_linkml-0.1.0a0/project/shacl/shareyourcloning_linkml.shacl.ttl
--rw-r--r--   0        0        0     8269 2024-04-24 14:51:46.822483 shareyourcloning_linkml-0.1.0a0/project/shex/shareyourcloning_linkml.shex
--rw-r--r--   0        0        0    27043 2024-04-24 14:51:46.822483 shareyourcloning_linkml-0.1.0a0/project/sqlschema/shareyourcloning_linkml.sql
--rw-r--r--   0        0        0     1420 2024-04-24 14:51:56.802466 shareyourcloning_linkml-0.1.0a0/pyproject.toml
--rw-r--r--   0        0        0      186 2024-04-24 14:51:46.822483 shareyourcloning_linkml-0.1.0a0/src/shareyourcloning_linkml/_version.py
--rw-r--r--   0        0        0       39 2024-04-24 14:51:46.822483 shareyourcloning_linkml-0.1.0a0/src/shareyourcloning_linkml/datamodel/__init__.py
--rw-r--r--   0        0        0    20901 2024-04-24 14:51:46.822483 shareyourcloning_linkml-0.1.0a0/src/shareyourcloning_linkml/datamodel/_models.py
--rw-r--r--   0        0        0    52413 2024-04-24 14:51:46.822483 shareyourcloning_linkml-0.1.0a0/src/shareyourcloning_linkml/datamodel/shareyourcloning_linkml.py
--rw-r--r--   0        0        0    13200 2024-04-24 14:51:46.822483 shareyourcloning_linkml-0.1.0a0/src/shareyourcloning_linkml/schema/shareyourcloning_linkml.yaml
--rw-r--r--   0        0        0     2045 1970-01-01 00:00:00.000000 shareyourcloning_linkml-0.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2024-04-24 15:12:08.713148 shareyourcloning_linkml-0.1.1a0/LICENSE
+-rw-r--r--   0        0        0      923 2024-04-24 15:12:08.713148 shareyourcloning_linkml-0.1.1a0/README.md
+-rw-r--r--   0        0        0    15882 2024-04-24 15:12:08.713148 shareyourcloning_linkml-0.1.1a0/project/excel/shareyourcloning_linkml.xlsx
+-rw-r--r--   0        0        0     3623 2024-04-24 15:12:08.713148 shareyourcloning_linkml-0.1.1a0/project/graphql/shareyourcloning_linkml.graphql
+-rw-r--r--   0        0        0     6281 2024-04-24 15:12:08.713148 shareyourcloning_linkml-0.1.1a0/project/jsonld/shareyourcloning_linkml.context.jsonld
+-rw-r--r--   0        0        0    67794 2024-04-24 15:12:08.713148 shareyourcloning_linkml-0.1.1a0/project/jsonld/shareyourcloning_linkml.jsonld
+-rw-r--r--   0        0        0    36392 2024-04-24 15:12:08.713148 shareyourcloning_linkml-0.1.1a0/project/jsonschema/shareyourcloning_linkml.schema.json
+-rw-r--r--   0        0        0    46328 2024-04-24 15:12:08.717148 shareyourcloning_linkml-0.1.1a0/project/owl/shareyourcloning_linkml.owl.ttl
+-rw-r--r--   0        0        0      400 2024-04-24 15:12:08.717148 shareyourcloning_linkml-0.1.1a0/project/prefixmap/shareyourcloning_linkml.yaml
+-rw-r--r--   0        0        0     5299 2024-04-24 15:12:08.717148 shareyourcloning_linkml-0.1.1a0/project/protobuf/shareyourcloning_linkml.proto
+-rw-r--r--   0        0        0    38377 2024-04-24 15:12:08.717148 shareyourcloning_linkml-0.1.1a0/project/shacl/shareyourcloning_linkml.shacl.ttl
+-rw-r--r--   0        0        0     8269 2024-04-24 15:12:08.717148 shareyourcloning_linkml-0.1.1a0/project/shex/shareyourcloning_linkml.shex
+-rw-r--r--   0        0        0    27043 2024-04-24 15:12:08.717148 shareyourcloning_linkml-0.1.1a0/project/sqlschema/shareyourcloning_linkml.sql
+-rw-r--r--   0        0        0     1364 2024-04-24 15:12:25.541082 shareyourcloning_linkml-0.1.1a0/pyproject.toml
+-rw-r--r--   0        0        0      186 2024-04-24 15:12:08.717148 shareyourcloning_linkml-0.1.1a0/src/shareyourcloning_linkml/_version.py
+-rw-r--r--   0        0        0       39 2024-04-24 15:12:08.717148 shareyourcloning_linkml-0.1.1a0/src/shareyourcloning_linkml/datamodel/__init__.py
+-rw-r--r--   0        0        0    20901 2024-04-24 15:12:08.717148 shareyourcloning_linkml-0.1.1a0/src/shareyourcloning_linkml/datamodel/_models.py
+-rw-r--r--   0        0        0    52413 2024-04-24 15:12:08.717148 shareyourcloning_linkml-0.1.1a0/src/shareyourcloning_linkml/datamodel/shareyourcloning_linkml.py
+-rw-r--r--   0        0        0    13200 2024-04-24 15:12:08.717148 shareyourcloning_linkml-0.1.1a0/src/shareyourcloning_linkml/schema/shareyourcloning_linkml.yaml
+-rw-r--r--   0        0        0     1836 1970-01-01 00:00:00.000000 shareyourcloning_linkml-0.1.1a0/PKG-INFO
```

### Comparing `shareyourcloning_linkml-0.1.0a0/LICENSE` & `shareyourcloning_linkml-0.1.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.0a0/README.md` & `shareyourcloning_linkml-0.1.1a0/README.md`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.0a0/project/excel/shareyourcloning_linkml.xlsx` & `shareyourcloning_linkml-0.1.1a0/project/excel/shareyourcloning_linkml.xlsx`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.0a0/project/graphql/shareyourcloning_linkml.graphql` & `shareyourcloning_linkml-0.1.1a0/project/graphql/shareyourcloning_linkml.graphql`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.0a0/project/jsonld/shareyourcloning_linkml.context.jsonld` & `shareyourcloning_linkml-0.1.1a0/project/jsonld/shareyourcloning_linkml.context.jsonld`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.0a0/project/jsonld/shareyourcloning_linkml.jsonld` & `shareyourcloning_linkml-0.1.1a0/project/jsonld/shareyourcloning_linkml.jsonld`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.0a0/project/jsonschema/shareyourcloning_linkml.schema.json` & `shareyourcloning_linkml-0.1.1a0/project/jsonschema/shareyourcloning_linkml.schema.json`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.0a0/project/owl/shareyourcloning_linkml.owl.ttl` & `shareyourcloning_linkml-0.1.1a0/project/owl/shareyourcloning_linkml.owl.ttl`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.0a0/project/protobuf/shareyourcloning_linkml.proto` & `shareyourcloning_linkml-0.1.1a0/project/protobuf/shareyourcloning_linkml.proto`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.0a0/project/shacl/shareyourcloning_linkml.shacl.ttl` & `shareyourcloning_linkml-0.1.1a0/project/shacl/shareyourcloning_linkml.shacl.ttl`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.0a0/project/shex/shareyourcloning_linkml.shex` & `shareyourcloning_linkml-0.1.1a0/project/shex/shareyourcloning_linkml.shex`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.0a0/project/sqlschema/shareyourcloning_linkml.sql` & `shareyourcloning_linkml-0.1.1a0/project/sqlschema/shareyourcloning_linkml.sql`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.0a0/pyproject.toml` & `shareyourcloning_linkml-0.1.1a0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 authors = ["Manuel Lera-Ramirez <manuel.lera-ramirez@ucl.ac.uk>"]
 description = "A LinkML data model for ShareYourCloning"
 include = ["README.md", "src/shareyourcloning_linkml/schema", "project"]
 license = "MIT"
 name = "shareyourcloning-linkml"
 readme = "README.md"
-version = "0.1.0a0"
+version = "0.1.1a0"
 
 homepage = "https://github.com/genestorian/ShareYourCloning_LinkML"
 repository = "https://github.com/genestorian/ShareYourCloning_LinkML"
 documentation = "https://genestorian.github.io/ShareYourCloning_LinkML"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -19,31 +19,31 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 
 [tool.poetry.dependencies]
-linkml-runtime = "^1.1.24"
 python = "^3.9"
-rdflib = "6"
-linkml = "^1.7.8"
-pydna = "^5.2.0"
-twine = "^5.0.0"
+
 
 [tool.poetry-dynamic-versioning]
 enable = false
 style = "pep440"
 vcs = "git"
 
-[tool.poetry.dev-dependencies]
-linkml = "^1.3.5"
+[tool.poetry.group.dev.dependencies]
+linkml = "^1.7.8"
+linkml-runtime = "^1.7.5"
 mkdocs-material = "^8.2.8"
 mkdocs-mermaid2-plugin = "^0.6.0"
 schemasheets = "^0.1.14"
 
 [build-system]
 build-backend = "poetry_dynamic_versioning.backend"
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 
+
+
+
 [tool.poetry.extras]
 docs = ["linkml", "mkdocs-material"]
```

### Comparing `shareyourcloning_linkml-0.1.0a0/src/shareyourcloning_linkml/datamodel/_models.py` & `shareyourcloning_linkml-0.1.1a0/src/shareyourcloning_linkml/datamodel/_models.py`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.0a0/src/shareyourcloning_linkml/datamodel/shareyourcloning_linkml.py` & `shareyourcloning_linkml-0.1.1a0/src/shareyourcloning_linkml/datamodel/shareyourcloning_linkml.py`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.0a0/src/shareyourcloning_linkml/schema/shareyourcloning_linkml.yaml` & `shareyourcloning_linkml-0.1.1a0/src/shareyourcloning_linkml/schema/shareyourcloning_linkml.yaml`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.0a0/PKG-INFO` & `shareyourcloning_linkml-0.1.1a0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareyourcloning-linkml
-Version: 0.1.0a0
+Version: 0.1.1a0
 Summary: A LinkML data model for ShareYourCloning
 Home-page: https://github.com/genestorian/ShareYourCloning_LinkML
 License: MIT
 Author: Manuel Lera-Ramirez
 Author-email: manuel.lera-ramirez@ucl.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -12,19 +12,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: docs
-Requires-Dist: linkml (>=1.7.8,<2.0.0) ; extra == "docs"
-Requires-Dist: linkml-runtime (>=1.1.24,<2.0.0)
-Requires-Dist: pydna (>=5.2.0,<6.0.0)
-Requires-Dist: rdflib (==6)
-Requires-Dist: twine (>=5.0.0,<6.0.0)
 Project-URL: Documentation, https://genestorian.github.io/ShareYourCloning_LinkML
 Project-URL: Repository, https://github.com/genestorian/ShareYourCloning_LinkML
 Description-Content-Type: text/markdown
 
 # ShareYourCloning_LinkML
 
 A LinkML data model for ShareYourCloning
```

