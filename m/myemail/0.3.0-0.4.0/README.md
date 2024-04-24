# Comparing `tmp/myemail-0.3.0.tar.gz` & `tmp/myemail-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myemail-0.3.0.tar", max compression
+gzip compressed data, was "myemail-0.4.0.tar", max compression
```

## Comparing `myemail-0.3.0.tar` & `myemail-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1063 2024-04-24 13:21:13.393519 myemail-0.3.0/LICENSE
--rw-r--r--   0        0        0        0 2024-04-24 13:11:14.867595 myemail-0.3.0/README.md
--rw-r--r--   0        0        0       32 2024-04-24 13:18:32.223261 myemail-0.3.0/myemail/__init__.py
--rw-r--r--   0        0        0     1618 2024-04-24 18:59:30.362504 myemail-0.3.0/myemail/myemail.py
--rw-r--r--   0        0        0      358 2024-04-24 19:01:19.201962 myemail-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      456 1970-01-01 00:00:00.000000 myemail-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-24 13:21:13.393519 myemail-0.4.0/LICENSE
+-rw-r--r--   0        0        0      614 2024-04-24 19:27:37.695303 myemail-0.4.0/README.md
+-rw-r--r--   0        0        0       32 2024-04-24 13:18:32.223261 myemail-0.4.0/myemail/__init__.py
+-rw-r--r--   0        0        0     1619 2024-04-24 19:26:51.751488 myemail-0.4.0/myemail/myemail.py
+-rw-r--r--   0        0        0      401 2024-04-24 19:14:45.826489 myemail-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1113 1970-01-01 00:00:00.000000 myemail-0.4.0/PKG-INFO
```

### Comparing `myemail-0.3.0/LICENSE` & `myemail-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `myemail-0.3.0/myemail/myemail.py` & `myemail-0.4.0/myemail/myemail.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,9 +49,9 @@
     send(
         msg_content="test",
         from_email=emailvar,
         to_email=emailvar,
         subject="test",
         sslport=sslport,
         password=password,
-        attachment_path=attachment_path
+        attachment_path=attachment_path,
     )
```

