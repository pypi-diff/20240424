# Comparing `tmp/zro2-0.2.0.tar.gz` & `tmp/zro2-0.2.0b1.tar.gz`

## Comparing `zro2-0.2.0.tar` & `zro2-0.2.0b1.tar`

### file list

```diff
@@ -1,30 +1,24 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 zro2-0.2.0/.gitattributes
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 zro2-0.2.0/.python-version
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 zro2-0.2.0/cli.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 zro2-0.2.0/requirements-dev.lock
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 zro2-0.2.0/requirements.lock
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 zro2-0.2.0/src/zro2/__init__.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 zro2-0.2.0/src/zro2/easyocr.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 zro2-0.2.0/src/zro2/hashlib.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 zro2-0.2.0/src/zro2/io.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 zro2-0.2.0/src/zro2/json.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 zro2-0.2.0/src/zro2/keyring.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 zro2-0.2.0/src/zro2/logging.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 zro2-0.2.0/src/zro2/pandas.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 zro2-0.2.0/src/zro2/pygetwindow.py
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 zro2-0.2.0/src/zro2/pyscreeze.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 zro2-0.2.0/src/zro2/readchar.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 zro2-0.2.0/src/zro2/requests.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 zro2-0.2.0/src/zro2/screeninfo.py
--rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 zro2-0.2.0/src/zro2/subprocess.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 zro2-0.2.0/src/zro2/time.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 zro2-0.2.0/src/zro2/typing.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 zro2-0.2.0/src/zro2/uiautomator.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 zro2-0.2.0/tests/image1.png
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 zro2-0.2.0/tests/pyscreeze.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 zro2-0.2.0/tests/test_pandas.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 zro2-0.2.0/tests/test_readchar.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 zro2-0.2.0/.gitignore
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 zro2-0.2.0/README.md
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 zro2-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 zro2-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 zro2-0.2.0b1/.gitattributes
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 zro2-0.2.0b1/.python-version
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 zro2-0.2.0b1/CHANGELOG
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 zro2-0.2.0b1/cli.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 zro2-0.2.0b1/requirements-dev.lock
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 zro2-0.2.0b1/requirements.lock
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 zro2-0.2.0b1/.vscode/settings.json
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 zro2-0.2.0b1/src/zro2/__init__.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 zro2-0.2.0b1/src/zro2/hashlib.py
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 zro2-0.2.0b1/src/zro2/io.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 zro2-0.2.0b1/src/zro2/json.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 zro2-0.2.0b1/src/zro2/keyring.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 zro2-0.2.0b1/src/zro2/logging.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 zro2-0.2.0b1/src/zro2/pygetwindow.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 zro2-0.2.0b1/src/zro2/readchar.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 zro2-0.2.0b1/src/zro2/requests.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 zro2-0.2.0b1/src/zro2/screeninfo.py
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 zro2-0.2.0b1/src/zro2/subprocess.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 zro2-0.2.0b1/src/zro2/typing.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 zro2-0.2.0b1/tests/test_readchar.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 zro2-0.2.0b1/.gitignore
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 zro2-0.2.0b1/README.md
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 zro2-0.2.0b1/pyproject.toml
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 zro2-0.2.0b1/PKG-INFO
```

### Comparing `zro2-0.2.0/cli.py` & `zro2-0.2.0b1/cli.py`

 * *Files identical despite different names*

### Comparing `zro2-0.2.0/src/zro2/__init__.py` & `zro2-0.2.0b1/src/zro2/__init__.py`

 * *Files identical despite different names*

### Comparing `zro2-0.2.0/src/zro2/hashlib.py` & `zro2-0.2.0b1/src/zro2/hashlib.py`

 * *Files identical despite different names*

### Comparing `zro2-0.2.0/src/zro2/io.py` & `zro2-0.2.0b1/src/zro2/io.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,25 +35,25 @@
         with open(path, 'rb') as f:
             return f.read()
 
     def __init__(
         self, 
         path : property, 
         watching : typing.List[typing.Literal["mdate", "adate", "sha256", "size"]] = ["mdate","size", ],
-        callback : typing.Callable | None = None,
-        loadmethod : typing.Callable | None = None
+        callback : typing.Callable = None,
+        loadmethod : typing.Callable = None
     ):
         self.path = path
         self.watching = watching
         self.callback = callback
         self.loadmethod = loadmethod or FileProperty.__defaultLoadMethod
 
     def __get__(self, instance, owner):
         if isinstance(self.path, property):
-            self.path = self.path.fget(instance) # type: ignore
+            self.path = self.path.fget(instance)
         
         if not os.path.exists(self.path):
             return None
         
         recordedCtx =self._properties.get(self.path, {})
         
         prepNewCtx = {}
@@ -74,10 +74,10 @@
         else:
             recordedContent = recordedCtx.get("content", None)
             if isinstance(recordedContent, io.TextIOWrapper):
                 recordedContent.close()
 
             content = self.loadmethod(self.path)
             prepNewCtx["content"] = content
-            self._properties[self.path] = prepNewCtx # type: ignore 
+            self._properties[self.path] = prepNewCtx
             return content
```

### Comparing `zro2-0.2.0/src/zro2/pygetwindow.py` & `zro2-0.2.0b1/src/zro2/pygetwindow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from time import sleep
 import pygetwindow as gw
 import typing
+
 from zro2.screeninfo import get_screen_dimensions
 
 def activate_wnd(wnd : gw.Window):
     try:
         wnd.activate()
     except gw.PyGetWindowException:
         pass
@@ -12,18 +13,18 @@
 def get_window_pos(wnd : gw.Window) -> typing.Tuple[float, float, float, float]:
     return (wnd.left, wnd.top, wnd.width, wnd.height)
 
 def grid_orientation(
     wnds : typing.List[gw.Window],
     row : int, 
     col : int, 
-    maxwidth : float | None = None,
-    maxheight : float | None = None,
-    minwidth : float | None = None,
-    minheight : float | None = None,
+    maxwidth : float = None,
+    maxheight : float = None,
+    minwidth : float = None,
+    minheight : float = None,
     monitor : int = 0,
     sleepTime : float = 0.2
 ):
 
     screen_width, screen_height, monitor_x, monitor_y = get_screen_dimensions(monitor_index=monitor)
     num_windows = len(wnds)
     if num_windows == 0 or row == 0 or col == 0:
```

### Comparing `zro2-0.2.0/src/zro2/readchar.py` & `zro2-0.2.0b1/src/zro2/readchar.py`

 * *Files identical despite different names*

### Comparing `zro2-0.2.0/src/zro2/screeninfo.py` & `zro2-0.2.0b1/src/zro2/screeninfo.py`

 * *Files identical despite different names*

### Comparing `zro2-0.2.0/src/zro2/subprocess.py` & `zro2-0.2.0b1/src/zro2/subprocess.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         )
         return proc.stdout
     except subprocess.TimeoutExpired as e:
         raise e
     except subprocess.CalledProcessError as e:
         raise e
     
-def query(path: str, *args, timeout: int = 5, raw: bool = False, decode_order: List[str] = ["utf-8", "gbk"], to_list: bool = False, strip_null_lines: bool = False) -> Union[str, List[str], bytes]:
+def query(path: str, *args, timeout: int = 5, raw: bool = False, decode_order: List[str] = ["utf-8", "gbk"], to_list: bool = False, strip_null_lines: bool = False) -> Union[str, List[str]]:
     """
     Perform a query with optional parameters for timeout, raw output, return context, decoding order, conversion to list, and stripping null lines.
 
     Args:
         path: The executable path.
         *args: Variable length argument list.
         timeout (int): Timeout duration in seconds (default is 5).
@@ -72,15 +72,15 @@
     for decoder in decode_order:
         try:
             decoded = raw_output.decode(decoder)
             break
         except UnicodeDecodeError:
             continue
     else:
-        raise UnicodeDecodeError("Failed to decode output using provided decode orders.") # type: ignore
+        raise UnicodeDecodeError("Failed to decode output using provided decode orders.")
 
     if to_list:
         decoded = decoded.strip().split("\r\n")
         if strip_null_lines:
             decoded = [line.strip() for line in decoded if line]
 
     return decoded
```

### Comparing `zro2-0.2.0/tests/test_readchar.py` & `zro2-0.2.0b1/tests/test_readchar.py`

 * *Files identical despite different names*

### Comparing `zro2-0.2.0/.gitignore` & `zro2-0.2.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `zro2-0.2.0/README.md` & `zro2-0.2.0b1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # ZrO2
 util functions for projects
 
 ## Features
-This module contains a series of files, each providing extended utility functions specific to the module that it named. The goal is to primarily utilize standard libraries to ensure maximum compatibility. 
-
-This project does not introduce additional dependencies. However, some files may require extra dependencies and co-dependencies. Please refer to the table below for detailed information.
+This module contains a series of files, each providing extended utility functions specific to the module that it named. The goal is to primarily utilize standard libraries to ensure maximum compatibility. This project does not introduce additional dependencies. However, some files may require extra dependencies and co-dependencies. Please refer to the table below for detailed information.
 
 ## Install
 ### by pypi
 
 ```bash
 pip install zro2
 ```
@@ -17,28 +15,24 @@
 
 ```bash
 pip install git+https://github.com/ZackaryW/ZrO2.git
 ```
 
 ## Index
 
-|    File     |    Non Std Dependencies    | Co-dependencies | Test State |
-| ----------- | -------------------------- | --------------- | ---------- |
-| hashlib     | [None]                     | [None]          | tested     |
-| json        | [None]                     | [None]          | untested   |
-| logging     | [None]                     | [None]          | tested     |
-| pygetwindow | pygetwindow                | sceeninfo       | untested   |
-| requests    | [None]                     | [None]          | untested   |
-| screeninfo  | screeninfo, pygetwindow    | [None]          | untested   |
-| typing      | [None]                     | [None]          | untested   |
-| subprocess  | [None]                     | [None]          | untested   |
-| keyring     | keyring                    | [None]          | untested   |
-| io          | pyyaml, toml               | [None]          | untested   |
-| time        | [None]                     | [None]          | untested   |
-| easyocr     | easyocr, numpy             | [None]          | untested   |
-| pyscreeze   | pyscreeze, screeninfo, PIL | [None]          | tested     |
-| pandas      | pandas                     | [None]          | tested   |
+| File        | Non Std Dependencies    | Co-dependencies |
+| ----------- | ----------------------- | --------------- |
+| hashlib     | [None]                  | [None]          |
+| json        | [None]                  | [None]          |
+| logging     | [None]                  | [None]          |
+| pygetwindow | pygetwindow             | sceeninfo       |
+| requests    | [None]                  | [None]          |
+| screeninfo  | screeninfo, pygetwindow | [None]          |
+| typing      | [None]                  | [None]          |
+| subprocess  | [None]                  | [None]          |
+| keyring     | keyring                 | [None]          |
+| io          | pyyaml, toml            | [None]          |
 
 ## Update cycles
 1. by default, this project will update util functions every 30 days (month)
 2. a beta release will be made available each week
```

