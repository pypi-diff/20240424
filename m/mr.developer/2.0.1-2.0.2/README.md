# Comparing `tmp/mr.developer-2.0.1.tar.gz` & `tmp/mr.developer-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mr.developer-2.0.1.tar", last modified: Wed Aug 19 20:12:51 2020, max compression
+gzip compressed data, was "mr.developer-2.0.2.tar", last modified: Wed Apr 24 19:50:07 2024, max compression
```

## Comparing `mr.developer-2.0.1.tar` & `mr.developer-2.0.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-08-19 20:12:51.000000 mr.developer-2.0.1/
--rw-r--r--   0 maurits    (501) staff       (20)    63465 2020-08-19 20:12:51.000000 mr.developer-2.0.1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)       53 2020-08-19 20:12:51.000000 mr.developer-2.0.1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     4116 2020-08-19 20:12:51.000000 mr.developer-2.0.1/setup.py
--rw-r--r--   0 maurits    (501) staff       (20)      474 2020-08-19 20:12:51.000000 mr.developer-2.0.1/tox.ini
--rw-r--r--   0 maurits    (501) staff       (20)    11611 2020-08-19 20:12:51.000000 mr.developer-2.0.1/HELP.rst
--rw-r--r--   0 maurits    (501) staff       (20)      207 2020-08-19 20:12:51.000000 mr.developer-2.0.1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)    16094 2020-08-19 20:12:51.000000 mr.developer-2.0.1/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)    21759 2020-08-19 20:12:51.000000 mr.developer-2.0.1/CHANGES.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr/developer/
--rw-r--r--   0 maurits    (501) staff       (20)    13888 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr/developer/git.py
--rw-r--r--   0 maurits    (501) staff       (20)      206 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr/developer/compat.py
--rw-r--r--   0 maurits    (501) staff       (20)    15126 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr/developer/svn.py
--rw-r--r--   0 maurits    (501) staff       (20)     1547 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr/developer/filesystem.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr/developer/tests/
--rw-r--r--   0 maurits    (501) staff       (20)    12850 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr/developer/tests/test_extension.py
--rw-r--r--   0 maurits    (501) staff       (20)     1075 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr/developer/tests/conftest.py
--rw-r--r--   0 maurits    (501) staff       (20)     4652 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr/developer/tests/test_common.py
--rw-r--r--   0 maurits    (501) staff       (20)    11011 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr/developer/tests/test_git.py
--rw-r--r--   0 maurits    (501) staff       (20)        2 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr/developer/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3267 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr/developer/tests/test_svn.py
--rw-r--r--   0 maurits    (501) staff       (20)     5536 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr/developer/tests/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     4908 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr/developer/tests/test_commands.py
--rw-r--r--   0 maurits    (501) staff       (20)     4620 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr/developer/tests/test_mercurial.py
--rw-r--r--   0 maurits    (501) staff       (20)    14799 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr/developer/tests/test_git_submodules.py
--rw-r--r--   0 maurits    (501) staff       (20)      147 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr/developer/tests/test_cvs.py
--rw-r--r--   0 maurits    (501) staff       (20)      244 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr/developer/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     7563 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr/developer/mercurial.py
--rw-r--r--   0 maurits    (501) staff       (20)     3942 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr/developer/bazaar.py
--rw-r--r--   0 maurits    (501) staff       (20)     2145 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr/developer/gitsvn.py
--rw-r--r--   0 maurits    (501) staff       (20)    23252 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr/developer/common.py
--rw-r--r--   0 maurits    (501) staff       (20)    11438 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr/developer/extension.py
--rwxr-xr-x   0 maurits    (501) staff       (20)     4534 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr/developer/darcs.py
--rw-r--r--   0 maurits    (501) staff       (20)     7237 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr/developer/cvs.py
--rw-r--r--   0 maurits    (501) staff       (20)     3959 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr/developer/develop.py
--rw-r--r--   0 maurits    (501) staff       (20)    37486 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr/developer/commands.py
--rw-r--r--   0 maurits    (501) staff       (20)      244 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr.developer.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    63465 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr.developer.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)        1 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr.developer.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)       16 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr.developer.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1215 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr.developer.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1235 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr.developer.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       75 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr.developer.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        3 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr.developer.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2020-08-19 20:12:51.000000 mr.developer-2.0.1/src/mr.developer.egg-info/dependency_links.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-24 19:50:07.373812 mr.developer-2.0.2/
+-rw-r--r--   0 maurits    (501) staff       (20)    21869 2024-04-24 19:50:06.000000 mr.developer-2.0.2/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    11611 2024-04-24 19:50:06.000000 mr.developer-2.0.2/HELP.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       53 2024-04-24 19:50:06.000000 mr.developer-2.0.2/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    50397 2024-04-24 19:50:07.374009 mr.developer-2.0.2/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)    15955 2024-04-24 19:50:06.000000 mr.developer-2.0.2/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      207 2024-04-24 19:50:07.374601 mr.developer-2.0.2/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     4116 2024-04-24 19:50:06.000000 mr.developer-2.0.2/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-24 19:50:07.356999 mr.developer-2.0.2/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-24 19:50:07.360407 mr.developer-2.0.2/src/mr/
+-rw-r--r--   0 maurits    (501) staff       (20)      244 2024-04-24 19:50:06.000000 mr.developer-2.0.2/src/mr/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-24 19:50:07.369279 mr.developer-2.0.2/src/mr/developer/
+-rw-r--r--   0 maurits    (501) staff       (20)      244 2024-04-24 19:50:06.000000 mr.developer-2.0.2/src/mr/developer/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3942 2024-04-24 19:50:06.000000 mr.developer-2.0.2/src/mr/developer/bazaar.py
+-rw-r--r--   0 maurits    (501) staff       (20)    37486 2024-04-24 19:50:06.000000 mr.developer-2.0.2/src/mr/developer/commands.py
+-rw-r--r--   0 maurits    (501) staff       (20)    23796 2024-04-24 19:50:06.000000 mr.developer-2.0.2/src/mr/developer/common.py
+-rw-r--r--   0 maurits    (501) staff       (20)      206 2024-04-24 19:50:06.000000 mr.developer-2.0.2/src/mr/developer/compat.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7237 2024-04-24 19:50:06.000000 mr.developer-2.0.2/src/mr/developer/cvs.py
+-rwxr-xr-x   0 maurits    (501) staff       (20)     4534 2024-04-24 19:50:06.000000 mr.developer-2.0.2/src/mr/developer/darcs.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3959 2024-04-24 19:50:06.000000 mr.developer-2.0.2/src/mr/developer/develop.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11438 2024-04-24 19:50:06.000000 mr.developer-2.0.2/src/mr/developer/extension.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1547 2024-04-24 19:50:06.000000 mr.developer-2.0.2/src/mr/developer/filesystem.py
+-rw-r--r--   0 maurits    (501) staff       (20)    13888 2024-04-24 19:50:06.000000 mr.developer-2.0.2/src/mr/developer/git.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2145 2024-04-24 19:50:06.000000 mr.developer-2.0.2/src/mr/developer/gitsvn.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7563 2024-04-24 19:50:06.000000 mr.developer-2.0.2/src/mr/developer/mercurial.py
+-rw-r--r--   0 maurits    (501) staff       (20)    15126 2024-04-24 19:50:06.000000 mr.developer-2.0.2/src/mr/developer/svn.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-24 19:50:07.373591 mr.developer-2.0.2/src/mr/developer/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2024-04-24 19:50:06.000000 mr.developer-2.0.2/src/mr/developer/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1075 2024-04-24 19:50:06.000000 mr.developer-2.0.2/src/mr/developer/tests/conftest.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4956 2024-04-24 19:50:06.000000 mr.developer-2.0.2/src/mr/developer/tests/test_commands.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4652 2024-04-24 19:50:06.000000 mr.developer-2.0.2/src/mr/developer/tests/test_common.py
+-rw-r--r--   0 maurits    (501) staff       (20)      147 2024-04-24 19:50:06.000000 mr.developer-2.0.2/src/mr/developer/tests/test_cvs.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12882 2024-04-24 19:50:06.000000 mr.developer-2.0.2/src/mr/developer/tests/test_extension.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11043 2024-04-24 19:50:06.000000 mr.developer-2.0.2/src/mr/developer/tests/test_git.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14975 2024-04-24 19:50:06.000000 mr.developer-2.0.2/src/mr/developer/tests/test_git_submodules.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4636 2024-04-24 19:50:06.000000 mr.developer-2.0.2/src/mr/developer/tests/test_mercurial.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3283 2024-04-24 19:50:06.000000 mr.developer-2.0.2/src/mr/developer/tests/test_svn.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5552 2024-04-24 19:50:06.000000 mr.developer-2.0.2/src/mr/developer/tests/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-24 19:50:07.363558 mr.developer-2.0.2/src/mr.developer.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    50397 2024-04-24 19:50:07.000000 mr.developer-2.0.2/src/mr.developer.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1215 2024-04-24 19:50:07.000000 mr.developer-2.0.2/src/mr.developer.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-24 19:50:07.000000 mr.developer-2.0.2/src/mr.developer.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1069 2024-04-24 19:50:07.000000 mr.developer-2.0.2/src/mr.developer.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2024-04-24 19:50:07.000000 mr.developer-2.0.2/src/mr.developer.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-24 19:50:07.000000 mr.developer-2.0.2/src/mr.developer.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)       75 2024-04-24 19:50:07.000000 mr.developer-2.0.2/src/mr.developer.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        3 2024-04-24 19:50:07.000000 mr.developer-2.0.2/src/mr.developer.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      474 2024-04-24 19:50:06.000000 mr.developer-2.0.2/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mr.developer-2.0.1/setup.py` & `mr.developer-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pkg_resources import parse_version
 from setuptools import setup
 import sys
 
 
-version = '2.0.1'
+version = '2.0.2'
 
 
 def has_environment_marker_support():
     """
     Tests that setuptools has support for PEP-426 environment marker support.
 
     The first known release to support it is 0.7 (and the earliest on PyPI seems to be 0.7.2
```

### Comparing `mr.developer-2.0.1/HELP.rst` & `mr.developer-2.0.2/HELP.rst`

 * *Files identical despite different names*

### Comparing `mr.developer-2.0.1/README.rst` & `mr.developer-2.0.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 .. contents:: :depth: 1
 
 Introduction
 ============
 
-.. figure:: http://fschulze.github.com/mr.developer/xkcd-buildout.png
+.. figure:: https://fschulze.github.io/mr.developer/xkcd-buildout.png
     :figwidth: image
 
     Let Mr. Developer help you win the everlasting buildout battle!
 
-    (Remixed by Matt Hamilton, original from http://xkcd.com/303)
+    (Remixed by Matt Hamilton, original from https://xkcd.com/303)
 
 **mr.developer** is a `zc.buildout`_ extension that makes it easy to work with
 buildouts containing lots of packages, of which you only want to develop some.
-The basic idea comes from Wichert Akkerman's plonenext_ effort.
+The basic idea comes from Wichert Akkerman's plonenext effort.
 
-.. image:: https://secure.travis-ci.org/fschulze/mr.developer.png
+.. _`zc.buildout`: https://pypi.org/project/zc.buildout/
 
-.. _`zc.buildout`: http://pypi.python.org/pypi/zc.buildout
-.. _plonenext: http://svn.plone.org/svn/plone/plonenext/3.3/README.txt
 
 Usage
 =====
 
 Add ``mr.developer`` to the ``extensions`` entry in your ``[buildout]``
 section::
 
@@ -103,17 +101,17 @@
 
 Common options
   The ``path`` option allows you to set the base directory where the
   package will be checked out. The name of the package will be appended to
   the base path. If ``path`` is not set, ``sources-dir`` is used.
 
   With ``full-path`` you can set the directory where the package will be
-  checked out. This is the actual destination, nothing will be added. As 
+  checked out. This is the actual destination, nothing will be added. As
   an example::
-  
+
     [sources]
     pkg = fs pkg full-path=/path/to/pkg
 
   The ``update`` option allows you to specify whether a package will be
   updated during buildout or not. If it's ``true``, then it will always be
   updated. If it's ``false``, then it will never be updated, even if the
   global ``always-checkout`` option is set.
@@ -129,15 +127,15 @@
   those which start with the prefix.
   These two options currently only work for ``cvs`` and ``hg``.
 
 ``svn``
   The ``url`` is one of the urls supported by subversion.
 
   You can specify a url with a revision pin, like
-  ``http://example.com/trunk@123``.
+  ``https://example.com/trunk@123``.
 
   You can also set the ``rev`` or ``revision`` option, which is either a pin
   like with ``rev=123`` or a minimum revision like ``rev=>123`` or
   ``rev=>=123``. When you set a minimum revision, the repository is updated
   when the current revision is lower.
 
 ``git``
@@ -195,15 +193,15 @@
 Here's an example of how your ``buildout.cfg`` may look like::
 
   [buildout]
   extensions = mr.developer
   auto-checkout = my.package
 
   [sources]
-  my.package = svn http://example.com/svn/my.package/trunk update=true
+  my.package = svn https://example.com/svn/my.package/trunk update=true
   some.other.package = git git://example.com/git/some.other.package.git
 
 When you run buildout, the script ``bin/develop`` is created in your
 buildout directory. With this script you can perform various actions on
 packages, like checking out their source code, without the need to know where
 the repositories are located.
 
@@ -248,15 +246,15 @@
   the rule.
 
 ``~``
   This runs a regular expression substitution. The substitute is read from the
   next line. You can use groups in the expression and the backslash syntax in
   the substitute. See `re.sub`_ documentation.
 
-.. _`re.sub`: http://docs.python.org/2/library/re.html#re.sub
+.. _`re.sub`: https://docs.python.org/3/library/re.html#re.sub
 
 The following are useful examples::
 
   [rewrites]
 
   plone_svn =
     url ~ ^http://svn.plone.org/svn/
```

### Comparing `mr.developer-2.0.1/CHANGES.rst` & `mr.developer-2.0.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 Changelog
 =========
 
 
+2.0.2 (2024-04-24)
+------------------
+
+* Fix ValueError: too many values to unpack (expected 2).  [flipmcf]
+
+
 2.0.1 (2020-08-19)
 ------------------
 
 * Fix ``bin/develop help`` on Python 3.
 
 
 2.0.0 (2019-03-04)
```

### Comparing `mr.developer-2.0.1/src/mr/developer/git.py` & `mr.developer-2.0.2/src/mr/developer/git.py`

 * *Files identical despite different names*

### Comparing `mr.developer-2.0.1/src/mr/developer/svn.py` & `mr.developer-2.0.2/src/mr/developer/svn.py`

 * *Files identical despite different names*

### Comparing `mr.developer-2.0.1/src/mr/developer/filesystem.py` & `mr.developer-2.0.2/src/mr/developer/filesystem.py`

 * *Files identical despite different names*

### Comparing `mr.developer-2.0.1/src/mr/developer/tests/test_extension.py` & `mr.developer-2.0.2/src/mr/developer/tests/test_extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,15 +267,15 @@
         _exists = patch('os.path.exists')
         exists = _exists.__enter__()
         try:
             exists().return_value = True
 
             (develop, develeggs, versions) = extension.get_develop_info()
         finally:
-            _exists.__exit__()
+            _exists.__exit__(None, None, None)
         assert buildout['versions'] == {
             'pkg.foo-bar': '',
             'pkg.bar-foo': '1.0'}
 
     def testDevelopOrder(self, buildout, extension):
         buildout['buildout']['develop'] = '/normal/develop ' \
             '/develop/with/slash/'
@@ -292,15 +292,15 @@
 
         _exists = patch('os.path.exists')
         exists = _exists.__enter__()
         try:
             exists().return_value = True
             (develop, develeggs, versions) = extension.get_develop_info()
         finally:
-            _exists.__exit__()
+            _exists.__exit__(None, None, None)
         assert develop == ['/normal/develop', '/develop/with/slash/', 'src/pkg.bar']
 
     def testMissingSourceSection(self, buildout, extension):
         del buildout['sources']
         assert extension.get_sources() == {}
```

### Comparing `mr.developer-2.0.1/src/mr/developer/tests/conftest.py` & `mr.developer-2.0.2/src/mr/developer/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mr.developer-2.0.1/src/mr/developer/tests/test_common.py` & `mr.developer-2.0.2/src/mr/developer/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `mr.developer-2.0.1/src/mr/developer/tests/test_git.py` & `mr.developer-2.0.2/src/mr/developer/tests/test_git.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
             captured = capsys.readouterr()
             assert captured.out == ""
             CmdStatus(develop)(develop.parser.parse_args(['status', '-v']))
             captured = capsys.readouterr()
             assert captured.out == "~   A egg\n      ## master...origin/master\n\n"
 
         finally:
-            _log.__exit__()
+            _log.__exit__(None, None, None)
 
     def testUpdateVerbose(self, develop, mkgitrepo, src, capsys):
         from mr.developer.commands import CmdCheckout
         from mr.developer.commands import CmdUpdate
         from mr.developer.commands import CmdStatus
         repository = mkgitrepo('repository')
         repository.add_file('foo')
@@ -174,15 +174,15 @@
             # git output varies between versions...
             assert captured.out in [older, newer]
             CmdStatus(develop)(develop.parser.parse_args(['status', '-v']))
             captured = capsys.readouterr()
             assert captured.out == "~   A egg\n      ## master...origin/master\n\n"
 
         finally:
-            _log.__exit__()
+            _log.__exit__(None, None, None)
 
     def testDepthOption(self, mkgitrepo, src, tempdir):
         from mr.developer.develop import develop
 
         # create repository and make two commits on it
         repository = mkgitrepo('repository')
         self.createDefaultContent(repository)
```

### Comparing `mr.developer-2.0.1/src/mr/developer/tests/test_svn.py` & `mr.developer-2.0.2/src/mr/developer/tests/test_svn.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             assert set(os.listdir(src['egg'])) == set(('.svn', 'bar', 'foo'))
             CmdUpdate(develop)(develop.parser.parse_args(['up', 'egg']))
             assert set(os.listdir(src['egg'])) == set(('.svn', 'bar', 'foo'))
             assert log.method_calls == [
                 ('info', ("Checked out 'egg' with subversion.",), {}),
                 ('info', ("Updated 'egg' with subversion.",), {})]
         finally:
-            _log.__exit__()
+            _log.__exit__(None, None, None)
 
     def testUpdateWithRevisionPin(self, develop, src, tempdir):
         from mr.developer.commands import CmdCheckout
         from mr.developer.commands import CmdUpdate
         process = Process()
         repository = tempdir['repository']
         process.check_call("svnadmin create %s" % repository)
```

### Comparing `mr.developer-2.0.1/src/mr/developer/tests/utils.py` & `mr.developer-2.0.2/src/mr/developer/tests/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     )
 
     bt = background_thread(tee2, (process, echo2))
     bt.__enter__()
     try:
         lines = tee(process, echo)
     finally:
-        bt.__exit__()
+        bt.__exit__(None, None, None)
     return process.returncode, lines
 
 
 class On(object):
     """A tee filter printing all lines."""
 
     def __call__(self, line):
```

### Comparing `mr.developer-2.0.1/src/mr/developer/tests/test_commands.py` & `mr.developer-2.0.2/src/mr/developer/tests/test_commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,30 +88,30 @@
         develop.config.develop['bar'] = False
         args = develop.parser.parse_args(args=['deactivate', 'bar'])
         _logger = patch('mr.developer.develop.logger')
         logger = _logger.__enter__()
         try:
             cmd(args)
         finally:
-            _logger.__exit__()
+            _logger.__exit__(None, None, None)
         assert develop.config.develop == dict(
             bar=False,
             foo='auto',
             ham='auto')
         assert logger.mock_calls == []
 
     def testDeactivateActivatedPackage(self, cmd, develop):
         develop.config.develop['bar'] = True
         args = develop.parser.parse_args(args=['deactivate', 'bar'])
         _logger = patch('mr.developer.commands.logger')
         logger = _logger.__enter__()
         try:
             cmd(args)
         finally:
-            _logger.__exit__()
+            _logger.__exit__(None, None, None)
         assert develop.config.develop == dict(
             bar=False,
             foo='auto',
             ham='auto')
         assert logger.mock_calls == [
             ('info', ("Deactivated 'bar'.",), {}),
             ('warn', ("Don't forget to run buildout again, so the deactived packages are actually not used anymore.",), {})]
@@ -119,15 +119,15 @@
     def testDeactivateAutoCheckoutPackage(self, cmd, develop):
         args = develop.parser.parse_args(args=['deactivate', 'foo'])
         _logger = patch('mr.developer.commands.logger')
         logger = _logger.__enter__()
         try:
             cmd(args)
         finally:
-            _logger.__exit__()
+            _logger.__exit__(None, None, None)
         assert develop.config.develop == dict(
             foo=False,
             ham='auto')
         assert logger.mock_calls == [
             ('info', ("Deactivated 'foo'.",), {}),
             ('warn', ("Don't forget to run buildout again, so the deactived packages are actually not used anymore.",), {})]
```

### Comparing `mr.developer-2.0.1/src/mr/developer/tests/test_mercurial.py` & `mr.developer-2.0.2/src/mr/developer/tests/test_mercurial.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             CmdUpdate(develop)(develop.parser.parse_args(['up', 'egg']))
             assert set(os.listdir(os.path.join(src, 'egg'))) == set(('.hg', 'bar', 'foo'))
             assert log.method_calls == [
                 ('info', ("Cloned 'egg' with mercurial.",), {}),
                 ('info', ("Updated 'egg' with mercurial.",), {}),
                 ('info', ("Switched 'egg' to default.",), {})]
         finally:
-            _log.__exit__()
+            _log.__exit__(None, None, None)
 
     def testUpdateWithRevisionPin(self, develop, src, tempdir):
         from mr.developer.commands import CmdCheckout
         from mr.developer.commands import CmdUpdate
         repository = tempdir['repository']
         os.mkdir(repository)
         process = Process(cwd=repository)
```

### Comparing `mr.developer-2.0.1/src/mr/developer/tests/test_git_submodules.py` & `mr.developer-2.0.2/src/mr/developer/tests/test_git_submodules.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             CmdCheckout(develop)(develop.parser.parse_args(['co', 'egg']))
             assert set(os.listdir(src['egg'])) == set(('submodule_a', '.git', 'bar', '.gitmodules'))
             assert set(os.listdir(src['egg/%s' % submodule_name])) == set(('.git', 'foo'))
             assert log.method_calls == [
                 ('info', ("Cloned 'egg' with git from '%s'." % egg.url,), {}),
                 ('info', ("Initialized 'egg' submodule at '%s' with git." % submodule_name,), {})]
         finally:
-            _log.__exit__()
+            _log.__exit__(None, None, None)
 
     def testCheckoutWithTwoSubmodules(self, develop, mkgitrepo, src):
         """
             Tests the checkout of a module 'egg' with a submodule 'submodule_a'
             and a submodule 'submodule_b' in it.
         """
         from mr.developer.commands import CmdCheckout
@@ -67,15 +67,15 @@
             assert set(os.listdir(src['egg/%s' % submodule_name])) == set(('.git', 'foo'))
             assert set(os.listdir(src['egg/%s' % submodule_b_name])) == set(('.git', 'foo_b'))
             assert log.method_calls == [
                 ('info', ("Cloned 'egg' with git from '%s'." % egg.url,), {}),
                 ('info', ("Initialized 'egg' submodule at '%s' with git." % submodule_name,), {}),
                 ('info', ("Initialized 'egg' submodule at '%s' with git." % submodule_b_name,), {})]
         finally:
-            _log.__exit__()
+            _log.__exit__(None, None, None)
 
     def testUpdateWithSubmodule(self, develop, mkgitrepo, src):
         """
             Tests the checkout of a module 'egg' with a submodule 'submodule_a' in it.
             Add a new 'submodule_b' to 'egg' and check it succesfully initializes.
         """
         from mr.developer.commands import CmdCheckout, CmdUpdate
@@ -98,15 +98,15 @@
             CmdCheckout(develop)(develop.parser.parse_args(['co', 'egg']))
             assert set(os.listdir(src['egg'])) == set(('submodule_a', '.git', 'bar', '.gitmodules'))
             assert set(os.listdir(src['egg/%s' % submodule_name])) == set(('.git', 'foo'))
             assert log.method_calls == [
                 ('info', ("Cloned 'egg' with git from '%s'." % egg.url,), {}),
                 ('info', ("Initialized 'egg' submodule at '%s' with git." % submodule_name,), {})]
         finally:
-            _log.__exit__()
+            _log.__exit__(None, None, None)
 
         submodule_b_name = 'submodule_b'
         submodule_b = mkgitrepo(submodule_b_name)
         submodule_b.add_file('foo_b')
         egg.add_submodule(submodule_b, submodule_b_name)
 
         log = _log.__enter__()
@@ -115,15 +115,15 @@
             assert set(os.listdir(src['egg'])) == set(('submodule_a', 'submodule_b', '.git', 'bar', '.gitmodules'))
             assert set(os.listdir(src['egg/%s' % submodule_b_name])) == set(('.git', 'foo_b'))
             assert log.method_calls == [
                 ('info', ("Updated 'egg' with git.",), {}),
                 ('info', ("Switching to branch 'master'.",), {}),
                 ('info', ("Initialized 'egg' submodule at '%s' with git." % submodule_b_name,), {})]
         finally:
-            _log.__exit__()
+            _log.__exit__(None, None, None)
 
     def testCheckoutWithSubmodulesOptionNever(self, develop, mkgitrepo, src):
         """
             Tests the checkout of a module 'egg' with a submodule 'submodule_a' in it
             without initializing the submodule, restricted by global 'never'
         """
 
@@ -147,15 +147,15 @@
         try:
             CmdCheckout(develop)(develop.parser.parse_args(['co', 'egg']))
             assert set(os.listdir(src['egg'])) == set(('submodule_a', '.git', 'bar', '.gitmodules'))
             assert set(os.listdir(src['egg/%s' % submodule_name])) == set()
             assert log.method_calls == [
                 ('info', ("Cloned 'egg' with git from '%s'." % egg.url,), {})]
         finally:
-            _log.__exit__()
+            _log.__exit__(None, None, None)
 
     def testCheckoutWithSubmodulesOptionNeverSourceAlways(self, develop, mkgitrepo, src):
         """
             Tests the checkout of a module 'egg' with a submodule 'submodule_a' in it
             and a module 'egg2' with the same submodule, initializing only the submodule
             on egg that has the 'always' option
         """
@@ -195,15 +195,15 @@
             assert set(os.listdir(src['egg2/%s' % submodule_name])) == set()
 
             assert log.method_calls == [
                 ('info', ("Cloned 'egg' with git from '%s'." % egg.url,), {}),
                 ('info', ("Initialized 'egg' submodule at '%s' with git." % submodule_name,), {}),
                 ('info', ("Cloned 'egg2' with git from '%s'." % egg2.url,), {})]
         finally:
-            _log.__exit__()
+            _log.__exit__(None, None, None)
 
     def testCheckoutWithSubmodulesOptionAlwaysSourceNever(self, develop, mkgitrepo, src):
         """
             Tests the checkout of a module 'egg' with a submodule 'submodule_a' in it
             and a module 'egg2' with the same submodule, not initializing the submodule
             on egg2 that has the 'never' option
 
@@ -242,15 +242,15 @@
             assert set(os.listdir(src['egg2/%s' % submodule_name])) == set()
 
             assert log.method_calls == [
                 ('info', ("Cloned 'egg' with git from '%s'." % egg.url,), {}),
                 ('info', ("Initialized 'egg' submodule at '%s' with git." % submodule_name,), {}),
                 ('info', ("Cloned 'egg2' with git from '%s'." % egg2.url,), {})]
         finally:
-            _log.__exit__()
+            _log.__exit__(None, None, None)
 
     def testUpdateWithSubmoduleCheckout(self, develop, mkgitrepo, src):
         """
             Tests the checkout of a module 'egg' with a submodule 'submodule_a' in it.
             Add a new 'submodule_b' to 'egg' and check it doesn't get initialized.
         """
         from mr.developer.commands import CmdCheckout, CmdUpdate
@@ -274,15 +274,15 @@
             CmdCheckout(develop)(develop.parser.parse_args(['co', 'egg']))
             assert set(os.listdir(src['egg'])) == set(('submodule_a', '.git', 'bar', '.gitmodules'))
             assert set(os.listdir(src['egg/%s' % submodule_name])) == set(('.git', 'foo'))
             assert log.method_calls == [
                 ('info', ("Cloned 'egg' with git from '%s'." % egg.url,), {}),
                 ('info', ("Initialized 'egg' submodule at '%s' with git." % submodule_name,), {})]
         finally:
-            _log.__exit__()
+            _log.__exit__(None, None, None)
 
         submodule_b_name = 'submodule_b'
         submodule_b = mkgitrepo(submodule_b_name)
         submodule_b.add_file('foo_b')
         egg.add_submodule(submodule_b, submodule_b_name)
 
         log = _log.__enter__()
@@ -290,15 +290,15 @@
             CmdUpdate(develop)(develop.parser.parse_args(['up', 'egg']))
             assert set(os.listdir(src['egg'])) == set(('submodule_a', 'submodule_b', '.git', 'bar', '.gitmodules'))
             assert set(os.listdir(src['egg/%s' % submodule_b_name])) == set()
             assert log.method_calls == [
                 ('info', ("Updated 'egg' with git.",), {}),
                 ('info', ("Switching to branch 'master'.",), {})]
         finally:
-            _log.__exit__()
+            _log.__exit__(None, None, None)
 
     def testUpdateWithSubmoduleDontUpdatePreviousSubmodules(self, develop, mkgitrepo, src):
         """
             Tests the checkout of a module 'egg' with a submodule 'submodule_a' in it.
             Commits changes in the detached submodule, and checks update didn't break
             the changes.
         """
@@ -322,23 +322,23 @@
             CmdCheckout(develop)(develop.parser.parse_args(['co', 'egg']))
             assert set(os.listdir(src['egg'])) == set(('submodule_a', '.git', 'bar', '.gitmodules'))
             assert set(os.listdir(src['egg/%s' % submodule_name])) == set(('.git', 'foo'))
             assert log.method_calls == [
                 ('info', ("Cloned 'egg' with git from '%s'." % egg.url,), {}),
                 ('info', ("Initialized 'egg' submodule at '%s' with git." % submodule_name,), {})]
         finally:
-            _log.__exit__()
+            _log.__exit__(None, None, None)
 
         repo = GitRepo(src['egg/%s' % submodule_name])
         repo.setup_user()
         repo.add_file('newfile')
 
         log = _log.__enter__()
         try:
             CmdUpdate(develop)(develop.parser.parse_args(['up', '-f', 'egg']))
             assert set(os.listdir(src['egg'])) == set(('submodule_a', '.git', 'bar', '.gitmodules'))
             assert set(os.listdir(src['egg/%s' % submodule_name])) == set(('.git', 'foo', 'newfile'))
             assert log.method_calls == [
                 ('info', ("Updated 'egg' with git.",), {}),
                 ('info', ("Switching to branch 'master'.",), {})]
         finally:
-            _log.__exit__()
+            _log.__exit__(None, None, None)
```

### Comparing `mr.developer-2.0.1/src/mr/developer/mercurial.py` & `mr.developer-2.0.2/src/mr/developer/mercurial.py`

 * *Files identical despite different names*

### Comparing `mr.developer-2.0.1/src/mr/developer/bazaar.py` & `mr.developer-2.0.2/src/mr/developer/bazaar.py`

 * *Files identical despite different names*

### Comparing `mr.developer-2.0.1/src/mr/developer/gitsvn.py` & `mr.developer-2.0.2/src/mr/developer/gitsvn.py`

 * *Files identical despite different names*

### Comparing `mr.developer-2.0.1/src/mr/developer/common.py` & `mr.developer-2.0.2/src/mr/developer/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -168,22 +168,34 @@
             return
         try:
             output = action(**kwargs)
         except WCError:
             output_lock.acquire()
             for lvl, msg in wc._output:
                 lvl(msg)
-            for l in sys.exc_info()[1].args[0].split('\n'):
-                logger.error(l)
+            for line in sys.exc_info()[1].args[0].split('\n'):
+                logger.error(line)
             working_copies.errors = True
             output_lock.release()
         else:
             output_lock.acquire()
-            for lvl, msg in wc._output:
+
+            # See GitHub issue # 210
+            # wc._output is a list containing n-length tuples which are messages from the thread.
+            # each tuple (item) first position is a logger function
+            # the rest of the tuple is the message. 
+            
+            # In cases where the message tuple has more than 2 elements in it 
+            #  (logger, message, message, ... ) 
+            # then all messages are joined.
+            for item in wc._output:
+                lvl = item[0]
+                msg = ','.join(item[1:])
                 lvl(msg)
+                
             if kwargs.get('verbose', False) and output is not None and output.strip():
                 if six.PY3 and isinstance(output, six.binary_type):
                     output = output.decode('utf8')
                 print(output)
             output_lock.release()
 
 
@@ -329,16 +341,16 @@
             kind = source['kind']
             wc = self.workingcopytypes.get(kind)(source)
             if wc is None:
                 logger.error("Unknown repository type '%s'." % kind)
                 sys.exit(1)
             return wc.matches()
         except WCError:
-            for l in sys.exc_info()[1].args[0].split('\n'):
-                logger.error(l)
+            for line in sys.exc_info()[1].args[0].split('\n'):
+                logger.error(line)
             sys.exit(1)
 
     def status(self, source, **kwargs):
         name = source['name']
         if name not in self.sources:
             logger.error("Status failed. No source defined for '%s'." % name)
             sys.exit(1)
@@ -347,16 +359,16 @@
             kind = source['kind']
             wc = self.workingcopytypes.get(kind)(source)
             if wc is None:
                 logger.error("Unknown repository type '%s'." % kind)
                 sys.exit(1)
             return wc.status(**kwargs)
         except WCError:
-            for l in sys.exc_info()[1].args[0].split('\n'):
-                logger.error(l)
+            for line in sys.exc_info()[1].args[0].split('\n'):
+                logger.error(line)
             sys.exit(1)
 
     def update(self, packages, **kwargs):
         the_queue = queue.Queue()
         for name in packages:
             kw = kwargs.copy()
             if name not in self.sources:
```

### Comparing `mr.developer-2.0.1/src/mr/developer/extension.py` & `mr.developer-2.0.2/src/mr/developer/extension.py`

 * *Files identical despite different names*

### Comparing `mr.developer-2.0.1/src/mr/developer/darcs.py` & `mr.developer-2.0.2/src/mr/developer/darcs.py`

 * *Files identical despite different names*

### Comparing `mr.developer-2.0.1/src/mr/developer/cvs.py` & `mr.developer-2.0.2/src/mr/developer/cvs.py`

 * *Files identical despite different names*

### Comparing `mr.developer-2.0.1/src/mr/developer/develop.py` & `mr.developer-2.0.2/src/mr/developer/develop.py`

 * *Files identical despite different names*

### Comparing `mr.developer-2.0.1/src/mr/developer/commands.py` & `mr.developer-2.0.2/src/mr/developer/commands.py`

 * *Files identical despite different names*

### Comparing `mr.developer-2.0.1/src/mr.developer.egg-info/SOURCES.txt` & `mr.developer-2.0.2/src/mr.developer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

