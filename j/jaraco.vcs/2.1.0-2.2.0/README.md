# Comparing `tmp/jaraco_vcs-2.1.0.tar.gz` & `tmp/jaraco_vcs-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco_vcs-2.1.0.tar", last modified: Mon Apr 22 16:02:08 2024, max compression
+gzip compressed data, was "jaraco_vcs-2.2.0.tar", last modified: Wed Apr 24 13:22:56 2024, max compression
```

## Comparing `jaraco_vcs-2.1.0.tar` & `jaraco_vcs-2.2.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:02:08.819067 jaraco_vcs-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:02:08.815067 jaraco_vcs-2.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:02:08.815067 jaraco_vcs-2.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-22 16:02:08.819067 jaraco_vcs-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:02:08.815067 jaraco_vcs-2.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:02:08.811066 jaraco_vcs-2.1.0/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:02:08.819067 jaraco_vcs-2.1.0/jaraco/vcs/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/jaraco/vcs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3500 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/jaraco/vcs/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/jaraco/vcs/cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/jaraco/vcs/library.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/jaraco/vcs/reentry.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/jaraco/vcs/subprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:02:08.819067 jaraco_vcs-2.1.0/jaraco.vcs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-22 16:02:08.000000 jaraco_vcs-2.1.0/jaraco.vcs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-22 16:02:08.000000 jaraco_vcs-2.1.0/jaraco.vcs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 16:02:08.000000 jaraco_vcs-2.1.0/jaraco.vcs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-22 16:02:08.000000 jaraco_vcs-2.1.0/jaraco.vcs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-22 16:02:08.000000 jaraco_vcs-2.1.0/jaraco.vcs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 16:02:08.819067 jaraco_vcs-2.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:02:08.819067 jaraco_vcs-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/tests/test_git.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/tests/test_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/tests/test_mercurial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/tests/test_reentry.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-22 16:01:46.000000 jaraco_vcs-2.1.0/tox.ini
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-04-24 13:22:56.531101 jaraco_vcs-2.2.0/
+-rw-r--r--   0 jaraco     (501) staff       (20)      200 2024-03-25 19:04:26.000000 jaraco_vcs-2.2.0/.coveragerc
+-rw-r--r--   0 jaraco     (501) staff       (20)      246 2024-02-02 02:03:18.000000 jaraco_vcs-2.2.0/.editorconfig
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-04-24 13:22:56.525506 jaraco_vcs-2.2.0/.github/
+-rw-r--r--   0 jaraco     (501) staff       (20)      148 2024-02-02 02:03:18.000000 jaraco_vcs-2.2.0/.github/dependabot.yml
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-04-24 13:22:56.525628 jaraco_vcs-2.2.0/.github/workflows/
+-rw-r--r--   0 jaraco     (501) staff       (20)     2918 2024-04-22 14:54:48.000000 jaraco_vcs-2.2.0/.github/workflows/main.yml
+-rw-r--r--   0 jaraco     (501) staff       (20)      116 2024-02-02 02:03:18.000000 jaraco_vcs-2.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 jaraco     (501) staff       (20)      335 2024-03-25 19:04:30.000000 jaraco_vcs-2.2.0/.readthedocs.yaml
+-rw-r--r--   0 jaraco     (501) staff       (20)     1023 2024-02-02 02:03:18.000000 jaraco_vcs-2.2.0/LICENSE
+-rw-r--r--   0 jaraco     (501) staff       (20)      684 2024-04-24 12:53:02.000000 jaraco_vcs-2.2.0/NEWS.rst
+-rw-r--r--   0 jaraco     (501) staff       (20)     3954 2024-04-24 13:22:56.530860 jaraco_vcs-2.2.0/PKG-INFO
+-rw-r--r--   0 jaraco     (501) staff       (20)     2454 2024-03-25 19:04:26.000000 jaraco_vcs-2.2.0/README.rst
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-04-24 13:22:56.526173 jaraco_vcs-2.2.0/docs/
+-rw-r--r--   0 jaraco     (501) staff       (20)     1193 2024-02-02 02:03:18.000000 jaraco_vcs-2.2.0/docs/conf.py
+-rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-02-02 02:03:18.000000 jaraco_vcs-2.2.0/docs/history.rst
+-rw-r--r--   0 jaraco     (501) staff       (20)      519 2024-02-02 02:03:18.000000 jaraco_vcs-2.2.0/docs/index.rst
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-04-24 13:22:56.522832 jaraco_vcs-2.2.0/jaraco/
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-04-24 13:22:56.528651 jaraco_vcs-2.2.0/jaraco/vcs/
+-rw-r--r--   0 jaraco     (501) staff       (20)      212 2024-04-01 00:54:05.000000 jaraco_vcs-2.2.0/jaraco/vcs/__init__.py
+-rwxr-xr-x   0 jaraco     (501) staff       (20)     3500 2024-04-22 15:05:13.000000 jaraco_vcs-2.2.0/jaraco/vcs/base.py
+-rw-r--r--   0 jaraco     (501) staff       (20)     6461 2024-04-24 12:51:51.000000 jaraco_vcs-2.2.0/jaraco/vcs/cmd.py
+-rw-r--r--   0 jaraco     (501) staff       (20)      709 2024-04-01 00:54:05.000000 jaraco_vcs-2.2.0/jaraco/vcs/library.py
+-rw-r--r--   0 jaraco     (501) staff       (20)     1581 2024-04-01 00:54:05.000000 jaraco_vcs-2.2.0/jaraco/vcs/reentry.py
+-rw-r--r--   0 jaraco     (501) staff       (20)      987 2024-04-01 00:54:05.000000 jaraco_vcs-2.2.0/jaraco/vcs/subprocess.py
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-04-24 13:22:56.529832 jaraco_vcs-2.2.0/jaraco.vcs.egg-info/
+-rw-r--r--   0 jaraco     (501) staff       (20)     3954 2024-04-24 13:22:56.000000 jaraco_vcs-2.2.0/jaraco.vcs.egg-info/PKG-INFO
+-rw-r--r--   0 jaraco     (501) staff       (20)      679 2024-04-24 13:22:56.000000 jaraco_vcs-2.2.0/jaraco.vcs.egg-info/SOURCES.txt
+-rw-r--r--   0 jaraco     (501) staff       (20)        1 2024-04-24 13:22:56.000000 jaraco_vcs-2.2.0/jaraco.vcs.egg-info/dependency_links.txt
+-rw-r--r--   0 jaraco     (501) staff       (20)      305 2024-04-24 13:22:56.000000 jaraco_vcs-2.2.0/jaraco.vcs.egg-info/requires.txt
+-rw-r--r--   0 jaraco     (501) staff       (20)        7 2024-04-24 13:22:56.000000 jaraco_vcs-2.2.0/jaraco.vcs.egg-info/top_level.txt
+-rw-r--r--   0 jaraco     (501) staff       (20)      154 2024-02-02 02:03:18.000000 jaraco_vcs-2.2.0/mypy.ini
+-rw-r--r--   0 jaraco     (501) staff       (20)     1228 2024-04-22 15:03:45.000000 jaraco_vcs-2.2.0/pyproject.toml
+-rw-r--r--   0 jaraco     (501) staff       (20)      584 2024-04-01 00:52:14.000000 jaraco_vcs-2.2.0/pytest.ini
+-rw-r--r--   0 jaraco     (501) staff       (20)      419 2024-03-25 19:04:30.000000 jaraco_vcs-2.2.0/ruff.toml
+-rw-r--r--   0 jaraco     (501) staff       (20)       38 2024-04-24 13:22:56.531143 jaraco_vcs-2.2.0/setup.cfg
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-04-24 13:22:56.529640 jaraco_vcs-2.2.0/tests/
+-rw-r--r--   0 jaraco     (501) staff       (20)        0 2024-02-02 02:03:18.000000 jaraco_vcs-2.2.0/tests/__init__.py
+-rw-r--r--   0 jaraco     (501) staff       (20)     1151 2024-04-01 00:54:05.000000 jaraco_vcs-2.2.0/tests/conftest.py
+-rw-r--r--   0 jaraco     (501) staff       (20)     1435 2024-04-22 15:05:34.000000 jaraco_vcs-2.2.0/tests/test_git.py
+-rw-r--r--   0 jaraco     (501) staff       (20)      766 2024-04-01 00:54:05.000000 jaraco_vcs-2.2.0/tests/test_managers.py
+-rw-r--r--   0 jaraco     (501) staff       (20)     5568 2024-04-22 15:05:50.000000 jaraco_vcs-2.2.0/tests/test_mercurial.py
+-rw-r--r--   0 jaraco     (501) staff       (20)     2394 2024-02-02 02:03:18.000000 jaraco_vcs-2.2.0/tests/test_reentry.py
+-rw-r--r--   0 jaraco     (501) staff       (20)       44 2024-02-02 02:03:18.000000 jaraco_vcs-2.2.0/towncrier.toml
+-rw-r--r--   0 jaraco     (501) staff       (20)     1364 2024-03-25 19:04:30.000000 jaraco_vcs-2.2.0/tox.ini
```

### Comparing `jaraco_vcs-2.1.0/.github/workflows/main.yml` & `jaraco_vcs-2.2.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `jaraco_vcs-2.1.0/LICENSE` & `jaraco_vcs-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco_vcs-2.1.0/NEWS.rst` & `jaraco_vcs-2.2.0/NEWS.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v2.2.0
+======
+
+Features
+--------
+
+- Remove check on minimum git version.
+
+
 v2.1.0
 ======
 
 Features
 --------
 
 - Added .get_timestamp method for retrieving the timestamp of a given revision.
```

### Comparing `jaraco_vcs-2.1.0/PKG-INFO` & `jaraco_vcs-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.vcs
-Version: 2.1.0
+Version: 2.2.0
 Summary: Facilities for working with VCS repositories
 Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
 Project-URL: Homepage, https://github.com/jaraco/jaraco.vcs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jaraco_vcs-2.1.0/README.rst` & `jaraco_vcs-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `jaraco_vcs-2.1.0/docs/conf.py` & `jaraco_vcs-2.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco_vcs-2.1.0/docs/index.rst` & `jaraco_vcs-2.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jaraco_vcs-2.1.0/jaraco/vcs/base.py` & `jaraco_vcs-2.2.0/jaraco/vcs/base.py`

 * *Files identical despite different names*

### Comparing `jaraco_vcs-2.1.0/jaraco/vcs/cmd.py` & `jaraco_vcs-2.2.0/jaraco/vcs/cmd.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import collections
 import itertools
 import operator
 import os.path
 import re
 
-import packaging
-
 TaggedRevision = collections.namedtuple('TaggedRevision', 'tag revision')
 
 
 class Command:
     def is_valid(self):
         try:
             # Check if both command and repo are valid
@@ -149,22 +147,15 @@
 
 
 class Git(Command):
     exe = 'git'
     version_pattern = r'git version (\d+\.\d+[^ ]*)'
 
     def is_valid(self):
-        return super().is_valid() and self.version_suitable()
-
-    def version_suitable(self):
-        req_ver = packaging.version.Version('1.7.10')
-        act_ver = packaging.version.Version(
-            self.version().replace('.windows', '+windows')
-        )
-        return act_ver >= req_ver
+        return super().is_valid()
 
     def find_root(self):
         try:
             return self._invoke('rev-parse', '--top-level').strip()
         except Exception:
             pass
```

### Comparing `jaraco_vcs-2.1.0/jaraco/vcs/library.py` & `jaraco_vcs-2.2.0/jaraco/vcs/library.py`

 * *Files identical despite different names*

### Comparing `jaraco_vcs-2.1.0/jaraco/vcs/reentry.py` & `jaraco_vcs-2.2.0/jaraco/vcs/reentry.py`

 * *Files identical despite different names*

### Comparing `jaraco_vcs-2.1.0/jaraco/vcs/subprocess.py` & `jaraco_vcs-2.2.0/jaraco/vcs/subprocess.py`

 * *Files identical despite different names*

### Comparing `jaraco_vcs-2.1.0/jaraco.vcs.egg-info/PKG-INFO` & `jaraco_vcs-2.2.0/jaraco.vcs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.vcs
-Version: 2.1.0
+Version: 2.2.0
 Summary: Facilities for working with VCS repositories
 Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
 Project-URL: Homepage, https://github.com/jaraco/jaraco.vcs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jaraco_vcs-2.1.0/jaraco.vcs.egg-info/SOURCES.txt` & `jaraco_vcs-2.2.0/jaraco.vcs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaraco_vcs-2.1.0/pyproject.toml` & `jaraco_vcs-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jaraco_vcs-2.1.0/pytest.ini` & `jaraco_vcs-2.2.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `jaraco_vcs-2.1.0/tests/conftest.py` & `jaraco_vcs-2.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jaraco_vcs-2.1.0/tests/test_git.py` & `jaraco_vcs-2.2.0/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `jaraco_vcs-2.1.0/tests/test_managers.py` & `jaraco_vcs-2.2.0/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `jaraco_vcs-2.1.0/tests/test_mercurial.py` & `jaraco_vcs-2.2.0/tests/test_mercurial.py`

 * *Files identical despite different names*

### Comparing `jaraco_vcs-2.1.0/tests/test_reentry.py` & `jaraco_vcs-2.2.0/tests/test_reentry.py`

 * *Files identical despite different names*

### Comparing `jaraco_vcs-2.1.0/tox.ini` & `jaraco_vcs-2.2.0/tox.ini`

 * *Files identical despite different names*

