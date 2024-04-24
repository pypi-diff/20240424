# Comparing `tmp/pipez-0.0.93.tar.gz` & `tmp/pipez-0.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipez-0.0.93.tar", last modified: Wed Apr 24 12:34:34 2024, max compression
+gzip compressed data, was "pipez-0.0.94.tar", last modified: Wed Apr 24 15:45:29 2024, max compression
```

## Comparing `pipez-0.0.93.tar` & `pipez-0.0.94.tar`

### file list

```diff
@@ -1,232 +1,232 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:34.347904 pipez-0.0.93/
--rw-rw-rw-   0        0        0    35823 2024-01-22 12:34:35.000000 pipez-0.0.93/LICENSE
--rw-rw-rw-   0        0        0      126 2024-04-08 09:46:56.000000 pipez-0.0.93/MANIFEST.in
--rw-rw-rw-   0        0        0     4041 2024-04-24 12:34:34.346308 pipez-0.0.93/PKG-INFO
--rw-rw-rw-   0        0        0     3499 2024-04-13 20:09:12.000000 pipez-0.0.93/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:33.906102 pipez-0.0.93/pipez/
--rw-rw-rw-   0        0        0       24 2024-04-24 12:33:57.000000 pipez-0.0.93/pipez/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:33.957108 pipez-0.0.93/pipez/core/
--rw-rw-rw-   0        0        0      146 2024-04-13 20:09:12.000000 pipez-0.0.93/pipez/core/__init__.py
--rw-rw-rw-   0        0        0     1247 2024-04-13 19:08:05.000000 pipez-0.0.93/pipez/core/batch.py
--rw-rw-rw-   0        0        0      543 2024-04-13 15:27:35.000000 pipez-0.0.93/pipez/core/enums.py
--rw-rw-rw-   0        0        0     2331 2024-02-04 10:03:20.000000 pipez-0.0.93/pipez/core/legacy_batch.py
--rw-rw-rw-   0        0        0     2837 2024-04-13 16:03:09.000000 pipez-0.0.93/pipez/core/legacy_build.py
--rw-rw-rw-   0        0        0     9549 2024-04-13 20:09:12.000000 pipez-0.0.93/pipez/core/legacy_node.py
--rw-rw-rw-   0        0        0     1148 2024-04-12 14:59:21.000000 pipez-0.0.93/pipez/core/legacy_registry.py
--rw-rw-rw-   0        0        0     2795 2024-02-02 11:31:56.000000 pipez-0.0.93/pipez/core/legacy_shared_memory.py
--rw-rw-rw-   0        0        0     3713 2024-04-12 19:23:48.000000 pipez-0.0.93/pipez/core/legacy_watchdog.py
--rw-rw-rw-   0        0        0      747 2024-04-12 15:57:46.000000 pipez-0.0.93/pipez/core/memory.py
--rw-rw-rw-   0        0        0     1034 2024-04-24 11:55:20.000000 pipez-0.0.93/pipez/core/metrics.py
--rw-rw-rw-   0        0        0     6023 2024-04-24 11:51:30.000000 pipez-0.0.93/pipez/core/node.py
--rw-rw-rw-   0        0        0      850 2024-04-12 18:24:39.000000 pipez-0.0.93/pipez/core/queue_wrapper.py
--rw-rw-rw-   0        0        0      577 2024-04-12 15:40:37.000000 pipez-0.0.93/pipez/core/registry.py
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:33.958498 pipez-0.0.93/pipez/core/static/
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:33.968571 pipez-0.0.93/pipez/core/static/DataTables/
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:33.870905 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:34.009324 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/
--rw-rw-rw-   0        0        0    13174 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap.css
--rw-rw-rw-   0        0        0    11219 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap.min.css
--rw-rw-rw-   0        0        0    13511 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap4.css
--rw-rw-rw-   0        0        0    11523 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap4.min.css
--rw-rw-rw-   0        0        0    14198 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap5.css
--rw-rw-rw-   0        0        0    12168 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap5.min.css
--rw-rw-rw-   0        0        0    12157 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bulma.css
--rw-rw-rw-   0        0        0    10395 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bulma.min.css
--rw-rw-rw-   0        0        0        0 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.dataTables.css
--rw-rw-rw-   0        0        0        0 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.dataTables.min.css
--rw-rw-rw-   0        0        0    11266 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.foundation.css
--rw-rw-rw-   0        0        0     9580 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.foundation.min.css
--rw-rw-rw-   0        0        0    28554 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.jqueryui.css
--rw-rw-rw-   0        0        0    24415 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.jqueryui.min.css
--rw-rw-rw-   0        0        0    11471 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.semanticui.css
--rw-rw-rw-   0        0        0     9783 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.semanticui.min.css
--rw-rw-rw-   0        0        0    26541 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/jquery.dataTables.css
--rw-rw-rw-   0        0        0    22712 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/jquery.dataTables.min.css
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:34.019856 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/images/
--rw-rw-rw-   0        0        0      160 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/images/sort_asc.png
--rw-rw-rw-   0        0        0      148 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/images/sort_asc_disabled.png
--rw-rw-rw-   0        0        0      201 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/images/sort_both.png
--rw-rw-rw-   0        0        0      158 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/images/sort_desc.png
--rw-rw-rw-   0        0        0      146 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/images/sort_desc_disabled.png
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:34.059480 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/
--rw-rw-rw-   0        0        0     5214 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap.js
--rw-rw-rw-   0        0        0     2226 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap.min.js
--rw-rw-rw-   0        0        0     5350 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap4.js
--rw-rw-rw-   0        0        0     2343 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap4.min.js
--rw-rw-rw-   0        0        0     5494 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap5.js
--rw-rw-rw-   0        0        0     2361 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap5.min.js
--rw-rw-rw-   0        0        0     5701 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bulma.js
--rw-rw-rw-   0        0        0     2484 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bulma.min.js
--rw-rw-rw-   0        0        0     1205 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.dataTables.js
--rw-rw-rw-   0        0        0      588 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.dataTables.min.js
--rw-rw-rw-   0        0        0     5235 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.foundation.js
--rw-rw-rw-   0        0        0     2398 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.foundation.min.js
--rw-rw-rw-   0        0        0     2518 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.jqueryui.js
--rw-rw-rw-   0        0        0     1226 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.jqueryui.min.js
--rw-rw-rw-   0        0        0     5923 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.semanticui.js
--rw-rw-rw-   0        0        0     2672 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.semanticui.min.js
--rw-rw-rw-   0        0        0   473441 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/jquery.dataTables.js
--rw-rw-rw-   0        0        0    87279 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/jquery.dataTables.min.js
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:33.873272 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:34.097493 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/
--rw-rw-rw-   0        0        0     1316 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap.css
--rw-rw-rw-   0        0        0     1124 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap.min.css
--rw-rw-rw-   0        0        0     1339 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap4.css
--rw-rw-rw-   0        0        0     1147 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap4.min.css
--rw-rw-rw-   0        0        0     1452 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap5.css
--rw-rw-rw-   0        0        0     1247 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap5.min.css
--rw-rw-rw-   0        0        0     1263 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bulma.css
--rw-rw-rw-   0        0        0     1084 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bulma.min.css
--rw-rw-rw-   0        0        0     1263 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.dataTables.css
--rw-rw-rw-   0        0        0     1084 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.dataTables.min.css
--rw-rw-rw-   0        0        0      396 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.foundation.css
--rw-rw-rw-   0        0        0      339 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.foundation.min.css
--rw-rw-rw-   0        0        0     1263 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.jqueryui.css
--rw-rw-rw-   0        0        0     1084 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.jqueryui.min.css
--rw-rw-rw-   0        0        0     1263 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.semanticui.css
--rw-rw-rw-   0        0        0     1084 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.semanticui.min.css
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:34.136800 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/
--rw-rw-rw-   0        0        0    41008 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/dataTables.scroller.js
--rw-rw-rw-   0        0        0    12430 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/dataTables.scroller.min.js
--rw-rw-rw-   0        0        0     1339 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap.js
--rw-rw-rw-   0        0        0      691 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap.min.js
--rw-rw-rw-   0        0        0     1341 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap4.js
--rw-rw-rw-   0        0        0      693 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap4.min.js
--rw-rw-rw-   0        0        0     1341 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap5.js
--rw-rw-rw-   0        0        0      693 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap5.min.js
--rw-rw-rw-   0        0        0     1333 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bulma.js
--rw-rw-rw-   0        0        0      685 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bulma.min.js
--rw-rw-rw-   0        0        0     1338 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.dataTables.js
--rw-rw-rw-   0        0        0      690 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.dataTables.min.js
--rw-rw-rw-   0        0        0     1338 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.foundation.js
--rw-rw-rw-   0        0        0      690 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.foundation.min.js
--rw-rw-rw-   0        0        0     1341 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.jqueryui.js
--rw-rw-rw-   0        0        0      693 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.jqueryui.min.js
--rw-rw-rw-   0        0        0     1338 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.semanticui.js
--rw-rw-rw-   0        0        0      690 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.semanticui.min.js
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:33.879440 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:34.171478 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/
--rw-rw-rw-   0        0        0     6724 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap.css
--rw-rw-rw-   0        0        0     5854 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap.min.css
--rw-rw-rw-   0        0        0     6981 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap4.css
--rw-rw-rw-   0        0        0     6077 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap4.min.css
--rw-rw-rw-   0        0        0     7186 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap5.css
--rw-rw-rw-   0        0        0     6249 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap5.min.css
--rw-rw-rw-   0        0        0     7015 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bulma.css
--rw-rw-rw-   0        0        0     6100 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bulma.min.css
--rw-rw-rw-   0        0        0     8908 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.dataTables.css
--rw-rw-rw-   0        0        0     7734 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.dataTables.min.css
--rw-rw-rw-   0        0        0     7184 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.foundation.css
--rw-rw-rw-   0        0        0     6254 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.foundation.min.css
--rw-rw-rw-   0        0        0     6733 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.jqueryui.css
--rw-rw-rw-   0        0        0     5869 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.jqueryui.min.css
--rw-rw-rw-   0        0        0     8090 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.semanticui.css
--rw-rw-rw-   0        0        0     7041 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.semanticui.min.css
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:34.210414 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/
--rw-rw-rw-   0        0        0   179224 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/dataTables.searchBuilder.js
--rw-rw-rw-   0        0        0    67309 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/dataTables.searchBuilder.min.js
--rw-rw-rw-   0        0        0     1950 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap.js
--rw-rw-rw-   0        0        0     1190 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap.min.js
--rw-rw-rw-   0        0        0     1941 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap4.js
--rw-rw-rw-   0        0        0     1181 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap4.min.js
--rw-rw-rw-   0        0        0     2021 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap5.js
--rw-rw-rw-   0        0        0     1247 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap5.min.js
--rw-rw-rw-   0        0        0     1812 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bulma.js
--rw-rw-rw-   0        0        0     1066 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bulma.min.js
--rw-rw-rw-   0        0        0     1366 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.dataTables.js
--rw-rw-rw-   0        0        0      718 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.dataTables.min.js
--rw-rw-rw-   0        0        0     1901 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.foundation.js
--rw-rw-rw-   0        0        0     1141 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.foundation.min.js
--rw-rw-rw-   0        0        0     2291 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.jqueryui.js
--rw-rw-rw-   0        0        0     1531 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.jqueryui.min.js
--rw-rw-rw-   0        0        0     2527 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.semanticui.js
--rw-rw-rw-   0        0        0     1550 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.semanticui.min.js
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:33.881815 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:34.243910 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/
--rw-rw-rw-   0        0        0    12192 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap.css
--rw-rw-rw-   0        0        0    10844 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap.min.css
--rw-rw-rw-   0        0        0    12489 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap4.css
--rw-rw-rw-   0        0        0    11153 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap4.min.css
--rw-rw-rw-   0        0        0    15085 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap5.css
--rw-rw-rw-   0        0        0    13537 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap5.min.css
--rw-rw-rw-   0        0        0    12232 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bulma.css
--rw-rw-rw-   0        0        0    10955 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bulma.min.css
--rw-rw-rw-   0        0        0    14718 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.dataTables.css
--rw-rw-rw-   0        0        0    13089 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.dataTables.min.css
--rw-rw-rw-   0        0        0    12527 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.foundation.css
--rw-rw-rw-   0        0        0    11137 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.foundation.min.css
--rw-rw-rw-   0        0        0    15420 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.jqueryui.css
--rw-rw-rw-   0        0        0    13689 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.jqueryui.min.css
--rw-rw-rw-   0        0        0    14238 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.semanticui.css
--rw-rw-rw-   0        0        0    12644 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.semanticui.min.css
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:34.283844 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/
--rw-rw-rw-   0        0        0   167377 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/dataTables.searchPanes.js
--rw-rw-rw-   0        0        0    56665 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/dataTables.searchPanes.min.js
--rw-rw-rw-   0        0        0     2183 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap.js
--rw-rw-rw-   0        0        0     1360 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap.min.js
--rw-rw-rw-   0        0        0     2295 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap4.js
--rw-rw-rw-   0        0        0     1444 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap4.min.js
--rw-rw-rw-   0        0        0     2159 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap5.js
--rw-rw-rw-   0        0        0     1336 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap5.min.js
--rw-rw-rw-   0        0        0     1782 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bulma.js
--rw-rw-rw-   0        0        0     1046 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bulma.min.js
--rw-rw-rw-   0        0        0     1357 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.dataTables.js
--rw-rw-rw-   0        0        0      709 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.dataTables.min.js
--rw-rw-rw-   0        0        0     2117 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.foundation.js
--rw-rw-rw-   0        0        0     1311 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.foundation.min.js
--rw-rw-rw-   0        0        0     1862 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.jqueryui.js
--rw-rw-rw-   0        0        0     1134 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.jqueryui.min.js
--rw-rw-rw-   0        0        0     2152 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.semanticui.js
--rw-rw-rw-   0        0        0     1301 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.semanticui.min.js
--rw-rw-rw-   0        0        0    38379 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/datatables.css
--rw-rw-rw-   0        0        0  1166936 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/datatables.js
--rw-rw-rw-   0        0        0    33659 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/datatables.min.css
--rw-rw-rw-   0        0        0   316604 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/datatables.min.js
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:34.288429 pipez-0.0.93/pipez/core/static/DataTables/jQuery-3.7.0/
--rw-rw-rw-   0        0        0   295700 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/jQuery-3.7.0/jquery-3.7.0.js
--rw-rw-rw-   0        0        0    87464 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/static/DataTables/jQuery-3.7.0/jquery-3.7.0.min.js
--rw-rw-rw-   0        0        0        0 2024-02-13 14:55:57.000000 pipez-0.0.93/pipez/core/static/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:34.293436 pipez-0.0.93/pipez/core/templates/
--rw-rw-rw-   0        0        0        0 2024-02-02 08:26:03.000000 pipez-0.0.93/pipez/core/templates/__init__.py
--rw-rw-rw-   0        0        0     4968 2024-02-05 15:51:59.000000 pipez-0.0.93/pipez/core/templates/home.html
--rw-rw-rw-   0        0        0     4211 2024-04-24 12:33:45.000000 pipez-0.0.93/pipez/core/watchdog.py
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:34.295753 pipez-0.0.93/pipez/nodes/
--rw-rw-rw-   0        0        0        0 2024-03-21 18:00:34.000000 pipez-0.0.93/pipez/nodes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:34.301051 pipez-0.0.93/pipez/nodes/common/
--rw-rw-rw-   0        0        0       56 2024-04-13 18:05:30.000000 pipez-0.0.93/pipez/nodes/common/__init__.py
--rw-rw-rw-   0        0        0      749 2024-04-14 00:13:16.000000 pipez-0.0.93/pipez/nodes/common/group.py
--rw-rw-rw-   0        0        0     1394 2024-04-14 00:13:16.000000 pipez-0.0.93/pipez/nodes/common/ungroup.py
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:34.304970 pipez-0.0.93/pipez/nodes/cv/
--rw-rw-rw-   0        0        0       48 2024-04-13 20:32:11.000000 pipez-0.0.93/pipez/nodes/cv/__init__.py
--rw-rw-rw-   0        0        0     5238 2024-04-12 19:23:48.000000 pipez-0.0.93/pipez/nodes/cv/loop_video_reader.py
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:34.307415 pipez-0.0.93/pipez/nodes/nn/
--rw-rw-rw-   0        0        0        0 2024-01-23 07:32:10.000000 pipez-0.0.93/pipez/nodes/nn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:34.315147 pipez-0.0.93/pipez/nodes/nn/cv/
--rw-rw-rw-   0        0        0       87 2024-04-13 21:14:31.000000 pipez-0.0.93/pipez/nodes/nn/cv/__init__.py
--rw-rw-rw-   0        0        0     3132 2024-04-13 21:14:31.000000 pipez-0.0.93/pipez/nodes/nn/cv/async_ort.py
--rw-rw-rw-   0        0        0     2943 2024-04-13 21:47:01.000000 pipez-0.0.93/pipez/nodes/nn/cv/base.py
--rw-rw-rw-   0        0        0     2274 2024-04-13 21:14:31.000000 pipez-0.0.93/pipez/nodes/nn/cv/sync_ort.py
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:34.321474 pipez-0.0.93/pipez/nodes/ort/
--rw-rw-rw-   0        0        0       27 2024-04-13 21:48:22.000000 pipez-0.0.93/pipez/nodes/ort/__init__.py
--rw-rw-rw-   0        0        0     2338 2024-04-13 22:08:13.000000 pipez-0.0.93/pipez/nodes/ort/base.py
--rw-rw-rw-   0        0        0     1619 2024-04-13 22:09:07.000000 pipez-0.0.93/pipez/nodes/ort/sync.py
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:34.326015 pipez-0.0.93/pipez/nodes/web/
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:34.331989 pipez-0.0.93/pipez/nodes/web/SwaggerUI/
--rw-rw-rw-   0        0        0  1385226 2024-03-21 17:40:59.000000 pipez-0.0.93/pipez/nodes/web/SwaggerUI/swagger-ui-bundle.js
--rw-rw-rw-   0        0        0   151211 2024-03-21 17:41:04.000000 pipez-0.0.93/pipez/nodes/web/SwaggerUI/swagger-ui.css
--rw-rw-rw-   0        0        0       54 2024-03-18 11:04:58.000000 pipez-0.0.93/pipez/nodes/web/__init__.py
--rw-rw-rw-   0        0        0     2129 2024-04-13 20:36:54.000000 pipez-0.0.93/pipez/nodes/web/fastapi_node.py
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:34.336984 pipez-0.0.93/pipez/tools/
--rw-rw-rw-   0        0        0       36 2024-04-13 20:32:11.000000 pipez-0.0.93/pipez/tools/__init__.py
--rw-rw-rw-   0        0        0      574 2024-04-12 15:57:46.000000 pipez-0.0.93/pipez/tools/json2nodes.py
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:34.340516 pipez-0.0.93/pipez/utils/
--rw-rw-rw-   0        0        0       28 2024-04-13 20:32:11.000000 pipez-0.0.93/pipez/utils/__init__.py
--rw-rw-rw-   0        0        0      735 2024-03-12 07:18:26.000000 pipez-0.0.93/pipez/utils/resize.py
-drwxrwxrwx   0        0        0        0 2024-04-24 12:34:34.343999 pipez-0.0.93/pipez.egg-info/
--rw-rw-rw-   0        0        0     4041 2024-04-24 12:34:33.000000 pipez-0.0.93/pipez.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    12614 2024-04-24 12:34:33.000000 pipez-0.0.93/pipez.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 12:34:33.000000 pipez-0.0.93/pipez.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-04-24 12:34:33.000000 pipez-0.0.93/pipez.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-24 12:34:33.000000 pipez-0.0.93/pipez.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 12:34:34.347904 pipez-0.0.93/setup.cfg
--rw-rw-rw-   0        0        0      832 2024-04-13 21:41:28.000000 pipez-0.0.93/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.484279 pipez-0.0.94/
+-rw-rw-rw-   0        0        0    35823 2024-01-22 12:34:35.000000 pipez-0.0.94/LICENSE
+-rw-rw-rw-   0        0        0      126 2024-04-08 09:46:56.000000 pipez-0.0.94/MANIFEST.in
+-rw-rw-rw-   0        0        0     4041 2024-04-24 15:45:29.483332 pipez-0.0.94/PKG-INFO
+-rw-rw-rw-   0        0        0     3499 2024-04-13 20:09:12.000000 pipez-0.0.94/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.041711 pipez-0.0.94/pipez/
+-rw-rw-rw-   0        0        0       24 2024-04-24 15:45:01.000000 pipez-0.0.94/pipez/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.068808 pipez-0.0.94/pipez/core/
+-rw-rw-rw-   0        0        0      146 2024-04-13 20:09:12.000000 pipez-0.0.94/pipez/core/__init__.py
+-rw-rw-rw-   0        0        0     1247 2024-04-13 19:08:05.000000 pipez-0.0.94/pipez/core/batch.py
+-rw-rw-rw-   0        0        0      543 2024-04-13 15:27:35.000000 pipez-0.0.94/pipez/core/enums.py
+-rw-rw-rw-   0        0        0     2331 2024-02-04 10:03:20.000000 pipez-0.0.94/pipez/core/legacy_batch.py
+-rw-rw-rw-   0        0        0     2837 2024-04-13 16:03:09.000000 pipez-0.0.94/pipez/core/legacy_build.py
+-rw-rw-rw-   0        0        0     9549 2024-04-13 20:09:12.000000 pipez-0.0.94/pipez/core/legacy_node.py
+-rw-rw-rw-   0        0        0     1148 2024-04-12 14:59:21.000000 pipez-0.0.94/pipez/core/legacy_registry.py
+-rw-rw-rw-   0        0        0     2795 2024-02-02 11:31:56.000000 pipez-0.0.94/pipez/core/legacy_shared_memory.py
+-rw-rw-rw-   0        0        0     3713 2024-04-12 19:23:48.000000 pipez-0.0.94/pipez/core/legacy_watchdog.py
+-rw-rw-rw-   0        0        0      747 2024-04-12 15:57:46.000000 pipez-0.0.94/pipez/core/memory.py
+-rw-rw-rw-   0        0        0     1034 2024-04-24 11:55:20.000000 pipez-0.0.94/pipez/core/metrics.py
+-rw-rw-rw-   0        0        0     6023 2024-04-24 11:51:30.000000 pipez-0.0.94/pipez/core/node.py
+-rw-rw-rw-   0        0        0      850 2024-04-12 18:24:39.000000 pipez-0.0.94/pipez/core/queue_wrapper.py
+-rw-rw-rw-   0        0        0      577 2024-04-12 15:40:37.000000 pipez-0.0.94/pipez/core/registry.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.070176 pipez-0.0.94/pipez/core/static/
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.081453 pipez-0.0.94/pipez/core/static/DataTables/
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.022626 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.113978 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/
+-rw-rw-rw-   0        0        0    13174 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap.css
+-rw-rw-rw-   0        0        0    11219 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap.min.css
+-rw-rw-rw-   0        0        0    13511 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap4.css
+-rw-rw-rw-   0        0        0    11523 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap4.min.css
+-rw-rw-rw-   0        0        0    14198 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap5.css
+-rw-rw-rw-   0        0        0    12168 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap5.min.css
+-rw-rw-rw-   0        0        0    12157 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bulma.css
+-rw-rw-rw-   0        0        0    10395 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bulma.min.css
+-rw-rw-rw-   0        0        0        0 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.dataTables.css
+-rw-rw-rw-   0        0        0        0 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.dataTables.min.css
+-rw-rw-rw-   0        0        0    11266 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.foundation.css
+-rw-rw-rw-   0        0        0     9580 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.foundation.min.css
+-rw-rw-rw-   0        0        0    28554 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.jqueryui.css
+-rw-rw-rw-   0        0        0    24415 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.jqueryui.min.css
+-rw-rw-rw-   0        0        0    11471 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.semanticui.css
+-rw-rw-rw-   0        0        0     9783 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.semanticui.min.css
+-rw-rw-rw-   0        0        0    26541 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/jquery.dataTables.css
+-rw-rw-rw-   0        0        0    22712 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/jquery.dataTables.min.css
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.123652 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/images/
+-rw-rw-rw-   0        0        0      160 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/images/sort_asc.png
+-rw-rw-rw-   0        0        0      148 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/images/sort_asc_disabled.png
+-rw-rw-rw-   0        0        0      201 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/images/sort_both.png
+-rw-rw-rw-   0        0        0      158 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/images/sort_desc.png
+-rw-rw-rw-   0        0        0      146 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/images/sort_desc_disabled.png
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.172078 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/
+-rw-rw-rw-   0        0        0     5214 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap.js
+-rw-rw-rw-   0        0        0     2226 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap.min.js
+-rw-rw-rw-   0        0        0     5350 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap4.js
+-rw-rw-rw-   0        0        0     2343 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap4.min.js
+-rw-rw-rw-   0        0        0     5494 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap5.js
+-rw-rw-rw-   0        0        0     2361 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap5.min.js
+-rw-rw-rw-   0        0        0     5701 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bulma.js
+-rw-rw-rw-   0        0        0     2484 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bulma.min.js
+-rw-rw-rw-   0        0        0     1205 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.dataTables.js
+-rw-rw-rw-   0        0        0      588 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.dataTables.min.js
+-rw-rw-rw-   0        0        0     5235 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.foundation.js
+-rw-rw-rw-   0        0        0     2398 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.foundation.min.js
+-rw-rw-rw-   0        0        0     2518 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.jqueryui.js
+-rw-rw-rw-   0        0        0     1226 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.jqueryui.min.js
+-rw-rw-rw-   0        0        0     5923 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.semanticui.js
+-rw-rw-rw-   0        0        0     2672 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.semanticui.min.js
+-rw-rw-rw-   0        0        0   473441 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/jquery.dataTables.js
+-rw-rw-rw-   0        0        0    87279 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/jquery.dataTables.min.js
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.024678 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.201479 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/
+-rw-rw-rw-   0        0        0     1316 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap.css
+-rw-rw-rw-   0        0        0     1124 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap.min.css
+-rw-rw-rw-   0        0        0     1339 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap4.css
+-rw-rw-rw-   0        0        0     1147 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap4.min.css
+-rw-rw-rw-   0        0        0     1452 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap5.css
+-rw-rw-rw-   0        0        0     1247 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap5.min.css
+-rw-rw-rw-   0        0        0     1263 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bulma.css
+-rw-rw-rw-   0        0        0     1084 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bulma.min.css
+-rw-rw-rw-   0        0        0     1263 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.dataTables.css
+-rw-rw-rw-   0        0        0     1084 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.dataTables.min.css
+-rw-rw-rw-   0        0        0      396 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.foundation.css
+-rw-rw-rw-   0        0        0      339 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.foundation.min.css
+-rw-rw-rw-   0        0        0     1263 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.jqueryui.css
+-rw-rw-rw-   0        0        0     1084 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.jqueryui.min.css
+-rw-rw-rw-   0        0        0     1263 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.semanticui.css
+-rw-rw-rw-   0        0        0     1084 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.semanticui.min.css
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.260422 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/
+-rw-rw-rw-   0        0        0    41008 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/dataTables.scroller.js
+-rw-rw-rw-   0        0        0    12430 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/dataTables.scroller.min.js
+-rw-rw-rw-   0        0        0     1339 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap.js
+-rw-rw-rw-   0        0        0      691 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap.min.js
+-rw-rw-rw-   0        0        0     1341 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap4.js
+-rw-rw-rw-   0        0        0      693 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap4.min.js
+-rw-rw-rw-   0        0        0     1341 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap5.js
+-rw-rw-rw-   0        0        0      693 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap5.min.js
+-rw-rw-rw-   0        0        0     1333 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bulma.js
+-rw-rw-rw-   0        0        0      685 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bulma.min.js
+-rw-rw-rw-   0        0        0     1338 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.dataTables.js
+-rw-rw-rw-   0        0        0      690 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.dataTables.min.js
+-rw-rw-rw-   0        0        0     1338 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.foundation.js
+-rw-rw-rw-   0        0        0      690 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.foundation.min.js
+-rw-rw-rw-   0        0        0     1341 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.jqueryui.js
+-rw-rw-rw-   0        0        0      693 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.jqueryui.min.js
+-rw-rw-rw-   0        0        0     1338 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.semanticui.js
+-rw-rw-rw-   0        0        0      690 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.semanticui.min.js
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.025654 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.307594 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/
+-rw-rw-rw-   0        0        0     6724 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap.css
+-rw-rw-rw-   0        0        0     5854 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap.min.css
+-rw-rw-rw-   0        0        0     6981 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap4.css
+-rw-rw-rw-   0        0        0     6077 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap4.min.css
+-rw-rw-rw-   0        0        0     7186 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap5.css
+-rw-rw-rw-   0        0        0     6249 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap5.min.css
+-rw-rw-rw-   0        0        0     7015 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bulma.css
+-rw-rw-rw-   0        0        0     6100 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bulma.min.css
+-rw-rw-rw-   0        0        0     8908 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.dataTables.css
+-rw-rw-rw-   0        0        0     7734 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.dataTables.min.css
+-rw-rw-rw-   0        0        0     7184 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.foundation.css
+-rw-rw-rw-   0        0        0     6254 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.foundation.min.css
+-rw-rw-rw-   0        0        0     6733 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.jqueryui.css
+-rw-rw-rw-   0        0        0     5869 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.jqueryui.min.css
+-rw-rw-rw-   0        0        0     8090 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.semanticui.css
+-rw-rw-rw-   0        0        0     7041 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.semanticui.min.css
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.349115 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/
+-rw-rw-rw-   0        0        0   179224 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/dataTables.searchBuilder.js
+-rw-rw-rw-   0        0        0    67309 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/dataTables.searchBuilder.min.js
+-rw-rw-rw-   0        0        0     1950 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap.js
+-rw-rw-rw-   0        0        0     1190 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap.min.js
+-rw-rw-rw-   0        0        0     1941 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap4.js
+-rw-rw-rw-   0        0        0     1181 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap4.min.js
+-rw-rw-rw-   0        0        0     2021 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap5.js
+-rw-rw-rw-   0        0        0     1247 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap5.min.js
+-rw-rw-rw-   0        0        0     1812 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bulma.js
+-rw-rw-rw-   0        0        0     1066 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bulma.min.js
+-rw-rw-rw-   0        0        0     1366 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.dataTables.js
+-rw-rw-rw-   0        0        0      718 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.dataTables.min.js
+-rw-rw-rw-   0        0        0     1901 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.foundation.js
+-rw-rw-rw-   0        0        0     1141 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.foundation.min.js
+-rw-rw-rw-   0        0        0     2291 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.jqueryui.js
+-rw-rw-rw-   0        0        0     1531 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.jqueryui.min.js
+-rw-rw-rw-   0        0        0     2527 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.semanticui.js
+-rw-rw-rw-   0        0        0     1550 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.semanticui.min.js
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.028275 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.376831 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/
+-rw-rw-rw-   0        0        0    12192 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap.css
+-rw-rw-rw-   0        0        0    10844 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap.min.css
+-rw-rw-rw-   0        0        0    12489 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap4.css
+-rw-rw-rw-   0        0        0    11153 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap4.min.css
+-rw-rw-rw-   0        0        0    15085 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap5.css
+-rw-rw-rw-   0        0        0    13537 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap5.min.css
+-rw-rw-rw-   0        0        0    12232 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bulma.css
+-rw-rw-rw-   0        0        0    10955 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bulma.min.css
+-rw-rw-rw-   0        0        0    14718 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.dataTables.css
+-rw-rw-rw-   0        0        0    13089 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.dataTables.min.css
+-rw-rw-rw-   0        0        0    12527 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.foundation.css
+-rw-rw-rw-   0        0        0    11137 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.foundation.min.css
+-rw-rw-rw-   0        0        0    15420 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.jqueryui.css
+-rw-rw-rw-   0        0        0    13689 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.jqueryui.min.css
+-rw-rw-rw-   0        0        0    14238 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.semanticui.css
+-rw-rw-rw-   0        0        0    12644 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.semanticui.min.css
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.417145 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/
+-rw-rw-rw-   0        0        0   167377 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/dataTables.searchPanes.js
+-rw-rw-rw-   0        0        0    56665 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/dataTables.searchPanes.min.js
+-rw-rw-rw-   0        0        0     2183 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap.js
+-rw-rw-rw-   0        0        0     1360 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap.min.js
+-rw-rw-rw-   0        0        0     2295 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap4.js
+-rw-rw-rw-   0        0        0     1444 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap4.min.js
+-rw-rw-rw-   0        0        0     2159 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap5.js
+-rw-rw-rw-   0        0        0     1336 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap5.min.js
+-rw-rw-rw-   0        0        0     1782 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bulma.js
+-rw-rw-rw-   0        0        0     1046 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bulma.min.js
+-rw-rw-rw-   0        0        0     1357 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.dataTables.js
+-rw-rw-rw-   0        0        0      709 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.dataTables.min.js
+-rw-rw-rw-   0        0        0     2117 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.foundation.js
+-rw-rw-rw-   0        0        0     1311 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.foundation.min.js
+-rw-rw-rw-   0        0        0     1862 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.jqueryui.js
+-rw-rw-rw-   0        0        0     1134 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.jqueryui.min.js
+-rw-rw-rw-   0        0        0     2152 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.semanticui.js
+-rw-rw-rw-   0        0        0     1301 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.semanticui.min.js
+-rw-rw-rw-   0        0        0    38379 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/datatables.css
+-rw-rw-rw-   0        0        0  1166936 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/datatables.js
+-rw-rw-rw-   0        0        0    33659 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/datatables.min.css
+-rw-rw-rw-   0        0        0   316604 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/datatables.min.js
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.422142 pipez-0.0.94/pipez/core/static/DataTables/jQuery-3.7.0/
+-rw-rw-rw-   0        0        0   295700 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/jQuery-3.7.0/jquery-3.7.0.js
+-rw-rw-rw-   0        0        0    87464 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/static/DataTables/jQuery-3.7.0/jquery-3.7.0.min.js
+-rw-rw-rw-   0        0        0        0 2024-02-13 14:55:57.000000 pipez-0.0.94/pipez/core/static/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.425669 pipez-0.0.94/pipez/core/templates/
+-rw-rw-rw-   0        0        0        0 2024-02-02 08:26:03.000000 pipez-0.0.94/pipez/core/templates/__init__.py
+-rw-rw-rw-   0        0        0     4968 2024-02-05 15:51:59.000000 pipez-0.0.94/pipez/core/templates/home.html
+-rw-rw-rw-   0        0        0     4251 2024-04-24 15:45:01.000000 pipez-0.0.94/pipez/core/watchdog.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.427670 pipez-0.0.94/pipez/nodes/
+-rw-rw-rw-   0        0        0        0 2024-03-21 18:00:34.000000 pipez-0.0.94/pipez/nodes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.432514 pipez-0.0.94/pipez/nodes/common/
+-rw-rw-rw-   0        0        0       56 2024-04-13 18:05:30.000000 pipez-0.0.94/pipez/nodes/common/__init__.py
+-rw-rw-rw-   0        0        0      749 2024-04-14 00:13:16.000000 pipez-0.0.94/pipez/nodes/common/group.py
+-rw-rw-rw-   0        0        0     1394 2024-04-14 00:13:16.000000 pipez-0.0.94/pipez/nodes/common/ungroup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.436914 pipez-0.0.94/pipez/nodes/cv/
+-rw-rw-rw-   0        0        0       48 2024-04-13 20:32:11.000000 pipez-0.0.94/pipez/nodes/cv/__init__.py
+-rw-rw-rw-   0        0        0     5238 2024-04-12 19:23:48.000000 pipez-0.0.94/pipez/nodes/cv/loop_video_reader.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.437925 pipez-0.0.94/pipez/nodes/nn/
+-rw-rw-rw-   0        0        0        0 2024-01-23 07:32:10.000000 pipez-0.0.94/pipez/nodes/nn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.446034 pipez-0.0.94/pipez/nodes/nn/cv/
+-rw-rw-rw-   0        0        0       87 2024-04-13 21:14:31.000000 pipez-0.0.94/pipez/nodes/nn/cv/__init__.py
+-rw-rw-rw-   0        0        0     3132 2024-04-13 21:14:31.000000 pipez-0.0.94/pipez/nodes/nn/cv/async_ort.py
+-rw-rw-rw-   0        0        0     2943 2024-04-13 21:47:01.000000 pipez-0.0.94/pipez/nodes/nn/cv/base.py
+-rw-rw-rw-   0        0        0     2274 2024-04-13 21:14:31.000000 pipez-0.0.94/pipez/nodes/nn/cv/sync_ort.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.453930 pipez-0.0.94/pipez/nodes/ort/
+-rw-rw-rw-   0        0        0       27 2024-04-13 21:48:22.000000 pipez-0.0.94/pipez/nodes/ort/__init__.py
+-rw-rw-rw-   0        0        0     2338 2024-04-13 22:08:13.000000 pipez-0.0.94/pipez/nodes/ort/base.py
+-rw-rw-rw-   0        0        0     1619 2024-04-13 22:09:07.000000 pipez-0.0.94/pipez/nodes/ort/sync.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.457426 pipez-0.0.94/pipez/nodes/web/
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.466698 pipez-0.0.94/pipez/nodes/web/SwaggerUI/
+-rw-rw-rw-   0        0        0  1385226 2024-03-21 17:40:59.000000 pipez-0.0.94/pipez/nodes/web/SwaggerUI/swagger-ui-bundle.js
+-rw-rw-rw-   0        0        0   151211 2024-03-21 17:41:04.000000 pipez-0.0.94/pipez/nodes/web/SwaggerUI/swagger-ui.css
+-rw-rw-rw-   0        0        0       54 2024-03-18 11:04:58.000000 pipez-0.0.94/pipez/nodes/web/__init__.py
+-rw-rw-rw-   0        0        0     2129 2024-04-13 20:36:54.000000 pipez-0.0.94/pipez/nodes/web/fastapi_node.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.473576 pipez-0.0.94/pipez/tools/
+-rw-rw-rw-   0        0        0       36 2024-04-13 20:32:11.000000 pipez-0.0.94/pipez/tools/__init__.py
+-rw-rw-rw-   0        0        0      574 2024-04-12 15:57:46.000000 pipez-0.0.94/pipez/tools/json2nodes.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.477905 pipez-0.0.94/pipez/utils/
+-rw-rw-rw-   0        0        0       28 2024-04-13 20:32:11.000000 pipez-0.0.94/pipez/utils/__init__.py
+-rw-rw-rw-   0        0        0      735 2024-03-12 07:18:26.000000 pipez-0.0.94/pipez/utils/resize.py
+drwxrwxrwx   0        0        0        0 2024-04-24 15:45:29.480303 pipez-0.0.94/pipez.egg-info/
+-rw-rw-rw-   0        0        0     4041 2024-04-24 15:45:28.000000 pipez-0.0.94/pipez.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    12614 2024-04-24 15:45:29.000000 pipez-0.0.94/pipez.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 15:45:28.000000 pipez-0.0.94/pipez.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-04-24 15:45:28.000000 pipez-0.0.94/pipez.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-24 15:45:28.000000 pipez-0.0.94/pipez.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 15:45:29.484279 pipez-0.0.94/setup.cfg
+-rw-rw-rw-   0        0        0      832 2024-04-13 21:41:28.000000 pipez-0.0.94/setup.py
```

### Comparing `pipez-0.0.93/LICENSE` & `pipez-0.0.94/LICENSE`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/PKG-INFO` & `pipez-0.0.94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipez
-Version: 0.0.93
+Version: 0.0.94
 Home-page: https://github.com/tam2511/pipez
 Author: Alexander Timofeev
 Author-email: tam2511@mail.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `pipez-0.0.93/README.md` & `pipez-0.0.94/README.md`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/batch.py` & `pipez-0.0.94/pipez/core/batch.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/enums.py` & `pipez-0.0.94/pipez/core/enums.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/legacy_batch.py` & `pipez-0.0.94/pipez/core/legacy_batch.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/legacy_build.py` & `pipez-0.0.94/pipez/core/legacy_build.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/legacy_node.py` & `pipez-0.0.94/pipez/core/legacy_node.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/legacy_registry.py` & `pipez-0.0.94/pipez/core/legacy_registry.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/legacy_shared_memory.py` & `pipez-0.0.94/pipez/core/legacy_shared_memory.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/legacy_watchdog.py` & `pipez-0.0.94/pipez/core/legacy_watchdog.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/memory.py` & `pipez-0.0.94/pipez/core/memory.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/metrics.py` & `pipez-0.0.94/pipez/core/metrics.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/node.py` & `pipez-0.0.94/pipez/core/node.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/queue_wrapper.py` & `pipez-0.0.94/pipez/core/queue_wrapper.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/registry.py` & `pipez-0.0.94/pipez/core/registry.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap.css` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap4.css` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap4.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap4.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap4.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap5.css` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap5.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap5.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bootstrap5.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bulma.css` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bulma.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bulma.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.bulma.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.foundation.css` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.foundation.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.foundation.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.foundation.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.jqueryui.css` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.jqueryui.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.jqueryui.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.jqueryui.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.semanticui.css` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.semanticui.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.semanticui.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/dataTables.semanticui.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/jquery.dataTables.css` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/jquery.dataTables.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/css/jquery.dataTables.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/css/jquery.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap.js` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap4.js` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap4.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap4.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap4.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap5.js` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap5.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap5.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bootstrap5.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bulma.js` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bulma.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bulma.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.bulma.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.dataTables.js` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.dataTables.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.dataTables.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.foundation.js` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.foundation.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.foundation.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.foundation.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.jqueryui.js` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.jqueryui.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.jqueryui.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.jqueryui.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.semanticui.js` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.semanticui.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.semanticui.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/dataTables.semanticui.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/jquery.dataTables.js` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/jquery.dataTables.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/DataTables-1.13.8/js/jquery.dataTables.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/DataTables-1.13.8/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap.css` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap4.css` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap4.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap4.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap4.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap5.css` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap5.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap5.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bootstrap5.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bulma.css` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bulma.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bulma.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.bulma.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.dataTables.css` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.dataTables.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.dataTables.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.jqueryui.css` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.jqueryui.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.jqueryui.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.jqueryui.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.semanticui.css` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.semanticui.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.semanticui.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/css/scroller.semanticui.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/dataTables.scroller.js` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/dataTables.scroller.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/dataTables.scroller.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/dataTables.scroller.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap.js` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap4.js` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap4.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap4.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap4.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap5.js` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap5.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap5.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bootstrap5.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bulma.js` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bulma.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bulma.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.bulma.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.dataTables.js` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.dataTables.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.dataTables.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.foundation.js` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.foundation.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.foundation.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.foundation.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.jqueryui.js` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.jqueryui.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.jqueryui.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.jqueryui.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.semanticui.js` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.semanticui.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.semanticui.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/Scroller-2.3.0/js/scroller.semanticui.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap4.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap4.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap4.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap4.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap5.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap5.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap5.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bootstrap5.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bulma.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bulma.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bulma.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.bulma.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.dataTables.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.dataTables.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.dataTables.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.foundation.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.foundation.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.foundation.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.foundation.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.jqueryui.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.jqueryui.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.jqueryui.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.jqueryui.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.semanticui.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.semanticui.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.semanticui.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/css/searchBuilder.semanticui.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/dataTables.searchBuilder.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/dataTables.searchBuilder.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/dataTables.searchBuilder.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/dataTables.searchBuilder.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap4.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap4.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap4.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap4.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap5.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap5.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap5.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bootstrap5.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bulma.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bulma.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bulma.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.bulma.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.dataTables.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.dataTables.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.dataTables.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.foundation.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.foundation.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.foundation.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.foundation.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.jqueryui.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.jqueryui.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.jqueryui.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.jqueryui.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.semanticui.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.semanticui.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.semanticui.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchBuilder-1.6.0/js/searchBuilder.semanticui.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap4.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap4.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap4.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap4.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap5.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap5.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap5.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bootstrap5.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bulma.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bulma.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bulma.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.bulma.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.dataTables.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.dataTables.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.dataTables.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.foundation.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.foundation.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.foundation.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.foundation.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.jqueryui.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.jqueryui.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.jqueryui.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.jqueryui.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.semanticui.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.semanticui.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.semanticui.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/css/searchPanes.semanticui.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/dataTables.searchPanes.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/dataTables.searchPanes.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/dataTables.searchPanes.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/dataTables.searchPanes.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap4.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap4.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap4.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap4.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap5.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap5.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap5.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bootstrap5.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bulma.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bulma.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bulma.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.bulma.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.dataTables.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.dataTables.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.dataTables.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.foundation.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.foundation.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.foundation.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.foundation.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.jqueryui.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.jqueryui.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.jqueryui.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.jqueryui.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.semanticui.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.semanticui.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.semanticui.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/SearchPanes-2.2.0/js/searchPanes.semanticui.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/datatables.css` & `pipez-0.0.94/pipez/core/static/DataTables/datatables.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/datatables.js` & `pipez-0.0.94/pipez/core/static/DataTables/datatables.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/datatables.min.css` & `pipez-0.0.94/pipez/core/static/DataTables/datatables.min.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/datatables.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/datatables.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/jQuery-3.7.0/jquery-3.7.0.js` & `pipez-0.0.94/pipez/core/static/DataTables/jQuery-3.7.0/jquery-3.7.0.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/static/DataTables/jQuery-3.7.0/jquery-3.7.0.min.js` & `pipez-0.0.94/pipez/core/static/DataTables/jQuery-3.7.0/jquery-3.7.0.min.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/templates/home.html` & `pipez-0.0.94/pipez/core/templates/home.html`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/core/watchdog.py` & `pipez-0.0.94/pipez/core/watchdog.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,23 +30,23 @@
         self._build_pipeline()
 
         if verbose_metrics:
             self._request = Request
             self._templates = Jinja2Templates(directory=os.path.join(os.path.dirname(os.path.abspath(__file__)), 'templates'))
 
             app = FastAPI()
-            app.mount(path='/static',
-                      app=StaticFiles(directory=os.path.join(os.path.dirname(os.path.abspath(__file__)), 'static'), html=True),
-                      name='static')
-
-            router = APIRouter()
-            router.add_api_route(path='/metrics', endpoint=self._print_metrics, methods=['GET'], response_class=HTMLResponse)
-            router.add_api_route(path='/metrics_api', endpoint=self._print_metrics_api, methods=['GET'])
-
-            app.include_router(router)
+            # app.mount(path='/static',
+            #           app=StaticFiles(directory=os.path.join(os.path.dirname(os.path.abspath(__file__)), 'static'), html=True),
+            #           name='static')
+            #
+            # router = APIRouter()
+            # router.add_api_route(path='/metrics', endpoint=self._print_metrics, methods=['GET'], response_class=HTMLResponse)
+            # router.add_api_route(path='/metrics_api', endpoint=self._print_metrics_api, methods=['GET'])
+            #
+            # app.include_router(router)
             uvicorn.run(app, host=metrics_host, port=metrics_port)
 
         self.start()
 
     def _print_metrics(self, request: Request):
         return self._templates.TemplateResponse('home.html', dict(request=request))
```

### Comparing `pipez-0.0.93/pipez/nodes/common/group.py` & `pipez-0.0.94/pipez/nodes/common/group.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/nodes/common/ungroup.py` & `pipez-0.0.94/pipez/nodes/common/ungroup.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/nodes/cv/loop_video_reader.py` & `pipez-0.0.94/pipez/nodes/cv/loop_video_reader.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/nodes/nn/cv/async_ort.py` & `pipez-0.0.94/pipez/nodes/nn/cv/async_ort.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/nodes/nn/cv/base.py` & `pipez-0.0.94/pipez/nodes/nn/cv/base.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/nodes/nn/cv/sync_ort.py` & `pipez-0.0.94/pipez/nodes/nn/cv/sync_ort.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/nodes/ort/base.py` & `pipez-0.0.94/pipez/nodes/ort/base.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/nodes/ort/sync.py` & `pipez-0.0.94/pipez/nodes/ort/sync.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/nodes/web/SwaggerUI/swagger-ui-bundle.js` & `pipez-0.0.94/pipez/nodes/web/SwaggerUI/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/nodes/web/SwaggerUI/swagger-ui.css` & `pipez-0.0.94/pipez/nodes/web/SwaggerUI/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/nodes/web/fastapi_node.py` & `pipez-0.0.94/pipez/nodes/web/fastapi_node.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/tools/json2nodes.py` & `pipez-0.0.94/pipez/tools/json2nodes.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez/utils/resize.py` & `pipez-0.0.94/pipez/utils/resize.py`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/pipez.egg-info/PKG-INFO` & `pipez-0.0.94/pipez.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipez
-Version: 0.0.93
+Version: 0.0.94
 Home-page: https://github.com/tam2511/pipez
 Author: Alexander Timofeev
 Author-email: tam2511@mail.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `pipez-0.0.93/pipez.egg-info/SOURCES.txt` & `pipez-0.0.94/pipez.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pipez-0.0.93/setup.py` & `pipez-0.0.94/setup.py`

 * *Files identical despite different names*

