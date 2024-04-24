# Comparing `tmp/dav_tools-0.1.1.tar.gz` & `tmp/dav_tools-0.1.2.tar.gz`

## Comparing `dav_tools-0.1.1.tar` & `dav_tools-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 dav_tools-0.1.1/.readthedocs.yaml
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 dav_tools-0.1.1/Makefile
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dav_tools-0.1.1/requirements.txt
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 dav_tools-0.1.1/docs/Makefile
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 dav_tools-0.1.1/docs/conf.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 dav_tools-0.1.1/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 dav_tools-0.1.1/docs/make.bat
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dav_tools-0.1.1/docs/requirements.txt
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 dav_tools-0.1.1/src/dav_tools/__init__.py
--rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 dav_tools-0.1.1/src/dav_tools/_arg_parser.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 dav_tools-0.1.1/src/dav_tools/_text_format.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 dav_tools-0.1.1/src/dav_tools/commands.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 dav_tools-0.1.1/src/dav_tools/devtools.py
--rw-r--r--   0        0        0     7900 2020-02-02 00:00:00.000000 dav_tools-0.1.1/src/dav_tools/messages.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 dav_tools-0.1.1/src/dav_tools/requirements.py
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 dav_tools-0.1.1/src/dav_tools/text_color.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dav_tools-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 dav_tools-0.1.1/tests/test_messages.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 dav_tools-0.1.1/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 dav_tools-0.1.1/LICENSE
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 dav_tools-0.1.1/README.md
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 dav_tools-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 dav_tools-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 dav_tools-0.1.2/.readthedocs.yaml
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 dav_tools-0.1.2/Makefile
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dav_tools-0.1.2/requirements.txt
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 dav_tools-0.1.2/docs/Makefile
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 dav_tools-0.1.2/docs/conf.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 dav_tools-0.1.2/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 dav_tools-0.1.2/docs/make.bat
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dav_tools-0.1.2/docs/requirements.txt
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 dav_tools-0.1.2/src/dav_tools/__init__.py
+-rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 dav_tools-0.1.2/src/dav_tools/_arg_parser.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 dav_tools-0.1.2/src/dav_tools/_text_format.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 dav_tools-0.1.2/src/dav_tools/commands.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 dav_tools-0.1.2/src/dav_tools/devtools.py
+-rw-r--r--   0        0        0     7986 2020-02-02 00:00:00.000000 dav_tools-0.1.2/src/dav_tools/messages.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 dav_tools-0.1.2/src/dav_tools/requirements.py
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 dav_tools-0.1.2/src/dav_tools/text_format.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dav_tools-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 dav_tools-0.1.2/tests/test_messages.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 dav_tools-0.1.2/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 dav_tools-0.1.2/LICENSE
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 dav_tools-0.1.2/README.md
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 dav_tools-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 dav_tools-0.1.2/PKG-INFO
```

### Comparing `dav_tools-0.1.1/.readthedocs.yaml` & `dav_tools-0.1.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.1/Makefile` & `dav_tools-0.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.1/docs/Makefile` & `dav_tools-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.1/docs/conf.py` & `dav_tools-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.1/docs/index.rst` & `dav_tools-0.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.1/docs/make.bat` & `dav_tools-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.1/src/dav_tools/_arg_parser.py` & `dav_tools-0.1.2/src/dav_tools/_arg_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''Customized argument parser.'''
 
 import argparse
-from . import text_color
+from . import text_format
 
 class ArgumentAction:
     STORE = 'store'
     STORE_CONST = 'store_const'
     STORE_TRUE = 'store_true'
     STORE_FALSE = 'store_false'
     APPEND = 'append'
@@ -56,15 +56,15 @@
         Set information about the developer of the project.
         These informations will be displayed at the bottom of the --help command. 
 
         :param name: Name to be displayed
         :param email: Email address to be displayed
         '''
 
-        self.parser.epilog = text_color.get_colored_text(f'--Developed by {name} ({email})', text_color.TextFormat.Style.ITALIC)
+        self.parser.epilog = text_format.format_text(f'--Developed by {name} ({email})', text_format.TextFormat.Style.ITALIC)
 
     @property
     def args(self) -> argparse.Namespace:
         '''
         Parse and return arguments specified on command line.
 
         :returns: The arguments
@@ -84,15 +84,15 @@
 
         if name in self.__groups:
             return self.__groups[name] 
 
         if description is None:
             group = self.parser.add_argument_group(name)
         else:
-            group = self.parser.add_argument_group(name, text_color.get_colored_text(description, text_color.TextFormat.Style.ITALIC))
+            group = self.parser.add_argument_group(name, text_format.format_text(description, text_format.TextFormat.Style.ITALIC))
 
         self.__groups[name] = group
         return group
 
     def add_mutually_exclusive_group(self, parent: argparse._ArgumentGroup = None) -> argparse._MutuallyExclusiveGroup:
         '''
         Create a mutually exclusive argument group.
```

### Comparing `dav_tools-0.1.1/src/dav_tools/_text_format.py` & `dav_tools-0.1.2/src/dav_tools/_text_format.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.1/src/dav_tools/commands.py` & `dav_tools-0.1.2/src/dav_tools/commands.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.1/src/dav_tools/devtools.py` & `dav_tools-0.1.2/src/dav_tools/devtools.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.1/src/dav_tools/messages.py` & `dav_tools-0.1.2/src/dav_tools/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 '''Print messages on screen and ask for user input.'''
 
 import sys as _sys
 
-from .text_color import TextFormat
-from .text_color import print_colored_text as _print_colored_text
-from .text_color import input_colored as _input_colored
-from .text_color import clear_line as _clear_line
+from .text_format import TextFormat
+from .text_format import print_text as _print_colored_text
+from .text_format import input_formatted as _input_colored
+from .text_format import clear_line as _clear_line
 
 
 def message(*text: str | object,
             text_min_len: list[int] = [], default_text_options: list = [], additional_text_options: list[list] = [[]],
             icon: str = None, icon_options: list = [], blink: bool = False,
             end: str = '\n', file = _sys.stderr):
     '''
@@ -68,17 +68,20 @@
     :param text_options: Styling options applied to single messages.
     :param blink: If True, the icon blinks.
     '''
 
     message(*text,
             icon='*',
             icon_options=[
-                TextFormat.Color.BLUE
+                TextFormat.Color.CYAN
             ],
             text_min_len=text_min_len,
+            default_text_options=[
+                TextFormat.Color.CYAN
+            ],
             additional_text_options=text_options,
             blink=blink)
 
 
 def progress(*text: str | object, text_min_len: list[int] = [], text_options: list[list] = [[]]):
     '''
     Message indicating an action which is still happening.
```

### Comparing `dav_tools-0.1.1/src/dav_tools/requirements.py` & `dav_tools-0.1.2/src/dav_tools/requirements.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.1/src/dav_tools/text_color.py` & `dav_tools-0.1.2/src/dav_tools/text_format.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 '''Utilities for handling text formatting.'''
 
 import sys as _sys
 import os as _os
 from ._text_format import TextFormat
 
 
-def get_format(*options) -> str:
+def _get_format(*options) -> str:
     '''
     Get the format string generated from the arguments.
     Needed for manually setting text style. Otherwise use ``set_format()``.
 
     :param option: Text styling options.
 
     :returns: The format string corresponding to the options.
@@ -18,67 +18,67 @@
     result = ''
 
     for option in options:
         result += option.decode()
 
     return result
 
-def set_format(*options, file = _sys.stdout):
+def _set_format(*options, file = _sys.stdout):
     '''
     Set text styling.
 
     :param option: Text styling options.
     :param file: Where to set text styling.
     '''
 
     for option in options:
         print(option.decode(), end='', file=file)
 
-def get_colored_text(text: str, *format_options) -> str:
+def format_text(text: str, *format_options) -> str:
     '''
     Return a styled text.
 
     :param text: Text to print.
     :param format_options: Text styling options.
 
     :returns: The text properly styled.
     '''
     
     result = ''
-    result += get_format(*format_options)
+    result += _get_format(*format_options)
     result += text
-    result += get_format(TextFormat.RESET)
+    result += _get_format(TextFormat.RESET)
 
     return result
 
-def print_colored_text(text: str = '', *format_options, end: str='\n', file=_sys.stdout, flush=False):
+def print_text(text: str = '', *format_options, end: str='\n', file=_sys.stdout, flush=False):
     '''
     Print a styled text.
 
     :param text: Text to print.
     :param format_options: Text styling options.
     :param end: Character to be printed after the text.
     :param file: Where to print the text.
     :param flush: Whether to flush the stream after printing.
     '''
 
-    text = get_colored_text(text, *format_options)
+    text = format_text(text, *format_options)
     print(text, end=end, file=file, flush=flush)
 
-def input_colored(*format_options) -> str:
+def input_formatted(*format_options) -> str:
     '''
     Ask input from a user using specified styling options.
 
     :param format_options: Text styling options.
 
     :returns: User input.
     '''
-    set_format(*format_options, file=_sys.stderr)
+    _set_format(*format_options, file=_sys.stderr)
     result = input()
-    set_format(TextFormat.RESET)
+    _set_format(TextFormat.RESET)
 
     return result
 
 def clear_line(file=_sys.stdout, flush=False):
     '''
     Clears the current line from any text of formatting.
     Not really suitable for files.
```

### Comparing `dav_tools-0.1.1/tests/test_messages.py` & `dav_tools-0.1.2/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.1/LICENSE` & `dav_tools-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.1/pyproject.toml` & `dav_tools-0.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dav_tools"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Davide Ponzini", email="davide.ponzini95@gmail.com" },
 ]
 description = "Various utilies to aid in program development."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dav_tools-0.1.1/PKG-INFO` & `dav_tools-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: dav_tools
-Version: 0.1.1
+Version: 0.1.2
 Summary: Various utilies to aid in program development.
 Project-URL: Repository, https://github.com/DavidePonzini/dav-utils
 Project-URL: Documentation, https://dav-tools.readthedocs.io/en/latest/index.html
 Project-URL: Bug Tracker, https://github.com/DavidePonzini/dav-utils/issues
 Author-email: Davide Ponzini <davide.ponzini95@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

