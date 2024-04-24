# Comparing `tmp/pytctracer-0.1.9.tar.gz` & `tmp/pytctracer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytctracer-0.1.9.tar", last modified: Fri Apr  5 16:25:03 2024, max compression
+gzip compressed data, was "pytctracer-0.2.0.tar", last modified: Wed Apr 24 03:17:28 2024, max compression
```

## Comparing `pytctracer-0.1.9.tar` & `pytctracer-0.2.0.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.171188 pytctracer-0.1.9/
--rw-r--r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1789 2024-04-05 16:25:03.171188 pytctracer-0.1.9/PKG-INFO
--rwxr-xr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)      863 2024-04-05 16:22:58.000000 pytctracer-0.1.9/README.md
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.163188 pytctracer-0.1.9/data/
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.159188 pytctracer-0.1.9/data/ground-truth-data/
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.163188 pytctracer-0.1.9/data/ground-truth-data/pyopenssl/
--rwxr-xr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)    14927 2023-12-12 17:26:56.000000 pytctracer-0.1.9/data/ground-truth-data/pyopenssl/pyopenssl_all_functions.py
--rwxr-xr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)     2737 2024-01-17 14:14:19.000000 pytctracer-0.1.9/data/ground-truth-data/pyopenssl/pyopenssl_chosen_tests.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     2240 2024-03-21 02:03:31.000000 pytctracer-0.1.9/data/t.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      464 2024-02-25 02:21:54.000000 pytctracer-0.1.9/data/tes.py
--rwxr-xr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)    83796 2024-03-28 11:46:42.000000 pytctracer-0.1.9/data/trace_parser_dynamic.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1019 2024-04-05 16:24:32.000000 pytctracer-0.1.9/pyproject.toml
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.163188 pytctracer-0.1.9/pytctracer/
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      104 2024-03-31 18:38:21.000000 pytctracer-0.1.9/pytctracer/__init__.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)    19254 2024-04-03 23:07:28.000000 pytctracer-0.1.9/pytctracer/analyser.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     9390 2024-04-03 23:07:08.000000 pytctracer-0.1.9/pytctracer/cli.py
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.163188 pytctracer-0.1.9/pytctracer/config/
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)       49 2024-03-30 00:46:49.000000 pytctracer-0.1.9/pytctracer/config/__init__.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      821 2024-03-30 14:16:16.000000 pytctracer-0.1.9/pytctracer/config/config.py
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.167188 pytctracer-0.1.9/pytctracer/config/constants/
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      904 2024-04-03 23:07:54.000000 pytctracer-0.1.9/pytctracer/config/constants/__init__.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      180 2024-04-03 23:05:28.000000 pytctracer-0.1.9/pytctracer/config/constants/classification_type.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      380 2024-04-03 23:05:47.000000 pytctracer-0.1.9/pytctracer/config/constants/event_type.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      216 2024-04-03 23:05:58.000000 pytctracer-0.1.9/pytctracer/config/constants/function_type.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      129 2024-04-03 23:06:06.000000 pytctracer-0.1.9/pytctracer/config/constants/instruction_opname.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)       99 2024-04-03 23:07:08.000000 pytctracer-0.1.9/pytctracer/config/constants/level_type.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      202 2024-04-03 23:07:13.000000 pytctracer-0.1.9/pytctracer/config/constants/metric_score_type.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      535 2024-04-03 23:07:28.000000 pytctracer-0.1.9/pytctracer/config/constants/technique_parameter.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      298 2024-04-03 23:07:36.000000 pytctracer-0.1.9/pytctracer/config/constants/technique_threshold.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      149 2024-04-03 23:07:44.000000 pytctracer-0.1.9/pytctracer/config/constants/testing_method_event_type.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      572 2024-04-03 23:07:50.000000 pytctracer-0.1.9/pytctracer/config/constants/trace_data_header.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      507 2024-04-03 23:07:54.000000 pytctracer-0.1.9/pytctracer/config/constants/trace_data_variable.py
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.167188 pytctracer-0.1.9/pytctracer/evaluation/
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      170 2024-03-26 14:14:33.000000 pytctracer-0.1.9/pytctracer/evaluation/__init__.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1325 2024-04-03 23:05:28.000000 pytctracer-0.1.9/pytctracer/evaluation/classify_predictions.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1234 2024-04-03 23:07:13.000000 pytctracer-0.1.9/pytctracer/evaluation/evaluate_predictions.py
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.167188 pytctracer-0.1.9/pytctracer/evaluation/metrics/
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      613 2024-03-30 00:46:46.000000 pytctracer-0.1.9/pytctracer/evaluation/metrics/__init__.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1581 2024-04-03 23:07:13.000000 pytctracer-0.1.9/pytctracer/evaluation/metrics/area_under_curve.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     2967 2024-03-30 00:46:45.000000 pytctracer-0.1.9/pytctracer/evaluation/metrics/arg_name_to_metric_mapper.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      914 2024-04-03 23:07:13.000000 pytctracer-0.1.9/pytctracer/evaluation/metrics/f1.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      989 2024-04-03 23:07:13.000000 pytctracer-0.1.9/pytctracer/evaluation/metrics/false_negatives.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      989 2024-04-03 23:07:13.000000 pytctracer-0.1.9/pytctracer/evaluation/metrics/false_positives.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1470 2024-04-03 23:07:13.000000 pytctracer-0.1.9/pytctracer/evaluation/metrics/mean_average_precision.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      744 2024-04-03 23:07:13.000000 pytctracer-0.1.9/pytctracer/evaluation/metrics/metric.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1084 2024-04-03 23:07:13.000000 pytctracer-0.1.9/pytctracer/evaluation/metrics/precision.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1060 2024-04-03 23:07:13.000000 pytctracer-0.1.9/pytctracer/evaluation/metrics/recall.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      995 2024-04-03 23:07:13.000000 pytctracer-0.1.9/pytctracer/evaluation/metrics/true_positives.py
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.167188 pytctracer-0.1.9/pytctracer/io/
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-03-30 00:46:30.000000 pytctracer-0.1.9/pytctracer/io/__init__.py
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.167188 pytctracer-0.1.9/pytctracer/io/input/
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      110 2024-03-30 00:46:37.000000 pytctracer-0.1.9/pytctracer/io/input/__init__.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      920 2024-03-30 00:46:37.000000 pytctracer-0.1.9/pytctracer/io/input/from_file.py
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.167188 pytctracer-0.1.9/pytctracer/io/output/
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      367 2024-03-30 00:46:35.000000 pytctracer-0.1.9/pytctracer/io/output/__init__.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1714 2024-03-30 00:46:34.000000 pytctracer-0.1.9/pytctracer/io/output/to_display.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1097 2024-03-30 14:22:59.000000 pytctracer-0.1.9/pytctracer/io/output/to_file.py
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.167188 pytctracer-0.1.9/pytctracer/parsing/
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1382 2024-03-30 00:46:28.000000 pytctracer-0.1.9/pytctracer/parsing/__init__.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     5292 2024-04-03 23:07:50.000000 pytctracer-0.1.9/pytctracer/parsing/find_class_level_calls.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1274 2024-04-03 23:07:50.000000 pytctracer-0.1.9/pytctracer/parsing/find_class_level_names.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     4728 2024-04-03 23:07:50.000000 pytctracer-0.1.9/pytctracer/parsing/find_function_level_calls.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1214 2024-04-03 23:07:50.000000 pytctracer-0.1.9/pytctracer/parsing/find_function_level_names.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     3403 2024-04-03 23:07:50.000000 pytctracer-0.1.9/pytctracer/parsing/functions_called_before_assert.py
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.171188 pytctracer-0.1.9/pytctracer/techniques/
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      883 2024-03-27 16:49:38.000000 pytctracer-0.1.9/pytctracer/techniques/__init__.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     3749 2024-03-30 00:46:03.000000 pytctracer-0.1.9/pytctracer/techniques/arg_name_to_technique_mapper.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1553 2024-04-03 23:07:36.000000 pytctracer-0.1.9/pytctracer/techniques/combined.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     4021 2024-04-03 23:07:28.000000 pytctracer-0.1.9/pytctracer/techniques/last_call_before_assert.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     4735 2024-04-03 23:07:36.000000 pytctracer-0.1.9/pytctracer/techniques/levenshtein_distance.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)    10083 2024-04-03 23:07:36.000000 pytctracer-0.1.9/pytctracer/techniques/longest_common_subsequence.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     6032 2024-04-03 23:07:28.000000 pytctracer-0.1.9/pytctracer/techniques/naming_conventions.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     4613 2024-04-03 23:07:37.000000 pytctracer-0.1.9/pytctracer/techniques/tarantula.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     5544 2024-03-30 14:24:31.000000 pytctracer-0.1.9/pytctracer/techniques/technique.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)    10121 2024-04-03 23:07:37.000000 pytctracer-0.1.9/pytctracer/techniques/tfidf.py
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)    20952 2024-04-03 23:07:54.000000 pytctracer-0.1.9/pytctracer/tracer.py
-drwxrwxr-x   0 jasonho2582001  (1001) jasonho2582001  (1001)        0 2024-04-05 16:25:03.171188 pytctracer-0.1.9/pytctracer.egg-info/
--rw-r--r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     1789 2024-04-05 16:25:03.000000 pytctracer-0.1.9/pytctracer.egg-info/PKG-INFO
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)     2634 2024-04-05 16:25:03.000000 pytctracer-0.1.9/pytctracer.egg-info/SOURCES.txt
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)        1 2024-04-05 16:25:03.000000 pytctracer-0.1.9/pytctracer.egg-info/dependency_links.txt
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)       50 2024-04-05 16:25:03.000000 pytctracer-0.1.9/pytctracer.egg-info/entry_points.txt
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)      145 2024-04-05 16:25:03.000000 pytctracer-0.1.9/pytctracer.egg-info/requires.txt
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)       21 2024-04-05 16:25:03.000000 pytctracer-0.1.9/pytctracer.egg-info/top_level.txt
--rw-rw-r--   0 jasonho2582001  (1001) jasonho2582001  (1001)       38 2024-04-05 16:25:03.171188 pytctracer-0.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.413494 pytctracer-0.2.0/
+-rw-rw-rw-   0        0        0    17287 2024-04-24 03:17:28.411855 pytctracer-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    16293 2024-04-24 03:00:56.000000 pytctracer-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.291186 pytctracer-0.2.0/data/
+drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.278504 pytctracer-0.2.0/data/ground-truth-data/
+drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.293703 pytctracer-0.2.0/data/ground-truth-data/pyopenssl/
+-rw-rw-rw-   0        0        0    14927 2023-12-12 17:26:56.000000 pytctracer-0.2.0/data/ground-truth-data/pyopenssl/pyopenssl_all_functions.py
+-rw-rw-rw-   0        0        0     2737 2024-01-17 14:14:19.000000 pytctracer-0.2.0/data/ground-truth-data/pyopenssl/pyopenssl_chosen_tests.py
+-rw-rw-rw-   0        0        0     2195 2024-04-09 23:53:27.000000 pytctracer-0.2.0/data/t.py
+-rw-rw-rw-   0        0        0      464 2024-02-25 02:21:54.000000 pytctracer-0.2.0/data/tes.py
+-rw-rw-rw-   0        0        0    81882 2024-04-10 01:44:54.000000 pytctracer-0.2.0/data/trace_parser_dynamic.py
+-rw-rw-rw-   0        0        0     1045 2024-04-24 03:16:49.000000 pytctracer-0.2.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.299840 pytctracer-0.2.0/pytctracer/
+-rw-rw-rw-   0        0        0      104 2024-03-31 18:38:21.000000 pytctracer-0.2.0/pytctracer/__init__.py
+-rw-rw-rw-   0        0        0    19325 2024-04-24 00:24:50.000000 pytctracer-0.2.0/pytctracer/analyser.py
+-rw-rw-rw-   0        0        0     9121 2024-04-24 00:28:28.000000 pytctracer-0.2.0/pytctracer/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.337488 pytctracer-0.2.0/pytctracer/config/
+-rw-rw-rw-   0        0        0       49 2024-03-30 00:46:49.000000 pytctracer-0.2.0/pytctracer/config/__init__.py
+-rw-rw-rw-   0        0        0     1101 2024-04-24 01:08:28.000000 pytctracer-0.2.0/pytctracer/config/config.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.354537 pytctracer-0.2.0/pytctracer/config/constants/
+-rw-rw-rw-   0        0        0      904 2024-04-03 23:07:54.000000 pytctracer-0.2.0/pytctracer/config/constants/__init__.py
+-rw-rw-rw-   0        0        0      180 2024-04-03 23:05:28.000000 pytctracer-0.2.0/pytctracer/config/constants/classification_type.py
+-rw-rw-rw-   0        0        0      380 2024-04-03 23:05:47.000000 pytctracer-0.2.0/pytctracer/config/constants/event_type.py
+-rw-rw-rw-   0        0        0      216 2024-04-03 23:05:58.000000 pytctracer-0.2.0/pytctracer/config/constants/function_type.py
+-rw-rw-rw-   0        0        0      129 2024-04-03 23:06:06.000000 pytctracer-0.2.0/pytctracer/config/constants/instruction_opname.py
+-rw-rw-rw-   0        0        0       99 2024-04-03 23:07:08.000000 pytctracer-0.2.0/pytctracer/config/constants/level_type.py
+-rw-rw-rw-   0        0        0      202 2024-04-03 23:07:13.000000 pytctracer-0.2.0/pytctracer/config/constants/metric_score_type.py
+-rw-rw-rw-   0        0        0      535 2024-04-03 23:07:28.000000 pytctracer-0.2.0/pytctracer/config/constants/technique_parameter.py
+-rw-rw-rw-   0        0        0      915 2024-04-24 01:14:30.000000 pytctracer-0.2.0/pytctracer/config/constants/technique_threshold.py
+-rw-rw-rw-   0        0        0      149 2024-04-03 23:07:44.000000 pytctracer-0.2.0/pytctracer/config/constants/testing_method_event_type.py
+-rw-rw-rw-   0        0        0      572 2024-04-03 23:07:50.000000 pytctracer-0.2.0/pytctracer/config/constants/trace_data_header.py
+-rw-rw-rw-   0        0        0      507 2024-04-03 23:07:54.000000 pytctracer-0.2.0/pytctracer/config/constants/trace_data_variable.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.358893 pytctracer-0.2.0/pytctracer/evaluation/
+-rw-rw-rw-   0        0        0      170 2024-03-26 14:14:33.000000 pytctracer-0.2.0/pytctracer/evaluation/__init__.py
+-rw-rw-rw-   0        0        0     2358 2024-04-24 01:05:02.000000 pytctracer-0.2.0/pytctracer/evaluation/classify_predictions.py
+-rw-rw-rw-   0        0        0     2808 2024-04-24 01:06:16.000000 pytctracer-0.2.0/pytctracer/evaluation/evaluate_predictions.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.373440 pytctracer-0.2.0/pytctracer/evaluation/metrics/
+-rw-rw-rw-   0        0        0      613 2024-03-30 00:46:46.000000 pytctracer-0.2.0/pytctracer/evaluation/metrics/__init__.py
+-rw-rw-rw-   0        0        0     1581 2024-04-03 23:07:13.000000 pytctracer-0.2.0/pytctracer/evaluation/metrics/area_under_curve.py
+-rw-rw-rw-   0        0        0     2967 2024-03-30 00:46:45.000000 pytctracer-0.2.0/pytctracer/evaluation/metrics/arg_name_to_metric_mapper.py
+-rw-rw-rw-   0        0        0      914 2024-04-03 23:07:13.000000 pytctracer-0.2.0/pytctracer/evaluation/metrics/f1.py
+-rw-rw-rw-   0        0        0      989 2024-04-03 23:07:13.000000 pytctracer-0.2.0/pytctracer/evaluation/metrics/false_negatives.py
+-rw-rw-rw-   0        0        0      989 2024-04-03 23:07:13.000000 pytctracer-0.2.0/pytctracer/evaluation/metrics/false_positives.py
+-rw-rw-rw-   0        0        0     1470 2024-04-03 23:07:13.000000 pytctracer-0.2.0/pytctracer/evaluation/metrics/mean_average_precision.py
+-rw-rw-rw-   0        0        0      744 2024-04-03 23:07:13.000000 pytctracer-0.2.0/pytctracer/evaluation/metrics/metric.py
+-rw-rw-rw-   0        0        0     1084 2024-04-03 23:07:13.000000 pytctracer-0.2.0/pytctracer/evaluation/metrics/precision.py
+-rw-rw-rw-   0        0        0     1060 2024-04-03 23:07:13.000000 pytctracer-0.2.0/pytctracer/evaluation/metrics/recall.py
+-rw-rw-rw-   0        0        0      995 2024-04-03 23:07:13.000000 pytctracer-0.2.0/pytctracer/evaluation/metrics/true_positives.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.375742 pytctracer-0.2.0/pytctracer/io/
+-rw-rw-rw-   0        0        0        0 2024-03-30 00:46:30.000000 pytctracer-0.2.0/pytctracer/io/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.377740 pytctracer-0.2.0/pytctracer/io/input/
+-rw-rw-rw-   0        0        0      110 2024-03-30 00:46:37.000000 pytctracer-0.2.0/pytctracer/io/input/__init__.py
+-rw-rw-rw-   0        0        0     2337 2024-04-24 01:04:25.000000 pytctracer-0.2.0/pytctracer/io/input/from_file.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.382738 pytctracer-0.2.0/pytctracer/io/output/
+-rw-rw-rw-   0        0        0      367 2024-03-30 00:46:35.000000 pytctracer-0.2.0/pytctracer/io/output/__init__.py
+-rw-rw-rw-   0        0        0     3167 2024-04-24 01:02:45.000000 pytctracer-0.2.0/pytctracer/io/output/to_display.py
+-rw-rw-rw-   0        0        0     2372 2024-04-24 01:00:34.000000 pytctracer-0.2.0/pytctracer/io/output/to_file.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.392564 pytctracer-0.2.0/pytctracer/parsing/
+-rw-rw-rw-   0        0        0     1382 2024-03-30 00:46:28.000000 pytctracer-0.2.0/pytctracer/parsing/__init__.py
+-rw-rw-rw-   0        0        0     7243 2024-04-24 00:56:25.000000 pytctracer-0.2.0/pytctracer/parsing/find_class_level_calls.py
+-rw-rw-rw-   0        0        0     2124 2024-04-24 00:54:18.000000 pytctracer-0.2.0/pytctracer/parsing/find_class_level_names.py
+-rw-rw-rw-   0        0        0     6552 2024-04-24 00:53:40.000000 pytctracer-0.2.0/pytctracer/parsing/find_function_level_calls.py
+-rw-rw-rw-   0        0        0     2032 2024-04-24 00:51:05.000000 pytctracer-0.2.0/pytctracer/parsing/find_function_level_names.py
+-rw-rw-rw-   0        0        0     4285 2024-04-24 00:49:28.000000 pytctracer-0.2.0/pytctracer/parsing/functions_called_before_assert.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.408011 pytctracer-0.2.0/pytctracer/techniques/
+-rw-rw-rw-   0        0        0      883 2024-03-27 16:49:38.000000 pytctracer-0.2.0/pytctracer/techniques/__init__.py
+-rw-rw-rw-   0        0        0     4333 2024-04-24 00:24:31.000000 pytctracer-0.2.0/pytctracer/techniques/arg_name_to_technique_mapper.py
+-rw-rw-rw-   0        0        0     3510 2024-04-24 00:47:26.000000 pytctracer-0.2.0/pytctracer/techniques/combined.py
+-rw-rw-rw-   0        0        0     4021 2024-04-03 23:07:28.000000 pytctracer-0.2.0/pytctracer/techniques/last_call_before_assert.py
+-rw-rw-rw-   0        0        0     5118 2024-04-24 00:41:57.000000 pytctracer-0.2.0/pytctracer/techniques/levenshtein_distance.py
+-rw-rw-rw-   0        0        0    11089 2024-04-24 00:41:20.000000 pytctracer-0.2.0/pytctracer/techniques/longest_common_subsequence.py
+-rw-rw-rw-   0        0        0     6043 2024-04-24 00:40:03.000000 pytctracer-0.2.0/pytctracer/techniques/naming_conventions.py
+-rw-rw-rw-   0        0        0     4976 2024-04-24 00:39:20.000000 pytctracer-0.2.0/pytctracer/techniques/tarantula.py
+-rw-rw-rw-   0        0        0     6966 2024-04-24 00:44:46.000000 pytctracer-0.2.0/pytctracer/techniques/technique.py
+-rw-rw-rw-   0        0        0    11270 2024-04-24 00:36:56.000000 pytctracer-0.2.0/pytctracer/techniques/tfidf.py
+-rw-rw-rw-   0        0        0    21573 2024-04-24 01:38:40.000000 pytctracer-0.2.0/pytctracer/tracer.py
+drwxrwxrwx   0        0        0        0 2024-04-24 03:17:28.410112 pytctracer-0.2.0/pytctracer.egg-info/
+-rw-rw-rw-   0        0        0    17287 2024-04-24 03:17:28.000000 pytctracer-0.2.0/pytctracer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2634 2024-04-24 03:17:28.000000 pytctracer-0.2.0/pytctracer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 03:17:28.000000 pytctracer-0.2.0/pytctracer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-24 03:17:28.000000 pytctracer-0.2.0/pytctracer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      166 2024-04-24 03:17:28.000000 pytctracer-0.2.0/pytctracer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       38 2024-04-24 03:17:28.000000 pytctracer-0.2.0/pytctracer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 03:17:28.413494 pytctracer-0.2.0/setup.cfg
```

### Comparing `pytctracer-0.1.9/data/ground-truth-data/pyopenssl/pyopenssl_all_functions.py` & `pytctracer-0.2.0/data/ground-truth-data/pyopenssl/pyopenssl_all_functions.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.9/data/ground-truth-data/pyopenssl/pyopenssl_chosen_tests.py` & `pytctracer-0.2.0/data/ground-truth-data/pyopenssl/pyopenssl_chosen_tests.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.9/data/t.py` & `pytctracer-0.2.0/data/t.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 
 kedro_class_level_analysis_path = "analysis/kedro/class/kedro_class_predictions_results.csv"
 arrow_class_level_analysis_path = "analysis/arrow/class/arrow_predictions_class_results.csv"
 pyopenssl_class_level_analysis_path = "analysis/pyopenssl/class/pyopenssl_predictions_class_results.csv"
 chartify_class_level_analysis_path = "analysis/chartify/class/chartify_predictions_class_results.csv"
 
 # Load the CSV files into DataFrames
-df1 = pd.read_csv(kedro_class_level_analysis_path)
-df2 = pd.read_csv(arrow_class_level_analysis_path)
-df3 = pd.read_csv(pyopenssl_class_level_analysis_path)
-df4 = pd.read_csv(chartify_class_level_analysis_path)
+df1 = pd.read_csv(kedro_analysis_path)
+df2 = pd.read_csv(arrow_analysis_path)
+df3 = pd.read_csv(pyopenssl_analysis_path)
+df4 = pd.read_csv(chartify_analysis_path)
 
 df1 = df1.replace({'-': 0})
 df2 = df2.replace({'-': 0})
 df3 = df3.replace({'-': 0})
 df4 = df4.replace({'-': 0})
 # Identify numeric columns
 numeric_columns = df1.select_dtypes(include=np.number).columns.tolist()
@@ -32,16 +32,16 @@
 
 for df in [df1, df2, df3, df4]:
     for col in df.columns:
         if df[col].dtype == 'float64':
             df[col] = df[col].round(3)
 
 # Ensure that all DataFrames have the same structure
-assert df1.columns.equals(df2.columns) and df1.columns.equals(df3.columns) and df1.columns.equals(df4.columns)
+assert df1.columns.equals(df2.columns) and df2.columns.equals(df3.columns) and df1.columns.equals(df4.columns)
 
 # Add the numeric columns in the DataFrames together and divide by the number of CSV files
 df_avg = df1.copy()
 for column in numeric_columns:
     df_avg[column] = ((df1[column] + df2[column] + df3[column] + df4[column]) / 4).round(1)
 
 # Save the resulting DataFrame to a new CSV file
-df_avg.to_csv('average_class.csv', index=False)
+df_avg.to_csv('average_function.csv', index=False)
```

### Comparing `pytctracer-0.1.9/data/trace_parser_dynamic.py` & `pytctracer-0.2.0/data/trace_parser_dynamic.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from typing import Optional, Set, List, Dict, Tuple
 from math import log
 import csv
 import json
 import sys
 from sklearn.metrics import precision_recall_curve, auc
 
-csv.field_size_limit(sys.maxsize)
+csv.field_size_limit(int(1e9))
 
 THRESHOLD_FOR_LCSU = 0.75
-THRESHOLD_FOR_LCSB = 0.65
+THRESHOLD_FOR_LCSB = 0.55
 THRESHOLD_FOR_LEVENSHTEIN = 0.95
 THRESHOLD_FOR_TARANTULA = 0.95
 THRESHOLD_FOR_TFIDF = 0.9
 THRESHOLD_FOR_TFIDF_COUNT = 0.9
 THRESHOLD_FOR_AVERAGE = sum(threshold_arr := [THRESHOLD_FOR_LCSU, THRESHOLD_FOR_LCSB, THRESHOLD_FOR_TFIDF_COUNT, THRESHOLD_FOR_LEVENSHTEIN, THRESHOLD_FOR_TARANTULA, THRESHOLD_FOR_TFIDF])/len(threshold_arr)
 DISCOUNT_FACTOR = 0.5
 
@@ -433,15 +433,15 @@
             tfidf_dict[test_name][function_name] = tf * idf_set[function_name]
     
     return normalise_dict(use_call_depth_discounting_dict(tfidf_dict, depths_of_functions_called_by_each_test_dict), functions_called_by_each_test_count_dict)
 
 
 def find_average_score(result_dicts: List[Dict[str, Dict[str, float]]], function_names: Set[str], test_names: Set[str], functions_called_by_each_test_dict: Dict[str, Set[str]]) -> Dict[str, Dict[str, float]]:
     average_score_dict = None
-    num_of_result_dicts = 9
+    num_of_result_dicts = len(result_dicts)
     for result_dict in result_dicts:
         if average_score_dict is None:
             average_score_dict = defaultdict(lambda: defaultdict(float))
         for test_name, res in result_dict.items():
             for function_name, score in res.items():
                 average_score_dict[test_name][function_name] += score/num_of_result_dicts
     
@@ -853,15 +853,15 @@
 
         lcsb_dict = longest_common_subsequence_both(function_names_tuple, test_names_tuple, functions_called_by_each_test_dict, depths_of_functions_called_by_each_test_dict)
         naming_conventions_dict = naming_conventions(function_names_tuple, test_names_tuple, functions_called_by_each_test_dict)
         naming_convention_contains_dict = naming_convention_contains(function_names_tuple, test_names_tuple, functions_called_by_each_test_dict)
         lcsb_dict = longest_common_subsequence_both(function_names_tuple, test_names_tuple, functions_called_by_each_test_dict, depths_of_functions_called_by_each_test_dict)
         lcsu_dict = longest_common_subsequence_unit(function_names_tuple, test_names_tuple, functions_called_by_each_test_dict, depths_of_functions_called_by_each_test_dict)
         levenshtein_dict = levenshtein_distance(function_names_tuple, test_names_tuple, functions_called_by_each_test_dict, depths_of_functions_called_by_each_test_dict)
-        lcba_dict = last_call_before_assert_class(data, fully_qualified_function_names, fully_qualified_test_names)
+        lcba_dict = last_call_before_assert(data, fully_qualified_function_names, fully_qualified_test_names)
         tarantula_dict = tarantula(functions_called_by_each_test_dict, tests_that_call_each_function_dict, fully_qualified_function_names, fully_qualified_test_names, depths_of_functions_called_by_each_test_dict)
         tfidf_dict = tfidf(functions_called_by_each_test_dict, tests_that_call_each_function_dict, fully_qualified_function_names, fully_qualified_test_names, depths_of_functions_called_by_each_test_dict)
         tfidf_count_dict = tfidf_count(functions_called_by_each_test_count_dict, tests_that_call_each_function_dict, fully_qualified_function_names, fully_qualified_test_names, depths_of_functions_called_by_each_test_dict)
         result_dicts = [naming_conventions_dict, naming_convention_contains_dict, lcsb_dict, lcsu_dict, levenshtein_dict, lcba_dict, tarantula_dict, tfidf_dict, tfidf_count_dict]
         average_dict = find_average_score(result_dicts, fully_qualified_function_names, fully_qualified_test_names, functions_called_by_each_test_dict)
 
         # PRODUCING PREDICTIONS
@@ -953,26 +953,26 @@
             for i in range(len(res_lists[0])):
                 s = 0
                 for j in range(len(res_lists)):
                     s += res_lists[j][i]
                 s /= len(res_lists)
                 final_res_dict[metric].append(s)
 
-        plt.figure(figsize=(10, 6))
+        plt.figure()
 
         # Use the 'seaborn' style
         plt.style.use('ggplot')
 
         # For each metric
         for metric in ["Precision", "Recall", "F1", "MAP"]:
             # Plot the metric values against the threshold values with increased line width
             plt.plot(thresholds, final_res_dict[metric], label=metric, linewidth=2)
 
         # Add a vertical line at threshold 0.5
-        plt.axvline(x=normal_threshold, color='black', linestyle='--', label=f't = {normal_threshold}')
+        plt.axvline(x=normal_threshold, color='black', linestyle='--', label=f't = {normal_threshold:.2f}')
         # Set the x-axis range to [0, 1]
         plt.xlim([0, 1])
         font = {
                 'weight': 'normal',
                 'size': 14,
                 'style': 'italic'}
         # Set the y-axis range to [0, 1]
@@ -981,74 +981,63 @@
         plt.yticks([0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100])
         # Add labels and title with increased font size
         plt.xlabel('Threshold', fontdict=font)
         plt.ylabel('Value',  fontdict=font)
         plt.title(title, fontsize=16)
 
         # Add a legend
-        plt.legend()
+        plt.legend(fontsize=14)
 
         # Add a grid
         plt.grid(True)
         plt.subplots_adjust(left=0.1, right=0.95, top=0.9, bottom=0.1)
         # Show the plot
         plt.show()
     
-    plot_threshold_sensitivity(lcsb_dicts, THRESHOLD_FOR_LCSB, "Threshold Sensitivity for LCS-B (Function Level)")
-    plot_threshold_sensitivity(lcsu_dicts, THRESHOLD_FOR_LCSU, "Threshold Sensitivity for LCS-U (Function Level)")
-    plot_threshold_sensitivity(levenshtein_dicts, THRESHOLD_FOR_LEVENSHTEIN, "Threshold Sensitivity for Levenshtein (Function Level)")
-    plot_threshold_sensitivity(tarantula_dicts, THRESHOLD_FOR_TARANTULA, "Threshold Sensitivity for Tarantula (Function Level)")
-    plot_threshold_sensitivity(tfidf_dicts, THRESHOLD_FOR_TFIDF, "Threshold Sensitivity for TF-IDF (Function Level)")
-    plot_threshold_sensitivity(tfidf_count_dicts, THRESHOLD_FOR_TFIDF_COUNT, "Threshold Sensitivity for TF-IDF* (Function Level)")
-    plot_threshold_sensitivity(average_dicts, THRESHOLD_FOR_AVERAGE, "Threshold Sensitivity for Combined (Function Level)")
+    plot_threshold_sensitivity(lcsb_dicts, THRESHOLD_FOR_LCSB, "LCS-B (Function Level)")
+    plot_threshold_sensitivity(lcsu_dicts, THRESHOLD_FOR_LCSU, "LCS-U (Function Level)")
+    plot_threshold_sensitivity(levenshtein_dicts, THRESHOLD_FOR_LEVENSHTEIN, "Levenshtein (Function Level)")
+    plot_threshold_sensitivity(tarantula_dicts, THRESHOLD_FOR_TARANTULA, "Tarantula (Function Level)")
+    plot_threshold_sensitivity(tfidf_dicts, THRESHOLD_FOR_TFIDF, "TF-IDF (Function Level)")
+    plot_threshold_sensitivity(tfidf_count_dicts, THRESHOLD_FOR_TFIDF_COUNT, "TF-IDF* (Function Level)")
+    plot_threshold_sensitivity(average_dicts, THRESHOLD_FOR_AVERAGE, "Combined (Function Level)")
 
 
 def vary_threshold_class():
     file_paths = ["tracing-logs/pyopenssl/pyopenssl_pytest_tracer_logs.csv",
                     "tracing-logs/arrow/arrow_pytest_tracer_logs.csv",
                   "tracing-logs/kedro/kedro_pytest_tracer_logs.csv", 
                   "tracing-logs/chartify/chartify_pytest_tracer_logs.csv"]
     ground_truth_paths = ["ground-truth-data/pyopenssl/class/pyopenssl_ground_truth_classes.json",
                           "ground-truth-data/arrow/class/arrow_ground_truth_classes.json",
                           "ground-truth-data/kedro/class/kedro_ground_truth_classes.json",
                           "ground-truth-data/chartify/class/chartify_ground_truth_classes.json"]
-    ground_truth_function_class_paths = ["ground-truth-data/pyopenssl/class/pyopenssl_all_function_class_names.txt",
-                                            "ground-truth-data/arrow/class/arrow_all_function_class_names.txt",
-                                            "ground-truth-data/kedro/class/kedro_all_function_class_names.txt",
-                                            "ground-truth-data/chartify/class/chartify_all_function_class_names.txt"]
-    
-    ground_truth_test_class_paths = ["ground-truth-data/pyopenssl/class/pyopenssl_all_test_class_names.txt",
-                                        "ground-truth-data/arrow/class/arrow_all_test_class_names.txt",
-                                        "ground-truth-data/kedro/class/kedro_all_test_class_names.txt",
-                                        "ground-truth-data/chartify/class/chartify_all_test_class_names.txt"]
+
     lcsb_dicts = []
     lcsu_dicts = []
     levenshtein_dicts = []
     tarantula_dicts = []
     tfidf_dicts = []
     tfidf_count_dicts = []
     average_dicts = []
 
     for i in range(4):
         file_path = file_paths[i]
         ground_truth_path = ground_truth_paths[i]
         ground_truth_dict = load_link_json(ground_truth_path)
-        ground_truth_function_class_path = ground_truth_function_class_paths[i]
-        ground_truth_test_class_path = ground_truth_test_class_paths[i]
         columns, data = read_csv_log(file_path)
-        ground_truth_function_class_names, ground_truth_test_class_names = extract_ground_truth_class_names(ground_truth_function_class_path, ground_truth_test_class_path)
         
-        function_names_tuple, test_names_tuple = extract_function_class_and_test_class_names_tuple(data, ground_truth_function_class_names, ground_truth_test_class_names)
+        function_names_tuple, test_names_tuple = extract_function_class_and_test_class_names_tuple(data)
         fully_qualified_function_names = set(fully_qualified_function_name for fully_qualified_function_name, _ in function_names_tuple)
         fully_qualified_test_names = set(fully_qualified_test_name for fully_qualified_test_name, _ in test_names_tuple)
-        functions_called_by_each_test_dict = find_function_classes_called_by_each_test_class(data, ground_truth_function_class_names, ground_truth_test_class_names)
-        functions_called_by_each_test_count_dict = find_function_classes_called_by_each_test_class_count(data, ground_truth_function_class_names, ground_truth_test_class_names)
-        tests_that_call_each_function_dict = find_test_classes_that_call_each_function_class(data, ground_truth_function_class_names, ground_truth_test_class_names)
+        functions_called_by_each_test_dict = find_function_classes_called_by_each_test_class(data)
+        functions_called_by_each_test_count_dict = find_function_classes_called_by_each_test_class_count(data)
+        tests_that_call_each_function_dict = find_test_classes_that_call_each_function_class(data)
         tests_to_create_links_for = set(ground_truth_dict.keys())
-        depths_of_functions_called_by_each_test_dict = find_depths_of_function_classes_called_by_each_test_class(data, ground_truth_function_class_names, ground_truth_test_class_names)
+        depths_of_functions_called_by_each_test_dict = find_depths_of_function_classes_called_by_each_test_class(data)
         
         # print(function_names_tuple)
 
         # TECHNIQUES
         naming_conventions_dict = naming_conventions(function_names_tuple, test_names_tuple, functions_called_by_each_test_dict)
         naming_convention_contains_dict = naming_convention_contains(function_names_tuple, test_names_tuple, functions_called_by_each_test_dict)
         lcsb_dict = longest_common_subsequence_both(function_names_tuple, test_names_tuple, functions_called_by_each_test_dict, depths_of_functions_called_by_each_test_dict)
@@ -1149,26 +1138,26 @@
             for i in range(len(res_lists[0])):
                 s = 0
                 for j in range(len(res_lists)):
                     s += res_lists[j][i]
                 s /= len(res_lists)
                 final_res_dict[metric].append(s)
 
-        plt.figure(figsize=(10, 6))
+        plt.figure()
 
         # Use the 'seaborn' style
         plt.style.use('ggplot')
 
         # For each metric
         for metric in ["Precision", "Recall", "F1", "MAP"]:
             # Plot the metric values against the threshold values with increased line width
             plt.plot(thresholds, final_res_dict[metric], label=metric, linewidth=2)
 
         # Add a vertical line at threshold 0.5
-        plt.axvline(x=normal_threshold, color='black', linestyle='--', label=f't = {normal_threshold}')
+        plt.axvline(x=normal_threshold, color='black', linestyle='--', label=f't = {normal_threshold:.2f}')
         # Set the x-axis range to [0, 1]
         plt.xlim([0, 1])
         font = {
                 'weight': 'normal',
                 'size': 14,
                 'style': 'italic'}
         # Set the y-axis range to [0, 1]
@@ -1177,29 +1166,29 @@
         plt.yticks([0, 10, 20, 30, 40, 50, 60, 70, 80, 90, 100])
         # Add labels and title with increased font size
         plt.xlabel('Threshold', fontdict=font)
         plt.ylabel('Value',  fontdict=font)
         plt.title(title, fontsize=16)
 
         # Add a legend
-        plt.legend()
+        plt.legend(fontsize=14)
 
         # Add a grid
         plt.grid(True)
         plt.subplots_adjust(left=0.1, right=0.95, top=0.9, bottom=0.1)
         # Show the plot
         plt.show()
     
-    plot_threshold_sensitivity(lcsb_dicts, THRESHOLD_FOR_LCSB, "Threshold Sensitivity for LCS-B (Class Level)")
-    plot_threshold_sensitivity(lcsu_dicts, THRESHOLD_FOR_LCSU, "Threshold Sensitivity for LCS-U (Class Level)")
-    plot_threshold_sensitivity(levenshtein_dicts, THRESHOLD_FOR_LEVENSHTEIN, "Threshold Sensitivity for Levenshtein (Class Level)")
-    plot_threshold_sensitivity(tarantula_dicts, THRESHOLD_FOR_TARANTULA, "Threshold Sensitivity for Tarantula (Class Level)")
-    plot_threshold_sensitivity(tfidf_dicts, THRESHOLD_FOR_TFIDF, "Threshold Sensitivity for TF-IDF (Class Level)")
-    plot_threshold_sensitivity(tfidf_count_dicts, THRESHOLD_FOR_TFIDF_COUNT, "Threshold Sensitivity for TF-IDF* (Class Level)")
-    plot_threshold_sensitivity(average_dicts, THRESHOLD_FOR_AVERAGE, "Threshold Sensitivity for Combined (Class Level)")
+    plot_threshold_sensitivity(lcsb_dicts, THRESHOLD_FOR_LCSB, "LCS-B (Class Level)")
+    plot_threshold_sensitivity(lcsu_dicts, THRESHOLD_FOR_LCSU, "LCS-U (Class Level)")
+    plot_threshold_sensitivity(levenshtein_dicts, THRESHOLD_FOR_LEVENSHTEIN, "Levenshtein (Class Level)")
+    plot_threshold_sensitivity(tarantula_dicts, THRESHOLD_FOR_TARANTULA, "Tarantula (Class Level)")
+    plot_threshold_sensitivity(tfidf_dicts, THRESHOLD_FOR_TFIDF, "TF-IDF (Class Level)")
+    plot_threshold_sensitivity(tfidf_count_dicts, THRESHOLD_FOR_TFIDF_COUNT, "TF-IDF* (Class Level)")
+    plot_threshold_sensitivity(average_dicts, THRESHOLD_FOR_AVERAGE, "Combined (Class Level)")
 
 
 
 kedro_tracer_logs_path = "tracing-logs/kedro/kedro_pytest_tracer_logs.csv"
 kedro_ground_truth_path = "ground-truth-data/kedro/function/kedro_ground_truth.json"
 kedro_analysis_path = "analysis/kedro/function/kedro_predictions_results.csv"
 kedro_breakdown_path = "analysis/kedro/function/kedro_breakdown.json"
@@ -1262,14 +1251,14 @@
 
 if __name__ == "__main__":
     # analyse_trace(pyopenssl_tracer_logs_path, pyopenssl_ground_truth_path, pyopenssl_analysis_path, pyopenssl_breakdown_path, pyopenssl_copilot_function_prediction_path, pyopenssl_copilot_function_breakdown_path)
     # analyse_trace(arrow_tracer_logs_path, arrow_ground_truth_path, arrow_analysis_path, arrow_breakdown_path, arrow_copilot_function_prediction_path, arrow_copilot_function_breakdown_path)
     # analyse_trace(kedro_tracer_logs_path, kedro_ground_truth_path, kedro_analysis_path, kedro_breakdown_path, kedro_copilot_function_prediction_path, kedro_copilot_function_breakdown_path)
     # analyse_trace(chartify_tracer_logs_path, chartify_ground_truth_path, chartify_analysis_path, chartify_breakdown_path, chartify_copilot_function_prediction_path, chartify_copilot_function_breakdown_path)
     
-    analyse_trace_class_level(pyopenssl_tracer_logs_path, pyopenssl_ground_truth_class_path, pyopenssl_class_level_analysis_path, pyopenssl_class_level_breakdown_path, pyopenssl_ground_truth_function_class_path, pyopenssl_ground_truth_test_class_path, pyopenssl_copilot_class_prediction_path, pyopenssl_copilot_class_breakdown_path)
+    # analyse_trace_class_level(pyopenssl_tracer_logs_path, pyopenssl_ground_truth_class_path, pyopenssl_class_level_analysis_path, pyopenssl_class_level_breakdown_path, pyopenssl_ground_truth_function_class_path, pyopenssl_ground_truth_test_class_path, pyopenssl_copilot_class_prediction_path, pyopenssl_copilot_class_breakdown_path)
     # analyse_trace_class_level(arrow_tracer_logs_path, arrow_ground_truth_class_path, arrow_class_level_analysis_path, arrow_class_level_breakdown_path, arrow_ground_truth_function_class_path, arrow_ground_truth_test_class_path, arrow_copilot_class_prediction_path, arrow_copilot_class_breakdown_path)
     # analyse_trace_class_level(kedro_tracer_logs_path, kedro_ground_truth_class_path, kedro_class_level_analysis_path, kedro_class_level_breakdown_path, kedro_ground_truth_function_class_path, kedro_ground_truth_test_class_path, kedro_copilot_class_prediction_path, kedro_copilot_class_breakdown_path)
     # analyse_trace_class_level(chartify_tracer_logs_path, chartify_ground_truth_class_path, chartify_class_level_analysis_path, chartify_class_level_breakdown_path, chartify_ground_truth_function_class_path, chartify_ground_truth_test_class_path, chartify_copilot_class_prediction_path, chartify_copilot_class_breakdown_path)
 
-    # vary_threshold()
-    # vary_threshold_class()
+    vary_threshold()
+    vary_threshold_class()
```

### Comparing `pytctracer-0.1.9/pyproject.toml` & `pytctracer-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [project]
 authors = [
   {name = "Jason Ho"}
 ]
 description = """Research library demonstrating test-to-code traceability techniques on Python codebases that use the Pytest testing framework."""
 readme = "README.md"
 name = "pytctracer"
-version = "0.1.9"
+version = "0.2.0"
 classifiers=[
     "Natural Language :: English",
     "Intended Audience :: Science/Research",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 requires-python = ">=3.11"
 dependencies = [
   "matplotlib==3.8.3",
   "scikit-learn==1.4.1.post1",
   "click==8.1.7",
-  "pytest<=8.1.0"
+  "pytest<=8.1.0",
+  "python-dotenv==1.0.1"
 ]
 urls = { "Repository" = "https://github.com/jasonho2582001/comp0138-pytctracer" }
 
 [tool.setuptools.packages.find]
 where = ["."] 
 
 [build-system]
```

### Comparing `pytctracer-0.1.9/pytctracer/analyser.py` & `pytctracer-0.2.0/pytctracer/analyser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import List, Optional, Dict, Any, Tuple, Set
-from click import ClickException
 from pytctracer.config.constants import LevelType, TechniqueParameter
 from pytctracer.config import Config
 from pytctracer.io.input import read_trace_csv_log, load_link_json
 from pytctracer.io.output import (
     display_predicted_links,
     write_dict_to_json,
     write_evaluation_metrics_to_csv,
@@ -28,14 +27,18 @@
 )
 from pytctracer.evaluation.metrics import ArgNameToMetricMapper, Metric
 from pytctracer.evaluation import classify_predictions, evaluate_predictions
 from pytctracer.techniques import ArgNameToTechniqueMapper, Combined
 
 
 class Analyser:
+    """
+    Class which handles the the generation, evaluation and comparison
+    of test-to-code traceability links.
+    """
     def __init__(self) -> None:
         self.arg_name_to_technique_map = ArgNameToTechniqueMapper()
         self.arg_name_to_metric_map = ArgNameToMetricMapper()
         self.default_technique_names = Config.DEFAULT_CHOSEN_TECHNIQUE_NAMES
         self.default_metric_names = Config.DEFAULT_CHOSEN_METRIC_NAMES
 
     def compare_traceability_links(
@@ -95,15 +98,15 @@
         self,
         predicted_links: Dict[str, List[str]],
         ground_truth_links: Dict[str, List[str]],
     ) -> None:
         tests_in_predicted_links = set(predicted_links.keys())
         for test in ground_truth_links:
             if test not in tests_in_predicted_links:
-                raise ClickException(
+                raise ValueError(
                     f"Test '{test}' in ground truth but not in predicted links"
                 )
 
     def evaluate_traceability_links_for_trace(
         self,
         trace_csv_log_path: str,
         ground_truth_path: str,
@@ -201,16 +204,15 @@
         traceability_level: LevelType,
     ) -> None:
         for (
             technique_arg_name,
             classifications,
         ) in classifications_for_techniques.items():
             technique_arg_name = technique_arg_name.replace("-", "_")
-            file_path = f"{classifications_output_directory_path}/
-            {technique_arg_name}_{traceability_level.lower()}_classifications.json"
+            file_path = f"""{classifications_output_directory_path}/{technique_arg_name}_{traceability_level.lower()}_classifications.json"""
             write_dict_to_json(classifications, file_path)
 
     def _display_classifications_for_techniques(
         self, classifications_for_techniques: Dict[str, Dict[str, List[str]]]
     ) -> None:
         for (
             technique_arg_name,
@@ -328,16 +330,15 @@
         traceability_level: LevelType,
     ) -> None:
         for (
             technique_arg_name,
             link_predictions,
         ) in link_predictions_for_techniques.items():
             technique_arg_name = technique_arg_name.replace("-", "_")
-            file_path = f"{prediction_output_directory_path}/
-            {technique_arg_name}_{traceability_level.lower()}_predicted_links.json"
+            file_path = f"""{prediction_output_directory_path}/{technique_arg_name}_{traceability_level.lower()}_predicted_links.json"""
             write_dict_to_json(link_predictions, file_path)
 
     def _display_predicted_links_for_techniques(
         self, link_predictions_for_techniques: Dict[str, Dict[str, List[str]]]
     ) -> None:
         for (
             technique_arg_name,
```

### Comparing `pytctracer-0.1.9/pytctracer/cli.py` & `pytctracer-0.2.0/pytctracer/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,23 +58,26 @@
 def produce_links(
     trace_csv_log_path: str,
     technique: Optional[Tuple[str]],
     level: str,
     add_combined: bool,
     output_directory: Optional[str],
 ):
-    analyser = Analyser()
-    chosen_technique_names = list(technique)
-    analyser.produce_traceability_links_for_trace(
-        trace_csv_log_path=trace_csv_log_path,
-        traceability_level=level,
-        add_combined_technique=add_combined,
-        chosen_technique_names=chosen_technique_names,
-        prediction_output_directory_path=output_directory,
-    )
+    try:
+        analyser = Analyser()
+        chosen_technique_names = list(technique)
+        analyser.produce_traceability_links_for_trace(
+            trace_csv_log_path=trace_csv_log_path,
+            traceability_level=level,
+            add_combined_technique=add_combined,
+            chosen_technique_names=chosen_technique_names,
+            prediction_output_directory_path=output_directory,
+        )
+    except Exception as e:
+        click.ClickException(str(e))
 
 
 @cli.command(
     "evaluate-links",
     short_help="Produce and evaluate links against a ground truth.",
     help="""Produce and evaluate test-to-code traceability links against
     ground truth links for a given trace log CSV file, 
@@ -136,42 +139,47 @@
     "--classifications-output-directory",
     type=click.Path(exists=True),
     help="""Directory to write the output classifications to. 
               Each technique's classifications will be written to a separate JSON file.""",
 )
 @click.option(
     "--metrics-output-path",
-    type=click.Path(exists=True),
+    type=click.Path(exists=False),
     help="""Path to write the CSV containing the evaluation metric results to.""",
 )
 def evaluate_links(
     trace_csv_log_path: str,
     ground_truth_path: str,
     technique: Optional[Tuple[str]],
     metric: Optional[Tuple[str]],
     level: str,
     add_combined: bool,
     as_percentage: bool,
     classifications_output_directory: Optional[str],
+    display_classifications: bool,
     metrics_output_path: Optional[str],
 ):
-    analyser = Analyser()
-    chosen_technique_names = list(technique)
-    chosen_metric_names = list(metric)
-    analyser.evaluate_traceability_links_for_trace(
-        trace_csv_log_path=trace_csv_log_path,
-        ground_truth_path=ground_truth_path,
-        traceability_level=level,
-        add_combined_technique=add_combined,
-        metric_as_percentage=as_percentage,
-        chosen_technique_names=chosen_technique_names,
-        chosen_metric_names=chosen_metric_names,
-        classifications_output_directory_path=classifications_output_directory,
-        evaluation_metrics_output_path=metrics_output_path,
-    )
+    try:
+        analyser = Analyser()
+        chosen_technique_names = list(technique)
+        chosen_metric_names = list(metric)
+        analyser.evaluate_traceability_links_for_trace(
+            trace_csv_log_path=trace_csv_log_path,
+            ground_truth_path=ground_truth_path,
+            traceability_level=level,
+            add_combined_technique=add_combined,
+            metric_as_percentage=as_percentage,
+            chosen_technique_names=chosen_technique_names,
+            chosen_metric_names=chosen_metric_names,
+            classifications_output_directory_path=classifications_output_directory,
+            display_classifications_to_stdout=display_classifications,
+            evaluation_metrics_output_path=metrics_output_path,
+        )
+    except Exception as e:
+        click.ClickException(str(e))
 
 
 @cli.command(
     "compare-links",
     short_help="Compare a set of links against a ground truth.",
     help="""Compare a set of test-to-code traceability links against ground truth links
     using specified evaluation metrics.
@@ -185,66 +193,54 @@
     show for each test artefact, which code artefacts were classified as true positives,
     false positives, and false negatives. The evaluation metrics will be reported for
     each set of links, and is saveable to a CSV file.""",
 )
 @click.argument("predicted-links-path", type=click.Path(exists=True))
 @click.argument("ground-truth-path", type=click.Path(exists=True))
 @click.option(
-    "--metric", type=click.Choice(Config.SELECTABLE_METRIC_NAMES), multiple=True,
+    "--metric",
+    type=click.Choice(Config.SELECTABLE_METRIC_NAMES),
+    multiple=True,
     help="""Use a specified evaluation metric (can be multiple of this flag). If omitted,
     all selectable metrics are used by default.""",
 )
 @click.option(
-    "--level",
-    type=click.Choice([LevelType.FUNCTION, LevelType.CLASS]),
-    default=LevelType.FUNCTION,
-    help="""What level of traceability to produce links for (function or class).
-    If omitted, links are produced at the function level by default.""",
-)
-@click.option(
     "--as-percentage",
     is_flag=True,
     default=False,
     help="""Report continous metrics as percentages. If omitted,
               metrics are reported as raw values by default.""",
 )
 @click.option(
     "--classifications-output-path",
     type=click.Path(exists=True),
     help="""Path to write the JSON containing the classifications to.""",
 )
 @click.option(
     "--metrics-output-path",
-    type=click.Path(exists=True),
+    type=click.Path(exists=False),
     help="""Path to write the CSV containing the evaluation metric results to.""",
 )
 def compare_links(
     predicted_links_path: str,
     ground_truth_path: str,
     metric: Optional[Tuple[str]],
-    level: str,
     as_percentage: bool,
     classifications_output_path: Optional[str],
     metrics_output_path: Optional[str],
 ):
-    analyser = Analyser()
-    chosen_metric_names = list(metric)
-    analyser.compare_traceability_links(
-        predicted_links_path=predicted_links_path,
-        ground_truth_path=ground_truth_path,
-        chosen_metric_names=chosen_metric_names,
-        metric_as_percentage=as_percentage,
-        classifications_output_path=classifications_output_path,
-        evaluation_metrics_output_path=metrics_output_path,
-    )
-    # predicted_links_path="copilot-predictions/pyopenssl/function/pyopenssl_copilot_function_predictions.json",
-    # ground_truth_path="ground-truth-data/pyopenssl/function/pyopenssl_ground_truth.json",
-
-
-# tracing-logs/pyopenssl/pyopenssl_pytest_tracer_logs.csv
-
-# trace_csv_log_path="tracing-logs/pyopenssl/pyopenssl_pytest_tracer_logs.csv",
-# ground_truth_path="ground-truth-data/pyopenssl/class/pyopenssl_ground_truth_classes.json",
-
+    try:
+        analyser = Analyser()
+        chosen_metric_names = list(metric)
+        analyser.compare_traceability_links(
+            predicted_links_path=predicted_links_path,
+            ground_truth_path=ground_truth_path,
+            chosen_metric_names=chosen_metric_names,
+            metric_as_percentage=as_percentage,
+            classifications_output_path=classifications_output_path,
+            evaluation_metrics_output_path=metrics_output_path,
+        )
+    except Exception as e:
+        click.ClickException(str(e))
 
 if __name__ == "__main__":
     cli()
```

### Comparing `pytctracer-0.1.9/pytctracer/config/config.py` & `pytctracer-0.2.0/pytctracer/config/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 class Config:
+    """
+    Class storing configuration variables for the package.
+    """
     SELECTABLE_TECHNIQUE_NAMES = [
         "nc",
         "ncc",
         "lcsb",
         "lcsu",
         "leven",
         "lcba",
@@ -38,10 +41,18 @@
         "map",
         "auc",
         "tp",
         "fp",
         "fn",
     ]
     EVALUATION_METRICS_TITLE = "Evaluation Metrics"
-
+    DEFAULT_THRESHOLDS = {
+        "lcsu": 0.75,
+        "lcsb": 0.55,
+        "leven": 0.95,
+        "tarantula": 0.95,
+        "tfidf": 0.9,
+        "tfidf_multiset": 0.9,
+        "combined": 0.85,
+    }
 
 __all__ = ["Config"]
```

### Comparing `pytctracer-0.1.9/pytctracer/config/constants/__init__.py` & `pytctracer-0.2.0/pytctracer/config/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.9/pytctracer/config/constants/technique_parameter.py` & `pytctracer-0.2.0/pytctracer/config/constants/technique_parameter.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.9/pytctracer/config/constants/trace_data_header.py` & `pytctracer-0.2.0/pytctracer/config/constants/trace_data_header.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.9/pytctracer/evaluation/metrics/__init__.py` & `pytctracer-0.2.0/pytctracer/evaluation/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.9/pytctracer/evaluation/metrics/area_under_curve.py` & `pytctracer-0.2.0/pytctracer/evaluation/metrics/area_under_curve.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.9/pytctracer/evaluation/metrics/arg_name_to_metric_mapper.py` & `pytctracer-0.2.0/pytctracer/evaluation/metrics/arg_name_to_metric_mapper.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.9/pytctracer/evaluation/metrics/f1.py` & `pytctracer-0.2.0/pytctracer/evaluation/metrics/f1.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.9/pytctracer/evaluation/metrics/false_negatives.py` & `pytctracer-0.2.0/pytctracer/evaluation/metrics/false_negatives.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.9/pytctracer/evaluation/metrics/false_positives.py` & `pytctracer-0.2.0/pytctracer/evaluation/metrics/false_positives.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.9/pytctracer/evaluation/metrics/mean_average_precision.py` & `pytctracer-0.2.0/pytctracer/evaluation/metrics/mean_average_precision.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.9/pytctracer/evaluation/metrics/metric.py` & `pytctracer-0.2.0/pytctracer/evaluation/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.9/pytctracer/evaluation/metrics/precision.py` & `pytctracer-0.2.0/pytctracer/evaluation/metrics/precision.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.9/pytctracer/evaluation/metrics/recall.py` & `pytctracer-0.2.0/pytctracer/evaluation/metrics/recall.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.9/pytctracer/evaluation/metrics/true_positives.py` & `pytctracer-0.2.0/pytctracer/evaluation/metrics/true_positives.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.9/pytctracer/parsing/__init__.py` & `pytctracer-0.2.0/pytctracer/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.9/pytctracer/techniques/__init__.py` & `pytctracer-0.2.0/pytctracer/techniques/__init__.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.9/pytctracer/techniques/arg_name_to_technique_mapper.py` & `pytctracer-0.2.0/pytctracer/techniques/arg_name_to_technique_mapper.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 from .tarantula import Tarantula
 from .tfidf import TFIDF, TFIDFMultiset
 from .technique import Technique
 from .combined import Combined
 
 
 class ArgNameToTechniqueMapper:
+    """
+    Class providing mappings between the argument name of each technique to 
+    some relevant properties, including the technique's class, full name and
+    short name.
+    """
     def __init__(self):
         self._arg_name_to_technique = {
             LevenshteinDistance.arg_name: LevenshteinDistance,
             NamingConventions.arg_name: NamingConventions,
             NamingConventionsContains.arg_name: NamingConventionsContains,
             LastCallBeforeAssert.arg_name: LastCallBeforeAssert,
             LongestCommonSubsequenceBoth.arg_name: LongestCommonSubsequenceBoth,
@@ -49,17 +54,32 @@
             TFIDF.arg_name: TFIDF.short_name,
             TFIDFMultiset.arg_name: TFIDFMultiset.short_name,
             Combined.arg_name: Combined.short_name,
         }
         self._arg_names = list(self._arg_name_to_technique.keys())
 
     def get_arg_names(self) -> List[str]:
+        """
+        Return the list of valid technique argument names.
+        
+        Returns:
+            List[str]: List of valid technique argument names.
+        """
         return self._arg_names
 
     def get_technique(self, arg_name: str) -> Technique:
+        """
+        Get the technique class for the given argument name.
+
+        Args:
+            arg_name (str): The argument name of the technique.
+
+        Returns:
+            Technique: The technique class.
+        """
         if arg_name not in self._arg_name_to_technique:
             raise ValueError(
                 f"Invalid technique arg name: {arg_name} for retrieving technique class."
             )
 
         return self._arg_name_to_technique[arg_name]
```

### Comparing `pytctracer-0.1.9/pytctracer/techniques/last_call_before_assert.py` & `pytctracer-0.2.0/pytctracer/techniques/last_call_before_assert.py`

 * *Files identical despite different names*

### Comparing `pytctracer-0.1.9/pytctracer/techniques/levenshtein_distance.py` & `pytctracer-0.2.0/pytctracer/techniques/levenshtein_distance.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,20 @@
             is the short name of the test or test class.
 
             functions_called_by_tests (Dict[str, Set[str]]): A dictionary
             where the keys are the fully qualified names of the test or test
             classes, and the values are sets containing the fully qualified
             names of each function or function class invoked.
 
+            functions_called_by_test_depth (Dict[str, Dict[str, int]]): A
+            dictionary where the keys are the fully qualified names of the test
+            or test classes, and the values are dictionaries containing the
+            fully qualified names of each function or function class invoked,
+            along with the call depth of each function or function class.
+
         Returns:
             Dict[str, Dict[str, Union[int, float]]]: A dictionary where the
             keys are the fully qualified names of the test or test classes,
             and the values are dictionaries containing the traceability scores
             for each function or function class.
         """
         levenshtein_scores = defaultdict(dict)
```

### Comparing `pytctracer-0.1.9/pytctracer/techniques/longest_common_subsequence.py` & `pytctracer-0.2.0/pytctracer/techniques/longest_common_subsequence.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,20 @@
             is the short name of the test or test class.
 
             functions_called_by_tests (Dict[str, Set[str]]): A dictionary
             where the keys are the fully qualified names of the test or test
             classes, and the values are sets containing the fully qualified
             names of each function or function class invoked.
 
+            functions_called_by_test_depth (Dict[str, Dict[str, int]]): A dictionary
+            where the keys are the fully qualified names of the test or test
+            classes, and the values are dictionaries containing the fully qualified
+            names of each function or function class invoked and the depth of the
+            call.
+
         Returns:
             Dict[str, Dict[str, Union[int, float]]]: A dictionary where the
             keys are the fully qualified names of the test or test classes,
             and the values are dictionaries containing the traceability scores
             for each function or function class.
         """
         return self._run(
@@ -92,16 +98,15 @@
             lcs_scores = self._normalise_dict(lcs_scores)
 
         return lcs_scores
 
     @abstractmethod
     def _compute_lcs_score(self, _function_name: str, _test_name: str) -> int:
         raise NotImplementedError(
-            """LCS classes must implement this method 
-                                  to compute the traceability score"""
+            """LCS classes must implement this method to compute the traceability score"""
         )
 
     def _compute_lcs(self, function_name: str, test_name: str) -> int:
         m = len(function_name)
         n = len(test_name)
         lcs_matrix = [[0 for _ in range(n + 1)] for _ in range(m + 1)]
         for i in range(1, m + 1):
@@ -149,14 +154,20 @@
             is the short name of the test or test class.
 
             functions_called_by_tests (Dict[str, Set[str]]): A dictionary
             where the keys are the fully qualified names of the test or test
             classes, and the values are sets containing the fully qualified
             names of each function or function class invoked.
 
+            functions_called_by_test_depth (Dict[str, Dict[str, int]]): A dictionary
+            where the keys are the fully qualified names of the test or test
+            classes, and the values are dictionaries containing the fully qualified
+            names of each function or function class invoked and the depth of the
+            call.
+
         Returns:
             Dict[str, Dict[str, Union[int, float]]]: A dictionary where the
             keys are the fully qualified names of the test or test classes,
             and the values are dictionaries containing the traceability scores
             for each function or function class.
         """
         return self._run(
@@ -211,14 +222,20 @@
             is the short name of the test or test class.
 
             functions_called_by_tests (Dict[str, Set[str]]): A dictionary
             where the keys are the fully qualified names of the test or test
             classes, and the values are sets containing the fully qualified
             names of each function or function class invoked.
 
+            functions_called_by_test_depth (Dict[str, Dict[str, int]]): A dictionary
+            where the keys are the fully qualified names of the test or test
+            classes, and the values are dictionaries containing the fully qualified
+            names of each function or function class invoked and the depth of the
+            call.
+
         Returns:
             Dict[str, Dict[str, Union[int, float]]]: A dictionary where the
             keys are the fully qualified names of the test or test classes,
             and the values are dictionaries containing the traceability scores
             for each function or function class.
         """
         return self._run(
```

### Comparing `pytctracer-0.1.9/pytctracer/techniques/naming_conventions.py` & `pytctracer-0.2.0/pytctracer/techniques/naming_conventions.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         stripped_test_name = self._strip_test_name(test_name)
 
         return 1 if function_name == stripped_test_name else 0
 
 
 class NamingConventionsContains(NamingConventions):
     """
-    Class implementing the Naming Conventions traceability technique.
+    Class implementing the Naming Conventions - Contains traceability technique.
     """
 
     full_name = "Naming Conventions - Contains"
     short_name = "NCC"
     description = "TBC"
     arg_name = "ncc"
     required_parameters = {
```

### Comparing `pytctracer-0.1.9/pytctracer/techniques/tarantula.py` & `pytctracer-0.2.0/pytctracer/techniques/tarantula.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,15 +54,21 @@
             test classes, and the values are sets containing the fully
             qualified names of each function or function class that the
             test invokes.
 
             tests_that_call_functions (Dict[str, Set[str]]): A dictionary
             where the keys are the fully qualified names of the function or
             function classes, and the values are sets containing each
-            test or test class that calls the function or function class
+            test or test class that calls the function or function class.
+
+            functions_called_by_test_depth (Dict[str, Dict[str, int]]): A
+            dictionary where the keys are the fully qualified names of the
+            test or test classes, and the values are dictionaries containing
+            the fully qualified names of each function or function class
+            that the test invokes, and the depth of the call.
 
         Returns:
             Dict[str, Dict[str, Union[int, float]]]: A dictionary where the
             keys are the fully qualified names of the test or test classes,
             and the values are dictionaries containing the traceability scores
             for each function or function class.
         """
```

### Comparing `pytctracer-0.1.9/pytctracer/techniques/tfidf.py` & `pytctracer-0.2.0/pytctracer/techniques/tfidf.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,20 +46,32 @@
             element is the short name of the function or function class.
 
             test_names_tuple (List[Tuple[str, str]]): A list of tuples,
             where the first element of each tuple is the fully qualified
             (full path) name of a test or test class, and the second element
             is the short name of the test or test class.
 
+            functions_called_by_tests (Dict[str, Set[str]]): A dictionary where
+            the keys are the fully qualified names of the test or test classes,
+            and the values are sets containing the fully qualified names of each
+            function or function class called by the test or test class.
+
             tests_that_call_functions (Dict[str, Set[str]]): A dictionary
             where the keys are the fully qualified names of the function or
             function classes, and the values are sets containing the fully
             qualified names of each test or test class that invokes the
             function or function class.
 
+            functions_called_by_test_depth (Dict[str, Dict[str, int]]): A
+            dictionary where the keys are the fully qualified names of the test
+            or test classes, and the values are dictionaries containing the
+            fully qualified names of each function or function class called by
+            the test or test class and the call depth of the function or function
+            class.
+
         Returns:
             Dict[str, Dict[str, Union[int, float]]]: A dictionary where the
             keys are the fully qualified names of the test or test classes,
             and the values are dictionaries containing the traceability scores
             for each function or function class.
         """
         tfidf_scores = defaultdict(dict)
@@ -158,15 +170,15 @@
         function_names_tuple: List[Tuple[str, str]],
         test_names_tuple: List[Tuple[str, str]],
         functions_called_by_test_count: Dict[str, Dict[str, int]],
         tests_that_call_functions: Dict[str, Set[str]],
         functions_called_by_test_depth: Dict[str, Dict[str, int]],
     ) -> Dict[str, Dict[str, Union[int, float]]]:
         """
-        Invokes the TF-IDF traceability technique
+        Invokes the TF-IDF* (multiset) traceability technique
         to produce traceability scores for each test-to-code pair given.
 
         Args:
             function_names_tuple (List[Tuple[str, str]]): A list of tuples,
             where the first element of each tuple is the fully qualified
             (full path) name of a function or function class, and the second
             element is the short name of the function or function class.
@@ -181,16 +193,22 @@
             function classes, and the values are dictionaries containing each
             function or function class called by the test or test class and the
             number of times it was called.
 
             tests_that_call_functions (Dict[str, Set[str]]): A dictionary
             where the keys are the fully qualified names of the function or
             function classes, and the values are sets containing each
-            test or test class that calls the function or function class
+            test or test class that calls the function or function class.
 
+            functions_called_by_test_depth (Dict[str, Dict[str, int]]): A
+            dictionary where the keys are the fully qualified names of the test
+            or test classes, and the values are dictionaries containing the
+            fully qualified names of each function or function class called by
+            the test or test class and the call depth of the function or function
+            class.
 
         Returns:
             Dict[str, Dict[str, Union[int, float]]]: A dictionary where the
             keys are the fully qualified names of the test or test classes,
             and the values are dictionaries containing the traceability scores
             for each function or function class.
         """
```

### Comparing `pytctracer-0.1.9/pytctracer/tracer.py` & `pytctracer-0.2.0/pytctracer/tracer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from types import FrameType, CodeType
-from typing import List, Optional, Any, Tuple
+from typing import Callable, List, Optional, Any, Tuple
 import os
 import inspect
 import pytest
 import csv
 import threading
 import dis
 from pytctracer.config.constants import (
@@ -21,21 +21,38 @@
 TEST_PREFIX = "test"
 TEST_CLASS_PREFIX = "Test"
 LOCALS = "<locals>"
 MODULE = "<module>"
 
 
 class PytestTracer:
+    """
+    Class which allows for the tracing of a Pytest test suite invocation,
+    capturing and storing dynamic information, and writing of the information
+    to a CSV format.
+    """
     def __init__(
         self,
         project_root: str,
         test_folders: List[str],
         source_folders: List[str],
         output_csv_file_name: str,
     ) -> None:
+        """
+        Class which allows for the tracing of a Pytest test suite invocation,
+        capturing and storing dynamic information, and writing of the information
+        to a CSV format.
+
+        Args:
+            project_root (str): The root directory of the project.
+            test_folders (List[str]): A list of directories containing test files.
+            source_folders (List[str]): A list of directories containing source files.
+            output_csv_file_name (str): The name of the output CSV file.
+        """
+
         project_root = os.path.normcase(project_root)
         self._project_root = os.path.normcase(os.path.abspath(project_root))
         self._test_folders = [
             os.path.normcase(os.path.join(self._project_root, test_folder))
             for test_folder in test_folders
         ]
         self._source_folders = [
@@ -53,15 +70,27 @@
         self._line_of_last_assert = None
         self._csv_data = []
         self._in_line_functions_left_list = []
         self._assert_line_values = []
         self._handle_in_line_functions = False
         self._in_line_function_calls = 0
 
-    def trace(self, frame: FrameType, event, arg=None):
+    def trace(self, frame: FrameType, event: str, arg: Optional[Any]=None) -> Callable:
+        """
+        Trace function to be used by `sys.settrace` to capture the tracing of Python code
+        during a Pytest test suite invocation.
+
+        Args:
+            frame (FrameType): The current frame.
+            event (str): The event type.
+            arg (Optional[Any]): The argument associated with the event.
+        
+        Returns:
+            Callable: The trace function.
+        """
         if not self.our_frame(frame):
             code_of_current_frame = frame.f_code
             file_name = os.path.normcase(code_of_current_frame.co_filename)
             function_name = code_of_current_frame.co_name
             qualified_function_name = code_of_current_frame.co_qualname
             current_thread_id = threading.current_thread().ident
             line_number = frame.f_lineno
@@ -75,25 +104,22 @@
 
             # Only trace after if the function is one of unittest, test or source
             if function_type and MODULE not in qualified_function_name:
                 qualified_class_name, class_name = self._get_class_names(
                     code_qualified_name=qualified_function_name,
                     function_name=function_name,
                     file_name=file_name,
-                    function_type=function_type,
                 )
                 fully_qualified_function_name = self._get_fully_qualified_name(
                     file_name=file_name,
                     code_qualified_name=qualified_function_name,
-                    function_type=function_type,
                 )
                 fully_qualified_class_name = self._get_fully_qualified_name(
                     file_name=file_name,
                     code_qualified_name=qualified_class_name,
-                    function_type=function_type,
                 )
                 if (
                     event == SetTraceEventType.LINE
                     and function_type == FunctionType.ASSERT
                 ):
                     if self._check_in_line_functions_in_assert():
                         self._save_assert_line_values(
@@ -153,24 +179,22 @@
 
                     self._current_depth += 1
 
                 elif event == SetTraceEventType.RETURN:
                     # Keep track of the last function that was last returned
                     self._current_depth -= 1
                     self._function_stack.pop()
-                    # print(f"{'  ' * (self._current_depth)}< {self._current_depth}: Function '{fully_qualified_function_name}()' returned at line {line_number} with value: '{arg}' of type {type(arg)}")
+                    
                     if (
                         function_type.startswith(TEST_PREFIX.upper())
                         or function_type == FunctionType.ASSERT
                     ):
                         self._test_function_stack.pop()
-                        # if len(self._test_function_stack) == 0:
-                        #     print(f"=== EXITING TEST FUNCTION '{fully_qualified_function_name}\n")
+
                     if function_type == FunctionType.ASSERT:
-                        # If an assert happens to be on the last line, it may get caught as a return event, so we add a duplicate entry to account for assert line and return
                         self._add_csv_row_data(
                             depth=self._current_depth + 1,
                             function_type=function_type,
                             function_name=function_name,
                             fully_qualified_function_name=fully_qualified_function_name,
                             class_name=class_name,
                             fully_qualified_class_name=fully_qualified_class_name,
@@ -202,15 +226,15 @@
                         testing_method=testing_method,
                         thread_id=current_thread_id,
                     )
                     self._check_remaining_in_line_functions(self._current_depth)
 
                 elif event == SetTraceEventType.EXCEPTION:
                     exc_type, exc_value, exc_traceback = arg
-                    # print(f"{'  ' * (self._current_depth - 1)}- {self._current_depth}: Function '{fully_qualified_function_name}()' at line {line_number} has raised an Exception, with exception type: {exc_type} and message: '{str(exc_value)}'")
+            
                     self._add_csv_row_data(
                         depth=self._current_depth,
                         function_type=function_type,
                         function_name=function_name,
                         fully_qualified_function_name=fully_qualified_function_name,
                         class_name=class_name,
                         fully_qualified_class_name=fully_qualified_class_name,
@@ -219,53 +243,69 @@
                         exception_type=exc_type,
                         exception_message=str(exc_value),
                     )
 
         return self.trace
 
     def trace_in_built(self, _frame: FrameType, event, _arg=None):
-        # Handle in-line function returns that don't get captured by sys.settrace, for assert checking
-        # For example, isinstance within an assert statement
-        # These built in functions won't be caught by the sys.settrace function, so we need to check
-        # for them here.
+        """
+        Handle in-line function returns that don't get captured by sys.settrace, for assert checking
+        For example, `isinstance` within an assert statement
+        These built in functions won't be caught by the sys.settrace function, so we need to check
+        for them here.
+        """
         if event == SetProfileCEventType.C_CALL:
             self._current_depth += 1
         if (
             event == SetProfileCEventType.C_RETURN
             or event == SetProfileCEventType.C_EXCEPTION
         ):
             self._current_depth -= 1
             self._check_remaining_in_line_functions(self._current_depth)
 
     def write_to_csv(self) -> None:
+        """
+        Write stored trace data to a CSV file. The CSV is written to
+        the file specified in the `output_csv_file_name` parameter the
+        class was initialised with.
+        """
         with open(self._csv_name, "w", newline="") as csv_file:
             csv_writer = csv.DictWriter(csv_file, fieldnames=self._csv_headers)
             csv_writer.writeheader()
             for data_row in self._csv_data:
                 csv_writer.writerow(data_row)
 
     def our_frame(self, frame: FrameType) -> bool:
-        """Return true if `frame` is in the current (inspecting) class."""
+        """
+        Checks whether the current code being traced is the PytestTracer class itself.
+        
+        Args:
+            frame (FrameType): The current frame.
+        
+        Returns:
+            bool: True if the current code being traced is the PytestTracer class itself,
+            False otherwise.
+        """
         return frame.f_code.co_qualname == TRACE_QUALIFIED_NAME
 
     def _add_csv_row_data(
         self,
         depth: int,
         function_type: str,
         function_name: str,
         fully_qualified_function_name: str,
         class_name: str,
         fully_qualified_class_name: str,
         line_number: int,
         event_type: str,
         return_value: Optional[Any] = "",
-        return_type: Optional[str] = "",
-        exception_type: Optional[str] = "",
-        exception_message: Optional[str] = "",
-        testing_method: Optional[str] = "",
+        return_type: str = "",
+        exception_type: str = "",
+        exception_message: str = "",
+        testing_method: str = "",
         thread_id: Optional[int] = None,
     ):
         data = {
             TraceDataHeader.DEPTH: depth,
             TraceDataHeader.FUNCTION_TYPE: function_type,
             TraceDataHeader.TESTNG_METHOD: testing_method,
             TraceDataHeader.FUNCTION_NAME: function_name,
@@ -283,52 +323,52 @@
         self._csv_data.append(data)
 
     def _get_class_names(
         self,
         code_qualified_name: str,
         function_name: str,
         file_name: str,
-        function_type: str,
     ) -> Tuple[str, str]:
         if code_qualified_name != function_name and not code_qualified_name.startswith(
             LOCALS
         ):
             class_name_list = code_qualified_name.split(".")
 
             # Remove last element, which should be the function name
             class_name_list.pop()
 
-            # Check current last element is not <locals>. If it is, we need to remove it, and the previous element
+            # Check current last element is not <locals>. If it is, we need to remove it, 
+            # and the previous element.
             # This represents an inner function, so we need to remove it as well to get the actual class
             while class_name_list and class_name_list[-1] == LOCALS:
                 class_name_list.pop()
                 class_name_list.pop()
 
             if class_name_list:
                 return ".".join(class_name_list), class_name_list[-1]
 
-        module_name = self._get_module_name(file_name, function_type)
+        module_name = self._get_module_name(file_name)
 
         return "", module_name.split(".")[-1]
 
-    def _get_module_name(self, file_name: str, function_type: str) -> str:
+    def _get_module_name(self, file_name: str) -> str:
         relative_file_path = os.path.relpath(file_name, self._project_root)
         relative_file_path = relative_file_path.replace(os.path.sep, "/")
 
         # remove file extension
         module_path, _ = os.path.splitext(relative_file_path)
 
         module_name = module_path.replace("/", ".")
 
         return module_name
 
     def _get_fully_qualified_name(
-        self, file_name: str, code_qualified_name: str, function_type: str
+        self, file_name: str, code_qualified_name: str
     ) -> str:
-        module_name = self._get_module_name(file_name, function_type)
+        module_name = self._get_module_name(file_name)
 
         return (
             (module_name + "." + code_qualified_name)
             if code_qualified_name
             else module_name
         )
```

### Comparing `pytctracer-0.1.9/pytctracer.egg-info/SOURCES.txt` & `pytctracer-0.2.0/pytctracer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

