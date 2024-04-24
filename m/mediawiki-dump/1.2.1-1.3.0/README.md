# Comparing `tmp/mediawiki_dump-1.2.1.tar.gz` & `tmp/mediawiki_dump-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediawiki_dump-1.2.1.tar", last modified: Wed Apr 17 09:22:02 2024, max compression
+gzip compressed data, was "mediawiki_dump-1.3.0.tar", last modified: Wed Apr 24 12:11:38 2024, max compression
```

## Comparing `mediawiki_dump-1.2.1.tar` & `mediawiki_dump-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:02.112660 mediawiki_dump-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-17 09:21:54.000000 mediawiki_dump-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 09:21:54.000000 mediawiki_dump-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8693 2024-04-17 09:22:02.112660 mediawiki_dump-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-04-17 09:21:54.000000 mediawiki_dump-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:02.108660 mediawiki_dump-1.2.1/mediawiki_dump/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:21:54.000000 mediawiki_dump-1.2.1/mediawiki_dump/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-04-17 09:21:54.000000 mediawiki_dump-1.2.1/mediawiki_dump/dumps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 09:21:54.000000 mediawiki_dump-1.2.1/mediawiki_dump/entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-04-17 09:21:54.000000 mediawiki_dump-1.2.1/mediawiki_dump/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-17 09:21:54.000000 mediawiki_dump-1.2.1/mediawiki_dump/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-17 09:21:54.000000 mediawiki_dump-1.2.1/mediawiki_dump/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:02.112660 mediawiki_dump-1.2.1/mediawiki_dump.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8693 2024-04-17 09:22:02.000000 mediawiki_dump-1.2.1/mediawiki_dump.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-17 09:22:02.000000 mediawiki_dump-1.2.1/mediawiki_dump.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:22:02.000000 mediawiki_dump-1.2.1/mediawiki_dump.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-17 09:22:02.000000 mediawiki_dump-1.2.1/mediawiki_dump.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-17 09:22:02.000000 mediawiki_dump-1.2.1/mediawiki_dump.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 09:22:02.112660 mediawiki_dump-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-17 09:21:54.000000 mediawiki_dump-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:11:38.850647 mediawiki_dump-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-24 12:11:22.000000 mediawiki_dump-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 12:11:22.000000 mediawiki_dump-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9546 2024-04-24 12:11:38.850647 mediawiki_dump-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8547 2024-04-24 12:11:22.000000 mediawiki_dump-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:11:38.850647 mediawiki_dump-1.3.0/mediawiki_dump/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:11:22.000000 mediawiki_dump-1.3.0/mediawiki_dump/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-04-24 12:11:22.000000 mediawiki_dump-1.3.0/mediawiki_dump/dumps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-24 12:11:22.000000 mediawiki_dump-1.3.0/mediawiki_dump/entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-04-24 12:11:22.000000 mediawiki_dump-1.3.0/mediawiki_dump/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-24 12:11:22.000000 mediawiki_dump-1.3.0/mediawiki_dump/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-24 12:11:22.000000 mediawiki_dump-1.3.0/mediawiki_dump/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:11:38.850647 mediawiki_dump-1.3.0/mediawiki_dump.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9546 2024-04-24 12:11:38.000000 mediawiki_dump-1.3.0/mediawiki_dump.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-24 12:11:38.000000 mediawiki_dump-1.3.0/mediawiki_dump.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 12:11:38.000000 mediawiki_dump-1.3.0/mediawiki_dump.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-24 12:11:38.000000 mediawiki_dump-1.3.0/mediawiki_dump.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-24 12:11:38.000000 mediawiki_dump-1.3.0/mediawiki_dump.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 12:11:38.850647 mediawiki_dump-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-24 12:11:22.000000 mediawiki_dump-1.3.0/setup.py
```

### Comparing `mediawiki_dump-1.2.1/LICENSE` & `mediawiki_dump-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mediawiki_dump-1.2.1/PKG-INFO` & `mediawiki_dump-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mediawiki_dump
-Version: 1.2.1
+Version: 1.3.0
 Summary: Python package for working with MediaWiki XML content dumps
 Home-page: https://github.com/macbre/mediawiki-dump
 Author: Maciej Brencz
 Author-email: maciej.brencz@gmail.com
 License: MIT
-Keywords: dump fandom mediawiki wikipedia wikia
+Keywords: dump fandom mediawiki wikipedia wikia xml
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -233,7 +233,43 @@
 
 with open("pages.txt", mode="wt", encoding="utf-8") as fp:
     for entry in with_places_tag:
         fp.write(entry + "\n")
 
 logging.info("pages.txt file created")
 ```
+
+## Reading dumps from local files
+
+You can also read dumps from local, non-compressed XML files:
+
+```python
+from mediawiki_dump.dumps import LocalFileDump
+from mediawiki_dump.reader import DumpReader
+
+dump = LocalFileDump(dump_file="test/fixtures/dump.xml")
+reader = DumpReader()
+
+pages = [entry.title for entry in reader.read(dump)]
+print(dump, pages)
+```
+
+## Reading dumps from compressed local files
+
+Or any other iterators (like HTTP responses):
+
+```python
+import bz2
+
+from mediawiki_dump.dumps import IteratorDump
+from mediawiki_dump.reader import DumpReader
+
+def get_content(file_name: str):
+    with bz2.open(file_name, mode="r") as fp:
+        yield from fp
+
+dump = IteratorDump(iterator=get_content(file_name="test/fixtures/dump.xml.bz2"))
+reader = DumpReader()
+
+pages = [entry.title for entry in reader.read(dump)]
+print(dump, pages)
+```
```

### Comparing `mediawiki_dump-1.2.1/README.md` & `mediawiki_dump-1.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -206,7 +206,43 @@
 
 with open("pages.txt", mode="wt", encoding="utf-8") as fp:
     for entry in with_places_tag:
         fp.write(entry + "\n")
 
 logging.info("pages.txt file created")
 ```
+
+## Reading dumps from local files
+
+You can also read dumps from local, non-compressed XML files:
+
+```python
+from mediawiki_dump.dumps import LocalFileDump
+from mediawiki_dump.reader import DumpReader
+
+dump = LocalFileDump(dump_file="test/fixtures/dump.xml")
+reader = DumpReader()
+
+pages = [entry.title for entry in reader.read(dump)]
+print(dump, pages)
+```
+
+## Reading dumps from compressed local files
+
+Or any other iterators (like HTTP responses):
+
+```python
+import bz2
+
+from mediawiki_dump.dumps import IteratorDump
+from mediawiki_dump.reader import DumpReader
+
+def get_content(file_name: str):
+    with bz2.open(file_name, mode="r") as fp:
+        yield from fp
+
+dump = IteratorDump(iterator=get_content(file_name="test/fixtures/dump.xml.bz2"))
+reader = DumpReader()
+
+pages = [entry.title for entry in reader.read(dump)]
+print(dump, pages)
+```
```

### Comparing `mediawiki_dump-1.2.1/mediawiki_dump/dumps.py` & `mediawiki_dump-1.3.0/mediawiki_dump/dumps.py`

 * *Files 8% similar despite different names*

```diff
@@ -174,30 +174,47 @@
 
         with self.fetch() as handler:
             with libarchive.file_reader(handler.name) as archive:
                 for entry in archive:
                     yield from entry.get_blocks()
 
 
-class LocalFileDump(BaseDump):
+class IteratorDump(BaseDump):
+    """
+    This class can be used to pass the XML dump via an iterator,
+    for instance when streaming and decompressing a local file.
+    """
+
+    def __init__(self, iterator: iter):
+        super().__init__(wiki="")
+        self.iterator = iterator
+
+    def get_url(self):
+        pass
+
+    def get_content(self):
+        yield from self.iterator
+
+
+class LocalFileDump(IteratorDump):
     """
     This class can be used to load locally stored XML dump file
     """
 
     def __init__(self, dump_file: str):
         super().__init__("")
         self.dump_file = dump_file
 
     def get_url(self):
         pass
 
     def get_content(self):
-        """Yields processed pieces of content"""
-        # pylint:disable=consider-using-with
-        return open(self.dump_file, mode="rt", encoding="utf-8")
+        with open(self.dump_file, mode="rb") as fp:
+            self.iterator = fp
+            yield from super().get_content()
 
 
 class StringDump(BaseDump):
     """
     This class can be used to load XML from a variable
     """
```

### Comparing `mediawiki_dump-1.2.1/mediawiki_dump/entry.py` & `mediawiki_dump-1.3.0/mediawiki_dump/entry.py`

 * *Files identical despite different names*

### Comparing `mediawiki_dump-1.2.1/mediawiki_dump/reader.py` & `mediawiki_dump-1.3.0/mediawiki_dump/reader.py`

 * *Files identical despite different names*

### Comparing `mediawiki_dump-1.2.1/mediawiki_dump/tokenizer.py` & `mediawiki_dump-1.3.0/mediawiki_dump/tokenizer.py`

 * *Files identical despite different names*

### Comparing `mediawiki_dump-1.2.1/mediawiki_dump.egg-info/PKG-INFO` & `mediawiki_dump-1.3.0/mediawiki_dump.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mediawiki_dump
-Version: 1.2.1
+Version: 1.3.0
 Summary: Python package for working with MediaWiki XML content dumps
 Home-page: https://github.com/macbre/mediawiki-dump
 Author: Maciej Brencz
 Author-email: maciej.brencz@gmail.com
 License: MIT
-Keywords: dump fandom mediawiki wikipedia wikia
+Keywords: dump fandom mediawiki wikipedia wikia xml
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -233,7 +233,43 @@
 
 with open("pages.txt", mode="wt", encoding="utf-8") as fp:
     for entry in with_places_tag:
         fp.write(entry + "\n")
 
 logging.info("pages.txt file created")
 ```
+
+## Reading dumps from local files
+
+You can also read dumps from local, non-compressed XML files:
+
+```python
+from mediawiki_dump.dumps import LocalFileDump
+from mediawiki_dump.reader import DumpReader
+
+dump = LocalFileDump(dump_file="test/fixtures/dump.xml")
+reader = DumpReader()
+
+pages = [entry.title for entry in reader.read(dump)]
+print(dump, pages)
+```
+
+## Reading dumps from compressed local files
+
+Or any other iterators (like HTTP responses):
+
+```python
+import bz2
+
+from mediawiki_dump.dumps import IteratorDump
+from mediawiki_dump.reader import DumpReader
+
+def get_content(file_name: str):
+    with bz2.open(file_name, mode="r") as fp:
+        yield from fp
+
+dump = IteratorDump(iterator=get_content(file_name="test/fixtures/dump.xml.bz2"))
+reader = DumpReader()
+
+pages = [entry.title for entry in reader.read(dump)]
+print(dump, pages)
+```
```

### Comparing `mediawiki_dump-1.2.1/setup.py` & `mediawiki_dump-1.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "1.2.1"
+VERSION = "1.3.0"
 
 # @see https://packaging.python.org/tutorials/packaging-projects/#creating-setup-py
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # @see https://github.com/pypa/sampleproject/blob/master/setup.py
 setup(
@@ -12,15 +12,15 @@
     version=VERSION,
     author="Maciej Brencz",
     author_email="maciej.brencz@gmail.com",
     license="MIT",
     description="Python package for working with MediaWiki XML content dumps",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    keywords="dump fandom mediawiki wikipedia wikia",
+    keywords="dump fandom mediawiki wikipedia wikia xml",
     url="https://github.com/macbre/mediawiki-dump",
     # https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
```

