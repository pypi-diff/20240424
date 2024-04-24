# Comparing `tmp/pgtricks-1.0.0.tar.gz` & `tmp/pgtricks-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pgtricks-1.0.0.tar", last modified: Sun Sep 12 08:32:33 2021, max compression
+gzip compressed data, was "pgtricks-1.1.0.tar", last modified: Wed Apr 24 20:00:14 2024, max compression
```

## Comparing `pgtricks-1.0.0.tar` & `pgtricks-1.1.0.tar`

### file list

```diff
@@ -1,31 +1,21 @@
-drwxrwxr-x   0 kaiant    (1000) kaiant    (1000)        0 2021-09-12 08:32:33.413764 pgtricks-1.0.0/
-drwxrwxr-x   0 kaiant    (1000) kaiant    (1000)        0 2021-09-12 08:32:33.410764 pgtricks-1.0.0/.github/
-drwxrwxr-x   0 kaiant    (1000) kaiant    (1000)        0 2021-09-12 08:32:33.411764 pgtricks-1.0.0/.github/workflows/
--rw-rw-r--   0 kaiant    (1000) kaiant    (1000)      955 2021-09-12 07:51:23.000000 pgtricks-1.0.0/.github/workflows/python-package.yml
--rw-rw-r--   0 kaiant    (1000) kaiant    (1000)       53 2019-10-14 16:48:49.000000 pgtricks-1.0.0/.gitignore
--rw-rw-r--   0 kaiant    (1000) kaiant    (1000)      766 2021-09-11 18:54:47.000000 pgtricks-1.0.0/CHANGES.rst
--rw-rw-r--   0 kaiant    (1000) kaiant    (1000)      121 2020-06-29 21:49:46.000000 pgtricks-1.0.0/CONTRIBUTORS.rst
--rw-rw-r--   0 kaiant    (1000) kaiant    (1000)     1524 2019-10-14 16:32:32.000000 pgtricks-1.0.0/LICENSE
--rw-rw-r--   0 kaiant    (1000) kaiant    (1000)     3781 2021-09-12 08:32:33.413764 pgtricks-1.0.0/PKG-INFO
--rw-rw-r--   0 kaiant    (1000) kaiant    (1000)     2798 2020-06-26 20:35:33.000000 pgtricks-1.0.0/README.rst
--rw-rw-r--   0 kaiant    (1000) kaiant    (1000)      827 2021-09-11 18:32:26.000000 pgtricks-1.0.0/mypy.ini
-drwxrwxr-x   0 kaiant    (1000) kaiant    (1000)        0 2021-09-12 08:32:33.411764 pgtricks-1.0.0/pgtricks/
--rw-rw-r--   0 kaiant    (1000) kaiant    (1000)        0 2019-10-14 16:48:49.000000 pgtricks-1.0.0/pgtricks/__init__.py
--rwxrwxr-x   0 kaiant    (1000) kaiant    (1000)     3466 2021-09-11 19:15:00.000000 pgtricks-1.0.0/pgtricks/pg_dump_splitsort.py
--rwxrwxr-x   0 kaiant    (1000) kaiant    (1000)     2434 2020-07-04 08:06:03.000000 pgtricks-1.0.0/pgtricks/pg_incremental_backup.py
--rwxrwxr-x   0 kaiant    (1000) kaiant    (1000)     2307 2020-07-04 08:06:03.000000 pgtricks-1.0.0/pgtricks/pg_split_schema_dump.py
-drwxrwxr-x   0 kaiant    (1000) kaiant    (1000)        0 2021-09-12 08:32:33.412764 pgtricks-1.0.0/pgtricks/tests/
--rw-rw-r--   0 kaiant    (1000) kaiant    (1000)        0 2019-10-14 16:48:49.000000 pgtricks-1.0.0/pgtricks/tests/__init__.py
--rw-rw-r--   0 kaiant    (1000) kaiant    (1000)     2888 2021-09-11 18:32:26.000000 pgtricks-1.0.0/pgtricks/tests/test_pg_dump_splitsort.py
--rw-rw-r--   0 kaiant    (1000) kaiant    (1000)     1674 2020-07-04 08:06:03.000000 pgtricks-1.0.0/pgtricks/tests/test_pg_incremental_backup.py
--rw-rw-r--   0 kaiant    (1000) kaiant    (1000)     3940 2021-09-11 19:23:34.000000 pgtricks-1.0.0/pgtricks/tests/test_pg_split_schema_dump.py
-drwxrwxr-x   0 kaiant    (1000) kaiant    (1000)        0 2021-09-12 08:32:33.412764 pgtricks-1.0.0/pgtricks.egg-info/
--rw-rw-r--   0 kaiant    (1000) kaiant    (1000)     3781 2021-09-12 08:32:33.000000 pgtricks-1.0.0/pgtricks.egg-info/PKG-INFO
--rw-rw-r--   0 kaiant    (1000) kaiant    (1000)      603 2021-09-12 08:32:33.000000 pgtricks-1.0.0/pgtricks.egg-info/SOURCES.txt
--rw-rw-r--   0 kaiant    (1000) kaiant    (1000)        1 2021-09-12 08:32:33.000000 pgtricks-1.0.0/pgtricks.egg-info/dependency_links.txt
--rw-rw-r--   0 kaiant    (1000) kaiant    (1000)      189 2021-09-12 08:32:33.000000 pgtricks-1.0.0/pgtricks.egg-info/entry_points.txt
--rw-rw-r--   0 kaiant    (1000) kaiant    (1000)       60 2021-09-12 08:32:33.000000 pgtricks-1.0.0/pgtricks.egg-info/requires.txt
--rw-rw-r--   0 kaiant    (1000) kaiant    (1000)        9 2021-09-12 08:32:33.000000 pgtricks-1.0.0/pgtricks.egg-info/top_level.txt
--rw-rw-r--   0 kaiant    (1000) kaiant    (1000)      109 2020-07-04 08:06:03.000000 pgtricks-1.0.0/pytest.ini
--rw-rw-r--   0 kaiant    (1000) kaiant    (1000)     1315 2021-09-12 08:32:33.413764 pgtricks-1.0.0/setup.cfg
--rw-rw-r--   0 kaiant    (1000) kaiant    (1000)       39 2020-06-26 20:35:33.000000 pgtricks-1.0.0/setup.py
+drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-24 20:00:14.647071 pgtricks-1.1.0/
+-rw-r--r--   0 akaihola  (1000) users      (100)     1524 2023-08-05 20:39:18.000000 pgtricks-1.1.0/LICENSE
+-rw-r--r--   0 akaihola  (1000) users      (100)     5637 2024-04-24 20:00:14.647071 pgtricks-1.1.0/PKG-INFO
+-rw-r--r--   0 akaihola  (1000) users      (100)     9241 2024-04-24 19:59:46.000000 pgtricks-1.1.0/README.rst
+drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-24 20:00:14.646071 pgtricks-1.1.0/pgtricks/
+-rw-r--r--   0 akaihola  (1000) users      (100)        0 2023-08-05 20:39:18.000000 pgtricks-1.1.0/pgtricks/__init__.py
+-rw-r--r--   0 akaihola  (1000) users      (100)     2970 2024-04-22 13:57:06.000000 pgtricks-1.1.0/pgtricks/mergesort.py
+-rwxr-xr-x   0 akaihola  (1000) users      (100)     5352 2024-04-24 19:50:56.000000 pgtricks-1.1.0/pgtricks/pg_dump_splitsort.py
+-rwxr-xr-x   0 akaihola  (1000) users      (100)     2434 2023-08-05 20:39:18.000000 pgtricks-1.1.0/pgtricks/pg_incremental_backup.py
+-rwxr-xr-x   0 akaihola  (1000) users      (100)     2324 2024-04-19 19:41:47.000000 pgtricks-1.1.0/pgtricks/pg_split_schema_dump.py
+-rw-r--r--   0 akaihola  (1000) users      (100)       87 2024-04-24 19:54:12.000000 pgtricks-1.1.0/pgtricks/version.py
+drwxr-xr-x   0 akaihola  (1000) users      (100)        0 2024-04-24 20:00:14.647071 pgtricks-1.1.0/pgtricks.egg-info/
+-rw-r--r--   0 akaihola  (1000) users      (100)     5637 2024-04-24 20:00:14.000000 pgtricks-1.1.0/pgtricks.egg-info/PKG-INFO
+-rw-r--r--   0 akaihola  (1000) users      (100)      406 2024-04-24 20:00:14.000000 pgtricks-1.1.0/pgtricks.egg-info/SOURCES.txt
+-rw-r--r--   0 akaihola  (1000) users      (100)        1 2024-04-24 20:00:14.000000 pgtricks-1.1.0/pgtricks.egg-info/dependency_links.txt
+-rw-r--r--   0 akaihola  (1000) users      (100)      188 2024-04-24 20:00:14.000000 pgtricks-1.1.0/pgtricks.egg-info/entry_points.txt
+-rw-r--r--   0 akaihola  (1000) users      (100)       97 2024-04-24 20:00:14.000000 pgtricks-1.1.0/pgtricks.egg-info/requires.txt
+-rw-r--r--   0 akaihola  (1000) users      (100)        9 2024-04-24 20:00:14.000000 pgtricks-1.1.0/pgtricks.egg-info/top_level.txt
+-rw-r--r--   0 akaihola  (1000) users      (100)     1085 2024-04-22 13:57:06.000000 pgtricks-1.1.0/pyproject.toml
+-rw-r--r--   0 akaihola  (1000) users      (100)     1502 2024-04-24 20:00:14.648071 pgtricks-1.1.0/setup.cfg
+-rw-r--r--   0 akaihola  (1000) users      (100)     1795 2024-04-24 19:58:52.000000 pgtricks-1.1.0/setup.py
```

### Comparing `pgtricks-1.0.0/LICENSE` & `pgtricks-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pgtricks-1.0.0/pgtricks/pg_incremental_backup.py` & `pgtricks-1.1.0/pgtricks/pg_incremental_backup.py`

 * *Files identical despite different names*

### Comparing `pgtricks-1.0.0/pgtricks/pg_split_schema_dump.py` & `pgtricks-1.1.0/pgtricks/pg_split_schema_dump.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                 "Can't identify the following SQL chunk in {sqlpath}:\n"
                 "{divider}\n"
                 "{chunk}\n"
                 "{divider}".format(sqlpath=sqlpath, chunk=part, divider=77 * '=')
             )
             print(part)
             continue
-        name = match.group(1).replace(" ", "_")
+        name = match.group(1).replace(" ", "_").replace('"', "")
         type_ = match.group(2).replace(" ", "_")
         schema = match.group(3)
         if schema == "-":
             schema = "no_schema"
         if name == "id":
             continue
         dump_filename = "{}.{}.{}".format(schema, name, type_)
```

### Comparing `pgtricks-1.0.0/setup.cfg` & `pgtricks-1.1.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pgtricks
-version = 1.0.0
+version = attr: pgtricks.version.__version__
 author = Antti Kaihola
 author_email = 13725+akaihola@users.noreply.github.com
 license = BSD
 license_file = LICENSE
 description = PostgreSQL utilities
 long_description = file:README.rst
 long_description_content_type = text/x-rst
@@ -13,14 +13,17 @@
 	Environment :: Console
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Database
 	Topic :: System :: Archiving :: Backup
 keywords = 
 	database
 	postgresql
 	backup
 	git
@@ -44,14 +47,16 @@
 test = 
 	darker[isort]
 	flake8
 	mypy
 	pylint
 	pytest
 	pytest-mypy
+release = 
+	darkgray-dev-tools~=0.0.2
 
 [flake8]
 max-line-length = 88
 extend-ignore = E203
 
 [egg_info]
 tag_build =
```

