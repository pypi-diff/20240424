# Comparing `tmp/load_envfile-0.3.tar.gz` & `tmp/load_envfile-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "load_envfile-0.3.tar", last modified: Tue Apr 23 16:48:31 2024, max compression
+gzip compressed data, was "load_envfile-0.5.tar", last modified: Wed Apr 24 06:26:10 2024, max compression
```

## Comparing `load_envfile-0.3.tar` & `load_envfile-0.5.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 16:48:31.225529 load_envfile-0.3/
--rw-rw-rw-   0        0        0      242 2024-04-23 16:48:31.224529 load_envfile-0.3/PKG-INFO
--rw-rw-rw-   0        0        0      985 2024-04-23 11:02:57.000000 load_envfile-0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 16:48:31.222535 load_envfile-0.3/load_envfile.egg-info/
--rw-rw-rw-   0        0        0      242 2024-04-23 16:48:31.000000 load_envfile-0.3/load_envfile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-04-23 16:48:31.000000 load_envfile-0.3/load_envfile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 16:48:31.000000 load_envfile-0.3/load_envfile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-23 16:48:31.000000 load_envfile-0.3/load_envfile.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 16:48:31.000000 load_envfile-0.3/load_envfile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 16:48:31.225529 load_envfile-0.3/setup.cfg
--rw-rw-rw-   0        0        0      368 2024-04-23 16:48:12.000000 load_envfile-0.3/setup.py
+drwxr-xr-x   0 maria      (502) staff       (20)        0 2024-04-24 06:26:10.063428 load_envfile-0.5/
+-rw-r--r--   0 maria      (502) staff       (20)      258 2024-04-24 06:26:10.062903 load_envfile-0.5/PKG-INFO
+-rw-r--r--   0 maria      (502) staff       (20)      985 2024-04-24 05:36:26.000000 load_envfile-0.5/README.md
+drwxr-xr-x   0 maria      (502) staff       (20)        0 2024-04-24 06:26:10.059488 load_envfile-0.5/load_envfile/
+-rw-r--r--   0 maria      (502) staff       (20)       38 2024-04-24 05:42:11.000000 load_envfile-0.5/load_envfile/__init__.py
+-rw-r--r--   0 maria      (502) staff       (20)      440 2024-04-24 06:20:25.000000 load_envfile-0.5/load_envfile/load_envfile.py
+drwxr-xr-x   0 maria      (502) staff       (20)        0 2024-04-24 06:26:10.062255 load_envfile-0.5/load_envfile.egg-info/
+-rw-r--r--   0 maria      (502) staff       (20)      258 2024-04-24 06:26:10.000000 load_envfile-0.5/load_envfile.egg-info/PKG-INFO
+-rw-r--r--   0 maria      (502) staff       (20)      251 2024-04-24 06:26:10.000000 load_envfile-0.5/load_envfile.egg-info/SOURCES.txt
+-rw-r--r--   0 maria      (502) staff       (20)        1 2024-04-24 06:26:10.000000 load_envfile-0.5/load_envfile.egg-info/dependency_links.txt
+-rw-r--r--   0 maria      (502) staff       (20)       14 2024-04-24 06:26:10.000000 load_envfile-0.5/load_envfile.egg-info/requires.txt
+-rw-r--r--   0 maria      (502) staff       (20)       13 2024-04-24 06:26:10.000000 load_envfile-0.5/load_envfile.egg-info/top_level.txt
+-rw-r--r--   0 maria      (502) staff       (20)       38 2024-04-24 06:26:10.063557 load_envfile-0.5/setup.cfg
+-rw-r--r--   0 maria      (502) staff       (20)      538 2024-04-24 06:24:58.000000 load_envfile-0.5/setup.py
```

### Comparing `load_envfile-0.3/README.md` & `load_envfile-0.5/README.md`

 * *Files identical despite different names*

