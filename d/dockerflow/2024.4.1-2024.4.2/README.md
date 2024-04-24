# Comparing `tmp/dockerflow-2024.4.1.tar.gz` & `tmp/dockerflow-2024.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dockerflow-2024.4.1.tar", last modified: Fri Apr  5 19:40:28 2024, max compression
+gzip compressed data, was "dockerflow-2024.4.2.tar", last modified: Wed Apr 24 20:13:01 2024, max compression
```

## Comparing `dockerflow-2024.4.1.tar` & `dockerflow-2024.4.2.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:40:28.676024 dockerflow-2024.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:40:28.656024 dockerflow-2024.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:40:28.660024 dockerflow-2024.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-05 19:40:28.676024 dockerflow-2024.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:40:28.664024 dockerflow-2024.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7795 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:40:28.664024 dockerflow-2024.4.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/docs/api/django.rst
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/docs/api/fastapi.rst
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/docs/api/flask.rst
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/docs/api/logging.rst
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/docs/api/sanic.rst
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/docs/api/version.rst
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10976 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/docs/development.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14949 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/docs/django.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/docs/fastapi.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15439 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/docs/flask.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/docs/logging.rst
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14771 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/docs/sanic.rst
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-05 19:40:28.676024 dockerflow-2024.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:40:28.656024 dockerflow-2024.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:40:28.664024 dockerflow-2024.4.1/src/dockerflow/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/src/dockerflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:40:28.664024 dockerflow-2024.4.1/src/dockerflow/checks/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/src/dockerflow/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/src/dockerflow/checks/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/src/dockerflow/checks/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:40:28.668024 dockerflow-2024.4.1/src/dockerflow/django/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/src/dockerflow/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/src/dockerflow/django/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/src/dockerflow/django/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/src/dockerflow/django/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/src/dockerflow/django/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/src/dockerflow/django/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:40:28.668024 dockerflow-2024.4.1/src/dockerflow/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/src/dockerflow/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/src/dockerflow/fastapi/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/src/dockerflow/fastapi/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:40:28.668024 dockerflow-2024.4.1/src/dockerflow/flask/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/src/dockerflow/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13516 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/src/dockerflow/flask/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:40:28.668024 dockerflow-2024.4.1/src/dockerflow/flask/checks/
--rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/src/dockerflow/flask/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/src/dockerflow/flask/checks/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/src/dockerflow/flask/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/src/dockerflow/health.py
--rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/src/dockerflow/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:40:28.668024 dockerflow-2024.4.1/src/dockerflow/sanic/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/src/dockerflow/sanic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9912 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/src/dockerflow/sanic/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/src/dockerflow/sanic/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/src/dockerflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:40:28.676024 dockerflow-2024.4.1/src/dockerflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-05 19:40:28.000000 dockerflow-2024.4.1/src/dockerflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-05 19:40:28.000000 dockerflow-2024.4.1/src/dockerflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:40:28.000000 dockerflow-2024.4.1/src/dockerflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:40:28.000000 dockerflow-2024.4.1/src/dockerflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-05 19:40:28.000000 dockerflow-2024.4.1/src/dockerflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 19:40:28.000000 dockerflow-2024.4.1/src/dockerflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:40:28.668024 dockerflow-2024.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:40:28.672024 dockerflow-2024.4.1/tests/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/constraints/django-3.2.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/constraints/django-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/constraints/django-4.1.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/constraints/django-4.2.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/constraints/django-5.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/constraints/fastapi-0.100.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/constraints/flask-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/constraints/flask-2.1.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/constraints/flask-2.2.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/constraints/flask-2.3.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/constraints/flask-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/constraints/sanic-21.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/constraints/sanic-22.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/constraints/sanic-23.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:40:28.672024 dockerflow-2024.4.1/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/core/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/core/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/core/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:40:28.672024 dockerflow-2024.4.1/tests/django/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/django/django_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/django/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/django/test_django.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/django/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:40:28.672024 dockerflow-2024.4.1/tests/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/fastapi/test_fastapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:40:28.672024 dockerflow-2024.4.1/tests/flask/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:40:28.672024 dockerflow-2024.4.1/tests/flask/migrations/
--rwxr-xr-x   0 runner    (1001) docker     (127)       38 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/flask/migrations/README
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/flask/migrations/alembic.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)     2689 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/flask/migrations/env.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      494 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/flask/migrations/script.py.mako
--rw-r--r--   0 runner    (1001) docker     (127)    18297 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/flask/test_flask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:40:28.676024 dockerflow-2024.4.1/tests/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/requirements/default.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/requirements/django.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/requirements/fastapi.txt
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/requirements/flask.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/requirements/lint.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/requirements/sanic.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:40:28.676024 dockerflow-2024.4.1/tests/sanic/
--rw-r--r--   0 runner    (1001) docker     (127)     9854 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tests/sanic/test_sanic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-05 19:40:21.000000 dockerflow-2024.4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:01.699468 dockerflow-2024.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:01.679468 dockerflow-2024.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:01.687468 dockerflow-2024.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-24 20:13:01.699468 dockerflow-2024.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:01.687468 dockerflow-2024.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7795 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:01.687468 dockerflow-2024.4.2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/docs/api/django.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/docs/api/fastapi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/docs/api/flask.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/docs/api/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/docs/api/sanic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/docs/api/version.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10976 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/docs/development.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    18819 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/docs/django.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/docs/fastapi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15445 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/docs/flask.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/docs/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14777 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/docs/sanic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-24 20:13:01.703468 dockerflow-2024.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:01.683468 dockerflow-2024.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:01.691468 dockerflow-2024.4.2/src/dockerflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/src/dockerflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:01.691468 dockerflow-2024.4.2/src/dockerflow/checks/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/src/dockerflow/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/src/dockerflow/checks/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/src/dockerflow/checks/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:01.691468 dockerflow-2024.4.2/src/dockerflow/django/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/src/dockerflow/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/src/dockerflow/django/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/src/dockerflow/django/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/src/dockerflow/django/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/src/dockerflow/django/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/src/dockerflow/django/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:01.691468 dockerflow-2024.4.2/src/dockerflow/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/src/dockerflow/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/src/dockerflow/fastapi/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/src/dockerflow/fastapi/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:01.691468 dockerflow-2024.4.2/src/dockerflow/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/src/dockerflow/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13508 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/src/dockerflow/flask/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:01.691468 dockerflow-2024.4.2/src/dockerflow/flask/checks/
+-rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/src/dockerflow/flask/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/src/dockerflow/flask/checks/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/src/dockerflow/flask/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/src/dockerflow/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/src/dockerflow/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:01.695468 dockerflow-2024.4.2/src/dockerflow/sanic/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/src/dockerflow/sanic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9904 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/src/dockerflow/sanic/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/src/dockerflow/sanic/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/src/dockerflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:01.699468 dockerflow-2024.4.2/src/dockerflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-24 20:13:01.000000 dockerflow-2024.4.2/src/dockerflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-24 20:13:01.000000 dockerflow-2024.4.2/src/dockerflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 20:13:01.000000 dockerflow-2024.4.2/src/dockerflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 20:13:01.000000 dockerflow-2024.4.2/src/dockerflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-24 20:13:01.000000 dockerflow-2024.4.2/src/dockerflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 20:13:01.000000 dockerflow-2024.4.2/src/dockerflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:01.695468 dockerflow-2024.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:01.695468 dockerflow-2024.4.2/tests/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/constraints/django-3.2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/constraints/django-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/constraints/django-4.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/constraints/django-4.2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/constraints/django-5.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/constraints/fastapi-0.100.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/constraints/flask-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/constraints/flask-2.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/constraints/flask-2.2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/constraints/flask-2.3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/constraints/flask-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/constraints/sanic-21.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/constraints/sanic-22.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/constraints/sanic-23.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:01.695468 dockerflow-2024.4.2/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/core/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/core/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/core/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:01.699468 dockerflow-2024.4.2/tests/django/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/django/django_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/django/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/django/test_django.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/django/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:01.699468 dockerflow-2024.4.2/tests/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/fastapi/test_fastapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:01.699468 dockerflow-2024.4.2/tests/flask/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:01.699468 dockerflow-2024.4.2/tests/flask/migrations/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       38 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/flask/migrations/README
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/flask/migrations/alembic.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2689 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/flask/migrations/env.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      494 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/flask/migrations/script.py.mako
+-rw-r--r--   0 runner    (1001) docker     (127)    18297 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/flask/test_flask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:01.699468 dockerflow-2024.4.2/tests/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/requirements/default.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/requirements/django.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/requirements/fastapi.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/requirements/flask.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/requirements/lint.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/requirements/sanic.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:13:01.699468 dockerflow-2024.4.2/tests/sanic/
+-rw-r--r--   0 runner    (1001) docker     (127)     9854 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tests/sanic/test_sanic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-24 20:12:56.000000 dockerflow-2024.4.2/tox.ini
```

### Comparing `dockerflow-2024.4.1/.github/workflows/release.yml` & `dockerflow-2024.4.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/.github/workflows/test.yml` & `dockerflow-2024.4.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/LICENSE` & `dockerflow-2024.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/PKG-INFO` & `dockerflow-2024.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dockerflow
-Version: 2024.4.1
+Version: 2024.4.2
 Summary: Python tools and helpers for Mozilla's Dockerflow
 Home-page: https://github.com/mozilla-services/python-dockerflow
 Author: Mozilla Foundation
 Author-email: dev-webdev@lists.mozilla.org
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment :: Mozilla
```

### Comparing `dockerflow-2024.4.1/README.rst` & `dockerflow-2024.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/docs/Makefile` & `dockerflow-2024.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/docs/api/django.rst` & `dockerflow-2024.4.2/docs/api/django.rst`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/docs/changelog.rst` & `dockerflow-2024.4.2/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/docs/conf.py` & `dockerflow-2024.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/docs/development.rst` & `dockerflow-2024.4.2/docs/development.rst`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/docs/django.rst` & `dockerflow-2024.4.2/docs/sanic.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,152 +1,164 @@
-Django
-======
+Sanic
+=====
 
-The package ``dockerflow.django`` package implements various tools to support
-Django projects that want to follow the Dockerflow specs:
+The package ``dockerflow.sanic`` package implements various tools to support
+Sanic based projects that want to follow the Dockerflow specs:
 
-- A Python logging formatter following the `mozlog`_ format to be used in
-  the ``LOGGING`` setting.
+- A Python logging formatter following the `mozlog`_ format.
 
-- A middleware to emit `request.summary`_ log records based on request specific
-  data.
+- A Sanic extension implements:
 
-- Views for health monitoring:
+  - Emitting of `request.summary`_ log records based on request specific data.
 
-  - ``/__version__`` - Serves a ``version.json`` file
+  - Views for health monitoring:
 
-  - ``/__heartbeat__`` - Run Django checks as configured
-    in the ``DOCKERFLOW_CHECKS`` setting
+    - ``/__version__`` - Serves a ``version.json`` file
 
-  - ``/__lbheartbeat__`` - Retuns a HTTP 200 response
+    - ``/__heartbeat__`` - Runs the configured Dockerflow checks
 
+    - ``/__lbheartbeat__`` - Retuns a HTTP 200 response
 
-- Signals for passed and failed heartbeats.
+  - Signals for passed and failed heartbeats.
+
+  - Built-in Dockerflow checks for SQLAlchemy and Redis connections
+    and validating Alembic migrations.
+
+  - Hooks to add custom Dockerflow checks.
 
 .. _`mozlog`: https://github.com/mozilla-services/Dockerflow/blob/main/docs/mozlog.md
 .. _`request.summary`: https://github.com/mozilla-services/Dockerflow/blob/main/docs/mozlog.md#application-request-summary-type-requestsummary
 
 .. seealso::
 
-    For more information see the :doc:`API documentation <api/django>` for
-    the ``dockerflow.django`` module.
+    For more information see the :doc:`API documentation <api/sanic>` for
+    the ``dockerflow.sanic`` module.
 
 Setup
 -----
 
-To install ``python-dockerflow``'s Django support please follow these steps:
+To install ``python-dockerflow``'s Sanic support please follow these steps:
 
-#. Add ``dockerflow.django`` to your ``INSTALLED_APPS`` setting
+#. In your code where your Sanic application lives set up the dockerflow Sanic
+   extension::
 
-#. Define a ``BASE_DIR`` setting that is the root path of your Django project.
-   This will be used to locate the ``version.json`` file that is generated by
-   CircleCI or another process during deployment.
+     from sanic import Sanic
+     from dockerflow.sanic import Dockerflow
 
-   .. seealso:: :ref:`django-versions` for more information
+     app = Sanic(__name__)
+     dockerflow = Dockerflow(app)
 
-#. Add the ``DockerflowMiddleware`` to your ``MIDDLEWARE_CLASSES`` or
-   ``MIDDLEWARE`` setting::
+#. Make sure the app root path is set correctly as this will be used
+   to locate the ``version.json`` file that is generated by
+   CircleCI or another process during deployment.
 
-    MIDDLEWARE_CLASSES = (
-        # ...
-        'dockerflow.django.middleware.DockerflowMiddleware',
-        # ...
-    )
+   .. seealso:: :ref:`sanic-versions` for more information
 
-#. :ref:`Configure logging <django-logging>` to use the
-   :class:`~dockerflow.logging.JsonLogFormatter`
-   logging formatter for the ``request.summary`` logger (you may have to
-   extend your existing logging configuration!).
+#. Configure logging to use the ``JsonLogFormatter`` logging formatter for the
+   ``request.summary`` logger (you may have to extend your existing logging
+   configuration), see :ref:`sanic-logging` for more information.
 
-.. _django-config:
+.. _sanic-config:
 
 Configuration
 -------------
 
 .. epigraph::
 
    Accept its configuration through environment variables.
 
 There are several options to handle configuration values through
-environment variables, e.g. as shown in the `configuration grid`_ on
-djangopackages.com.
+environment variables when configuring Sanic.
+
+Sanic configuration
+~~~~~~~~~~~~~~~~~~~
 
-``os.environ``
-~~~~~~~~~~~~~~
+The simplest is to use Sanic's own ability to access environment variables
+for settings and other variables.
 
-The simplest is to use Python's ``os.environ`` object to access
-environment variables for settings and other variables, e.g.::
+    Any variables defined with the ``SANIC_`` prefix will be applied to the
+    sanic config. For example, setting ``SANIC_REQUEST_TIMEOUT`` will be
+    loaded by the application automatically and fed into the
+    ``REQUEST_TIMEOUT`` config variable.
 
-    MY_SETTING = os.environ.get('DJANGO_MY_SETTING', 'default value')
+    -- `Sanic docs on configuration`_.
 
 The downside of that is that it nicely works only for string
 based variables, since that's what ``os.environ`` returns.
 
+.. _Sanic docs on configuration: https://sanic.dev/en/guide/deployment/configuration.html#environment-variables
+
 python-decouple
 ~~~~~~~~~~~~~~~
 
 A good replacement is python-decouple_ as it's agnostic to the
 framework in use and offers casting the returned value to the type
 wanted, e.g.::
 
     from decouple import config
 
-    MY_SETTING = config('DJANGO_MY_SETTING', default='default value')
-    DEBUG = config('DJANGO_DEBUG', default=False, cast=bool)
+    MY_SETTING = config('SANIC_MY_SETTING', default='default value')
+    DEBUG = config('SANIC_DEBUG', default=False, cast=bool)
 
-As you can see the ``DEBUG`` setting would be populated from the
-``DJANGO_DEBUG`` environment variable but also be cast as a boolean
+As you can see the ``DEBUG`` configuration value would be populated from
+the ``SANIC_DEBUG`` environment variable but also be cast as a boolean
 (while considering the string values ``'1'``, ``'yes'``, ``'true'`` and
 ``'on'`` as truthy values, and similar for falsey values).
 
-django-environ
-~~~~~~~~~~~~~~
-
-Django-environ_ follows similar patterns as python-decouple but implements
-specific casters for typical Django settings. E.g.::
+sanic-envconfig
+~~~~~~~~~~~~~~~
 
-    import environ
-    env = environ.Env()
+If you need to solve more complex configuration scenarios there are tools
+like sanic-envconfig_ which allows loading settings for different
+environments (e.g. dev, stage, prod) via environment variables.
+It provides a small Python base class to allow setting up the configuration
+values:
+
+E.g. in a ``config.py`` file next to your application::
+
+    from sanic_envconfig import EnvConfig
+
+    class Dev(EnvConfig):
+        DEBUG: bool = True
+        DB_URL: str = None
+        WORKERS: int = 1
+        PORT: int = 5000
 
-    MY_SETTING = env.str('DJANGO_MY_SETTING', default='default value')
-    DEBUG = env.bool('DJANGO_DEBUG', default=False)
-    DATABASES = {
-        'default': env.db(),  # automatically looks for DATABASE_URL
-    }
+    class Prod(Dev):
+        DEBUG: bool = False
 
-django-configurations
-~~~~~~~~~~~~~~~~~~~~~
+Then in your application code::
 
-If you're interested in even more complex scenarios there are
-tools like django-configurations_ which allows loading different sets
-of settings depending on an additional environment variable
-``DJANGO_CONFIGURATION`` to separate settings by environment
-(e.g. dev, stage, prod). It also ships with ``Value`` classes that
-implement configuration parsing from environment variable and casting,
-e.g.::
-
-    from configurations import Configuration, values
-
-    class Dev(Configuration):
-        SESSION_COOKIE_SECURE = False
-        DEBUG = values.BooleanValue(default=False)
+    import os
+    from sanic import Sanic
 
-    class Prod(Dev):
-        SESSION_COOKIE_SECURE = True
+    app = Sanic(__name__)
+    app.config.from_object(os.environ.get('SANIC_CONFIG', 'config.Dev'))
 
 In that example the configuration class that is given in the
-``DJANGO_CONFIGURATION`` environment variable would be used as the base
-for Django's settings.
+``SANIC_CONFIG`` environment variable would be used to update
+the default Sanic configuration values while allowing to override
+the values via environment variables.
+
+It's recommended to use the sanic-envconfig feature to define a prefix for the
+environment variable it uses to check, e.g.::
+
+    from sanic_envconfig import EnvConfig
+
+    class Dev(EnvConfig):
+        _ENV_PREFIX = 'ACME_'
+        DEBUG = True
+
+To override the config value of ``DEBUG`` the environment variable would be
+called ``ACME_DEBUG``.
 
-.. _configuration grid: https://djangopackages.org/grids/g/configuration/
 .. _python-decouple: https://pypi.python.org/pypi/python-decouple
-.. _Django-environ: https://django-environ.readthedocs.io/
-.. _Django-configurations: https://django-configurations.readthedocs.io/
+.. _sanic-envconfig: https://github.com/jamesstidard/sanic-envconfig
 
-.. _django-serving:
+.. _sanic-serving:
 
 ``PORT``
 --------
 
 .. epigraph::
 
    Listen on environment variable ``$PORT`` for HTTP requests.
@@ -158,110 +170,91 @@
 It's recommended to use port ``8000`` by default.
 
 Gunicorn
 ~~~~~~~~
 
 Gunicorn automatically will bind to the hostname:port combination of
 ``0.0.0.0:$PORT`` if it find the :envvar:`PORT` environment variable.
-That means running gunicorn is as simple as using this::
+That means running gunicorn is as simple as using this, for example::
 
-    gunicorn myproject.wsgi:application --workers 4 --access-logfile -
+    gunicorn myproject:app --worker-class sanic.worker.GunicornWorker
 
 .. seealso::
 
     The `full gunicorn documentation <http://docs.gunicorn.org/>`_
     for more details.
 
-uWSGI
-~~~~~
-
-For uWSGI all you have to do is to bind on the :envvar:`PORT` when you
-define the ``uwsgi.ini``, e.g.:
+ASGI
+~~~~
 
-.. code-block:: ini
-
-    [uwsgi]
-    http-socket = :$(PORT)
-    master = true
-    processes = 4
-    module = myproject.wsgi:application
-    chdir = /app
-    enable-threads = True
+Sanic is also ASGI-compliant. This means you can use your preferred ASGI
+webserver to run Sanic. The three main implementations of ASGI are Daphne,
+Uvicorn, and Hypercorn.
 
 .. seealso::
 
-    The `full uWSGI documentation <http://uwsgi-docs.readthedocs.io/>`_
-    for more details.
+    The `Sanic deployment documentation`_ has more details.
 
-.. _django-versions:
+.. _Sanic deployment documentation: https://sanic.dev/en/guide/deployment/running.html#asgi
+
+.. _sanic-versions:
 
 Versions
 --------
 
 .. epigraph::
 
    Must have a JSON version object at /app/version.json.
 
-Dockerflow requires writing a `version object`_ to the file ``/app/version.json``
-as seen from the docker container to be served under the URL path
-``/__version__``.
-
-To facilitate this python-dockerflow contains a Django view to read the
-file under path ``BASE_DIR + 'version.json'`` where
-``BASE_DIR`` is required to be defined in the Django project settings, e.g.:
-
-.. code-block:: python
-
-    import os
-    BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
-
-Assuming that the ``settings.py`` file is contained in the project folder
-That means the ``BASE_DIR`` setting will be the one where the ``manage.py``
-file is located in the below example directory tree:
-
-.. code-block:: text
-   :emphasize-lines: 14,22
-
-    .
-    ├── .dockerignore
-    ├── .gitignore
-    ├── Dockerfile
-    ├── README.rst
-    ├── circle.yml
-    ├── manage.py
-    ├── requirements.txt
-    ├── staticfiles
-    │   └── ..
-    ├── tests
-    │   └── ..
-    ├── version.json
-    ├── myproject
-    │   ├── app1
-    │   │   ├── ..
-    │   │   └── ..
-    │   ├── app2
-    │   │   ├── ..
-    │   │   └── ..
-    │   ├── settings.py
-    │   └── urls.py
-    └── ..
+Dockerflow requires writing a `version object`_ to the file
+``/app/version.json`` as seen from the docker container to be served under
+the URL path ``/__version__``.
+
+To facilitate this python-dockerflow comes with a Sanic view to read the
+file under the current worked directory (``.``).
+
+If you'd like to override the location from which the view is reading the
+``version.json`` file from, simply override the optional ``version_path``
+parameter to the :class:`~dockerflow.sanic.app.Dockerflow` class, e.g.::
+
+    from sanic import Sanic
+    from dockerflow.sanic import Dockerflow
+
+    app = Sanic(__name__)
+    dockerflow = Dockerflow(app, version_path='/app')
+
+Alternatively if you'd like to completely override the way the version
+information is read use the
+:meth:`~dockerflow.sanic.app.Dockerflow.version_callback` decorator to
+decorate a callback that gets the ``version_path`` value passed. E.g.::
+
+    import json
+    from sanic import Sanic
+    from dockerflow.sanic import Dockerflow
+
+    app = Sanic(__name__)
+    dockerflow = Dockerflow(app)
+
+    @dockerflow.version_callback
+    def my_version(root):
+        return json.loads(os.path.join(root, 'acme_version.json'))
 
 .. _version object: https://github.com/mozilla-services/Dockerflow/blob/main/docs/version_object.md
 
-.. _django-health:
+.. _sanic-health:
 
 Health monitoring
 -----------------
 
 Health monitoring happens via three different views following the Dockerflow_
 spec:
 
 .. http:get:: /__version__
 
-   The view that serves the :ref:`version information <django-versions>`.
+   The view that serves the :ref:`version information <sanic-versions>`.
 
    **Example request**:
 
    .. sourcecode:: http
 
       GET /__version__ HTTP/1.1
       Host: example.com
@@ -282,31 +275,71 @@
       }
 
    :statuscode 200: no error
    :statuscode 404: a version.json wasn't found
 
 .. http:get:: /__heartbeat__
 
-   The heartbeat view will go through the list of configured Dockerflow
-   checks in the :ref:`DOCKERFLOW_CHECKS` setting, run each check, and, if
-   `settings.DEBUG` is `True`, add their results to a JSON response.
+   The heartbeat view will go through the list of registered Dockerflow
+   checks, run each check and add their results to a JSON response.
 
-   The view will return HTTP responses with either a status code of 200 if
+   The view will return HTTP responses with either an status code of 200 if
    all checks ran successfully or 500 if there was one or more warnings or
    errors returned by the checks.
 
+   **Built-in Dockerflow checks:**
+
+   There are a few built-in checks that are automatically added to the list
+   of checks if the appropriate Sanic extension objects are passed to
+   the :class:`~dockerflow.sanic.app.Dockerflow` class during instantiation.
+
+   For detailed examples please see the API documentation for the built-in
+   :ref:`Sanic Dockerflow checks <sanic-checks>`.
+
    **Custom Dockerflow checks:**
 
-   To write your own custom Dockerflow checks, please follow the documentation
-   about :mod:`Django's system check framework <django.core.checks>` and
-   particularly the section **"Writing your own checks"**.
-
-   .. note:: Don't forget to add the check additionally to the
-             :ref:`DOCKERFLOW_CHECKS` setting once you've added it to your
-             code.
+   To write your own custom Dockerflow checks simply write a function
+   that returns a list of one or many check message instances representing
+   the severity of the check result. The :mod:`dockerflow.sanic.checks`
+   module contains a series of predefined check messages for the
+   severity levels: :class:`~dockerflow.sanic.checks.Debug`,
+   :class:`~dockerflow.sanic.checks.Info`,
+   :class:`~dockerflow.sanic.checks.Warning`,
+   :class:`~dockerflow.sanic.checks.Error`,
+   :class:`~dockerflow.sanic.checks.Critical`.
+
+   Here's an example of a check that handles various levels of exceptions
+   from an external storage system with different check message::
+
+       from sanic import Sanic
+       from dockerflow.sanic import checks, Dockerflow
+
+       app = Sanic(__name__)
+       dockerflow = Dockerflow(app)
+
+       @dockerflow.check
+       async def storage_reachable():
+           result = []
+           try:
+               acme.storage.ping()
+           except SlowConnectionException as exc:
+               result.append(checks.Warning(exc.msg, id='acme.health.0002'))
+           except StorageException as exc:
+               result.append(checks.Error(exc.msg, id='acme.health.0001'))
+           return result
+
+    also works without async::
+
+       @dockerflow.check
+           def storage_reachable():
+               result = []
+               # ...
+
+   Notice the use of the :meth:`~dockerflow.sanic.app.Dockerflow.check`
+   decorator to mark the check to be used.
 
    **Example request**:
 
    .. sourcecode:: http
 
       GET /__heartbeat__ HTTP/1.1
       Host: example.com
@@ -363,36 +396,38 @@
       Vary: Accept-Encoding
       Content-Type: application/json
 
    :statuscode 200: no error
 
 .. _Dockerflow: https://github.com/mozilla-services/Dockerflow
 
-.. _django-logging:
+.. _sanic-logging:
 
 Logging
 -------
 
 Dockerflow provides a :class:`~dockerflow.logging.JsonLogFormatter` Python
 logging formatter class.
 
-To use it, put something like this in your Django ``settings`` file and
-configure **at least** the ``request.summary`` logger that way::
+To use it, pass something like this to your Sanic app when it is initialized
+for at least the ``request.summary`` logger::
 
-    LOGGING = {
+    from sanic import Sanic
+
+    log_config = {
         'version': 1,
         'formatters': {
             'json': {
                 '()': 'dockerflow.logging.JsonLogFormatter',
                 'logger_name': 'myproject'
             }
         },
         'filters': {
             'request_id': {
-                '()': 'dockerflow.logging.RequestIdFilter',
+                '()': 'dockerflow.logging.RequestIdLogFilter',
             },
         },
         'handlers': {
             'console': {
                 'level': 'DEBUG',
                 'class': 'logging.StreamHandler',
                 'formatter': 'json',
@@ -401,19 +436,36 @@
         },
         'loggers': {
             'request.summary': {
                 'handlers': ['console'],
                 'level': 'DEBUG',
             },
         }
+    })
+
+    sanic = Sanic(__name__, log_config=log)
+
+By default the ``log_info`` parameter has the value of
+``sanic.log.LOGGING_CONFIG_DEFAULTS``.
+
+Alternatively you can also pass the same logging config dictionary to the
+``logging.conf.dictConfig`` utility **BEFORE** your Sanic app is initialized::
+
+    from logging.conf import dictConfig
+    from sanic import Sanic
+
+    log_config = {
+        # ...
     }
 
-In order to include querystrings in the request summary log, set this flag in settings:
+    dictConfig(log_config)
 
-.. code-block:: python
+    sanic = Sanic(__name__)
+
+In order to include querystrings in the request summary log, set this flag in :ref:`configuration <sanic-config>`::
 
     DOCKERFLOW_SUMMARY_LOG_QUERYSTRING = True
 
 
 MozLog App-Specific Fields
 ~~~~~~~~~~~~~~~~~~~~~~~~~~
 
@@ -429,91 +481,25 @@
 
 
 Requests Correlation ID
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 A unique request ID is read from the ``X-Request-ID`` request header, and a UUID4 value is generated if unset.
 
-Leveraging the ``RequestIdFilter`` in logging configuration as shown above will add a ``rid`` field into the ``Fields`` entry of all log messages.
+Leveraging the ``RequestIdLogFilter`` in logging configuration as shown above will add a ``rid`` field into the ``Fields`` entry of all log messages.
 
 The header name to obtain the request ID can be customized in settings:
 
 .. code-block:: python
 
     DOCKERFLOW_REQUEST_ID_HEADER_NAME = "X-Cloud-Trace-Context"
 
 
-.. _django-static:
+.. _sanic-static:
 
 Static content
 --------------
 
-To properly serve static content it's recommended to use `Whitenoise`_.
-It contains a middleware that is able to serve files that were built by
-Django's collectstatic management command (e.g. including bundle files
-built by django-pipeline) with **far-future headers** and proper response
-headers for the AWS CDN to work.
-
-To enable Whitenoise, please install it from PyPI and then enable it
-in your Django projet:
-
-#. Set your ``STATIC_ROOT`` setting::
-
-       STATIC_ROOT = os.path.join(BASE_DIR, 'staticfiles')
-
-#. Add the middleware to your ``MIDDLEWARE`` (or ``MIDDLEWARE_CLASSES``) setting::
-
-       MIDDLEWARE_CLASSES = [
-           # 'django.middleware.security.SecurityMiddleware',
-           'whitenoise.middleware.WhiteNoiseMiddleware',
-           # ...
-       ]
-
-   Make sure to follow the SecurityMiddleware.
-
-#. Enable the staticfiles_ storage that is able to compress files during
-   collection and ship them with far-future headers::
-
-       STATICFILES_STORAGE = 'whitenoise.storage.CompressedManifestStaticFilesStorage'
-
-.. _Whitenoise: https://whitenoise.readthedocs.io/
-
-#. Install brotlipy_ so the storage can generate compressed files of your
-   static files in the brotli_ format.
-
-For more configuration options and details how to use Whitenoise see
-the section about `Using WhiteNoise with Django`_ in its documentation.
-
-.. _staticfiles: https://docs.djangoproject.com/en/stable/howto/static-files/
-.. _brotli: https://en.wikipedia.org/wiki/Brotli
-.. _brotlipy: http://brotlipy.readthedocs.org/en/latest/
-.. _`Using WhiteNoise with Django`: https://whitenoise.readthedocs.io/en/stable/django.html
-
-Settings
---------
-
-.. _DOCKERFLOW_VERSION_CALLBACK:
-
-``DOCKERFLOW_VERSION_CALLBACK``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-The dotted import path for the callable that
-returns the content to return under ``/__version__``.
-
-Defaults to ``'dockerflow.version.get_version'`` which will be passed the
-``BASE_DIR`` setting by default.
-
-.. _DOCKERFLOW_CHECKS:
-
-``DOCKERFLOW_CHECKS``
-~~~~~~~~~~~~~~~~~~~~~
-
-A list of dotted import paths to register during
-Django setup, to be used in the rendering of the ``/__heartbeat__`` view.
-Defaults to:
-
-.. code-block:: python
+Please refer to the Sanic documentation about `serving static files`_ for more
+information.
 
-    DOCKERFLOW_CHECKS = [
-        'dockerflow.django.checks.check_database_connected',
-        'dockerflow.django.checks.check_migrations_applied',
-    ]
+.. _serving static files: https://sanic.dev/en/guide/basics/routing.html#static-files
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dockerflow-2024.4.1/docs/fastapi.rst` & `dockerflow-2024.4.2/docs/fastapi.rst`

 * *Files 1% similar despite different names*

```diff
@@ -296,15 +296,15 @@
             'json': {
                 '()': 'dockerflow.logging.JsonLogFormatter',
                 'logger_name': 'myproject'
             }
         },
         'filters': {
             'request_id': {
-                '()': 'dockerflow.logging.RequestIdFilter',
+                '()': 'dockerflow.logging.RequestIdLogFilter',
             },
         },
         'handlers': {
             'console': {
                 'level': 'DEBUG',
                 'class': 'logging.StreamHandler',
                 'filters': ['request_id'],
@@ -342,15 +342,15 @@
 
 
 Requests Correlation ID
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 A unique request ID is read from the ``X-Request-ID`` request header, and a UUID4 value is generated if unset.
 
-Leveraging the ``RequestIdFilter`` in logging configuration as shown above will add a ``rid`` field into the ``Fields`` entry of all log messages.
+Leveraging the ``RequestIdLogFilter`` in logging configuration as shown above will add a ``rid`` field into the ``Fields`` entry of all log messages.
 
 The header name to obtain the request ID can be customized in settings:
 
 .. code-block:: python
 
     app.state.DOCKERFLOW_REQUEST_ID_HEADER_NAME = "X-Cloud-Trace-Context"
```

### Comparing `dockerflow-2024.4.1/docs/flask.rst` & `dockerflow-2024.4.2/docs/flask.rst`

 * *Files 1% similar despite different names*

```diff
@@ -439,15 +439,15 @@
             'json': {
                 '()': 'dockerflow.logging.JsonLogFormatter',
                 'logger_name': 'myproject'
             }
         },
         'filters': {
             'request_id': {
-                '()': 'dockerflow.logging.RequestIdFilter',
+                '()': 'dockerflow.logging.RequestIdLogFilter',
             },
         },
         'handlers': {
             'console': {
                 'level': 'DEBUG',
                 'class': 'logging.StreamHandler',
                 'formatter': 'json',
@@ -482,15 +482,15 @@
 
 
 Requests Correlation ID
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 A unique request ID is read from the ``X-Request-ID`` request header, and a UUID4 value is generated if unset.
 
-Leveraging the ``RequestIdFilter`` in logging configuration as shown above will add a ``rid`` field into the ``Fields`` entry of all log messages.
+Leveraging the ``RequestIdLogFilter`` in logging configuration as shown above will add a ``rid`` field into the ``Fields`` entry of all log messages.
 
 The header name to obtain the request ID can be customized in settings:
 
 .. code-block:: python
 
     DOCKERFLOW_REQUEST_ID_HEADER_NAME = "X-Cloud-Trace-Context"
```

### Comparing `dockerflow-2024.4.1/docs/index.rst` & `dockerflow-2024.4.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/docs/logging.rst` & `dockerflow-2024.4.2/docs/logging.rst`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             'json': {
                 '()': 'dockerflow.logging.JsonLogFormatter',
                 'logger_name': 'myproject'
             }
         },
         'filters': {
             'request_id': {
-                '()': 'dockerflow.logging.RequestIdFilter',
+                '()': 'dockerflow.logging.RequestIdLogFilter',
             },
         },
         'handlers': {
             'console': {
                 'level': 'DEBUG',
                 'class': 'logging.StreamHandler',
                 'formatter': 'json',
@@ -86,15 +86,15 @@
     [formatters]
     keys = json
 
     [filters]
     keys = request_id
 
     [filter_request_id]
-    class = dockerflow.logging.RequestIdFilter
+    class = dockerflow.logging.RequestIdLogFilter
 
     [logger_root]
     level = INFO
     handlers = console
 
     [logger_myproject]
     level = DEBUG
```

### Comparing `dockerflow-2024.4.1/docs/sanic.rst` & `dockerflow-2024.4.2/src/dockerflow/flask/app.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,505 +1,400 @@
-Sanic
-=====
-
-The package ``dockerflow.sanic`` package implements various tools to support
-Sanic based projects that want to follow the Dockerflow specs:
-
-- A Python logging formatter following the `mozlog`_ format.
-
-- A Sanic extension implements:
-
-  - Emitting of `request.summary`_ log records based on request specific data.
-
-  - Views for health monitoring:
-
-    - ``/__version__`` - Serves a ``version.json`` file
-
-    - ``/__heartbeat__`` - Runs the configured Dockerflow checks
-
-    - ``/__lbheartbeat__`` - Retuns a HTTP 200 response
-
-  - Signals for passed and failed heartbeats.
-
-  - Built-in Dockerflow checks for SQLAlchemy and Redis connections
-    and validating Alembic migrations.
-
-  - Hooks to add custom Dockerflow checks.
-
-.. _`mozlog`: https://github.com/mozilla-services/Dockerflow/blob/main/docs/mozlog.md
-.. _`request.summary`: https://github.com/mozilla-services/Dockerflow/blob/main/docs/mozlog.md#application-request-summary-type-requestsummary
-
-.. seealso::
-
-    For more information see the :doc:`API documentation <api/sanic>` for
-    the ``dockerflow.sanic`` module.
-
-Setup
------
-
-To install ``python-dockerflow``'s Sanic support please follow these steps:
-
-#. In your code where your Sanic application lives set up the dockerflow Sanic
-   extension::
-
-     from sanic import Sanic
-     from dockerflow.sanic import Dockerflow
-
-     app = Sanic(__name__)
-     dockerflow = Dockerflow(app)
-
-#. Make sure the app root path is set correctly as this will be used
-   to locate the ``version.json`` file that is generated by
-   CircleCI or another process during deployment.
-
-   .. seealso:: :ref:`sanic-versions` for more information
-
-#. Configure logging to use the ``JsonLogFormatter`` logging formatter for the
-   ``request.summary`` logger (you may have to extend your existing logging
-   configuration), see :ref:`sanic-logging` for more information.
-
-.. _sanic-config:
-
-Configuration
--------------
-
-.. epigraph::
-
-   Accept its configuration through environment variables.
-
-There are several options to handle configuration values through
-environment variables when configuring Sanic.
-
-Sanic configuration
-~~~~~~~~~~~~~~~~~~~
-
-The simplest is to use Sanic's own ability to access environment variables
-for settings and other variables.
-
-    Any variables defined with the ``SANIC_`` prefix will be applied to the
-    sanic config. For example, setting ``SANIC_REQUEST_TIMEOUT`` will be
-    loaded by the application automatically and fed into the
-    ``REQUEST_TIMEOUT`` config variable.
-
-    -- `Sanic docs on configuration`_.
-
-The downside of that is that it nicely works only for string
-based variables, since that's what ``os.environ`` returns.
-
-.. _Sanic docs on configuration: https://sanic.dev/en/guide/deployment/configuration.html#environment-variables
-
-python-decouple
-~~~~~~~~~~~~~~~
-
-A good replacement is python-decouple_ as it's agnostic to the
-framework in use and offers casting the returned value to the type
-wanted, e.g.::
-
-    from decouple import config
-
-    MY_SETTING = config('SANIC_MY_SETTING', default='default value')
-    DEBUG = config('SANIC_DEBUG', default=False, cast=bool)
-
-As you can see the ``DEBUG`` configuration value would be populated from
-the ``SANIC_DEBUG`` environment variable but also be cast as a boolean
-(while considering the string values ``'1'``, ``'yes'``, ``'true'`` and
-``'on'`` as truthy values, and similar for falsey values).
-
-sanic-envconfig
-~~~~~~~~~~~~~~~
-
-If you need to solve more complex configuration scenarios there are tools
-like sanic-envconfig_ which allows loading settings for different
-environments (e.g. dev, stage, prod) via environment variables.
-It provides a small Python base class to allow setting up the configuration
-values:
-
-E.g. in a ``config.py`` file next to your application::
-
-    from sanic_envconfig import EnvConfig
-
-    class Dev(EnvConfig):
-        DEBUG: bool = True
-        DB_URL: str = None
-        WORKERS: int = 1
-        PORT: int = 5000
-
-    class Prod(Dev):
-        DEBUG: bool = False
-
-Then in your application code::
-
-    import os
-    from sanic import Sanic
-
-    app = Sanic(__name__)
-    app.config.from_object(os.environ.get('SANIC_CONFIG', 'config.Dev'))
-
-In that example the configuration class that is given in the
-``SANIC_CONFIG`` environment variable would be used to update
-the default Sanic configuration values while allowing to override
-the values via environment variables.
-
-It's recommended to use the sanic-envconfig feature to define a prefix for the
-environment variable it uses to check, e.g.::
-
-    from sanic_envconfig import EnvConfig
-
-    class Dev(EnvConfig):
-        _ENV_PREFIX = 'ACME_'
-        DEBUG = True
-
-To override the config value of ``DEBUG`` the environment variable would be
-called ``ACME_DEBUG``.
-
-.. _python-decouple: https://pypi.python.org/pypi/python-decouple
-.. _sanic-envconfig: https://github.com/jamesstidard/sanic-envconfig
-
-.. _sanic-serving:
-
-``PORT``
---------
-
-.. epigraph::
-
-   Listen on environment variable ``$PORT`` for HTTP requests.
-
-Depending on which WSGI server you are using to run your Python application
-there are different ways to accept the :envvar:`PORT` as the port to launch
-your application with.
-
-It's recommended to use port ``8000`` by default.
-
-Gunicorn
-~~~~~~~~
-
-Gunicorn automatically will bind to the hostname:port combination of
-``0.0.0.0:$PORT`` if it find the :envvar:`PORT` environment variable.
-That means running gunicorn is as simple as using this, for example::
-
-    gunicorn myproject:app --worker-class sanic.worker.GunicornWorker
-
-.. seealso::
-
-    The `full gunicorn documentation <http://docs.gunicorn.org/>`_
-    for more details.
-
-ASGI
-~~~~
-
-Sanic is also ASGI-compliant. This means you can use your preferred ASGI
-webserver to run Sanic. The three main implementations of ASGI are Daphne,
-Uvicorn, and Hypercorn.
-
-.. seealso::
-
-    The `Sanic deployment documentation`_ has more details.
-
-.. _Sanic deployment documentation: https://sanic.dev/en/guide/deployment/running.html#asgi
-
-.. _sanic-versions:
-
-Versions
---------
-
-.. epigraph::
-
-   Must have a JSON version object at /app/version.json.
-
-Dockerflow requires writing a `version object`_ to the file
-``/app/version.json`` as seen from the docker container to be served under
-the URL path ``/__version__``.
-
-To facilitate this python-dockerflow comes with a Sanic view to read the
-file under the current worked directory (``.``).
-
-If you'd like to override the location from which the view is reading the
-``version.json`` file from, simply override the optional ``version_path``
-parameter to the :class:`~dockerflow.sanic.app.Dockerflow` class, e.g.::
-
-    from sanic import Sanic
-    from dockerflow.sanic import Dockerflow
-
-    app = Sanic(__name__)
-    dockerflow = Dockerflow(app, version_path='/app')
-
-Alternatively if you'd like to completely override the way the version
-information is read use the
-:meth:`~dockerflow.sanic.app.Dockerflow.version_callback` decorator to
-decorate a callback that gets the ``version_path`` value passed. E.g.::
-
-    import json
-    from sanic import Sanic
-    from dockerflow.sanic import Dockerflow
-
-    app = Sanic(__name__)
-    dockerflow = Dockerflow(app)
-
-    @dockerflow.version_callback
-    def my_version(root):
-        return json.loads(os.path.join(root, 'acme_version.json'))
-
-.. _version object: https://github.com/mozilla-services/Dockerflow/blob/main/docs/version_object.md
-
-.. _sanic-health:
-
-Health monitoring
------------------
-
-Health monitoring happens via three different views following the Dockerflow_
-spec:
-
-.. http:get:: /__version__
-
-   The view that serves the :ref:`version information <sanic-versions>`.
-
-   **Example request**:
-
-   .. sourcecode:: http
-
-      GET /__version__ HTTP/1.1
-      Host: example.com
-
-   **Example response**:
-
-   .. sourcecode:: http
-
-      HTTP/1.1 200 OK
-      Vary: Accept-Encoding
-      Content-Type: application/json
-
-      {
-        "commit": "52ce614fbf99540a1bf6228e36be6cef63b4d73b",
-        "version": "2017.11.0",
-        "source": "https://github.com/mozilla/telemetry-analysis-service",
-        "build": "https://circleci.com/gh/mozilla/telemetry-analysis-service/2223"
-      }
-
-   :statuscode 200: no error
-   :statuscode 404: a version.json wasn't found
-
-.. http:get:: /__heartbeat__
-
-   The heartbeat view will go through the list of registered Dockerflow
-   checks, run each check and add their results to a JSON response.
-
-   The view will return HTTP responses with either an status code of 200 if
-   all checks ran successfully or 500 if there was one or more warnings or
-   errors returned by the checks.
-
-   **Built-in Dockerflow checks:**
-
-   There are a few built-in checks that are automatically added to the list
-   of checks if the appropriate Sanic extension objects are passed to
-   the :class:`~dockerflow.sanic.app.Dockerflow` class during instantiation.
-
-   For detailed examples please see the API documentation for the built-in
-   :ref:`Sanic Dockerflow checks <sanic-checks>`.
+# This Source Code Form is subject to the terms of the Mozilla Public
+# License, v. 2.0. If a copy of the MPL was not distributed with this
+# file, you can obtain one at http://mozilla.org/MPL/2.0/.
+import logging
+import os
+import time
+import warnings
+
+import flask
+from werkzeug.exceptions import InternalServerError
+
+from dockerflow import checks
+from dockerflow.logging import get_or_generate_request_id, request_id_context
+
+from .. import version
+from .checks import (
+    check_database_connected,
+    check_migrations_applied,
+    check_redis_connected,
+)
+from .signals import heartbeat_failed, heartbeat_passed
+
+try:
+    from flask_login import current_user
+except ImportError:  # pragma: nocover
+    has_flask_login = False
+else:
+    has_flask_login = True
+
+try:
+    from sqlalchemy.exc import SQLAlchemyError as UserLoadingError
+except ImportError:
+    # Just in case sqlalchemy isn't even used
+    class UserLoadingError(Exception):
+        pass
+
+
+class HeartbeatFailure(InternalServerError):
+    pass
+
+
+def extract_request_id(request):
+    """Extract request ID from request."""
+    rid = get_or_generate_request_id(
+        flask.request.headers,
+        header_name=flask.current_app.config.get(
+            "DOCKERFLOW_REQUEST_ID_HEADER_NAME", None
+        ),
+    )
+    request_id_context.set(rid)
+    flask.g._request_id = rid  # For retro-compatibility and tests.
+    if not hasattr(flask.g, "request_id"):
+        flask.g.request_id = rid
 
-   **Custom Dockerflow checks:**
 
-   To write your own custom Dockerflow checks simply write a function
-   that returns a list of one or many check message instances representing
-   the severity of the check result. The :mod:`dockerflow.sanic.checks`
-   module contains a series of predefined check messages for the
-   severity levels: :class:`~dockerflow.sanic.checks.Debug`,
-   :class:`~dockerflow.sanic.checks.Info`,
-   :class:`~dockerflow.sanic.checks.Warning`,
-   :class:`~dockerflow.sanic.checks.Error`,
-   :class:`~dockerflow.sanic.checks.Critical`.
+class Dockerflow(object):
+    """
+    The Dockerflow Flask extension. Set it up like this:
 
-   Here's an example of a check that handles various levels of exceptions
-   from an external storage system with different check message::
+    .. code-block:: python
+       :caption: ``myproject.py``
 
-       from sanic import Sanic
-       from dockerflow.sanic import checks, Dockerflow
+       from flask import Flask
+       from dockerflow.flask import Dockerflow
 
-       app = Sanic(__name__)
+       app = Flask(__name__)
        dockerflow = Dockerflow(app)
 
-       @dockerflow.check
-       async def storage_reachable():
-           result = []
-           try:
-               acme.storage.ping()
-           except SlowConnectionException as exc:
-               result.append(checks.Warning(exc.msg, id='acme.health.0002'))
-           except StorageException as exc:
-               result.append(checks.Error(exc.msg, id='acme.health.0001'))
-           return result
-
-    also works without async::
-
-       @dockerflow.check
-           def storage_reachable():
-               result = []
-               # ...
-
-   Notice the use of the :meth:`~dockerflow.sanic.app.Dockerflow.check`
-   decorator to mark the check to be used.
-
-   **Example request**:
-
-   .. sourcecode:: http
-
-      GET /__heartbeat__ HTTP/1.1
-      Host: example.com
-
-   **Example response**:
-
-   .. sourcecode:: http
-
-      HTTP/1.1 500 Internal Server Error
-      Vary: Accept-Encoding
-      Content-Type: application/json
-
-      {
-        "status": "warning",
-        "checks": {
-          "check_debug": "ok",
-          "check_sts_preload": "warning"
-        },
-        "details": {
-          "check_sts_preload": {
-            "status": "warning",
-            "level": 30,
-            "messages": {
-              "security.W021": "You have not set the SECURE_HSTS_PRELOAD setting to True. Without this, your site cannot be submitted to the browser preload list."
-            }
-          }
-        }
-      }
+    Or if you use the Flask application factory pattern, in
+    an own module set up Dockerflow first:
 
-   :statuscode 200: no error, with potential warnings
-   :statuscode 500: there was an error
+    .. code-block:: python
+       :caption: ``myproject/deployment.py``
 
-   .. note:: Failed status code can be configured with the ``DOCKERFLOW_HEARTBEAT_FAILED_STATUS_CODE``
-             setting (eg. 503 instead of 500)
+       from dockerflow.flask import Dockerflow
 
-.. http:get:: /__lbheartbeat__
-
-   The view that simply returns a successful HTTP response so that a load
-   balancer in front of the application can check that the web application
-   has started up.
-
-   **Example request**:
-
-   .. sourcecode:: http
-
-      GET /__lbheartbeat__ HTTP/1.1
-      Host: example.com
-
-   **Example response**:
-
-   .. sourcecode:: http
-
-      HTTP/1.1 200 OK
-      Vary: Accept-Encoding
-      Content-Type: application/json
-
-   :statuscode 200: no error
-
-.. _Dockerflow: https://github.com/mozilla-services/Dockerflow
-
-.. _sanic-logging:
-
-Logging
--------
-
-Dockerflow provides a :class:`~dockerflow.logging.JsonLogFormatter` Python
-logging formatter class.
-
-To use it, pass something like this to your Sanic app when it is initialized
-for at least the ``request.summary`` logger::
-
-    from sanic import Sanic
-
-    log_config = {
-        'version': 1,
-        'formatters': {
-            'json': {
-                '()': 'dockerflow.logging.JsonLogFormatter',
-                'logger_name': 'myproject'
-            }
-        },
-        'filters': {
-            'request_id': {
-                '()': 'dockerflow.logging.RequestIdFilter',
-            },
-        },
-        'handlers': {
-            'console': {
-                'level': 'DEBUG',
-                'class': 'logging.StreamHandler',
-                'formatter': 'json',
-                'filters': ['request_id']
-            },
-        },
-        'loggers': {
-            'request.summary': {
-                'handlers': ['console'],
-                'level': 'DEBUG',
-            },
+       dockerflow = Dockerflow()
+
+    and then import and initialize it with the Flask application
+    object when you create the application:
+
+    .. code-block:: python
+       :caption: ``myproject/app.py``
+
+       def create_app(config_filename):
+           app = Flask(__name__)
+           app.config.from_pyfile(config_filename)
+
+           from myproject.deployment import dockerflow
+           dockerflow.init_app(app)
+
+           from myproject.views.admin import admin
+           from myproject.views.frontend import frontend
+           app.register_blueprint(admin)
+           app.register_blueprint(frontend)
+
+            return app
+
+    See the parameters for a more detailed list of optional features when
+    initializing the extension.
+
+    :param app: The Flask app that this Dockerflow extension should be
+                initialized with.
+    :type app: ~flask.Flask or None
+
+    :param db: A Flask-SQLAlchemy extension instance to be used by the
+               built-in Dockerflow check for the database connection.
+    :param redis: A Redis connection to be used by the built-in Dockerflow
+                  check for the Redis connection.
+    :param migrate: A Flask-Migrate extension instance to be used by the
+                    built-in Dockerflow check for Alembic migrations.
+    :param silenced_checks: Dockerflow check IDs to ignore when running
+                            through the list of configured checks.
+    :type silenced_checks: list
+
+    :param version_path: The filesystem path where the ``version.json`` can
+                         be found. Defaults to the parent directory of the
+                         Flask app's root path.
+    """
+
+    def __init__(
+        self,
+        app=None,
+        db=None,
+        redis=None,
+        migrate=None,
+        silenced_checks=None,
+        version_path=None,
+        *args,
+        **kwargs,
+    ):
+        # The Flask blueprint to add the Dockerflow signal callbacks and views
+        self._blueprint = flask.Blueprint("dockerflow", "dockerflow.flask.app")
+
+        # The Dockerflow specific logger to be used by internals of this
+        # extension.
+        self.logger = logging.getLogger("dockerflow.flask")
+        self.logger.addHandler(logging.NullHandler())
+        self.logger.setLevel(logging.INFO)
+
+        # The request summary logger to be used by this extension
+        # without pre-configuration. See docs for how to set it up.
+        self.summary_logger = logging.getLogger("request.summary")
+
+        # A list of IDs of custom Dockerflow checks to ignore in case they
+        # show up.
+        self.silenced_checks = silenced_checks or []
+
+        # The path where to find the version JSON file. Defaults to the
+        # parent directory of the app root path.
+        self.version_path = version_path
+        self._version_callback = version.get_version
+
+        # Initialize the app if given.
+        if app:
+            self.init_app(app)
+        # Initialize the built-in checks.
+        if db:
+            checks.register_partial(check_database_connected, db)
+        if redis:
+            checks.register_partial(check_redis_connected, redis)
+        if migrate:
+            checks.register_partial(check_migrations_applied, migrate)
+
+    def init_app(self, app):
+        """
+        Initializes the extension with the given app, registers the
+        built-in views with an own blueprint and hooks up our signal
+        callbacks.
+        """
+        # If no version path was provided in the init of the Dockerflow
+        # class we'll use the parent directory of the app root path.
+        if self.version_path is None:
+            self.version_path = os.path.dirname(app.root_path)
+
+        for view in (
+            ("/__version__", "version", self._version_view),
+            ("/__heartbeat__", "heartbeat", self._heartbeat_view),
+            ("/__lbheartbeat__", "lbheartbeat", self._lbheartbeat_view),
+        ):
+            self._blueprint.add_url_rule(*view)
+        self._blueprint.before_app_request(self._before_request)
+        self._blueprint.after_app_request(self._after_request)
+        self._blueprint.app_errorhandler(HeartbeatFailure)(
+            self._heartbeat_exception_handler
+        )
+        app.register_blueprint(self._blueprint)
+        flask.got_request_exception.connect(self._got_request_exception, sender=app)
+
+        if not hasattr(app, "extensions"):  # pragma: nocover
+            app.extensions = {}
+        app.extensions["dockerflow"] = self
+
+    def _heartbeat_exception_handler(self, error):
+        """
+        An exception handler to act as a middleman to return
+        a heartbeat view response with a 500 error code.
+        """
+        return error.get_response()
+
+    def _before_request(self):
+        """
+        The before_request callback.
+        """
+        extract_request_id(flask.request)
+        flask.g._start_timestamp = time.time()
+
+    def _after_request(self, response):
+        """
+        The signal handler for the request_finished signal.
+        """
+        if not getattr(flask.g, "_has_exception", False):
+            extra = self.summary_extra()
+            self.summary_logger.info("", extra=extra)
+        return response
+
+    def _got_request_exception(self, sender, exception, **extra):
+        """
+        The signal handler for the got_request_exception signal.
+        """
+        extra = self.summary_extra()
+        extra["errno"] = 500
+        self.summary_logger.error(str(exception), extra=extra)
+        flask.g._has_exception = True
+
+    def user_id(self):
+        """
+        Return the ID of the current request's user
+        """
+        # This needs flask-login to be installed
+        if not has_flask_login:
+            return
+
+        # and the actual login manager installed
+        if not hasattr(flask.current_app, "login_manager"):
+            return
+
+        # fail if no current_user was attached to the request context
+        try:
+            is_authenticated = current_user.is_authenticated
+        except AttributeError:
+            return
+
+        # because is_authenticated could be a callable, call it
+        if callable(is_authenticated):
+            is_authenticated = is_authenticated()
+
+        # and fail if the user isn't authenticated
+        if not is_authenticated:
+            return
+
+        # finally return the user id
+        try:
+            return current_user.get_id()
+        except UserLoadingError:
+            # but don't fail if for some reason getting the user id
+            # created an exception to not accidently make exception
+            # handling worse. If sqlalchemy is used that catches
+            # all SQLAlchemyError exceptions.
+            pass
+
+    def summary_extra(self):
+        """
+        Build the extra data for the summary logger.
+        """
+        out = {
+            "errno": 0,
+            "agent": flask.request.headers.get("User-Agent", ""),
+            "lang": flask.request.headers.get("Accept-Language", ""),
+            "method": flask.request.method,
+            "path": flask.request.path,
         }
-    })
-
-    sanic = Sanic(__name__, log_config=log)
-
-By default the ``log_info`` parameter has the value of
-``sanic.log.LOGGING_CONFIG_DEFAULTS``.
-
-Alternatively you can also pass the same logging config dictionary to the
-``logging.conf.dictConfig`` utility **BEFORE** your Sanic app is initialized::
-
-    from logging.conf import dictConfig
-    from sanic import Sanic
-
-    log_config = {
-        # ...
-    }
-
-    dictConfig(log_config)
-
-    sanic = Sanic(__name__)
-
-In order to include querystrings in the request summary log, set this flag in :ref:`configuration <sanic-config>`::
 
-    DOCKERFLOW_SUMMARY_LOG_QUERYSTRING = True
+        if flask.current_app.config.get("DOCKERFLOW_SUMMARY_LOG_QUERYSTRING", False):
+            out["querystring"] = flask.request.query_string.decode()
 
+        # set the uid value to the current user ID
+        user_id = self.user_id()
+        if user_id is None:
+            user_id = ""
+        out["uid"] = user_id
+
+        # the rid value to the current request ID
+        out["rid"] = request_id_context.get()
+
+        # and the t value to the time it took to render
+        start_timestamp = flask.g.get("_start_timestamp", None)
+        if start_timestamp is not None:
+            # Duration of request, in milliseconds.
+            out["t"] = int(1000 * (time.time() - start_timestamp))
+
+        return out
+
+    def _version_view(self):
+        """
+        View that returns the contents of version.json or a 404.
+        """
+        version_json = self._version_callback(self.version_path)
+        if version_json is None:
+            return "version.json not found", 404
+        else:
+            return flask.jsonify(version_json)
+
+    def _lbheartbeat_view(self):
+        """
+        Lets the load balancer know the application is running and available.
+        Must return 200 (not 204) for ELB
+        http://docs.aws.amazon.com/ElasticLoadBalancing/latest/DeveloperGuide/elb-healthchecks.html
+        """
+        return "", 200
+
+    def _heartbeat_view(self):
+        """
+        Runs all the registered checks and returns a JSON response with either
+        a status code of 200 or 500 depending on the results of the checks.
+
+        Any check that returns an error or worse (critical) will return
+        a 500 response.
+        """
+        FAILED_STATUS_CODE = int(
+            flask.current_app.config.get(
+                "DOCKERFLOW_HEARTBEAT_FAILED_STATUS_CODE", "500"
+            )
+        )
+
+        check_results = checks.run_checks(
+            checks.get_checks().items(),
+            silenced_check_ids=self.silenced_checks,
+        )
+
+        payload = {
+            "status": checks.level_to_text(check_results.level),
+            "checks": check_results.statuses,
+            "details": check_results.details,
+        }
 
-MozLog App-Specific Fields
-~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-The *MozLog* formatter will output ``Fields`` application-specific fields. It can be populated through the ``extra`` parameter:
-
-.. code-block:: python
-
-    logger.info(
-        "Subsystem %s running at %s:%s",
-        name, host, port,
-        extra={"phase": "started", "host": host, "port": port}
-    )
-
-
-Requests Correlation ID
-~~~~~~~~~~~~~~~~~~~~~~~
-
-A unique request ID is read from the ``X-Request-ID`` request header, and a UUID4 value is generated if unset.
-
-Leveraging the ``RequestIdFilter`` in logging configuration as shown above will add a ``rid`` field into the ``Fields`` entry of all log messages.
-
-The header name to obtain the request ID can be customized in settings:
-
-.. code-block:: python
-
-    DOCKERFLOW_REQUEST_ID_HEADER_NAME = "X-Cloud-Trace-Context"
-
-
-.. _sanic-static:
-
-Static content
---------------
-
-Please refer to the Sanic documentation about `serving static files`_ for more
-information.
+        def render(status_code):
+            return flask.make_response(flask.jsonify(payload), status_code)
 
-.. _serving static files: https://sanic.dev/en/guide/basics/routing.html#static-files
+        if check_results.level < checks.ERROR:
+            status_code = 200
+            heartbeat_passed.send(self, level=check_results.level)
+            return render(status_code)
+        else:
+            status_code = FAILED_STATUS_CODE
+            heartbeat_failed.send(self, level=check_results.level)
+            raise HeartbeatFailure(response=render(status_code))
+
+    def version_callback(self, func):
+        """
+        A decorator to optionally register a new Dockerflow version callback
+        and use that instead of the default of
+        :func:`dockerflow.version.get_version`.
+
+        The callback will be passed the value of the
+        ``version_path`` parameter to the Dockerflow extension object,
+        which defaults to the parent directory of the Flask app's root path.
+
+        The callback should return a dictionary with the
+        version information as defined in the Dockerflow spec,
+        or None if no version information could be loaded.
+
+        E.g.::
+
+            app = Flask(__name__)
+            dockerflow = Dockerflow(app)
+
+            @dockerflow.version_callback
+            def my_version(root):
+                return json.loads(os.path.join(root, 'acme_version.json'))
+
+        """
+        self._version_callback = func
+
+    @property
+    def checks(self):
+        """
+        Backwards compatibility alias.
+        """
+        message = (
+            "`dockerflow.checks` is deprecated, use `checks.get_checks()` instead."
+        )
+        warnings.warn(message, DeprecationWarning)
+        return checks.get_checks()
+
+    def init_check(self, check, obj):
+        """
+        Backwards compatibility method.
+        """
+        message = "`dockerflow.init_check()` is deprecated, use `checks.register_partial()` instead."
+        warnings.warn(message, DeprecationWarning)
+        return checks.register_partial(check, obj)
+
+    def check(self, func=None, name=None):
+        """
+        Backwards compatibility method.
+        """
+        message = "`dockerflow.check()` is deprecated, use `checks.register()` instead."
+        warnings.warn(message, DeprecationWarning)
+        return checks.register(func, name)
```

### Comparing `dockerflow-2024.4.1/setup.py` & `dockerflow-2024.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/src/dockerflow/checks/__init__.py` & `dockerflow-2024.4.2/src/dockerflow/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/src/dockerflow/checks/messages.py` & `dockerflow-2024.4.2/src/dockerflow/checks/messages.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/src/dockerflow/checks/registry.py` & `dockerflow-2024.4.2/src/dockerflow/checks/registry.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,41 +13,28 @@
 logger = logging.getLogger(__name__)
 
 CheckFn = Callable[..., List[CheckMessage]]
 
 _REGISTERED_CHECKS = {}
 
 
-def _iscoroutinefunction_or_partial(obj):
-    """
-    Determine if the provided object is a coroutine function or a partial function
-    that wraps a coroutine function.
-
-    This function should be removed when we drop support for Python 3.7, as this is
-    handled directly by `inspect.iscoroutinefunction` in Python 3.8.
-    """
-    while isinstance(obj, functools.partial):
-        obj = obj.func
-    return inspect.iscoroutinefunction(obj)
-
-
 def register(func=None, name=None):
     """
     Register a check callback to be executed from
     the heartbeat endpoint.
     """
     if func is None:
         return functools.partial(register, name=name)
 
     if name is None:
         name = func.__name__
 
     logger.debug("Register Dockerflow check %s", name)
 
-    if _iscoroutinefunction_or_partial(func):
+    if inspect.iscoroutinefunction(func):
 
         @functools.wraps(func)
         async def decorated_function_asyc(*args, **kwargs):
             logger.debug("Called Dockerflow check %s", name)
             return await func(*args, **kwargs)
 
         _REGISTERED_CHECKS[name] = decorated_function_asyc
@@ -112,15 +99,15 @@
     details: Dict[str, Dict[str, Any]]
     statuses: Dict[str, str]
     level: int
 
 
 async def _run_check_async(check):
     name, check_fn = check
-    if _iscoroutinefunction_or_partial(check_fn):
+    if inspect.iscoroutinefunction(check_fn):
         errors = await check_fn()
     else:
         loop = asyncio.get_event_loop()
         errors = await loop.run_in_executor(None, check_fn)
 
     return (name, errors)
```

### Comparing `dockerflow-2024.4.1/src/dockerflow/django/checks.py` & `dockerflow-2024.4.2/src/dockerflow/django/checks.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/src/dockerflow/django/middleware.py` & `dockerflow-2024.4.2/src/dockerflow/django/middleware.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/src/dockerflow/django/signals.py` & `dockerflow-2024.4.2/src/dockerflow/django/signals.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/src/dockerflow/django/views.py` & `dockerflow-2024.4.2/src/dockerflow/django/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,16 +46,16 @@
 
 
 def heartbeat(request):
     """
     Runs all the Django checks and returns a JsonResponse with either
     a status code of 200 or 500 depending on the results of the checks.
 
-    Any check that returns a warning or worse (error, critical) will
-    return a 500 response.
+    Any check that returns an error or worse (critical) will return
+    a 500 response.
     """
     checks_to_run = (
         (check.__name__, lambda: check(app_configs=None))
         for check in django_check_registry.get_checks(
             include_deployment_checks=not settings.DEBUG
         )
     )
```

### Comparing `dockerflow-2024.4.1/src/dockerflow/fastapi/middleware.py` & `dockerflow-2024.4.2/src/dockerflow/fastapi/middleware.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/src/dockerflow/fastapi/views.py` & `dockerflow-2024.4.2/src/dockerflow/fastapi/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 from ..version import get_version
 
 
 def lbheartbeat():
     return {"status": "ok"}
 
 
-def heartbeat(request: Request, response: Response):
+async def heartbeat(request: Request, response: Response):
     FAILED_STATUS_CODE = int(
         getattr(request.app.state, "DOCKERFLOW_HEARTBEAT_FAILED_STATUS_CODE", "500")
     )
 
-    check_results = checks.run_checks(
+    check_results = await checks.run_checks_async(
         checks.get_checks().items(),
     )
 
     payload = {
         "status": checks.level_to_text(check_results.level),
         "checks": check_results.statuses,
         "details": check_results.details,
```

### Comparing `dockerflow-2024.4.1/src/dockerflow/flask/checks/__init__.py` & `dockerflow-2024.4.2/src/dockerflow/flask/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/src/dockerflow/flask/signals.py` & `dockerflow-2024.4.2/src/dockerflow/flask/signals.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/src/dockerflow/health.py` & `dockerflow-2024.4.2/src/dockerflow/health.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/src/dockerflow/logging.py` & `dockerflow-2024.4.2/src/dockerflow/logging.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/src/dockerflow/sanic/app.py` & `dockerflow-2024.4.2/src/dockerflow/sanic/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,16 +209,16 @@
         return response.raw(b"", 200)
 
     async def _heartbeat_view(self, request):
         """
         Runs all the registered checks and returns a JSON response with either
         a status code of 200 or 500 depending on the results of the checks.
 
-        Any check that returns a warning or worse (error, critical) will
-        return a 500 response.
+        Any check that returns an error or worse (critical) will return
+        a 500 response.
         """
         FAILED_STATUS_CODE = int(
             request.app.config.get("DOCKERFLOW_HEARTBEAT_FAILED_STATUS_CODE", "500")
         )
 
         check_results = await checks.run_checks_async(
             checks.get_checks().items(),
```

### Comparing `dockerflow-2024.4.1/src/dockerflow/sanic/checks.py` & `dockerflow-2024.4.2/src/dockerflow/sanic/checks.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/src/dockerflow/version.py` & `dockerflow-2024.4.2/src/dockerflow/version.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/src/dockerflow.egg-info/PKG-INFO` & `dockerflow-2024.4.2/src/dockerflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dockerflow
-Version: 2024.4.1
+Version: 2024.4.2
 Summary: Python tools and helpers for Mozilla's Dockerflow
 Home-page: https://github.com/mozilla-services/python-dockerflow
 Author: Mozilla Foundation
 Author-email: dev-webdev@lists.mozilla.org
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment :: Mozilla
```

### Comparing `dockerflow-2024.4.1/src/dockerflow.egg-info/SOURCES.txt` & `dockerflow-2024.4.2/src/dockerflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/tests/conftest.py` & `dockerflow-2024.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/tests/core/test_checks.py` & `dockerflow-2024.4.2/tests/core/test_checks.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/tests/core/test_logging.py` & `dockerflow-2024.4.2/tests/core/test_logging.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/tests/core/test_version.py` & `dockerflow-2024.4.2/tests/core/test_version.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/tests/django/settings.py` & `dockerflow-2024.4.2/tests/django/settings.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/tests/django/test_django.py` & `dockerflow-2024.4.2/tests/django/test_django.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/tests/fastapi/test_fastapi.py` & `dockerflow-2024.4.2/tests/fastapi/test_fastapi.py`

 * *Files 24% similar despite different names*

```diff
@@ -190,14 +190,61 @@
                 "level": 40,
                 "messages": {"foo": "BOOM"},
                 "status": "error",
             }
         },
     }
 
+def test_heartbeat_sync(client):
+    @checks.register
+    def sync_ok():
+        return []
+
+    response = client.get("/__heartbeat__")
+    assert response.status_code == 200
+    assert response.json() == {
+        "status": "ok",
+        "checks": {"sync_ok": "ok"},
+        "details": {},
+    }
+
+
+def test_heartbeat_async(client):
+    @checks.register
+    async def async_ok():
+        return []
+
+    response = client.get("/__heartbeat__")
+    assert response.status_code == 200
+    assert response.json() == {
+        "status": "ok",
+        "checks": {"async_ok": "ok"},
+        "details": {},
+    }
+
+
+def test_heartbeat_mixed_sync(client):
+    @checks.register
+    def sync_ok():
+        return []
+    @checks.register
+    async def async_ok():
+        return []
+
+    response = client.get("/__heartbeat__")
+    assert response.status_code == 200
+    assert response.json() == {
+        "status": "ok",
+        "checks": {
+            "sync_ok": "ok",
+            "async_ok": "ok",
+        },
+        "details": {},
+    }
+
 
 def test_heartbeat_head(client):
     @checks.register
     def return_sucess():
         return [checks.Info("Nice", id="foo")]
 
     response = client.head("/__heartbeat__")
```

### Comparing `dockerflow-2024.4.1/tests/flask/migrations/alembic.ini` & `dockerflow-2024.4.2/tests/flask/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/tests/flask/migrations/env.py` & `dockerflow-2024.4.2/tests/flask/migrations/env.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/tests/flask/test_flask.py` & `dockerflow-2024.4.2/tests/flask/test_flask.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/tests/sanic/test_sanic.py` & `dockerflow-2024.4.2/tests/sanic/test_sanic.py`

 * *Files identical despite different names*

### Comparing `dockerflow-2024.4.1/tox.ini` & `dockerflow-2024.4.2/tox.ini`

 * *Files identical despite different names*

