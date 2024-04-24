# Comparing `tmp/cli_fragments-1.0.0.tar.gz` & `tmp/cli_fragments-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli_fragments-1.0.0.tar", last modified: Tue Apr 23 17:27:54 2024, max compression
+gzip compressed data, was "cli_fragments-1.1.0.tar", last modified: Tue Apr 23 17:32:47 2024, max compression
```

## Comparing `cli_fragments-1.0.0.tar` & `cli_fragments-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sal        (501) staff       (20)        0 2024-04-23 17:27:54.847801 cli_fragments-1.0.0/
--rw-r--r--   0 sal        (501) staff       (20)    35149 2024-04-23 16:11:09.000000 cli_fragments-1.0.0/LICENSE
--rw-r--r--   0 sal        (501) staff       (20)     1317 2024-04-23 17:27:54.847577 cli_fragments-1.0.0/PKG-INFO
--rw-r--r--   0 sal        (501) staff       (20)      914 2024-04-23 16:30:36.000000 cli_fragments-1.0.0/README.md
-drwxr-xr-x   0 sal        (501) staff       (20)        0 2024-04-23 17:27:54.846863 cli_fragments-1.0.0/cli_fragments/
--rw-r--r--   0 sal        (501) staff       (20)       35 2024-04-23 17:20:15.000000 cli_fragments-1.0.0/cli_fragments/__init__.py
--rw-r--r--   0 sal        (501) staff       (20)     1312 2024-04-23 17:13:01.000000 cli_fragments-1.0.0/cli_fragments/cli_fragments.py
-drwxr-xr-x   0 sal        (501) staff       (20)        0 2024-04-23 17:27:54.847391 cli_fragments-1.0.0/cli_fragments.egg-info/
--rw-r--r--   0 sal        (501) staff       (20)     1317 2024-04-23 17:27:54.000000 cli_fragments-1.0.0/cli_fragments.egg-info/PKG-INFO
--rw-r--r--   0 sal        (501) staff       (20)      231 2024-04-23 17:27:54.000000 cli_fragments-1.0.0/cli_fragments.egg-info/SOURCES.txt
--rw-r--r--   0 sal        (501) staff       (20)        1 2024-04-23 17:27:54.000000 cli_fragments-1.0.0/cli_fragments.egg-info/dependency_links.txt
--rw-r--r--   0 sal        (501) staff       (20)       14 2024-04-23 17:27:54.000000 cli_fragments-1.0.0/cli_fragments.egg-info/top_level.txt
--rw-r--r--   0 sal        (501) staff       (20)       38 2024-04-23 17:27:54.847842 cli_fragments-1.0.0/setup.cfg
--rw-r--r--   0 sal        (501) staff       (20)      727 2024-04-23 17:26:07.000000 cli_fragments-1.0.0/setup.py
+drwxr-xr-x   0 sal        (501) staff       (20)        0 2024-04-23 17:32:47.494794 cli_fragments-1.1.0/
+-rw-r--r--   0 sal        (501) staff       (20)    35149 2024-04-23 16:11:09.000000 cli_fragments-1.1.0/LICENSE
+-rw-r--r--   0 sal        (501) staff       (20)     1887 2024-04-23 17:32:47.494625 cli_fragments-1.1.0/PKG-INFO
+-rw-r--r--   0 sal        (501) staff       (20)     1485 2024-04-23 17:32:31.000000 cli_fragments-1.1.0/README.md
+drwxr-xr-x   0 sal        (501) staff       (20)        0 2024-04-23 17:32:47.493889 cli_fragments-1.1.0/cli_fragments/
+-rw-r--r--   0 sal        (501) staff       (20)       53 2024-04-23 17:30:31.000000 cli_fragments-1.1.0/cli_fragments/__init__.py
+-rw-r--r--   0 sal        (501) staff       (20)     1545 2024-04-23 17:30:14.000000 cli_fragments-1.1.0/cli_fragments/cli_fragments.py
+drwxr-xr-x   0 sal        (501) staff       (20)        0 2024-04-23 17:32:47.494437 cli_fragments-1.1.0/cli_fragments.egg-info/
+-rw-r--r--   0 sal        (501) staff       (20)     1887 2024-04-23 17:32:47.000000 cli_fragments-1.1.0/cli_fragments.egg-info/PKG-INFO
+-rw-r--r--   0 sal        (501) staff       (20)      231 2024-04-23 17:32:47.000000 cli_fragments-1.1.0/cli_fragments.egg-info/SOURCES.txt
+-rw-r--r--   0 sal        (501) staff       (20)        1 2024-04-23 17:32:47.000000 cli_fragments-1.1.0/cli_fragments.egg-info/dependency_links.txt
+-rw-r--r--   0 sal        (501) staff       (20)       14 2024-04-23 17:32:47.000000 cli_fragments-1.1.0/cli_fragments.egg-info/top_level.txt
+-rw-r--r--   0 sal        (501) staff       (20)       38 2024-04-23 17:32:47.494837 cli_fragments-1.1.0/setup.cfg
+-rw-r--r--   0 sal        (501) staff       (20)      727 2024-04-23 17:32:44.000000 cli_fragments-1.1.0/setup.py
```

### Comparing `cli_fragments-1.0.0/LICENSE` & `cli_fragments-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cli_fragments-1.0.0/PKG-INFO` & `cli_fragments-1.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-fragments
-Version: 1.0.0
+Version: 1.1.0
 Summary: Awesome CLI input and output functions for Python 3.x scripts.
 Author: Luca Saladino
 Author-email: sal65535@protonmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Freeware
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -21,7 +21,36 @@
  - `error`: a red message having `[✕]` as prefix
  - `success`: a green message having `[✓]` as prefix
  - `warning`: a yellow message having `[!]` as prefix
  - `text`: a standard text in terminal having the proper padding
  - `debug`: a default color message having `[#]` as prefix
  - `notice`: a blue message having `[~]` as prefix
  - `ask`: a qustion to the user having `[?]` as prefix. The input value can be optionally validated passing a `validator` callback
+
+## Usage
+
+```shell
+pip install cli-fragments
+```
+
+```python
+from cli_fragments import CliFragments
+
+
+def validator_function(value: str):
+    if value == "wrong":
+        raise ValueError
+
+
+io = CliFragments()
+
+io.debug("This is a debug message.")
+io.notice("This is a notice message.")
+io.warning("This is a warning message.")
+io.error("This is an error message.")
+io.success("This is a success message.")
+io.text("This is padded raw text message.")
+
+io.ask("This is a user question.", None, None)
+
+io.ask("This is a user question.", "default", validator_function)
+```
```

### Comparing `cli_fragments-1.0.0/cli_fragments/cli_fragments.py` & `cli_fragments-1.1.0/cli_fragments/cli_fragments.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,75 +1,70 @@
 from typing import Callable
 
 
-def error(text: str):
-    """Prints an error statement."""
+class CliFragments:
+    def error(self, text: str):
+        """Prints an error statement."""
 
-    line = "\033[31m[✕] " + text + "\033[m"
-    line = "\n" + line
+        line = "\033[31m[✕] " + text + "\033[m"
+        line = "\n" + line
 
-    print(line)
+        print(line)
 
+    def success(self, text: str):
+        """Prints a success statement."""
 
-def success(text: str):
-    """Prints a success statement."""
+        line = "\033[32m[✓] " + text + "\033[m"
+        line = "\n" + line
 
-    line = "\033[32m[✓] " + text + "\033[m"
-    line = "\n" + line
+        print(line)
 
-    print(line)
+    def warning(self, text: str):
+        """Prints a warning statement."""
 
+        line = "\033[33m[!] " + text + "\033[m"
+        line = "\n" + line
 
-def warning(text: str):
-    """Prints a warning statement."""
+        print(line)
 
-    line = "\033[33m[!] " + text + "\033[m"
-    line = "\n" + line
+    def text(self, text: str):
+        """Prints a text statement."""
 
-    print(line)
+        line = text
+        line = "\n" + line
 
+        print(line)
 
-def text(text: str):
-    """Prints a text statement."""
+    def debug(self, text: str):
+        """Prints a notice statement."""
 
-    line = text
-    line = "\n" + line
+        line = "[#] " + text
+        line = "\n" + line
 
-    print(line)
+        print(line)
 
+    def notice(self, text: str):
+        """Prints a notice statement."""
 
-def debug(text: str):
-    """Prints a notice statement."""
+        line = "\033[34m[~] " + text + "\033[m"
+        line = "\n" + line
 
-    line = "[#] " + text
-    line = "\n" + line
+        print(line)
 
-    print(line)
+    def ask(self, question: str, default, validator=Callable[[str], str]):
+        """Asks to the user an input and validates the value with the given validator function."""
 
+        line = "\n[?] " + question
 
-def notice(text: str):
-    """Prints a notice statement."""
+        if default:
+            line += " [" + str(default) + "]"
 
-    line = "\033[34m[~] " + text + "\033[m"
-    line = "\n" + line
+        line += ": "
 
-    print(line)
+        while True:
+            value = str(input(line))
 
-
-def ask(question: str, default, validator=Callable[[str], str]):
-    """Asks to the user an input and validates the value with the given validator function."""
-
-    line = "\n[?] " + question
-
-    if default:
-        line += " [" + str(default) + "]"
-
-    line += ": "
-
-    while True:
-        value = str(input(line))
-
-        try:
-            validator(value)
-            return value
-        except ValueError as e:
-            error(str(e))
+            try:
+                validator(value)
+                return value
+            except ValueError as e:
+                self.error(str(e))
```

### Comparing `cli_fragments-1.0.0/cli_fragments.egg-info/PKG-INFO` & `cli_fragments-1.1.0/cli_fragments.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cli-fragments
-Version: 1.0.0
+Version: 1.1.0
 Summary: Awesome CLI input and output functions for Python 3.x scripts.
 Author: Luca Saladino
 Author-email: sal65535@protonmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Freeware
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -21,7 +21,36 @@
  - `error`: a red message having `[✕]` as prefix
  - `success`: a green message having `[✓]` as prefix
  - `warning`: a yellow message having `[!]` as prefix
  - `text`: a standard text in terminal having the proper padding
  - `debug`: a default color message having `[#]` as prefix
  - `notice`: a blue message having `[~]` as prefix
  - `ask`: a qustion to the user having `[?]` as prefix. The input value can be optionally validated passing a `validator` callback
+
+## Usage
+
+```shell
+pip install cli-fragments
+```
+
+```python
+from cli_fragments import CliFragments
+
+
+def validator_function(value: str):
+    if value == "wrong":
+        raise ValueError
+
+
+io = CliFragments()
+
+io.debug("This is a debug message.")
+io.notice("This is a notice message.")
+io.warning("This is a warning message.")
+io.error("This is an error message.")
+io.success("This is a success message.")
+io.text("This is padded raw text message.")
+
+io.ask("This is a user question.", None, None)
+
+io.ask("This is a user question.", "default", validator_function)
+```
```

### Comparing `cli_fragments-1.0.0/setup.py` & `cli_fragments-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="cli-fragments",
-    version="1.0.0",
+    version="1.1.0",
     author="Luca Saladino",
     author_email="sal65535@protonmail.com",
     description="Awesome CLI input and output functions for Python 3.x scripts.",
     packages=["cli_fragments"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Freeware",
```

