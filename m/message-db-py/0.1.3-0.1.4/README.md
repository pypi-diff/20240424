# Comparing `tmp/message_db_py-0.1.3.tar.gz` & `tmp/message_db_py-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "message_db_py-0.1.3.tar", max compression
+gzip compressed data, was "message_db_py-0.1.4.tar", max compression
```

## Comparing `message_db_py-0.1.3.tar` & `message_db_py-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1080 2024-04-23 22:49:09.333522 message_db_py-0.1.3/LICENSE
--rw-r--r--   0        0        0     1269 2024-04-23 23:03:47.862606 message_db_py-0.1.3/README.md
--rw-r--r--   0        0        0      963 2024-04-23 23:52:46.715013 message_db_py-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-23 23:52:46.715427 message_db_py-0.1.3/src/message_db/__init__.py
--rw-r--r--   0        0        0     7765 2024-04-23 21:56:55.046160 message_db_py-0.1.3/src/message_db/client.py
--rw-r--r--   0        0        0     1880 2022-01-20 19:19:52.169102 message_db_py-0.1.3/src/message_db/connection.py
--rw-r--r--   0        0        0     1866 1970-01-01 00:00:00.000000 message_db_py-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-04-23 22:49:09.333522 message_db_py-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1269 2024-04-23 23:03:47.862606 message_db_py-0.1.4/README.md
+-rw-r--r--   0        0        0      963 2024-04-24 00:16:28.551787 message_db_py-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-24 00:16:28.552175 message_db_py-0.1.4/src/message_db/__init__.py
+-rw-r--r--   0        0        0     7765 2024-04-23 21:56:55.046160 message_db_py-0.1.4/src/message_db/client.py
+-rw-r--r--   0        0        0     1880 2022-01-20 19:19:52.169102 message_db_py-0.1.4/src/message_db/connection.py
+-rw-r--r--   0        0        0     1866 1970-01-01 00:00:00.000000 message_db_py-0.1.4/PKG-INFO
```

### Comparing `message_db_py-0.1.3/LICENSE` & `message_db_py-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `message_db_py-0.1.3/README.md` & `message_db_py-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `message_db_py-0.1.3/pyproject.toml` & `message_db_py-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "message-db-py"
-version = "0.1.3"
+version = "0.1.4"
 description = "The Python interface to the MessageDB Event Store and Message Store"
 authors = ["Subhash Bhushan <subhash.bhushan@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: MIT License",
```

### Comparing `message_db_py-0.1.3/src/message_db/client.py` & `message_db_py-0.1.4/src/message_db/client.py`

 * *Files identical despite different names*

### Comparing `message_db_py-0.1.3/src/message_db/connection.py` & `message_db_py-0.1.4/src/message_db/connection.py`

 * *Files identical despite different names*

### Comparing `message_db_py-0.1.3/PKG-INFO` & `message_db_py-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: message-db-py
-Version: 0.1.3
+Version: 0.1.4
 Summary: The Python interface to the MessageDB Event Store and Message Store
 License: MIT
 Author: Subhash Bhushan
 Author-email: subhash.bhushan@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

