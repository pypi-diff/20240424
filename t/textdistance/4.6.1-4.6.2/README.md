# Comparing `tmp/textdistance-4.6.1.tar.gz` & `tmp/textdistance-4.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textdistance-4.6.1.tar", last modified: Fri Dec 29 09:26:29 2023, max compression
+gzip compressed data, was "textdistance-4.6.2.tar", last modified: Wed Apr 24 11:35:42 2024, max compression
```

## Comparing `textdistance-4.6.1.tar` & `textdistance-4.6.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 gram      (1000) gram      (1000)        0 2023-12-29 09:26:29.240310 textdistance-4.6.1/
--rw-rw-r--   0 gram      (1000) gram      (1000)     1049 2022-09-06 10:08:11.000000 textdistance-4.6.1/LICENSE
--rw-rw-r--   0 gram      (1000) gram      (1000)       35 2022-09-06 10:08:11.000000 textdistance-4.6.1/MANIFEST.in
--rw-r--r--   0 gram      (1000) gram      (1000)    18148 2023-12-29 09:26:29.240310 textdistance-4.6.1/PKG-INFO
--rw-rw-r--   0 gram      (1000) gram      (1000)    13581 2023-09-28 08:28:37.000000 textdistance-4.6.1/README.md
--rw-rw-r--   0 gram      (1000) gram      (1000)      195 2023-09-27 06:42:27.000000 textdistance-4.6.1/pyproject.toml
--rw-rw-r--   0 gram      (1000) gram      (1000)      641 2023-12-29 09:26:29.240310 textdistance-4.6.1/setup.cfg
--rw-rw-r--   0 gram      (1000) gram      (1000)     3798 2023-12-29 09:25:55.000000 textdistance-4.6.1/setup.py
-drwxrwxr-x   0 gram      (1000) gram      (1000)        0 2023-12-29 09:26:29.232310 textdistance-4.6.1/tests/
--rw-rw-r--   0 gram      (1000) gram      (1000)     2679 2022-09-06 10:08:11.000000 textdistance-4.6.1/tests/test_common.py
--rw-rw-r--   0 gram      (1000) gram      (1000)     3791 2023-09-28 07:20:22.000000 textdistance-4.6.1/tests/test_external.py
-drwxrwxr-x   0 gram      (1000) gram      (1000)        0 2023-12-29 09:26:29.236310 textdistance-4.6.1/textdistance/
--rw-rw-r--   0 gram      (1000) gram      (1000)      355 2023-12-29 09:25:52.000000 textdistance-4.6.1/textdistance/__init__.py
-drwxrwxr-x   0 gram      (1000) gram      (1000)        0 2023-12-29 09:26:29.236310 textdistance-4.6.1/textdistance/algorithms/
--rw-rw-r--   0 gram      (1000) gram      (1000)      217 2022-09-06 11:25:30.000000 textdistance-4.6.1/textdistance/algorithms/__init__.py
--rw-rw-r--   0 gram      (1000) gram      (1000)     6332 2023-09-28 08:28:37.000000 textdistance-4.6.1/textdistance/algorithms/base.py
--rw-rw-r--   0 gram      (1000) gram      (1000)     8190 2023-09-28 08:28:37.000000 textdistance-4.6.1/textdistance/algorithms/compression_based.py
--rw-rw-r--   0 gram      (1000) gram      (1000)    27593 2023-09-27 11:33:22.000000 textdistance-4.6.1/textdistance/algorithms/edit_based.py
--rw-rw-r--   0 gram      (1000) gram      (1000)     6133 2023-09-27 11:33:22.000000 textdistance-4.6.1/textdistance/algorithms/phonetic.py
--rw-rw-r--   0 gram      (1000) gram      (1000)     6158 2023-09-27 11:33:22.000000 textdistance-4.6.1/textdistance/algorithms/sequence_based.py
--rw-rw-r--   0 gram      (1000) gram      (1000)     3209 2023-09-27 11:33:22.000000 textdistance-4.6.1/textdistance/algorithms/simple.py
--rw-rw-r--   0 gram      (1000) gram      (1000)     9405 2023-09-28 08:28:37.000000 textdistance-4.6.1/textdistance/algorithms/token_based.py
--rw-rw-r--   0 gram      (1000) gram      (1000)      166 2023-09-27 11:33:22.000000 textdistance-4.6.1/textdistance/algorithms/types.py
--rw-rw-r--   0 gram      (1000) gram      (1000)     2821 2023-09-27 11:33:22.000000 textdistance-4.6.1/textdistance/algorithms/vector_based.py
--rw-rw-r--   0 gram      (1000) gram      (1000)     3818 2023-09-27 11:33:22.000000 textdistance-4.6.1/textdistance/benchmark.py
--rw-rw-r--   0 gram      (1000) gram      (1000)     1161 2023-12-29 09:20:18.000000 textdistance-4.6.1/textdistance/libraries.json
--rw-rw-r--   0 gram      (1000) gram      (1000)     6716 2023-09-28 07:20:22.000000 textdistance-4.6.1/textdistance/libraries.py
--rw-rw-r--   0 gram      (1000) gram      (1000)        0 2022-09-09 12:27:03.000000 textdistance-4.6.1/textdistance/py.typed
--rw-rw-r--   0 gram      (1000) gram      (1000)      783 2023-09-27 11:33:22.000000 textdistance-4.6.1/textdistance/utils.py
-drwxrwxr-x   0 gram      (1000) gram      (1000)        0 2023-12-29 09:26:29.236310 textdistance-4.6.1/textdistance.egg-info/
--rw-r--r--   0 gram      (1000) gram      (1000)    18148 2023-12-29 09:26:29.000000 textdistance-4.6.1/textdistance.egg-info/PKG-INFO
--rw-rw-r--   0 gram      (1000) gram      (1000)      810 2023-12-29 09:26:29.000000 textdistance-4.6.1/textdistance.egg-info/SOURCES.txt
--rw-rw-r--   0 gram      (1000) gram      (1000)        1 2023-12-29 09:26:29.000000 textdistance-4.6.1/textdistance.egg-info/dependency_links.txt
--rw-rw-r--   0 gram      (1000) gram      (1000)     1097 2023-12-29 09:26:29.000000 textdistance-4.6.1/textdistance.egg-info/requires.txt
--rw-rw-r--   0 gram      (1000) gram      (1000)       13 2023-12-29 09:26:29.000000 textdistance-4.6.1/textdistance.egg-info/top_level.txt
+drwxrwxr-x   0 gram      (1000) gram      (1000)        0 2024-04-24 11:35:42.832659 textdistance-4.6.2/
+-rw-rw-r--   0 gram      (1000) gram      (1000)     1049 2022-09-06 10:08:11.000000 textdistance-4.6.2/LICENSE
+-rw-rw-r--   0 gram      (1000) gram      (1000)       35 2022-09-06 10:08:11.000000 textdistance-4.6.2/MANIFEST.in
+-rw-rw-r--   0 gram      (1000) gram      (1000)    14636 2024-04-24 11:35:42.832659 textdistance-4.6.2/PKG-INFO
+-rw-rw-r--   0 gram      (1000) gram      (1000)    13581 2023-09-28 08:28:37.000000 textdistance-4.6.2/README.md
+-rw-rw-r--   0 gram      (1000) gram      (1000)      195 2023-09-27 06:42:27.000000 textdistance-4.6.2/pyproject.toml
+-rw-rw-r--   0 gram      (1000) gram      (1000)      641 2024-04-24 11:35:42.832659 textdistance-4.6.2/setup.cfg
+-rw-rw-r--   0 gram      (1000) gram      (1000)     3798 2024-04-24 11:34:59.000000 textdistance-4.6.2/setup.py
+drwxrwxr-x   0 gram      (1000) gram      (1000)        0 2024-04-24 11:35:42.828659 textdistance-4.6.2/tests/
+-rw-rw-r--   0 gram      (1000) gram      (1000)     2679 2022-09-06 10:08:11.000000 textdistance-4.6.2/tests/test_common.py
+-rw-rw-r--   0 gram      (1000) gram      (1000)     3791 2023-09-28 07:20:22.000000 textdistance-4.6.2/tests/test_external.py
+drwxrwxr-x   0 gram      (1000) gram      (1000)        0 2024-04-24 11:35:42.832659 textdistance-4.6.2/textdistance/
+-rw-rw-r--   0 gram      (1000) gram      (1000)      355 2024-04-24 11:34:56.000000 textdistance-4.6.2/textdistance/__init__.py
+drwxrwxr-x   0 gram      (1000) gram      (1000)        0 2024-04-24 11:35:42.832659 textdistance-4.6.2/textdistance/algorithms/
+-rw-rw-r--   0 gram      (1000) gram      (1000)      217 2022-09-06 11:25:30.000000 textdistance-4.6.2/textdistance/algorithms/__init__.py
+-rw-rw-r--   0 gram      (1000) gram      (1000)     6332 2023-09-28 08:28:37.000000 textdistance-4.6.2/textdistance/algorithms/base.py
+-rw-rw-r--   0 gram      (1000) gram      (1000)     8190 2023-09-28 08:28:37.000000 textdistance-4.6.2/textdistance/algorithms/compression_based.py
+-rw-rw-r--   0 gram      (1000) gram      (1000)    27598 2024-04-24 11:34:44.000000 textdistance-4.6.2/textdistance/algorithms/edit_based.py
+-rw-rw-r--   0 gram      (1000) gram      (1000)     6133 2023-09-27 11:33:22.000000 textdistance-4.6.2/textdistance/algorithms/phonetic.py
+-rw-rw-r--   0 gram      (1000) gram      (1000)     6158 2023-09-27 11:33:22.000000 textdistance-4.6.2/textdistance/algorithms/sequence_based.py
+-rw-rw-r--   0 gram      (1000) gram      (1000)     3209 2023-09-27 11:33:22.000000 textdistance-4.6.2/textdistance/algorithms/simple.py
+-rw-rw-r--   0 gram      (1000) gram      (1000)     9405 2023-09-28 08:28:37.000000 textdistance-4.6.2/textdistance/algorithms/token_based.py
+-rw-rw-r--   0 gram      (1000) gram      (1000)      166 2023-09-27 11:33:22.000000 textdistance-4.6.2/textdistance/algorithms/types.py
+-rw-rw-r--   0 gram      (1000) gram      (1000)     2821 2023-09-27 11:33:22.000000 textdistance-4.6.2/textdistance/algorithms/vector_based.py
+-rw-rw-r--   0 gram      (1000) gram      (1000)     3818 2023-09-27 11:33:22.000000 textdistance-4.6.2/textdistance/benchmark.py
+-rw-rw-r--   0 gram      (1000) gram      (1000)     1161 2023-12-29 09:20:18.000000 textdistance-4.6.2/textdistance/libraries.json
+-rw-rw-r--   0 gram      (1000) gram      (1000)     6716 2023-09-28 07:20:22.000000 textdistance-4.6.2/textdistance/libraries.py
+-rw-rw-r--   0 gram      (1000) gram      (1000)        0 2022-09-09 12:27:03.000000 textdistance-4.6.2/textdistance/py.typed
+-rw-rw-r--   0 gram      (1000) gram      (1000)      783 2023-09-27 11:33:22.000000 textdistance-4.6.2/textdistance/utils.py
+drwxrwxr-x   0 gram      (1000) gram      (1000)        0 2024-04-24 11:35:42.832659 textdistance-4.6.2/textdistance.egg-info/
+-rw-r--r--   0 gram      (1000) gram      (1000)    14636 2024-04-24 11:35:42.000000 textdistance-4.6.2/textdistance.egg-info/PKG-INFO
+-rw-rw-r--   0 gram      (1000) gram      (1000)      810 2024-04-24 11:35:42.000000 textdistance-4.6.2/textdistance.egg-info/SOURCES.txt
+-rw-rw-r--   0 gram      (1000) gram      (1000)        1 2024-04-24 11:35:42.000000 textdistance-4.6.2/textdistance.egg-info/dependency_links.txt
+-rw-rw-r--   0 gram      (1000) gram      (1000)     1097 2024-04-24 11:35:42.000000 textdistance-4.6.2/textdistance.egg-info/requires.txt
+-rw-rw-r--   0 gram      (1000) gram      (1000)       13 2024-04-24 11:35:42.000000 textdistance-4.6.2/textdistance.egg-info/top_level.txt
```

### Comparing `textdistance-4.6.1/LICENSE` & `textdistance-4.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `textdistance-4.6.1/PKG-INFO` & `textdistance-4.6.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textdistance
-Version: 4.6.1
+Version: 4.6.2
 Summary: Compute distance between the two texts.
 Home-page: https://github.com/orsinium/textdistance
 Download-URL: https://github.com/orsinium/textdistance/tarball/master
 Author: orsinium
 Author-email: gram@orsinium.dev
 License: MIT
 Keywords: distance between text strings sequences iterators
@@ -12,102 +12,28 @@
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Provides-Extra: extras
-Requires-Dist: jellyfish; extra == "extras"
-Requires-Dist: numpy; extra == "extras"
-Requires-Dist: Levenshtein; extra == "extras"
-Requires-Dist: pyxDamerauLevenshtein; extra == "extras"
-Requires-Dist: rapidfuzz>=2.6.0; extra == "extras"
 Provides-Extra: benchmark
-Requires-Dist: jellyfish; extra == "benchmark"
-Requires-Dist: numpy; extra == "benchmark"
-Requires-Dist: Levenshtein; extra == "benchmark"
-Requires-Dist: pyxDamerauLevenshtein; extra == "benchmark"
-Requires-Dist: rapidfuzz>=2.6.0; extra == "benchmark"
-Requires-Dist: distance; extra == "benchmark"
-Requires-Dist: pylev; extra == "benchmark"
-Requires-Dist: py_stringmatching; extra == "benchmark"
-Requires-Dist: tabulate; extra == "benchmark"
 Provides-Extra: test
-Requires-Dist: hypothesis; extra == "test"
-Requires-Dist: isort; extra == "test"
-Requires-Dist: numpy; extra == "test"
-Requires-Dist: pytest; extra == "test"
 Provides-Extra: lint
-Requires-Dist: twine; extra == "lint"
-Requires-Dist: mypy; extra == "lint"
-Requires-Dist: isort; extra == "lint"
-Requires-Dist: flake8; extra == "lint"
-Requires-Dist: types-tabulate; extra == "lint"
-Requires-Dist: flake8-blind-except; extra == "lint"
-Requires-Dist: flake8-bugbear; extra == "lint"
-Requires-Dist: flake8-commas; extra == "lint"
-Requires-Dist: flake8-logging-format; extra == "lint"
-Requires-Dist: flake8-mutable; extra == "lint"
-Requires-Dist: flake8-pep3101; extra == "lint"
-Requires-Dist: flake8-quotes; extra == "lint"
-Requires-Dist: flake8-string-format; extra == "lint"
-Requires-Dist: flake8-tidy-imports; extra == "lint"
-Requires-Dist: pep8-naming; extra == "lint"
-Provides-Extra: dameraulevenshtein
-Requires-Dist: rapidfuzz>=2.6.0; extra == "dameraulevenshtein"
-Requires-Dist: jellyfish; extra == "dameraulevenshtein"
-Requires-Dist: pyxDamerauLevenshtein; extra == "dameraulevenshtein"
-Provides-Extra: hamming
-Requires-Dist: Levenshtein; extra == "hamming"
-Requires-Dist: rapidfuzz>=2.6.0; extra == "hamming"
-Requires-Dist: jellyfish; extra == "hamming"
-Requires-Dist: distance; extra == "hamming"
-Provides-Extra: jaro
-Requires-Dist: rapidfuzz>=2.6.0; extra == "jaro"
-Requires-Dist: Levenshtein; extra == "jaro"
-Provides-Extra: jarowinkler
-Requires-Dist: rapidfuzz>=2.6.0; extra == "jarowinkler"
-Requires-Dist: jellyfish; extra == "jarowinkler"
-Provides-Extra: levenshtein
-Requires-Dist: rapidfuzz>=2.6.0; extra == "levenshtein"
-Requires-Dist: Levenshtein; extra == "levenshtein"
+Provides-Extra: DamerauLevenshtein
+Provides-Extra: Hamming
+Provides-Extra: Jaro
+Provides-Extra: JaroWinkler
+Provides-Extra: Levenshtein
 Provides-Extra: common
-Requires-Dist: jellyfish; extra == "common"
-Requires-Dist: numpy; extra == "common"
-Requires-Dist: Levenshtein; extra == "common"
-Requires-Dist: pyxDamerauLevenshtein; extra == "common"
-Requires-Dist: rapidfuzz>=2.6.0; extra == "common"
 Provides-Extra: all
-Requires-Dist: jellyfish; extra == "all"
-Requires-Dist: numpy; extra == "all"
-Requires-Dist: Levenshtein; extra == "all"
-Requires-Dist: pyxDamerauLevenshtein; extra == "all"
-Requires-Dist: rapidfuzz>=2.6.0; extra == "all"
-Requires-Dist: distance; extra == "all"
-Requires-Dist: pylev; extra == "all"
-Requires-Dist: py_stringmatching; extra == "all"
-Requires-Dist: tabulate; extra == "all"
 Provides-Extra: extra
-Requires-Dist: jellyfish; extra == "extra"
-Requires-Dist: numpy; extra == "extra"
-Requires-Dist: Levenshtein; extra == "extra"
-Requires-Dist: pyxDamerauLevenshtein; extra == "extra"
-Requires-Dist: rapidfuzz>=2.6.0; extra == "extra"
 Provides-Extra: benchmarks
-Requires-Dist: jellyfish; extra == "benchmarks"
-Requires-Dist: numpy; extra == "benchmarks"
-Requires-Dist: Levenshtein; extra == "benchmarks"
-Requires-Dist: pyxDamerauLevenshtein; extra == "benchmarks"
-Requires-Dist: rapidfuzz>=2.6.0; extra == "benchmarks"
-Requires-Dist: distance; extra == "benchmarks"
-Requires-Dist: pylev; extra == "benchmarks"
-Requires-Dist: py_stringmatching; extra == "benchmarks"
-Requires-Dist: tabulate; extra == "benchmarks"
+License-File: LICENSE
 
 # TextDistance
 
 ![TextDistance logo](logo.png)
 
 [![Build Status](https://travis-ci.org/life4/textdistance.svg?branch=master)](https://travis-ci.org/life4/textdistance) [![PyPI version](https://img.shields.io/pypi/v/textdistance.svg)](https://pypi.python.org/pypi/textdistance) [![Status](https://img.shields.io/pypi/status/textdistance.svg)](https://pypi.python.org/pypi/textdistance) [![License](https://img.shields.io/pypi/l/textdistance.svg)](LICENSE)
```

### Comparing `textdistance-4.6.1/README.md` & `textdistance-4.6.2/README.md`

 * *Files identical despite different names*

### Comparing `textdistance-4.6.1/setup.cfg` & `textdistance-4.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `textdistance-4.6.1/setup.py` & `textdistance-4.6.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         long_description = open('README.md').read()
     except UnicodeDecodeError:
         long_description = ''
 
 
 setup(
     name='textdistance',
-    version='4.6.1',
+    version='4.6.2',
 
     author='orsinium',
     author_email='gram@orsinium.dev',
 
     description='Compute distance between the two texts.',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `textdistance-4.6.1/tests/test_common.py` & `textdistance-4.6.2/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `textdistance-4.6.1/tests/test_external.py` & `textdistance-4.6.2/tests/test_external.py`

 * *Files identical despite different names*

### Comparing `textdistance-4.6.1/textdistance/algorithms/base.py` & `textdistance-4.6.2/textdistance/algorithms/base.py`

 * *Files identical despite different names*

### Comparing `textdistance-4.6.1/textdistance/algorithms/compression_based.py` & `textdistance-4.6.2/textdistance/algorithms/compression_based.py`

 * *Files identical despite different names*

### Comparing `textdistance-4.6.1/textdistance/algorithms/edit_based.py` & `textdistance-4.6.2/textdistance/algorithms/edit_based.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
             prev, cur = cur, [r] + [0] * (cols - 1)
             for c in range(1, cols):
                 deletion = prev[c] + 1
                 insertion = cur[c - 1] + 1
                 dist = self.test_func(s1[r - 1], s2[c - 1])
                 edit = prev[c - 1] + (not dist)
                 cur[c] = min(edit, deletion, insertion)
-        return cur[-1]
+        return int(cur[-1])
 
     def __call__(self, s1: Sequence[T], s2: Sequence[T]) -> int:
         s1, s2 = self._get_sequences(s1, s2)
 
         result = self.quick_answer(s1, s2)
         if result is not None:
             assert isinstance(result, int)
```

### Comparing `textdistance-4.6.1/textdistance/algorithms/phonetic.py` & `textdistance-4.6.2/textdistance/algorithms/phonetic.py`

 * *Files identical despite different names*

### Comparing `textdistance-4.6.1/textdistance/algorithms/sequence_based.py` & `textdistance-4.6.2/textdistance/algorithms/sequence_based.py`

 * *Files identical despite different names*

### Comparing `textdistance-4.6.1/textdistance/algorithms/simple.py` & `textdistance-4.6.2/textdistance/algorithms/simple.py`

 * *Files identical despite different names*

### Comparing `textdistance-4.6.1/textdistance/algorithms/token_based.py` & `textdistance-4.6.2/textdistance/algorithms/token_based.py`

 * *Files identical despite different names*

### Comparing `textdistance-4.6.1/textdistance/algorithms/vector_based.py` & `textdistance-4.6.2/textdistance/algorithms/vector_based.py`

 * *Files identical despite different names*

### Comparing `textdistance-4.6.1/textdistance/benchmark.py` & `textdistance-4.6.2/textdistance/benchmark.py`

 * *Files identical despite different names*

### Comparing `textdistance-4.6.1/textdistance/libraries.json` & `textdistance-4.6.2/textdistance/libraries.json`

 * *Files identical despite different names*

### Comparing `textdistance-4.6.1/textdistance/libraries.py` & `textdistance-4.6.2/textdistance/libraries.py`

 * *Files identical despite different names*

### Comparing `textdistance-4.6.1/textdistance/utils.py` & `textdistance-4.6.2/textdistance/utils.py`

 * *Files identical despite different names*

### Comparing `textdistance-4.6.1/textdistance.egg-info/PKG-INFO` & `textdistance-4.6.2/textdistance.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textdistance
-Version: 4.6.1
+Version: 4.6.2
 Summary: Compute distance between the two texts.
 Home-page: https://github.com/orsinium/textdistance
 Download-URL: https://github.com/orsinium/textdistance/tarball/master
 Author: orsinium
 Author-email: gram@orsinium.dev
 License: MIT
 Keywords: distance between text strings sequences iterators
@@ -12,102 +12,28 @@
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Provides-Extra: extras
-Requires-Dist: jellyfish; extra == "extras"
-Requires-Dist: numpy; extra == "extras"
-Requires-Dist: Levenshtein; extra == "extras"
-Requires-Dist: pyxDamerauLevenshtein; extra == "extras"
-Requires-Dist: rapidfuzz>=2.6.0; extra == "extras"
 Provides-Extra: benchmark
-Requires-Dist: jellyfish; extra == "benchmark"
-Requires-Dist: numpy; extra == "benchmark"
-Requires-Dist: Levenshtein; extra == "benchmark"
-Requires-Dist: pyxDamerauLevenshtein; extra == "benchmark"
-Requires-Dist: rapidfuzz>=2.6.0; extra == "benchmark"
-Requires-Dist: distance; extra == "benchmark"
-Requires-Dist: pylev; extra == "benchmark"
-Requires-Dist: py_stringmatching; extra == "benchmark"
-Requires-Dist: tabulate; extra == "benchmark"
 Provides-Extra: test
-Requires-Dist: hypothesis; extra == "test"
-Requires-Dist: isort; extra == "test"
-Requires-Dist: numpy; extra == "test"
-Requires-Dist: pytest; extra == "test"
 Provides-Extra: lint
-Requires-Dist: twine; extra == "lint"
-Requires-Dist: mypy; extra == "lint"
-Requires-Dist: isort; extra == "lint"
-Requires-Dist: flake8; extra == "lint"
-Requires-Dist: types-tabulate; extra == "lint"
-Requires-Dist: flake8-blind-except; extra == "lint"
-Requires-Dist: flake8-bugbear; extra == "lint"
-Requires-Dist: flake8-commas; extra == "lint"
-Requires-Dist: flake8-logging-format; extra == "lint"
-Requires-Dist: flake8-mutable; extra == "lint"
-Requires-Dist: flake8-pep3101; extra == "lint"
-Requires-Dist: flake8-quotes; extra == "lint"
-Requires-Dist: flake8-string-format; extra == "lint"
-Requires-Dist: flake8-tidy-imports; extra == "lint"
-Requires-Dist: pep8-naming; extra == "lint"
-Provides-Extra: dameraulevenshtein
-Requires-Dist: rapidfuzz>=2.6.0; extra == "dameraulevenshtein"
-Requires-Dist: jellyfish; extra == "dameraulevenshtein"
-Requires-Dist: pyxDamerauLevenshtein; extra == "dameraulevenshtein"
-Provides-Extra: hamming
-Requires-Dist: Levenshtein; extra == "hamming"
-Requires-Dist: rapidfuzz>=2.6.0; extra == "hamming"
-Requires-Dist: jellyfish; extra == "hamming"
-Requires-Dist: distance; extra == "hamming"
-Provides-Extra: jaro
-Requires-Dist: rapidfuzz>=2.6.0; extra == "jaro"
-Requires-Dist: Levenshtein; extra == "jaro"
-Provides-Extra: jarowinkler
-Requires-Dist: rapidfuzz>=2.6.0; extra == "jarowinkler"
-Requires-Dist: jellyfish; extra == "jarowinkler"
-Provides-Extra: levenshtein
-Requires-Dist: rapidfuzz>=2.6.0; extra == "levenshtein"
-Requires-Dist: Levenshtein; extra == "levenshtein"
+Provides-Extra: DamerauLevenshtein
+Provides-Extra: Hamming
+Provides-Extra: Jaro
+Provides-Extra: JaroWinkler
+Provides-Extra: Levenshtein
 Provides-Extra: common
-Requires-Dist: jellyfish; extra == "common"
-Requires-Dist: numpy; extra == "common"
-Requires-Dist: Levenshtein; extra == "common"
-Requires-Dist: pyxDamerauLevenshtein; extra == "common"
-Requires-Dist: rapidfuzz>=2.6.0; extra == "common"
 Provides-Extra: all
-Requires-Dist: jellyfish; extra == "all"
-Requires-Dist: numpy; extra == "all"
-Requires-Dist: Levenshtein; extra == "all"
-Requires-Dist: pyxDamerauLevenshtein; extra == "all"
-Requires-Dist: rapidfuzz>=2.6.0; extra == "all"
-Requires-Dist: distance; extra == "all"
-Requires-Dist: pylev; extra == "all"
-Requires-Dist: py_stringmatching; extra == "all"
-Requires-Dist: tabulate; extra == "all"
 Provides-Extra: extra
-Requires-Dist: jellyfish; extra == "extra"
-Requires-Dist: numpy; extra == "extra"
-Requires-Dist: Levenshtein; extra == "extra"
-Requires-Dist: pyxDamerauLevenshtein; extra == "extra"
-Requires-Dist: rapidfuzz>=2.6.0; extra == "extra"
 Provides-Extra: benchmarks
-Requires-Dist: jellyfish; extra == "benchmarks"
-Requires-Dist: numpy; extra == "benchmarks"
-Requires-Dist: Levenshtein; extra == "benchmarks"
-Requires-Dist: pyxDamerauLevenshtein; extra == "benchmarks"
-Requires-Dist: rapidfuzz>=2.6.0; extra == "benchmarks"
-Requires-Dist: distance; extra == "benchmarks"
-Requires-Dist: pylev; extra == "benchmarks"
-Requires-Dist: py_stringmatching; extra == "benchmarks"
-Requires-Dist: tabulate; extra == "benchmarks"
+License-File: LICENSE
 
 # TextDistance
 
 ![TextDistance logo](logo.png)
 
 [![Build Status](https://travis-ci.org/life4/textdistance.svg?branch=master)](https://travis-ci.org/life4/textdistance) [![PyPI version](https://img.shields.io/pypi/v/textdistance.svg)](https://pypi.python.org/pypi/textdistance) [![Status](https://img.shields.io/pypi/status/textdistance.svg)](https://pypi.python.org/pypi/textdistance) [![License](https://img.shields.io/pypi/l/textdistance.svg)](LICENSE)
```

### Comparing `textdistance-4.6.1/textdistance.egg-info/SOURCES.txt` & `textdistance-4.6.2/textdistance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `textdistance-4.6.1/textdistance.egg-info/requires.txt` & `textdistance-4.6.2/textdistance.egg-info/requires.txt`

 * *Files identical despite different names*

