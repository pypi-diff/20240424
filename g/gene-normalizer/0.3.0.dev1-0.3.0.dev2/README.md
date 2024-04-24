# Comparing `tmp/gene-normalizer-0.3.0.dev1.tar.gz` & `tmp/gene_normalizer-0.3.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gene-normalizer-0.3.0.dev1.tar", last modified: Fri Oct 20 17:27:27 2023, max compression
+gzip compressed data, was "gene_normalizer-0.3.0.dev2.tar", last modified: Wed Apr 24 19:10:37 2024, max compression
```

## Comparing `gene-normalizer-0.3.0.dev1.tar` & `gene_normalizer-0.3.0.dev2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 17:27:27.682479 gene-normalizer-0.3.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-10-20 17:27:18.000000 gene-normalizer-0.3.0.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6701 2023-10-20 17:27:27.682479 gene-normalizer-0.3.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2023-10-20 17:27:18.000000 gene-normalizer-0.3.0.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2023-10-20 17:27:18.000000 gene-normalizer-0.3.0.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-20 17:27:27.682479 gene-normalizer-0.3.0.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 17:27:27.674479 gene-normalizer-0.3.0.dev1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 17:27:27.678479 gene-normalizer-0.3.0.dev1/src/gene/
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2023-10-20 17:27:18.000000 gene-normalizer-0.3.0.dev1/src/gene/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10774 2023-10-20 17:27:18.000000 gene-normalizer-0.3.0.dev1/src/gene/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 17:27:27.678479 gene-normalizer-0.3.0.dev1/src/gene/database/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-10-20 17:27:18.000000 gene-normalizer-0.3.0.dev1/src/gene/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12611 2023-10-20 17:27:18.000000 gene-normalizer-0.3.0.dev1/src/gene/database/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    22409 2023-10-20 17:27:18.000000 gene-normalizer-0.3.0.dev1/src/gene/database/dynamodb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 17:27:27.678479 gene-normalizer-0.3.0.dev1/src/gene/database/postgresql/
--rw-r--r--   0 runner    (1001) docker     (127)      713 2023-10-20 17:27:18.000000 gene-normalizer-0.3.0.dev1/src/gene/database/postgresql/add_fkeys.sql
--rw-r--r--   0 runner    (1001) docker     (127)      630 2023-10-20 17:27:18.000000 gene-normalizer-0.3.0.dev1/src/gene/database/postgresql/add_indexes.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2023-10-20 17:27:18.000000 gene-normalizer-0.3.0.dev1/src/gene/database/postgresql/create_record_lookup_view.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2023-10-20 17:27:18.000000 gene-normalizer-0.3.0.dev1/src/gene/database/postgresql/create_tables.sql
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-10-20 17:27:18.000000 gene-normalizer-0.3.0.dev1/src/gene/database/postgresql/delete_normalized_concepts.sql
--rw-r--r--   0 runner    (1001) docker     (127)      383 2023-10-20 17:27:18.000000 gene-normalizer-0.3.0.dev1/src/gene/database/postgresql/drop_fkeys.sql
--rw-r--r--   0 runner    (1001) docker     (127)      381 2023-10-20 17:27:18.000000 gene-normalizer-0.3.0.dev1/src/gene/database/postgresql/drop_indexes.sql
--rw-r--r--   0 runner    (1001) docker     (127)    33614 2023-10-20 17:27:18.000000 gene-normalizer-0.3.0.dev1/src/gene/database/postgresql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 17:27:27.678479 gene-normalizer-0.3.0.dev1/src/gene/etl/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2023-10-20 17:27:18.000000 gene-normalizer-0.3.0.dev1/src/gene/etl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11352 2023-10-20 17:27:18.000000 gene-normalizer-0.3.0.dev1/src/gene/etl/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10862 2023-10-20 17:27:18.000000 gene-normalizer-0.3.0.dev1/src/gene/etl/ensembl.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2023-10-20 17:27:18.000000 gene-normalizer-0.3.0.dev1/src/gene/etl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12541 2023-10-20 17:27:18.000000 gene-normalizer-0.3.0.dev1/src/gene/etl/hgnc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7852 2023-10-20 17:27:18.000000 gene-normalizer-0.3.0.dev1/src/gene/etl/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    27138 2023-10-20 17:27:18.000000 gene-normalizer-0.3.0.dev1/src/gene/etl/ncbi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2023-10-20 17:27:18.000000 gene-normalizer-0.3.0.dev1/src/gene/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    28586 2023-10-20 17:27:18.000000 gene-normalizer-0.3.0.dev1/src/gene/query.py
--rw-r--r--   0 runner    (1001) docker     (127)    25992 2023-10-20 17:27:18.000000 gene-normalizer-0.3.0.dev1/src/gene/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-10-20 17:27:18.000000 gene-normalizer-0.3.0.dev1/src/gene/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 17:27:27.682479 gene-normalizer-0.3.0.dev1/src/gene_normalizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6701 2023-10-20 17:27:27.000000 gene-normalizer-0.3.0.dev1/src/gene_normalizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2023-10-20 17:27:27.000000 gene-normalizer-0.3.0.dev1/src/gene_normalizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-20 17:27:27.000000 gene-normalizer-0.3.0.dev1/src/gene_normalizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-10-20 17:27:27.000000 gene-normalizer-0.3.0.dev1/src/gene_normalizer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      354 2023-10-20 17:27:27.000000 gene-normalizer-0.3.0.dev1/src/gene_normalizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-20 17:27:27.000000 gene-normalizer-0.3.0.dev1/src/gene_normalizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:10:37.570116 gene_normalizer-0.3.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-24 19:10:27.000000 gene_normalizer-0.3.0.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-24 19:10:37.570116 gene_normalizer-0.3.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-04-24 19:10:27.000000 gene_normalizer-0.3.0.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-24 19:10:27.000000 gene_normalizer-0.3.0.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:10:37.570116 gene_normalizer-0.3.0.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:10:37.562116 gene_normalizer-0.3.0.dev2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:10:37.566116 gene_normalizer-0.3.0.dev2/src/gene/
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-24 19:10:27.000000 gene_normalizer-0.3.0.dev2/src/gene/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10788 2024-04-24 19:10:27.000000 gene_normalizer-0.3.0.dev2/src/gene/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:10:37.566116 gene_normalizer-0.3.0.dev2/src/gene/database/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-24 19:10:27.000000 gene_normalizer-0.3.0.dev2/src/gene/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12611 2024-04-24 19:10:27.000000 gene_normalizer-0.3.0.dev2/src/gene/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22409 2024-04-24 19:10:27.000000 gene_normalizer-0.3.0.dev2/src/gene/database/dynamodb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:10:37.566116 gene_normalizer-0.3.0.dev2/src/gene/database/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-24 19:10:27.000000 gene_normalizer-0.3.0.dev2/src/gene/database/postgresql/add_fkeys.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-24 19:10:27.000000 gene_normalizer-0.3.0.dev2/src/gene/database/postgresql/add_indexes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-24 19:10:27.000000 gene_normalizer-0.3.0.dev2/src/gene/database/postgresql/create_record_lookup_view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-24 19:10:27.000000 gene_normalizer-0.3.0.dev2/src/gene/database/postgresql/create_tables.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-24 19:10:27.000000 gene_normalizer-0.3.0.dev2/src/gene/database/postgresql/delete_normalized_concepts.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-24 19:10:27.000000 gene_normalizer-0.3.0.dev2/src/gene/database/postgresql/drop_fkeys.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-24 19:10:27.000000 gene_normalizer-0.3.0.dev2/src/gene/database/postgresql/drop_indexes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    33096 2024-04-24 19:10:27.000000 gene_normalizer-0.3.0.dev2/src/gene/database/postgresql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:10:37.566116 gene_normalizer-0.3.0.dev2/src/gene/etl/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-24 19:10:27.000000 gene_normalizer-0.3.0.dev2/src/gene/etl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9223 2024-04-24 19:10:27.000000 gene_normalizer-0.3.0.dev2/src/gene/etl/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-24 19:10:27.000000 gene_normalizer-0.3.0.dev2/src/gene/etl/ensembl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-24 19:10:27.000000 gene_normalizer-0.3.0.dev2/src/gene/etl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9308 2024-04-24 19:10:27.000000 gene_normalizer-0.3.0.dev2/src/gene/etl/hgnc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7852 2024-04-24 19:10:27.000000 gene_normalizer-0.3.0.dev2/src/gene/etl/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19699 2024-04-24 19:10:27.000000 gene_normalizer-0.3.0.dev2/src/gene/etl/ncbi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-24 19:10:27.000000 gene_normalizer-0.3.0.dev2/src/gene/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28586 2024-04-24 19:10:27.000000 gene_normalizer-0.3.0.dev2/src/gene/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25984 2024-04-24 19:10:27.000000 gene_normalizer-0.3.0.dev2/src/gene/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-24 19:10:27.000000 gene_normalizer-0.3.0.dev2/src/gene/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:10:37.570116 gene_normalizer-0.3.0.dev2/src/gene_normalizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-24 19:10:37.000000 gene_normalizer-0.3.0.dev2/src/gene_normalizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-24 19:10:37.000000 gene_normalizer-0.3.0.dev2/src/gene_normalizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:10:37.000000 gene_normalizer-0.3.0.dev2/src/gene_normalizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-24 19:10:37.000000 gene_normalizer-0.3.0.dev2/src/gene_normalizer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-24 19:10:37.000000 gene_normalizer-0.3.0.dev2/src/gene_normalizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 19:10:37.000000 gene_normalizer-0.3.0.dev2/src/gene_normalizer.egg-info/top_level.txt
```

### Comparing `gene-normalizer-0.3.0.dev1/LICENSE` & `gene_normalizer-0.3.0.dev2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020-2023 VICC
+Copyright (c) 2020-2024 VICC
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `gene-normalizer-0.3.0.dev1/PKG-INFO` & `gene_normalizer-0.3.0.dev2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gene-normalizer
-Version: 0.3.0.dev1
+Version: 0.3.0.dev2
 Summary: VICC normalization routines for genes
 Author: Alex Wagner, Kori Kuzma, James Stevenson
 License: MIT License
         
-        Copyright (c) 2020-2023 VICC
+        Copyright (c) 2020-2024 VICC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -53,59 +53,60 @@
 Requires-Dist: boto3
 Requires-Dist: ga4gh.vrs~=2.0.0a1
 Provides-Extra: pg
 Requires-Dist: psycopg[binary]; extra == "pg"
 Provides-Extra: etl
 Requires-Dist: gffutils; extra == "etl"
 Requires-Dist: biocommons.seqrepo; extra == "etl"
+Requires-Dist: wags-tails>=0.1.1; extra == "etl"
 Provides-Extra: test
 Requires-Dist: pytest>=6.0; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: mock; extra == "test"
 Requires-Dist: httpx; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: ruff; extra == "dev"
+Requires-Dist: ruff==0.2.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx==6.1.3; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints==1.22.0; extra == "docs"
 Requires-Dist: sphinx-autobuild==2021.3.14; extra == "docs"
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "docs"
 Requires-Dist: sphinxext-opengraph==0.8.2; extra == "docs"
 Requires-Dist: furo==2023.3.27; extra == "docs"
 Requires-Dist: gravis==0.1.0; extra == "docs"
+Requires-Dist: sphinx-github-changelog==1.2.1; extra == "docs"
 
 <h1 align="center">
 Gene Normalizer
 </h1>
 
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/gene-normalizer?color=gr) [![tests](https://github.com/cancervariants/gene-normalization/actions/workflows/github-actions.yml/badge.svg)](https://github.com/cancervariants/gene-normalization/actions/workflows/github-actions.yml) [![DOI](https://zenodo.org/badge/309797998.svg)](https://zenodo.org/badge/latestdoi/309797998)
+[![image](https://img.shields.io/pypi/v/gene-normalizer.svg)](https://pypi.python.org/pypi/gene-normalizer) [![image](https://img.shields.io/pypi/l/gene-normalizer.svg)](https://pypi.python.org/pypi/gene-normalizer) [![image](https://img.shields.io/pypi/pyversions/gene-normalizer.svg)](https://pypi.python.org/pypi/gene-normalizer) [![Actions status](https://github.com/cancervariants/gene-normalization/actions/workflows/checks.yaml/badge.svg)](https://github.com/cancervariants/gene-normalization/actions/workflows/checks.yaml) [![DOI](https://zenodo.org/badge/309797998.svg)](https://zenodo.org/badge/latestdoi/309797998)
 
 ## Overview
-
+<!-- description -->
 The Gene Normalizer provides tools for resolving ambiguous human gene references to consistently-structured, normalized terms. For gene concepts extracted from [NCBI Gene](https://www.ncbi.nlm.nih.gov/gene/), [Ensembl](https://useast.ensembl.org/index.html), and [HGNC](https://www.genenames.org/), it designates a [CURIE](https://en.wikipedia.org/wiki/CURIE), and provides additional metadata like current and previously-used symbols, aliases, database cross-references and associations, and coordinates.
-
+<!-- /description -->
 ---
 
 **[Live service](https://normalize.cancervariants.org/gene)**
 
-**[Documentation](https://gene-normalizer.readthedocs.io/en/latest/)** · [Installation](https://gene-normalizer.readthedocs.io/en/latest/install.html) · [Usage](https://gene-normalizer.readthedocs.io/en/latest/usage.html) · [API reference](https://gene-normalizer.readthedocs.io/en/latest/api/api.html)
+**[Documentation](https://gene-normalizer.readthedocs.io/latest/)** · [Installation](https://gene-normalizer.readthedocs.io/latest/install.html) · [Usage](https://gene-normalizer.readthedocs.io/latest/usage.html) · [API reference](https://gene-normalizer.readthedocs.io/latest/api/index.html)
 
 ---
 
 ## Install
 
 The Gene Normalizer is available on [PyPI](https://pypi.org/project/gene-normalizer/):
 
 ```shell
 python3 -m pip install gene-normalizer
 ```
 
-See [installation instruction](https://gene-normalizer.readthedocs.io/en/latest/install.html) in the documentation for a description of installation options and data setup requirements.
+See [installation instruction](https://gene-normalizer.readthedocs.io/latest/install.html) in the documentation for a description of installation options and data setup requirements.
 
 ## Examples
 
 Use the [live service](https://normalize.cancervariants.org/gene) to programmatically normalize gene terms, as in the following truncated example:
 
 ```shell
 $ curl 'https://normalize.cancervariants.org/gene/normalize?q=BRAF' | python -m json.tool
@@ -127,23 +128,23 @@
             "BRAF-1"
         ]
     }
     # ...
 }
 ```
 
-Or utilize the [Python API](https://gene-normalizer.readthedocs.io/en/latest/api/query_api.html) for fast access:
+Or utilize the [Python API](https://gene-normalizer.readthedocs.io/latest/api/query_api.html) for fast access:
 
 ```python
 >>> from gene.database import create_db
 >>> from gene.query import QueryHandler
 >>> q = QueryHandler(create_db())
 >>> result = q.normalize("KRAS")
 >>> result.normalized_id
 'hgnc:6407'
 ```
 
-See the [usage](https://gene-normalizer.readthedocs.io/en/latest/usage.html) and [normalization](https://gene-normalizer.readthedocs.io/en/latest/normalizing_data/normalization.html) entries in the documentation for more.
+See the [usage](https://gene-normalizer.readthedocs.io/latest/usage.html) and [normalization](https://gene-normalizer.readthedocs.io/latest/normalizing_data/normalization.html) entries in the documentation for more.
 
 ## Feedback and contributing
 
-We welcome bug reports, feature requests, and code contributions from users and interested collaborators. The [documentation](https://gene-normalizer.readthedocs.io/en/latest/contributing.html) contains guidance for submitting feedback and contributing new code.
+We welcome bug reports, feature requests, and code contributions from users and interested collaborators. The [documentation](https://gene-normalizer.readthedocs.io/latest/contributing.html) contains guidance for submitting feedback and contributing new code.
```

### Comparing `gene-normalizer-0.3.0.dev1/README.md` & `gene_normalizer-0.3.0.dev2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 <h1 align="center">
 Gene Normalizer
 </h1>
 
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/gene-normalizer?color=gr) [![tests](https://github.com/cancervariants/gene-normalization/actions/workflows/github-actions.yml/badge.svg)](https://github.com/cancervariants/gene-normalization/actions/workflows/github-actions.yml) [![DOI](https://zenodo.org/badge/309797998.svg)](https://zenodo.org/badge/latestdoi/309797998)
+[![image](https://img.shields.io/pypi/v/gene-normalizer.svg)](https://pypi.python.org/pypi/gene-normalizer) [![image](https://img.shields.io/pypi/l/gene-normalizer.svg)](https://pypi.python.org/pypi/gene-normalizer) [![image](https://img.shields.io/pypi/pyversions/gene-normalizer.svg)](https://pypi.python.org/pypi/gene-normalizer) [![Actions status](https://github.com/cancervariants/gene-normalization/actions/workflows/checks.yaml/badge.svg)](https://github.com/cancervariants/gene-normalization/actions/workflows/checks.yaml) [![DOI](https://zenodo.org/badge/309797998.svg)](https://zenodo.org/badge/latestdoi/309797998)
 
 ## Overview
-
+<!-- description -->
 The Gene Normalizer provides tools for resolving ambiguous human gene references to consistently-structured, normalized terms. For gene concepts extracted from [NCBI Gene](https://www.ncbi.nlm.nih.gov/gene/), [Ensembl](https://useast.ensembl.org/index.html), and [HGNC](https://www.genenames.org/), it designates a [CURIE](https://en.wikipedia.org/wiki/CURIE), and provides additional metadata like current and previously-used symbols, aliases, database cross-references and associations, and coordinates.
-
+<!-- /description -->
 ---
 
 **[Live service](https://normalize.cancervariants.org/gene)**
 
-**[Documentation](https://gene-normalizer.readthedocs.io/en/latest/)** · [Installation](https://gene-normalizer.readthedocs.io/en/latest/install.html) · [Usage](https://gene-normalizer.readthedocs.io/en/latest/usage.html) · [API reference](https://gene-normalizer.readthedocs.io/en/latest/api/api.html)
+**[Documentation](https://gene-normalizer.readthedocs.io/latest/)** · [Installation](https://gene-normalizer.readthedocs.io/latest/install.html) · [Usage](https://gene-normalizer.readthedocs.io/latest/usage.html) · [API reference](https://gene-normalizer.readthedocs.io/latest/api/index.html)
 
 ---
 
 ## Install
 
 The Gene Normalizer is available on [PyPI](https://pypi.org/project/gene-normalizer/):
 
 ```shell
 python3 -m pip install gene-normalizer
 ```
 
-See [installation instruction](https://gene-normalizer.readthedocs.io/en/latest/install.html) in the documentation for a description of installation options and data setup requirements.
+See [installation instruction](https://gene-normalizer.readthedocs.io/latest/install.html) in the documentation for a description of installation options and data setup requirements.
 
 ## Examples
 
 Use the [live service](https://normalize.cancervariants.org/gene) to programmatically normalize gene terms, as in the following truncated example:
 
 ```shell
 $ curl 'https://normalize.cancervariants.org/gene/normalize?q=BRAF' | python -m json.tool
@@ -50,23 +50,23 @@
             "BRAF-1"
         ]
     }
     # ...
 }
 ```
 
-Or utilize the [Python API](https://gene-normalizer.readthedocs.io/en/latest/api/query_api.html) for fast access:
+Or utilize the [Python API](https://gene-normalizer.readthedocs.io/latest/api/query_api.html) for fast access:
 
 ```python
 >>> from gene.database import create_db
 >>> from gene.query import QueryHandler
 >>> q = QueryHandler(create_db())
 >>> result = q.normalize("KRAS")
 >>> result.normalized_id
 'hgnc:6407'
 ```
 
-See the [usage](https://gene-normalizer.readthedocs.io/en/latest/usage.html) and [normalization](https://gene-normalizer.readthedocs.io/en/latest/normalizing_data/normalization.html) entries in the documentation for more.
+See the [usage](https://gene-normalizer.readthedocs.io/latest/usage.html) and [normalization](https://gene-normalizer.readthedocs.io/latest/normalizing_data/normalization.html) entries in the documentation for more.
 
 ## Feedback and contributing
 
-We welcome bug reports, feature requests, and code contributions from users and interested collaborators. The [documentation](https://gene-normalizer.readthedocs.io/en/latest/contributing.html) contains guidance for submitting feedback and contributing new code.
+We welcome bug reports, feature requests, and code contributions from users and interested collaborators. The [documentation](https://gene-normalizer.readthedocs.io/latest/contributing.html) contains guidance for submitting feedback and contributing new code.
```

### Comparing `gene-normalizer-0.3.0.dev1/src/gene/__init__.py` & `gene_normalizer-0.3.0.dev2/src/gene/__init__.py`

 * *Files identical despite different names*

### Comparing `gene-normalizer-0.3.0.dev1/src/gene/cli.py` & `gene_normalizer-0.3.0.dev2/src/gene/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
     except ModuleNotFoundError as e:
         click.echo(
             f"Encountered ModuleNotFoundError attempting to import {e.name}. {_etl_dependency_help}"
         )
         click.get_current_context().exit()
     SourceClass = eval(n.value)  # noqa: N806
 
-    source = SourceClass(database=db)
+    source = SourceClass(database=db, silent=False)
     try:
         processed_ids += source.perform_etl(use_existing)
     except GeneNormalizerEtlError as e:
         logger.error(e)
         click.echo(f"Encountered error while loading {n}: {e}.")
         click.get_current_context().exit()
     end_load = timer()
```

### Comparing `gene-normalizer-0.3.0.dev1/src/gene/database/database.py` & `gene_normalizer-0.3.0.dev2/src/gene/database/database.py`

 * *Files identical despite different names*

### Comparing `gene-normalizer-0.3.0.dev1/src/gene/database/dynamodb.py` & `gene_normalizer-0.3.0.dev2/src/gene/database/dynamodb.py`

 * *Files identical despite different names*

### Comparing `gene-normalizer-0.3.0.dev1/src/gene/database/postgresql/add_fkeys.sql` & `gene_normalizer-0.3.0.dev2/src/gene/database/postgresql/add_fkeys.sql`

 * *Files identical despite different names*

### Comparing `gene-normalizer-0.3.0.dev1/src/gene/database/postgresql/add_indexes.sql` & `gene_normalizer-0.3.0.dev2/src/gene/database/postgresql/add_indexes.sql`

 * *Files identical despite different names*

### Comparing `gene-normalizer-0.3.0.dev1/src/gene/database/postgresql/create_record_lookup_view.sql` & `gene_normalizer-0.3.0.dev2/src/gene/database/postgresql/create_record_lookup_view.sql`

 * *Files identical despite different names*

### Comparing `gene-normalizer-0.3.0.dev1/src/gene/database/postgresql/create_tables.sql` & `gene_normalizer-0.3.0.dev2/src/gene/database/postgresql/create_tables.sql`

 * *Files identical despite different names*

### Comparing `gene-normalizer-0.3.0.dev1/src/gene/database/postgresql/delete_normalized_concepts.sql` & `gene_normalizer-0.3.0.dev2/src/gene/database/postgresql/delete_normalized_concepts.sql`

 * *Files identical despite different names*

### Comparing `gene-normalizer-0.3.0.dev1/src/gene/database/postgresql.py` & `gene_normalizer-0.3.0.dev2/src/gene/database/postgresql.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,27 +51,27 @@
             * user: Postgres username
             * password: Postgres password (optional or blank if unneeded)
             * db_name: name of database to connect to
 
         :raise DatabaseInitializationException: if initial setup fails
         """
         if db_url:
-            conninfo = db_url
+            self.conninfo = db_url
         elif "GENE_NORM_DB_URL" in os.environ:
-            conninfo = os.environ["GENE_NORM_DB_URL"]
+            self.conninfo = os.environ["GENE_NORM_DB_URL"]
         else:
             user = db_args.get("user", "postgres")
             password = db_args.get("password", "")
             db_name = db_args.get("db_name", "gene_normalizer")
             if password:
-                conninfo = f"dbname={db_name} user={user} password={password}"
+                self.conninfo = f"postgresql://{user}:{password}@/{db_name}"
             else:
-                conninfo = f"dbname={db_name} user={user}"
+                self.conninfo = f"postgresql://{user}@/{db_name}"
 
-        self.conn = psycopg.connect(conninfo)
+        self.conn = psycopg.connect(self.conninfo)
         self.initialize_db()
         self._cached_sources = {}
 
         atexit.register(self.close_connection)
 
     _list_tables_query = b"""
     SELECT table_name FROM information_schema.tables
@@ -542,20 +542,24 @@
     INSERT INTO gene_concepts (
         concept_id, source, symbol_status, label,
         strand, location_annotations, locations, gene_type
     )
     VALUES (%s, %s, %s, %s, %s, %s, %s, %s);
     """
     _ins_symbol_query = (
-        b"INSERT INTO gene_symbols (symbol, concept_id) VALUES (%s, %s);"  # noqa: E501
+        b"INSERT INTO gene_symbols (symbol, concept_id) VALUES (%s, %s);"
+    )
+    _ins_prev_symbol_query = (
+        b"INSERT INTO gene_previous_symbols (prev_symbol, concept_id) VALUES (%s, %s);"
     )
-    _ins_prev_symbol_query = b"INSERT INTO gene_previous_symbols (prev_symbol, concept_id) VALUES (%s, %s);"  # noqa: E501
     _ins_alias_query = b"INSERT INTO gene_aliases (alias, concept_id) VALUES (%s, %s);"
     _ins_xref_query = b"INSERT INTO gene_xrefs (xref, concept_id) VALUES (%s, %s);"
-    _ins_assoc_query = b"INSERT INTO gene_associations (associated_with, concept_id) VALUES (%s, %s);"  # noqa: E501
+    _ins_assoc_query = (
+        b"INSERT INTO gene_associations (associated_with, concept_id) VALUES (%s, %s);"
+    )
 
     def add_record(self, record: Dict, src_name: SourceName) -> None:
         """Add new record to database.
 
         :param record: record to upload
         :param src_name: name of source for record. Not used by PostgreSQL instance.
         """
@@ -798,25 +802,20 @@
             tar = tarfile.open(temp_tarfile, "r:gz")
             tar_dump_file = [
                 f for f in tar.getmembers() if f.name.startswith("gene_norm_")
             ][0]
             tar.extractall(path=tempdir_path, members=[tar_dump_file])
             dump_file = tempdir_path / tar_dump_file.name
 
-            if self.conn.info.password:
-                pw_param = f"-W {self.conn.info.password}"
-            else:
-                pw_param = "-w"
-
             self.drop_db()
-            system_call = f"psql -d {self.conn.info.dbname} -U {self.conn.info.user} {pw_param} -f {dump_file.absolute()}"  # noqa: E501
+            system_call = f"psql {self.conninfo} -f {dump_file.absolute()}"
             result = os.system(system_call)
         if result != 0:
             raise DatabaseException(
-                f"System call '{result}' returned failing exit code."
+                f"System call '{system_call}' returned failing exit code {result}."
             )
 
     def export_db(self, output_directory: Path) -> None:
         """Dump DB to specified location.
 
         :param export_location: path to directory to save DB dump in
         :return: Nothing, but saves results of pg_dump to file named
@@ -826,22 +825,13 @@
         """
         if not output_directory.is_dir() or not output_directory.exists():
             raise ValueError(
                 f"Output location {output_directory} isn't a directory or doesn't exist"
             )  # noqa: E501
         now = datetime.now().strftime("%Y%m%d%H%M%S")
         output_location = output_directory / f"gene_norm_{now}.sql"
-        user = self.conn.info.user
-        host = self.conn.info.host
-        port = self.conn.info.port
-        database_name = self.conn.info.dbname
-        if self.conn.info.password:
-            pw_param = f"-W {self.conn.info.password}"
-        else:
-            pw_param = "-w"
-
-        system_call = f"pg_dump -E UTF8 -f {output_location} -U {user} {pw_param} -h {host} -p {port} {database_name}"  # noqa: E501
+        system_call = f"pg_dump {self.conninfo} -E UTF8 -f {output_location}"
         result = os.system(system_call)
         if result != 0:
             raise DatabaseException(
-                f"System call '{system_call}' returned failing exit code."
+                f"System call '{system_call}' returned failing exit code {result}."
             )
```

### Comparing `gene-normalizer-0.3.0.dev1/src/gene/etl/base.py` & `gene_normalizer-0.3.0.dev2/src/gene/etl/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,121 +1,108 @@
 """A base class for extraction, transformation, and loading of data."""
-import datetime
-import gzip
 import logging
 import re
-import shutil
 from abc import ABC, abstractmethod
-from ftplib import FTP
-from os import remove
 from pathlib import Path
-from typing import Callable, Dict, List, Optional
+from typing import Dict, List, Optional, Union
 
+import click
 import pydantic
 from biocommons.seqrepo import SeqRepo
-from dateutil import parser
 from gffutils.feature import Feature
+from wags_tails import EnsemblData, HgncData, NcbiGeneData
 
 from gene import ITEM_TYPES, SEQREPO_ROOT_DIR
 from gene.database import AbstractDatabase
 from gene.schemas import Gene, GeneSequenceLocation, MatchType, SourceName
 
 logger = logging.getLogger("gene")
 logger.setLevel(logging.DEBUG)
 
 
+DATA_DISPATCH = {
+    SourceName.HGNC: HgncData,
+    SourceName.ENSEMBL: EnsemblData,
+    SourceName.NCBI: NcbiGeneData,
+}
+
+
 class Base(ABC):
     """The ETL base class."""
 
     def __init__(
         self,
         database: AbstractDatabase,
-        host: str,
-        data_dir: str,
-        src_data_dir: Path,
         seqrepo_dir: Path = SEQREPO_ROOT_DIR,
+        data_path: Optional[Path] = None,
+        silent: bool = True,
     ) -> None:
         """Instantiate Base class.
 
         :param database: database instance
-        :param host: Hostname of FTP site
-        :param data_dir: Data directory of FTP site to look at
-        :param src_data_dir: Data directory for source
         :param seqrepo_dir: Path to seqrepo directory
+        :param data_path: path to app data directory
+        :param silent: if True, don't print ETL result to console
         """
-        self.src_data_dir = src_data_dir
-        self.src_data_dir.mkdir(exist_ok=True, parents=True)
+        self._silent = silent
         self._src_name = SourceName(self.__class__.__name__)
+        self._data_source = self._get_data_handler(data_path)
         self._database = database
-        self._host = host
-        self._data_dir = data_dir
-        self._processed_ids = list()
         self.seqrepo = self.get_seqrepo(seqrepo_dir)
+        self._processed_ids = list()
 
-    def perform_etl(self, use_existing: bool = False) -> List[str]:
-        """Extract, Transform, and Load data into database.
+    def _get_data_handler(
+        self, data_path: Optional[Path] = None
+    ) -> Union[HgncData, EnsemblData, NcbiGeneData]:
+        """Construct data handler instance for source. Overwrite for edge-case sources.
 
-        :param use_existing: if true, use most recent available local files
-        :return: Concept IDs of concepts successfully loaded
+        :param data_path: location of data storage
+        :return: instance of wags_tails.DataSource to manage source file(s)
+        """
+        return DATA_DISPATCH[self._src_name](data_dir=data_path, silent=self._silent)
+
+    def perform_etl(self, use_existing: bool = False) -> List[str]:
+        """Public-facing method to begin ETL procedures on given data.
+        Returned concept IDs can be passed to Merge method for computing
+        merged concepts.
+
+        :param use_existing: if True, don't try to retrieve latest source data
+        :return: list of concept IDs which were successfully processed and
+            uploaded.
         """
         self._extract_data(use_existing)
+        if not self._silent:
+            click.echo("Transforming and loading data to DB...")
         self._add_meta()
         self._transform_data()
         self._database.complete_write_transaction()
         return self._processed_ids
 
-    @abstractmethod
-    def _extract_data(self, *args, **kwargs) -> None:  # noqa: ANN002
-        """Extract data from FTP site or local data directory."""
-        raise NotImplementedError
+    def _extract_data(self, use_existing: bool) -> None:
+        """Acquire source data.
+
+        This method is responsible for initializing an instance of a data handler and,
+        in most cases, setting ``self._data_file`` and ``self._version``.
+
+        :param bool use_existing: if True, don't try to fetch latest source data
+        """
+        self._data_file, self._version = self._data_source.get_latest(
+            from_local=use_existing
+        )
 
     @abstractmethod
     def _transform_data(self) -> None:
         """Transform data to model."""
         raise NotImplementedError
 
     @abstractmethod
     def _add_meta(self) -> None:
         """Add source meta to database source info."""
         raise NotImplementedError
 
-    def _acquire_data_file(
-        self,
-        file_glob: str,
-        use_existing: bool,
-        check_latest_callback: Callable[[Path], bool],
-        download_callback: Callable[[], Path],
-    ) -> Path:
-        """Acquire data file.
-
-        :param file_glob: pattern to match relevant files against
-        :param use_existing: don't fetch from remote origin if local versions are
-            available
-        :param check_latest_callback: function to check whether local data is up-to-date
-        :param download_callback: function to download from remote
-        :return: path to acquired data file
-        :raise FileNotFoundError: if unable to find any files matching the pattern
-        """
-        matching_files = list(self.src_data_dir.glob(file_glob))
-        if not matching_files:
-            if use_existing:
-                raise FileNotFoundError(
-                    f"No local files matching pattern {self.src_data_dir.absolute().as_uri() + file_glob}"
-                )
-            else:
-                return download_callback()
-        else:
-            latest_file = list(sorted(matching_files))[-1]
-            if use_existing:
-                return latest_file
-            if not check_latest_callback(latest_file):
-                return download_callback()
-            else:
-                return latest_file
-
     def _load_gene(self, gene: Dict) -> None:
         """Load a gene record into database. This method takes responsibility for:
          * validating structure correctness
          * removing duplicates from list-like fields
          * removing empty fields
 
         :param gene: Gene record
@@ -138,57 +125,14 @@
                     elif isinstance(value, str):
                         continue
                     gene[attr_type] = list(set(value))
 
             self._database.add_record(gene, self._src_name)
             self._processed_ids.append(concept_id)
 
-    def _ftp_download(
-        self, host: str, data_dir: str, fn: str, source_dir: Path, data_fn: str
-    ) -> Optional[str]:
-        """Download data file from FTP site.
-
-        :param host: Source's FTP host name
-        :param data_dir: Data directory located on FTP site
-        :param fn: Filename for downloaded file
-        :param source_dir: Source's data directory
-        :param data_fn: Filename on FTP site to be downloaded
-        :return: Date file was last updated
-        """
-        with FTP(host) as ftp:
-            ftp.login()
-            timestamp = ftp.voidcmd(f"MDTM {data_dir}{data_fn}")[4:].strip()
-            date = str(parser.parse(timestamp)).split()[0]
-            version = datetime.datetime.strptime(date, "%Y-%m-%d").strftime("%Y%m%d")
-            ftp.cwd(data_dir)
-            self._ftp_download_file(ftp, data_fn, source_dir, fn)
-        return version
-
-    def _ftp_download_file(
-        self, ftp: FTP, data_fn: str, source_dir: Path, fn: str
-    ) -> None:
-        """Download data file from FTP
-
-        :param ftp: FTP instance
-        :param data_fn: Filename on FTP site to be downloaded
-        :param source_dir: Source's data directory
-        :param fn: Filename for downloaded file
-        """
-        if data_fn.endswith(".gz"):
-            filepath = source_dir / f"{fn}.gz"
-        else:
-            filepath = source_dir / fn
-        with open(filepath, "wb") as fp:
-            ftp.retrbinary(f"RETR {data_fn}", fp.write)
-        if data_fn.endswith(".gz"):
-            with gzip.open(filepath, "rb") as f_in:
-                with open(source_dir / fn, "wb") as f_out:
-                    shutil.copyfileobj(f_in, f_out)
-            remove(filepath)
-
     def get_seqrepo(self, seqrepo_dir: Path) -> SeqRepo:
         """Return SeqRepo instance if seqrepo_dir exists.
 
         :param seqrepo_dir: Path to seqrepo directory
         :return: SeqRepo instance
         """
         if not Path(seqrepo_dir).exists():
```

### Comparing `gene-normalizer-0.3.0.dev1/src/gene/etl/merge.py` & `gene_normalizer-0.3.0.dev2/src/gene/etl/merge.py`

 * *Files identical despite different names*

### Comparing `gene-normalizer-0.3.0.dev1/src/gene/etl/ncbi.py` & `gene_normalizer-0.3.0.dev2/src/gene/etl/ncbi.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """Defines ETL methods for the NCBI data source."""
 import csv
 import logging
 import re
-import shutil
-from ftplib import FTP
 from pathlib import Path
 from typing import Dict, List, Optional
 
 import gffutils
+from wags_tails import NcbiGenomeData
+from wags_tails.ncbi import NcbiGenePaths
 
-from gene import APP_ROOT, PREFIX_LOOKUP
+from gene import PREFIX_LOOKUP, SEQREPO_ROOT_DIR
 from gene.database import AbstractDatabase
 from gene.etl.base import Base
 from gene.etl.exceptions import (
-    GeneFileVersionError,
     GeneNormalizerEtlError,
-    GeneSourceFetchError,
 )
 from gene.schemas import (
     Annotation,
     Chromosome,
     NamespacePrefix,
     SourceMeta,
     SourceName,
@@ -32,215 +30,47 @@
 
 class NCBI(Base):
     """ETL class for NCBI source"""
 
     def __init__(
         self,
         database: AbstractDatabase,
-        host: str = "ftp.ncbi.nlm.nih.gov",
-        data_dir: str = "gene/DATA/",
-        src_data_dir: Path = APP_ROOT / "data" / "ncbi",
+        seqrepo_dir: Path = SEQREPO_ROOT_DIR,
+        data_path: Optional[Path] = None,
+        silent: bool = True,
     ) -> None:
-        """Construct the NCBI ETL instance.
+        """Instantiate Base class.
 
-        :param database: gene database for adding new data
-        :param host: FTP host name
-        :param data_dir: FTP data directory to use
-        :param src_data_dir: Data directory for NCBI
+        :param database: database instance
+        :param seqrepo_dir: Path to seqrepo directory
+        :param data_path: path to app data directory
+        :param silent: if True, don't print ETL result to console
         """
-        super().__init__(database, host, data_dir, src_data_dir)
-        self._ftp_hostname = host
-        self._assembly = None
-        self._gene_url = None
-        self._history_url = None
-        self._assembly_url = None
-
-    @staticmethod
-    def _navigate_ftp_genome_assembly(ftp: FTP) -> None:
-        """Navigate NCBI FTP filesystem to directory containing latest assembly annotation data.
-
-        :param ftp: logged-in FTP instance
-        :return: None, but modifies FTP connection in-place
-        :raise SourceFetchError: if navigation fails (e.g. because expected directories don't exist)
-        """
-        major_annotation_pattern = r"GCF_\d+\.\d+_GRCh\d+.+"
-        ftp.cwd(
-            "genomes/refseq/vertebrate_mammalian/Homo_sapiens/"
-            "latest_assembly_versions"
-        )
-        try:
-            grch_dirs = [d for d in ftp.nlst() if re.match(major_annotation_pattern, d)]
-            grch_dir = grch_dirs[0]
-        except (IndexError, AttributeError):
-            raise GeneSourceFetchError(
-                "No directories matching expected latest assembly version pattern"
-            )
-        ftp.cwd(grch_dir)
-
-    def _gff_is_up_to_date(self, gff: Path) -> bool:
-        """Verify whether local GRCh38 annotation file is up-to-date. Currently, their
-        API endpoints require auth keys (adding complexity for new users) and may or may not
-        give us exactly what we want, so we ascertain version availability by manually
-        checking what's listed in the FTP filesystem.
-
-        :param gff: path to local GFF file (file should be saved like `ncbi_GRCh38.p14.gff`)
-        :return: True if file version matches most recent known remote version
-        :raise GeneFileVersionError: if unable to parse version from local or remote file
-        :raise GeneSourceFetchError: if unable to get version from NCBI
-        """
-        try:
-            version = re.match(r"ncbi_(.+)", gff.stem).groups()[0]
-        except (IndexError, AttributeError):
-            raise GeneFileVersionError(
-                f"Unable to parse version from NCBI GRCh38 annotation file: {gff.absolute()}"
-            )
-
-        genomic_gff_pattern = r"GCF_\d+\.\d+_(GRCh\d+\.\w\d+)_genomic.gff.gz"
-        with FTP(self._host) as ftp:
-            ftp.login()
-            self._navigate_ftp_genome_assembly(ftp)
-            for file in ftp.nlst():
-                match = re.match(genomic_gff_pattern, file)
-                if match and match.groups():
-                    latest_version = match.groups()[0]
-                    return version == latest_version
-        raise GeneSourceFetchError(
-            "Unable to identify latest available NCBI GRCh38 annotation version"
-        )
-
-    def _download_gff(self) -> Path:
-        """Download NCBI GRCh38 annotation file.
-
-        :return: Path to downloaded file
-        :raise SourceFetchError: if unable to identify latest available file
-        """
-        logger.info("Downloading NCBI genome annotation file...")
-        genomic_gff_pattern = r"GCF_\d+\.\d+_(GRCh\d+\.\w\d+)_genomic.gff.gz"
-        with FTP(self._host) as ftp:
-            ftp.login()
-            self._navigate_ftp_genome_assembly(ftp)
-            genomic_filename = None
-            version = None
-            for f in ftp.nlst():
-                gff_match = re.match(genomic_gff_pattern, f)
-                if gff_match and gff_match.groups():
-                    genomic_filename = f
-                    version = gff_match.groups()[0]
-            if not version or not genomic_filename:
-                raise GeneSourceFetchError(
-                    "Unable to find latest available NCBI GRCh38 annotation"
-                )
-            new_filename = f"ncbi_{version}.gff"
-            self._ftp_download_file(
-                ftp, genomic_filename, self.src_data_dir, new_filename
-            )
-        logger.info(
-            f"Downloaded NCBI genome annotation file to {self.src_data_dir / new_filename}"
-        )
-        return self.src_data_dir / new_filename
-
-    def _history_file_is_up_to_date(self, history_file: Path) -> bool:
-        """Verify whether local NCBI name history file is up-to-date.
-
-        :param history_file: path to local history file (file should be saved like `ncbi_history_20230315.tsv`)
-        :return: True if file version matches most recent expected remote version
-        :raise GeneFileVersionError: if parsing version from local file fails
-        """
-        try:
-            version = re.match(r"ncbi_history_(\d+).tsv", history_file.name).groups()[0]
-        except (IndexError, AttributeError):
-            raise GeneFileVersionError(
-                f"Unable to parse version from NCBI history file: {history_file.absolute()}"
-            )
-        with FTP(self._host) as ftp:
-            ftp.login()
-            ftp.cwd("gene/DATA/")
-            file_changed_date = ftp.sendcmd("MDTM gene_history.gz")[4:12]
-        return version == file_changed_date
-
-    def _download_history_file(self) -> Path:
-        """Download NCBI gene name history file
-
-        :return: Path to downloaded file
-        """
-        logger.info("Downloading NCBI gene_history...")
-        tmp_fn = "ncbi_history_tmp.tsv"
-        data_fn = "gene_history.gz"
-        version = self._ftp_download(
-            self._host, self._data_dir, tmp_fn, self.src_data_dir, data_fn
-        )
-        final_location = f"{self.src_data_dir}/ncbi_history_{version}.tsv"
-        shutil.move(f"{self.src_data_dir}/{tmp_fn}", final_location)
-        logger.info(f"Successfully downloaded NCBI gene_history to {final_location}.")
-        return Path(final_location)
-
-    def _gene_file_is_up_to_date(self, gene_file: Path) -> bool:
-        """Verify whether local NCBI gene info file is up-to-date.
-
-        :param gene_file: path to local NCBI info file (file should be saved like `ncbi_info_20230315.tsv`)
-        :return: True if file version matches most recent known remote version
-        :raise GeneFileVersionError: if parsing version from local file fails
-        """
-        try:
-            version = re.match(r"ncbi_info_(\d+).tsv", gene_file.name).groups()[0]
-        except (IndexError, AttributeError):
-            raise GeneFileVersionError(
-                f"Unable to parse version from NCBI gene file: {gene_file.absolute()}"
-            )
-        with FTP(self._host) as ftp:
-            ftp.login()
-            ftp.cwd("gene/DATA/GENE_INFO/Mammalia/")
-            file_changed_date = ftp.sendcmd("MDTM Homo_sapiens.gene_info.gz")[4:12]
-        return version == file_changed_date
-
-    def _download_gene_file(self) -> Path:
-        """Download NCBI gene info file
-
-        :return: Path to downloaded file
-        """
-        data_dir = f"{self._data_dir}GENE_INFO/Mammalia/"
-        tmp_fn = "ncbi_info_tmp.tsv"
-        data_fn = "Homo_sapiens.gene_info.gz"
-        logger.info("Downloading NCBI gene_info....")
-        version = self._ftp_download(
-            self._host, data_dir, tmp_fn, self.src_data_dir, data_fn
-        )
-        final_location = f"{self.src_data_dir}/ncbi_info_{version}.tsv"
-        shutil.move(f"{self.src_data_dir}/{tmp_fn}", final_location)
-        logger.info(f"Successfully downloaded NCBI gene_info to {final_location}.")
-        return Path(final_location)
+        super().__init__(database, seqrepo_dir, data_path, silent)
+        self._genome_data_handler = NcbiGenomeData(data_path, silent)
 
     def _extract_data(self, use_existing: bool) -> None:
         """Acquire NCBI data file and get metadata.
 
         :param use_existing: if True, use latest available local file
         """
-        self._gff_src = self._acquire_data_file(
-            "ncbi_GRCh*.gff", use_existing, self._gff_is_up_to_date, self._download_gff
-        )
-        self._info_src = self._acquire_data_file(
-            "ncbi_info_*.tsv",
-            use_existing,
-            self._gene_file_is_up_to_date,
-            self._download_gene_file,
+        self._gff_src, self._assembly = self._genome_data_handler.get_latest(
+            from_local=use_existing
         )
-        self._version = self._info_src.stem.split("_")[-1]
-        self._history_src = self._acquire_data_file(
-            f"ncbi_history_{self._version}.tsv",
-            use_existing,
-            self._history_file_is_up_to_date,
-            self._download_history_file,
-        )
-
-        self._assembly = self._gff_src.stem.split("_")[-1]
+        gene_paths: NcbiGenePaths
+        gene_paths, self._version = self._data_source.get_latest(
+            from_local=use_existing
+        )  # type: ignore
+        self._info_src = gene_paths.gene_info
+        self._history_src = gene_paths.gene_history
         self._gene_url = (
-            f"{self._host}gene/DATA/GENE_INFO/Mammalia/Homo_sapiens.gene_info.gz"
+            "ftp.ncbi.nlm.nih.govgene/DATA/GENE_INFO/Mammalia/Homo_sapiens.gene_info.gz"
         )
-        self._history_url = f"{self._host}gene/DATA/gene_history.gz"
-        self._assembly_url = f"{self._host}genomes/refseq/vertebrate_mammalian/Homo_sapiens/latest_assembly_versions/"
+        self._history_url = "ftp.ncbi.nlm.nih.govgene/DATA/gene_history.gz"
+        self._assembly_url = "ftp.ncbi.nlm.nih.govgenomes/refseq/vertebrate_mammalian/Homo_sapiens/latest_assembly_versions/"
 
     def _get_prev_symbols(self) -> Dict[str, str]:
         """Store a gene's symbol history.
 
         :return: A dictionary of a gene's previous symbols
         """
         # get symbol history
```

### Comparing `gene-normalizer-0.3.0.dev1/src/gene/main.py` & `gene_normalizer-0.3.0.dev2/src/gene/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     operation_id="getUnmergedRecords",
     response_description=unmerged_response_descr,
     response_model=UnmergedNormalizationService,
     description=unmerged_normalize_description,
     tags=["Query"],
 )
 def normalize_unmerged(
-    q: str = Query(..., description=normalize_q_descr)
+    q: str = Query(..., description=normalize_q_descr),
 ) -> UnmergedNormalizationService:
     """Return all individual records associated with a normalized concept.
 
     :param q: Gene search term
     :returns: JSON response with matching normalized record and source metadata
     """
     response = query_handler.normalize_unmerged(html.unescape(q))
```

### Comparing `gene-normalizer-0.3.0.dev1/src/gene/query.py` & `gene_normalizer-0.3.0.dev2/src/gene/query.py`

 * *Files identical despite different names*

### Comparing `gene-normalizer-0.3.0.dev1/src/gene/schemas.py` & `gene_normalizer-0.3.0.dev2/src/gene/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,16 +90,15 @@
     concept_id: CURIE
     symbol: StrictStr
     symbol_status: Optional[SymbolStatus] = None
     label: Optional[StrictStr] = None
     strand: Optional[Strand] = None
     location_annotations: List[StrictStr] = []
     locations: Union[
-        List[models.SequenceLocation],
-        List[GeneSequenceLocation]
+        List[models.SequenceLocation], List[GeneSequenceLocation]
         # List[Union[SequenceLocation, ChromosomeLocation]],
         # List[Union[GeneSequenceLocation, GeneChromosomeLocation]]  # dynamodb
     ] = []
     aliases: List[StrictStr] = []
     previous_symbols: List[StrictStr] = []
     xrefs: List[CURIE] = []
     associated_with: List[CURIE] = []
```

### Comparing `gene-normalizer-0.3.0.dev1/src/gene_normalizer.egg-info/PKG-INFO` & `gene_normalizer-0.3.0.dev2/src/gene_normalizer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gene-normalizer
-Version: 0.3.0.dev1
+Version: 0.3.0.dev2
 Summary: VICC normalization routines for genes
 Author: Alex Wagner, Kori Kuzma, James Stevenson
 License: MIT License
         
-        Copyright (c) 2020-2023 VICC
+        Copyright (c) 2020-2024 VICC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -53,59 +53,60 @@
 Requires-Dist: boto3
 Requires-Dist: ga4gh.vrs~=2.0.0a1
 Provides-Extra: pg
 Requires-Dist: psycopg[binary]; extra == "pg"
 Provides-Extra: etl
 Requires-Dist: gffutils; extra == "etl"
 Requires-Dist: biocommons.seqrepo; extra == "etl"
+Requires-Dist: wags-tails>=0.1.1; extra == "etl"
 Provides-Extra: test
 Requires-Dist: pytest>=6.0; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: mock; extra == "test"
 Requires-Dist: httpx; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: ruff; extra == "dev"
+Requires-Dist: ruff==0.2.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx==6.1.3; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints==1.22.0; extra == "docs"
 Requires-Dist: sphinx-autobuild==2021.3.14; extra == "docs"
 Requires-Dist: sphinx-copybutton==0.5.2; extra == "docs"
 Requires-Dist: sphinxext-opengraph==0.8.2; extra == "docs"
 Requires-Dist: furo==2023.3.27; extra == "docs"
 Requires-Dist: gravis==0.1.0; extra == "docs"
+Requires-Dist: sphinx-github-changelog==1.2.1; extra == "docs"
 
 <h1 align="center">
 Gene Normalizer
 </h1>
 
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/gene-normalizer?color=gr) [![tests](https://github.com/cancervariants/gene-normalization/actions/workflows/github-actions.yml/badge.svg)](https://github.com/cancervariants/gene-normalization/actions/workflows/github-actions.yml) [![DOI](https://zenodo.org/badge/309797998.svg)](https://zenodo.org/badge/latestdoi/309797998)
+[![image](https://img.shields.io/pypi/v/gene-normalizer.svg)](https://pypi.python.org/pypi/gene-normalizer) [![image](https://img.shields.io/pypi/l/gene-normalizer.svg)](https://pypi.python.org/pypi/gene-normalizer) [![image](https://img.shields.io/pypi/pyversions/gene-normalizer.svg)](https://pypi.python.org/pypi/gene-normalizer) [![Actions status](https://github.com/cancervariants/gene-normalization/actions/workflows/checks.yaml/badge.svg)](https://github.com/cancervariants/gene-normalization/actions/workflows/checks.yaml) [![DOI](https://zenodo.org/badge/309797998.svg)](https://zenodo.org/badge/latestdoi/309797998)
 
 ## Overview
-
+<!-- description -->
 The Gene Normalizer provides tools for resolving ambiguous human gene references to consistently-structured, normalized terms. For gene concepts extracted from [NCBI Gene](https://www.ncbi.nlm.nih.gov/gene/), [Ensembl](https://useast.ensembl.org/index.html), and [HGNC](https://www.genenames.org/), it designates a [CURIE](https://en.wikipedia.org/wiki/CURIE), and provides additional metadata like current and previously-used symbols, aliases, database cross-references and associations, and coordinates.
-
+<!-- /description -->
 ---
 
 **[Live service](https://normalize.cancervariants.org/gene)**
 
-**[Documentation](https://gene-normalizer.readthedocs.io/en/latest/)** · [Installation](https://gene-normalizer.readthedocs.io/en/latest/install.html) · [Usage](https://gene-normalizer.readthedocs.io/en/latest/usage.html) · [API reference](https://gene-normalizer.readthedocs.io/en/latest/api/api.html)
+**[Documentation](https://gene-normalizer.readthedocs.io/latest/)** · [Installation](https://gene-normalizer.readthedocs.io/latest/install.html) · [Usage](https://gene-normalizer.readthedocs.io/latest/usage.html) · [API reference](https://gene-normalizer.readthedocs.io/latest/api/index.html)
 
 ---
 
 ## Install
 
 The Gene Normalizer is available on [PyPI](https://pypi.org/project/gene-normalizer/):
 
 ```shell
 python3 -m pip install gene-normalizer
 ```
 
-See [installation instruction](https://gene-normalizer.readthedocs.io/en/latest/install.html) in the documentation for a description of installation options and data setup requirements.
+See [installation instruction](https://gene-normalizer.readthedocs.io/latest/install.html) in the documentation for a description of installation options and data setup requirements.
 
 ## Examples
 
 Use the [live service](https://normalize.cancervariants.org/gene) to programmatically normalize gene terms, as in the following truncated example:
 
 ```shell
 $ curl 'https://normalize.cancervariants.org/gene/normalize?q=BRAF' | python -m json.tool
@@ -127,23 +128,23 @@
             "BRAF-1"
         ]
     }
     # ...
 }
 ```
 
-Or utilize the [Python API](https://gene-normalizer.readthedocs.io/en/latest/api/query_api.html) for fast access:
+Or utilize the [Python API](https://gene-normalizer.readthedocs.io/latest/api/query_api.html) for fast access:
 
 ```python
 >>> from gene.database import create_db
 >>> from gene.query import QueryHandler
 >>> q = QueryHandler(create_db())
 >>> result = q.normalize("KRAS")
 >>> result.normalized_id
 'hgnc:6407'
 ```
 
-See the [usage](https://gene-normalizer.readthedocs.io/en/latest/usage.html) and [normalization](https://gene-normalizer.readthedocs.io/en/latest/normalizing_data/normalization.html) entries in the documentation for more.
+See the [usage](https://gene-normalizer.readthedocs.io/latest/usage.html) and [normalization](https://gene-normalizer.readthedocs.io/latest/normalizing_data/normalization.html) entries in the documentation for more.
 
 ## Feedback and contributing
 
-We welcome bug reports, feature requests, and code contributions from users and interested collaborators. The [documentation](https://gene-normalizer.readthedocs.io/en/latest/contributing.html) contains guidance for submitting feedback and contributing new code.
+We welcome bug reports, feature requests, and code contributions from users and interested collaborators. The [documentation](https://gene-normalizer.readthedocs.io/latest/contributing.html) contains guidance for submitting feedback and contributing new code.
```

### Comparing `gene-normalizer-0.3.0.dev1/src/gene_normalizer.egg-info/SOURCES.txt` & `gene_normalizer-0.3.0.dev2/src/gene_normalizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

