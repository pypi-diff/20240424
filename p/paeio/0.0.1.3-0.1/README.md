# Comparing `tmp/paeio-0.0.1.3.tar.gz` & `tmp/paeio-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paeio-0.0.1.3.tar", last modified: Fri Mar  8 02:54:42 2024, max compression
+gzip compressed data, was "paeio-0.1.tar", last modified: Wed Apr 24 03:31:03 2024, max compression
```

## Comparing `paeio-0.0.1.3.tar` & `paeio-0.1.tar`

### file list

```diff
@@ -1,24 +1,19 @@
-drwxrwxr-x   0 atena_user  (1014) atena_user  (1014)        0 2024-03-08 02:54:42.405860 paeio-0.0.1.3/
--rw-rw-r--   0 atena_user  (1014) atena_user  (1014)     1068 2024-03-07 02:27:04.000000 paeio-0.0.1.3/LICENSE
--rw-r--r--   0 atena_user  (1014) atena_user  (1014)     3368 2024-03-08 02:54:42.405860 paeio-0.0.1.3/PKG-INFO
--rw-rw-r--   0 atena_user  (1014) atena_user  (1014)     2288 2024-03-08 02:03:54.000000 paeio-0.0.1.3/README.md
-drwxrwxr-x   0 atena_user  (1014) atena_user  (1014)        0 2024-03-08 02:54:42.401860 paeio-0.0.1.3/paeio/
-drwxrwxr-x   0 atena_user  (1014) atena_user  (1014)        0 2024-03-08 02:54:42.405860 paeio-0.0.1.3/paeio/data_cleaning/
--rw-rw-r--   0 atena_user  (1014) atena_user  (1014)     1369 2024-03-08 00:20:55.000000 paeio-0.0.1.3/paeio/data_cleaning/dates_holidays.py
--rw-rw-r--   0 atena_user  (1014) atena_user  (1014)     3165 2024-03-08 00:20:55.000000 paeio-0.0.1.3/paeio/data_cleaning/feature_engineering.py
--rw-rw-r--   0 atena_user  (1014) atena_user  (1014)    11213 2024-03-08 00:20:55.000000 paeio-0.0.1.3/paeio/data_cleaning/file_reading.py
--rw-rw-r--   0 atena_user  (1014) atena_user  (1014)     2104 2024-03-08 00:20:55.000000 paeio-0.0.1.3/paeio/data_cleaning/parallelism.py
--rw-rw-r--   0 atena_user  (1014) atena_user  (1014)     1133 2024-03-08 00:20:55.000000 paeio-0.0.1.3/paeio/data_cleaning/path.py
--rw-rw-r--   0 atena_user  (1014) atena_user  (1014)     1514 2024-03-08 00:20:55.000000 paeio-0.0.1.3/paeio/data_cleaning/utils.py
-drwxrwxr-x   0 atena_user  (1014) atena_user  (1014)        0 2024-03-08 02:54:42.405860 paeio-0.0.1.3/paeio/io/
--rw-rw-r--   0 atena_user  (1014) atena_user  (1014)    19655 2024-03-08 00:20:55.000000 paeio-0.0.1.3/paeio/io/io.py
--rw-rw-r--   0 atena_user  (1014) atena_user  (1014)     1081 2024-03-08 00:20:55.000000 paeio-0.0.1.3/paeio/io/keyvault.py
-drwxrwxr-x   0 atena_user  (1014) atena_user  (1014)        0 2024-03-08 02:54:42.405860 paeio-0.0.1.3/paeio.egg-info/
--rw-r--r--   0 atena_user  (1014) atena_user  (1014)     3368 2024-03-08 02:54:42.000000 paeio-0.0.1.3/paeio.egg-info/PKG-INFO
--rw-rw-r--   0 atena_user  (1014) atena_user  (1014)      448 2024-03-08 02:54:42.000000 paeio-0.0.1.3/paeio.egg-info/SOURCES.txt
--rw-rw-r--   0 atena_user  (1014) atena_user  (1014)        1 2024-03-08 02:54:42.000000 paeio-0.0.1.3/paeio.egg-info/dependency_links.txt
--rw-rw-r--   0 atena_user  (1014) atena_user  (1014)      132 2024-03-08 02:54:42.000000 paeio-0.0.1.3/paeio.egg-info/requires.txt
--rw-rw-r--   0 atena_user  (1014) atena_user  (1014)        6 2024-03-08 02:54:42.000000 paeio-0.0.1.3/paeio.egg-info/top_level.txt
--rw-rw-r--   0 atena_user  (1014) atena_user  (1014)      958 2024-03-08 02:52:55.000000 paeio-0.0.1.3/pyproject.toml
--rw-rw-r--   0 atena_user  (1014) atena_user  (1014)      131 2024-03-08 02:52:11.000000 paeio-0.0.1.3/requirements.txt
--rw-rw-r--   0 atena_user  (1014) atena_user  (1014)      108 2024-03-08 02:54:42.405860 paeio-0.0.1.3/setup.cfg
+drwxrwxr-x   0 atena_user  (1014) atena_user  (1014)        0 2024-04-24 03:31:03.875609 paeio-0.1/
+-rw-rw-r--   0 atena_user  (1014) atena_user  (1014)     1068 2024-03-07 02:27:04.000000 paeio-0.1/LICENSE
+-rw-r--r--   0 atena_user  (1014) atena_user  (1014)     3178 2024-04-24 03:31:03.875609 paeio-0.1/PKG-INFO
+-rw-rw-r--   0 atena_user  (1014) atena_user  (1014)     2288 2024-04-23 01:44:22.000000 paeio-0.1/README.md
+drwxrwxr-x   0 atena_user  (1014) atena_user  (1014)        0 2024-04-24 03:31:03.871610 paeio-0.1/paeio/
+-rw-rw-r--   0 atena_user  (1014) atena_user  (1014)        0 2024-04-24 03:19:58.000000 paeio-0.1/paeio/__init__.py
+-rw-rw-r--   0 atena_user  (1014) atena_user  (1014)    18996 2024-04-24 03:19:58.000000 paeio-0.1/paeio/io.py
+-rw-rw-r--   0 atena_user  (1014) atena_user  (1014)     2070 2024-04-24 03:19:58.000000 paeio-0.1/paeio/parallelism.py
+-rw-rw-r--   0 atena_user  (1014) atena_user  (1014)     1142 2024-04-24 03:19:58.000000 paeio-0.1/paeio/path.py
+-rw-rw-r--   0 atena_user  (1014) atena_user  (1014)     5673 2024-04-24 03:19:58.000000 paeio-0.1/paeio/versioned.py
+drwxrwxr-x   0 atena_user  (1014) atena_user  (1014)        0 2024-04-24 03:31:03.875609 paeio-0.1/paeio.egg-info/
+-rw-r--r--   0 atena_user  (1014) atena_user  (1014)     3178 2024-04-24 03:31:03.000000 paeio-0.1/paeio.egg-info/PKG-INFO
+-rw-rw-r--   0 atena_user  (1014) atena_user  (1014)      287 2024-04-24 03:31:03.000000 paeio-0.1/paeio.egg-info/SOURCES.txt
+-rw-rw-r--   0 atena_user  (1014) atena_user  (1014)        1 2024-04-24 03:31:03.000000 paeio-0.1/paeio.egg-info/dependency_links.txt
+-rw-rw-r--   0 atena_user  (1014) atena_user  (1014)       94 2024-04-24 03:31:03.000000 paeio-0.1/paeio.egg-info/requires.txt
+-rw-rw-r--   0 atena_user  (1014) atena_user  (1014)        6 2024-04-24 03:31:03.000000 paeio-0.1/paeio.egg-info/top_level.txt
+-rw-rw-r--   0 atena_user  (1014) atena_user  (1014)      861 2024-04-24 03:28:37.000000 paeio-0.1/pyproject.toml
+-rw-rw-r--   0 atena_user  (1014) atena_user  (1014)       93 2024-04-24 03:19:58.000000 paeio-0.1/requirements.txt
+-rw-rw-r--   0 atena_user  (1014) atena_user  (1014)      114 2024-04-24 03:31:03.875609 paeio-0.1/setup.cfg
```

### Comparing `paeio-0.0.1.3/LICENSE` & `paeio-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `paeio-0.0.1.3/PKG-INFO` & `paeio-0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Metadata-Version: 2.1
 Name: paeio
-Version: 0.0.1.3
+Version: 0.1
 Summary: Utilities library for read/write operations and general data cleaning routines
-Author-email: João Pedro Alves <jotapedro1997@gmail.com>, "Mauricio (Pae) Araujo" <mauricio.araujo97@gmail.com>
+Author-email: João Pedro Alves <jotapedro1997@gmail.com>
 Project-URL: Homepage, https://github.com/jotap123/paeio/tree/develop
 Project-URL: Issues, https://github.com/jotap123/paeio/issues
 Project-URL: Linkedin_JP, https://www.linkedin.com/in/jp111/
-Project-URL: Linkedin_Pae, https://www.linkedin.com/in/mauricio-arauujo/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 2 - Pre-Alpha
-Requires-Python: >=3.8
+Classifier: Development Status :: 5 - Production/Stable
+Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: azure-identity
-Requires-Dist: azure-keyvault
-Requires-Dist: azure-keyvault-secrets
 Requires-Dist: azure-storage-file-datalake
 Requires-Dist: joblib
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyarrow
 Requires-Dist: openpyxl
 Requires-Dist: python-dotenv
@@ -36,33 +33,33 @@
 
 ## Project Structure
 
 ```plaintext
 paeio
 ├── README.md
 ├── docs            -> Folder containing files for building the library.
-├── ipp_ds              -> Folder containing the library's code
+├── paeio              -> Folder containing the library's code
 │   ├── data_cleaning         -> Module for data cleaning.
 │   └── io                    -> Module for I/O operations.
 ├── dist             -> Folder containing files for package distribution
 │   ├── __init__.py
-│   └── ipp_ds-0.X-py3-none-any.whl                -> Installation with pip will be done from here.
+│   └── paeio-0.X-py3-none-any.whl               -> Installation with pip will be done from here.
 ├── tests            -> Folder containing test files for validating the package's implementations.
 ├── requirements.txt          -> Required packages to run the project
 └── pyproject.toml                  -> Setup file for generating the package installer.
 ```
 
 ## Daily Use
 
 ### Library Installation
 
 For development, it's highly recommended to create a separate environment. To do this, run:
 
 ```bash
-$ conda create -n paeio python==3.X (X >= 9)
+$ conda create -n paeio python==3.X #(X >= 7.1)
 ```
 
 For installation via pip, run the following command:
 
 ```bash
 $ pip3 install paeio
 ```
```

### Comparing `paeio-0.0.1.3/README.md` & `paeio-0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,33 +9,33 @@
 
 ## Project Structure
 
 ```plaintext
 paeio
 ├── README.md
 ├── docs            -> Folder containing files for building the library.
-├── ipp_ds              -> Folder containing the library's code
+├── paeio              -> Folder containing the library's code
 │   ├── data_cleaning         -> Module for data cleaning.
 │   └── io                    -> Module for I/O operations.
 ├── dist             -> Folder containing files for package distribution
 │   ├── __init__.py
-│   └── ipp_ds-0.X-py3-none-any.whl                -> Installation with pip will be done from here.
+│   └── paeio-0.X-py3-none-any.whl               -> Installation with pip will be done from here.
 ├── tests            -> Folder containing test files for validating the package's implementations.
 ├── requirements.txt          -> Required packages to run the project
 └── pyproject.toml                  -> Setup file for generating the package installer.
 ```
 
 ## Daily Use
 
 ### Library Installation
 
 For development, it's highly recommended to create a separate environment. To do this, run:
 
 ```bash
-$ conda create -n paeio python==3.X (X >= 9)
+$ conda create -n paeio python==3.X #(X >= 7.1)
 ```
 
 For installation via pip, run the following command:
 
 ```bash
 $ pip3 install paeio
 ```
```

### Comparing `paeio-0.0.1.3/paeio/data_cleaning/path.py` & `paeio-0.1/paeio/path.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import re
+
 import pandas as pd
 
 
-def path_join(*args, sep='/'):
-    """ Une partes de um path """
+def path_join(*args, sep="/"):
+    """Concatenate n strings to form a path."""
     return f"{sep}".join([*args])
 
 
 def get_date_from_names(names_list, sep="_", occ=-1):
-    """ Given a list with filenames, returns the dates contained within each filename
-    """
+    """Given a list with filenames, returns the dates contained within each filename"""
     result_list = []
     for item in names_list:
         if sep == "_":
             match = re.search(r"\d{4}_\d{2}_\d{2}", item.split("/")[occ])
         elif sep == "-":
             match = re.search(r"\d{4}-\d{2}-\d{2}", item.split("/")[occ])
         elif sep == "/":
```

### Comparing `paeio-0.0.1.3/paeio/io/io.py` & `paeio-0.1/paeio/io.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,144 +1,143 @@
-import re
 import gc
-import os
 import json
 import logging
+import os
+import pickle
+import re
 import tempfile
 import warnings
-import pandas as pd
-import numpy as np
-
 from functools import partial
 from io import BytesIO, StringIO
-from urllib.request import urlretrieve
 from typing import Union
+from urllib.request import urlretrieve
 
-from azure.storage.filedatalake import DataLakeServiceClient, DataLakeFileClient
-from azure.storage.blob import BlobServiceClient, BlobClient
-from azure.identity import DefaultAzureCredential
+import numpy as np
+import pandas as pd
 from azure.core.exceptions import ResourceNotFoundError
+from azure.identity import DefaultAzureCredential
+from azure.storage.blob import BlobClient, BlobServiceClient
+from azure.storage.filedatalake import DataLakeFileClient, DataLakeServiceClient
 
 # Set the logging level for all azure-* libraries
-logger = logging.getLogger('azure')
+logger = logging.getLogger("azure")
 logger.setLevel(logging.ERROR)
-warnings.filterwarnings('ignore')
+warnings.filterwarnings("ignore")
 
-DEFAULT_CREDENTIAL_KWARGS = json.loads(os.getenv('DEFAULT_CREDENTIAL_KWARGS', '{}'))
-DEFAULT_SERVICE_KWARGS = json.loads(os.getenv('DEFAULT_SERVICE_KWARGS', '{}'))
-DEFAULT_CONN_KWARGS = json.loads(os.getenv('DEFAULT_CONN_KWARGS', '{}'))
-DEFAULT_GLOB_CONN_KWARGS = json.loads(os.getenv('DEFAULT_GLOB_CONN_KWARGS', '{}'))
-DEFAULT_BLOB_SERVICE = os.getenv('DEFAULT_BLOB_SERVICE', 'gen2')
-DEFAULT_UPLOAD_MODE = os.getenv('DEFAULT_UPLOAD_MODE', 'full')
-DEFAULT_NUM_THREADS = os.getenv('DEFAULT_NUM_THREADS', -1)
+DEFAULT_CREDENTIAL_KWARGS = json.loads(os.getenv("DEFAULT_CREDENTIAL_KWARGS", "{}"))
+DEFAULT_SERVICE_KWARGS = json.loads(os.getenv("DEFAULT_SERVICE_KWARGS", "{}"))
+DEFAULT_CONN_KWARGS = json.loads(os.getenv("DEFAULT_CONN_KWARGS", "{}"))
+DEFAULT_GLOB_CONN_KWARGS = json.loads(os.getenv("DEFAULT_GLOB_CONN_KWARGS", "{}"))
+DEFAULT_BLOB_SERVICE = os.getenv("DEFAULT_BLOB_SERVICE", "gen2")
+DEFAULT_UPLOAD_MODE = os.getenv("DEFAULT_UPLOAD_MODE", "full")
+DEFAULT_NUM_THREADS = os.getenv("DEFAULT_NUM_THREADS", -1)
 
 
 def create_blob_service(
     uri,
     conn_type=DEFAULT_BLOB_SERVICE,
     service_kwargs=DEFAULT_SERVICE_KWARGS,
-    credential_kwargs=DEFAULT_CREDENTIAL_KWARGS
+    credential_kwargs=DEFAULT_CREDENTIAL_KWARGS,
 ):
     """
     Creates the connection service to a certain storage account
     Args:
         uri (str): Url with adress in a storage account
         conn_type (str): Type of connection to Azure. Can receive 'blob' or 'gen2'.
         service_kwargs (dict): dict with connection params to Azure services.
     Returns:
         object: DataLakeServiceClient (gen2)/BlobServiceClient (blob), depending on conn_type
     """
 
     credential = DefaultAzureCredential(**credential_kwargs)
 
-    account_name = uri.split('//')[1].split('.')[0]
+    account_name = uri.split("//")[1].split(".")[0]
 
-    if conn_type == 'gen2':
+    if conn_type == "gen2":
         dlService = DataLakeServiceClient(
             account_url=f"https://{account_name}.dfs.core.windows.net",
             credential=credential,
-            **service_kwargs
+            **service_kwargs,
         )
 
-    elif conn_type == 'blob':
+    elif conn_type == "blob":
         dlService = BlobServiceClient(
             account_url=f"https://{account_name}.blob.core.windows.net",
             credential=credential,
-            **service_kwargs
+            **service_kwargs,
         )
 
     return dlService
 
 
 def rename_file(uri_old, uri_new, conn_type=DEFAULT_BLOB_SERVICE):
-
     """
     Renames a file in an Azure Data Lake environment.
     Args:
         uri_old (str): old URL
         uri_new (str): new URL
         conn_type (str): Type of connection to Azure. Can receive 'blob' or 'gen2'.
     """
 
     service_client = create_blob_service(uri=uri_old, conn_type=conn_type)
-    container_name = uri_old.split('/')[3]
-    old_name = '/'.join(uri_old.split('/')[4:])
-    new_name = '/'.join(uri_new.split('/')[4:])
+    container_name = uri_old.split("/")[3]
+    old_name = "/".join(uri_old.split("/")[4:])
+    new_name = "/".join(uri_new.split("/")[4:])
 
     try:
-        if conn_type == 'gen2':
+        if conn_type == "gen2":
             file_system_client = service_client.get_file_system_client(
                 file_system=container_name
             )
             file_client = file_system_client.get_file_client(file_path=old_name)
 
-        elif conn_type == 'blob':
+        elif conn_type == "blob":
             file_client = service_client.get_blob_client(
                 container=container_name, blob=old_name
             )
 
         file_client.rename_file(new_name)
 
     finally:
         file_client.close()
         del file_client
 
-        if conn_type == 'gen2':
+        if conn_type == "gen2":
             file_system_client.close()
             del file_system_client
 
         service_client.close()
         del service_client
 
         gc.collect()
 
 
 def upload_chunks(
     file_client: Union[DataLakeFileClient, BlobClient],
     data: Union[BytesIO, StringIO],
-    **upload_kwargs
+    **upload_kwargs,
 ):
     """
     Generic function to upload files in chunks
 
     Args:
         file_client (Union[DataLakeFileClient,BlobClient]): Azure client file.
         data (Union[BytesIO,StringIO]): Data stream to be uploaded
         **upload_kwargs: Args to be used with upload_data/upload_blob.
         See DataLakeFileClient.upload_data ou BlobFileClient/upload_blob documentation
         for details.
 
     """
     message = "You must pass chunk_size if using upload_mode=chunks"
-    assert 'chunk_size' in upload_kwargs, message
+    assert "chunk_size" in upload_kwargs, message
 
-    if 'chunk_size' in upload_kwargs:
-        chunk_size = upload_kwargs.pop('chunk_size')
+    if "chunk_size" in upload_kwargs:
+        chunk_size = upload_kwargs.pop("chunk_size")
 
-    upload_kwargs.pop('overwrite')
+    upload_kwargs.pop("overwrite")
 
     if isinstance(file_client, DataLakeFileClient):
         file_client.create_file()
 
     elif isinstance(file_client, BlobClient):
         file_client.create_append_blob()
 
@@ -154,30 +153,30 @@
             else:
                 filesize_previous = 0
 
             file_client.append_data(
                 data=read_data,
                 offset=filesize_previous,
                 length=len(read_data),
-                **upload_kwargs
+                **upload_kwargs,
             )
-            file_client.flush_data(filesize_previous+len(read_data))
+            file_client.flush_data(filesize_previous + len(read_data))
 
         elif isinstance(data, StringIO):
-            read_data = ''.join(read_data)
+            read_data = "".join(read_data)
 
         elif isinstance(file_client, BlobClient):
             file_client.append_block(read_data, **upload_kwargs)
 
 
 def upload_data(
     byte_stream: Union[BytesIO, StringIO],
     file_client: Union[DataLakeFileClient, BlobClient],
     upload_mode: str = DEFAULT_UPLOAD_MODE,
-    **upload_kwargs
+    **upload_kwargs,
 ):
     """
     Generic function to upload files.
 
     Args:
         byte_stream (Union[BytesIO,StringIO]): Data stream to be uploaded
         file_client (Union[DataLakeFileClient,BlobClient]): Azure client file.
@@ -188,425 +187,423 @@
         for details.
     """
     if isinstance(file_client, DataLakeFileClient):
         delete_func = file_client.delete_file
     elif isinstance(file_client, BlobClient):
         delete_func = file_client.delete_blob
 
-    if upload_mode == 'full':
+    if upload_mode == "full":
         if isinstance(file_client, DataLakeFileClient):
             upload_func = file_client.upload_data
 
         elif isinstance(file_client, BlobClient):
-            if 'chunk_size' in upload_kwargs:
-                upload_kwargs.pop('chunk_size')
+            if "chunk_size" in upload_kwargs:
+                upload_kwargs.pop("chunk_size")
             upload_func = file_client.upload_blob
 
-    elif upload_mode == 'chunks':
+    elif upload_mode == "chunks":
         upload_func = partial(upload_chunks, file_client=file_client)
 
     if file_client.exists():
         delete_func()
 
     byte_stream.seek(0)
 
-    if upload_mode == 'full':
+    if upload_mode == "full":
         if isinstance(byte_stream, StringIO):
-            byte_stream = ''.join(byte_stream.readlines())
+            byte_stream = "".join(byte_stream.readlines())
 
-    upload_func(
-        data=byte_stream,
-        overwrite=True,
-        **upload_kwargs
-    )
+    upload_func(data=byte_stream, overwrite=True, **upload_kwargs)
 
     return file_client
 
 
 def to_any(
     byte_stream,
     uri,
     conn_type=DEFAULT_BLOB_SERVICE,
     upload_mode=DEFAULT_UPLOAD_MODE,
     verbose=1,
-    **upload_kwargs
+    **upload_kwargs,
 ):
     """
-    Funcao generica de escrita de arquivo na Azure.
+    Generic function for writing data.
 
     Args:
-        byte_stream (stream): Stream de dados a serem subidos
-        uri (url): Url a ser subida o stream de dados
-        upload_mode (str): Modo de upload.'full' (de uma vez só) ou 'chunks' (em pedaços).
-            No modo chunks, precisa explicitar o chunk_size no upload_kwargs.
-        conn_type (str): String com serviço de conexão a Azure. Pode ser blob ou gen2.
-        **upload_kwargs: Argumentos a serem passados para a upload_data/upload_blob.
-            Mais detalhes em DataLakeFileClient.upload_data ou BlobFileClient.upload_blob
+        byte_stream (stream): Data stream to be uploaded
+        uri (url): Target url to receive data stream
+        upload_mode (str): 'full' for direct upload or 'chunks' for uploading in parts.
+            If 'chunks' is set. 'chunk_size' has to be declared in 'upload_kwargs'.
+        conn_type (str): Type of connection to Azure. Can receive 'blob' or 'gen2'.
+        **upload_kwargs: Args to be used with upload_data/upload_blob.
+            See DataLakeFileClient.upload_data ou BlobFileClient/upload_blob documentation
+        for details.
     """
 
     service_client = create_blob_service(uri=uri, conn_type=conn_type)
-    container_name = uri.split('/')[3]
-    blob_name = '/'.join(uri.split('/')[4:])
+    container_name = uri.split("/")[3]
+    blob_name = "/".join(uri.split("/")[4:])
 
     if verbose > 0:
-        logger.info(f'Writing {blob_name}')
+        logger.info(f"Writing {blob_name}")
 
-    if conn_type == 'gen2':
+    if conn_type == "gen2":
         file_system_client = service_client.get_file_system_client(
             file_system=container_name
         )
         file_client = file_system_client.get_file_client(file_path=blob_name)
 
-    elif conn_type == 'blob':
+    elif conn_type == "blob":
         file_client = service_client.get_blob_client(
             container=container_name, blob=blob_name
         )
 
     try:
         file_client = upload_data(
             byte_stream=byte_stream,
             file_client=file_client,
             upload_mode=upload_mode,
-            **upload_kwargs
+            **upload_kwargs,
         )
 
     finally:
         file_client.close()
         del file_client
 
-        if conn_type == 'gen2':
+        if conn_type == "gen2":
             file_system_client.close()
             del file_system_client
 
         service_client.close()
         del service_client
 
         gc.collect()
 
 
 def read_any(uri, func, conn_type=DEFAULT_BLOB_SERVICE, **kwargs):
     """
-    Função de download genérico de arquivo na Azure
+    Generic function for reading data.
 
     Args:
-        uri (url): Url a ser subida o stream de dados
-        func: Função de leitura do arquivo
-        conn_type (str): String com serviço de conexão a Azure. Pode ser blob ou gen2.
-        **kwargs: Argumentos a serem passados para a função de leitura
+        uri (url): Url where data will be streamt from
+        func: Reading function
+        conn_type (str): Type of connection to Azure. Can receive 'blob' or 'gen2'.
+        **kwargs: Args to be passed to the Reading function
 
     Returns:
-        Output da função func
+        Output of function 'func'
     """
 
     def close_connections(*connections):
         for conn in connections:
             if conn:
                 conn.close()
                 del conn
 
     service_client = create_blob_service(uri, conn_type=conn_type)
-    container_name = uri.split('/')[3]
-    blob_name = '/'.join(uri.split('/')[4:])
+    container_name = uri.split("/")[3]
+    blob_name = "/".join(uri.split("/")[4:])
 
     byte_stream = BytesIO()
 
-    if conn_type == 'gen2':
+    if conn_type == "gen2":
         file_system_client = service_client.get_file_system_client(
             file_system=container_name
         )
         file_client = file_system_client.get_file_client(blob_name)
 
-    elif conn_type == 'blob':
+    elif conn_type == "blob":
         file_client = service_client.get_blob_client(
             container=container_name, blob=blob_name
         )
 
-    assert file_client.exists(), f'Could not find blob in {blob_name}'
+    assert file_client.exists(), f"Could not find blob in {blob_name}"
 
     try:
-        if conn_type == 'gen2':
+        if conn_type == "gen2":
             byte_stream.write(file_client.download_file().readall())
-        elif conn_type == 'blob':
+        elif conn_type == "blob":
             byte_stream.write(file_client.download_blob().readall())
 
         byte_stream.seek(0)
         df = func(byte_stream, **kwargs)
 
     except Exception as e:
-        raise Exception(f'Could not read blob in {blob_name}: {e}')
+        raise Exception(f"Could not read blob in {blob_name}: {e}")
 
     finally:
         close_connections(byte_stream, file_client, file_system_client, service_client)
         gc.collect()
 
     return df
 
 
 def to_parquet(
     df,
     uri,
     conn_type=DEFAULT_BLOB_SERVICE,
     upload_kwargs=DEFAULT_CONN_KWARGS,
     upload_mode=DEFAULT_UPLOAD_MODE,
-    **kwargs
+    **kwargs,
 ):
     """
-    Função de escrita para arquivos parquet e consequente subida a Azure.
+    Parquet writing function
 
     Args:
-        df (pd.DataFrame): DataFrame a se escrever em parquet e subir a Azure
-        uri (str): String com url a ser escrito o arquivo.
-        conn_type (str): String com serviço de conexão a Azure. Pode ser blob ou gen2.
-        upload_kwargs (dict): Argumentos a serem passados para a upload_data/upload_blob.
-            Mais detalhes em DataLakeFileClient.upload_data ou BlobFileClient.upload_blob
-        **kwargs: Argumentos a serem passados para a função de escrita em parquet.
-            Consultar df.to_parquet para mais detalhes.
+        df (pd.DataFrame): DataFrame to be uploaded in Azure
+        uri (str): Target URL for data upload
+        conn_type (str): Type of connection to Azure. Can receive 'blob' or 'gen2'.
+        upload_kwargs (dict): Args to be used with upload_data/upload_blob.
+            See DataLakeFileClient.upload_data ou BlobFileClient/upload_blob documentation
+        for details.
+        **kwargs: Args to be used with the parquet reading function.
+            See df.to_parquet for details.
     """
     byte_stream = BytesIO()
     df.to_parquet(byte_stream, use_deprecated_int96_timestamps=True, **kwargs)
-    to_any(byte_stream, uri, conn_type=conn_type, upload_mode=upload_mode, **upload_kwargs)
+    to_any(
+        byte_stream, uri, conn_type=conn_type, upload_mode=upload_mode, **upload_kwargs
+    )
 
 
 def to_excel(
     df,
     uri,
     conn_type=DEFAULT_BLOB_SERVICE,
-    mode='pandas',
+    mode="pandas",
     upload_kwargs=DEFAULT_CONN_KWARGS,
     upload_mode=DEFAULT_UPLOAD_MODE,
-    **kwargs
+    **kwargs,
 ):
     """
-    Função de escrita para arquivos excel e consequente subida a Azure.
+    Excel writing function.
 
     Args:
-        df (pd.DataFrame): DataFrame a se escrever em excel e subir a Azure
-        uri (str): String com url a ser escrito o arquivo.
-        conn_type (str): String com serviço de conexão a Azure. Pode ser blob ou gen2.
-        mode (str): Modo de escrita de excel. No momento somente suporte a 'pandas'.
-        upload_kwargs (dict): Argumentos a serem passados para a upload_data/upload_blob.
-            Mais detalhes em DataLakeFileClient.upload_data ou BlobFileClient.upload_blob
+        df (pd.DataFrame): DataFrame to be uploaded in Azure
+        uri (str): Target URL for data upload
+        conn_type (str): Type of connection to Azure. Can receive 'blob' or 'gen2'.
+        upload_kwargs (dict): Args to be used with upload_data/upload_blob.
+            See DataLakeFileClient.upload_data ou BlobFileClient/upload_blob documentation
+        for details.
         **kwargs: Argumentos a serem passados para a função de escrita em parquet.
             Consultar df.to_parquet para mais detalhes.
     """
 
     # Pyexcelerate still not supported
-    if mode == 'pyexcelerate':
-        logger.warn('to_excel method is currently not supported with pyexcelerate mode')
-        mode = 'pandas'
+    if mode == "pyexcelerate":
+        logger.warn("to_excel method is currently not supported with pyexcelerate mode")
+        mode = "pandas"
 
-    func_dict = {'pandas': pd.DataFrame.to_excel}
+    func_dict = {"pandas": pd.DataFrame.to_excel}
 
     byte_stream = BytesIO()
     func_dict[mode](df, byte_stream, **kwargs)
     to_any(
-        byte_stream,
-        uri,
-        conn_type=conn_type,
-        upload_mode=upload_mode,
-        **upload_kwargs
+        byte_stream, uri, conn_type=conn_type, upload_mode=upload_mode, **upload_kwargs
     )
 
 
 def to_csv(
     df,
     uri,
-    conn_type='gen2',
-    encoding='utf-8',
+    conn_type="gen2",
+    encoding="utf-8",
     upload_kwargs=DEFAULT_CONN_KWARGS,
     upload_mode=DEFAULT_UPLOAD_MODE,
-    **kwargs
+    **kwargs,
 ):
     """
     Função de escrita para arquivos csv e consequente subida a Azure.
 
     Args:
-        df (pd.DataFrame): DataFrame a se escrever em csv e subir a Azure
-        uri (str): String com url a ser escrito o arquivo.
-        conn_type (str): String com serviço de conexão a Azure. Pode ser blob ou gen2.
-        encoding (str): String com encoding do arquivo a ser subido.
-        upload_kwargs (dict): Argumentos a serem passados para a upload_data/upload_blob.
-            Mais detalhes em DataLakeFileClient.upload_data ou BlobFileClient.upload_blob
+        df (pd.DataFrame): DataFrame to be uploaded in Azure
+        uri (str): Target URL for data upload
+        conn_type (str): Type of connection to Azure. Can receive 'blob' or 'gen2'.
+        upload_kwargs (dict): Args to be used with upload_data/upload_blob.
+            See DataLakeFileClient.upload_data ou BlobFileClient/upload_blob documentation
+        for details.
         **kwargs: Argumentos a serem passados para a função de escrita em parquet.
             Consultar df.to_parquet para mais detalhes.
     """
     # Csv writing currently not supported in blob conn_type
-    if conn_type == 'blob':
-        logger.warn('to_csv method is currently not supported with blob conn_type')
-        conn_type = 'gen2'
+    if conn_type == "blob":
+        logger.warn("to_csv method is currently not supported with blob conn_type")
+        conn_type = "gen2"
 
     byte_stream = StringIO()
     df.to_csv(byte_stream, encoding=encoding, **kwargs)
 
     to_any(
         byte_stream,
         uri,
         encoding=encoding,
         conn_type=conn_type,
         upload_mode=upload_mode,
-        **upload_kwargs
+        **upload_kwargs,
     )
 
 
 def build_re(glob_str):
     """
-    Função que reimplementa o fnmatch.translate.
+    Function that matches a pattern for path recognition.
     Args:
-        glob_str (str): String com glob pattern.
+        glob_str (str): String with glob pattern.
     Returns:
-        str: String traduzida para regex pattern.
+        str: String translated to regex pattern.
     """
 
-    opts = re.compile('([.]|[*][*]/|[*]|[?])|(.)')
-    out = ''
-    for (pattern_match, literal_text) in opts.findall(glob_str):
-        if pattern_match == '.':
-            out += '[.]'
-        elif pattern_match == '**/':
-            out += '(?:.*/)?'
-        elif pattern_match == '*':
-            out += '[^/]*'
-        elif pattern_match == '?':
-            out += '.'
+    opts = re.compile("([.]|[*][*]/|[*]|[?])|(.)")
+    out = ""
+    for pattern_match, literal_text in opts.findall(glob_str):
+        if pattern_match == ".":
+            out += "[.]"
+        elif pattern_match == "**/":
+            out += "(?:.*/)?"
+        elif pattern_match == "*":
+            out += "[^/]*"
+        elif pattern_match == "?":
+            out += "."
         elif literal_text:
             out += literal_text
     return out
 
 
 def glob(uri, conn_kwargs=DEFAULT_GLOB_CONN_KWARGS, **kwargs):
     """
-    Função que permite, dado uma url, pegar todos os endereços de arquivos da pasta que
-    atendam aos requisitos.
+    Function that allows getting all files in a given root directory.
 
     Args:
-        uri (str): Url com padrão fnmatch de regex.
-            Já possuimos alguns recursos com suporte:
-                - * permite pegar qualquer url que possua qualquer string no lugar de *
-                - (word1|word2) permite filtrar urls que contenham as palavras word1 ou word2
-                - dentre outros
-        conn_kwargs (dict): Dicionário com argumentos de conexão a serem passados para a
-            função de get_paths
-        **kwargs (dict): Argumentos da função get_paths
+        uri (str): Url with regex pattern.
+            Supports:
+                - '*' gets any string between the last character right before it
+                and the first right after.
+                - (word1|word2) allows filtering str with either word1 or word2.
+        conn_kwargs (dict): connection args
+        **kwargs (dict): get_paths args
     Returns:
-        list: Lista com url dos diretórios que atendem ao requisito da uri
+        list: List with all files that match the given pattern and are inside root directory.
     """
 
-    blob_service = create_blob_service(uri, conn_type='gen2')
-    container_name = uri.split('/')[3]
-    container_url = '/'.join(uri.split('/')[:4])
-    blob_name = '/'.join(uri.split('/')[4:])
+    blob_service = create_blob_service(uri, conn_type="gen2")
+    container_name = uri.split("/")[3]
+    container_url = "/".join(uri.split("/")[:4])
+    blob_name = "/".join(uri.split("/")[4:])
     container_client = blob_service.get_file_system_client(file_system=container_name)
 
     # Como a get_paths exige que a path exista, nós quebramos a url em duas variaveis:
     # - path: com a parte da url que exista uma pasta
     # - path_suffix: com a query desejada dentro dessa pasta
 
-    # TODO: avaliar as sequencias de regex desse codigo
-    regex = re.compile("^(.*?[\*,\(,\[])")
-    lista = regex.split(blob_name)
+    lista = re.split("^(.*?[\*])", blob_name)
 
     if len(lista) == 1:
         path = lista[0]
-        path_suffix = ''
+        path_suffix = ""
     else:
-        new_split = '/'.join(lista[:-1]).split('/')
-        path = '/'.join(new_split[:-1])
+        new_split = "/".join(lista[:-1]).split("/")
+        path = "/".join(new_split[:-1])
         path_suffix = new_split[-1] + lista[-1]
 
     list_blobs = [
-        container_url + '/' + unit.name
+        container_url + "/" + unit.name
         for unit in container_client.get_paths(path=path, **kwargs, **conn_kwargs)
     ]
 
     result_list = []
 
     if len(list_blobs) == 0:
-        print('No file match the specified criteria')
+        print("No file match the specified criteria")
         return result_list
 
     if len(path_suffix) == 0:
         return list_blobs
 
     else:
-        path_suffix = build_re(path_suffix)  # traduz fnmatch para regex
+        path_suffix = build_re(path_suffix)
         result_list = [
             i for i in np.array(list_blobs) if re.search(path_suffix, i) is not None
         ]
 
     return result_list
 
 
-def read_parquet(uri, mode='pandas', conn_type=DEFAULT_BLOB_SERVICE, **kwargs):
-
+def read_parquet(uri, mode="pandas", conn_type=DEFAULT_BLOB_SERVICE, **kwargs):
     """
-    Função de leitura genérica de parquet
+    Generic parquet reading file.
     Args:
-        uri (str): Url do arquivo
-        conn_type (str): String com serviço de conexão a Azure. Pode ser blob ou gen2.
-        **kwargs: Argumentos extras das funções de leitura disponiveis.
+        uri (str): Target URL file
+        conn_type (str): Type of connection to Azure. Can receive 'blob' or 'gen2'.
+        **kwargs: Reader functions extra args.
     Returns:
-        pd.DataFrame: DataFrame desejado
+        pd.DataFrame
     """
-    func = {'pandas': pd.read_parquet}
+    func = {"pandas": pd.read_parquet}
     func = func[mode]
     return read_any(uri, func, conn_type=conn_type, **kwargs)
 
 
-def read_csv(uri, mode='pandas', conn_type=DEFAULT_BLOB_SERVICE, **kwargs):
-
+def read_csv(uri, mode="pandas", conn_type=DEFAULT_BLOB_SERVICE, **kwargs):
     """
-    Função de leitura genérica de csv
+    Generic csv reading file.
     Args:
-        uri (str): Url do arquivo
-        conn_type (str): String com serviço de conexão a Azure. Pode ser blob ou gen2.
-        **kwargs: Argumentos extras das funções de leitura disponiveis.
+        uri (str): Target URL file
+        conn_type (str): Type of connection to Azure. Can receive 'blob' or 'gen2'.
+        **kwargs: Reader functions extra args.
     Returns:
-        pd.DataFrame: DataFrame desejado
+        pd.DataFrame
     """
-    func = {'pandas': pd.read_csv}
+    func = {"pandas": pd.read_csv}
     func = func[mode]
     return read_any(uri, func, conn_type=conn_type, **kwargs)
 
 
-def read_excel(uri, mode='pandas', conn_type=DEFAULT_BLOB_SERVICE, **kwargs):
-
+def read_excel(uri, mode="pandas", conn_type=DEFAULT_BLOB_SERVICE, **kwargs):
     """
-    Função de leitura genérica de excel
+    Generic excel reading file.
     Args:
-        uri (str): Url do arquivo
-        mode (str): Pode ser 'pandas' para leitura padrão pelo pandas.
-        conn_type (str): String com serviço de conexão a Azure. Pode ser blob ou gen2.
-        **kwargs: Argumentos extras das funções de leitura disponiveis.
+        uri (str): Target URL file
+        conn_type (str): Type of connection to Azure. Can receive 'blob' or 'gen2'.
+        **kwargs: Reader functions extra args.
     Returns:
-        pd.DataFrame: DataFrame desejado
+        pd.DataFrame
     """
 
     # A partir de uma determinada versao, o xlrd parou de dar suporte a xlsx.
     # Usa-se por padrão a engine openpyxl. Se ela não for passada, agnt força a engine
-    if ('.xlsx' in uri) & ('engine' not in kwargs):
-        kwargs['engine'] = 'openpyxl'
+    if (".xlsx" in uri) & ("engine" not in kwargs):
+        kwargs["engine"] = "openpyxl"
 
-    func = {'pandas': pd.read_excel}
+    func = {"pandas": pd.read_excel}
     func = func[mode]
     return read_any(uri, func, conn_type=conn_type, **kwargs)
 
 
 def read_url(uri, sas_token, _format, **kwargs):
-    """Read from a container with SAS token """
+    """Read from a container with SAS token"""
     with tempfile.NamedTemporaryFile() as tf:
         url_tok = uri + sas_token
         urlretrieve(url_tok, tf.name)
         df = read_any(uri=tf.name, _format=_format, **kwargs)
         return df
 
 
 def file_exists(path):
-    """ Checa se um arquivo de Data Lake Azure existe """
-    last_dir = path.replace(path.split('/')[-1], "*")
+    """Checks if an Azure Data Lake file exists"""
+    last_dir = path.replace(path.split("/")[-1], "*")
 
     try:
         if path in glob(last_dir):
             return True
         else:
             return False
     except ResourceNotFoundError:
         return False
+
+
+def save_pickle(model, path):
+    """Save pickle files in an Azure Data Lake"""
+    with tempfile.NamedTemporaryFile() as tfile:
+        pickle.dump(model, open(tfile.name, "wb"))
+        model_file = open(tfile.name, "rb")
+        byte_stream = BytesIO()
+        byte_stream.write(model_file.read())
+        to_any(byte_stream, path)
```

### Comparing `paeio-0.0.1.3/paeio.egg-info/PKG-INFO` & `paeio-0.1/paeio.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Metadata-Version: 2.1
 Name: paeio
-Version: 0.0.1.3
+Version: 0.1
 Summary: Utilities library for read/write operations and general data cleaning routines
-Author-email: João Pedro Alves <jotapedro1997@gmail.com>, "Mauricio (Pae) Araujo" <mauricio.araujo97@gmail.com>
+Author-email: João Pedro Alves <jotapedro1997@gmail.com>
 Project-URL: Homepage, https://github.com/jotap123/paeio/tree/develop
 Project-URL: Issues, https://github.com/jotap123/paeio/issues
 Project-URL: Linkedin_JP, https://www.linkedin.com/in/jp111/
-Project-URL: Linkedin_Pae, https://www.linkedin.com/in/mauricio-arauujo/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 2 - Pre-Alpha
-Requires-Python: >=3.8
+Classifier: Development Status :: 5 - Production/Stable
+Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: azure-identity
-Requires-Dist: azure-keyvault
-Requires-Dist: azure-keyvault-secrets
 Requires-Dist: azure-storage-file-datalake
 Requires-Dist: joblib
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyarrow
 Requires-Dist: openpyxl
 Requires-Dist: python-dotenv
@@ -36,33 +33,33 @@
 
 ## Project Structure
 
 ```plaintext
 paeio
 ├── README.md
 ├── docs            -> Folder containing files for building the library.
-├── ipp_ds              -> Folder containing the library's code
+├── paeio              -> Folder containing the library's code
 │   ├── data_cleaning         -> Module for data cleaning.
 │   └── io                    -> Module for I/O operations.
 ├── dist             -> Folder containing files for package distribution
 │   ├── __init__.py
-│   └── ipp_ds-0.X-py3-none-any.whl                -> Installation with pip will be done from here.
+│   └── paeio-0.X-py3-none-any.whl               -> Installation with pip will be done from here.
 ├── tests            -> Folder containing test files for validating the package's implementations.
 ├── requirements.txt          -> Required packages to run the project
 └── pyproject.toml                  -> Setup file for generating the package installer.
 ```
 
 ## Daily Use
 
 ### Library Installation
 
 For development, it's highly recommended to create a separate environment. To do this, run:
 
 ```bash
-$ conda create -n paeio python==3.X (X >= 9)
+$ conda create -n paeio python==3.X #(X >= 7.1)
 ```
 
 For installation via pip, run the following command:
 
 ```bash
 $ pip3 install paeio
 ```
```

### Comparing `paeio-0.0.1.3/pyproject.toml` & `paeio-0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "paeio"
-version = "0.0.1.3"
+version = "0.1"
 authors = [
   { name="João Pedro Alves", email="jotapedro1997@gmail.com" },
-  { name="Mauricio (Pae) Araujo", email="mauricio.araujo97@gmail.com" }
 ]
 description = "Utilities library for read/write operations and general data cleaning routines"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.7.1"
 dynamic = ["dependencies"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
-    "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 5 - Production/Stable",
 ]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
 [project.urls]
 Homepage = "https://github.com/jotap123/paeio/tree/develop"
 Issues = "https://github.com/jotap123/paeio/issues"
 Linkedin_JP = "https://www.linkedin.com/in/jp111/"
-Linkedin_Pae = "https://www.linkedin.com/in/mauricio-arauujo/"
+
+[tool.isort]
+profile = "black"
```

