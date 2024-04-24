# Comparing `tmp/brightspacepyclient-0.0.3.tar.gz` & `tmp/brightspacepyclient-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brightspacepyclient-0.0.3.tar", last modified: Tue Apr 23 21:27:26 2024, max compression
+gzip compressed data, was "brightspacepyclient-0.0.4.tar", max compression
```

## Comparing `brightspacepyclient-0.0.3.tar` & `brightspacepyclient-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,3 @@
-drwxr-xr-x   0 jad        (501) staff       (20)        0 2024-04-23 21:27:26.254859 brightspacepyclient-0.0.3/
--rw-r--r--   0 jad        (501) staff       (20)      476 2024-04-23 21:27:26.254751 brightspacepyclient-0.0.3/PKG-INFO
-drwxr-xr-x   0 jad        (501) staff       (20)        0 2024-04-23 21:27:26.253173 brightspacepyclient-0.0.3/brightspace-py-client/
--rw-r--r--   0 jad        (501) staff       (20)       48 2024-04-23 21:01:36.000000 brightspacepyclient-0.0.3/brightspace-py-client/__init__.py
--rw-r--r--   0 jad        (501) staff       (20)     1774 2024-04-23 21:27:06.000000 brightspacepyclient-0.0.3/brightspace-py-client/brightspaceclient.py
-drwxr-xr-x   0 jad        (501) staff       (20)        0 2024-04-23 21:27:26.253292 brightspacepyclient-0.0.3/brightspace-py-client/src/
--rw-r--r--   0 jad        (501) staff       (20)      146 2024-04-23 21:24:40.000000 brightspacepyclient-0.0.3/brightspace-py-client/src/__init__.py
-drwxr-xr-x   0 jad        (501) staff       (20)        0 2024-04-23 21:27:26.253508 brightspacepyclient-0.0.3/brightspace-py-client/src/decorators/
--rw-r--r--   0 jad        (501) staff       (20)       30 2024-04-22 22:08:44.000000 brightspacepyclient-0.0.3/brightspace-py-client/src/decorators/__init__.py
--rw-r--r--   0 jad        (501) staff       (20)      320 2024-04-22 23:12:57.000000 brightspacepyclient-0.0.3/brightspace-py-client/src/decorators/decorators.py
-drwxr-xr-x   0 jad        (501) staff       (20)        0 2024-04-23 21:27:26.253722 brightspacepyclient-0.0.3/brightspace-py-client/src/models/
--rw-r--r--   0 jad        (501) staff       (20)      580 2024-04-22 22:58:03.000000 brightspacepyclient-0.0.3/brightspace-py-client/src/models/Response.py
--rw-r--r--   0 jad        (501) staff       (20)       50 2024-04-23 21:24:40.000000 brightspacepyclient-0.0.3/brightspace-py-client/src/models/__init__.py
-drwxr-xr-x   0 jad        (501) staff       (20)        0 2024-04-23 21:27:26.253948 brightspacepyclient-0.0.3/brightspace-py-client/src/utils/
--rw-r--r--   0 jad        (501) staff       (20)       51 2024-04-22 22:11:31.000000 brightspacepyclient-0.0.3/brightspace-py-client/src/utils/__init__.py
--rw-r--r--   0 jad        (501) staff       (20)      412 2024-04-22 22:13:27.000000 brightspacepyclient-0.0.3/brightspace-py-client/src/utils/requestswrapper.py
-drwxr-xr-x   0 jad        (501) staff       (20)        0 2024-04-23 21:27:26.254545 brightspacepyclient-0.0.3/brightspacepyclient.egg-info/
--rw-r--r--   0 jad        (501) staff       (20)      476 2024-04-23 21:27:26.000000 brightspacepyclient-0.0.3/brightspacepyclient.egg-info/PKG-INFO
--rw-r--r--   0 jad        (501) staff       (20)      622 2024-04-23 21:27:26.000000 brightspacepyclient-0.0.3/brightspacepyclient.egg-info/SOURCES.txt
--rw-r--r--   0 jad        (501) staff       (20)        1 2024-04-23 21:27:26.000000 brightspacepyclient-0.0.3/brightspacepyclient.egg-info/dependency_links.txt
--rw-r--r--   0 jad        (501) staff       (20)        9 2024-04-23 21:27:26.000000 brightspacepyclient-0.0.3/brightspacepyclient.egg-info/requires.txt
--rw-r--r--   0 jad        (501) staff       (20)       22 2024-04-23 21:27:26.000000 brightspacepyclient-0.0.3/brightspacepyclient.egg-info/top_level.txt
--rw-r--r--   0 jad        (501) staff       (20)       38 2024-04-23 21:27:26.254895 brightspacepyclient-0.0.3/setup.cfg
--rw-r--r--   0 jad        (501) staff       (20)      680 2024-04-23 21:27:13.000000 brightspacepyclient-0.0.3/setup.py
+-rw-r--r--   0        0        0      222 2024-04-24 01:01:44.832518 brightspacepyclient-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1796 2024-04-24 00:56:13.555568 brightspacepyclient-0.0.4/src/brightspacepyclient.py
+-rw-r--r--   0        0        0      387 1970-01-01 00:00:00.000000 brightspacepyclient-0.0.4/PKG-INFO
```

### Comparing `brightspacepyclient-0.0.3/brightspace-py-client/brightspaceclient.py` & `brightspacepyclient-0.0.4/src/brightspacepyclient.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from src import (RequestsSessionWrapper,
-                 ModuleResponse,
-                 AuthResponse)
+from utils.requestswrapper import RequestsSessionWrapper
+from decorators.decorators import unwrap
+
+import models
 
 
 class BrightSpaceClient:
     _version: float
     _session: RequestsSessionWrapper
 
     def __init__(self, base_url: str, d2lsessionval: str, d2lsecuresessionval: str, xcsrftoken: str,
@@ -16,15 +17,15 @@
         self._session = RequestsSessionWrapper(base_url)
         self._session.headers.update({"x-csrf-token": xcsrftoken})
         self._session.cookies.set("d2lSessionVal", d2lsessionval)
         self._session.cookies.set("d2lSecureSessionVal", d2lsecuresessionval)
 
     # Auth
     def get_access_token(self):
-        return AuthResponse(**self._session.post("/d2l/lp/auth/oauth2/token", {"scope": "*:*:*"}))
+        return models.AuthResponse(**self._session.post("/d2l/lp/auth/oauth2/token", {"scope": "*:*:*"}))
 
     # Root
     def get_my_enrollments(self):
         return self._session.get(f"/d2l/api/lp/{self._version}/enrollments/myenrollments/")
 
     # Organization a.k.a Course
     def get_users_in_org(self, org_unit_id: int):
@@ -32,12 +33,12 @@
 
     # Grades
     def get_student_grades_for_assessment(self, org_unit_id: int, assessment_id: int):
         return self._session.get(f"/d2l/api/le/{self._version}/{org_unit_id}/grades/{assessment_id}/values/")
 
     # Course Content
     def get_course_content(self, org_unit_id: int):
-        return list(map(lambda module: ModuleResponse(**module),
+        return list(map(lambda module: models.ModuleResponse(**module),
                         self._session.get(f"/d2l/api/le/{self._version}/{org_unit_id}/content/root/")))
 
     def get_attachment_for_content(self, org_unit_id: int, topic_id: int):
         return self._session.get(f"/d2l/api/le/{self._version}/{org_unit_id}/content/topics/{topic_id}/file/")
```

