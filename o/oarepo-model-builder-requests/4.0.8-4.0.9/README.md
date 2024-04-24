# Comparing `tmp/oarepo-model-builder-requests-4.0.8.tar.gz` & `tmp/oarepo-model-builder-requests-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-requests-4.0.8.tar", last modified: Wed Nov  1 14:00:25 2023, max compression
+gzip compressed data, was "oarepo-model-builder-requests-4.0.9.tar", last modified: Fri Nov 10 17:16:09 2023, max compression
```

## Comparing `oarepo-model-builder-requests-4.0.8.tar` & `oarepo-model-builder-requests-4.0.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 14:00:25.259882 oarepo-model-builder-requests-4.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2023-11-01 14:00:25.259882 oarepo-model-builder-requests-4.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 14:00:25.215881 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 14:00:25.223881 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/datatypes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/datatypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 14:00:25.223881 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/datatypes/components/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/datatypes/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 14:00:25.231881 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/datatypes/components/requests_model/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/datatypes/components/requests_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/datatypes/components/requests_model/parent_marshmallow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6034 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/datatypes/components/requests_model/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/datatypes/components/requests_model/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 14:00:25.247882 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/invenio_requests_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/invenio_requests_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/invenio_requests_parent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/invenio_requests_parent_marshmallow.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/invenio_requests_parent_marshmallow_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/invenio_requests_parent_marshmallow_link_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/invenio_requests_parent_marshmallow_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/invenio_requests_resolvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/invenio_requests_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/invenio_requests_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/invenio_requests_views_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/requests_setup_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 14:00:25.255882 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/templates/actions.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      693 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/templates/config.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      282 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/templates/parent.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/templates/parent_marshmallow.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/templates/parent_marshmallow_link.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      723 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/templates/resolvers.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/templates/types.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      443 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/templates/views.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 14:00:25.255882 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/tests/invenio_requests_conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/tests/invenio_requests_test_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 14:00:25.259882 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/tests/templates/conftest.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/tests/templates/test_requests.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 14:00:25.219881 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2023-11-01 14:00:25.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2023-11-01 14:00:25.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-01 14:00:25.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2023-11-01 14:00:25.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-11-01 14:00:25.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-11-01 14:00:25.000000 oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2023-11-01 14:00:25.259882 oarepo-model-builder-requests-4.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-01 13:55:28.000000 oarepo-model-builder-requests-4.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 17:16:09.346479 oarepo-model-builder-requests-4.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2023-11-10 17:16:09.346479 oarepo-model-builder-requests-4.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 17:16:09.314478 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 17:16:09.314478 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 17:16:09.314478 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/datatypes/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/datatypes/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 17:16:09.322478 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/datatypes/components/requests_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/datatypes/components/requests_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/datatypes/components/requests_model/parent_marshmallow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6358 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/datatypes/components/requests_model/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/datatypes/components/requests_model/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 17:16:09.334478 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/invenio_requests_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/invenio_requests_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/invenio_requests_parent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/invenio_requests_parent_marshmallow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/invenio_requests_parent_marshmallow_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/invenio_requests_parent_marshmallow_link_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/invenio_requests_parent_marshmallow_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/invenio_requests_resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/invenio_requests_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/invenio_requests_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/invenio_requests_views_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/requests_setup_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 17:16:09.338479 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/templates/actions.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/templates/config.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/templates/parent.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/templates/parent_marshmallow.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/templates/parent_marshmallow_link.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/templates/resolvers.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/templates/types.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/templates/views.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 17:16:09.342479 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/tests/invenio_requests_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/tests/invenio_requests_test_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 17:16:09.346479 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/tests/templates/conftest.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/tests/templates/test_requests.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-10 17:16:09.314478 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2023-11-10 17:16:09.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2023-11-10 17:16:09.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-10 17:16:09.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2023-11-10 17:16:09.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2023-11-10 17:16:09.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2023-11-10 17:16:09.000000 oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2023-11-10 17:16:09.346479 oarepo-model-builder-requests-4.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-10 17:11:28.000000 oarepo-model-builder-requests-4.0.9/setup.py
```

### Comparing `oarepo-model-builder-requests-4.0.8/LICENSE` & `oarepo-model-builder-requests-4.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-requests-4.0.8/PKG-INFO` & `oarepo-model-builder-requests-4.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-requests
-Version: 4.0.8
+Version: 4.0.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: oarepo-model-builder
 Requires-Dist: oarepo-model-builder-tests
 Provides-Extra: tests
 Requires-Dist: pytest-invenio>=1.4.11; extra == "tests"
```

### Comparing `oarepo-model-builder-requests-4.0.8/README.md` & `oarepo-model-builder-requests-4.0.9/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/datatypes/components/requests_model/parent_marshmallow.py` & `oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/datatypes/components/requests_model/parent_marshmallow.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import marshmallow as ma
 from oarepo_model_builder.datatypes import DataTypeComponent, ModelDataType
-from oarepo_model_builder.datatypes.components.model.utils import set_default, append_array
+from oarepo_model_builder.datatypes.components import (
+    DefaultsModelComponent,
+    MarshmallowModelComponent,
+)
+from oarepo_model_builder.datatypes.components.model.utils import set_default
 from oarepo_model_builder.validation.utils import ImportSchema
-from oarepo_model_builder.datatypes.components import DefaultsModelComponent, MarshmallowModelComponent
-
 
 
 class ParentMarshmallowClassSchema(ma.Schema):
     module = ma.fields.String(metadata={"doc": "Class module"})
     class_ = ma.fields.String(
         attribute="class",
         data_key="class",
@@ -19,24 +21,32 @@
         data_key="base-classes",
         metadata={"doc": "base classes"},
     )
     imports = ma.fields.List(
         ma.fields.Nested(ImportSchema), metadata={"doc": "List of python imports"}
     )
 
+
 class ParentMarshmallowComponent(DataTypeComponent):
     eligible_datatypes = [ModelDataType]
     depends_on = [DefaultsModelComponent, MarshmallowModelComponent]
 
     class ModelSchema(ma.Schema):
         parent_record_marshmallow = ma.fields.Nested(
             ParentMarshmallowClassSchema,
             attribute="parent-record-marshmallow",
             data_key="parent-record-marshmallow",
         )
 
     def before_model_prepare(self, datatype, *, context, **kwargs):
         marshmallow = set_default(datatype, "parent-record-marshmallow", {})
-        m_module = marshmallow.setdefault("module", datatype.definition["marshmallow"]["module"])
+        m_module = marshmallow.setdefault(
+            "module", datatype.definition["marshmallow"]["module"]
+        )
         marshmallow.setdefault("class", f"{m_module}.GeneratedParentSchema")
         marshmallow.setdefault("generate", True)
-        marshmallow.setdefault("base-classes", ["invenio_drafts_resources.services.records.schema.ParentSchema{InvenioParentSchema}"])
+        marshmallow.setdefault(
+            "base-classes",
+            [
+                "invenio_drafts_resources.services.records.schema.ParentSchema{InvenioParentSchema}"
+            ],
+        )
```

### Comparing `oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/datatypes/components/requests_model/requests.py` & `oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/datatypes/components/requests_model/requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import marshmallow as ma
 from oarepo_model_builder.datatypes import DataTypeComponent, ModelDataType
 from oarepo_model_builder.datatypes.components import (
     DefaultsModelComponent,
     MarshmallowModelComponent,
 )
-from oarepo_model_builder.datatypes.components.model.utils import (
-    set_default,
-    append_array,
-)
+from oarepo_model_builder.datatypes.components.model.utils import set_default
 from oarepo_model_builder.utils.camelcase import camel_case, snake_case
 from oarepo_model_builder.validation.utils import ImportSchema
 
 
 class RequestActionSchema(ma.Schema):
     class Meta:
         unknown = ma.RAISE
@@ -49,14 +46,25 @@
         attribute="base-classes",
         data_key="base-classes",
         metadata={"doc": "RequestType base classes"},
     )
     imports = ma.fields.List(
         ma.fields.Nested(ImportSchema), metadata={"doc": "List of python imports"}
     )
+    allowed_receiver_ref_types = ma.fields.List(
+        ma.fields.String,
+        attribute="allowed-receiver-ref-types",
+        data_key="allowed-receiver-ref-types",
+    )
+    needs_context = ma.fields.Dict(
+        keys=ma.fields.String,
+        values=ma.fields.String,
+        attribute="needs-context",
+        data_key="needs-context",
+    )
     id_ = ma.fields.String(attribute="id", data_key="id")
 
 
 class ParentMarshmallowSchema(ma.Schema):
     module = ma.fields.String(metadata={"doc": "Class module"})
     class_ = ma.fields.String(
         attribute="class",
```

### Comparing `oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/datatypes/components/requests_model/resolver.py` & `oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/datatypes/components/requests_model/resolver.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/invenio_requests_actions.py` & `oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/invenio_requests_actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 class InvenioRequestsActionsBuilder(InvenioBaseClassPythonBuilder):
     TYPE = "invenio_requests_actions"
     section = "requests"
     template = "requests-actions"
     skip_if_not_generating = False
 
     def finish(self, **extra_kwargs):
-        super(InvenioBaseClassPythonBuilder, self).finish() # calls super().finish() of InvenioBaseClassPythonBuilder
+        super(
+            InvenioBaseClassPythonBuilder, self
+        ).finish()  # calls super().finish() of InvenioBaseClassPythonBuilder
         if not self.generate:
             return
         vars = self.vars
 
         for request in vars["requests"].values():
             for action in request["actions"].values():
                 if not action["generate"]:
```

### Comparing `oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/invenio_requests_parent.py` & `oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/invenio_requests_parent.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,20 +9,22 @@
     section = "requests"
     template = "requests-parent-field"
 
     def finish(self, **extra_kwargs):
         if "draft-parent-record" not in self.current_model.definition:
             return
 
-        super(InvenioBaseClassPythonBuilder, self).finish() # calls super().finish() of InvenioBaseClassPythonBuilder
+        super(
+            InvenioBaseClassPythonBuilder, self
+        ).finish()  # calls super().finish() of InvenioBaseClassPythonBuilder
         vars = self.vars
         module = self.current_model.definition["draft-parent-record"]["module"]
         python_path = Path(module_to_path(module) + ".py")
         for request_name in vars["requests"]:
             self.process_template(
                 python_path,
                 self.template,
                 current_module=module,
                 vars=vars,
                 request_name=request_name.replace("-", "_"),
                 **extra_kwargs,
-            )
+            )
```

### Comparing `oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/invenio_requests_parent_marshmallow.py` & `oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/invenio_requests_parent_marshmallow.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,17 @@
     def get_marshmallow_module(self):
         return self.current_model.definition["marshmallow"]["module"]
 
     def finish(self, **extra_kwargs):
         if "draft-parent-record" not in self.current_model.definition:
             return
 
-        super(InvenioBaseClassPythonBuilder, self).finish() # calls super().finish() of InvenioBaseClassPythonBuilder
+        super(
+            InvenioBaseClassPythonBuilder, self
+        ).finish()  # calls super().finish() of InvenioBaseClassPythonBuilder
         vars = self.vars
         module = self.get_marshmallow_module()
         python_path = Path(module_to_path(module) + ".py")
         for request_name, request in vars["requests"].items():
             self.process_template(
                 python_path,
                 self.template,
```

### Comparing `oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/invenio_requests_parent_marshmallow_link.py` & `oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/invenio_requests_parent_marshmallow_link.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,12 +4,15 @@
 class InvenioRequestsParentMarshmallowLinkBuilder(InvenioBaseClassPythonBuilder):
     TYPE = "invenio_requests_parent_marshmallow_link"
     section = "parent-record-marshmallow"
     template = "requests-parent-marshmallow-link"
 
     def _get_marshmallow(self):
         return self.current_model.definition["marshmallow"]
+
     def finish(self, **extra_kwargs):
         # for now the ma schema for parent is generated only when requests are present
-        if "draft-parent-record" not in self.current_model.definition or getattr(self.current_model.definition, "requests", None):
+        if "draft-parent-record" not in self.current_model.definition or getattr(
+            self.current_model.definition, "requests", None
+        ):
             return
-        super().finish(marshmallow=self._get_marshmallow(), **extra_kwargs)
+        super().finish(marshmallow=self._get_marshmallow(), **extra_kwargs)
```

### Comparing `oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/invenio_requests_types.py` & `oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/invenio_requests_types.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 
 class InvenioRequestsTypesBuilder(InvenioBaseClassPythonBuilder):
     TYPE = "invenio_requests_types"
     section = "requests"
     template = "requests-types"
 
     def finish(self, **extra_kwargs):
-        super(InvenioBaseClassPythonBuilder, self).finish() # calls super().finish() of InvenioBaseClassPythonBuilder
+        super(
+            InvenioBaseClassPythonBuilder, self
+        ).finish()  # calls super().finish() of InvenioBaseClassPythonBuilder
         vars = self.vars
 
         for request_name, request in vars["requests"].items():
             if not request["type"]["generate"]:
                 continue
             module = request["type"]["module"]
             python_path = Path(module_to_path(module) + ".py")
```

### Comparing `oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/templates/actions.py.jinja2` & `oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/templates/actions.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/templates/config.py.jinja2` & `oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/templates/config.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/templates/parent_marshmallow.py.jinja2` & `oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/templates/parent_marshmallow.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/invenio/templates/resolvers.py.jinja2` & `oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/invenio/templates/resolvers.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/tests/templates/conftest.py.jinja2` & `oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/tests/templates/conftest.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests/tests/templates/test_requests.py.jinja2` & `oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests/tests/templates/test_requests.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests.egg-info/PKG-INFO` & `oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-requests
-Version: 4.0.8
+Version: 4.0.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: oarepo-model-builder
 Requires-Dist: oarepo-model-builder-tests
 Provides-Extra: tests
 Requires-Dist: pytest-invenio>=1.4.11; extra == "tests"
```

### Comparing `oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests.egg-info/SOURCES.txt` & `oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-requests-4.0.8/oarepo_model_builder_requests.egg-info/entry_points.txt` & `oarepo-model-builder-requests-4.0.9/oarepo_model_builder_requests.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-requests-4.0.8/setup.cfg` & `oarepo-model-builder-requests-4.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-requests
-version = 4.0.8
+version = 4.0.9
 description = 
 authors = Ronald Krist <krist@cesnet.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

