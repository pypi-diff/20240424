# Comparing `tmp/auth-checker-1.0.0.tar.gz` & `tmp/auth_checker-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auth-checker-1.0.0.tar", last modified: Thu Mar 16 19:06:33 2023, max compression
+gzip compressed data, was "auth_checker-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `auth-checker-1.0.0.tar` & `auth_checker-1.1.1.tar`

### file list

```diff
@@ -1,5 +1,18 @@
--rw-r--r--   0        0        0     1102 2023-01-20 21:12:43.401287 auth-checker-1.0.0/LICENSE
--rw-r--r--   0        0        0      254 2023-01-20 21:52:57.916220 auth-checker-1.0.0/README.md
--rw-r--r--   0        0        0     2787 2022-12-12 14:18:19.151786 auth-checker-1.0.0/auth_checker.py
--rw-r--r--   0        0        0      693 2023-03-16 18:59:52.067246 auth-checker-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 auth-checker-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      169 2024-04-24 19:25:54.465846 auth_checker-1.1.1/.coveragerc
+-rw-r--r--   0        0        0      296 2024-04-24 19:25:54.465846 auth_checker-1.1.1/.github/pr_template.md
+-rw-r--r--   0        0        0     9353 2024-04-24 19:25:54.465846 auth_checker-1.1.1/.github/workflows/test_publish_release.yml
+-rw-r--r--   0        0        0      242 2024-04-24 19:25:54.465846 auth_checker-1.1.1/.gitignore
+-rw-r--r--   0        0        0      875 2024-04-24 19:25:54.465846 auth_checker-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1102 2024-04-24 19:25:54.465846 auth_checker-1.1.1/LICENSE
+-rw-r--r--   0        0        0      589 2024-04-24 19:25:54.465846 auth_checker-1.1.1/Makefile
+-rw-r--r--   0        0        0      909 2024-04-24 19:25:54.465846 auth_checker-1.1.1/README.md
+-rw-r--r--   0        0        0       38 2024-04-24 19:25:54.465846 auth_checker-1.1.1/auth_checker/__init__.py
+-rw-r--r--   0        0        0     2610 2024-04-24 19:25:54.465846 auth_checker-1.1.1/auth_checker/auth_checker.py
+-rw-r--r--   0        0        0        0 2024-04-24 19:25:54.465846 auth_checker-1.1.1/auth_checker/tests/__init__.py
+-rw-r--r--   0        0        0     4932 2024-04-24 19:25:54.465846 auth_checker-1.1.1/auth_checker/tests/test_authchecker.py
+-rw-r--r--   0        0        0       60 2024-04-24 19:25:54.465846 auth_checker-1.1.1/envrc_sample
+-rw-r--r--   0        0        0     2559 2024-04-24 19:25:54.465846 auth_checker-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      219 2024-04-24 19:25:54.465846 auth_checker-1.1.1/pytest.ini
+-rw-r--r--   0        0        0      664 2024-04-24 19:25:54.465846 auth_checker-1.1.1/requirements/base/base.txt
+-rw-r--r--   0        0        0     2921 2024-04-24 19:25:54.465846 auth_checker-1.1.1/requirements/dev/dev.txt
+-rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 auth_checker-1.1.1/PKG-INFO
```

### Comparing `auth-checker-1.0.0/LICENSE` & `auth_checker-1.1.1/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 NC State Security Applications & Technologies
+Copyright (c) 2024 NC State Security Applications & Technologies
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `auth-checker-1.0.0/auth_checker.py` & `auth_checker-1.1.1/auth_checker/auth_checker.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,36 +33,28 @@
         Throw HTTP Exception if the user doesn't have all of the function's
         required authorizations.
         :param str authorization_header: the request's Authorization header.
             The header value is a JWT.
         """
         token = authorization_header.lstrip("Bearer").strip()
         if not token:
-            raise HTTPException(
-                401,
-                detail="No token provided in 'Authorization' header"
-            )
+            raise HTTPException(401, detail="No token provided in 'Authorization' header")
         try:
             secret = os.getenv("JWT_SECRET")
             if not secret:
-                raise HTTPException(
-                    400,
-                    detail="No environment variable JWT_SECRET found"
-                )
+                raise HTTPException(400, detail="No environment variable JWT_SECRET found")
             payload = jwt.decode(token, secret, algorithms=["HS256"])
         except jwt.exceptions.ExpiredSignatureError:
             raise HTTPException(401, detail="Token is expired")
         except jwt.exceptions.InvalidSignatureError:
-            raise HTTPException(400, detail=("Token has an invalid signature. "
-                                             "Check the JWT_SECRET variable."))
+            raise HTTPException(
+                400, detail=("Token has an invalid signature. " "Check the JWT_SECRET variable.")
+            )
 
         user_authorizations = payload.get("authorizations", {})
         if user_authorizations.get("root") is True:
             # Then the user is authorized. Continue without any exceptions.
             return
         for required_auth in self.required_authorizations:
             # Throw a 403 if the authorization isn't there or is set to False:
             if user_authorizations.get(required_auth, False) is False:
-                raise HTTPException(
-                    403,
-                    detail=f"{required_auth} authorization is required."
-                )
+                raise HTTPException(403, detail=f"{required_auth} authorization is required.")
```

