# Comparing `tmp/git-reviewers-0.8.0.tar.gz` & `tmp/git-reviewers-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/git-reviewers-0.8.0.tar", last modified: Wed Mar 28 05:15:52 2018, max compression
+gzip compressed data, was "dist/git-reviewers-0.9.0.tar", last modified: Wed Jul  4 05:17:03 2018, max compression
```

## Comparing `git-reviewers-0.8.0.tar` & `git-reviewers-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 albertyw  (1000) albertyw  (1000)        0 2018-03-28 05:15:52.000000 git-reviewers-0.8.0/
--rw-rw-r--   0 albertyw  (1000) albertyw  (1000)     4808 2018-03-28 05:15:52.000000 git-reviewers-0.8.0/PKG-INFO
--rw-rw-r--   0 albertyw  (1000) albertyw  (1000)     1888 2018-03-28 05:14:46.000000 git-reviewers-0.8.0/CHANGELOG.md
--rw-rw-r--   0 albertyw  (1000) albertyw  (1000)     3196 2018-03-24 19:12:03.000000 git-reviewers-0.8.0/README.rst
--rw-rw-r--   0 albertyw  (1000) albertyw  (1000)     1889 2017-11-12 02:55:22.000000 git-reviewers-0.8.0/setup.py
--rw-rw-r--   0 albertyw  (1000) albertyw  (1000)       40 2017-11-12 02:55:19.000000 git-reviewers-0.8.0/MANIFEST.in
-drwxrwxr-x   0 albertyw  (1000) albertyw  (1000)        0 2018-03-28 05:15:52.000000 git-reviewers-0.8.0/git_reviewers.egg-info/
--rw-rw-r--   0 albertyw  (1000) albertyw  (1000)      321 2018-03-28 05:15:51.000000 git-reviewers-0.8.0/git_reviewers.egg-info/SOURCES.txt
--rw-rw-r--   0 albertyw  (1000) albertyw  (1000)     4808 2018-03-28 05:15:51.000000 git-reviewers-0.8.0/git_reviewers.egg-info/PKG-INFO
--rw-rw-r--   0 albertyw  (1000) albertyw  (1000)       14 2018-03-28 05:15:51.000000 git-reviewers-0.8.0/git_reviewers.egg-info/top_level.txt
--rw-rw-r--   0 albertyw  (1000) albertyw  (1000)        1 2018-03-28 05:15:51.000000 git-reviewers-0.8.0/git_reviewers.egg-info/dependency_links.txt
--rw-rw-r--   0 albertyw  (1000) albertyw  (1000)       15 2018-03-28 05:15:51.000000 git-reviewers-0.8.0/git_reviewers.egg-info/requires.txt
--rw-rw-r--   0 albertyw  (1000) albertyw  (1000)       64 2018-03-28 05:15:51.000000 git-reviewers-0.8.0/git_reviewers.egg-info/entry_points.txt
--rw-rw-r--   0 albertyw  (1000) albertyw  (1000)       38 2018-03-28 05:15:52.000000 git-reviewers-0.8.0/setup.cfg
-drwxrwxr-x   0 albertyw  (1000) albertyw  (1000)        0 2018-03-28 05:15:52.000000 git-reviewers-0.8.0/git_reviewers/
--rw-rw-r--   0 albertyw  (1000) albertyw  (1000)        0 2017-11-12 02:55:19.000000 git-reviewers-0.8.0/git_reviewers/__init__.py
--rwxrwxr-x   0 albertyw  (1000) albertyw  (1000)     6775 2018-03-28 05:15:05.000000 git-reviewers-0.8.0/git_reviewers/reviewers.py
+drwxrwxr-x   0 albertyw  (1000) albertyw  (1004)        0 2018-07-04 05:17:03.000000 git-reviewers-0.9.0/
+-rw-rw-r--   0 albertyw  (1000) albertyw  (1004)     4801 2018-07-04 05:17:03.000000 git-reviewers-0.9.0/PKG-INFO
+-rw-rw-r--   0 albertyw  (1000) albertyw  (1004)       40 2018-06-30 06:44:38.000000 git-reviewers-0.9.0/MANIFEST.in
+-rw-rw-r--   0 albertyw  (1000) albertyw  (1004)     2018 2018-07-04 05:15:52.000000 git-reviewers-0.9.0/CHANGELOG.md
+drwxrwxr-x   0 albertyw  (1000) albertyw  (1004)        0 2018-07-04 05:17:03.000000 git-reviewers-0.9.0/git_reviewers/
+-rw-rw-r--   0 albertyw  (1000) albertyw  (1004)        0 2018-06-30 06:44:38.000000 git-reviewers-0.9.0/git_reviewers/__init__.py
+-rwxrwxr-x   0 albertyw  (1000) albertyw  (1004)     7082 2018-07-04 05:16:05.000000 git-reviewers-0.9.0/git_reviewers/reviewers.py
+-rw-rw-r--   0 albertyw  (1000) albertyw  (1004)     1889 2018-06-30 06:44:38.000000 git-reviewers-0.9.0/setup.py
+-rw-rw-r--   0 albertyw  (1000) albertyw  (1004)       38 2018-07-04 05:17:03.000000 git-reviewers-0.9.0/setup.cfg
+-rw-rw-r--   0 albertyw  (1000) albertyw  (1004)     3189 2018-06-30 06:44:38.000000 git-reviewers-0.9.0/README.rst
+drwxrwxr-x   0 albertyw  (1000) albertyw  (1004)        0 2018-07-04 05:17:03.000000 git-reviewers-0.9.0/git_reviewers.egg-info/
+-rw-rw-r--   0 albertyw  (1000) albertyw  (1004)     4801 2018-07-04 05:17:03.000000 git-reviewers-0.9.0/git_reviewers.egg-info/PKG-INFO
+-rw-rw-r--   0 albertyw  (1000) albertyw  (1004)       14 2018-07-04 05:17:03.000000 git-reviewers-0.9.0/git_reviewers.egg-info/top_level.txt
+-rw-rw-r--   0 albertyw  (1000) albertyw  (1004)        1 2018-07-04 05:17:03.000000 git-reviewers-0.9.0/git_reviewers.egg-info/dependency_links.txt
+-rw-rw-r--   0 albertyw  (1000) albertyw  (1004)       64 2018-07-04 05:17:03.000000 git-reviewers-0.9.0/git_reviewers.egg-info/entry_points.txt
+-rw-rw-r--   0 albertyw  (1000) albertyw  (1004)      321 2018-07-04 05:17:03.000000 git-reviewers-0.9.0/git_reviewers.egg-info/SOURCES.txt
+-rw-rw-r--   0 albertyw  (1000) albertyw  (1004)       15 2018-07-04 05:17:03.000000 git-reviewers-0.9.0/git_reviewers.egg-info/requires.txt
```

### Comparing `git-reviewers-0.8.0/PKG-INFO` & `git-reviewers-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-reviewers
-Version: 0.8.0
+Version: 0.9.0
 Summary: Suggest reviewers for your git branch
 Home-page: https://github.com/albertyw/git-reviewers
 Author: Albert Wang
 Author-email: git@albertyw.com
 License: MIT
 Description: git-reviewers
         =============
@@ -94,16 +94,16 @@
         
         .. |PyPI| image:: https://img.shields.io/pypi/v/git-reviewers.svg
            :target: https://github.com/albertyw/git-reviewers
         .. |Python Versions| image:: https://img.shields.io/pypi/pyversions/git-reviewers.svg
            :target: https://github.com/albertyw/git-reviewers
         .. |Codeship Status for albertyw/git-reviewers| image:: https://app.codeship.com/projects/17913cd0-3524-0135-2853-7e1f21584d06/status?branch=master
            :target: https://app.codeship.com/projects/227040
-        .. |Dependency Status| image:: https://gemnasium.com/badges/github.com/albertyw/git-reviewers.svg
-           :target: https://gemnasium.com/github.com/albertyw/git-reviewers
+        .. |Dependency Status| image:: https://pyup.io/repos/github/albertyw/git-reviewers/shield.svg
+           :target: https://pyup.io/repos/github/albertyw/git-reviewers/
         .. |Code Climate| image:: https://codeclimate.com/github/albertyw/git-reviewers/badges/gpa.svg
            :target: https://codeclimate.com/github/albertyw/git-reviewers
         .. |Test Coverage| image:: https://codeclimate.com/github/albertyw/git-reviewers/badges/coverage.svg
            :target: https://codeclimate.com/github/albertyw/git-reviewers/coverage
         
 Keywords: git code review reviewer log history
 Platform: UNKNOWN
@@ -113,9 +113,9 @@
 Classifier: Topic :: Software Development :: Version Control
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
-Provides-Extra: test
 Provides-Extra: dev
+Provides-Extra: test
```

### Comparing `git-reviewers-0.8.0/CHANGELOG.md` & `git-reviewers-0.9.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGELOG.md
 ============
 
+v0.9.0 (2018-07-03)
+-------------------
+
+ - Add verbose mode
+ - Fixes for copying data to clipboard
+ - Update test dependencies
+
+
 v0.8.0 (2018-03-27)
 -------------------
 
  - Refactors and optimizations
 
 
 v0.7.0 (2018-03-24)
```

### Comparing `git-reviewers-0.8.0/README.rst` & `git-reviewers-0.9.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -86,13 +86,13 @@
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/git-reviewers.svg
    :target: https://github.com/albertyw/git-reviewers
 .. |Python Versions| image:: https://img.shields.io/pypi/pyversions/git-reviewers.svg
    :target: https://github.com/albertyw/git-reviewers
 .. |Codeship Status for albertyw/git-reviewers| image:: https://app.codeship.com/projects/17913cd0-3524-0135-2853-7e1f21584d06/status?branch=master
    :target: https://app.codeship.com/projects/227040
-.. |Dependency Status| image:: https://gemnasium.com/badges/github.com/albertyw/git-reviewers.svg
-   :target: https://gemnasium.com/github.com/albertyw/git-reviewers
+.. |Dependency Status| image:: https://pyup.io/repos/github/albertyw/git-reviewers/shield.svg
+   :target: https://pyup.io/repos/github/albertyw/git-reviewers/
 .. |Code Climate| image:: https://codeclimate.com/github/albertyw/git-reviewers/badges/gpa.svg
    :target: https://codeclimate.com/github/albertyw/git-reviewers
 .. |Test Coverage| image:: https://codeclimate.com/github/albertyw/git-reviewers/badges/coverage.svg
    :target: https://codeclimate.com/github/albertyw/git-reviewers/coverage
```

### Comparing `git-reviewers-0.8.0/setup.py` & `git-reviewers-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `git-reviewers-0.8.0/git_reviewers.egg-info/PKG-INFO` & `git-reviewers-0.9.0/git_reviewers.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-reviewers
-Version: 0.8.0
+Version: 0.9.0
 Summary: Suggest reviewers for your git branch
 Home-page: https://github.com/albertyw/git-reviewers
 Author: Albert Wang
 Author-email: git@albertyw.com
 License: MIT
 Description: git-reviewers
         =============
@@ -94,16 +94,16 @@
         
         .. |PyPI| image:: https://img.shields.io/pypi/v/git-reviewers.svg
            :target: https://github.com/albertyw/git-reviewers
         .. |Python Versions| image:: https://img.shields.io/pypi/pyversions/git-reviewers.svg
            :target: https://github.com/albertyw/git-reviewers
         .. |Codeship Status for albertyw/git-reviewers| image:: https://app.codeship.com/projects/17913cd0-3524-0135-2853-7e1f21584d06/status?branch=master
            :target: https://app.codeship.com/projects/227040
-        .. |Dependency Status| image:: https://gemnasium.com/badges/github.com/albertyw/git-reviewers.svg
-           :target: https://gemnasium.com/github.com/albertyw/git-reviewers
+        .. |Dependency Status| image:: https://pyup.io/repos/github/albertyw/git-reviewers/shield.svg
+           :target: https://pyup.io/repos/github/albertyw/git-reviewers/
         .. |Code Climate| image:: https://codeclimate.com/github/albertyw/git-reviewers/badges/gpa.svg
            :target: https://codeclimate.com/github/albertyw/git-reviewers
         .. |Test Coverage| image:: https://codeclimate.com/github/albertyw/git-reviewers/badges/coverage.svg
            :target: https://codeclimate.com/github/albertyw/git-reviewers/coverage
         
 Keywords: git code review reviewer log history
 Platform: UNKNOWN
@@ -113,9 +113,9 @@
 Classifier: Topic :: Software Development :: Version Control
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
-Provides-Extra: test
 Provides-Extra: dev
+Provides-Extra: test
```

### Comparing `git-reviewers-0.8.0/git_reviewers/reviewers.py` & `git-reviewers-0.9.0/git_reviewers/reviewers.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import typing  # NOQA
 from typing import List, Tuple
 
 if sys.version_info < (3, 0): # NOQA pragma: no cover
     raise SystemError("Must be using Python 3")
 
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 STRIP_DOMAIN_USERNAMES = ['uber.com']
 REVIEWERS_LIMIT = 7
 
 
 class FindReviewers():
     def get_reviewers(self):  # type: () -> typing.Counter[str]
         """
@@ -134,25 +134,30 @@
     if not copy_clipboard:
         return
     try:
         p = subprocess.Popen(
             ['pbcopy', 'w'],
             stdin=subprocess.PIPE, close_fds=True
         )
-        p.communicate(input=reviewer_string)
+        p.communicate(input=reviewer_string.encode('utf-8'))
     except FileNotFoundError:
         pass
 
 
-def get_reviewers(ignores):  # type: (str) -> List[str]
+def get_reviewers(ignores, verbose):  # type: (str, bool) -> List[str]
     phabricator = False
     finders = [FindLogReviewers, FindArcCommitReviewers]
     reviewers = Counter()  # type: typing.Counter[str]
     for finder in finders:
         finder_reviewers = finder().get_reviewers()
+        if verbose:
+            print(
+                "Reviewers from %s: %s" %
+                (finder.__name__, dict(finder_reviewers))
+            )
         reviewers.update(finder_reviewers)
         if finder == FindArcCommitReviewers and finder_reviewers:
             phabricator = True
 
     reviewers_list = []  # type: List[str]
     ignore_list = ignores.split(',')
     most_common = [x[0] for x in reviewers.most_common()]
@@ -171,22 +176,25 @@
     description = "Suggest reviewers for your diff.\n"
     description += "https://github.com/albertyw/git-reviewers"
     parser = argparse.ArgumentParser(description=description)
     parser.add_argument(
         '-v', '--version', action='version', version=__version__,
     )
     parser.add_argument(
+        '--verbose', default=False, action='store_true', help='verbose mode',
+    )
+    parser.add_argument(
         '-i', '--ignore',
         default='', help='ignore a list of reviewers (comma separated)',
     )
     parser.add_argument(
         '-c', '--copy',
         default=False, action='store_true',
         help='Copy the list of reviewers to clipboard, if available',
     )
     args = parser.parse_args()
-    reviewers_list = get_reviewers(args.ignore)
+    reviewers_list = get_reviewers(args.ignore, args.verbose)
     show_reviewers(reviewers_list, args.copy)
 
 
 if __name__ == "__main__":
     main()
```

