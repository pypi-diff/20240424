# Comparing `tmp/cdk8s-awscdk-resolver-0.0.87.tar.gz` & `tmp/cdk8s-awscdk-resolver-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-awscdk-resolver-0.0.87.tar", last modified: Wed Apr 24 13:08:32 2024, max compression
+gzip compressed data, was "cdk8s-awscdk-resolver-0.0.9.tar", last modified: Mon Oct  9 12:16:32 2023, max compression
```

## Comparing `cdk8s-awscdk-resolver-0.0.87.tar` & `cdk8s-awscdk-resolver-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:08:32.267194 cdk8s-awscdk-resolver-0.0.87/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-24 13:08:20.000000 cdk8s-awscdk-resolver-0.0.87/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-24 13:08:20.000000 cdk8s-awscdk-resolver-0.0.87/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-24 13:08:32.267194 cdk8s-awscdk-resolver-0.0.87/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-24 13:08:20.000000 cdk8s-awscdk-resolver-0.0.87/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-24 13:08:20.000000 cdk8s-awscdk-resolver-0.0.87/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:08:32.267194 cdk8s-awscdk-resolver-0.0.87/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-24 13:08:20.000000 cdk8s-awscdk-resolver-0.0.87/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:08:32.263194 cdk8s-awscdk-resolver-0.0.87/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:08:32.263194 cdk8s-awscdk-resolver-0.0.87/src/cdk8s_awscdk_resolver/
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-04-24 13:08:20.000000 cdk8s-awscdk-resolver-0.0.87/src/cdk8s_awscdk_resolver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:08:32.267194 cdk8s-awscdk-resolver-0.0.87/src/cdk8s_awscdk_resolver/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-24 13:08:20.000000 cdk8s-awscdk-resolver-0.0.87/src/cdk8s_awscdk_resolver/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   979066 2024-04-24 13:08:20.000000 cdk8s-awscdk-resolver-0.0.87/src/cdk8s_awscdk_resolver/_jsii/awscdk-resolver@0.0.87.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:08:20.000000 cdk8s-awscdk-resolver-0.0.87/src/cdk8s_awscdk_resolver/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:08:32.267194 cdk8s-awscdk-resolver-0.0.87/src/cdk8s_awscdk_resolver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-04-24 13:08:32.000000 cdk8s-awscdk-resolver-0.0.87/src/cdk8s_awscdk_resolver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-24 13:08:32.000000 cdk8s-awscdk-resolver-0.0.87/src/cdk8s_awscdk_resolver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:08:32.000000 cdk8s-awscdk-resolver-0.0.87/src/cdk8s_awscdk_resolver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-24 13:08:32.000000 cdk8s-awscdk-resolver-0.0.87/src/cdk8s_awscdk_resolver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 13:08:32.000000 cdk8s-awscdk-resolver-0.0.87/src/cdk8s_awscdk_resolver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 12:16:32.902466 cdk8s-awscdk-resolver-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2023-10-09 12:16:18.000000 cdk8s-awscdk-resolver-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-10-09 12:16:18.000000 cdk8s-awscdk-resolver-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2023-10-09 12:16:32.902466 cdk8s-awscdk-resolver-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2023-10-09 12:16:18.000000 cdk8s-awscdk-resolver-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2023-10-09 12:16:18.000000 cdk8s-awscdk-resolver-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-09 12:16:32.902466 cdk8s-awscdk-resolver-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2023-10-09 12:16:18.000000 cdk8s-awscdk-resolver-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 12:16:32.898466 cdk8s-awscdk-resolver-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 12:16:32.898466 cdk8s-awscdk-resolver-0.0.9/src/cdk8s_awscdk_resolver/
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2023-10-09 12:16:18.000000 cdk8s-awscdk-resolver-0.0.9/src/cdk8s_awscdk_resolver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 12:16:32.898466 cdk8s-awscdk-resolver-0.0.9/src/cdk8s_awscdk_resolver/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2023-10-09 12:16:18.000000 cdk8s-awscdk-resolver-0.0.9/src/cdk8s_awscdk_resolver/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   804432 2023-10-09 12:16:18.000000 cdk8s-awscdk-resolver-0.0.9/src/cdk8s_awscdk_resolver/_jsii/awscdk-resolver@0.0.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-09 12:16:18.000000 cdk8s-awscdk-resolver-0.0.9/src/cdk8s_awscdk_resolver/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 12:16:32.898466 cdk8s-awscdk-resolver-0.0.9/src/cdk8s_awscdk_resolver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2023-10-09 12:16:32.000000 cdk8s-awscdk-resolver-0.0.9/src/cdk8s_awscdk_resolver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2023-10-09 12:16:32.000000 cdk8s-awscdk-resolver-0.0.9/src/cdk8s_awscdk_resolver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-09 12:16:32.000000 cdk8s-awscdk-resolver-0.0.9/src/cdk8s_awscdk_resolver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2023-10-09 12:16:32.000000 cdk8s-awscdk-resolver-0.0.9/src/cdk8s_awscdk_resolver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-09 12:16:32.000000 cdk8s-awscdk-resolver-0.0.9/src/cdk8s_awscdk_resolver.egg-info/top_level.txt
```

### Comparing `cdk8s-awscdk-resolver-0.0.87/LICENSE` & `cdk8s-awscdk-resolver-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-awscdk-resolver-0.0.87/PKG-INFO` & `cdk8s-awscdk-resolver-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: cdk8s-awscdk-resolver
-Version: 0.0.87
+Version: 0.0.9
 Summary: @cdk8s/awscdk-resolver
 Home-page: https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
-Requires-Python: ~=3.8
+Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AWS CDK Resolver
 
 The `AwsCdkResolver` is able to resolve any [`CfnOutput`](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.CfnOutput.html)
 defined by your AWS CDK application. In this example, we create an S3 `Bucket` with the AWS CDK, and pass its (deploy time generated)
```

### Comparing `cdk8s-awscdk-resolver-0.0.87/README.md` & `cdk8s-awscdk-resolver-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-awscdk-resolver-0.0.87/setup.py` & `cdk8s-awscdk-resolver-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-awscdk-resolver",
-    "version": "0.0.87",
+    "version": "0.0.9",
     "description": "@cdk8s/awscdk-resolver",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,34 +22,35 @@
     },
     "packages": [
         "cdk8s_awscdk_resolver",
         "cdk8s_awscdk_resolver._jsii"
     ],
     "package_data": {
         "cdk8s_awscdk_resolver._jsii": [
-            "awscdk-resolver@0.0.87.jsii.tgz"
+            "awscdk-resolver@0.0.9.jsii.tgz"
         ],
         "cdk8s_awscdk_resolver": [
             "py.typed"
         ]
     },
-    "python_requires": "~=3.8",
+    "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.106.1, <3.0.0",
-        "cdk8s>=2.68.3, <3.0.0",
+        "aws-cdk-lib>=2.100.0, <3.0.0",
+        "cdk8s>=2.66.8, <3.0.0",
         "constructs>=10.3.0, <11.0.0",
-        "jsii>=1.97.0, <2.0.0",
+        "jsii>=1.90.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved"
```

### Comparing `cdk8s-awscdk-resolver-0.0.87/src/cdk8s_awscdk_resolver/__init__.py` & `cdk8s-awscdk-resolver-0.0.9/src/cdk8s_awscdk_resolver/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -144,17 +144,14 @@
     }
  }]
 });
 
 k8sApp.synth();
 ```
 '''
-from pkgutil import extend_path
-__path__ = extend_path(__path__, __name__)
-
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
```

### Comparing `cdk8s-awscdk-resolver-0.0.87/src/cdk8s_awscdk_resolver.egg-info/PKG-INFO` & `cdk8s-awscdk-resolver-0.0.9/src/cdk8s_awscdk_resolver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: cdk8s-awscdk-resolver
-Version: 0.0.87
+Version: 0.0.9
 Summary: @cdk8s/awscdk-resolver
 Home-page: https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
-Requires-Python: ~=3.8
+Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AWS CDK Resolver
 
 The `AwsCdkResolver` is able to resolve any [`CfnOutput`](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.CfnOutput.html)
 defined by your AWS CDK application. In this example, we create an S3 `Bucket` with the AWS CDK, and pass its (deploy time generated)
```

