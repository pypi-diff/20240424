# Comparing `tmp/spotinst-sdk2-3.0.0.tar.gz` & `tmp/spotinst-sdk2-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotinst-sdk2-3.0.0.tar", last modified: Fri Apr 19 16:12:11 2024, max compression
+gzip compressed data, was "spotinst-sdk2-3.1.0.tar", last modified: Wed Apr 24 11:53:01 2024, max compression
```

## Comparing `spotinst-sdk2-3.0.0.tar` & `spotinst-sdk2-3.1.0.tar`

### file list

```diff
@@ -1,99 +1,101 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.338174 spotinst-sdk2-3.0.0/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    11356 2023-02-24 13:45:28.000000 spotinst-sdk2-3.0.0/LICENSE
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       43 2023-02-24 13:45:28.000000 spotinst-sdk2-3.0.0/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      751 2023-02-24 13:45:28.000000 spotinst-sdk2-3.0.0/NOTICE.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8093 2024-04-19 16:12:11.338174 spotinst-sdk2-3.0.0/PKG-INFO
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     7177 2023-02-24 13:45:28.000000 spotinst-sdk2-3.0.0/README.md
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       63 2024-04-19 16:12:11.338174 spotinst-sdk2-3.0.0/setup.cfg
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     3485 2024-04-19 16:12:01.000000 spotinst-sdk2-3.0.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     4931 2024-04-19 16:12:01.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15928 2023-11-20 13:07:49.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/client.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/clients/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/clients/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/clients/admin/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12645 2024-02-01 18:22:35.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/clients/admin/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/clients/elastigroup/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    78320 2024-04-19 16:12:01.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/clients/elastigroup/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/clients/functions/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3184 2023-11-08 04:20:46.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/clients/functions/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/clients/hpc/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3376 2023-11-08 04:20:46.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/clients/hpc/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/clients/managed_instance/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11698 2023-11-08 04:20:46.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/clients/managed_instance/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/clients/mcs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      916 2023-11-08 04:20:46.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/clients/mcs/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/clients/mrscaler/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6286 2024-02-25 21:58:42.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/clients/mrscaler/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/clients/ocean/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    58159 2024-04-19 15:58:50.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/clients/ocean/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/clients/ocean_cd/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30586 2023-11-08 04:20:46.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/clients/ocean_cd/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/clients/setup/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5562 2023-11-08 04:20:46.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/clients/setup/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/clients/stateful_node/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16650 2023-11-25 09:32:13.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/clients/stateful_node/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/clients/subscription/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3859 2024-01-27 17:33:52.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/clients/subscription/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/models/admin/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/admin/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      548 2023-02-24 13:45:28.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/admin/user_mapping.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/models/elastigroup/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/elastigroup/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/models/elastigroup/aws/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    40959 2024-04-19 15:27:36.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/elastigroup/aws/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      651 2023-11-08 04:20:46.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/elastigroup/aws/asg.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1278 2023-11-08 04:20:46.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/elastigroup/aws/deployment.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      931 2023-11-08 04:20:46.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/elastigroup/aws/deployment_action.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1478 2023-11-08 04:20:46.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/elastigroup/aws/stateful.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/models/elastigroup/azure_v3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21715 2023-11-08 04:20:46.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/elastigroup/azure_v3/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/models/elastigroup/gcp/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17709 2023-08-16 14:46:57.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/elastigroup/gcp/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/models/functions/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3685 2023-11-08 04:25:02.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/functions/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/models/hpc/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 14:21:47.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/hpc/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/models/hpc/aws/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4954 2023-11-08 04:25:02.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/hpc/aws/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/models/managed_instance/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/managed_instance/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/models/managed_instance/aws/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15583 2024-04-19 15:27:36.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/managed_instance/aws/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/models/mrscaler/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/mrscaler/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/models/mrscaler/aws/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18653 2024-02-25 21:58:42.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/mrscaler/aws/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/models/ocean/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/ocean/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/models/ocean/aws/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    36517 2024-02-25 21:58:42.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/ocean/aws/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2/models/ocean/azure/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19808 2024-04-19 15:58:50.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/ocean/azure/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.334174 spotinst-sdk2-3.0.0/spotinst_sdk2/models/ocean_cd/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      806 2023-04-11 10:16:17.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/ocean_cd/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2988 2023-11-08 04:23:08.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/ocean_cd/rollout.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8887 2023-04-11 10:16:17.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/ocean_cd/rollout_spec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4154 2023-04-11 10:16:17.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/ocean_cd/strategy.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2652 2023-11-08 04:23:37.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/ocean_cd/verification_provider.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9061 2023-11-08 04:23:47.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/ocean_cd/verification_template.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.334174 spotinst-sdk2-3.0.0/spotinst_sdk2/models/setup/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/setup/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.334174 spotinst-sdk2-3.0.0/spotinst_sdk2/models/setup/azure/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1082 2023-02-24 13:45:28.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/setup/azure/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.334174 spotinst-sdk2-3.0.0/spotinst_sdk2/models/setup/gcp/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1656 2023-02-24 13:45:28.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/setup/gcp/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.338174 spotinst-sdk2-3.0.0/spotinst_sdk2/models/stateful_node/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27588 2024-02-25 21:58:42.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/stateful_node/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.338174 spotinst-sdk2-3.0.0/spotinst_sdk2/models/subscription/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      856 2023-11-08 04:24:10.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/models/subscription/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2615 2023-11-08 04:24:57.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/session.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2024-04-19 16:12:01.000000 spotinst-sdk2-3.0.0/spotinst_sdk2/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-19 16:12:11.314176 spotinst-sdk2-3.0.0/spotinst_sdk2.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8093 2024-04-19 16:12:11.000000 spotinst-sdk2-3.0.0/spotinst_sdk2.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2349 2024-04-19 16:12:11.000000 spotinst-sdk2-3.0.0/spotinst_sdk2.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-19 16:12:11.000000 spotinst-sdk2-3.0.0/spotinst_sdk2.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       16 2024-04-19 16:12:11.000000 spotinst-sdk2-3.0.0/spotinst_sdk2.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2024-04-19 16:12:11.000000 spotinst-sdk2-3.0.0/spotinst_sdk2.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.845422 spotinst-sdk2-3.1.0/
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    11356 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/LICENSE
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       43 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      751 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/NOTICE.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8093 2024-04-24 11:53:01.845422 spotinst-sdk2-3.1.0/PKG-INFO
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     7177 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/README.md
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       63 2024-04-24 11:53:01.845422 spotinst-sdk2-3.1.0/setup.cfg
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     3535 2024-04-24 11:51:28.000000 spotinst-sdk2-3.1.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.825429 spotinst-sdk2-3.1.0/spotinst_sdk2/
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     5098 2024-04-24 11:51:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15928 2023-11-20 13:07:49.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/client.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.837425 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.837425 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/admin/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12645 2024-02-01 18:22:35.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/admin/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.837425 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/elastigroup/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    78320 2024-04-19 16:12:01.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/elastigroup/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/functions/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3184 2023-11-08 04:20:46.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/functions/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/hpc/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3376 2023-11-08 04:20:46.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/hpc/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/managed_instance/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11698 2023-11-08 04:20:46.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/managed_instance/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/mcs/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      916 2023-11-08 04:20:46.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/mcs/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/mrscaler/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6286 2024-02-25 21:58:42.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/mrscaler/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/ocean/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    80602 2024-04-24 11:51:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/ocean/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/ocean_cd/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30586 2023-11-08 04:20:46.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/ocean_cd/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/setup/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5562 2023-11-08 04:20:46.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/setup/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/stateful_node/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16650 2023-11-25 09:32:13.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/stateful_node/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/subscription/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3859 2024-01-27 17:33:52.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/clients/subscription/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/admin/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/admin/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      548 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/admin/user_mapping.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/aws/
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    40959 2024-04-19 15:27:36.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/aws/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      651 2023-11-08 04:20:46.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/aws/asg.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1278 2023-11-08 04:20:46.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/aws/deployment.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      931 2023-11-08 04:20:46.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/aws/deployment_action.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1478 2023-11-08 04:20:46.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/aws/stateful.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/azure_v3/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21715 2023-11-08 04:20:46.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/azure_v3/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/gcp/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17709 2023-08-16 14:46:57.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/gcp/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/functions/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3685 2023-11-08 04:25:02.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/functions/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/hpc/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-17 14:21:47.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/hpc/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/hpc/aws/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4954 2023-11-08 04:25:02.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/hpc/aws/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/managed_instance/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/managed_instance/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/managed_instance/aws/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15583 2024-04-19 15:27:36.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/managed_instance/aws/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/mrscaler/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/mrscaler/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/mrscaler/aws/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18653 2024-02-25 21:58:42.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/mrscaler/aws/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.841423 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean/aws/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    36517 2024-02-25 21:58:42.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean/aws/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.845422 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean/azure/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19808 2024-04-19 15:58:50.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean/azure/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.845422 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean/gcp/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    24001 2024-04-24 11:51:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean/gcp/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.845422 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean_cd/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      806 2023-04-11 10:16:17.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean_cd/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2988 2023-11-08 04:23:08.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean_cd/rollout.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8887 2023-04-11 10:16:17.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean_cd/rollout_spec.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4154 2023-04-11 10:16:17.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean_cd/strategy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2652 2023-11-08 04:23:37.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean_cd/verification_provider.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9061 2023-11-08 04:23:47.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean_cd/verification_template.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.845422 spotinst-sdk2-3.1.0/spotinst_sdk2/models/setup/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/setup/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.845422 spotinst-sdk2-3.1.0/spotinst_sdk2/models/setup/azure/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1082 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/setup/azure/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.845422 spotinst-sdk2-3.1.0/spotinst_sdk2/models/setup/gcp/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1656 2023-02-24 13:45:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/setup/gcp/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.845422 spotinst-sdk2-3.1.0/spotinst_sdk2/models/stateful_node/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27588 2024-02-25 21:58:42.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/stateful_node/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.845422 spotinst-sdk2-3.1.0/spotinst_sdk2/models/subscription/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      856 2023-11-08 04:24:10.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/models/subscription/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2615 2023-11-08 04:24:57.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/session.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       22 2024-04-24 11:51:28.000000 spotinst-sdk2-3.1.0/spotinst_sdk2/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-24 11:53:01.837425 spotinst-sdk2-3.1.0/spotinst_sdk2.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8093 2024-04-24 11:53:01.000000 spotinst-sdk2-3.1.0/spotinst_sdk2.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2392 2024-04-24 11:53:01.000000 spotinst-sdk2-3.1.0/spotinst_sdk2.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-24 11:53:01.000000 spotinst-sdk2-3.1.0/spotinst_sdk2.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       16 2024-04-24 11:53:01.000000 spotinst-sdk2-3.1.0/spotinst_sdk2.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2024-04-24 11:53:01.000000 spotinst-sdk2-3.1.0/spotinst_sdk2.egg-info/top_level.txt
```

### Comparing `spotinst-sdk2-3.0.0/LICENSE` & `spotinst-sdk2-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/NOTICE.md` & `spotinst-sdk2-3.1.0/NOTICE.md`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/PKG-INFO` & `spotinst-sdk2-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-sdk2
-Version: 3.0.0
+Version: 3.1.0
 Summary: A Python SDK for Spotinst
 Home-page: https://github.com/spotinst/spotinst-sdk-python
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst spot instances aws azure ec2 cloud infrastructure development elastigroup
 Platform: UNKNOWN
```

### Comparing `spotinst-sdk2-3.0.0/README.md` & `spotinst-sdk2-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/setup.py` & `spotinst-sdk2-3.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
             "spotinst_sdk2.models.hpc",
                 "spotinst_sdk2.models.hpc.aws",
             "spotinst_sdk2.models.mrscaler",
                 "spotinst_sdk2.models.mrscaler.aws",
             "spotinst_sdk2.models.ocean",
                 "spotinst_sdk2.models.ocean.aws",
                 "spotinst_sdk2.models.ocean.azure",
+                "spotinst_sdk2.models.ocean.gcp",
             "spotinst_sdk2.models.ocean_cd",
                 "spotinst_sdk2.models.ocean_cd",
             "spotinst_sdk2.models.setup",
                 "spotinst_sdk2.models.setup.azure",
                 "spotinst_sdk2.models.setup.gcp",
             "spotinst_sdk2.models.subscription",
             "spotinst_sdk2.models.managed_instance",
```

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/__init__.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,17 @@
             "mcs": McsClient(session=self.session, print_output=print_output, log_level=log_level,
                              user_agent=user_agent, timeout=timeout),
             "mrScaler_aws": MrScalerAwsClient(session=self.session, print_output=print_output, log_level=log_level,
                                               user_agent=user_agent, timeout=timeout),
             "ocean_aws": OceanAwsClient(session=self.session, print_output=print_output, log_level=log_level,
                                         user_agent=user_agent, timeout=timeout),
             "ocean_azure": OceanAzureClient(session=self.session, print_output=print_output, log_level=log_level,
-                                        user_agent=user_agent, timeout=timeout),                            
+                                        user_agent=user_agent, timeout=timeout),
+            "ocean_gcp": OceanGcpClient(session=self.session, print_output=print_output, log_level=log_level,
+                                            user_agent=user_agent, timeout=timeout),
             "oceancd": OceanCDClient(session=self.session, print_output=print_output, log_level=log_level,
                                       user_agent=user_agent, timeout=timeout),
             "managed_instance_aws": ManagedInstanceAwsClient(session=self.session, print_output=print_output,
                                                              log_level=log_level, user_agent=user_agent,
                                                              timeout=timeout),
             "subscription": SubscriptionClient(session=self.session, print_output=print_output, log_level=log_level,
                                                user_agent=user_agent, timeout=timeout),
```

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/client.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/client.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/clients/admin/__init__.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/clients/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/clients/elastigroup/__init__.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/clients/elastigroup/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/clients/functions/__init__.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/clients/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/clients/hpc/__init__.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/clients/hpc/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/clients/managed_instance/__init__.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/clients/managed_instance/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/clients/mcs/__init__.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/clients/mcs/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/clients/mrscaler/__init__.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/clients/mrscaler/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/clients/ocean/__init__.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/clients/ocean/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 from typing import List
 
 from spotinst_sdk2.client import Client
 import spotinst_sdk2.models.ocean.aws as aws_ocean
 import spotinst_sdk2.models.ocean.azure as azure_ocean
+import spotinst_sdk2.models.ocean.gcp as gcp_ocean
 
 # region AWS
 
 
 class OceanAwsClient(Client):
     __base_ocean_cluster_url = "/ocean/aws/k8s/cluster"
     __base_ocean_launchspec_url = "/ocean/aws/k8s/launchSpec"
@@ -1689,7 +1690,666 @@
         )
 
         formatted_response = self.convert_json(
             response, self.camel_to_underscore)
 
         return formatted_response["response"]
     # endregion
+
+
+class OceanGcpClient(Client):
+    __base_ocean_url = "/ocean/k8s/cluster/"
+    __base_ocean_cluster_url = "/ocean/gcp/k8s/cluster"
+    __base_ocean_launchspec_url = "/ocean/gcp/k8s/launchSpec"
+
+    def get_heartbeat_status(self, ocean_id: str):
+        """
+        Get the heartbeat status of the Ocean Controller for the cluster.
+        The response returns the heartbeat status and the last heartbeat timestamp.
+
+        # Arguments
+        ocean_id (String): ID of the Ocean Cluster
+
+        # Returns
+        (Object): Ocean Get Heartbeat response
+        """
+        response = self.send_get(
+            url=self.__base_ocean_url + ocean_id + "/controllerHeartbeat",
+            entity_name="ocean (Cluster Heartbeat)"
+        )
+
+        formatted_response = self.convert_json(
+            response, self.camel_to_underscore)
+
+        return formatted_response["response"]["items"][0]
+
+    def create_ocean_cluster(self, ocean: gcp_ocean.Ocean):
+        """
+        Create an Ocean Cluster
+
+        # Arguments
+        ocean (Ocean): Ocean Object
+
+        # Returns
+        (Object): Ocean API response
+        """
+        ocean = gcp_ocean.OceanRequest(ocean)
+
+        excluded_missing_dict = self.exclude_missing(
+            json.loads(ocean.toJSON()))
+
+        formatted_missing_dict = self.convert_json(
+            excluded_missing_dict, self.underscore_to_camel)
+
+        body_json = json.dumps(formatted_missing_dict)
+
+        response = self.send_post(
+            body=body_json,
+            url=self.__base_ocean_cluster_url,
+            entity_name='ocean')
+
+        formatted_response = self.convert_json(response,
+                                               self.camel_to_underscore)
+
+        return formatted_response["response"]["items"][0]
+
+    def get_all_ocean_clusters(self):
+        """
+        List the configurations for all Ocean clusters in the specified account.
+
+        # Returns
+        (Object): Ocean API response
+        """
+
+        response = self.send_get(
+            url=self.__base_ocean_cluster_url,
+            entity_name="ocean"
+        )
+
+        formatted_response = self.convert_json(
+            response, self.camel_to_underscore)
+
+        return formatted_response["response"]["items"]
+
+    def delete_ocean_cluster(self, ocean_id: str):
+        """
+        Delete a specified Ocean cluster.
+
+        # Arguments
+        ocean_id (String): ID of the Ocean Cluster
+
+        # Returns
+        (Object): Ocean API response
+        """
+        return self.send_delete(
+            url=self.__base_ocean_cluster_url + "/" + ocean_id,
+            entity_name="ocean"
+        )
+
+    def get_ocean_cluster(self, ocean_id: str):
+        """
+        Get the configuration for a specified Ocean cluster.
+
+        # Arguments
+        ocean_id (String): ID of the Ocean Cluster
+
+        # Returns
+        (Object): Ocean API response
+        """
+        response = self.send_get(
+            url=self.__base_ocean_cluster_url + "/" + ocean_id,
+            entity_name="ocean"
+        )
+
+        formatted_response = self.convert_json(
+            response, self.camel_to_underscore)
+
+        return formatted_response["response"]["items"][0]
+
+    def update_ocean_cluster(self, ocean_id: str, ocean: gcp_ocean.Ocean):
+        """
+        Update an existing Ocean Cluster
+
+        # Arguments
+        ocean_id (String): ID of the Ocean Cluster
+        ocean (Ocean): Ocean object
+
+        # Returns
+        (Object): Ocean API response
+        """
+        ocean = gcp_ocean.OceanRequest(ocean)
+
+        excluded_missing_dict = self.exclude_missing(
+            json.loads(ocean.toJSON()))
+
+        formatted_missing_dict = self.convert_json(
+            excluded_missing_dict, self.underscore_to_camel)
+
+        body_json = json.dumps(formatted_missing_dict)
+
+        response = self.send_put(
+            body=body_json,
+            url=self.__base_ocean_cluster_url + "/" + ocean_id,
+            entity_name='ocean')
+
+        formatted_response = self.convert_json(
+            response,
+            self.camel_to_underscore)
+
+        return formatted_response["response"]["items"][0]
+
+    def reimport_ocean_cluster(self, ocean_id: str):
+        """
+        Reimport the cluster's configuration from GKE.
+
+        # Arguments
+        ocean_id (String): ID of the Ocean Cluster
+        ocean (Ocean): Ocean object
+
+        # Returns
+        (Object): Reimport cluster response
+        """
+
+        response = self.send_put(
+            url=self.__base_ocean_cluster_url + "/" + ocean_id + '/reImport',
+            entity_name='ocean')
+
+        formatted_response = self.convert_json(
+            response,
+            self.camel_to_underscore)
+
+        return formatted_response["response"]["items"][0]
+
+    def get_elastilog(self, ocean_id: str, from_date: str, to_date: str, severity: str = None, resource_id: str = None,
+                      limit: int = None):
+        """
+        Get group’s Elastilog by
+
+        # Arguments
+        to_date (String): end date value
+        from_date (String): beginning date value
+        severity(String) (Optional): Log level severity
+        resource_id(String) (Optional): specific resource identifier
+        limit(int) (Optional): Maximum number of lines to extract in a response
+
+        # Returns
+        (Object): Ocean Get Log API response
+        """
+        geturl = self.__base_ocean_cluster_url + "/" + ocean_id + "/log"
+        query_params = dict(toDate=to_date, fromDate=from_date, severity=severity,
+                            resourceId=resource_id, limit=limit)
+
+        result = self.send_get(
+            url=geturl, entity_name='ocean_gcp_log', query_params=query_params)
+
+        formatted_response = self.convert_json(
+            result, self.camel_to_underscore)
+
+        return formatted_response["response"]["items"]
+
+    def get_rightsizing_recommendations(self, ocean_id: str, filter: gcp_ocean.RightSizingRecommendationFilter = None):
+        """
+        Get right-sizing recommendations for an Ocean cluster and filter them according to namespace or label.
+
+        # Arguments
+        ocean_id (String): Id of the Ocean Cluster
+        filter (RightSizingRecommendationFilter): Optional - may be null.
+
+        # Returns
+        (Object): Ocean API response
+        """
+        recommendation_request = gcp_ocean.RightSizingRecommendationRequest(
+            filter)
+
+        excluded_missing_dict = self.exclude_missing(
+            json.loads(recommendation_request.toJSON()))
+
+        formatted_missing_dict = self.convert_json(
+            excluded_missing_dict, self.underscore_to_camel)
+
+        body_json = json.dumps(formatted_missing_dict)
+
+        group_response = self.send_post(
+            body=body_json,
+            url=self.__base_ocean_cluster_url +
+            "/" + ocean_id + "/rightSizing/suggestion",
+            entity_name='ocean')
+
+        formatted_response = self.convert_json(
+            group_response, self.camel_to_underscore)
+
+        return formatted_response["response"]["items"]
+
+    def get_aggregated_cluster_costs(self, ocean_id: str, aggregated_cluster_costs: gcp_ocean.AggregatedClusterCosts):
+        """
+        Get aggregated cluster costs
+
+        # Arguments
+        ocean_id (String): ID of the Ocean Cluster
+        aggregated_cluster_costs (AggregatedClusterCosts): Aggregated Cluster Costs request
+
+        # Returns
+        (Object): Aggregated Cluster Costs API response
+        """
+        aggregated_cluster_costs_request = gcp_ocean.AggregatedClusterCostRequest(
+            aggregated_cluster_costs)
+
+        excluded_missing_dict = self.exclude_missing(
+            json.loads(aggregated_cluster_costs_request.toJSON()))
+
+        formatted_missing_dict = self.convert_json_with_list_of_lists(
+            excluded_missing_dict, self.underscore_to_camel)
+
+        body_json = json.dumps(formatted_missing_dict)
+
+        aggregated_costs_response = self.send_post(
+            body=body_json,
+            url=self.__base_ocean_cluster_url + "/" + ocean_id + "/aggregatedCosts",
+            entity_name='ocean (aggregated cluster costs)')
+
+        formatted_response = self.convert_json(
+            aggregated_costs_response, self.camel_to_underscore)
+
+        return formatted_response["response"]["items"][0]
+
+    def get_aggregated_summary_costs(self, ocean_id: str, aggregated_cluster_costs: gcp_ocean.AggregatedClusterCosts):
+        """
+        Get aggregated cluster costs
+
+        # Arguments
+        ocean_id (String): ID of the Ocean Cluster
+        aggregated_cluster_costs (AggregatedClusterCosts): Aggregated Cluster Costs request
+
+        # Returns
+        (Object): Aggregated Cluster Costs API response
+        """
+        aggregated_cluster_costs_request = gcp_ocean.AggregatedClusterCostRequest(
+            aggregated_cluster_costs)
+
+        excluded_missing_dict = self.exclude_missing(
+            json.loads(aggregated_cluster_costs_request.toJSON()))
+
+        formatted_missing_dict = self.convert_json_with_list_of_lists(
+            excluded_missing_dict, self.underscore_to_camel)
+
+        body_json = json.dumps(formatted_missing_dict)
+
+        aggregated_summary_costs_response = self.send_post(
+            body=body_json,
+            url=self.__base_ocean_cluster_url + "/" +
+            ocean_id + "/aggregatedCosts/summary",
+            entity_name='ocean (aggregated summary costs)')
+
+        formatted_response = self.convert_json(
+            aggregated_summary_costs_response, self.camel_to_underscore)
+
+        return formatted_response["response"]["items"][0]
+
+    def create_virtual_node_group(self, vng: gcp_ocean.VirtualNodeGroup):
+        """
+        Create a virtual node group.
+
+        # Arguments
+        vng (VirtualNodeGroup): VirtualNodeGroup Object
+
+        # Returns
+        (Object): Ocean Launch Spec response
+        """
+        ocean = gcp_ocean.VNGRequest(vng)
+
+        excluded_missing_dict = self.exclude_missing(
+            json.loads(ocean.toJSON()))
+
+        formatted_missing_dict = self.convert_json(
+            excluded_missing_dict, self.underscore_to_camel)
+
+        body_json = json.dumps(formatted_missing_dict)
+
+        response = self.send_post(
+            body=body_json,
+            url=self.__base_ocean_launchspec_url,
+            entity_name='ocean_gcp_vng')
+
+        formatted_response = self.convert_json(response,
+                                               self.camel_to_underscore)
+
+        return formatted_response["response"]["items"][0]
+
+    def get_all_virtual_node_groups(self, ocean_id: str):
+        """
+        List the configurations for all virtual node groups in the account
+        or in a specified cluster.
+
+        # Returns
+        (Object): Ocean VNG API response
+        """
+
+        response = self.send_get(
+            url=self.__base_ocean_launchspec_url,
+            entity_name="ocean_gcp_vng",
+            query_params=dict(oceanId=ocean_id)
+        )
+
+        formatted_response = self.convert_json(
+            response, self.camel_to_underscore)
+
+        return formatted_response["response"]["items"]
+
+    def import_gke_nodepool_to_vng_configuration(self, node_pool_name: str, ocean_id: str):
+        """
+        Import GKE Nodepool configurations and generate valid Ocean Virtual Node Group (VNG) configuration
+        which can be used to create VNGs
+
+        # Returns
+        (Object): Ocean API response
+        """
+
+        response = self.send_post_with_params(
+            body=None,
+            url=self.__base_ocean_launchspec_url + "/import",
+            entity_name='ocean_gcp_vng',
+            user_query_params=dict(nodePoolName=node_pool_name, oceanId=ocean_id))
+
+        formatted_response = self.convert_json(response,
+                                               self.camel_to_underscore)
+
+        return formatted_response["response"]["items"][0]
+
+    def delete_virtual_node_group(self, vng_id: str, delete_nodes: bool = None):
+        """
+        Delete an Ocean Cluster
+
+        # Arguments
+        vng_id (String): ID of the Ocean VNG
+        delete_nodes (Bool): When set to "true", all instances belonging to the deleted launch specification will be drained, detached, and terminated.
+
+        # Returns
+        (Object): Ocean Launch Specification Delete response
+        """
+        return self.send_delete_with_params(
+            url=self.__base_ocean_launchspec_url + "/" + vng_id,
+            entity_name="ocean_gcp_vng",
+            user_query_params=dict(deleteNodes=delete_nodes)
+        )
+
+    def update_virtual_node_group(self, vng_id: str, vng: gcp_ocean.VirtualNodeGroup):
+        """
+        Update an existing VNG inside an Ocean Cluster
+
+        # Arguments
+        vng_id (String): ID of the Ocean Virtual Node Group
+        ocean (Ocean): Ocean object
+
+        # Returns
+        (Object): Ocean Launch Spec response
+        """
+        ocean = gcp_ocean.VNGRequest(vng)
+
+        excluded_missing_dict = self.exclude_missing(
+            json.loads(ocean.toJSON()))
+
+        formatted_missing_dict = self.convert_json(
+            excluded_missing_dict, self.underscore_to_camel)
+
+        body_json = json.dumps(formatted_missing_dict)
+
+        response = self.send_put(
+            body=body_json,
+            url=self.__base_ocean_launchspec_url + "/" + vng_id,
+            entity_name='ocean_gcp_vng')
+
+        formatted_response = self.convert_json(
+            response,
+            self.camel_to_underscore)
+
+        return formatted_response["response"]["items"][0]
+
+    def get_virtual_node_group(self, ocean_launch_spec_id: str):
+        """
+        Get Virtual Node Group of the cluster
+
+        # Arguments
+        ocean_launch_spec_id (String): Ocean cluster launch specification identifier
+
+        # Returns
+        (Object): Ocean Allowed Instance Types response
+        """
+        response = self.send_get(
+            url=self.__base_ocean_launchspec_url + "/" + ocean_launch_spec_id,
+            entity_name="ocean_gcp_vng"
+        )
+
+        formatted_response = self.convert_json(
+            response, self.camel_to_underscore)
+
+        return formatted_response["response"]["items"]
+
+    def initiate_roll(self, ocean_id: str, cluster_roll: gcp_ocean.Roll):
+        """
+        Initiate Cluster Rolls
+
+        # Arguments
+        ocean_id (String): ID of the Ocean Cluster
+        cluster_roll (Roll): Cluster Roll / Roll with Instance Ids/ Launch specification Ids
+
+        # Returns
+        (Object): Cluster Roll API response
+        """
+        roll_request = gcp_ocean.ClusterRollInitiateRequest(cluster_roll)
+
+        excluded_missing_dict = self.exclude_missing(
+            json.loads(roll_request.toJSON()))
+
+        formatted_missing_dict = self.convert_json_with_list_of_lists(
+            excluded_missing_dict, self.underscore_to_camel)
+
+        body_json = json.dumps(formatted_missing_dict)
+
+        rolls_response = self.send_post(
+            body=body_json,
+            url=self.__base_ocean_cluster_url + "/" + ocean_id + "/roll",
+            entity_name='ocean (Cluster Roll)')
+
+        formatted_response = self.convert_json(
+            rolls_response, self.camel_to_underscore)
+
+        return formatted_response["response"]["items"][0]
+
+    def list_rolls(self, ocean_id: str):
+        """
+        Get status for all rolls of an Ocean cluster.
+
+        # Arguments
+        ocean_id (String): ID of the Ocean Cluster
+
+        # Returns
+        (Object): List of Cluster Roll API response
+        """
+        response = self.send_get(
+            url=self.__base_ocean_cluster_url + "/" + ocean_id + "/roll",
+            entity_name="ocean (Cluster Roll)"
+        )
+
+        formatted_response = self.convert_json(
+            response, self.camel_to_underscore)
+
+        return formatted_response["response"]["items"]
+
+    def update_roll(self, ocean_id: str, roll_id: str, status: str):
+        """
+        Update a roll of an Ocean cluster.
+        Performing the request will stop the next batch in a roll.
+
+        # Arguments
+        ocean_id (String): ID of the Ocean Cluster
+        roll_id (String): Ocean cluster roll identifier
+        update_roll (UpdateRoll): update roll request
+
+        # Returns
+        (Object): Cluster Roll API response
+        """
+        update_roll_request = gcp_ocean.ClusterRollUpdateRequest(status)
+
+        excluded_missing_dict = self.exclude_missing(
+            json.loads(update_roll_request.toJSON()))
+
+        formatted_missing_dict = self.convert_json(
+            excluded_missing_dict, self.underscore_to_camel)
+
+        body_json = json.dumps(formatted_missing_dict)
+
+        response = self.send_put(
+            body=body_json,
+            url=self.__base_ocean_cluster_url + "/" + ocean_id + "/roll/" + roll_id,
+            entity_name='ocean (Cluster Roll)')
+
+        formatted_response = self.convert_json(
+            response, self.camel_to_underscore)
+
+        return formatted_response["response"]["items"][0]
+
+    def get_roll(self, ocean_id: str, roll_id: str):
+        """
+        Get status for a roll of an Ocean cluster.
+
+        # Arguments
+        ocean_id (String): ID of the Ocean Cluster
+        account_id (String): The ID of the account associated with your token.
+        roll_id (String): Ocean cluster roll identifier
+
+        # Returns
+        (Object): Cluster Roll API response
+        """
+        response = self.send_get(
+            url=self.__base_ocean_cluster_url + "/" + ocean_id + "/roll/" + roll_id,
+            entity_name="ocean (Cluster Roll)"
+        )
+
+        formatted_response = self.convert_json(
+            response, self.camel_to_underscore)
+
+        return formatted_response["response"]["items"][0]
+
+    def get_cluster_nodes(self, ocean_id: str, instance_name: str = None, launch_spec_id: str = None):
+        """
+        Get nodes data of an Ocean cluster.
+
+        # Arguments
+        ocean_id (String): ID of the Ocean Cluster
+        instance_name (String): Get a specific node by instance id
+        launch_spec_id (String): Ocean cluster launch specification identifier.
+
+        # Returns
+        (Object): Ocean Kubernetes AWS Nodes Data response
+        """
+        query_params = dict(instanceName=instance_name,
+                            launchSpecId=launch_spec_id)
+
+        response = self.send_get(
+            url=self.__base_ocean_cluster_url + "/" + ocean_id + "/nodes",
+            entity_name="ocean (Cluster Nodes)",
+            query_params=query_params
+        )
+
+        formatted_response = self.convert_json(
+            response, self.camel_to_underscore)
+
+        return formatted_response["response"]["items"]
+
+    def update_elastigroup_to_ocean(self, group_id: str):
+        """
+        Upgrade an Elastigroup with Kubernetes integration to Ocean for Kubernetes cluster.
+
+        # Arguments
+        group_id (str): Elastigroup identifier
+
+        # Returns
+        (Object): Ocean API response
+        """
+
+        query_params = dict(groupId=group_id)
+
+        response = self.send_post_with_params(
+            body=None,
+            url=self.__base_ocean_cluster_url + "/import",
+            entity_name='ocean_gcp_update_eg_to_ocean',
+            user_query_params=query_params)
+
+        formatted_response = self.convert_json(response,
+                                               self.camel_to_underscore)
+
+        return formatted_response["response"]["items"][0]
+
+    def import_gke_cluster_to_ocean(self, cluster_name: str, location: str,
+                                    import_gke_to_ocean: gcp_ocean.ImportGkeClusterToOcean,
+                                    include_launchSpecs: bool = None, node_pool_name: str = None):
+        """
+        Create an Ocean configuration according to an GKE Cluster configuration.
+
+        # Arguments
+        cluster_name (String): Name of the GKE Cluster.
+        include_launchSpecs (String): When set to "true", GKE cluster node pools will be imported to Ocean custom VNG ("customLaunchSpec") configurations.
+        location (String): Location GKE Cluster Master.
+        node_pool_name (String): Name of the Node Pool to use as a default for the Cluster configuration.
+        import_gke_to_ocean (ImportGkeClusterToOcean): ImportGkeClusterToOcean Object
+
+        # Returns
+        (Object): Ocean GKE Cluster Import Response
+        """
+        import_gke_to_ocean_body = gcp_ocean.ImportGkeClusterToOceanRequest(
+            import_gke_to_ocean)
+
+        excluded_missing_dict = self.exclude_missing(
+            json.loads(import_gke_to_ocean_body.toJSON()))
+
+        formatted_missing_dict = self.convert_json(
+            excluded_missing_dict, self.underscore_to_camel)
+
+        body_json = json.dumps(formatted_missing_dict)
+
+        geturl = self.__base_ocean_cluster_url + "/gke/import"
+
+        query_params = dict(
+            clusterName=cluster_name, includeLaunchSpecs=include_launchSpecs, location=location, nodePoolName=node_pool_name)
+
+        result = self.send_post_with_params(
+            body=body_json,
+            url=geturl,
+            entity_name='import_gke_cluster_to_ocean',
+            user_query_params=query_params)
+
+        formatted_response = self.convert_json(
+            result, self.camel_to_underscore)
+
+        return formatted_response["response"]["items"]
+
+    def launch_nodes_in_vng(self, ocean_launch_spec_id: str, amount: int):
+        """
+        Launch nodes in Virtual Node Group.
+
+        # Arguments
+        ocean_launch_spec_id (String): Ocean cluster launch specification identifier.
+        amount (int): The number of nodes to launch.
+
+        # Returns
+        (Object): Ocean Virtual Node Group Launch API response
+        """
+        launch_node_request = gcp_ocean.LaunchNodesRequest(amount)
+
+        excluded_missing_dict = self.exclude_missing(
+            json.loads(launch_node_request.toJSON()))
+
+        formatted_missing_dict = self.convert_json(
+            excluded_missing_dict, self.underscore_to_camel)
+
+        body_json = json.dumps(formatted_missing_dict)
+
+        response = self.send_put(
+            body=body_json,
+            url=self.__base_ocean_launchspec_url + "/" +
+            ocean_launch_spec_id + "/launchNodes",
+            entity_name='ocean (Cluster Roll)')
+
+        formatted_response = self.convert_json(
+            response, self.camel_to_underscore)
+
+        return formatted_response["response"]["items"][0]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/clients/ocean_cd/__init__.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/clients/ocean_cd/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/clients/setup/__init__.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/clients/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/clients/stateful_node/__init__.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/clients/stateful_node/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/clients/subscription/__init__.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/clients/subscription/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/models/admin/user_mapping.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/models/admin/user_mapping.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/models/elastigroup/aws/__init__.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/models/elastigroup/aws/asg.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/aws/asg.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/models/elastigroup/aws/deployment.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/aws/deployment.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/models/elastigroup/aws/deployment_action.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/aws/deployment_action.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/models/elastigroup/aws/stateful.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/aws/stateful.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/models/elastigroup/azure_v3/__init__.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/azure_v3/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/models/elastigroup/gcp/__init__.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/models/elastigroup/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/models/functions/__init__.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/models/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/models/hpc/aws/__init__.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/models/hpc/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/models/managed_instance/aws/__init__.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/models/managed_instance/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/models/mrscaler/aws/__init__.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/models/mrscaler/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/models/ocean/aws/__init__.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/models/ocean/azure/__init__.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/models/ocean_cd/__init__.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean_cd/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/models/ocean_cd/rollout.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean_cd/rollout.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/models/ocean_cd/rollout_spec.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean_cd/rollout_spec.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/models/ocean_cd/strategy.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean_cd/strategy.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/models/ocean_cd/verification_provider.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean_cd/verification_provider.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/models/ocean_cd/verification_template.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/models/ocean_cd/verification_template.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/models/setup/azure/__init__.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/models/setup/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/models/setup/gcp/__init__.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/models/setup/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/models/stateful_node/__init__.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/models/stateful_node/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/models/subscription/__init__.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/models/subscription/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2/session.py` & `spotinst-sdk2-3.1.0/spotinst_sdk2/session.py`

 * *Files identical despite different names*

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2.egg-info/PKG-INFO` & `spotinst-sdk2-3.1.0/spotinst_sdk2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-sdk2
-Version: 3.0.0
+Version: 3.1.0
 Summary: A Python SDK for Spotinst
 Home-page: https://github.com/spotinst/spotinst-sdk-python
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst spot instances aws azure ec2 cloud infrastructure development elastigroup
 Platform: UNKNOWN
```

### Comparing `spotinst-sdk2-3.0.0/spotinst_sdk2.egg-info/SOURCES.txt` & `spotinst-sdk2-3.1.0/spotinst_sdk2.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 spotinst_sdk2/models/managed_instance/__init__.py
 spotinst_sdk2/models/managed_instance/aws/__init__.py
 spotinst_sdk2/models/mrscaler/__init__.py
 spotinst_sdk2/models/mrscaler/aws/__init__.py
 spotinst_sdk2/models/ocean/__init__.py
 spotinst_sdk2/models/ocean/aws/__init__.py
 spotinst_sdk2/models/ocean/azure/__init__.py
+spotinst_sdk2/models/ocean/gcp/__init__.py
 spotinst_sdk2/models/ocean_cd/__init__.py
 spotinst_sdk2/models/ocean_cd/rollout.py
 spotinst_sdk2/models/ocean_cd/rollout_spec.py
 spotinst_sdk2/models/ocean_cd/strategy.py
 spotinst_sdk2/models/ocean_cd/verification_provider.py
 spotinst_sdk2/models/ocean_cd/verification_template.py
 spotinst_sdk2/models/setup/__init__.py
```

