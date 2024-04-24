# Comparing `tmp/senfenico-0.1.2.tar.gz` & `tmp/senfenico-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "senfenico-0.1.2.tar", last modified: Mon Apr 22 18:38:09 2024, max compression
+gzip compressed data, was "senfenico-0.1.3.tar", last modified: Wed Apr 24 04:52:14 2024, max compression
```

## Comparing `senfenico-0.1.2.tar` & `senfenico-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 18:38:09.371061 senfenico-0.1.2/
--rw-rw-rw-   0        0        0     1189 2024-04-22 18:38:09.369552 senfenico-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      615 2024-04-22 18:36:03.000000 senfenico-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 18:38:09.339573 senfenico-0.1.2/senfenico/
--rw-rw-rw-   0        0        0      187 2024-04-19 22:01:48.000000 senfenico-0.1.2/senfenico/__init__.py
--rw-rw-rw-   0        0        0     1651 2024-04-19 21:09:01.000000 senfenico-0.1.2/senfenico/_balance.py
--rw-rw-rw-   0        0        0     6986 2024-04-19 02:44:06.000000 senfenico-0.1.2/senfenico/_charge.py
--rw-rw-rw-   0        0        0     3993 2024-04-19 00:13:52.000000 senfenico-0.1.2/senfenico/_checkout.py
--rw-rw-rw-   0        0        0     4610 2024-04-19 22:00:52.000000 senfenico-0.1.2/senfenico/_settlement.py
-drwxrwxrwx   0        0        0        0 2024-04-22 18:38:09.368555 senfenico-0.1.2/senfenico.egg-info/
--rw-rw-rw-   0        0        0     1189 2024-04-22 18:38:08.000000 senfenico-0.1.2/senfenico.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2024-04-22 18:38:08.000000 senfenico-0.1.2/senfenico.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 18:38:08.000000 senfenico-0.1.2/senfenico.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-22 18:38:08.000000 senfenico-0.1.2/senfenico.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-22 18:38:08.000000 senfenico-0.1.2/senfenico.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 18:38:09.372291 senfenico-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      925 2024-04-22 18:37:40.000000 senfenico-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 04:52:14.310872 senfenico-0.1.3/
+-rw-rw-rw-   0        0        0     1189 2024-04-24 04:52:14.265879 senfenico-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      615 2024-04-22 18:36:03.000000 senfenico-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-24 04:52:14.231202 senfenico-0.1.3/senfenico/
+-rw-rw-rw-   0        0        0      187 2024-04-19 22:01:48.000000 senfenico-0.1.3/senfenico/__init__.py
+-rw-rw-rw-   0        0        0     1541 2024-04-24 03:10:19.000000 senfenico-0.1.3/senfenico/_balance.py
+-rw-rw-rw-   0        0        0     5926 2024-04-24 03:40:26.000000 senfenico-0.1.3/senfenico/_charge.py
+-rw-rw-rw-   0        0        0     3590 2024-04-24 04:43:45.000000 senfenico-0.1.3/senfenico/_checkout.py
+-rw-rw-rw-   0        0        0     3699 2024-04-24 03:10:53.000000 senfenico-0.1.3/senfenico/_settlement.py
+-rw-rw-rw-   0        0        0     1034 2024-04-24 03:33:35.000000 senfenico-0.1.3/senfenico/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-24 04:52:14.263884 senfenico-0.1.3/senfenico.egg-info/
+-rw-rw-rw-   0        0        0     1189 2024-04-24 04:52:13.000000 senfenico-0.1.3/senfenico.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2024-04-24 04:52:13.000000 senfenico-0.1.3/senfenico.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 04:52:13.000000 senfenico-0.1.3/senfenico.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-24 04:52:13.000000 senfenico-0.1.3/senfenico.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-24 04:52:13.000000 senfenico-0.1.3/senfenico.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 04:52:14.310872 senfenico-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      900 2024-04-24 04:45:43.000000 senfenico-0.1.3/setup.py
```

### Comparing `senfenico-0.1.2/PKG-INFO` & `senfenico-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: senfenico
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python bindings for the Senfenico API
 Home-page: https://github.com/senfenico/senfenico-python
 Author: Senfenico
 Author-email: contact@senfenico.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/senfenico/senfenico-python/issues
 Project-URL: Documentation, https://docs.senfenico.com/en/
```

### Comparing `senfenico-0.1.2/README.md` & `senfenico-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `senfenico-0.1.2/senfenico/_balance.py` & `senfenico-0.1.3/senfenico/_balance.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from dataclasses import dataclass
 import requests
 from typing import List, Optional
+from senfenico.utils import SenfenicoJSONEncoder
+import json
 
 
 @dataclass
 class BalanceData:
     balance: float
     usable_balance: float
     currency: str
 
     def __str__(self):
-        return f'''{{
-            \t\t"balance": {self.balance},
-            \t\t"usable_balance": {self.usable_balance},
-            \t\t"currency": {self.currency},
-            \n\t}}'''
+        return json.dumps(self.__dict__, cls=SenfenicoJSONEncoder, indent=8)
 
     def __repr__(self):
         return self.__str__()
 
 
 @dataclass
 class SenfenicoObject:
@@ -33,15 +31,15 @@
         if isinstance(data, dict):
             data_obj = BalanceData(**data)
         else:
             data_obj = None
         return cls(status=data_dict['status'], message=data_dict['message'], errors=data_dict.get('errors'), data=data_obj)
 
     def __str__(self):
-        return f'{{\n\t"status": {self.status},\n\t"message": {self.message},\n\t"errors": {self.errors},\n\t"data": {self.data}\n}}'
+        return json.dumps(self.__dict__, cls=SenfenicoJSONEncoder, indent=4)
 
     def __repr__(self):
         return self.__str__()
 
 
 class Balance:
```

### Comparing `senfenico-0.1.2/senfenico/_checkout.py` & `senfenico-0.1.3/senfenico/_checkout.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from dataclasses import dataclass, field
 import requests
 import json
 from typing import Union, List, Optional
+from senfenico.utils import SenfenicoJSONEncoder
+import json
+
 
 @dataclass
 class CheckoutData:
     email: str
     reference: str
     charge_reference: str
     amount: int
@@ -15,26 +18,26 @@
     provider: str
     live_mode: bool
     created_at: str
     updated_at: str
     status: str
     
     def __str__(self):
-        return f'{{\n\t\t"email": {self.email},\n\t\t"reference": {self.reference},\n\t\t"charge_reference": {self.charge_reference},\n\t\t"amount": {self.amount},\n\t\t"success_url": {self.success_url},\n\t\t"cancel_url": {self.cancel_url},\n\t\t"phone": {self.phone},\n\t\t"provider": {self.provider},\n\t\t"live_mode": {self.live_mode},\n\t\t"created_at": {self.created_at},\n\t\t"updated_at": {self.status},\n\t\t"reference": {self.status}\n\t}}'
+        return json.dumps(self.__dict__, cls=SenfenicoJSONEncoder, indent=8)
 
     def __repr__(self):
         return self.__str__()
 
 @dataclass
 class CheckoutInitData:
     reference: str
     authorization_url: str
 
     def __str__(self):
-        return f'{{\n\t\t"reference": {self.reference},\n\t\t"authorization_url": {self.authorization_url}\n\t}}'
+        return json.dumps(self.__dict__, cls=SenfenicoJSONEncoder, indent=8)
 
     def __repr__(self):
         return self.__str__()
 
 
 @dataclass
 class SenfenicoObject:
@@ -56,15 +59,15 @@
         else:
             data_obj = None
         return cls(status=data_dict['status'], message=data_dict['message'], errors=data_dict.get('errors'), data=data_obj)
 
 
 
     def __str__(self):
-        return f'{{\n\t"status": {self.status},\n\t"message": {self.message},\n\t"errors": {self.errors},\n\t"data": {self.data}\n}}'
+        return json.dumps(self.__dict__, cls=SenfenicoJSONEncoder, indent=4)
 
     def __repr__(self):
         return self.__str__()
 
 
 class Checkout:
```

### Comparing `senfenico-0.1.2/senfenico.egg-info/PKG-INFO` & `senfenico-0.1.3/senfenico.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: senfenico
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python bindings for the Senfenico API
 Home-page: https://github.com/senfenico/senfenico-python
 Author: Senfenico
 Author-email: contact@senfenico.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/senfenico/senfenico-python/issues
 Project-URL: Documentation, https://docs.senfenico.com/en/
```

### Comparing `senfenico-0.1.2/setup.py` & `senfenico-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from setuptools import setup, find_packages
 import pathlib
-from codecs import open
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='senfenico',
-    version='0.1.2',
+    version='0.1.3',
 
     description="Python bindings for the Senfenico API",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     author="Senfenico",
     author_email="contact@senfenico.com",
     url="https://github.com/senfenico/senfenico-python",
```

