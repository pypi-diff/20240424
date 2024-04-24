# Comparing `tmp/graphlit_client-1.0.20240420011.tar.gz` & `tmp/graphlit_client-1.0.20240423001.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphlit_client-1.0.20240420011.tar", last modified: Sun Apr 21 01:30:18 2024, max compression
+gzip compressed data, was "graphlit_client-1.0.20240423001.tar", last modified: Wed Apr 24 05:27:37 2024, max compression
```

## Comparing `graphlit_client-1.0.20240420011.tar` & `graphlit_client-1.0.20240423001.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-21 01:30:18.381570 graphlit_client-1.0.20240420011/
--rw-r--r--   0 vsts      (1001) docker     (127)     1095 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-21 01:30:18.377570 graphlit_client-1.0.20240420011/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2321 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-21 01:30:18.365570 graphlit_client-1.0.20240420011/graphlit/
--rw-r--r--   0 vsts      (1001) docker     (127)       32 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1796 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit/graphlit.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-21 01:30:18.377570 graphlit_client-1.0.20240420011/graphlit_api/
--rw-r--r--   0 vsts      (1001) docker     (127)    59183 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      888 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/add_contents_to_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12578 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/async_base_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)      620 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/base_model.py
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/clear_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    42943 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/client.py
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/close_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/create_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/create_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/create_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/create_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/create_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/create_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      984 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/credits.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/delete_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/delete_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/delete_all_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/delete_all_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/delete_all_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/delete_all_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/delete_all_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/delete_all_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      452 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/delete_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      482 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/delete_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/delete_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/delete_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/delete_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/delete_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/delete_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/delete_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/delete_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/delete_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/delete_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/disable_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/disable_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/enable_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/enable_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16585 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2411 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (127)      957 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/extract_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3609 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/get_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      799 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/get_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7230 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/get_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4014 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/get_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7138 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/get_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1269 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/get_project.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4461 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/get_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7887 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/get_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      677 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/ingest_encoded_file.py
--rw-r--r--   0 vsts      (1001) docker     (127)      606 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/ingest_text.py
--rw-r--r--   0 vsts      (1001) docker     (127)      598 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/ingest_uri.py
--rw-r--r--   0 vsts      (1001) docker     (127)    68146 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/input_types.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/is_content_done.py
--rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/is_feed_done.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1050 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/lookup_credits.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1568 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/lookup_usage.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39649 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/operations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3256 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/prompt_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2055 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/prompt_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)      796 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/publish_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/publish_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/query_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/query_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1112 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/query_content_facets.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7934 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/query_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4623 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/query_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7942 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/query_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4912 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/query_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8865 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/query_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/remove_contents_from_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/suggest_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1096 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/summarize_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/update_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/update_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      644 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/update_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/update_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/update_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/update_project.py
--rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/update_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/update_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1482 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/graphlit_api/usage.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-21 01:30:18.377570 graphlit_client-1.0.20240420011/graphlit_client.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-21 01:30:18.000000 graphlit_client-1.0.20240420011/graphlit_client.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2870 2024-04-21 01:30:18.000000 graphlit_client-1.0.20240420011/graphlit_client.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-21 01:30:18.000000 graphlit_client-1.0.20240420011/graphlit_client.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-04-21 01:30:18.000000 graphlit_client-1.0.20240420011/graphlit_client.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-04-21 01:30:18.000000 graphlit_client-1.0.20240420011/graphlit_client.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      299 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-21 01:30:18.381570 graphlit_client-1.0.20240420011/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)      766 2024-04-21 01:30:04.000000 graphlit_client-1.0.20240420011/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 05:27:37.983565 graphlit_client-1.0.20240423001/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1095 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-24 05:27:37.983565 graphlit_client-1.0.20240423001/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2321 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 05:27:37.963565 graphlit_client-1.0.20240423001/graphlit/
+-rw-r--r--   0 vsts      (1001) docker     (127)       32 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1796 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit/graphlit.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 05:27:37.983565 graphlit_client-1.0.20240423001/graphlit_api/
+-rw-r--r--   0 vsts      (1001) docker     (127)    59431 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      888 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/add_contents_to_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12578 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/async_base_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      620 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/base_model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/clear_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    42943 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/close_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/create_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/create_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/create_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/create_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/create_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/create_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      984 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/credits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_all_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      507 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_all_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_all_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_all_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_all_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_all_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      452 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      482 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/delete_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/disable_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/disable_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/enable_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/enable_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16949 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2411 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      957 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/extract_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3609 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/get_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      799 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/get_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7230 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/get_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4014 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/get_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7138 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/get_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1269 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/get_project.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4502 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/get_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7887 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/get_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      677 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/ingest_encoded_file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      606 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/ingest_text.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      598 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/ingest_uri.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    69218 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/input_types.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/is_content_done.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/is_feed_done.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1050 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/lookup_credits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1568 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/lookup_usage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39649 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/operations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3256 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/prompt_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2055 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/prompt_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      796 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/publish_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/publish_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/query_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/query_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1112 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/query_content_facets.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7934 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/query_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4623 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/query_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7942 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/query_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4953 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/query_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8865 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/query_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/remove_contents_from_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/suggest_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1096 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/summarize_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/update_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/update_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      644 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/update_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/update_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/update_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/update_project.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/update_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/update_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1482 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/graphlit_api/usage.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-24 05:27:37.983565 graphlit_client-1.0.20240423001/graphlit_client.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-24 05:27:37.000000 graphlit_client-1.0.20240423001/graphlit_client.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2870 2024-04-24 05:27:37.000000 graphlit_client-1.0.20240423001/graphlit_client.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-24 05:27:37.000000 graphlit_client-1.0.20240423001/graphlit_client.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-04-24 05:27:37.000000 graphlit_client-1.0.20240423001/graphlit_client.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-04-24 05:27:37.000000 graphlit_client-1.0.20240423001/graphlit_client.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      295 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-24 05:27:37.983565 graphlit_client-1.0.20240423001/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)      766 2024-04-24 05:27:21.000000 graphlit_client-1.0.20240423001/setup.py
```

### Comparing `graphlit_client-1.0.20240420011/LICENSE` & `graphlit_client-1.0.20240423001/LICENSE`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/PKG-INFO` & `graphlit_client-1.0.20240423001/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlit-client
-Version: 1.0.20240420011
+Version: 1.0.20240423001
 Summary: Graphlit API Python Client
 Home-page: https://github.com/graphlit/graphlit-client-python
 Author: Unstruk Data Inc.
 Author-email: questions@graphlit.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `graphlit_client-1.0.20240420011/README.md` & `graphlit_client-1.0.20240423001/README.md`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit/graphlit.py` & `graphlit_client-1.0.20240423001/graphlit/graphlit.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/__init__.py` & `graphlit_client-1.0.20240423001/graphlit_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,14 +98,15 @@
     AlertTypes,
     AnthropicModels,
     ApplyPolicy,
     AzureDocumentIntelligenceModels,
     AzureOpenAIModels,
     BillableMetrics,
     CategoryFacetTypes,
+    CohereModels,
     CollectionTypes,
     ContentFacetTypes,
     ContentPublishingFormats,
     ContentPublishingServiceTypes,
     ContentTypes,
     ConversationRoleTypes,
     ConversationSearchTypes,
@@ -153,14 +154,15 @@
     PlaceFacetTypes,
     PolicyTimeTypes,
     ProductFacetTypes,
     PromptStrategyTypes,
     RenditionTypes,
     ReplicateModels,
     RepoFacetTypes,
+    RerankingModelServiceTypes,
     ResourceConnectorTypes,
     RetrievalStrategyTypes,
     SearchQueryTypes,
     SearchTypes,
     SharePointAuthenticationTypes,
     SiteTypes,
     SoftwareFacetTypes,
@@ -363,14 +365,16 @@
     AzureOpenAIModelPropertiesUpdateInput,
     AzureTextExtractionPropertiesInput,
     BoundingBoxInput,
     CategoryFacetInput,
     CategoryFilter,
     CategoryInput,
     CategoryUpdateInput,
+    CohereModelPropertiesInput,
+    CohereModelPropertiesUpdateInput,
     CollectionFilter,
     CollectionInput,
     CollectionUpdateInput,
     ContentCriteriaInput,
     ContentFacetInput,
     ContentFilter,
     ContentInput,
@@ -897,14 +901,17 @@
     "CategoryInput",
     "CategoryUpdateInput",
     "ClearConversation",
     "ClearConversationClearConversation",
     "Client",
     "CloseConversation",
     "CloseConversationCloseConversation",
+    "CohereModelPropertiesInput",
+    "CohereModelPropertiesUpdateInput",
+    "CohereModels",
     "CollectionFilter",
     "CollectionInput",
     "CollectionTypes",
     "CollectionUpdateInput",
     "ContentCriteriaInput",
     "ContentFacetInput",
     "ContentFacetTypes",
@@ -1539,14 +1546,15 @@
     "ReplicateModelPropertiesUpdateInput",
     "ReplicateModels",
     "RepoFacetInput",
     "RepoFacetTypes",
     "RepoFilter",
     "RepoInput",
     "RepoUpdateInput",
+    "RerankingModelServiceTypes",
     "RerankingStrategyInput",
     "RerankingStrategyUpdateInput",
     "ResourceConnectorTypes",
     "RetrievalStrategyInput",
     "RetrievalStrategyTypes",
     "RetrievalStrategyUpdateInput",
     "SUGGEST_CONVERSATION_GQL",
```

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/add_contents_to_collections.py` & `graphlit_client-1.0.20240423001/graphlit_api/add_contents_to_collections.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/async_base_client.py` & `graphlit_client-1.0.20240423001/graphlit_api/async_base_client.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/base_model.py` & `graphlit_client-1.0.20240423001/graphlit_api/base_model.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/clear_conversation.py` & `graphlit_client-1.0.20240423001/graphlit_api/clear_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/client.py` & `graphlit_client-1.0.20240423001/graphlit_api/client.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/close_conversation.py` & `graphlit_client-1.0.20240423001/graphlit_api/close_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/create_collection.py` & `graphlit_client-1.0.20240423001/graphlit_api/create_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/create_conversation.py` & `graphlit_client-1.0.20240423001/graphlit_api/create_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/create_specification.py` & `graphlit_client-1.0.20240423001/graphlit_api/create_specification.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/create_workflow.py` & `graphlit_client-1.0.20240423001/graphlit_api/create_workflow.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/credits.py` & `graphlit_client-1.0.20240423001/graphlit_api/credits.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/delete_all_conversations.py` & `graphlit_client-1.0.20240423001/graphlit_api/delete_all_conversations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/enums.py` & `graphlit_client-1.0.20240423001/graphlit_api/enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Generated by ariadne-codegen
-# Source: https://data-scus-dev.graphlit.io/api/v1/graphql
+# Source: https://data-scus.graphlit.io/api/v1/graphql
 
 from enum import Enum
 
 
 class ApplyPolicy(str, Enum):
     BEFORE_RESOLVER = "BEFORE_RESOLVER"
     AFTER_RESOLVER = "AFTER_RESOLVER"
@@ -469,14 +469,19 @@
 
 class RetrievalStrategyTypes(str, Enum):
     CONTENT = "CONTENT"
     CHUNK = "CHUNK"
     SECTION = "SECTION"
 
 
+class RerankingModelServiceTypes(str, Enum):
+    COHERE = "COHERE"
+    JINA = "JINA"
+
+
 class OpenAIModels(str, Enum):
     GPT35_TURBO = "GPT35_TURBO"
     GPT35_TURBO_0613 = "GPT35_TURBO_0613"
     GPT35_TURBO_16K = "GPT35_TURBO_16K"
     GPT35_TURBO_16K_0613 = "GPT35_TURBO_16K_0613"
     GPT35_TURBO_16K_1106 = "GPT35_TURBO_16K_1106"
     GPT35_TURBO_16K_0125 = "GPT35_TURBO_16K_0125"
@@ -496,14 +501,22 @@
 class AzureOpenAIModels(str, Enum):
     GPT35_TURBO_16K = "GPT35_TURBO_16K"
     GPT4 = "GPT4"
     GPT4_TURBO_128K = "GPT4_TURBO_128K"
     CUSTOM = "CUSTOM"
 
 
+class CohereModels(str, Enum):
+    EMBED_ENGLISH_3_0 = "EMBED_ENGLISH_3_0"
+    EMBED_MULTILINGUAL_3_0 = "EMBED_MULTILINGUAL_3_0"
+    COMMAND_R = "COMMAND_R"
+    COMMAND_R_PLUS = "COMMAND_R_PLUS"
+    CUSTOM = "CUSTOM"
+
+
 class AnthropicModels(str, Enum):
     CLAUDE_2 = "CLAUDE_2"
     CLAUDE_2_0 = "CLAUDE_2_0"
     CLAUDE_2_1 = "CLAUDE_2_1"
     CLAUDE_INSTANT_1 = "CLAUDE_INSTANT_1"
     CLAUDE_INSTANT_1_2 = "CLAUDE_INSTANT_1_2"
     CLAUDE_3_OPUS = "CLAUDE_3_OPUS"
@@ -530,14 +543,16 @@
     MISTRAL_MEDIUM = "MISTRAL_MEDIUM"
     MISTRAL_LARGE = "MISTRAL_LARGE"
     CUSTOM = "CUSTOM"
 
 
 class GroqModels(str, Enum):
     MIXTRAL_8X7B_INSTRUCT = "MIXTRAL_8X7B_INSTRUCT"
+    LLAMA_3_70B = "LLAMA_3_70B"
+    LLAMA_3_8B = "LLAMA_3_8B"
     CUSTOM = "CUSTOM"
 
 
 class ElevenLabsModels(str, Enum):
     MULTILINGUAL_V1 = "MULTILINGUAL_V1"
     MULTILINGUAL_V2 = "MULTILINGUAL_V2"
     ENGLISH_V1 = "ENGLISH_V1"
```

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/exceptions.py` & `graphlit_client-1.0.20240423001/graphlit_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/extract_contents.py` & `graphlit_client-1.0.20240423001/graphlit_api/extract_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/get_alert.py` & `graphlit_client-1.0.20240423001/graphlit_api/get_alert.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/get_collection.py` & `graphlit_client-1.0.20240423001/graphlit_api/get_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/get_content.py` & `graphlit_client-1.0.20240423001/graphlit_api/get_content.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/get_conversation.py` & `graphlit_client-1.0.20240423001/graphlit_api/get_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/get_feed.py` & `graphlit_client-1.0.20240423001/graphlit_api/get_feed.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/get_project.py` & `graphlit_client-1.0.20240423001/graphlit_api/get_project.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/get_specification.py` & `graphlit_client-1.0.20240423001/graphlit_api/get_specification.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     AzureOpenAIModels,
     ConversationStrategyTypes,
     EntityState,
     ModelServiceTypes,
     OpenAIModels,
     PromptStrategyTypes,
     ReplicateModels,
+    RerankingModelServiceTypes,
     RetrievalStrategyTypes,
     SpecificationTypes,
 )
 
 
 class GetSpecification(BaseModel):
     specification: Optional["GetSpecificationSpecification"]
@@ -72,15 +73,15 @@
 
 class GetSpecificationSpecificationRetrievalStrategy(BaseModel):
     type: RetrievalStrategyTypes
     content_limit: Optional[int] = Field(alias="contentLimit")
 
 
 class GetSpecificationSpecificationRerankingStrategy(BaseModel):
-    service_type: ModelServiceTypes = Field(alias="serviceType")
+    service_type: RerankingModelServiceTypes = Field(alias="serviceType")
 
 
 class GetSpecificationSpecificationOpenAi(BaseModel):
     token_limit: Optional[int] = Field(alias="tokenLimit")
     completion_token_limit: Optional[int] = Field(alias="completionTokenLimit")
     model: OpenAIModels
     key: Optional[str]
```

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/get_workflow.py` & `graphlit_client-1.0.20240423001/graphlit_api/get_workflow.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/ingest_encoded_file.py` & `graphlit_client-1.0.20240423001/graphlit_api/ingest_encoded_file.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/ingest_text.py` & `graphlit_client-1.0.20240423001/graphlit_api/ingest_text.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/ingest_uri.py` & `graphlit_client-1.0.20240423001/graphlit_api/ingest_uri.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/input_types.py` & `graphlit_client-1.0.20240423001/graphlit_api/input_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # Generated by ariadne-codegen
-# Source: https://data-scus-dev.graphlit.io/api/v1/graphql
+# Source: https://data-scus.graphlit.io/api/v1/graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .enums import (
     AlertTypes,
     AnthropicModels,
     AzureDocumentIntelligenceModels,
     AzureOpenAIModels,
     CategoryFacetTypes,
+    CohereModels,
     CollectionTypes,
     ContentFacetTypes,
     ContentPublishingFormats,
     ContentPublishingServiceTypes,
     ContentTypes,
     ConversationSearchTypes,
     ConversationStrategyTypes,
@@ -52,14 +53,15 @@
     PersonFacetTypes,
     PlaceFacetTypes,
     PolicyTimeTypes,
     ProductFacetTypes,
     PromptStrategyTypes,
     ReplicateModels,
     RepoFacetTypes,
+    RerankingModelServiceTypes,
     ResourceConnectorTypes,
     RetrievalStrategyTypes,
     SearchQueryTypes,
     SearchTypes,
     SharePointAuthenticationTypes,
     SoftwareFacetTypes,
     SpecificationTypes,
@@ -652,14 +654,15 @@
     tools: Optional[List["ToolDefinitionInput"]] = None
     open_ai: Optional["OpenAIModelPropertiesInput"] = Field(
         alias="openAI", default=None
     )
     azure_open_ai: Optional["AzureOpenAIModelPropertiesInput"] = Field(
         alias="azureOpenAI", default=None
     )
+    cohere: Optional["CohereModelPropertiesInput"] = None
     anthropic: Optional["AnthropicModelPropertiesInput"] = None
     replicate: Optional["ReplicateModelPropertiesInput"] = None
     mistral: Optional["MistralModelPropertiesInput"] = None
     groq: Optional["GroqModelPropertiesInput"] = None
 
 
 class WorkflowInput(BaseModel):
@@ -894,14 +897,15 @@
     tools: Optional[List["ToolDefinitionUpdateInput"]] = None
     open_ai: Optional["OpenAIModelPropertiesUpdateInput"] = Field(
         alias="openAI", default=None
     )
     azure_open_ai: Optional["AzureOpenAIModelPropertiesUpdateInput"] = Field(
         alias="azureOpenAI", default=None
     )
+    cohere: Optional["CohereModelPropertiesUpdateInput"] = None
     anthropic: Optional["AnthropicModelPropertiesUpdateInput"] = None
     replicate: Optional["ReplicateModelPropertiesUpdateInput"] = None
     mistral: Optional["MistralModelPropertiesUpdateInput"] = None
     groq: Optional["GroqModelPropertiesUpdateInput"] = None
 
 
 class WorkflowUpdateInput(BaseModel):
@@ -1147,15 +1151,15 @@
 
 class RetrievalStrategyInput(BaseModel):
     type: RetrievalStrategyTypes
     content_limit: Optional[int] = Field(alias="contentLimit", default=None)
 
 
 class RerankingStrategyInput(BaseModel):
-    service_type: ModelServiceTypes = Field(alias="serviceType")
+    service_type: RerankingModelServiceTypes = Field(alias="serviceType")
 
 
 class ToolDefinitionInput(BaseModel):
     name: str
     description: Optional[str] = None
     schema_: str = Field(alias="schema")
     uri: Optional[Any] = None
@@ -1182,14 +1186,26 @@
     probability: Optional[float] = None
     token_limit: Optional[int] = Field(alias="tokenLimit", default=None)
     completion_token_limit: Optional[int] = Field(
         alias="completionTokenLimit", default=None
     )
 
 
+class CohereModelPropertiesInput(BaseModel):
+    model: CohereModels
+    model_name: Optional[str] = Field(alias="modelName", default=None)
+    key: Optional[str] = None
+    temperature: Optional[float] = None
+    probability: Optional[float] = None
+    token_limit: Optional[int] = Field(alias="tokenLimit", default=None)
+    completion_token_limit: Optional[int] = Field(
+        alias="completionTokenLimit", default=None
+    )
+
+
 class AnthropicModelPropertiesInput(BaseModel):
     model: AnthropicModels
     model_name: Optional[str] = Field(alias="modelName", default=None)
     key: Optional[str] = None
     temperature: Optional[float] = None
     probability: Optional[float] = None
     token_limit: Optional[int] = Field(alias="tokenLimit", default=None)
@@ -1384,15 +1400,17 @@
 
 class RetrievalStrategyUpdateInput(BaseModel):
     type: Optional[RetrievalStrategyTypes] = None
     content_limit: Optional[int] = Field(alias="contentLimit", default=None)
 
 
 class RerankingStrategyUpdateInput(BaseModel):
-    service_type: Optional[ModelServiceTypes] = Field(alias="serviceType", default=None)
+    service_type: Optional[RerankingModelServiceTypes] = Field(
+        alias="serviceType", default=None
+    )
 
 
 class ToolDefinitionUpdateInput(BaseModel):
     name: Optional[str] = None
     description: Optional[str] = None
     schema_: Optional[str] = Field(alias="schema", default=None)
     uri: Optional[Any] = None
@@ -1418,14 +1436,26 @@
     temperature: Optional[float] = None
     probability: Optional[float] = None
     token_limit: Optional[int] = Field(alias="tokenLimit", default=None)
     completion_token_limit: Optional[int] = Field(
         alias="completionTokenLimit", default=None
     )
 
+
+class CohereModelPropertiesUpdateInput(BaseModel):
+    model: CohereModels
+    model_name: Optional[str] = Field(alias="modelName", default=None)
+    key: Optional[str] = None
+    temperature: Optional[float] = None
+    probability: Optional[float] = None
+    token_limit: Optional[int] = Field(alias="tokenLimit", default=None)
+    completion_token_limit: Optional[int] = Field(
+        alias="completionTokenLimit", default=None
+    )
+
 
 class AnthropicModelPropertiesUpdateInput(BaseModel):
     model: AnthropicModels
     model_name: Optional[str] = Field(alias="modelName", default=None)
     key: Optional[str] = None
     temperature: Optional[float] = None
     probability: Optional[float] = None
```

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/lookup_credits.py` & `graphlit_client-1.0.20240423001/graphlit_api/lookup_credits.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/lookup_usage.py` & `graphlit_client-1.0.20240423001/graphlit_api/lookup_usage.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/operations.py` & `graphlit_client-1.0.20240423001/graphlit_api/operations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/prompt_conversation.py` & `graphlit_client-1.0.20240423001/graphlit_api/prompt_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/prompt_specifications.py` & `graphlit_client-1.0.20240423001/graphlit_api/prompt_specifications.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/publish_contents.py` & `graphlit_client-1.0.20240423001/graphlit_api/publish_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/publish_conversation.py` & `graphlit_client-1.0.20240423001/graphlit_api/publish_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/query_alerts.py` & `graphlit_client-1.0.20240423001/graphlit_api/query_alerts.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/query_collections.py` & `graphlit_client-1.0.20240423001/graphlit_api/query_collections.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/query_content_facets.py` & `graphlit_client-1.0.20240423001/graphlit_api/query_content_facets.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/query_contents.py` & `graphlit_client-1.0.20240423001/graphlit_api/query_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/query_conversations.py` & `graphlit_client-1.0.20240423001/graphlit_api/query_conversations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/query_feeds.py` & `graphlit_client-1.0.20240423001/graphlit_api/query_feeds.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/query_specifications.py` & `graphlit_client-1.0.20240423001/graphlit_api/query_specifications.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     AzureOpenAIModels,
     ConversationStrategyTypes,
     EntityState,
     ModelServiceTypes,
     OpenAIModels,
     PromptStrategyTypes,
     ReplicateModels,
+    RerankingModelServiceTypes,
     RetrievalStrategyTypes,
     SpecificationTypes,
 )
 
 
 class QuerySpecifications(BaseModel):
     specifications: Optional["QuerySpecificationsSpecifications"]
@@ -78,15 +79,15 @@
 
 class QuerySpecificationsSpecificationsResultsRetrievalStrategy(BaseModel):
     type: RetrievalStrategyTypes
     content_limit: Optional[int] = Field(alias="contentLimit")
 
 
 class QuerySpecificationsSpecificationsResultsRerankingStrategy(BaseModel):
-    service_type: ModelServiceTypes = Field(alias="serviceType")
+    service_type: RerankingModelServiceTypes = Field(alias="serviceType")
 
 
 class QuerySpecificationsSpecificationsResultsOpenAi(BaseModel):
     token_limit: Optional[int] = Field(alias="tokenLimit")
     completion_token_limit: Optional[int] = Field(alias="completionTokenLimit")
     model: OpenAIModels
     key: Optional[str]
```

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/query_workflows.py` & `graphlit_client-1.0.20240423001/graphlit_api/query_workflows.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/remove_contents_from_collection.py` & `graphlit_client-1.0.20240423001/graphlit_api/remove_contents_from_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/summarize_contents.py` & `graphlit_client-1.0.20240423001/graphlit_api/summarize_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/update_collection.py` & `graphlit_client-1.0.20240423001/graphlit_api/update_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/update_content.py` & `graphlit_client-1.0.20240423001/graphlit_api/update_content.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/update_conversation.py` & `graphlit_client-1.0.20240423001/graphlit_api/update_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/update_specification.py` & `graphlit_client-1.0.20240423001/graphlit_api/update_specification.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/update_workflow.py` & `graphlit_client-1.0.20240423001/graphlit_api/update_workflow.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_api/usage.py` & `graphlit_client-1.0.20240423001/graphlit_api/usage.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/graphlit_client.egg-info/PKG-INFO` & `graphlit_client-1.0.20240423001/graphlit_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlit-client
-Version: 1.0.20240420011
+Version: 1.0.20240423001
 Summary: Graphlit API Python Client
 Home-page: https://github.com/graphlit/graphlit-client-python
 Author: Unstruk Data Inc.
 Author-email: questions@graphlit.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `graphlit_client-1.0.20240420011/graphlit_client.egg-info/SOURCES.txt` & `graphlit_client-1.0.20240423001/graphlit_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420011/setup.py` & `graphlit_client-1.0.20240423001/setup.py`

 * *Files identical despite different names*

