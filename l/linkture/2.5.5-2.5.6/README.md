# Comparing `tmp/linkture-2.5.5.tar.gz` & `tmp/linkture-2.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkture-2.5.5.tar", last modified: Wed Apr 24 13:23:30 2024, max compression
+gzip compressed data, was "linkture-2.5.6.tar", last modified: Wed Apr 24 13:53:18 2024, max compression
```

## Comparing `linkture-2.5.5.tar` & `linkture-2.5.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1064 2024-04-24 13:23:12.962485 linkture-2.5.5/LICENSE
--rw-r--r--   0        0        0     9870 2024-04-24 13:23:12.962485 linkture-2.5.5/README.md
--rw-r--r--   0        0        0     1345 2024-04-24 13:23:30.346438 linkture-2.5.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-24 13:23:12.962485 linkture-2.5.5/src/linkture/__init__.py
--rwxr-xr-x   0        0        0    29093 2024-04-24 13:23:12.962485 linkture-2.5.5/src/linkture/__main__.py
--rw-r--r--   0        0        0     1904 2024-04-24 13:23:12.962485 linkture-2.5.5/src/linkture/res/custom.json
--rw-r--r--   0        0        0   581632 2024-04-24 13:23:12.966485 linkture-2.5.5/src/linkture/res/resources.db
--rw-r--r--   0        0        0     1297 2024-04-24 13:23:12.966485 linkture-2.5.5/src/linkture/res/rss-36.png
--rw-r--r--   0        0        0    11098 1970-01-01 00:00:00.000000 linkture-2.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-24 13:53:05.188418 linkture-2.5.6/LICENSE
+-rw-r--r--   0        0        0     9870 2024-04-24 13:53:05.188418 linkture-2.5.6/README.md
+-rw-r--r--   0        0        0     1429 2024-04-24 13:53:18.036353 linkture-2.5.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-24 13:53:05.188418 linkture-2.5.6/src/linkture/__init__.py
+-rwxr-xr-x   0        0        0    29101 2024-04-24 13:53:05.188418 linkture-2.5.6/src/linkture/__main__.py
+-rw-r--r--   0        0        0     1904 2024-04-24 13:53:05.188418 linkture-2.5.6/src/linkture/res/custom.json
+-rw-r--r--   0        0        0   581632 2024-04-24 13:53:05.188418 linkture-2.5.6/src/linkture/res/resources.db
+-rw-r--r--   0        0        0     1297 2024-04-24 13:53:05.192417 linkture-2.5.6/src/linkture/res/rss-36.png
+-rw-r--r--   0        0        0    11098 1970-01-01 00:00:00.000000 linkture-2.5.6/PKG-INFO
```

### Comparing `linkture-2.5.5/LICENSE` & `linkture-2.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `linkture-2.5.5/README.md` & `linkture-2.5.6/README.md`

 * *Files identical despite different names*

### Comparing `linkture-2.5.5/pyproject.toml` & `linkture-2.5.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "linkture"
-version = "2.5.5"
+dynamic = []
 description = "PARSE and PROCESS BIBLE SCRIPTURE REFERENCES: extract, tag, link, rewrite, translate, BCV-encode and decode"
 authors = [
     { name = "Eryk J.", email = "infiniti@inventati.org" },
 ]
 dependencies = [
     "setuptools>=59.6.0",
     "argparse>=1.4.0",
@@ -32,14 +32,15 @@
     "bible",
     "scriptures",
     "scripture-references",
     "scripture-translation",
     "scripture-parser",
     "scripture-linker",
 ]
+version = "v2.5.6"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/erykjj/linkture"
 Issues = "https://github.com/erykjj/linkture/issues"
@@ -48,7 +49,11 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm]
 distribution = true
+
+[tool.pdm.version]
+source = "file"
+path = "src/linkture/__main__.py"
```

### Comparing `linkture-2.5.5/src/linkture/__main__.py` & `linkture-2.5.6/src/linkture/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
   AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
   LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
   OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
   SOFTWARE.
 """
 
-VERSION = 'v2.5.5'
+__version__ = 'v2.5.6'
 
 
 import argparse, json, regex, sqlite3
 import pandas as pd
 
 from ast import literal_eval
 from pathlib import Path
@@ -672,15 +672,15 @@
         print(txt)
 
 if __name__ == "__main__":
     PROJECT_PATH = Path(__file__).resolve().parent
     APP = 'linkture' # Path(__file__).stem
     parser = argparse.ArgumentParser(description="PARSE and PROCESS BIBLE SCRIPTURE REFERENCES: extract, tag, link, rewrite, translate, BCV-encode and decode. See README for more information")
 
-    parser.add_argument('-v', action='version', version=f"{APP} {VERSION}", help='show version and exit')
+    parser.add_argument('-v', action='version', version=f"{APP} {__version__}", help='show version and exit')
     parser.add_argument('-q', action='store_true', help="don't show errors")
 
     function_group = parser.add_argument_group('data source (one required - except for auxiliary functions, which only take command-line arguments)', 'choose between terminal or file input:')
     mode = function_group.add_mutually_exclusive_group()
     mode.add_argument('-f', metavar='in-file', help='get input from file (UTF-8)')
     mode.add_argument('-r', metavar='reference', help='process "reference; reference; etc."')
     parser.add_argument('-o', metavar='out-file', help='output file (terminal output if not provided)')
```

### Comparing `linkture-2.5.5/src/linkture/res/custom.json` & `linkture-2.5.6/src/linkture/res/custom.json`

 * *Files identical despite different names*

### Comparing `linkture-2.5.5/src/linkture/res/resources.db` & `linkture-2.5.6/src/linkture/res/resources.db`

 * *Files identical despite different names*

### Comparing `linkture-2.5.5/src/linkture/res/rss-36.png` & `linkture-2.5.6/src/linkture/res/rss-36.png`

 * *Files identical despite different names*

### Comparing `linkture-2.5.5/PKG-INFO` & `linkture-2.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkture
-Version: 2.5.5
+Version: 2.5.6
 Summary: PARSE and PROCESS BIBLE SCRIPTURE REFERENCES: extract, tag, link, rewrite, translate, BCV-encode and decode
 Keywords: bible,scriptures,scripture-references,scripture-translation,scripture-parser,scripture-linker
 Author-Email: "Eryk J." <infiniti@inventati.org>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
```

