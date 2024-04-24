# Comparing `tmp/remote_job_app-0.1.6.tar.gz` & `tmp/remote_job_app-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remote_job_app-0.1.6.tar", max compression
+gzip compressed data, was "remote_job_app-0.1.7.tar", max compression
```

## Comparing `remote_job_app-0.1.6.tar` & `remote_job_app-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0      136 2024-03-20 13:32:06.382852 remote_job_app-0.1.6/README.md
--rw-r--r--   0        0        0      803 2024-03-20 13:32:20.419057 remote_job_app-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-20 13:32:06.382852 remote_job_app-0.1.6/strangeworks_remote_job/__init__.py
--rw-r--r--   0        0        0     3333 2024-03-20 13:32:06.382852 remote_job_app-0.1.6/strangeworks_remote_job/app/__init__.py
--rw-r--r--   0        0        0     2268 2024-03-20 13:32:06.382852 remote_job_app-0.1.6/strangeworks_remote_job/app/main.py
--rw-r--r--   0        0        0     1966 2024-03-20 13:32:06.382852 remote_job_app-0.1.6/strangeworks_remote_job/app/middleware.py
--rw-r--r--   0        0        0        0 2024-03-20 13:32:06.382852 remote_job_app-0.1.6/strangeworks_remote_job/app/routers/__init__.py
--rw-r--r--   0        0        0     1785 2024-03-20 13:32:06.382852 remote_job_app-0.1.6/strangeworks_remote_job/app/routers/jobs.py
--rw-r--r--   0        0        0      798 2024-03-20 13:32:06.386852 remote_job_app-0.1.6/strangeworks_remote_job/app/routers/types/job.py
--rw-r--r--   0        0        0     1089 2024-03-20 13:32:06.382852 remote_job_app-0.1.6/strangeworks_remote_job/app.py
--rw-r--r--   0        0        0     1896 2024-03-20 13:32:06.386852 remote_job_app-0.1.6/strangeworks_remote_job/artifact.py
--rw-r--r--   0        0        0    15035 2024-03-20 13:32:06.386852 remote_job_app-0.1.6/strangeworks_remote_job/basic.py
--rw-r--r--   0        0        0     1486 2024-03-20 13:32:06.386852 remote_job_app-0.1.6/strangeworks_remote_job/ex.py
--rw-r--r--   0        0        0     2814 2024-03-20 13:32:06.386852 remote_job_app-0.1.6/strangeworks_remote_job/remote.py
--rw-r--r--   0        0        0      669 1970-01-01 00:00:00.000000 remote_job_app-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      136 2024-04-24 13:20:24.948196 remote_job_app-0.1.7/README.md
+-rw-r--r--   0        0        0      803 2024-04-24 13:20:35.952210 remote_job_app-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-24 13:20:24.948196 remote_job_app-0.1.7/strangeworks_remote_job/__init__.py
+-rw-r--r--   0        0        0     1437 2024-04-24 13:20:24.948196 remote_job_app-0.1.7/strangeworks_remote_job/admin.py
+-rw-r--r--   0        0        0     3333 2024-04-24 13:20:24.948196 remote_job_app-0.1.7/strangeworks_remote_job/app/__init__.py
+-rw-r--r--   0        0        0     2333 2024-04-24 13:20:24.948196 remote_job_app-0.1.7/strangeworks_remote_job/app/main.py
+-rw-r--r--   0        0        0     3082 2024-04-24 13:20:24.948196 remote_job_app-0.1.7/strangeworks_remote_job/app/middleware.py
+-rw-r--r--   0        0        0        0 2024-04-24 13:20:24.948196 remote_job_app-0.1.7/strangeworks_remote_job/app/routers/__init__.py
+-rw-r--r--   0        0        0      498 2024-04-24 13:20:24.948196 remote_job_app-0.1.7/strangeworks_remote_job/app/routers/admin.py
+-rw-r--r--   0        0        0     1785 2024-04-24 13:20:24.948196 remote_job_app-0.1.7/strangeworks_remote_job/app/routers/jobs.py
+-rw-r--r--   0        0        0      798 2024-04-24 13:20:24.948196 remote_job_app-0.1.7/strangeworks_remote_job/app/routers/types/job.py
+-rw-r--r--   0        0        0     1089 2024-04-24 13:20:24.948196 remote_job_app-0.1.7/strangeworks_remote_job/app.py
+-rw-r--r--   0        0        0     1896 2024-04-24 13:20:24.948196 remote_job_app-0.1.7/strangeworks_remote_job/artifact.py
+-rw-r--r--   0        0        0    15076 2024-04-24 13:20:24.948196 remote_job_app-0.1.7/strangeworks_remote_job/basic.py
+-rw-r--r--   0        0        0     1486 2024-04-24 13:20:24.948196 remote_job_app-0.1.7/strangeworks_remote_job/ex.py
+-rw-r--r--   0        0        0     2814 2024-04-24 13:20:24.948196 remote_job_app-0.1.7/strangeworks_remote_job/remote.py
+-rw-r--r--   0        0        0      669 1970-01-01 00:00:00.000000 remote_job_app-0.1.7/PKG-INFO
```

### Comparing `remote_job_app-0.1.6/pyproject.toml` & `remote_job_app-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "remote-job-app"
-version = "0.1.6"
+version = "0.1.7"
 description = "Remote Job API"
 authors = ["Your Name <you@example.com>"]
 packages = [{ include = "strangeworks_remote_job" }]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `remote_job_app-0.1.6/strangeworks_remote_job/app/__init__.py` & `remote_job_app-0.1.7/strangeworks_remote_job/app/__init__.py`

 * *Files identical despite different names*

### Comparing `remote_job_app-0.1.6/strangeworks_remote_job/app/main.py` & `remote_job_app-0.1.7/strangeworks_remote_job/app/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """main.py."""
+
 import logging
 import os
 
 from fastapi import FastAPI, Request, status
 from fastapi.responses import JSONResponse
 from strangeworks_core.config.config import Config
 from strangeworks_core.errors.error import StrangeworksError
 
 from strangeworks_remote_job.app.middleware import RequestContextMiddleware
-from strangeworks_remote_job.app.routers import jobs
+from strangeworks_remote_job.app.routers import admin, jobs
 
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger("strangeworks_remote_job")
 gql_logger = logging.getLogger("gql.transport.requests")
 gql_logger.setLevel(logging.DEBUG)
 
@@ -73,12 +74,14 @@
     return JSONResponse(status_code=400, content={"error": exc.message})
 
 
 # add routers
 app.add_middleware(RequestContextMiddleware)
 
 app.include_router(jobs.router)
+app.include_router(admin.router)
 
 
 @app.get("/", status_code=status.HTTP_200_OK)
 async def health_check():
+    """Health check."""
     return {"status": "ok"}
```

### Comparing `remote_job_app-0.1.6/strangeworks_remote_job/app/routers/jobs.py` & `remote_job_app-0.1.7/strangeworks_remote_job/app/routers/jobs.py`

 * *Files identical despite different names*

### Comparing `remote_job_app-0.1.6/strangeworks_remote_job/app/routers/types/job.py` & `remote_job_app-0.1.7/strangeworks_remote_job/app/routers/types/job.py`

 * *Files identical despite different names*

### Comparing `remote_job_app-0.1.6/strangeworks_remote_job/app.py` & `remote_job_app-0.1.7/strangeworks_remote_job/app.py`

 * *Files identical despite different names*

### Comparing `remote_job_app-0.1.6/strangeworks_remote_job/artifact.py` & `remote_job_app-0.1.7/strangeworks_remote_job/artifact.py`

 * *Files identical despite different names*

### Comparing `remote_job_app-0.1.6/strangeworks_remote_job/basic.py` & `remote_job_app-0.1.7/strangeworks_remote_job/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,17 +235,18 @@
             logging.info(f"uploaded result for job {job_slug}")
             # call remote cleanup...
             try:
                 logging.info(
                     f"Calling cleanup_at_exit for job {job_slug} (remote id {remote_id}"
                 )
                 remote_api.finalize(remote_id=remote_id, remote_status=remote_status)
-            except Exception:
+            except Exception as err:
                 # log this for now since there is nothing that the caller can do.
-                logging.exception(f"Error from cleanup_at_exit for job {job_slug}")
+                logging.error(f"Error from cleanup_at_exit for job {job_slug}")
+                logging.exception(err)
 
             if artifact_generator:
                 logging.info(f"generating artifacts for job {job_slug}")
                 for artifact in artifact_generator(
                     remote_id=remote_id, input=remote_result, job_slug=job_slug
                 ):
                     file = service.upload_job_artifact(
@@ -279,15 +280,15 @@
     - Upload job results
     - Update job status to COMPLETED
     - Enter a billing transaction (default: 0)
     """
     logging.info(f"handling job completion for {job_slug}")
     _handle_fetch_result(ctx, remote_api, job_slug, remote_id)
 
-    logging.info(f"setting job status to COMPLETEDe for job {job_slug}")
+    logging.info(f"setting job status to COMPLETED for job {job_slug}")
     try:
         updated_job = (
             service.update_job(
                 ctx,
                 job_slug=job_slug,
                 status=JobStatus.COMPLETED,
                 remote_status=remote_status,
```

### Comparing `remote_job_app-0.1.6/strangeworks_remote_job/ex.py` & `remote_job_app-0.1.7/strangeworks_remote_job/ex.py`

 * *Files identical despite different names*

### Comparing `remote_job_app-0.1.6/strangeworks_remote_job/remote.py` & `remote_job_app-0.1.7/strangeworks_remote_job/remote.py`

 * *Files identical despite different names*

