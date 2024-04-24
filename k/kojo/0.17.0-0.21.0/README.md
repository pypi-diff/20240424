# Comparing `tmp/kojo-0.17.0.tar.gz` & `tmp/kojo-0.21.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kojo-0.17.0.tar", last modified: Sun May 21 11:07:53 2023, max compression
+gzip compressed data, was "kojo-0.21.0.tar", last modified: Wed Apr 24 07:41:18 2024, max compression
```

## Comparing `kojo-0.17.0.tar` & `kojo-0.21.0.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxr-xr-x   0 olaf       (501) staff       (20)        0 2023-05-21 11:07:53.000000 kojo-0.17.0/
-drwxr-xr-x   0 olaf       (501) staff       (20)        0 2023-05-21 11:07:53.000000 kojo-0.17.0/kojo/
--rw-r--r--   0 olaf       (501) staff       (20)      454 2023-05-20 06:51:50.000000 kojo-0.17.0/kojo/duplicatefinder.py
--rw-r--r--   0 olaf       (501) staff       (20)     2188 2023-05-20 19:17:09.000000 kojo-0.17.0/kojo/io.py
--rw-r--r--   0 olaf       (501) staff       (20)      142 2023-05-20 06:51:50.000000 kojo-0.17.0/kojo/__init__.py
--rw-r--r--   0 olaf       (501) staff       (20)      947 2023-05-20 06:51:50.000000 kojo-0.17.0/kojo/jsonschemavalidator.py
--rw-r--r--   0 olaf       (501) staff       (20)     1314 2023-05-21 10:39:01.000000 kojo-0.17.0/kojo/process.py
--rw-r--r--   0 olaf       (501) staff       (20)     1844 2023-05-20 06:51:50.000000 kojo-0.17.0/kojo/propertiesconverter.py
--rw-r--r--   0 olaf       (501) staff       (20)     4108 2023-05-20 07:57:15.000000 kojo-0.17.0/kojo/item.py
--rw-r--r--   0 olaf       (501) staff       (20)      561 2023-05-21 11:07:53.000000 kojo-0.17.0/PKG-INFO
--rw-r--r--   0 olaf       (501) staff       (20)      693 2023-05-21 11:02:26.000000 kojo-0.17.0/setup.py
--rw-r--r--   0 olaf       (501) staff       (20)       39 2023-05-20 06:51:50.000000 kojo-0.17.0/setup.cfg
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-04-24 07:41:18.751580 kojo-0.21.0/
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)    35148 2023-04-27 08:31:58.000000 kojo-0.21.0/LICENSE.txt
+-rw-r--r--   0 olaf      (1000) olaf      (1000)     4494 2024-04-24 07:41:18.751580 kojo-0.21.0/PKG-INFO
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     3752 2023-04-27 09:07:15.000000 kojo-0.21.0/README.md
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-04-24 07:41:18.751580 kojo-0.21.0/kojo/
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      142 2023-04-27 08:51:59.000000 kojo-0.21.0/kojo/__init__.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     1115 2024-04-24 05:46:05.000000 kojo-0.21.0/kojo/extra.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     5238 2024-04-24 07:18:15.000000 kojo-0.21.0/kojo/item.py
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     1718 2024-04-23 12:07:56.000000 kojo-0.21.0/kojo/process.py
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2024-04-24 07:41:18.751580 kojo-0.21.0/kojo.egg-info/
+-rw-r--r--   0 olaf      (1000) olaf      (1000)     4494 2024-04-24 07:41:18.000000 kojo-0.21.0/kojo.egg-info/PKG-INFO
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      208 2024-04-24 07:41:18.000000 kojo-0.21.0/kojo.egg-info/SOURCES.txt
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)        1 2024-04-24 07:41:18.000000 kojo-0.21.0/kojo.egg-info/dependency_links.txt
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)        5 2024-04-24 07:41:18.000000 kojo-0.21.0/kojo.egg-info/top_level.txt
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      801 2024-04-24 06:06:46.000000 kojo-0.21.0/pyproject.toml
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)       38 2024-04-24 07:41:18.751580 kojo-0.21.0/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

