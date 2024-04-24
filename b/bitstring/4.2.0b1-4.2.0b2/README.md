# Comparing `tmp/bitstring-4.2.0b1.tar.gz` & `tmp/bitstring-4.2.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitstring-4.2.0b1.tar", last modified: Wed Jan 24 15:53:04 2024, max compression
+gzip compressed data, was "bitstring-4.2.0b2.tar", last modified: Wed Mar 27 20:47:38 2024, max compression
```

## Comparing `bitstring-4.2.0b1.tar` & `bitstring-4.2.0b2.tar`

### file list

```diff
@@ -1,43 +1,47 @@
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2024-01-24 15:53:04.456639 bitstring-4.2.0b1/
--rw-r--r--   0 scott     (1000) scott     (1000)     1127 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)      182 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/MANIFEST.in
--rw-r--r--   0 scott     (1000) scott     (1000)     5997 2024-01-24 15:53:04.456639 bitstring-4.2.0b1/PKG-INFO
--rw-r--r--   0 scott     (1000) scott     (1000)     5071 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/README.md
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2024-01-24 15:53:04.456639 bitstring-4.2.0b1/bitstring/
--rw-r--r--   0 scott     (1000) scott     (1000)    11728 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/bitstring/__init__.py
--rw-r--r--   0 scott     (1000) scott     (1000)     1706 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/bitstring/__main__.py
--rw-r--r--   0 scott     (1000) scott     (1000)    34521 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/bitstring/array_.py
--rw-r--r--   0 scott     (1000) scott     (1000)    22797 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/bitstring/bitarray_.py
--rw-r--r--   0 scott     (1000) scott     (1000)    77900 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/bitstring/bits.py
--rw-r--r--   0 scott     (1000) scott     (1000)     9677 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/bitstring/bitstore.py
--rw-r--r--   0 scott     (1000) scott     (1000)     8248 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/bitstring/bitstore_helpers.py
--rw-r--r--   0 scott     (1000) scott     (1000)    28801 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/bitstring/bitstream.py
--rw-r--r--   0 scott     (1000) scott     (1000)     3409 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/bitstring/bitstring_options.py
--rw-r--r--   0 scott     (1000) scott     (1000)    10770 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/bitstring/dtypes.py
--rw-r--r--   0 scott     (1000) scott     (1000)      578 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/bitstring/exceptions.py
--rw-r--r--   0 scott     (1000) scott     (1000)     9121 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/bitstring/fp8.py
--rw-r--r--   0 scott     (1000) scott     (1000)     4543 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/bitstring/methods.py
--rw-r--r--   0 scott     (1000) scott     (1000)        0 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/bitstring/py.typed
--rw-r--r--   0 scott     (1000) scott     (1000)     9489 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/bitstring/utils.py
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2024-01-24 15:53:04.456639 bitstring-4.2.0b1/bitstring.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     5997 2024-01-24 15:53:04.000000 bitstring-4.2.0b1/bitstring.egg-info/PKG-INFO
--rw-r--r--   0 scott     (1000) scott     (1000)      811 2024-01-24 15:53:04.000000 bitstring-4.2.0b1/bitstring.egg-info/SOURCES.txt
--rw-r--r--   0 scott     (1000) scott     (1000)        1 2024-01-24 15:53:04.000000 bitstring-4.2.0b1/bitstring.egg-info/dependency_links.txt
--rw-r--r--   0 scott     (1000) scott     (1000)       23 2024-01-24 15:53:04.000000 bitstring-4.2.0b1/bitstring.egg-info/requires.txt
--rw-r--r--   0 scott     (1000) scott     (1000)       10 2024-01-24 15:53:04.000000 bitstring-4.2.0b1/bitstring.egg-info/top_level.txt
--rw-r--r--   0 scott     (1000) scott     (1000)     1194 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/pyproject.toml
--rw-r--r--   0 scott     (1000) scott     (1000)    67468 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/release_notes.txt
--rw-r--r--   0 scott     (1000) scott     (1000)       38 2024-01-24 15:53:04.456639 bitstring-4.2.0b1/setup.cfg
-drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2024-01-24 15:53:04.456639 bitstring-4.2.0b1/tests/
--rw-r--r--   0 scott     (1000) scott     (1000)        0 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/tests/__init__.py
--rw-r--r--   0 scott     (1000) scott     (1000)        8 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/tests/smalltestfile
--rw-r--r--   0 scott     (1000) scott     (1000)   125300 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/tests/test.m1v
--rw-r--r--   0 scott     (1000) scott     (1000)    30598 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/tests/test_array.py
--rw-r--r--   0 scott     (1000) scott     (1000)    30484 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/tests/test_bitarray.py
--rw-r--r--   0 scott     (1000) scott     (1000)    32219 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/tests/test_bits.py
--rw-r--r--   0 scott     (1000) scott     (1000)     3193 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/tests/test_bitstore.py
--rw-r--r--   0 scott     (1000) scott     (1000)   147790 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/tests/test_bitstream.py
--rw-r--r--   0 scott     (1000) scott     (1000)     7152 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/tests/test_bitstring.py
--rw-r--r--   0 scott     (1000) scott     (1000)     7739 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/tests/test_constbitstream.py
--rw-r--r--   0 scott     (1000) scott     (1000)     2552 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/tests/test_dtypes.py
--rw-r--r--   0 scott     (1000) scott     (1000)     9299 2024-01-24 15:51:36.000000 bitstring-4.2.0b1/tests/test_fp8.py
+drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2024-03-27 20:47:38.663067 bitstring-4.2.0b2/
+-rw-r--r--   0 scott     (1000) scott     (1000)     1127 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)      182 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/MANIFEST.in
+-rw-r--r--   0 scott     (1000) scott     (1000)     6266 2024-03-27 20:47:38.663067 bitstring-4.2.0b2/PKG-INFO
+-rw-r--r--   0 scott     (1000) scott     (1000)     5341 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/README.md
+drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2024-03-27 20:47:38.653067 bitstring-4.2.0b2/bitstring/
+-rw-r--r--   0 scott     (1000) scott     (1000)    13977 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/bitstring/__init__.py
+-rw-r--r--   0 scott     (1000) scott     (1000)     1706 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/bitstring/__main__.py
+-rw-r--r--   0 scott     (1000) scott     (1000)    36502 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/bitstring/array_.py
+-rw-r--r--   0 scott     (1000) scott     (1000)    22797 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/bitstring/bitarray_.py
+-rw-r--r--   0 scott     (1000) scott     (1000)    78927 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/bitstring/bits.py
+-rw-r--r--   0 scott     (1000) scott     (1000)     9745 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/bitstring/bitstore.py
+-rw-r--r--   0 scott     (1000) scott     (1000)     9328 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/bitstring/bitstore_helpers.py
+-rw-r--r--   0 scott     (1000) scott     (1000)    29424 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/bitstring/bitstream.py
+-rw-r--r--   0 scott     (1000) scott     (1000)     3651 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/bitstring/bitstring_options.py
+-rw-r--r--   0 scott     (1000) scott     (1000)    16699 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/bitstring/dtypes.py
+-rw-r--r--   0 scott     (1000) scott     (1000)      578 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/bitstring/exceptions.py
+-rw-r--r--   0 scott     (1000) scott     (1000)     3865 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/bitstring/fp8.py
+-rw-r--r--   0 scott     (1000) scott     (1000)    27588 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/bitstring/luts.py
+-rw-r--r--   0 scott     (1000) scott     (1000)     4446 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/bitstring/methods.py
+-rw-r--r--   0 scott     (1000) scott     (1000)     9061 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/bitstring/mxfp.py
+-rw-r--r--   0 scott     (1000) scott     (1000)        0 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/bitstring/py.typed
+-rw-r--r--   0 scott     (1000) scott     (1000)     9403 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/bitstring/utils.py
+drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2024-03-27 20:47:38.663067 bitstring-4.2.0b2/bitstring.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     6266 2024-03-27 20:47:38.000000 bitstring-4.2.0b2/bitstring.egg-info/PKG-INFO
+-rw-r--r--   0 scott     (1000) scott     (1000)      894 2024-03-27 20:47:38.000000 bitstring-4.2.0b2/bitstring.egg-info/SOURCES.txt
+-rw-r--r--   0 scott     (1000) scott     (1000)        1 2024-03-27 20:47:38.000000 bitstring-4.2.0b2/bitstring.egg-info/dependency_links.txt
+-rw-r--r--   0 scott     (1000) scott     (1000)       23 2024-03-27 20:47:38.000000 bitstring-4.2.0b2/bitstring.egg-info/requires.txt
+-rw-r--r--   0 scott     (1000) scott     (1000)       10 2024-03-27 20:47:38.000000 bitstring-4.2.0b2/bitstring.egg-info/top_level.txt
+-rw-r--r--   0 scott     (1000) scott     (1000)     1194 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/pyproject.toml
+-rw-r--r--   0 scott     (1000) scott     (1000)    68944 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/release_notes.txt
+-rw-r--r--   0 scott     (1000) scott     (1000)       38 2024-03-27 20:47:38.663067 bitstring-4.2.0b2/setup.cfg
+drwxr-xr-x   0 scott     (1000) scott     (1000)        0 2024-03-27 20:47:38.663067 bitstring-4.2.0b2/tests/
+-rw-r--r--   0 scott     (1000) scott     (1000)        0 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/tests/__init__.py
+-rw-r--r--   0 scott     (1000) scott     (1000)        8 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/tests/smalltestfile
+-rw-r--r--   0 scott     (1000) scott     (1000)   125300 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/tests/test.m1v
+-rw-r--r--   0 scott     (1000) scott     (1000)    29098 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/tests/test_array.py
+-rw-r--r--   0 scott     (1000) scott     (1000)    28108 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/tests/test_bitarray.py
+-rw-r--r--   0 scott     (1000) scott     (1000)    30568 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/tests/test_bits.py
+-rw-r--r--   0 scott     (1000) scott     (1000)     2974 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/tests/test_bitstore.py
+-rw-r--r--   0 scott     (1000) scott     (1000)   136184 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/tests/test_bitstream.py
+-rw-r--r--   0 scott     (1000) scott     (1000)     6751 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/tests/test_bitstring.py
+-rw-r--r--   0 scott     (1000) scott     (1000)     7555 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/tests/test_constbitstream.py
+-rw-r--r--   0 scott     (1000) scott     (1000)     3748 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/tests/test_dtypes.py
+-rw-r--r--   0 scott     (1000) scott     (1000)    14031 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/tests/test_fp8.py
+-rw-r--r--   0 scott     (1000) scott     (1000)    14497 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/tests/test_mxfp.py
+-rw-r--r--   0 scott     (1000) scott     (1000)      263 2024-03-27 20:45:52.000000 bitstring-4.2.0b2/tests/test_scaled_dtypes.py
```

### Comparing `bitstring-4.2.0b1/LICENSE` & `bitstring-4.2.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `bitstring-4.2.0b1/PKG-INFO` & `bitstring-4.2.0b2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitstring
-Version: 4.2.0b1
+Version: 4.2.0b2
 Summary: Simple construction, analysis and modification of binary data.
 Author-email: Scott Griffiths <dr.scottgriffiths@gmail.com>
 Project-URL: homepage, https://github.com/scott-griffiths/bitstring
 Project-URL: documentation, https://bitstring.readthedocs.io/
 Keywords: binary,bitarray,bitvector,bitfield
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -33,25 +33,33 @@
 
 
 [![CI badge](https://github.com/scott-griffiths/bitstring/actions/workflows/.github/workflows/ci.yml/badge.svg)](https://github.com/scott-griffiths/bitstring/actions/workflows/ci.yml)
 [![Docs](https://img.shields.io/readthedocs/bitstring?logo=readthedocs&logoColor=white)](https://bitstring.readthedocs.io/en/latest/)
 [![Codacy Badge](https://img.shields.io/codacy/grade/8869499b2eed44548fa1a5149dd451f4?logo=codacy)](https://app.codacy.com/gh/scott-griffiths/bitstring/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/bitstring?logo=libraries.io&logoColor=white)](https://libraries.io/pypi/bitstring)
 &nbsp; &nbsp;
-[![Pepy Total Downlods](https://img.shields.io/pepy/dt/bitstring?logo=python&logoColor=white&labelColor=blue&color=blue)](https://pypistats.org/packages/bitstring)
+[![Pepy Total Downlods](https://img.shields.io/pepy/dt/bitstring?logo=python&logoColor=white&labelColor=blue&color=blue)](https://www.pepy.tech/projects/bitstring)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/bitstring?label=%40&labelColor=blue&color=blue)](https://pypistats.org/packages/bitstring)
 
 
 News
 ----
-**29th November 2023**: bitstring 4.1.4 released. Version 4.1 is a large update in terms of how much of the code has changed.
+**March 2024**: bitstring 4.2.0b2 released. This is the final beta release before 4.2. 
 
-* New Array class for homogeneous data.
-* Support for 8-bit floating point values.
-* Speed increased with bitarray dependency.
+Install the beta with `pip install bitstring==4.2.0b2`, or use `pip install bitstring` for the latest stable version.
+
+New in 4.2:
+
+* Dropped support for Python 3.7. Minimum version is now 3.8.
+* A new `Dtype` class can be optionally used to specify types.
+* The `bitstring.options` object is now the preferred method for changing module options.
+* New `fromstring` method as another way to create bitstrings from formatted strings.
+* More types can now be pretty printed.
+* A range of 8-bit, 6-bit and even 4-bit float formats added (beta):
+* Performance improvements.
 
 See the [release notes](https://github.com/scott-griffiths/bitstring/blob/main/release_notes.txt) for details. Please let me know if you encounter any problems.
 
 
 Overview
 --------
 
@@ -133,24 +141,17 @@
      >>> a.data
      BitArray('0x1390181')
      >>> a[::2] *= 5
      >>> a
      Array('uint7', [45, 100, 15, 1])
 
 
-Unit Tests
-----------
-
-The 700+ unit tests should all pass. They can be run from the root of the project with
-
-     python -m unittest
-
 
 Credits
 -------
 
 Created in 2006 to help with ad hoc parsing and creation of compressed video files.
 Maintained and expanded ever since as it became unexpectedly popular.
 Thanks to all those who have contributed ideas and code (and bug reports) over the years.
 
 
-<sub>Copyright (c) 2006 - 2023 Scott Griffiths</sub>
+<sub>Copyright (c) 2006 - 2024 Scott Griffiths</sub>
```

### Comparing `bitstring-4.2.0b1/README.md` & `bitstring-4.2.0b2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,25 +9,33 @@
 
 
 [![CI badge](https://github.com/scott-griffiths/bitstring/actions/workflows/.github/workflows/ci.yml/badge.svg)](https://github.com/scott-griffiths/bitstring/actions/workflows/ci.yml)
 [![Docs](https://img.shields.io/readthedocs/bitstring?logo=readthedocs&logoColor=white)](https://bitstring.readthedocs.io/en/latest/)
 [![Codacy Badge](https://img.shields.io/codacy/grade/8869499b2eed44548fa1a5149dd451f4?logo=codacy)](https://app.codacy.com/gh/scott-griffiths/bitstring/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/bitstring?logo=libraries.io&logoColor=white)](https://libraries.io/pypi/bitstring)
 &nbsp; &nbsp;
-[![Pepy Total Downlods](https://img.shields.io/pepy/dt/bitstring?logo=python&logoColor=white&labelColor=blue&color=blue)](https://pypistats.org/packages/bitstring)
+[![Pepy Total Downlods](https://img.shields.io/pepy/dt/bitstring?logo=python&logoColor=white&labelColor=blue&color=blue)](https://www.pepy.tech/projects/bitstring)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/bitstring?label=%40&labelColor=blue&color=blue)](https://pypistats.org/packages/bitstring)
 
 
 News
 ----
-**29th November 2023**: bitstring 4.1.4 released. Version 4.1 is a large update in terms of how much of the code has changed.
+**March 2024**: bitstring 4.2.0b2 released. This is the final beta release before 4.2. 
 
-* New Array class for homogeneous data.
-* Support for 8-bit floating point values.
-* Speed increased with bitarray dependency.
+Install the beta with `pip install bitstring==4.2.0b2`, or use `pip install bitstring` for the latest stable version.
+
+New in 4.2:
+
+* Dropped support for Python 3.7. Minimum version is now 3.8.
+* A new `Dtype` class can be optionally used to specify types.
+* The `bitstring.options` object is now the preferred method for changing module options.
+* New `fromstring` method as another way to create bitstrings from formatted strings.
+* More types can now be pretty printed.
+* A range of 8-bit, 6-bit and even 4-bit float formats added (beta):
+* Performance improvements.
 
 See the [release notes](https://github.com/scott-griffiths/bitstring/blob/main/release_notes.txt) for details. Please let me know if you encounter any problems.
 
 
 Overview
 --------
 
@@ -109,24 +117,17 @@
      >>> a.data
      BitArray('0x1390181')
      >>> a[::2] *= 5
      >>> a
      Array('uint7', [45, 100, 15, 1])
 
 
-Unit Tests
-----------
-
-The 700+ unit tests should all pass. They can be run from the root of the project with
-
-     python -m unittest
-
 
 Credits
 -------
 
 Created in 2006 to help with ad hoc parsing and creation of compressed video files.
 Maintained and expanded ever since as it became unexpectedly popular.
 Thanks to all those who have contributed ideas and code (and bug reports) over the years.
 
 
-<sub>Copyright (c) 2006 - 2023 Scott Griffiths</sub>
+<sub>Copyright (c) 2006 - 2024 Scott Griffiths</sub>
```

### Comparing `bitstring-4.2.0b1/bitstring/__init__.py` & `bitstring-4.2.0b2/bitstring/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 Classes:
 
 Bits -- An immutable container for binary data.
 BitArray -- A mutable container for binary data.
 ConstBitStream -- An immutable container with streaming methods.
 BitStream -- A mutable container with streaming methods.
 Array -- An efficient list-like container where each item has a fixed-length binary format.
+Dtype -- Encapsulate the data types used in the other classes.
 
 Functions:
 
 pack -- Create a BitStream from a format string.
 
 Data:
-options -- A container for module-wide options:
-    bytealigned -- Determines whether a number of methods default to working only on byte boundaries.
-    lsb0 -- If True, the least significant bit (the final bit) is indexed as bit zero.
+
+options -- Module-wide options.
 
 Exceptions:
 
 Error -- Module exception base class.
 CreationError -- Error during creation.
 InterpretError -- Inappropriate interpretation of binary data.
 ByteAlignError -- Whole byte position or length needed.
@@ -51,15 +51,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
 
-__version__ = "4.2.0b1"
+__version__ = "4.2.0b2"
 
 __author__ = "Scott Griffiths"
 
 import sys
 
 from .bits import Bits
 from .bitstring_options import Options
@@ -67,14 +67,20 @@
 from .bitstream import ConstBitStream, BitStream
 from .methods import pack
 from .array_ import Array
 from .exceptions import Error, ReadError, InterpretError, ByteAlignError, CreationError
 from .dtypes import DtypeDefinition, dtype_register, Dtype
 import types
 from typing import List, Tuple, Literal
+from .mxfp import decompress_luts as mxfp_decompress_luts
+from .fp8 import decompress_luts as binary8_decompress_luts
+
+# Decompress the LUTs for the exotic floating point formats
+mxfp_decompress_luts()
+binary8_decompress_luts()
 
 # The Options class returns a singleton.
 options = Options()
 
 # These get defined properly by the module magic below. This just stops mypy complaining about them.
 bytealigned = lsb0 = None
 
@@ -132,21 +138,48 @@
 def float_bits2chars(bitlength: Literal[16, 32, 64]):
     # These bit lengths were found by looking at lots of possible values
     if bitlength in [16, 32]:
         return 23  # Empirical value
     else:
         return 24  # Empirical value
 
-def e5m2float_bits2chars(bitlength: Literal[8]):
+def p3binary_bits2chars(bitlength: Literal[8]):
     return 19  # Empirical value
 
-def e4m3float_bits2chars(bitlength: Literal[8]):
+def p4binary_bits2chars(bitlength: Literal[8]):
     # Found by looking at all the possible values
     return 13  # Empirical value
 
+def e4m3mxfp_bits2chars(bitlength: Literal[8]):
+    return 13
+
+def e5m2mxfp_bits2chars(bitlength: Literal[8]):
+    return 19
+
+def e3m2mxfp_bits2chars(bitlength: Literal[6]):
+    # Not sure what the best value is here. It's 7 without considering the scale that could be applied.
+    return 7
+
+def e2m3mxfp_bits2chars(bitlength: Literal[6]):
+    # Not sure what the best value is here.
+    return 7
+
+def e2m1mxfp_bits2chars(bitlength: Literal[4]):
+    # Not sure what the best value is here.
+    return 7
+
+def e8m0mxfp_bits2chars(bitlength: Literal[8]):
+    # Can range same as float32
+    return 23
+
+def mxint_bits2chars(bitlength: Literal[8]):
+    # Not sure what the best value is here.
+    return 10
+
+
 def bfloat_bits2chars(bitlength: Literal[16]):
     # Found by looking at all the possible values
     return 23  # Empirical value
 
 def bits_bits2chars(bitlength: int):
     # For bits type we can see how long it needs to be printed by trying any value
     temp = Bits(bitlength)
@@ -171,21 +204,17 @@
     DtypeDefinition('intbe', Bits._setintbe, Bits._getintbe, int, True, int_bits2chars,
                     allowed_lengths=(8, 16, 24, ...), description="a two's complement big-endian signed int"),
     # String types
     DtypeDefinition('hex', Bits._sethex, Bits._gethex, str, False, hex_bits2chars,
                     allowed_lengths=(0, 4, 8, ...), description="a hexadecimal string"),
     DtypeDefinition('bin', Bits._setbin_safe, Bits._getbin, str, False, bin_bits2chars,
                     description="a binary string"),
-    DtypeDefinition('oct',Bits._setoct, Bits._getoct, str, False, oct_bits2chars,
+    DtypeDefinition('oct', Bits._setoct, Bits._getoct, str, False, oct_bits2chars,
                     allowed_lengths=(0, 3, 6, ...), description="an octal string"),
     # Float types
-    DtypeDefinition('e5m2float', Bits._sete5m2float, Bits._gete5m2float, float, True, e5m2float_bits2chars,
-                    allowed_lengths=(8,), description="an 8 bit float with e5m2float format"),
-    DtypeDefinition('e4m3float', Bits._sete4m3float, Bits._gete4m3float, float, True, e4m3float_bits2chars,
-                    allowed_lengths=(8,), description="an 8 bit float with e4m3float format"),
     DtypeDefinition('float', Bits._setfloatbe, Bits._getfloatbe, float, True, float_bits2chars,
                     allowed_lengths=(16, 32, 64), description="a big-endian floating point number"),
     DtypeDefinition('floatle', Bits._setfloatle, Bits._getfloatle, float, True, float_bits2chars,
                     allowed_lengths=(16, 32, 64), description="a little-endian floating point number"),
     DtypeDefinition('bfloat', Bits._setbfloatbe, Bits._getbfloatbe, float, True, bfloat_bits2chars,
                     allowed_lengths=(16,), description="a 16 bit big-endian bfloat floating point number"),
     DtypeDefinition('bfloatle', Bits._setbfloatle, Bits._getbfloatle, float, True, bfloat_bits2chars,
@@ -205,14 +234,34 @@
     DtypeDefinition('sie', Bits._setsie, Bits._getsie, int, True, None,
                     variable_length=True, description="a signed interleaved exponential-Golomb code"),
     DtypeDefinition('uie', Bits._setuie, Bits._getuie, int, False, None,
                     variable_length=True, description="an unsigned interleaved exponential-Golomb code"),
     # Special case pad type
     DtypeDefinition('pad', Bits._setpad, Bits._getpad, None, False, None,
                     description="a skipped section of padding"),
+
+    # MXFP and IEEE 8-bit float types
+    DtypeDefinition('p3binary', Bits._setp3binary, Bits._getp3binary, float, True, p3binary_bits2chars,
+                    allowed_lengths=(8,), description="an 8 bit float with binary8p3 format"),
+    DtypeDefinition('p4binary', Bits._setp4binary, Bits._getp4binary, float, True, p4binary_bits2chars,
+                    allowed_lengths=(8,), description="an 8 bit float with binary8p4 format"),
+    DtypeDefinition('e4m3mxfp', Bits._sete4m3mxfp, Bits._gete4m3mxfp, float, True, e4m3mxfp_bits2chars,
+                    allowed_lengths=(8,), description="an 8 bit float with MXFP E4M3 format"),
+    DtypeDefinition('e5m2mxfp', Bits._sete5m2mxfp, Bits._gete5m2mxfp, float, True, e5m2mxfp_bits2chars,
+                    allowed_lengths=(8,), description="an 8 bit float with MXFP E5M2 format"),
+    DtypeDefinition('e3m2mxfp', Bits._sete3m2mxfp, Bits._gete3m2mxfp, float, True, e3m2mxfp_bits2chars,
+                    allowed_lengths=(6,), description="a 6 bit float with MXFP E3M2 format"),
+    DtypeDefinition('e2m3mxfp', Bits._sete2m3mxfp, Bits._gete2m3mxfp, float, True, e2m3mxfp_bits2chars,
+                    allowed_lengths=(6,), description="a 6 bit float with MXFP E2M3 format"),
+    DtypeDefinition('e2m1mxfp', Bits._sete2m1mxfp, Bits._gete2m1mxfp, float, True, e2m1mxfp_bits2chars,
+                    allowed_lengths=(4,), description="a 4 bit float with MXFP E2M1 format"),
+    DtypeDefinition('e8m0mxfp', Bits._sete8m0mxfp, Bits._gete8m0mxfp, float, False, e8m0mxfp_bits2chars,
+                    allowed_lengths=(8,), description="an 8 bit float with MXFP E8M0 format"),
+    DtypeDefinition('mxint', Bits._setmxint, Bits._getmxint, float, True, mxint_bits2chars,
+                    allowed_lengths=(8,), description="an 8 bit float with MXFP INT8 format"),
 ]
 
 
 aliases: List[Tuple[str, str]] = [
     # Floats default to big endian
     ('float', 'floatbe'),
     ('bfloat', 'bfloatbe'),
```

### Comparing `bitstring-4.2.0b1/bitstring/__main__.py` & `bitstring-4.2.0b2/bitstring/__main__.py`

 * *Files identical despite different names*

### Comparing `bitstring-4.2.0b1/bitstring/array_.py` & `bitstring-4.2.0b2/bitstring/array_.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,14 +66,19 @@
 
 
     """
 
     def __init__(self, dtype: Union[str, Dtype], initializer: Optional[Union[int, Array, array.array, Iterable, Bits, bytes, bytearray, memoryview, BinaryIO]] = None,
                  trailing_bits: Optional[BitsType] = None) -> None:
         self.data = BitArray()
+        if isinstance(dtype, Dtype) and dtype.scale == 'auto':
+            if isinstance(initializer, (int, Bits, bytes, bytearray, memoryview, BinaryIO)):
+                raise TypeError("An Array with an 'auto' scale factor can only be created from an iterable of values.")
+            auto_scale = self._calculate_auto_scale(initializer, dtype.name, dtype.length)
+            dtype = Dtype(dtype.name, dtype.length, scale=auto_scale)
         try:
             self._set_dtype(dtype)
         except ValueError as e:
             raise CreationError(e)
 
         if isinstance(initializer, numbers.Integral):
             self.data = BitArray(initializer * self._dtype.bitlength)
@@ -83,68 +88,91 @@
             self.fromfile(initializer)
         elif initializer is not None:
             self.extend(initializer)
 
         if trailing_bits is not None:
             self.data += BitArray._create_from_bitstype(trailing_bits)
 
+    _largest_values = None
+    @staticmethod
+    def _calculate_auto_scale(initializer, name: str, length: Optional[int]) -> float:
+        # Now need to find the largest power of 2 representable with this format.
+        if Array._largest_values is None:
+            Array._largest_values = {
+                'mxint8': Bits('0b01111111').mxint8,  # 1.0 + 63.0/64.0,
+                'e2m1mxfp4': Bits('0b0111').e2m1mxfp4,  # 6.0
+                'e2m3mxfp6': Bits('0b011111').e2m3mxfp6,  # 7.5
+                'e3m2mxfp6': Bits('0b011111').e3m2mxfp6,  # 28.0
+                'e4m3mxfp8': Bits('0b01111110').e4m3mxfp8,  # 448.0
+                'e5m2mxfp8': Bits('0b01111011').e5m2mxfp8,  # 57344.0
+                'p4binary8': Bits('0b01111110').p4binary8,  # 224.0
+                'p3binary8': Bits('0b01111110').p3binary8,  # 49152.0
+                'float16': Bits('0x7bff').float16,  # 65504.0
+                # The bfloat range is so large the scaling algorithm doesn't work well, so I'm disallowing it.
+                # 'bfloat16': Bits('0x7f7f').bfloat16,  # 3.38953139e38,
+            }
+        if f'{name}{length}' in Array._largest_values.keys():
+            float_values = Array('float64', initializer).tolist()
+            max_float_value = max(abs(x) for x in float_values)
+            if max_float_value == 0:
+                # This special case isn't covered in the standard. I'm choosing to return no scale.
+                return 1.0
+            log2 = int(math.log2(max_float_value))
+            lp2 = int(math.log2(Array._largest_values[f'{name}{length}']))
+            lg_scale = log2 - lp2
+            # Saturate at values representable in E8M0 format.
+            if lg_scale > 127:
+                lg_scale = 127
+            elif lg_scale < -127:
+                lg_scale = -127
+            return 2 ** lg_scale
+        else:
+            raise ValueError(f"Can't calculate auto scale for format '{name}{length}'. "
+                             f"This feature is only available for these formats: {list(Array._largest_values.keys())}.")
+
     @property
     def itemsize(self) -> int:
         return self._dtype.length
 
     @property
     def trailing_bits(self) -> BitArray:
         trailing_bit_length = len(self.data) % self._dtype.bitlength
         return BitArray() if trailing_bit_length == 0 else self.data[-trailing_bit_length:]
 
-    # Converting array.array typecodes to our equivalents.
-    _array_typecodes: dict[str, str] = {'b': 'int8',
-                                        'B': 'uint8',
-                                        'h': 'intne16',
-                                        'H': 'uintne16',
-                                        'l': 'intne32',
-                                        'L': 'uintne32',
-                                        'q': 'intne64',
-                                        'Q': 'uintne64',
-                                        'e': 'floatne16',
-                                        'f': 'floatne32',
-                                        'd': 'floatne64'}
-
     @property
     def dtype(self) -> Dtype:
         return self._dtype
 
     @dtype.setter
     def dtype(self, new_dtype: Union[str, Dtype]) -> None:
         self._set_dtype(new_dtype)
 
     def _set_dtype(self, new_dtype: Union[str, Dtype]) -> None:
         if isinstance(new_dtype, Dtype):
             self._dtype = new_dtype
-            self._fmt = str(self._dtype)
         else:
             try:
                 dtype = Dtype(new_dtype)
             except ValueError:
                 name_length = utils.parse_single_struct_token(new_dtype)
                 if name_length is not None:
                     dtype = Dtype(*name_length)
                 else:
                     raise ValueError(f"Inappropriate Dtype for Array: '{new_dtype}'.")
             if dtype.length is None:
                 raise ValueError(f"A fixed length format is needed for an Array, received '{new_dtype}'.")
             self._dtype = dtype
-            self._fmt = new_dtype
+        if self._dtype.scale == 'auto':
+            raise ValueError("A Dtype with an 'auto' scale factor can only be used when creating a new Array.")
 
     def _create_element(self, value: ElementType) -> Bits:
         """Create Bits from value according to the token_name and token_length"""
-        b = Bits()
-        self._dtype.set_fn(b, value)
+        b = self._dtype.build(value)
         if len(b) != self._dtype.length:
-            raise ValueError(f"The value {value!r} has the wrong length for the format '{self._fmt}'.")
+            raise ValueError(f"The value {value!r} has the wrong length for the format '{self._dtype}'.")
         return b
 
     def __len__(self) -> int:
         return len(self.data) // self._dtype.length
 
     @overload
     def __getitem__(self, key: slice) -> Array:
@@ -157,19 +185,19 @@
     def __getitem__(self, key: Union[slice, int]) -> Union[Array, ElementType]:
         if isinstance(key, slice):
             start, stop, step = key.indices(len(self))
             if step != 1:
                 d = BitArray()
                 for s in range(start * self._dtype.length, stop * self._dtype.length, step * self._dtype.length):
                     d.append(self.data[s: s + self._dtype.length])
-                a = Array(self._dtype)
+                a = self.__class__(self._dtype)
                 a.data = d
                 return a
             else:
-                a = Array(self._dtype)
+                a = self.__class__(self._dtype)
                 a.data = self.data[start * self._dtype.length: stop * self._dtype.length]
                 return a
         else:
             if key < 0:
                 key += len(self)
             if key < 0 or key >= len(self):
                 raise IndexError(f"Index {key} out of range for Array of length {len(self)}.")
@@ -230,48 +258,48 @@
             del self.data[start: start + self._dtype.length]
 
     def __repr__(self) -> str:
         list_str = f"{self.tolist()}"
         trailing_bit_length = len(self.data) % self._dtype.length
         final_str = "" if trailing_bit_length == 0 else ", trailing_bits=" + repr(
             self.data[-trailing_bit_length:])
-        return f"Array('{self._fmt}', {list_str}{final_str})"
+        return f"Array('{self._dtype}', {list_str}{final_str})"
 
     def astype(self, dtype: Union[str, Dtype]) -> Array:
         """Return Array with elements of new dtype, initialised from current Array."""
-        new_array = Array(dtype, self.tolist())
+        new_array = self.__class__(dtype, self.tolist())
         return new_array
 
     def tolist(self) -> List[ElementType]:
-        return [self._dtype.read_fn(self.data, start=start)
+        return  [self._dtype.read_fn(self.data, start=start)
                 for start in range(0, len(self.data) - self._dtype.length + 1, self._dtype.length)]
 
     def append(self, x: ElementType) -> None:
         if len(self.data) % self._dtype.length != 0:
             raise ValueError("Cannot append to Array as its length is not a multiple of the format length.")
         self.data += self._create_element(x)
 
-    def extend(self, iterable: Union[Array, array.array, Iterable]) -> None:
+    def extend(self, iterable: Union[Array, array.array, Iterable[Any]]) -> None:
         if len(self.data) % self._dtype.length != 0:
             raise ValueError(f"Cannot extend Array as its data length ({len(self.data)} bits) is not a multiple of the format length ({self._dtype.length} bits).")
         if isinstance(iterable, Array):
             if self._dtype.name != iterable._dtype.name or self._dtype.length != iterable._dtype.length:
                 raise TypeError(
-                    f"Cannot extend an Array with format '{self._fmt}' from an Array of format '{iterable._fmt}'.")
+                    f"Cannot extend an Array with format '{self._dtype}' from an Array of format '{iterable._dtype}'.")
             # No need to iterate over the elements, we can just append the data
             self.data.append(iterable.data)
         elif isinstance(iterable, array.array):
             # array.array types are always native-endian, hence the '='
             name_value = utils.parse_single_struct_token('=' + iterable.typecode)
             if name_value is None:
                 raise ValueError(f"Cannot extend from array with typecode {iterable.typecode}.")
-            other_dtype = dtype_register.get_dtype(*name_value)
+            other_dtype = dtype_register.get_dtype(*name_value, scale=None)
             if self._dtype.name != other_dtype.name or self._dtype.length != other_dtype.length:
                 raise ValueError(
-                    f"Cannot extend an Array with format '{self._fmt}' from an array with typecode '{iterable.typecode}'.")
+                    f"Cannot extend an Array with format '{self._dtype}' from an array with typecode '{iterable.typecode}'.")
             self.data += iterable.tobytes()
         else:
             if isinstance(iterable, str):
                 raise TypeError("Can't extend an Array with a str.")
             for item in iterable:
                 self.data += self._create_element(item)
 
@@ -298,15 +326,15 @@
         """Change the endianness in-place of all items in the Array.
 
         If the Array format is not a whole number of bytes a ValueError will be raised.
 
         """
         if self._dtype.length % 8 != 0:
             raise ValueError(
-                f"byteswap can only be used for whole-byte elements. The '{self._fmt}' format is {self._dtype.length} bits long.")
+                f"byteswap can only be used for whole-byte elements. The '{self._dtype}' format is {self._dtype.length} bits long.")
         self.data.byteswap(self.itemsize // 8)
 
     def count(self, value: ElementType) -> int:
         """Return count of Array items that equal value.
 
         value -- The quantity to compare each Array element to. Type should be appropriate for the Array format.
 
@@ -364,28 +392,27 @@
         fmt -- Data format string. Defaults to current Array dtype.
         width -- Max width of printed lines in characters. Defaults to 120. A single group will always
                  be printed per line even if it exceeds the max width.
         show_offset -- If True shows the element offset in the first column of each line.
         stream -- A TextIO object with a write() method. Defaults to sys.stdout.
 
         """
-        colour = Colour(options.colourful_prettyprinting)
+        colour = Colour(not options.no_color)
         sep = ' '
         dtype2 = None
         tidy_fmt = None
         if fmt is None:
             fmt = self.dtype
             dtype1 = self.dtype
             tidy_fmt = "dtype='" + colour.purple + str(self.dtype) + "'" + colour.off
         else:
             token_list = utils.preprocess_tokens(fmt)
             if len(token_list) not in [1, 2]:
                 raise ValueError(f"Only one or two tokens can be used in an Array.pp() format - '{fmt}' has {len(token_list)} tokens.")
             dtype1 = Dtype(*utils.parse_name_length_token(token_list[0]))
-            parameter_str = f"fmt='{fmt}'"
             if len(token_list) == 2:
                 dtype2 = Dtype(*utils.parse_name_length_token(token_list[1]))
 
         token_length = dtype1.bitlength
         if dtype2 is not None:
             # For two types we're OK as long as they don't have different lengths given.
             if dtype1.bitlength is not None and dtype2.bitlength is not None and dtype1.bitlength != dtype2.bitlength:
@@ -401,15 +428,15 @@
             tidy_fmt = colour.purple + str(dtype1) + colour.off
             if dtype2 is not None:
                 tidy_fmt += ', ' + colour.blue + str(dtype2) + colour.off
             tidy_fmt = "fmt='" + tidy_fmt + "'"
         data = self.data if trailing_bit_length == 0 else self.data[0: -trailing_bit_length]
         length = len(self.data) // token_length
         len_str = colour.green + str(length) + colour.off
-        stream.write(f"<Array {tidy_fmt}, length={len_str}, itemsize={token_length} bits, total data size={(len(self.data) + 7) // 8} bytes> [\n")
+        stream.write(f"<{self.__class__.__name__} {tidy_fmt}, length={len_str}, itemsize={token_length} bits, total data size={(len(self.data) + 7) // 8} bytes> [\n")
         data._pp(dtype1, dtype2, token_length, width, sep, format_sep, show_offset, stream, False, token_length)
         stream.write("]")
         if trailing_bit_length != 0:
             stream.write(" + trailing_bits = " + str(self.data[-trailing_bit_length:]))
         stream.write("\n")
 
     def equals(self, other: Any) -> bool:
@@ -439,21 +466,21 @@
     def __iter__(self) -> Iterable[ElementType]:
         start = 0
         for _ in range(len(self)):
             yield self._dtype.read_fn(self.data, start=start)
             start += self._dtype.length
 
     def __copy__(self) -> Array:
-        a_copy = Array(self._fmt)
+        a_copy = self.__class__(self._dtype)
         a_copy.data = copy.copy(self.data)
         return a_copy
 
     def _apply_op_to_all_elements(self, op, value: Union[int, float, None], is_comparison: bool = False) -> Array:
         """Apply op with value to each element of the Array and return a new Array"""
-        new_array = Array('bool' if is_comparison else self._dtype)
+        new_array = self.__class__('bool' if is_comparison else self._dtype)
         new_data = BitArray()
         failures = index = 0
         msg = ''
         if value is not None:
             def partial_op(a):
                 return op(a, value)
         else:
@@ -501,30 +528,30 @@
         a_copy._apply_bitwise_op_to_all_elements_inplace(op, value)
         return a_copy
 
     def _apply_bitwise_op_to_all_elements_inplace(self, op, value: BitsType) -> Array:
         """Apply op with value to each element of the Array as an unsigned integer in place."""
         value = BitArray._create_from_bitstype(value)
         if len(value) != self._dtype.length:
-            raise ValueError(f"Bitwise op needs a bitstring of length {self._dtype.length} to match format {self._fmt}.")
+            raise ValueError(f"Bitwise op needs a bitstring of length {self._dtype.length} to match format {self._dtype}.")
         for start in range(0, len(self) * self._dtype.length, self._dtype.length):
             self.data[start: start + self._dtype.length] = op(self.data[start: start + self._dtype.length], value)
         return self
 
     def _apply_op_between_arrays(self, op, other: Array, is_comparison: bool = False) -> Array:
         if len(self) != len(other):
             msg = f"Cannot operate element-wise on Arrays with different lengths ({len(self)} and {len(other)})."
             if op == operator.add or op == operator.iadd:
                 msg += " Use extend() if you want to concatenate Arrays."
             raise ValueError(msg)
         if is_comparison:
             new_type = dtype_register.get_dtype('bool', 1)
         else:
             new_type = self._promotetype(self._dtype, other._dtype)
-        new_array = Array(new_type)
+        new_array = self.__class__(new_type)
         new_data = BitArray()
         failures = index = 0
         msg = ''
         for i in range(len(self)):
             a = self._dtype.read_fn(self.data, start=self._dtype.length * i)
             b = other._dtype.read_fn(other.data, start=other._dtype.length * i)
             try:
@@ -549,15 +576,15 @@
         3. Floating point types always win against integer types.
         4. Signed integer types always win against unsigned integer types.
         5. Longer types win against shorter types.
         6. In a tie the first type wins against the second type.
 
         """
         def is_float(x): return x.return_type is float
-        def is_int(x): return x.return_type is int
+        def is_int(x): return x.return_type is int or x.return_type is bool
         if is_float(type1) + is_int(type1) + is_float(type2) + is_int(type2) != 2:
             raise ValueError(f"Only integer and floating point types can be combined - not '{type1}' and '{type2}'.")
         # If same type choose the widest
         if type1.name == type2.name:
             return type1 if type1.length > type2.length else type2
         # We choose floats above integers, irrespective of the widths
         if is_float(type1) and is_int(type2):
@@ -718,23 +745,29 @@
         return self._apply_op_to_all_elements(operator.ge, other, is_comparison=True)
 
     def __le__(self, other: Union[int, float, Array]) -> Array:
         if isinstance(other, Array):
             return self._apply_op_between_arrays(operator.le, other, is_comparison=True)
         return self._apply_op_to_all_elements(operator.le, other, is_comparison=True)
 
-    def __eq__(self, other: Union[int, float, str, BitsType, Array]) -> Array:
-        if isinstance(other, Array):
-            return self._apply_op_between_arrays(operator.eq, other, is_comparison=True)
-        return self._apply_op_to_all_elements(operator.eq, other, is_comparison=True)
+    def _eq_ne(self, op, other: Any) -> Array:
+        if isinstance(other, (int, float, str, Bits)):
+            return self._apply_op_to_all_elements(op, other, is_comparison=True)
+        try:
+            other = self.__class__(self.dtype, other)
+        except:
+            return NotImplemented
+        finally:
+            return self._apply_op_between_arrays(op, other, is_comparison=True)
 
-    def __ne__(self, other: Union[int, float, str, BitsType, Array]) -> Array:
-        if isinstance(other, Array):
-            return self._apply_op_between_arrays(operator.ne, other, is_comparison=True)
-        return self._apply_op_to_all_elements(operator.ne, other, is_comparison=True)
+    def __eq__(self, other: Any) -> Array:
+        return self._eq_ne(operator.eq, other)
+
+    def __ne__(self, other: Any) -> Array:
+        return self._eq_ne(operator.ne, other)
 
     # Unary operators
 
     def __neg__(self):
         return self._apply_op_to_all_elements(operator.neg, None)
 
     def __abs__(self):
```

### Comparing `bitstring-4.2.0b1/bitstring/bitarray_.py` & `bitstring-4.2.0b2/bitstring/bitarray_.py`

 * *Files identical despite different names*

### Comparing `bitstring-4.2.0b1/bitstring/bits.py` & `bitstring-4.2.0b2/bitstring/bits.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,33 +5,34 @@
 import sys
 import mmap
 import struct
 import array
 import io
 from collections import abc
 import functools
-from typing import Tuple, Union, List, Iterable, Any, Optional, \
-    BinaryIO, TextIO, overload, Iterator, Type, TypeVar
+from typing import Tuple, Union, List, Iterable, Any, Optional, BinaryIO, TextIO, overload, Iterator, Type, TypeVar
 import bitarray
 import bitarray.util
 import bitstring
 from bitstring.bitstore import BitStore
 from bitstring import bitstore_helpers, utils
 from bitstring.dtypes import Dtype, dtype_register
-from bitstring.fp8 import e4m3float_fmt, e5m2float_fmt
-from bitstring.bitstring_options import  Colour
+from bitstring.fp8 import p4binary_fmt, p3binary_fmt
+from bitstring.mxfp import e3m2mxfp_fmt, e2m3mxfp_fmt, e2m1mxfp_fmt, e4m3mxfp_saturate_fmt, e5m2mxfp_saturate_fmt
+from bitstring.bitstring_options import Colour
 
 # Things that can be converted to Bits when a Bits type is needed
 BitsType = Union['Bits', str, Iterable[Any], bool, BinaryIO, bytearray, bytes, memoryview, bitarray.bitarray]
 
 TBits = TypeVar("TBits", bound='Bits')
 
 # Maximum number of digits to use in __str__ and __repr__.
 MAX_CHARS: int = 250
 
+
 class Bits:
     """A container holding an immutable sequence of bits.
 
     For a mutable container use the BitArray class instead.
 
     Methods:
 
@@ -60,15 +61,15 @@
     Properties:
 
     [GENERATED_PROPERTY_DESCRIPTIONS]
 
     len -- Length of the bitstring in bits.
 
     """
-    __slots__ = ('_bitstore',)
+    __slots__ = ('_bitstore', '_filename')
 
     def __init__(self, auto: Optional[Union[BitsType, int]] = None, /, length: Optional[int] = None,
                  offset: Optional[int] = None, **kwargs) -> None:
         """Either specify an 'auto' initialiser:
         A string of comma separated tokens, an integer, a file object,
         a bytearray, a boolean iterable, an array or another bitstring.
 
@@ -163,16 +164,16 @@
         except ValueError as e:
             raise bitstring.CreationError(e)
 
     def __getattr__(self, attribute: str) -> Any:
         # Support for arbitrary attributes like u16 or f64.
         try:
             d = Dtype(attribute)
-        except ValueError as e:
-            raise AttributeError(e)
+        except ValueError:
+            raise AttributeError(f"'{self.__class__.__name__}' object has no attribute '{attribute}'.")
         if d.bitlength is not None and len(self) != d.bitlength:
             raise ValueError(f"bitstring length {len(self)} doesn't match length {d.bitlength} of property '{attribute}'.")
         return d.read_fn(self, 0)
 
     def __iter__(self) -> Iterable[bool]:
         return iter(self._bitstore)
 
@@ -198,20 +199,18 @@
     def __add__(self: TBits, bs: BitsType) -> TBits:
         """Concatenate bitstrings and return new bitstring.
 
         bs -- the bitstring to append.
 
         """
         bs = self.__class__._create_from_bitstype(bs)
+        s = self._copy() if len(bs) <= len(self) else bs._copy()
         if len(bs) <= len(self):
-            s = self._copy()
             s._addright(bs)
         else:
-            s = bs._copy()
-            s = self.__class__(s)
             s._addleft(self)
         return s
 
     def __radd__(self: TBits, bs: BitsType) -> TBits:
         """Append current bitstring to bs and return new bitstring.
 
         bs -- An object that can be 'auto' initialised as a bitstring that will be appended to.
@@ -238,17 +237,16 @@
         '0b011'
         >>> print(BitArray('0x00112233')[1:3:8])
         '0x1122'
 
         """
         if isinstance(key, numbers.Integral):
             return bool(self._bitstore.getindex(key))
-        x = self._bitstore.getslice_withstep(key)
-        bs = self.__class__()
-        bs._bitstore = x
+        bs = super().__new__(self.__class__)
+        bs._bitstore = self._bitstore.getslice_withstep(key)
         return bs
 
     def __len__(self) -> int:
         """Return the length of the bitstring in bits."""
         return self._getlength()
 
     def __bytes__(self) -> bytes:
@@ -276,45 +274,44 @@
             return '0x' + self.hex
         # Otherwise first we do as much as we can in hex
         # then add on 1, 2 or 3 bits on at the end
         bits_at_end = length % 4
         return ''.join(('0x', self[0:length - bits_at_end]._gethex(),
                         ', ', '0b', self[length - bits_at_end:]._getbin()))
 
-    def _repr(self, classname: str, length: int, filename: str, pos: int):
+    def _repr(self, classname: str, length: int, pos: int):
         pos_string = f', pos={pos}' if pos else ''
-        if filename:
-            return f"{classname}(filename={repr(filename)}, length={length}{pos_string})"
+        if hasattr(self, '_filename') and self._filename:
+            return f"{classname}(filename={self._filename!r}, length={length}{pos_string})"
         else:
             s = self.__str__()
             lengthstring = ''
             if s.endswith('...'):
                 lengthstring = f'  # length={length}'
             return f"{classname}('{s}'{pos_string}){lengthstring}"
 
     def __repr__(self) -> str:
         """Return representation that could be used to recreate the bitstring.
 
         If the returned string is too long it will be truncated. See __str__().
 
         """
-        return self._repr(self.__class__.__name__, len(self), self._bitstore.filename, 0)
+        return self._repr(self.__class__.__name__, len(self), 0)
 
     def __eq__(self, bs: Any, /) -> bool:
         """Return True if two bitstrings have the same binary representation.
 
         >>> BitArray('0b1110') == '0xe'
         True
 
         """
         try:
-            bs = Bits._create_from_bitstype(bs)
+            return self._bitstore == Bits._create_from_bitstype(bs)._bitstore
         except TypeError:
             return False
-        return self._bitstore == bs._bitstore
 
     def __ne__(self, bs: Any, /) -> bool:
         """Return False if two bitstrings have the same binary representation.
 
         >>> BitArray('0b111') == '0x7'
         False
 
@@ -493,42 +490,35 @@
         """Reset the bitstring to an empty state."""
         self._bitstore = BitStore()
 
     def _setauto_no_length_or_offset(self, s: BitsType, /) -> None:
         """Set bitstring from a bitstring, file, bool, array, iterable or string."""
         if isinstance(s, str):
             self._bitstore = bitstore_helpers.str_to_bitstore(s)
-            return
-        if isinstance(s, Bits):
+        elif isinstance(s, Bits):
             self._bitstore = s._bitstore.copy()
-            return
-        if isinstance(s, (bytes, bytearray, memoryview)):
-            self._bitstore = BitStore(frombytes=bytearray(s))
-            return
-        if isinstance(s, io.BytesIO):
-            self._bitstore = BitStore(frombytes=s.getvalue())
-            return
-        if isinstance(s, io.BufferedReader):
+        elif isinstance(s, (bytes, bytearray, memoryview)):
+            self._bitstore = BitStore.frombytes(bytearray(s))
+        elif isinstance(s, io.BytesIO):
+            self._bitstore = BitStore.frombytes(s.getvalue())
+        elif isinstance(s, io.BufferedReader):
             self._setfile(s.name)
-            return
-        if isinstance(s, bitarray.bitarray):
+        elif isinstance(s, bitarray.bitarray):
             self._bitstore = BitStore(s)
-            return
-        if isinstance(s, array.array):
-            self._bitstore = BitStore(frombytes=bytearray(s.tobytes()))
-            return
-        if isinstance(s, abc.Iterable):
+        elif isinstance(s, array.array):
+            self._bitstore = BitStore.frombytes(s.tobytes())
+        elif isinstance(s, abc.Iterable):
             # Evaluate each item as True or False and set bits to 1 or 0.
             self._setbin_unsafe(''.join(str(int(bool(x))) for x in s))
-            return
-        if isinstance(s, numbers.Integral):
+        elif isinstance(s, numbers.Integral):
             raise TypeError(f"It's no longer possible to auto initialise a bitstring from an integer."
                             f" Use '{self.__class__.__name__}({s})' instead of just '{s}' as this makes it "
                             f"clearer that a bitstring of {int(s)} zero bits will be created.")
-        raise TypeError(f"Cannot initialise bitstring from type '{type(s)}'.")
+        else:
+            raise TypeError(f"Cannot initialise bitstring from type '{type(s)}'.")
 
     def _setauto(self, s: BitsType, length: Optional[int], offset: Optional[int], /) -> None:
         """Set bitstring from a bitstring, file, bool, array, iterable or string."""
         # As s can be so many different things it's important to do the checks
         # in the correct order, as some types are also other allowed types.
         if offset is None and length is None:
             return self._setauto_no_length_or_offset(s)
@@ -538,15 +528,15 @@
         if isinstance(s, io.BytesIO):
             if length is None:
                 length = s.seek(0, 2) * 8 - offset
             byteoffset, offset = divmod(offset, 8)
             bytelength = (length + byteoffset * 8 + offset + 7) // 8 - byteoffset
             if length + byteoffset * 8 + offset > s.seek(0, 2) * 8:
                 raise bitstring.CreationError("BytesIO object is not long enough for specified length and offset.")
-            self._bitstore = BitStore(frombytes=s.getvalue()[byteoffset: byteoffset + bytelength]).getslice(
+            self._bitstore = BitStore.frombytes(s.getvalue()[byteoffset: byteoffset + bytelength]).getslice(
                 offset, offset + length)
             return
 
         if isinstance(s, io.BufferedReader):
             self._setfile(s.name, length, offset)
             return
 
@@ -558,18 +548,19 @@
     def _setfile(self, filename: str, length: Optional[int] = None, offset: Optional[int] = None) -> None:
         """Use file as source of bits."""
         with open(pathlib.Path(filename), 'rb') as source:
             if offset is None:
                 offset = 0
             m = mmap.mmap(source.fileno(), 0, access=mmap.ACCESS_READ)
             if offset == 0:
-                self._bitstore = BitStore(buffer=m, length=length, filename=source.name, immutable=True)
+                self._filename = source.name
+                self._bitstore = BitStore.frombuffer(m, length=length)
             else:
                 # If offset is given then always read into memory.
-                temp = BitStore(buffer=m, filename=source.name, immutable=True)
+                temp = BitStore.frombuffer(m)
                 if length is None:
                     if offset > len(temp):
                         raise bitstring.CreationError(f"The offset of {offset} bits is greater than the file length ({len(temp)} bits).")
                     self._bitstore = temp.getslice(offset, None)
                 else:
                     self._bitstore = temp.getslice(offset, offset + length)
                     if len(self) != length:
@@ -588,23 +579,44 @@
                     f"Offset of {offset} and length of {length} too large for bitarray of length {len(ba)}.")
             self._bitstore = BitStore(ba[offset: offset + length])
 
     def _setbits(self, bs: BitsType, length: None = None) -> None:
         bs = Bits._create_from_bitstype(bs)
         self._bitstore = bs._bitstore
 
-    def _sete5m2float(self, f: float) -> None:
-        self._bitstore = bitstore_helpers.e5m2float2bitstore(f)
+    def _setp3binary(self, f: float) -> None:
+        self._bitstore = bitstore_helpers.p3binary2bitstore(f)
+
+    def _setp4binary(self, f: float) -> None:
+        self._bitstore = bitstore_helpers.p4binary2bitstore(f)
+
+    def _sete4m3mxfp(self, f: float) -> None:
+        self._bitstore = bitstore_helpers.e4m3mxfp2bitstore(f)
+
+    def _sete5m2mxfp(self, f: float) -> None:
+        self._bitstore = bitstore_helpers.e5m2mxfp2bitstore(f)
+
+    def _sete3m2mxfp(self, f: float) -> None:
+        self._bitstore = bitstore_helpers.e3m2mxfp2bitstore(f)
+
+    def _sete2m3mxfp(self, f: float) -> None:
+        self._bitstore = bitstore_helpers.e2m3mxfp2bitstore(f)
+
+    def _sete2m1mxfp(self, f: float) -> None:
+        self._bitstore = bitstore_helpers.e2m1mxfp2bitstore(f)
 
-    def _sete4m3float(self, f: float) -> None:
-        self._bitstore = bitstore_helpers.e4m3float2bitstore(f)
+    def _sete8m0mxfp(self, f: float) -> None:
+        self._bitstore = bitstore_helpers.e8m0mxfp2bitstore(f)
+
+    def _setmxint(self, f: float) -> None:
+        self._bitstore = bitstore_helpers.mxint2bitstore(f)
 
     def _setbytes(self, data: Union[bytearray, bytes], length:None = None) -> None:
         """Set the data from a bytes or bytearray object."""
-        self._bitstore = BitStore(frombytes=bytearray(data))
+        self._bitstore = BitStore.frombytes(data)
         return
 
     def _setbytes_with_truncation(self, data: Union[bytearray, bytes], length: Optional[int] = None, offset: Optional[int] = None) -> None:
         """Set the data from a bytes or bytearray object, with optional offset and length truncations."""
         if offset is None and length is None:
             return self._setbytes(data)
         data = bytearray(data)
@@ -612,15 +624,15 @@
             offset = 0
         if length is None:
             # Use to the end of the data
             length = len(data) * 8 - offset
         else:
             if length + offset > len(data) * 8:
                 raise bitstring.CreationError(f"Not enough data present. Need {length + offset} bits, have {len(data) * 8}.")
-        self._bitstore = BitStore(buffer=data).getslice_msb0(offset, offset + length)
+        self._bitstore = BitStore.frombytes(data).getslice_msb0(offset, offset + length)
 
     def _getbytes(self) -> bytes:
         """Return the data as an ordinary bytes object."""
         if len(self) % 8:
             raise bitstring.InterpretError("Cannot interpret as bytes unambiguously - not multiple of 8 bits.")
         return self._bitstore.tobytes()
 
@@ -637,142 +649,172 @@
     def _setuint(self, uint: int, length: Optional[int] = None) -> None:
         """Reset the bitstring to have given unsigned int interpretation."""
         # If no length given, and we've previously been given a length, use it.
         if length is None and hasattr(self, 'len') and len(self) != 0:
             length = len(self)
         if length is None or length == 0:
             raise bitstring.CreationError("A non-zero length must be specified with a uint initialiser.")
-        self._bitstore = bitstore_helpers.uint2bitstore(uint, length)
+        self._bitstore = bitstore_helpers.int2bitstore(uint, length, False)
 
     def _getuint(self) -> int:
         """Return data as an unsigned int."""
         if len(self) == 0:
             raise bitstring.InterpretError("Cannot interpret a zero length bitstring as an integer.")
         return self._bitstore.slice_to_uint()
 
     def _setint(self, int_: int, length: Optional[int] = None) -> None:
         """Reset the bitstring to have given signed int interpretation."""
         # If no length given, and we've previously been given a length, use it.
         if length is None and hasattr(self, 'len') and len(self) != 0:
             length = len(self)
         if length is None or length == 0:
             raise bitstring.CreationError("A non-zero length must be specified with an int initialiser.")
-        self._bitstore = bitstore_helpers.int2bitstore(int_, length)
+        self._bitstore = bitstore_helpers.int2bitstore(int_, length, True)
 
     def _getint(self) -> int:
         """Return data as a two's complement signed int."""
         if len(self) == 0:
             raise bitstring.InterpretError("Cannot interpret bitstring without a length as an integer.")
         return self._bitstore.slice_to_int()
 
     def _setuintbe(self, uintbe: int, length: Optional[int] = None) -> None:
         """Set the bitstring to a big-endian unsigned int interpretation."""
         if length is None and hasattr(self, 'len') and len(self) != 0:
             length = len(self)
         if length is None or length == 0:
             raise bitstring.CreationError("A non-zero length must be specified with a uintbe initialiser.")
-        self._bitstore = bitstore_helpers.uintbe2bitstore(uintbe, length)
+        self._bitstore = bitstore_helpers.int2bitstore(uintbe, length, False)
 
     def _getuintbe(self) -> int:
         """Return data as a big-endian two's complement unsigned int."""
         if len(self) % 8:
             raise bitstring.InterpretError(f"Big-endian integers must be whole-byte. Length = {len(self)} bits.")
         return self._getuint()
 
     def _setintbe(self, intbe: int, length: Optional[int] = None) -> None:
         """Set bitstring to a big-endian signed int interpretation."""
         if length is None and hasattr(self, 'len') and len(self) != 0:
             length = len(self)
         if length is None or length == 0:
             raise bitstring.CreationError("A non-zero length must be specified with a intbe initialiser.")
-        self._bitstore = bitstore_helpers.intbe2bitstore(intbe, length)
+        self._bitstore = bitstore_helpers.int2bitstore(intbe, length, True)
 
     def _getintbe(self) -> int:
         """Return data as a big-endian two's complement signed int."""
         if len(self) % 8:
             raise bitstring.InterpretError(f"Big-endian integers must be whole-byte. Length = {len(self)} bits.")
         return self._getint()
 
     def _setuintle(self, uintle: int, length: Optional[int] = None) -> None:
         if length is None and hasattr(self, 'len') and len(self) != 0:
             length = len(self)
         if length is None or length == 0:
             raise bitstring.CreationError("A non-zero length must be specified with a uintle initialiser.")
-        self._bitstore = bitstore_helpers.uintle2bitstore(uintle, length)
+        self._bitstore = bitstore_helpers.intle2bitstore(uintle, length, False)
 
     def _getuintle(self) -> int:
         """Interpret as a little-endian unsigned int."""
         if len(self) % 8:
             raise bitstring.InterpretError(f"Little-endian integers must be whole-byte. Length = {len(self)} bits.")
-        bs = BitStore(frombytes=self._bitstore.tobytes()[::-1])
+        bs = BitStore.frombytes(self._bitstore.tobytes()[::-1])
         return bs.slice_to_uint()
 
     def _setintle(self, intle: int, length: Optional[int] = None) -> None:
         if length is None and hasattr(self, 'len') and len(self) != 0:
             length = len(self)
         if length is None or length == 0:
             raise bitstring.CreationError("A non-zero length must be specified with an intle initialiser.")
-        self._bitstore = bitstore_helpers.intle2bitstore(intle, length)
+        self._bitstore = bitstore_helpers.intle2bitstore(intle, length, True)
 
     def _getintle(self) -> int:
         """Interpret as a little-endian signed int."""
         if len(self) % 8:
             raise bitstring.InterpretError(f"Little-endian integers must be whole-byte. Length = {len(self)} bits.")
-        bs = BitStore(frombytes=self._bitstore.tobytes()[::-1])
+        bs = BitStore.frombytes(self._bitstore.tobytes()[::-1])
         return bs.slice_to_int()
 
-    def _gete4m3float(self) -> float:
+    def _getp4binary(self) -> float:
         u = self._getuint()
-        return e4m3float_fmt.lut_int8_to_float[u]
+        return p4binary_fmt.lut_binary8_to_float[u]
 
-    def _gete5m2float(self) -> float:
+    def _getp3binary(self) -> float:
         u = self._getuint()
-        return e5m2float_fmt.lut_int8_to_float[u]
+        return p3binary_fmt.lut_binary8_to_float[u]
 
-    def _setfloatbe(self, f: float, length: Optional[int] = None) -> None:
+    def _gete4m3mxfp(self) -> float:
+        u = self._getuint()
+        return e4m3mxfp_saturate_fmt.lut_int_to_float[u]
+
+    def _gete5m2mxfp(self) -> float:
+        u = self._getuint()
+        return e5m2mxfp_saturate_fmt.lut_int_to_float[u]
+
+    def _gete3m2mxfp(self) -> float:
+        u = self._getuint()
+        return e3m2mxfp_fmt.lut_int_to_float[u]
+
+    def _gete2m3mxfp(self) -> float:
+        u = self._getuint()
+        return e2m3mxfp_fmt.lut_int_to_float[u]
+
+    def _gete2m1mxfp(self) -> float:
+        u = self._getuint()
+        return e2m1mxfp_fmt.lut_int_to_float[u]
+
+    def _gete8m0mxfp(self) -> float:
+        u = self._getuint() - 127
+        if u == 128:
+            return float('nan')
+        return 2.0 ** u
+
+    def _getmxint(self) -> float:
+        u = self._getint()
+        return float(u) * 2 ** -6
+
+
+    def _setfloat(self, f: float, length: Optional[int], big_endian: bool) -> None:
         if length is None and hasattr(self, 'len') and len(self) != 0:
             length = len(self)
         if length is None or length not in [16, 32, 64]:
             raise bitstring.CreationError("A length of 16, 32, or 64 must be specified with a float initialiser.")
-        self._bitstore = bitstore_helpers.float2bitstore(f, length)
+        self._bitstore = bitstore_helpers.float2bitstore(f, length, big_endian)
+
+    def _setfloatbe(self, f: float, length: Optional[int] = None) -> None:
+        self._setfloat(f, length, True)
 
     def _getfloatbe(self) -> float:
         """Interpret the whole bitstring as a big-endian float."""
         fmt = {16: '>e', 32: '>f', 64: '>d'}[len(self)]
         return struct.unpack(fmt, self._bitstore.tobytes())[0]
 
     def _setfloatle(self, f: float, length: Optional[int] = None) -> None:
-        if length is None and hasattr(self, 'len') and len(self) != 0:
-            length = len(self)
-        if length is None or length not in [16, 32, 64]:
-            raise bitstring.CreationError("A length of 16, 32, or 64 must be specified with a float initialiser.")
-        self._bitstore = bitstore_helpers.floatle2bitstore(f, length)
+        self._setfloat(f, length, False)
 
     def _getfloatle(self) -> float:
         """Interpret the whole bitstring as a little-endian float."""
         fmt = {16: '<e', 32: '<f', 64: '<d'}[len(self)]
         return struct.unpack(fmt, self._bitstore.tobytes())[0]
 
     def _getbfloatbe(self) -> float:
         zero_padded = self + Bits(16)
         return zero_padded._getfloatbe()
 
     def _setbfloatbe(self, f: Union[float, str], length: Optional[int] = None) -> None:
         if length is not None and length != 16:
             raise bitstring.CreationError(f"bfloats must be length 16, received a length of {length} bits.")
-        self._bitstore = bitstore_helpers.bfloat2bitstore(f)
+        self._bitstore = bitstore_helpers.bfloat2bitstore(f, True)
 
     def _getbfloatle(self) -> float:
         zero_padded = Bits(16) + self
         return zero_padded._getfloatle()
 
     def _setbfloatle(self, f: Union[float, str], length: Optional[int] = None) -> None:
         if length is not None and length != 16:
             raise bitstring.CreationError(f"bfloats must be length 16, received a length of {length} bits.")
-        self._bitstore = bitstore_helpers.bfloatle2bitstore(f)
+        self._bitstore = bitstore_helpers.bfloat2bitstore(f, False)
 
     def _setue(self, i: int) -> None:
         """Initialise bitstring with unsigned exponential-Golomb code for integer i.
 
         Raises CreationError if i < 0.
 
         """
@@ -783,15 +825,14 @@
     def _readue(self, pos: int) -> Tuple[int, int]:
         """Return interpretation of next bits as unsigned exponential-Golomb code.
 
         Raises ReadError if the end of the bitstring is encountered while
         reading the code.
 
         """
-        # _length is ignored - it's only present to make the function signature consistent.
         if bitstring.options.lsb0:
             raise bitstring.ReadError("Exp-Golomb codes cannot be read in lsb0 mode.")
         oldpos = pos
         try:
             while not self[pos]:
                 pos += 1
         except IndexError:
@@ -845,18 +886,15 @@
 
         Raises ReadError if the end of the bitstring is encountered while
         reading the code.
 
         """
         codenum, pos = self._readue(pos)
         m = (codenum + 1) // 2
-        if not codenum % 2:
-            return -m, pos
-        else:
-            return m, pos
+        return (m, pos) if codenum % 2 else (-m, pos)
 
     def _setuie(self, i: int) -> None:
         """Initialise bitstring with unsigned interleaved exponential-Golomb code for integer i.
 
         Raises CreationError if i < 0.
 
         """
@@ -879,16 +917,15 @@
                 pos += 1
                 codenum <<= 1
                 codenum += self[pos]
                 pos += 1
             pos += 1
         except IndexError:
             raise bitstring.ReadError("Read off end of bitstring trying to read code.")
-        codenum -= 1
-        return codenum, pos
+        return codenum - 1, pos
 
     def _setsie(self, i: int, ) -> None:
         """Initialise bitstring with signed interleaved exponential-Golomb code for integer i."""
         if bitstring.options.lsb0:
             raise bitstring.CreationError("Exp-Golomb codes cannot be used in lsb0 mode.")
         self._bitstore = bitstore_helpers.sie2bitstore(i)
 
@@ -901,18 +938,15 @@
         reading the code.
 
         """
         codenum, pos = self._readuie(pos)
         if not codenum:
             return 0, pos
         try:
-            if self[pos]:
-                return -codenum, pos + 1
-            else:
-                return codenum, pos + 1
+            return (-codenum, pos + 1) if self[pos] else (codenum, pos + 1)
         except IndexError:
             raise bitstring.ReadError("Read off end of bitstring trying to read code.")
 
     def _setbool(self, value: Union[bool, str]) -> None:
         # We deliberately don't want to have implicit conversions to bool here.
         # If we did then it would be difficult to deal with the 'False' string.
         if value in (1, 'True', '1'):
@@ -1062,15 +1096,15 @@
         assert pos + bits <= len(self), f"pos={pos}, bits={bits}, len={len(self)}"
         del self._bitstore[pos: pos + bits]
         return
 
     def _reversebytes(self, start: int, end: int) -> None:
         """Reverse bytes in-place."""
         assert (end - start) % 8 == 0
-        self._bitstore[start:end] = BitStore(frombytes=self._bitstore.getslice(start, end).tobytes()[::-1])
+        self._bitstore[start:end] = BitStore.frombytes(self._bitstore.getslice(start, end).tobytes()[::-1])
 
     def _invert(self, pos: int, /) -> None:
         """Flip bit at pos 1<->0."""
         assert 0 <= pos < len(self)
         self._bitstore.invert(pos)
 
     def _invert_all(self) -> None:
@@ -1090,44 +1124,34 @@
         self._addleft(Bits(n))
         self._truncateright(n)
         return self
 
     def _imul(self: TBits, n: int, /) -> TBits:
         """Concatenate n copies of self in place. Return self."""
         assert n >= 0
-        if not n:
+        if n == 0:
             self._clear()
-            return self
-        m: int = 1
-        old_len: int = len(self)
-        while m * 2 < n:
-            self._addright(self)
-            m *= 2
-        self._addright(self[0:(n - m) * old_len])
+        else:
+            m = 1
+            old_len = len(self)
+            while m * 2 < n:
+                self._addright(self)
+                m *= 2
+            self._addright(self[0:(n - m) * old_len])
         return self
 
     def _getbits(self: TBits):
         return self._copy()
 
     def _validate_slice(self, start: Optional[int], end: Optional[int]) -> Tuple[int, int]:
         """Validate start and end and return them as positive bit positions."""
-        if start is None:
-            start = 0
-        elif start < 0:
-            start += len(self)
-        if end is None:
-            end = len(self)
-        elif end < 0:
-            end += len(self)
-        if not 0 <= end <= len(self):
-            raise ValueError("end is not a valid position in the bitstring.")
-        if not 0 <= start <= len(self):
-            raise ValueError("start is not a valid position in the bitstring.")
-        if end < start:
-            raise ValueError("end must not be less than start.")
+        start = 0 if start is None else (start + len(self) if start < 0 else start)
+        end = len(self) if end is None else (end + len(self) if end < 0 else end)
+        if not 0 <= start <= end <= len(self):
+            raise ValueError(f"Invalid slice positions for bitstring length {len(self)}: start={start}, end={end}.")
         return start, end
 
     def unpack(self, fmt: Union[str, List[Union[str, int]]], **kwargs) -> List[Union[int, float, str, Bits, bool, bytes, None]]:
         """Interpret the whole bitstring using fmt and return list.
 
         fmt -- A single string or a list of strings with comma separated tokens
                describing how to interpret the bits in the bitstring. Items
@@ -1198,15 +1222,15 @@
                 pos += dtype.bitlength
             else:
                 val, pos = dtype.read_fn(self, pos)
             if val is not None:  # Don't append pad tokens
                 vals.append(val)
         return vals, pos
 
-    def find(self, bs: BitsType, start: Optional[int] = None, end: Optional[int] = None,
+    def find(self, bs: BitsType, /, start: Optional[int] = None, end: Optional[int] = None,
              bytealigned: Optional[bool] = None) -> Union[Tuple[int], Tuple[()]]:
         """Find first occurrence of substring bs.
 
         Returns a single item tuple with the bit position if found, or an
         empty tuple if not found. The bit position (pos property) will
         also be set to the start of the substring if it is found.
 
@@ -1314,15 +1338,15 @@
                 if not bytealigned or lsb0_pos % 8 == 0:
                     yield lsb0_pos
 
             pos = max(msb0_start, pos - increment)
             if pos == msb0_start:
                 return
 
-    def rfind(self, bs: BitsType, start: Optional[int] = None, end: Optional[int] = None,
+    def rfind(self, bs: BitsType, /, start: Optional[int] = None, end: Optional[int] = None,
               bytealigned: Optional[bool] = None) -> Union[Tuple[int], Tuple[()]]:
         """Find final occurrence of substring bs.
 
         Returns a single item tuple with the bit position if found, or an
         empty tuple if not found. The bit position (pos property) will
         also be set to the start of the substring if it is found.
 
@@ -1449,37 +1473,37 @@
 
         """
         s = self.__class__()
         if len(self) == 0:
             # Optimised version that doesn't need to add self between every item
             for item in sequence:
                 s._addright(Bits._create_from_bitstype(item))
+            return s
         else:
-            i = iter(sequence)
+            sequence_iter = iter(sequence)
             try:
-                s._addright(Bits._create_from_bitstype(next(i)))
-                while True:
-                    n = next(i)
-                    s._addright(self)
-                    s._addright(Bits._create_from_bitstype(n))
+                s._addright(Bits._create_from_bitstype(next(sequence_iter)))
             except StopIteration:
-                pass
-        return s
+                return s
+            for item in sequence_iter:
+                s._addright(self)
+                s._addright(Bits._create_from_bitstype(item))
+            return s
 
     def tobytes(self) -> bytes:
         """Return the bitstring as bytes, padding with zero bits if needed.
 
         Up to seven zero bits will be added at the end to byte align.
 
         """
         return self._bitstore.tobytes()
 
     def tobitarray(self) -> bitarray.bitarray:
         """Convert the bitstring to a bitarray object."""
-        if self._bitstore.modified:
+        if self._bitstore.modified_length is not None:
             # Removes the offset and truncates to length
             return self._bitstore.getslice(0, len(self))._bitarray
         else:
             return self._bitstore._bitarray
 
     def tofile(self, f: BinaryIO) -> None:
         """Write the bitstring to a file object, padding with zero bits if needed.
@@ -1498,81 +1522,59 @@
         prefix -- The bitstring to search for.
         start -- The bit position to start from. Defaults to 0.
         end -- The bit position to end at. Defaults to len(self).
 
         """
         prefix = self._create_from_bitstype(prefix)
         start, end = self._validate_slice(start, end)
-        if end < start + len(prefix):
-            return False
-        end = start + len(prefix)
-        return self._slice(start, end) == prefix
+        return self._slice(start, start + len(prefix)) == prefix if end >= start + len(prefix) else False
 
     def endswith(self, suffix: BitsType, start: Optional[int] = None, end: Optional[int] = None) -> bool:
         """Return whether the current bitstring ends with suffix.
 
         suffix -- The bitstring to search for.
         start -- The bit position to start from. Defaults to 0.
         end -- The bit position to end at. Defaults to len(self).
 
         """
         suffix = self._create_from_bitstype(suffix)
         start, end = self._validate_slice(start, end)
-        if start + len(suffix) > end:
-            return False
-        start = end - len(suffix)
-        return self._slice(start, end) == suffix
+        return self._slice(end - len(suffix), end) == suffix if start + len(suffix) <= end else False
 
     def all(self, value: Any, pos: Optional[Iterable[int]] = None) -> bool:
         """Return True if one or many bits are all set to bool(value).
 
         value -- If value is True then checks for bits set to 1, otherwise
                  checks for bits set to 0.
         pos -- An iterable of bit positions. Negative numbers are treated in
                the same way as slice indices. Defaults to the whole bitstring.
 
         """
-        value = bool(value)
-        length = len(self)
+        value = 1 if bool(value) else 0
         if pos is None:
-            if value is True:
-                return self._bitstore.all_set()
-            else:
-                return not self._bitstore.any_set()
+            return self._bitstore.all_set() if value else not self._bitstore.any_set()
         for p in pos:
-            if p < 0:
-                p += length
-            if not 0 <= p < length:
-                raise IndexError(f"Bit position {p} out of range.")
-            if not bool(self._bitstore.getindex(p)) is value:
+            if self._bitstore.getindex(p) != value:
                 return False
         return True
 
     def any(self, value: Any, pos: Optional[Iterable[int]] = None) -> bool:
         """Return True if any of one or many bits are set to bool(value).
 
         value -- If value is True then checks for bits set to 1, otherwise
                  checks for bits set to 0.
         pos -- An iterable of bit positions. Negative numbers are treated in
                the same way as slice indices. Defaults to the whole bitstring.
 
         """
-        value = bool(value)
-        length = len(self)
+        value = 1 if bool(value) else 0
         if pos is None:
-            if value is True:
-                return self._bitstore.any_set()
-            else:
-                return not self._bitstore.all_set()
+            return self._bitstore.any_set() if value else not self._bitstore.all_set()
         for p in pos:
-            if p < 0:
-                p += length
-            if not 0 <= p < length:
-                raise IndexError(f"Bit position {p} out of range.")
-            if bool(self._bitstore.getindex(p)) is value:
+            if self._bitstore.getindex(p) == value:
                 return True
         return False
 
     def count(self, value: Any) -> int:
         """Return count of total number of either zero or one bits.
 
         value -- If bool(value) is True then bits set to 1 are counted, otherwise bits set
@@ -1591,27 +1593,31 @@
         dtype = Dtype(fmt)
         bpc = Bits._bits_per_char(dtype.name)
         if dtype.bitlength is not None and dtype.bitlength % bpc != 0:
             raise ValueError(f"Bits per group must be a multiple of {bpc} for '{fmt}' format.")
         return dtype.name, dtype.bitlength
 
     @staticmethod
-    def _format_bits(bits: Bits, bits_per_group: int, sep: str, fmt: str,
+    def _format_bits(bits: Bits, bits_per_group: int, sep: str, dtype: Dtype,
                      colour_start: str, colour_end: str, width: Optional[int]=None) -> Tuple[str, int]:
-        get_fn = Bits._getbytes_printable if fmt == 'bytes' else dtype_register.get_dtype(fmt, bits_per_group).get_fn
+        get_fn = dtype.get_fn
+        if dtype.name == 'bytes':  # Special case for bytes to print one character each.
+            get_fn = Bits._getbytes_printable
+        if dtype.name == 'bool':  # Special case for bool to print '1' or '0' instead of `True` or `False`.
+            get_fn = dtype_register.get_dtype('uint', bits_per_group).get_fn
         if bits_per_group == 0:
             x = str(get_fn(bits))
         else:
             # Left-align for fixed width types when msb0, otherwise right-align.
-            align = '<' if fmt in ['bin', 'oct', 'hex', 'bits', 'bytes'] and not bitstring.options.lsb0 else '>'
-            if dtype_register[fmt].bitlength2chars_fn is not None:
-                chars_per_group = dtype_register[fmt].bitlength2chars_fn(bits_per_group)
-            else:
-                chars_per_group = 0
+            align = '<' if dtype.name in ['bin', 'oct', 'hex', 'bits', 'bytes'] and not bitstring.options.lsb0 else '>'
+            chars_per_group = 0
+            if dtype_register[dtype.name].bitlength2chars_fn is not None:
+                chars_per_group = dtype_register[dtype.name].bitlength2chars_fn(bits_per_group)
             x = sep.join(f"{str(get_fn(b)): {align}{chars_per_group}}" for b in bits.cut(bits_per_group))
+
         chars_used = len(x)
         padding_spaces = 0 if width is None else max(width - len(x), 0)
         x = colour_start + x + colour_end
         # Pad final line with spaces to align it
         if bitstring.options.lsb0:
             x = ' ' * padding_spaces + x
         else:
@@ -1631,21 +1637,21 @@
         if fmt not in ['bin', 'oct', 'hex', 'bytes']:
             raise ValueError
         return 24 // dtype_register[fmt].bitlength2chars_fn(24)
 
     def _pp(self, dtype1: Dtype, dtype2: Optional[Dtype], bits_per_group: int, width: int, sep: str, format_sep: str,
             show_offset: bool, stream: TextIO, lsb0: bool, offset_factor: int) -> None:
         """Internal pretty print method."""
-        colour = Colour(bitstring.options.colourful_prettyprinting)
+        colour = Colour(not bitstring.options.no_color)
         name1 = dtype1.name
         name2 = dtype2.name if dtype2 is not None else None
         if dtype1.variable_length:
             raise ValueError(f"Can't use Dtype '{dtype1}' in pp() as it has a variable length.")
         if dtype2 is not None and dtype2.variable_length:
-            raise ValueError(f"Can't use Dtype '{dtype1}' in pp() as it has a variable length.")
+            raise ValueError(f"Can't use Dtype '{dtype2}' in pp() as it has a variable length.")
         offset_width = 0
         offset_sep = ' :' if lsb0 else ': '
         if show_offset:
             # This could be 1 too large in some circumstances. Slightly recurrent logic needed to fix it...
             offset_width = len(str(len(self))) + len(offset_sep)
         if bits_per_group > 0:
             group_chars1 = Bits._chars_per_group(bits_per_group, name1)
@@ -1678,32 +1684,64 @@
                 offset = bitpos // offset_factor
                 bitpos += len(bits)
                 if bitstring.options.lsb0:
                     offset_str = colour.green + offset_sep + f'{offset: <{offset_width - len(offset_sep)}}' + colour.off
                 else:
                     offset_str = colour.green + f'{offset: >{offset_width - len(offset_sep)}}' + offset_sep + colour.off
 
-            fb1, chars_used = Bits._format_bits(bits, bits_per_group, sep, name1, colour.purple, colour.off, first_fb_width)
+            fb1, chars_used = Bits._format_bits(bits, bits_per_group, sep, dtype1, colour.purple, colour.off, first_fb_width)
             if first_fb_width is None:
                 first_fb_width = chars_used
 
             fb2 = ''
-            if name2 is not None:
-                fb2, chars_used = Bits._format_bits(bits, bits_per_group, sep, name2, colour.blue, colour.off, second_fb_width)
+            if dtype2 is not None:
+                fb2, chars_used = Bits._format_bits(bits, bits_per_group, sep, dtype2, colour.blue, colour.off, second_fb_width)
                 if second_fb_width is None:
                     second_fb_width = chars_used
                 fb2 = format_sep + fb2
 
             if bitstring.options.lsb0 is True:
                 line_fmt = fb1 + fb2 + offset_str + '\n'
             else:
                 line_fmt = offset_str + fb1 + fb2 + '\n'
             stream.write(line_fmt)
         return
 
+    @staticmethod
+    def _process_pp_tokens(token_list, fmt):
+        has_length_in_fmt = True
+        if len(token_list) == 1:
+            dtype1 = Dtype(*utils.parse_name_length_token(token_list[0]))
+            dtype2 = None
+            bits_per_group = dtype1.bitlength
+            if bits_per_group is None:
+                has_length_in_fmt = False
+                bits_per_group = {'bin': 8, 'hex': 8, 'oct': 12, 'bytes': 32}.get(dtype1.name)
+                if bits_per_group is None:
+                    raise ValueError(f"No length or default length available for pp() format '{fmt}'.")
+        elif len(token_list) == 2:
+            dtype1 = Dtype(*utils.parse_name_length_token(token_list[0]))
+            dtype2 = Dtype(*utils.parse_name_length_token(token_list[1]))
+            if dtype1.bitlength is not None and dtype2.bitlength is not None and dtype1.bitlength != dtype2.bitlength:
+                raise ValueError(
+                    f"Differing bit lengths of {dtype1.bitlength} and {dtype2.bitlength} in format string '{fmt}'.")
+            bits_per_group = dtype1.bitlength if dtype1.bitlength is not None else dtype2.bitlength
+            if bits_per_group is None:
+                has_length_in_fmt = False
+                try:
+                    bits_per_group = 2 * Bits._bits_per_char(dtype1.name) * Bits._bits_per_char(dtype2.name)
+                except ValueError:
+                    raise ValueError(f"Can't find a default bitlength to use for pp() format '{fmt}'.")
+                if bits_per_group >= 24:
+                    bits_per_group //= 2
+        else:
+            raise ValueError(
+                f"Only one or two tokens can be used in an pp() format - '{fmt}' has {len(token_list)} tokens.")
+        return dtype1, dtype2, bits_per_group, has_length_in_fmt
+
     def pp(self, fmt: Optional[str] = None, width: int = 120, sep: str = ' ',
            show_offset: bool = True, stream: TextIO = sys.stdout) -> None:
         """Pretty print the bitstring's value.
 
         fmt -- Printed data format. One or two of 'bin', 'oct', 'hex' or 'bytes'.
               The number of bits represented in each printed group defaults to 8 for hex and bin,
               12 for oct and 32 for bytes. This can be overridden with an explicit length, e.g. 'hex:64'.
@@ -1714,57 +1752,20 @@
         show_offset -- If True (the default) shows the bit offset in the first column of each line.
         stream -- A TextIO object with a write() method. Defaults to sys.stdout.
 
         >>> s.pp('hex16')
         >>> s.pp('b, h', sep='_', show_offset=False)
 
         """
-        colour = Colour(bitstring.options.colourful_prettyprinting)
+        colour = Colour(not bitstring.options.no_color)
         if fmt is None:
-            if len(self) % 8 == 0 and len(self) >= 8:
-                fmt = 'bin, hex'
-            else:
-                fmt = 'bin'
+            fmt = 'bin, hex' if len(self) % 8 == 0 and len(self) >= 8 else 'bin'
         token_list = utils.preprocess_tokens(fmt)
-        if len(token_list) not in [1, 2]:
-            raise ValueError(f"Only one or two tokens can be used in an pp() format - '{fmt}' has {len(token_list)} tokens.")
-        dtype1 = Dtype(*utils.parse_name_length_token(token_list[0]))
-        dtype2 = None
-        has_length_in_fmt = True
-        if len(token_list) == 1:
-            bits_per_group = dtype1.bitlength
-            if bits_per_group is None:
-                has_length_in_fmt = False
-                if dtype1.name in ['bin', 'hex']:
-                    bits_per_group = 8
-                elif dtype1.name == 'oct':
-                    bits_per_group = 12
-                elif dtype1.name == 'bytes':
-                    bits_per_group = 32
-                else:
-                    raise ValueError(f"No length or default length available for pp() format '{fmt}'.")
-        else:
-            dtype2 = Dtype(*utils.parse_name_length_token(token_list[1]))
-            if dtype1.bitlength is not None and dtype2.bitlength is not None and dtype1.bitlength != dtype2.bitlength:
-                raise ValueError(
-                    f"Differing bit lengths of {dtype1.bitlength} and {dtype2.bitlength} in format string '{fmt}'.")
-            bits_per_group = dtype1.bitlength if dtype1.bitlength is not None else dtype2.bitlength
-            if bits_per_group is None:
-                has_length_in_fmt = False
-                # Rule of thumb seems to work OK for all combinations.
-                try:
-                    bits_per_group = 2 * self._bits_per_char(dtype1.name) * self._bits_per_char(dtype2.name)
-                except ValueError:
-                    raise ValueError(f"Can't find a default bitlength to use for pp() format '{fmt}'.")
-                if bits_per_group >= 24:
-                    bits_per_group //= 2
-
-        trailing_bit_length = 0
-        if has_length_in_fmt and bits_per_group != 0:
-            trailing_bit_length = len(self) % bits_per_group
+        dtype1, dtype2, bits_per_group, has_length_in_fmt = Bits._process_pp_tokens(token_list, fmt)
+        trailing_bit_length = len(self) % bits_per_group if has_length_in_fmt and bits_per_group else 0
         data = self if trailing_bit_length == 0 else self[0: -trailing_bit_length]
         format_sep = " : "  # String to insert on each line between multiple formats
         tidy_fmt = colour.purple + str(dtype1) + colour.off
         if dtype2 is not None:
             tidy_fmt += ', ' + colour.blue + str(dtype2) + colour.off
         output_stream = io.StringIO()
         len_str = colour.green + str(len(self)) + colour.off
@@ -1780,10 +1781,17 @@
 
     def copy(self: TBits) -> TBits:
         """Return a copy of the bitstring."""
         # Note that if you want a new copy (different ID), use _copy instead.
         # The copy can return self as it's immutable.
         return self
 
+    @classmethod
+    def fromstring(cls: TBits, s: str, /) -> TBits:
+        """Create a new bitstring from a formatted string."""
+        x = super().__new__(cls)
+        x._bitstore = bitstore_helpers.str_to_bitstore(s)
+        return x
+
     len = length = property(_getlength, doc="The length of the bitstring in bits. Read only.")
```

### Comparing `bitstring-4.2.0b1/bitstring/bitstore.py` & `bitstring-4.2.0b2/bitstring/bitstore.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,49 +18,56 @@
     # First convert slice to all integers
     # Length already should take account of the offset
     start, stop, _ = slice(start, stop, None).indices(length)
     new_start = length - stop
     new_stop = length - start
     return new_start, new_stop
 
+
 class BitStore:
     """A light wrapper around bitarray that does the LSB0 stuff"""
 
-    __slots__ = ('_bitarray', 'modified', 'length', 'filename', 'immutable')
+    __slots__ = ('_bitarray', 'modified_length', 'immutable')
 
-    def __init__(self, initializer: Union[int, bitarray.bitarray, str, None] = None, buffer=None, immutable: bool = False,
-                 frombytes: Optional[Union[bytes, bytearray]] = None, filename: str = '', length: Optional[int] = None) -> None:
-        if buffer is None:
-            self._bitarray = bitarray.bitarray(initializer)
-        else:
-            self._bitarray = bitarray.bitarray(buffer=buffer)
-        if frombytes is not None:
-            self._bitarray = bitarray.bitarray()
-            self._bitarray.frombytes(frombytes)
+    def __init__(self, initializer: Union[int, bitarray.bitarray, str, None] = None,
+                 immutable: bool = False) -> None:
+        self._bitarray = bitarray.bitarray(initializer)
         self.immutable = immutable
-        self.length = None
-        self.filename = filename
-        # Here 'modified' means that it isn't just the underlying bitarray. It could have a different start and end, and be from a file.
-        # This also means that it shouldn't be changed further, so setting deleting etc. are disallowed.
-        self.modified = length is not None or filename != ''
-        if self.modified:
-            assert immutable is True
-
-            self.length = len(self._bitarray) if length is None else length
+        self.modified_length = None
 
-            if self.length < 0:
+    @classmethod
+    def frombytes(cls, b: Union[bytes, bytearray, memoryview], /) -> BitStore:
+        x = super().__new__(cls)
+        x._bitarray = bitarray.bitarray()
+        x._bitarray.frombytes(b)
+        x.immutable = False
+        x.modified_length = None
+        return x
+
+    @classmethod
+    def frombuffer(cls, buffer, /, length: Optional[int] = None) -> BitStore:
+        x = super().__new__(cls)
+        x._bitarray = bitarray.bitarray(buffer=buffer)
+        x.immutable = True
+        x.modified_length = length
+        # Here 'modified' means it shouldn't be changed further, so setting, deleting etc. are disallowed.
+        if x.modified_length is not None:
+            if x.modified_length < 0:
                 raise CreationError("Can't create bitstring with a negative length.")
-            if self.length > len(self._bitarray):
+            if x.modified_length > len(x._bitarray):
                 raise CreationError(
-                    f"Can't create bitstring with a length of {self.length} from {len(self._bitarray)} bits of data.")
+                    f"Can't create bitstring with a length of {x.modified_length} from {len(x._bitarray)} bits of data.")
+        return x
 
     def setall(self, value: int, /) -> None:
         self._bitarray.setall(value)
 
     def tobytes(self) -> bytes:
+        if self.modified_length is not None:
+            return self._bitarray[:self.modified_length].tobytes()
         return self._bitarray.tobytes()
 
     def slice_to_uint(self, start: Optional[int] = None, end: Optional[int] = None) -> int:
         return bitarray.util.ba2int(self.getslice(start, end)._bitarray, signed=False)
 
     def slice_to_int(self, start: Optional[int] = None, end: Optional[int] = None) -> int:
         return bitarray.util.ba2int(self.getslice(start, end)._bitarray, signed=True)
@@ -167,25 +174,25 @@
         # Use getindex or getslice instead
         raise NotImplementedError
 
     def getindex_msb0(self, index: int, /) -> bool:
         return bool(self._bitarray.__getitem__(index))
 
     def getslice_withstep_msb0(self, key: slice, /) -> BitStore:
-        if self.modified:
-            key = slice(*key.indices(len(self)))
+        if self.modified_length is not None:
+            key = slice(*key.indices(self.modified_length))
         return BitStore(self._bitarray.__getitem__(key))
 
     def getslice_withstep_lsb0(self, key: slice, /) -> BitStore:
         key = offset_slice_indices_lsb0(key, len(self))
         return BitStore(self._bitarray.__getitem__(key))
 
     def getslice_msb0(self, start: Optional[int], stop: Optional[int], /) -> BitStore:
-        if self.modified:
-            key = slice(*slice(start, stop, None).indices(len(self)))
+        if self.modified_length is not None:
+            key = slice(*slice(start, stop, None).indices(self.modified_length))
             start = key.start
             stop = key.stop
         return BitStore(self._bitarray[start:stop])
 
     def getslice_lsb0(self, start: Optional[int], stop: Optional[int], /) -> BitStore:
         start, stop = offset_start_stop_lsb0(start, stop, len(self))
         return BitStore(self._bitarray[start:stop])
@@ -231,15 +238,15 @@
     def any_set(self) -> bool:
         return self._bitarray.any()
 
     def all_set(self) -> bool:
         return self._bitarray.all()
 
     def __len__(self) -> int:
-        return self.length if self.length is not None else len(self._bitarray)
+        return self.modified_length if self.modified_length is not None else len(self._bitarray)
 
     def setitem_msb0(self, key, value, /):
         if isinstance(value, BitStore):
             self._bitarray.__setitem__(key, value._bitarray)
         else:
             self._bitarray.__setitem__(key, value)
```

### Comparing `bitstring-4.2.0b1/bitstring/bitstore_helpers.py` & `bitstring-4.2.0b2/bitstring/bitstore_helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from __future__ import annotations
 
-import sys
 import struct
+import math
 import functools
 from typing import Union, Optional, Dict, Callable
 import bitarray
 from bitstring.bitstore import BitStore
 import bitstring
-from bitstring.fp8 import e4m3float_fmt, e5m2float_fmt
-
-
-byteorder: str = sys.byteorder
+from bitstring.fp8 import p4binary_fmt, p3binary_fmt
+from bitstring.mxfp import e3m2mxfp_fmt, e2m3mxfp_fmt, e2m1mxfp_fmt, e4m3mxfp_saturate_fmt, e5m2mxfp_saturate_fmt, e4m3mxfp_overflow_fmt, e5m2mxfp_overflow_fmt
 
 # The size of various caches used to improve performance
 CACHE_SIZE = 256
 
 
 def tidy_input_string(s: str) -> str:
     """Return string made lowercase and with all whitespace and underscores removed."""
@@ -23,38 +21,35 @@
     except (AttributeError, TypeError):
         raise ValueError(f"Expected str object but received a {type(s)} with value {s}.")
     return ''.join(t).lower().replace('_', '')
 
 
 @functools.lru_cache(CACHE_SIZE)
 def str_to_bitstore(s: str) -> BitStore:
-    try:
-        _, tokens = bitstring.utils.tokenparser(s)
-    except ValueError as e:
-        raise bitstring.CreationError(*e.args)
+    _, tokens = bitstring.utils.tokenparser(s)
     bs = BitStore()
     for token in tokens:
         bs += bitstore_from_token(*token)
     bs.immutable = True
     return bs
 
 
 def bin2bitstore(binstring: str) -> BitStore:
     binstring = tidy_input_string(binstring)
     binstring = binstring.replace('0b', '')
-    return bin2bitstore_unsafe(binstring)
-
-
-def bin2bitstore_unsafe(binstring: str) -> BitStore:
     try:
         return BitStore(binstring)
     except ValueError:
         raise bitstring.CreationError(f"Invalid character in bin initialiser {binstring}.")
 
 
+def bin2bitstore_unsafe(binstring: str) -> BitStore:
+    return BitStore(binstring)
+
+
 def hex2bitstore(hexstring: str) -> BitStore:
     hexstring = tidy_input_string(hexstring)
     hexstring = hexstring.replace('0x', '')
     try:
         ba = bitarray.util.hex2ba(hexstring)
     except ValueError:
         raise bitstring.CreationError("Invalid symbol in hex initialiser.")
@@ -79,15 +74,15 @@
         return BitStore('1')
     tmp = i + 1
     leadingzeros = -1
     while tmp > 0:
         tmp >>= 1
         leadingzeros += 1
     remainingpart = i + 1 - (1 << leadingzeros)
-    return BitStore('0' * leadingzeros + '1') + uint2bitstore(remainingpart, leadingzeros)
+    return BitStore('0' * leadingzeros + '1') + int2bitstore(remainingpart, leadingzeros, False)
 
 
 def se2bitstore(i: Union[str, int]) -> BitStore:
     i = int(i)
     if i > 0:
         u = (i * 2) - 1
     else:
@@ -106,147 +101,160 @@
     i = int(i)
     if i == 0:
         return BitStore('1')
     else:
         return uie2bitstore(abs(i)) + (BitStore('1') if i < 0 else BitStore('0'))
 
 
-def bfloat2bitstore(f: Union[str, float]) -> BitStore:
+def bfloat2bitstore(f: Union[str, float], big_endian: bool) -> BitStore:
     f = float(f)
+    fmt = '>f' if big_endian else '<f'
     try:
-        b = struct.pack('>f', f)
+        b = struct.pack(fmt, f)
     except OverflowError:
         # For consistency we overflow to 'inf'.
-        b = struct.pack('>f', float('inf') if f > 0 else float('-inf'))
-    return BitStore(frombytes=b[0:2])
+        b = struct.pack(fmt, float('inf') if f > 0 else float('-inf'))
+    return BitStore.frombytes(b[0:2]) if big_endian else BitStore.frombytes(b[2:4])
 
 
-def bfloatle2bitstore(f: Union[str, float]) -> BitStore:
+def p4binary2bitstore(f: Union[str, float]) -> BitStore:
     f = float(f)
-    try:
-        b = struct.pack('<f', f)
-    except OverflowError:
-        # For consistency we overflow to 'inf'.
-        b = struct.pack('<f', float('inf') if f > 0 else float('-inf'))
-    return BitStore(frombytes=b[2:4])
+    u = p4binary_fmt.float_to_int8(f)
+    return int2bitstore(u, 8, False)
 
+def p3binary2bitstore(f: Union[str, float]) -> BitStore:
+    f = float(f)
+    u = p3binary_fmt.float_to_int8(f)
+    return int2bitstore(u, 8, False)
 
-def e4m3float2bitstore(f: Union[str, float]) -> BitStore:
+def e4m3mxfp2bitstore(f: Union[str, float]) -> BitStore:
     f = float(f)
-    u = e4m3float_fmt.float_to_int8(f)
-    return uint2bitstore(u, 8)
+    if bitstring.options.mxfp_overflow == 'saturate':
+        u = e4m3mxfp_saturate_fmt.float_to_int(f)
+    else:
+        u = e4m3mxfp_overflow_fmt.float_to_int(f)
+    return int2bitstore(u, 8, False)
 
+def e5m2mxfp2bitstore(f: Union[str, float]) -> BitStore:
+    f = float(f)
+    if bitstring.options.mxfp_overflow == 'saturate':
+        u = e5m2mxfp_saturate_fmt.float_to_int(f)
+    else:
+        u = e5m2mxfp_overflow_fmt.float_to_int(f)
+    return int2bitstore(u, 8, False)
 
-def e5m2float2bitstore(f: Union[str, float]) -> BitStore:
+def e3m2mxfp2bitstore(f: Union[str, float]) -> BitStore:
     f = float(f)
-    u = e5m2float_fmt.float_to_int8(f)
-    return uint2bitstore(u, 8)
+    if math.isnan(f):
+        raise ValueError("Cannot convert float('nan') to e3m2mxfp format as it has no representation for it.")
+    u = e3m2mxfp_fmt.float_to_int(f)
+    return int2bitstore(u, 6, False)
 
+def e2m3mxfp2bitstore(f: Union[str, float]) -> BitStore:
+    f = float(f)
+    if math.isnan(f):
+        raise ValueError("Cannot convert float('nan') to e2m3mxfp format as it has no representation for it.")
+    u = e2m3mxfp_fmt.float_to_int(f)
+    return int2bitstore(u, 6, False)
 
-def uint2bitstore(uint: Union[str, int], length: int) -> BitStore:
-    uint = int(uint)
+def e2m1mxfp2bitstore(f: Union[str, float]) -> BitStore:
+    f = float(f)
+    if math.isnan(f):
+        raise ValueError("Cannot convert float('nan') to e2m1mxfp format as it has no representation for it.")
+    u = e2m1mxfp_fmt.float_to_int(f)
+    return int2bitstore(u, 4, False)
+
+
+e8m0mxfp_allowed_values = [float(2 ** x) for x in range(-127, 128)]
+def e8m0mxfp2bitstore(f: Union[str, float]) -> BitStore:
+    f = float(f)
+    if math.isnan(f):
+        return BitStore('11111111')
     try:
-        x = BitStore(bitarray.util.int2ba(uint, length=length, endian='big', signed=False))
-    except OverflowError as e:
-        if uint >= (1 << length):
-            msg = f"{uint} is too large an unsigned integer for a bitstring of length {length}. " \
-                  f"The allowed range is [0, {(1 << length) - 1}]."
-            raise bitstring.CreationError(msg)
-        if uint < 0:
-            raise bitstring.CreationError("uint cannot be initialised with a negative number.")
-        raise e
-    return x
+        i = e8m0mxfp_allowed_values.index(f)
+    except ValueError:
+        raise ValueError(f"{f} is not a valid e8m0mxfp value. It must be exactly 2 ** i, for -127 <= i <= 127 or float('nan') as no rounding will be done.")
+    return int2bitstore(i, 8, False)
+
 
+def mxint2bitstore(f: Union[str, float]) -> BitStore:
+    f = float(f)
+    if math.isnan(f):
+        raise ValueError("Cannot convert float('nan') to mxint format as it has no representation for it.")
+    f *= 2 ** 6  # Remove the implicit scaling factor
+    if f > 127:  # 1 + 63/64
+        return BitStore('01111111')
+    if f <= -128:  # -2
+        return BitStore('10000000')
+    # Want to round to nearest, so move by 0.5 away from zero and round down by converting to int
+    if f >= 0.0:
+        f += 0.5
+        i = int(f)
+        # For ties-round-to-even
+        if f - i == 0.0 and i % 2:
+            i -= 1
+    else:
+        f -= 0.5
+        i = int(f)
+        if f - i == 0.0 and i % 2:
+            i += 1
+    return int2bitstore(i, 8, True)
 
-def int2bitstore(i: Union[str, int], length: int) -> BitStore:
+def int2bitstore(i: int, length: int, signed: bool) -> BitStore:
     i = int(i)
     try:
-        x = BitStore(bitarray.util.int2ba(i, length=length, endian='big', signed=True))
+        x = BitStore(bitarray.util.int2ba(i, length=length, endian='big', signed=signed))
     except OverflowError as e:
-        if i >= (1 << (length - 1)) or i < -(1 << (length - 1)):
-            raise bitstring.CreationError(f"{i} is too large a signed integer for a bitstring of length {length}. "
-                                f"The allowed range is [{-(1 << (length - 1))}, {(1 << (length - 1)) - 1}].")
+        if signed:
+            if i >= (1 << (length - 1)) or i < -(1 << (length - 1)):
+                raise bitstring.CreationError(f"{i} is too large a signed integer for a bitstring of length {length}. "
+                                    f"The allowed range is [{-(1 << (length - 1))}, {(1 << (length - 1)) - 1}].")
         else:
-            raise e
+            if i >= (1 << length):
+                raise bitstring.CreationError(f"{i} is too large an unsigned integer for a bitstring of length {length}. "
+                                    f"The allowed range is [0, {(1 << length) - 1}].")
+            if i < 0:
+                raise bitstring.CreationError("uint cannot be initialised with a negative number.")
+        raise e
     return x
 
 
-def uintbe2bitstore(i: Union[str, int], length: int) -> BitStore:
-    return uint2bitstore(i, length)
-
-
-def intbe2bitstore(i: int, length: int) -> BitStore:
-    return int2bitstore(i, length)
+def intle2bitstore(i: int, length: int, signed: bool) -> BitStore:
+    x = int2bitstore(i, length, signed).tobytes()
+    return BitStore.frombytes(x[::-1])
 
 
-def uintle2bitstore(i: int, length: int) -> BitStore:
-    x = uint2bitstore(i, length).tobytes()
-    return BitStore(frombytes=x[::-1])
-
-
-def intle2bitstore(i: int, length: int) -> BitStore:
-    x = int2bitstore(i, length).tobytes()
-    return BitStore(frombytes=x[::-1])
-
-
-def float2bitstore(f: Union[str, float], length: int) -> BitStore:
+def float2bitstore(f: Union[str, float], length: int, big_endian: bool) -> BitStore:
     f = float(f)
-    fmt = {16: '>e', 32: '>f', 64: '>d'}[length]
+    fmt = {16: '>e', 32: '>f', 64: '>d'}[length] if big_endian else {16: '<e', 32: '<f', 64: '<d'}[length]
     try:
         b = struct.pack(fmt, f)
-        assert len(b) * 8 == length
-    except (OverflowError, struct.error) as e:
-        # If float64 doesn't fit it automatically goes to 'inf'. This reproduces that behaviour for other types.
-        if length in [16, 32]:
-            b = struct.pack(fmt, float('inf') if f > 0 else float('-inf'))
-        else:
-            raise e
-    return BitStore(frombytes=b)
-
-
-def floatle2bitstore(f: Union[str, float], length: int) -> BitStore:
-    f = float(f)
-    fmt = {16: '<e', 32: '<f', 64: '<d'}[length]
-    try:
-        b = struct.pack(fmt, f)
-        assert len(b) * 8 == length
-    except (OverflowError, struct.error) as e:
+    except OverflowError:
         # If float64 doesn't fit it automatically goes to 'inf'. This reproduces that behaviour for other types.
-        if length in [16, 32]:
-            b = struct.pack(fmt, float('inf') if f > 0 else float('-inf'))
-        else:
-            raise e
-    return BitStore(frombytes=b)
-
-
-def bytes2bitstore(b: bytes, length: int) -> BitStore:
-    return BitStore(frombytes=b[:length])
+        b = struct.pack(fmt, float('inf') if f > 0 else float('-inf'))
+    return BitStore.frombytes(b)
 
 
 literal_bit_funcs: Dict[str, Callable[..., BitStore]] = {
     '0x': hex2bitstore,
     '0X': hex2bitstore,
     '0b': bin2bitstore,
     '0B': bin2bitstore,
     '0o': oct2bitstore,
     '0O': oct2bitstore,
 }
 
+
 def bitstore_from_token(name: str, token_length: Optional[int], value: Optional[str]) -> BitStore:
+    if name in literal_bit_funcs:
+        return literal_bit_funcs[name](value)
     try:
         d = bitstring.dtypes.Dtype(name, token_length)
     except ValueError as e:
-        if name in literal_bit_funcs:
-            bs = literal_bit_funcs[name](value)
-        else:
-            raise bitstring.CreationError(f"Can't parse token: {e}")
-    else:
-        b = bitstring.bits.Bits()
-        if value is None and name != 'pad':
-            # 'pad' is a special case - the only dtype that can be constructed from a length with no value.
-            raise ValueError
-        d.set_fn(b, value)
-        bs = b._bitstore
-        if token_length is not None and len(bs) != d.bitlength:
-            raise bitstring.CreationError(f"Token with length {token_length} packed with value of length {len(bs)} "
-                                f"({name}:{token_length}={value}).")
+        raise bitstring.CreationError(f"Can't parse token: {e}")
+    if value is None and name != 'pad':
+        raise ValueError(f"Token {name} requires a value.")
+    bs = d.build(value)._bitstore
+    if token_length is not None and len(bs) != d.bitlength:
+        raise bitstring.CreationError(f"Token with length {token_length} packed with value of length {len(bs)} "
+                                      f"({name}:{token_length}={value}).")
     return bs
```

### Comparing `bitstring-4.2.0b1/bitstring/bitstream.py` & `bitstring-4.2.0b2/bitstring/bitstream.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import bitstring
 from bitstring.bits import Bits, BitsType
+from bitstring.dtypes import Dtype
 from typing import Union, List, Any, Optional, overload, TypeVar, Tuple
 import copy
 import numbers
 
 TConstBitStream = TypeVar("TConstBitStream", bound='ConstBitStream')
 
 
@@ -200,15 +201,15 @@
 
     def __repr__(self) -> str:
         """Return representation that could be used to recreate the bitstring.
 
         If the returned string is too long it will be truncated. See __str__().
 
         """
-        return self._repr(self.__class__.__name__, len(self), self._bitstore.filename, self._pos)
+        return self._repr(self.__class__.__name__, len(self), self._pos)
 
     def overwrite(self, bs: BitsType, /, pos: Optional[int] = None) -> None:
         """Overwrite with bitstring at bit position pos.
 
         bs -- The bitstring to overwrite with.
         pos -- The bit position to begin overwriting from.
 
@@ -350,15 +351,15 @@
             val, self._pos = dtype.read_fn(self, self._pos)
 
         if self._pos > len(self):
             self._pos = p
             raise bitstring.ReadError(f"Reading off end of bitstring with fmt '{fmt}'. Only {len(self) - p} bits available.")
         return val
 
-    def readlist(self, fmt: Union[str, List[Union[int, str]]], **kwargs) \
+    def readlist(self, fmt: Union[str, List[Union[int, str, Dtype]]], **kwargs) \
             -> List[Union[int, float, str, Bits, bool, bytes, None]]:
         """Interpret next bits according to format string(s) and return list.
 
         fmt -- A single string or list of strings with comma separated tokens
                describing how to interpret the next bits in the bitstring. Items
                can also be integers, for reading new bitstring of the given length.
         kwargs -- A dictionary or keyword-value pairs - the keywords used in the
@@ -457,14 +458,30 @@
         aligning to the next byte.
 
         """
         skipped = (8 - (self._pos % 8)) % 8
         self.pos += skipped
         return skipped
 
+    @classmethod
+    def fromstring(cls: TBits, s: str, /) -> TBits:
+        x = super().fromstring(s)
+        x._pos = 0
+        x._bitstore.immutable = True
+        return x
+
+    def __getitem__(self: TBits, key: Union[slice, int], /) -> Union[TBits, bool]:
+        """Return a new bitstring representing a slice of the current bitstring."""
+        if isinstance(key, numbers.Integral):
+            return bool(self._bitstore.getindex(key))
+        bs = super().__new__(self.__class__)
+        bs._bitstore = self._bitstore.getslice_withstep(key)
+        bs._pos = 0
+        return bs
+
     pos = property(_getbitpos, _setbitpos,
                    doc="""The position in the bitstring in bits. Read and write.
                       """)
     bitpos = property(_getbitpos, _setbitpos,
                       doc="""The position in the bitstring in bits. Read and write.
                       """)
     bytepos = property(_getbytepos, _setbytepos,
```

### Comparing `bitstring-4.2.0b1/bitstring/exceptions.py` & `bitstring-4.2.0b2/bitstring/exceptions.py`

 * *Files identical despite different names*

### Comparing `bitstring-4.2.0b1/bitstring/methods.py` & `bitstring-4.2.0b2/bitstring/methods.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import bitstring
 from bitstring.bitstream import BitStream
 from bitstring.utils import tokenparser
 from bitstring.exceptions import CreationError
 from typing import Union, List
 from bitstring.bitstore import BitStore
 from bitstring.bitstore_helpers import bitstore_from_token
-from bitstring.dtypes import dtype_register
 
 
 def pack(fmt: Union[str, List[str]], *values, **kwargs) -> BitStream:
     """Pack the values according to the format string and return a new BitStream.
 
     fmt -- A single string or a list of strings with comma separated tokens
            describing how to create the BitStream.
@@ -55,19 +54,17 @@
     except ValueError as e:
         raise CreationError(*e.args)
     value_iter = iter(values)
     bsl: List[BitStore] = []
     try:
         for name, length, value in tokens:
             # If the value is in the kwd dictionary then it takes precedence.
-            if value in kwargs:
-                value = kwargs[value]
+            value = kwargs.get(value, value)
             # If the length is in the kwd dictionary then use that too.
-            if length in kwargs:
-                length = kwargs[length]
+            length = kwargs.get(length, length)
             # Also if we just have a dictionary name then we want to use it
             if name in kwargs and length is None and value is None:
                 bsl.append(BitStream(kwargs[name])._bitstore)
                 continue
             if length is not None:
                 length = int(length)
             if value is None and name != 'pad':
```

### Comparing `bitstring-4.2.0b1/bitstring/utils.py` & `bitstring-4.2.0b2/bitstring/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,37 +130,36 @@
         # If you don't specify a 'name' then the default is 'bits'
         name = 'bits'
         length = token
     return name, length, value
 
 @functools.lru_cache(CACHE_SIZE)
 def preprocess_tokens(fmt: str) -> List[str]:
-    # Remove whitespace
-    fmt = ''.join(fmt.split())
-    # Expand any brackets.
-    fmt = expand_brackets(fmt)
+    # Remove whitespace and expand brackets
+    fmt = expand_brackets(''.join(fmt.split()))
+
     # Split tokens by ',' and remove whitespace
-    # The meta_tokens can either be ordinary single tokens or multiple
-    # struct-format token strings.
+    # The meta_tokens can either be ordinary single tokens or multiple struct-format token strings.
     meta_tokens = [f.strip() for f in fmt.split(',')]
-    single_tokens = []
+    final_tokens = []
+
     for meta_token in meta_tokens:
-        # See if it has a multiplicative factor
-        if not (m := MULTIPLICATIVE_RE.match(meta_token)):
-            factor = 1
-        else:
+        # Extract factor and actual token if a multiplicative factor exists
+        factor = 1
+        if m := MULTIPLICATIVE_RE.match(meta_token):
             factor = int(m.group('factor'))
             meta_token = m.group('token')
-        # See if it's a struct-like format
-        if m := STRUCT_PACK_RE.match(meta_token):
-            tokens = structparser(m)
-        else:
-            tokens = [meta_token]
-        single_tokens.extend(tokens * factor)  # TODO: This is inefficient as the same token will be parsed multiple times.
-    return single_tokens
+
+        # Parse struct-like format into sub-tokens or treat as single token
+        tokens = structparser(m) if (m := STRUCT_PACK_RE.match(meta_token)) else [meta_token]
+
+        # Extend final tokens list with parsed tokens, repeated by the factor
+        final_tokens.extend(tokens * factor)
+    return final_tokens
+
 
 @functools.lru_cache(CACHE_SIZE)
 def tokenparser(fmt: str, keys: Tuple[str, ...] = ()) -> \
         Tuple[bool, List[Tuple[str, Union[int, str, None], Optional[str]]]]:
     """Divide the format string into tokens and parse them.
 
     Return stretchy token and list of [initialiser, length, value]
@@ -208,22 +207,19 @@
     while True:
         start = s.find('(')
         if start == -1:
             break
         count = 1  # Number of hanging open brackets
         p = start + 1
         while p < len(s):
-            if s[p] == '(':
-                count += 1
-            if s[p] == ')':
-                count -= 1
-            if not count:
+            count += (s[p] == '(') - (s[p] == ')')
+            if count == 0:
                 break
             p += 1
-        if count:
+        if count != 0:
             raise ValueError(f"Unbalanced parenthesis in '{s}'.")
         if start == 0 or s[start - 1] != '*':
             s = s[0:start] + s[start + 1:p] + s[p + 1:]
         else:
             # Looks for first number*(
             m = BRACKET_RE.search(s)
             if m:
```

### Comparing `bitstring-4.2.0b1/bitstring.egg-info/PKG-INFO` & `bitstring-4.2.0b2/bitstring.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitstring
-Version: 4.2.0b1
+Version: 4.2.0b2
 Summary: Simple construction, analysis and modification of binary data.
 Author-email: Scott Griffiths <dr.scottgriffiths@gmail.com>
 Project-URL: homepage, https://github.com/scott-griffiths/bitstring
 Project-URL: documentation, https://bitstring.readthedocs.io/
 Keywords: binary,bitarray,bitvector,bitfield
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -33,25 +33,33 @@
 
 
 [![CI badge](https://github.com/scott-griffiths/bitstring/actions/workflows/.github/workflows/ci.yml/badge.svg)](https://github.com/scott-griffiths/bitstring/actions/workflows/ci.yml)
 [![Docs](https://img.shields.io/readthedocs/bitstring?logo=readthedocs&logoColor=white)](https://bitstring.readthedocs.io/en/latest/)
 [![Codacy Badge](https://img.shields.io/codacy/grade/8869499b2eed44548fa1a5149dd451f4?logo=codacy)](https://app.codacy.com/gh/scott-griffiths/bitstring/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/bitstring?logo=libraries.io&logoColor=white)](https://libraries.io/pypi/bitstring)
 &nbsp; &nbsp;
-[![Pepy Total Downlods](https://img.shields.io/pepy/dt/bitstring?logo=python&logoColor=white&labelColor=blue&color=blue)](https://pypistats.org/packages/bitstring)
+[![Pepy Total Downlods](https://img.shields.io/pepy/dt/bitstring?logo=python&logoColor=white&labelColor=blue&color=blue)](https://www.pepy.tech/projects/bitstring)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/bitstring?label=%40&labelColor=blue&color=blue)](https://pypistats.org/packages/bitstring)
 
 
 News
 ----
-**29th November 2023**: bitstring 4.1.4 released. Version 4.1 is a large update in terms of how much of the code has changed.
+**March 2024**: bitstring 4.2.0b2 released. This is the final beta release before 4.2. 
 
-* New Array class for homogeneous data.
-* Support for 8-bit floating point values.
-* Speed increased with bitarray dependency.
+Install the beta with `pip install bitstring==4.2.0b2`, or use `pip install bitstring` for the latest stable version.
+
+New in 4.2:
+
+* Dropped support for Python 3.7. Minimum version is now 3.8.
+* A new `Dtype` class can be optionally used to specify types.
+* The `bitstring.options` object is now the preferred method for changing module options.
+* New `fromstring` method as another way to create bitstrings from formatted strings.
+* More types can now be pretty printed.
+* A range of 8-bit, 6-bit and even 4-bit float formats added (beta):
+* Performance improvements.
 
 See the [release notes](https://github.com/scott-griffiths/bitstring/blob/main/release_notes.txt) for details. Please let me know if you encounter any problems.
 
 
 Overview
 --------
 
@@ -133,24 +141,17 @@
      >>> a.data
      BitArray('0x1390181')
      >>> a[::2] *= 5
      >>> a
      Array('uint7', [45, 100, 15, 1])
 
 
-Unit Tests
-----------
-
-The 700+ unit tests should all pass. They can be run from the root of the project with
-
-     python -m unittest
-
 
 Credits
 -------
 
 Created in 2006 to help with ad hoc parsing and creation of compressed video files.
 Maintained and expanded ever since as it became unexpectedly popular.
 Thanks to all those who have contributed ideas and code (and bug reports) over the years.
 
 
-<sub>Copyright (c) 2006 - 2023 Scott Griffiths</sub>
+<sub>Copyright (c) 2006 - 2024 Scott Griffiths</sub>
```

### Comparing `bitstring-4.2.0b1/bitstring.egg-info/SOURCES.txt` & `bitstring-4.2.0b2/bitstring.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 bitstring/bitstore.py
 bitstring/bitstore_helpers.py
 bitstring/bitstream.py
 bitstring/bitstring_options.py
 bitstring/dtypes.py
 bitstring/exceptions.py
 bitstring/fp8.py
+bitstring/luts.py
 bitstring/methods.py
+bitstring/mxfp.py
 bitstring/py.typed
 bitstring/utils.py
 bitstring.egg-info/PKG-INFO
 bitstring.egg-info/SOURCES.txt
 bitstring.egg-info/dependency_links.txt
 bitstring.egg-info/requires.txt
 bitstring.egg-info/top_level.txt
@@ -30,8 +32,10 @@
 tests/test_bitarray.py
 tests/test_bits.py
 tests/test_bitstore.py
 tests/test_bitstream.py
 tests/test_bitstring.py
 tests/test_constbitstream.py
 tests/test_dtypes.py
-tests/test_fp8.py
+tests/test_fp8.py
+tests/test_mxfp.py
+tests/test_scaled_dtypes.py
```

### Comparing `bitstring-4.2.0b1/pyproject.toml` & `bitstring-4.2.0b2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bitstring"
-version = "4.2.0b1"
+version = "4.2.0b2"
 authors = [
   { name="Scott Griffiths", email="dr.scottgriffiths@gmail.com" },
 ]
 description = "Simple construction, analysis and modification of binary data."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `bitstring-4.2.0b1/release_notes.txt` & `bitstring-4.2.0b2/release_notes.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,50 @@
 --------------------------------
 bitstring module version history
 --------------------------------
 
------------------------------
-In preparation: version 4.2.0
------------------------------
+-------------------------
+March 2024: version 4.2.0
+-------------------------
+
+This release contains a fairly large refactor of how different types are managed. This
+shouldn't affect the end user, and the main noticable change should be the new Dtype
+class, which is optional to use.
+
+Support for 8-bit and smaller floats has been reworked and expanded. These are still
+a 'beta' feature.
+
+Backwardly incompatible changes:
 
-* Array class no longer 'beta'.
-* New Dtype class can be optionally used to specify types.
 * Dropped support for Python 3.7. Minimum version is now 3.8.
-* The bitstring.options object is now preferred method for changing module options.
+* For tokens that use a non-numeric length, a ':' is now compulsory rather than
+  recommended. For example use 'uint:foo' instead of 'uintfoo'.
+* The previous e4m3float and e5m2float formats have become the slightly modified
+  p4binary8 and p3binary8 formats.
+* Some parameters are now enforced as positional only, such as `auto` in constructors.
+
+Other changes:
+
+* The Array class is no longer 'beta'.
+* A new Dtype class can be optionally used to specify types.
+* The bitstring.options object is now the preferred method for changing module options.
+* New fromstring method as another way to create bitstrings from formatted strings.
+* More types can now be pretty printed.
+* Pretty printing is now prettier - optional terminal colours added.
+* A range of 8-bit, 6-bit and even 4-bit float formats added (beta):
+  p3binary8: IEEE 8-bit floating point with 3 bit precision.
+  p4binary8: IEEE 8-bit floating point with 4 bit precision.
+  e5m2mxfp: OCP 8-bit floating point with 3 bit precision.
+  e4m3mxfp: OCP 8-bit floating point with 4 bit precision.
+  e2m3mxfp: OCP 6-bit floating point with 4 bit precision.
+  e3m2mxfp: OCP 6-bit floating point with 3 bit precision.
+  e2m1mxfp: OCP 4-bit floating point with 2 bit precision.
+  e8m0mxfp: OCP 8-bit unsigned floating point designed to scale the other formats.
+  mxint: OCP 8-bit floating point that is a scaled integer representation.
 * Performance improvements.
-* More types can be pretty printed.
-* Pretty printing is now prettier - terminal colours added.
-
 
 
 ----------------------------
 November 2023: version 4.1.4
 ----------------------------
 Fixing a regression introduced in 4.1.3
```

### Comparing `bitstring-4.2.0b1/tests/test.m1v` & `bitstring-4.2.0b2/tests/test.m1v`

 * *Files identical despite different names*

### Comparing `bitstring-4.2.0b1/tests/test_bitstore.py` & `bitstring-4.2.0b2/tests/test_bitstore.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,94 +1,94 @@
 #!/usr/bin/env python
 
-import unittest
+import pytest
 import sys
 sys.path.insert(0, '..')
 import bitstring
 from bitstring.bitstore import BitStore, offset_slice_indices_lsb0
 import sys
 
 sys.path.insert(0, '..')
 
 
-class BasicFunctionality(unittest.TestCase):
+class TestBasicFunctionality:
 
-    def testGettingInt(self):
+    def test_getting_int(self):
         a = BitStore('001')
-        self.assertEqual(a.getindex(0), 0)
-        self.assertEqual(a.getindex(1), 0)
-        self.assertEqual(a.getindex(2), 1)
-
-        self.assertEqual(a.getindex(-1), 1)
-        self.assertEqual(a.getindex(-2), 0)
-        self.assertEqual(a.getindex(-3), 0)
+        assert a.getindex(0) == 0
+        assert a.getindex(1) == 0
+        assert a.getindex(2) == 1
+
+        assert a.getindex(-1) == 1
+        assert a.getindex(-2) == 0
+        assert a.getindex(-3) == 0
 
-        with self.assertRaises(IndexError):
+        with pytest.raises(IndexError):
             _ = a.getindex(3)
-        with self.assertRaises(IndexError):
+        with pytest.raises(IndexError):
             _ = a.getindex(-4)
 
 
-class BasicLSB0Functionality(unittest.TestCase):
+class TestBasicLSB0Functionality:
 
     @classmethod
-    def setUpClass(cls):
+    def setup_class(cls):
         bitstring.lsb0 = True
 
     @classmethod
-    def tearDownClass(cls):
+    def teardown_class(cls):
         bitstring.lsb0 = False
 
-    def testGettingInt(self):
+    def test_getting_int(self):
         a = BitStore('001')
-        self.assertEqual(a.getindex(0), 1)
-        self.assertEqual(a.getindex(1), 0)
-        self.assertEqual(a.getindex(2), 0)
-
-        self.assertEqual(a.getindex(-1), 0)
-        self.assertEqual(a.getindex(-2), 0)
-        self.assertEqual(a.getindex(-3), 1)
+        assert a.getindex(0) == 1
+        assert a.getindex(1) == 0
+        assert a.getindex(2) == 0
+
+        assert a.getindex(-1) == 0
+        assert a.getindex(-2) == 0
+        assert a.getindex(-3) == 1
 
-        with self.assertRaises(IndexError):
+        with pytest.raises(IndexError):
             _ = a.getindex(3)
-        with self.assertRaises(IndexError):
+        with pytest.raises(IndexError):
             _ = a.getindex(-4)
 
-    def testGettingSlice(self):
-        a = BitStore(buffer=b'12345678')
-        self.assertEqual(a.getslice(None, None).tobytes(), b'12345678')
-        self.assertEqual(a.getslice(None, -8).tobytes(), b'2345678')
-        self.assertEqual(a.getslice(8, None).tobytes(), b'1234567')
-        self.assertEqual(a.getslice(16, 24).tobytes(), b'6')
+    def test_getting_slice(self):
+        a = BitStore.frombytes(b'12345678')
+        assert a.getslice(None, None).tobytes() == b'12345678'
+        assert a.getslice(None, -8).tobytes() == b'2345678'
+        assert a.getslice(8, None).tobytes() == b'1234567'
+        assert a.getslice(16, 24).tobytes() == b'6'
 
-    def testSettingInt(self):
+    def test_setting_int(self):
         a = BitStore('00000')
         a[0] = 1
-        self.assertEqual(a.slice_to_bin(), '00001')
+        assert a.slice_to_bin() == '00001'
         a[-1] = 1
-        self.assertEqual(a.slice_to_bin(), '10001')
-        with self.assertRaises(IndexError):
+        assert a.slice_to_bin() == '10001'
+        with pytest.raises(IndexError):
             a[5] = 1
-        with self.assertRaises(IndexError):
+        with pytest.raises(IndexError):
             a[-6] = 0
 
 
-class GettingSlices(unittest.TestCase):
+class TestGettingSlices:
 
-    def tearDown(self) -> None:
+    def teardown_method(self) -> None:
         bitstring.lsb0 = False
 
-    def testEverything(self):
+    def test_everything(self):
         a = BitStore('010010001000110111001111101101001111')
 
         # Try combination of start and stop for msb0 and get the result.
         # Convert to start and stop needed for lsb0
         options = [5, 2, -2, 1, 7, -3, -9, 0, -1, -len(a), len(a), len(a) - 1, -len(a) - 1, -100, 100, None]
         for start_option in options:
             for end_option in options:
                 bitstring.lsb0 = True
                 lsb0 = a.getslice(start_option, end_option)
                 bitstring.lsb0 = False
                 msb0 = a.getslice(start_option, end_option)
                 new_slice = offset_slice_indices_lsb0(slice(start_option, end_option, None), len(a))
                 new_start, new_end = new_slice.start, new_slice.stop
-                self.assertEqual(len(msb0), len(lsb0), f"[{start_option}: {end_option}] -> [{new_start}: {new_end}]  len(msb0)={len(msb0)}, len(lsb0)={len(lsb0)}")
+                assert len(msb0) == len(lsb0), f"[{start_option}: {end_option}] -> [{new_start}: {new_end}]  len(msb0)={len(msb0)}, len(lsb0)={len(lsb0)}"
```

