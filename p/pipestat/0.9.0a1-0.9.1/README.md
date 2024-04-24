# Comparing `tmp/pipestat-0.9.0a1.tar.gz` & `tmp/pipestat-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipestat-0.9.0a1.tar", last modified: Thu Apr  4 17:46:46 2024, max compression
+gzip compressed data, was "pipestat-0.9.1.tar", last modified: Wed Apr 24 21:22:30 2024, max compression
```

## Comparing `pipestat-0.9.0a1.tar` & `pipestat-0.9.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.075006 pipestat-0.9.0a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-04 17:46:46.075006 pipestat-0.9.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.067005 pipestat-0.9.0a1/pipestat/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11512 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.067005 pipestat-0.9.0a1/pipestat/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/backends/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.067005 pipestat-0.9.0a1/pipestat/backends/db_backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/backends/db_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/backends/db_backend/db_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/backends/db_backend/db_parsed_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    21016 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/backends/db_backend/dbbackend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.067005 pipestat-0.9.0a1/pipestat/backends/file_backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/backends/file_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30130 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/backends/file_backend/filebackend.py
--rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.071005 pipestat-0.9.0a1/pipestat/jinja_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/footer_index.html
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/glossary.html
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/glossary_table.html
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/head.html
--rw-r--r--   0 runner    (1001) docker     (127)    10727 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/logo.html
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/navbar.html
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/navbar_links.html
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/navbar_list_parent.html
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/object.html
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/project_object.html
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/sample.html
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/status.html
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/status_table.html
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/status_table_no_links.html
--rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/parsed_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    37635 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/pipestat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.071005 pipestat-0.9.0a1/pipestat/pipestatreader/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/pipestatreader/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/pipestatreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/pipestatreader/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    58267 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/reports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.071005 pipestat-0.9.0a1/pipestat/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/schemas/pipestat_config_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/schemas/status_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/schemas/status_table_schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.075006 pipestat-0.9.0a1/pipestat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-04 17:46:46.000000 pipestat-0.9.0a1/pipestat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-04 17:46:46.000000 pipestat-0.9.0a1/pipestat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 17:46:46.000000 pipestat-0.9.0a1/pipestat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-04 17:46:46.000000 pipestat-0.9.0a1/pipestat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-04 17:46:46.000000 pipestat-0.9.0a1/pipestat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 17:46:46.000000 pipestat-0.9.0a1/pipestat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.075006 pipestat-0.9.0a1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/requirements/requirements-db-backend.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/requirements/requirements-pipestatreader.txt
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 17:46:46.075006 pipestat-0.9.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.075006 pipestat-0.9.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/tests/test_db_only_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/tests/test_parsed_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    87713 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/tests/test_pipestat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/tests/test_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:22:30.703644 pipestat-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-24 21:22:19.000000 pipestat-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-24 21:22:19.000000 pipestat-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-24 21:22:30.703644 pipestat-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-24 21:22:19.000000 pipestat-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:22:30.691644 pipestat-0.9.1/pipestat/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11918 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:22:30.695644 pipestat-0.9.1/pipestat/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/backends/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:22:30.695644 pipestat-0.9.1/pipestat/backends/db_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/backends/db_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/backends/db_backend/db_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14287 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/backends/db_backend/db_parsed_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27351 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/backends/db_backend/dbbackend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:22:30.695644 pipestat-0.9.1/pipestat/backends/file_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/backends/file_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32471 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/backends/file_backend/filebackend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:22:30.699644 pipestat-0.9.1/pipestat/jinja_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/jinja_templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/jinja_templates/footer_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/jinja_templates/glossary.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/jinja_templates/glossary_table.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/jinja_templates/head.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10734 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/jinja_templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/jinja_templates/logo.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/jinja_templates/navbar.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/jinja_templates/navbar_links.html
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/jinja_templates/navbar_list_parent.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/jinja_templates/object.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/jinja_templates/project_object.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/jinja_templates/sample.html
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/jinja_templates/status.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/jinja_templates/status_table.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/jinja_templates/status_table_no_links.html
+-rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/parsed_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40606 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/pipestat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:22:30.699644 pipestat-0.9.1/pipestat/pipestatreader/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/pipestatreader/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/pipestatreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/pipestatreader/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58737 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/reports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:22:30.699644 pipestat-0.9.1/pipestat/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/schemas/pipestat_config_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/schemas/status_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-24 21:22:19.000000 pipestat-0.9.1/pipestat/schemas/status_table_schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:22:30.699644 pipestat-0.9.1/pipestat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-24 21:22:30.000000 pipestat-0.9.1/pipestat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-24 21:22:30.000000 pipestat-0.9.1/pipestat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 21:22:30.000000 pipestat-0.9.1/pipestat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-24 21:22:30.000000 pipestat-0.9.1/pipestat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-24 21:22:30.000000 pipestat-0.9.1/pipestat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 21:22:30.000000 pipestat-0.9.1/pipestat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-24 21:22:19.000000 pipestat-0.9.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:22:30.699644 pipestat-0.9.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-24 21:22:19.000000 pipestat-0.9.1/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 21:22:19.000000 pipestat-0.9.1/requirements/requirements-db-backend.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 21:22:19.000000 pipestat-0.9.1/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-24 21:22:19.000000 pipestat-0.9.1/requirements/requirements-pipestatreader.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-24 21:22:19.000000 pipestat-0.9.1/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 21:22:30.703644 pipestat-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-24 21:22:19.000000 pipestat-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 21:22:30.699644 pipestat-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-24 21:22:19.000000 pipestat-0.9.1/tests/test_db_only_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-24 21:22:19.000000 pipestat-0.9.1/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-04-24 21:22:19.000000 pipestat-0.9.1/tests/test_parsed_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92283 2024-04-24 21:22:19.000000 pipestat-0.9.1/tests/test_pipestat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-24 21:22:19.000000 pipestat-0.9.1/tests/test_status.py
```

### Comparing `pipestat-0.9.0a1/LICENSE` & `pipestat-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0a1/PKG-INFO` & `pipestat-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipestat
-Version: 0.9.0a1
+Version: 0.9.1
 Summary: A pipeline results reporter
 Home-page: https://github.com/pepkit/pipestat
 Author: Michal Stolarczyk, Nathan Sheffield
 License: BSD2
 Keywords: project,metadata,bioinformatics,sequencing,ngs,workflow
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pipestat-0.9.0a1/README.md` & `pipestat-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0a1/pipestat/argparser.py` & `pipestat-0.9.1/pipestat/argparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from .const import ENV_VARS, PKG_NAME, STATUS_SCHEMA
 
 REPORT_CMD = "report"
 INSPECT_CMD = "inspect"
 REMOVE_CMD = "remove"
 RETRIEVE_CMD = "retrieve"
+HISTORY_CMD = "history"
 STATUS_CMD = "status"
 INIT_CMD = "init"
 SUMMARIZE_CMD = "summarize"
 LINK_CMD = "link"
 SERVE_CMD = "serve"
 SUBPARSER_MESSAGES = {
     REPORT_CMD: "Report a result.",
@@ -22,14 +23,15 @@
     REMOVE_CMD: "Remove a result.",
     RETRIEVE_CMD: "Retrieve a result.",
     STATUS_CMD: "Manage pipeline status.",
     INIT_CMD: "Initialize generic config file",
     SUMMARIZE_CMD: "Generates HTML Report",
     LINK_CMD: "Create symlinks of reported files",
     SERVE_CMD: "Initializes pipestatreader API",
+    HISTORY_CMD: "Retrieve history of reported results for one record identifier",
 }
 
 STATUS_GET_CMD = "get"
 STATUS_SET_CMD = "set"
 STATUS_SUBPARSER_MESSAGES = {
     STATUS_SET_CMD: "Set status.",
     STATUS_GET_CMD: "Get status.",
@@ -165,15 +167,15 @@
             "--pipeline-type",
             type=str,
             metavar="P",
             help="project or sample level pipeline type. ",
         )
 
     # remove, report and inspect
-    for cmd in [REMOVE_CMD, REPORT_CMD, INSPECT_CMD, RETRIEVE_CMD]:
+    for cmd in [REMOVE_CMD, REPORT_CMD, INSPECT_CMD, RETRIEVE_CMD, HISTORY_CMD]:
         sps[cmd].add_argument(
             "-f",
             "--results-file",
             type=str,
             metavar="F",
             help=f"Path to the YAML file where the results will be stored. "
             f"This file will be used as {PKG_NAME} backend and to restore"
@@ -235,21 +237,29 @@
             "-r",
             "--record-identifier",
             type=str,
             metavar="R",
             help=f"ID of the record to report the result for. {_env_txt('record_identifier')}",
         )
 
-    sps[RETRIEVE_CMD].add_argument(
-        "-r",
-        "--record-identifier",
-        type=str,
-        metavar="R",
-        help=f"ID of the record to report the result for. {_env_txt('record_identifier')}",
-    )
+    for cmd in [RETRIEVE_CMD, HISTORY_CMD]:
+        sps[cmd].add_argument(
+            "-i",
+            "--result-identifier",
+            type=str,
+            metavar="I",
+            help="ID of the result to report; needs to be defined in the schema",
+        )
+        sps[cmd].add_argument(
+            "-r",
+            "--record-identifier",
+            type=str,
+            metavar="R",
+            help=f"ID of the record to report the result for. {_env_txt('record_identifier')}",
+        )
 
     # report
     sps[REPORT_CMD].add_argument(
         "-v",
         "--value",
         required=True,
         metavar="V",
```

### Comparing `pipestat-0.9.0a1/pipestat/backends/abstract.py` & `pipestat-0.9.1/pipestat/backends/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,15 @@
 
     def report(
         self,
         values: Dict[str, Any],
         record_identifier: str,
         force_overwrite: bool = False,
         result_formatter: Optional[staticmethod] = None,
+        history_enabled: bool = True,
     ) -> str:
         _LOGGER.warning("Not implemented yet for this backend")
 
     def retrieve_distinct(
         self,
         columns: Optional[List[str]] = None,
     ) -> List[Any]:
```

### Comparing `pipestat-0.9.0a1/pipestat/backends/db_backend/db_helpers.py` & `pipestat-0.9.1/pipestat/backends/db_backend/db_helpers.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0a1/pipestat/backends/db_backend/db_parsed_schema.py` & `pipestat-0.9.1/pipestat/backends/db_backend/db_parsed_schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -192,14 +192,57 @@
         # return ARRAY if t == list else t
         return t
 
     @property
     def file_like_table_name(self):
         return self._table_name("files")
 
+    def build_history_model(self, pipeline_type):
+        """Creates model for history ORM
+        :param str pipeline_type: project or sample-level pipeline
+        :return model: (model, table_name)
+        """
+        if pipeline_type == "project":
+            history_table_name = self.project_table_name + "_history"
+            data = self.project_level_data
+            main_table_id = self.project_table_name + ".id"
+
+        elif pipeline_type == "sample":
+            history_table_name = self.sample_table_name + "_history"
+            data = self.sample_level_data
+            main_table_id = self.sample_table_name + ".id"
+
+        else:
+            raise PipestatError(
+                f"Building model requires pipeline type. Provided type: '{pipeline_type}' "
+            )
+
+        if not self.sample_level_data and not self.project_level_data:
+            return None
+
+        field_defs = self._make_field_definitions(data, require_type=True)
+        field_defs = self._add_status_field(field_defs)
+        field_defs = self._add_record_identifier_field(field_defs)
+        field_defs = self._add_id_field(field_defs)
+        field_defs = self._add_pipeline_name_field(field_defs)
+        field_defs = self._add_created_time_field(field_defs)
+        field_defs = self._add_modified_time_field(field_defs)
+
+        field_defs["source_record_id"] = (
+            int,
+            Field(
+                default=None,
+                foreign_key=main_table_id,
+            ),
+        )
+
+        history_model = _create_model(history_table_name, **field_defs)
+
+        return history_model, history_table_name
+
     def build_model(self, pipeline_type):
         if pipeline_type == "project":
             data = self.project_level_data
             # if using the same output schema and thus, pipeline name for samples and project
             # we must ensure there are distinct table names in the same database.
             table_name = self.project_table_name
```

### Comparing `pipestat-0.9.0a1/pipestat/backends/db_backend/dbbackend.py` & `pipestat-0.9.1/pipestat/backends/db_backend/dbbackend.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import datetime
 from logging import getLogger
 from contextlib import contextmanager
 from typing import List, Dict, Any, Optional, Union, NoReturn, Tuple
 
 from sqlmodel import SQLModel, Session, create_engine, select as sql_select
 
@@ -58,14 +59,16 @@
         self.status_schema = status_schema
         self.db_url = db_url
         self.show_db_logs = show_db_logs
         self.status_schema_source = status_schema_source
         self.result_formatter = result_formatter
 
         self.orms = self._create_orms(pipeline_type=pipeline_type)
+        self.history_table = self._create_history_orms(pipeline_type=pipeline_type)
+
         self.table_name = list(self.orms.keys())[0]
         SQLModel.metadata.create_all(self._engine)
 
     def check_record_exists(
         self,
         record_identifier: str,
     ) -> bool:
@@ -270,25 +273,43 @@
         :raises RecordNotFoundError: if record not found
         """
 
         record_identifier = record_identifier or self.record_identifier
         if rm_record:
             try:
                 ORMClass = self.get_model(table_name=self.table_name)
+                ORMClass_History = self.history_table[list(self.history_table.keys())[0]]
                 if self.check_record_exists(
                     record_identifier=record_identifier,
                 ):
                     with self.session as s:
+                        source_record_id = (
+                            s.exec(
+                                sql_select(ORMClass).where(
+                                    getattr(ORMClass, RECORD_IDENTIFIER) == record_identifier
+                                )
+                            )
+                            .first()
+                            .id
+                        )
+                        linked_records = s.exec(
+                            sql_select(ORMClass_History).where(
+                                getattr(ORMClass_History, "source_record_id") == source_record_id
+                            )
+                        ).all()
+                        for r in linked_records:
+                            s.delete(r)
+                        s.commit()
+                    with self.session as s:
                         record = s.exec(
                             sql_select(ORMClass).where(
                                 getattr(ORMClass, "record_identifier") == record_identifier
                             )
                         ).first()
                         s.delete(record)
-
                         s.commit()
                 else:
                     raise RecordNotFoundError(f"Record '{record_identifier}' not found")
             except Exception as e:
                 _LOGGER.error(f"Could not remove the result from the database. Exception: {e}")
                 raise
         else:
@@ -296,14 +317,15 @@
 
     def report(
         self,
         values: Dict[str, Any],
         record_identifier: str,
         force_overwrite: bool = True,
         result_formatter: Optional[staticmethod] = None,
+        history_enabled: bool = True,
     ) -> Union[List[str], bool]:
         """
         Update the value of a result in a current namespace.
 
         This method overwrites any existing data and creates the required
          hierarchical mapping structure if needed.
 
@@ -333,14 +355,15 @@
             _LOGGER.warning(f"These results exist for '{record_identifier}': {existing_str}")
             if not force_overwrite:
                 return False
             _LOGGER.info(f"Overwriting existing results: {existing_str}")
 
         try:
             ORMClass = self.get_model(table_name=self.table_name)
+            ORMClass_History = self.history_table[list(self.history_table.keys())[0]]
             values.update({RECORD_IDENTIFIER: record_identifier})
 
             if not self.check_record_exists(
                 record_identifier=record_identifier,
             ):
                 current_time = datetime.datetime.now()
                 values.update({CREATED_TIME: current_time})
@@ -352,19 +375,32 @@
             else:
                 with self.session as s:
                     record_to_update = s.exec(
                         sql_select(ORMClass).where(
                             getattr(ORMClass, RECORD_IDENTIFIER) == record_identifier
                         )
                     ).first()
-
+                    old_record_attributes = record_to_update.model_dump()
                     values.update({MODIFIED_TIME: datetime.datetime.now()})
                     for result_id, result_value in values.items():
                         setattr(record_to_update, result_id, result_value)
                     s.commit()
+                if history_enabled:
+                    if "id" in old_record_attributes:
+                        del old_record_attributes["id"]
+                    with self.session as s:
+                        source_record = s.exec(
+                            sql_select(ORMClass).where(
+                                getattr(ORMClass, RECORD_IDENTIFIER) == record_identifier
+                            )
+                        ).first()
+                        new_record_history = ORMClass_History(**old_record_attributes)
+                        new_record_history.source_record_id = source_record.id
+                        s.add(new_record_history)
+                        s.commit()
 
             for res_id, val in values.items():
                 results_formatted.append(
                     result_formatter(
                         pipeline_name=self.pipeline_name,
                         record_identifier=record_identifier,
                         res_id=res_id,
@@ -407,17 +443,18 @@
 
         ORM = self.get_model(table_name=self.table_name)
 
         with self.session as s:
             total_count = len(s.exec(sql_select(ORM)).all())
 
             if columns is not None:
+                columns = copy.deepcopy(columns)
                 for i in ["id", "record_identifier"]:  # Must add id, need it for cursor
                     if i not in columns:
-                        columns = [i] + columns
+                        columns.insert(0, i)
                 try:
                     statement = sql_select(*[getattr(ORM, column) for column in columns]).order_by(
                         ORM.id
                     )
                 except AttributeError:
                     raise ColumnNotFoundError(
                         msg=f"One of the supplied columns does not exist in current table: {columns}"
@@ -463,14 +500,113 @@
             "page_size": limit,
             "next_page_token": next_cursor,
             "records": end_results,
         }
 
         return records_dict
 
+    def retrieve_history_db(
+        self,
+        record_identifier: str,
+        result_identifier: Optional[Union[str, List[str]]] = None,
+    ) -> Dict[str, Any]:
+        """
+
+        :param record_identifier: single record_identifier
+        :param result_identifier: single or list of result identifiers
+        :return: dict records_dict = {
+            "history": List[Dict[{key, Any}]],
+        }
+        """
+
+        record_identifier = record_identifier or self.record_identifier
+
+        ORMClass = self.get_model(table_name=self.table_name)
+        ORMClass_History = self.history_table[list(self.history_table.keys())[0]]
+
+        if not result_identifier:
+            columns = None
+        else:
+            if isinstance(result_identifier, str):
+                columns = [result_identifier]
+            elif isinstance(result_identifier, list):
+                columns = copy.deepcopy(result_identifier)
+            else:
+                raise ValueError("Result identifier must be a str or list[str]")
+            for i in ["id", MODIFIED_TIME]:
+                if i not in columns:
+                    columns.insert(0, i)
+
+        if not self.check_record_exists(
+            record_identifier=record_identifier,
+        ):
+            raise RecordNotFoundError(f"{record_identifier} does not exist.")
+        else:
+            with self.session as s:
+                source_record_id = (
+                    s.exec(
+                        sql_select(ORMClass).where(
+                            getattr(ORMClass, RECORD_IDENTIFIER) == record_identifier
+                        )
+                    )
+                    .first()
+                    .id
+                )
+                if columns is not None:
+                    try:
+                        statement = sql_select(
+                            *[getattr(ORMClass_History, column) for column in columns]
+                        ).order_by(ORMClass_History.id)
+                    except AttributeError:
+                        raise ColumnNotFoundError(
+                            msg=f"One of the supplied columns does not exist in current table: {columns}"
+                        )
+                else:
+                    statement = sql_select(ORMClass_History).order_by(ORMClass_History.id)
+
+                statement = statement.where(
+                    getattr(ORMClass_History, "source_record_id") == source_record_id
+                )
+
+                history_records = s.exec(statement).all()
+
+        end_results = []
+
+        # SQL model returns either a SQLModelMetaCLass OR a sqlalchemy Row.
+        # We must create a dictionary containing the record before returning
+
+        if not columns:
+            end_results = [r.model_dump() for r in history_records]
+
+        else:
+            for record in history_records:
+                record_dict = dict(record._mapping)
+                end_results.append(record_dict)
+
+        # This next step is to process the results such that they will match output similar to the filebackend
+
+        collected_keys = []
+        new_history_dict = {}
+        for result in end_results:
+            for key, value in result.items():
+                if key == MODIFIED_TIME:
+                    continue
+                elif value:
+                    if key not in new_history_dict:
+                        collected_keys.append(key)
+                        new_history_dict[key] = {result[MODIFIED_TIME]: value}
+                    else:
+                        new_history_dict[key].update({result[MODIFIED_TIME]: value})
+
+        records_dict = {
+            "history": new_history_dict,
+        }
+
+        return records_dict
+
     def select_distinct(
         self,
         columns: Union[str, List[str]],
     ) -> List[Tuple]:
         """
         Perform a `SELECT DISTINCT` on given table and column
 
@@ -523,26 +659,42 @@
                 f"Could not insert into the status table ('{self.table_name}'). Exception: {e}"
             )
             raise
         if prev_status:
             _LOGGER.debug(f"Changed status from '{prev_status}' to '{status_identifier}'")
 
     def _create_orms(self, pipeline_type):
-        """Create ORMs."""
+        """Create ORMs.
+        :param str pipeline_type: project or sample-level pipeline
+        :return dict: {table_name: model}
+        """
         _LOGGER.debug(f"Creating models for '{self.pipeline_name}' table in '{PKG_NAME}' database")
         model = self.parsed_schema.build_model(pipeline_type=pipeline_type)
         table_name = self.parsed_schema._table_name(pipeline_type)
         # TODO reconsider line below. Why do we need to return a dict?
         if model:
             return {table_name: model}
         else:
             raise SchemaError(
                 f"Neither project nor samples model could be built from schema source: {self.status_schema_source}"
             )
 
+    def _create_history_orms(self, pipeline_type):
+        """Creates the additional ORMs for auditing result modifications
+        :param str pipeline_type: project or sample-level pipeline
+        :return dict: {table_name: model}
+        """
+        model, table_name = self.parsed_schema.build_history_model(pipeline_type=pipeline_type)
+        if model:
+            return {table_name: model}
+        else:
+            raise SchemaError(
+                f"Neither project nor samples model could be built from schema source: {self.status_schema_source}"
+            )
+
     @property
     def _engine(self):
         """Access the database engine backing this manager."""
         try:
             return self.db_engine_key
         except AttributeError:
             # Do it this way rather than .setdefault to avoid evaluating
```

### Comparing `pipestat-0.9.0a1/pipestat/backends/file_backend/filebackend.py` & `pipestat-0.9.1/pipestat/backends/file_backend/filebackend.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from ubiquerg import create_lock, remove_lock
 
 from typing import List, Dict, Any, Optional, Union, Literal, Callable, Tuple
 
 from ...exceptions import UnrecognizedStatusError, PipestatError
 from ...backends.abstract import PipestatBackend
-from ...const import DATE_FORMAT, PKG_NAME, CREATED_TIME, MODIFIED_TIME
+from ...const import DATE_FORMAT, PKG_NAME, CREATED_TIME, MODIFIED_TIME, META_KEY, HISTORY_KEY
 
 
 _LOGGER = getLogger(PKG_NAME)
 
 
 class FileBackend(PipestatBackend):
     def __init__(
@@ -249,19 +249,26 @@
         if result_identifier and not self.check_result_exists(
             result_identifier, record_identifier
         ):
             _LOGGER.error(f"'{result_identifier}' has not been reported for '{record_identifier}'")
             return False
 
         if rm_record:
+            # NOTE: THIS CURRENTLY REMOVES ALL HISTORY OF THE RECORD AS WELL
             self.remove_record(
                 record_identifier=record_identifier,
                 rm_record=rm_record,
             )
         else:
+            self._modify_history(
+                data=self._data[self.pipeline_name][self.pipeline_type][record_identifier],
+                res_id=result_identifier,
+                time=datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
+                value="",
+            )
             del self._data[self.pipeline_name][self.pipeline_type][record_identifier][
                 result_identifier
             ]
             _LOGGER.info(
                 f"Removed result '{result_identifier}' for record "
                 f"'{record_identifier}' from '{self.pipeline_name}' namespace"
             )
@@ -274,27 +281,17 @@
                     record_identifier=record_identifier,
                     rm_record=rm_record,
                 )
             # Check if the last remaining attributes are the timestamps
             remaining_attributes = list(
                 self._data[self.pipeline_name][self.pipeline_type][record_identifier].keys()
             )
-            if (
-                len(remaining_attributes) == 2
-                and CREATED_TIME in remaining_attributes
-                and MODIFIED_TIME in remaining_attributes
-            ):
-                _LOGGER.info(
-                    f"Last result removed for '{record_identifier}'. " f"Removing the record"
-                )
-                rm_record = True
-                self.remove_record(
-                    record_identifier=record_identifier,
-                    rm_record=rm_record,
-                )
+            if len(remaining_attributes) == 1 and META_KEY in remaining_attributes:
+                _LOGGER.info(f"Last result removed for '{record_identifier}'.")
+
             with write_lock(self._data) as locked_data:
                 locked_data.write()
         return True
 
     def remove_record(
         self,
         record_identifier: Optional[str] = None,
@@ -316,22 +313,25 @@
                 return True
             except:
                 _LOGGER.warning(
                     f" Unable to remove record, aborting Removing '{record_identifier}' record"
                 )
                 return False
         else:
-            _LOGGER.info(f" rm_record flag False, aborting Removing '{record_identifier}' record")
+            _LOGGER.info(
+                f" rm_record flag is set to False, aborting Removing '{record_identifier}' record"
+            )
 
     def report(
         self,
         values: Dict[str, Any],
         record_identifier: Optional[str] = None,
         force_overwrite: bool = True,
         result_formatter: Optional[staticmethod] = None,
+        history_enabled: bool = True,
     ) -> Union[List[str], bool]:
         """
         Update the value of a result in a current namespace.
 
         This method overwrites any existing data and creates the required
          hierarchical mapping structure if needed.
 
@@ -351,35 +351,65 @@
         current_time = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
 
         result_identifiers = list(values.keys())
         if self.parsed_schema is not None:
             self.assert_results_defined(
                 results=result_identifiers, pipeline_type=self.pipeline_type
             )
+
         existing = self.list_results(
             record_identifier=record_identifier,
             restrict_to=result_identifiers,
         )
+
         if existing:
             existing_str = ", ".join(existing)
             _LOGGER.warning(f"These results exist for '{record_identifier}': {existing_str}")
             if not force_overwrite:
                 return False
             _LOGGER.info(f"Overwriting existing results: {existing_str}")
-            values.update({MODIFIED_TIME: current_time})
+            self._data[self.pipeline_name][self.pipeline_type][record_identifier][META_KEY].update(
+                {MODIFIED_TIME: current_time}
+            )
         if not existing:
             if record_identifier in self._data[self.pipeline_name][self.pipeline_type].keys():
-                values.update({MODIFIED_TIME: current_time})
-            else:
-                values.update({CREATED_TIME: current_time})
-                values.update({MODIFIED_TIME: current_time})
+                self._data[self.pipeline_name][self.pipeline_type][record_identifier].setdefault(
+                    META_KEY, {}
+                )
+                self._data[self.pipeline_name][self.pipeline_type][record_identifier][
+                    META_KEY
+                ].update({MODIFIED_TIME: current_time})
 
-        self._data[self.pipeline_name][self.pipeline_type].setdefault(record_identifier, {})
+            else:
+                self._data[self.pipeline_name][self.pipeline_type].setdefault(
+                    record_identifier, {}
+                )
+                self._data[self.pipeline_name][self.pipeline_type][record_identifier].setdefault(
+                    META_KEY, {}
+                )
+                self._data[self.pipeline_name][self.pipeline_type][record_identifier][
+                    META_KEY
+                ].update({MODIFIED_TIME: current_time})
+                self._data[self.pipeline_name][self.pipeline_type][record_identifier][
+                    META_KEY
+                ].update({CREATED_TIME: current_time})
 
         for res_id, val in values.items():
+            if history_enabled:
+                if existing:
+                    self._modify_history(
+                        data=self._data[self.pipeline_name][self.pipeline_type][record_identifier][
+                            META_KEY
+                        ],
+                        res_id=res_id,
+                        time=current_time,
+                        value=self._data[self.pipeline_name][self.pipeline_type][
+                            record_identifier
+                        ][res_id],
+                    )
             self._data[self.pipeline_name][self.pipeline_type][record_identifier][res_id] = val
             results_formatted.append(
                 result_formatter(
                     pipeline_name=self.pipeline_name,
                     record_identifier=record_identifier,
                     res_id=res_id,
                     value=val,
@@ -425,27 +455,29 @@
     def select_records(
         self,
         columns: Optional[List[str]] = None,
         filter_conditions: Optional[List[Dict[str, Any]]] = None,
         limit: Optional[int] = 1000,
         cursor: Optional[int] = None,
         bool_operator: Optional[str] = "AND",
+        meta_data_bool: Optional[bool] = False,
     ) -> Dict[str, Any]:
         """
         Select records from the FileBackend
 
         :param list[str] columns: columns to include in the result
         :param list[dict]  filter_conditions: e.g. [{"key": ["id"], "operator": "eq", "value": 1)], operator list:
             - eq for ==
             - lt for <
             - ge for >=
             - in for in_
         :param int limit: maximum number of results to retrieve per page
         :param int cursor: cursor position to begin retrieving records
         :param bool bool_operator: Perform filtering with AND or OR Logic.
+        :param bool meta_data: Should this return associated meta data with records?
         :return dict records_dict = {
             "total_size": int,
             "page_size": int,
             "next_page_token": int,
             "records": List[Dict[{key, Any}]],
         }
         """
@@ -515,39 +547,42 @@
                 retrieved_results = []
 
                 # Check each sample's dict
                 for record_identifier in list(data.keys())[0:limit]:
                     if filter_condition["key"] != "record_identifier":
                         for key, value in data[record_identifier].items():
                             result = False
-                            if isinstance(value, dict):
+                            if isinstance(value, dict) and key != "meta":
                                 if key == filter_condition["key"][0]:
                                     result = get_nested_column(
                                         value,
                                         filter_condition["key"][1:],
                                         retrieved_operator,
                                     )
                             else:
-                                if filter_condition["key"] == key:
+                                if key == "meta":
                                     # Filter datetime objects
-                                    if key in CREATED_TIME or key in MODIFIED_TIME:
+                                    if (
+                                        filter_condition["key"] == CREATED_TIME
+                                        or filter_condition["key"] == MODIFIED_TIME
+                                    ):
                                         try:
                                             time_stamp = datetime.datetime.strptime(
-                                                data[record_identifier][key],
+                                                data[record_identifier][META_KEY][
+                                                    filter_condition["key"]
+                                                ],
                                                 DATE_FORMAT,
                                             )
                                             result = retrieved_operator(
                                                 time_stamp, filter_condition["value"]
                                             )
                                         except TypeError:
                                             result = False
-                                    else:
-                                        result = retrieved_operator(
-                                            value, filter_condition["value"]
-                                        )
+                                elif filter_condition["key"] == key:
+                                    result = retrieved_operator(value, filter_condition["value"])
 
                             if result:
                                 retrieved_results.append(record_identifier)
                     else:
                         # If user wants record_identifier
                         if isinstance(filter_condition["value"], list):
                             for v in filter_condition["value"]:
@@ -585,14 +620,16 @@
                     if "record_identifier" in columns:
                         record.update({"record_identifier": record_identifier})
                 else:
                     record = data[record_identifier]
                 if record != {}:
                     record.update({"record_identifier": record_identifier})
                     records_list.append(record)
+                    if "meta" in record and not meta_data_bool:
+                        del record["meta"]
 
         records_dict = {
             "total_size": total_count,
             "page_size": limit,
             "next_page_token": 0,
             "records": records_list,
         }
@@ -734,7 +771,20 @@
                 _LOGGER.warning("MULTI PIPELINES FOR SINGLE RESULTS FILE")
             else:
                 raise PipestatError(
                     f"Trying to report result for namespace '{self.pipeline_name}' at '{self.results_file_path}', but "
                     f"{num_namespaces} other namespaces are already in the file: [{', '.join(namespaces_reported)}]. "
                     f"Pipestat will not report multiple namespaces to one file unless `multi_pipelines` is True."
                 )
+
+    def _modify_history(self, data, res_id, time, value):
+        """Modify File backend with each change
+
+        data is the loaded yaml results file in dict format
+        type = "report", "deletion"
+        """
+        if "history" not in data:
+            data.setdefault(HISTORY_KEY, {})
+        if res_id not in data[HISTORY_KEY]:
+            data[HISTORY_KEY].setdefault(res_id, {})
+
+        data[HISTORY_KEY][res_id].update({time: value})
```

### Comparing `pipestat-0.9.0a1/pipestat/cli.py` & `pipestat-0.9.1/pipestat/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     STATUS_CMD,
     STATUS_GET_CMD,
     STATUS_SET_CMD,
     INIT_CMD,
     SUMMARIZE_CMD,
     SERVE_CMD,
     LINK_CMD,
+    HISTORY_CMD,
 )
 from .const import (
     SCHEMA_KEY,
     SCHEMA_TYPE_KEY,
     CANONICAL_TYPES,
     PKG_NAME,
 )
@@ -117,15 +118,15 @@
         database_only=args.database_only,
         flag_file_dir=args.flag_dir,
         pipeline_type=args.pipeline_type,
     )
     types_to_read_from_json = ["object"] + list(CANONICAL_TYPES.keys())
 
     # The next few commands require a record_identifier. Need to also check ENV variables for its existence.
-    if args.record_identifier is None:
+    if not hasattr(args, "record_identifier") or getattr(args, "record_identifier", None) is None:
         args.record_identifier = os.getenv("PIPESTAT_RECORD_IDENTIFIER")
 
     if args.command == REPORT_CMD:
         value = args.value
         if psm.cfg[SCHEMA_KEY] is None:
             raise SchemaNotFoundError(msg="report", cli=True)
         result_metadata = psm.cfg[SCHEMA_KEY].results_data[args.result_identifier]
@@ -170,9 +171,16 @@
         if args.subcommand == STATUS_GET_CMD:
             print(psm.get_status(record_identifier=args.record_identifier))
         if args.subcommand == STATUS_SET_CMD:
             psm.set_status(
                 status_identifier=args.status_identifier,
                 record_identifier=args.record_identifier,
             )
+    if args.command == HISTORY_CMD:
+        print(f"\nHistory for Record: {args.record_identifier}")
+        print(
+            psm.retrieve_history(
+                record_identifier=args.record_identifier, result_identifier=args.result_identifier
+            )
+        )
 
     sys.exit(0)
```

### Comparing `pipestat-0.9.0a1/pipestat/const.py` & `pipestat-0.9.1/pipestat/const.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,14 +59,17 @@
     "TEMPLATES_DIRNAME",
     "NO_DATA_PLACEHOLDER",
     "PROFILE_COLNAMES",
     "OUTPUT_DIR",
     "RECORD_IDENTIFIER",
     "CREATED_TIME",
     "MODIFIED_TIME",
+    "DATE_FORMAT",
+    "META_KEY",
+    "HISTORY_KEY",
 ]
 
 PKG_NAME = "pipestat"
 LOCK_PREFIX = "lock."
 
 # object attribute names
 SAMPLE_NAME_ID_KEY = "_sample_name"
@@ -80,14 +83,17 @@
 # DB column names
 SAMPLE_NAME = "sample_name"
 RECORD_IDENTIFIER = "record_identifier"
 STATUS = "status"
 CREATED_TIME = "pipestat_created_time"
 MODIFIED_TIME = "pipestat_modified_time"
 
+META_KEY = "meta"
+HISTORY_KEY = "history"
+
 CANONICAL_TYPES = {
     "image": {
         "type": "object",
         "properties": {
             "path": {"type": "string"},
             "thumbnail_path": {"type": "string"},
             "title": {"type": "string"},
```

### Comparing `pipestat-0.9.0a1/pipestat/exceptions.py` & `pipestat-0.9.1/pipestat/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     "PipestatDataError",
     "UnrecognizedStatusError",
     "RecordNotFoundError",
     "PipelineTypeNotSuppliedError",
     "InvalidTimeFormatError",
     "PipestatDependencyError",
     "ColumnNotFoundError",
+    "SchemaValidationErrorDuringReport",
 ]
 
 
 class RecordNotFoundError(LookupError):
     def __init__(self, msg):
         super(RecordNotFoundError, self).__init__(msg)
```

### Comparing `pipestat-0.9.0a1/pipestat/helpers.py` & `pipestat-0.9.1/pipestat/helpers.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0a1/pipestat/jinja_templates/footer_index.html` & `pipestat-0.9.1/pipestat/jinja_templates/footer_index.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0a1/pipestat/jinja_templates/glossary_table.html` & `pipestat-0.9.1/pipestat/jinja_templates/glossary_table.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0a1/pipestat/jinja_templates/head.html` & `pipestat-0.9.1/pipestat/jinja_templates/head.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0a1/pipestat/jinja_templates/index.html` & `pipestat-0.9.1/pipestat/jinja_templates/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
 	<!--			}, function () {-->
 	<!--				var index = $(this).data('index');-->
 	<!--				that.$body.find('> tr[data-index="' + index + '"]').removeClass('hover');-->
 	<!--			});-->
 	<!--		};-->
 
 	<!--		})(jQuery);-->
-	</script>
+<!--	</script>-->
 	<script>
 		$.noConflict();
 		jQuery(function ($) {
 			$('[data-toggle="popover"]').popover();
 			$('#summary-table').on('all.bs.table', function (e, name, args) {
 				$('[data-toggle="popover"]').popover();
 			});
```

### Comparing `pipestat-0.9.0a1/pipestat/jinja_templates/logo.html` & `pipestat-0.9.1/pipestat/jinja_templates/logo.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0a1/pipestat/jinja_templates/navbar.html` & `pipestat-0.9.1/pipestat/jinja_templates/navbar.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0a1/pipestat/jinja_templates/navbar_links.html` & `pipestat-0.9.1/pipestat/jinja_templates/navbar_links.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0a1/pipestat/jinja_templates/navbar_list_parent.html` & `pipestat-0.9.1/pipestat/jinja_templates/navbar_list_parent.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0a1/pipestat/jinja_templates/object.html` & `pipestat-0.9.1/pipestat/jinja_templates/object.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0a1/pipestat/jinja_templates/project_object.html` & `pipestat-0.9.1/pipestat/jinja_templates/project_object.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0a1/pipestat/jinja_templates/sample.html` & `pipestat-0.9.1/pipestat/jinja_templates/sample.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0a1/pipestat/jinja_templates/status_table.html` & `pipestat-0.9.1/pipestat/jinja_templates/status_table.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0a1/pipestat/jinja_templates/status_table_no_links.html` & `pipestat-0.9.1/pipestat/jinja_templates/status_table_no_links.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0a1/pipestat/parsed_schema.py` & `pipestat-0.9.1/pipestat/parsed_schema.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0a1/pipestat/pipestat.py` & `pipestat-0.9.1/pipestat/pipestat.py`

 * *Files 4% similar despite different names*

```diff
@@ -472,14 +472,15 @@
             except ValueError:
                 raise InvalidTimeFormatError(msg=f"Incorrect time format, requires: {date_format}")
 
         if time_column == "created":
             col_name = CREATED_TIME
         else:
             col_name = MODIFIED_TIME
+
         results = self.select_records(
             limit=limit,
             filter_conditions=[
                 {
                     "key": col_name,
                     "operator": "lt",
                     "value": start,
@@ -487,15 +488,14 @@
                 {
                     "key": col_name,
                     "operator": "gt",
                     "value": end,
                 },
             ],
         )
-
         return results
 
     def process_schema(self, schema_path):
         # Load pipestat schema in two parts: 1) main and 2) status
         self._schema_path = self.cfg[CONFIG_KEY].priority_get(
             "schema_path", env_var=ENV_VARS["schema"], override=schema_path
         )
@@ -543,34 +543,47 @@
         r_id = record_identifier or self.cfg[RECORD_IDENTIFIER]
         return self.backend.remove(
             record_identifier=r_id,
             result_identifier=result_identifier,
         )
 
     @require_backend
+    def remove_record(
+        self,
+        record_identifier: Optional[str] = None,
+        rm_record: Optional[bool] = False,
+    ) -> bool:
+        return self.backend.remove_record(
+            record_identifier=record_identifier,
+            rm_record=rm_record,
+        )
+
+    @require_backend
     def report(
         self,
         values: Dict[str, Any],
         record_identifier: Optional[str] = None,
         force_overwrite: bool = True,
         result_formatter: Optional[staticmethod] = None,
         strict_type: bool = True,
+        history_enabled: bool = True,
     ) -> Union[List[str], bool]:
         """
         Report a result.
 
         :param Dict[str, any] values: dictionary of result-value pairs
         :param str record_identifier: unique identifier of the record, value
             in 'record_identifier' column to look for to determine if the record
             already exists
         :param bool force_overwrite: whether to overwrite the existing record
         :param str result_formatter: function for formatting result
         :param bool strict_type: whether the type of the reported values should
             remain as is. Pipestat would attempt to convert to the
             schema-defined one otherwise
+        :param bool history_enabled: Should history of reported results be enabled?
         :return str reported_results: return list of formatted string
         """
 
         result_formatter = result_formatter or self.cfg[RESULT_FORMATTER]
         values = deepcopy(values)
         r_id = record_identifier or self.cfg[RECORD_IDENTIFIER]
         if r_id is None:
@@ -593,14 +606,15 @@
                 )
 
         reported_results = self.backend.report(
             values=values,
             record_identifier=r_id,
             force_overwrite=force_overwrite,
             result_formatter=result_formatter,
+            history_enabled=history_enabled,
         )
 
         return reported_results
 
     @require_backend
     def select_distinct(
         self,
@@ -661,21 +675,18 @@
         self,
         record_identifier: str = None,
         result_identifier: Optional[Union[str, List[str]]] = None,
     ) -> Union[Any, Dict[str, Any]]:
         """
         Retrieve a single record
         :param str record_identifier: single record_identifier
-        :param str result_identifier: single record_identifier
-        :return: Dict[str, any]: a mapping with filtered
-
-
-            results reported for the record
+        :param str result_identifier: single record_identifier or list of result identifiers
+        :return: Dict[str, any]: a mapping with filtered results reported for the record
         """
-        r_id = record_identifier or self.record_identifier
+        record_identifier = record_identifier or self.record_identifier
 
         filter_conditions = [
             {
                 "key": "record_identifier",
                 "operator": "eq",
                 "value": record_identifier,
             },
@@ -717,14 +728,77 @@
                     except IndexError:
                         raise RecordNotFoundError(f"Record '{record_identifier}' not found")
                 else:
                     raise RecordNotFoundError(f"Record '{record_identifier}' not found")
             except IndexError:
                 raise RecordNotFoundError(f"Record '{record_identifier}' not found")
 
+    def retrieve_history(
+        self,
+        record_identifier: str = None,
+        result_identifier: Optional[Union[str, List[str]]] = None,
+    ) -> Union[Any, Dict[str, Any]]:
+        """
+        Retrieve a single record's history
+        :param str record_identifier: single record_identifier
+        :param str result_identifier: single result_identifier or list of result identifiers
+        :return: Dict[str, any]: a mapping with filtered historical results
+        """
+
+        record_identifier = record_identifier or self.record_identifier
+
+        if self.file:
+            result = self.backend.select_records(
+                filter_conditions=[
+                    {
+                        "key": "record_identifier",
+                        "operator": "eq",
+                        "value": record_identifier,
+                    }
+                ],
+                meta_data_bool=True,
+            )["records"][0]
+
+            if "meta" in result and "history" in result["meta"]:
+                history = {}
+                if isinstance(result_identifier, str) and result_identifier in result:
+                    history.update(
+                        {result_identifier: result["meta"]["history"][result_identifier]}
+                    )
+                elif isinstance(result_identifier, list):
+                    for r in result_identifier:
+                        if r in result["meta"]["history"]:
+                            history.update({r: result["meta"]["history"][r]})
+                else:
+                    history = result["meta"]["history"]
+            else:
+                _LOGGER.warning(f"No history available for Record: {record_identifier}")
+                return {}
+
+        else:
+            if result_identifier:
+                history = self.backend.retrieve_history_db(record_identifier, result_identifier)[
+                    "history"
+                ]
+            else:
+                history = self.backend.retrieve_history_db(record_identifier)["history"]
+
+            # DB backend returns some extra_keys that we can remove before returning them to the user.
+            extra_keys_to_delete = [
+                "id",
+                "pipestat_created_time",
+                "source_record_id",
+                "record_identifier",
+            ]
+            history = {
+                key: value for key, value in history.items() if key not in extra_keys_to_delete
+            }
+
+        return history
+
     def retrieve_many(
         self,
         record_identifiers: List[str],
         result_identifier: Optional[str] = None,
     ) -> Union[Any, Dict[str, Any]]:
         """
         :param record_identifiers: list of record identifiers
```

### Comparing `pipestat-0.9.0a1/pipestat/pipestatreader/README.md` & `pipestat-0.9.1/pipestat/pipestatreader/README.md`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0a1/pipestat/pipestatreader/reader.py` & `pipestat-0.9.1/pipestat/pipestatreader/reader.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0a1/pipestat/reports.py` & `pipestat-0.9.1/pipestat/reports.py`

 * *Files 1% similar despite different names*

```diff
@@ -700,15 +700,15 @@
         if self.looper_samples is not None:
             # If looper passes the samples from the PEP, we should add the attributes to the cell tables:
             input_sample_attributes = self.looper_samples[0]._mapped_attr["_attributes"]
             # Place at front of columns
             all_result_identifiers = input_sample_attributes + all_result_identifiers
 
         if self.prj.cfg["multi_result_files"] is True:
-            pipeline_types = ["sample", "project"]
+            pipeline_types = ["sample"]
         else:
             pipeline_types = [self.prj.backend.pipeline_type]
 
         sorted_sample_stat_results = {}
         for pipeline_type in pipeline_types:
             self.prj.backend.pipeline_type = pipeline_type
             for sample in self.prj.backend.select_records()["records"]:
@@ -727,14 +727,23 @@
                                 value = self.looper_samples[s]._mapped_attr[attribute]
                                 sample_stat_results.update({attribute: value})
 
                 for key in all_result_identifiers:
                     if key not in sample_stat_results.keys():
                         sample_stat_results[key] = ""
 
+                for key in self.schema.keys():
+                    if "type" in self.schema[key]:
+                        if (
+                            self.schema[key]["type"] == "file"
+                            or self.schema[key]["type"] == "image"
+                            or self.schema[key]["type"] == "object"
+                        ):
+                            del sample_stat_results[key]
+
                 # Sort to ensure alignment in the table
                 sorted_sample_stat_results = dict(sorted(sample_stat_results.items()))
 
                 sample_html = self.create_sample_html(
                     sorted_sample_stat_results,
                     navbar,
                     footer,
@@ -776,21 +785,22 @@
         glossary_table = create_glossary_table(project=self.prj)
         save_html(
             path=os.path.join(self.pipeline_reports, "glossary.html"),
             template=self.create_glossary_html(glossary_table, navbar, footer),
         )
 
         project_objects = self.create_project_objects()
-        columns = ["Record Identifiers"] + list(sorted_sample_stat_results.keys())
+        columns_table = ["Record Identifiers"] + list(sorted_sample_stat_results.keys())
+        columns_stats = list(sorted_sample_stat_results.keys())
         template_vars = dict(
             navbar=navbar,
             stats_file_path=stats_file_path,
             objs_file_path=objs_file_path,
-            columns=columns,
-            columns_json=dumps(columns),
+            columns=columns_table,
+            columns_json=dumps(columns_stats),
             table_row_data=table_row_data,
             project_name=self.prj.cfg[PROJECT_NAME],
             pipeline_name=self.pipeline_name,
             stats_json=self._stats_to_json_str(),
             project_objects=project_objects,
             footer=footer,
             amendments="",
@@ -934,15 +944,15 @@
                     results.append(key)
 
         return results
 
     def _stats_to_json_str(self):
         results = {}
         if self.prj.cfg["multi_result_files"] is True:
-            pipeline_types = ["sample", "project"]
+            pipeline_types = ["sample"]
         else:
             pipeline_types = [self.prj.backend.pipeline_type]
 
         for pipeline_type in pipeline_types:
             self.prj.backend.pipeline_type = pipeline_type
             for sample in self.prj.backend.select_records()["records"]:
                 sample_name = sample["record_identifier"]
```

### Comparing `pipestat-0.9.0a1/pipestat/schemas/pipestat_config_schema.yaml` & `pipestat-0.9.1/pipestat/schemas/pipestat_config_schema.yaml`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0a1/pipestat.egg-info/PKG-INFO` & `pipestat-0.9.1/pipestat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipestat
-Version: 0.9.0a1
+Version: 0.9.1
 Summary: A pipeline results reporter
 Home-page: https://github.com/pepkit/pipestat
 Author: Michal Stolarczyk, Nathan Sheffield
 License: BSD2
 Keywords: project,metadata,bioinformatics,sequencing,ngs,workflow
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pipestat-0.9.0a1/pipestat.egg-info/SOURCES.txt` & `pipestat-0.9.1/pipestat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0a1/setup.py` & `pipestat-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0a1/tests/test_db_only_mode.py` & `pipestat-0.9.1/tests/test_db_only_mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,15 @@
             try:
                 SamplePipestatManager(
                     schema_path=schema_file_path,
                     record_identifier="irrelevant",
                     database_only=True,
                     config_file=config_file_path,
                 )
+                print("done")
             except Exception as e:
                 pytest.fail(f"Pipestat manager construction failed: {e})")
 
     @pytest.mark.parametrize(["rec_id", "res_id"], [("sample2", "number_of_things")])
     def test_select_invalid_filter_column__raises_expected_exception(
         self,
         rec_id,
```

### Comparing `pipestat-0.9.0a1/tests/test_init.py` & `pipestat-0.9.1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0a1/tests/test_parsed_schema.py` & `pipestat-0.9.1/tests/test_parsed_schema.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0a1/tests/test_pipestat.py` & `pipestat-0.9.1/tests/test_pipestat.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             ("sample2", {"number_of_things": 2}),
             ("sample2", {"percentage_of_things": 10.1}),
             ("sample2", {"name_of_something": "test_name"}),
             ("sample3", {"name_of_something": "test_name"}),
         ],
     )
     @pytest.mark.parametrize("backend", ["file", "db"])
-    def test_basics(
+    def test_basics_all(
         self,
         rec_id,
         val,
         config_file_path,
         schema_file_path,
         results_file_path,
         backend,
@@ -86,14 +86,15 @@
             assert status == "running"
             assert psm.retrieve_one(record_identifier=rec_id)[val_name] == val[val_name]
             psm.remove(record_identifier=rec_id, result_identifier=val_name)
             if backend == "file":
                 psm.clear_status(record_identifier=rec_id)
                 status = psm.get_status(record_identifier=rec_id)
                 assert status is None
+                psm.remove_record(record_identifier=rec_id, rm_record=True)
                 with pytest.raises(RecordNotFoundError):
                     psm.retrieve_one(record_identifier=rec_id)
             if backend == "db":
                 assert psm.retrieve_one(record_identifier=rec_id).get(val_name, None) is None
                 psm.remove(record_identifier=rec_id)
                 with pytest.raises(RecordNotFoundError):
                     psm.retrieve_one(record_identifier=rec_id)
@@ -173,16 +174,16 @@
             assert status == "running"
             assert psm.retrieve_one(record_identifier=rec_id)[val_name] == val[val_name]
             psm.remove(record_identifier=rec_id, result_identifier=val_name)
             if backend == "file":
                 psm.clear_status(record_identifier=rec_id)
                 status = psm.get_status(record_identifier=rec_id)
                 assert status is None
-                with pytest.raises(RecordNotFoundError):
-                    psm.retrieve_one(record_identifier=rec_id)
+                # with pytest.raises(RecordNotFoundError):
+                #     psm.retrieve_one(record_identifier=rec_id)
             if backend == "db":
                 psm.remove(record_identifier=rec_id)
                 with pytest.raises(RecordNotFoundError):
                     psm.retrieve_one(record_identifier=rec_id)
 
 
 @pytest.mark.skipif(not DB_DEPENDENCIES, reason="Requires dependencies")
@@ -195,15 +196,15 @@
             ("sample1", {"number_of_things": 1}),
             ("sample2", {"number_of_things": 2}),
             ("sample2", {"percentage_of_things": 10.1}),
             ("sample2", {"name_of_something": "test_name"}),
             ("sample3", {"name_of_something": "test_name"}),
         ],
     )
-    @pytest.mark.parametrize("backend", ["file", "db"])
+    @pytest.mark.parametrize("backend", ["db"])
     def test_report_basic(
         self,
         rec_id,
         val,
         config_file_path,
         schema_file_path,
         results_file_path,
@@ -323,15 +324,15 @@
                     "properties": {
                         "prop1": {"properties": {"path": "pathstring", "title": "titlestring"}}
                     }
                 }
             },
         ],
     )
-    @pytest.mark.parametrize("backend", ["file", "db"])
+    @pytest.mark.parametrize("backend", ["file"])
     def test_complex_object_report(
         self, val, config_file_path, recursive_schema_file_path, results_file_path, backend
     ):
         with NamedTemporaryFile() as f, ContextManagerDBTesting(DB_URL):
             results_file_path = f.name
             args = dict(schema_path=recursive_schema_file_path, database_only=False)
             backend_data = (
@@ -351,14 +352,46 @@
                         "operator": "eq",
                         "value": val[val_name],
                     }
                 ]
             )
 
     @pytest.mark.parametrize(
+        "val",
+        [
+            {"output_file": {"path": "path_string", "title": "title_string"}},
+            {
+                "output_image": {
+                    "path": "path_string",
+                    "thumbnail_path": "thumbnail_path_string",
+                    "title": "title_string",
+                }
+            },
+        ],
+    )
+    @pytest.mark.parametrize("backend", ["db"])
+    def test_complex_object_report_missing_fields(
+        self, val, config_file_path, recursive_schema_file_path, results_file_path, backend
+    ):
+        with NamedTemporaryFile() as f, ContextManagerDBTesting(DB_URL):
+            results_file_path = f.name
+            args = dict(schema_path=recursive_schema_file_path, database_only=False)
+            backend_data = (
+                {"config_file": config_file_path}
+                if backend == "db"
+                else {"results_file_path": results_file_path}
+            )
+            args.update(backend_data)
+
+            psm = SamplePipestatManager(**args)
+            del val[list(val.keys())[0]]["path"]
+            with pytest.raises(SchemaValidationErrorDuringReport):
+                psm.report(record_identifier=REC_ID, values=val, force_overwrite=True)
+
+    @pytest.mark.parametrize(
         ["rec_id", "val"],
         [
             ("sample1", {"name_of_something": "test_name"}),
         ],
     )
     @pytest.mark.parametrize("backend", ["file", "db"])
     def test_report_setitem(
@@ -587,14 +620,47 @@
             assert str(list(val.keys())[0]) in list(retrieved_val.keys())
             # Test Retrieve Whole Record
             assert isinstance(psm.retrieve_one(record_identifier=rec_id), Mapping)
 
     @pytest.mark.parametrize(
         ["rec_id", "val"],
         [
+            ("sample1", {"name_of_something": "test_name"}),
+            ("sample1", {"number_of_things": 2}),
+        ],
+    )
+    @pytest.mark.parametrize("backend", ["file", "db"])
+    def test_retrieve_basic_no_record_identifier(
+        self,
+        rec_id,
+        val,
+        config_file_path,
+        results_file_path,
+        schema_file_path,
+        backend,
+    ):
+        with NamedTemporaryFile() as f, ContextManagerDBTesting(DB_URL):
+            results_file_path = f.name
+            args = dict(schema_path=schema_file_path, database_only=False)
+            backend_data = (
+                {"config_file": config_file_path}
+                if backend == "db"
+                else {"results_file_path": results_file_path}
+            )
+            args.update(backend_data)
+            args.update(record_identifier=rec_id)
+            psm = SamplePipestatManager(**args)
+            psm.report(record_identifier=rec_id, values=val, force_overwrite=True)
+            assert (
+                psm.retrieve_one(result_identifier=list(val.keys())[0]) == list(val.items())[0][1]
+            )
+
+    @pytest.mark.parametrize(
+        ["rec_id", "val"],
+        [
             ("sample1", {"number_of_things": 2}),
         ],
     )
     @pytest.mark.parametrize("backend", ["file", "db"])
     def test_retrieve_one_single_result_as_list(
         self,
         rec_id,
@@ -861,45 +927,14 @@
                 if backend == "db"
                 else {"results_file_path": results_file_path}
             )
             args.update(backend_data)
             psm = SamplePipestatManager(**args)
             assert not psm.remove(record_identifier=rec_id)
 
-    @pytest.mark.parametrize(["rec_id", "res_id"], [("sample3", "name_of_something")])
-    @pytest.mark.parametrize("backend", ["file"])
-    def test_last_result_removal_removes_record(
-        self,
-        rec_id,
-        res_id,
-        schema_file_path,
-        config_file_path,
-        results_file_path,
-        backend,
-    ):
-        with NamedTemporaryFile() as f, ContextManagerDBTesting(DB_URL):
-            results_file_path = f.name
-            args = dict(schema_path=schema_file_path, database_only=False)
-            backend_data = (
-                {"config_file": config_file_path}
-                if backend == "db"
-                else {"results_file_path": results_file_path}
-            )
-            args.update(backend_data)
-            psm = SamplePipestatManager(**args)
-            psm.report(
-                record_identifier=rec_id,
-                values={res_id: "something"},
-                force_overwrite=True,
-            )
-            assert psm.remove(record_identifier=rec_id, result_identifier=res_id)
-
-            with pytest.raises(RecordNotFoundError):
-                result = psm.retrieve_one(record_identifier=rec_id)
-
 
 @pytest.mark.skipif(not DB_DEPENDENCIES, reason="Requires dependencies")
 @pytest.mark.skipif(SERVICE_UNAVAILABLE, reason="requires postgres service to be available")
 class TestNoRecordID:
     @pytest.mark.parametrize(
         "val",
         [
@@ -1031,15 +1066,14 @@
         monkeypatch.setenv(ENV_VARS["results_file"], results_file_path)
         monkeypatch.setenv(ENV_VARS["schema"], schema_file_path)
         try:
             SamplePipestatManager()
         except Exception as e:
             pytest.fail(f"Error during pipestat manager creation: {e}")
 
-    # @pytest.mark.skip(reason="known failure for now with config file")
     def test_config__psm_is_built_from_config_file_env_var(self, monkeypatch, config_file_path):
         """PSM can be created from config parsed from env var value."""
         monkeypatch.setenv(ENV_VARS["config"], config_file_path)
         try:
             SamplePipestatManager()
         except Exception as e:
             pytest.fail(f"Error during pipestat manager creation: {e}")
@@ -1389,15 +1423,15 @@
                     "report",
                     "--record-identifier",
                     rec_id,
                     "--result-identifier",
                     list(val.keys())[0],
                     "--value",
                     list(val.values())[0],
-                    "--config-file",
+                    "--config",
                     config_file_path,
                     "--schema",
                     schema_file_path,
                 ]
 
             with pytest.raises(
                 SystemExit
@@ -1408,31 +1442,54 @@
             if backend != "db":
                 x = [
                     "retrieve",
                     "--record-identifier",
                     rec_id,
                     "--result-identifier",
                     list(val.keys())[0],
-                    "--value",
-                    list(val.values())[0],
                     "--results-file",
                     results_file_path,
                     "--schema",
                     schema_file_path,
                 ]
             else:
                 x = [
                     "retrieve",
                     "--record-identifier",
                     rec_id,
                     "--result-identifier",
                     list(val.keys())[0],
-                    "--value",
-                    list(val.values())[0],
-                    "--config-file",
+                    "--config",
+                    config_file_path,
+                    "--schema",
+                    schema_file_path,
+                ]
+
+            with pytest.raises(
+                SystemExit
+            ):  # pipestat cli normal behavior is to end with a "sys.exit(0)"
+                main(test_args=x)
+
+            # history
+            if backend != "db":
+                x = [
+                    "history",
+                    "--record-identifier",
+                    rec_id,
+                    "--results-file",
+                    results_file_path,
+                    "--schema",
+                    schema_file_path,
+                ]
+            else:
+                x = [
+                    "history",
+                    "--record-identifier",
+                    rec_id,
+                    "--config",
                     config_file_path,
                     "--schema",
                     schema_file_path,
                 ]
 
             with pytest.raises(
                 SystemExit
@@ -1489,99 +1546,14 @@
                 # TODO This example will have collision if the file names and property names are the same
                 print(files)
 
 
 @pytest.mark.skipif(not DB_DEPENDENCIES, reason="Requires dependencies")
 @pytest.mark.skipif(SERVICE_UNAVAILABLE, reason="requires service X to be available")
 class TestTimeStamp:
-    @pytest.mark.parametrize(
-        ["rec_id", "val"],
-        [
-            ("sample1", {"name_of_something": "test_name"}),
-        ],
-    )
-    @pytest.mark.parametrize("backend", ["file", "db"])
-    def test_basic_time_stamp(
-        self,
-        rec_id,
-        val,
-        config_file_path,
-        schema_file_path,
-        results_file_path,
-        backend,
-    ):
-        with NamedTemporaryFile() as f, ContextManagerDBTesting(DB_URL):
-            results_file_path = f.name
-            args = dict(schema_path=schema_file_path, database_only=False)
-            backend_data = (
-                {"config_file": config_file_path}
-                if backend == "db"
-                else {"results_file_path": results_file_path}
-            )
-            args.update(backend_data)
-            psm = SamplePipestatManager(**args)
-            psm.report(record_identifier=rec_id, values=val, force_overwrite=True)
-
-            # CHECK CREATION AND MODIFY TIME EXIST
-
-            created = psm.select_records(
-                filter_conditions=[
-                    {
-                        "key": "record_identifier",
-                        "operator": "eq",
-                        "value": rec_id,
-                    },
-                ],
-                columns=[CREATED_TIME],
-            )["records"][0][CREATED_TIME]
-
-            modified = psm.select_records(
-                filter_conditions=[
-                    {
-                        "key": "record_identifier",
-                        "operator": "eq",
-                        "value": rec_id,
-                    },
-                ],
-                columns=[MODIFIED_TIME],
-            )["records"][0][MODIFIED_TIME]
-
-            assert created is not None
-            assert modified is not None
-            assert created == modified
-            # Report new
-            val = {"number_of_things": 1}
-            time.sleep(
-                1
-            )  # The filebackend is so fast that the updated time will equal the created time
-            psm.report(record_identifier="sample1", values=val, force_overwrite=True)
-            # CHECK MODIFY TIME DIFFERS FROM CREATED TIME
-            created = psm.select_records(
-                filter_conditions=[
-                    {
-                        "key": "record_identifier",
-                        "operator": "eq",
-                        "value": rec_id,
-                    },
-                ],
-                columns=[CREATED_TIME],
-            )["records"][0][CREATED_TIME]
-
-            modified = psm.select_records(
-                filter_conditions=[
-                    {
-                        "key": "record_identifier",
-                        "operator": "eq",
-                        "value": rec_id,
-                    },
-                ],
-                columns=[MODIFIED_TIME],
-            )["records"][0][MODIFIED_TIME]
-
-            assert created != modified
 
     @pytest.mark.parametrize("backend", ["db", "file"])
     def test_list_recent_results(
         self,
         config_file_path,
         schema_file_path,
         results_file_path,
@@ -1625,15 +1597,15 @@
             results = psm.list_recent_results(start="2100-01-01 0:0:0", end="1970-01-01 0:0:0")
             assert len(results["records"]) == 10
 
 
 @pytest.mark.skipif(not DB_DEPENDENCIES, reason="Requires dependencies")
 @pytest.mark.skipif(SERVICE_UNAVAILABLE, reason="requires service X to be available")
 class TestSelectRecords:
-    @pytest.mark.parametrize("backend", ["file", "db"])
+    @pytest.mark.parametrize("backend", ["db", "file"])
     def test_select_records_basic(
         self,
         config_file_path,
         results_file_path,
         recursive_schema_file_path,
         backend,
         range_values,
@@ -2367,7 +2339,177 @@
                 r_id = i[0]
                 val = i[1]
                 psm.report(record_identifier=r_id, values=val, force_overwrite=True)
 
             mod = psm.backend.get_model(table_name=psm.backend.table_name)
             assert mod.md5sum.index is True
             assert mod.number_of_things.index is False
+
+
+@pytest.mark.skipif(not DB_DEPENDENCIES, reason="Requires dependencies")
+@pytest.mark.skipif(SERVICE_UNAVAILABLE, reason="requires service X to be available")
+class TestRetrieveHistory:
+    @pytest.mark.parametrize(
+        ["rec_id", "val"],
+        [
+            ("sample1", {"name_of_something": "test_name"}),
+        ],
+    )
+    @pytest.mark.parametrize("backend", ["db", "file"])
+    def test_select_history_basic(
+        self,
+        config_file_path,
+        results_file_path,
+        schema_file_path,
+        backend,
+        range_values,
+        rec_id,
+        val,
+    ):
+        with NamedTemporaryFile() as f, ContextManagerDBTesting(DB_URL):
+            results_file_path = f.name
+            args = dict(schema_path=schema_file_path, database_only=False)
+            backend_data = (
+                {"config_file": config_file_path}
+                if backend == "db"
+                else {"results_file_path": results_file_path}
+            )
+            args.update(backend_data)
+            psm = SamplePipestatManager(**args)
+
+            val["number_of_things"] = 1
+
+            psm.report(record_identifier=rec_id, values=val, force_overwrite=True)
+
+            val = {"name_of_something": "MODIFIED_test_name", "number_of_things": 2}
+
+            time.sleep(1)
+
+            psm.report(record_identifier=rec_id, values=val, force_overwrite=True)
+
+            history_result = psm.retrieve_history(
+                record_identifier="sample1", result_identifier="name_of_something"
+            )
+
+            all_history_result = psm.retrieve_history(record_identifier="sample1")
+
+            assert len(all_history_result.keys()) == 2
+            assert len(history_result.keys()) == 1
+            assert len(history_result["name_of_something"].keys()) == 1
+
+    @pytest.mark.parametrize(
+        ["rec_id", "val"],
+        [
+            ("sample1", {"name_of_something": "test_name"}),
+        ],
+    )
+    @pytest.mark.parametrize("backend", ["db", "file"])
+    def test_select_history_multi_results(
+        self,
+        config_file_path,
+        results_file_path,
+        schema_file_path,
+        backend,
+        range_values,
+        rec_id,
+        val,
+    ):
+        with NamedTemporaryFile() as f, ContextManagerDBTesting(DB_URL):
+            results_file_path = f.name
+            args = dict(schema_path=schema_file_path, database_only=False)
+            backend_data = (
+                {"config_file": config_file_path}
+                if backend == "db"
+                else {"results_file_path": results_file_path}
+            )
+            args.update(backend_data)
+            psm = SamplePipestatManager(**args)
+
+            val["number_of_things"] = 1
+
+            psm.report(record_identifier=rec_id, values=val, force_overwrite=True)
+
+            val = {"name_of_something": "MODIFIED_test_name", "number_of_things": 2}
+
+            time.sleep(1)
+
+            psm.report(record_identifier=rec_id, values=val, force_overwrite=True)
+
+            history_result = psm.retrieve_history(
+                record_identifier="sample1",
+                result_identifier=["name_of_something", "number_of_things"],
+            )
+
+            assert len(history_result.keys()) == 2
+            assert len(history_result["name_of_something"].keys()) == 1
+
+    @pytest.mark.parametrize(
+        ["rec_id", "val"],
+        [
+            (
+                "sample1",
+                {
+                    "output_image": {
+                        "path": "path_string",
+                        "thumbnail_path": "thumbnail_path_string",
+                        "title": "title_string",
+                    }
+                },
+            ),
+        ],
+    )
+    @pytest.mark.parametrize("backend", ["db", "file"])
+    def test_select_history_complex_objects(
+        self,
+        config_file_path,
+        results_file_path,
+        recursive_schema_file_path,
+        backend,
+        range_values,
+        rec_id,
+        val,
+    ):
+        with NamedTemporaryFile() as f, ContextManagerDBTesting(DB_URL):
+            results_file_path = f.name
+            args = dict(schema_path=recursive_schema_file_path, database_only=False)
+            backend_data = (
+                {"config_file": config_file_path}
+                if backend == "db"
+                else {"results_file_path": results_file_path}
+            )
+            args.update(backend_data)
+            psm = SamplePipestatManager(**args)
+
+            psm.report(record_identifier=rec_id, values=val, force_overwrite=True)
+
+            val = {
+                "output_image": {
+                    "path": "path_string2",
+                    "thumbnail_path": "thumbnail_path_string2",
+                    "title": "title_string2",
+                }
+            }
+
+            time.sleep(1)
+
+            psm.report(record_identifier=rec_id, values=val, force_overwrite=True)
+
+            val = {
+                "output_image": {
+                    "path": "path_string3",
+                    "thumbnail_path": "thumbnail_path_string3",
+                    "title": "title_string3",
+                }
+            }
+
+            time.sleep(1)
+
+            psm.report(record_identifier=rec_id, values=val, force_overwrite=True)
+
+            history_result = psm.retrieve_history(
+                record_identifier="sample1",
+                result_identifier="output_image",
+            )
+
+            assert len(history_result.keys()) == 1
+            assert "output_image" in history_result
+            assert len(history_result["output_image"].keys()) == 2
```

### Comparing `pipestat-0.9.0a1/tests/test_status.py` & `pipestat-0.9.1/tests/test_status.py`

 * *Files identical despite different names*

