# Comparing `tmp/load_envfile-0.2.tar.gz` & `tmp/load_envfile-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "load_envfile-0.2.tar", last modified: Tue Apr 23 16:31:18 2024, max compression
+gzip compressed data, was "load_envfile-0.3.tar", last modified: Tue Apr 23 16:48:31 2024, max compression
```

## Comparing `load_envfile-0.2.tar` & `load_envfile-0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 16:31:18.786780 load_envfile-0.2/
--rw-rw-rw-   0        0        0      242 2024-04-23 16:31:18.784782 load_envfile-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      985 2024-04-23 11:02:57.000000 load_envfile-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 16:31:18.782783 load_envfile-0.2/load_envfile.egg-info/
--rw-rw-rw-   0        0        0      242 2024-04-23 16:31:18.000000 load_envfile-0.2/load_envfile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-04-23 16:31:18.000000 load_envfile-0.2/load_envfile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 16:31:18.000000 load_envfile-0.2/load_envfile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-23 16:31:18.000000 load_envfile-0.2/load_envfile.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 16:31:18.000000 load_envfile-0.2/load_envfile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 16:31:18.786780 load_envfile-0.2/setup.cfg
--rw-rw-rw-   0        0        0      368 2024-04-23 16:30:44.000000 load_envfile-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 16:48:31.225529 load_envfile-0.3/
+-rw-rw-rw-   0        0        0      242 2024-04-23 16:48:31.224529 load_envfile-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      985 2024-04-23 11:02:57.000000 load_envfile-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 16:48:31.222535 load_envfile-0.3/load_envfile.egg-info/
+-rw-rw-rw-   0        0        0      242 2024-04-23 16:48:31.000000 load_envfile-0.3/load_envfile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-04-23 16:48:31.000000 load_envfile-0.3/load_envfile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 16:48:31.000000 load_envfile-0.3/load_envfile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-23 16:48:31.000000 load_envfile-0.3/load_envfile.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 16:48:31.000000 load_envfile-0.3/load_envfile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 16:48:31.225529 load_envfile-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      368 2024-04-23 16:48:12.000000 load_envfile-0.3/setup.py
```

### Comparing `load_envfile-0.2/README.md` & `load_envfile-0.3/README.md`

 * *Files identical despite different names*

