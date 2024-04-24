# Comparing `tmp/retell_sdk-3.8.0.tar.gz` & `tmp/retell_sdk-3.9.0.tar.gz`

## Comparing `retell_sdk-3.8.0.tar` & `retell_sdk-3.9.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/__init__.py
--rw-r--r--   0        0        0    64254 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_base_client.py
--rw-r--r--   0        0        0    15337 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_constants.py
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_files.py
--rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_qs.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_resource.py
--rw-r--r--   0        0        0    28375 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_response.py
--rw-r--r--   0        0        0    10100 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_streaming.py
--rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_types.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_utils/__init__.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/lib/.keep
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/resources/__init__.py
--rw-r--r--   0        0        0    43021 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/resources/agent.py
--rw-r--r--   0        0        0    25014 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/resources/call.py
--rw-r--r--   0        0        0    26571 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/resources/llm.py
--rw-r--r--   0        0        0    17883 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/resources/phone_number.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/__init__.py
--rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/agent_create_params.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/agent_list_response.py
--rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/agent_response.py
--rw-r--r--   0        0        0     5329 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/agent_update_params.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/call_create_params.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/call_list_params.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/call_list_response.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/call_register_params.py
--rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/call_response.py
--rw-r--r--   0        0        0    17703 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/llm_create_params.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/llm_list_response.py
--rw-r--r--   0        0        0    17807 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/llm_response.py
--rw-r--r--   0        0        0    17703 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/llm_update_params.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/phone_number_create_params.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/phone_number_list_response.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/phone_number_response.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/phone_number_update_params.py
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell/types/register_call_response.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell_ai/lib/.keep
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/retell_sdk/lib/.keep
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/src/toddlzt/lib/.keep
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/.gitignore
--rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/LICENSE
--rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/pyproject.toml
--rw-r--r--   0        0        0    11945 2020-02-02 00:00:00.000000 retell_sdk-3.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/__init__.py
+-rw-r--r--   0        0        0    64254 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/_base_client.py
+-rw-r--r--   0        0        0    15593 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/_constants.py
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/_files.py
+-rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/_qs.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/_resource.py
+-rw-r--r--   0        0        0    28375 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/_response.py
+-rw-r--r--   0        0        0    10100 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/_streaming.py
+-rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/_types.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/_utils/__init__.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/lib/.keep
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/resources/__init__.py
+-rw-r--r--   0        0        0    43254 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/resources/agent.py
+-rw-r--r--   0        0        0    26428 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/resources/call.py
+-rw-r--r--   0        0        0    26800 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/resources/llm.py
+-rw-r--r--   0        0        0    18109 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/resources/phone_number.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/types/__init__.py
+-rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/types/agent_create_params.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/types/agent_list_response.py
+-rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/types/agent_response.py
+-rw-r--r--   0        0        0     5329 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/types/agent_update_params.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/types/call_create_params.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/types/call_list_params.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/types/call_list_response.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/types/call_register_params.py
+-rw-r--r--   0        0        0    10305 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/types/call_response.py
+-rw-r--r--   0        0        0    17703 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/types/llm_create_params.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/types/llm_list_response.py
+-rw-r--r--   0        0        0    17807 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/types/llm_response.py
+-rw-r--r--   0        0        0    17703 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/types/llm_update_params.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/types/phone_number_create_params.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/types/phone_number_list_response.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/types/phone_number_response.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/types/phone_number_update_params.py
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell/types/register_call_response.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell_ai/lib/.keep
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/retell_sdk/lib/.keep
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/src/toddlzt/lib/.keep
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/.gitignore
+-rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/LICENSE
+-rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/pyproject.toml
+-rw-r--r--   0        0        0    11948 2020-02-02 00:00:00.000000 retell_sdk-3.9.0/PKG-INFO
```

### Comparing `retell_sdk-3.8.0/src/retell/__init__.py` & `retell_sdk-3.9.0/src/retell/__init__.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.8.0/src/retell/_base_client.py` & `retell_sdk-3.9.0/src/retell/_base_client.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.8.0/src/retell/_client.py` & `retell_sdk-3.9.0/src/retell/_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,18 +42,18 @@
     "AsyncRetell",
     "Client",
     "AsyncClient",
 ]
 
 
 class Retell(SyncAPIClient):
-    call: resources.Call
-    phone_number: resources.PhoneNumber
-    agent: resources.Agent
-    llm: resources.Llm
+    call: resources.CallResource
+    phone_number: resources.PhoneNumberResource
+    agent: resources.AgentResource
+    llm: resources.LlmResource
     with_raw_response: RetellWithRawResponse
     with_streaming_response: RetellWithStreamedResponse
 
     # client options
     api_key: str
 
     def __init__(
@@ -94,18 +94,18 @@
             timeout=timeout,
             http_client=http_client,
             custom_headers=default_headers,
             custom_query=default_query,
             _strict_response_validation=_strict_response_validation,
         )
 
-        self.call = resources.Call(self)
-        self.phone_number = resources.PhoneNumber(self)
-        self.agent = resources.Agent(self)
-        self.llm = resources.Llm(self)
+        self.call = resources.CallResource(self)
+        self.phone_number = resources.PhoneNumberResource(self)
+        self.agent = resources.AgentResource(self)
+        self.llm = resources.LlmResource(self)
         self.with_raw_response = RetellWithRawResponse(self)
         self.with_streaming_response = RetellWithStreamedResponse(self)
 
     @property
     @override
     def qs(self) -> Querystring:
         return Querystring(array_format="comma")
@@ -207,18 +207,18 @@
 
         if response.status_code >= 500:
             return _exceptions.InternalServerError(err_msg, response=response, body=body)
         return APIStatusError(err_msg, response=response, body=body)
 
 
 class AsyncRetell(AsyncAPIClient):
-    call: resources.AsyncCall
-    phone_number: resources.AsyncPhoneNumber
-    agent: resources.AsyncAgent
-    llm: resources.AsyncLlm
+    call: resources.AsyncCallResource
+    phone_number: resources.AsyncPhoneNumberResource
+    agent: resources.AsyncAgentResource
+    llm: resources.AsyncLlmResource
     with_raw_response: AsyncRetellWithRawResponse
     with_streaming_response: AsyncRetellWithStreamedResponse
 
     # client options
     api_key: str
 
     def __init__(
@@ -259,18 +259,18 @@
             timeout=timeout,
             http_client=http_client,
             custom_headers=default_headers,
             custom_query=default_query,
             _strict_response_validation=_strict_response_validation,
         )
 
-        self.call = resources.AsyncCall(self)
-        self.phone_number = resources.AsyncPhoneNumber(self)
-        self.agent = resources.AsyncAgent(self)
-        self.llm = resources.AsyncLlm(self)
+        self.call = resources.AsyncCallResource(self)
+        self.phone_number = resources.AsyncPhoneNumberResource(self)
+        self.agent = resources.AsyncAgentResource(self)
+        self.llm = resources.AsyncLlmResource(self)
         self.with_raw_response = AsyncRetellWithRawResponse(self)
         self.with_streaming_response = AsyncRetellWithStreamedResponse(self)
 
     @property
     @override
     def qs(self) -> Querystring:
         return Querystring(array_format="comma")
@@ -373,40 +373,40 @@
         if response.status_code >= 500:
             return _exceptions.InternalServerError(err_msg, response=response, body=body)
         return APIStatusError(err_msg, response=response, body=body)
 
 
 class RetellWithRawResponse:
     def __init__(self, client: Retell) -> None:
-        self.call = resources.CallWithRawResponse(client.call)
-        self.phone_number = resources.PhoneNumberWithRawResponse(client.phone_number)
-        self.agent = resources.AgentWithRawResponse(client.agent)
-        self.llm = resources.LlmWithRawResponse(client.llm)
+        self.call = resources.CallResourceWithRawResponse(client.call)
+        self.phone_number = resources.PhoneNumberResourceWithRawResponse(client.phone_number)
+        self.agent = resources.AgentResourceWithRawResponse(client.agent)
+        self.llm = resources.LlmResourceWithRawResponse(client.llm)
 
 
 class AsyncRetellWithRawResponse:
     def __init__(self, client: AsyncRetell) -> None:
-        self.call = resources.AsyncCallWithRawResponse(client.call)
-        self.phone_number = resources.AsyncPhoneNumberWithRawResponse(client.phone_number)
-        self.agent = resources.AsyncAgentWithRawResponse(client.agent)
-        self.llm = resources.AsyncLlmWithRawResponse(client.llm)
+        self.call = resources.AsyncCallResourceWithRawResponse(client.call)
+        self.phone_number = resources.AsyncPhoneNumberResourceWithRawResponse(client.phone_number)
+        self.agent = resources.AsyncAgentResourceWithRawResponse(client.agent)
+        self.llm = resources.AsyncLlmResourceWithRawResponse(client.llm)
 
 
 class RetellWithStreamedResponse:
     def __init__(self, client: Retell) -> None:
-        self.call = resources.CallWithStreamingResponse(client.call)
-        self.phone_number = resources.PhoneNumberWithStreamingResponse(client.phone_number)
-        self.agent = resources.AgentWithStreamingResponse(client.agent)
-        self.llm = resources.LlmWithStreamingResponse(client.llm)
+        self.call = resources.CallResourceWithStreamingResponse(client.call)
+        self.phone_number = resources.PhoneNumberResourceWithStreamingResponse(client.phone_number)
+        self.agent = resources.AgentResourceWithStreamingResponse(client.agent)
+        self.llm = resources.LlmResourceWithStreamingResponse(client.llm)
 
 
 class AsyncRetellWithStreamedResponse:
     def __init__(self, client: AsyncRetell) -> None:
-        self.call = resources.AsyncCallWithStreamingResponse(client.call)
-        self.phone_number = resources.AsyncPhoneNumberWithStreamingResponse(client.phone_number)
-        self.agent = resources.AsyncAgentWithStreamingResponse(client.agent)
-        self.llm = resources.AsyncLlmWithStreamingResponse(client.llm)
+        self.call = resources.AsyncCallResourceWithStreamingResponse(client.call)
+        self.phone_number = resources.AsyncPhoneNumberResourceWithStreamingResponse(client.phone_number)
+        self.agent = resources.AsyncAgentResourceWithStreamingResponse(client.agent)
+        self.llm = resources.AsyncLlmResourceWithStreamingResponse(client.llm)
 
 
 Client = Retell
 
 AsyncClient = AsyncRetell
```

### Comparing `retell_sdk-3.8.0/src/retell/_compat.py` & `retell_sdk-3.9.0/src/retell/_compat.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.8.0/src/retell/_exceptions.py` & `retell_sdk-3.9.0/src/retell/_exceptions.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.8.0/src/retell/_files.py` & `retell_sdk-3.9.0/src/retell/_files.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.8.0/src/retell/_models.py` & `retell_sdk-3.9.0/src/retell/_models.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.8.0/src/retell/_qs.py` & `retell_sdk-3.9.0/src/retell/_qs.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.8.0/src/retell/_resource.py` & `retell_sdk-3.9.0/src/retell/_resource.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.8.0/src/retell/_response.py` & `retell_sdk-3.9.0/src/retell/_response.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.8.0/src/retell/_streaming.py` & `retell_sdk-3.9.0/src/retell/_streaming.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.8.0/src/retell/_types.py` & `retell_sdk-3.9.0/src/retell/_types.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.8.0/src/retell/_utils/__init__.py` & `retell_sdk-3.9.0/src/retell/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.8.0/src/retell/_utils/_logs.py` & `retell_sdk-3.9.0/src/retell/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.8.0/src/retell/_utils/_proxy.py` & `retell_sdk-3.9.0/src/retell/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.8.0/src/retell/_utils/_sync.py` & `retell_sdk-3.9.0/src/retell/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.8.0/src/retell/_utils/_transform.py` & `retell_sdk-3.9.0/src/retell/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.8.0/src/retell/_utils/_typing.py` & `retell_sdk-3.9.0/src/retell/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.8.0/src/retell/_utils/_utils.py` & `retell_sdk-3.9.0/src/retell/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.8.0/src/retell/resources/agent.py` & `retell_sdk-3.9.0/src/retell/resources/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 from typing import List, Optional
 from typing_extensions import Literal
 
 import httpx
 
-from ..types import AgentResponse, AgentListResponse, agent_create_params, agent_update_params
+from ..types import agent_create_params, agent_update_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NoneType, NotGiven
 from .._utils import (
     maybe_transform,
     async_maybe_transform,
 )
 from .._compat import cached_property
 from .._resource import SyncAPIResource, AsyncAPIResource
@@ -20,26 +20,28 @@
     to_streamed_response_wrapper,
     async_to_raw_response_wrapper,
     async_to_streamed_response_wrapper,
 )
 from .._base_client import (
     make_request_options,
 )
+from ..types.agent_response import AgentResponse
+from ..types.agent_list_response import AgentListResponse
 
-__all__ = ["Agent", "AsyncAgent"]
+__all__ = ["AgentResource", "AsyncAgentResource"]
 
 
-class Agent(SyncAPIResource):
+class AgentResource(SyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> AgentWithRawResponse:
-        return AgentWithRawResponse(self)
+    def with_raw_response(self) -> AgentResourceWithRawResponse:
+        return AgentResourceWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> AgentWithStreamingResponse:
-        return AgentWithStreamingResponse(self)
+    def with_streaming_response(self) -> AgentResourceWithStreamingResponse:
+        return AgentResourceWithStreamingResponse(self)
 
     def create(
         self,
         *,
         llm_websocket_url: str,
         voice_id: str,
         agent_name: Optional[str] | NotGiven = NOT_GIVEN,
@@ -434,22 +436,22 @@
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=NoneType,
         )
 
 
-class AsyncAgent(AsyncAPIResource):
+class AsyncAgentResource(AsyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> AsyncAgentWithRawResponse:
-        return AsyncAgentWithRawResponse(self)
+    def with_raw_response(self) -> AsyncAgentResourceWithRawResponse:
+        return AsyncAgentResourceWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> AsyncAgentWithStreamingResponse:
-        return AsyncAgentWithStreamingResponse(self)
+    def with_streaming_response(self) -> AsyncAgentResourceWithStreamingResponse:
+        return AsyncAgentResourceWithStreamingResponse(self)
 
     async def create(
         self,
         *,
         llm_websocket_url: str,
         voice_id: str,
         agent_name: Optional[str] | NotGiven = NOT_GIVEN,
@@ -844,16 +846,16 @@
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=NoneType,
         )
 
 
-class AgentWithRawResponse:
-    def __init__(self, agent: Agent) -> None:
+class AgentResourceWithRawResponse:
+    def __init__(self, agent: AgentResource) -> None:
         self._agent = agent
 
         self.create = to_raw_response_wrapper(
             agent.create,
         )
         self.retrieve = to_raw_response_wrapper(
             agent.retrieve,
@@ -865,16 +867,16 @@
             agent.list,
         )
         self.delete = to_raw_response_wrapper(
             agent.delete,
         )
 
 
-class AsyncAgentWithRawResponse:
-    def __init__(self, agent: AsyncAgent) -> None:
+class AsyncAgentResourceWithRawResponse:
+    def __init__(self, agent: AsyncAgentResource) -> None:
         self._agent = agent
 
         self.create = async_to_raw_response_wrapper(
             agent.create,
         )
         self.retrieve = async_to_raw_response_wrapper(
             agent.retrieve,
@@ -886,16 +888,16 @@
             agent.list,
         )
         self.delete = async_to_raw_response_wrapper(
             agent.delete,
         )
 
 
-class AgentWithStreamingResponse:
-    def __init__(self, agent: Agent) -> None:
+class AgentResourceWithStreamingResponse:
+    def __init__(self, agent: AgentResource) -> None:
         self._agent = agent
 
         self.create = to_streamed_response_wrapper(
             agent.create,
         )
         self.retrieve = to_streamed_response_wrapper(
             agent.retrieve,
@@ -907,16 +909,16 @@
             agent.list,
         )
         self.delete = to_streamed_response_wrapper(
             agent.delete,
         )
 
 
-class AsyncAgentWithStreamingResponse:
-    def __init__(self, agent: AsyncAgent) -> None:
+class AsyncAgentResourceWithStreamingResponse:
+    def __init__(self, agent: AsyncAgentResource) -> None:
         self._agent = agent
 
         self.create = async_to_streamed_response_wrapper(
             agent.create,
         )
         self.retrieve = async_to_streamed_response_wrapper(
             agent.retrieve,
```

### Comparing `retell_sdk-3.8.0/src/retell/resources/call.py` & `retell_sdk-3.9.0/src/retell/resources/call.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,15 @@
 from __future__ import annotations
 
 from typing import Dict
 from typing_extensions import Literal
 
 import httpx
 
-from ..types import (
-    CallResponse,
-    CallListResponse,
-    RegisterCallResponse,
-    call_list_params,
-    call_create_params,
-    call_register_params,
-)
+from ..types import call_list_params, call_create_params, call_register_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import (
     maybe_transform,
     async_maybe_transform,
 )
 from .._compat import cached_property
 from .._resource import SyncAPIResource, AsyncAPIResource
@@ -27,32 +20,36 @@
     to_streamed_response_wrapper,
     async_to_raw_response_wrapper,
     async_to_streamed_response_wrapper,
 )
 from .._base_client import (
     make_request_options,
 )
+from ..types.call_response import CallResponse
+from ..types.call_list_response import CallListResponse
+from ..types.register_call_response import RegisterCallResponse
 
-__all__ = ["Call", "AsyncCall"]
+__all__ = ["CallResource", "AsyncCallResource"]
 
 
-class Call(SyncAPIResource):
+class CallResource(SyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> CallWithRawResponse:
-        return CallWithRawResponse(self)
+    def with_raw_response(self) -> CallResourceWithRawResponse:
+        return CallResourceWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> CallWithStreamingResponse:
-        return CallWithStreamingResponse(self)
+    def with_streaming_response(self) -> CallResourceWithStreamingResponse:
+        return CallResourceWithStreamingResponse(self)
 
     def create(
         self,
         *,
         from_number: str,
         to_number: str,
+        drop_call_if_machine_detected: bool | NotGiven = NOT_GIVEN,
         override_agent_id: str | NotGiven = NOT_GIVEN,
         retell_llm_dynamic_variables: Dict[str, object] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
@@ -62,14 +59,17 @@
         Create a new phone call
 
         Args:
           from_number: The number you own in BCP 47 format.
 
           to_number: The number you want to call, in BCP 47 format.
 
+          drop_call_if_machine_detected: If set, will drop the call if machine (voicemail, IVR) is detected. If not set,
+              default value of false will apply.
+
           override_agent_id: For this particular call, override the agent used with this agent id. This does
               not bind the agent to this number, this is for one time override.
 
           retell_llm_dynamic_variables: Add optional dynamic variables in key value pairs of string that injects into
               your Retell LLM prompt and tool description. Only applicable for Retell LLM.
 
           extra_headers: Send extra headers
@@ -82,14 +82,15 @@
         """
         return self._post(
             "/create-phone-call",
             body=maybe_transform(
                 {
                     "from_number": from_number,
                     "to_number": to_number,
+                    "drop_call_if_machine_detected": drop_call_if_machine_detected,
                     "override_agent_id": override_agent_id,
                     "retell_llm_dynamic_variables": retell_llm_dynamic_variables,
                 },
                 call_create_params.CallCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
@@ -131,28 +132,32 @@
         )
 
     def list(
         self,
         *,
         filter_criteria: call_list_params.FilterCriteria | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
+        pagination_key: str | NotGiven = NOT_GIVEN,
         sort_order: Literal["ascending", "descending"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> CallListResponse:
         """
         Retrieve call details
 
         Args:
           limit: Limit the number of calls returned.
 
+          pagination_key: The pagination call id to continue fetching the next page of calls. If not set,
+              will start from the beginning.
+
           sort_order: The calls will be sorted by `start_timestamp`, whether to return the calls in
               ascending or descending order.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
@@ -167,14 +172,15 @@
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
                         "filter_criteria": filter_criteria,
                         "limit": limit,
+                        "pagination_key": pagination_key,
                         "sort_order": sort_order,
                     },
                     call_list_params.CallListParams,
                 ),
             ),
             cast_to=CallListResponse,
         )
@@ -286,28 +292,29 @@
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=RegisterCallResponse,
         )
 
 
-class AsyncCall(AsyncAPIResource):
+class AsyncCallResource(AsyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> AsyncCallWithRawResponse:
-        return AsyncCallWithRawResponse(self)
+    def with_raw_response(self) -> AsyncCallResourceWithRawResponse:
+        return AsyncCallResourceWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> AsyncCallWithStreamingResponse:
-        return AsyncCallWithStreamingResponse(self)
+    def with_streaming_response(self) -> AsyncCallResourceWithStreamingResponse:
+        return AsyncCallResourceWithStreamingResponse(self)
 
     async def create(
         self,
         *,
         from_number: str,
         to_number: str,
+        drop_call_if_machine_detected: bool | NotGiven = NOT_GIVEN,
         override_agent_id: str | NotGiven = NOT_GIVEN,
         retell_llm_dynamic_variables: Dict[str, object] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
@@ -317,14 +324,17 @@
         Create a new phone call
 
         Args:
           from_number: The number you own in BCP 47 format.
 
           to_number: The number you want to call, in BCP 47 format.
 
+          drop_call_if_machine_detected: If set, will drop the call if machine (voicemail, IVR) is detected. If not set,
+              default value of false will apply.
+
           override_agent_id: For this particular call, override the agent used with this agent id. This does
               not bind the agent to this number, this is for one time override.
 
           retell_llm_dynamic_variables: Add optional dynamic variables in key value pairs of string that injects into
               your Retell LLM prompt and tool description. Only applicable for Retell LLM.
 
           extra_headers: Send extra headers
@@ -337,14 +347,15 @@
         """
         return await self._post(
             "/create-phone-call",
             body=await async_maybe_transform(
                 {
                     "from_number": from_number,
                     "to_number": to_number,
+                    "drop_call_if_machine_detected": drop_call_if_machine_detected,
                     "override_agent_id": override_agent_id,
                     "retell_llm_dynamic_variables": retell_llm_dynamic_variables,
                 },
                 call_create_params.CallCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
@@ -386,28 +397,32 @@
         )
 
     async def list(
         self,
         *,
         filter_criteria: call_list_params.FilterCriteria | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
+        pagination_key: str | NotGiven = NOT_GIVEN,
         sort_order: Literal["ascending", "descending"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> CallListResponse:
         """
         Retrieve call details
 
         Args:
           limit: Limit the number of calls returned.
 
+          pagination_key: The pagination call id to continue fetching the next page of calls. If not set,
+              will start from the beginning.
+
           sort_order: The calls will be sorted by `start_timestamp`, whether to return the calls in
               ascending or descending order.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
@@ -422,14 +437,15 @@
                 extra_query=extra_query,
                 extra_body=extra_body,
                 timeout=timeout,
                 query=await async_maybe_transform(
                     {
                         "filter_criteria": filter_criteria,
                         "limit": limit,
+                        "pagination_key": pagination_key,
                         "sort_order": sort_order,
                     },
                     call_list_params.CallListParams,
                 ),
             ),
             cast_to=CallListResponse,
         )
@@ -541,16 +557,16 @@
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=RegisterCallResponse,
         )
 
 
-class CallWithRawResponse:
-    def __init__(self, call: Call) -> None:
+class CallResourceWithRawResponse:
+    def __init__(self, call: CallResource) -> None:
         self._call = call
 
         self.create = to_raw_response_wrapper(
             call.create,
         )
         self.retrieve = to_raw_response_wrapper(
             call.retrieve,
@@ -559,16 +575,16 @@
             call.list,
         )
         self.register = to_raw_response_wrapper(
             call.register,
         )
 
 
-class AsyncCallWithRawResponse:
-    def __init__(self, call: AsyncCall) -> None:
+class AsyncCallResourceWithRawResponse:
+    def __init__(self, call: AsyncCallResource) -> None:
         self._call = call
 
         self.create = async_to_raw_response_wrapper(
             call.create,
         )
         self.retrieve = async_to_raw_response_wrapper(
             call.retrieve,
@@ -577,16 +593,16 @@
             call.list,
         )
         self.register = async_to_raw_response_wrapper(
             call.register,
         )
 
 
-class CallWithStreamingResponse:
-    def __init__(self, call: Call) -> None:
+class CallResourceWithStreamingResponse:
+    def __init__(self, call: CallResource) -> None:
         self._call = call
 
         self.create = to_streamed_response_wrapper(
             call.create,
         )
         self.retrieve = to_streamed_response_wrapper(
             call.retrieve,
@@ -595,16 +611,16 @@
             call.list,
         )
         self.register = to_streamed_response_wrapper(
             call.register,
         )
 
 
-class AsyncCallWithStreamingResponse:
-    def __init__(self, call: AsyncCall) -> None:
+class AsyncCallResourceWithStreamingResponse:
+    def __init__(self, call: AsyncCallResource) -> None:
         self._call = call
 
         self.create = async_to_streamed_response_wrapper(
             call.create,
         )
         self.retrieve = async_to_streamed_response_wrapper(
             call.retrieve,
```

### Comparing `retell_sdk-3.8.0/src/retell/resources/llm.py` & `retell_sdk-3.9.0/src/retell/resources/llm.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 from typing import Iterable, Optional
 from typing_extensions import Literal
 
 import httpx
 
-from ..types import LlmResponse, LlmListResponse, llm_create_params, llm_update_params
+from ..types import llm_create_params, llm_update_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NoneType, NotGiven
 from .._utils import (
     maybe_transform,
     async_maybe_transform,
 )
 from .._compat import cached_property
 from .._resource import SyncAPIResource, AsyncAPIResource
@@ -20,26 +20,28 @@
     to_streamed_response_wrapper,
     async_to_raw_response_wrapper,
     async_to_streamed_response_wrapper,
 )
 from .._base_client import (
     make_request_options,
 )
+from ..types.llm_response import LlmResponse
+from ..types.llm_list_response import LlmListResponse
 
-__all__ = ["Llm", "AsyncLlm"]
+__all__ = ["LlmResource", "AsyncLlmResource"]
 
 
-class Llm(SyncAPIResource):
+class LlmResource(SyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> LlmWithRawResponse:
-        return LlmWithRawResponse(self)
+    def with_raw_response(self) -> LlmResourceWithRawResponse:
+        return LlmResourceWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> LlmWithStreamingResponse:
-        return LlmWithStreamingResponse(self)
+    def with_streaming_response(self) -> LlmResourceWithStreamingResponse:
+        return LlmResourceWithStreamingResponse(self)
 
     def create(
         self,
         *,
         begin_message: Optional[str] | NotGiven = NOT_GIVEN,
         general_prompt: Optional[str] | NotGiven = NOT_GIVEN,
         general_tools: Optional[Iterable[llm_create_params.GeneralTool]] | NotGiven = NOT_GIVEN,
@@ -283,22 +285,22 @@
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=NoneType,
         )
 
 
-class AsyncLlm(AsyncAPIResource):
+class AsyncLlmResource(AsyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> AsyncLlmWithRawResponse:
-        return AsyncLlmWithRawResponse(self)
+    def with_raw_response(self) -> AsyncLlmResourceWithRawResponse:
+        return AsyncLlmResourceWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> AsyncLlmWithStreamingResponse:
-        return AsyncLlmWithStreamingResponse(self)
+    def with_streaming_response(self) -> AsyncLlmResourceWithStreamingResponse:
+        return AsyncLlmResourceWithStreamingResponse(self)
 
     async def create(
         self,
         *,
         begin_message: Optional[str] | NotGiven = NOT_GIVEN,
         general_prompt: Optional[str] | NotGiven = NOT_GIVEN,
         general_tools: Optional[Iterable[llm_create_params.GeneralTool]] | NotGiven = NOT_GIVEN,
@@ -542,16 +544,16 @@
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=NoneType,
         )
 
 
-class LlmWithRawResponse:
-    def __init__(self, llm: Llm) -> None:
+class LlmResourceWithRawResponse:
+    def __init__(self, llm: LlmResource) -> None:
         self._llm = llm
 
         self.create = to_raw_response_wrapper(
             llm.create,
         )
         self.retrieve = to_raw_response_wrapper(
             llm.retrieve,
@@ -563,16 +565,16 @@
             llm.list,
         )
         self.delete = to_raw_response_wrapper(
             llm.delete,
         )
 
 
-class AsyncLlmWithRawResponse:
-    def __init__(self, llm: AsyncLlm) -> None:
+class AsyncLlmResourceWithRawResponse:
+    def __init__(self, llm: AsyncLlmResource) -> None:
         self._llm = llm
 
         self.create = async_to_raw_response_wrapper(
             llm.create,
         )
         self.retrieve = async_to_raw_response_wrapper(
             llm.retrieve,
@@ -584,16 +586,16 @@
             llm.list,
         )
         self.delete = async_to_raw_response_wrapper(
             llm.delete,
         )
 
 
-class LlmWithStreamingResponse:
-    def __init__(self, llm: Llm) -> None:
+class LlmResourceWithStreamingResponse:
+    def __init__(self, llm: LlmResource) -> None:
         self._llm = llm
 
         self.create = to_streamed_response_wrapper(
             llm.create,
         )
         self.retrieve = to_streamed_response_wrapper(
             llm.retrieve,
@@ -605,16 +607,16 @@
             llm.list,
         )
         self.delete = to_streamed_response_wrapper(
             llm.delete,
         )
 
 
-class AsyncLlmWithStreamingResponse:
-    def __init__(self, llm: AsyncLlm) -> None:
+class AsyncLlmResourceWithStreamingResponse:
+    def __init__(self, llm: AsyncLlmResource) -> None:
         self._llm = llm
 
         self.create = async_to_streamed_response_wrapper(
             llm.create,
         )
         self.retrieve = async_to_streamed_response_wrapper(
             llm.retrieve,
```

### Comparing `retell_sdk-3.8.0/src/retell/resources/phone_number.py` & `retell_sdk-3.9.0/src/retell/resources/phone_number.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 import httpx
 
-from ..types import (
-    PhoneNumberResponse,
-    PhoneNumberListResponse,
-    phone_number_create_params,
-    phone_number_update_params,
-)
+from ..types import phone_number_create_params, phone_number_update_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NoneType, NotGiven
 from .._utils import (
     maybe_transform,
     async_maybe_transform,
 )
 from .._compat import cached_property
 from .._resource import SyncAPIResource, AsyncAPIResource
@@ -22,26 +17,28 @@
     to_streamed_response_wrapper,
     async_to_raw_response_wrapper,
     async_to_streamed_response_wrapper,
 )
 from .._base_client import (
     make_request_options,
 )
+from ..types.phone_number_response import PhoneNumberResponse
+from ..types.phone_number_list_response import PhoneNumberListResponse
 
-__all__ = ["PhoneNumber", "AsyncPhoneNumber"]
+__all__ = ["PhoneNumberResource", "AsyncPhoneNumberResource"]
 
 
-class PhoneNumber(SyncAPIResource):
+class PhoneNumberResource(SyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> PhoneNumberWithRawResponse:
-        return PhoneNumberWithRawResponse(self)
+    def with_raw_response(self) -> PhoneNumberResourceWithRawResponse:
+        return PhoneNumberResourceWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> PhoneNumberWithStreamingResponse:
-        return PhoneNumberWithStreamingResponse(self)
+    def with_streaming_response(self) -> PhoneNumberResourceWithStreamingResponse:
+        return PhoneNumberResourceWithStreamingResponse(self)
 
     def create(
         self,
         *,
         agent_id: str,
         area_code: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
@@ -205,22 +202,22 @@
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=NoneType,
         )
 
 
-class AsyncPhoneNumber(AsyncAPIResource):
+class AsyncPhoneNumberResource(AsyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> AsyncPhoneNumberWithRawResponse:
-        return AsyncPhoneNumberWithRawResponse(self)
+    def with_raw_response(self) -> AsyncPhoneNumberResourceWithRawResponse:
+        return AsyncPhoneNumberResourceWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> AsyncPhoneNumberWithStreamingResponse:
-        return AsyncPhoneNumberWithStreamingResponse(self)
+    def with_streaming_response(self) -> AsyncPhoneNumberResourceWithStreamingResponse:
+        return AsyncPhoneNumberResourceWithStreamingResponse(self)
 
     async def create(
         self,
         *,
         agent_id: str,
         area_code: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
@@ -386,16 +383,16 @@
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=NoneType,
         )
 
 
-class PhoneNumberWithRawResponse:
-    def __init__(self, phone_number: PhoneNumber) -> None:
+class PhoneNumberResourceWithRawResponse:
+    def __init__(self, phone_number: PhoneNumberResource) -> None:
         self._phone_number = phone_number
 
         self.create = to_raw_response_wrapper(
             phone_number.create,
         )
         self.retrieve = to_raw_response_wrapper(
             phone_number.retrieve,
@@ -407,16 +404,16 @@
             phone_number.list,
         )
         self.delete = to_raw_response_wrapper(
             phone_number.delete,
         )
 
 
-class AsyncPhoneNumberWithRawResponse:
-    def __init__(self, phone_number: AsyncPhoneNumber) -> None:
+class AsyncPhoneNumberResourceWithRawResponse:
+    def __init__(self, phone_number: AsyncPhoneNumberResource) -> None:
         self._phone_number = phone_number
 
         self.create = async_to_raw_response_wrapper(
             phone_number.create,
         )
         self.retrieve = async_to_raw_response_wrapper(
             phone_number.retrieve,
@@ -428,16 +425,16 @@
             phone_number.list,
         )
         self.delete = async_to_raw_response_wrapper(
             phone_number.delete,
         )
 
 
-class PhoneNumberWithStreamingResponse:
-    def __init__(self, phone_number: PhoneNumber) -> None:
+class PhoneNumberResourceWithStreamingResponse:
+    def __init__(self, phone_number: PhoneNumberResource) -> None:
         self._phone_number = phone_number
 
         self.create = to_streamed_response_wrapper(
             phone_number.create,
         )
         self.retrieve = to_streamed_response_wrapper(
             phone_number.retrieve,
@@ -449,16 +446,16 @@
             phone_number.list,
         )
         self.delete = to_streamed_response_wrapper(
             phone_number.delete,
         )
 
 
-class AsyncPhoneNumberWithStreamingResponse:
-    def __init__(self, phone_number: AsyncPhoneNumber) -> None:
+class AsyncPhoneNumberResourceWithStreamingResponse:
+    def __init__(self, phone_number: AsyncPhoneNumberResource) -> None:
         self._phone_number = phone_number
 
         self.create = async_to_streamed_response_wrapper(
             phone_number.create,
         )
         self.retrieve = async_to_streamed_response_wrapper(
             phone_number.retrieve,
```

### Comparing `retell_sdk-3.8.0/src/retell/types/__init__.py` & `retell_sdk-3.9.0/src/retell/types/__init__.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.8.0/src/retell/types/agent_create_params.py` & `retell_sdk-3.9.0/src/retell/types/agent_create_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.8.0/src/retell/types/agent_response.py` & `retell_sdk-3.9.0/src/retell/types/agent_response.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.8.0/src/retell/types/agent_update_params.py` & `retell_sdk-3.9.0/src/retell/types/agent_update_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.8.0/src/retell/types/call_list_params.py` & `retell_sdk-3.9.0/src/retell/types/call_list_params.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 
 class CallListParams(TypedDict, total=False):
     filter_criteria: FilterCriteria
 
     limit: int
     """Limit the number of calls returned."""
 
+    pagination_key: str
+    """The pagination call id to continue fetching the next page of calls.
+
+    If not set, will start from the beginning.
+    """
+
     sort_order: Literal["ascending", "descending"]
     """
     The calls will be sorted by `start_timestamp`, whether to return the calls in
     ascending or descending order.
     """
```

### Comparing `retell_sdk-3.8.0/src/retell/types/call_register_params.py` & `retell_sdk-3.9.0/src/retell/types/call_register_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.8.0/src/retell/types/llm_create_params.py` & `retell_sdk-3.9.0/src/retell/types/llm_create_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.8.0/src/retell/types/llm_response.py` & `retell_sdk-3.9.0/src/retell/types/llm_response.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.8.0/src/retell/types/llm_update_params.py` & `retell_sdk-3.9.0/src/retell/types/llm_update_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.8.0/src/retell/types/phone_number_create_params.py` & `retell_sdk-3.9.0/src/retell/types/phone_number_create_params.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.8.0/src/retell/types/phone_number_response.py` & `retell_sdk-3.9.0/src/retell/types/phone_number_response.py`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.8.0/src/retell/types/register_call_response.py` & `retell_sdk-3.9.0/src/retell/types/register_call_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,14 +67,20 @@
 
       - elevenlabs voices: 16000, 22050, 24000, 44100.
       - openai voices: 24000.
 
       - deepgram voices: 8000, 16000, 24000, 32000, 48000.
     """
 
+    drop_call_if_machine_detected: Optional[bool] = None
+    """If set, will drop the call if machine (voicemail, IVR) is detected.
+
+    If not set, default value of false will apply.
+    """
+
     end_call_after_silence_ms: Optional[int] = None
     """If users stay silent for a period, end the call.
 
     By default, it is set to 600,000 ms (10 min). The minimum value allowed is
     10,000 ms (10 s).
     """
```

### Comparing `retell_sdk-3.8.0/LICENSE` & `retell_sdk-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `retell_sdk-3.8.0/pyproject.toml` & `retell_sdk-3.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "retell-sdk"
-version = "3.8.0"
+version = "3.9.0"
 description = "The official Python library for the retell API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Retell", email = "founders@retellai.com" },
 ]
 dependencies = [
```

### Comparing `retell_sdk-3.8.0/PKG-INFO` & `retell_sdk-3.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: retell-sdk
-Version: 3.8.0
+Version: 3.9.0
 Summary: The official Python library for the retell API
 Project-URL: Homepage, https://github.com/RetellAI/retell-python-sdk
 Project-URL: Repository, https://github.com/RetellAI/retell-python-sdk
 Author-email: Retell <founders@retellai.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -265,15 +265,15 @@
         print(line)
 ```
 
 The context manager is required so that the response will reliably be closed.
 
 ### Making custom/undocumented requests
 
-This library is typed for convenient access the documented API.
+This library is typed for convenient access to the documented API.
 
 If you need to access undocumented endpoints, params, or response properties, the library can still be used.
 
 #### Undocumented endpoints
 
 To make requests to undocumented endpoints, you can make requests using `client.get`, `client.post`, and other
 http verbs. Options on the client will be respected (such as retries) will be respected when making this
```

