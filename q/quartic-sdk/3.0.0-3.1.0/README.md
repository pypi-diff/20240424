# Comparing `tmp/quartic-sdk-3.0.0.tar.gz` & `tmp/quartic-sdk-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quartic-sdk-3.0.0.tar", last modified: Sun Mar  3 07:06:22 2024, max compression
+gzip compressed data, was "quartic-sdk-3.1.0.tar", last modified: Wed Apr 24 07:11:18 2024, max compression
```

## Comparing `quartic-sdk-3.0.0.tar` & `quartic-sdk-3.1.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 07:06:22.211631 quartic-sdk-3.0.0/
--rw-rw-r--   0 root         (0) root         (0)     1049 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8555 2024-03-03 07:06:22.211631 quartic-sdk-3.0.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     7900 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 07:06:22.207631 quartic-sdk-3.0.0/examples/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/examples/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      600 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/examples/expression.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 07:06:22.207631 quartic-sdk-3.0.0/quartic_sdk/
--rw-rw-r--   0 root         (0) root         (0)       98 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/__init__.py
--rw-rw-r--   0 root         (0) root         (0)       73 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 07:06:22.207631 quartic-sdk-3.0.0/quartic_sdk/api/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/api/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5342 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/api/api_helper.py
--rw-rw-r--   0 root         (0) root         (0)     5915 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 07:06:22.207631 quartic-sdk-3.0.0/quartic_sdk/core/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 07:06:22.207631 quartic-sdk-3.0.0/quartic_sdk/core/entities/
--rw-rw-r--   0 root         (0) root         (0)      785 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/core/entities/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5682 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/core/entities/asset.py
--rw-rw-r--   0 root         (0) root         (0)     1575 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/core/entities/base.py
--rw-rw-r--   0 root         (0) root         (0)      493 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/core/entities/batch.py
--rw-rw-r--   0 root         (0) root         (0)     1119 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/core/entities/context_frame.py
--rw-rw-r--   0 root         (0) root         (0)      586 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/core/entities/context_frame_occurrence.py
--rw-rw-r--   0 root         (0) root         (0)     5264 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/core/entities/edge_connector.py
--rw-rw-r--   0 root         (0) root         (0)     1497 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/core/entities/event_frame.py
--rw-rw-r--   0 root         (0) root         (0)      662 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/core/entities/event_frame_occurrence.py
--rw-rw-r--   0 root         (0) root         (0)     1531 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/core/entities/model.py
--rw-rw-r--   0 root         (0) root         (0)     1329 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/core/entities/procedure.py
--rw-rw-r--   0 root         (0) root         (0)     1229 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/core/entities/procedure_step.py
--rw-rw-r--   0 root         (0) root         (0)     1150 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/core/entities/product.py
--rw-rw-r--   0 root         (0) root         (0)      742 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/core/entities/site.py
--rw-rw-r--   0 root         (0) root         (0)     6859 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/core/entities/tag.py
--rw-rw-r--   0 root         (0) root         (0)      706 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/core/entities/type_mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 07:06:22.207631 quartic-sdk-3.0.0/quartic_sdk/core/entity_helpers/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/core/entity_helpers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1869 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/core/entity_helpers/entity_factory.py
--rw-rw-r--   0 root         (0) root         (0)     7724 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/core/entity_helpers/entity_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 07:06:22.211631 quartic-sdk-3.0.0/quartic_sdk/core/iterators/
--rw-rw-r--   0 root         (0) root         (0)       79 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/core/iterators/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      718 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/core/iterators/entity_list_iterator.py
--rw-rw-r--   0 root         (0) root         (0)     3432 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/core/iterators/historical_tag_data_iterator.py
--rw-rw-r--   0 root         (0) root         (0)      301 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/exceptions.py
--rw-rw-r--   0 root         (0) root         (0)     6356 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/graphql_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 07:06:22.211631 quartic-sdk-3.0.0/quartic_sdk/model/
--rw-rw-r--   0 root         (0) root         (0)     7538 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/model/BaseQuarticModel.py
--rw-rw-r--   0 root         (0) root         (0)     7399 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/model/BaseReckonExpression.py
--rw-rw-r--   0 root         (0) root         (0)     5953 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/model/BaseSpectralModel.py
--rw-rw-r--   0 root         (0) root         (0)      201 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/model/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4955 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/model/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 07:06:22.211631 quartic-sdk-3.0.0/quartic_sdk/model/tests/
--rw-rw-r--   0 root         (0) root         (0)     2400 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/model/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3231 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/model/tests/test_helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 07:06:22.211631 quartic-sdk-3.0.0/quartic_sdk/utilities/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/utilities/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2150 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/utilities/configuration.py
--rw-rw-r--   0 root         (0) root         (0)     4610 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/utilities/constants.py
--rw-rw-r--   0 root         (0) root         (0)     9921 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/utilities/decorator.py
--rw-rw-r--   0 root         (0) root         (0)      452 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/utilities/exceptions.py
--rw-rw-r--   0 root         (0) root         (0)       79 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/utilities/jupyter_utils.py
--rw-rw-r--   0 root         (0) root         (0)     8094 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/utilities/tag_data.py
--rw-rw-r--   0 root         (0) root         (0)     5956 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/utilities/test_helpers.py
--rw-rw-r--   0 root         (0) root         (0)     2340 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/quartic_sdk/utilities/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-03 07:06:22.207631 quartic-sdk-3.0.0/quartic_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8555 2024-03-03 07:06:22.000000 quartic-sdk-3.0.0/quartic_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1976 2024-03-03 07:06:22.000000 quartic-sdk-3.0.0/quartic_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-03 07:06:22.000000 quartic-sdk-3.0.0/quartic_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     7650 2024-03-03 07:06:22.000000 quartic-sdk-3.0.0/quartic_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-03 07:06:22.000000 quartic-sdk-3.0.0/quartic_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       66 2024-03-03 07:06:22.211631 quartic-sdk-3.0.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1733 2024-03-03 07:02:45.000000 quartic-sdk-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:11:18.692917 quartic-sdk-3.1.0/
+-rw-rw-r--   0 root         (0) root         (0)     1049 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8555 2024-04-24 07:11:18.692917 quartic-sdk-3.1.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     7900 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:11:18.688917 quartic-sdk-3.1.0/examples/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/examples/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      600 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/examples/expression.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:11:18.688917 quartic-sdk-3.1.0/quartic_sdk/
+-rw-rw-r--   0 root         (0) root         (0)       98 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)       73 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:11:18.688917 quartic-sdk-3.1.0/quartic_sdk/api/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/api/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5342 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/api/api_helper.py
+-rw-rw-r--   0 root         (0) root         (0)     5915 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:11:18.688917 quartic-sdk-3.1.0/quartic_sdk/core/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:11:18.688917 quartic-sdk-3.1.0/quartic_sdk/core/entities/
+-rw-rw-r--   0 root         (0) root         (0)      785 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/core/entities/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5682 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/core/entities/asset.py
+-rw-rw-r--   0 root         (0) root         (0)     1575 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/core/entities/base.py
+-rw-rw-r--   0 root         (0) root         (0)      493 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/core/entities/batch.py
+-rw-rw-r--   0 root         (0) root         (0)     1119 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/core/entities/context_frame.py
+-rw-rw-r--   0 root         (0) root         (0)      586 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/core/entities/context_frame_occurrence.py
+-rw-rw-r--   0 root         (0) root         (0)     5264 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/core/entities/edge_connector.py
+-rw-rw-r--   0 root         (0) root         (0)     1497 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/core/entities/event_frame.py
+-rw-rw-r--   0 root         (0) root         (0)      662 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/core/entities/event_frame_occurrence.py
+-rw-rw-r--   0 root         (0) root         (0)     1531 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/core/entities/model.py
+-rw-rw-r--   0 root         (0) root         (0)     1329 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/core/entities/procedure.py
+-rw-rw-r--   0 root         (0) root         (0)     1229 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/core/entities/procedure_step.py
+-rw-rw-r--   0 root         (0) root         (0)     1150 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/core/entities/product.py
+-rw-rw-r--   0 root         (0) root         (0)      742 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/core/entities/site.py
+-rw-rw-r--   0 root         (0) root         (0)     6859 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/core/entities/tag.py
+-rw-rw-r--   0 root         (0) root         (0)      706 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/core/entities/type_mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:11:18.688917 quartic-sdk-3.1.0/quartic_sdk/core/entity_helpers/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/core/entity_helpers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1869 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/core/entity_helpers/entity_factory.py
+-rw-rw-r--   0 root         (0) root         (0)     7724 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/core/entity_helpers/entity_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:11:18.688917 quartic-sdk-3.1.0/quartic_sdk/core/iterators/
+-rw-rw-r--   0 root         (0) root         (0)       79 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/core/iterators/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      718 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/core/iterators/entity_list_iterator.py
+-rw-rw-r--   0 root         (0) root         (0)     3432 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/core/iterators/historical_tag_data_iterator.py
+-rw-rw-r--   0 root         (0) root         (0)      301 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)     6356 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/graphql_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:11:18.692917 quartic-sdk-3.1.0/quartic_sdk/model/
+-rw-rw-r--   0 root         (0) root         (0)     7538 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/model/BaseQuarticModel.py
+-rw-rw-r--   0 root         (0) root         (0)     7399 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/model/BaseReckonExpression.py
+-rw-rw-r--   0 root         (0) root         (0)     5953 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/model/BaseSpectralModel.py
+-rw-rw-r--   0 root         (0) root         (0)      201 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/model/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4955 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/model/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:11:18.692917 quartic-sdk-3.1.0/quartic_sdk/model/tests/
+-rw-rw-r--   0 root         (0) root         (0)     2400 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/model/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3231 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/model/tests/test_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:11:18.692917 quartic-sdk-3.1.0/quartic_sdk/utilities/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/utilities/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2150 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/utilities/configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     4610 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/utilities/constants.py
+-rw-rw-r--   0 root         (0) root         (0)     9921 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/utilities/decorator.py
+-rw-rw-r--   0 root         (0) root         (0)      452 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/utilities/exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)       79 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/utilities/jupyter_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     8094 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/utilities/tag_data.py
+-rw-rw-r--   0 root         (0) root         (0)     5956 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/utilities/test_helpers.py
+-rw-rw-r--   0 root         (0) root         (0)     2340 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/quartic_sdk/utilities/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 07:11:18.688917 quartic-sdk-3.1.0/quartic_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8555 2024-04-24 07:11:18.000000 quartic-sdk-3.1.0/quartic_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1976 2024-04-24 07:11:18.000000 quartic-sdk-3.1.0/quartic_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 07:11:18.000000 quartic-sdk-3.1.0/quartic_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     7645 2024-04-24 07:11:18.000000 quartic-sdk-3.1.0/quartic_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-24 07:11:18.000000 quartic-sdk-3.1.0/quartic_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2024-04-24 07:11:18.692917 quartic-sdk-3.1.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1733 2024-04-24 07:08:37.000000 quartic-sdk-3.1.0/setup.py
```

### Comparing `quartic-sdk-3.0.0/LICENSE` & `quartic-sdk-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/PKG-INFO` & `quartic-sdk-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quartic-sdk
-Version: 3.0.0
+Version: 3.1.0
 Summary: QuarticSDK is the SDK package which exposes the APIs to the user
 Home-page: https://github.com/Quarticai/QuarticSDK/
 Author: Quartic.ai engineering team
 Author-email: tech@quartic.ai
 License: MIT
 Keywords: Quartic,QuarticSDK
 Platform: UNKNOWN
```

### Comparing `quartic-sdk-3.0.0/README.md` & `quartic-sdk-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/examples/expression.py` & `quartic-sdk-3.1.0/examples/expression.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/api/api_helper.py` & `quartic-sdk-3.1.0/quartic_sdk/api/api_helper.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/api_client.py` & `quartic-sdk-3.1.0/quartic_sdk/api_client.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/core/entities/__init__.py` & `quartic-sdk-3.1.0/quartic_sdk/core/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/core/entities/asset.py` & `quartic-sdk-3.1.0/quartic_sdk/core/entities/asset.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/core/entities/base.py` & `quartic-sdk-3.1.0/quartic_sdk/core/entities/base.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/core/entities/context_frame.py` & `quartic-sdk-3.1.0/quartic_sdk/core/entities/context_frame.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/core/entities/context_frame_occurrence.py` & `quartic-sdk-3.1.0/quartic_sdk/core/entities/context_frame_occurrence.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/core/entities/edge_connector.py` & `quartic-sdk-3.1.0/quartic_sdk/core/entities/edge_connector.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/core/entities/event_frame.py` & `quartic-sdk-3.1.0/quartic_sdk/core/entities/event_frame.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/core/entities/event_frame_occurrence.py` & `quartic-sdk-3.1.0/quartic_sdk/core/entities/event_frame_occurrence.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/core/entities/model.py` & `quartic-sdk-3.1.0/quartic_sdk/core/entities/model.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/core/entities/procedure.py` & `quartic-sdk-3.1.0/quartic_sdk/core/entities/procedure.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/core/entities/procedure_step.py` & `quartic-sdk-3.1.0/quartic_sdk/core/entities/procedure_step.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/core/entities/product.py` & `quartic-sdk-3.1.0/quartic_sdk/core/entities/product.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/core/entities/site.py` & `quartic-sdk-3.1.0/quartic_sdk/core/entities/site.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/core/entities/tag.py` & `quartic-sdk-3.1.0/quartic_sdk/core/entities/tag.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/core/entities/type_mapping.py` & `quartic-sdk-3.1.0/quartic_sdk/core/entities/type_mapping.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/core/entity_helpers/entity_factory.py` & `quartic-sdk-3.1.0/quartic_sdk/core/entity_helpers/entity_factory.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/core/entity_helpers/entity_list.py` & `quartic-sdk-3.1.0/quartic_sdk/core/entity_helpers/entity_list.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/core/iterators/entity_list_iterator.py` & `quartic-sdk-3.1.0/quartic_sdk/core/iterators/entity_list_iterator.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/core/iterators/historical_tag_data_iterator.py` & `quartic-sdk-3.1.0/quartic_sdk/core/iterators/historical_tag_data_iterator.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/graphql_client.py` & `quartic-sdk-3.1.0/quartic_sdk/graphql_client.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/model/BaseQuarticModel.py` & `quartic-sdk-3.1.0/quartic_sdk/model/BaseQuarticModel.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/model/BaseReckonExpression.py` & `quartic-sdk-3.1.0/quartic_sdk/model/BaseReckonExpression.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/model/BaseSpectralModel.py` & `quartic-sdk-3.1.0/quartic_sdk/model/BaseSpectralModel.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/model/helpers.py` & `quartic-sdk-3.1.0/quartic_sdk/model/helpers.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/model/tests/__init__.py` & `quartic-sdk-3.1.0/quartic_sdk/model/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/model/tests/test_helpers.py` & `quartic-sdk-3.1.0/quartic_sdk/model/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/utilities/configuration.py` & `quartic-sdk-3.1.0/quartic_sdk/utilities/configuration.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/utilities/constants.py` & `quartic-sdk-3.1.0/quartic_sdk/utilities/constants.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/utilities/decorator.py` & `quartic-sdk-3.1.0/quartic_sdk/utilities/decorator.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/utilities/tag_data.py` & `quartic-sdk-3.1.0/quartic_sdk/utilities/tag_data.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/utilities/test_helpers.py` & `quartic-sdk-3.1.0/quartic_sdk/utilities/test_helpers.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk/utilities/utils.py` & `quartic-sdk-3.1.0/quartic_sdk/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk.egg-info/PKG-INFO` & `quartic-sdk-3.1.0/quartic_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quartic-sdk
-Version: 3.0.0
+Version: 3.1.0
 Summary: QuarticSDK is the SDK package which exposes the APIs to the user
 Home-page: https://github.com/Quarticai/QuarticSDK/
 Author: Quartic.ai engineering team
 Author-email: tech@quartic.ai
 License: MIT
 Keywords: Quartic,QuarticSDK
 Platform: UNKNOWN
```

### Comparing `quartic-sdk-3.0.0/quartic_sdk.egg-info/SOURCES.txt` & `quartic-sdk-3.1.0/quartic_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quartic-sdk-3.0.0/quartic_sdk.egg-info/requires.txt` & `quartic-sdk-3.1.0/quartic_sdk.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 cachetools==5.2.0
 certifi==2022.12.7
 charset-normalizer==2.0.12
 click==8.0.3
 cloudpickle==1.6.0
 colorama==0.4.6
 coloredlogs==15.0.1
-comm==0.2.1
+comm==0.2.2
 cssutils==2.6.0
 cycler==0.12.1
 debugpy==1.8.1
 decorator==5.1.1
 dict2css==0.3.0.post1
 docutils==0.17.1
 domdf-python-tools==3.7.0
@@ -43,33 +43,33 @@
 importlib-metadata==7.0.1
 iniconfig==2.0.0
 ipykernel==6.25.2
 ipynbname==2023.2.0.0
 ipython==8.18.1
 jedi==0.19.1
 jinja2==3.0.3
-joblib==1.3.2
+joblib==1.4.0
 jupyter-client==7.2.0
-jupyter-core==5.7.1
+jupyter-core==5.7.2
 lazy-object-proxy==1.10.0
 livereload==2.6.3
 lockfile==0.12.2
 lunr==0.5.8
 markupsafe==2.1.1
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
 msgpack==1.0.2
 multidict==6.0.3
 natsort==8.4.0
 nest-asyncio==1.5.4
 nltk==3.6.6
 nose==1.3.7
 numpy==1.22.0
 packaging==20.9
 pandas==1.3.0
-parso==0.8.3
+parso==0.8.4
 pexpect==4.8.0
 pillow==9.0.1
 platformdirs==3.7.0
 pluggy==0.13.1
 prompt-toolkit==3.0.43
 psutil==5.9.4
 ptyprocess==0.7.0
@@ -81,15 +81,15 @@
 pygments==2.17.2
 pyparsing==2.4.7
 pytest==6.2.2
 python-dateutil==2.8.2
 pytz==2022.7.1
 pyyaml==5.4.1
 pyzmq==22.0.2
-regex==2023.12.25
+regex==2024.4.16
 requests==2.26.0
 rsa==4.9
 ruamel-yaml==0.17.22
 ruamel-yaml-clib==0.2.8
 six==1.15.0
 snowballstemmer==2.2.0
 soupsieve==2.4.1
@@ -104,29 +104,29 @@
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
 stack-data==0.6.3
 tabulate==0.9.0
-tensorflow-io-gcs-filesystem==0.32.0
+tensorflow-io-gcs-filesystem==0.31.0
 toml==0.10.2
 tornado==6.1
 tqdm==4.66.2
-traitlets==5.14.1
+traitlets==5.14.3
 typed-ast==1.4.2
 typing-extensions==4.6.0
 unidecode==1.3.8
 urllib3==1.26.6
 validators==0.18.2
 wcwidth==0.2.13
 webencodings==0.5.1
 wrapt==1.12.1
 yarl==1.8.2
-zipp==3.17.0
+zipp==3.18.1
 
 [complete]
 aiogqlc==2.2.0
 aiohttp==3.8.1
 aiosignal==1.3.1
 alabaster==0.7.16
 aloe==0.2.0
@@ -144,15 +144,15 @@
 cachetools==5.2.0
 certifi==2022.12.7
 charset-normalizer==2.0.12
 click==8.0.3
 cloudpickle==1.6.0
 colorama==0.4.6
 coloredlogs==15.0.1
-comm==0.2.1
+comm==0.2.2
 cssutils==2.6.0
 cycler==0.12.1
 debugpy==1.8.1
 decorator==5.1.1
 dict2css==0.3.0.post1
 docutils==0.17.1
 domdf-python-tools==3.7.0
@@ -170,33 +170,33 @@
 importlib-metadata==7.0.1
 iniconfig==2.0.0
 ipykernel==6.25.2
 ipynbname==2023.2.0.0
 ipython==8.18.1
 jedi==0.19.1
 jinja2==3.0.3
-joblib==1.3.2
+joblib==1.4.0
 jupyter-client==7.2.0
-jupyter-core==5.7.1
+jupyter-core==5.7.2
 lazy-object-proxy==1.10.0
 livereload==2.6.3
 lockfile==0.12.2
 lunr==0.5.8
 markupsafe==2.1.1
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
 msgpack==1.0.2
 multidict==6.0.3
 natsort==8.4.0
 nest-asyncio==1.5.4
 nltk==3.6.6
 nose==1.3.7
 numpy==1.22.0
 packaging==20.9
 pandas==1.3.0
-parso==0.8.3
+parso==0.8.4
 pexpect==4.8.0
 pillow==9.0.1
 platformdirs==3.7.0
 pluggy==0.13.1
 prompt-toolkit==3.0.43
 psutil==5.9.4
 ptyprocess==0.7.0
@@ -208,15 +208,15 @@
 pygments==2.17.2
 pyparsing==2.4.7
 pytest==6.2.2
 python-dateutil==2.8.2
 pytz==2022.7.1
 pyyaml==5.4.1
 pyzmq==22.0.2
-regex==2023.12.25
+regex==2024.4.16
 requests==2.26.0
 rsa==4.9
 ruamel-yaml==0.17.22
 ruamel-yaml-clib==0.2.8
 six==1.15.0
 snowballstemmer==2.2.0
 soupsieve==2.4.1
@@ -231,29 +231,29 @@
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
 stack-data==0.6.3
 tabulate==0.9.0
-tensorflow-io-gcs-filesystem==0.32.0
+tensorflow-io-gcs-filesystem==0.31.0
 toml==0.10.2
 tornado==6.1
 tqdm==4.66.2
-traitlets==5.14.1
+traitlets==5.14.3
 typed-ast==1.4.2
 typing-extensions==4.6.0
 unidecode==1.3.8
 urllib3==1.26.6
 validators==0.18.2
 wcwidth==0.2.13
 webencodings==0.5.1
 wrapt==1.12.1
 yarl==1.8.2
-zipp==3.17.0
+zipp==3.18.1
 absl-py==2.1.0
 aiogqlc==2.2.0
 aiohttp==3.8.1
 aiosignal==1.3.1
 alabaster==0.7.16
 aloe==0.2.0
 ansicolors==1.1.8
@@ -271,15 +271,15 @@
 cachetools==5.2.0
 certifi==2022.12.7
 charset-normalizer==2.0.12
 click==8.0.3
 cloudpickle==1.6.0
 colorama==0.4.6
 coloredlogs==15.0.1
-comm==0.2.1
+comm==0.2.2
 cssutils==2.6.0
 cycler==0.12.1
 debugpy==1.8.1
 decorator==5.1.1
 dict2css==0.3.0.post1
 docutils==0.17.1
 domdf-python-tools==3.7.0
@@ -289,59 +289,59 @@
 flatbuffers==2.0.7
 frozenlist==1.3.3
 future==1.0.0
 gast==0.4.0
 gherkin-official==4.1.3
 google-auth==2.15.0
 google-pasta==0.2.0
-grpcio==1.62.0
+grpcio==1.62.2
 h2o==3.32.0.4
-h5py==3.10.0
+h5py==3.11.0
 html5lib==1.1
 humanfriendly==10.0
 idna==3.4
 imagesize==1.4.1
 importlib-metadata==7.0.1
 iniconfig==2.0.0
 ipykernel==6.25.2
 ipython==8.18.1
 jedi==0.19.1
 jinja2==3.0.3
-joblib==1.3.2
+joblib==1.4.0
 jupyter-client==7.2.0
-jupyter-core==5.7.1
+jupyter-core==5.7.2
 keras==2.7.0
 keras-preprocessing==1.1.2
 kiwisolver==1.4.5
 lazy-object-proxy==1.10.0
-libclang==16.0.6
+libclang==18.1.1
 lightgbm==2.2.2
 livereload==2.6.3
 llvmlite==0.36.0
 lockfile==0.12.2
 lunr==0.5.8
-markdown==3.5.2
+markdown==3.6
 markupsafe==2.1.1
 matplotlib==3.3.4
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
 msgpack==1.0.2
 multidict==6.0.3
 natsort==8.4.0
 nest-asyncio==1.5.4
 nltk==3.6.6
 nose==1.3.7
 numba==0.53.1
 numexpr==2.7.2
 numpy==1.22.0
 onnx==1.9.0
 opt-einsum==3.3.0
 packaging==20.9
 pamela==1.0.0
 pandas==1.3.0
-parso==0.8.3
+parso==0.8.4
 patsy==0.5.1
 pexpect==4.8.0
 pillow==9.0.1
 platformdirs==3.7.0
 plotly==4.14.3
 pluggy==0.13.1
 prompt-toolkit==3.0.43
@@ -361,15 +361,15 @@
 pypmml==0.9.9
 pytest==6.2.2
 python-dateutil==2.8.2
 pytorch-ignite==0.4.3
 pytz==2022.7.1
 pyyaml==5.4.1
 pyzmq==22.0.2
-regex==2023.12.25
+regex==2024.4.16
 requests==2.26.0
 retrying==1.3.4
 rsa==4.9
 ruamel-yaml==0.17.22
 ruamel-yaml-clib==0.2.8
 scikit-learn==1.1.3
 scikit-optimize==0.8.1
@@ -390,34 +390,34 @@
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
 stack-data==0.6.3
 statsmodels==0.12.2
 tabulate==0.9.0
-tbb==2021.11.0
+tbb==2021.12.0
 tensorboard==2.16.2
 tensorboard-data-server==0.7.2
 tensorflow==2.7.1
 tensorflow-estimator==2.7.0
-tensorflow-io-gcs-filesystem==0.32.0
+tensorflow-io-gcs-filesystem==0.31.0
 termcolor==2.4.0
-threadpoolctl==3.3.0
+threadpoolctl==3.4.0
 toml==0.10.2
 torch==1.7.1
 tornado==6.1
 tqdm==4.66.2
-traitlets==5.14.1
+traitlets==5.14.3
 typed-ast==1.4.2
 typing-extensions==4.6.0
 umap-learn==0.4.1
 unidecode==1.3.8
 urllib3==1.26.6
 validators==0.18.2
 wcwidth==0.2.13
 webencodings==0.5.1
-werkzeug==3.0.1
-wheel==0.42.0
+werkzeug==3.0.2
+wheel==0.43.0
 wrapt==1.12.1
 xgboost==0.81
 yarl==1.8.2
-zipp==3.17.0
+zipp==3.18.1
```

### Comparing `quartic-sdk-3.0.0/setup.py` & `quartic-sdk-3.1.0/setup.py`

 * *Files identical despite different names*

