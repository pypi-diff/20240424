# Comparing `tmp/bondzai.idetect40-interface-0.0.1.tar.gz` & `tmp/bondzai.idetect40-interface-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.idetect40-interface-0.0.1.tar", last modified: Wed Apr 24 10:48:02 2024, max compression
+gzip compressed data, was "bondzai.idetect40-interface-0.0.2.tar", last modified: Wed Apr 24 14:32:44 2024, max compression
```

## Comparing `bondzai.idetect40-interface-0.0.1.tar` & `bondzai.idetect40-interface-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 10:48:02.354300 bondzai.idetect40-interface-0.0.1/
--rw-rw-rw-   0        0        0      547 2023-10-17 12:30:45.000000 bondzai.idetect40-interface-0.0.1/NOTICE
--rw-rw-rw-   0        0        0      805 2024-04-24 10:48:02.354300 bondzai.idetect40-interface-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      360 2024-04-24 10:47:45.000000 bondzai.idetect40-interface-0.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-24 10:48:02.326146 bondzai.idetect40-interface-0.0.1/bondzai/
-drwxrwxrwx   0        0        0        0 2024-04-24 10:48:02.333993 bondzai.idetect40-interface-0.0.1/bondzai/idetect40_interface/
--rw-rw-rw-   0        0        0       22 2024-04-24 10:20:11.000000 bondzai.idetect40-interface-0.0.1/bondzai/idetect40_interface/__init__.py
--rw-rw-rw-   0        0        0     2429 2024-04-24 10:29:44.000000 bondzai.idetect40-interface-0.0.1/bondzai/idetect40_interface/dict.py
--rw-rw-rw-   0        0        0     8417 2024-04-24 08:59:19.000000 bondzai.idetect40-interface-0.0.1/bondzai/idetect40_interface/exchange_table.py
--rw-rw-rw-   0        0        0    11553 2024-04-22 15:43:39.000000 bondzai.idetect40-interface-0.0.1/bondzai/idetect40_interface/socket.py
-drwxrwxrwx   0        0        0        0 2024-04-24 10:48:02.353220 bondzai.idetect40-interface-0.0.1/bondzai.idetect40_interface.egg-info/
--rw-rw-rw-   0        0        0      805 2024-04-24 10:48:02.000000 bondzai.idetect40-interface-0.0.1/bondzai.idetect40_interface.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      883 2024-04-24 10:48:02.000000 bondzai.idetect40-interface-0.0.1/bondzai.idetect40_interface.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 10:48:02.000000 bondzai.idetect40-interface-0.0.1/bondzai.idetect40_interface.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-24 10:48:02.000000 bondzai.idetect40-interface-0.0.1/bondzai.idetect40_interface.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0       28 2024-04-24 10:48:02.000000 bondzai.idetect40-interface-0.0.1/bondzai.idetect40_interface.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-24 10:48:02.000000 bondzai.idetect40-interface-0.0.1/bondzai.idetect40_interface.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-24 10:48:02.000000 bondzai.idetect40-interface-0.0.1/bondzai.idetect40_interface.egg-info/zip-safe
--rw-rw-rw-   0        0        0       71 2023-10-17 12:30:45.000000 bondzai.idetect40-interface-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      733 2024-04-24 10:48:02.355870 bondzai.idetect40-interface-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       36 2023-10-17 12:30:45.000000 bondzai.idetect40-interface-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-24 10:48:02.337059 bondzai.idetect40-interface-0.0.1/tests/
--rw-rw-rw-   0        0        0     2383 2024-04-24 10:29:44.000000 bondzai.idetect40-interface-0.0.1/tests/test_dict.py
--rw-rw-rw-   0        0        0     3586 2024-04-24 10:31:34.000000 bondzai.idetect40-interface-0.0.1/tests/test_exchange_table.py
--rw-rw-rw-   0        0        0     5998 2024-04-24 10:33:37.000000 bondzai.idetect40-interface-0.0.1/tests/test_socket.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:32:44.783136 bondzai.idetect40-interface-0.0.2/
+-rw-rw-rw-   0        0        0      547 2023-10-17 12:30:45.000000 bondzai.idetect40-interface-0.0.2/NOTICE
+-rw-rw-rw-   0        0        0      805 2024-04-24 14:32:44.783687 bondzai.idetect40-interface-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2024-04-24 10:47:45.000000 bondzai.idetect40-interface-0.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-24 14:32:44.761988 bondzai.idetect40-interface-0.0.2/bondzai/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:32:44.769122 bondzai.idetect40-interface-0.0.2/bondzai/idetect40_interface/
+-rw-rw-rw-   0        0        0       22 2024-04-24 14:31:55.000000 bondzai.idetect40-interface-0.0.2/bondzai/idetect40_interface/__init__.py
+-rw-rw-rw-   0        0        0     2429 2024-04-24 10:29:44.000000 bondzai.idetect40-interface-0.0.2/bondzai/idetect40_interface/dict.py
+-rw-rw-rw-   0        0        0    13464 2024-04-24 14:26:44.000000 bondzai.idetect40-interface-0.0.2/bondzai/idetect40_interface/exchange_table.py
+-rw-rw-rw-   0        0        0       66 2024-04-24 13:20:02.000000 bondzai.idetect40-interface-0.0.2/bondzai/idetect40_interface/poc.py
+-rw-rw-rw-   0        0        0    11553 2024-04-22 15:43:39.000000 bondzai.idetect40-interface-0.0.2/bondzai/idetect40_interface/socket.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:32:44.782041 bondzai.idetect40-interface-0.0.2/bondzai.idetect40_interface.egg-info/
+-rw-rw-rw-   0        0        0      805 2024-04-24 14:32:44.000000 bondzai.idetect40-interface-0.0.2/bondzai.idetect40_interface.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      955 2024-04-24 14:32:44.000000 bondzai.idetect40-interface-0.0.2/bondzai.idetect40_interface.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 14:32:44.000000 bondzai.idetect40-interface-0.0.2/bondzai.idetect40_interface.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-24 14:32:44.000000 bondzai.idetect40-interface-0.0.2/bondzai.idetect40_interface.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0       28 2024-04-24 14:32:44.000000 bondzai.idetect40-interface-0.0.2/bondzai.idetect40_interface.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-24 14:32:44.000000 bondzai.idetect40-interface-0.0.2/bondzai.idetect40_interface.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-24 14:32:44.000000 bondzai.idetect40-interface-0.0.2/bondzai.idetect40_interface.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       71 2023-10-17 12:30:45.000000 bondzai.idetect40-interface-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      733 2024-04-24 14:32:44.784844 bondzai.idetect40-interface-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       36 2023-10-17 12:30:45.000000 bondzai.idetect40-interface-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:32:44.771000 bondzai.idetect40-interface-0.0.2/tests/
+-rw-rw-rw-   0        0        0     2383 2024-04-24 10:29:44.000000 bondzai.idetect40-interface-0.0.2/tests/test_dict.py
+-rw-rw-rw-   0        0        0     4578 2024-04-24 14:26:44.000000 bondzai.idetect40-interface-0.0.2/tests/test_exchange_table.py
+-rw-rw-rw-   0        0        0     5998 2024-04-24 10:33:37.000000 bondzai.idetect40-interface-0.0.2/tests/test_socket.py
```

### Comparing `bondzai.idetect40-interface-0.0.1/NOTICE` & `bondzai.idetect40-interface-0.0.2/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.idetect40-interface-0.0.1/PKG-INFO` & `bondzai.idetect40-interface-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.idetect40-interface
-Version: 0.0.1
+Version: 0.0.2
 Summary: Bondzai iDetect 4.0 interface
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,idetect40
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.idetect40-interface-0.0.1/bondzai/idetect40_interface/dict.py` & `bondzai.idetect40-interface-0.0.2/bondzai/idetect40_interface/dict.py`

 * *Files identical despite different names*

### Comparing `bondzai.idetect40-interface-0.0.1/bondzai/idetect40_interface/socket.py` & `bondzai.idetect40-interface-0.0.2/bondzai/idetect40_interface/socket.py`

 * *Files identical despite different names*

### Comparing `bondzai.idetect40-interface-0.0.1/bondzai.idetect40_interface.egg-info/PKG-INFO` & `bondzai.idetect40-interface-0.0.2/bondzai.idetect40_interface.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.idetect40-interface
-Version: 0.0.1
+Version: 0.0.2
 Summary: Bondzai iDetect 4.0 interface
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,idetect40
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.idetect40-interface-0.0.1/bondzai.idetect40_interface.egg-info/SOURCES.txt` & `bondzai.idetect40-interface-0.0.2/bondzai.idetect40_interface.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 ./bondzai/idetect40_interface/__init__.py
 ./bondzai/idetect40_interface/dict.py
 ./bondzai/idetect40_interface/exchange_table.py
+./bondzai/idetect40_interface/poc.py
 ./bondzai/idetect40_interface/socket.py
 ./tests/test_dict.py
 ./tests/test_exchange_table.py
 ./tests/test_socket.py
 bondzai.idetect40_interface.egg-info/PKG-INFO
 bondzai.idetect40_interface.egg-info/SOURCES.txt
 bondzai.idetect40_interface.egg-info/dependency_links.txt
 bondzai.idetect40_interface.egg-info/namespace_packages.txt
 bondzai.idetect40_interface.egg-info/requires.txt
 bondzai.idetect40_interface.egg-info/top_level.txt
 bondzai.idetect40_interface.egg-info/zip-safe
 bondzai/idetect40_interface/__init__.py
 bondzai/idetect40_interface/dict.py
 bondzai/idetect40_interface/exchange_table.py
+bondzai/idetect40_interface/poc.py
 bondzai/idetect40_interface/socket.py
 tests/test_dict.py
 tests/test_exchange_table.py
 tests/test_socket.py
```

### Comparing `bondzai.idetect40-interface-0.0.1/setup.cfg` & `bondzai.idetect40-interface-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `bondzai.idetect40-interface-0.0.1/tests/test_dict.py` & `bondzai.idetect40-interface-0.0.2/tests/test_dict.py`

 * *Files identical despite different names*

### Comparing `bondzai.idetect40-interface-0.0.1/tests/test_exchange_table.py` & `bondzai.idetect40-interface-0.0.2/tests/test_exchange_table.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from bondzai.idetect40_interface.dict import check_dict_equity
-from bondzai.idetect40_interface.exchange_table import ExchangeTableConverter
+from bondzai.idetect40_interface.exchange_table import ExchangeTable, I40Table, PLCTable
 
 
 TEST_DESCRIPTOR = {
     "agents": {
         "nb_sources": 4,
         "nb_agents": 4
     },
@@ -27,59 +26,84 @@
             "name": "over pressure",
             "type": "BOOL",
             "size": 1
         }
     ]
 }
 
-class Test_ExchangeTableConverter():
-    exchange_table_converter = ExchangeTableConverter(TEST_DESCRIPTOR)
+def table_from_dict(descriptor: dict, d: dict) -> ExchangeTable:
+    if "result" in d:
+        table = I40Table(descriptor)
+        table.set_exception_occured(d["system"]["exception_occured"])
+        table.set_exception(d["system"]["exception"])
+        table.set_result(d["result"]["agent_id"], d["result"]["source_id"], d["result"]["key_id"], 
+                         d["result"]["value_id"], d["result"]["category_id"])
+    else:
+        table = PLCTable(descriptor)
+        table.set_ack_result(d["system"]["ack_result"])
+        table.set_ack_exception(d["system"]["ack_exception"])
+    table.set_system_running(d["system"]["running"])
+    table.set_process_ongoing(d["system"]["process_ongoing"])
+    table.set_heart_beat(d["system"]["heart_beat"])
+    for agent_id, agent_dict in d["agents"].items():
+        table.activate_agent(agent_id, agent_dict["active"])
+        for source_id, scr_active in agent_dict["sources"].items():
+            table.activate_source(agent_id, source_id, scr_active)
+    for attribute_name, value in d["attributes"].items():
+        table.set_attribute_value(attribute_name, value)
+    return table
+    
+
+
+class Test_ExchangeTable():
     is_connected = False
     error_code = 7
-    input_table = {
+    input_table_dict = {
         "system": {"running": True, "process_ongoing": False, "heart_beat": False, 
                    "ack_result": True, "ack_exception": True},
         "agents": {
             1: {"active": True, "sources": {1: True, 2: False, 3: True, 4: False}},
             2: {"active": True, "sources": {1: False, 2: False, 3: True, 4: False}},
             3: {"active": False, "sources": {1: True, 2: True, 3: True, 4: False}},
             4: {"active": False, "sources": {1: True, 2: False, 3: True, 4: True}}
         },
         "attributes": {"serial number": 12, "vehicule type": "abc", "temperature": 48.70000076293945, 
                        "over pressure": False}
         }
+    input_table = table_from_dict(TEST_DESCRIPTOR, input_table_dict)
     input_bin_table = bytearray([25, 0, 11, 0, 9, 0, 14, 0, 26, 0, 12, 0, 97, 98, 99, 0, 205, 204, 66, 66, 0, 0])
-    output_table = {
+    output_table_dict = {
         "system": {"running": True, "process_ongoing": False, "heart_beat": False, "exception_occured": True, 
                 "exception": error_code},
         "agents": {
         1: {"active": True, "sources": {1: True, 2: False, 3: True, 4: False}},
         2: {"active": True, "sources": {1: False, 2: False, 3: True, 4: False}},
         3: {"active": False, "sources": {1: True, 2: True, 3: True, 4: False}},
         4: {"active": False, "sources": {1: True, 2: False, 3: True, 4: True}}
         },
         "result": {"agent_id": 1, "source_id": 3, "key_id": 1, "value_id": 6, "category_id": 4},
         "attributes": {"serial number": 12, "vehicule type": "ab", "temperature": 48.70000076293945, 
                        "over pressure": False}
         } 
+    output_table = table_from_dict(TEST_DESCRIPTOR, output_table_dict)
     output_bin_table = bytearray([9, error_code, 11, 0, 9, 0, 14, 0, 26, 0, 1, 3, 1, 6, 4, 0, 12, 0, 97, 98, 0, 0, 205, 
                                   204, 66, 66, 0, 0])
            
     def test_msg_to_table(self):
-        result = self.exchange_table_converter.msg_to_table(self.input_bin_table) 
-        assert check_dict_equity(result, self.input_table)
-        result = self.exchange_table_converter.msg_to_table(self.output_bin_table) 
-        assert check_dict_equity(result, self.output_table)
+        table_from_msg = PLCTable(TEST_DESCRIPTOR, self.input_bin_table)
+        assert self.input_table == table_from_msg
+        table_from_msg = I40Table(TEST_DESCRIPTOR, self.output_bin_table)
+        assert self.output_table == table_from_msg
 
     def test_table_to_msg(self):
-        result = self.exchange_table_converter.table_to_msg(self.input_table) 
+        result = self.input_table.to_msg()
         assert result == self.input_bin_table
-        result = self.exchange_table_converter.table_to_msg(self.output_table) 
+        result = self.output_table.to_msg()
         assert result == self.output_bin_table
     
     def test_get_input_table_size(self):
-        input_size = self.exchange_table_converter.get_input_table_size()
+        input_size = len(self.input_table)
         assert input_size == len(self.input_bin_table)
     
     def test_get_output_table_size(self):
-        output_size = self.exchange_table_converter.get_output_table_size()
+        output_size = len(self.output_table)
         assert output_size == len(self.output_bin_table)
```

### Comparing `bondzai.idetect40-interface-0.0.1/tests/test_socket.py` & `bondzai.idetect40-interface-0.0.2/tests/test_socket.py`

 * *Files identical despite different names*

