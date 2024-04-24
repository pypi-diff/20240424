# Comparing `tmp/SideJITServer-1.3.0.tar.gz` & `tmp/sidejitserver-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SideJITServer-1.3.0.tar", last modified: Fri Apr 12 08:33:49 2024, max compression
+gzip compressed data, was "sidejitserver-1.3.1.tar", last modified: Wed Apr 24 05:01:18 2024, max compression
```

## Comparing `SideJITServer-1.3.0.tar` & `sidejitserver-1.3.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:49.841055 SideJITServer-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-12 08:33:33.000000 SideJITServer-1.3.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:49.837055 SideJITServer-1.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:49.837055 SideJITServer-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-12 08:33:33.000000 SideJITServer-1.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-12 08:33:33.000000 SideJITServer-1.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-12 08:33:33.000000 SideJITServer-1.3.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-12 08:33:49.841055 SideJITServer-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-12 08:33:33.000000 SideJITServer-1.3.0/README.Docker.md
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-12 08:33:33.000000 SideJITServer-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:49.837055 SideJITServer-1.3.0/SideJITServer/
--rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-04-12 08:33:33.000000 SideJITServer-1.3.0/SideJITServer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-12 08:33:33.000000 SideJITServer-1.3.0/SideJITServer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-12 08:33:49.000000 SideJITServer-1.3.0/SideJITServer/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:49.841055 SideJITServer-1.3.0/SideJITServer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-12 08:33:49.000000 SideJITServer-1.3.0/SideJITServer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-12 08:33:49.000000 SideJITServer-1.3.0/SideJITServer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 08:33:49.000000 SideJITServer-1.3.0/SideJITServer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-12 08:33:49.000000 SideJITServer-1.3.0/SideJITServer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-12 08:33:49.000000 SideJITServer-1.3.0/SideJITServer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-12 08:33:49.000000 SideJITServer-1.3.0/SideJITServer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-12 08:33:33.000000 SideJITServer-1.3.0/compose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-12 08:33:33.000000 SideJITServer-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-12 08:33:33.000000 SideJITServer-1.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 08:33:49.841055 SideJITServer-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:01:18.528153 sidejitserver-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-24 05:01:07.000000 sidejitserver-1.3.1/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:01:18.524153 sidejitserver-1.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:01:18.524153 sidejitserver-1.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-24 05:01:07.000000 sidejitserver-1.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-24 05:01:07.000000 sidejitserver-1.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-24 05:01:07.000000 sidejitserver-1.3.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-24 05:01:18.528153 sidejitserver-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-24 05:01:07.000000 sidejitserver-1.3.1/README.Docker.md
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-24 05:01:07.000000 sidejitserver-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:01:18.524153 sidejitserver-1.3.1/SideJITServer/
+-rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-04-24 05:01:07.000000 sidejitserver-1.3.1/SideJITServer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 05:01:07.000000 sidejitserver-1.3.1/SideJITServer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-24 05:01:18.000000 sidejitserver-1.3.1/SideJITServer/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:01:18.528153 sidejitserver-1.3.1/SideJITServer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-24 05:01:18.000000 sidejitserver-1.3.1/SideJITServer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-24 05:01:18.000000 sidejitserver-1.3.1/SideJITServer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 05:01:18.000000 sidejitserver-1.3.1/SideJITServer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-24 05:01:18.000000 sidejitserver-1.3.1/SideJITServer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-24 05:01:18.000000 sidejitserver-1.3.1/SideJITServer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 05:01:18.000000 sidejitserver-1.3.1/SideJITServer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-24 05:01:07.000000 sidejitserver-1.3.1/compose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-24 05:01:07.000000 sidejitserver-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-24 05:01:07.000000 sidejitserver-1.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 05:01:18.528153 sidejitserver-1.3.1/setup.cfg
```

### Comparing `SideJITServer-1.3.0/.dockerignore` & `sidejitserver-1.3.1/.dockerignore`

 * *Files identical despite different names*

### Comparing `SideJITServer-1.3.0/.github/workflows/python-publish.yml` & `sidejitserver-1.3.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `SideJITServer-1.3.0/.gitignore` & `sidejitserver-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `SideJITServer-1.3.0/Dockerfile` & `sidejitserver-1.3.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `SideJITServer-1.3.0/PKG-INFO` & `sidejitserver-1.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SideJITServer
-Version: 1.3.0
+Version: 1.3.1
 Summary: SideJITServer is an iOS 17 JIT enabler for Windows/macOS!
 Author: khanhduytran0
 Author-email: nythepegasus <me@nythepegas.us>, JoeMatt <git@joemattiello.com>
 Maintainer-email: nythepegasus <me@nythepegas.us>
 Project-URL: Homepage, https://github.com/nythepegasus/SideJITServer
 Project-URL: Bug Reports, https://github.com/nythepegasus/SideJITServer/issues
 Keywords: ios,automation,cli,jit
@@ -17,22 +17,24 @@
 Classifier: Operating System :: iOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: pymobiledevice3<3.5.0,>=3.4.0
+Requires-Dist: pymobiledevice3<4.3.0,>=4.2.3
+Requires-Dist: pymobiledevice3>=3.4.0
 Requires-Dist: Flask==3.0.2
+Requires-Dist: zeroconf==0.132.2
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 
 # SideJITServer
-This project allows you to start a server that wirelessly gives you JIT for iOS 17+ on Windows/macOS. Linux support depends on a [kernel patch](https://github.com/doronz88/pymobiledevice3/issues/566#issuecomment-1850486679).
+This project allows you to start a server that wirelessly or via USB gives you JIT for iOS 17+ on Windows/macOS/Linux if you use the correct newer pymobiledevice3 version.
 
 
 To get it going: (run this in an admin terminal if you're on Windows)
 ```sh
 python3 -m venv venv
 
 # If you're on macOS/Linux
@@ -42,15 +44,15 @@
 # CMD
 .\venv\Scripts\Activate.bat
 
 # All
 pip3 install -r requirements.txt
 # Windows
 .\venv\Scripts\python3.exe main.py
-# macOS
+# macOS/Linux
 sudo python3 -m SideJITServer --help
 ```
 
 Or with PyPI:
 ```
 python3 -m venv venv
 # Activate venv..
```

### Comparing `SideJITServer-1.3.0/README.md` & `sidejitserver-1.3.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SideJITServer
-This project allows you to start a server that wirelessly gives you JIT for iOS 17+ on Windows/macOS. Linux support depends on a [kernel patch](https://github.com/doronz88/pymobiledevice3/issues/566#issuecomment-1850486679).
+This project allows you to start a server that wirelessly or via USB gives you JIT for iOS 17+ on Windows/macOS/Linux if you use the correct newer pymobiledevice3 version.
 
 
 To get it going: (run this in an admin terminal if you're on Windows)
 ```sh
 python3 -m venv venv
 
 # If you're on macOS/Linux
@@ -13,15 +13,15 @@
 # CMD
 .\venv\Scripts\Activate.bat
 
 # All
 pip3 install -r requirements.txt
 # Windows
 .\venv\Scripts\python3.exe main.py
-# macOS
+# macOS/Linux
 sudo python3 -m SideJITServer --help
 ```
 
 Or with PyPI:
 ```
 python3 -m venv venv
 # Activate venv..
```

### Comparing `SideJITServer-1.3.0/SideJITServer/__init__.py` & `sidejitserver-1.3.1/SideJITServer/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import click
 import socket
 import logging
 import inquirer3
 import multiprocessing
 from time import sleep
 from flask import Flask
+from zeroconf import ServiceInfo, Zeroconf
 
 from pymobiledevice3.remote.common import TunnelProtocol
 from pymobiledevice3.exceptions import AlreadyMountedError
 from pymobiledevice3.usbmux import select_devices_by_connection_type
 from pymobiledevice3.lockdown import LockdownClient, create_using_usbmux
 from pymobiledevice3.services.installation_proxy import InstallationProxyService
 from pymobiledevice3.services.mobile_image_mounter import auto_mount_personalized
@@ -175,14 +176,39 @@
     device_question = [inquirer3.List('device', message='choose device', choices=device_list, carousel=True)]
     try:
         result = inquirer3.prompt(device_question, raise_keyboard_interrupt=True)
         return result['device']
     except KeyboardInterrupt:
         raise Exception()
 
+def create_service(port=8080):
+    # Get local IP address
+    s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+    s.connect(("8.8.8.8", 80))
+    ip_address = s.getsockname()[0]
+    s.close()
+
+    # Create a unique service name
+    service_name = "SideJITServer._http._tcp.local."
+    service_info = ServiceInfo(
+        "_http._tcp.local.",
+        service_name,
+        addresses=[socket.inet_aton(ip_address)],
+        port=port,
+        properties={'path': '/SideJITServer/'},
+    )
+
+    zeroconf = Zeroconf()
+    print(f"Registration of service {service_name} in progress...")
+    zeroconf.register_service(service_info)
+    print(f"Service {service_name} registered")
+
+    atexit.register(zeroconf.unregister_service, service_info)
+    atexit.register(zeroconf.close)
+
 @click.command()
 @click.option('-p', '--port', default=8080, help='Set the server port')
 @click.option('-e', '--version', is_flag=True, default=False, help='Prints the versions of pymobiledevice3 and SideJITServer')
 @click.option('-d', '--debug', is_flag=True, default=False, help='Enables debug output of the flask server')
 @click.option('-t', '--timeout', default=10, help='The number of seconds to wait for the pymd3 admin tunnel')
 @click.option('-v', '--verbose', default=0, count=True, help='Increase verbosity (-v for INFO, -vv for DEBUG)')
 @click.option('-y', '--pair', is_flag=True, default=False, help='Alternate pairing mode, will wait to pair to 1 device')
@@ -210,19 +236,19 @@
         dev.pair()
         if "y" not in input("Continue? [y/N]: ").lower():
             return
 
     log_levels = [logging.WARNING, logging.INFO, logging.DEBUG]
     verbosity_level = min(len(log_levels) - 1, verbose)
     logging.getLogger().setLevel(log_levels[verbosity_level])
-
     if not tunnel:
         tunneld = multiprocessing.Process(target=start_tunneld_proc)
         tunneld.start()
 
         atexit.register(tunneld.terminate)
 
         sleep(timeout)
 
     refresh_devs()
 
+    create_service()
     app.run(host='0.0.0.0', port=port, debug=debug)
```

### Comparing `SideJITServer-1.3.0/SideJITServer.egg-info/PKG-INFO` & `sidejitserver-1.3.1/SideJITServer.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SideJITServer
-Version: 1.3.0
+Version: 1.3.1
 Summary: SideJITServer is an iOS 17 JIT enabler for Windows/macOS!
 Author: khanhduytran0
 Author-email: nythepegasus <me@nythepegas.us>, JoeMatt <git@joemattiello.com>
 Maintainer-email: nythepegasus <me@nythepegas.us>
 Project-URL: Homepage, https://github.com/nythepegasus/SideJITServer
 Project-URL: Bug Reports, https://github.com/nythepegasus/SideJITServer/issues
 Keywords: ios,automation,cli,jit
@@ -17,22 +17,24 @@
 Classifier: Operating System :: iOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: pymobiledevice3<3.5.0,>=3.4.0
+Requires-Dist: pymobiledevice3<4.3.0,>=4.2.3
+Requires-Dist: pymobiledevice3>=3.4.0
 Requires-Dist: Flask==3.0.2
+Requires-Dist: zeroconf==0.132.2
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 
 # SideJITServer
-This project allows you to start a server that wirelessly gives you JIT for iOS 17+ on Windows/macOS. Linux support depends on a [kernel patch](https://github.com/doronz88/pymobiledevice3/issues/566#issuecomment-1850486679).
+This project allows you to start a server that wirelessly or via USB gives you JIT for iOS 17+ on Windows/macOS/Linux if you use the correct newer pymobiledevice3 version.
 
 
 To get it going: (run this in an admin terminal if you're on Windows)
 ```sh
 python3 -m venv venv
 
 # If you're on macOS/Linux
@@ -42,15 +44,15 @@
 # CMD
 .\venv\Scripts\Activate.bat
 
 # All
 pip3 install -r requirements.txt
 # Windows
 .\venv\Scripts\python3.exe main.py
-# macOS
+# macOS/Linux
 sudo python3 -m SideJITServer --help
 ```
 
 Or with PyPI:
 ```
 python3 -m venv venv
 # Activate venv..
```

### Comparing `SideJITServer-1.3.0/compose.yaml` & `sidejitserver-1.3.1/compose.yaml`

 * *Files identical despite different names*

### Comparing `SideJITServer-1.3.0/pyproject.toml` & `sidejitserver-1.3.1/pyproject.toml`

 * *Files identical despite different names*

