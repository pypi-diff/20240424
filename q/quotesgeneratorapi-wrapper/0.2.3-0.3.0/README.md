# Comparing `tmp/quotesgeneratorapi_wrapper-0.2.3.tar.gz` & `tmp/quotesgeneratorapi_wrapper-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quotesgeneratorapi_wrapper-0.2.3.tar", max compression
+gzip compressed data, was "quotesgeneratorapi_wrapper-0.3.0.tar", max compression
```

## Comparing `quotesgeneratorapi_wrapper-0.2.3.tar` & `quotesgeneratorapi_wrapper-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1080 2024-03-05 18:28:23.204977 quotesgeneratorapi_wrapper-0.2.3/LICENSE
--rw-r--r--   0        0        0        0 2024-04-14 20:50:25.840847 quotesgeneratorapi_wrapper-0.2.3/README.md
--rw-r--r--   0        0        0      301 2024-04-14 21:00:56.230023 quotesgeneratorapi_wrapper-0.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-14 20:50:25.840847 quotesgeneratorapi_wrapper-0.2.3/quotesgeneratorapi_wrapper/__init__.py
--rw-r--r--   0        0        0      491 2024-04-14 21:00:47.773846 quotesgeneratorapi_wrapper-0.2.3/quotesgeneratorapi_wrapper/quotesgenerator.py
--rw-r--r--   0        0        0      371 1970-01-01 00:00:00.000000 quotesgeneratorapi_wrapper-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-03-05 18:28:23.204977 quotesgeneratorapi_wrapper-0.3.0/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-14 20:50:25.840847 quotesgeneratorapi_wrapper-0.3.0/README.md
+-rw-r--r--   0        0        0      373 2024-04-24 21:04:29.299667 quotesgeneratorapi_wrapper-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-14 20:50:25.840847 quotesgeneratorapi_wrapper-0.3.0/quotesgeneratorapi_wrapper/__init__.py
+-rw-r--r--   0        0        0      491 2024-04-14 21:21:56.700740 quotesgeneratorapi_wrapper-0.3.0/quotesgeneratorapi_wrapper/quotesgenerator.py
+-rw-r--r--   0        0        0      663 1970-01-01 00:00:00.000000 quotesgeneratorapi_wrapper-0.3.0/PKG-INFO
```

### Comparing `quotesgeneratorapi_wrapper-0.2.3/LICENSE` & `quotesgeneratorapi_wrapper-0.3.0/LICENSE`

 * *Files identical despite different names*

