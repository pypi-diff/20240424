# Comparing `tmp/openobd_protocol-0.0.39.tar.gz` & `tmp/openobd_protocol-0.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openobd_protocol-0.0.39.tar", last modified: Tue Apr 23 10:19:50 2024, max compression
+gzip compressed data, was "openobd_protocol-0.0.40.tar", last modified: Wed Apr 24 13:12:16 2024, max compression
```

## Comparing `openobd_protocol-0.0.39.tar` & `openobd_protocol-0.0.40.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:19:50.472398 openobd_protocol-0.0.39/
--rw-r--r--   0 root         (0) root         (0)     1066 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2457 2024-04-23 10:19:50.472398 openobd_protocol-0.0.39/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      241 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/README.md
--rw-r--r--   0 root         (0) root         (0)     1895 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 10:19:50.472398 openobd_protocol-0.0.39/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:19:50.454398 openobd_protocol-0.0.39/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:19:50.463398 openobd_protocol-0.0.39/src/openobd_protocol/
--rw-r--r--   0 root         (0) root         (0)     1745 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/Authentication_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/Authentication_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1234 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/BasicResponse_pb2.py
--rw-r--r--   0 root         (0) root         (0)      504 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/BasicResponse_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     5065 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/BusConfiguration_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6043 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/BusConfiguration_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:19:50.466398 openobd_protocol-0.0.39/src/openobd_protocol/CAN/
--rw-r--r--   0 root         (0) root         (0)     2103 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/CAN/CanServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      462 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/CAN/CanServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     4415 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/CAN/CanServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2636 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/CAN/Isotp_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2500 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/CAN/Isotp_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2349 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/RemoteDiagnosticServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      405 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/RemoteDiagnosticServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     8395 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:19:50.469398 openobd_protocol-0.0.39/src/openobd_protocol/SessionController/
--rw-r--r--   0 root         (0) root         (0)     2169 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/SessionController/SessionServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      265 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/SessionController/SessionServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     9730 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     1713 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/SessionController/Session_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1449 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/SessionController/Session_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1712 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/Status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1203 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/Status_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:19:50.471398 openobd_protocol-0.0.39/src/openobd_protocol/UserInterface/
--rw-r--r--   0 root         (0) root         (0)     1748 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      273 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2973 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3920 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/UserInterface/UserInterface_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4208 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:19:50.471398 openobd_protocol-0.0.39/src/openobd_protocol.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2457 2024-04-23 10:19:50.000000 openobd_protocol-0.0.39/src/openobd_protocol.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1610 2024-04-23 10:19:50.000000 openobd_protocol-0.0.39/src/openobd_protocol.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 10:19:50.000000 openobd_protocol-0.0.39/src/openobd_protocol.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2024-04-23 10:19:50.000000 openobd_protocol-0.0.39/src/openobd_protocol.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-23 10:19:50.000000 openobd_protocol-0.0.39/src/openobd_protocol.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:12:16.930296 openobd_protocol-0.0.40/
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-24 13:12:16.929296 openobd_protocol-0.0.40/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      241 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/README.md
+-rw-r--r--   0 root         (0) root         (0)     1895 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 13:12:16.930296 openobd_protocol-0.0.40/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:12:16.905295 openobd_protocol-0.0.40/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:12:16.916295 openobd_protocol-0.0.40/src/openobd_protocol/
+-rw-r--r--   0 root         (0) root         (0)     1745 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/Authentication_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/Authentication_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1359 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/BasicResponse_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      598 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/BasicResponse_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     5065 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/BusConfiguration_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6043 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/BusConfiguration_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:12:16.921296 openobd_protocol-0.0.40/src/openobd_protocol/CAN/
+-rw-r--r--   0 root         (0) root         (0)     1978 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/CAN/CanServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      462 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/CAN/CanServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2751 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/CAN/CanServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2565 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/CAN/Isotp_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2400 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/CAN/Isotp_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2349 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/RemoteDiagnosticServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      405 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/RemoteDiagnosticServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     8395 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:12:16.924296 openobd_protocol-0.0.40/src/openobd_protocol/SessionController/
+-rw-r--r--   0 root         (0) root         (0)     2460 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/SessionController/SessionServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      334 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/SessionController/SessionServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    10370 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2492 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/SessionController/Session_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2430 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/SessionController/Session_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1712 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/Status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/Status_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:12:16.928296 openobd_protocol-0.0.40/src/openobd_protocol/UserInterface/
+-rw-r--r--   0 root         (0) root         (0)     1748 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      273 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2973 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3920 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/UserInterface/UserInterface_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4208 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-24 13:12:12.000000 openobd_protocol-0.0.40/src/openobd_protocol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:12:16.929296 openobd_protocol-0.0.40/src/openobd_protocol.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-24 13:12:16.000000 openobd_protocol-0.0.40/src/openobd_protocol.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1610 2024-04-24 13:12:16.000000 openobd_protocol-0.0.40/src/openobd_protocol.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 13:12:16.000000 openobd_protocol-0.0.40/src/openobd_protocol.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2024-04-24 13:12:16.000000 openobd_protocol-0.0.40/src/openobd_protocol.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-24 13:12:16.000000 openobd_protocol-0.0.40/src/openobd_protocol.egg-info/top_level.txt
```

### Comparing `openobd_protocol-0.0.39/LICENSE` & `openobd_protocol-0.0.40/LICENSE`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.39/PKG-INFO` & `openobd_protocol-0.0.40/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openobd-protocol
-Version: 0.0.39
+Version: 0.0.40
 Summary: Jifeline Networks OpenOBD Protocol Buffers gRPC
 Author-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 Maintainer-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 License: Copyright (c) 2024 Jifeline Networks B.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `openobd_protocol-0.0.39/pyproject.toml` & `openobd_protocol-0.0.40/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.39/src/openobd_protocol/Authentication_pb2.py` & `openobd_protocol-0.0.40/src/openobd_protocol/Authentication_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.39/src/openobd_protocol/Authentication_pb2.pyi` & `openobd_protocol-0.0.40/src/openobd_protocol/Authentication_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.39/src/openobd_protocol/BasicResponse_pb2.py` & `openobd_protocol-0.0.40/src/openobd_protocol/BasicResponse_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$openobd_protocol/BasicResponse.proto\x12\x1d\x63om.jifeline.OpenOBD.Protocol\"-\n\x06Result\x12\x0e\n\x06result\x18\x01 \x01(\r\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\tB\x02P\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$openobd_protocol/BasicResponse.proto\x12\x1d\x63om.jifeline.OpenOBD.Protocol\"-\n\x06Result\x12\x0e\n\x06result\x18\x01 \x01(\r\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\"\x0e\n\x0c\x45mptyRequestB\x02P\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'openobd_protocol.BasicResponse_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'P\001'
   _globals['_RESULT']._serialized_start=71
   _globals['_RESULT']._serialized_end=116
+  _globals['_EMPTYREQUEST']._serialized_start=118
+  _globals['_EMPTYREQUEST']._serialized_end=132
 # @@protoc_insertion_point(module_scope)
```

### Comparing `openobd_protocol-0.0.39/src/openobd_protocol/BusConfiguration_pb2.py` & `openobd_protocol-0.0.40/src/openobd_protocol/BusConfiguration_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.39/src/openobd_protocol/BusConfiguration_pb2.pyi` & `openobd_protocol-0.0.40/src/openobd_protocol/BusConfiguration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.39/src/openobd_protocol/CAN/CanServices_pb2.py` & `openobd_protocol-0.0.40/src/openobd_protocol/CAN/CanServices_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 from openobd_protocol import Authentication_pb2 as openobd__protocol_dot_Authentication__pb2
 from openobd_protocol import BasicResponse_pb2 as openobd__protocol_dot_BasicResponse__pb2
 from openobd_protocol import BusConfiguration_pb2 as openobd__protocol_dot_BusConfiguration__pb2
 from openobd_protocol import Status_pb2 as openobd__protocol_dot_Status__pb2
 from openobd_protocol.CAN import Isotp_pb2 as openobd__protocol_dot_CAN_dot_Isotp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&openobd_protocol/CAN/CanServices.proto\x12!com.jifeline.OpenOBD.Protocol.CAN\x1a%openobd_protocol/Authentication.proto\x1a$openobd_protocol/BasicResponse.proto\x1a\'openobd_protocol/BusConfiguration.proto\x1a\x1dopenobd_protocol/Status.proto\x1a openobd_protocol/CAN/Isotp.proto2\xf0\x01\n\x0b\x43\x61nServices\x12j\n\x04send\x12/.com.jifeline.OpenOBD.Protocol.CAN.IsotpMessage\x1a/.com.jifeline.OpenOBD.Protocol.CAN.IsotpMessage\"\x00\x12u\n\x0bopenChannel\x12/.com.jifeline.OpenOBD.Protocol.CAN.IsotpMessage\x1a/.com.jifeline.OpenOBD.Protocol.CAN.IsotpMessage\"\x00(\x01\x30\x01\x42\x02P\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&openobd_protocol/CAN/CanServices.proto\x12!com.jifeline.OpenOBD.Protocol.CAN\x1a%openobd_protocol/Authentication.proto\x1a$openobd_protocol/BasicResponse.proto\x1a\'openobd_protocol/BusConfiguration.proto\x1a\x1dopenobd_protocol/Status.proto\x1a openobd_protocol/CAN/Isotp.proto2\x84\x01\n\x0b\x43\x61nServices\x12u\n\x0bopenChannel\x12/.com.jifeline.OpenOBD.Protocol.CAN.IsotpMessage\x1a/.com.jifeline.OpenOBD.Protocol.CAN.IsotpMessage\"\x00(\x01\x30\x01\x42\x02P\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'openobd_protocol.CAN.CanServices_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'P\001'
   _globals['_CANSERVICES']._serialized_start=261
-  _globals['_CANSERVICES']._serialized_end=501
+  _globals['_CANSERVICES']._serialized_end=393
 # @@protoc_insertion_point(module_scope)
```

### Comparing `openobd_protocol-0.0.39/src/openobd_protocol/CAN/CanServices_pb2_grpc.py` & `openobd_protocol-0.0.40/src/openobd_protocol/CAN/CanServices_pb2_grpc.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,49 +10,33 @@
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.send = channel.unary_unary(
-                '/com.jifeline.OpenOBD.Protocol.CAN.CanServices/send',
-                request_serializer=openobd__protocol_dot_CAN_dot_Isotp__pb2.IsotpMessage.SerializeToString,
-                response_deserializer=openobd__protocol_dot_CAN_dot_Isotp__pb2.IsotpMessage.FromString,
-                )
         self.openChannel = channel.stream_stream(
                 '/com.jifeline.OpenOBD.Protocol.CAN.CanServices/openChannel',
                 request_serializer=openobd__protocol_dot_CAN_dot_Isotp__pb2.IsotpMessage.SerializeToString,
                 response_deserializer=openobd__protocol_dot_CAN_dot_Isotp__pb2.IsotpMessage.FromString,
                 )
 
 
 class CanServicesServicer(object):
     """Missing associated documentation comment in .proto file."""
 
-    def send(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
     def openChannel(self, request_iterator, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_CanServicesServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'send': grpc.unary_unary_rpc_method_handler(
-                    servicer.send,
-                    request_deserializer=openobd__protocol_dot_CAN_dot_Isotp__pb2.IsotpMessage.FromString,
-                    response_serializer=openobd__protocol_dot_CAN_dot_Isotp__pb2.IsotpMessage.SerializeToString,
-            ),
             'openChannel': grpc.stream_stream_rpc_method_handler(
                     servicer.openChannel,
                     request_deserializer=openobd__protocol_dot_CAN_dot_Isotp__pb2.IsotpMessage.FromString,
                     response_serializer=openobd__protocol_dot_CAN_dot_Isotp__pb2.IsotpMessage.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
@@ -61,31 +45,14 @@
 
 
  # This class is part of an EXPERIMENTAL API.
 class CanServices(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def send(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/com.jifeline.OpenOBD.Protocol.CAN.CanServices/send',
-            openobd__protocol_dot_CAN_dot_Isotp__pb2.IsotpMessage.SerializeToString,
-            openobd__protocol_dot_CAN_dot_Isotp__pb2.IsotpMessage.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
     def openChannel(request_iterator,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `openobd_protocol-0.0.39/src/openobd_protocol/CAN/Isotp_pb2.py` & `openobd_protocol-0.0.40/src/openobd_protocol/CAN/Isotp_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from openobd_protocol import Status_pb2 as openobd__protocol_dot_Status__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n openobd_protocol/CAN/Isotp.proto\x12!com.jifeline.OpenOBD.Protocol.CAN\x1a\x1dopenobd_protocol/Status.proto\"\x8c\x02\n\x0cIsotpMessage\x12@\n\x07\x63hannel\x18\x01 \x01(\x0b\x32/.com.jifeline.OpenOBD.Protocol.CAN.IsotpChannel\x12\x0f\n\x07payload\x18\x02 \x01(\t\x12\x14\n\x07timeout\x18\x03 \x01(\rH\x00\x88\x01\x01\x12\x1c\n\x0fignore_response\x18\x04 \x01(\x08H\x01\x88\x01\x01\x12\x42\n\x0emessage_status\x18\x05 \x01(\x0b\x32%.com.jifeline.OpenOBD.Protocol.StatusH\x02\x88\x01\x01\x42\n\n\x08_timeoutB\x12\n\x10_ignore_responseB\x11\n\x0f_message_status\"\xa1\x02\n\x0cIsotpChannel\x12\x10\n\x08\x62us_name\x18\x01 \x01(\t\x12\x12\n\nrequest_id\x18\x02 \x01(\r\x12\x13\n\x0bresponse_id\x18\x03 \x01(\r\x12%\n\x18\x65xtended_request_address\x18\x04 \x01(\rH\x00\x88\x01\x01\x12&\n\x19\x65xtended_response_address\x18\x05 \x01(\rH\x01\x88\x01\x01\x12@\n\x07padding\x18\x06 \x01(\x0e\x32*.com.jifeline.OpenOBD.Protocol.CAN.PaddingH\x02\x88\x01\x01\x42\x1b\n\x19_extended_request_addressB\x1c\n\x1a_extended_response_addressB\n\n\x08_padding*\x99\x01\n\x07Padding\x12\x15\n\x11PADDING_UNDEFINED\x10\x00\x12\x13\n\x0fPADDING_ENABLED\x10\x01\x12\x15\n\x11PADDING_DETECTION\x10\x02\x12\x14\n\x10PADDING_DISABLED\x10\x03\x12\x18\n\x14PADDING_SET_FROM_ECU\x10\x04\x12\x1b\n\x17PADDING_SET_TOWARDS_ECU\x10\x05\x42\x02P\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n openobd_protocol/CAN/Isotp.proto\x12!com.jifeline.OpenOBD.Protocol.CAN\x1a\x1dopenobd_protocol/Status.proto\"\xea\x01\n\x0cIsotpMessage\x12@\n\x07\x63hannel\x18\x01 \x01(\x0b\x32/.com.jifeline.OpenOBD.Protocol.CAN.IsotpChannel\x12\x0f\n\x07payload\x18\x02 \x01(\t\x12\x1c\n\x0fignore_response\x18\x04 \x01(\x08H\x00\x88\x01\x01\x12\x42\n\x0emessage_status\x18\x05 \x01(\x0b\x32%.com.jifeline.OpenOBD.Protocol.StatusH\x01\x88\x01\x01\x42\x12\n\x10_ignore_responseB\x11\n\x0f_message_status\"\xa1\x02\n\x0cIsotpChannel\x12\x10\n\x08\x62us_name\x18\x01 \x01(\t\x12\x12\n\nrequest_id\x18\x02 \x01(\r\x12\x13\n\x0bresponse_id\x18\x03 \x01(\r\x12%\n\x18\x65xtended_request_address\x18\x04 \x01(\rH\x00\x88\x01\x01\x12&\n\x19\x65xtended_response_address\x18\x05 \x01(\rH\x01\x88\x01\x01\x12@\n\x07padding\x18\x06 \x01(\x0e\x32*.com.jifeline.OpenOBD.Protocol.CAN.PaddingH\x02\x88\x01\x01\x42\x1b\n\x19_extended_request_addressB\x1c\n\x1a_extended_response_addressB\n\n\x08_padding*\x99\x01\n\x07Padding\x12\x15\n\x11PADDING_UNDEFINED\x10\x00\x12\x13\n\x0fPADDING_ENABLED\x10\x01\x12\x15\n\x11PADDING_DETECTION\x10\x02\x12\x14\n\x10PADDING_DISABLED\x10\x03\x12\x18\n\x14PADDING_SET_FROM_ECU\x10\x04\x12\x1b\n\x17PADDING_SET_TOWARDS_ECU\x10\x05\x42\x02P\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'openobd_protocol.CAN.Isotp_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'P\001'
-  _globals['_PADDING']._serialized_start=666
-  _globals['_PADDING']._serialized_end=819
+  _globals['_PADDING']._serialized_start=632
+  _globals['_PADDING']._serialized_end=785
   _globals['_ISOTPMESSAGE']._serialized_start=103
-  _globals['_ISOTPMESSAGE']._serialized_end=371
-  _globals['_ISOTPCHANNEL']._serialized_start=374
-  _globals['_ISOTPCHANNEL']._serialized_end=663
+  _globals['_ISOTPMESSAGE']._serialized_end=337
+  _globals['_ISOTPCHANNEL']._serialized_start=340
+  _globals['_ISOTPCHANNEL']._serialized_end=629
 # @@protoc_insertion_point(module_scope)
```

### Comparing `openobd_protocol-0.0.39/src/openobd_protocol/CAN/Isotp_pb2.pyi` & `openobd_protocol-0.0.40/src/openobd_protocol/CAN/Isotp_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -18,26 +18,24 @@
 PADDING_ENABLED: Padding
 PADDING_DETECTION: Padding
 PADDING_DISABLED: Padding
 PADDING_SET_FROM_ECU: Padding
 PADDING_SET_TOWARDS_ECU: Padding
 
 class IsotpMessage(_message.Message):
-    __slots__ = ("channel", "payload", "timeout", "ignore_response", "message_status")
+    __slots__ = ("channel", "payload", "ignore_response", "message_status")
     CHANNEL_FIELD_NUMBER: _ClassVar[int]
     PAYLOAD_FIELD_NUMBER: _ClassVar[int]
-    TIMEOUT_FIELD_NUMBER: _ClassVar[int]
     IGNORE_RESPONSE_FIELD_NUMBER: _ClassVar[int]
     MESSAGE_STATUS_FIELD_NUMBER: _ClassVar[int]
     channel: IsotpChannel
     payload: str
-    timeout: int
     ignore_response: bool
     message_status: _Status_pb2.Status
-    def __init__(self, channel: _Optional[_Union[IsotpChannel, _Mapping]] = ..., payload: _Optional[str] = ..., timeout: _Optional[int] = ..., ignore_response: bool = ..., message_status: _Optional[_Union[_Status_pb2.Status, _Mapping]] = ...) -> None: ...
+    def __init__(self, channel: _Optional[_Union[IsotpChannel, _Mapping]] = ..., payload: _Optional[str] = ..., ignore_response: bool = ..., message_status: _Optional[_Union[_Status_pb2.Status, _Mapping]] = ...) -> None: ...
 
 class IsotpChannel(_message.Message):
     __slots__ = ("bus_name", "request_id", "response_id", "extended_request_address", "extended_response_address", "padding")
     BUS_NAME_FIELD_NUMBER: _ClassVar[int]
     REQUEST_ID_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_ID_FIELD_NUMBER: _ClassVar[int]
     EXTENDED_REQUEST_ADDRESS_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `openobd_protocol-0.0.39/src/openobd_protocol/RemoteDiagnosticServices_pb2.py` & `openobd_protocol-0.0.40/src/openobd_protocol/RemoteDiagnosticServices_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from openobd_protocol import Authentication_pb2 as openobd__protocol_dot_Authentication__pb2
 from openobd_protocol import BasicResponse_pb2 as openobd__protocol_dot_BasicResponse__pb2
 from openobd_protocol import BusConfiguration_pb2 as openobd__protocol_dot_BusConfiguration__pb2
 from openobd_protocol import Status_pb2 as openobd__protocol_dot_Status__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/openobd_protocol/RemoteDiagnosticServices.proto\x12\x1d\x63om.jifeline.OpenOBD.Protocol\x1a%openobd_protocol/Authentication.proto\x1a$openobd_protocol/BasicResponse.proto\x1a\'openobd_protocol/BusConfiguration.proto\x1a\x1dopenobd_protocol/Status.proto2\xfa\x03\n\x18RemoteDiagnosticServices\x12h\n\x0c\x63onfigureBus\x12/.com.jifeline.OpenOBD.Protocol.BusConfiguration\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x12l\n\x0e\x63onfigureBuses\x12/.com.jifeline.OpenOBD.Protocol.BusConfiguration\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00(\x01\x12}\n\x0c\x41uthenticate\x12\x34.com.jifeline.OpenOBD.Protocol.AuthenticationRequest\x1a\x35.com.jifeline.OpenOBD.Protocol.AuthenticationResponse\"\x00\x12\x86\x01\n\x15RefreshAuthentication\x12\x34.com.jifeline.OpenOBD.Protocol.AuthenticationRequest\x1a\x35.com.jifeline.OpenOBD.Protocol.AuthenticationResponse\"\x00\x42\x02P\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/openobd_protocol/RemoteDiagnosticServices.proto\x12\x1d\x63om.jifeline.OpenOBD.Protocol\x1a%openobd_protocol/Authentication.proto\x1a$openobd_protocol/BasicResponse.proto\x1a\'openobd_protocol/BusConfiguration.proto\x1a\x1dopenobd_protocol/Status.proto2\xfa\x03\n\x18RemoteDiagnosticServices\x12h\n\x0c\x63onfigureBus\x12/.com.jifeline.OpenOBD.Protocol.BusConfiguration\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x12l\n\x0e\x63onfigureBuses\x12/.com.jifeline.OpenOBD.Protocol.BusConfiguration\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00(\x01\x12}\n\x0c\x61uthenticate\x12\x34.com.jifeline.OpenOBD.Protocol.AuthenticationRequest\x1a\x35.com.jifeline.OpenOBD.Protocol.AuthenticationResponse\"\x00\x12\x86\x01\n\x15refreshAuthentication\x12\x34.com.jifeline.OpenOBD.Protocol.AuthenticationRequest\x1a\x35.com.jifeline.OpenOBD.Protocol.AuthenticationResponse\"\x00\x42\x02P\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'openobd_protocol.RemoteDiagnosticServices_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'P\001'
```

### Comparing `openobd_protocol-0.0.39/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py` & `openobd_protocol-0.0.40/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,21 +22,21 @@
                 response_deserializer=openobd__protocol_dot_Status__pb2.Status.FromString,
                 )
         self.configureBuses = channel.stream_unary(
                 '/com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices/configureBuses',
                 request_serializer=openobd__protocol_dot_BusConfiguration__pb2.BusConfiguration.SerializeToString,
                 response_deserializer=openobd__protocol_dot_Status__pb2.Status.FromString,
                 )
-        self.Authenticate = channel.unary_unary(
-                '/com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices/Authenticate',
+        self.authenticate = channel.unary_unary(
+                '/com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices/authenticate',
                 request_serializer=openobd__protocol_dot_Authentication__pb2.AuthenticationRequest.SerializeToString,
                 response_deserializer=openobd__protocol_dot_Authentication__pb2.AuthenticationResponse.FromString,
                 )
-        self.RefreshAuthentication = channel.unary_unary(
-                '/com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices/RefreshAuthentication',
+        self.refreshAuthentication = channel.unary_unary(
+                '/com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices/refreshAuthentication',
                 request_serializer=openobd__protocol_dot_Authentication__pb2.AuthenticationRequest.SerializeToString,
                 response_deserializer=openobd__protocol_dot_Authentication__pb2.AuthenticationResponse.FromString,
                 )
 
 
 class RemoteDiagnosticServicesServicer(object):
     """Missing associated documentation comment in .proto file."""
@@ -49,21 +49,21 @@
 
     def configureBuses(self, request_iterator, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def Authenticate(self, request, context):
+    def authenticate(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def RefreshAuthentication(self, request, context):
+    def refreshAuthentication(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_RemoteDiagnosticServicesServicer_to_server(servicer, server):
@@ -74,21 +74,21 @@
                     response_serializer=openobd__protocol_dot_Status__pb2.Status.SerializeToString,
             ),
             'configureBuses': grpc.stream_unary_rpc_method_handler(
                     servicer.configureBuses,
                     request_deserializer=openobd__protocol_dot_BusConfiguration__pb2.BusConfiguration.FromString,
                     response_serializer=openobd__protocol_dot_Status__pb2.Status.SerializeToString,
             ),
-            'Authenticate': grpc.unary_unary_rpc_method_handler(
-                    servicer.Authenticate,
+            'authenticate': grpc.unary_unary_rpc_method_handler(
+                    servicer.authenticate,
                     request_deserializer=openobd__protocol_dot_Authentication__pb2.AuthenticationRequest.FromString,
                     response_serializer=openobd__protocol_dot_Authentication__pb2.AuthenticationResponse.SerializeToString,
             ),
-            'RefreshAuthentication': grpc.unary_unary_rpc_method_handler(
-                    servicer.RefreshAuthentication,
+            'refreshAuthentication': grpc.unary_unary_rpc_method_handler(
+                    servicer.refreshAuthentication,
                     request_deserializer=openobd__protocol_dot_Authentication__pb2.AuthenticationRequest.FromString,
                     response_serializer=openobd__protocol_dot_Authentication__pb2.AuthenticationResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
@@ -129,39 +129,39 @@
         return grpc.experimental.stream_unary(request_iterator, target, '/com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices/configureBuses',
             openobd__protocol_dot_BusConfiguration__pb2.BusConfiguration.SerializeToString,
             openobd__protocol_dot_Status__pb2.Status.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def Authenticate(request,
+    def authenticate(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices/Authenticate',
+        return grpc.experimental.unary_unary(request, target, '/com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices/authenticate',
             openobd__protocol_dot_Authentication__pb2.AuthenticationRequest.SerializeToString,
             openobd__protocol_dot_Authentication__pb2.AuthenticationResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def RefreshAuthentication(request,
+    def refreshAuthentication(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices/RefreshAuthentication',
+        return grpc.experimental.unary_unary(request, target, '/com.jifeline.OpenOBD.Protocol.RemoteDiagnosticServices/refreshAuthentication',
             openobd__protocol_dot_Authentication__pb2.AuthenticationRequest.SerializeToString,
             openobd__protocol_dot_Authentication__pb2.AuthenticationResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `openobd_protocol-0.0.39/src/openobd_protocol/SessionController/SessionServices_pb2.py` & `openobd_protocol-0.0.40/src/openobd_protocol/SessionController/SessionServices_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,20 +10,21 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from openobd_protocol import Status_pb2 as openobd__protocol_dot_Status__pb2
 from openobd_protocol.SessionController import Session_pb2 as openobd__protocol_dot_SessionController_dot_Session__pb2
+from openobd_protocol import BasicResponse_pb2 as openobd__protocol_dot_BasicResponse__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n8openobd_protocol/SessionController/SessionServices.proto\x12/com.jifeline.OpenOBD.Protocol.SessionController\x1a\x1dopenobd_protocol/Status.proto\x1a\x30openobd_protocol/SessionController/Session.proto2\xa4\x04\n\x0fSessionServices\x12\x61\n\x0fgetSessionToken\x12%.com.jifeline.OpenOBD.Protocol.Status\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x12\x8e\x01\n\rcreateSession\x12=.com.jifeline.OpenOBD.Protocol.SessionController.startSession\x1a<.com.jifeline.OpenOBD.Protocol.SessionController.sessionInfo\"\x00\x12\\\n\ngetSession\x12%.com.jifeline.OpenOBD.Protocol.Status\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x12_\n\rdeleteSession\x12%.com.jifeline.OpenOBD.Protocol.Status\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x12^\n\x0clistSessions\x12%.com.jifeline.OpenOBD.Protocol.Status\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x42\x02P\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n8openobd_protocol/SessionController/SessionServices.proto\x12/com.jifeline.OpenOBD.Protocol.SessionController\x1a\x1dopenobd_protocol/Status.proto\x1a\x30openobd_protocol/SessionController/Session.proto\x1a$openobd_protocol/BasicResponse.proto2\xb8\x05\n\x0fSessionServices\x12\x91\x01\n\x0fgetSessionToken\x12=.com.jifeline.OpenOBD.Protocol.SessionController.Authenticate\x1a=.com.jifeline.OpenOBD.Protocol.SessionController.SessionToken\"\x00\x12\x8e\x01\n\rcreateSession\x12=.com.jifeline.OpenOBD.Protocol.SessionController.StartSession\x1a<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x00\x12\x88\x01\n\ngetSession\x12:.com.jifeline.OpenOBD.Protocol.SessionController.SessionId\x1a<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x00\x12t\n\rdeleteSession\x12:.com.jifeline.OpenOBD.Protocol.SessionController.SessionId\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x12\x7f\n\x0clistSessions\x12+.com.jifeline.OpenOBD.Protocol.EmptyRequest\x1a@.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfoList\"\x00\x42\x02P\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'openobd_protocol.SessionController.SessionServices_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'P\001'
-  _globals['_SESSIONSERVICES']._serialized_start=191
-  _globals['_SESSIONSERVICES']._serialized_end=739
+  _globals['_SESSIONSERVICES']._serialized_start=229
+  _globals['_SESSIONSERVICES']._serialized_end=925
 # @@protoc_insertion_point(module_scope)
```

### Comparing `openobd_protocol-0.0.39/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py` & `openobd_protocol-0.0.40/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
+from openobd_protocol import BasicResponse_pb2 as openobd__protocol_dot_BasicResponse__pb2
 from openobd_protocol.SessionController import Session_pb2 as openobd__protocol_dot_SessionController_dot_Session__pb2
 from openobd_protocol import Status_pb2 as openobd__protocol_dot_Status__pb2
 
 
 class SessionServicesStub(object):
     """Missing associated documentation comment in .proto file."""
 
@@ -13,36 +14,36 @@
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.getSessionToken = channel.unary_unary(
                 '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/getSessionToken',
-                request_serializer=openobd__protocol_dot_Status__pb2.Status.SerializeToString,
-                response_deserializer=openobd__protocol_dot_Status__pb2.Status.FromString,
+                request_serializer=openobd__protocol_dot_SessionController_dot_Session__pb2.Authenticate.SerializeToString,
+                response_deserializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionToken.FromString,
                 )
         self.createSession = channel.unary_unary(
                 '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/createSession',
-                request_serializer=openobd__protocol_dot_SessionController_dot_Session__pb2.startSession.SerializeToString,
-                response_deserializer=openobd__protocol_dot_SessionController_dot_Session__pb2.sessionInfo.FromString,
+                request_serializer=openobd__protocol_dot_SessionController_dot_Session__pb2.StartSession.SerializeToString,
+                response_deserializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfo.FromString,
                 )
         self.getSession = channel.unary_unary(
                 '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/getSession',
-                request_serializer=openobd__protocol_dot_Status__pb2.Status.SerializeToString,
-                response_deserializer=openobd__protocol_dot_Status__pb2.Status.FromString,
+                request_serializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionId.SerializeToString,
+                response_deserializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfo.FromString,
                 )
         self.deleteSession = channel.unary_unary(
                 '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/deleteSession',
-                request_serializer=openobd__protocol_dot_Status__pb2.Status.SerializeToString,
+                request_serializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionId.SerializeToString,
                 response_deserializer=openobd__protocol_dot_Status__pb2.Status.FromString,
                 )
         self.listSessions = channel.unary_unary(
                 '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/listSessions',
-                request_serializer=openobd__protocol_dot_Status__pb2.Status.SerializeToString,
-                response_deserializer=openobd__protocol_dot_Status__pb2.Status.FromString,
+                request_serializer=openobd__protocol_dot_BasicResponse__pb2.EmptyRequest.SerializeToString,
+                response_deserializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfoList.FromString,
                 )
 
 
 class SessionServicesServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def getSessionToken(self, request, context):
@@ -76,36 +77,36 @@
         raise NotImplementedError('Method not implemented!')
 
 
 def add_SessionServicesServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'getSessionToken': grpc.unary_unary_rpc_method_handler(
                     servicer.getSessionToken,
-                    request_deserializer=openobd__protocol_dot_Status__pb2.Status.FromString,
-                    response_serializer=openobd__protocol_dot_Status__pb2.Status.SerializeToString,
+                    request_deserializer=openobd__protocol_dot_SessionController_dot_Session__pb2.Authenticate.FromString,
+                    response_serializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionToken.SerializeToString,
             ),
             'createSession': grpc.unary_unary_rpc_method_handler(
                     servicer.createSession,
-                    request_deserializer=openobd__protocol_dot_SessionController_dot_Session__pb2.startSession.FromString,
-                    response_serializer=openobd__protocol_dot_SessionController_dot_Session__pb2.sessionInfo.SerializeToString,
+                    request_deserializer=openobd__protocol_dot_SessionController_dot_Session__pb2.StartSession.FromString,
+                    response_serializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfo.SerializeToString,
             ),
             'getSession': grpc.unary_unary_rpc_method_handler(
                     servicer.getSession,
-                    request_deserializer=openobd__protocol_dot_Status__pb2.Status.FromString,
-                    response_serializer=openobd__protocol_dot_Status__pb2.Status.SerializeToString,
+                    request_deserializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionId.FromString,
+                    response_serializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfo.SerializeToString,
             ),
             'deleteSession': grpc.unary_unary_rpc_method_handler(
                     servicer.deleteSession,
-                    request_deserializer=openobd__protocol_dot_Status__pb2.Status.FromString,
+                    request_deserializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionId.FromString,
                     response_serializer=openobd__protocol_dot_Status__pb2.Status.SerializeToString,
             ),
             'listSessions': grpc.unary_unary_rpc_method_handler(
                     servicer.listSessions,
-                    request_deserializer=openobd__protocol_dot_Status__pb2.Status.FromString,
-                    response_serializer=openobd__protocol_dot_Status__pb2.Status.SerializeToString,
+                    request_deserializer=openobd__protocol_dot_BasicResponse__pb2.EmptyRequest.FromString,
+                    response_serializer=openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfoList.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'com.jifeline.OpenOBD.Protocol.SessionController.SessionServices', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
@@ -121,16 +122,16 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/getSessionToken',
-            openobd__protocol_dot_Status__pb2.Status.SerializeToString,
-            openobd__protocol_dot_Status__pb2.Status.FromString,
+            openobd__protocol_dot_SessionController_dot_Session__pb2.Authenticate.SerializeToString,
+            openobd__protocol_dot_SessionController_dot_Session__pb2.SessionToken.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def createSession(request,
             target,
             options=(),
@@ -138,16 +139,16 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/createSession',
-            openobd__protocol_dot_SessionController_dot_Session__pb2.startSession.SerializeToString,
-            openobd__protocol_dot_SessionController_dot_Session__pb2.sessionInfo.FromString,
+            openobd__protocol_dot_SessionController_dot_Session__pb2.StartSession.SerializeToString,
+            openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfo.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def getSession(request,
             target,
             options=(),
@@ -155,16 +156,16 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/getSession',
-            openobd__protocol_dot_Status__pb2.Status.SerializeToString,
-            openobd__protocol_dot_Status__pb2.Status.FromString,
+            openobd__protocol_dot_SessionController_dot_Session__pb2.SessionId.SerializeToString,
+            openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfo.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def deleteSession(request,
             target,
             options=(),
@@ -172,15 +173,15 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/deleteSession',
-            openobd__protocol_dot_Status__pb2.Status.SerializeToString,
+            openobd__protocol_dot_SessionController_dot_Session__pb2.SessionId.SerializeToString,
             openobd__protocol_dot_Status__pb2.Status.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def listSessions(request,
             target,
@@ -189,11 +190,11 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/listSessions',
-            openobd__protocol_dot_Status__pb2.Status.SerializeToString,
-            openobd__protocol_dot_Status__pb2.Status.FromString,
+            openobd__protocol_dot_BasicResponse__pb2.EmptyRequest.SerializeToString,
+            openobd__protocol_dot_SessionController_dot_Session__pb2.SessionInfoList.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `openobd_protocol-0.0.39/src/openobd_protocol/SessionController/Session_pb2.py` & `openobd_protocol-0.0.40/src/openobd_protocol/SessionController/Session_pb2.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,22 +8,31 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from openobd_protocol import Status_pb2 as openobd__protocol_dot_Status__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0openobd_protocol/SessionController/Session.proto\x12/com.jifeline.OpenOBD.Protocol.SessionController\"g\n\x0cstartSession\x12\x11\n\tclient_id\x18\x01 \x01(\t\x12\x1a\n\x12\x63lient_credentials\x18\x02 \x01(\t\x12\x0f\n\x07\x61pi_key\x18\x03 \x01(\t\x12\x17\n\x0f\x63onnection_uuid\x18\x04 \x01(\t\"u\n\x0bsessionInfo\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x12\n\ncreated_at\x18\x03 \x01(\t\x12\x18\n\x10session_endpoint\x18\x04 \x01(\t\x12\x1c\n\x14\x61uthentication_token\x18\x05 \x01(\tB\x02P\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0openobd_protocol/SessionController/Session.proto\x12/com.jifeline.OpenOBD.Protocol.SessionController\x1a\x1dopenobd_protocol/Status.proto\"\'\n\x0cStartSession\x12\x17\n\x0f\x63onnection_uuid\x18\x01 \x01(\t\"}\n\x0bSessionInfo\x12\n\n\x02id\x18\x01 \x01(\t\x12\x16\n\x0esession_status\x18\x02 \x01(\t\x12\x12\n\ncreated_at\x18\x03 \x01(\t\x12\x18\n\x10session_endpoint\x18\x04 \x01(\t\x12\x1c\n\x14\x61uthentication_token\x18\x05 \x01(\t\"N\n\x0c\x41uthenticate\x12\x11\n\tclient_id\x18\x01 \x01(\t\x12\x1a\n\x12\x63lient_credentials\x18\x02 \x01(\t\x12\x0f\n\x07\x61pi_key\x18\x03 \x01(\t\"\x1d\n\x0cSessionToken\x12\r\n\x05token\x18\x01 \x01(\t\"a\n\x0fSessionInfoList\x12N\n\x08sessions\x18\x01 \x03(\x0b\x32<.com.jifeline.OpenOBD.Protocol.SessionController.SessionInfo\"\x1f\n\tSessionId\x12\x12\n\nsession_id\x18\x01 \x01(\tB\x02P\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'openobd_protocol.SessionController.Session_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'P\001'
-  _globals['_STARTSESSION']._serialized_start=101
-  _globals['_STARTSESSION']._serialized_end=204
-  _globals['_SESSIONINFO']._serialized_start=206
-  _globals['_SESSIONINFO']._serialized_end=323
+  _globals['_STARTSESSION']._serialized_start=132
+  _globals['_STARTSESSION']._serialized_end=171
+  _globals['_SESSIONINFO']._serialized_start=173
+  _globals['_SESSIONINFO']._serialized_end=298
+  _globals['_AUTHENTICATE']._serialized_start=300
+  _globals['_AUTHENTICATE']._serialized_end=378
+  _globals['_SESSIONTOKEN']._serialized_start=380
+  _globals['_SESSIONTOKEN']._serialized_end=409
+  _globals['_SESSIONINFOLIST']._serialized_start=411
+  _globals['_SESSIONINFOLIST']._serialized_end=508
+  _globals['_SESSIONID']._serialized_start=510
+  _globals['_SESSIONID']._serialized_end=541
 # @@protoc_insertion_point(module_scope)
```

### Comparing `openobd_protocol-0.0.39/src/openobd_protocol/SessionController/Session_pb2.pyi` & `openobd_protocol-0.0.40/src/openobd_protocol/SessionController/Session_pb2.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,55 @@
+from openobd_protocol import Status_pb2 as _Status_pb2
+from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Optional as _Optional
+from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class startSession(_message.Message):
-    __slots__ = ("client_id", "client_credentials", "api_key", "connection_uuid")
-    CLIENT_ID_FIELD_NUMBER: _ClassVar[int]
-    CLIENT_CREDENTIALS_FIELD_NUMBER: _ClassVar[int]
-    API_KEY_FIELD_NUMBER: _ClassVar[int]
+class StartSession(_message.Message):
+    __slots__ = ("connection_uuid",)
     CONNECTION_UUID_FIELD_NUMBER: _ClassVar[int]
-    client_id: str
-    client_credentials: str
-    api_key: str
     connection_uuid: str
-    def __init__(self, client_id: _Optional[str] = ..., client_credentials: _Optional[str] = ..., api_key: _Optional[str] = ..., connection_uuid: _Optional[str] = ...) -> None: ...
+    def __init__(self, connection_uuid: _Optional[str] = ...) -> None: ...
 
-class sessionInfo(_message.Message):
-    __slots__ = ("id", "status", "created_at", "session_endpoint", "authentication_token")
+class SessionInfo(_message.Message):
+    __slots__ = ("id", "session_status", "created_at", "session_endpoint", "authentication_token")
     ID_FIELD_NUMBER: _ClassVar[int]
-    STATUS_FIELD_NUMBER: _ClassVar[int]
+    SESSION_STATUS_FIELD_NUMBER: _ClassVar[int]
     CREATED_AT_FIELD_NUMBER: _ClassVar[int]
     SESSION_ENDPOINT_FIELD_NUMBER: _ClassVar[int]
     AUTHENTICATION_TOKEN_FIELD_NUMBER: _ClassVar[int]
     id: str
-    status: str
+    session_status: str
     created_at: str
     session_endpoint: str
     authentication_token: str
-    def __init__(self, id: _Optional[str] = ..., status: _Optional[str] = ..., created_at: _Optional[str] = ..., session_endpoint: _Optional[str] = ..., authentication_token: _Optional[str] = ...) -> None: ...
+    def __init__(self, id: _Optional[str] = ..., session_status: _Optional[str] = ..., created_at: _Optional[str] = ..., session_endpoint: _Optional[str] = ..., authentication_token: _Optional[str] = ...) -> None: ...
+
+class Authenticate(_message.Message):
+    __slots__ = ("client_id", "client_credentials", "api_key")
+    CLIENT_ID_FIELD_NUMBER: _ClassVar[int]
+    CLIENT_CREDENTIALS_FIELD_NUMBER: _ClassVar[int]
+    API_KEY_FIELD_NUMBER: _ClassVar[int]
+    client_id: str
+    client_credentials: str
+    api_key: str
+    def __init__(self, client_id: _Optional[str] = ..., client_credentials: _Optional[str] = ..., api_key: _Optional[str] = ...) -> None: ...
+
+class SessionToken(_message.Message):
+    __slots__ = ("token",)
+    TOKEN_FIELD_NUMBER: _ClassVar[int]
+    token: str
+    def __init__(self, token: _Optional[str] = ...) -> None: ...
+
+class SessionInfoList(_message.Message):
+    __slots__ = ("sessions",)
+    SESSIONS_FIELD_NUMBER: _ClassVar[int]
+    sessions: _containers.RepeatedCompositeFieldContainer[SessionInfo]
+    def __init__(self, sessions: _Optional[_Iterable[_Union[SessionInfo, _Mapping]]] = ...) -> None: ...
+
+class SessionId(_message.Message):
+    __slots__ = ("session_id",)
+    SESSION_ID_FIELD_NUMBER: _ClassVar[int]
+    session_id: str
+    def __init__(self, session_id: _Optional[str] = ...) -> None: ...
```

### Comparing `openobd_protocol-0.0.39/src/openobd_protocol/Status_pb2.py` & `openobd_protocol-0.0.40/src/openobd_protocol/Status_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.39/src/openobd_protocol/Status_pb2.pyi` & `openobd_protocol-0.0.40/src/openobd_protocol/Status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.39/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py` & `openobd_protocol-0.0.40/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.39/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py` & `openobd_protocol-0.0.40/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.39/src/openobd_protocol/UserInterface/UserInterface_pb2.py` & `openobd_protocol-0.0.40/src/openobd_protocol/UserInterface/UserInterface_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.39/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi` & `openobd_protocol-0.0.40/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.39/src/openobd_protocol.egg-info/PKG-INFO` & `openobd_protocol-0.0.40/src/openobd_protocol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openobd-protocol
-Version: 0.0.39
+Version: 0.0.40
 Summary: Jifeline Networks OpenOBD Protocol Buffers gRPC
 Author-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 Maintainer-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 License: Copyright (c) 2024 Jifeline Networks B.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `openobd_protocol-0.0.39/src/openobd_protocol.egg-info/SOURCES.txt` & `openobd_protocol-0.0.40/src/openobd_protocol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

