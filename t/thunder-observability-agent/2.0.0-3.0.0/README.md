# Comparing `tmp/thunder-observability-agent-2.0.0.tar.gz` & `tmp/thunder_observability_agent-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunder-observability-agent-2.0.0.tar", last modified: Thu Nov 30 14:02:19 2023, max compression
+gzip compressed data, was "thunder_observability_agent-3.0.0.tar", last modified: Thu Apr 18 19:28:15 2024, max compression
```

## Comparing `thunder-observability-agent-2.0.0.tar` & `thunder_observability_agent-3.0.0.tar`

### file list

```diff
@@ -1,54 +1,60 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-30 14:02:19.945897 thunder-observability-agent-2.0.0/
--rwxrwxrwx   0 root         (0) root         (0)       40 2023-11-30 13:00:13.000000 thunder-observability-agent-2.0.0/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)     3751 2023-11-30 14:02:19.928099 thunder-observability-agent-2.0.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2370 2023-11-30 13:28:23.000000 thunder-observability-agent-2.0.0/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-11-30 14:02:19.948987 thunder-observability-agent-2.0.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     4956 2023-11-30 13:17:56.000000 thunder-observability-agent-2.0.0/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-30 14:02:19.354184 thunder-observability-agent-2.0.0/thunder-observability-agent/
--rwxrwxrwx   0 root         (0) root         (0)     7532 2023-11-30 13:32:35.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-30 14:02:18.399150 thunder-observability-agent-2.0.0/thunder-observability-agent/common/
--rwxrwxrwx   0 root         (0) root         (0)    23488 2023-11-30 13:00:24.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/common/toa_constant.py
--rwxrwxrwx   0 root         (0) root         (0)     8377 2023-11-30 13:00:24.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/common/toa_helper.py
--rwxrwxrwx   0 root         (0) root         (0)      878 2023-11-30 13:00:13.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/common/toa_logging.py
--rwxrwxrwx   0 root         (0) root         (0)    45930 2023-11-30 13:00:24.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/common/toa_utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-30 14:02:18.000799 thunder-observability-agent-2.0.0/thunder-observability-agent/config/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-30 14:02:19.528494 thunder-observability-agent-2.0.0/thunder-observability-agent/config/.aws/
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-11-30 13:00:13.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/config/.aws/config
--rwxrwxrwx   0 root         (0) root         (0)       65 2023-11-30 13:00:13.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/config/.aws/credentials
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-30 14:02:19.582654 thunder-observability-agent-2.0.0/thunder-observability-agent/config/.azure/
--rwxrwxrwx   0 root         (0) root         (0)      119 2023-11-30 13:00:13.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/config/.azure/credentials
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-30 14:02:19.630652 thunder-observability-agent-2.0.0/thunder-observability-agent/config/.elasticsearch/
--rwxrwxrwx   0 root         (0) root         (0)       28 2023-11-30 13:00:24.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/config/.elasticsearch/credentials
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-30 14:02:19.695407 thunder-observability-agent-2.0.0/thunder-observability-agent/config/.pushgateway/
--rwxrwxrwx   0 root         (0) root         (0)       28 2023-11-30 13:00:24.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/config/.pushgateway/credentials
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-30 14:02:19.738704 thunder-observability-agent-2.0.0/thunder-observability-agent/config/.splunk/
--rwxrwxrwx   0 root         (0) root         (0)       33 2023-11-30 13:00:24.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/config/.splunk/credentials
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-30 14:02:19.783963 thunder-observability-agent-2.0.0/thunder-observability-agent/config/.thunder/
--rwxrwxrwx   0 root         (0) root         (0)      242 2023-11-30 13:00:13.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/config/.thunder/credentials
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-30 14:02:19.828781 thunder-observability-agent-2.0.0/thunder-observability-agent/config/.vmware/
--rwxrwxrwx   0 root         (0) root         (0)       54 2023-11-30 13:00:13.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/config/.vmware/credentials
--rwxrwxrwx   0 root         (0) root         (0)     2827 2023-11-30 13:00:24.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/config.json
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-30 14:02:18.727272 thunder-observability-agent-2.0.0/thunder-observability-agent/handler/
--rwxrwxrwx   0 root         (0) root         (0)     8425 2023-11-30 13:00:24.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/handler/aws_handler.py
--rwxrwxrwx   0 root         (0) root         (0)     9438 2023-11-30 13:00:13.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/handler/azure_handler.py
--rwxrwxrwx   0 root         (0) root         (0)     4650 2023-11-30 13:00:24.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/handler/elasticsearch_handler.py
--rwxrwxrwx   0 root         (0) root         (0)     5254 2023-11-30 13:00:24.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/handler/pushgateway_handler.py
--rwxrwxrwx   0 root         (0) root         (0)     4902 2023-11-30 13:00:24.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/handler/splunk_handler.py
--rwxrwxrwx   0 root         (0) root         (0)    31031 2023-11-30 13:00:24.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/handler/thunder_handler.py
--rwxrwxrwx   0 root         (0) root         (0)     5732 2023-11-30 13:00:13.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/handler/vmware_handler.py
--rwxrwxrwx   0 root         (0) root         (0)     2748 2023-11-30 13:56:36.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/init.sh
--rwxrwxrwx   0 root         (0) root         (0)      523 2023-11-30 13:00:13.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/logging.conf
--rwxrwxrwx   0 root         (0) root         (0)      601 2023-11-30 13:00:24.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/main.properties
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-30 14:02:18.951361 thunder-observability-agent-2.0.0/thunder-observability-agent/processor/
--rwxrwxrwx   0 root         (0) root         (0)     3953 2023-11-30 13:00:24.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/processor/log_processor.py
--rwxrwxrwx   0 root         (0) root         (0)     4508 2023-11-30 13:00:24.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/processor/metric_processor.py
--rwxrwxrwx   0 root         (0) root         (0)     2159 2023-11-30 13:00:13.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/processor/partition_processor.py
--rwxrwxrwx   0 root         (0) root         (0)     3989 2023-11-30 13:00:13.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/processor/thunder_processor.py
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-11-30 13:00:13.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)     1079 2023-11-30 13:00:13.000000 thunder-observability-agent-2.0.0/thunder-observability-agent/toa.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-11-30 14:02:19.893385 thunder-observability-agent-2.0.0/thunder_observability_agent.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     3751 2023-11-30 14:02:16.000000 thunder-observability-agent-2.0.0/thunder_observability_agent.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1868 2023-11-30 14:02:17.000000 thunder-observability-agent-2.0.0/thunder_observability_agent.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-11-30 14:02:16.000000 thunder-observability-agent-2.0.0/thunder_observability_agent.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-11-30 14:02:16.000000 thunder-observability-agent-2.0.0/thunder_observability_agent.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       28 2023-11-30 14:02:16.000000 thunder-observability-agent-2.0.0/thunder_observability_agent.egg-info/top_level.txt
+drwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)        0 2024-04-18 19:28:15.728631 thunder_observability_agent-3.0.0/
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)       40 2024-04-18 19:13:24.000000 thunder_observability_agent-3.0.0/MANIFEST.in
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)     4234 2024-04-18 19:28:15.728631 thunder_observability_agent-3.0.0/PKG-INFO
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)     2777 2024-04-18 19:13:58.000000 thunder_observability_agent-3.0.0/README.md
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)       38 2024-04-18 19:28:15.728631 thunder_observability_agent-3.0.0/setup.cfg
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)     5363 2024-04-18 19:13:58.000000 thunder_observability_agent-3.0.0/setup.py
+drwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)        0 2024-04-18 19:28:15.683617 thunder_observability_agent-3.0.0/thunder-observability-agent/
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)     8448 2024-04-18 19:13:58.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/README.md
+drwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)        0 2024-04-18 19:28:15.594075 thunder_observability_agent-3.0.0/thunder-observability-agent/common/
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)    27375 2024-04-18 19:13:58.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/common/toa_constant.py
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)     8377 2024-04-18 19:13:58.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/common/toa_helper.py
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)      878 2024-04-18 19:13:24.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/common/toa_logging.py
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)    56742 2024-04-18 19:13:58.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/common/toa_utils.py
+drwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)        0 2024-04-18 19:28:15.551447 thunder_observability_agent-3.0.0/thunder-observability-agent/config/
+drwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)        0 2024-04-18 19:28:15.687183 thunder_observability_agent-3.0.0/thunder-observability-agent/config/.aws/
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)       41 2024-04-18 19:13:24.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/config/.aws/config
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)       65 2024-04-18 19:13:24.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/config/.aws/credentials
+drwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)        0 2024-04-18 19:28:15.696806 thunder_observability_agent-3.0.0/thunder-observability-agent/config/.azure/
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)      119 2024-04-18 19:13:24.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/config/.azure/credentials
+drwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)        0 2024-04-18 19:28:15.697887 thunder_observability_agent-3.0.0/thunder-observability-agent/config/.elasticsearch/
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)       28 2024-04-18 19:13:58.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/config/.elasticsearch/credentials
+drwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)        0 2024-04-18 19:28:15.697887 thunder_observability_agent-3.0.0/thunder-observability-agent/config/.gcp/
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)       50 2024-04-18 19:13:58.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/config/.gcp/credentials
+drwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)        0 2024-04-18 19:28:15.707438 thunder_observability_agent-3.0.0/thunder-observability-agent/config/.oci/
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)       23 2024-04-18 19:13:58.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/config/.oci/credentials
+drwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)        0 2024-04-18 19:28:15.707438 thunder_observability_agent-3.0.0/thunder-observability-agent/config/.pushgateway/
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)       28 2024-04-18 19:13:58.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/config/.pushgateway/credentials
+drwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)        0 2024-04-18 19:28:15.714959 thunder_observability_agent-3.0.0/thunder-observability-agent/config/.splunk/
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)       33 2024-04-18 19:13:58.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/config/.splunk/credentials
+drwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)        0 2024-04-18 19:28:15.719094 thunder_observability_agent-3.0.0/thunder-observability-agent/config/.thunder/
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)      242 2024-04-18 19:13:58.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/config/.thunder/credentials
+drwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)        0 2024-04-18 19:28:15.719094 thunder_observability_agent-3.0.0/thunder-observability-agent/config/.vmware/
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)       54 2024-04-18 19:13:24.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/config/.vmware/credentials
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)     3573 2024-04-18 19:13:58.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/config.json
+drwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)        0 2024-04-18 19:28:15.634705 thunder_observability_agent-3.0.0/thunder-observability-agent/handler/
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)     8425 2024-04-18 19:13:58.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/handler/aws_handler.py
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)     9438 2024-04-18 19:13:24.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/handler/azure_handler.py
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)     4650 2024-04-18 19:13:58.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/handler/elasticsearch_handler.py
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)     7318 2024-04-18 19:13:58.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/handler/gcp_handler.py
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)     7723 2024-04-18 19:13:58.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/handler/oci_handler.py
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)     5254 2024-04-18 19:13:58.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/handler/pushgateway_handler.py
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)     4902 2024-04-18 19:13:58.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/handler/splunk_handler.py
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)    32237 2024-04-18 19:13:58.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/handler/thunder_handler.py
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)     5732 2024-04-18 19:13:24.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/handler/vmware_handler.py
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)     3053 2024-04-18 19:20:52.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/init.sh
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)      523 2024-04-18 19:13:24.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/logging.conf
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)      693 2024-04-18 19:13:58.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/main.properties
+drwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)        0 2024-04-18 19:28:15.652287 thunder_observability_agent-3.0.0/thunder-observability-agent/processor/
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)     4730 2024-04-18 19:13:58.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/processor/log_processor.py
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)     5411 2024-04-18 19:13:58.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/processor/metric_processor.py
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)     2159 2024-04-18 19:13:24.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/processor/partition_processor.py
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)     3989 2024-04-18 19:13:24.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/processor/thunder_processor.py
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)       67 2024-04-18 19:13:58.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/requirements.txt
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)     1131 2024-04-18 19:13:58.000000 thunder_observability_agent-3.0.0/thunder-observability-agent/toa.py
+drwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)        0 2024-04-18 19:28:15.725616 thunder_observability_agent-3.0.0/thunder_observability_agent.egg-info/
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)     4234 2024-04-18 19:28:15.000000 thunder_observability_agent-3.0.0/thunder_observability_agent.egg-info/PKG-INFO
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)     2078 2024-04-18 19:28:15.000000 thunder_observability_agent-3.0.0/thunder_observability_agent.egg-info/SOURCES.txt
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)        1 2024-04-18 19:28:15.000000 thunder_observability_agent-3.0.0/thunder_observability_agent.egg-info/dependency_links.txt
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)       65 2024-04-18 19:28:15.000000 thunder_observability_agent-3.0.0/thunder_observability_agent.egg-info/requires.txt
+-rwxrwxrwx   0 vishnoikhushi  (1000) vishnoikhushi  (1000)       28 2024-04-18 19:28:15.000000 thunder_observability_agent-3.0.0/thunder_observability_agent.egg-info/top_level.txt
```

### Comparing `thunder-observability-agent-2.0.0/PKG-INFO` & `thunder_observability_agent-3.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,69 @@
 Metadata-Version: 2.1
 Name: thunder-observability-agent
-Version: 2.0.0
+Version: 3.0.0
 Summary: A10 Thunder Observability Agent is a lightweight autonomous data processing engine that can be externally installed and configured for multiple A10 Thunder Instances to collect, process and publish performance metrics and logs into multiple monitoring dashboard.
 Home-page: https://github.com/a10networks/thunder-observability-agent
-Author: Dinesh Kumar Lohia
-Author-email: dlohia@a10networks.com
+Author: A10 Networks
+Author-email: support@a10networks.com
 Maintainer: A10 Networks
 Maintainer-email: support@a10networks.com
 License: THUNDER OBSERVABILITY AGENT END USER SOFTWARE LICENSE AGREEMENT.
-Keywords: Python,A10Networks,Observability,Agent,Thunder,vThunder,cThunder,Thunder,AWS,Azure,Cloudwatch,VMware,Log,Insight,Application,App,Insight,Analytics,Dashboard,Monitoring,VROPS,VRLI,Operations,A10,Splunk,Prometheus,PushGateway,ElasticSearch,ACOS,A10
+Keywords: Python,A10Networks,Observability,Agent,Thunder,vThunder,cThunder,Thunder,AWS,Azure,Cloudwatch,VMware,Log,Insight,Application,App,Insight,Analytics,Dashboard,Monitoring,VROPS,VRLI,Operations,A10,Splunk,Prometheus,PushGateway,ElasticSearch,ACOS,A10,Google Cloud Platform (GCP),Oracle Cloud Infrastructure (OCI)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Requires-Dist: requests>=2.27.1
 Requires-Dist: boto3>=1.23.10
+Requires-Dist: google-auth>=2.22.0
+Requires-Dist: oci>=2.121.1
 
-# A10's Thunder Observability Agent (TOA) - v2.0.0
+# A10's Thunder Observability Agent (TOA) - v3.0.0
 	The TOA is a lightweight autonomous data processing engine that can be externally installed and configured for any Thunder device.
 	TOA offers the following capabilities on Application Delivery Controller (ADC):
 	
 	- Collects, processes and publishes Thunder metrics. 
 	  The default data collection frequency is 1 minute. 
-	  Thunder metrics can be sent to the platform where Thunder is deployed, which includes AWS, Azure, and VMware or can be sent to shared platforms like Elasticsearch (Kibana), Prometheus (Grafana), and Splunk. 
+	  Thunder metrics can be sent to the platform where Thunder is deployed, which includes AWS, Azure, VMware, Elasticsearch (Kibana), Prometheus (Grafana), and Splunkor can be sent to shared platforms like Google Cloud Platform(GCP), and Oracle Cloud Infrastructure(OCI) . 
 	  Metrics can be sent to any one platform at a time. For more information on Thunder metrics, see Supported Thunder Metrics.
 
 	
 	- Collects, processes, and publishes Thunder Syslogs. 
 	  The default data collection frequency is 1 minute. 
-	  The logs can be published on various platforms like AWS, Azure, VMware, Kibana (Elasticsearch), Grafana (Prometheus and Pushgateway), or Splunk. 
+	  The logs can be published on various platforms like AWS, Azure, VMware, Kibana (Elasticsearch), Grafana (Prometheus and Pushgateway), Splunk Google Cloud Platform(GCP), or Oracle Cloud Infrastructure(OCI). 
       Logs can be sent to any one platform at a time. For more information on Thunder logs, see Supported Thunder Logs.
 
     Supported Monitoring Platforms:
 	1. AWS.
 	2. Azure.
 	3. VMware.
 	4. Splunk
 	5. ElasticSearch-Kibana
 	6. Prometheus-Grafana [PushGateway]
+	7. Google Cloud Platform(GCP)
+	8. Oracle Cloud Infrastructure(OCI)
 
 	Supported Use Cases:
 	1. Monitoring thunder adc metrics or logs or both into AWS Cloudwatch.
 	2. Monitoring thunder adc metrics or logs or both into Azure Application Insight and Log Analytics Workspace.
 	3. Monitoring thunder adc metrics or logs or both into VMware vRealize Operations and Log Insight.
 	4. Monitoring thunder adc metrics or logs or both into Splunk Console.
 	5. Monitoring thunder adc metrics or logs or both into ElasticSearch/Kibana Console.
 	6. Monitoring thunder adc metrics or logs or both into Prometheus/Grafana Console using PushGateway.
+	7. Monitoring thunder adc metrics or logs or both into Google Cloud Platform (GCP).
+	8. Monitoring thunder adc metrics or logs or both into Oracle Cloud Infrastructure (OCI).
 	
 
 	Links:
 	License				: https://www.a10networks.com/wp-content/uploads/EULA_Thunder_Observability_Agent.pdf
-	Open Source (Notice)            : https://github.com/a10networks/thunder-observability-agent/tree/release/v2.0.0/OPEN-SOURCE-DISCLAIMER.pdf
+	Open Source (Notice)            : https://github.com/a10networks/thunder-observability-agent/tree/release/v3.0.0/OPEN-SOURCE-Notice.pdf
 	Documentation		        : https://documentation.a10networks.com/docs/Install/Software/thunder-observability-agent/
-	Repository			: https://github.com/a10networks/thunder-observability-agent/tree/release/v2.0.0
-	Example				: https://github.com/a10networks/thunder-observability-agent/tree/release/v2.0.0/examples
+	Repository			: https://github.com/a10networks/thunder-observability-agent/tree/release/v3.0.0
+	Example				: https://github.com/a10networks/thunder-observability-agent/tree/release/v3.0.0/examples
```

### Comparing `thunder-observability-agent-2.0.0/setup.py` & `thunder_observability_agent-3.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,59 +28,64 @@
 
 
 this_directory = Path(__file__).parent
 readme = (this_directory / "README.md").read_text()
 
 setup(
     name="thunder-observability-agent",
-    version="2.0.0",
+    version="3.0.0",
     description="A10 Thunder Observability Agent is a lightweight autonomous data processing engine that can be externally installed and configured for multiple A10 Thunder Instances to collect, process and publish performance metrics and logs into multiple monitoring dashboard.",
-    keywords=["Python","A10Networks","Observability","Agent","Thunder","vThunder","cThunder","Thunder","AWS","Azure","Cloudwatch","VMware","Log","Insight","Application","App","Insight","Analytics","Dashboard","Monitoring","VROPS","VRLI","Operations","A10", "Splunk", "Prometheus", "PushGateway", "ElasticSearch", "ACOS", "A10"],
+    keywords=["Python","A10Networks","Observability","Agent","Thunder","vThunder","cThunder","Thunder","AWS","Azure","Cloudwatch","VMware","Log","Insight","Application","App","Insight","Analytics","Dashboard","Monitoring","VROPS","VRLI","Operations","A10", "Splunk", "Prometheus", "PushGateway", "ElasticSearch", "ACOS", "A10","Google Cloud Platform (GCP)","Oracle Cloud Infrastructure (OCI)"],
     long_description=readme,
     long_description_content_type='text/markdown',
     Documentation="https://documentation.a10networks.com",
-    Repository="https://github.com/a10networks/thunder-observability-agent/tree/release/v2.0.0",
-    Changelog="https://github.com/a10networks/thunder-observability-agent/tree/release/v2.0.0/README.md",
+    Repository="https://github.com/a10networks/thunder-observability-agent/tree/release/v3.0.0",
+    Changelog="https://github.com/a10networks/thunder-observability-agent/tree/release/v3.0.0/README.md",
     dependencies=[
       "crontab",
       "rsyslog"
       "requests>=2.27.1",
-      "boto3>=1.23.10"
+      "boto3>=1.23.10",
+      "google-auth>=2.22.0",
+      "oci>=2.121.1"
     ],
     # requires-python=">=3.6",
     url="https://github.com/a10networks/thunder-observability-agent",
     # authors=[{"name" == "Dinesh Kumar Lohia", "email" == "dlohia@a10networks.com"}],
-    author="Dinesh Kumar Lohia",
-    author_email="dlohia@a10networks.com",
+    author="A10 Networks",
+    author_email="support@a10networks.com",
     maintainer="A10 Networks",
     maintainer_email="support@a10networks.com",
     # maintainers = [{"name" == "Dinesh Kumar Lohia", "email" =="dlohia@a10networks.com"}],
     license="THUNDER OBSERVABILITY AGENT END USER SOFTWARE LICENSE AGREEMENT.",
     packages=["thunder-observability-agent", "thunder-observability-agent.common",
               "thunder-observability-agent.handler", "thunder-observability-agent.processor", "thunder-observability-agent.config"],
     include_package_data=True,
     data_files=[("thunder-observability-agent", ["thunder-observability-agent/config.json",
                                                  "thunder-observability-agent/logging.conf",
                                                  "thunder-observability-agent/main.properties",
                                                  "thunder-observability-agent/init.sh"]),
                 ("thunder-observability-agent/.tmp/config/.aws", ["thunder-observability-agent/config/.aws/config",
                                                                   "thunder-observability-agent/config/.aws/credentials"]),
                 ("thunder-observability-agent/.tmp/config/.elasticsearch", ["thunder-observability-agent/config/.elasticsearch/credentials"]),
+                ("thunder-observability-agent/.tmp/config/.gcp", ["thunder-observability-agent/config/.gcp/credentials"]),
+                ("thunder-observability-agent/.tmp/config/.oci", ["thunder-observability-agent/config/.oci/credentials"]),
                 ("thunder-observability-agent/.tmp/config/.pushgateway", ["thunder-observability-agent/config/.pushgateway/credentials"]),
                 ("thunder-observability-agent/.tmp/config/.splunk", ["thunder-observability-agent/config/.splunk/credentials"]),
                 ("thunder-observability-agent/.tmp/config/.azure", ["thunder-observability-agent/config/.azure/credentials"]),
                 ("thunder-observability-agent/.tmp/config/.vmware", ["thunder-observability-agent/config/.vmware/credentials"]),
                 ("thunder-observability-agent/.tmp/config/.thunder", ["thunder-observability-agent/config/.thunder/credentials"])
                 ],
     package_dir=package_dir_loc,
     package_data={"thunder-observability-agent": ["*.py", "*.md", "*.txt", "pdf"],
                   "thunder-observability-agent.common": ["*.py"],
                   "thunder-observability-agent.handler": ["*.py"],
                   "thunder-observability-agent.processor": ["*.py"]},
-    install_requires=["requests>=2.27.1", "boto3>=1.23.10"],
+    install_requires=["requests>=2.27.1", "boto3>=1.23.10",
+      "google-auth>=2.22.0","oci>=2.121.1"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: Other/Proprietary License",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

### Comparing `thunder-observability-agent-2.0.0/thunder-observability-agent/README.md` & `thunder_observability_agent-3.0.0/thunder-observability-agent/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,130 +1,147 @@
-# A10's Thunder Observability Agent (TOA) - v2.0.0
-	The TOA is a lightweight autonomous data processing engine that can be externally installed and configured for any Thunder device.
-	TOA offers the following capabilities on Application Delivery Controller (ADC):
-	
-	- Collects, processes, and publishes 14 Thunder metrics. 
- 	  The default data collection frequency is 1 minute. Thunder metrics can be sent to the platform where Thunder is deployed, which includes AWS, Azure, and VMware or can be sent to shared platforms like Elasticsearch (Kibana), Prometheus (Grafana), and Splunk. Metrics can be sent to any one platform at a time. For more information on Thunder metrics, see Supported Thunder Metrics.
-	
-	- Collects, processes, and publishes Thunder Syslogs.
- 	  The default data collection frequency is 1 minute. The logs can be published on various platforms like AWS, Azure, VMware, Kibana (Elasticsearch), Grafana (Prometheus and Pushgateway), or Splunk. 
-	  Logs can be sent to any one platform at a time. For more information on Thunder logs, see Supported Thunder Logs.
-
-	- Manages the data collection, processing, aggregation, and publishing internally.
-	- Provides multitasking capabilities to collect and process multiple Thunder instances and its partitions simultaneously. Default it collects from shared partition.
-	- TOA supports Shared and L3V partitions. The maximum number of partitions supported per Thunder is 20.
-	- Installs on any orchestration platform such as public cloud compute instances, private cloud physical or virtual machines, 	hypervisor VMs, and on-premise physical hardware and is self-driven.
-	- Installs on Linux, CentOS, and Ubuntu platforms as a Python Plugin installation package and Docker containerization.
-	- Supports single or multiple Thunder instances.
-	- Supports Thunder instances running under AWS autoscale group or Azure Virtual machine scale set (VMSS).
-	- Collects data from any type of Thunder device installed on public cloud compute instances, private cloud physical or virtual 	machines, hypervisor VMs and on-premise physical hardware installation.
-	- Publishes data to Azure Cloud, AWS Cloud, and VMware ESXi.
-
-### Supported Use Cases
-	1. Monitoring thunder adc metrics or logs or both into AWS Cloudwatch.
-	2. Monitoring thunder adc metrics or logs or both into Azure Application Insight and Log Analytics Workspace.
-	3. Monitoring thunder adc metrics or logs or both into VMware vRealize Operations and Log Insight.
-	4. Monitoring thunder adc metrics or logs or both into Splunk Console.
-	5. Monitoring thunder adc metrics or logs or both into ElasticSearch/Kibana Console.
-	6. Monitoring thunder adc metrics or logs or both into Prometheus/Grafana Console using PushGateway.
-
-### Supported Installation Options
-	1. Python Plugin.
-		pip install thunder-observability-agent
-		
-	2. Docker Container [Kubernetes manifest].
-		Download from [/dist/kubernetes]
-	
-	For detailed installation and configuration please check documentation section.
-
-### Documentation
-<a href="https://documentation.a10networks.com/docs/Install/Software/thunder-observability-agent/">A10 TOA Documentation Site</a>.
-	
-
-### Supported Thunder vADC Performance Metrics
-	1.  CPU Usage Percentage (Data).
-	2.  Memory Usage Percentage.
-	3.  Disk Usage Percentage.
-	4.  Throughput Rate (Global/BPS)
-	5.  Interface Down Count (Data)
-	6.  Total New Connection (Sec)
-	7.  Transactions Rate (Sec)
-	8.  Server Down Count
-	9.  Server Down Percentage
-	10. SSL Errors Count
-	11. Server Errors Count
-	12. Total Session Count
-	13. Packet Rate (Sec) [Since ACOS 5.2.1-P7+]
-	14. Packet Drop Rate (Sec) [Since ACOS 5.2.1-P7+]
-	   
-### Supported Thunder vADC Performance Logs
-	- SysLogs.
-	
-### Supported Monitoring Platforms
-	1. AWS.
-	2. Azure.
-	3. VMware.
-	4. Splunk
-	5. ElasticSearch-Kibana
-	6. Prometheus-Grafana [PushGateway]
-
-### Supported A10 Thunder ADC Versions
-	64-bit Advanced Core OS (ACOS) version 6.0.2.
-	64-bit Advanced Core OS (ACOS) version 6.0.1.
-	64-bit Advanced Core OS (ACOS) version 6.0.0-P2-SP1.
-	64-bit Advanced Core OS (ACOS) version 6.0.0-P1.
-	64-bit Advanced Core OS (ACOS) version 5.2.1-P7.
-	64-bit Advanced Core OS (ACOS) version 5.2.1-P6.
-	64-bit Advanced Core OS (ACOS) version 5.2.1-P5.
-	64-bit Advanced Core OS (ACOS) version 4.1.4-GR1.
-
-
-### License 
-<a href="https://www.a10networks.com/wp-content/uploads/EULA_Thunder_Observability_Agent.pdf">THUNDER OBSERVABILITY AGENT END USER SOFTWARE LICENSE AGREEMENT</a>.
-
-All rights reserved @A10 Networks Inc.
-
-### Open Source Disclaimer
-	For more information, please refer [/OPEN-SOURCE-DISCLAIMER.pdf]
-
-### Examples
-	
-	VMware	Platform: 
-	UC_01	  Collect metrics and logs from thunder/thunders running in vmware environment and publish it into vmware-vrops and vmware-vrli.
-	UC_02	: Collect logs from thunder/thunders running in vmware environment and publish it into vmware-vrli.
-	UC_03	: Collect metrics from thunder/thunders running in vmware environment and publish it into vmware-vrops.
-	UC_04	: Collect logs from thunder/thunders running in vmware environment and publish it into aws-cloudwatch.
-	UC_05	: Collect logs from thunder/thunders running in vmware environment and publish it into azure-log-workspace.
-	
-	Azure Cloud:
-	UC_01	: Collect metrics and logs from thunder/thunders running in azure environment and publish it into azure-application-insights and azure-log-analytics-workspace.
-	UC_02	: Collect logs from thunder/thunders running in azure environment and publish it into azure-log-analytics-workspace.
-	UC_03	: Collect metrics from thunder/thunders running in azure environment and publish it into azure-application-insights.
-	UC_04	: Collect logs from thunder/thunders running in azure environment and publish it into vmware-vrli.
-	UC_05	: Collect logs from thunder/thunders running in azure environment and publish it into aws-cloudwatch.
-	  
-	AWS Cloud:	 
-	UC_01	: Collect metrics and logs from thunder/thunders running in aws environment and publish it into aws-cloudwatch.
-	UC_02	: Collect only logs of thunder/thunders running in aws environment and publish it into aws-cloudwatch.
-	UC_03	: Collect only metrics of thunder/thunders running in aws environment and publish it into aws-cloudwatch.
-	UC_04	: Collect only logs of thunder/thunders running in aws environment and publish it into vmware-vrli.
-	UC_05	: Collect only logs of thunder/thunders running in aws environment and publish it into azure-log-analytics-workspace.
-	
-	ElasticSearch:
-	UC_01	: Collect metrics and logs from thunder/thunders and publish it into elasticsearch/kibana.
-	UC_02	: Collect only logs of thunder/thunders and publish it into elasticsearch/kibana.
-	UC_03	: Collect only metrics of thunder/thunders and publish it into elasticsearch/kibana.
-
-	Prometheus/Grafana:
-	UC_01	: Collect metrics and logs from thunder/thunders and publish it into prometheus/grafana using pushgateway.
-	UC_02	: Collect only logs of thunder/thunders and publish it into prometheus/grafana using pushgateway.
-	UC_03	: Collect only metrics of thunder/thunders and publish it into prometheus/grafana using pushgateway.
-
-	Splunk:
-	UC_01	: Collect metrics and logs from thunder/thunders and publish it into splunk.
-	UC_02	: Collect only logs of thunder/thunders and publish it into splunk.
-	UC_03	: Collect only metrics of thunder/thunders and publish it into splunk.
-
-	For detail description and sample configuration files, please refer [/examples].
-	
-### Support Information
-	Please contact support@a10networks.com with subject : "TOA Support Request"
+# A10's Thunder Observability Agent (TOA) - v3.0.0
+	The TOA is a lightweight autonomous data processing engine that can be externally installed and configured for any Thunder device.
+	TOA offers the following capabilities on Application Delivery Controller (ADC):
+	
+	- Collects, processes and publishes fourteen Thunder metrics. 
+	  The default data collection frequency is 1 minute. 
+	  The metrics can be published on the same platform where the Thunder instance is deployed.
+	  The metrics can be sent to AWS, Azure, VMware, Splunk, ElasticSearch/Kibana, Prometheus/Grafana, Google Cloud Platform (GCP), or Oracle Cloud Infrastructure(OCI) platforms.
+	  For more information on Thunder metrics, see Thunder Metric Support.
+	
+	- Collects, processes, and publishes Thunder Syslogs. 
+	  The default data collection frequency is 1 minute. 
+	  The logs can be published on the same platform where the Thunder instance is deployed. 
+	  Additionally, logs can also be sent to any AWS, Azure, VMware ESXi, Splunk, ElasticSearch/Kibana, Prometheus/Grafana, Google Cloud Platform (GCP), or Oracle Cloud Infrastructure(OCI) platforms.
+
+	- Manages the data collection, processing, aggregation, and publishing internally.
+	- Provides multitasking capabilities to collect and process multiple Thunder instances and its partitions simultaneously. Default it collects from shared partition.
+	- Installs on any orchestration platform such as public cloud compute instances, private cloud physical or virtual machines, 	hypervisor VMs, and on-premise physical hardware and is self-driven.
+	- Supports Linux, CentOS, and Ubuntu platforms as a Python Plugin installation package and Docker containerization.
+	- Supports single or multiple Thunder instances.
+	- Supports Thunder instances running under AWS autoscale group or Azure Virtual machine scale set (VMSS).
+	- Collects data from any type of Thunder device installed on public cloud compute instances, private cloud physical or virtual 	machines, hypervisor VMs and on-premise physical hardware installation.
+	- Publishes data to Azure Cloud, AWS Cloud, VMware ESXi, Splunk, ElasticSearch/Kibana, Prometheus/Grafana, Google Cloud Platform (GCP), or Oracle Cloud Infrastructure(OCI) platforms.
+
+### Supported Use Cases
+	1. Monitoring thunder adc metrics or logs or both into AWS Cloudwatch.
+	2. Monitoring thunder adc metrics or logs or both into Azure Application Insight and Log Analytics Workspace.
+	3. Monitoring thunder adc metrics or logs or both into VMware vRealize Operations and Log Insight.
+	4. Monitoring thunder adc metrics or logs or both into Splunk Console.
+	5. Monitoring thunder adc metrics or logs or both into ElasticSearch/Kibana Console.
+	6. Monitoring thunder adc metrics or logs or both into Prometheus/Grafana Console.
+	7. Monitoring thunder adc metrics or logs or both into Google Cloud Platform.
+	8. Monitoring thunder adc metrics or logs or both into Oracle Cloud Infrastructure .
+
+### Supported Installation Options
+	1. Python Plugin.
+		pip install thunder-observability-agent
+		
+	2. Docker Container [Kubernetes manifest].
+		Download from [/dist/kubernetes]
+	
+	For detailed installation and configuration please check documentation section.
+
+### Documentation
+<a href="https://documentation.a10networks.com/docs/Install/Software/thunder-observability-agent/">A10 TOA Documentation Site</a>.
+	
+
+### Supported Thunder vADC Performance Metrics
+	1.  CPU Usage Percentage (Data).
+	2.  Memory Usage Percentage.
+	3.  Disk Usage Percentage.
+	4.  Throughput Rate (Global/BPS)
+	5.  Interface Down Count (Data)
+	6.  Total New Connection (Sec)
+	7.  Transactions Rate (Sec)
+	8.  Server Down Count
+	9.  Server Down Percentage
+	10. SSL Errors Count
+	11. Server Errors Count
+	12. Total Session Count
+	13. Packet Rate (Sec) [Since ACOS 5.2.1-P7+]
+	14. Packet Drop Rate (Sec) [Since ACOS 5.2.1-P7+]
+	   
+### Supported Thunder vADC Performance Logs
+	- SysLogs.
+	
+### Supported Monitoring Platforms
+	1. AWS.
+	2. Azure.
+	3. VMware.
+	4. Splunk
+	5. ElasticSearch-Kibana
+	6. Prometheus-Grafana
+	7. Google Cloud Platform
+	8. Oracle Cloud Infrastructure
+
+### Supported A10 Thunder ADC Versions
+	64-bit Advanced Core OS (ACOS) version 6.0.2.
+	64-bit Advanced Core OS (ACOS) version 6.0.1.
+	64-bit Advanced Core OS (ACOS) version 6.0.0-P2-SP1.
+	64-bit Advanced Core OS (ACOS) version 6.0.0-P1.
+	64-bit Advanced Core OS (ACOS) version 5.2.1-P7.
+	64-bit Advanced Core OS (ACOS) version 5.2.1-P6.
+	64-bit Advanced Core OS (ACOS) version 5.2.1-P5.
+	64-bit Advanced Core OS (ACOS) version 4.1.4-GR1.
+
+
+### License 
+<a href="https://www.a10networks.com/wp-content/uploads/EULA_Thunder_Observability_Agent.pdf">THUNDER OBSERVABILITY AGENT END USER SOFTWARE LICENSE AGREEMENT</a>.
+
+All rights reserved @A10 Networks Inc.
+
+### Open Source Disclaimer
+	For more information, please refer [/OPEN-SOURCE-DISCLAIMER.pdf]
+
+### Examples
+	
+	VMware	Platform: 
+	UC_01	  Collect metrics and logs from thunder/thunders running in vmware environment and publish it into vmware-vrops and vmware-vrli.
+	UC_02	: Collect logs from thunder/thunders running in vmware environment and publish it into vmware-vrli.
+	UC_03	: Collect metrics from thunder/thunders running in vmware environment and publish it into vmware-vrops.
+	UC_04	: Collect logs from thunder/thunders running in vmware environment and publish it into aws-cloudwatch.
+	UC_05	: Collect logs from thunder/thunders running in vmware environment and publish it into azure-log-workspace.
+	
+	Azure Cloud:
+	UC_01	: Collect metrics and logs from thunder/thunders running in azure environment and publish it into azure-application-insights and azure-log-analytics-workspace.
+	UC_02	: Collect logs from thunder/thunders running in azure environment and publish it into azure-log-analytics-workspace.
+	UC_03	: Collect metrics from thunder/thunders running in azure environment and publish it into azure-application-insights.
+	UC_04	: Collect logs from thunder/thunders running in azure environment and publish it into vmware-vrli.
+	UC_05	: Collect logs from thunder/thunders running in azure environment and publish it into aws-cloudwatch.
+	  
+	AWS Cloud:	 
+	UC_01	: Collect metrics and logs from thunder/thunders running in aws environment and publish it into aws-cloudwatch.
+	UC_02	: Collect only logs of thunder/thunders running in aws environment and publish it into aws-cloudwatch.
+	UC_03	: Collect only metrics of thunder/thunders running in aws environment and publish it into aws-cloudwatch.
+	UC_04	: Collect only logs of thunder/thunders running in aws environment and publish it into vmware-vrli.
+	UC_05	: Collect only logs of thunder/thunders running in aws environment and publish it into azure-log-analytics-workspace.
+	
+	ElasticSearch:
+	UC_01	: Collect metrics and logs from thunder/thunders and publish it into elasticsearch/kibana.
+	UC_02	: Collect only logs of thunder/thunders and publish it into elasticsearch/kibana.
+	UC_03	: Collect only metrics of thunder/thunders and publish it into elasticsearch/kibana.
+
+	Prometheus/Grafana:
+	UC_01	: Collect metrics and logs from thunder/thunders and publish it into prometheus/grafana using pushgateway.
+	UC_02	: Collect only logs of thunder/thunders and publish it into prometheus/grafana using pushgateway.
+	UC_03	: Collect only metrics of thunder/thunders and publish it into prometheus/grafana using pushgateway.
+
+	Splunk:
+	UC_01	: Collect metrics and logs from thunder/thunders and publish it into splunk.
+	UC_02	: Collect only logs of thunder/thunders and publish it into splunk.
+	UC_03	: Collect only metrics of thunder/thunders and publish it into splunk.
+
+	Google Cloud Platform (GCP):
+	UC_01	: Collect metrics and logs from thunder/thunders and publish it into gcp.
+	UC_02	: Collect only logs of thunder/thunders and publish it into gcp.
+	UC_03	: Collect only metrics of thunder/thunders and publish it into gcp.
+
+	Oracle Cloud Infrastructure (OCI):
+	UC_01	: Collect metrics and logs from thunder/thunders and publish it into oci.
+	UC_02	: Collect only logs of thunder/thunders and publish it into oci.
+	UC_03	: Collect only metrics of thunder/thunders and publish it into oci.
+
+	For detail description and sample configuration files, please refer [/examples].
+	
+### Support Information
+	Please contact support@a10networks.com with subject : "TOA Support Request"
```

#### html2text {}

```diff
@@ -1,95 +1,104 @@
-# A10's Thunder Observability Agent (TOA) - v2.0.0 The TOA is a lightweight
+# A10's Thunder Observability Agent (TOA) - v3.0.0 The TOA is a lightweight
 autonomous data processing engine that can be externally installed and
 configured for any Thunder device. TOA offers the following capabilities on
-Application Delivery Controller (ADC): - Collects, processes, and publishes 14
-Thunder metrics. The default data collection frequency is 1 minute. Thunder
-metrics can be sent to the platform where Thunder is deployed, which includes
-AWS, Azure, and VMware or can be sent to shared platforms like Elasticsearch
-(Kibana), Prometheus (Grafana), and Splunk. Metrics can be sent to any one
-platform at a time. For more information on Thunder metrics, see Supported
-Thunder Metrics. - Collects, processes, and publishes Thunder Syslogs. The
-default data collection frequency is 1 minute. The logs can be published on
-various platforms like AWS, Azure, VMware, Kibana (Elasticsearch), Grafana
-(Prometheus and Pushgateway), or Splunk. Logs can be sent to any one platform
-at a time. For more information on Thunder logs, see Supported Thunder Logs. -
-Manages the data collection, processing, aggregation, and publishing
-internally. - Provides multitasking capabilities to collect and process
-multiple Thunder instances and its partitions simultaneously. Default it
-collects from shared partition. - TOA supports Shared and L3V partitions. The
-maximum number of partitions supported per Thunder is 20. - Installs on any
-orchestration platform such as public cloud compute instances, private cloud
-physical or virtual machines, hypervisor VMs, and on-premise physical hardware
-and is self-driven. - Installs on Linux, CentOS, and Ubuntu platforms as a
-Python Plugin installation package and Docker containerization. - Supports
-single or multiple Thunder instances. - Supports Thunder instances running
-under AWS autoscale group or Azure Virtual machine scale set (VMSS). - Collects
-data from any type of Thunder device installed on public cloud compute
-instances, private cloud physical or virtual machines, hypervisor VMs and on-
-premise physical hardware installation. - Publishes data to Azure Cloud, AWS
-Cloud, and VMware ESXi. ### Supported Use Cases 1. Monitoring thunder adc
-metrics or logs or both into AWS Cloudwatch. 2. Monitoring thunder adc metrics
-or logs or both into Azure Application Insight and Log Analytics Workspace. 3.
-Monitoring thunder adc metrics or logs or both into VMware vRealize Operations
-and Log Insight. 4. Monitoring thunder adc metrics or logs or both into Splunk
-Console. 5. Monitoring thunder adc metrics or logs or both into ElasticSearch/
-Kibana Console. 6. Monitoring thunder adc metrics or logs or both into
-Prometheus/Grafana Console using PushGateway. ### Supported Installation
-Options 1. Python Plugin. pip install thunder-observability-agent 2. Docker
-Container [Kubernetes manifest]. Download from [/dist/kubernetes] For detailed
-installation and configuration please check documentation section. ###
+Application Delivery Controller (ADC): - Collects, processes and publishes
+fourteen Thunder metrics. The default data collection frequency is 1 minute.
+The metrics can be published on the same platform where the Thunder instance is
+deployed. The metrics can be sent to AWS, Azure, VMware, Splunk, ElasticSearch/
+Kibana, Prometheus/Grafana, Google Cloud Platform (GCP), or Oracle Cloud
+Infrastructure(OCI) platforms. For more information on Thunder metrics, see
+Thunder Metric Support. - Collects, processes, and publishes Thunder Syslogs.
+The default data collection frequency is 1 minute. The logs can be published on
+the same platform where the Thunder instance is deployed. Additionally, logs
+can also be sent to any AWS, Azure, VMware ESXi, Splunk, ElasticSearch/Kibana,
+Prometheus/Grafana, Google Cloud Platform (GCP), or Oracle Cloud Infrastructure
+(OCI) platforms. - Manages the data collection, processing, aggregation, and
+publishing internally. - Provides multitasking capabilities to collect and
+process multiple Thunder instances and its partitions simultaneously. Default
+it collects from shared partition. - Installs on any orchestration platform
+such as public cloud compute instances, private cloud physical or virtual
+machines, hypervisor VMs, and on-premise physical hardware and is self-driven.
+- Supports Linux, CentOS, and Ubuntu platforms as a Python Plugin installation
+package and Docker containerization. - Supports single or multiple Thunder
+instances. - Supports Thunder instances running under AWS autoscale group or
+Azure Virtual machine scale set (VMSS). - Collects data from any type of
+Thunder device installed on public cloud compute instances, private cloud
+physical or virtual machines, hypervisor VMs and on-premise physical hardware
+installation. - Publishes data to Azure Cloud, AWS Cloud, VMware ESXi, Splunk,
+ElasticSearch/Kibana, Prometheus/Grafana, Google Cloud Platform (GCP), or
+Oracle Cloud Infrastructure(OCI) platforms. ### Supported Use Cases 1.
+Monitoring thunder adc metrics or logs or both into AWS Cloudwatch. 2.
+Monitoring thunder adc metrics or logs or both into Azure Application Insight
+and Log Analytics Workspace. 3. Monitoring thunder adc metrics or logs or both
+into VMware vRealize Operations and Log Insight. 4. Monitoring thunder adc
+metrics or logs or both into Splunk Console. 5. Monitoring thunder adc metrics
+or logs or both into ElasticSearch/Kibana Console. 6. Monitoring thunder adc
+metrics or logs or both into Prometheus/Grafana Console. 7. Monitoring thunder
+adc metrics or logs or both into Google Cloud Platform. 8. Monitoring thunder
+adc metrics or logs or both into Oracle Cloud Infrastructure . ### Supported
+Installation Options 1. Python Plugin. pip install thunder-observability-agent
+2. Docker Container [Kubernetes manifest]. Download from [/dist/kubernetes] For
+detailed installation and configuration please check documentation section. ###
 Documentation _A_1_0_ _T_O_A_ _D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_i_t_e. ### Supported Thunder vADC
 Performance Metrics 1. CPU Usage Percentage (Data). 2. Memory Usage Percentage.
 3. Disk Usage Percentage. 4. Throughput Rate (Global/BPS) 5. Interface Down
 Count (Data) 6. Total New Connection (Sec) 7. Transactions Rate (Sec) 8. Server
 Down Count 9. Server Down Percentage 10. SSL Errors Count 11. Server Errors
 Count 12. Total Session Count 13. Packet Rate (Sec) [Since ACOS 5.2.1-P7+] 14.
 Packet Drop Rate (Sec) [Since ACOS 5.2.1-P7+] ### Supported Thunder vADC
 Performance Logs - SysLogs. ### Supported Monitoring Platforms 1. AWS. 2.
-Azure. 3. VMware. 4. Splunk 5. ElasticSearch-Kibana 6. Prometheus-Grafana
-[PushGateway] ### Supported A10 Thunder ADC Versions 64-bit Advanced Core OS
-(ACOS) version 6.0.2. 64-bit Advanced Core OS (ACOS) version 6.0.1. 64-bit
-Advanced Core OS (ACOS) version 6.0.0-P2-SP1. 64-bit Advanced Core OS (ACOS)
-version 6.0.0-P1. 64-bit Advanced Core OS (ACOS) version 5.2.1-P7. 64-bit
-Advanced Core OS (ACOS) version 5.2.1-P6. 64-bit Advanced Core OS (ACOS)
-version 5.2.1-P5. 64-bit Advanced Core OS (ACOS) version 4.1.4-GR1. ### License
-_T_H_U_N_D_E_R_ _O_B_S_E_R_V_A_B_I_L_I_T_Y_ _A_G_E_N_T_ _E_N_D_ _U_S_E_R_ _S_O_F_T_W_A_R_E_ _L_I_C_E_N_S_E_ _A_G_R_E_E_M_E_N_T. All rights
-reserved @A10 Networks Inc. ### Open Source Disclaimer For more information,
-please refer [/OPEN-SOURCE-DISCLAIMER.pdf] ### Examples VMware Platform: UC_01
-Collect metrics and logs from thunder/thunders running in vmware environment
-and publish it into vmware-vrops and vmware-vrli. UC_02 : Collect logs from
-thunder/thunders running in vmware environment and publish it into vmware-vrli.
-UC_03 : Collect metrics from thunder/thunders running in vmware environment and
-publish it into vmware-vrops. UC_04 : Collect logs from thunder/thunders
-running in vmware environment and publish it into aws-cloudwatch. UC_05 :
-Collect logs from thunder/thunders running in vmware environment and publish it
-into azure-log-workspace. Azure Cloud: UC_01 : Collect metrics and logs from
+Azure. 3. VMware. 4. Splunk 5. ElasticSearch-Kibana 6. Prometheus-Grafana 7.
+Google Cloud Platform 8. Oracle Cloud Infrastructure ### Supported A10 Thunder
+ADC Versions 64-bit Advanced Core OS (ACOS) version 6.0.2. 64-bit Advanced Core
+OS (ACOS) version 6.0.1. 64-bit Advanced Core OS (ACOS) version 6.0.0-P2-SP1.
+64-bit Advanced Core OS (ACOS) version 6.0.0-P1. 64-bit Advanced Core OS (ACOS)
+version 5.2.1-P7. 64-bit Advanced Core OS (ACOS) version 5.2.1-P6. 64-bit
+Advanced Core OS (ACOS) version 5.2.1-P5. 64-bit Advanced Core OS (ACOS)
+version 4.1.4-GR1. ### License _T_H_U_N_D_E_R_ _O_B_S_E_R_V_A_B_I_L_I_T_Y_ _A_G_E_N_T_ _E_N_D_ _U_S_E_R_ _S_O_F_T_W_A_R_E
+_L_I_C_E_N_S_E_ _A_G_R_E_E_M_E_N_T. All rights reserved @A10 Networks Inc. ### Open Source
+Disclaimer For more information, please refer [/OPEN-SOURCE-DISCLAIMER.pdf] ###
+Examples VMware Platform: UC_01 Collect metrics and logs from thunder/thunders
+running in vmware environment and publish it into vmware-vrops and vmware-vrli.
+UC_02 : Collect logs from thunder/thunders running in vmware environment and
+publish it into vmware-vrli. UC_03 : Collect metrics from thunder/thunders
+running in vmware environment and publish it into vmware-vrops. UC_04 : Collect
+logs from thunder/thunders running in vmware environment and publish it into
+aws-cloudwatch. UC_05 : Collect logs from thunder/thunders running in vmware
+environment and publish it into azure-log-workspace. Azure Cloud: UC_01 :
+Collect metrics and logs from thunder/thunders running in azure environment and
+publish it into azure-application-insights and azure-log-analytics-workspace.
+UC_02 : Collect logs from thunder/thunders running in azure environment and
+publish it into azure-log-analytics-workspace. UC_03 : Collect metrics from
 thunder/thunders running in azure environment and publish it into azure-
-application-insights and azure-log-analytics-workspace. UC_02 : Collect logs
-from thunder/thunders running in azure environment and publish it into azure-
-log-analytics-workspace. UC_03 : Collect metrics from thunder/thunders running
-in azure environment and publish it into azure-application-insights. UC_04 :
-Collect logs from thunder/thunders running in azure environment and publish it
-into vmware-vrli. UC_05 : Collect logs from thunder/thunders running in azure
-environment and publish it into aws-cloudwatch. AWS Cloud: UC_01 : Collect
-metrics and logs from thunder/thunders running in aws environment and publish
-it into aws-cloudwatch. UC_02 : Collect only logs of thunder/thunders running
-in aws environment and publish it into aws-cloudwatch. UC_03 : Collect only
-metrics of thunder/thunders running in aws environment and publish it into aws-
-cloudwatch. UC_04 : Collect only logs of thunder/thunders running in aws
-environment and publish it into vmware-vrli. UC_05 : Collect only logs of
-thunder/thunders running in aws environment and publish it into azure-log-
-analytics-workspace. ElasticSearch: UC_01 : Collect metrics and logs from
-thunder/thunders and publish it into elasticsearch/kibana. UC_02 : Collect only
-logs of thunder/thunders and publish it into elasticsearch/kibana. UC_03 :
-Collect only metrics of thunder/thunders and publish it into elasticsearch/
-kibana. Prometheus/Grafana: UC_01 : Collect metrics and logs from thunder/
-thunders and publish it into prometheus/grafana using pushgateway. UC_02 :
-Collect only logs of thunder/thunders and publish it into prometheus/grafana
-using pushgateway. UC_03 : Collect only metrics of thunder/thunders and publish
-it into prometheus/grafana using pushgateway. Splunk: UC_01 : Collect metrics
-and logs from thunder/thunders and publish it into splunk. UC_02 : Collect only
-logs of thunder/thunders and publish it into splunk. UC_03 : Collect only
-metrics of thunder/thunders and publish it into splunk. For detail description
-and sample configuration files, please refer [/examples]. ### Support
-Information Please contact support@a10networks.com with subject : "TOA Support
-Request"
+application-insights. UC_04 : Collect logs from thunder/thunders running in
+azure environment and publish it into vmware-vrli. UC_05 : Collect logs from
+thunder/thunders running in azure environment and publish it into aws-
+cloudwatch. AWS Cloud: UC_01 : Collect metrics and logs from thunder/thunders
+running in aws environment and publish it into aws-cloudwatch. UC_02 : Collect
+only logs of thunder/thunders running in aws environment and publish it into
+aws-cloudwatch. UC_03 : Collect only metrics of thunder/thunders running in aws
+environment and publish it into aws-cloudwatch. UC_04 : Collect only logs of
+thunder/thunders running in aws environment and publish it into vmware-vrli.
+UC_05 : Collect only logs of thunder/thunders running in aws environment and
+publish it into azure-log-analytics-workspace. ElasticSearch: UC_01 : Collect
+metrics and logs from thunder/thunders and publish it into elasticsearch/
+kibana. UC_02 : Collect only logs of thunder/thunders and publish it into
+elasticsearch/kibana. UC_03 : Collect only metrics of thunder/thunders and
+publish it into elasticsearch/kibana. Prometheus/Grafana: UC_01 : Collect
+metrics and logs from thunder/thunders and publish it into prometheus/grafana
+using pushgateway. UC_02 : Collect only logs of thunder/thunders and publish it
+into prometheus/grafana using pushgateway. UC_03 : Collect only metrics of
+thunder/thunders and publish it into prometheus/grafana using pushgateway.
+Splunk: UC_01 : Collect metrics and logs from thunder/thunders and publish it
+into splunk. UC_02 : Collect only logs of thunder/thunders and publish it into
+splunk. UC_03 : Collect only metrics of thunder/thunders and publish it into
+splunk. Google Cloud Platform (GCP): UC_01 : Collect metrics and logs from
+thunder/thunders and publish it into gcp. UC_02 : Collect only logs of thunder/
+thunders and publish it into gcp. UC_03 : Collect only metrics of thunder/
+thunders and publish it into gcp. Oracle Cloud Infrastructure (OCI): UC_01 :
+Collect metrics and logs from thunder/thunders and publish it into oci. UC_02 :
+Collect only logs of thunder/thunders and publish it into oci. UC_03 : Collect
+only metrics of thunder/thunders and publish it into oci. For detail
+description and sample configuration files, please refer [/examples]. ###
+Support Information Please contact support@a10networks.com with subject : "TOA
+Support Request"
```

### Comparing `thunder-observability-agent-2.0.0/thunder-observability-agent/common/toa_constant.py` & `thunder_observability_agent-3.0.0/thunder-observability-agent/common/toa_constant.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,16 @@
     _AWS_CONFIG_PATH = "aws_config_path"
     
     _AZURE_CREDENTIALS_PATH = "azure_credentials_path"
     _VMWARE_CREDENTIALS_PATH = "vmware_credentials_path"
     _ES_CREDENTIALS_PATH = "elasticsearch_credentials_path"
     _PUSH_GATEWAY_CREDENTIALS_PATH = "pushgateway_credentials_path"
     _SPLUNK_CREDENTIALS_PATH = "splunk_credentials_path"
+    _GCP_CREDENTIALS_PATH = "gcp_credentials_path"
+    _OCI_CREDENTIALS_PATH = "oci_credentials_path"
     _THUNDER_CREDENTIALS_PATH = "thunder_credentials_path"
     _LOG_DELAY_MIN="log_collection_delay_min"
     _CRON_DELAY_MIN="cron_job_frequency_min"
     _THREADPOOL_MAX_WORKERS="max_threads"
     _API_TIMEOUT="http_connection_timeout_sec"
     _SSL_VERIFY="http_ssl_verify"
     _USERNAME="username"
@@ -61,14 +63,24 @@
 
     _SPLUNK_TOKEN_LOG="token_log"
     _SPLUNK_TOKEN_METRICS="token_metric"
     _SPLUNK_HOST="splunk_host"
 
     _ES_HOST="es_host"
     _PUSH_GATEWAY_HOST="pushgateway_host"
+
+    _GCP_PROJECT_ID="gcp_project_id"
+    _GCP_SERVICE_KEY_PATH="gcp_service_key_path"
+    _GCP_LOG_NAME="Thunder"
+
+    _OCI_API_KEY_PATH = "oci_api_key_path"
+    _OCI_LOG_ID = "oci_log_id"
+    _OCI_METRIC_NAMESPACE = "thunder"
+    _OCI_METRIC_RESOURCE_GROUP = "Thunder"
+    _OCI_COMPARTMENT_ID = "oci_compartment_id"
     
     _THUNDER="THUNDER"
     _THUNDERS="thunders"
     _SYSLOG="Syslog"
     _TOA="TOA"
     _NAMESPACE="namespace"
     
@@ -117,15 +129,17 @@
     _ERROR_VMWARE_CREDENTIALS_NOT_FOUND ="VMWare credentials not found. Please check [vmware_credentials_path] in main.properties. "
     _ERROR_AWS_CRED_NOT_FOUND           =_ERROR_REQ_PARAM_NOT_FOUND + "Please check [aws_access_key_id, aws_secret_access_key] in aws credentials. Metric/log publish task abort."
     
 
     _ERROR_ES_CREDENTIALS_NOT_FOUND     ="ElasticSearch credentials not found. Please check [elasticsearch_credentials_path] in main.properties. "
     _ERROR_PUSH_GATEWAY_CREDENTIALS_NOT_FOUND   ="PushGateway credentials not found. Please check [pushgateway_credentials_path] in main.properties. "
     _ERROR_SPLUNK_CREDENTIALS_NOT_FOUND ="Splunk credentials not found. Please check [splunk_credentials_path] in main.properties. "
-    
+    _ERROR_GCP_CREDENTIALS_NOT_FOUND ="GCP credentials not found. Please check [gcp_credentials_path] in main.properties. "
+    _ERROR_OCI_CREDENTIALS_NOT_FOUND = "OCI credentials not found. Please check [oci_credentials_path] in main.properties. "
+
     _ERROR_AZURE_CRED_AUTO_METRIC_NOT_FOUND  = _ERROR_REQ_PARAM_NOT_FOUND + "Please check [azure_client_id, azure_secret_id, azure_tenant_id] in azure credentials. Collect thunders from autoscale task abort."
     _ERROR_AZURE_CREDENTIALS_METRIC_NOT_FOUND= _ERROR_REQ_PARAM_NOT_FOUND + "Please check [azure_client_id, azure_secret_id, azure_tenant_id, azure_location] in azure credentials. Metric publish task abort."
     _ERROR_AZURE_CREDENTIALS_LOG_NOT_FOUND   = _ERROR_REQ_PARAM_NOT_FOUND + "Please check [azure_workspace_primary_key] in azure credentials. Log publish task abort."
     _ERROR_AZURE_CONFIG_METRIC_NOT_FOUND     = _ERROR_REQ_PARAM_NOT_FOUND + "Please check [azure_metric_resource_id] in config.json. Metric publish task abort."
     _ERROR_AZURE_CONFIG_LOG_NOT_FOUND        = _ERROR_REQ_PARAM_NOT_FOUND + "Please check [azure_log_workspace_id] in config.json. Log publish task abort."
     _ERROR_AWS_CONFIG_METRIC_NOT_FOUND       = _ERROR_REQ_PARAM_NOT_FOUND + "Please check [region] in aws config. Metric/Log publish task abort."
     _ERROR_AWS_CONFIG_LOG_NOT_FOUND          = _ERROR_REQ_PARAM_NOT_FOUND + "Please check [aws_log_group_name] in config.json. Log publish task abort."
@@ -140,14 +154,24 @@
     _ERROR_PUSH_GATEWAY_CRED_NOT_FOUND          = _ERROR_REQ_PARAM_NOT_FOUND + "Please check [username, password] in pushgateway credentials. Log/Metric publish task abort."
     _ERROR_PUSH_GATEWAY_CONFIG_NOT_FOUND        = _ERROR_REQ_PARAM_NOT_FOUND + "Please check [pushgateway_host] in config.json. Log/Metric publish task abort."
     
     _ERROR_SPLUNK_CONFIG_NOT_FOUND      = _ERROR_REQ_PARAM_NOT_FOUND + "Please check [splunk_host] in config.json. Log/Metric publish task abort."
     _ERROR_SPLUNK_CRED_METRIC_NOT_FOUND = _ERROR_REQ_PARAM_NOT_FOUND + "Please check [token_metrics] in splunk credentials. Metric publish task abort."
     _ERROR_SPLUNK_CRED_LOG_NOT_FOUND    = _ERROR_REQ_PARAM_NOT_FOUND + "Please check [token_log] in splunk credentials. Log publish task abort."
     
+    _ERROR_GCP_CRED_NOT_FOUND = _ERROR_REQ_PARAM_NOT_FOUND + "Please check [gcp_project_id,gcp_service_key_path] in gcp credentials. Log/Metric publish task abort."
+    _ERROR_GCP_CRED_LOG_NOT_FOUND = _ERROR_REQ_PARAM_NOT_FOUND + "Please check [gcp_log_name] in config.json. Log publish task abort."
+    _ERROR_GCP_CRED_METRIC_NOT_FOUND = _ERROR_REQ_PARAM_NOT_FOUND + "Please check [gcp_project_id,gcp_service_key_path] in config.json. Metric publish task abort."
+    _ERROR_GCP_TOKEN_NOT_CREATED = "ERROR           : Request failed [GCPServiceKeyPath: {}, Trace: {}]."                  + _ERROR_TASK_ABORT
+    
+    _ERROR_OCI_CRED_NOT_FOUND = _ERROR_REQ_PARAM_NOT_FOUND + "Please check [oci_api_key_path] in oci credentials. Log/Metric publish task abort."
+    _ERROR_OCI_CRED_LOG_NOT_FOUND = _ERROR_REQ_PARAM_NOT_FOUND + "Please check [oci_log_id] in config.json. Log publish task abort."
+    _ERROR_OCI_CRED_METRIC_NOT_FOUND = _ERROR_REQ_PARAM_NOT_FOUND + "Please check [oci_compartment_id] in . Metric publish task abort."
+    _ERROR_OCI_FILE_NOT_FOUND = "ERROR           : Request failed [OCIAPIKEYPATH: {}, Trace :{}]."                  + _ERROR_TASK_ABORT
+    _ERROR_OCI_SERVICE_ERROR = "ERROR           : Request failed [Trace :{}]."                  + _ERROR_TASK_ABORT
     
     _ERROR_NO_VALID_LOG_DELAY_IN_MIN_FOUND   = "WARNING       : Invalid value found for "+_LOG_DELAY_MIN  +": [{}]. Only positive integer value is allowed for example [0 or 1 or 2 or nth.]. Considering default value [0] for processing, please check and update in main.properties"
     _ERROR_NO_VALID_CRON_DELAY_IN_MIN_FOUND  = "WARNING       : Invalid value found for "+_CRON_DELAY_MIN +": [{}]. Only positive integer value is allowed for example [0 or 1 or 2 or nth.]. Considering default value [1] for processing, please check and update in main.properties"
     
     
     _ERROR_AWS_LOGSTREAM            = "Error           : Request failed [Trace: {}]. Unable to publish logstream into aws cloudwatch."            + _ERROR_TASK_ABORT
     _ERROR_AWS_CLOUDWATCH_LOGS      = "Error           : Request failed [LogGroupName: {}, Trace: {}]. Unable to publish log into aws cloudwatch."                  + _ERROR_TASK_ABORT
@@ -178,24 +202,28 @@
     _ERROR_METRIC_PACKET_DROP_NOT_FOUND = "Unable to fetch 'Packet Drop Rate (Sec)' metric from thunder."           + _ERROR_TASK_ABORT
     
     _ERROR_PARTITION_NOT_FOUND = "Unable to fetch partition details from thunder."           + _ERROR_TASK_ABORT 
     _ERROR_PARTITION = "Unable to activate partition into thunder."           + _ERROR_TASK_ABORT 
     
     
     
-    _ERROR_VMWARE_VROPS_METRIC              = "Unable to publish metric into vmware vrops."                   + _ERROR_TASK_ABORT
-    _ERROR_VMWARE_VRLI_LOGS                 = "Unable to publish logs into vmware vrli."                            + _ERROR_TASK_ABORT
-    _ERROR_ES_LOGS                          = "Unable to publish logs into elasticsearch."                            + _ERROR_TASK_ABORT
-    _ERROR_ES_METRIC                        = "Unable to publish metric into elasticsearch."                   + _ERROR_TASK_ABORT
-    _ERROR_PUSH_GATEWAY_LOGS                        = "Unable to publish logs into pushgateway."                            + _ERROR_TASK_ABORT
-    _ERROR_PUSH_GATEWAY_METRIC                      = "Unable to publish metric into pushgateway."                   + _ERROR_TASK_ABORT
-    _ERROR_SPLUNK_METRIC                    = "Unable to publish metric into splunk."                     +_ERROR_TASK_ABORT
-    _ERROR_SPLUNK_LOG                       = "Unable to publish logs into splunk."                     +_ERROR_TASK_ABORT
-    _ERROR_AZURE_LOGS                       = "Unable to publish logs into azure log workspace."                    + _ERROR_TASK_ABORT
-    _ERROR_AZURE_METRICS                    = "Unable to publish metric into azure insight/vm."               + _ERROR_TASK_ABORT
+    _ERROR_VMWARE_VROPS_METRIC              = "Unable to publish metric into vmware vrops."          + _ERROR_TASK_ABORT
+    _ERROR_VMWARE_VRLI_LOGS                 = "Unable to publish logs into vmware vrli."             + _ERROR_TASK_ABORT
+    _ERROR_ES_LOGS                          = "Unable to publish logs into elasticsearch."           + _ERROR_TASK_ABORT
+    _ERROR_ES_METRIC                        = "Unable to publish metric into elasticsearch."         + _ERROR_TASK_ABORT
+    _ERROR_PUSH_GATEWAY_LOGS                = "Unable to publish logs into pushgateway."             + _ERROR_TASK_ABORT
+    _ERROR_PUSH_GATEWAY_METRIC              = "Unable to publish metric into pushgateway."           + _ERROR_TASK_ABORT
+    _ERROR_SPLUNK_METRIC                    = "Unable to publish metric into splunk."                +_ERROR_TASK_ABORT
+    _ERROR_SPLUNK_LOG                       = "Unable to publish logs into splunk."                  +_ERROR_TASK_ABORT
+    _ERROR_GCP_METRIC                       = "Unable to publish metric into GCP."                   +_ERROR_TASK_ABORT
+    _ERROR_GCP_LOG                          = "Unable to publish logs into GCP."                     +_ERROR_TASK_ABORT
+    _ERROR_OCI_METRIC                       = "Unable to publish metric into OCI."                   +_ERROR_TASK_ABORT
+    _ERROR_OCI_LOG                          = "Unable to publish logs into OCI."                     +_ERROR_TASK_ABORT
+    _ERROR_AZURE_LOGS                       = "Unable to publish logs into azure log workspace."     + _ERROR_TASK_ABORT
+    _ERROR_AZURE_METRICS                    = "Unable to publish metric into azure insight/vm."      + _ERROR_TASK_ABORT
     _ERROR_AZURE_AUTOSCALE_THUNDERS         = "Unable to fetch thunder instances from azure autoscale [resource_id: {}]."
     
     _ERROR_NO_VALID_PROVIDER_FOUND          ="WARNING       : No provider is enabled for [metric: {}, log: {}]. To enable [provider: {} set to [1]] in config.json."
     _ERROR_NO_VALID_PROVIDER_CONFIG_FOUND   ="WARNING       : No log or metric is enabled. To enable [metric, log set to [1]] in config.json."
     _ERROR_NO_VALID_METRIC_FOUND            ="WARNING       : No metric enabled. To enable [cpu, memory, ...etc seto to [1]] in config.json."
     
     _ERROR_INVALID_THUNDER_AUTO             ="WARNING       : No thunder found for autoscale provider: {}, please check [autoscale[0/1], provider[aws/azure], username, password and resource_id] in thunder credentials. Thunder collection in autoscale mode task abort."
@@ -217,15 +245,17 @@
     _AUTOSCALE="autoscale"
     _PROVIDER="provider"
     _AZURE="azure"
     _AWS="aws"
     _ES="elasticsearch"
     _PUSH_GATEWAY="pushgateway"
     _SPLUNK="splunk"
+    _GCP="gcp"
     _VMWARE="vmware"
+    _OCI = "oci"
     
     _VMWARE_PROVIDER="vmware_provider"
     _VMWARE_METRIC="vmware_metric"
     _VMWARE_LOG="vmware_log"
     
     
     _AWS_PROVIDER="aws_provider"
@@ -239,14 +269,22 @@
     _PUSH_GATEWAY_PROVIDER="pushgateway_provider"
     _PUSH_GATEWAY_METRIC="pushgateway_metric"
     _PUSH_GATEWAY_LOG="pushgateway_log"
 
     _SPLUNK_PROVIDER="splunk_provider"
     _SPLUNK_METRIC="splunk_metric"
     _SPLUNK_LOG="splunk_log"
+
+    _GCP_PROVIDER="gcp_provider"
+    _GCP_METRIC="gcp_metric"
+    _GCP_LOG="gcp_log"
+
+    _OCI_PROVIDER="oci_provider"
+    _OCI_METRIC="oci_metric"
+    _OCI_LOG="oci_log"
     
     _AZURE_CPU="azure_cpu"
     _AZURE_MEMORY="azure_memory"
     _AZURE_DISK="azure_disk"
     _AZURE_THROUGHPUT="azure_throughput"
     _AZURE_INTERFACES="azure_interfaces"
     _AZURE_CPS="azure_cps"
@@ -319,14 +357,45 @@
     _SPLUNK_SERVER_DOWN_COUNT="splunk_server_down_count"
     _SPLUNK_SERVER_DOWN_PERCENTAGE="splunk_server_down_percentage"
     _SPLUNK_SSL_CERT="splunk_ssl_cert"
     _SPLUNK_SERVER_ERROR="splunk_server_error"
     _SPLUNK_SESSION="splunk_sessions"
     _SPLUNK_PACKET_RATE="splunk_packet_rate"
     _SPLUNK_PACKET_DROP="splunk_packet_drop"
+
+    _GCP_CPU="gcp_cpu"
+    _GCP_MEMORY="gcp_memory"
+    _GCP_DISK="gcp_disk"
+    _GCP_THROUGHPUT="gcp_throughput"
+    _GCP_INTERFACES="gcp_interfaces"
+    _GCP_CPS="gcp_cps"
+    _GCP_TPS="gcp_tps"
+    _GCP_SERVER_DOWN_COUNT="gcp_server_down_count"
+    _GCP_SERVER_DOWN_PERCENTAGE="gcp_server_down_percentage"
+    _GCP_SSL_CERT="gcp_ssl_cert"
+    _GCP_SERVER_ERROR="gcp_server_error"
+    _GCP_SESSION="gcp_sessions"
+    _GCP_PACKET_RATE="gcp_packet_rate"
+    _GCP_PACKET_DROP="gcp_packet_drop"
+
+    _OCI_CPU="oci_cpu"
+    _OCI_MEMORY="oci_memory"
+    _OCI_DISK="oci_disk"
+    _OCI_THROUGHPUT="oci_throughput"
+    _OCI_INTERFACES="oci_interfaces"
+    _OCI_CPS="oci_cps"
+    _OCI_TPS="oci_tps"
+    _OCI_SERVER_DOWN_COUNT="oci_server_down_count"
+    _OCI_SERVER_DOWN_PERCENTAGE="oci_server_down_percentage"
+    _OCI_SSL_CERT="oci_ssl_cert"
+    _OCI_SERVER_ERROR="oci_server_error"
+    _OCI_SESSION="oci_sessions"
+    _OCI_PACKET_RATE="oci_packet_rate"
+    _OCI_PACKET_DROP="oci_packet_drop"
+    
     
     _VMWARE_CPU="vmware_cpu"
     _VMWARE_MEMORY="vmware_memory"
     _VMWARE_DISK="vmware_disk"
     _VMWARE_THROUGHPUT="vmware_throughput"
     _VMWARE_INTERFACES="vmware_interfaces"
     _VMWARE_CPS="vmware_cps"
@@ -361,15 +430,20 @@
     _AZURE_MANAGEMENT_RESOURCE="https://management.azure.com/"
     
     _ES_LOG_URL = "https://{}/thunder-logs/_bulk"
     _ES_METRIC_URL = "https://{}/thunder-metrics/_bulk"
     
     _PUSH_GATEWAY_URL="http://{}/metrics/job/thunder"
     
-    _SPLUNK_BASE_URL="https://{}/services/collector/event"  
+    _SPLUNK_BASE_URL="https://{}/services/collector/event"
+
+    _GCP_SCOPE_URL= "https://www.googleapis.com/auth/cloud-platform"
+    _GCP_TIME_SERIES_URL = "https://monitoring.googleapis.com/v3/projects/{}/timeSeries"
+    _GCP_CUSTOM_METRIC_URL = "https://monitoring.googleapis.com/v3/projects/{}/metricDescriptors"
+    _GCP_LOG_URL = "https://logging.googleapis.com/v2/entries:write"  
     
     _CONTENT_TYPE="Content-Type"
     _ACCEPT="Accept"
     _APPLICATION_JSON="application/json"
     _TEXT_XML="text/xml"
     _APPLICATION_URLENCODED="application/x-www-form-urlencoded"
     
@@ -389,10 +463,8 @@
     _INFO_ACTIVE_PROVIDER_METRIC         = "Metric Provider  : {}."
     _INFO_ACTIVE_LOG_PROVIDER_FOUND      = "Log              : {}."
     _INFO_ACTIVE_METRIC_PROVIDER_FOUND   = "Metric           : {}."
     _SUCCESS_METRIC                      = "Published Metric : {} {} [Count: {}] [{}]."
     _SUCCESS_LOG                         = "Published Log    : {} {} [Count: {}]."
     _SKIP_LOG                            = "Published Log    : {} {} [No Data Found]."
     _SKIP_METRIC                         = "Published Metric : {} {} [No Data Found]."
-    _DOCS                                = "Documentation    : www.a10networks.com or https://github.com/a10networks/thunder-observability-agent."
-    
-    
+    _DOCS                                = "Documentation    : www.a10networks.com or https://github.com/a10networks/thunder-observability-agent."
```

### Comparing `thunder-observability-agent-2.0.0/thunder-observability-agent/common/toa_helper.py` & `thunder_observability_agent-3.0.0/thunder-observability-agent/common/toa_helper.py`

 * *Files identical despite different names*

### Comparing `thunder-observability-agent-2.0.0/thunder-observability-agent/common/toa_logging.py` & `thunder_observability_agent-3.0.0/thunder-observability-agent/common/toa_logging.py`

 * *Files identical despite different names*

### Comparing `thunder-observability-agent-2.0.0/thunder-observability-agent/common/toa_utils.py` & `thunder_observability_agent-3.0.0/thunder-observability-agent/common/toa_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,21 +31,24 @@
     _aws_credentials=None
     _aws_config=None
     _azure_credentials=None
     _vmware_credentials=None
     _es_credentials=None
     _pushgateway_credentials=None
     _splunk_credentials=None
+    _gcp_credentials= None
+    _oci_credentials= None
     _metrics=None
     _non_l4v_metrics=None
     _datetime      = datetime.datetime.now(datetime.timezone.utc)
     _datetime_epoc = int(datetime.datetime.timestamp(_datetime) * 1000)
     _datetime_str  =_datetime.strftime("%Y-%m-%dT%H:%M:%S")
     _datetime_id   =_datetime.strftime("%Y%m%d%H%M%S")
     _datetime_gmt_str =  _datetime.strftime('%a, %d %b %Y %H:%M:%S GMT')
+    _datetime_utc_str = _datetime.strftime("%Y-%m-%dT%H:%M:%S+00:00")
     _http_ssl_verify=None
     
     @staticmethod
     def load_properties():
         Utils._main = Utils.load_configuration(Constant._MAIN_CONF_PATH, Utils._main, Constant._ERROR_MAIN_NOT_FOUND, Constant._KEYVALUE) 
     
     @staticmethod
@@ -214,14 +217,59 @@
                         
                 if(Utils._active_log_provider==Constant._SPLUNK_LOG
                     and (not Utils.is_valid(Utils._splunk_credentials)
                        or (Utils.is_valid(Utils._splunk_credentials) 
                           and not Utils.is_valid(Utils._splunk_credentials.get(Constant._SPLUNK_TOKEN_LOG))))):
                         Utils._logger.error(Constant._ERROR_SPLUNK_CRED_LOG_NOT_FOUND)
                         Utils._active_log_provider= None
+
+            if((Utils._active_log_provider==Constant._GCP_LOG or Utils._active_metric_provider==Constant._GCP_METRIC)):
+                if(not Utils.is_valid(Utils._gcp_credentials)): 
+                    Utils._gcp_credentials =  Utils.load_configuration(Utils._main.get(Constant._GCP_CREDENTIALS_PATH), Utils._gcp_credentials, Constant._ERROR_GCP_CREDENTIALS_NOT_FOUND, Constant._KEYVALUE)
+                
+                if(not Utils.is_valid(Utils._gcp_credentials) or (Utils.is_valid(Utils._gcp_credentials)
+                    and (not Utils.is_valid(Utils._gcp_credentials.get(Constant._GCP_PROJECT_ID)) 
+                    or not Utils.is_valid(Utils._gcp_credentials.get(Constant._GCP_SERVICE_KEY_PATH))))): 
+                        Utils._logger.error(Constant._ERROR_GCP_CRED_NOT_FOUND)
+                        Utils._active_log_provider=None
+                        Utils._active_metric_provider=None
+
+                if (Utils._active_metric_provider == Constant._GCP_METRIC):
+                    if (not Utils.is_valid(Utils._gcp_credentials) or (Utils.is_valid(Utils._gcp_credentials)
+                        and (not Utils.is_valid(Utils._gcp_credentials.get(Constant._GCP_PROJECT_ID))or not Utils.is_valid(Utils._gcp_credentials.get(Constant._GCP_SERVICE_KEY_PATH))))):
+                        Utils._logger.error(Constant._ERROR_GCP_CRED_METRIC_NOT_FOUND)
+                        Utils._active_metric_provider = None
+
+                if (Utils._active_log_provider == Constant._GCP_LOG):
+                    if (not Utils.is_valid(Utils._gcp_credentials) or (Utils.is_valid(Utils._gcp_credentials)
+                        and (not Utils.is_valid(Utils._gcp_credentials.get(Constant._GCP_PROJECT_ID))or not Utils.is_valid(Utils._gcp_credentials.get(Constant._GCP_SERVICE_KEY_PATH))))):
+                        Utils._logger.error(Constant._ERROR_GCP_CRED_LOG_NOT_FOUND)
+                        Utils._active_log_provider = None
+
+            if((Utils._active_log_provider==Constant._OCI_LOG or Utils._active_metric_provider==Constant._OCI_METRIC)):
+                if(not Utils.is_valid(Utils._oci_credentials)): 
+                    Utils._oci_credentials =  Utils.load_configuration(Utils._main.get(Constant._OCI_CREDENTIALS_PATH), Utils._oci_credentials, Constant._ERROR_OCI_CREDENTIALS_NOT_FOUND, Constant._KEYVALUE) 
+                
+                if(not Utils.is_valid(Utils._oci_credentials) or (Utils.is_valid(Utils._oci_credentials)
+                    and (not Utils.is_valid(Utils._oci_credentials.get(Constant._OCI_API_KEY_PATH))))): 
+                        Utils._logger.error(Constant._ERROR_OCI_CRED_NOT_FOUND)
+                        Utils._active_log_provider=None
+                        Utils._active_metric_provider=None
+
+                if (Utils._active_metric_provider == Constant._OCI_METRIC):
+                    if(Utils.is_valid(Utils._config) and (not Utils.is_valid(Utils._config.get(Constant._OCI_COMPARTMENT_ID)) )):
+                        Utils._logger.error(Constant._ERROR_OCI_CRED_METRIC_NOT_FOUND)
+                        Utils._active_metric_provider = None
+
+                if (Utils._active_log_provider == Constant._GCP_LOG):
+                    if(Utils.is_valid(Utils._config) and (not Utils.is_valid(Utils._config.get(Constant._OCI_LOG_ID)))):
+                        Utils._logger.error(Constant._ERROR_OCI_CRED_LOG_NOT_FOUND)
+                        Utils._active_log_provider = None
+
+
                   
     @staticmethod
     def validate_provider():
         if(Utils.is_valid(Utils._config)):
             if ((not Utils.is_valid(Utils._config.get(Constant._AZURE_PROVIDER)) or  Utils._config.get(Constant._AZURE_PROVIDER)!=1)
                 and ((Utils.is_valid(Utils._config.get(Constant._AZURE_METRIC)) and Utils._config.get(Constant._AZURE_METRIC) == 1)
                 or ((Utils.is_valid(Utils._config.get(Constant._AZURE_LOG)) and Utils._config.get(Constant._AZURE_LOG) == 1)))):
@@ -247,14 +295,24 @@
                 or ((Utils.is_valid(Utils._config.get(Constant._PUSH_GATEWAY_LOG)) and Utils._config.get(Constant._PUSH_GATEWAY_LOG) == 1)))):
                 Utils._logger.warn(Constant._ERROR_NO_VALID_PROVIDER_FOUND.format(str(Utils._config.get(Constant._PUSH_GATEWAY_METRIC)),str(Utils._config.get(Constant._PUSH_GATEWAY_LOG)), Constant._PUSH_GATEWAY_PROVIDER))
             
             elif ((not Utils.is_valid(Utils._config.get(Constant._SPLUNK_PROVIDER)) or Utils._config.get(Constant._SPLUNK_PROVIDER)!=1)
                 and ((Utils.is_valid(Utils._config.get(Constant._SPLUNK_METRIC)) and Utils._config.get(Constant._SPLUNK_METRIC)==1)
                 or ((Utils.is_valid(Utils._config.get(Constant._SPLUNK_LOG)) and Utils._config.get(Constant._SPLUNK_LOG) == 1)))):
                 Utils._logger.warn(Constant._ERROR_NO_VALID_PROVIDER_FOUND.format(str(Utils._config.get(Constant._SPLUNK_METRIC)),str(Utils._config.get(Constant._SPLUNK_LOG)), Constant._SPLUNK_PROVIDER))
+            
+            elif ((not Utils.is_valid(Utils._config.get(Constant._GCP_PROVIDER)) or Utils._config.get(Constant._GCP_PROVIDER)!=1)
+                and ((Utils.is_valid(Utils._config.get(Constant._GCP_METRIC)) and Utils._config.get(Constant._GCP_METRIC)==1)
+                or ((Utils.is_valid(Utils._config.get(Constant._GCP_LOG)) and Utils._config.get(Constant._GCP_LOG) == 1)))):
+                Utils._logger.warn(Constant._ERROR_NO_VALID_PROVIDER_FOUND.format(str(Utils._config.get(Constant._GCP_METRIC)),str(Utils._config.get(Constant._GCP_LOG)), Constant._GCP_PROVIDER))
+
+            elif ((not Utils.is_valid(Utils._config.get(Constant._OCI_PROVIDER)) or Utils._config.get(Constant._OCI_PROVIDER)!=1)
+                and ((Utils.is_valid(Utils._config.get(Constant._OCI_METRIC)) and Utils._config.get(Constant._OCI_METRIC)==1)
+                or ((Utils.is_valid(Utils._config.get(Constant._OCI_LOG)) and Utils._config.get(Constant._OCI_LOG) == 1)))):
+                Utils._logger.warn(Constant._ERROR_NO_VALID_PROVIDER_FOUND.format(str(Utils._config.get(Constant._OCI_METRIC)),str(Utils._config.get(Constant._OCI_LOG)), Constant._OCI_PROVIDER))
         
     @staticmethod
     def load_active_log_provider():
         if(not Utils.is_valid(Utils._config)):
             return None
         if (Utils._config.get(Constant._AZURE_PROVIDER) 
             and Utils._config.get(Constant._AZURE_LOG)
@@ -288,14 +346,27 @@
             Utils._active_log_provider =  Constant._PUSH_GATEWAY_LOG
         elif (Utils._config.get(Constant._SPLUNK_PROVIDER)
             and Utils._config.get(Constant._SPLUNK_LOG)
             and Utils._config.get(Constant._SPLUNK_PROVIDER) ==1 
             and Utils._config.get(Constant._SPLUNK_LOG)==1):
             Utils._logger.info(Constant._INFO_ACTIVE_PROVIDER_LOG.format(Constant._SPLUNK.upper()))
             Utils._active_log_provider = Constant._SPLUNK_LOG
+        elif (Utils._config.get(Constant._GCP_PROVIDER)
+            and Utils._config.get(Constant._GCP_LOG)
+            and Utils._config.get(Constant._GCP_PROVIDER) ==1 
+            and Utils._config.get(Constant._GCP_LOG)==1):
+            Utils._logger.info(Constant._INFO_ACTIVE_PROVIDER_LOG.format(Constant._GCP.upper()))
+            Utils._active_log_provider = Constant._GCP_LOG
+
+        elif (Utils._config.get(Constant._OCI_PROVIDER)
+            and Utils._config.get(Constant._OCI_LOG)
+            and Utils._config.get(Constant._OCI_PROVIDER) ==1 
+            and Utils._config.get(Constant._OCI_LOG)==1):
+            Utils._logger.info(Constant._INFO_ACTIVE_PROVIDER_LOG.format(Constant._OCI.upper()))
+            Utils._active_log_provider = Constant._OCI_LOG
         if(Utils.is_valid(Utils._active_log_provider)):
             Utils._logger.info(Constant._INFO_ACTIVE_LOG_PROVIDER_FOUND.format(Utils._active_log_provider.upper())) 
         count = 0    
         
         if(Utils._config.get(Constant._AZURE_LOG)==1):
             count = count + 1
         if(Utils._config.get(Constant._VMWARE_LOG)==1):
@@ -303,14 +374,18 @@
         if(Utils._config.get(Constant._AWS_LOG)==1):
             count = count + 1
         if(Utils._config.get(Constant._ES_LOG)==1):
             count = count + 1
         if(Utils._config.get(Constant._PUSH_GATEWAY_LOG)==1):
             count = count + 1
         if(Utils._config.get(Constant._SPLUNK_LOG)==1):
+            count = count + 1
+        if(Utils._config.get(Constant._GCP_LOG)==1):
+            count = count + 1
+        if(Utils._config.get(Constant._OCI_LOG)==1):
             count = count + 1  
         if(count > 1):
             Utils._logger.warn(Constant._WARN_MULTIPLE_LOG_FOUND) 
                    
     @staticmethod
     def load_active_metric_provider():
         if(not Utils.is_valid(Utils._config)):
@@ -415,15 +490,15 @@
             if(Utils._config.get(Constant._VMWARE_PACKET_DROP)==1):
                 Utils._metrics.append(Constant._VMWARE_PACKET_DROP)
                 
         elif (Utils._config.get(Constant._AWS_PROVIDER) 
             and Utils._config.get(Constant._AWS_METRIC)
             and Utils._config.get(Constant._AWS_PROVIDER) == 1
             and Utils._config.get(Constant._AWS_METRIC)==1):
-            Utils._active_metric_provider=Constant._AWS_METRIC;
+            Utils._active_metric_provider=Constant._AWS_METRIC
             Utils._logger.info(Constant._INFO_ACTIVE_PROVIDER_METRIC.format(Constant._AWS.upper()))
             Utils._metrics = []
             Utils._non_l4v_metrics = []
             if(Utils._config.get(Constant._AWS_CPU)==1):
                 Utils._metrics.append(Constant._AWS_CPU)
                 
             if(Utils._config.get(Constant._AWS_MEMORY)==1):
@@ -610,14 +685,114 @@
                 Utils._metrics.append(Constant._SPLUNK_SESSION)
         
             if(Utils._config.get(Constant._SPLUNK_PACKET_RATE)==1):
                 Utils._metrics.append(Constant._SPLUNK_PACKET_RATE)
         
             if(Utils._config.get(Constant._SPLUNK_PACKET_DROP)==1):
                 Utils._metrics.append(Constant._SPLUNK_PACKET_DROP)
+        
+        elif (Utils._config.get(Constant._GCP_PROVIDER) 
+            and Utils._config.get(Constant._GCP_METRIC)
+            and Utils._config.get(Constant._GCP_PROVIDER) == 1
+            and Utils._config.get(Constant._GCP_METRIC)==1):
+            Utils._active_metric_provider=Constant._GCP_METRIC
+            Utils._logger.info(Constant._INFO_ACTIVE_PROVIDER_METRIC.format(Constant._GCP.upper()))
+            Utils._metrics = []
+            Utils._non_l4v_metrics = []
+            if(Utils._config.get(Constant._GCP_CPU)==1):
+                Utils._metrics.append(Constant._GCP_CPU)
+        
+            if(Utils._config.get(Constant._GCP_MEMORY)==1):
+                Utils._non_l4v_metrics.append(Constant._GCP_MEMORY)
+        
+            if(Utils._config.get(Constant._GCP_DISK)==1):
+                Utils._non_l4v_metrics.append(Constant._GCP_DISK)
+        
+            if(Utils._config.get(Constant._GCP_THROUGHPUT)==1):
+                Utils._metrics.append(Constant._GCP_THROUGHPUT)
+        
+            if(Utils._config.get(Constant._GCP_INTERFACES)==1):
+                Utils._metrics.append(Constant._GCP_INTERFACES)
+        
+            if(Utils._config.get(Constant._GCP_CPS)==1):
+                Utils._metrics.append(Constant._GCP_CPS)
+        
+            if(Utils._config.get(Constant._GCP_TPS)==1):
+                Utils._metrics.append(Constant._GCP_TPS)
+        
+            if(Utils._config.get(Constant._GCP_SERVER_DOWN_COUNT)==1):
+                Utils._metrics.append(Constant._GCP_SERVER_DOWN_COUNT) 
+        
+            if(Utils._config.get(Constant._GCP_SERVER_DOWN_PERCENTAGE)==1):
+                Utils._metrics.append(Constant._GCP_SERVER_DOWN_PERCENTAGE)
+        
+            if(Utils._config.get(Constant._GCP_SSL_CERT)==1):
+                Utils._metrics.append(Constant._GCP_SSL_CERT) 
+        
+            if(Utils._config.get(Constant._GCP_SERVER_ERROR)==1):
+                Utils._metrics.append(Constant._GCP_SERVER_ERROR)
+        
+            if(Utils._config.get(Constant._GCP_SESSION)==1):
+                Utils._metrics.append(Constant._GCP_SESSION)
+        
+            if(Utils._config.get(Constant._GCP_PACKET_RATE)==1):
+                Utils._metrics.append(Constant._GCP_PACKET_RATE)
+        
+            if(Utils._config.get(Constant._GCP_PACKET_DROP)==1):
+                Utils._metrics.append(Constant._GCP_PACKET_DROP)
+        
+        elif (Utils._config.get(Constant._OCI_PROVIDER) 
+            and Utils._config.get(Constant._OCI_METRIC)
+            and Utils._config.get(Constant._OCI_PROVIDER) == 1
+            and Utils._config.get(Constant._OCI_METRIC)==1):
+            Utils._active_metric_provider=Constant._OCI_METRIC
+            Utils._logger.info(Constant._INFO_ACTIVE_PROVIDER_METRIC.format(Constant._OCI.upper()))
+            Utils._metrics = []
+            Utils._non_l4v_metrics = []
+            if(Utils._config.get(Constant._OCI_CPU)==1):
+                Utils._metrics.append(Constant._OCI_CPU)
+        
+            if(Utils._config.get(Constant._OCI_MEMORY)==1):
+                Utils._non_l4v_metrics.append(Constant._OCI_MEMORY)
+        
+            if(Utils._config.get(Constant._OCI_DISK)==1):
+                Utils._non_l4v_metrics.append(Constant._OCI_DISK)
+        
+            if(Utils._config.get(Constant._OCI_THROUGHPUT)==1):
+                Utils._metrics.append(Constant._OCI_THROUGHPUT)
+        
+            if(Utils._config.get(Constant._OCI_INTERFACES)==1):
+                Utils._metrics.append(Constant._OCI_INTERFACES)
+        
+            if(Utils._config.get(Constant._OCI_CPS)==1):
+                Utils._metrics.append(Constant._OCI_CPS)
+        
+            if(Utils._config.get(Constant._OCI_TPS)==1):
+                Utils._metrics.append(Constant._OCI_TPS)
+        
+            if(Utils._config.get(Constant._OCI_SERVER_DOWN_COUNT)==1):
+                Utils._metrics.append(Constant._OCI_SERVER_DOWN_COUNT) 
+        
+            if(Utils._config.get(Constant._OCI_SERVER_DOWN_PERCENTAGE)==1):
+                Utils._metrics.append(Constant._OCI_SERVER_DOWN_PERCENTAGE)
+        
+            if(Utils._config.get(Constant._OCI_SSL_CERT)==1):
+                Utils._metrics.append(Constant._OCI_SSL_CERT) 
+        
+            if(Utils._config.get(Constant._OCI_SERVER_ERROR)==1):
+                Utils._metrics.append(Constant._OCI_SERVER_ERROR)
+        
+            if(Utils._config.get(Constant._OCI_SESSION)==1):
+                Utils._metrics.append(Constant._OCI_SESSION)
+        
+            if(Utils._config.get(Constant._OCI_PACKET_RATE)==1):
+                Utils._metrics.append(Constant._OCI_PACKET_RATE)
+        
+            if(Utils._config.get(Constant._OCI_PACKET_DROP)==1):
+                Utils._metrics.append(Constant._OCI_PACKET_DROP)
                 
         if(Utils.is_valid(Utils._active_metric_provider)):
             Utils._logger.info(Constant._INFO_ACTIVE_METRIC_PROVIDER_FOUND.format(Utils._active_metric_provider.upper())) 
         count = 0    
         
         if(Utils._config.get(Constant._AZURE_METRIC)==1):
             count = count + 1
@@ -626,14 +801,18 @@
         if(Utils._config.get(Constant._AWS_METRIC)==1):
             count = count + 1
         if(Utils._config.get(Constant._ES_METRIC)==1):
             count = count + 1
         if(Utils._config.get(Constant._PUSH_GATEWAY_METRIC)==1):
             count = count + 1
         if(Utils._config.get(Constant._SPLUNK_METRIC)==1):
+            count = count + 1 
+        if(Utils._config.get(Constant._GCP_METRIC)==1):
+            count = count + 1    
+        if(Utils._config.get(Constant._OCI_METRIC)==1):
             count = count + 1    
         if(count > 1):
             Utils._logger.warn(Constant._WARN_MULTIPLE_METRIC_FOUND)  
             
     @staticmethod
     def validate():
         status=True
@@ -660,15 +839,15 @@
      
     @staticmethod
     def is_valid(*arguments):
         valid=True
         for arg in arguments:
             if(arg is None or arg =="XXXX" or arg=="" or arg==" " or arg=="none" or arg=="None"):
                 return False
-        return valid;
+        return valid
     
     @staticmethod
     def is_integer(n):
         try:
             float(n)
         except ValueError:
             return False
@@ -821,8 +1000,9 @@
             if log['log-data'] not in unq:
                 logs.append(log)
                 unq.add(log['log-data'])
         return logs       
         
         
         
+
```

### Comparing `thunder-observability-agent-2.0.0/thunder-observability-agent/handler/aws_handler.py` & `thunder_observability_agent-3.0.0/thunder-observability-agent/handler/aws_handler.py`

 * *Files identical despite different names*

### Comparing `thunder-observability-agent-2.0.0/thunder-observability-agent/handler/azure_handler.py` & `thunder_observability_agent-3.0.0/thunder-observability-agent/handler/azure_handler.py`

 * *Files identical despite different names*

### Comparing `thunder-observability-agent-2.0.0/thunder-observability-agent/handler/elasticsearch_handler.py` & `thunder_observability_agent-3.0.0/thunder-observability-agent/handler/elasticsearch_handler.py`

 * *Files identical despite different names*

### Comparing `thunder-observability-agent-2.0.0/thunder-observability-agent/handler/pushgateway_handler.py` & `thunder_observability_agent-3.0.0/thunder-observability-agent/handler/pushgateway_handler.py`

 * *Files identical despite different names*

### Comparing `thunder-observability-agent-2.0.0/thunder-observability-agent/handler/splunk_handler.py` & `thunder_observability_agent-3.0.0/thunder-observability-agent/handler/splunk_handler.py`

 * *Files identical despite different names*

### Comparing `thunder-observability-agent-2.0.0/thunder-observability-agent/handler/thunder_handler.py` & `thunder_observability_agent-3.0.0/thunder-observability-agent/handler/thunder_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -432,54 +432,54 @@
          
             except Exception as exp:
                 self._logger.debug(exp)
                 return None
                                                
     def collect_metric(self):
         
-        if(self._metric == Constant._AWS_CPS or self._metric == Constant._AZURE_CPS or self._metric == Constant._VMWARE_CPS or self._metric == Constant._PUSH_GATEWAY_CPS or self._metric == Constant._ES_CPS or self._metric == Constant._SPLUNK_CPS):
+        if(self._metric == Constant._AWS_CPS or self._metric == Constant._AZURE_CPS or self._metric == Constant._VMWARE_CPS or self._metric == Constant._PUSH_GATEWAY_CPS or self._metric == Constant._ES_CPS or self._metric == Constant._SPLUNK_CPS or self._metric == Constant._GCP_CPS or self._metric == Constant._OCI_CPS):
             return self.collect_metric_cps()
         
-        elif(self._metric == Constant._AWS_CPU or self._metric == Constant._AZURE_CPU or self._metric == Constant._VMWARE_CPU or self._metric == Constant._PUSH_GATEWAY_CPU or self._metric == Constant._ES_CPU or self._metric == Constant._SPLUNK_CPU): 
+        elif(self._metric == Constant._AWS_CPU or self._metric == Constant._AZURE_CPU or self._metric == Constant._VMWARE_CPU or self._metric == Constant._PUSH_GATEWAY_CPU or self._metric == Constant._ES_CPU or self._metric == Constant._SPLUNK_CPU or self._metric == Constant._GCP_CPU or self._metric == Constant._OCI_CPU): 
             return self.collect_metric_cpu()
             
-        elif(self._metric == Constant._AWS_MEMORY or self._metric == Constant._AZURE_MEMORY or self._metric == Constant._VMWARE_MEMORY or self._metric == Constant._PUSH_GATEWAY_MEMORY or self._metric == Constant._ES_MEMORY or self._metric == Constant._SPLUNK_MEMORY):
+        elif(self._metric == Constant._AWS_MEMORY or self._metric == Constant._AZURE_MEMORY or self._metric == Constant._VMWARE_MEMORY or self._metric == Constant._PUSH_GATEWAY_MEMORY or self._metric == Constant._ES_MEMORY or self._metric == Constant._SPLUNK_MEMORY or self._metric == Constant._GCP_MEMORY or self._metric == Constant._OCI_MEMORY):
             return self.collect_metric_memory()
         
-        elif(self._metric == Constant._AWS_DISK or self._metric == Constant._AZURE_DISK or self._metric == Constant._VMWARE_DISK or self._metric == Constant._PUSH_GATEWAY_DISK or self._metric == Constant._ES_DISK or self._metric == Constant._SPLUNK_DISK):
+        elif(self._metric == Constant._AWS_DISK or self._metric == Constant._AZURE_DISK or self._metric == Constant._VMWARE_DISK or self._metric == Constant._PUSH_GATEWAY_DISK or self._metric == Constant._ES_DISK or self._metric == Constant._SPLUNK_DISK or self._metric == Constant._GCP_DISK or self._metric == Constant._OCI_DISK):
             return self.collect_metric_disk()
         
-        elif(self._metric == Constant._AWS_THROUGHPUT or self._metric == Constant._AZURE_THROUGHPUT or self._metric == Constant._VMWARE_THROUGHPUT or self._metric == Constant._PUSH_GATEWAY_THROUGHPUT or self._metric == Constant._ES_THROUGHPUT or self._metric == Constant._SPLUNK_THROUGHPUT):
+        elif(self._metric == Constant._AWS_THROUGHPUT or self._metric == Constant._AZURE_THROUGHPUT or self._metric == Constant._VMWARE_THROUGHPUT or self._metric == Constant._PUSH_GATEWAY_THROUGHPUT or self._metric == Constant._ES_THROUGHPUT or self._metric == Constant._SPLUNK_THROUGHPUT or self._metric == Constant._GCP_THROUGHPUT or self._metric == Constant._OCI_THROUGHPUT):
             return self.collect_metric_throughput()
         
-        elif(self._metric == Constant._AWS_INTERFACES or self._metric == Constant._AZURE_INTERFACES or self._metric == Constant._VMWARE_INTERFACES or self._metric == Constant._PUSH_GATEWAY_INTERFACES or self._metric == Constant._ES_INTERFACES or self._metric == Constant._SPLUNK_INTERFACES):
+        elif(self._metric == Constant._AWS_INTERFACES or self._metric == Constant._AZURE_INTERFACES or self._metric == Constant._VMWARE_INTERFACES or self._metric == Constant._PUSH_GATEWAY_INTERFACES or self._metric == Constant._ES_INTERFACES or self._metric == Constant._SPLUNK_INTERFACES or self._metric == Constant._GCP_INTERFACES or self._metric == Constant._OCI_INTERFACES):
             return self.collect_metric_interface()
         
-        elif(self._metric == Constant._AWS_TPS or self._metric == Constant._AZURE_TPS or self._metric == Constant._VMWARE_TPS or self._metric == Constant._PUSH_GATEWAY_TPS or self._metric == Constant._ES_TPS or self._metric == Constant._SPLUNK_TPS):
+        elif(self._metric == Constant._AWS_TPS or self._metric == Constant._AZURE_TPS or self._metric == Constant._VMWARE_TPS or self._metric == Constant._PUSH_GATEWAY_TPS or self._metric == Constant._ES_TPS or self._metric == Constant._SPLUNK_TPS or self._metric == Constant._GCP_TPS or self._metric == Constant._OCI_TPS):
             return self.collect_metric_transaction()
         
-        elif(self._metric == Constant._AWS_SERVER_DOWN_COUNT or self._metric == Constant._AZURE_SERVER_DOWN_COUNT or self._metric == Constant._VMWARE_SERVER_DOWN_COUNT or self._metric == Constant._PUSH_GATEWAY_SERVER_DOWN_COUNT or self._metric == Constant._ES_SERVER_DOWN_COUNT or self._metric == Constant._SPLUNK_SERVER_DOWN_COUNT):
+        elif(self._metric == Constant._AWS_SERVER_DOWN_COUNT or self._metric == Constant._AZURE_SERVER_DOWN_COUNT or self._metric == Constant._VMWARE_SERVER_DOWN_COUNT or self._metric == Constant._PUSH_GATEWAY_SERVER_DOWN_COUNT or self._metric == Constant._ES_SERVER_DOWN_COUNT or self._metric == Constant._SPLUNK_SERVER_DOWN_COUNT or self._metric == Constant._GCP_SERVER_DOWN_COUNT or self._metric == Constant._OCI_SERVER_DOWN_COUNT):
             return self.collect_metric_server_down()
             
-        elif(self._metric == Constant._AWS_SERVER_DOWN_PERCENTAGE or self._metric == Constant._AZURE_SERVER_DOWN_PERCENTAGE or self._metric == Constant._VMWARE_SERVER_DOWN_PERCENTAGE or self._metric == Constant._PUSH_GATEWAY_SERVER_DOWN_PERCENTAGE or self._metric == Constant._ES_SERVER_DOWN_PERCENTAGE or self._metric == Constant._SPLUNK_SERVER_DOWN_PERCENTAGE):
+        elif(self._metric == Constant._AWS_SERVER_DOWN_PERCENTAGE or self._metric == Constant._AZURE_SERVER_DOWN_PERCENTAGE or self._metric == Constant._VMWARE_SERVER_DOWN_PERCENTAGE or self._metric == Constant._PUSH_GATEWAY_SERVER_DOWN_PERCENTAGE or self._metric == Constant._ES_SERVER_DOWN_PERCENTAGE or self._metric == Constant._SPLUNK_SERVER_DOWN_PERCENTAGE or self._metric == Constant._GCP_SERVER_DOWN_PERCENTAGE or self._metric == Constant._OCI_SERVER_DOWN_PERCENTAGE):
             return self.collect_metric_server_down_per()
 
-        elif(self._metric == Constant._AWS_SSL_CERT or self._metric == Constant._AZURE_SSL_CERT  or self._metric == Constant._VMWARE_SSL_CERT or self._metric == Constant._PUSH_GATEWAY_SSL_CERT or self._metric == Constant._ES_SSL_CERT or self._metric == Constant._SPLUNK_SSL_CERT):
+        elif(self._metric == Constant._AWS_SSL_CERT or self._metric == Constant._AZURE_SSL_CERT  or self._metric == Constant._VMWARE_SSL_CERT or self._metric == Constant._PUSH_GATEWAY_SSL_CERT or self._metric == Constant._ES_SSL_CERT or self._metric == Constant._SPLUNK_SSL_CERT or self._metric == Constant._GCP_SSL_CERT or self._metric == Constant._OCI_SSL_CERT):
             return self.collect_metric_ssl()
         
-        elif(self._metric == Constant._AWS_SERVER_ERROR or self._metric == Constant._AZURE_SERVER_ERROR or self._metric == Constant._VMWARE_SERVER_ERROR or self._metric == Constant._PUSH_GATEWAY_SERVER_ERROR or self._metric == Constant._ES_SERVER_ERROR or self._metric == Constant._SPLUNK_SERVER_ERROR):
+        elif(self._metric == Constant._AWS_SERVER_ERROR or self._metric == Constant._AZURE_SERVER_ERROR or self._metric == Constant._VMWARE_SERVER_ERROR or self._metric == Constant._PUSH_GATEWAY_SERVER_ERROR or self._metric == Constant._ES_SERVER_ERROR or self._metric == Constant._SPLUNK_SERVER_ERROR or self._metric == Constant._GCP_SERVER_ERROR or self._metric == Constant._OCI_SERVER_ERROR):
             return self.collect_metric_server_error()
             
-        elif(self._metric == Constant._AWS_SESSION or self._metric == Constant._AZURE_SESSION or self._metric == Constant._VMWARE_SESSION or self._metric == Constant._PUSH_GATEWAY_SESSION or self._metric == Constant._ES_SESSION or self._metric == Constant._SPLUNK_SESSION):
+        elif(self._metric == Constant._AWS_SESSION or self._metric == Constant._AZURE_SESSION or self._metric == Constant._VMWARE_SESSION or self._metric == Constant._PUSH_GATEWAY_SESSION or self._metric == Constant._ES_SESSION or self._metric == Constant._SPLUNK_SESSION or self._metric == Constant._GCP_SESSION or self._metric == Constant._OCI_SESSION):
             return self.collect_metric_session()
             
-        elif(self._metric == Constant._AWS_PACKET_RATE or self._metric == Constant._AZURE_PACKET_RATE or self._metric == Constant._VMWARE_PACKET_RATE or self._metric == Constant._PUSH_GATEWAY_PACKET_RATE or self._metric == Constant._ES_PACKET_RATE or self._metric == Constant._SPLUNK_PACKET_RATE):
+        elif(self._metric == Constant._AWS_PACKET_RATE or self._metric == Constant._AZURE_PACKET_RATE or self._metric == Constant._VMWARE_PACKET_RATE or self._metric == Constant._PUSH_GATEWAY_PACKET_RATE or self._metric == Constant._ES_PACKET_RATE or self._metric == Constant._SPLUNK_PACKET_RATE or self._metric == Constant._GCP_PACKET_RATE or self._metric == Constant._OCI_PACKET_RATE):
             return self.collect_metric_packet_rate()
             
-        elif(self._metric == Constant._AWS_PACKET_DROP or self._metric == Constant._AZURE_PACKET_DROP or self._metric == Constant._VMWARE_PACKET_DROP or self._metric == Constant._PUSH_GATEWAY_PACKET_DROP or self._metric == Constant._ES_PACKET_DROP or self._metric == Constant._SPLUNK_PACKET_DROP):
+        elif(self._metric == Constant._AWS_PACKET_DROP or self._metric == Constant._AZURE_PACKET_DROP or self._metric == Constant._VMWARE_PACKET_DROP or self._metric == Constant._PUSH_GATEWAY_PACKET_DROP or self._metric == Constant._ES_PACKET_DROP or self._metric == Constant._SPLUNK_PACKET_DROP or self._metric == Constant._GCP_PACKET_DROP or self._metric == Constant._OCI_PACKET_DROP):
             return self.collect_metric_packet_drop()
 
     def partitions(self):
         try:
             response = Utils.rest_api(self._url+"/partition", self._headers, {}, Constant._GET, Constant._ERROR_PARTITION_NOT_FOUND, self._thunder.get(Constant._IP))
             if(not Utils.is_valid(response)): 
                 return None
```

### Comparing `thunder-observability-agent-2.0.0/thunder-observability-agent/handler/vmware_handler.py` & `thunder_observability_agent-3.0.0/thunder-observability-agent/handler/vmware_handler.py`

 * *Files identical despite different names*

### Comparing `thunder-observability-agent-2.0.0/thunder-observability-agent/init.sh` & `thunder_observability_agent-3.0.0/thunder-observability-agent/init.sh`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 ### virtualenv toaenv
 ### source toaenv/bin/activate
 ### echo "Successfully created python virtual environment with name 'toaenv'."
 
 ### Install plugin dependencies ###
 pip3 install requests>=2.27.1
 pip3 install boto3>=1.23.10
+pip3 install google-auth>=2.22.0
+pip3 install oci>=2.121.1
 echo "Successfully installed TOA dependencies."
 
 ### Set default toa config directory ###
 export TOA_CONFIG_PATH="/usr/toaenv/thunder-observability-agent"
 echo "TOA configuration files directory: /usr/toaenv/thunder-observability-agent"
 echo "TOA_CONFIG_PATH : "$TOA_CONFIG_PATH
 
@@ -71,14 +73,26 @@
 
 if [ ! -d "/root/.splunk" ]
 then
     ### echo "Directory /root/.splunk DOES NOT exists." 
 	cp -r .tmp/config/.splunk /root/.splunk
 fi
 
+if [ ! -d "/root/.gcp" ]
+then
+    ### echo "Directory /root/.gcp DOES NOT exists." 
+	cp -r .tmp/config/.gcp /root/.gcp
+fi
+
+if [ ! -d "/root/.oci" ]
+then
+    ### echo "Directory /root/.oci DOES NOT exists." 
+	cp -r .tmp/config/.oci /root/.oci
+fi
+
 if [ ! -d "/root/.thunder" ]
 then
     ### echo "Directory /root/.thunder DOES NOT exists." 
 	cp -r .tmp/config/.thunder /root/.thunder
 fi
 
 if [ ! -d "/var/log/thunder-observability-agent" ]
```

### Comparing `thunder-observability-agent-2.0.0/thunder-observability-agent/logging.conf` & `thunder_observability_agent-3.0.0/thunder-observability-agent/logging.conf`

 * *Files identical despite different names*

### Comparing `thunder-observability-agent-2.0.0/thunder-observability-agent/processor/log_processor.py` & `thunder_observability_agent-3.0.0/thunder-observability-agent/processor/log_processor.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 from handler.thunder_handler import ThunderHandler
 from handler.aws_handler import AWSHandler
 from handler.vmware_handler import VMWareHandler
 from handler.azure_handler import AzureHandler
 from handler.elasticsearch_handler import ElasticSearchHandler
 from handler.pushgateway_handler import PushGatewayHandler 
 from handler.splunk_handler import SplunkHandler
+from handler.gcp_handler import GCPHandler
+from handler.oci_handler import OCIHandler
 import concurrent.futures
 class LogProcessor:
     
     _logger = Logging().get_logger("LogProcessor")
     
     def process(self, thunder):
         if(Utils.is_valid(Utils._active_log_provider)):
@@ -33,14 +35,18 @@
                 self.process_vmware_log(thunder)
             elif Utils._active_log_provider==Constant._ES_LOG:
                 self.process_es_log(thunder)
             elif Utils._active_log_provider==Constant._PUSH_GATEWAY_LOG:
                 self.process_pushgateway_log(thunder)
             elif Utils._active_log_provider==Constant._SPLUNK_LOG:
                 self.process_splunk_log(thunder)
+            elif Utils._active_log_provider==Constant._GCP_LOG:
+                self.process_gcp_log(thunder)
+            elif Utils._active_log_provider==Constant._OCI_LOG:
+                self.process_oci_log(thunder)
             
     def process_aws_log(self, thunder):
         logs = self.collect_log(thunder)
         if(Utils.is_valid(logs)):
             handler = AWSHandler(thunder._thunder, Constant._AWS_BOTO3_SERVICE_LOGS)  
             handler.publish_log(logs)
        
@@ -69,14 +75,27 @@
             handler.publish_log(logs)
     
     def process_splunk_log(self,thunder):
         logs = self.collect_log(thunder)
         if(Utils.is_valid(logs)):
             handler = SplunkHandler(thunder._thunder)
             handler.publish_log(logs)
+    
+    def process_gcp_log(self, thunder): 
+        logs = self.collect_log(thunder)
+        if(Utils.is_valid(logs)):
+            handler = GCPHandler(thunder._thunder, None)
+            handler.token()
+            handler.publish_log(logs)
+    
+    def process_oci_log(self,thunder):
+        logs = self.collect_log(thunder)
+        if(Utils.is_valid(logs)):
+            handler = OCIHandler(thunder._thunder)
+            handler.publish_log(logs)
 
     def collect_log(self, thunder): 
         logs_data = []
         dates = thunder.dates()
         
         thunders = [ThunderHandler(metric=None, date=date, thunder=thunder._thunder, token=thunder._token, callback=None) for date in dates]
         with ThreadPoolExecutor(max_workers=int(Utils._main.get(Constant._THREADPOOL_MAX_WORKERS))) as collect:
```

### Comparing `thunder-observability-agent-2.0.0/thunder-observability-agent/processor/metric_processor.py` & `thunder_observability_agent-3.0.0/thunder-observability-agent/processor/metric_processor.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 from handler.thunder_handler import ThunderHandler
 from handler.aws_handler import AWSHandler
 from handler.vmware_handler import VMWareHandler
 from handler.azure_handler import AzureHandler
 from handler.elasticsearch_handler import ElasticSearchHandler
 from handler.pushgateway_handler import PushGatewayHandler 
 from handler.splunk_handler import SplunkHandler
+from handler.gcp_handler import GCPHandler
+from handler.oci_handler import OCIHandler
 from concurrent.futures import ThreadPoolExecutor
 
 class MetricProcessor:
     
     _logger = Logging().get_logger("MetricProcessor")
     _metric=None
     _type=None
@@ -42,14 +44,18 @@
                 self.process_vmware_metric(_thunder, thunder)
             elif Utils._active_metric_provider==Constant._ES_METRIC:
                 self.process_es_metric(_thunder, thunder)
             elif Utils._active_metric_provider==Constant._PUSH_GATEWAY_METRIC:
                 self.process_pushgateway_metric(_thunder, thunder)
             elif Utils._active_metric_provider==Constant._SPLUNK_METRIC:
                 self.process_splunk_metric(_thunder, thunder)
+            elif Utils._active_metric_provider==Constant._GCP_METRIC:
+                self.process_gcp_metric(_thunder, thunder)
+            elif Utils._active_metric_provider==Constant._OCI_METRIC:
+                self.process_oci_metric(_thunder,thunder)
 
     def process_aws_metric(self, _thunder, thunder):
         _metrics = self.collect_metric(_thunder, thunder, None)
         if(Utils.is_valid(_metrics)):
             AWSHandler(_thunder, Constant._AWS_BOTO3_SERVICE_CLOUDWATCH).publish_metric(_metrics)
        
     def process_vmware_metric(self, _thunder, thunder): 
@@ -77,14 +83,28 @@
             handler.publish_metric(_metrics)
             
     def process_splunk_metric(self, _thunder, thunder): 
         _metrics = self.collect_metric(_thunder, thunder, None)
         if(Utils.is_valid(_metrics)):
             handler = SplunkHandler(_thunder)
             handler.publish_metric(_metrics)
+
+    def process_gcp_metric(self, _thunder, thunder): 
+        _metrics = self.collect_metric(_thunder, thunder, None)
+        if(Utils.is_valid(_metrics)):
+            handler = GCPHandler(_thunder,None)
+            handler.token()
+            handler.publish_metric(_metrics)
+            
+    def process_oci_metric(self,_thunder,thunder):
+        _metrics = self.collect_metric(_thunder,thunder, None)
+        if(Utils.is_valid(_metrics)):
+            handler = OCIHandler(_thunder)
+            handler.publish_metric(_metrics)
+        
         
     def collect_metric(self, _thunder,  thunder, callback):
         metric_data = []
         thunders = [ThunderHandler(metric=metric, date=None, thunder=_thunder, token=thunder._token, callback=callback) for metric in self._metric]
         with ThreadPoolExecutor(max_workers=int(Utils._main.get(Constant._THREADPOOL_MAX_WORKERS))) as collect:
             futures = [collect.submit(thunder.collect_metric) for thunder in thunders]
             for future in concurrent.futures.as_completed(futures):
```

### Comparing `thunder-observability-agent-2.0.0/thunder-observability-agent/processor/partition_processor.py` & `thunder_observability_agent-3.0.0/thunder-observability-agent/processor/partition_processor.py`

 * *Files identical despite different names*

### Comparing `thunder-observability-agent-2.0.0/thunder-observability-agent/processor/thunder_processor.py` & `thunder_observability_agent-3.0.0/thunder-observability-agent/processor/thunder_processor.py`

 * *Files identical despite different names*

### Comparing `thunder-observability-agent-2.0.0/thunder-observability-agent/toa.py` & `thunder_observability_agent-3.0.0/thunder-observability-agent/toa.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 # Copyright 2023, A10 Networks Inc. All Rights Reserved.
 # THUNDER OBSERVABILITY AGENT END USER SOFTWARE LICENSE AGREEMENT
 """
 Configure and run thunder agent.
 To use, simply 'import Toa' and use it!
 """
 __author__ = 'Dinesh Kumar Lohia (DLohia@a10networks.com)'
-
+import time
 from common.toa_helper import Helper
 from common.toa_logging import Logging
 from common.toa_utils import Utils
 from common.toa_constant import Constant
 
 _logger = Logging().get_logger("main")
 
 if __name__ == "__main__":
-    _job_start_time = Utils._datetime
-    _logger.info(Constant._INFO_JOB_ID.format(str(Utils._datetime_id)))
-    _logger.info(Constant._INFO_JOB_START.format(str(_job_start_time)))
+    
+        _job_start_time = Utils._datetime
+        _logger.info(Constant._INFO_JOB_ID.format(str(Utils._datetime_id)))
+        _logger.info(Constant._INFO_JOB_START.format(str(_job_start_time)))
 
-    Helper.init()
+        Helper.init()
 
-    _job_end_time=Utils.date_time_utc()
-    _logger.info(Constant._INFO_JOB_TIME.format(( _job_end_time - _job_start_time).total_seconds()))
-    _logger.info(Constant._INFO_JOB_END.format(str(_job_end_time)))
-    _logger.info(Constant._DOCS)
-    _logger.info("##### TOA  ###### All Rights Reserved @A10 Networks Inc ##### TOA #####")
-    
-    
+        _job_end_time = Utils.date_time_utc()
+        _logger.info(Constant._INFO_JOB_TIME.format((_job_end_time - _job_start_time).total_seconds()))
+        _logger.info(Constant._INFO_JOB_END.format(str(_job_end_time)))
+        _logger.info(Constant._DOCS)
+        _logger.info("##### TOA  ###### All Rights Reserved @A10 Networks Inc ##### TOA #####")
+
```

### Comparing `thunder-observability-agent-2.0.0/thunder_observability_agent.egg-info/PKG-INFO` & `thunder_observability_agent-3.0.0/thunder_observability_agent.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,69 @@
 Metadata-Version: 2.1
 Name: thunder-observability-agent
-Version: 2.0.0
+Version: 3.0.0
 Summary: A10 Thunder Observability Agent is a lightweight autonomous data processing engine that can be externally installed and configured for multiple A10 Thunder Instances to collect, process and publish performance metrics and logs into multiple monitoring dashboard.
 Home-page: https://github.com/a10networks/thunder-observability-agent
-Author: Dinesh Kumar Lohia
-Author-email: dlohia@a10networks.com
+Author: A10 Networks
+Author-email: support@a10networks.com
 Maintainer: A10 Networks
 Maintainer-email: support@a10networks.com
 License: THUNDER OBSERVABILITY AGENT END USER SOFTWARE LICENSE AGREEMENT.
-Keywords: Python,A10Networks,Observability,Agent,Thunder,vThunder,cThunder,Thunder,AWS,Azure,Cloudwatch,VMware,Log,Insight,Application,App,Insight,Analytics,Dashboard,Monitoring,VROPS,VRLI,Operations,A10,Splunk,Prometheus,PushGateway,ElasticSearch,ACOS,A10
+Keywords: Python,A10Networks,Observability,Agent,Thunder,vThunder,cThunder,Thunder,AWS,Azure,Cloudwatch,VMware,Log,Insight,Application,App,Insight,Analytics,Dashboard,Monitoring,VROPS,VRLI,Operations,A10,Splunk,Prometheus,PushGateway,ElasticSearch,ACOS,A10,Google Cloud Platform (GCP),Oracle Cloud Infrastructure (OCI)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Requires-Dist: requests>=2.27.1
 Requires-Dist: boto3>=1.23.10
+Requires-Dist: google-auth>=2.22.0
+Requires-Dist: oci>=2.121.1
 
-# A10's Thunder Observability Agent (TOA) - v2.0.0
+# A10's Thunder Observability Agent (TOA) - v3.0.0
 	The TOA is a lightweight autonomous data processing engine that can be externally installed and configured for any Thunder device.
 	TOA offers the following capabilities on Application Delivery Controller (ADC):
 	
 	- Collects, processes and publishes Thunder metrics. 
 	  The default data collection frequency is 1 minute. 
-	  Thunder metrics can be sent to the platform where Thunder is deployed, which includes AWS, Azure, and VMware or can be sent to shared platforms like Elasticsearch (Kibana), Prometheus (Grafana), and Splunk. 
+	  Thunder metrics can be sent to the platform where Thunder is deployed, which includes AWS, Azure, VMware, Elasticsearch (Kibana), Prometheus (Grafana), and Splunkor can be sent to shared platforms like Google Cloud Platform(GCP), and Oracle Cloud Infrastructure(OCI) . 
 	  Metrics can be sent to any one platform at a time. For more information on Thunder metrics, see Supported Thunder Metrics.
 
 	
 	- Collects, processes, and publishes Thunder Syslogs. 
 	  The default data collection frequency is 1 minute. 
-	  The logs can be published on various platforms like AWS, Azure, VMware, Kibana (Elasticsearch), Grafana (Prometheus and Pushgateway), or Splunk. 
+	  The logs can be published on various platforms like AWS, Azure, VMware, Kibana (Elasticsearch), Grafana (Prometheus and Pushgateway), Splunk Google Cloud Platform(GCP), or Oracle Cloud Infrastructure(OCI). 
       Logs can be sent to any one platform at a time. For more information on Thunder logs, see Supported Thunder Logs.
 
     Supported Monitoring Platforms:
 	1. AWS.
 	2. Azure.
 	3. VMware.
 	4. Splunk
 	5. ElasticSearch-Kibana
 	6. Prometheus-Grafana [PushGateway]
+	7. Google Cloud Platform(GCP)
+	8. Oracle Cloud Infrastructure(OCI)
 
 	Supported Use Cases:
 	1. Monitoring thunder adc metrics or logs or both into AWS Cloudwatch.
 	2. Monitoring thunder adc metrics or logs or both into Azure Application Insight and Log Analytics Workspace.
 	3. Monitoring thunder adc metrics or logs or both into VMware vRealize Operations and Log Insight.
 	4. Monitoring thunder adc metrics or logs or both into Splunk Console.
 	5. Monitoring thunder adc metrics or logs or both into ElasticSearch/Kibana Console.
 	6. Monitoring thunder adc metrics or logs or both into Prometheus/Grafana Console using PushGateway.
+	7. Monitoring thunder adc metrics or logs or both into Google Cloud Platform (GCP).
+	8. Monitoring thunder adc metrics or logs or both into Oracle Cloud Infrastructure (OCI).
 	
 
 	Links:
 	License				: https://www.a10networks.com/wp-content/uploads/EULA_Thunder_Observability_Agent.pdf
-	Open Source (Notice)            : https://github.com/a10networks/thunder-observability-agent/tree/release/v2.0.0/OPEN-SOURCE-DISCLAIMER.pdf
+	Open Source (Notice)            : https://github.com/a10networks/thunder-observability-agent/tree/release/v3.0.0/OPEN-SOURCE-Notice.pdf
 	Documentation		        : https://documentation.a10networks.com/docs/Install/Software/thunder-observability-agent/
-	Repository			: https://github.com/a10networks/thunder-observability-agent/tree/release/v2.0.0
-	Example				: https://github.com/a10networks/thunder-observability-agent/tree/release/v2.0.0/examples
+	Repository			: https://github.com/a10networks/thunder-observability-agent/tree/release/v3.0.0
+	Example				: https://github.com/a10networks/thunder-observability-agent/tree/release/v3.0.0/examples
```

### Comparing `thunder-observability-agent-2.0.0/thunder_observability_agent.egg-info/SOURCES.txt` & `thunder_observability_agent-3.0.0/thunder_observability_agent.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 ./thunder-observability-agent/common/toa_constant.py
 ./thunder-observability-agent/common/toa_helper.py
 ./thunder-observability-agent/common/toa_logging.py
 ./thunder-observability-agent/common/toa_utils.py
 ./thunder-observability-agent/handler/aws_handler.py
 ./thunder-observability-agent/handler/azure_handler.py
 ./thunder-observability-agent/handler/elasticsearch_handler.py
+./thunder-observability-agent/handler/gcp_handler.py
+./thunder-observability-agent/handler/oci_handler.py
 ./thunder-observability-agent/handler/pushgateway_handler.py
 ./thunder-observability-agent/handler/splunk_handler.py
 ./thunder-observability-agent/handler/thunder_handler.py
 ./thunder-observability-agent/handler/vmware_handler.py
 ./thunder-observability-agent/processor/log_processor.py
 ./thunder-observability-agent/processor/metric_processor.py
 ./thunder-observability-agent/processor/partition_processor.py
@@ -28,11 +30,13 @@
 thunder-observability-agent/init.sh
 thunder-observability-agent/logging.conf
 thunder-observability-agent/main.properties
 thunder-observability-agent/config/.aws/config
 thunder-observability-agent/config/.aws/credentials
 thunder-observability-agent/config/.azure/credentials
 thunder-observability-agent/config/.elasticsearch/credentials
+thunder-observability-agent/config/.gcp/credentials
+thunder-observability-agent/config/.oci/credentials
 thunder-observability-agent/config/.pushgateway/credentials
 thunder-observability-agent/config/.splunk/credentials
 thunder-observability-agent/config/.thunder/credentials
 thunder-observability-agent/config/.vmware/credentials
```

