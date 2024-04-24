# Comparing `tmp/drf_easily_auth-0.1.7.tar.gz` & `tmp/drf_easily_auth-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_easily_auth-0.1.7.tar", max compression
+gzip compressed data, was "drf_easily_auth-0.1.8.tar", max compression
```

## Comparing `drf_easily_auth-0.1.7.tar` & `drf_easily_auth-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1351 2024-04-21 07:13:07.732940 drf_easily_auth-0.1.7/README.md
--rw-r--r--   0        0        0        0 2024-04-20 16:52:04.771826 drf_easily_auth-0.1.7/drf_easily_auth/__init__.py
--rw-r--r--   0        0        0       99 2024-04-20 20:52:30.739037 drf_easily_auth-0.1.7/drf_easily_auth/admin.py
--rw-r--r--   0        0        0      876 2024-04-21 12:38:05.789001 drf_easily_auth-0.1.7/drf_easily_auth/apps.py
--rw-r--r--   0        0        0     1981 2024-04-21 07:03:41.564184 drf_easily_auth-0.1.7/drf_easily_auth/firebase.py
--rw-r--r--   0        0        0        0 2024-04-20 20:51:36.378447 drf_easily_auth-0.1.7/drf_easily_auth/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-20 20:51:36.378447 drf_easily_auth-0.1.7/drf_easily_auth/management/commands/__init__.py
--rw-r--r--   0        0        0     1881 2024-04-21 07:03:47.860231 drf_easily_auth-0.1.7/drf_easily_auth/management/commands/syncfirebaseusers.py
--rw-r--r--   0        0        0      957 2024-04-20 20:51:36.386448 drf_easily_auth-0.1.7/drf_easily_auth/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-04-20 20:51:36.386448 drf_easily_auth-0.1.7/drf_easily_auth/migrations/__init__.py
--rw-r--r--   0        0        0      473 2024-04-20 20:52:32.875060 drf_easily_auth-0.1.7/drf_easily_auth/models.py
--rw-r--r--   0        0        0       63 2024-04-20 20:51:36.418448 drf_easily_auth-0.1.7/drf_easily_auth/tests.py
--rw-r--r--   0        0        0      915 2024-04-21 07:17:40.129448 drf_easily_auth-0.1.7/drf_easily_auth/utils.py
--rw-r--r--   0        0        0      716 2024-04-21 12:40:02.345862 drf_easily_auth-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2175 1970-01-01 00:00:00.000000 drf_easily_auth-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1351 2024-04-21 07:13:07.732940 drf_easily_auth-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2024-04-20 16:52:04.771826 drf_easily_auth-0.1.8/drf_easily_auth/__init__.py
+-rw-r--r--   0        0        0       99 2024-04-20 20:52:30.739037 drf_easily_auth-0.1.8/drf_easily_auth/admin.py
+-rw-r--r--   0        0        0      876 2024-04-21 12:38:05.789001 drf_easily_auth-0.1.8/drf_easily_auth/apps.py
+-rw-r--r--   0        0        0     2016 2024-04-24 15:06:41.252038 drf_easily_auth-0.1.8/drf_easily_auth/firebase.py
+-rw-r--r--   0        0        0        0 2024-04-20 20:51:36.378447 drf_easily_auth-0.1.8/drf_easily_auth/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-20 20:51:36.378447 drf_easily_auth-0.1.8/drf_easily_auth/management/commands/__init__.py
+-rw-r--r--   0        0        0     1881 2024-04-21 07:03:47.860231 drf_easily_auth-0.1.8/drf_easily_auth/management/commands/syncfirebaseusers.py
+-rw-r--r--   0        0        0      957 2024-04-20 20:51:36.386448 drf_easily_auth-0.1.8/drf_easily_auth/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-20 20:51:36.386448 drf_easily_auth-0.1.8/drf_easily_auth/migrations/__init__.py
+-rw-r--r--   0        0        0      473 2024-04-20 20:52:32.875060 drf_easily_auth-0.1.8/drf_easily_auth/models.py
+-rw-r--r--   0        0        0       63 2024-04-20 20:51:36.418448 drf_easily_auth-0.1.8/drf_easily_auth/tests.py
+-rw-r--r--   0        0        0     1159 2024-04-24 15:09:04.305881 drf_easily_auth-0.1.8/drf_easily_auth/utils.py
+-rw-r--r--   0        0        0      716 2024-04-24 15:09:33.754258 drf_easily_auth-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2175 1970-01-01 00:00:00.000000 drf_easily_auth-0.1.8/PKG-INFO
```

### Comparing `drf_easily_auth-0.1.7/README.md` & `drf_easily_auth-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `drf_easily_auth-0.1.7/drf_easily_auth/apps.py` & `drf_easily_auth-0.1.8/drf_easily_auth/apps.py`

 * *Files identical despite different names*

### Comparing `drf_easily_auth-0.1.7/drf_easily_auth/firebase.py` & `drf_easily_auth-0.1.8/drf_easily_auth/firebase.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,21 +25,21 @@
             uid = decoded_token['uid']
             aud = decoded_token['aud']
             email = decoded_token['email']
             email_verified = decoded_token['email_verified']
             provider = decoded_token['firebase']['sign_in_provider']
 
         except auth.InvalidIdTokenError:
-            raise exceptions.AuthenticationFailed('Invalid authentication token.')
+            raise exceptions.AuthenticationFailed({'error': 'Invalid authentication token.'})
         except auth.ExpiredIdTokenError:
-            raise exceptions.AuthenticationFailed('Expired authentication token.')
+            raise exceptions.AuthenticationFailed({'error': 'Expired authentication token.'})
         except auth.RevokedIdTokenError:
-            raise exceptions.AuthenticationFailed('Revoked authentication token.')
+            raise exceptions.AuthenticationFailed({'error': 'Revoked authentication token.'})
         except Exception as e:
-            raise exceptions.AuthenticationFailed(f'Authentication failed: {str(e)}')
+            raise exceptions.AuthenticationFailed({'error': 'Could not authenticate.'})
 
         user, created = User.objects.get_or_create(username=uid, email=email)
         if created:
             # Disable user password
             user.set_unusable_password()
             user.save()
```

### Comparing `drf_easily_auth-0.1.7/drf_easily_auth/management/commands/syncfirebaseusers.py` & `drf_easily_auth-0.1.8/drf_easily_auth/management/commands/syncfirebaseusers.py`

 * *Files identical despite different names*

### Comparing `drf_easily_auth-0.1.7/drf_easily_auth/migrations/0001_initial.py` & `drf_easily_auth-0.1.8/drf_easily_auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf_easily_auth-0.1.7/drf_easily_auth/utils.py` & `drf_easily_auth-0.1.8/drf_easily_auth/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,8 +22,16 @@
             user.save()
 
             Firebase.objects.create(
                 user=user,
                 email_verified=firebase_user.email_verified,
                 sign_in_provider=firebase_user.provider_id
             )
-    return User.objects.all()
+    return User.objects.all()
+
+
+# Fonction pour ajouter des informations personnalisées à un utilisateur Firebase
+def add_custom_claims(uid: str, claims: dict) -> None:
+    """
+    Add custom claims to a Firebase user.
+    """
+    auth.set_custom_user_claims(uid, claims)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `drf_easily_auth-0.1.7/pyproject.toml` & `drf_easily_auth-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-easily-auth"
-version = "0.1.7"
+version = "0.1.8"
 description = "This package allows integration with Firebase for authentication outside the Django context."
 authors = ["Alexandre Meline <alexandre.meline.dev@gmail.com>"]
 readme = "README.md"
 keywords = [
     "Django",
     "Firebase",
     "Authentication",
```

### Comparing `drf_easily_auth-0.1.7/PKG-INFO` & `drf_easily_auth-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-easily-auth
-Version: 0.1.7
+Version: 0.1.8
 Summary: This package allows integration with Firebase for authentication outside the Django context.
 Home-page: https://github.com/alexandre-meline/drf_easily_auth/
 Keywords: Django,Firebase,Authentication,User Synchronization,DRF,Python,User Management,Security,API,JSON Web Tokens
 Author: Alexandre Meline
 Author-email: alexandre.meline.dev@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
```

