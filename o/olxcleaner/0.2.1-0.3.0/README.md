# Comparing `tmp/olxcleaner-0.2.1.tar.gz` & `tmp/olxcleaner-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/olxcleaner-0.2.1.tar", last modified: Fri Feb  3 21:36:24 2023, max compression
+gzip compressed data, was "olxcleaner-0.3.0.tar", last modified: Wed Apr 24 16:21:10 2024, max compression
```

## Comparing `olxcleaner-0.2.1.tar` & `olxcleaner-0.3.0.tar`

### file list

```diff
@@ -1,58 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 21:36:24.000000 olxcleaner-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-02-03 21:36:24.000000 olxcleaner-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 21:36:24.000000 olxcleaner-0.2.1/olxcleaner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      119 2023-02-03 21:36:24.000000 olxcleaner-0.2.1/olxcleaner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1348 2023-02-03 21:36:24.000000 olxcleaner-0.2.1/olxcleaner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-02-03 21:36:24.000000 olxcleaner-0.2.1/olxcleaner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     7263 2023-02-03 21:36:24.000000 olxcleaner-0.2.1/olxcleaner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-02-03 21:36:24.000000 olxcleaner-0.2.1/olxcleaner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-03 21:36:24.000000 olxcleaner-0.2.1/olxcleaner.egg-info/dependency_links.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 21:36:24.000000 olxcleaner-0.2.1/olxcleaner/
--rw-r--r--   0 runner    (1001) docker     (122)     1321 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/errorstore.py
--rw-r--r--   0 runner    (1001) docker     (122)     5213 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/reporting.py
--rw-r--r--   0 runner    (1001) docker     (122)     1598 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 21:36:24.000000 olxcleaner-0.2.1/olxcleaner/entries/
--rwxr-xr-x   0 runner    (1001) docker     (122)     6195 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/entries/edxreporter.py
--rw-r--r--   0 runner    (1001) docker     (122)      231 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/entries/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4339 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/entries/edxcleaner.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 21:36:24.000000 olxcleaner-0.2.1/olxcleaner/loader/
--rw-r--r--   0 runner    (1001) docker     (122)    11876 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/loader/xml.py
--rw-r--r--   0 runner    (1001) docker     (122)     6633 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/loader/xml_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2222 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/loader/policy.py
--rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/loader/policy_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      821 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3259 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 21:36:24.000000 olxcleaner-0.2.1/olxcleaner/objects/
--rw-r--r--   0 runner    (1001) docker     (122)     2228 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/objects/lti_consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)      803 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/objects/html.py
--rw-r--r--   0 runner    (1001) docker     (122)    11042 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/objects/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/objects/lti.py
--rw-r--r--   0 runner    (1001) docker     (122)     6392 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/objects/problem.py
--rw-r--r--   0 runner    (1001) docker     (122)     3118 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/objects/course.py
--rw-r--r--   0 runner    (1001) docker     (122)      927 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2496 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/objects/chapter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1696 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/objects/draganddropv2.py
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/objects/wiki.py
--rw-r--r--   0 runner    (1001) docker     (122)     1191 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/objects/discussion.py
--rw-r--r--   0 runner    (1001) docker     (122)     2702 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/objects/vertical.py
--rw-r--r--   0 runner    (1001) docker     (122)      730 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/objects/video.py
--rw-r--r--   0 runner    (1001) docker     (122)     3183 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/objects/sequential.py
--rw-r--r--   0 runner    (1001) docker     (122)     4754 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/objects/openassessment.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-03 21:36:24.000000 olxcleaner-0.2.1/olxcleaner/parser/
--rw-r--r--   0 runner    (1001) docker     (122)    11920 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/parser/policy.py
--rw-r--r--   0 runner    (1001) docker     (122)     2679 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/parser/validators.py
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6311 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/parser/parser_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5868 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/parser/slowvalidators.py
--rw-r--r--   0 runner    (1001) docker     (122)       95 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2437 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/olxcleaner/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)       91 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7263 2023-02-03 21:36:24.000000 olxcleaner-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      450 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/changelog.md
--rw-r--r--   0 runner    (1001) docker     (122)      625 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/wishlist.md
--rw-r--r--   0 runner    (1001) docker     (122)     1915 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/vision.md
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/errors.md
--rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1344 2023-02-03 21:36:21.000000 olxcleaner-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:21:10.130023 olxcleaner-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-04-24 16:21:10.130023 olxcleaner-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/errors.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:21:10.122023 olxcleaner-0.3.0/olxcleaner/
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:21:10.126023 olxcleaner-0.3.0/olxcleaner/entries/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/entries/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4339 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/entries/edxcleaner.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6195 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/entries/edxreporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/errorstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:21:10.126023 olxcleaner-0.3.0/olxcleaner/loader/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/loader/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/loader/policy_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11876 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/loader/xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/loader/xml_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:21:10.130023 olxcleaner-0.3.0/olxcleaner/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/objects/chapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/objects/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/objects/course.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/objects/discussion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/objects/draganddropv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/objects/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/objects/lti.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/objects/lti_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/objects/openassessment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6392 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/objects/problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/objects/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/objects/vertical.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/objects/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/objects/wiki.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:21:10.130023 olxcleaner-0.3.0/olxcleaner/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/parser/parser_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11920 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/parser/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/parser/slowvalidators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/parser/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/olxcleaner/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:21:10.130023 olxcleaner-0.3.0/olxcleaner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6443 2024-04-24 16:21:10.000000 olxcleaner-0.3.0/olxcleaner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-24 16:21:10.000000 olxcleaner-0.3.0/olxcleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 16:21:10.000000 olxcleaner-0.3.0/olxcleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-24 16:21:10.000000 olxcleaner-0.3.0/olxcleaner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-24 16:21:10.000000 olxcleaner-0.3.0/olxcleaner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 16:21:10.000000 olxcleaner-0.3.0/olxcleaner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-24 16:21:10.130023 olxcleaner-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 16:21:10.130023 olxcleaner-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/tests/test_load_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7430 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/tests/test_load_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15384 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16321 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/tests/test_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10086 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/tests/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7366 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/tests/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/vision.md
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-24 16:20:58.000000 olxcleaner-0.3.0/wishlist.md
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `olxcleaner-0.2.1/olxcleaner.egg-info/PKG-INFO` & `olxcleaner-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,140 +1,145 @@
 Metadata-Version: 2.1
 Name: olxcleaner
-Version: 0.2.1
+Version: 0.3.0
 Summary: Tool to scan Open edX courses for various errors
 Home-page: https://github.com/openedx/olxcleaner
 Author: Jolyon Bloomfield
 Author-email: jolyon@mit.edu
 License: LICENSE
-Description: # OLX Cleaner
-        
-        [![Build Status](https://github.com/openedx/olxcleaner/actions/workflows/ci.yml/badge.svg)](https://github.com/openedx/olxcleaner/actions/workflows/ci.yaml) [![Coverage Status](https://codecov.io/gh/jolyonb/olxcleaner/branch/master/graphs/badge.svg)](https://codecov.io/gh/jolyonb/olxcleaner)
-        
-        This library aims to perform two functions:
-        
-        * Parse the XML code for an edX course, loading it into python objects
-        * Validate the objects for errors
-        
-        Based on this, two scripts are provided that leverage the library:
-        
-        * `edx-cleaner` constructs an error report, course tree and course statistics
-        * `edx-reporter` constructs a LaTeX file representation of the course structure
-        
-        Copyright (C) 2018-2019 Jolyon Bloomfield
-        
-        Copyright (C) 2020-2023 The Center for Reimagining Learning, Inc. and Contributors
-        
-        ## Links
-        
-        * [Error Listing](errors.md)
-        * [Wishlist](wishlist.md)
-        * [Vision](vision.md)
-        * [Changelog](changelog.md)
-        * [License](LICENSE)
-        
-        ## Installation
-        
-        This package may be installed from PYPI using `pip install olxcleaner`. It requires python 3.6 or later.
-        
-        ### Repository Installation (advanced) 
-        
-        Clone this repository, and set up a virtual environment for python 3.6 or later. Run `pip install -r requirements.txt` to install the libraries, followed by `pytest` to ensure that all tests are passing as expected.
-        
-        ## edx-cleaner Usage
-        
-        Used to validate OLX (edX XML) code. This is a very light wrapper around the olxcleaner library, but exposes all of the functionality thereof.
-        
-        Basic usage: run `edx-cleaner` in the directory of the course you want to validate.
-        
-        Command-line options:
-        
-        ```text
-        edx-cleaner [-h] 
-                    [-c COURSE]
-                    [-p {1,2,3,4,5,6,7,8}] 
-                    [-t TREE] [-l {0,1,2,3,4}]
-                    [-q] [-e] [-s] [-S]
-                    [-f {0,1,2,3,4}]
-                    [-i IGNORE [IGNORE ...]]
-        ```
-        
-        * `-h`: Display help.
-        * `-c`: Specify the course file to analyze. If not specified, looks for `course.xml` in the current directory. If given a directory, looks for `course.xml` in that directory.
-        * `-p`: Specify the validation level you wish analyze the course at:
-          * 1: Load the course
-          * 2: Load the policy and grading policy
-          * 3: Validate url_names
-          * 4: Merge policy data with course, ensuring that all references are valid
-          * 5: Validate the grading policy
-          * 6: Have every object validate itself
-          * 7: Parse the course for global errors
-          * 8: Parse the course for detailed global errors (default)
-        * `-t TREE`: Specify a file to output the tree structure to.
-        * `-l`: Specify the depth level to output the tree structure to. Only used if the `-t` option is set. 0 = Course, 1 = Chapter, 2 = Sequential, 3 = Vertical, 4 = Content. 
-        * `-q`: Quiet mode. Does not output anything to the screen.
-        * `-e`: Suppress error listing. Implied by `-q`.
-        * `-s`: Suppress summary of errors. Implied by `-q`.
-        * `-S`: Display course statistics (off by default). Overridden by `-q`.
-        * `-f`: Select the error level at which to exit with an error code. 0 = DEBUG, 1 = INFO, 2 = WARNING, 3 = ERROR (default), 4 = NEVER. Exit code is set to `1` if an error at the specified level or higher is present.
-        * `-i`: Specify a space-separated list of error names to ignore. See [Error Listing](errors.md).
-        
-        ## edx-reporter Usage
-        
-        The olxcleaner library includes modules that parse a course into python objects. This can be useful if you want to scan a course to generate a report. We exploit this in `edx-reporter` to generate a LaTeX report of course structure.
-        
-        Basic usage: run `edx-reporter` in the directory of the course you want to generate a report about.
-        
-        Command-line options:
-        
-        ```text
-        edx-reporter.py [-h] 
-                        [-c COURSE]
-                        [-u]
-                        [> latexfile.tex]
-        ```
-        
-        * `-h`: Display help.
-        * `-c`: Specify the course file to analyze. If not specified, looks for `course.xml` in the current directory. If given a directory, looks for `course.xml` in that directory.
-        * `-u`: Include url_names for verticals.
-        * `> latexfile.tex`: Output the report to a file.
-        
-        If you get an error like ``Character cannot be encoded into LaTeX: U+FEFF - `'``, then you have some bad unicode in your `display_name` entries. Look through the LaTeX output for `{\bfseries ?}`, which is what that character is converted into.
-        
-        Once you have generated a latex file, you can compile it into a PDF file by running `pdflatex latexfile.tex`. Note that the latex file can be modified with any text editor; its format should be self-explanatory.
-        
-        ## Library usage
-        
-        The workhorse of the library is `olxcleaner.validate`, which validates a course in a number of steps.
-        
-        ```python
-        olxcleaner.validate(filename, steps=8, ignore=None, allowed_xblocks=None)
-        ```
-        
-        * `filename`: Pass in either the course directory or the path of `course.xml` for the course you wish to validate.
-        * `steps`: Choose how many validation steps you wish to perform:
-            * 1: Load the course
-            * 2: Load the policy and grading policy
-            * 3: Validate `url_name`s
-            * 4: Merge policy data with course, ensuring that all references are valid
-            * 5: Validate the grading policy
-            * 6: Have every object validate itself
-            * 7: Parse the course for global errors
-            * 8: Parse the course for global errors that may be time-consuming to detect
-        * `ignore`: A list of error names to ignore
-        * `allowed_xblocks`: A list of all allowed xblocks that course olx may contain.
-        
-        Returns `EdxCourse`, `ErrorStore`, `url_names` (dictionary `{'url_name': EdxObject}`, or `None` if `steps < 3`)
-        
-        See examples of how to use `olxcleaner.validate` and the objects it returns in `olxcleaner.entries`.
-        
 Keywords: edx
-Platform: UNKNOWN
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Education :: Computer Aided Instruction (CAI)
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: lxml
+Requires-Dist: python-dateutil
+Requires-Dist: pytz
+Requires-Dist: pylatexenc
+
+# OLX Cleaner
+
+[![Build Status](https://github.com/openedx/olxcleaner/actions/workflows/ci.yml/badge.svg)](https://github.com/openedx/olxcleaner/actions/workflows/ci.yaml) [![Coverage Status](https://codecov.io/gh/jolyonb/olxcleaner/branch/master/graphs/badge.svg)](https://codecov.io/gh/jolyonb/olxcleaner)
+
+This library aims to perform two functions:
+
+* Parse the XML code for an edX course, loading it into python objects
+* Validate the objects for errors
+
+Based on this, two scripts are provided that leverage the library:
+
+* `edx-cleaner` constructs an error report, course tree and course statistics
+* `edx-reporter` constructs a LaTeX file representation of the course structure
+
+Copyright (C) 2018-2019 Jolyon Bloomfield
+
+Copyright (C) 2020-2023 The Center for Reimagining Learning, Inc. and Contributors
+
+## Links
+
+* [Error Listing](errors.md)
+* [Wishlist](wishlist.md)
+* [Vision](vision.md)
+* [Changelog](changelog.md)
+* [License](LICENSE)
+
+## Installation
+
+This package may be installed from PYPI using `pip install olxcleaner`. It requires python 3.6 or later.
+
+### Repository Installation (advanced) 
+
+Clone this repository, and set up a virtual environment for python 3.6 or later. Run `pip install -r requirements.txt` to install the libraries, followed by `pytest` to ensure that all tests are passing as expected.
+
+## edx-cleaner Usage
+
+Used to validate OLX (edX XML) code. This is a very light wrapper around the olxcleaner library, but exposes all of the functionality thereof.
+
+Basic usage: run `edx-cleaner` in the directory of the course you want to validate.
+
+Command-line options:
+
+```text
+edx-cleaner [-h] 
+            [-c COURSE]
+            [-p {1,2,3,4,5,6,7,8}] 
+            [-t TREE] [-l {0,1,2,3,4}]
+            [-q] [-e] [-s] [-S]
+            [-f {0,1,2,3,4}]
+            [-i IGNORE [IGNORE ...]]
+```
+
+* `-h`: Display help.
+* `-c`: Specify the course file to analyze. If not specified, looks for `course.xml` in the current directory. If given a directory, looks for `course.xml` in that directory.
+* `-p`: Specify the validation level you wish analyze the course at:
+  * 1: Load the course
+  * 2: Load the policy and grading policy
+  * 3: Validate url_names
+  * 4: Merge policy data with course, ensuring that all references are valid
+  * 5: Validate the grading policy
+  * 6: Have every object validate itself
+  * 7: Parse the course for global errors
+  * 8: Parse the course for detailed global errors (default)
+* `-t TREE`: Specify a file to output the tree structure to.
+* `-l`: Specify the depth level to output the tree structure to. Only used if the `-t` option is set. 0 = Course, 1 = Chapter, 2 = Sequential, 3 = Vertical, 4 = Content. 
+* `-q`: Quiet mode. Does not output anything to the screen.
+* `-e`: Suppress error listing. Implied by `-q`.
+* `-s`: Suppress summary of errors. Implied by `-q`.
+* `-S`: Display course statistics (off by default). Overridden by `-q`.
+* `-f`: Select the error level at which to exit with an error code. 0 = DEBUG, 1 = INFO, 2 = WARNING, 3 = ERROR (default), 4 = NEVER. Exit code is set to `1` if an error at the specified level or higher is present.
+* `-i`: Specify a space-separated list of error names to ignore. See [Error Listing](errors.md).
+
+## edx-reporter Usage
+
+The olxcleaner library includes modules that parse a course into python objects. This can be useful if you want to scan a course to generate a report. We exploit this in `edx-reporter` to generate a LaTeX report of course structure.
+
+Basic usage: run `edx-reporter` in the directory of the course you want to generate a report about.
+
+Command-line options:
+
+```text
+edx-reporter.py [-h] 
+                [-c COURSE]
+                [-u]
+                [> latexfile.tex]
+```
+
+* `-h`: Display help.
+* `-c`: Specify the course file to analyze. If not specified, looks for `course.xml` in the current directory. If given a directory, looks for `course.xml` in that directory.
+* `-u`: Include url_names for verticals.
+* `> latexfile.tex`: Output the report to a file.
+
+If you get an error like ``Character cannot be encoded into LaTeX: U+FEFF - `'``, then you have some bad unicode in your `display_name` entries. Look through the LaTeX output for `{\bfseries ?}`, which is what that character is converted into.
+
+Once you have generated a latex file, you can compile it into a PDF file by running `pdflatex latexfile.tex`. Note that the latex file can be modified with any text editor; its format should be self-explanatory.
+
+## Library usage
+
+The workhorse of the library is `olxcleaner.validate`, which validates a course in a number of steps.
+
+```python
+olxcleaner.validate(filename, steps=8, ignore=None, allowed_xblocks=None)
+```
+
+* `filename`: Pass in either the course directory or the path of `course.xml` for the course you wish to validate.
+* `steps`: Choose how many validation steps you wish to perform:
+    * 1: Load the course
+    * 2: Load the policy and grading policy
+    * 3: Validate `url_name`s
+    * 4: Merge policy data with course, ensuring that all references are valid
+    * 5: Validate the grading policy
+    * 6: Have every object validate itself
+    * 7: Parse the course for global errors
+    * 8: Parse the course for global errors that may be time-consuming to detect
+* `ignore`: A list of error names to ignore
+* `allowed_xblocks`: A list of all allowed xblocks that course olx may contain.
+
+Returns `EdxCourse`, `ErrorStore`, `url_names` (dictionary `{'url_name': EdxObject}`, or `None` if `steps < 3`)
+
+See examples of how to use `olxcleaner.validate` and the objects it returns in `olxcleaner.entries`.
```

### Comparing `olxcleaner-0.2.1/olxcleaner/errorstore.py` & `olxcleaner-0.3.0/olxcleaner/errorstore.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/reporting.py` & `olxcleaner-0.3.0/olxcleaner/reporting.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/exceptions.py` & `olxcleaner-0.3.0/olxcleaner/exceptions.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/entries/edxreporter.py` & `olxcleaner-0.3.0/olxcleaner/entries/edxreporter.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/entries/edxcleaner.py` & `olxcleaner-0.3.0/olxcleaner/entries/edxcleaner.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/loader/xml.py` & `olxcleaner-0.3.0/olxcleaner/loader/xml.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/loader/xml_exceptions.py` & `olxcleaner-0.3.0/olxcleaner/loader/xml_exceptions.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/loader/policy.py` & `olxcleaner-0.3.0/olxcleaner/loader/policy.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/loader/policy_exceptions.py` & `olxcleaner-0.3.0/olxcleaner/loader/policy_exceptions.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/__init__.py` & `olxcleaner-0.3.0/olxcleaner/__init__.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/validate.py` & `olxcleaner-0.3.0/olxcleaner/validate.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/objects/lti_consumer.py` & `olxcleaner-0.3.0/olxcleaner/objects/lti_consumer.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/objects/html.py` & `olxcleaner-0.3.0/olxcleaner/objects/html.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/objects/common.py` & `olxcleaner-0.3.0/olxcleaner/objects/common.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/objects/lti.py` & `olxcleaner-0.3.0/olxcleaner/objects/lti.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/objects/problem.py` & `olxcleaner-0.3.0/olxcleaner/objects/problem.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/objects/course.py` & `olxcleaner-0.3.0/olxcleaner/objects/course.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/objects/__init__.py` & `olxcleaner-0.3.0/olxcleaner/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/objects/chapter.py` & `olxcleaner-0.3.0/olxcleaner/objects/chapter.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/objects/draganddropv2.py` & `olxcleaner-0.3.0/olxcleaner/objects/draganddropv2.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/objects/wiki.py` & `olxcleaner-0.3.0/olxcleaner/objects/wiki.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/objects/discussion.py` & `olxcleaner-0.3.0/olxcleaner/objects/discussion.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/objects/vertical.py` & `olxcleaner-0.3.0/olxcleaner/objects/vertical.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/objects/video.py` & `olxcleaner-0.3.0/olxcleaner/objects/video.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/objects/sequential.py` & `olxcleaner-0.3.0/olxcleaner/objects/sequential.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/objects/openassessment.py` & `olxcleaner-0.3.0/olxcleaner/objects/openassessment.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/parser/policy.py` & `olxcleaner-0.3.0/olxcleaner/parser/policy.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/parser/validators.py` & `olxcleaner-0.3.0/olxcleaner/parser/validators.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/parser/parser_exceptions.py` & `olxcleaner-0.3.0/olxcleaner/parser/parser_exceptions.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/parser/slowvalidators.py` & `olxcleaner-0.3.0/olxcleaner/parser/slowvalidators.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/olxcleaner/utils.py` & `olxcleaner-0.3.0/olxcleaner/utils.py`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/PKG-INFO` & `olxcleaner-0.3.0/olxcleaner.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,140 +1,145 @@
 Metadata-Version: 2.1
 Name: olxcleaner
-Version: 0.2.1
+Version: 0.3.0
 Summary: Tool to scan Open edX courses for various errors
 Home-page: https://github.com/openedx/olxcleaner
 Author: Jolyon Bloomfield
 Author-email: jolyon@mit.edu
 License: LICENSE
-Description: # OLX Cleaner
-        
-        [![Build Status](https://github.com/openedx/olxcleaner/actions/workflows/ci.yml/badge.svg)](https://github.com/openedx/olxcleaner/actions/workflows/ci.yaml) [![Coverage Status](https://codecov.io/gh/jolyonb/olxcleaner/branch/master/graphs/badge.svg)](https://codecov.io/gh/jolyonb/olxcleaner)
-        
-        This library aims to perform two functions:
-        
-        * Parse the XML code for an edX course, loading it into python objects
-        * Validate the objects for errors
-        
-        Based on this, two scripts are provided that leverage the library:
-        
-        * `edx-cleaner` constructs an error report, course tree and course statistics
-        * `edx-reporter` constructs a LaTeX file representation of the course structure
-        
-        Copyright (C) 2018-2019 Jolyon Bloomfield
-        
-        Copyright (C) 2020-2023 The Center for Reimagining Learning, Inc. and Contributors
-        
-        ## Links
-        
-        * [Error Listing](errors.md)
-        * [Wishlist](wishlist.md)
-        * [Vision](vision.md)
-        * [Changelog](changelog.md)
-        * [License](LICENSE)
-        
-        ## Installation
-        
-        This package may be installed from PYPI using `pip install olxcleaner`. It requires python 3.6 or later.
-        
-        ### Repository Installation (advanced) 
-        
-        Clone this repository, and set up a virtual environment for python 3.6 or later. Run `pip install -r requirements.txt` to install the libraries, followed by `pytest` to ensure that all tests are passing as expected.
-        
-        ## edx-cleaner Usage
-        
-        Used to validate OLX (edX XML) code. This is a very light wrapper around the olxcleaner library, but exposes all of the functionality thereof.
-        
-        Basic usage: run `edx-cleaner` in the directory of the course you want to validate.
-        
-        Command-line options:
-        
-        ```text
-        edx-cleaner [-h] 
-                    [-c COURSE]
-                    [-p {1,2,3,4,5,6,7,8}] 
-                    [-t TREE] [-l {0,1,2,3,4}]
-                    [-q] [-e] [-s] [-S]
-                    [-f {0,1,2,3,4}]
-                    [-i IGNORE [IGNORE ...]]
-        ```
-        
-        * `-h`: Display help.
-        * `-c`: Specify the course file to analyze. If not specified, looks for `course.xml` in the current directory. If given a directory, looks for `course.xml` in that directory.
-        * `-p`: Specify the validation level you wish analyze the course at:
-          * 1: Load the course
-          * 2: Load the policy and grading policy
-          * 3: Validate url_names
-          * 4: Merge policy data with course, ensuring that all references are valid
-          * 5: Validate the grading policy
-          * 6: Have every object validate itself
-          * 7: Parse the course for global errors
-          * 8: Parse the course for detailed global errors (default)
-        * `-t TREE`: Specify a file to output the tree structure to.
-        * `-l`: Specify the depth level to output the tree structure to. Only used if the `-t` option is set. 0 = Course, 1 = Chapter, 2 = Sequential, 3 = Vertical, 4 = Content. 
-        * `-q`: Quiet mode. Does not output anything to the screen.
-        * `-e`: Suppress error listing. Implied by `-q`.
-        * `-s`: Suppress summary of errors. Implied by `-q`.
-        * `-S`: Display course statistics (off by default). Overridden by `-q`.
-        * `-f`: Select the error level at which to exit with an error code. 0 = DEBUG, 1 = INFO, 2 = WARNING, 3 = ERROR (default), 4 = NEVER. Exit code is set to `1` if an error at the specified level or higher is present.
-        * `-i`: Specify a space-separated list of error names to ignore. See [Error Listing](errors.md).
-        
-        ## edx-reporter Usage
-        
-        The olxcleaner library includes modules that parse a course into python objects. This can be useful if you want to scan a course to generate a report. We exploit this in `edx-reporter` to generate a LaTeX report of course structure.
-        
-        Basic usage: run `edx-reporter` in the directory of the course you want to generate a report about.
-        
-        Command-line options:
-        
-        ```text
-        edx-reporter.py [-h] 
-                        [-c COURSE]
-                        [-u]
-                        [> latexfile.tex]
-        ```
-        
-        * `-h`: Display help.
-        * `-c`: Specify the course file to analyze. If not specified, looks for `course.xml` in the current directory. If given a directory, looks for `course.xml` in that directory.
-        * `-u`: Include url_names for verticals.
-        * `> latexfile.tex`: Output the report to a file.
-        
-        If you get an error like ``Character cannot be encoded into LaTeX: U+FEFF - `'``, then you have some bad unicode in your `display_name` entries. Look through the LaTeX output for `{\bfseries ?}`, which is what that character is converted into.
-        
-        Once you have generated a latex file, you can compile it into a PDF file by running `pdflatex latexfile.tex`. Note that the latex file can be modified with any text editor; its format should be self-explanatory.
-        
-        ## Library usage
-        
-        The workhorse of the library is `olxcleaner.validate`, which validates a course in a number of steps.
-        
-        ```python
-        olxcleaner.validate(filename, steps=8, ignore=None, allowed_xblocks=None)
-        ```
-        
-        * `filename`: Pass in either the course directory or the path of `course.xml` for the course you wish to validate.
-        * `steps`: Choose how many validation steps you wish to perform:
-            * 1: Load the course
-            * 2: Load the policy and grading policy
-            * 3: Validate `url_name`s
-            * 4: Merge policy data with course, ensuring that all references are valid
-            * 5: Validate the grading policy
-            * 6: Have every object validate itself
-            * 7: Parse the course for global errors
-            * 8: Parse the course for global errors that may be time-consuming to detect
-        * `ignore`: A list of error names to ignore
-        * `allowed_xblocks`: A list of all allowed xblocks that course olx may contain.
-        
-        Returns `EdxCourse`, `ErrorStore`, `url_names` (dictionary `{'url_name': EdxObject}`, or `None` if `steps < 3`)
-        
-        See examples of how to use `olxcleaner.validate` and the objects it returns in `olxcleaner.entries`.
-        
 Keywords: edx
-Platform: UNKNOWN
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Education :: Computer Aided Instruction (CAI)
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: lxml
+Requires-Dist: python-dateutil
+Requires-Dist: pytz
+Requires-Dist: pylatexenc
+
+# OLX Cleaner
+
+[![Build Status](https://github.com/openedx/olxcleaner/actions/workflows/ci.yml/badge.svg)](https://github.com/openedx/olxcleaner/actions/workflows/ci.yaml) [![Coverage Status](https://codecov.io/gh/jolyonb/olxcleaner/branch/master/graphs/badge.svg)](https://codecov.io/gh/jolyonb/olxcleaner)
+
+This library aims to perform two functions:
+
+* Parse the XML code for an edX course, loading it into python objects
+* Validate the objects for errors
+
+Based on this, two scripts are provided that leverage the library:
+
+* `edx-cleaner` constructs an error report, course tree and course statistics
+* `edx-reporter` constructs a LaTeX file representation of the course structure
+
+Copyright (C) 2018-2019 Jolyon Bloomfield
+
+Copyright (C) 2020-2023 The Center for Reimagining Learning, Inc. and Contributors
+
+## Links
+
+* [Error Listing](errors.md)
+* [Wishlist](wishlist.md)
+* [Vision](vision.md)
+* [Changelog](changelog.md)
+* [License](LICENSE)
+
+## Installation
+
+This package may be installed from PYPI using `pip install olxcleaner`. It requires python 3.6 or later.
+
+### Repository Installation (advanced) 
+
+Clone this repository, and set up a virtual environment for python 3.6 or later. Run `pip install -r requirements.txt` to install the libraries, followed by `pytest` to ensure that all tests are passing as expected.
+
+## edx-cleaner Usage
+
+Used to validate OLX (edX XML) code. This is a very light wrapper around the olxcleaner library, but exposes all of the functionality thereof.
+
+Basic usage: run `edx-cleaner` in the directory of the course you want to validate.
+
+Command-line options:
+
+```text
+edx-cleaner [-h] 
+            [-c COURSE]
+            [-p {1,2,3,4,5,6,7,8}] 
+            [-t TREE] [-l {0,1,2,3,4}]
+            [-q] [-e] [-s] [-S]
+            [-f {0,1,2,3,4}]
+            [-i IGNORE [IGNORE ...]]
+```
+
+* `-h`: Display help.
+* `-c`: Specify the course file to analyze. If not specified, looks for `course.xml` in the current directory. If given a directory, looks for `course.xml` in that directory.
+* `-p`: Specify the validation level you wish analyze the course at:
+  * 1: Load the course
+  * 2: Load the policy and grading policy
+  * 3: Validate url_names
+  * 4: Merge policy data with course, ensuring that all references are valid
+  * 5: Validate the grading policy
+  * 6: Have every object validate itself
+  * 7: Parse the course for global errors
+  * 8: Parse the course for detailed global errors (default)
+* `-t TREE`: Specify a file to output the tree structure to.
+* `-l`: Specify the depth level to output the tree structure to. Only used if the `-t` option is set. 0 = Course, 1 = Chapter, 2 = Sequential, 3 = Vertical, 4 = Content. 
+* `-q`: Quiet mode. Does not output anything to the screen.
+* `-e`: Suppress error listing. Implied by `-q`.
+* `-s`: Suppress summary of errors. Implied by `-q`.
+* `-S`: Display course statistics (off by default). Overridden by `-q`.
+* `-f`: Select the error level at which to exit with an error code. 0 = DEBUG, 1 = INFO, 2 = WARNING, 3 = ERROR (default), 4 = NEVER. Exit code is set to `1` if an error at the specified level or higher is present.
+* `-i`: Specify a space-separated list of error names to ignore. See [Error Listing](errors.md).
+
+## edx-reporter Usage
+
+The olxcleaner library includes modules that parse a course into python objects. This can be useful if you want to scan a course to generate a report. We exploit this in `edx-reporter` to generate a LaTeX report of course structure.
+
+Basic usage: run `edx-reporter` in the directory of the course you want to generate a report about.
+
+Command-line options:
+
+```text
+edx-reporter.py [-h] 
+                [-c COURSE]
+                [-u]
+                [> latexfile.tex]
+```
+
+* `-h`: Display help.
+* `-c`: Specify the course file to analyze. If not specified, looks for `course.xml` in the current directory. If given a directory, looks for `course.xml` in that directory.
+* `-u`: Include url_names for verticals.
+* `> latexfile.tex`: Output the report to a file.
+
+If you get an error like ``Character cannot be encoded into LaTeX: U+FEFF - `'``, then you have some bad unicode in your `display_name` entries. Look through the LaTeX output for `{\bfseries ?}`, which is what that character is converted into.
+
+Once you have generated a latex file, you can compile it into a PDF file by running `pdflatex latexfile.tex`. Note that the latex file can be modified with any text editor; its format should be self-explanatory.
+
+## Library usage
+
+The workhorse of the library is `olxcleaner.validate`, which validates a course in a number of steps.
+
+```python
+olxcleaner.validate(filename, steps=8, ignore=None, allowed_xblocks=None)
+```
+
+* `filename`: Pass in either the course directory or the path of `course.xml` for the course you wish to validate.
+* `steps`: Choose how many validation steps you wish to perform:
+    * 1: Load the course
+    * 2: Load the policy and grading policy
+    * 3: Validate `url_name`s
+    * 4: Merge policy data with course, ensuring that all references are valid
+    * 5: Validate the grading policy
+    * 6: Have every object validate itself
+    * 7: Parse the course for global errors
+    * 8: Parse the course for global errors that may be time-consuming to detect
+* `ignore`: A list of error names to ignore
+* `allowed_xblocks`: A list of all allowed xblocks that course olx may contain.
+
+Returns `EdxCourse`, `ErrorStore`, `url_names` (dictionary `{'url_name': EdxObject}`, or `None` if `steps < 3`)
+
+See examples of how to use `olxcleaner.validate` and the objects it returns in `olxcleaner.entries`.
```

### Comparing `olxcleaner-0.2.1/wishlist.md` & `olxcleaner-0.3.0/wishlist.md`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/vision.md` & `olxcleaner-0.3.0/vision.md`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/LICENSE` & `olxcleaner-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/errors.md` & `olxcleaner-0.3.0/errors.md`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/README.md` & `olxcleaner-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `olxcleaner-0.2.1/setup.py` & `olxcleaner-0.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,29 +7,30 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="olxcleaner",
-    version="0.2.1",
+    version="0.3.0",
     author="Jolyon Bloomfield",
     author_email="jolyon@mit.edu",
     description="Tool to scan Open edX courses for various errors",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/openedx/olxcleaner",
     license='LICENSE',
     packages=setuptools.find_packages(exclude=['tests']),
     classifiers=[
         "Intended Audience :: Education",
         "Topic :: Education :: Computer Aided Instruction (CAI)",
         "Development Status :: 4 - Beta",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     keywords='edx',
     install_requires=[
        'lxml',
        'python-dateutil',
```

