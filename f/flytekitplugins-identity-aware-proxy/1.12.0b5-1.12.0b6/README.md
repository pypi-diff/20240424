# Comparing `tmp/flytekitplugins-identity_aware_proxy-1.12.0b5.tar.gz` & `tmp/flytekitplugins_identity_aware_proxy-1.12.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-identity_aware_proxy-1.12.0b5.tar", last modified: Wed Apr 10 17:16:52 2024, max compression
+gzip compressed data, was "flytekitplugins_identity_aware_proxy-1.12.0b6.tar", last modified: Wed Apr 24 18:30:36 2024, max compression
```

## Comparing `flytekitplugins-identity_aware_proxy-1.12.0b5.tar` & `flytekitplugins_identity_aware_proxy-1.12.0b6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:52.775269 flytekitplugins-identity_aware_proxy-1.12.0b5/
--rw-r--r--   0 runner    (1001) docker     (127)    21942 2024-04-10 17:16:52.775269 flytekitplugins-identity_aware_proxy-1.12.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20805 2024-04-10 17:16:22.000000 flytekitplugins-identity_aware_proxy-1.12.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:52.775269 flytekitplugins-identity_aware_proxy-1.12.0b5/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:52.775269 flytekitplugins-identity_aware_proxy-1.12.0b5/flytekitplugins/identity_aware_proxy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:22.000000 flytekitplugins-identity_aware_proxy-1.12.0b5/flytekitplugins/identity_aware_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9491 2024-04-10 17:16:22.000000 flytekitplugins-identity_aware_proxy-1.12.0b5/flytekitplugins/identity_aware_proxy/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:52.775269 flytekitplugins-identity_aware_proxy-1.12.0b5/flytekitplugins_identity_aware_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21942 2024-04-10 17:16:52.000000 flytekitplugins-identity_aware_proxy-1.12.0b5/flytekitplugins_identity_aware_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-10 17:16:52.000000 flytekitplugins-identity_aware_proxy-1.12.0b5/flytekitplugins_identity_aware_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:16:52.000000 flytekitplugins-identity_aware_proxy-1.12.0b5/flytekitplugins_identity_aware_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-10 17:16:52.000000 flytekitplugins-identity_aware_proxy-1.12.0b5/flytekitplugins_identity_aware_proxy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 17:16:52.000000 flytekitplugins-identity_aware_proxy-1.12.0b5/flytekitplugins_identity_aware_proxy.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-10 17:16:52.000000 flytekitplugins-identity_aware_proxy-1.12.0b5/flytekitplugins_identity_aware_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 17:16:52.000000 flytekitplugins-identity_aware_proxy-1.12.0b5/flytekitplugins_identity_aware_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 17:16:52.775269 flytekitplugins-identity_aware_proxy-1.12.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-10 17:16:47.000000 flytekitplugins-identity_aware_proxy-1.12.0b5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:52.775269 flytekitplugins-identity_aware_proxy-1.12.0b5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-04-10 17:16:22.000000 flytekitplugins-identity_aware_proxy-1.12.0b5/tests/test_flytekitplugins_iap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:36.585215 flytekitplugins_identity_aware_proxy-1.12.0b6/
+-rw-r--r--   0 runner    (1001) docker     (127)    21942 2024-04-24 18:30:36.585215 flytekitplugins_identity_aware_proxy-1.12.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20805 2024-04-24 18:30:04.000000 flytekitplugins_identity_aware_proxy-1.12.0b6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:36.581215 flytekitplugins_identity_aware_proxy-1.12.0b6/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:36.581215 flytekitplugins_identity_aware_proxy-1.12.0b6/flytekitplugins/identity_aware_proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:04.000000 flytekitplugins_identity_aware_proxy-1.12.0b6/flytekitplugins/identity_aware_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9491 2024-04-24 18:30:04.000000 flytekitplugins_identity_aware_proxy-1.12.0b6/flytekitplugins/identity_aware_proxy/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:36.585215 flytekitplugins_identity_aware_proxy-1.12.0b6/flytekitplugins_identity_aware_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21942 2024-04-24 18:30:36.000000 flytekitplugins_identity_aware_proxy-1.12.0b6/flytekitplugins_identity_aware_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-24 18:30:36.000000 flytekitplugins_identity_aware_proxy-1.12.0b6/flytekitplugins_identity_aware_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 18:30:36.000000 flytekitplugins_identity_aware_proxy-1.12.0b6/flytekitplugins_identity_aware_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 18:30:36.000000 flytekitplugins_identity_aware_proxy-1.12.0b6/flytekitplugins_identity_aware_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 18:30:36.000000 flytekitplugins_identity_aware_proxy-1.12.0b6/flytekitplugins_identity_aware_proxy.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-24 18:30:36.000000 flytekitplugins_identity_aware_proxy-1.12.0b6/flytekitplugins_identity_aware_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 18:30:36.000000 flytekitplugins_identity_aware_proxy-1.12.0b6/flytekitplugins_identity_aware_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 18:30:36.585215 flytekitplugins_identity_aware_proxy-1.12.0b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-24 18:30:31.000000 flytekitplugins_identity_aware_proxy-1.12.0b6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:36.585215 flytekitplugins_identity_aware_proxy-1.12.0b6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-04-24 18:30:04.000000 flytekitplugins_identity_aware_proxy-1.12.0b6/tests/test_flytekitplugins_iap.py
```

### Comparing `flytekitplugins-identity_aware_proxy-1.12.0b5/PKG-INFO` & `flytekitplugins_identity_aware_proxy-1.12.0b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-identity_aware_proxy
-Version: 1.12.0b5
+Version: 1.12.0b6
 Summary: External command plugin to generate ID tokens for GCP Identity Aware Proxy
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-identity-aware-proxy
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins-identity_aware_proxy-1.12.0b5/README.md` & `flytekitplugins_identity_aware_proxy-1.12.0b6/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-identity_aware_proxy-1.12.0b5/flytekitplugins/identity_aware_proxy/cli.py` & `flytekitplugins_identity_aware_proxy-1.12.0b6/flytekitplugins/identity_aware_proxy/cli.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-identity_aware_proxy-1.12.0b5/flytekitplugins_identity_aware_proxy.egg-info/PKG-INFO` & `flytekitplugins_identity_aware_proxy-1.12.0b6/flytekitplugins_identity_aware_proxy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-identity_aware_proxy
-Version: 1.12.0b5
+Version: 1.12.0b6
 Summary: External command plugin to generate ID tokens for GCP Identity Aware Proxy
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-identity-aware-proxy
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins-identity_aware_proxy-1.12.0b5/flytekitplugins_identity_aware_proxy.egg-info/SOURCES.txt` & `flytekitplugins_identity_aware_proxy-1.12.0b6/flytekitplugins_identity_aware_proxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flytekitplugins-identity_aware_proxy-1.12.0b5/setup.py` & `flytekitplugins_identity_aware_proxy-1.12.0b6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "google-auth",
     "flytekit>=1.10",
     # https://github.com/grpc/grpc/issues/33935
     # https://github.com/grpc/grpc/issues/35323
     "grpcio>=1.62.0",
 ]
 
-__version__ = "1.12.0b5"
+__version__ = "1.12.0b6"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="External command plugin to generate ID tokens for GCP Identity Aware Proxy",
```

### Comparing `flytekitplugins-identity_aware_proxy-1.12.0b5/tests/test_flytekitplugins_iap.py` & `flytekitplugins_identity_aware_proxy-1.12.0b6/tests/test_flytekitplugins_iap.py`

 * *Files identical despite different names*

