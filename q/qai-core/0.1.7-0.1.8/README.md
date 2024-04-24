# Comparing `tmp/qai_core-0.1.7.tar.gz` & `tmp/qai_core-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qai_core-0.1.7.tar", max compression
+gzip compressed data, was "qai_core-0.1.8.tar", max compression
```

## Comparing `qai_core-0.1.7.tar` & `qai_core-0.1.8.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0       46 2024-01-09 22:46:54.394446 qai_core-0.1.7/README.md
--rw-r--r--   0        0        0      358 2024-02-13 23:00:20.223300 qai_core-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      120 2024-02-08 16:38:24.567686 qai_core-0.1.7/qcore/__init__.py
--rw-r--r--   0        0        0    10738 2024-02-09 20:20:46.352722 qai_core-0.1.7/qcore/meta.py
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 qai_core-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       46 2024-02-10 04:57:58.583991 qai_core-0.1.8/README.md
+-rw-r--r--   0        0        0      389 2024-04-24 02:32:00.862774 qai_core-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      182 2024-02-14 16:52:33.551102 qai_core-0.1.8/src/qai/core/__init__.py
+-rw-r--r--   0        0        0      527 2024-02-11 05:30:15.864404 qai_core-0.1.8/src/qai/core/message.py
+-rw-r--r--   0        0        0    16829 2024-02-27 19:52:58.047418 qai_core-0.1.8/src/qai/core/meta.py
+-rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 qai_core-0.1.8/PKG-INFO
```

