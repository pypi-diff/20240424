# Comparing `tmp/dav_tools-0.1.2.tar.gz` & `tmp/dav_tools-0.1.3.tar.gz`

## Comparing `dav_tools-0.1.2.tar` & `dav_tools-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 dav_tools-0.1.2/.readthedocs.yaml
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 dav_tools-0.1.2/Makefile
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dav_tools-0.1.2/requirements.txt
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 dav_tools-0.1.2/docs/Makefile
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 dav_tools-0.1.2/docs/conf.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 dav_tools-0.1.2/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 dav_tools-0.1.2/docs/make.bat
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dav_tools-0.1.2/docs/requirements.txt
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 dav_tools-0.1.2/src/dav_tools/__init__.py
--rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 dav_tools-0.1.2/src/dav_tools/_arg_parser.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 dav_tools-0.1.2/src/dav_tools/_text_format.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 dav_tools-0.1.2/src/dav_tools/commands.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 dav_tools-0.1.2/src/dav_tools/devtools.py
--rw-r--r--   0        0        0     7986 2020-02-02 00:00:00.000000 dav_tools-0.1.2/src/dav_tools/messages.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 dav_tools-0.1.2/src/dav_tools/requirements.py
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 dav_tools-0.1.2/src/dav_tools/text_format.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dav_tools-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 dav_tools-0.1.2/tests/test_messages.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 dav_tools-0.1.2/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 dav_tools-0.1.2/LICENSE
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 dav_tools-0.1.2/README.md
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 dav_tools-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 dav_tools-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 dav_tools-0.1.3/.readthedocs.yaml
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 dav_tools-0.1.3/Makefile
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dav_tools-0.1.3/requirements.txt
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 dav_tools-0.1.3/docs/Makefile
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 dav_tools-0.1.3/docs/conf.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 dav_tools-0.1.3/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 dav_tools-0.1.3/docs/make.bat
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dav_tools-0.1.3/docs/requirements.txt
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 dav_tools-0.1.3/src/dav_tools/__init__.py
+-rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 dav_tools-0.1.3/src/dav_tools/_arg_parser.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 dav_tools-0.1.3/src/dav_tools/_text_format.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 dav_tools-0.1.3/src/dav_tools/commands.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 dav_tools-0.1.3/src/dav_tools/devtools.py
+-rw-r--r--   0        0        0     8079 2020-02-02 00:00:00.000000 dav_tools-0.1.3/src/dav_tools/messages.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 dav_tools-0.1.3/src/dav_tools/requirements.py
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 dav_tools-0.1.3/src/dav_tools/text_format.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dav_tools-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 dav_tools-0.1.3/tests/test_messages.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 dav_tools-0.1.3/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 dav_tools-0.1.3/LICENSE
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 dav_tools-0.1.3/README.md
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 dav_tools-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 dav_tools-0.1.3/PKG-INFO
```

### Comparing `dav_tools-0.1.2/.readthedocs.yaml` & `dav_tools-0.1.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.2/Makefile` & `dav_tools-0.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.2/docs/Makefile` & `dav_tools-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.2/docs/conf.py` & `dav_tools-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.2/docs/index.rst` & `dav_tools-0.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.2/docs/make.bat` & `dav_tools-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.2/src/dav_tools/_arg_parser.py` & `dav_tools-0.1.3/src/dav_tools/_arg_parser.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.2/src/dav_tools/_text_format.py` & `dav_tools-0.1.3/src/dav_tools/_text_format.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.2/src/dav_tools/commands.py` & `dav_tools-0.1.3/src/dav_tools/commands.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.2/src/dav_tools/devtools.py` & `dav_tools-0.1.3/src/dav_tools/devtools.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.2/src/dav_tools/messages.py` & `dav_tools-0.1.3/src/dav_tools/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,17 +208,19 @@
     '''
 
     message(f'{question}{end}',
             icon='?',
             icon_options=[
                 TextFormat.Color.PURPLE
             ],
+            default_text_options=[TextFormat.Color.PURPLE],
             end='')
     
     return _input_colored(
+        TextFormat.Color.PURPLE,
         TextFormat.Style.ITALIC,
     )
 
 def ask_continue(text: str=None):
     '''
     Prints a question asking the user if they want to continue executing the program:
     a positive answer makes the program continues its normal execution;
```

### Comparing `dav_tools-0.1.2/src/dav_tools/requirements.py` & `dav_tools-0.1.3/src/dav_tools/requirements.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.2/src/dav_tools/text_format.py` & `dav_tools-0.1.3/src/dav_tools/text_format.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,17 +68,23 @@
     '''
     Ask input from a user using specified styling options.
 
     :param format_options: Text styling options.
 
     :returns: User input.
     '''
-    _set_format(*format_options, file=_sys.stderr)
-    result = input()
-    _set_format(TextFormat.RESET)
+
+    result = None
+
+    try:
+        _set_format(*format_options, file=_sys.stderr)
+        result = input()
+    except KeyboardInterrupt as e:
+        _set_format(TextFormat.RESET, file=_sys.stderr)
+        raise e
 
     return result
 
 def clear_line(file=_sys.stdout, flush=False):
     '''
     Clears the current line from any text of formatting.
     Not really suitable for files.
```

### Comparing `dav_tools-0.1.2/tests/test_messages.py` & `dav_tools-0.1.3/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.2/LICENSE` & `dav_tools-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dav_tools-0.1.2/pyproject.toml` & `dav_tools-0.1.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dav_tools"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Davide Ponzini", email="davide.ponzini95@gmail.com" },
 ]
 description = "Various utilies to aid in program development."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dav_tools-0.1.2/PKG-INFO` & `dav_tools-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dav_tools
-Version: 0.1.2
+Version: 0.1.3
 Summary: Various utilies to aid in program development.
 Project-URL: Repository, https://github.com/DavidePonzini/dav-utils
 Project-URL: Documentation, https://dav-tools.readthedocs.io/en/latest/index.html
 Project-URL: Bug Tracker, https://github.com/DavidePonzini/dav-utils/issues
 Author-email: Davide Ponzini <davide.ponzini95@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

