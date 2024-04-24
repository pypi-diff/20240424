# Comparing `tmp/oarepo-model-builder-drafts-4.0.8.tar.gz` & `tmp/oarepo-model-builder-drafts-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-drafts-4.0.8.tar", last modified: Mon Sep 25 20:29:32 2023, max compression
+gzip compressed data, was "oarepo-model-builder-drafts-4.0.9.tar", last modified: Tue Sep 26 08:29:17 2023, max compression
```

## Comparing `oarepo-model-builder-drafts-4.0.8.tar` & `oarepo-model-builder-drafts-4.0.9.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 20:29:32.698348 oarepo-model-builder-drafts-4.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2023-09-25 20:29:32.698348 oarepo-model-builder-drafts-4.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 20:29:32.682348 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 20:29:32.682348 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/builders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/builders/parent_jsonschema_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 20:29:32.682348 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 20:29:32.686348 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/draft.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 20:29:32.686348 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/draft_model/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/draft_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/draft_model/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     8271 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/draft_model/draft_parent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/draft_model/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/draft_model/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/draft_model/pid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/draft_model/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/draft_model/record_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/draft_model/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/draft_model/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/draft_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     6752 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/published_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/draft.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 20:29:32.690348 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/invenio_drafts_has_draft_checkfield.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/invenio_drafts_parent_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/invenio_drafts_parent_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/invenio_drafts_parent_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/invenio_drafts_proxies.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/invenio_drafts_published_api_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/invenio_drafts_published_app_views.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/invenio_drafts_published_invenio_ext_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/invenio_drafts_published_record_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/invenio_drafts_published_record_service_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/invenio_drafts_record_extra_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/invenio_drafts_record_metadata_extra_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/invenio_drafts_record_service_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/invenio_drafts_setup_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 20:29:32.694348 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_api_views_published.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      458 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_app_views_published.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      348 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_has_draft_checkfield.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      258 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_parent_metadata.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      481 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_parent_record.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      518 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_parent_state.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_proxies.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      877 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_published_ext_service.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_published_record_service.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_published_record_service_config.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      422 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_record_extra_fields.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      254 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_record_metadata_extra_fields.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      216 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_record_service_config.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 20:29:32.694348 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/profiles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/profiles/draft.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 20:29:32.698348 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/tests/invenio_drafts_conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/tests/invenio_drafts_test_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/tests/invenio_drafts_test_services.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 20:29:32.698348 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/tests/templates/invenio_conftest.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     9452 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/tests/templates/invenio_test_resources.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      754 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/tests/templates/invenio_test_services.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 20:29:32.682348 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2023-09-25 20:29:32.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2023-09-25 20:29:32.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 20:29:32.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2023-09-25 20:29:32.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-09-25 20:29:32.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-09-25 20:29:32.000000 oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2023-09-25 20:29:32.698348 oarepo-model-builder-drafts-4.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-25 20:25:34.000000 oarepo-model-builder-drafts-4.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 08:29:17.646119 oarepo-model-builder-drafts-4.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2023-09-26 08:29:17.646119 oarepo-model-builder-drafts-4.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 08:29:17.622119 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 08:29:17.622119 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/builders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/builders/parent_jsonschema_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 08:29:17.622119 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 08:29:17.626119 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5249 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/draft.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 08:29:17.630119 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/draft_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/draft_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/draft_model/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8271 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/draft_model/draft_parent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/draft_model/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/draft_model/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/draft_model/pid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/draft_model/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/draft_model/record_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/draft_model/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/draft_model/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/draft_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6752 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/published_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/draft.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 08:29:17.638119 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/invenio_drafts_has_draft_checkfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/invenio_drafts_parent_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/invenio_drafts_parent_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/invenio_drafts_parent_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/invenio_drafts_proxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/invenio_drafts_published_api_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/invenio_drafts_published_app_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/invenio_drafts_published_invenio_ext_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/invenio_drafts_published_record_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/invenio_drafts_published_record_service_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/invenio_drafts_record_extra_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/invenio_drafts_record_metadata_extra_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/invenio_drafts_record_service_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/invenio_drafts_setup_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 08:29:17.642119 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_api_views_published.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_app_views_published.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_has_draft_checkfield.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_parent_metadata.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_parent_record.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_parent_state.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_proxies.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_published_ext_service.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_published_record_service.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_published_record_service_config.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_record_extra_fields.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_record_metadata_extra_fields.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_record_service_config.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 08:29:17.642119 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/profiles/draft.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 08:29:17.646119 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/tests/invenio_drafts_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/tests/invenio_drafts_test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/tests/invenio_drafts_test_services.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 08:29:17.646119 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/tests/templates/invenio_conftest.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     9452 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/tests/templates/invenio_test_resources.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/tests/templates/invenio_test_services.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 08:29:17.622119 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2023-09-26 08:29:17.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2023-09-26 08:29:17.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-26 08:29:17.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2023-09-26 08:29:17.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2023-09-26 08:29:17.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2023-09-26 08:29:17.000000 oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2023-09-26 08:29:17.646119 oarepo-model-builder-drafts-4.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-26 08:24:48.000000 oarepo-model-builder-drafts-4.0.9/setup.py
```

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/builders/parent_jsonschema_builder.py` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/builders/parent_jsonschema_builder.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/__init__.py` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/draft.py` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/draft.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                 ),
                 Link(
                     name="self_html",
                     link_class="ConditionalLink",
                     link_args=[
                         "cond=is_record",
                         f'if_=RecordLink("{{+ui}}{html_url_prefix}{{id}}")',
-                        'else_=RecordLink("{+ui}/uploads/{id}")',
+                        f'else_=RecordLink("{{+ui}}{html_url_prefix}{{id}}/edit")',
                     ],
                     imports=[
                         Import("invenio_records_resources.services.ConditionalLink"),
                         Import("invenio_records_resources.services.RecordLink"),
                         Import(
                             "invenio_drafts_resources.services.records.config.is_record"
                         ),
```

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/draft_model/__init__.py` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/draft_model/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/draft_model/defaults.py` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/draft_model/defaults.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/draft_model/draft_parent.py` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/draft_model/draft_parent.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/draft_model/jsonschema.py` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/draft_model/jsonschema.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/draft_model/mapping.py` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/draft_model/mapping.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/draft_model/pid.py` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/draft_model/pid.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/draft_model/record.py` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/draft_model/record.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/draft_model/record_metadata.py` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/draft_model/record_metadata.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/draft_model/resource.py` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/draft_model/resource.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/draft_model/service.py` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/draft_model/service.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/draft_tests.py` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/draft_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             "links": {
                 "draft": "https://{site_hostname}/api{BASE_URL}{pid_value}/draft",
                 "latest": "https://{site_hostname}/api{BASE_URL}{pid_value}/versions/latest",
                 "latest_html": "https://{site_hostname}{BASE_URL}{pid_value}/latest",
                 "publish": "https://{site_hostname}/api{BASE_URL}{pid_value}/draft/actions/publish",
                 "record": "https://{site_hostname}/api{BASE_URL}{pid_value}",
                 "self": "https://{site_hostname}/api{BASE_URL}{pid_value}/draft",
-                "self_html": "https://{site_hostname}/uploads/{pid_value}",
+                "self_html": "https://{site_hostname}{BASE_URL}{pid_value}/edit",
                 "versions": "https://{site_hostname}/api{BASE_URL}{pid_value}/versions",
             },
             "links_record": {
                 "draft": "https://{site_hostname}/api{BASE_URL}{pid_value}/draft",
                 "latest": "https://{site_hostname}/api{BASE_URL}{pid_value}/versions/latest",
                 "latest_html": "https://{site_hostname}{BASE_URL}{pid_value}/latest",
                 "publish": "https://{site_hostname}/api{BASE_URL}{pid_value}/draft/actions/publish",
```

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/datatypes/components/published_service.py` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/datatypes/components/published_service.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/__init__.py` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/invenio_drafts_parent_record.py` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/invenio_drafts_parent_record.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/invenio_drafts_published_api_views.py` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/invenio_drafts_published_api_views.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/invenio_drafts_published_app_views.py` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/invenio_drafts_published_app_views.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/invenio_drafts_published_invenio_ext_service.py` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/invenio_drafts_published_invenio_ext_service.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/invenio_drafts_record_metadata_extra_fields.py` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/invenio_drafts_record_metadata_extra_fields.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/invenio_drafts_setup_cfg.py` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/invenio_drafts_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_parent_state.py.jinja2` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_parent_state.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_published_ext_service.py.jinja2` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/invenio/templates/invenio_drafts_published_ext_service.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/profiles/draft.py` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/profiles/draft.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/tests/invenio_drafts_conftest.py` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/tests/invenio_drafts_conftest.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/tests/invenio_drafts_test_resources.py` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/tests/invenio_drafts_test_resources.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/tests/invenio_drafts_test_services.py` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/tests/invenio_drafts_test_services.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/tests/templates/invenio_conftest.py.jinja2` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/tests/templates/invenio_conftest.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/tests/templates/invenio_test_resources.py.jinja2` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/tests/templates/invenio_test_resources.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts/tests/templates/invenio_test_services.py.jinja2` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts/tests/templates/invenio_test_services.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts.egg-info/SOURCES.txt` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/oarepo_model_builder_drafts.egg-info/entry_points.txt` & `oarepo-model-builder-drafts-4.0.9/oarepo_model_builder_drafts.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-4.0.8/setup.cfg` & `oarepo-model-builder-drafts-4.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-drafts
-version = 4.0.8
+version = 4.0.9
 description = 
 authors = Ronald Krist <krist@cesnet.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

