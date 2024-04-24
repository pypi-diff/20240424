# Comparing `tmp/flytekitplugins-openai-1.12.0b5.tar.gz` & `tmp/flytekitplugins_openai-1.12.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-openai-1.12.0b5.tar", last modified: Wed Apr 10 17:16:55 2024, max compression
+gzip compressed data, was "flytekitplugins_openai-1.12.0b6.tar", last modified: Wed Apr 24 18:30:39 2024, max compression
```

## Comparing `flytekitplugins-openai-1.12.0b5.tar` & `flytekitplugins_openai-1.12.0b6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:55.715240 flytekitplugins-openai-1.12.0b5/
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-10 17:16:55.715240 flytekitplugins-openai-1.12.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-10 17:16:22.000000 flytekitplugins-openai-1.12.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:55.711240 flytekitplugins-openai-1.12.0b5/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:55.711240 flytekitplugins-openai-1.12.0b5/flytekitplugins/openai/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-10 17:16:22.000000 flytekitplugins-openai-1.12.0b5/flytekitplugins/openai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:55.715240 flytekitplugins-openai-1.12.0b5/flytekitplugins/openai/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:22.000000 flytekitplugins-openai-1.12.0b5/flytekitplugins/openai/chatgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-10 17:16:22.000000 flytekitplugins-openai-1.12.0b5/flytekitplugins/openai/chatgpt/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-10 17:16:22.000000 flytekitplugins-openai-1.12.0b5/flytekitplugins/openai/chatgpt/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:55.715240 flytekitplugins-openai-1.12.0b5/flytekitplugins_openai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-10 17:16:55.000000 flytekitplugins-openai-1.12.0b5/flytekitplugins_openai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-10 17:16:55.000000 flytekitplugins-openai-1.12.0b5/flytekitplugins_openai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 17:16:55.000000 flytekitplugins-openai-1.12.0b5/flytekitplugins_openai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-10 17:16:55.000000 flytekitplugins-openai-1.12.0b5/flytekitplugins_openai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 17:16:55.000000 flytekitplugins-openai-1.12.0b5/flytekitplugins_openai.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-10 17:16:55.000000 flytekitplugins-openai-1.12.0b5/flytekitplugins_openai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 17:16:55.000000 flytekitplugins-openai-1.12.0b5/flytekitplugins_openai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 17:16:55.715240 flytekitplugins-openai-1.12.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-10 17:16:47.000000 flytekitplugins-openai-1.12.0b5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 17:16:55.715240 flytekitplugins-openai-1.12.0b5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-10 17:16:22.000000 flytekitplugins-openai-1.12.0b5/tests/test_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-10 17:16:22.000000 flytekitplugins-openai-1.12.0b5/tests/test_chatgpt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:39.585234 flytekitplugins_openai-1.12.0b6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-24 18:30:39.585234 flytekitplugins_openai-1.12.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-24 18:30:04.000000 flytekitplugins_openai-1.12.0b6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:39.581234 flytekitplugins_openai-1.12.0b6/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:39.581234 flytekitplugins_openai-1.12.0b6/flytekitplugins/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-24 18:30:04.000000 flytekitplugins_openai-1.12.0b6/flytekitplugins/openai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:39.581234 flytekitplugins_openai-1.12.0b6/flytekitplugins/openai/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:04.000000 flytekitplugins_openai-1.12.0b6/flytekitplugins/openai/chatgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-24 18:30:04.000000 flytekitplugins_openai-1.12.0b6/flytekitplugins/openai/chatgpt/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-24 18:30:04.000000 flytekitplugins_openai-1.12.0b6/flytekitplugins/openai/chatgpt/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:39.585234 flytekitplugins_openai-1.12.0b6/flytekitplugins_openai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-24 18:30:39.000000 flytekitplugins_openai-1.12.0b6/flytekitplugins_openai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-24 18:30:39.000000 flytekitplugins_openai-1.12.0b6/flytekitplugins_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 18:30:39.000000 flytekitplugins_openai-1.12.0b6/flytekitplugins_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 18:30:39.000000 flytekitplugins_openai-1.12.0b6/flytekitplugins_openai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 18:30:39.000000 flytekitplugins_openai-1.12.0b6/flytekitplugins_openai.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-24 18:30:39.000000 flytekitplugins_openai-1.12.0b6/flytekitplugins_openai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 18:30:39.000000 flytekitplugins_openai-1.12.0b6/flytekitplugins_openai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 18:30:39.585234 flytekitplugins_openai-1.12.0b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-24 18:30:31.000000 flytekitplugins_openai-1.12.0b6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:39.585234 flytekitplugins_openai-1.12.0b6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-24 18:30:04.000000 flytekitplugins_openai-1.12.0b6/tests/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-24 18:30:04.000000 flytekitplugins_openai-1.12.0b6/tests/test_chatgpt.py
```

### Comparing `flytekitplugins-openai-1.12.0b5/PKG-INFO` & `flytekitplugins_openai-1.12.0b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-openai
-Version: 1.12.0b5
+Version: 1.12.0b6
 Summary: This package holds the openai plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-openai-1.12.0b5/README.md` & `flytekitplugins_openai-1.12.0b6/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-openai-1.12.0b5/flytekitplugins/openai/chatgpt/agent.py` & `flytekitplugins_openai-1.12.0b6/flytekitplugins/openai/chatgpt/agent.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-openai-1.12.0b5/flytekitplugins/openai/chatgpt/task.py` & `flytekitplugins_openai-1.12.0b6/flytekitplugins/openai/chatgpt/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-openai-1.12.0b5/flytekitplugins_openai.egg-info/PKG-INFO` & `flytekitplugins_openai-1.12.0b6/flytekitplugins_openai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-openai
-Version: 1.12.0b5
+Version: 1.12.0b6
 Summary: This package holds the openai plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-openai-1.12.0b5/flytekitplugins_openai.egg-info/SOURCES.txt` & `flytekitplugins_openai-1.12.0b6/flytekitplugins_openai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flytekitplugins-openai-1.12.0b5/setup.py` & `flytekitplugins_openai-1.12.0b6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "openai"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>1.10.7", "openai>=1.12.0", "flyteidl>=1.11.0"]
 
-__version__ = "1.12.0b5"
+__version__ = "1.12.0b6"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package holds the openai plugins for flytekit",
```

### Comparing `flytekitplugins-openai-1.12.0b5/tests/test_agent.py` & `flytekitplugins_openai-1.12.0b6/tests/test_agent.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-openai-1.12.0b5/tests/test_chatgpt.py` & `flytekitplugins_openai-1.12.0b6/tests/test_chatgpt.py`

 * *Files identical despite different names*

