# Comparing `tmp/pulumi_awsx-2.7.0.tar.gz` & `tmp/pulumi_awsx-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_awsx-2.7.0.tar", last modified: Thu Apr 11 14:33:32 2024, max compression
+gzip compressed data, was "pulumi_awsx-2.8.0.tar", last modified: Fri Apr 19 19:21:49 2024, max compression
```

## Comparing `pulumi_awsx-2.7.0.tar` & `pulumi_awsx-2.8.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:33:32.949266 pulumi_awsx-2.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-04-11 14:33:32.949266 pulumi_awsx-2.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:33:32.945266 pulumi_awsx-2.7.0/pulumi_awsx/
--rw-------   0 runner    (1001) docker     (127)     2193 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/__init__.py
--rw-------   0 runner    (1001) docker     (127)     8056 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:33:32.945266 pulumi_awsx-2.7.0/pulumi_awsx/awsx/
--rw-------   0 runner    (1001) docker     (127)      223 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/awsx/__init__.py
--rw-------   0 runner    (1001) docker     (127)    57488 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/awsx/_inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:33:32.945266 pulumi_awsx-2.7.0/pulumi_awsx/cloudtrail/
--rw-------   0 runner    (1001) docker     (127)      265 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/cloudtrail/__init__.py
--rw-------   0 runner    (1001) docker     (127)    23412 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/cloudtrail/trail.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:33:32.945266 pulumi_awsx-2.7.0/pulumi_awsx/ec2/
--rw-------   0 runner    (1001) docker     (127)      388 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/ec2/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1983 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/ec2/_enums.py
--rw-------   0 runner    (1001) docker     (127)    34412 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/ec2/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     3839 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/ec2/default_vpc.py
--rw-------   0 runner    (1001) docker     (127)     3454 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/ec2/get_default_vpc.py
--rw-------   0 runner    (1001) docker     (127)     4520 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/ec2/outputs.py
--rw-------   0 runner    (1001) docker     (127)    41221 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/ec2/vpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:33:32.949266 pulumi_awsx-2.7.0/pulumi_awsx/ecr/
--rw-------   0 runner    (1001) docker     (127)      336 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/ecr/__init__.py
--rw-------   0 runner    (1001) docker     (127)      834 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/ecr/_enums.py
--rw-------   0 runner    (1001) docker     (127)     7578 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/ecr/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    14415 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/ecr/image.py
--rw-------   0 runner    (1001) docker     (127)    14431 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/ecr/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:33:32.949266 pulumi_awsx-2.7.0/pulumi_awsx/ecs/
--rw-------   0 runner    (1001) docker     (127)      421 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/ecs/__init__.py
--rw-------   0 runner    (1001) docker     (127)      354 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/ecs/_enums.py
--rw-------   0 runner    (1001) docker     (127)    86174 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/ecs/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    46322 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/ecs/ec2_service.py
--rw-------   0 runner    (1001) docker     (127)    31286 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/ecs/ec2_task_definition.py
--rw-------   0 runner    (1001) docker     (127)    45038 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/ecs/fargate_service.py
--rw-------   0 runner    (1001) docker     (127)    30189 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/ecs/fargate_task_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:33:32.949266 pulumi_awsx-2.7.0/pulumi_awsx/lb/
--rw-------   0 runner    (1001) docker     (127)      384 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/lb/__init__.py
--rw-------   0 runner    (1001) docker     (127)    97738 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/lb/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    43234 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/lb/application_load_balancer.py
--rw-------   0 runner    (1001) docker     (127)    40347 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/lb/network_load_balancer.py
--rw-------   0 runner    (1001) docker     (127)    11113 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/lb/target_group_attachment.py
--rw-------   0 runner    (1001) docker     (127)     2719 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/provider.py
--rw-------   0 runner    (1001) docker     (127)       41 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pulumi_awsx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 14:33:32.949266 pulumi_awsx-2.7.0/pulumi_awsx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-04-11 14:33:32.000000 pulumi_awsx-2.7.0/pulumi_awsx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-11 14:33:32.000000 pulumi_awsx-2.7.0/pulumi_awsx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 14:33:32.000000 pulumi_awsx-2.7.0/pulumi_awsx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-11 14:33:32.000000 pulumi_awsx-2.7.0/pulumi_awsx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 14:33:32.000000 pulumi_awsx-2.7.0/pulumi_awsx.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      747 2024-04-11 14:33:26.000000 pulumi_awsx-2.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 14:33:32.949266 pulumi_awsx-2.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:21:49.699719 pulumi_awsx-2.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-04-19 19:21:49.699719 pulumi_awsx-2.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:21:49.691719 pulumi_awsx-2.8.0/pulumi_awsx/
+-rw-------   0 runner    (1001) docker     (127)     2193 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     9223 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:21:49.691719 pulumi_awsx-2.8.0/pulumi_awsx/awsx/
+-rw-------   0 runner    (1001) docker     (127)      223 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/awsx/__init__.py
+-rw-------   0 runner    (1001) docker     (127)    57488 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/awsx/_inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:21:49.691719 pulumi_awsx-2.8.0/pulumi_awsx/cloudtrail/
+-rw-------   0 runner    (1001) docker     (127)      265 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/cloudtrail/__init__.py
+-rw-------   0 runner    (1001) docker     (127)    23412 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/cloudtrail/trail.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:21:49.695719 pulumi_awsx-2.8.0/pulumi_awsx/ec2/
+-rw-------   0 runner    (1001) docker     (127)      388 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ec2/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1983 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ec2/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    34412 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ec2/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     3839 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ec2/default_vpc.py
+-rw-------   0 runner    (1001) docker     (127)     3454 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ec2/get_default_vpc.py
+-rw-------   0 runner    (1001) docker     (127)     4520 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ec2/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    41221 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ec2/vpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:21:49.695719 pulumi_awsx-2.8.0/pulumi_awsx/ecr/
+-rw-------   0 runner    (1001) docker     (127)      336 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ecr/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      834 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ecr/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     7578 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ecr/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    15525 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ecr/image.py
+-rw-------   0 runner    (1001) docker     (127)    14431 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ecr/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:21:49.695719 pulumi_awsx-2.8.0/pulumi_awsx/ecs/
+-rw-------   0 runner    (1001) docker     (127)      421 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ecs/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      354 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ecs/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    86174 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ecs/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    46322 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ecs/ec2_service.py
+-rw-------   0 runner    (1001) docker     (127)    31286 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ecs/ec2_task_definition.py
+-rw-------   0 runner    (1001) docker     (127)    45038 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ecs/fargate_service.py
+-rw-------   0 runner    (1001) docker     (127)    30189 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ecs/fargate_task_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:21:49.695719 pulumi_awsx-2.8.0/pulumi_awsx/lb/
+-rw-------   0 runner    (1001) docker     (127)      384 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/lb/__init__.py
+-rw-------   0 runner    (1001) docker     (127)    97738 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/lb/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    43234 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/lb/application_load_balancer.py
+-rw-------   0 runner    (1001) docker     (127)    40347 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/lb/network_load_balancer.py
+-rw-------   0 runner    (1001) docker     (127)    11113 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/lb/target_group_attachment.py
+-rw-------   0 runner    (1001) docker     (127)     2719 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/provider.py
+-rw-------   0 runner    (1001) docker     (127)       41 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:21:49.699719 pulumi_awsx-2.8.0/pulumi_awsx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-04-19 19:21:49.000000 pulumi_awsx-2.8.0/pulumi_awsx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-19 19:21:49.000000 pulumi_awsx-2.8.0/pulumi_awsx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:21:49.000000 pulumi_awsx-2.8.0/pulumi_awsx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-19 19:21:49.000000 pulumi_awsx-2.8.0/pulumi_awsx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 19:21:49.000000 pulumi_awsx-2.8.0/pulumi_awsx.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      747 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:21:49.699719 pulumi_awsx-2.8.0/setup.cfg
```

### Comparing `pulumi_awsx-2.7.0/PKG-INFO` & `pulumi_awsx-2.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pulumi_awsx
-Version: 2.7.0
+Version: 2.8.0
 Summary: Pulumi Amazon Web Services (AWS) AWSX Components.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-awsx
 Keywords: pulumi,aws,awsx,kind/component,category/cloud
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
 Requires-Dist: pulumi<4.0.0,>=3.91.1
 Requires-Dist: pulumi-aws<7.0.0,>=6.0.4
 Requires-Dist: pulumi-docker<5.0.0,>=4.5.1
 Requires-Dist: semver>=2.8.1
```

### Comparing `pulumi_awsx-2.7.0/README.md` & `pulumi_awsx-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.7.0/pulumi_awsx/__init__.py` & `pulumi_awsx-2.8.0/pulumi_awsx/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.7.0/pulumi_awsx/_utilities.py` & `pulumi_awsx-2.8.0/pulumi_awsx/_utilities.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # coding=utf-8
 # *** WARNING: this file was generated by pulumi-gen-awsx. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 
+import asyncio
+import importlib.metadata
 import importlib.util
 import inspect
 import json
 import os
-import pkg_resources
 import sys
 import typing
 
 import pulumi
 import pulumi.runtime
+from pulumi.runtime.sync_await import _sync_await
 
 from semver import VersionInfo as SemverVersion
 from parver import Version as PEP440Version
 
 
 def get_env(*args):
     for v in args:
@@ -66,15 +68,15 @@
     # pkg_resources uses setuptools to inspect the set of installed packages. We use it here to ask
     # for the currently installed version of the root package (i.e. us) and get its version.
 
     # Unfortunately, PEP440 and semver differ slightly in incompatible ways. The Pulumi engine expects
     # to receive a valid semver string when receiving requests from the language host, so it's our
     # responsibility as the library to convert our own PEP440 version into a valid semver string.
 
-    pep440_version_string = pkg_resources.require(root_package)[0].version
+    pep440_version_string = importlib.metadata.version(root_package)
     pep440_version = PEP440Version.parse(pep440_version_string)
     (major, minor, patch) = pep440_version.release
     prerelease = None
     if pep440_version.pre_tag == 'a':
         prerelease = f"alpha.{pep440_version.pre}"
     elif pep440_version.pre_tag == 'b':
         prerelease = f"beta.{pep440_version.pre}"
@@ -242,9 +244,48 @@
             'kwargs': bound_args.kwargs
         }).apply(lambda resolved_args: func(*resolved_args['args'],
                                             opts=opts,
                                             **resolved_args['kwargs']))
 
     return (lambda _: lifted_func)
 
+
+def call_plain(
+    tok: str,
+    props: pulumi.Inputs,
+    res: typing.Optional[pulumi.Resource] = None,
+    typ: typing.Optional[type] = None,
+) -> typing.Any:
+    """
+    Wraps pulumi.runtime.plain to force the output and return it plainly.
+    """
+
+    output = pulumi.runtime.call(tok, props, res, typ)
+
+    # Ingoring deps silently. They are typically non-empty, r.f() calls include r as a dependency.
+    result, known, secret, _ = _sync_await(asyncio.ensure_future(_await_output(output)))
+
+    problem = None
+    if not known:
+        problem = ' an unknown value'
+    elif secret:
+        problem = ' a secret value'
+
+    if problem:
+        raise AssertionError(
+            f"Plain resource method '{tok}' incorrectly returned {problem}. "
+            + "This is an error in the provider, please report this to the provider developer."
+        )
+
+    return result
+
+
+async def _await_output(o: pulumi.Output[typing.Any]) -> typing.Tuple[object, bool, bool, set]:
+    return (
+        await o._future,
+        await o._is_known,
+        await o._is_secret,
+        await o._resources,
+    )
+
 def get_plugin_download_url():
 	return None
```

### Comparing `pulumi_awsx-2.7.0/pulumi_awsx/awsx/_inputs.py` & `pulumi_awsx-2.8.0/pulumi_awsx/awsx/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.7.0/pulumi_awsx/cloudtrail/trail.py` & `pulumi_awsx-2.8.0/pulumi_awsx/cloudtrail/trail.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.7.0/pulumi_awsx/ec2/_enums.py` & `pulumi_awsx-2.8.0/pulumi_awsx/ec2/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.7.0/pulumi_awsx/ec2/_inputs.py` & `pulumi_awsx-2.8.0/pulumi_awsx/ec2/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.7.0/pulumi_awsx/ec2/default_vpc.py` & `pulumi_awsx-2.8.0/pulumi_awsx/ec2/default_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.7.0/pulumi_awsx/ec2/get_default_vpc.py` & `pulumi_awsx-2.8.0/pulumi_awsx/ec2/get_default_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.7.0/pulumi_awsx/ec2/outputs.py` & `pulumi_awsx-2.8.0/pulumi_awsx/ec2/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.7.0/pulumi_awsx/ec2/vpc.py` & `pulumi_awsx-2.8.0/pulumi_awsx/ec2/vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.7.0/pulumi_awsx/ecr/_enums.py` & `pulumi_awsx-2.8.0/pulumi_awsx/ecr/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.7.0/pulumi_awsx/ecr/_inputs.py` & `pulumi_awsx-2.8.0/pulumi_awsx/ecr/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.7.0/pulumi_awsx/ecr/image.py` & `pulumi_awsx-2.8.0/pulumi_awsx/ecr/image.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,26 +17,28 @@
     def __init__(__self__, *,
                  repository_url: pulumi.Input[str],
                  args: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  builder_version: Optional['BuilderVersion'] = None,
                  cache_from: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  context: Optional[pulumi.Input[str]] = None,
                  dockerfile: Optional[pulumi.Input[str]] = None,
+                 image_name: Optional[pulumi.Input[str]] = None,
                  image_tag: Optional[pulumi.Input[str]] = None,
                  platform: Optional[pulumi.Input[str]] = None,
                  registry_id: Optional[pulumi.Input[str]] = None,
                  target: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Image resource.
         :param pulumi.Input[str] repository_url: Url of the repository
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] args: An optional map of named build-time argument variables to set during the Docker build.  This flag allows you to pass built-time variables that can be accessed like environment variables inside the `RUN` instruction.
         :param 'BuilderVersion' builder_version: The version of the Docker builder.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] cache_from: Images to consider as cache sources
         :param pulumi.Input[str] context: Path to a directory to use for the Docker build context, usually the directory in which the Dockerfile resides (although dockerfile may be used to choose a custom location independent of this choice). If not specified, the context defaults to the current working directory; if a relative path is used, it is relative to the current working directory that Pulumi is evaluating.
         :param pulumi.Input[str] dockerfile: dockerfile may be used to override the default Dockerfile name and/or location.  By default, it is assumed to be a file named Dockerfile in the root of the build context.
+        :param pulumi.Input[str] image_name: Custom name for the underlying Docker image resource. If omitted, the image tag assigned by the provider will be used
         :param pulumi.Input[str] image_tag: Custom image tag for the resulting docker image. If omitted a random string will be used
         :param pulumi.Input[str] platform: The architecture of the platform you want to build this image for, e.g. `linux/arm64`.
         :param pulumi.Input[str] registry_id: ID of the ECR registry in which to store the image.  If not provided, this will be inferred from the repository URL)
         :param pulumi.Input[str] target: The target of the dockerfile to build
         """
         pulumi.set(__self__, "repository_url", repository_url)
         if args is not None:
@@ -45,14 +47,16 @@
             pulumi.set(__self__, "builder_version", builder_version)
         if cache_from is not None:
             pulumi.set(__self__, "cache_from", cache_from)
         if context is not None:
             pulumi.set(__self__, "context", context)
         if dockerfile is not None:
             pulumi.set(__self__, "dockerfile", dockerfile)
+        if image_name is not None:
+            pulumi.set(__self__, "image_name", image_name)
         if image_tag is not None:
             pulumi.set(__self__, "image_tag", image_tag)
         if platform is not None:
             pulumi.set(__self__, "platform", platform)
         if registry_id is not None:
             pulumi.set(__self__, "registry_id", registry_id)
         if target is not None:
@@ -127,14 +131,26 @@
         return pulumi.get(self, "dockerfile")
 
     @dockerfile.setter
     def dockerfile(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "dockerfile", value)
 
     @property
+    @pulumi.getter(name="imageName")
+    def image_name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Custom name for the underlying Docker image resource. If omitted, the image tag assigned by the provider will be used
+        """
+        return pulumi.get(self, "image_name")
+
+    @image_name.setter
+    def image_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "image_name", value)
+
+    @property
     @pulumi.getter(name="imageTag")
     def image_tag(self) -> Optional[pulumi.Input[str]]:
         """
         Custom image tag for the resulting docker image. If omitted a random string will be used
         """
         return pulumi.get(self, "image_tag")
 
@@ -185,14 +201,15 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  args: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  builder_version: Optional['BuilderVersion'] = None,
                  cache_from: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  context: Optional[pulumi.Input[str]] = None,
                  dockerfile: Optional[pulumi.Input[str]] = None,
+                 image_name: Optional[pulumi.Input[str]] = None,
                  image_tag: Optional[pulumi.Input[str]] = None,
                  platform: Optional[pulumi.Input[str]] = None,
                  registry_id: Optional[pulumi.Input[str]] = None,
                  repository_url: Optional[pulumi.Input[str]] = None,
                  target: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
@@ -201,14 +218,15 @@
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] args: An optional map of named build-time argument variables to set during the Docker build.  This flag allows you to pass built-time variables that can be accessed like environment variables inside the `RUN` instruction.
         :param 'BuilderVersion' builder_version: The version of the Docker builder.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] cache_from: Images to consider as cache sources
         :param pulumi.Input[str] context: Path to a directory to use for the Docker build context, usually the directory in which the Dockerfile resides (although dockerfile may be used to choose a custom location independent of this choice). If not specified, the context defaults to the current working directory; if a relative path is used, it is relative to the current working directory that Pulumi is evaluating.
         :param pulumi.Input[str] dockerfile: dockerfile may be used to override the default Dockerfile name and/or location.  By default, it is assumed to be a file named Dockerfile in the root of the build context.
+        :param pulumi.Input[str] image_name: Custom name for the underlying Docker image resource. If omitted, the image tag assigned by the provider will be used
         :param pulumi.Input[str] image_tag: Custom image tag for the resulting docker image. If omitted a random string will be used
         :param pulumi.Input[str] platform: The architecture of the platform you want to build this image for, e.g. `linux/arm64`.
         :param pulumi.Input[str] registry_id: ID of the ECR registry in which to store the image.  If not provided, this will be inferred from the repository URL)
         :param pulumi.Input[str] repository_url: Url of the repository
         :param pulumi.Input[str] target: The target of the dockerfile to build
         """
         ...
@@ -236,14 +254,15 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  args: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  builder_version: Optional['BuilderVersion'] = None,
                  cache_from: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  context: Optional[pulumi.Input[str]] = None,
                  dockerfile: Optional[pulumi.Input[str]] = None,
+                 image_name: Optional[pulumi.Input[str]] = None,
                  image_tag: Optional[pulumi.Input[str]] = None,
                  platform: Optional[pulumi.Input[str]] = None,
                  registry_id: Optional[pulumi.Input[str]] = None,
                  repository_url: Optional[pulumi.Input[str]] = None,
                  target: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
@@ -257,14 +276,15 @@
             __props__ = ImageArgs.__new__(ImageArgs)
 
             __props__.__dict__["args"] = args
             __props__.__dict__["builder_version"] = builder_version
             __props__.__dict__["cache_from"] = cache_from
             __props__.__dict__["context"] = context
             __props__.__dict__["dockerfile"] = dockerfile
+            __props__.__dict__["image_name"] = image_name
             __props__.__dict__["image_tag"] = image_tag
             __props__.__dict__["platform"] = platform
             __props__.__dict__["registry_id"] = registry_id
             if repository_url is None and not opts.urn:
                 raise TypeError("Missing required property 'repository_url'")
             __props__.__dict__["repository_url"] = repository_url
             __props__.__dict__["target"] = target
```

### Comparing `pulumi_awsx-2.7.0/pulumi_awsx/ecr/repository.py` & `pulumi_awsx-2.8.0/pulumi_awsx/ecr/repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.7.0/pulumi_awsx/ecs/_inputs.py` & `pulumi_awsx-2.8.0/pulumi_awsx/ecs/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.7.0/pulumi_awsx/ecs/ec2_service.py` & `pulumi_awsx-2.8.0/pulumi_awsx/ecs/ec2_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.7.0/pulumi_awsx/ecs/ec2_task_definition.py` & `pulumi_awsx-2.8.0/pulumi_awsx/ecs/ec2_task_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.7.0/pulumi_awsx/ecs/fargate_service.py` & `pulumi_awsx-2.8.0/pulumi_awsx/ecs/fargate_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.7.0/pulumi_awsx/ecs/fargate_task_definition.py` & `pulumi_awsx-2.8.0/pulumi_awsx/ecs/fargate_task_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.7.0/pulumi_awsx/lb/_inputs.py` & `pulumi_awsx-2.8.0/pulumi_awsx/lb/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.7.0/pulumi_awsx/lb/application_load_balancer.py` & `pulumi_awsx-2.8.0/pulumi_awsx/lb/application_load_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.7.0/pulumi_awsx/lb/network_load_balancer.py` & `pulumi_awsx-2.8.0/pulumi_awsx/lb/network_load_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.7.0/pulumi_awsx/lb/target_group_attachment.py` & `pulumi_awsx-2.8.0/pulumi_awsx/lb/target_group_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.7.0/pulumi_awsx/provider.py` & `pulumi_awsx-2.8.0/pulumi_awsx/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.7.0/pulumi_awsx.egg-info/PKG-INFO` & `pulumi_awsx-2.8.0/pulumi_awsx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pulumi_awsx
-Version: 2.7.0
+Version: 2.8.0
 Summary: Pulumi Amazon Web Services (AWS) AWSX Components.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-awsx
 Keywords: pulumi,aws,awsx,kind/component,category/cloud
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
 Requires-Dist: pulumi<4.0.0,>=3.91.1
 Requires-Dist: pulumi-aws<7.0.0,>=6.0.4
 Requires-Dist: pulumi-docker<5.0.0,>=4.5.1
 Requires-Dist: semver>=2.8.1
```

### Comparing `pulumi_awsx-2.7.0/pulumi_awsx.egg-info/SOURCES.txt` & `pulumi_awsx-2.8.0/pulumi_awsx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.7.0/pyproject.toml` & `pulumi_awsx-2.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_awsx"
   description = "Pulumi Amazon Web Services (AWS) AWSX Components."
   dependencies = ["parver>=0.2.1", "pulumi>=3.91.1,<4.0.0", "pulumi-aws>=6.0.4,<7.0.0", "pulumi-docker>=4.5.1,<5.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "aws", "awsx", "kind/component", "category/cloud"]
   readme = "README.md"
-  requires-python = ">=3.7"
-  version = "2.7.0"
+  requires-python = ">=3.8"
+  version = "2.8.0"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.com"
     Repository = "https://github.com/pulumi/pulumi-awsx"
 
 [build-system]
```

