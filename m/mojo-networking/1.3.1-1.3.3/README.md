# Comparing `tmp/mojo_networking-1.3.1.tar.gz` & `tmp/mojo_networking-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_networking-1.3.1.tar", max compression
+gzip compressed data, was "mojo_networking-1.3.3.tar", max compression
```

## Comparing `mojo_networking-1.3.1.tar` & `mojo_networking-1.3.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1083 2024-01-26 02:54:48.206905 mojo_networking-1.3.1/LICENSE.txt
--rw-r--r--   0        0        0      117 2024-01-26 02:54:48.207038 mojo_networking-1.3.1/README.md
--rw-r--r--   0        0        0      889 2024-03-08 04:16:11.114580 mojo_networking-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      500 2024-01-26 02:54:48.208882 mojo_networking-1.3.1/source/packages/mojo/networking/__init__.py
--rw-r--r--   0        0        0      613 2024-01-26 02:54:48.208987 mojo_networking-1.3.1/source/packages/mojo/networking/broadcast.py
--rw-r--r--   0        0        0     6959 2024-01-26 02:54:48.209050 mojo_networking-1.3.1/source/packages/mojo/networking/constants.py
--rw-r--r--   0        0        0     2910 2024-01-26 02:54:48.209132 mojo_networking-1.3.1/source/packages/mojo/networking/exceptions.py
--rw-r--r--   0        0        0     9204 2024-01-26 02:54:48.209233 mojo_networking-1.3.1/source/packages/mojo/networking/interfaces.py
--rw-r--r--   0        0        0     8824 2024-01-26 02:54:48.209339 mojo_networking-1.3.1/source/packages/mojo/networking/multicast.py
--rw-r--r--   0        0        0     2381 2024-01-26 02:54:48.209415 mojo_networking-1.3.1/source/packages/mojo/networking/resolution.py
--rw-r--r--   0        0        0     1845 2024-01-26 02:54:48.209499 mojo_networking-1.3.1/source/packages/mojo/networking/trafficcapturecontext.py
--rw-r--r--   0        0        0     4543 2024-01-26 02:54:48.209575 mojo_networking-1.3.1/source/packages/mojo/networking/unicast.py
--rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 mojo_networking-1.3.1/setup.py
--rw-r--r--   0        0        0     1037 1970-01-01 00:00:00.000000 mojo_networking-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-01-26 02:54:48.206905 mojo_networking-1.3.3/LICENSE.txt
+-rw-r--r--   0        0        0      117 2024-01-26 02:54:48.207038 mojo_networking-1.3.3/README.md
+-rw-r--r--   0        0        0      889 2024-04-24 03:30:57.707357 mojo_networking-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0      500 2024-01-26 02:54:48.208882 mojo_networking-1.3.3/source/packages/mojo/networking/__init__.py
+-rw-r--r--   0        0        0      613 2024-01-26 02:54:48.208987 mojo_networking-1.3.3/source/packages/mojo/networking/broadcast.py
+-rw-r--r--   0        0        0     7259 2024-04-23 18:40:08.355498 mojo_networking-1.3.3/source/packages/mojo/networking/constants.py
+-rw-r--r--   0        0        0     2910 2024-01-26 02:54:48.209132 mojo_networking-1.3.3/source/packages/mojo/networking/exceptions.py
+-rw-r--r--   0        0        0     9204 2024-01-26 02:54:48.209233 mojo_networking-1.3.3/source/packages/mojo/networking/interfaces.py
+-rw-r--r--   0        0        0     8824 2024-01-26 02:54:48.209339 mojo_networking-1.3.3/source/packages/mojo/networking/multicast.py
+-rw-r--r--   0        0        0     5795 2024-04-23 20:33:28.693413 mojo_networking-1.3.3/source/packages/mojo/networking/resolution.py
+-rw-r--r--   0        0        0     1845 2024-01-26 02:54:48.209499 mojo_networking-1.3.3/source/packages/mojo/networking/trafficcapturecontext.py
+-rw-r--r--   0        0        0     4543 2024-01-26 02:54:48.209575 mojo_networking-1.3.3/source/packages/mojo/networking/unicast.py
+-rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 mojo_networking-1.3.3/setup.py
+-rw-r--r--   0        0        0     1037 1970-01-01 00:00:00.000000 mojo_networking-1.3.3/PKG-INFO
```

### Comparing `mojo_networking-1.3.1/LICENSE.txt` & `mojo_networking-1.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mojo_networking-1.3.1/pyproject.toml` & `mojo_networking-1.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mojo-networking"
 description = "Automation Mojo Netorking Package (mojo-networking)"
-version = "1.3.1"
+version = "1.3.3"
 authors = [
     "Myron Walker <myron.walker@gmail.com>"
 ]
 readme = "README.md"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `mojo_networking-1.3.1/source/packages/mojo/networking/broadcast.py` & `mojo_networking-1.3.3/source/packages/mojo/networking/broadcast.py`

 * *Files identical despite different names*

### Comparing `mojo_networking-1.3.1/source/packages/mojo/networking/constants.py` & `mojo_networking-1.3.3/source/packages/mojo/networking/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 __version__ = "1.0.0"
 __maintainer__ = "Myron Walker"
 __email__ = "myron.walker@gmail.com"
 __status__ = "Development" # Prototype, Development or Production
 __license__ = "MIT"
 
 import platform
+import re
 import socket
 
 HTTP1_1_LINESEP = b"\r\n"
 HTTP1_1_END_OF_HEADER = b"\r\n\r\n"
 HTTP1_1_END_OF_MESSAGE = b"\r\n\r\n"
 
 if hasattr(socket, "IPPROTO_IPV6"):
@@ -39,14 +40,20 @@
 UPNP_GROUP_LOCAL_ADDR6 = 'FF02::1'
 UPNP_GROUP_SITE_ADDR6 = 'FF05::1'
 UPNP_GROUP_ORG_ADDR6 = 'FF08::1'
 UPNP_GROUP_GLOBAL_ADDR6 = 'FF0E::1'
 
 UPNP_PORT = 1900
 
+
+CHARSET_IPV6_ADDR = 'ABCDEFabcdef0123456789:'
+
+REGEX_IPV4_COMPONENTS = re.compile(r"^([0-9]+)\.([0-9]+)\.([0-9]+)\.([0-9]+)$")
+REGEX_IPV6_COMPONENTS = re.compile(r"^([0-9A-Fa-f]+):([0-9A-Fa-f]+):([0-9A-Fa-f]+):([0-9A-Fa-f]+):([0-9A-Fa-f]+):([0-9A-Fa-f]+):([0-9A-Fa-f]+):([0-9A-Fa-f]+)$")
+
 if hasattr(socket, "SO_RECV_ANYIF"):
     SO_RECV_ANYIF = socket.SO_RECV_ANYIF
 else:
     # https://opensource.apple.com/source/xnu/xnu-4570.41.2/bsd/sys/socket.h
     SO_RECV_ANYIF = 0x1104
 
 class RegisteredMulticastAddresses:
```

### Comparing `mojo_networking-1.3.1/source/packages/mojo/networking/exceptions.py` & `mojo_networking-1.3.3/source/packages/mojo/networking/exceptions.py`

 * *Files identical despite different names*

### Comparing `mojo_networking-1.3.1/source/packages/mojo/networking/interfaces.py` & `mojo_networking-1.3.3/source/packages/mojo/networking/interfaces.py`

 * *Files identical despite different names*

### Comparing `mojo_networking-1.3.1/source/packages/mojo/networking/multicast.py` & `mojo_networking-1.3.3/source/packages/mojo/networking/multicast.py`

 * *Files identical despite different names*

### Comparing `mojo_networking-1.3.1/source/packages/mojo/networking/trafficcapturecontext.py` & `mojo_networking-1.3.3/source/packages/mojo/networking/trafficcapturecontext.py`

 * *Files identical despite different names*

### Comparing `mojo_networking-1.3.1/source/packages/mojo/networking/unicast.py` & `mojo_networking-1.3.3/source/packages/mojo/networking/unicast.py`

 * *Files identical despite different names*

### Comparing `mojo_networking-1.3.1/setup.py` & `mojo_networking-1.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['netifaces>=0.11.0,<0.12.0', 'requests>=2.31.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'mojo-networking',
-    'version': '1.3.1',
+    'version': '1.3.3',
     'description': 'Automation Mojo Netorking Package (mojo-networking)',
     'long_description': '# python-package-template\nThis is a template repository that can be used to quickly create a python package project.\n',
     'author': 'Myron Walker',
     'author_email': 'myron.walker@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'http://automationmojo.com',
```

### Comparing `mojo_networking-1.3.1/PKG-INFO` & `mojo_networking-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mojo-networking
-Version: 1.3.1
+Version: 1.3.3
 Summary: Automation Mojo Netorking Package (mojo-networking)
 Home-page: http://automationmojo.com
 License: LICENSE.txt
 Keywords: python
 Author: Myron Walker
 Author-email: myron.walker@gmail.com
 Requires-Python: >=3.8,<4.0
```

