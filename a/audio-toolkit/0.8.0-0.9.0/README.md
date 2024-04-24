# Comparing `tmp/audio_toolkit-0.8.0.tar.gz` & `tmp/audio_toolkit-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio_toolkit-0.8.0.tar", last modified: Wed Apr 17 08:57:08 2024, max compression
+gzip compressed data, was "audio_toolkit-0.9.0.tar", last modified: Wed Apr 17 09:02:57 2024, max compression
```

## Comparing `audio_toolkit-0.8.0.tar` & `audio_toolkit-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 khanh     (1004) asr      (10001)        0 2024-04-17 08:57:08.595770 audio_toolkit-0.8.0/
--rw-r--r--   0 khanh     (1004) asr      (10001)     1069 2024-04-04 09:00:44.000000 audio_toolkit-0.8.0/LICENSE
--rw-r--r--   0 khanh     (1004) asr      (10001)      426 2024-04-17 08:57:08.595770 audio_toolkit-0.8.0/PKG-INFO
--rw-r--r--   0 khanh     (1004) asr      (10001)      110 2024-04-04 09:00:44.000000 audio_toolkit-0.8.0/README.md
-drwxr-xr-x   0 khanh     (1004) asr      (10001)        0 2024-04-17 08:57:08.595770 audio_toolkit-0.8.0/audio_toolkit/
--rw-r--r--   0 khanh     (1004) asr      (10001)       50 2024-04-04 09:12:18.000000 audio_toolkit-0.8.0/audio_toolkit/__init__.py
--rw-r--r--   0 khanh     (1004) asr      (10001)     7702 2024-04-17 08:52:24.000000 audio_toolkit-0.8.0/audio_toolkit/audio_stats.py
-drwxr-xr-x   0 khanh     (1004) asr      (10001)        0 2024-04-17 08:57:08.595770 audio_toolkit-0.8.0/audio_toolkit.egg-info/
--rw-r--r--   0 khanh     (1004) asr      (10001)      426 2024-04-17 08:57:08.000000 audio_toolkit-0.8.0/audio_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 khanh     (1004) asr      (10001)      265 2024-04-17 08:57:08.000000 audio_toolkit-0.8.0/audio_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 khanh     (1004) asr      (10001)        1 2024-04-17 08:57:08.000000 audio_toolkit-0.8.0/audio_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 khanh     (1004) asr      (10001)       31 2024-04-17 08:57:08.000000 audio_toolkit-0.8.0/audio_toolkit.egg-info/requires.txt
--rw-r--r--   0 khanh     (1004) asr      (10001)       14 2024-04-17 08:57:08.000000 audio_toolkit-0.8.0/audio_toolkit.egg-info/top_level.txt
--rw-r--r--   0 khanh     (1004) asr      (10001)       38 2024-04-17 08:57:08.595770 audio_toolkit-0.8.0/setup.cfg
--rw-r--r--   0 khanh     (1004) asr      (10001)      818 2024-04-17 08:57:00.000000 audio_toolkit-0.8.0/setup.py
+drwxr-xr-x   0 khanh     (1004) asr      (10001)        0 2024-04-17 09:02:57.233595 audio_toolkit-0.9.0/
+-rw-r--r--   0 khanh     (1004) asr      (10001)     1069 2024-04-04 09:00:44.000000 audio_toolkit-0.9.0/LICENSE
+-rw-r--r--   0 khanh     (1004) asr      (10001)      426 2024-04-17 09:02:57.233595 audio_toolkit-0.9.0/PKG-INFO
+-rw-r--r--   0 khanh     (1004) asr      (10001)      110 2024-04-04 09:00:44.000000 audio_toolkit-0.9.0/README.md
+drwxr-xr-x   0 khanh     (1004) asr      (10001)        0 2024-04-17 09:02:57.229594 audio_toolkit-0.9.0/audio_toolkit/
+-rw-r--r--   0 khanh     (1004) asr      (10001)       50 2024-04-04 09:12:18.000000 audio_toolkit-0.9.0/audio_toolkit/__init__.py
+-rw-r--r--   0 khanh     (1004) asr      (10001)     7702 2024-04-17 08:52:24.000000 audio_toolkit-0.9.0/audio_toolkit/audio_stats.py
+drwxr-xr-x   0 khanh     (1004) asr      (10001)        0 2024-04-17 09:02:57.233595 audio_toolkit-0.9.0/audio_toolkit.egg-info/
+-rw-r--r--   0 khanh     (1004) asr      (10001)      426 2024-04-17 09:02:57.000000 audio_toolkit-0.9.0/audio_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 khanh     (1004) asr      (10001)      265 2024-04-17 09:02:57.000000 audio_toolkit-0.9.0/audio_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 khanh     (1004) asr      (10001)        1 2024-04-17 09:02:57.000000 audio_toolkit-0.9.0/audio_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 khanh     (1004) asr      (10001)       31 2024-04-17 09:02:57.000000 audio_toolkit-0.9.0/audio_toolkit.egg-info/requires.txt
+-rw-r--r--   0 khanh     (1004) asr      (10001)       14 2024-04-17 09:02:57.000000 audio_toolkit-0.9.0/audio_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 khanh     (1004) asr      (10001)       38 2024-04-17 09:02:57.233595 audio_toolkit-0.9.0/setup.cfg
+-rw-r--r--   0 khanh     (1004) asr      (10001)      614 2024-04-17 09:02:57.000000 audio_toolkit-0.9.0/setup.py
```

### Comparing `audio_toolkit-0.8.0/LICENSE` & `audio_toolkit-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `audio_toolkit-0.8.0/audio_toolkit/audio_stats.py` & `audio_toolkit-0.9.0/audio_toolkit/audio_stats.py`

 * *Files identical despite different names*

