# Comparing `tmp/myemail-0.4.0.tar.gz` & `tmp/myemail-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myemail-0.4.0.tar", max compression
+gzip compressed data, was "myemail-0.5.0.tar", max compression
```

## Comparing `myemail-0.4.0.tar` & `myemail-0.5.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1063 2024-04-24 13:21:13.393519 myemail-0.4.0/LICENSE
--rw-r--r--   0        0        0      614 2024-04-24 19:27:37.695303 myemail-0.4.0/README.md
--rw-r--r--   0        0        0       32 2024-04-24 13:18:32.223261 myemail-0.4.0/myemail/__init__.py
--rw-r--r--   0        0        0     1619 2024-04-24 19:26:51.751488 myemail-0.4.0/myemail/myemail.py
--rw-r--r--   0        0        0      401 2024-04-24 19:14:45.826489 myemail-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1113 1970-01-01 00:00:00.000000 myemail-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-24 13:21:13.393519 myemail-0.5.0/LICENSE
+-rw-r--r--   0        0        0      614 2024-04-24 19:27:37.695303 myemail-0.5.0/README.md
+-rw-r--r--   0        0        0       32 2024-04-24 13:18:32.223261 myemail-0.5.0/myemail/__init__.py
+-rw-r--r--   0        0        0     1619 2024-04-24 19:26:51.751488 myemail-0.5.0/myemail/myemail.py
+-rw-r--r--   0        0        0      401 2024-04-24 19:39:20.603866 myemail-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1164 1970-01-01 00:00:00.000000 myemail-0.5.0/PKG-INFO
```

### Comparing `myemail-0.4.0/LICENSE` & `myemail-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `myemail-0.4.0/README.md` & `myemail-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `myemail-0.4.0/myemail/myemail.py` & `myemail-0.5.0/myemail/myemail.py`

 * *Files identical despite different names*

### Comparing `myemail-0.4.0/PKG-INFO` & `myemail-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: myemail
-Version: 0.4.0
+Version: 0.5.0
 Summary: A simple package to send emails with python
 Home-page: https://github.com/tct123/myemail
 Author: tct123
 Author-email: 42028373+tct123@users.noreply.github.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://github.com/tct123/myemail
 Description-Content-Type: text/markdown
 
 # MyEmail
 A simple library to send emails with python
```

