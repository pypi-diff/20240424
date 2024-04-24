# Comparing `tmp/djau_gsuite_email-0.1.4.tar.gz` & `tmp/djau_gsuite_email-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djau_gsuite_email-0.1.4.tar", last modified: Tue Apr 23 09:34:23 2024, max compression
+gzip compressed data, was "djau_gsuite_email-0.1.5.tar", last modified: Wed Apr 24 01:16:38 2024, max compression
```

## Comparing `djau_gsuite_email-0.1.4.tar` & `djau_gsuite_email-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:34:23.611354 djau_gsuite_email-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-23 09:34:14.000000 djau_gsuite_email-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-23 09:34:14.000000 djau_gsuite_email-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-23 09:34:23.611354 djau_gsuite_email-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-23 09:34:14.000000 djau_gsuite_email-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:34:23.607354 djau_gsuite_email-0.1.4/django_gsuite_email/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-23 09:34:14.000000 djau_gsuite_email-0.1.4/django_gsuite_email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-23 09:34:14.000000 djau_gsuite_email-0.1.4/django_gsuite_email/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-04-23 09:34:14.000000 djau_gsuite_email-0.1.4/django_gsuite_email/backends.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-23 09:34:14.000000 djau_gsuite_email-0.1.4/django_gsuite_email/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-23 09:34:14.000000 djau_gsuite_email-0.1.4/django_gsuite_email/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:34:23.611354 djau_gsuite_email-0.1.4/djau_gsuite_email.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-23 09:34:23.000000 djau_gsuite_email-0.1.4/djau_gsuite_email.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-23 09:34:23.000000 djau_gsuite_email-0.1.4/djau_gsuite_email.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 09:34:23.000000 djau_gsuite_email-0.1.4/djau_gsuite_email.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-23 09:34:23.000000 djau_gsuite_email-0.1.4/djau_gsuite_email.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-23 09:34:23.000000 djau_gsuite_email-0.1.4/djau_gsuite_email.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 09:34:23.611354 djau_gsuite_email-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-04-23 09:34:14.000000 djau_gsuite_email-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:16:38.699227 djau_gsuite_email-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-24 01:16:29.000000 djau_gsuite_email-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-24 01:16:29.000000 djau_gsuite_email-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-24 01:16:38.699227 djau_gsuite_email-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-24 01:16:29.000000 djau_gsuite_email-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:16:38.695227 djau_gsuite_email-0.1.5/django_gsuite_email/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-24 01:16:29.000000 djau_gsuite_email-0.1.5/django_gsuite_email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-24 01:16:29.000000 djau_gsuite_email-0.1.5/django_gsuite_email/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-24 01:16:29.000000 djau_gsuite_email-0.1.5/django_gsuite_email/backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-24 01:16:29.000000 djau_gsuite_email-0.1.5/django_gsuite_email/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-24 01:16:29.000000 djau_gsuite_email-0.1.5/django_gsuite_email/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:16:38.699227 djau_gsuite_email-0.1.5/djau_gsuite_email.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-24 01:16:38.000000 djau_gsuite_email-0.1.5/djau_gsuite_email.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-24 01:16:38.000000 djau_gsuite_email-0.1.5/djau_gsuite_email.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 01:16:38.000000 djau_gsuite_email-0.1.5/djau_gsuite_email.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-24 01:16:38.000000 djau_gsuite_email-0.1.5/djau_gsuite_email.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-24 01:16:38.000000 djau_gsuite_email-0.1.5/djau_gsuite_email.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 01:16:38.699227 djau_gsuite_email-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-04-24 01:16:29.000000 djau_gsuite_email-0.1.5/setup.py
```

### Comparing `djau_gsuite_email-0.1.4/LICENSE` & `djau_gsuite_email-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `djau_gsuite_email-0.1.4/PKG-INFO` & `djau_gsuite_email-0.1.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djau-gsuite-email
-Version: 0.1.4
+Version: 0.1.5
 Summary: Send emails via a GSuite Service-account.
 Home-page: https://github.com/slicefox/django-gsuite-email
 Author: slicefox
 Author-email: adithya.webdev@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -54,17 +54,22 @@
 EMAIL_BACKEND = 'django_gsuite_email.GSuiteEmailBackend'
 ```
 
 #### 3. Set location of credentials file.
 To do this, either set `GSUITE_CREDENTIALS_FILE` environment variable.\
 OR \
 set `GSUITE_CREDENTIALS_FILE` in `settings.py`
-````python
+
+```python
 GSUITE_CREDENTIALS_FILE="/path/to/credentials/file.json"
-````
+GSUITE_USER_FROM_EMAIL = False  # use the user of from_email if True. Default value False.
+GMAIL_USER = 'user@domain'      # default user if GSUITE_USER_FROM_EMAIL is not True. Default value None.
+GMAIL_SCOPES = ['https://www.googleapis.com/auth/gmail.send', ... ] # Default value ['https://www.googleapis.com/auth/gmail.send', ]
+```
+
 > #### Note: `GSUITE_CREDENTIALS_FILE` in `settings.py` will take precedence over environment variable.
 
 #### 4. Send emails
 ```python
 from django.core.mail import send_mail
 
 send_mail(
```

### Comparing `djau_gsuite_email-0.1.4/README.md` & `djau_gsuite_email-0.1.5/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -33,17 +33,22 @@
 EMAIL_BACKEND = 'django_gsuite_email.GSuiteEmailBackend'
 ```
 
 #### 3. Set location of credentials file.
 To do this, either set `GSUITE_CREDENTIALS_FILE` environment variable.\
 OR \
 set `GSUITE_CREDENTIALS_FILE` in `settings.py`
-````python
+
+```python
 GSUITE_CREDENTIALS_FILE="/path/to/credentials/file.json"
-````
+GSUITE_USER_FROM_EMAIL = False  # use the user of from_email if True. Default value False.
+GMAIL_USER = 'user@domain'      # default user if GSUITE_USER_FROM_EMAIL is not True. Default value None.
+GMAIL_SCOPES = ['https://www.googleapis.com/auth/gmail.send', ... ] # Default value ['https://www.googleapis.com/auth/gmail.send', ]
+```
+
 > #### Note: `GSUITE_CREDENTIALS_FILE` in `settings.py` will take precedence over environment variable.
 
 #### 4. Send emails
 ```python
 from django.core.mail import send_mail
 
 send_mail(
```

### Comparing `djau_gsuite_email-0.1.4/django_gsuite_email/backends.py` & `djau_gsuite_email-0.1.5/django_gsuite_email/backends.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,21 @@
 class GSuiteEmailBackend(BaseEmailBackend):
     def __init__(self, fail_silently=False, **kwargs):
 
         super().__init__(fail_silently=fail_silently)
         
         self.fail_silently = fail_silently
         self.credentials = get_credentials_file()
-        self.API_SCOPE = settings.GMAIL_SCOPES if settings.GMAIL_SCOPES else ['https://www.googleapis.com/auth/gmail.send', ]
+        self.API_SCOPE = settings.GMAIL_SCOPES if hasattr(settings, 'GMAIL_SCOPES') else ['https://www.googleapis.com/auth/gmail.send', ]
         # to reopen connection with different delegation when user changes
         self.current_user = None
         self.connection = None
+        self.gmail_user = settings.GMAIL_USER if hasattr(settings, 'GMAIL_USER') else None
+        self.user_from_email = settings.GSUITE_USER_FROM_EMAIL if hasattr(settings, 'GSUITE_USER_FROM_EMAIL') else False
         self._lock = threading.RLock()
-        self.gmail_user = settings.GMAIL_USER
 
     def _delegate_user(self, user_id):
         credentials = service_account.Credentials.from_service_account_file(
             self.credentials, scopes=self.API_SCOPE)
         credentials_delegated = credentials.with_subject(user_id)
         return credentials_delegated
 
@@ -39,17 +40,18 @@
         import re
         
         if not email_messages:
             return 0
         with self._lock:
             num_sent = 0
             for message in email_messages:
-                encoding = message.encoding or settings.DEFAULT_CHARSET
-                self.gmail_user = sanitize_address(message.from_email, encoding)
-                self.gmail_user = re.findall(r"[a-z0-9\.\-+_]+@[a-z0-9\.\-+_]+\.[a-z]+", self.gmail_user)[0]
+                if self.user_from_email:
+                    encoding = message.encoding or settings.DEFAULT_CHARSET
+                    self.gmail_user = sanitize_address(message.from_email, encoding)
+                    self.gmail_user = re.findall(r"[a-z0-9\.\-+_]+@[a-z0-9\.\-+_]+\.[a-z]+", self.gmail_user)[0]
                 new_conn_created = self.open()
                 if not self.connection or new_conn_created is None:
                     # skip this message
                     continue
                 sent = self._send(message)
                 if sent:
                     num_sent += 1
```

### Comparing `djau_gsuite_email-0.1.4/django_gsuite_email/utils.py` & `djau_gsuite_email-0.1.5/django_gsuite_email/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -25,13 +25,17 @@
         if check_file(file_path):
             return file_path
 
     if environ.get('GSUITE_CREDENTIALS_FILE') is not None:
         file_path = environ.get('GSUITE_CREDENTIALS_FILE')
         if check_file(file_path):
             return file_path
-    raise ImproperlyConfigured('GSUITE_CREDENTIALS_FILE is not set, set it in seetings or as environment variable')
+    raise ImproperlyConfigured('GSUITE_CREDENTIALS_FILE is not set, set it in settings or as environment variable')
 
 
 
 def check_ready():
+    gmail_user = settings.GMAIL_USER if hasattr(settings, 'GMAIL_USER') else None
+    user_from_email = settings.GSUITE_USER_FROM_EMAIL if hasattr(settings, 'GSUITE_USER_FROM_EMAIL') else False
+    if gmail_user is None and not user_from_email:
+        raise ImproperlyConfigured('GMAIL_USER mandatory if GSUITE_USER_FROM_EMAIL is not True, set it in settings')
     return bool(get_credentials_file())
```

### Comparing `djau_gsuite_email-0.1.4/djau_gsuite_email.egg-info/PKG-INFO` & `djau_gsuite_email-0.1.5/djau_gsuite_email.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djau-gsuite-email
-Version: 0.1.4
+Version: 0.1.5
 Summary: Send emails via a GSuite Service-account.
 Home-page: https://github.com/slicefox/django-gsuite-email
 Author: slicefox
 Author-email: adithya.webdev@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -54,17 +54,22 @@
 EMAIL_BACKEND = 'django_gsuite_email.GSuiteEmailBackend'
 ```
 
 #### 3. Set location of credentials file.
 To do this, either set `GSUITE_CREDENTIALS_FILE` environment variable.\
 OR \
 set `GSUITE_CREDENTIALS_FILE` in `settings.py`
-````python
+
+```python
 GSUITE_CREDENTIALS_FILE="/path/to/credentials/file.json"
-````
+GSUITE_USER_FROM_EMAIL = False  # use the user of from_email if True. Default value False.
+GMAIL_USER = 'user@domain'      # default user if GSUITE_USER_FROM_EMAIL is not True. Default value None.
+GMAIL_SCOPES = ['https://www.googleapis.com/auth/gmail.send', ... ] # Default value ['https://www.googleapis.com/auth/gmail.send', ]
+```
+
 > #### Note: `GSUITE_CREDENTIALS_FILE` in `settings.py` will take precedence over environment variable.
 
 #### 4. Send emails
 ```python
 from django.core.mail import send_mail
 
 send_mail(
```

### Comparing `djau_gsuite_email-0.1.4/setup.py` & `djau_gsuite_email-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # Package meta-data.
 NAME = 'djau-gsuite-email'
 DESCRIPTION = 'Send emails via a GSuite Service-account.'
 URL = 'https://github.com/slicefox/django-gsuite-email'
 EMAIL = 'adithya.webdev@gmail.com'
 AUTHOR = 'slicefox'
 REQUIRES_PYTHON = '>=3.0.0'
-VERSION = '0.1.4'
+VERSION = '0.1.5'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
    'google-api-python-client>=1.8.0',
    'google-auth>=1.11.3'
 ]
```

