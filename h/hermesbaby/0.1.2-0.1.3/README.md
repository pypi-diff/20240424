# Comparing `tmp/hermesbaby-0.1.2.tar.gz` & `tmp/hermesbaby-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermesbaby-0.1.2.tar", max compression
+gzip compressed data, was "hermesbaby-0.1.3.tar", max compression
```

## Comparing `hermesbaby-0.1.2.tar` & `hermesbaby-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0      117 2024-04-22 04:05:52.750497 hermesbaby-0.1.2/AUTHORS.rst
--rw-r--r--   0        0        0     1104 2024-04-22 04:07:33.370496 hermesbaby-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0     1694 2024-04-22 04:07:42.126496 hermesbaby-0.1.2/README.rst
--rw-r--r--   0        0        0      704 2024-04-23 04:08:09.563541 hermesbaby-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        1 2024-04-22 04:34:17.510486 hermesbaby-0.1.2/src/hermesbaby/__init__.py
--rw-r--r--   0        0        0      269 2024-04-23 04:06:33.843538 hermesbaby-0.1.2/src/hermesbaby/cli.py
--rw-r--r--   0        0        0     2259 1970-01-01 00:00:00.000000 hermesbaby-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      117 2024-04-22 04:05:52.750497 hermesbaby-0.1.3/AUTHORS.rst
+-rw-r--r--   0        0        0     1104 2024-04-22 04:07:33.370496 hermesbaby-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0      454 2024-04-24 04:32:01.252082 hermesbaby-0.1.3/README.md
+-rw-r--r--   0        0        0      737 2024-04-24 04:44:33.740053 hermesbaby-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        1 2024-04-22 04:34:17.510486 hermesbaby-0.1.3/src/hermesbaby/__init__.py
+-rw-r--r--   0        0        0      269 2024-04-23 04:06:33.843538 hermesbaby-0.1.3/src/hermesbaby/cli.py
+-rw-r--r--   0        0        0        0 2024-04-24 04:30:38.840085 hermesbaby-0.1.3/src/hermesbaby/cmd/__init_.py
+-rw-r--r--   0        0        0      269 2024-04-24 04:30:38.852085 hermesbaby-0.1.3/src/hermesbaby/cmd/hb.py
+-rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 hermesbaby-0.1.3/PKG-INFO
```

### Comparing `hermesbaby-0.1.2/LICENSE.txt` & `hermesbaby-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hermesbaby-0.1.2/pyproject.toml` & `hermesbaby-0.1.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "hermesbaby"
-version = "0.1.2"
+version = "0.1.3"
 description = "The Software Engineers' Typewriter"
 authors = ["Alexander Mann-Wahrenberg (basejumpa) <alexander.mannwahrenberg@gmail.com>"]
 license = "MIT"
-readme = "README.rst"
+readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 sphinx = "^7.3.7"
 
 [tool.poetry.scripts]
+hermesbaby = "hermesbaby.cli:main"
 hb = "hermesbaby.cli:main"
 
 [build-system]
 requires = [
     "poetry-core",
     "setuptools>=46.1.0", 
     "setuptools_scm[toml]>=5"
@@ -22,8 +23,8 @@
 
 # build-backend = "poetry.core.masonry.api"
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 # For smarter version schemes and other configuration options,
 # check out https://github.com/pypa/setuptools_scm
-version_scheme = "no-guess-dev"
+version_scheme = "no-guess-dev"
```

