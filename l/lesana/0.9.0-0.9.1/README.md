# Comparing `tmp/lesana-0.9.0.tar.gz` & `tmp/lesana-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lesana-0.9.0.tar", last modified: Fri Dec 24 09:44:07 2021, max compression
+gzip compressed data, was "lesana-0.9.1.tar", last modified: Fri Dec 31 15:01:57 2021, max compression
```

## Comparing `lesana-0.9.0.tar` & `lesana-0.9.1.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.383934 lesana-0.9.0/
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.359935 lesana-0.9.0/.builds/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      403 2021-06-06 10:04:29.000000 lesana-0.9.0/.builds/archlinux.yml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      412 2021-09-16 20:15:57.000000 lesana-0.9.0/.builds/debian_oldstable.yml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      409 2021-06-06 10:04:29.000000 lesana-0.9.0/.builds/debian_stable.yml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     3013 2021-12-24 09:38:54.000000 lesana-0.9.0/CHANGELOG.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)    35147 2021-06-06 10:04:29.000000 lesana-0.9.0/COPYING.txt
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      182 2021-06-06 10:04:29.000000 lesana-0.9.0/MANIFEST.in
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     4412 2021-12-24 09:44:07.383934 lesana-0.9.0/PKG-INFO
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     3139 2021-12-23 18:40:25.000000 lesana-0.9.0/README.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      265 2021-06-06 10:04:29.000000 lesana-0.9.0/TODO.rst
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.363935 lesana-0.9.0/docs/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)        6 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/.gitignore
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      638 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/Makefile
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.347935 lesana-0.9.0/docs/examples/
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.363935 lesana-0.9.0/docs/examples/bookmarks/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      235 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/examples/bookmarks/README.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      395 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/examples/bookmarks/settings.yaml
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.363935 lesana-0.9.0/docs/examples/bookmarks/templates/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      405 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/examples/bookmarks/templates/page.html
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.363935 lesana-0.9.0/docs/examples/books/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      202 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/examples/books/README.txt
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.363935 lesana-0.9.0/docs/examples/books/import/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1566 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/examples/books/import/from_tellico.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1476 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/examples/books/settings.yaml
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.363935 lesana-0.9.0/docs/examples/books/templates/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      698 2021-09-16 20:15:57.000000 lesana-0.9.0/docs/examples/books/templates/from_openlibrary.yaml
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.363935 lesana-0.9.0/docs/examples/music/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      197 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/examples/music/README.txt
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.363935 lesana-0.9.0/docs/examples/music/import/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      777 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/examples/music/import/from_tellico.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      637 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/examples/music/settings.yaml
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.363935 lesana-0.9.0/docs/examples/ticket_tracker/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      226 2021-09-16 20:15:57.000000 lesana-0.9.0/docs/examples/ticket_tracker/README.rst
--rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)      366 2021-09-18 16:00:31.000000 lesana-0.9.0/docs/examples/ticket_tracker/aliases.sh
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      718 2021-12-24 09:23:56.000000 lesana-0.9.0/docs/examples/ticket_tracker/settings.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      293 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/field_types.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      799 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/make.bat
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.363935 lesana-0.9.0/docs/source/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     3271 2021-12-24 09:36:55.000000 lesana-0.9.0/docs/source/conf.py
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.367935 lesana-0.9.0/docs/source/contrib/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      216 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/source/contrib/index.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      534 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/source/contrib/release_procedure.rst
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.367935 lesana-0.9.0/docs/source/devel/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      224 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/source/devel/index.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1002 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/source/devel/promises.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1319 2021-12-23 18:40:37.000000 lesana-0.9.0/docs/source/index.rst
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.367935 lesana-0.9.0/docs/source/man/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      140 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/source/man/Makefile
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      237 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/source/man/index.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      614 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/source/man/lesana-edit.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      486 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/source/man/lesana-export.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      844 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/source/man/lesana-get-values.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      498 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/source/man/lesana-index.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1121 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/source/man/lesana-init.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      604 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/source/man/lesana-new.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      385 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/source/man/lesana-rm.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1675 2021-12-24 09:17:01.000000 lesana-0.9.0/docs/source/man/lesana-search.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      870 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/source/man/lesana-show.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1770 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/source/man/lesana.rst
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.371935 lesana-0.9.0/docs/source/reference/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      139 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/source/reference/lesana.collection.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      130 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/source/reference/lesana.command.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      123 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/source/reference/lesana.data.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      309 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/source/reference/lesana.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      139 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/source/reference/lesana.templating.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      124 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/source/reference/lesana.types.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)       75 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/source/reference/modules.rst
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.371935 lesana-0.9.0/docs/source/user/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      425 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/source/user/derivatives.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     2642 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/source/user/getting_started_command_line.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      266 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/source/user/index.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1449 2021-06-06 10:04:29.000000 lesana-0.9.0/docs/source/user/moving_data_between_collections.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1461 2021-12-24 09:17:01.000000 lesana-0.9.0/docs/source/user/search.rst
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     4579 2021-12-24 09:17:01.000000 lesana-0.9.0/docs/source/user/settings.rst
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.371935 lesana-0.9.0/lesana/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      156 2021-06-06 10:04:29.000000 lesana-0.9.0/lesana/__init__.py
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)    23057 2021-12-24 09:33:41.000000 lesana-0.9.0/lesana/collection.py
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)    15716 2021-12-24 09:17:01.000000 lesana-0.9.0/lesana/command.py
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.375934 lesana-0.9.0/lesana/data/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)        0 2021-06-06 10:04:29.000000 lesana-0.9.0/lesana/data/__init__.py
--rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)      663 2021-10-03 08:37:37.000000 lesana-0.9.0/lesana/data/post-checkout
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      167 2021-06-06 10:04:29.000000 lesana-0.9.0/lesana/data/settings.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1120 2021-06-06 10:04:29.000000 lesana-0.9.0/lesana/templating.py
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)    10966 2021-12-23 15:50:53.000000 lesana-0.9.0/lesana/types.py
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.371935 lesana-0.9.0/lesana.egg-info/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     4412 2021-12-24 09:44:06.000000 lesana-0.9.0/lesana.egg-info/PKG-INFO
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     4125 2021-12-24 09:44:07.000000 lesana-0.9.0/lesana.egg-info/SOURCES.txt
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)        1 2021-12-24 09:44:06.000000 lesana-0.9.0/lesana.egg-info/dependency_links.txt
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)       35 2021-12-24 09:44:06.000000 lesana-0.9.0/lesana.egg-info/requires.txt
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)       13 2021-12-24 09:44:06.000000 lesana-0.9.0/lesana.egg-info/top_level.txt
--rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)      158 2021-06-06 10:04:29.000000 lesana-0.9.0/run_coverage
--rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)       58 2021-06-06 10:04:29.000000 lesana-0.9.0/run_qa
--rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)       66 2021-06-06 10:04:29.000000 lesana-0.9.0/run_tests
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.379934 lesana-0.9.0/scripts/
--rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)      962 2021-12-23 10:48:07.000000 lesana-0.9.0/scripts/lesana
--rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)     2790 2021-10-03 16:21:02.000000 lesana-0.9.0/scripts/openlibrary2lesana
--rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)     4161 2021-06-06 10:04:29.000000 lesana-0.9.0/scripts/tellico2lesana
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)       38 2021-12-24 09:44:07.383934 lesana-0.9.0/setup.cfg
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1884 2021-12-24 09:36:34.000000 lesana-0.9.0/setup.py
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.379934 lesana-0.9.0/tests/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)        0 2021-06-06 10:04:29.000000 lesana-0.9.0/tests/__init__.py
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.351935 lesana-0.9.0/tests/data/
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.379934 lesana-0.9.0/tests/data/complex/
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.379934 lesana-0.9.0/tests/data/complex/items/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      191 2021-06-06 10:04:29.000000 lesana-0.9.0/tests/data/complex/items/0b33e2b72add4ccab93a8cb7e2014b10.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      100 2021-06-06 10:04:29.000000 lesana-0.9.0/tests/data/complex/items/28b15099c84b41ab892133cd64876a32.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      487 2021-12-23 15:31:41.000000 lesana-0.9.0/tests/data/complex/items/5084bc6e94f24dc6976629282ef30419.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      192 2021-06-06 10:04:29.000000 lesana-0.9.0/tests/data/complex/items/5be0a92b6ad745fc9ffced106c94d221.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      151 2021-06-06 10:04:29.000000 lesana-0.9.0/tests/data/complex/items/73097121f1874a6ea2f927db7dc4f11e.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      309 2021-12-23 15:43:26.000000 lesana-0.9.0/tests/data/complex/items/8e9fa1ed3c1b4a30a6be7a98eda0cfa7.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      309 2021-12-23 16:30:39.000000 lesana-0.9.0/tests/data/complex/items/a4265cc5dfa94c3d8030d7df4a0ab747.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      197 2021-06-06 10:04:29.000000 lesana-0.9.0/tests/data/complex/items/b4b1feb620aa46f5b6784fbc608e4cd8.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      182 2021-06-06 10:04:29.000000 lesana-0.9.0/tests/data/complex/items/d35a1a71000e4378a25583e050561355.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      124 2021-06-06 10:04:29.000000 lesana-0.9.0/tests/data/complex/items/d4f361b0e3e541508eaf82c04451797f.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1363 2021-12-24 09:17:01.000000 lesana-0.9.0/tests/data/complex/settings.yaml
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.379934 lesana-0.9.0/tests/data/derivative/
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.379934 lesana-0.9.0/tests/data/derivative/items/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)       34 2021-06-06 10:04:29.000000 lesana-0.9.0/tests/data/derivative/items/48d73d796c0b47af964722e154fe879c.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      173 2021-06-06 10:04:29.000000 lesana-0.9.0/tests/data/derivative/settings.yaml
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.379934 lesana-0.9.0/tests/data/empty/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)        0 2021-06-06 10:04:29.000000 lesana-0.9.0/tests/data/empty/.gitignore
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.379934 lesana-0.9.0/tests/data/simple/
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.379934 lesana-0.9.0/tests/data/simple/items/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      201 2021-06-06 10:04:29.000000 lesana-0.9.0/tests/data/simple/items/085682ed-6792-499d-a3ab-9aebd683c011.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)       82 2021-06-06 10:04:29.000000 lesana-0.9.0/tests/data/simple/items/11189ee47ddf4796b718a483b379f976.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)       82 2021-06-06 10:04:29.000000 lesana-0.9.0/tests/data/simple/items/8b69b063b2a64db7b5714294a69255c7.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      550 2021-06-06 10:04:29.000000 lesana-0.9.0/tests/data/simple/settings.yaml
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.383934 lesana-0.9.0/tests/data/simple/templates/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      116 2021-06-06 10:04:29.000000 lesana-0.9.0/tests/data/simple/templates/collection_template.txt
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      103 2021-06-06 10:04:29.000000 lesana-0.9.0/tests/data/simple/templates/from_self.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      359 2021-09-16 20:15:57.000000 lesana-0.9.0/tests/data/simple/templates/new_entry_from_data.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      448 2021-09-16 20:15:57.000000 lesana-0.9.0/tests/data/simple/templates/new_entry_from_data_broken.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      423 2021-09-16 20:15:57.000000 lesana-0.9.0/tests/data/simple/templates/new_entry_from_data_invalid_yaml.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      425 2021-09-16 20:15:57.000000 lesana-0.9.0/tests/data/simple/templates/new_entry_from_multiple_data.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)       12 2021-06-06 10:04:29.000000 lesana-0.9.0/tests/data/simple/templates/trivial_template.txt
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.383934 lesana-0.9.0/tests/data/wrong/
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-24 09:44:07.383934 lesana-0.9.0/tests/data/wrong/items/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      384 2021-12-23 15:14:51.000000 lesana-0.9.0/tests/data/wrong/items/139770330d344a2f9d73945fab3bf47b.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      363 2021-12-23 15:14:51.000000 lesana-0.9.0/tests/data/wrong/items/5748adc272534bb699febe2c92ad05d9.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      378 2021-12-23 15:14:51.000000 lesana-0.9.0/tests/data/wrong/items/7496e7b7763b44d994ed07c134e66bdc.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      349 2021-12-23 15:14:51.000000 lesana-0.9.0/tests/data/wrong/items/b682034f7e2c454aa927606953680330.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      148 2021-12-23 15:14:51.000000 lesana-0.9.0/tests/data/wrong/items/b9a832309c984ada9f267471660c1313.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      363 2021-12-23 15:14:51.000000 lesana-0.9.0/tests/data/wrong/items/c54ae3caf262423d988cdc99ee9d0348.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      884 2021-12-23 15:14:51.000000 lesana-0.9.0/tests/data/wrong/settings.yaml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)    31780 2021-12-24 09:33:34.000000 lesana-0.9.0/tests/test_collection.py
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     6854 2021-12-24 09:17:01.000000 lesana-0.9.0/tests/test_commands.py
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      807 2021-06-06 10:04:29.000000 lesana-0.9.0/tests/test_derivatives.py
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1516 2021-06-06 10:04:29.000000 lesana-0.9.0/tests/test_templating.py
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)    17384 2021-09-16 20:15:57.000000 lesana-0.9.0/tests/test_types.py
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      525 2021-06-06 10:04:29.000000 lesana-0.9.0/tests/utils.py
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.997537 lesana-0.9.1/
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.729541 lesana-0.9.1/.builds/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      403 2021-06-06 10:04:29.000000 lesana-0.9.1/.builds/archlinux.yml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      412 2021-09-16 20:15:57.000000 lesana-0.9.1/.builds/debian_oldstable.yml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      409 2021-06-06 10:04:29.000000 lesana-0.9.1/.builds/debian_stable.yml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     3104 2021-12-31 14:59:24.000000 lesana-0.9.1/CHANGELOG.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)    35147 2021-06-06 10:04:29.000000 lesana-0.9.1/COPYING.txt
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      182 2021-06-06 10:04:29.000000 lesana-0.9.1/MANIFEST.in
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     4412 2021-12-31 15:01:56.997537 lesana-0.9.1/PKG-INFO
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     3139 2021-12-23 18:40:25.000000 lesana-0.9.1/README.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      265 2021-06-06 10:04:29.000000 lesana-0.9.1/TODO.rst
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.733541 lesana-0.9.1/docs/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)        6 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/.gitignore
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      638 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/Makefile
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.689542 lesana-0.9.1/docs/examples/
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.737541 lesana-0.9.1/docs/examples/bookmarks/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      235 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/examples/bookmarks/README.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      395 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/examples/bookmarks/settings.yaml
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.737541 lesana-0.9.1/docs/examples/bookmarks/templates/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      405 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/examples/bookmarks/templates/page.html
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.737541 lesana-0.9.1/docs/examples/books/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      202 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/examples/books/README.txt
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.737541 lesana-0.9.1/docs/examples/books/import/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1566 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/examples/books/import/from_tellico.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1476 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/examples/books/settings.yaml
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.737541 lesana-0.9.1/docs/examples/books/templates/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      698 2021-09-16 20:15:57.000000 lesana-0.9.1/docs/examples/books/templates/from_openlibrary.yaml
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.741541 lesana-0.9.1/docs/examples/music/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      197 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/examples/music/README.txt
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.741541 lesana-0.9.1/docs/examples/music/import/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      777 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/examples/music/import/from_tellico.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      637 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/examples/music/settings.yaml
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.749541 lesana-0.9.1/docs/examples/ticket_tracker/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      226 2021-09-16 20:15:57.000000 lesana-0.9.1/docs/examples/ticket_tracker/README.rst
+-rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)      366 2021-09-18 16:00:31.000000 lesana-0.9.1/docs/examples/ticket_tracker/aliases.sh
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      718 2021-12-24 09:23:56.000000 lesana-0.9.1/docs/examples/ticket_tracker/settings.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      293 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/field_types.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      799 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/make.bat
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.769541 lesana-0.9.1/docs/source/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     3277 2021-12-31 14:59:12.000000 lesana-0.9.1/docs/source/conf.py
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.769541 lesana-0.9.1/docs/source/contrib/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      216 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/source/contrib/index.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      735 2021-12-24 10:39:38.000000 lesana-0.9.1/docs/source/contrib/release_procedure.rst
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.801540 lesana-0.9.1/docs/source/devel/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      224 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/source/devel/index.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1002 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/source/devel/promises.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1319 2021-12-24 12:14:53.000000 lesana-0.9.1/docs/source/index.rst
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.813540 lesana-0.9.1/docs/source/man/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      140 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/source/man/Makefile
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      237 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/source/man/index.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      614 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/source/man/lesana-edit.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      486 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/source/man/lesana-export.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      844 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/source/man/lesana-get-values.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      498 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/source/man/lesana-index.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1121 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/source/man/lesana-init.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      604 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/source/man/lesana-new.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      385 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/source/man/lesana-rm.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1675 2021-12-24 09:17:01.000000 lesana-0.9.1/docs/source/man/lesana-search.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      870 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/source/man/lesana-show.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1770 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/source/man/lesana.rst
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.817540 lesana-0.9.1/docs/source/reference/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      139 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/source/reference/lesana.collection.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      130 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/source/reference/lesana.command.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      123 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/source/reference/lesana.data.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      309 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/source/reference/lesana.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      139 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/source/reference/lesana.templating.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      124 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/source/reference/lesana.types.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)       75 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/source/reference/modules.rst
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.841540 lesana-0.9.1/docs/source/user/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      425 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/source/user/derivatives.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     2642 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/source/user/getting_started_command_line.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      266 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/source/user/index.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1449 2021-06-06 10:04:29.000000 lesana-0.9.1/docs/source/user/moving_data_between_collections.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1461 2021-12-24 09:17:01.000000 lesana-0.9.1/docs/source/user/search.rst
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     4579 2021-12-24 09:17:01.000000 lesana-0.9.1/docs/source/user/settings.rst
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.861539 lesana-0.9.1/lesana/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      156 2021-06-06 10:04:29.000000 lesana-0.9.1/lesana/__init__.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)    23075 2021-12-29 09:33:45.000000 lesana-0.9.1/lesana/collection.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)    15716 2021-12-29 09:16:00.000000 lesana-0.9.1/lesana/command.py
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.897539 lesana-0.9.1/lesana/data/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)        0 2021-06-06 10:04:29.000000 lesana-0.9.1/lesana/data/__init__.py
+-rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)      663 2021-10-03 08:37:37.000000 lesana-0.9.1/lesana/data/post-checkout
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      167 2021-06-06 10:04:29.000000 lesana-0.9.1/lesana/data/settings.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1120 2021-06-06 10:04:29.000000 lesana-0.9.1/lesana/templating.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)    10967 2021-12-25 18:18:00.000000 lesana-0.9.1/lesana/types.py
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.869539 lesana-0.9.1/lesana.egg-info/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     4412 2021-12-31 15:01:55.000000 lesana-0.9.1/lesana.egg-info/PKG-INFO
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     4125 2021-12-31 15:01:56.000000 lesana-0.9.1/lesana.egg-info/SOURCES.txt
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)        1 2021-12-31 15:01:55.000000 lesana-0.9.1/lesana.egg-info/dependency_links.txt
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)       35 2021-12-31 15:01:55.000000 lesana-0.9.1/lesana.egg-info/requires.txt
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)       13 2021-12-31 15:01:55.000000 lesana-0.9.1/lesana.egg-info/top_level.txt
+-rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)      158 2021-06-06 10:04:29.000000 lesana-0.9.1/run_coverage
+-rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)       58 2021-06-06 10:04:29.000000 lesana-0.9.1/run_qa
+-rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)       66 2021-06-06 10:04:29.000000 lesana-0.9.1/run_tests
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.921539 lesana-0.9.1/scripts/
+-rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)      962 2021-12-23 10:48:07.000000 lesana-0.9.1/scripts/lesana
+-rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)     2790 2021-10-03 16:21:02.000000 lesana-0.9.1/scripts/openlibrary2lesana
+-rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)     4161 2021-06-06 10:04:29.000000 lesana-0.9.1/scripts/tellico2lesana
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)       38 2021-12-31 15:01:56.997537 lesana-0.9.1/setup.cfg
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1901 2021-12-31 14:58:42.000000 lesana-0.9.1/setup.py
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.929539 lesana-0.9.1/tests/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)        0 2021-06-06 10:04:29.000000 lesana-0.9.1/tests/__init__.py
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.693542 lesana-0.9.1/tests/data/
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.933539 lesana-0.9.1/tests/data/complex/
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.965538 lesana-0.9.1/tests/data/complex/items/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      191 2021-06-06 10:04:29.000000 lesana-0.9.1/tests/data/complex/items/0b33e2b72add4ccab93a8cb7e2014b10.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      100 2021-06-06 10:04:29.000000 lesana-0.9.1/tests/data/complex/items/28b15099c84b41ab892133cd64876a32.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      487 2021-12-23 15:31:41.000000 lesana-0.9.1/tests/data/complex/items/5084bc6e94f24dc6976629282ef30419.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      192 2021-06-06 10:04:29.000000 lesana-0.9.1/tests/data/complex/items/5be0a92b6ad745fc9ffced106c94d221.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      151 2021-06-06 10:04:29.000000 lesana-0.9.1/tests/data/complex/items/73097121f1874a6ea2f927db7dc4f11e.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      309 2021-12-23 15:43:26.000000 lesana-0.9.1/tests/data/complex/items/8e9fa1ed3c1b4a30a6be7a98eda0cfa7.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      309 2021-12-23 16:30:39.000000 lesana-0.9.1/tests/data/complex/items/a4265cc5dfa94c3d8030d7df4a0ab747.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      197 2021-06-06 10:04:29.000000 lesana-0.9.1/tests/data/complex/items/b4b1feb620aa46f5b6784fbc608e4cd8.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      182 2021-06-06 10:04:29.000000 lesana-0.9.1/tests/data/complex/items/d35a1a71000e4378a25583e050561355.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      124 2021-06-06 10:04:29.000000 lesana-0.9.1/tests/data/complex/items/d4f361b0e3e541508eaf82c04451797f.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1363 2021-12-24 09:17:01.000000 lesana-0.9.1/tests/data/complex/settings.yaml
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.965538 lesana-0.9.1/tests/data/derivative/
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.965538 lesana-0.9.1/tests/data/derivative/items/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)       34 2021-06-06 10:04:29.000000 lesana-0.9.1/tests/data/derivative/items/48d73d796c0b47af964722e154fe879c.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      173 2021-06-06 10:04:29.000000 lesana-0.9.1/tests/data/derivative/settings.yaml
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.965538 lesana-0.9.1/tests/data/empty/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)        0 2021-06-06 10:04:29.000000 lesana-0.9.1/tests/data/empty/.gitignore
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.965538 lesana-0.9.1/tests/data/simple/
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.969538 lesana-0.9.1/tests/data/simple/items/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      201 2021-06-06 10:04:29.000000 lesana-0.9.1/tests/data/simple/items/085682ed-6792-499d-a3ab-9aebd683c011.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)       82 2021-06-06 10:04:29.000000 lesana-0.9.1/tests/data/simple/items/11189ee47ddf4796b718a483b379f976.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)       82 2021-06-06 10:04:29.000000 lesana-0.9.1/tests/data/simple/items/8b69b063b2a64db7b5714294a69255c7.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      550 2021-06-06 10:04:29.000000 lesana-0.9.1/tests/data/simple/settings.yaml
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.981538 lesana-0.9.1/tests/data/simple/templates/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      116 2021-06-06 10:04:29.000000 lesana-0.9.1/tests/data/simple/templates/collection_template.txt
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      103 2021-06-06 10:04:29.000000 lesana-0.9.1/tests/data/simple/templates/from_self.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      359 2021-09-16 20:15:57.000000 lesana-0.9.1/tests/data/simple/templates/new_entry_from_data.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      448 2021-09-16 20:15:57.000000 lesana-0.9.1/tests/data/simple/templates/new_entry_from_data_broken.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      423 2021-09-16 20:15:57.000000 lesana-0.9.1/tests/data/simple/templates/new_entry_from_data_invalid_yaml.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      425 2021-09-16 20:15:57.000000 lesana-0.9.1/tests/data/simple/templates/new_entry_from_multiple_data.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)       12 2021-06-06 10:04:29.000000 lesana-0.9.1/tests/data/simple/templates/trivial_template.txt
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.985538 lesana-0.9.1/tests/data/wrong/
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2021-12-31 15:01:56.997537 lesana-0.9.1/tests/data/wrong/items/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      384 2021-12-23 15:14:51.000000 lesana-0.9.1/tests/data/wrong/items/139770330d344a2f9d73945fab3bf47b.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      363 2021-12-23 15:14:51.000000 lesana-0.9.1/tests/data/wrong/items/5748adc272534bb699febe2c92ad05d9.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      378 2021-12-23 15:14:51.000000 lesana-0.9.1/tests/data/wrong/items/7496e7b7763b44d994ed07c134e66bdc.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      349 2021-12-23 15:14:51.000000 lesana-0.9.1/tests/data/wrong/items/b682034f7e2c454aa927606953680330.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      148 2021-12-23 15:14:51.000000 lesana-0.9.1/tests/data/wrong/items/b9a832309c984ada9f267471660c1313.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      363 2021-12-23 15:14:51.000000 lesana-0.9.1/tests/data/wrong/items/c54ae3caf262423d988cdc99ee9d0348.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      884 2021-12-23 15:14:51.000000 lesana-0.9.1/tests/data/wrong/settings.yaml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)    31780 2021-12-24 09:33:34.000000 lesana-0.9.1/tests/test_collection.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     7649 2021-12-29 09:18:01.000000 lesana-0.9.1/tests/test_commands.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      807 2021-06-06 10:04:29.000000 lesana-0.9.1/tests/test_derivatives.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1516 2021-06-06 10:04:29.000000 lesana-0.9.1/tests/test_templating.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)    17384 2021-09-16 20:15:57.000000 lesana-0.9.1/tests/test_types.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      525 2021-06-06 10:04:29.000000 lesana-0.9.1/tests/utils.py
```

### Comparing `lesana-0.9.0/CHANGELOG.rst` & `lesana-0.9.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 ***********
  CHANGELOG
 ***********
 
 Unreleased
 ==========
 
+0.9.1
+=====
+
+Bugfix release
+
+* Included the post-checkout script in the released package.
+
 0.9.0
 =====
 
 * New data type: geo (for Geo URIs).
 * New custom filter for templates: to_yaml.
 * git hook to update the lesana cache when files are changed by git.
```

### Comparing `lesana-0.9.0/COPYING.txt` & `lesana-0.9.1/COPYING.txt`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/PKG-INFO` & `lesana-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lesana
-Version: 0.9.0
+Version: 0.9.1
 Summary: Manage collection inventories throught yaml files.
 Home-page: https://lesana.trueelena.org/
 Author: Elena ``of Valhalla'' Grandi
 Author-email: valhalla@trueelena.org
 License: GPLv3+
 Project-URL: Source, https://git.sr.ht/~valhalla/lesana
 Project-URL: Documentation, https://lesana.trueelena.org/
```

### Comparing `lesana-0.9.0/README.rst` & `lesana-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/docs/Makefile` & `lesana-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/docs/examples/books/import/from_tellico.yaml` & `lesana-0.9.1/docs/examples/books/import/from_tellico.yaml`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/docs/examples/books/settings.yaml` & `lesana-0.9.1/docs/examples/books/settings.yaml`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/docs/examples/books/templates/from_openlibrary.yaml` & `lesana-0.9.1/docs/examples/books/templates/from_openlibrary.yaml`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/docs/examples/music/import/from_tellico.yaml` & `lesana-0.9.1/docs/examples/music/import/from_tellico.yaml`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/docs/examples/music/settings.yaml` & `lesana-0.9.1/docs/examples/music/settings.yaml`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/docs/examples/ticket_tracker/settings.yaml` & `lesana-0.9.1/docs/examples/ticket_tracker/settings.yaml`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/docs/make.bat` & `lesana-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/docs/source/conf.py` & `lesana-0.9.1/docs/source/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 
 
 # -- Project information -----------------------------------------------------
 
 project = 'lesana'
-copyright = "2020, Elena Grandi"
+copyright = "2020-2021, Elena Grandi"
 author = "Elena ``of Valhalla''"
 
 # The full version, including alpha/beta/rc tags
-release = '0.9.0'
+release = '0.9.1'
 # The major project version
-version = '0.9'
+version = '0.10'
 
 # compatibility with sphinx 1.8 on buster
 master_doc = 'index'
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `lesana-0.9.0/docs/source/contrib/release_procedure.rst` & `lesana-0.9.1/docs/source/contrib/release_procedure.rst`

 * *Files 13% similar despite different names*

```diff
@@ -24,7 +24,14 @@
   for the tag content use something like::
 
      Version $VERSION
 
      * contents
      * of the relevant
      * changelog
+
+* Send the release announce to::
+
+     valhalla/lesana-announce@lists.sr.ht, ~valhalla/lesana-discuss@lists.sr.ht
+
+* Close the bugs marked as pending_release on
+  https://todo.sr.ht/~valhalla/lesana.
```

### Comparing `lesana-0.9.0/docs/source/devel/promises.rst` & `lesana-0.9.1/docs/source/devel/promises.rst`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/docs/source/index.rst` & `lesana-0.9.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/docs/source/man/lesana-edit.rst` & `lesana-0.9.1/docs/source/man/lesana-edit.rst`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/docs/source/man/lesana-get-values.rst` & `lesana-0.9.1/docs/source/man/lesana-get-values.rst`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/docs/source/man/lesana-init.rst` & `lesana-0.9.1/docs/source/man/lesana-init.rst`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/docs/source/man/lesana-new.rst` & `lesana-0.9.1/docs/source/man/lesana-new.rst`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/docs/source/man/lesana-search.rst` & `lesana-0.9.1/docs/source/man/lesana-search.rst`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/docs/source/man/lesana-show.rst` & `lesana-0.9.1/docs/source/man/lesana-show.rst`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/docs/source/man/lesana.rst` & `lesana-0.9.1/docs/source/man/lesana.rst`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/docs/source/user/getting_started_command_line.rst` & `lesana-0.9.1/docs/source/user/getting_started_command_line.rst`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/docs/source/user/moving_data_between_collections.rst` & `lesana-0.9.1/docs/source/user/moving_data_between_collections.rst`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/docs/source/user/search.rst` & `lesana-0.9.1/docs/source/user/search.rst`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/docs/source/user/settings.rst` & `lesana-0.9.1/docs/source/user/settings.rst`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/lesana/collection.py` & `lesana-0.9.1/lesana/collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -506,15 +506,17 @@
         )
         for eid in eids:
             for entry in self.entries_from_short_eid(eid):
                 if entry is not None:
                     cache.delete_document(entry.idterm)
                     self.remove_file(entry.fname)
                 else:
-                    logger.warning("No such entry: {}, ignoring".format(eid))
+                    logger.warning("Not removing {}: no such entry".format(
+                        eid
+                    ))
         cache.commit()
         cache.close()
 
     def remove_file(self, fname):
         f_path = os.path.join(self.itemdir, fname)
         if git_available and self.settings.get('git', False):
             try:
@@ -557,15 +559,15 @@
     def entry_from_rendered_template(self, template, data):
         try:
             template = self.get_template(template)
             rendered = template.render(**data)
         except jinja2.exceptions.TemplateSyntaxError as e:
             raise TemplatingError(e)
         try:
-            data = ruamel.yaml.load(rendered, ruamel.yaml.RoundTripLoader)
+            data = self.yaml.load(rendered)
         except ruamel.yaml.YAMLError as e:
             logger.warning(
                 "The following data failed to load as YAML: \n{}".format(
                     rendered
                 )
 
             )
```

### Comparing `lesana-0.9.0/lesana/command.py` & `lesana-0.9.1/lesana/command.py`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/lesana/data/post-checkout` & `lesana-0.9.1/lesana/data/post-checkout`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/lesana/templating.py` & `lesana-0.9.1/lesana/templating.py`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/lesana/types.py` & `lesana-0.9.1/lesana/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
         See LesanaList for an idea on how to do so.
         """
         to_index = self.field.get('index', False)
         if not to_index:
             return
         if not value:
-            logger.info(
+            logger.debug(
                 "Not indexing empty value {}".format(value)
             )
             return
         prefix = self.field.get('prefix', 'X' + self.field['name'].upper())
         indexer.index_text(self._to_index_text(value), 1, prefix)
         if to_index == 'free':
             indexer.index_text(self._to_index_text(value))
```

### Comparing `lesana-0.9.0/lesana.egg-info/PKG-INFO` & `lesana-0.9.1/lesana.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lesana
-Version: 0.9.0
+Version: 0.9.1
 Summary: Manage collection inventories throught yaml files.
 Home-page: https://lesana.trueelena.org/
 Author: Elena ``of Valhalla'' Grandi
 Author-email: valhalla@trueelena.org
 License: GPLv3+
 Project-URL: Source, https://git.sr.ht/~valhalla/lesana
 Project-URL: Documentation, https://lesana.trueelena.org/
```

### Comparing `lesana-0.9.0/lesana.egg-info/SOURCES.txt` & `lesana-0.9.1/lesana.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/scripts/lesana` & `lesana-0.9.1/scripts/lesana`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/scripts/openlibrary2lesana` & `lesana-0.9.1/scripts/openlibrary2lesana`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/scripts/tellico2lesana` & `lesana-0.9.1/scripts/tellico2lesana`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/setup.py` & `lesana-0.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,19 +5,19 @@
         long_description = fp.read()
 except IOError:
     print("Could not read README.rst, long_description will be empty.")
     long_description = ""
 
 setup(
     name='lesana',
-    version='0.9.0',
+    version='0.9.1',
     packages=find_packages(),
     scripts=['scripts/lesana'],
     package_data={
-        '': ['*.yaml']
+        '': ['*.yaml', 'post-checkout']
     },
     test_suite='tests',
     install_requires=[
         # 'xapian >= 1.4',
         'ruamel.yaml',
         'jinja2',
         'python-dateutil',
```

### Comparing `lesana-0.9.0/tests/data/complex/settings.yaml` & `lesana-0.9.1/tests/data/complex/settings.yaml`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/tests/data/simple/settings.yaml` & `lesana-0.9.1/tests/data/simple/settings.yaml`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/tests/data/wrong/settings.yaml` & `lesana-0.9.1/tests/data/wrong/settings.yaml`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/tests/test_collection.py` & `lesana-0.9.1/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/tests/test_commands.py` & `lesana-0.9.1/tests/test_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,21 @@
     def setUp(self):
         self.tmpdir = tempfile.TemporaryDirectory()
         utils.copytree(
             'tests/data/simple',
             self.tmpdir.name,
             dirs_exist_ok=True,
         )
+        # re-index the collection before running each test
+        args = {
+            'collection': self.tmpdir.name,
+            "files": None,
+            "reset": True,
+        }
+        self._run_command(command.Index(), args)
 
     def tearDown(self):
         pass
 
     def test_init(self):
         args = {
             'collection': self.tmpdir.name,
@@ -159,19 +166,28 @@
         self.assertEqual(streams['stdout'].getvalue(), '')
         self.assertEqual(streams['stderr'].getvalue(), '')
 
     def test_remove(self):
         args = {
             'collection': self.tmpdir.name,
             'git': True,
-            'entries': '11189ee4',
+            'entries': ['11189ee4'],
         }
         streams = self._run_command(command.Remove(), args)
         self.assertEqual(streams['stdout'].getvalue(), '')
         self.assertEqual(streams['stderr'].getvalue(), '')
+        # and check that the entry has been removed
+        args = {
+            'collection': self.tmpdir.name,
+            'git': True,
+            'eid': '11189ee4',
+            'template': False,
+        }
+        streams = self._run_command(command.Show(), args)
+        self.assertEqual(streams['stderr'].getvalue(), '')
 
     def test_update(self):
         args = {
             'collection': self.tmpdir.name,
             'git': True,
             'query': 'Another',
             'field': 'position',
@@ -186,14 +202,21 @@
     def setUp(self):
         self.tmpdir = tempfile.TemporaryDirectory()
         utils.copytree(
             'tests/data/complex',
             self.tmpdir.name,
             dirs_exist_ok=True,
         )
+        # re-index the collection before running each test
+        args = {
+            'collection': self.tmpdir.name,
+            "files": None,
+            "reset": True,
+        }
+        self._run_command(command.Index(), args)
 
     def tearDown(self):
         pass
 
     def test_get_values_from_list(self):
         args = {
             'collection': self.tmpdir.name,
```

### Comparing `lesana-0.9.0/tests/test_derivatives.py` & `lesana-0.9.1/tests/test_derivatives.py`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/tests/test_templating.py` & `lesana-0.9.1/tests/test_templating.py`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/tests/test_types.py` & `lesana-0.9.1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `lesana-0.9.0/tests/utils.py` & `lesana-0.9.1/tests/utils.py`

 * *Files identical despite different names*

