# Comparing `tmp/aws-glue-sessions-1.0.4.tar.gz` & `tmp/aws-glue-sessions-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-glue-sessions-1.0.4.tar", last modified: Sat Dec  2 00:07:54 2023, max compression
+gzip compressed data, was "aws-glue-sessions-1.0.5.tar", last modified: Tue Apr 23 19:26:17 2024, max compression
```

## Comparing `aws-glue-sessions-1.0.4.tar` & `aws-glue-sessions-1.0.5.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 szkart     (504) ANT\Domain Users (1896053708)        0 2023-12-02 00:07:54.816076 aws-glue-sessions-1.0.4/
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)    11358 2023-10-16 20:40:38.000000 aws-glue-sessions-1.0.4/LICENSE
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)       40 2023-10-13 21:40:28.000000 aws-glue-sessions-1.0.4/MANIFEST.in
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)     3199 2023-12-02 00:07:54.815767 aws-glue-sessions-1.0.4/PKG-INFO
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)     2371 2023-12-01 22:45:24.000000 aws-glue-sessions-1.0.4/README.md
-drwxr-xr-x   0 szkart     (504) ANT\Domain Users (1896053708)        0 2023-12-02 00:07:54.808690 aws-glue-sessions-1.0.4/configuration/
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)       77 2023-10-18 18:53:35.000000 aws-glue-sessions-1.0.4/configuration/entry_point.sh
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)       38 2023-12-02 00:07:54.816130 aws-glue-sessions-1.0.4/setup.cfg
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)     2116 2023-12-01 17:51:13.000000 aws-glue-sessions-1.0.4/setup.py
-drwxr-xr-x   0 szkart     (504) ANT\Domain Users (1896053708)        0 2023-12-02 00:07:54.807736 aws-glue-sessions-1.0.4/src/
-drwxr-xr-x   0 szkart     (504) ANT\Domain Users (1896053708)        0 2023-12-02 00:07:54.809331 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)       88 2023-08-16 00:03:29.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/__init__.py
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)     1929 2023-08-15 16:37:33.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_kernel.py
-drwxr-xr-x   0 szkart     (504) ANT\Domain Users (1896053708)        0 2023-12-02 00:07:54.809800 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_kernel_base/
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)    45458 2023-12-01 01:37:33.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_kernel_base/BaseKernel.py
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)        0 2023-08-15 16:37:33.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_kernel_base/__init__.py
-drwxr-xr-x   0 szkart     (504) ANT\Domain Users (1896053708)        0 2023-12-02 00:07:54.811013 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_kernel_configs/
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)     3154 2023-09-01 11:32:52.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_kernel_configs/AWSFileConfigRetriever.py
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)      193 2023-09-01 09:48:42.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_kernel_configs/ConfigRetriever.py
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)      351 2023-09-01 09:48:42.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_kernel_configs/DefaultConfigRetriever.py
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)      976 2023-09-01 09:48:42.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_kernel_configs/GlueConfigManager.py
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)      360 2023-09-01 09:48:42.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_kernel_configs/OverriddenConfigRetriever.py
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)     3446 2023-12-01 06:16:20.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_kernel_configs/SystemEnvConfigRetriever.py
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)        0 2023-09-01 09:48:42.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_kernel_configs/__init__.py
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)      983 2023-09-01 12:00:44.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_kernel_configs/config.py
-drwxr-xr-x   0 szkart     (504) ANT\Domain Users (1896053708)        0 2023-12-02 00:07:54.811931 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_kernel_utils/
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)    10395 2023-12-01 01:43:35.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_kernel_utils/GlueSessionsConstants.py
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)    14850 2023-09-01 11:32:52.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_kernel_utils/KernelGateway.py
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)    19403 2023-09-01 19:27:33.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_kernel_utils/KernelMagics.py
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)      647 2023-09-01 11:32:52.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_kernel_utils/ValidationUtils.py
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)        0 2023-08-15 16:37:33.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_kernel_utils/__init__.py
-drwxr-xr-x   0 szkart     (504) ANT\Domain Users (1896053708)        0 2023-12-02 00:07:54.812747 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_pyspark/
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)     2874 2023-09-01 11:32:52.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_pyspark/GlueKernel.py
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)        0 2023-08-15 16:37:33.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_pyspark/__init__.py
-drwxr-xr-x   0 szkart     (504) ANT\Domain Users (1896053708)        0 2023-12-02 00:07:54.807385 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_pyspark/glue/
-drwxr-xr-x   0 szkart     (504) ANT\Domain Users (1896053708)        0 2023-12-02 00:07:54.812897 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_pyspark/glue/2017-03-31/
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)   397673 2023-08-15 16:37:33.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_pyspark/glue/2017-03-31/service-2.json
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)      204 2023-08-15 16:37:33.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_pyspark/kernel.json
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)     3200 2023-08-15 16:37:33.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_pyspark/logo-128x128.png
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)      890 2023-08-15 16:37:33.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_pyspark/logo-32x32.png
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)     1727 2023-08-15 16:37:33.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_pyspark/logo-64x64.png
-drwxr-xr-x   0 szkart     (504) ANT\Domain Users (1896053708)        0 2023-12-02 00:07:54.813979 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_spark/
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)     1749 2023-09-01 15:03:35.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_spark/GlueKernel.py
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)        0 2023-08-15 16:37:33.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_spark/__init__.py
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)      199 2023-08-15 16:37:33.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_spark/kernel.json
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)     3200 2023-08-15 16:37:33.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_spark/logo-128x128.png
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)      890 2023-08-15 16:37:33.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_spark/logo-32x32.png
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)     1727 2023-08-15 16:37:33.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_spark/logo-64x64.png
--rwxr-xr-x   0 szkart     (504) ANT\Domain Users (1896053708)      925 2023-08-15 16:37:33.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/install.sh
-drwxr-xr-x   0 szkart     (504) ANT\Domain Users (1896053708)        0 2023-12-02 00:07:54.814414 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/logos/
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)     3200 2023-08-15 16:37:33.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/logos/logo-128x128.png
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)      890 2023-08-15 16:37:33.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/logos/logo-32x32.png
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)     1727 2023-08-15 16:37:33.000000 aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/logos/logo-64x64.png
-drwxr-xr-x   0 szkart     (504) ANT\Domain Users (1896053708)        0 2023-12-02 00:07:54.815250 aws-glue-sessions-1.0.4/src/aws_glue_sessions.egg-info/
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)     3199 2023-12-02 00:07:54.000000 aws-glue-sessions-1.0.4/src/aws_glue_sessions.egg-info/PKG-INFO
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)     2764 2023-12-02 00:07:54.000000 aws-glue-sessions-1.0.4/src/aws_glue_sessions.egg-info/SOURCES.txt
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)        1 2023-12-02 00:07:54.000000 aws-glue-sessions-1.0.4/src/aws_glue_sessions.egg-info/dependency_links.txt
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)       98 2023-12-02 00:07:54.000000 aws-glue-sessions-1.0.4/src/aws_glue_sessions.egg-info/entry_points.txt
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)      209 2023-12-02 00:07:54.000000 aws-glue-sessions-1.0.4/src/aws_glue_sessions.egg-info/requires.txt
--rw-r--r--   0 szkart     (504) ANT\Domain Users (1896053708)       37 2023-12-02 00:07:54.000000 aws-glue-sessions-1.0.4/src/aws_glue_sessions.egg-info/top_level.txt
+drwxr-xr-x   0 rnaiir     (504) staff       (20)        0 2024-04-23 19:26:17.409258 aws-glue-sessions-1.0.5/
+-rw-r--r--   0 rnaiir     (504) staff       (20)    11358 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/LICENSE
+-rw-r--r--   0 rnaiir     (504) staff       (20)       40 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/MANIFEST.in
+-rw-r--r--   0 rnaiir     (504) staff       (20)     3404 2024-04-23 19:26:17.408641 aws-glue-sessions-1.0.5/PKG-INFO
+-rw-r--r--   0 rnaiir     (504) staff       (20)     2576 2024-04-19 23:02:39.000000 aws-glue-sessions-1.0.5/README.md
+drwxr-xr-x   0 rnaiir     (504) staff       (20)        0 2024-04-23 19:26:17.377235 aws-glue-sessions-1.0.5/configuration/
+-rw-r--r--   0 rnaiir     (504) staff       (20)       77 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/configuration/entry_point.sh
+-rw-r--r--   0 rnaiir     (504) staff       (20)       38 2024-04-23 19:26:17.409396 aws-glue-sessions-1.0.5/setup.cfg
+-rw-r--r--   0 rnaiir     (504) staff       (20)     2116 2024-04-19 23:02:39.000000 aws-glue-sessions-1.0.5/setup.py
+drwxr-xr-x   0 rnaiir     (504) staff       (20)        0 2024-04-23 19:26:17.374420 aws-glue-sessions-1.0.5/src/
+drwxr-xr-x   0 rnaiir     (504) staff       (20)        0 2024-04-23 19:26:17.379436 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/
+-rw-r--r--   0 rnaiir     (504) staff       (20)       88 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/__init__.py
+-rw-r--r--   0 rnaiir     (504) staff       (20)     1929 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_kernel.py
+drwxr-xr-x   0 rnaiir     (504) staff       (20)        0 2024-04-23 19:26:17.381576 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_kernel_base/
+-rw-r--r--   0 rnaiir     (504) staff       (20)    47220 2024-04-23 17:40:29.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_kernel_base/BaseKernel.py
+-rw-r--r--   0 rnaiir     (504) staff       (20)        0 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_kernel_base/__init__.py
+drwxr-xr-x   0 rnaiir     (504) staff       (20)        0 2024-04-23 19:26:17.386279 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_kernel_configs/
+-rw-r--r--   0 rnaiir     (504) staff       (20)     3154 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_kernel_configs/AWSFileConfigRetriever.py
+-rw-r--r--   0 rnaiir     (504) staff       (20)      193 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_kernel_configs/ConfigRetriever.py
+-rw-r--r--   0 rnaiir     (504) staff       (20)      351 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_kernel_configs/DefaultConfigRetriever.py
+-rw-r--r--   0 rnaiir     (504) staff       (20)      976 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_kernel_configs/GlueConfigManager.py
+-rw-r--r--   0 rnaiir     (504) staff       (20)      360 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_kernel_configs/OverriddenConfigRetriever.py
+-rw-r--r--   0 rnaiir     (504) staff       (20)     3446 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_kernel_configs/SystemEnvConfigRetriever.py
+-rw-r--r--   0 rnaiir     (504) staff       (20)        0 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_kernel_configs/__init__.py
+-rw-r--r--   0 rnaiir     (504) staff       (20)     1011 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_kernel_configs/config.py
+drwxr-xr-x   0 rnaiir     (504) staff       (20)        0 2024-04-23 19:26:17.390788 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_kernel_utils/
+-rw-r--r--   0 rnaiir     (504) staff       (20)    11406 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_kernel_utils/GlueSessionsConstants.py
+-rw-r--r--   0 rnaiir     (504) staff       (20)    15471 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_kernel_utils/KernelGateway.py
+-rw-r--r--   0 rnaiir     (504) staff       (20)    20772 2024-04-19 23:02:39.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_kernel_utils/KernelMagics.py
+-rw-r--r--   0 rnaiir     (504) staff       (20)      647 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_kernel_utils/ValidationUtils.py
+-rw-r--r--   0 rnaiir     (504) staff       (20)        0 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_kernel_utils/__init__.py
+drwxr-xr-x   0 rnaiir     (504) staff       (20)        0 2024-04-23 19:26:17.395461 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_pyspark/
+-rw-r--r--   0 rnaiir     (504) staff       (20)     2874 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_pyspark/GlueKernel.py
+-rw-r--r--   0 rnaiir     (504) staff       (20)        0 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_pyspark/__init__.py
+drwxr-xr-x   0 rnaiir     (504) staff       (20)        0 2024-04-23 19:26:17.373602 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_pyspark/glue/
+drwxr-xr-x   0 rnaiir     (504) staff       (20)        0 2024-04-23 19:26:17.396268 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_pyspark/glue/2017-03-31/
+-rw-r--r--   0 rnaiir     (504) staff       (20)   387012 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_pyspark/glue/2017-03-31/service-2.json
+-rw-r--r--   0 rnaiir     (504) staff       (20)      204 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_pyspark/kernel.json
+-rw-r--r--   0 rnaiir     (504) staff       (20)     3200 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_pyspark/logo-128x128.png
+-rw-r--r--   0 rnaiir     (504) staff       (20)      890 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_pyspark/logo-32x32.png
+-rw-r--r--   0 rnaiir     (504) staff       (20)     1727 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_pyspark/logo-64x64.png
+drwxr-xr-x   0 rnaiir     (504) staff       (20)        0 2024-04-23 19:26:17.401548 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_spark/
+-rw-r--r--   0 rnaiir     (504) staff       (20)     1749 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_spark/GlueKernel.py
+-rw-r--r--   0 rnaiir     (504) staff       (20)        0 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_spark/__init__.py
+-rw-r--r--   0 rnaiir     (504) staff       (20)      199 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_spark/kernel.json
+-rw-r--r--   0 rnaiir     (504) staff       (20)     3200 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_spark/logo-128x128.png
+-rw-r--r--   0 rnaiir     (504) staff       (20)      890 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_spark/logo-32x32.png
+-rw-r--r--   0 rnaiir     (504) staff       (20)     1727 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_spark/logo-64x64.png
+-rwxr-xr-x   0 rnaiir     (504) staff       (20)      925 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/install.sh
+drwxr-xr-x   0 rnaiir     (504) staff       (20)        0 2024-04-23 19:26:17.403703 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/logos/
+-rw-r--r--   0 rnaiir     (504) staff       (20)     3200 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/logos/logo-128x128.png
+-rw-r--r--   0 rnaiir     (504) staff       (20)      890 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/logos/logo-32x32.png
+-rw-r--r--   0 rnaiir     (504) staff       (20)     1727 2024-04-19 20:20:15.000000 aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/logos/logo-64x64.png
+drwxr-xr-x   0 rnaiir     (504) staff       (20)        0 2024-04-23 19:26:17.407595 aws-glue-sessions-1.0.5/src/aws_glue_sessions.egg-info/
+-rw-r--r--   0 rnaiir     (504) staff       (20)     3404 2024-04-23 19:26:17.000000 aws-glue-sessions-1.0.5/src/aws_glue_sessions.egg-info/PKG-INFO
+-rw-r--r--   0 rnaiir     (504) staff       (20)     2764 2024-04-23 19:26:17.000000 aws-glue-sessions-1.0.5/src/aws_glue_sessions.egg-info/SOURCES.txt
+-rw-r--r--   0 rnaiir     (504) staff       (20)        1 2024-04-23 19:26:17.000000 aws-glue-sessions-1.0.5/src/aws_glue_sessions.egg-info/dependency_links.txt
+-rw-r--r--   0 rnaiir     (504) staff       (20)       98 2024-04-23 19:26:17.000000 aws-glue-sessions-1.0.5/src/aws_glue_sessions.egg-info/entry_points.txt
+-rw-r--r--   0 rnaiir     (504) staff       (20)      209 2024-04-23 19:26:17.000000 aws-glue-sessions-1.0.5/src/aws_glue_sessions.egg-info/requires.txt
+-rw-r--r--   0 rnaiir     (504) staff       (20)       37 2024-04-23 19:26:17.000000 aws-glue-sessions-1.0.5/src/aws_glue_sessions.egg-info/top_level.txt
```

### Comparing `aws-glue-sessions-1.0.4/LICENSE` & `aws-glue-sessions-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-glue-sessions-1.0.4/PKG-INFO` & `aws-glue-sessions-1.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-glue-sessions
-Version: 1.0.4
+Version: 1.0.5
 Summary: Glue Interactive Sessions Jupyter kernel that integrates almost anywhere Jupyter does including your favorite IDEs.
 Home-page: https://aws.amazon.com/glue/
 Author: Glue Development Team
 Author-email: glue-sessions-preview@amazon.com
 License: Apache 2.0 License
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -57,14 +57,19 @@
 ### Using the kernel via other IDEs
 
 You may also use this kernel via VSCode or other IDEs that support Jupyter kernels.
 To set up the Glue Interactive Sessions kernel for Visual Studio Code follow [these instructions](https://docs.aws.amazon.com/glue/latest/dg/interactive-sessions-vscode.html).
 
 
 ## ChangeLog
+### v1.0.5 (2024-04-19)
+
+* New magic %timeout for configuring 'Timeout' parameter for Session.
+* New magic %reconnect, Customers can use %reconnect <sessionId> and reconnect to any of their live Session.
+
 ### v1.0.4 (2023-12-01)
 
 Added support for inferring region from AWS_REGION environment variable.
 
 ### v1.0.3 (2023-11-15)
 
 Added support for handling special characters in owner tag.
```

### Comparing `aws-glue-sessions-1.0.4/README.md` & `aws-glue-sessions-1.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,19 @@
 ### Using the kernel via other IDEs
 
 You may also use this kernel via VSCode or other IDEs that support Jupyter kernels.
 To set up the Glue Interactive Sessions kernel for Visual Studio Code follow [these instructions](https://docs.aws.amazon.com/glue/latest/dg/interactive-sessions-vscode.html).
 
 
 ## ChangeLog
+### v1.0.5 (2024-04-19)
+
+* New magic %timeout for configuring 'Timeout' parameter for Session.
+* New magic %reconnect, Customers can use %reconnect <sessionId> and reconnect to any of their live Session.
+
 ### v1.0.4 (2023-12-01)
 
 Added support for inferring region from AWS_REGION environment variable.
 
 ### v1.0.3 (2023-11-15)
 
 Added support for handling special characters in owner tag.
```

### Comparing `aws-glue-sessions-1.0.4/setup.py` & `aws-glue-sessions-1.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="aws-glue-sessions",
-    version="1.0.4",
+    version="1.0.5",
     description="Glue Interactive Sessions Jupyter kernel that integrates almost anywhere Jupyter does including your favorite IDEs.",
     url="https://aws.amazon.com/glue/",
     author="Glue Development Team",
     author_email="glue-sessions-preview@amazon.com",
     license="Apache 2.0 License",
     # declare your packages
     packages=find_packages(where="src", exclude=("test",)),
```

### Comparing `aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_kernel.py` & `aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_kernel.py`

 * *Files identical despite different names*

### Comparing `aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_kernel_base/BaseKernel.py` & `aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_kernel_base/BaseKernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import ast
 import base64
 import json
+
 from ipykernel.ipkernel import IPythonKernel
 from IPython.display import publish_display_data
 import re
 
 from importlib_metadata import version
 import os
 import sys
 import uuid
 import requests
 import subprocess
 
+
 from aws_glue_interactive_sessions_kernel.glue_kernel_configs.AWSFileConfigRetriever import AWSFileConfigRetriever
 from aws_glue_interactive_sessions_kernel.glue_kernel_configs.DefaultConfigRetriever import DefaultConfigRetriever
 from aws_glue_interactive_sessions_kernel.glue_kernel_configs.GlueConfigManager import GlueConfigManager
 from aws_glue_interactive_sessions_kernel.glue_kernel_configs.OverriddenConfigRetriever import OverriddenConfigRetriever
 from aws_glue_interactive_sessions_kernel.glue_kernel_configs.SystemEnvConfigRetriever import SystemEnvConfigRetriever
 from aws_glue_interactive_sessions_kernel.glue_kernel_configs.config import Config, default_configs
 
@@ -245,15 +247,16 @@
             "max_capacity",
             "number_of_workers",
             "worker_type",
             "connections",
             "glue_version",
             "security_config",
             "idle_timeout",
-            "tags"
+            "tags",
+            "timeout"
         }
         try:
             configs = ast.literal_eval(configs_json)
             if "profile" in configs:
                 self.set_profile(configs.get("profile"))
             if "endpoint" in configs:
                 self.set_endpoint_url(configs.get("endpoint"))
@@ -275,14 +278,16 @@
                 self.set_connections(configs.get("connections"))
             if "security_config" in configs:
                 self.set_security_config(configs.get("security_config"))
             if "glue_version" in configs:
                 self.set_glue_version(configs.get("glue_version"))
             if "idle_timeout" in configs:
                 self.set_idle_timeout(configs.get("idle_timeout"))
+            if "timeout" in configs:
+                self.set_timeout(configs.get("timeout"))
             if "tags" in configs:
                 self.add_tag_to_resource(configs.get("tags"))
             for arg, val in configs.items():
                 if arg not in kernel_managed_params:
                     self.add_default_argument(arg, val)
         except Exception as e:
             sys.stderr.write(
@@ -514,14 +519,20 @@
 
     def get_idle_timeout(self):
         return self.config_manager.get_config_by_priority(IDLE_TIMEOUT)
 
     def set_idle_timeout(self, idle_timeout):
         setattr(self.overrides, IDLE_TIMEOUT, idle_timeout)
 
+    def get_timeout(self):
+        return self.config_manager.get_config_by_priority(TIMEOUT)
+
+    def set_timeout(self, timeout):
+        setattr(self.overrides, TIMEOUT, timeout)
+
     def set_spark_conf(self, conf):
         setattr(self.overrides, SPARK_CONF, conf)
 
     def get_spark_conf(self):
         return self.config_manager.get_config_by_priority(SPARK_CONF)
 
     # TODO: Migrate ray configs using config priority.
@@ -548,15 +559,14 @@
             return f"{prefix}-{custom_id}"
         else:
             if not custom_id:
                 return f"{uuid.uuid4()}"
             return custom_id
 
     def create_session(self):
-
         glue_role_arn = self.get_glue_role_arn()
         if not glue_role_arn:
             glue_arn_from_sts = self.kernel_gateway.get_iam_role_using_sts(self.get_profile(), self.get_region())
             if glue_arn_from_sts:
                 self.set_glue_role_arn(glue_arn_from_sts)
             else:
                 raise ValueError('Glue Role ARN not provided')
@@ -576,30 +586,27 @@
         try:
             session_type = self._convert_to_pretty_name(self.get_session_type())
             session_type_enum = SessionType[session_type]
             self._send_output(f"Session Type: {self.get_session_type()}")
         except KeyError:
             raise ValueError(f"Unsupported session type {self.get_session_type()}")
 
-        # If the customer hasn't provided both number of workers and max_capacity, then use the default value.
-        if not self.get_max_capacity() and not self.get_number_of_workers() :
-            #Both max capacity and number of workers are not provided by the customers.
-            #Using the default values from the session type enum.
-            self.set_number_of_workers(session_type_enum.default_number_of_workers())
-
-        # If the customer hasn't provided both max_capacity and worker type, then use the default worker type.
-        if not self.get_max_capacity() and not self.get_worker_type():
-            self.set_worker_type(session_type_enum.default_worker_type())
-
         # Print Max Capacity if it is set. Else print Number of Workers and Worker Type
         if self.get_max_capacity():
             self._send_output(f"Max Capacity: {self.get_max_capacity()}")
         else:
-            self._send_output(f"Worker Type: {self.get_worker_type()}")
-            self._send_output(f"Number of Workers: {self.get_number_of_workers()}")
+            if self.get_worker_type():
+                self._send_output(f"Worker Type: {self.get_worker_type()}")
+            if self.get_number_of_workers():
+                self._send_output(f"Number of Workers: {self.get_number_of_workers()}")
+
+        if self.get_idle_timeout():
+            self._send_output(f"Idle Timeout: {self.get_idle_timeout()}")
+        if self.get_timeout():
+            self._send_output(f"Timeout: {self.get_timeout()}")
 
         self._send_output(f"Session ID: {self.get_new_session_id()}")
 
         additional_args = self._get_additional_arguments()
 
         response = self.kernel_gateway.create_session(
             self.get_glue_role_arn(),
@@ -647,14 +654,16 @@
             additional_args["NumberOfWorkers"] = int(self.get_number_of_workers())
         if self.get_worker_type():
             additional_args["WorkerType"] = self.get_worker_type()
         if self.get_security_config():
             additional_args["SecurityConfiguration"] = self.get_security_config()
         if self.get_idle_timeout():
             additional_args["IdleTimeout"] = int(self.get_idle_timeout())
+        if self.get_timeout():
+            additional_args["Timeout"] = int(self.get_timeout())
         if self.get_connections():
             additional_args["Connections"] = {"Connections" : list(self.get_connections().split(","))}
         if self.get_glue_version():
             additional_args["GlueVersion"] = self.get_glue_version()
         if self.get_request_origin():
             additional_args["RequestOrigin"] = self.get_request_origin()
 
@@ -951,14 +960,42 @@
 
     def reset_kernel(self):
         self.set_session_id(None)
         self.set_new_session_id(None)
         self.execution_counter = 1
         self.kernel_gateway = KernelGateway(self.ipython_display)
 
+    def switch_session(self, session_id):
+        if session_id == self.get_session_id():
+            self._send_output(f'Session: {session_id} is already active.')
+            return
+        self.kernel_gateway.initialize_clients(profile=self.get_profile(), region=self.get_region(), endpoint_url=self.get_endpoint_url(), temp_credentials=self.get_temp_credentials())
+        session = None
+        try:
+            session = self.kernel_gateway.get_session(session_id)['Session']
+        except Exception as e:
+            error_code = e.response['Error']['Code']
+            error_message = e.response['Error']['Message']
+            if error_code in 'EntityNotFoundException':
+                self._send_output(Colour.Red + Colour.Bold + f"Exception encountered while retrieving session: {error_message}"
+                                                             f" Please make sure the session exists for the account in the configured region.")
+                return
+            else:
+                self._send_output(Colour.Red + Colour.Bold + f"Exception encountered while retrieving session: {error_message} \n")
+                return
+        if session is None or session['Status'] in UNHEALTHY_SESSION_STATUS:
+            self._send_output(Colour.Red + Colour.Bold + f'Failed to switch, Session: {session_id} is not in {READY_SESSION_STATUS} state.')
+            return
+        # Not printing statement history, once we have customer feedback on whether we should have it & how, implement
+        # statements = self.kernel_gateway.list_statements(session_id)
+        self.set_session_id(session_id)
+        self.set_new_session_id(None)
+        self._send_output(f'Switched to Session: {session_id}.')
+        self.execution_counter = 1
+
     # https://github.com/ipython/ipykernel/issues/795
     # Redirect logs to only print in terminal
 
     def _setup_terminal_logging(self):
         for std, __std__ in [
             (sys.stdout, sys.__stdout__),
             (sys.stderr, sys.__stderr__),
```

### Comparing `aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_kernel_configs/AWSFileConfigRetriever.py` & `aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_kernel_configs/AWSFileConfigRetriever.py`

 * *Files identical despite different names*

### Comparing `aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_kernel_configs/GlueConfigManager.py` & `aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_kernel_configs/GlueConfigManager.py`

 * *Files identical despite different names*

### Comparing `aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_kernel_configs/SystemEnvConfigRetriever.py` & `aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_kernel_configs/SystemEnvConfigRetriever.py`

 * *Files identical despite different names*

### Comparing `aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_kernel_configs/config.py` & `aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_kernel_configs/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,12 +20,13 @@
         self.additional_python_modules = None
         self.extra_py_files = None
         self.enable_data_catalog = None
         self.extra_jars = None
         self.spark_conf = None
         self.session_type = None
         self.temp_credentials = None
+        self.timeout = None
 
 
 default_configs = Config()
 default_configs.session_type = SessionType.etl.pretty_name()
 default_configs.glue_version = "4.0"
```

### Comparing `aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_kernel_utils/GlueSessionsConstants.py` & `aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_kernel_utils/GlueSessionsConstants.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,40 +22,33 @@
     ImagePng = ("image/png")
     S3URI = ("text/uri-list")
 
 # Symbols for referencing session types
 @unique
 class SessionType(Enum):
 
-    def __new__(cls, value, pretty_name, python_version , default_number_of_workers, default_worker_type):
+    def __new__(cls, value, pretty_name, python_version):
         obj = object.__new__(cls)
         obj._value_ = value
         obj._pretty_name = pretty_name
         obj._python_version = python_version
-        obj._default_number_of_workers = default_number_of_workers
-        obj._default_worker_type = default_worker_type
         return obj
 
-    etl = ("glueetl", 'etl',  "3", "5", "G.1X")
-    streaming = ("gluestreaming", 'streaming', "3", "5", "G.1X")
-    glue_ray = ("glueray", 'glue_ray', "3.9", "5", "Z.2X")
+    etl = ("glueetl", 'etl',  "3")
+    streaming = ("gluestreaming", 'streaming', "3")
+    glue_ray = ("glueray", 'glue_ray', "3.9")
 
     def python_version(self):
         return self._python_version
 
     def session_type(self):
         return self._value_
 
     def pretty_name(self):
         return self._pretty_name
-    def default_number_of_workers(self):
-        return self._default_number_of_workers
-
-    def default_worker_type(self):
-        return self._default_worker_type
 
 
 WAIT_TIME = 1
 
 READY_SESSION_STATUS = "READY"
 PROVISIONING_SESSION_STATUS = "PROVISIONING"
 NOT_FOUND_SESSION_STATUS = "NOT_FOUND"
@@ -113,25 +106,28 @@
     %help                             Return a list of descriptions and input types for all magic commands. 
     %profile            String        Specify a profile in your aws configuration to use as the credentials provider.
     %region             String        Specify the AWS region in which to initialize a session. 
                                       Default from ~/.aws/config on Linux or macOS, 
                                       or C:\\Users\\ USERNAME \\.aws\\config" on Windows.
     %idle_timeout       Int           The number of minutes of inactivity after which a session will timeout. 
                                       Default: 2880 minutes (48 hours).
+    %timeout            Int           The number of minutes after which a session will timeout. 
+                                      Default: 2880 minutes (48 hours).
     %session_id_prefix  String        Define a String that will precede all session IDs in the format 
                                       [session_id_prefix]-[session_id]. If a session ID is not provided,
                                       a random UUID will be generated.
     %status                           Returns the status of the current Glue session including its duration, 
                                       configuration and executing user / role.
-    %session_id                       Returns the session ID for the running session. 
+    %session_id                       Returns the session ID for the running session.
     %list_sessions                    Lists all currently running sessions by ID.
     %stop_session                     Stops the current session.
     %glue_version       String        The version of Glue to be used by this session. 
                                       Currently, the only valid options are 2.0, 3.0 and 4.0. 
                                       Default: 2.0.
+    %reconnect          String        Specify a live session ID to switch/reconnect to the sessions.
 ----
 
 ## Selecting Session Types
 
 ----
     %streaming          String        Sets the session type to Glue Streaming.
     %etl                String        Sets the session type to Glue ETL.
@@ -195,14 +191,34 @@
 
 ## Action Magic
 
 ----
 
     %%sql               String        Run SQL code. All lines after the initial %%sql magic will be passed
                                       as part of the SQL code.  
+    %matplot      Matplotlib figure   Visualize your data using the matplotlib library.
+                                      E.g. 
+                                      import matplotlib.pyplot as plt
+                                      # Set X-axis and Y-axis values
+                                      x = [5, 2, 8, 4, 9]
+                                      y = [10, 4, 8, 5, 2]
+                                      # Create a bar chart 
+                                      plt.bar(x, y) 
+                                      # Show the plot
+                                      %matplot plt    
+    %plotly            Plotly figure  Visualize your data using the plotly library.
+                                      E.g.
+                                      import plotly.express as px
+                                      #Create a graphical figure
+                                      fig = px.line(x=["a","b","c"], y=[1,3,2], title="sample figure")
+                                      #Show the figure
+                                      %plotly fig
+
+  
+                
 ----
 
 '''
 
 OWNER_TAG = "owner"
 GLUE_STUDIO_NOTEBOOK_IDENTIFIER = "GlueStudioNotebook"
 SAGEMAKER_STUDIO_NOTEBOOK_IDENTIFIERS = ['SageMakerStudioPySparkNotebook', 'SageMakerStudioSparkNotebook']
@@ -234,14 +250,15 @@
 MAX_CAPACITY = "max_capacity"
 WORKER_TYPE = "worker_type"
 SECURITY_CONFIG = "security_config"
 SESSION_TYPE = "session_type"
 SPARK_CONF = "spark_conf"
 TAGS = "tags"
 TEMP_CREDENTIALS = "temp_credentials"
+TIMEOUT = "timeout"
 
 REMAP_DEFAULT_ARGUMENTS = {
     "min_workers": "auto-scaling-ray-min-workers",
     "object_memory_head": "object_store_memory_head",
     "object_memory_worker": "object_store_memory_worker"
 }
```

### Comparing `aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_kernel_utils/KernelGateway.py` & `aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_kernel_utils/KernelGateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,14 +204,27 @@
                 if error_code in ('InternalServiceException', 'OperationTimeoutException'):
                     time.sleep(i * self.min_retry_time)
                     continue
                 else:
                     raise
         raise RuntimeError('Error while getting list of session')
 
+    def list_statements(self, session_id):
+        for i in range(1, self.max_tries + 1):
+            try:
+                return self.glue_client.list_statements(SessionId=session_id)
+            except botocore.exceptions.ClientError as e:
+                error_code = e.response['Error']['Code']
+                if error_code in ('InternalServiceException', 'OperationTimeoutException'):
+                    time.sleep(i * self.min_retry_time)
+                    continue
+                else:
+                    raise
+        raise RuntimeError(f'Error while getting list of statements for session: {session_id}')
+
     def get_tags(self, resource_arn):
         for i in range(1, self.max_tries + 1):
             try:
                 return self.glue_client.get_tags(ResourceArn=resource_arn).get("Tags")
             except botocore.exceptions.ClientError as e:
                 error_code = e.response['Error']['Code']
                 if error_code in ('InternalServiceException', 'OperationTimeoutException'):
```

### Comparing `aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_kernel_utils/KernelMagics.py` & `aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_kernel_utils/KernelMagics.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,50 +30,67 @@
     def set_idle_timeout(self, idle_timeout=2880):
         self._validate_magic()
         idle_timeout = self._strip_quotes(idle_timeout)
         self.kernel._send_output(f'Current idle_timeout is {self.kernel.get_idle_timeout()} minutes.')
         self.kernel.set_idle_timeout(int(idle_timeout))
         self.kernel._send_output(f'idle_timeout has been set to {self.kernel.get_idle_timeout()} minutes.')
 
+    @line_magic('timeout')
+    def set_timeout(self, timeout=2880):
+        self._validate_magic()
+        timeout = self._strip_quotes(timeout)
+        self.kernel._send_output(f'Current timeout is {self.kernel.get_timeout()} minutes.')
+        self.kernel.set_timeout(int(timeout))
+        self.kernel._send_output(f'timeout has been set to {self.kernel.get_timeout()} minutes.')
+
     @line_magic('profile')
     def set_profile(self, profile):
         self._validate_magic()
         profile = self._strip_quotes(profile)
         self.kernel._send_output(f'Previous profile: {self.kernel.get_profile()}')
         self.kernel._send_output(f'Setting new profile to: {profile}')
         self.kernel.set_profile(profile)
 
     @line_magic('status')
     def get_status(self, line=None):
         if not self.kernel.get_session_id():
             self.kernel._send_output('There is no current session.')
             return
+        session = self.kernel.get_current_session()
         status = self.kernel.get_current_session_status()
         role = self.kernel.get_current_session_role()
-        session_id = self.kernel.get_current_session()['Id']
-        created_on = self.kernel.get_current_session()['CreatedOn']
-        glue_version = self.kernel.get_current_session()['GlueVersion']
-        session_type = self.kernel.get_session_type()
+        session_id = session['Id']
+        created_on = session['CreatedOn']
+        glue_version = session['GlueVersion']
+        if session['Command']:
+            session_type = session['Command']['Name']
         tags, exception_error = self.kernel.get_tags_from_resource()
         self.kernel._send_output(f'Session ID: {session_id}')
         self.kernel._send_output(f'Status: {status}')
         self.kernel._send_output(f'Role: {role}')
         self.kernel._send_output(f'CreatedOn: {created_on}')
         self.kernel._send_output(f'GlueVersion: {glue_version}')
         self.kernel._send_output(f'Session Type: {session_type}')
+        self.kernel._send_output(f"Idle Timeout: {session['IdleTimeout']}")
+        if 'Timeout' in session:
+            self.kernel._send_output(f"Timeout: {session['Timeout']}")
+        # Uncomment after introducing Timeout in GetSessionResponse
+        # self.kernel._send_output(f"Timeout: {session['Timeout']}")
         if exception_error:
             self.kernel._send_output(exception_error)
         else:
             self.kernel._send_output(f'Tags: {tags}')
         # Print Max Capacity if it is set. Else print Number of Workers and Worker Type
         if self.kernel.get_max_capacity():
-            self.kernel._send_output(f"Max Capacity: {self.kernel.get_max_capacity()}")
+            self.kernel._send_output(f"Max Capacity: {session['MaxCapacity']}")
         else:
-            self.kernel._send_output(f"Worker Type: {self.kernel.get_worker_type()}")
-            self.kernel._send_output(f"Number of Workers: {self.kernel.get_number_of_workers()}")
+            if session['WorkerType']:
+                self.kernel._send_output(f"Worker Type: {session['WorkerType']}")
+            if session['NumberOfWorkers']:
+                self.kernel._send_output(f"Number of Workers: {session['NumberOfWorkers']}")
         self.kernel._send_output(f'Region: {self.kernel.get_region()}')
         if self.kernel.get_connections():
             connections = self.kernel.get_connections()
             self.kernel._send_output(f"Connections: {connections}")
         default_arguments = self.kernel.get_default_arguments()
         args_list = [str(f"{k}: {v}") for k,v in default_arguments.items()]
         self.kernel._send_output(f"Arguments Passed: {args_list}")
@@ -108,14 +125,25 @@
     @line_magic('session_id')
     def set_session_id(self, line=None):
         if not self.kernel.get_session_id():
             self.kernel._send_output('There is no current session.')
         else:
             self.kernel._send_output(f'Current active Session ID: {self.kernel.get_session_id()}')
 
+    @line_magic('reconnect')
+    def reconnect_session(self, session_id):
+        self._strip_quotes(session_id)
+        if session_id:
+            self.kernel._send_output(f'Trying to switch to Session: {session_id}')
+            self.kernel._send_output(Colour.LightYellow + Colour.Bold + f'NOTE: Switching to a live session will not terminate the current session.' + Colour.Reset)
+            self.kernel.switch_session(session_id)
+        else:
+            self._send_output(Colour.Red + Colour.Bold + f'Invalid input, Session Id: {session_id}.')
+            self.kernel._send_output(f'Current active Session ID: {self.kernel.get_session_id()}')
+
     @line_magic('session_id_prefix')
     def set_session_id_prefix(self, line=None):
         formatted_line = self._strip_quotes(line)
         if not self._validate_prefix(formatted_line):
             self.kernel._send_output(f'Not a valid input, the prefix only accepts -._#/A-Za-z0-9')
         else:
             self.kernel.set_session_id_prefix(formatted_line)
@@ -332,16 +360,15 @@
                     exception_error = self.kernel.add_tags_to_resource_ready_state(valid_tags)
                     if exception_error:
                         self.kernel._send_output(exception_error)
                         return
                     self.kernel.add_tag_to_resource(valid_tags)
                 self.kernel._send_output(f'Tag {valid_tags} added')
             except Exception:
-                tags = {"tag_key1": "tag_value1", 'tag_key2': 'tag_value2'}
-                self.kernel._send_error_output(f"Please provide magics like {json.dumps(tags)}")
+                self.kernel.handle_exception(Exception(f'Please provide magics like {{"tag_key":"tag_value"}} : {cell}'))
         return
 
     @cell_magic('assume_role')
     def assume_role_for_cross_account(self, line=None, cell=None):
         self._validate_magic()
         if cell:
             cell = ast.literal_eval(cell)
```

### Comparing `aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_kernel_utils/ValidationUtils.py` & `aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_kernel_utils/ValidationUtils.py`

 * *Files identical despite different names*

### Comparing `aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_pyspark/GlueKernel.py` & `aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_pyspark/GlueKernel.py`

 * *Files identical despite different names*

### Comparing `aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_pyspark/glue/2017-03-31/service-2.json` & `aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_pyspark/glue/2017-03-31/service-2.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9444055221641623%*

 * *Differences: {"'operations'": "{'BatchGetPartition': {'errors': {insert: [(6, OrderedDict([('shape', "*

 * *                 "'FederationSourceRetryableException')]))]}}, 'DeleteCrawler': {'errors': "*

 * *                 "{insert: [(4, OrderedDict([('shape', 'InvalidInputException')]))]}}, "*

 * *                 "'DeleteJob': {'errors': {insert: [(3, OrderedDict([('shape', "*

 * *                 "'AccessDeniedException')]))]}}, 'GetBlueprintRun': {'errors': {insert: [(0, "*

 * *                 "OrderedDict([('shape', 'InvalidInputException […]*

```diff
@@ -7,42 +7,14 @@
         "serviceFullName": "glue",
         "serviceId": "Glue",
         "signatureVersion": "v4",
         "targetPrefix": "AWSGlue",
         "uid": "glue-2017-03-31"
     },
     "operations": {
-        "BatchCreateLineageNodes": {
-            "documentation": "Persists the lineage graph represented in the input.",
-            "errors": [
-                {
-                    "shape": "InternalServiceException"
-                },
-                {
-                    "shape": "InvalidInputException"
-                },
-                {
-                    "shape": "OperationTimeoutException"
-                },
-                {
-                    "shape": "ConcurrentModificationException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "BatchCreateLineageNodesRequest"
-            },
-            "name": "BatchCreateLineageNodes",
-            "output": {
-                "shape": "BatchCreateLineageNodesResponse"
-            }
-        },
         "BatchCreatePartition": {
             "errors": [
                 {
                     "shape": "InvalidInputException"
                 },
                 {
                     "shape": "AlreadyExistsException"
@@ -191,42 +163,14 @@
                 "shape": "BatchDeleteTableVersionRequest"
             },
             "name": "BatchDeleteTableVersion",
             "output": {
                 "shape": "BatchDeleteTableVersionResponse"
             }
         },
-        "BatchGetBlueprintInstances": {
-            "errors": [
-                {
-                    "shape": "EntityNotFoundException"
-                },
-                {
-                    "shape": "InternalServiceException"
-                },
-                {
-                    "shape": "OperationTimeoutException"
-                },
-                {
-                    "shape": "InvalidInputException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "BatchGetBlueprintInstancesRequest"
-            },
-            "internalonly": true,
-            "name": "BatchGetBlueprintInstances",
-            "output": {
-                "shape": "BatchGetBlueprintInstancesResponse"
-            }
-        },
         "BatchGetBlueprints": {
             "errors": [
                 {
                     "shape": "InternalServiceException"
                 },
                 {
                     "shape": "OperationTimeoutException"
@@ -243,41 +187,14 @@
                 "shape": "BatchGetBlueprintsRequest"
             },
             "name": "BatchGetBlueprints",
             "output": {
                 "shape": "BatchGetBlueprintsResponse"
             }
         },
-        "BatchGetColumnStatisticsForTable": {
-            "errors": [
-                {
-                    "shape": "InvalidInputException"
-                },
-                {
-                    "shape": "InternalServiceException"
-                },
-                {
-                    "shape": "OperationTimeoutException"
-                },
-                {
-                    "shape": "GlueEncryptionException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "BatchGetColumnStatisticsForTableRequest"
-            },
-            "name": "BatchGetColumnStatisticsForTable",
-            "output": {
-                "shape": "BatchGetColumnStatisticsForTableResponse"
-            }
-        },
         "BatchGetCrawlers": {
             "errors": [
                 {
                     "shape": "OperationTimeoutException"
                 },
                 {
                     "shape": "InvalidInputException"
@@ -366,51 +283,14 @@
                 "shape": "BatchGetDevEndpointsRequest"
             },
             "name": "BatchGetDevEndpoints",
             "output": {
                 "shape": "BatchGetDevEndpointsResponse"
             }
         },
-        "BatchGetInternalUnfilteredTable": {
-            "errors": [
-                {
-                    "shape": "EntityNotFoundException"
-                },
-                {
-                    "shape": "InvalidInputException"
-                },
-                {
-                    "shape": "InternalServiceException"
-                },
-                {
-                    "shape": "OperationTimeoutException"
-                },
-                {
-                    "shape": "GlueEncryptionException"
-                },
-                {
-                    "shape": "ResourceNotReadyException"
-                },
-                {
-                    "shape": "FederationSourceException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "BatchGetInternalUnfilteredTableRequest"
-            },
-            "internalonly": true,
-            "name": "BatchGetInternalUnfilteredTable",
-            "output": {
-                "shape": "BatchGetInternalUnfilteredTableResponse"
-            }
-        },
         "BatchGetJobs": {
             "errors": [
                 {
                     "shape": "InternalServiceException"
                 },
                 {
                     "shape": "OperationTimeoutException"
@@ -427,39 +307,14 @@
                 "shape": "BatchGetJobsRequest"
             },
             "name": "BatchGetJobs",
             "output": {
                 "shape": "BatchGetJobsResponse"
             }
         },
-        "BatchGetMLTransform": {
-            "errors": [
-                {
-                    "shape": "InvalidInputException"
-                },
-                {
-                    "shape": "OperationTimeoutException"
-                },
-                {
-                    "shape": "InternalServiceException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "BatchGetMLTransformRequest"
-            },
-            "internalonly": true,
-            "name": "BatchGetMLTransform",
-            "output": {
-                "shape": "BatchGetMLTransformResponse"
-            }
-        },
         "BatchGetPartition": {
             "errors": [
                 {
                     "shape": "InvalidInputException"
                 },
                 {
                     "shape": "EntityNotFoundException"
@@ -471,59 +326,59 @@
                     "shape": "InternalServiceException"
                 },
                 {
                     "shape": "GlueEncryptionException"
                 },
                 {
                     "shape": "FederationSourceException"
+                },
+                {
+                    "shape": "FederationSourceRetryableException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "BatchGetPartitionRequest"
             },
             "name": "BatchGetPartition",
             "output": {
                 "shape": "BatchGetPartitionResponse"
             }
         },
-        "BatchGetTable": {
+        "BatchGetTableOptimizer": {
             "errors": [
                 {
                     "shape": "EntityNotFoundException"
                 },
                 {
                     "shape": "InvalidInputException"
                 },
                 {
-                    "shape": "OperationTimeoutException"
+                    "shape": "AccessDeniedException"
                 },
                 {
                     "shape": "InternalServiceException"
                 },
                 {
-                    "shape": "GlueEncryptionException"
-                },
-                {
-                    "shape": "FederationSourceException"
+                    "shape": "ThrottlingException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
-                "shape": "BatchGetTableRequest"
+                "shape": "BatchGetTableOptimizerRequest"
             },
-            "name": "BatchGetTable",
+            "name": "BatchGetTableOptimizer",
             "output": {
-                "shape": "BatchGetTableResponse"
+                "shape": "BatchGetTableOptimizerResponse"
             }
         },
         "BatchGetTriggers": {
             "errors": [
                 {
                     "shape": "InternalServiceException"
                 },
@@ -788,54 +643,14 @@
                 "shape": "CreateBlueprintRequest"
             },
             "name": "CreateBlueprint",
             "output": {
                 "shape": "CreateBlueprintResponse"
             }
         },
-        "CreateBlueprintInstance": {
-            "errors": [
-                {
-                    "shape": "AccessDeniedException"
-                },
-                {
-                    "shape": "AlreadyExistsException"
-                },
-                {
-                    "shape": "InvalidInputException"
-                },
-                {
-                    "shape": "OperationTimeoutException"
-                },
-                {
-                    "shape": "InternalServiceException"
-                },
-                {
-                    "shape": "ResourceNumberLimitExceededException"
-                },
-                {
-                    "shape": "EntityNotFoundException"
-                },
-                {
-                    "shape": "IllegalBlueprintStateException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "CreateBlueprintInstanceRequest"
-            },
-            "internalonly": true,
-            "name": "CreateBlueprintInstance",
-            "output": {
-                "shape": "CreateBlueprintInstanceResponse"
-            }
-        },
         "CreateClassifier": {
             "errors": [
                 {
                     "shape": "AccessDeniedException"
                 },
                 {
                     "shape": "AlreadyExistsException"
@@ -1060,47 +875,14 @@
                 "shape": "CreateDevEndpointRequest"
             },
             "name": "CreateDevEndpoint",
             "output": {
                 "shape": "CreateDevEndpointResponse"
             }
         },
-        "CreateFederationProfile": {
-            "errors": [
-                {
-                    "shape": "AlreadyExistsException"
-                },
-                {
-                    "shape": "InvalidInputException"
-                },
-                {
-                    "shape": "ResourceNumberLimitExceededException"
-                },
-                {
-                    "shape": "InternalServiceException"
-                },
-                {
-                    "shape": "GlueEncryptionException"
-                },
-                {
-                    "shape": "OperationTimeoutException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "CreateFederationProfileRequest"
-            },
-            "name": "CreateFederationProfile",
-            "output": {
-                "shape": "CreateFederationProfileResponse"
-            }
-        },
         "CreateJob": {
             "errors": [
                 {
                     "shape": "InvalidInputException"
                 },
                 {
                     "shape": "IdempotentParameterMismatchException"
@@ -1484,14 +1266,50 @@
                 "shape": "CreateTableRequest"
             },
             "name": "CreateTable",
             "output": {
                 "shape": "CreateTableResponse"
             }
         },
+        "CreateTableOptimizer": {
+            "errors": [
+                {
+                    "shape": "EntityNotFoundException"
+                },
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "InvalidInputException"
+                },
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "AlreadyExistsException"
+                },
+                {
+                    "shape": "InternalServiceException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "CreateTableOptimizerRequest"
+            },
+            "name": "CreateTableOptimizer",
+            "output": {
+                "shape": "CreateTableOptimizerResponse"
+            }
+        },
         "CreateTrigger": {
             "errors": [
                 {
                     "shape": "AccessDeniedException"
                 },
                 {
                     "shape": "AlreadyExistsException"
@@ -1526,14 +1344,47 @@
                 "shape": "CreateTriggerRequest"
             },
             "name": "CreateTrigger",
             "output": {
                 "shape": "CreateTriggerResponse"
             }
         },
+        "CreateUsageProfile": {
+            "errors": [
+                {
+                    "shape": "InvalidInputException"
+                },
+                {
+                    "shape": "InternalServiceException"
+                },
+                {
+                    "shape": "AlreadyExistsException"
+                },
+                {
+                    "shape": "OperationTimeoutException"
+                },
+                {
+                    "shape": "ResourceNumberLimitExceededException"
+                },
+                {
+                    "shape": "OperationNotSupportedException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "CreateUsageProfileRequest"
+            },
+            "name": "CreateUsageProfile",
+            "output": {
+                "shape": "CreateUsageProfileResponse"
+            }
+        },
         "CreateUserDefinedFunction": {
             "errors": [
                 {
                     "shape": "AlreadyExistsException"
                 },
                 {
                     "shape": "InvalidInputException"
@@ -1743,14 +1594,17 @@
                     "shape": "CrawlerRunningException"
                 },
                 {
                     "shape": "SchedulerTransitioningException"
                 },
                 {
                     "shape": "OperationTimeoutException"
+                },
+                {
+                    "shape": "InvalidInputException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -1874,96 +1728,41 @@
                 "shape": "DeleteDevEndpointRequest"
             },
             "name": "DeleteDevEndpoint",
             "output": {
                 "shape": "DeleteDevEndpointResponse"
             }
         },
-        "DeleteFederationProfile": {
+        "DeleteJob": {
             "errors": [
                 {
-                    "shape": "EntityNotFoundException"
-                },
-                {
                     "shape": "InvalidInputException"
                 },
                 {
                     "shape": "InternalServiceException"
                 },
                 {
                     "shape": "OperationTimeoutException"
                 },
                 {
-                    "shape": "GlueEncryptionException"
-                },
-                {
-                    "shape": "ConcurrentModificationException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "DeleteFederationProfileRequest"
-            },
-            "name": "DeleteFederationProfile",
-            "output": {
-                "shape": "DeleteFederationProfileResponse"
-            }
-        },
-        "DeleteJob": {
-            "errors": [
-                {
-                    "shape": "InvalidInputException"
-                },
-                {
-                    "shape": "InternalServiceException"
-                },
-                {
-                    "shape": "OperationTimeoutException"
+                    "shape": "AccessDeniedException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DeleteJobRequest"
             },
             "name": "DeleteJob",
             "output": {
                 "shape": "DeleteJobResponse"
             }
         },
-        "DeleteLineageNode": {
-            "documentation": "Deletes the lineage node represented in the input. This may result in gaps in Lineage Graph, please be careful when using this API.",
-            "errors": [
-                {
-                    "shape": "InternalServiceException"
-                },
-                {
-                    "shape": "InvalidInputException"
-                },
-                {
-                    "shape": "OperationTimeoutException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "DeleteLineageNodeRequest"
-            },
-            "name": "DeleteLineageNode",
-            "output": {
-                "shape": "DeleteLineageNodeResponse"
-            }
-        },
         "DeleteMLTransform": {
             "errors": [
                 {
                     "shape": "EntityNotFoundException"
                 },
                 {
                     "shape": "InvalidInputException"
@@ -2256,14 +2055,44 @@
                 "shape": "DeleteTableRequest"
             },
             "name": "DeleteTable",
             "output": {
                 "shape": "DeleteTableResponse"
             }
         },
+        "DeleteTableOptimizer": {
+            "errors": [
+                {
+                    "shape": "EntityNotFoundException"
+                },
+                {
+                    "shape": "InvalidInputException"
+                },
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "InternalServiceException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "DeleteTableOptimizerRequest"
+            },
+            "name": "DeleteTableOptimizer",
+            "output": {
+                "shape": "DeleteTableOptimizerResponse"
+            }
+        },
         "DeleteTableVersion": {
             "errors": [
                 {
                     "shape": "EntityNotFoundException"
                 },
                 {
                     "shape": "InvalidInputException"
@@ -2313,94 +2142,96 @@
                 "shape": "DeleteTriggerRequest"
             },
             "name": "DeleteTrigger",
             "output": {
                 "shape": "DeleteTriggerResponse"
             }
         },
-        "DeleteUserDefinedFunction": {
+        "DeleteUsageProfile": {
             "errors": [
                 {
-                    "shape": "EntityNotFoundException"
-                },
-                {
                     "shape": "InvalidInputException"
                 },
                 {
                     "shape": "InternalServiceException"
                 },
                 {
                     "shape": "OperationTimeoutException"
                 },
                 {
-                    "shape": "GlueEncryptionException"
+                    "shape": "OperationNotSupportedException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
-                "shape": "DeleteUserDefinedFunctionRequest"
+                "shape": "DeleteUsageProfileRequest"
             },
-            "name": "DeleteUserDefinedFunction",
+            "name": "DeleteUsageProfile",
             "output": {
-                "shape": "DeleteUserDefinedFunctionResponse"
+                "shape": "DeleteUsageProfileResponse"
             }
         },
-        "DeleteWorkflow": {
+        "DeleteUserDefinedFunction": {
             "errors": [
                 {
+                    "shape": "EntityNotFoundException"
+                },
+                {
                     "shape": "InvalidInputException"
                 },
                 {
                     "shape": "InternalServiceException"
                 },
                 {
                     "shape": "OperationTimeoutException"
                 },
                 {
-                    "shape": "ConcurrentModificationException"
+                    "shape": "GlueEncryptionException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
-                "shape": "DeleteWorkflowRequest"
+                "shape": "DeleteUserDefinedFunctionRequest"
             },
-            "name": "DeleteWorkflow",
+            "name": "DeleteUserDefinedFunction",
             "output": {
-                "shape": "DeleteWorkflowResponse"
+                "shape": "DeleteUserDefinedFunctionResponse"
             }
         },
-        "ExportLineageGraph": {
-            "documentation": "Retrieves the list of lineage nodes in the specified catalog. If no catalog is specified, the AWS account ID is used by default.",
+        "DeleteWorkflow": {
             "errors": [
                 {
                     "shape": "InvalidInputException"
                 },
                 {
                     "shape": "InternalServiceException"
                 },
                 {
                     "shape": "OperationTimeoutException"
+                },
+                {
+                    "shape": "ConcurrentModificationException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
-                "shape": "ExportLineageGraphRequest"
+                "shape": "DeleteWorkflowRequest"
             },
-            "name": "ExportLineageGraph",
+            "name": "DeleteWorkflow",
             "output": {
-                "shape": "ExportLineageGraphResponse"
+                "shape": "DeleteWorkflowResponse"
             }
         },
         "GetBlueprint": {
             "errors": [
                 {
                     "shape": "EntityNotFoundException"
                 },
@@ -2422,42 +2253,20 @@
                 "shape": "GetBlueprintRequest"
             },
             "name": "GetBlueprint",
             "output": {
                 "shape": "GetBlueprintResponse"
             }
         },
-        "GetBlueprintInstance": {
+        "GetBlueprintRun": {
             "errors": [
                 {
-                    "shape": "EntityNotFoundException"
-                },
-                {
-                    "shape": "InternalServiceException"
+                    "shape": "InvalidInputException"
                 },
                 {
-                    "shape": "OperationTimeoutException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "GetBlueprintInstanceRequest"
-            },
-            "internalonly": true,
-            "name": "GetBlueprintInstance",
-            "output": {
-                "shape": "GetBlueprintInstanceResponse"
-            }
-        },
-        "GetBlueprintRun": {
-            "errors": [
-                {
                     "shape": "EntityNotFoundException"
                 },
                 {
                     "shape": "InternalServiceException"
                 },
                 {
                     "shape": "OperationTimeoutException"
@@ -2522,28 +2331,14 @@
                 "shape": "GetCatalogImportStatusRequest"
             },
             "name": "GetCatalogImportStatus",
             "output": {
                 "shape": "GetCatalogImportStatusResponse"
             }
         },
-        "GetCellInfo": {
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "GetCellInfoRequest"
-            },
-            "internalonly": true,
-            "name": "GetCellInfo",
-            "output": {
-                "shape": "GetCellInfoResponse"
-            }
-        },
         "GetClassifier": {
             "errors": [
                 {
                     "shape": "EntityNotFoundException"
                 },
                 {
                     "shape": "OperationTimeoutException"
@@ -2635,14 +2430,59 @@
                 "shape": "GetColumnStatisticsForTableRequest"
             },
             "name": "GetColumnStatisticsForTable",
             "output": {
                 "shape": "GetColumnStatisticsForTableResponse"
             }
         },
+        "GetColumnStatisticsTaskRun": {
+            "errors": [
+                {
+                    "shape": "EntityNotFoundException"
+                },
+                {
+                    "shape": "OperationTimeoutException"
+                },
+                {
+                    "shape": "InvalidInputException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "GetColumnStatisticsTaskRunRequest"
+            },
+            "name": "GetColumnStatisticsTaskRun",
+            "output": {
+                "shape": "GetColumnStatisticsTaskRunResponse"
+            }
+        },
+        "GetColumnStatisticsTaskRuns": {
+            "errors": [
+                {
+                    "shape": "InvalidInputException"
+                },
+                {
+                    "shape": "OperationTimeoutException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "GetColumnStatisticsTaskRunsRequest"
+            },
+            "name": "GetColumnStatisticsTaskRuns",
+            "output": {
+                "shape": "GetColumnStatisticsTaskRunsResponse"
+            }
+        },
         "GetConnection": {
             "errors": [
                 {
                     "shape": "EntityNotFoundException"
                 },
                 {
                     "shape": "OperationTimeoutException"
@@ -3053,192 +2893,30 @@
                 "shape": "GetDevEndpointsRequest"
             },
             "name": "GetDevEndpoints",
             "output": {
                 "shape": "GetDevEndpointsResponse"
             }
         },
-        "GetFederationProfile": {
-            "errors": [
-                {
-                    "shape": "EntityNotFoundException"
-                },
-                {
-                    "shape": "InvalidInputException"
-                },
-                {
-                    "shape": "InternalServiceException"
-                },
-                {
-                    "shape": "OperationTimeoutException"
-                },
-                {
-                    "shape": "GlueEncryptionException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "GetFederationProfileRequest"
-            },
-            "name": "GetFederationProfile",
-            "output": {
-                "shape": "GetFederationProfileResponse"
-            }
-        },
-        "GetFederationProfiles": {
-            "errors": [
-                {
-                    "shape": "InvalidInputException"
-                },
-                {
-                    "shape": "InternalServiceException"
-                },
-                {
-                    "shape": "OperationTimeoutException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "GetFederationProfilesRequest"
-            },
-            "name": "GetFederationProfiles",
-            "output": {
-                "shape": "GetFederationProfilesResponse"
-            }
-        },
-        "GetInternalUnfilteredPartition": {
-            "errors": [
-                {
-                    "shape": "EntityNotFoundException"
-                },
-                {
-                    "shape": "InvalidInputException"
-                },
-                {
-                    "shape": "InternalServiceException"
-                },
-                {
-                    "shape": "OperationTimeoutException"
-                },
-                {
-                    "shape": "GlueEncryptionException"
-                },
-                {
-                    "shape": "FederationSourceException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "GetInternalUnfilteredPartitionRequest"
-            },
-            "internalonly": true,
-            "name": "GetInternalUnfilteredPartition",
-            "output": {
-                "shape": "GetInternalUnfilteredPartitionResponse"
-            }
-        },
-        "GetInternalUnfilteredPartitions": {
+        "GetJob": {
             "errors": [
                 {
-                    "shape": "EntityNotFoundException"
-                },
-                {
                     "shape": "InvalidInputException"
                 },
                 {
-                    "shape": "InternalServiceException"
-                },
-                {
-                    "shape": "OperationTimeoutException"
-                },
-                {
-                    "shape": "GlueEncryptionException"
-                },
-                {
-                    "shape": "InvalidStateException"
-                },
-                {
-                    "shape": "ResourceNotReadyException"
-                },
-                {
-                    "shape": "FederationSourceException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "GetInternalUnfilteredPartitionsRequest"
-            },
-            "internalonly": true,
-            "name": "GetInternalUnfilteredPartitions",
-            "output": {
-                "shape": "GetInternalUnfilteredPartitionsResponse"
-            }
-        },
-        "GetInternalUnfilteredTable": {
-            "errors": [
-                {
                     "shape": "EntityNotFoundException"
                 },
                 {
-                    "shape": "InvalidInputException"
-                },
-                {
                     "shape": "InternalServiceException"
                 },
                 {
                     "shape": "OperationTimeoutException"
                 },
                 {
-                    "shape": "GlueEncryptionException"
-                },
-                {
-                    "shape": "ResourceNotReadyException"
-                },
-                {
-                    "shape": "FederationSourceException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "GetInternalUnfilteredTableRequest"
-            },
-            "internalonly": true,
-            "name": "GetInternalUnfilteredTable",
-            "output": {
-                "shape": "GetInternalUnfilteredTableResponse"
-            }
-        },
-        "GetJob": {
-            "errors": [
-                {
-                    "shape": "InvalidInputException"
-                },
-                {
-                    "shape": "EntityNotFoundException"
-                },
-                {
-                    "shape": "InternalServiceException"
-                },
-                {
-                    "shape": "OperationTimeoutException"
+                    "shape": "AccessDeniedException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -3297,14 +2975,15 @@
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "GetJobBookmarksRequest"
             },
+            "internalonly": true,
             "name": "GetJobBookmarks",
             "output": {
                 "shape": "GetJobBookmarksResponse"
             }
         },
         "GetJobRun": {
             "errors": [
@@ -3383,64 +3062,14 @@
                 "shape": "GetJobsRequest"
             },
             "name": "GetJobs",
             "output": {
                 "shape": "GetJobsResponse"
             }
         },
-        "GetLineageCaptureSettings": {
-            "documentation": "Retrieves the automatic lineage publishing configuration in the specified catalog.",
-            "errors": [
-                {
-                    "shape": "InternalServiceException"
-                },
-                {
-                    "shape": "InvalidInputException"
-                },
-                {
-                    "shape": "OperationTimeoutException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "GetLineageCaptureSettingsRequest"
-            },
-            "name": "GetLineageCaptureSettings",
-            "output": {
-                "shape": "GetLineageCaptureSettingsResponse"
-            }
-        },
-        "GetLineageGraph": {
-            "documentation": "Retrieves the lineage node identified in the input, and all its immediate neighbors in the lineage graph.",
-            "errors": [
-                {
-                    "shape": "InvalidInputException"
-                },
-                {
-                    "shape": "InternalServiceException"
-                },
-                {
-                    "shape": "OperationTimeoutException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "GetLineageGraphRequest"
-            },
-            "name": "GetLineageGraph",
-            "output": {
-                "shape": "GetLineageGraphResponse"
-            }
-        },
         "GetMLTaskRun": {
             "errors": [
                 {
                     "shape": "EntityNotFoundException"
                 },
                 {
                     "shape": "InvalidInputException"
@@ -3615,14 +3244,17 @@
                     "shape": "OperationTimeoutException"
                 },
                 {
                     "shape": "GlueEncryptionException"
                 },
                 {
                     "shape": "FederationSourceException"
+                },
+                {
+                    "shape": "FederationSourceRetryableException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -3684,14 +3316,17 @@
                     "shape": "InvalidStateException"
                 },
                 {
                     "shape": "ResourceNotReadyException"
                 },
                 {
                     "shape": "FederationSourceException"
+                },
+                {
+                    "shape": "FederationSourceRetryableException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -3838,61 +3473,14 @@
             },
             "internalonly": true,
             "name": "GetResourcePolicy",
             "output": {
                 "shape": "GetResourcePolicyResponse"
             }
         },
-        "GetResourcePolicyInternal": {
-            "documentation": "Internal API to get the resource policy on a resource",
-            "errors": [
-                {
-                    "shape": "RAMResourceNotFoundException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "GetResourcePolicyInternalRequest"
-            },
-            "name": "GetResourcePolicyInternal",
-            "output": {
-                "shape": "GetResourcePolicyInternalResponse"
-            }
-        },
-        "GetSaveLocationForTableStatistics": {
-            "errors": [
-                {
-                    "shape": "EntityNotFoundException"
-                },
-                {
-                    "shape": "InvalidInputException"
-                },
-                {
-                    "shape": "OperationTimeoutException"
-                },
-                {
-                    "shape": "InternalServiceException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "GetSaveLocationForTableStatisticsRequest"
-            },
-            "internalonly": true,
-            "name": "GetSaveLocationForTableStatistics",
-            "output": {
-                "shape": "GetSaveLocationForTableStatisticsResponse"
-            }
-        },
         "GetSaveLocationForTransformArtifact": {
             "errors": [
                 {
                     "shape": "EntityNotFoundException"
                 },
                 {
                     "shape": "InvalidInputException"
@@ -4160,82 +3748,59 @@
                     "shape": "GlueEncryptionException"
                 },
                 {
                     "shape": "ResourceNotReadyException"
                 },
                 {
                     "shape": "FederationSourceException"
+                },
+                {
+                    "shape": "FederationSourceRetryableException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "GetTableRequest"
             },
             "name": "GetTable",
             "output": {
                 "shape": "GetTableResponse"
             }
         },
-        "GetTableStatisticsMetadata": {
+        "GetTableOptimizer": {
             "errors": [
                 {
                     "shape": "EntityNotFoundException"
                 },
                 {
                     "shape": "InvalidInputException"
                 },
                 {
-                    "shape": "OperationTimeoutException"
+                    "shape": "AccessDeniedException"
                 },
                 {
                     "shape": "InternalServiceException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "GetTableStatisticsMetadataRequest"
-            },
-            "internalonly": true,
-            "name": "GetTableStatisticsMetadata",
-            "output": {
-                "shape": "GetTableStatisticsMetadataResponse"
-            }
-        },
-        "GetTableStatisticsTaskRun": {
-            "errors": [
-                {
-                    "shape": "EntityNotFoundException"
-                },
-                {
-                    "shape": "InvalidInputException"
                 },
                 {
-                    "shape": "OperationTimeoutException"
-                },
-                {
-                    "shape": "InternalServiceException"
+                    "shape": "ThrottlingException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
-                "shape": "GetTableStatisticsTaskRunRequest"
+                "shape": "GetTableOptimizerRequest"
             },
-            "internalonly": true,
-            "name": "GetTableStatisticsTaskRun",
+            "name": "GetTableOptimizer",
             "output": {
-                "shape": "GetTableStatisticsTaskRunResponse"
+                "shape": "GetTableOptimizerResponse"
             }
         },
         "GetTableVersion": {
             "errors": [
                 {
                     "shape": "EntityNotFoundException"
                 },
@@ -4309,56 +3874,31 @@
                     "shape": "InternalServiceException"
                 },
                 {
                     "shape": "GlueEncryptionException"
                 },
                 {
                     "shape": "FederationSourceException"
+                },
+                {
+                    "shape": "FederationSourceRetryableException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "GetTablesRequest"
             },
             "name": "GetTables",
             "output": {
                 "shape": "GetTablesResponse"
             }
         },
-        "GetTaggedResources": {
-            "errors": [
-                {
-                    "shape": "InvalidInputException"
-                },
-                {
-                    "shape": "InternalServiceException"
-                },
-                {
-                    "shape": "OperationTimeoutException"
-                },
-                {
-                    "shape": "EntityNotFoundException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "GetTaggedResourcesRequest"
-            },
-            "internalonly": true,
-            "name": "GetTaggedResources",
-            "output": {
-                "shape": "GetTaggedResourcesResponse"
-            }
-        },
         "GetTags": {
             "errors": [
                 {
                     "shape": "InvalidInputException"
                 },
                 {
                     "shape": "InternalServiceException"
@@ -4516,15 +4056,15 @@
                 "shape": "GetTriggersRequest"
             },
             "name": "GetTriggers",
             "output": {
                 "shape": "GetTriggersResponse"
             }
         },
-        "GetUnfilteredPartition": {
+        "GetUnfilteredPartitionMetadata": {
             "errors": [
                 {
                     "shape": "EntityNotFoundException"
                 },
                 {
                     "shape": "InvalidInputException"
                 },
@@ -4534,63 +4074,36 @@
                 {
                     "shape": "OperationTimeoutException"
                 },
                 {
                     "shape": "GlueEncryptionException"
                 },
                 {
-                    "shape": "FederationSourceException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "GetUnfilteredPartitionRequest"
-            },
-            "name": "GetUnfilteredPartition",
-            "output": {
-                "shape": "GetUnfilteredPartitionResponse"
-            }
-        },
-        "GetUnfilteredPartitionMetadata": {
-            "errors": [
-                {
-                    "shape": "EntityNotFoundException"
-                },
-                {
-                    "shape": "InvalidInputException"
-                },
-                {
-                    "shape": "InternalServiceException"
-                },
-                {
-                    "shape": "OperationTimeoutException"
+                    "shape": "PermissionTypeMismatchException"
                 },
                 {
-                    "shape": "GlueEncryptionException"
+                    "shape": "FederationSourceException"
                 },
                 {
-                    "shape": "PermissionTypeMismatchException"
+                    "shape": "FederationSourceRetryableException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "GetUnfilteredPartitionMetadataRequest"
             },
             "name": "GetUnfilteredPartitionMetadata",
             "output": {
                 "shape": "GetUnfilteredPartitionMetadataResponse"
             }
         },
-        "GetUnfilteredPartitions": {
+        "GetUnfilteredPartitionsMetadata": {
             "errors": [
                 {
                     "shape": "EntityNotFoundException"
                 },
                 {
                     "shape": "InvalidInputException"
                 },
@@ -4603,66 +4116,36 @@
                 {
                     "shape": "GlueEncryptionException"
                 },
                 {
                     "shape": "InvalidStateException"
                 },
                 {
-                    "shape": "FederationSourceException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "GetUnfilteredPartitionsRequest"
-            },
-            "name": "GetUnfilteredPartitions",
-            "output": {
-                "shape": "GetUnfilteredPartitionsResponse"
-            }
-        },
-        "GetUnfilteredPartitionsMetadata": {
-            "errors": [
-                {
-                    "shape": "EntityNotFoundException"
-                },
-                {
-                    "shape": "InvalidInputException"
-                },
-                {
-                    "shape": "InternalServiceException"
-                },
-                {
-                    "shape": "OperationTimeoutException"
-                },
-                {
-                    "shape": "GlueEncryptionException"
+                    "shape": "PermissionTypeMismatchException"
                 },
                 {
-                    "shape": "InvalidStateException"
+                    "shape": "FederationSourceException"
                 },
                 {
-                    "shape": "PermissionTypeMismatchException"
+                    "shape": "FederationSourceRetryableException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "GetUnfilteredPartitionsMetadataRequest"
             },
             "name": "GetUnfilteredPartitionsMetadata",
             "output": {
                 "shape": "GetUnfilteredPartitionsMetadataResponse"
             }
         },
-        "GetUnfilteredTable": {
+        "GetUnfilteredTableMetadata": {
             "errors": [
                 {
                     "shape": "EntityNotFoundException"
                 },
                 {
                     "shape": "InvalidInputException"
                 },
@@ -4675,63 +4158,63 @@
                 {
                     "shape": "GlueEncryptionException"
                 },
                 {
                     "shape": "ResourceNotReadyException"
                 },
                 {
+                    "shape": "PermissionTypeMismatchException"
+                },
+                {
                     "shape": "FederationSourceException"
+                },
+                {
+                    "shape": "FederationSourceRetryableException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
-                "shape": "GetUnfilteredTableRequest"
+                "shape": "GetUnfilteredTableMetadataRequest"
             },
-            "name": "GetUnfilteredTable",
+            "name": "GetUnfilteredTableMetadata",
             "output": {
-                "shape": "GetUnfilteredTableResponse"
+                "shape": "GetUnfilteredTableMetadataResponse"
             }
         },
-        "GetUnfilteredTableMetadata": {
+        "GetUsageProfile": {
             "errors": [
                 {
-                    "shape": "EntityNotFoundException"
-                },
-                {
                     "shape": "InvalidInputException"
                 },
                 {
                     "shape": "InternalServiceException"
                 },
                 {
-                    "shape": "OperationTimeoutException"
-                },
-                {
-                    "shape": "GlueEncryptionException"
+                    "shape": "EntityNotFoundException"
                 },
                 {
-                    "shape": "ResourceNotReadyException"
+                    "shape": "OperationTimeoutException"
                 },
                 {
-                    "shape": "PermissionTypeMismatchException"
+                    "shape": "OperationNotSupportedException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
-                "shape": "GetUnfilteredTableMetadataRequest"
+                "shape": "GetUsageProfileRequest"
             },
-            "name": "GetUnfilteredTableMetadata",
+            "name": "GetUsageProfile",
             "output": {
-                "shape": "GetUnfilteredTableMetadataResponse"
+                "shape": "GetUsageProfileResponse"
             }
         },
         "GetUserDefinedFunction": {
             "errors": [
                 {
                     "shape": "EntityNotFoundException"
                 },
@@ -4949,78 +4432,54 @@
             },
             "internalonly": true,
             "name": "InstantiateTemplate",
             "output": {
                 "shape": "InstantiateTemplateResponse"
             }
         },
-        "ListBlueprintInstances": {
+        "ListBlueprints": {
             "errors": [
                 {
                     "shape": "InvalidInputException"
                 },
                 {
-                    "shape": "EntityNotFoundException"
-                },
-                {
                     "shape": "InternalServiceException"
                 },
                 {
                     "shape": "OperationTimeoutException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
-                "shape": "ListBlueprintInstancesRequest"
+                "shape": "ListBlueprintsRequest"
             },
-            "internalonly": true,
-            "name": "ListBlueprintInstances",
+            "name": "ListBlueprints",
             "output": {
-                "shape": "ListBlueprintInstancesResponse"
+                "shape": "ListBlueprintsResponse"
             }
         },
-        "ListBlueprints": {
+        "ListColumnStatisticsTaskRuns": {
             "errors": [
                 {
-                    "shape": "InvalidInputException"
-                },
-                {
-                    "shape": "InternalServiceException"
-                },
-                {
                     "shape": "OperationTimeoutException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
-                "shape": "ListBlueprintsRequest"
+                "shape": "ListColumnStatisticsTaskRunsRequest"
             },
-            "name": "ListBlueprints",
+            "name": "ListColumnStatisticsTaskRuns",
             "output": {
-                "shape": "ListBlueprintsResponse"
-            }
-        },
-        "ListConsumerAccounts": {
-            "documentation": "Returns a paginated list of all consumer accounts which has shared resources. This API is used for reconcile.",
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "ListConsumerAccountsRequest"
-            },
-            "name": "ListConsumerAccounts",
-            "output": {
-                "shape": "ListConsumerAccountsResponse"
+                "shape": "ListColumnStatisticsTaskRunsResponse"
             }
         },
         "ListCrawlers": {
             "errors": [
                 {
                     "shape": "OperationTimeoutException"
                 }
@@ -5285,28 +4744,14 @@
                 "shape": "ListRegistriesInput"
             },
             "name": "ListRegistries",
             "output": {
                 "shape": "ListRegistriesResponse"
             }
         },
-        "ListResourcesSupportPolicy": {
-            "documentation": "List all of the resources that have a policy document",
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "ListResourcesSupportPolicyRequest"
-            },
-            "name": "ListResourcesSupportPolicy",
-            "output": {
-                "shape": "ListResourcesSupportPolicyResponse"
-            }
-        },
         "ListSchemaVersions": {
             "errors": [
                 {
                     "shape": "InvalidInputException"
                 },
                 {
                     "shape": "AccessDeniedException"
@@ -5380,28 +4825,14 @@
                 "shape": "ListSessionsRequest"
             },
             "name": "ListSessions",
             "output": {
                 "shape": "ListSessionsResponse"
             }
         },
-        "ListSharedResources": {
-            "documentation": "Lists all of the resources an account has been shared to. This API is used for reconcile.",
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "ListSharedResourcesRequest"
-            },
-            "name": "ListSharedResources",
-            "output": {
-                "shape": "ListSharedResourcesResponse"
-            }
-        },
         "ListStatements": {
             "errors": [
                 {
                     "shape": "AccessDeniedException"
                 },
                 {
                     "shape": "EntityNotFoundException"
@@ -5427,93 +4858,123 @@
                 "shape": "ListStatementsRequest"
             },
             "name": "ListStatements",
             "output": {
                 "shape": "ListStatementsResponse"
             }
         },
-        "ListTriggers": {
+        "ListTableOptimizerRuns": {
             "errors": [
                 {
                     "shape": "EntityNotFoundException"
                 },
                 {
+                    "shape": "AccessDeniedException"
+                },
+                {
                     "shape": "InvalidInputException"
                 },
                 {
+                    "shape": "ValidationException"
+                },
+                {
                     "shape": "InternalServiceException"
                 },
                 {
-                    "shape": "OperationTimeoutException"
+                    "shape": "ThrottlingException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
-                "shape": "ListTriggersRequest"
+                "shape": "ListTableOptimizerRunsRequest"
             },
-            "name": "ListTriggers",
+            "name": "ListTableOptimizerRuns",
             "output": {
-                "shape": "ListTriggersResponse"
+                "shape": "ListTableOptimizerRunsResponse"
             }
         },
-        "ListWorkflows": {
+        "ListTriggers": {
             "errors": [
                 {
+                    "shape": "EntityNotFoundException"
+                },
+                {
                     "shape": "InvalidInputException"
                 },
                 {
                     "shape": "InternalServiceException"
                 },
                 {
                     "shape": "OperationTimeoutException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
-                "shape": "ListWorkflowsRequest"
+                "shape": "ListTriggersRequest"
             },
-            "name": "ListWorkflows",
+            "name": "ListTriggers",
             "output": {
-                "shape": "ListWorkflowsResponse"
+                "shape": "ListTriggersResponse"
             }
         },
-        "NotifyEvent": {
+        "ListUsageProfiles": {
             "errors": [
                 {
-                    "shape": "EntityNotFoundException"
-                },
-                {
                     "shape": "InternalServiceException"
                 },
                 {
                     "shape": "OperationTimeoutException"
                 },
                 {
                     "shape": "InvalidInputException"
                 },
                 {
-                    "shape": "ConcurrentRunsExceededException"
+                    "shape": "OperationNotSupportedException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
-                "shape": "NotifyEventRequest"
+                "shape": "ListUsageProfilesRequest"
             },
-            "name": "NotifyEvent",
+            "name": "ListUsageProfiles",
             "output": {
-                "shape": "NotifyEventResponse"
+                "shape": "ListUsageProfilesResponse"
+            }
+        },
+        "ListWorkflows": {
+            "errors": [
+                {
+                    "shape": "InvalidInputException"
+                },
+                {
+                    "shape": "InternalServiceException"
+                },
+                {
+                    "shape": "OperationTimeoutException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "ListWorkflowsRequest"
+            },
+            "name": "ListWorkflows",
+            "output": {
+                "shape": "ListWorkflowsResponse"
             }
         },
         "PublishDataQualityResult": {
             "errors": [
                 {
                     "shape": "InvalidInputException"
                 },
@@ -5676,39 +5137,14 @@
             },
             "internalonly": true,
             "name": "PutJobMetadataForMLTransform",
             "output": {
                 "shape": "PutJobMetadataForMLTransformResponse"
             }
         },
-        "PutLineageCaptureSettings": {
-            "documentation": "Updates the automatic lineage publishing configuration in the specified catalog.",
-            "errors": [
-                {
-                    "shape": "InternalServiceException"
-                },
-                {
-                    "shape": "InvalidInputException"
-                },
-                {
-                    "shape": "OperationTimeoutException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "PutLineageCaptureSettingsRequest"
-            },
-            "name": "PutLineageCaptureSettings",
-            "output": {
-                "shape": "PutLineageCaptureSettingsResponse"
-            }
-        },
         "PutResourcePolicy": {
             "errors": [
                 {
                     "shape": "EntityNotFoundException"
                 },
                 {
                     "shape": "InternalServiceException"
@@ -5720,14 +5156,17 @@
                     "shape": "InvalidInputException"
                 },
                 {
                     "shape": "ConditionCheckFailureException"
                 },
                 {
                     "shape": "GlueEncryptionException"
+                },
+                {
+                    "shape": "ConcurrentModificationException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -5966,14 +5405,17 @@
                 {
                     "shape": "ValidationException"
                 },
                 {
                     "shape": "ResourceNumberLimitExceededException"
                 },
                 {
+                    "shape": "SessionBusyException"
+                },
+                {
                     "shape": "IllegalSessionStateException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
@@ -6044,14 +5486,47 @@
                 "shape": "StartBlueprintRunRequest"
             },
             "name": "StartBlueprintRun",
             "output": {
                 "shape": "StartBlueprintRunResponse"
             }
         },
+        "StartColumnStatisticsTaskRun": {
+            "errors": [
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "EntityNotFoundException"
+                },
+                {
+                    "shape": "ColumnStatisticsTaskRunningException"
+                },
+                {
+                    "shape": "OperationTimeoutException"
+                },
+                {
+                    "shape": "ResourceNumberLimitExceededException"
+                },
+                {
+                    "shape": "InvalidInputException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "StartColumnStatisticsTaskRunRequest"
+            },
+            "name": "StartColumnStatisticsTaskRun",
+            "output": {
+                "shape": "StartColumnStatisticsTaskRunResponse"
+            }
+        },
         "StartCrawler": {
             "errors": [
                 {
                     "shape": "AccessDeniedException"
                 },
                 {
                     "shape": "EntityNotFoundException"
@@ -6123,14 +5598,17 @@
                     "shape": "OperationTimeoutException"
                 },
                 {
                     "shape": "InternalServiceException"
                 },
                 {
                     "shape": "ConflictException"
+                },
+                {
+                    "shape": "ResourceNumberLimitExceededException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "idempotent": true,
@@ -6154,14 +5632,17 @@
                     "shape": "OperationTimeoutException"
                 },
                 {
                     "shape": "InternalServiceException"
                 },
                 {
                     "shape": "ConflictException"
+                },
+                {
+                    "shape": "ResourceNumberLimitExceededException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "idempotent": true,
@@ -6325,45 +5806,14 @@
                 "shape": "StartMLLabelingSetGenerationTaskRunRequest"
             },
             "name": "StartMLLabelingSetGenerationTaskRun",
             "output": {
                 "shape": "StartMLLabelingSetGenerationTaskRunResponse"
             }
         },
-        "StartTableStatisticsTaskRun": {
-            "errors": [
-                {
-                    "shape": "InvalidInputException"
-                },
-                {
-                    "shape": "OperationTimeoutException"
-                },
-                {
-                    "shape": "InternalServiceException"
-                },
-                {
-                    "shape": "AccessDeniedException"
-                },
-                {
-                    "shape": "ResourceNumberLimitExceededException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "StartTableStatisticsTaskRunRequest"
-            },
-            "internalonly": true,
-            "name": "StartTableStatisticsTaskRun",
-            "output": {
-                "shape": "StartTableStatisticsTaskRunResponse"
-            }
-        },
         "StartTrigger": {
             "errors": [
                 {
                     "shape": "AccessDeniedException"
                 },
                 {
                     "shape": "InvalidInputException"
@@ -6437,14 +5887,44 @@
                 "shape": "StartWorkflowRunRequest"
             },
             "name": "StartWorkflowRun",
             "output": {
                 "shape": "StartWorkflowRunResponse"
             }
         },
+        "StopColumnStatisticsTaskRun": {
+            "errors": [
+                {
+                    "shape": "EntityNotFoundException"
+                },
+                {
+                    "shape": "ColumnStatisticsTaskNotRunningException"
+                },
+                {
+                    "shape": "ColumnStatisticsTaskStoppingException"
+                },
+                {
+                    "shape": "InvalidInputException"
+                },
+                {
+                    "shape": "OperationTimeoutException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "StopColumnStatisticsTaskRunRequest"
+            },
+            "name": "StopColumnStatisticsTaskRun",
+            "output": {
+                "shape": "StopColumnStatisticsTaskRunResponse"
+            }
+        },
         "StopCrawler": {
             "errors": [
                 {
                     "shape": "EntityNotFoundException"
                 },
                 {
                     "shape": "CrawlerNotRunningException"
@@ -6800,14 +6280,17 @@
                 {
                     "shape": "VersionMismatchException"
                 },
                 {
                     "shape": "EntityNotFoundException"
                 },
                 {
+                    "shape": "ResourceNumberLimitExceededException"
+                },
+                {
                     "shape": "CrawlerRunningException"
                 },
                 {
                     "shape": "OperationTimeoutException"
                 }
             ],
             "http": {
@@ -6947,50 +6430,14 @@
                 "shape": "UpdateDevEndpointRequest"
             },
             "name": "UpdateDevEndpoint",
             "output": {
                 "shape": "UpdateDevEndpointResponse"
             }
         },
-        "UpdateFederationProfile": {
-            "errors": [
-                {
-                    "shape": "EntityNotFoundException"
-                },
-                {
-                    "shape": "InvalidInputException"
-                },
-                {
-                    "shape": "ResourceNumberLimitExceededException"
-                },
-                {
-                    "shape": "InternalServiceException"
-                },
-                {
-                    "shape": "OperationTimeoutException"
-                },
-                {
-                    "shape": "GlueEncryptionException"
-                },
-                {
-                    "shape": "ConcurrentModificationException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "UpdateFederationProfileRequest"
-            },
-            "name": "UpdateFederationProfile",
-            "output": {
-                "shape": "UpdateFederationProfileResponse"
-            }
-        },
         "UpdateJob": {
             "errors": [
                 {
                     "shape": "InvalidInputException"
                 },
                 {
                     "shape": "EntityNotFoundException"
@@ -6999,14 +6446,17 @@
                     "shape": "InternalServiceException"
                 },
                 {
                     "shape": "OperationTimeoutException"
                 },
                 {
                     "shape": "ConcurrentModificationException"
+                },
+                {
+                    "shape": "AccessDeniedException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -7080,45 +6530,14 @@
                 "shape": "UpdateJobFromSourceControlRequest"
             },
             "name": "UpdateJobFromSourceControl",
             "output": {
                 "shape": "UpdateJobFromSourceControlResponse"
             }
         },
-        "UpdateLineageNode": {
-            "documentation": "Updates the properties of the lineage node, ie, attributes within LineageNodeMetadata, with the ones specified in the input. Values for any existing key are overwritten, whereas, new key-value pairs are added. Returns the updated lineage node with all properties.",
-            "errors": [
-                {
-                    "shape": "InternalServiceException"
-                },
-                {
-                    "shape": "InvalidInputException"
-                },
-                {
-                    "shape": "EntityNotFoundException"
-                },
-                {
-                    "shape": "OperationTimeoutException"
-                },
-                {
-                    "shape": "ConcurrentModificationException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "UpdateLineageNodeRequest"
-            },
-            "name": "UpdateLineageNode",
-            "output": {
-                "shape": "UpdateLineageNodeResponse"
-            }
-        },
         "UpdateMLTransform": {
             "errors": [
                 {
                     "shape": "EntityNotFoundException"
                 },
                 {
                     "shape": "InvalidInputException"
@@ -7201,39 +6620,14 @@
                 "shape": "UpdateRegistryInput"
             },
             "name": "UpdateRegistry",
             "output": {
                 "shape": "UpdateRegistryResponse"
             }
         },
-        "UpdateResourceSharingState": {
-            "documentation": "Updates resource sharing state if sequence number matches.",
-            "errors": [
-                {
-                    "shape": "RAMResourceNotFoundException"
-                },
-                {
-                    "shape": "RAMInternalIdMismatchException"
-                },
-                {
-                    "shape": "RAMResourceNotSharedException"
-                },
-                {
-                    "shape": "RAMInvalidSequenceNumberException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "UpdateResourceSharingStateRequest"
-            },
-            "name": "UpdateResourceSharingState"
-        },
         "UpdateSchema": {
             "errors": [
                 {
                     "shape": "InvalidInputException"
                 },
                 {
                     "shape": "AccessDeniedException"
@@ -7331,14 +6725,47 @@
                 "shape": "UpdateTableRequest"
             },
             "name": "UpdateTable",
             "output": {
                 "shape": "UpdateTableResponse"
             }
         },
+        "UpdateTableOptimizer": {
+            "errors": [
+                {
+                    "shape": "EntityNotFoundException"
+                },
+                {
+                    "shape": "InvalidInputException"
+                },
+                {
+                    "shape": "AccessDeniedException"
+                },
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "InternalServiceException"
+                },
+                {
+                    "shape": "ThrottlingException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/"
+            },
+            "input": {
+                "shape": "UpdateTableOptimizerRequest"
+            },
+            "name": "UpdateTableOptimizer",
+            "output": {
+                "shape": "UpdateTableOptimizerResponse"
+            }
+        },
         "UpdateTrigger": {
             "errors": [
                 {
                     "shape": "InvalidInputException"
                 },
                 {
                     "shape": "InternalServiceException"
@@ -7420,67 +6847,24 @@
             "input": {
                 "shape": "UpdateWorkflowRequest"
             },
             "name": "UpdateWorkflow",
             "output": {
                 "shape": "UpdateWorkflowResponse"
             }
-        },
-        "ValidateResourceSharing": {
-            "documentation": "Validate if a given resource with a given internal id (if applicable) can be shared by a given owner account.",
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "ValidateResourceSharingRequest"
-            },
-            "name": "ValidateResourceSharing",
-            "output": {
-                "shape": "ValidateResourceSharingResponse"
-            }
-        },
-        "VerifyResourcesExistForTagris": {
-            "errors": [
-                {
-                    "shape": "TagrisAccessDeniedException"
-                },
-                {
-                    "shape": "TagrisInternalServiceException"
-                },
-                {
-                    "shape": "TagrisInvalidArnException"
-                },
-                {
-                    "shape": "TagrisInvalidParameterException"
-                },
-                {
-                    "shape": "TagrisPartialResourcesExistResultsException"
-                },
-                {
-                    "shape": "TagrisThrottledException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "TagrisVerifyResourcesExistInput"
-            },
-            "internalonly": true,
-            "name": "VerifyResourcesExistForTagris",
-            "output": {
-                "shape": "TagrisVerifyResourcesExistOutput"
-            }
         }
     },
     "shapes": {
         "AWSAccountArn": {
-            "pattern": "(^arn:aws:iam::\\w{12}:root)",
+            "pattern": "(^arn:aws(-(cn|us-gov|iso(-[bef])?))?:iam::\\w{12}:root)",
+            "type": "string"
+        },
+        "AWSManagedClientApplicationReference": {
+            "max": 2048,
+            "pattern": "\\S+",
             "type": "string"
         },
         "AccessDeniedException": {
             "exception": true,
             "members": {
                 "Message": {
                     "shape": "MessageString"
@@ -7518,32 +6902,52 @@
         },
         "ActionList": {
             "member": {
                 "shape": "Action"
             },
             "type": "list"
         },
+        "AdditionalContextMap": {
+            "key": {
+                "shape": "ContextKey"
+            },
+            "type": "map",
+            "value": {
+                "shape": "ContextValue"
+            }
+        },
         "AdditionalPlanOptionsMap": {
             "key": {
                 "shape": "GenericString"
             },
             "type": "map",
             "value": {
                 "shape": "GenericString"
             }
         },
+        "AllowedValuesStringList": {
+            "member": {
+                "shape": "ConfigValueString"
+            },
+            "type": "list"
+        },
         "AlreadyExistsException": {
             "exception": true,
             "members": {
                 "Message": {
                     "shape": "MessageString"
                 }
             },
             "type": "structure"
         },
+        "ArnString": {
+            "max": 2048,
+            "min": 20,
+            "type": "string"
+        },
         "ArtifactNotFoundException": {
             "exception": true,
             "internalonly": true,
             "members": {
                 "Message": {
                     "shape": "MessageString"
                 }
@@ -7587,14 +6991,73 @@
         },
         "AuthTokenString": {
             "max": 255,
             "min": 1,
             "pattern": "[\\u0020-\\uD7FF\\uE000-\\uFFFD\\uD800\\uDC00-\\uDBFF\\uDFFF\\t]*",
             "type": "string"
         },
+        "AuthenticationConfiguration": {
+            "members": {
+                "AuthenticationType": {
+                    "shape": "AuthenticationType"
+                },
+                "CustomAuthenticationProperties": {
+                    "shape": "CustomAuthenticationProperties"
+                },
+                "OAuth2Properties": {
+                    "shape": "OAuth2Properties"
+                },
+                "SecretArn": {
+                    "shape": "SecretArn"
+                }
+            },
+            "type": "structure"
+        },
+        "AuthenticationConfigurationInput": {
+            "members": {
+                "AuthenticationType": {
+                    "shape": "AuthenticationType"
+                },
+                "CustomAuthenticationProperties": {
+                    "shape": "CustomAuthenticationProperties"
+                },
+                "OAuth2Properties": {
+                    "shape": "OAuth2PropertiesInput"
+                },
+                "SecretArn": {
+                    "shape": "SecretArn"
+                }
+            },
+            "type": "structure"
+        },
+        "AuthenticationType": {
+            "enum": [
+                "BASIC",
+                "OAUTH2",
+                "CUSTOM"
+            ],
+            "type": "string"
+        },
+        "AuthorizationCode": {
+            "max": 4096,
+            "min": 1,
+            "pattern": "\\S+",
+            "type": "string"
+        },
+        "AuthorizationCodeProperties": {
+            "members": {
+                "AuthorizationCode": {
+                    "shape": "AuthorizationCode"
+                },
+                "RedirectUri": {
+                    "shape": "RedirectUri"
+                }
+            },
+            "type": "structure"
+        },
         "BackfillError": {
             "members": {
                 "Code": {
                     "shape": "BackfillErrorCode"
                 },
                 "Partitions": {
                     "shape": "BackfillErroredPartitionsList"
@@ -7620,79 +7083,14 @@
         },
         "BackfillErrors": {
             "member": {
                 "shape": "BackfillError"
             },
             "type": "list"
         },
-        "BatchColumnStatisticsColumnNamesList": {
-            "max": 20,
-            "member": {
-                "shape": "NameString"
-            },
-            "min": 1,
-            "type": "list"
-        },
-        "BatchColumnStatisticsRequestEntry": {
-            "members": {
-                "ColumnNames": {
-                    "shape": "BatchColumnStatisticsColumnNamesList"
-                },
-                "DatabaseName": {
-                    "shape": "NameString"
-                },
-                "TableName": {
-                    "shape": "NameString"
-                }
-            },
-            "required": [
-                "DatabaseName",
-                "TableName",
-                "ColumnNames"
-            ],
-            "type": "structure"
-        },
-        "BatchColumnStatisticsRequestEntryList": {
-            "max": 10,
-            "member": {
-                "shape": "BatchColumnStatisticsRequestEntry"
-            },
-            "min": 1,
-            "type": "list"
-        },
-        "BatchCreateLineageNodeList": {
-            "documentation": "A list of lineage nodes about to be added to graph.",
-            "max": 30,
-            "member": {
-                "shape": "LineageNode"
-            },
-            "type": "list"
-        },
-        "BatchCreateLineageNodesRequest": {
-            "members": {
-                "CatalogId": {
-                    "shape": "CatalogIdString"
-                },
-                "Nodes": {
-                    "shape": "BatchCreateLineageNodeList"
-                }
-            },
-            "required": [
-                "Nodes"
-            ],
-            "type": "structure"
-        },
-        "BatchCreateLineageNodesResponse": {
-            "members": {
-                "UnprocessedNodes": {
-                    "shape": "LineageNodeList"
-                }
-            },
-            "type": "structure"
-        },
         "BatchCreatePartitionRequest": {
             "members": {
                 "CatalogId": {
                     "shape": "CatalogIdString"
                 },
                 "DatabaseName": {
                     "shape": "NameString"
@@ -7853,48 +7251,14 @@
             "members": {
                 "Errors": {
                     "shape": "TableVersionErrors"
                 }
             },
             "type": "structure"
         },
-        "BatchGetBlueprintInstanceNames": {
-            "max": 25,
-            "member": {
-                "shape": "OrchestrationNameString"
-            },
-            "min": 1,
-            "type": "list"
-        },
-        "BatchGetBlueprintInstancesRequest": {
-            "members": {
-                "BlueprintName": {
-                    "shape": "OrchestrationNameString"
-                },
-                "Names": {
-                    "shape": "BatchGetBlueprintInstanceNames"
-                }
-            },
-            "required": [
-                "Names",
-                "BlueprintName"
-            ],
-            "type": "structure"
-        },
-        "BatchGetBlueprintInstancesResponse": {
-            "members": {
-                "Instances": {
-                    "shape": "BlueprintInstances"
-                },
-                "MissingInstances": {
-                    "shape": "BlueprintInstanceNames"
-                }
-            },
-            "type": "structure"
-        },
         "BatchGetBlueprintNames": {
             "max": 25,
             "member": {
                 "shape": "OrchestrationNameString"
             },
             "min": 1,
             "type": "list"
@@ -7927,39 +7291,14 @@
                 },
                 "MissingBlueprints": {
                     "shape": "BlueprintNames"
                 }
             },
             "type": "structure"
         },
-        "BatchGetColumnStatisticsForTableRequest": {
-            "members": {
-                "CatalogId": {
-                    "shape": "CatalogIdString"
-                },
-                "Entries": {
-                    "shape": "BatchColumnStatisticsRequestEntryList"
-                }
-            },
-            "required": [
-                "Entries"
-            ],
-            "type": "structure"
-        },
-        "BatchGetColumnStatisticsForTableResponse": {
-            "members": {
-                "ColumnStatisticsForTableList": {
-                    "shape": "ColumnStatisticsForTableList"
-                },
-                "Errors": {
-                    "shape": "ColumnStatisticsForTableErrorList"
-                }
-            },
-            "type": "structure"
-        },
         "BatchGetCrawlersRequest": {
             "members": {
                 "CrawlerNames": {
                     "shape": "CrawlerNameList"
                 }
             },
             "required": [
@@ -7976,14 +7315,18 @@
                     "shape": "CrawlerNameList"
                 }
             },
             "type": "structure"
         },
         "BatchGetCustomEntityTypesRequest": {
             "members": {
+                "JobRunId": {
+                    "internalonly": true,
+                    "shape": "NameString"
+                },
                 "Names": {
                     "shape": "CustomEntityTypeNames"
                 }
             },
             "required": [
                 "Names"
             ],
@@ -8051,42 +7394,14 @@
                 },
                 "DevEndpointsNotFound": {
                     "shape": "DevEndpointNames"
                 }
             },
             "type": "structure"
         },
-        "BatchGetInternalUnfilteredTableRequest": {
-            "members": {
-                "AuditContext": {
-                    "shape": "AuditContext"
-                },
-                "CatalogId": {
-                    "shape": "CatalogIdString"
-                },
-                "Entries": {
-                    "shape": "BatchTableRequestEntryList"
-                }
-            },
-            "required": [
-                "Entries"
-            ],
-            "type": "structure"
-        },
-        "BatchGetInternalUnfilteredTableResponse": {
-            "members": {
-                "Errors": {
-                    "shape": "BatchTableErrorList"
-                },
-                "TableList": {
-                    "shape": "UnfilteredTableList"
-                }
-            },
-            "type": "structure"
-        },
         "BatchGetJobsRequest": {
             "members": {
                 "JobNames": {
                     "shape": "JobNameList"
                 }
             },
             "required": [
@@ -8101,33 +7416,14 @@
                 },
                 "JobsNotFound": {
                     "shape": "JobNameList"
                 }
             },
             "type": "structure"
         },
-        "BatchGetMLTransformRequest": {
-            "members": {
-                "TransformIds": {
-                    "shape": "TransformIds"
-                }
-            },
-            "type": "structure"
-        },
-        "BatchGetMLTransformResponse": {
-            "members": {
-                "MLTransforms": {
-                    "shape": "TransformList"
-                },
-                "MLTransformsNotFound": {
-                    "shape": "TransformIds"
-                }
-            },
-            "type": "structure"
-        },
         "BatchGetPartitionRequest": {
             "members": {
                 "CatalogId": {
                     "shape": "CatalogIdString"
                 },
                 "DatabaseName": {
                     "shape": "NameString"
@@ -8161,35 +7457,81 @@
             "max": 1000,
             "member": {
                 "shape": "PartitionValueList"
             },
             "min": 0,
             "type": "list"
         },
-        "BatchGetTableRequest": {
+        "BatchGetTableOptimizerEntries": {
+            "member": {
+                "shape": "BatchGetTableOptimizerEntry"
+            },
+            "type": "list"
+        },
+        "BatchGetTableOptimizerEntry": {
             "members": {
-                "CatalogId": {
+                "catalogId": {
+                    "shape": "CatalogIdString"
+                },
+                "databaseName": {
+                    "shape": "databaseNameString"
+                },
+                "tableName": {
+                    "shape": "tableNameString"
+                },
+                "type": {
+                    "shape": "TableOptimizerType"
+                }
+            },
+            "type": "structure"
+        },
+        "BatchGetTableOptimizerError": {
+            "members": {
+                "catalogId": {
                     "shape": "CatalogIdString"
                 },
+                "databaseName": {
+                    "shape": "databaseNameString"
+                },
+                "error": {
+                    "shape": "ErrorDetail"
+                },
+                "tableName": {
+                    "shape": "tableNameString"
+                },
+                "type": {
+                    "shape": "TableOptimizerType"
+                }
+            },
+            "type": "structure"
+        },
+        "BatchGetTableOptimizerErrors": {
+            "member": {
+                "shape": "BatchGetTableOptimizerError"
+            },
+            "type": "list"
+        },
+        "BatchGetTableOptimizerRequest": {
+            "members": {
                 "Entries": {
-                    "shape": "BatchTableRequestEntryList"
+                    "shape": "BatchGetTableOptimizerEntries"
                 }
             },
             "required": [
                 "Entries"
             ],
             "type": "structure"
         },
-        "BatchGetTableResponse": {
+        "BatchGetTableOptimizerResponse": {
             "members": {
-                "Errors": {
-                    "shape": "BatchTableErrorList"
+                "Failures": {
+                    "shape": "BatchGetTableOptimizerErrors"
                 },
-                "TableList": {
-                    "shape": "BatchTableResponseList"
+                "TableOptimizers": {
+                    "shape": "BatchTableOptimizers"
                 }
             },
             "type": "structure"
         },
         "BatchGetTriggersRequest": {
             "members": {
                 "TriggerNames": {
@@ -8309,83 +7651,34 @@
         },
         "BatchStopJobRunSuccessfulSubmissionList": {
             "member": {
                 "shape": "BatchStopJobRunSuccessfulSubmission"
             },
             "type": "list"
         },
-        "BatchTableError": {
+        "BatchTableOptimizer": {
             "members": {
-                "Entry": {
-                    "shape": "BatchTableRequestEntry"
-                },
-                "Error": {
-                    "shape": "ErrorDetail"
-                }
-            },
-            "type": "structure"
-        },
-        "BatchTableErrorList": {
-            "max": 100,
-            "member": {
-                "shape": "BatchTableError"
-            },
-            "type": "list"
-        },
-        "BatchTableRequestEntry": {
-            "members": {
-                "ContextMap": {
-                    "shape": "RequestContextMap"
-                },
-                "DatabaseName": {
-                    "shape": "NameString"
-                },
-                "Id": {
-                    "shape": "Identifier"
-                },
-                "Name": {
-                    "shape": "NameString"
+                "catalogId": {
+                    "shape": "CatalogIdString"
                 },
-                "QueryAsOfTime": {
-                    "shape": "Timestamp"
+                "databaseName": {
+                    "shape": "databaseNameString"
                 },
-                "TransactionId": {
-                    "shape": "TransactionIdString"
-                }
-            },
-            "required": [
-                "Id",
-                "DatabaseName",
-                "Name"
-            ],
-            "type": "structure"
-        },
-        "BatchTableRequestEntryList": {
-            "max": 100,
-            "member": {
-                "shape": "BatchTableRequestEntry"
-            },
-            "min": 1,
-            "type": "list"
-        },
-        "BatchTableResponseEntry": {
-            "members": {
-                "Table": {
-                    "shape": "Table"
+                "tableName": {
+                    "shape": "tableNameString"
                 },
-                "UseAdvancedFiltering": {
-                    "internalonly": true,
-                    "shape": "BooleanNullable"
+                "tableOptimizer": {
+                    "shape": "TableOptimizer"
                 }
             },
             "type": "structure"
         },
-        "BatchTableResponseList": {
+        "BatchTableOptimizers": {
             "member": {
-                "shape": "BatchTableResponseEntry"
+                "shape": "BatchTableOptimizer"
             },
             "type": "list"
         },
         "BatchUpdatePartitionFailureEntry": {
             "members": {
                 "ErrorDetail": {
                     "shape": "ErrorDetail"
@@ -8545,70 +7838,14 @@
                 },
                 "RunId": {
                     "shape": "IdString"
                 }
             },
             "type": "structure"
         },
-        "BlueprintInstance": {
-            "members": {
-                "BlueprintName": {
-                    "shape": "OrchestrationNameString"
-                },
-                "CompletedOn": {
-                    "shape": "TimestampValue"
-                },
-                "ErrorMessage": {
-                    "shape": "OrchestrationMessageString"
-                },
-                "Name": {
-                    "shape": "OrchestrationNameString"
-                },
-                "Parameters": {
-                    "shape": "BlueprintParameters"
-                },
-                "RoleArn": {
-                    "shape": "OrchestrationIAMRoleArn"
-                },
-                "RollbackErrorMessage": {
-                    "shape": "OrchestrationMessageString"
-                },
-                "StartedOn": {
-                    "shape": "TimestampValue"
-                },
-                "State": {
-                    "shape": "BlueprintInstanceState"
-                },
-                "WorkflowName": {
-                    "shape": "NameString"
-                }
-            },
-            "type": "structure"
-        },
-        "BlueprintInstanceNames": {
-            "member": {
-                "shape": "OrchestrationNameString"
-            },
-            "type": "list"
-        },
-        "BlueprintInstanceState": {
-            "enum": [
-                "CREATING",
-                "CREATED",
-                "CREATION_FAILED",
-                "ROLLING_BACK"
-            ],
-            "type": "string"
-        },
-        "BlueprintInstances": {
-            "member": {
-                "shape": "BlueprintInstance"
-            },
-            "type": "list"
-        },
         "BlueprintNames": {
             "member": {
                 "shape": "OrchestrationNameString"
             },
             "type": "list"
         },
         "BlueprintParameterSpec": {
@@ -8732,17 +7969,21 @@
                 "RunId"
             ],
             "type": "structure"
         },
         "CancelDataQualityRuleRecommendationRunResponse": {
             "members": {
                 "RunId": {
+                    "deprecated": true,
+                    "internalonly": true,
                     "shape": "HashString"
                 },
                 "Status": {
+                    "deprecated": true,
+                    "internalonly": true,
                     "shape": "TaskStatusType"
                 }
             },
             "type": "structure"
         },
         "CancelDataQualityRulesetEvaluationRunRequest": {
             "members": {
@@ -8754,17 +7995,21 @@
                 "RunId"
             ],
             "type": "structure"
         },
         "CancelDataQualityRulesetEvaluationRunResponse": {
             "members": {
                 "RunId": {
+                    "deprecated": true,
+                    "internalonly": true,
                     "shape": "HashString"
                 },
                 "Status": {
+                    "deprecated": true,
+                    "internalonly": true,
                     "shape": "TaskStatusType"
                 }
             },
             "type": "structure"
         },
         "CancelMLTaskRunRequest": {
             "members": {
@@ -8816,15 +8061,16 @@
         "CancelStatementResponse": {
             "members": {},
             "type": "structure"
         },
         "CatalogEncryptionMode": {
             "enum": [
                 "DISABLED",
-                "SSE-KMS"
+                "SSE-KMS",
+                "SSE-KMS-WITH-SERVICE-ROLE"
             ],
             "type": "string"
         },
         "CatalogEntries": {
             "member": {
                 "shape": "CatalogEntry"
             },
@@ -8907,46 +8153,14 @@
         },
         "CatalogTargetList": {
             "member": {
                 "shape": "CatalogTarget"
             },
             "type": "list"
         },
-        "CellAccountIdString": {
-            "type": "string"
-        },
-        "CellEndpointString": {
-            "type": "string"
-        },
-        "CellInfoItem": {
-            "members": {
-                "CellAccountId": {
-                    "shape": "CellAccountIdString"
-                },
-                "CellEndpoint": {
-                    "shape": "CellEndpointString"
-                },
-                "CellIndex": {
-                    "shape": "CellInfoItemString"
-                },
-                "IsClosed": {
-                    "shape": "isCellClosed"
-                }
-            },
-            "type": "structure"
-        },
-        "CellInfoItemList": {
-            "member": {
-                "shape": "CellInfoItem"
-            },
-            "type": "list"
-        },
-        "CellInfoItemString": {
-            "type": "string"
-        },
         "CheckSchemaVersionValidityInput": {
             "members": {
                 "DataFormat": {
                     "shape": "DataFormat"
                 },
                 "SchemaDefinition": {
                     "shape": "SchemaDefinitionString"
@@ -9162,14 +8376,20 @@
         },
         "ColumnList": {
             "member": {
                 "shape": "Column"
             },
             "type": "list"
         },
+        "ColumnNameList": {
+            "member": {
+                "shape": "NameString"
+            },
+            "type": "list"
+        },
         "ColumnNameString": {
             "max": 1024,
             "min": 1,
             "pattern": "[\\u0020-\\uD7FF\\uE000-\\uFFFD\\uD800\\uDC00-\\uDBFF\\uDFFF\\t]*",
             "type": "string"
         },
         "ColumnRowFilter": {
@@ -9277,60 +8497,130 @@
         },
         "ColumnStatisticsErrors": {
             "member": {
                 "shape": "ColumnStatisticsError"
             },
             "type": "list"
         },
-        "ColumnStatisticsForTable": {
+        "ColumnStatisticsList": {
+            "member": {
+                "shape": "ColumnStatistics"
+            },
+            "type": "list"
+        },
+        "ColumnStatisticsState": {
+            "enum": [
+                "STARTING",
+                "RUNNING",
+                "SUCCEEDED",
+                "FAILED",
+                "STOPPED"
+            ],
+            "type": "string"
+        },
+        "ColumnStatisticsTaskNotRunningException": {
+            "exception": true,
             "members": {
-                "ColumnStatisticsList": {
-                    "shape": "ColumnStatisticsList"
-                },
-                "DatabaseName": {
-                    "shape": "NameString"
-                },
-                "TableName": {
-                    "shape": "NameString"
+                "Message": {
+                    "shape": "MessageString"
                 }
             },
             "type": "structure"
         },
-        "ColumnStatisticsForTableError": {
+        "ColumnStatisticsTaskRun": {
             "members": {
-                "ColumnErrors": {
-                    "shape": "ColumnErrors"
+                "CatalogID": {
+                    "shape": "CatalogIdString"
+                },
+                "ColumnNameList": {
+                    "shape": "ColumnNameList"
+                },
+                "ColumnStatisticsTaskRunId": {
+                    "shape": "HashString"
+                },
+                "CreationTime": {
+                    "shape": "Timestamp"
+                },
+                "CustomerId": {
+                    "shape": "AccountId"
+                },
+                "DPUSeconds": {
+                    "shape": "NonNegativeDouble"
                 },
                 "DatabaseName": {
-                    "shape": "NameString"
+                    "shape": "DatabaseName"
+                },
+                "EndTime": {
+                    "shape": "Timestamp"
+                },
+                "ErrorMessage": {
+                    "shape": "DescriptionString"
+                },
+                "LastUpdated": {
+                    "shape": "Timestamp"
+                },
+                "NumberOfWorkers": {
+                    "shape": "PositiveInteger"
+                },
+                "Role": {
+                    "shape": "Role"
+                },
+                "SampleSize": {
+                    "shape": "SampleSizePercentage"
+                },
+                "SecurityConfiguration": {
+                    "shape": "CrawlerSecurityConfiguration"
+                },
+                "StartTime": {
+                    "shape": "Timestamp"
+                },
+                "Status": {
+                    "shape": "ColumnStatisticsState"
                 },
                 "TableName": {
+                    "shape": "TableName"
+                },
+                "WorkerType": {
                     "shape": "NameString"
                 }
             },
             "type": "structure"
         },
-        "ColumnStatisticsForTableErrorList": {
+        "ColumnStatisticsTaskRunIdList": {
+            "max": 100,
             "member": {
-                "shape": "ColumnStatisticsForTableError"
+                "shape": "HashString"
             },
+            "min": 0,
             "type": "list"
         },
-        "ColumnStatisticsForTableList": {
-            "member": {
-                "shape": "ColumnStatisticsForTable"
+        "ColumnStatisticsTaskRunningException": {
+            "exception": true,
+            "members": {
+                "Message": {
+                    "shape": "MessageString"
+                }
             },
-            "type": "list"
+            "type": "structure"
         },
-        "ColumnStatisticsList": {
+        "ColumnStatisticsTaskRunsList": {
             "member": {
-                "shape": "ColumnStatistics"
+                "shape": "ColumnStatisticsTaskRun"
             },
             "type": "list"
         },
+        "ColumnStatisticsTaskStoppingException": {
+            "exception": true,
+            "members": {
+                "Message": {
+                    "shape": "MessageString"
+                }
+            },
+            "type": "structure"
+        },
         "ColumnStatisticsType": {
             "enum": [
                 "BOOLEAN",
                 "DATE",
                 "DECIMAL",
                 "DOUBLE",
                 "LONG",
@@ -9438,14 +8728,46 @@
         },
         "ConditionList": {
             "member": {
                 "shape": "Condition"
             },
             "type": "list"
         },
+        "ConfigValueString": {
+            "max": 128,
+            "min": 1,
+            "pattern": "[a-zA-Z0-9_.-]+",
+            "type": "string"
+        },
+        "ConfigurationMap": {
+            "key": {
+                "shape": "NameString"
+            },
+            "type": "map",
+            "value": {
+                "shape": "ConfigurationObject"
+            }
+        },
+        "ConfigurationObject": {
+            "members": {
+                "AllowedValues": {
+                    "shape": "AllowedValuesStringList"
+                },
+                "DefaultValue": {
+                    "shape": "ConfigValueString"
+                },
+                "MaxValue": {
+                    "shape": "ConfigValueString"
+                },
+                "MinValue": {
+                    "shape": "ConfigValueString"
+                }
+            },
+            "type": "structure"
+        },
         "ConflictException": {
             "exception": true,
             "members": {
                 "Message": {
                     "shape": "MessageString"
                 }
             },
@@ -9466,46 +8788,67 @@
                     "shape": "RecordsCount"
                 }
             },
             "type": "structure"
         },
         "Connection": {
             "members": {
+                "AuthenticationConfiguration": {
+                    "shape": "AuthenticationConfiguration"
+                },
                 "ConnectionProperties": {
                     "shape": "ConnectionProperties"
                 },
                 "ConnectionType": {
                     "shape": "ConnectionType"
                 },
                 "CreationTime": {
                     "shape": "Timestamp"
                 },
                 "Description": {
                     "shape": "DescriptionString"
                 },
+                "LastConnectionValidationTime": {
+                    "shape": "Timestamp"
+                },
+                "LastUpdateStatus": {
+                    "shape": "ConnectionStatus"
+                },
+                "LastUpdateStatusReason": {
+                    "shape": "LongValueString"
+                },
                 "LastUpdatedBy": {
                     "shape": "NameString"
                 },
                 "LastUpdatedTime": {
                     "shape": "Timestamp"
                 },
                 "MatchCriteria": {
                     "shape": "MatchCriteria"
                 },
                 "Name": {
                     "shape": "NameString"
                 },
                 "PhysicalConnectionRequirements": {
                     "shape": "PhysicalConnectionRequirements"
+                },
+                "Status": {
+                    "shape": "ConnectionStatus"
+                },
+                "StatusReason": {
+                    "shape": "LongValueString"
                 }
             },
             "type": "structure"
         },
         "ConnectionInput": {
             "members": {
+                "AuthenticationConfiguration": {
+                    "shape": "AuthenticationConfigurationInput"
+                },
                 "ConnectionProperties": {
                     "shape": "ConnectionProperties"
                 },
                 "ConnectionType": {
                     "shape": "ConnectionType"
                 },
                 "Description": {
@@ -9515,14 +8858,17 @@
                     "shape": "MatchCriteria"
                 },
                 "Name": {
                     "shape": "NameString"
                 },
                 "PhysicalConnectionRequirements": {
                     "shape": "PhysicalConnectionRequirements"
+                },
+                "ValidateCredentials": {
+                    "shape": "Boolean"
                 }
             },
             "required": [
                 "Name",
                 "ConnectionType",
                 "ConnectionProperties"
             ],
@@ -9587,14 +8933,17 @@
                 "KAFKA_SKIP_CUSTOM_CERT_VALIDATION",
                 "KAFKA_CLIENT_KEYSTORE",
                 "KAFKA_CLIENT_KEYSTORE_PASSWORD",
                 "KAFKA_CLIENT_KEY_PASSWORD",
                 "ENCRYPTED_KAFKA_CLIENT_KEYSTORE_PASSWORD",
                 "ENCRYPTED_KAFKA_CLIENT_KEY_PASSWORD",
                 "KAFKA_SASL_MECHANISM",
+                "KAFKA_SASL_PLAIN_USERNAME",
+                "KAFKA_SASL_PLAIN_PASSWORD",
+                "ENCRYPTED_KAFKA_SASL_PLAIN_PASSWORD",
                 "KAFKA_SASL_SCRAM_USERNAME",
                 "KAFKA_SASL_SCRAM_PASSWORD",
                 "KAFKA_SASL_SCRAM_SECRETS_ARN",
                 "ENCRYPTED_KAFKA_SASL_SCRAM_PASSWORD",
                 "KAFKA_SASL_GSSAPI_KEYTAB",
                 "KAFKA_SASL_GSSAPI_KRB5_CONF",
                 "KAFKA_SASL_GSSAPI_SERVICE",
@@ -9606,44 +8955,65 @@
                 "ENDPOINT",
                 "ENDPOINT_TYPE",
                 "ROLE_ARN",
                 "REGION"
             ],
             "type": "string"
         },
+        "ConnectionStatus": {
+            "enum": [
+                "READY",
+                "IN_PROGRESS",
+                "FAILED"
+            ],
+            "type": "string"
+        },
         "ConnectionType": {
             "enum": [
                 "JDBC",
                 "SFTP",
+                "REDSHIFT",
+                "ATHENA",
                 "MONGODB",
                 "KAFKA",
                 "NETWORK",
                 "YARNRESOURCEMANAGER",
                 "MARKETPLACE",
                 "HIVE_METASTORE",
-                "CUSTOM"
+                "CUSTOM",
+                "SALESFORCE"
             ],
             "type": "string"
         },
         "ConnectionsList": {
             "members": {
                 "Connections": {
                     "shape": "OrchestrationStringList"
                 }
             },
             "type": "structure"
         },
+        "ContextKey": {
+            "max": 128,
+            "min": 1,
+            "type": "string"
+        },
         "ContextMapKey": {
             "max": 1024,
             "type": "string"
         },
         "ContextMapValue": {
             "max": 10240,
             "type": "string"
         },
+        "ContextValue": {
+            "max": 256,
+            "min": 0,
+            "type": "string"
+        },
         "ContextWords": {
             "max": 20,
             "member": {
                 "shape": "NameString"
             },
             "min": 1,
             "type": "list"
@@ -9729,14 +9099,17 @@
                 },
                 "LineageConfiguration": {
                     "shape": "LineageConfiguration"
                 },
                 "Name": {
                     "shape": "NameString"
                 },
+                "PIIConfiguration": {
+                    "shape": "PIIConfiguration"
+                },
                 "RecrawlPolicy": {
                     "shape": "RecrawlPolicy"
                 },
                 "Role": {
                     "shape": "Role"
                 },
                 "Schedule": {
@@ -9955,14 +9328,20 @@
                 },
                 "DeltaTargets": {
                     "shape": "DeltaTargetList"
                 },
                 "DynamoDBTargets": {
                     "shape": "DynamoDBTargetList"
                 },
+                "HudiTargets": {
+                    "shape": "HudiTargetList"
+                },
+                "IcebergTargets": {
+                    "shape": "IcebergTargetList"
+                },
                 "JdbcTargets": {
                     "shape": "JdbcTargetList"
                 },
                 "MongoDBTargets": {
                     "shape": "MongoDBTargetList"
                 },
                 "S3Targets": {
@@ -9987,44 +9366,14 @@
         },
         "CrawlsFilterList": {
             "member": {
                 "shape": "CrawlsFilter"
             },
             "type": "list"
         },
-        "CreateBlueprintInstanceRequest": {
-            "members": {
-                "BlueprintName": {
-                    "shape": "OrchestrationNameString"
-                },
-                "Name": {
-                    "shape": "OrchestrationNameString"
-                },
-                "Parameters": {
-                    "shape": "BlueprintParameters"
-                },
-                "RoleArn": {
-                    "shape": "OrchestrationIAMRoleArn"
-                }
-            },
-            "required": [
-                "BlueprintName",
-                "Name",
-                "RoleArn"
-            ],
-            "type": "structure"
-        },
-        "CreateBlueprintInstanceResponse": {
-            "members": {
-                "Name": {
-                    "shape": "OrchestrationNameString"
-                }
-            },
-            "type": "structure"
-        },
         "CreateBlueprintRequest": {
             "members": {
                 "BlueprintLocation": {
                     "shape": "OrchestrationS3Location"
                 },
                 "Description": {
                     "shape": "Generic512CharString"
@@ -10089,15 +9438,19 @@
             },
             "required": [
                 "ConnectionInput"
             ],
             "type": "structure"
         },
         "CreateConnectionResponse": {
-            "members": {},
+            "members": {
+                "CreateConnectionStatus": {
+                    "shape": "ConnectionStatus"
+                }
+            },
             "type": "structure"
         },
         "CreateCrawlerRequest": {
             "members": {
                 "Classifiers": {
                     "shape": "ClassifierNameList"
                 },
@@ -10118,14 +9471,17 @@
                 },
                 "LineageConfiguration": {
                     "shape": "LineageConfiguration"
                 },
                 "Name": {
                     "shape": "NameString"
                 },
+                "PIIConfiguration": {
+                    "shape": "PIIConfiguration"
+                },
                 "RecrawlPolicy": {
                     "shape": "RecrawlPolicy"
                 },
                 "Role": {
                     "shape": "Role"
                 },
                 "Schedule": {
@@ -10182,14 +9538,17 @@
                     "shape": "CsvHeader"
                 },
                 "Name": {
                     "shape": "NameString"
                 },
                 "QuoteSymbol": {
                     "shape": "CsvQuoteSymbol"
+                },
+                "Serde": {
+                    "shape": "CsvSerdeOption"
                 }
             },
             "required": [
                 "Name"
             ],
             "type": "structure"
         },
@@ -10199,14 +9558,17 @@
                     "shape": "ContextWords"
                 },
                 "Name": {
                     "shape": "NameString"
                 },
                 "RegexString": {
                     "shape": "NameString"
+                },
+                "Tags": {
+                    "shape": "TagsMap"
                 }
             },
             "required": [
                 "Name",
                 "RegexString"
             ],
             "type": "structure"
@@ -10249,33 +9611,49 @@
                 "Ruleset"
             ],
             "type": "structure"
         },
         "CreateDataQualityRulesetResponse": {
             "members": {
                 "CreatedOn": {
+                    "deprecated": true,
+                    "internalonly": true,
                     "shape": "Timestamp"
                 },
                 "Description": {
+                    "deprecated": true,
+                    "internalonly": true,
                     "shape": "DescriptionString"
                 },
+                "Identifier": {
+                    "deprecated": true,
+                    "internalonly": true,
+                    "shape": "DataQualityRulesetIdentifier"
+                },
                 "LastModifiedOn": {
+                    "deprecated": true,
+                    "internalonly": true,
                     "shape": "Timestamp"
                 },
                 "Name": {
                     "shape": "NameString"
                 },
                 "RecommendationRunId": {
+                    "deprecated": true,
                     "internalonly": true,
                     "shape": "HashString"
                 },
                 "Ruleset": {
+                    "deprecated": true,
+                    "internalonly": true,
                     "shape": "DataQualityRulesetString"
                 },
                 "TargetTable": {
+                    "deprecated": true,
+                    "internalonly": true,
                     "shape": "DataQualityTargetTable"
                 }
             },
             "type": "structure"
         },
         "CreateDatabaseRequest": {
             "members": {
@@ -10410,29 +9788,14 @@
                 },
                 "ZeppelinRemoteSparkInterpreterPort": {
                     "shape": "IntegerValue"
                 }
             },
             "type": "structure"
         },
-        "CreateFederationProfileRequest": {
-            "members": {
-                "ProfileInput": {
-                    "shape": "FederationProfileInput"
-                }
-            },
-            "required": [
-                "ProfileInput"
-            ],
-            "type": "structure"
-        },
-        "CreateFederationProfileResponse": {
-            "members": {},
-            "type": "structure"
-        },
         "CreateGrokClassifierRequest": {
             "members": {
                 "Classification": {
                     "shape": "Classification"
                 },
                 "CustomPatterns": {
                     "shape": "CustomPatterns"
@@ -10507,14 +9870,17 @@
                 },
                 "ExecutionProperty": {
                     "shape": "ExecutionProperty"
                 },
                 "GlueVersion": {
                     "shape": "GlueVersionString"
                 },
+                "JobMode": {
+                    "shape": "JobMode"
+                },
                 "LogUri": {
                     "shape": "OrchestrationUriString"
                 },
                 "MaxCapacity": {
                     "shape": "NullableDouble"
                 },
                 "MaxRetries": {
@@ -10535,14 +9901,18 @@
                 "NumberOfWorkers": {
                     "shape": "NullableInteger"
                 },
                 "PartitionId": {
                     "internalonly": true,
                     "shape": "TokenString"
                 },
+                "ProfileName": {
+                    "internalonly": true,
+                    "shape": "NameString"
+                },
                 "Role": {
                     "shape": "OrchestrationRoleString"
                 },
                 "SecurityConfiguration": {
                     "shape": "NameString"
                 },
                 "SourceControlDetails": {
@@ -10893,14 +10263,18 @@
                 "NumberOfWorkers": {
                     "shape": "NullableInteger"
                 },
                 "PartitionId": {
                     "internalonly": true,
                     "shape": "TokenString"
                 },
+                "ProfileName": {
+                    "internalonly": true,
+                    "shape": "NameString"
+                },
                 "RequestOrigin": {
                     "shape": "OrchestrationNameString"
                 },
                 "Role": {
                     "shape": "OrchestrationRoleArn"
                 },
                 "SecurityConfiguration": {
@@ -10927,22 +10301,59 @@
             "members": {
                 "Session": {
                     "shape": "Session"
                 }
             },
             "type": "structure"
         },
+        "CreateTableOptimizerRequest": {
+            "members": {
+                "CatalogId": {
+                    "shape": "CatalogIdString"
+                },
+                "DatabaseName": {
+                    "shape": "NameString"
+                },
+                "TableName": {
+                    "shape": "NameString"
+                },
+                "TableOptimizerConfiguration": {
+                    "shape": "TableOptimizerConfiguration"
+                },
+                "Type": {
+                    "shape": "TableOptimizerType"
+                }
+            },
+            "required": [
+                "CatalogId",
+                "DatabaseName",
+                "TableName",
+                "Type",
+                "TableOptimizerConfiguration"
+            ],
+            "type": "structure"
+        },
+        "CreateTableOptimizerResponse": {
+            "members": {},
+            "type": "structure"
+        },
         "CreateTableRequest": {
             "members": {
                 "CatalogId": {
                     "shape": "CatalogIdString"
                 },
+                "ContextMap": {
+                    "shape": "RequestContextMap"
+                },
                 "DatabaseName": {
                     "shape": "NameString"
                 },
+                "OpenTableFormatInput": {
+                    "shape": "OpenTableFormatInput"
+                },
                 "PartitionIndexes": {
                     "shape": "PartitionIndexList"
                 },
                 "TableInput": {
                     "shape": "TableInput"
                 },
                 "Tags": {
@@ -10955,15 +10366,19 @@
             "required": [
                 "DatabaseName",
                 "TableInput"
             ],
             "type": "structure"
         },
         "CreateTableResponse": {
-            "members": {},
+            "members": {
+                "DataParameters": {
+                    "shape": "BlobParametersMap"
+                }
+            },
             "type": "structure"
         },
         "CreateTriggerRequest": {
             "members": {
                 "Actions": {
                     "shape": "ActionList"
                 },
@@ -11009,14 +10424,43 @@
             "members": {
                 "Name": {
                     "shape": "NameString"
                 }
             },
             "type": "structure"
         },
+        "CreateUsageProfileRequest": {
+            "members": {
+                "Configuration": {
+                    "shape": "ProfileConfiguration"
+                },
+                "Description": {
+                    "shape": "DescriptionString"
+                },
+                "ProfileName": {
+                    "shape": "NameString"
+                },
+                "Tags": {
+                    "shape": "TagsMap"
+                }
+            },
+            "required": [
+                "ProfileName",
+                "Configuration"
+            ],
+            "type": "structure"
+        },
+        "CreateUsageProfileResponse": {
+            "members": {
+                "ProfileName": {
+                    "shape": "NameString"
+                }
+            },
+            "type": "structure"
+        },
         "CreateUserDefinedFunctionRequest": {
             "members": {
                 "CatalogId": {
                     "shape": "CatalogIdString"
                 },
                 "DatabaseName": {
                     "shape": "NameString"
@@ -11121,14 +10565,17 @@
                 },
                 "Name": {
                     "shape": "NameString"
                 },
                 "QuoteSymbol": {
                     "shape": "CsvQuoteSymbol"
                 },
+                "Serde": {
+                    "shape": "CsvSerdeOption"
+                },
                 "Version": {
                     "shape": "VersionId"
                 }
             },
             "required": [
                 "Name"
             ],
@@ -11156,14 +10603,41 @@
         },
         "CsvQuoteSymbol": {
             "max": 1,
             "min": 1,
             "pattern": "[^\\r\\n]",
             "type": "string"
         },
+        "CsvSerdeOption": {
+            "enum": [
+                "OpenCSVSerDe",
+                "LazySimpleSerDe",
+                "None"
+            ],
+            "type": "string"
+        },
+        "CustomAuthenticationProperties": {
+            "key": {
+                "shape": "CustomAuthenticationPropertyKey"
+            },
+            "type": "map",
+            "value": {
+                "shape": "CustomAuthenticationPropertyValue"
+            }
+        },
+        "CustomAuthenticationPropertyKey": {
+            "max": 128,
+            "min": 1,
+            "type": "string"
+        },
+        "CustomAuthenticationPropertyValue": {
+            "max": 2048,
+            "min": 1,
+            "type": "string"
+        },
         "CustomDatatypes": {
             "member": {
                 "shape": "NameString"
             },
             "type": "list"
         },
         "CustomEntityType": {
@@ -11200,29 +10674,34 @@
         },
         "CustomPatterns": {
             "max": 16000,
             "min": 0,
             "pattern": "[\\u0020-\\uD7FF\\uE000-\\uFFFD\\uD800\\uDC00-\\uDBFF\\uDFFF\\r\\n\\t]*",
             "type": "string"
         },
-        "CustomerAccountIdString": {
-            "type": "string"
-        },
         "DagEdges": {
             "member": {
                 "shape": "CodeGenEdge"
             },
             "type": "list"
         },
         "DagNodes": {
             "member": {
                 "shape": "CodeGenNode"
             },
             "type": "list"
         },
+        "DataAccessModeEnum": {
+            "enum": [
+                "LakeFormation",
+                "Hybrid",
+                "Other"
+            ],
+            "type": "string"
+        },
         "DataCatalogEncryptionSettings": {
             "members": {
                 "ConnectionPasswordEncryption": {
                     "shape": "ConnectionPasswordEncryption"
                 },
                 "EncryptionAtRest": {
                     "shape": "EncryptionAtRest"
@@ -11247,35 +10726,118 @@
             "type": "structure"
         },
         "DataLakePrincipalString": {
             "max": 255,
             "min": 1,
             "type": "string"
         },
+        "DataQualityAnalyzerResult": {
+            "members": {
+                "Description": {
+                    "shape": "DataQualityRuleResultDescription"
+                },
+                "EvaluatedMetrics": {
+                    "shape": "EvaluatedMetricsMap"
+                },
+                "EvaluationMessage": {
+                    "shape": "DataQualityRuleResultDescription"
+                },
+                "Name": {
+                    "shape": "NameString"
+                }
+            },
+            "type": "structure"
+        },
+        "DataQualityAnalyzerResults": {
+            "max": 2000,
+            "member": {
+                "shape": "DataQualityAnalyzerResult"
+            },
+            "min": 0,
+            "type": "list"
+        },
         "DataQualityEvaluationRunAdditionalRunOptions": {
             "members": {
+                "CloudWatchMetricsEnabled": {
+                    "shape": "NullableBoolean"
+                },
                 "PublishCloudwatchMetrics": {
+                    "internalonly": true,
                     "shape": "NullableBoolean"
                 },
                 "ResultsS3Path": {
+                    "deprecated": true,
+                    "shape": "UriString"
+                },
+                "ResultsS3Prefix": {
                     "shape": "UriString"
                 }
             },
             "type": "structure"
         },
         "DataQualityEvaluationRunResultExportOptions": {
+            "deprecated": true,
+            "internalonly": true,
             "members": {
                 "ResultsS3Path": {
+                    "deprecated": true,
                     "shape": "UriString"
                 }
             },
             "type": "structure"
         },
+        "DataQualityMetricValues": {
+            "members": {
+                "ActualValue": {
+                    "shape": "NullableDouble"
+                },
+                "ExpectedValue": {
+                    "shape": "NullableDouble"
+                },
+                "LowerLimit": {
+                    "shape": "NullableDouble"
+                },
+                "UpperLimit": {
+                    "shape": "NullableDouble"
+                }
+            },
+            "sensitive": true,
+            "type": "structure"
+        },
+        "DataQualityObservation": {
+            "members": {
+                "Description": {
+                    "shape": "DataQualityObservationDescription"
+                },
+                "MetricBasedObservation": {
+                    "shape": "MetricBasedObservation"
+                }
+            },
+            "type": "structure"
+        },
+        "DataQualityObservationDescription": {
+            "max": 2048,
+            "min": 0,
+            "pattern": "[\\u0020-\\uD7FF\\uE000-\\uFFFD\\uD800\\uDC00-\\uDBFF\\uDFFF\\r\\n\\t]*",
+            "sensitive": true,
+            "type": "string"
+        },
+        "DataQualityObservations": {
+            "max": 50,
+            "member": {
+                "shape": "DataQualityObservation"
+            },
+            "min": 0,
+            "type": "list"
+        },
         "DataQualityResult": {
             "members": {
+                "AnalyzerResults": {
+                    "shape": "DataQualityAnalyzerResults"
+                },
                 "CompletedOn": {
                     "shape": "Timestamp"
                 },
                 "DataSource": {
                     "shape": "DataSource"
                 },
                 "EvaluationContext": {
@@ -11283,23 +10845,31 @@
                 },
                 "JobName": {
                     "shape": "NameString"
                 },
                 "JobRunId": {
                     "shape": "HashString"
                 },
+                "Observations": {
+                    "shape": "DataQualityObservations"
+                },
                 "ResultId": {
                     "shape": "HashString"
                 },
                 "RuleResults": {
                     "shape": "DataQualityRuleResults"
                 },
                 "RulesetEvaluationRunId": {
                     "shape": "HashString"
                 },
+                "RulesetIdentifier": {
+                    "deprecated": true,
+                    "internalonly": true,
+                    "shape": "DataQualityRulesetIdentifier"
+                },
                 "RulesetName": {
                     "shape": "NameString"
                 },
                 "Score": {
                     "shape": "GenericBoundedDouble"
                 },
                 "StartedOn": {
@@ -11393,55 +10963,77 @@
             },
             "type": "structure"
         },
         "DataQualityRuleRecommendationRunFilter": {
             "members": {
                 "DataSource": {
                     "shape": "DataSource"
+                },
+                "StartedAfter": {
+                    "shape": "Timestamp"
+                },
+                "StartedBefore": {
+                    "shape": "Timestamp"
                 }
             },
+            "required": [
+                "DataSource"
+            ],
             "type": "structure"
         },
         "DataQualityRuleRecommendationRunList": {
             "member": {
                 "shape": "DataQualityRuleRecommendationRunDescription"
             },
             "type": "list"
         },
         "DataQualityRuleResult": {
             "members": {
                 "Description": {
-                    "shape": "DescriptionString"
+                    "shape": "DataQualityRuleResultDescription"
+                },
+                "EvaluatedMetrics": {
+                    "shape": "EvaluatedMetricsMap"
+                },
+                "EvaluatedRule": {
+                    "shape": "DataQualityRuleResultDescription"
                 },
                 "EvaluationMessage": {
-                    "shape": "DescriptionString"
+                    "shape": "DataQualityRuleResultDescription"
                 },
                 "Name": {
                     "shape": "NameString"
                 },
                 "Result": {
                     "shape": "DataQualityRuleResultStatus"
                 }
             },
             "type": "structure"
         },
+        "DataQualityRuleResultDescription": {
+            "max": 2048,
+            "min": 0,
+            "pattern": "[\\u0020-\\uD7FF\\uE000-\\uFFFD\\uD800\\uDC00-\\uDBFF\\uDFFF\\r\\n\\t]*",
+            "sensitive": true,
+            "type": "string"
+        },
         "DataQualityRuleResultStatus": {
             "enum": [
                 "PASS",
                 "FAIL",
                 "ERROR"
             ],
             "type": "string"
         },
         "DataQualityRuleResults": {
-            "max": 200,
+            "max": 2000,
             "member": {
                 "shape": "DataQualityRuleResult"
             },
-            "min": 1,
+            "min": 0,
             "type": "list"
         },
         "DataQualityRulesetEvaluationRunDescription": {
             "members": {
                 "DataSource": {
                     "shape": "DataSource"
                 },
@@ -11465,14 +11057,17 @@
                 "StartedAfter": {
                     "shape": "Timestamp"
                 },
                 "StartedBefore": {
                     "shape": "Timestamp"
                 }
             },
+            "required": [
+                "DataSource"
+            ],
             "type": "structure"
         },
         "DataQualityRulesetEvaluationRunList": {
             "member": {
                 "shape": "DataQualityRulesetEvaluationRunDescription"
             },
             "type": "list"
@@ -11484,14 +11079,19 @@
                 },
                 "CreatedBefore": {
                     "shape": "Timestamp"
                 },
                 "Description": {
                     "shape": "DescriptionString"
                 },
+                "Identifier": {
+                    "deprecated": true,
+                    "internalonly": true,
+                    "shape": "DataQualityRulesetIdentifier"
+                },
                 "LastModifiedAfter": {
                     "shape": "Timestamp"
                 },
                 "LastModifiedBefore": {
                     "shape": "Timestamp"
                 },
                 "Name": {
@@ -11500,14 +11100,15 @@
                 "TargetTable": {
                     "shape": "DataQualityTargetTable"
                 }
             },
             "type": "structure"
         },
         "DataQualityRulesetIdentifier": {
+            "internalonly": true,
             "max": 255,
             "min": 1,
             "pattern": "[\\u0020-\\uD7FF\\uE000-\\uFFFD\\uD800\\uDC00-\\uDBFF\\uDFFF\\t]*",
             "type": "string"
         },
         "DataQualityRulesetList": {
             "member": {
@@ -11538,29 +11139,33 @@
                 "TargetTable": {
                     "shape": "DataQualityTargetTable"
                 }
             },
             "type": "structure"
         },
         "DataQualityRulesetString": {
-            "max": 8192,
+            "max": 65536,
             "min": 1,
+            "sensitive": true,
             "type": "string"
         },
         "DataQualityTargetTable": {
             "members": {
+                "CatalogId": {
+                    "shape": "NameString"
+                },
                 "DatabaseName": {
                     "shape": "NameString"
                 },
-                "Name": {
+                "TableName": {
                     "shape": "NameString"
                 }
             },
             "required": [
-                "Name",
+                "TableName",
                 "DatabaseName"
             ],
             "type": "structure"
         },
         "DataSource": {
             "members": {
                 "GlueTable": {
@@ -11568,31 +11173,49 @@
                 }
             },
             "required": [
                 "GlueTable"
             ],
             "type": "structure"
         },
+        "DataSourceMap": {
+            "key": {
+                "shape": "NameString"
+            },
+            "type": "map",
+            "value": {
+                "shape": "DataSource"
+            }
+        },
         "Database": {
             "members": {
                 "CatalogId": {
                     "shape": "CatalogIdString"
                 },
                 "CreateTableDefaultPermissions": {
                     "shape": "PrincipalPermissionsList"
                 },
                 "CreateTime": {
                     "shape": "Timestamp"
                 },
+                "DataParameters": {
+                    "shape": "BlobParametersMap"
+                },
+                "DataProvider": {
+                    "shape": "NameString"
+                },
                 "Description": {
                     "shape": "DescriptionString"
                 },
                 "FederatedDatabase": {
                     "shape": "FederatedDatabase"
                 },
+                "LakeFormationPermissionEnforced": {
+                    "shape": "LakeFormationPermissionEnforcedEnum"
+                },
                 "LocationUri": {
                     "shape": "URI"
                 },
                 "Name": {
                     "shape": "NameString"
                 },
                 "Parameters": {
@@ -11603,14 +11226,29 @@
                 }
             },
             "required": [
                 "Name"
             ],
             "type": "structure"
         },
+        "DatabaseAttributes": {
+            "enum": [
+                "NAME",
+                "DATA_ACCESS_MODE",
+                "DEFAULT",
+                "ALL"
+            ],
+            "type": "string"
+        },
+        "DatabaseAttributesList": {
+            "member": {
+                "shape": "DatabaseAttributes"
+            },
+            "type": "list"
+        },
         "DatabaseIdString": {
             "max": 100,
             "pattern": "[\\u0020-\\uD7FF\\uE000-\\uFFFD\\uD800\\uDC00-\\uDBFF\\uDFFF\\t]*",
             "type": "string"
         },
         "DatabaseIdentifier": {
             "members": {
@@ -11882,20 +11520,25 @@
                 }
             },
             "type": "structure"
         },
         "DeleteDataQualityRulesetRequest": {
             "members": {
                 "Identifier": {
+                    "deprecated": true,
+                    "internalonly": true,
                     "shape": "DataQualityRulesetIdentifier"
                 },
                 "Name": {
                     "shape": "NameString"
                 }
             },
+            "required": [
+                "Name"
+            ],
             "type": "structure"
         },
         "DeleteDataQualityRulesetResponse": {
             "members": {},
             "type": "structure"
         },
         "DeleteDatabaseRequest": {
@@ -11931,29 +11574,14 @@
             ],
             "type": "structure"
         },
         "DeleteDevEndpointResponse": {
             "members": {},
             "type": "structure"
         },
-        "DeleteFederationProfileRequest": {
-            "members": {
-                "Name": {
-                    "shape": "NameString"
-                }
-            },
-            "required": [
-                "Name"
-            ],
-            "type": "structure"
-        },
-        "DeleteFederationProfileResponse": {
-            "members": {},
-            "type": "structure"
-        },
         "DeleteJobRequest": {
             "members": {
                 "JobName": {
                     "shape": "NameString"
                 }
             },
             "required": [
@@ -11965,32 +11593,14 @@
             "members": {
                 "JobName": {
                     "shape": "NameString"
                 }
             },
             "type": "structure"
         },
-        "DeleteLineageNodeRequest": {
-            "members": {
-                "CatalogId": {
-                    "shape": "CatalogIdString"
-                },
-                "Node": {
-                    "shape": "LineageNode"
-                }
-            },
-            "required": [
-                "Node"
-            ],
-            "type": "structure"
-        },
-        "DeleteLineageNodeResponse": {
-            "members": {},
-            "type": "structure"
-        },
         "DeleteMLTransformRequest": {
             "members": {
                 "TransformId": {
                     "shape": "HashString"
                 }
             },
             "required": [
@@ -12182,19 +11792,49 @@
             "members": {
                 "Id": {
                     "shape": "NameString"
                 }
             },
             "type": "structure"
         },
+        "DeleteTableOptimizerRequest": {
+            "members": {
+                "CatalogId": {
+                    "shape": "CatalogIdString"
+                },
+                "DatabaseName": {
+                    "shape": "NameString"
+                },
+                "TableName": {
+                    "shape": "NameString"
+                },
+                "Type": {
+                    "shape": "TableOptimizerType"
+                }
+            },
+            "required": [
+                "CatalogId",
+                "DatabaseName",
+                "TableName",
+                "Type"
+            ],
+            "type": "structure"
+        },
+        "DeleteTableOptimizerResponse": {
+            "members": {},
+            "type": "structure"
+        },
         "DeleteTableRequest": {
             "members": {
                 "CatalogId": {
                     "shape": "CatalogIdString"
                 },
+                "ContextMap": {
+                    "shape": "RequestContextMap"
+                },
                 "DatabaseName": {
                     "shape": "NameString"
                 },
                 "Name": {
                     "shape": "NameString"
                 },
                 "TransactionId": {
@@ -12252,14 +11892,29 @@
             "members": {
                 "Name": {
                     "shape": "NameString"
                 }
             },
             "type": "structure"
         },
+        "DeleteUsageProfileRequest": {
+            "members": {
+                "ProfileName": {
+                    "shape": "NameString"
+                }
+            },
+            "required": [
+                "ProfileName"
+            ],
+            "type": "structure"
+        },
+        "DeleteUsageProfileResponse": {
+            "members": {},
+            "type": "structure"
+        },
         "DeleteUserDefinedFunctionRequest": {
             "members": {
                 "CatalogId": {
                     "shape": "CatalogIdString"
                 },
                 "DatabaseName": {
                     "shape": "NameString"
@@ -12298,14 +11953,17 @@
             "type": "structure"
         },
         "DeltaTarget": {
             "members": {
                 "ConnectionName": {
                     "shape": "ConnectionName"
                 },
+                "CreateNativeDeltaTable": {
+                    "shape": "NullableBoolean"
+                },
                 "DeltaTables": {
                     "shape": "PathList"
                 },
                 "WriteManifest": {
                     "shape": "NullableBoolean"
                 }
             },
@@ -12519,14 +12177,20 @@
         },
         "EdgeList": {
             "member": {
                 "shape": "Edge"
             },
             "type": "list"
         },
+        "EnableAdditionalMetadata": {
+            "member": {
+                "shape": "JdbcMetadataEntry"
+            },
+            "type": "list"
+        },
         "EnableHybridValues": {
             "enum": [
                 "TRUE",
                 "FALSE"
             ],
             "type": "string"
         },
@@ -12542,14 +12206,17 @@
             "type": "structure"
         },
         "EncryptionAtRest": {
             "members": {
                 "CatalogEncryptionMode": {
                     "shape": "CatalogEncryptionMode"
                 },
+                "CatalogEncryptionServiceRole": {
+                    "shape": "IAMRoleArn"
+                },
                 "SseAwsKmsKeyId": {
                     "shape": "NameString"
                 }
             },
             "required": [
                 "CatalogEncryptionMode"
             ],
@@ -12593,14 +12260,17 @@
                 "SSE-KMS"
             ],
             "type": "string"
         },
         "EntityNotFoundException": {
             "exception": true,
             "members": {
+                "FromFederationSource": {
+                    "shape": "NullableBoolean"
+                },
                 "Message": {
                     "shape": "MessageString"
                 }
             },
             "type": "structure"
         },
         "EntityType": {
@@ -12609,14 +12279,20 @@
                 "DATABASE",
                 "TABLE",
                 "PARTITION",
                 "COLUMN"
             ],
             "type": "string"
         },
+        "EntityTypesToDetect": {
+            "member": {
+                "shape": "PIIEntityTypes"
+            },
+            "type": "list"
+        },
         "ErrorByName": {
             "key": {
                 "shape": "NameString"
             },
             "type": "map",
             "value": {
                 "shape": "ErrorDetail"
@@ -12646,14 +12322,24 @@
                 }
             },
             "type": "structure"
         },
         "ErrorMessageString": {
             "type": "string"
         },
+        "EvaluatedMetricsMap": {
+            "key": {
+                "shape": "NameString"
+            },
+            "sensitive": true,
+            "type": "map",
+            "value": {
+                "shape": "NullableDouble"
+            }
+        },
         "EvaluationMetrics": {
             "members": {
                 "FillMissingValuesMetrics": {
                     "shape": "FillMissingValuesMetrics"
                 },
                 "FindMatchesMetrics": {
                     "shape": "FindMatchesMetrics"
@@ -12680,22 +12366,14 @@
                 "BatchSize"
             ],
             "type": "structure"
         },
         "EventQueueArn": {
             "type": "string"
         },
-        "EventTarget": {
-            "members": {
-                "WorkflowName": {
-                    "shape": "OrchestrationNameString"
-                }
-            },
-            "type": "structure"
-        },
         "ExecutionClass": {
             "enum": [
                 "FLEX",
                 "STANDARD"
             ],
             "max": 16,
             "type": "string"
@@ -12723,42 +12401,14 @@
             "members": {
                 "OutputS3Path": {
                     "shape": "UriString"
                 }
             },
             "type": "structure"
         },
-        "ExportLineageGraphRequest": {
-            "members": {
-                "CatalogId": {
-                    "shape": "CatalogIdString"
-                },
-                "EndAt": {
-                    "shape": "ISO8601TimestampPrefix"
-                },
-                "NextToken": {
-                    "shape": "Token"
-                },
-                "StartAt": {
-                    "shape": "ISO8601TimestampPrefix"
-                }
-            },
-            "type": "structure"
-        },
-        "ExportLineageGraphResponse": {
-            "members": {
-                "NextToken": {
-                    "shape": "Token"
-                },
-                "Nodes": {
-                    "shape": "LineageNodeList"
-                }
-            },
-            "type": "structure"
-        },
         "FederatedDatabase": {
             "members": {
                 "ConnectionName": {
                     "shape": "NameString"
                 },
                 "Identifier": {
                     "shape": "FederationIdentifier"
@@ -12800,73 +12450,26 @@
         },
         "FederationIdentifier": {
             "max": 512,
             "min": 1,
             "pattern": "[\\u0020-\\uD7FF\\uE000-\\uFFFD\\uD800\\uDC00-\\uDBFF\\uDFFF\\t]*",
             "type": "string"
         },
-        "FederationProfile": {
-            "members": {
-                "ConnectionName": {
-                    "shape": "NameString"
-                },
-                "CreationTime": {
-                    "shape": "Timestamp"
-                },
-                "Description": {
-                    "shape": "DescriptionString"
-                },
-                "Name": {
-                    "shape": "NameString"
-                },
-                "VersionId": {
-                    "shape": "VersionString"
-                }
-            },
-            "required": [
-                "Name",
-                "ConnectionName"
-            ],
-            "type": "structure"
-        },
-        "FederationProfileInput": {
-            "members": {
-                "ConnectionName": {
-                    "shape": "NameString"
-                },
-                "Description": {
-                    "shape": "DescriptionString"
-                },
-                "Name": {
-                    "shape": "NameString"
-                }
-            },
-            "required": [
-                "Name",
-                "ConnectionName"
-            ],
-            "type": "structure"
-        },
-        "FederationProfileList": {
-            "max": 100,
-            "member": {
-                "shape": "FederationProfile"
-            },
-            "type": "list"
-        },
         "FederationSourceErrorCode": {
             "enum": [
                 "AccessDeniedException",
-                "ThrottlingException",
+                "EntityNotFoundException",
+                "InvalidCredentialsException",
                 "InvalidInputException",
                 "InvalidResponseException",
-                "EntityNotFoundException",
                 "OperationTimeoutException",
                 "OperationNotSupportedException",
-                "InternalServiceException"
+                "InternalServiceException",
+                "PartialFailureException",
+                "ThrottlingException"
             ],
             "type": "string"
         },
         "FederationSourceException": {
             "exception": true,
             "members": {
                 "FederationSourceErrorCode": {
@@ -12874,14 +12477,23 @@
                 },
                 "Message": {
                     "shape": "MessageString"
                 }
             },
             "type": "structure"
         },
+        "FederationSourceRetryableException": {
+            "exception": true,
+            "members": {
+                "Message": {
+                    "shape": "MessageString"
+                }
+            },
+            "type": "structure"
+        },
         "FieldName": {
             "enum": [
                 "CRAWL_ID",
                 "STATE",
                 "START_TIME",
                 "END_TIME",
                 "DPU_HOUR"
@@ -12907,22 +12519,14 @@
                 }
             },
             "required": [
                 "TargetColumnName"
             ],
             "type": "structure"
         },
-        "FilterLevel": {
-            "enum": [
-                "PARTIAL",
-                "NONE",
-                "COMPLETE"
-            ],
-            "type": "string"
-        },
         "FilterOperator": {
             "enum": [
                 "GT",
                 "GE",
                 "LT",
                 "LE",
                 "EQ",
@@ -13062,37 +12666,14 @@
             "value": {
                 "shape": "GenericString"
             }
         },
         "GenericString": {
             "type": "string"
         },
-        "GetBlueprintInstanceRequest": {
-            "members": {
-                "BlueprintName": {
-                    "shape": "OrchestrationNameString"
-                },
-                "Name": {
-                    "shape": "OrchestrationNameString"
-                }
-            },
-            "required": [
-                "Name",
-                "BlueprintName"
-            ],
-            "type": "structure"
-        },
-        "GetBlueprintInstanceResponse": {
-            "members": {
-                "BlueprintInstance": {
-                    "shape": "BlueprintInstance"
-                }
-            },
-            "type": "structure"
-        },
         "GetBlueprintRequest": {
             "members": {
                 "IncludeBlueprint": {
                     "shape": "NullableBoolean"
                 },
                 "IncludeParameterSpec": {
                     "shape": "NullableBoolean"
@@ -13189,33 +12770,14 @@
             "members": {
                 "ImportStatus": {
                     "shape": "CatalogImportStatus"
                 }
             },
             "type": "structure"
         },
-        "GetCellInfoRequest": {
-            "members": {
-                "CustomerAccountId": {
-                    "shape": "CustomerAccountIdString"
-                }
-            },
-            "required": [
-                "CustomerAccountId"
-            ],
-            "type": "structure"
-        },
-        "GetCellInfoResponse": {
-            "members": {
-                "Cells": {
-                    "shape": "CellInfoItemList"
-                }
-            },
-            "type": "structure"
-        },
         "GetClassifierRequest": {
             "members": {
                 "Name": {
                     "shape": "NameString"
                 }
             },
             "required": [
@@ -13259,26 +12821,35 @@
                 "shape": "NameString"
             },
             "min": 0,
             "type": "list"
         },
         "GetColumnStatisticsForPartitionRequest": {
             "members": {
+                "AllColumnsRequested": {
+                    "shape": "NullableBoolean"
+                },
                 "CatalogId": {
                     "shape": "CatalogIdString"
                 },
                 "ColumnNames": {
                     "shape": "GetColumnNamesList"
                 },
                 "DatabaseName": {
                     "shape": "NameString"
                 },
                 "PartitionValues": {
                     "shape": "ValueStringList"
                 },
+                "QuerySessionContext": {
+                    "shape": "QuerySessionContext"
+                },
+                "Region": {
+                    "shape": "ValueString"
+                },
                 "TableName": {
                     "shape": "NameString"
                 }
             },
             "required": [
                 "DatabaseName",
                 "TableName",
@@ -13296,23 +12867,32 @@
                     "shape": "ColumnErrors"
                 }
             },
             "type": "structure"
         },
         "GetColumnStatisticsForTableRequest": {
             "members": {
+                "AllColumnsRequested": {
+                    "shape": "NullableBoolean"
+                },
                 "CatalogId": {
                     "shape": "CatalogIdString"
                 },
                 "ColumnNames": {
                     "shape": "GetColumnNamesList"
                 },
                 "DatabaseName": {
                     "shape": "NameString"
                 },
+                "QuerySessionContext": {
+                    "shape": "QuerySessionContext"
+                },
+                "Region": {
+                    "shape": "ValueString"
+                },
                 "TableName": {
                     "shape": "NameString"
                 }
             },
             "required": [
                 "DatabaseName",
                 "TableName",
@@ -13327,21 +12907,72 @@
                 },
                 "Errors": {
                     "shape": "ColumnErrors"
                 }
             },
             "type": "structure"
         },
+        "GetColumnStatisticsTaskRunRequest": {
+            "members": {
+                "ColumnStatisticsTaskRunId": {
+                    "shape": "HashString"
+                }
+            },
+            "required": [
+                "ColumnStatisticsTaskRunId"
+            ],
+            "type": "structure"
+        },
+        "GetColumnStatisticsTaskRunResponse": {
+            "members": {
+                "ColumnStatisticsTaskRun": {
+                    "shape": "ColumnStatisticsTaskRun"
+                }
+            },
+            "type": "structure"
+        },
+        "GetColumnStatisticsTaskRunsRequest": {
+            "members": {
+                "DatabaseName": {
+                    "shape": "DatabaseName"
+                },
+                "MaxResults": {
+                    "shape": "PageSize"
+                },
+                "NextToken": {
+                    "shape": "Token"
+                },
+                "TableName": {
+                    "shape": "NameString"
+                }
+            },
+            "required": [
+                "DatabaseName",
+                "TableName"
+            ],
+            "type": "structure"
+        },
+        "GetColumnStatisticsTaskRunsResponse": {
+            "members": {
+                "ColumnStatisticsTaskRuns": {
+                    "shape": "ColumnStatisticsTaskRunsList"
+                },
+                "NextToken": {
+                    "shape": "Token"
+                }
+            },
+            "type": "structure"
+        },
         "GetConnectionRequest": {
             "members": {
                 "CatalogId": {
                     "shape": "CatalogIdString"
                 },
                 "HidePassword": {
-                    "shape": "Boolean"
+                    "shape": "BooleanNullable"
                 },
                 "Name": {
                     "shape": "NameString"
                 }
             },
             "required": [
                 "Name"
@@ -13372,15 +13003,15 @@
                 "CatalogId": {
                     "shape": "CatalogIdString"
                 },
                 "Filter": {
                     "shape": "GetConnectionsFilter"
                 },
                 "HidePassword": {
-                    "shape": "Boolean"
+                    "shape": "BooleanNullable"
                 },
                 "MaxResults": {
                     "shape": "PageSize"
                 },
                 "NextToken": {
                     "shape": "Token"
                 }
@@ -13518,14 +13149,17 @@
             "required": [
                 "ResultId"
             ],
             "type": "structure"
         },
         "GetDataQualityResultResponse": {
             "members": {
+                "AnalyzerResults": {
+                    "shape": "DataQualityAnalyzerResults"
+                },
                 "CompletedOn": {
                     "shape": "Timestamp"
                 },
                 "DataSource": {
                     "shape": "DataSource"
                 },
                 "EvaluationContext": {
@@ -13533,23 +13167,34 @@
                 },
                 "JobName": {
                     "shape": "NameString"
                 },
                 "JobRunId": {
                     "shape": "HashString"
                 },
+                "Observations": {
+                    "shape": "DataQualityObservations"
+                },
+                "ProfileId": {
+                    "shape": "HashString"
+                },
                 "ResultId": {
                     "shape": "HashString"
                 },
                 "RuleResults": {
                     "shape": "DataQualityRuleResults"
                 },
                 "RulesetEvaluationRunId": {
                     "shape": "HashString"
                 },
+                "RulesetIdentifier": {
+                    "deprecated": true,
+                    "internalonly": true,
+                    "shape": "DataQualityRulesetIdentifier"
+                },
                 "RulesetName": {
                     "shape": "NameString"
                 },
                 "Score": {
                     "shape": "GenericBoundedDouble"
                 },
                 "StartedOn": {
@@ -13622,14 +13267,17 @@
             "required": [
                 "RunId"
             ],
             "type": "structure"
         },
         "GetDataQualityRulesetEvaluationRunResponse": {
             "members": {
+                "AdditionalDataSources": {
+                    "shape": "DataSourceMap"
+                },
                 "AdditionalRunOptions": {
                     "shape": "DataQualityEvaluationRunAdditionalRunOptions"
                 },
                 "CompletedOn": {
                     "shape": "Timestamp"
                 },
                 "DataSource": {
@@ -13644,22 +13292,28 @@
                 "LastModifiedOn": {
                     "shape": "Timestamp"
                 },
                 "NumberOfWorkers": {
                     "shape": "NullableInteger"
                 },
                 "ResultExportOptions": {
+                    "deprecated": true,
+                    "internalonly": true,
                     "shape": "DataQualityEvaluationRunResultExportOptions"
                 },
                 "ResultIds": {
                     "shape": "DataQualityResultIdList"
                 },
                 "Role": {
                     "shape": "RoleString"
                 },
+                "RulesetIdentifiers": {
+                    "internalonly": true,
+                    "shape": "RulesetIdentifiers"
+                },
                 "RulesetNames": {
                     "shape": "RulesetNames"
                 },
                 "RunId": {
                     "shape": "HashString"
                 },
                 "StartedOn": {
@@ -13673,30 +13327,38 @@
                 }
             },
             "type": "structure"
         },
         "GetDataQualityRulesetRequest": {
             "members": {
                 "Identifier": {
+                    "internalonly": true,
                     "shape": "DataQualityRulesetIdentifier"
                 },
                 "Name": {
                     "shape": "NameString"
                 }
             },
+            "required": [
+                "Name"
+            ],
             "type": "structure"
         },
         "GetDataQualityRulesetResponse": {
             "members": {
                 "CreatedOn": {
                     "shape": "Timestamp"
                 },
                 "Description": {
                     "shape": "DescriptionString"
                 },
+                "Identifier": {
+                    "internalonly": true,
+                    "shape": "DataQualityRulesetIdentifier"
+                },
                 "LastModifiedOn": {
                     "shape": "Timestamp"
                 },
                 "Name": {
                     "shape": "NameString"
                 },
                 "RecommendationRunId": {
@@ -13709,17 +13371,29 @@
                     "shape": "DataQualityTargetTable"
                 }
             },
             "type": "structure"
         },
         "GetDatabaseRequest": {
             "members": {
+                "AttributesToGet": {
+                    "shape": "DatabaseAttributesList"
+                },
                 "CatalogId": {
                     "shape": "CatalogIdString"
                 },
+                "ContextMap": {
+                    "shape": "RequestContextMap"
+                },
+                "FederateToSource": {
+                    "shape": "Boolean"
+                },
+                "IncludeAccessMode": {
+                    "shape": "BooleanNullable"
+                },
                 "Name": {
                     "shape": "NameString"
                 }
             },
             "required": [
                 "Name"
             ],
@@ -13731,20 +13405,26 @@
                     "shape": "Database"
                 }
             },
             "type": "structure"
         },
         "GetDatabasesRequest": {
             "members": {
+                "AttributesToGet": {
+                    "shape": "DatabaseAttributesList"
+                },
                 "CatalogId": {
                     "shape": "CatalogIdString"
                 },
                 "Expression": {
                     "shape": "FilterString"
                 },
+                "IncludeAccessMode": {
+                    "shape": "BooleanNullable"
+                },
                 "MaxResults": {
                     "shape": "CatalogGetterPageSize"
                 },
                 "NextToken": {
                     "shape": "Token"
                 },
                 "ResourceShareType": {
@@ -13831,209 +13511,14 @@
                 },
                 "NextToken": {
                     "shape": "GenericString"
                 }
             },
             "type": "structure"
         },
-        "GetFederationProfileRequest": {
-            "members": {
-                "Name": {
-                    "shape": "NameString"
-                }
-            },
-            "required": [
-                "Name"
-            ],
-            "type": "structure"
-        },
-        "GetFederationProfileResponse": {
-            "members": {
-                "Profile": {
-                    "shape": "FederationProfile"
-                }
-            },
-            "type": "structure"
-        },
-        "GetFederationProfilesRequest": {
-            "members": {
-                "MaxResults": {
-                    "shape": "PageSize"
-                },
-                "NextToken": {
-                    "shape": "Token"
-                }
-            },
-            "type": "structure"
-        },
-        "GetFederationProfilesResponse": {
-            "members": {
-                "NextToken": {
-                    "shape": "Token"
-                },
-                "ProfileList": {
-                    "shape": "FederationProfileList"
-                }
-            },
-            "type": "structure"
-        },
-        "GetInternalUnfilteredPartitionRequest": {
-            "members": {
-                "AuditContext": {
-                    "shape": "AuditContext"
-                },
-                "CatalogId": {
-                    "shape": "CatalogIdString"
-                },
-                "DatabaseName": {
-                    "shape": "NameString"
-                },
-                "PartitionValues": {
-                    "shape": "ValueStringList"
-                },
-                "TableName": {
-                    "shape": "NameString"
-                }
-            },
-            "required": [
-                "DatabaseName",
-                "TableName",
-                "PartitionValues"
-            ],
-            "type": "structure"
-        },
-        "GetInternalUnfilteredPartitionResponse": {
-            "members": {
-                "AuthorizedColumns": {
-                    "shape": "NameStringList"
-                },
-                "IsRegisteredWithLakeFormation": {
-                    "shape": "Boolean"
-                },
-                "Partition": {
-                    "shape": "Partition"
-                }
-            },
-            "type": "structure"
-        },
-        "GetInternalUnfilteredPartitionsRequest": {
-            "members": {
-                "AuditContext": {
-                    "shape": "AuditContext"
-                },
-                "CatalogId": {
-                    "shape": "CatalogIdString"
-                },
-                "DatabaseName": {
-                    "shape": "NameString"
-                },
-                "ExcludeColumnSchema": {
-                    "shape": "BooleanNullable"
-                },
-                "Expression": {
-                    "shape": "PredicateString"
-                },
-                "MaxResults": {
-                    "shape": "PageSize"
-                },
-                "NextToken": {
-                    "shape": "Token"
-                },
-                "QueryAsOfTime": {
-                    "shape": "Timestamp"
-                },
-                "Segment": {
-                    "shape": "Segment"
-                },
-                "TableName": {
-                    "shape": "NameString"
-                },
-                "TransactionId": {
-                    "shape": "TransactionIdString"
-                }
-            },
-            "required": [
-                "DatabaseName",
-                "TableName"
-            ],
-            "type": "structure"
-        },
-        "GetInternalUnfilteredPartitionsResponse": {
-            "members": {
-                "NextToken": {
-                    "shape": "Token"
-                },
-                "PruningLevel": {
-                    "shape": "FilterLevel"
-                },
-                "UnfilteredPartitions": {
-                    "shape": "UnfilteredPartitionList"
-                }
-            },
-            "type": "structure"
-        },
-        "GetInternalUnfilteredTableRequest": {
-            "members": {
-                "AuditContext": {
-                    "shape": "AuditContext"
-                },
-                "CatalogId": {
-                    "shape": "CatalogIdString"
-                },
-                "ContextMap": {
-                    "shape": "RequestContextMap"
-                },
-                "DatabaseName": {
-                    "shape": "NameString"
-                },
-                "Name": {
-                    "shape": "NameString"
-                },
-                "QueryAsOfTime": {
-                    "shape": "Timestamp"
-                },
-                "TransactionId": {
-                    "shape": "TransactionIdString"
-                }
-            },
-            "required": [
-                "DatabaseName",
-                "Name"
-            ],
-            "type": "structure"
-        },
-        "GetInternalUnfilteredTableResponse": {
-            "members": {
-                "AuthorizedColumns": {
-                    "shape": "NameStringList"
-                },
-                "ColumnRowFilters": {
-                    "shape": "ColumnRowFilterList"
-                },
-                "CombinedRowFilter": {
-                    "shape": "PredicateString"
-                },
-                "IsAllowedToViewDataFilters": {
-                    "shape": "Boolean"
-                },
-                "IsRegisteredWithLakeFormation": {
-                    "shape": "Boolean"
-                },
-                "RowFilter": {
-                    "shape": "PredicateString"
-                },
-                "Table": {
-                    "shape": "Table"
-                },
-                "UseAdvancedFiltering": {
-                    "shape": "Boolean"
-                }
-            },
-            "type": "structure"
-        },
         "GetJobBookmarkRequest": {
             "members": {
                 "JobName": {
                     "shape": "JobName"
                 },
                 "RunId": {
                     "shape": "RunId"
@@ -14130,15 +13615,15 @@
         },
         "GetJobRunsRequest": {
             "members": {
                 "JobName": {
                     "shape": "NameString"
                 },
                 "MaxResults": {
-                    "shape": "PageSize"
+                    "shape": "OrchestrationPageSize200"
                 },
                 "NextToken": {
                     "shape": "OrchestrationToken"
                 }
             },
             "required": [
                 "JobName"
@@ -14174,58 +13659,14 @@
                 },
                 "NextToken": {
                     "shape": "OrchestrationToken"
                 }
             },
             "type": "structure"
         },
-        "GetLineageCaptureSettingsRequest": {
-            "members": {
-                "CatalogId": {
-                    "shape": "CatalogIdString"
-                }
-            },
-            "type": "structure"
-        },
-        "GetLineageCaptureSettingsResponse": {
-            "members": {
-                "LineageCaptureState": {
-                    "shape": "LineageCaptureState"
-                }
-            },
-            "type": "structure"
-        },
-        "GetLineageGraphRequest": {
-            "members": {
-                "CatalogId": {
-                    "shape": "CatalogIdString"
-                },
-                "NextToken": {
-                    "shape": "Token"
-                },
-                "Node": {
-                    "shape": "LineageNode"
-                }
-            },
-            "required": [
-                "Node"
-            ],
-            "type": "structure"
-        },
-        "GetLineageGraphResponse": {
-            "members": {
-                "NextToken": {
-                    "shape": "Token"
-                },
-                "Nodes": {
-                    "shape": "LineageNodeList"
-                }
-            },
-            "type": "structure"
-        },
         "GetMLTaskRunRequest": {
             "members": {
                 "TaskRunId": {
                     "shape": "HashString"
                 },
                 "TransformId": {
                     "shape": "HashString"
@@ -14704,33 +14145,14 @@
         },
         "GetResourcePoliciesResponseList": {
             "member": {
                 "shape": "GluePolicy"
             },
             "type": "list"
         },
-        "GetResourcePolicyInternalRequest": {
-            "members": {
-                "InternalId": {
-                    "shape": "RAMInternalId"
-                },
-                "ResourceArn": {
-                    "shape": "RAMResourceARN"
-                }
-            },
-            "type": "structure"
-        },
-        "GetResourcePolicyInternalResponse": {
-            "members": {
-                "Policy": {
-                    "shape": "RAMPolicy"
-                }
-            },
-            "type": "structure"
-        },
         "GetResourcePolicyRequest": {
             "members": {
                 "PrincipalArn": {
                     "shape": "AWSAccountArn"
                 },
                 "ResourceArn": {
                     "shape": "GlueResourceArn"
@@ -14751,36 +14173,14 @@
                 },
                 "UpdateTime": {
                     "shape": "Timestamp"
                 }
             },
             "type": "structure"
         },
-        "GetSaveLocationForTableStatisticsRequest": {
-            "members": {
-                "TaskRunId": {
-                    "shape": "HashString"
-                }
-            },
-            "required": [
-                "TaskRunId"
-            ],
-            "type": "structure"
-        },
-        "GetSaveLocationForTableStatisticsResponse": {
-            "members": {
-                "EncryptionDataKey": {
-                    "shape": "KmsUserDataKey"
-                },
-                "HttpPath": {
-                    "shape": "UriString"
-                }
-            },
-            "type": "structure"
-        },
         "GetSaveLocationForTransformArtifactRequest": {
             "members": {
                 "ArtifactType": {
                     "shape": "ArtifactType"
                 },
                 "CallerSchemeVersion": {
                     "shape": "SchemeVersion"
@@ -14992,18 +14392,24 @@
             "members": {
                 "SecurityConfiguration": {
                     "shape": "SecurityConfiguration"
                 }
             },
             "type": "structure"
         },
+        "GetSecurityConfigurationsPageSize": {
+            "box": true,
+            "max": 200,
+            "min": 1,
+            "type": "integer"
+        },
         "GetSecurityConfigurationsRequest": {
             "members": {
                 "MaxResults": {
-                    "shape": "PageSize"
+                    "shape": "GetSecurityConfigurationsPageSize"
                 },
                 "NextToken": {
                     "shape": "GenericString"
                 }
             },
             "type": "structure"
         },
@@ -15062,126 +14468,92 @@
             "members": {
                 "Statement": {
                     "shape": "Statement"
                 }
             },
             "type": "structure"
         },
-        "GetTableRequest": {
+        "GetTableOptimizerRequest": {
             "members": {
                 "CatalogId": {
                     "shape": "CatalogIdString"
                 },
                 "DatabaseName": {
                     "shape": "NameString"
                 },
-                "Name": {
+                "TableName": {
                     "shape": "NameString"
                 },
-                "QueryAsOfTime": {
-                    "shape": "Timestamp"
-                },
-                "TransactionId": {
-                    "shape": "TransactionIdString"
+                "Type": {
+                    "shape": "TableOptimizerType"
                 }
             },
             "required": [
+                "CatalogId",
                 "DatabaseName",
-                "Name"
+                "TableName",
+                "Type"
             ],
             "type": "structure"
         },
-        "GetTableResponse": {
+        "GetTableOptimizerResponse": {
             "members": {
-                "Table": {
-                    "shape": "Table"
+                "CatalogId": {
+                    "shape": "CatalogIdString"
                 },
-                "UseAdvancedFiltering": {
-                    "internalonly": true,
-                    "shape": "BooleanNullable"
-                }
-            },
-            "type": "structure"
-        },
-        "GetTableStatisticsMetadataRequest": {
-            "members": {
-                "TaskRunId": {
-                    "shape": "HashString"
-                }
-            },
-            "required": [
-                "TaskRunId"
-            ],
-            "type": "structure"
-        },
-        "GetTableStatisticsMetadataResponse": {
-            "members": {
-                "EncryptionDataKey": {
-                    "shape": "KmsUserDataKey"
+                "DatabaseName": {
+                    "shape": "NameString"
                 },
-                "HttpPath": {
-                    "shape": "UriString"
-                }
-            },
-            "type": "structure"
-        },
-        "GetTableStatisticsTaskRunRequest": {
-            "members": {
-                "TaskRunId": {
-                    "shape": "HashString"
+                "TableName": {
+                    "shape": "NameString"
+                },
+                "TableOptimizer": {
+                    "shape": "TableOptimizer"
                 }
             },
-            "required": [
-                "TaskRunId"
-            ],
             "type": "structure"
         },
-        "GetTableStatisticsTaskRunResponse": {
+        "GetTableRequest": {
             "members": {
-                "CatalogId": {
-                    "shape": "NameString"
-                },
-                "CompletedOn": {
-                    "shape": "Timestamp"
+                "AttributesToGet": {
+                    "shape": "TableAttributesList"
                 },
-                "ConnectionName": {
-                    "shape": "NameString"
-                },
-                "CreatedOn": {
-                    "shape": "Timestamp"
+                "CatalogId": {
+                    "shape": "CatalogIdString"
                 },
                 "DatabaseName": {
                     "shape": "NameString"
                 },
-                "ErrorString": {
-                    "shape": "GenericString"
-                },
-                "ExecutionTime": {
-                    "shape": "ExecutionTime"
-                },
-                "LastModifiedOn": {
-                    "shape": "Timestamp"
-                },
-                "LogGroupName": {
-                    "shape": "GenericString"
-                },
-                "Role": {
-                    "shape": "NameString"
+                "IncludeAccessMode": {
+                    "shape": "BooleanNullable"
                 },
-                "SecurityConfiguration": {
+                "Name": {
                     "shape": "NameString"
                 },
-                "Status": {
-                    "shape": "TaskStatusType"
+                "QueryAsOfTime": {
+                    "shape": "Timestamp"
                 },
-                "TableName": {
-                    "shape": "NameString"
+                "TransactionId": {
+                    "shape": "TransactionIdString"
+                }
+            },
+            "required": [
+                "DatabaseName",
+                "Name"
+            ],
+            "type": "structure"
+        },
+        "GetTableResponse": {
+            "members": {
+                "Table": {
+                    "shape": "Table"
                 },
-                "TaskRunId": {
-                    "shape": "HashString"
+                "UseAdvancedFiltering": {
+                    "internalonly": true,
+                    "shape": "BooleanNullable"
                 }
             },
             "type": "structure"
         },
         "GetTableVersionRequest": {
             "members": {
                 "CatalogId": {
@@ -15251,23 +14623,29 @@
                     "shape": "GetTableVersionsList"
                 }
             },
             "type": "structure"
         },
         "GetTablesRequest": {
             "members": {
+                "AttributesToGet": {
+                    "shape": "TableAttributesList"
+                },
                 "CatalogId": {
                     "shape": "CatalogIdString"
                 },
                 "DatabaseName": {
                     "shape": "NameString"
                 },
                 "Expression": {
                     "shape": "FilterString"
                 },
+                "IncludeAccessMode": {
+                    "shape": "BooleanNullable"
+                },
                 "MaxResults": {
                     "shape": "CatalogGetterPageSize"
                 },
                 "NextToken": {
                     "shape": "Token"
                 },
                 "QueryAsOfTime": {
@@ -15289,45 +14667,14 @@
                 },
                 "TableList": {
                     "shape": "TableList"
                 }
             },
             "type": "structure"
         },
-        "GetTaggedResourcesRequest": {
-            "members": {
-                "PaginationToken": {
-                    "shape": "PaginationTokenString"
-                },
-                "ResourceTypeFilters": {
-                    "shape": "ResourceTypeStringList"
-                },
-                "ResourcesPerPage": {
-                    "shape": "ResourcesPerPageInteger"
-                },
-                "TagFilters": {
-                    "shape": "TagFilterList"
-                },
-                "TagsPerPage": {
-                    "shape": "TagsPerPageInteger"
-                }
-            },
-            "type": "structure"
-        },
-        "GetTaggedResourcesResponse": {
-            "members": {
-                "PaginationToken": {
-                    "shape": "PaginationTokenString"
-                },
-                "ResourceTagMappingList": {
-                    "shape": "ResourceTagMappingListObject"
-                }
-            },
-            "type": "structure"
-        },
         "GetTagsRequest": {
             "members": {
                 "ResourceArn": {
                     "shape": "GlueResourceArn"
                 }
             },
             "required": [
@@ -15444,15 +14791,15 @@
         },
         "GetTriggersRequest": {
             "members": {
                 "DependentJobName": {
                     "shape": "NameString"
                 },
                 "MaxResults": {
-                    "shape": "PageSize"
+                    "shape": "OrchestrationPageSize200"
                 },
                 "NextToken": {
                     "shape": "OrchestrationToken"
                 }
             },
             "type": "structure"
         },
@@ -15477,14 +14824,20 @@
                 },
                 "DatabaseName": {
                     "shape": "NameString"
                 },
                 "PartitionValues": {
                     "shape": "ValueStringList"
                 },
+                "QuerySessionContext": {
+                    "shape": "QuerySessionContext"
+                },
+                "Region": {
+                    "shape": "ValueString"
+                },
                 "SupportedPermissionTypes": {
                     "shape": "PermissionTypeList"
                 },
                 "TableName": {
                     "shape": "NameString"
                 }
             },
@@ -15507,53 +14860,14 @@
                 },
                 "Partition": {
                     "shape": "Partition"
                 }
             },
             "type": "structure"
         },
-        "GetUnfilteredPartitionRequest": {
-            "members": {
-                "AuditContext": {
-                    "shape": "AuditContext"
-                },
-                "CatalogId": {
-                    "shape": "CatalogIdString"
-                },
-                "DatabaseName": {
-                    "shape": "NameString"
-                },
-                "PartitionValues": {
-                    "shape": "ValueStringList"
-                },
-                "TableName": {
-                    "shape": "NameString"
-                }
-            },
-            "required": [
-                "CatalogId",
-                "TableName",
-                "PartitionValues"
-            ],
-            "type": "structure"
-        },
-        "GetUnfilteredPartitionResponse": {
-            "members": {
-                "AuthorizedColumns": {
-                    "shape": "NameStringList"
-                },
-                "IsRegisteredWithLakeFormation": {
-                    "shape": "Boolean"
-                },
-                "Partition": {
-                    "shape": "Partition"
-                }
-            },
-            "type": "structure"
-        },
         "GetUnfilteredPartitionsMetadataRequest": {
             "members": {
                 "AuditContext": {
                     "shape": "AuditContext"
                 },
                 "CatalogId": {
                     "shape": "CatalogIdString"
@@ -15566,14 +14880,20 @@
                 },
                 "MaxResults": {
                     "shape": "PageSize"
                 },
                 "NextToken": {
                     "shape": "Token"
                 },
+                "QuerySessionContext": {
+                    "shape": "QuerySessionContext"
+                },
+                "Region": {
+                    "shape": "ValueString"
+                },
                 "Segment": {
                     "shape": "Segment"
                 },
                 "SupportedPermissionTypes": {
                     "shape": "PermissionTypeList"
                 },
                 "TableName": {
@@ -15595,59 +14915,14 @@
                 },
                 "UnfilteredPartitions": {
                     "shape": "UnfilteredPartitionList"
                 }
             },
             "type": "structure"
         },
-        "GetUnfilteredPartitionsRequest": {
-            "members": {
-                "AuditContext": {
-                    "shape": "AuditContext"
-                },
-                "CatalogId": {
-                    "shape": "CatalogIdString"
-                },
-                "DatabaseName": {
-                    "shape": "NameString"
-                },
-                "Expression": {
-                    "shape": "PredicateString"
-                },
-                "MaxResults": {
-                    "shape": "PageSize"
-                },
-                "NextToken": {
-                    "shape": "Token"
-                },
-                "Segment": {
-                    "shape": "Segment"
-                },
-                "TableName": {
-                    "shape": "NameString"
-                }
-            },
-            "required": [
-                "CatalogId",
-                "DatabaseName",
-                "TableName"
-            ],
-            "type": "structure"
-        },
-        "GetUnfilteredPartitionsResponse": {
-            "members": {
-                "NextToken": {
-                    "shape": "Token"
-                },
-                "UnfilteredPartitions": {
-                    "shape": "UnfilteredPartitionList"
-                }
-            },
-            "type": "structure"
-        },
         "GetUnfilteredTableMetadataRequest": {
             "members": {
                 "AuditContext": {
                     "shape": "AuditContext"
                 },
                 "CatalogId": {
                     "shape": "CatalogIdString"
@@ -15657,16 +14932,34 @@
                 },
                 "DatabaseName": {
                     "shape": "NameString"
                 },
                 "Name": {
                     "shape": "NameString"
                 },
+                "Permissions": {
+                    "shape": "PermissionList"
+                },
+                "QuerySessionContext": {
+                    "shape": "QuerySessionContext"
+                },
+                "Region": {
+                    "shape": "ValueString"
+                },
+                "SupportedDialect": {
+                    "shape": "SupportedDialect"
+                },
                 "SupportedPermissionTypes": {
                     "shape": "PermissionTypeList"
+                },
+                "parentResourceArn": {
+                    "shape": "ArnString"
+                },
+                "rootResourceArn": {
+                    "shape": "ArnString"
                 }
             },
             "required": [
                 "CatalogId",
                 "DatabaseName",
                 "Name",
                 "SupportedPermissionTypes"
@@ -15677,63 +14970,65 @@
             "members": {
                 "AuthorizedColumns": {
                     "shape": "NameStringList"
                 },
                 "CellFilters": {
                     "shape": "ColumnRowFilterList"
                 },
+                "IsMultiDialectView": {
+                    "shape": "Boolean"
+                },
+                "IsProtected": {
+                    "shape": "Boolean"
+                },
                 "IsRegisteredWithLakeFormation": {
                     "shape": "Boolean"
                 },
+                "Permissions": {
+                    "shape": "PermissionList"
+                },
+                "QueryAuthorizationId": {
+                    "shape": "HashString"
+                },
+                "ResourceArn": {
+                    "shape": "ArnString"
+                },
                 "Table": {
                     "shape": "Table"
                 }
             },
             "type": "structure"
         },
-        "GetUnfilteredTableRequest": {
+        "GetUsageProfileRequest": {
             "members": {
-                "AuditContext": {
-                    "shape": "AuditContext"
-                },
-                "CatalogId": {
-                    "shape": "CatalogIdString"
-                },
-                "ContextMap": {
-                    "shape": "RequestContextMap"
-                },
-                "DatabaseName": {
-                    "shape": "NameString"
-                },
-                "Name": {
+                "ProfileName": {
                     "shape": "NameString"
-                },
-                "QueryAsOfTime": {
-                    "shape": "Timestamp"
-                },
-                "TransactionId": {
-                    "shape": "TransactionIdString"
                 }
             },
             "required": [
-                "CatalogId",
-                "Name"
+                "ProfileName"
             ],
             "type": "structure"
         },
-        "GetUnfilteredTableResponse": {
+        "GetUsageProfileResponse": {
             "members": {
-                "AuthorizedColumns": {
-                    "shape": "NameStringList"
+                "Configuration": {
+                    "shape": "ProfileConfiguration"
                 },
-                "IsRegisteredWithLakeFormation": {
-                    "shape": "Boolean"
+                "CreatedOn": {
+                    "shape": "TimestampValue"
                 },
-                "Table": {
-                    "shape": "Table"
+                "Description": {
+                    "shape": "DescriptionString"
+                },
+                "LastModifiedOn": {
+                    "shape": "TimestampValue"
+                },
+                "ProfileName": {
+                    "shape": "NameString"
                 }
             },
             "type": "structure"
         },
         "GetUserDefinedFunctionRequest": {
             "members": {
                 "CatalogId": {
@@ -15924,15 +15219,15 @@
                 }
             },
             "type": "structure"
         },
         "GlueResourceArn": {
             "max": 10240,
             "min": 1,
-            "pattern": "arn:(aws|aws-us-gov|aws-cn):glue:.*",
+            "pattern": "arn:aws(-(cn|us-gov|iso(-[bef])?))?:glue:.*",
             "type": "string"
         },
         "GlueTable": {
             "members": {
                 "AdditionalOptions": {
                     "shape": "GlueTableAdditionalOptions"
                 },
@@ -16019,19 +15314,78 @@
         },
         "HashString": {
             "max": 255,
             "min": 1,
             "pattern": "[\\u0020-\\uD7FF\\uE000-\\uFFFD\\uD800\\uDC00-\\uDBFF\\uDFFF\\t]*",
             "type": "string"
         },
-        "ISO8601TimestampPrefix": {
-            "documentation": "A timestamp prefix in ISO 8601 format.",
-            "max": 32,
+        "HudiTarget": {
+            "members": {
+                "ConnectionName": {
+                    "shape": "ConnectionName"
+                },
+                "Exclusions": {
+                    "shape": "PathList"
+                },
+                "MaximumTraversalDepth": {
+                    "shape": "NullableInteger"
+                },
+                "Paths": {
+                    "shape": "PathList"
+                }
+            },
+            "type": "structure"
+        },
+        "HudiTargetList": {
+            "member": {
+                "shape": "HudiTarget"
+            },
+            "type": "list"
+        },
+        "IAMRoleArn": {
+            "pattern": "^arn:aws(-(cn|us-gov|iso(-[bef])?))?:iam::[0-9]{12}:role/.+",
             "type": "string"
         },
+        "IcebergInput": {
+            "members": {
+                "MetadataOperation": {
+                    "shape": "MetadataOperation"
+                },
+                "Version": {
+                    "shape": "VersionString"
+                }
+            },
+            "required": [
+                "MetadataOperation"
+            ],
+            "type": "structure"
+        },
+        "IcebergTarget": {
+            "members": {
+                "ConnectionName": {
+                    "shape": "ConnectionName"
+                },
+                "Exclusions": {
+                    "shape": "PathList"
+                },
+                "MaximumTraversalDepth": {
+                    "shape": "NullableInteger"
+                },
+                "Paths": {
+                    "shape": "PathList"
+                }
+            },
+            "type": "structure"
+        },
+        "IcebergTargetList": {
+            "member": {
+                "shape": "IcebergTarget"
+            },
+            "type": "list"
+        },
         "IdString": {
             "max": 255,
             "min": 1,
             "pattern": "[\\u0020-\\uD7FF\\uE000-\\uFFFD\\uD800\\uDC00-\\uDBFF\\uDFFF\\t]*",
             "type": "string"
         },
         "IdempotentParameterMismatchException": {
@@ -16039,18 +15393,17 @@
             "members": {
                 "Message": {
                     "shape": "MessageString"
                 }
             },
             "type": "structure"
         },
-        "Identifier": {
-            "max": 255,
-            "min": 1,
-            "type": "string"
+        "IdleTimeout": {
+            "box": true,
+            "type": "integer"
         },
         "IllegalBlueprintStateException": {
             "exception": true,
             "members": {
                 "Message": {
                     "shape": "OrchestrationMessageString"
                 }
@@ -16145,14 +15498,17 @@
                 }
             },
             "type": "structure"
         },
         "InvalidInputException": {
             "exception": true,
             "members": {
+                "FromFederationSource": {
+                    "shape": "NullableBoolean"
+                },
                 "Message": {
                     "shape": "MessageString"
                 }
             },
             "type": "structure"
         },
         "InvalidStateException": {
@@ -16163,27 +15519,37 @@
                 }
             },
             "type": "structure"
         },
         "IsVersionValid": {
             "type": "boolean"
         },
+        "JdbcMetadataEntry": {
+            "enum": [
+                "COMMENTS",
+                "RAWTYPES"
+            ],
+            "type": "string"
+        },
         "JdbcTarget": {
             "members": {
                 "ConnectionName": {
                     "shape": "ConnectionName"
                 },
+                "EnableAdditionalMetadata": {
+                    "shape": "EnableAdditionalMetadata"
+                },
                 "Exclusions": {
                     "shape": "PathList"
                 },
                 "Path": {
                     "shape": "Path"
                 },
                 "customJdbcDriverClassName": {
-                    "shape": "NameString"
+                    "shape": "NullableString"
                 },
                 "customJdbcDriverS3Path": {
                     "shape": "Path"
                 }
             },
             "type": "structure"
         },
@@ -16227,14 +15593,17 @@
                 },
                 "ExecutionProperty": {
                     "shape": "ExecutionProperty"
                 },
                 "GlueVersion": {
                     "shape": "GlueVersionString"
                 },
+                "JobMode": {
+                    "shape": "JobMode"
+                },
                 "LastModifiedOn": {
                     "shape": "TimestampValue"
                 },
                 "LogUri": {
                     "shape": "OrchestrationUriString"
                 },
                 "MaxCapacity": {
@@ -16258,14 +15627,17 @@
                 "NumberOfWorkers": {
                     "shape": "NullableInteger"
                 },
                 "PartitionId": {
                     "internalonly": true,
                     "shape": "TokenString"
                 },
+                "ProfileName": {
+                    "shape": "NameString"
+                },
                 "Role": {
                     "shape": "OrchestrationRoleString"
                 },
                 "Running": {
                     "shape": "NullableBoolean"
                 },
                 "SecurityConfiguration": {
@@ -16337,14 +15709,17 @@
             "members": {
                 "Name": {
                     "shape": "JobCommandNameString"
                 },
                 "PythonVersion": {
                     "shape": "PythonVersionString"
                 },
+                "Runtime": {
+                    "shape": "RuntimeNameString"
+                },
                 "ScriptLocation": {
                     "shape": "ScriptLocationString"
                 }
             },
             "type": "structure"
         },
         "JobCommandNameString": {
@@ -16353,14 +15728,22 @@
         },
         "JobList": {
             "member": {
                 "shape": "Job"
             },
             "type": "list"
         },
+        "JobMode": {
+            "enum": [
+                "SCRIPT",
+                "VISUAL",
+                "NOTEBOOK"
+            ],
+            "type": "string"
+        },
         "JobName": {
             "type": "string"
         },
         "JobNameList": {
             "member": {
                 "shape": "NameString"
             },
@@ -16408,14 +15791,17 @@
                 },
                 "GlueVersion": {
                     "shape": "GlueVersionString"
                 },
                 "Id": {
                     "shape": "IdString"
                 },
+                "JobMode": {
+                    "shape": "JobMode"
+                },
                 "JobName": {
                     "shape": "NameString"
                 },
                 "JobRunState": {
                     "shape": "JobRunState"
                 },
                 "LastModifiedOn": {
@@ -16438,20 +15824,26 @@
                 },
                 "PredecessorRuns": {
                     "shape": "PredecessorList"
                 },
                 "PreviousRunId": {
                     "shape": "IdString"
                 },
+                "ProfileName": {
+                    "shape": "NameString"
+                },
                 "SecurityConfiguration": {
                     "shape": "NameString"
                 },
                 "StartedOn": {
                     "shape": "TimestampValue"
                 },
+                "StateDetail": {
+                    "shape": "OrchestrationMessageString"
+                },
                 "Timeout": {
                     "shape": "Timeout"
                 },
                 "TriggerName": {
                     "shape": "NameString"
                 },
                 "WorkerType": {
@@ -16511,14 +15903,17 @@
                 },
                 "ExecutionProperty": {
                     "shape": "ExecutionProperty"
                 },
                 "GlueVersion": {
                     "shape": "GlueVersionString"
                 },
+                "JobMode": {
+                    "shape": "JobMode"
+                },
                 "LogUri": {
                     "shape": "OrchestrationUriString"
                 },
                 "MaxCapacity": {
                     "shape": "NullableDouble"
                 },
                 "MaxRetries": {
@@ -16536,14 +15931,18 @@
                 "NumberOfWorkers": {
                     "shape": "NullableInteger"
                 },
                 "PartitionId": {
                     "internalonly": true,
                     "shape": "TokenString"
                 },
+                "ProfileName": {
+                    "internalonly": true,
+                    "shape": "NameString"
+                },
                 "Role": {
                     "shape": "OrchestrationRoleString"
                 },
                 "SecurityConfiguration": {
                     "shape": "NameString"
                 },
                 "SourceControlDetails": {
@@ -16657,14 +16056,22 @@
                 },
                 "UseLakeFormationCredentials": {
                     "shape": "NullableBoolean"
                 }
             },
             "type": "structure"
         },
+        "LakeFormationPermissionEnforcedEnum": {
+            "enum": [
+                "AllUsers",
+                "SomeUsers",
+                "NoUser"
+            ],
+            "type": "string"
+        },
         "Language": {
             "enum": [
                 "PYTHON",
                 "SCALA"
             ],
             "type": "string"
         },
@@ -16722,171 +16129,30 @@
                 "FAILED"
             ],
             "type": "string"
         },
         "LatestSchemaVersionBoolean": {
             "type": "boolean"
         },
-        "LineageCaptureState": {
-            "documentation": "The value of automatic lineage capture in the AWS Glue Data Catalog.",
-            "enum": [
-                "ENABLED",
-                "DISABLED",
-                "NEVER_ON"
-            ],
-            "type": "string"
-        },
         "LineageConfiguration": {
             "members": {
                 "CrawlerLineageSettings": {
                     "shape": "CrawlerLineageSettings"
                 }
             },
             "type": "structure"
         },
-        "LineageNode": {
-            "documentation": "Denotes a lineage node that represents meta-data about datasets or processes in AWS Glue.",
-            "members": {
-                "Id": {
-                    "shape": "LineageNodeIdentifier"
-                },
-                "Metadata": {
-                    "shape": "LineageNodeMetadata"
-                },
-                "Type": {
-                    "shape": "LineageNodeType"
-                }
-            },
-            "type": "structure"
-        },
-        "LineageNodeIdList": {
-            "documentation": "A list of lineage node identifiers.",
-            "max": 20,
-            "member": {
-                "shape": "LineageNodeIdentifier"
-            },
-            "min": 1,
-            "type": "list"
-        },
-        "LineageNodeIdentifier": {
-            "documentation": "Denotes the unique identifier for a lineage node.",
-            "max": 255,
-            "min": 1,
-            "type": "string"
-        },
-        "LineageNodeIoMapping": {
-            "documentation": "Describes a transform that takes certain inputs and produces certain outputs. Also contains a properties map to store meta-data about the transform.",
-            "members": {
-                "Attributes": {
-                    "shape": "ParametersMap"
-                },
-                "Inputs": {
-                    "shape": "LineageNodeIdList"
-                },
-                "Outputs": {
-                    "shape": "LineageNodeIdList"
-                }
-            },
-            "type": "structure"
-        },
-        "LineageNodeIoMappingList": {
-            "documentation": "The list of transforms performed by a lineage node.",
-            "max": 10,
-            "member": {
-                "shape": "LineageNodeIoMapping"
-            },
-            "type": "list"
-        },
-        "LineageNodeList": {
-            "documentation": "A list of lineage nodes.",
-            "member": {
-                "shape": "LineageNode"
-            },
-            "type": "list"
-        },
-        "LineageNodeMetadata": {
-            "documentation": "Contains the collected meta-data about a lineage node.",
-            "members": {
-                "Attributes": {
-                    "shape": "ParametersMap"
-                },
-                "IoMappings": {
-                    "shape": "LineageNodeIoMappingList"
-                },
-                "Relations": {
-                    "shape": "LineageNodeRelationList"
-                }
-            },
-            "type": "structure"
-        },
-        "LineageNodeRelation": {
-            "documentation": "Denotes a relationship between two lineage nodes.",
-            "members": {
-                "Name": {
-                    "shape": "LineageNodeRelationName"
-                },
-                "Target": {
-                    "shape": "LineageNodeIdentifier"
-                }
-            },
-            "type": "structure"
-        },
-        "LineageNodeRelationList": {
-            "documentation": "A list of relationships of a lineage node.",
-            "max": 20,
-            "member": {
-                "shape": "LineageNodeRelation"
-            },
-            "type": "list"
-        },
-        "LineageNodeRelationName": {
-            "documentation": "The name of the relationship between two lineage nodes.",
-            "max": 100,
-            "type": "string"
-        },
-        "LineageNodeType": {
-            "documentation": "Denotes the type of a lineage node.",
-            "type": "string"
-        },
-        "ListBlueprintInstancesRequest": {
-            "members": {
-                "BlueprintName": {
-                    "shape": "OrchestrationNameString"
-                },
-                "MaxResults": {
-                    "shape": "PageSize"
-                },
-                "NextToken": {
-                    "shape": "OrchestrationToken"
-                }
-            },
-            "required": [
-                "BlueprintName"
-            ],
-            "type": "structure"
-        },
-        "ListBlueprintInstancesResponse": {
-            "members": {
-                "Instances": {
-                    "shape": "BlueprintInstanceNames"
-                },
-                "NextToken": {
-                    "shape": "OrchestrationToken"
-                }
-            },
-            "type": "structure"
-        },
         "ListBlueprintsRequest": {
             "members": {
                 "LFBlueprint": {
                     "internalonly": true,
                     "shape": "NullableBoolean"
                 },
                 "MaxResults": {
-                    "shape": "PageSize"
+                    "shape": "OrchestrationPageSize25"
                 },
                 "NextToken": {
                     "shape": "OrchestrationToken"
                 },
                 "Tags": {
                     "shape": "TagsMap"
                 }
@@ -16900,40 +16166,34 @@
                 },
                 "NextToken": {
                     "shape": "OrchestrationToken"
                 }
             },
             "type": "structure"
         },
-        "ListConsumerAccountsRequest": {
+        "ListColumnStatisticsTaskRunsRequest": {
             "members": {
                 "MaxResults": {
-                    "shape": "RAMMaxResults"
+                    "shape": "PageSize"
                 },
                 "NextToken": {
-                    "shape": "RAMNextToken"
-                },
-                "ResourceType": {
-                    "shape": "RAMResourceType"
+                    "shape": "Token"
                 }
             },
             "type": "structure"
         },
-        "ListConsumerAccountsResponse": {
+        "ListColumnStatisticsTaskRunsResponse": {
             "members": {
-                "AccountIds": {
-                    "shape": "RAMAccountIds"
+                "ColumnStatisticsTaskRunIds": {
+                    "shape": "ColumnStatisticsTaskRunIdList"
                 },
                 "NextToken": {
-                    "shape": "RAMNextToken"
+                    "shape": "Token"
                 }
             },
-            "required": [
-                "AccountIds"
-            ],
             "type": "structure"
         },
         "ListCrawlersRequest": {
             "members": {
                 "MaxResults": {
                     "shape": "PageSize"
                 },
@@ -16991,14 +16251,17 @@
         "ListCustomEntityTypesRequest": {
             "members": {
                 "MaxResults": {
                     "shape": "PageSize"
                 },
                 "NextToken": {
                     "shape": "PaginationToken"
+                },
+                "Tags": {
+                    "shape": "TagsMap"
                 }
             },
             "type": "structure"
         },
         "ListCustomEntityTypesResponse": {
             "members": {
                 "CustomEntityTypes": {
@@ -17218,42 +16481,14 @@
                 },
                 "Registries": {
                     "shape": "RegistryListDefinition"
                 }
             },
             "type": "structure"
         },
-        "ListResourcesSupportPolicyRequest": {
-            "members": {
-                "MaxResults": {
-                    "shape": "RAMMaxResults"
-                },
-                "NextToken": {
-                    "shape": "RAMNextToken"
-                },
-                "ResourceType": {
-                    "shape": "RAMResourceType"
-                }
-            },
-            "type": "structure"
-        },
-        "ListResourcesSupportPolicyResponse": {
-            "members": {
-                "NextToken": {
-                    "shape": "RAMNextToken"
-                },
-                "Resources": {
-                    "shape": "RAMResourceList"
-                }
-            },
-            "required": [
-                "Resources"
-            ],
-            "type": "structure"
-        },
         "ListSchemaVersionsInput": {
             "members": {
                 "MaxResults": {
                     "shape": "MaxResultsNumber"
                 },
                 "NextToken": {
                     "shape": "SchemaRegistryTokenString"
@@ -17301,16 +16536,16 @@
                     "shape": "SchemaListDefinition"
                 }
             },
             "type": "structure"
         },
         "ListSessionsRequest": {
             "members": {
-                "CommandType": {
-                    "shape": "SessionCommand"
+                "Command": {
+                    "shape": "OrchestrationNameString"
                 },
                 "MaxResults": {
                     "shape": "PageSize"
                 },
                 "NextToken": {
                     "shape": "OrchestrationToken"
                 },
@@ -17336,83 +16571,104 @@
                 },
                 "Sessions": {
                     "shape": "SessionList"
                 }
             },
             "type": "structure"
         },
-        "ListSharedResourcesRequest": {
+        "ListStatementsRequest": {
             "members": {
-                "ConsumerAccountId": {
-                    "shape": "RAMAWSAccountId"
-                },
                 "MaxResults": {
-                    "shape": "RAMMaxResults"
+                    "shape": "PageSize"
                 },
                 "NextToken": {
-                    "shape": "RAMNextToken"
+                    "shape": "OrchestrationToken"
                 },
-                "ResourceType": {
-                    "shape": "RAMResourceType"
+                "RequestOrigin": {
+                    "shape": "OrchestrationNameString"
+                },
+                "SessionId": {
+                    "shape": "NameString"
                 }
             },
             "required": [
-                "ConsumerAccountId"
+                "SessionId"
             ],
             "type": "structure"
         },
-        "ListSharedResourcesResponse": {
+        "ListStatementsResponse": {
             "members": {
                 "NextToken": {
-                    "shape": "RAMNextToken"
+                    "shape": "OrchestrationToken"
                 },
-                "VersionedResources": {
-                    "shape": "RAMVersionedSharedResourceList"
+                "Statements": {
+                    "shape": "StatementList"
                 }
             },
-            "required": [
-                "VersionedResources"
-            ],
             "type": "structure"
         },
-        "ListStatementsRequest": {
+        "ListTableOptimizerRunsRequest": {
             "members": {
-                "NextToken": {
-                    "shape": "OrchestrationToken"
+                "CatalogId": {
+                    "shape": "CatalogIdString"
                 },
-                "RequestOrigin": {
-                    "shape": "OrchestrationNameString"
+                "DatabaseName": {
+                    "shape": "NameString"
                 },
-                "SessionId": {
+                "MaxResults": {
+                    "shape": "MaxListTableOptimizerRunsTokenResults"
+                },
+                "NextToken": {
+                    "shape": "ListTableOptimizerRunsToken"
+                },
+                "TableName": {
                     "shape": "NameString"
+                },
+                "Type": {
+                    "shape": "TableOptimizerType"
                 }
             },
             "required": [
-                "SessionId"
+                "CatalogId",
+                "DatabaseName",
+                "TableName",
+                "Type"
             ],
             "type": "structure"
         },
-        "ListStatementsResponse": {
+        "ListTableOptimizerRunsResponse": {
             "members": {
+                "CatalogId": {
+                    "shape": "CatalogIdString"
+                },
+                "DatabaseName": {
+                    "shape": "NameString"
+                },
                 "NextToken": {
-                    "shape": "OrchestrationToken"
+                    "shape": "ListTableOptimizerRunsToken"
                 },
-                "Statements": {
-                    "shape": "StatementList"
+                "TableName": {
+                    "shape": "NameString"
+                },
+                "TableOptimizerRuns": {
+                    "shape": "TableOptimizerRuns"
                 }
             },
             "type": "structure"
         },
+        "ListTableOptimizerRunsToken": {
+            "type": "string"
+        },
         "ListTriggersRequest": {
             "members": {
                 "DependentJobName": {
                     "shape": "NameString"
                 },
                 "MaxResults": {
-                    "shape": "PageSize"
+                    "shape": "OrchestrationPageSize200"
                 },
                 "NextToken": {
                     "shape": "OrchestrationToken"
                 },
                 "Tags": {
                     "shape": "TagsMap"
                 }
@@ -17426,18 +16682,40 @@
                 },
                 "TriggerNames": {
                     "shape": "TriggerNameList"
                 }
             },
             "type": "structure"
         },
+        "ListUsageProfilesRequest": {
+            "members": {
+                "MaxResults": {
+                    "shape": "OrchestrationPageSize200"
+                },
+                "NextToken": {
+                    "shape": "OrchestrationToken"
+                }
+            },
+            "type": "structure"
+        },
+        "ListUsageProfilesResponse": {
+            "members": {
+                "NextToken": {
+                    "shape": "OrchestrationToken"
+                },
+                "Profiles": {
+                    "shape": "UsageProfileDefinitionList"
+                }
+            },
+            "type": "structure"
+        },
         "ListWorkflowsRequest": {
             "members": {
                 "MaxResults": {
-                    "shape": "PageSize"
+                    "shape": "OrchestrationPageSize25"
                 },
                 "NextToken": {
                     "shape": "OrchestrationToken"
                 },
                 "Tags": {
                     "shape": "TagsMap"
                 }
@@ -17547,14 +16825,19 @@
                 "NumberOfDistinctValues"
             ],
             "type": "structure"
         },
         "LongValue": {
             "type": "long"
         },
+        "LongValueString": {
+            "max": 16384,
+            "min": 1,
+            "type": "string"
+        },
         "MLTransform": {
             "members": {
                 "CreatedOn": {
                     "shape": "Timestamp"
                 },
                 "Description": {
                     "shape": "DescriptionString"
@@ -17693,14 +16976,17 @@
             },
             "min": 0,
             "type": "list"
         },
         "MaxConcurrentRuns": {
             "type": "integer"
         },
+        "MaxListTableOptimizerRunsTokenResults": {
+            "type": "integer"
+        },
         "MaxResultsNumber": {
             "box": true,
             "max": 100,
             "min": 1,
             "type": "integer"
         },
         "MaxRetries": {
@@ -17757,23 +17043,64 @@
         },
         "MetadataList": {
             "member": {
                 "shape": "MetadataKeyValuePair"
             },
             "type": "list"
         },
+        "MetadataOperation": {
+            "enum": [
+                "CREATE"
+            ],
+            "type": "string"
+        },
         "MetadataValueString": {
             "max": 256,
             "min": 1,
             "pattern": "[a-zA-Z0-9+-=._./@]+",
             "type": "string"
         },
+        "MetricBasedObservation": {
+            "members": {
+                "MetricName": {
+                    "shape": "NameString"
+                },
+                "MetricValues": {
+                    "shape": "DataQualityMetricValues"
+                },
+                "ModifiedRules": {
+                    "shape": "ModifiedRules"
+                },
+                "NewRules": {
+                    "shape": "NewRules"
+                }
+            },
+            "type": "structure"
+        },
         "MillisecondsCount": {
             "type": "long"
         },
+        "ModifiedRule": {
+            "members": {
+                "source": {
+                    "shape": "NameString"
+                },
+                "target": {
+                    "shape": "NameString"
+                }
+            },
+            "type": "structure"
+        },
+        "ModifiedRules": {
+            "member": {
+                "shape": "ModifiedRule"
+            },
+            "sensitive": true,
+            "type": "list"
+        },
         "MongoDBTarget": {
             "members": {
                 "ConnectionName": {
                     "shape": "ConnectionName"
                 },
                 "Path": {
                     "shape": "Path"
@@ -17798,14 +17125,21 @@
         },
         "NameStringList": {
             "member": {
                 "shape": "NameString"
             },
             "type": "list"
         },
+        "NewRules": {
+            "member": {
+                "shape": "NameString"
+            },
+            "sensitive": true,
+            "type": "list"
+        },
         "NoScheduleException": {
             "exception": true,
             "members": {
                 "Message": {
                     "shape": "MessageString"
                 }
             },
@@ -17875,49 +17209,103 @@
             "type": "structure"
         },
         "NotifyDelayAfter": {
             "box": true,
             "min": 1,
             "type": "integer"
         },
-        "NotifyEventRequest": {
-            "members": {
-                "EventPayload": {
-                    "shape": "GenericMap"
-                },
-                "RuleName": {
-                    "shape": "Generic512CharString"
-                },
-                "Target": {
-                    "shape": "EventTarget"
-                }
-            },
-            "required": [
-                "Target",
-                "RuleName",
-                "EventPayload"
-            ],
-            "type": "structure"
-        },
-        "NotifyEventResponse": {
-            "members": {},
-            "type": "structure"
-        },
         "NullableBoolean": {
             "box": true,
             "type": "boolean"
         },
         "NullableDouble": {
             "box": true,
             "type": "double"
         },
         "NullableInteger": {
             "box": true,
             "type": "integer"
         },
+        "NullableString": {
+            "box": true,
+            "type": "string"
+        },
+        "OAuth2ClientApplication": {
+            "members": {
+                "AWSManagedClientApplicationReference": {
+                    "shape": "AWSManagedClientApplicationReference"
+                },
+                "UserManagedClientApplicationClientId": {
+                    "shape": "UserManagedClientApplicationClientId"
+                }
+            },
+            "type": "structure"
+        },
+        "OAuth2GrantType": {
+            "enum": [
+                "AUTHORIZATION_CODE",
+                "CLIENT_CREDENTIALS",
+                "JWT_BEARER"
+            ],
+            "type": "string"
+        },
+        "OAuth2Properties": {
+            "members": {
+                "OAuth2ClientApplication": {
+                    "shape": "OAuth2ClientApplication"
+                },
+                "OAuth2GrantType": {
+                    "shape": "OAuth2GrantType"
+                },
+                "TokenUrl": {
+                    "shape": "TokenUrl"
+                },
+                "TokenUrlParametersMap": {
+                    "shape": "TokenUrlParametersMap"
+                }
+            },
+            "type": "structure"
+        },
+        "OAuth2PropertiesInput": {
+            "members": {
+                "AuthorizationCodeProperties": {
+                    "shape": "AuthorizationCodeProperties"
+                },
+                "OAuth2ClientApplication": {
+                    "shape": "OAuth2ClientApplication"
+                },
+                "OAuth2GrantType": {
+                    "shape": "OAuth2GrantType"
+                },
+                "TokenUrl": {
+                    "shape": "TokenUrl"
+                },
+                "TokenUrlParametersMap": {
+                    "shape": "TokenUrlParametersMap"
+                }
+            },
+            "type": "structure"
+        },
+        "OpenTableFormatInput": {
+            "members": {
+                "IcebergInput": {
+                    "shape": "IcebergInput"
+                }
+            },
+            "type": "structure"
+        },
+        "OperationNotSupportedException": {
+            "exception": true,
+            "members": {
+                "Message": {
+                    "shape": "MessageString"
+                }
+            },
+            "type": "structure"
+        },
         "OperationTimeoutException": {
             "exception": true,
             "members": {
                 "Message": {
                     "shape": "MessageString"
                 }
             },
@@ -17939,31 +17327,43 @@
             "min": 0,
             "pattern": "[\\u0020-\\uD7FF\\uE000-\\uFFFD\\uD800\\uDC00-\\uDBFF\\uDFFF\\r\\n\\t]*",
             "type": "string"
         },
         "OrchestrationIAMRoleArn": {
             "max": 1024,
             "min": 1,
-            "pattern": "arn:aws[^:]*:iam::[0-9]*:role/.+",
+            "pattern": "arn:aws(-(cn|us-gov|iso(-[bef])?))?:iam::[0-9]*:role/.+",
             "type": "string"
         },
         "OrchestrationMessageString": {
             "max": 400000,
             "type": "string"
         },
         "OrchestrationNameString": {
             "max": 128,
             "min": 1,
             "pattern": "[\\.\\-_A-Za-z0-9]+",
             "type": "string"
         },
+        "OrchestrationPageSize200": {
+            "box": true,
+            "max": 200,
+            "min": 1,
+            "type": "integer"
+        },
+        "OrchestrationPageSize25": {
+            "box": true,
+            "max": 25,
+            "min": 1,
+            "type": "integer"
+        },
         "OrchestrationRoleArn": {
             "max": 2048,
             "min": 20,
-            "pattern": "arn:aws[^:]*:iam::[0-9]*:role/.+",
+            "pattern": "arn:aws(-(cn|us-gov|iso(-[bef])?))?:iam::[0-9]*:role/.+",
             "type": "string"
         },
         "OrchestrationRoleString": {
             "max": 400000,
             "type": "string"
         },
         "OrchestrationS3Location": {
@@ -18024,28 +17424,68 @@
                 },
                 "MetadataValue": {
                     "shape": "MetadataValueString"
                 }
             },
             "type": "structure"
         },
+        "PIIConfiguration": {
+            "members": {
+                "EnablePIIDetection": {
+                    "shape": "NullableBoolean"
+                },
+                "OverrideOnTagConflict": {
+                    "shape": "NullableBoolean"
+                },
+                "PIIEntityTypes": {
+                    "shape": "EntityTypesToDetect"
+                },
+                "PIILFTagMappingName": {
+                    "shape": "NameString"
+                },
+                "SampleSize": {
+                    "shape": "SampleSizePercentage"
+                }
+            },
+            "type": "structure"
+        },
+        "PIIEntityTypes": {
+            "enum": [
+                "ALL",
+                "PERSON_NAME",
+                "DATE",
+                "USA_SSN",
+                "EMAIL",
+                "USA_ITIN",
+                "USA_PASSPORT_NUMBER",
+                "PHONE_NUMBER",
+                "BANK_ACCOUNT",
+                "IP_ADDRESS",
+                "MAC_ADDRESS",
+                "USA_CPT_CODE",
+                "USA_HCPCS_CODE",
+                "USA_NATIONAL_DRUG_CODE",
+                "USA_MEDICARE_BENEFICIARY_IDENTIFIER",
+                "USA_HEALTH_INSURANCE_CLAIM_NUMBER",
+                "CREDIT_CARD",
+                "USA_NATIONAL_PROVIDER_IDENTIFIER",
+                "USA_DEA_NUMBER",
+                "USA_DRIVING_LICENSE"
+            ],
+            "type": "string"
+        },
         "PageSize": {
             "box": true,
             "max": 1000,
             "min": 1,
             "type": "integer"
         },
         "PaginationToken": {
             "type": "string"
         },
-        "PaginationTokenString": {
-            "max": 2048,
-            "min": 1,
-            "type": "string"
-        },
         "ParametersMap": {
             "key": {
                 "shape": "KeyString"
             },
             "type": "map",
             "value": {
                 "shape": "ParametersMapValue"
@@ -18225,30 +17665,36 @@
                 "DROP",
                 "DELETE",
                 "INSERT",
                 "DESCRIBE",
                 "CREATE_DATABASE",
                 "CREATE_TABLE",
                 "DATA_LOCATION_ACCESS",
-                "CREATE_TAG",
-                "ASSOCIATE"
+                "READ",
+                "WRITE",
+                "CREATE_LF_TAG",
+                "ASSOCIATE",
+                "UPDATE",
+                "GRANT_WITH_LF_TAG_EXPRESSION"
             ],
             "type": "string"
         },
         "PermissionList": {
             "member": {
                 "shape": "Permission"
             },
             "type": "list"
         },
         "PermissionType": {
             "enum": [
                 "COLUMN_PERMISSION",
                 "CELL_FILTER_PERMISSION",
-                "TABLE_PERMISSION"
+                "TABLE_PERMISSION",
+                "NESTED_PERMISSION",
+                "NESTED_CELL_PERMISSION"
             ],
             "type": "string"
         },
         "PermissionTypeList": {
             "max": 255,
             "member": {
                 "shape": "PermissionType"
@@ -18299,14 +17745,18 @@
             ],
             "type": "string"
         },
         "PolicyJsonString": {
             "min": 2,
             "type": "string"
         },
+        "PositiveInteger": {
+            "min": 1,
+            "type": "integer"
+        },
         "Predecessor": {
             "members": {
                 "JobName": {
                     "shape": "NameString"
                 },
                 "RunId": {
                     "shape": "IdString"
@@ -18358,14 +17808,25 @@
             "enum": [
                 "USER",
                 "ROLE",
                 "GROUP"
             ],
             "type": "string"
         },
+        "ProfileConfiguration": {
+            "members": {
+                "JobConfiguration": {
+                    "shape": "ConfigurationMap"
+                },
+                "SessionConfiguration": {
+                    "shape": "ConfigurationMap"
+                }
+            },
+            "type": "structure"
+        },
         "PropertyPredicate": {
             "members": {
                 "Comparator": {
                     "shape": "Comparator"
                 },
                 "Key": {
                     "shape": "ValueString"
@@ -18389,14 +17850,17 @@
             "member": {
                 "shape": "GenericString"
             },
             "type": "list"
         },
         "PublishDataQualityResultRequest": {
             "members": {
+                "AnalyzerResults": {
+                    "shape": "DataQualityAnalyzerResults"
+                },
                 "ClientToken": {
                     "shape": "HashString"
                 },
                 "DataSource": {
                     "shape": "DataSource"
                 },
                 "EphemeralRuleset": {
@@ -18416,17 +17880,23 @@
                 },
                 "JobName": {
                     "shape": "NameString"
                 },
                 "JobRunId": {
                     "shape": "HashString"
                 },
+                "Observations": {
+                    "shape": "DataQualityObservations"
+                },
                 "RuleResults": {
                     "shape": "DataQualityRuleResults"
                 },
+                "RulesetIdentifier": {
+                    "shape": "DataQualityRulesetIdentifier"
+                },
                 "RulesetName": {
                     "shape": "HashString"
                 },
                 "Score": {
                     "shape": "GenericBoundedDouble"
                 }
             },
@@ -18593,23 +18063,24 @@
         },
         "PutDataQualityRunMetadataRequest": {
             "members": {
                 "RunId": {
                     "shape": "HashString"
                 },
                 "RunResults": {
-                    "shape": "RunResultsType"
+                    "shape": "DataQualityRulesetString"
                 },
                 "Status": {
+                    "deprecated": true,
+                    "internalonly": true,
                     "shape": "TaskStatusType"
                 }
             },
             "required": [
                 "RunId",
-                "Status",
                 "RunResults"
             ],
             "type": "structure"
         },
         "PutDataQualityRunMetadataResponse": {
             "members": {},
             "type": "structure"
@@ -18667,32 +18138,14 @@
         },
         "PutJobMetadataType": {
             "enum": [
                 "FIND_MATCHES"
             ],
             "type": "string"
         },
-        "PutLineageCaptureSettingsRequest": {
-            "members": {
-                "CatalogId": {
-                    "shape": "CatalogIdString"
-                },
-                "LineageCaptureState": {
-                    "shape": "LineageCaptureState"
-                }
-            },
-            "required": [
-                "LineageCaptureState"
-            ],
-            "type": "structure"
-        },
-        "PutLineageCaptureSettingsResponse": {
-            "members": {},
-            "type": "structure"
-        },
         "PutResourcePolicyRequest": {
             "members": {
                 "EnableHybrid": {
                     "shape": "EnableHybridValues"
                 },
                 "PolicyExistsCondition": {
                     "shape": "ExistCondition"
@@ -18840,186 +18293,34 @@
                 },
                 "SchemaVersionId": {
                     "shape": "SchemaVersionIdString"
                 }
             },
             "type": "structure"
         },
-        "RAMAWSAccountId": {
-            "documentation": "12 digits AWS account ID",
-            "pattern": "\\d{12}",
-            "type": "string"
-        },
-        "RAMAccountIds": {
-            "documentation": "List of AWS account IDs",
-            "member": {
-                "shape": "RAMAWSAccountId"
-            },
-            "type": "list"
-        },
-        "RAMExceptionMessage": {
-            "documentation": "ExceptionMessage return to API caller",
-            "type": "string"
-        },
-        "RAMInternalId": {
-            "documentation": "Internal id for reusable resource ARN",
-            "max": 64,
-            "min": 2,
-            "type": "string"
-        },
-        "RAMInternalIdMismatchException": {
-            "documentation": "InternalId provided by RAM does not match current Internal ID in ROS",
-            "exception": true,
-            "members": {
-                "Message": {
-                    "shape": "RAMExceptionMessage"
-                }
-            },
-            "required": [
-                "Message"
-            ],
-            "type": "structure"
-        },
-        "RAMInvalidSequenceNumberException": {
-            "documentation": "ROS receives a different sequence number than expected",
-            "exception": true,
-            "members": {
-                "Message": {
-                    "shape": "RAMExceptionMessage"
-                }
-            },
-            "required": [
-                "Message"
-            ],
-            "type": "structure"
-        },
-        "RAMMaxResults": {
-            "documentation": "Maximum number of results to return in this page.",
-            "min": 1,
-            "type": "integer"
-        },
-        "RAMNextToken": {
-            "documentation": "The token returned by a previous request to continue paginating through results",
-            "max": 8192,
-            "min": 1,
-            "type": "string"
-        },
-        "RAMPolicy": {
-            "documentation": "Policy document",
-            "type": "string"
-        },
-        "RAMResource": {
-            "documentation": "Unversioned resource",
+        "QuerySessionContext": {
             "members": {
-                "InternalId": {
-                    "shape": "RAMInternalId"
+                "AdditionalContext": {
+                    "shape": "AdditionalContextMap"
                 },
-                "ResourceArn": {
-                    "shape": "RAMResourceARN"
-                }
-            },
-            "type": "structure"
-        },
-        "RAMResourceARN": {
-            "documentation": "AWS resource ARN",
-            "max": 255,
-            "min": 1,
-            "type": "string"
-        },
-        "RAMResourceList": {
-            "documentation": "List of unversioned resource",
-            "member": {
-                "shape": "RAMResource"
-            },
-            "type": "list"
-        },
-        "RAMResourceNotFoundException": {
-            "documentation": "ROS cannot find a resource with the given resource ARN",
-            "exception": true,
-            "members": {
-                "Message": {
-                    "shape": "RAMExceptionMessage"
-                }
-            },
-            "required": [
-                "Message"
-            ],
-            "type": "structure"
-        },
-        "RAMResourceNotSharedException": {
-            "documentation": "ROS receives unshared action when user does not have resource shared",
-            "exception": true,
-            "members": {
-                "Message": {
-                    "shape": "RAMExceptionMessage"
-                }
-            },
-            "required": [
-                "Message"
-            ],
-            "type": "structure"
-        },
-        "RAMResourceType": {
-            "documentation": "Type of resource within an ROS",
-            "max": 256,
-            "min": 1,
-            "type": "string"
-        },
-        "RAMSequenceNumber": {
-            "documentation": "Monotonically increasing sequence where all odd numbers are SHARE actions and all even numbers are UNSHARE actions",
-            "min": 0,
-            "type": "integer"
-        },
-        "RAMSharingAction": {
-            "documentation": "Sharing action: SHARE or UNSHARE",
-            "enum": [
-                "SHARE",
-                "UNSHARE"
-            ],
-            "type": "string"
-        },
-        "RAMValidationMessage": {
-            "documentation": "Detailed information for the validation result. This is currently only consumed by RAM engineers for debugging purposes and is not propagated to customers.",
-            "type": "string"
-        },
-        "RAMValidationResult": {
-            "documentation": "Result of validation, can be one of the following: 1. VALID - The given resource is valid, exists, is owned by the given owner account, has the given internal id (if applicable), and can be shared. 2. RESOURCE_NOT_FOUND - The given resource is invalid, does not exist, does not have the given internal id (if applicable), or is not owned by the given owner account. 3. RESOURCE_CANNOT_BE_SHARED - The given resource is valid, exists, and is owned by the given owner account, but, the resource cannot be shared. This may be due to whitelisting or some other restrictions that the ROS is applying.",
-            "enum": [
-                "VALID",
-                "RESOURCE_NOT_FOUND",
-                "RESOURCE_CANNOT_BE_SHARED"
-            ],
-            "type": "string"
-        },
-        "RAMVersionedSharedResource": {
-            "documentation": "Shared resource ARN and sequence number",
-            "members": {
-                "InternalId": {
-                    "shape": "RAMInternalId"
+                "ClusterId": {
+                    "shape": "NullableString"
+                },
+                "QueryAuthorizationId": {
+                    "shape": "HashString"
                 },
-                "Resource": {
-                    "shape": "RAMResourceARN"
+                "QueryId": {
+                    "shape": "HashString"
                 },
-                "SequenceNumber": {
-                    "shape": "RAMSequenceNumber"
+                "QueryStartTime": {
+                    "shape": "Timestamp"
                 }
             },
-            "required": [
-                "SequenceNumber",
-                "Resource"
-            ],
             "type": "structure"
         },
-        "RAMVersionedSharedResourceList": {
-            "documentation": "List of versioned shared resources",
-            "member": {
-                "shape": "RAMVersionedSharedResource"
-            },
-            "type": "list"
-        },
         "RecordsCount": {
             "box": true,
             "type": "long"
         },
         "RecrawlBehavior": {
             "enum": [
                 "CRAWL_EVERYTHING",
@@ -19032,14 +18333,19 @@
             "members": {
                 "RecrawlBehavior": {
                     "shape": "RecrawlBehavior"
                 }
             },
             "type": "structure"
         },
+        "RedirectUri": {
+            "max": 512,
+            "pattern": "^(https?):\\/\\/[^\\s/$.?#].[^\\s]*$",
+            "type": "string"
+        },
         "RegisterSchemaVersionInput": {
             "members": {
                 "SchemaDefinition": {
                     "shape": "SchemaDefinitionString"
                 },
                 "SchemaId": {
                     "shape": "SchemaId"
@@ -19191,17 +18497,14 @@
             "members": {
                 "JobBookmarkEntry": {
                     "shape": "JobBookmarkEntry"
                 }
             },
             "type": "structure"
         },
-        "ResourceArnString": {
-            "type": "string"
-        },
         "ResourceNotReadyException": {
             "exception": true,
             "members": {
                 "Message": {
                     "shape": "MessageString"
                 }
             },
@@ -19220,54 +18523,22 @@
             "enum": [
                 "FOREIGN",
                 "FEDERATED",
                 "ALL"
             ],
             "type": "string"
         },
-        "ResourceTagMapping": {
-            "members": {
-                "ResourceArn": {
-                    "shape": "ResourceArnString"
-                },
-                "Tags": {
-                    "shape": "ResourceTagMappingTagList"
-                }
-            },
-            "type": "structure"
-        },
-        "ResourceTagMappingListObject": {
-            "member": {
-                "shape": "ResourceTagMapping"
-            },
-            "type": "list"
-        },
-        "ResourceTagMappingTagList": {
-            "member": {
-                "shape": "Tag"
-            },
-            "type": "list"
-        },
         "ResourceType": {
             "enum": [
                 "JAR",
                 "FILE",
                 "ARCHIVE"
             ],
             "type": "string"
         },
-        "ResourceTypeString": {
-            "type": "string"
-        },
-        "ResourceTypeStringList": {
-            "member": {
-                "shape": "ResourceTypeString"
-            },
-            "type": "list"
-        },
         "ResourceUri": {
             "members": {
                 "ResourceType": {
                     "shape": "ResourceType"
                 },
                 "Uri": {
                     "shape": "URI"
@@ -19279,20 +18550,14 @@
             "max": 1000,
             "member": {
                 "shape": "ResourceUri"
             },
             "min": 0,
             "type": "list"
         },
-        "ResourcesPerPageInteger": {
-            "box": true,
-            "max": 50,
-            "min": 1,
-            "type": "integer"
-        },
         "ResumeWorkflowRunRequest": {
             "members": {
                 "Name": {
                     "shape": "NameString"
                 },
                 "NodeIds": {
                     "shape": "NodeIdList"
@@ -19328,29 +18593,50 @@
         },
         "RoleString": {
             "type": "string"
         },
         "RowTag": {
             "type": "string"
         },
+        "RulesetIdentifiers": {
+            "internalonly": true,
+            "max": 10,
+            "member": {
+                "shape": "DataQualityRulesetIdentifier"
+            },
+            "min": 1,
+            "type": "list"
+        },
         "RulesetNames": {
             "max": 10,
             "member": {
                 "shape": "NameString"
             },
             "min": 1,
             "type": "list"
         },
         "RunId": {
             "type": "string"
         },
-        "RunResultsType": {
-            "max": 65536,
-            "min": 1,
-            "type": "string"
+        "RunMetrics": {
+            "members": {
+                "JobDurationInHour": {
+                    "shape": "MessageString"
+                },
+                "NumberOfBytesCompacted": {
+                    "shape": "MessageString"
+                },
+                "NumberOfDpus": {
+                    "shape": "MessageString"
+                },
+                "NumberOfFilesCompacted": {
+                    "shape": "MessageString"
+                }
+            },
+            "type": "structure"
         },
         "RunStatementRequest": {
             "members": {
                 "Code": {
                     "shape": "OrchestrationStatementCodeString"
                 },
                 "RequestOrigin": {
@@ -19370,14 +18656,19 @@
             "members": {
                 "Id": {
                     "shape": "IntegerValue"
                 }
             },
             "type": "structure"
         },
+        "RuntimeNameString": {
+            "max": 64,
+            "pattern": ".*",
+            "type": "string"
+        },
         "S3Encryption": {
             "members": {
                 "KmsKeyArn": {
                     "shape": "KmsKeyArn"
                 },
                 "S3EncryptionMode": {
                     "shape": "S3EncryptionMode"
@@ -19424,14 +18715,19 @@
         },
         "S3TargetList": {
             "member": {
                 "shape": "S3Target"
             },
             "type": "list"
         },
+        "SampleSizePercentage": {
+            "max": 100,
+            "min": 0,
+            "type": "double"
+        },
         "ScalaCode": {
             "type": "string"
         },
         "Schedule": {
             "members": {
                 "ScheduleExpression": {
                     "shape": "CronExpression"
@@ -19710,14 +19006,17 @@
             "members": {
                 "CatalogId": {
                     "shape": "CatalogIdString"
                 },
                 "Filters": {
                     "shape": "SearchPropertyPredicates"
                 },
+                "IncludeAccessMode": {
+                    "shape": "BooleanNullable"
+                },
                 "MaxResults": {
                     "shape": "PageSize"
                 },
                 "NextToken": {
                     "shape": "Token"
                 },
                 "ResourceShareType": {
@@ -19739,14 +19038,18 @@
                 },
                 "TableList": {
                     "shape": "TableList"
                 }
             },
             "type": "structure"
         },
+        "SecretArn": {
+            "pattern": "arn:aws(-(cn|us-gov|iso(-[bef])?))?:secretsmanager:.*",
+            "type": "string"
+        },
         "SecurityConfiguration": {
             "members": {
                 "CreatedTimeStamp": {
                     "shape": "TimestampValue"
                 },
                 "EncryptionConfiguration": {
                     "shape": "EncryptionConfiguration"
@@ -19801,57 +19104,90 @@
             "type": "structure"
         },
         "Session": {
             "members": {
                 "Command": {
                     "shape": "SessionCommand"
                 },
+                "CompletedOn": {
+                    "shape": "TimestampValue"
+                },
                 "Connections": {
                     "shape": "ConnectionsList"
                 },
                 "CreatedOn": {
                     "shape": "TimestampValue"
                 },
+                "DPUSeconds": {
+                    "shape": "NullableDouble"
+                },
                 "DataAccessId": {
                     "internalonly": true,
                     "shape": "TokenString"
                 },
                 "DefaultArguments": {
                     "shape": "OrchestrationArgumentsMap"
                 },
                 "Description": {
                     "shape": "DescriptionString"
                 },
                 "ErrorMessage": {
                     "shape": "DescriptionString"
                 },
+                "ExecutionTime": {
+                    "shape": "NullableDouble"
+                },
                 "GlueVersion": {
                     "shape": "GlueVersionString"
                 },
                 "Id": {
                     "shape": "NameString"
                 },
+                "IdleTimeout": {
+                    "shape": "IdleTimeout"
+                },
                 "MaxCapacity": {
                     "shape": "NullableDouble"
                 },
+                "NumberOfWorkers": {
+                    "shape": "NullableInteger"
+                },
                 "PartitionId": {
                     "internalonly": true,
                     "shape": "TokenString"
                 },
+                "ProfileName": {
+                    "shape": "NameString"
+                },
                 "Progress": {
                     "shape": "DoubleValue"
                 },
                 "Role": {
                     "shape": "OrchestrationRoleArn"
                 },
                 "SecurityConfiguration": {
                     "shape": "NameString"
                 },
                 "Status": {
                     "shape": "SessionStatus"
+                },
+                "Timeout": {
+                    "shape": "Timeout"
+                },
+                "WorkerType": {
+                    "shape": "WorkerType"
+                }
+            },
+            "type": "structure"
+        },
+        "SessionBusyException": {
+            "exception": true,
+            "members": {
+                "Message": {
+                    "shape": "OrchestrationMessageString"
                 }
             },
             "type": "structure"
         },
         "SessionCommand": {
             "members": {
                 "Name": {
@@ -19878,15 +19214,16 @@
         "SessionStatus": {
             "enum": [
                 "PROVISIONING",
                 "READY",
                 "FAILED",
                 "TIMEOUT",
                 "STOPPING",
-                "STOPPED"
+                "STOPPED",
+                "BUSY"
             ],
             "type": "string"
         },
         "SkewedInfo": {
             "members": {
                 "SkewedColumnNames": {
                     "shape": "NameStringList"
@@ -19972,14 +19309,16 @@
                 }
             },
             "type": "structure"
         },
         "SourceControlProvider": {
             "enum": [
                 "GITHUB",
+                "GITLAB",
+                "BITBUCKET",
                 "AWS_CODE_COMMIT"
             ],
             "type": "string"
         },
         "StartBlueprintRunRequest": {
             "members": {
                 "BlueprintName": {
@@ -20006,14 +19345,53 @@
             "members": {
                 "RunId": {
                     "shape": "IdString"
                 }
             },
             "type": "structure"
         },
+        "StartColumnStatisticsTaskRunRequest": {
+            "members": {
+                "CatalogID": {
+                    "shape": "NameString"
+                },
+                "ColumnNameList": {
+                    "shape": "ColumnNameList"
+                },
+                "DatabaseName": {
+                    "shape": "NameString"
+                },
+                "Role": {
+                    "shape": "NameString"
+                },
+                "SampleSize": {
+                    "shape": "SampleSizePercentage"
+                },
+                "SecurityConfiguration": {
+                    "shape": "NameString"
+                },
+                "TableName": {
+                    "shape": "NameString"
+                }
+            },
+            "required": [
+                "DatabaseName",
+                "TableName",
+                "Role"
+            ],
+            "type": "structure"
+        },
+        "StartColumnStatisticsTaskRunResponse": {
+            "members": {
+                "ColumnStatisticsTaskRunId": {
+                    "shape": "HashString"
+                }
+            },
+            "type": "structure"
+        },
         "StartCrawlerRequest": {
             "members": {
                 "Name": {
                     "shape": "NameString"
                 }
             },
             "required": [
@@ -20073,32 +19451,42 @@
                     "shape": "HashString"
                 }
             },
             "type": "structure"
         },
         "StartDataQualityRulesetEvaluationRunRequest": {
             "members": {
+                "AdditionalDataSources": {
+                    "shape": "DataSourceMap"
+                },
                 "AdditionalRunOptions": {
                     "shape": "DataQualityEvaluationRunAdditionalRunOptions"
                 },
                 "ClientToken": {
                     "shape": "HashString"
                 },
                 "DataSource": {
                     "shape": "DataSource"
                 },
                 "NumberOfWorkers": {
                     "shape": "NullableInteger"
                 },
                 "ResultExportOptions": {
+                    "deprecated": true,
+                    "internalonly": true,
                     "shape": "DataQualityEvaluationRunResultExportOptions"
                 },
                 "Role": {
                     "shape": "RoleString"
                 },
+                "RulesetIdentifiers": {
+                    "deprecated": true,
+                    "internalonly": true,
+                    "shape": "RulesetIdentifiers"
+                },
                 "RulesetNames": {
                     "shape": "RulesetNames"
                 },
                 "Timeout": {
                     "shape": "Timeout"
                 }
             },
@@ -20199,14 +19587,18 @@
                 },
                 "NotificationProperty": {
                     "shape": "NotificationProperty"
                 },
                 "NumberOfWorkers": {
                     "shape": "NullableInteger"
                 },
+                "ProfileName": {
+                    "internalonly": true,
+                    "shape": "NameString"
+                },
                 "SecurityConfiguration": {
                     "shape": "NameString"
                 },
                 "Timeout": {
                     "shape": "Timeout"
                 },
                 "WorkerType": {
@@ -20267,56 +19659,14 @@
             "members": {
                 "TaskRunId": {
                     "shape": "HashString"
                 }
             },
             "type": "structure"
         },
-        "StartTableStatisticsTaskRunRequest": {
-            "members": {
-                "CallerReference": {
-                    "shape": "GenericString"
-                },
-                "CatalogId": {
-                    "shape": "NameString"
-                },
-                "ClientToken": {
-                    "shape": "GenericString"
-                },
-                "ConnectionName": {
-                    "shape": "NameString"
-                },
-                "DatabaseName": {
-                    "shape": "NameString"
-                },
-                "Role": {
-                    "shape": "NameString"
-                },
-                "SecurityConfiguration": {
-                    "shape": "NameString"
-                },
-                "TableName": {
-                    "shape": "NameString"
-                }
-            },
-            "required": [
-                "DatabaseName",
-                "TableName",
-                "Role"
-            ],
-            "type": "structure"
-        },
-        "StartTableStatisticsTaskRunResponse": {
-            "members": {
-                "TaskRunId": {
-                    "shape": "HashString"
-                }
-            },
-            "type": "structure"
-        },
         "StartTriggerRequest": {
             "members": {
                 "Name": {
                     "shape": "NameString"
                 }
             },
             "required": [
@@ -20450,14 +19800,33 @@
                 "AVAILABLE",
                 "CANCELLING",
                 "CANCELLED",
                 "ERROR"
             ],
             "type": "string"
         },
+        "StopColumnStatisticsTaskRunRequest": {
+            "members": {
+                "DatabaseName": {
+                    "shape": "DatabaseName"
+                },
+                "TableName": {
+                    "shape": "NameString"
+                }
+            },
+            "required": [
+                "DatabaseName",
+                "TableName"
+            ],
+            "type": "structure"
+        },
+        "StopColumnStatisticsTaskRunResponse": {
+            "members": {},
+            "type": "structure"
+        },
         "StopCrawlerRequest": {
             "members": {
                 "Name": {
                     "shape": "NameString"
                 }
             },
             "required": [
@@ -20616,46 +19985,69 @@
         },
         "StringList": {
             "member": {
                 "shape": "GenericString"
             },
             "type": "list"
         },
+        "SupportedDialect": {
+            "members": {
+                "Dialect": {
+                    "shape": "ViewDialect"
+                },
+                "DialectVersion": {
+                    "shape": "ViewDialectVersionString"
+                }
+            },
+            "type": "structure"
+        },
         "Table": {
             "members": {
                 "CatalogId": {
                     "shape": "CatalogIdString"
                 },
                 "CreateTime": {
                     "shape": "Timestamp"
                 },
                 "CreatedBy": {
                     "shape": "NameString"
                 },
+                "DataAccessMode": {
+                    "shape": "DataAccessModeEnum"
+                },
                 "DataParameters": {
                     "shape": "BlobParametersMap"
                 },
+                "DataProvider": {
+                    "shape": "NameString"
+                },
                 "DatabaseId": {
                     "shape": "DatabaseIdString"
                 },
                 "DatabaseName": {
                     "shape": "NameString"
                 },
                 "Description": {
                     "shape": "DescriptionString"
                 },
                 "FederatedTable": {
                     "shape": "FederatedTable"
                 },
+                "IsMultiDialectView": {
+                    "shape": "NullableBoolean"
+                },
                 "IsRegisteredWithLakeFormation": {
                     "shape": "Boolean"
                 },
                 "IsRowFilteringEnabled": {
                     "shape": "Boolean"
                 },
+                "LakeFormationPermissionEnforced": {
+                    "shape": "LakeFormationPermissionEnforcedEnum"
+                },
                 "LastAccessTime": {
                     "shape": "Timestamp"
                 },
                 "LastAnalyzedTime": {
                     "shape": "Timestamp"
                 },
                 "Name": {
@@ -20672,38 +20064,62 @@
                 },
                 "Retention": {
                     "shape": "NonNegativeInteger"
                 },
                 "StorageDescriptor": {
                     "shape": "StorageDescriptor"
                 },
+                "TableId": {
+                    "shape": "TableIdString"
+                },
                 "TableType": {
                     "shape": "TableTypeString"
                 },
                 "TargetTable": {
                     "shape": "TableIdentifier"
                 },
                 "UpdateTime": {
                     "shape": "Timestamp"
                 },
                 "VersionId": {
                     "shape": "VersionString"
                 },
+                "ViewDefinition": {
+                    "shape": "ViewDefinition"
+                },
                 "ViewExpandedText": {
                     "shape": "ViewTextString"
                 },
                 "ViewOriginalText": {
                     "shape": "ViewTextString"
                 }
             },
             "required": [
                 "Name"
             ],
             "type": "structure"
         },
+        "TableAttributes": {
+            "enum": [
+                "NAME",
+                "VERSION_ID",
+                "DATA_ACCESS_MODE",
+                "DEFAULT",
+                "ALL",
+                "TABLE_TYPE",
+                "DESCRIPTION"
+            ],
+            "type": "string"
+        },
+        "TableAttributesList": {
+            "member": {
+                "shape": "TableAttributes"
+            },
+            "type": "list"
+        },
         "TableError": {
             "members": {
                 "ErrorDetail": {
                     "shape": "ErrorDetail"
                 },
                 "TableName": {
                     "shape": "NameString"
@@ -20713,14 +20129,19 @@
         },
         "TableErrors": {
             "member": {
                 "shape": "TableError"
             },
             "type": "list"
         },
+        "TableIdString": {
+            "max": 100,
+            "pattern": "[\\u0020-\\uD7FF\\uE000-\\uFFFD\\uD800\\uDC00-\\uDBFF\\uDFFF\\t]*",
+            "type": "string"
+        },
         "TableIdentifier": {
             "members": {
                 "CatalogId": {
                     "shape": "CatalogIdString"
                 },
                 "DatabaseId": {
                     "shape": "DatabaseIdString"
@@ -20774,14 +20195,17 @@
                 },
                 "TableType": {
                     "shape": "TableTypeString"
                 },
                 "TargetTable": {
                     "shape": "TableIdentifier"
                 },
+                "ViewDefinition": {
+                    "shape": "ViewDefinitionDDLInput"
+                },
                 "ViewExpandedText": {
                     "shape": "ViewTextString"
                 },
                 "ViewOriginalText": {
                     "shape": "ViewTextString"
                 }
             },
@@ -20795,14 +20219,96 @@
                 "shape": "Table"
             },
             "type": "list"
         },
         "TableName": {
             "type": "string"
         },
+        "TableOptimizer": {
+            "members": {
+                "configuration": {
+                    "shape": "TableOptimizerConfiguration"
+                },
+                "lastRun": {
+                    "shape": "TableOptimizerRun"
+                },
+                "type": {
+                    "shape": "TableOptimizerType"
+                }
+            },
+            "type": "structure"
+        },
+        "TableOptimizerConfiguration": {
+            "members": {
+                "enabled": {
+                    "shape": "NullableBoolean"
+                },
+                "roleArn": {
+                    "shape": "ArnString"
+                },
+                "vpcConfiguration": {
+                    "shape": "TableOptimizerVpcConfiguration"
+                }
+            },
+            "type": "structure"
+        },
+        "TableOptimizerEventType": {
+            "enum": [
+                "starting",
+                "completed",
+                "failed",
+                "in_progress"
+            ],
+            "type": "string"
+        },
+        "TableOptimizerRun": {
+            "members": {
+                "endTimestamp": {
+                    "shape": "TableOptimizerRunTimestamp"
+                },
+                "error": {
+                    "shape": "MessageString"
+                },
+                "eventType": {
+                    "shape": "TableOptimizerEventType"
+                },
+                "metrics": {
+                    "shape": "RunMetrics"
+                },
+                "startTimestamp": {
+                    "shape": "TableOptimizerRunTimestamp"
+                }
+            },
+            "type": "structure"
+        },
+        "TableOptimizerRunTimestamp": {
+            "type": "timestamp"
+        },
+        "TableOptimizerRuns": {
+            "member": {
+                "shape": "TableOptimizerRun"
+            },
+            "type": "list"
+        },
+        "TableOptimizerType": {
+            "enum": [
+                "compaction"
+            ],
+            "type": "string"
+        },
+        "TableOptimizerVpcConfiguration": {
+            "documentation": "The Union of TableOptimizerVpcConfigurations. Only one of them will ever be populated at a given time. See https://w.amazon.com/bin/view/Coral/Model/XML/Traits/#Union for more info on unions in XML.",
+            "members": {
+                "glueConnectionName": {
+                    "shape": "glueConnectionNameString"
+                }
+            },
+            "type": "structure",
+            "union": true
+        },
         "TablePrefix": {
             "max": 128,
             "min": 0,
             "type": "string"
         },
         "TableProfilingConfiguration": {
             "members": {
@@ -20843,42 +20349,14 @@
         },
         "TableVersionErrors": {
             "member": {
                 "shape": "TableVersionError"
             },
             "type": "list"
         },
-        "Tag": {
-            "members": {
-                "key": {
-                    "shape": "TagKey"
-                },
-                "value": {
-                    "shape": "TagValue"
-                }
-            },
-            "type": "structure"
-        },
-        "TagFilter": {
-            "members": {
-                "Key": {
-                    "shape": "TagKey"
-                },
-                "Values": {
-                    "shape": "TagValueList"
-                }
-            },
-            "type": "structure"
-        },
-        "TagFilterList": {
-            "member": {
-                "shape": "TagFilter"
-            },
-            "type": "list"
-        },
         "TagKey": {
             "max": 128,
             "min": 1,
             "type": "string"
         },
         "TagKeysList": {
             "max": 50,
@@ -20908,182 +20386,25 @@
             "type": "structure"
         },
         "TagValue": {
             "max": 256,
             "min": 0,
             "type": "string"
         },
-        "TagValueList": {
-            "member": {
-                "shape": "TagValue"
-            },
-            "type": "list"
-        },
-        "TagrisAccessDeniedException": {
-            "exception": true,
-            "members": {
-                "message": {
-                    "shape": "TagrisExceptionMessage"
-                }
-            },
-            "type": "structure"
-        },
-        "TagrisAccountId": {
-            "max": 12,
-            "min": 12,
-            "type": "string"
-        },
-        "TagrisAmazonResourceName": {
-            "max": 1011,
-            "min": 1,
-            "type": "string"
-        },
-        "TagrisExceptionMessage": {
-            "max": 2048,
-            "min": 0,
-            "type": "string"
-        },
-        "TagrisInternalId": {
-            "max": 64,
-            "min": 0,
-            "type": "string"
-        },
-        "TagrisInternalServiceException": {
-            "exception": true,
-            "fault": true,
-            "members": {
-                "message": {
-                    "shape": "TagrisExceptionMessage"
-                }
-            },
-            "type": "structure"
-        },
-        "TagrisInvalidArnException": {
-            "exception": true,
-            "members": {
-                "message": {
-                    "shape": "TagrisExceptionMessage"
-                },
-                "sweepListItem": {
-                    "shape": "TagrisSweepListItem"
-                }
-            },
-            "type": "structure"
-        },
-        "TagrisInvalidParameterException": {
-            "exception": true,
-            "members": {
-                "message": {
-                    "shape": "TagrisExceptionMessage"
-                }
-            },
-            "type": "structure"
-        },
-        "TagrisPartialResourcesExistResultsException": {
-            "exception": true,
-            "members": {
-                "message": {
-                    "shape": "TagrisExceptionMessage"
-                },
-                "resourceExistenceInformation": {
-                    "shape": "TagrisSweepListResult"
-                }
-            },
-            "type": "structure"
-        },
-        "TagrisStatus": {
-            "enum": [
-                "ACTIVE",
-                "NOT_ACTIVE"
-            ],
-            "type": "string"
-        },
-        "TagrisSweepList": {
-            "member": {
-                "shape": "TagrisSweepListItem"
-            },
-            "type": "list"
-        },
-        "TagrisSweepListItem": {
-            "members": {
-                "TagrisAccountId": {
-                    "shape": "TagrisAccountId"
-                },
-                "TagrisAmazonResourceName": {
-                    "shape": "TagrisAmazonResourceName"
-                },
-                "TagrisInternalId": {
-                    "shape": "TagrisInternalId"
-                },
-                "TagrisVersion": {
-                    "shape": "TagrisVersion"
-                }
-            },
-            "type": "structure"
-        },
-        "TagrisSweepListResult": {
-            "key": {
-                "shape": "TagrisAmazonResourceName"
-            },
-            "type": "map",
-            "value": {
-                "shape": "TagrisStatus"
-            }
-        },
-        "TagrisThrottledException": {
-            "exception": true,
-            "members": {
-                "message": {
-                    "shape": "TagrisExceptionMessage"
-                }
-            },
-            "type": "structure"
-        },
-        "TagrisVerifyResourcesExistInput": {
-            "members": {
-                "TagrisSweepList": {
-                    "shape": "TagrisSweepList"
-                }
-            },
-            "required": [
-                "TagrisSweepList"
-            ],
-            "type": "structure"
-        },
-        "TagrisVerifyResourcesExistOutput": {
-            "members": {
-                "TagrisSweepListResult": {
-                    "shape": "TagrisSweepListResult"
-                }
-            },
-            "required": [
-                "TagrisSweepListResult"
-            ],
-            "type": "structure"
-        },
-        "TagrisVersion": {
-            "type": "long"
-        },
         "TagsMap": {
             "key": {
                 "shape": "TagKey"
             },
             "max": 50,
             "min": 0,
             "type": "map",
             "value": {
                 "shape": "TagValue"
             }
         },
-        "TagsPerPageInteger": {
-            "box": true,
-            "max": 500,
-            "min": 100,
-            "type": "integer"
-        },
         "TaskRun": {
             "members": {
                 "CompletedOn": {
                     "shape": "Timestamp"
                 },
                 "ErrorString": {
                     "shape": "GenericString"
@@ -21247,14 +20568,23 @@
         },
         "TemplateInstances": {
             "member": {
                 "shape": "TemplateInstance"
             },
             "type": "list"
         },
+        "ThrottlingException": {
+            "exception": true,
+            "members": {
+                "Message": {
+                    "shape": "MessageString"
+                }
+            },
+            "type": "structure"
+        },
         "Timeout": {
             "box": true,
             "min": 1,
             "type": "integer"
         },
         "Timestamp": {
             "type": "timestamp"
@@ -21266,14 +20596,38 @@
             "type": "string"
         },
         "TokenString": {
             "max": 36,
             "min": 1,
             "type": "string"
         },
+        "TokenUrl": {
+            "max": 256,
+            "pattern": "^(https?)://[-a-zA-Z0-9+&@#/%?=~_|!:,.;]*[-a-zA-Z0-9+&@#/%=~_|]",
+            "type": "string"
+        },
+        "TokenUrlParameterKey": {
+            "max": 128,
+            "min": 1,
+            "type": "string"
+        },
+        "TokenUrlParameterValue": {
+            "max": 512,
+            "min": 1,
+            "type": "string"
+        },
+        "TokenUrlParametersMap": {
+            "key": {
+                "shape": "TokenUrlParameterKey"
+            },
+            "type": "map",
+            "value": {
+                "shape": "TokenUrlParameterValue"
+            }
+        },
         "TotalSegmentsInteger": {
             "max": 10,
             "min": 1,
             "type": "integer"
         },
         "TransactionIdString": {
             "max": 255,
@@ -21326,21 +20680,14 @@
         },
         "TransformIdList": {
             "member": {
                 "shape": "HashString"
             },
             "type": "list"
         },
-        "TransformIds": {
-            "max": 100,
-            "member": {
-                "shape": "HashString"
-            },
-            "type": "list"
-        },
         "TransformList": {
             "member": {
                 "shape": "MLTransform"
             },
             "type": "list"
         },
         "TransformParameterMap": {
@@ -21550,50 +20897,14 @@
         },
         "UnfilteredPartitionList": {
             "member": {
                 "shape": "UnfilteredPartition"
             },
             "type": "list"
         },
-        "UnfilteredTable": {
-            "members": {
-                "AuthorizedColumns": {
-                    "shape": "NameStringList"
-                },
-                "ColumnRowFilters": {
-                    "shape": "ColumnRowFilterList"
-                },
-                "CombinedRowFilter": {
-                    "shape": "PredicateString"
-                },
-                "IsAllowedToViewDataFilters": {
-                    "shape": "Boolean"
-                },
-                "IsRegisteredWithLakeFormation": {
-                    "shape": "Boolean"
-                },
-                "RowFilter": {
-                    "shape": "PredicateString"
-                },
-                "Table": {
-                    "shape": "Table"
-                },
-                "UseAdvancedFiltering": {
-                    "shape": "Boolean"
-                }
-            },
-            "type": "structure"
-        },
-        "UnfilteredTableList": {
-            "max": 100,
-            "member": {
-                "shape": "UnfilteredTable"
-            },
-            "type": "list"
-        },
         "UntagResourceRequest": {
             "members": {
                 "ResourceArn": {
                     "shape": "GlueResourceArn"
                 },
                 "TagsToRemove": {
                     "shape": "TagKeysList"
@@ -21783,14 +21094,17 @@
                 },
                 "LineageConfiguration": {
                     "shape": "LineageConfiguration"
                 },
                 "Name": {
                     "shape": "NameString"
                 },
+                "PIIConfiguration": {
+                    "shape": "PIIConfiguration"
+                },
                 "RecrawlPolicy": {
                     "shape": "RecrawlPolicy"
                 },
                 "Role": {
                     "shape": "Role"
                 },
                 "Schedule": {
@@ -21860,62 +21174,84 @@
                     "shape": "CsvHeader"
                 },
                 "Name": {
                     "shape": "NameString"
                 },
                 "QuoteSymbol": {
                     "shape": "CsvQuoteSymbol"
+                },
+                "Serde": {
+                    "shape": "CsvSerdeOption"
                 }
             },
             "required": [
                 "Name"
             ],
             "type": "structure"
         },
         "UpdateDataQualityRulesetRequest": {
             "members": {
                 "Description": {
                     "shape": "DescriptionString"
                 },
                 "Identifier": {
+                    "deprecated": true,
+                    "internalonly": true,
                     "shape": "DataQualityRulesetIdentifier"
                 },
                 "Name": {
                     "shape": "NameString"
                 },
                 "Ruleset": {
                     "shape": "DataQualityRulesetString"
                 },
                 "UpdatedName": {
+                    "deprecated": true,
                     "shape": "NameString"
                 }
             },
+            "required": [
+                "Name"
+            ],
             "type": "structure"
         },
         "UpdateDataQualityRulesetResponse": {
             "members": {
                 "CreatedOn": {
+                    "deprecated": true,
+                    "internalonly": true,
                     "shape": "Timestamp"
                 },
                 "Description": {
                     "shape": "DescriptionString"
                 },
+                "Identifier": {
+                    "deprecated": true,
+                    "internalonly": true,
+                    "shape": "DataQualityRulesetIdentifier"
+                },
                 "LastModifiedOn": {
+                    "deprecated": true,
+                    "internalonly": true,
                     "shape": "Timestamp"
                 },
                 "Name": {
                     "shape": "NameString"
                 },
                 "RecommendationRunId": {
+                    "deprecated": true,
+                    "internalonly": true,
                     "shape": "HashString"
                 },
                 "Ruleset": {
                     "shape": "DataQualityRulesetString"
                 },
                 "TargetTable": {
+                    "deprecated": true,
+                    "internalonly": true,
                     "shape": "DataQualityTargetTable"
                 }
             },
             "type": "structure"
         },
         "UpdateDatabaseRequest": {
             "members": {
@@ -21971,32 +21307,14 @@
             ],
             "type": "structure"
         },
         "UpdateDevEndpointResponse": {
             "members": {},
             "type": "structure"
         },
-        "UpdateFederationProfileRequest": {
-            "members": {
-                "ProfileInput": {
-                    "shape": "FederationProfileInput"
-                },
-                "VersionId": {
-                    "shape": "VersionString"
-                }
-            },
-            "required": [
-                "ProfileInput"
-            ],
-            "type": "structure"
-        },
-        "UpdateFederationProfileResponse": {
-            "members": {},
-            "type": "structure"
-        },
         "UpdateGrokClassifierRequest": {
             "members": {
                 "Classification": {
                     "shape": "Classification"
                 },
                 "CustomPatterns": {
                     "shape": "CustomPatterns"
@@ -22092,14 +21410,18 @@
         "UpdateJobRequest": {
             "members": {
                 "JobName": {
                     "shape": "NameString"
                 },
                 "JobUpdate": {
                     "shape": "JobUpdate"
+                },
+                "ProfileName": {
+                    "internalonly": true,
+                    "shape": "NameString"
                 }
             },
             "required": [
                 "JobName",
                 "JobUpdate"
             ],
             "type": "structure"
@@ -22122,36 +21444,14 @@
                 }
             },
             "required": [
                 "Name"
             ],
             "type": "structure"
         },
-        "UpdateLineageNodeRequest": {
-            "members": {
-                "CatalogId": {
-                    "shape": "CatalogIdString"
-                },
-                "Node": {
-                    "shape": "LineageNode"
-                }
-            },
-            "required": [
-                "Node"
-            ],
-            "type": "structure"
-        },
-        "UpdateLineageNodeResponse": {
-            "members": {
-                "Node": {
-                    "shape": "LineageNode"
-                }
-            },
-            "type": "structure"
-        },
         "UpdateMLTransformRequest": {
             "members": {
                 "Description": {
                     "shape": "DescriptionString"
                 },
                 "GlueVersion": {
                     "shape": "GlueVersionString"
@@ -22249,44 +21549,14 @@
                 },
                 "RegistryName": {
                     "shape": "SchemaRegistryNameString"
                 }
             },
             "type": "structure"
         },
-        "UpdateResourceSharingStateRequest": {
-            "members": {
-                "Action": {
-                    "shape": "RAMSharingAction"
-                },
-                "ConsumerAccountId": {
-                    "shape": "RAMAWSAccountId"
-                },
-                "InternalId": {
-                    "shape": "RAMInternalId"
-                },
-                "OwnerAccountId": {
-                    "shape": "RAMAWSAccountId"
-                },
-                "Resource": {
-                    "shape": "RAMResourceARN"
-                },
-                "SequenceNumber": {
-                    "shape": "RAMSequenceNumber"
-                }
-            },
-            "required": [
-                "Action",
-                "OwnerAccountId",
-                "Resource",
-                "ConsumerAccountId",
-                "SequenceNumber"
-            ],
-            "type": "structure"
-        },
         "UpdateSchemaInput": {
             "members": {
                 "Compatibility": {
                     "shape": "Compatibility"
                 },
                 "Description": {
                     "shape": "DescriptionString"
@@ -22353,33 +21623,73 @@
             "members": {
                 "JobName": {
                     "shape": "NameString"
                 }
             },
             "type": "structure"
         },
+        "UpdateTableOptimizerRequest": {
+            "members": {
+                "CatalogId": {
+                    "shape": "CatalogIdString"
+                },
+                "DatabaseName": {
+                    "shape": "NameString"
+                },
+                "TableName": {
+                    "shape": "NameString"
+                },
+                "TableOptimizerConfiguration": {
+                    "shape": "TableOptimizerConfiguration"
+                },
+                "Type": {
+                    "shape": "TableOptimizerType"
+                }
+            },
+            "required": [
+                "CatalogId",
+                "DatabaseName",
+                "TableName",
+                "Type",
+                "TableOptimizerConfiguration"
+            ],
+            "type": "structure"
+        },
+        "UpdateTableOptimizerResponse": {
+            "members": {},
+            "type": "structure"
+        },
         "UpdateTableRequest": {
             "members": {
                 "CatalogId": {
                     "shape": "CatalogIdString"
                 },
+                "ContextMap": {
+                    "shape": "RequestContextMap"
+                },
                 "DatabaseName": {
                     "shape": "NameString"
                 },
+                "Force": {
+                    "shape": "Boolean"
+                },
                 "SkipArchive": {
                     "shape": "BooleanNullable"
                 },
                 "TableInput": {
                     "shape": "TableInput"
                 },
                 "TransactionId": {
                     "shape": "TransactionIdString"
                 },
                 "VersionId": {
                     "shape": "VersionString"
+                },
+                "ViewUpdateAction": {
+                    "shape": "ViewUpdateAction"
                 }
             },
             "required": [
                 "DatabaseName",
                 "TableInput"
             ],
             "type": "structure"
@@ -22484,14 +21794,37 @@
         },
         "UpdatedTimestamp": {
             "type": "string"
         },
         "UriString": {
             "type": "string"
         },
+        "UsageProfileDefinition": {
+            "members": {
+                "CreatedOn": {
+                    "shape": "TimestampValue"
+                },
+                "Description": {
+                    "shape": "DescriptionString"
+                },
+                "LastModifiedOn": {
+                    "shape": "TimestampValue"
+                },
+                "ProfileName": {
+                    "shape": "NameString"
+                }
+            },
+            "type": "structure"
+        },
+        "UsageProfileDefinitionList": {
+            "member": {
+                "shape": "UsageProfileDefinition"
+            },
+            "type": "list"
+        },
         "UserDefinedFunction": {
             "members": {
                 "CatalogId": {
                     "shape": "CatalogIdString"
                 },
                 "ClassName": {
                     "shape": "NameString"
@@ -22539,48 +21872,18 @@
         },
         "UserDefinedFunctionList": {
             "member": {
                 "shape": "UserDefinedFunction"
             },
             "type": "list"
         },
-        "ValidateResourceSharingRequest": {
-            "members": {
-                "InternalId": {
-                    "shape": "RAMInternalId"
-                },
-                "OwnerAccountId": {
-                    "shape": "RAMAWSAccountId"
-                },
-                "Resource": {
-                    "shape": "RAMResourceARN"
-                }
-            },
-            "required": [
-                "OwnerAccountId",
-                "Resource"
-            ],
-            "type": "structure"
-        },
-        "ValidateResourceSharingResponse": {
-            "members": {
-                "InternalId": {
-                    "shape": "RAMInternalId"
-                },
-                "ValidationMessage": {
-                    "shape": "RAMValidationMessage"
-                },
-                "ValidationResult": {
-                    "shape": "RAMValidationResult"
-                }
-            },
-            "required": [
-                "ValidationResult"
-            ],
-            "type": "structure"
+        "UserManagedClientApplicationClientId": {
+            "max": 2048,
+            "pattern": "\\S+",
+            "type": "string"
         },
         "ValidationException": {
             "exception": true,
             "members": {
                 "Message": {
                     "shape": "MessageString"
                 }
@@ -22624,25 +21927,153 @@
         },
         "VersionsString": {
             "max": 100000,
             "min": 1,
             "pattern": "[1-9][0-9]*|[1-9][0-9]*-[1-9][0-9]*",
             "type": "string"
         },
+        "ViewDefinition": {
+            "members": {
+                "Definer": {
+                    "shape": "ArnString"
+                },
+                "IsProtected": {
+                    "shape": "NullableBoolean"
+                },
+                "Representations": {
+                    "shape": "ViewRepresentationList"
+                },
+                "SubObjects": {
+                    "shape": "ViewSubObjectsList"
+                }
+            },
+            "type": "structure"
+        },
+        "ViewDefinitionDDLInput": {
+            "internalonly": true,
+            "members": {
+                "Definer": {
+                    "shape": "ArnString"
+                },
+                "IsProtected": {
+                    "shape": "NullableBoolean"
+                },
+                "Representations": {
+                    "shape": "ViewRepresentationDDLInputList"
+                },
+                "SubObjects": {
+                    "shape": "ViewSubObjectsList"
+                }
+            },
+            "type": "structure"
+        },
+        "ViewDialect": {
+            "enum": [
+                "REDSHIFT",
+                "ATHENA",
+                "SPARK"
+            ],
+            "type": "string"
+        },
+        "ViewDialectVersionString": {
+            "max": 255,
+            "min": 1,
+            "pattern": "[a-zA-Z0-9_.-]+",
+            "type": "string"
+        },
+        "ViewRepresentation": {
+            "members": {
+                "Dialect": {
+                    "shape": "ViewDialect"
+                },
+                "DialectVersion": {
+                    "shape": "ViewDialectVersionString"
+                },
+                "IsStale": {
+                    "shape": "NullableBoolean"
+                },
+                "ValidationConnection": {
+                    "shape": "NameString"
+                },
+                "ViewExpandedText": {
+                    "shape": "ViewTextString"
+                },
+                "ViewOriginalText": {
+                    "shape": "ViewTextString"
+                },
+                "ViewValidationText": {
+                    "shape": "ViewTextString"
+                }
+            },
+            "type": "structure"
+        },
+        "ViewRepresentationDDLInput": {
+            "internalonly": true,
+            "members": {
+                "Dialect": {
+                    "shape": "ViewDialect"
+                },
+                "DialectVersion": {
+                    "shape": "ViewDialectVersionString"
+                },
+                "ViewExpandedText": {
+                    "shape": "ViewTextString"
+                },
+                "ViewOriginalText": {
+                    "shape": "ViewTextString"
+                }
+            },
+            "type": "structure"
+        },
+        "ViewRepresentationDDLInputList": {
+            "internalonly": true,
+            "max": 1,
+            "member": {
+                "shape": "ViewRepresentationDDLInput"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "ViewRepresentationList": {
+            "max": 1000,
+            "member": {
+                "shape": "ViewRepresentation"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "ViewSubObjectsList": {
+            "max": 10,
+            "member": {
+                "shape": "ArnString"
+            },
+            "min": 0,
+            "type": "list"
+        },
         "ViewTextString": {
             "max": 409600,
             "type": "string"
         },
+        "ViewUpdateAction": {
+            "enum": [
+                "ADD",
+                "REPLACE",
+                "ADD_OR_REPLACE",
+                "DROP"
+            ],
+            "type": "string"
+        },
         "WorkerType": {
             "enum": [
                 "Standard",
                 "G.1X",
                 "G.2X",
+                "G.4X",
+                "G.8X",
                 "G.025X",
-                "Z.1X",
                 "Z.2X"
             ],
             "type": "string"
         },
         "Workflow": {
             "members": {
                 "BlueprintDetails": {
@@ -22831,13 +22262,22 @@
             },
             "required": [
                 "Name",
                 "Classification"
             ],
             "type": "structure"
         },
-        "isCellClosed": {
-            "type": "boolean"
+        "databaseNameString": {
+            "min": 1,
+            "type": "string"
+        },
+        "glueConnectionNameString": {
+            "min": 1,
+            "type": "string"
+        },
+        "tableNameString": {
+            "min": 1,
+            "type": "string"
         }
     },
     "version": "2.0"
 }
```

### Comparing `aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_pyspark/logo-128x128.png` & `aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_pyspark/logo-128x128.png`

 * *Files identical despite different names*

### Comparing `aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_pyspark/logo-32x32.png` & `aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_pyspark/logo-32x32.png`

 * *Files identical despite different names*

### Comparing `aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_pyspark/logo-64x64.png` & `aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_pyspark/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_spark/GlueKernel.py` & `aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_spark/GlueKernel.py`

 * *Files identical despite different names*

### Comparing `aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_spark/logo-128x128.png` & `aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_spark/logo-128x128.png`

 * *Files identical despite different names*

### Comparing `aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_spark/logo-32x32.png` & `aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_spark/logo-32x32.png`

 * *Files identical despite different names*

### Comparing `aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/glue_spark/logo-64x64.png` & `aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/glue_spark/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/install.sh` & `aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/install.sh`

 * *Files identical despite different names*

### Comparing `aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/logos/logo-128x128.png` & `aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/logos/logo-128x128.png`

 * *Files identical despite different names*

### Comparing `aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/logos/logo-32x32.png` & `aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/logos/logo-32x32.png`

 * *Files identical despite different names*

### Comparing `aws-glue-sessions-1.0.4/src/aws_glue_interactive_sessions_kernel/logos/logo-64x64.png` & `aws-glue-sessions-1.0.5/src/aws_glue_interactive_sessions_kernel/logos/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `aws-glue-sessions-1.0.4/src/aws_glue_sessions.egg-info/PKG-INFO` & `aws-glue-sessions-1.0.5/src/aws_glue_sessions.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-glue-sessions
-Version: 1.0.4
+Version: 1.0.5
 Summary: Glue Interactive Sessions Jupyter kernel that integrates almost anywhere Jupyter does including your favorite IDEs.
 Home-page: https://aws.amazon.com/glue/
 Author: Glue Development Team
 Author-email: glue-sessions-preview@amazon.com
 License: Apache 2.0 License
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -57,14 +57,19 @@
 ### Using the kernel via other IDEs
 
 You may also use this kernel via VSCode or other IDEs that support Jupyter kernels.
 To set up the Glue Interactive Sessions kernel for Visual Studio Code follow [these instructions](https://docs.aws.amazon.com/glue/latest/dg/interactive-sessions-vscode.html).
 
 
 ## ChangeLog
+### v1.0.5 (2024-04-19)
+
+* New magic %timeout for configuring 'Timeout' parameter for Session.
+* New magic %reconnect, Customers can use %reconnect <sessionId> and reconnect to any of their live Session.
+
 ### v1.0.4 (2023-12-01)
 
 Added support for inferring region from AWS_REGION environment variable.
 
 ### v1.0.3 (2023-11-15)
 
 Added support for handling special characters in owner tag.
```

### Comparing `aws-glue-sessions-1.0.4/src/aws_glue_sessions.egg-info/SOURCES.txt` & `aws-glue-sessions-1.0.5/src/aws_glue_sessions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

