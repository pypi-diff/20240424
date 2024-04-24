# Comparing `tmp/antigrav-1.0.tar.gz` & `tmp/antigrav-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antigrav-1.0.tar", last modified: Sat Mar 16 13:05:17 2024, max compression
+gzip compressed data, was "antigrav-1.1.tar", last modified: Wed Apr 24 12:41:15 2024, max compression
```

## Comparing `antigrav-1.0.tar` & `antigrav-1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-03-16 13:05:17.298816 antigrav-1.0/
--rw-rw-rw-   0        0        0       79 2024-03-16 13:02:10.000000 antigrav-1.0/CHANGELOG.txt
--rw-rw-rw-   0        0        0       25 2024-01-25 13:25:38.000000 antigrav-1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1460 2024-03-16 13:05:17.293733 antigrav-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1002 2024-03-16 13:04:35.000000 antigrav-1.0/README.txt
-drwxrwxrwx   0        0        0        0 2024-03-16 13:05:17.272150 antigrav-1.0/antigrav/
--rw-rw-rw-   0        0        0    11967 2024-03-16 13:01:08.000000 antigrav-1.0/antigrav/__init__.py
--rw-rw-rw-   0        0        0    12994 2024-03-16 12:50:29.000000 antigrav-1.0/antigrav/decoder.py
--rw-rw-rw-   0        0        0    16957 2024-03-16 12:44:30.000000 antigrav-1.0/antigrav/encoder.py
--rw-rw-rw-   0        0        0     3033 2024-03-16 12:39:35.000000 antigrav-1.0/antigrav/scanner.py
--rw-rw-rw-   0        0        0     3480 2024-03-16 12:36:38.000000 antigrav-1.0/antigrav/tool.py
-drwxrwxrwx   0        0        0        0 2024-03-16 13:05:17.292228 antigrav-1.0/antigrav.egg-info/
--rw-rw-rw-   0        0        0     1460 2024-03-16 13:05:17.000000 antigrav-1.0/antigrav.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2024-03-16 13:05:17.000000 antigrav-1.0/antigrav.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-16 13:05:17.000000 antigrav-1.0/antigrav.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-16 13:05:17.000000 antigrav-1.0/antigrav.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-16 13:05:17.298816 antigrav-1.0/setup.cfg
--rw-rw-rw-   0        0        0      695 2024-03-16 13:05:13.000000 antigrav-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 12:41:15.964174 antigrav-1.1/
+-rw-rw-rw-   0        0        0      181 2024-04-24 12:34:49.000000 antigrav-1.1/CHANGELOG.txt
+-rw-rw-rw-   0        0        0       25 2024-01-25 13:25:38.000000 antigrav-1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1466 2024-04-24 12:41:15.963175 antigrav-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1002 2024-03-16 13:04:35.000000 antigrav-1.1/README.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 12:41:15.942147 antigrav-1.1/antigrav/
+-rw-rw-rw-   0        0        0    12121 2024-04-24 12:37:00.000000 antigrav-1.1/antigrav/__init__.py
+-rw-rw-rw-   0        0        0    12994 2024-04-24 12:36:13.000000 antigrav-1.1/antigrav/decoder.py
+-rw-rw-rw-   0        0        0    16957 2024-03-16 12:44:30.000000 antigrav-1.1/antigrav/encoder.py
+-rw-rw-rw-   0        0        0     3342 2024-04-24 12:14:42.000000 antigrav-1.1/antigrav/scanner.py
+-rw-rw-rw-   0        0        0     3480 2024-03-16 12:36:38.000000 antigrav-1.1/antigrav/tool.py
+drwxrwxrwx   0        0        0        0 2024-04-24 12:41:15.962160 antigrav-1.1/antigrav.egg-info/
+-rw-rw-rw-   0        0        0     1466 2024-04-24 12:41:15.000000 antigrav-1.1/antigrav.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2024-04-24 12:41:15.000000 antigrav-1.1/antigrav.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 12:41:15.000000 antigrav-1.1/antigrav.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-24 12:41:15.000000 antigrav-1.1/antigrav.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 12:41:15.964174 antigrav-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      699 2024-04-24 12:41:02.000000 antigrav-1.1/setup.py
```

### Comparing `antigrav-1.0/PKG-INFO` & `antigrav-1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: antigrav
-Version: 1.0
+Version: 1.1
 Summary: antigrav is basically JSON but supports complex numbers
 Home-page: 
 Author: tema5002
 Author-email: xtema5002x@gmail.com
 Keywords: kreisi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Programming Language :: Python :: 3
-Description-Content-Type: True
+Description-Content-Type: text/plain
 
 a modified json because i got bored
 WOW IT FINALLY WORKS YAYAYYAYAYYAYYAYYAYYA IM SO HAPPY RIGHT NOW
 
 >>> import antigrav
 >>> from cmath import sqrt
 >>> antigrav.dump({"int": 2234, "float": 324.235, "str": "qoofy string", "list": [1, 2, "hello moon", [3, 4, [[5]]]], "tuple": ("amigger", "and", "his", "family"), "dict": {1: 2, 3: 4, 5: {6: 7}}, "complex": sqrt(-1)}, open("test.antigrav", "w"), sort_keys=True, indent=4)
```

### Comparing `antigrav-1.0/README.txt` & `antigrav-1.1/README.txt`

 * *Files identical despite different names*

### Comparing `antigrav-1.0/antigrav/__init__.py` & `antigrav-1.1/antigrav/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,26 +6,26 @@
     {
         "4": 5,
         "6": 1.0+3.0i
     }
 I JUST TOOK ENTIRE JSON SOURCE CODE PLEASE DON'T SUE ME
 <https://json.org>
 """
-__version__ = '2.0.9'
+__json_version__ = '2.0.9'
 __all__ = [
     'dump', 'dumps', 'load', 'loads',
     'ANTIGRAVDecoder', 'ANTIGRAVDecodeError', 'ANTIGRAVEncoder',
 ]
 
 __author__ = "tema5002 <tema5002@gmail.com>"
-__version__ = "1.0"
+__version__ = "1.1"
 __short_description__ = "antigrav is basically JSON but supports complex numbers"
 
-from .decoder import ANTIGRAVDecoder, ANTIGRAVDecodeError
-from .encoder import ANTIGRAVEncoder
+from decoder import ANTIGRAVDecoder, ANTIGRAVDecodeError
+from encoder import ANTIGRAVEncoder
 import codecs
 
 _default_encoder = ANTIGRAVEncoder(
     skipkeys=False,
     ensure_ascii=True,
     check_circular=True,
     allow_nan=True,
@@ -270,7 +270,9 @@
     if parse_float is not None:
         kw['parse_float'] = parse_float
     if parse_int is not None:
         kw['parse_int'] = parse_int
     if parse_constant is not None:
         kw['parse_constant'] = parse_constant
     return cls(**kw).decode(s)
+
+dump([1+2j, 1+2.0j, 1.0+2j, 1.0+2.5j, 232849432796556755848387957375+357456987877877789779j], open("test.antigrav", "w"), indent=4, sort_keys=True)
```

### Comparing `antigrav-1.0/antigrav/decoder.py` & `antigrav-1.1/antigrav/decoder.py`

 * *Files identical despite different names*

### Comparing `antigrav-1.0/antigrav/encoder.py` & `antigrav-1.1/antigrav/encoder.py`

 * *Files identical despite different names*

### Comparing `antigrav-1.0/antigrav/scanner.py` & `antigrav-1.1/antigrav/scanner.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,20 +44,29 @@
             return None, idx + 4
         elif nextchar == 't' and string[idx:idx + 4] == 'true':
             return True, idx + 4
         elif nextchar == 'f' and string[idx:idx + 5] == 'false':
             return False, idx + 5
 
         m = re.compile(
-            r"(?P<real>[+-]?\d+\.\d+|\d+)(?P<sign>[+-])(?P<imag>[+-]?\d+\.\d+|\d+)i",
+            r"(?P<real>(?:\d+|\d+\.\d+|\d+\.\d+e[+-]\d+))(?P<sign>[+-])(?P<imag>(?:\d+|\d+\.\d+|\d+\.\d+e[+-]\d+)|(?:0))i",
             (re.VERBOSE | re.MULTILINE | re.DOTALL)
         ).match(string, idx)
         if m:
-            real = float(m.group("real"))
-            imag = float(m.group("imag")) * (-1 if m.group("sign") == "-" else 1)
+            real = m.group("real")
+            if real.isdigit():
+                real = parse_int(real)
+            else:
+                real = parse_float(real)
+            imag = m.group("imag")
+            if imag.isdigit():
+                imag = parse_int(imag)
+            else:
+                imag = parse_float(imag)
+            imag *= (-1 if m.group("sign") == "-" else 1)
             res = parse_complex(real, imag)
             return res, m.end()
 
         m = NUMBER_RE.match(string, idx)
         if m is not None:
             integer, frac, exp = m.groups()
             if frac or exp:
```

### Comparing `antigrav-1.0/antigrav/tool.py` & `antigrav-1.1/antigrav/tool.py`

 * *Files identical despite different names*

### Comparing `antigrav-1.0/antigrav.egg-info/PKG-INFO` & `antigrav-1.1/antigrav.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: antigrav
-Version: 1.0
+Version: 1.1
 Summary: antigrav is basically JSON but supports complex numbers
 Home-page: 
 Author: tema5002
 Author-email: xtema5002x@gmail.com
 Keywords: kreisi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Programming Language :: Python :: 3
-Description-Content-Type: True
+Description-Content-Type: text/plain
 
 a modified json because i got bored
 WOW IT FINALLY WORKS YAYAYYAYAYYAYYAYYAYYA IM SO HAPPY RIGHT NOW
 
 >>> import antigrav
 >>> from cmath import sqrt
 >>> antigrav.dump({"int": 2234, "float": 324.235, "str": "qoofy string", "list": [1, 2, "hello moon", [3, 4, [[5]]]], "tuple": ("amigger", "and", "his", "family"), "dict": {1: 2, 3: 4, 5: {6: 7}}, "complex": sqrt(-1)}, open("test.antigrav", "w"), sort_keys=True, indent=4)
```

### Comparing `antigrav-1.0/setup.py` & `antigrav-1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
- 
+
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Education",
     "Operating System :: Microsoft :: Windows :: Windows 11",
     "Programming Language :: Python :: 3"
 ]
- 
+
 setup(
     name="antigrav",
-    version="1.0",
+    version="1.1",
     description="antigrav is basically JSON but supports complex numbers",
     long_description=open("README.txt").read(),
     url="",
     author="tema5002",
     author_email="xtema5002x@gmail.com",
-    license=None,
+    license="",
     classifiers=classifiers,
     keywords="kreisi",
     packages=find_packages(),
     install_requires=[""],
-    long_description_content_type=True
+    long_description_content_type="text/plain"
 )
```

