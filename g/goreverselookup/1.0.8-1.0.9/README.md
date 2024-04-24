# Comparing `tmp/goreverselookup-1.0.8.tar.gz` & `tmp/goreverselookup-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goreverselookup-1.0.8.tar", last modified: Sat Sep 30 12:01:27 2023, max compression
+gzip compressed data, was "goreverselookup-1.0.9.tar", last modified: Sat Sep 30 15:23:42 2023, max compression
```

## Comparing `goreverselookup-1.0.8.tar` & `goreverselookup-1.0.9.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:01:27.462099 goreverselookup-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:01:27.446099 goreverselookup-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:01:27.446099 goreverselookup-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/.github/workflows/publish_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/.github/workflows/test_on_push.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    27553 2023-09-30 12:01:27.462099 goreverselookup-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26406 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:01:27.454099 goreverselookup-1.0.8/exe_version/
--rw-r--r--   0 runner    (1001) docker     (127)  6692774 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/exe_version/GOReverseLookup.exe
--rw-r--r--   0 runner    (1001) docker     (127)      223 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/exe_version/dev_info.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:01:27.454099 goreverselookup-1.0.8/exe_version/input_files/
--rw-r--r--   0 runner    (1001) docker     (127)    29397 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/exe_version/input_files/input.txt
--rw-r--r--   0 runner    (1001) docker     (127)      861 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/exe_version/logging_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/exe_version/main_model_exe.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/exe_version/main_model_exe_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:01:27.454099 goreverselookup-1.0.8/input_files/
--rw-r--r--   0 runner    (1001) docker     (127)    29502 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/input_files/input.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:01:27.454099 goreverselookup-1.0.8/log_output/
--rw-r--r--   0 runner    (1001) docker     (127)   725104 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/log_output/goterm_product_mismatches.txt
--rw-r--r--   0 runner    (1001) docker     (127)      861 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/logging_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2023-09-30 12:00:59.000000 goreverselookup-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-30 12:01:27.462099 goreverselookup-1.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:01:27.446099 goreverselookup-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:01:27.458099 goreverselookup-1.0.8/src/goreverselookup/
--rw-r--r--   0 runner    (1001) docker     (127)   108584 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/src/goreverselookup/Model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17552 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/src/goreverselookup/Workflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/src/goreverselookup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:01:27.458099 goreverselookup-1.0.8/src/goreverselookup/core/
--rw-r--r--   0 runner    (1001) docker     (127)    18446 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/src/goreverselookup/core/GOTerm.py
--rw-r--r--   0 runner    (1001) docker     (127)    20277 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/src/goreverselookup/core/GOTerm_new.py
--rw-r--r--   0 runner    (1001) docker     (127)    58316 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/src/goreverselookup/core/Metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/src/goreverselookup/core/ModelSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)    33144 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/src/goreverselookup/core/Product.py
--rw-r--r--   0 runner    (1001) docker     (127)    33476 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/src/goreverselookup/core/Report.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/src/goreverselookup/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/src/goreverselookup/core/miRNA.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:01:27.458099 goreverselookup-1.0.8/src/goreverselookup/parse/
--rw-r--r--   0 runner    (1001) docker     (127)    17182 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/src/goreverselookup/parse/GOAFParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9694 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/src/goreverselookup/parse/OBOParser.py
--rw-r--r--   0 runner    (1001) docker     (127)    27948 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/src/goreverselookup/parse/OrthologParsers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/src/goreverselookup/parse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:01:27.458099 goreverselookup-1.0.8/src/goreverselookup/util/
--rw-r--r--   0 runner    (1001) docker     (127)    17059 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/src/goreverselookup/util/CacheUtil.py
--rw-r--r--   0 runner    (1001) docker     (127)     9842 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/src/goreverselookup/util/FileUtil.py
--rw-r--r--   0 runner    (1001) docker     (127)     7756 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/src/goreverselookup/util/JsonUtil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/src/goreverselookup/util/LogConfigLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/src/goreverselookup/util/Timer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/src/goreverselookup/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:01:27.458099 goreverselookup-1.0.8/src/goreverselookup/web_apis/
--rw-r--r--   0 runner    (1001) docker     (127)    27702 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/src/goreverselookup/web_apis/EnsemblApi.py
--rw-r--r--   0 runner    (1001) docker     (127)    17455 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/src/goreverselookup/web_apis/GOApi.py
--rw-r--r--   0 runner    (1001) docker     (127)    28830 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/src/goreverselookup/web_apis/UniprotApi.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/src/goreverselookup/web_apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:01:27.458099 goreverselookup-1.0.8/src/goreverselookup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27553 2023-09-30 12:01:27.000000 goreverselookup-1.0.8/src/goreverselookup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2023-09-30 12:01:27.000000 goreverselookup-1.0.8/src/goreverselookup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-30 12:01:27.000000 goreverselookup-1.0.8/src/goreverselookup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-09-30 12:01:27.000000 goreverselookup-1.0.8/src/goreverselookup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-09-30 12:01:27.000000 goreverselookup-1.0.8/src/goreverselookup.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 12:01:27.462099 goreverselookup-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/tests/no_test_main_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/tests/no_test_main_workflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/tests/no_test_playground.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2023-09-30 12:00:56.000000 goreverselookup-1.0.8/tests/test_webapis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 15:23:42.512809 goreverselookup-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 15:23:42.492809 goreverselookup-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 15:23:42.496809 goreverselookup-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/.github/workflows/publish_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/.github/workflows/test_on_push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    27553 2023-09-30 15:23:42.512809 goreverselookup-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26406 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 15:23:42.504809 goreverselookup-1.0.9/exe_version/
+-rw-r--r--   0 runner    (1001) docker     (127)  6692774 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/exe_version/GOReverseLookup.exe
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/exe_version/dev_info.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 15:23:42.504809 goreverselookup-1.0.9/exe_version/input_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    29397 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/exe_version/input_files/input.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/exe_version/logging_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/exe_version/main_model_exe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/exe_version/main_model_exe_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 15:23:42.504809 goreverselookup-1.0.9/input_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    29501 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/input_files/input.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 15:23:42.504809 goreverselookup-1.0.9/log_output/
+-rw-r--r--   0 runner    (1001) docker     (127)   725104 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/log_output/goterm_product_mismatches.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/logging_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2023-09-30 15:23:14.000000 goreverselookup-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-30 15:23:42.512809 goreverselookup-1.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 15:23:42.492809 goreverselookup-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 15:23:42.504809 goreverselookup-1.0.9/src/goreverselookup/
+-rw-r--r--   0 runner    (1001) docker     (127)   108295 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/src/goreverselookup/Model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17670 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/src/goreverselookup/Workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/src/goreverselookup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 15:23:42.508809 goreverselookup-1.0.9/src/goreverselookup/core/
+-rw-r--r--   0 runner    (1001) docker     (127)    18446 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/src/goreverselookup/core/GOTerm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20277 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/src/goreverselookup/core/GOTerm_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58604 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/src/goreverselookup/core/Metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/src/goreverselookup/core/ModelSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33144 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/src/goreverselookup/core/Product.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33476 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/src/goreverselookup/core/Report.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/src/goreverselookup/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/src/goreverselookup/core/miRNA.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 15:23:42.508809 goreverselookup-1.0.9/src/goreverselookup/parse/
+-rw-r--r--   0 runner    (1001) docker     (127)    18932 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/src/goreverselookup/parse/GOAFParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11153 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/src/goreverselookup/parse/OBOParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27948 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/src/goreverselookup/parse/OrthologParsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/src/goreverselookup/parse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 15:23:42.508809 goreverselookup-1.0.9/src/goreverselookup/util/
+-rw-r--r--   0 runner    (1001) docker     (127)    17059 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/src/goreverselookup/util/CacheUtil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9842 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/src/goreverselookup/util/FileUtil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7756 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/src/goreverselookup/util/JsonUtil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/src/goreverselookup/util/LogConfigLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/src/goreverselookup/util/Timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/src/goreverselookup/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 15:23:42.512809 goreverselookup-1.0.9/src/goreverselookup/web_apis/
+-rw-r--r--   0 runner    (1001) docker     (127)    27702 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/src/goreverselookup/web_apis/EnsemblApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17455 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/src/goreverselookup/web_apis/GOApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28830 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/src/goreverselookup/web_apis/UniprotApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/src/goreverselookup/web_apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 15:23:42.508809 goreverselookup-1.0.9/src/goreverselookup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27553 2023-09-30 15:23:42.000000 goreverselookup-1.0.9/src/goreverselookup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2023-09-30 15:23:42.000000 goreverselookup-1.0.9/src/goreverselookup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-30 15:23:42.000000 goreverselookup-1.0.9/src/goreverselookup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2023-09-30 15:23:42.000000 goreverselookup-1.0.9/src/goreverselookup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-09-30 15:23:42.000000 goreverselookup-1.0.9/src/goreverselookup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-30 15:23:42.512809 goreverselookup-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/tests/no_test_main_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/tests/no_test_main_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/tests/no_test_playground.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2023-09-30 15:23:11.000000 goreverselookup-1.0.9/tests/test_webapis.py
```

### Comparing `goreverselookup-1.0.8/.github/workflows/publish_release.yml` & `goreverselookup-1.0.9/.github/workflows/publish_release.yml`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/.github/workflows/test_on_push.yml` & `goreverselookup-1.0.9/.github/workflows/test_on_push.yml`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/.gitignore` & `goreverselookup-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/LICENSE` & `goreverselookup-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/PKG-INFO` & `goreverselookup-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goreverselookup
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python library for Gene Ontology Reverse Lookup
 Author-email: Aljoša Škorjanc <skorjanc.aljosa@gmail.com>, Vladimir Smrkolj <vladimir.smrkolj@gmail.com>
 License: Apache License 2.0
 Keywords: gene ontology,reverse lookup
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `goreverselookup-1.0.8/README.md` & `goreverselookup-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/exe_version/GOReverseLookup.exe` & `goreverselookup-1.0.9/exe_version/GOReverseLookup.exe`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/exe_version/input_files/input.txt` & `goreverselookup-1.0.9/exe_version/input_files/input.txt`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/exe_version/logging_config.json` & `goreverselookup-1.0.9/exe_version/logging_config.json`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/exe_version/main_model_exe.py` & `goreverselookup-1.0.9/exe_version/main_model_exe.py`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/input_files/input.txt` & `goreverselookup-1.0.9/input_files/input.txt`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 #		# in future runs, you can load up the model using:
 #		model_data_file = "model/data.json"
 #		model = ReverseLookup.load_model(model_data_file)
 ###settings
 #homosapiens_only	True
 #require_product_evidence_codes	False
 fisher_test_use_online_query	False
-include_indirect_annotations	False
+include_indirect_annotations	True
 uniprotkb_genename_online_query	False
 pvalue	0.05
 ###filepaths
 go_obo_filepath	data_files/go.obo
 goaf_filepath	data_files/goa_human.gaf
 zfin_human_ortho_mapping_filepath	data_files/zfin_human_ortholog_mapping.txt
 mgi_human_ortho_mapping_filepath	data_files/mgi_human_ortholog_mapping.txt
```

### Comparing `goreverselookup-1.0.8/log_output/goterm_product_mismatches.txt` & `goreverselookup-1.0.9/log_output/goterm_product_mismatches.txt`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/logging_config.json` & `goreverselookup-1.0.9/logging_config.json`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/pyproject.toml` & `goreverselookup-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "tqdm",
     "requests",
     "networkx",
     "tabulate",
     "statsmodels"
 ]
 
-version = "1.0.8"
+version = "1.0.9"
 #dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
     "pytest",
     "pytest-asyncio",
     "tox",
```

### Comparing `goreverselookup-1.0.8/src/goreverselookup/Model.py` & `goreverselookup-1.0.9/src/goreverselookup/Model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1837,15 +1837,15 @@
 
         # TODO: save statistical analysis as a part of the model's json and load it up on startup
         self.statistically_relevant_products = (
             statistically_relevant_products_final_sorted
         )
         logger.info(
             "Finished with product statistical analysis. Found"
-            f" {len(statistically_relevant_products)} statistically relevant products."
+            f" {len(statistically_relevant_products)} statistically relevant products. p = {self.model_settings.pvalue}"
         )
         JsonUtil.save_json(
             data_dictionary=statistically_relevant_products_final_sorted,
             filepath=filepath,
         )
         return statistically_relevant_products_final
 
@@ -1912,26 +1912,20 @@
                     datafile_paths["go_obo_filepath"] is not None
                     and datafile_paths["go_obo_filepath"] != ""
                 ):
                     obo_parser = OboParser(datafile_paths["go_obo_filepath"])
             else:
                 obo_parser = OboParser()
             for goterm in goterms:
-                assert isinstance(goterm, GOTerm)
+                assert isinstance(goterm, GOTerm) # TODO: FIX HERE !!!!!!!!! obo now returns a dict and not a goterm!!!
                 if goterm.parent_term_ids == [] or goterm.parent_term_ids is None:
-                    goterm_obo = obo_parser.all_goterms[
-                        goterm.id
-                    ]  # obo representation of this goterm
-                    goterm.update(
-                        goterm_obo
-                    )  # update current goterm with information from .obo file
-
-                    goterm_parent_ids = obo_parser.get_parent_terms(
-                        goterm.id
-                    )  # calculate parent term ids for this goterm
+                    goterm_obo = GOTerm.from_dict(obo_parser.all_goterms[goterm.id].__dict__)  # obo representation of this goterm is in json form
+                    goterm.update(goterm_obo)  # update current goterm with information from .obo file
+
+                    goterm_parent_ids = obo_parser.get_parent_terms(goterm.id)  # calculate parent term ids for this goterm
                     goterm.parent_term_ids = goterm_parent_ids  # update parent term ids
 
         products = []
         for product_dict in data.get("products", []):
             products.append(Product.from_dict(product_dict))
 
         miRNAs = []
@@ -2123,46 +2117,34 @@
             )
 
             # update goterms to include all parents and children
             with logging_redirect_tqdm():
                 for goterm in tqdm(go_terms, desc="Compute indirect nodes"):
                     assert isinstance(goterm, GOTerm)
                     if goterm.parent_term_ids == [] or goterm.parent_term_ids is None:
-                        goterm_obo = obo_parser.all_goterms[
-                            goterm.id
-                        ]  # obo representation of this goterm
-                        goterm.update(
-                            goterm_obo
-                        )  # update current goterm with information from .obo file
-
-                        goterm_parent_ids = obo_parser.get_parent_terms(
-                            goterm.id
-                        )  # calculate parent term ids for this goterm
-                        goterm_children_ids = obo_parser.get_child_terms(
-                            goterm.id
-                        )  # calculdate child term ids for this goterm
-                        goterm.parent_term_ids = (
-                            goterm_parent_ids  # update parent term ids
-                        )
-                        goterm.child_term_ids = (
-                            goterm_children_ids  # update child term ids
-                        )
+                        goterm_obo = GOTerm.from_dict(obo_parser.all_goterms[goterm.id].__dict__)  # obo representation of this goterm
+                        goterm.update(goterm_obo)  # update current goterm with information from .obo file
+
+                        goterm_parent_ids = obo_parser.get_parent_terms(goterm.id)  # calculate parent term ids for this goterm
+                        goterm_children_ids = obo_parser.get_child_terms(goterm.id)  # calculdate child term ids for this goterm
+                        goterm.parent_term_ids = goterm_parent_ids  # update parent term ids
+                        # goterm.child_term_ids = goterm_children_ids  # update child term ids
             logger.info("Indirect annotations have been computed.")
 
             """      
             for goterm in go_terms:
                 assert isinstance(goterm, GOTerm)
                 if goterm.parent_term_ids == [] or goterm.parent_term_ids == None:
                     goterm_obo = obo_parser.all_goterms[goterm.id] # obo representation of this goterm
                     goterm.update(goterm_obo) # update current goterm with information from .obo file
 
                     goterm_parent_ids = obo_parser.get_parent_terms(goterm.id) # calculate parent term ids for this goterm
                     goterm_children_ids = obo_parser.get_child_terms(goterm.id) # calculdate child term ids for this goterm
                     goterm.parent_term_ids = goterm_parent_ids # update parent term ids
-                    goterm.child_term_ids = goterm_children_ids # update child term ids
+                    # goterm.child_term_ids = goterm_children_ids # update child term ids
             """
 
         logger.info("Creating model from input file with:")
         logger.info(f"  - input file filepath: {filepath}")
         logger.info(f"  - input file line count: {filepath_readlines}")
         logger.info(f"  - count GO Terms: {len(go_terms)} ")
         logger.info(f"  - target_processes: {target_processes}")
```

### Comparing `goreverselookup-1.0.8/src/goreverselookup/Workflows.py` & `goreverselookup-1.0.9/src/goreverselookup/Workflows.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     adv_product_score,
     nterms,
     fisher_exact_test,
     binomial_test,
     basic_mirna_score,
 )
 from .core.Report import ReportGenerator
+from .core.ModelSettings import ModelSettings
 
 import logging
 
 # from logging import config
 # config.fileConfig("logging_config.py")
 logger = logging.getLogger(__name__)
 
@@ -317,45 +318,48 @@
         # constructor chooses appropriate method to initialise the Model based on supplied parameters. A ReverseLookup 'model' instance takes precedence over input_file_fpath.
         super().__init__(input_file_fpath, save_folder_dir, model, name)
         self.create_workflow(debug=debug)
 
     def create_workflow(self, debug: bool = False, fetch_mirna=False):
         # Fetch all GO term names and descriptions
         self.add_function(
-            self.model.fetch_all_go_term_names_descriptions, run_async=True
+            self.model.fetch_all_go_term_names_descriptions, 
+            run_async=True,
+            req_delay=0.5,
+            max_connections=20
         )
         # Fetch all GO term products
         self.add_function(
             self.model.fetch_all_go_term_products,
             web_download=True,
             run_async=True,
             recalculate=False,
             max_connections=40,
             request_params={"rows": 50000},
-            delay=0.0,
+            delay=0.5,
         )
         # Create product instances from GO terms
         self.add_function(self.model.create_products_from_goterms)
         # Fetch human ortholog for products (either UniProtID, ENSG or genename)
         self.add_function(
             self.model.fetch_ortholog_products,
             refetch=False,
             run_async=True,
-            max_connections=15,
+            max_connections=10,
             req_delay=0.1,
             semaphore_connections=5,
         )
         self.add_function(self.model.prune_products)
         self.add_function(self.model.save_model, self.model_save_filepath)
         # Fetch product information (from UniprotAPI or EnsemblAPI)
         self.add_function(
             self.model.fetch_product_infos,
             refetch=False,
             run_async=True,
-            max_connections=12,
+            max_connections=15,
             semaphore_connections=10,
             req_delay=0.1,
         )
         self.add_function(self.model.prune_products)
         self.add_function(self.model.save_model, self.model_save_filepath)
 
         # Score products with the scores supplied in scoring_classes
```

### Comparing `goreverselookup-1.0.8/src/goreverselookup/__init__.py` & `goreverselookup-1.0.9/src/goreverselookup/__init__.py`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/src/goreverselookup/core/GOTerm.py` & `goreverselookup-1.0.9/src/goreverselookup/core/GOTerm.py`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/src/goreverselookup/core/GOTerm_new.py` & `goreverselookup-1.0.9/src/goreverselookup/core/GOTerm_new.py`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/src/goreverselookup/core/Metrics.py` & `goreverselookup-1.0.9/src/goreverselookup/core/Metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -636,15 +636,18 @@
                 else:
                     # skip iteration, there was an error with querying goterms associated with a product
                     logger.warning(f"Online query for GO Terms associated with {product.uniprot_id} failed! Product: {json.dumps(product.__dict__)}")
                     continue
                 # num_goterms_product_general = len(self.online_query_api.get_goterms(product.uniprot_id, go_categories=self.reverse_lookup.go_categories))
                 logger.debug(f"Fisher test online num_goterms_product_general query: {num_goterms_product_general}")
             else:  # offline pathway: get goterms from GOAF
-                goterms_product_general = self.goaf.get_all_terms_for_product(product.genename)
+                if self.reverse_lookup.model_settings.include_indirect_annotations == True:
+                    goterms_product_general = self.goaf.get_all_terms_for_product(product.genename, indirect_annotations=True, obo_parser=self.reverse_lookup.obo_parser)
+                else:
+                    goterms_product_general = self.goaf.get_all_terms_for_product(product.genename)
                 num_goterms_product_general = len(goterms_product_general)  # all GO Terms associated with the current input Product instance (genename) from the GO Annotation File
 
             # find the number of parent indirect annotations
             if self.reverse_lookup.model_settings.include_indirect_annotations is True:
                 # include all parent goterms in the scoring
                 directly_associated_goterms = list(goterms_product_general)  # calling list constructor creates two separate entities, which prevents infinite looping !
                 for directly_associated_goterm in directly_associated_goterms:  # WARNING: don't iterate over goterms_product_general, since this list is being updated in the for loop !!
```

### Comparing `goreverselookup-1.0.8/src/goreverselookup/core/ModelSettings.py` & `goreverselookup-1.0.9/src/goreverselookup/core/ModelSettings.py`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/src/goreverselookup/core/Product.py` & `goreverselookup-1.0.9/src/goreverselookup/core/Product.py`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/src/goreverselookup/core/Report.py` & `goreverselookup-1.0.9/src/goreverselookup/core/Report.py`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/src/goreverselookup/core/miRNA.py` & `goreverselookup-1.0.9/src/goreverselookup/core/miRNA.py`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/src/goreverselookup/parse/GOAFParser.py` & `goreverselookup-1.0.9/src/goreverselookup/parse/GOAFParser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from typing import List
 import os
 import gzip
 import urllib
 
+from .OBOParser import OboParser
+
 import logging
 
 # from logging import config
 # config.fileConfig("../logging_config.py")
 logger = logging.getLogger(__name__)
 
 
@@ -19,14 +21,15 @@
             "molecular_activity",
             "cellular_component",
         ],
     ) -> None:
         """
         This class provides access to a Gene Ontology Annotations File, which stores the relations between each GO Term and it's products (genes),
         along with an evidence code, confirming the truth of the interaction. A GO Annotation comprises of a) GO Term, b) gene / gene product c) evidence code.
+        WARNING: GOAF stores only DIRECT annotations (See https://geneontology.org/docs/faq/ "Why does AmiGO display annotations to term X but these annotations aren’t in the GAF file?")
 
         Parameters:
           - (str) filepath: the filepath to the GO Annotations File downloaded file from http://current.geneontology.org/products/pages/downloads.html -> Homo Sapiens (EBI Gene Ontology Database) - protein = goa_human.gaf; link = http://geneontology.org/gene-associations/goa_human.gaf.gz
                             if left to default value, self._filepath will be set to 'app/goreverselookup/data_files/goa_human.gaf'. The file should reside in app/goreverselookup/data_files/ and the parameter filepath should be the file name of the downloaded file inside data_files/
           - (list) go_categories: determines which GO categories are valid. Default is that all three GO categories are valid. Setting GO categories determines which products
                                   or terms are returned from goaf.get_all_products_for_goterm and goaf.get_all_terms_for_product functions. The algorithm excludes any associations whose category doesn't match go_categories already in
                                   the GOAF file read phase - lines not containing a desired category (from go_categories) won't be read.
@@ -141,104 +144,109 @@
                 return "biological_process"
             case "F":  # molecular function in https requests when querying GO Terms associated with gene ids is returned as molecular_activity
                 return "molecular_activity"
             case "C":
                 return "cellular_component"
         return None
 
-    def get_all_products_for_goterm(self, goterm_id: str) -> List[str]:
+    def get_all_products_for_goterm(self, goterm_id: str, indirect_annotations:bool=False, obo_parser:OboParser=None) -> List[str]:
         """
         This method returns all unique products associated with the GO term id.
         The return of this function is influenced by the go_categories supplied to the constructor of the GOAF!
 
         Args:
-            goterm_id (str): a GO Term identifier, eg. GO:0003723
+          - (str) goterm_id: a GO Term identifier, eg. GO:0003723
+          - (bool) indirect_annotations: if True, will return a list of unique products for the specified goterm_id and for all of the children goterms of the 'goterm_id'
+          - (OboParser) obo_parser: an OboParser instance, to prevent recalculations. If no OboParser is passed, then this function will attempt to call OboParser() to create an OboParser instance.
 
         Returns:
             List[str]: a List of all product (gene/gene products) gene names, eg. ['NUDT4B', ...]
 
         Example: for 'GO:0003723' it returns ['KMT2C', 'CLNS1A', 'ZCCHC9', 'TERT', 'BUD23', 'DDX19B', 'CCAR2', 'NAP1L4', 'SAMSN1', 'ERVK-9', 'COA6', 'RTF1', 'AHCYL1', 'SMARCA4', ... (total len = 1378)]
         """
 
         if self.terms_dict is None:
             self.populate_terms_dict()
 
-        return self.terms_dict.get(goterm_id, [])
+        direct_products = self.terms_dict.get(goterm_id, [])
+        if indirect_annotations == False:
+            return direct_products
+        else:
+            if obo_parser is None:
+                obo_parser = OboParser()
+
+            indirect_products = []
+            child_goterm_ids = obo_parser.get_child_terms(goterm_id)
+            for child_goterm_id in child_goterm_ids:
+                child_products = self.terms_dict.get(child_goterm_id, [])
+                indirect_products += child_products
+            
+            return set(direct_products + indirect_products)
+            
 
     def populate_poducts_dict(self):
         """
         For each line in the readlines of the GO Annotations File, it creates a connection between a product gene name and an associated GO Term.
 
         The result is a dictionary (self.products_dict), mapping keys (product gene names, eg. NUDT4B) to a List of all associated
         GO Terms (eg. ['GO:0003723', ...])
         """
         self.products_dict = {}
-        for (
-            line
-        ) in (
-            self._readlines
-        ):  # example line: 'UniProtKB \t A0A024RBG1 \t NUDT4B \t enables \t GO:0003723 \t GO_REF:0000043 \t IEA \t UniProtKB-KW:KW-0694 \t F \t Diphosphoinositol polyphosphate phosphohydrolase NUDT4B \t NUDT4B \t protein \t taxon:9606 \t 20230306 \t UniProt'
+        for line in self._readlines:  # example line: 'UniProtKB \t A0A024RBG1 \t NUDT4B \t enables \t GO:0003723 \t GO_REF:0000043 \t IEA \t UniProtKB-KW:KW-0694 \t F \t Diphosphoinositol polyphosphate phosphohydrolase NUDT4B \t NUDT4B \t protein \t taxon:9606 \t 20230306 \t UniProt'
             chunks = line.split("\t")
-            self.products_dict.setdefault(chunks[2], set()).add(
-                chunks[4]
-            )  # create a key with the line's product gene name (if the key already exists, don't re-create the key - specified by the setdefault method) and add the associated GO Term to the value set. eg. {'NUDT4B': {'GO:0003723'}}, after first line is processed, {'NUDT4B': {'GO:0003723'}, 'NUDT4B': {'GO:0046872'}} after second line ...
-        for (
-            key,
-            values,
-        ) in (
-            self.products_dict.items()
-        ):  # the set() above prevents the value elements (GO Terms) in dictionary to be repeated
-            self.products_dict[key] = list(
-                values
-            )  # converts the set to a List, eg. {'NUDT4B': ['GO:0003723']}
+            self.products_dict.setdefault(chunks[2], set()).add(chunks[4])  # create a key with the line's product gene name (if the key already exists, don't re-create the key - specified by the setdefault method) and add the associated GO Term to the value set. eg. {'NUDT4B': {'GO:0003723'}}, after first line is processed, {'NUDT4B': {'GO:0003723'}, 'NUDT4B': {'GO:0046872'}} after second line ...
+        for key,values in self.products_dict.items():  # the set() above prevents the value elements (GO Terms) in dictionary to be repeated
+            self.products_dict[key] = list(values)  # converts the set to a List, eg. {'NUDT4B': ['GO:0003723']}
 
     def populate_terms_dict(self):
         """
         For each line in the readlines of the GO Annotations File, it creates a connection between a GO Term and it's associated product gene name.
 
         The result is a dictionary (self.terms_dict), mapping keys (GO Terms, eg. GO:0003723) to a List of all
         associated product gene names (eg. ['NUDT4B', ...])
         """
         self.terms_dict = {}
-        for (
-            line
-        ) in (
-            self._readlines
-        ):  # example line: 'UniProtKB \t A0A024RBG1 \t NUDT4B \t enables \t GO:0003723 \t GO_REF:0000043 \t IEA \t UniProtKB-KW:KW-0694 \t F \t Diphosphoinositol polyphosphate phosphohydrolase NUDT4B \t NUDT4B \t protein \t taxon:9606 \t 20230306 \t UniProt'
+        for line in self._readlines:  # example line: 'UniProtKB \t A0A024RBG1 \t NUDT4B \t enables \t GO:0003723 \t GO_REF:0000043 \t IEA \t UniProtKB-KW:KW-0694 \t F \t Diphosphoinositol polyphosphate phosphohydrolase NUDT4B \t NUDT4B \t protein \t taxon:9606 \t 20230306 \t UniProt'
             chunks = line.split("\t")
-            self.terms_dict.setdefault(chunks[4], set()).add(
-                chunks[2]
-            )  # create a key with the line's GO Term (if the key already exists, don't re-create the key - specified by the setdefault method) and add the product' gene name to the value set. eg. {'GO:0003723': {'NUDT4B'}}, after first line is processed, {'GO:0003723': {'NUDT4B'}, 'GO:0046872': {'NUDT4B'}} after second line ...
-        for (
-            key,
-            values,
-        ) in (
-            self.terms_dict.items()
-        ):  # the previous set() prevents the value elements (product gene names) in dictionary to be repeated
-            self.terms_dict[key] = list(
-                values
-            )  # converts the set to a List, eg. {'NUDT4B': ['GO:0003723']}
+            self.terms_dict.setdefault(chunks[4], set()).add(chunks[2])  # create a key with the line's GO Term (if the key already exists, don't re-create the key - specified by the setdefault method) and add the product' gene name to the value set. eg. {'GO:0003723': {'NUDT4B'}}, after first line is processed, {'GO:0003723': {'NUDT4B'}, 'GO:0046872': {'NUDT4B'}} after second line ...
+        for key,values in self.terms_dict.items():  # the previous set() prevents the value elements (product gene names) in dictionary to be repeated
+            self.terms_dict[key] = list(values)  # converts the set to a List, eg. {'NUDT4B': ['GO:0003723']}
 
-    def get_all_terms_for_product(self, product: str) -> List[str]:
+    def get_all_terms_for_product(self, product: str, indirect_annotations:bool=False, obo_parser:OboParser=None) -> List[str]:
         """
         Gets all GO Terms associated to a product gene name.
         The return of this function is influenced by the go_categories supplied to the constructor of the GOAF!
 
         Args:
           - (str) product: must be a gene name corresponding to a specific gene/gene product, eg. NUDT4B
+          - (bool) indirect_annotations: if True, will also return all indirectly annotated terms for product (ie. all children of directly annotated terms in the GOAF)
+          - (OboParser) obo_parser: an OboParser instance, to prevent recalculations. If no OboParser is passed, then this function will attempt to call OboParser() to create an OboParser instance.
 
         Returns:
           - List[str]: a List of all GO Term ids associated with the input product's gene name
 
         Example: for 'NUDT4B', it returns ['GO:1901911', 'GO:0071543', 'GO:0005737', 'GO:0000298', 'GO:0005634', 'GO:0034431', 'GO:0034432', 'GO:0046872', 'GO:0008486', 'GO:1901909', 'GO:0003723', 'GO:1901907', 'GO:0005829']
         """
         if self.products_dict is None:
             self.populate_poducts_dict()
 
-        return self.products_dict.get(product, [])
+        direct_annotations = self.products_dict.get(product, [])
+        if indirect_annotations == False:
+            return direct_annotations
+        else:
+            if obo_parser is None:
+                obo_parser = OboParser()
+
+            indirect_annotations = []
+            for goterm_id in direct_annotations:
+                children = obo_parser.get_child_terms(goterm_id)
+                indirect_annotations += children
+            
+            return (direct_annotations + indirect_annotations)
+
 
     def get_all_terms(self) -> List[str]:
         """
         Returns a List of all unique GO Terms read from the GO Annotations file.
         In the current (27_04_2023) GO Annotation File, there are 18880 unique GO Terms.
 
         The return of this function is influenced by the go_categories supplied to the constructor of the GOAF!
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `goreverselookup-1.0.8/src/goreverselookup/parse/OBOParser.py` & `goreverselookup-1.0.9/src/goreverselookup/parse/OBOParser.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,42 @@
 import networkx as nx
 import os
+from typing import Set, List, Dict, Optional
 
-from ..core.GOTerm import GOTerm
 from ..util.Timer import Timer
 
 import logging
 
 # from logging import config
 # config.fileConfig("../logging_config.py")
 logger = logging.getLogger(__name__)
 
+# workaround class, as importing GOTerm would cause a circular import
+class GOTerm_placeholder:
+    def __init__(self, id: str, processes: List[Dict] = None, name: Optional[str] = None, description: Optional[str] = None, category: Optional[str] = None, parent_term_ids: Optional[List[str]] = None, is_obsolete:bool = False, weight: float = 1.0, products: List[str] = [], http_error_codes:dict={}):
+        """
+        A placeholder class to construct GO Terms
+
+        Args:
+            id (str): The ID of the GO term.
+            name (str): Name (optional).
+            description (str): A description of the GO term (optional).
+            products (list): Products associated with the term (optional).
+            category (str): biological_process, molecular_activity or cellular_component
+            parent_term_ids (list[str]): GO ids of the parent terms (parsed from .obo)
+            is_obsolete (bool): if the term is labelled as obsolete in the .obo file
+        """
+        self.id = id
+        self.name = name
+        self.description = description
+        self.products = products
+        self.category = category
+        self.parent_term_ids = parent_term_ids
+        self.is_obsolete = is_obsolete
+
 
 class OboParser:
     def __init__(self, obo_filepath: str = "app/goreverselookup/data_files/go.obo"):
         """
         Parses the Gene Ontology OBO file.
 
         Params:
@@ -65,15 +88,15 @@
                     if (
                         term_data["id"] is not None
                     ):  # term_data != _reset_term_data check is used so that if all values in JSON are none, the goterm creation block isn't executed
                         # 'is_obsolete' is not present in all GO Terms. If it isn't present, set 'is_obsolete' to false
                         if "is_obsolete" not in term_data:
                             term_data["is_obsolete"] = False
 
-                        current_goterm = GOTerm(
+                        current_goterm = GOTerm_placeholder(
                             id=term_data["id"],
                             name=term_data["name"],
                             category=term_data["category"],
                             description=term_data["description"],
                             parent_term_ids=term_data["parent_term_ids"],
                             is_obsolete=term_data["is_obsolete"],
                         )
@@ -85,60 +108,52 @@
                     line_value = chunks[1]
                     match line_identifier:
                         case "id":
                             term_data["id"] = line_value
                         case "name":
                             term_data["name"] = line_value
                         case "def":
-                            line_value = line_value.strip(
-                                '"'
-                            )  # definition line value contains double quotes in obo, strip them
+                            line_value = line_value.strip('"')  # definition line value contains double quotes in obo, strip them
                             term_data["description"] = line_value
                         case "namespace":
                             term_data["category"] = line_value
                         case "is_a":
-                            line_value = line_value.split(" ")[
-                                0
-                            ]  # GO:0000090 ! mitotic anaphase -> split into GO:0000090
+                            line_value = line_value.split(" ")[0]  # GO:0000090 ! mitotic anaphase -> split into GO:0000090
                             term_data["parent_term_ids"].append(line_value)
                         case "is_obsolete":
                             is_obsolete = True if line_value == "true" else False
                             term_data["is_obsolete"] = is_obsolete
 
         # all go terms from OBO are now constructed as GOTerm objects in all_goterms dictionary
         # create a Direcected Acyclic Graph from the created GO Terms
         for goid, goterm in all_goterms.items():
-            assert isinstance(goterm, GOTerm)
+            assert isinstance(goterm, GOTerm_placeholder)
             if dag.has_node(goterm.id) is False:
                 dag.add_node(goterm.id)
             for parent_id in goterm.parent_term_ids:
                 # nodes are automatically added if they are not yet in the graph when using add_edge
                 dag.add_edge(all_goterms[parent_id].id, goterm.id)
 
         self.filepath = obo_filepath
         self.dag = dag
         self.all_goterms = all_goterms
-        self.previously_computed_parents_cache = (
-            {}
-        )  # cache dictionary between already computed goterms and their parents
-        self.previously_computed_children_cache = (
-            {}
-        )  # cache dictionary between already computed goterms and their children
+        self.previously_computed_parents_cache = {}  # cache dictionary between already computed goterms and their parents
+        self.previously_computed_children_cache = {} # cache dictionary between already computed goterms and their children
         logger.info("Obo parser init completed.")
 
     def get_parent_terms(
-        self, term_id: str, return_as_class: bool = False, ordered: bool = True
+        self, term_id: str, return_as_json:bool = False, ordered: bool = True
     ):
         """
         Gets all of GO Term parents of 'term_id'.
 
         Parameters:
           - (str) term_id: The GO Term whose parents you wish to obtain
-          - (bool) return_as_class: If False, will return a list of string ids of parent GO Terms.
-                                    If True, will return a list of GO Term parent classes.
+          - (bool) return_as_json: If False, will return a list of string ids of parent GO Terms.
+                                    If True, will return a list of GO Term parents represented as JSON objects, with the following structure: {'id':xxxx, 'name':xxxx, 'description':xxxxx, 'products':[...], 'category':xxxx, 'parent_term_ids':[...], 'is_obsolete':True/False}
           - (bool) ordered: If True, parents will be returned topologically (closest parents will be listed first in the returned list)
 
         Returns: A list of parent GO Terms (either ids or classes)
         """
         # attempt to cache old data
         if term_id in self.previously_computed_parents_cache:
             return self.previously_computed_parents_cache[term_id]
@@ -158,34 +173,34 @@
             }
             # Sort ancestors by distance in ascending order
             sorted_distances = dict(sorted(distances.items(), key=lambda item: item[1]))
             ancestors = sorted_distances.keys()
         # logger.debug(f"ancestors ordering elapsed: {timer.get_elapsed_formatted('milliseconds', reset_start_time=True)}")
 
         for parent_id in ancestors:
-            if return_as_class is True:
-                parents.append(self.all_goterms[parent_id])
+            if return_as_json is True:
+                parents.append(self.all_goterms[parent_id].__dict__)
             else:
                 parents.append(parent_id)
 
         # cache
         self.previously_computed_parents_cache[term_id] = parents
 
         return parents
 
     def get_child_terms(
-        self, term_id: str, return_as_class: bool = False, ordered: bool = True
+        self, term_id: str, return_as_json: bool = False, ordered: bool = True
     ):
         """
         Gets all of GO Term children of 'term_id'.
 
         Parameters:
           - (str) term_id: The GO Term whose children you wish to obtain
-          - (bool) return_as_class: If False, will return a list of string ids of parent GO Terms.
-                                    If True, will return a list of GO Term parent classes.
+          - (bool) return_as_json: If False, will return a list of string ids of parent GO Terms.
+                                    If True, will return a list of GO Term parents represented as JSON objects, with the following structure: {'id':xxxx, 'name':xxxx, 'description':xxxxx, 'products':[...], 'category':xxxx, 'parent_term_ids':[...], 'is_obsolete':True/False}
           - (bool) ordered: If True, parents will be returned topologically (closest children will be listed first in the returned list)
 
         Returns: A list of children GO Terms (either ids or classes)
         """
         # attempt to cache old data
         if term_id in self.previously_computed_children_cache:
             return self.previously_computed_children_cache[term_id]
@@ -205,15 +220,15 @@
             }
             # Sort ancestors by distance in ascending order
             sorted_distances = dict(sorted(distances.items(), key=lambda item: item[1]))
             descendants = sorted_distances.keys()
         # logger.debug(f"descendants ordering elapsed: {timer.get_elapsed_formatted('milliseconds', reset_start_time=True)}")
 
         for child_id in descendants:
-            if return_as_class is True:
-                children.append(self.all_goterms[child_id])
+            if return_as_json is True:
+                children.append(self.all_goterms[child_id].__dict__)
             else:
                 children.append(child_id)
 
         # cache and return
         self.previously_computed_children_cache[term_id] = children
         return children
```

### Comparing `goreverselookup-1.0.8/src/goreverselookup/parse/OrthologParsers.py` & `goreverselookup-1.0.9/src/goreverselookup/parse/OrthologParsers.py`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/src/goreverselookup/util/CacheUtil.py` & `goreverselookup-1.0.9/src/goreverselookup/util/CacheUtil.py`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/src/goreverselookup/util/FileUtil.py` & `goreverselookup-1.0.9/src/goreverselookup/util/FileUtil.py`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/src/goreverselookup/util/JsonUtil.py` & `goreverselookup-1.0.9/src/goreverselookup/util/JsonUtil.py`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/src/goreverselookup/util/LogConfigLoader.py` & `goreverselookup-1.0.9/src/goreverselookup/util/LogConfigLoader.py`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/src/goreverselookup/util/Timer.py` & `goreverselookup-1.0.9/src/goreverselookup/util/Timer.py`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/src/goreverselookup/web_apis/EnsemblApi.py` & `goreverselookup-1.0.9/src/goreverselookup/web_apis/EnsemblApi.py`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/src/goreverselookup/web_apis/GOApi.py` & `goreverselookup-1.0.9/src/goreverselookup/web_apis/GOApi.py`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/src/goreverselookup/web_apis/UniprotApi.py` & `goreverselookup-1.0.9/src/goreverselookup/web_apis/UniprotApi.py`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/src/goreverselookup.egg-info/PKG-INFO` & `goreverselookup-1.0.9/src/goreverselookup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goreverselookup
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python library for Gene Ontology Reverse Lookup
 Author-email: Aljoša Škorjanc <skorjanc.aljosa@gmail.com>, Vladimir Smrkolj <vladimir.smrkolj@gmail.com>
 License: Apache License 2.0
 Keywords: gene ontology,reverse lookup
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `goreverselookup-1.0.8/src/goreverselookup.egg-info/SOURCES.txt` & `goreverselookup-1.0.9/src/goreverselookup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/tests/conftest.py` & `goreverselookup-1.0.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/tests/no_test_main_model.py` & `goreverselookup-1.0.9/tests/no_test_main_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,12 +44,12 @@
 nterms_score = nterms(model)
 adv_prod_score = adv_product_score(model)
 binom_score = binomial_test(model)
 fisher_score = fisher_exact_test(model)
 model.score_products(
     score_classes=[nterms_score, adv_prod_score, binom_score, fisher_score]
 )
-model.model_settings.pvalue = 0.10  # set pvalue to be used in statistical analysis
+# model.model_settings.pvalue = 0.10  # set pvalue to be used in statistical analysis
 model.perform_statistical_analysis(
     test_name="fisher_test", filepath="results/statistically_relevant_genes.json"
 )
 model.save_model("results/data.json")
```

### Comparing `goreverselookup-1.0.8/tests/no_test_main_workflows.py` & `goreverselookup-1.0.9/tests/no_test_main_workflows.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 # This file demonstrates how to run the analysis using Workflows.
 
 # import
 import os
 from goreverselookup import PrimaryWorkflow
 from goreverselookup import Cacher
 from goreverselookup import LogConfigLoader
-
 # setup logger
 import logging
 
 # logger = logging.getLogger(__name__)
 # logger.addHandler(logging.StreamHandler) # this doesn't work on windows
 LogConfigLoader.setup_logging_config(log_config_json_filepath="logging_config.json")
 logger = logging.getLogger(__name__)
 
 logger.info("Starting Workflows Test!")
 logger.info(f"os.getcwd() =  {os.getcwd()}")
 
 # setup and run workflows
 Cacher.init(cache_dir="cache")
 # Cacher.clear_cache("ALL")
-workflow = PrimaryWorkflow(
-    input_file_fpath="input_files/input.txt", save_folder_dir="results"
-)
+workflow = PrimaryWorkflow(input_file_fpath="input_files/input.txt", save_folder_dir="results")
 workflow.run_workflow()
```

### Comparing `goreverselookup-1.0.8/tests/no_test_playground.py` & `goreverselookup-1.0.9/tests/no_test_playground.py`

 * *Files identical despite different names*

### Comparing `goreverselookup-1.0.8/tests/test_webapis.py` & `goreverselookup-1.0.9/tests/test_webapis.py`

 * *Files identical despite different names*

