# Comparing `tmp/deepgram_sdk-3.2.6.tar.gz` & `tmp/deepgram_sdk-3.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepgram_sdk-3.2.6.tar", last modified: Wed Apr 17 00:53:02 2024, max compression
+gzip compressed data, was "deepgram_sdk-3.2.7.tar", last modified: Wed Apr 24 20:39:38 2024, max compression
```

## Comparing `deepgram_sdk-3.2.6.tar` & `deepgram_sdk-3.2.7.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.702455 deepgram_sdk-3.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12275 2024-04-17 00:53:02.702455 deepgram_sdk-3.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11524 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.690455 deepgram_sdk-3.2.6/deepgram/
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.690455 deepgram_sdk-3.2.6/deepgram/audio/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/audio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.690455 deepgram_sdk-3.2.6/deepgram/audio/microphone/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/audio/microphone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/audio/microphone/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/audio/microphone/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/audio/microphone/microphone.py
--rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.694455 deepgram_sdk-3.2.6/deepgram/clients/
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/abstract_async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/abstract_sync_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.694455 deepgram_sdk-3.2.6/deepgram/clients/analyze/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/analyze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/analyze/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/analyze/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/analyze/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.694455 deepgram_sdk-3.2.6/deepgram/clients/analyze/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/analyze/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12291 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/analyze/v1/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12411 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/analyze/v1/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/analyze/v1/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/analyze/v1/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/analyze/v1/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/listen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.694455 deepgram_sdk-3.2.6/deepgram/clients/live/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/live/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/live/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/live/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/live/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/live/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.694455 deepgram_sdk-3.2.6/deepgram/clients/live/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/live/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21559 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/live/v1/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    20858 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/live/v1/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/live/v1/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/live/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.694455 deepgram_sdk-3.2.6/deepgram/clients/manage/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/manage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/manage/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.698455 deepgram_sdk-3.2.6/deepgram/clients/manage/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/manage/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33519 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/manage/v1/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    33112 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/manage/v1/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/manage/v1/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    16279 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/manage/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.698455 deepgram_sdk-3.2.6/deepgram/clients/onprem/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/onprem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/onprem/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.698455 deepgram_sdk-3.2.6/deepgram/clients/onprem/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/onprem/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/onprem/v1/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/onprem/v1/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.698455 deepgram_sdk-3.2.6/deepgram/clients/prerecorded/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/prerecorded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/prerecorded/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/prerecorded/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/prerecorded/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.698455 deepgram_sdk-3.2.6/deepgram/clients/prerecorded/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/prerecorded/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12830 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/prerecorded/v1/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12762 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/prerecorded/v1/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/prerecorded/v1/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/prerecorded/v1/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    21250 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/prerecorded/v1/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/read.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.702455 deepgram_sdk-3.2.6/deepgram/clients/speak/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/speak/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/speak/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/speak/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.702455 deepgram_sdk-3.2.6/deepgram/clients/speak/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/speak/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/speak/v1/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/speak/v1/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/speak/v1/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/speak/v1/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/clients/speak/v1/response.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/deepgram/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:53:02.702455 deepgram_sdk-3.2.6/deepgram_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12275 2024-04-17 00:53:02.000000 deepgram_sdk-3.2.6/deepgram_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-17 00:53:02.000000 deepgram_sdk-3.2.6/deepgram_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 00:53:02.000000 deepgram_sdk-3.2.6/deepgram_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-17 00:53:02.000000 deepgram_sdk-3.2.6/deepgram_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 00:53:02.000000 deepgram_sdk-3.2.6/deepgram_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 00:53:02.702455 deepgram_sdk-3.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-17 00:52:52.000000 deepgram_sdk-3.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:39:38.830999 deepgram_sdk-3.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12280 2024-04-24 20:39:38.830999 deepgram_sdk-3.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11529 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:39:38.818999 deepgram_sdk-3.2.7/deepgram/
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:39:38.818999 deepgram_sdk-3.2.7/deepgram/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/audio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:39:38.818999 deepgram_sdk-3.2.7/deepgram/audio/microphone/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/audio/microphone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/audio/microphone/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/audio/microphone/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/audio/microphone/microphone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:39:38.818999 deepgram_sdk-3.2.7/deepgram/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/abstract_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/abstract_sync_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:39:38.822999 deepgram_sdk-3.2.7/deepgram/clients/analyze/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/analyze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/analyze/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/analyze/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/analyze/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:39:38.822999 deepgram_sdk-3.2.7/deepgram/clients/analyze/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/analyze/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12291 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/analyze/v1/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12411 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/analyze/v1/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/analyze/v1/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/analyze/v1/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/analyze/v1/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/listen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:39:38.822999 deepgram_sdk-3.2.7/deepgram/clients/live/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/live/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/live/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/live/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/live/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/live/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:39:38.822999 deepgram_sdk-3.2.7/deepgram/clients/live/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/live/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22243 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/live/v1/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21640 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/live/v1/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/live/v1/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/live/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:39:38.822999 deepgram_sdk-3.2.7/deepgram/clients/manage/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/manage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/manage/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:39:38.826999 deepgram_sdk-3.2.7/deepgram/clients/manage/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/manage/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33519 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/manage/v1/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33112 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/manage/v1/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/manage/v1/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16279 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/manage/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:39:38.826999 deepgram_sdk-3.2.7/deepgram/clients/onprem/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/onprem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/onprem/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:39:38.826999 deepgram_sdk-3.2.7/deepgram/clients/onprem/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/onprem/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/onprem/v1/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/onprem/v1/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:39:38.826999 deepgram_sdk-3.2.7/deepgram/clients/prerecorded/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/prerecorded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/prerecorded/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/prerecorded/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/prerecorded/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:39:38.826999 deepgram_sdk-3.2.7/deepgram/clients/prerecorded/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/prerecorded/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12830 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/prerecorded/v1/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12762 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/prerecorded/v1/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/prerecorded/v1/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/prerecorded/v1/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21250 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/prerecorded/v1/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/read.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:39:38.826999 deepgram_sdk-3.2.7/deepgram/clients/speak/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/speak/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/speak/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/speak/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:39:38.830999 deepgram_sdk-3.2.7/deepgram/clients/speak/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/speak/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/speak/v1/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/speak/v1/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/speak/v1/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/speak/v1/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/clients/speak/v1/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/deepgram/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:39:38.830999 deepgram_sdk-3.2.7/deepgram_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12280 2024-04-24 20:39:38.000000 deepgram_sdk-3.2.7/deepgram_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-24 20:39:38.000000 deepgram_sdk-3.2.7/deepgram_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 20:39:38.000000 deepgram_sdk-3.2.7/deepgram_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-24 20:39:38.000000 deepgram_sdk-3.2.7/deepgram_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 20:39:38.000000 deepgram_sdk-3.2.7/deepgram_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 20:39:38.830999 deepgram_sdk-3.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-24 20:39:26.000000 deepgram_sdk-3.2.7/setup.py
```

### Comparing `deepgram_sdk-3.2.6/LICENSE` & `deepgram_sdk-3.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/PKG-INFO` & `deepgram_sdk-3.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepgram-sdk
-Version: 3.2.6
+Version: 3.2.7
 Summary: The official Python SDK for the Deepgram automated speech recognition platform.
 Home-page: https://github.com/deepgram/deepgram-python-sdk
 Author: Deepgram
 Author-email: devrel@deepgram.com
 License: MIT
 Keywords: deepgram,deepgram speech-to-text
 Classifier: Intended Audience :: Developers
@@ -91,15 +91,15 @@
 
 # Quickstarts
 
 This SDK aims to reduce complexity and abtract/hide some internal Deepgram details that clients shouldn't need to know about.  However you can still tweak options and settings if you need.
 
 ## PreRecorded Audio Transcription Quickstart
 
-You can find a [walkthrough](https://developers.deepgram.com/docs/pre-recorded-audio-transcription) on our documentation site. Transcribing Pre-Recorded Audio can be done using the following sample code:
+You can find a [walkthrough](https://developers.deepgram.com/docs/python-sdk-pre-recorded-transcription) on our documentation site. Transcribing Pre-Recorded Audio can be done using the following sample code:
 
 ```python
 AUDIO_URL = {
     "url": "https://static.deepgram.com/examples/Bueller-Life-moves-pretty-fast.wav"
 }
 
 # STEP 1 Create a Deepgram client using the API key from environment variables
```

### Comparing `deepgram_sdk-3.2.6/README.md` & `deepgram_sdk-3.2.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
 # Quickstarts
 
 This SDK aims to reduce complexity and abtract/hide some internal Deepgram details that clients shouldn't need to know about.  However you can still tweak options and settings if you need.
 
 ## PreRecorded Audio Transcription Quickstart
 
-You can find a [walkthrough](https://developers.deepgram.com/docs/pre-recorded-audio-transcription) on our documentation site. Transcribing Pre-Recorded Audio can be done using the following sample code:
+You can find a [walkthrough](https://developers.deepgram.com/docs/python-sdk-pre-recorded-transcription) on our documentation site. Transcribing Pre-Recorded Audio can be done using the following sample code:
 
 ```python
 AUDIO_URL = {
     "url": "https://static.deepgram.com/examples/Bueller-Life-moves-pretty-fast.wav"
 }
 
 # STEP 1 Create a Deepgram client using the API key from environment variables
```

### Comparing `deepgram_sdk-3.2.6/deepgram/__init__.py` & `deepgram_sdk-3.2.7/deepgram/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2023-2024 Deepgram SDK contributors. All Rights Reserved.
 # Use of this source code is governed by a MIT license that can be found in the LICENSE file.
 # SPDX-License-Identifier: MIT
 
 # version
-__version__ = "v3.2.6"
+__version__ = "v3.2.7"
 
 # entry point for the deepgram python sdk
 from .client import Deepgram, DeepgramClient
 from .options import DeepgramClientOptions, ClientOptionsFromEnv
 import logging, verboselogs
 
 # listen client
```

### Comparing `deepgram_sdk-3.2.6/deepgram/audio/microphone/errors.py` & `deepgram_sdk-3.2.7/deepgram/audio/microphone/errors.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/audio/microphone/microphone.py` & `deepgram_sdk-3.2.7/deepgram/audio/microphone/microphone.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/client.py` & `deepgram_sdk-3.2.7/deepgram/client.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/__init__.py` & `deepgram_sdk-3.2.7/deepgram/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/abstract_async_client.py` & `deepgram_sdk-3.2.7/deepgram/clients/abstract_async_client.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/abstract_sync_client.py` & `deepgram_sdk-3.2.7/deepgram/clients/abstract_sync_client.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/analyze/__init__.py` & `deepgram_sdk-3.2.7/deepgram/clients/analyze/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/analyze/client.py` & `deepgram_sdk-3.2.7/deepgram/clients/analyze/client.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/analyze/errors.py` & `deepgram_sdk-3.2.7/deepgram/clients/analyze/errors.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/analyze/v1/__init__.py` & `deepgram_sdk-3.2.7/deepgram/clients/analyze/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/analyze/v1/async_client.py` & `deepgram_sdk-3.2.7/deepgram/clients/analyze/v1/async_client.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/analyze/v1/client.py` & `deepgram_sdk-3.2.7/deepgram/clients/analyze/v1/client.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/analyze/v1/helpers.py` & `deepgram_sdk-3.2.7/deepgram/clients/analyze/v1/helpers.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/analyze/v1/options.py` & `deepgram_sdk-3.2.7/deepgram/clients/analyze/v1/options.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/analyze/v1/response.py` & `deepgram_sdk-3.2.7/deepgram/clients/analyze/v1/response.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/errors.py` & `deepgram_sdk-3.2.7/deepgram/clients/errors.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/helpers.py` & `deepgram_sdk-3.2.7/deepgram/clients/helpers.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/listen.py` & `deepgram_sdk-3.2.7/deepgram/clients/listen.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/live/__init__.py` & `deepgram_sdk-3.2.7/deepgram/clients/live/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/live/client.py` & `deepgram_sdk-3.2.7/deepgram/clients/live/client.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/live/enums.py` & `deepgram_sdk-3.2.7/deepgram/clients/live/enums.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/live/errors.py` & `deepgram_sdk-3.2.7/deepgram/clients/live/errors.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/live/v1/__init__.py` & `deepgram_sdk-3.2.7/deepgram/clients/live/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/live/v1/async_client.py` & `deepgram_sdk-3.2.7/deepgram/clients/live/v1/async_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -279,14 +279,19 @@
 
             except websockets.exceptions.ConnectionClosedOK as e:
                 self.logger.notice(f"_listening({e.code}) exiting gracefully")
                 self.logger.debug("AsyncLiveClient._listening LEAVE")
                 return
 
             except websockets.exceptions.WebSocketException as e:
+                if e.code == 1000:
+                    self.logger.notice(f"_listening({e.code}) exiting gracefully")
+                    self.logger.debug("AsyncLiveClient._listening LEAVE")
+                    return
+
                 self.logger.error(
                     "WebSocketException in AsyncLiveClient._listening: %s", e
                 )
                 error: ErrorResponse = {
                     "type": "Exception",
                     "description": "WebSocketException in AsyncLiveClient._listening",
                     "message": f"{e}",
@@ -353,14 +358,19 @@
 
             except websockets.exceptions.ConnectionClosedOK as e:
                 self.logger.notice(f"_keep_alive({e.code}) exiting gracefully")
                 self.logger.debug("AsyncLiveClient._keep_alive LEAVE")
                 return
 
             except websockets.exceptions.WebSocketException as e:
+                if e.code == 1000:
+                    self.logger.notice(f"_keep_alive({e.code}) exiting gracefully")
+                    self.logger.debug("AsyncLiveClient._keep_alive LEAVE")
+                    return
+
                 self.logger.error(
                     "WebSocketException in AsyncLiveClient._keep_alive: %s", e
                 )
                 error: ErrorResponse = {
                     "type": "Exception",
                     "description": "WebSocketException in AsyncLiveClient._keep_alive",
                     "message": f"{e}",
@@ -415,19 +425,26 @@
             return False
 
         if self._socket is not None:
             try:
                 await self._socket.send(data)
             except websockets.exceptions.ConnectionClosedOK as e:
                 self.logger.notice(f"send() exiting gracefully: {e.code}")
-                self.logger.debug("AsyncLiveClient._keep_alive LEAVE")
+                self.logger.debug("AsyncLiveClient.send LEAVE")
                 if self.config.options.get("termination_exception_send") == "true":
                     raise
                 return True
             except websockets.exceptions.WebSocketException as e:
+                if e.code == 1000:
+                    self.logger.notice(f"send({e.code}) exiting gracefully")
+                    self.logger.debug("AsyncLiveClient.send LEAVE")
+                    if self.config.options.get("termination_exception_send") == "true":
+                        raise
+                    return True
+
                 self.logger.error("send() failed - WebSocketException: %s", str(e))
                 self.logger.spam("AsyncLiveClient.send LEAVE")
                 if self.config.options.get("termination_exception_send") == "true":
                     raise
                 return False
             except Exception as e:
                 self.logger.error("send() failed - Exception: %s", str(e))
@@ -465,16 +482,14 @@
             if self._listen_thread is not None:
                 self._listen_thread.cancel()
                 tasks.append(self._listen_thread)
 
             # Use asyncio.gather to wait for tasks to be cancelled
             await asyncio.gather(*filter(None, tasks), return_exceptions=True)
             self.logger.notice("threads joined")
-            self._listen_thread = None
-            self._keep_alive_thread = None
 
             self._socket = None
 
             self.logger.notice("finish succeeded")
             self.logger.spam("AsyncLiveClient.finish LEAVE")
             return True
```

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/live/v1/client.py` & `deepgram_sdk-3.2.7/deepgram/clients/live/v1/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
             # listening thread
             self._listen_thread = threading.Thread(target=self._listening)
             self._listen_thread.start()
 
             # keepalive thread
             if self.config.options.get("keepalive") == "true":
-                self.logger.notice("keepalive is disabled")
+                self.logger.notice("keepalive is enabled")
                 self._keep_alive_thread = threading.Thread(target=self._keep_alive)
                 self._keep_alive_thread.start()
             else:
                 self.logger.notice("keepalive is disabled")
                 self._keep_alive_thread = None
 
             # push open event
@@ -279,14 +279,19 @@
 
             except websockets.exceptions.ConnectionClosedOK as e:
                 self.logger.notice(f"_listening({e.code}) exiting gracefully")
                 self.logger.debug("LiveClient._listening LEAVE")
                 return
 
             except websockets.exceptions.WebSocketException as e:
+                if e.code == 1000:
+                    self.logger.notice(f"_listening({e.code}) exiting gracefully")
+                    self.logger.debug("LiveClient._listening LEAVE")
+                    return
+
                 self.logger.error(
                     "WebSocketException in AsyncLiveClient._listening: %s", e
                 )
                 error: ErrorResponse = {
                     "type": "Exception",
                     "description": "WebSocketException in LiveClient._listening",
                     "message": f"{e}",
@@ -353,14 +358,19 @@
 
             except websockets.exceptions.ConnectionClosedOK as e:
                 self.logger.notice(f"_keep_alive({e.code}) exiting gracefully")
                 self.logger.debug("LiveClient._keep_alive LEAVE")
                 return
 
             except websockets.exceptions.WebSocketException as e:
+                if e.code == 1000:
+                    self.logger.notice(f"_keep_alive({e.code}) exiting gracefully")
+                    self.logger.debug("LiveClient._keep_alive LEAVE")
+                    return
+
                 self.logger.error(
                     "WebSocketException in AsyncLiveClient._keep_alive: %s", e
                 )
                 error: ErrorResponse = {
                     "type": "Exception",
                     "description": "WebSocketException in LiveClient._keep_alive",
                     "message": f"{e}",
@@ -419,14 +429,23 @@
                 except websockets.exceptions.ConnectionClosedOK as e:
                     self.logger.notice(f"send() exiting gracefully: {e.code}")
                     self.logger.debug("LiveClient._keep_alive LEAVE")
                     if self.config.options.get("termination_exception_send") == "true":
                         raise
                     return True
                 except websockets.exceptions.WebSocketException as e:
+                    if e.code == 1000:
+                        self.logger.notice(f"send({e.code}) exiting gracefully")
+                        self.logger.debug("LiveClient.send LEAVE")
+                        if (
+                            self.config.options.get("termination_exception_send")
+                            == "true"
+                        ):
+                            raise
+                        return True
                     self.logger.error("send() failed - WebSocketException: %s", str(e))
                     self.logger.spam("LiveClient.send LEAVE")
                     if self.config.options.get("termination_exception_send") == "true":
                         raise
                     return False
                 except Exception as e:
                     self.logger.error("send() failed - Exception: %s", str(e))
@@ -453,20 +472,18 @@
         # signal exit
         self._signal_exit()
 
         # stop the threads
         self.logger.verbose("cancelling tasks...")
         if self._keep_alive_thread is not None:
             self._keep_alive_thread.join()
-            self._keep_alive_thread = None
         self.logger.notice("processing thread joined")
 
         if self._listen_thread is not None:
             self._listen_thread.join()
-            self._listen_thread = None
         self.logger.notice("listening thread joined")
 
         self._socket = None
 
         self.logger.notice("finish succeeded")
         self.logger.spam("LiveClient.finish LEAVE")
         return True
```

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/live/v1/options.py` & `deepgram_sdk-3.2.7/deepgram/clients/live/v1/options.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     keywords: Optional[Union[List[str], str]] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     language: Optional[str] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     model: Optional[str] = field(
-        default=None, metadata=config(exclude=lambda f: f is None)
+        default="nova-2", metadata=config(exclude=lambda f: f is None)
     )
     multichannel: Optional[bool] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     numerals: Optional[bool] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
```

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/live/v1/response.py` & `deepgram_sdk-3.2.7/deepgram/clients/live/v1/response.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/manage/__init__.py` & `deepgram_sdk-3.2.7/deepgram/clients/manage/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/manage/client.py` & `deepgram_sdk-3.2.7/deepgram/clients/manage/client.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/manage/v1/__init__.py` & `deepgram_sdk-3.2.7/deepgram/clients/manage/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/manage/v1/async_client.py` & `deepgram_sdk-3.2.7/deepgram/clients/manage/v1/async_client.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/manage/v1/client.py` & `deepgram_sdk-3.2.7/deepgram/clients/manage/v1/client.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/manage/v1/options.py` & `deepgram_sdk-3.2.7/deepgram/clients/manage/v1/options.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/manage/v1/response.py` & `deepgram_sdk-3.2.7/deepgram/clients/manage/v1/response.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/onprem/client.py` & `deepgram_sdk-3.2.7/deepgram/clients/onprem/client.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/onprem/v1/async_client.py` & `deepgram_sdk-3.2.7/deepgram/clients/onprem/v1/async_client.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/onprem/v1/client.py` & `deepgram_sdk-3.2.7/deepgram/clients/onprem/v1/client.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/prerecorded/__init__.py` & `deepgram_sdk-3.2.7/deepgram/clients/prerecorded/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/prerecorded/client.py` & `deepgram_sdk-3.2.7/deepgram/clients/prerecorded/client.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/prerecorded/errors.py` & `deepgram_sdk-3.2.7/deepgram/clients/prerecorded/errors.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/prerecorded/v1/__init__.py` & `deepgram_sdk-3.2.7/deepgram/clients/prerecorded/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/prerecorded/v1/async_client.py` & `deepgram_sdk-3.2.7/deepgram/clients/prerecorded/v1/async_client.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/prerecorded/v1/client.py` & `deepgram_sdk-3.2.7/deepgram/clients/prerecorded/v1/client.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/prerecorded/v1/helpers.py` & `deepgram_sdk-3.2.7/deepgram/clients/prerecorded/v1/helpers.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/prerecorded/v1/options.py` & `deepgram_sdk-3.2.7/deepgram/clients/prerecorded/v1/options.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     language: Optional[str] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     measurements: Optional[bool] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     model: Optional[str] = field(
-        default=None, metadata=config(exclude=lambda f: f is None)
+        default="nova-2", metadata=config(exclude=lambda f: f is None)
     )
     multichannel: Optional[bool] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     numerals: Optional[bool] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
```

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/prerecorded/v1/response.py` & `deepgram_sdk-3.2.7/deepgram/clients/prerecorded/v1/response.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/read.py` & `deepgram_sdk-3.2.7/deepgram/clients/read.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/speak/client.py` & `deepgram_sdk-3.2.7/deepgram/clients/speak/client.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/speak/errors.py` & `deepgram_sdk-3.2.7/deepgram/clients/speak/errors.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/speak/v1/async_client.py` & `deepgram_sdk-3.2.7/deepgram/clients/speak/v1/async_client.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/speak/v1/client.py` & `deepgram_sdk-3.2.7/deepgram/clients/speak/v1/client.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/speak/v1/options.py` & `deepgram_sdk-3.2.7/deepgram/clients/speak/v1/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     Contains all the options for the SpeakOptions.
 
     Reference:
     https://developers.deepgram.com/reference/text-to-speech-preview-api
     """
 
     model: Optional[str] = field(
-        default=None, metadata=config(exclude=lambda f: f is None)
+        default="aura-asteria-en", metadata=config(exclude=lambda f: f is None)
     )
     encoding: Optional[str] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     container: Optional[str] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
```

### Comparing `deepgram_sdk-3.2.6/deepgram/clients/speak/v1/response.py` & `deepgram_sdk-3.2.7/deepgram/clients/speak/v1/response.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/errors.py` & `deepgram_sdk-3.2.7/deepgram/errors.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram/options.py` & `deepgram_sdk-3.2.7/deepgram/options.py`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/deepgram_sdk.egg-info/PKG-INFO` & `deepgram_sdk-3.2.7/deepgram_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepgram-sdk
-Version: 3.2.6
+Version: 3.2.7
 Summary: The official Python SDK for the Deepgram automated speech recognition platform.
 Home-page: https://github.com/deepgram/deepgram-python-sdk
 Author: Deepgram
 Author-email: devrel@deepgram.com
 License: MIT
 Keywords: deepgram,deepgram speech-to-text
 Classifier: Intended Audience :: Developers
@@ -91,15 +91,15 @@
 
 # Quickstarts
 
 This SDK aims to reduce complexity and abtract/hide some internal Deepgram details that clients shouldn't need to know about.  However you can still tweak options and settings if you need.
 
 ## PreRecorded Audio Transcription Quickstart
 
-You can find a [walkthrough](https://developers.deepgram.com/docs/pre-recorded-audio-transcription) on our documentation site. Transcribing Pre-Recorded Audio can be done using the following sample code:
+You can find a [walkthrough](https://developers.deepgram.com/docs/python-sdk-pre-recorded-transcription) on our documentation site. Transcribing Pre-Recorded Audio can be done using the following sample code:
 
 ```python
 AUDIO_URL = {
     "url": "https://static.deepgram.com/examples/Bueller-Life-moves-pretty-fast.wav"
 }
 
 # STEP 1 Create a Deepgram client using the API key from environment variables
```

### Comparing `deepgram_sdk-3.2.6/deepgram_sdk.egg-info/SOURCES.txt` & `deepgram_sdk-3.2.7/deepgram_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/pyproject.toml` & `deepgram_sdk-3.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deepgram_sdk-3.2.6/setup.py` & `deepgram_sdk-3.2.7/setup.py`

 * *Files identical despite different names*

