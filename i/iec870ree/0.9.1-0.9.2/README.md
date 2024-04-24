# Comparing `tmp/iec870ree-0.9.1.tar.gz` & `tmp/iec870ree-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/iec870ree-0.9.1.tar", last modified: Thu Nov 25 12:49:20 2021, max compression
+gzip compressed data, was "dist/iec870ree-0.9.2.tar", last modified: Thu Dec  9 11:36:52 2021, max compression
```

## Comparing `iec870ree-0.9.1.tar` & `iec870ree-0.9.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2021-11-25 12:49:20.000000 iec870ree-0.9.1/
--rw-rw-r--   0 afita     (1000) afita     (1000)     3993 2021-11-25 12:49:20.000000 iec870ree-0.9.1/PKG-INFO
--rw-r--r--   0 afita     (1000) afita     (1000)      130 2021-11-25 12:49:20.000000 iec870ree-0.9.1/setup.cfg
--rw-r--r--   0 afita     (1000) afita     (1000)     1225 2021-11-25 12:43:41.000000 iec870ree-0.9.1/setup.py
--rw-r--r--   0 afita     (1000) afita     (1000)       34 2021-11-25 12:15:58.000000 iec870ree-0.9.1/requirements-dev.txt
-drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2021-11-25 12:49:20.000000 iec870ree-0.9.1/iec870ree/
--rw-r--r--   0 afita     (1000) afita     (1000)    39149 2021-11-24 18:32:30.000000 iec870ree-0.9.1/iec870ree/app_asdu.py
--rw-r--r--   0 afita     (1000) afita     (1000)     8755 2020-10-28 15:10:44.000000 iec870ree-0.9.1/iec870ree/base_asdu.py
--rw-r--r--   0 afita     (1000) afita     (1000)        0 2020-02-25 16:56:40.000000 iec870ree-0.9.1/iec870ree/__init__.py
--rw-r--r--   0 afita     (1000) afita     (1000)     5273 2020-02-25 16:56:40.000000 iec870ree-0.9.1/iec870ree/modem.py
--rw-rw-r--   0 afita     (1000) afita     (1000)    15369 2021-11-25 12:43:33.000000 iec870ree-0.9.1/iec870ree/protocol.py
--rw-r--r--   0 afita     (1000) afita     (1000)     2817 2020-08-12 11:06:01.000000 iec870ree-0.9.1/iec870ree/ip.py
--rw-r--r--   0 afita     (1000) afita     (1000)    34520 2020-02-25 16:56:40.000000 iec870ree-0.9.1/LICENSE
-drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2021-11-25 12:49:20.000000 iec870ree-0.9.1/iec870ree.egg-info/
--rw-r--r--   0 afita     (1000) afita     (1000)       10 2021-11-25 12:49:20.000000 iec870ree-0.9.1/iec870ree.egg-info/top_level.txt
--rw-r--r--   0 afita     (1000) afita     (1000)      375 2021-11-25 12:49:20.000000 iec870ree-0.9.1/iec870ree.egg-info/SOURCES.txt
--rw-r--r--   0 afita     (1000) afita     (1000)     3993 2021-11-25 12:49:20.000000 iec870ree-0.9.1/iec870ree.egg-info/PKG-INFO
--rw-r--r--   0 afita     (1000) afita     (1000)        1 2021-11-25 12:49:20.000000 iec870ree-0.9.1/iec870ree.egg-info/dependency_links.txt
--rw-r--r--   0 afita     (1000) afita     (1000)       40 2021-11-25 12:49:20.000000 iec870ree-0.9.1/iec870ree.egg-info/requires.txt
--rw-r--r--   0 afita     (1000) afita     (1000)     2837 2020-02-25 16:56:40.000000 iec870ree-0.9.1/README.rst
--rw-r--r--   0 afita     (1000) afita     (1000)       70 2020-02-25 16:56:40.000000 iec870ree-0.9.1/MANIFEST.in
--rw-r--r--   0 afita     (1000) afita     (1000)       40 2020-02-25 16:56:40.000000 iec870ree-0.9.1/requirements.txt
+drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2021-12-09 11:36:52.000000 iec870ree-0.9.2/
+-rw-rw-r--   0 afita     (1000) afita     (1000)     3993 2021-12-09 11:36:52.000000 iec870ree-0.9.2/PKG-INFO
+-rw-r--r--   0 afita     (1000) afita     (1000)      130 2021-12-09 11:36:52.000000 iec870ree-0.9.2/setup.cfg
+-rw-r--r--   0 afita     (1000) afita     (1000)     1225 2021-12-09 10:44:42.000000 iec870ree-0.9.2/setup.py
+-rw-r--r--   0 afita     (1000) afita     (1000)       34 2021-11-25 12:15:58.000000 iec870ree-0.9.2/requirements-dev.txt
+drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2021-12-09 11:36:52.000000 iec870ree-0.9.2/iec870ree/
+-rw-r--r--   0 afita     (1000) afita     (1000)    39149 2021-11-24 18:32:30.000000 iec870ree-0.9.2/iec870ree/app_asdu.py
+-rw-r--r--   0 afita     (1000) afita     (1000)     8755 2020-10-28 15:10:44.000000 iec870ree-0.9.2/iec870ree/base_asdu.py
+-rw-r--r--   0 afita     (1000) afita     (1000)        0 2020-02-25 16:56:40.000000 iec870ree-0.9.2/iec870ree/__init__.py
+-rw-r--r--   0 afita     (1000) afita     (1000)     5273 2020-02-25 16:56:40.000000 iec870ree-0.9.2/iec870ree/modem.py
+-rw-rw-r--   0 afita     (1000) afita     (1000)    16773 2021-12-09 10:44:33.000000 iec870ree-0.9.2/iec870ree/protocol.py
+-rw-r--r--   0 afita     (1000) afita     (1000)     2817 2020-08-12 11:06:01.000000 iec870ree-0.9.2/iec870ree/ip.py
+-rw-r--r--   0 afita     (1000) afita     (1000)    34520 2020-02-25 16:56:40.000000 iec870ree-0.9.2/LICENSE
+drwxrwxr-x   0 afita     (1000) afita     (1000)        0 2021-12-09 11:36:52.000000 iec870ree-0.9.2/iec870ree.egg-info/
+-rw-r--r--   0 afita     (1000) afita     (1000)       10 2021-12-09 11:36:52.000000 iec870ree-0.9.2/iec870ree.egg-info/top_level.txt
+-rw-r--r--   0 afita     (1000) afita     (1000)      375 2021-12-09 11:36:52.000000 iec870ree-0.9.2/iec870ree.egg-info/SOURCES.txt
+-rw-r--r--   0 afita     (1000) afita     (1000)     3993 2021-12-09 11:36:52.000000 iec870ree-0.9.2/iec870ree.egg-info/PKG-INFO
+-rw-r--r--   0 afita     (1000) afita     (1000)        1 2021-12-09 11:36:52.000000 iec870ree-0.9.2/iec870ree.egg-info/dependency_links.txt
+-rw-r--r--   0 afita     (1000) afita     (1000)       40 2021-12-09 11:36:52.000000 iec870ree-0.9.2/iec870ree.egg-info/requires.txt
+-rw-r--r--   0 afita     (1000) afita     (1000)     2837 2020-02-25 16:56:40.000000 iec870ree-0.9.2/README.rst
+-rw-r--r--   0 afita     (1000) afita     (1000)       70 2020-02-25 16:56:40.000000 iec870ree-0.9.2/MANIFEST.in
+-rw-r--r--   0 afita     (1000) afita     (1000)       40 2020-02-25 16:56:40.000000 iec870ree-0.9.2/requirements.txt
```

### Comparing `iec870ree-0.9.1/PKG-INFO` & `iec870ree-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iec870ree
-Version: 0.9.1
+Version: 0.9.2
 Summary: Library to connect and query information about electricmeters following REE protocol.
 Home-page: https://github.com/gisce/iec870ree
 Author: GISCE-TI, S.L.
 Author-email: devel@gisce.net
 License: GNU Affero General Public License v3
 Description: iec870ree
         =========
```

### Comparing `iec870ree-0.9.1/setup.py` & `iec870ree-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     TEST_REQUIRES += ['mock']
 
 with open('README.rst') as f:
     readme = f.read()
 
 setup(
     name="iec870ree",
-    version="0.9.1",
+    version="0.9.2",
     author="GISCE-TI, S.L.",
     author_email="devel@gisce.net",
     description=("Library to connect and query information about electric"
                  "meters following REE protocol."),
     long_description=readme,
     long_description_content_type="text/x-rst",
     url="https://github.com/gisce/iec870ree",
```

### Comparing `iec870ree-0.9.1/iec870ree/app_asdu.py` & `iec870ree-0.9.2/iec870ree/app_asdu.py`

 * *Files identical despite different names*

### Comparing `iec870ree-0.9.1/iec870ree/base_asdu.py` & `iec870ree-0.9.2/iec870ree/base_asdu.py`

 * *Files identical despite different names*

### Comparing `iec870ree-0.9.1/iec870ree/modem.py` & `iec870ree-0.9.2/iec870ree/modem.py`

 * *Files identical despite different names*

### Comparing `iec870ree-0.9.1/iec870ree/protocol.py` & `iec870ree-0.9.2/iec870ree/protocol.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from abc import ABCMeta, abstractmethod
 from .base_asdu import (
     AsduParser, FixedAsdu, VariableAsdu
 )
 from .app_asdu import *
 from .app_asdu import INSTANT_VALUES_OBJECTS
 import math
+from datetime import datetime
 
 from six import with_metaclass
 
 
 logger = logging.getLogger('iec870ree')
 
 
@@ -83,25 +84,56 @@
     def __str__(self):
         return 'Requested ASDU Type Not Available'
 
 class ASDUDirectionUnknown(Exception):
     pass
 
 
+class NoContentTimeoutException(Exception):
+
+    def __str__(self):
+        return 'Timeout: To many Time Without Content'
+
+
 class AppLayer(with_metaclass(ABCMeta)):
 
+    def __init__(self):
+        self.last_content_heartbeat = self.connection_start = datetime.now()
+        self.set_content_timeout(300)  # in seconds
+
+
     def initialize(self, link_layer):
         self.link_layer = link_layer
+        self.last_content_heartbeat = datetime.now()
 
     def send_user_data(self, asdu):
         pass
 
     def get_user_data(self):
         pass
 
+    def set_content_timeout(self, timeout):
+        self.max_content_timeout = timeout
+
+    def reset_content_received(self):
+        logger.info("RESET Last Content Heartbeat, content received")
+        self.last_content_heartbeat = datetime.now()
+
+    def check_content_timeout(self):
+        now = datetime.now()
+        diff = (now - self.last_content_heartbeat).total_seconds()
+        logger.info("Last Content Heartbeat: {} seconds".format(diff))
+        logger.info("TOTAL Current Duration: {} seconds".format(self.get_connection_duration()))
+        if diff > self.max_content_timeout:
+            raise NoContentTimeoutException
+
+    def get_connection_duration(self):
+        now = datetime.now()
+        return (now - self.connection_start).total_seconds()
+
     def process_request(self, request_asdu):
         self.link_layer.send_frame(request_asdu)
         asdu_ack = self.link_layer.get_frame()
         if not asdu_ack:
             raise ProtocolException("Didn't get ACK")
         return self.process_requestresponse()
 
@@ -122,14 +154,15 @@
             asdu_resp = self.link_layer.get_frame()
             if not asdu_resp:
                 logger.error("Did not receive ASDU response.")
                 raise ProtocolException("Didn't get ASDU")
             yield asdu_resp
 
             if not isinstance(asdu_resp, VariableAsdu):
+                self.check_content_timeout()
                 continue
             if asdu_resp.causa_tm == 0x05 and asdu_resp.tipo in [
                 M_TA_VC_2.type, M_TA_VM_2.type, M_IT_TK_2.type, M_IT_TG_2.type,
                 M_IB_TK_2.type]:
                 logger.info("Received request for next batch of information")
             elif asdu_resp.causa_tm == 0x05:
                 logger.info("Request or asked")
@@ -151,14 +184,16 @@
                 raise IntegrationPeriodNotAvailable()
             elif asdu_resp.causa_tm == 0x12:
                 logger.error("Requested integration period not available")
                 raise IntegrationPeriodNotAvailable()
             else:
                 raise Exception('ERROR: Transmission cause unknown: {}'.format(asdu_resp.causa_tm))
 
+            self.check_content_timeout()
+
     def authenticate(self, clave_pm):
         #183
         asdu = self.create_asdu_request(C_AC_NA_2(clave_pm))
         resps = list(self.process_request(asdu))
         return resps[0]
 
     def finish_session(self):
@@ -178,14 +213,15 @@
             raise ValueError
         asdu = self.create_asdu_request(C_CI_NT_2(start_date, end_date),
                                         register)
         #do not remove this as we have to iterate over physical layer frames.
         resps = list(self.process_request(asdu))
         for resp in self.process_requestresponse():
             if resp.tipo == M_IT_TG_2.type:
+                self.reset_content_received()
                 yield resp
 
     def read_incremental_values(self, start_date, end_date, register='profiles'):
         #123
         if register in READINGS_REGISTERS:
             register = READINGS_REGISTERS[register]
         else:
@@ -193,14 +229,15 @@
             raise ValueError
         asdu = self.create_asdu_request(C_CI_NU_2(start_date, end_date),
                                         register)
         #do not remove this as we have to iterate over physical layer frames.
         resps = list(self.process_request(asdu))
         for resp in self.process_requestresponse():
             if isinstance(resp, VariableAsdu) and resp.tipo == M_IT_TK_2.type:
+                self.reset_content_received()
                 yield resp
 
     def read_datetime(self):
         #103
         asdu = self.create_asdu_request(C_TI_NA_2())
         resps = list(self.process_request(asdu))
         for resp in resps:
@@ -222,27 +259,29 @@
         else:
             logger.error("Wrong values for register")
             raise ValueError
         asdu = self.create_asdu_request(C_TA_VC_2(), register)
         resps = list(self.process_request(asdu))
         for resp in self.process_requestresponse():
             if resp.tipo == M_TA_VC_2.type:
+                self.reset_content_received()
                 yield resp
 
     def stored_tariff_info(self, start_date, end_date, register=1):
         #134 stored values
         if register in CONTRACTS_REGISTERS:
             register = CONTRACTS_REGISTERS[register]
         else:
             logger.error("Wrong values for register")
             raise ValueError
         asdu = self.create_asdu_request(C_TA_VM_2(start_date, end_date), register)
         resps = list(self.process_request(asdu))
         for resp in self.process_requestresponse():
             if resp.tipo == M_TA_VM_2.type:
+                self.reset_content_received()
                 yield resp
 
     def get_configuration(self):
         #141
         asdu = self.create_asdu_request(C_RM_NA_2())
         resps = list(self.process_request(asdu))
         for resp in resps:
```

### Comparing `iec870ree-0.9.1/iec870ree/ip.py` & `iec870ree-0.9.2/iec870ree/ip.py`

 * *Files identical despite different names*

### Comparing `iec870ree-0.9.1/LICENSE` & `iec870ree-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iec870ree-0.9.1/iec870ree.egg-info/PKG-INFO` & `iec870ree-0.9.2/iec870ree.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iec870ree
-Version: 0.9.1
+Version: 0.9.2
 Summary: Library to connect and query information about electricmeters following REE protocol.
 Home-page: https://github.com/gisce/iec870ree
 Author: GISCE-TI, S.L.
 Author-email: devel@gisce.net
 License: GNU Affero General Public License v3
 Description: iec870ree
         =========
```

### Comparing `iec870ree-0.9.1/README.rst` & `iec870ree-0.9.2/README.rst`

 * *Files identical despite different names*

