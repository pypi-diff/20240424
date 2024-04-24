# Comparing `tmp/codeflex-3.1.1.tar.gz` & `tmp/codeflex-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeflex-3.1.1.tar", last modified: Mon Apr 22 14:49:24 2024, max compression
+gzip compressed data, was "codeflex-4.0.0.tar", last modified: Wed Apr 24 13:52:36 2024, max compression
```

## Comparing `codeflex-3.1.1.tar` & `codeflex-4.0.0.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 14:49:24.916438 codeflex-3.1.1/
--rw-rw-rw-   0        0        0     1913 2024-04-18 01:41:25.000000 codeflex-3.1.1/LICENSE
--rw-rw-rw-   0        0        0     6241 2024-04-22 14:49:24.916438 codeflex-3.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5364 2024-04-22 14:48:42.000000 codeflex-3.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-22 14:49:24.916438 codeflex-3.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1043 2024-04-22 14:48:45.000000 codeflex-3.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 14:49:24.627986 codeflex-3.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-22 14:49:24.659228 codeflex-3.1.1/src/codeflex/
--rw-rw-rw-   0        0        0        0 2024-04-17 23:25:20.000000 codeflex-3.1.1/src/codeflex/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 14:49:24.706092 codeflex-3.1.1/src/codeflex/company/
--rw-rw-rw-   0        0        0        0 2024-04-17 23:25:20.000000 codeflex-3.1.1/src/codeflex/company/__init__.py
--rw-rw-rw-   0        0        0     6298 2024-04-22 14:45:41.000000 codeflex-3.1.1/src/codeflex/company/mysql.py
--rw-rw-rw-   0        0        0     1233 2024-04-22 14:43:29.000000 codeflex-3.1.1/src/codeflex/company/polly.py
-drwxrwxrwx   0        0        0        0 2024-04-22 14:49:24.768582 codeflex-3.1.1/src/codeflex/server/
--rw-rw-rw-   0        0        0     2621 2024-04-21 22:48:54.000000 codeflex-3.1.1/src/codeflex/server/__init__.py
--rw-rw-rw-   0        0        0       30 2024-02-14 20:44:10.000000 codeflex-3.1.1/src/codeflex/server/__main__.py
--rw-rw-rw-   0        0        0    59700 2024-04-21 22:43:12.000000 codeflex-3.1.1/src/codeflex/server/app.py
--rw-rw-rw-   0        0        0     3156 2024-04-21 22:18:03.000000 codeflex-3.1.1/src/codeflex/server/blueprints.py
-drwxrwxrwx   0        0        0        0 2024-04-22 14:49:24.768582 codeflex-3.1.1/src/codeflex/server/cero/
--rw-rw-rw-   0        0        0        0 2024-04-17 23:25:20.000000 codeflex-3.1.1/src/codeflex/server/cero/__init__.py
--rw-rw-rw-   0        0        0    38209 2024-02-14 20:44:10.000000 codeflex-3.1.1/src/codeflex/server/cero/app.py
--rw-rw-rw-   0        0        0    24637 2024-02-14 20:44:10.000000 codeflex-3.1.1/src/codeflex/server/cero/blueprints.py
--rw-rw-rw-   0        0        0    30879 2024-02-14 20:44:10.000000 codeflex-3.1.1/src/codeflex/server/cero/scaffold.py
--rw-rw-rw-   0        0        0    35797 2024-04-21 22:48:00.000000 codeflex-3.1.1/src/codeflex/server/cli.py
--rw-rw-rw-   0        0        0    13326 2024-04-21 22:18:04.000000 codeflex-3.1.1/src/codeflex/server/config.py
--rw-rw-rw-   0        0        0    15114 2024-04-21 22:46:10.000000 codeflex-3.1.1/src/codeflex/server/ctx.py
--rw-rw-rw-   0        0        0     6076 2024-04-21 22:18:05.000000 codeflex-3.1.1/src/codeflex/server/debughelpers.py
--rw-rw-rw-   0        0        0     1709 2024-04-21 22:45:40.000000 codeflex-3.1.1/src/codeflex/server/globals.py
--rw-rw-rw-   0        0        0    23084 2024-02-14 20:44:10.000000 codeflex-3.1.1/src/codeflex/server/helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-22 14:49:24.791463 codeflex-3.1.1/src/codeflex/server/json/
--rw-rw-rw-   0        0        0     5602 2024-02-14 20:44:10.000000 codeflex-3.1.1/src/codeflex/server/json/__init__.py
--rw-rw-rw-   0        0        0     7646 2024-02-14 20:44:10.000000 codeflex-3.1.1/src/codeflex/server/json/provider.py
--rw-rw-rw-   0        0        0     9280 2024-02-14 20:44:10.000000 codeflex-3.1.1/src/codeflex/server/json/tag.py
--rw-rw-rw-   0        0        0     2375 2024-04-21 22:18:07.000000 codeflex-3.1.1/src/codeflex/server/logging.py
--rw-rw-rw-   0        0        0        0 2024-02-14 20:44:10.000000 codeflex-3.1.1/src/codeflex/server/py.typed
--rw-rw-rw-   0        0        0    14488 2024-04-21 22:45:08.000000 codeflex-3.1.1/src/codeflex/server/sessions.py
--rw-rw-rw-   0        0        0      750 2024-02-14 20:44:10.000000 codeflex-3.1.1/src/codeflex/server/signals.py
--rw-rw-rw-   0        0        0     7527 2024-04-21 22:44:16.000000 codeflex-3.1.1/src/codeflex/server/templating.py
--rw-rw-rw-   0        0        0    10157 2024-04-21 22:44:02.000000 codeflex-3.1.1/src/codeflex/server/testing.py
--rw-rw-rw-   0        0        0     3190 2024-02-14 20:44:10.000000 codeflex-3.1.1/src/codeflex/server/typing.py
--rw-rw-rw-   0        0        0     6939 2024-02-14 20:44:10.000000 codeflex-3.1.1/src/codeflex/server/views.py
--rw-rw-rw-   0        0        0     5831 2024-02-14 20:44:10.000000 codeflex-3.1.1/src/codeflex/server/wrappers.py
-drwxrwxrwx   0        0        0        0 2024-04-22 14:49:24.791463 codeflex-3.1.1/src/codeflex/url/
--rw-rw-rw-   0        0        0        0 2024-04-17 23:25:20.000000 codeflex-3.1.1/src/codeflex/url/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 14:49:24.900818 codeflex-3.1.1/src/codeflex/url/connect/
--rw-rw-rw-   0        0        0     4963 2024-02-14 20:45:27.000000 codeflex-3.1.1/src/codeflex/url/connect/__init__.py
--rw-rw-rw-   0        0        0      435 2024-02-14 20:45:27.000000 codeflex-3.1.1/src/codeflex/url/connect/__version__.py
--rw-rw-rw-   0        0        0     1495 2024-02-14 20:45:27.000000 codeflex-3.1.1/src/codeflex/url/connect/_internal_utils.py
--rw-rw-rw-   0        0        0    19553 2024-02-14 20:45:27.000000 codeflex-3.1.1/src/codeflex/url/connect/adapters.py
--rw-rw-rw-   0        0        0     6449 2024-02-14 20:45:27.000000 codeflex-3.1.1/src/codeflex/url/connect/api.py
--rw-rw-rw-   0        0        0    10187 2024-02-14 20:45:27.000000 codeflex-3.1.1/src/codeflex/url/connect/auth.py
--rw-rw-rw-   0        0        0      429 2024-02-14 20:45:27.000000 codeflex-3.1.1/src/codeflex/url/connect/certs.py
--rw-rw-rw-   0        0        0     1451 2024-02-14 20:45:27.000000 codeflex-3.1.1/src/codeflex/url/connect/compat.py
--rw-rw-rw-   0        0        0    18560 2024-02-14 20:45:27.000000 codeflex-3.1.1/src/codeflex/url/connect/cookies.py
--rw-rw-rw-   0        0        0     3811 2024-02-14 20:45:27.000000 codeflex-3.1.1/src/codeflex/url/connect/exceptions.py
--rw-rw-rw-   0        0        0     3875 2024-02-14 20:45:27.000000 codeflex-3.1.1/src/codeflex/url/connect/help.py
--rw-rw-rw-   0        0        0      733 2024-02-14 20:45:27.000000 codeflex-3.1.1/src/codeflex/url/connect/hooks.py
--rw-rw-rw-   0        0        0    35223 2024-02-14 20:45:27.000000 codeflex-3.1.1/src/codeflex/url/connect/models.py
--rw-rw-rw-   0        0        0      957 2024-02-14 20:45:27.000000 codeflex-3.1.1/src/codeflex/url/connect/packages.py
--rw-rw-rw-   0        0        0    30373 2024-02-14 20:45:27.000000 codeflex-3.1.1/src/codeflex/url/connect/sessions.py
--rw-rw-rw-   0        0        0     4235 2024-02-14 20:45:27.000000 codeflex-3.1.1/src/codeflex/url/connect/status_codes.py
--rw-rw-rw-   0        0        0     2912 2024-02-14 20:45:27.000000 codeflex-3.1.1/src/codeflex/url/connect/structures.py
--rw-rw-rw-   0        0        0    33448 2024-02-14 20:45:27.000000 codeflex-3.1.1/src/codeflex/url/connect/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-22 14:49:24.900818 codeflex-3.1.1/src/codeflex.egg-info/
--rw-rw-rw-   0        0        0     6241 2024-04-22 14:49:24.000000 codeflex-3.1.1/src/codeflex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1811 2024-04-22 14:49:24.000000 codeflex-3.1.1/src/codeflex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 14:49:24.000000 codeflex-3.1.1/src/codeflex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-22 14:49:24.000000 codeflex-3.1.1/src/codeflex.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 13:52:36.278401 codeflex-4.0.0/
+-rw-rw-rw-   0        0        0     1913 2024-04-18 01:41:25.000000 codeflex-4.0.0/LICENSE
+-rw-rw-rw-   0        0        0     6492 2024-04-24 13:52:36.278401 codeflex-4.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5364 2024-04-22 14:48:42.000000 codeflex-4.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 13:52:36.278401 codeflex-4.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1286 2024-04-24 13:51:21.000000 codeflex-4.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:52:34.421529 codeflex-4.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-24 13:52:34.477925 codeflex-4.0.0/src/codeflex/
+-rw-rw-rw-   0        0        0        0 2024-04-17 23:25:20.000000 codeflex-4.0.0/src/codeflex/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:52:34.736585 codeflex-4.0.0/src/codeflex/company/
+-rw-rw-rw-   0        0        0        0 2024-04-17 23:25:20.000000 codeflex-4.0.0/src/codeflex/company/__init__.py
+-rw-rw-rw-   0        0        0     6298 2024-04-22 14:45:41.000000 codeflex-4.0.0/src/codeflex/company/mysql.py
+-rw-rw-rw-   0        0        0     1233 2024-04-22 14:43:29.000000 codeflex-4.0.0/src/codeflex/company/polly.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:52:35.553038 codeflex-4.0.0/src/codeflex/server/
+-rw-rw-rw-   0        0        0     2621 2024-04-21 22:48:54.000000 codeflex-4.0.0/src/codeflex/server/__init__.py
+-rw-rw-rw-   0        0        0       30 2024-02-14 20:44:10.000000 codeflex-4.0.0/src/codeflex/server/__main__.py
+-rw-rw-rw-   0        0        0    59700 2024-04-21 22:43:12.000000 codeflex-4.0.0/src/codeflex/server/app.py
+-rw-rw-rw-   0        0        0     3156 2024-04-21 22:18:03.000000 codeflex-4.0.0/src/codeflex/server/blueprints.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:52:35.678605 codeflex-4.0.0/src/codeflex/server/cero/
+-rw-rw-rw-   0        0        0        0 2024-04-17 23:25:20.000000 codeflex-4.0.0/src/codeflex/server/cero/__init__.py
+-rw-rw-rw-   0        0        0    38209 2024-02-14 20:44:10.000000 codeflex-4.0.0/src/codeflex/server/cero/app.py
+-rw-rw-rw-   0        0        0    24637 2024-02-14 20:44:10.000000 codeflex-4.0.0/src/codeflex/server/cero/blueprints.py
+-rw-rw-rw-   0        0        0    30879 2024-02-14 20:44:10.000000 codeflex-4.0.0/src/codeflex/server/cero/scaffold.py
+-rw-rw-rw-   0        0        0    35797 2024-04-21 22:48:00.000000 codeflex-4.0.0/src/codeflex/server/cli.py
+-rw-rw-rw-   0        0        0    13326 2024-04-21 22:18:04.000000 codeflex-4.0.0/src/codeflex/server/config.py
+-rw-rw-rw-   0        0        0    15114 2024-04-21 22:46:10.000000 codeflex-4.0.0/src/codeflex/server/ctx.py
+-rw-rw-rw-   0        0        0     6076 2024-04-21 22:18:05.000000 codeflex-4.0.0/src/codeflex/server/debughelpers.py
+-rw-rw-rw-   0        0        0     1709 2024-04-21 22:45:40.000000 codeflex-4.0.0/src/codeflex/server/globals.py
+-rw-rw-rw-   0        0        0    23084 2024-02-14 20:44:10.000000 codeflex-4.0.0/src/codeflex/server/helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:52:35.794178 codeflex-4.0.0/src/codeflex/server/json/
+-rw-rw-rw-   0        0        0     5602 2024-02-14 20:44:10.000000 codeflex-4.0.0/src/codeflex/server/json/__init__.py
+-rw-rw-rw-   0        0        0     7646 2024-02-14 20:44:10.000000 codeflex-4.0.0/src/codeflex/server/json/provider.py
+-rw-rw-rw-   0        0        0     9280 2024-02-14 20:44:10.000000 codeflex-4.0.0/src/codeflex/server/json/tag.py
+-rw-rw-rw-   0        0        0     2375 2024-04-21 22:18:07.000000 codeflex-4.0.0/src/codeflex/server/logging.py
+-rw-rw-rw-   0        0        0        0 2024-02-14 20:44:10.000000 codeflex-4.0.0/src/codeflex/server/py.typed
+-rw-rw-rw-   0        0        0    14488 2024-04-21 22:45:08.000000 codeflex-4.0.0/src/codeflex/server/sessions.py
+-rw-rw-rw-   0        0        0      750 2024-02-14 20:44:10.000000 codeflex-4.0.0/src/codeflex/server/signals.py
+-rw-rw-rw-   0        0        0     7527 2024-04-21 22:44:16.000000 codeflex-4.0.0/src/codeflex/server/templating.py
+-rw-rw-rw-   0        0        0    10157 2024-04-21 22:44:02.000000 codeflex-4.0.0/src/codeflex/server/testing.py
+-rw-rw-rw-   0        0        0     3190 2024-02-14 20:44:10.000000 codeflex-4.0.0/src/codeflex/server/typing.py
+-rw-rw-rw-   0        0        0     6939 2024-02-14 20:44:10.000000 codeflex-4.0.0/src/codeflex/server/views.py
+-rw-rw-rw-   0        0        0     5831 2024-02-14 20:44:10.000000 codeflex-4.0.0/src/codeflex/server/wrappers.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:52:35.794178 codeflex-4.0.0/src/codeflex/url/
+-rw-rw-rw-   0        0        0        0 2024-04-17 23:25:20.000000 codeflex-4.0.0/src/codeflex/url/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:52:36.278401 codeflex-4.0.0/src/codeflex/url/connect/
+-rw-rw-rw-   0        0        0     4963 2024-02-14 20:45:27.000000 codeflex-4.0.0/src/codeflex/url/connect/__init__.py
+-rw-rw-rw-   0        0        0      435 2024-02-14 20:45:27.000000 codeflex-4.0.0/src/codeflex/url/connect/__version__.py
+-rw-rw-rw-   0        0        0     1495 2024-02-14 20:45:27.000000 codeflex-4.0.0/src/codeflex/url/connect/_internal_utils.py
+-rw-rw-rw-   0        0        0    19553 2024-02-14 20:45:27.000000 codeflex-4.0.0/src/codeflex/url/connect/adapters.py
+-rw-rw-rw-   0        0        0     6449 2024-02-14 20:45:27.000000 codeflex-4.0.0/src/codeflex/url/connect/api.py
+-rw-rw-rw-   0        0        0    10187 2024-02-14 20:45:27.000000 codeflex-4.0.0/src/codeflex/url/connect/auth.py
+-rw-rw-rw-   0        0        0      429 2024-02-14 20:45:27.000000 codeflex-4.0.0/src/codeflex/url/connect/certs.py
+-rw-rw-rw-   0        0        0     1451 2024-02-14 20:45:27.000000 codeflex-4.0.0/src/codeflex/url/connect/compat.py
+-rw-rw-rw-   0        0        0    18560 2024-02-14 20:45:27.000000 codeflex-4.0.0/src/codeflex/url/connect/cookies.py
+-rw-rw-rw-   0        0        0     3811 2024-02-14 20:45:27.000000 codeflex-4.0.0/src/codeflex/url/connect/exceptions.py
+-rw-rw-rw-   0        0        0     3875 2024-02-14 20:45:27.000000 codeflex-4.0.0/src/codeflex/url/connect/help.py
+-rw-rw-rw-   0        0        0      733 2024-02-14 20:45:27.000000 codeflex-4.0.0/src/codeflex/url/connect/hooks.py
+-rw-rw-rw-   0        0        0    35223 2024-02-14 20:45:27.000000 codeflex-4.0.0/src/codeflex/url/connect/models.py
+-rw-rw-rw-   0        0        0      957 2024-02-14 20:45:27.000000 codeflex-4.0.0/src/codeflex/url/connect/packages.py
+-rw-rw-rw-   0        0        0    30373 2024-02-14 20:45:27.000000 codeflex-4.0.0/src/codeflex/url/connect/sessions.py
+-rw-rw-rw-   0        0        0     4235 2024-02-14 20:45:27.000000 codeflex-4.0.0/src/codeflex/url/connect/status_codes.py
+-rw-rw-rw-   0        0        0     2912 2024-02-14 20:45:27.000000 codeflex-4.0.0/src/codeflex/url/connect/structures.py
+-rw-rw-rw-   0        0        0    33448 2024-02-14 20:45:27.000000 codeflex-4.0.0/src/codeflex/url/connect/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 13:52:36.278401 codeflex-4.0.0/src/codeflex.egg-info/
+-rw-rw-rw-   0        0        0     6492 2024-04-24 13:52:34.000000 codeflex-4.0.0/src/codeflex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1846 2024-04-24 13:52:34.000000 codeflex-4.0.0/src/codeflex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 13:52:34.000000 codeflex-4.0.0/src/codeflex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2024-04-24 13:52:34.000000 codeflex-4.0.0/src/codeflex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-24 13:52:34.000000 codeflex-4.0.0/src/codeflex.egg-info/top_level.txt
```

### Comparing `codeflex-3.1.1/LICENSE` & `codeflex-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/PKG-INFO` & `codeflex-4.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 Metadata-Version: 2.1
 Name: codeflex
-Version: 3.1.1
+Version: 4.0.0
 Summary: ¡Conecta a los Microservicios de CodeFlex desde una Sola Librería!
 Home-page: https://codeflex.com.co/
 Author: CODEFLEX S.A.S.
 Author-email: info@codeflex.com.co
 License: This software is owned by CodeFlex S.A.S. and is protected by applicable copyright laws. The distribution and use of this software are subject to the terms and conditions outlined below.
 Project-URL: Bug Tracker, https://docs.codeflex.com.co/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: idna
+Requires-Dist: charset_normalizer
+Requires-Dist: chardet
+Requires-Dist: urllib3
+Requires-Dist: certifi
+Requires-Dist: werkzeug
+Requires-Dist: click
+Requires-Dist: blinker
+Requires-Dist: jinja2
+Requires-Dist: itsdangerous
 
 [![MIT License][license-shield]](https://s3.amazonaws.com/www.codeflex.lat/documentos/c3320017-1937-4353-8881-475e3c89e25e/LICENSE.txt)
 
 <!-- PROJECT LOGO -->
 <br />
 <p align="center">
   <a href="https://codeflex.com.co">
```

#### html2text {}

```diff
@@ -1,19 +1,22 @@
-Metadata-Version: 2.1 Name: codeflex Version: 3.1.1 Summary: Â¡Conecta a los
+Metadata-Version: 2.1 Name: codeflex Version: 4.0.0 Summary: Â¡Conecta a los
 Microservicios de CodeFlex desde una Sola LibrerÃ­a! Home-page: https://
 codeflex.com.co/ Author: CODEFLEX S.A.S. Author-email: info@codeflex.com.co
 License: This software is owned by CodeFlex S.A.S. and is protected by
 applicable copyright laws. The distribution and use of this software are
 subject to the terms and conditions outlined below. Project-URL: Bug Tracker,
 https://docs.codeflex.com.co/ Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
-markdown License-File: LICENSE [![MIT License][license-shield]](https://
-s3.amazonaws.com/www.codeflex.lat/documentos/c3320017-1937-4353-8881-
-475e3c89e25e/LICENSE.txt)
+markdown License-File: LICENSE Requires-Dist: idna Requires-Dist:
+charset_normalizer Requires-Dist: chardet Requires-Dist: urllib3 Requires-Dist:
+certifi Requires-Dist: werkzeug Requires-Dist: click Requires-Dist: blinker
+Requires-Dist: jinja2 Requires-Dist: itsdangerous [![MIT License][license-
+shield]](https://s3.amazonaws.com/www.codeflex.lat/documentos/c3320017-1937-
+4353-8881-475e3c89e25e/LICENSE.txt)
                                     _[_L_o_g_o_]
                            ******** CCOODDEEFFLLEEXX SS..AA..SS.. ********
               CodificaciÃ³n y Almacenamiento Simplificados | IDE
                               _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 ## About The Project [![miniatura][miniatura]](https://codeflex.com.co) ###
 Installation ```python pip install codeflex ``` ## Usage * Example 1 |
 Connection to MySQL ```python from codeflex.company import mysql respuesta =
```

### Comparing `codeflex-3.1.1/README.md` & `codeflex-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/company/mysql.py` & `codeflex-4.0.0/src/codeflex/company/mysql.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/company/polly.py` & `codeflex-4.0.0/src/codeflex/company/polly.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/server/__init__.py` & `codeflex-4.0.0/src/codeflex/server/__init__.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/server/app.py` & `codeflex-4.0.0/src/codeflex/server/app.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/server/blueprints.py` & `codeflex-4.0.0/src/codeflex/server/blueprints.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/server/cero/app.py` & `codeflex-4.0.0/src/codeflex/server/cero/app.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/server/cero/blueprints.py` & `codeflex-4.0.0/src/codeflex/server/cero/blueprints.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/server/cero/scaffold.py` & `codeflex-4.0.0/src/codeflex/server/cero/scaffold.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/server/cli.py` & `codeflex-4.0.0/src/codeflex/server/cli.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/server/config.py` & `codeflex-4.0.0/src/codeflex/server/config.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/server/ctx.py` & `codeflex-4.0.0/src/codeflex/server/ctx.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/server/debughelpers.py` & `codeflex-4.0.0/src/codeflex/server/debughelpers.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/server/globals.py` & `codeflex-4.0.0/src/codeflex/server/globals.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/server/helpers.py` & `codeflex-4.0.0/src/codeflex/server/helpers.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/server/json/__init__.py` & `codeflex-4.0.0/src/codeflex/server/json/__init__.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/server/json/provider.py` & `codeflex-4.0.0/src/codeflex/server/json/provider.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/server/json/tag.py` & `codeflex-4.0.0/src/codeflex/server/json/tag.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/server/logging.py` & `codeflex-4.0.0/src/codeflex/server/logging.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/server/sessions.py` & `codeflex-4.0.0/src/codeflex/server/sessions.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/server/signals.py` & `codeflex-4.0.0/src/codeflex/server/signals.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/server/templating.py` & `codeflex-4.0.0/src/codeflex/server/templating.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/server/testing.py` & `codeflex-4.0.0/src/codeflex/server/testing.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/server/typing.py` & `codeflex-4.0.0/src/codeflex/server/typing.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/server/views.py` & `codeflex-4.0.0/src/codeflex/server/views.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/server/wrappers.py` & `codeflex-4.0.0/src/codeflex/server/wrappers.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/url/connect/__init__.py` & `codeflex-4.0.0/src/codeflex/url/connect/__init__.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/url/connect/_internal_utils.py` & `codeflex-4.0.0/src/codeflex/url/connect/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/url/connect/adapters.py` & `codeflex-4.0.0/src/codeflex/url/connect/adapters.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/url/connect/api.py` & `codeflex-4.0.0/src/codeflex/url/connect/api.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/url/connect/auth.py` & `codeflex-4.0.0/src/codeflex/url/connect/auth.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/url/connect/compat.py` & `codeflex-4.0.0/src/codeflex/url/connect/compat.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/url/connect/cookies.py` & `codeflex-4.0.0/src/codeflex/url/connect/cookies.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/url/connect/exceptions.py` & `codeflex-4.0.0/src/codeflex/url/connect/exceptions.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/url/connect/help.py` & `codeflex-4.0.0/src/codeflex/url/connect/help.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/url/connect/hooks.py` & `codeflex-4.0.0/src/codeflex/url/connect/hooks.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/url/connect/models.py` & `codeflex-4.0.0/src/codeflex/url/connect/models.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/url/connect/packages.py` & `codeflex-4.0.0/src/codeflex/url/connect/packages.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/url/connect/sessions.py` & `codeflex-4.0.0/src/codeflex/url/connect/sessions.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/url/connect/status_codes.py` & `codeflex-4.0.0/src/codeflex/url/connect/status_codes.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/url/connect/structures.py` & `codeflex-4.0.0/src/codeflex/url/connect/structures.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex/url/connect/utils.py` & `codeflex-4.0.0/src/codeflex/url/connect/utils.py`

 * *Files identical despite different names*

### Comparing `codeflex-3.1.1/src/codeflex.egg-info/PKG-INFO` & `codeflex-4.0.0/src/codeflex.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 Metadata-Version: 2.1
 Name: codeflex
-Version: 3.1.1
+Version: 4.0.0
 Summary: ¡Conecta a los Microservicios de CodeFlex desde una Sola Librería!
 Home-page: https://codeflex.com.co/
 Author: CODEFLEX S.A.S.
 Author-email: info@codeflex.com.co
 License: This software is owned by CodeFlex S.A.S. and is protected by applicable copyright laws. The distribution and use of this software are subject to the terms and conditions outlined below.
 Project-URL: Bug Tracker, https://docs.codeflex.com.co/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: idna
+Requires-Dist: charset_normalizer
+Requires-Dist: chardet
+Requires-Dist: urllib3
+Requires-Dist: certifi
+Requires-Dist: werkzeug
+Requires-Dist: click
+Requires-Dist: blinker
+Requires-Dist: jinja2
+Requires-Dist: itsdangerous
 
 [![MIT License][license-shield]](https://s3.amazonaws.com/www.codeflex.lat/documentos/c3320017-1937-4353-8881-475e3c89e25e/LICENSE.txt)
 
 <!-- PROJECT LOGO -->
 <br />
 <p align="center">
   <a href="https://codeflex.com.co">
```

#### html2text {}

```diff
@@ -1,19 +1,22 @@
-Metadata-Version: 2.1 Name: codeflex Version: 3.1.1 Summary: Â¡Conecta a los
+Metadata-Version: 2.1 Name: codeflex Version: 4.0.0 Summary: Â¡Conecta a los
 Microservicios de CodeFlex desde una Sola LibrerÃ­a! Home-page: https://
 codeflex.com.co/ Author: CODEFLEX S.A.S. Author-email: info@codeflex.com.co
 License: This software is owned by CodeFlex S.A.S. and is protected by
 applicable copyright laws. The distribution and use of this software are
 subject to the terms and conditions outlined below. Project-URL: Bug Tracker,
 https://docs.codeflex.com.co/ Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
-markdown License-File: LICENSE [![MIT License][license-shield]](https://
-s3.amazonaws.com/www.codeflex.lat/documentos/c3320017-1937-4353-8881-
-475e3c89e25e/LICENSE.txt)
+markdown License-File: LICENSE Requires-Dist: idna Requires-Dist:
+charset_normalizer Requires-Dist: chardet Requires-Dist: urllib3 Requires-Dist:
+certifi Requires-Dist: werkzeug Requires-Dist: click Requires-Dist: blinker
+Requires-Dist: jinja2 Requires-Dist: itsdangerous [![MIT License][license-
+shield]](https://s3.amazonaws.com/www.codeflex.lat/documentos/c3320017-1937-
+4353-8881-475e3c89e25e/LICENSE.txt)
                                     _[_L_o_g_o_]
                            ******** CCOODDEEFFLLEEXX SS..AA..SS.. ********
               CodificaciÃ³n y Almacenamiento Simplificados | IDE
                               _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 ## About The Project [![miniatura][miniatura]](https://codeflex.com.co) ###
 Installation ```python pip install codeflex ``` ## Usage * Example 1 |
 Connection to MySQL ```python from codeflex.company import mysql respuesta =
```

### Comparing `codeflex-3.1.1/src/codeflex.egg-info/SOURCES.txt` & `codeflex-4.0.0/src/codeflex.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 setup.py
 src/codeflex/__init__.py
 src/codeflex.egg-info/PKG-INFO
 src/codeflex.egg-info/SOURCES.txt
 src/codeflex.egg-info/dependency_links.txt
+src/codeflex.egg-info/requires.txt
 src/codeflex.egg-info/top_level.txt
 src/codeflex/company/__init__.py
 src/codeflex/company/mysql.py
 src/codeflex/company/polly.py
 src/codeflex/server/__init__.py
 src/codeflex/server/__main__.py
 src/codeflex/server/app.py
```

