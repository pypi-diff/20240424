# Comparing `tmp/openyieldtables-0.0.0.tar.gz` & `tmp/openyieldtables-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openyieldtables-0.0.0.tar", max compression
+gzip compressed data, was "openyieldtables-1.0.0.tar", max compression
```

## Comparing `openyieldtables-0.0.0.tar` & `openyieldtables-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1087 2024-04-18 13:09:13.209518 openyieldtables-0.0.0/LICENSE
--rw-r--r--   0        0        0      890 2024-04-18 13:09:13.209518 openyieldtables-0.0.0/README.md
--rw-r--r--   0        0        0     1563 2024-04-18 13:09:14.025520 openyieldtables-0.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-18 13:09:13.213518 openyieldtables-0.0.0/src/openyieldtables/__init__.py
--rw-r--r--   0        0        0   485247 2024-04-18 13:09:13.213518 openyieldtables-0.0.0/src/openyieldtables/data/yield_tables.csv
--rw-r--r--   0        0        0     7205 2024-04-18 13:09:13.213518 openyieldtables-0.0.0/src/openyieldtables/data/yield_tables_meta.csv
--rw-r--r--   0        0        0      119 2024-04-18 13:09:13.213518 openyieldtables-0.0.0/src/openyieldtables/models/__init__.py
--rw-r--r--   0        0        0     1124 2024-04-18 13:09:13.213518 openyieldtables-0.0.0/src/openyieldtables/models/yieldtable.py
--rw-r--r--   0        0        0        0 2024-04-18 13:09:13.213518 openyieldtables-0.0.0/src/openyieldtables/py.typed
--rw-r--r--   0        0        0       55 2024-04-18 13:09:13.213518 openyieldtables-0.0.0/src/openyieldtables/utils/__init__.py
--rw-r--r--   0        0        0     1379 2024-04-18 13:09:13.213518 openyieldtables-0.0.0/src/openyieldtables/utils/utils.py
--rw-r--r--   0        0        0     6256 2024-04-18 13:09:13.213518 openyieldtables-0.0.0/src/openyieldtables/yieldtables.py
--rw-r--r--   0        0        0     1376 1970-01-01 00:00:00.000000 openyieldtables-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-23 21:08:06.091670 openyieldtables-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1509 2024-04-23 21:08:06.091670 openyieldtables-1.0.0/README.md
+-rw-r--r--   0        0        0     1784 2024-04-23 21:08:07.567665 openyieldtables-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-23 21:08:06.091670 openyieldtables-1.0.0/src/openyieldtables/__init__.py
+-rw-r--r--   0        0        0   485247 2024-04-23 21:08:06.095670 openyieldtables-1.0.0/src/openyieldtables/data/yield_tables.csv
+-rw-r--r--   0        0        0     7205 2024-04-23 21:08:06.095670 openyieldtables-1.0.0/src/openyieldtables/data/yield_tables_meta.csv
+-rw-r--r--   0        0        0      119 2024-04-23 21:08:06.095670 openyieldtables-1.0.0/src/openyieldtables/models/__init__.py
+-rw-r--r--   0        0        0     1118 2024-04-23 21:08:06.095670 openyieldtables-1.0.0/src/openyieldtables/models/yieldtable.py
+-rw-r--r--   0        0        0        0 2024-04-23 21:08:06.095670 openyieldtables-1.0.0/src/openyieldtables/py.typed
+-rw-r--r--   0        0        0       55 2024-04-23 21:08:06.095670 openyieldtables-1.0.0/src/openyieldtables/utils/__init__.py
+-rw-r--r--   0        0        0     1379 2024-04-23 21:08:06.095670 openyieldtables-1.0.0/src/openyieldtables/utils/utils.py
+-rw-r--r--   0        0        0     6249 2024-04-23 21:08:06.095670 openyieldtables-1.0.0/src/openyieldtables/yieldtables.py
+-rw-r--r--   0        0        0     2319 1970-01-01 00:00:00.000000 openyieldtables-1.0.0/PKG-INFO
```

### Comparing `openyieldtables-0.0.0/LICENSE` & `openyieldtables-1.0.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2024 to Tree.ly FlexCo and FMM GmbH
+Copyright (c) 2024 to Tree.ly FlexKapG and FMM GmbH
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `openyieldtables-0.0.0/pyproject.toml` & `openyieldtables-1.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 [tool.poetry]
 name = "openyieldtables"
-version = "0.0.0"
+version = "1.0.0"
 description = ""
-authors = ["Tree.ly", "FMM"]
+authors = ["Tree.ly <hello@tree.ly>", "FMM <fmm@fmm.at>"]
+maintainers = ["FMM <fmm@fmm.at>", "Tree.ly <hello@tree.ly>"]
 readme = "README.md"
+license = "MIT"
+repository = "https://github.com/treely/openyieldtables"
+documentation = "https://openyieldtables.readthedocs.io"
 packages = [
   { include = "openyieldtables", from = "src" },
   { include = "src/openyieldtables/py.typed" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `openyieldtables-0.0.0/src/openyieldtables/data/yield_tables.csv` & `openyieldtables-1.0.0/src/openyieldtables/data/yield_tables.csv`

 * *Files identical despite different names*

### Comparing `openyieldtables-0.0.0/src/openyieldtables/data/yield_tables_meta.csv` & `openyieldtables-1.0.0/src/openyieldtables/data/yield_tables_meta.csv`

 * *Files identical despite different names*

### Comparing `openyieldtables-0.0.0/src/openyieldtables/models/yieldtable.py` & `openyieldtables-1.0.0/src/openyieldtables/models/yieldtable.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,8 +36,8 @@
 
 
 class YieldTableData(BaseModel):
     yield_classes: List[YieldClass]
 
 
 class YieldTable(YieldTableMeta):
-    data: List[YieldTableData]
+    data: YieldTableData
```

### Comparing `openyieldtables-0.0.0/src/openyieldtables/utils/utils.py` & `openyieldtables-1.0.0/src/openyieldtables/utils/utils.py`

 * *Files identical despite different names*

### Comparing `openyieldtables-0.0.0/src/openyieldtables/yieldtables.py` & `openyieldtables-1.0.0/src/openyieldtables/yieldtables.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     for yield_table_meta in yield_table_meta_list:
         if yield_table_meta.id == id:
             return yield_table_meta
 
     raise ValueError(f"Yield table with ID {id} not found.")
 
 
-def get_yield_table_data(id: int) -> YieldTable:
+def get_yield_table(id: int) -> YieldTable:
     """
     Reads the yield table data for a specific yield table ID from
     `data/yield_tables.csv` and returns a YieldTable instance.
 
     The CSV file is expected to be in a specific format, with columns for
     `id`, `yield_class`, `age`, `dominant_height`, `average_height`, etc.
 
@@ -179,9 +179,9 @@
     yield_classes = [
         YieldClass(yield_class=yc, rows=rows)
         for yc, rows in yield_classes_dict.items()
     ]
 
     return YieldTable(
         **yield_table_meta.model_dump(),
-        data=[YieldTableData(yield_classes=yield_classes)],
+        data=YieldTableData(yield_classes=yield_classes),
     )
```

