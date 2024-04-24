# Comparing `tmp/linkture-2.5.4.tar.gz` & `tmp/linkture-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkture-2.5.4.tar", last modified: Wed Apr 24 11:58:19 2024, max compression
+gzip compressed data, was "linkture-2.5.5.tar", last modified: Wed Apr 24 13:23:30 2024, max compression
```

## Comparing `linkture-2.5.4.tar` & `linkture-2.5.5.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1064 2024-04-24 11:58:06.254156 linkture-2.5.4/LICENSE
--rw-r--r--   0        0        0     9850 2024-04-24 11:58:06.254156 linkture-2.5.4/README.md
--rw-r--r--   0        0        0        0 2024-04-24 11:58:06.254156 linkture-2.5.4/__init__.py
--rwxr-xr-x   0        0        0    29080 2024-04-24 11:58:06.254156 linkture-2.5.4/linkture.py
--rw-r--r--   0        0        0     1292 2024-04-24 11:58:19.218121 linkture-2.5.4/pyproject.toml
--rw-r--r--   0        0        0     1491 2024-04-24 11:58:06.258156 linkture-2.5.4/setup.py
--rw-r--r--   0        0        0    11015 1970-01-01 00:00:00.000000 linkture-2.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-24 13:23:12.962485 linkture-2.5.5/LICENSE
+-rw-r--r--   0        0        0     9870 2024-04-24 13:23:12.962485 linkture-2.5.5/README.md
+-rw-r--r--   0        0        0     1345 2024-04-24 13:23:30.346438 linkture-2.5.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-24 13:23:12.962485 linkture-2.5.5/src/linkture/__init__.py
+-rwxr-xr-x   0        0        0    29093 2024-04-24 13:23:12.962485 linkture-2.5.5/src/linkture/__main__.py
+-rw-r--r--   0        0        0     1904 2024-04-24 13:23:12.962485 linkture-2.5.5/src/linkture/res/custom.json
+-rw-r--r--   0        0        0   581632 2024-04-24 13:23:12.966485 linkture-2.5.5/src/linkture/res/resources.db
+-rw-r--r--   0        0        0     1297 2024-04-24 13:23:12.966485 linkture-2.5.5/src/linkture/res/rss-36.png
+-rw-r--r--   0        0        0    11098 1970-01-01 00:00:00.000000 linkture-2.5.5/PKG-INFO
```

### Comparing `linkture-2.5.4/LICENSE` & `linkture-2.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `linkture-2.5.4/README.md` & `linkture-2.5.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 `python3 -m pip install linkture`
 
 ____
 ## Command-line usage
 
 ```
-> python3 linkture.py -h
+> python3 -m linkture -h
 usage: linkture.py [-h] [-v] [-q] [-f in-file | -r reference] [-o out-file]
                    [--language {Cebuano,Chinese,Danish,Dutch,English,French,German,Greek,Hungarian,Italian,Japanese,Korean,Norwegian,Polish,Portuguese,Russian,Spanish,Tagalog,Ukrainian}]
                    [--translate {Cebuano,Chinese,Danish,Dutch,English,French,German,Greek,Hungarian,Italian,Japanese,Korean,Norwegian,Polish,Portuguese,Russian,Spanish,Tagalog,Ukrainian}]
                    [-s separator] [-u] [--full | --official | --standard]
                    [-c | -d | -l [prefix [suffix ...]] | -t | -x]
                    [-sc BCV | -sv BCV | -cc chapter | -cv verse]
 
@@ -73,73 +73,69 @@
 auxiliary functions:
   -sc BCV               return the serial number (1-1189) of the chapter with code "BCV" ("bbcccvvv")
   -sv BCV               return the serial number (1-31091) of the verse with code "BCV" ("bbcccvvv")
   -cc chapter           return the BCV range for serial chapter number "chapter" (integer value)
   -cv verse             return the BCV code for serial verse number "verse" (integer value)
 ```
 
-Or, make it executable first and run directly:
-```
-$ chmod +x linkture.py
-```
-
 Some examples:
 ```
-$ ./linkture.py -r "Joh 17:17; 2Ti 3:16, 17" --full -u
+$ python3 -m linkture -r "Joh 17:17; 2Ti 3:16, 17" --full -u
 JOHN 17:17; 2 TIMOTHY 3:16, 17
 
-$ ./linkture.py -r "Joh 17:17; 2Ti 3:16, 17" --standard
+$ python3 -m linkture -r "Joh 17:17; 2Ti 3:16, 17" --standard
 John 17:17; 2 Tim. 3:16, 17
 
-$ ./linkture.py -r "Joh 17:17; 2Ti 3:16, 17" --official
+$ python3 -m linkture -r "Joh 17:17; 2Ti 3:16, 17" --official
 Joh 17:17; 2Ti 3:16, 17
 
-$ ./linkture.py -r "Joh 17:17; 2Ti 3:16, 17" -c
+$ python3 -m linkture -r "Joh 17:17; 2Ti 3:16, 17" -c
 [('43017017', '43017017'), ('55003016', '55003017')]
 
-$ ./linkture.py -r "[('43017017', '43017017'), ('55003016', '55003017')]" -d --translate German
+$ python3 -m linkture -r "[('43017017', '43017017'), ('55003016', '55003017')]" -d --translate German
 ['Johannes 17:17', '2. Timotheus 3:16, 17']
 
-$ ./linkture.py -r "Joh 17:17; 2Ti 3:16, 17" -l '<a href="https://my.website.com/' '/index.html" class="test">'
+$ python3 -m linkture -r "Joh 17:17; 2Ti 3:16, 17" -l '<a href="https://my.website.com/' '/index.html" class="test">'
 <a href="https://my.website.com/43:17:17/index.html" class="test">John 17:17</a>; <a href="https://my.website.com/55:3:16-55:3:17/index.html" class="test">2 Timothy 3:16, 17</a>
 
-$ ./linkture.py -r "Joh 17:17; 2Ti 3:16, 17" --translate Chinese
+$ python3 -m linkture -r "Joh 17:17; 2Ti 3:16, 17" --translate Chinese
 约翰福音 17:17; 提摩太后书 3:16, 17
 
-$ ./linkture.py -r "约翰福音 17:17; 提摩太后书 3:16, 17" --language Chinese --translate Dutch
+$ python3 -m linkture -r "约翰福音 17:17; 提摩太后书 3:16, 17" --language Chinese --translate Dutch
 Johannes 17:17; 2 Timotheüs 3:16, 17
 
-$ ./linkture.py -r "{{Jean 17:17}}; 2 Timothée 3:16, 17" --language French --translate Spanish --standard
+$ python3 -m linkture -r "{{Jean 17:17}}; 2 Timothée 3:16, 17" --language French --translate Spanish --standard
 Juan 17:17; 2 Tim. 3:16, 17
 
-$ ./linkture.py -r "Mat 17:17; Paul 3:16, 17" --full -x
+$ python3 -m linkture -r "Mat 17:17; Paul 3:16, 17" --full -x
 ['Matthew 17:17']
 
-$ ./linkture.py -cc 2
+$ python3 -m linkture -cc 2
 ('01002001', '01002025')
 
-$ ./linkture.py -cv 31091
+$ python3 -m linkture -cv 31091
 ('66022021', '66022021')
 
-$ ./linkture.py -sv '01001001'
+$ python3 -m linkture -sv '01001001'
 1
 
-./linkture.py -sc '66022001'
+python3 -m linkture -sc '66022001'
 1189
 
-./linkture.py -r '2Ti 3:16, 17' --full -s '_'
+python3 -m linkture -r '2Ti 3:16, 17' --full -s '_'
 2_Timothy_3:16,_17
 ```
 
 **Note**: The serial verse options (`-sv` and `-cv`) *do not* count Psalm headings as separate verses.
 
 Of course, you can pass a whole text file to parse and process using the `-f in_file` flag, instead of `-r "references"`. And you can output to another text file (instead of the terminal) using `-o out_file`.
 
 Unless you use `-q`, you will see in the terminal any out-of-range errors encountered while parsing. Of course, these entries will not be processed, but they will not affect the rest of the operation.
 
+____
 ## Script/import usage
 
 Assume the text (short string or long document) you want to process is in the variable `txt`. It's in English, but you would like the scriptures to be in Spanish, with the full book name:
 ```
 from linkture import Scriptures
 
 s = Scriptures(language="English", translate="Spanish", form="full")
@@ -185,8 +181,8 @@
 * *verbose* - if **True**, show (in terminal) any out-of-range errors encountered while parsing (**False** by default)
 
 ____
 ## Feedback
 
 Feel free to [get in touch and post any issues and suggestions](https://github.com/erykjj/linkture/issues).
 
-[![RSS of releases](res/rss-36.png)](https://github.com/erykjj/linkture/releases.atom)
+[![RSS of releases](src/res/rss-36.png)](https://github.com/erykjj/linkture/releases.atom)
```

### Comparing `linkture-2.5.4/linkture.py` & `linkture-2.5.5/src/linkture/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
   AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
   LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
   OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
   SOFTWARE.
 """
 
-VERSION = 'v2.5.4'
+VERSION = 'v2.5.5'
 
 
 import argparse, json, regex, sqlite3
 import pandas as pd
 
 from ast import literal_eval
 from pathlib import Path
@@ -669,15 +669,15 @@
         with open(args['o'], 'w', encoding='UTF-8') as f:
             f.write(str(txt))
     else:
         print(txt)
 
 if __name__ == "__main__":
     PROJECT_PATH = Path(__file__).resolve().parent
-    APP = Path(__file__).stem
+    APP = 'linkture' # Path(__file__).stem
     parser = argparse.ArgumentParser(description="PARSE and PROCESS BIBLE SCRIPTURE REFERENCES: extract, tag, link, rewrite, translate, BCV-encode and decode. See README for more information")
 
     parser.add_argument('-v', action='version', version=f"{APP} {VERSION}", help='show version and exit')
     parser.add_argument('-q', action='store_true', help="don't show errors")
 
     function_group = parser.add_argument_group('data source (one required - except for auxiliary functions, which only take command-line arguments)', 'choose between terminal or file input:')
     mode = function_group.add_mutually_exclusive_group()
```

### Comparing `linkture-2.5.4/pyproject.toml` & `linkture-2.5.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "linkture"
-version = "2.5.4"
+version = "2.5.5"
 description = "PARSE and PROCESS BIBLE SCRIPTURE REFERENCES: extract, tag, link, rewrite, translate, BCV-encode and decode"
 authors = [
     { name = "Eryk J.", email = "infiniti@inventati.org" },
 ]
 dependencies = [
     "setuptools>=59.6.0",
     "argparse>=1.4.0",
@@ -38,14 +38,15 @@
 ]
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/erykjj/linkture"
+Issues = "https://github.com/erykjj/linkture/issues"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `linkture-2.5.4/PKG-INFO` & `linkture-2.5.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkture
-Version: 2.5.4
+Version: 2.5.5
 Summary: PARSE and PROCESS BIBLE SCRIPTURE REFERENCES: extract, tag, link, rewrite, translate, BCV-encode and decode
 Keywords: bible,scriptures,scripture-references,scripture-translation,scripture-parser,scripture-linker
 Author-Email: "Eryk J." <infiniti@inventati.org>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Topic :: Religion
 Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Text Processing :: Linguistic
 Project-URL: Homepage, https://github.com/erykjj/linkture
+Project-URL: Issues, https://github.com/erykjj/linkture/issues
 Requires-Python: >=3.9
 Requires-Dist: setuptools>=59.6.0
 Requires-Dist: argparse>=1.4.0
 Requires-Dist: regex>=2023.8.8
 Requires-Dist: unidecode>=1.3.8
 Requires-Dist: pathlib>=1.0.1
 Requires-Dist: pandas==2.2.2
@@ -48,15 +49,15 @@
 
 `python3 -m pip install linkture`
 
 ____
 ## Command-line usage
 
 ```
-> python3 linkture.py -h
+> python3 -m linkture -h
 usage: linkture.py [-h] [-v] [-q] [-f in-file | -r reference] [-o out-file]
                    [--language {Cebuano,Chinese,Danish,Dutch,English,French,German,Greek,Hungarian,Italian,Japanese,Korean,Norwegian,Polish,Portuguese,Russian,Spanish,Tagalog,Ukrainian}]
                    [--translate {Cebuano,Chinese,Danish,Dutch,English,French,German,Greek,Hungarian,Italian,Japanese,Korean,Norwegian,Polish,Portuguese,Russian,Spanish,Tagalog,Ukrainian}]
                    [-s separator] [-u] [--full | --official | --standard]
                    [-c | -d | -l [prefix [suffix ...]] | -t | -x]
                    [-sc BCV | -sv BCV | -cc chapter | -cv verse]
 
@@ -101,73 +102,69 @@
 auxiliary functions:
   -sc BCV               return the serial number (1-1189) of the chapter with code "BCV" ("bbcccvvv")
   -sv BCV               return the serial number (1-31091) of the verse with code "BCV" ("bbcccvvv")
   -cc chapter           return the BCV range for serial chapter number "chapter" (integer value)
   -cv verse             return the BCV code for serial verse number "verse" (integer value)
 ```
 
-Or, make it executable first and run directly:
-```
-$ chmod +x linkture.py
-```
-
 Some examples:
 ```
-$ ./linkture.py -r "Joh 17:17; 2Ti 3:16, 17" --full -u
+$ python3 -m linkture -r "Joh 17:17; 2Ti 3:16, 17" --full -u
 JOHN 17:17; 2 TIMOTHY 3:16, 17
 
-$ ./linkture.py -r "Joh 17:17; 2Ti 3:16, 17" --standard
+$ python3 -m linkture -r "Joh 17:17; 2Ti 3:16, 17" --standard
 John 17:17; 2 Tim. 3:16, 17
 
-$ ./linkture.py -r "Joh 17:17; 2Ti 3:16, 17" --official
+$ python3 -m linkture -r "Joh 17:17; 2Ti 3:16, 17" --official
 Joh 17:17; 2Ti 3:16, 17
 
-$ ./linkture.py -r "Joh 17:17; 2Ti 3:16, 17" -c
+$ python3 -m linkture -r "Joh 17:17; 2Ti 3:16, 17" -c
 [('43017017', '43017017'), ('55003016', '55003017')]
 
-$ ./linkture.py -r "[('43017017', '43017017'), ('55003016', '55003017')]" -d --translate German
+$ python3 -m linkture -r "[('43017017', '43017017'), ('55003016', '55003017')]" -d --translate German
 ['Johannes 17:17', '2. Timotheus 3:16, 17']
 
-$ ./linkture.py -r "Joh 17:17; 2Ti 3:16, 17" -l '<a href="https://my.website.com/' '/index.html" class="test">'
+$ python3 -m linkture -r "Joh 17:17; 2Ti 3:16, 17" -l '<a href="https://my.website.com/' '/index.html" class="test">'
 <a href="https://my.website.com/43:17:17/index.html" class="test">John 17:17</a>; <a href="https://my.website.com/55:3:16-55:3:17/index.html" class="test">2 Timothy 3:16, 17</a>
 
-$ ./linkture.py -r "Joh 17:17; 2Ti 3:16, 17" --translate Chinese
+$ python3 -m linkture -r "Joh 17:17; 2Ti 3:16, 17" --translate Chinese
 约翰福音 17:17; 提摩太后书 3:16, 17
 
-$ ./linkture.py -r "约翰福音 17:17; 提摩太后书 3:16, 17" --language Chinese --translate Dutch
+$ python3 -m linkture -r "约翰福音 17:17; 提摩太后书 3:16, 17" --language Chinese --translate Dutch
 Johannes 17:17; 2 Timotheüs 3:16, 17
 
-$ ./linkture.py -r "{{Jean 17:17}}; 2 Timothée 3:16, 17" --language French --translate Spanish --standard
+$ python3 -m linkture -r "{{Jean 17:17}}; 2 Timothée 3:16, 17" --language French --translate Spanish --standard
 Juan 17:17; 2 Tim. 3:16, 17
 
-$ ./linkture.py -r "Mat 17:17; Paul 3:16, 17" --full -x
+$ python3 -m linkture -r "Mat 17:17; Paul 3:16, 17" --full -x
 ['Matthew 17:17']
 
-$ ./linkture.py -cc 2
+$ python3 -m linkture -cc 2
 ('01002001', '01002025')
 
-$ ./linkture.py -cv 31091
+$ python3 -m linkture -cv 31091
 ('66022021', '66022021')
 
-$ ./linkture.py -sv '01001001'
+$ python3 -m linkture -sv '01001001'
 1
 
-./linkture.py -sc '66022001'
+python3 -m linkture -sc '66022001'
 1189
 
-./linkture.py -r '2Ti 3:16, 17' --full -s '_'
+python3 -m linkture -r '2Ti 3:16, 17' --full -s '_'
 2_Timothy_3:16,_17
 ```
 
 **Note**: The serial verse options (`-sv` and `-cv`) *do not* count Psalm headings as separate verses.
 
 Of course, you can pass a whole text file to parse and process using the `-f in_file` flag, instead of `-r "references"`. And you can output to another text file (instead of the terminal) using `-o out_file`.
 
 Unless you use `-q`, you will see in the terminal any out-of-range errors encountered while parsing. Of course, these entries will not be processed, but they will not affect the rest of the operation.
 
+____
 ## Script/import usage
 
 Assume the text (short string or long document) you want to process is in the variable `txt`. It's in English, but you would like the scriptures to be in Spanish, with the full book name:
 ```
 from linkture import Scriptures
 
 s = Scriptures(language="English", translate="Spanish", form="full")
@@ -213,8 +210,8 @@
 * *verbose* - if **True**, show (in terminal) any out-of-range errors encountered while parsing (**False** by default)
 
 ____
 ## Feedback
 
 Feel free to [get in touch and post any issues and suggestions](https://github.com/erykjj/linkture/issues).
 
-[![RSS of releases](res/rss-36.png)](https://github.com/erykjj/linkture/releases.atom)
+[![RSS of releases](src/res/rss-36.png)](https://github.com/erykjj/linkture/releases.atom)
```

