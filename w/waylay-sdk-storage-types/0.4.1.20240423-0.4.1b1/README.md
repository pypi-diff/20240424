# Comparing `tmp/waylay_sdk_storage_types-0.4.1.20240423.tar.gz` & `tmp/waylay-sdk-storage-types-0.4.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_sdk_storage_types-0.4.1.20240423.tar", last modified: Tue Apr 23 16:14:41 2024, max compression
+gzip compressed data, was "waylay-sdk-storage-types-0.4.1b1.tar", last modified: Thu Mar 28 13:32:40 2024, max compression
```

## Comparing `waylay_sdk_storage_types-0.4.1.20240423.tar` & `waylay-sdk-storage-types-0.4.1b1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:14:41.381584 waylay_sdk_storage_types-0.4.1.20240423/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-23 16:14:41.381584 waylay_sdk_storage_types-0.4.1.20240423/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 16:14:41.381584 waylay_sdk_storage_types-0.4.1.20240423/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:14:41.369584 waylay_sdk_storage_types-0.4.1.20240423/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:14:41.369584 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:14:41.369584 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:14:41.369584 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:14:41.377584 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/authentication_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/bucket_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/bucket_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/bucket_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/bucket_object_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/bucketcreationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/bucketpolicystatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/channeltype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/event_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/expiry.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/hal_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/hal_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/httpmethod.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/links.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/location_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/notification_queue_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/notification_queue_status_report.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/object.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/payload_config.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/queuesetupstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/response_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/sign.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/store.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/storetype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/subscription_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/subscriptions_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/system_channel_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/system_channel_config_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/tenant_status_report.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/venttype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/web_script_channel_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/web_script_channel_config_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:14:41.377584 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/queries/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/queries/about_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/queries/bucket_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/queries/object_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/queries/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-04-23 16:14:37.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/queries/subscription_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:14:41.377584 waylay_sdk_storage_types-0.4.1.20240423/src/waylay_sdk_storage_types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-23 16:14:41.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay_sdk_storage_types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-23 16:14:41.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay_sdk_storage_types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:14:41.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay_sdk_storage_types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-23 16:14:41.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay_sdk_storage_types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 16:14:41.000000 waylay_sdk_storage_types-0.4.1.20240423/src/waylay_sdk_storage_types.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:40.865666 waylay-sdk-storage-types-0.4.1b1/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-03-28 13:32:40.865666 waylay-sdk-storage-types-0.4.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 13:32:40.865666 waylay-sdk-storage-types-0.4.1b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:40.853666 waylay-sdk-storage-types-0.4.1b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:40.853666 waylay-sdk-storage-types-0.4.1b1/src/waylay/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:40.853666 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:40.853666 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:40.861666 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/authentication_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/bucket_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/bucket_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/bucket_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/bucket_object_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/bucketcreationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/bucketpolicystatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/channeltype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/event_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/expiry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/hal_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/hal_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/httpmethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/location_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/notification_queue_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/notification_queue_status_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/payload_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/queuesetupstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/response_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/sign.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/storetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/subscription_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/subscriptions_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/system_channel_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/system_channel_config_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/tenant_status_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/venttype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/web_script_channel_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/web_script_channel_config_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:40.861666 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/queries/about_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/queries/bucket_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/queries/object_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/queries/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-03-28 13:32:36.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/queries/subscription_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:32:40.861666 waylay-sdk-storage-types-0.4.1b1/src/waylay_sdk_storage_types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-03-28 13:32:40.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay_sdk_storage_types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-03-28 13:32:40.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay_sdk_storage_types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 13:32:40.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay_sdk_storage_types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-28 13:32:40.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay_sdk_storage_types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-28 13:32:40.000000 waylay-sdk-storage-types-0.4.1b1/src/waylay_sdk_storage_types.egg-info/top_level.txt
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/LICENSE.txt` & `waylay-sdk-storage-types-0.4.1b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/PKG-INFO` & `waylay-sdk-storage-types-0.4.1b1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-storage-types
-Version: 0.4.1.20240423
+Version: 0.4.1b1
 Summary: Waylay Storage Types 
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -13,23 +13,22 @@
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 Project-URL: Homepage, https://www.waylay.io/
-Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
+Project-URL: Documentation, https://docs.waylay.io/#/
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-storage-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/storage.html
 Keywords: Waylay Storage,Types
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.1
-Requires-Dist: waylay-sdk-storage==0.4.1.20240423
+Requires-Dist: waylay-sdk~=0.0.4rc5
+Requires-Dist: waylay-sdk-storage==0.4.1b1
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -47,37 +46,37 @@
 
 # Waylay Storage Service
 
 Manage storage buckets and subscriptions.
 
 
 This Python package is automatically generated based on the 
-Waylay Storage OpenAPI specification (API version: 0.4.1)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/storage.html).
+Waylay Storage OpenAPI specification (API version: v0.4.1)
 
 It is considered an extension of the waylay-sdk-storage package, and it consists of the typed model classes for all path params, query params, body params and responses for each of the api methods in `waylay-sdk-storage`.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-storage is included in:
-- ```pip install waylay-sdk-core[storage]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[storage]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-storage and waylay-sdk-storage-types are included in:
-- ```pip install waylay-sdk-core[storage,storage-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[storage,storage-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-storage-types` is installed
@@ -89,8 +88,7 @@
     print("The response of storage.about.version:\n")
     pprint(api_response)
 except ApiError as e:
     print("Exception when calling storage.about.version: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/README.md` & `waylay-sdk-storage-types-0.4.1b1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # Waylay Storage Service
 
 Manage storage buckets and subscriptions.
 
 
 This Python package is automatically generated based on the 
-Waylay Storage OpenAPI specification (API version: 0.4.1)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/storage.html).
+Waylay Storage OpenAPI specification (API version: v0.4.1)
 
 It is considered an extension of the waylay-sdk-storage package, and it consists of the typed model classes for all path params, query params, body params and responses for each of the api methods in `waylay-sdk-storage`.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-storage is included in:
-- ```pip install waylay-sdk-core[storage]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[storage]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-storage and waylay-sdk-storage-types are included in:
-- ```pip install waylay-sdk-core[storage,storage-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[storage,storage-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-storage-types` is installed
@@ -42,8 +42,7 @@
     print("The response of storage.about.version:\n")
     pprint(api_response)
 except ApiError as e:
     print("Exception when calling storage.about.version: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/pyproject.toml` & `waylay-sdk-storage-types-0.4.1b1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waylay-sdk-storage-types"
-version = "0.4.1.20240423"
+version = "0.4.1b1"
 description = "Waylay Storage Types "
 authors = [
     { name = "Waylay", email = "info@waylay.io"}
 ]
 keywords = ["Waylay Storage" , "Types"]
 requires-python = ">= 3.9"
 dependencies = [
-    "waylay-sdk-core ~= 0.2.1",
-    "waylay-sdk-storage == 0.4.1.20240423",
+    "waylay-sdk ~= 0.0.4rc5",
+    "waylay-sdk-storage == 0.4.1b1",
     "pydantic ~= 2.6",
     "typing-extensions ~= 4.10",
     "eval-type-backport ~= 0.1.3; python_version < '3.10'",
 ]
 readme = "README.md"
 license={file = "LICENSE.txt"}
 
 [project.urls]
 Homepage = "https://www.waylay.io/"
-Documentation = "https://docs.waylay.io/#/api/?id=software-development-kits"
+Documentation = "https://docs.waylay.io/#/"
 Repository = "https://github.com/waylayio/waylay-sdk-storage-py.git"
-"Openapi Specification" = "https://docs.waylay.io/openapi/public/redocly/storage.html"
 
 [project.optional-dependencies]
 dev = [
     "mypy",
     "ruff",
     "types-python-jose",
     "types-appdirs",
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/__init__.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # coding: utf-8
 """Waylay Storage: REST Models.
 
 This code was generated from the OpenAPI documentation of 'Waylay Storage'
 
-version: 0.4.1
+version: v0.4.1
 
  Manage storage buckets and subscriptions.
 
 Generated by OpenAPI Generator (https://openapi-generator.tech)
 
 Do not edit the class manually.
 """
 
-__version__ = "0.4.1.20240423"
+__version__ = "0.4.1b1"
 
 # import models into model package
 from .auth import AUTH
 from .authentication_config import AuthenticationConfig
 from .bucket import Bucket
 from .bucket_configuration import BucketConfiguration
 from .bucket_listing import BucketListing
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/auth.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/auth.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/authentication_config.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/payload_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,26 +7,29 @@
 
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
+from typing import Any, List
+
 from pydantic import (
     ConfigDict,
-    StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.auth import AUTH
+from ..models.sign import SIGN
 
 
-class AuthenticationConfig(WaylayBaseModel):
-    """Configuration for the authentication method used when forwarding an event to a channel.."""
+class PayloadConfig(WaylayBaseModel):
+    """Configuration object that specifies the expected notification payload.."""
 
-    method: AUTH | None = None
-    key: StrictStr | None = None
-    secret: StrictStr | None = None
+    signed_links: List[SIGN] | None = None
+    reference: Any | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/bucket.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/bucket_object.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,29 +13,38 @@
 
 from datetime import datetime
 from typing import Dict
 
 from pydantic import (
     ConfigDict,
     Field,
+    StrictBool,
     StrictInt,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
+from ..models.bucket import Bucket
 from ..models.links import Links
-from ..models.store import Store
 
 
-class Bucket(WaylayBaseModel):
-    """Representation of a storage bucket.."""
+class BucketObject(WaylayBaseModel):
+    """Representation of a storage object.."""
 
     links: Dict[str, Links] | None = Field(default=None, alias="_links")
-    alias: StrictStr | None = None
+    bucket: Bucket
     name: StrictStr
-    store: Store | None = None
-    creation_date: datetime | None = None
+    last_modified: datetime | None = None
+    etag: StrictStr | None = None
     size: StrictInt | None = None
+    content_type: StrictStr | None = None
+    is_dir: StrictBool | None = False
+    storage_class: StrictStr | None = None
+    owner_id: StrictStr | None = None
+    owner_name: StrictStr | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/bucket_configuration.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/bucket_configuration.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,9 +38,12 @@
     size: StrictInt | None = None
     status: BUCKETCREATIONSTATUS | None = None
     public_policy_json: Dict[str, Any] | None = None
     public_policy_type: StrictStr | None = None
     error: StrictStr | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/bucket_listing.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/subscriptions_listing.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,16 +19,19 @@
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
 from ..models.bucket import Bucket
 from ..models.links import Links
 
 
-class BucketListing(WaylayBaseModel):
-    """List of Bucket representations.."""
+class SubscriptionsListing(WaylayBaseModel):
+    """List of buckets that support subscriptions.."""
 
     links: Dict[str, Links] | None = Field(default=None, alias="_links")
     buckets: List[Bucket]
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/bucket_object.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/queries/bucket_api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,57 @@
 # coding: utf-8
-"""Waylay Storage models.
+"""Waylay Storage query parameters.
 
 This code was generated from the OpenAPI documentation of 'Waylay Storage'
 
 Generated by OpenAPI Generator (https://openapi-generator.tech)
 
 Do not edit the class manually.
-
 """
 
-from __future__ import annotations
-
-from datetime import datetime
-from typing import Dict
+from __future__ import annotations  # for Python 3.7–3.9
 
 from pydantic import (
     ConfigDict,
-    Field,
-    StrictBool,
-    StrictInt,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.bucket import Bucket
-from ..models.links import Links
+
+def _get_query_alias_for(field_name: str) -> str:
+    if field_name == "store":
+        return "store"
+    return field_name
+
+
+class GetQuery(WaylayBaseModel):
+    """Model for `get` query parameters."""
+
+    store: StrictStr | None = None
+
+    model_config = ConfigDict(
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
+        alias_generator=_get_query_alias_for,
+        populate_by_name=True,
+    )
+
+
+def _list_query_alias_for(field_name: str) -> str:
+    if field_name == "store":
+        return "store"
+    return field_name
 
 
-class BucketObject(WaylayBaseModel):
-    """Representation of a storage object.."""
+class ListQuery(WaylayBaseModel):
+    """Model for `list` query parameters."""
 
-    links: Dict[str, Links] | None = Field(default=None, alias="_links")
-    bucket: Bucket
-    name: StrictStr
-    last_modified: datetime | None = None
-    etag: StrictStr | None = None
-    size: StrictInt | None = None
-    content_type: StrictStr | None = None
-    is_dir: StrictBool | None = False
-    storage_class: StrictStr | None = None
-    owner_id: StrictStr | None = None
-    owner_name: StrictStr | None = None
+    store: StrictStr | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="allow",
+        alias_generator=_list_query_alias_for,
+        populate_by_name=True,
     )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/bucket_object_listing.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/bucket_object_listing.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,9 +26,12 @@
 class BucketObjectListing(WaylayBaseModel):
     """List of storage object representations.."""
 
     links: Dict[str, Links] | None = Field(default=None, alias="_links")
     objects: List[BucketObject]
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/bucketcreationstatus.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/bucketcreationstatus.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/bucketpolicystatus.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/bucketpolicystatus.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/channel.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/channel.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/event_filter.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/event_filter.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,9 +28,12 @@
     prefix: StrictStr | None = None
     suffix: StrictStr | None = None
     events: List[VENTTYPE] | None = None
     description: StrictStr | None = None
     queue: StrictStr | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/expiry.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/bucket_listing.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,24 +7,31 @@
 
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
+from typing import Dict, List
+
 from pydantic import (
     ConfigDict,
-    StrictInt,
+    Field,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
+from ..models.bucket import Bucket
+from ..models.links import Links
+
 
-class Expiry(WaylayBaseModel):
-    """Input model for expiry parameters.."""
+class BucketListing(WaylayBaseModel):
+    """List of Bucket representations.."""
 
-    seconds: StrictInt | None = None
-    hours: StrictInt | None = None
-    days: StrictInt | None = None
+    links: Dict[str, Links] | None = Field(default=None, alias="_links")
+    buckets: List[Bucket]
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/hal_entity.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/hal_entity.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,9 +24,12 @@
 
 class HALEntity(WaylayBaseModel):
     """Output model representing a collection of HAL links.."""
 
     links: Dict[str, Links] | None = Field(default=None, alias="_links")
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/hal_link.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/bucket.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,26 +7,38 @@
 
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
-from typing import Any, Dict
+from datetime import datetime
+from typing import Dict
 
 from pydantic import (
     ConfigDict,
+    Field,
+    StrictInt,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
+from ..models.links import Links
+from ..models.store import Store
 
-class HALLink(WaylayBaseModel):
-    """Represents a HAL link.."""
 
-    href: StrictStr
-    method: StrictStr | None = None
-    form_data: Dict[str, Any] | None = None
+class Bucket(WaylayBaseModel):
+    """Representation of a storage bucket.."""
+
+    links: Dict[str, Links] | None = Field(default=None, alias="_links")
+    alias: StrictStr | None = None
+    name: StrictStr
+    store: Store | None = None
+    creation_date: datetime | None = None
+    size: StrictInt | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/http_validation_error.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/validation_error.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,21 +11,27 @@
 
 from __future__ import annotations
 
 from typing import List
 
 from pydantic import (
     ConfigDict,
+    StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.validation_error import ValidationError
+from ..models.location_inner import LocationInner
 
 
-class HTTPValidationError(WaylayBaseModel):
-    """HTTPValidationError."""
+class ValidationError(WaylayBaseModel):
+    """ValidationError."""
 
-    detail: List[ValidationError] | None = None
+    loc: List[LocationInner]
+    msg: StrictStr
+    type: StrictStr
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/notification_queue_status.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/subscription_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,31 +7,37 @@
 
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
-from typing import Any, Dict
+from typing import Dict, List
 
 from pydantic import (
     ConfigDict,
+    Field,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.queuesetupstatus import QUEUESETUPSTATUS
+from ..models.channel import Channel
+from ..models.event_filter import EventFilter
+from ..models.links import Links
 
 
-class NotificationQueueStatus(WaylayBaseModel):
-    """Response model for the notification queue configuration.."""
-
-    status: QUEUESETUPSTATUS
-    name: StrictStr
-    method: StrictStr
-    configured_parameters: Dict[str, Any] | None = None
-    actual_parameters: Dict[str, Any] | None = None
-    error: StrictStr | None = None
+class SubscriptionConfig(WaylayBaseModel):
+    """Specification of a notification subscription that forwards to a given channel.."""
+
+    links: Dict[str, Links] | None = Field(default=None, alias="_links")
+    id: StrictStr | None = None
+    title: StrictStr | None = None
+    description: StrictStr | None = None
+    channel: Channel
+    filters: List[EventFilter]
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/notification_queue_status_report.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/http_validation_error.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
-from typing import Any, Dict, List
+from typing import List
 
 from pydantic import (
     ConfigDict,
-    StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.notification_queue_status import NotificationQueueStatus
+from ..models.validation_error import ValidationError
 
 
-class NotificationQueueStatusReport(WaylayBaseModel):
-    """Response model for a notification queue status report.."""
+class HTTPValidationError(WaylayBaseModel):
+    """HTTPValidationError."""
 
-    store: StrictStr
-    notification_queues: List[NotificationQueueStatus]
-    messages: List[Dict[str, Any]] | None = None
+    detail: List[ValidationError] | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/payload_config.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/authentication_config.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,26 +7,29 @@
 
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
-from typing import Any, List
-
 from pydantic import (
     ConfigDict,
+    StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.sign import SIGN
+from ..models.auth import AUTH
 
 
-class PayloadConfig(WaylayBaseModel):
-    """Configuration object that specifies the expected notification payload.."""
+class AuthenticationConfig(WaylayBaseModel):
+    """Configuration for the authentication method used when forwarding an event to a channel.."""
 
-    signed_links: List[SIGN] | None = None
-    reference: Any | None = None
+    method: AUTH | None = None
+    key: StrictStr | None = None
+    secret: StrictStr | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/queuesetupstatus.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/queuesetupstatus.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/response_list.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/response_list.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/store.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/store.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,9 +29,12 @@
 
     links: Dict[str, Links] | None = Field(default=None, alias="_links")
     type: STORETYPE
     name: StrictStr
     url: StrictStr
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/subscriptions.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/subscriptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,9 +29,12 @@
 
     links: Dict[str, Links] | None = Field(default=None, alias="_links")
     bucket: Bucket
     subscriptions: List[SubscriptionConfig]
     warnings: List[Dict[str, Any]] | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/subscriptions_listing.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/expiry.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,28 +7,27 @@
 
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
-from typing import Dict, List
-
 from pydantic import (
     ConfigDict,
-    Field,
+    StrictInt,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.bucket import Bucket
-from ..models.links import Links
-
 
-class SubscriptionsListing(WaylayBaseModel):
-    """List of buckets that support subscriptions.."""
+class Expiry(WaylayBaseModel):
+    """Input model for expiry parameters.."""
 
-    links: Dict[str, Links] | None = Field(default=None, alias="_links")
-    buckets: List[Bucket]
+    seconds: StrictInt | None = None
+    hours: StrictInt | None = None
+    days: StrictInt | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/system_channel_config.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/system_channel_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,9 +29,12 @@
     type: SystemChannelConfigType | None = None
     description: StrictStr | None = None
     payload: PayloadConfig | None = None
     authentication: AuthenticationConfig | None = None
     expiry: Expiry | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/tenant_status_report.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/tenant_status_report.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,9 +35,12 @@
     queues: List[NotificationQueueStatusReport] | None = None
     total_size: StrictInt | None = None
     bucket_status: BUCKETCREATIONSTATUS | None = None
     policy_status: BUCKETPOLICYSTATUS | None = None
     queue_status: QUEUESETUPSTATUS | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/validation_error.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/hal_link.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 
 Do not edit the class manually.
 
 """
 
 from __future__ import annotations
 
-from typing import List
+from typing import Any, Dict
 
 from pydantic import (
     ConfigDict,
     StrictStr,
 )
 from waylay.sdk.api._models import BaseModel as WaylayBaseModel
 
-from ..models.location_inner import LocationInner
 
+class HALLink(WaylayBaseModel):
+    """Represents a HAL link.."""
 
-class ValidationError(WaylayBaseModel):
-    """ValidationError."""
-
-    loc: List[LocationInner]
-    msg: StrictStr
-    type: StrictStr
+    href: StrictStr
+    method: StrictStr | None = None
+    form_data: Dict[str, Any] | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/models/web_script_channel_config.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/models/web_script_channel_config.py`

 * *Files 25% similar despite different names*

```diff
@@ -33,9 +33,12 @@
     authentication: AuthenticationConfig | None = None
     expiry: Expiry | None = None
     name: StrictStr
     version: StrictStr | None = None
     method: HTTPMETHOD | None = None
 
     model_config = ConfigDict(
-        populate_by_name=True, protected_namespaces=(), extra="ignore"
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+        extra="ignore",
     )
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/queries/about_api.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/queries/about_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
     store: StrictStr | None = None
     include_buckets: StrictBool | None = None
     include_queues: StrictBool | None = None
     include_disk_usage: StrictBool | None = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_status_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -50,12 +51,13 @@
     return field_name
 
 
 class VersionQuery(WaylayBaseModel):
     """Model for `version` query parameters."""
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_version_query_alias_for,
         populate_by_name=True,
     )
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/queries/object_api.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/queries/object_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     """Model for `copy_or_move` query parameters."""
 
     source: StrictStr
     move: StrictBool | None = None
     store: StrictStr | None = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_copy_or_move_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -55,14 +56,15 @@
 class CreateFolderQuery(WaylayBaseModel):
     """Model for `create_folder` query parameters."""
 
     all: StrictBool | None = None
     store: StrictStr | None = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_create_folder_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -116,14 +118,15 @@
     expiry_hours: StrictInt | None = None
     expiry_seconds: StrictInt | None = None
     content_length_min: StrictInt | None = None
     content_length_max: StrictInt | None = None
     content_type: StrictStr | None = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_list_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -147,12 +150,13 @@
     recursive: StrictBool | None = None
     all: StrictBool | None = None
     start_after: StrictStr | None = None
     max_keys: StrictInt | None = None
     store: StrictStr | None = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_remove_query_alias_for,
         populate_by_name=True,
     )
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay/services/storage/queries/subscription_api.py` & `waylay-sdk-storage-types-0.4.1b1/src/waylay/services/storage/queries/subscription_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 class CreateQuery(WaylayBaseModel):
     """Model for `create` query parameters."""
 
     store: StrictStr | None = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_create_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -69,14 +70,15 @@
     event_type: VENTTYPE | None = None
     channel_type: CHANNELTYPE | None = None
     channel_id: StrictStr | None = None
     store: StrictStr | None = None
     max_keys: StrictInt | None = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_delete_by_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -88,14 +90,15 @@
 
 class GetQuery(WaylayBaseModel):
     """Model for `get` query parameters."""
 
     store: StrictStr | None = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_get_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -125,14 +128,15 @@
     suffix: StrictStr | None = None
     event_type: VENTTYPE | None = None
     channel_type: CHANNELTYPE | None = None
     channel_id: StrictStr | None = None
     max_keys: StrictInt | None = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_list_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -165,14 +169,15 @@
     suffix: StrictStr | None = None
     event_type: VENTTYPE | None = None
     channel_type: CHANNELTYPE | None = None
     channel_id: StrictStr | None = None
     max_keys: StrictInt | None = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_query_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -184,14 +189,15 @@
 
 class RemoveQuery(WaylayBaseModel):
     """Model for `remove` query parameters."""
 
     store: StrictStr | None = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_remove_query_alias_for,
         populate_by_name=True,
     )
 
 
@@ -203,12 +209,13 @@
 
 class ReplaceQuery(WaylayBaseModel):
     """Model for `replace` query parameters."""
 
     store: StrictStr | None = None
 
     model_config = ConfigDict(
+        validate_assignment=True,
         protected_namespaces=(),
         extra="allow",
         alias_generator=_replace_query_alias_for,
         populate_by_name=True,
     )
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay_sdk_storage_types.egg-info/PKG-INFO` & `waylay-sdk-storage-types-0.4.1b1/src/waylay_sdk_storage_types.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-storage-types
-Version: 0.4.1.20240423
+Version: 0.4.1b1
 Summary: Waylay Storage Types 
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -13,23 +13,22 @@
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 Project-URL: Homepage, https://www.waylay.io/
-Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
+Project-URL: Documentation, https://docs.waylay.io/#/
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-storage-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/storage.html
 Keywords: Waylay Storage,Types
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.1
-Requires-Dist: waylay-sdk-storage==0.4.1.20240423
+Requires-Dist: waylay-sdk~=0.0.4rc5
+Requires-Dist: waylay-sdk-storage==0.4.1b1
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -47,37 +46,37 @@
 
 # Waylay Storage Service
 
 Manage storage buckets and subscriptions.
 
 
 This Python package is automatically generated based on the 
-Waylay Storage OpenAPI specification (API version: 0.4.1)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/storage.html).
+Waylay Storage OpenAPI specification (API version: v0.4.1)
 
 It is considered an extension of the waylay-sdk-storage package, and it consists of the typed model classes for all path params, query params, body params and responses for each of the api methods in `waylay-sdk-storage`.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-storage is included in:
-- ```pip install waylay-sdk-core[storage]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[storage]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-storage and waylay-sdk-storage-types are included in:
-- ```pip install waylay-sdk-core[storage,storage-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[storage,storage-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-storage-types` is installed
@@ -89,8 +88,7 @@
     print("The response of storage.about.version:\n")
     pprint(api_response)
 except ApiError as e:
     print("Exception when calling storage.about.version: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_storage_types-0.4.1.20240423/src/waylay_sdk_storage_types.egg-info/SOURCES.txt` & `waylay-sdk-storage-types-0.4.1b1/src/waylay_sdk_storage_types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

