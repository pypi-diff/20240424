# Comparing `tmp/sitepy-0.4.0.tar.gz` & `tmp/sitepy-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitepy-0.4.0.tar", last modified: Sat Apr 20 02:33:38 2024, max compression
+gzip compressed data, was "sitepy-0.4.1.tar", last modified: Wed Apr 24 14:44:26 2024, max compression
```

## Comparing `sitepy-0.4.0.tar` & `sitepy-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 02:33:38.878552 sitepy-0.4.0/
--rw-rw-rw-   0        0        0      566 2024-04-18 20:48:30.000000 sitepy-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     1817 2024-04-20 02:33:38.877552 sitepy-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      920 2024-04-18 18:57:48.000000 sitepy-0.4.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-20 02:33:38.878552 sitepy-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1074 2024-04-20 02:33:08.000000 sitepy-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-20 02:33:38.863549 sitepy-0.4.0/sitepy/
--rw-rw-rw-   0        0        0      125 2024-04-19 00:15:25.000000 sitepy-0.4.0/sitepy/__init__.py
--rw-rw-rw-   0        0        0    12175 2024-04-20 02:22:50.000000 sitepy-0.4.0/sitepy/core.py
--rw-rw-rw-   0        0        0     1010 2024-04-18 23:46:26.000000 sitepy-0.4.0/sitepy/db.py
--rw-rw-rw-   0        0        0      236 2024-04-18 22:58:21.000000 sitepy-0.4.0/sitepy/gpt.py
--rw-rw-rw-   0        0        0      457 2024-04-20 02:11:02.000000 sitepy-0.4.0/sitepy/log.py
--rw-rw-rw-   0        0        0    28925 2024-04-18 22:58:26.000000 sitepy-0.4.0/sitepy/profanity.py
--rw-rw-rw-   0        0        0      318 2024-04-18 22:59:08.000000 sitepy-0.4.0/sitepy/recaptcha.py
-drwxrwxrwx   0        0        0        0 2024-04-20 02:33:38.874552 sitepy-0.4.0/sitepy.egg-info/
--rw-rw-rw-   0        0        0     1817 2024-04-20 02:33:38.000000 sitepy-0.4.0/sitepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2024-04-20 02:33:38.000000 sitepy-0.4.0/sitepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 02:33:38.000000 sitepy-0.4.0/sitepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-20 02:33:38.000000 sitepy-0.4.0/sitepy.egg-info/top_level.txt
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-24 14:44:26.558975 sitepy-0.4.1/
+-rw-r--r--   0 lewis-family   (501) staff       (20)      554 2024-04-24 14:29:53.000000 sitepy-0.4.1/LICENSE
+-rw-r--r--   0 lewis-family   (501) staff       (20)     2389 2024-04-24 14:44:26.558009 sitepy-0.4.1/PKG-INFO
+-rw-r--r--   0 lewis-family   (501) staff       (20)      875 2024-04-24 14:30:00.000000 sitepy-0.4.1/README.md
+-rw-r--r--   0 lewis-family   (501) staff       (20)       38 2024-04-24 14:44:26.559176 sitepy-0.4.1/setup.cfg
+-rw-r--r--   0 lewis-family   (501) staff       (20)     1057 2024-04-24 14:44:09.000000 sitepy-0.4.1/setup.py
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-24 14:44:26.554077 sitepy-0.4.1/sitepy/
+-rw-r--r--   0 lewis-family   (501) staff       (20)      103 2024-04-24 14:31:25.000000 sitepy-0.4.1/sitepy/__init__.py
+-rw-r--r--   0 lewis-family   (501) staff       (20)    11709 2024-04-24 14:30:00.000000 sitepy-0.4.1/sitepy/core.py
+-rw-r--r--   0 lewis-family   (501) staff       (20)      227 2024-04-24 14:30:00.000000 sitepy-0.4.1/sitepy/gpt.py
+-rw-r--r--   0 lewis-family   (501) staff       (20)     2631 2024-04-24 14:30:00.000000 sitepy-0.4.1/sitepy/log.py
+-rw-r--r--   0 lewis-family   (501) staff       (20)      331 2024-04-24 14:38:24.000000 sitepy-0.4.1/sitepy/profanity.py
+-rw-r--r--   0 lewis-family   (501) staff       (20)      306 2024-04-24 14:30:00.000000 sitepy-0.4.1/sitepy/recaptcha.py
+-rw-r--r--   0 lewis-family   (501) staff       (20)    26817 2024-04-24 14:37:08.000000 sitepy-0.4.1/sitepy/word_list.py
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-24 14:44:26.557401 sitepy-0.4.1/sitepy.egg-info/
+-rw-r--r--   0 lewis-family   (501) staff       (20)     2389 2024-04-24 14:44:26.000000 sitepy-0.4.1/sitepy.egg-info/PKG-INFO
+-rw-r--r--   0 lewis-family   (501) staff       (20)      268 2024-04-24 14:44:26.000000 sitepy-0.4.1/sitepy.egg-info/SOURCES.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-04-24 14:44:26.000000 sitepy-0.4.1/sitepy.egg-info/dependency_links.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)        7 2024-04-24 14:44:26.000000 sitepy-0.4.1/sitepy.egg-info/top_level.txt
```

### Comparing `sitepy-0.4.0/PKG-INFO` & `sitepy-0.4.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,80 @@
-Metadata-Version: 2.1
-Name: sitepy
-Version: 0.4.0
-Summary: A simple web framework.
-Home-page: https://github.com/WolfTheDeveloper/sitepy
-Author: WolfTheDev
-Author-email: wolfthedev@gmail.com
-License: Apache 2.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# sitepy
-
-A simple web framework for Python.
-
-## Installation
-
-You can install sitepy with pip:
-
-```sh
-pip install sitepy
-```
-
-## Usage
-
-Here's a basic example of a sitepy application:
-
-```python
-from sitepy import sitepy
-
-app = sitepy()
-
-@app.route("/", methods=['GET', 'POST'])
-def index():
-    return "Hello, world!"
-
-if __name__ == "__main__":
-    app.run()
-```
-
-This will start a server on localhost:8080 and respond with "Hello, world!" to GET and POST requests at the root URL.
-
-## Features
-
-- Simple routing: Use the @app.route decorator to define routes.
-
-- Middleware support: Use app.use to add middleware functions.
-
-- Static file serving: Files in the static directory are served at /static.
-
-## Contributing
-
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-
-## License
-[Apache](sitepy/LICENSE)
+Metadata-Version: 2.1
+Name: sitepy
+Version: 0.4.1
+Summary: A simple web framework.
+Home-page: https://github.com/WolfTheDeveloper/sitepy
+Author: WolfTheDev
+Author-email: wolfthedev@gmail.com
+License: Copyright [2024] [WolfTheDev]
+        
+        Licensed under the Apache License, Version 2.0 (the "License");
+        you may not use this file except in compliance with the License.
+        You may obtain a copy of the License at
+        
+            http://www.apache.org/licenses/LICENSE-2.0
+        
+        Unless required by applicable law or agreed to in writing, software
+        distributed under the License is distributed on an "AS IS" BASIS,
+        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+        See the License for the specific language governing permissions and
+        limitations under the License.
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# sitepy
+
+A simple web framework for Python.
+
+## Installation
+
+You can install sitepy with pip:
+
+```sh
+pip install sitepy
+```
+
+## Usage
+
+Here's a basic example of a sitepy application:
+
+```python
+from sitepy import sitepy
+
+app = sitepy()
+
+@app.route("/", methods=['GET', 'POST'])
+def index():
+    return "Hello, world!"
+
+if __name__ == "__main__":
+    app.run()
+```
+
+This will start a server on localhost:8080 and respond with "Hello, world!" to GET and POST requests at the root URL.
+
+## Features
+
+- Simple routing: Use the @app.route decorator to define routes.
+
+- Middleware support: Use app.use to add middleware functions.
+
+- Static file serving: Files in the static directory are served at /static.
+
+## Contributing
+
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+## License
+[Apache](sitepy/LICENSE)
```

### Comparing `sitepy-0.4.0/README.md` & `sitepy-0.4.1/README.md`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-# sitepy
-
-A simple web framework for Python.
-
-## Installation
-
-You can install sitepy with pip:
-
-```sh
-pip install sitepy
-```
-
-## Usage
-
-Here's a basic example of a sitepy application:
-
-```python
-from sitepy import sitepy
-
-app = sitepy()
-
-@app.route("/", methods=['GET', 'POST'])
-def index():
-    return "Hello, world!"
-
-if __name__ == "__main__":
-    app.run()
-```
-
-This will start a server on localhost:8080 and respond with "Hello, world!" to GET and POST requests at the root URL.
-
-## Features
-
-- Simple routing: Use the @app.route decorator to define routes.
-
-- Middleware support: Use app.use to add middleware functions.
-
-- Static file serving: Files in the static directory are served at /static.
-
-## Contributing
-
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-
-## License
-[Apache](sitepy/LICENSE)
+# sitepy
+
+A simple web framework for Python.
+
+## Installation
+
+You can install sitepy with pip:
+
+```sh
+pip install sitepy
+```
+
+## Usage
+
+Here's a basic example of a sitepy application:
+
+```python
+from sitepy import sitepy
+
+app = sitepy()
+
+@app.route("/", methods=['GET', 'POST'])
+def index():
+    return "Hello, world!"
+
+if __name__ == "__main__":
+    app.run()
+```
+
+This will start a server on localhost:8080 and respond with "Hello, world!" to GET and POST requests at the root URL.
+
+## Features
+
+- Simple routing: Use the @app.route decorator to define routes.
+
+- Middleware support: Use app.use to add middleware functions.
+
+- Static file serving: Files in the static directory are served at /static.
+
+## Contributing
+
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+## License
+[Apache](sitepy/LICENSE)
```

### Comparing `sitepy-0.4.0/setup.py` & `sitepy-0.4.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from setuptools import setup, find_packages
-
-setup(
-    name='sitepy',
-    version='0.4.0',
-    description='A simple web framework.',
-    author='WolfTheDev',
-    author_email='wolfthedev@gmail.com',
-    url='https://github.com/WolfTheDeveloper/sitepy',
-    license='Apache 2.0',
-    packages=find_packages(),
-    long_description=open('README.md').read(),
-    long_description_content_type='text/markdown',  # Add this line
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: Apache Software License',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3.12',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-    ],
-    python_requires='>=3.6',
+from setuptools import setup, find_packages
+
+setup(
+    name='sitepy',
+    version='0.4.1',
+    description='A simple web framework.',
+    author='WolfTheDev',
+    author_email='wolfthedev@gmail.com',
+    url='https://github.com/WolfTheDeveloper/sitepy',
+    license=open('LICENSE').read(),
+    packages=find_packages(),
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',  # Add this line
+    classifiers=[
+        'Development Status :: 3 - Alpha',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: Apache Software License',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
+        'Topic :: Software Development :: Libraries :: Python Modules',
+    ],
+    python_requires='>=3.6',
 )
```

### Comparing `sitepy-0.4.0/sitepy/core.py` & `sitepy-0.4.1/sitepy/core.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,761 +1,732 @@
-00000000: 696d 706f 7274 206f 730d 0a66 726f 6d20  import os..from 
-00000010: 7572 6c6c 6962 2e70 6172 7365 2069 6d70  urllib.parse imp
-00000020: 6f72 7420 7061 7273 655f 7173 0d0a 6672  ort parse_qs..fr
-00000030: 6f6d 2077 7367 6972 6566 2e73 696d 706c  om wsgiref.simpl
-00000040: 655f 7365 7276 6572 2069 6d70 6f72 7420  e_server import 
-00000050: 6d61 6b65 5f73 6572 7665 720d 0a69 6d70  make_server..imp
-00000060: 6f72 7420 696e 7370 6563 740d 0a66 726f  ort inspect..fro
-00000070: 6d20 6a69 6e6a 6132 2069 6d70 6f72 7420  m jinja2 import 
-00000080: 456e 7669 726f 6e6d 656e 742c 2046 696c  Environment, Fil
-00000090: 6553 7973 7465 6d4c 6f61 6465 720d 0a0d  eSystemLoader...
-000000a0: 0a66 6f66 203d 2022 2222 0d0a 3c21 444f  .fof = """..<!DO
-000000b0: 4354 5950 4520 6874 6d6c 3e0d 0a3c 6874  CTYPE html>..<ht
-000000c0: 6d6c 206c 616e 673d 2265 6e22 3e0d 0a0d  ml lang="en">...
-000000d0: 0a3c 6865 6164 3e0d 0a20 2020 203c 6d65  .<head>..    <me
-000000e0: 7461 2063 6861 7273 6574 3d22 5554 462d  ta charset="UTF-
-000000f0: 3822 3e0d 0a20 2020 203c 6d65 7461 206e  8">..    <meta n
-00000100: 616d 653d 2276 6965 7770 6f72 7422 2063  ame="viewport" c
-00000110: 6f6e 7465 6e74 3d22 7769 6474 683d 6465  ontent="width=de
-00000120: 7669 6365 2d77 6964 7468 2c20 696e 6974  vice-width, init
-00000130: 6961 6c2d 7363 616c 653d 312e 3022 3e0d  ial-scale=1.0">.
-00000140: 0a20 2020 203c 7469 746c 653e 446f 6375  .    <title>Docu
-00000150: 6d65 6e74 3c2f 7469 746c 653e 0d0a 2020  ment</title>..  
-00000160: 2020 3c73 7479 6c65 3e0d 0a20 2020 2020    <style>..     
-00000170: 2020 2040 696d 706f 7274 2027 6874 7470     @import 'http
-00000180: 733a 2f2f 666f 6e74 732e 676f 6f67 6c65  s://fonts.google
-00000190: 6170 6973 2e63 6f6d 2f63 7373 3f66 616d  apis.com/css?fam
-000001a0: 696c 793d 496e 636f 6e73 6f6c 6174 6127  ily=Inconsolata'
-000001b0: 3b0d 0a0d 0a20 2020 2020 2020 2068 746d  ;....        htm
-000001c0: 6c20 7b0d 0a20 2020 2020 2020 2020 2020  l {..           
-000001d0: 206d 696e 2d68 6569 6768 743a 2031 3030   min-height: 100
-000001e0: 253b 0d0a 2020 2020 2020 2020 7d0d 0a0d  %;..        }...
-000001f0: 0a20 2020 2020 2020 2062 6f64 7920 7b0d  .        body {.
-00000200: 0a20 2020 2020 2020 2020 2020 2062 6f78  .            box
-00000210: 2d73 697a 696e 673a 2062 6f72 6465 722d  -sizing: border-
-00000220: 626f 783b 0d0a 2020 2020 2020 2020 2020  box;..          
-00000230: 2020 6865 6967 6874 3a20 3130 3025 3b0d    height: 100%;.
-00000240: 0a20 2020 2020 2020 2020 2020 2062 6163  .            bac
-00000250: 6b67 726f 756e 642d 636f 6c6f 723a 2023  kground-color: #
-00000260: 3030 3030 3030 3b0d 0a20 2020 2020 2020  000000;..       
-00000270: 2020 2020 2062 6163 6b67 726f 756e 642d       background-
-00000280: 696d 6167 653a 2072 6164 6961 6c2d 6772  image: radial-gr
-00000290: 6164 6965 6e74 2823 3131 3538 3145 2c20  adient(#11581E, 
-000002a0: 2330 3431 3630 3729 2c20 7572 6c28 2268  #041607), url("h
-000002b0: 7474 7073 3a2f 2f6d 6564 6961 2e67 6970  ttps://media.gip
-000002c0: 6879 2e63 6f6d 2f6d 6564 6961 2f6f 4549  hy.com/media/oEI
-000002d0: 3975 4259 537a 4c70 424b 2f67 6970 6879  9uBYSzLpBK/giphy
-000002e0: 2e67 6966 2229 3b0d 0a20 2020 2020 2020  .gif");..       
-000002f0: 2020 2020 2062 6163 6b67 726f 756e 642d       background-
-00000300: 7265 7065 6174 3a20 6e6f 2d72 6570 6561  repeat: no-repea
-00000310: 743b 0d0a 2020 2020 2020 2020 2020 2020  t;..            
-00000320: 6261 636b 6772 6f75 6e64 2d73 697a 653a  background-size:
-00000330: 2063 6f76 6572 3b0d 0a20 2020 2020 2020   cover;..       
-00000340: 2020 2020 2066 6f6e 742d 6661 6d69 6c79       font-family
-00000350: 3a20 2749 6e63 6f6e 736f 6c61 7461 272c  : 'Inconsolata',
-00000360: 2048 656c 7665 7469 6361 2c20 7361 6e73   Helvetica, sans
-00000370: 2d73 6572 6966 3b0d 0a20 2020 2020 2020  -serif;..       
-00000380: 2020 2020 2066 6f6e 742d 7369 7a65 3a20       font-size: 
-00000390: 312e 3572 656d 3b0d 0a20 2020 2020 2020  1.5rem;..       
-000003a0: 2020 2020 2063 6f6c 6f72 3a20 7267 6261       color: rgba
-000003b0: 2831 3238 2c20 3235 352c 2031 3238 2c20  (128, 255, 128, 
-000003c0: 302e 3829 3b0d 0a20 2020 2020 2020 2020  0.8);..         
-000003d0: 2020 2074 6578 742d 7368 6164 6f77 3a0d     text-shadow:.
-000003e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000003f0: 2030 2030 2031 6578 2072 6762 6128 3531   0 0 1ex rgba(51
-00000400: 2c20 3235 352c 2035 312c 2031 292c 0d0a  , 255, 51, 1),..
-00000410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000420: 3020 3020 3270 7820 7267 6261 2832 3535  0 0 2px rgba(255
-00000430: 2c20 3235 352c 2032 3535 2c20 302e 3829  , 255, 255, 0.8)
-00000440: 3b0d 0a20 2020 2020 2020 207d 0d0a 0d0a  ;..        }....
-00000450: 2020 2020 2020 2020 2e6e 6f69 7365 207b          .noise {
-00000460: 0d0a 2020 2020 2020 2020 2020 2020 706f  ..            po
-00000470: 696e 7465 722d 6576 656e 7473 3a20 6e6f  inter-events: no
-00000480: 6e65 3b0d 0a20 2020 2020 2020 2020 2020  ne;..           
-00000490: 2070 6f73 6974 696f 6e3a 2061 6273 6f6c   position: absol
-000004a0: 7574 653b 0d0a 2020 2020 2020 2020 2020  ute;..          
-000004b0: 2020 7769 6474 683a 2031 3030 253b 0d0a    width: 100%;..
-000004c0: 2020 2020 2020 2020 2020 2020 6865 6967              heig
-000004d0: 6874 3a20 3130 3025 3b0d 0a20 2020 2020  ht: 100%;..     
-000004e0: 2020 2020 2020 2062 6163 6b67 726f 756e         backgroun
-000004f0: 642d 696d 6167 653a 2075 726c 2822 6874  d-image: url("ht
-00000500: 7470 733a 2f2f 6d65 6469 612e 6769 7068  tps://media.giph
-00000510: 792e 636f 6d2f 6d65 6469 612f 6f45 4939  y.com/media/oEI9
-00000520: 7542 5953 7a4c 7042 4b2f 6769 7068 792e  uBYSzLpBK/giphy.
-00000530: 6769 6622 293b 0d0a 2020 2020 2020 2020  gif");..        
-00000540: 2020 2020 6261 636b 6772 6f75 6e64 2d72      background-r
-00000550: 6570 6561 743a 206e 6f2d 7265 7065 6174  epeat: no-repeat
-00000560: 3b0d 0a20 2020 2020 2020 2020 2020 2062  ;..            b
-00000570: 6163 6b67 726f 756e 642d 7369 7a65 3a20  ackground-size: 
-00000580: 636f 7665 723b 0d0a 2020 2020 2020 2020  cover;..        
-00000590: 2020 2020 7a2d 696e 6465 783a 202d 313b      z-index: -1;
-000005a0: 0d0a 2020 2020 2020 2020 2020 2020 6f70  ..            op
-000005b0: 6163 6974 793a 202e 3032 3b0d 0a20 2020  acity: .02;..   
-000005c0: 2020 2020 207d 0d0a 0d0a 2020 2020 2020       }....      
-000005d0: 2020 2e6f 7665 726c 6179 207b 0d0a 2020    .overlay {..  
-000005e0: 2020 2020 2020 2020 2020 706f 696e 7465            pointe
-000005f0: 722d 6576 656e 7473 3a20 6e6f 6e65 3b0d  r-events: none;.
-00000600: 0a20 2020 2020 2020 2020 2020 2070 6f73  .            pos
-00000610: 6974 696f 6e3a 2061 6273 6f6c 7574 653b  ition: absolute;
-00000620: 0d0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
-00000630: 6474 683a 2031 3030 253b 0d0a 2020 2020  dth: 100%;..    
-00000640: 2020 2020 2020 2020 6865 6967 6874 3a20          height: 
-00000650: 3130 3025 3b0d 0a20 2020 2020 2020 2020  100%;..         
-00000660: 2020 2062 6163 6b67 726f 756e 643a 0d0a     background:..
+00000000: 696d 706f 7274 206f 730a 6672 6f6d 2075  import os.from u
+00000010: 726c 6c69 622e 7061 7273 6520 696d 706f  rllib.parse impo
+00000020: 7274 2070 6172 7365 5f71 730a 6672 6f6d  rt parse_qs.from
+00000030: 2077 7367 6972 6566 2e73 696d 706c 655f   wsgiref.simple_
+00000040: 7365 7276 6572 2069 6d70 6f72 7420 6d61  server import ma
+00000050: 6b65 5f73 6572 7665 720a 696d 706f 7274  ke_server.import
+00000060: 2069 6e73 7065 6374 0a66 726f 6d20 6a69   inspect.from ji
+00000070: 6e6a 6132 2069 6d70 6f72 7420 456e 7669  nja2 import Envi
+00000080: 726f 6e6d 656e 742c 2046 696c 6553 7973  ronment, FileSys
+00000090: 7465 6d4c 6f61 6465 720a 0a66 6f66 203d  temLoader..fof =
+000000a0: 2022 2222 0a3c 2144 4f43 5459 5045 2068   """.<!DOCTYPE h
+000000b0: 746d 6c3e 0a3c 6874 6d6c 206c 616e 673d  tml>.<html lang=
+000000c0: 2265 6e22 3e0a 0a3c 6865 6164 3e0a 2020  "en">..<head>.  
+000000d0: 2020 3c6d 6574 6120 6368 6172 7365 743d    <meta charset=
+000000e0: 2255 5446 2d38 223e 0a20 2020 203c 6d65  "UTF-8">.    <me
+000000f0: 7461 206e 616d 653d 2276 6965 7770 6f72  ta name="viewpor
+00000100: 7422 2063 6f6e 7465 6e74 3d22 7769 6474  t" content="widt
+00000110: 683d 6465 7669 6365 2d77 6964 7468 2c20  h=device-width, 
+00000120: 696e 6974 6961 6c2d 7363 616c 653d 312e  initial-scale=1.
+00000130: 3022 3e0a 2020 2020 3c74 6974 6c65 3e44  0">.    <title>D
+00000140: 6f63 756d 656e 743c 2f74 6974 6c65 3e0a  ocument</title>.
+00000150: 2020 2020 3c73 7479 6c65 3e0a 2020 2020      <style>.    
+00000160: 2020 2020 4069 6d70 6f72 7420 2768 7474      @import 'htt
+00000170: 7073 3a2f 2f66 6f6e 7473 2e67 6f6f 676c  ps://fonts.googl
+00000180: 6561 7069 732e 636f 6d2f 6373 733f 6661  eapis.com/css?fa
+00000190: 6d69 6c79 3d49 6e63 6f6e 736f 6c61 7461  mily=Inconsolata
+000001a0: 273b 0a0a 2020 2020 2020 2020 6874 6d6c  ';..        html
+000001b0: 207b 0a20 2020 2020 2020 2020 2020 206d   {.            m
+000001c0: 696e 2d68 6569 6768 743a 2031 3030 253b  in-height: 100%;
+000001d0: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
+000001e0: 2020 2020 626f 6479 207b 0a20 2020 2020      body {.     
+000001f0: 2020 2020 2020 2062 6f78 2d73 697a 696e         box-sizin
+00000200: 673a 2062 6f72 6465 722d 626f 783b 0a20  g: border-box;. 
+00000210: 2020 2020 2020 2020 2020 2068 6569 6768             heigh
+00000220: 743a 2031 3030 253b 0a20 2020 2020 2020  t: 100%;.       
+00000230: 2020 2020 2062 6163 6b67 726f 756e 642d       background-
+00000240: 636f 6c6f 723a 2023 3030 3030 3030 3b0a  color: #000000;.
+00000250: 2020 2020 2020 2020 2020 2020 6261 636b              back
+00000260: 6772 6f75 6e64 2d69 6d61 6765 3a20 7261  ground-image: ra
+00000270: 6469 616c 2d67 7261 6469 656e 7428 2331  dial-gradient(#1
+00000280: 3135 3831 452c 2023 3034 3136 3037 292c  1581E, #041607),
+00000290: 2075 726c 2822 6874 7470 733a 2f2f 6d65   url("https://me
+000002a0: 6469 612e 6769 7068 792e 636f 6d2f 6d65  dia.giphy.com/me
+000002b0: 6469 612f 6f45 4939 7542 5953 7a4c 7042  dia/oEI9uBYSzLpB
+000002c0: 4b2f 6769 7068 792e 6769 6622 293b 0a20  K/giphy.gif");. 
+000002d0: 2020 2020 2020 2020 2020 2062 6163 6b67             backg
+000002e0: 726f 756e 642d 7265 7065 6174 3a20 6e6f  round-repeat: no
+000002f0: 2d72 6570 6561 743b 0a20 2020 2020 2020  -repeat;.       
+00000300: 2020 2020 2062 6163 6b67 726f 756e 642d       background-
+00000310: 7369 7a65 3a20 636f 7665 723b 0a20 2020  size: cover;.   
+00000320: 2020 2020 2020 2020 2066 6f6e 742d 6661           font-fa
+00000330: 6d69 6c79 3a20 2749 6e63 6f6e 736f 6c61  mily: 'Inconsola
+00000340: 7461 272c 2048 656c 7665 7469 6361 2c20  ta', Helvetica, 
+00000350: 7361 6e73 2d73 6572 6966 3b0a 2020 2020  sans-serif;.    
+00000360: 2020 2020 2020 2020 666f 6e74 2d73 697a          font-siz
+00000370: 653a 2031 2e35 7265 6d3b 0a20 2020 2020  e: 1.5rem;.     
+00000380: 2020 2020 2020 2063 6f6c 6f72 3a20 7267         color: rg
+00000390: 6261 2831 3238 2c20 3235 352c 2031 3238  ba(128, 255, 128
+000003a0: 2c20 302e 3829 3b0a 2020 2020 2020 2020  , 0.8);.        
+000003b0: 2020 2020 7465 7874 2d73 6861 646f 773a      text-shadow:
+000003c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000003d0: 2030 2030 2031 6578 2072 6762 6128 3531   0 0 1ex rgba(51
+000003e0: 2c20 3235 352c 2035 312c 2031 292c 0a20  , 255, 51, 1),. 
+000003f0: 2020 2020 2020 2020 2020 2020 2020 2030                 0
+00000400: 2030 2032 7078 2072 6762 6128 3235 352c   0 2px rgba(255,
+00000410: 2032 3535 2c20 3235 352c 2030 2e38 293b   255, 255, 0.8);
+00000420: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
+00000430: 2020 2020 2e6e 6f69 7365 207b 0a20 2020      .noise {.   
+00000440: 2020 2020 2020 2020 2070 6f69 6e74 6572           pointer
+00000450: 2d65 7665 6e74 733a 206e 6f6e 653b 0a20  -events: none;. 
+00000460: 2020 2020 2020 2020 2020 2070 6f73 6974             posit
+00000470: 696f 6e3a 2061 6273 6f6c 7574 653b 0a20  ion: absolute;. 
+00000480: 2020 2020 2020 2020 2020 2077 6964 7468             width
+00000490: 3a20 3130 3025 3b0a 2020 2020 2020 2020  : 100%;.        
+000004a0: 2020 2020 6865 6967 6874 3a20 3130 3025      height: 100%
+000004b0: 3b0a 2020 2020 2020 2020 2020 2020 6261  ;.            ba
+000004c0: 636b 6772 6f75 6e64 2d69 6d61 6765 3a20  ckground-image: 
+000004d0: 7572 6c28 2268 7474 7073 3a2f 2f6d 6564  url("https://med
+000004e0: 6961 2e67 6970 6879 2e63 6f6d 2f6d 6564  ia.giphy.com/med
+000004f0: 6961 2f6f 4549 3975 4259 537a 4c70 424b  ia/oEI9uBYSzLpBK
+00000500: 2f67 6970 6879 2e67 6966 2229 3b0a 2020  /giphy.gif");.  
+00000510: 2020 2020 2020 2020 2020 6261 636b 6772            backgr
+00000520: 6f75 6e64 2d72 6570 6561 743a 206e 6f2d  ound-repeat: no-
+00000530: 7265 7065 6174 3b0a 2020 2020 2020 2020  repeat;.        
+00000540: 2020 2020 6261 636b 6772 6f75 6e64 2d73      background-s
+00000550: 697a 653a 2063 6f76 6572 3b0a 2020 2020  ize: cover;.    
+00000560: 2020 2020 2020 2020 7a2d 696e 6465 783a          z-index:
+00000570: 202d 313b 0a20 2020 2020 2020 2020 2020   -1;.           
+00000580: 206f 7061 6369 7479 3a20 2e30 323b 0a20   opacity: .02;. 
+00000590: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
+000005a0: 2020 2e6f 7665 726c 6179 207b 0a20 2020    .overlay {.   
+000005b0: 2020 2020 2020 2020 2070 6f69 6e74 6572           pointer
+000005c0: 2d65 7665 6e74 733a 206e 6f6e 653b 0a20  -events: none;. 
+000005d0: 2020 2020 2020 2020 2020 2070 6f73 6974             posit
+000005e0: 696f 6e3a 2061 6273 6f6c 7574 653b 0a20  ion: absolute;. 
+000005f0: 2020 2020 2020 2020 2020 2077 6964 7468             width
+00000600: 3a20 3130 3025 3b0a 2020 2020 2020 2020  : 100%;.        
+00000610: 2020 2020 6865 6967 6874 3a20 3130 3025      height: 100%
+00000620: 3b0a 2020 2020 2020 2020 2020 2020 6261  ;.            ba
+00000630: 636b 6772 6f75 6e64 3a0a 2020 2020 2020  ckground:.      
+00000640: 2020 2020 2020 2020 2020 7265 7065 6174            repeat
+00000650: 696e 672d 6c69 6e65 6172 2d67 7261 6469  ing-linear-gradi
+00000660: 656e 7428 3138 3064 6567 2c0a 2020 2020  ent(180deg,.    
 00000670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000680: 7265 7065 6174 696e 672d 6c69 6e65 6172  repeating-linear
-00000690: 2d67 7261 6469 656e 7428 3138 3064 6567  -gradient(180deg
-000006a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000006b0: 2020 2020 2020 2072 6762 6128 302c 2030         rgba(0, 0
-000006c0: 2c20 302c 2030 2920 302c 0d0a 2020 2020  , 0, 0) 0,..    
-000006d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006e0: 7267 6261 2830 2c20 302c 2030 2c20 302e  rgba(0, 0, 0, 0.
-000006f0: 3329 2035 3025 2c0d 0a20 2020 2020 2020  3) 50%,..       
-00000700: 2020 2020 2020 2020 2020 2020 2072 6762               rgb
-00000710: 6128 302c 2030 2c20 302c 2030 2920 3130  a(0, 0, 0, 0) 10
-00000720: 3025 293b 0d0a 2020 2020 2020 2020 2020  0%);..          
-00000730: 2020 6261 636b 6772 6f75 6e64 2d73 697a    background-siz
-00000740: 653a 2061 7574 6f20 3470 783b 0d0a 2020  e: auto 4px;..  
-00000750: 2020 2020 2020 2020 2020 7a2d 696e 6465            z-inde
-00000760: 783a 2031 3b0d 0a20 2020 2020 2020 207d  x: 1;..        }
-00000770: 0d0a 0d0a 2020 2020 2020 2020 2e6f 7665  ....        .ove
-00000780: 726c 6179 3a3a 6265 666f 7265 207b 0d0a  rlay::before {..
-00000790: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-000007a0: 656e 743a 2022 223b 0d0a 2020 2020 2020  ent: "";..      
-000007b0: 2020 2020 2020 706f 696e 7465 722d 6576        pointer-ev
-000007c0: 656e 7473 3a20 6e6f 6e65 3b0d 0a20 2020  ents: none;..   
-000007d0: 2020 2020 2020 2020 2070 6f73 6974 696f           positio
-000007e0: 6e3a 2061 6273 6f6c 7574 653b 0d0a 2020  n: absolute;..  
-000007f0: 2020 2020 2020 2020 2020 6469 7370 6c61            displa
-00000800: 793a 2062 6c6f 636b 3b0d 0a20 2020 2020  y: block;..     
-00000810: 2020 2020 2020 2074 6f70 3a20 303b 0d0a         top: 0;..
-00000820: 2020 2020 2020 2020 2020 2020 6c65 6674              left
-00000830: 3a20 303b 0d0a 2020 2020 2020 2020 2020  : 0;..          
-00000840: 2020 7269 6768 743a 2030 3b0d 0a20 2020    right: 0;..   
-00000850: 2020 2020 2020 2020 2062 6f74 746f 6d3a           bottom:
-00000860: 2030 3b0d 0a20 2020 2020 2020 2020 2020   0;..           
-00000870: 2077 6964 7468 3a20 3130 3025 3b0d 0a20   width: 100%;.. 
-00000880: 2020 2020 2020 2020 2020 2068 6569 6768             heigh
-00000890: 743a 2031 3030 253b 0d0a 2020 2020 2020  t: 100%;..      
-000008a0: 2020 2020 2020 6261 636b 6772 6f75 6e64        background
-000008b0: 2d69 6d61 6765 3a20 6c69 6e65 6172 2d67  -image: linear-g
-000008c0: 7261 6469 656e 7428 3064 6567 2c0d 0a20  radient(0deg,.. 
-000008d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008e0: 2020 2074 7261 6e73 7061 7265 6e74 2030     transparent 0
-000008f0: 252c 0d0a 2020 2020 2020 2020 2020 2020  %,..            
-00000900: 2020 2020 2020 2020 7267 6261 2833 322c          rgba(32,
-00000910: 2031 3238 2c20 3332 2c20 302e 3229 2032   128, 32, 0.2) 2
-00000920: 252c 0d0a 2020 2020 2020 2020 2020 2020  %,..            
-00000930: 2020 2020 2020 2020 7267 6261 2833 322c          rgba(32,
-00000940: 2031 3238 2c20 3332 2c20 302e 3829 2033   128, 32, 0.8) 3
-00000950: 252c 0d0a 2020 2020 2020 2020 2020 2020  %,..            
-00000960: 2020 2020 2020 2020 7267 6261 2833 322c          rgba(32,
-00000970: 2031 3238 2c20 3332 2c20 302e 3229 2033   128, 32, 0.2) 3
-00000980: 252c 0d0a 2020 2020 2020 2020 2020 2020  %,..            
-00000990: 2020 2020 2020 2020 7472 616e 7370 6172          transpar
-000009a0: 656e 7420 3130 3025 293b 0d0a 2020 2020  ent 100%);..    
-000009b0: 2020 2020 2020 2020 6261 636b 6772 6f75          backgrou
-000009c0: 6e64 2d72 6570 6561 743a 206e 6f2d 7265  nd-repeat: no-re
-000009d0: 7065 6174 3b0d 0a20 2020 2020 2020 2020  peat;..         
-000009e0: 2020 2061 6e69 6d61 7469 6f6e 3a20 7363     animation: sc
-000009f0: 616e 2037 2e35 7320 6c69 6e65 6172 2030  an 7.5s linear 0
-00000a00: 7320 696e 6669 6e69 7465 3b0d 0a20 2020  s infinite;..   
-00000a10: 2020 2020 207d 0d0a 0d0a 2020 2020 2020       }....      
-00000a20: 2020 406b 6579 6672 616d 6573 2073 6361    @keyframes sca
-00000a30: 6e20 7b0d 0a20 2020 2020 2020 2020 2020  n {..           
-00000a40: 2030 2520 7b0d 0a20 2020 2020 2020 2020   0% {..         
-00000a50: 2020 2020 2020 2062 6163 6b67 726f 756e         backgroun
-00000a60: 642d 706f 7369 7469 6f6e 3a20 3020 2d31  d-position: 0 -1
-00000a70: 3030 7668 3b0d 0a20 2020 2020 2020 2020  00vh;..         
-00000a80: 2020 207d 0d0a 0d0a 2020 2020 2020 2020     }....        
-00000a90: 2020 2020 3335 252c 0d0a 2020 2020 2020      35%,..      
-00000aa0: 2020 2020 2020 3130 3025 207b 0d0a 2020        100% {..  
-00000ab0: 2020 2020 2020 2020 2020 2020 2020 6261                ba
-00000ac0: 636b 6772 6f75 6e64 2d70 6f73 6974 696f  ckground-positio
-00000ad0: 6e3a 2030 2031 3030 7668 3b0d 0a20 2020  n: 0 100vh;..   
-00000ae0: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
-00000af0: 2020 2020 7d0d 0a0d 0a20 2020 2020 2020      }....       
-00000b00: 202e 7465 726d 696e 616c 207b 0d0a 2020   .terminal {..  
-00000b10: 2020 2020 2020 2020 2020 626f 782d 7369            box-si
-00000b20: 7a69 6e67 3a20 696e 6865 7269 743b 0d0a  zing: inherit;..
-00000b30: 2020 2020 2020 2020 2020 2020 706f 7369              posi
-00000b40: 7469 6f6e 3a20 6162 736f 6c75 7465 3b0d  tion: absolute;.
-00000b50: 0a20 2020 2020 2020 2020 2020 2068 6569  .            hei
-00000b60: 6768 743a 2031 3030 253b 0d0a 2020 2020  ght: 100%;..    
-00000b70: 2020 2020 2020 2020 7769 6474 683a 2031          width: 1
-00000b80: 3030 3070 783b 0d0a 2020 2020 2020 2020  000px;..        
-00000b90: 2020 2020 6d61 782d 7769 6474 683a 2031      max-width: 1
-00000ba0: 3030 253b 0d0a 2020 2020 2020 2020 2020  00%;..          
-00000bb0: 2020 7061 6464 696e 673a 2034 7265 6d3b    padding: 4rem;
-00000bc0: 0d0a 2020 2020 2020 2020 2020 2020 7465  ..            te
-00000bd0: 7874 2d74 7261 6e73 666f 726d 3a20 7570  xt-transform: up
-00000be0: 7065 7263 6173 653b 0d0a 2020 2020 2020  percase;..      
-00000bf0: 2020 7d0d 0a0d 0a20 2020 2020 2020 202e    }....        .
-00000c00: 6f75 7470 7574 207b 0d0a 2020 2020 2020  output {..      
-00000c10: 2020 2020 2020 636f 6c6f 723a 2072 6762        color: rgb
-00000c20: 6128 3132 382c 2032 3535 2c20 3132 382c  a(128, 255, 128,
-00000c30: 2030 2e38 293b 0d0a 2020 2020 2020 2020   0.8);..        
-00000c40: 2020 2020 7465 7874 2d73 6861 646f 773a      text-shadow:
-00000c50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000c60: 2020 3020 3020 3170 7820 7267 6261 2835    0 0 1px rgba(5
-00000c70: 312c 2032 3535 2c20 3531 2c20 302e 3429  1, 255, 51, 0.4)
-00000c80: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000c90: 2020 2030 2030 2032 7078 2072 6762 6128     0 0 2px rgba(
-00000ca0: 3235 352c 2032 3535 2c20 3235 352c 2030  255, 255, 255, 0
-00000cb0: 2e38 293b 0d0a 2020 2020 2020 2020 7d0d  .8);..        }.
-00000cc0: 0a0d 0a20 2020 2020 2020 202e 6f75 7470  ...        .outp
-00000cd0: 7574 3a3a 6265 666f 7265 207b 0d0a 2020  ut::before {..  
-00000ce0: 2020 2020 2020 2020 2020 636f 6e74 656e            conten
-00000cf0: 743a 2022 3e20 223b 0d0a 2020 2020 2020  t: "> ";..      
-00000d00: 2020 7d0d 0a0d 0a20 2020 2020 2020 2061    }....        a
-00000d10: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00000d20: 636f 6c6f 723a 2023 6666 663b 0d0a 2020  color: #fff;..  
-00000d30: 2020 2020 2020 2020 2020 7465 7874 2d64            text-d
-00000d40: 6563 6f72 6174 696f 6e3a 206e 6f6e 653b  ecoration: none;
-00000d50: 0d0a 2020 2020 2020 2020 7d0d 0a0d 0a20  ..        }.... 
-00000d60: 2020 2020 2020 2061 3a3a 6265 666f 7265         a::before
-00000d70: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00000d80: 636f 6e74 656e 743a 2022 5b22 3b0d 0a20  content: "[";.. 
-00000d90: 2020 2020 2020 207d 0d0a 0d0a 2020 2020         }....    
-00000da0: 2020 2020 613a 3a61 6674 6572 207b 0d0a      a::after {..
-00000db0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00000dc0: 656e 743a 2022 5d22 3b0d 0a20 2020 2020  ent: "]";..     
-00000dd0: 2020 207d 0d0a 0d0a 2020 2020 2020 2020     }....        
-00000de0: 2e65 7272 6f72 636f 6465 207b 0d0a 2020  .errorcode {..  
-00000df0: 2020 2020 2020 2020 2020 636f 6c6f 723a            color:
-00000e00: 2077 6869 7465 3b0d 0a20 2020 2020 2020   white;..       
-00000e10: 207d 0d0a 2020 2020 3c2f 7374 796c 653e   }..    </style>
-00000e20: 0d0a 3c2f 6865 6164 3e0d 0a0d 0a3c 626f  ..</head>....<bo
-00000e30: 6479 3e0d 0a20 2020 203c 6469 7620 636c  dy>..    <div cl
-00000e40: 6173 733d 226e 6f69 7365 223e 3c2f 6469  ass="noise"></di
-00000e50: 763e 0d0a 2020 2020 3c64 6976 2063 6c61  v>..    <div cla
-00000e60: 7373 3d22 6f76 6572 6c61 7922 3e3c 2f64  ss="overlay"></d
-00000e70: 6976 3e0d 0a20 2020 203c 6469 7620 636c  iv>..    <div cl
-00000e80: 6173 733d 2274 6572 6d69 6e61 6c22 3e0d  ass="terminal">.
-00000e90: 0a20 2020 2020 2020 203c 6831 3e45 7272  .        <h1>Err
-00000ea0: 6f72 203c 7370 616e 2063 6c61 7373 3d22  or <span class="
-00000eb0: 6572 726f 7263 6f64 6522 3e34 3034 3c2f  errorcode">404</
-00000ec0: 7370 616e 3e3c 2f68 313e 0d0a 2020 2020  span></h1>..    
-00000ed0: 2020 2020 3c70 2063 6c61 7373 3d22 6f75      <p class="ou
-00000ee0: 7470 7574 223e 5468 6520 7061 6765 2079  tput">The page y
-00000ef0: 6f75 2061 7265 206c 6f6f 6b69 6e67 2066  ou are looking f
-00000f00: 6f72 206d 6967 6874 2068 6176 6520 6265  or might have be
-00000f10: 656e 2072 656d 6f76 6564 2c20 6861 6420  en removed, had 
-00000f20: 6974 7320 6e61 6d65 2063 6861 6e67 6564  its name changed
-00000f30: 206f 7220 6973 2074 656d 706f 7261 7269   or is temporari
-00000f40: 6c79 0d0a 2020 2020 2020 2020 2020 2020  ly..            
-00000f50: 756e 6176 6169 6c61 626c 652e 3c2f 703e  unavailable.</p>
-00000f60: 0d0a 2020 2020 2020 2020 3c70 2063 6c61  ..        <p cla
-00000f70: 7373 3d22 6f75 7470 7574 223e 506c 6561  ss="output">Plea
-00000f80: 7365 203c 6120 6872 6566 3d22 2f22 3e72  se <a href="/">r
-00000f90: 6574 7572 6e20 746f 2074 6865 2068 6f6d  eturn to the hom
-00000fa0: 6570 6167 653c 2f61 3e2e 3c2f 703e 0d0a  epage</a>.</p>..
-00000fb0: 2020 2020 2020 2020 3c70 2063 6c61 7373          <p class
-00000fc0: 3d22 6f75 7470 7574 223e 476f 6f64 206c  ="output">Good l
-00000fd0: 7563 6b2e 3c2f 703e 0d0a 2020 2020 2020  uck.</p>..      
-00000fe0: 2020 3c70 2063 6c61 7373 3d22 6f75 7470    <p class="outp
-00000ff0: 7574 223e 4372 6564 6974 7320 746f 203c  ut">Credits to <
-00001000: 6120 6872 6566 3d27 6874 7470 733a 2f2f  a href='https://
-00001010: 636f 6465 7065 6e2e 696f 2f63 6f64 6532  codepen.io/code2
-00001020: 7269 7468 696b 2720 7461 7267 6574 3d22  rithik' target="
-00001030: 5f62 6c61 6e6b 223e 5269 7468 696b 2053  _blank">Rithik S
-00001040: 616d 616e 7468 756c 6120 2840 636f 6465  amanthula (@code
-00001050: 3272 6974 6869 6b29 213c 2f61 3e3c 2f70  2rithik)!</a></p
-00001060: 3e0d 0a20 2020 203c 2f64 6976 3e0d 0a3c  >..    </div>..<
-00001070: 2f62 6f64 793e 0d0a 0d0a 3c2f 6874 6d6c  /body>....</html
-00001080: 3e0d 0a22 2222 0d0a 0d0a 6630 3020 3d20  >.."""....f00 = 
-00001090: 2222 220d 0a3c 2144 4f43 5459 5045 2068  """..<!DOCTYPE h
-000010a0: 746d 6c3e 0d0a 3c68 746d 6c20 6c61 6e67  tml>..<html lang
-000010b0: 3d22 656e 223e 0d0a 3c68 6561 643e 0d0a  ="en">..<head>..
-000010c0: 3c73 7479 6c65 3e0d 0a2a 2c0d 0a2a 3a3a  <style>..*,..*::
-000010d0: 6166 7465 722c 0d0a 2a3a 3a62 6566 6f72  after,..*::befor
-000010e0: 6520 7b0d 0a09 626f 782d 7369 7a69 6e67  e {...box-sizing
-000010f0: 3a20 626f 7264 6572 2d62 6f78 3b0d 0a7d  : border-box;..}
-00001100: 0d0a 0d0a 6874 6d6c 2c0d 0a62 6f64 7920  ....html,..body 
-00001110: 7b0d 0a09 616c 6967 6e2d 6974 656d 733a  {...align-items:
-00001120: 2063 656e 7465 723b 0d0a 0962 6163 6b67   center;...backg
-00001130: 726f 756e 643a 206c 696e 6561 722d 6772  round: linear-gr
-00001140: 6164 6965 6e74 2823 3030 3365 6666 2c20  adient(#003eff, 
-00001150: 2330 3032 3861 3929 3b0d 0a09 636f 6c6f  #0028a9);...colo
-00001160: 723a 2077 6869 7465 3b0d 0a09 6469 7370  r: white;...disp
-00001170: 6c61 793a 2066 6c65 783b 0d0a 0966 6f6e  lay: flex;...fon
-00001180: 743a 2032 7265 6d20 2250 6f69 7265 7420  t: 2rem "Poiret 
-00001190: 4f6e 6522 3b0d 0a09 6865 6967 6874 3a20  One";...height: 
-000011a0: 3130 3076 683b 0d0a 096a 7573 7469 6679  100vh;...justify
-000011b0: 2d63 6f6e 7465 6e74 3a20 6365 6e74 6572  -content: center
-000011c0: 3b0d 0a09 6d61 7267 696e 3a20 303b 0d0a  ;...margin: 0;..
-000011d0: 0970 6164 6469 6e67 3a20 303b 0d0a 7d0d  .padding: 0;..}.
-000011e0: 0a0d 0a2e 626f 7820 7b0d 0a09 6865 6967  ....box {...heig
-000011f0: 6874 3a20 3130 3070 783b 0d0a 096d 6172  ht: 100px;...mar
-00001200: 6769 6e3a 2030 2031 3070 783b 0d0a 096f  gin: 0 10px;...o
-00001210: 7665 7266 6c6f 773a 2068 6964 6465 6e3b  verflow: hidden;
-00001220: 0d0a 0970 6f73 6974 696f 6e3a 2072 656c  ...position: rel
-00001230: 6174 6976 653b 0d0a 0974 7261 6e73 666f  ative;...transfo
-00001240: 726d 3a20 726f 7461 7465 5a28 3237 3064  rm: rotateZ(270d
-00001250: 6567 2920 7363 616c 6528 312e 3035 293b  eg) scale(1.05);
-00001260: 0d0a 0977 6964 7468 3a20 3130 3070 783b  ...width: 100px;
-00001270: 0d0a 7d0d 0a0d 0a2e 626f 783a 6e74 682d  ..}.....box:nth-
-00001280: 6f66 2d74 7970 6528 3229 207b 0d0a 096c  of-type(2) {...l
-00001290: 6566 743a 202d 3238 7078 3b0d 0a09 7472  eft: -28px;...tr
-000012a0: 616e 7366 6f72 6d3a 2072 6f74 6174 6558  ansform: rotateX
-000012b0: 282d 3138 3064 6567 2920 726f 7461 7465  (-180deg) rotate
-000012c0: 5928 3138 3064 6567 2920 726f 7461 7465  Y(180deg) rotate
-000012d0: 5a28 3237 3064 6567 2920 7363 616c 6528  Z(270deg) scale(
-000012e0: 312e 3035 293b 0d0a 7d0d 0a0d 0a2e 626f  1.05);..}.....bo
-000012f0: 7820 7370 616e 207b 0d0a 0961 6e69 6d61  x span {...anima
-00001300: 7469 6f6e 3a20 6c6f 6164 6572 2034 2e38  tion: loader 4.8
-00001310: 7320 696e 6669 6e69 7465 2062 6f74 683b  s infinite both;
-00001320: 0d0a 0964 6973 706c 6179 3a20 626c 6f63  ...display: bloc
-00001330: 6b3b 0d0a 0968 6569 6768 743a 2031 3030  k;...height: 100
-00001340: 253b 0d0a 0970 6f73 6974 696f 6e3a 2061  %;...position: a
-00001350: 6273 6f6c 7574 653b 0d0a 0977 6964 7468  bsolute;...width
-00001360: 3a20 3130 3025 3b0d 0a7d 0d0a 0d0a 2e62  : 100%;..}.....b
-00001370: 6f78 2073 7061 6e3a 6e74 682d 6368 696c  ox span:nth-chil
-00001380: 6428 3129 207b 0d0a 0961 6e69 6d61 7469  d(1) {...animati
-00001390: 6f6e 2d64 656c 6179 3a20 302e 3273 3b0d  on-delay: 0.2s;.
-000013a0: 0a7d 0d0a 0d0a 2e62 6f78 2073 7061 6e3a  .}.....box span:
-000013b0: 6e74 682d 6368 696c 6428 3229 207b 0d0a  nth-child(2) {..
-000013c0: 0961 6e69 6d61 7469 6f6e 2d64 656c 6179  .animation-delay
-000013d0: 3a20 302e 3473 3b0d 0a7d 0d0a 0d0a 2e62  : 0.4s;..}.....b
-000013e0: 6f78 2073 7061 6e3a 6e74 682d 6368 696c  ox span:nth-chil
-000013f0: 6428 3329 207b 0d0a 0961 6e69 6d61 7469  d(3) {...animati
-00001400: 6f6e 2d64 656c 6179 3a20 302e 3673 3b0d  on-delay: 0.6s;.
-00001410: 0a7d 0d0a 0d0a 2e62 6f78 2073 7061 6e3a  .}.....box span:
-00001420: 6e74 682d 6368 696c 6428 3429 207b 0d0a  nth-child(4) {..
-00001430: 0961 6e69 6d61 7469 6f6e 2d64 656c 6179  .animation-delay
-00001440: 3a20 302e 3873 3b0d 0a7d 0d0a 0d0a 2e62  : 0.8s;..}.....b
-00001450: 6f78 2073 7061 6e3a 6e74 682d 6368 696c  ox span:nth-chil
-00001460: 6428 3529 207b 0d0a 0961 6e69 6d61 7469  d(5) {...animati
-00001470: 6f6e 2d64 656c 6179 3a20 3173 3b0d 0a7d  on-delay: 1s;..}
-00001480: 0d0a 0d0a 2e62 6f78 2073 7061 6e3a 6e74  .....box span:nt
-00001490: 682d 6368 696c 6428 3629 207b 0d0a 0961  h-child(6) {...a
-000014a0: 6e69 6d61 7469 6f6e 2d64 656c 6179 3a20  nimation-delay: 
-000014b0: 312e 3273 3b0d 0a7d 0d0a 0d0a 2e62 6f78  1.2s;..}.....box
-000014c0: 2073 7061 6e3a 3a61 6674 6572 207b 0d0a   span::after {..
-000014d0: 0962 6163 6b67 726f 756e 643a 2023 6666  .background: #ff
-000014e0: 663b 0d0a 0962 6f72 6465 722d 7261 6469  f;...border-radi
-000014f0: 7573 3a20 3530 253b 0d0a 0963 6f6e 7465  us: 50%;...conte
-00001500: 6e74 3a20 2222 3b0d 0a09 6c65 6674 3a20  nt: "";...left: 
-00001510: 3530 253b 0d0a 0970 6164 6469 6e67 3a20  50%;...padding: 
-00001520: 3670 783b 0d0a 0970 6f73 6974 696f 6e3a  6px;...position:
-00001530: 2061 6273 6f6c 7574 653b 0d0a 0974 6f70   absolute;...top
-00001540: 3a20 303b 0d0a 0974 7261 6e73 666f 726d  : 0;...transform
-00001550: 3a20 7472 616e 736c 6174 6558 282d 3530  : translateX(-50
-00001560: 2529 3b0d 0a7d 0d0a 0d0a 406b 6579 6672  %);..}....@keyfr
-00001570: 616d 6573 206c 6f61 6465 7220 7b0d 0a09  ames loader {...
-00001580: 3025 207b 0d0a 0909 6f70 6163 6974 793a  0% {....opacity:
-00001590: 2030 3b0d 0a09 0974 7261 6e73 666f 726d   0;....transform
-000015a0: 3a20 726f 7461 7465 2831 3830 6465 6729  : rotate(180deg)
-000015b0: 3b0d 0a09 0961 6e69 6d61 7469 6f6e 2d74  ;....animation-t
-000015c0: 696d 696e 672d 6675 6e63 7469 6f6e 3a20  iming-function: 
-000015d0: 6561 7365 2d6f 7574 3b0d 0a09 7d0d 0a09  ease-out;...}...
-000015e0: 3525 207b 0d0a 0909 6f70 6163 6974 793a  5% {....opacity:
-000015f0: 2031 3b0d 0a09 0974 7261 6e73 666f 726d   1;....transform
-00001600: 3a20 726f 7461 7465 2833 3030 6465 6729  : rotate(300deg)
-00001610: 3b0d 0a09 0961 6e69 6d61 7469 6f6e 2d74  ;....animation-t
-00001620: 696d 696e 672d 6675 6e63 7469 6f6e 3a20  iming-function: 
-00001630: 6c69 6e65 6172 3b0d 0a09 7d0d 0a09 3330  linear;...}...30
-00001640: 2520 7b0d 0a09 0974 7261 6e73 666f 726d  % {....transform
-00001650: 3a20 726f 7461 7465 2834 3230 6465 6729  : rotate(420deg)
-00001660: 3b0d 0a09 0961 6e69 6d61 7469 6f6e 2d74  ;....animation-t
-00001670: 696d 696e 672d 6675 6e63 7469 6f6e 3a20  iming-function: 
-00001680: 6561 7365 2d69 6e2d 6f75 743b 0d0a 097d  ease-in-out;...}
-00001690: 0d0a 0933 3525 207b 0d0a 0909 7472 616e  ...35% {....tran
-000016a0: 7366 6f72 6d3a 2072 6f74 6174 6528 3632  sform: rotate(62
-000016b0: 3564 6567 293b 0d0a 0909 616e 696d 6174  5deg);....animat
-000016c0: 696f 6e2d 7469 6d69 6e67 2d66 756e 6374  ion-timing-funct
-000016d0: 696f 6e3a 206c 696e 6561 723b 0d0a 097d  ion: linear;...}
-000016e0: 0d0a 0937 3025 207b 0d0a 0909 7472 616e  ...70% {....tran
-000016f0: 7366 6f72 6d3a 2072 6f74 6174 6528 3830  sform: rotate(80
-00001700: 3064 6567 293b 0d0a 0909 616e 696d 6174  0deg);....animat
-00001710: 696f 6e2d 7469 6d69 6e67 2d66 756e 6374  ion-timing-funct
-00001720: 696f 6e3a 2065 6173 652d 6f75 743b 0d0a  ion: ease-out;..
-00001730: 0909 6f70 6163 6974 793a 2031 3b0d 0a09  ..opacity: 1;...
-00001740: 7d0d 0a09 3735 2520 7b0d 0a09 096f 7061  }...75% {....opa
-00001750: 6369 7479 3a20 303b 0d0a 0909 7472 616e  city: 0;....tran
-00001760: 7366 6f72 6d3a 2072 6f74 6174 6528 3930  sform: rotate(90
-00001770: 3064 6567 293b 0d0a 0909 616e 696d 6174  0deg);....animat
-00001780: 696f 6e2d 7469 6d69 6e67 2d66 756e 6374  ion-timing-funct
-00001790: 696f 6e3a 2065 6173 652d 6f75 743b 0d0a  ion: ease-out;..
-000017a0: 097d 0d0a 0937 3625 207b 0d0a 0909 6f70  .}...76% {....op
-000017b0: 6163 6974 793a 2030 3b0d 0a09 0974 7261  acity: 0;....tra
-000017c0: 6e73 666f 726d 3a20 726f 7461 7465 2839  nsform: rotate(9
-000017d0: 3030 6465 6729 3b0d 0a09 7d0d 0a09 3130  00deg);...}...10
-000017e0: 3025 207b 0d0a 0909 6f70 6163 6974 793a  0% {....opacity:
-000017f0: 2030 3b0d 0a09 0974 7261 6e73 666f 726d   0;....transform
-00001800: 3a20 726f 7461 7465 2839 3030 6465 6729  : rotate(900deg)
-00001810: 3b0d 0a09 7d0d 0a7d 0d0a 0d0a 6831 207b  ;...}..}....h1 {
-00001820: 0d0a 0974 6578 742d 7368 6164 6f77 3a20  ...text-shadow: 
-00001830: 3020 3020 3130 7078 2023 6666 663b 0d0a  0 0 10px #fff;..
-00001840: 0961 6e69 6d61 7469 6f6e 3a20 626c 696e  .animation: blin
-00001850: 6b20 342e 3873 2069 6e66 696e 6974 6520  k 4.8s infinite 
-00001860: 626f 7468 3b0d 0a7d 0d0a 0d0a 6831 3a6e  both;..}....h1:n
-00001870: 7468 2d6f 662d 7479 7065 2832 2920 7b0d  th-of-type(2) {.
-00001880: 0a09 616e 696d 6174 696f 6e3a 206e 6f6e  ..animation: non
-00001890: 653b 0d0a 096c 6574 7465 722d 7370 6163  e;...letter-spac
-000018a0: 696e 673a 202d 3134 7078 3b0d 0a09 6d61  ing: -14px;...ma
-000018b0: 7267 696e 3a20 3020 6175 746f 3b0d 0a09  rgin: 0 auto;...
-000018c0: 6f70 6163 6974 793a 2030 2e31 3b0d 0a09  opacity: 0.1;...
-000018d0: 7061 6464 696e 672d 6c65 6674 3a20 3431  padding-left: 41
-000018e0: 7078 3b0d 0a09 706f 7369 7469 6f6e 3a20  px;...position: 
-000018f0: 6162 736f 6c75 7465 3b0d 0a09 746f 703a  absolute;...top:
-00001900: 2035 3025 3b0d 0a09 7472 616e 7366 6f72   50%;...transfor
-00001910: 6d3a 2074 7261 6e73 6c61 7465 7928 2d35  m: translatey(-5
-00001920: 3025 293b 0d0a 7d0d 0a0d 0a40 6b65 7966  0%);..}....@keyf
-00001930: 7261 6d65 7320 626c 696e 6b20 7b0d 0a09  rames blink {...
-00001940: 3025 2c0d 0a09 3530 252c 0d0a 0931 3030  0%,...50%,...100
-00001950: 2520 7b0d 0a09 096f 7061 6369 7479 3a20  % {....opacity: 
-00001960: 302e 323b 0d0a 097d 0d0a 0932 3525 2c0d  0.2;...}...25%,.
-00001970: 0a09 3735 2520 7b0d 0a09 096f 7061 6369  ..75% {....opaci
-00001980: 7479 3a20 313b 0d0a 097d 0d0a 7d0d 0a0d  ty: 1;...}..}...
-00001990: 0a68 352c 0d0a 7020 7b0d 0a09 706f 7369  .h5,..p {...posi
-000019a0: 7469 6f6e 3a20 6162 736f 6c75 7465 3b0d  tion: absolute;.
-000019b0: 0a09 666f 6e74 2d66 616d 696c 793a 206d  ..font-family: m
-000019c0: 6f6e 6f73 7061 6365 3b0d 0a7d 0d0a 0d0a  onospace;..}....
-000019d0: 6835 207b 0d0a 0974 6f70 3a20 3130 253b  h5 {...top: 10%;
-000019e0: 0d0a 0966 6f6e 742d 7369 7a65 3a20 302e  ...font-size: 0.
-000019f0: 3465 6d3b 0d0a 090d 0a7d 0d0a 0d0a 7020  4em;.....}....p 
-00001a00: 7b0d 0a09 666f 6e74 2d73 697a 653a 2030  {...font-size: 0
-00001a10: 2e33 656d 3b0d 0a09 626f 7474 6f6d 3a20  .3em;...bottom: 
-00001a20: 3130 253b 0d0a 0977 6964 7468 3a20 3530  10%;...width: 50
-00001a30: 253b 0d0a 0974 6578 742d 616c 6967 6e3a  %;...text-align:
-00001a40: 2063 656e 7465 723b 0d0a 7d0d 0a0d 0a70   center;..}....p
-00001a50: 2061 207b 0d0a 0963 6f6c 6f72 3a20 6379   a {...color: cy
-00001a60: 616e 3b0d 0a7d 0d0a 0d0a 3c2f 7374 796c  an;..}....</styl
-00001a70: 653e 0d0a 3c2f 6865 6164 3e0d 0a3c 626f  e>..</head>..<bo
-00001a80: 6479 3e0d 0a3c 6835 3e49 6e74 6572 6e61  dy>..<h5>Interna
-00001a90: 6c20 5365 7276 6572 2065 7272 6f72 2021  l Server error !
-00001aa0: 3c2f 6835 3e0d 0a20 2020 203c 6831 3e35  </h5>..    <h1>5
-00001ab0: 3c2f 6831 3e0d 0a20 2020 203c 6831 3e30  </h1>..    <h1>0
-00001ac0: 303c 2f68 313e 0d0a 2020 2020 3c64 6976  0</h1>..    <div
-00001ad0: 2063 6c61 7373 3d22 626f 7822 3e0d 0a09   class="box">...
-00001ae0: 0909 3c73 7061 6e3e 3c2f 7370 616e 3e3c  ..<span></span><
-00001af0: 7370 616e 3e3c 2f73 7061 6e3e 0d0a 0909  span></span>....
-00001b00: 093c 7370 616e 3e3c 2f73 7061 6e3e 3c73  .<span></span><s
-00001b10: 7061 6e3e 3c2f 7370 616e 3e0d 0a09 0909  pan></span>.....
-00001b20: 3c73 7061 6e3e 3c2f 7370 616e 3e0d 0a09  <span></span>...
-00001b30: 093c 2f64 6976 3e0d 0a20 2020 203c 6469  .</div>..    <di
-00001b40: 7620 636c 6173 733d 2262 6f78 223e 0d0a  v class="box">..
-00001b50: 0909 093c 7370 616e 3e3c 2f73 7061 6e3e  ...<span></span>
-00001b60: 3c73 7061 6e3e 3c2f 7370 616e 3e0d 0a09  <span></span>...
-00001b70: 0909 3c73 7061 6e3e 3c2f 7370 616e 3e3c  ..<span></span><
-00001b80: 7370 616e 3e3c 2f73 7061 6e3e 0d0a 0909  span></span>....
-00001b90: 093c 7370 616e 3e3c 2f73 7061 6e3e 0d0a  .<span></span>..
-00001ba0: 0909 3c2f 6469 763e 0d0a 2020 2020 3c70  ..</div>..    <p
-00001bb0: 3e20 5765 2772 6520 756e 6162 6c65 2074  > We're unable t
-00001bc0: 6f20 6669 6e64 206f 7574 2077 6861 7427  o find out what'
-00001bd0: 7320 6861 7070 656e 696e 6721 2057 6520  s happening! We 
-00001be0: 7375 6767 6573 7420 796f 7520 746f 0d0a  suggest you to..
-00001bf0: 0909 093c 6272 2f3e 0d0a 0909 093c 6120  ...<br/>.....<a 
-00001c00: 6872 6566 3d22 2f22 3e47 6f20 486f 6d65  href="/">Go Home
-00001c10: 3c2f 613e 0d0a 0909 096f 7220 7669 7369  </a>.....or visi
-00001c20: 7420 6865 7265 206c 6174 6572 2e20 4372  t here later. Cr
-00001c30: 6564 6974 7320 746f 203c 6120 6872 6566  edits to <a href
-00001c40: 3d27 6874 7470 733a 2f2f 636f 6465 7065  ='https://codepe
-00001c50: 6e2e 696f 2f61 6473 696e 6768 3134 2720  n.io/adsingh14' 
-00001c60: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
-00001c70: 414d 414e 2028 4061 6473 696e 6768 3134  AMAN (@adsingh14
-00001c80: 2921 3c2f 613e 3c2f 703e 0d0a 3c2f 626f  )!</a></p>..</bo
-00001c90: 6479 3e0d 0a3c 2f68 746d 6c3e 0d0a 2222  dy>..</html>..""
-00001ca0: 220d 0a0d 0a0d 0a63 6c61 7373 2053 6974  "......class Sit
-00001cb0: 6550 793a 0d0a 2020 2020 6465 6620 5f5f  ePy:..    def __
-00001cc0: 696e 6974 5f5f 280d 0a20 2020 2020 2020  init__(..       
-00001cd0: 2073 656c 662c 2073 7461 7469 635f 6469   self, static_di
-00001ce0: 723d 2273 7461 7469 6322 2c20 7465 6d70  r="static", temp
-00001cf0: 6c61 7465 735f 6469 723d 2274 656d 706c  lates_dir="templ
-00001d00: 6174 6573 222c 2063 7573 746f 6d5f 3430  ates", custom_40
-00001d10: 345f 7061 6765 3d4e 6f6e 652c 2063 7573  4_page=None, cus
-00001d20: 746f 6d5f 3530 305f 7061 6765 3d4e 6f6e  tom_500_page=Non
-00001d30: 650d 0a20 2020 2029 3a0d 0a20 2020 2020  e..    ):..     
-00001d40: 2020 2073 656c 662e 726f 7574 6573 203d     self.routes =
-00001d50: 207b 7d0d 0a20 2020 2020 2020 2073 656c   {}..        sel
-00001d60: 662e 6d69 6464 6c65 7761 7265 203d 205b  f.middleware = [
-00001d70: 7365 6c66 2e6c 6f67 6765 725f 6d69 6464  self.logger_midd
-00001d80: 6c65 7761 7265 5d0d 0a20 2020 2020 2020  leware]..       
-00001d90: 2073 656c 662e 7374 6174 6963 5f64 6972   self.static_dir
-00001da0: 203d 2073 7461 7469 635f 6469 720d 0a20   = static_dir.. 
-00001db0: 2020 2020 2020 2073 656c 662e 7465 6d70         self.temp
-00001dc0: 6c61 7465 735f 6469 7220 3d20 7465 6d70  lates_dir = temp
-00001dd0: 6c61 7465 735f 6469 720d 0a20 2020 2020  lates_dir..     
-00001de0: 2020 2073 656c 662e 6375 7374 6f6d 5f34     self.custom_4
-00001df0: 3034 5f70 6167 6520 3d20 6375 7374 6f6d  04_page = custom
-00001e00: 5f34 3034 5f70 6167 650d 0a20 2020 2020  _404_page..     
-00001e10: 2020 2073 656c 662e 6375 7374 6f6d 5f35     self.custom_5
-00001e20: 3030 5f70 6167 6520 3d20 6375 7374 6f6d  00_page = custom
-00001e30: 5f35 3030 5f70 6167 650d 0a0d 0a20 2020  _500_page....   
-00001e40: 2064 6566 2072 656e 6465 725f 7465 6d70   def render_temp
-00001e50: 6c61 7465 2873 656c 662c 2074 656d 706c  late(self, templ
-00001e60: 6174 655f 6e61 6d65 2c20 2a2a 636f 6e74  ate_name, **cont
-00001e70: 6578 7429 3a0d 0a20 2020 2020 2020 2065  ext):..        e
-00001e80: 6e76 203d 2045 6e76 6972 6f6e 6d65 6e74  nv = Environment
-00001e90: 286c 6f61 6465 723d 4669 6c65 5379 7374  (loader=FileSyst
-00001ea0: 656d 4c6f 6164 6572 2873 656c 662e 7465  emLoader(self.te
-00001eb0: 6d70 6c61 7465 735f 6469 7229 290d 0a20  mplates_dir)).. 
-00001ec0: 2020 2020 2020 2074 656d 706c 6174 6520         template 
-00001ed0: 3d20 656e 762e 6765 745f 7465 6d70 6c61  = env.get_templa
-00001ee0: 7465 2874 656d 706c 6174 655f 6e61 6d65  te(template_name
-00001ef0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00001f00: 6e20 7465 6d70 6c61 7465 2e72 656e 6465  n template.rende
-00001f10: 7228 2a2a 636f 6e74 6578 7429 0d0a 0d0a  r(**context)....
-00001f20: 2020 2020 6465 6620 726f 7574 6528 7365      def route(se
-00001f30: 6c66 2c20 7061 7468 2c20 6d65 7468 6f64  lf, path, method
-00001f40: 733d 5b22 4745 5422 5d29 3a0d 0a20 2020  s=["GET"]):..   
-00001f50: 2020 2020 2064 6566 2077 7261 7070 6572       def wrapper
-00001f60: 2868 616e 646c 6572 293a 0d0a 2020 2020  (handler):..    
-00001f70: 2020 2020 2020 2020 7365 6c66 2e72 6f75          self.rou
-00001f80: 7465 735b 2870 6174 682c 2074 7570 6c65  tes[(path, tuple
-00001f90: 286d 6574 686f 6473 2929 5d20 3d20 6861  (methods))] = ha
-00001fa0: 6e64 6c65 720d 0a20 2020 2020 2020 2020  ndler..         
-00001fb0: 2020 2072 6574 7572 6e20 6861 6e64 6c65     return handle
-00001fc0: 720d 0a0d 0a20 2020 2020 2020 2072 6574  r....        ret
-00001fd0: 7572 6e20 7772 6170 7065 720d 0a0d 0a20  urn wrapper.... 
-00001fe0: 2020 2064 6566 2075 7365 2873 656c 662c     def use(self,
-00001ff0: 206d 6964 646c 6577 6172 6529 3a0d 0a20   middleware):.. 
-00002000: 2020 2020 2020 2073 656c 662e 6d69 6464         self.midd
-00002010: 6c65 7761 7265 2e61 7070 656e 6428 6d69  leware.append(mi
-00002020: 6464 6c65 7761 7265 290d 0a0d 0a20 2020  ddleware)....   
-00002030: 2064 6566 206c 6f67 6765 725f 6d69 6464   def logger_midd
-00002040: 6c65 7761 7265 2873 656c 662c 2065 6e76  leware(self, env
-00002050: 6972 6f6e 293a 0d0a 2020 2020 2020 2020  iron):..        
-00002060: 7072 696e 7428 6622 5265 7175 6573 7420  print(f"Request 
-00002070: 7265 6365 6976 6564 2066 6f72 207b 656e  received for {en
-00002080: 7669 726f 6e5b 2750 4154 485f 494e 464f  viron['PATH_INFO
-00002090: 275d 7d22 290d 0a0d 0a20 2020 2064 6566  ']}")....    def
-000020a0: 205f 5f63 616c 6c5f 5f28 7365 6c66 2c20   __call__(self, 
-000020b0: 656e 7669 726f 6e2c 2073 7461 7274 5f72  environ, start_r
-000020c0: 6573 706f 6e73 6529 3a0d 0a20 2020 2020  esponse):..     
-000020d0: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
-000020e0: 2020 2020 2070 6174 6820 3d20 656e 7669       path = envi
-000020f0: 726f 6e5b 2250 4154 485f 494e 464f 225d  ron["PATH_INFO"]
-00002100: 0d0a 2020 2020 2020 2020 2020 2020 6d65  ..            me
-00002110: 7468 6f64 203d 2065 6e76 6972 6f6e 5b22  thod = environ["
-00002120: 5245 5155 4553 545f 4d45 5448 4f44 225d  REQUEST_METHOD"]
-00002130: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-00002140: 7220 6d69 6464 6c65 7761 7265 2069 6e20  r middleware in 
-00002150: 7365 6c66 2e6d 6964 646c 6577 6172 653a  self.middleware:
-00002160: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002170: 2020 6d69 6464 6c65 7761 7265 2865 6e76    middleware(env
-00002180: 6972 6f6e 290d 0a20 2020 2020 2020 2020  iron)..         
-00002190: 2020 2068 616e 646c 6572 203d 204e 6f6e     handler = Non
-000021a0: 650d 0a20 2020 2020 2020 2020 2020 2066  e..            f
-000021b0: 6f72 2072 6f75 7465 2c20 6d65 7468 6f64  or route, method
-000021c0: 7320 696e 2073 656c 662e 726f 7574 6573  s in self.routes
-000021d0: 2e6b 6579 7328 293a 0d0a 2020 2020 2020  .keys():..      
-000021e0: 2020 2020 2020 2020 2020 6d61 7463 6820            match 
-000021f0: 3d20 726f 7574 652e 6d61 7463 6828 7061  = route.match(pa
-00002200: 7468 290d 0a20 2020 2020 2020 2020 2020  th)..           
-00002210: 2020 2020 2069 6620 6d61 7463 6820 616e       if match an
-00002220: 6420 6d65 7468 6f64 2069 6e20 6d65 7468  d method in meth
-00002230: 6f64 733a 0d0a 2020 2020 2020 2020 2020  ods:..          
-00002240: 2020 2020 2020 2020 2020 6861 6e64 6c65            handle
-00002250: 7220 3d20 7365 6c66 2e72 6f75 7465 735b  r = self.routes[
-00002260: 2872 6f75 7465 2c20 6d65 7468 6f64 7329  (route, methods)
-00002270: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00002280: 2020 2020 2020 2070 6172 616d 7320 3d20         params = 
-00002290: 6d61 7463 682e 6772 6f75 7064 6963 7428  match.groupdict(
-000022a0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000022b0: 2020 2020 2020 2062 7265 616b 0d0a 2020         break..  
-000022c0: 2020 2020 2020 2020 2020 6966 2068 616e            if han
-000022d0: 646c 6572 3a0d 0a20 2020 2020 2020 2020  dler:..         
-000022e0: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
-000022f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002300: 2072 6571 7565 7374 5f62 6f64 795f 7369   request_body_si
-00002310: 7a65 203d 2069 6e74 2865 6e76 6972 6f6e  ze = int(environ
-00002320: 2e67 6574 2822 434f 4e54 454e 545f 4c45  .get("CONTENT_LE
-00002330: 4e47 5448 222c 2030 2929 0d0a 2020 2020  NGTH", 0))..    
-00002340: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-00002350: 7074 2056 616c 7565 4572 726f 723a 0d0a  pt ValueError:..
-00002360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002370: 2020 2020 7265 7175 6573 745f 626f 6479      request_body
-00002380: 5f73 697a 6520 3d20 300d 0a20 2020 2020  _size = 0..     
-00002390: 2020 2020 2020 2020 2020 2072 6571 7565             reque
-000023a0: 7374 5f62 6f64 7920 3d20 656e 7669 726f  st_body = enviro
-000023b0: 6e5b 2277 7367 692e 696e 7075 7422 5d2e  n["wsgi.input"].
-000023c0: 7265 6164 2872 6571 7565 7374 5f62 6f64  read(request_bod
-000023d0: 795f 7369 7a65 290d 0a20 2020 2020 2020  y_size)..       
-000023e0: 2020 2020 2020 2020 2062 6f64 795f 7061           body_pa
-000023f0: 7261 6d73 203d 2070 6172 7365 5f71 7328  rams = parse_qs(
-00002400: 7265 7175 6573 745f 626f 6479 2e64 6563  request_body.dec
-00002410: 6f64 6528 2929 2069 6620 7265 7175 6573  ode()) if reques
-00002420: 745f 626f 6479 2065 6c73 6520 7b7d 0d0a  t_body else {}..
-00002430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002440: 7061 7261 6d73 203d 2070 6172 7365 5f71  params = parse_q
-00002450: 7328 7265 7175 6573 745f 626f 6479 2e64  s(request_body.d
-00002460: 6563 6f64 6528 2929 2069 6620 7265 7175  ecode()) if requ
-00002470: 6573 745f 626f 6479 2065 6c73 6520 7b7d  est_body else {}
-00002480: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002490: 2020 7061 7261 6d73 2e75 7064 6174 6528    params.update(
-000024a0: 626f 6479 5f70 6172 616d 7329 0d0a 2020  body_params)..  
-000024b0: 2020 2020 2020 2020 2020 2020 2020 6861                ha
-000024c0: 6e64 6c65 725f 6172 6773 203d 2069 6e73  ndler_args = ins
-000024d0: 7065 6374 2e73 6967 6e61 7475 7265 2868  pect.signature(h
-000024e0: 616e 646c 6572 292e 7061 7261 6d65 7465  andler).paramete
-000024f0: 7273 0d0a 2020 2020 2020 2020 2020 2020  rs..            
-00002500: 2020 2020 7265 7370 6f6e 7365 5f62 6f64      response_bod
-00002510: 7920 3d20 6861 6e64 6c65 7228 7061 7261  y = handler(para
-00002520: 6d73 2920 6966 2068 616e 646c 6572 5f61  ms) if handler_a
-00002530: 7267 7320 656c 7365 2068 616e 646c 6572  rgs else handler
-00002540: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00002550: 2020 2020 7374 6174 7573 203d 2022 3230      status = "20
-00002560: 3020 4f4b 220d 0a20 2020 2020 2020 2020  0 OK"..         
-00002570: 2020 2020 2020 2068 6561 6465 7273 203d         headers =
-00002580: 205b 2822 436f 6e74 656e 742d 7479 7065   [("Content-type
-00002590: 222c 2022 7465 7874 2f68 746d 6c22 295d  ", "text/html")]
-000025a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000025b0: 2020 7374 6172 745f 7265 7370 6f6e 7365    start_response
-000025c0: 2873 7461 7475 732c 2068 6561 6465 7273  (status, headers
-000025d0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000025e0: 2020 2072 6574 7572 6e20 5b72 6573 706f     return [respo
-000025f0: 6e73 655f 626f 6479 2e65 6e63 6f64 6528  nse_body.encode(
-00002600: 295d 0d0a 2020 2020 2020 2020 2020 2020  )]..            
-00002610: 656c 6966 2070 6174 682e 7374 6172 7473  elif path.starts
-00002620: 7769 7468 2822 2f22 202b 2073 656c 662e  with("/" + self.
-00002630: 7374 6174 6963 5f64 6972 293a 0d0a 2020  static_dir):..  
-00002640: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-00002650: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
-00002660: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
-00002670: 6e28 7061 7468 5b31 3a5d 2c20 2272 6222  n(path[1:], "rb"
-00002680: 2920 6173 2066 3a0d 0a20 2020 2020 2020  ) as f:..       
-00002690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026a0: 2072 6573 706f 6e73 655f 626f 6479 203d   response_body =
-000026b0: 2066 2e72 6561 6428 290d 0a20 2020 2020   f.read()..     
-000026c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000026d0: 7461 7475 7320 3d20 2232 3030 204f 4b22  tatus = "200 OK"
-000026e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000026f0: 2020 2020 2020 6865 6164 6572 7320 3d20        headers = 
-00002700: 5b28 2243 6f6e 7465 6e74 2d74 7970 6522  [("Content-type"
-00002710: 2c20 2261 7070 6c69 6361 7469 6f6e 2f6f  , "application/o
-00002720: 6374 6574 2d73 7472 6561 6d22 295d 0d0a  ctet-stream")]..
+00000680: 7267 6261 2830 2c20 302c 2030 2c20 3029  rgba(0, 0, 0, 0)
+00000690: 2030 2c0a 2020 2020 2020 2020 2020 2020   0,.            
+000006a0: 2020 2020 2020 2020 7267 6261 2830 2c20          rgba(0, 
+000006b0: 302c 2030 2c20 302e 3329 2035 3025 2c0a  0, 0, 0.3) 50%,.
+000006c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006d0: 2020 2020 7267 6261 2830 2c20 302c 2030      rgba(0, 0, 0
+000006e0: 2c20 3029 2031 3030 2529 3b0a 2020 2020  , 0) 100%);.    
+000006f0: 2020 2020 2020 2020 6261 636b 6772 6f75          backgrou
+00000700: 6e64 2d73 697a 653a 2061 7574 6f20 3470  nd-size: auto 4p
+00000710: 783b 0a20 2020 2020 2020 2020 2020 207a  x;.            z
+00000720: 2d69 6e64 6578 3a20 313b 0a20 2020 2020  -index: 1;.     
+00000730: 2020 207d 0a0a 2020 2020 2020 2020 2e6f     }..        .o
+00000740: 7665 726c 6179 3a3a 6265 666f 7265 207b  verlay::before {
+00000750: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+00000760: 7465 6e74 3a20 2222 3b0a 2020 2020 2020  tent: "";.      
+00000770: 2020 2020 2020 706f 696e 7465 722d 6576        pointer-ev
+00000780: 656e 7473 3a20 6e6f 6e65 3b0a 2020 2020  ents: none;.    
+00000790: 2020 2020 2020 2020 706f 7369 7469 6f6e          position
+000007a0: 3a20 6162 736f 6c75 7465 3b0a 2020 2020  : absolute;.    
+000007b0: 2020 2020 2020 2020 6469 7370 6c61 793a          display:
+000007c0: 2062 6c6f 636b 3b0a 2020 2020 2020 2020   block;.        
+000007d0: 2020 2020 746f 703a 2030 3b0a 2020 2020      top: 0;.    
+000007e0: 2020 2020 2020 2020 6c65 6674 3a20 303b          left: 0;
+000007f0: 0a20 2020 2020 2020 2020 2020 2072 6967  .            rig
+00000800: 6874 3a20 303b 0a20 2020 2020 2020 2020  ht: 0;.         
+00000810: 2020 2062 6f74 746f 6d3a 2030 3b0a 2020     bottom: 0;.  
+00000820: 2020 2020 2020 2020 2020 7769 6474 683a            width:
+00000830: 2031 3030 253b 0a20 2020 2020 2020 2020   100%;.         
+00000840: 2020 2068 6569 6768 743a 2031 3030 253b     height: 100%;
+00000850: 0a20 2020 2020 2020 2020 2020 2062 6163  .            bac
+00000860: 6b67 726f 756e 642d 696d 6167 653a 206c  kground-image: l
+00000870: 696e 6561 722d 6772 6164 6965 6e74 2830  inear-gradient(0
+00000880: 6465 672c 0a20 2020 2020 2020 2020 2020  deg,.           
+00000890: 2020 2020 2020 2020 2074 7261 6e73 7061           transpa
+000008a0: 7265 6e74 2030 252c 0a20 2020 2020 2020  rent 0%,.       
+000008b0: 2020 2020 2020 2020 2020 2020 2072 6762               rgb
+000008c0: 6128 3332 2c20 3132 382c 2033 322c 2030  a(32, 128, 32, 0
+000008d0: 2e32 2920 3225 2c0a 2020 2020 2020 2020  .2) 2%,.        
+000008e0: 2020 2020 2020 2020 2020 2020 7267 6261              rgba
+000008f0: 2833 322c 2031 3238 2c20 3332 2c20 302e  (32, 128, 32, 0.
+00000900: 3829 2033 252c 0a20 2020 2020 2020 2020  8) 3%,.         
+00000910: 2020 2020 2020 2020 2020 2072 6762 6128             rgba(
+00000920: 3332 2c20 3132 382c 2033 322c 2030 2e32  32, 128, 32, 0.2
+00000930: 2920 3325 2c0a 2020 2020 2020 2020 2020  ) 3%,.          
+00000940: 2020 2020 2020 2020 2020 7472 616e 7370            transp
+00000950: 6172 656e 7420 3130 3025 293b 0a20 2020  arent 100%);.   
+00000960: 2020 2020 2020 2020 2062 6163 6b67 726f           backgro
+00000970: 756e 642d 7265 7065 6174 3a20 6e6f 2d72  und-repeat: no-r
+00000980: 6570 6561 743b 0a20 2020 2020 2020 2020  epeat;.         
+00000990: 2020 2061 6e69 6d61 7469 6f6e 3a20 7363     animation: sc
+000009a0: 616e 2037 2e35 7320 6c69 6e65 6172 2030  an 7.5s linear 0
+000009b0: 7320 696e 6669 6e69 7465 3b0a 2020 2020  s infinite;.    
+000009c0: 2020 2020 7d0a 0a20 2020 2020 2020 2040      }..        @
+000009d0: 6b65 7966 7261 6d65 7320 7363 616e 207b  keyframes scan {
+000009e0: 0a20 2020 2020 2020 2020 2020 2030 2520  .            0% 
+000009f0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00000a00: 2020 6261 636b 6772 6f75 6e64 2d70 6f73    background-pos
+00000a10: 6974 696f 6e3a 2030 202d 3130 3076 683b  ition: 0 -100vh;
+00000a20: 0a20 2020 2020 2020 2020 2020 207d 0a0a  .            }..
+00000a30: 2020 2020 2020 2020 2020 2020 3335 252c              35%,
+00000a40: 0a20 2020 2020 2020 2020 2020 2031 3030  .            100
+00000a50: 2520 7b0a 2020 2020 2020 2020 2020 2020  % {.            
+00000a60: 2020 2020 6261 636b 6772 6f75 6e64 2d70      background-p
+00000a70: 6f73 6974 696f 6e3a 2030 2031 3030 7668  osition: 0 100vh
+00000a80: 3b0a 2020 2020 2020 2020 2020 2020 7d0a  ;.            }.
+00000a90: 2020 2020 2020 2020 7d0a 0a20 2020 2020          }..     
+00000aa0: 2020 202e 7465 726d 696e 616c 207b 0a20     .terminal {. 
+00000ab0: 2020 2020 2020 2020 2020 2062 6f78 2d73             box-s
+00000ac0: 697a 696e 673a 2069 6e68 6572 6974 3b0a  izing: inherit;.
+00000ad0: 2020 2020 2020 2020 2020 2020 706f 7369              posi
+00000ae0: 7469 6f6e 3a20 6162 736f 6c75 7465 3b0a  tion: absolute;.
+00000af0: 2020 2020 2020 2020 2020 2020 6865 6967              heig
+00000b00: 6874 3a20 3130 3025 3b0a 2020 2020 2020  ht: 100%;.      
+00000b10: 2020 2020 2020 7769 6474 683a 2031 3030        width: 100
+00000b20: 3070 783b 0a20 2020 2020 2020 2020 2020  0px;.           
+00000b30: 206d 6178 2d77 6964 7468 3a20 3130 3025   max-width: 100%
+00000b40: 3b0a 2020 2020 2020 2020 2020 2020 7061  ;.            pa
+00000b50: 6464 696e 673a 2034 7265 6d3b 0a20 2020  dding: 4rem;.   
+00000b60: 2020 2020 2020 2020 2074 6578 742d 7472           text-tr
+00000b70: 616e 7366 6f72 6d3a 2075 7070 6572 6361  ansform: upperca
+00000b80: 7365 3b0a 2020 2020 2020 2020 7d0a 0a20  se;.        }.. 
+00000b90: 2020 2020 2020 202e 6f75 7470 7574 207b         .output {
+00000ba0: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
+00000bb0: 6f72 3a20 7267 6261 2831 3238 2c20 3235  or: rgba(128, 25
+00000bc0: 352c 2031 3238 2c20 302e 3829 3b0a 2020  5, 128, 0.8);.  
+00000bd0: 2020 2020 2020 2020 2020 7465 7874 2d73            text-s
+00000be0: 6861 646f 773a 0a20 2020 2020 2020 2020  hadow:.         
+00000bf0: 2020 2020 2020 2030 2030 2031 7078 2072         0 0 1px r
+00000c00: 6762 6128 3531 2c20 3235 352c 2035 312c  gba(51, 255, 51,
+00000c10: 2030 2e34 292c 0a20 2020 2020 2020 2020   0.4),.         
+00000c20: 2020 2020 2020 2030 2030 2032 7078 2072         0 0 2px r
+00000c30: 6762 6128 3235 352c 2032 3535 2c20 3235  gba(255, 255, 25
+00000c40: 352c 2030 2e38 293b 0a20 2020 2020 2020  5, 0.8);.       
+00000c50: 207d 0a0a 2020 2020 2020 2020 2e6f 7574   }..        .out
+00000c60: 7075 743a 3a62 6566 6f72 6520 7b0a 2020  put::before {.  
+00000c70: 2020 2020 2020 2020 2020 636f 6e74 656e            conten
+00000c80: 743a 2022 3e20 223b 0a20 2020 2020 2020  t: "> ";.       
+00000c90: 207d 0a0a 2020 2020 2020 2020 6120 7b0a   }..        a {.
+00000ca0: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
+00000cb0: 723a 2023 6666 663b 0a20 2020 2020 2020  r: #fff;.       
+00000cc0: 2020 2020 2074 6578 742d 6465 636f 7261       text-decora
+00000cd0: 7469 6f6e 3a20 6e6f 6e65 3b0a 2020 2020  tion: none;.    
+00000ce0: 2020 2020 7d0a 0a20 2020 2020 2020 2061      }..        a
+00000cf0: 3a3a 6265 666f 7265 207b 0a20 2020 2020  ::before {.     
+00000d00: 2020 2020 2020 2063 6f6e 7465 6e74 3a20         content: 
+00000d10: 225b 223b 0a20 2020 2020 2020 207d 0a0a  "[";.        }..
+00000d20: 2020 2020 2020 2020 613a 3a61 6674 6572          a::after
+00000d30: 207b 0a20 2020 2020 2020 2020 2020 2063   {.            c
+00000d40: 6f6e 7465 6e74 3a20 225d 223b 0a20 2020  ontent: "]";.   
+00000d50: 2020 2020 207d 0a0a 2020 2020 2020 2020       }..        
+00000d60: 2e65 7272 6f72 636f 6465 207b 0a20 2020  .errorcode {.   
+00000d70: 2020 2020 2020 2020 2063 6f6c 6f72 3a20           color: 
+00000d80: 7768 6974 653b 0a20 2020 2020 2020 207d  white;.        }
+00000d90: 0a20 2020 203c 2f73 7479 6c65 3e0a 3c2f  .    </style>.</
+00000da0: 6865 6164 3e0a 0a3c 626f 6479 3e0a 2020  head>..<body>.  
+00000db0: 2020 3c64 6976 2063 6c61 7373 3d22 6e6f    <div class="no
+00000dc0: 6973 6522 3e3c 2f64 6976 3e0a 2020 2020  ise"></div>.    
+00000dd0: 3c64 6976 2063 6c61 7373 3d22 6f76 6572  <div class="over
+00000de0: 6c61 7922 3e3c 2f64 6976 3e0a 2020 2020  lay"></div>.    
+00000df0: 3c64 6976 2063 6c61 7373 3d22 7465 726d  <div class="term
+00000e00: 696e 616c 223e 0a20 2020 2020 2020 203c  inal">.        <
+00000e10: 6831 3e45 7272 6f72 203c 7370 616e 2063  h1>Error <span c
+00000e20: 6c61 7373 3d22 6572 726f 7263 6f64 6522  lass="errorcode"
+00000e30: 3e34 3034 3c2f 7370 616e 3e3c 2f68 313e  >404</span></h1>
+00000e40: 0a20 2020 2020 2020 203c 7020 636c 6173  .        <p clas
+00000e50: 733d 226f 7574 7075 7422 3e54 6865 2070  s="output">The p
+00000e60: 6167 6520 796f 7520 6172 6520 6c6f 6f6b  age you are look
+00000e70: 696e 6720 666f 7220 6d69 6768 7420 6861  ing for might ha
+00000e80: 7665 2062 6565 6e20 7265 6d6f 7665 642c  ve been removed,
+00000e90: 2068 6164 2069 7473 206e 616d 6520 6368   had its name ch
+00000ea0: 616e 6765 6420 6f72 2069 7320 7465 6d70  anged or is temp
+00000eb0: 6f72 6172 696c 790a 2020 2020 2020 2020  orarily.        
+00000ec0: 2020 2020 756e 6176 6169 6c61 626c 652e      unavailable.
+00000ed0: 3c2f 703e 0a20 2020 2020 2020 203c 7020  </p>.        <p 
+00000ee0: 636c 6173 733d 226f 7574 7075 7422 3e50  class="output">P
+00000ef0: 6c65 6173 6520 3c61 2068 7265 663d 222f  lease <a href="/
+00000f00: 223e 7265 7475 726e 2074 6f20 7468 6520  ">return to the 
+00000f10: 686f 6d65 7061 6765 3c2f 613e 2e3c 2f70  homepage</a>.</p
+00000f20: 3e0a 2020 2020 2020 2020 3c70 2063 6c61  >.        <p cla
+00000f30: 7373 3d22 6f75 7470 7574 223e 476f 6f64  ss="output">Good
+00000f40: 206c 7563 6b2e 3c2f 703e 0a20 2020 2020   luck.</p>.     
+00000f50: 2020 203c 7020 636c 6173 733d 226f 7574     <p class="out
+00000f60: 7075 7422 3e43 7265 6469 7473 2074 6f20  put">Credits to 
+00000f70: 3c61 2068 7265 663d 2768 7474 7073 3a2f  <a href='https:/
+00000f80: 2f63 6f64 6570 656e 2e69 6f2f 636f 6465  /codepen.io/code
+00000f90: 3272 6974 6869 6b27 2074 6172 6765 743d  2rithik' target=
+00000fa0: 225f 626c 616e 6b22 3e52 6974 6869 6b20  "_blank">Rithik 
+00000fb0: 5361 6d61 6e74 6875 6c61 2028 4063 6f64  Samanthula (@cod
+00000fc0: 6532 7269 7468 696b 2921 3c2f 613e 3c2f  e2rithik)!</a></
+00000fd0: 703e 0a20 2020 203c 2f64 6976 3e0a 3c2f  p>.    </div>.</
+00000fe0: 626f 6479 3e0a 0a3c 2f68 746d 6c3e 0a22  body>..</html>."
+00000ff0: 2222 0a0a 6630 3020 3d20 2222 220a 3c21  ""..f00 = """.<!
+00001000: 444f 4354 5950 4520 6874 6d6c 3e0a 3c68  DOCTYPE html>.<h
+00001010: 746d 6c20 6c61 6e67 3d22 656e 223e 0a3c  tml lang="en">.<
+00001020: 6865 6164 3e0a 3c73 7479 6c65 3e0a 2a2c  head>.<style>.*,
+00001030: 0a2a 3a3a 6166 7465 722c 0a2a 3a3a 6265  .*::after,.*::be
+00001040: 666f 7265 207b 0a09 626f 782d 7369 7a69  fore {..box-sizi
+00001050: 6e67 3a20 626f 7264 6572 2d62 6f78 3b0a  ng: border-box;.
+00001060: 7d0a 0a68 746d 6c2c 0a62 6f64 7920 7b0a  }..html,.body {.
+00001070: 0961 6c69 676e 2d69 7465 6d73 3a20 6365  .align-items: ce
+00001080: 6e74 6572 3b0a 0962 6163 6b67 726f 756e  nter;..backgroun
+00001090: 643a 206c 696e 6561 722d 6772 6164 6965  d: linear-gradie
+000010a0: 6e74 2823 3030 3365 6666 2c20 2330 3032  nt(#003eff, #002
+000010b0: 3861 3929 3b0a 0963 6f6c 6f72 3a20 7768  8a9);..color: wh
+000010c0: 6974 653b 0a09 6469 7370 6c61 793a 2066  ite;..display: f
+000010d0: 6c65 783b 0a09 666f 6e74 3a20 3272 656d  lex;..font: 2rem
+000010e0: 2022 506f 6972 6574 204f 6e65 223b 0a09   "Poiret One";..
+000010f0: 6865 6967 6874 3a20 3130 3076 683b 0a09  height: 100vh;..
+00001100: 6a75 7374 6966 792d 636f 6e74 656e 743a  justify-content:
+00001110: 2063 656e 7465 723b 0a09 6d61 7267 696e   center;..margin
+00001120: 3a20 303b 0a09 7061 6464 696e 673a 2030  : 0;..padding: 0
+00001130: 3b0a 7d0a 0a2e 626f 7820 7b0a 0968 6569  ;.}...box {..hei
+00001140: 6768 743a 2031 3030 7078 3b0a 096d 6172  ght: 100px;..mar
+00001150: 6769 6e3a 2030 2031 3070 783b 0a09 6f76  gin: 0 10px;..ov
+00001160: 6572 666c 6f77 3a20 6869 6464 656e 3b0a  erflow: hidden;.
+00001170: 0970 6f73 6974 696f 6e3a 2072 656c 6174  .position: relat
+00001180: 6976 653b 0a09 7472 616e 7366 6f72 6d3a  ive;..transform:
+00001190: 2072 6f74 6174 655a 2832 3730 6465 6729   rotateZ(270deg)
+000011a0: 2073 6361 6c65 2831 2e30 3529 3b0a 0977   scale(1.05);..w
+000011b0: 6964 7468 3a20 3130 3070 783b 0a7d 0a0a  idth: 100px;.}..
+000011c0: 2e62 6f78 3a6e 7468 2d6f 662d 7479 7065  .box:nth-of-type
+000011d0: 2832 2920 7b0a 096c 6566 743a 202d 3238  (2) {..left: -28
+000011e0: 7078 3b0a 0974 7261 6e73 666f 726d 3a20  px;..transform: 
+000011f0: 726f 7461 7465 5828 2d31 3830 6465 6729  rotateX(-180deg)
+00001200: 2072 6f74 6174 6559 2831 3830 6465 6729   rotateY(180deg)
+00001210: 2072 6f74 6174 655a 2832 3730 6465 6729   rotateZ(270deg)
+00001220: 2073 6361 6c65 2831 2e30 3529 3b0a 7d0a   scale(1.05);.}.
+00001230: 0a2e 626f 7820 7370 616e 207b 0a09 616e  ..box span {..an
+00001240: 696d 6174 696f 6e3a 206c 6f61 6465 7220  imation: loader 
+00001250: 342e 3873 2069 6e66 696e 6974 6520 626f  4.8s infinite bo
+00001260: 7468 3b0a 0964 6973 706c 6179 3a20 626c  th;..display: bl
+00001270: 6f63 6b3b 0a09 6865 6967 6874 3a20 3130  ock;..height: 10
+00001280: 3025 3b0a 0970 6f73 6974 696f 6e3a 2061  0%;..position: a
+00001290: 6273 6f6c 7574 653b 0a09 7769 6474 683a  bsolute;..width:
+000012a0: 2031 3030 253b 0a7d 0a0a 2e62 6f78 2073   100%;.}...box s
+000012b0: 7061 6e3a 6e74 682d 6368 696c 6428 3129  pan:nth-child(1)
+000012c0: 207b 0a09 616e 696d 6174 696f 6e2d 6465   {..animation-de
+000012d0: 6c61 793a 2030 2e32 733b 0a7d 0a0a 2e62  lay: 0.2s;.}...b
+000012e0: 6f78 2073 7061 6e3a 6e74 682d 6368 696c  ox span:nth-chil
+000012f0: 6428 3229 207b 0a09 616e 696d 6174 696f  d(2) {..animatio
+00001300: 6e2d 6465 6c61 793a 2030 2e34 733b 0a7d  n-delay: 0.4s;.}
+00001310: 0a0a 2e62 6f78 2073 7061 6e3a 6e74 682d  ...box span:nth-
+00001320: 6368 696c 6428 3329 207b 0a09 616e 696d  child(3) {..anim
+00001330: 6174 696f 6e2d 6465 6c61 793a 2030 2e36  ation-delay: 0.6
+00001340: 733b 0a7d 0a0a 2e62 6f78 2073 7061 6e3a  s;.}...box span:
+00001350: 6e74 682d 6368 696c 6428 3429 207b 0a09  nth-child(4) {..
+00001360: 616e 696d 6174 696f 6e2d 6465 6c61 793a  animation-delay:
+00001370: 2030 2e38 733b 0a7d 0a0a 2e62 6f78 2073   0.8s;.}...box s
+00001380: 7061 6e3a 6e74 682d 6368 696c 6428 3529  pan:nth-child(5)
+00001390: 207b 0a09 616e 696d 6174 696f 6e2d 6465   {..animation-de
+000013a0: 6c61 793a 2031 733b 0a7d 0a0a 2e62 6f78  lay: 1s;.}...box
+000013b0: 2073 7061 6e3a 6e74 682d 6368 696c 6428   span:nth-child(
+000013c0: 3629 207b 0a09 616e 696d 6174 696f 6e2d  6) {..animation-
+000013d0: 6465 6c61 793a 2031 2e32 733b 0a7d 0a0a  delay: 1.2s;.}..
+000013e0: 2e62 6f78 2073 7061 6e3a 3a61 6674 6572  .box span::after
+000013f0: 207b 0a09 6261 636b 6772 6f75 6e64 3a20   {..background: 
+00001400: 2366 6666 3b0a 0962 6f72 6465 722d 7261  #fff;..border-ra
+00001410: 6469 7573 3a20 3530 253b 0a09 636f 6e74  dius: 50%;..cont
+00001420: 656e 743a 2022 223b 0a09 6c65 6674 3a20  ent: "";..left: 
+00001430: 3530 253b 0a09 7061 6464 696e 673a 2036  50%;..padding: 6
+00001440: 7078 3b0a 0970 6f73 6974 696f 6e3a 2061  px;..position: a
+00001450: 6273 6f6c 7574 653b 0a09 746f 703a 2030  bsolute;..top: 0
+00001460: 3b0a 0974 7261 6e73 666f 726d 3a20 7472  ;..transform: tr
+00001470: 616e 736c 6174 6558 282d 3530 2529 3b0a  anslateX(-50%);.
+00001480: 7d0a 0a40 6b65 7966 7261 6d65 7320 6c6f  }..@keyframes lo
+00001490: 6164 6572 207b 0a09 3025 207b 0a09 096f  ader {..0% {...o
+000014a0: 7061 6369 7479 3a20 303b 0a09 0974 7261  pacity: 0;...tra
+000014b0: 6e73 666f 726d 3a20 726f 7461 7465 2831  nsform: rotate(1
+000014c0: 3830 6465 6729 3b0a 0909 616e 696d 6174  80deg);...animat
+000014d0: 696f 6e2d 7469 6d69 6e67 2d66 756e 6374  ion-timing-funct
+000014e0: 696f 6e3a 2065 6173 652d 6f75 743b 0a09  ion: ease-out;..
+000014f0: 7d0a 0935 2520 7b0a 0909 6f70 6163 6974  }..5% {...opacit
+00001500: 793a 2031 3b0a 0909 7472 616e 7366 6f72  y: 1;...transfor
+00001510: 6d3a 2072 6f74 6174 6528 3330 3064 6567  m: rotate(300deg
+00001520: 293b 0a09 0961 6e69 6d61 7469 6f6e 2d74  );...animation-t
+00001530: 696d 696e 672d 6675 6e63 7469 6f6e 3a20  iming-function: 
+00001540: 6c69 6e65 6172 3b0a 097d 0a09 3330 2520  linear;..}..30% 
+00001550: 7b0a 0909 7472 616e 7366 6f72 6d3a 2072  {...transform: r
+00001560: 6f74 6174 6528 3432 3064 6567 293b 0a09  otate(420deg);..
+00001570: 0961 6e69 6d61 7469 6f6e 2d74 696d 696e  .animation-timin
+00001580: 672d 6675 6e63 7469 6f6e 3a20 6561 7365  g-function: ease
+00001590: 2d69 6e2d 6f75 743b 0a09 7d0a 0933 3525  -in-out;..}..35%
+000015a0: 207b 0a09 0974 7261 6e73 666f 726d 3a20   {...transform: 
+000015b0: 726f 7461 7465 2836 3235 6465 6729 3b0a  rotate(625deg);.
+000015c0: 0909 616e 696d 6174 696f 6e2d 7469 6d69  ..animation-timi
+000015d0: 6e67 2d66 756e 6374 696f 6e3a 206c 696e  ng-function: lin
+000015e0: 6561 723b 0a09 7d0a 0937 3025 207b 0a09  ear;..}..70% {..
+000015f0: 0974 7261 6e73 666f 726d 3a20 726f 7461  .transform: rota
+00001600: 7465 2838 3030 6465 6729 3b0a 0909 616e  te(800deg);...an
+00001610: 696d 6174 696f 6e2d 7469 6d69 6e67 2d66  imation-timing-f
+00001620: 756e 6374 696f 6e3a 2065 6173 652d 6f75  unction: ease-ou
+00001630: 743b 0a09 096f 7061 6369 7479 3a20 313b  t;...opacity: 1;
+00001640: 0a09 7d0a 0937 3525 207b 0a09 096f 7061  ..}..75% {...opa
+00001650: 6369 7479 3a20 303b 0a09 0974 7261 6e73  city: 0;...trans
+00001660: 666f 726d 3a20 726f 7461 7465 2839 3030  form: rotate(900
+00001670: 6465 6729 3b0a 0909 616e 696d 6174 696f  deg);...animatio
+00001680: 6e2d 7469 6d69 6e67 2d66 756e 6374 696f  n-timing-functio
+00001690: 6e3a 2065 6173 652d 6f75 743b 0a09 7d0a  n: ease-out;..}.
+000016a0: 0937 3625 207b 0a09 096f 7061 6369 7479  .76% {...opacity
+000016b0: 3a20 303b 0a09 0974 7261 6e73 666f 726d  : 0;...transform
+000016c0: 3a20 726f 7461 7465 2839 3030 6465 6729  : rotate(900deg)
+000016d0: 3b0a 097d 0a09 3130 3025 207b 0a09 096f  ;..}..100% {...o
+000016e0: 7061 6369 7479 3a20 303b 0a09 0974 7261  pacity: 0;...tra
+000016f0: 6e73 666f 726d 3a20 726f 7461 7465 2839  nsform: rotate(9
+00001700: 3030 6465 6729 3b0a 097d 0a7d 0a0a 6831  00deg);..}.}..h1
+00001710: 207b 0a09 7465 7874 2d73 6861 646f 773a   {..text-shadow:
+00001720: 2030 2030 2031 3070 7820 2366 6666 3b0a   0 0 10px #fff;.
+00001730: 0961 6e69 6d61 7469 6f6e 3a20 626c 696e  .animation: blin
+00001740: 6b20 342e 3873 2069 6e66 696e 6974 6520  k 4.8s infinite 
+00001750: 626f 7468 3b0a 7d0a 0a68 313a 6e74 682d  both;.}..h1:nth-
+00001760: 6f66 2d74 7970 6528 3229 207b 0a09 616e  of-type(2) {..an
+00001770: 696d 6174 696f 6e3a 206e 6f6e 653b 0a09  imation: none;..
+00001780: 6c65 7474 6572 2d73 7061 6369 6e67 3a20  letter-spacing: 
+00001790: 2d31 3470 783b 0a09 6d61 7267 696e 3a20  -14px;..margin: 
+000017a0: 3020 6175 746f 3b0a 096f 7061 6369 7479  0 auto;..opacity
+000017b0: 3a20 302e 313b 0a09 7061 6464 696e 672d  : 0.1;..padding-
+000017c0: 6c65 6674 3a20 3431 7078 3b0a 0970 6f73  left: 41px;..pos
+000017d0: 6974 696f 6e3a 2061 6273 6f6c 7574 653b  ition: absolute;
+000017e0: 0a09 746f 703a 2035 3025 3b0a 0974 7261  ..top: 50%;..tra
+000017f0: 6e73 666f 726d 3a20 7472 616e 736c 6174  nsform: translat
+00001800: 6579 282d 3530 2529 3b0a 7d0a 0a40 6b65  ey(-50%);.}..@ke
+00001810: 7966 7261 6d65 7320 626c 696e 6b20 7b0a  yframes blink {.
+00001820: 0930 252c 0a09 3530 252c 0a09 3130 3025  .0%,..50%,..100%
+00001830: 207b 0a09 096f 7061 6369 7479 3a20 302e   {...opacity: 0.
+00001840: 323b 0a09 7d0a 0932 3525 2c0a 0937 3525  2;..}..25%,..75%
+00001850: 207b 0a09 096f 7061 6369 7479 3a20 313b   {...opacity: 1;
+00001860: 0a09 7d0a 7d0a 0a68 352c 0a70 207b 0a09  ..}.}..h5,.p {..
+00001870: 706f 7369 7469 6f6e 3a20 6162 736f 6c75  position: absolu
+00001880: 7465 3b0a 0966 6f6e 742d 6661 6d69 6c79  te;..font-family
+00001890: 3a20 6d6f 6e6f 7370 6163 653b 0a7d 0a0a  : monospace;.}..
+000018a0: 6835 207b 0a09 746f 703a 2031 3025 3b0a  h5 {..top: 10%;.
+000018b0: 0966 6f6e 742d 7369 7a65 3a20 302e 3465  .font-size: 0.4e
+000018c0: 6d3b 0a09 0a7d 0a0a 7020 7b0a 0966 6f6e  m;...}..p {..fon
+000018d0: 742d 7369 7a65 3a20 302e 3365 6d3b 0a09  t-size: 0.3em;..
+000018e0: 626f 7474 6f6d 3a20 3130 253b 0a09 7769  bottom: 10%;..wi
+000018f0: 6474 683a 2035 3025 3b0a 0974 6578 742d  dth: 50%;..text-
+00001900: 616c 6967 6e3a 2063 656e 7465 723b 0a7d  align: center;.}
+00001910: 0a0a 7020 6120 7b0a 0963 6f6c 6f72 3a20  ..p a {..color: 
+00001920: 6379 616e 3b0a 7d0a 0a3c 2f73 7479 6c65  cyan;.}..</style
+00001930: 3e0a 3c2f 6865 6164 3e0a 3c62 6f64 793e  >.</head>.<body>
+00001940: 0a3c 6835 3e49 6e74 6572 6e61 6c20 5365  .<h5>Internal Se
+00001950: 7276 6572 2065 7272 6f72 2021 3c2f 6835  rver error !</h5
+00001960: 3e0a 2020 2020 3c68 313e 353c 2f68 313e  >.    <h1>5</h1>
+00001970: 0a20 2020 203c 6831 3e30 303c 2f68 313e  .    <h1>00</h1>
+00001980: 0a20 2020 203c 6469 7620 636c 6173 733d  .    <div class=
+00001990: 2262 6f78 223e 0a09 0909 3c73 7061 6e3e  "box">....<span>
+000019a0: 3c2f 7370 616e 3e3c 7370 616e 3e3c 2f73  </span><span></s
+000019b0: 7061 6e3e 0a09 0909 3c73 7061 6e3e 3c2f  pan>....<span></
+000019c0: 7370 616e 3e3c 7370 616e 3e3c 2f73 7061  span><span></spa
+000019d0: 6e3e 0a09 0909 3c73 7061 6e3e 3c2f 7370  n>....<span></sp
+000019e0: 616e 3e0a 0909 3c2f 6469 763e 0a20 2020  an>...</div>.   
+000019f0: 203c 6469 7620 636c 6173 733d 2262 6f78   <div class="box
+00001a00: 223e 0a09 0909 3c73 7061 6e3e 3c2f 7370  ">....<span></sp
+00001a10: 616e 3e3c 7370 616e 3e3c 2f73 7061 6e3e  an><span></span>
+00001a20: 0a09 0909 3c73 7061 6e3e 3c2f 7370 616e  ....<span></span
+00001a30: 3e3c 7370 616e 3e3c 2f73 7061 6e3e 0a09  ><span></span>..
+00001a40: 0909 3c73 7061 6e3e 3c2f 7370 616e 3e0a  ..<span></span>.
+00001a50: 0909 3c2f 6469 763e 0a20 2020 203c 703e  ..</div>.    <p>
+00001a60: 2057 6527 7265 2075 6e61 626c 6520 746f   We're unable to
+00001a70: 2066 696e 6420 6f75 7420 7768 6174 2773   find out what's
+00001a80: 2068 6170 7065 6e69 6e67 2120 5765 2073   happening! We s
+00001a90: 7567 6765 7374 2079 6f75 2074 6f0a 0909  uggest you to...
+00001aa0: 093c 6272 2f3e 0a09 0909 3c61 2068 7265  .<br/>....<a hre
+00001ab0: 663d 222f 223e 476f 2048 6f6d 653c 2f61  f="/">Go Home</a
+00001ac0: 3e0a 0909 096f 7220 7669 7369 7420 6865  >....or visit he
+00001ad0: 7265 206c 6174 6572 2e20 4372 6564 6974  re later. Credit
+00001ae0: 7320 746f 203c 6120 6872 6566 3d27 6874  s to <a href='ht
+00001af0: 7470 733a 2f2f 636f 6465 7065 6e2e 696f  tps://codepen.io
+00001b00: 2f61 6473 696e 6768 3134 2720 7461 7267  /adsingh14' targ
+00001b10: 6574 3d22 5f62 6c61 6e6b 223e 414d 414e  et="_blank">AMAN
+00001b20: 2028 4061 6473 696e 6768 3134 2921 3c2f   (@adsingh14)!</
+00001b30: 613e 3c2f 703e 0a3c 2f62 6f64 793e 0a3c  a></p>.</body>.<
+00001b40: 2f68 746d 6c3e 0a22 2222 0a0a 0a63 6c61  /html>."""...cla
+00001b50: 7373 2053 6974 6550 793a 0a20 2020 2064  ss SitePy:.    d
+00001b60: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+00001b70: 2020 2020 2073 656c 662c 2073 7461 7469       self, stati
+00001b80: 635f 6469 723d 2273 7461 7469 6322 2c20  c_dir="static", 
+00001b90: 7465 6d70 6c61 7465 735f 6469 723d 2274  templates_dir="t
+00001ba0: 656d 706c 6174 6573 222c 2063 7573 746f  emplates", custo
+00001bb0: 6d5f 3430 345f 7061 6765 3d4e 6f6e 652c  m_404_page=None,
+00001bc0: 2063 7573 746f 6d5f 3530 305f 7061 6765   custom_500_page
+00001bd0: 3d4e 6f6e 650a 2020 2020 293a 0a20 2020  =None.    ):.   
+00001be0: 2020 2020 2073 656c 662e 726f 7574 6573       self.routes
+00001bf0: 203d 207b 7d0a 2020 2020 2020 2020 7365   = {}.        se
+00001c00: 6c66 2e6d 6964 646c 6577 6172 6520 3d20  lf.middleware = 
+00001c10: 5b73 656c 662e 6c6f 6767 6572 5f6d 6964  [self.logger_mid
+00001c20: 646c 6577 6172 655d 0a20 2020 2020 2020  dleware].       
+00001c30: 2073 656c 662e 7374 6174 6963 5f64 6972   self.static_dir
+00001c40: 203d 2073 7461 7469 635f 6469 720a 2020   = static_dir.  
+00001c50: 2020 2020 2020 7365 6c66 2e74 656d 706c        self.templ
+00001c60: 6174 6573 5f64 6972 203d 2074 656d 706c  ates_dir = templ
+00001c70: 6174 6573 5f64 6972 0a20 2020 2020 2020  ates_dir.       
+00001c80: 2073 656c 662e 6375 7374 6f6d 5f34 3034   self.custom_404
+00001c90: 5f70 6167 6520 3d20 6375 7374 6f6d 5f34  _page = custom_4
+00001ca0: 3034 5f70 6167 650a 2020 2020 2020 2020  04_page.        
+00001cb0: 7365 6c66 2e63 7573 746f 6d5f 3530 305f  self.custom_500_
+00001cc0: 7061 6765 203d 2063 7573 746f 6d5f 3530  page = custom_50
+00001cd0: 305f 7061 6765 0a0a 2020 2020 6465 6620  0_page..    def 
+00001ce0: 7265 6e64 6572 5f74 656d 706c 6174 6528  render_template(
+00001cf0: 7365 6c66 2c20 7465 6d70 6c61 7465 5f6e  self, template_n
+00001d00: 616d 652c 202a 2a63 6f6e 7465 7874 293a  ame, **context):
+00001d10: 0a20 2020 2020 2020 2065 6e76 203d 2045  .        env = E
+00001d20: 6e76 6972 6f6e 6d65 6e74 286c 6f61 6465  nvironment(loade
+00001d30: 723d 4669 6c65 5379 7374 656d 4c6f 6164  r=FileSystemLoad
+00001d40: 6572 2873 656c 662e 7465 6d70 6c61 7465  er(self.template
+00001d50: 735f 6469 7229 290a 2020 2020 2020 2020  s_dir)).        
+00001d60: 7465 6d70 6c61 7465 203d 2065 6e76 2e67  template = env.g
+00001d70: 6574 5f74 656d 706c 6174 6528 7465 6d70  et_template(temp
+00001d80: 6c61 7465 5f6e 616d 6529 0a20 2020 2020  late_name).     
+00001d90: 2020 2072 6574 7572 6e20 7465 6d70 6c61     return templa
+00001da0: 7465 2e72 656e 6465 7228 2a2a 636f 6e74  te.render(**cont
+00001db0: 6578 7429 0a0a 2020 2020 6465 6620 726f  ext)..    def ro
+00001dc0: 7574 6528 7365 6c66 2c20 7061 7468 2c20  ute(self, path, 
+00001dd0: 6d65 7468 6f64 733d 5b22 4745 5422 5d29  methods=["GET"])
+00001de0: 3a0a 2020 2020 2020 2020 6465 6620 7772  :.        def wr
+00001df0: 6170 7065 7228 6861 6e64 6c65 7229 3a0a  apper(handler):.
+00001e00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00001e10: 2e72 6f75 7465 735b 2870 6174 682c 2074  .routes[(path, t
+00001e20: 7570 6c65 286d 6574 686f 6473 2929 5d20  uple(methods))] 
+00001e30: 3d20 6861 6e64 6c65 720a 2020 2020 2020  = handler.      
+00001e40: 2020 2020 2020 7265 7475 726e 2068 616e        return han
+00001e50: 646c 6572 0a0a 2020 2020 2020 2020 7265  dler..        re
+00001e60: 7475 726e 2077 7261 7070 6572 0a0a 2020  turn wrapper..  
+00001e70: 2020 6465 6620 7573 6528 7365 6c66 2c20    def use(self, 
+00001e80: 6d69 6464 6c65 7761 7265 293a 0a20 2020  middleware):.   
+00001e90: 2020 2020 2073 656c 662e 6d69 6464 6c65       self.middle
+00001ea0: 7761 7265 2e61 7070 656e 6428 6d69 6464  ware.append(midd
+00001eb0: 6c65 7761 7265 290a 0a20 2020 2064 6566  leware)..    def
+00001ec0: 206c 6f67 6765 725f 6d69 6464 6c65 7761   logger_middlewa
+00001ed0: 7265 2873 656c 662c 2065 6e76 6972 6f6e  re(self, environ
+00001ee0: 293a 0a20 2020 2020 2020 2070 7269 6e74  ):.        print
+00001ef0: 2866 2252 6571 7565 7374 2072 6563 6569  (f"Request recei
+00001f00: 7665 6420 666f 7220 7b65 6e76 6972 6f6e  ved for {environ
+00001f10: 5b27 5041 5448 5f49 4e46 4f27 5d7d 2229  ['PATH_INFO']}")
+00001f20: 0a0a 2020 2020 6465 6620 5f5f 6361 6c6c  ..    def __call
+00001f30: 5f5f 2873 656c 662c 2065 6e76 6972 6f6e  __(self, environ
+00001f40: 2c20 7374 6172 745f 7265 7370 6f6e 7365  , start_response
+00001f50: 293a 0a20 2020 2020 2020 2074 7279 3a0a  ):.        try:.
+00001f60: 2020 2020 2020 2020 2020 2020 7061 7468              path
+00001f70: 203d 2065 6e76 6972 6f6e 5b22 5041 5448   = environ["PATH
+00001f80: 5f49 4e46 4f22 5d0a 2020 2020 2020 2020  _INFO"].        
+00001f90: 2020 2020 6d65 7468 6f64 203d 2065 6e76      method = env
+00001fa0: 6972 6f6e 5b22 5245 5155 4553 545f 4d45  iron["REQUEST_ME
+00001fb0: 5448 4f44 225d 0a20 2020 2020 2020 2020  THOD"].         
+00001fc0: 2020 2066 6f72 206d 6964 646c 6577 6172     for middlewar
+00001fd0: 6520 696e 2073 656c 662e 6d69 6464 6c65  e in self.middle
+00001fe0: 7761 7265 3a0a 2020 2020 2020 2020 2020  ware:.          
+00001ff0: 2020 2020 2020 6d69 6464 6c65 7761 7265        middleware
+00002000: 2865 6e76 6972 6f6e 290a 2020 2020 2020  (environ).      
+00002010: 2020 2020 2020 6861 6e64 6c65 7220 3d20        handler = 
+00002020: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+00002030: 2066 6f72 2072 6f75 7465 2c20 6d65 7468   for route, meth
+00002040: 6f64 7320 696e 2073 656c 662e 726f 7574  ods in self.rout
+00002050: 6573 2e6b 6579 7328 293a 0a20 2020 2020  es.keys():.     
+00002060: 2020 2020 2020 2020 2020 206d 6174 6368             match
+00002070: 203d 2072 6f75 7465 2e6d 6174 6368 2870   = route.match(p
+00002080: 6174 6829 0a20 2020 2020 2020 2020 2020  ath).           
+00002090: 2020 2020 2069 6620 6d61 7463 6820 616e       if match an
+000020a0: 6420 6d65 7468 6f64 2069 6e20 6d65 7468  d method in meth
+000020b0: 6f64 733a 0a20 2020 2020 2020 2020 2020  ods:.           
+000020c0: 2020 2020 2020 2020 2068 616e 646c 6572           handler
+000020d0: 203d 2073 656c 662e 726f 7574 6573 5b28   = self.routes[(
+000020e0: 726f 7574 652c 206d 6574 686f 6473 295d  route, methods)]
+000020f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002100: 2020 2020 2070 6172 616d 7320 3d20 6d61       params = ma
+00002110: 7463 682e 6772 6f75 7064 6963 7428 290a  tch.groupdict().
+00002120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002130: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
+00002140: 2020 2020 2020 6966 2068 616e 646c 6572        if handler
+00002150: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00002160: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00002170: 2020 2020 2020 2020 2020 2072 6571 7565             reque
+00002180: 7374 5f62 6f64 795f 7369 7a65 203d 2069  st_body_size = i
+00002190: 6e74 2865 6e76 6972 6f6e 2e67 6574 2822  nt(environ.get("
+000021a0: 434f 4e54 454e 545f 4c45 4e47 5448 222c  CONTENT_LENGTH",
+000021b0: 2030 2929 0a20 2020 2020 2020 2020 2020   0)).           
+000021c0: 2020 2020 2065 7863 6570 7420 5661 6c75       except Valu
+000021d0: 6545 7272 6f72 3a0a 2020 2020 2020 2020  eError:.        
+000021e0: 2020 2020 2020 2020 2020 2020 7265 7175              requ
+000021f0: 6573 745f 626f 6479 5f73 697a 6520 3d20  est_body_size = 
+00002200: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
+00002210: 2020 7265 7175 6573 745f 626f 6479 203d    request_body =
+00002220: 2065 6e76 6972 6f6e 5b22 7773 6769 2e69   environ["wsgi.i
+00002230: 6e70 7574 225d 2e72 6561 6428 7265 7175  nput"].read(requ
+00002240: 6573 745f 626f 6479 5f73 697a 6529 0a20  est_body_size). 
+00002250: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00002260: 6f64 795f 7061 7261 6d73 203d 2070 6172  ody_params = par
+00002270: 7365 5f71 7328 7265 7175 6573 745f 626f  se_qs(request_bo
+00002280: 6479 2e64 6563 6f64 6528 2929 2069 6620  dy.decode()) if 
+00002290: 7265 7175 6573 745f 626f 6479 2065 6c73  request_body els
+000022a0: 6520 7b7d 0a20 2020 2020 2020 2020 2020  e {}.           
+000022b0: 2020 2020 2070 6172 616d 7320 3d20 7061       params = pa
+000022c0: 7273 655f 7173 2872 6571 7565 7374 5f62  rse_qs(request_b
+000022d0: 6f64 792e 6465 636f 6465 2829 2920 6966  ody.decode()) if
+000022e0: 2072 6571 7565 7374 5f62 6f64 7920 656c   request_body el
+000022f0: 7365 207b 7d0a 2020 2020 2020 2020 2020  se {}.          
+00002300: 2020 2020 2020 7061 7261 6d73 2e75 7064        params.upd
+00002310: 6174 6528 626f 6479 5f70 6172 616d 7329  ate(body_params)
+00002320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002330: 2068 616e 646c 6572 5f61 7267 7320 3d20   handler_args = 
+00002340: 696e 7370 6563 742e 7369 676e 6174 7572  inspect.signatur
+00002350: 6528 6861 6e64 6c65 7229 2e70 6172 616d  e(handler).param
+00002360: 6574 6572 730a 2020 2020 2020 2020 2020  eters.          
+00002370: 2020 2020 2020 7265 7370 6f6e 7365 5f62        response_b
+00002380: 6f64 7920 3d20 6861 6e64 6c65 7228 7061  ody = handler(pa
+00002390: 7261 6d73 2920 6966 2068 616e 646c 6572  rams) if handler
+000023a0: 5f61 7267 7320 656c 7365 2068 616e 646c  _args else handl
+000023b0: 6572 2829 0a20 2020 2020 2020 2020 2020  er().           
+000023c0: 2020 2020 2073 7461 7475 7320 3d20 2232       status = "2
+000023d0: 3030 204f 4b22 0a20 2020 2020 2020 2020  00 OK".         
+000023e0: 2020 2020 2020 2068 6561 6465 7273 203d         headers =
+000023f0: 205b 2822 436f 6e74 656e 742d 7479 7065   [("Content-type
+00002400: 222c 2022 7465 7874 2f68 746d 6c22 295d  ", "text/html")]
+00002410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002420: 2073 7461 7274 5f72 6573 706f 6e73 6528   start_response(
+00002430: 7374 6174 7573 2c20 6865 6164 6572 7329  status, headers)
+00002440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002450: 2072 6574 7572 6e20 5b72 6573 706f 6e73   return [respons
+00002460: 655f 626f 6479 2e65 6e63 6f64 6528 295d  e_body.encode()]
+00002470: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+00002480: 6620 7061 7468 2e73 7461 7274 7377 6974  f path.startswit
+00002490: 6828 222f 2220 2b20 7365 6c66 2e73 7461  h("/" + self.sta
+000024a0: 7469 635f 6469 7229 3a0a 2020 2020 2020  tic_dir):.      
+000024b0: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+000024c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024d0: 2020 2077 6974 6820 6f70 656e 2870 6174     with open(pat
+000024e0: 685b 313a 5d2c 2022 7262 2229 2061 7320  h[1:], "rb") as 
+000024f0: 663a 0a20 2020 2020 2020 2020 2020 2020  f:.             
+00002500: 2020 2020 2020 2020 2020 2072 6573 706f             respo
+00002510: 6e73 655f 626f 6479 203d 2066 2e72 6561  nse_body = f.rea
+00002520: 6428 290a 2020 2020 2020 2020 2020 2020  d().            
+00002530: 2020 2020 2020 2020 7374 6174 7573 203d          status =
+00002540: 2022 3230 3020 4f4b 220a 2020 2020 2020   "200 OK".      
+00002550: 2020 2020 2020 2020 2020 2020 2020 6865                he
+00002560: 6164 6572 7320 3d20 5b28 2243 6f6e 7465  aders = [("Conte
+00002570: 6e74 2d74 7970 6522 2c20 2261 7070 6c69  nt-type", "appli
+00002580: 6361 7469 6f6e 2f6f 6374 6574 2d73 7472  cation/octet-str
+00002590: 6561 6d22 295d 0a20 2020 2020 2020 2020  eam")].         
+000025a0: 2020 2020 2020 2020 2020 2073 7461 7274             start
+000025b0: 5f72 6573 706f 6e73 6528 7374 6174 7573  _response(status
+000025c0: 2c20 6865 6164 6572 7329 0a20 2020 2020  , headers).     
+000025d0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000025e0: 6574 7572 6e20 5b72 6573 706f 6e73 655f  eturn [response_
+000025f0: 626f 6479 5d0a 2020 2020 2020 2020 2020  body].          
+00002600: 2020 2020 2020 6578 6365 7074 2046 696c        except Fil
+00002610: 654e 6f74 466f 756e 6445 7272 6f72 3a0a  eNotFoundError:.
+00002620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002630: 2020 2020 7374 6174 7573 203d 2022 3430      status = "40
+00002640: 3420 4e4f 5420 464f 554e 4422 0a20 2020  4 NOT FOUND".   
+00002650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002660: 2068 6561 6465 7273 203d 205b 2822 436f   headers = [("Co
+00002670: 6e74 656e 742d 7479 7065 222c 2022 7465  ntent-type", "te
+00002680: 7874 2f68 746d 6c22 295d 0a20 2020 2020  xt/html")].     
+00002690: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000026a0: 7461 7274 5f72 6573 706f 6e73 6528 7374  tart_response(st
+000026b0: 6174 7573 2c20 6865 6164 6572 7329 0a20  atus, headers). 
+000026c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026d0: 2020 2072 6574 7572 6e20 5b0a 2020 2020     return [.    
+000026e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026f0: 2020 2020 280a 2020 2020 2020 2020 2020      (.          
+00002700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002710: 2020 7365 6c66 2e63 7573 746f 6d5f 3430    self.custom_40
+00002720: 345f 7061 6765 2e65 6e63 6f64 6528 290a  4_page.encode().
 00002730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002740: 2020 2020 7374 6172 745f 7265 7370 6f6e      start_respon
-00002750: 7365 2873 7461 7475 732c 2068 6561 6465  se(status, heade
-00002760: 7273 290d 0a20 2020 2020 2020 2020 2020  rs)..           
-00002770: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00002780: 5b72 6573 706f 6e73 655f 626f 6479 5d0d  [response_body].
-00002790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000027a0: 2065 7863 6570 7420 4669 6c65 4e6f 7446   except FileNotF
-000027b0: 6f75 6e64 4572 726f 723a 0d0a 2020 2020  oundError:..    
-000027c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027d0: 7374 6174 7573 203d 2022 3430 3420 4e4f  status = "404 NO
-000027e0: 5420 464f 554e 4422 0d0a 2020 2020 2020  T FOUND"..      
-000027f0: 2020 2020 2020 2020 2020 2020 2020 6865                he
-00002800: 6164 6572 7320 3d20 5b28 2243 6f6e 7465  aders = [("Conte
-00002810: 6e74 2d74 7970 6522 2c20 2274 6578 742f  nt-type", "text/
-00002820: 6874 6d6c 2229 5d0d 0a20 2020 2020 2020  html")]..       
-00002830: 2020 2020 2020 2020 2020 2020 2073 7461               sta
-00002840: 7274 5f72 6573 706f 6e73 6528 7374 6174  rt_response(stat
-00002850: 7573 2c20 6865 6164 6572 7329 0d0a 2020  us, headers)..  
-00002860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002870: 2020 7265 7475 726e 205b 0d0a 2020 2020    return [..    
+00002740: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00002750: 656c 662e 6375 7374 6f6d 5f34 3034 5f70  elf.custom_404_p
+00002760: 6167 650a 2020 2020 2020 2020 2020 2020  age.            
+00002770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002780: 656c 7365 2066 6f66 2e65 6e63 6f64 6528  else fof.encode(
+00002790: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000027a0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+000027b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027c0: 5d0a 2020 2020 2020 2020 2020 2020 656c  ].            el
+000027d0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000027e0: 2020 2020 7374 6174 7573 203d 2022 3430      status = "40
+000027f0: 3420 4e4f 5420 464f 554e 4422 0a20 2020  4 NOT FOUND".   
+00002800: 2020 2020 2020 2020 2020 2020 2068 6561               hea
+00002810: 6465 7273 203d 205b 2822 436f 6e74 656e  ders = [("Conten
+00002820: 742d 7479 7065 222c 2022 7465 7874 2f68  t-type", "text/h
+00002830: 746d 6c22 295d 0a20 2020 2020 2020 2020  tml")].         
+00002840: 2020 2020 2020 2073 7461 7274 5f72 6573         start_res
+00002850: 706f 6e73 6528 7374 6174 7573 2c20 6865  ponse(status, he
+00002860: 6164 6572 7329 0a20 2020 2020 2020 2020  aders).         
+00002870: 2020 2020 2020 2072 6574 7572 6e20 5b0a         return [.
 00002880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002890: 2020 2020 280d 0a20 2020 2020 2020 2020      (..         
-000028a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028b0: 2020 2073 656c 662e 6375 7374 6f6d 5f34     self.custom_4
-000028c0: 3034 5f70 6167 652e 656e 636f 6465 2829  04_page.encode()
-000028d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000028e0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000028f0: 2073 656c 662e 6375 7374 6f6d 5f34 3034   self.custom_404
-00002900: 5f70 6167 650d 0a20 2020 2020 2020 2020  _page..         
-00002910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002920: 2020 2065 6c73 6520 666f 662e 656e 636f     else fof.enco
-00002930: 6465 2829 0d0a 2020 2020 2020 2020 2020  de()..          
-00002940: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-00002950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002960: 2020 2020 205d 0d0a 2020 2020 2020 2020       ]..        
-00002970: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00002980: 2020 2020 2020 2020 2020 2073 7461 7475             statu
-00002990: 7320 3d20 2234 3034 204e 4f54 2046 4f55  s = "404 NOT FOU
-000029a0: 4e44 220d 0a20 2020 2020 2020 2020 2020  ND"..           
-000029b0: 2020 2020 2068 6561 6465 7273 203d 205b       headers = [
-000029c0: 2822 436f 6e74 656e 742d 7479 7065 222c  ("Content-type",
-000029d0: 2022 7465 7874 2f68 746d 6c22 295d 0d0a   "text/html")]..
-000029e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029f0: 7374 6172 745f 7265 7370 6f6e 7365 2873  start_response(s
-00002a00: 7461 7475 732c 2068 6561 6465 7273 290d  tatus, headers).
-00002a10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002a20: 2072 6574 7572 6e20 5b0d 0a20 2020 2020   return [..     
-00002a30: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-00002a40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002a50: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-00002a60: 7573 746f 6d5f 3430 345f 7061 6765 2e65  ustom_404_page.e
-00002a70: 6e63 6f64 6528 290d 0a20 2020 2020 2020  ncode()..       
-00002a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a90: 2069 6620 7365 6c66 2e63 7573 746f 6d5f   if self.custom_
-00002aa0: 3430 345f 7061 6765 0d0a 2020 2020 2020  404_page..      
-00002ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ac0: 2020 656c 7365 2066 6f66 2e65 6e63 6f64    else fof.encod
-00002ad0: 6528 290d 0a20 2020 2020 2020 2020 2020  e()..           
-00002ae0: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-00002af0: 2020 2020 2020 2020 2020 2020 5d0d 0a20              ].. 
-00002b00: 2020 2020 2020 2065 7863 6570 7420 4b65         except Ke
-00002b10: 7962 6f61 7264 496e 7465 7272 7570 743a  yboardInterrupt:
-00002b20: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-00002b30: 696e 7428 225c 6e53 6572 7665 7220 7368  int("\nServer sh
-00002b40: 7574 7469 6e67 2064 6f77 6e2e 2e2e 2229  utting down...")
-00002b50: 0d0a 2020 2020 2020 2020 6578 6365 7074  ..        except
-00002b60: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
-00002b70: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
-00002b80: 6174 7573 203d 2022 3530 3020 494e 5445  atus = "500 INTE
-00002b90: 524e 414c 2053 4552 5645 5220 4552 524f  RNAL SERVER ERRO
-00002ba0: 5222 0d0a 2020 2020 2020 2020 2020 2020  R"..            
-00002bb0: 6865 6164 6572 7320 3d20 5b28 2243 6f6e  headers = [("Con
-00002bc0: 7465 6e74 2d74 7970 6522 2c20 2274 6578  tent-type", "tex
-00002bd0: 742f 6874 6d6c 2229 5d0d 0a20 2020 2020  t/html")]..     
-00002be0: 2020 2020 2020 2073 7461 7274 5f72 6573         start_res
-00002bf0: 706f 6e73 6528 7374 6174 7573 2c20 6865  ponse(status, he
-00002c00: 6164 6572 7329 0d0a 2020 2020 2020 2020  aders)..        
-00002c10: 2020 2020 7072 696e 7428 6529 0d0a 2020      print(e)..  
-00002c20: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00002c30: 205b 0d0a 2020 2020 2020 2020 2020 2020   [..            
-00002c40: 2020 2020 280d 0a20 2020 2020 2020 2020      (..         
-00002c50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00002c60: 6375 7374 6f6d 5f35 3030 5f70 6167 652e  custom_500_page.
-00002c70: 656e 636f 6465 2829 0d0a 2020 2020 2020  encode()..      
-00002c80: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00002c90: 2073 656c 662e 6375 7374 6f6d 5f35 3030   self.custom_500
-00002ca0: 5f70 6167 650d 0a20 2020 2020 2020 2020  _page..         
-00002cb0: 2020 2020 2020 2020 2020 2065 6c73 6520             else 
-00002cc0: 6630 302e 656e 636f 6465 2829 0d0a 2020  f00.encode()..  
-00002cd0: 2020 2020 2020 2020 2020 2020 2020 290d                ).
-00002ce0: 0a20 2020 2020 2020 2020 2020 205d 0d0a  .            ]..
-00002cf0: 2020 2020 0d0a 2020 2020 6465 6620 6a73      ..    def js
-00002d00: 6f6e 5f72 6573 706f 6e73 6528 7365 6c66  on_response(self
-00002d10: 2c20 6461 7461 293a 0d0a 2020 2020 2020  , data):..      
-00002d20: 2020 696d 706f 7274 206a 736f 6e0d 0a20    import json.. 
-00002d30: 2020 2020 2020 2072 6573 706f 6e73 655f         response_
-00002d40: 626f 6479 203d 206a 736f 6e2e 6475 6d70  body = json.dump
-00002d50: 7328 6461 7461 290d 0a20 2020 2020 2020  s(data)..       
-00002d60: 2064 6566 2072 6573 706f 6e73 6528 7374   def response(st
-00002d70: 6172 745f 7265 7370 6f6e 7365 293a 0d0a  art_response):..
-00002d80: 2020 2020 2020 2020 2020 2020 7374 6174              stat
-00002d90: 7573 203d 2022 3230 3020 4f4b 220d 0a20  us = "200 OK".. 
-00002da0: 2020 2020 2020 2020 2020 2068 6561 6465             heade
-00002db0: 7273 203d 205b 2822 436f 6e74 656e 742d  rs = [("Content-
-00002dc0: 7479 7065 222c 2022 6170 706c 6963 6174  type", "applicat
-00002dd0: 696f 6e2f 6a73 6f6e 2229 5d0d 0a20 2020  ion/json")]..   
-00002de0: 2020 2020 2020 2020 2073 7461 7274 5f72           start_r
-00002df0: 6573 706f 6e73 6528 7374 6174 7573 2c20  esponse(status, 
-00002e00: 6865 6164 6572 7329 0d0a 2020 2020 2020  headers)..      
-00002e10: 2020 2020 2020 7265 7475 726e 205b 7265        return [re
-00002e20: 7370 6f6e 7365 5f62 6f64 792e 656e 636f  sponse_body.enco
-00002e30: 6465 2829 5d0d 0a20 2020 2020 2020 2072  de()]..        r
-00002e40: 6574 7572 6e20 7265 7370 6f6e 7365 0d0a  eturn response..
-00002e50: 0d0a 2020 2020 6465 6620 7275 6e28 7365  ..    def run(se
-00002e60: 6c66 2c20 686f 7374 3d22 6c6f 6361 6c68  lf, host="localh
-00002e70: 6f73 7422 2c20 706f 7274 3d38 3038 3029  ost", port=8080)
-00002e80: 3a0d 0a20 2020 2020 2020 2074 7279 3a0d  :..        try:.
-00002e90: 0a20 2020 2020 2020 2020 2020 2073 6572  .            ser
-00002ea0: 7665 7220 3d20 6d61 6b65 5f73 6572 7665  ver = make_serve
-00002eb0: 7228 686f 7374 2c20 706f 7274 2c20 7365  r(host, port, se
-00002ec0: 6c66 290d 0a20 2020 2020 2020 2020 2020  lf)..           
-00002ed0: 2070 7269 6e74 2866 2253 6572 7669 6e67   print(f"Serving
-00002ee0: 206f 6e20 7b68 6f73 747d 3a7b 706f 7274   on {host}:{port
-00002ef0: 7d22 290d 0a20 2020 2020 2020 2020 2020  }")..           
-00002f00: 2073 6572 7665 722e 7365 7276 655f 666f   server.serve_fo
-00002f10: 7265 7665 7228 290d 0a20 2020 2020 2020  rever()..       
-00002f20: 2065 7863 6570 7420 4b65 7962 6f61 7264   except Keyboard
-00002f30: 496e 7465 7272 7570 743a 0d0a 2020 2020  Interrupt:..    
-00002f40: 2020 2020 2020 2020 7072 696e 7428 225c          print("\
-00002f50: 6e53 6572 7665 7220 7368 7574 7469 6e67  nServer shutting
-00002f60: 2064 6f77 6e2e 2e2e 2229 0d0a 2020 2020   down...")..    
-00002f70: 2020 2020 2020 2020 7365 7276 6572 2e73          server.s
-00002f80: 6572 7665 725f 636c 6f73 6528 290d 0a    erver_close()..
+00002890: 2020 2020 280a 2020 2020 2020 2020 2020      (.          
+000028a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000028b0: 6c66 2e63 7573 746f 6d5f 3430 345f 7061  lf.custom_404_pa
+000028c0: 6765 2e65 6e63 6f64 6528 290a 2020 2020  ge.encode().    
+000028d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028e0: 2020 2020 6966 2073 656c 662e 6375 7374      if self.cust
+000028f0: 6f6d 5f34 3034 5f70 6167 650a 2020 2020  om_404_page.    
+00002900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002910: 2020 2020 656c 7365 2066 6f66 2e65 6e63      else fof.enc
+00002920: 6f64 6528 290a 2020 2020 2020 2020 2020  ode().          
+00002930: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00002940: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
+00002950: 2020 2020 2020 6578 6365 7074 204b 6579        except Key
+00002960: 626f 6172 6449 6e74 6572 7275 7074 3a0a  boardInterrupt:.
+00002970: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00002980: 7428 225c 6e53 6572 7665 7220 7368 7574  t("\nServer shut
+00002990: 7469 6e67 2064 6f77 6e2e 2e2e 2229 0a20  ting down..."). 
+000029a0: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+000029b0: 6365 7074 696f 6e20 6173 2065 3a0a 2020  ception as e:.  
+000029c0: 2020 2020 2020 2020 2020 7374 6174 7573            status
+000029d0: 203d 2022 3530 3020 494e 5445 524e 414c   = "500 INTERNAL
+000029e0: 2053 4552 5645 5220 4552 524f 5222 0a20   SERVER ERROR". 
+000029f0: 2020 2020 2020 2020 2020 2068 6561 6465             heade
+00002a00: 7273 203d 205b 2822 436f 6e74 656e 742d  rs = [("Content-
+00002a10: 7479 7065 222c 2022 7465 7874 2f68 746d  type", "text/htm
+00002a20: 6c22 295d 0a20 2020 2020 2020 2020 2020  l")].           
+00002a30: 2073 7461 7274 5f72 6573 706f 6e73 6528   start_response(
+00002a40: 7374 6174 7573 2c20 6865 6164 6572 7329  status, headers)
+00002a50: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00002a60: 6e74 2865 290a 2020 2020 2020 2020 2020  nt(e).          
+00002a70: 2020 7265 7475 726e 205b 0a20 2020 2020    return [.     
+00002a80: 2020 2020 2020 2020 2020 2028 0a20 2020             (.   
+00002a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002aa0: 2073 656c 662e 6375 7374 6f6d 5f35 3030   self.custom_500
+00002ab0: 5f70 6167 652e 656e 636f 6465 2829 0a20  _page.encode(). 
+00002ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ad0: 2020 2069 6620 7365 6c66 2e63 7573 746f     if self.custo
+00002ae0: 6d5f 3530 305f 7061 6765 0a20 2020 2020  m_500_page.     
+00002af0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00002b00: 6c73 6520 6630 302e 656e 636f 6465 2829  lse f00.encode()
+00002b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002b20: 2029 0a20 2020 2020 2020 2020 2020 205d   ).            ]
+00002b30: 0a20 2020 200a 2020 2020 6465 6620 6a73  .    .    def js
+00002b40: 6f6e 5f72 6573 706f 6e73 6528 7365 6c66  on_response(self
+00002b50: 2c20 6461 7461 293a 0a20 2020 2020 2020  , data):.       
+00002b60: 2069 6d70 6f72 7420 6a73 6f6e 0a20 2020   import json.   
+00002b70: 2020 2020 2072 6573 706f 6e73 655f 626f       response_bo
+00002b80: 6479 203d 206a 736f 6e2e 6475 6d70 7328  dy = json.dumps(
+00002b90: 6461 7461 290a 2020 2020 2020 2020 6465  data).        de
+00002ba0: 6620 7265 7370 6f6e 7365 2873 7461 7274  f response(start
+00002bb0: 5f72 6573 706f 6e73 6529 3a0a 2020 2020  _response):.    
+00002bc0: 2020 2020 2020 2020 7374 6174 7573 203d          status =
+00002bd0: 2022 3230 3020 4f4b 220a 2020 2020 2020   "200 OK".      
+00002be0: 2020 2020 2020 6865 6164 6572 7320 3d20        headers = 
+00002bf0: 5b28 2243 6f6e 7465 6e74 2d74 7970 6522  [("Content-type"
+00002c00: 2c20 2261 7070 6c69 6361 7469 6f6e 2f6a  , "application/j
+00002c10: 736f 6e22 295d 0a20 2020 2020 2020 2020  son")].         
+00002c20: 2020 2073 7461 7274 5f72 6573 706f 6e73     start_respons
+00002c30: 6528 7374 6174 7573 2c20 6865 6164 6572  e(status, header
+00002c40: 7329 0a20 2020 2020 2020 2020 2020 2072  s).            r
+00002c50: 6574 7572 6e20 5b72 6573 706f 6e73 655f  eturn [response_
+00002c60: 626f 6479 2e65 6e63 6f64 6528 295d 0a20  body.encode()]. 
+00002c70: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00002c80: 7370 6f6e 7365 0a0a 2020 2020 6465 6620  sponse..    def 
+00002c90: 7275 6e28 7365 6c66 2c20 686f 7374 3d22  run(self, host="
+00002ca0: 6c6f 6361 6c68 6f73 7422 2c20 706f 7274  localhost", port
+00002cb0: 3d38 3038 3029 3a0a 2020 2020 2020 2020  =8080):.        
+00002cc0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00002cd0: 2073 6572 7665 7220 3d20 6d61 6b65 5f73   server = make_s
+00002ce0: 6572 7665 7228 686f 7374 2c20 706f 7274  erver(host, port
+00002cf0: 2c20 7365 6c66 290a 2020 2020 2020 2020  , self).        
+00002d00: 2020 2020 7072 696e 7428 6622 5365 7276      print(f"Serv
+00002d10: 696e 6720 6f6e 207b 686f 7374 7d3a 7b70  ing on {host}:{p
+00002d20: 6f72 747d 2229 0a20 2020 2020 2020 2020  ort}").         
+00002d30: 2020 2073 6572 7665 722e 7365 7276 655f     server.serve_
+00002d40: 666f 7265 7665 7228 290a 2020 2020 2020  forever().      
+00002d50: 2020 6578 6365 7074 204b 6579 626f 6172    except Keyboar
+00002d60: 6449 6e74 6572 7275 7074 3a0a 2020 2020  dInterrupt:.    
+00002d70: 2020 2020 2020 2020 7072 696e 7428 225c          print("\
+00002d80: 6e53 6572 7665 7220 7368 7574 7469 6e67  nServer shutting
+00002d90: 2064 6f77 6e2e 2e2e 2229 0a20 2020 2020   down...").     
+00002da0: 2020 2020 2020 2073 6572 7665 722e 7365         server.se
+00002db0: 7276 6572 5f63 6c6f 7365 2829 0a         rver_close().
```

### Comparing `sitepy-0.4.0/sitepy.egg-info/PKG-INFO` & `sitepy-0.4.1/sitepy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,80 @@
-Metadata-Version: 2.1
-Name: sitepy
-Version: 0.4.0
-Summary: A simple web framework.
-Home-page: https://github.com/WolfTheDeveloper/sitepy
-Author: WolfTheDev
-Author-email: wolfthedev@gmail.com
-License: Apache 2.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# sitepy
-
-A simple web framework for Python.
-
-## Installation
-
-You can install sitepy with pip:
-
-```sh
-pip install sitepy
-```
-
-## Usage
-
-Here's a basic example of a sitepy application:
-
-```python
-from sitepy import sitepy
-
-app = sitepy()
-
-@app.route("/", methods=['GET', 'POST'])
-def index():
-    return "Hello, world!"
-
-if __name__ == "__main__":
-    app.run()
-```
-
-This will start a server on localhost:8080 and respond with "Hello, world!" to GET and POST requests at the root URL.
-
-## Features
-
-- Simple routing: Use the @app.route decorator to define routes.
-
-- Middleware support: Use app.use to add middleware functions.
-
-- Static file serving: Files in the static directory are served at /static.
-
-## Contributing
-
-Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-
-## License
-[Apache](sitepy/LICENSE)
+Metadata-Version: 2.1
+Name: sitepy
+Version: 0.4.1
+Summary: A simple web framework.
+Home-page: https://github.com/WolfTheDeveloper/sitepy
+Author: WolfTheDev
+Author-email: wolfthedev@gmail.com
+License: Copyright [2024] [WolfTheDev]
+        
+        Licensed under the Apache License, Version 2.0 (the "License");
+        you may not use this file except in compliance with the License.
+        You may obtain a copy of the License at
+        
+            http://www.apache.org/licenses/LICENSE-2.0
+        
+        Unless required by applicable law or agreed to in writing, software
+        distributed under the License is distributed on an "AS IS" BASIS,
+        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+        See the License for the specific language governing permissions and
+        limitations under the License.
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# sitepy
+
+A simple web framework for Python.
+
+## Installation
+
+You can install sitepy with pip:
+
+```sh
+pip install sitepy
+```
+
+## Usage
+
+Here's a basic example of a sitepy application:
+
+```python
+from sitepy import sitepy
+
+app = sitepy()
+
+@app.route("/", methods=['GET', 'POST'])
+def index():
+    return "Hello, world!"
+
+if __name__ == "__main__":
+    app.run()
+```
+
+This will start a server on localhost:8080 and respond with "Hello, world!" to GET and POST requests at the root URL.
+
+## Features
+
+- Simple routing: Use the @app.route decorator to define routes.
+
+- Middleware support: Use app.use to add middleware functions.
+
+- Static file serving: Files in the static directory are served at /static.
+
+## Contributing
+
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+## License
+[Apache](sitepy/LICENSE)
```

