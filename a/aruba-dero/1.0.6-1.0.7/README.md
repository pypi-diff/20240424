# Comparing `tmp/aruba_dero-1.0.6.tar.gz` & `tmp/aruba_dero-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aruba_dero-1.0.6.tar", last modified: Fri Apr 19 11:34:57 2024, max compression
+gzip compressed data, was "aruba_dero-1.0.7.tar", last modified: Wed Apr 24 08:34:16 2024, max compression
```

## Comparing `aruba_dero-1.0.6.tar` & `aruba_dero-1.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:34:57.655728 aruba_dero-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-19 11:34:57.655728 aruba_dero-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-19 11:34:53.000000 aruba_dero-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-19 11:34:53.000000 aruba_dero-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 11:34:57.655728 aruba_dero-1.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:34:57.651728 aruba_dero-1.0.6/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-04-19 11:34:53.000000 aruba_dero-1.0.6/src/Module.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 11:34:53.000000 aruba_dero-1.0.6/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:34:57.655728 aruba_dero-1.0.6/src/aruba_dero.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-19 11:34:57.000000 aruba_dero-1.0.6/src/aruba_dero.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-19 11:34:57.000000 aruba_dero-1.0.6/src/aruba_dero.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 11:34:57.000000 aruba_dero-1.0.6/src/aruba_dero.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-19 11:34:57.000000 aruba_dero-1.0.6/src/aruba_dero.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-19 11:34:57.000000 aruba_dero-1.0.6/src/aruba_dero.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 11:34:57.000000 aruba_dero-1.0.6/src/aruba_dero.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:34:57.651728 aruba_dero-1.0.6/src/dero-modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 11:34:53.000000 aruba_dero-1.0.6/src/dero-modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:34:57.655728 aruba_dero-1.0.6/src/dero-modules/clearpass/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 11:34:53.000000 aruba_dero-1.0.6/src/dero-modules/clearpass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15281 2024-04-19 11:34:53.000000 aruba_dero-1.0.6/src/dero-modules/clearpass/clearpass.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-19 11:34:53.000000 aruba_dero-1.0.6/src/dero-modules/clearpass/module.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-19 11:34:53.000000 aruba_dero-1.0.6/src/dero-modules/clearpass/temp_webserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-04-19 11:34:53.000000 aruba_dero-1.0.6/src/dero-modules/clearpass/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-19 11:34:53.000000 aruba_dero-1.0.6/src/dero-modules/clearpass/webserver-process.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-19 11:34:53.000000 aruba_dero-1.0.6/src/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-19 11:34:53.000000 aruba_dero-1.0.6/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:34:16.368844 aruba_dero-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-24 08:34:16.368844 aruba_dero-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-24 08:34:05.000000 aruba_dero-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-24 08:34:05.000000 aruba_dero-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 08:34:16.368844 aruba_dero-1.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:34:16.364844 aruba_dero-1.0.7/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-04-24 08:34:05.000000 aruba_dero-1.0.7/src/Module.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:34:05.000000 aruba_dero-1.0.7/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:34:16.368844 aruba_dero-1.0.7/src/aruba_dero.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-24 08:34:16.000000 aruba_dero-1.0.7/src/aruba_dero.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-24 08:34:16.000000 aruba_dero-1.0.7/src/aruba_dero.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:34:16.000000 aruba_dero-1.0.7/src/aruba_dero.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-24 08:34:16.000000 aruba_dero-1.0.7/src/aruba_dero.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-24 08:34:16.000000 aruba_dero-1.0.7/src/aruba_dero.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-24 08:34:16.000000 aruba_dero-1.0.7/src/aruba_dero.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:34:16.364844 aruba_dero-1.0.7/src/dero-modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:34:05.000000 aruba_dero-1.0.7/src/dero-modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:34:16.368844 aruba_dero-1.0.7/src/dero-modules/clearpass/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:34:05.000000 aruba_dero-1.0.7/src/dero-modules/clearpass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15273 2024-04-24 08:34:05.000000 aruba_dero-1.0.7/src/dero-modules/clearpass/clearpass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-24 08:34:05.000000 aruba_dero-1.0.7/src/dero-modules/clearpass/module.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-24 08:34:05.000000 aruba_dero-1.0.7/src/dero-modules/clearpass/temp_webserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-04-24 08:34:05.000000 aruba_dero-1.0.7/src/dero-modules/clearpass/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-24 08:34:05.000000 aruba_dero-1.0.7/src/dero-modules/clearpass/webserver-process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-24 08:34:05.000000 aruba_dero-1.0.7/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-24 08:34:05.000000 aruba_dero-1.0.7/src/utils.py
```

### Comparing `aruba_dero-1.0.6/PKG-INFO` & `aruba_dero-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aruba-dero
-Version: 1.0.6
+Version: 1.0.7
 Summary: DEmo ROllout helper - Modular Tool to automate demo rollouts
 Author-email: Lukas Lanzner <lukas.lanzner@hpe.com>
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 Requires-Dist: pyclearpass>=1.0.4
 Requires-Dist: psutil~=5.9.8
 Requires-Dist: pyyaml~=6.0.1
```

### Comparing `aruba_dero-1.0.6/README.md` & `aruba_dero-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `aruba_dero-1.0.6/pyproject.toml` & `aruba_dero-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aruba-dero"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
     { name = "Lukas Lanzner", email = "lukas.lanzner@hpe.com" },
 ]
 description = "DEmo ROllout helper - Modular Tool to automate demo rollouts"
 readme = "README.md"
 requires-python = ">=3.12"
 dependencies = [
```

### Comparing `aruba_dero-1.0.6/src/Module.py` & `aruba_dero-1.0.7/src/Module.py`

 * *Files identical despite different names*

### Comparing `aruba_dero-1.0.6/src/aruba_dero.egg-info/PKG-INFO` & `aruba_dero-1.0.7/src/aruba_dero.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aruba-dero
-Version: 1.0.6
+Version: 1.0.7
 Summary: DEmo ROllout helper - Modular Tool to automate demo rollouts
 Author-email: Lukas Lanzner <lukas.lanzner@hpe.com>
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 Requires-Dist: pyclearpass>=1.0.4
 Requires-Dist: psutil~=5.9.8
 Requires-Dist: pyyaml~=6.0.1
```

### Comparing `aruba_dero-1.0.6/src/aruba_dero.egg-info/SOURCES.txt` & `aruba_dero-1.0.7/src/aruba_dero.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aruba_dero-1.0.6/src/dero-modules/clearpass/clearpass.py` & `aruba_dero-1.0.7/src/dero-modules/clearpass/clearpass.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
                 return False
 
             if webserver.host == "0.0.0.0":
 
                 webhost = os.environ.get("CPPM_CERT_SERVE_HOST") or Input("Enter host ip: ", default=f"{utils.get_net_ifaces()[-1].get("ip4")}", word_color=colors.foreground["yellow"]).launch()
                 webhost += f":{webserver.port}"
             else:
-                webhost = f"https://{webserver.host}:{webserver.port}"
+                webhost = f"{webserver.host}:{webserver.port}"
 
             print(f"Serving on http://{webserver.host}:{webserver.port}...")
 
             body = {
                 "certificate_url": f"http://{webhost}/{pathlib.PurePath(os.path.relpath(certificate_file, start=self.serve_dir)).as_posix()}",
                 "pkcs12_file_url": f"http://{webhost}/{pathlib.PurePath(os.path.relpath(key_file, start=self.serve_dir)).as_posix()}",
                 "pkcs12_passphrase": f"{self.passphrase}",
```

### Comparing `aruba_dero-1.0.6/src/dero-modules/clearpass/temp_webserver.py` & `aruba_dero-1.0.7/src/dero-modules/clearpass/temp_webserver.py`

 * *Files identical despite different names*

### Comparing `aruba_dero-1.0.6/src/dero-modules/clearpass/utils.py` & `aruba_dero-1.0.7/src/dero-modules/clearpass/utils.py`

 * *Files identical despite different names*

### Comparing `aruba_dero-1.0.6/src/dero-modules/clearpass/webserver-process.py` & `aruba_dero-1.0.7/src/dero-modules/clearpass/webserver-process.py`

 * *Files identical despite different names*

### Comparing `aruba_dero-1.0.6/src/main.py` & `aruba_dero-1.0.7/src/main.py`

 * *Files identical despite different names*

### Comparing `aruba_dero-1.0.6/src/utils.py` & `aruba_dero-1.0.7/src/utils.py`

 * *Files identical despite different names*

