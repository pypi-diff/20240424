# Comparing `tmp/remote_mole-1.4.0.tar.gz` & `tmp/remote_mole-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remote_mole-1.4.0.tar", last modified: Tue Oct 17 20:43:55 2023, max compression
+gzip compressed data, was "remote_mole-1.4.1.tar", last modified: Wed Apr 24 21:53:07 2024, max compression
```

## Comparing `remote_mole-1.4.0.tar` & `remote_mole-1.4.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 20:43:55.762481 remote_mole-1.4.0/
--rw-rw-rw-   0 root         (0) root         (0)    34451 2023-10-17 20:43:16.000000 remote_mole-1.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      865 2023-10-17 20:43:55.761481 remote_mole-1.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      534 2023-10-17 20:43:16.000000 remote_mole-1.4.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-10-17 20:43:55.763481 remote_mole-1.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1182 2023-10-17 20:43:16.000000 remote_mole-1.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 20:43:55.744481 remote_mole-1.4.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 20:43:55.747481 remote_mole-1.4.0/src/remote_mole/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 20:43:55.754481 remote_mole-1.4.0/src/remote_mole/_internal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-17 20:43:16.000000 remote_mole-1.4.0/src/remote_mole/_internal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 20:43:55.755481 remote_mole-1.4.0/src/remote_mole/_internal/platforms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-17 20:43:16.000000 remote_mole-1.4.0/src/remote_mole/_internal/platforms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 20:43:55.756481 remote_mole-1.4.0/src/remote_mole/_internal/platforms/discord/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-17 20:43:16.000000 remote_mole-1.4.0/src/remote_mole/_internal/platforms/discord/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7193 2023-10-17 20:43:16.000000 remote_mole-1.4.0/src/remote_mole/_internal/platforms/discord/daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 20:43:55.758481 remote_mole-1.4.0/src/remote_mole/_internal/services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-17 20:43:16.000000 remote_mole-1.4.0/src/remote_mole/_internal/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1920 2023-10-17 20:43:16.000000 remote_mole-1.4.0/src/remote_mole/_internal/services/lxi.py
--rw-rw-rw-   0 root         (0) root         (0)     2459 2023-10-17 20:43:16.000000 remote_mole-1.4.0/src/remote_mole/_internal/services/ngrok.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 20:43:55.760481 remote_mole-1.4.0/src/remote_mole/setup/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-17 20:43:16.000000 remote_mole-1.4.0/src/remote_mole/setup/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4201 2023-10-17 20:43:16.000000 remote_mole-1.4.0/src/remote_mole/setup/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 20:43:55.754481 remote_mole-1.4.0/src/remote_mole.egg-info/
--rw-r--r--   0 root         (0) root         (0)      865 2023-10-17 20:43:55.000000 remote_mole-1.4.0/src/remote_mole.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      661 2023-10-17 20:43:55.000000 remote_mole-1.4.0/src/remote_mole.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-17 20:43:55.000000 remote_mole-1.4.0/src/remote_mole.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-10-17 20:43:55.000000 remote_mole-1.4.0/src/remote_mole.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-10-17 20:43:55.000000 remote_mole-1.4.0/src/remote_mole.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-10-17 20:43:55.000000 remote_mole-1.4.0/src/remote_mole.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 21:53:07.267799 remote_mole-1.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)    34451 2024-04-24 21:52:23.000000 remote_mole-1.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      865 2024-04-24 21:53:07.265798 remote_mole-1.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      534 2024-04-24 21:52:23.000000 remote_mole-1.4.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 21:53:07.267799 remote_mole-1.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2024-04-24 21:52:23.000000 remote_mole-1.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 21:53:07.249798 remote_mole-1.4.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 21:53:07.252798 remote_mole-1.4.1/src/remote_mole/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 21:53:07.259798 remote_mole-1.4.1/src/remote_mole/_internal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 21:52:23.000000 remote_mole-1.4.1/src/remote_mole/_internal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 21:53:07.260799 remote_mole-1.4.1/src/remote_mole/_internal/platforms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 21:52:23.000000 remote_mole-1.4.1/src/remote_mole/_internal/platforms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 21:53:07.261798 remote_mole-1.4.1/src/remote_mole/_internal/platforms/discord/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 21:52:23.000000 remote_mole-1.4.1/src/remote_mole/_internal/platforms/discord/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7349 2024-04-24 21:52:23.000000 remote_mole-1.4.1/src/remote_mole/_internal/platforms/discord/daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 21:53:07.263799 remote_mole-1.4.1/src/remote_mole/_internal/services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 21:52:23.000000 remote_mole-1.4.1/src/remote_mole/_internal/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1920 2024-04-24 21:52:23.000000 remote_mole-1.4.1/src/remote_mole/_internal/services/lxi.py
+-rw-rw-rw-   0 root         (0) root         (0)     2525 2024-04-24 21:52:23.000000 remote_mole-1.4.1/src/remote_mole/_internal/services/ngrok.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 21:53:07.264798 remote_mole-1.4.1/src/remote_mole/setup/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 21:52:23.000000 remote_mole-1.4.1/src/remote_mole/setup/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4201 2024-04-24 21:52:23.000000 remote_mole-1.4.1/src/remote_mole/setup/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 21:53:07.259798 remote_mole-1.4.1/src/remote_mole.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      865 2024-04-24 21:53:07.000000 remote_mole-1.4.1/src/remote_mole.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      661 2024-04-24 21:53:07.000000 remote_mole-1.4.1/src/remote_mole.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 21:53:07.000000 remote_mole-1.4.1/src/remote_mole.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-24 21:53:07.000000 remote_mole-1.4.1/src/remote_mole.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-24 21:53:07.000000 remote_mole-1.4.1/src/remote_mole.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-24 21:53:07.000000 remote_mole-1.4.1/src/remote_mole.egg-info/top_level.txt
```

### Comparing `remote_mole-1.4.0/LICENSE` & `remote_mole-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `remote_mole-1.4.0/PKG-INFO` & `remote_mole-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remote_mole
-Version: 1.4.0
+Version: 1.4.1
 Summary: Create moles on remote setups.
 Home-page: http://packages.python.org/remote_mole
 Author: ACESRG
 Author-email: aces.rg@gmail.com
 License: GPLv3
 Keywords: bots ssh jupyter ngrok discord
 Platform: UNKNOWN
```

### Comparing `remote_mole-1.4.0/README.md` & `remote_mole-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `remote_mole-1.4.0/setup.py` & `remote_mole-1.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="remote_mole",
-    version="1.4.0",
+    version="1.4.1",
     author="ACESRG",
     author_email="aces.rg@gmail.com",
     description=("Create moles on remote setups."),
     license="GPLv3",
     keywords="bots ssh jupyter ngrok discord",
     url="http://packages.python.org/remote_mole",
     packages=[
@@ -24,15 +24,15 @@
             where='src/remote_mole'
         )
     ],
     package_dir={'': 'src'},
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     install_requires=[
-        'pyngrok==5.0.5',
+        'pyngrok==7.1.6',
         'discord.py==1.7.3',
         'questionary==2.0.1',
         'pillow==10.1.0',
     ],
 
     entry_points={
         'console_scripts': [
```

### Comparing `remote_mole-1.4.0/src/remote_mole/_internal/platforms/discord/daemon.py` & `remote_mole-1.4.1/src/remote_mole/_internal/platforms/discord/daemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 SUPPORTED_TUNNELS = (
     'ssh',
     'custom',
     'jupyter',
     'grafana',
     'camera',
+    'vnc'
 )
 
 
 def _format_string_as_code(string):
     return f'`{string}`'
 
 
@@ -78,14 +79,18 @@
             f'You can access a web server on -> http://{tunnel.address} or '
             f'you can access a live feed at http://{tunnel.address}/html'
         )
     elif tunnel_type == 'custom':
         return _format_string_as_code(
             f'The port 1209 was open on: {tunnel.address}'
         )
+    elif tunnel_type == 'vnc':
+        return _format_string_as_code(
+            f'You can access the device vnc on: {tunnel.address}'
+        )
     else:
         return _format_string_as_code(
             f'The port was open on: {tunnel.address}'
         )
 
 
 @bot.command()
```

### Comparing `remote_mole-1.4.0/src/remote_mole/_internal/services/lxi.py` & `remote_mole-1.4.1/src/remote_mole/_internal/services/lxi.py`

 * *Files identical despite different names*

### Comparing `remote_mole-1.4.0/src/remote_mole/_internal/services/ngrok.py` & `remote_mole-1.4.1/src/remote_mole/_internal/services/ngrok.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,18 @@
     'grafana': {
         'port': 3000,
         'proto': 'http',
     },
     'camera': {
         'port': 56000,
         'proto': 'http',
+    },
+    'vnc': {
+        'port': 5900,
+        'proto': 'tcp',
     }
 }
 HOST = 'localhost'
 
 
 def _get_addr_from_url(url):
     return url.split("//")[-1].split(":")[0]
```

### Comparing `remote_mole-1.4.0/src/remote_mole/setup/entrypoint.py` & `remote_mole-1.4.1/src/remote_mole/setup/entrypoint.py`

 * *Files identical despite different names*

### Comparing `remote_mole-1.4.0/src/remote_mole.egg-info/PKG-INFO` & `remote_mole-1.4.1/src/remote_mole.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remote-mole
-Version: 1.4.0
+Version: 1.4.1
 Summary: Create moles on remote setups.
 Home-page: http://packages.python.org/remote_mole
 Author: ACESRG
 Author-email: aces.rg@gmail.com
 License: GPLv3
 Keywords: bots ssh jupyter ngrok discord
 Platform: UNKNOWN
```

### Comparing `remote_mole-1.4.0/src/remote_mole.egg-info/SOURCES.txt` & `remote_mole-1.4.1/src/remote_mole.egg-info/SOURCES.txt`

 * *Files identical despite different names*

