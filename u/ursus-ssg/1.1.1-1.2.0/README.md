# Comparing `tmp/ursus_ssg-1.1.1.tar.gz` & `tmp/ursus_ssg-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ursus_ssg-1.1.1.tar", last modified: Fri Oct 13 04:54:15 2023, max compression
+gzip compressed data, was "ursus_ssg-1.2.0.tar", last modified: Wed Apr 24 08:01:13 2024, max compression
```

## Comparing `ursus_ssg-1.1.1.tar` & `ursus_ssg-1.2.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-10-13 04:54:15.867189 ursus_ssg-1.1.1/
--rw-r--r--   0 nicolas    (501) staff       (20)    12971 2023-10-13 04:54:15.866956 ursus_ssg-1.1.1/PKG-INFO
--rw-r--r--   0 nicolas    (501) staff       (20)    12191 2023-08-02 10:26:53.000000 ursus_ssg-1.1.1/README.md
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-10-13 04:54:15.860016 ursus_ssg-1.1.1/bin/
--rwxr-xr-x   0 nicolas    (501) staff       (20)     2363 2023-05-24 19:39:22.000000 ursus_ssg-1.1.1/bin/ursus
--rw-r--r--   0 nicolas    (501) staff       (20)       38 2023-10-13 04:54:15.867237 ursus_ssg-1.1.1/setup.cfg
--rw-r--r--   0 nicolas    (501) staff       (20)     1124 2023-10-13 04:53:36.000000 ursus_ssg-1.1.1/setup.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-10-13 04:54:15.861000 ursus_ssg-1.1.1/ursus/
--rw-r--r--   0 nicolas    (501) staff       (20)     1554 2023-05-24 18:21:49.000000 ursus_ssg-1.1.1/ursus/__init__.py
--rw-r--r--   0 nicolas    (501) staff       (20)     4274 2023-06-28 10:41:08.000000 ursus_ssg-1.1.1/ursus/config.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-10-13 04:54:15.862846 ursus_ssg-1.1.1/ursus/context_processors/
--rw-r--r--   0 nicolas    (501) staff       (20)     1096 2023-06-25 13:27:40.000000 ursus_ssg-1.1.1/ursus/context_processors/__init__.py
--rw-r--r--   0 nicolas    (501) staff       (20)     2523 2023-07-17 10:08:25.000000 ursus_ssg-1.1.1/ursus/context_processors/get_entries.py
--rw-r--r--   0 nicolas    (501) staff       (20)     1609 2023-04-07 09:59:42.000000 ursus_ssg-1.1.1/ursus/context_processors/git_date.py
--rw-r--r--   0 nicolas    (501) staff       (20)      785 2023-06-23 08:56:06.000000 ursus_ssg-1.1.1/ursus/context_processors/image.py
--rw-r--r--   0 nicolas    (501) staff       (20)    16385 2023-08-02 08:34:26.000000 ursus_ssg-1.1.1/ursus/context_processors/markdown.py
--rw-------   0 nicolas    (501) staff       (20)     1203 2023-04-30 06:26:51.000000 ursus_ssg-1.1.1/ursus/context_processors/related.py
--rw-r--r--   0 nicolas    (501) staff       (20)      636 2023-03-21 09:18:09.000000 ursus_ssg-1.1.1/ursus/context_processors/stale.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-10-13 04:54:15.863269 ursus_ssg-1.1.1/ursus/generators/
--rw-r--r--   0 nicolas    (501) staff       (20)     1904 2023-07-02 10:01:21.000000 ursus_ssg-1.1.1/ursus/generators/__init__.py
--rw-r--r--   0 nicolas    (501) staff       (20)     2122 2023-05-02 14:07:06.000000 ursus_ssg-1.1.1/ursus/generators/static.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-10-13 04:54:15.864292 ursus_ssg-1.1.1/ursus/linters/
--rw-r--r--   0 nicolas    (501) staff       (20)     1170 2023-08-08 16:45:10.000000 ursus_ssg-1.1.1/ursus/linters/__init__.py
--rw-r--r--   0 nicolas    (501) staff       (20)     1178 2023-09-27 03:08:45.000000 ursus_ssg-1.1.1/ursus/linters/footnotes.py
--rw-r--r--   0 nicolas    (501) staff       (20)     1222 2023-04-11 15:59:59.000000 ursus_ssg-1.1.1/ursus/linters/images.py
--rw-r--r--   0 nicolas    (501) staff       (20)     6742 2023-04-11 14:46:36.000000 ursus_ssg-1.1.1/ursus/linters/markdown.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-10-13 04:54:15.865507 ursus_ssg-1.1.1/ursus/renderers/
--rw-------   0 nicolas    (501) staff       (20)      628 2023-02-09 22:09:00.000000 ursus_ssg-1.1.1/ursus/renderers/__init__.py
--rw-r--r--   0 nicolas    (501) staff       (20)     2078 2023-06-23 08:56:07.000000 ursus_ssg-1.1.1/ursus/renderers/image.py
--rw-r--r--   0 nicolas    (501) staff       (20)    11290 2023-07-16 18:24:21.000000 ursus_ssg-1.1.1/ursus/renderers/jinja.py
--rw-r--r--   0 nicolas    (501) staff       (20)     2993 2023-09-06 06:38:47.000000 ursus_ssg-1.1.1/ursus/renderers/lunr.py
--rw-r--r--   0 nicolas    (501) staff       (20)     1043 2023-06-20 10:47:27.000000 ursus_ssg-1.1.1/ursus/renderers/sass.py
--rw-r--r--   0 nicolas    (501) staff       (20)     1057 2023-04-11 14:46:55.000000 ursus_ssg-1.1.1/ursus/renderers/static.py
--rw-r--r--   0 nicolas    (501) staff       (20)     1476 2023-05-16 20:18:11.000000 ursus_ssg-1.1.1/ursus/server.py
--rw-r--r--   0 nicolas    (501) staff       (20)    11670 2023-09-23 04:17:18.000000 ursus_ssg-1.1.1/ursus/utils.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-10-13 04:54:15.866632 ursus_ssg-1.1.1/ursus_ssg.egg-info/
--rw-r--r--   0 nicolas    (501) staff       (20)    12971 2023-10-13 04:54:15.000000 ursus_ssg-1.1.1/ursus_ssg.egg-info/PKG-INFO
--rw-r--r--   0 nicolas    (501) staff       (20)      855 2023-10-13 04:54:15.000000 ursus_ssg-1.1.1/ursus_ssg.egg-info/SOURCES.txt
--rw-r--r--   0 nicolas    (501) staff       (20)        1 2023-10-13 04:54:15.000000 ursus_ssg-1.1.1/ursus_ssg.egg-info/dependency_links.txt
--rw-r--r--   0 nicolas    (501) staff       (20)        1 2023-08-02 08:41:25.000000 ursus_ssg-1.1.1/ursus_ssg.egg-info/not-zip-safe
--rw-r--r--   0 nicolas    (501) staff       (20)      268 2023-10-13 04:54:15.000000 ursus_ssg-1.1.1/ursus_ssg.egg-info/requires.txt
--rw-r--r--   0 nicolas    (501) staff       (20)        6 2023-10-13 04:54:15.000000 ursus_ssg-1.1.1/ursus_ssg.egg-info/top_level.txt
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-04-24 08:01:13.933506 ursus_ssg-1.2.0/
+-rw-r--r--   0 nicolas    (501) staff       (20)    12981 2024-04-24 08:01:13.933285 ursus_ssg-1.2.0/PKG-INFO
+-rw-r--r--   0 nicolas    (501) staff       (20)    12191 2023-08-02 10:26:53.000000 ursus_ssg-1.2.0/README.md
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-04-24 08:01:13.925346 ursus_ssg-1.2.0/bin/
+-rwxr-xr-x   0 nicolas    (501) staff       (20)     2654 2024-03-01 09:08:21.000000 ursus_ssg-1.2.0/bin/ursus
+-rw-r--r--   0 nicolas    (501) staff       (20)       38 2024-04-24 08:01:13.933545 ursus_ssg-1.2.0/setup.cfg
+-rw-r--r--   0 nicolas    (501) staff       (20)     1619 2024-04-24 07:46:29.000000 ursus_ssg-1.2.0/setup.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-04-24 08:01:13.926607 ursus_ssg-1.2.0/ursus/
+-rw-r--r--   0 nicolas    (501) staff       (20)     1776 2023-12-18 22:05:19.000000 ursus_ssg-1.2.0/ursus/__init__.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     5303 2024-04-23 16:19:59.000000 ursus_ssg-1.2.0/ursus/config.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-04-24 08:01:13.928787 ursus_ssg-1.2.0/ursus/context_processors/
+-rw-r--r--   0 nicolas    (501) staff       (20)     1096 2023-06-25 13:27:40.000000 ursus_ssg-1.2.0/ursus/context_processors/__init__.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     2523 2023-07-17 10:08:25.000000 ursus_ssg-1.2.0/ursus/context_processors/get_entries.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     1747 2024-04-09 07:37:31.000000 ursus_ssg-1.2.0/ursus/context_processors/git_date.py
+-rw-r--r--   0 nicolas    (501) staff       (20)      785 2023-06-23 08:56:06.000000 ursus_ssg-1.2.0/ursus/context_processors/image.py
+-rw-r--r--   0 nicolas    (501) staff       (20)    11253 2024-04-23 16:00:53.000000 ursus_ssg-1.2.0/ursus/context_processors/markdown.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     1374 2023-10-31 11:36:53.000000 ursus_ssg-1.2.0/ursus/context_processors/related.py
+-rw-r--r--   0 nicolas    (501) staff       (20)      636 2023-03-21 09:18:09.000000 ursus_ssg-1.2.0/ursus/context_processors/stale.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-04-24 08:01:13.929334 ursus_ssg-1.2.0/ursus/generators/
+-rw-r--r--   0 nicolas    (501) staff       (20)     1904 2023-07-02 10:01:21.000000 ursus_ssg-1.2.0/ursus/generators/__init__.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     2122 2023-05-02 14:07:06.000000 ursus_ssg-1.2.0/ursus/generators/static.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-04-24 08:01:13.930430 ursus_ssg-1.2.0/ursus/linters/
+-rw-r--r--   0 nicolas    (501) staff       (20)     1170 2023-08-08 16:45:10.000000 ursus_ssg-1.2.0/ursus/linters/__init__.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     1178 2023-09-27 03:08:45.000000 ursus_ssg-1.2.0/ursus/linters/footnotes.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     1171 2023-12-18 21:47:50.000000 ursus_ssg-1.2.0/ursus/linters/images.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     6614 2024-04-23 16:05:23.000000 ursus_ssg-1.2.0/ursus/linters/markdown.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-04-24 08:01:13.931812 ursus_ssg-1.2.0/ursus/renderers/
+-rw-------   0 nicolas    (501) staff       (20)      628 2023-02-09 22:09:00.000000 ursus_ssg-1.2.0/ursus/renderers/__init__.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     2207 2024-04-09 05:18:25.000000 ursus_ssg-1.2.0/ursus/renderers/image.py
+-rw-r--r--   0 nicolas    (501) staff       (20)    11290 2023-07-16 18:24:21.000000 ursus_ssg-1.2.0/ursus/renderers/jinja.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     2993 2023-09-06 06:38:47.000000 ursus_ssg-1.2.0/ursus/renderers/lunr.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     1043 2023-06-20 10:47:27.000000 ursus_ssg-1.2.0/ursus/renderers/sass.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     2257 2024-04-08 06:07:10.000000 ursus_ssg-1.2.0/ursus/renderers/static.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     1648 2024-03-02 00:58:56.000000 ursus_ssg-1.2.0/ursus/server.py
+-rw-r--r--   0 nicolas    (501) staff       (20)    11670 2024-04-23 15:15:15.000000 ursus_ssg-1.2.0/ursus/utils.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2024-04-24 08:01:13.933048 ursus_ssg-1.2.0/ursus_ssg.egg-info/
+-rw-r--r--   0 nicolas    (501) staff       (20)    12981 2024-04-24 08:01:13.000000 ursus_ssg-1.2.0/ursus_ssg.egg-info/PKG-INFO
+-rw-r--r--   0 nicolas    (501) staff       (20)      891 2024-04-24 08:01:13.000000 ursus_ssg-1.2.0/ursus_ssg.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)        1 2024-04-24 08:01:13.000000 ursus_ssg-1.2.0/ursus_ssg.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)      363 2024-04-24 08:01:13.000000 ursus_ssg-1.2.0/ursus_ssg.egg-info/entry_points.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)        1 2023-08-02 08:41:25.000000 ursus_ssg-1.2.0/ursus_ssg.egg-info/not-zip-safe
+-rw-r--r--   0 nicolas    (501) staff       (20)      268 2024-04-24 08:01:13.000000 ursus_ssg-1.2.0/ursus_ssg.egg-info/requires.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)        6 2024-04-24 08:01:13.000000 ursus_ssg-1.2.0/ursus_ssg.egg-info/top_level.txt
```

### Comparing `ursus_ssg-1.1.1/PKG-INFO` & `ursus_ssg-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ursus_ssg
-Version: 1.1.1
+Version: 1.2.0
 Summary: Static site generator
-Home-page: http://github.com/nicbou/ursus
+Home-page: http://github.com/all-about-berlin/ursus
 Author: Nicolas Bouliane
 Author-email: contact@nicolasbouliane.com
 License: MIT
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: coloredlogs==15.0.1
 Requires-Dist: GitPython==3.1.30
```

### Comparing `ursus_ssg-1.1.1/README.md` & `ursus_ssg-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ursus_ssg-1.1.1/bin/ursus` & `ursus_ssg-1.2.0/bin/ursus`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 from pathlib import Path
 from ursus import build, lint
 from ursus.config import config
-from ursus.server import serve_async
+from ursus.server import serve, serve_async
 from ursus.utils import import_module_or_path
 import argparse
 import coloredlogs
 import logging
 
 
 if __name__ == '__main__':
@@ -23,26 +23,30 @@
         help='Action to perform.'
     )
     parser.add_argument(
         '-c', '--config',
         help="Path to a Python config file or module. The `config` variable will be imported from that file."
     )
     parser.add_argument(
-        '-w', '--watch', action='store_true',
-        help="Regenerate files when <content_path> and <templates_path> change."
-    )
-    parser.add_argument(
         '-f', '--fast', action='store_true',
         help="Fast rebuilds. Prefer faster page rebuilds to completeness. Related pages might not be reloaded."
     )
     parser.add_argument(
+        '--level', default='INFO',
+        help="Log level for ursus lint (INFO, WARNING, ERROR). Errors below this level are ignored."
+    )
+    parser.add_argument(
         '-s', '--serve', dest='port', nargs='?', const=80, default=None,
         help="Start a static file server, and serve the generated website on the given port. The default port is 80."
     )
     parser.add_argument(
+        '-w', '--watch', action='store_true',
+        help="Regenerate files when <content_path> and <templates_path> change."
+    )
+    parser.add_argument(
         'files', type=Path, nargs='*',
         help="Only lint the given file(s)"
     )
     args = parser.parse_args()
 
     if args.config:
         import_module_or_path(args.config)
@@ -57,18 +61,20 @@
     if args.config:
         logging.info(f"Loaded config from {args.config}")
     elif Path('./ursus_config.py').exists():
         logging.info("Loaded config from ./ursus_config.py")
     else:
         logging.warning("No config supplied. Using default config.")
 
-    logging.info(f"Content path: {str(config.content_path)}")
-    logging.info(f"Templates path: {str(config.templates_path)}")
-    logging.info(f"Output path: {str(config.output_path)}")
-
     if args.port:
-        serve_async(args.port)
+        if args.watch:
+            serve_async(args.port)
+        else:
+            serve(args.port)
 
+    logging.info(f"Content path: {str(config.content_path)}")
     if args.action == 'build':
+        logging.info(f"Templates path: {str(config.templates_path)}")
+        logging.info(f"Output path: {str(config.output_path)}")
         build(args.watch)
     elif args.action == 'lint':
-        lint(files_to_lint=args.files or None)
+        lint(files_to_lint=args.files or None, min_level=getattr(logging, args.level))
```

### Comparing `ursus_ssg-1.1.1/setup.py` & `ursus_ssg-1.2.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name='ursus_ssg',
-    version='1.1.1',
+    version='1.2.0',
     description='Static site generator',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='http://github.com/nicbou/ursus',
+    url='http://github.com/all-about-berlin/ursus',
     author='Nicolas Bouliane',
     author_email='contact@nicolasbouliane.com',
     license='MIT',
     packages=find_packages(),
     scripts=['bin/ursus'],
+    entry_points={
+        'markdown.extensions': [
+            'better_footnotes = ursus.context_processors.markdown:FootnotesExtension',
+            'jinja = ursus.context_processors.markdown:JinjaExtension',
+            'responsive_images = ursus.context_processors.markdown:ResponsiveImagesExtension',
+            'superscript = ursus.context_processors.markdown:SuperscriptExtension',
+            'tasklist = ursus.context_processors.markdown:TaskListExtension',
+        ]
+    },
     python_requires='>=3.11',
     install_requires=[
         'coloredlogs==15.0.1',
         'GitPython==3.1.30',
         'imagesize==1.4.1',
         'Jinja2==3.1.2',
         'jinja2-simple-tags==0.5.0',
```

### Comparing `ursus_ssg-1.1.1/ursus/context_processors/__init__.py` & `ursus_ssg-1.2.0/ursus/context_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `ursus_ssg-1.1.1/ursus/context_processors/get_entries.py` & `ursus_ssg-1.2.0/ursus/context_processors/get_entries.py`

 * *Files identical despite different names*

### Comparing `ursus_ssg-1.1.1/ursus/context_processors/git_date.py` & `ursus_ssg-1.2.0/ursus/context_processors/git_date.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import datetime
+from datetime import datetime, timezone
 from pathlib import Path
 from ursus.config import config
 from ursus.context_processors import ContextProcessor
 import git
 
 
 class GitDateProcessor(ContextProcessor):
@@ -21,18 +21,19 @@
             return str(abs_commit_path.relative_to(config.content_path))
         except ValueError:
             return None
 
     def process(self, context: dict, changed_files: set = None) -> dict:
         if not config.fast_rebuilds:
             for commit in self.repo.iter_commits("master"):
-                commit_date = datetime.fromtimestamp(commit.authored_date)
+                commit_date = datetime.fromtimestamp(commit.authored_date, tz=timezone.utc)
                 for file in self.repo.git.show(commit.hexsha, name_only=True, diff_filter='ACMR').split('\n'):
                     entry_uri = self.commit_path_to_entry_uri(file)
                     if entry_uri and entry_uri in context['entries']:
                         entry = context['entries'][entry_uri]
                         if not entry.get('date_updated') or commit_date > entry['date_updated']:
-                            entry['date_updated'] = commit_date
+                            # Make the date timezone-aware, then convert it to the local timezone
+                            entry['date_updated'] = commit_date.astimezone()
 
         for entry in context['entries'].values():
             entry.setdefault('date_updated', datetime.now())
         return context
```

### Comparing `ursus_ssg-1.1.1/ursus/context_processors/image.py` & `ursus_ssg-1.2.0/ursus/context_processors/image.py`

 * *Files identical despite different names*

### Comparing `ursus_ssg-1.1.1/ursus/context_processors/markdown.py` & `ursus_ssg-1.2.0/ursus/context_processors/markdown.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 from . import EntryContextProcessor
 from datetime import datetime
 from markdown.extensions import Extension
 from markdown.extensions.footnotes import FootnoteExtension, FN_BACKLINK_TEXT, NBSP_PLACEHOLDER
-from markdown.extensions.smarty import SubstituteTextPattern
-from markdown.extensions.toc import TocExtension, slugify
-from markdown.extensions.wikilinks import WikiLinkExtension, build_url
 from markdown.inlinepatterns import SimpleTagPattern
 from markdown.postprocessors import RawHtmlPostprocessor
 from markdown.preprocessors import Preprocessor
-from markdown.treeprocessors import Treeprocessor, InlineProcessor
-from markdown.extensions.codehilite import CodeHiliteExtension
+from markdown.treeprocessors import Treeprocessor
 from pathlib import Path
 from ursus.config import config
 from ursus.utils import make_figure_element, make_picture_element
 from xml.etree import ElementTree
 import logging
 import markdown
 import re
@@ -64,42 +60,14 @@
         }
         super().__init__(**kwargs)
 
     def extendMarkdown(self, md):
         md.treeprocessors.register(TaskListProcessor(self), "gfm-tasklist", 100)
 
 
-class TypographyExtension(Extension):
-    """
-    Minor typographic improvements
-    """
-    def extendMarkdown(self, md):
-        inline_processor = InlineProcessor(md)
-
-        sectionPattern = SubstituteTextPattern(r'§ ', ('§&nbsp;',), md)
-        inline_processor.inlinePatterns.register(sectionPattern, 'typo-section', 10)
-
-        arrowPattern = SubstituteTextPattern(r' ➞', ('&nbsp;➞',), md)
-        inline_processor.inlinePatterns.register(arrowPattern, 'typo-arrow', 10)
-
-        ellipsisPattern = SubstituteTextPattern(r'\.\.\.', ('&hellip;',), md)
-        inline_processor.inlinePatterns.register(ellipsisPattern, 'typo-ellipsis', 10)
-
-        ellipsisPattern = SubstituteTextPattern(r' - ', ('&nbsp;–&nbsp;',), md)
-        inline_processor.inlinePatterns.register(ellipsisPattern, 'typo-emdash', 10)
-
-        squaredPattern = SubstituteTextPattern(r'\^2\^', ('²',), md)
-        inline_processor.inlinePatterns.register(squaredPattern, 'squared', 65)
-
-        cubedPattern = SubstituteTextPattern(r'\^3\^', ('³',), md)
-        inline_processor.inlinePatterns.register(cubedPattern, 'cubed', 65)
-
-        md.treeprocessors.register(inline_processor, 'typography', 2)
-
-
 class JinjaPreprocessor(Preprocessor):
     """
     Ignore Jinja {{ ... }} and {% ... %} tags.
     """
     JINJA_RE = re.compile('({{([^}]+)}})|({%([^}]+)%})', re.MULTILINE | re.DOTALL)
 
     def run(self, lines):
@@ -131,48 +99,14 @@
     """
     def extendMarkdown(self, md):
         md.postprocessors.deregister('raw_html')
         md.preprocessors.register(JinjaPreprocessor(md), 'jinja', 25)
         md.postprocessors.register(JinjaHtmlPostProcessor(md), 'raw_html', 30)
 
 
-class JinjaCurrencyPreprocessor(Preprocessor):
-    """
-    Wraps jinja template variables followed with "€" in a <span class="currency"> tag
-    """
-    JINJA_RE = re.compile('({{([^}]+)}})€', re.MULTILINE | re.DOTALL)
-
-    def run(self, lines):
-        text = "\n".join(lines)
-
-        def replace_match(match):
-            placeholder = self.md.htmlStash.store(f'<span class="currency">{match[1]}</span>€')
-            return placeholder
-
-        return re.sub(self.JINJA_RE, replace_match, text).split("\n")
-
-
-class CurrencyExtension(Extension):
-    """
-    Wraps currency in a <span class="currency"> tag
-    """
-    def extendMarkdown(self, md):
-        inline_processor = InlineProcessor(md)
-
-        # 1,234.56€
-        currencyPattern = SubstituteTextPattern(
-            r'((\d+(,\d{3})*(\.\d{2})?))€',
-            ('<span class="currency">', 1, '</span>€'), md
-        )
-        inline_processor.inlinePatterns.register(currencyPattern, 'currency', 65)
-        md.treeprocessors.register(inline_processor, 'currency', 2)
-
-        md.preprocessors.register(JinjaCurrencyPreprocessor(md), 'jinja-cur', 26)
-
-
 class ResponsiveImageProcessor(Treeprocessor):
     allowed_parents = (
         'a', 'p', 'pre', 'ul', 'ol', 'dl', 'div', 'blockquote', 'noscript', 'section', 'nav', 'article',
         'aside', 'header', 'footer', 'table', 'form', 'fieldset', 'menu', 'canvas', 'details'
     )
 
     def _swap_element(self, parent, old, new):
@@ -270,76 +204,29 @@
         self.reset()
         md.treeprocessors.register(ResponsiveImageProcessor(md), 'figure', 0)
 
     def reset(self):
         pass
 
 
-class WrappedTableProcessor(Treeprocessor):
-    """
-    Wrap tables in a <div> to allow scrollable tables on mobile.
-    """
-    def wrap_table(self, table, parent):
-        wrapper = ElementTree.Element('div', attrib={
-            'class': self.md.getConfig('table_wrapper_class')
-        })
-        wrapper.append(table)
-
-        for index, element in enumerate(parent):
-            if element == table:
-                parent[index] = wrapper
-                wrapper.tail = table.tail
-                return
-
-    def run(self, root):
-        parent_map = {}
-        for parent in root.iter():
-            for child in parent:
-                parent_map[child] = parent
-
-        for table in root.iter('table'):
-            child = table
-            parents = []
-            while parent := parent_map.get(child):
-                parents.append(parent)
-                child = parent
-
-            self.wrap_table(table, parents[0])
-
-
-class WrappedTableExtension(Extension):
-    """
-    Tables are wrapped in a <div>
-    """
-    def __init__(self, **kwargs):
-        self.config = {
-            "table_wrapper_class": ['', 'CSS class to add to the <div> element that wraps the table'],
-        }
-        super().__init__(**kwargs)
-
-    def extendMarkdown(self, md):
-        if self.getConfig('table_wrapper_class'):
-            md.treeprocessors.register(WrappedTableProcessor(self), 'wrappedtable', 0)
-
-
 class SuperscriptExtension(Extension):
     """
     ^text^ is converted to <sup>text</sup>
     """
 
     # match ^, at least one character that is not ^, and ^ again
     SUPERSCRIPT_RE = r"(\^)([^\^]+)\2"
 
     def extendMarkdown(self, md):
         """Insert 'superscript' pattern before 'not_strong' pattern (priority 70)."""
 
         md.inlinePatterns.register(SimpleTagPattern(self.SUPERSCRIPT_RE, "sup"), 'superscript', 60)
 
 
-class CustomFootnotesExtension(FootnoteExtension):
+class FootnotesExtension(FootnoteExtension):
     def extendMarkdown(self, md):
         super().extendMarkdown(md)
 
     def makeFootnotesDiv(self, root):
         if not list(self.footnotes.keys()):
             return None
 
@@ -381,76 +268,47 @@
                 else:
                     p = ElementTree.SubElement(li, "p")
                     p.append(backlink)
 
         return container
 
 
-def patched_slugify(value, separator, keep_unicode=False):
-    return slugify(value.lstrip(' 0123456789'), separator, keep_unicode)
-
-
 class MarkdownProcessor(EntryContextProcessor):
     def __init__(self):
         super().__init__()
 
         self.markdown = markdown.Markdown(
             output_format='html',
-            extensions=[
-                'fenced_code',
-                'meta',
-                'tables',
-                'smarty',
-                CodeHiliteExtension(guess_lang=False),
-                TocExtension(slugify=patched_slugify),
-                CustomFootnotesExtension(BACKLINK_TEXT="⤴"),
-                JinjaExtension(),
-                SuperscriptExtension(),
-                TypographyExtension(),
-                CurrencyExtension(),
-                ResponsiveImagesExtension(),
-                WikiLinkExtension(
-                    base_url=config.wikilinks_base_url + '/',
-                    end_url=config.wikilinks_url_suffix,
-                    build_url=config.wikilinks_url_builder or build_url,
-                    html_class=config.wikilinks_html_class,
-                ),
-                TaskListExtension(
-                    list_item_class=config.checkbox_list_item_class,
-                    checkbox_class=config.checkbox_list_item_input_class,
-                ),
-                WrappedTableExtension(
-                    table_wrapper_class=config.table_wrapper_class,
-                )
-            ]
+            extensions=list(config.markdown_extensions.keys()),
+            extension_configs=config.markdown_extensions,
         )
 
     def _parse_metadata(self, raw_metadata):
         metadata = {}
         for key, value in raw_metadata.items():
             if len(value) == 0:
                 continue
             if len(value) == 1:
                 value = value[0]
 
             if key.startswith('date_'):
-                value = datetime.strptime(value, '%Y-%m-%d')
+                value = datetime.strptime(value, '%Y-%m-%d').astimezone()
 
             if key.startswith('related_'):
                 if type(value) == list:
                     values = list(filter(bool, [v.strip() for v in value]))
                 else:
                     values = [v.strip() for v in value.split(',')]
                 value = values if len(values) > 1 else values[0]
 
             metadata[key] = value
         return metadata
 
     def process_entry(self, context: dict, entry_uri: str):
-        if entry_uri.endswith('.md'):
+        if entry_uri.lower().endswith('.md'):
             with (config.content_path / entry_uri).open(encoding='utf-8') as f:
                 self.markdown.context = context
                 html = self.markdown.reset().convert(f.read())
 
             context['entries'][entry_uri].update({
                 **self._parse_metadata(self.markdown.Meta),
                 'body': html,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ursus_ssg-1.1.1/ursus/context_processors/related.py` & `ursus_ssg-1.2.0/ursus/context_processors/related.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import UserDict
 from . import ContextProcessor
+import sys
 
 
 class RelatedEntriesProcessor(ContextProcessor):
     """
     Entry fields that start with related_* return a list of entries, instead of
     a list of entry URIs.
     """
@@ -11,18 +12,21 @@
         def __init__(self, entry, all_entries):
             self.all_entries = all_entries
             super().__init__(entry)
 
         def __getitem__(self, key):
             if key.startswith('related_') and key in self.data:
                 related_value = self.data[key]
-                if isinstance(related_value, str):  # Single URI string
-                    return [self.all_entries[related_value]]
-                else:  # List of URI strings
-                    return [self.all_entries[subvalue] for subvalue in related_value]
+                try:
+                    if isinstance(related_value, str):  # Single URI string
+                        return [self.all_entries[related_value]]
+                    else:  # List of URI strings
+                        return [self.all_entries[subvalue] for subvalue in related_value]
+                except KeyError:
+                    raise ValueError(f"{key} contains invalid value {sys.exc_info()[1]}")
             return super().__getitem__(key)
 
     def process(self, context: dict, changed_files: set = None) -> dict:
         for uri, entry in context['entries'].items():
             if type(context['entries'][uri]) is not self.RelatedEntryReferenceDict:
                 context['entries'][uri] = self.RelatedEntryReferenceDict(entry, context['entries'])
```

### Comparing `ursus_ssg-1.1.1/ursus/context_processors/stale.py` & `ursus_ssg-1.2.0/ursus/context_processors/stale.py`

 * *Files identical despite different names*

### Comparing `ursus_ssg-1.1.1/ursus/generators/__init__.py` & `ursus_ssg-1.2.0/ursus/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `ursus_ssg-1.1.1/ursus/generators/static.py` & `ursus_ssg-1.2.0/ursus/generators/static.py`

 * *Files identical despite different names*

### Comparing `ursus_ssg-1.1.1/ursus/linters/__init__.py` & `ursus_ssg-1.2.0/ursus/linters/__init__.py`

 * *Files identical despite different names*

### Comparing `ursus_ssg-1.1.1/ursus/linters/footnotes.py` & `ursus_ssg-1.2.0/ursus/linters/footnotes.py`

 * *Files identical despite different names*

### Comparing `ursus_ssg-1.1.1/ursus/linters/images.py` & `ursus_ssg-1.2.0/ursus/linters/images.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,13 +17,13 @@
 
         link_regex = MarkdownLinksLinter.regex
 
         for markdown_path in get_files_in_path(config.content_path, suffix='.md'):
             with (config.content_path / markdown_path).open() as file:
                 for line_no, line in enumerate(file.readlines()):
                     for match in link_regex.finditer(line):
-                        entry_uri = match['url_group'].split(" ", maxsplit=1)[0].removeprefix('/')
+                        entry_uri = match['url'].removeprefix('/')
                         self.all_entry_links.add(entry_uri)
 
     def lint(self, file_path: Path):
         if is_image(config.content_path / file_path) and str(file_path) not in self.all_entry_links:
-            yield None, f"Unused image: {str(file_path)}", logging.WARNING
+            yield None, "Unused image", logging.WARNING
```

### Comparing `ursus_ssg-1.1.1/ursus/linters/markdown.py` & `ursus_ssg-1.2.0/ursus/linters/markdown.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,79 +1,72 @@
 from itertools import chain
 from markdown.blockprocessors import HashHeaderProcessor
 from pathlib import Path
 from requests.exceptions import ConnectionError
 from urllib.parse import unquote, urlparse
 from ursus.config import config
-from ursus.context_processors.markdown import patched_slugify
 from ursus.linters import RegexLinter
 import logging
 import re
 import requests
 
 
 class MarkdownLinksLinter(RegexLinter):
     """
     Verifies external links in Markdown files
     """
     file_suffixes = ('.md',)
 
     # Matches [], supports escaped brackets, ignores ![] images.
-    first_half = r"(?P<first_half>!?\[(?P<text>([^\]]|\\\])*)(?<!\\)\])"
+    first_half = r"(?P<first_half>!?\[(?P<alt_text>([^\]]|\\\])*)(?<!\\)\])"
 
     # Matches (), supports escaped parentheses
-    second_half = r"(?P<second_half>\((?P<url_group>([^\)]|\\\))*)(?<!\\)\))"
+    second_half = r"(?P<second_half>\((?P<url>([^\) ]|\\\))*)(\s+(?P<caption>\".*\"))?(?<!\\)\))"
 
     regex = re.compile(first_half + second_half)
 
     def handle_match(self, file_path: Path, match: re.Match):
-        text = match['text'].strip()
-        url = None
-        title = None
+        alt_text = match['alt_text'].strip()
         is_image = match['first_half'].startswith('!')
 
-        if match['url_group']:
-            parts = match['url_group'].split(" ", maxsplit=1)
-            url = parts[0]
-            if len(parts) == 2:
-                title = parts[1]
+        caption = match['caption']
 
         for error, level in chain(
-            self.validate_link_text(text, is_image, file_path),
-            self.validate_link_title(title, is_image, file_path),
-            self.validate_link_url(url, is_image, file_path),
+            self.validate_link_alt_text(alt_text, is_image, file_path),
+            self.validate_link_caption(caption, is_image, file_path),
+            self.validate_link_url(match['url'], is_image, file_path),
         ):
             yield f"{error}: {match.group(0)}", level
 
-    def validate_link_text(self, text: str, is_image: bool, file_path: Path):
+    def validate_link_alt_text(self, text: str, is_image: bool, file_path: Path):
         return
         yield
 
     def validate_link_url(self, url: str, is_image: bool, file_path: Path):
         return
         yield
 
-    def validate_link_title(self, title: str, is_image: bool, file_path: Path):
+    def validate_link_caption(self, caption: str, is_image: bool, file_path: Path):
         return
         yield
 
 
 class MarkdownLinkTextsLinter(MarkdownLinksLinter):
-    def validate_link_text(self, text: str, is_image: bool, file_path: Path):
+    def validate_link_alt_text(self, text: str, is_image: bool, file_path: Path):
         if not text:
             yield "Image has no alt text", logging.WARNING
 
 
 class MarkdownLinkTitlesLinter(MarkdownLinksLinter):
-    def validate_link_title(self, title: str, is_image: bool, file_path: Path):
-        if title is not None:
-            if not (title.startswith('"') and title.endswith('"')):
-                yield "Title is not quoted", logging.ERROR
-            elif title == title.strip('"'):
-                yield "Title is empty", logging.WARNING
+    def validate_link_caption(self, caption: str, is_image: bool, file_path: Path):
+        if caption is not None:
+            if not (caption.startswith('"') and caption.endswith('"')):
+                yield "Image caption is not quoted", logging.ERROR
+            elif caption == caption.strip('"'):
+                yield "Image caption is empty", logging.WARNING
 
 
 class MarkdownExternalLinksLinter(MarkdownLinksLinter):
     user_agent = "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Safari/537.36"
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -131,15 +124,15 @@
     def get_title_slugs(self, file_path: Path):
         if file_path not in self.title_slugs_cache:
             self.title_slugs_cache[file_path] = set()
             with file_path.open() as file:
                 for line in file.readlines():
                     if bool(self.header_regex.search(line)):
                         self.title_slugs_cache[file_path].add(
-                            patched_slugify(line.lstrip('#').strip(), '-')
+                            config.markdown_extensions['toc']['slugify'](line.lstrip('#').strip(), '-')
                         )
         return self.title_slugs_cache[file_path]
 
     def validate_link_url(self, url: str, is_image: bool, current_file_path: Path):
         for ignored_url in self.ignored_urls:
             if ignored_url.match(url):
                 return
```

### Comparing `ursus_ssg-1.1.1/ursus/renderers/__init__.py` & `ursus_ssg-1.2.0/ursus/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `ursus_ssg-1.1.1/ursus/renderers/image.py` & `ursus_ssg-1.2.0/ursus/renderers/image.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,18 @@
 
             for transform in entry.get('transforms', []):
                 output_path = transform['output_path']
                 abs_output_path = config.output_path / output_path
                 max_size = transform['max_size']
 
                 has_changed = changed_files is None or abs_file_path in changed_files
-                if has_changed and not abs_output_path.exists():
+                if has_changed and (
+                    (not abs_output_path.exists())
+                    or abs_file_path.stat().st_mtime > abs_output_path.stat().st_mtime
+                ):
                     if is_pdf(abs_file_path):
                         if abs_output_path.suffix.lower() == '.pdf':
                             logger.info('Copying %s to %s', entry_uri, str(output_path))
                             copy_file(abs_file_path, abs_output_path)
                         else:
                             logger.info('Generating %s preview as %s', entry_uri, str(output_path))
                             make_pdf_thumbnail(abs_file_path, max_size, abs_output_path)
```

### Comparing `ursus_ssg-1.1.1/ursus/renderers/jinja.py` & `ursus_ssg-1.2.0/ursus/renderers/jinja.py`

 * *Files identical despite different names*

### Comparing `ursus_ssg-1.1.1/ursus/renderers/lunr.py` & `ursus_ssg-1.2.0/ursus/renderers/lunr.py`

 * *Files identical despite different names*

### Comparing `ursus_ssg-1.1.1/ursus/renderers/sass.py` & `ursus_ssg-1.2.0/ursus/renderers/sass.py`

 * *Files identical despite different names*

### Comparing `ursus_ssg-1.1.1/ursus/renderers/static.py` & `ursus_ssg-1.2.0/ursus/renderers/static.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,30 +3,65 @@
 from ursus.utils import get_files_in_path, copy_file
 import logging
 
 
 logger = logging.getLogger(__name__)
 
 
-class StaticAssetRenderer(Renderer):
+class StaticFileRenderer(Renderer):
     """
-    Copies static assets in `templates_path` to `output_path`.
+    Copies static files to `output_path`
+    """
+    def get_files_to_copy(self, changed_files: set = None):
+        # Return list of tuples: (absolute_original_path, destination_relative_to_output_path)
+        return []
+
+    def render(self, context: dict, changed_files: set = None) -> set:
+        files_to_keep = set()
+        for asset_path, rel_output_path in self.get_files_to_copy():
+            abs_output_path = config.output_path / rel_output_path
+
+            if changed_files is None or asset_path in changed_files:
+                logger.info('Copying asset %s', str(rel_output_path))
+                copy_file(asset_path, abs_output_path)
+            files_to_keep.add(rel_output_path)
+
+        return files_to_keep
+
+
+class StaticAssetRenderer(StaticFileRenderer):
+    """
+    Copies static assets in `templates_path` to `output_path`
     """
     ignored_suffixes = ('.jinja', )
 
-    def get_assets_to_copy(self, changed_files: set = None):
+    def get_files_to_copy(self, changed_files: set = None):
         return [
-            f for f in get_files_in_path(config.templates_path)
+            (config.templates_path / f, f)
+            for f in get_files_in_path(config.templates_path)
             if f.suffix.lower() not in self.ignored_suffixes
         ]
 
+
+class ArchiveRenderer(Renderer):
+    """
+    Copies archives in `content_path` to `output_path`
+    """
+    included_suffixes = ('.zip', '.rar', '.gz', '.7z')
+
+    def get_assets_to_copy(self, changed_files: set = None):
+        return [
+            f for f in get_files_in_path(config.content_path)
+            if f.suffix.lower() in self.included_suffixes
+        ]
+
     def render(self, context: dict, changed_files: set = None) -> set:
         files_to_keep = set()
         for asset_path in self.get_assets_to_copy():
             abs_output_path = config.output_path / asset_path
 
-            if changed_files is None or config.templates_path / asset_path in changed_files:
-                logger.info('Copying asset %s', str(asset_path))
-                copy_file(config.templates_path / asset_path, abs_output_path)
+            if changed_files is None or config.content_path / asset_path in changed_files:
+                logger.info('Copying static entry %s', str(asset_path))
+                copy_file(config.content_path / asset_path, abs_output_path)
             files_to_keep.add(asset_path)
 
         return files_to_keep
```

### Comparing `ursus_ssg-1.1.1/ursus/server.py` & `ursus_ssg-1.2.0/ursus/server.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,26 +15,32 @@
         abs_index_path = abs_path / 'index.html'
 
         if not abs_path.exists():
             if abs_path.suffix == config.html_url_extension and abs_html_path.exists():
                 self.path = str(abs_html_path.relative_to(config.output_path))
             elif abs_index_path.exists():
                 self.path = str(abs_index_path.relative_to(config.output_path))
-        return super().do_GET()
+
+        try:
+            return super().do_GET()
+        except BrokenPipeError:
+            # These errors have no impact
+            pass
 
     def log_message(self, format, *args):
         logging.debug(f"Request to {self.path}")
 
 
 def serve(port: int = 80):
     """Start a static file server that serves Ursus on the given port.
 
     Args:
         port (int, optional): The port on which to serve the static site. Default is port 80.
     """
+    socketserver.ThreadingTCPServer.allow_reuse_address = True
     with socketserver.ThreadingTCPServer(("", port), HttpRequestHandler) as server:
         logging.info(f"Serving static site on port {port}")
         server.serve_forever()
 
 
 def serve_async(port: int = 80):
     thread = Thread(target=serve, args=(port, ), daemon=True)
```

### Comparing `ursus_ssg-1.1.1/ursus/utils.py` & `ursus_ssg-1.2.0/ursus/utils.py`

 * *Files identical despite different names*

### Comparing `ursus_ssg-1.1.1/ursus_ssg.egg-info/PKG-INFO` & `ursus_ssg-1.2.0/ursus_ssg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: ursus-ssg
-Version: 1.1.1
+Name: ursus_ssg
+Version: 1.2.0
 Summary: Static site generator
-Home-page: http://github.com/nicbou/ursus
+Home-page: http://github.com/all-about-berlin/ursus
 Author: Nicolas Bouliane
 Author-email: contact@nicolasbouliane.com
 License: MIT
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: coloredlogs==15.0.1
 Requires-Dist: GitPython==3.1.30
```

### Comparing `ursus_ssg-1.1.1/ursus_ssg.egg-info/SOURCES.txt` & `ursus_ssg-1.2.0/ursus_ssg.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -23,10 +23,11 @@
 ursus/renderers/jinja.py
 ursus/renderers/lunr.py
 ursus/renderers/sass.py
 ursus/renderers/static.py
 ursus_ssg.egg-info/PKG-INFO
 ursus_ssg.egg-info/SOURCES.txt
 ursus_ssg.egg-info/dependency_links.txt
+ursus_ssg.egg-info/entry_points.txt
 ursus_ssg.egg-info/not-zip-safe
 ursus_ssg.egg-info/requires.txt
 ursus_ssg.egg-info/top_level.txt
```

