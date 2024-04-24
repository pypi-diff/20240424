# Comparing `tmp/mypy-boto3-datasync-1.34.37.tar.gz` & `tmp/mypy_boto3_datasync-1.34.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-datasync-1.34.37.tar", last modified: Wed Feb  7 20:32:17 2024, max compression
+gzip compressed data, was "mypy_boto3_datasync-1.34.91.tar", last modified: Wed Apr 24 19:19:04 2024, max compression
```

## Comparing `mypy-boto3-datasync-1.34.37.tar` & `mypy_boto3_datasync-1.34.91.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 20:32:17.981119 mypy-boto3-datasync-1.34.37/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-07 20:31:47.000000 mypy-boto3-datasync-1.34.37/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-02-07 20:32:17.981119 mypy-boto3-datasync-1.34.37/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-02-07 20:31:47.000000 mypy-boto3-datasync-1.34.37/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 20:32:17.981119 mypy-boto3-datasync-1.34.37/mypy_boto3_datasync/
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-02-07 20:31:47.000000 mypy-boto3-datasync-1.34.37/mypy_boto3_datasync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-02-07 20:31:47.000000 mypy-boto3-datasync-1.34.37/mypy_boto3_datasync/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-02-07 20:31:47.000000 mypy-boto3-datasync-1.34.37/mypy_boto3_datasync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48473 2024-02-07 20:31:48.000000 mypy-boto3-datasync-1.34.37/mypy_boto3_datasync/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    48470 2024-02-07 20:31:48.000000 mypy-boto3-datasync-1.34.37/mypy_boto3_datasync/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14094 2024-02-07 20:31:48.000000 mypy-boto3-datasync-1.34.37/mypy_boto3_datasync/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14094 2024-02-07 20:31:48.000000 mypy-boto3-datasync-1.34.37/mypy_boto3_datasync/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9875 2024-02-07 20:31:48.000000 mypy-boto3-datasync-1.34.37/mypy_boto3_datasync/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-02-07 20:31:48.000000 mypy-boto3-datasync-1.34.37/mypy_boto3_datasync/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 20:31:47.000000 mypy-boto3-datasync-1.34.37/mypy_boto3_datasync/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    53477 2024-02-07 20:31:49.000000 mypy-boto3-datasync-1.34.37/mypy_boto3_datasync/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    53477 2024-02-07 20:31:49.000000 mypy-boto3-datasync-1.34.37/mypy_boto3_datasync/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-07 20:31:47.000000 mypy-boto3-datasync-1.34.37/mypy_boto3_datasync/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 20:32:17.981119 mypy-boto3-datasync-1.34.37/mypy_boto3_datasync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-02-07 20:32:17.000000 mypy-boto3-datasync-1.34.37/mypy_boto3_datasync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-02-07 20:32:17.000000 mypy-boto3-datasync-1.34.37/mypy_boto3_datasync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 20:32:17.000000 mypy-boto3-datasync-1.34.37/mypy_boto3_datasync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 20:32:17.000000 mypy-boto3-datasync-1.34.37/mypy_boto3_datasync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-07 20:32:17.000000 mypy-boto3-datasync-1.34.37/mypy_boto3_datasync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-07 20:32:17.000000 mypy-boto3-datasync-1.34.37/mypy_boto3_datasync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 20:32:17.981119 mypy-boto3-datasync-1.34.37/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-02-07 20:31:47.000000 mypy-boto3-datasync-1.34.37/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:04.979908 mypy_boto3_datasync-1.34.91/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-24 19:17:54.000000 mypy_boto3_datasync-1.34.91/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-04-24 19:19:04.979908 mypy_boto3_datasync-1.34.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-04-24 19:17:54.000000 mypy_boto3_datasync-1.34.91/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:04.979908 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-24 19:17:54.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-24 19:17:54.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-24 19:17:54.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48576 2024-04-24 19:17:54.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48573 2024-04-24 19:17:54.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-04-24 19:17:55.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14374 2024-04-24 19:17:55.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9875 2024-04-24 19:17:55.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-04-24 19:17:55.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:17:54.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    53925 2024-04-24 19:17:56.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53925 2024-04-24 19:17:55.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-24 19:17:54.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:19:04.979908 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-04-24 19:19:04.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-24 19:19:04.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:19:04.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:19:04.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-24 19:19:04.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-24 19:19:04.000000 mypy_boto3_datasync-1.34.91/mypy_boto3_datasync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:19:04.979908 mypy_boto3_datasync-1.34.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-24 19:17:54.000000 mypy_boto3_datasync-1.34.91/setup.py
```

### Comparing `mypy-boto3-datasync-1.34.37/LICENSE` & `mypy_boto3_datasync-1.34.91/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.34.37/PKG-INFO` & `mypy_boto3_datasync-1.34.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-datasync
-Version: 1.34.37
-Summary: Type annotations for boto3.DataSync 1.34.37 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.91
+Summary: Type annotations for boto3.DataSync 1.34.91 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datasync.svg?color=blue)](https://pypi.org/project/mypy-boto3-datasync)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-datasync)](https://pepy.tech/project/mypy-boto3-datasync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataSync 1.34.37](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
+[boto3.DataSync 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-datasync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-datasync-1.34.37/README.md` & `mypy_boto3_datasync-1.34.91/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datasync.svg?color=blue)](https://pypi.org/project/mypy-boto3-datasync)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-datasync)](https://pepy.tech/project/mypy-boto3-datasync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataSync 1.34.37](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
+[boto3.DataSync 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-datasync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-datasync-1.34.37/mypy_boto3_datasync/__init__.py` & `mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.34.37/mypy_boto3_datasync/__init__.pyi` & `mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.34.37/mypy_boto3_datasync/__main__.py` & `mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DataSync 1.34.37\n"
-        "Version:         1.34.37\n"
-        "Builder version: 7.23.1\n"
+        "Type annotations for boto3.DataSync 1.34.91\n"
+        "Version:         1.34.91\n"
+        "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.37")
+    print("1.34.91")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-datasync-1.34.37/mypy_boto3_datasync/client.py` & `mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,16 +415,15 @@
         Schedule: TaskScheduleTypeDef = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         Includes: Sequence[FilterRuleTypeDef] = ...,
         ManifestConfig: ManifestConfigTypeDef = ...,
         TaskReportConfig: TaskReportConfigTypeDef = ...,
     ) -> CreateTaskResponseTypeDef:
         """
-        Configures a transfer task, which defines where and how DataSync moves your
-        data.
+        Configures a *task*, which defines where and how DataSync transfers your data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_task)
         """
 
     def delete_agent(self, *, AgentArn: str) -> Dict[str, Any]:
         """
@@ -640,15 +639,17 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_storage_system_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_storage_system_resources)
         """
 
     def describe_task(self, *, TaskArn: str) -> DescribeTaskResponseTypeDef:
         """
-        Provides information about an DataSync transfer task.
+        Provides information about a *task*, which defines where and how DataSync
+        transfers your
+        data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_task)
         """
 
     def describe_task_execution(
         self, *, TaskExecutionArn: str
@@ -991,15 +992,17 @@
         Name: str = ...,
         CloudWatchLogGroupArn: str = ...,
         Includes: Sequence[FilterRuleTypeDef] = ...,
         ManifestConfig: ManifestConfigTypeDef = ...,
         TaskReportConfig: TaskReportConfigTypeDef = ...,
     ) -> Dict[str, Any]:
         """
-        Updates the configuration of an DataSync transfer task.
+        Updates the configuration of a *task*, which defines where and how DataSync
+        transfers your
+        data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_task)
         """
 
     def update_task_execution(
         self, *, TaskExecutionArn: str, Options: OptionsTypeDef
```

### Comparing `mypy-boto3-datasync-1.34.37/mypy_boto3_datasync/client.pyi` & `mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -412,16 +412,15 @@
         Schedule: TaskScheduleTypeDef = ...,
         Tags: Sequence[TagListEntryTypeDef] = ...,
         Includes: Sequence[FilterRuleTypeDef] = ...,
         ManifestConfig: ManifestConfigTypeDef = ...,
         TaskReportConfig: TaskReportConfigTypeDef = ...,
     ) -> CreateTaskResponseTypeDef:
         """
-        Configures a transfer task, which defines where and how DataSync moves your
-        data.
+        Configures a *task*, which defines where and how DataSync transfers your data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.create_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#create_task)
         """
 
     def delete_agent(self, *, AgentArn: str) -> Dict[str, Any]:
         """
@@ -637,15 +636,17 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_storage_system_resources)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_storage_system_resources)
         """
 
     def describe_task(self, *, TaskArn: str) -> DescribeTaskResponseTypeDef:
         """
-        Provides information about an DataSync transfer task.
+        Provides information about a *task*, which defines where and how DataSync
+        transfers your
+        data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.describe_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#describe_task)
         """
 
     def describe_task_execution(
         self, *, TaskExecutionArn: str
@@ -988,15 +989,17 @@
         Name: str = ...,
         CloudWatchLogGroupArn: str = ...,
         Includes: Sequence[FilterRuleTypeDef] = ...,
         ManifestConfig: ManifestConfigTypeDef = ...,
         TaskReportConfig: TaskReportConfigTypeDef = ...,
     ) -> Dict[str, Any]:
         """
-        Updates the configuration of an DataSync transfer task.
+        Updates the configuration of a *task*, which defines where and how DataSync
+        transfers your
+        data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync.Client.update_task)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/client/#update_task)
         """
 
     def update_task_execution(
         self, *, TaskExecutionArn: str, Options: OptionsTypeDef
```

### Comparing `mypy-boto3-datasync-1.34.37/mypy_boto3_datasync/literals.py` & `mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,16 @@
     "PosixPermissionsType",
     "PreserveDeletedFilesType",
     "PreserveDevicesType",
     "RecommendationStatusType",
     "ReportLevelType",
     "ReportOutputTypeType",
     "S3StorageClassType",
+    "ScheduleDisabledByType",
+    "ScheduleStatusType",
     "SmbSecurityDescriptorCopyFlagsType",
     "SmbVersionType",
     "StorageSystemConnectivityStatusType",
     "TaskExecutionStatusType",
     "TaskFilterNameType",
     "TaskQueueingType",
     "TaskStatusType",
@@ -143,14 +145,16 @@
     "GLACIER_INSTANT_RETRIEVAL",
     "INTELLIGENT_TIERING",
     "ONEZONE_IA",
     "OUTPOSTS",
     "STANDARD",
     "STANDARD_IA",
 ]
+ScheduleDisabledByType = Literal["SERVICE", "USER"]
+ScheduleStatusType = Literal["DISABLED", "ENABLED"]
 SmbSecurityDescriptorCopyFlagsType = Literal["NONE", "OWNER_DACL", "OWNER_DACL_SACL"]
 SmbVersionType = Literal["AUTOMATIC", "SMB1", "SMB2", "SMB2_0", "SMB3"]
 StorageSystemConnectivityStatusType = Literal["FAIL", "PASS", "UNKNOWN"]
 TaskExecutionStatusType = Literal[
     "ERROR", "LAUNCHING", "PREPARING", "QUEUED", "SUCCESS", "TRANSFERRING", "VERIFYING"
 ]
 TaskFilterNameType = Literal["CreationTime", "LocationId"]
@@ -182,14 +186,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -200,14 +205,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -225,14 +231,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -245,24 +252,26 @@
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
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -323,15 +332,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -460,14 +468,15 @@
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
@@ -511,14 +520,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-datasync-1.34.37/mypy_boto3_datasync/literals.pyi` & `mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,16 @@
     "PosixPermissionsType",
     "PreserveDeletedFilesType",
     "PreserveDevicesType",
     "RecommendationStatusType",
     "ReportLevelType",
     "ReportOutputTypeType",
     "S3StorageClassType",
+    "ScheduleDisabledByType",
+    "ScheduleStatusType",
     "SmbSecurityDescriptorCopyFlagsType",
     "SmbVersionType",
     "StorageSystemConnectivityStatusType",
     "TaskExecutionStatusType",
     "TaskFilterNameType",
     "TaskQueueingType",
     "TaskStatusType",
@@ -143,14 +145,16 @@
     "GLACIER_INSTANT_RETRIEVAL",
     "INTELLIGENT_TIERING",
     "ONEZONE_IA",
     "OUTPOSTS",
     "STANDARD",
     "STANDARD_IA",
 ]
+ScheduleDisabledByType = Literal["SERVICE", "USER"]
+ScheduleStatusType = Literal["DISABLED", "ENABLED"]
 SmbSecurityDescriptorCopyFlagsType = Literal["NONE", "OWNER_DACL", "OWNER_DACL_SACL"]
 SmbVersionType = Literal["AUTOMATIC", "SMB1", "SMB2", "SMB2_0", "SMB3"]
 StorageSystemConnectivityStatusType = Literal["FAIL", "PASS", "UNKNOWN"]
 TaskExecutionStatusType = Literal[
     "ERROR", "LAUNCHING", "PREPARING", "QUEUED", "SUCCESS", "TRANSFERRING", "VERIFYING"
 ]
 TaskFilterNameType = Literal["CreationTime", "LocationId"]
@@ -182,14 +186,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -200,14 +205,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -225,14 +231,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -245,24 +252,26 @@
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
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -323,15 +332,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -460,14 +468,15 @@
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
@@ -511,14 +520,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-datasync-1.34.37/mypy_boto3_datasync/paginator.py` & `mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.34.37/mypy_boto3_datasync/paginator.pyi` & `mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.34.37/mypy_boto3_datasync/type_defs.py` & `mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,16 @@
     PosixPermissionsType,
     PreserveDeletedFilesType,
     PreserveDevicesType,
     RecommendationStatusType,
     ReportLevelType,
     ReportOutputTypeType,
     S3StorageClassType,
+    ScheduleDisabledByType,
+    ScheduleStatusType,
     SmbSecurityDescriptorCopyFlagsType,
     SmbVersionType,
     StorageSystemConnectivityStatusType,
     TaskExecutionStatusType,
     TaskFilterNameType,
     TaskQueueingType,
     TaskStatusType,
@@ -113,14 +115,15 @@
     "PaginatorConfigTypeDef",
     "TimestampTypeDef",
     "DescribeStorageSystemResourcesRequestRequestTypeDef",
     "DescribeTaskExecutionRequestRequestTypeDef",
     "ReportResultTypeDef",
     "TaskExecutionResultDetailTypeDef",
     "DescribeTaskRequestRequestTypeDef",
+    "TaskScheduleDetailsTypeDef",
     "DiscoveryJobListEntryTypeDef",
     "GenerateRecommendationsRequestRequestTypeDef",
     "IOPSTypeDef",
     "LatencyTypeDef",
     "ListAgentsRequestRequestTypeDef",
     "ListDiscoveryJobsRequestRequestTypeDef",
     "LocationFilterTypeDef",
@@ -258,18 +261,18 @@
         "Value": NotRequired[str],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 PlatformTypeDef = TypedDict(
     "PlatformTypeDef",
     {
         "Version": NotRequired[str],
     },
@@ -368,14 +371,15 @@
         "ObjectTags": NotRequired[ObjectTagsType],
     },
 )
 TaskScheduleTypeDef = TypedDict(
     "TaskScheduleTypeDef",
     {
         "ScheduleExpression": str,
+        "Status": NotRequired[ScheduleStatusType],
     },
 )
 DeleteAgentRequestRequestTypeDef = TypedDict(
     "DeleteAgentRequestRequestTypeDef",
     {
         "AgentArn": str,
     },
@@ -535,14 +539,22 @@
 )
 DescribeTaskRequestRequestTypeDef = TypedDict(
     "DescribeTaskRequestRequestTypeDef",
     {
         "TaskArn": str,
     },
 )
+TaskScheduleDetailsTypeDef = TypedDict(
+    "TaskScheduleDetailsTypeDef",
+    {
+        "StatusUpdateTime": NotRequired[datetime],
+        "DisabledReason": NotRequired[str],
+        "DisabledBy": NotRequired[ScheduleDisabledByType],
+    },
+)
 DiscoveryJobListEntryTypeDef = TypedDict(
     "DiscoveryJobListEntryTypeDef",
     {
         "DiscoveryJobArn": NotRequired[str],
         "Status": NotRequired[DiscoveryJobStatusType],
     },
 )
@@ -1661,14 +1673,15 @@
         "Schedule": TaskScheduleTypeDef,
         "ErrorCode": str,
         "ErrorDetail": str,
         "CreationTime": datetime,
         "Includes": List[FilterRuleTypeDef],
         "ManifestConfig": ManifestConfigTypeDef,
         "TaskReportConfig": TaskReportConfigTypeDef,
+        "ScheduleDetails": TaskScheduleDetailsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 StartTaskExecutionRequestRequestTypeDef = TypedDict(
     "StartTaskExecutionRequestRequestTypeDef",
     {
         "TaskArn": str,
```

### Comparing `mypy-boto3-datasync-1.34.37/mypy_boto3_datasync/type_defs.pyi` & `mypy_boto3_datasync-1.34.91/mypy_boto3_datasync/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,16 @@
     PosixPermissionsType,
     PreserveDeletedFilesType,
     PreserveDevicesType,
     RecommendationStatusType,
     ReportLevelType,
     ReportOutputTypeType,
     S3StorageClassType,
+    ScheduleDisabledByType,
+    ScheduleStatusType,
     SmbSecurityDescriptorCopyFlagsType,
     SmbVersionType,
     StorageSystemConnectivityStatusType,
     TaskExecutionStatusType,
     TaskFilterNameType,
     TaskQueueingType,
     TaskStatusType,
@@ -113,14 +115,15 @@
     "PaginatorConfigTypeDef",
     "TimestampTypeDef",
     "DescribeStorageSystemResourcesRequestRequestTypeDef",
     "DescribeTaskExecutionRequestRequestTypeDef",
     "ReportResultTypeDef",
     "TaskExecutionResultDetailTypeDef",
     "DescribeTaskRequestRequestTypeDef",
+    "TaskScheduleDetailsTypeDef",
     "DiscoveryJobListEntryTypeDef",
     "GenerateRecommendationsRequestRequestTypeDef",
     "IOPSTypeDef",
     "LatencyTypeDef",
     "ListAgentsRequestRequestTypeDef",
     "ListDiscoveryJobsRequestRequestTypeDef",
     "LocationFilterTypeDef",
@@ -258,18 +261,18 @@
         "Value": NotRequired[str],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 PlatformTypeDef = TypedDict(
     "PlatformTypeDef",
     {
         "Version": NotRequired[str],
     },
@@ -368,14 +371,15 @@
         "ObjectTags": NotRequired[ObjectTagsType],
     },
 )
 TaskScheduleTypeDef = TypedDict(
     "TaskScheduleTypeDef",
     {
         "ScheduleExpression": str,
+        "Status": NotRequired[ScheduleStatusType],
     },
 )
 DeleteAgentRequestRequestTypeDef = TypedDict(
     "DeleteAgentRequestRequestTypeDef",
     {
         "AgentArn": str,
     },
@@ -535,14 +539,22 @@
 )
 DescribeTaskRequestRequestTypeDef = TypedDict(
     "DescribeTaskRequestRequestTypeDef",
     {
         "TaskArn": str,
     },
 )
+TaskScheduleDetailsTypeDef = TypedDict(
+    "TaskScheduleDetailsTypeDef",
+    {
+        "StatusUpdateTime": NotRequired[datetime],
+        "DisabledReason": NotRequired[str],
+        "DisabledBy": NotRequired[ScheduleDisabledByType],
+    },
+)
 DiscoveryJobListEntryTypeDef = TypedDict(
     "DiscoveryJobListEntryTypeDef",
     {
         "DiscoveryJobArn": NotRequired[str],
         "Status": NotRequired[DiscoveryJobStatusType],
     },
 )
@@ -1661,14 +1673,15 @@
         "Schedule": TaskScheduleTypeDef,
         "ErrorCode": str,
         "ErrorDetail": str,
         "CreationTime": datetime,
         "Includes": List[FilterRuleTypeDef],
         "ManifestConfig": ManifestConfigTypeDef,
         "TaskReportConfig": TaskReportConfigTypeDef,
+        "ScheduleDetails": TaskScheduleDetailsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 StartTaskExecutionRequestRequestTypeDef = TypedDict(
     "StartTaskExecutionRequestRequestTypeDef",
     {
         "TaskArn": str,
```

### Comparing `mypy-boto3-datasync-1.34.37/mypy_boto3_datasync.egg-info/PKG-INFO` & `mypy_boto3_datasync-1.34.91/mypy_boto3_datasync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-datasync
-Version: 1.34.37
-Summary: Type annotations for boto3.DataSync 1.34.37 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.91
+Summary: Type annotations for boto3.DataSync 1.34.91 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datasync.svg?color=blue)](https://pypi.org/project/mypy-boto3-datasync)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-datasync)](https://pepy.tech/project/mypy-boto3-datasync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataSync 1.34.37](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
+[boto3.DataSync 1.34.91](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#DataSync)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-datasync docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datasync/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-datasync-1.34.37/mypy_boto3_datasync.egg-info/SOURCES.txt` & `mypy_boto3_datasync-1.34.91/mypy_boto3_datasync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datasync-1.34.37/setup.py` & `mypy_boto3_datasync-1.34.91/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-datasync",
-    version="1.34.37",
+    version="1.34.91",
     packages=["mypy_boto3_datasync"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.DataSync 1.34.37 service generated with mypy-boto3-builder 7.23.1",
+    description="Type annotations for boto3.DataSync 1.34.91 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

