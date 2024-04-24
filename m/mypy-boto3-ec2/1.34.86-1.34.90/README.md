# Comparing `tmp/mypy_boto3_ec2-1.34.86.tar.gz` & `tmp/mypy_boto3_ec2-1.34.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_ec2-1.34.86.tar", last modified: Wed Apr 17 19:47:43 2024, max compression
+gzip compressed data, was "mypy_boto3_ec2-1.34.90.tar", last modified: Tue Apr 23 19:34:20 2024, max compression
```

## Comparing `mypy_boto3_ec2-1.34.86.tar` & `mypy_boto3_ec2-1.34.90.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:47:43.873910 mypy_boto3_ec2-1.34.86/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-17 19:46:59.000000 mypy_boto3_ec2-1.34.86/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    50489 2024-04-17 19:47:43.873910 mypy_boto3_ec2-1.34.86/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    48950 2024-04-17 19:46:59.000000 mypy_boto3_ec2-1.34.86/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:47:43.869910 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/
--rw-r--r--   0 runner    (1001) docker     (127)    47454 2024-04-17 19:46:59.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47454 2024-04-17 19:46:59.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-17 19:46:59.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   542214 2024-04-17 19:47:05.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   542211 2024-04-17 19:47:02.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    96841 2024-04-17 19:47:12.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    96841 2024-04-17 19:47:12.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   187422 2024-04-17 19:47:10.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)   187279 2024-04-17 19:47:10.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:46:59.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   271947 2024-04-17 19:47:08.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)   271869 2024-04-17 19:47:07.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   869264 2024-04-17 19:47:29.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   869264 2024-04-17 19:47:23.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-17 19:46:59.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    39773 2024-04-17 19:47:11.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    39737 2024-04-17 19:47:11.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:47:43.873910 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    50489 2024-04-17 19:47:43.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-17 19:47:43.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:47:43.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:47:43.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-17 19:47:43.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 19:47:43.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 19:47:43.873910 mypy_boto3_ec2-1.34.86/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-17 19:46:59.000000 mypy_boto3_ec2-1.34.86/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:20.992573 mypy_boto3_ec2-1.34.90/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-23 19:33:26.000000 mypy_boto3_ec2-1.34.90/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    50489 2024-04-23 19:34:20.992573 mypy_boto3_ec2-1.34.90/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    48950 2024-04-23 19:33:26.000000 mypy_boto3_ec2-1.34.90/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:20.992573 mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/
+-rw-r--r--   0 runner    (1001) docker     (127)    47454 2024-04-23 19:33:26.000000 mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47454 2024-04-23 19:33:26.000000 mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-23 19:33:26.000000 mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   543462 2024-04-23 19:33:32.000000 mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   543459 2024-04-23 19:33:29.000000 mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    96896 2024-04-23 19:33:38.000000 mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96896 2024-04-23 19:33:38.000000 mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   187422 2024-04-23 19:33:36.000000 mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)   187279 2024-04-23 19:33:35.000000 mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:33:26.000000 mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   272010 2024-04-23 19:33:35.000000 mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)   271932 2024-04-23 19:33:33.000000 mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   870550 2024-04-23 19:33:55.000000 mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   870550 2024-04-23 19:33:49.000000 mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 19:33:26.000000 mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39773 2024-04-23 19:33:37.000000 mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39737 2024-04-23 19:33:36.000000 mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:20.992573 mypy_boto3_ec2-1.34.90/mypy_boto3_ec2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    50489 2024-04-23 19:34:20.000000 mypy_boto3_ec2-1.34.90/mypy_boto3_ec2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-23 19:34:20.000000 mypy_boto3_ec2-1.34.90/mypy_boto3_ec2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:34:20.000000 mypy_boto3_ec2-1.34.90/mypy_boto3_ec2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:34:20.000000 mypy_boto3_ec2-1.34.90/mypy_boto3_ec2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 19:34:20.000000 mypy_boto3_ec2-1.34.90/mypy_boto3_ec2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-23 19:34:20.000000 mypy_boto3_ec2-1.34.90/mypy_boto3_ec2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:34:20.992573 mypy_boto3_ec2-1.34.90/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-23 19:33:24.000000 mypy_boto3_ec2-1.34.90/setup.py
```

### Comparing `mypy_boto3_ec2-1.34.86/LICENSE` & `mypy_boto3_ec2-1.34.90/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_ec2-1.34.86/PKG-INFO` & `mypy_boto3_ec2-1.34.90/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ec2
-Version: 1.34.86
-Summary: Type annotations for boto3.EC2 1.34.86 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.90
+Summary: Type annotations for boto3.EC2 1.34.90 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ec2.svg?color=blue)](https://pypi.org/project/mypy-boto3-ec2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ec2)](https://pepy.tech/project/mypy-boto3-ec2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EC2 1.34.86](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
+[boto3.EC2 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_ec2-1.34.86/README.md` & `mypy_boto3_ec2-1.34.90/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ec2.svg?color=blue)](https://pypi.org/project/mypy-boto3-ec2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ec2)](https://pepy.tech/project/mypy-boto3-ec2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EC2 1.34.86](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
+[boto3.EC2 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/__init__.py` & `mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/__init__.pyi` & `mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/__main__.py` & `mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EC2 1.34.86\n"
-        "Version:         1.34.86\n"
+        "Type annotations for boto3.EC2 1.34.90\n"
+        "Version:         1.34.90\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.86")
+    print("1.34.90")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/client.py` & `mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -624,14 +624,15 @@
     DisableAddressTransferResultTypeDef,
     DisableAwsNetworkPerformanceMetricSubscriptionResultTypeDef,
     DisableEbsEncryptionByDefaultResultTypeDef,
     DisableFastLaunchResultTypeDef,
     DisableFastSnapshotRestoresResultTypeDef,
     DisableImageBlockPublicAccessResultTypeDef,
     DisableImageDeprecationResultTypeDef,
+    DisableImageDeregistrationProtectionResultTypeDef,
     DisableImageResultTypeDef,
     DisableIpamOrganizationAdminAccountResultTypeDef,
     DisableSerialConsoleAccessResultTypeDef,
     DisableSnapshotBlockPublicAccessResultTypeDef,
     DisableTransitGatewayRouteTablePropagationResultTypeDef,
     DisableVpcClassicLinkDnsSupportResultTypeDef,
     DisableVpcClassicLinkResultTypeDef,
@@ -658,14 +659,15 @@
     EnableAddressTransferResultTypeDef,
     EnableAwsNetworkPerformanceMetricSubscriptionResultTypeDef,
     EnableEbsEncryptionByDefaultResultTypeDef,
     EnableFastLaunchResultTypeDef,
     EnableFastSnapshotRestoresResultTypeDef,
     EnableImageBlockPublicAccessResultTypeDef,
     EnableImageDeprecationResultTypeDef,
+    EnableImageDeregistrationProtectionResultTypeDef,
     EnableImageResultTypeDef,
     EnableIpamOrganizationAdminAccountResultTypeDef,
     EnableReachabilityAnalyzerOrganizationSharingResultTypeDef,
     EnableSerialConsoleAccessResultTypeDef,
     EnableSnapshotBlockPublicAccessResultTypeDef,
     EnableTransitGatewayRouteTablePropagationResultTypeDef,
     EnableVpcClassicLinkDnsSupportResultTypeDef,
@@ -6690,14 +6692,24 @@
         """
         Cancels the deprecation of the specified AMI.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.disable_image_deprecation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#disable_image_deprecation)
         """
 
+    def disable_image_deregistration_protection(
+        self, *, ImageId: str, DryRun: bool = ...
+    ) -> DisableImageDeregistrationProtectionResultTypeDef:
+        """
+        Disables deregistration protection for an AMI.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.disable_image_deregistration_protection)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#disable_image_deregistration_protection)
+        """
+
     def disable_ipam_organization_admin_account(
         self, *, DelegatedAdminAccountId: str, DryRun: bool = ...
     ) -> DisableIpamOrganizationAdminAccountResultTypeDef:
         """
         Disable the IPAM account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.disable_ipam_organization_admin_account)
@@ -7049,14 +7061,24 @@
         """
         Enables deprecation of the specified AMI at the specified date and time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.enable_image_deprecation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#enable_image_deprecation)
         """
 
+    def enable_image_deregistration_protection(
+        self, *, ImageId: str, WithCooldown: bool = ..., DryRun: bool = ...
+    ) -> EnableImageDeregistrationProtectionResultTypeDef:
+        """
+        Enables deregistration protection for an AMI.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.enable_image_deregistration_protection)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#enable_image_deregistration_protection)
+        """
+
     def enable_ipam_organization_admin_account(
         self, *, DelegatedAdminAccountId: str, DryRun: bool = ...
     ) -> EnableIpamOrganizationAdminAccountResultTypeDef:
         """
         Enable an Organizations member account as the IPAM admin account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.enable_ipam_organization_admin_account)
```

### Comparing `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/client.pyi` & `mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -624,14 +624,15 @@
     DisableAddressTransferResultTypeDef,
     DisableAwsNetworkPerformanceMetricSubscriptionResultTypeDef,
     DisableEbsEncryptionByDefaultResultTypeDef,
     DisableFastLaunchResultTypeDef,
     DisableFastSnapshotRestoresResultTypeDef,
     DisableImageBlockPublicAccessResultTypeDef,
     DisableImageDeprecationResultTypeDef,
+    DisableImageDeregistrationProtectionResultTypeDef,
     DisableImageResultTypeDef,
     DisableIpamOrganizationAdminAccountResultTypeDef,
     DisableSerialConsoleAccessResultTypeDef,
     DisableSnapshotBlockPublicAccessResultTypeDef,
     DisableTransitGatewayRouteTablePropagationResultTypeDef,
     DisableVpcClassicLinkDnsSupportResultTypeDef,
     DisableVpcClassicLinkResultTypeDef,
@@ -658,14 +659,15 @@
     EnableAddressTransferResultTypeDef,
     EnableAwsNetworkPerformanceMetricSubscriptionResultTypeDef,
     EnableEbsEncryptionByDefaultResultTypeDef,
     EnableFastLaunchResultTypeDef,
     EnableFastSnapshotRestoresResultTypeDef,
     EnableImageBlockPublicAccessResultTypeDef,
     EnableImageDeprecationResultTypeDef,
+    EnableImageDeregistrationProtectionResultTypeDef,
     EnableImageResultTypeDef,
     EnableIpamOrganizationAdminAccountResultTypeDef,
     EnableReachabilityAnalyzerOrganizationSharingResultTypeDef,
     EnableSerialConsoleAccessResultTypeDef,
     EnableSnapshotBlockPublicAccessResultTypeDef,
     EnableTransitGatewayRouteTablePropagationResultTypeDef,
     EnableVpcClassicLinkDnsSupportResultTypeDef,
@@ -6687,14 +6689,24 @@
         """
         Cancels the deprecation of the specified AMI.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.disable_image_deprecation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#disable_image_deprecation)
         """
 
+    def disable_image_deregistration_protection(
+        self, *, ImageId: str, DryRun: bool = ...
+    ) -> DisableImageDeregistrationProtectionResultTypeDef:
+        """
+        Disables deregistration protection for an AMI.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.disable_image_deregistration_protection)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#disable_image_deregistration_protection)
+        """
+
     def disable_ipam_organization_admin_account(
         self, *, DelegatedAdminAccountId: str, DryRun: bool = ...
     ) -> DisableIpamOrganizationAdminAccountResultTypeDef:
         """
         Disable the IPAM account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.disable_ipam_organization_admin_account)
@@ -7046,14 +7058,24 @@
         """
         Enables deprecation of the specified AMI at the specified date and time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.enable_image_deprecation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#enable_image_deprecation)
         """
 
+    def enable_image_deregistration_protection(
+        self, *, ImageId: str, WithCooldown: bool = ..., DryRun: bool = ...
+    ) -> EnableImageDeregistrationProtectionResultTypeDef:
+        """
+        Enables deregistration protection for an AMI.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.enable_image_deregistration_protection)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#enable_image_deregistration_protection)
+        """
+
     def enable_ipam_organization_admin_account(
         self, *, DelegatedAdminAccountId: str, DryRun: bool = ...
     ) -> EnableIpamOrganizationAdminAccountResultTypeDef:
         """
         Enable an Organizations member account as the IPAM admin account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.enable_ipam_organization_admin_account)
```

### Comparing `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/literals.py` & `mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1000,14 +1000,15 @@
 IamInstanceProfileAssociationStateType = Literal[
     "associated", "associating", "disassociated", "disassociating"
 ]
 Igmpv2SupportValueType = Literal["disable", "enable"]
 ImageAttributeNameType = Literal[
     "blockDeviceMapping",
     "bootMode",
+    "deregistrationProtection",
     "description",
     "imdsSupport",
     "kernel",
     "lastLaunchedTime",
     "launchPermission",
     "productCodes",
     "ramdisk",
@@ -2706,14 +2707,15 @@
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

### Comparing `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/literals.pyi` & `mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1000,14 +1000,15 @@
 IamInstanceProfileAssociationStateType = Literal[
     "associated", "associating", "disassociated", "disassociating"
 ]
 Igmpv2SupportValueType = Literal["disable", "enable"]
 ImageAttributeNameType = Literal[
     "blockDeviceMapping",
     "bootMode",
+    "deregistrationProtection",
     "description",
     "imdsSupport",
     "kernel",
     "lastLaunchedTime",
     "launchPermission",
     "productCodes",
     "ramdisk",
@@ -2706,14 +2707,15 @@
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

### Comparing `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/paginator.py` & `mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/paginator.pyi` & `mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/service_resource.py` & `mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/service_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -2361,14 +2361,16 @@
     tags: List[TagTypeDef]
     virtualization_type: VirtualizationTypeType
     boot_mode: BootModeValuesType
     tpm_support: Literal["v2.0"]
     deprecation_time: str
     imds_support: Literal["v2.0"]
     source_instance_id: str
+    deregistration_protection: str
+    last_launched_time: str
     id: str
     meta: "EC2ResourceMeta"
 
     def create_tags(self, *, Tags: Sequence[TagTypeDef], DryRun: bool = ...) -> None:
         """
         Adds or overwrites only the specified tags for the specified Amazon EC2
         resource or
```

### Comparing `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/service_resource.pyi` & `mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/service_resource.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2324,14 +2324,16 @@
     tags: List[TagTypeDef]
     virtualization_type: VirtualizationTypeType
     boot_mode: BootModeValuesType
     tpm_support: Literal["v2.0"]
     deprecation_time: str
     imds_support: Literal["v2.0"]
     source_instance_id: str
+    deregistration_protection: str
+    last_launched_time: str
     id: str
     meta: "EC2ResourceMeta"
 
     def create_tags(self, *, Tags: Sequence[TagTypeDef], DryRun: bool = ...) -> None:
         """
         Adds or overwrites only the specified tags for the specified Amazon EC2
         resource or
```

### Comparing `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/type_defs.py` & `mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -708,14 +708,15 @@
     "DisableEbsEncryptionByDefaultRequestRequestTypeDef",
     "DisableFastLaunchRequestRequestTypeDef",
     "DisableFastSnapshotRestoreStateErrorTypeDef",
     "DisableFastSnapshotRestoreSuccessItemTypeDef",
     "DisableFastSnapshotRestoresRequestRequestTypeDef",
     "DisableImageBlockPublicAccessRequestRequestTypeDef",
     "DisableImageDeprecationRequestRequestTypeDef",
+    "DisableImageDeregistrationProtectionRequestRequestTypeDef",
     "DisableImageRequestRequestTypeDef",
     "DisableIpamOrganizationAdminAccountRequestRequestTypeDef",
     "DisableSerialConsoleAccessRequestRequestTypeDef",
     "DisableSnapshotBlockPublicAccessRequestRequestTypeDef",
     "DisableTransitGatewayRouteTablePropagationRequestRequestTypeDef",
     "TransitGatewayPropagationTypeDef",
     "DisableVgwRoutePropagationRequestRequestTypeDef",
@@ -766,14 +767,15 @@
     "EnableEbsEncryptionByDefaultRequestRequestTypeDef",
     "FastLaunchLaunchTemplateSpecificationRequestTypeDef",
     "FastLaunchSnapshotConfigurationRequestTypeDef",
     "EnableFastSnapshotRestoreStateErrorTypeDef",
     "EnableFastSnapshotRestoreSuccessItemTypeDef",
     "EnableFastSnapshotRestoresRequestRequestTypeDef",
     "EnableImageBlockPublicAccessRequestRequestTypeDef",
+    "EnableImageDeregistrationProtectionRequestRequestTypeDef",
     "EnableImageRequestRequestTypeDef",
     "EnableIpamOrganizationAdminAccountRequestRequestTypeDef",
     "EnableReachabilityAnalyzerOrganizationSharingRequestRequestTypeDef",
     "EnableSerialConsoleAccessRequestRequestTypeDef",
     "EnableSnapshotBlockPublicAccessRequestRequestTypeDef",
     "EnableTransitGatewayRouteTablePropagationRequestRequestTypeDef",
     "EnableVgwRoutePropagationRequestRequestTypeDef",
@@ -1204,28 +1206,30 @@
     "DescribeAddressTransfersResultTypeDef",
     "DetachClassicLinkVpcResultTypeDef",
     "DisableAddressTransferResultTypeDef",
     "DisableAwsNetworkPerformanceMetricSubscriptionResultTypeDef",
     "DisableEbsEncryptionByDefaultResultTypeDef",
     "DisableImageBlockPublicAccessResultTypeDef",
     "DisableImageDeprecationResultTypeDef",
+    "DisableImageDeregistrationProtectionResultTypeDef",
     "DisableImageResultTypeDef",
     "DisableIpamOrganizationAdminAccountResultTypeDef",
     "DisableSerialConsoleAccessResultTypeDef",
     "DisableSnapshotBlockPublicAccessResultTypeDef",
     "DisableVpcClassicLinkDnsSupportResultTypeDef",
     "DisableVpcClassicLinkResultTypeDef",
     "DisassociateEnclaveCertificateIamRoleResultTypeDef",
     "DisassociateTrunkInterfaceResultTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EnableAddressTransferResultTypeDef",
     "EnableAwsNetworkPerformanceMetricSubscriptionResultTypeDef",
     "EnableEbsEncryptionByDefaultResultTypeDef",
     "EnableImageBlockPublicAccessResultTypeDef",
     "EnableImageDeprecationResultTypeDef",
+    "EnableImageDeregistrationProtectionResultTypeDef",
     "EnableImageResultTypeDef",
     "EnableIpamOrganizationAdminAccountResultTypeDef",
     "EnableReachabilityAnalyzerOrganizationSharingResultTypeDef",
     "EnableSerialConsoleAccessResultTypeDef",
     "EnableSnapshotBlockPublicAccessResultTypeDef",
     "EnableVpcClassicLinkDnsSupportResultTypeDef",
     "EnableVpcClassicLinkResultTypeDef",
@@ -5653,14 +5657,21 @@
 DisableImageDeprecationRequestRequestTypeDef = TypedDict(
     "DisableImageDeprecationRequestRequestTypeDef",
     {
         "ImageId": str,
         "DryRun": NotRequired[bool],
     },
 )
+DisableImageDeregistrationProtectionRequestRequestTypeDef = TypedDict(
+    "DisableImageDeregistrationProtectionRequestRequestTypeDef",
+    {
+        "ImageId": str,
+        "DryRun": NotRequired[bool],
+    },
+)
 DisableImageRequestRequestTypeDef = TypedDict(
     "DisableImageRequestRequestTypeDef",
     {
         "ImageId": str,
         "DryRun": NotRequired[bool],
     },
 )
@@ -6092,14 +6103,22 @@
 EnableImageBlockPublicAccessRequestRequestTypeDef = TypedDict(
     "EnableImageBlockPublicAccessRequestRequestTypeDef",
     {
         "ImageBlockPublicAccessState": Literal["block-new-sharing"],
         "DryRun": NotRequired[bool],
     },
 )
+EnableImageDeregistrationProtectionRequestRequestTypeDef = TypedDict(
+    "EnableImageDeregistrationProtectionRequestRequestTypeDef",
+    {
+        "ImageId": str,
+        "WithCooldown": NotRequired[bool],
+        "DryRun": NotRequired[bool],
+    },
+)
 EnableImageRequestRequestTypeDef = TypedDict(
     "EnableImageRequestRequestTypeDef",
     {
         "ImageId": str,
         "DryRun": NotRequired[bool],
     },
 )
@@ -9556,14 +9575,21 @@
 DisableImageDeprecationResultTypeDef = TypedDict(
     "DisableImageDeprecationResultTypeDef",
     {
         "Return": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DisableImageDeregistrationProtectionResultTypeDef = TypedDict(
+    "DisableImageDeregistrationProtectionResultTypeDef",
+    {
+        "Return": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DisableImageResultTypeDef = TypedDict(
     "DisableImageResultTypeDef",
     {
         "Return": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -9654,14 +9680,21 @@
 EnableImageDeprecationResultTypeDef = TypedDict(
     "EnableImageDeprecationResultTypeDef",
     {
         "Return": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+EnableImageDeregistrationProtectionResultTypeDef = TypedDict(
+    "EnableImageDeregistrationProtectionResultTypeDef",
+    {
+        "Return": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 EnableImageResultTypeDef = TypedDict(
     "EnableImageResultTypeDef",
     {
         "Return": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -19471,14 +19504,15 @@
         "RamdiskId": AttributeValueTypeDef,
         "SriovNetSupport": AttributeValueTypeDef,
         "BootMode": AttributeValueTypeDef,
         "TpmSupport": AttributeValueTypeDef,
         "UefiData": AttributeValueTypeDef,
         "LastLaunchedTime": AttributeValueTypeDef,
         "ImdsSupport": AttributeValueTypeDef,
+        "DeregistrationProtection": AttributeValueTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ImageTypeDef = TypedDict(
     "ImageTypeDef",
     {
         "Architecture": NotRequired[ArchitectureValuesType],
@@ -19508,14 +19542,16 @@
         "Tags": NotRequired[List[TagTypeDef]],
         "VirtualizationType": NotRequired[VirtualizationTypeType],
         "BootMode": NotRequired[BootModeValuesType],
         "TpmSupport": NotRequired[Literal["v2.0"]],
         "DeprecationTime": NotRequired[str],
         "ImdsSupport": NotRequired[Literal["v2.0"]],
         "SourceInstanceId": NotRequired[str],
+        "DeregistrationProtection": NotRequired[str],
+        "LastLaunchedTime": NotRequired[str],
     },
 )
 RegisterImageRequestRequestTypeDef = TypedDict(
     "RegisterImageRequestRequestTypeDef",
     {
         "Name": str,
         "ImageLocation": NotRequired[str],
```

### Comparing `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/type_defs.pyi` & `mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -708,14 +708,15 @@
     "DisableEbsEncryptionByDefaultRequestRequestTypeDef",
     "DisableFastLaunchRequestRequestTypeDef",
     "DisableFastSnapshotRestoreStateErrorTypeDef",
     "DisableFastSnapshotRestoreSuccessItemTypeDef",
     "DisableFastSnapshotRestoresRequestRequestTypeDef",
     "DisableImageBlockPublicAccessRequestRequestTypeDef",
     "DisableImageDeprecationRequestRequestTypeDef",
+    "DisableImageDeregistrationProtectionRequestRequestTypeDef",
     "DisableImageRequestRequestTypeDef",
     "DisableIpamOrganizationAdminAccountRequestRequestTypeDef",
     "DisableSerialConsoleAccessRequestRequestTypeDef",
     "DisableSnapshotBlockPublicAccessRequestRequestTypeDef",
     "DisableTransitGatewayRouteTablePropagationRequestRequestTypeDef",
     "TransitGatewayPropagationTypeDef",
     "DisableVgwRoutePropagationRequestRequestTypeDef",
@@ -766,14 +767,15 @@
     "EnableEbsEncryptionByDefaultRequestRequestTypeDef",
     "FastLaunchLaunchTemplateSpecificationRequestTypeDef",
     "FastLaunchSnapshotConfigurationRequestTypeDef",
     "EnableFastSnapshotRestoreStateErrorTypeDef",
     "EnableFastSnapshotRestoreSuccessItemTypeDef",
     "EnableFastSnapshotRestoresRequestRequestTypeDef",
     "EnableImageBlockPublicAccessRequestRequestTypeDef",
+    "EnableImageDeregistrationProtectionRequestRequestTypeDef",
     "EnableImageRequestRequestTypeDef",
     "EnableIpamOrganizationAdminAccountRequestRequestTypeDef",
     "EnableReachabilityAnalyzerOrganizationSharingRequestRequestTypeDef",
     "EnableSerialConsoleAccessRequestRequestTypeDef",
     "EnableSnapshotBlockPublicAccessRequestRequestTypeDef",
     "EnableTransitGatewayRouteTablePropagationRequestRequestTypeDef",
     "EnableVgwRoutePropagationRequestRequestTypeDef",
@@ -1204,28 +1206,30 @@
     "DescribeAddressTransfersResultTypeDef",
     "DetachClassicLinkVpcResultTypeDef",
     "DisableAddressTransferResultTypeDef",
     "DisableAwsNetworkPerformanceMetricSubscriptionResultTypeDef",
     "DisableEbsEncryptionByDefaultResultTypeDef",
     "DisableImageBlockPublicAccessResultTypeDef",
     "DisableImageDeprecationResultTypeDef",
+    "DisableImageDeregistrationProtectionResultTypeDef",
     "DisableImageResultTypeDef",
     "DisableIpamOrganizationAdminAccountResultTypeDef",
     "DisableSerialConsoleAccessResultTypeDef",
     "DisableSnapshotBlockPublicAccessResultTypeDef",
     "DisableVpcClassicLinkDnsSupportResultTypeDef",
     "DisableVpcClassicLinkResultTypeDef",
     "DisassociateEnclaveCertificateIamRoleResultTypeDef",
     "DisassociateTrunkInterfaceResultTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EnableAddressTransferResultTypeDef",
     "EnableAwsNetworkPerformanceMetricSubscriptionResultTypeDef",
     "EnableEbsEncryptionByDefaultResultTypeDef",
     "EnableImageBlockPublicAccessResultTypeDef",
     "EnableImageDeprecationResultTypeDef",
+    "EnableImageDeregistrationProtectionResultTypeDef",
     "EnableImageResultTypeDef",
     "EnableIpamOrganizationAdminAccountResultTypeDef",
     "EnableReachabilityAnalyzerOrganizationSharingResultTypeDef",
     "EnableSerialConsoleAccessResultTypeDef",
     "EnableSnapshotBlockPublicAccessResultTypeDef",
     "EnableVpcClassicLinkDnsSupportResultTypeDef",
     "EnableVpcClassicLinkResultTypeDef",
@@ -5653,14 +5657,21 @@
 DisableImageDeprecationRequestRequestTypeDef = TypedDict(
     "DisableImageDeprecationRequestRequestTypeDef",
     {
         "ImageId": str,
         "DryRun": NotRequired[bool],
     },
 )
+DisableImageDeregistrationProtectionRequestRequestTypeDef = TypedDict(
+    "DisableImageDeregistrationProtectionRequestRequestTypeDef",
+    {
+        "ImageId": str,
+        "DryRun": NotRequired[bool],
+    },
+)
 DisableImageRequestRequestTypeDef = TypedDict(
     "DisableImageRequestRequestTypeDef",
     {
         "ImageId": str,
         "DryRun": NotRequired[bool],
     },
 )
@@ -6092,14 +6103,22 @@
 EnableImageBlockPublicAccessRequestRequestTypeDef = TypedDict(
     "EnableImageBlockPublicAccessRequestRequestTypeDef",
     {
         "ImageBlockPublicAccessState": Literal["block-new-sharing"],
         "DryRun": NotRequired[bool],
     },
 )
+EnableImageDeregistrationProtectionRequestRequestTypeDef = TypedDict(
+    "EnableImageDeregistrationProtectionRequestRequestTypeDef",
+    {
+        "ImageId": str,
+        "WithCooldown": NotRequired[bool],
+        "DryRun": NotRequired[bool],
+    },
+)
 EnableImageRequestRequestTypeDef = TypedDict(
     "EnableImageRequestRequestTypeDef",
     {
         "ImageId": str,
         "DryRun": NotRequired[bool],
     },
 )
@@ -9556,14 +9575,21 @@
 DisableImageDeprecationResultTypeDef = TypedDict(
     "DisableImageDeprecationResultTypeDef",
     {
         "Return": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DisableImageDeregistrationProtectionResultTypeDef = TypedDict(
+    "DisableImageDeregistrationProtectionResultTypeDef",
+    {
+        "Return": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DisableImageResultTypeDef = TypedDict(
     "DisableImageResultTypeDef",
     {
         "Return": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -9654,14 +9680,21 @@
 EnableImageDeprecationResultTypeDef = TypedDict(
     "EnableImageDeprecationResultTypeDef",
     {
         "Return": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+EnableImageDeregistrationProtectionResultTypeDef = TypedDict(
+    "EnableImageDeregistrationProtectionResultTypeDef",
+    {
+        "Return": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 EnableImageResultTypeDef = TypedDict(
     "EnableImageResultTypeDef",
     {
         "Return": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -19471,14 +19504,15 @@
         "RamdiskId": AttributeValueTypeDef,
         "SriovNetSupport": AttributeValueTypeDef,
         "BootMode": AttributeValueTypeDef,
         "TpmSupport": AttributeValueTypeDef,
         "UefiData": AttributeValueTypeDef,
         "LastLaunchedTime": AttributeValueTypeDef,
         "ImdsSupport": AttributeValueTypeDef,
+        "DeregistrationProtection": AttributeValueTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ImageTypeDef = TypedDict(
     "ImageTypeDef",
     {
         "Architecture": NotRequired[ArchitectureValuesType],
@@ -19508,14 +19542,16 @@
         "Tags": NotRequired[List[TagTypeDef]],
         "VirtualizationType": NotRequired[VirtualizationTypeType],
         "BootMode": NotRequired[BootModeValuesType],
         "TpmSupport": NotRequired[Literal["v2.0"]],
         "DeprecationTime": NotRequired[str],
         "ImdsSupport": NotRequired[Literal["v2.0"]],
         "SourceInstanceId": NotRequired[str],
+        "DeregistrationProtection": NotRequired[str],
+        "LastLaunchedTime": NotRequired[str],
     },
 )
 RegisterImageRequestRequestTypeDef = TypedDict(
     "RegisterImageRequestRequestTypeDef",
     {
         "Name": str,
         "ImageLocation": NotRequired[str],
```

### Comparing `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/waiter.py` & `mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/waiter.pyi` & `mypy_boto3_ec2-1.34.90/mypy_boto3_ec2/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2.egg-info/PKG-INFO` & `mypy_boto3_ec2-1.34.90/mypy_boto3_ec2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ec2
-Version: 1.34.86
-Summary: Type annotations for boto3.EC2 1.34.86 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.90
+Summary: Type annotations for boto3.EC2 1.34.90 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ec2.svg?color=blue)](https://pypi.org/project/mypy-boto3-ec2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ec2)](https://pepy.tech/project/mypy-boto3-ec2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EC2 1.34.86](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
+[boto3.EC2 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2.egg-info/SOURCES.txt` & `mypy_boto3_ec2-1.34.90/mypy_boto3_ec2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_ec2-1.34.86/setup.py` & `mypy_boto3_ec2-1.34.90/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ec2",
-    version="1.34.86",
+    version="1.34.90",
     packages=["mypy_boto3_ec2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.EC2 1.34.86 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.EC2 1.34.90 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

