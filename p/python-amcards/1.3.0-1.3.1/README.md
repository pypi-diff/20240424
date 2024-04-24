# Comparing `tmp/python_amcards-1.3.0.tar.gz` & `tmp/python_amcards-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_amcards-1.3.0.tar", last modified: Thu Apr 18 05:23:22 2024, max compression
+gzip compressed data, was "python_amcards-1.3.1.tar", last modified: Wed Apr 24 17:42:33 2024, max compression
```

## Comparing `python_amcards-1.3.0.tar` & `python_amcards-1.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 simonesestili   (501) staff       (20)        0 2024-04-18 05:23:22.586978 python_amcards-1.3.0/
--rw-r--r--   0 simonesestili   (501) staff       (20)    11357 2022-11-05 02:56:15.000000 python_amcards-1.3.0/LICENSE
--rw-r--r--   0 simonesestili   (501) staff       (20)     3076 2024-04-18 05:23:22.586663 python_amcards-1.3.0/PKG-INFO
--rw-r--r--   0 simonesestili   (501) staff       (20)     2466 2023-05-19 17:59:31.000000 python_amcards-1.3.0/README.rst
-drwxr-xr-x   0 simonesestili   (501) staff       (20)        0 2024-04-18 05:23:22.585160 python_amcards-1.3.0/amcards/
--rw-r--r--   0 simonesestili   (501) staff       (20)     5466 2024-04-18 04:14:42.000000 python_amcards-1.3.0/amcards/__helpers.py
--rw-r--r--   0 simonesestili   (501) staff       (20)       34 2022-11-05 02:56:15.000000 python_amcards-1.3.0/amcards/__init__.py
--rw-r--r--   0 simonesestili   (501) staff       (20)    61560 2024-04-18 05:21:04.000000 python_amcards-1.3.0/amcards/amcards.py
--rw-r--r--   0 simonesestili   (501) staff       (20)     1978 2024-04-18 05:21:12.000000 python_amcards-1.3.0/amcards/exceptions.py
--rw-r--r--   0 simonesestili   (501) staff       (20)    30696 2024-04-18 05:05:32.000000 python_amcards-1.3.0/amcards/models.py
-drwxr-xr-x   0 simonesestili   (501) staff       (20)        0 2024-04-18 05:23:22.586335 python_amcards-1.3.0/python_amcards.egg-info/
--rw-r--r--   0 simonesestili   (501) staff       (20)     3076 2024-04-18 05:23:22.000000 python_amcards-1.3.0/python_amcards.egg-info/PKG-INFO
--rw-r--r--   0 simonesestili   (501) staff       (20)      316 2024-04-18 05:23:22.000000 python_amcards-1.3.0/python_amcards.egg-info/SOURCES.txt
--rw-r--r--   0 simonesestili   (501) staff       (20)        1 2024-04-18 05:23:22.000000 python_amcards-1.3.0/python_amcards.egg-info/dependency_links.txt
--rw-r--r--   0 simonesestili   (501) staff       (20)       12 2024-04-18 05:23:22.000000 python_amcards-1.3.0/python_amcards.egg-info/requires.txt
--rw-r--r--   0 simonesestili   (501) staff       (20)        8 2024-04-18 05:23:22.000000 python_amcards-1.3.0/python_amcards.egg-info/top_level.txt
--rw-r--r--   0 simonesestili   (501) staff       (20)       38 2024-04-18 05:23:22.587023 python_amcards-1.3.0/setup.cfg
--rw-r--r--   0 simonesestili   (501) staff       (20)      874 2024-04-18 05:23:12.000000 python_amcards-1.3.0/setup.py
+drwxr-xr-x   0 simonesestili   (501) staff       (20)        0 2024-04-24 17:42:33.571227 python_amcards-1.3.1/
+-rw-r--r--   0 simonesestili   (501) staff       (20)    11357 2022-11-05 02:56:15.000000 python_amcards-1.3.1/LICENSE
+-rw-r--r--   0 simonesestili   (501) staff       (20)     3076 2024-04-24 17:42:33.570893 python_amcards-1.3.1/PKG-INFO
+-rw-r--r--   0 simonesestili   (501) staff       (20)     2466 2023-05-19 17:59:31.000000 python_amcards-1.3.1/README.rst
+drwxr-xr-x   0 simonesestili   (501) staff       (20)        0 2024-04-24 17:42:33.565825 python_amcards-1.3.1/amcards/
+-rw-r--r--   0 simonesestili   (501) staff       (20)     5466 2024-04-18 04:14:42.000000 python_amcards-1.3.1/amcards/__helpers.py
+-rw-r--r--   0 simonesestili   (501) staff       (20)       34 2022-11-05 02:56:15.000000 python_amcards-1.3.1/amcards/__init__.py
+-rw-r--r--   0 simonesestili   (501) staff       (20)    61560 2024-04-18 05:21:04.000000 python_amcards-1.3.1/amcards/amcards.py
+-rw-r--r--   0 simonesestili   (501) staff       (20)     1978 2024-04-18 05:21:12.000000 python_amcards-1.3.1/amcards/exceptions.py
+-rw-r--r--   0 simonesestili   (501) staff       (20)    30937 2024-04-24 17:41:58.000000 python_amcards-1.3.1/amcards/models.py
+drwxr-xr-x   0 simonesestili   (501) staff       (20)        0 2024-04-24 17:42:33.570421 python_amcards-1.3.1/python_amcards.egg-info/
+-rw-r--r--   0 simonesestili   (501) staff       (20)     3076 2024-04-24 17:42:33.000000 python_amcards-1.3.1/python_amcards.egg-info/PKG-INFO
+-rw-r--r--   0 simonesestili   (501) staff       (20)      316 2024-04-24 17:42:33.000000 python_amcards-1.3.1/python_amcards.egg-info/SOURCES.txt
+-rw-r--r--   0 simonesestili   (501) staff       (20)        1 2024-04-24 17:42:33.000000 python_amcards-1.3.1/python_amcards.egg-info/dependency_links.txt
+-rw-r--r--   0 simonesestili   (501) staff       (20)       12 2024-04-24 17:42:33.000000 python_amcards-1.3.1/python_amcards.egg-info/requires.txt
+-rw-r--r--   0 simonesestili   (501) staff       (20)        8 2024-04-24 17:42:33.000000 python_amcards-1.3.1/python_amcards.egg-info/top_level.txt
+-rw-r--r--   0 simonesestili   (501) staff       (20)       38 2024-04-24 17:42:33.571286 python_amcards-1.3.1/setup.cfg
+-rw-r--r--   0 simonesestili   (501) staff       (20)      874 2024-04-24 17:42:17.000000 python_amcards-1.3.1/setup.py
```

### Comparing `python_amcards-1.3.0/LICENSE` & `python_amcards-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_amcards-1.3.0/PKG-INFO` & `python_amcards-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-amcards
-Version: 1.3.0
+Version: 1.3.1
 Summary: A wrapper for the AMcards API.
 Home-page: https://github.com/simonesestili/python-amcards
 Author: Simone Sestili
 Author-email: simone.sestili@amcards.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `python_amcards-1.3.0/README.rst` & `python_amcards-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `python_amcards-1.3.0/amcards/__helpers.py` & `python_amcards-1.3.1/amcards/__helpers.py`

 * *Files identical despite different names*

### Comparing `python_amcards-1.3.0/amcards/amcards.py` & `python_amcards-1.3.1/amcards/amcards.py`

 * *Files identical despite different names*

### Comparing `python_amcards-1.3.0/amcards/exceptions.py` & `python_amcards-1.3.1/amcards/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_amcards-1.3.0/amcards/models.py` & `python_amcards-1.3.1/amcards/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -349,14 +349,15 @@
         is_international: bool,
         template_name: str,
         thumbnail: str,
         campaign_id: Optional[int],
         shipping_address: dict,
         return_address: dict,
         gifts: List[Gift],
+        extra_data: dict,
     ) -> None:
         self._id = id
         self._amount_charged = amount_charged
         self._status = status
         self._initiator = initiator
         self._send_date = send_date
         self._date_created = date_created
@@ -365,14 +366,15 @@
         self._is_international = is_international
         self._template_name = template_name
         self._thumbnail = thumbnail
         self._campaign_id = campaign_id
         self._shipping_address = shipping_address
         self._return_address = return_address
         self._gifts = gifts
+        self._extra_data = extra_data
 
     __repr__ = helpers.repr
 
     @property
     def id(self) -> int:
         """Card's unique identifier."""
         return self._id
@@ -485,14 +487,19 @@
         return self._return_address
 
     @property
     def gifts(self) -> List[Gift]:
         """Gifts attached to this card."""
         return self._gifts
 
+    @property
+    def extra_data(self) -> dict:
+        """Extra data attached to this card."""
+        return self._gifts
+
     @classmethod
     def _from_json(cls, json: dict):
         return cls(
             id=json['id'],
             amount_charged=int(json['amount_charged'] * 100),
             status=CardStatus(json['status']),
             initiator=json['initiator'],
@@ -508,14 +515,15 @@
             return_address=helpers.parse_return_address(json),
             gifts=[Gift(
                 name=gift['name'],
                 thumbnail='',
                 base_cost=gift['price'],
                 shipping_and_handling_cost=gift['shipping_and_handling'],
             ) for gift in json['gifts']],
+            extra_data=json.get('extra_data') or {},
         )
 
 class MailingStatus(Enum):
     """Represents the status of an AMcards mailing."""
     COMPLETE = 0
     PROCESSING = 1
```

### Comparing `python_amcards-1.3.0/python_amcards.egg-info/PKG-INFO` & `python_amcards-1.3.1/python_amcards.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-amcards
-Version: 1.3.0
+Version: 1.3.1
 Summary: A wrapper for the AMcards API.
 Home-page: https://github.com/simonesestili/python-amcards
 Author: Simone Sestili
 Author-email: simone.sestili@amcards.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `python_amcards-1.3.0/setup.py` & `python_amcards-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def README():
     with open('README.rst') as f:
         return f.read()
 
 setup(
     name='python-amcards',
-    version='1.3.0',
+    version='1.3.1',
     description='A wrapper for the AMcards API.',
     long_description=README(),
     long_description_content_type='text/x-rst',
     author='Simone Sestili',
     author_email='simone.sestili@amcards.com',
     url='https://github.com/simonesestili/python-amcards',
     packages=['amcards'],
```

