# Comparing `tmp/xcom_proto-0.3.4.tar.gz` & `tmp/xcom_proto-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcom_proto-0.3.4.tar", max compression
+gzip compressed data, was "xcom_proto-0.3.5.tar", max compression
```

## Comparing `xcom_proto-0.3.4.tar` & `xcom_proto-0.3.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2021-05-28 08:45:09.224099 xcom_proto-0.3.4/LICENSE
--rw-r--r--   0        0        0     6253 2024-02-20 12:29:52.524605 xcom_proto-0.3.4/README.md
--rw-r--r--   0        0        0      557 2024-02-20 15:07:11.020687 xcom_proto-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     2129 2024-02-20 14:54:25.383464 xcom_proto-0.3.4/xcom_proto/XcomAbs.py
--rw-r--r--   0        0        0     4241 2024-02-20 14:57:20.703484 xcom_proto-0.3.4/xcom_proto/XcomLAN.py
--rw-r--r--   0        0        0     1160 2024-02-20 14:55:53.073475 xcom_proto-0.3.4/xcom_proto/XcomRS232.py
--rwxr-xr-x   0        0        0      151 2023-12-01 12:44:46.219550 xcom_proto-0.3.4/xcom_proto/__init__.py
--rw-r--r--   0        0        0     8766 2024-01-31 15:29:29.574821 xcom_proto-0.3.4/xcom_proto/parameters.py
--rw-r--r--   0        0        0     7411 2024-02-20 15:04:36.617239 xcom_proto-0.3.4/xcom_proto/protocol.py
--rw-r--r--   0        0        0     7003 1970-01-01 00:00:00.000000 xcom_proto-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-05-28 08:45:09.224099 xcom_proto-0.3.5/LICENSE
+-rw-r--r--   0        0        0     6253 2024-02-20 12:29:52.524605 xcom_proto-0.3.5/README.md
+-rw-r--r--   0        0        0      557 2024-04-24 13:43:16.528317 xcom_proto-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     2129 2024-02-20 14:54:25.383464 xcom_proto-0.3.5/xcom_proto/XcomAbs.py
+-rw-r--r--   0        0        0     4241 2024-02-20 14:57:20.703484 xcom_proto-0.3.5/xcom_proto/XcomLAN.py
+-rw-r--r--   0        0        0     1219 2024-04-24 13:23:19.767515 xcom_proto-0.3.5/xcom_proto/XcomRS232.py
+-rwxr-xr-x   0        0        0      151 2023-12-01 12:44:46.219550 xcom_proto-0.3.5/xcom_proto/__init__.py
+-rw-r--r--   0        0        0     8766 2024-01-31 15:29:29.574821 xcom_proto-0.3.5/xcom_proto/parameters.py
+-rw-r--r--   0        0        0     7559 2024-04-24 13:35:45.098869 xcom_proto-0.3.5/xcom_proto/protocol.py
+-rw-r--r--   0        0        0     7003 1970-01-01 00:00:00.000000 xcom_proto-0.3.5/PKG-INFO
```

### Comparing `xcom_proto-0.3.4/LICENSE` & `xcom_proto-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xcom_proto-0.3.4/README.md` & `xcom_proto-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `xcom_proto-0.3.4/pyproject.toml` & `xcom_proto-0.3.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xcom_proto"
-version = "0.3.4"
+version = "0.3.5"
 description = "Python library implementing Studer-Innotec Xcom protocol used by Xcom-232i and Xcom-LAN"
 authors = ["zocker_160 <zocker1600@posteo.net>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/zocker-160/xcom-protocol"
 repository = "https://github.com/zocker-160/xcom-protocol"
```

### Comparing `xcom_proto-0.3.4/xcom_proto/XcomAbs.py` & `xcom_proto-0.3.5/xcom_proto/XcomAbs.py`

 * *Files identical despite different names*

### Comparing `xcom_proto-0.3.4/xcom_proto/XcomLAN.py` & `xcom_proto-0.3.5/xcom_proto/XcomLAN.py`

 * *Files identical despite different names*

### Comparing `xcom_proto-0.3.4/xcom_proto/XcomRS232.py` & `xcom_proto-0.3.5/xcom_proto/XcomRS232.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
         with serial.Serial(self.serialDevice, self.baudrate, timeout=self.timeout) as ser:
             self.log.debug(f" --> {data.hex()}")
             ser.write(data)
 
             response: bytes = ser.read_until(SERIAL_TERMINATOR, size=MSG_MAX_LENGTH)
             self.log.debug(f" <-- {response.hex()}")
+            assert len(response) > 0, "got empty response"
 
         retPackage = Package.parseBytes(response[:-len(SERIAL_TERMINATOR)])
         self.log.debug(retPackage)
 
         if err := retPackage.getError():
             raise KeyError("Error received", err)
```

### Comparing `xcom_proto-0.3.4/xcom_proto/parameters.py` & `xcom_proto-0.3.5/xcom_proto/parameters.py`

 * *Files identical despite different names*

### Comparing `xcom_proto-0.3.4/xcom_proto/protocol.py` & `xcom_proto-0.3.5/xcom_proto/protocol.py`

 * *Files 3% similar despite different names*

```diff
@@ -141,20 +141,27 @@
 class Package:
 
     start_byte: bytes = b'\xAA'
     header: Header
     frame_data: Frame
 
     @staticmethod
+    def seekPackageStart(f: BufferedReader) -> bool:
+        while True:
+            byte = f.read(1)
+            if not byte:
+                return False
+            if byte == Package.start_byte:
+                f.seek(-1, 1)
+                return True
+
+    @staticmethod
     def parse(f: BufferedReader):
-        # package sometimes starts with 0xff
-        if (sb := f.read(1)) == b'\xff':
-            assert f.read(1) == Package.start_byte, "invalid package start byte"
-        else:
-            assert sb == Package.start_byte, f"invalid package start byte ({sb})"
+        if not Package.seekPackageStart(f):
+            raise AssertionError("empty or invalid package: package start byte not found")
 
         h_raw = f.read(Header.length)
         assert checksum(h_raw) == f.read(2), "invalid header checksum"
         header = Header.parseBytes(h_raw)
 
         f_raw = f.read(header.data_length)
         assert checksum(f_raw) == f.read(2), "invalid data checksum"
```

### Comparing `xcom_proto-0.3.4/PKG-INFO` & `xcom_proto-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcom-proto
-Version: 0.3.4
+Version: 0.3.5
 Summary: Python library implementing Studer-Innotec Xcom protocol used by Xcom-232i and Xcom-LAN
 Home-page: https://github.com/zocker-160/xcom-protocol
 License: GPL-3.0-or-later
 Author: zocker_160
 Author-email: zocker1600@posteo.net
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

