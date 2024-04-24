# Comparing `tmp/django_pgbulk-2.3.1.tar.gz` & `tmp/django_pgbulk-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pgbulk-2.3.1.tar", max compression
+gzip compressed data, was "django_pgbulk-2.4.0.tar", max compression
```

## Comparing `django_pgbulk-2.3.1.tar` & `django_pgbulk-2.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1456 2024-04-06 16:49:38.154177 django_pgbulk-2.3.1/LICENSE
--rw-r--r--   0        0        0     2051 2024-04-06 16:49:38.154177 django_pgbulk-2.3.1/README.md
--rw-r--r--   0        0        0      920 2024-04-06 16:49:38.154177 django_pgbulk-2.3.1/pgbulk/__init__.py
--rw-r--r--   0        0        0    23943 2024-04-06 16:49:38.154177 django_pgbulk-2.3.1/pgbulk/core.py
--rw-r--r--   0        0        0        0 2024-04-06 16:49:38.154177 django_pgbulk-2.3.1/pgbulk/py.typed
--rw-r--r--   0        0        0       80 2024-04-06 16:49:38.154177 django_pgbulk-2.3.1/pgbulk/version.py
--rw-r--r--   0        0        0     2198 2024-04-06 16:50:24.110373 django_pgbulk-2.3.1/pyproject.toml
--rw-r--r--   0        0        0     3258 1970-01-01 00:00:00.000000 django_pgbulk-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1456 2024-04-24 01:39:02.376995 django_pgbulk-2.4.0/LICENSE
+-rw-r--r--   0        0        0     2093 2024-04-24 01:39:02.376995 django_pgbulk-2.4.0/README.md
+-rw-r--r--   0        0        0      920 2024-04-24 01:39:02.376995 django_pgbulk-2.4.0/pgbulk/__init__.py
+-rw-r--r--   0        0        0    24376 2024-04-24 01:39:02.376995 django_pgbulk-2.4.0/pgbulk/core.py
+-rw-r--r--   0        0        0        0 2024-04-24 01:39:02.376995 django_pgbulk-2.4.0/pgbulk/py.typed
+-rw-r--r--   0        0        0       80 2024-04-24 01:39:02.376995 django_pgbulk-2.4.0/pgbulk/version.py
+-rw-r--r--   0        0        0     2518 2024-04-24 01:39:51.221379 django_pgbulk-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3300 1970-01-01 00:00:00.000000 django_pgbulk-2.4.0/PKG-INFO
```

### Comparing `django_pgbulk-2.3.1/LICENSE` & `django_pgbulk-2.4.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2023, Opus 10
+Copyright (c) 2024, Opus 10
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright
   notice, this list of conditions and the following disclaimer.
```

### Comparing `django_pgbulk-2.3.1/README.md` & `django_pgbulk-2.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -58,10 +58,15 @@
 
 After this, add `pgbulk` to the `INSTALLED_APPS` setting of your Django project.
 
 ## Contributing Guide
 
 For information on setting up django-pgbulk for development and contributing changes, view [CONTRIBUTING.md](CONTRIBUTING.md).
 
-## Primary Authors
+## Creators
 
 - [Wes Kendall](https://github.com/wesleykendall)
+
+## Other Contributors
+
+- @max-muoto
+- @dalberto
```

### Comparing `django_pgbulk-2.3.1/pgbulk/__init__.py` & `django_pgbulk-2.4.0/pgbulk/__init__.py`

 * *Files identical despite different names*

### Comparing `django_pgbulk-2.3.1/pgbulk/core.py` & `django_pgbulk-2.4.0/pgbulk/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,30 +16,30 @@
     try:
         import psycopg as Database  # type: ignore
     except ImportError:
         import psycopg2 as Database
     except Exception as exc:  # pragma: no cover
         raise ImproperlyConfigured("Error loading psycopg2 or psycopg module") from exc
 
-    version_tuple = get_version_tuple(Database.__version__.split(" ", 1)[0])
+    version_tuple = get_version_tuple(Database.__version__.split(" ", 1)[0])  # type: ignore
 
     if version_tuple[0] not in (2, 3):  # pragma: no cover
         raise ImproperlyConfigured(f"Pysocpg version {version_tuple[0]} not supported")
 
     return version_tuple
 
 
 psycopg_version = _psycopg_version()
 psycopg_maj_version = psycopg_version[0]
 
 
 if psycopg_maj_version == 2:
-    from psycopg2.extensions import AsIs as Literal
+    from psycopg2.extensions import AsIs as Literal  # type: ignore
 elif psycopg_maj_version == 3:
-    import psycopg.adapt
+    import psycopg.adapt  # type: ignore
 
     class Literal:  # pragma: no cover
         def __init__(self, val):
             self.val = val
 
     class LiteralDumper(psycopg.adapt.Dumper):  # pragma: no cover
         def dump(self, obj):
@@ -87,43 +87,43 @@
     Wraps a list of named tuples where the names correspond to the underlying
     Django model attribute names.
 
     Also provides properties to access created and updated rows.
     """
 
     @property
-    def created(self) -> List[namedtuple]:
+    def created(self) -> List[namedtuple]:  # type: ignore
         """Return the created rows"""
         return [i for i in self if i.status_ == "c"]
 
     @property
-    def updated(self) -> List[namedtuple]:
+    def updated(self) -> List[namedtuple]:  # type: ignore
         """Return the updated rows"""
         return [i for i in self if i.status_ == "u"]
 
 
 def _quote(field):
     return '"{0}"'.format(field)
 
 
 def _get_update_fields(queryset, to_update, exclude=None):
     """
     Get the fields to be updated in an upsert.
 
-    Always exclude auto_now_add and primary key fields
+    Always exclude auto_now_add, primary key, generated, and non-concrete fields
     """
     exclude = exclude or []
     model = queryset.model
     fields = {
-        **{field.attname: field for field in model._meta.fields},
-        **{field.name: field for field in model._meta.fields},
+        **{field.attname: field for field in _model_fields(model)},
+        **{field.name: field for field in _model_fields(model)},
     }
 
     if to_update is None:
-        to_update = [field.attname for field in model._meta.fields]
+        to_update = [field.attname for field in _model_fields(model)]
 
     to_update = [
         attname
         for attname in to_update
         if (
             attname not in exclude
             and not getattr(fields[attname], "auto_now_add", False)
@@ -139,15 +139,15 @@
     Given a list of models, fill in auto_now and auto_now_add fields
     for upserts. Since django manager utils passes Django's ORM, these values
     have to be automatically constructed
     """
     model = queryset.model
     auto_field_names = [
         f.attname
-        for f in model._meta.fields
+        for f in _model_fields(model)
         if getattr(f, "auto_now", False) or getattr(f, "auto_now_add", False)
     ]
     now = timezone.now()
     for value in values:
         for f in auto_field_names:
             setattr(value, f, now)
 
@@ -182,15 +182,15 @@
     Sort a list of models by their unique fields.
 
     Sorting models in an upsert greatly reduces the chances of deadlock
     when doing concurrent upserts
     """
     model = queryset.model
     connection = connections[queryset.db]
-    unique_fields = [field for field in model._meta.fields if field.attname in unique_fields]
+    unique_fields = [field for field in _model_fields(model) if field.attname in unique_fields]
 
     def sort_key(model_obj):
         return tuple(
             _get_field_db_val(queryset, field, getattr(model_obj, field.attname), connection)
             for field in unique_fields
         )
 
@@ -228,14 +228,19 @@
 
 def _get_return_fields_sql(returning):
     return_fields_sql = ", ".join(_quote(field) for field in returning)
     return_fields_sql += ", CASE WHEN xmax = 0 THEN 'c' ELSE 'u' END AS status_"
     return return_fields_sql
 
 
+def _model_fields(model: models.Model) -> List[models.Field]:
+    """Return the fields of a model, excluding generated and non-concrete ones."""
+    return [f for f in model._meta.fields if not getattr(f, "generated", False) and f.concrete]
+
+
 def _get_upsert_sql(
     queryset,
     model_objs,
     unique_fields,
     update_fields,
     returning,
     redundant_updates=False,
@@ -248,20 +253,20 @@
     """
     model = queryset.model
     update_expressions = {f: f.expression for f in update_fields if getattr(f, "expression", None)}
 
     # Use all fields except pk unless the uniqueness constraint is the pk field
     all_fields = [
         field
-        for field in model._meta.fields
+        for field in _model_fields(model)
         if field.column in unique_fields or not isinstance(field, models.AutoField)
     ]
 
     all_field_names = [field.column for field in all_fields]
-    returning = returning if returning is not True else [f.column for f in model._meta.fields]
+    returning = returning if returning is not True else [f.column for f in _model_fields(model)]
     all_field_names_sql = ", ".join([_quote(field) for field in all_field_names])
 
     # Convert field names to db column names
     unique_fields = [model._meta.get_field(unique_field) for unique_field in unique_fields]
     update_fields = [model._meta.get_field(update_field) for update_field in update_fields]
 
     row_values, sql_args = _get_values_for_rows(queryset, model_objs, all_fields)
@@ -345,15 +350,15 @@
             update_fields,
             returning,
             redundant_updates=redundant_updates,
         )
 
         with connection.cursor() as cursor:
             sql_args = _prep_sql_args(queryset, connection, cursor, sql_args)
-            cursor.execute(sql, sql_args)
+            cursor.execute(sql, sql_args)  # type: ignore
             if cursor.description:
                 nt_result = namedtuple("Result", [col[0] for col in cursor.description])
                 upserted = [nt_result(*row) for row in cursor.fetchall()]
 
     return UpsertResult(upserted)
 
 
@@ -388,15 +393,15 @@
             being updated. This is additive to the `unique_fields` list.
         returning: If True, returns all fields. If a list,
             only returns fields in the list.
         redundant_updates: Don't perform an update
             if all columns are identical to the row in the database.
     """
     exclude = exclude or []
-    queryset = queryset if isinstance(queryset, models.QuerySet) else queryset.objects.all()
+    queryset = queryset if isinstance(queryset, models.QuerySet) else queryset.objects.all()  # type: ignore
 
     # Populate automatically generated fields in the rows like date times
     _fill_auto_fields(queryset, model_objs)
 
     # Sort the rows to reduce the chances of deadlock during concurrent upserts
     model_objs = _sort_by_unique_fields(queryset, model_objs, unique_fields)
     update_fields = _get_update_fields(queryset, update_fields, exclude=[*exclude, *unique_fields])
@@ -444,15 +449,15 @@
                     MyModel(id=2, some_attr='some_val2')
                 ],
                 # These are the fields that will be updated. If not provided,
                 # all fields will be updated
                 ['some_attr']
             )
     """
-    queryset = queryset if isinstance(queryset, models.QuerySet) else queryset.objects.all()
+    queryset = queryset if isinstance(queryset, models.QuerySet) else queryset.objects.all()  # type: ignore
     connection = connections[queryset.db]
     model = queryset.model
     update_fields = _get_update_fields(queryset, update_fields, exclude)
 
     # Sort the model objects to reduce the likelihood of deadlocks
     model_objs = sorted(model_objs, key=lambda obj: obj.pk)
 
@@ -460,25 +465,25 @@
     value_fields = [model._meta.pk.attname] + update_fields
 
     row_values = [
         [
             _get_field_db_val(
                 queryset,
                 model_obj._meta.get_field(field),
-                getattr(model_obj, model_obj._meta.get_field(field).attname),
+                getattr(model_obj, model_obj._meta.get_field(field).attname),  # type: ignore
                 connection,
             )
             for field in value_fields
         ]
         for model_obj in model_objs
     ]
 
     # If we do not have any values or fields to update, just return
     if len(row_values) == 0 or len(update_fields) == 0:
-        return []
+        return
 
     db_types = [model._meta.get_field(field).db_type(connection) for field in value_fields]
 
     value_fields_sql = ", ".join(
         '"{field}"'.format(field=model._meta.get_field(field).column) for field in value_fields
     )
 
@@ -516,15 +521,15 @@
         value_fields_sql=value_fields_sql,
     )
 
     update_sql_params = list(itertools.chain(*row_values))
 
     with connection.cursor() as cursor:
         update_sql_params = _prep_sql_args(queryset, connection, cursor, update_sql_params)
-        return cursor.execute(update_sql, update_sql_params)
+        cursor.execute(update_sql, update_sql_params)  # type: ignore
 
 
 async def aupdate(
     queryset: Union[Type[models.Model], models.QuerySet],
     model_objs: Iterable[models.Model],
     update_fields: Union[List[str], None] = None,
     exclude: Union[List[str], None] = None,
```

### Comparing `django_pgbulk-2.3.1/pyproject.toml` & `django_pgbulk-2.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,94 +1,110 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.black]
-line-length = 99
-target-version = ['py38']
-
 [tool.coverage.run]
 branch = true
 source = ["pgbulk"]
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "raise AssertionError",
     "raise NotImplementedError",
     "pass",
-    "pytest.mark.skip"
+    "pytest.mark.skip",
+    "@(typing\\.)?overload",
+    "if TYPE_CHECKING:",
 ]
 show_missing = true
 fail_under = 100
 
 [tool.poetry]
 name = "django-pgbulk"
 packages = [
   { include = "pgbulk" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "2.3.1"
+version = "2.4.0"
 description = "Native postgres bulk update and upsert operations."
 authors = ["Wes Kendall"]
 classifiers = [
   "Framework :: Django",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
   "Framework :: Django :: 4.1",
   "Framework :: Django :: 4.2",
   "Framework :: Django :: 5.0",
+  
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: 3 :: Only",
   "Framework :: Django",
+  
 ]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/Opus10/django-pgbulk"
 repository = "https://github.com/Opus10/django-pgbulk"
 documentation = "https://django-pgbulk.readthedocs.io"
 
 [tool.poetry.dependencies]
 python = ">=3.8.0,<4"
 django = ">=3"
 
 [tool.poetry.dev-dependencies]
-black = "23.9.1"
-dj-database-url = "2.1.0"
 git-tidy = "1.2.0"
-psycopg2-binary = "2.9.9"
 pytest = "7.4.2"
 pytest-cov = "4.1.0"
 pytest-dotenv = "0.5.2"
-pytest-django = "4.5.2"
-django-dynamic-fixture = "4.0.1"
 tox = "4.11.3"
-ruff = "0.0.292"
+ruff = "0.3.7"
+pyright = "1.1.358"
 mkdocs = "1.5.3"
-mkdocs-material = "9.4.4"
-mkdocstrings-python = "1.7.2"
+black = "24.4.0"
+mkdocs-material = "9.5.18"
+mkdocstrings-python = "1.9.2"
 footing = "*"
 setuptools = "*"
 poetry-core = "*"
 django-timezone-field = "4.0"
 freezegun = "0.3.15"
+typing-extensions = "4.11.0"
+django-stubs = "4.2.7"
+dj-database-url = "2.1.0"
+psycopg2-binary = "2.9.9"
+pytest-django = "4.5.2"
+django-dynamic-fixture = "4.0.1"
+django-hashids = "0.7.0"
 
 [tool.pytest.ini_options]
 xfail_strict = true
-addopts = "--reuse-db"
 testpaths = "pgbulk/tests"
 norecursedirs = ".venv"
+addopts = "--reuse-db"
 DJANGO_SETTINGS_MODULE = "settings"
 
 [tool.ruff]
-select = ["E", "F", "B", "I", "G", "C4"]
+lint.select = ["E", "F", "B", "I", "G", "C4"]
 line-length = 99
 target-version = "py38"
+
+[tool.pyright]
+exclude = [
+    "**/node_modules",
+    "**/__pycache__",
+    "src/experimental",
+    "src/typestubs",
+    "**/migrations/**",
+    "**/tests/**",
+]
+pythonVersion = "3.8"
+typeCheckingMode = "standard"
```

### Comparing `django_pgbulk-2.3.1/PKG-INFO` & `django_pgbulk-2.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pgbulk
-Version: 2.3.1
+Version: 2.4.0
 Summary: Native postgres bulk update and upsert operations.
 Home-page: https://github.com/Opus10/django-pgbulk
 License: BSD-3-Clause
 Author: Wes Kendall
 Requires-Python: >=3.8.0,<4
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
@@ -17,16 +17,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: django (>=3)
 Project-URL: Documentation, https://django-pgbulk.readthedocs.io
 Project-URL: Repository, https://github.com/Opus10/django-pgbulk
 Description-Content-Type: text/markdown
 
 # django-pgbulk
 
@@ -88,11 +88,16 @@
 
 After this, add `pgbulk` to the `INSTALLED_APPS` setting of your Django project.
 
 ## Contributing Guide
 
 For information on setting up django-pgbulk for development and contributing changes, view [CONTRIBUTING.md](CONTRIBUTING.md).
 
-## Primary Authors
+## Creators
 
 - [Wes Kendall](https://github.com/wesleykendall)
 
+## Other Contributors
+
+- @max-muoto
+- @dalberto
+
```

