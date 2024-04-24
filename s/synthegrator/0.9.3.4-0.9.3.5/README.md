# Comparing `tmp/synthegrator-0.9.3.4.tar.gz` & `tmp/synthegrator-0.9.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthegrator-0.9.3.4.tar", last modified: Wed Apr 24 19:05:10 2024, max compression
+gzip compressed data, was "synthegrator-0.9.3.5.tar", last modified: Wed Apr 24 19:57:10 2024, max compression
```

## Comparing `synthegrator-0.9.3.4.tar` & `synthegrator-0.9.3.5.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:05:10.574287 synthegrator-0.9.3.4/
--rw-r--r--   0 dgros      (501) staff       (20)     1074 2024-01-31 01:30:32.000000 synthegrator-0.9.3.4/LICENSE
--rw-r--r--   0 dgros      (501) staff       (20)     4657 2024-04-24 19:05:10.574082 synthegrator-0.9.3.4/PKG-INFO
--rw-r--r--   0 dgros      (501) staff       (20)     2344 2024-02-07 16:58:12.000000 synthegrator-0.9.3.4/README.md
--rw-r--r--   0 dgros      (501) staff       (20)     5031 2024-04-24 18:50:48.000000 synthegrator-0.9.3.4/pyproject.toml
--rw-r--r--   0 dgros      (501) staff       (20)       38 2024-04-24 19:05:10.574327 synthegrator-0.9.3.4/setup.cfg
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:05:10.555792 synthegrator-0.9.3.4/synthegrator/
--rw-r--r--   0 dgros      (501) staff       (20)        0 2023-06-07 15:22:13.000000 synthegrator-0.9.3.4/synthegrator/__init__.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:05:10.556824 synthegrator-0.9.3.4/synthegrator/_vendor/
--rw-r--r--   0 dgros      (501) staff       (20)        0 2024-04-24 02:44:40.000000 synthegrator-0.9.3.4/synthegrator/_vendor/__init__.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:05:10.557834 synthegrator-0.9.3.4/synthegrator/_vendor/epicbox/
--rw-r--r--   0 dgros      (501) staff       (20)       70 2024-04-24 02:48:53.000000 synthegrator-0.9.3.4/synthegrator/_vendor/epicbox/__init__.py
--rw-r--r--   0 dgros      (501) staff       (20)     2235 2024-04-24 02:48:53.000000 synthegrator-0.9.3.4/synthegrator/_vendor/epicbox/config.py
--rw-r--r--   0 dgros      (501) staff       (20)      195 2024-04-24 02:48:53.000000 synthegrator-0.9.3.4/synthegrator/_vendor/epicbox/exceptions.py
--rw-r--r--   0 dgros      (501) staff       (20)    13035 2024-04-24 02:48:53.000000 synthegrator-0.9.3.4/synthegrator/_vendor/epicbox/sandboxes.py
--rw-r--r--   0 dgros      (501) staff       (20)    10163 2024-04-24 02:48:53.000000 synthegrator-0.9.3.4/synthegrator/_vendor/epicbox/utils.py
--rw-r--r--   0 dgros      (501) staff       (20)    13611 2024-03-17 08:36:57.000000 synthegrator-0.9.3.4/synthegrator/code_problem_builders.py
--rw-r--r--   0 dgros      (501) staff       (20)    14744 2024-03-19 03:36:50.000000 synthegrator-0.9.3.4/synthegrator/code_problems.py
--rw-r--r--   0 dgros      (501) staff       (20)    10006 2024-03-20 20:00:19.000000 synthegrator-0.9.3.4/synthegrator/code_solver.py
--rw-r--r--   0 dgros      (501) staff       (20)     3756 2024-03-16 23:08:47.000000 synthegrator-0.9.3.4/synthegrator/df_converters.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:05:10.558004 synthegrator-0.9.3.4/synthegrator/dypybench/
--rw-r--r--   0 dgros      (501) staff       (20)        0 2023-08-10 05:46:51.000000 synthegrator-0.9.3.4/synthegrator/dypybench/__init__.py
--rw-r--r--   0 dgros      (501) staff       (20)      385 2023-09-07 07:28:11.000000 synthegrator-0.9.3.4/synthegrator/environments.py
--rw-r--r--   0 dgros      (501) staff       (20)     6756 2024-03-16 23:08:47.000000 synthegrator-0.9.3.4/synthegrator/execution_threading.py
--rw-r--r--   0 dgros      (501) staff       (20)     6003 2024-03-23 01:20:01.000000 synthegrator-0.9.3.4/synthegrator/few_shotting.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:05:10.558532 synthegrator-0.9.3.4/synthegrator/human_eval/
--rw-r--r--   0 dgros      (501) staff       (20)        0 2023-06-07 15:23:22.000000 synthegrator-0.9.3.4/synthegrator/human_eval/__init__.py
--rw-r--r--   0 dgros      (501) staff       (20)     3516 2023-08-23 21:48:00.000000 synthegrator-0.9.3.4/synthegrator/human_eval/evaluation.py
--rw-r--r--   0 dgros      (501) staff       (20)     6721 2024-03-16 23:08:47.000000 synthegrator-0.9.3.4/synthegrator/human_eval/execution.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:05:10.559672 synthegrator-0.9.3.4/synthegrator/lang_specs/
--rw-r--r--   0 dgros      (501) staff       (20)        0 2023-10-13 20:26:11.000000 synthegrator-0.9.3.4/synthegrator/lang_specs/__init__.py
--rw-r--r--   0 dgros      (501) staff       (20)    11882 2024-03-23 01:20:01.000000 synthegrator-0.9.3.4/synthegrator/lang_specs/lang_spec.py
--rw-r--r--   0 dgros      (501) staff       (20)     5385 2024-03-17 08:36:57.000000 synthegrator-0.9.3.4/synthegrator/lang_specs/lang_spec_java.py
--rw-r--r--   0 dgros      (501) staff       (20)    10908 2024-03-16 23:08:47.000000 synthegrator-0.9.3.4/synthegrator/lang_specs/lang_spec_python.py
--rw-r--r--   0 dgros      (501) staff       (20)     2854 2023-10-13 20:26:11.000000 synthegrator-0.9.3.4/synthegrator/lang_specs/lang_util.py
--rw-r--r--   0 dgros      (501) staff       (20)     4118 2024-03-20 23:50:11.000000 synthegrator-0.9.3.4/synthegrator/lm_few_shotting_tools.py
--rw-r--r--   0 dgros      (501) staff       (20)    11780 2024-01-31 01:30:32.000000 synthegrator-0.9.3.4/synthegrator/memory_fs.py
--rw-r--r--   0 dgros      (501) staff       (20)    19158 2024-03-19 01:39:03.000000 synthegrator-0.9.3.4/synthegrator/problem_rendering.py
--rw-r--r--   0 dgros      (501) staff       (20)    12086 2024-03-21 03:32:15.000000 synthegrator-0.9.3.4/synthegrator/problem_rendering_insertion_tags.py
--rw-r--r--   0 dgros      (501) staff       (20)        0 2024-03-17 08:36:57.000000 synthegrator-0.9.3.4/synthegrator/prompt_renderer_edit.py
--rw-r--r--   0 dgros      (501) staff       (20)    13265 2024-03-19 09:14:42.000000 synthegrator-0.9.3.4/synthegrator/prompt_renderer_questions.py
--rw-r--r--   0 dgros      (501) staff       (20)     2046 2023-10-04 00:58:52.000000 synthegrator-0.9.3.4/synthegrator/prompting_test_case_selection.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:05:10.560339 synthegrator-0.9.3.4/synthegrator/randomstuff/
--rw-r--r--   0 dgros      (501) staff       (20)        0 2023-06-30 22:33:24.000000 synthegrator-0.9.3.4/synthegrator/randomstuff/__init__.py
--rw-r--r--   0 dgros      (501) staff       (20)      115 2023-08-10 05:46:51.000000 synthegrator-0.9.3.4/synthegrator/randomstuff/getk.py
--rw-r--r--   0 dgros      (501) staff       (20)      446 2023-08-23 21:48:00.000000 synthegrator-0.9.3.4/synthegrator/randomstuff/hellolangchain.py
--rw-r--r--   0 dgros      (501) staff       (20)     9488 2024-03-20 23:50:39.000000 synthegrator-0.9.3.4/synthegrator/response_parser.py
--rw-r--r--   0 dgros      (501) staff       (20)    18264 2024-04-24 03:55:04.000000 synthegrator-0.9.3.4/synthegrator/sandboxing.py
--rw-r--r--   0 dgros      (501) staff       (20)    23920 2024-04-24 02:16:05.000000 synthegrator-0.9.3.4/synthegrator/solution_eval.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:05:10.561947 synthegrator-0.9.3.4/synthegrator/synthdatasets/
--rw-r--r--   0 dgros      (501) staff       (20)        0 2023-08-10 05:46:51.000000 synthegrator-0.9.3.4/synthegrator/synthdatasets/__init__.py
--rw-r--r--   0 dgros      (501) staff       (20)     8168 2024-03-16 23:08:47.000000 synthegrator-0.9.3.4/synthegrator/synthdatasets/apps.py
--rw-r--r--   0 dgros      (501) staff       (20)     9523 2024-04-24 01:30:36.000000 synthegrator-0.9.3.4/synthegrator/synthdatasets/defects4j.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:05:10.563173 synthegrator-0.9.3.4/synthegrator/synthdatasets/defects4j_data/
--rw-r--r--   0 dgros      (501) staff       (20)      912 2024-01-31 01:30:33.000000 synthegrator-0.9.3.4/synthegrator/synthdatasets/defects4j_data/dataset.py
--rw-r--r--   0 dgros      (501) staff       (20)    14296 2024-03-17 08:36:57.000000 synthegrator-0.9.3.4/synthegrator/synthdatasets/defects4j_data/defects4j_script.py
--rw-r--r--   0 dgros      (501) staff       (20)     1365 2024-01-31 01:30:33.000000 synthegrator-0.9.3.4/synthegrator/synthdatasets/defects4j_data/projcleanup.py
--rw-r--r--   0 dgros      (501) staff       (20)     9042 2024-03-21 03:32:15.000000 synthegrator-0.9.3.4/synthegrator/synthdatasets/dypybench.py
--rw-r--r--   0 dgros      (501) staff       (20)     4274 2024-03-20 06:32:16.000000 synthegrator-0.9.3.4/synthegrator/synthdatasets/human_eval.py
--rw-r--r--   0 dgros      (501) staff       (20)      436 2024-01-31 01:30:33.000000 synthegrator-0.9.3.4/synthegrator/synthdatasets/humxplay.py
--rw-r--r--   0 dgros      (501) staff       (20)    15796 2024-03-16 23:08:47.000000 synthegrator-0.9.3.4/synthegrator/synthdatasets/mbpp.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:05:10.566983 synthegrator-0.9.3.4/synthegrator/tests/
--rw-r--r--   0 dgros      (501) staff       (20)        0 2023-06-07 15:22:25.000000 synthegrator-0.9.3.4/synthegrator/tests/__init__.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:05:10.571889 synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/
--rw-r--r--   0 dgros      (501) staff       (20)        0 2023-10-19 06:45:25.000000 synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/__init__.py
--rw-r--r--   0 dgros      (501) staff       (20)     1011 2023-10-19 06:45:25.000000 synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_code_problem.py
--rw-r--r--   0 dgros      (501) staff       (20)    26073 2024-03-22 00:38:03.000000 synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_code_solver.py
--rw-r--r--   0 dgros      (501) staff       (20)     2095 2024-02-21 20:24:16.000000 synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_df_converters.py
--rw-r--r--   0 dgros      (501) staff       (20)     3283 2024-03-16 23:08:47.000000 synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_environments.py
--rw-r--r--   0 dgros      (501) staff       (20)     1311 2024-01-31 01:30:33.000000 synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_examples.py
--rw-r--r--   0 dgros      (501) staff       (20)     1382 2024-03-23 01:20:01.000000 synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_few_shot_library.py
--rw-r--r--   0 dgros      (501) staff       (20)     8604 2024-03-21 19:45:20.000000 synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_java_stuff.py
--rw-r--r--   0 dgros      (501) staff       (20)     5090 2023-10-19 06:45:25.000000 synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_lang_spec.py
--rw-r--r--   0 dgros      (501) staff       (20)     1877 2024-03-16 23:08:47.000000 synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_line_str.py
--rw-r--r--   0 dgros      (501) staff       (20)     4537 2023-10-19 06:45:25.000000 synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_parsing.py
--rw-r--r--   0 dgros      (501) staff       (20)     9252 2024-03-22 00:38:03.000000 synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_problem_rendering.py
--rw-r--r--   0 dgros      (501) staff       (20)     5703 2024-03-21 03:32:15.000000 synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_problem_rendering_insertion_tags.py
--rw-r--r--   0 dgros      (501) staff       (20)     4716 2023-10-19 06:45:25.000000 synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_sandboxing.py
--rw-r--r--   0 dgros      (501) staff       (20)    18713 2024-04-24 02:16:05.000000 synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_solution_eval.py
--rw-r--r--   0 dgros      (501) staff       (20)    15134 2024-03-17 08:36:57.000000 synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_transformation_spec.py
--rw-r--r--   0 dgros      (501) staff       (20)     2105 2024-03-17 08:36:57.000000 synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_util.py
--rw-r--r--   0 dgros      (501) staff       (20)    13215 2024-03-19 09:14:42.000000 synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_value_question_render.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:05:10.573279 synthegrator-0.9.3.4/synthegrator/tests/x_datasets_tests/
--rw-r--r--   0 dgros      (501) staff       (20)        0 2023-10-19 06:45:25.000000 synthegrator-0.9.3.4/synthegrator/tests/x_datasets_tests/__init__.py
--rw-r--r--   0 dgros      (501) staff       (20)     1873 2024-03-16 23:08:47.000000 synthegrator-0.9.3.4/synthegrator/tests/x_datasets_tests/test_human_eval.py
--rw-r--r--   0 dgros      (501) staff       (20)      749 2023-10-19 06:45:25.000000 synthegrator-0.9.3.4/synthegrator/tests/x_datasets_tests/test_x_apps.py
--rw-r--r--   0 dgros      (501) staff       (20)     7878 2024-02-22 00:28:05.000000 synthegrator-0.9.3.4/synthegrator/tests/x_datasets_tests/test_x_mbpp.py
--rw-r--r--   0 dgros      (501) staff       (20)     8407 2024-04-24 01:39:02.000000 synthegrator-0.9.3.4/synthegrator/tests/x_datasets_tests/test_xx_defects4j.py
--rw-r--r--   0 dgros      (501) staff       (20)    23956 2024-04-24 02:16:05.000000 synthegrator-0.9.3.4/synthegrator/tests/x_datasets_tests/test_xx_dypybench.py
--rw-r--r--   0 dgros      (501) staff       (20)     1169 2024-03-17 08:37:58.000000 synthegrator-0.9.3.4/synthegrator/toytest.py
--rw-r--r--   0 dgros      (501) staff       (20)    37291 2024-04-11 20:07:27.000000 synthegrator-0.9.3.4/synthegrator/transformation_spec.py
--rw-r--r--   0 dgros      (501) staff       (20)     1199 2023-10-04 00:58:52.000000 synthegrator-0.9.3.4/synthegrator/uncertainty_modeling.py
--rw-r--r--   0 dgros      (501) staff       (20)    12278 2024-03-20 20:00:19.000000 synthegrator-0.9.3.4/synthegrator/util.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:05:10.573539 synthegrator-0.9.3.4/synthegrator.egg-info/
--rw-r--r--   0 dgros      (501) staff       (20)     4657 2024-04-24 19:05:10.000000 synthegrator-0.9.3.4/synthegrator.egg-info/PKG-INFO
--rw-r--r--   0 dgros      (501) staff       (20)     3470 2024-04-24 19:05:10.000000 synthegrator-0.9.3.4/synthegrator.egg-info/SOURCES.txt
--rw-r--r--   0 dgros      (501) staff       (20)        1 2024-04-24 19:05:10.000000 synthegrator-0.9.3.4/synthegrator.egg-info/dependency_links.txt
--rw-r--r--   0 dgros      (501) staff       (20)      370 2024-04-24 19:05:10.000000 synthegrator-0.9.3.4/synthegrator.egg-info/requires.txt
--rw-r--r--   0 dgros      (501) staff       (20)       13 2024-04-24 19:05:10.000000 synthegrator-0.9.3.4/synthegrator.egg-info/top_level.txt
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:57:10.467320 synthegrator-0.9.3.5/
+-rw-r--r--   0 dgros      (501) staff       (20)     1074 2024-01-31 01:30:32.000000 synthegrator-0.9.3.5/LICENSE
+-rw-r--r--   0 dgros      (501) staff       (20)     4657 2024-04-24 19:57:10.467059 synthegrator-0.9.3.5/PKG-INFO
+-rw-r--r--   0 dgros      (501) staff       (20)     2344 2024-02-07 16:58:12.000000 synthegrator-0.9.3.5/README.md
+-rw-r--r--   0 dgros      (501) staff       (20)     5031 2024-04-24 19:13:29.000000 synthegrator-0.9.3.5/pyproject.toml
+-rw-r--r--   0 dgros      (501) staff       (20)       38 2024-04-24 19:57:10.467365 synthegrator-0.9.3.5/setup.cfg
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:57:10.452232 synthegrator-0.9.3.5/synthegrator/
+-rw-r--r--   0 dgros      (501) staff       (20)        0 2023-06-07 15:22:13.000000 synthegrator-0.9.3.5/synthegrator/__init__.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:57:10.453128 synthegrator-0.9.3.5/synthegrator/_vendor/
+-rw-r--r--   0 dgros      (501) staff       (20)        0 2024-04-24 02:44:40.000000 synthegrator-0.9.3.5/synthegrator/_vendor/__init__.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:57:10.454200 synthegrator-0.9.3.5/synthegrator/_vendor/epicbox/
+-rw-r--r--   0 dgros      (501) staff       (20)       70 2024-04-24 02:48:53.000000 synthegrator-0.9.3.5/synthegrator/_vendor/epicbox/__init__.py
+-rw-r--r--   0 dgros      (501) staff       (20)     2235 2024-04-24 02:48:53.000000 synthegrator-0.9.3.5/synthegrator/_vendor/epicbox/config.py
+-rw-r--r--   0 dgros      (501) staff       (20)      195 2024-04-24 02:48:53.000000 synthegrator-0.9.3.5/synthegrator/_vendor/epicbox/exceptions.py
+-rw-r--r--   0 dgros      (501) staff       (20)    13035 2024-04-24 02:48:53.000000 synthegrator-0.9.3.5/synthegrator/_vendor/epicbox/sandboxes.py
+-rw-r--r--   0 dgros      (501) staff       (20)    10163 2024-04-24 02:48:53.000000 synthegrator-0.9.3.5/synthegrator/_vendor/epicbox/utils.py
+-rw-r--r--   0 dgros      (501) staff       (20)    13611 2024-03-17 08:36:57.000000 synthegrator-0.9.3.5/synthegrator/code_problem_builders.py
+-rw-r--r--   0 dgros      (501) staff       (20)    14744 2024-03-19 03:36:50.000000 synthegrator-0.9.3.5/synthegrator/code_problems.py
+-rw-r--r--   0 dgros      (501) staff       (20)    10006 2024-03-20 20:00:19.000000 synthegrator-0.9.3.5/synthegrator/code_solver.py
+-rw-r--r--   0 dgros      (501) staff       (20)     3756 2024-03-16 23:08:47.000000 synthegrator-0.9.3.5/synthegrator/df_converters.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:57:10.454362 synthegrator-0.9.3.5/synthegrator/dypybench/
+-rw-r--r--   0 dgros      (501) staff       (20)        0 2023-08-10 05:46:51.000000 synthegrator-0.9.3.5/synthegrator/dypybench/__init__.py
+-rw-r--r--   0 dgros      (501) staff       (20)      385 2023-09-07 07:28:11.000000 synthegrator-0.9.3.5/synthegrator/environments.py
+-rw-r--r--   0 dgros      (501) staff       (20)     6756 2024-03-16 23:08:47.000000 synthegrator-0.9.3.5/synthegrator/execution_threading.py
+-rw-r--r--   0 dgros      (501) staff       (20)     6003 2024-03-23 01:20:01.000000 synthegrator-0.9.3.5/synthegrator/few_shotting.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:57:10.454830 synthegrator-0.9.3.5/synthegrator/human_eval/
+-rw-r--r--   0 dgros      (501) staff       (20)        0 2023-06-07 15:23:22.000000 synthegrator-0.9.3.5/synthegrator/human_eval/__init__.py
+-rw-r--r--   0 dgros      (501) staff       (20)     3516 2023-08-23 21:48:00.000000 synthegrator-0.9.3.5/synthegrator/human_eval/evaluation.py
+-rw-r--r--   0 dgros      (501) staff       (20)     6721 2024-03-16 23:08:47.000000 synthegrator-0.9.3.5/synthegrator/human_eval/execution.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:57:10.456395 synthegrator-0.9.3.5/synthegrator/lang_specs/
+-rw-r--r--   0 dgros      (501) staff       (20)        0 2023-10-13 20:26:11.000000 synthegrator-0.9.3.5/synthegrator/lang_specs/__init__.py
+-rw-r--r--   0 dgros      (501) staff       (20)    11882 2024-03-23 01:20:01.000000 synthegrator-0.9.3.5/synthegrator/lang_specs/lang_spec.py
+-rw-r--r--   0 dgros      (501) staff       (20)     5385 2024-03-17 08:36:57.000000 synthegrator-0.9.3.5/synthegrator/lang_specs/lang_spec_java.py
+-rw-r--r--   0 dgros      (501) staff       (20)    10908 2024-03-16 23:08:47.000000 synthegrator-0.9.3.5/synthegrator/lang_specs/lang_spec_python.py
+-rw-r--r--   0 dgros      (501) staff       (20)     2854 2023-10-13 20:26:11.000000 synthegrator-0.9.3.5/synthegrator/lang_specs/lang_util.py
+-rw-r--r--   0 dgros      (501) staff       (20)     4118 2024-03-20 23:50:11.000000 synthegrator-0.9.3.5/synthegrator/lm_few_shotting_tools.py
+-rw-r--r--   0 dgros      (501) staff       (20)    11780 2024-01-31 01:30:32.000000 synthegrator-0.9.3.5/synthegrator/memory_fs.py
+-rw-r--r--   0 dgros      (501) staff       (20)    19158 2024-03-19 01:39:03.000000 synthegrator-0.9.3.5/synthegrator/problem_rendering.py
+-rw-r--r--   0 dgros      (501) staff       (20)    12086 2024-03-21 03:32:15.000000 synthegrator-0.9.3.5/synthegrator/problem_rendering_insertion_tags.py
+-rw-r--r--   0 dgros      (501) staff       (20)        0 2024-03-17 08:36:57.000000 synthegrator-0.9.3.5/synthegrator/prompt_renderer_edit.py
+-rw-r--r--   0 dgros      (501) staff       (20)    13265 2024-03-19 09:14:42.000000 synthegrator-0.9.3.5/synthegrator/prompt_renderer_questions.py
+-rw-r--r--   0 dgros      (501) staff       (20)     2046 2023-10-04 00:58:52.000000 synthegrator-0.9.3.5/synthegrator/prompting_test_case_selection.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:57:10.457028 synthegrator-0.9.3.5/synthegrator/randomstuff/
+-rw-r--r--   0 dgros      (501) staff       (20)        0 2023-06-30 22:33:24.000000 synthegrator-0.9.3.5/synthegrator/randomstuff/__init__.py
+-rw-r--r--   0 dgros      (501) staff       (20)      115 2023-08-10 05:46:51.000000 synthegrator-0.9.3.5/synthegrator/randomstuff/getk.py
+-rw-r--r--   0 dgros      (501) staff       (20)      446 2023-08-23 21:48:00.000000 synthegrator-0.9.3.5/synthegrator/randomstuff/hellolangchain.py
+-rw-r--r--   0 dgros      (501) staff       (20)     9488 2024-03-20 23:50:39.000000 synthegrator-0.9.3.5/synthegrator/response_parser.py
+-rw-r--r--   0 dgros      (501) staff       (20)    18264 2024-04-24 03:55:04.000000 synthegrator-0.9.3.5/synthegrator/sandboxing.py
+-rw-r--r--   0 dgros      (501) staff       (20)    23920 2024-04-24 02:16:05.000000 synthegrator-0.9.3.5/synthegrator/solution_eval.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:57:10.459044 synthegrator-0.9.3.5/synthegrator/synthdatasets/
+-rw-r--r--   0 dgros      (501) staff       (20)        0 2023-08-10 05:46:51.000000 synthegrator-0.9.3.5/synthegrator/synthdatasets/__init__.py
+-rw-r--r--   0 dgros      (501) staff       (20)     8168 2024-03-16 23:08:47.000000 synthegrator-0.9.3.5/synthegrator/synthdatasets/apps.py
+-rw-r--r--   0 dgros      (501) staff       (20)     9523 2024-04-24 01:30:36.000000 synthegrator-0.9.3.5/synthegrator/synthdatasets/defects4j.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:57:10.459839 synthegrator-0.9.3.5/synthegrator/synthdatasets/defects4j_data/
+-rw-r--r--   0 dgros      (501) staff       (20)      912 2024-01-31 01:30:33.000000 synthegrator-0.9.3.5/synthegrator/synthdatasets/defects4j_data/dataset.py
+-rw-r--r--   0 dgros      (501) staff       (20)    14296 2024-03-17 08:36:57.000000 synthegrator-0.9.3.5/synthegrator/synthdatasets/defects4j_data/defects4j_script.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1365 2024-01-31 01:30:33.000000 synthegrator-0.9.3.5/synthegrator/synthdatasets/defects4j_data/projcleanup.py
+-rw-r--r--   0 dgros      (501) staff       (20)     9042 2024-03-21 03:32:15.000000 synthegrator-0.9.3.5/synthegrator/synthdatasets/dypybench.py
+-rw-r--r--   0 dgros      (501) staff       (20)     4274 2024-03-20 06:32:16.000000 synthegrator-0.9.3.5/synthegrator/synthdatasets/human_eval.py
+-rw-r--r--   0 dgros      (501) staff       (20)      436 2024-01-31 01:30:33.000000 synthegrator-0.9.3.5/synthegrator/synthdatasets/humxplay.py
+-rw-r--r--   0 dgros      (501) staff       (20)    15796 2024-03-16 23:08:47.000000 synthegrator-0.9.3.5/synthegrator/synthdatasets/mbpp.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:57:10.460033 synthegrator-0.9.3.5/synthegrator/tests/
+-rw-r--r--   0 dgros      (501) staff       (20)        0 2023-06-07 15:22:25.000000 synthegrator-0.9.3.5/synthegrator/tests/__init__.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:57:10.464659 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/
+-rw-r--r--   0 dgros      (501) staff       (20)        0 2023-10-19 06:45:25.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/__init__.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1011 2023-10-19 06:45:25.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_code_problem.py
+-rw-r--r--   0 dgros      (501) staff       (20)    26073 2024-03-22 00:38:03.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_code_solver.py
+-rw-r--r--   0 dgros      (501) staff       (20)     2095 2024-02-21 20:24:16.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_df_converters.py
+-rw-r--r--   0 dgros      (501) staff       (20)     3283 2024-03-16 23:08:47.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_environments.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1311 2024-01-31 01:30:33.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_examples.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1382 2024-03-23 01:20:01.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_few_shot_library.py
+-rw-r--r--   0 dgros      (501) staff       (20)     8604 2024-03-21 19:45:20.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_java_stuff.py
+-rw-r--r--   0 dgros      (501) staff       (20)     5090 2023-10-19 06:45:25.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_lang_spec.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1877 2024-03-16 23:08:47.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_line_str.py
+-rw-r--r--   0 dgros      (501) staff       (20)     4537 2023-10-19 06:45:25.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_parsing.py
+-rw-r--r--   0 dgros      (501) staff       (20)     9252 2024-03-22 00:38:03.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_problem_rendering.py
+-rw-r--r--   0 dgros      (501) staff       (20)     5703 2024-03-21 03:32:15.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_problem_rendering_insertion_tags.py
+-rw-r--r--   0 dgros      (501) staff       (20)     4716 2023-10-19 06:45:25.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_sandboxing.py
+-rw-r--r--   0 dgros      (501) staff       (20)    18713 2024-04-24 02:16:05.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_solution_eval.py
+-rw-r--r--   0 dgros      (501) staff       (20)    15134 2024-03-17 08:36:57.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_transformation_spec.py
+-rw-r--r--   0 dgros      (501) staff       (20)     2105 2024-03-17 08:36:57.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_util.py
+-rw-r--r--   0 dgros      (501) staff       (20)    13215 2024-03-19 09:14:42.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_value_question_render.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:57:10.466126 synthegrator-0.9.3.5/synthegrator/tests/x_datasets_tests/
+-rw-r--r--   0 dgros      (501) staff       (20)        0 2023-10-19 06:45:25.000000 synthegrator-0.9.3.5/synthegrator/tests/x_datasets_tests/__init__.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1873 2024-03-16 23:08:47.000000 synthegrator-0.9.3.5/synthegrator/tests/x_datasets_tests/test_human_eval.py
+-rw-r--r--   0 dgros      (501) staff       (20)      749 2023-10-19 06:45:25.000000 synthegrator-0.9.3.5/synthegrator/tests/x_datasets_tests/test_x_apps.py
+-rw-r--r--   0 dgros      (501) staff       (20)     7878 2024-02-22 00:28:05.000000 synthegrator-0.9.3.5/synthegrator/tests/x_datasets_tests/test_x_mbpp.py
+-rw-r--r--   0 dgros      (501) staff       (20)     8407 2024-04-24 01:39:02.000000 synthegrator-0.9.3.5/synthegrator/tests/x_datasets_tests/test_xx_defects4j.py
+-rw-r--r--   0 dgros      (501) staff       (20)    23956 2024-04-24 02:16:05.000000 synthegrator-0.9.3.5/synthegrator/tests/x_datasets_tests/test_xx_dypybench.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1169 2024-03-17 08:37:58.000000 synthegrator-0.9.3.5/synthegrator/toytest.py
+-rw-r--r--   0 dgros      (501) staff       (20)    37291 2024-04-11 20:07:27.000000 synthegrator-0.9.3.5/synthegrator/transformation_spec.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1199 2023-10-04 00:58:52.000000 synthegrator-0.9.3.5/synthegrator/uncertainty_modeling.py
+-rw-r--r--   0 dgros      (501) staff       (20)    12278 2024-03-20 20:00:19.000000 synthegrator-0.9.3.5/synthegrator/util.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:57:10.466436 synthegrator-0.9.3.5/synthegrator.egg-info/
+-rw-r--r--   0 dgros      (501) staff       (20)     4657 2024-04-24 19:57:10.000000 synthegrator-0.9.3.5/synthegrator.egg-info/PKG-INFO
+-rw-r--r--   0 dgros      (501) staff       (20)     3470 2024-04-24 19:57:10.000000 synthegrator-0.9.3.5/synthegrator.egg-info/SOURCES.txt
+-rw-r--r--   0 dgros      (501) staff       (20)        1 2024-04-24 19:57:10.000000 synthegrator-0.9.3.5/synthegrator.egg-info/dependency_links.txt
+-rw-r--r--   0 dgros      (501) staff       (20)      370 2024-04-24 19:57:10.000000 synthegrator-0.9.3.5/synthegrator.egg-info/requires.txt
+-rw-r--r--   0 dgros      (501) staff       (20)       13 2024-04-24 19:57:10.000000 synthegrator-0.9.3.5/synthegrator.egg-info/top_level.txt
```

### Comparing `synthegrator-0.9.3.4/LICENSE` & `synthegrator-0.9.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/PKG-INFO` & `synthegrator-0.9.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthegrator
-Version: 0.9.3.4
+Version: 0.9.3.5
 Summary: Framework for code synthesis and AI4SE research
 Author-email: David Gros <DNGros@users.noreply.github.com>, Claudio Spiess <claudiosv@users.noreply.github.com>
 License: Copyright 2024 David Gros, Claudio Spiess
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `synthegrator-0.9.3.4/README.md` & `synthegrator-0.9.3.5/README.md`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/pyproject.toml` & `synthegrator-0.9.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 include = ["synthegrator*"]  # This pattern includes your main package and any subpackages or modules within it.
 
 [tool.pytest]
 python_classes = "ClassNamesAreIgnoredToNotConflictWithSynthegratorClasses"
 
 [project]
 name = "synthegrator"
-version = "0.9.3.4"
+version = "0.9.3.5"
 authors = [
     { name = "David Gros", email = "DNGros@users.noreply.github.com" },
     { name = "Claudio Spiess", email = "claudiosv@users.noreply.github.com" },
 ]
 description = "Framework for code synthesis and AI4SE research"
 license = { file = "LICENSE" }
 readme = "README.md"
```

### Comparing `synthegrator-0.9.3.4/synthegrator/_vendor/epicbox/config.py` & `synthegrator-0.9.3.5/synthegrator/_vendor/epicbox/config.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/_vendor/epicbox/sandboxes.py` & `synthegrator-0.9.3.5/synthegrator/_vendor/epicbox/sandboxes.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/_vendor/epicbox/utils.py` & `synthegrator-0.9.3.5/synthegrator/_vendor/epicbox/utils.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/code_problem_builders.py` & `synthegrator-0.9.3.5/synthegrator/code_problem_builders.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/code_problems.py` & `synthegrator-0.9.3.5/synthegrator/code_problems.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/code_solver.py` & `synthegrator-0.9.3.5/synthegrator/code_solver.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/df_converters.py` & `synthegrator-0.9.3.5/synthegrator/df_converters.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/execution_threading.py` & `synthegrator-0.9.3.5/synthegrator/execution_threading.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/few_shotting.py` & `synthegrator-0.9.3.5/synthegrator/few_shotting.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/human_eval/evaluation.py` & `synthegrator-0.9.3.5/synthegrator/human_eval/evaluation.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/human_eval/execution.py` & `synthegrator-0.9.3.5/synthegrator/human_eval/execution.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/lang_specs/lang_spec.py` & `synthegrator-0.9.3.5/synthegrator/lang_specs/lang_spec.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/lang_specs/lang_spec_java.py` & `synthegrator-0.9.3.5/synthegrator/lang_specs/lang_spec_java.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/lang_specs/lang_spec_python.py` & `synthegrator-0.9.3.5/synthegrator/lang_specs/lang_spec_python.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/lang_specs/lang_util.py` & `synthegrator-0.9.3.5/synthegrator/lang_specs/lang_util.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/lm_few_shotting_tools.py` & `synthegrator-0.9.3.5/synthegrator/lm_few_shotting_tools.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/memory_fs.py` & `synthegrator-0.9.3.5/synthegrator/memory_fs.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/problem_rendering.py` & `synthegrator-0.9.3.5/synthegrator/problem_rendering.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/problem_rendering_insertion_tags.py` & `synthegrator-0.9.3.5/synthegrator/problem_rendering_insertion_tags.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/prompt_renderer_questions.py` & `synthegrator-0.9.3.5/synthegrator/prompt_renderer_questions.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/prompting_test_case_selection.py` & `synthegrator-0.9.3.5/synthegrator/prompting_test_case_selection.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/response_parser.py` & `synthegrator-0.9.3.5/synthegrator/response_parser.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/sandboxing.py` & `synthegrator-0.9.3.5/synthegrator/sandboxing.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/solution_eval.py` & `synthegrator-0.9.3.5/synthegrator/solution_eval.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/synthdatasets/apps.py` & `synthegrator-0.9.3.5/synthegrator/synthdatasets/apps.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/synthdatasets/defects4j.py` & `synthegrator-0.9.3.5/synthegrator/synthdatasets/defects4j.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/synthdatasets/defects4j_data/dataset.py` & `synthegrator-0.9.3.5/synthegrator/synthdatasets/defects4j_data/dataset.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/synthdatasets/defects4j_data/defects4j_script.py` & `synthegrator-0.9.3.5/synthegrator/synthdatasets/defects4j_data/defects4j_script.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/synthdatasets/defects4j_data/projcleanup.py` & `synthegrator-0.9.3.5/synthegrator/synthdatasets/defects4j_data/projcleanup.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/synthdatasets/dypybench.py` & `synthegrator-0.9.3.5/synthegrator/synthdatasets/dypybench.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/synthdatasets/human_eval.py` & `synthegrator-0.9.3.5/synthegrator/synthdatasets/human_eval.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/synthdatasets/mbpp.py` & `synthegrator-0.9.3.5/synthegrator/synthdatasets/mbpp.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_code_problem.py` & `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_code_problem.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_code_solver.py` & `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_code_solver.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_df_converters.py` & `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_df_converters.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_environments.py` & `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_examples.py` & `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_few_shot_library.py` & `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_few_shot_library.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_java_stuff.py` & `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_java_stuff.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_lang_spec.py` & `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_lang_spec.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_line_str.py` & `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_line_str.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_parsing.py` & `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_problem_rendering.py` & `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_problem_rendering.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_problem_rendering_insertion_tags.py` & `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_problem_rendering_insertion_tags.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_sandboxing.py` & `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_sandboxing.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_solution_eval.py` & `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_solution_eval.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_transformation_spec.py` & `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_transformation_spec.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_util.py` & `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_util.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/tests/non_dataset_tests/test_value_question_render.py` & `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_value_question_render.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/tests/x_datasets_tests/test_human_eval.py` & `synthegrator-0.9.3.5/synthegrator/tests/x_datasets_tests/test_human_eval.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/tests/x_datasets_tests/test_x_apps.py` & `synthegrator-0.9.3.5/synthegrator/tests/x_datasets_tests/test_x_apps.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/tests/x_datasets_tests/test_x_mbpp.py` & `synthegrator-0.9.3.5/synthegrator/tests/x_datasets_tests/test_x_mbpp.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/tests/x_datasets_tests/test_xx_defects4j.py` & `synthegrator-0.9.3.5/synthegrator/tests/x_datasets_tests/test_xx_defects4j.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/tests/x_datasets_tests/test_xx_dypybench.py` & `synthegrator-0.9.3.5/synthegrator/tests/x_datasets_tests/test_xx_dypybench.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/toytest.py` & `synthegrator-0.9.3.5/synthegrator/toytest.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/transformation_spec.py` & `synthegrator-0.9.3.5/synthegrator/transformation_spec.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/uncertainty_modeling.py` & `synthegrator-0.9.3.5/synthegrator/uncertainty_modeling.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator/util.py` & `synthegrator-0.9.3.5/synthegrator/util.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.4/synthegrator.egg-info/PKG-INFO` & `synthegrator-0.9.3.5/synthegrator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthegrator
-Version: 0.9.3.4
+Version: 0.9.3.5
 Summary: Framework for code synthesis and AI4SE research
 Author-email: David Gros <DNGros@users.noreply.github.com>, Claudio Spiess <claudiosv@users.noreply.github.com>
 License: Copyright 2024 David Gros, Claudio Spiess
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `synthegrator-0.9.3.4/synthegrator.egg-info/SOURCES.txt` & `synthegrator-0.9.3.5/synthegrator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

