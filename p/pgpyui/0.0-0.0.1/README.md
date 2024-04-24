# Comparing `tmp/pgpyui-0.0.tar.gz` & `tmp/pgpyui-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgpyui-0.0.tar", last modified: Tue Apr 23 17:27:07 2024, max compression
+gzip compressed data, was "pgpyui-0.0.1.tar", last modified: Wed Apr 24 14:09:13 2024, max compression
```

## Comparing `pgpyui-0.0.tar` & `pgpyui-0.0.1.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 17:27:07.011524 pgpyui-0.0/
--rw-rw-rw-   0        0        0      181 2024-04-23 17:27:07.011524 pgpyui-0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-23 17:27:07.002098 pgpyui-0.0/pgpyui/
--rw-rw-rw-   0        0        0     8339 2024-04-23 17:22:12.000000 pgpyui-0.0/pgpyui/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:27:07.009620 pgpyui-0.0/pgpyui.egg-info/
--rw-rw-rw-   0        0        0      181 2024-04-23 17:27:06.000000 pgpyui-0.0/pgpyui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2024-04-23 17:27:06.000000 pgpyui-0.0/pgpyui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 17:27:06.000000 pgpyui-0.0/pgpyui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-23 17:27:06.000000 pgpyui-0.0/pgpyui.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2024-04-23 17:27:06.000000 pgpyui-0.0/pgpyui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 17:27:07.013523 pgpyui-0.0/setup.cfg
--rw-rw-rw-   0        0        0      275 2024-04-23 17:21:49.000000 pgpyui-0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:09:13.391296 pgpyui-0.0.1/
+-rw-rw-rw-   0        0        0     2249 2024-04-24 14:09:13.391296 pgpyui-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1669 2024-04-24 13:59:43.000000 pgpyui-0.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 14:09:13.372306 pgpyui-0.0.1/pgpyui/
+-rw-rw-rw-   0        0        0      149 2024-04-24 13:50:35.000000 pgpyui-0.0.1/pgpyui/__init__.py
+-rw-rw-rw-   0        0        0     2296 2024-04-24 13:49:49.000000 pgpyui-0.0.1/pgpyui/button.py
+-rw-rw-rw-   0        0        0     5498 2024-04-24 13:50:25.000000 pgpyui-0.0.1/pgpyui/textarea.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:09:13.390294 pgpyui-0.0.1/pgpyui.egg-info/
+-rw-rw-rw-   0        0        0     2249 2024-04-24 14:09:13.000000 pgpyui-0.0.1/pgpyui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2024-04-24 14:09:13.000000 pgpyui-0.0.1/pgpyui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 14:09:13.000000 pgpyui-0.0.1/pgpyui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-24 14:09:13.000000 pgpyui-0.0.1/pgpyui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-24 14:09:13.000000 pgpyui-0.0.1/pgpyui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 14:09:13.393297 pgpyui-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      822 2024-04-24 14:09:08.000000 pgpyui-0.0.1/setup.py
```

