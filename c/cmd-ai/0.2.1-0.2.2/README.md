# Comparing `tmp/cmd_ai-0.2.1.tar.gz` & `tmp/cmd_ai-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmd_ai-0.2.1.tar", last modified: Thu Apr 18 16:28:28 2024, max compression
+gzip compressed data, was "cmd_ai-0.2.2.tar", last modified: Wed Apr 24 12:30:19 2024, max compression
```

## Comparing `cmd_ai-0.2.1.tar` & `cmd_ai-0.2.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-18 16:28:28.386367 cmd_ai-0.2.1/
--rw-r--r--   0 ojr       (1000) ojr       (1000)     2914 2024-04-18 16:28:28.386367 cmd_ai-0.2.1/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     2440 2024-04-18 16:28:26.000000 cmd_ai-0.2.1/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-18 16:28:28.382367 cmd_ai-0.2.1/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    21189 2024-04-18 16:27:58.000000 cmd_ai-0.2.1/bin/cmd_ai
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-18 16:28:28.386367 cmd_ai-0.2.1/cmd_ai/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      245 2023-11-21 14:40:25.000000 cmd_ai-0.2.1/cmd_ai/__init__.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1129 2023-11-21 16:13:50.000000 cmd_ai-0.2.1/cmd_ai/api_key.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      608 2024-03-18 09:12:22.000000 cmd_ai-0.2.1/cmd_ai/best_examples.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     7596 2024-01-22 08:00:22.000000 cmd_ai-0.2.1/cmd_ai/config.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     9459 2024-01-05 12:51:47.000000 cmd_ai-0.2.1/cmd_ai/function_chmi.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2296 2023-12-28 08:29:31.000000 cmd_ai-0.2.1/cmd_ai/function_goog.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3228 2023-12-28 08:29:31.000000 cmd_ai-0.2.1/cmd_ai/function_webc.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1896 2024-04-18 15:32:23.000000 cmd_ai-0.2.1/cmd_ai/g_askdalle.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    17569 2024-04-18 14:58:55.000000 cmd_ai-0.2.1/cmd_ai/g_askme.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     3243 2024-04-18 16:22:26.000000 cmd_ai-0.2.1/cmd_ai/g_askvision.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6149 2023-11-21 16:13:50.000000 cmd_ai-0.2.1/cmd_ai/key_enter.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      555 2023-12-06 16:02:32.000000 cmd_ai-0.2.1/cmd_ai/pipe.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4916 2024-01-08 08:00:50.000000 cmd_ai-0.2.1/cmd_ai/speak.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8096 2024-04-18 15:45:02.000000 cmd_ai-0.2.1/cmd_ai/syscom.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8548 2024-04-18 15:43:11.000000 cmd_ai-0.2.1/cmd_ai/texts.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2736 2023-11-21 16:13:51.000000 cmd_ai-0.2.1/cmd_ai/topbar.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1077 2023-11-21 16:13:51.000000 cmd_ai-0.2.1/cmd_ai/unitname.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       21 2024-04-18 16:28:27.000000 cmd_ai-0.2.1/cmd_ai/version.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-18 16:28:28.386367 cmd_ai-0.2.1/cmd_ai.egg-info/
--rw-r--r--   0 ojr       (1000) ojr       (1000)     2914 2024-04-18 16:28:28.000000 cmd_ai-0.2.1/cmd_ai.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      527 2024-04-18 16:28:28.000000 cmd_ai-0.2.1/cmd_ai.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2024-04-18 16:28:28.000000 cmd_ai-0.2.1/cmd_ai.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       88 2024-04-18 16:28:28.000000 cmd_ai-0.2.1/cmd_ai.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        7 2024-04-18 16:28:28.000000 cmd_ai-0.2.1/cmd_ai.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2024-04-18 16:28:28.386367 cmd_ai-0.2.1/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1239 2024-02-14 13:35:42.000000 cmd_ai-0.2.1/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-24 12:30:19.446187 cmd_ai-0.2.2/
+-rw-r--r--   0 ojr       (1000) ojr       (1000)     2914 2024-04-24 12:30:19.446187 cmd_ai-0.2.2/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     2440 2024-04-24 12:30:17.000000 cmd_ai-0.2.2/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-24 12:30:19.438187 cmd_ai-0.2.2/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    21189 2024-04-18 16:27:58.000000 cmd_ai-0.2.2/bin/cmd_ai
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-24 12:30:19.442187 cmd_ai-0.2.2/cmd_ai/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      245 2023-11-21 14:40:25.000000 cmd_ai-0.2.2/cmd_ai/__init__.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1129 2023-11-21 16:13:50.000000 cmd_ai-0.2.2/cmd_ai/api_key.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      608 2024-03-18 09:12:22.000000 cmd_ai-0.2.2/cmd_ai/best_examples.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     7596 2024-01-22 08:00:22.000000 cmd_ai-0.2.2/cmd_ai/config.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     9459 2024-01-05 12:51:47.000000 cmd_ai-0.2.2/cmd_ai/function_chmi.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2296 2023-12-28 08:29:31.000000 cmd_ai-0.2.2/cmd_ai/function_goog.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3228 2023-12-28 08:29:31.000000 cmd_ai-0.2.2/cmd_ai/function_webc.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     2693 2024-04-24 12:29:20.000000 cmd_ai-0.2.2/cmd_ai/g_askdalle.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    17569 2024-04-18 14:58:55.000000 cmd_ai-0.2.2/cmd_ai/g_askme.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     3243 2024-04-18 16:22:26.000000 cmd_ai-0.2.2/cmd_ai/g_askvision.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6149 2023-11-21 16:13:50.000000 cmd_ai-0.2.2/cmd_ai/key_enter.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      555 2023-12-06 16:02:32.000000 cmd_ai-0.2.2/cmd_ai/pipe.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4916 2024-01-08 08:00:50.000000 cmd_ai-0.2.2/cmd_ai/speak.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8096 2024-04-18 15:45:02.000000 cmd_ai-0.2.2/cmd_ai/syscom.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8548 2024-04-18 15:43:11.000000 cmd_ai-0.2.2/cmd_ai/texts.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2736 2023-11-21 16:13:51.000000 cmd_ai-0.2.2/cmd_ai/topbar.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1077 2023-11-21 16:13:51.000000 cmd_ai-0.2.2/cmd_ai/unitname.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       21 2024-04-24 12:30:18.000000 cmd_ai-0.2.2/cmd_ai/version.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-24 12:30:19.446187 cmd_ai-0.2.2/cmd_ai.egg-info/
+-rw-r--r--   0 ojr       (1000) ojr       (1000)     2914 2024-04-24 12:30:19.000000 cmd_ai-0.2.2/cmd_ai.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      527 2024-04-24 12:30:19.000000 cmd_ai-0.2.2/cmd_ai.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2024-04-24 12:30:19.000000 cmd_ai-0.2.2/cmd_ai.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       88 2024-04-24 12:30:19.000000 cmd_ai-0.2.2/cmd_ai.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        7 2024-04-24 12:30:19.000000 cmd_ai-0.2.2/cmd_ai.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2024-04-24 12:30:19.446187 cmd_ai-0.2.2/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1239 2024-02-14 13:35:42.000000 cmd_ai-0.2.2/setup.py
```

### Comparing `cmd_ai-0.2.1/PKG-INFO` & `cmd_ai-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmd_ai
-Version: 0.2.1
+Version: 0.2.2
 Summary: Another ChatGTP project in commandline of linux
 Home-page: http://gitlab.com/me/cmd_ai
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
 Requires-Dist: fire
```

### Comparing `cmd_ai-0.2.1/README.md` & `cmd_ai-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.2.1/bin/cmd_ai` & `cmd_ai-0.2.2/bin/cmd_ai`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.2.1/cmd_ai/api_key.py` & `cmd_ai-0.2.2/cmd_ai/api_key.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.2.1/cmd_ai/best_examples.py` & `cmd_ai-0.2.2/cmd_ai/best_examples.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.2.1/cmd_ai/config.py` & `cmd_ai-0.2.2/cmd_ai/config.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.2.1/cmd_ai/function_chmi.py` & `cmd_ai-0.2.2/cmd_ai/function_chmi.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.2.1/cmd_ai/function_goog.py` & `cmd_ai-0.2.2/cmd_ai/function_goog.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.2.1/cmd_ai/function_webc.py` & `cmd_ai-0.2.2/cmd_ai/function_webc.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.2.1/cmd_ai/g_askdalle.py` & `cmd_ai-0.2.2/cmd_ai/g_askdalle.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,24 +20,30 @@
 #from  cmd_ai import function_webc # web content
 import json # for function call
 
 # importing modules
 import urllib.request
 from PIL import Image
 import tempfile
+import datetime as dt
 
-def get_tmp():
+def get_tmp( folder = "/tmp/", timetag = False, shortname = ""):
     """
     the printer understands to PNG
     """
     suffix = '.jpg'
-    tmp_dir = '/tmp'
-    temp_file = tempfile.NamedTemporaryFile(suffix=suffix, dir=tmp_dir, delete=False)
-    temp_filename = temp_file.name
-    temp_file.close()
+    tmp_dir = folder # '/tmp'
+    temp_filename = ""
+    if timetag:
+        tag = dt.datetime.now().strftime("%Y%m%d_%H%M%S")
+        temp_filename = f"{tmp_dir}{tag}_{shortname}.jpg"
+    else:
+        temp_file = tempfile.NamedTemporaryFile(suffix=suffix, dir=tmp_dir, delete=False)
+        temp_filename = temp_file.name
+        temp_file.close()
     return temp_filename
 
 
 
 
 def g_askdalle(
         prompt,
@@ -49,35 +55,47 @@
         quality="standard",
         n=1
 ):
     """
     send demand to dalle  and fetch the image()
     """
 
-    print(f"{fg.orange}i... using EXACT PROMPT: {fg.default}",texts.role_dalle)
+    print(f"{fg.orange}i... using EXACT PROMPT: {fg.default}\n",texts.role_dalle, prompt)
     response = config.client.images.generate(
         model=model,# "dall-e-3",
         prompt=texts.role_dalle + prompt, # "a white siamese cat",
         size=size,# "1024x1024",
         quality=quality,# "standard",
         n=n# 1,
     )
     print("D... responded...")
 
 
     if response is None:
         return None
 
     image_url = response.data[0].url
-    OUTPUT = get_tmp()
+    short = prompt.replace(" ","_").strip()
+    short = short.replace("$","_").strip()
+    short = short.replace("#","_").strip()
+    short = short.replace("/","_").strip()
+    short = short.replace("(","_").strip()
+    short = short.replace(")","_").strip()
+    short = short.replace("{","_").strip()
+    short = short.replace("}","_").strip()
+    short = short.replace("!","_").strip()
+    short = short.replace("?","_").strip()
+    if len(short)>14: short = short[:14]
+    OUTPUT = get_tmp(folder="./", timetag=True, shortname = short  ) # use "/"
     print(f"D... fetching {OUTPUT}...")
     urllib.request.urlretrieve( image_url , OUTPUT )
 
     img = Image.open( OUTPUT)
     img.show()
+
     return response
 
 
 
 if __name__ == "__main__":
     print("i... in the __main__ of unitname of cmd_ai")
     Fire()
```

### Comparing `cmd_ai-0.2.1/cmd_ai/g_askme.py` & `cmd_ai-0.2.2/cmd_ai/g_askme.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.2.1/cmd_ai/g_askvision.py` & `cmd_ai-0.2.2/cmd_ai/g_askvision.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.2.1/cmd_ai/key_enter.py` & `cmd_ai-0.2.2/cmd_ai/key_enter.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.2.1/cmd_ai/pipe.py` & `cmd_ai-0.2.2/cmd_ai/pipe.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.2.1/cmd_ai/speak.py` & `cmd_ai-0.2.2/cmd_ai/speak.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.2.1/cmd_ai/syscom.py` & `cmd_ai-0.2.2/cmd_ai/syscom.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.2.1/cmd_ai/texts.py` & `cmd_ai-0.2.2/cmd_ai/texts.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.2.1/cmd_ai/topbar.py` & `cmd_ai-0.2.2/cmd_ai/topbar.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.2.1/cmd_ai/unitname.py` & `cmd_ai-0.2.2/cmd_ai/unitname.py`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.2.1/cmd_ai.egg-info/PKG-INFO` & `cmd_ai-0.2.2/cmd_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmd_ai
-Version: 0.2.1
+Version: 0.2.2
 Summary: Another ChatGTP project in commandline of linux
 Home-page: http://gitlab.com/me/cmd_ai
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
 Requires-Dist: fire
```

### Comparing `cmd_ai-0.2.1/cmd_ai.egg-info/SOURCES.txt` & `cmd_ai-0.2.2/cmd_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmd_ai-0.2.1/setup.py` & `cmd_ai-0.2.2/setup.py`

 * *Files identical despite different names*

