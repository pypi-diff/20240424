# Comparing `tmp/pachyderm_sdk-2.9.3.tar.gz` & `tmp/pachyderm_sdk-2.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pachyderm_sdk-2.9.3.tar", max compression
+gzip compressed data, was "pachyderm_sdk-2.9.4.tar", max compression
```

## Comparing `pachyderm_sdk-2.9.3.tar` & `pachyderm_sdk-2.9.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     2913 2024-03-27 18:02:05.963640 pachyderm_sdk-2.9.3/README.md
--rw-r--r--   0        0        0      357 2024-03-27 18:02:05.963640 pachyderm_sdk-2.9.3/pachyderm_sdk/__init__.py
--rw-r--r--   0        0        0      645 2024-03-27 18:02:05.963640 pachyderm_sdk-2.9.3/pachyderm_sdk/__main__.py
--rw-r--r--   0        0        0        8 2024-03-27 18:02:05.963640 pachyderm_sdk-2.9.3/pachyderm_sdk/api/.gitignore
--rw-r--r--   0        0        0       66 2024-03-27 18:02:05.963640 pachyderm_sdk-2.9.3/pachyderm_sdk/api/__init__.py
--rw-r--r--   0        0        0     3172 2024-03-27 18:02:05.963640 pachyderm_sdk-2.9.3/pachyderm_sdk/api/admin/__init__.py
--rw-r--r--   0        0        0     1036 2024-03-27 18:02:05.963640 pachyderm_sdk-2.9.3/pachyderm_sdk/api/admin/extension.py
--rw-r--r--   0        0        0    31384 2024-03-27 18:02:05.963640 pachyderm_sdk-2.9.3/pachyderm_sdk/api/auth/__init__.py
--rw-r--r--   0        0        0    12630 2024-03-27 18:02:05.963640 pachyderm_sdk-2.9.3/pachyderm_sdk/api/debug/__init__.py
--rw-r--r--   0        0        0     1609 2024-03-27 18:02:05.963640 pachyderm_sdk-2.9.3/pachyderm_sdk/api/debug/extension.py
--rw-r--r--   0        0        0     8236 2024-03-27 18:02:05.963640 pachyderm_sdk-2.9.3/pachyderm_sdk/api/enterprise/__init__.py
--rw-r--r--   0        0        0    12315 2024-03-27 18:02:05.963640 pachyderm_sdk-2.9.3/pachyderm_sdk/api/identity/__init__.py
--rw-r--r--   0        0        0    10507 2024-03-27 18:02:05.963640 pachyderm_sdk-2.9.3/pachyderm_sdk/api/license/__init__.py
--rw-r--r--   0        0        0    56747 2024-03-27 18:02:05.963640 pachyderm_sdk-2.9.3/pachyderm_sdk/api/pfs/__init__.py
--rw-r--r--   0        0        0     5447 2024-03-27 18:02:05.963640 pachyderm_sdk-2.9.3/pachyderm_sdk/api/pfs/_additions.py
--rw-r--r--   0        0        0    25802 2024-03-27 18:02:05.963640 pachyderm_sdk-2.9.3/pachyderm_sdk/api/pfs/extension.py
--rw-r--r--   0        0        0     4018 2024-03-27 18:02:05.963640 pachyderm_sdk-2.9.3/pachyderm_sdk/api/pfs/file.py
--rw-r--r--   0        0        0    14258 2024-03-27 18:02:05.963640 pachyderm_sdk-2.9.3/pachyderm_sdk/api/pjs/__init__.py
--rw-r--r--   0        0        0    75665 2024-03-27 18:02:05.963640 pachyderm_sdk-2.9.3/pachyderm_sdk/api/pps/__init__.py
--rw-r--r--   0        0        0      679 2024-03-27 18:02:05.963640 pachyderm_sdk-2.9.3/pachyderm_sdk/api/pps/_additions.py
--rw-r--r--   0        0        0     4175 2024-03-27 18:02:05.963640 pachyderm_sdk-2.9.3/pachyderm_sdk/api/pps/extension.py
--rw-r--r--   0        0        0     1113 2024-03-27 18:02:05.963640 pachyderm_sdk-2.9.3/pachyderm_sdk/api/taskapi/__init__.py
--rw-r--r--   0        0        0     6822 2024-03-27 18:02:05.963640 pachyderm_sdk-2.9.3/pachyderm_sdk/api/transaction/__init__.py
--rw-r--r--   0        0        0     3614 2024-03-27 18:02:05.963640 pachyderm_sdk-2.9.3/pachyderm_sdk/api/transaction/extension.py
--rw-r--r--   0        0        0     1375 2024-03-27 18:02:05.963640 pachyderm_sdk-2.9.3/pachyderm_sdk/api/version/__init__.py
--rw-r--r--   0        0        0     2866 2024-03-27 18:02:05.963640 pachyderm_sdk-2.9.3/pachyderm_sdk/api/worker/__init__.py
--rw-r--r--   0        0        0     1872 2024-03-27 18:02:05.963640 pachyderm_sdk-2.9.3/pachyderm_sdk/api/worker/extension.py
--rw-r--r--   0        0        0    11519 2024-03-27 18:02:05.967640 pachyderm_sdk-2.9.3/pachyderm_sdk/client.py
--rw-r--r--   0        0        0     7114 2024-03-27 18:02:05.967640 pachyderm_sdk-2.9.3/pachyderm_sdk/config.py
--rw-r--r--   0        0        0     1083 2024-03-27 18:02:05.967640 pachyderm_sdk-2.9.3/pachyderm_sdk/constants.py
--rw-r--r--   0        0        0     1570 2024-03-27 18:02:05.967640 pachyderm_sdk-2.9.3/pachyderm_sdk/datum_batching.py
--rw-r--r--   0        0        0     1045 2024-03-27 18:02:05.967640 pachyderm_sdk-2.9.3/pachyderm_sdk/errors.py
--rw-r--r--   0        0        0     3439 2024-03-27 18:02:05.967640 pachyderm_sdk-2.9.3/pachyderm_sdk/interceptor.py
--rw-r--r--   0        0        0     1490 2024-03-27 18:02:42.107679 pachyderm_sdk-2.9.3/pyproject.toml
--rw-r--r--   0        0        0     4289 1970-01-01 00:00:00.000000 pachyderm_sdk-2.9.3/PKG-INFO
+-rw-r--r--   0        0        0     2913 2024-04-10 16:08:43.497161 pachyderm_sdk-2.9.4/README.md
+-rw-r--r--   0        0        0      357 2024-04-10 16:08:43.497161 pachyderm_sdk-2.9.4/pachyderm_sdk/__init__.py
+-rw-r--r--   0        0        0      645 2024-04-10 16:08:43.497161 pachyderm_sdk-2.9.4/pachyderm_sdk/__main__.py
+-rw-r--r--   0        0        0        8 2024-04-10 16:08:43.497161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/.gitignore
+-rw-r--r--   0        0        0       66 2024-04-10 16:08:43.497161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/__init__.py
+-rw-r--r--   0        0        0     3172 2024-04-10 16:08:43.497161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/admin/__init__.py
+-rw-r--r--   0        0        0     1036 2024-04-10 16:08:43.497161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/admin/extension.py
+-rw-r--r--   0        0        0    31384 2024-04-10 16:08:43.497161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/auth/__init__.py
+-rw-r--r--   0        0        0    13046 2024-04-10 16:08:43.497161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/debug/__init__.py
+-rw-r--r--   0        0        0     1609 2024-04-10 16:08:43.497161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/debug/extension.py
+-rw-r--r--   0        0        0     8236 2024-04-10 16:08:43.497161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/enterprise/__init__.py
+-rw-r--r--   0        0        0    12315 2024-04-10 16:08:43.497161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/identity/__init__.py
+-rw-r--r--   0        0        0    10507 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/license/__init__.py
+-rw-r--r--   0        0        0    56747 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/pfs/__init__.py
+-rw-r--r--   0        0        0     5447 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/pfs/_additions.py
+-rw-r--r--   0        0        0    25802 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/pfs/extension.py
+-rw-r--r--   0        0        0     4018 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/pfs/file.py
+-rw-r--r--   0        0        0    14258 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/pjs/__init__.py
+-rw-r--r--   0        0        0    75665 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/pps/__init__.py
+-rw-r--r--   0        0        0      679 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/pps/_additions.py
+-rw-r--r--   0        0        0     4175 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/pps/extension.py
+-rw-r--r--   0        0        0     1113 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/taskapi/__init__.py
+-rw-r--r--   0        0        0     6822 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/transaction/__init__.py
+-rw-r--r--   0        0        0     3614 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/transaction/extension.py
+-rw-r--r--   0        0        0     1375 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/version/__init__.py
+-rw-r--r--   0        0        0     2866 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/worker/__init__.py
+-rw-r--r--   0        0        0     1872 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/api/worker/extension.py
+-rw-r--r--   0        0        0    11519 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/client.py
+-rw-r--r--   0        0        0     7114 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/config.py
+-rw-r--r--   0        0        0     1083 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/constants.py
+-rw-r--r--   0        0        0     1570 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/datum_batching.py
+-rw-r--r--   0        0        0     1045 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/errors.py
+-rw-r--r--   0        0        0     3439 2024-04-10 16:08:43.501161 pachyderm_sdk-2.9.4/pachyderm_sdk/interceptor.py
+-rw-r--r--   0        0        0     1490 2024-04-10 16:09:21.369456 pachyderm_sdk-2.9.4/pyproject.toml
+-rw-r--r--   0        0        0     4289 1970-01-01 00:00:00.000000 pachyderm_sdk-2.9.4/PKG-INFO
```

### Comparing `pachyderm_sdk-2.9.3/README.md` & `pachyderm_sdk-2.9.4/README.md`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.3/pachyderm_sdk/__main__.py` & `pachyderm_sdk-2.9.4/pachyderm_sdk/__main__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.3/pachyderm_sdk/api/admin/__init__.py` & `pachyderm_sdk-2.9.4/pachyderm_sdk/api/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.3/pachyderm_sdk/api/admin/extension.py` & `pachyderm_sdk-2.9.4/pachyderm_sdk/api/admin/extension.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.3/pachyderm_sdk/api/auth/__init__.py` & `pachyderm_sdk-2.9.4/pachyderm_sdk/api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.3/pachyderm_sdk/api/debug/__init__.py` & `pachyderm_sdk-2.9.4/pachyderm_sdk/api/debug/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,26 @@
 
 @dataclass(eq=False, repr=False)
 class App(betterproto.Message):
     name: str = betterproto.string_field(1)
     pods: List["Pod"] = betterproto.message_field(2)
     timeout: timedelta = betterproto.message_field(3)
     pipeline: "Pipeline" = betterproto.message_field(4)
+    loki_args: "LokiArgs" = betterproto.message_field(5, group="extra_args")
+    profile_args: "ProfileArgs" = betterproto.message_field(6, group="extra_args")
+
+
+@dataclass(eq=False, repr=False)
+class ProfileArgs(betterproto.Message):
+    profiles: List["Profile"] = betterproto.message_field(1)
+
+
+@dataclass(eq=False, repr=False)
+class LokiArgs(betterproto.Message):
+    max_logs: int = betterproto.uint64_field(1)
 
 
 @dataclass(eq=False, repr=False)
 class System(betterproto.Message):
     helm: bool = betterproto.bool_field(1)
     database: bool = betterproto.bool_field(2)
     version: bool = betterproto.bool_field(3)
```

### Comparing `pachyderm_sdk-2.9.3/pachyderm_sdk/api/debug/extension.py` & `pachyderm_sdk-2.9.4/pachyderm_sdk/api/debug/extension.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.3/pachyderm_sdk/api/enterprise/__init__.py` & `pachyderm_sdk-2.9.4/pachyderm_sdk/api/enterprise/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.3/pachyderm_sdk/api/identity/__init__.py` & `pachyderm_sdk-2.9.4/pachyderm_sdk/api/identity/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.3/pachyderm_sdk/api/license/__init__.py` & `pachyderm_sdk-2.9.4/pachyderm_sdk/api/license/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.3/pachyderm_sdk/api/pfs/__init__.py` & `pachyderm_sdk-2.9.4/pachyderm_sdk/api/pfs/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.3/pachyderm_sdk/api/pfs/_additions.py` & `pachyderm_sdk-2.9.4/pachyderm_sdk/api/pfs/_additions.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.3/pachyderm_sdk/api/pfs/extension.py` & `pachyderm_sdk-2.9.4/pachyderm_sdk/api/pfs/extension.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.3/pachyderm_sdk/api/pfs/file.py` & `pachyderm_sdk-2.9.4/pachyderm_sdk/api/pfs/file.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.3/pachyderm_sdk/api/pjs/__init__.py` & `pachyderm_sdk-2.9.4/pachyderm_sdk/api/pjs/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.3/pachyderm_sdk/api/pps/__init__.py` & `pachyderm_sdk-2.9.4/pachyderm_sdk/api/pps/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.3/pachyderm_sdk/api/pps/_additions.py` & `pachyderm_sdk-2.9.4/pachyderm_sdk/api/pps/_additions.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.3/pachyderm_sdk/api/pps/extension.py` & `pachyderm_sdk-2.9.4/pachyderm_sdk/api/pps/extension.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.3/pachyderm_sdk/api/taskapi/__init__.py` & `pachyderm_sdk-2.9.4/pachyderm_sdk/api/taskapi/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.3/pachyderm_sdk/api/transaction/__init__.py` & `pachyderm_sdk-2.9.4/pachyderm_sdk/api/transaction/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.3/pachyderm_sdk/api/transaction/extension.py` & `pachyderm_sdk-2.9.4/pachyderm_sdk/api/transaction/extension.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.3/pachyderm_sdk/api/version/__init__.py` & `pachyderm_sdk-2.9.4/pachyderm_sdk/api/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.3/pachyderm_sdk/api/worker/__init__.py` & `pachyderm_sdk-2.9.4/pachyderm_sdk/api/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.3/pachyderm_sdk/api/worker/extension.py` & `pachyderm_sdk-2.9.4/pachyderm_sdk/api/worker/extension.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.3/pachyderm_sdk/client.py` & `pachyderm_sdk-2.9.4/pachyderm_sdk/client.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.3/pachyderm_sdk/config.py` & `pachyderm_sdk-2.9.4/pachyderm_sdk/config.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.3/pachyderm_sdk/constants.py` & `pachyderm_sdk-2.9.4/pachyderm_sdk/constants.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.3/pachyderm_sdk/datum_batching.py` & `pachyderm_sdk-2.9.4/pachyderm_sdk/datum_batching.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.3/pachyderm_sdk/errors.py` & `pachyderm_sdk-2.9.4/pachyderm_sdk/errors.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.3/pachyderm_sdk/interceptor.py` & `pachyderm_sdk-2.9.4/pachyderm_sdk/interceptor.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.3/pyproject.toml` & `pachyderm_sdk-2.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pachyderm_sdk"
-version = "2.9.3"
+version = "2.9.4"
 description = "Python Pachyderm Client"
 authors = ["Pachyderm Integrations <integrations@pachyderm.io>"]
 license = "Apache 2.0"
 documentation = "https://docs.pachyderm.com/latest/sdk/python/"
 readme = 'README.md'
 repository = "https://github.com/pachyderm/pachyderm/tree/master/python-sdk"
 keywords = ["pachyderm"]
```

### Comparing `pachyderm_sdk-2.9.3/PKG-INFO` & `pachyderm_sdk-2.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pachyderm-sdk
-Version: 2.9.3
+Version: 2.9.4
 Summary: Python Pachyderm Client
 Home-page: https://github.com/pachyderm/pachyderm/tree/master/python-sdk
 License: Apache 2.0
 Keywords: pachyderm
 Author: Pachyderm Integrations
 Author-email: integrations@pachyderm.io
 Requires-Python: >=3.8,<4.0
```

