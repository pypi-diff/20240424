# Comparing `tmp/kmt-0.3.0.tar.gz` & `tmp/kmt-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmt-0.3.0.tar", last modified: Tue Apr 23 01:37:13 2024, max compression
+gzip compressed data, was "kmt-0.3.1.tar", last modified: Tue Apr 23 01:59:27 2024, max compression
```

## Comparing `kmt-0.3.0.tar` & `kmt-0.3.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:37:13.699128 kmt-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-23 01:36:59.000000 kmt-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-23 01:37:13.695128 kmt-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 01:36:59.000000 kmt-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 01:37:13.699128 kmt-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-23 01:36:59.000000 kmt-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:37:13.695128 kmt-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:37:13.695128 kmt-0.3.0/src/kmt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 01:36:59.000000 kmt-0.3.0/src/kmt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-23 01:36:59.000000 kmt-0.3.0/src/kmt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24412 2024-04-23 01:36:59.000000 kmt-0.3.0/src/kmt/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-23 01:36:59.000000 kmt-0.3.0/src/kmt/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-23 01:36:59.000000 kmt-0.3.0/src/kmt/j2support.py
--rw-r--r--   0 runner    (1001) docker     (127)    11927 2024-04-23 01:36:59.000000 kmt-0.3.0/src/kmt/pipeline_support.py
--rw-r--r--   0 runner    (1001) docker     (127)    12658 2024-04-23 01:36:59.000000 kmt-0.3.0/src/kmt/step_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-04-23 01:36:59.000000 kmt-0.3.0/src/kmt/step_support.py
--rw-r--r--   0 runner    (1001) docker     (127)    13115 2024-04-23 01:36:59.000000 kmt-0.3.0/src/kmt/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     7336 2024-04-23 01:36:59.000000 kmt-0.3.0/src/kmt/yaml_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:37:13.695128 kmt-0.3.0/src/kmt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-23 01:37:13.000000 kmt-0.3.0/src/kmt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-23 01:37:13.000000 kmt-0.3.0/src/kmt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 01:37:13.000000 kmt-0.3.0/src/kmt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-23 01:37:13.000000 kmt-0.3.0/src/kmt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-23 01:37:13.000000 kmt-0.3.0/src/kmt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-23 01:37:13.000000 kmt-0.3.0/src/kmt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:59:27.634597 kmt-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-23 01:59:13.000000 kmt-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-23 01:59:27.634597 kmt-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 01:59:13.000000 kmt-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 01:59:27.634597 kmt-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-23 01:59:13.000000 kmt-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:59:27.630597 kmt-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:59:27.630597 kmt-0.3.1/src/kmt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 01:59:13.000000 kmt-0.3.1/src/kmt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 01:59:13.000000 kmt-0.3.1/src/kmt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-23 01:59:13.000000 kmt-0.3.1/src/kmt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24412 2024-04-23 01:59:13.000000 kmt-0.3.1/src/kmt/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-23 01:59:13.000000 kmt-0.3.1/src/kmt/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-23 01:59:13.000000 kmt-0.3.1/src/kmt/j2support.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11927 2024-04-23 01:59:13.000000 kmt-0.3.1/src/kmt/pipeline_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12658 2024-04-23 01:59:13.000000 kmt-0.3.1/src/kmt/step_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-04-23 01:59:13.000000 kmt-0.3.1/src/kmt/step_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13115 2024-04-23 01:59:13.000000 kmt-0.3.1/src/kmt/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7336 2024-04-23 01:59:13.000000 kmt-0.3.1/src/kmt/yaml_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:59:27.634597 kmt-0.3.1/src/kmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-23 01:59:27.000000 kmt-0.3.1/src/kmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-23 01:59:27.000000 kmt-0.3.1/src/kmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 01:59:27.000000 kmt-0.3.1/src/kmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-23 01:59:27.000000 kmt-0.3.1/src/kmt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-23 01:59:27.000000 kmt-0.3.1/src/kmt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-23 01:59:27.000000 kmt-0.3.1/src/kmt.egg-info/top_level.txt
```

### Comparing `kmt-0.3.0/LICENSE` & `kmt-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kmt-0.3.0/setup.py` & `kmt-0.3.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,14 @@
     "long_description": README,
     "license": "MIT",
     "packages": find_packages(where="src", include=["kmt", "kmt.*"]),
     "author": "Jesse Reichman",
     "keywords": ["Kubernetes", "Manifest", "Transform"],
     "url": "https://github.com/archmachina/kmt",
     "download_url": "https://pypi.org/project/kmt/",
-    "entry_points": {"console_scripts": ["kmt = kmt:main"]},
+    "entry_points": {"console_scripts": ["kmt = kmt.cli:main"]},
     "package_dir": {"": "src"},
     "install_requires": ["PyYAML>=6.0.0", "Jinja2>=3.1.0", "jsonpatch>=1.33", "jsonpath-ng>=1.6.1"],
 }
 
 if __name__ == "__main__":
     setup(**setup_args, include_package_data=True)
```

### Comparing `kmt-0.3.0/src/kmt/__main__.py` & `kmt-0.3.1/src/kmt/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -73,10 +73,7 @@
         ret = process_args()
         sys.stdout.flush()
         sys.exit(ret)
     except Exception as e:  # pylint: disable=broad-exception-caught
         logging.getLogger(__name__).exception(e)
         sys.stdout.flush()
         sys.exit(1)
-
-if __name__ == "__main__":
-    main()
```

### Comparing `kmt-0.3.0/src/kmt/core.py` & `kmt-0.3.1/src/kmt/core.py`

 * *Files identical despite different names*

### Comparing `kmt-0.3.0/src/kmt/exception.py` & `kmt-0.3.1/src/kmt/exception.py`

 * *Files identical despite different names*

### Comparing `kmt-0.3.0/src/kmt/j2support.py` & `kmt-0.3.1/src/kmt/j2support.py`

 * *Files identical despite different names*

### Comparing `kmt-0.3.0/src/kmt/pipeline_support.py` & `kmt-0.3.1/src/kmt/pipeline_support.py`

 * *Files identical despite different names*

### Comparing `kmt-0.3.0/src/kmt/step_handlers.py` & `kmt-0.3.1/src/kmt/step_handlers.py`

 * *Files identical despite different names*

### Comparing `kmt-0.3.0/src/kmt/step_support.py` & `kmt-0.3.1/src/kmt/step_support.py`

 * *Files identical despite different names*

### Comparing `kmt-0.3.0/src/kmt/util.py` & `kmt-0.3.1/src/kmt/util.py`

 * *Files identical despite different names*

### Comparing `kmt-0.3.0/src/kmt/yaml_types.py` & `kmt-0.3.1/src/kmt/yaml_types.py`

 * *Files identical despite different names*

