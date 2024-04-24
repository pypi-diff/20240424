# Comparing `tmp/swanspawner-1.1.3.tar.gz` & `tmp/swanspawner-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swanspawner-1.1.3.tar", last modified: Tue Jan 30 10:33:16 2024, max compression
+gzip compressed data, was "swanspawner-1.2.0.tar", last modified: Wed Apr 24 13:01:14 2024, max compression
```

## Comparing `swanspawner-1.1.3.tar` & `swanspawner-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 10:33:16.936402 swanspawner-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-01-30 10:33:06.000000 swanspawner-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-01-30 10:33:16.936402 swanspawner-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-01-30 10:33:06.000000 swanspawner-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-01-30 10:33:06.000000 swanspawner-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 10:33:16.936402 swanspawner-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-01-30 10:33:06.000000 swanspawner-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 10:33:16.936402 swanspawner-1.1.3/swanspawner/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-01-30 10:33:06.000000 swanspawner-1.1.3/swanspawner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-01-30 10:33:06.000000 swanspawner-1.1.3/swanspawner/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    14641 2024-01-30 10:33:06.000000 swanspawner-1.1.3/swanspawner/swandockerspawner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-01-30 10:33:06.000000 swanspawner-1.1.3/swanspawner/swankubespawner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8979 2024-01-30 10:33:06.000000 swanspawner-1.1.3/swanspawner/swanspawner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 10:33:16.936402 swanspawner-1.1.3/swanspawner/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-01-30 10:33:06.000000 swanspawner-1.1.3/swanspawner/templates/options_form_template.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 10:33:16.936402 swanspawner-1.1.3/swanspawner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-01-30 10:33:16.000000 swanspawner-1.1.3/swanspawner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-01-30 10:33:16.000000 swanspawner-1.1.3/swanspawner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 10:33:16.000000 swanspawner-1.1.3/swanspawner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 10:33:16.000000 swanspawner-1.1.3/swanspawner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-01-30 10:33:16.000000 swanspawner-1.1.3/swanspawner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-30 10:33:16.000000 swanspawner-1.1.3/swanspawner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:14.890463 swanspawner-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-24 13:01:05.000000 swanspawner-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-24 13:01:14.890463 swanspawner-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-24 13:01:05.000000 swanspawner-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-24 13:01:05.000000 swanspawner-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:01:14.890463 swanspawner-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-24 13:01:05.000000 swanspawner-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:14.886463 swanspawner-1.2.0/swanspawner/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-24 13:01:05.000000 swanspawner-1.2.0/swanspawner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-24 13:01:05.000000 swanspawner-1.2.0/swanspawner/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14641 2024-04-24 13:01:05.000000 swanspawner-1.2.0/swanspawner/swandockerspawner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-04-24 13:01:05.000000 swanspawner-1.2.0/swanspawner/swankubespawner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8979 2024-04-24 13:01:05.000000 swanspawner-1.2.0/swanspawner/swanspawner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:14.890463 swanspawner-1.2.0/swanspawner/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-04-24 13:01:05.000000 swanspawner-1.2.0/swanspawner/templates/options_form_template.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:01:14.890463 swanspawner-1.2.0/swanspawner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-24 13:01:14.000000 swanspawner-1.2.0/swanspawner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-24 13:01:14.000000 swanspawner-1.2.0/swanspawner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:01:14.000000 swanspawner-1.2.0/swanspawner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:01:14.000000 swanspawner-1.2.0/swanspawner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-24 13:01:14.000000 swanspawner-1.2.0/swanspawner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 13:01:14.000000 swanspawner-1.2.0/swanspawner.egg-info/top_level.txt
```

### Comparing `swanspawner-1.1.3/PKG-INFO` & `swanspawner-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swanspawner
-Version: 1.1.3
+Version: 1.2.0
 Summary: SWAN JupyterHub spawner
 Home-page: https://github.com/swan-cern/jupyterhub-extensions
 Author: SWAN Admins
 License: AGPL-3.0
 Keywords: JupyterHub,Spawner,SWAN,CERN
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `swanspawner-1.1.3/README.md` & `swanspawner-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `swanspawner-1.1.3/setup.py` & `swanspawner-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `swanspawner-1.1.3/swanspawner/swandockerspawner.py` & `swanspawner-1.2.0/swanspawner/swandockerspawner.py`

 * *Files identical despite different names*

### Comparing `swanspawner-1.1.3/swanspawner/swankubespawner.py` & `swanspawner-1.2.0/swanspawner/swankubespawner.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,24 +21,14 @@
         help='URL of the CentOS7 user image.'
     )
 
     async def start(self):
         """Perform extra configurations required for SWAN session spawning in
         kubernetes.
         """
-
-        if self._gpu_requested():
-            self.extra_resource_guarantees["nvidia.com/gpu"] = "1"
-            self.extra_resource_limits["nvidia.com/gpu"] = "1"
-        elif "nvidia.com/gpu" in self.extra_resource_guarantees:
-            del self.extra_resource_guarantees["nvidia.com/gpu"]
-            del self.extra_resource_limits["nvidia.com/gpu"]
-
-        # Resource requests and limits for user pods
-
         # CPU limit is set to what the user selects in the form
         # The request (guarantee) is statically set in the chart;
         # the resulting overcommit is acceptable since users stay idle
         # most of the time
         self.cpu_limit = self.user_options[self.user_n_cores]
 
         # Memory limit is set to what the user selects in the form
@@ -95,23 +85,7 @@
                     # Delete Kubernetes secret with Hadoop delegation tokens
                     hadoop_secret_name = f'hadoop-tokens-{username}'
                     self.log.info(f'Deleting secret {namespace}:{hadoop_secret_name}')
                     try:
                         await self.api.delete_namespaced_secret(hadoop_secret_name, namespace)
                     except ApiException as e:
                         self.log.error('Error deleting secret {namespace}:{hadoop_secret_name}: {e}')
-
-    def get_env(self):
-        """ Set base environmental variables for swan jupyter docker image """
-        env = super().get_env()
-
-        if self._gpu_requested():
-            env.update(dict(
-                # Configure OpenCL to use NVIDIA backend
-                OCL_ICD_FILENAMES = 'libnvidia-opencl.so.1',
-            ))
-
-        return env
-
-    def _gpu_requested(self):
-        """Returns true if the user requested a GPU"""
-        return "cu" in self.user_options[self.lcg_rel_field]
```

### Comparing `swanspawner-1.1.3/swanspawner/swanspawner.py` & `swanspawner-1.2.0/swanspawner/swanspawner.py`

 * *Files identical despite different names*

### Comparing `swanspawner-1.1.3/swanspawner/templates/options_form_template.html` & `swanspawner-1.2.0/swanspawner/templates/options_form_template.html`

 * *Files identical despite different names*

### Comparing `swanspawner-1.1.3/swanspawner.egg-info/PKG-INFO` & `swanspawner-1.2.0/swanspawner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swanspawner
-Version: 1.1.3
+Version: 1.2.0
 Summary: SWAN JupyterHub spawner
 Home-page: https://github.com/swan-cern/jupyterhub-extensions
 Author: SWAN Admins
 License: AGPL-3.0
 Keywords: JupyterHub,Spawner,SWAN,CERN
 Platform: Linux
 Platform: Mac OS X
```

