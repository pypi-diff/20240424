# Comparing `tmp/xblock-sdk-0.8.0.tar.gz` & `tmp/xblock-sdk-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xblock-sdk-0.8.0.tar", last modified: Thu Feb 29 15:44:36 2024, max compression
+gzip compressed data, was "xblock-sdk-0.9.0.tar", last modified: Thu Mar 21 13:03:51 2024, max compression
```

## Comparing `xblock-sdk-0.8.0.tar` & `xblock-sdk-0.9.0.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.775882 xblock-sdk-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/LICENSE.TXT
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-02-29 15:44:36.775882 xblock-sdk-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10990 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.759882 xblock-sdk-0.8.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/requirements/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.759882 xblock-sdk-0.8.0/sample_xblocks/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.763882 xblock-sdk-0.8.0/sample_xblocks/basic/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8847 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/basic/content.py
--rw-r--r--   0 runner    (1001) docker     (127)    21273 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/basic/problem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.755882 xblock-sdk-0.8.0/sample_xblocks/basic/public/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.763882 xblock-sdk-0.8.0/sample_xblocks/basic/public/images/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/basic/public/images/correct-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/basic/public/images/incorrect-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/basic/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/basic/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.763882 xblock-sdk-0.8.0/sample_xblocks/basic/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/basic/templates/problem.html
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/basic/templates/sequence.html
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/basic/templates/vertical.html
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/basic/view_counter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.763882 xblock-sdk-0.8.0/sample_xblocks/filethumbs/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/filethumbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/filethumbs/filethumbs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.763882 xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.763882 xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/css/thumbs.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.763882 xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/html/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/html/thumbs.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.763882 xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/js/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/js/SpecRunner.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.763882 xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/js/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.763882 xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/MIT.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    20765 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/jasmine-html.js
--rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/jasmine.css
--rw-r--r--   0 runner    (1001) docker     (127)    70892 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/jasmine.js
--rw-r--r--   0 runner    (1001) docker     (127)    20000 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/js/lib/jasmine-jquery.js
--rw-r--r--   0 runner    (1001) docker     (127)    92629 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/js/lib/jquery-1.9.1.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.763882 xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/js/spec/
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/js/spec/thumbs_spec.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.763882 xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/js/src/
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/js/src/thumbs.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.767882 xblock-sdk-0.8.0/sample_xblocks/thumbs/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/thumbs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.767882 xblock-sdk-0.8.0/sample_xblocks/thumbs/static/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/thumbs/static/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.767882 xblock-sdk-0.8.0/sample_xblocks/thumbs/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/thumbs/static/css/thumbs.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.767882 xblock-sdk-0.8.0/sample_xblocks/thumbs/static/html/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/thumbs/static/html/thumbs.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.767882 xblock-sdk-0.8.0/sample_xblocks/thumbs/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/thumbs/static/js/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/thumbs/static/js/SpecRunner.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.767882 xblock-sdk-0.8.0/sample_xblocks/thumbs/static/js/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.767882 xblock-sdk-0.8.0/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/MIT.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    20765 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/jasmine-html.js
--rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/jasmine.css
--rw-r--r--   0 runner    (1001) docker     (127)    70892 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/jasmine.js
--rw-r--r--   0 runner    (1001) docker     (127)    20000 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/thumbs/static/js/lib/jasmine-jquery.js
--rw-r--r--   0 runner    (1001) docker     (127)    92629 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/thumbs/static/js/lib/jquery-1.9.1.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.767882 xblock-sdk-0.8.0/sample_xblocks/thumbs/static/js/spec/
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/thumbs/static/js/spec/thumbs_spec.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.767882 xblock-sdk-0.8.0/sample_xblocks/thumbs/static/js/src/
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/thumbs/static/js/src/thumbs.js
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/sample_xblocks/thumbs/thumbs.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-29 15:44:36.775882 xblock-sdk-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.771882 xblock-sdk-0.8.0/workbench/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    17975 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/runtime_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/scenarios.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.759882 xblock-sdk-0.8.0/workbench/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.759882 xblock-sdk-0.8.0/workbench/static/workbench/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.771882 xblock-sdk-0.8.0/workbench/static/workbench/css/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/static/workbench/css/workbench.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.771882 xblock-sdk-0.8.0/workbench/static/workbench/images/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4716 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/static/workbench/images/header-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.759882 xblock-sdk-0.8.0/workbench/static/workbench/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.771882 xblock-sdk-0.8.0/workbench/static/workbench/js/runtime/
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/static/workbench/js/runtime/1.js
--rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/static/workbench/js/runtime/logger.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.771882 xblock-sdk-0.8.0/workbench/static/workbench/js/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)     9459 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/static/workbench/js/vendor/jquery-migrate.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/static/workbench/js/vendor/jquery.cookie.js
--rw-r--r--   0 runner    (1001) docker     (127)    85659 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/static/workbench/js/vendor/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    16449 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/static/workbench/js/vendor/underscore-min.js
--rw-r--r--   0 runner    (1001) docker     (127)    27589 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/static/workbench/js/vendor/underscore-min.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.771882 xblock-sdk-0.8.0/workbench/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/templates/500.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.771882 xblock-sdk-0.8.0/workbench/templates/workbench/
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/templates/workbench/block.html
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/templates/workbench/blockview.html
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/templates/workbench/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/templates/workbench/settings.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.771882 xblock-sdk-0.8.0/workbench/test/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/test/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/test/test_scenarios.py
--rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/test/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5544 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-02-29 15:44:33.000000 xblock-sdk-0.8.0/workbench/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 15:44:36.775882 xblock-sdk-0.8.0/xblock_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-02-29 15:44:36.000000 xblock-sdk-0.8.0/xblock_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-02-29 15:44:36.000000 xblock-sdk-0.8.0/xblock_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 15:44:36.000000 xblock-sdk-0.8.0/xblock_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-02-29 15:44:36.000000 xblock-sdk-0.8.0/xblock_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-29 15:44:36.000000 xblock-sdk-0.8.0/xblock_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-29 15:44:36.000000 xblock-sdk-0.8.0/xblock_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.317516 xblock-sdk-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/LICENSE.TXT
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-21 13:03:51.317516 xblock-sdk-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10990 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.301516 xblock-sdk-0.9.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/requirements/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.301516 xblock-sdk-0.9.0/sample_xblocks/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.301516 xblock-sdk-0.9.0/sample_xblocks/basic/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8833 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/basic/content.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21217 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/basic/problem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.297516 xblock-sdk-0.9.0/sample_xblocks/basic/public/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.305516 xblock-sdk-0.9.0/sample_xblocks/basic/public/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/basic/public/images/correct-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/basic/public/images/incorrect-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/basic/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/basic/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.305516 xblock-sdk-0.9.0/sample_xblocks/basic/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/basic/templates/problem.html
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/basic/templates/sequence.html
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/basic/templates/vertical.html
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/basic/view_counter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.305516 xblock-sdk-0.9.0/sample_xblocks/filethumbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/filethumbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/filethumbs/filethumbs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.305516 xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.305516 xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/css/thumbs.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.305516 xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/html/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/html/thumbs.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.305516 xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/js/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/js/SpecRunner.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.305516 xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/js/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.305516 xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/MIT.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20765 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/jasmine-html.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/jasmine.css
+-rw-r--r--   0 runner    (1001) docker     (127)    70892 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/jasmine.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20000 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/js/lib/jasmine-jquery.js
+-rw-r--r--   0 runner    (1001) docker     (127)    92629 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/js/lib/jquery-1.9.1.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.305516 xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/js/spec/
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/js/spec/thumbs_spec.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.305516 xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/js/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/js/src/thumbs.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.305516 xblock-sdk-0.9.0/sample_xblocks/thumbs/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/thumbs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.305516 xblock-sdk-0.9.0/sample_xblocks/thumbs/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/thumbs/static/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.305516 xblock-sdk-0.9.0/sample_xblocks/thumbs/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/thumbs/static/css/thumbs.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.305516 xblock-sdk-0.9.0/sample_xblocks/thumbs/static/html/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/thumbs/static/html/thumbs.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.305516 xblock-sdk-0.9.0/sample_xblocks/thumbs/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/thumbs/static/js/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/thumbs/static/js/SpecRunner.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.309516 xblock-sdk-0.9.0/sample_xblocks/thumbs/static/js/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.309516 xblock-sdk-0.9.0/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/MIT.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20765 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/jasmine-html.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/jasmine.css
+-rw-r--r--   0 runner    (1001) docker     (127)    70892 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/jasmine.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20000 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/thumbs/static/js/lib/jasmine-jquery.js
+-rw-r--r--   0 runner    (1001) docker     (127)    92629 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/thumbs/static/js/lib/jquery-1.9.1.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.309516 xblock-sdk-0.9.0/sample_xblocks/thumbs/static/js/spec/
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/thumbs/static/js/spec/thumbs_spec.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.309516 xblock-sdk-0.9.0/sample_xblocks/thumbs/static/js/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/thumbs/static/js/src/thumbs.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/sample_xblocks/thumbs/thumbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-21 13:03:51.317516 xblock-sdk-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.309516 xblock-sdk-0.9.0/workbench/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4529 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17948 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/runtime_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.297516 xblock-sdk-0.9.0/workbench/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.301516 xblock-sdk-0.9.0/workbench/static/workbench/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.309516 xblock-sdk-0.9.0/workbench/static/workbench/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/static/workbench/css/workbench.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.313516 xblock-sdk-0.9.0/workbench/static/workbench/images/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4716 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/static/workbench/images/header-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.301516 xblock-sdk-0.9.0/workbench/static/workbench/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.313516 xblock-sdk-0.9.0/workbench/static/workbench/js/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/static/workbench/js/runtime/1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/static/workbench/js/runtime/logger.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.313516 xblock-sdk-0.9.0/workbench/static/workbench/js/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)     9459 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/static/workbench/js/vendor/jquery-migrate.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/static/workbench/js/vendor/jquery.cookie.js
+-rw-r--r--   0 runner    (1001) docker     (127)    85659 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/static/workbench/js/vendor/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16449 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/static/workbench/js/vendor/underscore-min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    27589 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/static/workbench/js/vendor/underscore-min.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.313516 xblock-sdk-0.9.0/workbench/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/templates/500.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.313516 xblock-sdk-0.9.0/workbench/templates/workbench/
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/templates/workbench/block.html
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/templates/workbench/blockview.html
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/templates/workbench/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/templates/workbench/settings.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.313516 xblock-sdk-0.9.0/workbench/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/test/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/test/test_scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12386 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/test/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5544 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-03-21 13:03:43.000000 xblock-sdk-0.9.0/workbench/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:03:51.317516 xblock-sdk-0.9.0/xblock_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-21 13:03:51.000000 xblock-sdk-0.9.0/xblock_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-03-21 13:03:51.000000 xblock-sdk-0.9.0/xblock_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 13:03:51.000000 xblock-sdk-0.9.0/xblock_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-03-21 13:03:51.000000 xblock-sdk-0.9.0/xblock_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-21 13:03:51.000000 xblock-sdk-0.9.0/xblock_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-21 13:03:51.000000 xblock-sdk-0.9.0/xblock_sdk.egg-info/top_level.txt
```

### Comparing `xblock-sdk-0.8.0/CHANGELOG.rst` & `xblock-sdk-0.9.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 =============================
 Change history for XBlock SDK
 =============================
 
 These are notable changes in XBlock.
 
+0.9.0
+-----
+* Xblock bumped to 3.0.0. Removed the deprecated id_generator method parameter in xblock.runtime
+
 0.8.0
 -----
 * Added support for python 3.12
 * Dropped support for django 3.2
 
 
 0.7.0
```

### Comparing `xblock-sdk-0.8.0/LICENSE.TXT` & `xblock-sdk-0.9.0/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/PKG-INFO` & `xblock-sdk-0.9.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xblock-sdk
-Version: 0.8.0
+Version: 0.9.0
 Summary: XBlock SDK
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `xblock-sdk-0.8.0/README.rst` & `xblock-sdk-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/requirements/test.txt` & `xblock-sdk-0.9.0/requirements/test.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
 #    make upgrade
 #
-acid-xblock==0.2.1
+acid-xblock==0.3.0
     # via -r requirements/test.in
 appdirs==1.4.4
     # via
     #   -r requirements/base.txt
     #   fs
 arrow==1.3.0
     # via
     #   -r requirements/base.txt
     #   cookiecutter
-asgiref==3.7.2
+asgiref==3.8.0
     # via
     #   -r requirements/base.txt
     #   django
+backports-zoneinfo==0.2.1 ; python_version < "3.9"
+    # via
+    #   -c requirements/constraints.txt
+    #   -r requirements/base.txt
+    #   django
 binaryornot==0.4.4
     # via
     #   -r requirements/base.txt
     #   cookiecutter
-boto3==1.34.49
+boto3==1.34.67
     # via
     #   -r requirements/base.txt
     #   fs-s3fs
-botocore==1.34.49
+botocore==1.34.67
     # via
     #   -r requirements/base.txt
     #   boto3
     #   s3transfer
-cachetools==5.3.2
+cachetools==5.3.3
     # via tox
 certifi==2024.2.2
     # via
     #   -r requirements/base.txt
     #   requests
 chardet==5.2.0
     # via
@@ -50,15 +55,15 @@
     # via
     #   -r requirements/base.txt
     #   cookiecutter
 colorama==0.4.6
     # via tox
 cookiecutter==2.6.0
     # via -r requirements/base.txt
-coverage[toml]==7.4.3
+coverage[toml]==7.4.4
     # via
     #   -r requirements/test.in
     #   pytest-cov
 ddt==1.7.2
     # via -r requirements/test.in
 distlib==0.3.8
     # via virtualenv
@@ -128,15 +133,15 @@
     #   markdown-it-py
 mock==5.1.0
     # via -r requirements/test.in
 openedx-django-pyfs==3.5.0
     # via
     #   -r requirements/base.txt
     #   xblock
-packaging==23.2
+packaging==24.0
     # via
     #   pyproject-api
     #   pytest
     #   pytest-rerunfailures
     #   tox
 platformdirs==4.2.0
     # via
@@ -150,54 +155,53 @@
     # via
     #   -r requirements/base.txt
     #   rich
 pypng==0.20220715.0
     # via -r requirements/base.txt
 pyproject-api==1.6.1
     # via tox
-pytest==8.0.2
+pytest==8.1.1
     # via
     #   pytest-cov
     #   pytest-django
     #   pytest-rerunfailures
 pytest-cov==4.1.0
     # via -r requirements/test.in
 pytest-django==4.8.0
     # via -r requirements/test.in
-pytest-rerunfailures==13.0
+pytest-rerunfailures==14.0
     # via -r requirements/test.in
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   -r requirements/base.txt
     #   arrow
     #   botocore
     #   xblock
 python-slugify==8.0.4
     # via
     #   -r requirements/base.txt
     #   cookiecutter
 pytz==2024.1
     # via
     #   -r requirements/base.txt
-    #   django
     #   xblock
 pyyaml==6.0.1
     # via
     #   -r requirements/base.txt
     #   cookiecutter
     #   xblock
 requests==2.31.0
     # via
     #   -r requirements/base.txt
     #   cookiecutter
-rich==13.7.0
+rich==13.7.1
     # via
     #   -r requirements/base.txt
     #   cookiecutter
-s3transfer==0.10.0
+s3transfer==0.10.1
     # via
     #   -r requirements/base.txt
     #   boto3
 simplejson==3.19.2
     # via
     #   -r requirements/base.txt
     #   xblock
@@ -217,17 +221,17 @@
     #   python-slugify
 tomli==2.0.1
     # via
     #   coverage
     #   pyproject-api
     #   pytest
     #   tox
-tox==4.13.0
+tox==4.14.1
     # via -r requirements/test.in
-types-python-dateutil==2.8.19.20240106
+types-python-dateutil==2.9.0.20240316
     # via
     #   -r requirements/base.txt
     #   arrow
 typing-extensions==4.10.0
     # via
     #   -r requirements/base.txt
     #   asgiref
@@ -243,14 +247,14 @@
     # via
     #   -r requirements/base.txt
     #   xblock
 webob==1.8.7
     # via
     #   -r requirements/base.txt
     #   xblock
-xblock[django]==1.10.0
+xblock[django]==3.0.0
     # via
     #   -r requirements/base.txt
     #   acid-xblock
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `xblock-sdk-0.8.0/sample_xblocks/basic/content.py` & `xblock-sdk-0.9.0/sample_xblocks/basic/content.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
 
     def fallback_view(self, _view_name, context=None):
         """Provide a fallback view handler"""
         context = context or {}
         return Fragment(Template(self.content).substitute(**context))
 
     @classmethod
-    def parse_xml(cls, node, runtime, keys, id_generator):
+    def parse_xml(cls, node, runtime, keys):
         """
         Parse the XML for an HTML block.
 
         The entire subtree under `node` is re-serialized, and set as the
         content of the XBlock.
 
         """
```

### Comparing `xblock-sdk-0.8.0/sample_xblocks/basic/problem.py` & `xblock-sdk-0.9.0/sample_xblocks/basic/problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,23 +53,23 @@
     """
     script = String(help="Python code to compute values", scope=Scope.content, default="")
     seed = Integer(help="Random seed for this student", scope=Scope.user_state, default=0)
     problem_attempted = Boolean(help="Has the student attempted this problem?", scope=Scope.user_state, default=False)
     has_children = True
 
     @classmethod
-    def parse_xml(cls, node, runtime, keys, id_generator):
+    def parse_xml(cls, node, runtime, keys):
         block = runtime.construct_xblock_from_class(cls, keys)
 
         # Find <script> children, turn them into script content.
         for child in node:
             if child.tag == "script":
                 block.script += child.text
             else:
-                block.runtime.add_node_as_child(block, child, id_generator)
+                block.runtime.add_node_as_child(block, child)
 
         return block
 
     def set_student_seed(self):
         """Set a random seed for the student so they each have different but repeatable data."""
         # Don't return zero, that's the default, and the sign that we should make a new seed.
         self.seed = int(time.time() * 1000) % 100 + 1
@@ -337,20 +337,20 @@
             argspec = inspect.getargspec(self.check)  # pylint: disable=deprecated-method
         arguments = {}
         for arg in argspec.args[1:]:
             arguments[arg] = node.attrib.pop(arg)
         self.arguments = arguments
 
     @classmethod
-    def parse_xml(cls, node, runtime, keys, id_generator):
+    def parse_xml(cls, node, runtime, keys):
         """
         Parse the XML for a checker. A few arguments are handled specially,
         then the rest get the usual treatment.
         """
-        block = super().parse_xml(node, runtime, keys, id_generator)
+        block = super().parse_xml(node, runtime, keys)
         block.set_arguments_from_xml(node)
         return block
 
     def check(self, **kwargs):
         """
         Called with the data provided by the ProblemBlock.
         Returns any data, which will be passed to the Javascript handle_check
```

### Comparing `xblock-sdk-0.8.0/sample_xblocks/basic/slider.py` & `xblock-sdk-0.9.0/sample_xblocks/basic/slider.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/sample_xblocks/basic/structure.py` & `xblock-sdk-0.9.0/sample_xblocks/basic/structure.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/sample_xblocks/basic/view_counter.py` & `xblock-sdk-0.9.0/sample_xblocks/basic/view_counter.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/sample_xblocks/filethumbs/filethumbs.py` & `xblock-sdk-0.9.0/sample_xblocks/filethumbs/filethumbs.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/js/SpecRunner.html` & `xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/js/SpecRunner.html`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/MIT.LICENSE` & `xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/MIT.LICENSE`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/jasmine-html.js` & `xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/jasmine-html.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/jasmine.css` & `xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/jasmine.css`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/jasmine.js` & `xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/js/lib/jasmine-1.3.1/jasmine.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/js/lib/jasmine-jquery.js` & `xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/js/lib/jasmine-jquery.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/js/lib/jquery-1.9.1.min.js` & `xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/js/lib/jquery-1.9.1.min.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/js/spec/thumbs_spec.js` & `xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/js/spec/thumbs_spec.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/sample_xblocks/filethumbs/static/js/src/thumbs.js` & `xblock-sdk-0.9.0/sample_xblocks/filethumbs/static/js/src/thumbs.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/sample_xblocks/thumbs/static/js/SpecRunner.html` & `xblock-sdk-0.9.0/sample_xblocks/thumbs/static/js/SpecRunner.html`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/MIT.LICENSE` & `xblock-sdk-0.9.0/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/MIT.LICENSE`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/jasmine-html.js` & `xblock-sdk-0.9.0/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/jasmine-html.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/jasmine.css` & `xblock-sdk-0.9.0/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/jasmine.css`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/jasmine.js` & `xblock-sdk-0.9.0/sample_xblocks/thumbs/static/js/lib/jasmine-1.3.1/jasmine.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/sample_xblocks/thumbs/static/js/lib/jasmine-jquery.js` & `xblock-sdk-0.9.0/sample_xblocks/thumbs/static/js/lib/jasmine-jquery.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/sample_xblocks/thumbs/static/js/lib/jquery-1.9.1.min.js` & `xblock-sdk-0.9.0/sample_xblocks/thumbs/static/js/lib/jquery-1.9.1.min.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/sample_xblocks/thumbs/static/js/spec/thumbs_spec.js` & `xblock-sdk-0.9.0/sample_xblocks/thumbs/static/js/spec/thumbs_spec.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/sample_xblocks/thumbs/static/js/src/thumbs.js` & `xblock-sdk-0.9.0/sample_xblocks/thumbs/static/js/src/thumbs.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/sample_xblocks/thumbs/thumbs.py` & `xblock-sdk-0.9.0/sample_xblocks/thumbs/thumbs.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/setup.py` & `xblock-sdk-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/workbench/admin.py` & `xblock-sdk-0.9.0/workbench/admin.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/workbench/blocks.py` & `xblock-sdk-0.9.0/workbench/blocks.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/workbench/models.py` & `xblock-sdk-0.9.0/workbench/models.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/workbench/runtime.py` & `xblock-sdk-0.9.0/workbench/runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,16 +260,15 @@
         # XBlocks that require services that may be too specific
         # to include in the default workbench configuration.
         for service_name, service_path in (settings.WORKBENCH.get('services', {})).items():
             service = self._load_service(service_path)
             if service is not None:
                 services[service_name] = service
 
-        super().__init__(ID_MANAGER, services=services)
-        self.id_generator = ID_MANAGER
+        super().__init__(ID_MANAGER, ID_MANAGER, services=services)
         self.user_id = user_id
 
     def get_user_role(self):
         """Provide a dummy user role."""
         return 'Student'
 
     @property
```

### Comparing `xblock-sdk-0.8.0/workbench/scenarios.py` & `xblock-sdk-0.9.0/workbench/scenarios.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     assert scname not in SCENARIOS, "Already have a %r scenario" % scname
     runtime = WorkbenchRuntime()
 
     # WorkbenchRuntime has an id_generator, but most runtimes won't
     # (because the generator will be contextual), so we
     # pass it explicitly to parse_xml_string.
     runtime.id_generator.set_scenario(slugify(description))
-    usage_id = runtime.parse_xml_string(xml, runtime.id_generator)
+    usage_id = runtime.parse_xml_string(xml)
     SCENARIOS[scname] = Scenario(description, usage_id, xml)
 
 
 def remove_scenario(scname):
     """
     Remove a named scenario from the global list.
     """
```

### Comparing `xblock-sdk-0.8.0/workbench/services.py` & `xblock-sdk-0.9.0/workbench/services.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/workbench/settings.py` & `xblock-sdk-0.9.0/workbench/settings.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/workbench/static/workbench/css/workbench.css` & `xblock-sdk-0.9.0/workbench/static/workbench/css/workbench.css`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/workbench/static/workbench/images/header-logo.png` & `xblock-sdk-0.9.0/workbench/static/workbench/images/header-logo.png`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/workbench/static/workbench/js/runtime/1.js` & `xblock-sdk-0.9.0/workbench/static/workbench/js/runtime/1.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/workbench/static/workbench/js/runtime/logger.js` & `xblock-sdk-0.9.0/workbench/static/workbench/js/runtime/logger.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/workbench/static/workbench/js/vendor/jquery-migrate.min.js` & `xblock-sdk-0.9.0/workbench/static/workbench/js/vendor/jquery-migrate.min.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/workbench/static/workbench/js/vendor/jquery.cookie.js` & `xblock-sdk-0.9.0/workbench/static/workbench/js/vendor/jquery.cookie.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/workbench/static/workbench/js/vendor/jquery.min.js` & `xblock-sdk-0.9.0/workbench/static/workbench/js/vendor/jquery.min.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/workbench/static/workbench/js/vendor/underscore-min.js` & `xblock-sdk-0.9.0/workbench/static/workbench/js/vendor/underscore-min.js`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/workbench/static/workbench/js/vendor/underscore-min.map` & `xblock-sdk-0.9.0/workbench/static/workbench/js/vendor/underscore-min.map`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/workbench/templates/workbench/block.html` & `xblock-sdk-0.9.0/workbench/templates/workbench/block.html`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/workbench/templates/workbench/blockview.html` & `xblock-sdk-0.9.0/workbench/templates/workbench/blockview.html`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/workbench/templates/workbench/index.html` & `xblock-sdk-0.9.0/workbench/templates/workbench/index.html`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/workbench/test/test_runtime.py` & `xblock-sdk-0.9.0/workbench/test/test_runtime.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/workbench/test/test_scenarios.py` & `xblock-sdk-0.9.0/workbench/test/test_scenarios.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/workbench/test/test_views.py` & `xblock-sdk-0.9.0/workbench/test/test_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,19 @@
 
     # Change it again.
     response = client.post(handler_url, "{}", "text/json")
     the_data = json.loads(response.content.decode('utf-8'))['the_data']
     assert the_data == "defxx"
 
 
-@temp_scenario(XBlock)
+class XBlockWithoutHandler(XBlock):
+    pass
+
+
+@temp_scenario(XBlockWithoutHandler)
 def test_xblock_without_handler():
     # Test that an XBlock without a handler raises an Exception
     # when we try to hit a handler on it
     client = Client()
 
     # Pick the most-recent usage ID just made in the temp_scenario setup...
     usage_id = ID_MANAGER.last_created_usage_id()
```

### Comparing `xblock-sdk-0.8.0/workbench/test_utils.py` & `xblock-sdk-0.9.0/workbench/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             xml (string): Path to an XML definition of the XBlock, relative
                 to the test module.
 
         Returns:
             XBlock
         """
         block_id = self.runtime.parse_xml_string(
-            self.load_fixture_str(xml_path), self.runtime.id_generator
+            self.load_fixture_str(xml_path)
         )
         return self.runtime.get_block(block_id)
 
     def request(self, xblock, handler_name, content, request_method="POST", response_format=None):
         """Make a request to an XBlock handler.
 
         Args:
```

### Comparing `xblock-sdk-0.8.0/workbench/urls.py` & `xblock-sdk-0.9.0/workbench/urls.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/workbench/views.py` & `xblock-sdk-0.9.0/workbench/views.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/workbench/wsgi.py` & `xblock-sdk-0.9.0/workbench/wsgi.py`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/xblock_sdk.egg-info/PKG-INFO` & `xblock-sdk-0.9.0/xblock_sdk.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xblock-sdk
-Version: 0.8.0
+Version: 0.9.0
 Summary: XBlock SDK
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `xblock-sdk-0.8.0/xblock_sdk.egg-info/SOURCES.txt` & `xblock-sdk-0.9.0/xblock_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xblock-sdk-0.8.0/xblock_sdk.egg-info/entry_points.txt` & `xblock-sdk-0.9.0/xblock_sdk.egg-info/entry_points.txt`

 * *Files identical despite different names*

