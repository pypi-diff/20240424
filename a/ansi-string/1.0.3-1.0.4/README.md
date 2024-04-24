# Comparing `tmp/ansi-string-1.0.3.tar.gz` & `tmp/ansi-string-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansi-string-1.0.3.tar", last modified: Mon Apr 22 23:32:26 2024, max compression
+gzip compressed data, was "ansi-string-1.0.4.tar", last modified: Wed Apr 24 02:56:59 2024, max compression
```

## Comparing `ansi-string-1.0.3.tar` & `ansi-string-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:32:26.836627 ansi-string-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-22 23:32:19.000000 ansi-string-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-22 23:32:19.000000 ansi-string-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8173 2024-04-22 23:32:26.836627 ansi-string-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-04-22 23:32:19.000000 ansi-string-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-22 23:32:19.000000 ansi-string-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-22 23:32:26.840627 ansi-string-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-22 23:32:19.000000 ansi-string-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:32:26.836627 ansi-string-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:32:26.836627 ansi-string-1.0.3/src/ansi_string/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-22 23:32:19.000000 ansi-string-1.0.3/src/ansi_string/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    75795 2024-04-22 23:32:19.000000 ansi-string-1.0.3/src/ansi_string/ansi_string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:32:26.836627 ansi-string-1.0.3/src/ansi_string.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8173 2024-04-22 23:32:26.000000 ansi-string-1.0.3/src/ansi_string.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-22 23:32:26.000000 ansi-string-1.0.3/src/ansi_string.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:32:26.000000 ansi-string-1.0.3/src/ansi_string.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 23:32:26.000000 ansi-string-1.0.3/src/ansi_string.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-22 23:32:26.000000 ansi-string-1.0.3/src/ansi_string.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:56:59.545862 ansi-string-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-24 02:56:51.000000 ansi-string-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-24 02:56:51.000000 ansi-string-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8283 2024-04-24 02:56:59.545862 ansi-string-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-04-24 02:56:51.000000 ansi-string-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-24 02:56:51.000000 ansi-string-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-24 02:56:59.545862 ansi-string-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-24 02:56:51.000000 ansi-string-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:56:59.545862 ansi-string-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:56:59.545862 ansi-string-1.0.4/src/ansi_string/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-24 02:56:51.000000 ansi-string-1.0.4/src/ansi_string/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47399 2024-04-24 02:56:51.000000 ansi-string-1.0.4/src/ansi_string/ansi_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-24 02:56:51.000000 ansi-string-1.0.4/src/ansi_string/ansi_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40618 2024-04-24 02:56:51.000000 ansi-string-1.0.4/src/ansi_string/ansi_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-24 02:56:51.000000 ansi-string-1.0.4/src/ansi_string/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:56:59.545862 ansi-string-1.0.4/src/ansi_string.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8283 2024-04-24 02:56:59.000000 ansi-string-1.0.4/src/ansi_string.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-24 02:56:59.000000 ansi-string-1.0.4/src/ansi_string.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:56:59.000000 ansi-string-1.0.4/src/ansi_string.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 02:56:59.000000 ansi-string-1.0.4/src/ansi_string.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 02:56:59.000000 ansi-string-1.0.4/src/ansi_string.egg-info/top_level.txt
```

### Comparing `ansi-string-1.0.3/LICENSE` & `ansi-string-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ansi-string-1.0.3/PKG-INFO` & `ansi-string-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansi-string
-Version: 1.0.3
+Version: 1.0.4
 Summary: ANSI String Formatter in Python for CLI Color and Style Formatting
 Home-page: https://github.com/Tails86/ansi-string
 Author: James Smith
 Author-email: jmsmith86@gmail.com
 Project-URL: Documentation, https://github.com/Tails86/ansi-string
 Project-URL: Bug Reports, https://github.com/Tails86/ansi-string/issues
 Project-URL: Source Code, https://github.com/Tails86/ansi-string
@@ -84,24 +84,25 @@
 ```py
 class AnsiString:
     def __init__(self, s:str='', *setting_or_settings:Union[List[str], str, List[int], int, List[AnsiFormat], AnsiFormat]): ...
 ```
 
 The first argument, `s`, is a string to be formatted. The next 0 to N arguments are formatting setting directives that can be applied to the entire string. These arguments can be in the form of any of the following.
 - An AnsiFormat enum (ex: `AnsiFormat.BOLD`)
+- The result of calling `AnsiFormat.rgb()`, `AnsiFormat.fg_rgb()`, `AnsiFormat.bg_rgb()`, `AnsiFormat.ul_rgb()`, or `AnsiFormat.dul_rgb()`
 - A string color or formatting name (i.e. any name of the AnsiFormat enum in lower or upper case)
-- The result of calling `AnsiFormat.rgb()`, `AnsiFormat.fg_rgb()`, `AnsiFormat.bg_rgb()`, or `AnsiFormat.ul_rgb()`
 - An `rgb(...)` function directive as a string (ex: `"rgb(255, 255, 255)"`)
     - `rgb(...)` or `fg_rgb(...)` to adjust text color
     - `bg_rgb(...)` to adjust background color
     - `ul_rgb(...)` to enable underline and set the underline color
+    - `dul_rgb(...)` to enable double underline and set the underline color
     - Value given may be either a 24-bit integer or 3 x 8-bit integers, separated by commas
     - Each given value within the parenthesis is treated as hexadecimal if the value starts with "0x", otherwise it is treated as a decimal value
 
-A formatting setting may also be any of the following, but it's not advised to specify settings these ways unless there is a specific reason to do so.
+A formatting setting may also be any of the following, but it's not advised to specify settings in any of these ways unless there is a specific reason to do so.
 - An AnsiSetting object
 - A string containing known ANSI directives (ex: `"01;31"` for BOLD and FG_RED)
     - The string will normally be parsed into separate settings unless the character "[" is the first character of the string (ex: `"[38;5;214"`)
     - Never specify the reset directive (0) because this is implicitly handled internally
 - A single ANSI directive as an integer
 
 Examples:
```

### Comparing `ansi-string-1.0.3/README.md` & `ansi-string-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,24 +56,25 @@
 ```py
 class AnsiString:
     def __init__(self, s:str='', *setting_or_settings:Union[List[str], str, List[int], int, List[AnsiFormat], AnsiFormat]): ...
 ```
 
 The first argument, `s`, is a string to be formatted. The next 0 to N arguments are formatting setting directives that can be applied to the entire string. These arguments can be in the form of any of the following.
 - An AnsiFormat enum (ex: `AnsiFormat.BOLD`)
+- The result of calling `AnsiFormat.rgb()`, `AnsiFormat.fg_rgb()`, `AnsiFormat.bg_rgb()`, `AnsiFormat.ul_rgb()`, or `AnsiFormat.dul_rgb()`
 - A string color or formatting name (i.e. any name of the AnsiFormat enum in lower or upper case)
-- The result of calling `AnsiFormat.rgb()`, `AnsiFormat.fg_rgb()`, `AnsiFormat.bg_rgb()`, or `AnsiFormat.ul_rgb()`
 - An `rgb(...)` function directive as a string (ex: `"rgb(255, 255, 255)"`)
     - `rgb(...)` or `fg_rgb(...)` to adjust text color
     - `bg_rgb(...)` to adjust background color
     - `ul_rgb(...)` to enable underline and set the underline color
+    - `dul_rgb(...)` to enable double underline and set the underline color
     - Value given may be either a 24-bit integer or 3 x 8-bit integers, separated by commas
     - Each given value within the parenthesis is treated as hexadecimal if the value starts with "0x", otherwise it is treated as a decimal value
 
-A formatting setting may also be any of the following, but it's not advised to specify settings these ways unless there is a specific reason to do so.
+A formatting setting may also be any of the following, but it's not advised to specify settings in any of these ways unless there is a specific reason to do so.
 - An AnsiSetting object
 - A string containing known ANSI directives (ex: `"01;31"` for BOLD and FG_RED)
     - The string will normally be parsed into separate settings unless the character "[" is the first character of the string (ex: `"[38;5;214"`)
     - Never specify the reset directive (0) because this is implicitly handled internally
 - A single ANSI directive as an integer
 
 Examples:
```

### Comparing `ansi-string-1.0.3/setup.py` & `ansi-string-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `ansi-string-1.0.3/src/ansi_string.egg-info/PKG-INFO` & `ansi-string-1.0.4/src/ansi_string.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansi-string
-Version: 1.0.3
+Version: 1.0.4
 Summary: ANSI String Formatter in Python for CLI Color and Style Formatting
 Home-page: https://github.com/Tails86/ansi-string
 Author: James Smith
 Author-email: jmsmith86@gmail.com
 Project-URL: Documentation, https://github.com/Tails86/ansi-string
 Project-URL: Bug Reports, https://github.com/Tails86/ansi-string/issues
 Project-URL: Source Code, https://github.com/Tails86/ansi-string
@@ -84,24 +84,25 @@
 ```py
 class AnsiString:
     def __init__(self, s:str='', *setting_or_settings:Union[List[str], str, List[int], int, List[AnsiFormat], AnsiFormat]): ...
 ```
 
 The first argument, `s`, is a string to be formatted. The next 0 to N arguments are formatting setting directives that can be applied to the entire string. These arguments can be in the form of any of the following.
 - An AnsiFormat enum (ex: `AnsiFormat.BOLD`)
+- The result of calling `AnsiFormat.rgb()`, `AnsiFormat.fg_rgb()`, `AnsiFormat.bg_rgb()`, `AnsiFormat.ul_rgb()`, or `AnsiFormat.dul_rgb()`
 - A string color or formatting name (i.e. any name of the AnsiFormat enum in lower or upper case)
-- The result of calling `AnsiFormat.rgb()`, `AnsiFormat.fg_rgb()`, `AnsiFormat.bg_rgb()`, or `AnsiFormat.ul_rgb()`
 - An `rgb(...)` function directive as a string (ex: `"rgb(255, 255, 255)"`)
     - `rgb(...)` or `fg_rgb(...)` to adjust text color
     - `bg_rgb(...)` to adjust background color
     - `ul_rgb(...)` to enable underline and set the underline color
+    - `dul_rgb(...)` to enable double underline and set the underline color
     - Value given may be either a 24-bit integer or 3 x 8-bit integers, separated by commas
     - Each given value within the parenthesis is treated as hexadecimal if the value starts with "0x", otherwise it is treated as a decimal value
 
-A formatting setting may also be any of the following, but it's not advised to specify settings these ways unless there is a specific reason to do so.
+A formatting setting may also be any of the following, but it's not advised to specify settings in any of these ways unless there is a specific reason to do so.
 - An AnsiSetting object
 - A string containing known ANSI directives (ex: `"01;31"` for BOLD and FG_RED)
     - The string will normally be parsed into separate settings unless the character "[" is the first character of the string (ex: `"[38;5;214"`)
     - Never specify the reset directive (0) because this is implicitly handled internally
 - A single ANSI directive as an integer
 
 Examples:
```

