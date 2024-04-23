# Comparing `tmp/pyodmongo-0.7.3.tar.gz` & `tmp/pyodmongo-0.8.0.tar.gz`

## Comparing `pyodmongo-0.7.3.tar` & `pyodmongo-0.8.0.tar`

### file list

```diff
@@ -1,83 +1,84 @@
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/code_of_conduct.md
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/coverage.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/mkdocs.yml
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/pyproject.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/requirements.txt
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/.github/workflows/black_formatter.yml
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/.github/workflows/publishing_docs_s3.yml
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/.github/workflows/python_publish.yml
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/.github/workflows/tests.yml
--rw-r--r--   0        0        0    56292 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/docs/assets/images/favicon.png
--rw-r--r--   0        0        0    94192 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/docs/assets/images/insomnia_request.png
--rw-r--r--   0        0        0    57259 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/docs/assets/images/logo.png
--rw-r--r--   0        0        0    70935 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/docs/assets/images/pyodmongo_Logo_BG_Dark.png
--rw-r--r--   0        0        0    72399 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/docs/assets/images/pyodmongo_Logo_BG_White.png
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/docs/en/aggregation.md
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/docs/en/contributing.md
--rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/docs/en/db_model.md
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/docs/en/delete.md
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/docs/en/fastapi.md
--rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/docs/en/find.md
--rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/docs/en/getting_started.md
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/docs/en/index.md
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/docs/en/indexes.md
--rw-r--r--   0        0        0     7727 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/docs/en/query.md
--rw-r--r--   0        0        0     4849 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/docs/en/save.md
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/docs/pt-BR/aggregation.md
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/docs/pt-BR/contributing.md
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/docs/pt-BR/db_model.md
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/docs/pt-BR/delete.md
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/docs/pt-BR/fastapi.md
--rw-r--r--   0        0        0     7543 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/docs/pt-BR/find.md
--rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/docs/pt-BR/getting_started.md
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/docs/pt-BR/index.md
--rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/docs/pt-BR/indexes.md
--rw-r--r--   0        0        0     7888 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/docs/pt-BR/query.md
--rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/docs/pt-BR/save.md
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/docs/stylesheets/extras.css
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/pyodmongo/__init__.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/pyodmongo/version.py
--rw-r--r--   0        0        0     9674 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/pyodmongo/async_engine/engine.py
--rw-r--r--   0        0        0     9399 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/pyodmongo/engine/engine.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/pyodmongo/engine/utils.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/pyodmongo/models/db_field_info.py
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/pyodmongo/models/db_model.py
--rw-r--r--   0        0        0     9486 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/pyodmongo/models/fields.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/pyodmongo/models/id_model.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/pyodmongo/models/paginate.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/pyodmongo/models/query_operators.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/pyodmongo/models/responses.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/pyodmongo/queries/__init__.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/pyodmongo/queries/comparison_operators.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/pyodmongo/queries/logical_operators.py
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/pyodmongo/queries/query_string.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/pyodmongo/queries/sort_operator.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/pyodmongo/services/aggregate_stages.py
--rw-r--r--   0        0        0     7386 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/pyodmongo/services/model_init.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/pyodmongo/services/query_operators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/tests/__init__.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/tests/conftest.py
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/tests/test_async_aggregate.py
--rw-r--r--   0        0        0    18182 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/tests/test_async_crud_db.py
--rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/tests/test_class.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/tests/test_db_field_info.py
--rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/tests/test_db_index.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/tests/test_dict_empty.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/tests/test_fastapi.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/tests/test_model_init_functions.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/tests/test_object_id.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/tests/test_project_pipeline.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/tests/test_pydantic_validators.py
--rw-r--r--   0        0        0     9990 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/tests/test_queries.py
--rw-r--r--   0        0        0     9193 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/tests/test_reference_pipeline.py
--rw-r--r--   0        0        0     8320 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/tests/test_save_dict.py
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/tests/test_sync_aggregate.py
--rw-r--r--   0        0        0    12269 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/tests/test_sync_crud_db.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/tests/test_version.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/LICENSE
--rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/README.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 pyodmongo-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/code_of_conduct.md
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/coverage.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/mkdocs.yml
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/pyproject.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/requirements.txt
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/.github/workflows/black_formatter.yml
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/.github/workflows/publishing_docs_s3.yml
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/.github/workflows/python_publish.yml
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0    56292 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/docs/assets/images/favicon.png
+-rw-r--r--   0        0        0    94192 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/docs/assets/images/insomnia_request.png
+-rw-r--r--   0        0        0    57259 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/docs/assets/images/logo.png
+-rw-r--r--   0        0        0    70935 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/docs/assets/images/pyodmongo_Logo_BG_Dark.png
+-rw-r--r--   0        0        0    72399 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/docs/assets/images/pyodmongo_Logo_BG_White.png
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/docs/en/aggregation.md
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/docs/en/contributing.md
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/docs/en/db_model.md
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/docs/en/delete.md
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/docs/en/fastapi.md
+-rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/docs/en/find.md
+-rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/docs/en/getting_started.md
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/docs/en/index.md
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/docs/en/indexes.md
+-rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/docs/en/query.md
+-rw-r--r--   0        0        0     4849 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/docs/en/save.md
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/docs/pt-BR/aggregation.md
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/docs/pt-BR/contributing.md
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/docs/pt-BR/db_model.md
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/docs/pt-BR/delete.md
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/docs/pt-BR/fastapi.md
+-rw-r--r--   0        0        0     7543 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/docs/pt-BR/find.md
+-rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/docs/pt-BR/getting_started.md
+-rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/docs/pt-BR/index.md
+-rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/docs/pt-BR/indexes.md
+-rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/docs/pt-BR/query.md
+-rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/docs/pt-BR/save.md
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/docs/stylesheets/extras.css
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/pyodmongo/__init__.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/pyodmongo/version.py
+-rw-r--r--   0        0        0    16482 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/pyodmongo/async_engine/engine.py
+-rw-r--r--   0        0        0    18222 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/pyodmongo/engine/engine.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/pyodmongo/engine/utils.py
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/pyodmongo/models/db_field_info.py
+-rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/pyodmongo/models/db_model.py
+-rw-r--r--   0        0        0     9486 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/pyodmongo/models/fields.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/pyodmongo/models/id_model.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/pyodmongo/models/paginate.py
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/pyodmongo/models/query_operators.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/pyodmongo/models/responses.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/pyodmongo/models/sort_operators.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/pyodmongo/queries/__init__.py
+-rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/pyodmongo/queries/comparison_operators.py
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/pyodmongo/queries/logical_operators.py
+-rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/pyodmongo/queries/query_string.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/pyodmongo/queries/sort_operator.py
+-rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/pyodmongo/services/aggregate_stages.py
+-rw-r--r--   0        0        0     9853 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/pyodmongo/services/model_init.py
+-rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/pyodmongo/services/query_operators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/tests/conftest.py
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/tests/test_async_aggregate.py
+-rw-r--r--   0        0        0    18765 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/tests/test_async_crud_db.py
+-rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/tests/test_class.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/tests/test_db_field_info.py
+-rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/tests/test_db_index.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/tests/test_dict_empty.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/tests/test_fastapi.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/tests/test_model_init_functions.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/tests/test_object_id.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/tests/test_project_pipeline.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/tests/test_pydantic_validators.py
+-rw-r--r--   0        0        0    12859 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/tests/test_queries.py
+-rw-r--r--   0        0        0     9193 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/tests/test_reference_pipeline.py
+-rw-r--r--   0        0        0     8320 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/tests/test_save_dict.py
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/tests/test_sync_aggregate.py
+-rw-r--r--   0        0        0    12850 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/tests/test_sync_crud_db.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/tests/test_version.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/LICENSE
+-rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/README.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 pyodmongo-0.8.0/PKG-INFO
```

### Comparing `pyodmongo-0.7.3/code_of_conduct.md` & `pyodmongo-0.8.0/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/mkdocs.yml` & `pyodmongo-0.8.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/pyproject.py` & `pyodmongo-0.8.0/pyproject.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/requirements.txt` & `pyodmongo-0.8.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/.github/ISSUE_TEMPLATE/bug.yml` & `pyodmongo-0.8.0/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/.github/workflows/black_formatter.yml` & `pyodmongo-0.8.0/.github/workflows/black_formatter.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/.github/workflows/publishing_docs_s3.yml` & `pyodmongo-0.8.0/.github/workflows/publishing_docs_s3.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/.github/workflows/python_publish.yml` & `pyodmongo-0.8.0/.github/workflows/python_publish.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/.github/workflows/tests.yml` & `pyodmongo-0.8.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/docs/assets/images/favicon.png` & `pyodmongo-0.8.0/docs/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/docs/assets/images/insomnia_request.png` & `pyodmongo-0.8.0/docs/assets/images/insomnia_request.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/docs/assets/images/logo.png` & `pyodmongo-0.8.0/docs/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/docs/assets/images/pyodmongo_Logo_BG_Dark.png` & `pyodmongo-0.8.0/docs/assets/images/pyodmongo_Logo_BG_Dark.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/docs/assets/images/pyodmongo_Logo_BG_White.png` & `pyodmongo-0.8.0/docs/assets/images/pyodmongo_Logo_BG_White.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/docs/en/aggregation.md` & `pyodmongo-0.8.0/docs/en/aggregation.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/docs/en/contributing.md` & `pyodmongo-0.8.0/docs/en/contributing.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/docs/en/db_model.md` & `pyodmongo-0.8.0/docs/en/db_model.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/docs/en/delete.md` & `pyodmongo-0.8.0/docs/en/delete.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/docs/en/fastapi.md` & `pyodmongo-0.8.0/docs/en/fastapi.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/docs/en/find.md` & `pyodmongo-0.8.0/docs/en/find.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/docs/en/getting_started.md` & `pyodmongo-0.8.0/docs/en/getting_started.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/docs/en/index.md` & `pyodmongo-0.8.0/docs/en/index.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/docs/en/indexes.md` & `pyodmongo-0.8.0/docs/en/indexes.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/docs/en/query.md` & `pyodmongo-0.8.0/docs/en/query.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 Creating queries in **PyODMongo** is straightforward and intuitive. It simplifies the process of building MongoDB queries, providing a Pythonic and straightforward approach to working with **Comparison Operators** and **Logical Operators** found in MongoDB.
 
 In **PyODMongo**, a query serves as an essential attribute of the `find_many` and `find_one` methods, which are available through the `DbEngine` and `AsyncDbEngine` classes. These methods empower you to retrieve data from your MongoDB database with ease, combining the simplicity of Python with the robust querying capabilities of MongoDB.
 
 ## Comparison Operators
 
-| Operator | Description                          |
-| ---------| ------------------------------------ |
-| `eq`     | Matches values that are equal to a specified value.  |
-| `gt`     | Matches values that are greater than a specified value. |
-| `gte`    | Matches values that are greater than or equal to a specified value. |
-| `in_`    | Matches any of the values specified in an list. |
-| `lt`     | Matches values that are less than a specified value. |
-| `lte`    | Matches values that are less than or equal to a specified value. |
-| `ne`     | Matches all values that are not equal to a specified value. |
-| `nin`    | Matches none of the values specified in an list. |
+| Operator | Usage |
+| ---------|--- |
+| **EQ**  | `eq(Model.attr, value)`</br>`Model.attr == value` |
+| **GT**   | `gt(Model.attr, value)`</br>`Model.attr > value` |
+| **GTE** | `gte(Model.attr, value)`</br>`Model.attr >= value` |
+| **IN**        | `in_(Model.attr, value)` |
+| **LT**   | `lt(Model.attr, value)`</br>`Model.attr < value` |
+| **LTE** | `lte(Model.attr, value)`</br>`Model.attr <= value` |
+| **NE**  | `ne(Model.attr, value)`</br>`Model.attr != value` |
+| **NIN**            | `nin(Model.attr, value)` |
 
 
 When using these Comparison Operators in PyODMongo, you'll typically provide two arguments:
 
 - `field: DbField`: This argument represents the field of your PyODMongo `DbModel` class that you want to search in the database. It defines the property you want to apply the comparison operator to.
 
 - `value: Any`: This argument specifies the value you want to compare against the field defined in the first argument. It represents the reference value to be found in the database.
@@ -41,15 +41,16 @@
     name: str
     price: float
     is_available: bool
     _collection: ClassVar = 'products'
 
 
 async def main():
-    query = gte(Product.price, 5)
+    query =  Product.price >= 5
+    #query = gte(Product.price, 5)
     sort_oprator = sort((Product.name, 1), (Product.price, -1))
     result: Product = await engine.find_one(Model=Product, query=query, sort=sort_oprator)
 
 asyncio.run(main())
 ```
 ///
 /// tab | Sync
@@ -65,33 +66,34 @@
 class Product(DbModel):
     name: str
     price: float
     is_available: bool
     _collection: ClassVar = 'products'
 
 
-query = gte(Product.price, 5)
+query = Product.price >= 5
+#query = gte(Product.price, 5)
 sort_oprator = sort((Product.name, 1), (Product.price, -1))
 result: Product = engine.find_one(Model=Product, query=query, sort=sort_oprator)
 ```
 ///
 
 In this example, the query will return all documents  in 'products' collection where the 'price' field is equal to or greater than 5.
 
 ## Logical Operators
 
 Just like Comparison Operators, Logical Operators in **PyODMongo** are designed to mirror their counterparts in MongoDB itself.
 
 Here are the primary Logical Operators available in PyODMongo:
 
-| Operator | Description                          |
-| ---------| ------------------------------------ |
-| `and_` | Join query clauses with a logical **AND**. Returns all documents that match the conditions of all clauses. |
-| `or_` | Join query clauses with a logical **OR**. Returns all documents that match the conditions of any of the clauses. |
-| `nor` | Join query clauses with a logical **NOR**. Returns the inverse of **OR** |
+| Operator | Usage |
+| ---------|-|
+| **AND**| `and_(gt(Model.attr_1, value_1), lt(Model.attr_1, value_2))`</br>`(Model.attr_1 > value_1) & (Model.attr_1 < value_2)` |
+| **OR** | `or_(eq(Model.attr_1, value_1), eq(Model.attr_1, value_2))`</br>`(Model.attr_1 == value_1) | (Model.attr_1 == value_2)` |
+| **NOR** | `nor(Model.attr_1 == value_1, Model.attr_1 == value_2)` |
 
 
 Here's an example of how you can use Logical Operators in PyODMongo:
 
 /// tab | Async
 ```python hl_lines="18"
 from pyodmongo import AsyncDbEngine, DbModel
@@ -107,18 +109,19 @@
     name: str
     price: float
     is_available: bool
     _collection: ClassVar = 'products'
 
 
 async def main():
-    query = and_(
-        eq(Product.is_available, True),
-        gte(Product.price, 5)
-    )
+    query = (Product.is_available == True) & (Product.price >= 5)
+    # query = and_(
+    #     eq(Product.is_available, True),
+    #     gte(Product.price, 5)
+    # )
     sort_oprator = sort((Product.name, 1), (Product.price, -1))
     result: Product = await engine.find_one(Model=Product, query=query, sort=sort_oprator)
 
 asyncio.run(main())
 ```
 ///
 /// tab | Sync
@@ -135,18 +138,19 @@
 class Product(DbModel):
     name: str
     price: float
     is_available: bool
     _collection: ClassVar = 'products'
 
 
-query = and_(
-    eq(Product.is_available, True),
-    gte(Product.price, 5)
-)
+query = (Product.is_available == True) & (Product.price >= 5)
+# query = and_(
+#     eq(Product.is_available, True),
+#     gte(Product.price, 5)
+# )
 sort_oprator = sort((Product.name, 1), (Product.price, -1))
 result: Product = engine.find_one(Model=Product, query=query, sort=sort_oprator)
 
 ```
 ///
 
 In this example, the query returns all documents from the 'products' collection that `is_available` is `True` and that have `price` greater than or equal to 5
@@ -171,15 +175,15 @@
     name: str
     price: float
     is_available: bool
     _collection: ClassVar = 'products'
 
 
 async def main():
-    query = gte(Product.price, 5)
+    query = Product.price >= 5
     sort_oprator = sort((Product.name, 1), (Product.price, -1))
     result: Product = await engine.find_one(Model=Product, query=query, sort=sort_oprator)
 
 asyncio.run(main())
 ```
 ///
 /// tab | Sync
@@ -195,14 +199,14 @@
 class Product(DbModel):
     name: str
     price: float
     is_available: bool
     _collection: ClassVar = 'products'
 
 
-query = gte(Product.price, 5)
+query = Product.price >= 5
 sort_oprator = sort((Product.name, 1), (Product.price, -1))
 result: Product = engine.find_one(Model=Product, query=query, sort=sort_oprator)
 ```
 ///
 
 In the provided example, the `sort_operator` is defined using the `sort` function, which takes tuples. Each tuple contains two elements: the first one is the field by which you want to sort, and the second one is the sorting direction, where 1 indicates ascending order and -1 indicates descending order. In the presented case, the `sort_operator` sorts the results first by the name field in ascending order and then by the price field in descending order. Thus, the products are returned in alphabetical order by name and, in case of a tie, in descending order by price.
```

### Comparing `pyodmongo-0.7.3/docs/en/save.md` & `pyodmongo-0.8.0/docs/en/save.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/docs/pt-BR/aggregation.md` & `pyodmongo-0.8.0/docs/pt-BR/aggregation.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/docs/pt-BR/contributing.md` & `pyodmongo-0.8.0/docs/pt-BR/contributing.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/docs/pt-BR/db_model.md` & `pyodmongo-0.8.0/docs/pt-BR/db_model.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/docs/pt-BR/delete.md` & `pyodmongo-0.8.0/docs/pt-BR/delete.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/docs/pt-BR/fastapi.md` & `pyodmongo-0.8.0/docs/pt-BR/fastapi.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/docs/pt-BR/find.md` & `pyodmongo-0.8.0/docs/pt-BR/find.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/docs/pt-BR/getting_started.md` & `pyodmongo-0.8.0/docs/pt-BR/getting_started.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/docs/pt-BR/index.md` & `pyodmongo-0.8.0/docs/pt-BR/index.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/docs/pt-BR/indexes.md` & `pyodmongo-0.8.0/docs/pt-BR/indexes.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/docs/pt-BR/query.md` & `pyodmongo-0.8.0/docs/pt-BR/query.md`

 * *Files 21% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 Criar consultas no **PyODMongo** é simples e intuitivo. Ele simplifica o processo de criação de consultas do MongoDB, fornecendo uma abordagem Pythônica e direta para trabalhar com **Operadores de comparação** e **Operadores lógicos** encontrados no MongoDB.
 
 No **PyODMongo**, uma consulta serve como um atributo essencial dos métodos `find_many` e `find_one`, que estão disponíveis através das classes `DbEngine` e `AsyncDbEngine`. Esses métodos permitem recuperar dados do seu banco de dados MongoDB com facilidade, combinando a simplicidade do Python com os recursos robustos de consulta do MongoDB.
 
 ## Operadores de comparação
 
-| Operador | Descrição |
-| ---------| ------------------------------------ |
-| `eq` | Corresponde a valores iguais a um valor especificado. |
-| `gt` | Corresponde a valores maiores que um valor especificado. |
-| `gte` | Corresponde a valores maiores ou iguais a um valor especificado. |
-| `in_` | Corresponde a qualquer um dos valores especificados em uma lista. |
-| `lt` | Corresponde a valores menores que um valor especificado. |
-| `lte` | Corresponde a valores menores ou iguais a um valor especificado. |
-| `ne` | Corresponde a todos os valores que não são iguais a um valor especificado. |
-| `nin` | Corresponde a qualquer valor que não esteja na lista. |
+| Operador | Uso |
+| ---------|--- |
+| **EQ**  | `eq(Model.attr, value)`</br>`Model.attr == value` |
+| **GT**   | `gt(Model.attr, value)`</br>`Model.attr > value` |
+| **GTE** | `gte(Model.attr, value)`</br>`Model.attr >= value` |
+| **IN**        | `in_(Model.attr, value)` |
+| **LT**   | `lt(Model.attr, value)`</br>`Model.attr < value` |
+| **LTE** | `lte(Model.attr, value)`</br>`Model.attr <= value` |
+| **NE**  | `ne(Model.attr, value)`</br>`Model.attr != value` |
+| **NIN**            | `nin(Model.attr, value)` |
 
 
 Ao usar esses operadores de comparação no PyODMongo, você normalmente fornecerá dois argumentos:
 
 - `field: DbField`: Este argumento representa o campo da sua classe `DbModel` do PyODMongo que você deseja pesquisar no banco de dados. Ele define a propriedade à qual você deseja aplicar o operador de comparação.
 
 - `value: Any`: Este argumento especifica o valor que você deseja comparar com o campo definido no primeiro argumento. Representa o valor de referência a ser encontrado no banco de dados.
@@ -41,15 +41,16 @@
     name: str
     price: float
     is_available: bool
     _collection: ClassVar = 'products'
 
 
 async def main():
-    query = gte(Product.price, 5)
+    query =  Product.price >= 5
+    #query = gte(Product.price, 5)
     sort_oprator = sort((Product.name, 1), (Product.price, -1))
     result: Product = await engine.find_one(Model=Product, query=query, sort=sort_oprator)
 
 asyncio.run(main())
 ```
 ///
 /// tab | Sync
@@ -65,33 +66,34 @@
 class Product(DbModel):
     name: str
     price: float
     is_available: bool
     _collection: ClassVar = 'products'
 
 
-query = gte(Product.price, 5)
+query =  Product.price >= 5
+#query = gte(Product.price, 5)
 sort_oprator = sort((Product.name, 1), (Product.price, -1))
 result: Product = engine.find_one(Model=Product, query=query, sort=sort_oprator)
 ```
 ///
 
 Neste exemplo, a consulta retornará todos os documentos da collection 'products' onde o campo price for igual ou superior a 5.
 
 ## Operadores lógicos
 
 Assim como os operadores de comparação, os operadores lógicos no **PyODMongo** são projetados para espelhar seus equivalentes no próprio MongoDB.
 
 Aqui estão os principais operadores lógicos disponíveis no PyODMongo:
 
-| Operador | Descrição |
-| ---------| ------------------------------------ |
-| `and_` | Unir cláusulas de consulta com um **AND** lógico. Retorna todos os documentos que correspondem às condições de todas as cláusulas. |
-| `or_` | Unir cláusulas de consulta com um **OR** lógico. Retorna todos os documentos que correspondem às condições de qualquer uma das cláusulas. |
-| `nor` | Unir cláusulas de consulta com um **NOR** lógico. Retorna o inverso do **OR** |
+| Operador | Uso |
+| ---------|-|
+| **AND**| `and_(gt(Model.attr_1, value_1), lt(Model.attr_1, value_2))`</br>`(Model.attr_1 > value_1) & (Model.attr_1 < value_2)` |
+| **OR** | `or_(eq(Model.attr_1, value_1), eq(Model.attr_1, value_2))`</br>`(Model.attr_1 == value_1) | (Model.attr_1 == value_2)` |
+| **NOR** | `nor(Model.attr_1 == value_1, Model.attr_1 == value_2)` |
 
 
 Aqui está um exemplo de como você pode usar operadores lógicos no PyODMongo:
 
 /// tab | Async
 ```python hl_lines="18"
 from pyodmongo import AsyncDbEngine, DbModel
@@ -107,18 +109,19 @@
     name: str
     price: float
     is_available: bool
     _collection: ClassVar = 'products'
 
 
 async def main():
-    query = and_(
-        eq(Product.is_available, True),
-        gte(Product.price, 5)
-    )
+    query = (Product.is_available == True) & (Product.price >= 5)
+    # query = and_(
+    #     eq(Product.is_available, True),
+    #     gte(Product.price, 5)
+    # )
     sort_oprator = sort((Product.name, 1), (Product.price, -1))
     result: Product = await engine.find_one(Model=Product, query=query, sort=sort_oprator)
 
 asyncio.run(main())
 ```
 ///
 /// tab | Sync
@@ -135,18 +138,19 @@
 class Product(DbModel):
     name: str
     price: float
     is_available: bool
     _collection: ClassVar = 'products'
 
 
-query = and_(
-    eq(Product.is_available, True),
-    gte(Product.price, 5)
-)
+query = (Product.is_available == True) & (Product.price >= 5)
+# query = and_(
+#     eq(Product.is_available, True),
+#     gte(Product.price, 5)
+# )
 sort_oprator = sort((Product.name, 1), (Product.price, -1))
 result: Product = engine.find_one(Model=Product, query=query, sort=sort_oprator)
 
 ```
 ///
 
 Neste exemplo a consulta retornará todos os documentos da collecion 'products' que `is_available` seja `True` e que tenham `price` maior ou igual a 5
@@ -171,15 +175,15 @@
     name: str
     price: float
     is_available: bool
     _collection: ClassVar = 'products'
 
 
 async def main():
-    query = gte(Product.price, 5)
+    query = Product.price >= 5
     sort_oprator = sort((Product.name, 1), (Product.price, -1))
     result: Product = await engine.find_one(Model=Product, query=query, sort=sort_oprator)
 
 asyncio.run(main())
 ```
 ///
 /// tab | Sync
@@ -195,14 +199,14 @@
 class Product(DbModel):
     name: str
     price: float
     is_available: bool
     _collection: ClassVar = 'products'
 
 
-query = gte(Product.price, 5)
+query = Product.price >= 5
 sort_oprator = sort((Product.name, 1), (Product.price, -1))
 result: Product = engine.find_one(Model=Product, query=query, sort=sort_oprator)
 ```
 ///
 
 No exemplo fornecido, o `sort_operator` é definido usando a função `sort`, que aceita tuplas. Cada tupla contém dois elementos: o primeiro é o campo pelo qual você deseja ordenar e o segundo é a direção da ordenação, onde 1 indica ordem ascendente e -1 indica ordem descendente. No caso apresentado, o `sort_operator` ordena os resultados primeiro pelo campo name em ordem ascendente e, em seguida, pelo campo price em ordem descendente. Assim, os produtos são retornados em ordem alfabética pelo nome e, em caso de empate, em ordem decrescente pelo preço.
```

### Comparing `pyodmongo-0.7.3/docs/pt-BR/save.md` & `pyodmongo-0.8.0/docs/pt-BR/save.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/pyodmongo/models/fields.py` & `pyodmongo-0.8.0/pyodmongo/models/fields.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/tests/test_async_aggregate.py` & `pyodmongo-0.8.0/tests/test_async_aggregate.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/tests/test_async_crud_db.py` & `pyodmongo-0.8.0/tests/test_async_crud_db.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 
 @pytest.mark.asyncio
 async def test_create_and_delete_one(drop_collection, new_obj):
     result: SaveResponse = await db.save(new_obj)
     assert result.upserted_id is not None
     id = result.upserted_id
-    query = eq(MyClass.id, id)
+    query = MyClass.id == id
     result: DeleteResponse = await db.delete_one(Model=MyClass, query=query)
     assert result.deleted_count == 1
 
 
 @pytest.mark.asyncio
 async def test_find_one(drop_collection, new_obj):
     result: SaveResponse = await db.save(new_obj)
@@ -118,16 +118,16 @@
     await db.save_all(objs)
     response: DeleteResponse = await db.delete(MyClass, eq(MyClass.attr1, "attr_1"))
     assert response.deleted_count == 3
 
 
 @pytest.mark.asyncio
 async def test_find_many_without_paginate(drop_collection, create_100_docs_in_db):
-    obj_list_50 = await db.find_many(Model=MyClass, query=gt(MyClass.random_number, 50))
-    obj_list_100 = await db.find_many(Model=MyClass, query=gt(MyClass.random_number, 0))
+    obj_list_50 = await db.find_many(Model=MyClass, query=MyClass.random_number > 50)
+    obj_list_100 = await db.find_many(Model=MyClass, query=MyClass.random_number > 0)
     assert len(obj_list_50) == 50
     assert len(obj_list_100) == 100
     assert all(isinstance(obj, MyClass) for obj in obj_list_100)
 
 
 @pytest.mark.asyncio
 async def test_find_many_with_paginate(drop_collection, create_100_docs_in_db):
@@ -215,15 +215,15 @@
     await db._db[MyClass._collection].drop()
 
 
 @pytest.mark.asyncio
 async def test_find_many_with_zero_results(drop_collection):
     await db.save(obj=drop_collection)
     result = await db.find_many(
-        Model=MyClass, query=eq(MyClass.attr1, "value_that_not_exists"), paginate=True
+        Model=MyClass, query=MyClass.attr1 == "value_that_not_exists", paginate=True
     )
 
     assert result.page_quantity == 0
     assert result.docs_quantity == 0
     assert result.docs == []
 
 
@@ -582,7 +582,20 @@
     result_many = await db.find_many(Model=MySortClass, sort=sort_oprator)
     assert result_many[0] == obj_list[4]
     assert result_many[1] == obj_list[1]
 
     sort_oprator = sort((MySortClass.attr_3, 1))
     result_one = await db.find_one(Model=MySortClass, sort=sort_oprator)
     assert result_one == obj_list[2]
+
+    sort_oprator = ["attr_3", 1]
+    with pytest.raises(
+        TypeError,
+        match='sort argument must be a SortOperator from pyodmongo.queries. If you really need to make a very specific sort, use "raw_sort" argument',
+    ):
+        result_one = await db.find_one(Model=MySortClass, sort=sort_oprator)
+
+    with pytest.raises(
+        TypeError,
+        match='sort argument must be a SortOperator from pyodmongo.queries. If you really need to make a very specific sort, use "raw_sort" argument',
+    ):
+        result_many = await db.find_many(Model=MySortClass, sort=sort_oprator)
```

### Comparing `pyodmongo-0.7.3/tests/test_class.py` & `pyodmongo-0.8.0/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/tests/test_db_field_info.py` & `pyodmongo-0.8.0/tests/test_db_field_info.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/tests/test_db_index.py` & `pyodmongo-0.8.0/tests/test_db_index.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/tests/test_dict_empty.py` & `pyodmongo-0.8.0/tests/test_dict_empty.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,22 +9,21 @@
     class MyModel2(DbModel):
         attr2: str
         my_model_1: MyModel1 | Id
         _collection = "my_model_2"
 
     class MyModel3(DbModel):
         attr3: str
-        my_model_2: MyModel2 | Id
+        my_model_2: MyModel2 | Id | None
+        my_model_2_2: MyModel2 | Id | None
         _collection = "my_model_3"
 
-    dct = {
-        "attr3": "attr3",
-        "my_model_2": {},
-    }
+    dct = {"attr3": "attr3", "my_model_2": {}, "my_model_2_2": {"my_model_1": {}}}
     obj = MyModel3(**dct)
     assert obj.model_dump() == {
         "attr3": "attr3",
         "my_model_2": None,
+        "my_model_2_2": None,
         "id": None,
         "created_at": None,
         "updated_at": None,
     }
```

### Comparing `pyodmongo-0.7.3/tests/test_fastapi.py` & `pyodmongo-0.8.0/tests/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/tests/test_model_init_functions.py` & `pyodmongo-0.8.0/tests/test_model_init_functions.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/tests/test_object_id.py` & `pyodmongo-0.8.0/tests/test_object_id.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/tests/test_project_pipeline.py` & `pyodmongo-0.8.0/tests/test_project_pipeline.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/tests/test_pydantic_validators.py` & `pyodmongo-0.8.0/tests/test_pydantic_validators.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/tests/test_queries.py` & `pyodmongo-0.8.0/tests/test_queries.py`

 * *Files 20% similar despite different names*

```diff
@@ -221,26 +221,48 @@
 def test_mount_query_filter_with_regex():
     import re
 
     class MyModel(DbModel):
         attr1: str
         attr2: str
 
-    input_dict = {"attr1_in": "['/^agr[oóôõ]s/i', 123, 'abc']", "attr2_eq": "123"}
-
-    query, _ = mount_query_filter(
-        Model=MyModel, items=input_dict, initial_comparison_operators=[]
-    )
-    query_dct = query_dict(query_operator=query, dct={})
-    assert query_dct == {
+    input_dict_1 = {"attr1_in": "['/^agr[oóôõ]s/i', 123, 'abc']", "attr2_eq": "123"}
+    input_dict_2 = {"attr1_in": "['/^agr[oóôõ]s/m', 123, 'abc']", "attr2_eq": "123"}
+    input_dict_3 = {"attr1_in": "['/^agr[oóôõ]s/s', 123, 'abc']", "attr2_eq": "123"}
+
+    query_1, _ = mount_query_filter(
+        Model=MyModel, items=input_dict_1, initial_comparison_operators=[]
+    )
+    query_2, _ = mount_query_filter(
+        Model=MyModel, items=input_dict_2, initial_comparison_operators=[]
+    )
+    query_3, _ = mount_query_filter(
+        Model=MyModel, items=input_dict_3, initial_comparison_operators=[]
+    )
+    query_dct_1 = query_dict(query_operator=query_1, dct={})
+    query_dct_2 = query_dict(query_operator=query_2, dct={})
+    query_dct_3 = query_dict(query_operator=query_3, dct={})
+    assert query_dct_1 == {
         "$and": [
             {"attr1": {"$in": [re.compile("^agr[oóôõ]s", re.IGNORECASE), 123, "abc"]}},
             {"attr2": {"$eq": 123}},
         ]
     }
+    assert query_dct_2 == {
+        "$and": [
+            {"attr1": {"$in": [re.compile("^agr[oóôõ]s", re.MULTILINE), 123, "abc"]}},
+            {"attr2": {"$eq": 123}},
+        ]
+    }
+    assert query_dct_3 == {
+        "$and": [
+            {"attr1": {"$in": [re.compile("^agr[oóôõ]s", re.DOTALL), 123, "abc"]}},
+            {"attr2": {"$eq": 123}},
+        ]
+    }
 
 
 def test_mount_query_filter_with_data_types():
     class MyClass(DbModel):
         string_value: str
         int_value: int
         float_value: float
@@ -340,7 +362,69 @@
 
     assert query == and_(
         eq(MyClass.attr_1, "attr 1"),
         in_(MyClass.attr_2, ["value_1", "value_2"]),
         gte(MyClass.attr_3, 10),
     )
     assert sort_operator == sort((MyClass.attr_1, 1), (MyClass.attr_2, -1))
+
+
+def test_query_with_magic_methods():
+    class MyRefClass(DbModel):
+        attr_ref: str
+        _collection: ClassVar = "my_ref_class"
+
+    class MyMagicClass(DbModel):
+        attr_1: int
+        attr_2: int
+        attr_3: list[MyRefClass | Id]
+        _collection: ClassVar = "my_magic_class"
+
+    query_eq_magic_list = MyMagicClass.attr_3 == [
+        "628b7e33e36332a5dc17a0f7",
+        "628b7e5de36332a5dc17a119",
+    ]
+    query_eq_list = eq(
+        MyMagicClass.attr_3, ["628b7e33e36332a5dc17a0f7", "628b7e5de36332a5dc17a119"]
+    )
+
+    query_lt_magic = MyMagicClass.attr_1 < 123
+    query_lt = lt(MyMagicClass.attr_1, 123)
+    assert query_lt_magic == query_lt
+
+    query_lte_magic = MyMagicClass.attr_1 <= 123
+    query_lte = lte(MyMagicClass.attr_1, 123)
+    assert query_lte_magic == query_lte
+
+    query_eq_magic = MyMagicClass.attr_1 == 123
+    query_eq = eq(MyMagicClass.attr_1, 123)
+    assert query_eq_magic == query_eq
+
+    query_ne_magic = MyMagicClass.attr_1 != 123
+    query_ne = ne(MyMagicClass.attr_1, 123)
+    assert query_ne_magic == query_ne
+
+    query_gt_magic = MyMagicClass.attr_1 > 123
+    query_gt = gt(MyMagicClass.attr_1, 123)
+    assert query_gt_magic == query_gt
+
+    query_gte_magic = MyMagicClass.attr_1 >= 123
+    query_gte = gte(MyMagicClass.attr_1, 123)
+    assert query_gte_magic == query_gte
+
+    query_and_magic = ((MyMagicClass.attr_1 >= 100) | (MyMagicClass.attr_1 <= 200)) & (
+        MyMagicClass.attr_2 > 10
+    )
+    query_and = and_(
+        or_(gte(MyMagicClass.attr_1, 100), lte(MyMagicClass.attr_1, 200)),
+        gt(MyMagicClass.attr_2, 10),
+    )
+    assert query_and_magic == query_and
+
+    query_or_magic = (MyMagicClass.attr_1 == 100) & (MyMagicClass.attr_2 == 200) | (
+        MyMagicClass.attr_1 > 10
+    )
+    query_or = or_(
+        and_(eq(MyMagicClass.attr_1, 100), eq(MyMagicClass.attr_2, 200)),
+        gt(MyMagicClass.attr_1, 10),
+    )
+    assert query_or_magic == query_or
```

### Comparing `pyodmongo-0.7.3/tests/test_reference_pipeline.py` & `pyodmongo-0.8.0/tests/test_reference_pipeline.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/tests/test_save_dict.py` & `pyodmongo-0.8.0/tests/test_save_dict.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/tests/test_sync_aggregate.py` & `pyodmongo-0.8.0/tests/test_sync_aggregate.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/tests/test_sync_crud_db.py` & `pyodmongo-0.8.0/tests/test_sync_crud_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -391,7 +391,20 @@
     result_many = db.find_many(Model=MySortClass, sort=sort_oprator)
     assert result_many[0] == obj_list[4]
     assert result_many[1] == obj_list[1]
 
     sort_oprator = sort((MySortClass.attr_3, 1))
     result_one = db.find_one(Model=MySortClass, sort=sort_oprator)
     assert result_one == obj_list[2]
+
+    sort_oprator = ["attr_3", 1]
+    with pytest.raises(
+        TypeError,
+        match='sort argument must be a SortOperator from pyodmongo.queries. If you really need to make a very specific sort, use "raw_sort" argument',
+    ):
+        result_one = db.find_one(Model=MySortClass, sort=sort_oprator)
+
+    with pytest.raises(
+        TypeError,
+        match='sort argument must be a SortOperator from pyodmongo.queries. If you really need to make a very specific sort, use "raw_sort" argument',
+    ):
+        result_many = db.find_many(Model=MySortClass, sort=sort_oprator)
```

### Comparing `pyodmongo-0.7.3/.gitignore` & `pyodmongo-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/LICENSE` & `pyodmongo-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/README.md` & `pyodmongo-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.3/pyproject.toml` & `pyodmongo-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyodmongo"
-version = "0.7.3"
+version = "0.8.0"
 license = "MIT"
 authors = [
   { name="Mauro André", email="eng.mauroandre@gmail.com" },
 ]
 description = "A syncrounous and asyncrounous Python ODM for MongoDB based on Pydantic"
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `pyodmongo-0.7.3/PKG-INFO` & `pyodmongo-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyodmongo
-Version: 0.7.3
+Version: 0.8.0
 Summary: A syncrounous and asyncrounous Python ODM for MongoDB based on Pydantic
 Project-URL: Homepage, https://github.com/mauro-andre/pyodmongo
 Project-URL: Documentation, https://pyodmongo.dev
 Author-email: Mauro André <eng.mauroandre@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

