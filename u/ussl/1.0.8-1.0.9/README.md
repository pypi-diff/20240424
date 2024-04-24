# Comparing `tmp/ussl-1.0.8.tar.gz` & `tmp/ussl-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ussl-1.0.8.tar", last modified: Wed Jan 24 11:20:54 2024, max compression
+gzip compressed data, was "dist\ussl-1.0.9.tar", last modified: Mon Jan 29 09:51:04 2024, max compression
```

## Comparing `ussl-1.0.8.tar` & `ussl-1.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-01-24 11:20:54.662464 ussl-1.0.8/
--rw-rw-rw-   0        0        0    15089 2024-01-24 11:20:54.655961 ussl-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    14493 2024-01-24 10:53:59.000000 ussl-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-01-24 11:20:54.662464 ussl-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1092 2024-01-24 11:20:44.000000 ussl-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-24 11:20:54.620612 ussl-1.0.8/ussl/
--rw-rw-rw-   0        0        0        0 2024-01-24 09:57:50.000000 ussl-1.0.8/ussl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-24 11:20:54.631646 ussl-1.0.8/ussl/model/
--rw-rw-rw-   0        0        0     4319 2024-01-24 09:57:50.000000 ussl-1.0.8/ussl/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-24 11:20:54.635499 ussl-1.0.8/ussl/postprocessing/
--rw-rw-rw-   0        0        0     4696 2024-01-24 09:57:50.000000 ussl-1.0.8/ussl/postprocessing/__init__.py
--rw-rw-rw-   0        0        0     6590 2024-01-24 11:01:42.000000 ussl-1.0.8/ussl/postprocessing/base.py
-drwxrwxrwx   0        0        0        0 2024-01-24 11:20:54.648302 ussl-1.0.8/ussl/protocol/
--rw-rw-rw-   0        0        0      228 2024-01-24 09:57:50.000000 ussl-1.0.8/ussl/protocol/__init__.py
--rw-rw-rw-   0        0        0      457 2024-01-24 10:53:52.000000 ussl-1.0.8/ussl/protocol/base.py
--rw-rw-rw-   0        0        0     1557 2024-01-24 10:53:52.000000 ussl-1.0.8/ussl/protocol/ldap.py
--rw-rw-rw-   0        0        0     5630 2024-01-24 10:53:52.000000 ussl-1.0.8/ussl/protocol/ssh.py
--rw-rw-rw-   0        0        0        0 2024-01-24 09:57:50.000000 ussl-1.0.8/ussl/protocol/winexe.py
--rw-rw-rw-   0        0        0     7114 2024-01-24 10:53:52.000000 ussl-1.0.8/ussl/protocol/winrm.py
--rw-rw-rw-   0        0        0        0 2024-01-24 09:57:50.000000 ussl-1.0.8/ussl/protocol/wmi.py
-drwxrwxrwx   0        0        0        0 2024-01-24 11:20:54.650036 ussl-1.0.8/ussl/transport/
--rw-rw-rw-   0        0        0     1586 2024-01-24 10:53:52.000000 ussl-1.0.8/ussl/transport/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-24 11:20:54.654160 ussl-1.0.8/ussl/utils/
--rw-rw-rw-   0        0        0     1766 2024-01-24 09:57:50.000000 ussl-1.0.8/ussl/utils/__init__.py
--rw-rw-rw-   0        0        0     1527 2024-01-24 10:53:52.000000 ussl-1.0.8/ussl/utils/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-01-24 11:20:54.630754 ussl-1.0.8/ussl.egg-info/
--rw-rw-rw-   0        0        0    15089 2024-01-24 11:20:54.000000 ussl-1.0.8/ussl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2024-01-24 11:20:54.000000 ussl-1.0.8/ussl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-24 11:20:54.000000 ussl-1.0.8/ussl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-01-24 11:20:54.000000 ussl-1.0.8/ussl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-01-24 11:20:54.000000 ussl-1.0.8/ussl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-01-29 09:51:04.771256 ussl-1.0.9/
+-rw-rw-rw-   0        0        0    15089 2024-01-29 09:51:04.768296 ussl-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    14493 2024-01-26 07:22:38.000000 ussl-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-01-29 09:51:04.771875 ussl-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1237 2024-01-29 09:50:40.000000 ussl-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-01-29 09:51:04.702059 ussl-1.0.9/ussl/
+-rw-rw-rw-   0        0        0       84 2024-01-26 14:06:25.000000 ussl-1.0.9/ussl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 09:51:04.723396 ussl-1.0.9/ussl/model/
+-rw-rw-rw-   0        0        0     4319 2024-01-24 09:57:50.000000 ussl-1.0.9/ussl/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 09:51:04.729415 ussl-1.0.9/ussl/postprocessing/
+-rw-rw-rw-   0        0        0     4696 2024-01-24 09:57:50.000000 ussl-1.0.9/ussl/postprocessing/__init__.py
+-rw-rw-rw-   0        0        0     6579 2024-01-29 09:40:32.000000 ussl-1.0.9/ussl/postprocessing/base.py
+drwxrwxrwx   0        0        0        0 2024-01-29 09:51:04.757029 ussl-1.0.9/ussl/protocol/
+-rw-rw-rw-   0        0        0      258 2024-01-29 09:28:26.000000 ussl-1.0.9/ussl/protocol/__init__.py
+-rw-rw-rw-   0        0        0      457 2024-01-26 07:22:38.000000 ussl-1.0.9/ussl/protocol/base.py
+-rw-rw-rw-   0        0        0     1520 2024-01-29 09:40:32.000000 ussl-1.0.9/ussl/protocol/ldap.py
+-rw-rw-rw-   0        0        0     5585 2024-01-29 09:40:32.000000 ussl-1.0.9/ussl/protocol/ssh.py
+-rw-rw-rw-   0        0        0        0 2024-01-24 09:57:50.000000 ussl-1.0.9/ussl/protocol/winexe.py
+-rw-rw-rw-   0        0        0     7018 2024-01-29 09:45:00.000000 ussl-1.0.9/ussl/protocol/winrm.py
+-rw-rw-rw-   0        0        0        0 2024-01-24 09:57:50.000000 ussl-1.0.9/ussl/protocol/wmi.py
+drwxrwxrwx   0        0        0        0 2024-01-29 09:51:04.759671 ussl-1.0.9/ussl/transport/
+-rw-rw-rw-   0        0        0     1529 2024-01-29 09:40:32.000000 ussl-1.0.9/ussl/transport/__init__.py
+drwxrwxrwx   0        0        0        0 2024-01-29 09:51:04.764567 ussl-1.0.9/ussl/utils/
+-rw-rw-rw-   0        0        0     1766 2024-01-24 09:57:50.000000 ussl-1.0.9/ussl/utils/__init__.py
+-rw-rw-rw-   0        0        0     2068 2024-01-29 09:40:32.000000 ussl-1.0.9/ussl/utils/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-01-29 09:51:04.719730 ussl-1.0.9/ussl.egg-info/
+-rw-rw-rw-   0        0        0    15089 2024-01-29 09:51:04.000000 ussl-1.0.9/ussl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2024-01-29 09:51:04.000000 ussl-1.0.9/ussl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-29 09:51:04.000000 ussl-1.0.9/ussl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-01-29 09:51:04.000000 ussl-1.0.9/ussl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-01-29 09:51:04.000000 ussl-1.0.9/ussl.egg-info/top_level.txt
```

### Comparing `ussl-1.0.8/PKG-INFO` & `ussl-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ussl
-Version: 1.0.8
+Version: 1.0.9
 Summary: Пакет разработчиков USSC-SOC для упрощения взаимодействия с АРМ, серверами и сетевыми устройствами
 Author: ussc soc dev team
 Author-email: iushangaraev@ussc.ru, pbikkuzhina@ussc.ru
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 Requires-Dist: pywinrm==0.4.1
```

### Comparing `ussl-1.0.8/README.md` & `ussl-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ussl-1.0.8/setup.py` & `ussl-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 setup(
     name='ussl',
     author='ussc soc dev team',
     author_email='iushangaraev@ussc.ru, pbikkuzhina@ussc.ru',
     description='Пакет разработчиков USSC-SOC для упрощения взаимодействия с АРМ, серверами и сетевыми устройствами',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.0.8',
+    version='1.0.9',
     packages=[
         'ussl',
         'ussl.model',
         'ussl.postprocessing',
         'ussl.protocol',
         'ussl.transport',
         'ussl.utils',
     ],
     install_requires=[
         'pywinrm==0.4.1',
         'paramiko==2.7.2',
         'marshmallow==3.20.2',
-        'python-ldap==3.4.0',
+        'python-ldap==3.4.0', # адаптер https://www.lfd.uci.edu/~gohlke/pythonlibs/#python-ldap есть только для этой версии библиотеки
     ],
     classifiers=[
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.8'
     ]
 )
```

### Comparing `ussl-1.0.8/ussl/model/__init__.py` & `ussl-1.0.9/ussl/model/__init__.py`

 * *Files identical despite different names*

### Comparing `ussl-1.0.8/ussl/postprocessing/__init__.py` & `ussl-1.0.9/ussl/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `ussl-1.0.8/ussl/postprocessing/base.py` & `ussl-1.0.9/ussl/postprocessing/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import json
 import warnings
 import pathlib
 from marshmallow import Schema, exceptions
-from ussl.utils.exceptions import ValidationError, SOARException
+from ..utils.exceptions import DataError, SOARException
 
 
 warnings.filterwarnings("ignore")
 
 
 class BaseFunction:
     """
@@ -29,57 +29,58 @@
         Returns:
             ``None``
         """
 
         self.inputs_model = inputs_model
         self.secrets_model = secrets_model
         self.ensure_ascii = ensure_ascii
+        self._input_json = {}
+        self._secrets = {}
 
         inputs = pathlib.Path(sys.argv[1]).read_text(encoding='utf-8')
         secrets = pathlib.Path(sys.argv[2]).read_text(encoding='utf-8')
 
         if self.inputs_model is not None:
-            self._input_json: dict = self._check_input_data(self.inputs_model, inputs, obj="входные данные")
+            self._input_json: dict = self._check_input_data(self.inputs_model, inputs, obj="Input data")
         else:
             self._input_json: dict = json.loads(inputs)
 
         if self.secrets_model is not None:
-            self._secrets: dict = self._check_input_data(self.secrets_model, secrets, obj="секреты")
+            self._secrets: dict = self._check_input_data(self.secrets_model, secrets, obj="Secrets")
         else:
             self._secrets: dict = json.loads(secrets)
 
         try:
             self.input_json = self.validate_inputs(self._input_json)
             self.secrets = self.validate_secrets(self._secrets)
-        except ValidationError as e:
+        except DataError as e:
             self.output(e.__str__(), e.return_code)
         except NotImplementedError:
             self.input_json = self._input_json
             self.secrets = self._secrets
 
         try:
             result, message = self.function()
         except SOARException as e:
             self.output(e.__str__(), e.return_code)
         else:
-            self.output(result, message)
+            self.output(message, **result)
 
     def _check_input_data(self, model: Schema, data: str, obj: str) -> dict:
         """
         Проверка входных данных
         """
         try:
             checked_data = model.loads(data)
             return checked_data
         except exceptions.ValidationError as e:
             if isinstance(e.messages, dict):
-                formatted_names = ', '.join(e.messages.keys())
-                self.output(f"Отсутствуют {obj}: {formatted_names}", 1)
+                self.output(f"{obj} validation error", 1, **{"fields": e.messages})
             else:
-                self.output(f"Ошибка валидации входных данных: {e.__str__()}", 1)
+                self.output(f"{obj} validation error: {e.__str__()}", 1)
 
     def validate_inputs(self, input_json: dict) -> dict:
         """
         Метод для дополнительной валидации входных данных.
 
         При ошибке валидации выбрасывает ValidationError
         """
@@ -121,15 +122,17 @@
 
         Returns:
             ``None``
         """
         # Обновляем входной JSON с результатом или сообщением об ошибке
         self._input_json['error' if return_code else 'result'] = message
 
-        # Обновляем входной JSON с дополнительными аргументами
+        # Обновляем входной JSON новыми аргументами
         self._input_json.update(kwargs)
 
         # Выводим входной JSON в форматированном виде
         print(json.dumps(self._input_json, ensure_ascii=self.ensure_ascii))
 
+        if self._input_json.get("result"):
+            del self._input_json["result"]
         # Завершаем выполнение скрипта с кодом 0 в случае успешного выполнения или ненулевым в случае ошибки
         exit(return_code)
```

### Comparing `ussl-1.0.8/ussl/protocol/ssh.py` & `ussl-1.0.9/ussl/protocol/ssh.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 import re
 import socket
 import time
 from paramiko import AutoAddPolicy, Channel, SSHClient, RSAKey
 from paramiko.config import SSH_PORT
 from paramiko.ssh_exception import SSHException
 
-from ussl.utils.exceptions import (
-    ProtocolConnectionError,
-    ProtocolExecutionError,
-)
+
 from ..model import Query, Response, Protocol
 from .base import BaseProtocol
+from ..utils.exceptions import ConnectionFailedError, ExecutionError
 
 
 class SSHProtocol(BaseProtocol):
     name = 'ssh'
 
     def __init__(self) -> None:
         self._chan: Channel
@@ -59,15 +57,15 @@
                     timeout=timeout,
                     look_for_keys=look_for_keys,
                     auth_timeout=auth_timeout
                 )
                 self._chan = self._client.invoke_shell(width=window_width)
                 self._clean_channel()
             except SSHException as exc:
-                raise ProtocolConnectionError(exc) from exc
+                raise ConnectionFailedError(exc.__str__())
 
         elif protocol.pem_file:
             try:
                 keyfile = io.StringIO(protocol.pem_file)
                 self._client.connect(
                     protocol.host,
                     port,
@@ -76,15 +74,15 @@
                     timeout=timeout,
                     look_for_keys=look_for_keys,
                     auth_timeout=auth_timeout
                 )
                 self._chan = self._client.invoke_shell(width=window_width)
                 self._clean_channel()
             except SSHException as exc:
-                raise ProtocolConnectionError(exc) from exc
+                raise ConnectionFailedError(exc.__str__())
 
     def close(self) -> None:
         if self._chan is not None:
             self._chan.close()
         self._client.close()
 
     def execute(
@@ -96,22 +94,22 @@
         prev_timeout = self._chan.gettimeout()
 
         if query.sudo is not None:
             try:
                 self._chan.send(f'{query.command}\n')
                 self._chan.send(f'{query.sudo}\n')
             except SSHException as exc:
-                raise ProtocolExecutionError(
+                raise ExecutionError(
                     f'An error occurred while executing the command: {query.command}\n{exc}'
                 ) from exc
         else:
             try:
                 self._chan.send(f'{query.command}\n')
             except SSHException as exc:
-                raise ProtocolExecutionError(
+                raise ExecutionError(
                     f'An error occurred while executing the command: {query.command}\n{exc}'
                 ) from exc
 
         while True:
             self._chan.settimeout(query.timeout)
             try:
                 data = data + self._chan.recv(1024)
```

### Comparing `ussl-1.0.8/ussl/protocol/winrm.py` & `ussl-1.0.9/ussl/protocol/winrm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 import re
 import ssl
 from typing import Any, Union
 
 from requests.adapters import HTTPAdapter
 from requests.exceptions import ReadTimeout
-from ussl.utils.exceptions import (
-    ProtocolConnectionError,
-    ProtocolError,
-)
 from urllib3 import ProxyManager
 from urllib3.util.ssl_ import create_urllib3_context
 from winrm.exceptions import (
     AuthenticationError,
     WinRMError,
     WinRMOperationTimeoutError,
     WinRMTransportError,
 )
 from winrm.protocol import Protocol as WmProtocol
 
 from .base import BaseProtocol
 from ..model import Response, Protocol, Query
-
+from ..utils.exceptions import ConnectionFailedError, ExecutionError, CredentialsError
 
 WINRM_PORT = 5985
 WINRM_SSL_PORT = 5986
 VALID_TRANSPORT = {'plaintext', 'ntlm'}
 
 
 class TLSv1Adapter(HTTPAdapter):
@@ -85,15 +81,15 @@
         # обойти эту проблему, для декодирования используется кодировка 866
         encoding = protocol.default('encoding', 437)
         self._decoding = protocol.default('decoding', 866)
         window_width = protocol.default('window_width', 300)
         transport = protocol.default('transport', 'ntlm')
 
         if transport not in VALID_TRANSPORT:
-            raise ProtocolConnectionError(f'{transport} protocol is not supported')
+            raise ConnectionFailedError(f'{transport} protocol is not supported')
 
         # для BasicAuth явно преобразуем 'username' и 'password' из utf8 в cp1251, т.к. requests.auth.HTTPBasicAuth
         # по умолчанию преобразует utf8 строки в latin1, при этом bytes оставляет 'как есть'.
         # https://github.com/requests/requests/pull/3673
         _username: Union[str, bytes] = f'{domain}\\{username}'
         _password: Union[str, bytes] = password
         if transport == 'plaintext':
@@ -157,23 +153,23 @@
                     status=False)
             else:
                 return Response(
                     result=std_out,
                     text=f'Команда {query.command} выполнена успешно',
                     status=True)
 
-        except (WinRMTransportError, AuthenticationError) as exc:
-            raise ProtocolConnectionError(f'Connection setup error: {exc}') from exc
+        except WinRMTransportError as exc:
+            raise ConnectionFailedError(exc.__str__())
+
+        except AuthenticationError as exc:
+            raise CredentialsError(exc.__str__())
 
         except (WinRMOperationTimeoutError, ReadTimeout):
-            raise TimeoutError(
-                f'An error occurred while executing the command: {query.command}\n'
-                'Timeout for command execution result exceeded'
-            )
+            raise ConnectionFailedError('Connection timeout')
 
         except WinRMError as exc:
-            raise ProtocolError(
+            raise ExecutionError(
                 f'An error occurred while executing the command: {query.command}\n{exc}'
             ) from exc
 
         finally:
             self._protocol.cleanup_command(self._shell_id, command_id)
```

### Comparing `ussl-1.0.8/ussl/transport/__init__.py` & `ussl-1.0.9/ussl/transport/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,50 +1,47 @@
 from typing import Union
 
 from ..protocol import (
     INTERFACES,
     base
 )
-from ..utils import exceptions
-from ..model import Protocol, Response
+from ..model import Protocol, Response, Query
+from ..utils.exceptions import ConnectionFailedError
 
 
 class Transport:
     def __init__(self) -> None:
         pass
 
     def _connect(self, protocol: Protocol):
         if not protocol.interface:
-            raise exceptions.ProtocolExecutionError('Do not specify the interface on which you want to communicate')
+            raise ConnectionFailedError('Do not specify the interface on which you want to communicate')
         if protocol.interface not in INTERFACES:
-            raise exceptions.ProtocolExecutionError('Specified interface not supported')
+            raise ConnectionFailedError('Specified interface not supported')
 
         self.proto: base.BaseProtocol = INTERFACES[protocol.interface]()
         self.proto.connect(protocol)
 
-    def _execute(self, query: Union[dict, list]) -> str:
+    def _execute(self, query: Union[Query, list]) -> Response:
         try:
             if isinstance(query, list):
                 for q in range(len(query)):
                     response: Response = self.proto.execute(query[q])
                     if response.status is False:
                         return response
             else:
                 response: Response = self.proto.execute(query)
 
             return response
         finally:
             self.proto.close()
 
-    @classmethod
     def connect(self, protocol: Protocol):
-        self._connect(self, protocol)
+        self._connect(protocol)
 
-    @classmethod
-    def execute(self, query: Union[dict, list]) -> str:
-        return self._execute(self, query)
+    def execute(self, query: Union[dict, list]) -> Response:
+        return self._execute(query)
 
-    @classmethod
-    def connect_and_execute(self, protocol: Protocol) -> str:
+    def connect_and_execute(self, protocol: Protocol) -> Response:
         query = protocol.query
-        self._connect(self, protocol)
-        return self._execute(self, query)
+        self._connect(protocol)
+        return self._execute(query)
```

### Comparing `ussl-1.0.8/ussl/utils/__init__.py` & `ussl-1.0.9/ussl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ussl-1.0.8/ussl.egg-info/PKG-INFO` & `ussl-1.0.9/ussl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ussl
-Version: 1.0.8
+Version: 1.0.9
 Summary: Пакет разработчиков USSC-SOC для упрощения взаимодействия с АРМ, серверами и сетевыми устройствами
 Author: ussc soc dev team
 Author-email: iushangaraev@ussc.ru, pbikkuzhina@ussc.ru
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 Requires-Dist: pywinrm==0.4.1
```

