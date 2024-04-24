# Comparing `tmp/mypy-boto3-emr-containers-1.34.78.tar.gz` & `tmp/mypy_boto3_emr_containers-1.34.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-emr-containers-1.34.78.tar", last modified: Thu Apr  4 19:33:17 2024, max compression
+gzip compressed data, was "mypy_boto3_emr_containers-1.34.91.tar", last modified: Wed Apr 24 19:19:05 2024, max compression
```

## Comparing `mypy-boto3-emr-containers-1.34.78.tar` & `mypy_boto3_emr_containers-1.34.91.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:17.444019 mypy-boto3-emr-containers-1.34.78/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13551 2024-04-04 19:33:17.444019 mypy-boto3-emr-containers-1.34.78/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:17.444019 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18444 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    18441 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    28264 2024-04-04 19:33:02.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    28264 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:17.444019 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13551 2024-04-04 19:33:17.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-04 19:33:17.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:33:17.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:33:17.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-04 19:33:17.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-04 19:33:17.000000 mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 19:33:17.444019 mypy-boto3-emr-containers-1.34.78/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-04 19:33:01.000000 mypy-boto3-emr-containers-1.34.78/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:05.931894 mypy_boto3_emr_containers-1.34.91/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-24 19:18:37.000000 mypy_boto3_emr_containers-1.34.91/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13733 2024-04-24 19:19:05.927894 mypy_boto3_emr_containers-1.34.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12151 2024-04-24 19:18:37.000000 mypy_boto3_emr_containers-1.34.91/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:05.927894 mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-24 19:18:37.000000 mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-24 19:18:37.000000 mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-24 19:18:37.000000 mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21112 2024-04-24 19:18:37.000000 mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21109 2024-04-24 19:18:37.000000 mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10382 2024-04-24 19:18:37.000000 mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10382 2024-04-24 19:18:37.000000 mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-04-24 19:18:37.000000 mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-04-24 19:18:37.000000 mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:18:37.000000 mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    32958 2024-04-24 19:18:38.000000 mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32958 2024-04-24 19:18:38.000000 mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-24 19:18:37.000000 mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:05.927894 mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13733 2024-04-24 19:19:05.000000 mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-24 19:19:05.000000 mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:19:05.000000 mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:19:05.000000 mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-24 19:19:05.000000 mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-24 19:19:05.000000 mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:19:05.931894 mypy_boto3_emr_containers-1.34.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-24 19:18:37.000000 mypy_boto3_emr_containers-1.34.91/setup.py
```

### Comparing `mypy-boto3-emr-containers-1.34.78/LICENSE` & `mypy_boto3_emr_containers-1.34.91/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.34.78/PKG-INFO` & `mypy_boto3_emr_containers-1.34.91/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-containers
-Version: 1.34.78
-Summary: Type annotations for boto3.EMRContainers 1.34.78 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.91
+Summary: Type annotations for boto3.EMRContainers 1.34.91 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-containers.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-containers)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-containers)](https://pepy.tech/project/mypy-boto3-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRContainers 1.34.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[boto3.EMRContainers 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -285,26 +285,30 @@
 from boto3.session import Session
 
 from mypy_boto3_emr_containers import EMRContainersClient
 from mypy_boto3_emr_containers.paginator import (
     ListJobRunsPaginator,
     ListJobTemplatesPaginator,
     ListManagedEndpointsPaginator,
+    ListSecurityConfigurationsPaginator,
     ListVirtualClustersPaginator,
 )
 
 client: EMRContainersClient = Session().client("emr-containers")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_job_runs_paginator: ListJobRunsPaginator = client.get_paginator("list_job_runs")
 list_job_templates_paginator: ListJobTemplatesPaginator = client.get_paginator("list_job_templates")
 list_managed_endpoints_paginator: ListManagedEndpointsPaginator = client.get_paginator(
     "list_managed_endpoints"
 )
+list_security_configurations_paginator: ListSecurityConfigurationsPaginator = client.get_paginator(
+    "list_security_configurations"
+)
 list_virtual_clusters_paginator: ListVirtualClustersPaginator = client.get_paginator(
     "list_virtual_clusters"
 )
 ```
 
 <a id="literals"></a>
 
@@ -313,18 +317,18 @@
 `mypy_boto3_emr_containers.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 Full list of `EMRContainers` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/literals/).
 
 ```python
-from mypy_boto3_emr_containers.literals import ContainerProviderTypeType
+from mypy_boto3_emr_containers.literals import CertificateProviderTypeType
 
 
-def check_value(value: ContainerProviderTypeType) -> bool: ...
+def check_value(value: CertificateProviderTypeType) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_emr_containers.type_defs` module contains structures and shapes
```

### Comparing `mypy-boto3-emr-containers-1.34.78/README.md` & `mypy_boto3_emr_containers-1.34.91/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-containers.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-containers)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-containers)](https://pepy.tech/project/mypy-boto3-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRContainers 1.34.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[boto3.EMRContainers 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -252,26 +252,30 @@
 from boto3.session import Session
 
 from mypy_boto3_emr_containers import EMRContainersClient
 from mypy_boto3_emr_containers.paginator import (
     ListJobRunsPaginator,
     ListJobTemplatesPaginator,
     ListManagedEndpointsPaginator,
+    ListSecurityConfigurationsPaginator,
     ListVirtualClustersPaginator,
 )
 
 client: EMRContainersClient = Session().client("emr-containers")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_job_runs_paginator: ListJobRunsPaginator = client.get_paginator("list_job_runs")
 list_job_templates_paginator: ListJobTemplatesPaginator = client.get_paginator("list_job_templates")
 list_managed_endpoints_paginator: ListManagedEndpointsPaginator = client.get_paginator(
     "list_managed_endpoints"
 )
+list_security_configurations_paginator: ListSecurityConfigurationsPaginator = client.get_paginator(
+    "list_security_configurations"
+)
 list_virtual_clusters_paginator: ListVirtualClustersPaginator = client.get_paginator(
     "list_virtual_clusters"
 )
 ```
 
 <a id="literals"></a>
 
@@ -280,18 +284,18 @@
 `mypy_boto3_emr_containers.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 Full list of `EMRContainers` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/literals/).
 
 ```python
-from mypy_boto3_emr_containers.literals import ContainerProviderTypeType
+from mypy_boto3_emr_containers.literals import CertificateProviderTypeType
 
 
-def check_value(value: ContainerProviderTypeType) -> bool: ...
+def check_value(value: CertificateProviderTypeType) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_emr_containers.type_defs` module contains structures and shapes
```

### Comparing `mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/__init__.py` & `mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,38 +7,42 @@
     from boto3.session import Session
     from mypy_boto3_emr_containers import (
         Client,
         EMRContainersClient,
         ListJobRunsPaginator,
         ListJobTemplatesPaginator,
         ListManagedEndpointsPaginator,
+        ListSecurityConfigurationsPaginator,
         ListVirtualClustersPaginator,
     )
 
     session = Session()
     client: EMRContainersClient = session.client("emr-containers")
 
     list_job_runs_paginator: ListJobRunsPaginator = client.get_paginator("list_job_runs")
     list_job_templates_paginator: ListJobTemplatesPaginator = client.get_paginator("list_job_templates")
     list_managed_endpoints_paginator: ListManagedEndpointsPaginator = client.get_paginator("list_managed_endpoints")
+    list_security_configurations_paginator: ListSecurityConfigurationsPaginator = client.get_paginator("list_security_configurations")
     list_virtual_clusters_paginator: ListVirtualClustersPaginator = client.get_paginator("list_virtual_clusters")
     ```
 """
 
 from .client import EMRContainersClient
 from .paginator import (
     ListJobRunsPaginator,
     ListJobTemplatesPaginator,
     ListManagedEndpointsPaginator,
+    ListSecurityConfigurationsPaginator,
     ListVirtualClustersPaginator,
 )
 
 Client = EMRContainersClient
 
 __all__ = (
     "Client",
     "EMRContainersClient",
     "ListJobRunsPaginator",
     "ListJobTemplatesPaginator",
     "ListManagedEndpointsPaginator",
+    "ListSecurityConfigurationsPaginator",
     "ListVirtualClustersPaginator",
 )
```

### Comparing `mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/__init__.pyi` & `mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers/__init__.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -7,38 +7,42 @@
     from boto3.session import Session
     from mypy_boto3_emr_containers import (
         Client,
         EMRContainersClient,
         ListJobRunsPaginator,
         ListJobTemplatesPaginator,
         ListManagedEndpointsPaginator,
+        ListSecurityConfigurationsPaginator,
         ListVirtualClustersPaginator,
     )
 
     session = Session()
     client: EMRContainersClient = session.client("emr-containers")
 
     list_job_runs_paginator: ListJobRunsPaginator = client.get_paginator("list_job_runs")
     list_job_templates_paginator: ListJobTemplatesPaginator = client.get_paginator("list_job_templates")
     list_managed_endpoints_paginator: ListManagedEndpointsPaginator = client.get_paginator("list_managed_endpoints")
+    list_security_configurations_paginator: ListSecurityConfigurationsPaginator = client.get_paginator("list_security_configurations")
     list_virtual_clusters_paginator: ListVirtualClustersPaginator = client.get_paginator("list_virtual_clusters")
     ```
 """
 
 from .client import EMRContainersClient
 from .paginator import (
     ListJobRunsPaginator,
     ListJobTemplatesPaginator,
     ListManagedEndpointsPaginator,
+    ListSecurityConfigurationsPaginator,
     ListVirtualClustersPaginator,
 )
 
 Client = EMRContainersClient
 
 __all__ = (
     "Client",
     "EMRContainersClient",
     "ListJobRunsPaginator",
     "ListJobTemplatesPaginator",
     "ListManagedEndpointsPaginator",
+    "ListSecurityConfigurationsPaginator",
     "ListVirtualClustersPaginator",
 )
```

### Comparing `mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/__main__.py` & `mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EMRContainers 1.34.78\n"
-        "Version:         1.34.78\n"
+        "Type annotations for boto3.EMRContainers 1.34.91\n"
+        "Version:         1.34.91\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.78")
+    print("1.34.91")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/client.py` & `mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,39 +20,44 @@
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import EndpointStateType, JobRunStateType, VirtualClusterStateType
 from .paginator import (
     ListJobRunsPaginator,
     ListJobTemplatesPaginator,
     ListManagedEndpointsPaginator,
+    ListSecurityConfigurationsPaginator,
     ListVirtualClustersPaginator,
 )
 from .type_defs import (
     CancelJobRunResponseTypeDef,
     ConfigurationOverridesTypeDef,
     ContainerProviderTypeDef,
     CreateJobTemplateResponseTypeDef,
     CreateManagedEndpointResponseTypeDef,
+    CreateSecurityConfigurationResponseTypeDef,
     CreateVirtualClusterResponseTypeDef,
     DeleteJobTemplateResponseTypeDef,
     DeleteManagedEndpointResponseTypeDef,
     DeleteVirtualClusterResponseTypeDef,
     DescribeJobRunResponseTypeDef,
     DescribeJobTemplateResponseTypeDef,
     DescribeManagedEndpointResponseTypeDef,
+    DescribeSecurityConfigurationResponseTypeDef,
     DescribeVirtualClusterResponseTypeDef,
     GetManagedEndpointSessionCredentialsResponseTypeDef,
     JobDriverTypeDef,
     JobTemplateDataTypeDef,
     ListJobRunsResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     ListManagedEndpointsResponseTypeDef,
+    ListSecurityConfigurationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVirtualClustersResponseTypeDef,
     RetryPolicyConfigurationTypeDef,
+    SecurityConfigurationDataTypeDef,
     StartJobRunResponseTypeDef,
     TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
@@ -151,21 +156,37 @@
         """
         Creates a managed endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.create_managed_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#create_managed_endpoint)
         """
 
+    def create_security_configuration(
+        self,
+        *,
+        clientToken: str,
+        name: str,
+        securityConfigurationData: SecurityConfigurationDataTypeDef,
+        tags: Mapping[str, str] = ...,
+    ) -> CreateSecurityConfigurationResponseTypeDef:
+        """
+        Creates a security configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.create_security_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#create_security_configuration)
+        """
+
     def create_virtual_cluster(
         self,
         *,
         name: str,
         containerProvider: ContainerProviderTypeDef,
         clientToken: str,
         tags: Mapping[str, str] = ...,
+        securityConfigurationId: str = ...,
     ) -> CreateVirtualClusterResponseTypeDef:
         """
         Creates a virtual cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.create_virtual_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#create_virtual_cluster)
         """
@@ -218,14 +239,24 @@
         """
         Displays detailed information about a managed endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.describe_managed_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#describe_managed_endpoint)
         """
 
+    def describe_security_configuration(
+        self, *, id: str
+    ) -> DescribeSecurityConfigurationResponseTypeDef:
+        """
+        Displays detailed information about a specified security configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.describe_security_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#describe_security_configuration)
+        """
+
     def describe_virtual_cluster(self, *, id: str) -> DescribeVirtualClusterResponseTypeDef:
         """
         Displays detailed information about a specified virtual cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.describe_virtual_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#describe_virtual_cluster)
         """
@@ -309,14 +340,29 @@
         """
         Lists managed endpoints based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_managed_endpoints)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#list_managed_endpoints)
         """
 
+    def list_security_configurations(
+        self,
+        *,
+        createdAfter: TimestampTypeDef = ...,
+        createdBefore: TimestampTypeDef = ...,
+        maxResults: int = ...,
+        nextToken: str = ...,
+    ) -> ListSecurityConfigurationsResponseTypeDef:
+        """
+        Lists security configurations based on a set of parameters.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_security_configurations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#list_security_configurations)
+        """
+
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags assigned to the resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#list_tags_for_resource)
         """
@@ -401,13 +447,22 @@
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_security_configurations"]
+    ) -> ListSecurityConfigurationsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_virtual_clusters"]
     ) -> ListVirtualClustersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/client.pyi` & `mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers/client.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -20,39 +20,44 @@
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import EndpointStateType, JobRunStateType, VirtualClusterStateType
 from .paginator import (
     ListJobRunsPaginator,
     ListJobTemplatesPaginator,
     ListManagedEndpointsPaginator,
+    ListSecurityConfigurationsPaginator,
     ListVirtualClustersPaginator,
 )
 from .type_defs import (
     CancelJobRunResponseTypeDef,
     ConfigurationOverridesTypeDef,
     ContainerProviderTypeDef,
     CreateJobTemplateResponseTypeDef,
     CreateManagedEndpointResponseTypeDef,
+    CreateSecurityConfigurationResponseTypeDef,
     CreateVirtualClusterResponseTypeDef,
     DeleteJobTemplateResponseTypeDef,
     DeleteManagedEndpointResponseTypeDef,
     DeleteVirtualClusterResponseTypeDef,
     DescribeJobRunResponseTypeDef,
     DescribeJobTemplateResponseTypeDef,
     DescribeManagedEndpointResponseTypeDef,
+    DescribeSecurityConfigurationResponseTypeDef,
     DescribeVirtualClusterResponseTypeDef,
     GetManagedEndpointSessionCredentialsResponseTypeDef,
     JobDriverTypeDef,
     JobTemplateDataTypeDef,
     ListJobRunsResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     ListManagedEndpointsResponseTypeDef,
+    ListSecurityConfigurationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVirtualClustersResponseTypeDef,
     RetryPolicyConfigurationTypeDef,
+    SecurityConfigurationDataTypeDef,
     StartJobRunResponseTypeDef,
     TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
@@ -148,21 +153,37 @@
         """
         Creates a managed endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.create_managed_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#create_managed_endpoint)
         """
 
+    def create_security_configuration(
+        self,
+        *,
+        clientToken: str,
+        name: str,
+        securityConfigurationData: SecurityConfigurationDataTypeDef,
+        tags: Mapping[str, str] = ...,
+    ) -> CreateSecurityConfigurationResponseTypeDef:
+        """
+        Creates a security configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.create_security_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#create_security_configuration)
+        """
+
     def create_virtual_cluster(
         self,
         *,
         name: str,
         containerProvider: ContainerProviderTypeDef,
         clientToken: str,
         tags: Mapping[str, str] = ...,
+        securityConfigurationId: str = ...,
     ) -> CreateVirtualClusterResponseTypeDef:
         """
         Creates a virtual cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.create_virtual_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#create_virtual_cluster)
         """
@@ -215,14 +236,24 @@
         """
         Displays detailed information about a managed endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.describe_managed_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#describe_managed_endpoint)
         """
 
+    def describe_security_configuration(
+        self, *, id: str
+    ) -> DescribeSecurityConfigurationResponseTypeDef:
+        """
+        Displays detailed information about a specified security configuration.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.describe_security_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#describe_security_configuration)
+        """
+
     def describe_virtual_cluster(self, *, id: str) -> DescribeVirtualClusterResponseTypeDef:
         """
         Displays detailed information about a specified virtual cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.describe_virtual_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#describe_virtual_cluster)
         """
@@ -306,14 +337,29 @@
         """
         Lists managed endpoints based on a set of parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_managed_endpoints)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#list_managed_endpoints)
         """
 
+    def list_security_configurations(
+        self,
+        *,
+        createdAfter: TimestampTypeDef = ...,
+        createdBefore: TimestampTypeDef = ...,
+        maxResults: int = ...,
+        nextToken: str = ...,
+    ) -> ListSecurityConfigurationsResponseTypeDef:
+        """
+        Lists security configurations based on a set of parameters.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_security_configurations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#list_security_configurations)
+        """
+
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags assigned to the resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#list_tags_for_resource)
         """
@@ -398,13 +444,22 @@
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#get_paginator)
         """
 
     @overload
     def get_paginator(
+        self, operation_name: Literal["list_security_configurations"]
+    ) -> ListSecurityConfigurationsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#get_paginator)
+        """
+
+    @overload
+    def get_paginator(
         self, operation_name: Literal["list_virtual_clusters"]
     ) -> ListVirtualClustersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/client/#get_paginator)
         """
```

### Comparing `mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/literals.py` & `mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,59 +2,63 @@
 Type annotations for emr-containers service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_emr_containers.literals import ContainerProviderTypeType
+    from mypy_boto3_emr_containers.literals import CertificateProviderTypeType
 
-    data: ContainerProviderTypeType = "EKS"
+    data: CertificateProviderTypeType = "PEM"
     ```
 """
 
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
+    "CertificateProviderTypeType",
     "ContainerProviderTypeType",
     "EndpointStateType",
     "FailureReasonType",
     "JobRunStateType",
     "ListJobRunsPaginatorName",
     "ListJobTemplatesPaginatorName",
     "ListManagedEndpointsPaginatorName",
+    "ListSecurityConfigurationsPaginatorName",
     "ListVirtualClustersPaginatorName",
     "PersistentAppUIType",
     "TemplateParameterDataTypeType",
     "VirtualClusterStateType",
     "EMRContainersServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+CertificateProviderTypeType = Literal["PEM"]
 ContainerProviderTypeType = Literal["EKS"]
 EndpointStateType = Literal[
     "ACTIVE", "CREATING", "TERMINATED", "TERMINATED_WITH_ERRORS", "TERMINATING"
 ]
 FailureReasonType = Literal[
     "CLUSTER_UNAVAILABLE", "INTERNAL_ERROR", "USER_ERROR", "VALIDATION_ERROR"
 ]
 JobRunStateType = Literal[
     "CANCELLED", "CANCEL_PENDING", "COMPLETED", "FAILED", "PENDING", "RUNNING", "SUBMITTED"
 ]
 ListJobRunsPaginatorName = Literal["list_job_runs"]
 ListJobTemplatesPaginatorName = Literal["list_job_templates"]
 ListManagedEndpointsPaginatorName = Literal["list_managed_endpoints"]
+ListSecurityConfigurationsPaginatorName = Literal["list_security_configurations"]
 ListVirtualClustersPaginatorName = Literal["list_virtual_clusters"]
 PersistentAppUIType = Literal["DISABLED", "ENABLED"]
 TemplateParameterDataTypeType = Literal["NUMBER", "STRING"]
 VirtualClusterStateType = Literal["ARRESTED", "RUNNING", "TERMINATED", "TERMINATING"]
 EMRContainersServiceName = Literal["emr-containers"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -144,14 +148,15 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
@@ -359,14 +364,15 @@
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
@@ -448,15 +454,19 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
-    "list_job_runs", "list_job_templates", "list_managed_endpoints", "list_virtual_clusters"
+    "list_job_runs",
+    "list_job_templates",
+    "list_managed_endpoints",
+    "list_security_configurations",
+    "list_virtual_clusters",
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
```

### Comparing `mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/literals.pyi` & `mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,59 +2,63 @@
 Type annotations for emr-containers service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_emr_containers.literals import ContainerProviderTypeType
+    from mypy_boto3_emr_containers.literals import CertificateProviderTypeType
 
-    data: ContainerProviderTypeType = "EKS"
+    data: CertificateProviderTypeType = "PEM"
     ```
 """
 
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
+    "CertificateProviderTypeType",
     "ContainerProviderTypeType",
     "EndpointStateType",
     "FailureReasonType",
     "JobRunStateType",
     "ListJobRunsPaginatorName",
     "ListJobTemplatesPaginatorName",
     "ListManagedEndpointsPaginatorName",
+    "ListSecurityConfigurationsPaginatorName",
     "ListVirtualClustersPaginatorName",
     "PersistentAppUIType",
     "TemplateParameterDataTypeType",
     "VirtualClusterStateType",
     "EMRContainersServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+CertificateProviderTypeType = Literal["PEM"]
 ContainerProviderTypeType = Literal["EKS"]
 EndpointStateType = Literal[
     "ACTIVE", "CREATING", "TERMINATED", "TERMINATED_WITH_ERRORS", "TERMINATING"
 ]
 FailureReasonType = Literal[
     "CLUSTER_UNAVAILABLE", "INTERNAL_ERROR", "USER_ERROR", "VALIDATION_ERROR"
 ]
 JobRunStateType = Literal[
     "CANCELLED", "CANCEL_PENDING", "COMPLETED", "FAILED", "PENDING", "RUNNING", "SUBMITTED"
 ]
 ListJobRunsPaginatorName = Literal["list_job_runs"]
 ListJobTemplatesPaginatorName = Literal["list_job_templates"]
 ListManagedEndpointsPaginatorName = Literal["list_managed_endpoints"]
+ListSecurityConfigurationsPaginatorName = Literal["list_security_configurations"]
 ListVirtualClustersPaginatorName = Literal["list_virtual_clusters"]
 PersistentAppUIType = Literal["DISABLED", "ENABLED"]
 TemplateParameterDataTypeType = Literal["NUMBER", "STRING"]
 VirtualClusterStateType = Literal["ARRESTED", "RUNNING", "TERMINATED", "TERMINATING"]
 EMRContainersServiceName = Literal["emr-containers"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -144,14 +148,15 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
@@ -359,14 +364,15 @@
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
@@ -448,15 +454,19 @@
     "iam",
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal[
-    "list_job_runs", "list_job_templates", "list_managed_endpoints", "list_virtual_clusters"
+    "list_job_runs",
+    "list_job_templates",
+    "list_managed_endpoints",
+    "list_security_configurations",
+    "list_virtual_clusters",
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
```

### Comparing `mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/paginator.py` & `mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers/paginator.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,51 +9,55 @@
     from boto3.session import Session
 
     from mypy_boto3_emr_containers.client import EMRContainersClient
     from mypy_boto3_emr_containers.paginator import (
         ListJobRunsPaginator,
         ListJobTemplatesPaginator,
         ListManagedEndpointsPaginator,
+        ListSecurityConfigurationsPaginator,
         ListVirtualClustersPaginator,
     )
 
     session = Session()
     client: EMRContainersClient = session.client("emr-containers")
 
     list_job_runs_paginator: ListJobRunsPaginator = client.get_paginator("list_job_runs")
     list_job_templates_paginator: ListJobTemplatesPaginator = client.get_paginator("list_job_templates")
     list_managed_endpoints_paginator: ListManagedEndpointsPaginator = client.get_paginator("list_managed_endpoints")
+    list_security_configurations_paginator: ListSecurityConfigurationsPaginator = client.get_paginator("list_security_configurations")
     list_virtual_clusters_paginator: ListVirtualClustersPaginator = client.get_paginator("list_virtual_clusters")
     ```
 """
 
 import sys
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import EndpointStateType, JobRunStateType, VirtualClusterStateType
 from .type_defs import (
     ListJobRunsResponsePaginatorTypeDef,
     ListJobTemplatesResponsePaginatorTypeDef,
     ListManagedEndpointsResponsePaginatorTypeDef,
+    ListSecurityConfigurationsResponseTypeDef,
     ListVirtualClustersResponseTypeDef,
     PaginatorConfigTypeDef,
     TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "ListJobRunsPaginator",
     "ListJobTemplatesPaginator",
     "ListManagedEndpointsPaginator",
+    "ListSecurityConfigurationsPaginator",
     "ListVirtualClustersPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
@@ -122,14 +126,33 @@
     ) -> _PageIterator[ListManagedEndpointsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListManagedEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listmanagedendpointspaginator)
         """
 
 
+class ListSecurityConfigurationsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListSecurityConfigurations)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listsecurityconfigurationspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        createdAfter: TimestampTypeDef = ...,
+        createdBefore: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[ListSecurityConfigurationsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListSecurityConfigurations.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listsecurityconfigurationspaginator)
+        """
+
+
 class ListVirtualClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListVirtualClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listvirtualclusterspaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/paginator.pyi` & `mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers/paginator.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -9,51 +9,55 @@
     from boto3.session import Session
 
     from mypy_boto3_emr_containers.client import EMRContainersClient
     from mypy_boto3_emr_containers.paginator import (
         ListJobRunsPaginator,
         ListJobTemplatesPaginator,
         ListManagedEndpointsPaginator,
+        ListSecurityConfigurationsPaginator,
         ListVirtualClustersPaginator,
     )
 
     session = Session()
     client: EMRContainersClient = session.client("emr-containers")
 
     list_job_runs_paginator: ListJobRunsPaginator = client.get_paginator("list_job_runs")
     list_job_templates_paginator: ListJobTemplatesPaginator = client.get_paginator("list_job_templates")
     list_managed_endpoints_paginator: ListManagedEndpointsPaginator = client.get_paginator("list_managed_endpoints")
+    list_security_configurations_paginator: ListSecurityConfigurationsPaginator = client.get_paginator("list_security_configurations")
     list_virtual_clusters_paginator: ListVirtualClustersPaginator = client.get_paginator("list_virtual_clusters")
     ```
 """
 
 import sys
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import EndpointStateType, JobRunStateType, VirtualClusterStateType
 from .type_defs import (
     ListJobRunsResponsePaginatorTypeDef,
     ListJobTemplatesResponsePaginatorTypeDef,
     ListManagedEndpointsResponsePaginatorTypeDef,
+    ListSecurityConfigurationsResponseTypeDef,
     ListVirtualClustersResponseTypeDef,
     PaginatorConfigTypeDef,
     TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "ListJobRunsPaginator",
     "ListJobTemplatesPaginator",
     "ListManagedEndpointsPaginator",
+    "ListSecurityConfigurationsPaginator",
     "ListVirtualClustersPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
@@ -117,14 +121,32 @@
         PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListManagedEndpointsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListManagedEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listmanagedendpointspaginator)
         """
 
+class ListSecurityConfigurationsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListSecurityConfigurations)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listsecurityconfigurationspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        createdAfter: TimestampTypeDef = ...,
+        createdBefore: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[ListSecurityConfigurationsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListSecurityConfigurations.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listsecurityconfigurationspaginator)
+        """
+
 class ListVirtualClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers.Paginator.ListVirtualClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/paginators/#listvirtualclusterspaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/type_defs.py` & `mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers/type_defs.py`

 * *Files 15% similar despite different names*

```diff
@@ -50,82 +50,97 @@
     "CredentialsTypeDef",
     "DeleteJobTemplateRequestRequestTypeDef",
     "DeleteManagedEndpointRequestRequestTypeDef",
     "DeleteVirtualClusterRequestRequestTypeDef",
     "DescribeJobRunRequestRequestTypeDef",
     "DescribeJobTemplateRequestRequestTypeDef",
     "DescribeManagedEndpointRequestRequestTypeDef",
+    "DescribeSecurityConfigurationRequestRequestTypeDef",
     "DescribeVirtualClusterRequestRequestTypeDef",
     "GetManagedEndpointSessionCredentialsRequestRequestTypeDef",
+    "TLSCertificateConfigurationTypeDef",
     "SparkSqlJobDriverTypeDef",
     "SparkSubmitJobDriverPaginatorTypeDef",
     "SparkSubmitJobDriverTypeDef",
     "RetryPolicyConfigurationTypeDef",
     "RetryPolicyExecutionTypeDef",
     "TemplateParameterConfigurationTypeDef",
+    "SecureNamespaceInfoTypeDef",
     "PaginatorConfigTypeDef",
     "TimestampTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "S3MonitoringConfigurationTypeDef",
     "ParametricCloudWatchMonitoringConfigurationTypeDef",
     "ParametricS3MonitoringConfigurationTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "CancelJobRunResponseTypeDef",
     "CreateJobTemplateResponseTypeDef",
     "CreateManagedEndpointResponseTypeDef",
+    "CreateSecurityConfigurationResponseTypeDef",
     "CreateVirtualClusterResponseTypeDef",
     "DeleteJobTemplateResponseTypeDef",
     "DeleteManagedEndpointResponseTypeDef",
     "DeleteVirtualClusterResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartJobRunResponseTypeDef",
     "ContainerInfoTypeDef",
     "GetManagedEndpointSessionCredentialsResponseTypeDef",
+    "InTransitEncryptionConfigurationTypeDef",
     "JobDriverPaginatorTypeDef",
     "JobDriverTypeDef",
+    "LakeFormationConfigurationTypeDef",
     "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "ListJobRunsRequestRequestTypeDef",
     "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     "ListJobTemplatesRequestRequestTypeDef",
     "ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
     "ListManagedEndpointsRequestRequestTypeDef",
+    "ListSecurityConfigurationsRequestListSecurityConfigurationsPaginateTypeDef",
+    "ListSecurityConfigurationsRequestRequestTypeDef",
     "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
     "ListVirtualClustersRequestRequestTypeDef",
     "MonitoringConfigurationTypeDef",
     "ParametricMonitoringConfigurationTypeDef",
     "ContainerProviderTypeDef",
+    "EncryptionConfigurationTypeDef",
     "ConfigurationOverridesPaginatorTypeDef",
     "ConfigurationOverridesTypeDef",
     "ParametricConfigurationOverridesPaginatorTypeDef",
     "ParametricConfigurationOverridesTypeDef",
     "CreateVirtualClusterRequestRequestTypeDef",
     "VirtualClusterTypeDef",
+    "AuthorizationConfigurationTypeDef",
     "EndpointPaginatorTypeDef",
     "JobRunPaginatorTypeDef",
     "CreateManagedEndpointRequestRequestTypeDef",
     "EndpointTypeDef",
     "JobRunTypeDef",
     "StartJobRunRequestRequestTypeDef",
     "JobTemplateDataPaginatorTypeDef",
     "JobTemplateDataTypeDef",
     "DescribeVirtualClusterResponseTypeDef",
     "ListVirtualClustersResponseTypeDef",
+    "SecurityConfigurationDataTypeDef",
     "ListManagedEndpointsResponsePaginatorTypeDef",
     "ListJobRunsResponsePaginatorTypeDef",
     "DescribeManagedEndpointResponseTypeDef",
     "ListManagedEndpointsResponseTypeDef",
     "DescribeJobRunResponseTypeDef",
     "ListJobRunsResponseTypeDef",
     "JobTemplatePaginatorTypeDef",
     "CreateJobTemplateRequestRequestTypeDef",
     "JobTemplateTypeDef",
+    "CreateSecurityConfigurationRequestRequestTypeDef",
+    "SecurityConfigurationTypeDef",
     "ListJobTemplatesResponsePaginatorTypeDef",
     "DescribeJobTemplateResponseTypeDef",
     "ListJobTemplatesResponseTypeDef",
+    "DescribeSecurityConfigurationResponseTypeDef",
+    "ListSecurityConfigurationsResponseTypeDef",
 )
 
 CancelJobRunRequestRequestTypeDef = TypedDict(
     "CancelJobRunRequestRequestTypeDef",
     {
         "id": str,
         "virtualClusterId": str,
@@ -225,14 +240,20 @@
 DescribeManagedEndpointRequestRequestTypeDef = TypedDict(
     "DescribeManagedEndpointRequestRequestTypeDef",
     {
         "id": str,
         "virtualClusterId": str,
     },
 )
+DescribeSecurityConfigurationRequestRequestTypeDef = TypedDict(
+    "DescribeSecurityConfigurationRequestRequestTypeDef",
+    {
+        "id": str,
+    },
+)
 DescribeVirtualClusterRequestRequestTypeDef = TypedDict(
     "DescribeVirtualClusterRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 GetManagedEndpointSessionCredentialsRequestRequestTypeDef = TypedDict(
@@ -243,14 +264,22 @@
         "executionRoleArn": str,
         "credentialType": str,
         "durationInSeconds": NotRequired[int],
         "logContext": NotRequired[str],
         "clientToken": NotRequired[str],
     },
 )
+TLSCertificateConfigurationTypeDef = TypedDict(
+    "TLSCertificateConfigurationTypeDef",
+    {
+        "certificateProviderType": NotRequired[Literal["PEM"]],
+        "publicCertificateSecretArn": NotRequired[str],
+        "privateCertificateSecretArn": NotRequired[str],
+    },
+)
 SparkSqlJobDriverTypeDef = TypedDict(
     "SparkSqlJobDriverTypeDef",
     {
         "entryPoint": NotRequired[str],
         "sparkSqlParameters": NotRequired[str],
     },
 )
@@ -285,14 +314,21 @@
 TemplateParameterConfigurationTypeDef = TypedDict(
     "TemplateParameterConfigurationTypeDef",
     {
         "type": NotRequired[TemplateParameterDataTypeType],
         "defaultValue": NotRequired[str],
     },
 )
+SecureNamespaceInfoTypeDef = TypedDict(
+    "SecureNamespaceInfoTypeDef",
+    {
+        "clusterId": NotRequired[str],
+        "namespace": NotRequired[str],
+    },
+)
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": NotRequired[int],
         "PageSize": NotRequired[int],
         "StartingToken": NotRequired[str],
     },
@@ -361,14 +397,23 @@
         "id": str,
         "name": str,
         "arn": str,
         "virtualClusterId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateSecurityConfigurationResponseTypeDef = TypedDict(
+    "CreateSecurityConfigurationResponseTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 CreateVirtualClusterResponseTypeDef = TypedDict(
     "CreateVirtualClusterResponseTypeDef",
     {
         "id": str,
         "name": str,
         "arn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -424,28 +469,42 @@
     {
         "id": str,
         "credentials": CredentialsTypeDef,
         "expiresAt": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+InTransitEncryptionConfigurationTypeDef = TypedDict(
+    "InTransitEncryptionConfigurationTypeDef",
+    {
+        "tlsCertificateConfiguration": NotRequired[TLSCertificateConfigurationTypeDef],
+    },
+)
 JobDriverPaginatorTypeDef = TypedDict(
     "JobDriverPaginatorTypeDef",
     {
         "sparkSubmitJobDriver": NotRequired[SparkSubmitJobDriverPaginatorTypeDef],
         "sparkSqlJobDriver": NotRequired[SparkSqlJobDriverTypeDef],
     },
 )
 JobDriverTypeDef = TypedDict(
     "JobDriverTypeDef",
     {
         "sparkSubmitJobDriver": NotRequired[SparkSubmitJobDriverTypeDef],
         "sparkSqlJobDriver": NotRequired[SparkSqlJobDriverTypeDef],
     },
 )
+LakeFormationConfigurationTypeDef = TypedDict(
+    "LakeFormationConfigurationTypeDef",
+    {
+        "authorizedSessionTagValue": NotRequired[str],
+        "secureNamespaceInfo": NotRequired[SecureNamespaceInfoTypeDef],
+        "queryEngineRoleArn": NotRequired[str],
+    },
+)
 ListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
     "ListJobRunsRequestListJobRunsPaginateTypeDef",
     {
         "virtualClusterId": str,
         "createdBefore": NotRequired[TimestampTypeDef],
         "createdAfter": NotRequired[TimestampTypeDef],
         "name": NotRequired[str],
@@ -501,14 +560,31 @@
         "createdAfter": NotRequired[TimestampTypeDef],
         "types": NotRequired[Sequence[str]],
         "states": NotRequired[Sequence[EndpointStateType]],
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
     },
 )
+ListSecurityConfigurationsRequestListSecurityConfigurationsPaginateTypeDef = TypedDict(
+    "ListSecurityConfigurationsRequestListSecurityConfigurationsPaginateTypeDef",
+    {
+        "createdAfter": NotRequired[TimestampTypeDef],
+        "createdBefore": NotRequired[TimestampTypeDef],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
+ListSecurityConfigurationsRequestRequestTypeDef = TypedDict(
+    "ListSecurityConfigurationsRequestRequestTypeDef",
+    {
+        "createdAfter": NotRequired[TimestampTypeDef],
+        "createdBefore": NotRequired[TimestampTypeDef],
+        "maxResults": NotRequired[int],
+        "nextToken": NotRequired[str],
+    },
+)
 ListVirtualClustersRequestListVirtualClustersPaginateTypeDef = TypedDict(
     "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
     {
         "containerProviderId": NotRequired[str],
         "containerProviderType": NotRequired[Literal["EKS"]],
         "createdAfter": NotRequired[TimestampTypeDef],
         "createdBefore": NotRequired[TimestampTypeDef],
@@ -553,14 +629,20 @@
     "ContainerProviderTypeDef",
     {
         "type": Literal["EKS"],
         "id": str,
         "info": NotRequired[ContainerInfoTypeDef],
     },
 )
+EncryptionConfigurationTypeDef = TypedDict(
+    "EncryptionConfigurationTypeDef",
+    {
+        "inTransitEncryptionConfiguration": NotRequired[InTransitEncryptionConfigurationTypeDef],
+    },
+)
 ConfigurationOverridesPaginatorTypeDef = TypedDict(
     "ConfigurationOverridesPaginatorTypeDef",
     {
         "applicationConfiguration": NotRequired[List["ConfigurationPaginatorTypeDef"]],
         "monitoringConfiguration": NotRequired[MonitoringConfigurationTypeDef],
     },
 )
@@ -588,26 +670,35 @@
 CreateVirtualClusterRequestRequestTypeDef = TypedDict(
     "CreateVirtualClusterRequestRequestTypeDef",
     {
         "name": str,
         "containerProvider": ContainerProviderTypeDef,
         "clientToken": str,
         "tags": NotRequired[Mapping[str, str]],
+        "securityConfigurationId": NotRequired[str],
     },
 )
 VirtualClusterTypeDef = TypedDict(
     "VirtualClusterTypeDef",
     {
         "id": NotRequired[str],
         "name": NotRequired[str],
         "arn": NotRequired[str],
         "state": NotRequired[VirtualClusterStateType],
         "containerProvider": NotRequired[ContainerProviderTypeDef],
         "createdAt": NotRequired[datetime],
         "tags": NotRequired[Dict[str, str]],
+        "securityConfigurationId": NotRequired[str],
+    },
+)
+AuthorizationConfigurationTypeDef = TypedDict(
+    "AuthorizationConfigurationTypeDef",
+    {
+        "lakeFormationConfiguration": NotRequired[LakeFormationConfigurationTypeDef],
+        "encryptionConfiguration": NotRequired[EncryptionConfigurationTypeDef],
     },
 )
 EndpointPaginatorTypeDef = TypedDict(
     "EndpointPaginatorTypeDef",
     {
         "id": NotRequired[str],
         "name": NotRequired[str],
@@ -761,14 +852,20 @@
     "ListVirtualClustersResponseTypeDef",
     {
         "virtualClusters": List[VirtualClusterTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+SecurityConfigurationDataTypeDef = TypedDict(
+    "SecurityConfigurationDataTypeDef",
+    {
+        "authorizationConfiguration": NotRequired[AuthorizationConfigurationTypeDef],
+    },
+)
 ListManagedEndpointsResponsePaginatorTypeDef = TypedDict(
     "ListManagedEndpointsResponsePaginatorTypeDef",
     {
         "endpoints": List[EndpointPaginatorTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -845,14 +942,35 @@
         "createdAt": NotRequired[datetime],
         "createdBy": NotRequired[str],
         "tags": NotRequired[Dict[str, str]],
         "kmsKeyArn": NotRequired[str],
         "decryptionError": NotRequired[str],
     },
 )
+CreateSecurityConfigurationRequestRequestTypeDef = TypedDict(
+    "CreateSecurityConfigurationRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "name": str,
+        "securityConfigurationData": SecurityConfigurationDataTypeDef,
+        "tags": NotRequired[Mapping[str, str]],
+    },
+)
+SecurityConfigurationTypeDef = TypedDict(
+    "SecurityConfigurationTypeDef",
+    {
+        "id": NotRequired[str],
+        "name": NotRequired[str],
+        "arn": NotRequired[str],
+        "createdAt": NotRequired[datetime],
+        "createdBy": NotRequired[str],
+        "securityConfigurationData": NotRequired[SecurityConfigurationDataTypeDef],
+        "tags": NotRequired[Dict[str, str]],
+    },
+)
 ListJobTemplatesResponsePaginatorTypeDef = TypedDict(
     "ListJobTemplatesResponsePaginatorTypeDef",
     {
         "templates": List[JobTemplatePaginatorTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -868,7 +986,22 @@
     "ListJobTemplatesResponseTypeDef",
     {
         "templates": List[JobTemplateTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DescribeSecurityConfigurationResponseTypeDef = TypedDict(
+    "DescribeSecurityConfigurationResponseTypeDef",
+    {
+        "securityConfiguration": SecurityConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ListSecurityConfigurationsResponseTypeDef = TypedDict(
+    "ListSecurityConfigurationsResponseTypeDef",
+    {
+        "securityConfigurations": List[SecurityConfigurationTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers/type_defs.pyi` & `mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers/type_defs.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -50,82 +50,97 @@
     "CredentialsTypeDef",
     "DeleteJobTemplateRequestRequestTypeDef",
     "DeleteManagedEndpointRequestRequestTypeDef",
     "DeleteVirtualClusterRequestRequestTypeDef",
     "DescribeJobRunRequestRequestTypeDef",
     "DescribeJobTemplateRequestRequestTypeDef",
     "DescribeManagedEndpointRequestRequestTypeDef",
+    "DescribeSecurityConfigurationRequestRequestTypeDef",
     "DescribeVirtualClusterRequestRequestTypeDef",
     "GetManagedEndpointSessionCredentialsRequestRequestTypeDef",
+    "TLSCertificateConfigurationTypeDef",
     "SparkSqlJobDriverTypeDef",
     "SparkSubmitJobDriverPaginatorTypeDef",
     "SparkSubmitJobDriverTypeDef",
     "RetryPolicyConfigurationTypeDef",
     "RetryPolicyExecutionTypeDef",
     "TemplateParameterConfigurationTypeDef",
+    "SecureNamespaceInfoTypeDef",
     "PaginatorConfigTypeDef",
     "TimestampTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "S3MonitoringConfigurationTypeDef",
     "ParametricCloudWatchMonitoringConfigurationTypeDef",
     "ParametricS3MonitoringConfigurationTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "CancelJobRunResponseTypeDef",
     "CreateJobTemplateResponseTypeDef",
     "CreateManagedEndpointResponseTypeDef",
+    "CreateSecurityConfigurationResponseTypeDef",
     "CreateVirtualClusterResponseTypeDef",
     "DeleteJobTemplateResponseTypeDef",
     "DeleteManagedEndpointResponseTypeDef",
     "DeleteVirtualClusterResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartJobRunResponseTypeDef",
     "ContainerInfoTypeDef",
     "GetManagedEndpointSessionCredentialsResponseTypeDef",
+    "InTransitEncryptionConfigurationTypeDef",
     "JobDriverPaginatorTypeDef",
     "JobDriverTypeDef",
+    "LakeFormationConfigurationTypeDef",
     "ListJobRunsRequestListJobRunsPaginateTypeDef",
     "ListJobRunsRequestRequestTypeDef",
     "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     "ListJobTemplatesRequestRequestTypeDef",
     "ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef",
     "ListManagedEndpointsRequestRequestTypeDef",
+    "ListSecurityConfigurationsRequestListSecurityConfigurationsPaginateTypeDef",
+    "ListSecurityConfigurationsRequestRequestTypeDef",
     "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
     "ListVirtualClustersRequestRequestTypeDef",
     "MonitoringConfigurationTypeDef",
     "ParametricMonitoringConfigurationTypeDef",
     "ContainerProviderTypeDef",
+    "EncryptionConfigurationTypeDef",
     "ConfigurationOverridesPaginatorTypeDef",
     "ConfigurationOverridesTypeDef",
     "ParametricConfigurationOverridesPaginatorTypeDef",
     "ParametricConfigurationOverridesTypeDef",
     "CreateVirtualClusterRequestRequestTypeDef",
     "VirtualClusterTypeDef",
+    "AuthorizationConfigurationTypeDef",
     "EndpointPaginatorTypeDef",
     "JobRunPaginatorTypeDef",
     "CreateManagedEndpointRequestRequestTypeDef",
     "EndpointTypeDef",
     "JobRunTypeDef",
     "StartJobRunRequestRequestTypeDef",
     "JobTemplateDataPaginatorTypeDef",
     "JobTemplateDataTypeDef",
     "DescribeVirtualClusterResponseTypeDef",
     "ListVirtualClustersResponseTypeDef",
+    "SecurityConfigurationDataTypeDef",
     "ListManagedEndpointsResponsePaginatorTypeDef",
     "ListJobRunsResponsePaginatorTypeDef",
     "DescribeManagedEndpointResponseTypeDef",
     "ListManagedEndpointsResponseTypeDef",
     "DescribeJobRunResponseTypeDef",
     "ListJobRunsResponseTypeDef",
     "JobTemplatePaginatorTypeDef",
     "CreateJobTemplateRequestRequestTypeDef",
     "JobTemplateTypeDef",
+    "CreateSecurityConfigurationRequestRequestTypeDef",
+    "SecurityConfigurationTypeDef",
     "ListJobTemplatesResponsePaginatorTypeDef",
     "DescribeJobTemplateResponseTypeDef",
     "ListJobTemplatesResponseTypeDef",
+    "DescribeSecurityConfigurationResponseTypeDef",
+    "ListSecurityConfigurationsResponseTypeDef",
 )
 
 CancelJobRunRequestRequestTypeDef = TypedDict(
     "CancelJobRunRequestRequestTypeDef",
     {
         "id": str,
         "virtualClusterId": str,
@@ -225,14 +240,20 @@
 DescribeManagedEndpointRequestRequestTypeDef = TypedDict(
     "DescribeManagedEndpointRequestRequestTypeDef",
     {
         "id": str,
         "virtualClusterId": str,
     },
 )
+DescribeSecurityConfigurationRequestRequestTypeDef = TypedDict(
+    "DescribeSecurityConfigurationRequestRequestTypeDef",
+    {
+        "id": str,
+    },
+)
 DescribeVirtualClusterRequestRequestTypeDef = TypedDict(
     "DescribeVirtualClusterRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 GetManagedEndpointSessionCredentialsRequestRequestTypeDef = TypedDict(
@@ -243,14 +264,22 @@
         "executionRoleArn": str,
         "credentialType": str,
         "durationInSeconds": NotRequired[int],
         "logContext": NotRequired[str],
         "clientToken": NotRequired[str],
     },
 )
+TLSCertificateConfigurationTypeDef = TypedDict(
+    "TLSCertificateConfigurationTypeDef",
+    {
+        "certificateProviderType": NotRequired[Literal["PEM"]],
+        "publicCertificateSecretArn": NotRequired[str],
+        "privateCertificateSecretArn": NotRequired[str],
+    },
+)
 SparkSqlJobDriverTypeDef = TypedDict(
     "SparkSqlJobDriverTypeDef",
     {
         "entryPoint": NotRequired[str],
         "sparkSqlParameters": NotRequired[str],
     },
 )
@@ -285,14 +314,21 @@
 TemplateParameterConfigurationTypeDef = TypedDict(
     "TemplateParameterConfigurationTypeDef",
     {
         "type": NotRequired[TemplateParameterDataTypeType],
         "defaultValue": NotRequired[str],
     },
 )
+SecureNamespaceInfoTypeDef = TypedDict(
+    "SecureNamespaceInfoTypeDef",
+    {
+        "clusterId": NotRequired[str],
+        "namespace": NotRequired[str],
+    },
+)
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": NotRequired[int],
         "PageSize": NotRequired[int],
         "StartingToken": NotRequired[str],
     },
@@ -361,14 +397,23 @@
         "id": str,
         "name": str,
         "arn": str,
         "virtualClusterId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateSecurityConfigurationResponseTypeDef = TypedDict(
+    "CreateSecurityConfigurationResponseTypeDef",
+    {
+        "id": str,
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 CreateVirtualClusterResponseTypeDef = TypedDict(
     "CreateVirtualClusterResponseTypeDef",
     {
         "id": str,
         "name": str,
         "arn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -424,28 +469,42 @@
     {
         "id": str,
         "credentials": CredentialsTypeDef,
         "expiresAt": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+InTransitEncryptionConfigurationTypeDef = TypedDict(
+    "InTransitEncryptionConfigurationTypeDef",
+    {
+        "tlsCertificateConfiguration": NotRequired[TLSCertificateConfigurationTypeDef],
+    },
+)
 JobDriverPaginatorTypeDef = TypedDict(
     "JobDriverPaginatorTypeDef",
     {
         "sparkSubmitJobDriver": NotRequired[SparkSubmitJobDriverPaginatorTypeDef],
         "sparkSqlJobDriver": NotRequired[SparkSqlJobDriverTypeDef],
     },
 )
 JobDriverTypeDef = TypedDict(
     "JobDriverTypeDef",
     {
         "sparkSubmitJobDriver": NotRequired[SparkSubmitJobDriverTypeDef],
         "sparkSqlJobDriver": NotRequired[SparkSqlJobDriverTypeDef],
     },
 )
+LakeFormationConfigurationTypeDef = TypedDict(
+    "LakeFormationConfigurationTypeDef",
+    {
+        "authorizedSessionTagValue": NotRequired[str],
+        "secureNamespaceInfo": NotRequired[SecureNamespaceInfoTypeDef],
+        "queryEngineRoleArn": NotRequired[str],
+    },
+)
 ListJobRunsRequestListJobRunsPaginateTypeDef = TypedDict(
     "ListJobRunsRequestListJobRunsPaginateTypeDef",
     {
         "virtualClusterId": str,
         "createdBefore": NotRequired[TimestampTypeDef],
         "createdAfter": NotRequired[TimestampTypeDef],
         "name": NotRequired[str],
@@ -501,14 +560,31 @@
         "createdAfter": NotRequired[TimestampTypeDef],
         "types": NotRequired[Sequence[str]],
         "states": NotRequired[Sequence[EndpointStateType]],
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
     },
 )
+ListSecurityConfigurationsRequestListSecurityConfigurationsPaginateTypeDef = TypedDict(
+    "ListSecurityConfigurationsRequestListSecurityConfigurationsPaginateTypeDef",
+    {
+        "createdAfter": NotRequired[TimestampTypeDef],
+        "createdBefore": NotRequired[TimestampTypeDef],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
+ListSecurityConfigurationsRequestRequestTypeDef = TypedDict(
+    "ListSecurityConfigurationsRequestRequestTypeDef",
+    {
+        "createdAfter": NotRequired[TimestampTypeDef],
+        "createdBefore": NotRequired[TimestampTypeDef],
+        "maxResults": NotRequired[int],
+        "nextToken": NotRequired[str],
+    },
+)
 ListVirtualClustersRequestListVirtualClustersPaginateTypeDef = TypedDict(
     "ListVirtualClustersRequestListVirtualClustersPaginateTypeDef",
     {
         "containerProviderId": NotRequired[str],
         "containerProviderType": NotRequired[Literal["EKS"]],
         "createdAfter": NotRequired[TimestampTypeDef],
         "createdBefore": NotRequired[TimestampTypeDef],
@@ -553,14 +629,20 @@
     "ContainerProviderTypeDef",
     {
         "type": Literal["EKS"],
         "id": str,
         "info": NotRequired[ContainerInfoTypeDef],
     },
 )
+EncryptionConfigurationTypeDef = TypedDict(
+    "EncryptionConfigurationTypeDef",
+    {
+        "inTransitEncryptionConfiguration": NotRequired[InTransitEncryptionConfigurationTypeDef],
+    },
+)
 ConfigurationOverridesPaginatorTypeDef = TypedDict(
     "ConfigurationOverridesPaginatorTypeDef",
     {
         "applicationConfiguration": NotRequired[List["ConfigurationPaginatorTypeDef"]],
         "monitoringConfiguration": NotRequired[MonitoringConfigurationTypeDef],
     },
 )
@@ -588,26 +670,35 @@
 CreateVirtualClusterRequestRequestTypeDef = TypedDict(
     "CreateVirtualClusterRequestRequestTypeDef",
     {
         "name": str,
         "containerProvider": ContainerProviderTypeDef,
         "clientToken": str,
         "tags": NotRequired[Mapping[str, str]],
+        "securityConfigurationId": NotRequired[str],
     },
 )
 VirtualClusterTypeDef = TypedDict(
     "VirtualClusterTypeDef",
     {
         "id": NotRequired[str],
         "name": NotRequired[str],
         "arn": NotRequired[str],
         "state": NotRequired[VirtualClusterStateType],
         "containerProvider": NotRequired[ContainerProviderTypeDef],
         "createdAt": NotRequired[datetime],
         "tags": NotRequired[Dict[str, str]],
+        "securityConfigurationId": NotRequired[str],
+    },
+)
+AuthorizationConfigurationTypeDef = TypedDict(
+    "AuthorizationConfigurationTypeDef",
+    {
+        "lakeFormationConfiguration": NotRequired[LakeFormationConfigurationTypeDef],
+        "encryptionConfiguration": NotRequired[EncryptionConfigurationTypeDef],
     },
 )
 EndpointPaginatorTypeDef = TypedDict(
     "EndpointPaginatorTypeDef",
     {
         "id": NotRequired[str],
         "name": NotRequired[str],
@@ -761,14 +852,20 @@
     "ListVirtualClustersResponseTypeDef",
     {
         "virtualClusters": List[VirtualClusterTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+SecurityConfigurationDataTypeDef = TypedDict(
+    "SecurityConfigurationDataTypeDef",
+    {
+        "authorizationConfiguration": NotRequired[AuthorizationConfigurationTypeDef],
+    },
+)
 ListManagedEndpointsResponsePaginatorTypeDef = TypedDict(
     "ListManagedEndpointsResponsePaginatorTypeDef",
     {
         "endpoints": List[EndpointPaginatorTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -845,14 +942,35 @@
         "createdAt": NotRequired[datetime],
         "createdBy": NotRequired[str],
         "tags": NotRequired[Dict[str, str]],
         "kmsKeyArn": NotRequired[str],
         "decryptionError": NotRequired[str],
     },
 )
+CreateSecurityConfigurationRequestRequestTypeDef = TypedDict(
+    "CreateSecurityConfigurationRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "name": str,
+        "securityConfigurationData": SecurityConfigurationDataTypeDef,
+        "tags": NotRequired[Mapping[str, str]],
+    },
+)
+SecurityConfigurationTypeDef = TypedDict(
+    "SecurityConfigurationTypeDef",
+    {
+        "id": NotRequired[str],
+        "name": NotRequired[str],
+        "arn": NotRequired[str],
+        "createdAt": NotRequired[datetime],
+        "createdBy": NotRequired[str],
+        "securityConfigurationData": NotRequired[SecurityConfigurationDataTypeDef],
+        "tags": NotRequired[Dict[str, str]],
+    },
+)
 ListJobTemplatesResponsePaginatorTypeDef = TypedDict(
     "ListJobTemplatesResponsePaginatorTypeDef",
     {
         "templates": List[JobTemplatePaginatorTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -868,7 +986,22 @@
     "ListJobTemplatesResponseTypeDef",
     {
         "templates": List[JobTemplateTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DescribeSecurityConfigurationResponseTypeDef = TypedDict(
+    "DescribeSecurityConfigurationResponseTypeDef",
+    {
+        "securityConfiguration": SecurityConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ListSecurityConfigurationsResponseTypeDef = TypedDict(
+    "ListSecurityConfigurationsResponseTypeDef",
+    {
+        "securityConfigurations": List[SecurityConfigurationTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers.egg-info/PKG-INFO` & `mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr-containers
-Version: 1.34.78
-Summary: Type annotations for boto3.EMRContainers 1.34.78 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.91
+Summary: Type annotations for boto3.EMRContainers 1.34.91 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr-containers.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr-containers)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr-containers)](https://pepy.tech/project/mypy-boto3-emr-containers)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMRContainers 1.34.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
+[boto3.EMRContainers 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -285,26 +285,30 @@
 from boto3.session import Session
 
 from mypy_boto3_emr_containers import EMRContainersClient
 from mypy_boto3_emr_containers.paginator import (
     ListJobRunsPaginator,
     ListJobTemplatesPaginator,
     ListManagedEndpointsPaginator,
+    ListSecurityConfigurationsPaginator,
     ListVirtualClustersPaginator,
 )
 
 client: EMRContainersClient = Session().client("emr-containers")
 
 # Explicit type annotations are optional here
 # Types should be correctly discovered by mypy and IDEs
 list_job_runs_paginator: ListJobRunsPaginator = client.get_paginator("list_job_runs")
 list_job_templates_paginator: ListJobTemplatesPaginator = client.get_paginator("list_job_templates")
 list_managed_endpoints_paginator: ListManagedEndpointsPaginator = client.get_paginator(
     "list_managed_endpoints"
 )
+list_security_configurations_paginator: ListSecurityConfigurationsPaginator = client.get_paginator(
+    "list_security_configurations"
+)
 list_virtual_clusters_paginator: ListVirtualClustersPaginator = client.get_paginator(
     "list_virtual_clusters"
 )
 ```
 
 <a id="literals"></a>
 
@@ -313,18 +317,18 @@
 `mypy_boto3_emr_containers.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
 Full list of `EMRContainers` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr_containers/literals/).
 
 ```python
-from mypy_boto3_emr_containers.literals import ContainerProviderTypeType
+from mypy_boto3_emr_containers.literals import CertificateProviderTypeType
 
 
-def check_value(value: ContainerProviderTypeType) -> bool: ...
+def check_value(value: CertificateProviderTypeType) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_emr_containers.type_defs` module contains structures and shapes
```

### Comparing `mypy-boto3-emr-containers-1.34.78/mypy_boto3_emr_containers.egg-info/SOURCES.txt` & `mypy_boto3_emr_containers-1.34.91/mypy_boto3_emr_containers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-containers-1.34.78/setup.py` & `mypy_boto3_emr_containers-1.34.91/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-emr-containers",
-    version="1.34.78",
+    version="1.34.91",
     packages=["mypy_boto3_emr_containers"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.EMRContainers 1.34.78 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.EMRContainers 1.34.91 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

