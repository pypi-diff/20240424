# Comparing `tmp/mypy_boto3_entityresolution-1.34.85.tar.gz` & `tmp/mypy_boto3_entityresolution-1.34.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_entityresolution-1.34.85.tar", last modified: Tue Apr 16 19:33:15 2024, max compression
+gzip compressed data, was "mypy_boto3_entityresolution-1.34.91.tar", last modified: Wed Apr 24 19:19:06 2024, max compression
```

## Comparing `mypy_boto3_entityresolution-1.34.85.tar` & `mypy_boto3_entityresolution-1.34.91.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:15.084309 mypy_boto3_entityresolution-1.34.85/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-16 19:32:50.000000 mypy_boto3_entityresolution-1.34.85/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14175 2024-04-16 19:33:15.084309 mypy_boto3_entityresolution-1.34.85/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12584 2024-04-16 19:32:50.000000 mypy_boto3_entityresolution-1.34.85/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:15.084309 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-16 19:32:50.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-16 19:32:50.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-16 19:32:50.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30395 2024-04-16 19:32:50.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    30392 2024-04-16 19:32:50.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10406 2024-04-16 19:32:50.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10406 2024-04-16 19:32:50.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-04-16 19:32:50.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-04-16 19:32:50.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 19:32:50.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    34558 2024-04-16 19:32:51.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    34558 2024-04-16 19:32:51.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 19:32:50.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:33:15.084309 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14175 2024-04-16 19:33:15.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-16 19:33:15.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:33:15.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:33:15.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-16 19:33:15.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-16 19:33:15.000000 mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 19:33:15.084309 mypy_boto3_entityresolution-1.34.85/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-16 19:32:50.000000 mypy_boto3_entityresolution-1.34.85/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:06.275889 mypy_boto3_entityresolution-1.34.91/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-24 19:18:38.000000 mypy_boto3_entityresolution-1.34.91/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14175 2024-04-24 19:19:06.275889 mypy_boto3_entityresolution-1.34.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12584 2024-04-24 19:18:38.000000 mypy_boto3_entityresolution-1.34.91/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:06.271890 mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution/
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-24 19:18:38.000000 mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-24 19:18:38.000000 mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-24 19:18:38.000000 mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31003 2024-04-24 19:18:38.000000 mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31000 2024-04-24 19:18:38.000000 mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10631 2024-04-24 19:18:38.000000 mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10631 2024-04-24 19:18:38.000000 mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-04-24 19:18:38.000000 mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-04-24 19:18:38.000000 mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:18:38.000000 mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    35603 2024-04-24 19:18:40.000000 mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35603 2024-04-24 19:18:39.000000 mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-24 19:18:38.000000 mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:06.275889 mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14175 2024-04-24 19:19:06.000000 mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-24 19:19:06.000000 mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:19:06.000000 mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:19:06.000000 mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-24 19:19:06.000000 mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-24 19:19:06.000000 mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:19:06.275889 mypy_boto3_entityresolution-1.34.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-24 19:18:38.000000 mypy_boto3_entityresolution-1.34.91/setup.py
```

### Comparing `mypy_boto3_entityresolution-1.34.85/LICENSE` & `mypy_boto3_entityresolution-1.34.91/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_entityresolution-1.34.85/PKG-INFO` & `mypy_boto3_entityresolution-1.34.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-entityresolution
-Version: 1.34.85
-Summary: Type annotations for boto3.EntityResolution 1.34.85 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.91
+Summary: Type annotations for boto3.EntityResolution 1.34.91 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-entityresolution.svg?color=blue)](https://pypi.org/project/mypy-boto3-entityresolution)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-entityresolution)](https://pepy.tech/project/mypy-boto3-entityresolution)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EntityResolution 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
+[boto3.EntityResolution 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_entityresolution-1.34.85/README.md` & `mypy_boto3_entityresolution-1.34.91/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-entityresolution.svg?color=blue)](https://pypi.org/project/mypy-boto3-entityresolution)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-entityresolution)](https://pepy.tech/project/mypy-boto3-entityresolution)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EntityResolution 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
+[boto3.EntityResolution 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/__init__.py` & `mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/__init__.pyi` & `mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/__main__.py` & `mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EntityResolution 1.34.85\n"
-        "Version:         1.34.85\n"
+        "Type annotations for boto3.EntityResolution 1.34.91\n"
+        "Version:         1.34.91\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.85")
+    print("1.34.91")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/client.py` & `mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     ListMatchingJobsPaginator,
     ListMatchingWorkflowsPaginator,
     ListProviderServicesPaginator,
     ListSchemaMappingsPaginator,
 )
 from .type_defs import (
     AddPolicyStatementOutputTypeDef,
+    BatchDeleteUniqueIdOutputTypeDef,
     CreateIdMappingWorkflowOutputTypeDef,
     CreateIdNamespaceOutputTypeDef,
     CreateMatchingWorkflowOutputTypeDef,
     CreateSchemaMappingOutputTypeDef,
     DeleteIdMappingWorkflowOutputTypeDef,
     DeleteIdNamespaceOutputTypeDef,
     DeleteMatchingWorkflowOutputTypeDef,
@@ -134,14 +135,24 @@
         """
         Adds a policy statement object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.add_policy_statement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#add_policy_statement)
         """
 
+    def batch_delete_unique_id(
+        self, *, uniqueIds: Sequence[str], workflowName: str, inputSource: str = ...
+    ) -> BatchDeleteUniqueIdOutputTypeDef:
+        """
+        Deletes multiple unique IDs in a matching workflow.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.batch_delete_unique_id)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#batch_delete_unique_id)
+        """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#can_paginate)
         """
```

### Comparing `mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/client.pyi` & `mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     ListMatchingJobsPaginator,
     ListMatchingWorkflowsPaginator,
     ListProviderServicesPaginator,
     ListSchemaMappingsPaginator,
 )
 from .type_defs import (
     AddPolicyStatementOutputTypeDef,
+    BatchDeleteUniqueIdOutputTypeDef,
     CreateIdMappingWorkflowOutputTypeDef,
     CreateIdNamespaceOutputTypeDef,
     CreateMatchingWorkflowOutputTypeDef,
     CreateSchemaMappingOutputTypeDef,
     DeleteIdMappingWorkflowOutputTypeDef,
     DeleteIdNamespaceOutputTypeDef,
     DeleteMatchingWorkflowOutputTypeDef,
@@ -131,14 +132,24 @@
         """
         Adds a policy statement object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.add_policy_statement)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#add_policy_statement)
         """
 
+    def batch_delete_unique_id(
+        self, *, uniqueIds: Sequence[str], workflowName: str, inputSource: str = ...
+    ) -> BatchDeleteUniqueIdOutputTypeDef:
+        """
+        Deletes multiple unique IDs in a matching workflow.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.batch_delete_unique_id)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#batch_delete_unique_id)
+        """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/client/#can_paginate)
         """
```

### Comparing `mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/literals.py` & `mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AttributeMatchingModelType",
+    "DeleteUniqueIdErrorTypeType",
+    "DeleteUniqueIdStatusType",
     "IdMappingTypeType",
     "IdNamespaceTypeType",
     "IncrementalRunTypeType",
     "JobStatusType",
     "ListIdMappingJobsPaginatorName",
     "ListIdMappingWorkflowsPaginatorName",
     "ListIdNamespacesPaginatorName",
@@ -39,14 +41,16 @@
     "EntityResolutionServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
 AttributeMatchingModelType = Literal["MANY_TO_MANY", "ONE_TO_ONE"]
+DeleteUniqueIdErrorTypeType = Literal["SERVICE_ERROR", "VALIDATION_ERROR"]
+DeleteUniqueIdStatusType = Literal["ACCEPTED", "COMPLETED"]
 IdMappingTypeType = Literal["PROVIDER"]
 IdNamespaceTypeType = Literal["SOURCE", "TARGET"]
 IncrementalRunTypeType = Literal["IMMEDIATE"]
 JobStatusType = Literal["FAILED", "QUEUED", "RUNNING", "SUCCEEDED"]
 ListIdMappingJobsPaginatorName = Literal["list_id_mapping_jobs"]
 ListIdMappingWorkflowsPaginatorName = Literal["list_id_mapping_workflows"]
 ListIdNamespacesPaginatorName = Literal["list_id_namespaces"]
@@ -384,14 +388,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/literals.pyi` & `mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AttributeMatchingModelType",
+    "DeleteUniqueIdErrorTypeType",
+    "DeleteUniqueIdStatusType",
     "IdMappingTypeType",
     "IdNamespaceTypeType",
     "IncrementalRunTypeType",
     "JobStatusType",
     "ListIdMappingJobsPaginatorName",
     "ListIdMappingWorkflowsPaginatorName",
     "ListIdNamespacesPaginatorName",
@@ -39,14 +41,16 @@
     "EntityResolutionServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
 AttributeMatchingModelType = Literal["MANY_TO_MANY", "ONE_TO_ONE"]
+DeleteUniqueIdErrorTypeType = Literal["SERVICE_ERROR", "VALIDATION_ERROR"]
+DeleteUniqueIdStatusType = Literal["ACCEPTED", "COMPLETED"]
 IdMappingTypeType = Literal["PROVIDER"]
 IdNamespaceTypeType = Literal["SOURCE", "TARGET"]
 IncrementalRunTypeType = Literal["IMMEDIATE"]
 JobStatusType = Literal["FAILED", "QUEUED", "RUNNING", "SUCCEEDED"]
 ListIdMappingJobsPaginatorName = Literal["list_id_mapping_jobs"]
 ListIdMappingWorkflowsPaginatorName = Literal["list_id_mapping_workflows"]
 ListIdNamespacesPaginatorName = Literal["list_id_namespaces"]
@@ -384,14 +388,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/paginator.py` & `mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/paginator.pyi` & `mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/type_defs.py` & `mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     AttributeMatchingModelType,
+    DeleteUniqueIdErrorTypeType,
+    DeleteUniqueIdStatusType,
     IdNamespaceTypeType,
     JobStatusType,
     ResolutionTypeType,
     SchemaAttributeTypeType,
     ServiceTypeType,
     StatementEffectType,
 )
@@ -38,14 +40,17 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddPolicyStatementInputRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "BatchDeleteUniqueIdInputRequestTypeDef",
+    "DeleteUniqueIdErrorTypeDef",
+    "DeletedUniqueIdTypeDef",
     "IdMappingWorkflowInputSourceTypeDef",
     "IdMappingWorkflowOutputSourceTypeDef",
     "IdNamespaceInputSourceTypeDef",
     "IncrementalRunConfigTypeDef",
     "InputSourceTypeDef",
     "SchemaInputAttributeTypeDef",
     "DeleteIdMappingWorkflowInputRequestTypeDef",
@@ -101,14 +106,15 @@
     "DeletePolicyStatementOutputTypeDef",
     "DeleteSchemaMappingOutputTypeDef",
     "GetMatchIdOutputTypeDef",
     "GetPolicyOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "PutPolicyOutputTypeDef",
     "StartMatchingJobOutputTypeDef",
+    "BatchDeleteUniqueIdOutputTypeDef",
     "CreateSchemaMappingInputRequestTypeDef",
     "CreateSchemaMappingOutputTypeDef",
     "GetSchemaMappingOutputTypeDef",
     "UpdateSchemaMappingInputRequestTypeDef",
     "UpdateSchemaMappingOutputTypeDef",
     "GetIdMappingJobOutputTypeDef",
     "StartIdMappingJobInputRequestTypeDef",
@@ -171,14 +177,35 @@
         "RequestId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
         "HostId": NotRequired[str],
     },
 )
+BatchDeleteUniqueIdInputRequestTypeDef = TypedDict(
+    "BatchDeleteUniqueIdInputRequestTypeDef",
+    {
+        "uniqueIds": Sequence[str],
+        "workflowName": str,
+        "inputSource": NotRequired[str],
+    },
+)
+DeleteUniqueIdErrorTypeDef = TypedDict(
+    "DeleteUniqueIdErrorTypeDef",
+    {
+        "errorType": DeleteUniqueIdErrorTypeType,
+        "uniqueId": str,
+    },
+)
+DeletedUniqueIdTypeDef = TypedDict(
+    "DeletedUniqueIdTypeDef",
+    {
+        "uniqueId": str,
+    },
+)
 IdMappingWorkflowInputSourceTypeDef = TypedDict(
     "IdMappingWorkflowInputSourceTypeDef",
     {
         "inputSourceARN": str,
         "schemaName": NotRequired[str],
         "type": NotRequired[IdNamespaceTypeType],
     },
@@ -645,14 +672,24 @@
 StartMatchingJobOutputTypeDef = TypedDict(
     "StartMatchingJobOutputTypeDef",
     {
         "jobId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+BatchDeleteUniqueIdOutputTypeDef = TypedDict(
+    "BatchDeleteUniqueIdOutputTypeDef",
+    {
+        "deleted": List[DeletedUniqueIdTypeDef],
+        "disconnectedUniqueIds": List[str],
+        "errors": List[DeleteUniqueIdErrorTypeDef],
+        "status": DeleteUniqueIdStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 CreateSchemaMappingInputRequestTypeDef = TypedDict(
     "CreateSchemaMappingInputRequestTypeDef",
     {
         "mappedInputFields": Sequence[SchemaInputAttributeTypeDef],
         "schemaName": str,
         "description": NotRequired[str],
         "tags": NotRequired[Mapping[str, str]],
```

### Comparing `mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution/type_defs.pyi` & `mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     AttributeMatchingModelType,
+    DeleteUniqueIdErrorTypeType,
+    DeleteUniqueIdStatusType,
     IdNamespaceTypeType,
     JobStatusType,
     ResolutionTypeType,
     SchemaAttributeTypeType,
     ServiceTypeType,
     StatementEffectType,
 )
@@ -38,14 +40,17 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddPolicyStatementInputRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "BatchDeleteUniqueIdInputRequestTypeDef",
+    "DeleteUniqueIdErrorTypeDef",
+    "DeletedUniqueIdTypeDef",
     "IdMappingWorkflowInputSourceTypeDef",
     "IdMappingWorkflowOutputSourceTypeDef",
     "IdNamespaceInputSourceTypeDef",
     "IncrementalRunConfigTypeDef",
     "InputSourceTypeDef",
     "SchemaInputAttributeTypeDef",
     "DeleteIdMappingWorkflowInputRequestTypeDef",
@@ -101,14 +106,15 @@
     "DeletePolicyStatementOutputTypeDef",
     "DeleteSchemaMappingOutputTypeDef",
     "GetMatchIdOutputTypeDef",
     "GetPolicyOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "PutPolicyOutputTypeDef",
     "StartMatchingJobOutputTypeDef",
+    "BatchDeleteUniqueIdOutputTypeDef",
     "CreateSchemaMappingInputRequestTypeDef",
     "CreateSchemaMappingOutputTypeDef",
     "GetSchemaMappingOutputTypeDef",
     "UpdateSchemaMappingInputRequestTypeDef",
     "UpdateSchemaMappingOutputTypeDef",
     "GetIdMappingJobOutputTypeDef",
     "StartIdMappingJobInputRequestTypeDef",
@@ -171,14 +177,35 @@
         "RequestId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
         "HostId": NotRequired[str],
     },
 )
+BatchDeleteUniqueIdInputRequestTypeDef = TypedDict(
+    "BatchDeleteUniqueIdInputRequestTypeDef",
+    {
+        "uniqueIds": Sequence[str],
+        "workflowName": str,
+        "inputSource": NotRequired[str],
+    },
+)
+DeleteUniqueIdErrorTypeDef = TypedDict(
+    "DeleteUniqueIdErrorTypeDef",
+    {
+        "errorType": DeleteUniqueIdErrorTypeType,
+        "uniqueId": str,
+    },
+)
+DeletedUniqueIdTypeDef = TypedDict(
+    "DeletedUniqueIdTypeDef",
+    {
+        "uniqueId": str,
+    },
+)
 IdMappingWorkflowInputSourceTypeDef = TypedDict(
     "IdMappingWorkflowInputSourceTypeDef",
     {
         "inputSourceARN": str,
         "schemaName": NotRequired[str],
         "type": NotRequired[IdNamespaceTypeType],
     },
@@ -645,14 +672,24 @@
 StartMatchingJobOutputTypeDef = TypedDict(
     "StartMatchingJobOutputTypeDef",
     {
         "jobId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+BatchDeleteUniqueIdOutputTypeDef = TypedDict(
+    "BatchDeleteUniqueIdOutputTypeDef",
+    {
+        "deleted": List[DeletedUniqueIdTypeDef],
+        "disconnectedUniqueIds": List[str],
+        "errors": List[DeleteUniqueIdErrorTypeDef],
+        "status": DeleteUniqueIdStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 CreateSchemaMappingInputRequestTypeDef = TypedDict(
     "CreateSchemaMappingInputRequestTypeDef",
     {
         "mappedInputFields": Sequence[SchemaInputAttributeTypeDef],
         "schemaName": str,
         "description": NotRequired[str],
         "tags": NotRequired[Mapping[str, str]],
```

### Comparing `mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution.egg-info/PKG-INFO` & `mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-entityresolution
-Version: 1.34.85
-Summary: Type annotations for boto3.EntityResolution 1.34.85 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.91
+Summary: Type annotations for boto3.EntityResolution 1.34.91 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-entityresolution.svg?color=blue)](https://pypi.org/project/mypy-boto3-entityresolution)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_entityresolution/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-entityresolution)](https://pepy.tech/project/mypy-boto3-entityresolution)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EntityResolution 1.34.85](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
+[boto3.EntityResolution 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_entityresolution-1.34.85/mypy_boto3_entityresolution.egg-info/SOURCES.txt` & `mypy_boto3_entityresolution-1.34.91/mypy_boto3_entityresolution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_entityresolution-1.34.85/setup.py` & `mypy_boto3_entityresolution-1.34.91/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-entityresolution",
-    version="1.34.85",
+    version="1.34.91",
     packages=["mypy_boto3_entityresolution"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.EntityResolution 1.34.85 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.EntityResolution 1.34.91 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

