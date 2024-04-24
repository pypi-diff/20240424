# Comparing `tmp/evodict-0.1.tar.gz` & `tmp/evodict-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evodict-0.1.tar", last modified: Wed Apr 24 06:03:03 2024, max compression
+gzip compressed data, was "evodict-0.2.tar", last modified: Wed Apr 24 09:53:19 2024, max compression
```

## Comparing `evodict-0.1.tar` & `evodict-0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 06:03:03.110098 evodict-0.1/
-drwxrwxrwx   0        0        0        0 2024-04-24 06:03:03.110098 evodict-0.1/EvoDict.egg-info/
--rw-rw-rw-   0        0        0      289 2024-04-24 06:03:03.000000 evodict-0.1/EvoDict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2024-04-24 06:03:03.000000 evodict-0.1/EvoDict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 06:03:03.000000 evodict-0.1/EvoDict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-04-24 06:03:03.000000 evodict-0.1/EvoDict.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 06:03:03.000000 evodict-0.1/EvoDict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      289 2024-04-24 06:03:03.110098 evodict-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-24 06:03:03.110098 evodict-0.1/setup.cfg
--rw-rw-rw-   0        0        0      408 2024-04-24 06:01:16.000000 evodict-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 09:53:19.028166 evodict-0.2/
+drwxrwxrwx   0        0        0        0 2024-04-24 09:53:19.024631 evodict-0.2/EvoDict.egg-info/
+-rw-rw-rw-   0        0        0      245 2024-04-24 09:53:18.000000 evodict-0.2/EvoDict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2024-04-24 09:53:18.000000 evodict-0.2/EvoDict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 09:53:18.000000 evodict-0.2/EvoDict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-04-24 09:53:18.000000 evodict-0.2/EvoDict.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 09:53:18.000000 evodict-0.2/EvoDict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      245 2024-04-24 09:53:19.028166 evodict-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-24 09:53:19.028166 evodict-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      364 2024-04-24 09:52:26.000000 evodict-0.2/setup.py
```

