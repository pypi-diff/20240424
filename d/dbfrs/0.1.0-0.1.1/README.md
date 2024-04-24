# Comparing `tmp/dbfrs-0.1.0.tar.gz` & `tmp/dbfrs-0.1.1.tar.gz`

## Comparing `dbfrs-0.1.0.tar` & `dbfrs-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0      434 1970-01-01 00:00:00.000000 dbfrs-0.1.0/Cargo.toml
--rw-r--r--   0     1000     1000       20 2024-04-23 20:14:54.000000 dbfrs-0.1.0/.gitignore
--rw-r--r--   0     1000     1000        8 2024-04-23 20:14:46.000000 dbfrs-0.1.0/README.md
--rw-r--r--   0     1000     1000      160 2024-04-23 20:20:11.000000 dbfrs-0.1.0/pyvenv.cfg
--rw-r--r--   0     1000     1000     4747 2024-04-23 20:22:33.000000 dbfrs-0.1.0/src/lib.rs
--rw-r--r--   0     1000     1000    11928 2024-04-23 20:13:44.000000 dbfrs-0.1.0/Cargo.lock
--rw-r--r--   0     1000     1000      233 2024-04-23 17:06:06.000000 dbfrs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      127 1970-01-01 00:00:00.000000 dbfrs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 dbfrs-0.1.1/Cargo.toml
+-rw-r--r--   0     1000     1000       33 2024-04-24 11:48:36.000000 dbfrs-0.1.1/.gitignore
+-rw-r--r--   0     1000     1000      115 2024-04-24 11:49:30.000000 dbfrs-0.1.1/CHANGELOG.md
+-rw-r--r--   0     1000     1000     1125 2024-04-24 07:40:04.000000 dbfrs-0.1.1/README.md
+-rw-r--r--   0     1000     1000      160 2024-04-24 11:10:54.000000 dbfrs-0.1.1/pyvenv.cfg
+-rw-r--r--   0     1000     1000     8922 2024-04-24 11:45:11.000000 dbfrs-0.1.1/src/lib.rs
+-rw-r--r--   0     1000     1000      286 2024-04-24 11:44:03.000000 dbfrs-0.1.1/tests/test.dbf
+-rw-r--r--   0     1000     1000      457 2024-04-24 11:42:31.000000 dbfrs-0.1.1/tests/test_rw.py
+-rw-r--r--   0     1000     1000    11928 2024-04-24 11:47:25.000000 dbfrs-0.1.1/Cargo.lock
+-rw-r--r--   0     1000     1000      409 2024-04-23 20:56:02.000000 dbfrs-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1542 1970-01-01 00:00:00.000000 dbfrs-0.1.1/PKG-INFO
```

### Comparing `dbfrs-0.1.0/Cargo.lock` & `dbfrs-0.1.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
  "byteorder",
  "time",
  "yore",
 ]
 
 [[package]]
 name = "dbfrs"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "dbase",
  "pyo3",
  "rand",
 ]
 
 [[package]]
```

