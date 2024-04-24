# Comparing `tmp/flytekitplugins-mmcloud-1.12.0b5.tar.gz` & `tmp/flytekitplugins_mmcloud-1.12.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-mmcloud-1.12.0b5.tar", last modified: Wed Apr 10 17:16:54 2024, max compression
+gzip compressed data, was "flytekitplugins_mmcloud-1.12.0b6.tar", last modified: Wed Apr 24 18:30:38 2024, max compression
```

## Comparing `flytekitplugins-mmcloud-1.12.0b5.tar` & `flytekitplugins_mmcloud-1.12.0b6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:54.379253 flytekitplugins-mmcloud-1.12.0b5/
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-10 17:16:54.379253 flytekitplugins-mmcloud-1.12.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-10 17:16:22.000000 flytekitplugins-mmcloud-1.12.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:54.375254 flytekitplugins-mmcloud-1.12.0b5/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:54.379253 flytekitplugins-mmcloud-1.12.0b5/flytekitplugins/mmcloud/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-10 17:16:22.000000 flytekitplugins-mmcloud-1.12.0b5/flytekitplugins/mmcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-04-10 17:16:22.000000 flytekitplugins-mmcloud-1.12.0b5/flytekitplugins/mmcloud/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-10 17:16:22.000000 flytekitplugins-mmcloud-1.12.0b5/flytekitplugins/mmcloud/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-10 17:16:22.000000 flytekitplugins-mmcloud-1.12.0b5/flytekitplugins/mmcloud/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:54.379253 flytekitplugins-mmcloud-1.12.0b5/flytekitplugins_mmcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-10 17:16:54.000000 flytekitplugins-mmcloud-1.12.0b5/flytekitplugins_mmcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-10 17:16:54.000000 flytekitplugins-mmcloud-1.12.0b5/flytekitplugins_mmcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:16:54.000000 flytekitplugins-mmcloud-1.12.0b5/flytekitplugins_mmcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-10 17:16:54.000000 flytekitplugins-mmcloud-1.12.0b5/flytekitplugins_mmcloud.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 17:16:54.000000 flytekitplugins-mmcloud-1.12.0b5/flytekitplugins_mmcloud.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-10 17:16:54.000000 flytekitplugins-mmcloud-1.12.0b5/flytekitplugins_mmcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 17:16:54.000000 flytekitplugins-mmcloud-1.12.0b5/flytekitplugins_mmcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 17:16:54.379253 flytekitplugins-mmcloud-1.12.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-10 17:16:47.000000 flytekitplugins-mmcloud-1.12.0b5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:54.379253 flytekitplugins-mmcloud-1.12.0b5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-04-10 17:16:22.000000 flytekitplugins-mmcloud-1.12.0b5/tests/test_mmcloud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:38.245226 flytekitplugins_mmcloud-1.12.0b6/
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-24 18:30:38.245226 flytekitplugins_mmcloud-1.12.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-24 18:30:04.000000 flytekitplugins_mmcloud-1.12.0b6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:38.241225 flytekitplugins_mmcloud-1.12.0b6/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:38.241225 flytekitplugins_mmcloud-1.12.0b6/flytekitplugins/mmcloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-24 18:30:04.000000 flytekitplugins_mmcloud-1.12.0b6/flytekitplugins/mmcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-04-24 18:30:04.000000 flytekitplugins_mmcloud-1.12.0b6/flytekitplugins/mmcloud/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-24 18:30:04.000000 flytekitplugins_mmcloud-1.12.0b6/flytekitplugins/mmcloud/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-24 18:30:04.000000 flytekitplugins_mmcloud-1.12.0b6/flytekitplugins/mmcloud/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:38.245226 flytekitplugins_mmcloud-1.12.0b6/flytekitplugins_mmcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-24 18:30:38.000000 flytekitplugins_mmcloud-1.12.0b6/flytekitplugins_mmcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-24 18:30:38.000000 flytekitplugins_mmcloud-1.12.0b6/flytekitplugins_mmcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 18:30:38.000000 flytekitplugins_mmcloud-1.12.0b6/flytekitplugins_mmcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-24 18:30:38.000000 flytekitplugins_mmcloud-1.12.0b6/flytekitplugins_mmcloud.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 18:30:38.000000 flytekitplugins_mmcloud-1.12.0b6/flytekitplugins_mmcloud.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-24 18:30:38.000000 flytekitplugins_mmcloud-1.12.0b6/flytekitplugins_mmcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 18:30:38.000000 flytekitplugins_mmcloud-1.12.0b6/flytekitplugins_mmcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 18:30:38.245226 flytekitplugins_mmcloud-1.12.0b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-24 18:30:31.000000 flytekitplugins_mmcloud-1.12.0b6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:38.245226 flytekitplugins_mmcloud-1.12.0b6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-04-24 18:30:04.000000 flytekitplugins_mmcloud-1.12.0b6/tests/test_mmcloud.py
```

### Comparing `flytekitplugins-mmcloud-1.12.0b5/PKG-INFO` & `flytekitplugins_mmcloud-1.12.0b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-mmcloud
-Version: 1.12.0b5
+Version: 1.12.0b6
 Summary: MemVerge Flyte plugin
 Author: Edwin Yu, Helen Zhang
 Author-email: helen.zhang@memverge.com
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-mmcloud-1.12.0b5/README.md` & `flytekitplugins_mmcloud-1.12.0b6/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-mmcloud-1.12.0b5/flytekitplugins/mmcloud/agent.py` & `flytekitplugins_mmcloud-1.12.0b6/flytekitplugins/mmcloud/agent.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-mmcloud-1.12.0b5/flytekitplugins/mmcloud/task.py` & `flytekitplugins_mmcloud-1.12.0b6/flytekitplugins/mmcloud/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-mmcloud-1.12.0b5/flytekitplugins/mmcloud/utils.py` & `flytekitplugins_mmcloud-1.12.0b6/flytekitplugins/mmcloud/utils.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-mmcloud-1.12.0b5/flytekitplugins_mmcloud.egg-info/PKG-INFO` & `flytekitplugins_mmcloud-1.12.0b6/flytekitplugins_mmcloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-mmcloud
-Version: 1.12.0b5
+Version: 1.12.0b6
 Summary: MemVerge Flyte plugin
 Author: Edwin Yu, Helen Zhang
 Author-email: helen.zhang@memverge.com
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-mmcloud-1.12.0b5/flytekitplugins_mmcloud.egg-info/SOURCES.txt` & `flytekitplugins_mmcloud-1.12.0b6/flytekitplugins_mmcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flytekitplugins-mmcloud-1.12.0b5/setup.py` & `flytekitplugins_mmcloud-1.12.0b6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "mmcloud"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.9.1,<2.0.0", "kubernetes"]
 
-__version__ = "1.12.0b5"
+__version__ = "1.12.0b6"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="Edwin Yu, Helen Zhang",
     author_email="helen.zhang@memverge.com",
     description="MemVerge Flyte plugin",
```

### Comparing `flytekitplugins-mmcloud-1.12.0b5/tests/test_mmcloud.py` & `flytekitplugins_mmcloud-1.12.0b6/tests/test_mmcloud.py`

 * *Files identical despite different names*

