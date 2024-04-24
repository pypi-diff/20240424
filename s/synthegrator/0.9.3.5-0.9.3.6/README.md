# Comparing `tmp/synthegrator-0.9.3.5.tar.gz` & `tmp/synthegrator-0.9.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthegrator-0.9.3.5.tar", last modified: Wed Apr 24 19:57:10 2024, max compression
+gzip compressed data, was "synthegrator-0.9.3.6.tar", last modified: Wed Apr 24 20:32:50 2024, max compression
```

## Comparing `synthegrator-0.9.3.5.tar` & `synthegrator-0.9.3.6.tar`

### file list

```diff
@@ -1,99 +1,2221 @@
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:57:10.467320 synthegrator-0.9.3.5/
--rw-r--r--   0 dgros      (501) staff       (20)     1074 2024-01-31 01:30:32.000000 synthegrator-0.9.3.5/LICENSE
--rw-r--r--   0 dgros      (501) staff       (20)     4657 2024-04-24 19:57:10.467059 synthegrator-0.9.3.5/PKG-INFO
--rw-r--r--   0 dgros      (501) staff       (20)     2344 2024-02-07 16:58:12.000000 synthegrator-0.9.3.5/README.md
--rw-r--r--   0 dgros      (501) staff       (20)     5031 2024-04-24 19:13:29.000000 synthegrator-0.9.3.5/pyproject.toml
--rw-r--r--   0 dgros      (501) staff       (20)       38 2024-04-24 19:57:10.467365 synthegrator-0.9.3.5/setup.cfg
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:57:10.452232 synthegrator-0.9.3.5/synthegrator/
--rw-r--r--   0 dgros      (501) staff       (20)        0 2023-06-07 15:22:13.000000 synthegrator-0.9.3.5/synthegrator/__init__.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:57:10.453128 synthegrator-0.9.3.5/synthegrator/_vendor/
--rw-r--r--   0 dgros      (501) staff       (20)        0 2024-04-24 02:44:40.000000 synthegrator-0.9.3.5/synthegrator/_vendor/__init__.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:57:10.454200 synthegrator-0.9.3.5/synthegrator/_vendor/epicbox/
--rw-r--r--   0 dgros      (501) staff       (20)       70 2024-04-24 02:48:53.000000 synthegrator-0.9.3.5/synthegrator/_vendor/epicbox/__init__.py
--rw-r--r--   0 dgros      (501) staff       (20)     2235 2024-04-24 02:48:53.000000 synthegrator-0.9.3.5/synthegrator/_vendor/epicbox/config.py
--rw-r--r--   0 dgros      (501) staff       (20)      195 2024-04-24 02:48:53.000000 synthegrator-0.9.3.5/synthegrator/_vendor/epicbox/exceptions.py
--rw-r--r--   0 dgros      (501) staff       (20)    13035 2024-04-24 02:48:53.000000 synthegrator-0.9.3.5/synthegrator/_vendor/epicbox/sandboxes.py
--rw-r--r--   0 dgros      (501) staff       (20)    10163 2024-04-24 02:48:53.000000 synthegrator-0.9.3.5/synthegrator/_vendor/epicbox/utils.py
--rw-r--r--   0 dgros      (501) staff       (20)    13611 2024-03-17 08:36:57.000000 synthegrator-0.9.3.5/synthegrator/code_problem_builders.py
--rw-r--r--   0 dgros      (501) staff       (20)    14744 2024-03-19 03:36:50.000000 synthegrator-0.9.3.5/synthegrator/code_problems.py
--rw-r--r--   0 dgros      (501) staff       (20)    10006 2024-03-20 20:00:19.000000 synthegrator-0.9.3.5/synthegrator/code_solver.py
--rw-r--r--   0 dgros      (501) staff       (20)     3756 2024-03-16 23:08:47.000000 synthegrator-0.9.3.5/synthegrator/df_converters.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:57:10.454362 synthegrator-0.9.3.5/synthegrator/dypybench/
--rw-r--r--   0 dgros      (501) staff       (20)        0 2023-08-10 05:46:51.000000 synthegrator-0.9.3.5/synthegrator/dypybench/__init__.py
--rw-r--r--   0 dgros      (501) staff       (20)      385 2023-09-07 07:28:11.000000 synthegrator-0.9.3.5/synthegrator/environments.py
--rw-r--r--   0 dgros      (501) staff       (20)     6756 2024-03-16 23:08:47.000000 synthegrator-0.9.3.5/synthegrator/execution_threading.py
--rw-r--r--   0 dgros      (501) staff       (20)     6003 2024-03-23 01:20:01.000000 synthegrator-0.9.3.5/synthegrator/few_shotting.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:57:10.454830 synthegrator-0.9.3.5/synthegrator/human_eval/
--rw-r--r--   0 dgros      (501) staff       (20)        0 2023-06-07 15:23:22.000000 synthegrator-0.9.3.5/synthegrator/human_eval/__init__.py
--rw-r--r--   0 dgros      (501) staff       (20)     3516 2023-08-23 21:48:00.000000 synthegrator-0.9.3.5/synthegrator/human_eval/evaluation.py
--rw-r--r--   0 dgros      (501) staff       (20)     6721 2024-03-16 23:08:47.000000 synthegrator-0.9.3.5/synthegrator/human_eval/execution.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:57:10.456395 synthegrator-0.9.3.5/synthegrator/lang_specs/
--rw-r--r--   0 dgros      (501) staff       (20)        0 2023-10-13 20:26:11.000000 synthegrator-0.9.3.5/synthegrator/lang_specs/__init__.py
--rw-r--r--   0 dgros      (501) staff       (20)    11882 2024-03-23 01:20:01.000000 synthegrator-0.9.3.5/synthegrator/lang_specs/lang_spec.py
--rw-r--r--   0 dgros      (501) staff       (20)     5385 2024-03-17 08:36:57.000000 synthegrator-0.9.3.5/synthegrator/lang_specs/lang_spec_java.py
--rw-r--r--   0 dgros      (501) staff       (20)    10908 2024-03-16 23:08:47.000000 synthegrator-0.9.3.5/synthegrator/lang_specs/lang_spec_python.py
--rw-r--r--   0 dgros      (501) staff       (20)     2854 2023-10-13 20:26:11.000000 synthegrator-0.9.3.5/synthegrator/lang_specs/lang_util.py
--rw-r--r--   0 dgros      (501) staff       (20)     4118 2024-03-20 23:50:11.000000 synthegrator-0.9.3.5/synthegrator/lm_few_shotting_tools.py
--rw-r--r--   0 dgros      (501) staff       (20)    11780 2024-01-31 01:30:32.000000 synthegrator-0.9.3.5/synthegrator/memory_fs.py
--rw-r--r--   0 dgros      (501) staff       (20)    19158 2024-03-19 01:39:03.000000 synthegrator-0.9.3.5/synthegrator/problem_rendering.py
--rw-r--r--   0 dgros      (501) staff       (20)    12086 2024-03-21 03:32:15.000000 synthegrator-0.9.3.5/synthegrator/problem_rendering_insertion_tags.py
--rw-r--r--   0 dgros      (501) staff       (20)        0 2024-03-17 08:36:57.000000 synthegrator-0.9.3.5/synthegrator/prompt_renderer_edit.py
--rw-r--r--   0 dgros      (501) staff       (20)    13265 2024-03-19 09:14:42.000000 synthegrator-0.9.3.5/synthegrator/prompt_renderer_questions.py
--rw-r--r--   0 dgros      (501) staff       (20)     2046 2023-10-04 00:58:52.000000 synthegrator-0.9.3.5/synthegrator/prompting_test_case_selection.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:57:10.457028 synthegrator-0.9.3.5/synthegrator/randomstuff/
--rw-r--r--   0 dgros      (501) staff       (20)        0 2023-06-30 22:33:24.000000 synthegrator-0.9.3.5/synthegrator/randomstuff/__init__.py
--rw-r--r--   0 dgros      (501) staff       (20)      115 2023-08-10 05:46:51.000000 synthegrator-0.9.3.5/synthegrator/randomstuff/getk.py
--rw-r--r--   0 dgros      (501) staff       (20)      446 2023-08-23 21:48:00.000000 synthegrator-0.9.3.5/synthegrator/randomstuff/hellolangchain.py
--rw-r--r--   0 dgros      (501) staff       (20)     9488 2024-03-20 23:50:39.000000 synthegrator-0.9.3.5/synthegrator/response_parser.py
--rw-r--r--   0 dgros      (501) staff       (20)    18264 2024-04-24 03:55:04.000000 synthegrator-0.9.3.5/synthegrator/sandboxing.py
--rw-r--r--   0 dgros      (501) staff       (20)    23920 2024-04-24 02:16:05.000000 synthegrator-0.9.3.5/synthegrator/solution_eval.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:57:10.459044 synthegrator-0.9.3.5/synthegrator/synthdatasets/
--rw-r--r--   0 dgros      (501) staff       (20)        0 2023-08-10 05:46:51.000000 synthegrator-0.9.3.5/synthegrator/synthdatasets/__init__.py
--rw-r--r--   0 dgros      (501) staff       (20)     8168 2024-03-16 23:08:47.000000 synthegrator-0.9.3.5/synthegrator/synthdatasets/apps.py
--rw-r--r--   0 dgros      (501) staff       (20)     9523 2024-04-24 01:30:36.000000 synthegrator-0.9.3.5/synthegrator/synthdatasets/defects4j.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:57:10.459839 synthegrator-0.9.3.5/synthegrator/synthdatasets/defects4j_data/
--rw-r--r--   0 dgros      (501) staff       (20)      912 2024-01-31 01:30:33.000000 synthegrator-0.9.3.5/synthegrator/synthdatasets/defects4j_data/dataset.py
--rw-r--r--   0 dgros      (501) staff       (20)    14296 2024-03-17 08:36:57.000000 synthegrator-0.9.3.5/synthegrator/synthdatasets/defects4j_data/defects4j_script.py
--rw-r--r--   0 dgros      (501) staff       (20)     1365 2024-01-31 01:30:33.000000 synthegrator-0.9.3.5/synthegrator/synthdatasets/defects4j_data/projcleanup.py
--rw-r--r--   0 dgros      (501) staff       (20)     9042 2024-03-21 03:32:15.000000 synthegrator-0.9.3.5/synthegrator/synthdatasets/dypybench.py
--rw-r--r--   0 dgros      (501) staff       (20)     4274 2024-03-20 06:32:16.000000 synthegrator-0.9.3.5/synthegrator/synthdatasets/human_eval.py
--rw-r--r--   0 dgros      (501) staff       (20)      436 2024-01-31 01:30:33.000000 synthegrator-0.9.3.5/synthegrator/synthdatasets/humxplay.py
--rw-r--r--   0 dgros      (501) staff       (20)    15796 2024-03-16 23:08:47.000000 synthegrator-0.9.3.5/synthegrator/synthdatasets/mbpp.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:57:10.460033 synthegrator-0.9.3.5/synthegrator/tests/
--rw-r--r--   0 dgros      (501) staff       (20)        0 2023-06-07 15:22:25.000000 synthegrator-0.9.3.5/synthegrator/tests/__init__.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:57:10.464659 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/
--rw-r--r--   0 dgros      (501) staff       (20)        0 2023-10-19 06:45:25.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/__init__.py
--rw-r--r--   0 dgros      (501) staff       (20)     1011 2023-10-19 06:45:25.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_code_problem.py
--rw-r--r--   0 dgros      (501) staff       (20)    26073 2024-03-22 00:38:03.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_code_solver.py
--rw-r--r--   0 dgros      (501) staff       (20)     2095 2024-02-21 20:24:16.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_df_converters.py
--rw-r--r--   0 dgros      (501) staff       (20)     3283 2024-03-16 23:08:47.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_environments.py
--rw-r--r--   0 dgros      (501) staff       (20)     1311 2024-01-31 01:30:33.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_examples.py
--rw-r--r--   0 dgros      (501) staff       (20)     1382 2024-03-23 01:20:01.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_few_shot_library.py
--rw-r--r--   0 dgros      (501) staff       (20)     8604 2024-03-21 19:45:20.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_java_stuff.py
--rw-r--r--   0 dgros      (501) staff       (20)     5090 2023-10-19 06:45:25.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_lang_spec.py
--rw-r--r--   0 dgros      (501) staff       (20)     1877 2024-03-16 23:08:47.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_line_str.py
--rw-r--r--   0 dgros      (501) staff       (20)     4537 2023-10-19 06:45:25.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_parsing.py
--rw-r--r--   0 dgros      (501) staff       (20)     9252 2024-03-22 00:38:03.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_problem_rendering.py
--rw-r--r--   0 dgros      (501) staff       (20)     5703 2024-03-21 03:32:15.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_problem_rendering_insertion_tags.py
--rw-r--r--   0 dgros      (501) staff       (20)     4716 2023-10-19 06:45:25.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_sandboxing.py
--rw-r--r--   0 dgros      (501) staff       (20)    18713 2024-04-24 02:16:05.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_solution_eval.py
--rw-r--r--   0 dgros      (501) staff       (20)    15134 2024-03-17 08:36:57.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_transformation_spec.py
--rw-r--r--   0 dgros      (501) staff       (20)     2105 2024-03-17 08:36:57.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_util.py
--rw-r--r--   0 dgros      (501) staff       (20)    13215 2024-03-19 09:14:42.000000 synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_value_question_render.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:57:10.466126 synthegrator-0.9.3.5/synthegrator/tests/x_datasets_tests/
--rw-r--r--   0 dgros      (501) staff       (20)        0 2023-10-19 06:45:25.000000 synthegrator-0.9.3.5/synthegrator/tests/x_datasets_tests/__init__.py
--rw-r--r--   0 dgros      (501) staff       (20)     1873 2024-03-16 23:08:47.000000 synthegrator-0.9.3.5/synthegrator/tests/x_datasets_tests/test_human_eval.py
--rw-r--r--   0 dgros      (501) staff       (20)      749 2023-10-19 06:45:25.000000 synthegrator-0.9.3.5/synthegrator/tests/x_datasets_tests/test_x_apps.py
--rw-r--r--   0 dgros      (501) staff       (20)     7878 2024-02-22 00:28:05.000000 synthegrator-0.9.3.5/synthegrator/tests/x_datasets_tests/test_x_mbpp.py
--rw-r--r--   0 dgros      (501) staff       (20)     8407 2024-04-24 01:39:02.000000 synthegrator-0.9.3.5/synthegrator/tests/x_datasets_tests/test_xx_defects4j.py
--rw-r--r--   0 dgros      (501) staff       (20)    23956 2024-04-24 02:16:05.000000 synthegrator-0.9.3.5/synthegrator/tests/x_datasets_tests/test_xx_dypybench.py
--rw-r--r--   0 dgros      (501) staff       (20)     1169 2024-03-17 08:37:58.000000 synthegrator-0.9.3.5/synthegrator/toytest.py
--rw-r--r--   0 dgros      (501) staff       (20)    37291 2024-04-11 20:07:27.000000 synthegrator-0.9.3.5/synthegrator/transformation_spec.py
--rw-r--r--   0 dgros      (501) staff       (20)     1199 2023-10-04 00:58:52.000000 synthegrator-0.9.3.5/synthegrator/uncertainty_modeling.py
--rw-r--r--   0 dgros      (501) staff       (20)    12278 2024-03-20 20:00:19.000000 synthegrator-0.9.3.5/synthegrator/util.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 19:57:10.466436 synthegrator-0.9.3.5/synthegrator.egg-info/
--rw-r--r--   0 dgros      (501) staff       (20)     4657 2024-04-24 19:57:10.000000 synthegrator-0.9.3.5/synthegrator.egg-info/PKG-INFO
--rw-r--r--   0 dgros      (501) staff       (20)     3470 2024-04-24 19:57:10.000000 synthegrator-0.9.3.5/synthegrator.egg-info/SOURCES.txt
--rw-r--r--   0 dgros      (501) staff       (20)        1 2024-04-24 19:57:10.000000 synthegrator-0.9.3.5/synthegrator.egg-info/dependency_links.txt
--rw-r--r--   0 dgros      (501) staff       (20)      370 2024-04-24 19:57:10.000000 synthegrator-0.9.3.5/synthegrator.egg-info/requires.txt
--rw-r--r--   0 dgros      (501) staff       (20)       13 2024-04-24 19:57:10.000000 synthegrator-0.9.3.5/synthegrator.egg-info/top_level.txt
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.571369 synthegrator-0.9.3.6/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.182669 synthegrator-0.9.3.6/.github/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.428140 synthegrator-0.9.3.6/.github/workflows/
+-rw-r--r--   0 dgros      (501) staff       (20)      998 2024-03-16 23:08:47.000000 synthegrator-0.9.3.6/.github/workflows/python-package.yml
+-rw-r--r--   0 dgros      (501) staff       (20)     3273 2024-04-24 20:24:25.000000 synthegrator-0.9.3.6/.gitignore
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.428893 synthegrator-0.9.3.6/.vscode/
+-rw-r--r--   0 dgros      (501) staff       (20)      495 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/.vscode/launch.json
+-rw-r--r--   0 dgros      (501) staff       (20)      131 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/.vscode/settings.json
+-rw-r--r--   0 dgros      (501) staff       (20)     1074 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/LICENSE
+-rw-r--r--   0 dgros      (501) staff       (20)     4602 2024-04-24 20:32:50.570932 synthegrator-0.9.3.6/PKG-INFO
+-rw-r--r--   0 dgros      (501) staff       (20)     2289 2024-04-24 19:58:46.000000 synthegrator-0.9.3.6/README.md
+-rwxr-xr-x   0 dgros      (501) staff       (20)       16 2024-04-06 06:01:29.000000 synthegrator-0.9.3.6/build.sh
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.430761 synthegrator-0.9.3.6/examples/
+-rw-r--r--   0 dgros      (501) staff       (20)     2573 2024-03-16 23:08:47.000000 synthegrator-0.9.3.6/examples/make_results_table.py
+-rw-r--r--   0 dgros      (501) staff       (20)      795 2024-02-10 07:33:07.000000 synthegrator-0.9.3.6/examples/run_defects4j.py
+-rw-r--r--   0 dgros      (501) staff       (20)      671 2024-03-16 23:08:47.000000 synthegrator-0.9.3.6/examples/run_dypy.py
+-rw-r--r--   0 dgros      (501) staff       (20)     6042 2024-03-16 23:08:47.000000 synthegrator-0.9.3.6/examples/run_human_eval.py
+-rw-r--r--   0 dgros      (501) staff       (20)      816 2024-02-21 20:24:16.000000 synthegrator-0.9.3.6/examples/run_mbpp.py
+-rwxr-xr-x   0 dgros      (501) staff       (20)     3887 2024-04-24 20:22:45.000000 synthegrator-0.9.3.6/publish.sh
+-rw-r--r--   0 dgros      (501) staff       (20)     5200 2024-04-24 20:16:43.000000 synthegrator-0.9.3.6/pyproject.toml
+-rwxr-xr-x   0 dgros      (501) staff       (20)      516 2024-03-16 23:08:47.000000 synthegrator-0.9.3.6/run_lint.sh
+-rwxr-xr-x   0 dgros      (501) staff       (20)        6 2024-04-06 06:01:29.000000 synthegrator-0.9.3.6/run_tests.sh
+-rw-r--r--   0 dgros      (501) staff       (20)       38 2024-04-24 20:32:50.571438 synthegrator-0.9.3.6/setup.cfg
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.439831 synthegrator-0.9.3.6/synthegrator/
+-rw-r--r--   0 dgros      (501) staff       (20)    10229 2023-10-04 00:58:52.000000 synthegrator-0.9.3.6/synthegrator/JUnit.xsd
+-rw-r--r--   0 dgros      (501) staff       (20)        0 2023-06-07 15:22:13.000000 synthegrator-0.9.3.6/synthegrator/__init__.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.441808 synthegrator-0.9.3.6/synthegrator/_vendor/
+-rw-r--r--   0 dgros      (501) staff       (20)      362 2024-04-24 02:49:54.000000 synthegrator-0.9.3.6/synthegrator/_vendor/README.md
+-rw-r--r--   0 dgros      (501) staff       (20)        0 2024-04-24 02:44:40.000000 synthegrator-0.9.3.6/synthegrator/_vendor/__init__.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.443978 synthegrator-0.9.3.6/synthegrator/_vendor/epicbox/
+-rw-r--r--   0 dgros      (501) staff       (20)     1072 2024-04-24 18:48:55.000000 synthegrator-0.9.3.6/synthegrator/_vendor/epicbox/LICENSE
+-rw-r--r--   0 dgros      (501) staff       (20)     4166 2024-04-24 18:48:39.000000 synthegrator-0.9.3.6/synthegrator/_vendor/epicbox/README.md
+-rw-r--r--   0 dgros      (501) staff       (20)       70 2024-04-24 02:48:53.000000 synthegrator-0.9.3.6/synthegrator/_vendor/epicbox/__init__.py
+-rw-r--r--   0 dgros      (501) staff       (20)     2235 2024-04-24 02:48:53.000000 synthegrator-0.9.3.6/synthegrator/_vendor/epicbox/config.py
+-rw-r--r--   0 dgros      (501) staff       (20)      195 2024-04-24 02:48:53.000000 synthegrator-0.9.3.6/synthegrator/_vendor/epicbox/exceptions.py
+-rw-r--r--   0 dgros      (501) staff       (20)    13035 2024-04-24 02:48:53.000000 synthegrator-0.9.3.6/synthegrator/_vendor/epicbox/sandboxes.py
+-rw-r--r--   0 dgros      (501) staff       (20)    10163 2024-04-24 02:48:53.000000 synthegrator-0.9.3.6/synthegrator/_vendor/epicbox/utils.py
+-rw-r--r--   0 dgros      (501) staff       (20)    13611 2024-03-17 08:36:57.000000 synthegrator-0.9.3.6/synthegrator/code_problem_builders.py
+-rw-r--r--   0 dgros      (501) staff       (20)    14744 2024-03-19 03:36:50.000000 synthegrator-0.9.3.6/synthegrator/code_problems.py
+-rw-r--r--   0 dgros      (501) staff       (20)    10006 2024-03-20 20:00:19.000000 synthegrator-0.9.3.6/synthegrator/code_solver.py
+-rw-r--r--   0 dgros      (501) staff       (20)     3756 2024-03-16 23:08:47.000000 synthegrator-0.9.3.6/synthegrator/df_converters.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.445912 synthegrator-0.9.3.6/synthegrator/dypybench/
+-rw-r--r--   0 dgros      (501) staff       (20)        0 2023-08-10 05:46:51.000000 synthegrator-0.9.3.6/synthegrator/dypybench/__init__.py
+-rw-r--r--   0 dgros      (501) staff       (20)      300 2023-08-10 05:46:51.000000 synthegrator-0.9.3.6/synthegrator/dypybench/copy-project.sh
+-rw-r--r--   0 dgros      (501) staff       (20)    29263 2023-08-10 05:46:51.000000 synthegrator-0.9.3.6/synthegrator/dypybench/dypybench.py.nolint
+-rw-r--r--   0 dgros      (501) staff       (20)      879 2023-08-10 05:46:51.000000 synthegrator-0.9.3.6/synthegrator/dypybench/run-test-temp.sh
+-rw-r--r--   0 dgros      (501) staff       (20)      385 2023-09-07 07:28:11.000000 synthegrator-0.9.3.6/synthegrator/environments.py
+-rw-r--r--   0 dgros      (501) staff       (20)     6756 2024-03-16 23:08:47.000000 synthegrator-0.9.3.6/synthegrator/execution_threading.py
+-rw-r--r--   0 dgros      (501) staff       (20)     6003 2024-03-23 01:20:01.000000 synthegrator-0.9.3.6/synthegrator/few_shotting.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.447339 synthegrator-0.9.3.6/synthegrator/human_eval/
+-rw-r--r--   0 dgros      (501) staff       (20)     1083 2023-05-29 16:47:52.000000 synthegrator-0.9.3.6/synthegrator/human_eval/LICENSE
+-rw-r--r--   0 dgros      (501) staff       (20)        0 2023-06-07 15:23:22.000000 synthegrator-0.9.3.6/synthegrator/human_eval/__init__.py
+-rw-r--r--   0 dgros      (501) staff       (20)     3516 2023-08-23 21:48:00.000000 synthegrator-0.9.3.6/synthegrator/human_eval/evaluation.py
+-rw-r--r--   0 dgros      (501) staff       (20)     6721 2024-03-16 23:08:47.000000 synthegrator-0.9.3.6/synthegrator/human_eval/execution.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.449365 synthegrator-0.9.3.6/synthegrator/lang_specs/
+-rw-r--r--   0 dgros      (501) staff       (20)        0 2023-10-13 20:26:11.000000 synthegrator-0.9.3.6/synthegrator/lang_specs/__init__.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.450270 synthegrator-0.9.3.6/synthegrator/lang_specs/extra_files/
+-rw-r--r--   0 dgros      (501) staff       (20)      265 2023-10-13 20:26:11.000000 synthegrator-0.9.3.6/synthegrator/lang_specs/extra_files/DummyTest.java
+-rw-r--r--   0 dgros      (501) staff       (20)     1216 2023-10-13 20:26:11.000000 synthegrator-0.9.3.6/synthegrator/lang_specs/extra_files/default_java_pom.xml
+-rw-r--r--   0 dgros      (501) staff       (20)    11882 2024-03-23 01:20:01.000000 synthegrator-0.9.3.6/synthegrator/lang_specs/lang_spec.py
+-rw-r--r--   0 dgros      (501) staff       (20)     5385 2024-03-17 08:36:57.000000 synthegrator-0.9.3.6/synthegrator/lang_specs/lang_spec_java.py
+-rw-r--r--   0 dgros      (501) staff       (20)    10908 2024-03-16 23:08:47.000000 synthegrator-0.9.3.6/synthegrator/lang_specs/lang_spec_python.py
+-rw-r--r--   0 dgros      (501) staff       (20)     2854 2023-10-13 20:26:11.000000 synthegrator-0.9.3.6/synthegrator/lang_specs/lang_util.py
+-rw-r--r--   0 dgros      (501) staff       (20)     4118 2024-03-20 23:50:11.000000 synthegrator-0.9.3.6/synthegrator/lm_few_shotting_tools.py
+-rw-r--r--   0 dgros      (501) staff       (20)    11780 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/memory_fs.py
+-rw-r--r--   0 dgros      (501) staff       (20)    19158 2024-03-19 01:39:03.000000 synthegrator-0.9.3.6/synthegrator/problem_rendering.py
+-rw-r--r--   0 dgros      (501) staff       (20)    12086 2024-03-21 03:32:15.000000 synthegrator-0.9.3.6/synthegrator/problem_rendering_insertion_tags.py
+-rw-r--r--   0 dgros      (501) staff       (20)        0 2024-03-17 08:36:57.000000 synthegrator-0.9.3.6/synthegrator/prompt_renderer_edit.py
+-rw-r--r--   0 dgros      (501) staff       (20)    13265 2024-03-19 09:14:42.000000 synthegrator-0.9.3.6/synthegrator/prompt_renderer_questions.py
+-rw-r--r--   0 dgros      (501) staff       (20)     2046 2023-10-04 00:58:52.000000 synthegrator-0.9.3.6/synthegrator/prompting_test_case_selection.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.451082 synthegrator-0.9.3.6/synthegrator/randomstuff/
+-rw-r--r--   0 dgros      (501) staff       (20)        0 2023-06-30 22:33:24.000000 synthegrator-0.9.3.6/synthegrator/randomstuff/__init__.py
+-rw-r--r--   0 dgros      (501) staff       (20)      115 2023-08-10 05:46:51.000000 synthegrator-0.9.3.6/synthegrator/randomstuff/getk.py
+-rw-r--r--   0 dgros      (501) staff       (20)      446 2023-08-23 21:48:00.000000 synthegrator-0.9.3.6/synthegrator/randomstuff/hellolangchain.py
+-rw-r--r--   0 dgros      (501) staff       (20)     9488 2024-03-20 23:50:39.000000 synthegrator-0.9.3.6/synthegrator/response_parser.py
+-rw-r--r--   0 dgros      (501) staff       (20)    18264 2024-04-24 03:55:04.000000 synthegrator-0.9.3.6/synthegrator/sandboxing.py
+-rw-r--r--   0 dgros      (501) staff       (20)    23920 2024-04-24 02:16:05.000000 synthegrator-0.9.3.6/synthegrator/solution_eval.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.454089 synthegrator-0.9.3.6/synthegrator/synthdatasets/
+-rw-r--r--   0 dgros      (501) staff       (20)        0 2023-08-10 05:46:51.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/__init__.py
+-rw-r--r--   0 dgros      (501) staff       (20)     8168 2024-03-16 23:08:47.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/apps.py
+-rw-r--r--   0 dgros      (501) staff       (20)     9523 2024-04-24 01:30:36.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.457604 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/
+-rw-r--r--   0 dgros      (501) staff       (20)     8791 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_oneLiner_metadata.csv
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.420210 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.183845 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_1/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.183899 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_1/source/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.183953 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_1/source/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.184011 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_1/source/org/jfree/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.184065 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_1/source/org/jfree/chart/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.184117 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_1/source/org/jfree/chart/renderer/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.458001 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_1/source/org/jfree/chart/renderer/category/
+-rw-r--r--   0 dgros      (501) staff       (20)    75804 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_1/source/org/jfree/chart/renderer/category/AbstractCategoryItemRenderer.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.184272 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_10/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.184326 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_10/source/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.184379 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_10/source/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.184431 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_10/source/org/jfree/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.184486 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_10/source/org/jfree/chart/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.458847 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_10/source/org/jfree/chart/imagemap/
+-rw-r--r--   0 dgros      (501) staff       (20)     2395 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_10/source/org/jfree/chart/imagemap/StandardToolTipTagFragmentGenerator.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.184643 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_10_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.184693 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_10_fixed/source/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.184750 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_10_fixed/source/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.184805 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_10_fixed/source/org/jfree/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.184863 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_10_fixed/source/org/jfree/chart/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.459339 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_10_fixed/source/org/jfree/chart/imagemap/
+-rw-r--r--   0 dgros      (501) staff       (20)     2426 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_10_fixed/source/org/jfree/chart/imagemap/StandardToolTipTagFragmentGenerator.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.185013 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_11/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.185066 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_11/source/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.185117 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_11/source/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.185169 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_11/source/org/jfree/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.185219 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_11/source/org/jfree/chart/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.459661 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_11/source/org/jfree/chart/util/
+-rw-r--r--   0 dgros      (501) staff       (20)    19851 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_11/source/org/jfree/chart/util/ShapeUtilities.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.185367 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_11_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.185425 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_11_fixed/source/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.185479 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_11_fixed/source/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.185531 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_11_fixed/source/org/jfree/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.185584 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_11_fixed/source/org/jfree/chart/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.460024 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_11_fixed/source/org/jfree/chart/util/
+-rw-r--r--   0 dgros      (501) staff       (20)    19851 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_11_fixed/source/org/jfree/chart/util/ShapeUtilities.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.185733 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_12/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.185785 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_12/source/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.185840 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_12/source/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.185894 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_12/source/org/jfree/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.185951 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_12/source/org/jfree/chart/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.460404 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_12/source/org/jfree/chart/plot/
+-rw-r--r--   0 dgros      (501) staff       (20)    21421 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_12/source/org/jfree/chart/plot/MultiplePiePlot.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.186099 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_12_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.186151 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_12_fixed/source/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.186204 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_12_fixed/source/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.186257 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_12_fixed/source/org/jfree/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.186308 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_12_fixed/source/org/jfree/chart/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.460742 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_12_fixed/source/org/jfree/chart/plot/
+-rw-r--r--   0 dgros      (501) staff       (20)    21418 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_12_fixed/source/org/jfree/chart/plot/MultiplePiePlot.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.186460 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_13/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.186511 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_13/source/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.186565 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_13/source/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.186618 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_13/source/org/jfree/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.186671 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_13/source/org/jfree/chart/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.461076 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_13/source/org/jfree/chart/block/
+-rw-r--r--   0 dgros      (501) staff       (20)    20547 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_13/source/org/jfree/chart/block/BorderArrangement.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.186816 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_13_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.186869 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_13_fixed/source/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.186924 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_13_fixed/source/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.186977 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_13_fixed/source/org/jfree/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.187031 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_13_fixed/source/org/jfree/chart/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.461512 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_13_fixed/source/org/jfree/chart/block/
+-rw-r--r--   0 dgros      (501) staff       (20)    20562 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_13_fixed/source/org/jfree/chart/block/BorderArrangement.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.187190 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_1_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.187242 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_1_fixed/source/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.187296 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_1_fixed/source/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.187349 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_1_fixed/source/org/jfree/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.187403 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_1_fixed/source/org/jfree/chart/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.187458 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_1_fixed/source/org/jfree/chart/renderer/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.461904 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_1_fixed/source/org/jfree/chart/renderer/category/
+-rw-r--r--   0 dgros      (501) staff       (20)    75804 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_1_fixed/source/org/jfree/chart/renderer/category/AbstractCategoryItemRenderer.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.187608 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_20/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.187662 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_20/source/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.187715 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_20/source/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.187768 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_20/source/org/jfree/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.187823 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_20/source/org/jfree/chart/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.462279 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_20/source/org/jfree/chart/plot/
+-rw-r--r--   0 dgros      (501) staff       (20)     4977 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_20/source/org/jfree/chart/plot/ValueMarker.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.187972 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_20_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.188027 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_20_fixed/source/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.188080 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_20_fixed/source/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.188133 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_20_fixed/source/org/jfree/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.188186 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_20_fixed/source/org/jfree/chart/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.462560 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_20_fixed/source/org/jfree/chart/plot/
+-rw-r--r--   0 dgros      (501) staff       (20)     4991 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_20_fixed/source/org/jfree/chart/plot/ValueMarker.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.188340 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_24/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.188399 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_24/source/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.188461 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_24/source/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.188524 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_24/source/org/jfree/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.188599 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_24/source/org/jfree/chart/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.462889 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_24/source/org/jfree/chart/renderer/
+-rw-r--r--   0 dgros      (501) staff       (20)     5343 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_24/source/org/jfree/chart/renderer/GrayPaintScale.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.188760 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_24_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.188813 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_24_fixed/source/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.188874 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_24_fixed/source/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.188938 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_24_fixed/source/org/jfree/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.188994 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_24_fixed/source/org/jfree/chart/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.463173 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_24_fixed/source/org/jfree/chart/renderer/
+-rw-r--r--   0 dgros      (501) staff       (20)     5339 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_24_fixed/source/org/jfree/chart/renderer/GrayPaintScale.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.189170 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_8/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.189240 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_8/source/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.189404 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_8/source/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.189497 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_8/source/org/jfree/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.189568 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_8/source/org/jfree/data/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.463426 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_8/source/org/jfree/data/time/
+-rw-r--r--   0 dgros      (501) staff       (20)    21920 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_8/source/org/jfree/data/time/Week.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.189769 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_8_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.189839 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_8_fixed/source/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.189898 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_8_fixed/source/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.189971 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_8_fixed/source/org/jfree/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.190031 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_8_fixed/source/org/jfree/data/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.463766 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_8_fixed/source/org/jfree/data/time/
+-rw-r--r--   0 dgros      (501) staff       (20)    21889 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_8_fixed/source/org/jfree/data/time/Week.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.190224 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_9/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.190282 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_9/source/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.190366 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_9/source/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.190425 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_9/source/org/jfree/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.190486 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_9/source/org/jfree/data/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.464106 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_9/source/org/jfree/data/time/
+-rw-r--r--   0 dgros      (501) staff       (20)    37353 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_9/source/org/jfree/data/time/TimeSeries.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.190649 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_9_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.190707 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_9_fixed/source/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.190763 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_9_fixed/source/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.190819 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_9_fixed/source/org/jfree/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.190874 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_9_fixed/source/org/jfree/data/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.464434 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_9_fixed/source/org/jfree/data/time/
+-rw-r--r--   0 dgros      (501) staff       (20)    37383 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Chart_9_fixed/source/org/jfree/data/time/TimeSeries.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.191034 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_11/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.191094 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_11/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.191151 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_11/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.191210 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_11/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.191264 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_11/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.191323 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_11/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.464779 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_11/src/java/org/apache/commons/cli/
+-rw-r--r--   0 dgros      (501) staff       (20)    30418 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_11/src/java/org/apache/commons/cli/HelpFormatter.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.191486 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_11_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.191542 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_11_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.191603 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_11_fixed/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.191662 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_11_fixed/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.191721 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_11_fixed/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.191776 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_11_fixed/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.465071 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_11_fixed/src/java/org/apache/commons/cli/
+-rw-r--r--   0 dgros      (501) staff       (20)    30408 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_11_fixed/src/java/org/apache/commons/cli/HelpFormatter.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.191933 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_25/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.191995 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_25/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.192050 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_25/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.192109 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_25/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.192172 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_25/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.192251 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_25/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.465413 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_25/src/java/org/apache/commons/cli/
+-rw-r--r--   0 dgros      (501) staff       (20)    29998 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_25/src/java/org/apache/commons/cli/HelpFormatter.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.192449 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_25_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.192518 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_25_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.192579 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_25_fixed/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.192636 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_25_fixed/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.192702 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_25_fixed/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.192772 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_25_fixed/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.465875 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_25_fixed/src/java/org/apache/commons/cli/
+-rw-r--r--   0 dgros      (501) staff       (20)    29990 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_25_fixed/src/java/org/apache/commons/cli/HelpFormatter.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.192932 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_28/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.192988 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_28/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.193043 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_28/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.193101 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_28/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.193154 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_28/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.193210 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_28/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.466311 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_28/src/java/org/apache/commons/cli/
+-rw-r--r--   0 dgros      (501) staff       (20)    13034 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_28/src/java/org/apache/commons/cli/Parser.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.193371 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_28_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.193425 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_28_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.193481 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_28_fixed/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.193539 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_28_fixed/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.193594 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_28_fixed/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.193648 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_28_fixed/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.466642 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_28_fixed/src/java/org/apache/commons/cli/
+-rw-r--r--   0 dgros      (501) staff       (20)    13037 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_28_fixed/src/java/org/apache/commons/cli/Parser.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.193798 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_40/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.193853 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_40/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.193906 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_40/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.193957 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_40/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.194013 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_40/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.194069 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_40/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.194123 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_40/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.466965 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_40/src/main/java/org/apache/commons/cli/
+-rw-r--r--   0 dgros      (501) staff       (20)     8135 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_40/src/main/java/org/apache/commons/cli/TypeHandler.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.194279 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_40_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.194332 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_40_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.194384 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_40_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.194438 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_40_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.194490 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_40_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.194544 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_40_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.194599 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_40_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.467297 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_40_fixed/src/main/java/org/apache/commons/cli/
+-rw-r--r--   0 dgros      (501) staff       (20)     8188 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_40_fixed/src/main/java/org/apache/commons/cli/TypeHandler.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.194770 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_8/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.194824 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_8/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.194878 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_8/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.194932 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_8/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.194985 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_8/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.195044 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_8/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.467601 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_8/src/java/org/apache/commons/cli/
+-rw-r--r--   0 dgros      (501) staff       (20)    29486 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_8/src/java/org/apache/commons/cli/HelpFormatter.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.195222 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_8_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.195290 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_8_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.195346 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_8_fixed/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.195401 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_8_fixed/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.195456 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_8_fixed/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.195512 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_8_fixed/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.467973 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_8_fixed/src/java/org/apache/commons/cli/
+-rw-r--r--   0 dgros      (501) staff       (20)    29472 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Cli_8_fixed/src/java/org/apache/commons/cli/HelpFormatter.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.195699 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_10/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.195760 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_10/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.195819 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_10/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.195890 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_10/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.195947 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_10/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.468352 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_10/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    95395 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_10/src/com/google/javascript/jscomp/NodeUtil.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.196103 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_104/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.196170 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_104/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.196238 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_104/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.196311 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_104/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.196373 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_104/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.196433 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_104/src/com/google/javascript/rhino/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.468793 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_104/src/com/google/javascript/rhino/jstype/
+-rw-r--r--   0 dgros      (501) staff       (20)    14307 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_104/src/com/google/javascript/rhino/jstype/UnionType.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.196600 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_104_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.196661 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_104_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.196715 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_104_fixed/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.196771 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_104_fixed/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.196833 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_104_fixed/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.196899 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_104_fixed/src/com/google/javascript/rhino/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.469114 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_104_fixed/src/com/google/javascript/rhino/jstype/
+-rw-r--r--   0 dgros      (501) staff       (20)    14311 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_104_fixed/src/com/google/javascript/rhino/jstype/UnionType.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.197109 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_10_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.197171 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_10_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.197228 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_10_fixed/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.197291 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_10_fixed/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.197354 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_10_fixed/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.469427 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_10_fixed/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    95395 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_10_fixed/src/com/google/javascript/jscomp/NodeUtil.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.197525 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_113/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.197579 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_113/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.197636 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_113/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.197693 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_113/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.197759 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_113/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.469846 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_113/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    41804 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_113/src/com/google/javascript/jscomp/ProcessClosurePrimitives.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.197940 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_113_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.198012 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_113_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.198089 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_113_fixed/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.198200 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_113_fixed/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.198326 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_113_fixed/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.470196 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_113_fixed/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    41828 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_113_fixed/src/com/google/javascript/jscomp/ProcessClosurePrimitives.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.198686 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_114/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.198801 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_114/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.198889 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_114/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.198974 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_114/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.199070 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_114/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.470590 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_114/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    62192 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_114/src/com/google/javascript/jscomp/NameAnalyzer.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.199348 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_114_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.199428 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_114_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.199511 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_114_fixed/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.199602 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_114_fixed/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.199686 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_114_fixed/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.471182 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_114_fixed/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    62247 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_114_fixed/src/com/google/javascript/jscomp/NameAnalyzer.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.200038 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_123/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.200142 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_123/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.200247 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_123/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.200348 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_123/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.200442 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_123/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.471564 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_123/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    39978 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_123/src/com/google/javascript/jscomp/CodeGenerator.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.200773 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_123_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.200860 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_123_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.200943 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_123_fixed/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.201035 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_123_fixed/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.201131 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_123_fixed/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.471884 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_123_fixed/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    39999 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_123_fixed/src/com/google/javascript/jscomp/CodeGenerator.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.201398 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_125/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.201501 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_125/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.201667 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_125/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.201755 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_125/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.201845 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_125/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.472244 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_125/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    74509 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_125/src/com/google/javascript/jscomp/TypeCheck.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.202183 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_125_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.202260 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_125_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.202352 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_125_fixed/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.202454 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_125_fixed/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.202547 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_125_fixed/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.472669 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_125_fixed/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    74537 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_125_fixed/src/com/google/javascript/jscomp/TypeCheck.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.202791 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_130/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.202870 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_130/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.202949 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_130/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.203029 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_130/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.203101 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_130/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.473246 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_130/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    34685 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_130/src/com/google/javascript/jscomp/CollapseProperties.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.203272 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_130_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.203357 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_130_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.203438 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_130_fixed/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.203518 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_130_fixed/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.203609 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_130_fixed/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.473629 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_130_fixed/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    34704 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_130_fixed/src/com/google/javascript/jscomp/CollapseProperties.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.203971 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_14/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.204070 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_14/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.204156 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_14/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.204247 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_14/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.204338 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_14/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.474385 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_14/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    35019 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_14/src/com/google/javascript/jscomp/ControlFlowAnalysis.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.204608 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_14_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.204712 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_14_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.204856 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_14_fixed/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.204978 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_14_fixed/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.205064 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_14_fixed/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.474740 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_14_fixed/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    35018 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_14_fixed/src/com/google/javascript/jscomp/ControlFlowAnalysis.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.205338 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_18/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.205439 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_18/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.205533 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_18/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.205621 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_18/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.205704 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_18/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.475097 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_18/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    75213 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_18/src/com/google/javascript/jscomp/Compiler.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.206030 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_18_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.206104 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_18_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.206165 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_18_fixed/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.206300 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_18_fixed/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.206444 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_18_fixed/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.475487 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_18_fixed/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    75190 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_18_fixed/src/com/google/javascript/jscomp/Compiler.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.206706 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_38/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.206795 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_38/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.206885 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_38/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.206958 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_38/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.207021 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_38/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.475888 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_38/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)     7059 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_38/src/com/google/javascript/jscomp/CodeConsumer.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.207211 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_38_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.207266 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_38_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.207387 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_38_fixed/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.207497 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_38_fixed/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.207587 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_38_fixed/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.476154 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_38_fixed/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)     7077 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_38_fixed/src/com/google/javascript/jscomp/CodeConsumer.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.207935 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_51/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.208021 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_51/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.208082 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_51/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.208149 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_51/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.208233 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_51/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.476464 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_51/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)     6658 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_51/src/com/google/javascript/jscomp/CodeConsumer.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.208495 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_51_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.208576 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_51_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.208652 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_51_fixed/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.208733 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_51_fixed/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.208881 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_51_fixed/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.476746 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_51_fixed/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)     6780 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_51_fixed/src/com/google/javascript/jscomp/CodeConsumer.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.209087 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_52/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.209148 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_52/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.209206 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_52/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.209275 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_52/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.209367 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_52/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.476954 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_52/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    37654 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_52/src/com/google/javascript/jscomp/CodeGenerator.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.209622 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_52_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.209714 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_52_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.209798 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_52_fixed/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.209878 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_52_fixed/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.209959 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_52_fixed/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.477209 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_52_fixed/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    37676 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_52_fixed/src/com/google/javascript/jscomp/CodeGenerator.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.210235 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_57/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.210327 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_57/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.210453 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_57/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.210549 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_57/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.210667 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_57/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.477545 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_57/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    12726 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_57/src/com/google/javascript/jscomp/ClosureCodingConvention.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.210897 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_57_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.211012 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_57_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.211113 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_57_fixed/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.211222 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_57_fixed/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.211338 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_57_fixed/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.477762 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_57_fixed/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    12762 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_57_fixed/src/com/google/javascript/jscomp/ClosureCodingConvention.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.211680 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_62/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.211800 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_62/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.211871 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_62/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.211932 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_62/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.211991 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_62/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.477983 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_62/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)     5282 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_62/src/com/google/javascript/jscomp/LightweightMessageFormatter.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.212231 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_62_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.212322 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_62_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.212416 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_62_fixed/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.212509 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_62_fixed/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.212592 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_62_fixed/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.478214 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_62_fixed/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)     5283 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_62_fixed/src/com/google/javascript/jscomp/LightweightMessageFormatter.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.212813 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_65/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.212896 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_65/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.212988 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_65/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.213084 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_65/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.213244 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_65/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.478483 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_65/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    37652 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_65/src/com/google/javascript/jscomp/CodeGenerator.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.213560 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_65_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.213657 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_65_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.213766 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_65_fixed/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.213861 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_65_fixed/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.213958 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_65_fixed/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.478808 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_65_fixed/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    37654 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_65_fixed/src/com/google/javascript/jscomp/CodeGenerator.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.214234 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_67/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.214370 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_67/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.214471 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_67/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.214588 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_67/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.214682 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_67/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.479130 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_67/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    22383 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_67/src/com/google/javascript/jscomp/AnalyzePrototypeProperties.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.215096 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_67_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.215223 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_67_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.215353 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_67_fixed/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.215459 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_67_fixed/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.215626 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_67_fixed/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.479489 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_67_fixed/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    22435 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_67_fixed/src/com/google/javascript/jscomp/AnalyzePrototypeProperties.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.215939 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_70/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.216059 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_70/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.216174 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_70/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.216311 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_70/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.216417 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_70/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.479974 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_70/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    67134 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_70/src/com/google/javascript/jscomp/TypedScopeCreator.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.216877 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_70_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.216971 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_70_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.217059 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_70_fixed/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.217147 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_70_fixed/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.217238 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_70_fixed/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.480321 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_70_fixed/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    67135 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_70_fixed/src/com/google/javascript/jscomp/TypedScopeCreator.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.217524 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_71/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.217628 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_71/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.217722 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_71/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.217813 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_71/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.217895 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_71/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.480743 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_71/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    22255 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_71/src/com/google/javascript/jscomp/CheckAccessControls.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.218147 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_71_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.218231 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_71_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.218333 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_71_fixed/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.218434 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_71_fixed/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.218523 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_71_fixed/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.481071 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_71_fixed/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    22267 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_71_fixed/src/com/google/javascript/jscomp/CheckAccessControls.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.218849 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_73/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.218945 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_73/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.219024 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_73/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.219100 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_73/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.219190 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_73/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.481418 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_73/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    37217 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_73/src/com/google/javascript/jscomp/CodeGenerator.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.219432 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_73_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.219512 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_73_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.219594 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_73_fixed/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.219670 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_73_fixed/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.219740 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_73_fixed/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.481767 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_73_fixed/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    37216 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_73_fixed/src/com/google/javascript/jscomp/CodeGenerator.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.219924 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_86/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.219987 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_86/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.220051 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_86/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.220121 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_86/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.220209 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_86/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.482210 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_86/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    75861 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_86/src/com/google/javascript/jscomp/NodeUtil.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.220550 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_86_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.220687 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_86_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.220808 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_86_fixed/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.220932 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_86_fixed/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.221046 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_86_fixed/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.482670 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_86_fixed/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    75862 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_86_fixed/src/com/google/javascript/jscomp/NodeUtil.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.221393 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_92/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.221517 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_92/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.221615 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_92/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.224854 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_92/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.224998 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_92/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.483085 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_92/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    32465 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_92/src/com/google/javascript/jscomp/ProcessClosurePrimitives.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.225331 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_92_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.225451 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_92_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.225563 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_92_fixed/src/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.225681 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_92_fixed/src/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.226939 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_92_fixed/src/com/google/javascript/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.483407 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_92_fixed/src/com/google/javascript/jscomp/
+-rw-r--r--   0 dgros      (501) staff       (20)    32469 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Closure_92_fixed/src/com/google/javascript/jscomp/ProcessClosurePrimitives.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.227276 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_1/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.227373 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_1/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.227460 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_1/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.227526 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_1/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.227595 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_1/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.227661 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_1/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.227728 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_1/src/java/org/apache/commons/codec/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.483745 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_1/src/java/org/apache/commons/codec/language/
+-rw-r--r--   0 dgros      (501) staff       (20)     7223 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_1/src/java/org/apache/commons/codec/language/Caverphone.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.227908 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_10/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.227969 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_10/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.228053 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_10/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.228140 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_10/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.228214 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_10/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.228298 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_10/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.232452 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_10/src/java/org/apache/commons/codec/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.484114 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_10/src/java/org/apache/commons/codec/language/
+-rw-r--r--   0 dgros      (501) staff       (20)     7248 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_10/src/java/org/apache/commons/codec/language/Caverphone.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.233365 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_10_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.233465 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_10_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.233533 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_10_fixed/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.233600 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_10_fixed/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.233669 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_10_fixed/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.233888 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_10_fixed/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.233985 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_10_fixed/src/java/org/apache/commons/codec/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.484493 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_10_fixed/src/java/org/apache/commons/codec/language/
+-rw-r--r--   0 dgros      (501) staff       (20)     7248 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_10_fixed/src/java/org/apache/commons/codec/language/Caverphone.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.234225 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_16/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.234293 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_16/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.234359 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_16/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.234427 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_16/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.234493 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_16/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.234561 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_16/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.234628 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_16/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.234696 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_16/src/main/java/org/apache/commons/codec/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.484767 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_16/src/main/java/org/apache/commons/codec/binary/
+-rw-r--r--   0 dgros      (501) staff       (20)    26050 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_16/src/main/java/org/apache/commons/codec/binary/Base32.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.234884 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_16_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.234953 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_16_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.235022 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_16_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.235165 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_16_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.235264 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_16_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.235342 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_16_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.235414 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_16_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.235486 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_16_fixed/src/main/java/org/apache/commons/codec/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.485089 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_16_fixed/src/main/java/org/apache/commons/codec/binary/
+-rw-r--r--   0 dgros      (501) staff       (20)    26095 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_16_fixed/src/main/java/org/apache/commons/codec/binary/Base32.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.235695 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_1_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.235759 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_1_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.235823 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_1_fixed/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.236050 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_1_fixed/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.236153 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_1_fixed/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.236222 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_1_fixed/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.236291 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_1_fixed/src/java/org/apache/commons/codec/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.485470 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_1_fixed/src/java/org/apache/commons/codec/language/
+-rw-r--r--   0 dgros      (501) staff       (20)     7247 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_1_fixed/src/java/org/apache/commons/codec/language/Caverphone.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.236526 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_2/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.236608 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_2/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.236686 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_2/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.236755 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_2/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.236845 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_2/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.236936 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_2/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.237040 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_2/src/java/org/apache/commons/codec/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.485784 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_2/src/java/org/apache/commons/codec/binary/
+-rw-r--r--   0 dgros      (501) staff       (20)    34587 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_2/src/java/org/apache/commons/codec/binary/Base64.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.237314 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_2_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.237411 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_2_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.237508 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_2_fixed/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.237604 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_2_fixed/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.237706 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_2_fixed/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.237850 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_2_fixed/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.237930 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_2_fixed/src/java/org/apache/commons/codec/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.486111 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_2_fixed/src/java/org/apache/commons/codec/binary/
+-rw-r--r--   0 dgros      (501) staff       (20)    34598 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_2_fixed/src/java/org/apache/commons/codec/binary/Base64.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.238167 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_3/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.238242 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_3/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.238319 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_3/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.238404 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_3/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.238479 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_3/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.238559 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_3/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.238640 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_3/src/java/org/apache/commons/codec/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.486466 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_3/src/java/org/apache/commons/codec/language/
+-rw-r--r--   0 dgros      (501) staff       (20)    38942 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_3/src/java/org/apache/commons/codec/language/DoubleMetaphone.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.238895 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_3_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.238974 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_3_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.239062 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_3_fixed/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.239155 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_3_fixed/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.239243 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_3_fixed/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.239349 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_3_fixed/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.239443 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_3_fixed/src/java/org/apache/commons/codec/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.486819 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_3_fixed/src/java/org/apache/commons/codec/language/
+-rw-r--r--   0 dgros      (501) staff       (20)    38942 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_3_fixed/src/java/org/apache/commons/codec/language/DoubleMetaphone.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.239637 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_4/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.239691 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_4/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.239752 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_4/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.239821 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_4/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.239904 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_4/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.239996 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_4/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.240101 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_4/src/java/org/apache/commons/codec/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.487139 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_4/src/java/org/apache/commons/codec/binary/
+-rw-r--r--   0 dgros      (501) staff       (20)    40640 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_4/src/java/org/apache/commons/codec/binary/Base64.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.240507 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_4_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.240657 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_4_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.240773 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_4_fixed/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.240867 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_4_fixed/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.240960 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_4_fixed/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.241050 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_4_fixed/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.241149 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_4_fixed/src/java/org/apache/commons/codec/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.487508 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_4_fixed/src/java/org/apache/commons/codec/binary/
+-rw-r--r--   0 dgros      (501) staff       (20)    40636 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_4_fixed/src/java/org/apache/commons/codec/binary/Base64.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.241555 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_9/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.241807 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_9/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.241929 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_9/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.242035 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_9/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.242125 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_9/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.242209 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_9/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.242296 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_9/src/java/org/apache/commons/codec/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.487840 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_9/src/java/org/apache/commons/codec/binary/
+-rw-r--r--   0 dgros      (501) staff       (20)    40879 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_9/src/java/org/apache/commons/codec/binary/Base64.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.242572 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_9_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.242770 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_9_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.242887 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_9_fixed/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.243002 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_9_fixed/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.243105 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_9_fixed/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.243211 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_9_fixed/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.243329 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_9_fixed/src/java/org/apache/commons/codec/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.488175 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_9_fixed/src/java/org/apache/commons/codec/binary/
+-rw-r--r--   0 dgros      (501) staff       (20)    40895 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Codec_9_fixed/src/java/org/apache/commons/codec/binary/Base64.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.243867 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_19/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.243958 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_19/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.244184 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_19/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.244316 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_19/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.244436 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_19/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.244551 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_19/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.244670 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_19/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.244780 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_19/src/main/java/org/apache/commons/compress/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.244880 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_19/src/main/java/org/apache/commons/compress/archivers/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.488543 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_19/src/main/java/org/apache/commons/compress/archivers/zip/
+-rw-r--r--   0 dgros      (501) staff       (20)    13305 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_19/src/main/java/org/apache/commons/compress/archivers/zip/Zip64ExtendedInformationExtraField.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.245200 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_19_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.245305 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_19_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.245407 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_19_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.245522 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_19_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.245630 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_19_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.245747 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_19_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.245880 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_19_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.245997 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_19_fixed/src/main/java/org/apache/commons/compress/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.246125 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_19_fixed/src/main/java/org/apache/commons/compress/archivers/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.488837 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_19_fixed/src/main/java/org/apache/commons/compress/archivers/zip/
+-rw-r--r--   0 dgros      (501) staff       (20)    13304 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_19_fixed/src/main/java/org/apache/commons/compress/archivers/zip/Zip64ExtendedInformationExtraField.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.246557 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_23/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.246652 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_23/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.246742 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_23/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.246841 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_23/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.246933 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_23/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.247022 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_23/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.247099 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_23/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.247172 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_23/src/main/java/org/apache/commons/compress/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.247249 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_23/src/main/java/org/apache/commons/compress/archivers/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.489162 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_23/src/main/java/org/apache/commons/compress/archivers/sevenz/
+-rw-r--r--   0 dgros      (501) staff       (20)    11836 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_23/src/main/java/org/apache/commons/compress/archivers/sevenz/Coders.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.247541 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_23_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.247635 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_23_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.247708 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_23_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.247800 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_23_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.247889 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_23_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.247965 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_23_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.248039 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_23_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.248110 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_23_fixed/src/main/java/org/apache/commons/compress/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.249679 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_23_fixed/src/main/java/org/apache/commons/compress/archivers/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.489460 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_23_fixed/src/main/java/org/apache/commons/compress/archivers/sevenz/
+-rw-r--r--   0 dgros      (501) staff       (20)    11844 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_23_fixed/src/main/java/org/apache/commons/compress/archivers/sevenz/Coders.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.250039 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_38/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.250122 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_38/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.250211 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_38/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.250293 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_38/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.250501 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_38/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.250653 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_38/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.250762 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_38/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.250863 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_38/src/main/java/org/apache/commons/compress/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.250964 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_38/src/main/java/org/apache/commons/compress/archivers/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.489743 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_38/src/main/java/org/apache/commons/compress/archivers/tar/
+-rw-r--r--   0 dgros      (501) staff       (20)    38572 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_38/src/main/java/org/apache/commons/compress/archivers/tar/TarArchiveEntry.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.251320 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_38_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.251411 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_38_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.251499 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_38_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.251916 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_38_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.252018 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_38_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.252113 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_38_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.252215 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_38_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.252323 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_38_fixed/src/main/java/org/apache/commons/compress/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.252413 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_38_fixed/src/main/java/org/apache/commons/compress/archivers/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.490116 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_38_fixed/src/main/java/org/apache/commons/compress/archivers/tar/
+-rw-r--r--   0 dgros      (501) staff       (20)    38614 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Compress_38_fixed/src/main/java/org/apache/commons/compress/archivers/tar/TarArchiveEntry.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.252707 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_11/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.252820 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_11/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.253078 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_11/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.253201 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_11/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.253331 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_11/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.253444 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_11/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.253556 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_11/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.490508 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_11/src/main/java/org/apache/commons/csv/
+-rw-r--r--   0 dgros      (501) staff       (20)    17891 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_11/src/main/java/org/apache/commons/csv/CSVParser.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.253925 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_11_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.254028 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_11_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.254209 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_11_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.254291 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_11_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.254366 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_11_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.254436 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_11_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.254505 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_11_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.490894 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_11_fixed/src/main/java/org/apache/commons/csv/
+-rw-r--r--   0 dgros      (501) staff       (20)    17909 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_11_fixed/src/main/java/org/apache/commons/csv/CSVParser.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.254720 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_12/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.254786 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_12/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.254856 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_12/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.254923 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_12/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.254990 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_12/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.255059 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_12/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.255136 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_12/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.491207 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_12/src/main/java/org/apache/commons/csv/
+-rw-r--r--   0 dgros      (501) staff       (20)    36794 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_12/src/main/java/org/apache/commons/csv/CSVFormat.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.255419 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_12_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.255517 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_12_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.255602 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_12_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.255790 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_12_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.255913 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_12_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.256226 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_12_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.256335 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_12_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.491668 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_12_fixed/src/main/java/org/apache/commons/csv/
+-rw-r--r--   0 dgros      (501) staff       (20)    36828 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_12_fixed/src/main/java/org/apache/commons/csv/CSVFormat.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.256655 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_14/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.256743 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_14/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.256837 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_14/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.256946 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_14/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.257067 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_14/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.257319 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_14/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.257425 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_14/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.492054 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_14/src/main/java/org/apache/commons/csv/
+-rw-r--r--   0 dgros      (501) staff       (20)    65392 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_14/src/main/java/org/apache/commons/csv/CSVFormat.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.257736 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_14_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.257856 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_14_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.257953 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_14_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.258049 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_14_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.258244 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_14_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.258436 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_14_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.258542 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_14_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.492422 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_14_fixed/src/main/java/org/apache/commons/csv/
+-rw-r--r--   0 dgros      (501) staff       (20)    65398 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_14_fixed/src/main/java/org/apache/commons/csv/CSVFormat.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.258881 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_4/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.258969 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_4/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.259068 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_4/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.259160 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_4/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.259249 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_4/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.259468 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_4/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.259564 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_4/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.492793 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_4/src/main/java/org/apache/commons/csv/
+-rw-r--r--   0 dgros      (501) staff       (20)    15734 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_4/src/main/java/org/apache/commons/csv/CSVParser.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.259864 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_4_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.259931 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_4_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.260002 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_4_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.260073 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_4_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.260142 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_4_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.260224 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_4_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.260317 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_4_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.493058 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_4_fixed/src/main/java/org/apache/commons/csv/
+-rw-r--r--   0 dgros      (501) staff       (20)    15766 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Csv_4_fixed/src/main/java/org/apache/commons/csv/CSVParser.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.260608 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Gson_13/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.260709 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Gson_13/gson/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.260785 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Gson_13/gson/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.260862 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Gson_13/gson/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.260927 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Gson_13/gson/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.261001 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Gson_13/gson/src/main/java/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.261094 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Gson_13/gson/src/main/java/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.261184 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Gson_13/gson/src/main/java/com/google/gson/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.493335 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Gson_13/gson/src/main/java/com/google/gson/stream/
+-rw-r--r--   0 dgros      (501) staff       (20)    50392 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Gson_13/gson/src/main/java/com/google/gson/stream/JsonReader.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.261528 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Gson_13_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.261635 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Gson_13_fixed/gson/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.261740 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Gson_13_fixed/gson/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.261850 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Gson_13_fixed/gson/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.261963 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Gson_13_fixed/gson/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.262070 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Gson_13_fixed/gson/src/main/java/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.262178 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Gson_13_fixed/gson/src/main/java/com/google/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.262285 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Gson_13_fixed/gson/src/main/java/com/google/gson/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.493685 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Gson_13_fixed/gson/src/main/java/com/google/gson/stream/
+-rw-r--r--   0 dgros      (501) staff       (20)    50425 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Gson_13_fixed/gson/src/main/java/com/google/gson/stream/JsonReader.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.262635 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_14/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.262754 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_14/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.262860 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_14/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.262965 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_14/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.263085 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_14/src/main/java/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.263203 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_14/src/main/java/com/fasterxml/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.263321 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_14/src/main/java/com/fasterxml/jackson/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.263434 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_14/src/main/java/com/fasterxml/jackson/core/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.494044 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_14/src/main/java/com/fasterxml/jackson/core/io/
+-rw-r--r--   0 dgros      (501) staff       (20)     9688 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_14/src/main/java/com/fasterxml/jackson/core/io/IOContext.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.263809 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_14_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.263892 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_14_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.263977 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_14_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.264066 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_14_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.264164 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_14_fixed/src/main/java/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.264257 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_14_fixed/src/main/java/com/fasterxml/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.264353 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_14_fixed/src/main/java/com/fasterxml/jackson/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.264454 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_14_fixed/src/main/java/com/fasterxml/jackson/core/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.494327 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_14_fixed/src/main/java/com/fasterxml/jackson/core/io/
+-rw-r--r--   0 dgros      (501) staff       (20)     9690 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_14_fixed/src/main/java/com/fasterxml/jackson/core/io/IOContext.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.264736 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_5/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.264824 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_5/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.264905 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_5/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.264986 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_5/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.265066 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_5/src/main/java/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.265148 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_5/src/main/java/com/fasterxml/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.265311 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_5/src/main/java/com/fasterxml/jackson/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.494618 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_5/src/main/java/com/fasterxml/jackson/core/
+-rw-r--r--   0 dgros      (501) staff       (20)     8669 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_5/src/main/java/com/fasterxml/jackson/core/JsonPointer.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.265623 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_5_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.265720 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_5_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.265819 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_5_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.265922 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_5_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.266018 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_5_fixed/src/main/java/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.266116 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_5_fixed/src/main/java/com/fasterxml/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.266218 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_5_fixed/src/main/java/com/fasterxml/jackson/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.494917 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_5_fixed/src/main/java/com/fasterxml/jackson/core/
+-rw-r--r--   0 dgros      (501) staff       (20)     8667 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_5_fixed/src/main/java/com/fasterxml/jackson/core/JsonPointer.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.266507 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_8/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.266611 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_8/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.266699 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_8/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.266787 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_8/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.266881 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_8/src/main/java/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.266969 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_8/src/main/java/com/fasterxml/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.267064 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_8/src/main/java/com/fasterxml/jackson/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.267160 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_8/src/main/java/com/fasterxml/jackson/core/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.495183 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_8/src/main/java/com/fasterxml/jackson/core/util/
+-rw-r--r--   0 dgros      (501) staff       (20)    23081 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_8/src/main/java/com/fasterxml/jackson/core/util/TextBuffer.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.267451 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_8_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.267540 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_8_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.267633 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_8_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.267726 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_8_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.267816 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_8_fixed/src/main/java/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.267912 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_8_fixed/src/main/java/com/fasterxml/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.267998 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_8_fixed/src/main/java/com/fasterxml/jackson/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.268091 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_8_fixed/src/main/java/com/fasterxml/jackson/core/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.495508 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_8_fixed/src/main/java/com/fasterxml/jackson/core/util/
+-rw-r--r--   0 dgros      (501) staff       (20)    23108 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonCore_8_fixed/src/main/java/com/fasterxml/jackson/core/util/TextBuffer.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.268911 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_107/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.269012 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_107/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.269089 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_107/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.269157 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_107/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.269458 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_107/src/main/java/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.269574 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_107/src/main/java/com/fasterxml/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.269671 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_107/src/main/java/com/fasterxml/jackson/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.269768 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_107/src/main/java/com/fasterxml/jackson/databind/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.269866 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_107/src/main/java/com/fasterxml/jackson/databind/jsontype/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.495845 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_107/src/main/java/com/fasterxml/jackson/databind/jsontype/impl/
+-rw-r--r--   0 dgros      (501) staff       (20)    11833 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_107/src/main/java/com/fasterxml/jackson/databind/jsontype/impl/TypeDeserializerBase.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.270192 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_107_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.270280 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_107_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.270378 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_107_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.270457 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_107_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.270555 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_107_fixed/src/main/java/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.270651 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_107_fixed/src/main/java/com/fasterxml/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.270738 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_107_fixed/src/main/java/com/fasterxml/jackson/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.270840 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_107_fixed/src/main/java/com/fasterxml/jackson/databind/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.270933 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_107_fixed/src/main/java/com/fasterxml/jackson/databind/jsontype/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.496128 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_107_fixed/src/main/java/com/fasterxml/jackson/databind/jsontype/impl/
+-rw-r--r--   0 dgros      (501) staff       (20)    11860 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_107_fixed/src/main/java/com/fasterxml/jackson/databind/jsontype/impl/TypeDeserializerBase.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.271213 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_16/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.271302 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_16/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.271393 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_16/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.271518 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_16/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.271651 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_16/src/main/java/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.271774 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_16/src/main/java/com/fasterxml/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.272203 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_16/src/main/java/com/fasterxml/jackson/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.272327 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_16/src/main/java/com/fasterxml/jackson/databind/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.496451 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_16/src/main/java/com/fasterxml/jackson/databind/introspect/
+-rw-r--r--   0 dgros      (501) staff       (20)     3466 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_16/src/main/java/com/fasterxml/jackson/databind/introspect/AnnotationMap.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.272679 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_16_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.272770 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_16_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.272851 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_16_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.272930 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_16_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.273010 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_16_fixed/src/main/java/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.273105 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_16_fixed/src/main/java/com/fasterxml/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.273214 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_16_fixed/src/main/java/com/fasterxml/jackson/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.273310 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_16_fixed/src/main/java/com/fasterxml/jackson/databind/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.496768 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_16_fixed/src/main/java/com/fasterxml/jackson/databind/introspect/
+-rw-r--r--   0 dgros      (501) staff       (20)     3467 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_16_fixed/src/main/java/com/fasterxml/jackson/databind/introspect/AnnotationMap.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.273635 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_27/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.273735 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_27/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.273841 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_27/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.274043 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_27/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.274159 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_27/src/main/java/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.274249 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_27/src/main/java/com/fasterxml/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.274331 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_27/src/main/java/com/fasterxml/jackson/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.274424 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_27/src/main/java/com/fasterxml/jackson/databind/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.497053 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_27/src/main/java/com/fasterxml/jackson/databind/deser/
+-rw-r--r--   0 dgros      (501) staff       (20)    34392 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_27/src/main/java/com/fasterxml/jackson/databind/deser/BeanDeserializer.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.274716 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_27_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.274804 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_27_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.275035 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_27_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.275153 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_27_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.275266 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_27_fixed/src/main/java/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.275374 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_27_fixed/src/main/java/com/fasterxml/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.275497 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_27_fixed/src/main/java/com/fasterxml/jackson/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.275610 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_27_fixed/src/main/java/com/fasterxml/jackson/databind/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.497402 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_27_fixed/src/main/java/com/fasterxml/jackson/databind/deser/
+-rw-r--r--   0 dgros      (501) staff       (20)    34390 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_27_fixed/src/main/java/com/fasterxml/jackson/databind/deser/BeanDeserializer.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.275934 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_3/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.276040 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_3/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.276136 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_3/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.276235 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_3/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.276360 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_3/src/main/java/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.276476 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_3/src/main/java/com/fasterxml/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.276581 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_3/src/main/java/com/fasterxml/jackson/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.276677 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_3/src/main/java/com/fasterxml/jackson/databind/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.276780 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_3/src/main/java/com/fasterxml/jackson/databind/deser/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.497749 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_3/src/main/java/com/fasterxml/jackson/databind/deser/std/
+-rw-r--r--   0 dgros      (501) staff       (20)     5887 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_3/src/main/java/com/fasterxml/jackson/databind/deser/std/StringArrayDeserializer.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.277139 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_3_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.277235 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_3_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.277327 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_3_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.277411 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_3_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.277503 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_3_fixed/src/main/java/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.277599 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_3_fixed/src/main/java/com/fasterxml/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.277692 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_3_fixed/src/main/java/com/fasterxml/jackson/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.277778 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_3_fixed/src/main/java/com/fasterxml/jackson/databind/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.277955 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_3_fixed/src/main/java/com/fasterxml/jackson/databind/deser/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.498024 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_3_fixed/src/main/java/com/fasterxml/jackson/databind/deser/std/
+-rw-r--r--   0 dgros      (501) staff       (20)     5945 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_3_fixed/src/main/java/com/fasterxml/jackson/databind/deser/std/StringArrayDeserializer.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.278293 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_46/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.278378 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_46/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.278462 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_46/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.278553 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_46/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.278638 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_46/src/main/java/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.278730 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_46/src/main/java/com/fasterxml/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.278818 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_46/src/main/java/com/fasterxml/jackson/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.278910 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_46/src/main/java/com/fasterxml/jackson/databind/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.498353 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_46/src/main/java/com/fasterxml/jackson/databind/type/
+-rw-r--r--   0 dgros      (501) staff       (20)     5343 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_46/src/main/java/com/fasterxml/jackson/databind/type/ReferenceType.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.279243 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_46_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.279350 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_46_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.279454 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_46_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.279559 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_46_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.279672 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_46_fixed/src/main/java/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.279791 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_46_fixed/src/main/java/com/fasterxml/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.279900 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_46_fixed/src/main/java/com/fasterxml/jackson/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.280005 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_46_fixed/src/main/java/com/fasterxml/jackson/databind/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.498650 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_46_fixed/src/main/java/com/fasterxml/jackson/databind/type/
+-rw-r--r--   0 dgros      (501) staff       (20)     5344 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_46_fixed/src/main/java/com/fasterxml/jackson/databind/type/ReferenceType.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.280374 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_71/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.280466 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_71/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.280550 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_71/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.280635 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_71/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.280714 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_71/src/main/java/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.280810 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_71/src/main/java/com/fasterxml/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.280893 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_71/src/main/java/com/fasterxml/jackson/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.280973 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_71/src/main/java/com/fasterxml/jackson/databind/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.281061 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_71/src/main/java/com/fasterxml/jackson/databind/deser/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.498922 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_71/src/main/java/com/fasterxml/jackson/databind/deser/std/
+-rw-r--r--   0 dgros      (501) staff       (20)    14507 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_71/src/main/java/com/fasterxml/jackson/databind/deser/std/StdKeyDeserializer.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.281431 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_71_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.281528 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_71_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.281603 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_71_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.281675 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_71_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.281744 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_71_fixed/src/main/java/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.281809 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_71_fixed/src/main/java/com/fasterxml/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.281876 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_71_fixed/src/main/java/com/fasterxml/jackson/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.281942 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_71_fixed/src/main/java/com/fasterxml/jackson/databind/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.282012 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_71_fixed/src/main/java/com/fasterxml/jackson/databind/deser/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.499202 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_71_fixed/src/main/java/com/fasterxml/jackson/databind/deser/std/
+-rw-r--r--   0 dgros      (501) staff       (20)    14536 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_71_fixed/src/main/java/com/fasterxml/jackson/databind/deser/std/StdKeyDeserializer.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.282231 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_82/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.282296 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_82/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.282359 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_82/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.282423 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_82/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.282488 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_82/src/main/java/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.282551 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_82/src/main/java/com/fasterxml/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.282619 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_82/src/main/java/com/fasterxml/jackson/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.282685 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_82/src/main/java/com/fasterxml/jackson/databind/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.499482 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_82/src/main/java/com/fasterxml/jackson/databind/deser/
+-rw-r--r--   0 dgros      (501) staff       (20)    41582 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_82/src/main/java/com/fasterxml/jackson/databind/deser/BeanDeserializerFactory.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.282894 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_82_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.282953 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_82_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.283016 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_82_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.283077 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_82_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.283141 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_82_fixed/src/main/java/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.283204 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_82_fixed/src/main/java/com/fasterxml/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.283271 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_82_fixed/src/main/java/com/fasterxml/jackson/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.283338 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_82_fixed/src/main/java/com/fasterxml/jackson/databind/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.499975 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_82_fixed/src/main/java/com/fasterxml/jackson/databind/deser/
+-rw-r--r--   0 dgros      (501) staff       (20)    41601 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_82_fixed/src/main/java/com/fasterxml/jackson/databind/deser/BeanDeserializerFactory.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.283549 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_96/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.283614 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_96/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.283678 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_96/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.283743 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_96/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.283807 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_96/src/main/java/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.283872 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_96/src/main/java/com/fasterxml/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.283937 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_96/src/main/java/com/fasterxml/jackson/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.284005 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_96/src/main/java/com/fasterxml/jackson/databind/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.500452 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_96/src/main/java/com/fasterxml/jackson/databind/deser/
+-rw-r--r--   0 dgros      (501) staff       (20)    99497 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_96/src/main/java/com/fasterxml/jackson/databind/deser/BasicDeserializerFactory.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.284212 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_96_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.284276 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_96_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.284342 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_96_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.284407 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_96_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.284470 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_96_fixed/src/main/java/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.284533 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_96_fixed/src/main/java/com/fasterxml/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.284597 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_96_fixed/src/main/java/com/fasterxml/jackson/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.284664 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_96_fixed/src/main/java/com/fasterxml/jackson/databind/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.500894 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_96_fixed/src/main/java/com/fasterxml/jackson/databind/deser/
+-rw-r--r--   0 dgros      (501) staff       (20)    99485 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonDatabind_96_fixed/src/main/java/com/fasterxml/jackson/databind/deser/BasicDeserializerFactory.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.284852 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonXml_5/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.284914 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonXml_5/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.284980 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonXml_5/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.285063 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonXml_5/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.285143 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonXml_5/src/main/java/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.285229 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonXml_5/src/main/java/com/fasterxml/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.285317 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonXml_5/src/main/java/com/fasterxml/jackson/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.285409 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonXml_5/src/main/java/com/fasterxml/jackson/dataformat/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.285490 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonXml_5/src/main/java/com/fasterxml/jackson/dataformat/xml/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.501326 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonXml_5/src/main/java/com/fasterxml/jackson/dataformat/xml/ser/
+-rw-r--r--   0 dgros      (501) staff       (20)     8427 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonXml_5/src/main/java/com/fasterxml/jackson/dataformat/xml/ser/XmlSerializerProvider.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.285788 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonXml_5_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.285879 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonXml_5_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.285960 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonXml_5_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.286028 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonXml_5_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.286094 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonXml_5_fixed/src/main/java/com/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.286155 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonXml_5_fixed/src/main/java/com/fasterxml/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.286219 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonXml_5_fixed/src/main/java/com/fasterxml/jackson/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.286292 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonXml_5_fixed/src/main/java/com/fasterxml/jackson/dataformat/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.286383 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonXml_5_fixed/src/main/java/com/fasterxml/jackson/dataformat/xml/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.501598 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonXml_5_fixed/src/main/java/com/fasterxml/jackson/dataformat/xml/ser/
+-rw-r--r--   0 dgros      (501) staff       (20)     8431 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/JacksonXml_5_fixed/src/main/java/com/fasterxml/jackson/dataformat/xml/ser/XmlSerializerProvider.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.286692 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_15/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.286799 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_15/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.286898 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_15/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.287002 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_15/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.287112 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_15/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.287207 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_15/src/main/java/org/jsoup/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.501876 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_15/src/main/java/org/jsoup/parser/
+-rw-r--r--   0 dgros      (501) staff       (20)    68086 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_15/src/main/java/org/jsoup/parser/TreeBuilderState.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.287481 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_15_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.287564 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_15_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.287756 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_15_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.287870 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_15_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.287967 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_15_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.288064 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_15_fixed/src/main/java/org/jsoup/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.502372 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_15_fixed/src/main/java/org/jsoup/parser/
+-rw-r--r--   0 dgros      (501) staff       (20)    68096 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_15_fixed/src/main/java/org/jsoup/parser/TreeBuilderState.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.288394 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_17/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.288488 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_17/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.288572 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_17/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.288658 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_17/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.288748 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_17/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.288839 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_17/src/main/java/org/jsoup/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.503134 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_17/src/main/java/org/jsoup/parser/
+-rw-r--r--   0 dgros      (501) staff       (20)    68096 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_17/src/main/java/org/jsoup/parser/TreeBuilderState.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.289114 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_17_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.289283 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_17_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.289378 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_17_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.289533 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_17_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.289632 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_17_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.289718 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_17_fixed/src/main/java/org/jsoup/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.503561 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_17_fixed/src/main/java/org/jsoup/parser/
+-rw-r--r--   0 dgros      (501) staff       (20)    68098 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_17_fixed/src/main/java/org/jsoup/parser/TreeBuilderState.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.290370 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_25/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.290468 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_25/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.290556 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_25/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.290636 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_25/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.290706 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_25/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.290778 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_25/src/main/java/org/jsoup/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.503959 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_25/src/main/java/org/jsoup/parser/
+-rw-r--r--   0 dgros      (501) staff       (20)     8288 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_25/src/main/java/org/jsoup/parser/Tag.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.290985 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_25_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.291052 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_25_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.291116 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_25_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.291181 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_25_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.291251 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_25_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.291316 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_25_fixed/src/main/java/org/jsoup/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.504264 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_25_fixed/src/main/java/org/jsoup/parser/
+-rw-r--r--   0 dgros      (501) staff       (20)     8300 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_25_fixed/src/main/java/org/jsoup/parser/Tag.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.291521 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_32/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.291590 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_32/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.291658 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_32/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.291725 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_32/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.291797 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_32/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.291867 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_32/src/main/java/org/jsoup/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.504591 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_32/src/main/java/org/jsoup/nodes/
+-rw-r--r--   0 dgros      (501) staff       (20)    40267 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_32/src/main/java/org/jsoup/nodes/Element.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.292300 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_32_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.292415 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_32_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.292563 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_32_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.292684 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_32_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.292796 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_32_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.292907 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_32_fixed/src/main/java/org/jsoup/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.504931 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_32_fixed/src/main/java/org/jsoup/nodes/
+-rw-r--r--   0 dgros      (501) staff       (20)    40343 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_32_fixed/src/main/java/org/jsoup/nodes/Element.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.293253 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_43/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.293364 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_43/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.293452 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_43/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.293539 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_43/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.293638 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_43/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.293739 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_43/src/main/java/org/jsoup/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.505291 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_43/src/main/java/org/jsoup/nodes/
+-rw-r--r--   0 dgros      (501) staff       (20)    43122 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_43/src/main/java/org/jsoup/nodes/Element.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.294061 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_43_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.294168 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_43_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.294268 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_43_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.294367 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_43_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.294468 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_43_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.294575 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_43_fixed/src/main/java/org/jsoup/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.506000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_43_fixed/src/main/java/org/jsoup/nodes/
+-rw-r--r--   0 dgros      (501) staff       (20)    43117 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_43_fixed/src/main/java/org/jsoup/nodes/Element.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.294895 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_45/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.295001 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_45/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.295102 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_45/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.295210 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_45/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.295311 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_45/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.295413 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_45/src/main/java/org/jsoup/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.506331 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_45/src/main/java/org/jsoup/parser/
+-rw-r--r--   0 dgros      (501) staff       (20)    24727 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_45/src/main/java/org/jsoup/parser/HtmlTreeBuilder.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.295746 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_45_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.295892 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_45_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.296024 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_45_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.296140 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_45_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.296258 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_45_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.296380 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_45_fixed/src/main/java/org/jsoup/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.506650 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_45_fixed/src/main/java/org/jsoup/parser/
+-rw-r--r--   0 dgros      (501) staff       (20)    24727 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_45_fixed/src/main/java/org/jsoup/parser/HtmlTreeBuilder.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.296723 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_46/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.296826 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_46/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.296970 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_46/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.297080 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_46/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.297175 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_46/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.297280 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_46/src/main/java/org/jsoup/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.506967 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_46/src/main/java/org/jsoup/nodes/
+-rw-r--r--   0 dgros      (501) staff       (20)     9951 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_46/src/main/java/org/jsoup/nodes/Entities.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.297579 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_46_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.297675 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_46_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.297767 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_46_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.297863 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_46_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.298096 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_46_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.298221 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_46_fixed/src/main/java/org/jsoup/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.507219 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_46_fixed/src/main/java/org/jsoup/nodes/
+-rw-r--r--   0 dgros      (501) staff       (20)     9958 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_46_fixed/src/main/java/org/jsoup/nodes/Entities.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.298548 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_47/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.298630 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_47/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.298720 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_47/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.298808 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_47/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.298916 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_47/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.299002 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_47/src/main/java/org/jsoup/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.507478 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_47/src/main/java/org/jsoup/nodes/
+-rw-r--r--   0 dgros      (501) staff       (20)    10074 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_47/src/main/java/org/jsoup/nodes/Entities.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.299316 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_47_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.299406 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_47_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.299504 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_47_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.299592 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_47_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.299667 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_47_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.299751 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_47_fixed/src/main/java/org/jsoup/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.507750 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_47_fixed/src/main/java/org/jsoup/nodes/
+-rw-r--r--   0 dgros      (501) staff       (20)    10108 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_47_fixed/src/main/java/org/jsoup/nodes/Entities.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.299998 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_51/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.300081 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_51/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.300166 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_51/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.300259 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_51/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.300360 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_51/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.300457 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_51/src/main/java/org/jsoup/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.508058 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_51/src/main/java/org/jsoup/parser/
+-rw-r--r--   0 dgros      (501) staff       (20)    10960 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_51/src/main/java/org/jsoup/parser/CharacterReader.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.300775 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_51_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.300874 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_51_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.300957 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_51_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.301041 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_51_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.301134 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_51_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.301226 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_51_fixed/src/main/java/org/jsoup/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.508310 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_51_fixed/src/main/java/org/jsoup/parser/
+-rw-r--r--   0 dgros      (501) staff       (20)    10985 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_51_fixed/src/main/java/org/jsoup/parser/CharacterReader.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.301505 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_62/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.301603 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_62/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.301687 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_62/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.301765 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_62/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.301844 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_62/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.301934 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_62/src/main/java/org/jsoup/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.508571 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_62/src/main/java/org/jsoup/parser/
+-rw-r--r--   0 dgros      (501) staff       (20)    70965 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_62/src/main/java/org/jsoup/parser/HtmlTreeBuilderState.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.302212 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_62_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.302303 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_62_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.302390 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_62_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.302481 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_62_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.302563 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_62_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.302658 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_62_fixed/src/main/java/org/jsoup/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.508958 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_62_fixed/src/main/java/org/jsoup/parser/
+-rw-r--r--   0 dgros      (501) staff       (20)    71003 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_62_fixed/src/main/java/org/jsoup/parser/HtmlTreeBuilderState.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.302915 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_76/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.302996 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_76/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.303076 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_76/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.303168 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_76/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.303249 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_76/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.303322 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_76/src/main/java/org/jsoup/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.509328 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_76/src/main/java/org/jsoup/parser/
+-rw-r--r--   0 dgros      (501) staff       (20)    71507 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_76/src/main/java/org/jsoup/parser/HtmlTreeBuilderState.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.303592 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_76_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.303677 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_76_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.303764 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_76_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.303860 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_76_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.303954 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_76_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.304056 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_76_fixed/src/main/java/org/jsoup/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.509701 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_76_fixed/src/main/java/org/jsoup/parser/
+-rw-r--r--   0 dgros      (501) staff       (20)    71588 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_76_fixed/src/main/java/org/jsoup/parser/HtmlTreeBuilderState.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.304333 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_86/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.304428 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_86/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.304524 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_86/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.304610 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_86/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.304698 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_86/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.304789 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_86/src/main/java/org/jsoup/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.510058 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_86/src/main/java/org/jsoup/nodes/
+-rw-r--r--   0 dgros      (501) staff       (20)     2346 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_86/src/main/java/org/jsoup/nodes/Comment.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.305058 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_86_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.305148 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_86_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.305239 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_86_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.305317 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_86_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.305402 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_86_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.305494 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_86_fixed/src/main/java/org/jsoup/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.510325 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_86_fixed/src/main/java/org/jsoup/nodes/
+-rw-r--r--   0 dgros      (501) staff       (20)     2348 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_86_fixed/src/main/java/org/jsoup/nodes/Comment.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.305770 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_88/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.305854 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_88/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.311766 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_88/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.311953 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_88/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.314339 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_88/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.314456 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_88/src/main/java/org/jsoup/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.510592 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_88/src/main/java/org/jsoup/nodes/
+-rw-r--r--   0 dgros      (501) staff       (20)     6915 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_88/src/main/java/org/jsoup/nodes/Attribute.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.314768 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_88_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.314838 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_88_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.315011 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_88_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.315103 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_88_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.315172 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_88_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.315234 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_88_fixed/src/main/java/org/jsoup/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.510983 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_88_fixed/src/main/java/org/jsoup/nodes/
+-rw-r--r--   0 dgros      (501) staff       (20)     6940 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_88_fixed/src/main/java/org/jsoup/nodes/Attribute.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.315458 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_9/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.315516 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_9/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.315582 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_9/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.315672 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_9/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.315757 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_9/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.315825 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_9/src/main/java/org/jsoup/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.511531 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_9/src/main/java/org/jsoup/nodes/
+-rw-r--r--   0 dgros      (501) staff       (20)    76534 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_9/src/main/java/org/jsoup/nodes/Entities.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.316003 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_9_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.316063 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_9_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.316155 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_9_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.316247 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_9_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.316344 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_9_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.316437 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_9_fixed/src/main/java/org/jsoup/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.511985 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_9_fixed/src/main/java/org/jsoup/nodes/
+-rw-r--r--   0 dgros      (501) staff       (20)    76538 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Jsoup_9_fixed/src/main/java/org/jsoup/nodes/Entities.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.316721 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_16/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.316813 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_16/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.316898 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_16/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.316982 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_16/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.317047 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_16/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.317111 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_16/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.317174 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_16/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.317237 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_16/src/main/java/org/apache/commons/lang3/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.512436 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_16/src/main/java/org/apache/commons/lang3/math/
+-rw-r--r--   0 dgros      (501) staff       (20)    47695 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_16/src/main/java/org/apache/commons/lang3/math/NumberUtils.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.317443 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_16_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.317502 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_16_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.317565 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_16_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.317633 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_16_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.317699 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_16_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.317764 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_16_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.317830 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_16_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.317893 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_16_fixed/src/main/java/org/apache/commons/lang3/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.512827 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_16_fixed/src/main/java/org/apache/commons/lang3/math/
+-rw-r--r--   0 dgros      (501) staff       (20)    47744 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_16_fixed/src/main/java/org/apache/commons/lang3/math/NumberUtils.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.318089 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_21/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.318149 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_21/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.318214 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_21/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.318282 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_21/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.318349 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_21/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.318412 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_21/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.318476 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_21/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.318537 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_21/src/main/java/org/apache/commons/lang3/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.513232 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_21/src/main/java/org/apache/commons/lang3/time/
+-rw-r--r--   0 dgros      (501) staff       (20)    79296 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_21/src/main/java/org/apache/commons/lang3/time/DateUtils.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.318753 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_21_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.318814 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_21_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.318882 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_21_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.318947 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_21_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.319008 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_21_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.319075 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_21_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.319139 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_21_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.319202 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_21_fixed/src/main/java/org/apache/commons/lang3/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.513773 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_21_fixed/src/main/java/org/apache/commons/lang3/time/
+-rw-r--r--   0 dgros      (501) staff       (20)    79310 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_21_fixed/src/main/java/org/apache/commons/lang3/time/DateUtils.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.319410 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_24/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.319475 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_24/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.319536 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_24/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.319604 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_24/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.319669 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_24/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.319738 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_24/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.319841 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_24/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.319938 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_24/src/main/java/org/apache/commons/lang3/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.514664 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_24/src/main/java/org/apache/commons/lang3/math/
+-rw-r--r--   0 dgros      (501) staff       (20)    47953 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_24/src/main/java/org/apache/commons/lang3/math/NumberUtils.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.320229 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_24_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.320318 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_24_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.320404 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_24_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.320484 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_24_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.320571 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_24_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.320655 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_24_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.320735 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_24_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.320832 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_24_fixed/src/main/java/org/apache/commons/lang3/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.515057 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_24_fixed/src/main/java/org/apache/commons/lang3/math/
+-rw-r--r--   0 dgros      (501) staff       (20)    47969 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_24_fixed/src/main/java/org/apache/commons/lang3/math/NumberUtils.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.321108 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_26/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.321172 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_26/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.321252 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_26/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.321331 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_26/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.321421 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_26/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.321500 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_26/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.321594 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_26/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.321701 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_26/src/main/java/org/apache/commons/lang3/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.515437 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_26/src/main/java/org/apache/commons/lang3/time/
+-rw-r--r--   0 dgros      (501) staff       (20)    56991 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_26/src/main/java/org/apache/commons/lang3/time/FastDateFormat.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.322044 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_26_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.322151 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_26_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.322270 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_26_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.322368 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_26_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.322466 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_26_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.322550 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_26_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.322633 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_26_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.322713 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_26_fixed/src/main/java/org/apache/commons/lang3/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.515911 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_26_fixed/src/main/java/org/apache/commons/lang3/time/
+-rw-r--r--   0 dgros      (501) staff       (20)    57000 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_26_fixed/src/main/java/org/apache/commons/lang3/time/FastDateFormat.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.322950 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_29/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.323027 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_29/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.323111 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_29/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.323189 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_29/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.323279 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_29/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.323372 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_29/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.323621 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_29/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.516359 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_29/src/main/java/org/apache/commons/lang3/
+-rw-r--r--   0 dgros      (501) staff       (20)    60142 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_29/src/main/java/org/apache/commons/lang3/SystemUtils.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.323877 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_29_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.323961 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_29_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.324050 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_29_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.324138 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_29_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.324222 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_29_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.324306 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_29_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.324401 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_29_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.516788 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_29_fixed/src/main/java/org/apache/commons/lang3/
+-rw-r--r--   0 dgros      (501) staff       (20)    60140 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_29_fixed/src/main/java/org/apache/commons/lang3/SystemUtils.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.324662 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_33/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.324745 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_33/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.324827 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_33/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.324931 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_33/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.325042 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_33/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.325156 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_33/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.325265 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_33/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.517225 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_33/src/main/java/org/apache/commons/lang3/
+-rw-r--r--   0 dgros      (501) staff       (20)    42447 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_33/src/main/java/org/apache/commons/lang3/ClassUtils.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.325592 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_33_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.325677 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_33_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.325748 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_33_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.325828 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_33_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.325905 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_33_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.325984 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_33_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.326066 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_33_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.517575 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_33_fixed/src/main/java/org/apache/commons/lang3/
+-rw-r--r--   0 dgros      (501) staff       (20)    42473 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_33_fixed/src/main/java/org/apache/commons/lang3/ClassUtils.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.326374 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_57/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.326464 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_57/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.326546 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_57/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.326626 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_57/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.326713 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_57/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.326792 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_57/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.517917 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_57/src/java/org/apache/commons/lang/
+-rw-r--r--   0 dgros      (501) staff       (20)    11552 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_57/src/java/org/apache/commons/lang/LocaleUtils.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.327044 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_57_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.327125 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_57_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.327203 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_57_fixed/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.327283 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_57_fixed/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.327390 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_57_fixed/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.327495 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_57_fixed/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.518182 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_57_fixed/src/java/org/apache/commons/lang/
+-rw-r--r--   0 dgros      (501) staff       (20)    11554 2024-01-31 01:30:32.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_57_fixed/src/java/org/apache/commons/lang/LocaleUtils.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.327800 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_59/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.327887 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_59/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.327977 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_59/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.328074 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_59/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.328163 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_59/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.328257 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_59/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.329204 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_59/src/java/org/apache/commons/lang/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.518534 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_59/src/java/org/apache/commons/lang/text/
+-rw-r--r--   0 dgros      (501) staff       (20)    80811 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_59/src/java/org/apache/commons/lang/text/StrBuilder.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.329555 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_59_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.329660 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_59_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.329756 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_59_fixed/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.329837 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_59_fixed/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.329938 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_59_fixed/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.330023 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_59_fixed/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.330123 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_59_fixed/src/java/org/apache/commons/lang/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.519277 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_59_fixed/src/java/org/apache/commons/lang/text/
+-rw-r--r--   0 dgros      (501) staff       (20)    80810 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_59_fixed/src/java/org/apache/commons/lang/text/StrBuilder.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.330394 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_6/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.330458 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_6/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.331494 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_6/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.331685 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_6/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.331887 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_6/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.332068 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_6/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.332164 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_6/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.332368 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_6/src/main/java/org/apache/commons/lang3/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.332483 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_6/src/main/java/org/apache/commons/lang3/text/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.519669 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_6/src/main/java/org/apache/commons/lang3/text/translate/
+-rw-r--r--   0 dgros      (501) staff       (20)     4948 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_6/src/main/java/org/apache/commons/lang3/text/translate/CharSequenceTranslator.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.332802 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_61/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.332893 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_61/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.332981 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_61/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.333073 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_61/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.333168 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_61/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.333263 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_61/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.333346 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_61/src/java/org/apache/commons/lang/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.519935 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_61/src/java/org/apache/commons/lang/text/
+-rw-r--r--   0 dgros      (501) staff       (20)    80832 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_61/src/java/org/apache/commons/lang/text/StrBuilder.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.333631 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_61_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.333727 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_61_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.336154 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_61_fixed/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.336441 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_61_fixed/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.336560 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_61_fixed/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.336675 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_61_fixed/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.336779 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_61_fixed/src/java/org/apache/commons/lang/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.520312 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_61_fixed/src/java/org/apache/commons/lang/text/
+-rw-r--r--   0 dgros      (501) staff       (20)    80826 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_61_fixed/src/java/org/apache/commons/lang/text/StrBuilder.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.337122 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_6_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.341920 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_6_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.342134 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_6_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.342378 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_6_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.342486 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_6_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.342560 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_6_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.342629 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_6_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.342697 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_6_fixed/src/main/java/org/apache/commons/lang3/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.342767 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_6_fixed/src/main/java/org/apache/commons/lang3/text/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.520698 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_6_fixed/src/main/java/org/apache/commons/lang3/text/translate/
+-rw-r--r--   0 dgros      (501) staff       (20)     4947 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Lang_6_fixed/src/main/java/org/apache/commons/lang3/text/translate/CharSequenceTranslator.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.343555 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_104/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.343640 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_104/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.343729 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_104/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.343812 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_104/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.343902 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_104/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.343995 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_104/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.344092 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_104/src/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.520964 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_104/src/java/org/apache/commons/math/special/
+-rw-r--r--   0 dgros      (501) staff       (20)     9328 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_104/src/java/org/apache/commons/math/special/Gamma.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.344390 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_104_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.344484 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_104_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.344837 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_104_fixed/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.344986 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_104_fixed/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.345095 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_104_fixed/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.345198 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_104_fixed/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.345295 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_104_fixed/src/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.521262 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_104_fixed/src/java/org/apache/commons/math/special/
+-rw-r--r--   0 dgros      (501) staff       (20)     9329 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_104_fixed/src/java/org/apache/commons/math/special/Gamma.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.345614 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_105/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.345708 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_105/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.345795 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_105/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.345904 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_105/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.346000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_105/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.346113 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_105/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.346220 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_105/src/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.346316 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_105/src/java/org/apache/commons/math/stat/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.521535 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_105/src/java/org/apache/commons/math/stat/regression/
+-rw-r--r--   0 dgros      (501) staff       (20)    18430 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_105/src/java/org/apache/commons/math/stat/regression/SimpleRegression.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.346634 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_105_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.346722 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_105_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.346810 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_105_fixed/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.346924 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_105_fixed/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.347054 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_105_fixed/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.347203 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_105_fixed/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.347307 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_105_fixed/src/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.347407 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_105_fixed/src/java/org/apache/commons/math/stat/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.521965 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_105_fixed/src/java/org/apache/commons/math/stat/regression/
+-rw-r--r--   0 dgros      (501) staff       (20)    18444 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_105_fixed/src/java/org/apache/commons/math/stat/regression/SimpleRegression.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.347641 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_11/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.347708 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_11/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.347775 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_11/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.347840 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_11/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.347904 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_11/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.347971 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_11/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.348036 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_11/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.348099 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_11/src/main/java/org/apache/commons/math3/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.522405 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_11/src/main/java/org/apache/commons/math3/distribution/
+-rw-r--r--   0 dgros      (501) staff       (20)     9008 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_11/src/main/java/org/apache/commons/math3/distribution/MultivariateNormalDistribution.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.348302 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_11_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.348363 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_11_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.348427 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_11_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.348492 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_11_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.348557 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_11_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.348818 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_11_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.348990 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_11_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.349137 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_11_fixed/src/main/java/org/apache/commons/math3/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.522709 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_11_fixed/src/main/java/org/apache/commons/math3/distribution/
+-rw-r--r--   0 dgros      (501) staff       (20)     9010 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_11_fixed/src/main/java/org/apache/commons/math3/distribution/MultivariateNormalDistribution.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.349530 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_2/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.349627 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_2/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.349722 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_2/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.349795 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_2/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.349854 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_2/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.349994 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_2/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.350086 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_2/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.350167 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_2/src/main/java/org/apache/commons/math3/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.523026 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_2/src/main/java/org/apache/commons/math3/distribution/
+-rw-r--r--   0 dgros      (501) staff       (20)    11862 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_2/src/main/java/org/apache/commons/math3/distribution/HypergeometricDistribution.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.350503 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_27/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.350600 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_27/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.350697 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_27/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.350792 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_27/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.350888 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_27/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.351158 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_27/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.351258 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_27/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.351372 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_27/src/main/java/org/apache/commons/math3/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.523380 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_27/src/main/java/org/apache/commons/math3/fraction/
+-rw-r--r--   0 dgros      (501) staff       (20)    23381 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_27/src/main/java/org/apache/commons/math3/fraction/Fraction.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.351693 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_27_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.351802 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_27_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.351897 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_27_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.352000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_27_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.352144 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_27_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.352242 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_27_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.352339 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_27_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.352443 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_27_fixed/src/main/java/org/apache/commons/math3/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.523788 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_27_fixed/src/main/java/org/apache/commons/math3/fraction/
+-rw-r--r--   0 dgros      (501) staff       (20)    23373 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_27_fixed/src/main/java/org/apache/commons/math3/fraction/Fraction.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.352699 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_2_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.352787 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_2_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.352875 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_2_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.352969 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_2_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.353145 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_2_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.353235 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_2_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.353313 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_2_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.353389 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_2_fixed/src/main/java/org/apache/commons/math3/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.524179 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_2_fixed/src/main/java/org/apache/commons/math3/distribution/
+-rw-r--r--   0 dgros      (501) staff       (20)    11853 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_2_fixed/src/main/java/org/apache/commons/math3/distribution/HypergeometricDistribution.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.353643 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_30/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.353722 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_30/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.353793 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_30/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.353864 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_30/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.353932 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_30/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.353996 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_30/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.354072 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_30/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.354140 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_30/src/main/java/org/apache/commons/math3/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.354207 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_30/src/main/java/org/apache/commons/math3/stat/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.524651 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_30/src/main/java/org/apache/commons/math3/stat/inference/
+-rw-r--r--   0 dgros      (501) staff       (20)     8816 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_30/src/main/java/org/apache/commons/math3/stat/inference/MannWhitneyUTest.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.354437 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_30_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.354513 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_30_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.354577 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_30_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.354665 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_30_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.354742 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_30_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.354881 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_30_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.354994 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_30_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.355095 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_30_fixed/src/main/java/org/apache/commons/math3/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.355191 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_30_fixed/src/main/java/org/apache/commons/math3/stat/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.524942 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_30_fixed/src/main/java/org/apache/commons/math3/stat/inference/
+-rw-r--r--   0 dgros      (501) staff       (20)     8819 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_30_fixed/src/main/java/org/apache/commons/math3/stat/inference/MannWhitneyUTest.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.355505 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_32/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.355601 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_32/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.355693 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_32/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.355784 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_32/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.355870 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_32/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.355962 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_32/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.356054 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_32/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.356133 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_32/src/main/java/org/apache/commons/math3/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.356230 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_32/src/main/java/org/apache/commons/math3/geometry/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.356311 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_32/src/main/java/org/apache/commons/math3/geometry/euclidean/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.525295 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_32/src/main/java/org/apache/commons/math3/geometry/euclidean/twod/
+-rw-r--r--   0 dgros      (501) staff       (20)    19957 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_32/src/main/java/org/apache/commons/math3/geometry/euclidean/twod/PolygonsSet.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.356591 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_32_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.356678 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_32_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.356755 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_32_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.356837 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_32_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.356921 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_32_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.357008 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_32_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.357174 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_32_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.357325 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_32_fixed/src/main/java/org/apache/commons/math3/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.357428 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_32_fixed/src/main/java/org/apache/commons/math3/geometry/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.357523 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_32_fixed/src/main/java/org/apache/commons/math3/geometry/euclidean/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.525865 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_32_fixed/src/main/java/org/apache/commons/math3/geometry/euclidean/twod/
+-rw-r--r--   0 dgros      (501) staff       (20)    19982 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_32_fixed/src/main/java/org/apache/commons/math3/geometry/euclidean/twod/PolygonsSet.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.357842 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_33/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.357929 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_33/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.358012 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_33/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.358102 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_33/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.358191 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_33/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.358438 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_33/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.358540 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_33/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.358640 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_33/src/main/java/org/apache/commons/math3/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.358732 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_33/src/main/java/org/apache/commons/math3/optimization/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.526222 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_33/src/main/java/org/apache/commons/math3/optimization/linear/
+-rw-r--r--   0 dgros      (501) staff       (20)    22991 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_33/src/main/java/org/apache/commons/math3/optimization/linear/SimplexTableau.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.359027 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_33_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.359119 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_33_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.359239 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_33_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.359324 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_33_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.359416 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_33_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.359502 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_33_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.359591 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_33_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.359686 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_33_fixed/src/main/java/org/apache/commons/math3/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.359783 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_33_fixed/src/main/java/org/apache/commons/math3/optimization/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.526625 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_33_fixed/src/main/java/org/apache/commons/math3/optimization/linear/
+-rw-r--r--   0 dgros      (501) staff       (20)    22991 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_33_fixed/src/main/java/org/apache/commons/math3/optimization/linear/SimplexTableau.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.360004 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_34/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.360068 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_34/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.360135 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_34/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.360207 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_34/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.360272 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_34/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.360352 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_34/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.360432 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_34/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.360516 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_34/src/main/java/org/apache/commons/math3/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.527000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_34/src/main/java/org/apache/commons/math3/genetics/
+-rw-r--r--   0 dgros      (501) staff       (20)     8284 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_34/src/main/java/org/apache/commons/math3/genetics/ListPopulation.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.360777 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_34_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.360860 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_34_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.360940 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_34_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.361098 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_34_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.361196 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_34_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.361303 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_34_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.361402 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_34_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.361500 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_34_fixed/src/main/java/org/apache/commons/math3/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.527328 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_34_fixed/src/main/java/org/apache/commons/math3/genetics/
+-rw-r--r--   0 dgros      (501) staff       (20)     8289 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_34_fixed/src/main/java/org/apache/commons/math3/genetics/ListPopulation.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.361826 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_41/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.361927 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_41/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.362020 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_41/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.362105 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_41/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.362188 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_41/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.362269 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_41/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.362347 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_41/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.362442 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_41/src/main/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.362531 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_41/src/main/java/org/apache/commons/math/stat/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.362617 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_41/src/main/java/org/apache/commons/math/stat/descriptive/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.527665 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_41/src/main/java/org/apache/commons/math/stat/descriptive/moment/
+-rw-r--r--   0 dgros      (501) staff       (20)    24987 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_41/src/main/java/org/apache/commons/math/stat/descriptive/moment/Variance.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.362920 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_41_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.363011 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_41_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.363097 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_41_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.363200 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_41_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.363308 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_41_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.363401 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_41_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.363503 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_41_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.363617 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_41_fixed/src/main/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.363741 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_41_fixed/src/main/java/org/apache/commons/math/stat/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.363860 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_41_fixed/src/main/java/org/apache/commons/math/stat/descriptive/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.527991 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_41_fixed/src/main/java/org/apache/commons/math/stat/descriptive/moment/
+-rw-r--r--   0 dgros      (501) staff       (20)    24991 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_41_fixed/src/main/java/org/apache/commons/math/stat/descriptive/moment/Variance.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.364168 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_5/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.364256 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_5/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.364354 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_5/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.364431 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_5/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.364517 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_5/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.364600 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_5/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.364681 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_5/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.364767 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_5/src/main/java/org/apache/commons/math3/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.528322 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_5/src/main/java/org/apache/commons/math3/complex/
+-rw-r--r--   0 dgros      (501) staff       (20)    41467 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_5/src/main/java/org/apache/commons/math3/complex/Complex.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.365062 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_57/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.365145 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_57/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.365231 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_57/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.365321 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_57/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.365408 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_57/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.365487 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_57/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.365568 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_57/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.365657 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_57/src/main/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.365750 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_57/src/main/java/org/apache/commons/math/stat/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.528917 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_57/src/main/java/org/apache/commons/math/stat/clustering/
+-rw-r--r--   0 dgros      (501) staff       (20)    12566 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_57/src/main/java/org/apache/commons/math/stat/clustering/KMeansPlusPlusClusterer.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.366296 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_57_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.366390 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_57_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.366481 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_57_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.366580 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_57_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.366681 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_57_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.366775 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_57_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.366873 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_57_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.367092 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_57_fixed/src/main/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.367218 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_57_fixed/src/main/java/org/apache/commons/math/stat/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.529254 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_57_fixed/src/main/java/org/apache/commons/math/stat/clustering/
+-rw-r--r--   0 dgros      (501) staff       (20)    12569 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_57_fixed/src/main/java/org/apache/commons/math/stat/clustering/KMeansPlusPlusClusterer.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.367573 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_58/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.367661 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_58/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.367757 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_58/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.367851 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_58/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.367941 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_58/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.368031 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_58/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.368156 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_58/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.368256 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_58/src/main/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.368364 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_58/src/main/java/org/apache/commons/math/optimization/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.529550 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_58/src/main/java/org/apache/commons/math/optimization/fitting/
+-rw-r--r--   0 dgros      (501) staff       (20)    13601 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_58/src/main/java/org/apache/commons/math/optimization/fitting/GaussianFitter.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.368710 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_58_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.368798 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_58_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.369108 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_58_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.369222 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_58_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.369353 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_58_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.369469 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_58_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.370186 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_58_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.370313 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_58_fixed/src/main/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.370456 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_58_fixed/src/main/java/org/apache/commons/math/optimization/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.529848 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_58_fixed/src/main/java/org/apache/commons/math/optimization/fitting/
+-rw-r--r--   0 dgros      (501) staff       (20)    13574 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_58_fixed/src/main/java/org/apache/commons/math/optimization/fitting/GaussianFitter.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.371029 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_59/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.371117 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_59/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.373273 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_59/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.373417 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_59/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.373559 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_59/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.373655 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_59/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.373729 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_59/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.373798 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_59/src/main/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.530132 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_59/src/main/java/org/apache/commons/math/util/
+-rw-r--r--   0 dgros      (501) staff       (20)   103525 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_59/src/main/java/org/apache/commons/math/util/FastMath.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.374014 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_59_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.374080 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_59_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.374218 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_59_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.374315 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_59_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.374416 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_59_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.374512 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_59_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.374604 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_59_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.374697 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_59_fixed/src/main/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.530660 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_59_fixed/src/main/java/org/apache/commons/math/util/
+-rw-r--r--   0 dgros      (501) staff       (20)   103525 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_59_fixed/src/main/java/org/apache/commons/math/util/FastMath.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.375009 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_5_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.375096 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_5_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.375186 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_5_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.375278 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_5_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.375367 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_5_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.375459 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_5_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.375551 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_5_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.375635 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_5_fixed/src/main/java/org/apache/commons/math3/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.531358 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_5_fixed/src/main/java/org/apache/commons/math3/complex/
+-rw-r--r--   0 dgros      (501) staff       (20)    41467 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_5_fixed/src/main/java/org/apache/commons/math3/complex/Complex.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.375929 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_63/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.376020 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_63/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.376102 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_63/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.376189 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_63/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.376273 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_63/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.376357 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_63/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.376444 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_63/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.376538 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_63/src/main/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.531859 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_63/src/main/java/org/apache/commons/math/util/
+-rw-r--r--   0 dgros      (501) staff       (20)    69070 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_63/src/main/java/org/apache/commons/math/util/MathUtils.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.376814 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_63_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.376902 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_63_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.376988 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_63_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.377072 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_63_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.377168 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_63_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.377257 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_63_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.377350 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_63_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.377443 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_63_fixed/src/main/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.532667 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_63_fixed/src/main/java/org/apache/commons/math/util/
+-rw-r--r--   0 dgros      (501) staff       (20)    69039 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_63_fixed/src/main/java/org/apache/commons/math/util/MathUtils.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.377738 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_69/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.377825 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_69/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.377905 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_69/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.377992 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_69/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.378083 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_69/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.378170 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_69/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.378270 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_69/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.378356 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_69/src/main/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.378446 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_69/src/main/java/org/apache/commons/math/stat/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.533250 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_69/src/main/java/org/apache/commons/math/stat/correlation/
+-rw-r--r--   0 dgros      (501) staff       (20)    11236 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_69/src/main/java/org/apache/commons/math/stat/correlation/PearsonsCorrelation.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.378770 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_69_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.378857 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_69_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.378945 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_69_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.379035 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_69_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.379126 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_69_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.379215 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_69_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.379303 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_69_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.379387 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_69_fixed/src/main/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.379482 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_69_fixed/src/main/java/org/apache/commons/math/stat/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.533637 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_69_fixed/src/main/java/org/apache/commons/math/stat/correlation/
+-rw-r--r--   0 dgros      (501) staff       (20)    11231 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_69_fixed/src/main/java/org/apache/commons/math/stat/correlation/PearsonsCorrelation.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.379775 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_70/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.379857 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_70/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.379941 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_70/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.380022 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_70/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.380110 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_70/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.380211 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_70/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.380304 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_70/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.380393 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_70/src/main/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.380475 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_70/src/main/java/org/apache/commons/math/analysis/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.533980 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_70/src/main/java/org/apache/commons/math/analysis/solvers/
+-rw-r--r--   0 dgros      (501) staff       (20)     3633 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_70/src/main/java/org/apache/commons/math/analysis/solvers/BisectionSolver.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.380693 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_70_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.380754 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_70_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.380814 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_70_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.380877 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_70_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.380939 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_70_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.381406 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_70_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.381572 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_70_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.381684 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_70_fixed/src/main/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.381785 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_70_fixed/src/main/java/org/apache/commons/math/analysis/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.534332 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_70_fixed/src/main/java/org/apache/commons/math/analysis/solvers/
+-rw-r--r--   0 dgros      (501) staff       (20)     3636 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_70_fixed/src/main/java/org/apache/commons/math/analysis/solvers/BisectionSolver.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.382152 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_75/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.382257 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_75/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.382346 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_75/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.382437 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_75/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.382533 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_75/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.382791 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_75/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.382895 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_75/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.382966 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_75/src/main/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.534744 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_75/src/main/java/org/apache/commons/math/stat/
+-rw-r--r--   0 dgros      (501) staff       (20)    18691 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_75/src/main/java/org/apache/commons/math/stat/Frequency.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.383178 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_75_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.383254 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_75_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.383318 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_75_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.383404 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_75_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.383497 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_75_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.383579 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_75_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.383671 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_75_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.383770 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_75_fixed/src/main/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.535262 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_75_fixed/src/main/java/org/apache/commons/math/stat/
+-rw-r--r--   0 dgros      (501) staff       (20)    18688 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_75_fixed/src/main/java/org/apache/commons/math/stat/Frequency.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.384113 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_80/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.384226 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_80/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.384331 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_80/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.384429 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_80/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.384523 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_80/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.384689 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_80/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.384794 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_80/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.384889 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_80/src/main/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.535757 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_80/src/main/java/org/apache/commons/math/linear/
+-rw-r--r--   0 dgros      (501) staff       (20)    67167 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_80/src/main/java/org/apache/commons/math/linear/EigenDecompositionImpl.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.385177 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_80_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.385269 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_80_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.385368 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_80_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.385454 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_80_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.385538 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_80_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.385634 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_80_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.385739 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_80_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.385868 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_80_fixed/src/main/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.536301 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_80_fixed/src/main/java/org/apache/commons/math/linear/
+-rw-r--r--   0 dgros      (501) staff       (20)    67169 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_80_fixed/src/main/java/org/apache/commons/math/linear/EigenDecompositionImpl.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.386221 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_82/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.386322 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_82/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.386425 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_82/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.386536 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_82/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.386641 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_82/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.386798 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_82/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.386921 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_82/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.387020 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_82/src/main/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.387105 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_82/src/main/java/org/apache/commons/math/optimization/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.536804 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_82/src/main/java/org/apache/commons/math/optimization/linear/
+-rw-r--r--   0 dgros      (501) staff       (20)     7014 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_82/src/main/java/org/apache/commons/math/optimization/linear/SimplexSolver.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.387402 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_82_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.387491 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_82_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.387571 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_82_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.387658 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_82_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.387816 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_82_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.387912 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_82_fixed/src/main/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.388008 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_82_fixed/src/main/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.388101 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_82_fixed/src/main/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.388189 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_82_fixed/src/main/java/org/apache/commons/math/optimization/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.537155 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_82_fixed/src/main/java/org/apache/commons/math/optimization/linear/
+-rw-r--r--   0 dgros      (501) staff       (20)     7013 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_82_fixed/src/main/java/org/apache/commons/math/optimization/linear/SimplexSolver.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.388487 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_85/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.388583 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_85/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.388678 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_85/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.388773 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_85/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.388869 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_85/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.388959 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_85/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.389045 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_85/src/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.389130 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_85/src/java/org/apache/commons/math/analysis/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.537725 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_85/src/java/org/apache/commons/math/analysis/solvers/
+-rw-r--r--   0 dgros      (501) staff       (20)    10247 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_85/src/java/org/apache/commons/math/analysis/solvers/UnivariateRealSolverUtils.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.389412 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_85_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.389490 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_85_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.389575 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_85_fixed/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.389669 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_85_fixed/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.389762 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_85_fixed/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.389870 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_85_fixed/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.389959 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_85_fixed/src/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.390052 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_85_fixed/src/java/org/apache/commons/math/analysis/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.538068 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_85_fixed/src/java/org/apache/commons/math/analysis/solvers/
+-rw-r--r--   0 dgros      (501) staff       (20)    10246 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_85_fixed/src/java/org/apache/commons/math/analysis/solvers/UnivariateRealSolverUtils.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.390332 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_94/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.390426 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_94/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.390511 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_94/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.390598 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_94/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.390700 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_94/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.390789 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_94/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.390983 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_94/src/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.538359 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_94/src/java/org/apache/commons/math/util/
+-rw-r--r--   0 dgros      (501) staff       (20)    37123 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_94/src/java/org/apache/commons/math/util/MathUtils.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.391289 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_94_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.391377 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_94_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.391456 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_94_fixed/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.391538 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_94_fixed/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.391640 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_94_fixed/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.391747 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_94_fixed/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.391874 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_94_fixed/src/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.539131 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_94_fixed/src/java/org/apache/commons/math/util/
+-rw-r--r--   0 dgros      (501) staff       (20)    37133 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_94_fixed/src/java/org/apache/commons/math/util/MathUtils.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.392403 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_96/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.392501 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_96/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.392598 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_96/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.392691 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_96/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.392776 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_96/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.392880 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_96/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.392988 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_96/src/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.539555 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_96/src/java/org/apache/commons/math/complex/
+-rw-r--r--   0 dgros      (501) staff       (20)    31194 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_96/src/java/org/apache/commons/math/complex/Complex.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.393336 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_96_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.393452 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_96_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.393555 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_96_fixed/src/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.393657 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_96_fixed/src/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.393748 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_96_fixed/src/java/org/apache/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.393857 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_96_fixed/src/java/org/apache/commons/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.393965 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_96_fixed/src/java/org/apache/commons/math/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.540112 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_96_fixed/src/java/org/apache/commons/math/complex/
+-rw-r--r--   0 dgros      (501) staff       (20)    31072 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Math_96_fixed/src/java/org/apache/commons/math/complex/Complex.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.394289 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_24/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.394380 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_24/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.394480 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_24/src/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.394581 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_24/src/org/mockito/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.394689 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_24/src/org/mockito/internal/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.394789 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_24/src/org/mockito/internal/stubbing/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.540520 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_24/src/org/mockito/internal/stubbing/defaultanswers/
+-rw-r--r--   0 dgros      (501) staff       (20)     4666 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_24/src/org/mockito/internal/stubbing/defaultanswers/ReturnsEmptyValues.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.395068 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_24_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.395154 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_24_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.395242 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_24_fixed/src/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.395339 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_24_fixed/src/org/mockito/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.395440 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_24_fixed/src/org/mockito/internal/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.395537 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_24_fixed/src/org/mockito/internal/stubbing/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.540848 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_24_fixed/src/org/mockito/internal/stubbing/defaultanswers/
+-rw-r--r--   0 dgros      (501) staff       (20)     4725 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_24_fixed/src/org/mockito/internal/stubbing/defaultanswers/ReturnsEmptyValues.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.395824 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_26/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.395917 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_26/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.396021 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_26/src/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.396113 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_26/src/org/mockito/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.396300 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_26/src/org/mockito/internal/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.541180 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_26/src/org/mockito/internal/util/
+-rw-r--r--   0 dgros      (501) staff       (20)     2593 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_26/src/org/mockito/internal/util/Primitives.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.396660 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_26_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.396771 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_26_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.396875 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_26_fixed/src/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.396979 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_26_fixed/src/org/mockito/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.397073 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_26_fixed/src/org/mockito/internal/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.541472 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_26_fixed/src/org/mockito/internal/util/
+-rw-r--r--   0 dgros      (501) staff       (20)     2594 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_26_fixed/src/org/mockito/internal/util/Primitives.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.397459 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_29/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.397555 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_29/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.397658 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_29/src/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.397743 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_29/src/org/mockito/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.397827 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_29/src/org/mockito/internal/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.541960 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_29/src/org/mockito/internal/matchers/
+-rw-r--r--   0 dgros      (501) staff       (20)     1109 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_29/src/org/mockito/internal/matchers/Same.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.398090 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_29_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.398174 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_29_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.398257 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_29_fixed/src/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.398349 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_29_fixed/src/org/mockito/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.398426 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_29_fixed/src/org/mockito/internal/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.542326 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_29_fixed/src/org/mockito/internal/matchers/
+-rw-r--r--   0 dgros      (501) staff       (20)     1135 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_29_fixed/src/org/mockito/internal/matchers/Same.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.398656 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_34/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.398719 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_34/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.398780 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_34/src/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.398845 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_34/src/org/mockito/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.398929 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_34/src/org/mockito/internal/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.543250 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_34/src/org/mockito/internal/invocation/
+-rw-r--r--   0 dgros      (501) staff       (20)     3658 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_34/src/org/mockito/internal/invocation/InvocationMatcher.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.399176 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_34_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.399257 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_34_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.399342 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_34_fixed/src/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.399427 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_34_fixed/src/org/mockito/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.399518 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_34_fixed/src/org/mockito/internal/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.543734 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_34_fixed/src/org/mockito/internal/invocation/
+-rw-r--r--   0 dgros      (501) staff       (20)     3689 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_34_fixed/src/org/mockito/internal/invocation/InvocationMatcher.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.399815 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_38/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.399918 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_38/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.400014 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_38/src/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.400114 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_38/src/org/mockito/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.400217 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_38/src/org/mockito/internal/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.400327 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_38/src/org/mockito/internal/verification/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.544038 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_38/src/org/mockito/internal/verification/argumentmatching/
+-rw-r--r--   0 dgros      (501) staff       (20)     1681 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_38/src/org/mockito/internal/verification/argumentmatching/ArgumentMatchingTool.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.400659 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_38_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.400765 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_38_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.400868 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_38_fixed/src/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.400976 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_38_fixed/src/org/mockito/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.401078 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_38_fixed/src/org/mockito/internal/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.401149 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_38_fixed/src/org/mockito/internal/verification/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.544454 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_38_fixed/src/org/mockito/internal/verification/argumentmatching/
+-rw-r--r--   0 dgros      (501) staff       (20)     1703 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_38_fixed/src/org/mockito/internal/verification/argumentmatching/ArgumentMatchingTool.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.401389 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_5/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.401470 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_5/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.401550 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_5/src/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.401639 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_5/src/org/mockito/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.401724 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_5/src/org/mockito/internal/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.545013 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_5/src/org/mockito/internal/verification/
+-rw-r--r--   0 dgros      (501) staff       (20)     5925 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_5/src/org/mockito/internal/verification/VerificationOverTimeImpl.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.401981 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_5_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.402063 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_5_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.402135 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_5_fixed/src/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.402207 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_5_fixed/src/org/mockito/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.402272 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_5_fixed/src/org/mockito/internal/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.545722 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_5_fixed/src/org/mockito/internal/verification/
+-rw-r--r--   0 dgros      (501) staff       (20)     5876 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_5_fixed/src/org/mockito/internal/verification/VerificationOverTimeImpl.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.402517 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_8/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.402603 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_8/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.402691 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_8/src/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.402773 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_8/src/org/mockito/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.402855 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_8/src/org/mockito/internal/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.403438 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_8/src/org/mockito/internal/util/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.546071 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_8/src/org/mockito/internal/util/reflection/
+-rw-r--r--   0 dgros      (501) staff       (20)    25373 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_8/src/org/mockito/internal/util/reflection/GenericMetadataSupport.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.403722 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_8_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.403803 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_8_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.415464 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_8_fixed/src/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.415673 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_8_fixed/src/org/mockito/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.415781 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_8_fixed/src/org/mockito/internal/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.415883 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_8_fixed/src/org/mockito/internal/util/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.547116 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_8_fixed/src/org/mockito/internal/util/reflection/
+-rw-r--r--   0 dgros      (501) staff       (20)    25414 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Mockito_8_fixed/src/org/mockito/internal/util/reflection/GenericMetadataSupport.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.416288 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_16/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.416394 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_16/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.416515 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_16/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.416623 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_16/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.416763 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_16/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.416879 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_16/src/main/java/org/joda/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.416982 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_16/src/main/java/org/joda/time/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.547558 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_16/src/main/java/org/joda/time/format/
+-rw-r--r--   0 dgros      (501) staff       (20)    37325 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_16/src/main/java/org/joda/time/format/DateTimeFormatter.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.417296 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_16_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.417394 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_16_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.417492 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_16_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.417579 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_16_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.417677 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_16_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.417791 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_16_fixed/src/main/java/org/joda/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.417886 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_16_fixed/src/main/java/org/joda/time/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.548175 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_16_fixed/src/main/java/org/joda/time/format/
+-rw-r--r--   0 dgros      (501) staff       (20)    37344 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_16_fixed/src/main/java/org/joda/time/format/DateTimeFormatter.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.418186 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_19/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.418281 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_19/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.418362 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_19/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.418446 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_19/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.418528 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_19/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.418611 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_19/src/main/java/org/joda/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.548503 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_19/src/main/java/org/joda/time/
+-rw-r--r--   0 dgros      (501) staff       (20)    49694 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_19/src/main/java/org/joda/time/DateTimeZone.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.418879 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_19_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.418972 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_19_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.419059 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_19_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.419142 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_19_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.419225 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_19_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.419313 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_19_fixed/src/main/java/org/joda/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.548892 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_19_fixed/src/main/java/org/joda/time/
+-rw-r--r--   0 dgros      (501) staff       (20)    49695 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_19_fixed/src/main/java/org/joda/time/DateTimeZone.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.419575 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_4/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.419667 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_4/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.419761 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_4/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.419849 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_4/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.419933 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_4/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.420024 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_4/src/main/java/org/joda/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.549209 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_4/src/main/java/org/joda/time/
+-rw-r--r--   0 dgros      (501) staff       (20)    38976 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_4/src/main/java/org/joda/time/Partial.java
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.420306 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_4_fixed/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.420401 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_4_fixed/src/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.420489 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_4_fixed/src/main/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.420590 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_4_fixed/src/main/java/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.420690 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_4_fixed/src/main/java/org/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.420781 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_4_fixed/src/main/java/org/joda/
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.549498 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_4_fixed/src/main/java/org/joda/time/
+-rw-r--r--   0 dgros      (501) staff       (20)    38976 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Defects4J_projects_clean/Time_4_fixed/src/main/java/org/joda/time/Partial.java
+-rw-r--r--   0 dgros      (501) staff       (20)     1805 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/Dockerfile
+-rw-r--r--   0 dgros      (501) staff       (20)     1493 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/README.md
+-rw-r--r--   0 dgros      (501) staff       (20)      912 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/dataset.py
+-rw-r--r--   0 dgros      (501) staff       (20)    19341 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/defects4j.build.xml
+-rw-r--r--   0 dgros      (501) staff       (20)    14296 2024-03-17 08:36:57.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/defects4j_script.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1365 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/projcleanup.py
+-rw-r--r--   0 dgros      (501) staff       (20)     9042 2024-03-21 03:32:15.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/dypybench.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.550148 synthegrator-0.9.3.6/synthegrator/synthdatasets/dypybench_data/
+-rw-r--r--   0 dgros      (501) staff       (20)      486 2024-03-16 23:08:47.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/dypybench_data/dypybench_setup.md
+-rw-r--r--   0 dgros      (501) staff       (20)  1721994 2024-03-22 00:34:23.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/dypybench_data/func_dataset_subset.parquet
+-rw-r--r--   0 dgros      (501) staff       (20)     4274 2024-03-20 06:32:16.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/human_eval.py
+-rw-r--r--   0 dgros      (501) staff       (20)      436 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/humxplay.py
+-rw-r--r--   0 dgros      (501) staff       (20)    15796 2024-03-16 23:08:47.000000 synthegrator-0.9.3.6/synthegrator/synthdatasets/mbpp.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.552558 synthegrator-0.9.3.6/synthegrator/tests/
+-rw-r--r--   0 dgros      (501) staff       (20)        0 2023-06-07 15:22:25.000000 synthegrator-0.9.3.6/synthegrator/tests/__init__.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.566384 synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/
+-rw-r--r--   0 dgros      (501) staff       (20)        0 2023-10-19 06:45:25.000000 synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/__init__.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1011 2023-10-19 06:45:25.000000 synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_code_problem.py
+-rw-r--r--   0 dgros      (501) staff       (20)    26073 2024-03-22 00:38:03.000000 synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_code_solver.py
+-rw-r--r--   0 dgros      (501) staff       (20)     2095 2024-02-21 20:24:16.000000 synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_df_converters.py
+-rw-r--r--   0 dgros      (501) staff       (20)     3283 2024-03-16 23:08:47.000000 synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_environments.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1311 2024-01-31 01:30:33.000000 synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_examples.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1382 2024-03-23 01:20:01.000000 synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_few_shot_library.py
+-rw-r--r--   0 dgros      (501) staff       (20)     8604 2024-03-21 19:45:20.000000 synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_java_stuff.py
+-rw-r--r--   0 dgros      (501) staff       (20)     5090 2023-10-19 06:45:25.000000 synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_lang_spec.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1877 2024-03-16 23:08:47.000000 synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_line_str.py
+-rw-r--r--   0 dgros      (501) staff       (20)     4537 2023-10-19 06:45:25.000000 synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_parsing.py
+-rw-r--r--   0 dgros      (501) staff       (20)     9252 2024-03-22 00:38:03.000000 synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_problem_rendering.py
+-rw-r--r--   0 dgros      (501) staff       (20)     5703 2024-03-21 03:32:15.000000 synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_problem_rendering_insertion_tags.py
+-rw-r--r--   0 dgros      (501) staff       (20)     4716 2023-10-19 06:45:25.000000 synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_sandboxing.py
+-rw-r--r--   0 dgros      (501) staff       (20)    18713 2024-04-24 02:16:05.000000 synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_solution_eval.py
+-rw-r--r--   0 dgros      (501) staff       (20)    15134 2024-03-17 08:36:57.000000 synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_transformation_spec.py
+-rw-r--r--   0 dgros      (501) staff       (20)     2105 2024-03-17 08:36:57.000000 synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_util.py
+-rw-r--r--   0 dgros      (501) staff       (20)    13215 2024-03-19 09:14:42.000000 synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_value_question_render.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.568323 synthegrator-0.9.3.6/synthegrator/tests/x_datasets_tests/
+-rw-r--r--   0 dgros      (501) staff       (20)        0 2023-10-19 06:45:25.000000 synthegrator-0.9.3.6/synthegrator/tests/x_datasets_tests/__init__.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.569424 synthegrator-0.9.3.6/synthegrator/tests/x_datasets_tests/fixtures/
+-rw-r--r--   0 dgros      (501) staff       (20)    25660 2023-10-19 06:45:25.000000 synthegrator-0.9.3.6/synthegrator/tests/x_datasets_tests/fixtures/broken_document.py.fixture
+-rw-r--r--   0 dgros      (501) staff       (20)    26309 2023-10-19 06:45:25.000000 synthegrator-0.9.3.6/synthegrator/tests/x_datasets_tests/fixtures/document.py.fixture
+-rw-r--r--   0 dgros      (501) staff       (20)     1873 2024-03-16 23:08:47.000000 synthegrator-0.9.3.6/synthegrator/tests/x_datasets_tests/test_human_eval.py
+-rw-r--r--   0 dgros      (501) staff       (20)      749 2023-10-19 06:45:25.000000 synthegrator-0.9.3.6/synthegrator/tests/x_datasets_tests/test_x_apps.py
+-rw-r--r--   0 dgros      (501) staff       (20)     7878 2024-02-22 00:28:05.000000 synthegrator-0.9.3.6/synthegrator/tests/x_datasets_tests/test_x_mbpp.py
+-rw-r--r--   0 dgros      (501) staff       (20)     8407 2024-04-24 01:39:02.000000 synthegrator-0.9.3.6/synthegrator/tests/x_datasets_tests/test_xx_defects4j.py
+-rw-r--r--   0 dgros      (501) staff       (20)    23956 2024-04-24 02:16:05.000000 synthegrator-0.9.3.6/synthegrator/tests/x_datasets_tests/test_xx_dypybench.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1169 2024-03-17 08:37:58.000000 synthegrator-0.9.3.6/synthegrator/toytest.py
+-rw-r--r--   0 dgros      (501) staff       (20)    37291 2024-04-11 20:07:27.000000 synthegrator-0.9.3.6/synthegrator/transformation_spec.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1199 2023-10-04 00:58:52.000000 synthegrator-0.9.3.6/synthegrator/uncertainty_modeling.py
+-rw-r--r--   0 dgros      (501) staff       (20)    12278 2024-03-20 20:00:19.000000 synthegrator-0.9.3.6/synthegrator/util.py
+-rw-r--r--   0 dgros      (501) staff       (20)      416 2024-04-24 20:32:49.000000 synthegrator-0.9.3.6/synthegrator/version.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-24 20:32:50.570039 synthegrator-0.9.3.6/synthegrator.egg-info/
+-rw-r--r--   0 dgros      (501) staff       (20)     4602 2024-04-24 20:32:49.000000 synthegrator-0.9.3.6/synthegrator.egg-info/PKG-INFO
+-rw-r--r--   0 dgros      (501) staff       (20)    37958 2024-04-24 20:32:50.000000 synthegrator-0.9.3.6/synthegrator.egg-info/SOURCES.txt
+-rw-r--r--   0 dgros      (501) staff       (20)        1 2024-04-24 20:32:49.000000 synthegrator-0.9.3.6/synthegrator.egg-info/dependency_links.txt
+-rw-r--r--   0 dgros      (501) staff       (20)      370 2024-04-24 20:32:49.000000 synthegrator-0.9.3.6/synthegrator.egg-info/requires.txt
+-rw-r--r--   0 dgros      (501) staff       (20)       13 2024-04-24 20:32:49.000000 synthegrator-0.9.3.6/synthegrator.egg-info/top_level.txt
```

### Comparing `synthegrator-0.9.3.5/LICENSE` & `synthegrator-0.9.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/PKG-INFO` & `synthegrator-0.9.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthegrator
-Version: 0.9.3.5
+Version: 0.9.3.6
 Summary: Framework for code synthesis and AI4SE research
 Author-email: David Gros <DNGros@users.noreply.github.com>, Claudio Spiess <claudiosv@users.noreply.github.com>
 License: Copyright 2024 David Gros, Claudio Spiess
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -41,15 +41,15 @@
 # Synthegrator
 
 Synthegrator is a framework for code generation problems. It simplifies
 the process of loading common datasets and solving them with language models.
 
 # Installation
 ```bash
-pip install "synthegrator @ git+https://github.com/DaiseyCode/Synthegrator.git"
+pip install synthegrator
 ```
 
 Also, for execution you will need to [install docker](https://docs.docker.com/engine/install/).
 
 
 # Example
 Let's take a look at an example of how we can run a solver over
```

### Comparing `synthegrator-0.9.3.5/README.md` & `synthegrator-0.9.3.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Synthegrator
 
 Synthegrator is a framework for code generation problems. It simplifies
 the process of loading common datasets and solving them with language models.
 
 # Installation
 ```bash
-pip install "synthegrator @ git+https://github.com/DaiseyCode/Synthegrator.git"
+pip install synthegrator
 ```
 
 Also, for execution you will need to [install docker](https://docs.docker.com/engine/install/).
 
 
 # Example
 Let's take a look at an example of how we can run a solver over
```

### Comparing `synthegrator-0.9.3.5/pyproject.toml` & `synthegrator-0.9.3.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 [build-system]
-requires      = ["setuptools>=68.2.2"]
+requires      = ["setuptools>=68.2.2", "setuptools-scm>=6.3.2"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["."]  # Adjust if your packages are located in a subdirectory, e.g., "src".
 include = ["synthegrator*"]  # This pattern includes your main package and any subpackages or modules within it.
 
 [tool.pytest]
 python_classes = "ClassNamesAreIgnoredToNotConflictWithSynthegratorClasses"
 
+[tool.setuptools_scm]
+# Optional: Write the version number into your package's __init__.py as __version__
+write_to = "synthegrator/version.py"
+
 [project]
 name = "synthegrator"
-version = "0.9.3.5"
+version = "0.9.3.6"
 authors = [
     { name = "David Gros", email = "DNGros@users.noreply.github.com" },
     { name = "Claudio Spiess", email = "claudiosv@users.noreply.github.com" },
 ]
 description = "Framework for code synthesis and AI4SE research"
 license = { file = "LICENSE" }
 readme = "README.md"
```

### Comparing `synthegrator-0.9.3.5/synthegrator/_vendor/epicbox/config.py` & `synthegrator-0.9.3.6/synthegrator/_vendor/epicbox/config.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/_vendor/epicbox/sandboxes.py` & `synthegrator-0.9.3.6/synthegrator/_vendor/epicbox/sandboxes.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/_vendor/epicbox/utils.py` & `synthegrator-0.9.3.6/synthegrator/_vendor/epicbox/utils.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/code_problem_builders.py` & `synthegrator-0.9.3.6/synthegrator/code_problem_builders.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/code_problems.py` & `synthegrator-0.9.3.6/synthegrator/code_problems.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/code_solver.py` & `synthegrator-0.9.3.6/synthegrator/code_solver.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/df_converters.py` & `synthegrator-0.9.3.6/synthegrator/df_converters.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/execution_threading.py` & `synthegrator-0.9.3.6/synthegrator/execution_threading.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/few_shotting.py` & `synthegrator-0.9.3.6/synthegrator/few_shotting.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/human_eval/evaluation.py` & `synthegrator-0.9.3.6/synthegrator/human_eval/evaluation.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/human_eval/execution.py` & `synthegrator-0.9.3.6/synthegrator/human_eval/execution.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/lang_specs/lang_spec.py` & `synthegrator-0.9.3.6/synthegrator/lang_specs/lang_spec.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/lang_specs/lang_spec_java.py` & `synthegrator-0.9.3.6/synthegrator/lang_specs/lang_spec_java.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/lang_specs/lang_spec_python.py` & `synthegrator-0.9.3.6/synthegrator/lang_specs/lang_spec_python.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/lang_specs/lang_util.py` & `synthegrator-0.9.3.6/synthegrator/lang_specs/lang_util.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/lm_few_shotting_tools.py` & `synthegrator-0.9.3.6/synthegrator/lm_few_shotting_tools.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/memory_fs.py` & `synthegrator-0.9.3.6/synthegrator/memory_fs.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/problem_rendering.py` & `synthegrator-0.9.3.6/synthegrator/problem_rendering.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/problem_rendering_insertion_tags.py` & `synthegrator-0.9.3.6/synthegrator/problem_rendering_insertion_tags.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/prompt_renderer_questions.py` & `synthegrator-0.9.3.6/synthegrator/prompt_renderer_questions.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/prompting_test_case_selection.py` & `synthegrator-0.9.3.6/synthegrator/prompting_test_case_selection.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/response_parser.py` & `synthegrator-0.9.3.6/synthegrator/response_parser.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/sandboxing.py` & `synthegrator-0.9.3.6/synthegrator/sandboxing.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/solution_eval.py` & `synthegrator-0.9.3.6/synthegrator/solution_eval.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/synthdatasets/apps.py` & `synthegrator-0.9.3.6/synthegrator/synthdatasets/apps.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/synthdatasets/defects4j.py` & `synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/synthdatasets/defects4j_data/dataset.py` & `synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/dataset.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/synthdatasets/defects4j_data/defects4j_script.py` & `synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/defects4j_script.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/synthdatasets/defects4j_data/projcleanup.py` & `synthegrator-0.9.3.6/synthegrator/synthdatasets/defects4j_data/projcleanup.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/synthdatasets/dypybench.py` & `synthegrator-0.9.3.6/synthegrator/synthdatasets/dypybench.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/synthdatasets/human_eval.py` & `synthegrator-0.9.3.6/synthegrator/synthdatasets/human_eval.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/synthdatasets/mbpp.py` & `synthegrator-0.9.3.6/synthegrator/synthdatasets/mbpp.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_code_problem.py` & `synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_code_problem.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_code_solver.py` & `synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_code_solver.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_df_converters.py` & `synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_df_converters.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_environments.py` & `synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_examples.py` & `synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_few_shot_library.py` & `synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_few_shot_library.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_java_stuff.py` & `synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_java_stuff.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_lang_spec.py` & `synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_lang_spec.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_line_str.py` & `synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_line_str.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_parsing.py` & `synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_problem_rendering.py` & `synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_problem_rendering.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_problem_rendering_insertion_tags.py` & `synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_problem_rendering_insertion_tags.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_sandboxing.py` & `synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_sandboxing.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_solution_eval.py` & `synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_solution_eval.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_transformation_spec.py` & `synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_transformation_spec.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_util.py` & `synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_util.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/tests/non_dataset_tests/test_value_question_render.py` & `synthegrator-0.9.3.6/synthegrator/tests/non_dataset_tests/test_value_question_render.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/tests/x_datasets_tests/test_human_eval.py` & `synthegrator-0.9.3.6/synthegrator/tests/x_datasets_tests/test_human_eval.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/tests/x_datasets_tests/test_x_apps.py` & `synthegrator-0.9.3.6/synthegrator/tests/x_datasets_tests/test_x_apps.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/tests/x_datasets_tests/test_x_mbpp.py` & `synthegrator-0.9.3.6/synthegrator/tests/x_datasets_tests/test_x_mbpp.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/tests/x_datasets_tests/test_xx_defects4j.py` & `synthegrator-0.9.3.6/synthegrator/tests/x_datasets_tests/test_xx_defects4j.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/tests/x_datasets_tests/test_xx_dypybench.py` & `synthegrator-0.9.3.6/synthegrator/tests/x_datasets_tests/test_xx_dypybench.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/toytest.py` & `synthegrator-0.9.3.6/synthegrator/toytest.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/transformation_spec.py` & `synthegrator-0.9.3.6/synthegrator/transformation_spec.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/uncertainty_modeling.py` & `synthegrator-0.9.3.6/synthegrator/uncertainty_modeling.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator/util.py` & `synthegrator-0.9.3.6/synthegrator/util.py`

 * *Files identical despite different names*

### Comparing `synthegrator-0.9.3.5/synthegrator.egg-info/PKG-INFO` & `synthegrator-0.9.3.6/synthegrator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthegrator
-Version: 0.9.3.5
+Version: 0.9.3.6
 Summary: Framework for code synthesis and AI4SE research
 Author-email: David Gros <DNGros@users.noreply.github.com>, Claudio Spiess <claudiosv@users.noreply.github.com>
 License: Copyright 2024 David Gros, Claudio Spiess
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -41,15 +41,15 @@
 # Synthegrator
 
 Synthegrator is a framework for code generation problems. It simplifies
 the process of loading common datasets and solving them with language models.
 
 # Installation
 ```bash
-pip install "synthegrator @ git+https://github.com/DaiseyCode/Synthegrator.git"
+pip install synthegrator
 ```
 
 Also, for execution you will need to [install docker](https://docs.docker.com/engine/install/).
 
 
 # Example
 Let's take a look at an example of how we can run a solver over
```

