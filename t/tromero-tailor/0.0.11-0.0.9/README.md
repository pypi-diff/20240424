# Comparing `tmp/tromero_tailor-0.0.11.tar.gz` & `tmp/tromero_tailor-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tromero_tailor-0.0.11.tar", last modified: Tue Apr 23 11:05:53 2024, max compression
+gzip compressed data, was "tromero_tailor-0.0.9.tar", last modified: Thu Apr 18 10:04:22 2024, max compression
```

## Comparing `tromero_tailor-0.0.11.tar` & `tromero_tailor-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-04-23 11:05:53.804466 tromero_tailor-0.0.11/
--rw-r--r--   0 tadhgamin   (501) staff       (20)     1937 2024-04-23 11:05:53.804239 tromero_tailor-0.0.11/PKG-INFO
--rw-r--r--   0 tadhgamin   (501) staff       (20)      942 2024-04-08 16:49:32.000000 tromero_tailor-0.0.11/README.md
--rw-r--r--   0 tadhgamin   (501) staff       (20)       38 2024-04-23 11:05:53.804507 tromero_tailor-0.0.11/setup.cfg
--rw-r--r--   0 tadhgamin   (501) staff       (20)     1633 2024-04-23 11:05:48.000000 tromero_tailor-0.0.11/setup.py
-drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-04-23 11:05:53.802597 tromero_tailor-0.0.11/tests/
--rw-r--r--   0 tadhgamin   (501) staff       (20)     3672 2024-04-17 14:55:07.000000 tromero_tailor-0.0.11/tests/test.py
-drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-04-23 11:05:53.803146 tromero_tailor-0.0.11/tromero_tailor/
--rw-r--r--   0 tadhgamin   (501) staff       (20)       30 2024-04-08 15:07:54.000000 tromero_tailor-0.0.11/tromero_tailor/__init__.py
--rw-r--r--   0 tadhgamin   (501) staff       (20)     1349 2024-04-18 09:40:26.000000 tromero_tailor-0.0.11/tromero_tailor/tromero_requests.py
--rw-r--r--   0 tadhgamin   (501) staff       (20)      446 2024-04-12 11:06:15.000000 tromero_tailor-0.0.11/tromero_tailor/tromero_utils.py
--rw-r--r--   0 tadhgamin   (501) staff       (20)     2828 2024-04-23 11:05:42.000000 tromero_tailor-0.0.11/tromero_tailor/wrapper.py
-drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-04-23 11:05:53.803938 tromero_tailor-0.0.11/tromero_tailor.egg-info/
--rw-r--r--   0 tadhgamin   (501) staff       (20)     1937 2024-04-23 11:05:53.000000 tromero_tailor-0.0.11/tromero_tailor.egg-info/PKG-INFO
--rw-r--r--   0 tadhgamin   (501) staff       (20)      341 2024-04-23 11:05:53.000000 tromero_tailor-0.0.11/tromero_tailor.egg-info/SOURCES.txt
--rw-r--r--   0 tadhgamin   (501) staff       (20)        1 2024-04-23 11:05:53.000000 tromero_tailor-0.0.11/tromero_tailor.egg-info/dependency_links.txt
--rw-r--r--   0 tadhgamin   (501) staff       (20)      304 2024-04-23 11:05:53.000000 tromero_tailor-0.0.11/tromero_tailor.egg-info/requires.txt
--rw-r--r--   0 tadhgamin   (501) staff       (20)       15 2024-04-23 11:05:53.000000 tromero_tailor-0.0.11/tromero_tailor.egg-info/top_level.txt
+drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-04-18 10:04:22.426579 tromero_tailor-0.0.9/
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     1936 2024-04-18 10:04:22.426346 tromero_tailor-0.0.9/PKG-INFO
+-rw-r--r--   0 tadhgamin   (501) staff       (20)      942 2024-04-08 16:49:32.000000 tromero_tailor-0.0.9/README.md
+-rw-r--r--   0 tadhgamin   (501) staff       (20)       38 2024-04-18 10:04:22.426621 tromero_tailor-0.0.9/setup.cfg
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     1632 2024-04-18 10:04:08.000000 tromero_tailor-0.0.9/setup.py
+drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-04-18 10:04:22.423934 tromero_tailor-0.0.9/tests/
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     3672 2024-04-17 14:55:07.000000 tromero_tailor-0.0.9/tests/test.py
+drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-04-18 10:04:22.425190 tromero_tailor-0.0.9/tromero_tailor/
+-rw-r--r--   0 tadhgamin   (501) staff       (20)       30 2024-04-08 15:07:54.000000 tromero_tailor-0.0.9/tromero_tailor/__init__.py
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     1349 2024-04-18 09:40:26.000000 tromero_tailor-0.0.9/tromero_tailor/tromero_requests.py
+-rw-r--r--   0 tadhgamin   (501) staff       (20)      446 2024-04-12 11:06:15.000000 tromero_tailor-0.0.9/tromero_tailor/tromero_utils.py
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     2686 2024-04-18 10:04:02.000000 tromero_tailor-0.0.9/tromero_tailor/wrapper.py
+drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-04-18 10:04:22.426070 tromero_tailor-0.0.9/tromero_tailor.egg-info/
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     1936 2024-04-18 10:04:22.000000 tromero_tailor-0.0.9/tromero_tailor.egg-info/PKG-INFO
+-rw-r--r--   0 tadhgamin   (501) staff       (20)      341 2024-04-18 10:04:22.000000 tromero_tailor-0.0.9/tromero_tailor.egg-info/SOURCES.txt
+-rw-r--r--   0 tadhgamin   (501) staff       (20)        1 2024-04-18 10:04:22.000000 tromero_tailor-0.0.9/tromero_tailor.egg-info/dependency_links.txt
+-rw-r--r--   0 tadhgamin   (501) staff       (20)      304 2024-04-18 10:04:22.000000 tromero_tailor-0.0.9/tromero_tailor.egg-info/requires.txt
+-rw-r--r--   0 tadhgamin   (501) staff       (20)       15 2024-04-18 10:04:22.000000 tromero_tailor-0.0.9/tromero_tailor.egg-info/top_level.txt
```

### Comparing `tromero_tailor-0.0.11/PKG-INFO` & `tromero_tailor-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tromero_tailor
-Version: 0.0.11
+Version: 0.0.9
 Summary: A short description of your package
 Home-page: http://yourpackagehomepage.com
 Author: Tromero
 Author-email: tadhg.amin@tromero.ai
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tromero_tailor-0.0.11/README.md` & `tromero_tailor-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `tromero_tailor-0.0.11/setup.py` & `tromero_tailor-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="tromero_tailor",  # Replace with your package name
-    version="0.0.11",  # Replace with your package's version
+    version="0.0.9",  # Replace with your package's version
     author="Tromero",  # Replace with your name
     author_email="tadhg.amin@tromero.ai",  # Replace with your email address
     description="A short description of your package",  # Provide a short description
     long_description=open('README.md').read(),  # This will read your long description from README.md
     long_description_content_type='text/markdown',  # Indicates that the long description is in Markdown
     url="http://yourpackagehomepage.com",  # Replace with the URL to your package's homepage
     license="MIT",  # Replace with your chosen license
```

### Comparing `tromero_tailor-0.0.11/tests/test.py` & `tromero_tailor-0.0.9/tests/test.py`

 * *Files identical despite different names*

### Comparing `tromero_tailor-0.0.11/tromero_tailor/tromero_requests.py` & `tromero_tailor-0.0.9/tromero_tailor/tromero_requests.py`

 * *Files identical despite different names*

### Comparing `tromero_tailor-0.0.11/tromero_tailor/wrapper.py` & `tromero_tailor-0.0.9/tromero_tailor/wrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,38 +26,33 @@
             }
         }
     
     def _save_data(self, data):
         post_data(data, self._client.tromero_key)
 
     def check_model(self, model):
-        try:
-            models = self._client.models.list()
-        except:
-            return False
+        models = self._client.models.list()
         model_names = [m.id for m in models]
         return model in model_names
     
     def create(self, *args, **kwargs):
         input = {"model": kwargs['model'], "messages": kwargs['messages']}
-        tags = kwargs.get('tags', [])
         formatted_kwargs = {k: v for k, v in kwargs.items() if k not in ['model', 'messages']}
         if self.check_model(kwargs['model']):
             res = Completions.create(self, *args, **kwargs)  
             if hasattr(res, 'choices'):
                 usage = res.usage.model_dump()
                 for choice in res.choices:
                     formatted_choice = self._choice_to_dict(choice)
                     self._save_data({"messages": input['messages'] + [formatted_choice['message']],
                                     "model": input['model'],
                                     "kwargs": formatted_kwargs,
                                     "creation_time": str(datetime.datetime.now().isoformat()),
                                     "usage": usage,
-                                    "tags": tags
-                                    })
+                                        })
         else:
             messages = kwargs['messages']
             res = tromero_model_create(kwargs['model'], messages, self._client.tromero_key)
             # check if res has field 'generated_text'
             if 'generated_text' in res:
                 res = mock_openai_format(res['generated_text'])
         return res
@@ -74,8 +69,8 @@
 
 class TailorAI(OpenAI):
     chat: MockChat
     def __init__(self, api_key, tromero_key):
         super().__init__(api_key=api_key)
         self.current_prompt = []
         self.chat = MockChat(self)
-        self.tromero_key = tromero_key
+        self.tromero_key = tromero_key
```

### Comparing `tromero_tailor-0.0.11/tromero_tailor.egg-info/PKG-INFO` & `tromero_tailor-0.0.9/tromero_tailor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tromero_tailor
-Version: 0.0.11
+Version: 0.0.9
 Summary: A short description of your package
 Home-page: http://yourpackagehomepage.com
 Author: Tromero
 Author-email: tadhg.amin@tromero.ai
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

