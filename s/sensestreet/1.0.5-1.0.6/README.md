# Comparing `tmp/sensestreet-1.0.5.tar.gz` & `tmp/sensestreet-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sensestreet-1.0.5.tar", last modified: Wed Nov 15 11:51:52 2023, max compression
+gzip compressed data, was "sensestreet-1.0.6.tar", last modified: Wed Apr 24 07:29:32 2024, max compression
```

## Comparing `sensestreet-1.0.5.tar` & `sensestreet-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 michalg   (1001) michalg   (1001)        0 2023-11-15 11:51:52.250480 sensestreet-1.0.5/
--rw-rw-r--   0 michalg   (1001) michalg   (1001)    11327 2023-06-21 13:47:45.000000 sensestreet-1.0.5/LICENSE
--rw-rw-r--   0 michalg   (1001) michalg   (1001)     4322 2023-11-15 11:51:52.250480 sensestreet-1.0.5/PKG-INFO
--rw-rw-r--   0 michalg   (1001) michalg   (1001)     3280 2023-11-15 11:48:36.000000 sensestreet-1.0.5/README.md
--rw-rw-r--   0 michalg   (1001) michalg   (1001)      103 2023-11-15 11:51:52.250480 sensestreet-1.0.5/setup.cfg
--rw-rw-r--   0 michalg   (1001) michalg   (1001)      649 2023-11-15 11:48:36.000000 sensestreet-1.0.5/setup.py
-drwxrwxr-x   0 michalg   (1001) michalg   (1001)        0 2023-11-15 11:51:52.246479 sensestreet-1.0.5/src/
-drwxrwxr-x   0 michalg   (1001) michalg   (1001)        0 2023-11-15 11:51:52.246479 sensestreet-1.0.5/src/sensestreet/
--rw-rw-r--   0 michalg   (1001) michalg   (1001)       49 2023-06-21 13:47:45.000000 sensestreet-1.0.5/src/sensestreet/__init__.py
--rw-rw-r--   0 michalg   (1001) michalg   (1001)    11899 2023-11-15 11:48:36.000000 sensestreet-1.0.5/src/sensestreet/sensestreet_client.py
-drwxrwxr-x   0 michalg   (1001) michalg   (1001)        0 2023-11-15 11:51:52.250480 sensestreet-1.0.5/src/sensestreet.egg-info/
--rw-rw-r--   0 michalg   (1001) michalg   (1001)     4322 2023-11-15 11:51:52.000000 sensestreet-1.0.5/src/sensestreet.egg-info/PKG-INFO
--rw-rw-r--   0 michalg   (1001) michalg   (1001)      296 2023-11-15 11:51:52.000000 sensestreet-1.0.5/src/sensestreet.egg-info/SOURCES.txt
--rw-rw-r--   0 michalg   (1001) michalg   (1001)        1 2023-11-15 11:51:52.000000 sensestreet-1.0.5/src/sensestreet.egg-info/dependency_links.txt
--rw-rw-r--   0 michalg   (1001) michalg   (1001)       28 2023-11-15 11:51:52.000000 sensestreet-1.0.5/src/sensestreet.egg-info/requires.txt
--rw-rw-r--   0 michalg   (1001) michalg   (1001)       12 2023-11-15 11:51:52.000000 sensestreet-1.0.5/src/sensestreet.egg-info/top_level.txt
+drwxrwxr-x   0 michalg   (1001) michalg   (1001)        0 2024-04-24 07:29:32.518621 sensestreet-1.0.6/
+-rw-rw-r--   0 michalg   (1001) michalg   (1001)    11327 2023-06-21 13:47:45.000000 sensestreet-1.0.6/LICENSE
+-rw-rw-r--   0 michalg   (1001) michalg   (1001)     4047 2024-04-24 07:29:32.518621 sensestreet-1.0.6/PKG-INFO
+-rw-rw-r--   0 michalg   (1001) michalg   (1001)     3778 2024-04-24 07:26:03.000000 sensestreet-1.0.6/README.md
+-rw-rw-r--   0 michalg   (1001) michalg   (1001)      103 2024-04-24 07:29:32.518621 sensestreet-1.0.6/setup.cfg
+-rw-rw-r--   0 michalg   (1001) michalg   (1001)      649 2024-04-24 07:27:45.000000 sensestreet-1.0.6/setup.py
+drwxrwxr-x   0 michalg   (1001) michalg   (1001)        0 2024-04-24 07:29:32.514621 sensestreet-1.0.6/src/
+drwxrwxr-x   0 michalg   (1001) michalg   (1001)        0 2024-04-24 07:29:32.514621 sensestreet-1.0.6/src/sensestreet/
+-rw-rw-r--   0 michalg   (1001) michalg   (1001)      108 2024-04-24 07:26:03.000000 sensestreet-1.0.6/src/sensestreet/__init__.py
+-rw-rw-r--   0 michalg   (1001) michalg   (1001)     5628 2024-04-24 07:26:03.000000 sensestreet-1.0.6/src/sensestreet/anonymise.py
+-rw-rw-r--   0 michalg   (1001) michalg   (1001)    11899 2024-04-24 07:27:45.000000 sensestreet-1.0.6/src/sensestreet/sensestreet_client.py
+drwxrwxr-x   0 michalg   (1001) michalg   (1001)        0 2024-04-24 07:29:32.518621 sensestreet-1.0.6/src/sensestreet.egg-info/
+-rw-rw-r--   0 michalg   (1001) michalg   (1001)     4047 2024-04-24 07:29:32.000000 sensestreet-1.0.6/src/sensestreet.egg-info/PKG-INFO
+-rw-rw-r--   0 michalg   (1001) michalg   (1001)      325 2024-04-24 07:29:32.000000 sensestreet-1.0.6/src/sensestreet.egg-info/SOURCES.txt
+-rw-rw-r--   0 michalg   (1001) michalg   (1001)        1 2024-04-24 07:29:32.000000 sensestreet-1.0.6/src/sensestreet.egg-info/dependency_links.txt
+-rw-rw-r--   0 michalg   (1001) michalg   (1001)       28 2024-04-24 07:29:32.000000 sensestreet-1.0.6/src/sensestreet.egg-info/requires.txt
+-rw-rw-r--   0 michalg   (1001) michalg   (1001)       12 2024-04-24 07:29:32.000000 sensestreet-1.0.6/src/sensestreet.egg-info/top_level.txt
```

### Comparing `sensestreet-1.0.5/LICENSE` & `sensestreet-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sensestreet-1.0.5/PKG-INFO` & `sensestreet-1.0.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,109 +1,132 @@
 Metadata-Version: 2.1
 Name: sensestreet
-Version: 1.0.5
+Version: 1.0.6
 Summary: UNKNOWN
 Home-page: https://sensestreet.com
 Author: Sense Street
 Author-email: engineering@sensestreet.com
 License: Apache
-Description: # sensestreet
-        This is a Python client for Sense Street API.
-        
-        # Run the client
-        In order to use the client, import SenseStreetClient from sensestreet:
-        ```
-        from sensestreet import SenseStreetClient
-        ```
-        and provide the app_id and api_url:
-        ```
-        client = SenseStreetClient(app_id="test", api_url="https://server.com/api")
-        ```
-        To simply ping the server, use:
-        ```
-        client.ping()
-        ```
-        
-        # Overview of all functions:
-        
-        ## Pings
-        ```
-        ping()
-        ```
-        Sends ping to the server to check if server is up and responding.
-        
-        ```
-        ping_auth()
-        ```
-        Similar to ping but with authorisation - easy way to check if you're authorised to send requests to the server.
-        
-        ## Requests to prediction server:
-        
-        ```
-        predict_rfqs(conversation, options)
-        ```
-        Sends request to predict rfqs in a conversation. Conversation has to be either a dict or a json.
-        
-        ```
-        chat_snippet_predict_rfqs(chat_snippet, options)
-        ```
-        Sends request to predict rfqs in the conversation. Conversation has to be either a dict or a json. The difference between this function and the one above is the structure of the conversation, <em>predict_rfqs</em> is for a conversation in the Sense Street's format, while <em>chat_snippet_predict_rfqs</em> is for conversation that is a cutout from the chat.
-        
-        ## Batch job requests:
-        ```
-        upload_files_with_conversations(files_paths)
-        ```
-        Uploads specified files with conversation to be processed by the server. It returns an id for each file that will be nedded later on to obtain processed conversations. To run this function you need to have permission to open these files. Make sure you're not trying to upload over 1Gb of files in a single request.
-        
-        ```
-        upload_file_with_bond(file_path)
-        ```
-        Uploads file with bond data to the server.
-        
-        ```
-        get_processed_conv_file(file_id, save_path)
-        ```
-        Returns file with processed conversations, <em>file_id</em> is the id that was returned during the files upload - by the <em>upload_files_with_conversations</em> function.
-        
-        ```
-        get_conv_file_status(file_id)
-        ```
-        Returns the status of the uploaded file. With this function you can check if the file has already been processed by the server and is ready for download.
-        
-        # How to use your key to authorise requests
-        In order to send requests to the server you need to obtain a pair of keys - public and private (if you don't have a key contact the Sense Street to get one). In order to be correctly authorised by the server initialised the SenseStreetClient with the paths to both of the keys:
-        
-        ```
-        client = SenseStreetClient(
-            app_id="id of your app",
-            api_url="https://server.com/api",
-            priv_key_path='path to your private key',
-            pub_key_path='path to your public key'
-            )
-        ```
-        
-        # How to define proxies
-        In order to use proxy provide a dict of proxies when initializing Sense Street Client, eg.:
-        ```
-        client = SenseStreetClient(
-            app_id="id of your app",
-            api_url="https://server.com/api",
-            request_args= { 'proxies': {
-                "https": "https://10.10.1.10:1080",
-                    }
-                }
-            )
-        ```
-        
-        To read more about proxies refer to: https://requests.readthedocs.io/en/latest/user/advanced/#proxies
-        Similarly any additional request argument can be added:
-        
-        ```
-        client = SenseStreetClient(
-            app_id="id of your app",
-            api_url="https://server.com/api",
-            request_args= { 'verify': 'path'
-                }
-            )
-        ```
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# SenseStreetClient
+This is a Python client for Sense Street API.
+
+# Run the client
+In order to use the client, import SenseStreetClient from sensestreet:
+```
+from sensestreet import SenseStreetClient
+```
+and provide the app_id and api_url:
+```
+client = SenseStreetClient(app_id="test", api_url="https://server.com/api")
+```
+To simply ping the server, use:
+```
+client.ping()
+```
+
+# Overview of all functions:
+
+## Pings
+```
+ping()
+```
+Sends ping to the server to check if server is up and responding.
+
+```
+ping_auth()
+```
+Similar to ping but with authorisation - easy way to check if you're authorised to send requests to the server.
+
+## Requests to prediction server:
+
+```
+predict_rfqs(conversation, options)
+```
+Sends request to predict rfqs in a conversation. Conversation has to be either a dict or a json.
+
+```
+chat_snippet_predict_rfqs(chat_snippet, options)
+```
+Sends request to predict rfqs in the conversation. Conversation has to be either a dict or a json. The difference between this function and the one above is the structure of the conversation, <em>predict_rfqs</em> is for a conversation in the Sense Street's format, while <em>chat_snippet_predict_rfqs</em> is for conversation that is a cutout from the chat.
+
+## Batch job requests:
+```
+upload_files_with_conversations(files_paths)
+```
+Uploads specified files with conversation to be processed by the server. It returns an id for each file that will be nedded later on to obtain processed conversations. To run this function you need to have permission to open these files. Make sure you're not trying to upload over 1Gb of files in a single request.
+
+```
+upload_file_with_bond(file_path)
+```
+Uploads file with bond data to the server.
+
+```
+get_processed_conv_file(file_id, save_path)
+```
+Returns file with processed conversations, <em>file_id</em> is the id that was returned during the files upload - by the <em>upload_files_with_conversations</em> function.
+
+```
+get_conv_file_status(file_id)
+```
+Returns the status of the uploaded file. With this function you can check if the file has already been processed by the server and is ready for download.
+
+# How to use your key to authorise requests
+In order to send requests to the server you need to obtain a pair of keys - public and private (if you don't have a key contact the Sense Street to get one). In order to be correctly authorised by the server initialised the SenseStreetClient with the paths to both of the keys:
+
+```
+client = SenseStreetClient(
+    app_id="id of your app",
+    api_url="https://server.com/api",
+    priv_key_path='path to your private key',
+    pub_key_path='path to your public key'
+    )
+```
+
+# How to define proxies
+In order to use proxy provide a dict of proxies when initializing Sense Street Client, eg.:
+```
+client = SenseStreetClient(
+    app_id="id of your app",
+    api_url="https://server.com/api",
+    request_args= { 'proxies': {
+        "https": "https://10.10.1.10:1080",
+            }
+        }
+    )
+```
+
+To read more about proxies refer to: https://requests.readthedocs.io/en/latest/user/advanced/#proxies
+Similarly any additional request argument can be added:
+
+```
+client = SenseStreetClient(
+    app_id="id of your app",
+    api_url="https://server.com/api",
+    request_args= { 'verify': 'path'
+        }
+    )
+```
+
+# anonymise_bbg_xml
+Method for anonymisation of xml in bbg format.
+
+# example
+Parameters:
+xml_in: str - The input XML file path.
+xml_out: str - The output file path where the anonymized XML will be saved.
+mapping: str - The path to the JSON mapping file.
+bank_pattern: str - Regular expression pattern to identify bank side in conversation.
+
+```
+from sensestreet import anonymise_bbg_xml
+anonymise_bbg_xml(
+    "./example.xml",
+    "./test.xml",
+    "./mapping.json",
+    r"\bbank\b",
+)
+```
+
```

### Comparing `sensestreet-1.0.5/README.md` & `sensestreet-1.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# sensestreet
+# SenseStreetClient
 This is a Python client for Sense Street API.
 
 # Run the client
 In order to use the client, import SenseStreetClient from sensestreet:
 ```
 from sensestreet import SenseStreetClient
 ```
@@ -92,8 +92,28 @@
 ```
 client = SenseStreetClient(
     app_id="id of your app",
     api_url="https://server.com/api",
     request_args= { 'verify': 'path'
         }
     )
+```
+
+# anonymise_bbg_xml
+Method for anonymisation of xml in bbg format.
+
+# example
+Parameters:
+xml_in: str - The input XML file path.
+xml_out: str - The output file path where the anonymized XML will be saved.
+mapping: str - The path to the JSON mapping file.
+bank_pattern: str - Regular expression pattern to identify bank side in conversation.
+
+```
+from sensestreet import anonymise_bbg_xml
+anonymise_bbg_xml(
+    "./example.xml",
+    "./test.xml",
+    "./mapping.json",
+    r"\bbank\b",
+)
 ```
```

### Comparing `sensestreet-1.0.5/setup.py` & `sensestreet-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name='sensestreet',
-    version='1.0.5',
+    version='1.0.6',
     license='Apache',
     packages=find_packages('src'),
     author="Sense Street",
     author_email="engineering@sensestreet.com",
     url="https://sensestreet.com",
     package_dir={'': 'src'},
     install_requires=[
```

### Comparing `sensestreet-1.0.5/src/sensestreet/sensestreet_client.py` & `sensestreet-1.0.6/src/sensestreet/sensestreet_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
     get_conv_file_status(file_id):
         Check if conversations sent in file with the file_id have already been processed.
     
     
 
     """
-    __version__ = "1.0.5"
+    __version__ = "1.0.6"
 
     def __init__(self, app_id, api_url, priv_key_path=None, pub_key_id='default.pub', server_id='default', 
             req_timeout_sec=500, pub_key_path=None, extra_headers=None, request_args=None):
         self.api_url = self._prepare_api_url(api_url)
         self.app_id = app_id
         self.server_id = server_id
         self.pub_key_id = pub_key_id
```

### Comparing `sensestreet-1.0.5/src/sensestreet.egg-info/PKG-INFO` & `sensestreet-1.0.6/src/sensestreet.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,109 +1,132 @@
 Metadata-Version: 2.1
 Name: sensestreet
-Version: 1.0.5
+Version: 1.0.6
 Summary: UNKNOWN
 Home-page: https://sensestreet.com
 Author: Sense Street
 Author-email: engineering@sensestreet.com
 License: Apache
-Description: # sensestreet
-        This is a Python client for Sense Street API.
-        
-        # Run the client
-        In order to use the client, import SenseStreetClient from sensestreet:
-        ```
-        from sensestreet import SenseStreetClient
-        ```
-        and provide the app_id and api_url:
-        ```
-        client = SenseStreetClient(app_id="test", api_url="https://server.com/api")
-        ```
-        To simply ping the server, use:
-        ```
-        client.ping()
-        ```
-        
-        # Overview of all functions:
-        
-        ## Pings
-        ```
-        ping()
-        ```
-        Sends ping to the server to check if server is up and responding.
-        
-        ```
-        ping_auth()
-        ```
-        Similar to ping but with authorisation - easy way to check if you're authorised to send requests to the server.
-        
-        ## Requests to prediction server:
-        
-        ```
-        predict_rfqs(conversation, options)
-        ```
-        Sends request to predict rfqs in a conversation. Conversation has to be either a dict or a json.
-        
-        ```
-        chat_snippet_predict_rfqs(chat_snippet, options)
-        ```
-        Sends request to predict rfqs in the conversation. Conversation has to be either a dict or a json. The difference between this function and the one above is the structure of the conversation, <em>predict_rfqs</em> is for a conversation in the Sense Street's format, while <em>chat_snippet_predict_rfqs</em> is for conversation that is a cutout from the chat.
-        
-        ## Batch job requests:
-        ```
-        upload_files_with_conversations(files_paths)
-        ```
-        Uploads specified files with conversation to be processed by the server. It returns an id for each file that will be nedded later on to obtain processed conversations. To run this function you need to have permission to open these files. Make sure you're not trying to upload over 1Gb of files in a single request.
-        
-        ```
-        upload_file_with_bond(file_path)
-        ```
-        Uploads file with bond data to the server.
-        
-        ```
-        get_processed_conv_file(file_id, save_path)
-        ```
-        Returns file with processed conversations, <em>file_id</em> is the id that was returned during the files upload - by the <em>upload_files_with_conversations</em> function.
-        
-        ```
-        get_conv_file_status(file_id)
-        ```
-        Returns the status of the uploaded file. With this function you can check if the file has already been processed by the server and is ready for download.
-        
-        # How to use your key to authorise requests
-        In order to send requests to the server you need to obtain a pair of keys - public and private (if you don't have a key contact the Sense Street to get one). In order to be correctly authorised by the server initialised the SenseStreetClient with the paths to both of the keys:
-        
-        ```
-        client = SenseStreetClient(
-            app_id="id of your app",
-            api_url="https://server.com/api",
-            priv_key_path='path to your private key',
-            pub_key_path='path to your public key'
-            )
-        ```
-        
-        # How to define proxies
-        In order to use proxy provide a dict of proxies when initializing Sense Street Client, eg.:
-        ```
-        client = SenseStreetClient(
-            app_id="id of your app",
-            api_url="https://server.com/api",
-            request_args= { 'proxies': {
-                "https": "https://10.10.1.10:1080",
-                    }
-                }
-            )
-        ```
-        
-        To read more about proxies refer to: https://requests.readthedocs.io/en/latest/user/advanced/#proxies
-        Similarly any additional request argument can be added:
-        
-        ```
-        client = SenseStreetClient(
-            app_id="id of your app",
-            api_url="https://server.com/api",
-            request_args= { 'verify': 'path'
-                }
-            )
-        ```
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# SenseStreetClient
+This is a Python client for Sense Street API.
+
+# Run the client
+In order to use the client, import SenseStreetClient from sensestreet:
+```
+from sensestreet import SenseStreetClient
+```
+and provide the app_id and api_url:
+```
+client = SenseStreetClient(app_id="test", api_url="https://server.com/api")
+```
+To simply ping the server, use:
+```
+client.ping()
+```
+
+# Overview of all functions:
+
+## Pings
+```
+ping()
+```
+Sends ping to the server to check if server is up and responding.
+
+```
+ping_auth()
+```
+Similar to ping but with authorisation - easy way to check if you're authorised to send requests to the server.
+
+## Requests to prediction server:
+
+```
+predict_rfqs(conversation, options)
+```
+Sends request to predict rfqs in a conversation. Conversation has to be either a dict or a json.
+
+```
+chat_snippet_predict_rfqs(chat_snippet, options)
+```
+Sends request to predict rfqs in the conversation. Conversation has to be either a dict or a json. The difference between this function and the one above is the structure of the conversation, <em>predict_rfqs</em> is for a conversation in the Sense Street's format, while <em>chat_snippet_predict_rfqs</em> is for conversation that is a cutout from the chat.
+
+## Batch job requests:
+```
+upload_files_with_conversations(files_paths)
+```
+Uploads specified files with conversation to be processed by the server. It returns an id for each file that will be nedded later on to obtain processed conversations. To run this function you need to have permission to open these files. Make sure you're not trying to upload over 1Gb of files in a single request.
+
+```
+upload_file_with_bond(file_path)
+```
+Uploads file with bond data to the server.
+
+```
+get_processed_conv_file(file_id, save_path)
+```
+Returns file with processed conversations, <em>file_id</em> is the id that was returned during the files upload - by the <em>upload_files_with_conversations</em> function.
+
+```
+get_conv_file_status(file_id)
+```
+Returns the status of the uploaded file. With this function you can check if the file has already been processed by the server and is ready for download.
+
+# How to use your key to authorise requests
+In order to send requests to the server you need to obtain a pair of keys - public and private (if you don't have a key contact the Sense Street to get one). In order to be correctly authorised by the server initialised the SenseStreetClient with the paths to both of the keys:
+
+```
+client = SenseStreetClient(
+    app_id="id of your app",
+    api_url="https://server.com/api",
+    priv_key_path='path to your private key',
+    pub_key_path='path to your public key'
+    )
+```
+
+# How to define proxies
+In order to use proxy provide a dict of proxies when initializing Sense Street Client, eg.:
+```
+client = SenseStreetClient(
+    app_id="id of your app",
+    api_url="https://server.com/api",
+    request_args= { 'proxies': {
+        "https": "https://10.10.1.10:1080",
+            }
+        }
+    )
+```
+
+To read more about proxies refer to: https://requests.readthedocs.io/en/latest/user/advanced/#proxies
+Similarly any additional request argument can be added:
+
+```
+client = SenseStreetClient(
+    app_id="id of your app",
+    api_url="https://server.com/api",
+    request_args= { 'verify': 'path'
+        }
+    )
+```
+
+# anonymise_bbg_xml
+Method for anonymisation of xml in bbg format.
+
+# example
+Parameters:
+xml_in: str - The input XML file path.
+xml_out: str - The output file path where the anonymized XML will be saved.
+mapping: str - The path to the JSON mapping file.
+bank_pattern: str - Regular expression pattern to identify bank side in conversation.
+
+```
+from sensestreet import anonymise_bbg_xml
+anonymise_bbg_xml(
+    "./example.xml",
+    "./test.xml",
+    "./mapping.json",
+    r"\bbank\b",
+)
+```
+
```

