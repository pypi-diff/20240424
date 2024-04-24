# Comparing `tmp/pypipr-1.0.91.tar.gz` & `tmp/pypipr-1.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypipr-1.0.91.tar", max compression
+gzip compressed data, was "pypipr-1.0.92.tar", max compression
```

## Comparing `pypipr-1.0.91.tar` & `pypipr-1.0.92.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     3347 2024-04-24 04:39:24.109174 pypipr-1.0.91/pypipr/__init__.py
--rw-r--r--   0        0        0     2229 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/ComparePerformance.py
--rw-r--r--   0        0        0      100 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/LINUX.py
--rw-r--r--   0        0        0     7358 2024-04-23 10:50:10.015024 pypipr-1.0.91/pypipr/ibuiltins/RunParallel.py
--rw-r--r--   0        0        0      105 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/WINDOWS.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/__init__.py
--rw-r--r--   0        0        0      218 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/avg.py
--rw-r--r--   0        0        0      194 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/basename.py
--rw-r--r--   0        0        0      385 2024-04-22 13:19:16.948654 pypipr-1.0.91/pypipr/ibuiltins/chunk_array.py
--rw-r--r--   0        0        0      500 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/create_folder.py
--rw-r--r--   0        0        0      466 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/datetime_from_string.py
--rw-r--r--   0        0        0      476 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/datetime_now.py
--rw-r--r--   0        0        0      377 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/dict_first.py
--rw-r--r--   0        0        0      229 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/dirname.py
--rw-r--r--   0        0        0      321 2024-04-20 11:53:09.914721 pypipr-1.0.91/pypipr/ibuiltins/exit_if_empty.py
--rw-r--r--   0        0        0      543 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/filter_empty.py
--rw-r--r--   0        0        0      335 2024-04-23 12:23:59.246031 pypipr-1.0.91/pypipr/ibuiltins/get_by_index.py
--rw-r--r--   0        0        0      639 2024-04-22 21:58:29.290425 pypipr-1.0.91/pypipr/ibuiltins/get_class_method.py
--rw-r--r--   0        0        0      227 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/get_filemtime.py
--rw-r--r--   0        0        0      196 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/get_filesize.py
--rw-r--r--   0        0        0      683 2024-04-20 11:02:21.923096 pypipr-1.0.91/pypipr/ibuiltins/is_empty.py
--rw-r--r--   0        0        0      922 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/is_iterable.py
--rw-r--r--   0        0        0     1008 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/is_valid_url.py
--rw-r--r--   0        0        0      899 2024-04-23 09:16:42.841403 pypipr-1.0.91/pypipr/ibuiltins/ivars.py
--rw-r--r--   0        0        0      496 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/password_generator.py
--rw-r--r--   0        0        0      405 2024-03-17 17:38:37.508083 pypipr-1.0.91/pypipr/ibuiltins/random_bool.py
--rw-r--r--   0        0        0      698 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/ibuiltins/set_timeout.py
--rw-r--r--   0        0        0      325 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/ibuiltins/sets_ordered.py
--rw-r--r--   0        0        0      377 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/ibuiltins/str_cmp.py
--rw-r--r--   0        0        0      597 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/ibuiltins/to_str.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/iconsole/__init__.py
--rw-r--r--   0        0        0     1686 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/iconsole/choices.py
--rw-r--r--   0        0        0      525 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/iconsole/console_run.py
--rw-r--r--   0        0        0     1030 2024-04-23 12:02:12.950032 pypipr-1.0.91/pypipr/iconsole/input_char.py
--rw-r--r--   0        0        0     1041 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/iconsole/log.py
--rw-r--r--   0        0        0      474 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/iconsole/print_colorize.py
--rw-r--r--   0        0        0      930 2024-04-22 21:43:34.984645 pypipr-1.0.91/pypipr/iconsole/print_dir.py
--rw-r--r--   0        0        0      282 2024-04-22 21:44:47.788645 pypipr-1.0.91/pypipr/iconsole/print_log.py
--rw-r--r--   0        0        0      914 2024-04-24 02:48:07.180538 pypipr-1.0.91/pypipr/iconsole/print_to_last_line.py
--rw-r--r--   0        0        0      396 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/iconsole/text_colorize.py
--rw-r--r--   0        0        0     1093 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/idjango/APIMixinView.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/idjango/__init__.py
--rw-r--r--   0        0        0      222 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/iengineering/PintUreg.py
--rw-r--r--   0        0        0      118 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/iengineering/PintUregQuantity.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/iengineering/__init__.py
--rw-r--r--   0        0        0      695 2024-04-22 21:59:57.598425 pypipr-1.0.91/pypipr/iengineering/batch_calculate.py
--rw-r--r--   0        0        0     1277 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/iengineering/batchmaker.py
--rw-r--r--   0        0        0      805 2024-03-17 17:38:37.512083 pypipr-1.0.91/pypipr/iengineering/calculate.py
--rw-r--r--   0        0        0      966 2024-04-23 11:50:40.860964 pypipr-1.0.91/pypipr/iflow/auto_reload.py
--rw-r--r--   0        0        0      243 2024-03-17 17:38:37.516083 pypipr-1.0.91/pypipr/iflow/github_pull.py
--rw-r--r--   0        0        0      951 2024-03-17 17:38:37.516083 pypipr-1.0.91/pypipr/iflow/github_push.py
--rw-r--r--   0        0        0      600 2024-03-17 17:38:37.516083 pypipr-1.0.91/pypipr/iflow/github_user.py
--rw-r--r--   0        0        0      839 2024-04-20 02:24:51.624107 pypipr-1.0.91/pypipr/iflow/pip_freeze_without_version.py
--rw-r--r--   0        0        0      409 2024-03-17 17:38:37.516083 pypipr-1.0.91/pypipr/iflow/poetry_publish.py
--rw-r--r--   0        0        0      622 2024-03-17 17:38:37.516083 pypipr-1.0.91/pypipr/iflow/poetry_update_version.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.516083 pypipr-1.0.91/pypipr/ifunctions/__init__.py
--rw-r--r--   0        0        0      503 2024-04-23 11:45:29.548964 pypipr-1.0.91/pypipr/ifunctions/iargv.py
--rw-r--r--   0        0        0      748 2024-03-17 17:38:37.516083 pypipr-1.0.91/pypipr/ifunctions/idumps.py
--rw-r--r--   0        0        0     1423 2024-03-17 17:38:37.516083 pypipr-1.0.91/pypipr/ifunctions/idumps_html.py
--rw-r--r--   0        0        0      679 2024-04-23 11:41:52.328964 pypipr-1.0.91/pypipr/ifunctions/ienv.py
--rw-r--r--   0        0        0      465 2024-03-17 17:38:37.516083 pypipr-1.0.91/pypipr/ifunctions/iexec.py
--rw-r--r--   0        0        0     2069 2024-03-17 17:38:37.516083 pypipr-1.0.91/pypipr/ifunctions/ijoin.py
--rw-r--r--   0        0        0      638 2024-04-22 21:36:07.164645 pypipr-1.0.91/pypipr/ifunctions/iloads.py
--rw-r--r--   0        0        0     4146 2024-04-22 21:40:17.264645 pypipr-1.0.91/pypipr/ifunctions/iloads_html.py
--rw-r--r--   0        0        0     2808 2024-03-17 17:38:37.516083 pypipr-1.0.91/pypipr/ifunctions/iopen.py
--rw-r--r--   0        0        0      849 2024-04-22 21:41:31.764645 pypipr-1.0.91/pypipr/ifunctions/iprint.py
--rw-r--r--   0        0        0     2407 2024-03-17 17:38:37.516083 pypipr-1.0.91/pypipr/ifunctions/irange.py
--rw-r--r--   0        0        0      722 2024-03-17 17:38:37.516083 pypipr-1.0.91/pypipr/ifunctions/ireplace.py
--rw-r--r--   0        0        0      748 2024-04-23 09:11:14.125403 pypipr-1.0.91/pypipr/ifunctions/iscandir.py
--rw-r--r--   0        0        0      383 2024-03-17 17:38:37.520083 pypipr-1.0.91/pypipr/ifunctions/isplit.py
--rw-r--r--   0        0        0     1061 2024-04-20 02:38:18.131451 pypipr-1.0.91/pypipr/pypipr.py.bak
--rw-r--r--   0        0        0     1800 2024-04-23 13:05:42.093603 pypipr-1.0.91/pypipr/terminal.py
--rw-r--r--   0        0        0      544 2024-04-24 04:39:35.033174 pypipr-1.0.91/pyproject.toml
--rw-r--r--   0        0        0    49784 2024-04-24 04:39:27.445174 pypipr-1.0.91/readme.md
--rw-r--r--   0        0        0    50470 1970-01-01 00:00:00.000000 pypipr-1.0.91/PKG-INFO
+-rw-r--r--   0        0        0     3347 2024-04-24 08:04:26.350958 pypipr-1.0.92/pypipr/__init__.py
+-rw-r--r--   0        0        0     2229 2024-03-17 17:38:37.508083 pypipr-1.0.92/pypipr/ibuiltins/ComparePerformance.py
+-rw-r--r--   0        0        0      100 2024-03-17 17:38:37.508083 pypipr-1.0.92/pypipr/ibuiltins/LINUX.py
+-rw-r--r--   0        0        0     7358 2024-04-23 10:50:10.015024 pypipr-1.0.92/pypipr/ibuiltins/RunParallel.py
+-rw-r--r--   0        0        0      105 2024-03-17 17:38:37.508083 pypipr-1.0.92/pypipr/ibuiltins/WINDOWS.py
+-rw-r--r--   0        0        0        0 2024-03-17 17:38:37.508083 pypipr-1.0.92/pypipr/ibuiltins/__init__.py
+-rw-r--r--   0        0        0      218 2024-03-17 17:38:37.508083 pypipr-1.0.92/pypipr/ibuiltins/avg.py
+-rw-r--r--   0        0        0      194 2024-03-17 17:38:37.508083 pypipr-1.0.92/pypipr/ibuiltins/basename.py
+-rw-r--r--   0        0        0      385 2024-04-22 13:19:16.948654 pypipr-1.0.92/pypipr/ibuiltins/chunk_array.py
+-rw-r--r--   0        0        0      500 2024-03-17 17:38:37.508083 pypipr-1.0.92/pypipr/ibuiltins/create_folder.py
+-rw-r--r--   0        0        0      466 2024-03-17 17:38:37.508083 pypipr-1.0.92/pypipr/ibuiltins/datetime_from_string.py
+-rw-r--r--   0        0        0      476 2024-03-17 17:38:37.508083 pypipr-1.0.92/pypipr/ibuiltins/datetime_now.py
+-rw-r--r--   0        0        0      377 2024-03-17 17:38:37.508083 pypipr-1.0.92/pypipr/ibuiltins/dict_first.py
+-rw-r--r--   0        0        0      229 2024-03-17 17:38:37.508083 pypipr-1.0.92/pypipr/ibuiltins/dirname.py
+-rw-r--r--   0        0        0      321 2024-04-20 11:53:09.914721 pypipr-1.0.92/pypipr/ibuiltins/exit_if_empty.py
+-rw-r--r--   0        0        0      543 2024-03-17 17:38:37.508083 pypipr-1.0.92/pypipr/ibuiltins/filter_empty.py
+-rw-r--r--   0        0        0      335 2024-04-23 12:23:59.246031 pypipr-1.0.92/pypipr/ibuiltins/get_by_index.py
+-rw-r--r--   0        0        0      639 2024-04-22 21:58:29.290425 pypipr-1.0.92/pypipr/ibuiltins/get_class_method.py
+-rw-r--r--   0        0        0      227 2024-03-17 17:38:37.508083 pypipr-1.0.92/pypipr/ibuiltins/get_filemtime.py
+-rw-r--r--   0        0        0      196 2024-03-17 17:38:37.508083 pypipr-1.0.92/pypipr/ibuiltins/get_filesize.py
+-rw-r--r--   0        0        0      683 2024-04-20 11:02:21.923096 pypipr-1.0.92/pypipr/ibuiltins/is_empty.py
+-rw-r--r--   0        0        0      922 2024-03-17 17:38:37.508083 pypipr-1.0.92/pypipr/ibuiltins/is_iterable.py
+-rw-r--r--   0        0        0     1008 2024-03-17 17:38:37.508083 pypipr-1.0.92/pypipr/ibuiltins/is_valid_url.py
+-rw-r--r--   0        0        0      899 2024-04-23 09:16:42.841403 pypipr-1.0.92/pypipr/ibuiltins/ivars.py
+-rw-r--r--   0        0        0      496 2024-03-17 17:38:37.508083 pypipr-1.0.92/pypipr/ibuiltins/password_generator.py
+-rw-r--r--   0        0        0      405 2024-03-17 17:38:37.508083 pypipr-1.0.92/pypipr/ibuiltins/random_bool.py
+-rw-r--r--   0        0        0      698 2024-03-17 17:38:37.512083 pypipr-1.0.92/pypipr/ibuiltins/set_timeout.py
+-rw-r--r--   0        0        0      325 2024-03-17 17:38:37.512083 pypipr-1.0.92/pypipr/ibuiltins/sets_ordered.py
+-rw-r--r--   0        0        0      377 2024-03-17 17:38:37.512083 pypipr-1.0.92/pypipr/ibuiltins/str_cmp.py
+-rw-r--r--   0        0        0      597 2024-03-17 17:38:37.512083 pypipr-1.0.92/pypipr/ibuiltins/to_str.py
+-rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.92/pypipr/iconsole/__init__.py
+-rw-r--r--   0        0        0     1686 2024-03-17 17:38:37.512083 pypipr-1.0.92/pypipr/iconsole/choices.py
+-rw-r--r--   0        0        0      525 2024-03-17 17:38:37.512083 pypipr-1.0.92/pypipr/iconsole/console_run.py
+-rw-r--r--   0        0        0     1030 2024-04-23 12:02:12.950032 pypipr-1.0.92/pypipr/iconsole/input_char.py
+-rw-r--r--   0        0        0     1041 2024-03-17 17:38:37.512083 pypipr-1.0.92/pypipr/iconsole/log.py
+-rw-r--r--   0        0        0      474 2024-03-17 17:38:37.512083 pypipr-1.0.92/pypipr/iconsole/print_colorize.py
+-rw-r--r--   0        0        0      930 2024-04-22 21:43:34.984645 pypipr-1.0.92/pypipr/iconsole/print_dir.py
+-rw-r--r--   0        0        0      282 2024-04-22 21:44:47.788645 pypipr-1.0.92/pypipr/iconsole/print_log.py
+-rw-r--r--   0        0        0      914 2024-04-24 02:48:07.180538 pypipr-1.0.92/pypipr/iconsole/print_to_last_line.py
+-rw-r--r--   0        0        0      396 2024-03-17 17:38:37.512083 pypipr-1.0.92/pypipr/iconsole/text_colorize.py
+-rw-r--r--   0        0        0     1093 2024-03-17 17:38:37.512083 pypipr-1.0.92/pypipr/idjango/APIMixinView.py
+-rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.92/pypipr/idjango/__init__.py
+-rw-r--r--   0        0        0      222 2024-03-17 17:38:37.512083 pypipr-1.0.92/pypipr/iengineering/PintUreg.py
+-rw-r--r--   0        0        0      118 2024-03-17 17:38:37.512083 pypipr-1.0.92/pypipr/iengineering/PintUregQuantity.py
+-rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.92/pypipr/iengineering/__init__.py
+-rw-r--r--   0        0        0      695 2024-04-22 21:59:57.598425 pypipr-1.0.92/pypipr/iengineering/batch_calculate.py
+-rw-r--r--   0        0        0     1277 2024-03-17 17:38:37.512083 pypipr-1.0.92/pypipr/iengineering/batchmaker.py
+-rw-r--r--   0        0        0      805 2024-03-17 17:38:37.512083 pypipr-1.0.92/pypipr/iengineering/calculate.py
+-rw-r--r--   0        0        0      966 2024-04-23 11:50:40.860964 pypipr-1.0.92/pypipr/iflow/auto_reload.py
+-rw-r--r--   0        0        0      243 2024-03-17 17:38:37.516083 pypipr-1.0.92/pypipr/iflow/github_pull.py
+-rw-r--r--   0        0        0      951 2024-03-17 17:38:37.516083 pypipr-1.0.92/pypipr/iflow/github_push.py
+-rw-r--r--   0        0        0      600 2024-03-17 17:38:37.516083 pypipr-1.0.92/pypipr/iflow/github_user.py
+-rw-r--r--   0        0        0      839 2024-04-20 02:24:51.624107 pypipr-1.0.92/pypipr/iflow/pip_freeze_without_version.py
+-rw-r--r--   0        0        0      409 2024-03-17 17:38:37.516083 pypipr-1.0.92/pypipr/iflow/poetry_publish.py
+-rw-r--r--   0        0        0      622 2024-03-17 17:38:37.516083 pypipr-1.0.92/pypipr/iflow/poetry_update_version.py
+-rw-r--r--   0        0        0        0 2024-03-17 17:38:37.516083 pypipr-1.0.92/pypipr/ifunctions/__init__.py
+-rw-r--r--   0        0        0      552 2024-04-24 08:03:08.734958 pypipr-1.0.92/pypipr/ifunctions/iargv.py
+-rw-r--r--   0        0        0      748 2024-03-17 17:38:37.516083 pypipr-1.0.92/pypipr/ifunctions/idumps.py
+-rw-r--r--   0        0        0     1423 2024-03-17 17:38:37.516083 pypipr-1.0.92/pypipr/ifunctions/idumps_html.py
+-rw-r--r--   0        0        0      679 2024-04-23 11:41:52.328964 pypipr-1.0.92/pypipr/ifunctions/ienv.py
+-rw-r--r--   0        0        0      465 2024-03-17 17:38:37.516083 pypipr-1.0.92/pypipr/ifunctions/iexec.py
+-rw-r--r--   0        0        0     2069 2024-03-17 17:38:37.516083 pypipr-1.0.92/pypipr/ifunctions/ijoin.py
+-rw-r--r--   0        0        0      638 2024-04-22 21:36:07.164645 pypipr-1.0.92/pypipr/ifunctions/iloads.py
+-rw-r--r--   0        0        0     4146 2024-04-22 21:40:17.264645 pypipr-1.0.92/pypipr/ifunctions/iloads_html.py
+-rw-r--r--   0        0        0     2808 2024-03-17 17:38:37.516083 pypipr-1.0.92/pypipr/ifunctions/iopen.py
+-rw-r--r--   0        0        0      849 2024-04-22 21:41:31.764645 pypipr-1.0.92/pypipr/ifunctions/iprint.py
+-rw-r--r--   0        0        0     2407 2024-03-17 17:38:37.516083 pypipr-1.0.92/pypipr/ifunctions/irange.py
+-rw-r--r--   0        0        0      722 2024-03-17 17:38:37.516083 pypipr-1.0.92/pypipr/ifunctions/ireplace.py
+-rw-r--r--   0        0        0      748 2024-04-23 09:11:14.125403 pypipr-1.0.92/pypipr/ifunctions/iscandir.py
+-rw-r--r--   0        0        0      383 2024-03-17 17:38:37.520083 pypipr-1.0.92/pypipr/ifunctions/isplit.py
+-rw-r--r--   0        0        0     1061 2024-04-20 02:38:18.131451 pypipr-1.0.92/pypipr/pypipr.py.bak
+-rw-r--r--   0        0        0     1827 2024-04-24 08:04:11.598958 pypipr-1.0.92/pypipr/terminal.py
+-rw-r--r--   0        0        0      544 2024-04-24 08:04:38.114958 pypipr-1.0.92/pyproject.toml
+-rw-r--r--   0        0        0    49934 2024-04-24 08:04:29.582958 pypipr-1.0.92/readme.md
+-rw-r--r--   0        0        0    50620 1970-01-01 00:00:00.000000 pypipr-1.0.92/PKG-INFO
```

### Comparing `pypipr-1.0.91/pypipr/__init__.py` & `pypipr-1.0.92/pypipr/__init__.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/ibuiltins/ComparePerformance.py` & `pypipr-1.0.92/pypipr/ibuiltins/ComparePerformance.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/ibuiltins/RunParallel.py` & `pypipr-1.0.92/pypipr/ibuiltins/RunParallel.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/ibuiltins/filter_empty.py` & `pypipr-1.0.92/pypipr/ibuiltins/filter_empty.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/ibuiltins/get_class_method.py` & `pypipr-1.0.92/pypipr/ibuiltins/get_class_method.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/ibuiltins/is_empty.py` & `pypipr-1.0.92/pypipr/ibuiltins/is_empty.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/ibuiltins/is_iterable.py` & `pypipr-1.0.92/pypipr/ibuiltins/is_iterable.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/ibuiltins/is_valid_url.py` & `pypipr-1.0.92/pypipr/ibuiltins/is_valid_url.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/ibuiltins/ivars.py` & `pypipr-1.0.92/pypipr/ibuiltins/ivars.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/ibuiltins/set_timeout.py` & `pypipr-1.0.92/pypipr/ibuiltins/set_timeout.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/ibuiltins/to_str.py` & `pypipr-1.0.92/pypipr/ibuiltins/to_str.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/iconsole/choices.py` & `pypipr-1.0.92/pypipr/iconsole/choices.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/iconsole/console_run.py` & `pypipr-1.0.92/pypipr/iconsole/console_run.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/iconsole/input_char.py` & `pypipr-1.0.92/pypipr/iconsole/input_char.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/iconsole/log.py` & `pypipr-1.0.92/pypipr/iconsole/log.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/iconsole/print_dir.py` & `pypipr-1.0.92/pypipr/iconsole/print_dir.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/iconsole/print_to_last_line.py` & `pypipr-1.0.92/pypipr/iconsole/print_to_last_line.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/idjango/APIMixinView.py` & `pypipr-1.0.92/pypipr/idjango/APIMixinView.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/iengineering/batch_calculate.py` & `pypipr-1.0.92/pypipr/iengineering/batch_calculate.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/iengineering/batchmaker.py` & `pypipr-1.0.92/pypipr/iengineering/batchmaker.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/iengineering/calculate.py` & `pypipr-1.0.92/pypipr/iengineering/calculate.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/iflow/auto_reload.py` & `pypipr-1.0.92/pypipr/iflow/auto_reload.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/iflow/github_push.py` & `pypipr-1.0.92/pypipr/iflow/github_push.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/iflow/github_user.py` & `pypipr-1.0.92/pypipr/iflow/github_user.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/iflow/pip_freeze_without_version.py` & `pypipr-1.0.92/pypipr/iflow/pip_freeze_without_version.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/iflow/poetry_update_version.py` & `pypipr-1.0.92/pypipr/iflow/poetry_update_version.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/ifunctions/idumps.py` & `pypipr-1.0.92/pypipr/ifunctions/idumps.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/ifunctions/idumps_html.py` & `pypipr-1.0.92/pypipr/ifunctions/idumps_html.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/ifunctions/ienv.py` & `pypipr-1.0.92/pypipr/ifunctions/ienv.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/ifunctions/ijoin.py` & `pypipr-1.0.92/pypipr/ifunctions/ijoin.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/ifunctions/iloads.py` & `pypipr-1.0.92/pypipr/ifunctions/iloads.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/ifunctions/iloads_html.py` & `pypipr-1.0.92/pypipr/ifunctions/iloads_html.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/ifunctions/iopen.py` & `pypipr-1.0.92/pypipr/ifunctions/iopen.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/ifunctions/iprint.py` & `pypipr-1.0.92/pypipr/ifunctions/iprint.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/ifunctions/irange.py` & `pypipr-1.0.92/pypipr/ifunctions/irange.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/ifunctions/ireplace.py` & `pypipr-1.0.92/pypipr/ifunctions/ireplace.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/ifunctions/iscandir.py` & `pypipr-1.0.92/pypipr/ifunctions/iscandir.py`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/pypipr.py.bak` & `pypipr-1.0.92/pypipr/pypipr.py.bak`

 * *Files identical despite different names*

### Comparing `pypipr-1.0.91/pypipr/terminal.py` & `pypipr-1.0.92/pypipr/terminal.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pypipr
 
 
 def main():
+    print(pypipr.sys.argv)
     m = pypipr.ivars(pypipr)
     m = m["module"] | m["variable"] | m["class"] | m["function"]
     m = [x for x in m]
     a = pypipr.iargv(1)
     pd = False
     while isinstance(m, list):
         if a is None:
```

### Comparing `pypipr-1.0.91/pyproject.toml` & `pypipr-1.0.92/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypipr"
-version = "1.0.91"
+version = "1.0.92"
 description = "The Python Package Index Project"
 authors = ["ufiapjj <ufiapjj@gmail.com>"]
 readme = "readme.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 getch = { version = "*", markers = "platform_system == 'Linux'" }
```

### Comparing `pypipr-1.0.91/readme.md` & `pypipr-1.0.92/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: pypipr
+Version: 1.0.92
+Summary: The Python Package Index Project
+Author: ufiapjj
+Author-email: ufiapjj@gmail.com
+Requires-Python: >=3.9
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: colorama
+Requires-Dist: cssselect
+Requires-Dist: django
+Requires-Dist: getch ; platform_system == "Linux"
+Requires-Dist: lxml
+Requires-Dist: pint
+Requires-Dist: pyyaml
+Requires-Dist: requests
+Requires-Dist: tzdata
+Description-Content-Type: text/markdown
+
 
 # About
 The Python Package Index Project (pypipr)
 
 pypi : https://pypi.org/project/pypipr
 
 
@@ -74,15 +97,15 @@
 arr = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]  
 print(chunk_array(arr, 5))  
 print(list(chunk_array(arr, 5)))  
 ```
 
 Output:
 ```py
-<generator object chunk_array at 0x72f4fd0240>
+<generator object chunk_array at 0x6f6287c240>
 [[2, 3, 12, 3, 3], [42, 42, 1, 43, 2], [42, 41, 4, 24, 32], [42, 3, 12, 32, 42], [42]]
 ```
 
 ## create_folder
 
 `create_folder(folder_name)`
 
@@ -125,17 +148,17 @@
 print(datetime_now("Asia/Jakarta"))  
 print(datetime_now("GMT"))  
 print(datetime_now("Etc/GMT+7"))  
 ```
 
 Output:
 ```py
-2024-04-24 11:39:26.061287+07:00
-2024-04-24 04:39:26.061634+00:00
-2024-04-23 21:39:26.062212-07:00
+2024-04-24 15:04:28.168838+07:00
+2024-04-24 08:04:28.169670+00:00
+2024-04-24 01:04:28.172534-07:00
 ```
 
 ## dict_first
 
 `dict_first(d: dict, remove=False)`
 
 Mengambil nilai (key, value) pertama dari dictionary dalam bentuk tuple.  
@@ -194,15 +217,15 @@
 ```python  
 var = [1, None, False, 0, "0", True, {}, ['eee']]  
 print(filter_empty(var))  
 ```
 
 Output:
 ```py
-<generator object filter_empty at 0x72f4f66d40>
+<generator object filter_empty at 0x6f6280ed40>
 ```
 
 ## get_by_index
 
 `get_by_index(obj, index, on_error=None)`
 
 Mendapatkan value dari object berdasarkan indexnya.  
@@ -240,16 +263,16 @@
   
 print(get_class_method(ExampleGetClassMethod))  
 print(list(get_class_method(ExampleGetClassMethod)))  
 ```
 
 Output:
 ```py
-<generator object get_class_method at 0x72f4f67010>
-[<function ExampleGetClassMethod.a at 0x730657e7a0>, <function ExampleGetClassMethod.b at 0x72f4fd9580>, <function ExampleGetClassMethod.c at 0x72f4fd9620>, <function ExampleGetClassMethod.d at 0x72f4fd96c0>]
+<generator object get_class_method at 0x6f6280f010>
+[<function ExampleGetClassMethod.a at 0x6f73cfe7a0>, <function ExampleGetClassMethod.b at 0x6f62885580>, <function ExampleGetClassMethod.c at 0x6f62885620>, <function ExampleGetClassMethod.d at 0x6f628856c0>]
 ```
 
 ## get_filemtime
 
 `get_filemtime(filename)`
 
 Mengambil informasi last modification time file dalam nano seconds  
@@ -366,15 +389,15 @@
 Output:
 ```py
 {'module': {'ibuiltins': <module 'pypipr.ibuiltins' from '/data/data/com.termux/files/home/pypipr/pypipr/ibuiltins/__init__.py'>,
             'iconsole': <module 'pypipr.iconsole' from '/data/data/com.termux/files/home/pypipr/pypipr/iconsole/__init__.py'>,
             'idjango': <module 'pypipr.idjango' from '/data/data/com.termux/files/home/pypipr/pypipr/idjango/__init__.py'>,
             'iengineering': <module 'pypipr.iengineering' from '/data/data/com.termux/files/home/pypipr/pypipr/iengineering/__init__.py'>,
             'ifunctions': <module 'pypipr.ifunctions' from '/data/data/com.termux/files/home/pypipr/pypipr/ifunctions/__init__.py'>,
-            'iflow': <module 'pypipr.iflow' (<_frozen_importlib_external.NamespaceLoader object at 0x72f921efd0>)>,
+            'iflow': <module 'pypipr.iflow' (<_frozen_importlib_external.NamespaceLoader object at 0x6f66608a10>)>,
             'asyncio': <module 'asyncio' from '/data/data/com.termux/files/usr/lib/python3.11/asyncio/__init__.py'>,
             'colorama': <module 'colorama' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/colorama/__init__.py'>,
             'datetime': <module 'datetime' from '/data/data/com.termux/files/usr/lib/python3.11/datetime.py'>,
             'functools': <module 'functools' from '/data/data/com.termux/files/usr/lib/python3.11/functools.py'>,
             'inspect': <module 'inspect' from '/data/data/com.termux/files/usr/lib/python3.11/inspect.py'>,
             'io': <module 'io' (frozen)>,
             'json': <module 'json' from '/data/data/com.termux/files/usr/lib/python3.11/json/__init__.py'>,
@@ -403,87 +426,87 @@
             'zoneinfo': <module 'zoneinfo' from '/data/data/com.termux/files/usr/lib/python3.11/zoneinfo/__init__.py'>},
  'class': {'ComparePerformance': <class 'pypipr.ibuiltins.ComparePerformance.ComparePerformance'>,
            'RunParallel': <class 'pypipr.ibuiltins.RunParallel.RunParallel'>,
            'APIMixinView': <class 'pypipr.idjango.APIMixinView.APIMixinView'>,
            'PintUregQuantity': <class 'pint.Quantity'>},
  'variable': {'LINUX': True,
               'WINDOWS': False,
-              'PintUreg': <pint.registry.UnitRegistry object at 0x7302ccb1d0>},
- 'function': {'avg': <function avg at 0x73065b6d40>,
-              'basename': <function basename at 0x730657e8e0>,
-              'chunk_array': <function chunk_array at 0x7302c01120>,
-              'create_folder': <function create_folder at 0x7302c01300>,
-              'datetime_from_string': <function datetime_from_string at 0x7302c014e0>,
-              'datetime_now': <function datetime_now at 0x7302ca9620>,
-              'dict_first': <function dict_first at 0x7302ca9580>,
-              'dirname': <function dirname at 0x7302ca94e0>,
-              'exit_if_empty': <function exit_if_empty at 0x7302c834c0>,
-              'filter_empty': <function filter_empty at 0x7302ca91c0>,
-              'get_by_index': <function get_by_index at 0x7302ca8ea0>,
-              'get_class_method': <function get_class_method at 0x7302ca8cc0>,
-              'get_filemtime': <function get_filemtime at 0x7302ca8b80>,
-              'get_filesize': <function get_filesize at 0x7302ca89a0>,
-              'is_empty': <function is_empty at 0x7302ca9260>,
-              'is_iterable': <function is_iterable at 0x7302ca8fe0>,
-              'is_valid_url': <function is_valid_url at 0x7302ca8860>,
-              'ivars': <function ivars at 0x7302ca87c0>,
-              'password_generator': <function password_generator at 0x7302ca8680>,
-              'random_bool': <function random_bool at 0x7302ca8400>,
-              'set_timeout': <function set_timeout at 0x7302cab7e0>,
-              'sets_ordered': <function sets_ordered at 0x7302cab920>,
-              'str_cmp': <function str_cmp at 0x7302cab9c0>,
-              'to_str': <function to_str at 0x7302ca8f40>,
-              'choices': <function choices at 0x7302caba60>,
-              'console_run': <function console_run at 0x7302cabce0>,
-              'input_char': <function input_char at 0x7302cabe20>,
-              'log': <function log at 0x7302cd0040>,
-              'print_colorize': <function print_colorize at 0x7302cd00e0>,
-              'print_dir': <function print_dir at 0x7302cd0220>,
-              'print_log': <function print_log at 0x7302cabec0>,
-              'print_to_last_line': <function print_to_last_line at 0x7302cabc40>,
-              'text_colorize': <function text_colorize at 0x7302cabd80>,
-              'batch_calculate': <function batch_calculate at 0x72f9235580>,
-              'batchmaker': <function batchmaker at 0x72f920e980>,
-              'calculate': <function calculate at 0x72f92362a0>,
-              'auto_reload': <function auto_reload at 0x72f9236480>,
-              'github_pull': <function github_pull at 0x72f9236020>,
-              'github_push': <function github_push at 0x72f9236700>,
-              'github_user': <function github_user at 0x72f9236a20>,
-              'pip_freeze_without_version': <function pip_freeze_without_version at 0x72f8f5a020>,
-              'poetry_publish': <function poetry_publish at 0x72f8f5a160>,
-              'poetry_update_version': <function poetry_update_version at 0x72f8f7a980>,
-              'iargv': <function iargv at 0x72f51a00e0>,
-              'idumps': <function idumps at 0x72f51a0220>,
-              'idumps_html': <function idumps_html at 0x72f5204c20>,
-              'ienv': <function ienv at 0x72f51a0360>,
-              'iexec': <function iexec at 0x72f5204ea0>,
-              'ijoin': <function ijoin at 0x72f8f59ee0>,
-              'iloads': <function iloads at 0x72f5204f40>,
-              'iloads_html': <function iloads_html at 0x72f52051c0>,
-              'iopen': <function iopen at 0x72f8f5a200>,
-              'iprint': <function iprint at 0x72f51a0180>,
-              'irange': <function irange at 0x72f92363e0>,
-              'ireplace': <function ireplace at 0x72f5205080>,
-              'iscandir': <function iscandir at 0x72f5206e80>,
-              'isplit': <function isplit at 0x72f5206f20>}}
+              'PintUreg': <pint.registry.UnitRegistry object at 0x6f6ebab710>},
+ 'function': {'avg': <function avg at 0x6f73d36d40>,
+              'basename': <function basename at 0x6f73cfe8e0>,
+              'chunk_array': <function chunk_array at 0x6f6eae1120>,
+              'create_folder': <function create_folder at 0x6f6eae1300>,
+              'datetime_from_string': <function datetime_from_string at 0x6f6eae14e0>,
+              'datetime_now': <function datetime_now at 0x6f6eb89620>,
+              'dict_first': <function dict_first at 0x6f6eb89580>,
+              'dirname': <function dirname at 0x6f6eb894e0>,
+              'exit_if_empty': <function exit_if_empty at 0x6f6eb634c0>,
+              'filter_empty': <function filter_empty at 0x6f6eb891c0>,
+              'get_by_index': <function get_by_index at 0x6f6eb88ea0>,
+              'get_class_method': <function get_class_method at 0x6f6eb88cc0>,
+              'get_filemtime': <function get_filemtime at 0x6f6eb88b80>,
+              'get_filesize': <function get_filesize at 0x6f6eb889a0>,
+              'is_empty': <function is_empty at 0x6f6eb89260>,
+              'is_iterable': <function is_iterable at 0x6f6eb88fe0>,
+              'is_valid_url': <function is_valid_url at 0x6f6eb88860>,
+              'ivars': <function ivars at 0x6f6eb887c0>,
+              'password_generator': <function password_generator at 0x6f6eb88680>,
+              'random_bool': <function random_bool at 0x6f6eb88400>,
+              'set_timeout': <function set_timeout at 0x6f6eb8b7e0>,
+              'sets_ordered': <function sets_ordered at 0x6f6eb8b920>,
+              'str_cmp': <function str_cmp at 0x6f6eb8b9c0>,
+              'to_str': <function to_str at 0x6f6eb88f40>,
+              'choices': <function choices at 0x6f6eb8ba60>,
+              'console_run': <function console_run at 0x6f6eb8bce0>,
+              'input_char': <function input_char at 0x6f6eb8be20>,
+              'log': <function log at 0x6f6ebb0040>,
+              'print_colorize': <function print_colorize at 0x6f6ebb00e0>,
+              'print_dir': <function print_dir at 0x6f6ebb0220>,
+              'print_log': <function print_log at 0x6f6eb8bec0>,
+              'print_to_last_line': <function print_to_last_line at 0x6f6eb8bc40>,
+              'text_colorize': <function text_colorize at 0x6f6eb8bd80>,
+              'batch_calculate': <function batch_calculate at 0x6f66731580>,
+              'batchmaker': <function batchmaker at 0x6f6670a980>,
+              'calculate': <function calculate at 0x6f667322a0>,
+              'auto_reload': <function auto_reload at 0x6f66732480>,
+              'github_pull': <function github_pull at 0x6f66732020>,
+              'github_push': <function github_push at 0x6f66732700>,
+              'github_user': <function github_user at 0x6f66732a20>,
+              'pip_freeze_without_version': <function pip_freeze_without_version at 0x6f6645e020>,
+              'poetry_publish': <function poetry_publish at 0x6f6645e160>,
+              'poetry_update_version': <function poetry_update_version at 0x6f6647e980>,
+              'iargv': <function iargv at 0x6f62a4c0e0>,
+              'idumps': <function idumps at 0x6f62a4c220>,
+              'idumps_html': <function idumps_html at 0x6f62ab4c20>,
+              'ienv': <function ienv at 0x6f62a4c360>,
+              'iexec': <function iexec at 0x6f62ab4ea0>,
+              'ijoin': <function ijoin at 0x6f6645dee0>,
+              'iloads': <function iloads at 0x6f62ab4f40>,
+              'iloads_html': <function iloads_html at 0x6f62ab51c0>,
+              'iopen': <function iopen at 0x6f6645e200>,
+              'iprint': <function iprint at 0x6f62a4c180>,
+              'irange': <function irange at 0x6f667323e0>,
+              'ireplace': <function ireplace at 0x6f62ab5080>,
+              'iscandir': <function iscandir at 0x6f62ab6e80>,
+              'isplit': <function isplit at 0x6f62ab6f20>}}
 ```
 
 ## password_generator
 
 `password_generator(length=8, characters='abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~')`
 
 Membuat pssword secara acak  
   
 ```python  
 print(password_generator())  
 ```
 
 Output:
 ```py
-Uy}-6-Qh
+_Pq4e5\d
 ```
 
 ## random_bool
 
 `random_bool()`
 
 Menghasilkan nilai random True atau False.  
@@ -515,15 +538,15 @@
 print(x)  
 print("menghentikan timeout 7")  
 x.cancel()  
 ```
 
 Output:
 ```py
-<Timer(Thread-2, started 493713603824)>
+<Timer(Thread-2, started 478370839792)>
 menghentikan timeout 7
 ```
 
 ## sets_ordered
 
 `sets_ordered(iterator)`
 
@@ -533,15 +556,15 @@
 array = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]  
 print(sets_ordered(array))  
 print(list(sets_ordered(array)))  
 ```
 
 Output:
 ```py
-<generator object sets_ordered at 0x72f4fe41e0>
+<generator object sets_ordered at 0x6f628901e0>
 [2, 3, 12, 42, 1, 43, 41, 4, 24, 32]
 ```
 
 ## str_cmp
 
 `str_cmp(t1, t2)`
 
@@ -687,29 +710,29 @@
              __doc__ : Path subclass for non-Windows systems.
 
     On a POSIX system, instantiating a Path should return this object.
     
            __enter__ : https:/www.google.com
           __fspath__ : https:/www.google.com
         __getstate__ : (None, {'_drv': '', '_root': '', '_parts': ['https:', 'www.google.com'], '_str': 'https:/www.google.com'})
-            __hash__ : 1324913689339074732
+            __hash__ : -7677454752077529173
             __init__ : None
    __init_subclass__ : None
           __module__ : pathlib
           __reduce__ : (<class 'pathlib.PosixPath'>, ('https:', 'www.google.com'))
             __repr__ : PosixPath('https:/www.google.com')
           __sizeof__ : 72
            __slots__ : ()
              __str__ : https:/www.google.com
     __subclasshook__ : NotImplemented
       _cached_cparts : ['https:', 'www.google.com']
              _cparts : ['https:', 'www.google.com']
                 _drv : 
-            _flavour : <pathlib._PosixFlavour object at 0x7302c7c2d0>
-               _hash : 1324913689339074732
+            _flavour : <pathlib._PosixFlavour object at 0x6f6eb5c650>
+               _hash : -7677454752077529173
               _parts : ['https:', 'www.google.com']
                _root : 
                 _str : https:/www.google.com
             absolute : /data/data/com.termux/files/home/pypipr/https:/www.google.com
               anchor : 
             as_posix : https:/www.google.com
                  cwd : /data/data/com.termux/files/home/pypipr
@@ -723,15 +746,15 @@
               is_dir : False
              is_fifo : False
              is_file : False
             is_mount : False
          is_reserved : False
            is_socket : False
           is_symlink : False
-             iterdir : <generator object Path.iterdir at 0x72f4fbcc80>
+             iterdir : <generator object Path.iterdir at 0x6f62868c80>
             joinpath : https:/www.google.com
                 name : www.google.com
               parent : https:
              parents : <PosixPath.parents>
                parts : ('https:', 'www.google.com')
              resolve : /data/data/com.termux/files/home/pypipr/https:/www.google.com
                 root : 
@@ -790,15 +813,15 @@
 ```python  
 print(batch_calculate("{1 10} m ** {1 3}"))  
 print(list(batch_calculate("{1 10} m ** {1 3}")))  
 ```
 
 Output:
 ```py
-<generator object batch_calculate at 0x72f4f67b50>
+<generator object batch_calculate at 0x6f6280fb50>
 [('1 m ** 1', <Quantity(1, 'meter')>), ('1 m ** 2', <Quantity(1, 'meter ** 2')>), ('1 m ** 3', <Quantity(1, 'meter ** 3')>), ('2 m ** 1', <Quantity(2, 'meter')>), ('2 m ** 2', <Quantity(2, 'meter ** 2')>), ('2 m ** 3', <Quantity(2, 'meter ** 3')>), ('3 m ** 1', <Quantity(3, 'meter')>), ('3 m ** 2', <Quantity(3, 'meter ** 2')>), ('3 m ** 3', <Quantity(3, 'meter ** 3')>), ('4 m ** 1', <Quantity(4, 'meter')>), ('4 m ** 2', <Quantity(4, 'meter ** 2')>), ('4 m ** 3', <Quantity(4, 'meter ** 3')>), ('5 m ** 1', <Quantity(5, 'meter')>), ('5 m ** 2', <Quantity(5, 'meter ** 2')>), ('5 m ** 3', <Quantity(5, 'meter ** 3')>), ('6 m ** 1', <Quantity(6, 'meter')>), ('6 m ** 2', <Quantity(6, 'meter ** 2')>), ('6 m ** 3', <Quantity(6, 'meter ** 3')>), ('7 m ** 1', <Quantity(7, 'meter')>), ('7 m ** 2', <Quantity(7, 'meter ** 2')>), ('7 m ** 3', <Quantity(7, 'meter ** 3')>), ('8 m ** 1', <Quantity(8, 'meter')>), ('8 m ** 2', <Quantity(8, 'meter ** 2')>), ('8 m ** 3', <Quantity(8, 'meter ** 3')>), ('9 m ** 1', <Quantity(9, 'meter')>), ('9 m ** 2', <Quantity(9, 'meter ** 2')>), ('9 m ** 3', <Quantity(9, 'meter ** 3')>), ('10 m ** 1', <Quantity(10, 'meter')>), ('10 m ** 2', <Quantity(10, 'meter ** 2')>), ('10 m ** 3', <Quantity(10, 'meter ** 3')>)]
 ```
 
 ## batchmaker
 
 `batchmaker(pattern: str)`
 
@@ -815,15 +838,15 @@
 s = "Urutan {1/6/3} dan {10:9} dan {j k} dan {Z - A - 15} saja."  
 print(batchmaker(s))  
 print(list(batchmaker(s)))  
 ```
 
 Output:
 ```py
-<generator object batchmaker at 0x72f4fd4040>
+<generator object batchmaker at 0x6f62880040>
 ['Urutan 1 dan 10 dan j dan Z saja.', 'Urutan 1 dan 10 dan j dan K saja.', 'Urutan 1 dan 10 dan k dan Z saja.', 'Urutan 1 dan 10 dan k dan K saja.', 'Urutan 1 dan 9 dan j dan Z saja.', 'Urutan 1 dan 9 dan j dan K saja.', 'Urutan 1 dan 9 dan k dan Z saja.', 'Urutan 1 dan 9 dan k dan K saja.', 'Urutan 4 dan 10 dan j dan Z saja.', 'Urutan 4 dan 10 dan j dan K saja.', 'Urutan 4 dan 10 dan k dan Z saja.', 'Urutan 4 dan 10 dan k dan K saja.', 'Urutan 4 dan 9 dan j dan Z saja.', 'Urutan 4 dan 9 dan j dan K saja.', 'Urutan 4 dan 9 dan k dan Z saja.', 'Urutan 4 dan 9 dan k dan K saja.']
 ```
 
 ## calculate
 
 `calculate(teks)`
 
@@ -1179,15 +1202,15 @@
     recursive_flat=True))  
 print(ijoin(arr, separator='</div>\n<div>', start='<div>', end='</div>'))  
 print(ijoin(10, ' '))  
 ```
 
 Output:
 ```py
-dfs, weq, qweqw, asd
+asd, dfs, qweqw, weq
 ,ini,path,seperti,url,
 ini,path,seperti,url
 <li>satu</li>
 <li>12</li>
 <li>34</li>
 <li>56</li>
 <li>tiga</li>
@@ -1245,17 +1268,17 @@
 pprint.pprint(iloads_html(iopen("https://harga-emas.org/1-gram/")), depth=10)  
 ```
 
 Output:
 ```py
 (['Home', 'Emas 1 Gram', 'History', 'Trend', 'Perak 1 Gram', 'Pluang'],
  [['Harga Emas Hari Ini - Rabu, 24 April 2024'],
-  ['Spot Emas USD↓2.327,60 (-2,31) / oz',
+  ['Spot Emas USD↓2.320,94 (-8,97) / oz',
    'Kurs IDR↑16.244,00 (+20,00) / USD',
-   'Emas IDR↑1.215.605 (+292) / gr'],
+   'Emas IDR↓1.212.127 (-3.186) / gr'],
   ['LM Antam (Jual)↓1.320.000 (-5.000) / gr',
    'LM Antam (Beli)↓1.218.000 (-5.000) / gr']],
  [['Harga Emas Hari Ini'],
   ['Gram', 'Gedung Antam Jakarta', 'Pegadaian'],
   ['per Gram (Rp)', 'per Batangan (Rp)', 'per Gram (Rp)', 'per Batangan (Rp)'],
   ['1000',
    '1.261 (-5)',
@@ -1318,108 +1341,116 @@
    '1.208.000 (+8.000)',
    '604.000 (+4.000)'],
   ['Update harga LM Antam :24 April 2024, pukul 08:12Harga pembelian kembali '
    ':Rp. 1.218.000/gram (-5.000)',
    'Update harga LM Pegadaian :31 Agustus 2023']],
  [['Spot Harga Emas Hari Ini (Market Open)'],
   ['Satuan', 'USD', 'Kurs\xa0Dollar', 'IDR'],
-  ['Ounce\xa0(oz)', '2.327,60 (-2,31)', '16.244,00 (+20,00)', '37.809.534'],
-  ['Gram\xa0(gr)', '74,83', '16.244,00', '1.215.605 (+292)'],
-  ['Kilogram\xa0(kg)', '74.834,08', '16.244,00', '1.215.604.760'],
-  ['Update harga emas :24 April 2024, pukul 11:39Update kurs :24 April 2024, '
-   'pukul 09:10']],
+  ['Ounce\xa0(oz)', '2.320,94 (-8,97)', '16.244,00 (+20,00)', '37.701.349'],
+  ['Gram\xa0(gr)', '74,62', '16.244,00', '1.212.127 (-3.186)'],
+  ['Kilogram\xa0(kg)', '74.619,95', '16.244,00', '1.212.126.530'],
+  ['Update harga emas :24 April 2024, pukul 15:04Update kurs :24 April 2024, '
+   'pukul 13:10']],
  [['Gram', 'UBS Gold 99.99%'],
   ['Jual', 'Beli'],
   ['/ Batang', '/ Gram', '/ Batang', '/ Gram'],
   ['100',
-   '126.212.000 (-500.000)',
-   '1.262.120 (-5.000)',
-   '123.735.000',
-   '1.237.350'],
+   '126.000.000 (-712.000)',
+   '1.260.000 (-7.120)',
+   '124.485.000 (+750.000)',
+   '1.244.850 (+7.500)'],
   ['50',
-   '63.145.000 (-250.000)',
-   '1.262.900 (-5.000)',
-   '61.920.000',
-   '1.238.400'],
+   '63.100.000 (-295.000)',
+   '1.262.000 (-5.900)',
+   '62.295.000 (+375.000)',
+   '1.245.900 (+7.500)'],
   ['25',
-   '31.612.000 (-125.000)',
-   '1.264.480 (-5.000)',
-   '31.062.500',
-   '1.242.500'],
+   '31.600.000 (-137.000)',
+   '1.264.000 (-5.480)',
+   '31.250.000 (+187.500)',
+   '1.250.000 (+7.500)'],
   ['10',
-   '12.695.000 (-50.000)',
-   '1.269.500 (-5.000)',
-   '12.475.000',
-   '1.247.500'],
-  ['5', '6.375.000 (-25.000)', '1.275.000 (-5.000)', '6.289.500', '1.257.900'],
-  ['1', '1.320.000 (-5.000)', '1.320.000 (-5.000)', '1.290.500', '1.290.500'],
-  ['', 'Update :24 April 2024, pukul 10:55']],
+   '12.680.000 (-65.000)',
+   '1.268.000 (-6.500)',
+   '12.550.000 (+75.000)',
+   '1.255.000 (+7.500)'],
+  ['5',
+   '6.365.000 (-35.000)',
+   '1.273.000 (-7.000)',
+   '6.327.000 (+37.500)',
+   '1.265.400 (+7.500)'],
+  ['1',
+   '1.320.000 (-5.000)',
+   '1.320.000 (-5.000)',
+   '1.298.000 (+7.500)',
+   '1.298.000 (+7.500)'],
+  ['', 'Update :24 April 2024, pukul 13:02']],
  [['Konversi Satuan'],
   ['Satuan', 'Ounce (oz)', 'Gram (gr)', 'Kilogram (kg)'],
   ['Ounce\xa0(oz)', '1', '31,1034767696', '0,0311034768'],
   ['Gram\xa0(gr)', '0,0321507466', '1', '0.001'],
   ['Kilogram\xa0(kg)', '32,1507466000', '1.000', '1']],
  [['Pergerakan Harga Emas Dunia'],
   ['Waktu', 'Emas'],
   ['Unit', 'USD', 'IDR'],
   ['Angka', '+/-', 'Angka', '+/-'],
   ['Hari Ini', 'Kurs', '', '', '16.224', '+20+0,12%'],
-  ['oz', '2.329,91', '-2,31-0,10%', '37.800.460', '+9.075+0,02%'],
-  ['gr', '74,91', '-0,07-0,10%', '1.215.313', '+292+0,02%'],
+  ['oz', '2.329,91', '-8,97-0,38%', '37.800.460', '-99.110-0,26%'],
+  ['gr', '74,91', '-0,29-0,38%', '1.215.313', '-3.186-0,26%'],
   ['30 Hari', 'Kurs', '', '', '15.773', '+471+2,99%'],
-  ['oz', '2.175,55', '+152,05+6,99%', '34.314.950', '+3.494.584+10,18%'],
-  ['gr', '69,95', '+4,89+6,99%', '1.103.251', '+112.353+10,18%'],
+  ['oz', '2.175,55', '+145,39+6,68%', '34.314.950', '+3.386.399+9,87%'],
+  ['gr', '69,95', '+4,67+6,68%', '1.103.251', '+108.875+9,87%'],
   ['2 Bulan', 'Kurs', '', '', '15.630', '+614+3,93%'],
-  ['oz', '2.035,57', '+292,03+14,35%', '31.815.959', '+5.993.575+18,84%'],
-  ['gr', '65,45', '+9,39+14,35', '1.022.907', '+192.698+18,84%'],
+  ['oz', '2.035,57', '+285,37+14,02%', '31.815.959', '+5.885.390+18,50%'],
+  ['gr', '65,45', '+9,17+14,02', '1.022.907', '+189.220+18,50%'],
   ['6 Bulan', 'Kurs', '', '', '15.933', '+311+1,95%'],
-  ['oz', '1.983,13', '+344,47+17,37%', '31.597.210', '+6.212.324+19,66%'],
-  ['gr', '63,76', '+11,07+17,37%', '1.015.874', '+199.731+19,66%'],
+  ['oz', '1.983,13', '+337,81+17,03%', '31.597.210', '+6.104.139+19,32%'],
+  ['gr', '63,76', '+10,86+17,03%', '1.015.874', '+196.253+19,32%'],
   ['1 Tahun', 'Kurs', '', '', '15.731', '+513+3,26%'],
-  ['oz', '1.823,86', '+503,74+27,62%', '28.691.142', '+9.118.393+31,78%'],
-  ['gr', '58,64', '+16,20+27,62%', '922.442', '+293.163+31,78%'],
+  ['oz', '1.823,86', '+497,08+27,25%', '28.691.142', '+9.010.208+31,40%'],
+  ['gr', '58,64', '+15,98+27,25%', '922.442', '+289.685+31,40%'],
   ['2 Tahun', 'Kurs', '', '', '14.361', '+1.883+13,11%'],
-  ['oz', '1.896,13', '+431,47+22,76%', '27.230.342', '+10.579.193+38,85%'],
-  ['gr', '60,96', '+13,87+22,76%', '875.476', '+340.129+38,85%'],
+  ['oz', '1.896,13', '+424,81+22,40%', '27.230.342', '+10.471.007+38,45%'],
+  ['gr', '60,96', '+13,66+22,40%', '875.476', '+336.651+38,45%'],
   ['3 Tahun', 'Kurs', '', '', '14.530', '+1.714+11,80%'],
-  ['oz', '1.777,11', '+550,49+30,98%', '25.821.408', '+11.988.126+46,43%'],
-  ['gr', '57,14', '+17,70+30,98%', '830.178', '+385.427+46,43%'],
+  ['oz', '1.777,11', '+543,83+30,60%', '25.821.408', '+11.879.941+46,01%'],
+  ['gr', '57,14', '+17,48+30,60%', '830.178', '+381.949+46,01%'],
   ['5 Tahun', 'Kurs', '', '', '14.188', '+2.056+14,49%'],
-  ['oz', '1.288,10', '+1.039,50+80,70%', '18.275.563', '+19.533.972+106,89%'],
-  ['gr', '41,41', '+33,42+80,70%', '587.573', '+628.032+106,89%']])
+  ['oz', '1.288,10', '+1.032,84+80,18%', '18.275.563', '+19.425.787+106,29%'],
+  ['gr', '41,41', '+33,21+80,18%', '587.573', '+624.554+106,29%']])
 (['Home', 'Emas 1 Gram', 'History', 'Trend', 'Perak 1 Gram', 'Pluang'],
  [[''],
   ['Emas 24 KaratHarga Emas 1 Gram', ''],
-  ['USD', '74,83↓', '-0,08-0,11%'],
-  ['KURS', '16.151,15↑', '+4,25+0,03%'],
-  ['IDR', '1.208.656,42↓', '-881,15-0,07%'],
-  ['Rabu, 24 April 2024 11:39']],
+  ['USD', '74,62↓', '-0,29-0,39%'],
+  ['KURS', '16.171,45↑', '+24,55+0,15%'],
+  ['IDR', '1.206.712,85↓', '-2.824,72-0,23%'],
+  ['Rabu, 24 April 2024 15:04']],
  [[''],
   ['Emas 1 Gram (IDR)Emas 1 Gram (USD)Kurs USD-IDR',
    'Hari Ini',
    '1 Bulan',
    '1 Tahun',
    '5 Tahun',
    'Max',
    '']],
  [['Pergerakkan Harga Emas 1 Gram'],
   ['', 'Penutupan Kemarin', 'Pergerakkan Hari Ini', 'Rata-rata'],
-  ['USD', '74,91', '74,83 - 74,91', '74,87'],
-  ['KURS', '16.146,90', '16.146,90 - 16.151,15', '16.149,03'],
-  ['IDR', '1.209.537,57', '1.208.656,42 - 1.209.537,57', '1.209.097,00'],
+  ['USD', '74,91', '74,62 - 74,91', '74,77'],
+  ['KURS', '16.146,90', '16.146,90 - 16.171,45', '16.159,18'],
+  ['IDR', '1.209.537,57', '1.206.712,85 - 1.209.537,57', '1.208.125,21'],
   [''],
   ['', 'Awal Tahun', 'Pergerakkan YTD', '+/- YTD'],
-  ['USD', '66,32', '64,07 - 77,14', '+8,51 (12,83%)'],
-  ['KURS', '15.390,10', '15.390,00 - 16.307,80', '+761,05 (4,95%)'],
-  ['IDR', '1.020.729,53', '997.660,12 - 1.256.829,06', '+187.926,89 (18,41%)'],
+  ['USD', '66,32', '64,07 - 77,14', '+8,30 (12,52%)'],
+  ['KURS', '15.390,10', '15.390,00 - 16.307,80', '+781,35 (5,08%)'],
+  ['IDR', '1.020.729,53', '997.660,12 - 1.256.829,06', '+185.983,32 (18,22%)'],
   [''],
   ['', 'Tahun Lalu / 52 Minggu', 'Pergerakkan 52 Minggu', '+/- 52 Minggu'],
-  ['USD', '63,76', '58,43 - 77,14', '+11,07 (17,36%)'],
-  ['KURS', '14.936,00', '14.669,40 - 16.307,80', '+1.215,15 (8,14%)'],
-  ['IDR', '952.339,68', '912.925,68 - 1.256.829,06', '+256.316,74 (26,91%)']])
+  ['USD', '63,76', '58,43 - 77,14', '+10,86 (17,03%)'],
+  ['KURS', '14.936,00', '14.669,40 - 16.307,80', '+1.235,45 (8,27%)'],
+  ['IDR', '952.339,68', '912.925,68 - 1.256.829,06', '+254.373,17 (26,71%)']])
 ```
 
 ## iopen
 
 `iopen(path, data=None, regex=None, css_select=None, xpath=None, file_append=False)`
 
 Membaca atau Tulis pada path yang bisa merupakan FILE maupun URL.  
@@ -1453,15 +1484,15 @@
 print(iopen("https://www.google.com/", dict(coba="dulu"), xpath="//a"))  
 ```
 
 Output:
 ```py
 8
 ['mana', 'aja']
-[<Element a at 0x72f4fc6f80>, <Element a at 0x72f5012670>, <Element a at 0x72f5012710>, <Element a at 0x72f5012760>, <Element a at 0x72f50127b0>, <Element a at 0x72f5012800>, <Element a at 0x72f5012850>, <Element a at 0x72f50128a0>, <Element a at 0x72f50128f0>, <Element a at 0x72f5012940>, <Element a at 0x72f5012990>, <Element a at 0x72f50129e0>, <Element a at 0x72f5012a30>, <Element a at 0x72f5012a80>, <Element a at 0x72f5012ad0>, <Element a at 0x72f5012b20>, <Element a at 0x72f5012b70>, <Element a at 0x72f5012bc0>]
+[<Element a at 0x6f628736b0>, <Element a at 0x6f628be6c0>, <Element a at 0x6f628be760>, <Element a at 0x6f628be7b0>, <Element a at 0x6f628be800>, <Element a at 0x6f628be850>, <Element a at 0x6f628be8a0>, <Element a at 0x6f628be8f0>, <Element a at 0x6f628be940>, <Element a at 0x6f628be990>, <Element a at 0x6f628be9e0>, <Element a at 0x6f628bea30>, <Element a at 0x6f628bea80>, <Element a at 0x6f628bead0>, <Element a at 0x6f628beb20>, <Element a at 0x6f628beb70>, <Element a at 0x6f628bebc0>, <Element a at 0x6f628bec10>]
 False
 ```
 
 ## iprint
 
 `iprint(*args, color=None, sort_dicts=False, **kwargs)`
 
@@ -1494,16 +1525,16 @@
 print(list(irange('a', 'z', 10)))  
 print(list(irange(1, '7')))  
 print(list(irange(10, 5)))  
 ```
 
 Output:
 ```py
-<generator object irange at 0x72f4f9aac0>
-<generator object irange at 0x72f4f9aac0>
+<generator object irange at 0x6f62846ac0>
+<generator object irange at 0x6f62846ac0>
 ['a', 'k', 'u']
 [1, 2, 3, 4, 5, 6, 7]
 [10, 9, 8, 7, 6, 5]
 ```
 
 ## ireplace
 
@@ -1538,15 +1569,15 @@
 ```python  
 print(iscandir())  
 print(list(iscandir("./", recursive=False, scan_file=False)))  
 ```
 
 Output:
 ```py
-<generator object iscandir at 0x72f4fd0840>
+<generator object iscandir at 0x6f6287c840>
 [PosixPath('.git'), PosixPath('.vscode'), PosixPath('pypipr'), PosixPath('__pycache__'), PosixPath('dist')]
 ```
 
 ## isplit
 
 `isplit(text, separator='', include_separator=False)`
 
@@ -1595,15 +1626,15 @@
 print(ExampleComparePerformance().compare_performance())  
 print(ExampleComparePerformance().compare_performance())  
 print(ExampleComparePerformance().compare_performance())  
 ```
 
 Output:
 ```py
-{'a': <generator object ExampleComparePerformance.a.<locals>.<genexpr> at 0x72f4fe8520>,
+{'a': <generator object ExampleComparePerformance.a.<locals>.<genexpr> at 0x6f62890520>,
  'b': (0, 1, 2, 3, 4, 5, 6, 7, 8, 9),
  'c': [0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
  'd': [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
@@ -1727,7 +1758,8 @@
 class ExampleAPIView(APIMixinView, View):  
     pass  
 ```
 
 ## PintUregQuantity
 
 `PintUregQuantity(value, units=None)`
+
```

### Comparing `pypipr-1.0.91/PKG-INFO` & `pypipr-1.0.92/readme.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: pypipr
-Version: 1.0.91
-Summary: The Python Package Index Project
-Author: ufiapjj
-Author-email: ufiapjj@gmail.com
-Requires-Python: >=3.9
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: colorama
-Requires-Dist: cssselect
-Requires-Dist: django
-Requires-Dist: getch ; platform_system == "Linux"
-Requires-Dist: lxml
-Requires-Dist: pint
-Requires-Dist: pyyaml
-Requires-Dist: requests
-Requires-Dist: tzdata
-Description-Content-Type: text/markdown
-
 
 # About
 The Python Package Index Project (pypipr)
 
 pypi : https://pypi.org/project/pypipr
 
 
@@ -97,15 +74,15 @@
 arr = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]  
 print(chunk_array(arr, 5))  
 print(list(chunk_array(arr, 5)))  
 ```
 
 Output:
 ```py
-<generator object chunk_array at 0x72f4fd0240>
+<generator object chunk_array at 0x6f6287c240>
 [[2, 3, 12, 3, 3], [42, 42, 1, 43, 2], [42, 41, 4, 24, 32], [42, 3, 12, 32, 42], [42]]
 ```
 
 ## create_folder
 
 `create_folder(folder_name)`
 
@@ -148,17 +125,17 @@
 print(datetime_now("Asia/Jakarta"))  
 print(datetime_now("GMT"))  
 print(datetime_now("Etc/GMT+7"))  
 ```
 
 Output:
 ```py
-2024-04-24 11:39:26.061287+07:00
-2024-04-24 04:39:26.061634+00:00
-2024-04-23 21:39:26.062212-07:00
+2024-04-24 15:04:28.168838+07:00
+2024-04-24 08:04:28.169670+00:00
+2024-04-24 01:04:28.172534-07:00
 ```
 
 ## dict_first
 
 `dict_first(d: dict, remove=False)`
 
 Mengambil nilai (key, value) pertama dari dictionary dalam bentuk tuple.  
@@ -217,15 +194,15 @@
 ```python  
 var = [1, None, False, 0, "0", True, {}, ['eee']]  
 print(filter_empty(var))  
 ```
 
 Output:
 ```py
-<generator object filter_empty at 0x72f4f66d40>
+<generator object filter_empty at 0x6f6280ed40>
 ```
 
 ## get_by_index
 
 `get_by_index(obj, index, on_error=None)`
 
 Mendapatkan value dari object berdasarkan indexnya.  
@@ -263,16 +240,16 @@
   
 print(get_class_method(ExampleGetClassMethod))  
 print(list(get_class_method(ExampleGetClassMethod)))  
 ```
 
 Output:
 ```py
-<generator object get_class_method at 0x72f4f67010>
-[<function ExampleGetClassMethod.a at 0x730657e7a0>, <function ExampleGetClassMethod.b at 0x72f4fd9580>, <function ExampleGetClassMethod.c at 0x72f4fd9620>, <function ExampleGetClassMethod.d at 0x72f4fd96c0>]
+<generator object get_class_method at 0x6f6280f010>
+[<function ExampleGetClassMethod.a at 0x6f73cfe7a0>, <function ExampleGetClassMethod.b at 0x6f62885580>, <function ExampleGetClassMethod.c at 0x6f62885620>, <function ExampleGetClassMethod.d at 0x6f628856c0>]
 ```
 
 ## get_filemtime
 
 `get_filemtime(filename)`
 
 Mengambil informasi last modification time file dalam nano seconds  
@@ -389,15 +366,15 @@
 Output:
 ```py
 {'module': {'ibuiltins': <module 'pypipr.ibuiltins' from '/data/data/com.termux/files/home/pypipr/pypipr/ibuiltins/__init__.py'>,
             'iconsole': <module 'pypipr.iconsole' from '/data/data/com.termux/files/home/pypipr/pypipr/iconsole/__init__.py'>,
             'idjango': <module 'pypipr.idjango' from '/data/data/com.termux/files/home/pypipr/pypipr/idjango/__init__.py'>,
             'iengineering': <module 'pypipr.iengineering' from '/data/data/com.termux/files/home/pypipr/pypipr/iengineering/__init__.py'>,
             'ifunctions': <module 'pypipr.ifunctions' from '/data/data/com.termux/files/home/pypipr/pypipr/ifunctions/__init__.py'>,
-            'iflow': <module 'pypipr.iflow' (<_frozen_importlib_external.NamespaceLoader object at 0x72f921efd0>)>,
+            'iflow': <module 'pypipr.iflow' (<_frozen_importlib_external.NamespaceLoader object at 0x6f66608a10>)>,
             'asyncio': <module 'asyncio' from '/data/data/com.termux/files/usr/lib/python3.11/asyncio/__init__.py'>,
             'colorama': <module 'colorama' from '/data/data/com.termux/files/usr/lib/python3.11/site-packages/colorama/__init__.py'>,
             'datetime': <module 'datetime' from '/data/data/com.termux/files/usr/lib/python3.11/datetime.py'>,
             'functools': <module 'functools' from '/data/data/com.termux/files/usr/lib/python3.11/functools.py'>,
             'inspect': <module 'inspect' from '/data/data/com.termux/files/usr/lib/python3.11/inspect.py'>,
             'io': <module 'io' (frozen)>,
             'json': <module 'json' from '/data/data/com.termux/files/usr/lib/python3.11/json/__init__.py'>,
@@ -426,87 +403,87 @@
             'zoneinfo': <module 'zoneinfo' from '/data/data/com.termux/files/usr/lib/python3.11/zoneinfo/__init__.py'>},
  'class': {'ComparePerformance': <class 'pypipr.ibuiltins.ComparePerformance.ComparePerformance'>,
            'RunParallel': <class 'pypipr.ibuiltins.RunParallel.RunParallel'>,
            'APIMixinView': <class 'pypipr.idjango.APIMixinView.APIMixinView'>,
            'PintUregQuantity': <class 'pint.Quantity'>},
  'variable': {'LINUX': True,
               'WINDOWS': False,
-              'PintUreg': <pint.registry.UnitRegistry object at 0x7302ccb1d0>},
- 'function': {'avg': <function avg at 0x73065b6d40>,
-              'basename': <function basename at 0x730657e8e0>,
-              'chunk_array': <function chunk_array at 0x7302c01120>,
-              'create_folder': <function create_folder at 0x7302c01300>,
-              'datetime_from_string': <function datetime_from_string at 0x7302c014e0>,
-              'datetime_now': <function datetime_now at 0x7302ca9620>,
-              'dict_first': <function dict_first at 0x7302ca9580>,
-              'dirname': <function dirname at 0x7302ca94e0>,
-              'exit_if_empty': <function exit_if_empty at 0x7302c834c0>,
-              'filter_empty': <function filter_empty at 0x7302ca91c0>,
-              'get_by_index': <function get_by_index at 0x7302ca8ea0>,
-              'get_class_method': <function get_class_method at 0x7302ca8cc0>,
-              'get_filemtime': <function get_filemtime at 0x7302ca8b80>,
-              'get_filesize': <function get_filesize at 0x7302ca89a0>,
-              'is_empty': <function is_empty at 0x7302ca9260>,
-              'is_iterable': <function is_iterable at 0x7302ca8fe0>,
-              'is_valid_url': <function is_valid_url at 0x7302ca8860>,
-              'ivars': <function ivars at 0x7302ca87c0>,
-              'password_generator': <function password_generator at 0x7302ca8680>,
-              'random_bool': <function random_bool at 0x7302ca8400>,
-              'set_timeout': <function set_timeout at 0x7302cab7e0>,
-              'sets_ordered': <function sets_ordered at 0x7302cab920>,
-              'str_cmp': <function str_cmp at 0x7302cab9c0>,
-              'to_str': <function to_str at 0x7302ca8f40>,
-              'choices': <function choices at 0x7302caba60>,
-              'console_run': <function console_run at 0x7302cabce0>,
-              'input_char': <function input_char at 0x7302cabe20>,
-              'log': <function log at 0x7302cd0040>,
-              'print_colorize': <function print_colorize at 0x7302cd00e0>,
-              'print_dir': <function print_dir at 0x7302cd0220>,
-              'print_log': <function print_log at 0x7302cabec0>,
-              'print_to_last_line': <function print_to_last_line at 0x7302cabc40>,
-              'text_colorize': <function text_colorize at 0x7302cabd80>,
-              'batch_calculate': <function batch_calculate at 0x72f9235580>,
-              'batchmaker': <function batchmaker at 0x72f920e980>,
-              'calculate': <function calculate at 0x72f92362a0>,
-              'auto_reload': <function auto_reload at 0x72f9236480>,
-              'github_pull': <function github_pull at 0x72f9236020>,
-              'github_push': <function github_push at 0x72f9236700>,
-              'github_user': <function github_user at 0x72f9236a20>,
-              'pip_freeze_without_version': <function pip_freeze_without_version at 0x72f8f5a020>,
-              'poetry_publish': <function poetry_publish at 0x72f8f5a160>,
-              'poetry_update_version': <function poetry_update_version at 0x72f8f7a980>,
-              'iargv': <function iargv at 0x72f51a00e0>,
-              'idumps': <function idumps at 0x72f51a0220>,
-              'idumps_html': <function idumps_html at 0x72f5204c20>,
-              'ienv': <function ienv at 0x72f51a0360>,
-              'iexec': <function iexec at 0x72f5204ea0>,
-              'ijoin': <function ijoin at 0x72f8f59ee0>,
-              'iloads': <function iloads at 0x72f5204f40>,
-              'iloads_html': <function iloads_html at 0x72f52051c0>,
-              'iopen': <function iopen at 0x72f8f5a200>,
-              'iprint': <function iprint at 0x72f51a0180>,
-              'irange': <function irange at 0x72f92363e0>,
-              'ireplace': <function ireplace at 0x72f5205080>,
-              'iscandir': <function iscandir at 0x72f5206e80>,
-              'isplit': <function isplit at 0x72f5206f20>}}
+              'PintUreg': <pint.registry.UnitRegistry object at 0x6f6ebab710>},
+ 'function': {'avg': <function avg at 0x6f73d36d40>,
+              'basename': <function basename at 0x6f73cfe8e0>,
+              'chunk_array': <function chunk_array at 0x6f6eae1120>,
+              'create_folder': <function create_folder at 0x6f6eae1300>,
+              'datetime_from_string': <function datetime_from_string at 0x6f6eae14e0>,
+              'datetime_now': <function datetime_now at 0x6f6eb89620>,
+              'dict_first': <function dict_first at 0x6f6eb89580>,
+              'dirname': <function dirname at 0x6f6eb894e0>,
+              'exit_if_empty': <function exit_if_empty at 0x6f6eb634c0>,
+              'filter_empty': <function filter_empty at 0x6f6eb891c0>,
+              'get_by_index': <function get_by_index at 0x6f6eb88ea0>,
+              'get_class_method': <function get_class_method at 0x6f6eb88cc0>,
+              'get_filemtime': <function get_filemtime at 0x6f6eb88b80>,
+              'get_filesize': <function get_filesize at 0x6f6eb889a0>,
+              'is_empty': <function is_empty at 0x6f6eb89260>,
+              'is_iterable': <function is_iterable at 0x6f6eb88fe0>,
+              'is_valid_url': <function is_valid_url at 0x6f6eb88860>,
+              'ivars': <function ivars at 0x6f6eb887c0>,
+              'password_generator': <function password_generator at 0x6f6eb88680>,
+              'random_bool': <function random_bool at 0x6f6eb88400>,
+              'set_timeout': <function set_timeout at 0x6f6eb8b7e0>,
+              'sets_ordered': <function sets_ordered at 0x6f6eb8b920>,
+              'str_cmp': <function str_cmp at 0x6f6eb8b9c0>,
+              'to_str': <function to_str at 0x6f6eb88f40>,
+              'choices': <function choices at 0x6f6eb8ba60>,
+              'console_run': <function console_run at 0x6f6eb8bce0>,
+              'input_char': <function input_char at 0x6f6eb8be20>,
+              'log': <function log at 0x6f6ebb0040>,
+              'print_colorize': <function print_colorize at 0x6f6ebb00e0>,
+              'print_dir': <function print_dir at 0x6f6ebb0220>,
+              'print_log': <function print_log at 0x6f6eb8bec0>,
+              'print_to_last_line': <function print_to_last_line at 0x6f6eb8bc40>,
+              'text_colorize': <function text_colorize at 0x6f6eb8bd80>,
+              'batch_calculate': <function batch_calculate at 0x6f66731580>,
+              'batchmaker': <function batchmaker at 0x6f6670a980>,
+              'calculate': <function calculate at 0x6f667322a0>,
+              'auto_reload': <function auto_reload at 0x6f66732480>,
+              'github_pull': <function github_pull at 0x6f66732020>,
+              'github_push': <function github_push at 0x6f66732700>,
+              'github_user': <function github_user at 0x6f66732a20>,
+              'pip_freeze_without_version': <function pip_freeze_without_version at 0x6f6645e020>,
+              'poetry_publish': <function poetry_publish at 0x6f6645e160>,
+              'poetry_update_version': <function poetry_update_version at 0x6f6647e980>,
+              'iargv': <function iargv at 0x6f62a4c0e0>,
+              'idumps': <function idumps at 0x6f62a4c220>,
+              'idumps_html': <function idumps_html at 0x6f62ab4c20>,
+              'ienv': <function ienv at 0x6f62a4c360>,
+              'iexec': <function iexec at 0x6f62ab4ea0>,
+              'ijoin': <function ijoin at 0x6f6645dee0>,
+              'iloads': <function iloads at 0x6f62ab4f40>,
+              'iloads_html': <function iloads_html at 0x6f62ab51c0>,
+              'iopen': <function iopen at 0x6f6645e200>,
+              'iprint': <function iprint at 0x6f62a4c180>,
+              'irange': <function irange at 0x6f667323e0>,
+              'ireplace': <function ireplace at 0x6f62ab5080>,
+              'iscandir': <function iscandir at 0x6f62ab6e80>,
+              'isplit': <function isplit at 0x6f62ab6f20>}}
 ```
 
 ## password_generator
 
 `password_generator(length=8, characters='abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~')`
 
 Membuat pssword secara acak  
   
 ```python  
 print(password_generator())  
 ```
 
 Output:
 ```py
-Uy}-6-Qh
+_Pq4e5\d
 ```
 
 ## random_bool
 
 `random_bool()`
 
 Menghasilkan nilai random True atau False.  
@@ -538,15 +515,15 @@
 print(x)  
 print("menghentikan timeout 7")  
 x.cancel()  
 ```
 
 Output:
 ```py
-<Timer(Thread-2, started 493713603824)>
+<Timer(Thread-2, started 478370839792)>
 menghentikan timeout 7
 ```
 
 ## sets_ordered
 
 `sets_ordered(iterator)`
 
@@ -556,15 +533,15 @@
 array = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]  
 print(sets_ordered(array))  
 print(list(sets_ordered(array)))  
 ```
 
 Output:
 ```py
-<generator object sets_ordered at 0x72f4fe41e0>
+<generator object sets_ordered at 0x6f628901e0>
 [2, 3, 12, 42, 1, 43, 41, 4, 24, 32]
 ```
 
 ## str_cmp
 
 `str_cmp(t1, t2)`
 
@@ -710,29 +687,29 @@
              __doc__ : Path subclass for non-Windows systems.
 
     On a POSIX system, instantiating a Path should return this object.
     
            __enter__ : https:/www.google.com
           __fspath__ : https:/www.google.com
         __getstate__ : (None, {'_drv': '', '_root': '', '_parts': ['https:', 'www.google.com'], '_str': 'https:/www.google.com'})
-            __hash__ : 1324913689339074732
+            __hash__ : -7677454752077529173
             __init__ : None
    __init_subclass__ : None
           __module__ : pathlib
           __reduce__ : (<class 'pathlib.PosixPath'>, ('https:', 'www.google.com'))
             __repr__ : PosixPath('https:/www.google.com')
           __sizeof__ : 72
            __slots__ : ()
              __str__ : https:/www.google.com
     __subclasshook__ : NotImplemented
       _cached_cparts : ['https:', 'www.google.com']
              _cparts : ['https:', 'www.google.com']
                 _drv : 
-            _flavour : <pathlib._PosixFlavour object at 0x7302c7c2d0>
-               _hash : 1324913689339074732
+            _flavour : <pathlib._PosixFlavour object at 0x6f6eb5c650>
+               _hash : -7677454752077529173
               _parts : ['https:', 'www.google.com']
                _root : 
                 _str : https:/www.google.com
             absolute : /data/data/com.termux/files/home/pypipr/https:/www.google.com
               anchor : 
             as_posix : https:/www.google.com
                  cwd : /data/data/com.termux/files/home/pypipr
@@ -746,15 +723,15 @@
               is_dir : False
              is_fifo : False
              is_file : False
             is_mount : False
          is_reserved : False
            is_socket : False
           is_symlink : False
-             iterdir : <generator object Path.iterdir at 0x72f4fbcc80>
+             iterdir : <generator object Path.iterdir at 0x6f62868c80>
             joinpath : https:/www.google.com
                 name : www.google.com
               parent : https:
              parents : <PosixPath.parents>
                parts : ('https:', 'www.google.com')
              resolve : /data/data/com.termux/files/home/pypipr/https:/www.google.com
                 root : 
@@ -813,15 +790,15 @@
 ```python  
 print(batch_calculate("{1 10} m ** {1 3}"))  
 print(list(batch_calculate("{1 10} m ** {1 3}")))  
 ```
 
 Output:
 ```py
-<generator object batch_calculate at 0x72f4f67b50>
+<generator object batch_calculate at 0x6f6280fb50>
 [('1 m ** 1', <Quantity(1, 'meter')>), ('1 m ** 2', <Quantity(1, 'meter ** 2')>), ('1 m ** 3', <Quantity(1, 'meter ** 3')>), ('2 m ** 1', <Quantity(2, 'meter')>), ('2 m ** 2', <Quantity(2, 'meter ** 2')>), ('2 m ** 3', <Quantity(2, 'meter ** 3')>), ('3 m ** 1', <Quantity(3, 'meter')>), ('3 m ** 2', <Quantity(3, 'meter ** 2')>), ('3 m ** 3', <Quantity(3, 'meter ** 3')>), ('4 m ** 1', <Quantity(4, 'meter')>), ('4 m ** 2', <Quantity(4, 'meter ** 2')>), ('4 m ** 3', <Quantity(4, 'meter ** 3')>), ('5 m ** 1', <Quantity(5, 'meter')>), ('5 m ** 2', <Quantity(5, 'meter ** 2')>), ('5 m ** 3', <Quantity(5, 'meter ** 3')>), ('6 m ** 1', <Quantity(6, 'meter')>), ('6 m ** 2', <Quantity(6, 'meter ** 2')>), ('6 m ** 3', <Quantity(6, 'meter ** 3')>), ('7 m ** 1', <Quantity(7, 'meter')>), ('7 m ** 2', <Quantity(7, 'meter ** 2')>), ('7 m ** 3', <Quantity(7, 'meter ** 3')>), ('8 m ** 1', <Quantity(8, 'meter')>), ('8 m ** 2', <Quantity(8, 'meter ** 2')>), ('8 m ** 3', <Quantity(8, 'meter ** 3')>), ('9 m ** 1', <Quantity(9, 'meter')>), ('9 m ** 2', <Quantity(9, 'meter ** 2')>), ('9 m ** 3', <Quantity(9, 'meter ** 3')>), ('10 m ** 1', <Quantity(10, 'meter')>), ('10 m ** 2', <Quantity(10, 'meter ** 2')>), ('10 m ** 3', <Quantity(10, 'meter ** 3')>)]
 ```
 
 ## batchmaker
 
 `batchmaker(pattern: str)`
 
@@ -838,15 +815,15 @@
 s = "Urutan {1/6/3} dan {10:9} dan {j k} dan {Z - A - 15} saja."  
 print(batchmaker(s))  
 print(list(batchmaker(s)))  
 ```
 
 Output:
 ```py
-<generator object batchmaker at 0x72f4fd4040>
+<generator object batchmaker at 0x6f62880040>
 ['Urutan 1 dan 10 dan j dan Z saja.', 'Urutan 1 dan 10 dan j dan K saja.', 'Urutan 1 dan 10 dan k dan Z saja.', 'Urutan 1 dan 10 dan k dan K saja.', 'Urutan 1 dan 9 dan j dan Z saja.', 'Urutan 1 dan 9 dan j dan K saja.', 'Urutan 1 dan 9 dan k dan Z saja.', 'Urutan 1 dan 9 dan k dan K saja.', 'Urutan 4 dan 10 dan j dan Z saja.', 'Urutan 4 dan 10 dan j dan K saja.', 'Urutan 4 dan 10 dan k dan Z saja.', 'Urutan 4 dan 10 dan k dan K saja.', 'Urutan 4 dan 9 dan j dan Z saja.', 'Urutan 4 dan 9 dan j dan K saja.', 'Urutan 4 dan 9 dan k dan Z saja.', 'Urutan 4 dan 9 dan k dan K saja.']
 ```
 
 ## calculate
 
 `calculate(teks)`
 
@@ -1202,15 +1179,15 @@
     recursive_flat=True))  
 print(ijoin(arr, separator='</div>\n<div>', start='<div>', end='</div>'))  
 print(ijoin(10, ' '))  
 ```
 
 Output:
 ```py
-dfs, weq, qweqw, asd
+asd, dfs, qweqw, weq
 ,ini,path,seperti,url,
 ini,path,seperti,url
 <li>satu</li>
 <li>12</li>
 <li>34</li>
 <li>56</li>
 <li>tiga</li>
@@ -1268,17 +1245,17 @@
 pprint.pprint(iloads_html(iopen("https://harga-emas.org/1-gram/")), depth=10)  
 ```
 
 Output:
 ```py
 (['Home', 'Emas 1 Gram', 'History', 'Trend', 'Perak 1 Gram', 'Pluang'],
  [['Harga Emas Hari Ini - Rabu, 24 April 2024'],
-  ['Spot Emas USD↓2.327,60 (-2,31) / oz',
+  ['Spot Emas USD↓2.320,94 (-8,97) / oz',
    'Kurs IDR↑16.244,00 (+20,00) / USD',
-   'Emas IDR↑1.215.605 (+292) / gr'],
+   'Emas IDR↓1.212.127 (-3.186) / gr'],
   ['LM Antam (Jual)↓1.320.000 (-5.000) / gr',
    'LM Antam (Beli)↓1.218.000 (-5.000) / gr']],
  [['Harga Emas Hari Ini'],
   ['Gram', 'Gedung Antam Jakarta', 'Pegadaian'],
   ['per Gram (Rp)', 'per Batangan (Rp)', 'per Gram (Rp)', 'per Batangan (Rp)'],
   ['1000',
    '1.261 (-5)',
@@ -1341,108 +1318,116 @@
    '1.208.000 (+8.000)',
    '604.000 (+4.000)'],
   ['Update harga LM Antam :24 April 2024, pukul 08:12Harga pembelian kembali '
    ':Rp. 1.218.000/gram (-5.000)',
    'Update harga LM Pegadaian :31 Agustus 2023']],
  [['Spot Harga Emas Hari Ini (Market Open)'],
   ['Satuan', 'USD', 'Kurs\xa0Dollar', 'IDR'],
-  ['Ounce\xa0(oz)', '2.327,60 (-2,31)', '16.244,00 (+20,00)', '37.809.534'],
-  ['Gram\xa0(gr)', '74,83', '16.244,00', '1.215.605 (+292)'],
-  ['Kilogram\xa0(kg)', '74.834,08', '16.244,00', '1.215.604.760'],
-  ['Update harga emas :24 April 2024, pukul 11:39Update kurs :24 April 2024, '
-   'pukul 09:10']],
+  ['Ounce\xa0(oz)', '2.320,94 (-8,97)', '16.244,00 (+20,00)', '37.701.349'],
+  ['Gram\xa0(gr)', '74,62', '16.244,00', '1.212.127 (-3.186)'],
+  ['Kilogram\xa0(kg)', '74.619,95', '16.244,00', '1.212.126.530'],
+  ['Update harga emas :24 April 2024, pukul 15:04Update kurs :24 April 2024, '
+   'pukul 13:10']],
  [['Gram', 'UBS Gold 99.99%'],
   ['Jual', 'Beli'],
   ['/ Batang', '/ Gram', '/ Batang', '/ Gram'],
   ['100',
-   '126.212.000 (-500.000)',
-   '1.262.120 (-5.000)',
-   '123.735.000',
-   '1.237.350'],
+   '126.000.000 (-712.000)',
+   '1.260.000 (-7.120)',
+   '124.485.000 (+750.000)',
+   '1.244.850 (+7.500)'],
   ['50',
-   '63.145.000 (-250.000)',
-   '1.262.900 (-5.000)',
-   '61.920.000',
-   '1.238.400'],
+   '63.100.000 (-295.000)',
+   '1.262.000 (-5.900)',
+   '62.295.000 (+375.000)',
+   '1.245.900 (+7.500)'],
   ['25',
-   '31.612.000 (-125.000)',
-   '1.264.480 (-5.000)',
-   '31.062.500',
-   '1.242.500'],
+   '31.600.000 (-137.000)',
+   '1.264.000 (-5.480)',
+   '31.250.000 (+187.500)',
+   '1.250.000 (+7.500)'],
   ['10',
-   '12.695.000 (-50.000)',
-   '1.269.500 (-5.000)',
-   '12.475.000',
-   '1.247.500'],
-  ['5', '6.375.000 (-25.000)', '1.275.000 (-5.000)', '6.289.500', '1.257.900'],
-  ['1', '1.320.000 (-5.000)', '1.320.000 (-5.000)', '1.290.500', '1.290.500'],
-  ['', 'Update :24 April 2024, pukul 10:55']],
+   '12.680.000 (-65.000)',
+   '1.268.000 (-6.500)',
+   '12.550.000 (+75.000)',
+   '1.255.000 (+7.500)'],
+  ['5',
+   '6.365.000 (-35.000)',
+   '1.273.000 (-7.000)',
+   '6.327.000 (+37.500)',
+   '1.265.400 (+7.500)'],
+  ['1',
+   '1.320.000 (-5.000)',
+   '1.320.000 (-5.000)',
+   '1.298.000 (+7.500)',
+   '1.298.000 (+7.500)'],
+  ['', 'Update :24 April 2024, pukul 13:02']],
  [['Konversi Satuan'],
   ['Satuan', 'Ounce (oz)', 'Gram (gr)', 'Kilogram (kg)'],
   ['Ounce\xa0(oz)', '1', '31,1034767696', '0,0311034768'],
   ['Gram\xa0(gr)', '0,0321507466', '1', '0.001'],
   ['Kilogram\xa0(kg)', '32,1507466000', '1.000', '1']],
  [['Pergerakan Harga Emas Dunia'],
   ['Waktu', 'Emas'],
   ['Unit', 'USD', 'IDR'],
   ['Angka', '+/-', 'Angka', '+/-'],
   ['Hari Ini', 'Kurs', '', '', '16.224', '+20+0,12%'],
-  ['oz', '2.329,91', '-2,31-0,10%', '37.800.460', '+9.075+0,02%'],
-  ['gr', '74,91', '-0,07-0,10%', '1.215.313', '+292+0,02%'],
+  ['oz', '2.329,91', '-8,97-0,38%', '37.800.460', '-99.110-0,26%'],
+  ['gr', '74,91', '-0,29-0,38%', '1.215.313', '-3.186-0,26%'],
   ['30 Hari', 'Kurs', '', '', '15.773', '+471+2,99%'],
-  ['oz', '2.175,55', '+152,05+6,99%', '34.314.950', '+3.494.584+10,18%'],
-  ['gr', '69,95', '+4,89+6,99%', '1.103.251', '+112.353+10,18%'],
+  ['oz', '2.175,55', '+145,39+6,68%', '34.314.950', '+3.386.399+9,87%'],
+  ['gr', '69,95', '+4,67+6,68%', '1.103.251', '+108.875+9,87%'],
   ['2 Bulan', 'Kurs', '', '', '15.630', '+614+3,93%'],
-  ['oz', '2.035,57', '+292,03+14,35%', '31.815.959', '+5.993.575+18,84%'],
-  ['gr', '65,45', '+9,39+14,35', '1.022.907', '+192.698+18,84%'],
+  ['oz', '2.035,57', '+285,37+14,02%', '31.815.959', '+5.885.390+18,50%'],
+  ['gr', '65,45', '+9,17+14,02', '1.022.907', '+189.220+18,50%'],
   ['6 Bulan', 'Kurs', '', '', '15.933', '+311+1,95%'],
-  ['oz', '1.983,13', '+344,47+17,37%', '31.597.210', '+6.212.324+19,66%'],
-  ['gr', '63,76', '+11,07+17,37%', '1.015.874', '+199.731+19,66%'],
+  ['oz', '1.983,13', '+337,81+17,03%', '31.597.210', '+6.104.139+19,32%'],
+  ['gr', '63,76', '+10,86+17,03%', '1.015.874', '+196.253+19,32%'],
   ['1 Tahun', 'Kurs', '', '', '15.731', '+513+3,26%'],
-  ['oz', '1.823,86', '+503,74+27,62%', '28.691.142', '+9.118.393+31,78%'],
-  ['gr', '58,64', '+16,20+27,62%', '922.442', '+293.163+31,78%'],
+  ['oz', '1.823,86', '+497,08+27,25%', '28.691.142', '+9.010.208+31,40%'],
+  ['gr', '58,64', '+15,98+27,25%', '922.442', '+289.685+31,40%'],
   ['2 Tahun', 'Kurs', '', '', '14.361', '+1.883+13,11%'],
-  ['oz', '1.896,13', '+431,47+22,76%', '27.230.342', '+10.579.193+38,85%'],
-  ['gr', '60,96', '+13,87+22,76%', '875.476', '+340.129+38,85%'],
+  ['oz', '1.896,13', '+424,81+22,40%', '27.230.342', '+10.471.007+38,45%'],
+  ['gr', '60,96', '+13,66+22,40%', '875.476', '+336.651+38,45%'],
   ['3 Tahun', 'Kurs', '', '', '14.530', '+1.714+11,80%'],
-  ['oz', '1.777,11', '+550,49+30,98%', '25.821.408', '+11.988.126+46,43%'],
-  ['gr', '57,14', '+17,70+30,98%', '830.178', '+385.427+46,43%'],
+  ['oz', '1.777,11', '+543,83+30,60%', '25.821.408', '+11.879.941+46,01%'],
+  ['gr', '57,14', '+17,48+30,60%', '830.178', '+381.949+46,01%'],
   ['5 Tahun', 'Kurs', '', '', '14.188', '+2.056+14,49%'],
-  ['oz', '1.288,10', '+1.039,50+80,70%', '18.275.563', '+19.533.972+106,89%'],
-  ['gr', '41,41', '+33,42+80,70%', '587.573', '+628.032+106,89%']])
+  ['oz', '1.288,10', '+1.032,84+80,18%', '18.275.563', '+19.425.787+106,29%'],
+  ['gr', '41,41', '+33,21+80,18%', '587.573', '+624.554+106,29%']])
 (['Home', 'Emas 1 Gram', 'History', 'Trend', 'Perak 1 Gram', 'Pluang'],
  [[''],
   ['Emas 24 KaratHarga Emas 1 Gram', ''],
-  ['USD', '74,83↓', '-0,08-0,11%'],
-  ['KURS', '16.151,15↑', '+4,25+0,03%'],
-  ['IDR', '1.208.656,42↓', '-881,15-0,07%'],
-  ['Rabu, 24 April 2024 11:39']],
+  ['USD', '74,62↓', '-0,29-0,39%'],
+  ['KURS', '16.171,45↑', '+24,55+0,15%'],
+  ['IDR', '1.206.712,85↓', '-2.824,72-0,23%'],
+  ['Rabu, 24 April 2024 15:04']],
  [[''],
   ['Emas 1 Gram (IDR)Emas 1 Gram (USD)Kurs USD-IDR',
    'Hari Ini',
    '1 Bulan',
    '1 Tahun',
    '5 Tahun',
    'Max',
    '']],
  [['Pergerakkan Harga Emas 1 Gram'],
   ['', 'Penutupan Kemarin', 'Pergerakkan Hari Ini', 'Rata-rata'],
-  ['USD', '74,91', '74,83 - 74,91', '74,87'],
-  ['KURS', '16.146,90', '16.146,90 - 16.151,15', '16.149,03'],
-  ['IDR', '1.209.537,57', '1.208.656,42 - 1.209.537,57', '1.209.097,00'],
+  ['USD', '74,91', '74,62 - 74,91', '74,77'],
+  ['KURS', '16.146,90', '16.146,90 - 16.171,45', '16.159,18'],
+  ['IDR', '1.209.537,57', '1.206.712,85 - 1.209.537,57', '1.208.125,21'],
   [''],
   ['', 'Awal Tahun', 'Pergerakkan YTD', '+/- YTD'],
-  ['USD', '66,32', '64,07 - 77,14', '+8,51 (12,83%)'],
-  ['KURS', '15.390,10', '15.390,00 - 16.307,80', '+761,05 (4,95%)'],
-  ['IDR', '1.020.729,53', '997.660,12 - 1.256.829,06', '+187.926,89 (18,41%)'],
+  ['USD', '66,32', '64,07 - 77,14', '+8,30 (12,52%)'],
+  ['KURS', '15.390,10', '15.390,00 - 16.307,80', '+781,35 (5,08%)'],
+  ['IDR', '1.020.729,53', '997.660,12 - 1.256.829,06', '+185.983,32 (18,22%)'],
   [''],
   ['', 'Tahun Lalu / 52 Minggu', 'Pergerakkan 52 Minggu', '+/- 52 Minggu'],
-  ['USD', '63,76', '58,43 - 77,14', '+11,07 (17,36%)'],
-  ['KURS', '14.936,00', '14.669,40 - 16.307,80', '+1.215,15 (8,14%)'],
-  ['IDR', '952.339,68', '912.925,68 - 1.256.829,06', '+256.316,74 (26,91%)']])
+  ['USD', '63,76', '58,43 - 77,14', '+10,86 (17,03%)'],
+  ['KURS', '14.936,00', '14.669,40 - 16.307,80', '+1.235,45 (8,27%)'],
+  ['IDR', '952.339,68', '912.925,68 - 1.256.829,06', '+254.373,17 (26,71%)']])
 ```
 
 ## iopen
 
 `iopen(path, data=None, regex=None, css_select=None, xpath=None, file_append=False)`
 
 Membaca atau Tulis pada path yang bisa merupakan FILE maupun URL.  
@@ -1476,15 +1461,15 @@
 print(iopen("https://www.google.com/", dict(coba="dulu"), xpath="//a"))  
 ```
 
 Output:
 ```py
 8
 ['mana', 'aja']
-[<Element a at 0x72f4fc6f80>, <Element a at 0x72f5012670>, <Element a at 0x72f5012710>, <Element a at 0x72f5012760>, <Element a at 0x72f50127b0>, <Element a at 0x72f5012800>, <Element a at 0x72f5012850>, <Element a at 0x72f50128a0>, <Element a at 0x72f50128f0>, <Element a at 0x72f5012940>, <Element a at 0x72f5012990>, <Element a at 0x72f50129e0>, <Element a at 0x72f5012a30>, <Element a at 0x72f5012a80>, <Element a at 0x72f5012ad0>, <Element a at 0x72f5012b20>, <Element a at 0x72f5012b70>, <Element a at 0x72f5012bc0>]
+[<Element a at 0x6f628736b0>, <Element a at 0x6f628be6c0>, <Element a at 0x6f628be760>, <Element a at 0x6f628be7b0>, <Element a at 0x6f628be800>, <Element a at 0x6f628be850>, <Element a at 0x6f628be8a0>, <Element a at 0x6f628be8f0>, <Element a at 0x6f628be940>, <Element a at 0x6f628be990>, <Element a at 0x6f628be9e0>, <Element a at 0x6f628bea30>, <Element a at 0x6f628bea80>, <Element a at 0x6f628bead0>, <Element a at 0x6f628beb20>, <Element a at 0x6f628beb70>, <Element a at 0x6f628bebc0>, <Element a at 0x6f628bec10>]
 False
 ```
 
 ## iprint
 
 `iprint(*args, color=None, sort_dicts=False, **kwargs)`
 
@@ -1517,16 +1502,16 @@
 print(list(irange('a', 'z', 10)))  
 print(list(irange(1, '7')))  
 print(list(irange(10, 5)))  
 ```
 
 Output:
 ```py
-<generator object irange at 0x72f4f9aac0>
-<generator object irange at 0x72f4f9aac0>
+<generator object irange at 0x6f62846ac0>
+<generator object irange at 0x6f62846ac0>
 ['a', 'k', 'u']
 [1, 2, 3, 4, 5, 6, 7]
 [10, 9, 8, 7, 6, 5]
 ```
 
 ## ireplace
 
@@ -1561,15 +1546,15 @@
 ```python  
 print(iscandir())  
 print(list(iscandir("./", recursive=False, scan_file=False)))  
 ```
 
 Output:
 ```py
-<generator object iscandir at 0x72f4fd0840>
+<generator object iscandir at 0x6f6287c840>
 [PosixPath('.git'), PosixPath('.vscode'), PosixPath('pypipr'), PosixPath('__pycache__'), PosixPath('dist')]
 ```
 
 ## isplit
 
 `isplit(text, separator='', include_separator=False)`
 
@@ -1618,15 +1603,15 @@
 print(ExampleComparePerformance().compare_performance())  
 print(ExampleComparePerformance().compare_performance())  
 print(ExampleComparePerformance().compare_performance())  
 ```
 
 Output:
 ```py
-{'a': <generator object ExampleComparePerformance.a.<locals>.<genexpr> at 0x72f4fe8520>,
+{'a': <generator object ExampleComparePerformance.a.<locals>.<genexpr> at 0x6f62890520>,
  'b': (0, 1, 2, 3, 4, 5, 6, 7, 8, 9),
  'c': [0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
  'd': [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
 {'a': 0, 'b': 0, 'c': 0, 'd': 0}
@@ -1750,8 +1735,7 @@
 class ExampleAPIView(APIMixinView, View):  
     pass  
 ```
 
 ## PintUregQuantity
 
 `PintUregQuantity(value, units=None)`
-
```

