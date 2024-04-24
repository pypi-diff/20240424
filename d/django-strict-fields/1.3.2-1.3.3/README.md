# Comparing `tmp/django_strict_fields-1.3.2.tar.gz` & `tmp/django_strict_fields-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_strict_fields-1.3.2.tar", max compression
+gzip compressed data, was "django_strict_fields-1.3.3.tar", max compression
```

## Comparing `django_strict_fields-1.3.2.tar` & `django_strict_fields-1.3.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1456 2024-04-18 12:17:04.008830 django_strict_fields-1.3.2/LICENSE
--rw-r--r--   0        0        0      829 2024-04-18 12:17:04.008830 django_strict_fields-1.3.2/README.md
--rw-r--r--   0        0        0     2470 2024-04-18 12:17:57.705106 django_strict_fields-1.3.2/pyproject.toml
--rw-r--r--   0        0        0      442 2024-04-18 12:17:04.008830 django_strict_fields-1.3.2/strict_fields/__init__.py
--rw-r--r--   0        0        0     3032 2024-04-18 12:17:04.008830 django_strict_fields-1.3.2/strict_fields/apps.py
--rw-r--r--   0        0        0     2900 2024-04-18 12:17:04.008830 django_strict_fields-1.3.2/strict_fields/fields.py
--rw-r--r--   0        0        0      990 2024-04-18 12:17:04.008830 django_strict_fields-1.3.2/strict_fields/helpers.py
--rw-r--r--   0        0        0       87 2024-04-18 12:17:04.008830 django_strict_fields-1.3.2/strict_fields/version.py
--rw-r--r--   0        0        0     2097 1970-01-01 00:00:00.000000 django_strict_fields-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1456 2024-04-24 01:07:49.534858 django_strict_fields-1.3.3/LICENSE
+-rw-r--r--   0        0        0      828 2024-04-24 01:07:49.534858 django_strict_fields-1.3.3/README.md
+-rw-r--r--   0        0        0     2547 2024-04-24 01:08:38.826863 django_strict_fields-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0      442 2024-04-24 01:07:49.538858 django_strict_fields-1.3.3/strict_fields/__init__.py
+-rw-r--r--   0        0        0     3032 2024-04-24 01:07:49.538858 django_strict_fields-1.3.3/strict_fields/apps.py
+-rw-r--r--   0        0        0     2900 2024-04-24 01:07:49.538858 django_strict_fields-1.3.3/strict_fields/fields.py
+-rw-r--r--   0        0        0      990 2024-04-24 01:07:49.538858 django_strict_fields-1.3.3/strict_fields/helpers.py
+-rw-r--r--   0        0        0       87 2024-04-24 01:07:49.538858 django_strict_fields-1.3.3/strict_fields/version.py
+-rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 django_strict_fields-1.3.3/PKG-INFO
```

### Comparing `django_strict_fields-1.3.2/LICENSE` & `django_strict_fields-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_strict_fields-1.3.2/README.md` & `django_strict_fields-1.3.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 [View the django-strict-fields docs here](https://django-strict-fields.readthedocs.io/)
 
 ## Installation
 
 Install `django-strict-fields` with:
 
     pip3 install django-strict-fields
-
 After this, add `strict_fields` to the `INSTALLED_APPS` setting of your Django project.
 
 ## Contributing Guide
 
 For information on setting up django-strict-fields for development and contributing changes, view [CONTRIBUTING.md](CONTRIBUTING.md).
 
 ## Primary Authors
```

### Comparing `django_strict_fields-1.3.2/pyproject.toml` & `django_strict_fields-1.3.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -10,27 +10,28 @@
 exclude_lines = [
     "pragma: no cover",
     "raise AssertionError",
     "raise NotImplementedError",
     "pass",
     "pytest.mark.skip",
     "@(typing\\.)?overload",
+    "if TYPE_CHECKING:",
 ]
 show_missing = true
 fail_under = 100
 
 [tool.poetry]
 name = "django-strict-fields"
 packages = [
   { include = "strict_fields" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "1.3.2"
+version = "1.3.3"
 description = "A collection of fields and utilities to help make model fields more strict."
 authors = ["Tomas Arni Jonasson"]
 classifiers = [
   "Framework :: Django",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
   "Framework :: Django :: 4.1",
@@ -60,30 +61,31 @@
 django = ">=3"
 
 [tool.poetry.dev-dependencies]
 git-tidy = "1.2.0"
 pytest = "7.4.2"
 pytest-cov = "4.1.0"
 pytest-dotenv = "0.5.2"
-pytest-mock = "3.1.0"
+pytest-django = "4.5.2"
+pytest-mock = "3.14.0"
+django-dynamic-fixture = "4.0.1"
 tox = "4.11.3"
 ruff = "0.3.7"
 pyright = "1.1.358"
 mkdocs = "1.5.3"
 black = "24.4.0"
 mkdocs-material = "9.5.18"
 mkdocstrings-python = "1.9.2"
 footing = "*"
 setuptools = "*"
 poetry-core = "*"
 dj-database-url = "2.1.0"
 psycopg2-binary = "2.9.9"
-pytest-django = "4.5.2"
-django-dynamic-fixture = "4.0.1"
-
+typing-extensions = "4.11.0"
+django-stubs = "4.2.7"
 
 [tool.pytest.ini_options]
 xfail_strict = true
 testpaths = "strict_fields/tests"
 norecursedirs = ".venv"
 addopts = "--reuse-db"
 DJANGO_SETTINGS_MODULE = "settings"
```

### Comparing `django_strict_fields-1.3.2/strict_fields/apps.py` & `django_strict_fields-1.3.3/strict_fields/apps.py`

 * *Files identical despite different names*

### Comparing `django_strict_fields-1.3.2/strict_fields/fields.py` & `django_strict_fields-1.3.3/strict_fields/fields.py`

 * *Files identical despite different names*

### Comparing `django_strict_fields-1.3.2/strict_fields/helpers.py` & `django_strict_fields-1.3.3/strict_fields/helpers.py`

 * *Files identical despite different names*

### Comparing `django_strict_fields-1.3.2/PKG-INFO` & `django_strict_fields-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-strict-fields
-Version: 1.3.2
+Version: 1.3.3
 Summary: A collection of fields and utilities to help make model fields more strict.
 Home-page: https://github.com/Opus10/django-strict-fields
 License: BSD-3-Clause
 Author: Tomas Arni Jonasson
 Requires-Python: >=3.8.0,<4
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
@@ -41,15 +41,14 @@
 [View the django-strict-fields docs here](https://django-strict-fields.readthedocs.io/)
 
 ## Installation
 
 Install `django-strict-fields` with:
 
     pip3 install django-strict-fields
-
 After this, add `strict_fields` to the `INSTALLED_APPS` setting of your Django project.
 
 ## Contributing Guide
 
 For information on setting up django-strict-fields for development and contributing changes, view [CONTRIBUTING.md](CONTRIBUTING.md).
 
 ## Primary Authors
```

