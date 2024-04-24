# Comparing `tmp/ckanext-editable-config-0.0.4.tar.gz` & `tmp/ckanext_editable_config-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-editable-config-0.0.4.tar", last modified: Fri Jul 28 22:50:04 2023, max compression
+gzip compressed data, was "ckanext_editable_config-0.0.5.tar", last modified: Wed Apr 24 09:21:03 2024, max compression
```

## Comparing `ckanext-editable-config-0.0.4.tar` & `ckanext_editable_config-0.0.5.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.4/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      215 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.4/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)    12795 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)    12207 2023-07-28 22:11:05.000000 ckanext-editable-config-0.0.4/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.963428 ckanext-editable-config-0.0.4/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      202 2023-06-18 20:14:29.000000 ckanext-editable-config-0.0.4/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/ckanext/editable_config/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/ckanext/editable_config/assets/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/ckanext/editable_config/assets/js/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      418 2023-07-28 22:08:36.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/assets/js/editable-config-toggle-field.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)      167 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/assets/script.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)       35 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/assets/style.css
--rw-r--r--   0 sergey    (1000) sergey    (1000)      356 2023-07-28 21:54:04.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/assets/webassets.yml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1211 2023-07-28 16:17:04.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/config.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      636 2023-07-28 22:26:11.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/helpers.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/ckanext/editable_config/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 11:15:55.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6695 2023-07-28 22:10:23.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/logic/action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1782 2023-07-25 22:20:05.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/logic/auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2719 2023-06-19 20:17:49.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/logic/schema.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 11:16:21.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/logic/validators.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.963428 ckanext-editable-config-0.0.4/ckanext/editable_config/migration/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/ckanext/editable_config/migration/editable_config/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1834 2023-06-18 15:19:17.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/migration/editable_config/alembic.ini
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2148 2023-06-18 20:14:29.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/migration/editable_config/env.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2023-06-18 15:19:17.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/migration/editable_config/script.py.mako
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/ckanext/editable_config/migration/editable_config/versions/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      655 2023-06-18 19:08:06.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/migration/editable_config/versions/a8d116986c3f_create_editable_config_table.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/ckanext/editable_config/model/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       49 2023-06-18 19:08:06.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/model/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2492 2023-07-25 21:26:13.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/model/option.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4544 2023-07-28 21:56:38.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4130 2023-07-28 22:49:10.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/shared.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.963428 ckanext-editable-config-0.0.4/ckanext/editable_config/templates/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/ckanext/editable_config/templates/admin/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      680 2023-07-28 16:20:12.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/templates/admin/base.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/ckanext/editable_config/templates/editable_config/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2307 2023-07-28 22:25:24.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/templates/editable_config/config.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/ckanext/editable_config/templates/editable_config/snippets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1033 2023-07-28 22:23:30.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/templates/editable_config/snippets/field.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/ckanext/editable_config/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1528 2023-07-25 22:45:15.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/tests/conftest.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/ckanext/editable_config/tests/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 20:35:03.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/tests/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5025 2023-07-25 23:02:01.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/tests/logic/test_action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      750 2023-06-19 12:49:49.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/tests/logic/test_schema.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/ckanext/editable_config/tests/model/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 21:22:56.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/tests/model/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3473 2023-06-19 20:17:49.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/tests/model/test_option.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1609 2023-06-19 20:17:42.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/tests/test_fixtures.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 19:08:32.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/tests/test_plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3444 2023-07-25 22:45:46.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/tests/test_shared.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1830 2023-07-28 22:26:11.000000 ckanext-editable-config-0.0.4/ckanext/editable_config/views.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-07-28 22:50:04.973429 ckanext-editable-config-0.0.4/ckanext_editable_config.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    12795 2023-07-28 22:50:04.000000 ckanext-editable-config-0.0.4/ckanext_editable_config.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2019 2023-07-28 22:50:04.000000 ckanext-editable-config-0.0.4/ckanext_editable_config.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-07-28 22:50:04.000000 ckanext-editable-config-0.0.4/ckanext_editable_config.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      142 2023-07-28 22:50:04.000000 ckanext-editable-config-0.0.4/ckanext_editable_config.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-07-28 22:50:04.000000 ckanext-editable-config-0.0.4/ckanext_editable_config.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-07-28 22:50:04.000000 ckanext-editable-config-0.0.4/ckanext_editable_config.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4324 2023-06-18 20:58:41.000000 ckanext-editable-config-0.0.4/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2023-06-18 11:13:48.000000 ckanext-editable-config-0.0.4/requirements.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1691 2023-07-28 22:50:04.983430 ckanext-editable-config-0.0.4/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)      505 2023-06-18 19:08:08.000000 ckanext-editable-config-0.0.4/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 09:21:03.414174 ckanext_editable_config-0.0.5/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      215 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    12962 2024-04-24 09:21:03.414174 ckanext_editable_config-0.0.5/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    12207 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 09:21:03.404174 ckanext_editable_config-0.0.5/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      202 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 09:21:03.404174 ckanext_editable_config-0.0.5/ckanext/editable_config/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 09:21:03.404174 ckanext_editable_config-0.0.5/ckanext/editable_config/assets/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 09:21:03.407508 ckanext_editable_config-0.0.5/ckanext/editable_config/assets/css/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       83 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/assets/css/editable_config.css
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 09:21:03.407508 ckanext_editable_config-0.0.5/ckanext/editable_config/assets/js/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      418 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/assets/js/editable-config-toggle-field.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      346 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/assets/webassets.yml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1211 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/config.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      636 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/helpers.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 09:21:03.407508 ckanext_editable_config-0.0.5/ckanext/editable_config/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6675 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/logic/action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1782 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/logic/auth.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2719 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/logic/schema.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/logic/validators.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 09:21:03.400841 ckanext_editable_config-0.0.5/ckanext/editable_config/migration/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 09:21:03.407508 ckanext_editable_config-0.0.5/ckanext/editable_config/migration/editable_config/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1834 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/migration/editable_config/alembic.ini
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2148 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/migration/editable_config/env.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/migration/editable_config/script.py.mako
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 09:21:03.407508 ckanext_editable_config-0.0.5/ckanext/editable_config/migration/editable_config/versions/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      655 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/migration/editable_config/versions/a8d116986c3f_create_editable_config_table.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 09:21:03.407508 ckanext_editable_config-0.0.5/ckanext/editable_config/model/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       49 2024-01-28 13:50:18.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/model/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2729 2024-01-30 22:02:21.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/model/option.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3253 2024-01-28 13:52:55.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7059 2024-01-28 13:30:54.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/shared.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 09:21:03.400841 ckanext_editable_config-0.0.5/ckanext/editable_config/templates/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 09:21:03.407508 ckanext_editable_config-0.0.5/ckanext/editable_config/templates/admin/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      680 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/templates/admin/base.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 09:21:03.407508 ckanext_editable_config-0.0.5/ckanext/editable_config/templates/editable_config/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2559 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/templates/editable_config/config.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 09:21:03.410841 ckanext_editable_config-0.0.5/ckanext/editable_config/templates/editable_config/snippets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1033 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/templates/editable_config/snippets/field.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 09:21:03.410841 ckanext_editable_config-0.0.5/ckanext/editable_config/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1394 2024-01-28 13:37:26.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/tests/conftest.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 09:21:03.410841 ckanext_editable_config-0.0.5/ckanext/editable_config/tests/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/tests/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5005 2024-01-28 13:37:47.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/tests/logic/test_action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      750 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/tests/logic/test_schema.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 09:21:03.410841 ckanext_editable_config-0.0.5/ckanext/editable_config/tests/model/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/tests/model/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3469 2024-01-28 13:37:35.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/tests/model/test_option.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1519 2024-01-28 13:37:53.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/tests/test_fixtures.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/tests/test_plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3440 2024-01-28 13:37:31.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/tests/test_shared.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1830 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/ckanext/editable_config/views.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 09:21:03.414174 ckanext_editable_config-0.0.5/ckanext_editable_config.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    12962 2024-04-24 09:21:03.000000 ckanext_editable_config-0.0.5/ckanext_editable_config.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2038 2024-04-24 09:21:03.000000 ckanext_editable_config-0.0.5/ckanext_editable_config.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-04-24 09:21:03.000000 ckanext_editable_config-0.0.5/ckanext_editable_config.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      142 2024-04-24 09:21:03.000000 ckanext_editable_config-0.0.5/ckanext_editable_config.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-04-24 09:21:03.000000 ckanext_editable_config-0.0.5/ckanext_editable_config.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       53 2024-04-24 09:21:03.000000 ckanext_editable_config-0.0.5/ckanext_editable_config.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-04-24 09:21:03.000000 ckanext_editable_config-0.0.5/ckanext_editable_config.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4421 2024-01-28 13:50:25.000000 ckanext_editable_config-0.0.5/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/requirements.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1738 2024-04-24 09:21:03.414174 ckanext_editable_config-0.0.5/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      505 2024-01-26 15:10:52.000000 ckanext_editable_config-0.0.5/setup.py
```

### Comparing `ckanext-editable-config-0.0.4/LICENSE` & `ckanext_editable_config-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.4/PKG-INFO` & `ckanext_editable_config-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: ckanext-editable-config
-Version: 0.0.4
-Home-page: https://github.com/DataShades/ckanext-editable-config
+Version: 0.0.5
+Home-page: https://github.com/ckan/ckanext-editable-config
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: test
+Requires-Dist: pytest-ckan; extra == "test"
+Provides-Extra: dev
+Requires-Dist: pytest-ckan; extra == "dev"
+Requires-Dist: git-changelog; extra == "dev"
 
 [![Tests](https://github.com/DataShades/ckanext-editable-config/workflows/Tests/badge.svg?branch=main)](https://github.com/DataShades/ckanext-editable-config/actions)
 
 # ckanext-editable-config
 
 Edit CKAN configuration in runtime.
```

### Comparing `ckanext-editable-config-0.0.4/README.md` & `ckanext_editable_config-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.4/ckanext/editable_config/config.py` & `ckanext_editable_config-0.0.5/ckanext/editable_config/config.py`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.4/ckanext/editable_config/helpers.py` & `ckanext_editable_config-0.0.5/ckanext/editable_config/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.4/ckanext/editable_config/logic/action.py` & `ckanext_editable_config-0.0.5/ckanext/editable_config/logic/action.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from typing_extensions import TypedDict
 
 import ckan.plugins.toolkit as tk
 from ckan import types
 from ckan.common import CKANConfig
 from ckan.common import config_declaration as cd
-from ckan.config.declaration import Key
 from ckan.config.declaration.option import Flag
 from ckan.logic import validate
 
 from ckanext.editable_config import shared
 from ckanext.editable_config.model import Option
 
 from . import schema
@@ -130,15 +129,16 @@
     if data_dict["apply"]:
         shared.apply_config_overrides()
 
     return result
 
 
 def _make_option(key: str, value: Any):
-    if key not in cd or not cd[Key.from_string(key)].has_flag(Flag.editable):
+    option = shared.get_declaration(key)
+    if not option or not option.has_flag(Flag.editable):
         raise tk.ValidationError({key: ["Not editable"]})
 
     _, errors = cd.validate(CKANConfig(tk.config, **{key: value}))
     if errors:
         raise tk.ValidationError(errors)
 
     return Option.set(key, value)
```

### Comparing `ckanext-editable-config-0.0.4/ckanext/editable_config/logic/auth.py` & `ckanext_editable_config-0.0.5/ckanext/editable_config/logic/auth.py`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.4/ckanext/editable_config/logic/schema.py` & `ckanext_editable_config-0.0.5/ckanext/editable_config/logic/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.4/ckanext/editable_config/migration/editable_config/alembic.ini` & `ckanext_editable_config-0.0.5/ckanext/editable_config/migration/editable_config/alembic.ini`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.4/ckanext/editable_config/migration/editable_config/env.py` & `ckanext_editable_config-0.0.5/ckanext/editable_config/migration/editable_config/env.py`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.4/ckanext/editable_config/migration/editable_config/versions/a8d116986c3f_create_editable_config_table.py` & `ckanext_editable_config-0.0.5/ckanext/editable_config/migration/editable_config/versions/a8d116986c3f_create_editable_config_table.py`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.4/ckanext/editable_config/model/option.py` & `ckanext_editable_config-0.0.5/ckanext/editable_config/model/option.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,49 @@
 from __future__ import annotations
 
 from datetime import datetime
 from typing import Any, cast
 
 import sqlalchemy as sa
+from sqlalchemy.orm import Mapped
 from typing_extensions import Self
 
 import ckan.plugins.toolkit as tk
 from ckan import model, types
 from ckan.lib.dictization import table_dictize
 
 from ckanext.editable_config import shared
 
 
-class Option(tk.BaseModel):
-    __tablename__ = "editable_config_option"
-
-    key = sa.Column(sa.Text, primary_key=True)
-    value = sa.Column(sa.Text, nullable=False)
-    updated_at = sa.Column(sa.DateTime, nullable=False)
-    prev_value = sa.Column(sa.Text, nullable=False)
+class Option(tk.BaseModel):  # pyright: ignore[reportUntypedBaseClass]
+    __table__ = sa.Table(
+        "editable_config_option",
+        tk.BaseModel.metadata,
+        sa.Column("key", sa.Text, primary_key=True),
+        sa.Column("value", sa.Text, nullable=False),
+        sa.Column("updated_at", sa.DateTime, nullable=False),
+        sa.Column("prev_value", sa.Text, nullable=False),
+    )
+
+    key: Mapped[str]
+    value: Mapped[str]
+    updated_at: Mapped[datetime]
+    prev_value: Mapped[str]
 
     @classmethod
     def get(cls, key: str) -> Self | None:
         """Search for option."""
         return cast(
             Self,
             model.Session.get(cls, key),
         )
 
     @classmethod
     def set(cls, key: str, value: Any) -> Self:
         """Create/update an option."""
-        option: Self
         safe_value = shared.value_as_string(key, value)
 
         if option := cls.get(key):
             option.value = safe_value
         else:
             option = cls(key=key, value=safe_value)
```

### Comparing `ckanext-editable-config-0.0.4/ckanext/editable_config/templates/admin/base.html` & `ckanext_editable_config-0.0.5/ckanext/editable_config/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.4/ckanext/editable_config/templates/editable_config/config.html` & `ckanext_editable_config-0.0.5/ckanext/editable_config/templates/editable_config/config.html`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 } %}
 
 {% block scripts %}
     {{ super() }}
     {% asset "editable_config/editable_config-js" %}
 {% endblock scripts %}
 
+{% block styles %}
+    {{ super() }}
+    {% asset "editable_config/editable_config-css" %}
+{% endblock styles %}
+
+
 {% block primary_content_inner %}
     {% block form %}
 
         {% block errors %}
             {{ form.errors(error_summary) }}
         {% endblock errors %}
 
@@ -60,15 +66,18 @@
             {% endblock sidebar_heading %}
         </h2>
 
         <div class="module-content">
             {% block sidebar_content %}
                 {% for name in options %}
                     <p>
-                        <label for="{{ "field-value-" ~ name.replace(".", "-") }}">
+                        <label
+                            class="editable-option-help--key"
+                            title="{{ name }}"
+                            for="{{ "field-value-" ~ name.replace(".", "-") }}">
                             {{ name }}
                         </label>
                         {{ h.render_markdown(h.editable_config_option_description(name), allow_html=true) }}
                     </p>
                 {% endfor %}
             {% endblock sidebar_content %}
         </div>
```

### Comparing `ckanext-editable-config-0.0.4/ckanext/editable_config/templates/editable_config/snippets/field.html` & `ckanext_editable_config-0.0.5/ckanext/editable_config/templates/editable_config/snippets/field.html`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.4/ckanext/editable_config/tests/conftest.py` & `ckanext_editable_config-0.0.5/ckanext/editable_config/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,31 +5,24 @@
 
 import pytest
 from pytest_factoryboy import register
 
 from ckan import model
 from ckan.tests import factories
 from ckan.tests.helpers import call_action
-
 from ckanext.editable_config.model import Option
 from ckanext.editable_config.shared import apply_config_overrides
 
 
 @pytest.fixture(autouse=True)
 def reset_last_check():
     """Remove freezetime dates in future from config_overrides."""
     apply_config_overrides._last_check = None
 
 
-@pytest.fixture(scope="session")
-def reset_db_once(reset_db, migrate_db_for):
-    reset_db()
-    migrate_db_for("editable_config")
-
-
 @pytest.fixture()
 def clean_db(reset_db, migrate_db_for):
     reset_db()
     migrate_db_for("editable_config")
 
 
 @register
```

### Comparing `ckanext-editable-config-0.0.4/ckanext/editable_config/tests/logic/test_action.py` & `ckanext_editable_config-0.0.5/ckanext/editable_config/tests/logic/test_action.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 import ckan.plugins.toolkit as tk
 from ckan.tests.helpers import call_action
 
 from ckanext.editable_config import config, shared
 
 
 @pytest.mark.ckan_config(config.WHITELIST, ["ckan.site_title", "ckan.site_description"])
-@pytest.mark.usefixtures("with_plugins", "non_clean_db")
+@pytest.mark.usefixtures("with_plugins", "clean_db")
 class TestList:
     def test_default(self):
         result = call_action("editable_config_list")
         assert set(result) == {"ckan.site_title", "ckan.site_description"}
 
     def test_pattern(self):
         result = call_action("editable_config_list", pattern="*title")
         assert set(result) == {"ckan.site_title"}
 
 
-@pytest.mark.usefixtures("with_plugins", "non_clean_db", "with_autoclean")
+@pytest.mark.usefixtures("with_plugins", "clean_db", "with_autoclean")
 class TestUpdate:
     def test_empty(self):
         result = call_action("editable_config_update")
         assert not any(v for v in result.values())
         assert shared.apply_config_overrides() == 0
 
     def test_one_per_group(self, faker, option_factory, ckan_config):
@@ -46,15 +46,15 @@
             ckan_config["ckan.site_title"]
             == result["change"]["ckan.site_title"]["value"]
         )
         assert ckan_config[revert_option["key"]] == revert_option["prev_value"]
         assert ckan_config[reset_option["key"]] is None
 
 
-@pytest.mark.usefixtures("with_plugins", "non_clean_db", "with_autoclean")
+@pytest.mark.usefixtures("with_plugins", "clean_db", "with_autoclean")
 class TestChange:
     def test_undeclared(self, option_factory, faker):
         """Undeclared options are not allowed."""
         with pytest.raises(tk.ValidationError):
             call_action("editable_config_change", options={faker.word(): faker.word()})
 
     def test_not_editable(self, option_factory, faker):
@@ -94,15 +94,15 @@
             )
         call_action(
             "editable_config_change",
             options={"ckan.datasets_per_page": 1},
         )
 
 
-@pytest.mark.usefixtures("with_plugins", "non_clean_db", "with_autoclean")
+@pytest.mark.usefixtures("with_plugins", "clean_db", "with_autoclean")
 class TestRevert:
     def test_revert_missing(self):
         with pytest.raises(tk.ObjectNotFound):
             call_action("editable_config_revert", keys=["ckan.site_title"])
 
     def test_revert_initial(self, ckan_config, faker, option_factory):
         initial = ckan_config["ckan.site_title"]
@@ -110,15 +110,15 @@
         option_factory(key="ckan.site_title", value=updated)
 
         result = call_action("editable_config_revert", keys=["ckan.site_title"])
         assert result["ckan.site_title"]["value"] == initial
         assert result["ckan.site_title"]["prev_value"] == updated
 
 
-@pytest.mark.usefixtures("with_plugins", "non_clean_db", "with_autoclean")
+@pytest.mark.usefixtures("with_plugins", "clean_db", "with_autoclean")
 class TestReset:
     def test_reset_missing(self):
         with pytest.raises(tk.ObjectNotFound):
             call_action("editable_config_reset", keys=["ckan.site_title"])
 
     def test_resert_initial(self, ckan_config, faker, option_factory):
         initial = ckan_config["ckan.site_title"]
```

### Comparing `ckanext-editable-config-0.0.4/ckanext/editable_config/tests/logic/test_schema.py` & `ckanext_editable_config-0.0.5/ckanext/editable_config/tests/logic/test_schema.py`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.4/ckanext/editable_config/tests/model/test_option.py` & `ckanext_editable_config-0.0.5/ckanext/editable_config/tests/model/test_option.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from unittest.mock import ANY
 
 import pytest
 
 from ckanext.editable_config.model import Option
 
 
-@pytest.mark.usefixtures("with_plugins", "non_clean_db")
+@pytest.mark.usefixtures("with_plugins", "clean_db")
 class TestOption:
     def test_get(self, faker, option_factory):
         """Option.get returns exition option or None."""
         with option_factory.autoclean(key="ckan.site_title", value=faker.word()):
             assert Option.get("ckan.site_title")
 
         assert Option.get("ckan.site_title") is None
```

### Comparing `ckanext-editable-config-0.0.4/ckanext/editable_config/tests/test_fixtures.py` & `ckanext_editable_config-0.0.5/ckanext/editable_config/tests/test_fixtures.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 from __future__ import annotations
 
 from unittest.mock import ANY
 
 import pytest
 
 import ckan.plugins.toolkit as tk
-from ckan.common import config_declaration as cd
 
 
-@pytest.mark.usefixtures("with_plugins", "non_clean_db")
+@pytest.mark.usefixtures("with_plugins", "clean_db")
 class TestOptionFactory:
     def test_key_and_value_required(self, option_factory):
         """OptionFactory requires key and value."""
         with pytest.raises(tk.ValidationError) as e:
             option_factory()
 
         assert "key" in e.value.error_dict
         assert "value" in e.value.error_dict
 
     def test_key_cannot_be_undeclared(self, option_factory, faker):
         """Undeclared options are not allowed."""
-        while (key := faker.word()) in cd:
-            continue
+        key = faker.word()
 
         with pytest.raises(tk.ValidationError) as e:
             option_factory(key=key, value=faker.word())
 
         assert e.value.error_dict == {key: [ANY]}
 
     def test_key_must_be_editable(self, option_factory, faker):
```

### Comparing `ckanext-editable-config-0.0.4/ckanext/editable_config/tests/test_shared.py` & `ckanext_editable_config-0.0.5/ckanext/editable_config/tests/test_shared.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 @pytest.mark.ckan_config("ckan.plugins", ["text_view", "image_view"])
 def test_value_as_string():
     assert shared.value_as_string("ckan.site_title", 123) == "123"
     assert shared.value_as_string("ckan.requests.timeout", 123) == "123"
     assert shared.value_as_string("ckan.plugins", ["hello", "world"]) == "hello world"
 
 
-@pytest.mark.usefixtures("with_plugins", "non_clean_db")
+@pytest.mark.usefixtures("with_plugins", "clean_db")
 class TestUpdater:
     def test_apply_new_updates(self, faker, ckan_config, freezer, autoclean_option):
         """New updates are applied."""
         freezer.move_to(timedelta(seconds=1))
         key = autoclean_option["key"]
         value = faker.sentence()
```

### Comparing `ckanext-editable-config-0.0.4/ckanext/editable_config/views.py` & `ckanext_editable_config-0.0.5/ckanext/editable_config/views.py`

 * *Files identical despite different names*

### Comparing `ckanext-editable-config-0.0.4/ckanext_editable_config.egg-info/PKG-INFO` & `ckanext_editable_config-0.0.5/ckanext_editable_config.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: ckanext-editable-config
-Version: 0.0.4
-Home-page: https://github.com/DataShades/ckanext-editable-config
+Version: 0.0.5
+Home-page: https://github.com/ckan/ckanext-editable-config
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: test
+Requires-Dist: pytest-ckan; extra == "test"
+Provides-Extra: dev
+Requires-Dist: pytest-ckan; extra == "dev"
+Requires-Dist: git-changelog; extra == "dev"
 
 [![Tests](https://github.com/DataShades/ckanext-editable-config/workflows/Tests/badge.svg?branch=main)](https://github.com/DataShades/ckanext-editable-config/actions)
 
 # ckanext-editable-config
 
 Edit CKAN configuration in runtime.
```

### Comparing `ckanext-editable-config-0.0.4/ckanext_editable_config.egg-info/SOURCES.txt` & `ckanext_editable_config-0.0.5/ckanext_editable_config.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,16 @@
 ckanext/__init__.py
 ckanext/editable_config/__init__.py
 ckanext/editable_config/config.py
 ckanext/editable_config/helpers.py
 ckanext/editable_config/plugin.py
 ckanext/editable_config/shared.py
 ckanext/editable_config/views.py
-ckanext/editable_config/assets/script.js
-ckanext/editable_config/assets/style.css
 ckanext/editable_config/assets/webassets.yml
+ckanext/editable_config/assets/css/editable_config.css
 ckanext/editable_config/assets/js/editable-config-toggle-field.js
 ckanext/editable_config/logic/__init__.py
 ckanext/editable_config/logic/action.py
 ckanext/editable_config/logic/auth.py
 ckanext/editable_config/logic/schema.py
 ckanext/editable_config/logic/validators.py
 ckanext/editable_config/migration/editable_config/alembic.ini
@@ -41,8 +40,9 @@
 ckanext/editable_config/tests/model/__init__.py
 ckanext/editable_config/tests/model/test_option.py
 ckanext_editable_config.egg-info/PKG-INFO
 ckanext_editable_config.egg-info/SOURCES.txt
 ckanext_editable_config.egg-info/dependency_links.txt
 ckanext_editable_config.egg-info/entry_points.txt
 ckanext_editable_config.egg-info/namespace_packages.txt
+ckanext_editable_config.egg-info/requires.txt
 ckanext_editable_config.egg-info/top_level.txt
```

### Comparing `ckanext-editable-config-0.0.4/pyproject.toml` & `ckanext_editable_config-0.0.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,19 @@
 addopts = "--ckan-ini test.ini"
 filterwarnings = [
                "ignore::sqlalchemy.exc.SADeprecationWarning",
                "ignore::sqlalchemy.exc.SAWarning",
                "ignore::DeprecationWarning",
 ]
 
+[tool.git-changelog]
+output = "CHANGELOG.md"
+convention = "conventional"
+parse-trailers = true
+
 [tool.pyright]
 pythonVersion = "3.8"
 include = ["ckanext"]
 exclude = [
     "**/test*",
     "**/migration",
 ]
@@ -72,15 +77,15 @@
 
 # Check the meaning of rules here
 # https://github.com/microsoft/pyright/blob/main/docs/configuration.md
 reportFunctionMemberAccess = true # non-standard member accesses for functions
 reportMissingImports = true
 reportMissingModuleSource = true
 reportMissingTypeStubs = false
-reportImportCycles = true
+reportImportCycles = false
 reportUnusedImport = true
 reportUnusedClass = true
 reportUnusedFunction = true
 reportUnusedVariable = true
 reportDuplicateImport = true
 reportOptionalSubscript = true
 reportOptionalMemberAccess = true
```

### Comparing `ckanext-editable-config-0.0.4/setup.cfg` & `ckanext_editable_config-0.0.5/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = ckanext-editable-config
-version = 0.0.4
+version = 0.0.5
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/DataShades/ckanext-editable-config
+url = https://github.com/ckan/ckanext-editable-config
 author = Sergey Motornyuk
 author_email = sergey.motornyuk@linkdigital.com.au
 license = AGPL
 classifiers = 
 	Development Status :: 4 - Beta
 	License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 	Programming Language :: Python :: 3.8
@@ -25,14 +25,19 @@
 [options.entry_points]
 ckan.plugins = 
 	editable_config = ckanext.editable_config.plugin:EditableConfigPlugin
 babel.extractors = 
 	ckan = ckan.lib.extract:extract_ckan
 
 [options.extras_require]
+test = 
+	pytest-ckan
+dev = 
+	%(test)s
+	git-changelog
 
 [extract_messages]
 keywords = translate isPlural
 add_comments = TRANSLATORS:
 output_file = ckanext/editable_config/i18n/ckanext-editable_config.pot
 width = 80
```

