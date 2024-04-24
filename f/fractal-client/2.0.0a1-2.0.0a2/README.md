# Comparing `tmp/fractal_client-2.0.0a1.tar.gz` & `tmp/fractal_client-2.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_client-2.0.0a1.tar", max compression
+gzip compressed data, was "fractal_client-2.0.0a2.tar", max compression
```

## Comparing `fractal_client-2.0.0a1.tar` & `fractal_client-2.0.0a2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1576 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/LICENSE
--rw-r--r--   0        0        0     2706 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/README.md
--rw-r--r--   0        0        0       24 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/__init__.py
--rw-r--r--   0        0        0     3660 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/authclient.py
--rw-r--r--   0        0        0     4157 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/client.py
--rw-r--r--   0        0        0    11368 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/cmd/__init__.py
--rw-r--r--   0        0        0     7611 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/cmd/_aux_task_caching.py
--rw-r--r--   0        0        0     2456 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/cmd/_dataset.py
--rw-r--r--   0        0        0     4750 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/cmd/_job.py
--rw-r--r--   0        0        0     1758 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/cmd/_project.py
--rw-r--r--   0        0        0     6316 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/cmd/_task.py
--rw-r--r--   0        0        0     4766 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/cmd/_user.py
--rw-r--r--   0        0        0     8501 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/cmd/_workflow.py
--rw-r--r--   0        0        0     1126 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/config.py
--rw-r--r--   0        0        0      363 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/interface.py
--rw-r--r--   0        0        0    22092 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/parser.py
--rw-r--r--   0        0        0     2384 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/fractal_client/response.py
--rw-r--r--   0        0        0     2248 2024-04-17 07:33:42.923673 fractal_client-2.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     3807 1970-01-01 00:00:00.000000 fractal_client-2.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1576 2024-04-24 06:58:33.288842 fractal_client-2.0.0a2/LICENSE
+-rw-r--r--   0        0        0     2706 2024-04-24 06:58:33.288842 fractal_client-2.0.0a2/README.md
+-rw-r--r--   0        0        0       24 2024-04-24 06:58:33.288842 fractal_client-2.0.0a2/fractal_client/__init__.py
+-rw-r--r--   0        0        0     3660 2024-04-24 06:58:33.288842 fractal_client-2.0.0a2/fractal_client/authclient.py
+-rw-r--r--   0        0        0     4157 2024-04-24 06:58:33.288842 fractal_client-2.0.0a2/fractal_client/client.py
+-rw-r--r--   0        0        0    11368 2024-04-24 06:58:33.288842 fractal_client-2.0.0a2/fractal_client/cmd/__init__.py
+-rw-r--r--   0        0        0     7611 2024-04-24 06:58:33.288842 fractal_client-2.0.0a2/fractal_client/cmd/_aux_task_caching.py
+-rw-r--r--   0        0        0     2456 2024-04-24 06:58:33.288842 fractal_client-2.0.0a2/fractal_client/cmd/_dataset.py
+-rw-r--r--   0        0        0     4750 2024-04-24 06:58:33.288842 fractal_client-2.0.0a2/fractal_client/cmd/_job.py
+-rw-r--r--   0        0        0     1758 2024-04-24 06:58:33.288842 fractal_client-2.0.0a2/fractal_client/cmd/_project.py
+-rw-r--r--   0        0        0     6316 2024-04-24 06:58:33.288842 fractal_client-2.0.0a2/fractal_client/cmd/_task.py
+-rw-r--r--   0        0        0     4409 2024-04-24 06:58:33.288842 fractal_client-2.0.0a2/fractal_client/cmd/_user.py
+-rw-r--r--   0        0        0     8451 2024-04-24 06:58:33.288842 fractal_client-2.0.0a2/fractal_client/cmd/_workflow.py
+-rw-r--r--   0        0        0     1126 2024-04-24 06:58:33.288842 fractal_client-2.0.0a2/fractal_client/config.py
+-rw-r--r--   0        0        0      363 2024-04-24 06:58:33.288842 fractal_client-2.0.0a2/fractal_client/interface.py
+-rw-r--r--   0        0        0    22092 2024-04-24 06:58:33.288842 fractal_client-2.0.0a2/fractal_client/parser.py
+-rw-r--r--   0        0        0     2384 2024-04-24 06:58:33.288842 fractal_client-2.0.0a2/fractal_client/response.py
+-rw-r--r--   0        0        0     2248 2024-04-24 06:58:33.288842 fractal_client-2.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0     3807 1970-01-01 00:00:00.000000 fractal_client-2.0.0a2/PKG-INFO
```

### Comparing `fractal_client-2.0.0a1/LICENSE` & `fractal_client-2.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_client-2.0.0a1/README.md` & `fractal_client-2.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `fractal_client-2.0.0a1/fractal_client/authclient.py` & `fractal_client-2.0.0a2/fractal_client/authclient.py`

 * *Files identical despite different names*

### Comparing `fractal_client-2.0.0a1/fractal_client/client.py` & `fractal_client-2.0.0a2/fractal_client/client.py`

 * *Files identical despite different names*

### Comparing `fractal_client-2.0.0a1/fractal_client/cmd/__init__.py` & `fractal_client-2.0.0a2/fractal_client/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_client-2.0.0a1/fractal_client/cmd/_aux_task_caching.py` & `fractal_client-2.0.0a2/fractal_client/cmd/_aux_task_caching.py`

 * *Files identical despite different names*

### Comparing `fractal_client-2.0.0a1/fractal_client/cmd/_dataset.py` & `fractal_client-2.0.0a2/fractal_client/cmd/_dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_client-2.0.0a1/fractal_client/cmd/_job.py` & `fractal_client-2.0.0a2/fractal_client/cmd/_job.py`

 * *Files identical despite different names*

### Comparing `fractal_client-2.0.0a1/fractal_client/cmd/_project.py` & `fractal_client-2.0.0a2/fractal_client/cmd/_project.py`

 * *Files identical despite different names*

### Comparing `fractal_client-2.0.0a1/fractal_client/cmd/_task.py` & `fractal_client-2.0.0a2/fractal_client/cmd/_task.py`

 * *Files identical despite different names*

### Comparing `fractal_client-2.0.0a1/fractal_client/cmd/_user.py` & `fractal_client-2.0.0a2/fractal_client/cmd/_user.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ..response import check_response
 
 
 def user_register(
     client: AuthClient,
     *,
     new_email: str,
-    new_password: Optional[str] = None,
+    new_password: str,
     slurm_user: Optional[str] = None,
     cache_dir: Optional[str] = None,
     username: Optional[str] = None,
     superuser: bool = False,
     verified: bool = True,  # TODO: this is not currently exposed in the CLI
     batch: bool = False,
 ) -> Interface:
@@ -26,24 +26,14 @@
     if slurm_user:
         new_user["slurm_user"] = slurm_user
     if cache_dir:
         new_user["cache_dir"] = cache_dir
     if username:
         new_user["username"] = username
 
-    from getpass import getpass
-
-    if new_password is None:
-        new_password = getpass()
-        confirm_new_password = getpass("Confirm password: ")
-        if new_password == confirm_new_password:
-            new_user["password"] = new_password
-        else:
-            return Interface(retcode=1, data="Passwords do not match.")
-
     res = client.post(
         f"{settings.FRACTAL_SERVER}/auth/register/", json=new_user
     )
     data = check_response(res, expected_status_code=201)
 
     if superuser or verified:
         patch_payload = dict(is_superuser=superuser, is_verified=verified)
```

### Comparing `fractal_client-2.0.0a1/fractal_client/cmd/_workflow.py` & `fractal_client-2.0.0a2/fractal_client/cmd/_workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,18 +243,14 @@
         sources_str = ", ".join([f"'{s}'" for s in warnings])
         logging.warning(
             "This workflow includes custom tasks (the ones with sources: "
             f"{sources_str}), which are not meant to be portable; "
             "importing this workflow may not work as expected."
         )
 
-    from devtools import debug
-
-    debug(batch)
-
     if batch:
         datastr = f"{wf_read['id']}"
         for wftask in wf_read["task_list"]:
             datastr += f" {wftask['id']}"
         return Interface(retcode=0, data=datastr)
     else:
         return Interface(retcode=0, data=wf_read)
```

### Comparing `fractal_client-2.0.0a1/fractal_client/config.py` & `fractal_client-2.0.0a2/fractal_client/config.py`

 * *Files identical despite different names*

### Comparing `fractal_client-2.0.0a1/fractal_client/parser.py` & `fractal_client-2.0.0a2/fractal_client/parser.py`

 * *Files identical despite different names*

### Comparing `fractal_client-2.0.0a1/fractal_client/response.py` & `fractal_client-2.0.0a2/fractal_client/response.py`

 * *Files identical despite different names*

### Comparing `fractal_client-2.0.0a1/pyproject.toml` & `fractal_client-2.0.0a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-client"
-version = "2.0.0a1"
+version = "2.0.0a2"
 description = "Client component of the Fractal analytics platform"
 authors = [
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
 ]
 readme = "README.md"
@@ -52,15 +52,15 @@
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bumpver]
-current_version = "2.0.0a1"
+current_version = "2.0.0a2"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_client-2.0.0a1/PKG-INFO` & `fractal_client-2.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-client
-Version: 2.0.0a1
+Version: 2.0.0a2
 Summary: Client component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-client
 License: BSD-3-Clause
 Author: Tommaso Comparin
 Author-email: tommaso.comparin@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

