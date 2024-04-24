# Comparing `tmp/drf-social-oauth2-2.1.3.tar.gz` & `tmp/drf-social-oauth2-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-social-oauth2-2.1.3.tar", last modified: Tue Jun  6 12:16:39 2023, max compression
+gzip compressed data, was "drf-social-oauth2-2.2.0.tar", last modified: Wed Apr 24 17:35:01 2024, max compression
```

## Comparing `drf-social-oauth2-2.1.3.tar` & `drf-social-oauth2-2.2.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-06-06 12:16:39.088857 drf-social-oauth2-2.1.3/
--rw-r--r--   0 wagner.delima   (502) staff       (20)     7573 2023-05-01 09:46:25.000000 drf-social-oauth2-2.1.3/CHANGELOG.rst
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1080 2020-06-27 18:20:06.000000 drf-social-oauth2-2.1.3/LICENSE.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)       81 2020-06-27 18:20:06.000000 drf-social-oauth2-2.1.3/MANIFEST.in
--rw-r--r--   0 wagner.delima   (502) staff       (20)     2066 2023-06-06 12:16:39.088291 drf-social-oauth2-2.1.3/PKG-INFO
--rw-r--r--   0 wagner.delima   (502) staff       (20)      933 2023-04-25 12:21:07.000000 drf-social-oauth2-2.1.3/README.rst
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-06-06 12:16:39.075070 drf-social-oauth2-2.1.3/drf_social_oauth2/
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1379 2023-06-06 12:15:46.000000 drf-social-oauth2-2.1.3/drf_social_oauth2/__init__.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     2962 2023-05-01 09:46:25.000000 drf-social-oauth2-2.1.3/drf_social_oauth2/authentication.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1253 2023-05-01 09:46:25.000000 drf-social-oauth2-2.1.3/drf_social_oauth2/backends.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1166 2022-01-06 11:17:42.000000 drf-social-oauth2-2.1.3/drf_social_oauth2/oauth2_backends.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     5664 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.3/drf_social_oauth2/oauth2_endpoints.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     4637 2023-05-01 09:46:25.000000 drf-social-oauth2-2.1.3/drf_social_oauth2/oauth2_grants.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)      948 2023-06-06 12:15:46.000000 drf-social-oauth2-2.1.3/drf_social_oauth2/serializers.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)      558 2023-06-06 12:07:13.000000 drf-social-oauth2-2.1.3/drf_social_oauth2/settings.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     2135 2023-05-01 20:51:46.000000 drf-social-oauth2-2.1.3/drf_social_oauth2/test_settings.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     2158 2023-06-06 12:07:13.000000 drf-social-oauth2-2.1.3/drf_social_oauth2/urls.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     8791 2023-06-06 12:07:13.000000 drf-social-oauth2-2.1.3/drf_social_oauth2/views.py
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-06-06 12:16:39.080268 drf-social-oauth2-2.1.3/drf_social_oauth2.egg-info/
--rw-r--r--   0 wagner.delima   (502) staff       (20)     2066 2023-06-06 12:16:38.000000 drf-social-oauth2-2.1.3/drf_social_oauth2.egg-info/PKG-INFO
--rw-r--r--   0 wagner.delima   (502) staff       (20)      901 2023-06-06 12:16:39.000000 drf-social-oauth2-2.1.3/drf_social_oauth2.egg-info/SOURCES.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)        1 2023-06-06 12:16:38.000000 drf-social-oauth2-2.1.3/drf_social_oauth2.egg-info/dependency_links.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)        1 2023-05-01 18:49:32.000000 drf-social-oauth2-2.1.3/drf_social_oauth2.egg-info/not-zip-safe
--rw-r--r--   0 wagner.delima   (502) staff       (20)      120 2023-06-06 12:16:38.000000 drf-social-oauth2-2.1.3/drf_social_oauth2.egg-info/requires.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)       24 2023-06-06 12:16:38.000000 drf-social-oauth2-2.1.3/drf_social_oauth2.egg-info/top_level.txt
--rw-r--r--   0 wagner.delima   (502) staff       (20)      274 2023-03-26 14:58:52.000000 drf-social-oauth2-2.1.3/pyproject.toml
--rw-r--r--   0 wagner.delima   (502) staff       (20)       38 2023-06-06 12:16:39.089066 drf-social-oauth2-2.1.3/setup.cfg
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1276 2023-05-01 21:14:10.000000 drf-social-oauth2-2.1.3/setup.py
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-06-06 12:16:39.080966 drf-social-oauth2-2.1.3/tests/
--rw-r--r--   0 wagner.delima   (502) staff       (20)        0 2020-08-30 10:08:43.000000 drf-social-oauth2-2.1.3/tests/__init__.py
-drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2023-06-06 12:16:39.085807 drf-social-oauth2-2.1.3/tests/drf_social_oauth2/
--rw-r--r--   0 wagner.delima   (502) staff       (20)        0 2023-04-22 11:25:22.000000 drf-social-oauth2-2.1.3/tests/drf_social_oauth2/__init__.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     1560 2023-04-22 18:56:44.000000 drf-social-oauth2-2.1.3/tests/drf_social_oauth2/drf_fixtures.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     3241 2023-05-01 09:46:25.000000 drf-social-oauth2-2.1.3/tests/drf_social_oauth2/test_authentication.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     4538 2023-05-01 09:46:25.000000 drf-social-oauth2-2.1.3/tests/drf_social_oauth2/test_oauth2_endpoints.py
--rw-r--r--   0 wagner.delima   (502) staff       (20)     7226 2023-05-01 09:46:25.000000 drf-social-oauth2-2.1.3/tests/drf_social_oauth2/test_views.py
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2024-04-24 17:35:01.532401 drf-social-oauth2-2.2.0/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     7573 2023-05-01 09:46:25.000000 drf-social-oauth2-2.2.0/CHANGELOG.rst
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1080 2020-06-27 18:20:06.000000 drf-social-oauth2-2.2.0/LICENSE.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)       81 2020-06-27 18:20:06.000000 drf-social-oauth2-2.2.0/MANIFEST.in
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     2136 2024-04-24 17:35:01.532078 drf-social-oauth2-2.2.0/PKG-INFO
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1003 2023-09-21 11:27:47.000000 drf-social-oauth2-2.2.0/README.rst
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2024-04-24 17:35:01.527005 drf-social-oauth2-2.2.0/drf_social_oauth2/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1369 2024-04-24 17:34:56.000000 drf-social-oauth2-2.2.0/drf_social_oauth2/__init__.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     2962 2023-05-01 09:46:25.000000 drf-social-oauth2-2.2.0/drf_social_oauth2/authentication.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1253 2023-05-01 09:46:25.000000 drf-social-oauth2-2.2.0/drf_social_oauth2/backends.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1166 2022-01-06 11:17:42.000000 drf-social-oauth2-2.2.0/drf_social_oauth2/oauth2_backends.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     5664 2024-04-24 17:04:50.000000 drf-social-oauth2-2.2.0/drf_social_oauth2/oauth2_endpoints.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     4637 2023-05-01 09:46:25.000000 drf-social-oauth2-2.2.0/drf_social_oauth2/oauth2_grants.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      948 2024-04-24 17:04:55.000000 drf-social-oauth2-2.2.0/drf_social_oauth2/serializers.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      558 2023-06-06 12:07:13.000000 drf-social-oauth2-2.2.0/drf_social_oauth2/settings.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     2135 2023-05-01 20:51:46.000000 drf-social-oauth2-2.2.0/drf_social_oauth2/test_settings.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     2158 2023-06-06 12:07:13.000000 drf-social-oauth2-2.2.0/drf_social_oauth2/urls.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     9397 2023-09-21 11:27:47.000000 drf-social-oauth2-2.2.0/drf_social_oauth2/views.py
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2024-04-24 17:35:01.529233 drf-social-oauth2-2.2.0/drf_social_oauth2.egg-info/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     2136 2024-04-24 17:35:01.000000 drf-social-oauth2-2.2.0/drf_social_oauth2.egg-info/PKG-INFO
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      901 2024-04-24 17:35:01.000000 drf-social-oauth2-2.2.0/drf_social_oauth2.egg-info/SOURCES.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)        1 2024-04-24 17:35:01.000000 drf-social-oauth2-2.2.0/drf_social_oauth2.egg-info/dependency_links.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)        1 2023-05-01 18:49:32.000000 drf-social-oauth2-2.2.0/drf_social_oauth2.egg-info/not-zip-safe
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      100 2024-04-24 17:35:01.000000 drf-social-oauth2-2.2.0/drf_social_oauth2.egg-info/requires.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)       24 2024-04-24 17:35:01.000000 drf-social-oauth2-2.2.0/drf_social_oauth2.egg-info/top_level.txt
+-rw-r--r--   0 wagner.delima   (502) staff       (20)      254 2024-04-24 17:04:55.000000 drf-social-oauth2-2.2.0/pyproject.toml
+-rw-r--r--   0 wagner.delima   (502) staff       (20)       38 2024-04-24 17:35:01.532533 drf-social-oauth2-2.2.0/setup.cfg
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1255 2024-04-24 17:04:55.000000 drf-social-oauth2-2.2.0/setup.py
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2024-04-24 17:35:01.529558 drf-social-oauth2-2.2.0/tests/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)        0 2020-08-30 10:08:43.000000 drf-social-oauth2-2.2.0/tests/__init__.py
+drwxr-xr-x   0 wagner.delima   (502) staff       (20)        0 2024-04-24 17:35:01.531340 drf-social-oauth2-2.2.0/tests/drf_social_oauth2/
+-rw-r--r--   0 wagner.delima   (502) staff       (20)        0 2023-04-22 11:25:22.000000 drf-social-oauth2-2.2.0/tests/drf_social_oauth2/__init__.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     1560 2023-04-22 18:56:44.000000 drf-social-oauth2-2.2.0/tests/drf_social_oauth2/drf_fixtures.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     3241 2023-05-01 09:46:25.000000 drf-social-oauth2-2.2.0/tests/drf_social_oauth2/test_authentication.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     4538 2024-04-24 17:04:50.000000 drf-social-oauth2-2.2.0/tests/drf_social_oauth2/test_oauth2_endpoints.py
+-rw-r--r--   0 wagner.delima   (502) staff       (20)     7226 2023-05-01 09:46:25.000000 drf-social-oauth2-2.2.0/tests/drf_social_oauth2/test_views.py
```

### Comparing `drf-social-oauth2-2.1.3/CHANGELOG.rst` & `drf-social-oauth2-2.2.0/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.3/LICENSE.txt` & `drf-social-oauth2-2.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.3/PKG-INFO` & `drf-social-oauth2-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-social-oauth2
-Version: 2.1.3
+Version: 2.2.0
 Summary:  drf-social-oauth2 is a frameworks meant to be used with Django and Django Rest Framework. drf-social-oauth2 offers support to oauth2 authentication and authorization. It's one of the easiest frameworks to integrate Oauth2 to your Django Rest Framework application. By using drf-social-oauth2 you can authenticate with major vendors such as Google, Facebook, Instagram, Github, Twitter and a ton more! 
 Home-page: https://github.com/wagnerdelima/drf-social-oauth2
 Author: Wagner de Lima
 Author-email: waglds@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -39,17 +39,19 @@
 ---------------------
 
 You can read the whole drf-social-oauth2's documentation at: https://drf-social-oauth2.readthedocs.io/en/latest/.
 
 Contributing
 ------------
 
-Details `here <https://github.com/wagnerdelima/drf-social-oauth2/blob/master/CONTRIBUTING.md.>`_
+Details `here <https://github.com/wagnerdelima/drf-social-oauth2/blob/master/CONTRIBUTING.md#:~:text=CODE_OF_CONDUCT.md-,CONTRIBUTING,-.md.>`_
 
 What Am I Working Next?
 ^^^^^^^^^^^^^^^^^^^^^^^
 
 I will be working on the issues below. Anyone is welcome to contribute.
 
     - Investigating Issues.
 
+From Spain, with Love.
+
```

### Comparing `drf-social-oauth2-2.1.3/README.rst` & `drf-social-oauth2-2.2.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 ---------------------
 
 You can read the whole drf-social-oauth2's documentation at: https://drf-social-oauth2.readthedocs.io/en/latest/.
 
 Contributing
 ------------
 
-Details `here <https://github.com/wagnerdelima/drf-social-oauth2/blob/master/CONTRIBUTING.md.>`_
+Details `here <https://github.com/wagnerdelima/drf-social-oauth2/blob/master/CONTRIBUTING.md#:~:text=CODE_OF_CONDUCT.md-,CONTRIBUTING,-.md.>`_
 
 What Am I Working Next?
 ^^^^^^^^^^^^^^^^^^^^^^^
 
 I will be working on the issues below. Anyone is welcome to contribute.
 
     - Investigating Issues.
+
+From Spain, with Love.
```

### Comparing `drf-social-oauth2-2.1.3/drf_social_oauth2/__init__.py` & `drf-social-oauth2-2.2.0/drf_social_oauth2/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 drf-social-oauth2 is a frameworks meant to be used with Django and Django Rest Framework.
 drf-social-oauth2 offers support to oauth2 authentication and authorization.
 It's one of the easiest frameworks to integrate Oauth2 to your Django Rest Framework application.
 By using drf-social-oauth2 you can authenticate with major vendors such as Google, Facebook, Instagram, Github, Twitter
 and a ton more!
 """
 
-__version__ = '2.1.3'
+__version__ = '2.2.0'
 
 try:
     from secrets import SystemRandom
 except ImportError:
     from random import SystemRandom
 
 
@@ -23,15 +23,15 @@
     """Generates a non-guessable OAuth Json Web Token
     OAuth (1 and 2) does not specify the format of tokens except that they
     should be strings of random characters. Tokens should not be guessable
     and entropy when generating the random characters is important. Which is
     why SystemRandom is used instead of the default random.choice method.
     """
     from django.conf import settings
-    from jose import jwt
+    import jwt
 
     rand = SystemRandom()
     secret = getattr(settings, 'SECRET_KEY')
 
     token = ''.join(rand.choice(chars) for x in range(length))
     jwtted_token = jwt.encode({'token': token}, secret, algorithm='HS256')
     return jwtted_token
```

### Comparing `drf-social-oauth2-2.1.3/drf_social_oauth2/authentication.py` & `drf-social-oauth2-2.2.0/drf_social_oauth2/authentication.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.3/drf_social_oauth2/backends.py` & `drf-social-oauth2-2.2.0/drf_social_oauth2/backends.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.3/drf_social_oauth2/oauth2_backends.py` & `drf-social-oauth2-2.2.0/drf_social_oauth2/oauth2_backends.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.3/drf_social_oauth2/oauth2_endpoints.py` & `drf-social-oauth2-2.2.0/drf_social_oauth2/oauth2_endpoints.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.3/drf_social_oauth2/oauth2_grants.py` & `drf-social-oauth2-2.2.0/drf_social_oauth2/oauth2_grants.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.3/drf_social_oauth2/serializers.py` & `drf-social-oauth2-2.2.0/drf_social_oauth2/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 
 
 class ConvertTokenSerializer(Serializer):
     grant_type = CharField(max_length=50)
     backend = CharField(max_length=200)
     client_id = CharField(max_length=200)
     client_secret = CharField(max_length=500)
-    token = CharField(max_length=2000)
+    token = CharField(max_length=5000)
 
 
 class RevokeTokenSerializer(Serializer):
     client_id = CharField(max_length=200)
     client_secret = CharField(max_length=500)
-    token = CharField(max_length=2000)
+    token = CharField(max_length=5000)
 
 
 class DisconnectBackendSerializer(Serializer):
     backend = CharField(max_length=200)
     association_id = IntegerField()
```

### Comparing `drf-social-oauth2-2.1.3/drf_social_oauth2/settings.py` & `drf-social-oauth2-2.2.0/drf_social_oauth2/settings.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.3/drf_social_oauth2/test_settings.py` & `drf-social-oauth2-2.2.0/drf_social_oauth2/test_settings.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.3/drf_social_oauth2/urls.py` & `drf-social-oauth2-2.2.0/drf_social_oauth2/urls.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.3/drf_social_oauth2/views.py` & `drf-social-oauth2-2.2.0/drf_social_oauth2/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,14 +129,30 @@
                 status=HTTP_400_BAD_REQUEST,
             )
         except AccessDeniedError:
             return Response(
                 {'access_denied': f'The token you provided is invalid or expired.'},
                 status=HTTP_400_BAD_REQUEST,
             )
+        except IntegrityError as e:
+            if 'email' in str(e) and 'already exists' in str(e):
+                return Response(
+                    {'error': 'A user with this email already exists.'},
+                    status=HTTP_400_BAD_REQUEST,
+                )
+            else:
+                return Response(
+                    {'error': 'Database error.'},
+                    status=HTTP_400_BAD_REQUEST,
+                )
+        except Exception as e:
+            return Response(
+                {'error': str(e)},
+                status=HTTP_500_INTERNAL_SERVER_ERROR,
+            )
 
         return Response(data=json_loads(body), status=status)
 
 
 class RevokeTokenView(CsrfExemptMixin, OAuthLibMixin, APIView):
     """
     Implements an endpoint to revoke access or refresh tokens
```

### Comparing `drf-social-oauth2-2.1.3/drf_social_oauth2.egg-info/PKG-INFO` & `drf-social-oauth2-2.2.0/drf_social_oauth2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-social-oauth2
-Version: 2.1.3
+Version: 2.2.0
 Summary:  drf-social-oauth2 is a frameworks meant to be used with Django and Django Rest Framework. drf-social-oauth2 offers support to oauth2 authentication and authorization. It's one of the easiest frameworks to integrate Oauth2 to your Django Rest Framework application. By using drf-social-oauth2 you can authenticate with major vendors such as Google, Facebook, Instagram, Github, Twitter and a ton more! 
 Home-page: https://github.com/wagnerdelima/drf-social-oauth2
 Author: Wagner de Lima
 Author-email: waglds@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -39,17 +39,19 @@
 ---------------------
 
 You can read the whole drf-social-oauth2's documentation at: https://drf-social-oauth2.readthedocs.io/en/latest/.
 
 Contributing
 ------------
 
-Details `here <https://github.com/wagnerdelima/drf-social-oauth2/blob/master/CONTRIBUTING.md.>`_
+Details `here <https://github.com/wagnerdelima/drf-social-oauth2/blob/master/CONTRIBUTING.md#:~:text=CODE_OF_CONDUCT.md-,CONTRIBUTING,-.md.>`_
 
 What Am I Working Next?
 ^^^^^^^^^^^^^^^^^^^^^^^
 
 I will be working on the issues below. Anyone is welcome to contribute.
 
     - Investigating Issues.
 
+From Spain, with Love.
+
```

### Comparing `drf-social-oauth2-2.1.3/drf_social_oauth2.egg-info/SOURCES.txt` & `drf-social-oauth2-2.2.0/drf_social_oauth2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.3/setup.py` & `drf-social-oauth2-2.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,12 +26,12 @@
         'Intended Audience :: Information Technology',
         'Natural Language :: English',
     ],
     install_requires=[
         'djangorestframework>=3.10.3',
         'django-oauth-toolkit>=0.12.0',
         'social-auth-app-django>=3.1.0',
-        'python-jose[cryptography]>=3.3.0',
+        'PyJWT>=2.8.0'
     ],
     include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `drf-social-oauth2-2.1.3/tests/drf_social_oauth2/drf_fixtures.py` & `drf-social-oauth2-2.2.0/tests/drf_social_oauth2/drf_fixtures.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.3/tests/drf_social_oauth2/test_authentication.py` & `drf-social-oauth2-2.2.0/tests/drf_social_oauth2/test_authentication.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.3/tests/drf_social_oauth2/test_oauth2_endpoints.py` & `drf-social-oauth2-2.2.0/tests/drf_social_oauth2/test_oauth2_endpoints.py`

 * *Files identical despite different names*

### Comparing `drf-social-oauth2-2.1.3/tests/drf_social_oauth2/test_views.py` & `drf-social-oauth2-2.2.0/tests/drf_social_oauth2/test_views.py`

 * *Files identical despite different names*

