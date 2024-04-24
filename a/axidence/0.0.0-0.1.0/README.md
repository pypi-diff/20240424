# Comparing `tmp/axidence-0.0.0.tar.gz` & `tmp/axidence-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axidence-0.0.0.tar", last modified: Wed Apr 17 22:18:28 2024, max compression
+gzip compressed data, was "axidence-0.1.0.tar", last modified: Wed Apr 24 15:15:20 2024, max compression
```

## Comparing `axidence-0.0.0.tar` & `axidence-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:18:28.114949 axidence-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-17 22:18:24.000000 axidence-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-17 22:18:28.114949 axidence-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-17 22:18:24.000000 axidence-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:18:28.114949 axidence-0.0.0/axidence/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-17 22:18:24.000000 axidence-0.0.0/axidence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:18:28.114949 axidence-0.0.0/axidence.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-17 22:18:28.000000 axidence-0.0.0/axidence.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-17 22:18:28.000000 axidence-0.0.0/axidence.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 22:18:28.000000 axidence-0.0.0/axidence.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 22:18:28.000000 axidence-0.0.0/axidence.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 22:18:28.000000 axidence-0.0.0/axidence.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-17 22:18:24.000000 axidence-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-17 22:18:28.114949 axidence-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:18:28.114949 axidence-0.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-17 22:18:24.000000 axidence-0.0.0/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:20.695610 axidence-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-24 15:15:13.000000 axidence-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-04-24 15:15:20.691610 axidence-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-24 15:15:13.000000 axidence-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:20.691610 axidence-0.1.0/axidence/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:20.691610 axidence-0.1.0/axidence/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:20.691610 axidence-0.1.0/axidence/plugins/isolated/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/plugins/isolated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/plugins/isolated/isolated_s1.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/plugins/isolated/isolated_s2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:20.691610 axidence-0.1.0/axidence/plugins/pairing/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/plugins/pairing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/plugins/pairing/paired_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/plugins/pairing/paired_peaks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:20.691610 axidence-0.1.0/axidence/plugins/salting/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/plugins/salting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/plugins/salting/event_building.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/plugins/salting/event_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/plugins/salting/peak_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9262 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/plugins/salting/salting_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/plugins/salting/salting_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-24 15:15:13.000000 axidence-0.1.0/axidence/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:20.691610 axidence-0.1.0/axidence.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-04-24 15:15:20.000000 axidence-0.1.0/axidence.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-24 15:15:20.000000 axidence-0.1.0/axidence.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:15:20.000000 axidence-0.1.0/axidence.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 15:15:20.000000 axidence-0.1.0/axidence.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 15:15:20.000000 axidence-0.1.0/axidence.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-24 15:15:13.000000 axidence-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-24 15:15:20.695610 axidence-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:15:20.691610 axidence-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-24 15:15:13.000000 axidence-0.1.0/tests/test_deps_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-24 15:15:13.000000 axidence-0.1.0/tests/test_exhaust_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-24 15:15:13.000000 axidence-0.1.0/tests/test_salting.py
```

### Comparing `axidence-0.0.0/LICENSE` & `axidence-0.1.0/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2018, The axidence contributors and the XENON collaboration
+Copyright (c) 2018, axidence contributors.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `axidence-0.0.0/PKG-INFO` & `axidence-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: axidence
-Version: 0.0.0
+Version: 0.1.0
 Summary: strax-based data-driven accidental coincidence background simulation and peak-level salting
 Author-email: Dacheng Xu <dx2227@columbia.edu>
 Maintainer-email: Dacheng Xu <dx2227@columbia.edu>
 License: BSD 3-Clause License
         
-        Copyright (c) 2018, The axidence contributors and the XENON collaboration
+        Copyright (c) 2018, axidence contributors.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         * Redistributions of source code must retain the above copyright notice, this
           list of conditions and the following disclaimer.
@@ -42,16 +42,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: strax>=1.6.0
-Requires-Dist: straxen>=2.2.0
+Requires-Dist: strax
+Requires-Dist: straxen
 
 # Axidence
 
 [![Test package](https://github.com/dachengx/axidence/actions/workflows/pytest.yml/badge.svg?branch=main)](https://github.com/dachengx/axidence/actions/workflows/pytest.yml)
 [![Coverage Status](https://coveralls.io/repos/github/dachengx/axidence/badge.svg?branch=main&kill_cache=1)](https://coveralls.io/github/dachengx/axidence?branch=main&kill_cache=1)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/axidence.svg)](https://pypi.python.org/pypi/axidence/)
 [![Documentation Status](https://readthedocs.org/projects/axidence/badge/?version=latest)](https://axidence.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `axidence-0.0.0/README.md` & `axidence-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `axidence-0.0.0/axidence.egg-info/PKG-INFO` & `axidence-0.1.0/axidence.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: axidence
-Version: 0.0.0
+Version: 0.1.0
 Summary: strax-based data-driven accidental coincidence background simulation and peak-level salting
 Author-email: Dacheng Xu <dx2227@columbia.edu>
 Maintainer-email: Dacheng Xu <dx2227@columbia.edu>
 License: BSD 3-Clause License
         
-        Copyright (c) 2018, The axidence contributors and the XENON collaboration
+        Copyright (c) 2018, axidence contributors.
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         * Redistributions of source code must retain the above copyright notice, this
           list of conditions and the following disclaimer.
@@ -42,16 +42,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: strax>=1.6.0
-Requires-Dist: straxen>=2.2.0
+Requires-Dist: strax
+Requires-Dist: straxen
 
 # Axidence
 
 [![Test package](https://github.com/dachengx/axidence/actions/workflows/pytest.yml/badge.svg?branch=main)](https://github.com/dachengx/axidence/actions/workflows/pytest.yml)
 [![Coverage Status](https://coveralls.io/repos/github/dachengx/axidence/badge.svg?branch=main&kill_cache=1)](https://coveralls.io/github/dachengx/axidence?branch=main&kill_cache=1)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/axidence.svg)](https://pypi.python.org/pypi/axidence/)
 [![Documentation Status](https://readthedocs.org/projects/axidence/badge/?version=latest)](https://axidence.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `axidence-0.0.0/pyproject.toml` & `axidence-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "axidence"
-version = "0.0.0"
+version = "0.1.0"
 description = "strax-based data-driven accidental coincidence background simulation and peak-level salting"
 readme = "README.md"
 license.file = "LICENSE"
 authors = [
   { name = "Dacheng Xu", email = "dx2227@columbia.edu" },
 ]
 maintainers = [
   { name = "Dacheng Xu", email = "dx2227@columbia.edu" },
 ]
 requires-python = ">=3.9"
 
 dependencies = [
-  "strax>=1.6.0",
-  "straxen>=2.2.0",
+  "strax",
+  "straxen",
 ]
 
 classifiers = [
   "Development Status :: 3 - Alpha",
   "License :: OSI Approved :: BSD License",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.9",
```

