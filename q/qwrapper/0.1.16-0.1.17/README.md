# Comparing `tmp/qwrapper-0.1.16.tar.gz` & `tmp/qwrapper-0.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwrapper-0.1.16.tar", last modified: Fri Apr 19 15:51:27 2024, max compression
+gzip compressed data, was "qwrapper-0.1.17.tar", last modified: Wed Apr 24 19:44:01 2024, max compression
```

## Comparing `qwrapper-0.1.16.tar` & `qwrapper-0.1.17.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:51:27.303478 qwrapper-0.1.16/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1130 2024-04-19 15:51:22.000000 qwrapper-0.1.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-19 15:51:27.303478 qwrapper-0.1.16/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     1116 2024-04-19 15:51:22.000000 qwrapper-0.1.16/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      586 2024-04-19 15:51:22.000000 qwrapper-0.1.16/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:51:27.303478 qwrapper-0.1.16/qwrapper/
--rwxr-xr-x   0 runner    (1001) docker     (127)       38 2024-04-19 15:51:22.000000 qwrapper-0.1.16/qwrapper/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      752 2024-04-19 15:51:22.000000 qwrapper-0.1.16/qwrapper/qemumachine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:51:27.303478 qwrapper-0.1.16/qwrapper/x86/
--rwxr-xr-x   0 runner    (1001) docker     (127)       34 2024-04-19 15:51:22.000000 qwrapper-0.1.16/qwrapper/x86/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:51:27.303478 qwrapper-0.1.16/qwrapper/x86/utils/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:51:22.000000 qwrapper-0.1.16/qwrapper/x86/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      245 2024-04-19 15:51:22.000000 qwrapper-0.1.16/qwrapper/x86/utils/debugging.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1041 2024-04-19 15:51:22.000000 qwrapper-0.1.16/qwrapper/x86/utils/machinestate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1147 2024-04-19 15:51:22.000000 qwrapper-0.1.16/qwrapper/x86/utils/memory.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2432 2024-04-19 15:51:22.000000 qwrapper-0.1.16/qwrapper/x86/utils/registers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4056 2024-04-19 15:51:22.000000 qwrapper-0.1.16/qwrapper/x86/x86machine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 15:51:27.303478 qwrapper-0.1.16/qwrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-19 15:51:27.000000 qwrapper-0.1.16/qwrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-19 15:51:27.000000 qwrapper-0.1.16/qwrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 15:51:27.000000 qwrapper-0.1.16/qwrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 15:51:27.000000 qwrapper-0.1.16/qwrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 15:51:27.303478 qwrapper-0.1.16/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:01.474137 qwrapper-0.1.17/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1130 2024-04-24 19:43:56.000000 qwrapper-0.1.17/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-24 19:44:01.474137 qwrapper-0.1.17/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1116 2024-04-24 19:43:56.000000 qwrapper-0.1.17/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      626 2024-04-24 19:43:56.000000 qwrapper-0.1.17/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:01.470137 qwrapper-0.1.17/qwrapper/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       38 2024-04-24 19:43:56.000000 qwrapper-0.1.17/qwrapper/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      752 2024-04-24 19:43:56.000000 qwrapper-0.1.17/qwrapper/qemumachine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:01.474137 qwrapper-0.1.17/qwrapper/x86/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       34 2024-04-24 19:43:56.000000 qwrapper-0.1.17/qwrapper/x86/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:01.474137 qwrapper-0.1.17/qwrapper/x86/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:43:56.000000 qwrapper-0.1.17/qwrapper/x86/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      245 2024-04-24 19:43:56.000000 qwrapper-0.1.17/qwrapper/x86/utils/debugging.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1041 2024-04-24 19:43:56.000000 qwrapper-0.1.17/qwrapper/x86/utils/machinestate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1147 2024-04-24 19:43:56.000000 qwrapper-0.1.17/qwrapper/x86/utils/memory.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2432 2024-04-24 19:43:56.000000 qwrapper-0.1.17/qwrapper/x86/utils/registers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4116 2024-04-24 19:43:56.000000 qwrapper-0.1.17/qwrapper/x86/x86machine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:01.474137 qwrapper-0.1.17/qwrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-24 19:44:01.000000 qwrapper-0.1.17/qwrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-24 19:44:01.000000 qwrapper-0.1.17/qwrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:44:01.000000 qwrapper-0.1.17/qwrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-24 19:44:01.000000 qwrapper-0.1.17/qwrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 19:44:01.000000 qwrapper-0.1.17/qwrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:44:01.474137 qwrapper-0.1.17/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:01.474137 qwrapper-0.1.17/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-24 19:43:56.000000 qwrapper-0.1.17/tests/test_qwrapper_x86.py
```

### Comparing `qwrapper-0.1.16/LICENSE` & `qwrapper-0.1.17/LICENSE`

 * *Files identical despite different names*

### Comparing `qwrapper-0.1.16/PKG-INFO` & `qwrapper-0.1.17/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwrapper
-Version: 0.1.16
+Version: 0.1.17
 Summary: A QEMU wrapper for Python
 Author-email: Daniel Dybing <danieldy@uia.no>, Ali Sirvanovitsj Ismailov <alisi18@uia.no>, Sirén Elise Lund Lohre <selohre@uia.no>
 License: MIT License
         
         Copyright (c) 2024 Ali Ismailov, Daniel Dybing, Sirén Elise Lund Lohre
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,14 +26,16 @@
         SOFTWARE.
         
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pygdbmi
+Requires-Dist: qemu.qmp
 
 # QWrapper
 
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/ddybing/qwrapper/pypi-publish.yml)
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/qwrapper)
```

### Comparing `qwrapper-0.1.16/README.md` & `qwrapper-0.1.17/README.md`

 * *Files identical despite different names*

### Comparing `qwrapper-0.1.16/qwrapper/qemumachine.py` & `qwrapper-0.1.17/qwrapper/qemumachine.py`

 * *Files identical despite different names*

### Comparing `qwrapper-0.1.16/qwrapper/x86/utils/machinestate.py` & `qwrapper-0.1.17/qwrapper/x86/utils/machinestate.py`

 * *Files identical despite different names*

### Comparing `qwrapper-0.1.16/qwrapper/x86/utils/memory.py` & `qwrapper-0.1.17/qwrapper/x86/utils/memory.py`

 * *Files identical despite different names*

### Comparing `qwrapper-0.1.16/qwrapper/x86/utils/registers.py` & `qwrapper-0.1.17/qwrapper/x86/utils/registers.py`

 * *Files identical despite different names*

### Comparing `qwrapper-0.1.16/qwrapper/x86/x86machine.py` & `qwrapper-0.1.17/qwrapper/x86/x86machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,31 +12,32 @@
 
 class X86Machine(QemuMachine):
         gdbControl = gdbcontroller.GdbController()
         gdbConnected = False
         qemuCmd = []
         QemuProcess = None
 
-        def __init__(self, disk_images, qmpwait=False,):
+        def __init__(self, disk_images=None, qmpwait=False):
             super().__init__()
 
             self.disk_counter = ord('a') # Initial disk value
 
             if qmpwait == True:
                 self.qemuCmd = ['qemu-system-i386', '-display', 'none', '-S', '-s', '-qmp', 'unix:/tmp/qmp.socket,server=on,wait=on']
             if qmpwait == False:
                 self.qemuCmd = ['qemu-system-i386', '-display', 'none', '-S', '-s', '-qmp', 'unix:/tmp/qmp.socket,server=on,wait=off']
 
-            for image in disk_images:
-                if self.disk_counter > ord('z'):
-                    print("Error: Too many disk images")
-                    break
-                self.qemuCmd.append('-hd' + chr(self.disk_counter))
-                self.qemuCmd.append(image)
-                self.disk_counter += 1
+            if disk_images:
+                for image in disk_images:
+                    if self.disk_counter > ord('z'):
+                        print("Error: Too many disk images")
+                        break
+                    self.qemuCmd.append('-hd' + chr(self.disk_counter))
+                    self.qemuCmd.append(image)
+                    self.disk_counter += 1
             
 
             print("Setting up virtual machine...")
             # Start Qemu with gdb stub and QMP Server. Add the kernel and disk images.
             # Virtual machine starts in "wait" mode. Waits for user to start VM execution.
             self.QemuProcess = subprocess.Popen(self.qemuCmd, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
```

### Comparing `qwrapper-0.1.16/qwrapper.egg-info/PKG-INFO` & `qwrapper-0.1.17/qwrapper.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwrapper
-Version: 0.1.16
+Version: 0.1.17
 Summary: A QEMU wrapper for Python
 Author-email: Daniel Dybing <danieldy@uia.no>, Ali Sirvanovitsj Ismailov <alisi18@uia.no>, Sirén Elise Lund Lohre <selohre@uia.no>
 License: MIT License
         
         Copyright (c) 2024 Ali Ismailov, Daniel Dybing, Sirén Elise Lund Lohre
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,14 +26,16 @@
         SOFTWARE.
         
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pygdbmi
+Requires-Dist: qemu.qmp
 
 # QWrapper
 
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/ddybing/qwrapper/pypi-publish.yml)
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/qwrapper)
```

