# Comparing `tmp/rocm_docs_core-1.0.0.tar.gz` & `tmp/rocm_docs_core-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocm_docs_core-1.0.0.tar", last modified: Wed Apr 17 23:05:33 2024, max compression
+gzip compressed data, was "rocm_docs_core-1.1.0.tar", last modified: Wed Apr 24 15:45:55 2024, max compression
```

## Comparing `rocm_docs_core-1.0.0.tar` & `rocm_docs_core-1.1.0.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:33.837326 rocm_docs_core-1.0.0/
--rwxrwxrwx   0 root         (0) root         (0)    17095 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/LICENSE.txt
--rwxrwxrwx   0 root         (0) root         (0)     3966 2024-04-17 23:05:33.829329 rocm_docs_core-1.0.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2347 2024-02-21 19:55:38.000000 rocm_docs_core-1.0.0/README.md
--rwxrwxrwx   0 root         (0) root         (0)     3592 2024-04-17 23:04:15.000000 rocm_docs_core-1.0.0/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-17 23:05:33.838539 rocm_docs_core-1.0.0/setup.cfg
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:30.056692 rocm_docs_core-1.0.0/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:30.245573 rocm_docs_core-1.0.0/src/rocm_docs/
--rwxrwxrwx   0 root         (0) root         (0)     2663 2024-04-17 22:59:16.000000 rocm_docs_core-1.0.0/src/rocm_docs/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    11121 2024-04-17 22:59:16.000000 rocm_docs_core-1.0.0/src/rocm_docs/core.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:30.291377 rocm_docs_core-1.0.0/src/rocm_docs/data/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:30.401984 rocm_docs_core-1.0.0/src/rocm_docs/data/_doxygen/
--rwxrwxrwx   0 root         (0) root         (0)    72476 2024-04-17 22:44:44.000000 rocm_docs_core-1.0.0/src/rocm_docs/data/_doxygen/extra_stylesheet.css
--rwxrwxrwx   0 root         (0) root         (0)      112 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/data/_doxygen/footer.html
--rwxrwxrwx   0 root         (0) root         (0)     1428 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/data/_doxygen/header.html
--rwxrwxrwx   0 root         (0) root         (0)    37255 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/data/_doxygen/stylesheet.css
--rwxrwxrwx   0 root         (0) root         (0)     2940 2024-02-21 19:55:38.000000 rocm_docs_core-1.0.0/src/rocm_docs/data/projects.schema.json
--rwxrwxrwx   0 root         (0) root         (0)     4222 2024-02-21 19:55:38.000000 rocm_docs_core-1.0.0/src/rocm_docs/data/projects.yaml
--rwxrwxrwx   0 root         (0) root         (0)     8600 2024-04-17 22:59:16.000000 rocm_docs_core-1.0.0/src/rocm_docs/doxygen.py
--rwxrwxrwx   0 root         (0) root         (0)     4663 2024-04-17 22:59:16.000000 rocm_docs_core-1.0.0/src/rocm_docs/formatting.py
--rwxrwxrwx   0 root         (0) root         (0)    17085 2024-04-17 22:59:16.000000 rocm_docs_core-1.0.0/src/rocm_docs/projects.py
--rwxrwxrwx   0 root         (0) root         (0)       59 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/py.typed
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:30.472070 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/
--rwxrwxrwx   0 root         (0) root         (0)      185 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/404.html
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:30.562229 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/components/
--rwxrwxrwx   0 root         (0) root         (0)     1931 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/components/article-info.html
--rwxrwxrwx   0 root         (0) root         (0)      215 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/components/left-side-menu.html
--rwxrwxrwx   0 root         (0) root         (0)      217 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/components/toggle-primary-sidebar.html
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:30.017452 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/flavors/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:30.666545 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/flavors/rocm/
--rwxrwxrwx   0 root         (0) root         (0)      149 2024-03-13 19:55:26.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/flavors/rocm/footer.jinja
--rwxrwxrwx   0 root         (0) root         (0)     1424 2024-03-13 19:55:26.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/flavors/rocm/header.jinja
--rwxrwxrwx   0 root         (0) root         (0)       67 2024-03-13 19:55:26.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/flavors/rocm/left-side-menu.jinja
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:30.767980 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/
--rwxrwxrwx   0 root         (0) root         (0)       45 2024-02-21 19:55:38.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/footer.jinja
--rwxrwxrwx   0 root         (0) root         (0)      703 2024-03-13 19:55:26.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/header.jinja
--rwxrwxrwx   0 root         (0) root         (0)       75 2024-03-13 19:55:26.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/left-side-menu.jinja
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:30.899227 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/
--rwxrwxrwx   0 root         (0) root         (0)      149 2024-03-13 19:55:26.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/footer.jinja
--rwxrwxrwx   0 root         (0) root         (0)     1424 2024-03-13 19:55:26.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/header.jinja
--rwxrwxrwx   0 root         (0) root         (0)       70 2024-03-13 19:55:26.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/left-side-menu.jinja
--rwxrwxrwx   0 root         (0) root         (0)      344 2024-04-17 22:44:51.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/layout.html
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:31.005508 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/sections/
--rwxrwxrwx   0 root         (0) root         (0)      318 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/sections/footer-content.html
--rwxrwxrwx   0 root         (0) root         (0)     2137 2024-02-21 19:55:38.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/sections/footer.html
--rwxrwxrwx   0 root         (0) root         (0)     2267 2024-02-21 19:55:38.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/sections/header.html
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:31.358365 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/
--rwxrwxrwx   0 root         (0) root         (0)      831 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/code_word_breaks.js
--rwxrwxrwx   0 root         (0) root         (0)     3984 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/custom.css
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:30.045367 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:33.425927 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/
--rwxrwxrwx   0 root         (0) root         (0)    20756 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff
--rwxrwxrwx   0 root         (0) root         (0)    16748 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff2
--rwxrwxrwx   0 root         (0) root         (0)    21924 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff
--rwxrwxrwx   0 root         (0) root         (0)    17872 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff2
--rwxrwxrwx   0 root         (0) root         (0)    20780 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff
--rwxrwxrwx   0 root         (0) root         (0)    16808 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff2
--rwxrwxrwx   0 root         (0) root         (0)    21876 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff
--rwxrwxrwx   0 root         (0) root         (0)    17876 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff2
--rwxrwxrwx   0 root         (0) root         (0)    20672 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff
--rwxrwxrwx   0 root         (0) root         (0)    16756 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff2
--rwxrwxrwx   0 root         (0) root         (0)    21820 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff
--rwxrwxrwx   0 root         (0) root         (0)    17780 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff2
--rwxrwxrwx   0 root         (0) root         (0)    20172 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff
--rwxrwxrwx   0 root         (0) root         (0)    16372 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff2
--rwxrwxrwx   0 root         (0) root         (0)    21248 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff
--rwxrwxrwx   0 root         (0) root         (0)    17384 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff2
--rwxrwxrwx   0 root         (0) root         (0)    20664 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff
--rwxrwxrwx   0 root         (0) root         (0)    16696 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff2
--rwxrwxrwx   0 root         (0) root         (0)    21520 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff
--rwxrwxrwx   0 root         (0) root         (0)    17544 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff2
--rwxrwxrwx   0 root         (0) root         (0)    27552 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff
--rwxrwxrwx   0 root         (0) root         (0)    22132 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff2
--rwxrwxrwx   0 root         (0) root         (0)    29388 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff
--rwxrwxrwx   0 root         (0) root         (0)    23712 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff2
--rwxrwxrwx   0 root         (0) root         (0)    27592 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff
--rwxrwxrwx   0 root         (0) root         (0)    22184 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff2
--rwxrwxrwx   0 root         (0) root         (0)    29392 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff
--rwxrwxrwx   0 root         (0) root         (0)    23824 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff2
--rwxrwxrwx   0 root         (0) root         (0)    27456 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff
--rwxrwxrwx   0 root         (0) root         (0)    22212 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff2
--rwxrwxrwx   0 root         (0) root         (0)    29224 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff
--rwxrwxrwx   0 root         (0) root         (0)    23676 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff2
--rwxrwxrwx   0 root         (0) root         (0)    26652 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff
--rwxrwxrwx   0 root         (0) root         (0)    21516 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff2
--rwxrwxrwx   0 root         (0) root         (0)    28292 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff
--rwxrwxrwx   0 root         (0) root         (0)    22904 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff2
--rwxrwxrwx   0 root         (0) root         (0)    27376 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff
--rwxrwxrwx   0 root         (0) root         (0)    22040 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff2
--rwxrwxrwx   0 root         (0) root         (0)    28704 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff
--rwxrwxrwx   0 root         (0) root         (0)    23168 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff2
--rwxrwxrwx   0 root         (0) root         (0)    29304 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff
--rwxrwxrwx   0 root         (0) root         (0)    23704 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff2
--rwxrwxrwx   0 root         (0) root         (0)    27520 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff
--rwxrwxrwx   0 root         (0) root         (0)    22084 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff2
--rwxrwxrwx   0 root         (0) root         (0)    21856 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff
--rwxrwxrwx   0 root         (0) root         (0)    17820 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff2
--rwxrwxrwx   0 root         (0) root         (0)    20712 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff
--rwxrwxrwx   0 root         (0) root         (0)    16740 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff2
--rwxrwxrwx   0 root         (0) root         (0)     9931 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts.css
--rwxrwxrwx   0 root         (0) root         (0)     3502 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts.css.map
--rwxrwxrwx   0 root         (0) root         (0)     1503 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts.scss
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:33.573687 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/images/
--rwxrwxrwx   0 root         (0) root         (0)     1611 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/images/alpha-watermark.svg
--rwxrwxrwx   0 root         (0) root         (0)      925 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/images/amd-header-logo.svg
--rwxrwxrwx   0 root         (0) root         (0)     1760 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/images/beta-watermark.svg
--rwxrwxrwx   0 root         (0) root         (0)    10074 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/images/rocm-logo.png
--rwxrwxrwx   0 root         (0) root         (0)     3426 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/rdcMisc.js
--rwxrwxrwx   0 root         (0) root         (0)      780 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/renameVersionLinks.js
--rwxrwxrwx   0 root         (0) root         (0)     1260 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/rocm_footer.css
--rwxrwxrwx   0 root         (0) root         (0)    19276 2024-02-21 19:55:38.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/rocm_header.css
--rwxrwxrwx   0 root         (0) root         (0)      596 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/theme_mode_captions.js
--rwxrwxrwx   0 root         (0) root         (0)      243 2024-04-17 22:44:44.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/theme.conf
--rwxrwxrwx   0 root         (0) root         (0)     5279 2024-04-17 22:59:16.000000 rocm_docs_core-1.0.0/src/rocm_docs/theme.py
--rwxrwxrwx   0 root         (0) root         (0)     5975 2024-04-17 22:59:13.000000 rocm_docs_core-1.0.0/src/rocm_docs/util.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:33.814071 rocm_docs_core-1.0.0/src/rocm_docs_core.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     3966 2024-04-17 23:05:28.000000 rocm_docs_core-1.0.0/src/rocm_docs_core.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     6839 2024-04-17 23:05:29.000000 rocm_docs_core-1.0.0/src/rocm_docs_core.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-17 23:05:28.000000 rocm_docs_core-1.0.0/src/rocm_docs_core.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       55 2024-04-17 23:05:28.000000 rocm_docs_core-1.0.0/src/rocm_docs_core.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)      485 2024-04-17 23:05:28.000000 rocm_docs_core-1.0.0/src/rocm_docs_core.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       10 2024-04-17 23:05:28.000000 rocm_docs_core-1.0.0/src/rocm_docs_core.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:33.784843 rocm_docs_core-1.0.0/tests/
--rwxrwxrwx   0 root         (0) root         (0)     2637 2024-02-21 19:55:38.000000 rocm_docs_core-1.0.0/tests/test_doxygen.py
--rwxrwxrwx   0 root         (0) root         (0)     1272 2024-02-21 19:55:38.000000 rocm_docs_core-1.0.0/tests/test_meta.py
--rwxrwxrwx   0 root         (0) root         (0)     5682 2024-04-17 22:59:17.000000 rocm_docs_core-1.0.0/tests/test_projects.py
--rwxrwxrwx   0 root         (0) root         (0)     1854 2024-04-17 22:59:17.000000 rocm_docs_core-1.0.0/tests/test_sites.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.862615 rocm_docs_core-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    17095 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-24 15:45:55.862615 rocm_docs_core-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:45:55.862615 rocm_docs_core-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.838615 rocm_docs_core-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.838615 rocm_docs_core-1.1.0/src/rocm_docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11121 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.838615 rocm_docs_core-1.1.0/src/rocm_docs/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.838615 rocm_docs_core-1.1.0/src/rocm_docs/data/_doxygen/
+-rw-r--r--   0 runner    (1001) docker     (127)    72476 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/data/_doxygen/extra_stylesheet.css
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/data/_doxygen/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/data/_doxygen/header.html
+-rw-r--r--   0 runner    (1001) docker     (127)    37255 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/data/_doxygen/stylesheet.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/data/projects.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/data/projects.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/doxygen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17085 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.842615 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/404.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.842615 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/components/article-info.html
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/components/left-side-menu.html
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/components/toggle-primary-sidebar.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.834615 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.842615 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm/footer.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm/header.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm/left-side-menu.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.842615 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/footer.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/header.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/left-side-menu.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.842615 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/footer.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/header.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/left-side-menu.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.842615 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/sections/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/sections/footer-content.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/sections/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/sections/header.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.846615 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/code_word_breaks.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.838615 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.858615 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20756 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16748 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21924 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17872 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20780 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16808 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21876 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17876 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20672 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16756 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21820 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17780 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20172 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16372 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21248 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17384 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20664 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16696 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21520 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17544 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27552 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22132 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29388 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23712 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27592 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22184 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29392 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23824 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27456 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22212 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29224 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23676 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26652 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21516 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28292 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22904 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27376 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22040 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28704 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23168 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29304 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23704 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27520 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22084 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21856 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17820 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20712 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16740 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     9931 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.858615 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/images/alpha-watermark.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      925 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/images/amd-header-logo.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1760 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/images/beta-watermark.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10074 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/images/rocm-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/rdcMisc.js
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/renameVersionLinks.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/rocm_footer.css
+-rw-r--r--   0 runner    (1001) docker     (127)    19276 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/rocm_header.css
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/theme_mode_captions.js
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/src/rocm_docs/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.858615 rocm_docs_core-1.1.0/src/rocm_docs_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-24 15:45:55.000000 rocm_docs_core-1.1.0/src/rocm_docs_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-04-24 15:45:55.000000 rocm_docs_core-1.1.0/src/rocm_docs_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:45:55.000000 rocm_docs_core-1.1.0/src/rocm_docs_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-24 15:45:55.000000 rocm_docs_core-1.1.0/src/rocm_docs_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-24 15:45:55.000000 rocm_docs_core-1.1.0/src/rocm_docs_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 15:45:55.000000 rocm_docs_core-1.1.0/src/rocm_docs_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:45:55.858615 rocm_docs_core-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/tests/test_doxygen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/tests/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-24 15:45:43.000000 rocm_docs_core-1.1.0/tests/test_sites.py
```

### Comparing `rocm_docs_core-1.0.0/LICENSE.txt` & `rocm_docs_core-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/PKG-INFO` & `rocm_docs_core-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocm-docs-core
-Version: 1.0.0
+Version: 1.1.0
 Summary: Core utilities for all ROCm documentation on RTD
 Author-email: Lauren Wrubleski <Lauren.Wrubleski@amd.com>
 Project-URL: repository, https://github.com/RadeonOpenCompute/rocm-docs-core
 Project-URL: documentation, https://docs.amd.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rocm_docs_core-1.0.0/README.md` & `rocm_docs_core-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/pyproject.toml` & `rocm_docs_core-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'rocm-docs-core'
-version = "1.0.0"
+version = "1.1.0"
 authors=[
   {name="Lauren Wrubleski", email="Lauren.Wrubleski@amd.com"}
 ]
 description ='Core utilities for all ROCm documentation on RTD'
 readme="README.md"
 classifiers = [
   "Programming Language :: Python :: 3",
@@ -68,19 +68,18 @@
 [tool.black]
 target-version = ["py310"]
 line-length = 80
 color = true
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.0.0"
+version = "1.1.0"
 version_files = ["pyproject.toml:^version", "docs/conf.py:^(version|release)"]
 tag_format = "v$version"
 annotated_tag = true
-major_version_zero = true
 
 [tool.isort]
 # https://github.com/timothycrosley/isort/
 py_version = "310"
 line_length = 80
 
 known_typing = ["typing", "types", "typing_extensions", "mypy", "mypy_extensions"]
```

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/__init__.py` & `rocm_docs_core-1.1.0/src/rocm_docs/__init__.py`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/core.py` & `rocm_docs_core-1.1.0/src/rocm_docs/core.py`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/data/_doxygen/extra_stylesheet.css` & `rocm_docs_core-1.1.0/src/rocm_docs/data/_doxygen/extra_stylesheet.css`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/data/_doxygen/header.html` & `rocm_docs_core-1.1.0/src/rocm_docs/data/_doxygen/header.html`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/data/_doxygen/stylesheet.css` & `rocm_docs_core-1.1.0/src/rocm_docs/data/_doxygen/stylesheet.css`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/data/projects.schema.json` & `rocm_docs_core-1.1.0/src/rocm_docs/data/projects.schema.json`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/data/projects.yaml` & `rocm_docs_core-1.1.0/src/rocm_docs/data/projects.yaml`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/doxygen.py` & `rocm_docs_core-1.1.0/src/rocm_docs/doxygen.py`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/formatting.py` & `rocm_docs_core-1.1.0/src/rocm_docs/formatting.py`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/projects.py` & `rocm_docs_core-1.1.0/src/rocm_docs/projects.py`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/components/article-info.html` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/components/article-info.html`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/flavors/rocm/header.jinja` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm/header.jinja`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/header.jinja` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/header.jinja`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/header.jinja` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/header.jinja`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/sections/footer.html` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/sections/footer.html`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                         <!-- OneTrust Cookies Settings button end -->
                     </ul>
                 </div>
             </div>
             <div class="row d-flex align-items-center">
                 <div class="col-12 text-center">
                     <div>
-                        <span class="copyright">© 2023 Advanced Micro Devices, Inc</span>
+                        <span class="copyright">© 2024 Advanced Micro Devices, Inc</span>
                     </div>
                 </div>
             </div>
         </section>
     </div>
 </footer>
```

#### html2text {}

```diff
@@ -5,8 +5,8 @@
     * _P_r_i_v_a_c_y
     * _T_r_a_d_e_m_a_r_k_s
     * _S_t_a_t_e_m_e_n_t_ _o_n_ _F_o_r_c_e_d_ _L_a_b_o_r
     * _F_a_i_r_ _a_n_d_ _O_p_e_n_ _C_o_m_p_e_t_i_t_i_o_n
     * _U_K_ _T_a_x_ _S_t_r_a_t_e_g_y
     * _C_o_o_k_i_e_ _P_o_l_i_c_y
     * _C_o_o_k_i_e_ _S_e_t_t_i_n_g_s
-Â© 2023 Advanced Micro Devices, Inc
+Â© 2024 Advanced Micro Devices, Inc
```

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/sections/header.html` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/sections/header.html`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/code_word_breaks.js` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/code_word_breaks.js`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/custom.css` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/custom.css`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff2` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff2` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff2` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff2` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff2` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff2` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff2` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff2` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff2` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff2` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff2` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff2` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff2` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff2` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff2` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff2` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff2` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff2` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff2` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff2` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff2` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff2` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff2` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff2` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts.css` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts.css`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts.css.map` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts.css.map`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts.scss` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/fonts.scss`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/images/alpha-watermark.svg` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/images/alpha-watermark.svg`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/images/amd-header-logo.svg` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/images/amd-header-logo.svg`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/images/beta-watermark.svg` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/images/beta-watermark.svg`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/images/rocm-logo.png` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/images/rocm-logo.png`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/rdcMisc.js` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/rdcMisc.js`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/renameVersionLinks.js` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/renameVersionLinks.js`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/rocm_footer.css` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/rocm_footer.css`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/rocm_header.css` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/rocm_header.css`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/theme_mode_captions.js` & `rocm_docs_core-1.1.0/src/rocm_docs/rocm_docs_theme/static/theme_mode_captions.js`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/theme.py` & `rocm_docs_core-1.1.0/src/rocm_docs/theme.py`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs/util.py` & `rocm_docs_core-1.1.0/src/rocm_docs/util.py`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs_core.egg-info/PKG-INFO` & `rocm_docs_core-1.1.0/src/rocm_docs_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocm-docs-core
-Version: 1.0.0
+Version: 1.1.0
 Summary: Core utilities for all ROCm documentation on RTD
 Author-email: Lauren Wrubleski <Lauren.Wrubleski@amd.com>
 Project-URL: repository, https://github.com/RadeonOpenCompute/rocm-docs-core
 Project-URL: documentation, https://docs.amd.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rocm_docs_core-1.0.0/src/rocm_docs_core.egg-info/SOURCES.txt` & `rocm_docs_core-1.1.0/src/rocm_docs_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/tests/test_doxygen.py` & `rocm_docs_core-1.1.0/tests/test_doxygen.py`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/tests/test_meta.py` & `rocm_docs_core-1.1.0/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/tests/test_projects.py` & `rocm_docs_core-1.1.0/tests/test_projects.py`

 * *Files identical despite different names*

### Comparing `rocm_docs_core-1.0.0/tests/test_sites.py` & `rocm_docs_core-1.1.0/tests/test_sites.py`

 * *Files identical despite different names*

