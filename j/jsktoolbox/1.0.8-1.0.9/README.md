# Comparing `tmp/jsktoolbox-1.0.8.tar.gz` & `tmp/jsktoolbox-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsktoolbox-1.0.8.tar", max compression
+gzip compressed data, was "jsktoolbox-1.0.9.tar", max compression
```

## Comparing `jsktoolbox-1.0.8.tar` & `jsktoolbox-1.0.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1081 2023-07-04 10:26:37.611936 jsktoolbox-1.0.8/LICENSE
--rw-r--r--   0        0        0     1309 2023-11-17 12:52:58.524738 jsktoolbox-1.0.8/README.md
--rw-r--r--   0        0        0        1 2023-07-04 10:43:20.338920 jsktoolbox-1.0.8/jsktoolbox/__init__.py
--rw-r--r--   0        0        0     2226 2023-11-07 09:41:29.231317 jsktoolbox-1.0.8/jsktoolbox/attribtool.py
--rw-r--r--   0        0        0        0 2023-09-01 13:34:11.495755 jsktoolbox-1.0.8/jsktoolbox/configtool/__init__.py
--rw-r--r--   0        0        0        1 2023-11-06 08:38:32.985743 jsktoolbox-1.0.8/jsktoolbox/configtool/libs/__init__.py
--rw-r--r--   0        0        0    11535 2023-11-17 12:49:47.904681 jsktoolbox-1.0.8/jsktoolbox/configtool/libs/data.py
--rw-r--r--   0        0        0     2885 2023-11-17 12:49:47.904681 jsktoolbox-1.0.8/jsktoolbox/configtool/libs/file.py
--rw-r--r--   0        0        0     5853 2023-11-17 12:49:47.904681 jsktoolbox-1.0.8/jsktoolbox/configtool/main.py
--rw-r--r--   0        0        0        1 2023-11-02 12:38:12.781049 jsktoolbox-1.0.8/jsktoolbox/devices/__init__.py
--rw-r--r--   0        0        0        1 2023-11-02 12:38:12.781049 jsktoolbox-1.0.8/jsktoolbox/devices/libs/__init__.py
--rw-r--r--   0        0        0        0 2023-11-02 12:38:12.781049 jsktoolbox-1.0.8/jsktoolbox/devices/mikrotik/__init__.py
--rw-r--r--   0        0        0        0 2023-11-02 12:38:12.781049 jsktoolbox-1.0.8/jsktoolbox/devices/network/__init__.py
--rw-r--r--   0        0        0     1507 2023-11-02 12:38:12.781049 jsktoolbox-1.0.8/jsktoolbox/devices/network/connectors.py
--rw-r--r--   0        0        0        1 2023-11-02 12:38:12.781049 jsktoolbox-1.0.8/jsktoolbox/libs/__init__.py
--rw-r--r--   0        0        0     1544 2023-11-17 12:49:47.904681 jsktoolbox-1.0.8/jsktoolbox/libs/base_data.py
--rw-r--r--   0        0        0     7552 2023-11-17 12:49:47.908681 jsktoolbox-1.0.8/jsktoolbox/libs/base_logs.py
--rw-r--r--   0        0        0     8597 2023-11-17 12:49:47.908681 jsktoolbox-1.0.8/jsktoolbox/libs/base_th.py
--rw-r--r--   0        0        0        1 2023-09-25 09:14:22.727340 jsktoolbox-1.0.8/jsktoolbox/libs/interfaces/__init__.py
--rw-r--r--   0        0        0     1176 2023-11-02 12:12:51.516959 jsktoolbox-1.0.8/jsktoolbox/libs/interfaces/comparators.py
--rw-r--r--   0        0        0      442 2023-11-06 08:39:31.093723 jsktoolbox-1.0.8/jsktoolbox/libs/interfaces/logger_engine.py
--rw-r--r--   0        0        0    11666 2023-11-17 12:49:47.908681 jsktoolbox-1.0.8/jsktoolbox/libs/system.py
--rw-r--r--   0        0        0        1 2023-11-06 08:38:46.033736 jsktoolbox-1.0.8/jsktoolbox/logstool/__init__.py
--rw-r--r--   0        0        0    10409 2023-11-17 12:49:47.908681 jsktoolbox-1.0.8/jsktoolbox/logstool/engines.py
--rw-r--r--   0        0        0     1845 2023-11-06 08:39:31.093723 jsktoolbox-1.0.8/jsktoolbox/logstool/formatters.py
--rw-r--r--   0        0        0    11945 2023-11-17 12:49:47.908681 jsktoolbox-1.0.8/jsktoolbox/logstool/logs.py
--rw-r--r--   0        0        0        0 2023-07-04 10:43:20.338920 jsktoolbox-1.0.8/jsktoolbox/netaddresstool/__init__.py
--rw-r--r--   0        0        0    15758 2023-11-17 12:49:47.908681 jsktoolbox-1.0.8/jsktoolbox/netaddresstool/ipv4.py
--rw-r--r--   0        0        0    16007 2023-11-17 12:49:47.908681 jsktoolbox-1.0.8/jsktoolbox/netaddresstool/ipv6.py
--rw-r--r--   0        0        0        0 2023-07-04 10:43:20.338920 jsktoolbox-1.0.8/jsktoolbox/netaddresstool/libs/__init__.py
--rw-r--r--   0        0        0     3762 2023-11-17 12:49:47.908681 jsktoolbox-1.0.8/jsktoolbox/netaddresstool/libs/octets.py
--rw-r--r--   0        0        0     4003 2023-11-17 12:49:47.908681 jsktoolbox-1.0.8/jsktoolbox/netaddresstool/libs/words.py
--rw-r--r--   0        0        0     7701 2023-09-01 13:35:37.015786 jsktoolbox-1.0.8/jsktoolbox/raisetool.py
--rw-r--r--   0        0        0        0 2023-11-06 08:38:32.989743 jsktoolbox-1.0.8/jsktoolbox/stringtool/__init__.py
--rw-r--r--   0        0        0     6568 2023-11-17 12:49:47.908681 jsktoolbox-1.0.8/jsktoolbox/stringtool/crypto.py
--rw-r--r--   0        0        0      752 2023-11-17 12:51:18.672708 jsktoolbox-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     2134 1970-01-01 00:00:00.000000 jsktoolbox-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-07-04 10:26:37.611936 jsktoolbox-1.0.9/LICENSE
+-rw-r--r--   0        0        0     1309 2023-11-17 14:13:11.960073 jsktoolbox-1.0.9/README.md
+-rw-r--r--   0        0        0        1 2023-07-04 10:43:20.338920 jsktoolbox-1.0.9/jsktoolbox/__init__.py
+-rw-r--r--   0        0        0     2226 2023-11-07 09:41:29.231317 jsktoolbox-1.0.9/jsktoolbox/attribtool.py
+-rw-r--r--   0        0        0        0 2023-09-01 13:34:11.495755 jsktoolbox-1.0.9/jsktoolbox/configtool/__init__.py
+-rw-r--r--   0        0        0        1 2023-11-06 08:38:32.985743 jsktoolbox-1.0.9/jsktoolbox/configtool/libs/__init__.py
+-rw-r--r--   0        0        0    11535 2023-11-17 12:49:47.904681 jsktoolbox-1.0.9/jsktoolbox/configtool/libs/data.py
+-rw-r--r--   0        0        0     2885 2023-11-17 12:49:47.904681 jsktoolbox-1.0.9/jsktoolbox/configtool/libs/file.py
+-rw-r--r--   0        0        0     6818 2023-11-17 14:10:10.080047 jsktoolbox-1.0.9/jsktoolbox/configtool/main.py
+-rw-r--r--   0        0        0        1 2023-11-02 12:38:12.781049 jsktoolbox-1.0.9/jsktoolbox/devices/__init__.py
+-rw-r--r--   0        0        0        1 2023-11-02 12:38:12.781049 jsktoolbox-1.0.9/jsktoolbox/devices/libs/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-02 12:38:12.781049 jsktoolbox-1.0.9/jsktoolbox/devices/mikrotik/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-02 12:38:12.781049 jsktoolbox-1.0.9/jsktoolbox/devices/network/__init__.py
+-rw-r--r--   0        0        0     1507 2023-11-02 12:38:12.781049 jsktoolbox-1.0.9/jsktoolbox/devices/network/connectors.py
+-rw-r--r--   0        0        0        1 2023-11-02 12:38:12.781049 jsktoolbox-1.0.9/jsktoolbox/libs/__init__.py
+-rw-r--r--   0        0        0     1544 2023-11-17 12:49:47.904681 jsktoolbox-1.0.9/jsktoolbox/libs/base_data.py
+-rw-r--r--   0        0        0     7552 2023-11-17 12:49:47.908681 jsktoolbox-1.0.9/jsktoolbox/libs/base_logs.py
+-rw-r--r--   0        0        0     8597 2023-11-17 12:49:47.908681 jsktoolbox-1.0.9/jsktoolbox/libs/base_th.py
+-rw-r--r--   0        0        0        1 2023-09-25 09:14:22.727340 jsktoolbox-1.0.9/jsktoolbox/libs/interfaces/__init__.py
+-rw-r--r--   0        0        0     1176 2023-11-02 12:12:51.516959 jsktoolbox-1.0.9/jsktoolbox/libs/interfaces/comparators.py
+-rw-r--r--   0        0        0      442 2023-11-06 08:39:31.093723 jsktoolbox-1.0.9/jsktoolbox/libs/interfaces/logger_engine.py
+-rw-r--r--   0        0        0    11666 2023-11-17 12:49:47.908681 jsktoolbox-1.0.9/jsktoolbox/libs/system.py
+-rw-r--r--   0        0        0        1 2023-11-06 08:38:46.033736 jsktoolbox-1.0.9/jsktoolbox/logstool/__init__.py
+-rw-r--r--   0        0        0    10409 2023-11-17 12:49:47.908681 jsktoolbox-1.0.9/jsktoolbox/logstool/engines.py
+-rw-r--r--   0        0        0     1845 2023-11-06 08:39:31.093723 jsktoolbox-1.0.9/jsktoolbox/logstool/formatters.py
+-rw-r--r--   0        0        0    11945 2023-11-17 12:49:47.908681 jsktoolbox-1.0.9/jsktoolbox/logstool/logs.py
+-rw-r--r--   0        0        0        0 2023-07-04 10:43:20.338920 jsktoolbox-1.0.9/jsktoolbox/netaddresstool/__init__.py
+-rw-r--r--   0        0        0    15758 2023-11-17 12:49:47.908681 jsktoolbox-1.0.9/jsktoolbox/netaddresstool/ipv4.py
+-rw-r--r--   0        0        0    16007 2023-11-17 12:49:47.908681 jsktoolbox-1.0.9/jsktoolbox/netaddresstool/ipv6.py
+-rw-r--r--   0        0        0        0 2023-07-04 10:43:20.338920 jsktoolbox-1.0.9/jsktoolbox/netaddresstool/libs/__init__.py
+-rw-r--r--   0        0        0     3762 2023-11-17 12:49:47.908681 jsktoolbox-1.0.9/jsktoolbox/netaddresstool/libs/octets.py
+-rw-r--r--   0        0        0     4003 2023-11-17 12:49:47.908681 jsktoolbox-1.0.9/jsktoolbox/netaddresstool/libs/words.py
+-rw-r--r--   0        0        0     7701 2023-09-01 13:35:37.015786 jsktoolbox-1.0.9/jsktoolbox/raisetool.py
+-rw-r--r--   0        0        0        0 2023-11-06 08:38:32.989743 jsktoolbox-1.0.9/jsktoolbox/stringtool/__init__.py
+-rw-r--r--   0        0        0     6568 2023-11-17 12:49:47.908681 jsktoolbox-1.0.9/jsktoolbox/stringtool/crypto.py
+-rw-r--r--   0        0        0      752 2023-11-17 14:12:45.956070 jsktoolbox-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2134 1970-01-01 00:00:00.000000 jsktoolbox-1.0.9/PKG-INFO
```

### Comparing `jsktoolbox-1.0.8/LICENSE` & `jsktoolbox-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jsktoolbox-1.0.8/README.md` & `jsktoolbox-1.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,39 +2,39 @@
 
 The project contains sets of base classes for various operations.
 
 ## AttribTool
 
 The project contains base classes that limit the possibility of adding new attributes without their prior declaration inside classes inheriting from them or their objects.
 
-[AttribTool Readme](https://github.com/Szumak75/JskToolBox/blob/1.0.8/docs/AttribTool.md)
+[AttribTool Readme](https://github.com/Szumak75/JskToolBox/blob/1.0.9/docs/AttribTool.md)
 
 ## ConfigTool
 
 The project contains classes that enable common operations on configuration files.
 
-[ConfigTool Readme](https://github.com/Szumak75/JskToolBox/blob/1.0.8/docs/ConfigTool.md)
+[ConfigTool Readme](https://github.com/Szumak75/JskToolBox/blob/1.0.9/docs/ConfigTool.md)
 
 ## LogsTool
 
 The project contains several classes that create a logging subsystem for the designed solutions.
 
-[LogsTool Readme](https://github.com/Szumak75/JskToolBox/blob/1.0.8/docs/LogsTool.md)
+[LogsTool Readme](https://github.com/Szumak75/JskToolBox/blob/1.0.9/docs/LogsTool.md)
 
 ## NetAddressTool
 
 The project contains sets of base classes for operations on IPv4 and IPv6 addresses.
 
-[NetAddressTool Readme](https://github.com/Szumak75/JskToolBox/blob/1.0.8/docs/NetAddressTool.md)
+[NetAddressTool Readme](https://github.com/Szumak75/JskToolBox/blob/1.0.9/docs/NetAddressTool.md)
 
 ## RaiseTool
 
 The project contains small class for formatting thrown exception messages.
 
-[RaiseTool Readme](https://github.com/Szumak75/JskToolBox/blob/1.0.8/docs/RaiseTool.md)
+[RaiseTool Readme](https://github.com/Szumak75/JskToolBox/blob/1.0.9/docs/RaiseTool.md)
 
 ## StringTool
 
 The project contains sets of classes for various operations on string.
 
-[StringTool Readme](https://github.com/Szumak75/JskToolBox/blob/1.0.8/docs/StringTool.md)
+[StringTool Readme](https://github.com/Szumak75/JskToolBox/blob/1.0.9/docs/StringTool.md)
```

### Comparing `jsktoolbox-1.0.8/jsktoolbox/attribtool.py` & `jsktoolbox-1.0.9/jsktoolbox/attribtool.py`

 * *Files identical despite different names*

### Comparing `jsktoolbox-1.0.8/jsktoolbox/configtool/libs/data.py` & `jsktoolbox-1.0.9/jsktoolbox/configtool/libs/data.py`

 * *Files identical despite different names*

### Comparing `jsktoolbox-1.0.8/jsktoolbox/configtool/libs/file.py` & `jsktoolbox-1.0.9/jsktoolbox/configtool/libs/file.py`

 * *Files identical despite different names*

### Comparing `jsktoolbox-1.0.8/jsktoolbox/configtool/main.py` & `jsktoolbox-1.0.9/jsktoolbox/configtool/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -171,9 +171,34 @@
         varname: Optional[str] = None,
         value: Optional[Any] = None,
         desc: Optional[str] = None,
     ) -> None:
         """Set data."""
         self.__dp.set(section, varname, value, desc)
 
+    def has_section(self, section_name: str) -> bool:
+        """Check section name in config file."""
+        if not isinstance(section_name, str):
+            raise Raise(
+                f"Expected String type, received: '{type(section_name)}'.",
+                TypeError,
+                self._c_name,
+                currentframe(),
+            )
+        return self.__dp.get_section(section_name) is not None
+
+    def has_varname(self, section_name: str, var_name: str) -> bool:
+        """Check varname in section."""
+        if not isinstance(var_name, str):
+            raise Raise(
+                f"Expected String type, received: '{type(var_name)}'.",
+                TypeError,
+                self._c_name,
+                currentframe(),
+            )
+        if self.has_section(section_name):
+            found_section = self.__dp.get_section(section_name)
+            return found_section.get_variable(var_name) is not None
+        return False
+
 
 # #[EOF]#######################################################################
```

### Comparing `jsktoolbox-1.0.8/jsktoolbox/devices/network/connectors.py` & `jsktoolbox-1.0.9/jsktoolbox/devices/network/connectors.py`

 * *Files identical despite different names*

### Comparing `jsktoolbox-1.0.8/jsktoolbox/libs/base_data.py` & `jsktoolbox-1.0.9/jsktoolbox/libs/base_data.py`

 * *Files identical despite different names*

### Comparing `jsktoolbox-1.0.8/jsktoolbox/libs/base_logs.py` & `jsktoolbox-1.0.9/jsktoolbox/libs/base_logs.py`

 * *Files identical despite different names*

### Comparing `jsktoolbox-1.0.8/jsktoolbox/libs/base_th.py` & `jsktoolbox-1.0.9/jsktoolbox/libs/base_th.py`

 * *Files identical despite different names*

### Comparing `jsktoolbox-1.0.8/jsktoolbox/libs/interfaces/comparators.py` & `jsktoolbox-1.0.9/jsktoolbox/libs/interfaces/comparators.py`

 * *Files identical despite different names*

### Comparing `jsktoolbox-1.0.8/jsktoolbox/libs/system.py` & `jsktoolbox-1.0.9/jsktoolbox/libs/system.py`

 * *Files identical despite different names*

### Comparing `jsktoolbox-1.0.8/jsktoolbox/logstool/engines.py` & `jsktoolbox-1.0.9/jsktoolbox/logstool/engines.py`

 * *Files identical despite different names*

### Comparing `jsktoolbox-1.0.8/jsktoolbox/logstool/formatters.py` & `jsktoolbox-1.0.9/jsktoolbox/logstool/formatters.py`

 * *Files identical despite different names*

### Comparing `jsktoolbox-1.0.8/jsktoolbox/logstool/logs.py` & `jsktoolbox-1.0.9/jsktoolbox/logstool/logs.py`

 * *Files identical despite different names*

### Comparing `jsktoolbox-1.0.8/jsktoolbox/netaddresstool/ipv4.py` & `jsktoolbox-1.0.9/jsktoolbox/netaddresstool/ipv4.py`

 * *Files identical despite different names*

### Comparing `jsktoolbox-1.0.8/jsktoolbox/netaddresstool/ipv6.py` & `jsktoolbox-1.0.9/jsktoolbox/netaddresstool/ipv6.py`

 * *Files identical despite different names*

### Comparing `jsktoolbox-1.0.8/jsktoolbox/netaddresstool/libs/octets.py` & `jsktoolbox-1.0.9/jsktoolbox/netaddresstool/libs/octets.py`

 * *Files identical despite different names*

### Comparing `jsktoolbox-1.0.8/jsktoolbox/netaddresstool/libs/words.py` & `jsktoolbox-1.0.9/jsktoolbox/netaddresstool/libs/words.py`

 * *Files identical despite different names*

### Comparing `jsktoolbox-1.0.8/jsktoolbox/raisetool.py` & `jsktoolbox-1.0.9/jsktoolbox/raisetool.py`

 * *Files identical despite different names*

### Comparing `jsktoolbox-1.0.8/jsktoolbox/stringtool/crypto.py` & `jsktoolbox-1.0.9/jsktoolbox/stringtool/crypto.py`

 * *Files identical despite different names*

### Comparing `jsktoolbox-1.0.8/pyproject.toml` & `jsktoolbox-1.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "jsktoolbox"
-version = "1.0.8"
+version = "1.0.9"
 description = "Small sets of classes for varoius operations."
 authors = ["Jacek 'Szumak' Kotlarski <szumak@virthost.pl>"]
 maintainers = ["Jacek 'Szumak' Kotlarski <szumak@virthost.pl>"]
 license = "MIT"
 readme = "README.md"
-repository = "https://github.com/Szumak75/JskToolBox/tree/1.0.8"
+repository = "https://github.com/Szumak75/JskToolBox/tree/1.0.9"
 classifiers = [
         "Programming Language :: Python :: 3",
         "Topic :: Software Development :: Libraries"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `jsktoolbox-1.0.8/PKG-INFO` & `jsktoolbox-1.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 Metadata-Version: 2.1
 Name: jsktoolbox
-Version: 1.0.8
+Version: 1.0.9
 Summary: Small sets of classes for varoius operations.
-Home-page: https://github.com/Szumak75/JskToolBox/tree/1.0.8
+Home-page: https://github.com/Szumak75/JskToolBox/tree/1.0.9
 License: MIT
 Author: Jacek 'Szumak' Kotlarski
 Author-email: szumak@virthost.pl
 Maintainer: Jacek 'Szumak' Kotlarski
 Maintainer-email: szumak@virthost.pl
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
-Project-URL: Repository, https://github.com/Szumak75/JskToolBox/tree/1.0.8
+Project-URL: Repository, https://github.com/Szumak75/JskToolBox/tree/1.0.9
 Description-Content-Type: text/markdown
 
 # JskToolBox
 
 The project contains sets of base classes for various operations.
 
 ## AttribTool
 
 The project contains base classes that limit the possibility of adding new attributes without their prior declaration inside classes inheriting from them or their objects.
 
-[AttribTool Readme](https://github.com/Szumak75/JskToolBox/blob/1.0.8/docs/AttribTool.md)
+[AttribTool Readme](https://github.com/Szumak75/JskToolBox/blob/1.0.9/docs/AttribTool.md)
 
 ## ConfigTool
 
 The project contains classes that enable common operations on configuration files.
 
-[ConfigTool Readme](https://github.com/Szumak75/JskToolBox/blob/1.0.8/docs/ConfigTool.md)
+[ConfigTool Readme](https://github.com/Szumak75/JskToolBox/blob/1.0.9/docs/ConfigTool.md)
 
 ## LogsTool
 
 The project contains several classes that create a logging subsystem for the designed solutions.
 
-[LogsTool Readme](https://github.com/Szumak75/JskToolBox/blob/1.0.8/docs/LogsTool.md)
+[LogsTool Readme](https://github.com/Szumak75/JskToolBox/blob/1.0.9/docs/LogsTool.md)
 
 ## NetAddressTool
 
 The project contains sets of base classes for operations on IPv4 and IPv6 addresses.
 
-[NetAddressTool Readme](https://github.com/Szumak75/JskToolBox/blob/1.0.8/docs/NetAddressTool.md)
+[NetAddressTool Readme](https://github.com/Szumak75/JskToolBox/blob/1.0.9/docs/NetAddressTool.md)
 
 ## RaiseTool
 
 The project contains small class for formatting thrown exception messages.
 
-[RaiseTool Readme](https://github.com/Szumak75/JskToolBox/blob/1.0.8/docs/RaiseTool.md)
+[RaiseTool Readme](https://github.com/Szumak75/JskToolBox/blob/1.0.9/docs/RaiseTool.md)
 
 ## StringTool
 
 The project contains sets of classes for various operations on string.
 
-[StringTool Readme](https://github.com/Szumak75/JskToolBox/blob/1.0.8/docs/StringTool.md)
+[StringTool Readme](https://github.com/Szumak75/JskToolBox/blob/1.0.9/docs/StringTool.md)
```

