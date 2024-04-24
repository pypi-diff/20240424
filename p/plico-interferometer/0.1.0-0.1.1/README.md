# Comparing `tmp/plico_interferometer-0.1.0.tar.gz` & `tmp/plico_interferometer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plico_interferometer-0.1.0.tar", last modified: Wed Apr 19 16:34:33 2023, max compression
+gzip compressed data, was "plico_interferometer-0.1.1.tar", last modified: Wed Apr 24 10:53:14 2024, max compression
```

## Comparing `plico_interferometer-0.1.0.tar` & `plico_interferometer-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:33.663877 plico_interferometer-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-19 16:34:33.663877 plico_interferometer-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:33.659877 plico_interferometer-0.1.0/plico_interferometer/
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/plico_interferometer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/plico_interferometer/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:33.663877 plico_interferometer-0.1.0/plico_interferometer/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/plico_interferometer/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/plico_interferometer/client/abstract_interferometer_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/plico_interferometer/client/interferometer_WCF_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/plico_interferometer/client/interferometer_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/plico_interferometer/client/simulated_interferometer_client.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/plico_interferometer/client/snapshot_entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:33.663877 plico_interferometer-0.1.0/plico_interferometer/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/plico_interferometer/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/plico_interferometer/types/interferometer_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:33.663877 plico_interferometer-0.1.0/plico_interferometer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/plico_interferometer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/plico_interferometer/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/plico_interferometer/utils/timeout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:33.663877 plico_interferometer-0.1.0/plico_interferometer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-19 16:34:33.000000 plico_interferometer-0.1.0/plico_interferometer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-19 16:34:33.000000 plico_interferometer-0.1.0/plico_interferometer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 16:34:33.000000 plico_interferometer-0.1.0/plico_interferometer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-19 16:34:33.000000 plico_interferometer-0.1.0/plico_interferometer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-19 16:34:33.000000 plico_interferometer-0.1.0/plico_interferometer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 16:34:33.663877 plico_interferometer-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:33.663877 plico_interferometer-0.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/test/fake_time_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)    16662 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/test/test_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:33.663877 plico_interferometer-0.1.0/test/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/test/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-19 16:34:21.000000 plico_interferometer-0.1.0/test/types/interferometer_status_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:53:14.675573 plico_interferometer-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-24 10:53:10.000000 plico_interferometer-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 10:53:10.000000 plico_interferometer-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-24 10:53:14.675573 plico_interferometer-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-24 10:53:10.000000 plico_interferometer-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:53:14.671573 plico_interferometer-0.1.1/plico_interferometer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-24 10:53:10.000000 plico_interferometer-0.1.1/plico_interferometer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-24 10:53:10.000000 plico_interferometer-0.1.1/plico_interferometer/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:53:14.675573 plico_interferometer-0.1.1/plico_interferometer/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:53:10.000000 plico_interferometer-0.1.1/plico_interferometer/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-24 10:53:10.000000 plico_interferometer-0.1.1/plico_interferometer/client/abstract_interferometer_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-24 10:53:10.000000 plico_interferometer-0.1.1/plico_interferometer/client/interferometer_WCF_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-24 10:53:10.000000 plico_interferometer-0.1.1/plico_interferometer/client/interferometer_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-24 10:53:10.000000 plico_interferometer-0.1.1/plico_interferometer/client/simulated_interferometer_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-24 10:53:10.000000 plico_interferometer-0.1.1/plico_interferometer/client/snapshot_entry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:53:14.675573 plico_interferometer-0.1.1/plico_interferometer/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:53:10.000000 plico_interferometer-0.1.1/plico_interferometer/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-24 10:53:10.000000 plico_interferometer-0.1.1/plico_interferometer/types/interferometer_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:53:14.675573 plico_interferometer-0.1.1/plico_interferometer/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:53:10.000000 plico_interferometer-0.1.1/plico_interferometer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-24 10:53:10.000000 plico_interferometer-0.1.1/plico_interferometer/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-24 10:53:10.000000 plico_interferometer-0.1.1/plico_interferometer/utils/timeout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:53:14.675573 plico_interferometer-0.1.1/plico_interferometer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-24 10:53:14.000000 plico_interferometer-0.1.1/plico_interferometer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-24 10:53:14.000000 plico_interferometer-0.1.1/plico_interferometer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:53:14.000000 plico_interferometer-0.1.1/plico_interferometer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 10:53:14.000000 plico_interferometer-0.1.1/plico_interferometer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 10:53:14.000000 plico_interferometer-0.1.1/plico_interferometer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 10:53:14.675573 plico_interferometer-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-24 10:53:10.000000 plico_interferometer-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:53:14.675573 plico_interferometer-0.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:53:10.000000 plico_interferometer-0.1.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-24 10:53:10.000000 plico_interferometer-0.1.1/test/fake_time_mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16662 2024-04-24 10:53:10.000000 plico_interferometer-0.1.1/test/test_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:53:14.675573 plico_interferometer-0.1.1/test/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:53:10.000000 plico_interferometer-0.1.1/test/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-24 10:53:10.000000 plico_interferometer-0.1.1/test/types/interferometer_status_test.py
```

### Comparing `plico_interferometer-0.1.0/LICENSE` & `plico_interferometer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `plico_interferometer-0.1.0/PKG-INFO` & `plico_interferometer-0.1.1/plico_interferometer/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,57 @@
-Metadata-Version: 2.1
-Name: plico_interferometer
-Version: 0.1.0
-Summary: interferometer controller with PLICO
-Home-page: https://github.com/ArcetriAdaptiveOptics/plico_interferometer
-Author: Lorenzo Busoni, Alfio Puglisi
-Author-email: lorenzo.busoni@inaf.it
-License: MIT
-Keywords: plico,interferometer,laboratory,instrumentation control
-Classifier: Development Status :: 4 - Beta
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 2.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# plico_interferometer
-
-client of an interferometer controlled under the plico environment 
-
-
- ![Python package](https://github.com/ArcetriAdaptiveOptics/plico_interferometer/workflows/Python%20package/badge.svg)
- [![codecov](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_interferometer/branch/main/graph/badge.svg?token=ApWOrs49uw)](https://codecov.io/gh/ArcetriAdaptiveOptics/plico_interferometer)
- [![Documentation Status](https://readthedocs.org/projects/plico_interferometer/badge/?version=latest)](https://plico_interferometer.readthedocs.io/en/latest/?badge=latest)
- [![PyPI version](https://badge.fury.io/py/plico-interferometer.svg)](https://badge.fury.io/py/plico-interferometer)
+from plico_interferometer.utils.constants import Constants
 
 
-plico_interferometer is an application to control motors under the [plico][plico] environment.
+def _getDefaultConfigFilePath():
+    from plico.utils.config_file_manager import ConfigFileManager
+    cfgFileMgr = ConfigFileManager(Constants.APP_NAME,
+                                   Constants.APP_AUTHOR,
+                                   Constants.THIS_PACKAGE)
+    return cfgFileMgr.getConfigFilePath()
 
-[plico]: https://github.com/ArcetriAdaptiveOptics/plico
+
+default_config_file_path = _getDefaultConfigFilePath()
+
+
+def interferometer(hostname, port):
+    '''
+    create client of plico interferometer server
+
+    Parameters
+    ----------
+    hostname: string
+        ip address of the computer running the plico interferometer server
+
+    port: integer
+        port of the plico interferometer server, specified in the
+        config file on the plico interferometer server. Typical = 7300
+    '''
+
+    from plico_interferometer.client.interferometer_client import \
+        InterferometerClient
+    from plico.rpc.zmq_remote_procedure_call import ZmqRemoteProcedureCall
+    from plico.rpc.zmq_ports import ZmqPorts
+    from plico.rpc.sockets import Sockets
+
+    rpc = ZmqRemoteProcedureCall()
+    zmqPorts = ZmqPorts(hostname, port)
+    sockets = Sockets(zmqPorts, rpc)
+    return InterferometerClient(rpc, sockets)
+
+
+def interferometer_4SightFocus_client(hostname, port):
+    '''
+    create client of 4SightFocus
+
+    Parameters
+    ----------
+    hostname: string
+        ip address of the computer running the 4SightFocus software
+
+    port: integer
+        port of the 4SightFocus software
+    '''
+    from plico_interferometer.client.interferometer_WCF_client import \
+        InterferometerWCFClient
+
+    interferometer = InterferometerWCFClient(hostname, port)
+    return interferometer
```

### Comparing `plico_interferometer-0.1.0/plico_interferometer/client/abstract_interferometer_client.py` & `plico_interferometer-0.1.1/plico_interferometer/client/abstract_interferometer_client.py`

 * *Files identical despite different names*

### Comparing `plico_interferometer-0.1.0/plico_interferometer/client/interferometer_WCF_client.py` & `plico_interferometer-0.1.1/plico_interferometer/client/interferometer_WCF_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             image_list = []
             for i in range(how_many):
                 width, height, pixel_size_in_microns, data_array = \
                     self._i4d.take_single_measurement()
                 masked_ima = self._fromDataArrayToMaskedArray(
                     width, height, data_array * 632.8e-9)
                 image_list.append(masked_ima)
-            images = np.dstack(image_list)
+            images = np.ma.dstack(image_list)
             masked_ima = np.ma.mean(images, axis=2)
 
         return masked_ima
 
     def _fromDataArrayToMaskedArray(self, width, height, data_array):
         data = np.reshape(data_array, (width, height))
         idx, idy = np.where(np.isnan(data))
```

### Comparing `plico_interferometer-0.1.0/plico_interferometer/client/interferometer_client.py` & `plico_interferometer-0.1.1/plico_interferometer/client/interferometer_client.py`

 * *Files identical despite different names*

### Comparing `plico_interferometer-0.1.0/plico_interferometer/client/simulated_interferometer_client.py` & `plico_interferometer-0.1.1/plico_interferometer/client/simulated_interferometer_client.py`

 * *Files identical despite different names*

### Comparing `plico_interferometer-0.1.0/plico_interferometer.egg-info/SOURCES.txt` & `plico_interferometer-0.1.1/plico_interferometer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plico_interferometer-0.1.0/setup.py` & `plico_interferometer-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `plico_interferometer-0.1.0/test/fake_time_mod.py` & `plico_interferometer-0.1.1/test/fake_time_mod.py`

 * *Files identical despite different names*

### Comparing `plico_interferometer-0.1.0/test/test_helper.py` & `plico_interferometer-0.1.1/test/test_helper.py`

 * *Files identical despite different names*

### Comparing `plico_interferometer-0.1.0/test/types/interferometer_status_test.py` & `plico_interferometer-0.1.1/test/types/interferometer_status_test.py`

 * *Files identical despite different names*

