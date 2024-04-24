# Comparing `tmp/pypipr-1.0.90.tar.gz` & `tmp/pypipr-1.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypipr-1.0.90.tar", max compression
+gzip compressed data, was "pypipr-1.0.91.tar", max compression
```

## Comparing `pypipr-1.0.90.tar` & `pypipr-1.0.91.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     3347 2024-04-24 04:34:27.529174 pypipr-1.0.90/pypipr/__init__.py
--rw-r--r--   0        0        0     2229 2024-03-17 17:38:37.508083 pypipr-1.0.90/pypipr/ibuiltins/ComparePerformance.py
--rw-r--r--   0        0        0      100 2024-03-17 17:38:37.508083 pypipr-1.0.90/pypipr/ibuiltins/LINUX.py
--rw-r--r--   0        0        0     7358 2024-04-23 10:50:10.015024 pypipr-1.0.90/pypipr/ibuiltins/RunParallel.py
--rw-r--r--   0        0        0      105 2024-03-17 17:38:37.508083 pypipr-1.0.90/pypipr/ibuiltins/WINDOWS.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.508083 pypipr-1.0.90/pypipr/ibuiltins/__init__.py
--rw-r--r--   0        0        0      218 2024-03-17 17:38:37.508083 pypipr-1.0.90/pypipr/ibuiltins/avg.py
--rw-r--r--   0        0        0      194 2024-03-17 17:38:37.508083 pypipr-1.0.90/pypipr/ibuiltins/basename.py
--rw-r--r--   0        0        0      385 2024-04-22 13:19:16.948654 pypipr-1.0.90/pypipr/ibuiltins/chunk_array.py
--rw-r--r--   0        0        0      500 2024-03-17 17:38:37.508083 pypipr-1.0.90/pypipr/ibuiltins/create_folder.py
--rw-r--r--   0        0        0      466 2024-03-17 17:38:37.508083 pypipr-1.0.90/pypipr/ibuiltins/datetime_from_string.py
--rw-r--r--   0        0        0      476 2024-03-17 17:38:37.508083 pypipr-1.0.90/pypipr/ibuiltins/datetime_now.py
--rw-r--r--   0        0        0      377 2024-03-17 17:38:37.508083 pypipr-1.0.90/pypipr/ibuiltins/dict_first.py
--rw-r--r--   0        0        0      229 2024-03-17 17:38:37.508083 pypipr-1.0.90/pypipr/ibuiltins/dirname.py
--rw-r--r--   0        0        0      321 2024-04-20 11:53:09.914721 pypipr-1.0.90/pypipr/ibuiltins/exit_if_empty.py
--rw-r--r--   0        0        0      543 2024-03-17 17:38:37.508083 pypipr-1.0.90/pypipr/ibuiltins/filter_empty.py
--rw-r--r--   0        0        0      335 2024-04-23 12:23:59.246031 pypipr-1.0.90/pypipr/ibuiltins/get_by_index.py
--rw-r--r--   0        0        0      639 2024-04-22 21:58:29.290425 pypipr-1.0.90/pypipr/ibuiltins/get_class_method.py
--rw-r--r--   0        0        0      227 2024-03-17 17:38:37.508083 pypipr-1.0.90/pypipr/ibuiltins/get_filemtime.py
--rw-r--r--   0        0        0      196 2024-03-17 17:38:37.508083 pypipr-1.0.90/pypipr/ibuiltins/get_filesize.py
--rw-r--r--   0        0        0      683 2024-04-20 11:02:21.923096 pypipr-1.0.90/pypipr/ibuiltins/is_empty.py
--rw-r--r--   0        0        0      922 2024-03-17 17:38:37.508083 pypipr-1.0.90/pypipr/ibuiltins/is_iterable.py
--rw-r--r--   0        0        0     1008 2024-03-17 17:38:37.508083 pypipr-1.0.90/pypipr/ibuiltins/is_valid_url.py
--rw-r--r--   0        0        0      899 2024-04-23 09:16:42.841403 pypipr-1.0.90/pypipr/ibuiltins/ivars.py
--rw-r--r--   0        0        0      496 2024-03-17 17:38:37.508083 pypipr-1.0.90/pypipr/ibuiltins/password_generator.py
--rw-r--r--   0        0        0      405 2024-03-17 17:38:37.508083 pypipr-1.0.90/pypipr/ibuiltins/random_bool.py
--rw-r--r--   0        0        0      698 2024-03-17 17:38:37.512083 pypipr-1.0.90/pypipr/ibuiltins/set_timeout.py
--rw-r--r--   0        0        0      325 2024-03-17 17:38:37.512083 pypipr-1.0.90/pypipr/ibuiltins/sets_ordered.py
--rw-r--r--   0        0        0      377 2024-03-17 17:38:37.512083 pypipr-1.0.90/pypipr/ibuiltins/str_cmp.py
--rw-r--r--   0        0        0      597 2024-03-17 17:38:37.512083 pypipr-1.0.90/pypipr/ibuiltins/to_str.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.90/pypipr/iconsole/__init__.py
--rw-r--r--   0        0        0     1686 2024-03-17 17:38:37.512083 pypipr-1.0.90/pypipr/iconsole/choices.py
--rw-r--r--   0        0        0      525 2024-03-17 17:38:37.512083 pypipr-1.0.90/pypipr/iconsole/console_run.py
--rw-r--r--   0        0        0     1030 2024-04-23 12:02:12.950032 pypipr-1.0.90/pypipr/iconsole/input_char.py
--rw-r--r--   0        0        0     1041 2024-03-17 17:38:37.512083 pypipr-1.0.90/pypipr/iconsole/log.py
--rw-r--r--   0        0        0      474 2024-03-17 17:38:37.512083 pypipr-1.0.90/pypipr/iconsole/print_colorize.py
--rw-r--r--   0        0        0      930 2024-04-22 21:43:34.984645 pypipr-1.0.90/pypipr/iconsole/print_dir.py
--rw-r--r--   0        0        0      282 2024-04-22 21:44:47.788645 pypipr-1.0.90/pypipr/iconsole/print_log.py
--rw-r--r--   0        0        0      914 2024-04-24 02:48:07.180538 pypipr-1.0.90/pypipr/iconsole/print_to_last_line.py
--rw-r--r--   0        0        0      396 2024-03-17 17:38:37.512083 pypipr-1.0.90/pypipr/iconsole/text_colorize.py
--rw-r--r--   0        0        0     1093 2024-03-17 17:38:37.512083 pypipr-1.0.90/pypipr/idjango/APIMixinView.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.90/pypipr/idjango/__init__.py
--rw-r--r--   0        0        0      222 2024-03-17 17:38:37.512083 pypipr-1.0.90/pypipr/iengineering/PintUreg.py
--rw-r--r--   0        0        0      118 2024-03-17 17:38:37.512083 pypipr-1.0.90/pypipr/iengineering/PintUregQuantity.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.90/pypipr/iengineering/__init__.py
--rw-r--r--   0        0        0      695 2024-04-22 21:59:57.598425 pypipr-1.0.90/pypipr/iengineering/batch_calculate.py
--rw-r--r--   0        0        0     1277 2024-03-17 17:38:37.512083 pypipr-1.0.90/pypipr/iengineering/batchmaker.py
--rw-r--r--   0        0        0      805 2024-03-17 17:38:37.512083 pypipr-1.0.90/pypipr/iengineering/calculate.py
--rw-r--r--   0        0        0      966 2024-04-23 11:50:40.860964 pypipr-1.0.90/pypipr/iflow/auto_reload.py
--rw-r--r--   0        0        0      243 2024-03-17 17:38:37.516083 pypipr-1.0.90/pypipr/iflow/github_pull.py
--rw-r--r--   0        0        0      951 2024-03-17 17:38:37.516083 pypipr-1.0.90/pypipr/iflow/github_push.py
--rw-r--r--   0        0        0      600 2024-03-17 17:38:37.516083 pypipr-1.0.90/pypipr/iflow/github_user.py
--rw-r--r--   0        0        0      839 2024-04-20 02:24:51.624107 pypipr-1.0.90/pypipr/iflow/pip_freeze_without_version.py
--rw-r--r--   0        0        0      409 2024-03-17 17:38:37.516083 pypipr-1.0.90/pypipr/iflow/poetry_publish.py
--rw-r--r--   0        0        0      622 2024-03-17 17:38:37.516083 pypipr-1.0.90/pypipr/iflow/poetry_update_version.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.516083 pypipr-1.0.90/pypipr/ifunctions/__init__.py
--rw-r--r--   0        0        0      503 2024-04-23 11:45:29.548964 pypipr-1.0.90/pypipr/ifunctions/iargv.py
--rw-r--r--   0        0        0      748 2024-03-17 17:38:37.516083 pypipr-1.0.90/pypipr/ifunctions/idumps.py
--rw-r--r--   0        0        0     1423 2024-03-17 17:38:37.516083 pypipr-1.0.90/pypipr/ifunctions/idumps_html.py
--rw-r--r--   0        0        0      679 2024-04-23 11:41:52.328964 pypipr-1.0.90/pypipr/ifunctions/ienv.py
--rw-r--r--   0        0        0      465 2024-03-17 17:38:37.516083 pypipr-1.0.90/pypipr/ifunctions/iexec.py
--rw-r--r--   0        0        0     2069 2024-03-17 17:38:37.516083 pypipr-1.0.90/pypipr/ifunctions/ijoin.py
--rw-r--r--   0        0        0      638 2024-04-22 21:36:07.164645 pypipr-1.0.90/pypipr/ifunctions/iloads.py
--rw-r--r--   0        0        0     4146 2024-04-22 21:40:17.264645 pypipr-1.0.90/pypipr/ifunctions/iloads_html.py
--rw-r--r--   0        0        0     2808 2024-03-17 17:38:37.516083 pypipr-1.0.90/pypipr/ifunctions/iopen.py
--rw-r--r--   0        0        0      849 2024-04-22 21:41:31.764645 pypipr-1.0.90/pypipr/ifunctions/iprint.py
--rw-r--r--   0        0        0     2407 2024-03-17 17:38:37.516083 pypipr-1.0.90/pypipr/ifunctions/irange.py
--rw-r--r--   0        0        0      722 2024-03-17 17:38:37.516083 pypipr-1.0.90/pypipr/ifunctions/ireplace.py
--rw-r--r--   0        0        0      748 2024-04-23 09:11:14.125403 pypipr-1.0.90/pypipr/ifunctions/iscandir.py
--rw-r--r--   0        0        0      383 2024-03-17 17:38:37.520083 pypipr-1.0.90/pypipr/ifunctions/isplit.py
--rw-r--r--   0        0        0     1061 2024-04-20 02:38:18.131451 pypipr-1.0.90/pypipr/pypipr.py.bak
--rw-r--r--   0        0        0     1800 2024-04-23 13:05:42.093603 pypipr-1.0.90/pypipr/terminal.py
--rw-r--r--   0        0        0      544 2024-04-24 04:34:38.101174 pypipr-1.0.90/pyproject.toml
--rw-r--r--   0        0        0   149197 2024-04-24 04:34:31.705174 pypipr-1.0.90/readme.md
--rw-r--r--   0        0        0   149883 1970-01-01 00:00:00.000000 pypipr-1.0.90/PKG-INFO
+-rw-r--r--   0        0        0     3347 2024-04-24 04:39:24.109174 pypipr-1.0.91/pypipr/__init__.py
+-rw-r--r--   0        0        0     2229 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/ComparePerformance.py
+-rw-r--r--   0        0        0      100 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/LINUX.py
+-rw-r--r--   0        0        0     7358 2024-04-23 10:50:10.015024 pypipr-1.0.91/pypipr/ibuiltins/RunParallel.py
+-rw-r--r--   0        0        0      105 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/WINDOWS.py
+-rw-r--r--   0        0        0        0 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/__init__.py
+-rw-r--r--   0        0        0      218 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/avg.py
+-rw-r--r--   0        0        0      194 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/basename.py
+-rw-r--r--   0        0        0      385 2024-04-22 13:19:16.948654 pypipr-1.0.91/pypipr/ibuiltins/chunk_array.py
+-rw-r--r--   0        0        0      500 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/create_folder.py
+-rw-r--r--   0        0        0      466 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/datetime_from_string.py
+-rw-r--r--   0        0        0      476 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/datetime_now.py
+-rw-r--r--   0        0        0      377 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/dict_first.py
+-rw-r--r--   0        0        0      229 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/dirname.py
+-rw-r--r--   0        0        0      321 2024-04-20 11:53:09.914721 pypipr-1.0.91/pypipr/ibuiltins/exit_if_empty.py
+-rw-r--r--   0        0        0      543 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/filter_empty.py
+-rw-r--r--   0        0        0      335 2024-04-23 12:23:59.246031 pypipr-1.0.91/pypipr/ibuiltins/get_by_index.py
+-rw-r--r--   0        0        0      639 2024-04-22 21:58:29.290425 pypipr-1.0.91/pypipr/ibuiltins/get_class_method.py
+-rw-r--r--   0        0        0      227 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/get_filemtime.py
+-rw-r--r--   0        0        0      196 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/get_filesize.py
+-rw-r--r--   0        0        0      683 2024-04-20 11:02:21.923096 pypipr-1.0.91/pypipr/ibuiltins/is_empty.py
+-rw-r--r--   0        0        0      922 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/is_iterable.py
+-rw-r--r--   0        0        0     1008 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/is_valid_url.py
+-rw-r--r--   0        0        0      899 2024-04-23 09:16:42.841403 pypipr-1.0.91/pypipr/ibuiltins/ivars.py
+-rw-r--r--   0        0        0      496 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/password_generator.py
+-rw-r--r--   0        0        0      405 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/random_bool.py
+-rw-r--r--   0        0        0      698 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/ibuiltins/set_timeout.py
+-rw-r--r--   0        0        0      325 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/ibuiltins/sets_ordered.py
+-rw-r--r--   0        0        0      377 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/ibuiltins/str_cmp.py
+-rw-r--r--   0        0        0      597 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/ibuiltins/to_str.py
+-rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/iconsole/__init__.py
+-rw-r--r--   0        0        0     1686 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/iconsole/choices.py
+-rw-r--r--   0        0        0      525 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/iconsole/console_run.py
+-rw-r--r--   0        0        0     1030 2024-04-23 12:02:12.950032 pypipr-1.0.91/pypipr/iconsole/input_char.py
+-rw-r--r--   0        0        0     1041 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/iconsole/log.py
+-rw-r--r--   0        0        0      474 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/iconsole/print_colorize.py
+-rw-r--r--   0        0        0      930 2024-04-22 21:43:34.984645 pypipr-1.0.91/pypipr/iconsole/print_dir.py
+-rw-r--r--   0        0        0      282 2024-04-22 21:44:47.788645 pypipr-1.0.91/pypipr/iconsole/print_log.py
+-rw-r--r--   0        0        0      914 2024-04-24 02:48:07.180538 pypipr-1.0.91/pypipr/iconsole/print_to_last_line.py
+-rw-r--r--   0        0        0      396 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/iconsole/text_colorize.py
+-rw-r--r--   0        0        0     1093 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/idjango/APIMixinView.py
+-rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/idjango/__init__.py
+-rw-r--r--   0        0        0      222 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/iengineering/PintUreg.py
+-rw-r--r--   0        0        0      118 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/iengineering/PintUregQuantity.py
+-rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/iengineering/__init__.py
+-rw-r--r--   0        0        0      695 2024-04-22 21:59:57.598425 pypipr-1.0.91/pypipr/iengineering/batch_calculate.py
+-rw-r--r--   0        0        0     1277 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/iengineering/batchmaker.py
+-rw-r--r--   0        0        0      805 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/iengineering/calculate.py
+-rw-r--r--   0        0        0      966 2024-04-23 11:50:40.860964 pypipr-1.0.91/pypipr/iflow/auto_reload.py
+-rw-r--r--   0        0        0      243 2024-03-17 17:38:37.516083 pypipr-1.0.91/pypipr/iflow/github_pull.py
+-rw-r--r--   0        0        0      951 2024-03-17 17:38:37.516083 pypipr-1.0.91/pypipr/iflow/github_push.py
+-rw-r--r--   0        0        0      600 2024-03-17 17:38:37.516083 pypipr-1.0.91/pypipr/iflow/github_user.py
+-rw-r--r--   0        0        0      839 2024-04-20 02:24:51.624107 pypipr-1.0.91/pypipr/iflow/pip_freeze_without_version.py
+-rw-r--r--   0        0        0      409 2024-03-17 17:38:37.516083 pypipr-1.0.91/pypipr/iflow/poetry_publish.py
+-rw-r--r--   0        0        0      622 2024-03-17 17:38:37.516083 pypipr-1.0.91/pypipr/iflow/poetry_update_version.py
+-rw-r--r--   0        0        0        0 2024-03-17 17:38:37.516083 pypipr-1.0.91/pypipr/ifunctions/__init__.py
+-rw-r--r--   0        0        0      503 2024-04-23 11:45:29.548964 pypipr-1.0.91/pypipr/ifunctions/iargv.py
+-rw-r--r--   0        0        0      748 2024-03-17 17:38:37.516083 pypipr-1.0.91/pypipr/ifunctions/idumps.py
+-rw-r--r--   0        0        0     1423 2024-03-17 17:38:37.516083 pypipr-1.0.91/pypipr/ifunctions/idumps_html.py
+-rw-r--r--   0        0        0      679 2024-04-23 11:41:52.328964 pypipr-1.0.91/pypipr/ifunctions/ienv.py
+-rw-r--r--   0        0        0      465 2024-03-17 17:38:37.516083 pypipr-1.0.91/pypipr/ifunctions/iexec.py
+-rw-r--r--   0        0        0     2069 2024-03-17 17:38:37.516083 pypipr-1.0.91/pypipr/ifunctions/ijoin.py
+-rw-r--r--   0        0        0      638 2024-04-22 21:36:07.164645 pypipr-1.0.91/pypipr/ifunctions/iloads.py
+-rw-r--r--   0        0        0     4146 2024-04-22 21:40:17.264645 pypipr-1.0.91/pypipr/ifunctions/iloads_html.py
+-rw-r--r--   0        0        0     2808 2024-03-17 17:38:37.516083 pypipr-1.0.91/pypipr/ifunctions/iopen.py
+-rw-r--r--   0        0        0      849 2024-04-22 21:41:31.764645 pypipr-1.0.91/pypipr/ifunctions/iprint.py
+-rw-r--r--   0        0        0     2407 2024-03-17 17:38:37.516083 pypipr-1.0.91/pypipr/ifunctions/irange.py
+-rw-r--r--   0        0        0      722 2024-03-17 17:38:37.516083 pypipr-1.0.91/pypipr/ifunctions/ireplace.py
+-rw-r--r--   0        0        0      748 2024-04-23 09:11:14.125403 pypipr-1.0.91/pypipr/ifunctions/iscandir.py
+-rw-r--r--   0        0        0      383 2024-03-17 17:38:37.520083 pypipr-1.0.91/pypipr/ifunctions/isplit.py
+-rw-r--r--   0        0        0     1061 2024-04-20 02:38:18.131451 pypipr-1.0.91/pypipr/pypipr.py.bak
+-rw-r--r--   0        0        0     1800 2024-04-23 13:05:42.093603 pypipr-1.0.91/pypipr/terminal.py
+-rw-r--r--   0        0        0      544 2024-04-24 04:39:35.033174 pypipr-1.0.91/pyproject.toml
+-rw-r--r--   0        0        0    49784 2024-04-24 04:39:27.445174 pypipr-1.0.91/readme.md
+-rw-r--r--   0        0        0    50470 1970-01-01 00:00:00.000000 pypipr-1.0.91/PKG-INFO
```

### Comparing `pypipr-1.0.90/pypipr/__init__.py` & `pypipr-1.0.91/pypipr/__init__.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/ibuiltins/ComparePerformance.py` & `pypipr-1.0.91/pypipr/ibuiltins/ComparePerformance.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/ibuiltins/RunParallel.py` & `pypipr-1.0.91/pypipr/ibuiltins/RunParallel.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/ibuiltins/filter_empty.py` & `pypipr-1.0.91/pypipr/ibuiltins/filter_empty.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/ibuiltins/get_class_method.py` & `pypipr-1.0.91/pypipr/ibuiltins/get_class_method.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/ibuiltins/is_empty.py` & `pypipr-1.0.91/pypipr/ibuiltins/is_empty.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/ibuiltins/is_iterable.py` & `pypipr-1.0.91/pypipr/ibuiltins/is_iterable.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/ibuiltins/is_valid_url.py` & `pypipr-1.0.91/pypipr/ibuiltins/is_valid_url.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/ibuiltins/ivars.py` & `pypipr-1.0.91/pypipr/ibuiltins/ivars.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/ibuiltins/set_timeout.py` & `pypipr-1.0.91/pypipr/ibuiltins/set_timeout.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/ibuiltins/to_str.py` & `pypipr-1.0.91/pypipr/ibuiltins/to_str.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/iconsole/choices.py` & `pypipr-1.0.91/pypipr/iconsole/choices.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/iconsole/console_run.py` & `pypipr-1.0.91/pypipr/iconsole/console_run.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/iconsole/input_char.py` & `pypipr-1.0.91/pypipr/iconsole/input_char.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/iconsole/log.py` & `pypipr-1.0.91/pypipr/iconsole/log.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/iconsole/print_dir.py` & `pypipr-1.0.91/pypipr/iconsole/print_dir.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/iconsole/print_to_last_line.py` & `pypipr-1.0.91/pypipr/iconsole/print_to_last_line.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/idjango/APIMixinView.py` & `pypipr-1.0.91/pypipr/idjango/APIMixinView.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/iengineering/batch_calculate.py` & `pypipr-1.0.91/pypipr/iengineering/batch_calculate.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/iengineering/batchmaker.py` & `pypipr-1.0.91/pypipr/iengineering/batchmaker.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/iengineering/calculate.py` & `pypipr-1.0.91/pypipr/iengineering/calculate.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/iflow/auto_reload.py` & `pypipr-1.0.91/pypipr/iflow/auto_reload.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/iflow/github_push.py` & `pypipr-1.0.91/pypipr/iflow/github_push.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/iflow/github_user.py` & `pypipr-1.0.91/pypipr/iflow/github_user.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/iflow/pip_freeze_without_version.py` & `pypipr-1.0.91/pypipr/iflow/pip_freeze_without_version.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/iflow/poetry_update_version.py` & `pypipr-1.0.91/pypipr/iflow/poetry_update_version.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/ifunctions/idumps.py` & `pypipr-1.0.91/pypipr/ifunctions/idumps.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/ifunctions/idumps_html.py` & `pypipr-1.0.91/pypipr/ifunctions/idumps_html.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/ifunctions/ienv.py` & `pypipr-1.0.91/pypipr/ifunctions/ienv.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/ifunctions/ijoin.py` & `pypipr-1.0.91/pypipr/ifunctions/ijoin.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/ifunctions/iloads.py` & `pypipr-1.0.91/pypipr/ifunctions/iloads.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/ifunctions/iloads_html.py` & `pypipr-1.0.91/pypipr/ifunctions/iloads_html.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/ifunctions/iopen.py` & `pypipr-1.0.91/pypipr/ifunctions/iopen.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/ifunctions/iprint.py` & `pypipr-1.0.91/pypipr/ifunctions/iprint.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/ifunctions/irange.py` & `pypipr-1.0.91/pypipr/ifunctions/irange.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/ifunctions/ireplace.py` & `pypipr-1.0.91/pypipr/ifunctions/ireplace.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/ifunctions/iscandir.py` & `pypipr-1.0.91/pypipr/ifunctions/iscandir.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/pypipr.py.bak` & `pypipr-1.0.91/pypipr/pypipr.py.bak`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pypipr/terminal.py` & `pypipr-1.0.91/pypipr/terminal.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.90/pyproject.toml` & `pypipr-1.0.91/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypipr"
-version = "1.0.90"
+version = "1.0.91"
 description = "The Python Package Index Project"
 authors = ["ufiapjj <ufiapjj@gmail.com>"]
 readme = "readme.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 getch = { version = "*", markers = "platform_system == 'Linux'" }
```

