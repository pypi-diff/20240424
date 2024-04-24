# Comparing `tmp/eidolon_ai_usage_client-0.1.2.tar.gz` & `tmp/eidolon_ai_usage_client-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eidolon_ai_usage_client-0.1.2.tar", max compression
+gzip compressed data, was "eidolon_ai_usage_client-0.1.3.tar", max compression
```

## Comparing `eidolon_ai_usage_client-0.1.2.tar` & `eidolon_ai_usage_client-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-03-19 16:13:23.010729 eidolon_ai_usage_client-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-03-21 23:17:38.645326 eidolon_ai_usage_client-0.1.2/eidolon_ai_usage_client/__init__.py
--rw-r--r--   0        0        0     1723 2024-04-18 18:24:50.935853 eidolon_ai_usage_client-0.1.2/eidolon_ai_usage_client/client.py
--rw-r--r--   0        0        0      460 2024-03-21 23:17:38.647427 eidolon_ai_usage_client-0.1.2/eidolon_ai_usage_client/models.py
--rw-r--r--   0        0        0      420 2024-04-18 19:08:47.133447 eidolon_ai_usage_client-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 eidolon_ai_usage_client-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-24 05:50:43.488579 eidolon_ai_usage_client-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-24 05:50:43.488579 eidolon_ai_usage_client-0.1.3/eidolon_ai_usage_client/__init__.py
+-rw-r--r--   0        0        0     1723 2024-04-24 05:50:43.488579 eidolon_ai_usage_client-0.1.3/eidolon_ai_usage_client/client.py
+-rw-r--r--   0        0        0      460 2024-04-24 05:50:43.488579 eidolon_ai_usage_client-0.1.3/eidolon_ai_usage_client/models.py
+-rw-r--r--   0        0        0      501 2024-04-24 05:51:15.980378 eidolon_ai_usage_client-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 eidolon_ai_usage_client-0.1.3/PKG-INFO
```

### Comparing `eidolon_ai_usage_client-0.1.2/eidolon_ai_usage_client/client.py` & `eidolon_ai_usage_client-0.1.3/eidolon_ai_usage_client/client.py`

 * *Files identical despite different names*

