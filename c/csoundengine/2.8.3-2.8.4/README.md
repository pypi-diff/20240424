# Comparing `tmp/csoundengine-2.8.3.tar.gz` & `tmp/csoundengine-2.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csoundengine-2.8.3.tar", last modified: Fri Apr 19 13:24:18 2024, max compression
+gzip compressed data, was "csoundengine-2.8.4.tar", last modified: Tue Apr 23 22:14:15 2024, max compression
```

## Comparing `csoundengine-2.8.3.tar` & `csoundengine-2.8.4.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-19 13:24:18.604920 csoundengine-2.8.3/
--rw-rw-r--   0 em        (1000) em        (1000)    35128 2021-11-13 21:37:59.000000 csoundengine-2.8.3/LICENSE.txt
--rw-rw-r--   0 em        (1000) em        (1000)       24 2021-11-13 21:37:59.000000 csoundengine-2.8.3/MANIFEST.in
--rw-r--r--   0 em        (1000) em        (1000)     6716 2024-04-19 13:24:18.604920 csoundengine-2.8.3/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)     5728 2024-01-10 12:24:51.000000 csoundengine-2.8.3/README.rst
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-19 13:24:18.586920 csoundengine-2.8.3/csoundengine/
--rw-r--r--   0 em        (1000) em        (1000)     4112 2024-04-19 12:36:50.000000 csoundengine-2.8.3/csoundengine/__init__.py
--rw-rw-r--   0 em        (1000) em        (1000)     1055 2023-03-14 09:38:54.000000 csoundengine-2.8.3/csoundengine/__sessionbase.py
--rw-r--r--   0 em        (1000) em        (1000)      177 2023-11-24 08:20:24.000000 csoundengine-2.8.3/csoundengine/_common.py
--rw-r--r--   0 em        (1000) em        (1000)     5978 2023-11-14 20:14:02.000000 csoundengine-2.8.3/csoundengine/abstractrenderer.py
--rw-r--r--   0 em        (1000) em        (1000)    11621 2024-02-21 14:58:04.000000 csoundengine-2.8.3/csoundengine/baseschedevent.py
--rw-rw-r--   0 em        (1000) em        (1000)     5848 2024-04-17 08:24:25.000000 csoundengine-2.8.3/csoundengine/busproxy.py
--rw-r--r--   0 em        (1000) em        (1000)     8213 2024-04-03 07:08:12.000000 csoundengine-2.8.3/csoundengine/config.py
--rw-rw-r--   0 em        (1000) em        (1000)        0 2023-10-17 11:02:49.000000 csoundengine-2.8.3/csoundengine/contants.py
--rwxr-xr-x   0 em        (1000) em        (1000)   126875 2024-04-19 12:01:57.000000 csoundengine-2.8.3/csoundengine/csoundlib.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-19 13:24:18.579920 csoundengine-2.8.3/csoundengine/data/
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-19 13:24:18.579920 csoundengine-2.8.3/csoundengine/data/plugins6/
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-19 13:24:18.589920 csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/
--rw-rw-r--   0 em        (1000) em        (1000)    31400 2024-04-03 07:40:27.000000 csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/libbeosc.so
--rw-rw-r--   0 em        (1000) em        (1000)   130864 2024-04-03 07:40:27.000000 csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/libelse.so
--rw-rw-r--   0 em        (1000) em        (1000)   346592 2024-04-03 07:40:27.000000 csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/libjsfx.so
--rw-rw-r--   0 em        (1000) em        (1000)   108568 2024-04-03 07:40:27.000000 csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/libklib.so
--rw-rw-r--   0 em        (1000) em        (1000)    28312 2024-04-03 07:40:27.000000 csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/libpathtools.so
--rw-rw-r--   0 em        (1000) em        (1000)    31624 2024-04-03 07:40:27.000000 csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/libpoly.so
--rw-rw-r--   0 em        (1000) em        (1000)    18392 2024-04-03 07:40:27.000000 csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/librisset.so
--rw-rw-r--   0 em        (1000) em        (1000)    18616 2024-04-03 07:40:27.000000 csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/libsndmeta.so
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-19 13:24:18.592920 csoundengine-2.8.3/csoundengine/data/plugins6/macos-arm64/
--rw-rw-r--   0 em        (1000) em        (1000)    67147 2024-04-03 07:40:28.000000 csoundengine-2.8.3/csoundengine/data/plugins6/macos-arm64/libbeosc.dylib
--rw-rw-r--   0 em        (1000) em        (1000)   122938 2024-04-03 07:40:28.000000 csoundengine-2.8.3/csoundengine/data/plugins6/macos-arm64/libelse.dylib
--rw-rw-r--   0 em        (1000) em        (1000)   104074 2024-04-03 07:40:28.000000 csoundengine-2.8.3/csoundengine/data/plugins6/macos-arm64/libklib.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    51231 2024-04-03 07:40:28.000000 csoundengine-2.8.3/csoundengine/data/plugins6/macos-arm64/libpathtools.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    67578 2024-04-03 07:40:28.000000 csoundengine-2.8.3/csoundengine/data/plugins6/macos-arm64/libpoly.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    50588 2024-04-03 07:40:28.000000 csoundengine-2.8.3/csoundengine/data/plugins6/macos-arm64/librisset.dylib
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-19 13:24:18.595920 csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/
--rw-rw-r--   0 em        (1000) em        (1000)    66544 2024-04-03 07:40:29.000000 csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/libbeosc.dylib
--rw-rw-r--   0 em        (1000) em        (1000)   138896 2024-04-03 07:40:29.000000 csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/libelse.dylib
--rw-rw-r--   0 em        (1000) em        (1000)   483304 2024-04-03 07:40:29.000000 csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/libjsfx.dylib
--rw-rw-r--   0 em        (1000) em        (1000)   103560 2024-04-03 07:40:29.000000 csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/libklib.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    50784 2024-04-03 07:40:29.000000 csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/libpathtools.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    67016 2024-04-03 07:40:29.000000 csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/libpoly.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    50056 2024-04-03 07:40:29.000000 csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/librisset.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    50080 2024-04-03 07:40:29.000000 csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/libsndmeta.dylib
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-19 13:24:18.596920 csoundengine-2.8.3/csoundengine/data/plugins6/windows-x86_64/
--rw-rw-r--   0 em        (1000) em        (1000)    45568 2024-04-03 07:40:29.000000 csoundengine-2.8.3/csoundengine/data/plugins6/windows-x86_64/beosc.dll
--rw-rw-r--   0 em        (1000) em        (1000)    98304 2024-04-03 07:40:29.000000 csoundengine-2.8.3/csoundengine/data/plugins6/windows-x86_64/else.dll
--rw-rw-r--   0 em        (1000) em        (1000)    60928 2024-04-03 07:40:29.000000 csoundengine-2.8.3/csoundengine/data/plugins6/windows-x86_64/klib.dll
--rw-rw-r--   0 em        (1000) em        (1000)    18432 2024-04-03 07:40:29.000000 csoundengine-2.8.3/csoundengine/data/plugins6/windows-x86_64/pathtools.dll
--rw-rw-r--   0 em        (1000) em        (1000)    24576 2024-04-03 07:40:29.000000 csoundengine-2.8.3/csoundengine/data/plugins6/windows-x86_64/poly.dll
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-19 13:24:18.579920 csoundengine-2.8.3/csoundengine/data/plugins7/
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-19 13:24:18.598920 csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/
--rw-rw-r--   0 em        (1000) em        (1000)    31400 2024-04-03 07:40:30.000000 csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/libbeosc.so
--rw-rw-r--   0 em        (1000) em        (1000)   130864 2024-04-03 07:40:30.000000 csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/libelse.so
--rw-rw-r--   0 em        (1000) em        (1000)   346592 2024-04-03 07:40:30.000000 csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/libjsfx.so
--rw-rw-r--   0 em        (1000) em        (1000)   108568 2024-04-03 07:40:30.000000 csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/libklib.so
--rw-rw-r--   0 em        (1000) em        (1000)    28312 2024-04-03 07:40:30.000000 csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/libpathtools.so
--rw-rw-r--   0 em        (1000) em        (1000)    31624 2024-04-03 07:40:30.000000 csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/libpoly.so
--rw-rw-r--   0 em        (1000) em        (1000)    18392 2024-04-03 07:40:30.000000 csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/librisset.so
--rw-rw-r--   0 em        (1000) em        (1000)    18616 2024-04-03 07:40:30.000000 csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/libsndmeta.so
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-19 13:24:18.601920 csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/
--rw-rw-r--   0 em        (1000) em        (1000)    66544 2024-04-03 07:40:31.000000 csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/libbeosc.dylib
--rw-rw-r--   0 em        (1000) em        (1000)   138896 2024-04-03 07:40:31.000000 csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/libelse.dylib
--rw-rw-r--   0 em        (1000) em        (1000)   483304 2024-04-03 07:40:31.000000 csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/libjsfx.dylib
--rw-rw-r--   0 em        (1000) em        (1000)   103560 2024-04-03 07:40:31.000000 csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/libklib.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    50784 2024-04-03 07:40:31.000000 csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/libpathtools.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    67016 2024-04-03 07:40:31.000000 csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/libpoly.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    50056 2024-04-03 07:40:31.000000 csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/librisset.dylib
--rw-rw-r--   0 em        (1000) em        (1000)    50080 2024-04-03 07:40:31.000000 csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/libsndmeta.dylib
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-19 13:24:18.602920 csoundengine-2.8.3/csoundengine/data/plugins7/windows-x86_64/
--rw-rw-r--   0 em        (1000) em        (1000)    45568 2024-04-03 07:40:32.000000 csoundengine-2.8.3/csoundengine/data/plugins7/windows-x86_64/beosc.dll
--rw-rw-r--   0 em        (1000) em        (1000)    98304 2024-04-03 07:40:32.000000 csoundengine-2.8.3/csoundengine/data/plugins7/windows-x86_64/else.dll
--rw-rw-r--   0 em        (1000) em        (1000)    60928 2024-04-03 07:40:32.000000 csoundengine-2.8.3/csoundengine/data/plugins7/windows-x86_64/klib.dll
--rw-rw-r--   0 em        (1000) em        (1000)    18432 2024-04-03 07:40:32.000000 csoundengine-2.8.3/csoundengine/data/plugins7/windows-x86_64/pathtools.dll
--rw-rw-r--   0 em        (1000) em        (1000)    24576 2024-04-03 07:40:32.000000 csoundengine-2.8.3/csoundengine/data/plugins7/windows-x86_64/poly.dll
--rw-rw-r--   0 em        (1000) em        (1000)    13367 2024-04-19 12:39:25.000000 csoundengine-2.8.3/csoundengine/dependencies.py
--rwxr-xr-x   0 em        (1000) em        (1000)   154239 2024-04-18 20:01:10.000000 csoundengine-2.8.3/csoundengine/engine.py
--rw-r--r--   0 em        (1000) em        (1000)    24396 2024-04-17 08:14:41.000000 csoundengine-2.8.3/csoundengine/engineorc.py
--rw-rw-r--   0 em        (1000) em        (1000)      145 2023-10-11 21:51:48.000000 csoundengine-2.8.3/csoundengine/errors.py
--rw-r--r--   0 em        (1000) em        (1000)     2686 2024-04-18 10:55:30.000000 csoundengine-2.8.3/csoundengine/event.py
--rw-r--r--   0 em        (1000) em        (1000)    41738 2024-04-18 11:00:12.000000 csoundengine-2.8.3/csoundengine/instr.py
--rw-r--r--   0 em        (1000) em        (1000)    12223 2024-04-03 10:31:58.000000 csoundengine-2.8.3/csoundengine/instrtools.py
--rw-r--r--   0 em        (1000) em        (1000)    10720 2023-11-14 20:14:02.000000 csoundengine-2.8.3/csoundengine/interact.py
--rw-r--r--   0 em        (1000) em        (1000)    21429 2024-04-10 06:06:37.000000 csoundengine-2.8.3/csoundengine/internal.py
--rw-r--r--   0 em        (1000) em        (1000)     4997 2023-11-14 20:14:02.000000 csoundengine-2.8.3/csoundengine/jacktools.py
--rw-rw-r--   0 em        (1000) em        (1000)     3121 2023-10-26 22:00:07.000000 csoundengine-2.8.3/csoundengine/jupytertools.py
--rw-r--r--   0 em        (1000) em        (1000)     4517 2024-04-17 08:24:52.000000 csoundengine-2.8.3/csoundengine/linuxaudio.py
--rw-r--r--   0 em        (1000) em        (1000)     5815 2023-11-14 20:14:02.000000 csoundengine-2.8.3/csoundengine/magic.py
--rw-r--r--   0 em        (1000) em        (1000)    69729 2024-04-18 20:08:09.000000 csoundengine-2.8.3/csoundengine/offline.py
--rw-rw-r--   0 em        (1000) em        (1000)     5690 2023-11-01 14:45:02.000000 csoundengine-2.8.3/csoundengine/offlineorc.py
--rw-rw-r--   0 em        (1000) em        (1000)     6007 2023-10-11 21:51:48.000000 csoundengine-2.8.3/csoundengine/paramtable.py
--rwxrwxr-x   0 em        (1000) em        (1000)     7787 2024-04-17 07:56:12.000000 csoundengine-2.8.3/csoundengine/plotting.py
--rw-rw-r--   0 em        (1000) em        (1000)        0 2021-11-13 21:37:59.000000 csoundengine-2.8.3/csoundengine/py.typed
--rw-r--r--   0 em        (1000) em        (1000)    14940 2024-02-25 13:29:47.000000 csoundengine-2.8.3/csoundengine/schedevent.py
--rw-r--r--   0 em        (1000) em        (1000)    87296 2024-04-18 19:40:51.000000 csoundengine-2.8.3/csoundengine/session.py
--rw-rw-r--   0 em        (1000) em        (1000)      779 2024-03-28 17:26:41.000000 csoundengine-2.8.3/csoundengine/sessionhandler.py
--rw-r--r--   0 em        (1000) em        (1000)     6917 2024-02-29 10:28:35.000000 csoundengine-2.8.3/csoundengine/sessioninstrs.py
--rw-rw-r--   0 em        (1000) em        (1000)     1996 2024-04-19 11:09:00.000000 csoundengine-2.8.3/csoundengine/state.py
--rw-r--r--   0 em        (1000) em        (1000)    35051 2024-04-18 20:04:42.000000 csoundengine-2.8.3/csoundengine/synth.py
--rw-r--r--   0 em        (1000) em        (1000)     5965 2023-11-14 20:14:02.000000 csoundengine-2.8.3/csoundengine/tableproxy.py
--rw-rw-r--   0 em        (1000) em        (1000)      600 2022-09-25 13:10:18.000000 csoundengine-2.8.3/csoundengine/termui.py
--rw-rw-r--   0 em        (1000) em        (1000)     3101 2024-04-16 11:20:08.000000 csoundengine-2.8.3/csoundengine/tools.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-19 13:24:18.604920 csoundengine-2.8.3/csoundengine.egg-info/
--rw-r--r--   0 em        (1000) em        (1000)     6716 2024-04-19 13:24:18.000000 csoundengine-2.8.3/csoundengine.egg-info/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)     3778 2024-04-19 13:24:18.000000 csoundengine-2.8.3/csoundengine.egg-info/SOURCES.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2024-04-19 13:24:18.000000 csoundengine-2.8.3/csoundengine.egg-info/dependency_links.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2022-02-17 19:50:17.000000 csoundengine-2.8.3/csoundengine.egg-info/not-zip-safe
--rw-rw-r--   0 em        (1000) em        (1000)      259 2024-04-19 13:24:18.000000 csoundengine-2.8.3/csoundengine.egg-info/requires.txt
--rw-rw-r--   0 em        (1000) em        (1000)       13 2024-04-19 13:24:18.000000 csoundengine-2.8.3/csoundengine.egg-info/top_level.txt
--rw-rw-r--   0 em        (1000) em        (1000)       38 2024-04-19 13:24:18.604920 csoundengine-2.8.3/setup.cfg
--rwxrwxr-x   0 em        (1000) em        (1000)     1725 2024-04-19 13:21:08.000000 csoundengine-2.8.3/setup.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-19 13:24:18.603920 csoundengine-2.8.3/test/
--rw-rw-r--   0 em        (1000) em        (1000)      548 2023-09-17 06:41:11.000000 csoundengine-2.8.3/test/test1.py
--rw-rw-r--   0 em        (1000) em        (1000)      642 2024-02-23 13:40:16.000000 csoundengine-2.8.3/test/test2.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-23 22:14:15.285878 csoundengine-2.8.4/
+-rw-rw-r--   0 em        (1000) em        (1000)    35128 2021-11-13 21:37:59.000000 csoundengine-2.8.4/LICENSE.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       24 2021-11-13 21:37:59.000000 csoundengine-2.8.4/MANIFEST.in
+-rw-r--r--   0 em        (1000) em        (1000)     6716 2024-04-23 22:14:15.284878 csoundengine-2.8.4/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)     5728 2024-01-10 12:24:51.000000 csoundengine-2.8.4/README.rst
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-23 22:14:15.251878 csoundengine-2.8.4/csoundengine/
+-rw-r--r--   0 em        (1000) em        (1000)     4112 2024-04-19 12:36:50.000000 csoundengine-2.8.4/csoundengine/__init__.py
+-rw-rw-r--   0 em        (1000) em        (1000)     1055 2023-03-14 09:38:54.000000 csoundengine-2.8.4/csoundengine/__sessionbase.py
+-rw-r--r--   0 em        (1000) em        (1000)      177 2023-11-24 08:20:24.000000 csoundengine-2.8.4/csoundengine/_common.py
+-rw-r--r--   0 em        (1000) em        (1000)     5977 2024-04-23 21:51:02.000000 csoundengine-2.8.4/csoundengine/abstractrenderer.py
+-rw-r--r--   0 em        (1000) em        (1000)    11621 2024-02-21 14:58:04.000000 csoundengine-2.8.4/csoundengine/baseschedevent.py
+-rw-rw-r--   0 em        (1000) em        (1000)     5848 2024-04-17 08:24:25.000000 csoundengine-2.8.4/csoundengine/busproxy.py
+-rw-r--r--   0 em        (1000) em        (1000)     8213 2024-04-03 07:08:12.000000 csoundengine-2.8.4/csoundengine/config.py
+-rw-rw-r--   0 em        (1000) em        (1000)        0 2023-10-17 11:02:49.000000 csoundengine-2.8.4/csoundengine/contants.py
+-rwxr-xr-x   0 em        (1000) em        (1000)   126875 2024-04-19 12:01:57.000000 csoundengine-2.8.4/csoundengine/csoundlib.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-23 22:14:15.235877 csoundengine-2.8.4/csoundengine/data/
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-23 22:14:15.235877 csoundengine-2.8.4/csoundengine/data/plugins6/
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-23 22:14:15.256878 csoundengine-2.8.4/csoundengine/data/plugins6/linux-x86_64/
+-rw-rw-r--   0 em        (1000) em        (1000)    31400 2024-04-03 07:40:27.000000 csoundengine-2.8.4/csoundengine/data/plugins6/linux-x86_64/libbeosc.so
+-rw-rw-r--   0 em        (1000) em        (1000)   130864 2024-04-03 07:40:27.000000 csoundengine-2.8.4/csoundengine/data/plugins6/linux-x86_64/libelse.so
+-rw-rw-r--   0 em        (1000) em        (1000)   346592 2024-04-03 07:40:27.000000 csoundengine-2.8.4/csoundengine/data/plugins6/linux-x86_64/libjsfx.so
+-rw-rw-r--   0 em        (1000) em        (1000)   108568 2024-04-03 07:40:27.000000 csoundengine-2.8.4/csoundengine/data/plugins6/linux-x86_64/libklib.so
+-rw-rw-r--   0 em        (1000) em        (1000)    28312 2024-04-03 07:40:27.000000 csoundengine-2.8.4/csoundengine/data/plugins6/linux-x86_64/libpathtools.so
+-rw-rw-r--   0 em        (1000) em        (1000)    31624 2024-04-03 07:40:27.000000 csoundengine-2.8.4/csoundengine/data/plugins6/linux-x86_64/libpoly.so
+-rw-rw-r--   0 em        (1000) em        (1000)    18392 2024-04-03 07:40:27.000000 csoundengine-2.8.4/csoundengine/data/plugins6/linux-x86_64/librisset.so
+-rw-rw-r--   0 em        (1000) em        (1000)    18616 2024-04-03 07:40:27.000000 csoundengine-2.8.4/csoundengine/data/plugins6/linux-x86_64/libsndmeta.so
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-23 22:14:15.260878 csoundengine-2.8.4/csoundengine/data/plugins6/macos-arm64/
+-rw-rw-r--   0 em        (1000) em        (1000)    67147 2024-04-03 07:40:28.000000 csoundengine-2.8.4/csoundengine/data/plugins6/macos-arm64/libbeosc.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)   122938 2024-04-03 07:40:28.000000 csoundengine-2.8.4/csoundengine/data/plugins6/macos-arm64/libelse.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)   104074 2024-04-03 07:40:28.000000 csoundengine-2.8.4/csoundengine/data/plugins6/macos-arm64/libklib.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    51231 2024-04-03 07:40:28.000000 csoundengine-2.8.4/csoundengine/data/plugins6/macos-arm64/libpathtools.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    67578 2024-04-03 07:40:28.000000 csoundengine-2.8.4/csoundengine/data/plugins6/macos-arm64/libpoly.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    50588 2024-04-03 07:40:28.000000 csoundengine-2.8.4/csoundengine/data/plugins6/macos-arm64/librisset.dylib
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-23 22:14:15.268878 csoundengine-2.8.4/csoundengine/data/plugins6/macos-x86_64/
+-rw-rw-r--   0 em        (1000) em        (1000)    66544 2024-04-03 07:40:29.000000 csoundengine-2.8.4/csoundengine/data/plugins6/macos-x86_64/libbeosc.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)   138896 2024-04-03 07:40:29.000000 csoundengine-2.8.4/csoundengine/data/plugins6/macos-x86_64/libelse.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)   483304 2024-04-03 07:40:29.000000 csoundengine-2.8.4/csoundengine/data/plugins6/macos-x86_64/libjsfx.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)   103560 2024-04-03 07:40:29.000000 csoundengine-2.8.4/csoundengine/data/plugins6/macos-x86_64/libklib.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    50784 2024-04-03 07:40:29.000000 csoundengine-2.8.4/csoundengine/data/plugins6/macos-x86_64/libpathtools.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    67016 2024-04-03 07:40:29.000000 csoundengine-2.8.4/csoundengine/data/plugins6/macos-x86_64/libpoly.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    50056 2024-04-03 07:40:29.000000 csoundengine-2.8.4/csoundengine/data/plugins6/macos-x86_64/librisset.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    50080 2024-04-03 07:40:29.000000 csoundengine-2.8.4/csoundengine/data/plugins6/macos-x86_64/libsndmeta.dylib
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-23 22:14:15.270878 csoundengine-2.8.4/csoundengine/data/plugins6/windows-x86_64/
+-rw-rw-r--   0 em        (1000) em        (1000)    45568 2024-04-03 07:40:29.000000 csoundengine-2.8.4/csoundengine/data/plugins6/windows-x86_64/beosc.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    98304 2024-04-03 07:40:29.000000 csoundengine-2.8.4/csoundengine/data/plugins6/windows-x86_64/else.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    60928 2024-04-03 07:40:29.000000 csoundengine-2.8.4/csoundengine/data/plugins6/windows-x86_64/klib.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    18432 2024-04-03 07:40:29.000000 csoundengine-2.8.4/csoundengine/data/plugins6/windows-x86_64/pathtools.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    24576 2024-04-03 07:40:29.000000 csoundengine-2.8.4/csoundengine/data/plugins6/windows-x86_64/poly.dll
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-23 22:14:15.235877 csoundengine-2.8.4/csoundengine/data/plugins7/
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-23 22:14:15.275878 csoundengine-2.8.4/csoundengine/data/plugins7/linux-x86_64/
+-rw-rw-r--   0 em        (1000) em        (1000)    31400 2024-04-03 07:40:30.000000 csoundengine-2.8.4/csoundengine/data/plugins7/linux-x86_64/libbeosc.so
+-rw-rw-r--   0 em        (1000) em        (1000)   130864 2024-04-03 07:40:30.000000 csoundengine-2.8.4/csoundengine/data/plugins7/linux-x86_64/libelse.so
+-rw-rw-r--   0 em        (1000) em        (1000)   346592 2024-04-03 07:40:30.000000 csoundengine-2.8.4/csoundengine/data/plugins7/linux-x86_64/libjsfx.so
+-rw-rw-r--   0 em        (1000) em        (1000)   108568 2024-04-03 07:40:30.000000 csoundengine-2.8.4/csoundengine/data/plugins7/linux-x86_64/libklib.so
+-rw-rw-r--   0 em        (1000) em        (1000)    28312 2024-04-03 07:40:30.000000 csoundengine-2.8.4/csoundengine/data/plugins7/linux-x86_64/libpathtools.so
+-rw-rw-r--   0 em        (1000) em        (1000)    31624 2024-04-03 07:40:30.000000 csoundengine-2.8.4/csoundengine/data/plugins7/linux-x86_64/libpoly.so
+-rw-rw-r--   0 em        (1000) em        (1000)    18392 2024-04-03 07:40:30.000000 csoundengine-2.8.4/csoundengine/data/plugins7/linux-x86_64/librisset.so
+-rw-rw-r--   0 em        (1000) em        (1000)    18616 2024-04-03 07:40:30.000000 csoundengine-2.8.4/csoundengine/data/plugins7/linux-x86_64/libsndmeta.so
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-23 22:14:15.280878 csoundengine-2.8.4/csoundengine/data/plugins7/macos-x86_64/
+-rw-rw-r--   0 em        (1000) em        (1000)    66544 2024-04-03 07:40:31.000000 csoundengine-2.8.4/csoundengine/data/plugins7/macos-x86_64/libbeosc.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)   138896 2024-04-03 07:40:31.000000 csoundengine-2.8.4/csoundengine/data/plugins7/macos-x86_64/libelse.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)   483304 2024-04-03 07:40:31.000000 csoundengine-2.8.4/csoundengine/data/plugins7/macos-x86_64/libjsfx.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)   103560 2024-04-03 07:40:31.000000 csoundengine-2.8.4/csoundengine/data/plugins7/macos-x86_64/libklib.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    50784 2024-04-03 07:40:31.000000 csoundengine-2.8.4/csoundengine/data/plugins7/macos-x86_64/libpathtools.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    67016 2024-04-03 07:40:31.000000 csoundengine-2.8.4/csoundengine/data/plugins7/macos-x86_64/libpoly.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    50056 2024-04-03 07:40:31.000000 csoundengine-2.8.4/csoundengine/data/plugins7/macos-x86_64/librisset.dylib
+-rw-rw-r--   0 em        (1000) em        (1000)    50080 2024-04-03 07:40:31.000000 csoundengine-2.8.4/csoundengine/data/plugins7/macos-x86_64/libsndmeta.dylib
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-23 22:14:15.282878 csoundengine-2.8.4/csoundengine/data/plugins7/windows-x86_64/
+-rw-rw-r--   0 em        (1000) em        (1000)    45568 2024-04-03 07:40:32.000000 csoundengine-2.8.4/csoundengine/data/plugins7/windows-x86_64/beosc.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    98304 2024-04-03 07:40:32.000000 csoundengine-2.8.4/csoundengine/data/plugins7/windows-x86_64/else.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    60928 2024-04-03 07:40:32.000000 csoundengine-2.8.4/csoundengine/data/plugins7/windows-x86_64/klib.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    18432 2024-04-03 07:40:32.000000 csoundengine-2.8.4/csoundengine/data/plugins7/windows-x86_64/pathtools.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    24576 2024-04-03 07:40:32.000000 csoundengine-2.8.4/csoundengine/data/plugins7/windows-x86_64/poly.dll
+-rw-rw-r--   0 em        (1000) em        (1000)    13367 2024-04-19 12:39:25.000000 csoundengine-2.8.4/csoundengine/dependencies.py
+-rwxr-xr-x   0 em        (1000) em        (1000)   154239 2024-04-18 20:01:10.000000 csoundengine-2.8.4/csoundengine/engine.py
+-rw-r--r--   0 em        (1000) em        (1000)    24396 2024-04-17 08:14:41.000000 csoundengine-2.8.4/csoundengine/engineorc.py
+-rw-rw-r--   0 em        (1000) em        (1000)      145 2023-10-11 21:51:48.000000 csoundengine-2.8.4/csoundengine/errors.py
+-rw-r--r--   0 em        (1000) em        (1000)     2686 2024-04-18 10:55:30.000000 csoundengine-2.8.4/csoundengine/event.py
+-rw-r--r--   0 em        (1000) em        (1000)    41738 2024-04-18 11:00:12.000000 csoundengine-2.8.4/csoundengine/instr.py
+-rw-r--r--   0 em        (1000) em        (1000)    12225 2024-04-23 10:37:57.000000 csoundengine-2.8.4/csoundengine/instrtools.py
+-rw-r--r--   0 em        (1000) em        (1000)    10720 2023-11-14 20:14:02.000000 csoundengine-2.8.4/csoundengine/interact.py
+-rw-r--r--   0 em        (1000) em        (1000)    21429 2024-04-10 06:06:37.000000 csoundengine-2.8.4/csoundengine/internal.py
+-rw-r--r--   0 em        (1000) em        (1000)     4997 2023-11-14 20:14:02.000000 csoundengine-2.8.4/csoundengine/jacktools.py
+-rw-rw-r--   0 em        (1000) em        (1000)     3121 2023-10-26 22:00:07.000000 csoundengine-2.8.4/csoundengine/jupytertools.py
+-rw-r--r--   0 em        (1000) em        (1000)     4517 2024-04-17 08:24:52.000000 csoundengine-2.8.4/csoundengine/linuxaudio.py
+-rw-r--r--   0 em        (1000) em        (1000)     5815 2023-11-14 20:14:02.000000 csoundengine-2.8.4/csoundengine/magic.py
+-rw-r--r--   0 em        (1000) em        (1000)    70158 2024-04-23 21:52:31.000000 csoundengine-2.8.4/csoundengine/offline.py
+-rw-rw-r--   0 em        (1000) em        (1000)     5690 2023-11-01 14:45:02.000000 csoundengine-2.8.4/csoundengine/offlineorc.py
+-rw-rw-r--   0 em        (1000) em        (1000)     6007 2023-10-11 21:51:48.000000 csoundengine-2.8.4/csoundengine/paramtable.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     7787 2024-04-17 07:56:12.000000 csoundengine-2.8.4/csoundengine/plotting.py
+-rw-rw-r--   0 em        (1000) em        (1000)        0 2021-11-13 21:37:59.000000 csoundengine-2.8.4/csoundengine/py.typed
+-rw-r--r--   0 em        (1000) em        (1000)    14940 2024-02-25 13:29:47.000000 csoundengine-2.8.4/csoundengine/schedevent.py
+-rw-r--r--   0 em        (1000) em        (1000)    87796 2024-04-23 21:51:39.000000 csoundengine-2.8.4/csoundengine/session.py
+-rw-rw-r--   0 em        (1000) em        (1000)      779 2024-03-28 17:26:41.000000 csoundengine-2.8.4/csoundengine/sessionhandler.py
+-rw-r--r--   0 em        (1000) em        (1000)     8113 2024-04-23 21:31:04.000000 csoundengine-2.8.4/csoundengine/sessioninstrs.py
+-rw-rw-r--   0 em        (1000) em        (1000)     1996 2024-04-19 11:09:00.000000 csoundengine-2.8.4/csoundengine/state.py
+-rw-r--r--   0 em        (1000) em        (1000)    35051 2024-04-18 20:04:42.000000 csoundengine-2.8.4/csoundengine/synth.py
+-rw-r--r--   0 em        (1000) em        (1000)     5965 2023-11-14 20:14:02.000000 csoundengine-2.8.4/csoundengine/tableproxy.py
+-rw-rw-r--   0 em        (1000) em        (1000)      600 2022-09-25 13:10:18.000000 csoundengine-2.8.4/csoundengine/termui.py
+-rw-rw-r--   0 em        (1000) em        (1000)     3101 2024-04-16 11:20:08.000000 csoundengine-2.8.4/csoundengine/tools.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-23 22:14:15.284878 csoundengine-2.8.4/csoundengine.egg-info/
+-rw-r--r--   0 em        (1000) em        (1000)     6716 2024-04-23 22:14:15.000000 csoundengine-2.8.4/csoundengine.egg-info/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)     3778 2024-04-23 22:14:15.000000 csoundengine-2.8.4/csoundengine.egg-info/SOURCES.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2024-04-23 22:14:15.000000 csoundengine-2.8.4/csoundengine.egg-info/dependency_links.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2022-02-17 19:50:17.000000 csoundengine-2.8.4/csoundengine.egg-info/not-zip-safe
+-rw-rw-r--   0 em        (1000) em        (1000)      259 2024-04-23 22:14:15.000000 csoundengine-2.8.4/csoundengine.egg-info/requires.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       13 2024-04-23 22:14:15.000000 csoundengine-2.8.4/csoundengine.egg-info/top_level.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       38 2024-04-23 22:14:15.285878 csoundengine-2.8.4/setup.cfg
+-rwxrwxr-x   0 em        (1000) em        (1000)     1725 2024-04-23 22:13:57.000000 csoundengine-2.8.4/setup.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2024-04-23 22:14:15.284878 csoundengine-2.8.4/test/
+-rw-rw-r--   0 em        (1000) em        (1000)      548 2023-09-17 06:41:11.000000 csoundengine-2.8.4/test/test1.py
+-rw-rw-r--   0 em        (1000) em        (1000)      914 2024-04-19 14:03:08.000000 csoundengine-2.8.4/test/test2.py
```

### Comparing `csoundengine-2.8.3/LICENSE.txt` & `csoundengine-2.8.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/PKG-INFO` & `csoundengine-2.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csoundengine
-Version: 2.8.3
+Version: 2.8.4
 Summary: A synthesis framework using csound
 Home-page: https://github.com/gesellkammer/csoundengine
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
 License: BSD
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `csoundengine-2.8.3/README.rst` & `csoundengine-2.8.4/README.rst`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/__init__.py` & `csoundengine-2.8.4/csoundengine/__init__.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/__sessionbase.py` & `csoundengine-2.8.4/csoundengine/__sessionbase.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/abstractrenderer.py` & `csoundengine-2.8.4/csoundengine/abstractrenderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
                        for event in events]
         return SchedEventGroup(schedevents)
 
     @abstractmethod
     def playSample(self,
                    source: int | tableproxy.TableProxy | str | tuple[np.ndarray, int],
                    delay=0.,
-                   dur=-1.,
+                   dur=0.,
                    chan=1,
                    gain=1.,
                    speed=1.,
                    loop=False,
                    pan=0.5,
                    skip=0.,
                    fade: float | tuple[float, float] | None = None,
```

### Comparing `csoundengine-2.8.3/csoundengine/baseschedevent.py` & `csoundengine-2.8.4/csoundengine/baseschedevent.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/busproxy.py` & `csoundengine-2.8.4/csoundengine/busproxy.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/config.py` & `csoundengine-2.8.4/csoundengine/config.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/csoundlib.py` & `csoundengine-2.8.4/csoundengine/csoundlib.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/libbeosc.so` & `csoundengine-2.8.4/csoundengine/data/plugins6/linux-x86_64/libbeosc.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/libelse.so` & `csoundengine-2.8.4/csoundengine/data/plugins6/linux-x86_64/libelse.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/libjsfx.so` & `csoundengine-2.8.4/csoundengine/data/plugins6/linux-x86_64/libjsfx.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/libklib.so` & `csoundengine-2.8.4/csoundengine/data/plugins6/linux-x86_64/libklib.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/libpathtools.so` & `csoundengine-2.8.4/csoundengine/data/plugins6/linux-x86_64/libpathtools.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/libpoly.so` & `csoundengine-2.8.4/csoundengine/data/plugins6/linux-x86_64/libpoly.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/librisset.so` & `csoundengine-2.8.4/csoundengine/data/plugins6/linux-x86_64/librisset.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins6/linux-x86_64/libsndmeta.so` & `csoundengine-2.8.4/csoundengine/data/plugins6/linux-x86_64/libsndmeta.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins6/macos-arm64/libbeosc.dylib` & `csoundengine-2.8.4/csoundengine/data/plugins6/macos-arm64/libbeosc.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins6/macos-arm64/libelse.dylib` & `csoundengine-2.8.4/csoundengine/data/plugins6/macos-arm64/libelse.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins6/macos-arm64/libklib.dylib` & `csoundengine-2.8.4/csoundengine/data/plugins6/macos-arm64/libklib.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins6/macos-arm64/libpathtools.dylib` & `csoundengine-2.8.4/csoundengine/data/plugins6/macos-arm64/libpathtools.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins6/macos-arm64/libpoly.dylib` & `csoundengine-2.8.4/csoundengine/data/plugins6/macos-arm64/libpoly.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins6/macos-arm64/librisset.dylib` & `csoundengine-2.8.4/csoundengine/data/plugins6/macos-arm64/librisset.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/libbeosc.dylib` & `csoundengine-2.8.4/csoundengine/data/plugins6/macos-x86_64/libbeosc.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/libelse.dylib` & `csoundengine-2.8.4/csoundengine/data/plugins6/macos-x86_64/libelse.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/libjsfx.dylib` & `csoundengine-2.8.4/csoundengine/data/plugins6/macos-x86_64/libjsfx.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/libklib.dylib` & `csoundengine-2.8.4/csoundengine/data/plugins6/macos-x86_64/libklib.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/libpathtools.dylib` & `csoundengine-2.8.4/csoundengine/data/plugins6/macos-x86_64/libpathtools.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/libpoly.dylib` & `csoundengine-2.8.4/csoundengine/data/plugins6/macos-x86_64/libpoly.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/librisset.dylib` & `csoundengine-2.8.4/csoundengine/data/plugins6/macos-x86_64/librisset.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins6/macos-x86_64/libsndmeta.dylib` & `csoundengine-2.8.4/csoundengine/data/plugins6/macos-x86_64/libsndmeta.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins6/windows-x86_64/beosc.dll` & `csoundengine-2.8.4/csoundengine/data/plugins6/windows-x86_64/beosc.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins6/windows-x86_64/else.dll` & `csoundengine-2.8.4/csoundengine/data/plugins6/windows-x86_64/else.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins6/windows-x86_64/klib.dll` & `csoundengine-2.8.4/csoundengine/data/plugins6/windows-x86_64/klib.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins6/windows-x86_64/pathtools.dll` & `csoundengine-2.8.4/csoundengine/data/plugins6/windows-x86_64/pathtools.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins6/windows-x86_64/poly.dll` & `csoundengine-2.8.4/csoundengine/data/plugins6/windows-x86_64/poly.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/libbeosc.so` & `csoundengine-2.8.4/csoundengine/data/plugins7/linux-x86_64/libbeosc.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/libelse.so` & `csoundengine-2.8.4/csoundengine/data/plugins7/linux-x86_64/libelse.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/libjsfx.so` & `csoundengine-2.8.4/csoundengine/data/plugins7/linux-x86_64/libjsfx.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/libklib.so` & `csoundengine-2.8.4/csoundengine/data/plugins7/linux-x86_64/libklib.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/libpathtools.so` & `csoundengine-2.8.4/csoundengine/data/plugins7/linux-x86_64/libpathtools.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/libpoly.so` & `csoundengine-2.8.4/csoundengine/data/plugins7/linux-x86_64/libpoly.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/librisset.so` & `csoundengine-2.8.4/csoundengine/data/plugins7/linux-x86_64/librisset.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins7/linux-x86_64/libsndmeta.so` & `csoundengine-2.8.4/csoundengine/data/plugins7/linux-x86_64/libsndmeta.so`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/libbeosc.dylib` & `csoundengine-2.8.4/csoundengine/data/plugins7/macos-x86_64/libbeosc.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/libelse.dylib` & `csoundengine-2.8.4/csoundengine/data/plugins7/macos-x86_64/libelse.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/libjsfx.dylib` & `csoundengine-2.8.4/csoundengine/data/plugins7/macos-x86_64/libjsfx.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/libklib.dylib` & `csoundengine-2.8.4/csoundengine/data/plugins7/macos-x86_64/libklib.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/libpathtools.dylib` & `csoundengine-2.8.4/csoundengine/data/plugins7/macos-x86_64/libpathtools.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/libpoly.dylib` & `csoundengine-2.8.4/csoundengine/data/plugins7/macos-x86_64/libpoly.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/librisset.dylib` & `csoundengine-2.8.4/csoundengine/data/plugins7/macos-x86_64/librisset.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins7/macos-x86_64/libsndmeta.dylib` & `csoundengine-2.8.4/csoundengine/data/plugins7/macos-x86_64/libsndmeta.dylib`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins7/windows-x86_64/beosc.dll` & `csoundengine-2.8.4/csoundengine/data/plugins7/windows-x86_64/beosc.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins7/windows-x86_64/else.dll` & `csoundengine-2.8.4/csoundengine/data/plugins7/windows-x86_64/else.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins7/windows-x86_64/klib.dll` & `csoundengine-2.8.4/csoundengine/data/plugins7/windows-x86_64/klib.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins7/windows-x86_64/pathtools.dll` & `csoundengine-2.8.4/csoundengine/data/plugins7/windows-x86_64/pathtools.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/data/plugins7/windows-x86_64/poly.dll` & `csoundengine-2.8.4/csoundengine/data/plugins7/windows-x86_64/poly.dll`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/dependencies.py` & `csoundengine-2.8.4/csoundengine/dependencies.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/engine.py` & `csoundengine-2.8.4/csoundengine/engine.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/engineorc.py` & `csoundengine-2.8.4/csoundengine/engineorc.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/event.py` & `csoundengine-2.8.4/csoundengine/event.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/instr.py` & `csoundengine-2.8.4/csoundengine/instr.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/instrtools.py` & `csoundengine-2.8.4/csoundengine/instrtools.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,21 +122,21 @@
     line0 = 0
     line1 = 0
     delim = ''
     for i, line in enumerate(lines):
         line = line.strip()
         if not line:
             continue
-        if re.match(r'\|\s*[ik]\w+', line):
+        if re.match(r'\|\s*[ikS]\w+', line):
             if inlineArgsStarted:
                 raise ValueError(f"Invalid inline args: {lines}")
             line0 = i
             delim = '||'
             inlineArgsStarted = True
-        elif not inlineArgsStarted and re.match(r'\{\s*[ik]\w+', line):
+        elif not inlineArgsStarted and re.match(r'\{\s*[ikS]\w+', line):
             delim = '{}'
             line0 = i
             inlineArgsStarted = True
 
         if inlineArgsStarted and line.endswith('|'):
             line1 = i + 1
             assert delim == '||'
```

### Comparing `csoundengine-2.8.3/csoundengine/interact.py` & `csoundengine-2.8.4/csoundengine/interact.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/internal.py` & `csoundengine-2.8.4/csoundengine/internal.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/jacktools.py` & `csoundengine-2.8.4/csoundengine/jacktools.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/jupytertools.py` & `csoundengine-2.8.4/csoundengine/jupytertools.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/linuxaudio.py` & `csoundengine-2.8.4/csoundengine/linuxaudio.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/magic.py` & `csoundengine-2.8.4/csoundengine/magic.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/offline.py` & `csoundengine-2.8.4/csoundengine/offline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1047,14 +1047,18 @@
         endmarker = self._endMarker or endtime
         renderend = min(endtime, scoreend, endmarker) + tail
 
         if renderend == float('inf'):
             raise RenderError("Cannot render an infinite score. Set an endtime when calling "
                               ".render(...)")
         if renderend <= scorestart:
+            logger.error("Invalid render time. Score: ")
+            events = sorted(self.scheduledEvents.values(), key=lambda event: event.start)
+            for ev in events:
+                logger.error(f"    {event}")
             raise RenderError(f"No score to render (start: {scorestart}, end: {renderend})")
 
         if numthreads == 0:
             numthreads = config['rec_numthreads'] or config['numthreads']
 
         csd = self.csd.copy()
 
@@ -1354,15 +1358,15 @@
                               skiptime=skiptime)
         self._soundfileRegistry[path] = tabproxy
         return tabproxy
 
     def playSample(self,
                    source: int | str | TableProxy | tuple[np.ndarray, int],
                    delay=0.,
-                   dur=0,
+                   dur=0.,
                    chan=1,
                    gain=1.,
                    speed=1.,
                    loop=False,
                    pan=0.5,
                    skip=0.,
                    fade: float | tuple[float, float] | None = None,
@@ -1388,55 +1392,65 @@
                 multichannel samples panning is not taken into account at the moment
             gain: apply a gain to playback
             fade: fade-in / fade-out ramp, in seconds
             skip: playback does not start at the beginning of
                 the table but at `starttime`
             dur: duration of playback. -1=indefinite duration, will stop at the end of the
                 sample if no looping was set; 0=definite duration, the event is scheduled
-                with dur=sampledur/speed
+                with dur=sampledur/speed. Do not use this if you plan to modify or modulate
+                the playback speed.
             crossfade: if looping, this indicates the length of the crossfade
         """
         if loop and dur == 0:
-            logger.warning(f"playSample was called with loop=True, but the duration ({dur}) given "
-                           f"will result in no looping taking place")
-        if isinstance(source, tuple):
+            dur = -1
+
+        if isinstance(fade, (int, float)):
+            fadein = fadeout = fade
+        elif isinstance(fade, tuple):
+            fadein, fadeout = fade
+        elif fade is None:
+            fadein = fadeout = config['sample_fade_time']
+        else:
+            raise TypeError(f"fade should be None to use default, or a time or a tuple "
+                            f"(fadein, fadeout), got {fade}")
+
+        if isinstance(source, str):
+            source = os.path.abspath(source)
+            args = dict(
+                Spath=source,
+                ifadein=fadein,
+                ifadeout=fadeout,
+                iloop=int(loop),
+                kspeed=speed,
+                kpan=pan,
+                ichan=chan
+            )
+            if not loop and dur == 0:
+                info = sndfileio.sndinfo(source)
+                dur = info.duration / speed + fadeout
+            return self.sched('.diskin', delay=delay, dur=dur, args=args)
+
+        elif isinstance(source, tuple):
             assert len(source) == 2 and isinstance(source[0], np.ndarray)
             data, sr = source
             tabproxy = self.makeTable(data=source[0], sr=sr)
             tabnum = tabproxy.tabnum
             if dur == 0:
                 dur = (len(data)/sr) / speed
         elif isinstance(source, TableProxy):
             tabnum = source.tabnum
-        elif isinstance(source, str):
-            tabproxy = self.readSoundfile(path=source, delay=delay, skiptime=skip)
-            tabnum = tabproxy.tabnum
-            if dur == 0:
-                dur = tabproxy.duration() / speed
         elif isinstance(source, int):
             tabnum = source
-            if dur == 0:
-                dur = -1
         else:
             raise TypeError(f"Not a valid source: {source}, expected a TableProxy, "
                             f"path, table number or sample data as (samples, sr: int)")
         assert tabnum > 0
         if not loop:
             crossfade = -1
 
-        if isinstance(fade, (int, float)):
-            fadein = fadeout = fade
-        elif isinstance(fade, tuple):
-            fadein, fadeout = fade
-        elif fade is None:
-            fadein = fadeout = config['sample_fade_time']
-        else:
-            raise TypeError(f"fade should be None to use default, or a time or a tuple "
-                            f"(fadein, fadeout), got {fade}")
-
         args = dict(isndtab=tabnum, istart=skip,
                     ifadein=fadein, ifadeout=fadeout,
                     kchan=chan, kspeed=speed, kpan=pan, kgain=gain,
                     ixfade=crossfade)
         return self.sched('.playSample', delay=delay, dur=dur, args=args)
 
     def automate(self,
```

### Comparing `csoundengine-2.8.3/csoundengine/offlineorc.py` & `csoundengine-2.8.4/csoundengine/offlineorc.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/paramtable.py` & `csoundengine-2.8.4/csoundengine/paramtable.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/plotting.py` & `csoundengine-2.8.4/csoundengine/plotting.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/schedevent.py` & `csoundengine-2.8.4/csoundengine/schedevent.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/session.py` & `csoundengine-2.8.4/csoundengine/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -2041,15 +2041,15 @@
                                     kmaxbw=maxbw,
                                     kfreqoffset=freqoffset,
                                     kminamp=minamp))
 
     def playSample(self,
                    source: int | TableProxy | str | tuple[np.ndarray, int],
                    delay=0.,
-                   dur=-1.,
+                   dur=0.,
                    chan=1,
                    gain=1.,
                    speed=1.,
                    loop=False,
                    pan=0.5,
                    skip=0.,
                    fade: float | tuple[float, float] | None = None,
@@ -2058,28 +2058,29 @@
                    ) -> Synth:
 
         """
         Play a sample.
 
         This method ensures that the sample is played at the original pitch,
         independent of the current samplerate. The source can be a table,
-        a soundfile or a :class:`~csoundengine.tableproxy.TableProxy`
+        a soundfile or a :class:`~csoundengine.tableproxy.TableProxy`. If a path
+        to a soundfile is given, the 'diskin2' opcode is used by default
 
         Args:
             source: table number, a path to a sample or a TableProxy, or a tuple
-                (numpy array, samplerate)
+                (numpy array, samplerate).
             dur: the duration of playback (-1 to play until the end of the sample
-                or indefinitely if loop==True)
+                or indefinitely if loop==True).
             chan: the channel to play the sample to. In the case of multichannel
                   samples, this is the first channel
             pan: a value between 0-1. -1 means default, which is 0 for mono,
                 0.5 for stereo. For multichannel (3+) samples, panning is not
                 taken into account
             gain: gain factor.
-            speed: speed of playback
+            speed: speed of playback. Pitch will be changed as well.
             loop: True/False or -1 to loop as defined in the file itself (not all
                 file formats define loop points)
             delay: time to wait before playback starts
             skip: the starting playback time (0=play from beginning)
             fade: fade in/out in secods. None=default. Either a fade value or a tuple
                 (fadein, fadeout)
             crossfade: if looping, this indicates the length of the crossfade
@@ -2088,37 +2089,46 @@
         Returns:
             A Synth with the following mutable parameters: kgain, kspeed, kchan, kpan
 
         """
         if self.isRendering():
             raise RuntimeError("This Session is in rendering mode. Call .playSample on the renderer instead")
 
-        if isinstance(source, int):
+        if fade is None:
+            fadein = fadeout = config['sample_fade_time']
+        else:
+            fadein, fadeout = fade if isinstance(fade, tuple) else fade, fade
+
+        if loop and dur == 0:
+            dur = -1
+
+        if isinstance(source, str):
+            if not loop and dur == 0:
+                info = sndfileio.sndinfo(source)
+                dur = info.duration / speed + fadeout
+            return self.sched('.diskin',
+                              delay=delay,
+                              dur=dur,
+                              Spath=source,
+                              ifadein=fadein,
+                              ifadeout=fadeout,
+                              iloop=int(loop),
+                              kspeed=speed,
+                              kpan=pan,
+                              ichan=chan)
+        elif isinstance(source, int):
             tabnum = source
         elif isinstance(source, TableProxy):
             tabnum = source.tabnum
-        elif isinstance(source, str):
-            table = self.readSoundfile(source, block=blockread)
-            tabnum = table.tabnum
         elif isinstance(source, tuple) and isinstance(source[0], np.ndarray) and isinstance(source[1], int):
             table = self.makeTable(source[0], sr=source[1], unique=False, block=blockread)
             tabnum = table.tabnum
         else:
             raise TypeError(f"Expected table number as int, TableProxy, a path to a soundfile as str or a "
                             f"tuple (samples: np.ndarray, sr: int), got {source}")
-        # isndtab, iloop, istart, ifade
-        if fade is None:
-            fadein = fadeout = config['sample_fade_time']
-        else:
-            if isinstance(fade, tuple):
-                fadein, fadeout = fade
-            else:
-                fadein = fadeout = fade
-        if not loop:
-            crossfade = -1
 
         assert isinstance(tabnum, int) and tabnum >= 1
         return self.sched('.playSample',
                           delay=delay,
                           dur=dur,
                           args=dict(isndtab=tabnum,
                                     istart=skip,
```

### Comparing `csoundengine-2.8.3/csoundengine/sessionhandler.py` & `csoundengine-2.8.4/csoundengine/sessionhandler.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/sessioninstrs.py` & `csoundengine-2.8.4/csoundengine/sessioninstrs.py`

 * *Files 9% similar despite different names*

```diff
@@ -99,14 +99,44 @@
         endif   
         know += ionecycle * kspeed
         imaxtime = idur - ifadeout - ionecycle
         if iloop == 0 && know >= imaxtime then
             turnoff
         endif
     """, aliases={'speed': 'kspeed', 'gain': 'kgain', 'pan': 'kpan'}),
+    Instr('.diskin', body=r'''
+        |Spath, ichan=1, kgain=1, kspeed=1, kpan=-1, ifadein=0, ifadeout=0, iloop=0, istart=0, iwsize=4|
+        iformat = 0
+        know init 0
+        ionecycle = ksmps/sr
+        ifiledur = filelen(Spath)
+        idur = ifiledur / i(kspeed)
+        imaxtime = idur + ifadeout + ionecycle
+        aouts[] diskin2 Spath, kspeed, istart, iloop, iformat, iwsize
+        inumouts = lenarray(aouts)
+        aenv linsegr 0, ifadein, 1, ifadeout, 0
+        aenv *= interp(kgain)
+        aouts *= aenv
+        if inumouts == 1 then
+            kpan = kpan >= 0 ? kpan : 0.5
+            aL, aR pan2 aouts[0], kpan
+            outch ichan, aL, ichan+1, aR
+        elseif inumouts == 2 then
+            aL, aR panstereo aouts[0], aouts[1], kpan
+            outch ichan, aL, ichan+1, aR
+        else
+            ; panning is disabled for soundfiles with more than 2 channels
+            ichans[] genarray ichan, ichan+inumouts-1
+            poly0 inumouts, "outch", ichans, aouts
+        endif
+        know += ionecycle/kspeed 
+        if p3 < 0 && iloop == 0 && know > imaxtime then
+            turnoff
+        endif 
+    ''', aliases={'speed': 'kspeed', 'gain': 'kgain'}),
     Instr('.playbuf', body="""
         |itabnum=0, ioutchan=1, igain=1, iloop=0|
         inumsamps ftlen itabnum
         idur = inumsamps / ftsr(itabnum)
 
         if (iloop == 1) then
             iPitch = 1
```

### Comparing `csoundengine-2.8.3/csoundengine/state.py` & `csoundengine-2.8.4/csoundengine/state.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/synth.py` & `csoundengine-2.8.4/csoundengine/synth.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/tableproxy.py` & `csoundengine-2.8.4/csoundengine/tableproxy.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/termui.py` & `csoundengine-2.8.4/csoundengine/termui.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine/tools.py` & `csoundengine-2.8.4/csoundengine/tools.py`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/csoundengine.egg-info/PKG-INFO` & `csoundengine-2.8.4/csoundengine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csoundengine
-Version: 2.8.3
+Version: 2.8.4
 Summary: A synthesis framework using csound
 Home-page: https://github.com/gesellkammer/csoundengine
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
 License: BSD
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `csoundengine-2.8.3/csoundengine.egg-info/SOURCES.txt` & `csoundengine-2.8.4/csoundengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csoundengine-2.8.3/setup.py` & `csoundengine-2.8.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from setuptools import setup
 import os
 
-version = (2, 8, 3)
+version = (2, 8, 4)
 
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
```

### Comparing `csoundengine-2.8.3/test/test1.py` & `csoundengine-2.8.4/test/test1.py`

 * *Files identical despite different names*

