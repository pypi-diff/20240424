# Comparing `tmp/npiai_proto-0.0.1.dev3.tar.gz` & `tmp/npiai_proto-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npiai_proto-0.0.1.dev3.tar", max compression
+gzip compressed data, was "npiai_proto-0.0.2.tar", max compression
```

## Comparing `npiai_proto-0.0.1.dev3.tar` & `npiai_proto-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       30 2024-04-19 21:33:34.559893 npiai_proto-0.0.1.dev3/README.md
--rw-r--r--   0        0        0     5859 2024-04-19 21:50:03.347460 npiai_proto-0.0.1.dev3/npiai_proto/api_pb2.py
--rw-r--r--   0        0        0     7203 2024-04-19 21:50:03.347674 npiai_proto-0.0.1.dev3/npiai_proto/api_pb2.pyi
--rw-r--r--   0        0        0     3829 2024-04-20 01:18:19.817912 npiai_proto-0.0.1.dev3/npiai_proto/api_pb2_grpc.py
--rw-r--r--   0        0        0      517 2024-04-20 01:18:26.420252 npiai_proto-0.0.1.dev3/pyproject.toml
--rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 npiai_proto-0.0.1.dev3/PKG-INFO
+-rw-r--r--   0        0        0       30 2024-04-19 21:33:34.559893 npiai_proto-0.0.2/README.md
+-rw-r--r--   0        0        0     5899 2024-04-24 21:41:11.918761 npiai_proto-0.0.2/npiai_proto/api_pb2.py
+-rw-r--r--   0        0        0     7260 2024-04-24 21:41:11.918929 npiai_proto-0.0.2/npiai_proto/api_pb2.pyi
+-rw-r--r--   0        0        0     3822 2024-04-24 21:41:11.919396 npiai_proto-0.0.2/npiai_proto/api_pb2_grpc.py
+-rw-r--r--   0        0        0      512 2024-04-24 21:54:54.015068 npiai_proto-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      712 1970-01-01 00:00:00.000000 npiai_proto-0.0.2/PKG-INFO
```

### Comparing `npiai_proto-0.0.1.dev3/npiai_proto/api_pb2.py` & `npiai_proto-0.0.2/npiai_proto/api_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,32 +11,32 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tapi.proto\x12\x0cnpi.core.api\x1a\x1bgoogle/protobuf/empty.proto\"\x84\x02\n\x07Request\x12\'\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x19.npi.core.api.RequestCode\x12\x12\n\nrequest_id\x18\x02 \x01(\t\x12\x11\n\tthread_id\x18\x03 \x01(\t\x12\x31\n\x0c\x63hat_request\x18\n \x01(\x0b\x32\x19.npi.core.api.ChatRequestH\x00\x12\x42\n\x15\x61\x63tion_result_request\x18\x0c \x01(\x0b\x32!.npi.core.api.ActionResultRequestH\x00\x12\'\n\x05\x65mpty\x18\x63 \x01(\x0b\x32\x16.google.protobuf.EmptyH\x00\x42\t\n\x07request\"7\n\x10\x41ppSchemaRequest\x12#\n\x04type\x18\x01 \x01(\x0e\x32\x15.npi.core.api.AppType\"8\n\x11\x41ppSchemaResponse\x12\x0e\n\x06schema\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\"G\n\x0b\x43hatRequest\x12#\n\x04type\x18\x01 \x01(\x0e\x32\x15.npi.core.api.AppType\x12\x13\n\x0binstruction\x18\x02 \x01(\t\"?\n\x13\x41\x63tionResultRequest\x12\x11\n\taction_id\x18\x01 \x01(\t\x12\x15\n\raction_result\x18\x02 \x01(\t\"\xfe\x01\n\x08Response\x12(\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x1a.npi.core.api.ResponseCode\x12\x12\n\nrequest_id\x18\x02 \x01(\t\x12\x11\n\tthread_id\x18\x03 \x01(\t\x12\x33\n\rchat_response\x18\n \x01(\x0b\x32\x1a.npi.core.api.ChatResponseH\x00\x12\x37\n\x0f\x61\x63tion_response\x18\x0b \x01(\x0b\x32\x1c.npi.core.api.ActionResponseH\x00\x12\'\n\x05\x65mpty\x18\x63 \x01(\x0b\x32\x16.google.protobuf.EmptyH\x00\x42\n\n\x08response\"\x1f\n\x0c\x43hatResponse\x12\x0f\n\x07message\x18\x01 \x01(\t\"\xc8\x01\n\x0e\x41\x63tionResponse\x12&\n\x04type\x18\x01 \x01(\x0e\x32\x18.npi.core.api.ActionType\x12\x11\n\taction_id\x18\x02 \x01(\t\x12;\n\x0ehuman_feedback\x18\n \x01(\x0b\x32!.npi.core.api.HumanFeedbackActionH\x00\x12\x32\n\tsafeguard\x18\x0b \x01(\x0b\x32\x1d.npi.core.api.SafeguardActionH\x00\x42\n\n\x08response\"k\n\x13HumanFeedbackAction\x12\x33\n\x04type\x18\x01 \x01(\x0e\x32%.npi.core.api.HumanFeedbackActionType\x12\x0e\n\x06notice\x18\x02 \x01(\t\x12\x0f\n\x07options\x18\x03 \x03(\t\"7\n\x0fSafeguardAction\x12\x11\n\taction_id\x18\x01 \x01(\t\x12\x11\n\tsafeguard\x18\x02 \x01(\t*J\n\x0bRequestCode\x12\x13\n\x0fREQUEST_UNKNOWN\x10\x00\x12\x08\n\x04\x43HAT\x10\x01\x12\t\n\x05\x46\x45TCH\x10\x02\x12\x11\n\rACTION_RESULT\x10\x03*r\n\x07\x41ppType\x12\x0f\n\x0b\x41PP_UNKNOWN\x10\x00\x12\x10\n\x0cGOOGLE_GMAIL\x10\x01\x12\x13\n\x0fGOOGLE_CALENDAR\x10\x02\x12\n\n\x06GITHUB\x10\x03\x12\t\n\x05SLACK\x10\x04\x12\x0b\n\x07\x44ISCORD\x10\x05\x12\x0b\n\x07TWITTER\x10\x06*m\n\x0cResponseCode\x12\x14\n\x10RESPONSE_UNKNOWN\x10\x00\x12\x0b\n\x07SUCCESS\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02\x12\x0b\n\x07MESSAGE\x10\x03\x12\x13\n\x0f\x41\x43TION_REQUIRED\x10\x04\x12\x0c\n\x08\x46INISHED\x10\x05*C\n\nActionType\x12\x12\n\x0eUNKNOWN_ACTION\x10\x00\x12\x12\n\x0eHUMAN_FEEDBACK\x10\x01\x12\r\n\tSAFEGUARD\x10\x02*z\n\x17HumanFeedbackActionType\x12\x14\n\x10UNKNOWN_FEEDBACK\x10\x00\x12\t\n\x05INPUT\x10\x01\x12\x14\n\x10SINGLE_SELECTION\x10\x02\x12\x16\n\x12MULTIPLE_SELECTION\x10\x03\x12\x10\n\x0c\x43ONFIRMATION\x10\x04\x32\x93\x01\n\tAppServer\x12\x35\n\x04\x43hat\x12\x15.npi.core.api.Request\x1a\x16.npi.core.api.Response\x12O\n\x0cGetAppSchema\x12\x1e.npi.core.api.AppSchemaRequest\x1a\x1f.npi.core.api.AppSchemaResponseB\x1eZ\x1cgithub.com/npi-ai/npi/serverb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tapi.proto\x12\x0cnpi.core.api\x1a\x1bgoogle/protobuf/empty.proto\"\x84\x02\n\x07Request\x12\'\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x19.npi.core.api.RequestCode\x12\x12\n\nrequest_id\x18\x02 \x01(\t\x12\x11\n\tthread_id\x18\x03 \x01(\t\x12\x31\n\x0c\x63hat_request\x18\n \x01(\x0b\x32\x19.npi.core.api.ChatRequestH\x00\x12\x42\n\x15\x61\x63tion_result_request\x18\x0c \x01(\x0b\x32!.npi.core.api.ActionResultRequestH\x00\x12\'\n\x05\x65mpty\x18\x63 \x01(\x0b\x32\x16.google.protobuf.EmptyH\x00\x42\t\n\x07request\"7\n\x10\x41ppSchemaRequest\x12#\n\x04type\x18\x01 \x01(\x0e\x32\x15.npi.core.api.AppType\"8\n\x11\x41ppSchemaResponse\x12\x0e\n\x06schema\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\"G\n\x0b\x43hatRequest\x12#\n\x04type\x18\x01 \x01(\x0e\x32\x15.npi.core.api.AppType\x12\x13\n\x0binstruction\x18\x02 \x01(\t\"?\n\x13\x41\x63tionResultRequest\x12\x11\n\taction_id\x18\x01 \x01(\t\x12\x15\n\raction_result\x18\x02 \x01(\t\"\xfe\x01\n\x08Response\x12(\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x1a.npi.core.api.ResponseCode\x12\x12\n\nrequest_id\x18\x02 \x01(\t\x12\x11\n\tthread_id\x18\x03 \x01(\t\x12\x33\n\rchat_response\x18\n \x01(\x0b\x32\x1a.npi.core.api.ChatResponseH\x00\x12\x37\n\x0f\x61\x63tion_response\x18\x0b \x01(\x0b\x32\x1c.npi.core.api.ActionResponseH\x00\x12\'\n\x05\x65mpty\x18\x63 \x01(\x0b\x32\x16.google.protobuf.EmptyH\x00\x42\n\n\x08response\"\x1f\n\x0c\x43hatResponse\x12\x0f\n\x07message\x18\x01 \x01(\t\"\xc8\x01\n\x0e\x41\x63tionResponse\x12&\n\x04type\x18\x01 \x01(\x0e\x32\x18.npi.core.api.ActionType\x12\x11\n\taction_id\x18\x02 \x01(\t\x12;\n\x0ehuman_feedback\x18\n \x01(\x0b\x32!.npi.core.api.HumanFeedbackActionH\x00\x12\x32\n\tsafeguard\x18\x0b \x01(\x0b\x32\x1d.npi.core.api.SafeguardActionH\x00\x42\n\n\x08response\"k\n\x13HumanFeedbackAction\x12\x33\n\x04type\x18\x01 \x01(\x0e\x32%.npi.core.api.HumanFeedbackActionType\x12\x0e\n\x06notice\x18\x02 \x01(\t\x12\x0f\n\x07options\x18\x03 \x03(\t\"7\n\x0fSafeguardAction\x12\x11\n\taction_id\x18\x01 \x01(\t\x12\x11\n\tsafeguard\x18\x02 \x01(\t*J\n\x0bRequestCode\x12\x13\n\x0fREQUEST_UNKNOWN\x10\x00\x12\x08\n\x04\x43HAT\x10\x01\x12\t\n\x05\x46\x45TCH\x10\x02\x12\x11\n\rACTION_RESULT\x10\x03*\x83\x01\n\x07\x41ppType\x12\x0f\n\x0b\x41PP_UNKNOWN\x10\x00\x12\x10\n\x0cGOOGLE_GMAIL\x10\x01\x12\x13\n\x0fGOOGLE_CALENDAR\x10\x02\x12\n\n\x06GITHUB\x10\x03\x12\t\n\x05SLACK\x10\x04\x12\x0b\n\x07\x44ISCORD\x10\x05\x12\x0b\n\x07TWITTER\x10\x06\x12\x0f\n\x0bWEB_BROWSER\x10\x07*m\n\x0cResponseCode\x12\x14\n\x10RESPONSE_UNKNOWN\x10\x00\x12\x0b\n\x07SUCCESS\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02\x12\x0b\n\x07MESSAGE\x10\x03\x12\x13\n\x0f\x41\x43TION_REQUIRED\x10\x04\x12\x0c\n\x08\x46INISHED\x10\x05*C\n\nActionType\x12\x12\n\x0eUNKNOWN_ACTION\x10\x00\x12\x12\n\x0eHUMAN_FEEDBACK\x10\x01\x12\r\n\tSAFEGUARD\x10\x02*z\n\x17HumanFeedbackActionType\x12\x14\n\x10UNKNOWN_FEEDBACK\x10\x00\x12\t\n\x05INPUT\x10\x01\x12\x14\n\x10SINGLE_SELECTION\x10\x02\x12\x16\n\x12MULTIPLE_SELECTION\x10\x03\x12\x10\n\x0c\x43ONFIRMATION\x10\x04\x32\x93\x01\n\tAppServer\x12\x35\n\x04\x43hat\x12\x15.npi.core.api.Request\x1a\x16.npi.core.api.Response\x12O\n\x0cGetAppSchema\x12\x1e.npi.core.api.AppSchemaRequest\x1a\x1f.npi.core.api.AppSchemaResponseB\x1eZ\x1cgithub.com/npi-ai/npi/serverb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'api_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'Z\034github.com/npi-ai/npi/server'
   _globals['_REQUESTCODE']._serialized_start=1231
   _globals['_REQUESTCODE']._serialized_end=1305
-  _globals['_APPTYPE']._serialized_start=1307
-  _globals['_APPTYPE']._serialized_end=1421
-  _globals['_RESPONSECODE']._serialized_start=1423
-  _globals['_RESPONSECODE']._serialized_end=1532
-  _globals['_ACTIONTYPE']._serialized_start=1534
-  _globals['_ACTIONTYPE']._serialized_end=1601
-  _globals['_HUMANFEEDBACKACTIONTYPE']._serialized_start=1603
-  _globals['_HUMANFEEDBACKACTIONTYPE']._serialized_end=1725
+  _globals['_APPTYPE']._serialized_start=1308
+  _globals['_APPTYPE']._serialized_end=1439
+  _globals['_RESPONSECODE']._serialized_start=1441
+  _globals['_RESPONSECODE']._serialized_end=1550
+  _globals['_ACTIONTYPE']._serialized_start=1552
+  _globals['_ACTIONTYPE']._serialized_end=1619
+  _globals['_HUMANFEEDBACKACTIONTYPE']._serialized_start=1621
+  _globals['_HUMANFEEDBACKACTIONTYPE']._serialized_end=1743
   _globals['_REQUEST']._serialized_start=57
   _globals['_REQUEST']._serialized_end=317
   _globals['_APPSCHEMAREQUEST']._serialized_start=319
   _globals['_APPSCHEMAREQUEST']._serialized_end=374
   _globals['_APPSCHEMARESPONSE']._serialized_start=376
   _globals['_APPSCHEMARESPONSE']._serialized_end=432
   _globals['_CHATREQUEST']._serialized_start=434
@@ -49,10 +49,10 @@
   _globals['_CHATRESPONSE']._serialized_end=860
   _globals['_ACTIONRESPONSE']._serialized_start=863
   _globals['_ACTIONRESPONSE']._serialized_end=1063
   _globals['_HUMANFEEDBACKACTION']._serialized_start=1065
   _globals['_HUMANFEEDBACKACTION']._serialized_end=1172
   _globals['_SAFEGUARDACTION']._serialized_start=1174
   _globals['_SAFEGUARDACTION']._serialized_end=1229
-  _globals['_APPSERVER']._serialized_start=1728
-  _globals['_APPSERVER']._serialized_end=1875
+  _globals['_APPSERVER']._serialized_start=1746
+  _globals['_APPSERVER']._serialized_end=1893
 # @@protoc_insertion_point(module_scope)
```

### Comparing `npiai_proto-0.0.1.dev3/npiai_proto/api_pb2.pyi` & `npiai_proto-0.0.2/npiai_proto/api_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     APP_UNKNOWN: _ClassVar[AppType]
     GOOGLE_GMAIL: _ClassVar[AppType]
     GOOGLE_CALENDAR: _ClassVar[AppType]
     GITHUB: _ClassVar[AppType]
     SLACK: _ClassVar[AppType]
     DISCORD: _ClassVar[AppType]
     TWITTER: _ClassVar[AppType]
+    WEB_BROWSER: _ClassVar[AppType]
 
 class ResponseCode(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = ()
     RESPONSE_UNKNOWN: _ClassVar[ResponseCode]
     SUCCESS: _ClassVar[ResponseCode]
     FAILED: _ClassVar[ResponseCode]
     MESSAGE: _ClassVar[ResponseCode]
@@ -53,14 +54,15 @@
 APP_UNKNOWN: AppType
 GOOGLE_GMAIL: AppType
 GOOGLE_CALENDAR: AppType
 GITHUB: AppType
 SLACK: AppType
 DISCORD: AppType
 TWITTER: AppType
+WEB_BROWSER: AppType
 RESPONSE_UNKNOWN: ResponseCode
 SUCCESS: ResponseCode
 FAILED: ResponseCode
 MESSAGE: ResponseCode
 ACTION_REQUIRED: ResponseCode
 FINISHED: ResponseCode
 UNKNOWN_ACTION: ActionType
```

### Comparing `npiai_proto-0.0.1.dev3/npiai_proto/api_pb2_grpc.py` & `npiai_proto-0.0.2/npiai_proto/api_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from . import api_pb2 as api__pb2
+import api_pb2 as api__pb2
 
 
 class AppServerStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
```

### Comparing `npiai_proto-0.0.1.dev3/pyproject.toml` & `npiai_proto-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "npiai-proto"
-version = "v0.0.1.dev3"
+version = "v0.0.2"
 description = "The NPI.AI Proto"
 license = "Apache-2.0"
 authors = ["Wells Wang <wells@npi.ai>"]
 readme = "README.md"
 homepage = "https://github.com/npi-ai/proto/python"
 repository = "https://github.com/npi-ai/proto/python"
```

### Comparing `npiai_proto-0.0.1.dev3/PKG-INFO` & `npiai_proto-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npiai-proto
-Version: 0.0.1.dev3
+Version: 0.0.2
 Summary: The NPI.AI Proto
 Home-page: https://github.com/npi-ai/proto/python
 License: Apache-2.0
 Author: Wells Wang
 Author-email: wells@npi.ai
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

