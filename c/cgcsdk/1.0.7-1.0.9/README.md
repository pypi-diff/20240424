# Comparing `tmp/cgcsdk-1.0.7.tar.gz` & `tmp/cgcsdk-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgcsdk-1.0.7.tar", last modified: Thu Apr  4 10:27:22 2024, max compression
+gzip compressed data, was "cgcsdk-1.0.9.tar", last modified: Tue Apr 23 14:23:16 2024, max compression
```

## Comparing `cgcsdk-1.0.7.tar` & `cgcsdk-1.0.9.tar`

### file list

```diff
@@ -1,109 +1,114 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 10:27:22.598588 cgcsdk-1.0.7/
--rw-rw-rw-   0        0        0        0 2022-04-21 08:27:42.000000 cgcsdk-1.0.7/LICENSE
--rw-rw-rw-   0        0        0      112 2023-06-13 11:20:10.000000 cgcsdk-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     3173 2024-04-04 10:27:22.578670 cgcsdk-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1811 2024-03-27 14:48:25.000000 cgcsdk-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 10:27:20.606882 cgcsdk-1.0.7/cgc/
--rw-rw-rw-   0        0        0      209 2024-04-04 10:26:20.000000 cgcsdk-1.0.7/cgc/.env
--rw-rw-rw-   0        0        0     7808 2024-04-04 10:26:21.000000 cgcsdk-1.0.7/cgc/CHANGELOG.md
--rw-rw-rw-   0        0        0      326 2023-04-18 09:56:45.000000 cgcsdk-1.0.7/cgc/__init__.py
--rw-rw-rw-   0        0        0     1493 2024-04-04 10:26:21.000000 cgcsdk-1.0.7/cgc/cgc.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:27:20.656354 cgcsdk-1.0.7/cgc/commands/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-1.0.7/cgc/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:27:20.703998 cgcsdk-1.0.7/cgc/commands/auth/
--rw-rw-rw-   0        0        0      399 2023-05-18 12:02:14.000000 cgcsdk-1.0.7/cgc/commands/auth/__init__.py
--rw-rw-rw-   0        0        0     3856 2023-10-30 10:28:44.000000 cgcsdk-1.0.7/cgc/commands/auth/auth_cmd.py
--rw-rw-rw-   0        0        0     1839 2023-10-30 10:06:10.000000 cgcsdk-1.0.7/cgc/commands/auth/auth_responses.py
--rw-rw-rw-   0        0        0     5359 2023-10-30 10:06:10.000000 cgcsdk-1.0.7/cgc/commands/auth/auth_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:27:20.744462 cgcsdk-1.0.7/cgc/commands/billing/
--rw-rw-rw-   0        0        0      753 2023-04-14 14:28:08.000000 cgcsdk-1.0.7/cgc/commands/billing/__init__.py
--rw-rw-rw-   0        0        0     4140 2023-11-15 10:46:21.000000 cgcsdk-1.0.7/cgc/commands/billing/billing_cmd.py
--rw-rw-rw-   0        0        0     1949 2023-04-14 14:28:08.000000 cgcsdk-1.0.7/cgc/commands/billing/billing_responses.py
--rw-rw-rw-   0        0        0     4711 2023-06-14 08:36:45.000000 cgcsdk-1.0.7/cgc/commands/billing/billing_utils.py
--rw-rw-rw-   0        0        0     4956 2024-04-04 10:26:21.000000 cgcsdk-1.0.7/cgc/commands/cgc_cmd.py
--rw-rw-rw-   0        0        0     2245 2024-04-04 10:26:21.000000 cgcsdk-1.0.7/cgc/commands/cgc_cmd_responses.py
--rw-rw-rw-   0        0        0     1174 2024-03-13 09:33:01.000000 cgcsdk-1.0.7/cgc/commands/cgc_helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:27:20.805689 cgcsdk-1.0.7/cgc/commands/compute/
--rw-rw-rw-   0        0        0      239 2023-02-15 11:40:43.000000 cgcsdk-1.0.7/cgc/commands/compute/__init__.py
--rw-rw-rw-   0        0        0    15490 2024-03-13 09:36:12.000000 cgcsdk-1.0.7/cgc/commands/compute/compute_cmd.py
--rw-rw-rw-   0        0        0     1173 2024-04-04 10:26:21.000000 cgcsdk-1.0.7/cgc/commands/compute/compute_models.py
--rw-rw-rw-   0        0        0     5807 2024-03-08 11:15:19.000000 cgcsdk-1.0.7/cgc/commands/compute/compute_responses.py
--rw-rw-rw-   0        0        0     8812 2024-04-04 10:26:21.000000 cgcsdk-1.0.7/cgc/commands/compute/compute_utills.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:27:20.826492 cgcsdk-1.0.7/cgc/commands/db/
--rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-1.0.7/cgc/commands/db/__init__.py
--rw-rw-rw-   0        0        0     3309 2024-03-13 09:33:01.000000 cgcsdk-1.0.7/cgc/commands/db/db_cmd.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:27:20.846858 cgcsdk-1.0.7/cgc/commands/debug/
--rw-rw-rw-   0        0        0        0 2023-04-18 09:56:45.000000 cgcsdk-1.0.7/cgc/commands/debug/__init__.py
--rw-rw-rw-   0        0        0      412 2023-04-17 11:02:43.000000 cgcsdk-1.0.7/cgc/commands/debug/debug_cmd.py
--rw-rw-rw-   0        0        0       45 2023-02-15 11:40:43.000000 cgcsdk-1.0.7/cgc/commands/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:27:20.890910 cgcsdk-1.0.7/cgc/commands/jobs/
--rw-rw-rw-   0        0        0      231 2024-04-04 10:26:21.000000 cgcsdk-1.0.7/cgc/commands/jobs/__init__.py
--rw-rw-rw-   0        0        0     5952 2024-04-04 10:26:21.000000 cgcsdk-1.0.7/cgc/commands/jobs/job_utils.py
--rw-rw-rw-   0        0        0     6555 2024-04-04 10:26:21.000000 cgcsdk-1.0.7/cgc/commands/jobs/jobs_cmd.py
--rw-rw-rw-   0        0        0     1771 2024-04-04 10:26:21.000000 cgcsdk-1.0.7/cgc/commands/jobs/jobs_responses.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:27:20.922278 cgcsdk-1.0.7/cgc/commands/resource/
--rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-1.0.7/cgc/commands/resource/__init__.py
--rw-rw-rw-   0        0        0     4053 2024-03-13 09:33:01.000000 cgcsdk-1.0.7/cgc/commands/resource/resource_cmd.py
--rw-rw-rw-   0        0        0      197 2023-11-21 14:55:48.000000 cgcsdk-1.0.7/cgc/commands/resource/resource_responses.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:27:20.983915 cgcsdk-1.0.7/cgc/commands/volume/
--rw-rw-rw-   0        0        0      384 2023-02-15 11:40:43.000000 cgcsdk-1.0.7/cgc/commands/volume/__init__.py
--rw-rw-rw-   0        0        0     1295 2023-10-30 10:06:10.000000 cgcsdk-1.0.7/cgc/commands/volume/data_model.py
--rw-rw-rw-   0        0        0     7673 2024-03-13 09:33:01.000000 cgcsdk-1.0.7/cgc/commands/volume/volume_cmd.py
--rw-rw-rw-   0        0        0     3199 2023-02-15 11:40:43.000000 cgcsdk-1.0.7/cgc/commands/volume/volume_responses.py
--rw-rw-rw-   0        0        0     1919 2023-02-15 11:40:43.000000 cgcsdk-1.0.7/cgc/commands/volume/volume_utils.py
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-1.0.7/cgc/config.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:27:21.081126 cgcsdk-1.0.7/cgc/sdk/
--rw-rw-rw-   0        0        0      297 2024-04-04 10:26:21.000000 cgcsdk-1.0.7/cgc/sdk/__init__.py
--rw-rw-rw-   0        0        0      214 2024-03-08 13:51:26.000000 cgcsdk-1.0.7/cgc/sdk/exceptions.py
--rw-rw-rw-   0        0        0      868 2023-04-18 09:56:45.000000 cgcsdk-1.0.7/cgc/sdk/handlers.py
--rw-rw-rw-   0        0        0     5332 2024-04-04 10:26:21.000000 cgcsdk-1.0.7/cgc/sdk/job.py
--rw-rw-rw-   0        0        0     7221 2023-04-18 13:47:14.000000 cgcsdk-1.0.7/cgc/sdk/mongodb.py
--rw-rw-rw-   0        0        0     1637 2023-04-18 10:57:57.000000 cgcsdk-1.0.7/cgc/sdk/postgresql.py
--rw-rw-rw-   0        0        0     2844 2023-07-17 12:07:43.000000 cgcsdk-1.0.7/cgc/sdk/redis.py
--rw-rw-rw-   0        0        0    13544 2024-04-04 10:26:21.000000 cgcsdk-1.0.7/cgc/sdk/resource.py
--rw-rw-rw-   0        0        0     1452 2023-05-31 13:31:37.000000 cgcsdk-1.0.7/cgc/server.crt
-drwxrwxrwx   0        0        0        0 2024-04-04 10:27:21.118981 cgcsdk-1.0.7/cgc/telemetry/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-1.0.7/cgc/telemetry/__init__.py
--rw-rw-rw-   0        0        0     3175 2023-05-18 12:51:21.000000 cgcsdk-1.0.7/cgc/telemetry/basic.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:27:21.160856 cgcsdk-1.0.7/cgc/tests/
--rw-rw-rw-   0        0        0   102743 2023-07-17 12:07:43.000000 cgcsdk-1.0.7/cgc/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:27:21.474480 cgcsdk-1.0.7/cgc/tests/desired_responses/
--rw-rw-rw-   0        0        0     1579 2023-03-09 13:52:51.000000 cgcsdk-1.0.7/cgc/tests/desired_responses/test_billing_invoice.txt
--rw-rw-rw-   0        0        0     2381 2023-03-09 13:52:48.000000 cgcsdk-1.0.7/cgc/tests/desired_responses/test_billing_status.txt
--rw-rw-rw-   0        0        0      234 2023-03-09 13:52:45.000000 cgcsdk-1.0.7/cgc/tests/desired_responses/test_billing_stop_events_compute.txt
--rw-rw-rw-   0        0        0      302 2023-03-09 13:52:42.000000 cgcsdk-1.0.7/cgc/tests/desired_responses/test_billing_stop_events_volume.txt
--rw-rw-rw-   0        0        0      759 2023-03-10 08:35:09.000000 cgcsdk-1.0.7/cgc/tests/desired_responses/test_compute_list.txt
--rw-rw-rw-   0        0        0      155 2023-03-09 13:46:50.000000 cgcsdk-1.0.7/cgc/tests/desired_responses/test_compute_list_no_labels.txt
--rw-rw-rw-   0        0        0      789 2023-02-15 11:40:43.000000 cgcsdk-1.0.7/cgc/tests/desired_responses/test_tabulate_response.txt
--rw-rw-rw-   0        0        0      309 2023-03-09 13:52:32.000000 cgcsdk-1.0.7/cgc/tests/desired_responses/test_volume_list.txt
--rw-rw-rw-   0        0        0     9181 2023-04-14 14:28:08.000000 cgcsdk-1.0.7/cgc/tests/responses_tests.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:27:21.936790 cgcsdk-1.0.7/cgc/utils/
--rw-rw-rw-   0        0        0     3466 2023-06-13 12:13:50.000000 cgcsdk-1.0.7/cgc/utils/__init__.py
--rw-rw-rw-   0        0        0      633 2023-02-17 10:02:49.000000 cgcsdk-1.0.7/cgc/utils/click_group.py
--rw-rw-rw-   0        0        0     2729 2023-05-23 09:02:22.000000 cgcsdk-1.0.7/cgc/utils/config_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:27:22.076793 cgcsdk-1.0.7/cgc/utils/consts/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-1.0.7/cgc/utils/consts/__init__.py
--rw-rw-rw-   0        0        0     1286 2024-03-08 11:15:19.000000 cgcsdk-1.0.7/cgc/utils/consts/env_consts.py
--rw-rw-rw-   0        0        0     1218 2023-06-13 09:54:33.000000 cgcsdk-1.0.7/cgc/utils/consts/message_consts.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:27:22.235438 cgcsdk-1.0.7/cgc/utils/cryptography/
--rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-1.0.7/cgc/utils/cryptography/__init__.py
--rw-rw-rw-   0        0        0     3333 2022-09-30 09:28:09.000000 cgcsdk-1.0.7/cgc/utils/cryptography/aes_crypto.py
--rw-rw-rw-   0        0        0     1958 2022-09-30 09:28:09.000000 cgcsdk-1.0.7/cgc/utils/cryptography/encryption_module.py
--rw-rw-rw-   0        0        0     4180 2022-09-30 09:28:09.000000 cgcsdk-1.0.7/cgc/utils/cryptography/rsa_crypto.py
--rw-rw-rw-   0        0        0     2432 2024-04-04 10:26:21.000000 cgcsdk-1.0.7/cgc/utils/custom_exceptions.py
--rw-rw-rw-   0        0        0     1766 2023-10-30 10:18:38.000000 cgcsdk-1.0.7/cgc/utils/message_utils.py
--rw-rw-rw-   0        0        0     2561 2024-03-13 09:33:01.000000 cgcsdk-1.0.7/cgc/utils/prepare_headers.py
--rw-rw-rw-   0        0        0     2050 2023-06-13 11:20:10.000000 cgcsdk-1.0.7/cgc/utils/requests_helper.py
--rw-rw-rw-   0        0        0     7374 2024-03-08 11:15:19.000000 cgcsdk-1.0.7/cgc/utils/response_utils.py
--rw-rw-rw-   0        0        0      413 2022-12-02 13:13:31.000000 cgcsdk-1.0.7/cgc/utils/update.py
--rw-rw-rw-   0        0        0     3267 2023-06-13 11:20:10.000000 cgcsdk-1.0.7/cgc/utils/version_control.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:27:22.444849 cgcsdk-1.0.7/cgcsdk.egg-info/
--rw-rw-rw-   0        0        0     3173 2024-04-04 10:27:20.000000 cgcsdk-1.0.7/cgcsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2674 2024-04-04 10:27:20.000000 cgcsdk-1.0.7/cgcsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 10:27:20.000000 cgcsdk-1.0.7/cgcsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-04 10:27:20.000000 cgcsdk-1.0.7/cgcsdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      124 2024-04-04 10:27:20.000000 cgcsdk-1.0.7/cgcsdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-04 10:27:20.000000 cgcsdk-1.0.7/cgcsdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       97 2022-07-05 07:57:23.000000 cgcsdk-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-04 10:27:22.600011 cgcsdk-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2096 2023-06-13 11:20:10.000000 cgcsdk-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 14:23:16.492930 cgcsdk-1.0.9/
+-rw-rw-rw-   0        0        0        0 2022-04-21 08:27:42.000000 cgcsdk-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0      112 2023-06-13 11:20:10.000000 cgcsdk-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3056 2024-04-23 14:23:16.489178 cgcsdk-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1742 2024-04-16 11:34:36.000000 cgcsdk-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 14:23:16.162777 cgcsdk-1.0.9/cgc/
+-rw-rw-rw-   0        0        0      209 2024-04-23 13:55:23.000000 cgcsdk-1.0.9/cgc/.env
+-rw-rw-rw-   0        0        0     8255 2024-04-23 13:55:23.000000 cgcsdk-1.0.9/cgc/CHANGELOG.md
+-rw-rw-rw-   0        0        0      326 2023-04-18 09:56:45.000000 cgcsdk-1.0.9/cgc/__init__.py
+-rw-rw-rw-   0        0        0     1571 2024-04-10 12:49:45.000000 cgcsdk-1.0.9/cgc/cgc.py
+drwxrwxrwx   0        0        0        0 2024-04-23 14:23:16.184378 cgcsdk-1.0.9/cgc/commands/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-1.0.9/cgc/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 14:23:16.198523 cgcsdk-1.0.9/cgc/commands/auth/
+-rw-rw-rw-   0        0        0      397 2024-04-23 13:55:23.000000 cgcsdk-1.0.9/cgc/commands/auth/__init__.py
+-rw-rw-rw-   0        0        0     4196 2024-04-23 14:03:57.000000 cgcsdk-1.0.9/cgc/commands/auth/auth_cmd.py
+-rw-rw-rw-   0        0        0     1959 2024-04-23 13:55:23.000000 cgcsdk-1.0.9/cgc/commands/auth/auth_responses.py
+-rw-rw-rw-   0        0        0     5507 2024-04-23 14:18:13.000000 cgcsdk-1.0.9/cgc/commands/auth/auth_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-23 14:23:16.216694 cgcsdk-1.0.9/cgc/commands/billing/
+-rw-rw-rw-   0        0        0      753 2023-04-14 14:28:08.000000 cgcsdk-1.0.9/cgc/commands/billing/__init__.py
+-rw-rw-rw-   0        0        0     4140 2023-11-15 10:46:21.000000 cgcsdk-1.0.9/cgc/commands/billing/billing_cmd.py
+-rw-rw-rw-   0        0        0     1949 2023-04-14 14:28:08.000000 cgcsdk-1.0.9/cgc/commands/billing/billing_responses.py
+-rw-rw-rw-   0        0        0     4711 2023-06-14 08:36:45.000000 cgcsdk-1.0.9/cgc/commands/billing/billing_utils.py
+-rw-rw-rw-   0        0        0     4956 2024-04-04 10:26:21.000000 cgcsdk-1.0.9/cgc/commands/cgc_cmd.py
+-rw-rw-rw-   0        0        0     2245 2024-04-04 10:26:21.000000 cgcsdk-1.0.9/cgc/commands/cgc_cmd_responses.py
+-rw-rw-rw-   0        0        0     1174 2024-03-13 09:33:01.000000 cgcsdk-1.0.9/cgc/commands/cgc_helpers.py
+-rw-rw-rw-   0        0        0      182 2024-04-10 12:49:45.000000 cgcsdk-1.0.9/cgc/commands/cgc_models.py
+drwxrwxrwx   0        0        0        0 2024-04-23 14:23:16.240443 cgcsdk-1.0.9/cgc/commands/compute/
+-rw-rw-rw-   0        0        0      239 2023-02-15 11:40:43.000000 cgcsdk-1.0.9/cgc/commands/compute/__init__.py
+-rw-rw-rw-   0        0        0    15490 2024-03-13 09:36:12.000000 cgcsdk-1.0.9/cgc/commands/compute/compute_cmd.py
+-rw-rw-rw-   0        0        0      778 2024-04-16 11:34:36.000000 cgcsdk-1.0.9/cgc/commands/compute/compute_models.py
+-rw-rw-rw-   0        0        0     5807 2024-03-08 11:15:19.000000 cgcsdk-1.0.9/cgc/commands/compute/compute_responses.py
+-rw-rw-rw-   0        0        0     8812 2024-04-04 10:26:21.000000 cgcsdk-1.0.9/cgc/commands/compute/compute_utills.py
+drwxrwxrwx   0        0        0        0 2024-04-23 14:23:16.255282 cgcsdk-1.0.9/cgc/commands/db/
+-rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-1.0.9/cgc/commands/db/__init__.py
+-rw-rw-rw-   0        0        0     3513 2024-04-16 11:34:36.000000 cgcsdk-1.0.9/cgc/commands/db/db_cmd.py
+-rw-rw-rw-   0        0        0     1036 2024-04-23 13:55:23.000000 cgcsdk-1.0.9/cgc/commands/db/db_models.py
+drwxrwxrwx   0        0        0        0 2024-04-23 14:23:16.265807 cgcsdk-1.0.9/cgc/commands/debug/
+-rw-rw-rw-   0        0        0        0 2023-04-18 09:56:45.000000 cgcsdk-1.0.9/cgc/commands/debug/__init__.py
+-rw-rw-rw-   0        0        0      412 2023-04-17 11:02:43.000000 cgcsdk-1.0.9/cgc/commands/debug/debug_cmd.py
+-rw-rw-rw-   0        0        0      155 2024-04-16 11:34:36.000000 cgcsdk-1.0.9/cgc/commands/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-23 14:23:16.282543 cgcsdk-1.0.9/cgc/commands/jobs/
+-rw-rw-rw-   0        0        0      231 2024-04-04 10:26:21.000000 cgcsdk-1.0.9/cgc/commands/jobs/__init__.py
+-rw-rw-rw-   0        0        0     6195 2024-04-23 13:55:23.000000 cgcsdk-1.0.9/cgc/commands/jobs/job_utils.py
+-rw-rw-rw-   0        0        0     6555 2024-04-04 10:26:21.000000 cgcsdk-1.0.9/cgc/commands/jobs/jobs_cmd.py
+-rw-rw-rw-   0        0        0     1771 2024-04-23 13:55:23.000000 cgcsdk-1.0.9/cgc/commands/jobs/jobs_responses.py
+drwxrwxrwx   0        0        0        0 2024-04-23 14:23:16.299716 cgcsdk-1.0.9/cgc/commands/keys/
+-rw-rw-rw-   0        0        0      112 2024-04-10 12:49:45.000000 cgcsdk-1.0.9/cgc/commands/keys/__init__.py
+-rw-rw-rw-   0        0        0     4437 2024-04-10 13:23:29.000000 cgcsdk-1.0.9/cgc/commands/keys/keys_cmd.py
+-rw-rw-rw-   0        0        0      378 2024-04-10 12:49:45.000000 cgcsdk-1.0.9/cgc/commands/keys/keys_models.py
+-rw-rw-rw-   0        0        0     1474 2024-04-16 11:34:36.000000 cgcsdk-1.0.9/cgc/commands/keys/keys_responses.py
+-rw-rw-rw-   0        0        0     2285 2024-04-10 13:23:29.000000 cgcsdk-1.0.9/cgc/commands/keys/keys_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-23 14:23:16.313306 cgcsdk-1.0.9/cgc/commands/resource/
+-rw-rw-rw-   0        0        0        0 2023-04-14 14:28:08.000000 cgcsdk-1.0.9/cgc/commands/resource/__init__.py
+-rw-rw-rw-   0        0        0     4090 2024-04-16 11:34:36.000000 cgcsdk-1.0.9/cgc/commands/resource/resource_cmd.py
+-rw-rw-rw-   0        0        0      197 2023-11-21 14:55:48.000000 cgcsdk-1.0.9/cgc/commands/resource/resource_responses.py
+drwxrwxrwx   0        0        0        0 2024-04-23 14:23:16.334491 cgcsdk-1.0.9/cgc/commands/volume/
+-rw-rw-rw-   0        0        0      384 2023-02-15 11:40:43.000000 cgcsdk-1.0.9/cgc/commands/volume/__init__.py
+-rw-rw-rw-   0        0        0     1295 2023-10-30 10:06:10.000000 cgcsdk-1.0.9/cgc/commands/volume/data_model.py
+-rw-rw-rw-   0        0        0     7673 2024-03-13 09:33:01.000000 cgcsdk-1.0.9/cgc/commands/volume/volume_cmd.py
+-rw-rw-rw-   0        0        0     3199 2023-02-15 11:40:43.000000 cgcsdk-1.0.9/cgc/commands/volume/volume_responses.py
+-rw-rw-rw-   0        0        0     1919 2023-02-15 11:40:43.000000 cgcsdk-1.0.9/cgc/commands/volume/volume_utils.py
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-1.0.9/cgc/config.py
+drwxrwxrwx   0        0        0        0 2024-04-23 14:23:16.352511 cgcsdk-1.0.9/cgc/sdk/
+-rw-rw-rw-   0        0        0      177 2024-04-16 11:34:36.000000 cgcsdk-1.0.9/cgc/sdk/__init__.py
+-rw-rw-rw-   0        0        0      214 2024-03-08 13:51:26.000000 cgcsdk-1.0.9/cgc/sdk/exceptions.py
+-rw-rw-rw-   0        0        0     5318 2024-04-16 11:34:36.000000 cgcsdk-1.0.9/cgc/sdk/job.py
+-rw-rw-rw-   0        0        0     1637 2023-04-18 10:57:57.000000 cgcsdk-1.0.9/cgc/sdk/postgresql.py
+-rw-rw-rw-   0        0        0    13544 2024-04-04 10:26:21.000000 cgcsdk-1.0.9/cgc/sdk/resource.py
+-rw-rw-rw-   0        0        0     1452 2023-05-31 13:31:37.000000 cgcsdk-1.0.9/cgc/server.crt
+drwxrwxrwx   0        0        0        0 2024-04-23 14:23:16.362195 cgcsdk-1.0.9/cgc/telemetry/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-1.0.9/cgc/telemetry/__init__.py
+-rw-rw-rw-   0        0        0     3175 2023-05-18 12:51:21.000000 cgcsdk-1.0.9/cgc/telemetry/basic.py
+drwxrwxrwx   0        0        0        0 2024-04-23 14:23:16.368749 cgcsdk-1.0.9/cgc/tests/
+-rw-rw-rw-   0        0        0   102743 2023-07-17 12:07:43.000000 cgcsdk-1.0.9/cgc/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 14:23:16.395340 cgcsdk-1.0.9/cgc/tests/desired_responses/
+-rw-rw-rw-   0        0        0     1579 2023-03-09 13:52:51.000000 cgcsdk-1.0.9/cgc/tests/desired_responses/test_billing_invoice.txt
+-rw-rw-rw-   0        0        0     2381 2023-03-09 13:52:48.000000 cgcsdk-1.0.9/cgc/tests/desired_responses/test_billing_status.txt
+-rw-rw-rw-   0        0        0      234 2023-03-09 13:52:45.000000 cgcsdk-1.0.9/cgc/tests/desired_responses/test_billing_stop_events_compute.txt
+-rw-rw-rw-   0        0        0      302 2023-03-09 13:52:42.000000 cgcsdk-1.0.9/cgc/tests/desired_responses/test_billing_stop_events_volume.txt
+-rw-rw-rw-   0        0        0      759 2023-03-10 08:35:09.000000 cgcsdk-1.0.9/cgc/tests/desired_responses/test_compute_list.txt
+-rw-rw-rw-   0        0        0      155 2023-03-09 13:46:50.000000 cgcsdk-1.0.9/cgc/tests/desired_responses/test_compute_list_no_labels.txt
+-rw-rw-rw-   0        0        0      789 2023-02-15 11:40:43.000000 cgcsdk-1.0.9/cgc/tests/desired_responses/test_tabulate_response.txt
+-rw-rw-rw-   0        0        0      309 2023-03-09 13:52:32.000000 cgcsdk-1.0.9/cgc/tests/desired_responses/test_volume_list.txt
+-rw-rw-rw-   0        0        0     9181 2023-04-14 14:28:08.000000 cgcsdk-1.0.9/cgc/tests/responses_tests.py
+drwxrwxrwx   0        0        0        0 2024-04-23 14:23:16.432808 cgcsdk-1.0.9/cgc/utils/
+-rw-rw-rw-   0        0        0     3669 2024-04-23 13:55:23.000000 cgcsdk-1.0.9/cgc/utils/__init__.py
+-rw-rw-rw-   0        0        0      633 2023-02-17 10:02:49.000000 cgcsdk-1.0.9/cgc/utils/click_group.py
+-rw-rw-rw-   0        0        0     2884 2024-04-23 14:18:13.000000 cgcsdk-1.0.9/cgc/utils/config_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-23 14:23:16.444222 cgcsdk-1.0.9/cgc/utils/consts/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-1.0.9/cgc/utils/consts/__init__.py
+-rw-rw-rw-   0        0        0     1290 2024-04-23 13:55:23.000000 cgcsdk-1.0.9/cgc/utils/consts/env_consts.py
+-rw-rw-rw-   0        0        0     1218 2023-06-13 09:54:33.000000 cgcsdk-1.0.9/cgc/utils/consts/message_consts.py
+drwxrwxrwx   0        0        0        0 2024-04-23 14:23:16.460985 cgcsdk-1.0.9/cgc/utils/cryptography/
+-rw-rw-rw-   0        0        0        0 2022-09-30 09:28:09.000000 cgcsdk-1.0.9/cgc/utils/cryptography/__init__.py
+-rw-rw-rw-   0        0        0     3333 2022-09-30 09:28:09.000000 cgcsdk-1.0.9/cgc/utils/cryptography/aes_crypto.py
+-rw-rw-rw-   0        0        0     1958 2022-09-30 09:28:09.000000 cgcsdk-1.0.9/cgc/utils/cryptography/encryption_module.py
+-rw-rw-rw-   0        0        0     4180 2022-09-30 09:28:09.000000 cgcsdk-1.0.9/cgc/utils/cryptography/rsa_crypto.py
+-rw-rw-rw-   0        0        0     2628 2024-04-10 12:49:45.000000 cgcsdk-1.0.9/cgc/utils/custom_exceptions.py
+-rw-rw-rw-   0        0        0     1790 2024-04-10 12:49:45.000000 cgcsdk-1.0.9/cgc/utils/message_utils.py
+-rw-rw-rw-   0        0        0     2838 2024-04-23 14:18:13.000000 cgcsdk-1.0.9/cgc/utils/prepare_headers.py
+-rw-rw-rw-   0        0        0     2038 2024-04-10 12:49:45.000000 cgcsdk-1.0.9/cgc/utils/requests_helper.py
+-rw-rw-rw-   0        0        0     7374 2024-03-08 11:15:19.000000 cgcsdk-1.0.9/cgc/utils/response_utils.py
+-rw-rw-rw-   0        0        0      413 2022-12-02 13:13:31.000000 cgcsdk-1.0.9/cgc/utils/update.py
+-rw-rw-rw-   0        0        0     3267 2023-06-13 11:20:10.000000 cgcsdk-1.0.9/cgc/utils/version_control.py
+drwxrwxrwx   0        0        0        0 2024-04-23 14:23:16.486263 cgcsdk-1.0.9/cgcsdk.egg-info/
+-rw-rw-rw-   0        0        0     3056 2024-04-23 14:23:16.000000 cgcsdk-1.0.9/cgcsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2835 2024-04-23 14:23:16.000000 cgcsdk-1.0.9/cgcsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 14:23:16.000000 cgcsdk-1.0.9/cgcsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-23 14:23:16.000000 cgcsdk-1.0.9/cgcsdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2024-04-23 14:23:16.000000 cgcsdk-1.0.9/cgcsdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-23 14:23:16.000000 cgcsdk-1.0.9/cgcsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       97 2022-07-05 07:57:23.000000 cgcsdk-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-23 14:23:16.493934 cgcsdk-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2060 2024-04-16 11:34:36.000000 cgcsdk-1.0.9/setup.py
```

### Comparing `cgcsdk-1.0.7/PKG-INFO` & `cgcsdk-1.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgcsdk
-Version: 1.0.7
+Version: 1.0.9
 Summary: Comtegra GPU Cloud REST API client
 Author: Comtegra AI Team
 Author-email: ai@comtegra.pl
 License: BSD 2-clause
 Project-URL: Documentation, https://example.com/documentation/
 Project-URL: GitHub, https://github.com/foobar/foobar/
 Project-URL: Changelog, https://github.com/foobar/foobar/blob/master/CHANGELOG.md
@@ -26,16 +26,14 @@
 Requires-Dist: tabulate
 Requires-Dist: pycryptodomex
 Requires-Dist: paramiko>=2.11
 Requires-Dist: statsd
 Requires-Dist: requests
 Requires-Dist: setuptools
 Requires-Dist: colorama
-Requires-Dist: redis
-Requires-Dist: pymongo
 Requires-Dist: psycopg2-binary
 
 # Comtegra GPU Cloud CLI Client
 
 ## Basic info
 
 CGC Clinet is complete solution to create and manage your compute resources through CLI interface and python code. It incorporates CLI and SDK in one package.
@@ -50,18 +48,16 @@
 2. [Triton inferencing server](https://docs.nvidia.com/deeplearning/triton-inference-server/) for large scale inferencing
 3. [Label studio](https://labelstud.io/) for easy management of your data annotation tasks with variety of modes
 4. [Rapids](https://rapids.ai/) suite of accelerated libraries for data processing
 
 Notebooks are equiped with all CUDA libraries and GPU drivers which enables the usage of GPU for accelerated computations.
 Apart from compute resources, we provide the database engines accessible from within your namespace:
 
-1. [MongoDB](https://www.mongodb.org/)
-2. [PostgreSQL](https://www.postgresql.org/)
-3. [Redis](https://redis.io/)
-4. [Weaviate](https://weaviate.io/)
+1. [PostgreSQL](https://www.postgresql.org/)
+2. [Weaviate](https://weaviate.io/)
 
 More are coming!
 Please follow instructions to get started.
 
 ## More info
 
 If you'd like to know more visit:
```

### Comparing `cgcsdk-1.0.7/README.md` & `cgcsdk-1.0.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -14,18 +14,16 @@
 2. [Triton inferencing server](https://docs.nvidia.com/deeplearning/triton-inference-server/) for large scale inferencing
 3. [Label studio](https://labelstud.io/) for easy management of your data annotation tasks with variety of modes
 4. [Rapids](https://rapids.ai/) suite of accelerated libraries for data processing
 
 Notebooks are equiped with all CUDA libraries and GPU drivers which enables the usage of GPU for accelerated computations.
 Apart from compute resources, we provide the database engines accessible from within your namespace:
 
-1. [MongoDB](https://www.mongodb.org/)
-2. [PostgreSQL](https://www.postgresql.org/)
-3. [Redis](https://redis.io/)
-4. [Weaviate](https://weaviate.io/)
+1. [PostgreSQL](https://www.postgresql.org/)
+2. [Weaviate](https://weaviate.io/)
 
 More are coming!
 Please follow instructions to get started.
 
 ## More info
 
 If you'd like to know more visit:
```

### Comparing `cgcsdk-1.0.7/cgc/CHANGELOG.md` & `cgcsdk-1.0.9/cgc/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,28 @@
 # Change Log
 
+## 1.0.9
+
+Release on April 23, 2024
+
+* updated cgc to work with cgc-server 1.1.0
+* updated registration process
+* updated available apps, so it reflects changes in cgc-server
+* hotfix: listening jobs, which are not Running
+
+## 1.0.8
+
+Release on April 11, 2024
+
+* added new command group: cgc keys
+  * ssh create - create new ssh key, for ssh access
+  * ssh list - list all ssh keys
+  * ssh delete - delete ssh key
+  * ssh update - update ssh key
+
 ## 1.0.7
 
 Release on April 04, 2024
 
 * speed of resource creation with volumes / shared memory, has been improved
 * added jobs creation: cgc job create
 * added jobs list: cgc job list
```

### Comparing `cgcsdk-1.0.7/cgc/cgc.py` & `cgcsdk-1.0.9/cgc/cgc.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     cgc_rm,
     cgc_status,
     cgc_logs,
     sending_telemetry_permission,
     resource_events,
     context_group,
 )
+from cgc.commands.keys.keys_cmd import keys_group
 
 from cgc.utils.version_control import check_version, _get_version
 from cgc.utils.click_group import CustomGroup
 
 
 @click.group(cls=CustomGroup)
 @click.version_option(_get_version())
@@ -42,12 +43,13 @@
 cli.add_command(resource_events)
 cli.add_command(resource_group)
 cli.add_command(billing_group)
 cli.add_command(cgc_status)
 cli.add_command(sending_telemetry_permission)
 cli.add_command(cgc_logs)
 cli.add_command(job_group)
+cli.add_command(keys_group)
 
 if __name__ == "__main__" or __name__ == "cgc.cgc":
     cli()
 else:
     raise Exception("This program is not intended for importing!")
```

### Comparing `cgcsdk-1.0.7/cgc/commands/auth/auth_cmd.py` & `cgcsdk-1.0.9/cgc/commands/auth/auth_cmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,25 +5,30 @@
     login_successful_response,
 )
 from cgc.commands.auth.auth_utils import (
     auth_create_api_key_with_save,
     auth_delete_api_key,
     auth_list_api_keys,
 )
-from cgc.utils.prepare_headers import get_url_and_prepare_headers_register
+from cgc.utils.prepare_headers import (
+    get_url_and_prepare_headers_register,
+    load_user_api_url,
+    load_user_cgc_secret,
+)
 from cgc.utils.cryptography import rsa_crypto
 from cgc.utils.click_group import CustomCommand, CustomGroup
 from cgc.utils.requests_helper import call_api, EndpointTypes
 from cgc.utils.response_utils import (
     fill_missing_values_in_a_response,
     retrieve_and_validate_response_send_metric,
     tabulate_a_response,
 )
 from cgc.utils import (
     check_if_config_exist,
+    require_answer_loop,
     require_confirm_loop,
     find_first_available_config_name,
 )
 
 
 @click.group("api-keys", cls=CustomGroup, hidden=False)
 def api_keys_group():
@@ -51,17 +56,22 @@
     """
 
     if check_if_config_exist(config_filename):
         click.echo("Already registered.")
         require_confirm_loop("Do you want to add new context?")
         config_filename = find_first_available_config_name()
 
+    cgc_api_url = require_answer_loop("Enter CGC server address", load_user_api_url())
+    cgc_secret = require_answer_loop("Enter CGC secret", load_user_cgc_secret())
+
     user_id = input("User ID: ")
     access_key = input("Access key: ")
-    url, headers = get_url_and_prepare_headers_register(user_id, access_key)
+    url, headers = get_url_and_prepare_headers_register(
+        user_id, access_key, cgc_api_url, cgc_secret
+    )
     metric = "auth.register"
     pub_key_bytes, priv_key_bytes = rsa_crypto.key_generate_pair()
     __payload = pub_key_bytes
     __res = call_api(
         request=EndpointTypes.post,
         url=url,
         headers=headers,
@@ -70,14 +80,16 @@
     )
     click.echo(
         auth_register_response(
             retrieve_and_validate_response_send_metric(__res, metric, False),
             user_id,
             priv_key_bytes,
             config_filename,
+            cgc_api_url,
+            cgc_secret,
         )
     )
 
 
 @api_keys_group.command("create", cls=CustomCommand)
 @click.option(
     "--user",
```

### Comparing `cgcsdk-1.0.7/cgc/commands/auth/auth_responses.py` & `cgcsdk-1.0.9/cgc/commands/auth/auth_responses.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,22 +4,29 @@
 from cgc.commands.auth import auth_utils
 from cgc.utils.consts.env_consts import TMP_DIR, get_config_file_name
 from cgc.utils.config_utils import get_config_path, save_to_config
 from cgc.utils.message_utils import key_error_decorator_for_helpers
 
 
 @key_error_decorator_for_helpers
-def auth_register_response(response, user_id, priv_key_bytes, config_filename) -> str:
+def auth_register_response(
+    response, user_id, priv_key_bytes, config_filename, cgc_api_url, cgc_secret
+) -> str:
     TMP_DIR_PATH = os.path.join(get_config_path(), TMP_DIR)
     unzip_dir, namespace = auth_utils.save_and_unzip_file(response)
     aes_key, password = auth_utils.get_aes_key_and_password(unzip_dir, priv_key_bytes)
 
     os.environ["CONFIG_FILE_NAME"] = config_filename
     save_to_config(
-        user_id=user_id, password=password, aes_key=aes_key, namespace=namespace
+        user_id=user_id,
+        password=password,
+        aes_key=aes_key,
+        namespace=namespace,
+        cgc_api_url=cgc_api_url,
+        cgc_secret=cgc_secret,
     )
     auth_utils.auth_create_api_key_with_save()
     shutil.rmtree(TMP_DIR_PATH)
     # config.json
     if config_filename == "config.json":
         return f"Register successful! You can now use the CLI. Saved data to:{os.path.join(get_config_path(),config_filename)}\n\
         Consider backup this file. It stores data accessible only to you with which you can access CGC platform."
```

### Comparing `cgcsdk-1.0.7/cgc/commands/auth/auth_utils.py` & `cgcsdk-1.0.9/cgc/commands/auth/auth_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import requests
 
 from cgc.utils.config_utils import get_config_path
 from cgc.utils.config_utils import save_to_config
 from cgc.utils.config_utils import read_from_cfg
 from cgc.utils.cryptography import rsa_crypto
 from cgc.utils import prepare_headers
-from cgc.utils.consts.env_consts import API_URL, TMP_DIR
+from cgc.utils.consts.env_consts import TMP_DIR
 
 from cgc.utils.requests_helper import call_api, EndpointTypes
 from cgc.utils.response_utils import retrieve_and_validate_response_send_metric
 
 TMP_DIR_PATH = os.path.join(get_config_path(), TMP_DIR)
 
 
@@ -25,17 +25,18 @@
     :type user_id: str
     :param password: _description_
     :type password: str
     """
     if user_id is None or password is None:
         if user_id is not None or password is not None:
             raise ValueError("Both user_id and password must be provided")
+    if user_id is None and password is None:
         user_id = urllib.parse.quote(read_from_cfg("user_id"))
         password = urllib.parse.quote(read_from_cfg("password"))
-    url = f"{API_URL}/v1/api/user/create/token"
+    url = f"{prepare_headers.load_user_api_url()}/v1/api/user/create/token"
     headers = {
         "accept": "application/json",
         "Content-Type": "application/x-www-form-urlencoded",
     }
     metric = "auth.jwt"
     __payload = f"grant_type=&username={user_id}&password={password}"
     __res = call_api(
@@ -50,15 +51,15 @@
 def get_jwt(user_id: str = None, password: str = None) -> str:
     json_data = _get_jwt_from_server(user_id, password)
     return json_data["access_token"]
 
 
 def auth_create_api_key_with_save(user_id: str = None, password: str = None):
     """Function to create API key and API secret for user and save it to config file."""
-    url = f"{API_URL}/v1/api/user/create/api-key"
+    url = f"{prepare_headers.load_user_api_url()}/v1/api/user/create/api-key"
     headers = prepare_headers.prepare_headers_api_key(user_id, password)
     metric = "auth.api-key"
     __res = call_api(
         request=EndpointTypes.post,
         url=url,
         headers=headers,
     )
@@ -70,30 +71,30 @@
     if user_id is not None and password is not None:
         save_to_config(user_id=user_id, password=password)
     return api_key, secret
 
 
 def auth_delete_api_key(api_key: str, user_id: str = None, password: str = None):
     """Function to delete API key."""
-    url = f"{API_URL}/v1/api/user/delete/api-key?api_key={api_key}"
+    url = f"{prepare_headers.load_user_api_url()}/v1/api/user/delete/api-key?api_key={api_key}"
     headers = prepare_headers.prepare_headers_api_key(user_id, password)
     metric = "auth.api-key"
     __res = call_api(
         request=EndpointTypes.delete,
         url=url,
         headers=headers,
     )
 
     json_data = retrieve_and_validate_response_send_metric(__res, metric)
     return json_data["details"]
 
 
 def auth_list_api_keys(user_id: str = None, password: str = None):
     """Function to list API keys."""
-    url = f"{API_URL}/v1/api/user/list/api-key"
+    url = f"{prepare_headers.load_user_api_url()}/v1/api/user/list/api-key"
     headers = prepare_headers.prepare_headers_api_key(user_id, password)
     metric = "auth.api-key"
     __res = call_api(
         request=EndpointTypes.get,
         url=url,
         headers=headers,
     )
```

### Comparing `cgcsdk-1.0.7/cgc/commands/billing/__init__.py` & `cgcsdk-1.0.9/cgc/commands/billing/__init__.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/commands/billing/billing_cmd.py` & `cgcsdk-1.0.9/cgc/commands/billing/billing_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/commands/billing/billing_responses.py` & `cgcsdk-1.0.9/cgc/commands/billing/billing_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/commands/billing/billing_utils.py` & `cgcsdk-1.0.9/cgc/commands/billing/billing_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/commands/cgc_cmd.py` & `cgcsdk-1.0.9/cgc/commands/cgc_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/commands/cgc_cmd_responses.py` & `cgcsdk-1.0.9/cgc/commands/cgc_cmd_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/commands/cgc_helpers.py` & `cgcsdk-1.0.9/cgc/commands/cgc_helpers.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/commands/compute/compute_cmd.py` & `cgcsdk-1.0.9/cgc/commands/compute/compute_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/commands/compute/compute_models.py` & `cgcsdk-1.0.9/cgc/commands/compute/compute_models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,8 @@
-from enum import Enum
-
-
-class CGCEntityList(Enum):
-    """Base class for other lists"""
-
-    @classmethod
-    def get_list(cls) -> list[str]:
-        return [el.value for el in cls]
+from cgc.commands.cgc_models import CGCEntityList
 
 
 class ComputesList(CGCEntityList):
     """List of templates in cgc-server
 
     :param Enum: name of template
     :type Enum: str
@@ -25,28 +17,14 @@
     COMFY_UI = "comfy-ui"
     RAG = "rag"
     DEEPSTREAM = "deepstream"
     T2V_TRANSFORMERS = "t2v-transformers"
     CUSTOM = "custom"
 
 
-class DatabasesList(CGCEntityList):
-    """List of templates in cgc-server
-
-    :param Enum: name of template
-    :type Enum: str
-    """
-
-    MONGODB = "mongodb"
-    POSTGRESQL = "postgresql"
-    REDIS = "redis"
-    WEAVIATE = "weaviate"
-    # MINIO = "minio"
-
-
 class GPUsList(CGCEntityList):
     """List of templates in cgc-server
 
     :param Enum: name of template
     :type Enum: str
     """
```

### Comparing `cgcsdk-1.0.7/cgc/commands/compute/compute_responses.py` & `cgcsdk-1.0.9/cgc/commands/compute/compute_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/commands/compute/compute_utills.py` & `cgcsdk-1.0.9/cgc/commands/compute/compute_utills.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/commands/db/db_cmd.py` & `cgcsdk-1.0.9/cgc/commands/db/db_cmd.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import click
 
 from cgc.commands.compute.compute_responses import compute_list_response
-from cgc.commands.compute.compute_models import DatabasesList
+from cgc.commands.db.db_models import DatabasesList
 from cgc.commands.compute.compute_responses import compute_create_response
 from cgc.commands.compute.compute_utills import compute_create_payload
+from cgc.commands.exceptions import DatabaseCreationException
 from cgc.commands.resource.resource_cmd import resource_delete
 from cgc.utils.prepare_headers import get_api_url_and_prepare_headers
 from cgc.utils.response_utils import retrieve_and_validate_response_send_metric
 from cgc.utils.click_group import CustomGroup, CustomCommand
 from cgc.utils.requests_helper import call_api, EndpointTypes
 
 
@@ -62,14 +63,19 @@
     :param memory: GB of memory to be used by app
     :type memory: int
     :param volumes: list of volumes to mount
     :type volumes: list[str]
     :param name: name of app
     :type name: str
     """
+    try:
+        DatabasesList.verify(entity)
+    except DatabaseCreationException as e:
+        click.echo(e, err=True, color="yellow")
+        return
     api_url, headers = get_api_url_and_prepare_headers()
     url = f"{api_url}/v1/api/resource/create"
     metric = "db.create"
     __payload = compute_create_payload(
         name=name,
         entity=entity,
         cpu=cpu,
```

### Comparing `cgcsdk-1.0.7/cgc/commands/jobs/job_utils.py` & `cgcsdk-1.0.9/cgc/commands/jobs/job_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -102,74 +102,79 @@
                     )
             payload["config_maps_data"] = config_maps_data_dict
     except TypeError:
         pass
     return payload
 
 
-def get_job_list(job_pod_list: list, job_list: list):
-    list_of_json_data = get_job_pod_list(job_pod_list)
-    for json_data in list_of_json_data:
-        for job in job_list:
-            if job.get("name") == json_data.get("name"):
-                json_data["ttl_seconds_after_finished"] = job.get(
-                    "ttl_seconds_after_finished", "N/A"
-                )
+def get_job_list(job_list: list, job_pod_list: list):
+    list_of_json_job_data = get_job_json_data(job_list)
+
+    for i, job_data in enumerate(job_list):
+        list_of_json_job_data[i]["name"] = job_data.get("name", "")
+        list_of_json_job_data[i]["ttl_seconds_after_finished"] = job_data.get(
+            "ttl_seconds_after_finished", "N/A"
+        )
+    for job in list_of_json_job_data:
+        for job_pod in job_pod_list:
+            if job_pod.get("labels", {}).get("app-name") == job.get("name"):
+                job["status"] = job_pod.get("status", "Pending")
+                # job["status_reason"] = [
+                #     x.get("reason", "N/A") for x in job_pod.get("status_reasons", [])
+                # ]
+                # job["status_message"] = [
+                #     x.get("message", "N/A") for x in job_pod.get("status_reasons", [])
+                # ]
                 break
-    return list_of_json_data
+
+    return list_of_json_job_data
 
 
-def get_job_pod_list(job_pod_list: list) -> list:
+def get_job_json_data(job_list: list):
     """Formats and returns list of jobs to print.
 
-    :param pod_list: list of pods
-    :type pod_list: list
-    :return: formatted list of apps
+    :param job_list: list of jobs
+    :type job_list: list
+    :return: formatted list of jobs
     :rtype: list
     """
     output_data = []
 
-    for pod in job_pod_list:
+    for job in job_list:
         try:
             main_container_name = "custom-job"
             try:
                 main_container = [
                     x
-                    for x in pod.get("containers", [])
+                    for x in job.get("containers", [])
                     if x.get("name") == main_container_name
                 ][0]
             except IndexError:
                 raise Exception(
                     "Parser was unable to find main container in server output in container list"
                 )
             volumes_mounted = list_get_mounted_volumes(main_container.get("mounts", []))
             limits = main_container.get("resources", {}).get("limits")
             cpu = limits.get("cpu") if limits is not None else 0
             ram = limits.get("memory") if limits is not None else "0Gi"
 
-            pod_data = {
-                "name": pod.get("labels", {}).get("app-name"),
-                "status": pod.get("status", {}),
+            job_data = {
+                "name": job.get("labels", {}).get("app-name"),
+                "status": job.get("status", {}).get("phase", "Pending"),
                 "volumes_mounted": volumes_mounted,
                 "cpu": cpu,
                 "ram": ram,
-                "gpu-count": pod.get("labels", {}).get("gpu-count", 0),
-                "gpu-label": pod.get("labels", {}).get("gpu-label", "N/A"),
+                "gpu-count": job.get("labels", {}).get("gpu-count", 0),
+                "gpu-label": job.get("labels", {}).get("gpu-label", "N/A"),
             }
             # getting rid of unwanted and used values
-            if "pod-template-hash" in pod["labels"].keys():
-                pod["labels"].pop("pod-template-hash")
-            pod["labels"].pop("app-name")
-            pod["labels"].pop("entity")
-            pod["labels"].pop("resource-type")
-            pod["labels"].pop("job-name")
-            pod["labels"].pop("controller-uid")
-            pod["labels"].pop("api-key-id", None)
-            pod["labels"].pop("user-id", None)
+            if "pod-template-hash" in job["labels"].keys():
+                job["labels"].pop("pod-template-hash")
+            job["labels"].pop("entity")
 
             # appending the rest of labels
-            pod_data.update(pod["labels"])
-            output_data.append(pod_data)
+            job_data.update(job["labels"])
+            output_data.append(job_data)
         except KeyError:
             pass
 
     return output_data
```

### Comparing `cgcsdk-1.0.7/cgc/commands/jobs/jobs_cmd.py` & `cgcsdk-1.0.9/cgc/commands/jobs/jobs_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/commands/jobs/jobs_responses.py` & `cgcsdk-1.0.9/cgc/commands/jobs/jobs_responses.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     job_pod_list = data.get("details", {}).get("job_pod_list", [])
     job_list = data.get("details", {}).get("job_list", [])
     setup_gauge(f"{get_namespace()}.job.count", len(job_list))
 
     if not job_list:
         raise NoJobsToList()
 
-    list_of_json_data = get_job_list(job_pod_list, job_list)
+    list_of_json_data = get_job_list(job_list, job_pod_list)
     table = fill_missing_values_in_a_response(list_of_json_data)
 
     return tabulate_a_response(table)
 
 
 @key_error_decorator_for_helpers
 def job_create_response(data: dict) -> str:
```

### Comparing `cgcsdk-1.0.7/cgc/commands/resource/resource_cmd.py` & `cgcsdk-1.0.9/cgc/commands/resource/resource_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import click
 import json
 
-from cgc.commands.compute.compute_models import ComputesList, DatabasesList
+from cgc.commands.db.db_models import DatabasesList
+from cgc.commands.compute.compute_models import ComputesList
 from cgc.commands.compute.compute_responses import (
     template_list_response,
     template_get_start_path_response,
     compute_restart_response,
     compute_delete_response,
 )
```

### Comparing `cgcsdk-1.0.7/cgc/commands/volume/data_model.py` & `cgcsdk-1.0.9/cgc/commands/volume/data_model.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/commands/volume/volume_cmd.py` & `cgcsdk-1.0.9/cgc/commands/volume/volume_cmd.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/commands/volume/volume_responses.py` & `cgcsdk-1.0.9/cgc/commands/volume/volume_responses.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/commands/volume/volume_utils.py` & `cgcsdk-1.0.9/cgc/commands/volume/volume_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/sdk/job.py` & `cgcsdk-1.0.9/cgc/sdk/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     )
 
     return _response_utils.retrieve_and_validate_response_send_metric_for_sdk(
         __res, metric
     )
     # job_pod_list = _response.get("details", {}).get("job_pod_list", [])
     # job_list = _response.get("details", {}).get("job_list", [])
-    # return _job_utils.get_job_list(job_pod_list, job_list)
+    # return _job_utils.get_job_list(job_list)
 
 
 def job_delete(name: str):
     """
     Delete job using backend endpoint.
 
     :param name: name of job to delete
```

### Comparing `cgcsdk-1.0.7/cgc/sdk/postgresql.py` & `cgcsdk-1.0.9/cgc/sdk/postgresql.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/sdk/resource.py` & `cgcsdk-1.0.9/cgc/sdk/resource.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/server.crt` & `cgcsdk-1.0.9/cgc/server.crt`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/telemetry/basic.py` & `cgcsdk-1.0.9/cgc/telemetry/basic.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/tests/__init__.py` & `cgcsdk-1.0.9/cgc/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/tests/desired_responses/test_billing_invoice.txt` & `cgcsdk-1.0.9/cgc/tests/desired_responses/test_billing_invoice.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/tests/desired_responses/test_billing_status.txt` & `cgcsdk-1.0.9/cgc/tests/desired_responses/test_billing_status.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/tests/desired_responses/test_compute_list.txt` & `cgcsdk-1.0.9/cgc/tests/desired_responses/test_compute_list.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/tests/desired_responses/test_tabulate_response.txt` & `cgcsdk-1.0.9/cgc/tests/desired_responses/test_tabulate_response.txt`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/tests/responses_tests.py` & `cgcsdk-1.0.9/cgc/tests/responses_tests.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/utils/__init__.py` & `cgcsdk-1.0.9/cgc/utils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,22 @@
         answer = input(f"{message} (Y/N): ").lower()
         if answer in ("y", "yes"):
             break
         if answer in ("n", "no"):
             exit(0)
 
 
+def require_answer_loop(message: str, default: str):
+    while True:
+        answer = input(f"{message}: [{default}]").lower()
+        if answer == "":
+            return default
+        return answer
+
+
 def quick_sort(collection: list) -> list:
     """A pure Python implementation of quick sort algorithm
 
     :param collection: a mutable collection of comparable items
     :return: the same collection ordered by ascending
 
     Examples:
```

### Comparing `cgcsdk-1.0.7/cgc/utils/click_group.py` & `cgcsdk-1.0.9/cgc/utils/click_group.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/utils/config_utils.py` & `cgcsdk-1.0.9/cgc/utils/config_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import os
 import sys
 import click
 
 from cgc.commands.auth import NoNamespaceInConfig, NoConfigFileFound
 from cgc.utils.message_utils import prepare_error_message
-from cgc.utils.consts.env_consts import get_config_file_name
+from cgc.utils.consts.env_consts import CGC_API_URL, CGC_SECRET, get_config_file_name
 
 
 def get_config_path():
     """Function to get the path to the config file
 
     :return: path to the config file
     :rtype: str
@@ -74,14 +74,18 @@
                 return read_cfg
             return read_cfg[key]
     except FileNotFoundError:
         raise NoConfigFileFound()
     except KeyError:
         if key == "namespace":
             raise NoNamespaceInConfig()
+        elif key == "cgc_secret":
+            return CGC_SECRET
+        elif key == "cgc_api_url":
+            return CGC_API_URL
         print("Config file is corrupted. Please contact support at support@comtegra.pl")
         sys.exit()
 
 
 def get_namespace() -> str:
     """Function to get the namespace from the config file
```

### Comparing `cgcsdk-1.0.7/cgc/utils/consts/env_consts.py` & `cgcsdk-1.0.9/cgc/utils/consts/env_consts.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     __prefix = "https"
 elif API_SECURE_CONNECTION == "no":
     __prefix = "http"
 else:
     raise Exception("not defined API_SECURE_CONNECTION. set yes/no")
 
 API_PORT = os.getenv("API_PORT")
-API_URL = f"{__prefix}://{API_HOST}:{API_PORT}"
+CGC_API_URL = f"{__prefix}://{API_HOST}:{API_PORT}"
 TMP_DIR = os.getenv("TMP_DIR")
 RELEASE = int(os.getenv("RELEASE"))
 MAJOR_VERSION = int(os.getenv("MAJOR_VERSION"))
 MINOR_VERSION = int(os.getenv("MINOR_VERSION"))
 ON_PREMISES = True if os.getenv("ON_PREMISES") == "1" else False
```

### Comparing `cgcsdk-1.0.7/cgc/utils/consts/message_consts.py` & `cgcsdk-1.0.9/cgc/utils/consts/message_consts.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/utils/cryptography/aes_crypto.py` & `cgcsdk-1.0.9/cgc/utils/cryptography/aes_crypto.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/utils/cryptography/encryption_module.py` & `cgcsdk-1.0.9/cgc/utils/cryptography/encryption_module.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/utils/cryptography/rsa_crypto.py` & `cgcsdk-1.0.9/cgc/utils/cryptography/rsa_crypto.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/utils/custom_exceptions.py` & `cgcsdk-1.0.9/cgc/utils/custom_exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 ########### custom exceptions dict #############
 # warnings are divided by code, then by reason
 # every warning has its message that will be returned to print
 CUSTOM_EXCEPTIONS = {
     500: {
         "UNDEFINED": "undefined exception",
+        "USER_KEY_CREATE_ERROR": "Error while creating key",
     },
     413: {
         "PVC_CREATE_STORAGE_LIMIT_EXCEEDED": "This request exceeds your storage limits",
         "PVC_CREATE_NOT_ENOUGH_STORAGE_IN_CLUSTER": "No more storage available",
         "REQUEST_RESOURCE_LIMIT_EXCEEDED": "This request exceeds your resources limit",
         "RESOURCES_NOT_AVAILABLE_IN_CLUSTER": "Requested resources not available",
     },
     409: {
         "PVC_NAME_ALREADY_EXISTS": "Volume with this name already exists.",
         "PVC_DELETE_EXCEPTION": "Can't delete mounted volume, try with force",
         "RESOURCE_PORTS_ALREADY_EXISTS": "Port with this name already exists.",
         "RESOURCE_TEMPLATE_NAME_ALREADY_EXISTS": "Resource with this name already exists.",
         "JOB_CREATE_ALREADY_EXISTS": "Job with this name already exists.",
+        "USER_KEY_ALREADY_EXISTS": "Key with these data already exists.",
     },
     404: {
         "PVC_CREATE_NO_SC": "Selected disk type and access mode unavailable",
         "BILLING_STATUS_NO_DATA": "No data to print.",
         "NOT_DELETED_ANYTHING_IN_COMPUTE_DELETE": "No app with this name to delete.",
         "API_KEY_DELETE_ERROR": "No api key with this id to delete",
         "PVC_MOUNT_NOT_FOUND_TEMPLATE": "No app with this name to mount.",
@@ -29,14 +31,15 @@
         "PVC_DELETE_NOT_FOUND": "App with this name not found.",
         "COMPUTE_RESTART_TEMPLATE_NOT_FOUND": "App with this name not found.",
         "COMPUTE_CREATE_TEMPLATE_NOT_FOUND": "There is no template with this name.",
         "COMPUTE_TEMPLATE_NAME_NOT_FOUND": "No app with this name.",
         "COMPUTE_RESOURCE_QUOTA_NOT_FOUND": "You do not have enforced limits on your namespace.",
         "JOB_NOT_FOUND": "Job with this name not found.",
         "RESOURCE_NOT_FOUND": "Resource with this name not found.",
+        "USER_KEY_NOT_FOUND": "Key with this id not found.",
     },
     400: {
         "WRONG_DATE_FORMAT": "Wrong date format.",
         "ENTITY_NOT_ALLOWED": "You can't create this entity.",
         "PVC_MOUNT_ALREADY_MOUNTED": "This volume is already mounted.",
         "TEMPLATE_NAME_SYSTEM_RESERVED": "You can't create app with this name.",
         "JOB_LACKS_REQUIRED_PARAMETER": "Job requires container image parameter.",
```

### Comparing `cgcsdk-1.0.7/cgc/utils/message_utils.py` & `cgcsdk-1.0.9/cgc/utils/message_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,11 +54,11 @@
             exit(1)
         except (TypeError, KeyError, IndexError) as err:
             print(args, "\n", kwargs)
             increment_metric("client.parser", True)
             if "debug" in kwargs:
                 raise err
             return prepare_error_message(UNKNOWN_ERROR)
-        except ResponseException as err:
+        except (ResponseException, click.ClickException) as err:
             return prepare_warning_message(err)
 
     return wrapper
```

### Comparing `cgcsdk-1.0.7/cgc/utils/prepare_headers.py` & `cgcsdk-1.0.9/cgc/utils/prepare_headers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,66 @@
 from cgc.utils.config_utils import read_from_cfg
-from cgc.utils.consts.env_consts import API_URL, CGC_SECRET
 from cgc.commands.auth import auth_utils
 from cgc.utils.message_utils import key_error_decorator_for_helpers
 
 
 def load_user_api_keys():
     """Based on configuration getter creates pair of API keys
 
     :return: api_key and api_secret
     :rtype: list of strings
     """
     return read_from_cfg("api_key"), read_from_cfg("api_secret")
 
 
+def load_user_cgc_secret():
+    return read_from_cfg("cgc_secret")
+
+
+def load_user_api_url():
+    return read_from_cfg("cgc_api_url")
+
+
 @key_error_decorator_for_helpers
 def get_api_url_and_prepare_headers():
-    """Loads API_URL and user api keys into single function. Mend to be used as single point of truth for all endpoints except register - due to different Content-Type header
+    """Loads CGC_API_URL and user api keys into single function. Mend to be used as single point of truth for all endpoints except register - due to different Content-Type header
 
-    :return: API_URL and headers
+    :return: CGC_API_URL and headers
     :rtype: string and dict
     """
     api_key, api_secret = load_user_api_keys()
     headers = {
-        "Content-Type": "application/json; charset=UTF-8",
         "accept": "application/json",
+        "Content-Type": "application/json; charset=UTF-8",
+        "comtegra-cgc": load_user_cgc_secret(),
         "api-key": api_key,
         "api-secret": api_secret,
-        "comtegra-cgc": CGC_SECRET,
     }
-    return API_URL, headers
+    return load_user_api_url(), headers
 
 
-def get_url_and_prepare_headers_register(user_id: str, access_key: str):
+def get_url_and_prepare_headers_register(
+    user_id: str, access_key: str, url: str = None, secret: str = None
+):
     """Creates and returns url and headers for register request.
 
     :return: url, headers
     :rtype: string and dict
     """
-    url = f"{API_URL}/v1/api/user/register?user_id={user_id}&access_key={access_key}"
+    url = f"{load_user_api_url() if url is None else url}/v1/api/user/register?user_id={user_id}&access_key={access_key}"
     headers = {
         "accept": "application/json",
-        "comtegra-cgc": CGC_SECRET,
         "Content-Type": "octet-stream",
+        "comtegra-cgc": load_user_cgc_secret() if secret is None else secret,
     }
     return url, headers
 
 
 def get_url_and_headers_jwt_token():
-    url = f"{API_URL}/v1/api/user/create/token"
+    url = f"{load_user_api_url()}/v1/api/user/create/token"
     headers = {
         "accept": "application/json",
         "Content-Type": "application/x-www-form-urlencoded",
     }
     return url, headers
 
 
@@ -60,26 +69,26 @@
     """Prepares headers for create API key request.
 
     :return: headers in a for of dictionary
     :rtype: dict
     """
     headers = {
         "accept": "application/json",
-        "comtegra-cgc": CGC_SECRET,
         "Authorization": f"Bearer {auth_utils.get_jwt(user_id, password)}",
+        "comtegra-cgc": load_user_cgc_secret(),
     }
     return headers
 
 
 def get_api_url_and_prepare_headers_version_control():
     """Prepares headers for version control request.
 
     :return: url and headers in a for of dictionary
     :rtype: string, dict
     """
-    url = f"{API_URL}/v1/api/info/version"
+    url = f"{load_user_api_url()}/v1/api/info/version"
     headers = {
         "accept": "application/json",
-        "comtegra-cgc": CGC_SECRET,
         "Content-Type": "application/json",
+        "comtegra-cgc": load_user_cgc_secret(),
     }
     return url, headers
```

### Comparing `cgcsdk-1.0.7/cgc/utils/requests_helper.py` & `cgcsdk-1.0.9/cgc/utils/requests_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import requests
 import urllib3
 import urllib3.exceptions
-import ssl
 import click
 import sys
 
 from enum import Enum
 
 from cgc.utils.consts.env_consts import API_SECURE_CONNECTION
 from cgc.telemetry.basic import increment_metric
@@ -15,23 +14,22 @@
     UNKNOWN_ERROR,
     CONNECTION_ERROR,
     CERTIFICATE_ERROR,
 )
 
 urllib3.disable_warnings(urllib3.exceptions.SecurityWarning)
 
-
 class EndpointTypes(Enum):
     get = requests.get
     post = requests.post
     delete = requests.delete
 
 
 def _process_endpoint_kwargs(**kwargs):
-    if not "timeout" in kwargs.keys():
+    if "timeout" not in kwargs.keys():
         kwargs["timeout"] = 30
     return kwargs
 
 
 def _call_rest_endpoint(request: EndpointTypes, **kwargs):
     kwargs = _process_endpoint_kwargs(**kwargs)
     return request(**kwargs)
```

### Comparing `cgcsdk-1.0.7/cgc/utils/response_utils.py` & `cgcsdk-1.0.9/cgc/utils/response_utils.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgc/utils/version_control.py` & `cgcsdk-1.0.9/cgc/utils/version_control.py`

 * *Files identical despite different names*

### Comparing `cgcsdk-1.0.7/cgcsdk.egg-info/PKG-INFO` & `cgcsdk-1.0.9/cgcsdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgcsdk
-Version: 1.0.7
+Version: 1.0.9
 Summary: Comtegra GPU Cloud REST API client
 Author: Comtegra AI Team
 Author-email: ai@comtegra.pl
 License: BSD 2-clause
 Project-URL: Documentation, https://example.com/documentation/
 Project-URL: GitHub, https://github.com/foobar/foobar/
 Project-URL: Changelog, https://github.com/foobar/foobar/blob/master/CHANGELOG.md
@@ -26,16 +26,14 @@
 Requires-Dist: tabulate
 Requires-Dist: pycryptodomex
 Requires-Dist: paramiko>=2.11
 Requires-Dist: statsd
 Requires-Dist: requests
 Requires-Dist: setuptools
 Requires-Dist: colorama
-Requires-Dist: redis
-Requires-Dist: pymongo
 Requires-Dist: psycopg2-binary
 
 # Comtegra GPU Cloud CLI Client
 
 ## Basic info
 
 CGC Clinet is complete solution to create and manage your compute resources through CLI interface and python code. It incorporates CLI and SDK in one package.
@@ -50,18 +48,16 @@
 2. [Triton inferencing server](https://docs.nvidia.com/deeplearning/triton-inference-server/) for large scale inferencing
 3. [Label studio](https://labelstud.io/) for easy management of your data annotation tasks with variety of modes
 4. [Rapids](https://rapids.ai/) suite of accelerated libraries for data processing
 
 Notebooks are equiped with all CUDA libraries and GPU drivers which enables the usage of GPU for accelerated computations.
 Apart from compute resources, we provide the database engines accessible from within your namespace:
 
-1. [MongoDB](https://www.mongodb.org/)
-2. [PostgreSQL](https://www.postgresql.org/)
-3. [Redis](https://redis.io/)
-4. [Weaviate](https://weaviate.io/)
+1. [PostgreSQL](https://www.postgresql.org/)
+2. [Weaviate](https://weaviate.io/)
 
 More are coming!
 Please follow instructions to get started.
 
 ## More info
 
 If you'd like to know more visit:
```

### Comparing `cgcsdk-1.0.7/cgcsdk.egg-info/SOURCES.txt` & `cgcsdk-1.0.9/cgcsdk.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 cgc/cgc.py
 cgc/config.py
 cgc/server.crt
 cgc/commands/__init__.py
 cgc/commands/cgc_cmd.py
 cgc/commands/cgc_cmd_responses.py
 cgc/commands/cgc_helpers.py
+cgc/commands/cgc_models.py
 cgc/commands/exceptions.py
 cgc/commands/auth/__init__.py
 cgc/commands/auth/auth_cmd.py
 cgc/commands/auth/auth_responses.py
 cgc/commands/auth/auth_utils.py
 cgc/commands/billing/__init__.py
 cgc/commands/billing/billing_cmd.py
@@ -25,35 +26,38 @@
 cgc/commands/compute/__init__.py
 cgc/commands/compute/compute_cmd.py
 cgc/commands/compute/compute_models.py
 cgc/commands/compute/compute_responses.py
 cgc/commands/compute/compute_utills.py
 cgc/commands/db/__init__.py
 cgc/commands/db/db_cmd.py
+cgc/commands/db/db_models.py
 cgc/commands/debug/__init__.py
 cgc/commands/debug/debug_cmd.py
 cgc/commands/jobs/__init__.py
 cgc/commands/jobs/job_utils.py
 cgc/commands/jobs/jobs_cmd.py
 cgc/commands/jobs/jobs_responses.py
+cgc/commands/keys/__init__.py
+cgc/commands/keys/keys_cmd.py
+cgc/commands/keys/keys_models.py
+cgc/commands/keys/keys_responses.py
+cgc/commands/keys/keys_utils.py
 cgc/commands/resource/__init__.py
 cgc/commands/resource/resource_cmd.py
 cgc/commands/resource/resource_responses.py
 cgc/commands/volume/__init__.py
 cgc/commands/volume/data_model.py
 cgc/commands/volume/volume_cmd.py
 cgc/commands/volume/volume_responses.py
 cgc/commands/volume/volume_utils.py
 cgc/sdk/__init__.py
 cgc/sdk/exceptions.py
-cgc/sdk/handlers.py
 cgc/sdk/job.py
-cgc/sdk/mongodb.py
 cgc/sdk/postgresql.py
-cgc/sdk/redis.py
 cgc/sdk/resource.py
 cgc/telemetry/__init__.py
 cgc/telemetry/basic.py
 cgc/tests/__init__.py
 cgc/tests/responses_tests.py
 cgc/tests/desired_responses/test_billing_invoice.txt
 cgc/tests/desired_responses/test_billing_status.txt
```

### Comparing `cgcsdk-1.0.7/setup.py` & `cgcsdk-1.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,16 +37,14 @@
         "tabulate",
         "pycryptodomex",
         "paramiko>=2.11",
         "statsd",
         "requests",
         "setuptools",
         "colorama",
-        "redis",
-        "pymongo",
         "psycopg2-binary",
     ],
     entry_points={
         "console_scripts": [
             "cgc = cgc.cgc:cli",
         ],
     },
```

