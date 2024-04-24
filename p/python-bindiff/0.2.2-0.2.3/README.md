# Comparing `tmp/python-bindiff-0.2.2.tar.gz` & `tmp/python_bindiff-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-bindiff-0.2.2.tar", last modified: Fri Feb 23 21:11:32 2024, max compression
+gzip compressed data, was "python_bindiff-0.2.3.tar", last modified: Wed Apr 24 13:32:51 2024, max compression
```

## Comparing `python-bindiff-0.2.2.tar` & `python_bindiff-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:11:32.384779 python-bindiff-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-23 21:11:23.000000 python-bindiff-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-02-23 21:11:32.384779 python-bindiff-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-02-23 21:11:23.000000 python-bindiff-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-02-23 21:11:23.000000 python-bindiff-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 21:11:32.384779 python-bindiff-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:11:32.380779 python-bindiff-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:11:32.380779 python-bindiff-0.2.2/src/bindiff/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-23 21:11:23.000000 python-bindiff-0.2.2/src/bindiff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-02-23 21:11:23.000000 python-bindiff-0.2.2/src/bindiff/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15218 2024-02-23 21:11:23.000000 python-bindiff-0.2.2/src/bindiff/bindiff.py
--rw-r--r--   0 runner    (1001) docker     (127)    18903 2024-02-23 21:11:23.000000 python-bindiff-0.2.2/src/bindiff/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-02-23 21:11:23.000000 python-bindiff-0.2.2/src/bindiff/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:11:32.384779 python-bindiff-0.2.2/src/python_bindiff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-02-23 21:11:32.000000 python-bindiff-0.2.2/src/python_bindiff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-02-23 21:11:32.000000 python-bindiff-0.2.2/src/python_bindiff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 21:11:32.000000 python-bindiff-0.2.2/src/python_bindiff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-23 21:11:32.000000 python-bindiff-0.2.2/src/python_bindiff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-23 21:11:32.000000 python-bindiff-0.2.2/src/python_bindiff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-23 21:11:32.000000 python-bindiff-0.2.2/src/python_bindiff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:32:51.847669 python_bindiff-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 13:32:46.000000 python_bindiff-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-24 13:32:51.847669 python_bindiff-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-24 13:32:46.000000 python_bindiff-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-24 13:32:46.000000 python_bindiff-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:32:51.847669 python_bindiff-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:32:51.843669 python_bindiff-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:32:51.847669 python_bindiff-0.2.3/src/bindiff/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-24 13:32:46.000000 python_bindiff-0.2.3/src/bindiff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-24 13:32:46.000000 python_bindiff-0.2.3/src/bindiff/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15720 2024-04-24 13:32:46.000000 python_bindiff-0.2.3/src/bindiff/bindiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18903 2024-04-24 13:32:46.000000 python_bindiff-0.2.3/src/bindiff/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-24 13:32:46.000000 python_bindiff-0.2.3/src/bindiff/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:32:51.847669 python_bindiff-0.2.3/src/python_bindiff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-24 13:32:51.000000 python_bindiff-0.2.3/src/python_bindiff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-24 13:32:51.000000 python_bindiff-0.2.3/src/python_bindiff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:32:51.000000 python_bindiff-0.2.3/src/python_bindiff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-24 13:32:51.000000 python_bindiff-0.2.3/src/python_bindiff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-24 13:32:51.000000 python_bindiff-0.2.3/src/python_bindiff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 13:32:51.000000 python_bindiff-0.2.3/src/python_bindiff.egg-info/top_level.txt
```

### Comparing `python-bindiff-0.2.2/LICENSE` & `python_bindiff-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-bindiff-0.2.2/PKG-INFO` & `python_bindiff-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bindiff
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python wrapper to manipulate bindiff files
 Author-email: Robin David <rdavid@quarkslab.com>
 License: Apache Software License (Apache License, Version 2)
 Project-URL: Homepage, https://github.com/quarkslab/python-bindiff
 Project-URL: Repository, https://github.com/quarkslab/python-bindiff
 Project-URL: Documentation, https://diffing.quarkslab.com/differs/bindiff.html#python-bindiff
 Project-URL: Bug Tracker, https://github.com/quarkslab/python-bindiff/issues
@@ -13,15 +13,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-magic; os_name != "nt"
 Requires-Dist: python-magic-bin; os_name == "nt"
 Requires-Dist: click
-Requires-Dist: python-binexport>=0.2.0
+Requires-Dist: python-binexport>=0.3.3
 
 # Python Bindiff
 
 ``python-bindiff`` is a python module aiming to give a friendly interface to launch
 and manipulate bindiff between two binary iles.
 
 How it works ?
```

### Comparing `python-bindiff-0.2.2/README.md` & `python_bindiff-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `python-bindiff-0.2.2/pyproject.toml` & `python_bindiff-0.2.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 
 [project]
 name = "python-bindiff"
 description = "Python wrapper to manipulate bindiff files"
 authors = [{ name = "Robin David", email = "rdavid@quarkslab.com" }]
 license = { text = "Apache Software License (Apache License, Version 2)" }
 readme = { file = "README.md", content-type = "text/markdown" }
-version = '0.2.2'
+version = '0.2.3'
 requires-python = ">=3.9"
 dependencies = [
     "python-magic; os_name!='nt'",
     "python-magic-bin; os_name=='nt'",
     'click',
-    'python-binexport>=0.2.0',
+    'python-binexport>=0.3.3',
 ]
 classifiers = [
     'Topic :: Security',
     'Environment :: Console',
     'Operating System :: OS Independent',
 ]
```

### Comparing `python-bindiff-0.2.2/src/bindiff/__main__.py` & `python_bindiff-0.2.3/src/bindiff/__main__.py`

 * *Files identical despite different names*

### Comparing `python-bindiff-0.2.2/src/bindiff/bindiff.py` & `python_bindiff-0.2.3/src/bindiff/bindiff.py`

 * *Files 9% similar despite different names*

```diff
@@ -141,16 +141,16 @@
     ) -> list[BasicBlockBinExport]:
         bbs = []
         for bb_addr, bb in function.items():
             if maps := map.get(bb_addr):
                 # The block has been match but in another function thus unmatched here
                 if function.addr not in maps:
                     bbs.append(bb)
-                else:
-                    bbs.append(bb)
+            else:
+                bbs.append(bb)
         return bbs
 
     def primary_unmatched_basic_block(
         self, function: FunctionBinExport
     ) -> list[BasicBlockBinExport]:
         """
         Return a list of the unmatched basic blocks in the provided function.
@@ -322,52 +322,60 @@
             if not found:
                 logging.error("diff file .BinExport not found")
                 return False
         shutil.rmtree(tmp_dir, ignore_errors=True)
         return True
 
     @staticmethod
-    def from_binary_files(p1_path: str, p2_path: str, diff_out: str) -> Optional["BinDiff"]:
+    def from_binary_files(p1_path: str, p2_path: str, diff_out: str,
+                          override: bool = False) -> Optional["BinDiff"]:
         """
         Diff two executable files. Thus it export .BinExport files from IDA
         and then diff the two resulting files in BinDiff.
 
         :param p1_path: primary binary file to diff
         :param p2_path: secondary binary file to diff
         :param diff_out: output file for the diff
+        :param override: override Binexports files and diffing
         :return: BinDiff object representing the diff
         """
 
-        p1 = ProgramBinExport.from_binary_file(p1_path)
-        p2 = ProgramBinExport.from_binary_file(p2_path)
-        p1_binexport = Path(f"{p1_path}.BinExport")
-        p2_binexport = Path(f"{p2_path}.BinExport")
+        p1 = ProgramBinExport.from_binary_file(p1_path, override=override)
+        p2 = ProgramBinExport.from_binary_file(p2_path, override=override)
         if p1 and p2:
-            retcode = BinDiff.raw_diffing(p1_binexport, p2_binexport, diff_out)
-            return BinDiff(p1, p2, diff_out) if retcode else None
+            return BinDiff.from_binexport_files(p1, p2, diff_out, override=override)
         else:
             logging.error("p1 or p2 could not have been 'binexported'")
             return None
 
     @staticmethod
     def from_binexport_files(
-        p1_binexport: str, p2_binexport: str, diff_out: str
+        p1_binexport: Union[ProgramBinExport, str],
+        p2_binexport: Union[ProgramBinExport, str],
+        diff_out: str,
+        override: bool = False
     ) -> Optional["BinDiff"]:
         """
         Diff two binexport files. Diff the two binexport files with bindiff
         and then load a BinDiff instance.
 
-        :param p1_binexport: primary binexport file to diff
-        :param p2_binexport: secondary binexport file to diff
+        :param p1_binexport: primary binexport file to diff (path or object)
+        :param p2_binexport: secondary binexport file to diff (path or object)
         :param diff_out: output file for the diff
+        :param override: override Binexports files and diffing
         :return: BinDiff object representing the diff
         """
+        p1_path = p1_binexport.path if isinstance(p1_binexport, ProgramBinExport) else p1_binexport
+        p2_path = p2_binexport.path if isinstance(p2_binexport, ProgramBinExport) else p2_binexport
 
-        retcode = BinDiff.raw_diffing(p1_binexport, p2_binexport, diff_out)
-        return BinDiff(p1_binexport, p2_binexport, diff_out) if retcode else None
+        if not Path(diff_out).exists() or override:
+            retcode = BinDiff.raw_diffing(p1_path, p2_path, diff_out)
+            return BinDiff(p1_binexport, p2_binexport, diff_out) if retcode else None
+        else:
+            return BinDiff(p1_binexport, p2_binexport, diff_out)
 
     @staticmethod
     def _configure_bindiff_path() -> None:
         """
         Check BinDiff access paths
         """
         if not _check_environ():
```

### Comparing `python-bindiff-0.2.2/src/bindiff/file.py` & `python_bindiff-0.2.3/src/bindiff/file.py`

 * *Files identical despite different names*

### Comparing `python-bindiff-0.2.2/src/bindiff/types.py` & `python_bindiff-0.2.3/src/bindiff/types.py`

 * *Files identical despite different names*

### Comparing `python-bindiff-0.2.2/src/python_bindiff.egg-info/PKG-INFO` & `python_bindiff-0.2.3/src/python_bindiff.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bindiff
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python wrapper to manipulate bindiff files
 Author-email: Robin David <rdavid@quarkslab.com>
 License: Apache Software License (Apache License, Version 2)
 Project-URL: Homepage, https://github.com/quarkslab/python-bindiff
 Project-URL: Repository, https://github.com/quarkslab/python-bindiff
 Project-URL: Documentation, https://diffing.quarkslab.com/differs/bindiff.html#python-bindiff
 Project-URL: Bug Tracker, https://github.com/quarkslab/python-bindiff/issues
@@ -13,15 +13,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-magic; os_name != "nt"
 Requires-Dist: python-magic-bin; os_name == "nt"
 Requires-Dist: click
-Requires-Dist: python-binexport>=0.2.0
+Requires-Dist: python-binexport>=0.3.3
 
 # Python Bindiff
 
 ``python-bindiff`` is a python module aiming to give a friendly interface to launch
 and manipulate bindiff between two binary iles.
 
 How it works ?
```

