# Comparing `tmp/extools-0.13.43.tar.gz` & `tmp/extools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extools-0.13.43.tar", last modified: Wed Nov 22 00:49:19 2023, max compression
+gzip compressed data, was "dist/extools-0.3.0.tar", last modified: Mon Dec 16 18:06:07 2019, max compression
```

## Comparing `extools-0.13.43.tar` & `extools-0.3.0.tar`

### file list

```diff
@@ -1,135 +1,31 @@
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:19.075922 extools-0.13.43/
--rw-r--r--   0 sysadmin   (501) staff       (20)    35149 2019-09-15 02:40:36.000000 extools-0.13.43/LICENSE.txt
--rw-r--r--   0 sysadmin   (501) staff       (20)      157 2020-04-15 15:15:30.000000 extools-0.13.43/MANIFEST.in
--rw-r--r--   0 sysadmin   (501) staff       (20)     3379 2023-11-22 00:49:19.072450 extools-0.13.43/PKG-INFO
--rw-r--r--   0 sysadmin   (501) staff       (20)     2216 2020-02-12 02:51:45.000000 extools-0.13.43/README.rst
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:18.954002 extools-0.13.43/docs/
--rw-r--r--   0 sysadmin   (501) staff       (20)      586 2019-12-13 19:53:17.000000 extools-0.13.43/docs/Makefile
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:18.945492 extools-0.13.43/docs/_build/
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:18.945569 extools-0.13.43/docs/_build/html/
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:18.960451 extools-0.13.43/docs/_build/html/_static/
--rw-r--r--   0 sysadmin   (501) staff       (20)      756 2019-09-16 18:44:43.000000 extools-0.13.43/docs/_build/html/_static/comment-bright.png
--rw-r--r--   0 sysadmin   (501) staff       (20)      829 2019-09-16 18:44:43.000000 extools-0.13.43/docs/_build/html/_static/comment-close.png
--rw-r--r--   0 sysadmin   (501) staff       (20)      641 2019-09-16 18:44:43.000000 extools-0.13.43/docs/_build/html/_static/comment.png
--rw-r--r--   0 sysadmin   (501) staff       (20)      222 2019-09-16 18:44:43.000000 extools-0.13.43/docs/_build/html/_static/down-pressed.png
--rw-r--r--   0 sysadmin   (501) staff       (20)      202 2019-09-16 18:44:43.000000 extools-0.13.43/docs/_build/html/_static/down.png
--rw-r--r--   0 sysadmin   (501) staff       (20)      286 2019-09-16 18:44:43.000000 extools-0.13.43/docs/_build/html/_static/file.png
--rw-r--r--   0 sysadmin   (501) staff       (20)       90 2019-09-16 18:44:43.000000 extools-0.13.43/docs/_build/html/_static/minus.png
--rw-r--r--   0 sysadmin   (501) staff       (20)       90 2019-09-16 18:44:43.000000 extools-0.13.43/docs/_build/html/_static/plus.png
--rw-r--r--   0 sysadmin   (501) staff       (20)      214 2019-09-16 18:44:43.000000 extools-0.13.43/docs/_build/html/_static/up-pressed.png
--rw-r--r--   0 sysadmin   (501) staff       (20)      203 2019-09-16 18:44:43.000000 extools-0.13.43/docs/_build/html/_static/up.png
--rw-r--r--   0 sysadmin   (501) staff       (20)     5432 2021-08-03 15:13:54.000000 extools-0.13.43/docs/conf.py
--rw-r--r--   0 sysadmin   (501) staff       (20)     6262 2021-11-09 03:43:57.000000 extools-0.13.43/docs/index.rst
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:18.962754 extools-0.13.43/docs/src/
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:18.963460 extools-0.13.43/docs/src/env/
--rw-r--r--   0 sysadmin   (501) staff       (20)      683 2021-08-03 15:13:54.000000 extools-0.13.43/docs/src/env/exenv.rst
--rw-r--r--   0 sysadmin   (501) staff       (20)       91 2021-08-03 15:13:54.000000 extools-0.13.43/docs/src/error_stack.rst
--rw-r--r--   0 sysadmin   (501) staff       (20)      100 2021-01-15 19:53:33.000000 extools-0.13.43/docs/src/errors.rst
--rw-r--r--   0 sysadmin   (501) staff       (20)      141 2021-08-03 15:13:54.000000 extools-0.13.43/docs/src/extools.rst
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:18.964153 extools-0.13.43/docs/src/message/
--rw-r--r--   0 sysadmin   (501) staff       (20)      122 2020-02-26 21:30:39.000000 extools-0.13.43/docs/src/message/exmessages.rst
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:18.965567 extools-0.13.43/docs/src/notes/
--rw-r--r--   0 sysadmin   (501) staff       (20)      770 2021-08-03 15:13:54.000000 extools-0.13.43/docs/src/notes/custom_table_fields.rst
--rw-r--r--   0 sysadmin   (501) staff       (20)      242 2021-08-03 15:13:54.000000 extools-0.13.43/docs/src/notes/notes.rst
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:18.966964 extools-0.13.43/docs/src/report/
--rw-r--r--   0 sysadmin   (501) staff       (20)      122 2021-08-12 23:15:14.000000 extools-0.13.43/docs/src/report/exreport.rst
--rw-r--r--   0 sysadmin   (501) staff       (20)      146 2021-11-26 15:11:10.000000 extools-0.13.43/docs/src/report/printers.rst
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:18.967692 extools-0.13.43/docs/src/test/
--rw-r--r--   0 sysadmin   (501) staff       (20)      115 2020-02-26 21:30:41.000000 extools-0.13.43/docs/src/test/extest.rst
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:18.969212 extools-0.13.43/docs/src/tests/
--rw-r--r--   0 sysadmin   (501) staff       (20)      192 2019-12-23 20:22:36.000000 extools-0.13.43/docs/src/tests/extools.rst
--rw-r--r--   0 sysadmin   (501) staff       (20)      114 2019-12-23 20:31:39.000000 extools-0.13.43/docs/src/tests/exview.rst
--rw-r--r--   0 sysadmin   (501) staff       (20)      650 2020-02-26 21:30:47.000000 extools-0.13.43/docs/src/tests.rst
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:18.973073 extools-0.13.43/docs/src/ui/
--rw-r--r--   0 sysadmin   (501) staff       (20)      124 2019-12-23 20:31:39.000000 extools-0.13.43/docs/src/ui/bare.rst
--rw-r--r--   0 sysadmin   (501) staff       (20)     1428 2021-08-03 15:13:54.000000 extools-0.13.43/docs/src/ui/column.rst
--rw-r--r--   0 sysadmin   (501) staff       (20)      148 2021-08-03 15:13:54.000000 extools-0.13.43/docs/src/ui/custom_table.rst
--rw-r--r--   0 sysadmin   (501) staff       (20)      184 2021-08-03 15:13:54.000000 extools-0.13.43/docs/src/ui/exui.rst
--rw-r--r--   0 sysadmin   (501) staff       (20)      152 2021-08-03 15:13:54.000000 extools-0.13.43/docs/src/ui/field_security.rst
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:18.979958 extools-0.13.43/docs/src/view/
--rw-r--r--   0 sysadmin   (501) staff       (20)    10544 2020-02-27 03:21:07.000000 extools-0.13.43/docs/src/view/composition.rst
--rw-r--r--   0 sysadmin   (501) staff       (20)      116 2019-12-23 20:31:39.000000 extools-0.13.43/docs/src/view/errors.rst
--rw-r--r--   0 sysadmin   (501) staff       (20)      137 2021-02-22 16:19:17.000000 extools-0.13.43/docs/src/view/exsql.rst
--rw-r--r--   0 sysadmin   (501) staff       (20)     8894 2021-11-26 15:11:10.000000 extools-0.13.43/docs/src/view/exview.rst
--rw-r--r--   0 sysadmin   (501) staff       (20)     3370 2019-12-23 20:31:39.000000 extools-0.13.43/docs/src/view/optfields.rst
--rw-r--r--   0 sysadmin   (501) staff       (20)     4197 2021-11-26 15:11:10.000000 extools-0.13.43/docs/src/view/query.rst
--rw-r--r--   0 sysadmin   (501) staff       (20)      687 2021-08-03 15:13:54.000000 extools-0.13.43/docs/src/view/utils.rst
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:18.983481 extools-0.13.43/extools/
--rw-r--r--   0 sysadmin   (501) staff       (20)     1980 2019-12-15 04:08:08.000000 extools-0.13.43/extools/__init__.py
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:18.986783 extools-0.13.43/extools/auth/
--rw-r--r--   0 sysadmin   (501) staff       (20)     1404 2021-11-26 15:11:10.000000 extools-0.13.43/extools/auth/__init__.py
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:18.987576 extools-0.13.43/extools/eft/
--rw-r--r--   0 sysadmin   (501) staff       (20)     2264 2021-08-03 15:13:54.000000 extools-0.13.43/extools/eft/__init__.py
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:18.990465 extools-0.13.43/extools/env/
--rw-r--r--   0 sysadmin   (501) staff       (20)      421 2021-08-03 15:13:54.000000 extools-0.13.43/extools/env/__init__.py
--rw-r--r--   0 sysadmin   (501) staff       (20)     2086 2021-08-03 15:13:54.000000 extools-0.13.43/extools/env/stream_conductor.py
--rw-r--r--   0 sysadmin   (501) staff       (20)     1145 2023-02-24 00:54:58.000000 extools-0.13.43/extools/env/win32.py
--rw-r--r--   0 sysadmin   (501) staff       (20)      474 2021-08-03 15:13:54.000000 extools-0.13.43/extools/error_stack.py
--rw-r--r--   0 sysadmin   (501) staff       (20)      296 2019-12-14 19:02:49.000000 extools-0.13.43/extools/errors.py
--rw-r--r--   0 sysadmin   (501) staff       (20)      616 2020-04-05 20:23:21.000000 extools-0.13.43/extools/expi.json
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:18.993324 extools-0.13.43/extools/message/
--rw-r--r--   0 sysadmin   (501) staff       (20)     8641 2022-06-23 02:00:29.000000 extools-0.13.43/extools/message/__init__.py
--rw-r--r--   0 sysadmin   (501) staff       (20)     6771 2021-11-26 15:11:33.000000 extools-0.13.43/extools/message/email.py
--rw-r--r--   0 sysadmin   (501) staff       (20)     2621 2021-11-26 15:11:10.000000 extools-0.13.43/extools/message/jinja2.py
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:18.994143 extools-0.13.43/extools/package/
--rw-r--r--   0 sysadmin   (501) staff       (20)      601 2021-08-03 15:13:54.000000 extools-0.13.43/extools/package/__init__.py
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:18.996146 extools-0.13.43/extools/report/
--rw-r--r--   0 sysadmin   (501) staff       (20)     7047 2023-01-15 20:13:42.000000 extools-0.13.43/extools/report/__init__.py
--rwxr-xr-x   0 sysadmin   (501) staff       (20)    14012 2023-11-22 00:47:57.000000 extools-0.13.43/extools/report/printers.py
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:18.997084 extools-0.13.43/extools/test/
--rw-r--r--   0 sysadmin   (501) staff       (20)     8286 2019-12-23 20:31:39.000000 extools-0.13.43/extools/test/__init__.py
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:18.998100 extools-0.13.43/extools/test/vi/
--rw-r--r--   0 sysadmin   (501) staff       (20)     2144 2021-11-26 15:11:10.000000 extools-0.13.43/extools/test/vi/extools.testrunner.vi
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:18.999966 extools-0.13.43/extools/tests/
--rw-r--r--   0 sysadmin   (501) staff       (20)        0 2020-04-05 15:24:43.000000 extools-0.13.43/extools/tests/__init__.py
--rw-r--r--   0 sysadmin   (501) staff       (20)     1751 2019-12-23 20:31:39.000000 extools-0.13.43/extools/tests/extest_extools.py
--rw-r--r--   0 sysadmin   (501) staff       (20)      321 2020-03-31 16:13:58.000000 extools-0.13.43/extools/tests/test_extools.py
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:19.010856 extools-0.13.43/extools/ui/
--rw-r--r--   0 sysadmin   (501) staff       (20)     4371 2021-08-03 15:13:54.000000 extools-0.13.43/extools/ui/__init__.py
--rw-r--r--   0 sysadmin   (501) staff       (20)      986 2020-04-21 17:26:56.000000 extools-0.13.43/extools/ui/bare.py
--rw-r--r--   0 sysadmin   (501) staff       (20)     2807 2021-11-26 15:11:10.000000 extools-0.13.43/extools/ui/callback_column.py
--rw-r--r--   0 sysadmin   (501) staff       (20)     2181 2021-08-16 22:51:37.000000 extools-0.13.43/extools/ui/controls.py
--rw-r--r--   0 sysadmin   (501) staff       (20)    15763 2021-08-03 15:13:54.000000 extools-0.13.43/extools/ui/custom_table.py
--rw-r--r--   0 sysadmin   (501) staff       (20)     2214 2021-08-03 15:13:54.000000 extools-0.13.43/extools/ui/datasource_column.py
--rw-r--r--   0 sysadmin   (501) staff       (20)     4320 2021-08-03 15:13:54.000000 extools-0.13.43/extools/ui/field_security.py
--rw-r--r--   0 sysadmin   (501) staff       (20)     5245 2021-08-03 15:13:54.000000 extools-0.13.43/extools/ui/optfield_column.py
--rw-r--r--   0 sysadmin   (501) staff       (20)     6295 2021-08-03 15:13:54.000000 extools-0.13.43/extools/ui/optfield_multicolumn.py
--rwxr-xr-x   0 sysadmin   (501) staff       (20)     2242 2022-09-21 03:51:33.000000 extools-0.13.43/extools/ui/prompt.py
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:19.013276 extools-0.13.43/extools/vi/
--rw-r--r--   0 sysadmin   (501) staff       (20)     3965 2021-08-03 15:13:54.000000 extools-0.13.43/extools/vi/__init__.py
--rw-r--r--   0 sysadmin   (501) staff       (20)     1687 2021-08-03 15:13:54.000000 extools-0.13.43/extools/vi/screen_script_manager.py
--rw-r--r--   0 sysadmin   (501) staff       (20)      958 2021-08-03 15:13:54.000000 extools-0.13.43/extools/vi/sysaccess.py
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:19.026494 extools-0.13.43/extools/view/
--rw-r--r--   0 sysadmin   (501) staff       (20)    44257 2022-04-01 01:07:55.000000 extools-0.13.43/extools/view/__init__.py
--rw-r--r--   0 sysadmin   (501) staff       (20)     1648 2021-08-03 15:13:54.000000 extools-0.13.43/extools/view/criteria.py
--rw-r--r--   0 sysadmin   (501) staff       (20)     6429 2021-08-03 15:13:54.000000 extools-0.13.43/extools/view/errors.py
--rw-r--r--   0 sysadmin   (501) staff       (20)     8213 2021-11-26 15:11:10.000000 extools-0.13.43/extools/view/exsql.py
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:19.029906 extools-0.13.43/extools/view/importer/
--rw-r--r--   0 sysadmin   (501) staff       (20)     2052 2021-08-03 15:13:54.000000 extools-0.13.43/extools/view/importer/__init__.py
--rw-r--r--   0 sysadmin   (501) staff       (20)    20131 2021-08-03 15:13:54.000000 extools-0.13.43/extools/view/importer/excel_order_importer.py
--rwxr-xr-x   0 sysadmin   (501) staff       (20)   151033 2021-11-26 15:11:10.000000 extools-0.13.43/extools/view/map.py
--rw-r--r--   0 sysadmin   (501) staff       (20)    12751 2023-02-01 01:36:19.000000 extools-0.13.43/extools/view/query.py
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:19.067673 extools-0.13.43/extools/view/utils/
--rw-r--r--   0 sysadmin   (501) staff       (20)        0 2021-08-03 15:13:54.000000 extools-0.13.43/extools/view/utils/__init__.py
--rw-r--r--   0 sysadmin   (501) staff       (20)      491 2021-08-03 15:13:54.000000 extools-0.13.43/extools/view/utils/customer.py
--rw-r--r--   0 sysadmin   (501) staff       (20)     1654 2021-08-03 15:13:54.000000 extools-0.13.43/extools/view/utils/gl.py
--rw-r--r--   0 sysadmin   (501) staff       (20)      284 2021-08-03 15:13:54.000000 extools-0.13.43/extools/view/utils/glaccount.py
--rw-r--r--   0 sysadmin   (501) staff       (20)     3391 2021-08-03 15:13:54.000000 extools-0.13.43/extools/view/utils/iet.py
--rw-r--r--   0 sysadmin   (501) staff       (20)     1910 2021-11-26 15:11:10.000000 extools-0.13.43/extools/view/utils/item.py
--rw-r--r--   0 sysadmin   (501) staff       (20)     1281 2021-08-03 15:13:54.000000 extools-0.13.43/extools/view/utils/order.py
--rw-r--r--   0 sysadmin   (501) staff       (20)      639 2021-08-03 15:13:54.000000 extools-0.13.43/extools/view/utils/shipment.py
--rw-r--r--   0 sysadmin   (501) staff       (20)      252 2021-08-03 15:13:54.000000 extools-0.13.43/extools/view/utils/units.py
--rw-r--r--   0 sysadmin   (501) staff       (20)     3535 2021-11-26 15:11:10.000000 extools-0.13.43/extools/view/utils/users.py
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:19.070605 extools-0.13.43/extools/workflow/
--rw-r--r--   0 sysadmin   (501) staff       (20)     3091 2021-08-03 15:13:54.000000 extools-0.13.43/extools/workflow/__init__.py
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:19.071719 extools-0.13.43/extools/workflow/vi/
--rwxr-xr-x   0 sysadmin   (501) staff       (20)     1535 2021-11-26 15:11:10.000000 extools-0.13.43/extools/workflow/vi/Poplar.Workflow.StringMatching.vi
--rw-r--r--   0 sysadmin   (501) staff       (20)     1057 2021-11-26 15:11:10.000000 extools-0.13.43/extools/workflow/vi/poplar.workflow.vi
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-11-22 00:49:18.986298 extools-0.13.43/extools.egg-info/
--rw-r--r--   0 sysadmin   (501) staff       (20)     3379 2023-11-22 00:49:18.000000 extools-0.13.43/extools.egg-info/PKG-INFO
--rw-r--r--   0 sysadmin   (501) staff       (20)     2754 2023-11-22 00:49:18.000000 extools-0.13.43/extools.egg-info/SOURCES.txt
--rw-r--r--   0 sysadmin   (501) staff       (20)        1 2023-11-22 00:49:18.000000 extools-0.13.43/extools.egg-info/dependency_links.txt
--rw-r--r--   0 sysadmin   (501) staff       (20)       15 2023-11-22 00:49:18.000000 extools-0.13.43/extools.egg-info/requires.txt
--rw-r--r--   0 sysadmin   (501) staff       (20)        8 2023-11-22 00:49:18.000000 extools-0.13.43/extools.egg-info/top_level.txt
--rw-r--r--   0 sysadmin   (501) staff       (20)       38 2023-11-22 00:49:19.076501 extools-0.13.43/setup.cfg
--rw-r--r--   0 sysadmin   (501) staff       (20)     1135 2022-06-23 01:58:47.000000 extools-0.13.43/setup.py
+drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2019-12-16 18:06:07.000000 extools-0.3.0/
+-rw-r--r--   0 sysadmin   (501) staff       (20)     3339 2019-12-16 18:06:07.000000 extools-0.3.0/PKG-INFO
+drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2019-12-16 18:06:07.000000 extools-0.3.0/extools/
+drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2019-12-16 18:06:07.000000 extools-0.3.0/extools/vi/
+-rw-r--r--   0 sysadmin   (501) staff       (20)     2156 2019-12-16 03:42:22.000000 extools-0.3.0/extools/vi/extools.testrunner.vi
+drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2019-12-16 18:06:07.000000 extools-0.3.0/extools/extest/
+-rw-r--r--   0 sysadmin   (501) staff       (20)     7257 2019-12-16 03:42:22.000000 extools-0.3.0/extools/extest/__init__.py
+drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2019-12-16 18:06:07.000000 extools-0.3.0/extools/tests/
+-rw-r--r--   0 sysadmin   (501) staff       (20)      321 2019-12-14 22:33:17.000000 extools-0.3.0/extools/tests/test_extools.py
+-rw-r--r--   0 sysadmin   (501) staff       (20)     1753 2019-12-16 03:42:22.000000 extools-0.3.0/extools/tests/extest_extools.py
+-rw-r--r--   0 sysadmin   (501) staff       (20)        0 2019-12-14 22:31:24.000000 extools-0.3.0/extools/tests/__init__.py
+-rw-r--r--   0 sysadmin   (501) staff       (20)     1980 2019-12-15 04:08:08.000000 extools-0.3.0/extools/__init__.py
+drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2019-12-16 18:06:07.000000 extools-0.3.0/extools/exmessages/
+-rw-r--r--   0 sysadmin   (501) staff       (20)     6481 2019-12-14 18:17:19.000000 extools-0.3.0/extools/exmessages/__init__.py
+-rw-r--r--   0 sysadmin   (501) staff       (20)      598 2019-12-16 18:04:41.000000 extools-0.3.0/extools/expi.json
+drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2019-12-16 18:06:07.000000 extools-0.3.0/extools/exview/
+-rw-r--r--   0 sysadmin   (501) staff       (20)    30781 2019-12-16 17:54:29.000000 extools-0.3.0/extools/exview/__init__.py
+-rw-r--r--   0 sysadmin   (501) staff       (20)     2872 2019-12-14 18:24:53.000000 extools-0.3.0/extools/exview/exsql.py
+-rw-r--r--   0 sysadmin   (501) staff       (20)     4390 2019-12-14 19:27:31.000000 extools-0.3.0/extools/exview/errors.py
+-rw-r--r--   0 sysadmin   (501) staff       (20)      296 2019-12-14 19:02:49.000000 extools-0.3.0/extools/errors.py
+drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2019-12-16 18:06:07.000000 extools-0.3.0/extools/exui/
+-rw-r--r--   0 sysadmin   (501) staff       (20)     2026 2019-12-15 02:57:52.000000 extools-0.3.0/extools/exui/__init__.py
+-rw-r--r--   0 sysadmin   (501) staff       (20)      990 2019-12-15 04:08:08.000000 extools-0.3.0/extools/exui/bare.py
+-rw-r--r--   0 sysadmin   (501) staff       (20)     1156 2019-12-16 18:06:03.000000 extools-0.3.0/setup.py
+drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2019-12-16 18:06:07.000000 extools-0.3.0/extools.egg-info/
+-rw-r--r--   0 sysadmin   (501) staff       (20)     3339 2019-12-16 18:06:06.000000 extools-0.3.0/extools.egg-info/PKG-INFO
+-rw-r--r--   0 sysadmin   (501) staff       (20)      500 2019-12-16 18:06:06.000000 extools-0.3.0/extools.egg-info/SOURCES.txt
+-rw-r--r--   0 sysadmin   (501) staff       (20)        8 2019-12-16 18:06:06.000000 extools-0.3.0/extools.egg-info/top_level.txt
+-rw-r--r--   0 sysadmin   (501) staff       (20)        1 2019-12-16 18:06:06.000000 extools-0.3.0/extools.egg-info/dependency_links.txt
+-rw-r--r--   0 sysadmin   (501) staff       (20)       59 2019-12-16 18:06:07.000000 extools-0.3.0/setup.cfg
+-rw-r--r--   0 sysadmin   (501) staff       (20)     2216 2019-12-04 17:19:35.000000 extools-0.3.0/README.rst
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `extools-0.13.43/PKG-INFO` & `extools-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: extools
-Version: 0.13.43
+Version: 0.3.0
 Summary: Tools for Orchid Extender
-Home-page: https://poplars.dev
-Author: Chris Binckly, 2665093 Ontario Inc.
+Home-page: https://2665093.ca
+Author: Chris Binckly, 2665092 Ontario Inc.
 Author-email: cbinckly@gmail.com
 License: UNKNOWN
 Description: ##################
         Tools for Extender
         ##################
         
         -------------------------------------------------
@@ -72,8 +72,7 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.4
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Description-Content-Type: text/x-rst
```

### Comparing `extools-0.13.43/README.rst` & `extools-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `extools-0.13.43/extools/__init__.py` & `extools-0.3.0/extools/__init__.py`

 * *Files identical despite different names*

### Comparing `extools-0.13.43/extools/message/__init__.py` & `extools-0.3.0/extools/exmessages/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,19 @@
 import traceback
 import logging
-from logging.handlers import RotatingFileHandler
-from pathlib import Path
 
 try:
-    from accpac import *
+    from accpac import (showMessageBox,
+                        program, rotoID,
+                        error, message, warning, )
 except ImportError as e:
     # This happens when the tools are imported outside of the Extender env.
     # We can pass to let the tool do its work (likely sphinx making docs).
     pass
 
-from extools.error_stack import consume_errors
-
-__exm_loggers = {}
-
-def logger_for_module(module_name, level=None, box=None, **kwargs):
-    global __exm_loggers
-    filestem = module_name.split(".")[0]
-
-    log_path = Path(getOrgPath(), "{}.log".format(filestem))
-    log_debug_path = Path(getOrgPath(), "{}.debug".format(filestem))
-
-    if not level:
-        level = ExMessages.INFO
-        if log_debug_path.exists():
-            level = ExMessages.DEBUG
-    
-    if filestem not in __exm_loggers:
-        __exm_loggers[filestem] = ExMessages(
-                module_name, level=level, log_path=str(log_path), 
-                box=box, **kwargs)
-    else:
-        return  ExMessages(module_name, level=level, box=box, 
-                    handler=__exm_loggers[filestem].handler, **kwargs)
-    return __exm_loggers[filestem]
-
 class ExMessages(object):
     """A logger like object for writing messages for the user.
 
     The ExtenderMessageWriter acts like a logger, allowing a developer
     to add messages that are only displayed to the user if the current
     level is greater than or equal to the message level being called.
 
@@ -53,17 +28,17 @@
     :param log_path: the path of a log file to write to.
     :type log_path: str
     :param programs: the list of programs for which to display
         messages.  For example, if programs were ["OE1100", ] then messages
         will only be displayed if the Order Entry program is currently
         running.
     :type programs: list
-    :param box: indicates whether to show a message box, add a message to the
-        Sage message stack, or suppress UI messages. Defaults to True.
-    :type box: True (showMessageBox), False (message stack), None (suppress)
+    :param box: indicates whether to show a message box or
+        add a message to the Sage message stack. Defaults to True.
+    :type box: list
     :param disabled: disable all messages and logging.
         Defaults to False.
     :type disabled: bool
     """
 
     """Supported Levels"""
     PANIC       = 0
@@ -92,80 +67,62 @@
             ERROR: ("Error", "error", ),
             WARNING: ("Warning", "warning", ),
             INFO: ("Info", "info", ),
             DEBUG: ("Debug", "debug", ),
             RAW: ("Raw", "debug", ),
             }
 
-    YES_NO_DIALOG = 0x04
-    YES_NO_DIALOG_YES = 6
-    YES_NO_DIALOG_NO  = 7
-
     def __init__(self, name, level=None, log_path=None, programs=[], box=True,
-                 disabled=False, key="", handler=None):
+                 disabled=False, ):
         """Get a new ExMessages instance."""
         if not level:
             level = self.INFO
         self.level = level
         self.level_info = self._LEVEL_INFO[level]
         self.level_name = self.level_info[0]
 
         self.name = name
         self.disabled = disabled
         self.programs = programs
         self.box = box
-        self.key = key
-
-        self.handler = handler
 
         self.log = None
         self.log_path = log_path
-        self.log_level = getattr(logging, self.level_info[1].upper())
-        if self.log_path or self.handler:
+        self.log_level = getattr(logging, self.level_info[1])
+        if self.log_path:
             self._setup_log()
 
     def _setup_log(self):
-        self.log = logging.getLogger(self.name)
-        if not self.handler:
-            self.handler = RotatingFileHandler(
-                    filename=str(self.log_path),
-                    backupCount=1,
-                    maxBytes=10*1024*1024)
-            self.handler.setFormatter(logging.Formatter(
-                    fmt='%(asctime)s %(name)-12s %(levelname)-8s %(message)s',
-                    datefmt='%Y-%m-%dT%H:%M:%S',))
-
-        self.log.addHandler(self.handler)
-        self.log.setLevel(self.log_level)
+        self.log = logging.getLogger(name)
+        self.log.setLevel(self.log_level.DEBUG)
+        self.log_formatter = logging.Formatter(
+                '%(asctime)s - %(name)s %(message)s')
+        self.log_handler = logging.FileHandler(self.log_path)
+        self.log_handler.setFormatter(self.log_formatter)
+        self.log.addHandler(self.log_handler)
 
     def _write(self, level, msg):
         if self.disabled or (self.programs and program not in self.programs):
             return None
 
-        name = self.name
-        if self.key:
-            name =  "{}.{}".format(name, self.key)
-        msg_w_name = "{}\n\n{}".format(name, msg)
+        msg_w_name = "{}\n\n{}".format(self.name, msg)
         if level <= self.level:
-            if level == self.DEBUG:
-                msg_w_name  = "DEBUG {}\n\n{}".format(rotoID, msg_w_name)
-
             if self.box:
                 showMessageBox(msg_w_name)
-            elif self.box is not None:
+            else:
                 if level <= self.ERROR:
                     error(msg_w_name)
                 elif level <= self.WARNING:
                     warning(msg_w_name)
                 else:
                     message(msg_w_name)
 
         if self.log:
-            log_func = getattr(self.log, self._LEVEL_INFO[level][1])
-            log_func("{} {}".format(self.key, msg))
+            log_func = getattr(self.log, self._LEVEL_INFO[self.level][1])
+            log_func(msg)
 
         return msg
 
     def panic(self, msg, exc_info=None):
         """Display and log a panic message.
 
         :param msg: message to write.
@@ -228,14 +185,15 @@
 
         :param msg: message to write.
         :type msg: str
         :param exc_info: include last exception backtrace?
         :type exc_info: bool
         :rtype: None
         """
+        msg = "DEBUG {}\n---------\n{}".format(rotoID, msg)
         if exc_info:
             msg = "\n".join([msg, traceback.format_exc(), ])
         self._write(self.DEBUG, msg)
 
     def raw(self, msg, exc_info=False):
         """Display and log raw output.
 
@@ -245,30 +203,7 @@
         :type exc_info: bool
         :rtype: None
         """
         msg = "RAW {}\n---------\n{}".format(rotoID, msg)
         if exc_info:
             msg = "\n".join([msg, traceback.format_exc(), ])
         self._write(self.RAW, msg)
-
-    @classmethod
-    def prompt(self, title, message):
-        """Display a Yes/No dialog prompt.
-
-        :param title: The message box title.
-        :type title: str
-        :param message: The prompt to display.
-        :type message: str
-        :returns: True if User selects Yes, else No
-        :rtype: bool
-        """
-        answer = ask(message, title, self.YES_NO_DIALOG)
-        if answer == self.YES_NO_DIALOG_YES:
-            return True
-        return False
-
-    def debug_error_stack(self):
-        """Write the contents of the error stack to log as debug messages
-        and clear the stack."""
-        for priority, message in consume_errors():
-            self.debug("Error Stack {}: {}".format(priority, message))
-        return True
```

### Comparing `extools-0.13.43/extools/test/__init__.py` & `extools-0.3.0/extools/extest/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from datetime import datetime
 from contextlib import contextmanager
 from extools.errors import ExToolsError
-from extools.message import ExMessages
+from extools.exmessages import ExMessages
 
 class ExTestError(ExToolsError):
     """Raised by failed test cases."""
     pass
 
 def asserts(method):
     def wrapper(self, *args, **kw):
@@ -34,35 +33,35 @@
     Run all the tests in a project using the included ExTestRunner module.
 
     Let's say you want to test your set order decription custom function,
     which sets the order decription to the customer number.
 
     .. code-block:: python
 
-        from extools.view import exview
+        from extools.exview import exview
 
         def set_description_to_customer_number(ordnumber):
             '''Set the order description to the customer number.
 
             :param ordnumber: the order number to update.
             :type ordnumber: str
             :rtype: None
             :raises: ExViewError
             '''
             with exview("OE0500", seek_to={"ORDNUMBER": ordnumber}) as exv:
                 exv.update(DESC=exv.get("CUSTOMER"))
 
-    Using the :py:meth:`extools.view.exview` context manager makes opening,
+    Using the :py:meth:`extools.exview.exview` context manager makes opening,
     closing, and seeking the view easy.  To test it, we will need a record in
     the SAMINC database that we can change the Description on.  The first,
     ORD000000000001, seems to fit the bill.
 
     .. code-block:: python
 
-        from extools.test import ExTestCase
+        from extools.extest import ExTestCase
         from mymodule import set_description_to_customer_number
 
         class MyTest(ExTestCase):
 
             # Make the order to work on a constant
             ORDER_NUMBER = "ORD000000000001"
             ORDER_VIEW = "OE0500"
@@ -86,37 +85,37 @@
                     self.assertTrue(exv.get("CUSTOMER") == exv.get("DESC"))
 
         def main():
             # To run your tests, instantiate the class and run it!
             mt = MyTest()
             mt.run()
         """
-
+    
     # Try to set rotating indexes to avoid stepping on yourself.
     INDEX_MAX = 99
     _index = 9
-
-
+    
+    
     def __init__(self, log_level=ExMessages.INFO):
         self.name = self.__class__.__name__
         self.exm = ExMessages(self.name, log_level)
         self.index = self.generate_index()
 
-        # { 'test_name': { 'result': True/False, 'assertions': 0 }, ... }
+        # { 'test_name': { 'result': True/False, 'assertions': 0 }, ... } 
         self.results = {}
         self._current_test = None
-
+    
     def generate_index(self):
         """Get the next available view index and increment the counter."""
         # Avoid the first 10.
         self._index = (self._index + 1) % self.INDEX_MAX
         if self._index < 10:
             self._index = 10
         return self._index
-
+    
     @asserts
     def assert_true(self, obj):
         """Assert that something is truthy."""
         if not obj:
             raise ExTestError("{} is not true".format(obj))
 
     @asserts
@@ -148,73 +147,50 @@
         except exception:
             return True
         except Exception as e:
             raise ExTestError("{} not raised".format(exception), trigger_exc=e)
         else:
             raise ExTestError("{} not raised".format(exception))
 
-    def run(self, with_transaction=True):
+    def run(self):
         """Run all the tests in the class and provide a report."""
         passed = []
         failed = []
         try:
             self.setup_class()
             for meth in dir(self):
                 if meth.startswith('test_'):
                     self.exm.debug("Running {}".format(meth))
                     self._current_test = meth
                     self.results[meth] = { 'result': False, 'assertions': 0 }
                     try:
                         self.setup()
-                        # with self._db_transaction():
                         r = getattr(self, meth)()
                         self.results[meth]['result'] = True
-                        self.results[meth]['return'] = r
                         passed.append(meth)
                     except Exception as e:
                         failed.append(meth)
                         self.exm.error("{} failed: {}".format(meth, e),
                                         exc_info=True)
+
+
                     finally:
                         self.teardown()
         finally:
             self.teardown_class()
         self.exm.info("Failing tests ({}):\n{}\nPassing Tests({}):\n{}".format(
             len(failed), ", ".join(failed), len(passed), ", ".join(passed)))
-
+        
         s = ""
         for (test, data) in self.results.items():
-            s += "{} ({} assertions): {}\n".format(test,
-                                                   data['assertions'],
+            s += "{} ({} assertions): {}\n".format(test, 
+                                                   data['assertions'], 
                                                    data["result"], )
         self.exm.info(s)
 
-    def _db_transaction(self, transaction_name=None):
-        """This won't work because the transaction happens on a per-connection basis.
-
-        And I can't get to the connection pool, deep in the bowels of sage."""
-        if not transaction_name:
-            transaction_name = datetime.now().strftime(
-                    "%Y%m%d%H%M%S-{}".format(__name__))
-        try:
-            with exsql() as exs:
-                exs.query("BEGIN TRANSACTION {}".format(transaction_name))
-                yield exs
-        finally:
-            try:
-                exs.query("ROLLBACK TRANSACTION {}".format(transaction_name))
-            except:
-                self.exm.error("Failed to rollback {}. Database state may "
-                               "be inconsistent.".format(transaction_name))
-
-            try:
-                exs.close()
-            except:
-                pass # Do something useful
-
     def setup(self):
         """Steps that are run before every test."""
         pass
 
     def teardown(self):
         """Steps that are run after every test."""
         pass
```

### Comparing `extools-0.13.43/extools/test/vi/extools.testrunner.vi` & `extools-0.3.0/extools/vi/extools.testrunner.vi`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [MODULE]
 id=EXTESTER
 name=EXTESTER - extools Test Runner
 desc=Test executor for the extools package.
 company=2665093 Ontario Inc.
-version=0.13.43
+version=0.1
 website=https://2665093.ca
 
 [SCRIPT]
 FILENAME=ExToolsTester.2665093.py
 >>> SCRIPT >>>
 ###############################################################################
 #  ExToolsTester is a test runner for the extools package.
@@ -22,24 +22,24 @@
 #
 #  This software has a non-exclusive license and cannot be sublicensed, reused,
 #  transferred or modified without written consent from 2665093 Ontario Inc.
 #
 ###############################################################################
 from accpac import *
 from extools import success
-from extools.view import ExView, ExViewError
-from extools.message import ExMessages
-from extools.ui.bare import bareui
+from extools.exview import ExView, ExViewError
+from extools.exmessages import ExMessages
+from extools.exui.bare import bareui
 
-exm = ExMessages("extoolstester", ExMessages.DEBUG)
+exm = ExMessages("extoolstester", ExMessages.INFO)
 FILENAME_CONTAINS = "extest"
 ENTRY_FUNCTION = "main"
 
 def main(*args, **kwargs):
-    with bareui():
+    with bareui(close=True):
         exm.info("Starting.")
 
         test_scripts = []
         try:
             exv = ExView("VI0015")
             while(exv.fetch()):
                 filename = exv.get("FILENAME")
```

### Comparing `extools-0.13.43/extools/tests/extest_extools.py` & `extools-0.3.0/extools/tests/extest_extools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import extools
-from extools.test import ExTestCase
+from extools.extest import ExTestCase
 
 try:
     from accpac import *
 except ImportError:
     pass
 
 ORDER_HEADER_VIEWID = "OE0520"
```

### Comparing `extools-0.13.43/extools/ui/bare.py` & `extools-0.3.0/extools/exui/bare.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 @contextmanager
 def bareui(close=True):
     """Get a BareUI instance temporarily.
 
     Useful for running scripts that pop up messages but don't need to
     leave the UI window lingering.
-
+    
     :param close: whether to automatically close the UI. Disable to capture
                   lingering errors.
     :type close: bool
 
     .. code-block:: python
 
         # myextenderscript.py
```

### Comparing `extools-0.13.43/extools/view/__init__.py` & `extools-0.3.0/extools/exview/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,150 +1,92 @@
 """
 ExView is a fully functional wrapper around the Extender View object
 that raises exceptions instead of providing non-zero returns on error
-for the methods defined in :py:data:`extools.view.ExView.WRAP`.
+for the methods defined in :py:data:`extools.exview.ExView.WRAP`.
 
 It supports all the methods of the ``Extender.View`` class, along with many
 extra helpers.
 
 On startup an ``ExView`` introspects the underlying Sage view to automatically
 determine:
 
 - The view's composition tree
 - The field names
 - The allowed indexes and their key fields
 
 Based on this information, the class automatically configures itself to:
 
-- Self-compose on request (see :py:meth:`extools.view.ExView.compose`)
+- Self-compose on request (see :py:meth:`extools.exview.ExView.compose`)
 - Validate orders and keys before errors are raised by Sage
 - Automatically add the correct helpers
     - For detail views, the ``.lines()``, ``.lines_from(start, end)``,
       ``.lines_where(key=value, key=value, ...)`` generators and ``newline()``
       helper.
     - For optional field views, or any view composed with an optional
       field view, enable the ``create_optfield``, ``update_optfield``,
       ``get_optfield``, ``update_or_create_optfield``, ``seek_to_optfield``,
       and ``delete_optfield`` helpers.
 
 """
-
-try:
-    from accpac import *
-except ImportError as e:
-    # This happens when the tools are imported outside of the Extender env.
-    # We can pass to let the tool do its work (likely sphinx making docs).
-    pass
-
 from contextlib import contextmanager
 
 from extools import success
-from extools.message import logger_for_module
+from extools.exmessages import ExMessages
 
-from extools.view.map import VIEW_INFO_MAP
-from extools.view.errors import (ExViewError, ExViewComposeError,
+from .errors import (ExViewError, ExViewComposeError,
                      ExViewOpenError, ExViewInvalidOrder,
-                     ExViewFieldDoesNotExist, ExViewRecordDoesNotExist,
-                     ExViewIndexError, )
+                     ExViewFieldDoesNotExist, ExViewIndexError, )
 
-from datetime import datetime
+try:
+    from accpac import View
+except ImportError as e:
+    # This happens when the tools are imported outside of the Extender env.
+    # We can pass to let the tool do its work (likely sphinx making docs).
+    pass
 
-EXVIEW_BLACKLIST = {"OE0999", }
+EXVIEW_BLACKLIST = [ "OE0999", ]
 """Views that can never be composed with any other."""
 
-FIELD_DESC_BLACKLIST = {'Reserved', '', None, }
-
-STRFTIME = "%d/%m/%Y"
-STRPTIME = "%Y%m%d"
-
-def notme(function):
-    def func_wrapper(self, *args, **kwargs):
-        if self._me:
-            raise ExViewError("{} cannot be used with _me".format(function))
-        return function(self, *args, **kwargs)
-    return func_wrapper
+exm = ExMessages("extools.exview", ExMessages.DEBUG)
 
 @contextmanager
-def exview(rotoid, index=-1, seek_to={}, fetch=True, compose=False):
+def exview(rotoid, index=-1, seek_to={}):
     """Context manager to cleanly open and use an ExView.
 
     :param rotoid: the RotoID of the Sage view.
     :type rotoid: str
     :param index: the index to open the view with.
     :type index: int
     :param seek_to: field value mapping to seek to after opening. When set
         to an empty dictionary, seek to the first line in the view. If set
         to ``None``, disable seek after opening.
     :type seek_to: dict|None
-    :param fetch: automatically fetch the first matched record?
-    :type fetch: bool
-    :param compose: automatically compose before seeking?
-    :type compose: bool
     :raises: ExViewError
     :rtype: None
 
     When called the context manager will yield an open view
     object. On exit of the block the view will be closed cleanly.
 
     .. code-block:: python
 
         with exview("EX0001") as view:
             try:
                 view.recordClear()
                 view.browse("")
                 view.fetch()
                 value = view.get("KEY")
-            except ExViewError as err:
+            except ExToolError as err:
                 showMessageBox("Failed to get KEY, {}.".format(err))
     """
-    exv = ExView(rotoid, index)
+    exv = ExView(rotoid, index, seek_to)
     try:
-        if compose:
-            exv.compose()
-        if seek_to:
-            exv.seek_to(**seek_to, fetch=fetch)
-        elif fetch:
-            exv.fetch()
         yield exv
     finally:
         exv.close()
 
-def exgen(rotoid, index=-1, seek_to={}):
-    """Generator for iterating over all the entries in a view.
-
-    :param rotoid: the RotoID of the Sage view.
-    :type rotoid: str
-    :param index: the index to open the view with.
-    :type index: int
-    :param seek_to: field value mapping to seek to after opening. When set
-        to an empty dictionary, seek to the first line in the view. If set
-        to ``None``, disable seek after opening.
-    :type seek_to: dict|None
-    :raises: ExViewError
-    :rtype: None
-
-    When called, the generator will seek the view to the requested records,
-    or the first record if ``seek_to`` is empty.  It will then yield all
-    matching rows and then cleanly close the view.
-
-    .. code-block:: python
-
-        for record in exgen("EX0001"):
-            try:
-                record.get("FIELD")
-            except ExViewError as err:
-                showMessageBox("Failed to get FIELD, {}.".format(err))
-    """
-    with exview(rotoid, index, seek_to, fetch=False) as exv:
-        try:
-            while exv.fetch():
-                yield exv
-        except ExViewRecordDoesNotExist:
-            pass
-
 class ExView():
     """An exception raising wrapper around the Extender View class.
 
     ExViews can be used to replace repetitive error checking and to
     take advantage of the try/except/else/finally construct in Python.
 
     :param rotoid: the RotoID of the Sage view.
@@ -187,28 +129,28 @@
     With this:
 
     .. code-block:: python
 
         try:
             view = ExView("EX0001")
             value = view.get("KEY")
-        except ExViewError as err:
+        except ExToolError as err:
             showMessageBox("Failed to get KEY, {}.".format(err))
             return 1
         finally:
             view.close()
 
     You can even include the traceback using the ExMessages:
 
     .. code-block:: python
 
         try:
             view = ExView("EX0001")
             value = view.get("KEY")
-        except ExViewError as err:
+        except ExToolError as err:
             # Use ExMessages to display an error level message box and
             # log to a file (if configured). The last exception traceback
             # will be included in both the box and log if ``exc_info=True``.
             exm.error("Failed to get KEY, {}.".format(err), exc_info=True)
             return 1
         finally:
             view.close()
@@ -217,17 +159,17 @@
     views automatically.  Fully composed views require more database
     operations every time the header is changed and do not perform as well as
     standalone views or SQL access.  However, in cases where performance isn't
     paramount you cannot beat the convenience.
 
     .. code-block:: python
 
-        from extools import success
-        from extools.view import ExView
-        from extools.message import ExMessages
+        from extools.extools import success
+        from extools.exview import ExView
+        from extools.exmessages import ExMessages
 
         exm = ExMessages("compose-test", ExMessages.DEBUG)
 
         try:
             exv = ExView("OE0520")
             exv.compose()
         except Exception as e:
@@ -246,230 +188,154 @@
             for line in exv.oe0500.lines():
                 exm.info("Read new line {}".format(line.get("ITEM")))
                 # perform many important actions...
         except Exception as e:
             exm.error("Failed to perform action: {}".format(e), exc_info=True)
     """
 
-    WRAP = [ 'fetchLock', 'readLock',
+    WRAP = [ 'fetchLock', 'read', 'readLock',
              'insert', 'delete', 'init',
              'post', 'process', 'verify', 'recordClear',
-             'dirty', 'unlock', 'cancel',
+             'exists', 'dirty', 'unlock', 'cancel',
              'recordGenerate', 'put', 'browse', ]
     """These View functions raise an ``ExViewError`` on non-zero return."""
 
-    DETAIL_VIEW_HINTS = {'LINENUM', 'DETAILNUM', 'CNTENTR', 'ENTRY', }
+    DETAIL_VIEW_HINTS = {'LINENUM', 'DETAILNUM', }
     """Views containing any one of these fields may be detail views."""
 
     OPTFIELD_VIEW_HINTS = {'OPTFIELD', }
     """Views containing any one of these fields may be optional field views."""
 
     __exview_cache = {}
     """The view cache is shared by all instances of a class. Views can only be
-    opened once per index, to avoid opening views twice on compose,
+    opened once per index, to avoid opening views twice on compose, 
     cache them here.
-
+    
     format: { index: { viewid: view } }
     """
 
-    ATTR_A          = 0x002
-    ATTR_EDITABLE   = 0x004
-    ATTR_KEY        = 0x008
-    ATTR_COMPUTED   = 0x010
-    ATTR_P          = 0x020
-    ATTR_R          = 0x030
-    ATTR_X          = 0x040
-
-    ATTRS = {
-            "A": ATTR_A,
-            "E": ATTR_EDITABLE,
-            "K": ATTR_KEY,
-            "C": ATTR_COMPUTED,
-            "P": ATTR_P,
-            "R": ATTR_R,
-            "X": ATTR_X,
-    }
-
-    def __init__(self, rotoid, index=-1, seek_to={}, native_types=False,
-                 fetch=True, _root=True, _me=None, _cviews=[]):
+    def __init__(self, rotoid, index=-1, seek_to={}, _root=True):
         """Introspect and setup the object based on the results."""
         self.rotoid = rotoid
         self.index = index
-        self._view = None
-
-        self.log = logger_for_module('extools.view', key="{}[{}]".format(
-                self.rotoid, self.index))
-        self.log.debug("opening view {} [{}]".format(rotoid, index))
-
-        self.protocol = "FLAT"
-        self.table = ""
-        self.view_desc = ""
-        if "." in self.rotoid:
-            self.table = self.rotoid.split(".")[-1]
-        else:
-            if not self.rotoid in VIEW_INFO_MAP:
-                self.log.warn("rotoid {} not in view info map")
-            else:
-                info = VIEW_INFO_MAP[self.rotoid]
-                self.protocol = info.get("protocol", "FLAT")
-                self.table = info.get("name", "")
-                self.view_desc = info.get("desc", "")
-
+        
         # Is this a root view or opened on compose?
         self._root = _root
 
-        # Is this a `me` view?
-        self._me = _me
+        # The underlying Extender ``View`` object.
+        self._view = None
 
         # list of view rotoids this view composes with
         self._views = []
 
         # pointers to the views this view composes with in the view_cache
         self._cviews = []
-
-        # convert formats (date/time) to native py formats?
-        self.native_types = native_types
+        
+        self.composed = False
 
         # The current view order index.
         self._order = 0
 
         # The human readable field names in the view.
         self.field_names = []
 
-        # Dictionary of field names to their objects.
-        self.fields = {}
-
         # The indexes supported by this view, a list of field name tuples.
         self.indexes = []
 
-        self.detail_view = None
-        self.optfield_view = None
-
         # Open the underlying View
-        if not self._me:
-            self._open()
-            self._get_composed_views()
-        else:
-            self._view = self._me
-            if _cviews:
-                self.compose_from(_cviews)
+        self._open()
 
         # Wrap the view to raise on error instead of returning non-zero
         self._setup_wrapper()
 
         ## Introspection stuff
 
         # Get the field names
         self._get_field_names()
 
         # the indexes
         self._get_indexes()
+        
+        # the composed views
+        self._get_composed_views()
 
+        self.detail_view = None
         # If this looks like a detail view, then add extra detail functions.
         self._check_and_setup_detail_view()
 
         # If this looks like an optional field view, then add extra functions.
+        self.optfield_view = None
         self._check_and_setup_optfield_view()
 
         # Open the first record.
-        if seek_to and isinstance(seek_to, dict):
-            self.seek_to(fetch=fetch, **seek_to)
-        self.log.debug("opened.")
-
-    @classmethod
-    def from_me(cls, _me):
-        return ExView(_me.rotoid, _me=me)
-
-    @classmethod
-    def table_name(cls, rotoid):
-        # If rotoid is dotted, the table name is the last entry.
-        if "." in rotoid:
-            return rotoid.split('.')[-1]
-
-        # Try the map first, it is already in memory
-        if rotoid in VIEW_INFO_MAP:
-            return VIEW_INFO_MAP[rotoid]['name']
-
-        # Fall back to the table, which may or may not be populated.
-        try:
-            with exview("VI0005", seek_to={"VIEWID": rotoid}) as view:
-                return view.name
-        except ExViewError as e:
-            pass
+        if isinstance(seek_to, dict):
+            self.seek_to(**seek_to)
 
-        # fail
-        return ""
-
-    @notme
     def cached_view(self, viewid):
         """Get a view from the view cache.
-
+        
         :param viewid: the view ID, i.e. OE0500
         :type viewid: str
         :raises: ExViewError
         """
         view = self._view_cache.get(viewid)
         created = False
         if not view:
             view = ExView(viewid, self.index, _root=False)
             self._view_cache[viewid] = view
             created = True
+        
         return view, created
 
-    @notme
     def remove_cached_view(self, viewid):
         """Remove and close a view from the cache.
-
+        
         :param viewid: the view ID, i.e. OE0500
         :type viewid: str
         :raises: ExViewError
         """
         # We remove ourself from the cache in close only.
         if viewid == self.rotoid:
             raise ExViewError(self.rotoid, action="remove_cache")
-
+            
         view = self._view_cache.get(viewid)
         if view:
             view.close()
-
+        
         try:
             del self._view_cache[viewid]
         except KeyError:
             pass
-
+    
     @property
     def _view_cache(self):
         """Get the views cached for this index."""
-
+        
         cache_for_index = self.__exview_cache.get(self.index, {})
         if not cache_for_index:
             self.__exview_cache[self.index] = cache_for_index
-
+        
         return self.__exview_cache[self.index]
 
     def _check_and_setup_detail_view(self):
         """Check if this or a composed view is a detail view.
 
         :returns: True if self is or is composed with a detail view.
         :rtype: bool
         """
-
-        for view in self._cviews:
-            if view and self.DETAIL_VIEW_HINTS.intersection(
-                                                        view.field_names):
-                self.detail_view = view
-                break
-
-        if not self.detail_view:
-            if self.DETAIL_VIEW_HINTS.intersection(self.field_names):
-                self.detail_view = self
+        if self.DETAIL_VIEW_HINTS.intersection(self.field_names):
+            self.detail_view = self
+        else:
+            for view in self._cviews:
+                if view and self.DETAIL_VIEW_HINTS.intersection(
+                                                            view.field_names):
+                    self.detail_view = view
+                    break
 
         if self.detail_view:
-            self.log.debug("identified detail view {}".format(
-                    self.detail_view.rotoid))
             self._detail_func_factory(self.detail_view)
             return True
 
         return False
 
     def _check_and_setup_optfield_view(self):
         """Check if this or a composed view is an optional field view.
@@ -483,65 +349,57 @@
             for view in self._cviews:
                 if view and self.OPTFIELD_VIEW_HINTS.intersection(
                                                             view.field_names):
                     self.optfield_view = view
                     break
 
         if self.optfield_view:
-            self.log.debug("identified optfield view {}".format(
-                    self.optfield_view.rotoid))
             self._optf_func_factory(self.optfield_view)
             return True
 
         return False
 
-    @notme
     def _open(self):
         """Open the underlying view object. Called automatically on init.
 
         :raises: ExViewOpenError
         :rtype: None
         """
         if self._view:
             _c = self._view.close()
         self._view = View(self.rotoid, self.index)
         if not self._view:
             raise ExViewOpenError(self.rotoid, action_return=self._view)
         o = self._view.order(self._order)
         if not success(o):
-            raise ExViewInvalidOrder(self.rotoid,
-                                        order=self.order,
-                                        action_return=o)
+            raise ExViewOrderError(self.rotoid,
+                                   order=self.order,
+                                   action_return=o)
 
         self._view_cache[self.rotoid] = self
         return True
 
     def _get_field_names(self):
         """Get the field names from their positions in the view."""
         for i in range(0, self._view.fields()):
             field = self._view.fieldByPosition(i)
             if field:
                 self.field_names.append(field.name)
-                self.fields[field.name] = field
-
-    def _get_field_type(self, field):
-        f = self.fields[field]
-        return f.type
 
     def _get_indexes(self):
         """Get the indexes and their constituent fields."""
         for i in range(0, self._view.keyCount()):
             k = self._view.key(i)
             names = [self._view.fieldByIndex(j).name for j in k.fields]
             self.indexes.insert(i, names)
-
+    
     def _get_composed_views(self):
         """Get the composed view list."""
         self._views = self._composed_views()
-
+    
     def _get_index_for_fields(self, fields):
         sfields = set(fields)
         for i in range(0, len(self.indexes)):
             if sfields == set(self.indexes[i]):
                 return i
 
     def _setup_wrapper(self):
@@ -567,21 +425,18 @@
         :type funcname: str
         :returns: wrapper around ``self._view.<funcname>``
         :rtype: function
         """
         def func(*args, **kwargs):
             fu = getattr(self._view, funcname)
             r = fu(*args, **kwargs)
-            self.log.debug("{}({}, {}): {}".format(funcname, args, kwargs, r))
             if not success(r):
                 raise ExViewError(self.rotoid,
                                   action=funcname,
-                                  action_return=r,
-                                  fargs=args,
-                                  fkwargs=kwargs)
+                                  action_return=r)
             return r
         return func
 
     def _composed_views(self):
         """Get a list of all views that can be composed with this one.
 
         This method automatically filters out views that do not support
@@ -701,192 +556,109 @@
                                       for (k, v) in criteria.items()]))
             while(view.fetch()):
                 yield view
         self.lines_where = lines_where
 
     def all(self, ascending=True):
         """Generator that yields once for each record in the view.
-
+        
         :raises: ExViewError
         :yields: ExView
         """
         self.recordClear()
         self.browse("", ascending)
         while(self.fetch()):
             yield self
-
+    
     def where(self, **criteria):
-        """Get an ExQuery to retrieve records with the given criteria.
+        """Generator that yields each line matching the provided criteria.
 
         :param criteria: ``field=value`` criteria to browse to.
         :type critera: dict
-        :returns: ExQuery
+        :yields: ExView
         :raises: ExViewError
         """
-        from extools.view.query import ExQuery
-        self.log.debug("where({})".format(criteria))
-        return ExQuery(self.rotoid, _parent_keys=self.parent_key(), **criteria)
-
-    def current_key(self):
-        """Get the current unique key identifying the view record.
-
-        :returns: {field: value, field: value...}
-        """
-        kvs = {}
-        if self.indexes:
-            for field in self.indexes[0]:
-                kvs[field] = self._view.get(field)
-            # self.log.debug("current_key(): {}".format(kvs))
-        return kvs
-
-    def parent_key(self):
-        """Get the current unique key identifying the view record's parent.
-
-        Only relevant for detail views, return the key components before
-        the last one.
-
-        The views, as classified by Sage, may either be header, detail, flat
-        or batch.  Both detail, and headers with composite keys, may be
-        enumerated.
-
-        :returns: {field: value, field: value...}
-        """
-        kvs = {}
-        self.log.debug("deriving parent key for {} ({}) {}".format(
-            self.rotoid, self.protocol, self.to_dict()))
-        if self.protocol in ["DETAIL", "HEADER", ]:
-            if self.indexes:
-                if len(self.indexes[0]) > 1:
-                    for field in self.indexes[0][:-1]:
-                        kvs[field] = self._view.get(field)
-        return kvs
+        self.recordClear()
+        self.browse(" AND ".join(['{} = "{}"'.format(k, v)
+                                  for (k, v) in criteria.items()]))
+        while(self.fetch()):
+            yield self
+    
 
     def create(self, **fields):
         """Generate and insert a new entry with field/value pairs.
 
         :param fields: field value pairs that will be set on the new entry.
         :type fields: field=value
         :rtype: None
         :raises: ExViewError
         """
-        if self.indexes:
-            key_vals = ["{}={}".format(f, fields.get(f, ""))
-                        for f in self.indexes[0]]
-        else:
-            key_vals = ["{}={}".format(f, fields[f])
-                        for f in fields]
-        self.log.debug("creating {}".format(", ".join(key_vals)))
         self.recordClear()
         self.recordGenerate()
         for (field, value) in fields.items():
             self.put(field, value)
         self.insert()
 
-
     def update(self, **fields):
         """Update an entry with field/value pairs.
 
         :param kwargs: field value pairs that will be set on the new entry.
         :type kwargs: field=value
         :rtype: None
         :raises: ExViewError
         """
-        if self.indexes:
-            key_vals = ["{}={}".format(f, fields.get(f, ""))
-                        for f in self.indexes[0]]
-        else:
-            key_vals = ["{}={}".format(f, fields[f])
-                        for f in fields]
-        self.log.debug("updating {} with {}".format(
-            ", ".join(key_vals),
-            ", ".join(["{}={}".format(k,v) for k,v in fields.items()])))
-
         for (field, value) in fields.items():
             self.put(field, value)
         up = self._view.update()
         if not success(up):
             raise ExViewError(self.rotoid, action="update", action_return=up)
 
-
     def fetch(self):
         """A special wrapper because a non-zero fetch return isn't an error.
 
         :returns: True if a new line was fetched, else False.
         :rtype: bool
         """
         f = self._view.fetch()
-        self.log.debug("fetch(): {} [{}]".format(
-            success(f), self.current_key()))
-        return success(f)
-
-    def read(self):
-        """A special wrapper to raise ExViewRecordDoesNotExist.
-
-        :raises: ExViewRecordDoesNotExist
-        """
-        r = self._view.read()
-        self.log.debug("read(): {} [{}]".format(r, self.current_key()))
-        if not success(r):
-            raise ExViewRecordDoesNotExist(self.rotoid, action='read')
+        if success(f):
+            return True
+        return False
 
-    def get(self, field, _type=-1, size=-1, precision=-1, verify=True):
+    def get(self, field):
         """A special wrapper because get doesn't return 0 on success.
 
         :param field: field name to get.
         :type field: str
-        :param verify: verify that the field is listed in the view fields?
-        :type: bool
         :returns: value in the view.
         :rtype: builtin.*
         :raises: ExViewFieldDoesNotExist
         """
-        if verify and not field in self.field_names:
+        if not field in self.field_names:
             raise ExViewFieldDoesNotExist(self.rotoid,
                                           field=field,
                                           action="get")
 
-        val = self._view.get(field, _type, size, precision)
-        if self.native_types and field in self.field_names:
-            if self.fields[field].type == FT_DATE:
-                val = datetime.strptime(str(int(val)), "%Y%m%d")
-            elif self.fields[field].type == FT_TIME:
-                val = datetime.strptime(str(int(val)).zfill(8)[:6], "%H%M%S")
+        return self._view.get(field)
 
-        self.log.debug("get({}, {}, {}, {}, {}): {} [{}]".format(
-                field, _type, size, precision, verify, val, type(val)))
-
-        return val
-
-    def order(self, _ord):
+    def order(self, ord):
         """Wrap the order to track state in the class as it can't be queried.
 
         :param index: the index ID to order by.
         :type index: int
         :rtype: None
         :raises: ExViewError
         """
-        o = self._view.order(_ord)
-        self.log.debug("order({}): {}".format(_ord, o))
+        o = self._view.order(ord)
+
         if not success(o):
-            raise ExViewInvalidOrder(self.rotoid, _ord, action_return=o)
+            raise ExViewOrderError(self.rotoid, ord, action_return=o)
 
-        self._order = _ord
+        self._order = ord
         return o
 
-    def exists(self):
-        """Wrap exists to return True or False and not raise.
-
-        :returns: True if record in view exists (has been added), else False
-        :rtype: bool
-        """
-        if self._view.exists():
-            return True
-        return False
-
-    @notme
     def compose(self):
         """Recursively compose this and all related views.
 
         Enables this ``ExView`` to self-compose based on the compose
         information stored in the View.
 
         :raises: ExViewComposeError
@@ -917,25 +689,25 @@
             except ExViewComposeError as e:
                 # Handle a compose failure.
             except ExViewOpenError as e:
                 # Handle a view open error
             except ExViewError as e:
                 # handle an error processing the lines.
 
-        Note that :py:class:`extools.view.ExViewComposeError` and
-        :py:class:`extools.view.ExViewOpenError` are both children of
-        :py:class:`extools.view.ExViewError`, so if you don't care which
+        Note that :py:class:`extools.exview.ExViewComposeError` and
+        :py:class:`extools.exview.ExViewOpenError` are both children of
+        :py:class:`extools.exview.ExViewError`, so if you don't care which
         failure occurred, you can just except the more general ``ExViewError``.
 
         For more information and background, see :ref:`Self-composing views`.
         """
         try:
             # Find the blacklist filtered composed view list
             self._views = self._composed_views()
-            self.log.debug("composing with views {}".format(self._views))
+
             # Store the views to compose with this one in order.
             self._cviews = []
 
             # For each of the composed views...
             for i in range(0, len(self._views)):
 
                 # The entry may be None or blacklisted. Either way, there is
@@ -963,98 +735,61 @@
                     if view:
                         setattr(self, view.rotoid.lower(), view)
 
                 # Re-check the for optional field  and detail views.
                 self._check_and_setup_optfield_view()
                 self._check_and_setup_detail_view()
                 self.composed = True
-
+                
         except RuntimeError as err:
             raise ExViewComposeError(self.rotoid, compose_list=self._views,
                                      triggering_exc=err)
 
-    def compose_from(self, composed_views):
-        self.log.debug("composing from {}".format(composed_views))
-        try:
-            # Store the views to compose with this one in order.
-            self._cviews = []
-
-            with exview(self.rotoid) as exv:
-                cinfo = exv._composed_views()
-
-            # For each of the composed views...
-            for i in range(0, len(composed_views)):
-
-                # The entry may be None or blacklisted. Either way, there is
-                # no view to compose at this index.
-                if composed_views[i] and not composed_views[i] in EXVIEW_BLACKLIST:
-                    # Add the composed view to the compose list.
-                    exv = ExView(cinfo[i], _root=False, _me=composed_views[i])
-                    self._cviews.insert(i, exv)
-                    setattr(self, cinfo[i].lower(), exv)
-                else:
-                    # The entry was None, propagate to preserve argument order.
-                    self._cviews.insert(i, None)
-
-
-            # Re-check the for optional field  and detail views.
-            self._check_and_setup_optfield_view()
-            self._check_and_setup_detail_view()
-            self.composed = True
-
-        except RuntimeError as err:
-            raise ExViewComposeError(self.rotoid, compose_list=self._views,
-                                     triggering_exc=err)
-
-
-    @notme
     def _close_all_cached_views(self):
         """Close all composed views in the _view_cache.
-
+        
         :raises: ExViewError
         """
         views = [v for v in self._view_cache.values()]
         for view in views:
             if view:
                 if not view._root:
                     self.remove_cached_view(view.rotoid)
             else:
                  self.remove_cached_view(view.rotoid)
 
-    @notme
+
     def close(self):
         """Close me cleanly, closing all composed views first.
-
+        
         :rtype: None
         :raises: ExViewError
         """
-        self.log.debug('closing.')
+
         if self._root and len(self._view_cache.values()) > 1:
             self._close_all_cached_views()
         c = self._view.close()
         if not success(c):
             raise ExViewError(self.rotoid, action='close', action_return=c)
         if self.rotoid in self._view_cache.keys():
             del self._view_cache[self.rotoid]
 
-    def seek_to(self, fetch=True, **kwargs):
+    def seek_to(self, **kwargs):
         """Intelligently seek to a specific entry.
 
         This seek to implementation accepts an arbitrary set of field value
         pairs and then seeks to the entry using one of three methods:
 
         - If the current View order index is made up of exactly the fields
           requested, perform a straight put and read.
         - If the current View has an index made up of exactly the fields
           requested, temporarily change the index and perform and put a read.
         - If the current View does not have and index made up of exactly the
           fields requested, attempt to browse and fetch the record.
 
-        :param fetch: fetch after seeking? Default to true.
-        :type fetch: bool
         :param kwargs: (key)=(value) pairs, where the keys must be the same as
                         the current index keys.
         :type kwargs: dict
         :rtype: None
         :raises: ExViewError
 
         .. code-block:: python
@@ -1074,49 +809,44 @@
 
                 # The error, "failed to [open|seek]", is contained in the
                 # error message.
                 showMessage("Error doing something with view {}: {}".format(
                     viewid, e))
 
         """
-        self.log.debug("seeking to {}".format(kwargs))
         # If the current index matches the fields, read the record.
         if set(self.indexes[self._order]) == set(kwargs.keys()):
             # Try to read the record
-            self.log.debug("key match, reading.")
             self.recordClear()
             for (key, value) in kwargs.items():
                 self.put(key, value)
             self.read()
 
         elif self._get_index_for_fields(kwargs.keys()):
             # If there exists an index with these fields, use it.
             # Set the order back after reading
             index = self._get_index_for_fields(kwargs.keys())
-            self.log.debug("matching index? {}".format(index))
             if index is not None:
                 # Try to read the record
                 original_order = self._order
                 try:
                     self.order(index)
                     self.recordClear()
                     for (key, value) in kwargs.items():
                         self.put(key, value)
                     self.read()
                 finally:
                     self.order(original_order)
         else:
             # No index exists with these fields, try browsing.
-            self.log.debug("no index match.")
             criteria = " AND ".join(['{} = "{}"'.format(f, v)
                                      for (f, v) in kwargs.items()])
             self.recordClear()
             self.browse(criteria)
-            if fetch and not self.fetch():
-                raise ExViewRecordDoesNotExist(self.rotoid, "seek_to")
+            self.fetch()
 
     @property
     def is_optfield_view(self):
         """Is this an optional field view?
 
         :returns: True if this view is an optional field view.
         :rtype: bool
@@ -1132,58 +862,14 @@
         :returns: True if this view is composed with an optional field view.
         :rtype: bool
         """
         if self.optfield_view and not self.optfield_view == self:
             return True
         return False
 
-    def copy_to(self, view2, force=True, exclude=[], include=[], post_process=[],
-            skip_keys=True, skip_computed=True, save=False):
-        """Copy the current object to view2.
-
-        :param view2: the view to copy to.
-        :type view2: ExView
-        :param exclude: Fields to exclude from copy.
-        :type exclude: str[]
-        :param include: Fields to include, excluding all others.
-        :type include: str[]
-        :param post_process: run process with these processcmds after copy.
-        :type post_process: int[]
-        :param skip_keys: skip fields with the Key attribute. Default: yes.
-        :type skip_keys: bool
-        :param skip_computed: skip fields with the Key attribute. Default: yes.
-        :type skip_computed: bool
-        :param save: insert the object after copy. Default: no.
-        :type save: bool
-        :raises ExViewError: when any error occurs during the copy.
-        """
-        v1_fields = self.to_dict()
-        for field in self.field_names:
-            if field in exclude:
-                continue
-            if include and not field in include:
-                continue
-            value = v1_fields[field]
-
-            index = self._view.fieldByName(field).index
-            attrs = self._view.attribs(index)
-            if attrs & self.ATTR_EDITABLE:
-                if skip_keys and attrs & self.ATTR_KEY:
-                    continue
-                if skip_computed and attrs & self.ATTR_COMPUTED:
-                    continue
-                view2.put(field, value)
-        for cmd in post_process:
-            if cmd:
-                view2.put("PROCESSCMD", cmd)
-                view2.process()
-        if save:
-            view2.insert()
-        return view2
-
     def __getattr__(self, attr):
         """Check all unknown attributes against the underlying view.
 
         This is where some of the magic is. When a call is made to a property
         or method that is not explicitly (either static or dynamic)
         defined in ExView this handler is triggered by the interpreter.
 
@@ -1192,77 +878,14 @@
         delegate the call.
 
         An example is the ``.handle()`` method, a key one on views.  It isn't
         defined explicitly or dynamically on the ``ExView`` class but if you
         try calling ``exview.handle`` it will return the host view handle.
         The call was delegated to the ``_view`` here.
         """
-        try:
-            if hasattr(self, "_view"):
-                if hasattr(self._view, attr):
-                    return getattr(self._view, attr)
-                elif hasattr(self, "field_names"):
-                    if attr.upper() in self.field_names:
-                        return self.get(attr.upper())
-            raise AttributeError("attribute not found.")
-        except Exception as e:
-            self.log.error("failed to getattr {}: {}".format(
-                    attr, e), exc_info=True)
-            raise AttributeError(
-                "{} isn't set on self, _view, or a view field.".format(attr))
-
-    '''
-    def __setattr__(self, attr, value):
-        """Set a view field in short-hand.
-
-        Allows you to do this:
-
-        .. code-block: python
-
-            with exview("OE0500", seek_to={"ORDNUMBER": "ORD001"}) as exv:
-                exv.qtyordered = 50
-                exv.update()
-        """
-        if attr in self.field_names:
-            self.put(attr, value)
-        else:
-            super().__setattr__(attr, value)
-    '''
-
-    def __getitem__(self, attr):
-        """Return the value of the field from the view, if it exists.
-
-        A shorthand for .get() without params.
-        """
-        try:
-            return self.get(attr.upper())
-        except ExViewFieldDoesNotExist:
-            raise KeyError("Field {} does not exist in {}.".format(
-                attr, self.rotoid))
-
-    def __setitem__(self, attr, value):
-        """Set a view field in dict access notation.
-
-        Allows you to do this:
-
-        .. code-block: python
-
-            with exview("OE0500", seek_to={"ORDNUMBER": "ORD001"}) as exv:
-                exv['qtyordered'] = 50
-                exv.update()
-        """
-        if attr.upper() not in self.field_names:
-            raise KeyError("Field {} does not exist in {}.".format(
-                attr, self.rotoid))
-        self.put(attr.upper(), value)
-
-    def to_dict(self):
-        """Return all the fields in a view as a dictionary.
-
-        Useful for caching full rows for later use.
-        """
-        return { k: self._view.get(k)
-                 for k in self.field_names
-                 if self.fields[k].desc not in FIELD_DESC_BLACKLIST }
+        if hasattr(self, "_view") and hasattr(self._view, attr):
+            return getattr(self._view, attr)
+        raise AttributeError("Attr {} doesn't exist on {} or View.".format(
+            attr, self.rotoid))
 
     def __str__(self):
         return "ExView({})".format(self.rotoid)
```

### Comparing `extools-0.13.43/extools.egg-info/PKG-INFO` & `extools-0.3.0/extools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: extools
-Version: 0.13.43
+Version: 0.3.0
 Summary: Tools for Orchid Extender
-Home-page: https://poplars.dev
-Author: Chris Binckly, 2665093 Ontario Inc.
+Home-page: https://2665093.ca
+Author: Chris Binckly, 2665092 Ontario Inc.
 Author-email: cbinckly@gmail.com
 License: UNKNOWN
 Description: ##################
         Tools for Extender
         ##################
         
         -------------------------------------------------
@@ -72,8 +72,7 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.4
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Description-Content-Type: text/x-rst
```

### Comparing `extools-0.13.43/setup.py` & `extools-0.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,33 +4,34 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='extools',
-    version='0.13.43',
+    version='0.3.0',
     description='Tools for Orchid Extender',
     long_description=long_description,
     long_description_content_type='text/x-rst',
-    url='https://poplars.dev',
-    author='Chris Binckly, 2665093 Ontario Inc.',
+    url='https://2665093.ca',
+    author='Chris Binckly, 2665092 Ontario Inc.',
     author_email='cbinckly@gmail.com',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'Environment :: Win32 (MS Windows)',
         'Operating System :: Microsoft :: Windows',
         'Programming Language :: Python :: 3.4',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
     ],
     keywords='sage orchid extender',
     packages=find_packages(exclude=['contrib', 'docs', 'tests']),
-    install_requires=[
-        'jinja2>=2.10.1'
-        ],
+    python_requires='=3.4.*',
+    install_requires=[],
+    extras_require={
+    },
     package_data={
         'extools': ['expi.json', 'vi/*.vi',],
     },
 )
```

