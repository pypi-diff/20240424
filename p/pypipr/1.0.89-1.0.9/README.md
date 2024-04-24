# Comparing `tmp/pypipr-1.0.89.tar.gz` & `tmp/pypipr-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypipr-1.0.89.tar", max compression
+gzip compressed data, was "pypipr-1.0.9.tar", max compression
```

## Comparing `pypipr-1.0.89.tar` & `pypipr-1.0.9.tar`

### file list

```diff
@@ -1,75 +1,14 @@
--rw-r--r--   0        0        0     3347 2024-04-24 04:15:24.115050 pypipr-1.0.89/pypipr/__init__.py
--rw-r--r--   0        0        0     2229 2024-03-17 17:38:37.508083 pypipr-1.0.89/pypipr/ibuiltins/ComparePerformance.py
--rw-r--r--   0        0        0      100 2024-03-17 17:38:37.508083 pypipr-1.0.89/pypipr/ibuiltins/LINUX.py
--rw-r--r--   0        0        0     7358 2024-04-23 10:50:10.015024 pypipr-1.0.89/pypipr/ibuiltins/RunParallel.py
--rw-r--r--   0        0        0      105 2024-03-17 17:38:37.508083 pypipr-1.0.89/pypipr/ibuiltins/WINDOWS.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.508083 pypipr-1.0.89/pypipr/ibuiltins/__init__.py
--rw-r--r--   0        0        0      218 2024-03-17 17:38:37.508083 pypipr-1.0.89/pypipr/ibuiltins/avg.py
--rw-r--r--   0        0        0      194 2024-03-17 17:38:37.508083 pypipr-1.0.89/pypipr/ibuiltins/basename.py
--rw-r--r--   0        0        0      385 2024-04-22 13:19:16.948654 pypipr-1.0.89/pypipr/ibuiltins/chunk_array.py
--rw-r--r--   0        0        0      500 2024-03-17 17:38:37.508083 pypipr-1.0.89/pypipr/ibuiltins/create_folder.py
--rw-r--r--   0        0        0      466 2024-03-17 17:38:37.508083 pypipr-1.0.89/pypipr/ibuiltins/datetime_from_string.py
--rw-r--r--   0        0        0      476 2024-03-17 17:38:37.508083 pypipr-1.0.89/pypipr/ibuiltins/datetime_now.py
--rw-r--r--   0        0        0      377 2024-03-17 17:38:37.508083 pypipr-1.0.89/pypipr/ibuiltins/dict_first.py
--rw-r--r--   0        0        0      229 2024-03-17 17:38:37.508083 pypipr-1.0.89/pypipr/ibuiltins/dirname.py
--rw-r--r--   0        0        0      321 2024-04-20 11:53:09.914721 pypipr-1.0.89/pypipr/ibuiltins/exit_if_empty.py
--rw-r--r--   0        0        0      543 2024-03-17 17:38:37.508083 pypipr-1.0.89/pypipr/ibuiltins/filter_empty.py
--rw-r--r--   0        0        0      335 2024-04-23 12:23:59.246031 pypipr-1.0.89/pypipr/ibuiltins/get_by_index.py
--rw-r--r--   0        0        0      639 2024-04-22 21:58:29.290425 pypipr-1.0.89/pypipr/ibuiltins/get_class_method.py
--rw-r--r--   0        0        0      227 2024-03-17 17:38:37.508083 pypipr-1.0.89/pypipr/ibuiltins/get_filemtime.py
--rw-r--r--   0        0        0      196 2024-03-17 17:38:37.508083 pypipr-1.0.89/pypipr/ibuiltins/get_filesize.py
--rw-r--r--   0        0        0      683 2024-04-20 11:02:21.923096 pypipr-1.0.89/pypipr/ibuiltins/is_empty.py
--rw-r--r--   0        0        0      922 2024-03-17 17:38:37.508083 pypipr-1.0.89/pypipr/ibuiltins/is_iterable.py
--rw-r--r--   0        0        0     1008 2024-03-17 17:38:37.508083 pypipr-1.0.89/pypipr/ibuiltins/is_valid_url.py
--rw-r--r--   0        0        0      899 2024-04-23 09:16:42.841403 pypipr-1.0.89/pypipr/ibuiltins/ivars.py
--rw-r--r--   0        0        0      496 2024-03-17 17:38:37.508083 pypipr-1.0.89/pypipr/ibuiltins/password_generator.py
--rw-r--r--   0        0        0      405 2024-03-17 17:38:37.508083 pypipr-1.0.89/pypipr/ibuiltins/random_bool.py
--rw-r--r--   0        0        0      698 2024-03-17 17:38:37.512083 pypipr-1.0.89/pypipr/ibuiltins/set_timeout.py
--rw-r--r--   0        0        0      325 2024-03-17 17:38:37.512083 pypipr-1.0.89/pypipr/ibuiltins/sets_ordered.py
--rw-r--r--   0        0        0      377 2024-03-17 17:38:37.512083 pypipr-1.0.89/pypipr/ibuiltins/str_cmp.py
--rw-r--r--   0        0        0      597 2024-03-17 17:38:37.512083 pypipr-1.0.89/pypipr/ibuiltins/to_str.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.89/pypipr/iconsole/__init__.py
--rw-r--r--   0        0        0     1686 2024-03-17 17:38:37.512083 pypipr-1.0.89/pypipr/iconsole/choices.py
--rw-r--r--   0        0        0      525 2024-03-17 17:38:37.512083 pypipr-1.0.89/pypipr/iconsole/console_run.py
--rw-r--r--   0        0        0     1030 2024-04-23 12:02:12.950032 pypipr-1.0.89/pypipr/iconsole/input_char.py
--rw-r--r--   0        0        0     1041 2024-03-17 17:38:37.512083 pypipr-1.0.89/pypipr/iconsole/log.py
--rw-r--r--   0        0        0      474 2024-03-17 17:38:37.512083 pypipr-1.0.89/pypipr/iconsole/print_colorize.py
--rw-r--r--   0        0        0      930 2024-04-22 21:43:34.984645 pypipr-1.0.89/pypipr/iconsole/print_dir.py
--rw-r--r--   0        0        0      282 2024-04-22 21:44:47.788645 pypipr-1.0.89/pypipr/iconsole/print_log.py
--rw-r--r--   0        0        0      914 2024-04-24 02:48:07.180538 pypipr-1.0.89/pypipr/iconsole/print_to_last_line.py
--rw-r--r--   0        0        0      396 2024-03-17 17:38:37.512083 pypipr-1.0.89/pypipr/iconsole/text_colorize.py
--rw-r--r--   0        0        0     1093 2024-03-17 17:38:37.512083 pypipr-1.0.89/pypipr/idjango/APIMixinView.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.89/pypipr/idjango/__init__.py
--rw-r--r--   0        0        0      222 2024-03-17 17:38:37.512083 pypipr-1.0.89/pypipr/iengineering/PintUreg.py
--rw-r--r--   0        0        0      118 2024-03-17 17:38:37.512083 pypipr-1.0.89/pypipr/iengineering/PintUregQuantity.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.512083 pypipr-1.0.89/pypipr/iengineering/__init__.py
--rw-r--r--   0        0        0      695 2024-04-22 21:59:57.598425 pypipr-1.0.89/pypipr/iengineering/batch_calculate.py
--rw-r--r--   0        0        0     1277 2024-03-17 17:38:37.512083 pypipr-1.0.89/pypipr/iengineering/batchmaker.py
--rw-r--r--   0        0        0      805 2024-03-17 17:38:37.512083 pypipr-1.0.89/pypipr/iengineering/calculate.py
--rw-r--r--   0        0        0      966 2024-04-23 11:50:40.860964 pypipr-1.0.89/pypipr/iflow/auto_reload.py
--rw-r--r--   0        0        0      243 2024-03-17 17:38:37.516083 pypipr-1.0.89/pypipr/iflow/github_pull.py
--rw-r--r--   0        0        0      951 2024-03-17 17:38:37.516083 pypipr-1.0.89/pypipr/iflow/github_push.py
--rw-r--r--   0        0        0      600 2024-03-17 17:38:37.516083 pypipr-1.0.89/pypipr/iflow/github_user.py
--rw-r--r--   0        0        0      839 2024-04-20 02:24:51.624107 pypipr-1.0.89/pypipr/iflow/pip_freeze_without_version.py
--rw-r--r--   0        0        0      409 2024-03-17 17:38:37.516083 pypipr-1.0.89/pypipr/iflow/poetry_publish.py
--rw-r--r--   0        0        0      622 2024-03-17 17:38:37.516083 pypipr-1.0.89/pypipr/iflow/poetry_update_version.py
--rw-r--r--   0        0        0        0 2024-03-17 17:38:37.516083 pypipr-1.0.89/pypipr/ifunctions/__init__.py
--rw-r--r--   0        0        0      503 2024-04-23 11:45:29.548964 pypipr-1.0.89/pypipr/ifunctions/iargv.py
--rw-r--r--   0        0        0      748 2024-03-17 17:38:37.516083 pypipr-1.0.89/pypipr/ifunctions/idumps.py
--rw-r--r--   0        0        0     1423 2024-03-17 17:38:37.516083 pypipr-1.0.89/pypipr/ifunctions/idumps_html.py
--rw-r--r--   0        0        0      679 2024-04-23 11:41:52.328964 pypipr-1.0.89/pypipr/ifunctions/ienv.py
--rw-r--r--   0        0        0      465 2024-03-17 17:38:37.516083 pypipr-1.0.89/pypipr/ifunctions/iexec.py
--rw-r--r--   0        0        0     2069 2024-03-17 17:38:37.516083 pypipr-1.0.89/pypipr/ifunctions/ijoin.py
--rw-r--r--   0        0        0      638 2024-04-22 21:36:07.164645 pypipr-1.0.89/pypipr/ifunctions/iloads.py
--rw-r--r--   0        0        0     4146 2024-04-22 21:40:17.264645 pypipr-1.0.89/pypipr/ifunctions/iloads_html.py
--rw-r--r--   0        0        0     2808 2024-03-17 17:38:37.516083 pypipr-1.0.89/pypipr/ifunctions/iopen.py
--rw-r--r--   0        0        0      849 2024-04-22 21:41:31.764645 pypipr-1.0.89/pypipr/ifunctions/iprint.py
--rw-r--r--   0        0        0     2407 2024-03-17 17:38:37.516083 pypipr-1.0.89/pypipr/ifunctions/irange.py
--rw-r--r--   0        0        0      722 2024-03-17 17:38:37.516083 pypipr-1.0.89/pypipr/ifunctions/ireplace.py
--rw-r--r--   0        0        0      748 2024-04-23 09:11:14.125403 pypipr-1.0.89/pypipr/ifunctions/iscandir.py
--rw-r--r--   0        0        0      383 2024-03-17 17:38:37.520083 pypipr-1.0.89/pypipr/ifunctions/isplit.py
--rw-r--r--   0        0        0     1061 2024-04-20 02:38:18.131451 pypipr-1.0.89/pypipr/pypipr.py.bak
--rw-r--r--   0        0        0     1800 2024-04-23 13:05:42.093603 pypipr-1.0.89/pypipr/terminal.py
--rw-r--r--   0        0        0      544 2024-04-24 04:15:35.071050 pypipr-1.0.89/pyproject.toml
--rw-r--r--   0        0        0    49704 2024-04-24 04:15:28.819050 pypipr-1.0.89/readme.md
--rw-r--r--   0        0        0    50390 1970-01-01 00:00:00.000000 pypipr-1.0.89/PKG-INFO
+-rw-r--r--   0        0        0       18 2023-06-18 04:21:11.715384 pypipr-1.0.9/README.md
+-rw-r--r--   0        0        0        0 2023-06-17 13:04:18.403397 pypipr-1.0.9/pypipr/__init__.py
+-rw-r--r--   0        0        0     4037 2023-06-18 07:01:19.167393 pypipr-1.0.9/pypipr/console.py
+-rw-r--r--   0        0        0      854 2023-06-18 07:15:20.971392 pypipr-1.0.9/pypipr/engineering.py
+-rw-r--r--   0        0        0     1699 2023-06-18 12:56:11.511688 pypipr-1.0.9/pypipr/flow.py
+-rw-r--r--   0        0        0     9143 2023-06-18 07:12:55.259392 pypipr-1.0.9/pypipr/ifunctions.py
+-rw-r--r--   0        0        0      436 2023-06-18 04:18:24.039384 pypipr-1.0.9/pypipr/lib.py
+-rw-r--r--   0        0        0      665 2023-06-18 02:32:08.963389 pypipr-1.0.9/pypipr/libstd.py
+-rw-r--r--   0        0        0      348 2023-06-18 02:32:28.879389 pypipr-1.0.9/pypipr/libvendor.py
+-rw-r--r--   0        0        0    42809 2023-06-18 03:39:21.579386 pypipr-1.0.9/pypipr/pypipr copy.py
+-rw-r--r--   0        0        0      332 2023-06-18 06:35:45.735394 pypipr-1.0.9/pypipr/pypipr.py
+-rw-r--r--   0        0        0    25749 2023-06-18 07:13:14.523392 pypipr-1.0.9/pypipr/uncategorize.py
+-rw-r--r--   0        0        0      485 2023-06-18 13:04:16.667688 pypipr-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 pypipr-1.0.9/PKG-INFO
```

### Comparing `pypipr-1.0.89/pypipr/iengineering/calculate.py` & `pypipr-1.0.9/pypipr/engineering.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,37 @@
-from .PintUregQuantity import PintUregQuantity
-
-
-def calculate(teks):
-    """
-    Mengembalikan hasil dari perhitungan teks menggunakan modul pint.
-    Mendukung perhitungan matematika dasar dengan satuan.
-
-    Return value:
-    - Berupa class Quantity dari modul pint
-
-    Format:
-    - f"{result:~P}"            -> pretty
-    - f"{result:~H}"            -> html
-    - result.to_base_units()    -> SI
-    - result.to_compact()       -> human readable
-
-    ```python
-    fx = "3 meter * 10 cm * 3 km"
-    res = calculate(fx)
-    print(res)
-    print(res.to_base_units())
-    print(res.to_compact())
-    print(f"{res:~P}")
-    print(f"{res:~H}")
-    ```
-    """
-    return PintUregQuantity(teks)
-
-
-if __name__ == "__main__":
-    from ..ifunctions.iargv import iargv
-
-    if i := iargv(1):
-        print(i)
+'''
+Modul untuk analisa perhitungan 
+'''
+
+
+from .lib import *
+
+
+def calculate(teks):
+    """
+    Mengembalikan hasil dari perhitungan teks menggunakan modul pint.
+    Mendukung perhitungan matematika dasar dengan satuan.
+
+    Return value:
+    - Berupa class Quantity dari modul pint
+
+    Format:
+    - f"{result:~P}"            -> pretty
+    - f"{result:~H}"            -> html
+    - result.to_base_units()    -> SI
+    - result.to_compact()       -> human readable
+
+    ```python
+    fx = "3 meter * 10 cm * 3 km"
+    res = calculate(fx)
+    print(res)
+    print(res.to_base_units())
+    print(res.to_compact())
+    print(f"{res:~P}")
+    print(f"{res:~H}")
+    ```
+    """
+    return PintUregQuantity(teks)
+
+
+if __name__ == "__main__":
+    print_colorize("Anda menjalankan module pypipr", color=colorama.Fore.RED)
```

