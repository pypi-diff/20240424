# Comparing `tmp/macal-5.5.0a4.tar.gz` & `tmp/macal-5.5.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macal-5.5.0a4.tar", last modified: Thu Apr 18 16:08:09 2024, max compression
+gzip compressed data, was "macal-5.5.0a5.tar", last modified: Wed Apr 24 15:07:13 2024, max compression
```

## Comparing `macal-5.5.0a4.tar` & `macal-5.5.0a5.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-18 16:08:09.928512 macal-5.5.0a4/
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-18 16:08:09.918512 macal-5.5.0a4/.vscode/
--rw-r--r--   0 marco     (1000) marco     (1000)      540 2024-04-15 15:12:14.000000 macal-5.5.0a4/.vscode/launch.json
--rw-r--r--   0 marco     (1000) marco     (1000)       51 2024-04-15 15:12:14.000000 macal-5.5.0a4/.vscode/settings.json
--rw-r--r--   0 marco     (1000) marco     (1000)     1184 2024-03-22 12:04:18.000000 macal-5.5.0a4/LICENSE.txt
--rw-r--r--   0 marco     (1000) marco     (1000)      179 2024-04-16 17:31:53.000000 macal-5.5.0a4/MANIFEST.in
--rw-r--r--   0 marco     (1000) marco     (1000)     5367 2024-04-18 16:08:09.928512 macal-5.5.0a4/PKG-INFO
--rw-r--r--   0 marco     (1000) marco     (1000)     4551 2024-04-16 13:27:36.000000 macal-5.5.0a4/README.md
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-18 16:08:09.918512 macal-5.5.0a4/documentation/
--rw-r--r--   0 marco     (1000) marco     (1000)     7076 2024-04-15 15:03:44.000000 macal-5.5.0a4/documentation/history.txt
--rw-r--r--   0 marco     (1000) marco     (1000)     1016 2024-04-16 21:58:56.000000 macal-5.5.0a4/pyproject.toml
--rw-r--r--   0 marco     (1000) marco     (1000)       38 2024-04-18 16:08:09.928512 macal-5.5.0a4/setup.cfg
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-18 16:08:09.918512 macal-5.5.0a4/src/
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-18 16:08:09.918512 macal-5.5.0a4/src/macal/
--rw-r--r--   0 marco     (1000) marco     (1000)     1474 2024-04-18 13:46:47.000000 macal-5.5.0a4/src/macal/__about__.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:11:34.000000 macal-5.5.0a4/src/macal/__init__.py
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-18 16:08:09.928512 macal-5.5.0a4/src/macal/frontend/
--rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:10:27.000000 macal-5.5.0a4/src/macal/frontend/__init__.py
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-18 16:08:09.928512 macal-5.5.0a4/src/macal/frontend/ast/
--rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:13:42.000000 macal-5.5.0a4/src/macal/frontend/ast/__init__.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2568 2024-04-08 13:40:36.000000 macal-5.5.0a4/src/macal/frontend/ast/kind.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1892 2024-04-08 20:08:54.000000 macal-5.5.0a4/src/macal/frontend/ast/metadata.py
--rw-r--r--   0 marco     (1000) marco     (1000)    32164 2024-04-09 13:34:29.000000 macal-5.5.0a4/src/macal/frontend/ast/node.py
--rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-22 23:39:28.000000 macal-5.5.0a4/src/macal/frontend/ast/py.typed
--rw-r--r--   0 marco     (1000) marco     (1000)    20787 2024-04-15 14:41:47.000000 macal-5.5.0a4/src/macal/frontend/mlexer.py
--rw-r--r--   0 marco     (1000) marco     (1000)    49026 2024-04-16 21:09:39.000000 macal-5.5.0a4/src/macal/frontend/mparser.py
--rw-r--r--   0 marco     (1000) marco     (1000)     5053 2024-04-16 15:52:59.000000 macal-5.5.0a4/src/macal/frontend/mparserstate.py
--rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-22 16:29:45.000000 macal-5.5.0a4/src/macal/frontend/py.typed
--rw-r--r--   0 marco     (1000) marco     (1000)     5623 2024-04-18 13:45:52.000000 macal-5.5.0a4/src/macal/macal.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2172 2024-04-08 15:16:25.000000 macal-5.5.0a4/src/macal/mexceptions.py
--rw-r--r--   0 marco     (1000) marco     (1000)    15930 2024-04-18 16:03:02.000000 macal-5.5.0a4/src/macal/mrepl.py
--rw-r--r--   0 marco     (1000) marco     (1000)     7436 2024-04-15 17:26:42.000000 macal-5.5.0a4/src/macal/mrun.py
--rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-22 16:29:34.000000 macal-5.5.0a4/src/macal/py.typed
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-18 16:08:09.928512 macal-5.5.0a4/src/macal/runtime/
--rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:10:21.000000 macal-5.5.0a4/src/macal/runtime/__init__.py
--rw-r--r--   0 marco     (1000) marco     (1000)     9289 2024-04-16 15:54:17.000000 macal-5.5.0a4/src/macal/runtime/menvironment.py
--rw-r--r--   0 marco     (1000) marco     (1000)     4011 2024-04-10 20:55:22.000000 macal-5.5.0a4/src/macal/runtime/mimporter.py
--rw-r--r--   0 marco     (1000) marco     (1000)    72797 2024-04-18 13:35:19.000000 macal-5.5.0a4/src/macal/runtime/minterpreter.py
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-18 16:08:09.928512 macal-5.5.0a4/src/macal/runtime/native/
--rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-23 23:21:40.000000 macal-5.5.0a4/src/macal/runtime/native/__init__.py
--rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-24 20:22:17.000000 macal-5.5.0a4/src/macal/runtime/native/py.typed
--rw-r--r--   0 marco     (1000) marco     (1000)     2129 2024-04-15 14:35:04.000000 macal-5.5.0a4/src/macal/runtime/native/system.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1618 2024-03-24 06:01:49.000000 macal-5.5.0a4/src/macal/runtime/native/time.py
--rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-23 18:22:52.000000 macal-5.5.0a4/src/macal/runtime/py.typed
--rw-r--r--   0 marco     (1000) marco     (1000)     1705 2024-04-08 15:40:52.000000 macal-5.5.0a4/src/macal/runtime/value_type.py
--rw-r--r--   0 marco     (1000) marco     (1000)    17433 2024-04-11 16:42:19.000000 macal-5.5.0a4/src/macal/runtime/values.py
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-18 16:08:09.928512 macal-5.5.0a4/src/macal.egg-info/
--rw-r--r--   0 marco     (1000) marco     (1000)     5367 2024-04-18 16:08:09.000000 macal-5.5.0a4/src/macal.egg-info/PKG-INFO
--rw-r--r--   0 marco     (1000) marco     (1000)     1563 2024-04-18 16:08:09.000000 macal-5.5.0a4/src/macal.egg-info/SOURCES.txt
--rw-r--r--   0 marco     (1000) marco     (1000)        1 2024-04-18 16:08:09.000000 macal-5.5.0a4/src/macal.egg-info/dependency_links.txt
--rw-r--r--   0 marco     (1000) marco     (1000)       66 2024-04-18 16:08:09.000000 macal-5.5.0a4/src/macal.egg-info/entry_points.txt
--rw-r--r--   0 marco     (1000) marco     (1000)       73 2024-04-18 16:08:09.000000 macal-5.5.0a4/src/macal.egg-info/requires.txt
--rw-r--r--   0 marco     (1000) marco     (1000)        6 2024-04-18 16:08:09.000000 macal-5.5.0a4/src/macal.egg-info/top_level.txt
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-18 16:08:09.928512 macal-5.5.0a4/tests/
--rw-r--r--   0 marco     (1000) marco     (1000)     1030 2024-04-18 12:40:10.000000 macal-5.5.0a4/tests/agent.py
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-18 16:08:09.928512 macal-5.5.0a4/tests/lib/
--rw-r--r--   0 marco     (1000) marco     (1000)      639 2023-11-17 02:10:51.000000 macal-5.5.0a4/tests/lib/csv.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      996 2023-11-17 14:12:28.000000 macal-5.5.0a4/tests/lib/ext_csv.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2135 2024-04-04 21:12:11.000000 macal-5.5.0a4/tests/lib/ext_io.py
--rw-r--r--   0 marco     (1000) marco     (1000)      873 2023-11-17 14:12:28.000000 macal-5.5.0a4/tests/lib/ext_keyring.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2265 2023-11-17 14:12:28.000000 macal-5.5.0a4/tests/lib/ext_math.py
--rw-r--r--   0 marco     (1000) marco     (1000)     3810 2024-04-09 08:23:31.000000 macal-5.5.0a4/tests/lib/ext_strings.py
--rw-r--r--   0 marco     (1000) marco     (1000)     4601 2023-11-17 14:12:28.000000 macal-5.5.0a4/tests/lib/ext_syslog.py
--rw-r--r--   0 marco     (1000) marco     (1000)     4082 2024-04-10 19:30:13.000000 macal-5.5.0a4/tests/lib/ext_system.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1910 2023-11-17 14:12:28.000000 macal-5.5.0a4/tests/lib/ext_time.py
--rw-r--r--   0 marco     (1000) marco     (1000)      942 2024-04-04 21:00:01.000000 macal-5.5.0a4/tests/lib/io.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      808 2023-11-17 02:12:56.000000 macal-5.5.0a4/tests/lib/keyring.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     1329 2024-04-05 15:54:51.000000 macal-5.5.0a4/tests/lib/math.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)    34808 2024-04-10 20:24:42.000000 macal-5.5.0a4/tests/lib/meraki_api_library_v1.py
--rw-r--r--   0 marco     (1000) marco     (1000)     5577 2024-04-10 20:38:33.000000 macal-5.5.0a4/tests/lib/meraki_v1.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     2047 2023-11-27 14:53:48.000000 macal-5.5.0a4/tests/lib/strings.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      661 2023-11-17 02:14:43.000000 macal-5.5.0a4/tests/lib/syslog.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     2923 2024-04-18 14:01:00.000000 macal-5.5.0a4/tests/lib/system.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      991 2023-11-17 02:16:00.000000 macal-5.5.0a4/tests/lib/time.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     5867 2024-04-09 23:07:14.000000 macal-5.5.0a4/tests/test.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-24 15:07:13.721301 macal-5.5.0a5/
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-24 15:07:13.711301 macal-5.5.0a5/.vscode/
+-rw-r--r--   0 marco     (1000) marco     (1000)      540 2024-04-15 15:12:14.000000 macal-5.5.0a5/.vscode/launch.json
+-rw-r--r--   0 marco     (1000) marco     (1000)       51 2024-04-15 15:12:14.000000 macal-5.5.0a5/.vscode/settings.json
+-rw-r--r--   0 marco     (1000) marco     (1000)     1184 2024-03-22 12:04:18.000000 macal-5.5.0a5/LICENSE.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)      179 2024-04-16 17:31:53.000000 macal-5.5.0a5/MANIFEST.in
+-rw-r--r--   0 marco     (1000) marco     (1000)     7525 2024-04-24 15:07:13.721301 macal-5.5.0a5/PKG-INFO
+-rw-r--r--   0 marco     (1000) marco     (1000)     6709 2024-04-24 15:04:34.000000 macal-5.5.0a5/README.md
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-24 15:07:13.711301 macal-5.5.0a5/documentation/
+-rw-r--r--   0 marco     (1000) marco     (1000)     7076 2024-04-15 15:03:44.000000 macal-5.5.0a5/documentation/history.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)     1016 2024-04-16 21:58:56.000000 macal-5.5.0a5/pyproject.toml
+-rw-r--r--   0 marco     (1000) marco     (1000)       38 2024-04-24 15:07:13.721301 macal-5.5.0a5/setup.cfg
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-24 15:07:13.711301 macal-5.5.0a5/src/
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-24 15:07:13.711301 macal-5.5.0a5/src/macal/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1474 2024-04-24 14:58:33.000000 macal-5.5.0a5/src/macal/__about__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:11:34.000000 macal-5.5.0a5/src/macal/__init__.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-24 15:07:13.711301 macal-5.5.0a5/src/macal/frontend/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:10:27.000000 macal-5.5.0a5/src/macal/frontend/__init__.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-24 15:07:13.711301 macal-5.5.0a5/src/macal/frontend/ast/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:13:42.000000 macal-5.5.0a5/src/macal/frontend/ast/__init__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2568 2024-04-08 13:40:36.000000 macal-5.5.0a5/src/macal/frontend/ast/kind.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1892 2024-04-08 20:08:54.000000 macal-5.5.0a5/src/macal/frontend/ast/metadata.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    32164 2024-04-09 13:34:29.000000 macal-5.5.0a5/src/macal/frontend/ast/node.py
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-22 23:39:28.000000 macal-5.5.0a5/src/macal/frontend/ast/py.typed
+-rw-r--r--   0 marco     (1000) marco     (1000)    20787 2024-04-15 14:41:47.000000 macal-5.5.0a5/src/macal/frontend/mlexer.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    49026 2024-04-16 21:09:39.000000 macal-5.5.0a5/src/macal/frontend/mparser.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     5053 2024-04-16 15:52:59.000000 macal-5.5.0a5/src/macal/frontend/mparserstate.py
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-22 16:29:45.000000 macal-5.5.0a5/src/macal/frontend/py.typed
+-rw-r--r--   0 marco     (1000) marco     (1000)     5623 2024-04-18 13:45:52.000000 macal-5.5.0a5/src/macal/macal.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2172 2024-04-08 15:16:25.000000 macal-5.5.0a5/src/macal/mexceptions.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    15930 2024-04-18 16:03:02.000000 macal-5.5.0a5/src/macal/mrepl.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     7436 2024-04-15 17:26:42.000000 macal-5.5.0a5/src/macal/mrun.py
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-22 16:29:34.000000 macal-5.5.0a5/src/macal/py.typed
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-24 15:07:13.721301 macal-5.5.0a5/src/macal/runtime/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:10:21.000000 macal-5.5.0a5/src/macal/runtime/__init__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     9289 2024-04-16 15:54:17.000000 macal-5.5.0a5/src/macal/runtime/menvironment.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     4011 2024-04-10 20:55:22.000000 macal-5.5.0a5/src/macal/runtime/mimporter.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    72797 2024-04-18 13:35:19.000000 macal-5.5.0a5/src/macal/runtime/minterpreter.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-24 15:07:13.721301 macal-5.5.0a5/src/macal/runtime/native/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-23 23:21:40.000000 macal-5.5.0a5/src/macal/runtime/native/__init__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-24 20:22:17.000000 macal-5.5.0a5/src/macal/runtime/native/py.typed
+-rw-r--r--   0 marco     (1000) marco     (1000)     2129 2024-04-15 14:35:04.000000 macal-5.5.0a5/src/macal/runtime/native/system.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1618 2024-03-24 06:01:49.000000 macal-5.5.0a5/src/macal/runtime/native/time.py
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-23 18:22:52.000000 macal-5.5.0a5/src/macal/runtime/py.typed
+-rw-r--r--   0 marco     (1000) marco     (1000)     1705 2024-04-08 15:40:52.000000 macal-5.5.0a5/src/macal/runtime/value_type.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    17433 2024-04-11 16:42:19.000000 macal-5.5.0a5/src/macal/runtime/values.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-24 15:07:13.721301 macal-5.5.0a5/src/macal.egg-info/
+-rw-r--r--   0 marco     (1000) marco     (1000)     7525 2024-04-24 15:07:13.000000 macal-5.5.0a5/src/macal.egg-info/PKG-INFO
+-rw-r--r--   0 marco     (1000) marco     (1000)     1563 2024-04-24 15:07:13.000000 macal-5.5.0a5/src/macal.egg-info/SOURCES.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)        1 2024-04-24 15:07:13.000000 macal-5.5.0a5/src/macal.egg-info/dependency_links.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)       66 2024-04-24 15:07:13.000000 macal-5.5.0a5/src/macal.egg-info/entry_points.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)       73 2024-04-24 15:07:13.000000 macal-5.5.0a5/src/macal.egg-info/requires.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)        6 2024-04-24 15:07:13.000000 macal-5.5.0a5/src/macal.egg-info/top_level.txt
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-24 15:07:13.721301 macal-5.5.0a5/tests/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1030 2024-04-18 12:40:10.000000 macal-5.5.0a5/tests/agent.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-24 15:07:13.721301 macal-5.5.0a5/tests/lib/
+-rw-r--r--   0 marco     (1000) marco     (1000)      639 2023-11-17 02:10:51.000000 macal-5.5.0a5/tests/lib/csv.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      996 2023-11-17 14:12:28.000000 macal-5.5.0a5/tests/lib/ext_csv.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2135 2024-04-04 21:12:11.000000 macal-5.5.0a5/tests/lib/ext_io.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      873 2023-11-17 14:12:28.000000 macal-5.5.0a5/tests/lib/ext_keyring.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2265 2023-11-17 14:12:28.000000 macal-5.5.0a5/tests/lib/ext_math.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     3810 2024-04-09 08:23:31.000000 macal-5.5.0a5/tests/lib/ext_strings.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     4601 2023-11-17 14:12:28.000000 macal-5.5.0a5/tests/lib/ext_syslog.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     4082 2024-04-10 19:30:13.000000 macal-5.5.0a5/tests/lib/ext_system.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1910 2023-11-17 14:12:28.000000 macal-5.5.0a5/tests/lib/ext_time.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      942 2024-04-04 21:00:01.000000 macal-5.5.0a5/tests/lib/io.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      808 2023-11-17 02:12:56.000000 macal-5.5.0a5/tests/lib/keyring.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     1329 2024-04-05 15:54:51.000000 macal-5.5.0a5/tests/lib/math.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)    34808 2024-04-10 20:24:42.000000 macal-5.5.0a5/tests/lib/meraki_api_library_v1.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     5577 2024-04-10 20:38:33.000000 macal-5.5.0a5/tests/lib/meraki_v1.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     2047 2023-11-27 14:53:48.000000 macal-5.5.0a5/tests/lib/strings.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      661 2023-11-17 02:14:43.000000 macal-5.5.0a5/tests/lib/syslog.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     2923 2024-04-18 14:01:00.000000 macal-5.5.0a5/tests/lib/system.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      991 2023-11-17 02:16:00.000000 macal-5.5.0a5/tests/lib/time.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     5867 2024-04-09 23:07:14.000000 macal-5.5.0a5/tests/test.py
```

### Comparing `macal-5.5.0a4/.vscode/launch.json` & `macal-5.5.0a5/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/LICENSE.txt` & `macal-5.5.0a5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/PKG-INFO` & `macal-5.5.0a5/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,8 @@
-Metadata-Version: 2.1
-Name: macal
-Version: 5.5.0a4
-Summary: Macal DSL is used for collecting and transforming data from various sources.
-Author-email: Marco Caspers <SamaDevTeam@westcon.com>
-Project-URL: Homepage, https://github.com/Sama-Developer/macal
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: unidecode
-Requires-Dist: keyring
-Requires-Dist: keyrings.alt
-Requires-Dist: meraki
-Requires-Dist: pydantic
-Requires-Dist: python-jose[cryptography]
-
-# Macal DSL 5.5 Alpha 2
+# Macal DSL 5.5 Alpha 5
 
 ## Introduction
 
 This is version 5.5 of the Macal DSL language
 This is an interim version.
 
 I have removed the bytecode compiler and runtime.
@@ -33,31 +11,36 @@
 
 Known issues:
 1).  If you include a file for which there are multiple files in the file search path that have the same file name, 
      there is no way of telling which one gets included.
      A safeguard is in place to prevent importing a file from itself, but i can't exclude multiple files with
      the same name on the search path other than the user controlling the search path.
 
+2). The utilities mi and mr have been replaced with mrepl and mrun respectively.
+    Utilities mc and md have been removed.
+
 ## Installation
 
 ```bash
-python3 -m pip install macal==5.5.0.alpha.2
+python3 -m pip install macal==5.5.0.alpha.5
 ```
 
 ## Usage
 
 Macal can be used in 3 main ways:
 
 1). Use it on the commandline with 'mrepl' to run interactively.
 
 2). Use it on the commandline with 'mrun' to run a file. (type mrun -h to get help).
 
 3). Include the class in your product and work from there.
     An example will be provided in a later chapter.
 
+4). After installing the mide package you can use the mide utility which is a very simple cli/text based editor/ide.
+
 
 ## Instruction set "EBNF"
 
 
 letter = "a".."z" | "A".."Z"
 
 digit = "0".."9"
@@ -177,7 +160,95 @@
 
 member_expr = primary_expr ("." primary_expr | "[" "]" new array_element | "[" expr "]") 
 
 new_array_element = "=" expr
 
 primary_expr = ident | int_number | float_number | string_literal | "(" expr ")" | array_literal | record_literal |
                type_stmt | is_type_stmt
+
+
+## Statements
+
+a = 1;          // integer type is inferred from the assignment
+f = 1.0;        // a float
+b = true;       // boolean
+s = "this is a string"; // string
+s2 = 'this is also a string';
+s3 = $"this is a string with {a} {b} {s} interpolation.";
+
+arr = ["item1", "item2", "item3"];  // create a variable arr that has an array with 3 elements.
+rec = {"key1": "value1", "key2": 2, "key3": nil}; // create a variable rec with 3 key/value pairs.
+// alternative method to define the same array and record in a different way.
+arr = array;
+arr[] = "item1";
+arr[] = "item2";
+arr[] = "item3";
+rec = record;
+rec["key1"] = "value1";
+rec["key2"] = 2;
+rec["key3"] = nil;
+
+// getting the value from an array:
+print(arr[0]);
+print(arr[2]);
+
+// getting the values from a record, method 1:
+print(rec["key1"]);
+print(rec["key2"]);
+// Alternative way for getting the values from a record:
+print(rec.key1);
+print(rec.key2);
+
+
+print(a);
+print(s3);
+print(a, f, b);
+
+if <condition> {
+
+} elif <condition> {
+
+} else {
+
+}
+
+while <condition> {
+    // can use continue to continue the loop.
+    // can use break to break out of the loop.
+}
+
+foreach <iterable> {
+    print(it); // The it variable contains the current value of the iterator that is iterating over the iterable.
+    // can use continue to continue the loop.
+    // can use break to break out of the loop.
+}
+
+func_name => (a, b) { // function definition
+    print(a);
+    print(b);
+    return a + b;
+}
+
+// Defines a function that links to an external function that lives in a python module
+// called <module_name>.py with the name <ext_unc_name>
+func_name_2 => (a, b) external "<module_name>", "<ext_func_name>";
+
+
+switch <expr> {
+    case <expr> : {
+        break;
+    }
+    case <expr>: {
+
+    }
+    case <expr>: {
+
+    }
+    default : {
+
+    }
+}
+
+q = [{}];
+select distinct a as b from x() where c == 42 and d == "hot" merge into q;
+
+halt 1; // terminates execution.
```

### Comparing `macal-5.5.0a4/documentation/history.txt` & `macal-5.5.0a5/documentation/history.txt`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/pyproject.toml` & `macal-5.5.0a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/src/macal/__about__.py` & `macal-5.5.0a5/src/macal/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,12 +25,12 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 # IN THE SOFTWARE.
 #
 # SPDX-License-Identifier: MIT
 #
 
-__version__ = "5.5.0.alpha.4"
+__version__ = "5.5.0.alpha.5"
 __author__ = "Marco Caspers"
 __email__ = "samadevteam@westcon.com"
 __copyright__ = "Copyright 2024 Westcon Sama Development Team"
 __license__ = "MIT License"
```

### Comparing `macal-5.5.0a4/src/macal/__init__.py` & `macal-5.5.0a5/src/macal/__init__.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/src/macal/frontend/__init__.py` & `macal-5.5.0a5/src/macal/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/src/macal/frontend/ast/__init__.py` & `macal-5.5.0a5/src/macal/frontend/ast/__init__.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/src/macal/frontend/ast/kind.py` & `macal-5.5.0a5/src/macal/frontend/ast/kind.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/src/macal/frontend/ast/metadata.py` & `macal-5.5.0a5/src/macal/frontend/ast/metadata.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/src/macal/frontend/ast/node.py` & `macal-5.5.0a5/src/macal/frontend/ast/node.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/src/macal/frontend/mlexer.py` & `macal-5.5.0a5/src/macal/frontend/mlexer.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/src/macal/frontend/mparser.py` & `macal-5.5.0a5/src/macal/frontend/mparser.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/src/macal/frontend/mparserstate.py` & `macal-5.5.0a5/src/macal/frontend/mparserstate.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/src/macal/macal.py` & `macal-5.5.0a5/src/macal/macal.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/src/macal/mexceptions.py` & `macal-5.5.0a5/src/macal/mexceptions.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/src/macal/mrepl.py` & `macal-5.5.0a5/src/macal/mrepl.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/src/macal/mrun.py` & `macal-5.5.0a5/src/macal/mrun.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/src/macal/runtime/__init__.py` & `macal-5.5.0a5/src/macal/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/src/macal/runtime/menvironment.py` & `macal-5.5.0a5/src/macal/runtime/menvironment.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/src/macal/runtime/mimporter.py` & `macal-5.5.0a5/src/macal/runtime/mimporter.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/src/macal/runtime/minterpreter.py` & `macal-5.5.0a5/src/macal/runtime/minterpreter.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/src/macal/runtime/native/__init__.py` & `macal-5.5.0a5/src/macal/runtime/native/__init__.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/src/macal/runtime/native/system.py` & `macal-5.5.0a5/src/macal/runtime/native/system.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/src/macal/runtime/native/time.py` & `macal-5.5.0a5/src/macal/runtime/native/time.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/src/macal/runtime/value_type.py` & `macal-5.5.0a5/src/macal/runtime/value_type.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/src/macal/runtime/values.py` & `macal-5.5.0a5/src/macal/runtime/values.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/src/macal.egg-info/SOURCES.txt` & `macal-5.5.0a5/src/macal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/tests/agent.py` & `macal-5.5.0a5/tests/agent.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/tests/lib/csv.mcl` & `macal-5.5.0a5/tests/lib/csv.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/tests/lib/ext_csv.py` & `macal-5.5.0a5/tests/lib/ext_csv.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/tests/lib/ext_io.py` & `macal-5.5.0a5/tests/lib/ext_io.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/tests/lib/ext_keyring.py` & `macal-5.5.0a5/tests/lib/ext_keyring.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/tests/lib/ext_math.py` & `macal-5.5.0a5/tests/lib/ext_math.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/tests/lib/ext_strings.py` & `macal-5.5.0a5/tests/lib/ext_strings.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/tests/lib/ext_syslog.py` & `macal-5.5.0a5/tests/lib/ext_syslog.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/tests/lib/ext_system.py` & `macal-5.5.0a5/tests/lib/ext_system.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/tests/lib/ext_time.py` & `macal-5.5.0a5/tests/lib/ext_time.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/tests/lib/io.mcl` & `macal-5.5.0a5/tests/lib/io.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/tests/lib/keyring.mcl` & `macal-5.5.0a5/tests/lib/keyring.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/tests/lib/math.mcl` & `macal-5.5.0a5/tests/lib/math.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/tests/lib/meraki_api_library_v1.py` & `macal-5.5.0a5/tests/lib/meraki_api_library_v1.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/tests/lib/meraki_v1.mcl` & `macal-5.5.0a5/tests/lib/meraki_v1.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/tests/lib/strings.mcl` & `macal-5.5.0a5/tests/lib/strings.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/tests/lib/syslog.mcl` & `macal-5.5.0a5/tests/lib/syslog.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/tests/lib/system.mcl` & `macal-5.5.0a5/tests/lib/system.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/tests/lib/time.mcl` & `macal-5.5.0a5/tests/lib/time.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a4/tests/test.py` & `macal-5.5.0a5/tests/test.py`

 * *Files identical despite different names*

