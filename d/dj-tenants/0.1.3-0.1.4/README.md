# Comparing `tmp/dj_tenants-0.1.3.tar.gz` & `tmp/dj_tenants-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_tenants-0.1.3.tar", max compression
+gzip compressed data, was "dj_tenants-0.1.4.tar", max compression
```

## Comparing `dj_tenants-0.1.3.tar` & `dj_tenants-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1148 2024-04-16 21:50:11.453241 dj_tenants-0.1.3/dj_tenants/__init__.py
--rw-r--r--   0        0        0      411 2024-04-16 10:59:47.143776 dj_tenants-0.1.3/dj_tenants/apps.py
--rw-r--r--   0        0        0      324 2024-04-16 23:38:59.972309 dj_tenants-0.1.3/dj_tenants/conf.py
--rw-r--r--   0        0        0      996 2024-04-16 10:44:41.535837 dj_tenants-0.1.3/dj_tenants/context.py
--rw-r--r--   0        0        0       46 2024-04-16 10:06:02.548359 dj_tenants-0.1.3/dj_tenants/exceptions.py
--rw-r--r--   0        0        0     1500 2024-04-16 23:52:01.054742 dj_tenants-0.1.3/dj_tenants/middleware.py
--rw-r--r--   0        0        0     1295 2024-04-16 21:18:08.416811 dj_tenants-0.1.3/dj_tenants/models.py
--rw-r--r--   0        0        0        0 2024-04-16 11:29:02.214763 dj_tenants-0.1.3/dj_tenants/postgres_backend/__init__.py
--rw-r--r--   0        0        0      434 2024-04-16 11:55:58.663429 dj_tenants-0.1.3/dj_tenants/postgres_backend/base.py
--rw-r--r--   0        0        0     3666 2024-04-16 21:17:16.930323 dj_tenants-0.1.3/dj_tenants/postgres_backend/compiler.py
--rw-r--r--   0        0        0      224 2024-04-16 11:55:44.287371 dj_tenants-0.1.3/dj_tenants/postgres_backend/operations.py
--rw-r--r--   0        0        0      819 2024-04-16 14:33:07.299762 dj_tenants-0.1.3/dj_tenants/utils.py
--rw-r--r--   0        0        0      606 2024-04-16 23:52:13.338829 dj_tenants-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 03:34:42.506337 dj_tenants-0.1.3/README.md
--rw-r--r--   0        0        0      381 1970-01-01 00:00:00.000000 dj_tenants-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      849 2024-04-24 19:09:38.485122 dj_tenants-0.1.4/dj_tenants/__init__.py
+-rw-r--r--   0        0        0      411 2024-04-16 10:59:47.143776 dj_tenants-0.1.4/dj_tenants/apps.py
+-rw-r--r--   0        0        0      324 2024-04-16 23:38:59.972309 dj_tenants-0.1.4/dj_tenants/conf.py
+-rw-r--r--   0        0        0      996 2024-04-16 10:44:41.535837 dj_tenants-0.1.4/dj_tenants/context.py
+-rw-r--r--   0        0        0       46 2024-04-16 10:06:02.548359 dj_tenants-0.1.4/dj_tenants/exceptions.py
+-rw-r--r--   0        0        0     1354 2024-04-24 19:12:07.189740 dj_tenants-0.1.4/dj_tenants/middleware.py
+-rw-r--r--   0        0        0     1195 2024-04-24 19:08:03.595203 dj_tenants-0.1.4/dj_tenants/models.py
+-rw-r--r--   0        0        0        0 2024-04-16 11:29:02.214763 dj_tenants-0.1.4/dj_tenants/postgres_backend/__init__.py
+-rw-r--r--   0        0        0      434 2024-04-16 11:55:58.663429 dj_tenants-0.1.4/dj_tenants/postgres_backend/base.py
+-rw-r--r--   0        0        0     1639 2024-04-24 19:03:38.485193 dj_tenants-0.1.4/dj_tenants/postgres_backend/compiler.py
+-rw-r--r--   0        0        0      224 2024-04-16 11:55:44.287371 dj_tenants-0.1.4/dj_tenants/postgres_backend/operations.py
+-rw-r--r--   0        0        0      819 2024-04-16 14:33:07.299762 dj_tenants-0.1.4/dj_tenants/utils.py
+-rw-r--r--   0        0        0      606 2024-04-24 19:14:08.526446 dj_tenants-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 03:34:42.506337 dj_tenants-0.1.4/README.md
+-rw-r--r--   0        0        0      381 1970-01-01 00:00:00.000000 dj_tenants-0.1.4/PKG-INFO
```

### Comparing `dj_tenants-0.1.3/dj_tenants/context.py` & `dj_tenants-0.1.4/dj_tenants/context.py`

 * *Files identical despite different names*

### Comparing `dj_tenants-0.1.3/dj_tenants/middleware.py` & `dj_tenants-0.1.4/dj_tenants/middleware.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,18 +17,14 @@
         self.get_response = get_response
         self.TenantModel = get_tenant_model()
 
     def __call__(self, request):
         if not request.user.is_authenticated:
             return self.get_response(request)
 
-        if request.path.startswith("/admin/"):
-            with tenant_context_disabled():
-                return self.get_response(request)
-
         ignored_path = any(
             resolve(request.path).view_name == ignored for ignored in allowed_paths
         )
         if ignored_path:
             with tenant_context_disabled():
                 return self.get_response(request)
```

### Comparing `dj_tenants-0.1.3/dj_tenants/utils.py` & `dj_tenants-0.1.4/dj_tenants/utils.py`

 * *Files identical despite different names*

### Comparing `dj_tenants-0.1.3/pyproject.toml` & `dj_tenants-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dj-tenants"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Hugo Mesquita <hugohomesquita@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "dj_tenants" }]
 
 [tool.poetry.dependencies]
 python = "^3.12"
```

