# Comparing `tmp/myemail-0.1.0.tar.gz` & `tmp/myemail-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myemail-0.1.0.tar", max compression
+gzip compressed data, was "myemail-0.2.0.tar", max compression
```

## Comparing `myemail-0.1.0.tar` & `myemail-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1063 2024-04-24 13:21:13.393519 myemail-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2024-04-24 13:11:14.867595 myemail-0.1.0/README.md
--rw-r--r--   0        0        0       32 2024-04-24 13:18:32.223261 myemail-0.1.0/myemail/__init__.py
--rw-r--r--   0        0        0      562 2024-04-24 13:17:41.853717 myemail-0.1.0/myemail/myemail.py
--rw-r--r--   0        0        0      331 2024-04-24 13:22:58.425525 myemail-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      456 1970-01-01 00:00:00.000000 myemail-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-24 13:21:13.393519 myemail-0.2.0/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-24 13:11:14.867595 myemail-0.2.0/README.md
+-rw-r--r--   0        0        0       32 2024-04-24 13:18:32.223261 myemail-0.2.0/myemail/__init__.py
+-rw-r--r--   0        0        0      633 2024-04-24 13:24:26.796972 myemail-0.2.0/myemail/myemail.py
+-rw-r--r--   0        0        0      331 2024-04-24 13:25:15.812506 myemail-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      456 1970-01-01 00:00:00.000000 myemail-0.2.0/PKG-INFO
```

### Comparing `myemail-0.1.0/LICENSE` & `myemail-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `myemail-0.1.0/myemail/myemail.py` & `myemail-0.2.0/myemail/myemail.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-def send(msg_content,from_email, to_email,subject):
+import smtplib
+from email.message import EmailMessage
+import email
+
+
+def send(msg_content, from_email, to_email, subject):
     msg_content = msg_content
     message = EmailMessage()
     message["From"] = from_email
     message["To"] = to_email
     message["Subject"] = subject
     message.set_content(msg_content)
     try:
```

