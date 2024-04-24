# Comparing `tmp/types-peewee-3.17.3.20240420.tar.gz` & `tmp/types-peewee-3.17.3.20240424.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-peewee-3.17.3.20240420.tar", last modified: Sat Apr 20 02:15:03 2024, max compression
+gzip compressed data, was "types-peewee-3.17.3.20240424.tar", last modified: Wed Apr 24 02:17:43 2024, max compression
```

## Comparing `types-peewee-3.17.3.20240420.tar` & `types-peewee-3.17.3.20240424.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:15:03.676123 types-peewee-3.17.3.20240420/
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-20 02:15:03.000000 types-peewee-3.17.3.20240420/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-20 02:15:03.000000 types-peewee-3.17.3.20240420/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-20 02:15:03.676123 types-peewee-3.17.3.20240420/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:15:03.676123 types-peewee-3.17.3.20240420/peewee-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-20 02:15:03.000000 types-peewee-3.17.3.20240420/peewee-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)    63254 2024-04-20 02:15:03.000000 types-peewee-3.17.3.20240420/peewee-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 02:15:03.000000 types-peewee-3.17.3.20240420/peewee-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 02:15:03.676123 types-peewee-3.17.3.20240420/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-20 02:15:03.000000 types-peewee-3.17.3.20240420/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 02:15:03.676123 types-peewee-3.17.3.20240420/types_peewee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-20 02:15:03.000000 types-peewee-3.17.3.20240420/types_peewee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-20 02:15:03.000000 types-peewee-3.17.3.20240420/types_peewee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 02:15:03.000000 types-peewee-3.17.3.20240420/types_peewee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-20 02:15:03.000000 types-peewee-3.17.3.20240420/types_peewee.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:43.190289 types-peewee-3.17.3.20240424/
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-24 02:17:41.000000 types-peewee-3.17.3.20240424/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 02:17:41.000000 types-peewee-3.17.3.20240424/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-24 02:17:43.190289 types-peewee-3.17.3.20240424/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:43.186289 types-peewee-3.17.3.20240424/peewee-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-24 02:17:41.000000 types-peewee-3.17.3.20240424/peewee-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    63254 2024-04-24 02:17:41.000000 types-peewee-3.17.3.20240424/peewee-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 02:17:41.000000 types-peewee-3.17.3.20240424/peewee-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:43.190289 types-peewee-3.17.3.20240424/playhouse-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-24 02:17:41.000000 types-peewee-3.17.3.20240424/playhouse-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:29.000000 types-peewee-3.17.3.20240424/playhouse-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-24 02:17:29.000000 types-peewee-3.17.3.20240424/playhouse-stubs/flask_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 02:17:41.000000 types-peewee-3.17.3.20240424/playhouse-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 02:17:43.190289 types-peewee-3.17.3.20240424/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-24 02:17:41.000000 types-peewee-3.17.3.20240424/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:43.190289 types-peewee-3.17.3.20240424/types_peewee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-24 02:17:43.000000 types-peewee-3.17.3.20240424/types_peewee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-24 02:17:43.000000 types-peewee-3.17.3.20240424/types_peewee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:17:43.000000 types-peewee-3.17.3.20240424/types_peewee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-24 02:17:43.000000 types-peewee-3.17.3.20240424/types_peewee.egg-info/top_level.txt
```

### Comparing `types-peewee-3.17.3.20240420/CHANGELOG.md` & `types-peewee-3.17.3.20240424/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+## 3.17.3.20240424 (2024-04-24)
+
+Add peewee `playhouse.flask_utils` stubs (#11731)
+
+Co-authored-by: Avasam <samuel.06@hotmail.com>
+Co-authored-by: Alex Waygood <alex.waygood@gmail.com>
+
 ## 3.17.3.20240420 (2024-04-20)
 
 Bump peewee to 3.17.3 and fix stubtest entries (#11787)
 
 ## 3.17.0.20240311 (2024-03-11)
 
 Use PEP 570 syntax in third party stubs (#11554)
```

### Comparing `types-peewee-3.17.3.20240420/PKG-INFO` & `types-peewee-3.17.3.20240424/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-peewee
-Version: 3.17.3.20240420
+Version: 3.17.3.20240424
 Summary: Typing stubs for peewee
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/peewee.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -27,11 +27,15 @@
 
 This version of `types-peewee` aims to provide accurate annotations
 for `peewee==3.17.3`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/peewee. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `57f3dcac8dbed008479b251512975901a0206deb` and was tested
+This package was generated from typeshed commit `7ed91bc2e77ec18d28307dc6086a778ecc9c7bb3` and was tested
 with mypy 1.9.0, pyright 1.1.358, and
 pytype 2024.4.11.
```

### Comparing `types-peewee-3.17.3.20240420/peewee-stubs/__init__.pyi` & `types-peewee-3.17.3.20240424/peewee-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-peewee-3.17.3.20240420/setup.py` & `types-peewee-3.17.3.20240424/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,35 +16,39 @@
 
 This version of `types-peewee` aims to provide accurate annotations
 for `peewee==3.17.3`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/peewee. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `57f3dcac8dbed008479b251512975901a0206deb` and was tested
+This package was generated from typeshed commit `7ed91bc2e77ec18d28307dc6086a778ecc9c7bb3` and was tested
 with mypy 1.9.0, pyright 1.1.358, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="3.17.3.20240420",
+      version="3.17.3.20240424",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/peewee.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
-      packages=['peewee-stubs'],
-      package_data={'peewee-stubs': ['__init__.pyi', 'METADATA.toml', 'py.typed']},
+      packages=['playhouse-stubs', 'peewee-stubs'],
+      package_data={'playhouse-stubs': ['__init__.pyi', 'flask_utils.pyi', 'METADATA.toml', 'py.typed'], 'peewee-stubs': ['__init__.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
```

### Comparing `types-peewee-3.17.3.20240420/types_peewee.egg-info/PKG-INFO` & `types-peewee-3.17.3.20240424/types_peewee.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-peewee
-Version: 3.17.3.20240420
+Version: 3.17.3.20240424
 Summary: Typing stubs for peewee
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/peewee.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -27,11 +27,15 @@
 
 This version of `types-peewee` aims to provide accurate annotations
 for `peewee==3.17.3`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/peewee. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `57f3dcac8dbed008479b251512975901a0206deb` and was tested
+This package was generated from typeshed commit `7ed91bc2e77ec18d28307dc6086a778ecc9c7bb3` and was tested
 with mypy 1.9.0, pyright 1.1.358, and
 pytype 2024.4.11.
```

