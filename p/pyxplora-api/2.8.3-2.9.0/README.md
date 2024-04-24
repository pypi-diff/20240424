# Comparing `tmp/pyxplora_api-2.8.3.tar.gz` & `tmp/pyxplora_api-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxplora_api-2.8.3.tar", last modified: Sat Jun 10 09:35:41 2023, max compression
+gzip compressed data, was "pyxplora_api-2.9.0.tar", last modified: Mon Sep 25 17:34:36 2023, max compression
```

## Comparing `pyxplora_api-2.8.3.tar` & `pyxplora_api-2.9.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:35:41.428478 pyxplora_api-2.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    35587 2023-06-10 09:35:41.428478 pyxplora_api-2.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34609 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 09:35:41.428478 pyxplora_api-2.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:35:41.424478 pyxplora_api-2.8.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:35:41.428478 pyxplora_api-2.8.3/src/pyxplora_api/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/const.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/const_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/exception_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    44320 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/gql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/gql_handler_async.py
--rw-r--r--   0 runner    (1001) docker     (123)   118669 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (123)    64798 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/gql_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/graphql_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/handler_gql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16180 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/pyxplora.py
--rw-r--r--   0 runner    (1001) docker     (123)    27431 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/pyxplora_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30909 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/pyxplora_api_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-06-10 09:35:06.000000 pyxplora_api-2.8.3/src/pyxplora_api/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 09:35:41.428478 pyxplora_api-2.8.3/src/pyxplora_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    35587 2023-06-10 09:35:41.000000 pyxplora_api-2.8.3/src/pyxplora_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-10 09:35:41.000000 pyxplora_api-2.8.3/src/pyxplora_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 09:35:41.000000 pyxplora_api-2.8.3/src/pyxplora_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-10 09:35:41.000000 pyxplora_api-2.8.3/src/pyxplora_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-10 09:35:41.000000 pyxplora_api-2.8.3/src/pyxplora_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 17:34:36.670457 pyxplora_api-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-09-25 17:34:24.000000 pyxplora_api-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    35587 2023-09-25 17:34:36.670457 pyxplora_api-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    34609 2023-09-25 17:34:24.000000 pyxplora_api-2.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-25 17:34:36.670457 pyxplora_api-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2023-09-25 17:34:24.000000 pyxplora_api-2.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 17:34:36.666457 pyxplora_api-2.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 17:34:36.670457 pyxplora_api-2.9.0/src/pyxplora_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2023-09-25 17:34:24.000000 pyxplora_api-2.9.0/src/pyxplora_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2023-09-25 17:34:24.000000 pyxplora_api-2.9.0/src/pyxplora_api/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2023-09-25 17:34:24.000000 pyxplora_api-2.9.0/src/pyxplora_api/const_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2023-09-25 17:34:24.000000 pyxplora_api-2.9.0/src/pyxplora_api/exception_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43769 2023-09-25 17:34:24.000000 pyxplora_api-2.9.0/src/pyxplora_api/gql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24755 2023-09-25 17:34:24.000000 pyxplora_api-2.9.0/src/pyxplora_api/gql_handler_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119082 2023-09-25 17:34:24.000000 pyxplora_api-2.9.0/src/pyxplora_api/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64798 2023-09-25 17:34:24.000000 pyxplora_api-2.9.0/src/pyxplora_api/gql_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2023-09-25 17:34:24.000000 pyxplora_api-2.9.0/src/pyxplora_api/graphql_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2023-09-25 17:34:24.000000 pyxplora_api-2.9.0/src/pyxplora_api/handler_gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2023-09-25 17:34:24.000000 pyxplora_api-2.9.0/src/pyxplora_api/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15932 2023-09-25 17:34:24.000000 pyxplora_api-2.9.0/src/pyxplora_api/pyxplora.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27383 2023-09-25 17:34:24.000000 pyxplora_api-2.9.0/src/pyxplora_api/pyxplora_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30861 2023-09-25 17:34:24.000000 pyxplora_api-2.9.0/src/pyxplora_api/pyxplora_api_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2023-09-25 17:34:24.000000 pyxplora_api-2.9.0/src/pyxplora_api/status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 17:34:36.670457 pyxplora_api-2.9.0/src/pyxplora_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    35587 2023-09-25 17:34:36.000000 pyxplora_api-2.9.0/src/pyxplora_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2023-09-25 17:34:36.000000 pyxplora_api-2.9.0/src/pyxplora_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 17:34:36.000000 pyxplora_api-2.9.0/src/pyxplora_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2023-09-25 17:34:36.000000 pyxplora_api-2.9.0/src/pyxplora_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2023-09-25 17:34:36.000000 pyxplora_api-2.9.0/src/pyxplora_api.egg-info/top_level.txt
```

### Comparing `pyxplora_api-2.8.3/LICENSE` & `pyxplora_api-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.3/PKG-INFO` & `pyxplora_api-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxplora_api
-Version: 2.8.3
+Version: 2.9.0
 Summary: Python Xplora® Api
 Home-page: https://github.com/Ludy87/pyxplora_api
 Author: Ludy87
 Author-email: android@astra-g.org
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Ludy87/pyxplora_api/issues
 Keywords: api xplora watch
@@ -127,15 +127,15 @@
 | getWatchChats(wuid: str, offset: int = 0, limit: int = 0, msgId: str = "")                               | list[dict[str, any]]: | "msgId", "type", "sender_id", "sender_name", "receiver_id", receiver_name", "data_text", data_sender_name", "create" |
 | getWatchChatsRaw(wuid: str, offset: int = 0, limit: int = 0, msgId: str = "", show_del_msg: bool = True) | list[dict[str, any]]: |
 | getSWInfo(wuid: str)                                                                                     | dict[str, any]:       |
 | getWatchState(wuid: str)                                                                                 | dict[str, any]:       |
 
 ## Watch: Location Infos
 
-| Function                                                      | Result Type           | Retrun        |
+| Function                                                      | Result Type           | Return        |
 | ------------------------------------------------------------- | --------------------- | ------------- |
 | getWatchLastLocation(wuid: str, withAsk: bool = False)        | dict[str, any]:       |               |
 | getWatchLocate(wuid: str)                                     | dict[str, any]:       |               |
 | getWatchLocateType(wuid: str)                                 | str:                  | GPS/WIFI/CELL |
 | getWatchSafeZones(wuid: str)                                  | list[dict[str, any]]: |               |
 | getWatchIsInSafeZone(wuid: str)                               | bool:                 |               |
 | getWatchSafeZoneLabel(wuid: str)                              | str:                  |               |
@@ -491,15 +491,15 @@
 | Online Status                    | read       | str  |                                                 |
 | Unread Msg Count                 | read       | int  | ?BUG? Result is always 0                        |
 | Chats                            | read       | list | Don't all chats - confused                      |
 | last locate                      | read       | dict |                                                 |
 | locate Type                      | read       | str  | GPS/WIFI/CELL                                   |
 | locate now                       | read       | dict |                                                 |
 | is in Safezone                   | read       | bool |                                                 |
-| Safezone Lable                   | read       | str  |                                                 |
+| Safezone Label                   | read       | str  |                                                 |
 | Safezone                         | read/write | list |                                                 |
 | track Interval                   | read       | int  |                                                 |
 | ask Watch Locate                 | read       | bool |                                                 |
 | silents                          | read       | list | get all/enable/disable - enable all/disable all |
 | sendText                         | read       | bool | sender: logged User                             |
 | shutdown                         | read       | bool | only admins                                     |
 | reboot                           | read       | bool | only admins                                     |
```

### Comparing `pyxplora_api-2.8.3/README.md` & `pyxplora_api-2.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 | getWatchChats(wuid: str, offset: int = 0, limit: int = 0, msgId: str = "")                               | list[dict[str, any]]: | "msgId", "type", "sender_id", "sender_name", "receiver_id", receiver_name", "data_text", data_sender_name", "create" |
 | getWatchChatsRaw(wuid: str, offset: int = 0, limit: int = 0, msgId: str = "", show_del_msg: bool = True) | list[dict[str, any]]: |
 | getSWInfo(wuid: str)                                                                                     | dict[str, any]:       |
 | getWatchState(wuid: str)                                                                                 | dict[str, any]:       |
 
 ## Watch: Location Infos
 
-| Function                                                      | Result Type           | Retrun        |
+| Function                                                      | Result Type           | Return        |
 | ------------------------------------------------------------- | --------------------- | ------------- |
 | getWatchLastLocation(wuid: str, withAsk: bool = False)        | dict[str, any]:       |               |
 | getWatchLocate(wuid: str)                                     | dict[str, any]:       |               |
 | getWatchLocateType(wuid: str)                                 | str:                  | GPS/WIFI/CELL |
 | getWatchSafeZones(wuid: str)                                  | list[dict[str, any]]: |               |
 | getWatchIsInSafeZone(wuid: str)                               | bool:                 |               |
 | getWatchSafeZoneLabel(wuid: str)                              | str:                  |               |
@@ -464,15 +464,15 @@
 | Online Status                    | read       | str  |                                                 |
 | Unread Msg Count                 | read       | int  | ?BUG? Result is always 0                        |
 | Chats                            | read       | list | Don't all chats - confused                      |
 | last locate                      | read       | dict |                                                 |
 | locate Type                      | read       | str  | GPS/WIFI/CELL                                   |
 | locate now                       | read       | dict |                                                 |
 | is in Safezone                   | read       | bool |                                                 |
-| Safezone Lable                   | read       | str  |                                                 |
+| Safezone Label                   | read       | str  |                                                 |
 | Safezone                         | read/write | list |                                                 |
 | track Interval                   | read       | int  |                                                 |
 | ask Watch Locate                 | read       | bool |                                                 |
 | silents                          | read       | list | get all/enable/disable - enable all/disable all |
 | sendText                         | read       | bool | sender: logged User                             |
 | shutdown                         | read       | bool | only admins                                     |
 | reboot                           | read       | bool | only admins                                     |
```

### Comparing `pyxplora_api-2.8.3/setup.py` & `pyxplora_api-2.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+"""setup."""
 import configparser
 
 import setuptools
 
-with open("README.md") as fh:
+with open("README.md", encoding="utf8") as fh:
     long_description = fh.read()
 
-with open("./src/pyxplora_api/const_version.py") as f:
+with open("./src/pyxplora_api/const_version.py", encoding="utf8") as f:
     config_string = "[dummy_section]\n" + f.read()
     config = configparser.ConfigParser()
     config.read_string(config_string)
     version = config["dummy_section"]["VERSION"].strip('"')
 
 requirements_array = []
-with open("requirements.txt") as my_file:
+with open("requirements.txt", encoding="utf8") as my_file:
     for line in my_file:
         requirements_array.append(line.replace("\n", ""))
 
 setuptools.setup(
     name="pyxplora_api",
     version=version,
     author="Ludy87",
```

### Comparing `pyxplora_api-2.8.3/src/pyxplora_api/exception_classes.py` & `pyxplora_api-2.9.0/src/pyxplora_api/exception_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 from enum import Enum
 
 
 class ErrorMSG(Enum):
-    """Enum class for error messages"""
+    """Enum class for error messages."""
 
     SERVER_ERR = "Cannot connect to the server."
     LOGIN_ERR = "Login to Xplora® API failed. Check your input!\n{}"
     PHONE_MAIL_ERR = "Phone Number or Email address not exist"
 
 
 class Error(Exception):
-    """Base class for all Exceptions"""
+    """Base class for all Exceptions."""
 
     pass
 
 
 class NoAdminError(Error):
     """Exception raised when a user is not an administrator."""
```

### Comparing `pyxplora_api-2.8.3/src/pyxplora_api/gql_handler.py` & `pyxplora_api-2.9.0/src/pyxplora_api/gql_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from __future__ import annotations
 
 import logging
-from typing import Any, Dict
 
-from . import gql_mutations as gm
-from . import gql_queries as gq
+from . import gql_mutations as gm, gql_queries as gq
 from .const import ENDPOINT
 from .exception_classes import LoginError, NoAdminError
 from .graphql_client import GraphqlClient
 from .handler_gql import HandlerGQL
 from .model import Chats
 from .status import EmailAndPhoneVerificationTypeV2, NormalStatus, UserContactType
 
@@ -39,16 +37,16 @@
         timeZone: str,
         email: str | None = None,
         signup: bool = True,
     ) -> None:
         super().__init__(countryPhoneNumber, phoneNumber, password, userLang, timeZone, email, signup)
 
     def runGqlQuery(
-        self, query: str, variables: dict[str, Any] | None = None, operation_name: str | None = None
-    ) -> Dict[str, Any]:
+        self, query: str, variables: dict[str, any] | None = None, operation_name: str | None = None
+    ) -> dict[str, any]:
         """Execute a GraphQL query or mutation.
 
         Args:
             query (str): The GraphQL query string to be executed.
             variables (dict, optional): The variables to be passed to the query. Defaults to None.
             operation_name (str, optional): The name of the operation to be executed. Defaults to None.
 
@@ -61,48 +59,46 @@
         if query is None:
             raise Exception("GraphQL guery string MUST NOT be empty!")
         # Add Xplora® API headers
         requestHeaders = self.getRequestHeaders("application/json; charset=UTF-8")
         # create GQLClient
         gqlClient = GraphqlClient(endpoint=ENDPOINT, headers=requestHeaders)
         # execute QUERY|MUTATION
-        data: dict[str, Any] = gqlClient.execute(query=query, variables=variables, operation_name=operation_name)
+        data: dict[str, any] = gqlClient.execute(query=query, variables=variables, operation_name=operation_name)
         return data
 
     def runAuthorizedGqlQuery(
-        self, query: str, variables: dict[str, Any] | None = None, operation_name: str | None = None
-    ) -> Dict[str, Any]:
-        """
-        This function executes a GraphQL query that requires authorization.
+        self, query: str, variables: dict[str, any] | None = None, operation_name: str | None = None
+    ) -> dict[str, any]:
+        """This function executes a GraphQL query that requires authorization.
 
         Args:
             query (str): The GraphQL query string to be executed.
-            variables (dict[str, Any], optional): Variables to be passed along with the GraphQL query. Defaults to None.
+            variables (dict[str, any], optional): Variables to be passed along with the GraphQL query. Defaults to None.
             operation_name (str, optional): Name of the operation being executed. Defaults to None.
 
         Returns:
-            dict[str, Any]: A dictionary representing the response from the executed GraphQL query.
+            dict[str, any]: A dictionary representing the response from the executed GraphQL query.
 
         Raises:
             Exception: If the accessToken is None and signup flag is not set.
 
         """
         if self.accessToken is None and self.signup:
             self.login()
         # Run GraphQL query and return
         return self.runGqlQuery(query, variables, operation_name)
 
-    def login(self) -> Dict[str, Any]:
-        """
-        This method logs the user into the Xplora API by executing a GraphQL mutation `signInWithEmailOrPhone`.
+    def login(self) -> dict[str, any]:
+        """This method logs the user into the Xplora API by executing a GraphQL mutation `signInWithEmailOrPhone`.
         The user is identified by the `variables` property of the `Client` instance, which should contain the
         email or phone number and the password for the user.
 
         Returns:
-            dict[str, Any]: A dictionary representing the JSON response from the Xplora API. The relevant data for
+            dict[str, any]: A dictionary representing the JSON response from the Xplora API. The relevant data for
             the user is stored in the `Client` instance's `issueToken`, `sessionId`, `userId`, and `accessToken`
             properties.
         """
         dataAll = self.runGqlQuery(gm.SIGN_M.get("signInWithEmailOrPhoneM", ""), self.variables, "signInWithEmailOrPhone")
         if dataAll is None:
             return
         errors = dataAll.get("errors", None)
@@ -117,248 +113,235 @@
         self.issueToken = signIn
         self.sessionId = self.issueToken["id"]
         self.userId = self.issueToken["user"]["id"]
         self.accessToken = self.issueToken["token"]
 
         return self.issueToken
 
-    def isAdmin(self, wuid: str, query: str, variables: dict[str, Any], key: str) -> bool:
-        """
-        This method determines whether the currently logged-in user is an admin for the specified watch user.
+    def isAdmin(self, wuid: str, query: str, variables: dict[str, any], key: str) -> bool:
+        """This method determines whether the currently logged-in user is an admin for the specified watch user.
 
         Args:
             wuid (str): The id of the watch user for which the admin status of the current user should be determined.
             query (str): The GraphQL query that should be executed to determine the admin status of the current user.
-            variables (dict[str, Any]): The variables for the GraphQL query.
+            variables (dict[str, any]): The variables for the GraphQL query.
             key (str): The key in the JSON response from the Xplora API that represents the admin status of the
             current user.
 
         Returns:
             bool: `True` if the current user is an admin for the specified watch user, `False` otherwise.
 
         Raises:
             NoAdminError: If the current user is not an admin for the specified watch user.
         """
-        contacts: dict[str, Any] = self.getWatchUserContacts(wuid)
+        contacts: dict[str, any] = self.getWatchUserContacts(wuid)
         for contact in contacts["contacts"]["contacts"]:
             try:
                 id = contact["contactUser"]["id"]
-            except KeyError and TypeError:
+            except (KeyError, TypeError):
                 id = None
             if self.userId == id:
                 if contact["guardianType"] == "FIRST":
-                    data: dict[str, Any] = self.runAuthorizedGqlQuery(query, variables, key).get("data", {})
-                    for k in data.keys():
+                    data: dict[str, any] = self.runAuthorizedGqlQuery(query, variables, key).get("data", {})
+                    for k in data:
                         if k.upper() == key.upper():
                             return data.get(k, False)
         raise NoAdminError()
 
     ########## SECTION QUERY start ##########
 
-    def askWatchLocate(self, wuid: str) -> Dict[str, Any]:
-        """
-        Ask the watch for its location.
+    def askWatchLocate(self, wuid: str) -> dict[str, any]:
+        """Ask the watch for its location.
 
         Args:
             wuid (str): The watch identifier.
 
         Returns:
-            dict[str, Any]: A dictionary containing the response of the query, with a key "askWatchLocate".
+            dict[str, any]: A dictionary containing the response of the query, with a key "askWatchLocate".
         """
-        data: dict[str, Any] = self.runAuthorizedGqlQuery(gq.WATCH_Q.get("askLocateQ", ""), {"uid": wuid}, "AskWatchLocate")
+        data: dict[str, any] = self.runAuthorizedGqlQuery(gq.WATCH_Q.get("askLocateQ", ""), {"uid": wuid}, "AskWatchLocate")
         errors = data.get("errors", [])
         if errors:
             self.errors.append({"function": "askWatchLocate", "errors": errors})
-        res: dict[str, Any] = data.get("data", {})
+        res: dict[str, any] = data.get("data", {})
         if res["askWatchLocate"] is not None:
             return res
         return {"askWatchLocate": False}
 
-    def getWatchUserContacts(self, wuid: str) -> Dict[str, Any]:
-        """
-        Get the user contacts associated with the watch.
+    def getWatchUserContacts(self, wuid: str) -> dict[str, any]:
+        """Get the user contacts associated with the watch.
 
         Args:
             wuid (str): The watch identifier.
 
         Returns:
-            dict[str, Any]: A dictionary containing the response of the query.
+            dict[str, any]: A dictionary containing the response of the query.
         """
-        data: dict[str, Any] = self.runAuthorizedGqlQuery(gq.WATCH_Q.get("contactsQ", ""), {"uid": wuid}, "Contacts")
+        data: dict[str, any] = self.runAuthorizedGqlQuery(gq.WATCH_Q.get("contactsQ", ""), {"uid": wuid}, "Contacts")
         errors = data.get("errors", [])
         if errors:
             self.errors.append({"function": "getWatchUserContacts", "errors": errors})
         return data.get("data", {})
 
-    def getWatches(self, wuid: str) -> Dict[str, Any]:
-        """
-        Get the watches associated with the user.
+    def getWatches(self, wuid: str) -> dict[str, any]:
+        """Get the watches associated with the user.
 
         Args:
             wuid (str): The watch identifier.
 
         Returns:
-            dict[str, Any]: A dictionary containing the response of the query.
+            dict[str, any]: A dictionary containing the response of the query.
         """
-        data: dict[str, Any] = self.runAuthorizedGqlQuery(gq.WATCH_Q.get("watchesQ", ""), {"uid": wuid}, "Watches")
+        data: dict[str, any] = self.runAuthorizedGqlQuery(gq.WATCH_Q.get("watchesQ", ""), {"uid": wuid}, "Watches")
         errors = data.get("errors", [])
         if errors:
             self.errors.append({"function": "getWatches", "errors": errors})
         return data.get("data", {})
 
-    def getSWInfo(self, qrCode: str) -> Dict[str, Any]:
-        """
-        Get software information for a watch using its QR code.
+    def getSWInfo(self, qrCode: str) -> dict[str, any]:
+        """Get software information for a watch using its QR code.
 
         Args:
             qrCode (str): The QR code of the watch.
 
         Returns:
-            dict[str, Any]: A dictionary containing the response of the query.
+            dict[str, any]: A dictionary containing the response of the query.
         """
-        data: dict[str, Any] = self.runAuthorizedGqlQuery(
+        data: dict[str, any] = self.runAuthorizedGqlQuery(
             gq.WATCH_Q.get("checkByQrCodeQ", ""), {"qrCode": qrCode}, "CheckWatchByQrCode"
         )
         errors = data.get("errors", [])
         if errors:
             self.errors.append({"function": "getSWInfo", "errors": errors})
         return data.get("data", {})
 
-    def getWatchState(self, qrCode: str, qrt: str = "", qrc: str = "") -> Dict[str, Any]:
-        """
-        Get the state of a watch using its QR code.
+    def getWatchState(self, qrCode: str, qrt: str = "", qrc: str = "") -> dict[str, any]:
+        """Get the state of a watch using its QR code.
 
         Args:
             qrCode (str): The QR code of the watch.
             qrt (str, optional): The QR type. Defaults to "".
             qrc (str, optional): The QR code. Defaults to "".
 
         Returns:
-            dict[str, Any]: A dictionary containing the response of the query.
+            dict[str, any]: A dictionary containing the response of the query.
         """
         variables = {}
         if qrCode:
             variables["qrCode"] = qrCode
         if qrt:
             variables["qrt"] = qrt
         if qrc:
             variables["qrc"] = qrc
-        data: dict[str, Any] = self.runAuthorizedGqlQuery(gq.WATCH_Q.get("stateQ", ""), variables, "WatchState")
+        data: dict[str, any] = self.runAuthorizedGqlQuery(gq.WATCH_Q.get("stateQ", ""), variables, "WatchState")
         errors = data.get("errors", [])
         if errors:
             self.errors.append({"function": "getWatchState", "errors": errors})
         return data.get("data", {})
 
-    def getWatchLastLocation(self, wuid: str) -> Dict[str, Any]:
-        """
-        Get the last location of a watch.
+    def getWatchLastLocation(self, wuid: str) -> dict[str, any]:
+        """Get the last location of a watch.
 
         Args:
             wuid (str): The unique identifier of the watch.
 
         Returns:
-            dict[str, Any]: A dictionary containing the response of the query.
+            dict[str, any]: A dictionary containing the response of the query.
         """
-        data: dict[str, Any] = self.runAuthorizedGqlQuery(gq.WATCH_Q.get("locateQ", ""), {"uid": wuid}, "WatchLastLocate")
+        data: dict[str, any] = self.runAuthorizedGqlQuery(gq.WATCH_Q.get("locateQ", ""), {"uid": wuid}, "WatchLastLocate")
         errors = data.get("errors", [])
         if errors:
             self.errors.append({"function": "getWatchLastLocation", "errors": errors})
         return data.get("data", {})
 
-    def trackWatch(self, wuid: str) -> Dict[str, Any]:
-        """
-        Track a watch.
+    def trackWatch(self, wuid: str) -> dict[str, any]:
+        """Track a watch.
 
         Args:
             wuid (str): The unique identifier of the watch.
 
         Returns:
-            dict[str, Any]: A dictionary containing the response of the query.
+            dict[str, any]: A dictionary containing the response of the query.
         """
-        data: dict[str, Any] = self.runAuthorizedGqlQuery(gq.WATCH_Q.get("trackQ", ""), {"uid": wuid}, "TrackWatch")
+        data: dict[str, any] = self.runAuthorizedGqlQuery(gq.WATCH_Q.get("trackQ", ""), {"uid": wuid}, "TrackWatch")
         errors = data.get("errors", [])
         if errors:
             self.errors.append({"function": "trackWatch", "errors": errors})
         res = data.get("data", {})
         if res.get("trackWatch", {"trackWatch": -1}):
             return res
         return {"trackWatch": -1}
 
-    def getAlarmTime(self, wuid: str) -> Dict[str, Any]:
+    def getAlarmTime(self, wuid: str) -> dict[str, any]:
         """Get the alarm time of a watch.
 
         Args:
             wuid (str): The unique identifier of the watch.
 
         Returns:
             dict: A dictionary containing the response of the query.
         """
         return self.runAuthorizedGqlQuery(gq.WATCH_Q.get("alarmsQ", ""), {"uid": wuid}, "Alarms").get("data", {})
 
-    def getWifi(self, wuid: str) -> Dict[str, Any]:
+    def getWifi(self, wuid: str) -> dict[str, any]:
         """Get the Wi-Fi information of a watch.
 
         Args:
             wuid (str): The unique identifier of the watch.
 
         Returns:
             dict: A dictionary containing the response of the query.
         """
         return self.runAuthorizedGqlQuery(gq.WATCH_Q.get("getWifisQ", ""), {"uid": wuid}, "GetWifis").get("data", {})
 
-    def unReadChatMsgCount(self, wuid: str) -> Dict[str, Any]:
-        """
-        Get the count of unread chat messages for a watch.
+    def unReadChatMsgCount(self, wuid: str) -> dict[str, any]:
+        """Get the count of unread chat messages for a watch.
 
         Args:
             wuid (str): The unique identifier of the watch.
 
         Returns:
             dict: A dictionary containing the response of the query.
         """
         return self.runAuthorizedGqlQuery(gq.WATCH_Q.get("unReadChatMsgCountQ", ""), {"uid": wuid}, "UnReadChatMsgCount").get(
             "data", {}
         )
 
-    def safeZones(self, wuid: str) -> Dict[str, Any]:
-        """
-        Get the safe zones for a watch.
+    def safeZones(self, wuid: str) -> dict[str, any]:
+        """Get the safe zones for a watch.
 
         Args:
             wuid (str): The unique identifier of the watch.
 
         Returns:
             dict: A dictionary containing the response of the query.
         """
         return self.runAuthorizedGqlQuery(gq.WATCH_Q.get("safeZonesQ", ""), {"uid": wuid}, "SafeZones").get("data", {})
 
-    def safeZoneGroups(self) -> Dict[str, Any]:
-        """
-        Get the safe zone groups.
+    def safeZoneGroups(self) -> dict[str, any]:
+        """Get the safe zone groups.
 
         Returns:
             dict: A dictionary containing the response of the query.
         """
         return self.runAuthorizedGqlQuery(gq.WATCH_Q.get("safeZoneGroupsQ", ""), {}, "SafeZoneGroups").get("data", {})
 
-    def silentTimes(self, wuid: str) -> Dict[str, Any]:
-        """
-        Get the silent times for a watch.
+    def silentTimes(self, wuid: str) -> dict[str, any]:
+        """Get the silent times for a watch.
 
         Args:
             wuid (str): The unique identifier of the watch.
 
         Returns:
             dict: A dictionary containing the response of the query.
         """
         return self.runAuthorizedGqlQuery(gq.WATCH_Q.get("silentTimesQ", ""), {"uid": wuid}, "SlientTimes").get("data", {})
 
-    def chats(self, wuid: str, offset: int = 0, limit: int = 0, msgId: str = "", asObject=False) -> Dict[str, Any]:
-        """
-        Get the chat messages for a watch.
+    def chats(self, wuid: str, offset: int = 0, limit: int = 0, msgId: str = "", asObject=False) -> dict[str, any]:
+        """Get the chat messages for a watch.
 
         Args:
             wuid (str): The unique identifier of the watch.
             offset (int, optional): The number of messages to skip.
             limit (int, optional): The maximum number of messages to return.
             msgId (str, optional): The message identifier to start from.
             asObject (bool, optional): Return the data as a Chats object if True.
@@ -374,218 +357,203 @@
                 _LOGGER.error(res.get("errors", {}))
                 return Chats.from_dict(res.get("data", {}))
             return {}
         if asObject:
             return Chats.from_dict(res.get("data", {}))
         return res.get("data", {})
 
-    def fetchChatImage(self, wuid: str, msgId: str) -> Dict[str, Any]:
-        """
-        Fetches a chat image.
+    def fetchChatImage(self, wuid: str, msgId: str) -> dict[str, any]:
+        """Fetches a chat image.
 
         Args:
             wuid (str): The ID of the watch.
             msgId (str): The ID of the message.
 
         Returns:
-            Dict[str, Any]: The data of the image.
+            dict[str, any]: The data of the image.
         """
         return self.runAuthorizedGqlQuery(
             gq.WATCH_Q.get("fetchChatImageQ", ""), {"uid": wuid, "msgId": msgId}, "FetchChatImage"
         ).get("data", {})
 
-    def fetchChatMp3(self, wuid: str, msgId: str) -> Dict[str, Any]:
-        """
-        Fetches a chat mp3.
+    def fetchChatMp3(self, wuid: str, msgId: str) -> dict[str, any]:
+        """Fetches a chat mp3.
 
         Args:
             wuid (str): The ID of the watch.
             msgId (str): The ID of the message.
 
         Returns:
-            Dict[str, Any]: The data of the mp3.
+            dict[str, any]: The data of the mp3.
         """
         return self.runAuthorizedGqlQuery(
             gq.WATCH_Q.get("fetchChatMp3Q", ""), {"uid": wuid, "msgId": msgId}, "FetchChatMp3"
         ).get("data", {})
 
-    def fetchChatShortVideo(self, wuid: str, msgId: str) -> Dict[str, Any]:
-        """
-        Fetches a chat short video.
+    def fetchChatShortVideo(self, wuid: str, msgId: str) -> dict[str, any]:
+        """Fetches a chat short video.
 
         Args:
             wuid (str): The ID of the watch.
             msgId (str): The ID of the message.
 
         Returns:
-            Dict[str, Any]: The data of the short video.
+            dict[str, any]: The data of the short video.
         """
         return self.runAuthorizedGqlQuery(
             gq.WATCH_Q.get("fetchChatShortVideoQ", ""), {"uid": wuid, "msgId": msgId}, "FetchChatShortVideo"
         ).get("data", {})
 
-    def fetchChatShortVideoCover(self, wuid: str, msgId: str) -> Dict[str, Any]:
-        """
-        Fetches a chat short video cover.
+    def fetchChatShortVideoCover(self, wuid: str, msgId: str) -> dict[str, any]:
+        """Fetches a chat short video cover.
 
         Args:
             wuid (str): The ID of the watch.
             msgId (str): The ID of the message.
 
         Returns:
-            Dict[str, Any]: The data of the short video cover.
+            dict[str, any]: The data of the short video cover.
         """
         return self.runAuthorizedGqlQuery(
             gq.WATCH_Q.get("fetchChatShortVideoCoverQ", ""), {"uid": wuid, "msgId": msgId}, "FetchChatShortVideoCover"
         ).get("data", {})
 
-    def fetchChatVoice(self, wuid: str, msgId: str) -> Dict[str, Any]:
-        """
-        Fetches a chat voice.
+    def fetchChatVoice(self, wuid: str, msgId: str) -> dict[str, any]:
+        """Fetches a chat voice.
 
         Args:
             wuid (str): The ID of the watch.
             msgId (str): The ID of the message.
 
         Returns:
-            Dict[str, Any]: The data of the voice.
+            dict[str, any]: The data of the voice.
         """
         return self.runAuthorizedGqlQuery(
             gq.WATCH_Q.get("fetchChatVoiceQ", ""), {"uid": wuid, "msgId": msgId}, "FetchChatVoice"
         ).get("data", {})
 
-    def watchImei(self, imei: str, qrCode: str, deviceKey: str) -> Dict[str, Any]:
-        """
-        Retrieve data for a watch with a given IMEI.
+    def watchImei(self, imei: str, qrCode: str, deviceKey: str) -> dict[str, any]:
+        """Retrieve data for a watch with a given IMEI.
 
         Args:
             imei (str): IMEI of the watch to retrieve data for.
             qrCode (str): QR code associated with the watch.
             deviceKey (str): Key associated with the device.
 
         Returns:
-            Dict[str, Any]: Data for the watch with the given IMEI.
+            dict[str, any]: Data for the watch with the given IMEI.
         """
         return self.runAuthorizedGqlQuery(
             gq.WATCH_Q.get("imeiQ", ""), {"imei": imei, "qrCode": qrCode, "deviceKey": deviceKey}, "WatchImei"
         ).get("data", {})
 
-    def getWatchLocHistory(self, wuid: str, date: int, tz: str, limit: int) -> Dict[str, Any]:
-        """
-        Retrieve the location history for a watch with a given WUID.
+    def getWatchLocHistory(self, wuid: str, date: int, tz: str, limit: int) -> dict[str, any]:
+        """Retrieve the location history for a watch with a given WUID.
 
         Args:
             wuid (str): WUID of the watch to retrieve location history for.
             date (int): Date for the location history (in UNIX timestamp format).
             tz (str): Time zone for the location history.
             limit (int): Maximum number of locations to retrieve.
 
         Returns:
-            Dict[str, Any]: Location history for the watch with the given WUID.
+            dict[str, any]: Location history for the watch with the given WUID.
         """
         return self.runAuthorizedGqlQuery(
             gq.WATCH_Q.get("locHistoryQ", ""), {"uid": wuid, "date": date, "tz": tz, "limit": limit}, "LocHistory"
         ).get("data", {})
 
-    def watchesDynamic(self) -> Dict[str, Any]:
-        """
-        Retrieve dynamic data for all watches.
+    def watchesDynamic(self) -> dict[str, any]:
+        """Retrieve dynamic data for all watches.
 
         Returns:
-            Dict[str, Any]: Dynamic data for all watches.
+            dict[str, any]: Dynamic data for all watches.
         """
         return self.runAuthorizedGqlQuery(gq.WATCH_Q.get("watchesDynamicQ", ""), {}, "WatchesDynamic").get("data", {})
 
-    def coinHistory(self, wuid: str, start: int, end: int, type: str, offset: int, limit: int) -> Dict[str, Any]:
-        """
-        Retrieve coin history for a watch with a given WUID.
+    def coinHistory(self, wuid: str, start: int, end: int, type: str, offset: int, limit: int) -> dict[str, any]:
+        """Retrieve coin history for a watch with a given WUID.
 
         Args:
             wuid (str): WUID of the watch to retrieve coin history for.
             start (int): Start of the time range for the coin history (in UNIX timestamp format).
             end (int): End of the time range for the coin history (in UNIX timestamp format).
             type (str): Type of coin history to retrieve.
             offset (int): Offset for the coin history.
             limit (int): Maximum number of coins to retrieve.
 
         Returns:
-            Dict[str, Any]: Coin history for the watch with the given WUID.
+            dict[str, any]: Coin history for the watch with the given WUID.
         """
         return self.runAuthorizedGqlQuery(
             gq.XCOIN_Q.get("historyQ", ""),
             {"uid": wuid, "start": start, "end": end, "type": type, "offset": offset, "limit": limit},
             "CoinHistory",
         ).get("data", {})
 
-    def reminders(self, wuid: str) -> Dict[str, Any]:
-        """
-        Get reminder data for a given user.
+    def reminders(self, wuid: str) -> dict[str, any]:
+        """Get reminder data for a given user.
 
         Args:
             wuid (str): The user id for which the reminder data is to be retrieved.
 
         Returns:
-            Dict[str, Any]: The reminder data for the given user.
+            dict[str, any]: The reminder data for the given user.
         """
         return self.runAuthorizedGqlQuery(gq.XMOVE_Q.get("remindersQ", ""), {"uid": wuid}, "Reminders").get("data", {})
 
-    def groups(self, isCampaign: bool) -> Dict[str, Any]:
-        """
-        Get card group data.
+    def groups(self, isCampaign: bool) -> dict[str, any]:
+        """Get card group data.
 
         Args:
             isCampaign (bool): Whether to retrieve card group data for campaigns or not.
 
         Returns:
-            Dict[str, Any]: The card group data.
+            dict[str, any]: The card group data.
         """
         return self.runAuthorizedGqlQuery(gq.CARD_Q.get("groupsQ", ""), {"isCampaign": isCampaign}, "CardGroups").get(
             "data", {}
         )
 
-    def dynamic(self) -> Dict[str, Any]:
-        """
-        Get dynamic card data.
+    def dynamic(self) -> dict[str, any]:
+        """Get dynamic card data.
 
         Returns:
-            Dict[str, Any]: The dynamic card data.
+            dict[str, any]: The dynamic card data.
         """
         return self.runAuthorizedGqlQuery(gq.CARD_Q.get("dynamicQ", ""), {}, "DynamicCards").get("data", {})
 
-    def staticCard(self) -> Dict[str, Any]:
-        """
-        Get dynamic card data.
+    def staticCard(self) -> dict[str, any]:
+        """Get dynamic card data.
 
         Returns:
-            Dict[str, Any]: The dynamic card data.
+            dict[str, any]: The dynamic card data.
         """
         return self.runAuthorizedGqlQuery(gq.CARD_Q.get("staticQ", ""), {}, "StaticCard").get("data", {})
 
-    def familyInfo(self, wuid: str, watchId: str, tz: str, date: int) -> Dict[str, Any]:
-        """
-        Get family information for a given user.
+    def familyInfo(self, wuid: str, watchId: str, tz: str, date: int) -> dict[str, any]:
+        """Get family information for a given user.
 
         Args:
             wuid (str): The user id for which the family information is to be retrieved.
             watchId (str): The watch id associated with the user.
             tz (str): The timezone of the user.
             date (int): The date for which the family information is to be retrieved.
 
         Returns:
-            Dict[str, Any]: The family information for the given user.
+            dict[str, any]: The family information for the given user.
         """
         return self.runAuthorizedGqlQuery(
             gq.FAMILY_Q.get("infoQ", ""), {"uid": wuid, "watchId": watchId, "tz": tz, "date": date}, "FamilyInfo"
         ).get("data", {})
 
     def getMyTotalInfo(
         self, wuid: str, tz: str, date: int, start: int, end: int, type: str, offset: int, limit: int
-    ) -> Dict[str, Any]:
-        """
-        Retrieve total information for the given user.
+    ) -> dict[str, any]:
+        """Retrieve total information for the given user.
 
         Args:
             wuid (str): The user's unique identifier.
             tz (str): Timezone identifier.
             date (int): Date as an integer.
             start (int): Start time as an integer.
             end (int): End time as an integer.
@@ -600,17 +568,16 @@
             gq.MYINFO_Q.get("getMyTotalInfoQ", ""),
             {"uid": wuid, "tz": tz, "date": date, "start": start, "end": end, "type": type, "offset": offset, "limit": limit},
             "GetMyTotalInfo",
         ).get("data", {})
 
     def myInfoWithCoinHistory(
         self, wuid: str, start: int, end: int, tz: str, type: str, offset: int, limit: int
-    ) -> Dict[str, Any]:
-        """
-        Retrieve information for the given user with coin history.
+    ) -> dict[str, any]:
+        """Retrieve information for the given user with coin history.
 
         Args:
             wuid (str): The user's unique identifier.
             start (int): Start time as an integer.
             end (int): End time as an integer.
             tz (str): Timezone identifier.
             type (str): Type of information to retrieve.
@@ -622,257 +589,239 @@
         """
         return self.runAuthorizedGqlQuery(
             gq.MYINFO_Q.get("myInfoWithCoinHistoryQ", ""),
             {"uid": wuid, "start": start, "end": end, "tz": tz, "type": type, "offset": offset, "limit": limit},
             "MyInfoWithCoinHistory",
         ).get("data", {})
 
-    def getMyInfo(self) -> Dict[str, Any]:
-        """
-        Retrieve information for the logged in user.
+    def getMyInfo(self) -> dict[str, any]:
+        """Retrieve information for the logged in user.
 
         Returns:
             dict: Information retrieved for the logged in user, including the data field.
         """
         # Profil from login Account
         return self.runAuthorizedGqlQuery(gq.MYINFO_Q.get("readQ", ""), {}, "ReadMyInfo").get("data", {})
 
-    def readCampaignProfile(self, wuid: str) -> Dict[str, Any]:
-        """
-        Retrieve campaign profile for the given user.
+    def readCampaignProfile(self, wuid: str) -> dict[str, any]:
+        """Retrieve campaign profile for the given user.
 
         Args:
             wuid (str): The user's unique identifier.
 
         Returns:
             dict: Campaign profile information retrieved for the given user, including the data field.
         """
         return self.runAuthorizedGqlQuery(
             gq.MYINFO_Q.get("readCampaignProfileQ", ""),
             {"uid": wuid},
         ).get("data", {})
 
-    def getReviewStatus(self, wuid: str) -> Dict[str, Any]:
-        """
-        Get the review status for a given user id.
+    def getReviewStatus(self, wuid: str) -> dict[str, any]:
+        """Get the review status for a given user id.
 
         Args:
             wuid (str): The user id for which the review status is to be retrieved.
 
         Returns:
-            Dict[str, Any]: The review status data in dictionary format.
+            dict[str, any]: The review status data in dictionary format.
         """
         return self.runAuthorizedGqlQuery(gq.REVIEW_Q.get("getStatusQ", ""), {"uid": wuid}, "GetReviewStatus").get("data", {})
 
-    def getWatchUserSteps(self, wuid: str, tz: str, date: int) -> Dict[str, Any]:
-        """
-        Get the step count data for a given user id.
+    def getWatchUserSteps(self, wuid: str, tz: str, date: int) -> dict[str, any]:
+        """Get the step count data for a given user id.
 
         Args:
             wuid (str): The user id for which the step count data is to be retrieved.
             tz (str): The time zone of the user.
             date (int): The date for which the step count data is to be retrieved.
 
         Returns:
-            Dict[str, Any]: The step count data in dictionary format.
+            dict[str, any]: The step count data in dictionary format.
         """
-        data: dict[str, Any] = self.runAuthorizedGqlQuery(
+        data: dict[str, any] = self.runAuthorizedGqlQuery(
             gq.STEP_Q.get("userQ", ""), {"uid": wuid, "tz": tz, "date": date}, "UserSteps"
         )
         errors = data.get("errors", [])
         if errors:
             self.errors.append({"function": "getWatchUserSteps", "errors": errors})
         return data.get("data", {})
 
-    def countries(self) -> Dict[str, Any]:
-        """
-        Get the list of countries supported by the service.
+    def countries(self) -> dict[str, any]:
+        """Get the list of countries supported by the service.
 
         Returns:
-            Dict[str, Any]: The list of countries in dictionary format.
+            dict[str, any]: The list of countries in dictionary format.
         """
         return self.runAuthorizedGqlQuery(gq.UTILS_Q.get("countriesQ", ""), {}, "Countries").get("data", {})
 
-    def avatars(self, id: str) -> Dict[str, Any]:
-        """
-        Get the avatar data for a given id.
+    def avatars(self, id: str) -> dict[str, any]:
+        """Get the avatar data for a given id.
 
         Args:
             id (str): The id for which the avatar data is to be retrieved.
 
         Returns:
-            Dict[str, Any]: The avatar data in dictionary format.
+            dict[str, any]: The avatar data in dictionary format.
         """
         return self.runAuthorizedGqlQuery(gq.CAMPAIGN_Q.get("avatarsQ", ""), {"id": id}, "Avatars").get("data", {})
 
-    def getFollowRequestWatchCount(self) -> Dict[str, Any]:
-        """
-        Get the follow request and watch count data.
+    def getFollowRequestWatchCount(self) -> dict[str, any]:
+        """Get the follow request and watch count data.
 
         Returns:
-            Dict[str, Any]: The follow request and watch count data in dictionary format.
+            dict[str, any]: The follow request and watch count data in dictionary format.
         """
         return self.runAuthorizedGqlQuery(
             gq.CAMPAIGN_Q.get("followRequestWatchCountQ", ""), {}, "FollowRequestWatchCount"
         ).get("data", {})
 
-    def campaigns(self, id: str, categoryId: str) -> Dict[str, Any]:
-        """
-        Get the campaigns for the given id and category id.
+    def campaigns(self, id: str, categoryId: str) -> dict[str, any]:
+        """Get the campaigns for the given id and category id.
 
         Args:
             id (str): The id of the campaign.
             categoryId (str): The id of the category.
 
         Returns:
-            Dict[str, Any]: The data returned by the query, in the form of a dictionary.
+            dict[str, any]: The data returned by the query, in the form of a dictionary.
         """
         return self.runAuthorizedGqlQuery(
             gq.CAMPAIGN_Q.get("campaignsQ", ""), {"id": id, "categoryId": categoryId}, "Campaigns"
         ).get("data", {})
 
-    def isSubscribed(self, id: str, wuid: str) -> Dict[str, Any]:
-        """
-        Check if the user with the given wuid is subscribed to the campaign with the given id.
+    def isSubscribed(self, id: str, wuid: str) -> dict[str, any]:
+        """Check if the user with the given wuid is subscribed to the campaign with the given id.
 
         Args:
             id (str): The id of the campaign.
             wuid (str): The wuid of the user.
 
         Returns:
-            Dict[str, Any]: The data returned by the query, in the form of a dictionary.
+            dict[str, any]: The data returned by the query, in the form of a dictionary.
         """
         return self.runAuthorizedGqlQuery(
             gq.CAMPAIGN_Q.get("isSubscribedQ", ""), {"id": id, "uid": wuid}, "IsSubscribedCampaign"
         ).get("data", {})
 
-    def subscribed(self, wuid: str, needDetail: bool) -> Dict[str, Any]:
-        """
-        Get the campaigns that the user with the given wuid is subscribed to.
+    def subscribed(self, wuid: str, needDetail: bool) -> dict[str, any]:
+        """Get the campaigns that the user with the given wuid is subscribed to.
 
         Args:
             wuid (str): The wuid of the user.
             needDetail (bool): Indicates whether detailed information is needed.
 
         Returns:
-            Dict[str, Any]: The data returned by the query, in the form of a dictionary.
+            dict[str, any]: The data returned by the query, in the form of a dictionary.
         """
         return self.runAuthorizedGqlQuery(
             gq.CAMPAIGN_Q.get("subscribedQ", ""), {"uid": wuid, "needDetail": needDetail}, "SubscribedCampaign"
         ).get("data", {})
 
-    def ranks(self, campaignId: str) -> Dict[str, Any]:
-        """
-        Get the ranks for the campaign with the given id.
+    def ranks(self, campaignId: str) -> dict[str, any]:
+        """Get the ranks for the campaign with the given id.
 
         Args:
             campaignId (str): The id of the campaign.
 
         Returns:
-            Dict[str, Any]: The data returned by the query, in the form of a dictionary.
+            dict[str, any]: The data returned by the query, in the form of a dictionary.
         """
         return self.runAuthorizedGqlQuery(gq.CAMPAIGN_Q.get("ranksQ", ""), {"campaignId": campaignId}, "Ranks").get("data", {})
 
-    def conv360IDToO2OID(self, qid: str, deviceId: str) -> Dict[str, Any]:
-        """
-        Convert the 360 ID to the O2O ID.
+    def conv360IDToO2OID(self, qid: str, deviceId: str) -> dict[str, any]:
+        """Convert the 360 ID to the O2O ID.
 
         Args:
             qid (str): The 360 ID.
             deviceId (str): The device ID.
 
         Returns:
-            Dict[str, Any]: The data returned by the query, in the form of a dictionary.
+            dict[str, any]: The data returned by the query, in the form of a dictionary.
         """
         return self.runAuthorizedGqlQuery(
             gq.QUERY.get("conv360IDToO2OIDQ", ""), {"qid": qid, "deviceId": deviceId}, "Conv360IDToO2OID"
         ).get("data", {})
 
-    def getAppVersion(self) -> Dict[str, Any]:
-        """
-        Returns the data for the GetAppVersion query.
+    def getAppVersion(self) -> dict[str, any]:
+        """Returns the data for the GetAppVersion query.
 
         Returns:
-            Dict[str, Any]: The data for the GetAppVersion query.
+            dict[str, any]: The data for the GetAppVersion query.
         """
         return self.runAuthorizedGqlQuery(gq.QUERY.get("getAppVersionQ", ""), {}, "GetAppVersion").get("data", {})
 
-    def watchGroups(self, id: str = "") -> Dict[str, Any]:
-        """
-        Returns the data for the WatchGroups query.
+    def watchGroups(self, id: str = "") -> dict[str, any]:
+        """Returns the data for the WatchGroups query.
 
         Args:
             id (str, optional): The id of the watch group. Defaults to "".
 
         Returns:
-            Dict[str, Any]: The data for the WatchGroups query.
+            dict[str, any]: The data for the WatchGroups query.
         """
         return self.runAuthorizedGqlQuery(gq.WATCHGROUP_Q.get("watchGroupsQ", ""), {"id": id}, "WatchGroups").get("data", {})
 
-    def getStartTrackingWatch(self, wuid: str) -> Dict[str, Any]:
-        """
-        Returns the data for the StartTrackingWatch query.
+    def getStartTrackingWatch(self, wuid: str) -> dict[str, any]:
+        """Returns the data for the StartTrackingWatch query.
 
         Args:
             wuid (str): The wuid of the user.
 
         Returns:
-            Dict[str, Any]: The data for the StartTrackingWatch query.
+            dict[str, any]: The data for the StartTrackingWatch query.
         """
         data = self.runAuthorizedGqlQuery(gq.WATCH_Q.get("startTrackingWatchQ", ""), {"uid": wuid}, "StartTrackingWatch")
         errors: list[dict[str, str]] = data.get("errors", [])
         if errors:
             self.errors.append({"function": "getStartTrackingWatch", "error": errors})
         return data.get("data", {})
 
-    def getEndTrackingWatch(self, wuid: str) -> Dict[str, Any]:
-        """
-        Returns the data for the EndTrackingWatch query.
+    def getEndTrackingWatch(self, wuid: str) -> dict[str, any]:
+        """Returns the data for the EndTrackingWatch query.
 
         Args:
             wuid (str): The wuid of the user.
 
         Returns:
-            Dict[str, Any]: The data for the EndTrackingWatch query.
+            dict[str, any]: The data for the EndTrackingWatch query.
         """
         data = self.runAuthorizedGqlQuery(gq.WATCH_Q.get("endTrackingWatchQ", ""), {"uid": wuid}, "EndTrackingWatch")
         errors: list[dict[str, str]] = data.get("errors", [])
         if errors:
             self.errors.append({"function": "getEndTrackingWatch", "error": errors})
         return data.get("data", {})
 
     def checkEmailOrPhoneExist(
         self, type: UserContactType, email: str = "", countryCode: str = "", phoneNumber: str = ""
-    ) -> Dict[str, bool]:
-        """
-        Check if email or phone number exist.
+    ) -> dict[str, bool]:
+        """Check if email or phone number exist.
 
         Args:
             type (UserContactType): The type of contact to check (email or phone number).
             email (str, optional): The email to check.
             countryCode (str, optional): The country code for the phone number.
             phoneNumber (str, optional): The phone number to check.
 
         Returns:
-            Dict[str, bool]: A dictionary containing the result of the existence check.
+            dict[str, bool]: A dictionary containing the result of the existence check.
         """
         data = self.runAuthorizedGqlQuery(
             gq.UTILS_Q.get("checkEmailOrPhoneExistQ", ""),
             {"type": type.value, "email": email, "countryCode": countryCode, "phoneNumber": phoneNumber},
             "CheckEmailOrPhoneExist",
         )
         return data.get("data", {})
 
     ########## SECTION QUERY end ##########
 
     ########## SECTION MUTATION start ##########
 
     def sendText(self, wuid: str, text: str) -> bool:
-        """
-        Sends a chat text to a specified user.
+        """Sends a chat text to a specified user.
 
         Args:
             wuid (str): The ID of the user.
             text (str): The text to send.
 
         Returns:
             bool: Whether the text was sent successfully.
@@ -882,140 +831,133 @@
                 "data", {}
             )["sendChatText"]
             is not None
         ):
             return True
         return False
 
-    def addStep(self, stepCount: int) -> Dict[str, Any]:
-        """
-        Adds a specified number of steps.
+    def addStep(self, stepCount: int) -> dict[str, any]:
+        """Adds a specified number of steps.
 
         Args:
             stepCount (int): The number of steps to add.
 
         Returns:
             dict: A dictionary containing the data from the response.
         """
         return self.runAuthorizedGqlQuery(gm.STEP_M.get("addM", ""), {"stepCount": stepCount}, "AddStep").get("data", {})
 
     def shutdown(self, wuid: str) -> bool:
-        """
-        Shuts down the system for a specified user.
+        """Shuts down the system for a specified user.
 
         Args:
             wuid (str): The ID of the user.
 
         Returns:
             bool: Whether the system was shut down successfully.
         """
         return self.isAdmin(wuid, gm.WATCH_M.get("shutdownM", ""), {"uid": wuid}, "ShutDown")
 
     def reboot(self, wuid: str) -> bool:
-        """
-        Reboots the system for a specified user.
+        """Reboots the system for a specified user.
 
         Args:
             wuid (str): The ID of the user.
 
         Returns:
             bool: Whether the system was rebooted successfully.
         """
         return self.isAdmin(wuid, gm.WATCH_M.get("rebootM", ""), {"uid": wuid}, "reboot")
 
-    def modifyAlert(self, id: str, yesOrNo: str) -> Dict[str, Any]:
-        """
-        Modifies an alert.
+    def modifyAlert(self, id: str, yesOrNo: str) -> dict[str, any]:
+        """Modifies an alert.
 
         Args:
             id (str): The ID of the alert.
             yesOrNo (str): The value to set for the alert.
 
         Returns:
             dict: A dictionary containing the data from the response.
         """
         return self.runAuthorizedGqlQuery(gm.WATCH_M.get("modifyAlertM", ""), {"uid": id, "remind": yesOrNo}, "modifyAlert")
 
-    def setEnableSilentTime(self, silent_id: str, status: str = NormalStatus.ENABLE.value) -> Dict[str, Any]:
-        """
-        Sets the silent time for a specified user.
+    def setEnableSilentTime(self, silent_id: str, status: str = NormalStatus.ENABLE.value) -> dict[str, any]:
+        """Sets the silent time for a specified user.
 
         Args:
             silent_id (str): The ID of the silent time.
             status (str, optional): The status to set for the silent time. Defaults to `NormalStatus.ENABLE.value`.
 
         Returns:
             dict: A dictionary containing the data from the response.
         """
         return self.runAuthorizedGqlQuery(
             gm.WATCH_M.get("setEnableSlientTimeM", ""), {"silentId": silent_id, "status": status}, "SetEnableSlientTime"
         ).get("data", {})
 
-    def setEnableAlarmTime(self, alarm_id: str, status: str = NormalStatus.ENABLE.value) -> Dict[str, Any]:
-        """
-        Enable or disable alarm time.
+    def setEnableAlarmTime(self, alarm_id: str, status: str = NormalStatus.ENABLE.value) -> dict[str, any]:
+        """Enable or disable alarm time.
 
         Args:
             alarm_id (str): ID of the alarm to modify.
-            status (str, optional): New status for the alarm, either `NormalStatus.ENABLE.value` or `NormalStatus.DISABLE.value`. Defaults to `NormalStatus.ENABLE.value`.
+            status (str, optional):
+                New status for the alarm, either `NormalStatus.ENABLE.value` or `NormalStatus.DISABLE.value`.
+                Defaults to `NormalStatus.ENABLE.value`.
 
         Returns:
-            Dict[str, Any]: Dictionary containing the response data.
+            dict[str, any]: Dictionary containing the response data.
         """
         return self.runAuthorizedGqlQuery(
             gm.WATCH_M.get("modifyAlarmM", ""), {"alarmId": alarm_id, "status": status}, "ModifyAlarm"
         ).get("data", {})
 
-    def setReadChatMsg(self, wuid: str, msgId: str, id: str) -> Dict[str, Any]:
-        """
-        Mark a chat message as read.
+    def setReadChatMsg(self, wuid: str, msgId: str, id: str) -> dict[str, any]:
+        """Mark a chat message as read.
 
         Args:
             wuid (str): ID of the user who sent the chat message.
             msgId (str): ID of the chat message to mark as read.
             id (str): ID of the message in the chat history.
 
         Returns:
-            Dict[str, Any]: Dictionary containing the response data.
+            dict[str, any]: Dictionary containing the response data.
         """
         return self.runAuthorizedGqlQuery(
             gm.WATCH_M.get("setReadChatMsgM", ""), {"uid": wuid, "msgId": msgId, "id": id}, "setReadChatMsg"
         ).get("data", {})
 
-    def submitIncorrectLocationData(self, wuid: str, lat: str, lng: str, timestamp: str) -> Dict[str, Any]:
-        """
-        Submit incorrect location data.
+    def submitIncorrectLocationData(self, wuid: str, lat: str, lng: str, timestamp: str) -> dict[str, any]:
+        """Submit incorrect location data.
 
         Args:
             wuid (str): ID of the user.
             lat (str): Latitude of the location.
             lng (str): Longitude of the location.
             timestamp (str): Timestamp of the location.
 
         Returns:
-            Dict[str, Any]: Dictionary containing the response data.
+            dict[str, any]: Dictionary containing the response data.
         """
         return self.runAuthorizedGqlQuery(
             gm.WATCH_M.get("submitIncorrectLocationDataM", ""),
             {"uid": wuid, "lat": lat, "lng": lng, "timestamp": timestamp},
             "SubmitIncorrectLocationData",
         ).get("data", {})
 
-    def modifyContact(self, contactId: str, isAdmin: bool, contactName: str = "", fileId: str = "") -> Dict[str, Any]:
-        """
-        Modify a contact.
+    def modifyContact(self, contactId: str, isAdmin: bool, contactName: str = "", fileId: str = "") -> dict[str, any]:
+        """Modify a contact.
 
         Args:
             contactId (str): ID of the contact to modify.
             isAdmin (bool): Whether the contact should be an admin or not.
             contactName (str, optional): New name for the contact. Defaults to "".
             fileId (str, optional): New profile picture for the contact. Defaults to "".
 
         Returns:
-            Dict[str, Any]: Dictionary containing the response data.
+            dict[str, any]: Dictionary containing the response data.
         """
         return self.runAuthorizedGqlQuery(
             gm.WATCH_M.get("modifyContactM", ""),
             {"contactId": contactId, "contactName": contactName, "fileId": fileId, "isAdmin": isAdmin},
         )
 
     def issueEmailOrPhoneCode(
@@ -1023,28 +965,29 @@
         purpose: EmailAndPhoneVerificationTypeV2 = EmailAndPhoneVerificationTypeV2.UNKNOWN__,
         type: UserContactType = UserContactType.UNKNOWN__,
         email: str = "",
         phoneNumber: str = "",
         countryCode: str = "",
         previousToken: str = "",
         lang: str = "",
-    ) -> Dict[str, Any]:
+    ) -> dict[str, any]:
         """Issue a code for email or phone verification.
 
         Args:
-            purpose (EmailAndPhoneVerificationTypeV2, optional): Purpose of the code. Default is EmailAndPhoneVerificationTypeV2.UNKNOWN__.
+            purpose (EmailAndPhoneVerificationTypeV2, optional):
+                Purpose of the code. Default is EmailAndPhoneVerificationTypeV2.UNKNOWN__.
             type (UserContactType, optional): Type of user contact. Default is UserContactType.UNKNOWN__.
             email (str, optional): Email address. Default is an empty string.
             phoneNumber (str, optional): Phone number. Default is an empty string.
             countryCode (str, optional): Country code. Default is an empty string.
             previousToken (str, optional): Previous token. Default is an empty string.
             lang (str, optional): Language. Default is an empty string.
 
         Returns:
-            Dict[str, Any]: Result of the query.
+            dict[str, any]: Result of the query.
         """
         return self.runAuthorizedGqlQuery(
             gm.SIGN_M.get("issueEmailOrPhoneCodeM", ""),
             {
                 "purpose": purpose.value,
                 "type": type.value,
                 "email": email,
@@ -1060,101 +1003,98 @@
         self,
         countryPhoneCode: str = "",
         phoneNumber: str = "",
         password: str = "",
         name: str = "",
         emailAddress: str = "",
         emailConsent: int = -1,
-    ) -> Dict[str, Any]:
+    ) -> dict[str, any]:
         """Sign up with email and phone, version 2.
 
         Args:
             countryPhoneCode (str, optional): Country phone code. Default is an empty string.
             phoneNumber (str, optional): Phone number. Default is an empty string.
             password (str, optional): Password. Default is an empty string.
             name (str, optional): Name. Default is an empty string.
             emailAddress (str, optional): Email address. Default is an empty string.
             emailConsent (int, optional): Email consent. Default is -1.
 
         Returns:
-            Dict[str, Any]: Result of the query.
+            dict[str, any]: Result of the query.
         """
         return self.runAuthorizedGqlQuery(
             gm.SIGN_M.get("signUpWithEmailAndPhoneV2M", ""),
             {
                 "countryPhoneCode": countryPhoneCode,
                 "phoneNumber": phoneNumber,
                 "password": password,
                 "name": name,
                 "emailAddress": emailAddress,
                 "emailConsent": emailConsent,
             },
             "SignUpWithEmailAndPhoneV2",
         )
 
-    def verifyCaptcha(self, captchaString: str = "", type: str = "") -> Dict[str, Any]:
-        """
-        Verify a given captcha string.
+    def verifyCaptcha(self, captchaString: str = "", type: str = "") -> dict[str, any]:
+        """Verify a given captcha string.
 
         Args:
             captchaString (str, optional): The captcha string to verify.
             type (str, optional): The type of the captcha to verify.
 
         Returns:
-            Dict[str, Any]: The result of the `verifyCaptcha` query.
+            dict[str, any]: The result of the `verifyCaptcha` query.
         """
         return self.runAuthorizedGqlQuery(
             gm.SIGN_M.get("verifyCaptchaM", ""), {"captchaString": captchaString, "type": type}, "verifyCaptcha"
         )
 
     def verifyEmailOrPhoneCode(
         self,
         type: UserContactType = UserContactType.UNKNOWN__,
         email: str = "",
         phoneNumber: str = "",
         countryCode: str = "",
         verifyCode: str = "",
         verificationToken: str = "",
-    ) -> Dict[str, Any]:
-        """
-        Verify a given email or phone code.
+    ) -> dict[str, any]:
+        """Verify a given email or phone code.
 
         Args:
             type (UserContactType, optional): The type of the email or phone to verify.
             email (str, optional): The email to verify.
             phoneNumber (str, optional): The phone number to verify.
             countryCode (str, optional): The country code of the phone number to verify.
             verifyCode (str, optional): The code to verify.
             verificationToken (str, optional): The verification token to use.
 
         Returns:
-            Dict[str, Any]: The result of the `verifyEmailOrPhoneCode` query.
+            dict[str, any]: The result of the `verifyEmailOrPhoneCode` query.
         """
         return self.runAuthorizedGqlQuery(
             gm.SIGN_M.get("verifyEmailOrPhoneCodeM", ""),
             {
                 "type": type.value,
                 "email": email,
                 "phoneNumber": phoneNumber,
                 "countryCode": countryCode,
                 "verifyCode": verifyCode,
                 "verificationToken": verificationToken,
             },
             "verifyEmailOrPhoneCode",
         )
 
-    async def deleteMessageFromApp(self, wuid: str, msgId: str) -> Dict[str, Any]:
-        """
-        Delete a message from the app.
+    async def deleteMessageFromApp(self, wuid: str, msgId: str) -> dict[str, any]:
+        """Delete a message from the app.
 
         Args:
             wuid (str): The WUID of the message to delete.
             msgId (str): The ID of the message to delete.
 
         Returns:
-            Dict[str, Any]: The result of the `deleteChatMessage` query.
+            dict[str, any]: The result of the `deleteChatMessage` query.
         """
         return self.runAuthorizedGqlQuery(
             gm.WATCH_M.get("deleteChatMessageM", ""), {"uid": wuid, "msgId": msgId}, "DeleteChatMessage"
         ).get("data", {})
 
     ########## SECTION MUTATION end ##########
```

### Comparing `pyxplora_api-2.8.3/src/pyxplora_api/gql_handler_async.py` & `pyxplora_api-2.9.0/src/pyxplora_api/gql_handler_async.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
+"""GQL Handler."""
 from __future__ import annotations
 
 import logging
-from typing import Any, Dict
 
 import aiohttp
 
-from . import gql_mutations as gm
-from . import gql_queries as gq
+from . import gql_mutations as gm, gql_queries as gq
 from .const import API_KEY, API_SECRET, ENDPOINT
 from .exception_classes import LoginError, NoAdminError
 from .graphql_client import GraphqlClient
 from .handler_gql import HandlerGQL
 from .model import Chats
 from .status import EmailAndPhoneVerificationTypeV2, NormalStatus, UserContactType
 
@@ -31,41 +30,41 @@
     ) -> None:
         self._session = session
         super().__init__(countryPhoneNumber, phoneNumber, password, userLang, timeZone, email, signup)
 
     async def runGqlQuery_a(
         self,
         query: str,
-        variables: dict[str, Any] | None = None,
+        variables: dict[str, any] | None = None,
         operation_name: str | None = None,
-    ) -> Dict[str, Any]:
+    ) -> dict[str, any]:
         if query is None:
             raise Exception("GraphQL guery string MUST NOT be empty!")
         # Add Xplora® API headers
         requestHeaders = self.getRequestHeaders("application/json; charset=UTF-8")
         # create GQLClient
         gqlClient = GraphqlClient(endpoint=ENDPOINT, headers=requestHeaders)
         # execute QUERY|MUTATION
         if self._session:
-            data: dict[str, Any] = await gqlClient.ha_execute_async(
+            data: dict[str, any] = await gqlClient.ha_execute_async(
                 query=query, variables=variables, operation_name=operation_name, session=self._session
             )
         else:
-            data: dict[str, Any] = await gqlClient.execute_async(
+            data: dict[str, any] = await gqlClient.execute_async(
                 query=query, variables=variables, operation_name=operation_name
             )
         return data
 
     async def runAuthorizedGqlQuery_a(
-        self, query: str, variables: dict[str, Any] | None = None, operation_name: str | None = None
-    ) -> Dict[str, Any]:
+        self, query: str, variables: dict[str, any] | None = None, operation_name: str | None = None
+    ) -> dict[str, any]:
         # Run GraphQL query and return
         return await self.runGqlQuery_a(query, variables, operation_name)
 
-    async def login_a(self, key, sec) -> Dict[str, Any]:
+    async def login_a(self, key, sec) -> dict[str, any]:
         if key and sec:
             self._API_KEY = key
             self._API_SECRET = sec
         dataAll = await self.runGqlQuery_a(
             gm.SIGN_M.get("signInWithEmailOrPhoneM", ""), self.variables, "signInWithEmailOrPhone"
         )
         if dataAll is None:
@@ -91,213 +90,213 @@
         if w360:
             if w360.get("token") and w360.get("secret"):
                 self._API_KEY = w360.get("token", API_KEY)
                 self._API_SECRET = w360.get("secret", API_SECRET)
 
         return self.issueToken, self.refreshToken
 
-    async def isAdmin_a(self, wuid: str, query: str, variables: dict[str, Any], key: str) -> bool:
-        contacts: dict[str, Any] = await self.getWatchUserContacts_a(wuid)
+    async def isAdmin_a(self, wuid: str, query: str, variables: dict[str, any], key: str) -> bool:
+        contacts: dict[str, any] = await self.getWatchUserContacts_a(wuid)
         for contact in contacts["contacts"]["contacts"]:
             try:
                 id = contact["contactUser"]["id"]
-            except KeyError and TypeError:
+            except (KeyError, TypeError):
                 id = None
             if self.userId == id:
                 if contact["guardianType"] == "FIRST":
-                    data: dict[str, Any] = (await self.runGqlQuery_a(query, variables, key)).get("data", {})
-                    for k in data.keys():
+                    data: dict[str, any] = (await self.runGqlQuery_a(query, variables, key)).get("data", {})
+                    for k in data:
                         if k.upper() == key.upper():
                             return data.get(k, False)
         raise NoAdminError()
 
     ########## SECTION QUERY start ##########
 
-    async def askWatchLocate_a(self, wuid: str) -> Dict[str, Any]:
-        data: dict[str, Any] = await self.runGqlQuery_a(gq.WATCH_Q.get("askLocateQ", ""), {"uid": wuid}, "AskWatchLocate")
+    async def askWatchLocate_a(self, wuid: str) -> dict[str, any]:
+        data: dict[str, any] = await self.runGqlQuery_a(gq.WATCH_Q.get("askLocateQ", ""), {"uid": wuid}, "AskWatchLocate")
         errors = data.get("errors", [])
         if errors:
             self.errors.append({"function": "askWatchLocate", "errors": errors})
-        res: dict[str, Any] = data.get("data", {})
+        res: dict[str, any] = data.get("data", {})
         if res.get("askWatchLocate", None) is not None:
             return res
         return {"askWatchLocate": False}
 
-    async def getWatchUserContacts_a(self, wuid: str) -> Dict[str, Any]:
+    async def getWatchUserContacts_a(self, wuid: str) -> dict[str, any]:
         # Contacts from ownUser
-        data: dict[str, Any] = await self.runGqlQuery_a(gq.WATCH_Q.get("contactsQ", ""), {"uid": wuid}, "Contacts")
+        data: dict[str, any] = await self.runGqlQuery_a(gq.WATCH_Q.get("contactsQ", ""), {"uid": wuid}, "Contacts")
         errors = data.get("errors", [])
         if errors:
             self.errors.append({"function": "getWatchUserContacts", "errors": errors})
         return data.get("data", {})
 
-    async def getWatches_a(self, wuid: str) -> Dict[str, Any]:
-        data: dict[str, Any] = await self.runGqlQuery_a(gq.WATCH_Q.get("watchesQ", ""), {"uid": wuid}, "Watches")
+    async def getWatches_a(self, wuid: str) -> dict[str, any]:
+        data: dict[str, any] = await self.runGqlQuery_a(gq.WATCH_Q.get("watchesQ", ""), {"uid": wuid}, "Watches")
         errors = data.get("errors", [])
         if errors:
             self.errors.append({"function": "getWatches", "errors": errors})
         return data.get("data", {})
 
-    async def getSWInfo_a(self, qrCode: str) -> Dict[str, Any]:
-        data: dict[str, Any] = await self.runGqlQuery_a(
+    async def getSWInfo_a(self, qrCode: str) -> dict[str, any]:
+        data: dict[str, any] = await self.runGqlQuery_a(
             gq.WATCH_Q.get("checkByQrCodeQ", ""), {"qrCode": qrCode}, "CheckWatchByQrCode"
         )
         errors = data.get("errors", [])
         if errors:
             self.errors.append({"function": "getSWInfo", "errors": errors})
         return data.get("data", {})
 
-    async def getWatchState_a(self, qrCode: str, qrt: str = "", qrc: str = "") -> Dict[str, Any]:
+    async def getWatchState_a(self, qrCode: str, qrt: str = "", qrc: str = "") -> dict[str, any]:
         variables = {}
         if qrCode:
             variables["qrCode"] = qrCode
         if qrt:
             variables["qrt"] = qrt
         if qrc:
             variables["qrc"] = qrc
-        data: dict[str, Any] = await self.runGqlQuery_a(gq.WATCH_Q.get("stateQ", ""), variables, "WatchState")
+        data: dict[str, any] = await self.runGqlQuery_a(gq.WATCH_Q.get("stateQ", ""), variables, "WatchState")
         errors = data.get("errors", [])
         if errors:
             self.errors.append({"function": "getWatchState", "errors": errors})
         return data.get("data", {})
 
-    async def getWatchLastLocation_a(self, wuid: str) -> Dict[str, Any]:
-        data: dict[str, Any] = await self.runGqlQuery_a(gq.WATCH_Q.get("locateQ", ""), {"uid": wuid}, "WatchLastLocate")
+    async def getWatchLastLocation_a(self, wuid: str) -> dict[str, any]:
+        data: dict[str, any] = await self.runGqlQuery_a(gq.WATCH_Q.get("locateQ", ""), {"uid": wuid}, "WatchLastLocate")
         errors = data.get("errors", [])
         if errors:
             self.errors.append({"function": "getWatchLastLocation", "errors": errors})
         return data.get("data", {})
 
-    async def trackWatch_a(self, wuid: str) -> Dict[str, Any]:
+    async def trackWatch_a(self, wuid: str) -> dict[str, any]:
         # tracking time - seconds
-        data: dict[str, Any] = await self.runGqlQuery_a(gq.WATCH_Q.get("trackQ", ""), {"uid": wuid}, "TrackWatch")
+        data: dict[str, any] = await self.runGqlQuery_a(gq.WATCH_Q.get("trackQ", ""), {"uid": wuid}, "TrackWatch")
         errors = data.get("errors", [])
         if errors:
             self.errors.append({"function": "trackWatch", "errors": errors})
         res = data.get("data", {})
         if res.get("trackWatch", {"trackWatch": -1}):
             return res
         return {"trackWatch": -1}
 
-    async def getAlarmTime_a(self, wuid: str) -> Dict[str, Any]:
+    async def getAlarmTime_a(self, wuid: str) -> dict[str, any]:
         return (await self.runGqlQuery_a(gq.WATCH_Q.get("alarmsQ", ""), {"uid": wuid}, "Alarms")).get("data", {})
 
-    async def getWifi_a(self, wuid: str) -> Dict[str, Any]:
+    async def getWifi_a(self, wuid: str) -> dict[str, any]:
         # without function?
         return (await self.runGqlQuery_a(gq.WATCH_Q.get("getWifisQ", ""), {"uid": wuid}, "GetWifis")).get("data", {})
 
-    async def unReadChatMsgCount_a(self, wuid: str) -> Dict[str, Any]:
+    async def unReadChatMsgCount_a(self, wuid: str) -> dict[str, any]:
         return (await self.runGqlQuery_a(gq.WATCH_Q.get("unReadChatMsgCountQ", ""), {"uid": wuid}, "UnReadChatMsgCount")).get(
             "data", {}
         )
 
-    async def safeZones_a(self, wuid: str) -> Dict[str, Any]:
+    async def safeZones_a(self, wuid: str) -> dict[str, any]:
         return (await self.runGqlQuery_a(gq.WATCH_Q.get("safeZonesQ", ""), {"uid": wuid}, "SafeZones")).get("data", {})
 
-    async def safeZoneGroups_a(self) -> Dict[str, Any]:
+    async def safeZoneGroups_a(self) -> dict[str, any]:
         return (await self.runGqlQuery_a(gq.WATCH_Q.get("safeZoneGroupsQ", ""), {}, "SafeZoneGroups")).get("data", {})
 
-    async def silentTimes_a(self, wuid: str) -> Dict[str, Any]:
+    async def silentTimes_a(self, wuid: str) -> dict[str, any]:
         return (await self.runGqlQuery_a(gq.WATCH_Q.get("silentTimesQ", ""), {"uid": wuid}, "SlientTimes")).get("data", {})
 
     async def chats_a(
         self, wuid: str, offset: int = 0, limit: int = 0, msgId: str = "", asObject=False
-    ) -> Dict[str, Any] | Chats:
+    ) -> dict[str, any] | Chats:
         # ownUser id
         res: dict = await self.runGqlQuery_a(
             gq.WATCH_Q.get("chatsQ", ""), {"uid": wuid, "offset": offset, "limit": limit, "msgId": msgId}, "Chats"
         )
         if res.get("errors", None) or res.get("data", None) is None:
             if asObject:
                 _LOGGER.error(res.get("errors", None))
                 return Chats.from_dict(res.get("data", {}))
             return {}
         if asObject:
             return Chats.from_dict(res.get("data", {}))
         return res.get("data", {})
 
-    async def fetchChatImage_a(self, wuid: str, msgId: str) -> Dict[str, Any]:
+    async def fetchChatImage_a(self, wuid: str, msgId: str) -> dict[str, any]:
         return (
             await self.runGqlQuery_a(gq.WATCH_Q.get("fetchChatImageQ", ""), {"uid": wuid, "msgId": msgId}, "FetchChatImage")
         ).get("data", {})
 
-    async def fetchChatMp3_a(self, wuid: str, msgId: str) -> Dict[str, Any]:
+    async def fetchChatMp3_a(self, wuid: str, msgId: str) -> dict[str, any]:
         return (
             await self.runGqlQuery_a(gq.WATCH_Q.get("fetchChatMp3Q", ""), {"uid": wuid, "msgId": msgId}, "FetchChatMp3")
         ).get("data", {})
 
-    async def fetchChatShortVideo_a(self, wuid: str, msgId: str) -> Dict[str, Any]:
+    async def fetchChatShortVideo_a(self, wuid: str, msgId: str) -> dict[str, any]:
         return (
             await self.runGqlQuery_a(
                 gq.WATCH_Q.get("fetchChatShortVideoQ", ""), {"uid": wuid, "msgId": msgId}, "FetchChatShortVideo"
             )
         ).get("data", {})
 
-    async def fetchChatShortVideoCover_a(self, wuid: str, msgId: str) -> Dict[str, Any]:
+    async def fetchChatShortVideoCover_a(self, wuid: str, msgId: str) -> dict[str, any]:
         return (
             await self.runGqlQuery_a(
                 gq.WATCH_Q.get("fetchChatShortVideoCoverQ", ""), {"uid": wuid, "msgId": msgId}, "FetchChatShortVideoCover"
             )
         ).get("data", {})
 
-    async def fetchChatVoice_a(self, wuid: str, msgId: str) -> Dict[str, Any]:
+    async def fetchChatVoice_a(self, wuid: str, msgId: str) -> dict[str, any]:
         return (
             await self.runGqlQuery_a(gq.WATCH_Q.get("fetchChatVoiceQ", ""), {"uid": wuid, "msgId": msgId}, "FetchChatVoice")
         ).get("data", {})
 
-    async def watchImei_a(self, imei: str, qrCode: str, deviceKey: str) -> Dict[str, Any]:
+    async def watchImei_a(self, imei: str, qrCode: str, deviceKey: str) -> dict[str, any]:
         return (
             await self.runGqlQuery_a(
                 gq.WATCH_Q.get("imeiQ", ""), {"imei": imei, "qrCode": qrCode, "deviceKey": deviceKey}, "WatchImei"
             )
         ).get("data", {})
 
-    async def getWatchLocHistory_a(self, wuid: str, date: int = None, tz: str = None, limit: int = 1) -> Dict[str, Any]:
+    async def getWatchLocHistory_a(self, wuid: str, date: int = None, tz: str = None, limit: int = 1) -> dict[str, any]:
         return (
             await self.runGqlQuery_a(
                 gq.WATCH_Q.get("locHistoryQ", ""), {"uid": wuid, "date": date, "tz": tz, "limit": limit}, "LocHistory"
             )
         ).get("data", {})
 
-    async def watchesDynamic_a(self) -> Dict[str, Any]:
+    async def watchesDynamic_a(self) -> dict[str, any]:
         return (await self.runGqlQuery_a(gq.WATCH_Q.get("watchesDynamicQ", ""), {}, "WatchesDynamic")).get("data", {})
 
-    async def coinHistory_a(self, wuid: str, start: int, end: int, type: str, offset: int, limit: int) -> Dict[str, Any]:
+    async def coinHistory_a(self, wuid: str, start: int, end: int, type: str, offset: int, limit: int) -> dict[str, any]:
         return (
             await self.runGqlQuery_a(
                 gq.XCOIN_Q.get("historyQ", ""),
                 {"uid": wuid, "start": start, "end": end, "type": type, "offset": offset, "limit": limit},
                 "CoinHistory",
             )
         ).get("data", {})
 
-    async def reminders_a(self, wuid: str) -> Dict[str, Any]:
+    async def reminders_a(self, wuid: str) -> dict[str, any]:
         return (await self.runGqlQuery_a(gq.XMOVE_Q.get("remindersQ", ""), {"uid": wuid}, "Reminders")).get("data", {})
 
-    async def groups_a(self, isCampaign: bool) -> Dict[str, Any]:
+    async def groups_a(self, isCampaign: bool) -> dict[str, any]:
         return (await self.runGqlQuery_a(gq.CARD_Q.get("groupsQ", ""), {"isCampaign": isCampaign}, "CardGroups")).get(
             "data", {}
         )
 
-    async def dynamic_a(self) -> Dict[str, Any]:
+    async def dynamic_a(self) -> dict[str, any]:
         return (await self.runGqlQuery_a(gq.CARD_Q.get("dynamicQ", ""), {}, "DynamicCards")).get("data", {})
 
-    async def staticCard_a(self) -> Dict[str, Any]:
+    async def staticCard_a(self) -> dict[str, any]:
         return (await self.runGqlQuery_a(gq.CARD_Q.get("staticQ", ""), {}, "StaticCard")).get("data", {})
 
-    async def familyInfo_a(self, wuid: str, watchId: str, tz: str, date: int) -> Dict[str, Any]:
+    async def familyInfo_a(self, wuid: str, watchId: str, tz: str, date: int) -> dict[str, any]:
         return (
             await self.runGqlQuery_a(
                 gq.FAMILY_Q.get("infoQ", ""), {"uid": wuid, "watchId": watchId, "tz": tz, "date": date}, "FamilyInfo"
             )
         ).get("data", {})
 
     async def getMyTotalInfo_a(
         self, wuid: str, tz: str, date: int, start: int, end: int, type: str, offset: int, limit: int
-    ) -> Dict[str, Any]:
+    ) -> dict[str, any]:
         return (
             await self.runGqlQuery_a(
                 gq.MYINFO_Q.get("getMyTotalInfoQ", ""),
                 {
                     "uid": wuid,
                     "tz": tz,
                     "date": date,
@@ -309,109 +308,109 @@
                 },
                 "GetMyTotalInfo",
             )
         ).get("data", {})
 
     async def myInfoWithCoinHistory_a(
         self, wuid: str, start: int, end: int, tz: str, type: str, offset: int, limit: int
-    ) -> Dict[str, Any]:
+    ) -> dict[str, any]:
         return (
             await self.runGqlQuery_a(
                 gq.MYINFO_Q.get("myInfoWithCoinHistoryQ", ""),
                 {"uid": wuid, "start": start, "end": end, "tz": tz, "type": type, "offset": offset, "limit": limit},
                 "MyInfoWithCoinHistory",
             )
         ).get("data", {})
 
-    async def getMyInfo_a(self) -> Dict[str, Any]:
+    async def getMyInfo_a(self) -> dict[str, any]:
         # Profil from login Account
         return (await self.runGqlQuery_a(gq.MYINFO_Q.get("readQ", ""), {}, "ReadMyInfo")).get("data", {})
 
-    async def readCampaignProfile_a(self, wuid: str) -> Dict[str, Any]:
+    async def readCampaignProfile_a(self, wuid: str) -> dict[str, any]:
         return (
             await self.runGqlQuery_a(
                 gq.MYINFO_Q.get("readCampaignProfileQ", ""),
                 {"uid": wuid},
             )
         ).get("data", {})
 
-    async def getReviewStatus_a(self, wuid: str) -> Dict[str, Any]:
+    async def getReviewStatus_a(self, wuid: str) -> dict[str, any]:
         return (await self.runGqlQuery_a(gq.REVIEW_Q.get("getStatusQ", ""), {"uid": wuid}, "GetReviewStatus")).get("data", {})
 
-    async def getWatchUserSteps_a(self, wuid: str, tz: str, date: int) -> Dict[str, Any]:
-        data: dict[str, Any] = await self.runGqlQuery_a(
+    async def getWatchUserSteps_a(self, wuid: str, tz: str, date: int) -> dict[str, any]:
+        data: dict[str, any] = await self.runGqlQuery_a(
             gq.STEP_Q.get("userQ", ""), {"uid": wuid, "tz": tz, "date": date}, "UserSteps"
         )
         errors = data.get("errors", [])
         if errors:
             self.errors.append({"function": "getWatchUserSteps", "errors": errors})
         return data.get("data", {})
 
-    async def countries_a(self) -> Dict[str, Any]:
+    async def countries_a(self) -> dict[str, any]:
         # Country Support
         return (await self.runGqlQuery_a(gq.UTILS_Q.get("countriesQ", ""), {}, "Countries")).get("data", {})
 
-    async def avatars_a(self, id: str) -> Dict[str, Any]:
+    async def avatars_a(self, id: str) -> dict[str, any]:
         return (await self.runGqlQuery_a(gq.CAMPAIGN_Q.get("avatarsQ", ""), {"id": id}, "Avatars")).get("data", {})
 
-    async def getFollowRequestWatchCount_a(self) -> Dict[str, Any]:
+    async def getFollowRequestWatchCount_a(self) -> dict[str, any]:
         return (
             await self.runGqlQuery_a(gq.CAMPAIGN_Q.get("followRequestWatchCountQ", ""), {}, "FollowRequestWatchCount")
         ).get("data", {})
 
-    async def campaigns_a(self, id: str, categoryId: str) -> Dict[str, Any]:
+    async def campaigns_a(self, id: str, categoryId: str) -> dict[str, any]:
         return (
             await self.runGqlQuery_a(gq.CAMPAIGN_Q.get("campaignsQ", ""), {"id": id, "categoryId": categoryId}, "Campaigns")
         ).get("data", {})
 
-    async def isSubscribed_a(self, id: str, wuid: str) -> Dict[str, Any]:
+    async def isSubscribed_a(self, id: str, wuid: str) -> dict[str, any]:
         return (
             await self.runGqlQuery_a(gq.CAMPAIGN_Q.get("isSubscribedQ", ""), {"id": id, "uid": wuid}, "IsSubscribedCampaign")
         ).get("data", {})
 
-    async def subscribed_a(self, wuid: str, needDetail: bool) -> Dict[str, Any]:
+    async def subscribed_a(self, wuid: str, needDetail: bool) -> dict[str, any]:
         return (
             await self.runGqlQuery_a(
                 gq.CAMPAIGN_Q.get("subscribedQ", ""), {"uid": wuid, "needDetail": needDetail}, "SubscribedCampaign"
             )
         ).get("data", {})
 
-    async def ranks_a(self, campaignId: str) -> Dict[str, Any]:
+    async def ranks_a(self, campaignId: str) -> dict[str, any]:
         return (await self.runGqlQuery_a(gq.CAMPAIGN_Q.get("ranksQ", ""), {"campaignId": campaignId}, "Ranks")).get("data", {})
 
-    async def conv360IDToO2OID_a(self, qid: str, deviceId: str) -> Dict[str, Any]:
+    async def conv360IDToO2OID_a(self, qid: str, deviceId: str) -> dict[str, any]:
         return (
             await self.runGqlQuery_a(
                 gq.QUERY.get("conv360IDToO2OIDQ", ""), {"qid": qid, "deviceId": deviceId}, "Conv360IDToO2OID"
             )
         ).get("data", {})
 
-    async def getAppVersion_a(self) -> Dict[str, Any]:
+    async def getAppVersion_a(self) -> dict[str, any]:
         return (await self.runGqlQuery_a(gq.QUERY.get("getAppVersionQ", ""), {}, "GetAppVersion")).get("data", {})
 
-    async def watchGroups_a(self, id: str = "") -> Dict[str, Any]:
+    async def watchGroups_a(self, id: str = "") -> dict[str, any]:
         return (await self.runGqlQuery_a(gq.WATCHGROUP_Q.get("watchGroupsQ", ""), {"id": id}, "WatchGroups")).get("data", {})
 
-    async def getStartTrackingWatch_a(self, wuid: str) -> Dict[str, Any]:
+    async def getStartTrackingWatch_a(self, wuid: str) -> dict[str, any]:
         data = await self.runGqlQuery_a(gq.WATCH_Q.get("startTrackingWatchQ", ""), {"uid": wuid}, "StartTrackingWatch")
         errors: list[dict[str, str]] = data.get("errors", [])
         if errors:
             self.errors.append({"function": "getStartTrackingWatch", "error": errors})
         return data.get("data", {})
 
-    async def getEndTrackingWatch_a(self, wuid: str) -> Dict[str, Any]:
+    async def getEndTrackingWatch_a(self, wuid: str) -> dict[str, any]:
         data = await self.runGqlQuery_a(gq.WATCH_Q.get("endTrackingWatchQ", ""), {"uid": wuid}, "EndTrackingWatch")
         errors: list[dict[str, str]] = data.get("errors", [])
         if errors:
             self.errors.append({"function": "getEndTrackingWatch", "error": errors})
         return data.get("data", {})
 
     async def checkEmailOrPhoneExist_a(
         self, type: UserContactType, email: str = "", countryCode: str = "", phoneNumber: str = ""
-    ) -> Dict[str, bool]:
+    ) -> dict[str, bool]:
         data: dict[str, dict[str, bool]] = await self.runGqlQuery_a(
             gq.UTILS_Q.get("checkEmailOrPhoneExistQ", ""),
             {"type": type.value, "email": email, "countryCode": countryCode, "phoneNumber": phoneNumber},
             "CheckEmailOrPhoneExist",
         )
         return data.get("data", {})
 
@@ -423,75 +422,75 @@
         # ownUser id
         if (await self.runGqlQuery_a(gm.WATCH_M.get("sendChatTextM", ""), {"uid": wuid, "text": text}, "SendChatText")).get(
             "data", {}
         )["sendChatText"] is not None:
             return True
         return False
 
-    async def addStep_a(self, stepCount: int) -> Dict[str, Any]:
+    async def addStep_a(self, stepCount: int) -> dict[str, any]:
         return (await self.runGqlQuery_a(gm.STEP_M.get("addM", ""), {"stepCount": stepCount}, "AddStep")).get("data", {})
 
     async def shutdown_a(self, wuid: str) -> bool:
         # ownUser id
         return await self.isAdmin_a(wuid, gm.WATCH_M.get("shutdownM", ""), {"uid": wuid}, "ShutDown")
 
     async def reboot_a(self, wuid: str) -> bool:
         # ownUser id
         return await self.isAdmin_a(wuid, gm.WATCH_M.get("rebootM", ""), {"uid": wuid}, "reboot")
 
-    async def modifyAlert_a(self, id: str, yesOrNo: str) -> Dict[str, Any]:
+    async def modifyAlert_a(self, id: str, yesOrNo: str) -> dict[str, any]:
         # function?
         return await self.runGqlQuery_a(gm.WATCH_M.get("modifyAlertM", ""), {"uid": id, "remind": yesOrNo}, "modifyAlert")
 
-    async def setEnableSilentTime_a(self, silent_id: str, status: str = NormalStatus.ENABLE.value) -> Dict[str, Any]:
+    async def setEnableSilentTime_a(self, silent_id: str, status: str = NormalStatus.ENABLE.value) -> dict[str, any]:
         return (
             await self.runGqlQuery_a(
                 gm.WATCH_M.get("setEnableSlientTimeM", ""), {"silentId": silent_id, "status": status}, "SetEnableSlientTime"
             )
         ).get("data", {})
 
-    async def setEnableAlarmTime_a(self, alarm_id: str, status: str = NormalStatus.ENABLE.value) -> Dict[str, Any]:
+    async def setEnableAlarmTime_a(self, alarm_id: str, status: str = NormalStatus.ENABLE.value) -> dict[str, any]:
         return (
             await self.runGqlQuery_a(
                 gm.WATCH_M.get("modifyAlarmM", ""), {"alarmId": alarm_id, "status": status}, "ModifyAlarm"
             )
         ).get("data", {})
 
-    async def setReadChatMsg_a(self, wuid: str, msgId: str, id: str) -> Dict[str, Any]:
+    async def setReadChatMsg_a(self, wuid: str, msgId: str, id: str) -> dict[str, any]:
         return (
             await self.runGqlQuery_a(
                 gm.WATCH_M.get("setReadChatMsgM", ""), {"uid": wuid, "msgId": msgId, "id": id}, "setReadChatMsg"
             )
         ).get("data", {})
 
-    async def submitIncorrectLocationData_a(self, wuid: str, lat: str, lng: str, timestamp: str) -> Dict[str, Any]:
+    async def submitIncorrectLocationData_a(self, wuid: str, lat: str, lng: str, timestamp: str) -> dict[str, any]:
         return (
             await self.runGqlQuery_a(
                 gm.WATCH_M.get("submitIncorrectLocationDataM", ""),
                 {"uid": wuid, "lat": lat, "lng": lng, "timestamp": timestamp},
                 "SubmitIncorrectLocationData",
             )
         ).get("data", {})
 
-    async def modifyContact_a(self, contactId: str, isAdmin: bool, contactName: str = "", fileId: str = "") -> Dict[str, Any]:
+    async def modifyContact_a(self, contactId: str, isAdmin: bool, contactName: str = "", fileId: str = "") -> dict[str, any]:
         return await self.runGqlQuery_a(
             gm.WATCH_M.get("modifyContactM", ""),
             {"contactId": contactId, "contactName": contactName, "fileId": fileId, "isAdmin": isAdmin},
         )
 
     async def issueEmailOrPhoneCode_a(
         self,
         purpose: EmailAndPhoneVerificationTypeV2 = EmailAndPhoneVerificationTypeV2.UNKNOWN__,
         type: UserContactType = UserContactType.UNKNOWN__,
         email: str = "",
         phoneNumber: str = "",
         countryCode: str = "",
         previousToken: str = "",
         lang: str = "",
-    ) -> Dict[str, Any]:
+    ) -> dict[str, any]:
         return await self.runGqlQuery_a(
             gm.SIGN_M.get("issueEmailOrPhoneCodeM", ""),
             {
                 "purpose": purpose.value,
                 "type": type.value,
                 "email": email,
                 "phoneNumber": phoneNumber,
@@ -506,42 +505,42 @@
         self,
         countryPhoneCode: str = "",
         phoneNumber: str = "",
         password: str = "",
         name: str = "",
         emailAddress: str = "",
         emailConsent: int = -1,
-    ) -> Dict[str, Any]:
+    ) -> dict[str, any]:
         return await self.runGqlQuery_a(
             gm.SIGN_M.get("signUpWithEmailAndPhoneV2M", ""),
             {
                 "countryPhoneCode": countryPhoneCode,
                 "phoneNumber": phoneNumber,
                 "password": password,
                 "name": name,
                 "emailAddress": emailAddress,
                 "emailConsent": emailConsent,
             },
             "SignUpWithEmailAndPhoneV2",
         )
 
-    async def verifyCaptcha_a(self, captchaString: str = "", type: str = "") -> Dict[str, Any]:
+    async def verifyCaptcha_a(self, captchaString: str = "", type: str = "") -> dict[str, any]:
         return await self.runGqlQuery_a(
             gm.SIGN_M.get("verifyCaptchaM", ""), {"captchaString": captchaString, "type": type}, "verifyCaptcha"
         )
 
     async def verifyEmailOrPhoneCode_a(
         self,
         type: UserContactType = UserContactType.UNKNOWN__,
         email: str = "",
         phoneNumber: str = "",
         countryCode: str = "",
         verifyCode: str = "",
         verificationToken: str = "",
-    ) -> Dict[str, Any]:
+    ) -> dict[str, any]:
         return await self.runGqlQuery_a(
             gm.SIGN_M.get("verifyEmailOrPhoneCodeM", ""),
             {
                 "type": type.value,
                 "email": email,
                 "phoneNumber": phoneNumber,
                 "countryCode": countryCode,
```

### Comparing `pyxplora_api-2.8.3/src/pyxplora_api/gql_mutations.py` & `pyxplora_api-2.9.0/src/pyxplora_api/gql_mutations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Mutations for Xplora® Api."""
+# pylint: skip-file
 from __future__ import annotations
 
 CAMPAIGN_M: dict[str, str] = {
     "subscribeM": "mutation SubscribeCampaign($id: String!, $uid: String!, $avatarId: String, $fileId: String, $name: String, $gender: Gender, $weight: String, $height: String, $birth: Int, $birthStr: String) {\n  subscribeCampaign(id: $id, uid: $uid, avatarId: $avatarId, fileId: $fileId, name: $name, gender: $gender, weight: $weight, height: $height, birth: $birth, birthStr: $birthStr) {\n    __typename\n    ...SubscribedCampaignFragment\n  }\n}\nfragment SubscribedCampaignFragment on CampaignSubscribed {\n  __typename\n  campaign {\n    __typename\n    id\n  }\n  user {\n    __typename\n    id\n  }\n  avatar {\n    __typename\n    ...FileFragment\n  }\n  profile {\n    __typename\n    ...FileFragment\n  }\n  name\n  subscribedDate\n}\nfragment FileFragment on File {\n  __typename\n  id\n  name\n}",
     "unsubscribeM": "mutation UnsubscribeCampaign($id : String!, $uid : String!) {\n  unsubscribeCampaign(id: $id, uid: $uid)\n}",
     "addAvatarM": "mutation AddAvatar($fileId : String!, $name : String, $listOrder : Int) {\n  addAvatar(fileId: $fileId, name: $name, listOrder: $listOrder) {\n    __typename\n    ...AvatarFragment\n  }\n}\nfragment AvatarFragment on Avatar {\n  __typename\n  id\n  name\n  file {\n    __typename\n    ...FileFragment\n  }\n}\nfragment FileFragment on File {\n  __typename\n  id\n  name\n}",
     "modifyAvatarM": "mutation ModifyAvatar($id: String!, $fileId: String, $name : String, $listOrder : Int) {\n  modifyAvatar(id: $id, fileId: $fileId, name: $name, listOrder: $listOrder)\n}",
@@ -77,14 +79,15 @@
     "removeContactM": "mutation RemoveContact($contactId : String!) {\n  removeContact(contactId: $contactId)\n}",
     "addSilentTimeM": "mutation AddSilentTime($uid: String!, $start: Int!, $end: Int!, $weekRepeat: String!, $description: String, $extra: JSON) {\n  addSilentTime(uid: $uid, start: $start, end: $end, weekRepeat: $weekRepeat, description: $description, extra: $extra) {\n    __typename\n    ...SlientModeFragment\n  }\n}\nfragment SlientModeFragment on SilentMode {\n  __typename\n  id\n  vendorName\n  vendorId\n  watch {\n    __typename\n    ...WatchFragment\n  }\n  user {\n    __typename\n    ...UserFragment\n  }\n  start\n  end\n  weekRepeat\n  description\n  extra\n  start\n  create\n  update\n}\nfragment WatchFragment on Watch {\n  __typename\n  id\n  group {\n    __typename\n    ...WatchGroupFragment\n  }\n  vendor {\n    __typename\n    ...VendorFragment\n  }\n  user {\n    __typename\n    ...UserFragment\n  }\n  name\n  swKey\n  groupName\n  os\n  osName\n  osVersion\n  brand\n  phoneNumber\n  qrCode\n  countryPhoneCode\n  onlineStatus\n  status\n  activated\n  extra\n  create\n  update\n}\nfragment WatchGroupFragment on WatchGroup {\n  __typename\n  id\n  name\n  status\n  extra\n  description\n  create\n  update\n}\nfragment VendorFragment on Vendor {\n  __typename\n  id\n  name\n  status\n  extra\n  description\n  create\n  update\n}\nfragment UserFragment on User {\n  __typename\n  id\n  userId\n  name\n  nickname\n  gender\n  birth\n  birthStr\n  weight\n  height\n  countryCode\n  emailAddress\n  emailConsent\n  countryPhoneCode\n  phoneNumber\n  mobilePhoneNumber\n  emailConfirm\n  status\n  file {\n    __typename\n    ...FileFragment\n  }\n  extra\n  xcoin\n  currentStep\n  totalStep\n  create\n  update\n  children {\n    __typename\n    id\n    guardian {\n      __typename\n      ...SimpleUserFragment\n    }\n    ward {\n      __typename\n      ...SimpleUserFragment\n    }\n  }\n}\nfragment FileFragment on File {\n  __typename\n  id\n  name\n}\nfragment SimpleUserFragment on User {\n  __typename\n  id\n  userId\n  name\n  nickname\n  gender\n  countryCode\n  countryPhoneCode\n  phoneNumber\n  mobilePhoneNumber\n  file {\n    __typename\n    ...FileFragment\n  }\n  xcoin\n  currentStep\n  totalStep\n  extra\n  contacts {\n    __typename\n    ...ContactsFragment\n  }\n}\nfragment ContactsFragment on Contact {\n  __typename\n  id\n  me {\n    __typename\n    ...ContactorFragment\n  }\n  contacter {\n    __typename\n    ...ContactorFragment\n  }\n  phoneNumber\n  extra\n  listOrder\n  file {\n    __typename\n    ...FileFragment\n  }\n  create\n  update\n}\nfragment ContactorFragment on User {\n  __typename\n  id\n  userId\n  name\n  nickname\n  countryCode\n  countryPhoneCode\n  mobilePhoneNumber\n  phoneNumber\n}",
     "modifySilentTimeM": "mutation ModifySilentTime($silentId: String!, $start: Int, $end: Int, $weekRepeat: String, $description: String, $extra: JSON) {\n  modifySilentTime(silentId: $silentId, start: $start, end: $end, weekRepeat: $weekRepeat, description: $description, extra: $extra)\n}",
     "removeSilentTimeM": "mutation RemoveSilentTime($silentId : String!) {\n  removeSilentTime(silentId: $silentId)\n}",
     "setEnableSlientTimeM": "mutation SetEnableSlientTime($silentId : String!, $status: NormalStatus!) {\n  setEnableSilentTime(silentId: $silentId, status: $status)\n}",
     "addSafeZoneM": "mutation AddSafeZone($uid : String!, $groupId: String!, $name : String!, $lat: String!, $lng: String!, $rad: Int!, $address : String!) {\n  addSafeZone(uid: $uid, groupId: $groupId, name: $name, lat: $lat, lng: $lng, rad: $rad, address: $address) {\n    __typename\n    ...SafeZoneFragment\n  }\n}\nfragment SafeZoneFragment on SafeZone {\n  __typename\n  id\n  vendorName\n  vendorId\n  groupName\n  watch {\n    __typename\n    ...WatchFragment\n  }\n  user {\n    __typename\n    ...UserFragment\n  }\n  group {\n    __typename\n    ...SafeZoneGroupFragment\n  }\n  name\n  lat\n  lng\n  rad\n  address\n  description\n  extra\n  create\n  update\n}\nfragment WatchFragment on Watch {\n  __typename\n  id\n  group {\n    __typename\n    ...WatchGroupFragment\n  }\n  vendor {\n    __typename\n    ...VendorFragment\n  }\n  user {\n    __typename\n    ...UserFragment\n  }\n  name\n  swKey\n  groupName\n  os\n  osName\n  osVersion\n  brand\n  phoneNumber\n  qrCode\n  countryPhoneCode\n  onlineStatus\n  status\n  activated\n  extra\n  create\n  update\n}\nfragment WatchGroupFragment on WatchGroup {\n  __typename\n  id\n  name\n  status\n  extra\n  description\n  create\n  update\n}\nfragment VendorFragment on Vendor {\n  __typename\n  id\n  name\n  status\n  extra\n  description\n  create\n  update\n}\nfragment UserFragment on User {\n  __typename\n  id\n  userId\n  name\n  nickname\n  gender\n  birth\n  birthStr\n  weight\n  height\n  countryCode\n  emailAddress\n  emailConsent\n  countryPhoneCode\n  phoneNumber\n  mobilePhoneNumber\n  emailConfirm\n  status\n  file {\n    __typename\n    ...FileFragment\n  }\n  extra\n  xcoin\n  currentStep\n  totalStep\n  create\n  update\n  children {\n    __typename\n    id\n    guardian {\n      __typename\n      ...SimpleUserFragment\n    }\n    ward {\n      __typename\n      ...SimpleUserFragment\n    }\n  }\n}\nfragment FileFragment on File {\n  __typename\n  id\n  name\n}\nfragment SimpleUserFragment on User {\n  __typename\n  id\n  userId\n  name\n  nickname\n  gender\n  countryCode\n  countryPhoneCode\n  phoneNumber\n  mobilePhoneNumber\n  file {\n    __typename\n    ...FileFragment\n  }\n  xcoin\n  currentStep\n  totalStep\n  extra\n  contacts {\n    __typename\n    ...ContactsFragment\n  }\n}\nfragment ContactsFragment on Contact {\n  __typename\n  id\n  me {\n    __typename\n    ...ContactorFragment\n  }\n  contacter {\n    __typename\n    ...ContactorFragment\n  }\n  phoneNumber\n  extra\n  listOrder\n  file {\n    __typename\n    ...FileFragment\n  }\n  create\n  update\n}\nfragment ContactorFragment on User {\n  __typename\n  id\n  userId\n  name\n  nickname\n  countryCode\n  countryPhoneCode\n  mobilePhoneNumber\n  phoneNumber\n}\nfragment SafeZoneGroupFragment on SafeZoneGroup {\n  __typename\n  id\n  name\n  status\n  description\n  create\n  update\n}",
     "removeSafeZoneM": "mutation RemoveSafeZone($zoneId : String!) {\n  removeSafeZone(zoneId: $zoneId)\n}",
+    "modifySafeZone": "mutation modifySafeZone($zoneId: String!, $groupId: String, $name: String, $lat: String, $lng: String, $rad: Int, $address: String, $description: String, $extra: JSON) {\n  modifySafeZone(zoneId: $zoneId, groupId: $groupId, name: $name, lat: $lat, lng: $lng, rad: $rad, address: $address, description: $description, extra: $extra)\n}",
     "addWiFiM": "mutation AddWiFi($uid : String!, $ssid : String!, $name : String, $password : String) {\n  addWiFi(uid: $uid, ssid: $ssid, name: $name, password: $password) {\n    __typename\n    ...WiFiFragment\n  }\n}\nfragment WiFiFragment on WiFi {\n  __typename\n  id\n  name\n  ssid\n  password\n  state\n  create\n  update\n  user {\n    __typename\n    ...UserFragment\n  }\n  watch {\n    __typename\n    ...WatchFragment\n  }\n}\nfragment UserFragment on User {\n  __typename\n  id\n  userId\n  name\n  nickname\n  gender\n  birth\n  birthStr\n  weight\n  height\n  countryCode\n  emailAddress\n  emailConsent\n  countryPhoneCode\n  phoneNumber\n  mobilePhoneNumber\n  emailConfirm\n  status\n  file {\n    __typename\n    ...FileFragment\n  }\n  extra\n  xcoin\n  currentStep\n  totalStep\n  create\n  update\n  children {\n    __typename\n    id\n    guardian {\n      __typename\n      ...SimpleUserFragment\n    }\n    ward {\n      __typename\n      ...SimpleUserFragment\n    }\n  }\n}\nfragment FileFragment on File {\n  __typename\n  id\n  name\n}\nfragment SimpleUserFragment on User {\n  __typename\n  id\n  userId\n  name\n  nickname\n  gender\n  countryCode\n  countryPhoneCode\n  phoneNumber\n  mobilePhoneNumber\n  file {\n    __typename\n    ...FileFragment\n  }\n  xcoin\n  currentStep\n  totalStep\n  extra\n  contacts {\n    __typename\n    ...ContactsFragment\n  }\n}\nfragment ContactsFragment on Contact {\n  __typename\n  id\n  me {\n    __typename\n    ...ContactorFragment\n  }\n  contacter {\n    __typename\n    ...ContactorFragment\n  }\n  phoneNumber\n  extra\n  listOrder\n  file {\n    __typename\n    ...FileFragment\n  }\n  create\n  update\n}\nfragment ContactorFragment on User {\n  __typename\n  id\n  userId\n  name\n  nickname\n  countryCode\n  countryPhoneCode\n  mobilePhoneNumber\n  phoneNumber\n}\nfragment WatchFragment on Watch {\n  __typename\n  id\n  group {\n    __typename\n    ...WatchGroupFragment\n  }\n  vendor {\n    __typename\n    ...VendorFragment\n  }\n  user {\n    __typename\n    ...UserFragment\n  }\n  name\n  swKey\n  groupName\n  os\n  osName\n  osVersion\n  brand\n  phoneNumber\n  qrCode\n  countryPhoneCode\n  onlineStatus\n  status\n  activated\n  extra\n  create\n  update\n}\nfragment WatchGroupFragment on WatchGroup {\n  __typename\n  id\n  name\n  status\n  extra\n  description\n  create\n  update\n}\nfragment VendorFragment on Vendor {\n  __typename\n  id\n  name\n  status\n  extra\n  description\n  create\n  update\n}",
     "modifyWiFiM": "mutation ModifyWiFi($wifiId : String!, $name : String, $password : String) {\n  modifyWiFi(wifiId: $wifiId, name: $name, password: $password)\n}",
     "removeWiFiM": "mutation RemoveWiFi($wifiId : String!) {\n  removeWiFi(wifiId: $wifiId)\n}",
     "submitIncorrectLocationDataM": "mutation SubmitIncorrectLocationData($uid: String!, $lat: String!, $lng: String!, $timestamp: String!) {\n  submitIncorrectLocationData(uid: $uid, lat: $lat, lng: $lng, timestamp : $timestamp)\n}",
     "setUserSettingM": "mutation setUserSetting($uid: String!, $actionKey: String!, $enabled: Boolean!) {\n  setUserSetting(uid: $uid, actionKey: $actionKey, enabled: $enabled)\n}",
 }
 WATCHGROUP_M: dict[str, str] = {
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyxplora_api-2.8.3/src/pyxplora_api/gql_queries.py` & `pyxplora_api-2.9.0/src/pyxplora_api/gql_queries.py`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.3/src/pyxplora_api/graphql_client.py` & `pyxplora_api-2.9.0/src/pyxplora_api/graphql_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,80 +1,80 @@
 """Module containing graphQL client."""
 from __future__ import annotations
 
 import logging
-from typing import Any, Dict
 
 import aiohttp
 import requests
 
 from .const import DEFAULT_TIMEOUT, DEFAULT_USER_AGENT
 
 
 class GraphqlClient:
     """Class which represents the interface to make graphQL requests through."""
 
-    def __init__(self, endpoint: str, headers: Dict[str, str] = {}, **kwargs: Any):
+    def __init__(self, endpoint: str, headers: dict[str, str] = {}, **kwargs: any):
         """Insantiate the client."""
         self.logger = logging.getLogger(__name__)
         self.endpoint = endpoint
         self.headers = headers
         self.options = kwargs
 
-    def __request_body(self, query: str, variables: Dict[str, Any] = None, operation_name: str = None) -> Dict[str, Any]:
-        json: Dict[str, Any] = {"query": query}
+    def __request_body(self, query: str, variables: dict[str, any] = None, operation_name: str = None) -> dict[str, any]:
+        json: dict[str, any] = {"query": query}
 
         if variables:
             json.update({"variables": variables})
 
         if operation_name:
             json.update({"operationName": operation_name})
 
         return json
 
-    def execute(self, query: str, variables: Dict[str, Any] = None, operation_name: str = None, headers: Dict[str, str] = {}):
+    def execute(self, query: str, variables: dict[str, any] = None, operation_name: str = None, headers: dict[str, str] = {}):
         """Make synchronous request to graphQL server."""
         request_body = self.__request_body(query=query, variables=variables, operation_name=operation_name)
 
         if "user-agent" not in headers:
             headers["user-agent"] = DEFAULT_USER_AGENT
         result = requests.post(
             self.endpoint,
             json=request_body,
             headers={**self.headers, **headers},
             **self.options,
-            timeout=aiohttp.ClientTimeout(DEFAULT_TIMEOUT),
+            timeout=DEFAULT_TIMEOUT,
         )
 
         result.raise_for_status()
         return result.json()
 
     async def execute_async(
-        self, query: str, variables: Dict[str, Any] = None, operation_name: str = None, headers: Dict[str, str] = {}
+        self, query: str, variables: dict[str, any] = None, operation_name: str = None, headers: dict[str, str] = {}
     ):
         """Make asynchronous request to graphQL server."""
         request_body = self.__request_body(query=query, variables=variables, operation_name=operation_name)
 
         if "user-agent" not in headers:
             headers["user-agent"] = DEFAULT_USER_AGENT
-        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(DEFAULT_TIMEOUT)) as session:
-            async with session.post(self.endpoint, json=request_body, headers={**self.headers, **headers}) as response:
-                try:
-                    response.raise_for_status()
-                    return await response.json()
-                except (aiohttp.ContentTypeError, aiohttp.ClientResponseError) as err:
-                    self.logger.debug(err)
-                    return {}
+        async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(DEFAULT_TIMEOUT)) as session, session.post(
+            self.endpoint, json=request_body, headers={**self.headers, **headers}
+        ) as response:
+            try:
+                response.raise_for_status()
+                return await response.json()
+            except (aiohttp.ContentTypeError, aiohttp.ClientResponseError) as err:
+                self.logger.debug(err)
+                return {}
 
     async def ha_execute_async(
         self,
         query: str,
-        variables: Dict[str, Any] = None,
+        variables: dict[str, any] = None,
         operation_name: str = None,
-        headers: Dict[str, str] = {},
+        headers: dict[str, str] = {},
         session: aiohttp.ClientSession = None,
     ):
         """Make asynchronous request to graphQL server."""
         request_body = self.__request_body(query=query, variables=variables, operation_name=operation_name)
 
         if "user-agent" not in headers:
             headers["user-agent"] = DEFAULT_USER_AGENT
```

### Comparing `pyxplora_api-2.8.3/src/pyxplora_api/handler_gql.py` & `pyxplora_api-2.9.0/src/pyxplora_api/handler_gql.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 from __future__ import annotations
 
+import sys
+
+if sys.version_info >= (3, 11):
+    from datetime import UTC, datetime
+else:
+    from datetime import datetime, timezone
 import hashlib
 import math
-from datetime import datetime, timezone
 from time import time
-from typing import Any, Dict
 
 from .const import API_KEY, API_SECRET
 from .status import ClientType
 
 
 class HandlerGQL:
-    """
-    A class to handle GraphQL API requests for PyXplora.
+    """A class to handle GraphQL API requests for PyXplora.
 
     Attributes:
-        accessToken (Any): The access token used for authentication.
+        accessToken (any): The access token used for authentication.
         sessionId (None): The session ID.
         userId (None): The user ID.
         _API_KEY (str): The API key.
         _API_SECRET (str): The API secret.
-        issueToken (dict[str, Any]): The issue token.
-        errors (list[Any]): A list of errors.
+        issueToken (dict[str, any]): The issue token.
+        errors (list[any]): A list of errors.
 
     """
 
-    accessToken: Any = None
-    sessionId = None
-    userId = None
-    issueToken: dict[str, Any] = None
-    errors: list[Any] = []
+    accessToken: any = None  # noqa: N815
+    sessionId = None  # noqa: N815
+    userId = None  # noqa: N815
+    issueToken: dict[str, any] = None  # noqa: N815
+    errors: list[any] = []
 
     def __init__(
         self,
         countryPhoneNumber: str,
         phoneNumber: str,
         password: str,
         userLang: str,
         timeZone: str,
         email: str = None,
         signup: bool = True,
     ) -> None:
-        """
-        Initializes the class with the given parameters.
+        """Initializes the class with the given parameters.
 
         Args:
             countryPhoneNumber (str): The country phone number.
             phoneNumber (str): The phone number.
             password (str): The password.
             userLang (str): The user language.
             timeZone (str): The time zone.
@@ -71,42 +73,39 @@
             "timeZone": self.timeZone,
             "emailAddress": self.email,
             "client": ClientType.APP.value,
         }
         self.signup = signup
 
     def getApiKey(self):
-        """
-        Returns the API key.
+        """Returns the API key.
 
         Returns:
             str: The API key.
 
         """
         return self._API_KEY
 
     def getSecret(self):
-        """
-        Returns the API secret.
+        """Returns the API secret.
 
         Returns:
             str: The API secret.
 
         """
         return self._API_SECRET
 
-    def getRequestHeaders(self, acceptedContentType: str) -> Dict[str, Any]:
-        """
-        Returns the request headers with the specified content type.
+    def getRequestHeaders(self, acceptedContentType: str) -> dict[str, any]:
+        """Returns the request headers with the specified content type.
 
         Args:
             acceptedContentType (str): The accepted content type.
 
         Returns:
-            dict[str, Any]: The request headers.
+            dict[str, any]: The request headers.
 
         Raises:
             Exception: If `acceptedContentType` is empty or if `API_KEY` or `API_SECRET` is not set.
 
         """
         if acceptedContentType == "" or acceptedContentType is None:
             raise Exception("acceptedContentType MUST NOT be empty!")
@@ -116,30 +115,33 @@
             raise Exception("Xplorao2o API_SECRET MUST NOT be empty!")
 
         authorizationHeader = ""
 
         if (self.accessToken is None or not self.issueToken) and self._API_KEY == API_KEY:
             # OPEN authorization
             authorizationHeader = f"Open {self._API_KEY}:{self._API_SECRET}"
-        else:
-            # BEARER authorization
-            if self.issueToken:
-                w360: dict = self.issueToken.get("w360", None)
-                if w360:
-                    if w360.get("token") and w360.get("secret"):
-                        authorizationHeader = (
-                            f'Bearer {w360.get("token", self.accessToken)}:{w360.get("secret", self._API_SECRET)}'
-                        )
-                        self._API_KEY = w360.get("token", API_KEY)
-                        self._API_SECRET = w360.get("secret", API_SECRET)
-                else:
-                    authorizationHeader = f"Bearer {self.accessToken}:{self._API_SECRET}"
+        # else:
+        # BEARER authorization
+        elif self.issueToken:
+            w360: dict = self.issueToken.get("w360", None)
+            if w360:
+                if w360.get("token") and w360.get("secret"):
+                    authorizationHeader = (
+                        f'Bearer {w360.get("token", self.accessToken)}:{w360.get("secret", self._API_SECRET)}'
+                    )
+                    self._API_KEY = w360.get("token", API_KEY)
+                    self._API_SECRET = w360.get("secret", API_SECRET)
             else:
-                authorizationHeader = f"Bearer {self._API_KEY}:{self._API_SECRET}"
-
+                authorizationHeader = f"Bearer {self.accessToken}:{self._API_SECRET}"
+        else:
+            authorizationHeader = f"Bearer {self._API_KEY}:{self._API_SECRET}"
+        if sys.version_info >= (3, 11):
+            utc = UTC
+        else:
+            utc = timezone.utc
         requestHeaders = {
-            "H-Date": datetime.now(timezone.utc).strftime("%a, %d %b %Y %H:%M:%S") + " GMT",
+            "H-Date": datetime.now(utc).strftime("%a, %d %b %Y %H:%M:%S") + " GMT",
             "H-Tid": str(math.floor(time())),
             "Content-Type": acceptedContentType,
             "H-BackDoor-Authorization": authorizationHeader,
         }
         return requestHeaders
```

### Comparing `pyxplora_api-2.8.3/src/pyxplora_api/pyxplora.py` & `pyxplora_api-2.9.0/src/pyxplora_api/pyxplora.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,48 @@
 from __future__ import annotations
 
 from datetime import datetime, timedelta
 from time import time
-from typing import Any, List, Optional, Union
 
 from .exception_classes import ChildNoError, XTypeError
 
 
 class PyXplora:
-    """
-    This class represents the PyXplora client. It has class level attributes and methods to interact with the Xplora API.
+    """This class represents the PyXplora client. It has class level attributes and methods to interact with the Xplora API.
 
     Attributes:
-    _gql_handler (Any): The GQL handler to interact with the Xplora API.
+    _gql_handler (any): The GQL handler to interact with the Xplora API.
     error_message (str): A string representing the error message, if any.
     tokenExpiresAfter (int): An integer representing the time in seconds after which the token will expire.
     maxRetries (int): The maximum number of retries in case of API failure.
     retryDelay (int): The time in seconds to wait between retries.
-    device (dict[str, Any]): A dictionary representing the device details, if any.
-    watchs (list[Any]): A list of dictionaries representing the watch details, if any.
+    device (dict[str, any]): A dictionary representing the device details, if any.
+    watchs (list[any]): A list of dictionaries representing the watch details, if any.
     """
 
-    _gql_handler: Any = None
+    _gql_handler: any = None
     error_message = ""
-    tokenExpiresAfter = 240
-    maxRetries = 3
-    retryDelay = 2
-    device: dict[str, Any] = {}
-    watchs: list[Any] = []
+    tokenExpiresAfter = 240  # noqa: N815
+    maxRetries = 3  # noqa: N815
+    retryDelay = 2  # noqa: N815
+    device: dict[str, any] = {}
+    watchs: list[any] = []
 
     def __init__(
         self,
         countrycode: str,
         phoneNumber: str,
         password: str,
         userLang: str,
         timeZone: str,
         childPhoneNumber: list[str] = None,
         wuid: str | list | None = None,
         email: str | None = None,
     ) -> None:
-        """
-        Initialize the instance with the user's account information.
+        """Initialize the instance with the user's account information.
 
         Args:
             countrycode (str): The country code of the user's phone number.
             phoneNumber (str): The phone number of the user.
             password (str): The password of the user's account.
             userLang (str): The language setting of the user.
             timeZone (str): The time zone of the user.
@@ -68,155 +65,142 @@
         self._wuid = wuid
 
         self.dtIssueToken = int(time()) - (self.tokenExpiresAfter * 1000)
 
         self._logoff()
 
     def _isConnected(self) -> bool:
-        """
-        Check if the instance is connected to the server.
+        """Check if the instance is connected to the server.
 
         Returns:
             bool: True if the instance is connected, False otherwise.
         """
         return bool(self._gql_handler and self._issueToken and self._gql_handler.accessToken)
 
     def _logoff(self) -> None:
-        """
-        Log off the user by clearing the stored information.
+        """Log off the user by clearing the stored information.
 
         Returns:
             None
         """
-        self.user: dict[Any, Any] = {}
-        self._issueToken: dict[Any, Any] = {}
+        self.user: dict[any, any] = {}
+        self._issueToken: dict[any, any] = {}
 
     def _hasTokenExpired(self) -> bool:
-        """
-        Check if the token has expired.
+        """Check if the token has expired.
 
         Returns:
             bool: True if the token has expired, False otherwise.
         """
         return (int(time()) - self.dtIssueToken) > (self.tokenExpiresAfter * 1000)
 
     def delay(self, duration_in_seconds):
-        """
-        Delay the execution for a specified duration.
+        """Delay the execution for a specified duration.
 
         Args:
             duration_in_seconds (int): The duration to delay in seconds.
 
         Returns:
             None
         """
         end_time = datetime.now() + timedelta(seconds=duration_in_seconds)
         while datetime.now() < end_time:
             pass
 
     def getDevice(self, wuid: str):
-        """
-        Get the information for a specific watch.
+        """Get the information for a specific watch.
 
         Args:
             wuid (str): The ID of the watch.
 
         Returns:
             dict: A dictionary containing the information of the watch.
         """
         try:
             return self.device[wuid]
         except KeyError:
             return {}
 
     ##### User Info #####
     def getUserID(self) -> str:
-        """
-        This function returns the id of the user.
+        """This function returns the id of the user.
 
         Returns:
         str: The id of the user.
         """
         return self.user.get("id", "")
 
     def getUserName(self) -> str:
-        """
-        This function returns the name of the user.
+        """This function returns the name of the user.
 
         Returns:
         str: The name of the user.
         """
         return self.user.get("name", "")
 
     def getUserIcon(self) -> str:
-        """
-        This function returns the profile icon of the user.
+        """This function returns the profile icon of the user.
 
         Returns:
         str: The profile icon of the user.
         """
         extra = self.user.get("extra", {})
         return extra.get("profileIcon", "https://s3.eu-central-1.amazonaws.com/kids360uc/default_icon.png")
 
     def getUserXcoin(self) -> int:
-        """
-        This function returns the xcoin amount of the user.
+        """This function returns the xcoin amount of the user.
 
         Returns:
         int: The xcoin amount of the user.
         """
         return self.user.get("xcoin", -1)
 
     def getUserCurrentStep(self) -> int:
-        """
-        This function returns the current step count of the user.
+        """This function returns the current step count of the user.
 
         Returns:
         int: The current step count of the user.
         """
         return self.user.get("currentStep", -1)
 
     def getUserTotalStep(self) -> int:
-        """
-        This function returns the total step count of the user.
+        """This function returns the total step count of the user.
 
         Returns:
         int: The total step count of the user.
         """
         return self.user.get("totalStep", -1)
 
     def getUserCreate(self) -> str:
-        """
-        This function returns the creation date and time of the user.
+        """This function returns the creation date and time of the user.
 
         Returns:
         str: The creation date and time of the user in the format "YYYY-MM-DD HH:MM:SS".
         """
         return datetime.fromtimestamp(self.user.get("create", 0.0)).strftime("%Y-%m-%d %H:%M:%S")
 
     def getUserUpdate(self) -> str:
-        """
-        This function returns the user update time in a string format.
+        """This function returns the user update time in a string format.
 
         Returns:
         str: The user update time in the format 'YYYY-MM-DD HH:MM:SS'.
 
         """
         return datetime.fromtimestamp(self.user.get("update", 0.0)).strftime("%Y-%m-%d %H:%M:%S")
 
     ##### Watch Info #####
-    def getWatchUserIDs(self, watch_user_phone_numbers: Optional[List[str]] = None) -> List[str]:
-        """
-        This function returns the unique identifiers of the watch users.
+    def getWatchUserIDs(self, watch_user_phone_numbers: list[str] | None = None) -> list[str]:
+        """This function returns the unique identifiers of the watch users.
 
         Parameters:
-        watch_user_phone_numbers (List[str], optional): A list of watch user phone numbers to filter the watch users. If not provided, all watch user ids will be returned.
+        watch_user_phone_numbers (list[str], optional): A list of watch user phone numbers to filter the watch users.
+        If not provided, all watch user ids will be returned.
 
         Returns:
-        List[str]: A list of unique identifiers of the watch users.
+        list[str]: A list of unique identifiers of the watch users.
 
         """
         if isinstance(self._wuid, list) and self._wuid:
             return self._wuid
         if isinstance(self._wuid, str) and self._wuid:
             return [self._wuid]
         watch_ids = []
@@ -224,26 +208,25 @@
             if watch_user_phone_numbers:
                 if watch["ward"]["phoneNumber"] in watch_user_phone_numbers:
                     watch_ids.append(watch["ward"]["id"])
             else:
                 watch_ids.append(watch["ward"]["id"])
         return watch_ids
 
-    def getWatchUserPhoneNumbers(
-        self, wuid: Optional[Union[str, List[str]]] = None, ignoreError: bool = False
-    ) -> Union[str, List[str]]:
-        """
-        This function returns the phone number of the watch users.
+    def getWatchUserPhoneNumbers(self, wuid: str | list[str] | None = None, ignoreError: bool = False) -> str | list[str]:
+        """This function returns the phone number of the watch users.
 
         Parameters:
-        wuid (Union[str, List[str]], optional): The unique identifier of the watch user. If not provided, the function will retrieve all watch user ids using `self.getWatchUserIDs()`.
-        ignoreError (bool, optional): If True, the function will not raise error in case of missing information. Default value is False.
+        wuid (Union[str, list[str]], optional): The unique identifier of the watch user.
+        If not provided, the function will retrieve all watch user ids using `self.getWatchUserIDs()`.
+        ignoreError (bool, optional): If True, the function will not raise error in case of missing information.
+        Default value is False.
 
         Returns:
-        Union[str, List[str]]: The phone number(s) of the watch user(s).
+        Union[str, list[str]]: The phone number(s) of the watch user(s).
 
         Raises:
         ChildNoError: If no `wuid` provided or watch user ids are not found.
         XTypeError: If the `wuid` is not of type `str` or `list[str]`.
 
         """
         watchuserphonenumbers = []
@@ -263,24 +246,25 @@
                     return phone_number
             else:
                 raise XTypeError("str | list[str]", type(wuid))
         if not watchuserphonenumbers and not ignoreError:
             raise ChildNoError(["Child phonenumber"])
         return watchuserphonenumbers
 
-    def getWatchUserNames(self, wuid: Optional[Union[str, List[str]]] = None) -> Union[str, List[str]]:
-        """
-        This function returns the name of one or multiple users specified by their user ID. If no user ID is specified,
+    def getWatchUserNames(self, wuid: str | list[str] | None = None) -> str | list[str]:
+        """This function returns the name of one or multiple users specified by their user ID. If no user ID is specified,
         the names of all watched users are returned.
 
         Parameters:
-        wuid (str, list[str], optional): A string or a list of strings representing the user IDs of the watched users. Defaults to None.
+        wuid (str, list[str], optional): A string or a list of strings representing the user IDs of the watched users.
+        Defaults to None.
 
         Returns:
-        Union[str, List[str]]: A string representing the name of a single user or a list of strings representing the names of multiple users.
+        Union[str, list[str]]:
+            A string representing the name of a single user or a list of strings representing the names of multiple users.
 
         Raises:
         ChildNoError: If the user IDs are not found.
         XTypeError: If the `wuid` parameter is not a string or a list of strings.
 
         """
         watchusernames = []
@@ -297,17 +281,16 @@
                     return watch["ward"]["name"]
             else:
                 raise XTypeError("str | list[str]", type(wuid))
         # if not watchusernames:
         #     raise ChildNoError(["Watch username"])
         return watchusernames
 
-    def getWatchUserIcons(self, wuid: Optional[Union[str, List[str], None]] = None) -> Union[str, List[str]]:
-        """
-        Get the icon URL for watch users.
+    def getWatchUserIcons(self, wuid: str | list[str] | None | None = None) -> str | list[str]:
+        """Get the icon URL for watch users.
 
         Parameters:
         wuid (str or list[str] or None, optional): Watch User ID. Defaults to None.
         If None, all watch user IDs will be retrieved using `getWatchUserIDs()`.
 
         Returns:
         str or list[str]: The URL of the icon for the specified watch user(s).
@@ -331,20 +314,20 @@
                     return f"https://api.myxplora.com/file?id={watch['ward']['file']['id']}"
             else:
                 raise XTypeError("str | list[str]", type(wuid))
         # if not watch_user_icons:
         #     raise ChildNoError(["Watch User Icon"])
         return watch_user_icons
 
-    def getWatchUserXCoins(self, wuid: Optional[Union[str, List[str]]] = None) -> Union[int, List[int]]:
-        """
-        Get the XCoins earned by the watch user.
+    def getWatchUserXCoins(self, wuid: str | list[str] | None = None) -> int | list[int]:
+        """Get the XCoins earned by the watch user.
 
         Args:
-        wuid (str or list of str or None, optional): Watch User ID or a list of Watch User IDs. If None, returns XCoins for all Watch Users.
+        wuid (str or list of str or None, optional): Watch User ID or a list of Watch User IDs.
+        If None, returns XCoins for all Watch Users.
 
         Returns:
         int or list of int: XCoins earned by the specified Watch User or a list of XCoins earned by specified Watch Users.
 
         Raises:
         ChildNoError: If the specified Watch User ID(s) is not found.
         XTypeError: If the specified `wuid` is not of type str or list of str.
@@ -363,17 +346,16 @@
                     return int(watch["ward"]["xcoin"])
             else:
                 raise XTypeError("str | list[str]", type(wuid))
         # if not watchuserxcoins:
         #     raise ChildNoError(["Watch User XCoins"])
         return watchuserxcoins
 
-    def getWatchUserCurrentStep(self, wuid: Union[str, List[str], None] = None) -> Union[int, List[int]]:
-        """
-        Get the current step count of a watch user.
+    def getWatchUserCurrentStep(self, wuid: str | list[str] | None = None) -> int | list[int]:
+        """Get the current step count of a watch user.
 
         Args:
         wuid (str | list[str] | None): ID(s) of watch user(s). If None, all IDs are used. (default None)
 
         Returns:
         int | list[int]: current step count of the watch user(s).
 
@@ -395,20 +377,20 @@
                     return int(watch["ward"]["currentStep"])
             else:
                 raise XTypeError("str | list[str]", type(wuid))
         # if not watchusercurrentstep:
         #     raise ChildNoError(["Watch User Currentsteps"])
         return watchusercurrentstep
 
-    def getWatchUserTotalStep(self, wuid: Optional[Union[str, List[str], None]] = None) -> Union[int, List[int]]:
-        """
-        Get the total steps taken by a user or a list of users from the watch.
+    def getWatchUserTotalStep(self, wuid: str | list[str] | None | None = None) -> int | list[int]:
+        """Get the total steps taken by a user or a list of users from the watch.
 
         Args:
-        wuid (str | list[str] | None, optional): the watch user id or a list of watch user ids. If None, get total steps for all users. Default is None.
+        wuid (str | list[str] | None, optional): the watch user id or a list of watch user ids.
+        If None, get total steps for all users. Default is None.
 
         Returns:
         int | list[int]: the total steps taken by the user(s) or a list of total steps taken by each user in the list.
 
         Raises:
         ChildNoError: if wuid is an empty list.
         XTypeError: if wuid is not a string or a list of strings.
@@ -429,16 +411,15 @@
                 raise XTypeError("str | list[str]", type(wuid))
         # if not watchusertotalstep:
         #     raise ChildNoError(["Watch User totalsteps"])
         return watchusertotalstep
 
     ##### - #####
     def _helperTime(self, t: str) -> str:
-        """
-        Convert time in minutes to hours and minutes.
+        """Convert time in minutes to hours and minutes.
 
         Args:
         t (str): time in minutes as string
 
         Returns:
         str: time in hours and minutes format (hh:mm)
         """
```

### Comparing `pyxplora_api-2.8.3/src/pyxplora_api/pyxplora_api.py` & `pyxplora_api-2.9.0/src/pyxplora_api/pyxplora_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from __future__ import annotations
 
-import logging
 from datetime import datetime
+import logging
 from time import time
-from typing import Any, Dict, List, Optional, Union
 
 from .const_version import VERSION, VERSION_APP
 from .exception_classes import Error, ErrorMSG, LoginError, NoAdminError
 from .gql_handler import GQLHandler
 from .model import Chats, ChatsNew, SmallChat, SmallChatList
 from .pyxplora import PyXplora
-from .status import Emoji, LocationType, NormalStatus, UserContactType, WatchOnlineStatus
+from .status import (
+    Emoji,
+    LocationType,
+    NormalStatus,
+    UserContactType,
+    WatchOnlineStatus,
+)
 
 _LOGGER = logging.getLogger(__name__)
 
 LIST_DICT: list[dict[str, any]] = []
 
 
 class PyXploraApi(PyXplora):
@@ -32,15 +37,15 @@
         super().__init__(countrycode, phoneNumber, password, userLang, timeZone, childPhoneNumber, wuid, email)
 
     def initHandler(self, sign_up):
         self._gql_handler: GQLHandler = GQLHandler(
             self._countrycode, self._phoneNumber, self._password, self._userLang, self._timeZone, self._email, sign_up
         )
 
-    def _login(self, force_login: bool = False, sign_up: bool = True) -> Dict[str, Any]:
+    def _login(self, force_login: bool = False, sign_up: bool = True) -> dict[str, any]:
         if not self._isConnected() or self._hasTokenExpired() or force_login:
             retryCounter = 0
             while not self._isConnected() and (retryCounter < self.maxRetries + 2):
                 retryCounter += 1
 
                 # Try to login
                 try:
@@ -77,24 +82,24 @@
             self.watchs = [watch for watch in children if watch["ward"]["phoneNumber"] in self._childPhoneNumber]
 
         self.user = user
 
     def version(self) -> str:
         return f"{VERSION}-{VERSION_APP}"
 
-    def setDevices(self, ids: Optional[Union[str, List[str]]] = None) -> List[str]:
+    def setDevices(self, ids: str | list[str] | None = None) -> list[str]:
         if isinstance(ids, str):
             ids = [ids]
         return self._setDevices(ids or [])
 
-    def _setDevices(self, ids: List[str] = None) -> List[str]:
+    def _setDevices(self, ids: list[str] = None) -> list[str]:
         wuids = ids if ids else self.getWatchUserIDs()
         return wuids
 
-    def _setDevice(self, ids: list = None) -> List[str]:
+    def _setDevice(self, ids: list = None) -> list[str]:
         wuids = ids or self.getWatchUserIDs()
         for wuid in wuids:
             self.device[wuid] = {}
             self.device[wuid]["getWatchAlarm"] = self.getWatchAlarm(wuid=wuid)
             self.device[wuid]["loadWatchLocation"] = self.loadWatchLocation(wuid=wuid)
             loc = self.device[wuid]["loadWatchLocation"]
             self.device[wuid]["watch_battery"] = int(loc.get("watch_battery", -1))
@@ -113,15 +118,15 @@
             self.device[wuid]["getWatchUserSteps"] = self.getWatchUserSteps(wuid=wuid, date=int(dt.timestamp()))
             self.device[wuid]["getWatchOnlineStatus"] = self.getWatchOnlineStatus(wuid=wuid)
             self.device[wuid]["getWatchUserIcons"] = self.getWatchUserIcons(wuid=wuid)
             self.device[wuid]["getWatchUserXCoins"] = self.getWatchUserXCoins(wuid=wuid)
         return wuids
 
     ##### Contact Info #####
-    def getWatchUserContacts(self, wuid: str) -> List[dict[str, Any]]:
+    def getWatchUserContacts(self, wuid: str) -> list[dict[str, any]]:
         retries = 0
         contacts = []
         while retries < self.maxRetries + 2:
             try:
                 raw_contacts = self._gql_handler.getWatchUserContacts(wuid)
                 raw_contacts = raw_contacts.get("contacts", {})
                 if not raw_contacts:
@@ -145,17 +150,17 @@
                         )
                 break
             except (Error, TypeError) as error:
                 _LOGGER.debug(error)
                 self.delay(self.retryDelay)
         return contacts
 
-    def getWatchAlarm(self, wuid: str) -> List[Dict[str, Any]]:
+    def getWatchAlarm(self, wuid: str) -> list[dict[str, any]]:
         retry_counter = 0
-        alarms: List[Dict[str, Any]] = []
+        alarms: list[dict[str, any]] = []
 
         while retry_counter < self.maxRetries + 2:
             try:
                 alarms_raw = self._gql_handler.getAlarmTime(wuid)
                 raw_alarms = alarms_raw.get("alarms", [])
                 if not raw_alarms:
                     return []
@@ -173,15 +178,15 @@
                 break
             except Error as error:
                 retry_counter += 1
                 _LOGGER.debug(error)
                 self.delay(self.retryDelay)
         return alarms
 
-    def loadWatchLocation(self, wuid: str = "", with_ask: bool = True) -> Dict[str, Any]:
+    def loadWatchLocation(self, wuid: str = "", with_ask: bool = True) -> dict[str, any]:
         retry_counter = 0
         watch_location = {}
         while retry_counter < self.maxRetries + 1:
             try:
                 if with_ask:
                     self.askWatchLocate(wuid)
                 location_raw = self._gql_handler.getWatchLastLocation(wuid)
@@ -234,15 +239,15 @@
         return watch_location
 
     def getWatchBattery(self, wuid: str) -> int:
         watch_b = self.loadWatchLocation(wuid=wuid)
         return int(watch_b.get("watch_battery", -1))
 
     def getWatchIsCharging(self, wuid: str) -> bool:
-        watch_c: dict[str, Any] = self.loadWatchLocation(wuid=wuid)
+        watch_c: dict[str, any] = self.loadWatchLocation(wuid=wuid)
         return watch_c.get("watch_charging", False)
 
     def getWatchOnlineStatus(self, wuid: str) -> str:
         retries = 0
         status = WatchOnlineStatus.UNKNOWN
 
         while status is WatchOnlineStatus.UNKNOWN and retries < self.maxRetries + 2:
@@ -266,17 +271,17 @@
             return -1
         except Error as e:
             _LOGGER.error("Error getting unread chat message count: %s", e)
             return -1
 
     def getWatchChats(
         self, wuid: str, offset: int = 0, limit: int = 0, msgId: str = "", show_del_msg: bool = True, asObject=False
-    ) -> Union[List[Dict[str, Any]], SmallChatList]:
+    ) -> list[dict[str, any]] | SmallChatList:
         retry_counter = 0
-        chats: List[Dict[str, Any]] = []
+        chats: list[dict[str, any]] = []
 
         while not chats and retry_counter < self.maxRetries + 2:
             retry_counter += 1
             try:
                 _chats_new = self.getWatchChatsRaw(wuid, offset, limit, msgId, show_del_msg, asObject)
                 if isinstance(_chats_new, dict):
                     _chats_new = ChatsNew.from_dict(_chats_new)
@@ -318,15 +323,15 @@
         wuid: str,
         offset: int = 0,
         limit: int = 0,
         msgId: str = "",
         show_del_msg: bool = True,
         asObject=False,
         with_emoji_id=True,
-    ) -> Union[dict, ChatsNew]:
+    ) -> dict | ChatsNew:
         retry_counter = 0
         chats_new: dict = {}
         while not chats_new and retry_counter < self.maxRetries + 2:
             retry_counter += 1
             try:
                 result = self._gql_handler.chats(wuid, offset, limit, msgId, asObject)
                 if not result:
@@ -353,32 +358,32 @@
 
             if not chats_new:
                 self.delay(self.retryDelay)
 
         return ChatsNew.from_dict(chats_new, infer_missing=True) if asObject else chats_new
 
     ##### Watch Location Info #####
-    def getWatchLastLocation(self, wuid: str, withAsk: bool = False) -> Dict[str, Any]:
+    def getWatchLastLocation(self, wuid: str, withAsk: bool = False) -> dict[str, any]:
         loc = self.loadWatchLocation(wuid, withAsk)
         return loc.get("watch_last_location", {}) if isinstance(loc, dict) else {}
 
-    def getWatchLocate(self, wuid: str) -> Dict[str, Any]:
+    def getWatchLocate(self, wuid: str) -> dict[str, any]:
         return self.loadWatchLocation(wuid=wuid) or {}
 
     def getWatchLocateType(self, wuid: str) -> str:
         locate_info = self.getWatchLocate(wuid)
         return locate_info.get("locateType", LocationType.UNKNOWN.value)
 
     def getWatchIsInSafeZone(self, wuid: str) -> bool:
         return self.getWatchLocate(wuid).get("isInSafeZone", False)
 
     def getWatchSafeZoneLabel(self, wuid: str) -> str:
         return self.getWatchLocate(wuid).get("safeZoneLabel", "")
 
-    def getWatchSafeZones(self, wuid: str) -> List[dict[str, Any]]:
+    def getWatchSafeZones(self, wuid: str) -> list[dict[str, any]]:
         retry_counter = 0
         safe_zones = []
         while retry_counter < self.maxRetries + 2:
             try:
                 safe_zones_raw = self._gql_handler.safeZones(wuid)
                 _safe_zones = safe_zones_raw.get("safeZones", [])
                 if not _safe_zones:
@@ -405,19 +410,19 @@
     def getTrackWatchInterval(self, wuid: str) -> int:
         return self._gql_handler.trackWatch(wuid).get("trackWatch", -1)
 
     def askWatchLocate(self, wuid: str) -> bool:
         return self._gql_handler.askWatchLocate(wuid).get("askWatchLocate", False)
 
     ##### Feature #####
-    def getSilentTime(self, wuid: str) -> List[Dict[str, Any]]:
+    def getSilentTime(self, wuid: str) -> list[dict[str, any]]:
         retry_counter = 0
-        data_ok: List[Dict[str, Any]] = []
-        silent_times_raw: Dict[str, Any] = {}
-        school_silent_mode: List[Dict[str, Any]] = []
+        data_ok: list[dict[str, any]] = []
+        silent_times_raw: dict[str, any] = {}
+        school_silent_mode: list[dict[str, any]] = []
         while not data_ok and (retry_counter < self.maxRetries + 2):
             retry_counter += 1
             try:
                 silent_times_raw = self._gql_handler.silentTimes(wuid)
                 _silent_times = silent_times_raw.get("silentTimes", [])
                 if not _silent_times:
                     data_ok.append({})
@@ -469,24 +474,24 @@
             except Error as error:
                 _LOGGER.debug(error)
             if not result:
                 self.delay(self.retryDelay)
 
         return bool(result)
 
-    def setAllEnableSilentTime(self, wuid: str) -> List[bool]:
+    def setAllEnableSilentTime(self, wuid: str) -> list[bool]:
         results = []
         silent_times = self.getSilentTime(wuid)
         for silent_time in silent_times:
             id = silent_time.get("id")
             if id:
                 results.append(self.setEnableSilentTime(id))
         return results
 
-    def setAllDisableSilentTime(self, wuid: str) -> List[bool]:
+    def setAllDisableSilentTime(self, wuid: str) -> list[bool]:
         results = []
         for silentTime in self.getSilentTime(wuid):
             results.append(self.setDisableSilentTime(silentTime.get("id", "")))
         return results
 
     def setAlarmTime(self, alarm_id: str, status: NormalStatus) -> bool:
         retryCounter = 0
@@ -507,21 +512,21 @@
 
     def setEnableAlarmTime(self, alarm_id: str) -> bool:
         return self.setAlarmTime(alarm_id, NormalStatus.ENABLE)
 
     def setDisableAlarmTime(self, alarm_id: str) -> bool:
         return self.setAlarmTime(alarm_id, NormalStatus.DISABLE)
 
-    def setAllEnableAlarmTime(self, wuid: str) -> List[bool]:
+    def setAllEnableAlarmTime(self, wuid: str) -> list[bool]:
         res: list[bool] = []
         for alarmTime in self.getWatchAlarm(wuid):
             res.append(self.setEnableAlarmTime(alarmTime.get("id", "")))
         return res
 
-    def setAllDisableAlarmTime(self, wuid: str) -> List[bool]:
+    def setAllDisableAlarmTime(self, wuid: str) -> list[bool]:
         res: list[bool] = []
         for alarmTime in self.getWatchAlarm(wuid):
             res.append(self.setDisableAlarmTime(alarmTime.get("id", "")))
         return res
 
     def sendText(self, text: str, wuid: str) -> bool:
         # sender is login User
@@ -539,26 +544,26 @@
 
     def reboot(self, wuid: str) -> bool:
         if self.isAdmin(wuid):
             return self._gql_handler.reboot(wuid)
         raise NoAdminError()
 
     def getFollowRequestWatchCount(self) -> int:
-        c: dict[str, Any] = self._gql_handler.getFollowRequestWatchCount()
+        c: dict[str, any] = self._gql_handler.getFollowRequestWatchCount()
         return c.get("followRequestWatchCount", 0)
 
-    def getWatches(self, wuid: str) -> Dict[str, Any]:
+    def getWatches(self, wuid: str) -> dict[str, any]:
         retryCounter = 0
-        watches_raw: dict[str, Any] = {}
-        watch: dict[str, Any] = {}
+        watches_raw: dict[str, any] = {}
+        watch: dict[str, any] = {}
         while not watch and (retryCounter < self.maxRetries + 2):
             retryCounter += 1
             try:
                 watches_raw = self._gql_handler.getWatches(wuid)
-                _watches: list[dict[str, Any]] = watches_raw.get("watches", [])
+                _watches: list[dict[str, any]] = watches_raw.get("watches", [])
                 if not _watches:
                     return watch
                 watch = {
                     "imei": _watches[0]["swKey"],
                     "osVersion": _watches[0]["osVersion"],
                     "qrCode": _watches[0]["qrCode"],
                     "model": _watches[0]["groupName"],
@@ -567,89 +572,89 @@
                     return watch
             except Error as error:
                 _LOGGER.debug(error)
             if not watch:
                 self.delay(self.retryDelay)
         return watch
 
-    def getSWInfo(self, wuid: str, watches: dict[str, Any] = {}) -> Dict[str, Any]:
-        wqr: dict[str, Any] = watches if watches else self.getWatches(wuid=wuid)
+    def getSWInfo(self, wuid: str, watches: dict[str, any] = {}) -> dict[str, any]:
+        wqr: dict[str, any] = watches if watches else self.getWatches(wuid=wuid)
         qrCode: str = wqr.get("qrCode", "=")
         return self._gql_handler.getSWInfo(qrCode.split("=")[1])
 
-    def getWatchState(self, wuid: str, watches: dict[str, Any] = {}) -> Dict[str, Any]:
-        wqr: dict[str, Any] = watches if watches else self.getWatches(wuid=wuid)
+    def getWatchState(self, wuid: str, watches: dict[str, any] = {}) -> dict[str, any]:
+        wqr: dict[str, any] = watches if watches else self.getWatches(wuid=wuid)
         qrCode: str = wqr.get("qrCode", "=")
         return self._gql_handler.getWatchState(qrCode=qrCode.split("=")[1])
 
-    def conv360IDToO2OID(self, qid: str, deviceId: str) -> Dict[str, Any]:
+    def conv360IDToO2OID(self, qid: str, deviceId: str) -> dict[str, any]:
         return self._gql_handler.conv360IDToO2OID(qid, deviceId)
 
-    def campaigns(self, id: str, categoryId: str) -> Dict[str, Any]:
+    def campaigns(self, id: str, categoryId: str) -> dict[str, any]:
         return self._gql_handler.campaigns(id, categoryId)
 
-    def getCountries(self) -> List[dict[str, str]]:
-        countries: dict[str, Any] = self._gql_handler.countries()
+    def getCountries(self) -> list[dict[str, str]]:
+        countries: dict[str, any] = self._gql_handler.countries()
         return countries.get("countries", {})
 
-    def getWatchLocHistory(self, wuid: str, date: int, tz: str, limit: int) -> Dict[str, Any]:
+    def getWatchLocHistory(self, wuid: str, date: int, tz: str, limit: int) -> dict[str, any]:
         return self._gql_handler.getWatchLocHistory(wuid, date, tz, limit)
 
-    def watchesDynamic(self) -> Dict[str, Any]:
+    def watchesDynamic(self) -> dict[str, any]:
         return self._gql_handler.watchesDynamic()
 
-    def watchGroups(self, id: str = "") -> Dict[str, Any]:
+    def watchGroups(self, id: str = "") -> dict[str, any]:
         return self._gql_handler.watchGroups(id)
 
-    def familyInfo(self, wuid: str, watchId: str, tz: str, date: int) -> Dict[str, Any]:
+    def familyInfo(self, wuid: str, watchId: str, tz: str, date: int) -> dict[str, any]:
         return self._gql_handler.familyInfo(wuid, watchId, tz, date)
 
-    def avatars(self, id: str) -> Dict[str, Any]:
+    def avatars(self, id: str) -> dict[str, any]:
         return self._gql_handler.avatars(id)
 
-    def getWatchUserSteps(self, wuid: str, date: int) -> Dict[str, Any]:
+    def getWatchUserSteps(self, wuid: str, date: int) -> dict[str, any]:
         userSteps = self._gql_handler.getWatchUserSteps(wuid=wuid, tz=self._timeZone, date=date)
         if not userSteps:
             return {}
         userSteps = userSteps.get("userSteps", {})
         if not userSteps:
             return {}
         return userSteps
 
     # start tracking for 30min
     def getStartTrackingWatch(self, wuid: str) -> int:
-        data: dict[str, Any] = self._gql_handler.getStartTrackingWatch(wuid)
+        data: dict[str, any] = self._gql_handler.getStartTrackingWatch(wuid)
         return data.get("startTrackingWatch", -1)
 
     # stop tracking from getStartTrackingWatch
     def getEndTrackingWatch(self, wuid: str) -> int:
-        data: dict[str, Any] = self._gql_handler.getEndTrackingWatch(wuid)
+        data: dict[str, any] = self._gql_handler.getEndTrackingWatch(wuid)
         return data.get("endTrackingWatch", -1)
 
     def addStep(self, step: int) -> bool:
         s: dict[str, bool] = self._gql_handler.addStep(step)
         return s.get("addStep", False)
 
     def submitIncorrectLocationData(self, wuid: str, lat: str, lng: str, timestamp: str) -> bool:
         data: dict[str, bool] = self._gql_handler.submitIncorrectLocationData(wuid, lat, lng, timestamp)
         return data.get("submitIncorrectLocationData", False)
 
-    def getAppVersion(self) -> Dict[str, Any]:
+    def getAppVersion(self) -> dict[str, any]:
         data = self._gql_handler.getAppVersion()
         return data
 
     def checkEmailOrPhoneExist(
         self, type: UserContactType, email: str = "", countryCode: str = "", phoneNumber: str = ""
     ) -> bool:
         data = self._gql_handler.checkEmailOrPhoneExist(type, email, countryCode, phoneNumber)
         return data.get("checkEmailOrPhoneExist", False)
 
     def modifyContact(
         self, contactId: str, isAdmin: bool | None = None, contactName: str = "", fileId: str = ""
-    ) -> Dict[str, Any]:
+    ) -> dict[str, any]:
         data = self._gql_handler.modifyContact(contactId, isAdmin, contactName, fileId)
         return data
 
     def deleteMessageFromApp(self, wuid: str, msgId: str) -> bool:
         data = self._gql_handler.deleteMessageFromApp(wuid, msgId)
         if data.get("deleteMsg", False):
             return True
```

### Comparing `pyxplora_api-2.8.3/src/pyxplora_api/pyxplora_api_async.py` & `pyxplora_api-2.9.0/src/pyxplora_api/pyxplora_api_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 from __future__ import annotations
 
 import asyncio
-import logging
 from datetime import datetime
+import logging
 from time import time
-from typing import Any, Dict, List, Optional, Union
 
 import aiohttp
 
 from .const_version import VERSION, VERSION_APP
 from .exception_classes import Error, ErrorMSG, LoginError, NoAdminError
 from .gql_handler_async import GQLHandler
 from .model import Chats, ChatsNew, SmallChat, SmallChatList
 from .pyxplora import PyXplora
-from .status import Emoji, LocationType, NormalStatus, UserContactType, WatchOnlineStatus
+from .status import (
+    Emoji,
+    LocationType,
+    NormalStatus,
+    UserContactType,
+    WatchOnlineStatus,
+)
 
 _LOGGER = logging.getLogger(__name__)
 
 LIST_DICT: list[dict[str, any]] = []
 
 
 class PyXploraApi(PyXplora):
@@ -35,15 +40,15 @@
         session: aiohttp.ClientSession = None,
     ) -> None:
         super().__init__(countrycode, phoneNumber, password, userLang, timeZone, childPhoneNumber, wuid, email)
         self._gql_handler: GQLHandler = GQLHandler(
             self._countrycode, self._phoneNumber, self._password, self._userLang, self._timeZone, self._email, sign_up, session
         )
 
-    async def _login(self, force_login: bool = False, key=None, sec=None) -> Dict[str, Any]:
+    async def _login(self, force_login: bool = False, key=None, sec=None) -> dict[str, any]:
         if not self._isConnected() or self._hasTokenExpired() or force_login:
             retryCounter = 0
             while not self._isConnected() and (retryCounter < self.maxRetries + 2):
                 retryCounter += 1
                 self._refresh_token = ""
 
                 # Try to login
@@ -87,20 +92,20 @@
         else:
             self.watchs = [watch for watch in children if watch["ward"]["phoneNumber"] in self._childPhoneNumber]
         self.user = user
 
     def version(self) -> str:
         return f"{VERSION}-{VERSION_APP}"
 
-    async def setDevices(self, ids: Optional[Union[str, List[str]]] = None) -> List[str]:
+    async def setDevices(self, ids: str | list[str] | None = None) -> list[str]:
         if isinstance(ids, str):
             ids = [ids]
         return await self._setDevices(ids or [])
 
-    async def _setDevices(self, ids: List[str] = None) -> List[str]:
+    async def _setDevices(self, ids: list[str] = None) -> list[str]:
         wuids = ids if ids else self.getWatchUserIDs()
         tasks = [self._setDevice(wuid) for wuid in wuids]
         await asyncio.gather(*tasks)
         return wuids
 
     async def _setDevice(self, wuid: str) -> None:
         tasks = [
@@ -156,15 +161,15 @@
             "getWatchUserSteps": user_steps,
             "getWatchOnlineStatus": online_status,
             "getWatchUserIcons": self.getWatchUserIcons(wuid),
             "getWatchUserXCoins": self.getWatchUserXCoins(wuid),
         }
 
     ##### Contact Info #####
-    async def getWatchUserContacts(self, wuid: str) -> List[dict[str, Any]]:
+    async def getWatchUserContacts(self, wuid: str) -> list[dict[str, any]]:
         retries = 0
         contacts = []
         while retries < self.maxRetries + 2:
             retries += 1
             try:
                 raw_contacts = await self._gql_handler.getWatchUserContacts_a(wuid)
                 raw_contacts = raw_contacts.get("contacts", {})
@@ -189,17 +194,17 @@
                         )
                 break
             except (Error, TypeError) as error:
                 _LOGGER.debug(error)
                 await asyncio.sleep(self.retryDelay)
         return contacts
 
-    async def getWatchAlarm(self, wuid: str) -> List[Dict[str, Any]]:
+    async def getWatchAlarm(self, wuid: str) -> list[dict[str, any]]:
         retry_counter = 0
-        alarms: List[Dict[str, Any]] = []
+        alarms: list[dict[str, any]] = []
 
         while retry_counter < self.maxRetries + 2:
             try:
                 alarms_raw = await self._gql_handler.getAlarmTime_a(wuid)
                 raw_alarms = alarms_raw.get("alarms", [])
                 if not raw_alarms:
                     return []
@@ -217,15 +222,15 @@
                 break
             except Error as error:
                 retry_counter += 1
                 _LOGGER.debug(error)
                 await asyncio.sleep(self.retryDelay)
         return alarms
 
-    async def loadWatchLocation(self, wuid: str = "", with_ask: bool = True) -> Dict[str, Any]:
+    async def loadWatchLocation(self, wuid: str = "", with_ask: bool = True) -> dict[str, any]:
         retry_counter = 0
         watch_location = {}
         while retry_counter < self.maxRetries + 1:
             try:
                 if with_ask:
                     await self.askWatchLocate(wuid)
                     await asyncio.sleep(1)
@@ -316,17 +321,17 @@
             return -1
         except Error as e:
             _LOGGER.error("Error getting unread chat message count: %s", e)
             return -1
 
     async def getWatchChats(
         self, wuid: str, offset: int = 0, limit: int = 0, msgId: str = "", show_del_msg: bool = True, asObject=False
-    ) -> Union[List[Dict[str, Any]], SmallChatList]:
+    ) -> list[dict[str, any]] | SmallChatList:
         retry_counter = 0
-        chats: List[Dict[str, Any]] = []
+        chats: list[dict[str, any]] = []
 
         while not chats and retry_counter < self.maxRetries + 2:
             retry_counter += 1
             try:
                 _chats_new = await self.getWatchChatsRaw(wuid, offset, limit, msgId, show_del_msg, asObject)
                 if isinstance(_chats_new, dict):
                     _chats_new = ChatsNew.from_dict(_chats_new)
@@ -368,15 +373,15 @@
         wuid: str,
         offset: int = 0,
         limit: int = 0,
         msgId: str = "",
         show_del_msg: bool = True,
         asObject=False,
         with_emoji_id=True,
-    ) -> Union[dict, ChatsNew]:
+    ) -> dict | ChatsNew:
         retry_counter = 0
         chats_new: dict = {}
         while not chats_new and retry_counter < self.maxRetries + 2:
             retry_counter += 1
             try:
                 result = await self._gql_handler.chats_a(wuid, offset, limit, msgId, asObject)
                 if not result:
@@ -404,22 +409,22 @@
 
             if not chats_new:
                 await asyncio.sleep(self.retryDelay)
 
         return ChatsNew.from_dict(chats_new, infer_missing=True) if asObject else chats_new
 
     ##### Watch Location Info #####
-    async def getWatchLastLocation(self, wuid: str, withAsk: bool = False) -> Dict[str, Any]:
+    async def getWatchLastLocation(self, wuid: str, withAsk: bool = False) -> dict[str, any]:
         tasks = [self.loadWatchLocation(wuid)]
         results = await asyncio.gather(*tasks)
         if results:
             return results[0].get("watch_last_location", {})
         return {}
 
-    async def getWatchLocate(self, wuid: str) -> Dict[str, Any]:
+    async def getWatchLocate(self, wuid: str) -> dict[str, any]:
         tasks = [self.loadWatchLocation(wuid)]
         results = await asyncio.gather(*tasks)
         if results:
             return results[0]
         return {}
 
     async def getWatchLocateType(self, wuid: str) -> str:
@@ -428,15 +433,15 @@
 
     async def getWatchIsInSafeZone(self, wuid: str) -> bool:
         return (await self.getWatchLocate(wuid)).get("isInSafeZone", False)
 
     async def getWatchSafeZoneLabel(self, wuid: str) -> str:
         return (await self.getWatchLocate(wuid)).get("safeZoneLabel", "")
 
-    async def getWatchSafeZones(self, wuid: str) -> List[dict[str, Any]]:
+    async def getWatchSafeZones(self, wuid: str) -> list[dict[str, any]]:
         retry_counter = 0
         safe_zones = []
         while retry_counter < self.maxRetries + 2:
             try:
                 safe_zones_raw = await self._gql_handler.safeZones_a(wuid)
                 _safe_zones = safe_zones_raw.get("safeZones", [])
                 if not _safe_zones:
@@ -463,19 +468,19 @@
     async def getTrackWatchInterval(self, wuid: str) -> int:
         return (await self._gql_handler.trackWatch_a(wuid)).get("trackWatch", -1)
 
     async def askWatchLocate(self, wuid: str) -> bool:
         return (await self._gql_handler.askWatchLocate_a(wuid)).get("askWatchLocate", False)
 
     ##### Feature #####
-    async def getSilentTime(self, wuid: str) -> List[Dict[str, Any]]:
+    async def getSilentTime(self, wuid: str) -> list[dict[str, any]]:
         retry_counter = 0
-        data_ok: List[Dict[str, Any]] = []
-        silent_times_raw: Dict[str, Any] = {}
-        school_silent_mode: List[Dict[str, Any]] = []
+        data_ok: list[dict[str, any]] = []
+        silent_times_raw: dict[str, any] = {}
+        school_silent_mode: list[dict[str, any]] = []
         while not data_ok and (retry_counter < self.maxRetries + 2):
             retry_counter += 1
             try:
                 silent_times_raw = await self._gql_handler.silentTimes_a(wuid)
                 _silent_times = silent_times_raw.get("silentTimes", [])
                 if not _silent_times:
                     data_ok.append({})
@@ -527,24 +532,24 @@
             except Error as error:
                 _LOGGER.debug(error)
             if not result:
                 await asyncio.sleep(self.retryDelay)
 
         return bool(result)
 
-    async def setAllEnableSilentTime(self, wuid: str) -> List[bool]:
+    async def setAllEnableSilentTime(self, wuid: str) -> list[bool]:
         results = []
         silent_times = await self.getSilentTime(wuid)
         for silent_time in silent_times:
             id = silent_time.get("id")
             if id:
                 results.append(await self.setEnableSilentTime(id))
         return results
 
-    async def setAllDisableSilentTime(self, wuid: str) -> List[bool]:
+    async def setAllDisableSilentTime(self, wuid: str) -> list[bool]:
         results = []
         for silentTime in await self.getSilentTime(wuid):
             results.append(await self.setDisableSilentTime(silentTime.get("id", "")))
         return results
 
     async def setAlarmTime(self, alarm_id: str, status: NormalStatus) -> bool:
         retryCounter = 0
@@ -565,21 +570,21 @@
 
     async def setEnableAlarmTime(self, alarm_id: str) -> bool:
         return await self.setAlarmTime(alarm_id, NormalStatus.ENABLE)
 
     async def setDisableAlarmTime(self, alarm_id: str) -> bool:
         return await self.setAlarmTime(alarm_id, NormalStatus.DISABLE)
 
-    async def setAllEnableAlarmTime(self, wuid: str) -> List[bool]:
+    async def setAllEnableAlarmTime(self, wuid: str) -> list[bool]:
         res: list[bool] = []
         for alarmTime in await self.getWatchAlarm(wuid):
             res.append(await self.setEnableAlarmTime(alarmTime.get("id", "")))
         return res
 
-    async def setAllDisableAlarmTime(self, wuid: str) -> List[bool]:
+    async def setAllDisableAlarmTime(self, wuid: str) -> list[bool]:
         res: list[bool] = []
         for alarmTime in await self.getWatchAlarm(wuid):
             res.append(await self.setDisableAlarmTime(alarmTime.get("id", "")))
         return res
 
     async def sendText(self, text: str, wuid: str) -> bool:
         # sender is login User
@@ -597,26 +602,26 @@
 
     async def reboot(self, wuid: str) -> bool:
         if await self.isAdmin(wuid):
             return await self._gql_handler.reboot_a(wuid)
         raise NoAdminError()
 
     async def getFollowRequestWatchCount(self) -> int:
-        c: dict[str, Any] = await self._gql_handler.getFollowRequestWatchCount_a()
+        c: dict[str, any] = await self._gql_handler.getFollowRequestWatchCount_a()
         return c.get("followRequestWatchCount", 0)
 
-    async def getWatches(self, wuid: str) -> Dict[str, Any]:
+    async def getWatches(self, wuid: str) -> dict[str, any]:
         retryCounter = 0
-        watches_raw: dict[str, Any] = {}
-        watch: dict[str, Any] = {}
+        watches_raw: dict[str, any] = {}
+        watch: dict[str, any] = {}
         while not watch and (retryCounter < self.maxRetries + 2):
             retryCounter += 1
             try:
                 watches_raw = await self._gql_handler.getWatches_a(wuid)
-                _watches: list[dict[str, Any]] = watches_raw.get("watches", [])
+                _watches: list[dict[str, any]] = watches_raw.get("watches", [])
                 if not _watches:
                     return watch
                 watch = {
                     "imei": _watches[0]["swKey"],
                     "osVersion": _watches[0]["osVersion"],
                     "qrCode": _watches[0]["qrCode"],
                     "model": _watches[0]["groupName"],
@@ -625,87 +630,87 @@
                     return watch
             except Error as error:
                 _LOGGER.debug(error)
             if not watch:
                 await asyncio.sleep(self.retryDelay)
         return watch
 
-    async def getSWInfo(self, wuid: str, watches: dict[str, Any] = {}) -> Dict[str, Any]:
-        wqr: dict[str, Any] = watches if watches else await self.getWatches(wuid=wuid)
+    async def getSWInfo(self, wuid: str, watches: dict[str, any] = {}) -> dict[str, any]:
+        wqr: dict[str, any] = watches if watches else await self.getWatches(wuid=wuid)
         qrCode: str = wqr.get("qrCode", "=")
         return await self._gql_handler.getSWInfo_a(qrCode.split("=")[1])
 
-    async def getWatchState(self, wuid: str, watches: dict[str, Any] = {}) -> Dict[str, Any]:
-        wqr: dict[str, Any] = watches if watches else await self.getWatches(wuid=wuid)
+    async def getWatchState(self, wuid: str, watches: dict[str, any] = {}) -> dict[str, any]:
+        wqr: dict[str, any] = watches if watches else await self.getWatches(wuid=wuid)
         qrCode: str = wqr.get("qrCode", "=")
         return await self._gql_handler.getWatchState_a(qrCode=qrCode.split("=")[1])
 
-    async def conv360IDToO2OID(self, qid: str, deviceId: str) -> Dict[str, Any]:
+    async def conv360IDToO2OID(self, qid: str, deviceId: str) -> dict[str, any]:
         return await self._gql_handler.conv360IDToO2OID_a(qid, deviceId)
 
-    async def campaigns(self, id: str, categoryId: str) -> Dict[str, Any]:
+    async def campaigns(self, id: str, categoryId: str) -> dict[str, any]:
         return await self._gql_handler.campaigns_a(id, categoryId)
 
-    async def getCountries(self) -> List[dict[str, str]]:
-        countries: dict[str, Any] = await self._gql_handler.countries_a()
+    async def getCountries(self) -> list[dict[str, str]]:
+        countries: dict[str, any] = await self._gql_handler.countries_a()
         return countries.get("countries", {})
 
-    async def getWatchLocHistory(self, wuid: str, date: int, tz: str, limit: int) -> Dict[str, Any]:
+    async def getWatchLocHistory(self, wuid: str, date: int, tz: str, limit: int) -> dict[str, any]:
         return await self._gql_handler.getWatchLocHistory_a(wuid, date, tz, limit)
 
-    async def watchesDynamic(self) -> Dict[str, Any]:
+    async def watchesDynamic(self) -> dict[str, any]:
         return await self._gql_handler.watchesDynamic_a()
 
-    async def watchGroups(self, id: str = "") -> Dict[str, Any]:
+    async def watchGroups(self, id: str = "") -> dict[str, any]:
         return await self._gql_handler.watchGroups_a(id)
 
-    async def familyInfo(self, wuid: str, watchId: str, tz: str, date: int) -> Dict[str, Any]:
+    async def familyInfo(self, wuid: str, watchId: str, tz: str, date: int) -> dict[str, any]:
         return await self._gql_handler.familyInfo_a(wuid, watchId, tz, date)
 
-    async def avatars(self, id: str) -> Dict[str, Any]:
+    async def avatars(self, id: str) -> dict[str, any]:
         return await self._gql_handler.avatars_a(id)
 
-    async def getWatchUserSteps(self, wuid: str, date: int) -> Dict[str, Any]:
+    async def getWatchUserSteps(self, wuid: str, date: int) -> dict[str, any]:
         userSteps = await self._gql_handler.getWatchUserSteps_a(wuid=wuid, tz=self._timeZone, date=date)
         if not userSteps:
             return {}
         userSteps = userSteps.get("userSteps", {})
         if not userSteps:
             return {}
         return userSteps
 
     # start tracking for 30min
     async def getStartTrackingWatch(self, wuid: str) -> int:
-        data: dict[str, Any] = await self._gql_handler.getStartTrackingWatch_a(wuid)
+        data: dict[str, any] = await self._gql_handler.getStartTrackingWatch_a(wuid)
         return data.get("startTrackingWatch", -1)
 
     # stop tracking from getStartTrackingWatch
     async def getEndTrackingWatch(self, wuid: str) -> int:
-        data: dict[str, Any] = await self._gql_handler.getEndTrackingWatch_a(wuid)
+        data: dict[str, any] = await self._gql_handler.getEndTrackingWatch_a(wuid)
         return data.get("endTrackingWatch", -1)
 
     async def addStep(self, step: int) -> bool:
         s: dict[str, bool] = await self._gql_handler.addStep_a(step)
         return s.get("addStep", False)
 
     async def submitIncorrectLocationData(self, wuid: str, lat: str, lng: str, timestamp: str) -> bool:
         data: dict[str, bool] = await self._gql_handler.submitIncorrectLocationData_a(wuid, lat, lng, timestamp)
         return data.get("submitIncorrectLocationData", False)
 
-    async def getAppVersion(self) -> Dict[str, Any]:
+    async def getAppVersion(self) -> dict[str, any]:
         data = await self._gql_handler.getAppVersion_a()
         return data
 
     async def checkEmailOrPhoneExist(
         self, type: UserContactType, email: str = "", countryCode: str = "", phoneNumber: str = ""
     ) -> bool:
         data = await self._gql_handler.checkEmailOrPhoneExist_a(type, email, countryCode, phoneNumber)
         return data.get("checkEmailOrPhoneExist", False)
 
-    async def modifyContact(self, contactId: str, isAdmin: bool, contactName: str = "", fileId: str = "") -> Dict[str, Any]:
+    async def modifyContact(self, contactId: str, isAdmin: bool, contactName: str = "", fileId: str = "") -> dict[str, any]:
         data = await self._gql_handler.modifyContact_a(contactId, isAdmin, contactName, fileId)
         return data
 
     async def deleteMessageFromApp(self, wuid: str, msgId: str) -> bool:
         data = await self._gql_handler.deleteMessageFromApp_a(wuid, msgId)
         if data.get("deleteMsg", False):
             return True
```

### Comparing `pyxplora_api-2.8.3/src/pyxplora_api/status.py` & `pyxplora_api-2.9.0/src/pyxplora_api/status.py`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.3/src/pyxplora_api.egg-info/PKG-INFO` & `pyxplora_api-2.9.0/src/pyxplora_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxplora-api
-Version: 2.8.3
+Version: 2.9.0
 Summary: Python Xplora® Api
 Home-page: https://github.com/Ludy87/pyxplora_api
 Author: Ludy87
 Author-email: android@astra-g.org
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Ludy87/pyxplora_api/issues
 Keywords: api xplora watch
@@ -127,15 +127,15 @@
 | getWatchChats(wuid: str, offset: int = 0, limit: int = 0, msgId: str = "")                               | list[dict[str, any]]: | "msgId", "type", "sender_id", "sender_name", "receiver_id", receiver_name", "data_text", data_sender_name", "create" |
 | getWatchChatsRaw(wuid: str, offset: int = 0, limit: int = 0, msgId: str = "", show_del_msg: bool = True) | list[dict[str, any]]: |
 | getSWInfo(wuid: str)                                                                                     | dict[str, any]:       |
 | getWatchState(wuid: str)                                                                                 | dict[str, any]:       |
 
 ## Watch: Location Infos
 
-| Function                                                      | Result Type           | Retrun        |
+| Function                                                      | Result Type           | Return        |
 | ------------------------------------------------------------- | --------------------- | ------------- |
 | getWatchLastLocation(wuid: str, withAsk: bool = False)        | dict[str, any]:       |               |
 | getWatchLocate(wuid: str)                                     | dict[str, any]:       |               |
 | getWatchLocateType(wuid: str)                                 | str:                  | GPS/WIFI/CELL |
 | getWatchSafeZones(wuid: str)                                  | list[dict[str, any]]: |               |
 | getWatchIsInSafeZone(wuid: str)                               | bool:                 |               |
 | getWatchSafeZoneLabel(wuid: str)                              | str:                  |               |
@@ -491,15 +491,15 @@
 | Online Status                    | read       | str  |                                                 |
 | Unread Msg Count                 | read       | int  | ?BUG? Result is always 0                        |
 | Chats                            | read       | list | Don't all chats - confused                      |
 | last locate                      | read       | dict |                                                 |
 | locate Type                      | read       | str  | GPS/WIFI/CELL                                   |
 | locate now                       | read       | dict |                                                 |
 | is in Safezone                   | read       | bool |                                                 |
-| Safezone Lable                   | read       | str  |                                                 |
+| Safezone Label                   | read       | str  |                                                 |
 | Safezone                         | read/write | list |                                                 |
 | track Interval                   | read       | int  |                                                 |
 | ask Watch Locate                 | read       | bool |                                                 |
 | silents                          | read       | list | get all/enable/disable - enable all/disable all |
 | sendText                         | read       | bool | sender: logged User                             |
 | shutdown                         | read       | bool | only admins                                     |
 | reboot                           | read       | bool | only admins                                     |
```

### Comparing `pyxplora_api-2.8.3/src/pyxplora_api.egg-info/SOURCES.txt` & `pyxplora_api-2.9.0/src/pyxplora_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

