# Comparing `tmp/pywb-2.7.4.tar.gz` & `tmp/pywb-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywb-2.7.4.tar", last modified: Fri May 19 18:25:16 2023, max compression
+gzip compressed data, was "pywb-2.8.0.tar", last modified: Wed Apr 24 12:25:57 2024, max compression
```

## Comparing `pywb-2.7.4.tar` & `pywb-2.8.0.tar`

### file list

```diff
@@ -1,432 +1,432 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.290699 pywb-2.7.4/
--rwxr-xr-x   0 runner    (1001) docker     (123)      316 2023-05-19 18:25:04.000000 pywb-2.7.4/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-19 18:25:04.000000 pywb-2.7.4/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-19 18:25:04.000000 pywb-2.7.4/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)    81373 2023-05-19 18:25:04.000000 pywb-2.7.4/CHANGES.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-05-19 18:25:04.000000 pywb-2.7.4/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-05-19 18:25:04.000000 pywb-2.7.4/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-05-19 18:25:04.000000 pywb-2.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-19 18:25:04.000000 pywb-2.7.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-19 18:25:04.000000 pywb-2.7.4/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-05-19 18:25:16.290699 pywb-2.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-19 18:25:04.000000 pywb-2.7.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-19 18:25:04.000000 pywb-2.7.4/Vagrantfile
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-19 18:25:04.000000 pywb-2.7.4/appveyor.disabled.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      126 2023-05-19 18:25:04.000000 pywb-2.7.4/build-vue-ui.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      192 2023-05-19 18:25:04.000000 pywb-2.7.4/build-wombat.sh
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-19 18:25:04.000000 pywb-2.7.4/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-19 18:25:04.000000 pywb-2.7.4/docker-compose.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1115 2023-05-19 18:25:04.000000 pywb-2.7.4/docker-entrypoint.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.238695 pywb-2.7.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.242695 pywb-2.7.4/docs/code/
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/code/pywb.apps.rst
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/code/pywb.indexer.rst
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/code/pywb.manager.rst
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/code/pywb.recorder.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/code/pywb.rewrite.rst
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/code/pywb.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/code/pywb.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/code/pywb.warcserver.index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/code/pywb.warcserver.resource.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/code/pywb.warcserver.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.242695 pywb-2.7.4/docs/manual/
--rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/access-control.rst
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/apis.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/apps.rst
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/architecture.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10951 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/cdxserver_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)    27156 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/configuring.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/indexing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/localization.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/memento.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/migrating-cdx.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/outbackcdx.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/owb-pywb-terms.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10341 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/owb-to-pywb-config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/owb-to-pywb-deploy.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/owb-to-pywb-exclusions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/owb-transition.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/recorder.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/rewriter.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12846 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/template-guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/ui-customization.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/ui-guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15256 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/vue-ui.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-05-19 18:25:04.000000 pywb-2.7.4/docs/manual/warcserver.rst
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-19 18:25:04.000000 pywb-2.7.4/extra_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.242695 pywb-2.7.4/pywb/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.246695 pywb-2.7.4/pywb/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/apps/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    35411 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/apps/frontendapp.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/apps/live.py
--rw-r--r--   0 runner    (1001) docker     (123)    36153 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/apps/rewriterapp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/apps/static_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.246695 pywb-2.7.4/pywb/apps/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/apps/test/test_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/apps/test/test_wbrequestresponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/apps/warcserverapp.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/apps/wayback.py
--rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/apps/wbrequestresponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/default_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 18:25:15.000000 pywb-2.7.4/pywb/git_hash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.246695 pywb-2.7.4/pywb/indexer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/indexer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/indexer/archiveindexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14604 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/indexer/cdxindexer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.246695 pywb-2.7.4/pywb/indexer/test/
--rw-r--r--   0 runner    (1001) docker     (123)    26788 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/indexer/test/test_indexing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.246695 pywb-2.7.4/pywb/manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/manager/aclmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/manager/autoindex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/manager/locmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)    16485 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/manager/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/manager/migrate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.246695 pywb-2.7.4/pywb/recorder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/recorder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/recorder/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/recorder/multifilewarcwriter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/recorder/recorderapp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/recorder/redisindexer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.250695 pywb-2.7.4/pywb/recorder/test/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/recorder/test/rec.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/recorder/test/simplerec.py
--rw-r--r--   0 runner    (1001) docker     (123)    25051 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/recorder/test/test_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.250695 pywb-2.7.4/pywb/rewrite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17686 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/content_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/cookie_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/default_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/header_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/html_insert_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)    22051 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/html_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/jsonp_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13244 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/regex_rewriters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/rewrite_amf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/rewrite_dash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/rewrite_hls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/rewrite_js_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/rewriteinputreq.py
--rw-r--r--   0 runner    (1001) docker     (123)    17623 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/templateview.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.250695 pywb-2.7.4/pywb/rewrite/test/
--rw-r--r--   0 runner    (1001) docker     (123)    36556 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/test/test_content_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/test/test_cookie_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/test/test_header_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/test/test_html_insert_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)    23601 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/test/test_html_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/test/test_jsonp_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/test/test_regex_rewriters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/test/test_url_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/test/test_wburl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/url_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rewrite/wburl.py
--rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/rules.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.254696 pywb-2.7.4/pywb/static/
--rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/autoFetchWorker.js
--rw-r--r--   0 runner    (1001) docker     (123)    20175 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/calendar-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/calendar.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.254696 pywb-2.7.4/pywb/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/css/base.css
--rw-r--r--   0 runner    (1001) docker     (123)   153136 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    54636 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/css/font-awesome.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/css/query.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.254696 pywb-2.7.4/pywb/static/flowplayer/
--rw-r--r--   0 runner    (1001) docker     (123)   129773 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/flowplayer/flowplayer-3.2.18.swf
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/flowplayer/flowplayer.audio-3.2.11.swf
--rw-r--r--   0 runner    (1001) docker     (123)    38275 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/flowplayer/flowplayer.controls-3.2.16.swf
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/flowplayer/flowplayer.pseudostreaming-3.2.13.swf
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/flowplayer/toolbox.flashembed.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.258696 pywb-2.7.4/pywb/static/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.262696 pywb-2.7.4/pywb/static/fonts/font-awesome/
--rw-r--r--   0 runner    (1001) docker     (123)   125320 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)   660056 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)   125016 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    84568 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    72148 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    34388 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)   144523 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)    34092 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13608 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   186512 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (123)   816218 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (123)   186228 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    96248 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (123)    74320 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/font-awesome/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.262696 pywb-2.7.4/pywb/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    76308 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    86926 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/js/jquery-latest.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/js/url-polyfill.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.262696 pywb-2.7.4/pywb/static/loading-spinner/
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/loading-spinner/loading-spinner.js
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/loading-spinner/test.html
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/pywb-logo-sm.png
--rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/pywb-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    37329 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/query.js
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/queryWorker.js
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/scroll-webkit.css
--rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/search.js
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/timeline-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/transclusions.js
--rw-r--r--   0 runner    (1001) docker     (123)    22029 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/vidrw.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.262696 pywb-2.7.4/pywb/static/vue/
--rw-r--r--   0 runner    (1001) docker     (123)  1574967 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/vue/vueui.js
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/vue_banner.css
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/wb_frame.js
--rw-r--r--   0 runner    (1001) docker     (123)   128535 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/wombat.js
--rw-r--r--   0 runner    (1001) docker     (123)    15514 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/wombatProxyMode.js
--rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/wombatWorkers.js
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/static/zoom-out-icon-333316.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.266697 pywb-2.7.4/pywb/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/banner.html
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/bootstrap_jquery.html
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/collinfo.json
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/custom_banner.html
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/frame_insert.html
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/head.html
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/head_insert.html
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/header.html
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    15304 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/instructions.html
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/not_found.html
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/proxy_cert_download.html
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/proxy_select.html
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/query.html
--rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/templates/vue_loc.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.266697 pywb-2.7.4/pywb/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/utils/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/utils/binsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/utils/canonicalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/utils/geventserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    14378 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/utils/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/utils/memento.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/utils/merge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.270697 pywb-2.7.4/pywb/utils/test/
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/utils/test/test_binsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/utils/test/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/utils/wbexception.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.234694 pywb-2.7.4/pywb/vueui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.234694 pywb-2.7.4/pywb/vueui/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.270697 pywb-2.7.4/pywb/vueui/src/cdx-simulator/
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/vueui/src/cdx-simulator/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.270697 pywb-2.7.4/pywb/warcserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12024 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/access_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/amf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/basewarcserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.270697 pywb-2.7.4/pywb/warcserver/index/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/cdxobject.py
--rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/cdxops.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/fuzzymatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    24183 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/indexsource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.270697 pywb-2.7.4/pywb/warcserver/index/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/test/test_cdxobject.py
--rw-r--r--   0 runner    (1001) docker     (123)    20273 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/test/test_cdxops.py
--rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/test/test_dir_agg.py
--rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/test/test_fuzzymatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/test/test_indexsource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/test/test_lazy_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/test/test_memento_agg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/test/test_redis_agg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/test/test_timeouts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/test/test_xmlquery_indexsource.py
--rw-r--r--   0 runner    (1001) docker     (123)    13783 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/test/test_zipnum.py
--rw-r--r--   0 runner    (1001) docker     (123)    12327 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/index/zipnum.py
--rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/inputrequest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.274697 pywb-2.7.4/pywb/warcserver/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/resource/blockrecordloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/resource/pathresolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/resource/resolvingloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    20858 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/resource/responseloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.274697 pywb-2.7.4/pywb/warcserver/resource/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/resource/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15994 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/resource/test/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/resource/test/test_pathresolvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.274697 pywb-2.7.4/pywb/warcserver/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/test/live.ini
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/test/test_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/test/test_amf.py
--rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/test/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/test/test_inputreq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/test/test_upstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/test/test_warcserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/test/test_warcserver_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/test/testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/upstreamindexsource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11691 2023-05-19 18:25:04.000000 pywb-2.7.4/pywb/warcserver/warcserver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.246695 pywb-2.7.4/pywb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-05-19 18:25:16.000000 pywb-2.7.4/pywb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-05-19 18:25:16.000000 pywb-2.7.4/pywb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:25:16.000000 pywb-2.7.4/pywb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-19 18:25:16.000000 pywb-2.7.4/pywb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:25:16.000000 pywb-2.7.4/pywb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-19 18:25:16.000000 pywb-2.7.4/pywb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-19 18:25:16.000000 pywb-2.7.4/pywb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-19 18:25:04.000000 pywb-2.7.4/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      183 2023-05-19 18:25:04.000000 pywb-2.7.4/run-gunicorn.sh
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-19 18:25:04.000000 pywb-2.7.4/run-tests.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-05-19 18:25:04.000000 pywb-2.7.4/run-uwsgi.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.234694 pywb-2.7.4/sample_archive/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.274697 pywb-2.7.4/sample_archive/access/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/access/allows.aclj
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/access/blocks.aclj
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/access/list1.aclj
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/access/list2.aclj
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/access/pywb.aclj
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/access/single-line.aclj
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.274697 pywb-2.7.4/sample_archive/cdx/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/cdx/bad.cdx
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/cdx/dupes.cdx
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/cdx/example-arc-test.cdx
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/cdx/example-extra.cdx
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/cdx/example.cdx
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/cdx/httpbin-resource.cdxj
--rw-r--r--   0 runner    (1001) docker     (123)    30399 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/cdx/iana.cdx
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/cdx/missing-status-text.cdxj
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/cdx/post-test.cdx
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/cdx/url-agnost-example.cdx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.278698 pywb-2.7.4/sample_archive/cdxj/
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/cdxj/dupes.cdxj
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/cdxj/example-no-digest.cdxj
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/cdxj/example.cdxj
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-19 18:25:04.000000 pywb-2.7.4/sample_archive/cdxj/example2.cdxj
--rw-r--r--   0 runner    (1001) docker     (123)    43062 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/cdxj/iana.cdxj
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/cdxj/post-test.cdxj
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/cdxj/url-agnost-example.cdxj
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.278698 pywb-2.7.4/sample_archive/non-surt-cdx/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/non-surt-cdx/example-non-surt.cdx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.278698 pywb-2.7.4/sample_archive/text_content/
--rw-r--r--   0 runner    (1001) docker     (123)    13676 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/text_content/link_headers.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/text_content/pathindex.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/text_content/quickfox_repeated.compressed
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/text_content/sample.html
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/text_content/sample_dash.mpd
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/text_content/sample_hls.m3u8
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/text_content/sample_no_head.html
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/text_content/sample_no_head_2.html
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/text_content/sample_unclosed_script.html
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/text_content/toptest.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.282698 pywb-2.7.4/sample_archive/warcs/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/bad.arc
--rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/dupes.warc.gz
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/example-bad.warc.gz.bad
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/example-extra.warc
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/example-url-agnostic-orig.warc.gz
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/example-url-agnostic-revisit.warc.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/example-wget-1-14.warc.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/example-wpull.warc.gz
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/example.arc
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/example.arc.gz
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/example.warc
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/example.warc.gz
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/example2.warc.gz
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/httpbin-resource.warc.gz
--rw-r--r--   0 runner    (1001) docker     (123)   786828 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/iana.warc.gz
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/missing-status-text.warc
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/warcs/post-test.warc.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.282698 pywb-2.7.4/sample_archive/zipcdx/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/zipcdx/zipnum-bad.idx
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/zipcdx/zipnum-bad.loc
--rw-r--r--   0 runner    (1001) docker     (123)     9797 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/zipcdx/zipnum-sample.cdx.gz
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/zipcdx/zipnum-sample.idx
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-19 18:25:05.000000 pywb-2.7.4/sample_archive/zipcdx/zipnum-sample.loc
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 18:25:16.290699 pywb-2.7.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4886 2023-05-19 18:25:05.000000 pywb-2.7.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-19 18:25:05.000000 pywb-2.7.4/test_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.286698 pywb-2.7.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/base_config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/config_test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/config_test_access.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/config_test_cert_req.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/config_test_loc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/config_test_record.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/config_test_record_dedup.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/config_test_redirect_classic.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/config_test_root_coll.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.234694 pywb-2.7.4/tests/i18n-data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.234694 pywb-2.7.4/tests/i18n-data/l337/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.286698 pywb-2.7.4/tests/i18n-data/l337/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/i18n-data/l337/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/memento_fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_acl_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    19956 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_auto_colls.py
--rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_cdx_server_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_cert_req.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_embargo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_force_https.py
--rw-r--r--   0 runner    (1001) docker     (123)    25129 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_live_rewriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_locales.py
--rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_memento.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_prefer_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_prefixed_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)    19147 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_record_dedup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_record_replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_redirect_classic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_redirect_revisits.py
--rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_redirects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_root_coll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_socks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-05-19 18:25:05.000000 pywb-2.7.4/tests/test_zipnum_auto_dir.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:25:16.290699 pywb-2.7.4/tests_disabled/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/live.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/perms_fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/server_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/server_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_cdxserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_config_frames.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_config_memento.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_config_proxy_http_cookie.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_config_proxy_https_cookie.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_config_proxy_ip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_config_proxy_ip_redis.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_config_proxy_no_banner.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_config_root_coll.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_live_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    17290 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_memento.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_perms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_perms_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_proxy_http_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_proxy_http_cookie.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_proxy_http_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_proxy_http_ip_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_proxy_http_no_banner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_proxy_https_cookie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-19 18:25:05.000000 pywb-2.7.4/tests_disabled/test_rewrite_content.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      178 2023-05-19 18:25:05.000000 pywb-2.7.4/update-tag.sh
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-19 18:25:05.000000 pywb-2.7.4/uwsgi.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.310810 pywb-2.8.0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      316 2024-04-24 12:25:48.000000 pywb-2.8.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-24 12:25:48.000000 pywb-2.8.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-24 12:25:48.000000 pywb-2.8.0/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    81373 2024-04-24 12:25:48.000000 pywb-2.8.0/CHANGES.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      619 2024-04-24 12:25:48.000000 pywb-2.8.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-04-24 12:25:48.000000 pywb-2.8.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35121 2024-04-24 12:25:48.000000 pywb-2.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-24 12:25:48.000000 pywb-2.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-24 12:25:48.000000 pywb-2.8.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-04-24 12:25:57.310810 pywb-2.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-24 12:25:48.000000 pywb-2.8.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-24 12:25:48.000000 pywb-2.8.0/Vagrantfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-24 12:25:48.000000 pywb-2.8.0/appveyor.disabled.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      126 2024-04-24 12:25:48.000000 pywb-2.8.0/build-vue-ui.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      192 2024-04-24 12:25:48.000000 pywb-2.8.0/build-wombat.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-24 12:25:48.000000 pywb-2.8.0/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-24 12:25:48.000000 pywb-2.8.0/docker-compose.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1115 2024-04-24 12:25:48.000000 pywb-2.8.0/docker-entrypoint.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.250810 pywb-2.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.254810 pywb-2.8.0/docs/code/
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/code/pywb.apps.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/code/pywb.indexer.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/code/pywb.manager.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/code/pywb.recorder.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/code/pywb.rewrite.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/code/pywb.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/code/pywb.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/code/pywb.warcserver.index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/code/pywb.warcserver.resource.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/code/pywb.warcserver.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.258810 pywb-2.8.0/docs/manual/
+-rw-r--r--   0 runner    (1001) docker     (127)    11121 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/access-control.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/apis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/apps.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/architecture.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10951 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/cdxserver_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    27156 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/configuring.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/indexing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/localization.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/memento.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/migrating-cdx.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/outbackcdx.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/owb-pywb-terms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10341 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/owb-to-pywb-config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/owb-to-pywb-deploy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/owb-to-pywb-exclusions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/owb-transition.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/recorder.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/rewriter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12846 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/template-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/ui-customization.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/ui-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    16666 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/vue-ui.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12367 2024-04-24 12:25:48.000000 pywb-2.8.0/docs/manual/warcserver.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 12:25:48.000000 pywb-2.8.0/extra_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.258810 pywb-2.8.0/pywb/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.258810 pywb-2.8.0/pywb/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/apps/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35718 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/apps/frontendapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/apps/live.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36131 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/apps/rewriterapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/apps/static_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.262810 pywb-2.8.0/pywb/apps/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/apps/test/test_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/apps/test/test_wbrequestresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/apps/warcserverapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/apps/wayback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8584 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/apps/wbrequestresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/default_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 12:25:56.000000 pywb-2.8.0/pywb/git_hash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.262810 pywb-2.8.0/pywb/indexer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/indexer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11456 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/indexer/archiveindexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14604 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/indexer/cdxindexer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.262810 pywb-2.8.0/pywb/indexer/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    26788 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/indexer/test/test_indexing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.262810 pywb-2.8.0/pywb/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11183 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/manager/aclmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/manager/autoindex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/manager/locmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22199 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/manager/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/manager/migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.262810 pywb-2.8.0/pywb/recorder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/recorder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/recorder/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/recorder/multifilewarcwriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11083 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/recorder/recorderapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/recorder/redisindexer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.262810 pywb-2.8.0/pywb/recorder/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/recorder/test/rec.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/recorder/test/simplerec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25051 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/recorder/test/test_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.266810 pywb-2.8.0/pywb/rewrite/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17686 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/content_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/cookie_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/default_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/header_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/html_insert_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22052 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/html_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/jsonp_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13030 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/regex_rewriters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/rewrite_amf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/rewrite_dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/rewrite_hls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/rewrite_js_workers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/rewriteinputreq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17726 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/templateview.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.266810 pywb-2.8.0/pywb/rewrite/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    36556 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/test/test_content_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/test/test_cookie_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/test/test_header_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/test/test_html_insert_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23601 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/test/test_html_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/test/test_jsonp_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14291 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/test/test_regex_rewriters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/test/test_url_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11273 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/test/test_wburl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/url_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9806 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rewrite/wburl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13671 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/rules.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.270810 pywb-2.8.0/pywb/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/autoFetchWorker.js
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/calendar.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.270810 pywb-2.8.0/pywb/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/css/base.css
+-rw-r--r--   0 runner    (1001) docker     (127)   153136 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    54636 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/css/font-awesome.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/css/query.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.270810 pywb-2.8.0/pywb/static/flowplayer/
+-rw-r--r--   0 runner    (1001) docker     (127)   129773 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/flowplayer/flowplayer-3.2.18.swf
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/flowplayer/flowplayer.audio-3.2.11.swf
+-rw-r--r--   0 runner    (1001) docker     (127)    38275 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/flowplayer/flowplayer.controls-3.2.16.swf
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/flowplayer/flowplayer.pseudostreaming-3.2.13.swf
+-rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/flowplayer/toolbox.flashembed.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.270810 pywb-2.8.0/pywb/static/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.278810 pywb-2.8.0/pywb/static/fonts/font-awesome/
+-rw-r--r--   0 runner    (1001) docker     (127)   125320 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   660056 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   125016 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    84568 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    72148 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    34388 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   144523 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    34092 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16812 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13608 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   186512 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   816218 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   186228 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    96248 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    74320 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/font-awesome/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    20127 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   108738 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    45404 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    23424 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.278810 pywb-2.8.0/pywb/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    76308 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    86926 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/js/jquery-latest.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/js/url-polyfill.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.278810 pywb-2.8.0/pywb/static/loading-spinner/
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/loading-spinner/loading-spinner.js
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/loading-spinner/test.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/pywb-logo-sm.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10492 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/pywb-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    37329 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/query.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/queryWorker.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/scroll-webkit.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6950 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/search.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/transclusions.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22029 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/vidrw.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.278810 pywb-2.8.0/pywb/static/vue/
+-rw-r--r--   0 runner    (1001) docker     (127)  1577587 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/vue/vueui.js
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/vue_banner.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8654 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/wb_frame.js
+-rw-r--r--   0 runner    (1001) docker     (127)   130193 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/wombat.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15514 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/wombatProxyMode.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8893 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/static/wombatWorkers.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.282810 pywb-2.8.0/pywb/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/banner.html
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/bootstrap_jquery.html
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/collinfo.json
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/custom_banner.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/frame_insert.html
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/head.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/head_insert.html
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/header.html
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    15304 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/instructions.html
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/not_found.html
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/proxy_cert_download.html
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/proxy_select.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/query.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/templates/vue_loc.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.286810 pywb-2.8.0/pywb/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/utils/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/utils/binsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/utils/canonicalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/utils/geventserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14378 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/utils/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/utils/memento.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/utils/merge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.286810 pywb-2.8.0/pywb/utils/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/utils/test/test_binsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/utils/test/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/utils/wbexception.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.246810 pywb-2.8.0/pywb/vueui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.246810 pywb-2.8.0/pywb/vueui/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.286810 pywb-2.8.0/pywb/vueui/src/cdx-simulator/
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/vueui/src/cdx-simulator/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.286810 pywb-2.8.0/pywb/warcserver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12158 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/access_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/amf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/basewarcserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.286810 pywb-2.8.0/pywb/warcserver/index/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9008 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/cdxobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9816 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/cdxops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/fuzzymatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24183 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/indexsource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.290810 pywb-2.8.0/pywb/warcserver/index/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/test/test_cdxobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20273 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/test/test_cdxops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8987 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/test/test_dir_agg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/test/test_fuzzymatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8986 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/test/test_indexsource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/test/test_lazy_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15181 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/test/test_memento_agg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/test/test_redis_agg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/test/test_timeouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/test/test_xmlquery_indexsource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13783 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/test/test_zipnum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12327 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/index/zipnum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9770 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/inputrequest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.290810 pywb-2.8.0/pywb/warcserver/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/resource/blockrecordloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/resource/pathresolvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9310 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/resource/resolvingloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20858 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/resource/responseloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.290810 pywb-2.8.0/pywb/warcserver/resource/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/resource/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15994 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/resource/test/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/resource/test/test_pathresolvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.290810 pywb-2.8.0/pywb/warcserver/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/test/live.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/test/test_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/test/test_amf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22680 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/test/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/test/test_inputreq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/test/test_upstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/test/test_warcserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/test/test_warcserver_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/test/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/upstreamindexsource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11691 2024-04-24 12:25:48.000000 pywb-2.8.0/pywb/warcserver/warcserver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.258810 pywb-2.8.0/pywb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-04-24 12:25:57.000000 pywb-2.8.0/pywb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12313 2024-04-24 12:25:57.000000 pywb-2.8.0/pywb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 12:25:57.000000 pywb-2.8.0/pywb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-24 12:25:57.000000 pywb-2.8.0/pywb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 12:25:57.000000 pywb-2.8.0/pywb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-24 12:25:57.000000 pywb-2.8.0/pywb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 12:25:57.000000 pywb-2.8.0/pywb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-24 12:25:48.000000 pywb-2.8.0/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      183 2024-04-24 12:25:48.000000 pywb-2.8.0/run-gunicorn.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-24 12:25:48.000000 pywb-2.8.0/run-tests.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      283 2024-04-24 12:25:48.000000 pywb-2.8.0/run-uwsgi.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.246810 pywb-2.8.0/sample_archive/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.294810 pywb-2.8.0/sample_archive/access/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/access/allow_all.aclj
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/access/allows.aclj
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/access/blocks.aclj
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/access/list1.aclj
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/access/list2.aclj
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/access/pywb.aclj
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/access/single-line.aclj
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.294810 pywb-2.8.0/sample_archive/cdx/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdx/bad.cdx
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdx/dupes.cdx
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdx/example-arc-test.cdx
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdx/example-extra.cdx
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdx/example.cdx
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdx/httpbin-resource.cdxj
+-rw-r--r--   0 runner    (1001) docker     (127)    30399 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdx/iana.cdx
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdx/missing-status-text.cdxj
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdx/post-test.cdx
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdx/url-agnost-example.cdx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.294810 pywb-2.8.0/sample_archive/cdxj/
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdxj/dupes.cdxj
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdxj/example-no-digest.cdxj
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdxj/example.cdx.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdxj/example.cdxj
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdxj/example2.cdxj
+-rw-r--r--   0 runner    (1001) docker     (127)    43062 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdxj/iana.cdxj
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdxj/post-test.cdxj
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/cdxj/url-agnost-example.cdxj
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.294810 pywb-2.8.0/sample_archive/non-surt-cdx/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/non-surt-cdx/example-non-surt.cdx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.298810 pywb-2.8.0/sample_archive/text_content/
+-rw-r--r--   0 runner    (1001) docker     (127)    13676 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/text_content/link_headers.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/text_content/pathindex.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/text_content/quickfox_repeated.compressed
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/text_content/sample.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/text_content/sample_dash.mpd
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/text_content/sample_hls.m3u8
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/text_content/sample_no_head.html
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/text_content/sample_no_head_2.html
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/text_content/sample_unclosed_script.html
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/text_content/toptest.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.298810 pywb-2.8.0/sample_archive/warcs/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/bad.arc
+-rw-r--r--   0 runner    (1001) docker     (127)    12905 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/dupes.warc.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/example-bad.warc.gz.bad
+-rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/example-extra.warc
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/example-url-agnostic-orig.warc.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/example-url-agnostic-revisit.warc.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/example-wget-1-14.warc.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/example-wpull.warc.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/example.arc
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/example.arc.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/example.warc
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/example.warc.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/example2.warc.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/httpbin-resource.warc.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   786828 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/iana.warc.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/missing-status-text.warc
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/warcs/post-test.warc.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.302810 pywb-2.8.0/sample_archive/zipcdx/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/zipcdx/zipnum-bad.idx
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/zipcdx/zipnum-bad.loc
+-rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/zipcdx/zipnum-sample.cdx.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/zipcdx/zipnum-sample.idx
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 12:25:48.000000 pywb-2.8.0/sample_archive/zipcdx/zipnum-sample.loc
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 12:25:57.310810 pywb-2.8.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4729 2024-04-24 12:25:48.000000 pywb-2.8.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-24 12:25:48.000000 pywb-2.8.0/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.306810 pywb-2.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/base_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/config_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/config_test_access.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/config_test_cert_req.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/config_test_loc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/config_test_record.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/config_test_record_dedup.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/config_test_redirect_classic.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/config_test_root_coll.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.246810 pywb-2.8.0/tests/i18n-data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.246810 pywb-2.8.0/tests/i18n-data/l337/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.306810 pywb-2.8.0/tests/i18n-data/l337/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/i18n-data/l337/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/memento_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_acl_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19956 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_auto_colls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_cdx_server_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_cert_req.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_embargo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_force_https.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25129 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8676 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_live_rewriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_locales.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12071 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_memento.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10613 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_prefer_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_prefixed_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19147 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_record_dedup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_record_replay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_redirect_classic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_redirect_revisits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_redirects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_root_coll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_socks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-24 12:25:48.000000 pywb-2.8.0/tests/test_zipnum_auto_dir.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 12:25:57.310810 pywb-2.8.0/tests_disabled/
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/live.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/perms_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/server_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/server_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_cdxserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_config_frames.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_config_memento.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_config_proxy_http_cookie.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_config_proxy_https_cookie.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_config_proxy_ip.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_config_proxy_ip_redis.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_config_proxy_no_banner.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_config_root_coll.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_live_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17290 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_memento.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_perms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_perms_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_proxy_http_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_proxy_http_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_proxy_http_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_proxy_http_ip_redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_proxy_http_no_banner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_proxy_https_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-24 12:25:48.000000 pywb-2.8.0/tests_disabled/test_rewrite_content.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-04-24 12:25:48.000000 pywb-2.8.0/update-tag.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-24 12:25:48.000000 pywb-2.8.0/uwsgi.ini
```

### Comparing `pywb-2.7.4/.travis.yml` & `pywb-2.8.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/CHANGES.rst` & `pywb-2.8.0/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1177,15 +1177,15 @@
 
 * fix typo in wombat ``no_rewrite_prefixes``
 
 
 pywb 0.9.5 changelist
 ~~~~~~~~~~~~~~~~~~~~~
 
-* s3 loading: support ``s3://`` scheme in block loader, allowing for loading index and archive files from s3. ``boto`` library must be installed seperately
+* s3 loading: support ``s3://`` scheme in block loader, allowing for loading index and archive files from s3. ``boto`` library must be installed separately
   via ``pip install boto``. Attempt default boto auth path, and if that fails, attempt anonymous s3 connection.
   
 * Wombat/Client-Side Rewrite Customizations: New ``rewrite_opts.client`` settings from ``config.yaml`` are passed directly to wombat as json. 
   
   Allows for customizing wombat as needed. Currently supported options are: ``no_rewrite_prefixes`` for ignoring rewrite
   on certain domains, and ``skip_dom``, ``skip_setAttribute`` and ``skip_postmessage`` options for disabling 
   those overrides. Example usage in config:
@@ -1273,15 +1273,15 @@
 
 * Implement pagination support for zipnum cluster and added to cdx server api:
 
   https://github.com/ikreymer/pywb/wiki/CDX-Server-API
 
 * cdx server query: add support for ``url=*.host`` and ``url=host/*`` as shortcuts for ``matchType=domain`` and ``matchType=prefix``
 
-* zipnum cdx cluster: support loading index shared from prefix path instead of seperate location file.
+* zipnum cdx cluster: support loading index shared from prefix path instead of separate location file.
 
   The ``shard_index_loc`` config property may contain match and replace properties.
   Regex replacement is then used to obtain path prefix from the shard prefix path.
 
 * wombat: fix `document.write()` rewriting to rewrite each element at a time and use underlying write for better compatibility.
 
 
@@ -1639,15 +1639,15 @@
 
 * Tests: Additional testing of bad cdx lines, missing revisit records.
 
 * Rewrite: Removal of lxml support for now, as it leads to problematic replay and not much performance improvements.
 
 * Rewrite: Parsing of html as raw bytes instead of decode/encode, detection still needed for non-ascii compatible encoding.
 
-* Indexing: Refactoring of cdx-indexer using a seperate 'archive record iterator' and pluggable cdx writer classes. Groundwork for creating custom indexers.
+* Indexing: Refactoring of cdx-indexer using a separate 'archive record iterator' and pluggable cdx writer classes. Groundwork for creating custom indexers.
 
 * Indexing: Support for 9 field cdx formats with -9 flag.
 
 * Rewrite: Improved top -> WB_wombat_top rewriting.
 
 * Rewrite: Better handling of framed replay url notification
```

### Comparing `pywb-2.7.4/Dockerfile` & `pywb-2.8.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/INSTALL.rst` & `pywb-2.8.0/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/LICENSE` & `pywb-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/MANIFEST.in` & `pywb-2.8.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/PKG-INFO` & `pywb-2.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 Metadata-Version: 2.1
 Name: pywb
-Version: 2.7.4
+Version: 2.8.0
 Summary: Pywb Webrecorder web archive replay and capture tools
 Home-page: https://github.com/webrecorder/pywb
 Author: Ilya Kreymer
 Author-email: ikreymer@gmail.com
 License: GPL
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: Proxy Servers
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Server
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving
 Classifier: Topic :: System :: Archiving :: Backup
 Classifier: Topic :: Utilities
+Requires-Python: >=3.7,<3.12
 Provides-Extra: i18n
 License-File: LICENSE
 License-File: NOTICE
 
-Webrecorder pywb 2.7
+Webrecorder pywb 2.8
 ====================
 
 .. image:: https://raw.githubusercontent.com/webrecorder/pywb/main/pywb/static/pywb-logo.png
 
 .. image:: https://github.com/webrecorder/pywb/workflows/CI/badge.svg
       :target: https://github.com/webrecorder/pywb/actions
 .. image:: https://codecov.io/gh/webrecorder/pywb/branch/main/graph/badge.svg
@@ -93,27 +90,23 @@
 
 
 Installation for Deployment
 ---------------------------
 
 To install pywb for usage, you can use:
 
-```shell
-pip install pywb
-```
+``pip install pywb``
 
 Note: depending on your Python installation, you may have to use `pip3` instead of `pip`.
 
 
 Installation from local copy
 ----------------------------
 
-```shell
-git clone https://github.com/webrecorder/pywb
-```
+``git clone https://github.com/webrecorder/pywb``
 
 To install from a locally cloned copy, install with ``pip install -e .`` or ``python setup.py install``.
 
 To run tests, we recommend installing ``pip install tox tox-current-env`` and then running ``tox --current-env`` to test in your current Python environment.
 
 To Build docs locally, run:  ``cd docs; make html``. (The docs will be built in ``./_build/html/index.html``)
```

### Comparing `pywb-2.7.4/README.rst` & `pywb-2.8.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Webrecorder pywb 2.7
+Webrecorder pywb 2.8
 ====================
 
 .. image:: https://raw.githubusercontent.com/webrecorder/pywb/main/pywb/static/pywb-logo.png
 
 .. image:: https://github.com/webrecorder/pywb/workflows/CI/badge.svg
       :target: https://github.com/webrecorder/pywb/actions
 .. image:: https://codecov.io/gh/webrecorder/pywb/branch/main/graph/badge.svg
@@ -56,27 +56,23 @@
 
 
 Installation for Deployment
 ---------------------------
 
 To install pywb for usage, you can use:
 
-```shell
-pip install pywb
-```
+``pip install pywb``
 
 Note: depending on your Python installation, you may have to use `pip3` instead of `pip`.
 
 
 Installation from local copy
 ----------------------------
 
-```shell
-git clone https://github.com/webrecorder/pywb
-```
+``git clone https://github.com/webrecorder/pywb``
 
 To install from a locally cloned copy, install with ``pip install -e .`` or ``python setup.py install``.
 
 To run tests, we recommend installing ``pip install tox tox-current-env`` and then running ``tox --current-env`` to test in your current Python environment.
 
 To Build docs locally, run:  ``cd docs; make html``. (The docs will be built in ``./_build/html/index.html``)
```

### Comparing `pywb-2.7.4/Vagrantfile` & `pywb-2.8.0/Vagrantfile`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/appveyor.disabled.yml` & `pywb-2.8.0/appveyor.disabled.yml`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/config.yaml` & `pywb-2.8.0/config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # Uncomment to set banner colors and logo
 # ui:
   # logo: path/relative/from/static/logo.png
   # logo_home_url: https://example.com
   # navbar_background_hex: 0c49b0
   # navbar_color_hex: fff
   # navbar_light_buttons: true
+  # disable_printing: true
 
 collections:
     all: $all
     pywb:
         index_paths: ./sample_archive/cdx/
         archive_paths: ./sample_archive/warcs/
```

### Comparing `pywb-2.7.4/docker-entrypoint.sh` & `pywb-2.8.0/docker-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/docs/Makefile` & `pywb-2.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/docs/code/pywb.apps.rst` & `pywb-2.8.0/docs/code/pywb.apps.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/docs/code/pywb.manager.rst` & `pywb-2.8.0/docs/code/pywb.manager.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/docs/code/pywb.recorder.rst` & `pywb-2.8.0/docs/code/pywb.recorder.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/docs/code/pywb.rewrite.rst` & `pywb-2.8.0/docs/code/pywb.rewrite.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/docs/code/pywb.utils.rst` & `pywb-2.8.0/docs/code/pywb.utils.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/docs/code/pywb.warcserver.index.rst` & `pywb-2.8.0/docs/code/pywb.warcserver.index.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/docs/code/pywb.warcserver.resource.rst` & `pywb-2.8.0/docs/code/pywb.warcserver.resource.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/docs/code/pywb.warcserver.rst` & `pywb-2.8.0/docs/code/pywb.warcserver.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/docs/conf.py` & `pywb-2.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/docs/index.rst` & `pywb-2.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/docs/make.bat` & `pywb-2.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/docs/manual/access-control.rst` & `pywb-2.8.0/docs/manual/access-control.rst`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,20 @@
 
 Given these rules, a user would:
 
 * be allowed to visit ``http://httpbin.org/anything/something`` (allow)
 * but would receive an 'access blocked' error message when viewing ``http://httpbin.org/`` (block)
 * would receive a 404 not found error when viewing ``http://httpbin.org/anything`` (exclude)
 
+To match any possible URL in an .aclj file, set ``*,`` as the leading SURT, for example::
+
+  *, - {"access": "allow"}
+
+Lines starting with ``*,`` should generally be at the end of the file, respecting the reverse alphabetical order.
+
 
 Access Types: allow, block, exclude, allow_ignore_embargo
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The available access types are as follows:
 
 - ``exclude`` - when matched, results are excluded from the index, as if they do not exist. User will receive a 404.
@@ -145,14 +151,18 @@
   com,example)/restricted - {"access": "allow_ignore_embargo", "user": "staff"}
   com,example)/restricted - {"access": "allow"}
 
 To make this work, pywb must be running behind an Apache or Nginx system that is configured to set ``X-Pywb-ACL-User: staff`` based on certain settings.
 
 For example, this header may be set based on IP range, or based on password authentication.
 
+To allow a user access to all URLs, overriding more specific rules and the ``default_access`` configuration setting, use the ``*,`` SURT::
+
+  *, - {"access": "allow", "user": "staff"}
+
 Further examples of how to set this header will be provided in the deployments section.
 
 **Note: Do not use the user-based rules without configuring proper authentication on an Apache or Nginx frontend to set or remove this header, otherwise the 'X-Pywb-ACL-User' can easily be faked.**
 
 See the :ref:`config-acl-header` section in Usage for examples on how to configure this header.
```

### Comparing `pywb-2.7.4/docs/manual/apps.rst` & `pywb-2.8.0/docs/manual/apps.rst`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 
 The tool can be used while ``wayback`` is running, and pywb will detect many changes automatically.
 
 It can be used to:
 
 * Create a new collection --  ``wb-manager init <coll>``
 * Add WARCs to collection -- ``wb-manager add <coll> <warc>``
+* Unpack WACZs to add their WARCs and indices to collection -- ``wb-manager add --unpack-wacz <coll> <wacz>``
 * Add override templates
 * Add and remove metadata to a collections ``metadata.yaml``
 * List all collections
 * Reindex a collection
 * Migrate old CDX to CDXJ style indexes.
 
 For more details, run ``wb-manager -h``.
```

### Comparing `pywb-2.7.4/docs/manual/cdxserver_api.rst` & `pywb-2.8.0/docs/manual/cdxserver_api.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/docs/manual/configuring.rst` & `pywb-2.8.0/docs/manual/configuring.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/docs/manual/indexing.rst` & `pywb-2.8.0/docs/manual/indexing.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/docs/manual/localization.rst` & `pywb-2.8.0/docs/manual/localization.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/docs/manual/memento.rst` & `pywb-2.8.0/docs/manual/memento.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/docs/manual/migrating-cdx.rst` & `pywb-2.8.0/docs/manual/migrating-cdx.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/docs/manual/outbackcdx.rst` & `pywb-2.8.0/docs/manual/outbackcdx.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/docs/manual/owb-pywb-terms.rst` & `pywb-2.8.0/docs/manual/owb-pywb-terms.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/docs/manual/owb-to-pywb-config.rst` & `pywb-2.8.0/docs/manual/owb-to-pywb-config.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/docs/manual/owb-to-pywb-deploy.rst` & `pywb-2.8.0/docs/manual/owb-to-pywb-deploy.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/docs/manual/owb-to-pywb-exclusions.rst` & `pywb-2.8.0/docs/manual/owb-to-pywb-exclusions.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/docs/manual/recorder.rst` & `pywb-2.8.0/docs/manual/recorder.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/docs/manual/rewriter.rst` & `pywb-2.8.0/docs/manual/rewriter.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/docs/manual/template-guide.rst` & `pywb-2.8.0/docs/manual/template-guide.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/docs/manual/ui-guide.rst` & `pywb-2.8.0/docs/manual/ui-guide.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/docs/manual/usage.rst` & `pywb-2.8.0/docs/manual/usage.rst`

 * *Files 4% similar despite different names*

```diff
@@ -91,16 +91,16 @@
 For example, give a WARC at ``/path/to/my_warc.warc.gz`` and a pywb data directory of ``/pywb-data``, the following will
 add the WARC to a new collection and start pywb:
 
 .. code:: console
 
       docker pull webrecorder/pywb
       docker run -e INIT_COLLECTION=my-web-archive -v /pywb-data:/webarchive \
-         -v /path/to:/source webrecorder/pywb wb-manager add default /path/to/my_warc.warc.gz
-      docker run -p 8080:8080 -v /pywb-data/:/webarchive wayback
+         -v /path/to:/source webrecorder/pywb wb-manager add my-web-archive /source/my_warc.warc.gz
+      docker run -p 8080:8080 -v /pywb-data/:/webarchive webrecorder/pywb wayback
 
 This example is equivalent to the non-Docker example above.
 
 Setting ``INIT_COLLECTION=my-web-archive`` results in automatic collection initializiation via ``wb-manager init my-web-archive``.
 
 The ``wayback`` command is launched on port 8080 and mapped to the same on the local host.
 
@@ -110,14 +110,16 @@
 
 Using Existing Web Archive Collections
 --------------------------------------
 
 Existing archives of WARCs/ARCs files can be used with pywb with minimal amount of setup. By using ``wb-manager add``,
 WARC/ARC files will automatically be placed in the collection archive directory and indexed.
 
+In pywb 2.8.0 and later, preliminary support for WACZ files is also added with ``wb-manager add --unpack-wacz``. This will unpack the provided WACZ file, adding its WARCs and indices to the collection.
+
 By default ``wb-manager``, places new collections in ``collections/<coll name>`` subdirectory in the current working directory. To specify a different root directory, the ``wb-manager -d <dir>``. Other options can be set in the config file.
 
 If you have a large number of existing CDX index files, pywb will be able to read them as well after running through a simple conversion process.
 
 It is recommended that any index files be converted to the latest CDXJ format, which can be done by running:
 ``wb-manager cdx-convert <path/to/cdx>``
 
@@ -150,40 +152,48 @@
 
 
 .. _creating-warc:
 
 Creating a Web Archive
 ----------------------
 
-Using Webrecorder
-^^^^^^^^^^^^^^^^^
+Using ArchiveWeb.page
+^^^^^^^^^^^^^^^^^^^^^
 
-If you do not have a web archive to test, one easy way to create one is to use `Webrecorder <https://webrecorder.io>`_
+If you do not have a web archive to test, one easy way to create one is to use the `ArchiveWeb.page <https://archiveweb.page>`_ browser extension for Chrome and other Chromium-based browsers such as Brave Browser. ArchiveWeb.page records pages visited during an archiving session in the browser, and provides means of both replaying and downloading the archived items created.
 
-After recording, you can click **Stop** and then click `Download Collection` to receive a WARC (`.warc.gz`) file.
+Follow the instructions in `How To Create Web Archives with ArchiveWeb.page <https://archiveweb.page/en/usage/>`_. After recording, press **Stop** and then `download your collection <https://archiveweb.page/en/download/>`_ to receive a WARC (`.warc.gz`) file. If you choose to download your collection in the WACZ format, the WARC files can be found inside the zipped WACZ in the ``archive/`` directory.
 
-You can then use this with work with pywb.
+You can then use your WARCs to work with pywb.
 
 
 Using pywb Recorder
 ^^^^^^^^^^^^^^^^^^^
 
-The core recording functionality in Webrecorder is also part of :mod:`pywb`. If you want to create a WARC locally, this can be
+Recording functionality is also part of :mod:`pywb`. If you want to create a WARC locally, this can be
 done by directly recording into your pywb collection:
 
 1. Create a collection: ``wb-manager init my-web-archive`` (if you haven't already created a web archive collection)
 2. Run: ``wayback --record --live -a --auto-interval 10``
 3. Point your browser to ``http://localhost:8080/my-web-archive/record/<url>``
 
 For example, to record ``http://example.com/``, visit ``http://localhost:8080/my-web-archive/record/http://example.com/``
 
 In this configuration, the indexing happens every 10 seconds.. After 10 seconds, the recorded url will be accessible for replay, eg:
 ``http://localhost:8080/my-web-archive/http://example.com/``
 
 
+Using Browsertrix
+^^^^^^^^^^^^^^^^^
+
+For a more automated browser-based web archiving experience, `Browsertrix <https://browsertrix.com/>`_ provides a web interface for configuring, scheduling, running, reviewing, and curating crawls of web content. Crawl activity is shown in a live screencast of the browsers used for crawling and all web archives created in Browsertrix can be easily downloaded from the application in the WACZ format.
+
+`Browsertrix Crawler <https://crawler.docs.browsertrix.com/>`_, which provides the underlying crawling functionality of Browsertrix, can also be run standalone in a Docker container on your local computer.
+
+
 HTTP/S Proxy Mode Access
 ------------------------
 
 It is also possible to access any pywb collection via HTTP/S proxy mode, providing possibly better replay
 without client-side url rewriting.
 
 At this time, a single collection for proxy mode access can be specified with the ``--proxy`` flag.
```

### Comparing `pywb-2.7.4/docs/manual/vue-ui.rst` & `pywb-2.8.0/docs/manual/vue-ui.rst`

 * *Files 8% similar despite different names*

```diff
@@ -64,14 +64,29 @@
 
 .. code:: yaml
 
   ui:
     logo_home_url: https://example.com/web-archive-landing-page
 
 
+Printing
+^^^^^^^^
+
+As of pywb 2.8, the replay header includes a print button that prints the contents of the replay iframe.
+
+This button can be disabled by setting ``ui.disable_printing`` in ``config.yaml`` to any value.
+
+For example:
+
+.. code:: yaml
+
+  ui:
+    disable_printing: true
+
+
 Banner Colors
 ^^^^^^^^^^^^^
 
 It is possible to configure the background color, text color, and button outlines of the header by setting values in the ``ui`` section of ``config.yaml``.
 
 To customize the header background color, set ``ui.navbar_background_hex`` to the color's hex value, with the initial hash symbol (``#``) omitted. If omitted, ``#f8f9fa`` (Bootstrap 4's ``light``) will be used by default.
```

### Comparing `pywb-2.7.4/docs/manual/warcserver.rst` & `pywb-2.8.0/docs/manual/warcserver.rst`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/apps/cli.py` & `pywb-2.8.0/pywb/apps/cli.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/apps/frontendapp.py` & `pywb-2.8.0/pywb/apps/frontendapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from gevent.monkey import patch_all; patch_all()
 
 from werkzeug.routing import Map, Rule, RequestRedirect, Submount
-from werkzeug.wsgi import pop_path_info
+from wsgiref.util import shift_path_info
 from six.moves.urllib.parse import urljoin, parse_qsl
 from six import iteritems
 from warcio.utils import to_native_str
 from warcio.timeutils import iso_date_to_timestamp, timestamp_to_iso_date
 from wsgiprox.wsgiprox import WSGIProxMiddleware
 
 from pywb.recorder.multifilewarcwriter import MultiFileWARCWriter
@@ -430,15 +430,19 @@
             cdx_url += environ.get('QUERY_STRING')
 
         if self.query_limit:
             cdx_url += '&' if '?' in cdx_url else '?'
             cdx_url += 'limit=' + str(self.query_limit)
 
         try:
-            res = requests.get(cdx_url, stream=True)
+            headers = {}
+            for key in environ.keys():
+                if key.startswith("HTTP_X_"):
+                    headers[key[5:].replace("_", "-")] = environ[key]
+            res = requests.get(cdx_url, stream=True, headers=headers)
 
             status_line = '{} {}'.format(res.status_code, res.reason)
             content_type = res.headers.get('Content-Type')
 
             return WbResponse.bin_stream(StreamIter(res.raw),
                                          content_type=content_type,
                                          status=status_line,
@@ -550,17 +554,17 @@
         :param str coll: The name of the collection the record is to be served from
         :param bool record: Should the content being served by recorded (save to a warc). Only valid in record mode
         """
         if not coll or not self.warcserver.root_dir:
             return
 
         if coll != '$root':
-            pop_path_info(environ)
+            shift_path_info(environ)
             if record:
-                pop_path_info(environ)
+                shift_path_info(environ)
 
         paths = [self.warcserver.root_dir]
 
         if coll != '$root':
             paths.append(coll)
 
         paths.append(self.templates_dir)
@@ -595,15 +599,15 @@
                 coll in self.warcserver.list_dynamic_routes())
 
     def raise_not_found(self, environ, err_type, url):
         """Utility function for raising a werkzeug.exceptions.NotFound execption with the supplied WSGI environment
         and message.
 
         :param dict environ: The WSGI environment dictionary for the request
-        :param str err_type: The identifier for type of error that occured
+        :param str err_type: The identifier for type of error that occurred
         :param str url: The url of the archived page that was requested
         """
         raise AppPageNotFound(err_type, url)
 
     def _check_refer_redirect(self, environ):
         """Returns a WbResponse for a HTTP 307 redirection if the HTTP referer header is the same as the HTTP host header
 
@@ -659,18 +663,22 @@
             endpoint, args = urls.match()
 
             self.rewriterapp.prepare_env(environ)
 
             # store original script_name (original prefix) before modifications are made
             environ['ORIG_SCRIPT_NAME'] = environ.get('SCRIPT_NAME')
 
-            lang = args.pop('lang', self.default_locale)
+            lang = args.pop('lang', '')
+            if lang:
+                shift_path_info(environ)
+
             if lang:
-                pop_path_info(environ)
                 environ['pywb_lang'] = lang
+            elif self.default_locale:
+                environ['pywb_lang'] = self.default_locale
 
             response = endpoint(environ, **args)
 
         except RequestRedirect as rr:
             # if werkzeug throws this, likely a missing slash redirect
             # also check referrer here to avoid another redirect later
             redir = self._check_refer_redirect(environ)
```

### Comparing `pywb-2.7.4/pywb/apps/rewriterapp.py` & `pywb-2.8.0/pywb/apps/rewriterapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         self.default_rw = DefaultRewriter(replay_mod=self.replay_mod,
                                           config=config)
 
         self.js_proxy_rw = RewriterWithJSProxy(replay_mod=self.replay_mod)
 
         if not jinja_env:
             jinja_env = JinjaEnv(globals={'static_path': 'static'},
-                                 extensions=['jinja2.ext.i18n', 'jinja2.ext.with_'])
+                                 extensions=['jinja2.ext.i18n'])
             jinja_env.jinja_env.install_null_translations()
 
         self.jinja_env = jinja_env
         self.loc_map = {}
 
         self.jinja_env.init_loc(self.config.get('locales_root_dir'),
                                 self.config.get('locales'),
@@ -244,16 +244,16 @@
 
         wb_url.url = mod_url
         inputreq.url = mod_url
 
         range_start = start
         range_end = end
 
-        # if start with 0 and no end, load from upstream
-        if start == 0 and not end:
+        # if start with 0, load from upstream, but add range after
+        if start == 0:
             del inputreq.env['HTTP_RANGE']
         else:
             skip_record = True
 
         return range_start, range_end, skip_record
 
     def _add_range(self, record, wb_url, range_start, range_end):
```

### Comparing `pywb-2.7.4/pywb/apps/static_handler.py` & `pywb-2.8.0/pywb/apps/static_handler.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/apps/test/test_rewriter.py` & `pywb-2.8.0/pywb/apps/test/test_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/apps/test/test_wbrequestresponse.py` & `pywb-2.8.0/pywb/apps/test/test_wbrequestresponse.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/apps/wbrequestresponse.py` & `pywb-2.8.0/pywb/apps/wbrequestresponse.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/default_config.yaml` & `pywb-2.8.0/pywb/default_config.yaml`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/indexer/archiveindexer.py` & `pywb-2.8.0/pywb/indexer/archiveindexer.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/indexer/cdxindexer.py` & `pywb-2.8.0/pywb/indexer/cdxindexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -380,15 +380,15 @@
 Output CDX JSON format per line, with url timestamp first,
 followed by a json dict for all other fields:
 url timestamp { ... }
 """
 
     output_help = """
 Output file or directory.
-- If directory, each input file is written to a seperate output file
+- If directory, each input file is written to a separate output file
   with a .cdx extension
 - If output is '-', output is written to stdout
 """
 
     input_help = """
 Input file or directory.
 - If directory, all archive files from that directory are read
```

### Comparing `pywb-2.7.4/pywb/indexer/test/test_indexing.py` & `pywb-2.8.0/pywb/indexer/test/test_indexing.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/manager/aclmanager.py` & `pywb-2.8.0/pywb/manager/aclmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,19 +98,19 @@
                     if line:
                         self.rules.append(CDXObject(line))
 
             return True
 
         except IOError as io:
             if must_exist:
-                print('Error Occured: ' + str(io))
+                print('Error Occurred: ' + str(io))
             return False
 
         except Exception as e:
-            print('Error Occured: ' + str(e))
+            print('Error Occurred: ' + str(e))
             return False
 
     def save_acl(self, r=None):
         """Save the contents of the rules as cdxj entries to
         the access control list file
 
         :param argparse.Namespace|None r: Not used
```

### Comparing `pywb-2.7.4/pywb/manager/autoindex.py` & `pywb-2.8.0/pywb/manager/autoindex.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/manager/locmanager.py` & `pywb-2.8.0/pywb/manager/locmanager.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/manager/manager.py` & `pywb-2.8.0/pywb/manager/manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import os
 import shutil
 import sys
 import logging
 import heapq
 import yaml
 import re
+import gzip
 import six
+import pathlib
 
 from distutils.util import strtobool
 from pkg_resources import resource_string, get_distribution
 
 from argparse import ArgumentParser, RawTextHelpFormatter
+from tempfile import mkdtemp, TemporaryDirectory
+from zipfile import ZipFile
 
 from pywb.utils.loaders import load_yaml_config
 from warcio.timeutils import timestamp20_now
 
 from pywb import DEFAULT_CONFIG
 
 from six.moves import input
@@ -43,14 +47,17 @@
     """
     DEF_INDEX_FILE = 'index.cdxj'
 
     COLL_RX = re.compile('^[\w][-\w]*$')
 
     COLLS_DIR = 'collections'
 
+    WARC_RX = re.compile(r'.*\.w?arc(\.gz)?$')
+    WACZ_RX = re.compile(r'.*\.wacz$')
+
     def __init__(self, coll_name, colls_dir=None, must_exist=True):
         colls_dir = colls_dir or self.COLLS_DIR
         self.default_config = load_yaml_config(DEFAULT_CONFIG)
 
         if coll_name and not self.COLL_RX.match(coll_name):
             raise ValueError('Invalid Collection Name: ' + coll_name)
 
@@ -111,37 +118,150 @@
 
     def _assert_coll_exists(self):
         if not os.path.isdir(self.curr_coll_dir):
             msg = ('Collection {0} does not exist. ' +
                    'To create a new collection, run\n\n{1} init {0}')
             raise IOError(msg.format(self.coll_name, sys.argv[0]))
 
-    def add_warcs(self, warcs):
+    def add_archives(self, archives, unpack_wacz=False):
         if not os.path.isdir(self.archive_dir):
             raise IOError('Directory {0} does not exist'.
                           format(self.archive_dir))
 
+        invalid_archives = []
+        warc_paths = []
+        for archive in archives:
+            if self.WARC_RX.match(archive):
+                full_path = self._add_warc(archive)
+                if full_path:
+                    warc_paths.append(full_path)
+            elif self.WACZ_RX.match(archive):
+                if unpack_wacz:
+                    self._add_wacz_unpacked(archive)
+                else:
+                    raise NotImplementedError('Adding waczs without unpacking is not yet implemented. Use '
+                                              '\'--unpack-wacz\' flag to add the wacz\'s content.')
+            else:
+                invalid_archives.append(archive)
+
+        self._index_merge_warcs(warc_paths, self.DEF_INDEX_FILE)
+
+        if invalid_archives:
+            logging.warning(f'Invalid archives weren\'t added: {", ".join(invalid_archives)}')
+
+    def _rename_warc(self, warc_basename):
+        dupe_idx = 1
+        ext = ''.join(pathlib.Path(warc_basename).suffixes)
+        pre_ext_name = warc_basename.split(ext)[0]
+
+        while True:
+            new_basename = f'{pre_ext_name}-{dupe_idx}{ext}'
+            if not os.path.exists(os.path.join(self.archive_dir, new_basename)):
+                break
+            dupe_idx += 1
+
+        return new_basename
+
+    def _add_warc(self, warc):
+        warc_source = os.path.abspath(warc)
+        source_dir, warc_basename = os.path.split(warc_source)
+
+        # don't overwrite existing warcs with duplicate names
+        if os.path.exists(os.path.join(self.archive_dir, warc_basename)):
+            warc_basename = self._rename_warc(warc_basename)
+            logging.info(f'Warc {os.path.basename(warc)} already exists - renamed to {warc_basename}.')
+
+        warc_dest = os.path.join(self.archive_dir, warc_basename)
+        shutil.copy2(warc_source, warc_dest)
+        logging.info(f'Copied {warc} to {self.archive_dir} as {warc_basename}')
+        return warc_dest
+
+    def _add_wacz_unpacked(self, wacz):
+        wacz = os.path.abspath(wacz)
+        temp_dir = mkdtemp()
+        warc_regex = re.compile(r'.+\.warc(\.gz)?$')
+        cdx_regex = re.compile(r'.+\.cdx(\.gz)?$')
+        with ZipFile(wacz, 'r') as wacz_zip_file:
+            archive_members = wacz_zip_file.namelist()
+            warc_files = [file for file in archive_members if warc_regex.match(file)]
+            if not warc_files:
+                logging.warning(f'WACZ {wacz} does not contain any warc files.')
+                return
+
+            # extract warc files
+            for warc_file in warc_files:
+                wacz_zip_file.extract(warc_file, temp_dir)
+
+            cdx_files = [file for file in archive_members if cdx_regex.match(file)]
+            if not cdx_files:
+                logging.warning(f'WACZ {wacz} does not contain any indices.')
+                return
+
+            for cdx_file in cdx_files:
+                wacz_zip_file.extract(cdx_file, temp_dir)
+
+        # copy extracted warc files to collections archive dir, use wacz filename as filename with added index if
+        # multiple warc files exist
+        warc_filename_mapping = {}
         full_paths = []
-        duplicate_warcs = []
-        for filename in warcs:
-            filename = os.path.abspath(filename)
-
-            # don't overwrite existing warcs with duplicate names
-            if os.path.exists(os.path.join(self.archive_dir, os.path.basename(filename))):
-                duplicate_warcs.append(filename)
-                continue
-
-            shutil.copy2(filename, self.archive_dir)
-            full_paths.append(os.path.join(self.archive_dir, filename))
-            logging.info('Copied ' + filename + ' to ' + self.archive_dir)
+        for idx, extracted_warc_file in enumerate(warc_files):
+            _, warc_ext = os.path.splitext(extracted_warc_file)
+            if warc_ext == '.gz':
+                warc_ext = '.warc.gz'
+            warc_filename = os.path.basename(wacz)
+            warc_filename, _ = os.path.splitext(warc_filename)
+            warc_filename = f'{warc_filename}-{idx}{warc_ext}'
+            warc_destination_path = os.path.join(self.archive_dir, warc_filename)
+
+            if os.path.exists(warc_destination_path):
+                warc_filename = self._rename_warc(warc_filename)
+                logging.info(f'Warc {warc_destination_path} already exists - renamed to {warc_filename}.')
+                warc_destination_path = os.path.join(self.archive_dir, warc_filename)
+
+            warc_filename_mapping[os.path.basename(extracted_warc_file)] = warc_filename
+            shutil.copy2(os.path.join(temp_dir, extracted_warc_file), warc_destination_path)
+            full_paths.append(warc_destination_path)
+
+        # rewrite filenames in wacz indices and merge them with collection index file
+        for cdx_file in cdx_files:
+            self._add_wacz_index(os.path.join(self.indexes_dir, self.DEF_INDEX_FILE), os.path.join(temp_dir, cdx_file),
+                                 warc_filename_mapping)
+
+        # delete temporary files
+        shutil.rmtree(temp_dir)
+
+    def _add_wacz_index(self, collection_index_path, wacz_index_path, filename_mapping):
+        from pywb.warcserver.index.cdxobject import CDXObject
+
+        # rewrite wacz index to temporary index file
+        tempdir = TemporaryDirectory()
+        wacz_index_name = os.path.basename(wacz_index_path)
+        rewritten_index_path = os.path.join(tempdir.name, wacz_index_name)
+
+        with open(rewritten_index_path, 'w') as rewritten_index:
+            if wacz_index_path.endswith('.gz'):
+                wacz_index = gzip.open(wacz_index_path, 'rb')
+            else:
+                wacz_index = open(wacz_index_path, 'rb')
 
-        self._index_merge_warcs(full_paths, self.DEF_INDEX_FILE)
+            for line in wacz_index:
+                cdx_object = CDXObject(cdxline=line)
+                if cdx_object['filename'] in filename_mapping:
+                    cdx_object['filename'] = filename_mapping[cdx_object['filename']]
+                rewritten_index.write(cdx_object.to_cdxj())
 
-        if duplicate_warcs:
-            logging.warning(f'Warcs {", ".join(duplicate_warcs)} weren\'t added because of duplicate names.')
+        if not os.path.isfile(collection_index_path):
+            shutil.move(rewritten_index_path, collection_index_path)
+            return
+
+        temp_coll_index_path = collection_index_path + '.tmp.' + timestamp20_now()
+        self._merge_indices(collection_index_path, rewritten_index_path, temp_coll_index_path)
+        shutil.move(temp_coll_index_path, collection_index_path)
+
+        tempdir.cleanup()
 
     def reindex(self):
         cdx_file = os.path.join(self.indexes_dir, self.DEF_INDEX_FILE)
         logging.info('Indexing ' + self.archive_dir + ' to ' + cdx_file)
         self._cdx_index(cdx_file, [self.archive_dir])
 
     def _cdx_index(self, out, input_, rel_root=None):
@@ -186,28 +306,32 @@
         # no existing file, so just make it the new file
         if not os.path.isfile(cdx_file):
             shutil.move(temp_file, cdx_file)
             return
 
         merged_file = temp_file + '.merged'
 
-        last_line = None
-
-        with open(cdx_file, 'rb') as orig_index:
-            with open(temp_file, 'rb') as new_index:
-                with open(merged_file, 'w+b') as merged:
-                    for line in heapq.merge(orig_index, new_index):
-                        if last_line != line:
-                            merged.write(line)
-                            last_line = line
+        self._merge_indices(cdx_file, temp_file, merged_file)
 
         shutil.move(merged_file, cdx_file)
         #os.rename(merged_file, cdx_file)
         os.remove(temp_file)
 
+    @staticmethod
+    def _merge_indices(index1, index2, dest):
+        last_line = None
+
+        with open(index1, 'rb') as index1_f:
+            with open(index2, 'rb') as index2_f:
+                with open(dest, 'wb') as dest_f:
+                    for line in heapq.merge(index1_f, index2_f):
+                        if last_line != line:
+                            dest_f.write(line)
+                            last_line = line
+
     def set_metadata(self, namevalue_pairs):
         metadata_yaml = os.path.join(self.curr_coll_dir, 'metadata.yaml')
         metadata = None
         if os.path.isfile(metadata_yaml):
             with open(metadata_yaml, 'rb') as fh:
                 metadata = yaml.safe_load(fh)
 
@@ -379,24 +503,31 @@
         m = CollectionsManager('', must_exist=False)
         m.list_colls()
 
     list_help = 'List Collections'
     listcmd = subparsers.add_parser('list', help=list_help)
     listcmd.set_defaults(func=do_list)
 
-    # Add Warcs
+    # Add Warcs or Waczs
     def do_add(r):
         m = CollectionsManager(r.coll_name)
-        m.add_warcs(r.files)
+        m.add_archives(r.files, r.unpack_wacz)
 
-    addwarc_help = 'Copy ARCS/WARCS to collection directory and reindex'
-    addwarc = subparsers.add_parser('add', help=addwarc_help)
-    addwarc.add_argument('coll_name')
-    addwarc.add_argument('files', nargs='+')
-    addwarc.set_defaults(func=do_add)
+    add_archives_help = 'Copy ARCs/WARCs to collection directory and reindex'
+    add_unpack_wacz_help = 'Copy WARCs from WACZ to collection directory and reindex'
+    add_archives = subparsers.add_parser('add', help=add_archives_help)
+    add_archives.add_argument(
+        '--unpack-wacz',
+        dest='unpack_wacz',
+        action='store_true',
+        help=add_unpack_wacz_help
+    )
+    add_archives.add_argument('coll_name')
+    add_archives.add_argument('files', nargs='+')
+    add_archives.set_defaults(func=do_add)
 
     # Reindex All
     def do_reindex(r):
         m = CollectionsManager(r.coll_name)
         m.reindex()
 
     reindex_help = 'Re-Index entire collection'
```

### Comparing `pywb-2.7.4/pywb/manager/migrate.py` & `pywb-2.8.0/pywb/manager/migrate.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/recorder/filters.py` & `pywb-2.8.0/pywb/recorder/filters.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/recorder/multifilewarcwriter.py` & `pywb-2.8.0/pywb/recorder/multifilewarcwriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/recorder/recorderapp.py` & `pywb-2.8.0/pywb/recorder/recorderapp.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/recorder/redisindexer.py` & `pywb-2.8.0/pywb/recorder/redisindexer.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/recorder/test/simplerec.py` & `pywb-2.8.0/pywb/recorder/test/simplerec.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/recorder/test/test_recorder.py` & `pywb-2.8.0/pywb/recorder/test/test_recorder.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/rewrite/content_rewriter.py` & `pywb-2.8.0/pywb/rewrite/content_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/rewrite/cookie_rewriter.py` & `pywb-2.8.0/pywb/rewrite/cookie_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/rewrite/cookies.py` & `pywb-2.8.0/pywb/rewrite/cookies.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/rewrite/default_rewriter.py` & `pywb-2.8.0/pywb/rewrite/default_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/rewrite/header_rewriter.py` & `pywb-2.8.0/pywb/rewrite/header_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/rewrite/html_insert_rewriter.py` & `pywb-2.8.0/pywb/rewrite/html_insert_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/rewrite/html_rewriter.py` & `pywb-2.8.0/pywb/rewrite/html_rewriter.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,15 +264,15 @@
                 value = value.encode('iso-8859-1').decode(self.charset)
             except:
                 pass
 
         unesc_value = self.try_unescape(value)
         rewritten_value = self.url_rewriter.rewrite(unesc_value, mod, force_abs)
 
-        # if no rewriting has occured, ensure we return original, not reencoded value
+        # if no rewriting has occurred, ensure we return original, not reencoded value
         if rewritten_value == value:
             return orig_value
 
         if unesc_value != value and rewritten_value != unesc_value:
             rewritten_value = rewritten_value.replace(unesc_value, value)
 
         return rewritten_value
@@ -664,15 +664,15 @@
     #    self.out.write('&#' + data + ';')
 
     def handle_comment(self, data):
         self.out.write('<!--')
         if self.parse_comments:
             #data = self._rewrite_script(data)
 
-            # Rewrite with seperate HTMLRewriter
+            # Rewrite with separate HTMLRewriter
             comment_rewriter = HTMLRewriter(self.url_rewriter,
                                             defmod=self.defmod)
 
             data = comment_rewriter.rewrite_complete(data)
             self.out.write(data)
         else:
             self.parse_data(data)
```

### Comparing `pywb-2.7.4/pywb/rewrite/jsonp_rewriter.py` & `pywb-2.8.0/pywb/rewrite/jsonp_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/rewrite/regex_rewriters.py` & `pywb-2.8.0/pywb/rewrite/regex_rewriters.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,17 +120,15 @@
             (r'(?<!function)(?:\s|^)\beval\s*\(', self.replace_prefix_from(eval_str, 'eval'), 0),
             # rewriting 'x = eval' - no invocation
             (r'(?<=[=,])\s*\beval\b\s*(?![(:.$])', self.replace_str('self.eval', 'eval'), 0),
             (r'(?<=\.)postMessage\b\(', self.add_prefix('__WB_pmw(self).'), 0),
             (r'(?<![$.])\s*\blocation\b\s*[=]\s*(?![=])', self.add_suffix(check_loc), 0),
             # rewriting 'return this'
             (r'\breturn\s+this\b\s*(?![.$])', self.replace_str(this_rw), 0),
-            # rewriting 'this.' special properties access on new line, with ; prepended
-            (r'\n\s*this\b(?=(?:\.(?:{0})\b))'.format(prop_str), self.replace_str(';' + this_rw), 0),
-            # rewriting 'this.' special properties access, not on new line (no ;)
+            # rewriting 'this.' special properties access
             (r'(?<![$.])\s*this\b(?=(?:\.(?:{0})\b))'.format(prop_str), self.replace_str(this_rw), 0),
             # rewrite '= this' or ', this'
             (r'(?<=[=,])\s*this\b\s*(?![:.$])', self.replace_str(this_rw), 0),
             # rewrite ')(this)'
             ('\}(?:\s*\))?\s*\(this\)', self.replace_str(this_rw), 0),
             # rewrite this in && or || expr?
             (r'(?<=[^|&][|&]{2})\s*this\b\s*(?![|&.$]([^|&]|$))', self.replace_str(this_rw), 0),
```

### Comparing `pywb-2.7.4/pywb/rewrite/rewrite_amf.py` & `pywb-2.8.0/pywb/rewrite/rewrite_amf.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/rewrite/rewrite_dash.py` & `pywb-2.8.0/pywb/rewrite/rewrite_dash.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/rewrite/rewrite_hls.py` & `pywb-2.8.0/pywb/rewrite/rewrite_hls.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/rewrite/rewrite_js_workers.py` & `pywb-2.8.0/pywb/rewrite/rewrite_js_workers.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/rewrite/rewriteinputreq.py` & `pywb-2.8.0/pywb/rewrite/rewriteinputreq.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/rewrite/templateview.py` & `pywb-2.8.0/pywb/rewrite/templateview.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from warcio.timeutils import timestamp_to_datetime, timestamp_to_sec
 from warcio.timeutils import timestamp_now
 
 from pywb.utils.loaders import load
 
 from six.moves.urllib.parse import urlsplit, quote
 
-from jinja2 import Environment, TemplateNotFound, contextfunction, select_autoescape
+from jinja2 import Environment, TemplateNotFound, pass_context, select_autoescape
 from jinja2 import FileSystemLoader, PackageLoader, ChoiceLoader
 
 from webassets.ext.jinja2 import AssetsExtension
 from webassets.loaders import YAMLLoader
 from webassets.env import Resolver
 
 from pkg_resources import resource_filename
@@ -135,15 +135,15 @@
                 logging.warn("Ignoring Locales. You must install i18n extensions with 'pip install pywb[i18n]' to use localization features")
 
         def get_translate(context):
             loc = context.get('env', {}).get('pywb_lang', default_locale)
             return loc_map.get(loc)
 
         def override_func(jinja_env, name):
-            @contextfunction
+            @pass_context
             def get_override(context, text):
                 translate = get_translate(context)
                 if not translate:
                     return text
 
                 func = getattr(translate, name)
                 return func(text)
@@ -154,57 +154,57 @@
         override_func(self.jinja_env, 'gettext')
 
         # single/plural form translation function
         override_func(self.jinja_env, 'ngettext')
 
         # Special _Q() function to return %-encoded text, necessary for use
         # with text in banner
-        @contextfunction
+        @pass_context
         def quote_gettext(context, text):
             translate = get_translate(context)
             if not translate:
                 return text
 
             text = translate.gettext(text)
             return quote(text, safe='/: ')
 
         self.jinja_env.globals['locales'] = list(loc_map.keys())
         self.jinja_env.globals['_Q'] = quote_gettext
         self.jinja_env.globals['default_locale'] = default_locale
 
-        @contextfunction
+        @pass_context
         def switch_locale(context, locale):
             environ = context.get('env')
             curr_loc = environ.get('pywb_lang', '')
 
             request_uri = environ.get('REQUEST_URI', environ.get('PATH_INFO'))
 
-            if curr_loc:
+            if curr_loc and request_uri.startswith('/' + curr_loc + '/'):
                 return request_uri.replace(curr_loc, locale, 1)
 
             app_prefix = environ.get('pywb.app_prefix', '')
 
             if app_prefix and request_uri.startswith(app_prefix):
                 request_uri = request_uri.replace(app_prefix, '')
 
             return app_prefix + '/' + locale + request_uri
 
-        @contextfunction
+        @pass_context
         def get_locale_prefixes(context):
             environ = context.get('env')
             locale_prefixes = {}
 
             orig_prefix = environ.get('pywb.app_prefix', '')
             coll = environ.get('SCRIPT_NAME', '')
 
-            if orig_prefix:
+            if orig_prefix and coll.startswith(orig_prefix):
                 coll = coll[len(orig_prefix):]
 
             curr_loc = environ.get('pywb_lang', '')
-            if curr_loc:
+            if curr_loc and coll.startswith('/' + curr_loc):
                 coll = coll[len(curr_loc) + 1:]
 
             for locale in loc_map.keys():
                 locale_prefixes[locale] = orig_prefix + '/' + locale + coll + '/'
 
             return locale_prefixes
```

### Comparing `pywb-2.7.4/pywb/rewrite/test/test_content_rewriter.py` & `pywb-2.8.0/pywb/rewrite/test/test_content_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/rewrite/test/test_cookie_rewriter.py` & `pywb-2.8.0/pywb/rewrite/test/test_cookie_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/rewrite/test/test_header_rewriter.py` & `pywb-2.8.0/pywb/rewrite/test/test_header_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/rewrite/test/test_html_insert_rewriter.py` & `pywb-2.8.0/pywb/rewrite/test/test_html_insert_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/rewrite/test/test_html_rewriter.py` & `pywb-2.8.0/pywb/rewrite/test/test_html_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/rewrite/test/test_jsonp_rewriter.py` & `pywb-2.8.0/pywb/rewrite/test/test_jsonp_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/rewrite/test/test_regex_rewriters.py` & `pywb-2.8.0/pywb/rewrite/test/test_regex_rewriters.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 >>> _test_js_obj_proxy('location = "xyz"')
 'location = ((self.__WB_check_loc && self.__WB_check_loc(location, arguments)) || {}).href = "xyz"'
 
 >>> _test_js_obj_proxy('var foo = this.location')
 'var foo = _____WB$wombat$check$this$function_____(this).location'
 
 >>> _test_js_obj_proxy('A = B\nthis.location = "foo"')
-'A = B\n;_____WB$wombat$check$this$function_____(this).location = "foo"'
+'A = B\n_____WB$wombat$check$this$function_____(this).location = "foo"'
 
 >>> _test_js_obj_proxy('var foo = this.location2')
 'var foo = this.location2'
 
 >>> _test_js_obj_proxy('func(Function("return this"));')
 'func(Function("return _____WB$wombat$check$this$function_____(this)"));'
```

### Comparing `pywb-2.7.4/pywb/rewrite/test/test_url_rewriter.py` & `pywb-2.8.0/pywb/rewrite/test/test_url_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/rewrite/test/test_wburl.py` & `pywb-2.8.0/pywb/rewrite/test/test_wburl.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/rewrite/url_rewriter.py` & `pywb-2.8.0/pywb/rewrite/url_rewriter.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/rewrite/wburl.py` & `pywb-2.8.0/pywb/rewrite/wburl.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/rules.yaml` & `pywb-2.8.0/pywb/rules.yaml`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/autoFetchWorker.js` & `pywb-2.8.0/pywb/static/autoFetchWorker.js`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/css/base.css` & `pywb-2.8.0/pywb/static/css/base.css`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/css/bootstrap.min.css` & `pywb-2.8.0/pywb/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/css/font-awesome.min.css` & `pywb-2.8.0/pywb/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/flowplayer/flowplayer-3.2.18.swf` & `pywb-2.8.0/pywb/static/flowplayer/flowplayer-3.2.18.swf`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/flowplayer/flowplayer.audio-3.2.11.swf` & `pywb-2.8.0/pywb/static/flowplayer/flowplayer.audio-3.2.11.swf`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/flowplayer/flowplayer.controls-3.2.16.swf` & `pywb-2.8.0/pywb/static/flowplayer/flowplayer.controls-3.2.16.swf`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/flowplayer/flowplayer.pseudostreaming-3.2.13.swf` & `pywb-2.8.0/pywb/static/flowplayer/flowplayer.pseudostreaming-3.2.13.swf`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/flowplayer/toolbox.flashembed.js` & `pywb-2.8.0/pywb/static/flowplayer/toolbox.flashembed.js`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-brands-400.eot` & `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-brands-400.svg` & `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-brands-400.ttf` & `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-brands-400.woff` & `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-brands-400.woff2` & `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-regular-400.eot` & `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-regular-400.svg` & `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-regular-400.ttf` & `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-regular-400.woff` & `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-regular-400.woff2` & `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-solid-900.eot` & `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-solid-900.svg` & `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-solid-900.ttf` & `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-solid-900.woff` & `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/fonts/font-awesome/fa-solid-900.woff2` & `pywb-2.8.0/pywb/static/fonts/font-awesome/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/fonts/glyphicons-halflings-regular.eot` & `pywb-2.8.0/pywb/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/fonts/glyphicons-halflings-regular.svg` & `pywb-2.8.0/pywb/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/fonts/glyphicons-halflings-regular.ttf` & `pywb-2.8.0/pywb/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/fonts/glyphicons-halflings-regular.woff` & `pywb-2.8.0/pywb/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/fonts/glyphicons-halflings-regular.woff2` & `pywb-2.8.0/pywb/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/js/bootstrap.min.js` & `pywb-2.8.0/pywb/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/js/jquery-latest.min.js` & `pywb-2.8.0/pywb/static/js/jquery-latest.min.js`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/js/url-polyfill.min.js` & `pywb-2.8.0/pywb/static/js/url-polyfill.min.js`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/loading-spinner/loading-spinner.js` & `pywb-2.8.0/pywb/static/loading-spinner/loading-spinner.js`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/pywb-logo-sm.png` & `pywb-2.8.0/pywb/static/pywb-logo-sm.png`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/pywb-logo.png` & `pywb-2.8.0/pywb/static/pywb-logo.png`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/query.js` & `pywb-2.8.0/pywb/static/query.js`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/queryWorker.js` & `pywb-2.8.0/pywb/static/queryWorker.js`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/scroll-webkit.css` & `pywb-2.8.0/pywb/static/scroll-webkit.css`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/search.js` & `pywb-2.8.0/pywb/static/search.js`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/transclusions.js` & `pywb-2.8.0/pywb/static/transclusions.js`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/vidrw.js` & `pywb-2.8.0/pywb/static/vidrw.js`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/vue/vueui.js` & `pywb-2.8.0/pywb/static/vue/vueui.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -46,15 +46,15 @@
             }; // make a copy of config
         }
 
         // can get long (default) or short month string
         getMonth(id, type = 'long') {
             return decodeURIComponent(this.config[PywbI18N.monthIdPrefix[id] + '_' + type]);
         }
-        // can get long (default) or short day string or intial
+        // can get long (default) or short day string or initial
         // PywbI18N expects to receive day's initials like:
         // config.mon_short, config.tue_long, ...., config.<mmm>_short, config.<mmm>_long
         getWeekDay(id, type = 'long') {
             return decodeURIComponent(this.config[id + '_' + type])
         }
         getWeekDays(type = 'long') {
             let weekDays = ['sun', 'mon', 'tue', 'wed', 'thu', 'fri', 'sat'];
@@ -1123,15 +1123,15 @@
                                                 },
                                                 style: {
                                                     height: _vm.getHistoLineHeight(
                                                         histoPeriod.snapshotCount
                                                     )
                                                 },
                                                 attrs: {
-                                                    tabindex: "0"
+                                                    tabindex: histoPeriod.snapshotCount > 0 ? 0 : -1
                                                 },
                                                 on: {
                                                     click: function($event) {
                                                         return _vm.changePeriod(histoPeriod, $event)
                                                     },
                                                     keyup: function($event) {
                                                         if (
@@ -1162,17 +1162,14 @@
                                     _vm._v(" "),
                                     _c(
                                         "div", {
                                             staticClass: "inner",
                                             class: {
                                                 "has-single-snapshot": subPeriod.snapshotCount === 1
                                             },
-                                            attrs: {
-                                                tabindex: "0"
-                                            },
                                             on: {
                                                 click: function($event) {
                                                     return _vm.changePeriod(subPeriod, $event)
                                                 },
                                                 keyup: function($event) {
                                                     if (
                                                         !$event.type.indexOf("key") &&
@@ -1248,23 +1245,23 @@
     };
     var __vue_staticRenderFns__$6 = [];
     __vue_render__$6._withStripped = true;
 
     /* style */
     const __vue_inject_styles__$6 = function(inject) {
         if (!inject) return
-        inject("data-v-7627cc2c_0", {
+        inject("data-v-176cc9e0_0", {
             source: "\n.timeline {\n    position: relative;\n    display: flex;\n    width: auto;\n    height: 60px;\n    margin: 5px;\n    justify-content: left;\n}\n.timeline .id {\n    display: inline-block;\n    font-size: 30px;\n}\n.timeline .arrow {\n    display: inline-block;\n    width: 20px;\n    font-size: 20px; /* font-size = width of arrow, as it UTF char */\n    line-height: 60px;\n    vertical-align: top;\n    cursor: pointer;\n}\n.timeline .arrow.previous {\n}\n.timeline .arrow.next {\n}\n.timeline .arrow.disabled, .timeline .arrow.disabled:hover {\n    /*color: lightgray;*/\n    background-color: transparent;\n    /*cursor: not-allowed;*/\n    visibility: hidden;\n}\n.timeline .arrow:hover {\n    background-color: antiquewhite;\n    color: firebrick;\n}\n.timeline .scroll {\n    position: relative;\n    display: inline-block;\n    width: 100%; /* */\n    height: 100%;\n\n    /* maker scrollable horizontally */\n    overflow-x: scroll;\n    overflow-y: hidden;\n    white-space: nowrap;\n    scroll-behavior: smooth;\n\n    text-align: center;\n\n    transition: background-color 500ms ease-in;\n}\n/* hide scroll bar */\n.timeline .scroll::-webkit-scrollbar {\n    display: none;\n}\n/* highlight the scroll period: usually triggered from root app */\n.timeline .scroll.highlight {\n    background-color: #fff7ce;\n}\n.timeline .scroll .periods {\n    display: flex;\n    justify-content: space-between;\n    height: 100%;\n    width: 100%;\n    min-width: 600px;\n}\n.timeline .period {\n    flex-grow: 1;\n    position: relative;\n    display: inline-block;\n    height: 100%;\n    /* line-height: 80px; /* use to center middle vertically */\n    white-space: normal;\n    vertical-align: top;\n    text-align: center;\n    background-color: transparent;\n\n    transition: background-color 500ms ease-in-out;\n}\n/* 1st period period child el */\n.timeline .period:nth-child(1) {\n    /*border-left: 1px solid white; !* has left border; all other periods have right border *!*/\n}\n.timeline .period:hover {\n    background-color: #eeeeee;\n}\n.timeline .period.contains-current-snapshot, .timeline .period.contains-current-snapshot:hover {\n    background-color: #f7def4;\n}\n\n/* empty period */\n.timeline .period.empty {\n    color: #aaa;\n    /*background-color: transparent;*/\n}\n/* highlighted period */\n.timeline .period.highlight {\n    background-color: cyan;\n}\n.timeline .period .inner {\n    display: block;\n    position: absolute;\n    bottom: 0;\n    left: 0;\n    width: 100%;\n    height: 20px;\n    background-color: white;\n    border-top: 1px solid gray;\n    white-space: nowrap;\n    cursor: zoom-in;\n}\n.timeline .period .inner.has-single-snapshot {\n  cursor: pointer;\n}\n.timeline .period.last-level .inner, .timeline .period.empty .inner {\n  cursor: default;\n}\n.timeline .period .label {\n  width: 100%;\n  font-weight: bold;\n  font-size: 14px;\n  transition: background-color 500ms ease-in;\n}\n.timeline .period:hover .label {\n  position: absolute;\n  z-index: 20;\n  background-color: lightgrey;\n}\n.timeline .period .histo {\n    display: flex;\n    position: absolute;\n    top: 1px;\n    left: 0;\n    width: 100%;\n    height: 39px;\n    align-items: flex-end;\n    justify-content: space-between;\n    text-align: left;\n}\n.timeline .period .histo .line {\n    position: relative;\n    flex-grow: 1;\n    display: inline-block;\n    background-color: #a6cdf5;\n    margin: 0;\n    padding: 0;\n    cursor: zoom-in;\n}\n.timeline .period .histo .line.has-single-snapshot {\n  cursor: pointer;\n}\n\n/* Last level period histogram spaces things evenly */\n.timeline .period.last-level .histo {\n    justify-content: space-around;\n}\n\n/* Last level period histogram lines do not grow, but are fixed width/margin */\n.timeline .period.last-level .histo .line {\n    flex-grow: unset;\n    width: 5px;\n    margin-left: 2px;\n}\n\n    /* update line color on hover*/\n.timeline .period .histo .line:hover {\n        background-color: #f5a6eb;\n}\n.timeline .period .histo .line.contains-current-snapshot {\n        background-color: red;\n}\n\n    /* Period that contains ONE snapshot only will show snapshot info*/\n.timeline .period-tooltip {\n        position: fixed;\n        z-index: 100;\n        /*left or right set programmatically*/\n        display: block;\n        background-color: white;\n        border: 1px solid gray;\n        padding: 2px;\n        white-space: nowrap; /*no wrapping allowed*/\n}\n        /*show on hover*/\n.timeline .period-tooltip.show {\n            display: block;\n}\n\n",
             map: {
                 "version": 3,
                 "sources": ["/Users/tessa/dev/pywb/pywb/vueui/src/components/Timeline.vue"],
                 "names": [],
-                "mappings": ";AAyPA;IACA,kBAAA;IACA,aAAA;IACA,WAAA;IACA,YAAA;IACA,WAAA;IACA,qBAAA;AACA;AAEA;IACA,qBAAA;IACA,eAAA;AACA;AACA;IACA,qBAAA;IACA,WAAA;IACA,eAAA,EAAA,+CAAA;IACA,iBAAA;IACA,mBAAA;IACA,eAAA;AACA;AACA;AACA;AACA;AACA;AACA;IACA,oBAAA;IACA,6BAAA;IACA,uBAAA;IACA,kBAAA;AACA;AACA;IACA,8BAAA;IACA,gBAAA;AACA;AAEA;IACA,kBAAA;IACA,qBAAA;IACA,WAAA,EAAA,IAAA;IACA,YAAA;;IAEA,kCAAA;IACA,kBAAA;IACA,kBAAA;IACA,mBAAA;IACA,uBAAA;;IAEA,kBAAA;;IAEA,0CAAA;AACA;AACA,oBAAA;AACA;IACA,aAAA;AACA;AACA,iEAAA;AACA;IACA,yBAAA;AACA;AACA;IACA,aAAA;IACA,8BAAA;IACA,YAAA;IACA,WAAA;IACA,gBAAA;AACA;AAGA;IACA,YAAA;IACA,kBAAA;IACA,qBAAA;IACA,YAAA;IACA,0DAAA;IACA,mBAAA;IACA,mBAAA;IACA,kBAAA;IACA,6BAAA;;IAEA,8CAAA;AACA;AACA,+BAAA;AACA;IACA,2FAAA;AACA;AAEA;IACA,yBAAA;AACA;AACA;IACA,yBAAA;AACA;;AAEA,iBAAA;AACA;IACA,WAAA;IACA,iCAAA;AACA;AACA,uBAAA;AACA;IACA,sBAAA;AACA;AAEA;IACA,cAAA;IACA,kBAAA;IACA,SAAA;IACA,OAAA;IACA,WAAA;IACA,YAAA;IACA,uBAAA;IACA,0BAAA;IACA,mBAAA;IACA,eAAA;AACA;AACA;EACA,eAAA;AACA;AACA;EACA,eAAA;AACA;AAEA;EACA,WAAA;EACA,iBAAA;EACA,eAAA;EACA,0CAAA;AACA;AACA;EACA,kBAAA;EACA,WAAA;EACA,2BAAA;AACA;AAEA;IACA,aAAA;IACA,kBAAA;IACA,QAAA;IACA,OAAA;IACA,WAAA;IACA,YAAA;IACA,qBAAA;IACA,8BAAA;IACA,gBAAA;AACA;AAEA;IACA,kBAAA;IACA,YAAA;IACA,qBAAA;IACA,yBAAA;IACA,SAAA;IACA,UAAA;IACA,eAAA;AACA;AACA;EACA,eAAA;AACA;;AAEA,qDAAA;AACA;IACA,6BAAA;AACA;;AAEA,8EAAA;AACA;IACA,gBAAA;IACA,UAAA;IACA,gBAAA;AACA;;IAEA,8BAAA;AACA;QACA,yBAAA;AACA;AAEA;QACA,qBAAA;AACA;;IAEA,kEAAA;AACA;QACA,eAAA;QACA,YAAA;QACA,qCAAA;QACA,cAAA;QACA,uBAAA;QACA,sBAAA;QACA,YAAA;QACA,mBAAA,EAAA,sBAAA;AACA;QACA,gBAAA;AACA;YACA,cAAA;AACA",
+                "mappings": ";AAwPA;IACA,kBAAA;IACA,aAAA;IACA,WAAA;IACA,YAAA;IACA,WAAA;IACA,qBAAA;AACA;AAEA;IACA,qBAAA;IACA,eAAA;AACA;AACA;IACA,qBAAA;IACA,WAAA;IACA,eAAA,EAAA,+CAAA;IACA,iBAAA;IACA,mBAAA;IACA,eAAA;AACA;AACA;AACA;AACA;AACA;AACA;IACA,oBAAA;IACA,6BAAA;IACA,uBAAA;IACA,kBAAA;AACA;AACA;IACA,8BAAA;IACA,gBAAA;AACA;AAEA;IACA,kBAAA;IACA,qBAAA;IACA,WAAA,EAAA,IAAA;IACA,YAAA;;IAEA,kCAAA;IACA,kBAAA;IACA,kBAAA;IACA,mBAAA;IACA,uBAAA;;IAEA,kBAAA;;IAEA,0CAAA;AACA;AACA,oBAAA;AACA;IACA,aAAA;AACA;AACA,iEAAA;AACA;IACA,yBAAA;AACA;AACA;IACA,aAAA;IACA,8BAAA;IACA,YAAA;IACA,WAAA;IACA,gBAAA;AACA;AAGA;IACA,YAAA;IACA,kBAAA;IACA,qBAAA;IACA,YAAA;IACA,0DAAA;IACA,mBAAA;IACA,mBAAA;IACA,kBAAA;IACA,6BAAA;;IAEA,8CAAA;AACA;AACA,+BAAA;AACA;IACA,2FAAA;AACA;AAEA;IACA,yBAAA;AACA;AACA;IACA,yBAAA;AACA;;AAEA,iBAAA;AACA;IACA,WAAA;IACA,iCAAA;AACA;AACA,uBAAA;AACA;IACA,sBAAA;AACA;AAEA;IACA,cAAA;IACA,kBAAA;IACA,SAAA;IACA,OAAA;IACA,WAAA;IACA,YAAA;IACA,uBAAA;IACA,0BAAA;IACA,mBAAA;IACA,eAAA;AACA;AACA;EACA,eAAA;AACA;AACA;EACA,eAAA;AACA;AAEA;EACA,WAAA;EACA,iBAAA;EACA,eAAA;EACA,0CAAA;AACA;AACA;EACA,kBAAA;EACA,WAAA;EACA,2BAAA;AACA;AAEA;IACA,aAAA;IACA,kBAAA;IACA,QAAA;IACA,OAAA;IACA,WAAA;IACA,YAAA;IACA,qBAAA;IACA,8BAAA;IACA,gBAAA;AACA;AAEA;IACA,kBAAA;IACA,YAAA;IACA,qBAAA;IACA,yBAAA;IACA,SAAA;IACA,UAAA;IACA,eAAA;AACA;AACA;EACA,eAAA;AACA;;AAEA,qDAAA;AACA;IACA,6BAAA;AACA;;AAEA,8EAAA;AACA;IACA,gBAAA;IACA,UAAA;IACA,gBAAA;AACA;;IAEA,8BAAA;AACA;QACA,yBAAA;AACA;AAEA;QACA,qBAAA;AACA;;IAEA,kEAAA;AACA;QACA,eAAA;QACA,YAAA;QACA,qCAAA;QACA,cAAA;QACA,uBAAA;QACA,sBAAA;QACA,YAAA;QACA,mBAAA,EAAA,sBAAA;AACA;QACA,gBAAA;AACA;YACA,cAAA;AACA",
                 "file": "Timeline.vue",
-                "sourcesContent": ["<template>\n    <div class=\"timeline\">\n        <div class=\"period-tooltip\" v-show=\"tooltipPeriod\" :style=\"{left: tooltipPeriodPos.x+'px', top: tooltipPeriodPos.y+'px'}\">\n            <template v-if=\"tooltipPeriod\">\n              <div v-if=\"tooltipPeriod.snapshot\">\n                {{ $root._('View capture on {date}', {date: tooltipPeriod.snapshot.getTimeDateFormatted()}) }}\n              </div>\n              <div v-else-if=\"tooltipPeriod.snapshotPeriod\">\n                {{ $root._('View capture on {date}', {date: tooltipPeriod.snapshotPeriod.snapshot.getTimeDateFormatted()}) }}\n              </div>\n              <div v-else-if=\"tooltipPeriod.snapshotCount\">\n                {{ $root._(\n                  isTooltipPeriodDayOrHour ? '{capture_text} on {date}':'{capture_text} in {month}', // TODO: split translation into \"in {year}\" and \"in {month}\"\n                  { capture_text: $root._(tooltipPeriod.snapshotCount !== 1 ? '{count} captures' : '{count} capture', {count: tooltipPeriod.snapshotCount}), [isTooltipPeriodDayOrHour ? 'date':'month']: tooltipPeriod.getFullReadableId() } )\n                }}\n              </div>\n            </template>\n        </div>\n        <div v-html=\"'&#x25C0;'\"\n          class=\"arrow previous\"\n          :class=\"{disabled: isScrollZero && !previousPeriod}\"\n          @click=\"scrollPrev\"\n          @keyup.enter=\"scrollPrev\"\n          @dblclick.stop.prevent tabindex=\"0\"></div>\n        <div class=\"scroll\" ref=\"periodScroll\" :class=\"{highlight: highlight}\">\n            <div class=\"periods\" ref=\"periods\">\n                <div v-for=\"subPeriod in period.children\"\n                     :key=\"subPeriod.fullId\"\n                     class=\"period\"\n                     :class=\"{empty: !subPeriod.snapshotCount, highlight: highlightPeriod === subPeriod, 'last-level': !canZoom, 'contains-current-snapshot': containsCurrentSnapshot(subPeriod) }\"\n                >\n                    <div class=\"histo\">\n                        <div class=\"line\"\n                             v-for=\"histoPeriod in subPeriod.children\"\n                             :key=\"histoPeriod.fullId\"\n                             :style=\"{height: getHistoLineHeight(histoPeriod.snapshotCount)}\"\n                             :class=\"{'has-single-snapshot': histoPeriod.snapshotCount === 1, 'contains-current-snapshot': containsCurrentSnapshot(histoPeriod)}\"\n                             @click=\"changePeriod(histoPeriod, $event)\"\n                             @keyup.enter=\"changePeriod(histoPeriod, $event)\"\n                             @mouseover=\"setTooltipPeriod(histoPeriod, $event)\"\n                             @mouseout=\"setTooltipPeriod(null, $event)\"\n                             tabindex=\"0\"\n                        >\n                        </div>\n                    </div>\n                    <div class=\"inner\"\n                         :class=\"{'has-single-snapshot': subPeriod.snapshotCount === 1}\"\n                         @click=\"changePeriod(subPeriod, $event)\"\n                         @keyup.enter=\"changePeriod(histoPeriod, $event)\"\n                         @mouseover=\"setTooltipPeriod(subPeriod, $event)\"\n                         @mouseout=\"setTooltipPeriod(null, $event)\"\n                         tabindex=\"0\"\n                    >\n                        <div class=\"label\">\n                          {{subPeriod.getReadableId()}}\n                        </div>\n                    </div>\n                </div>\n            </div>\n        </div>\n        <div\n          v-html=\"'&#x25B6;'\"\n          class=\"arrow next\"\n          :class=\"{disabled: isScrollMax && !nextPeriod}\"\n          @click=\"scrollNext\"\n          @keyup.enter=\"scrollNext\"\n          @dblclick.stop.prevent tabindex=\"0\"></div>\n    </div>\n</template>\n\n<script>\nimport { PywbPeriod } from \"../model.js\";\n\nexport default{\n  props: {\n    period: { required: true },\n    currentSnapshot: { required: false, default: null},\n    highlight: { required: false, default: false},\n    stayWithinPeriod: { required: false, default: false},\n    maxZoomLevel: { required: false, default: PywbPeriod.Type.snapshot}\n  },\n  data: function() {\n    return {\n      highlightPeriod: null,\n      previousPeriod: null,\n      nextPeriod: null,\n      isScrollZero: true,\n      isScrollMax: true,\n      tooltipPeriod: null,\n      tooltipPeriodPos: {x:0,y:0}\n    };\n  },\n  created: function() {\n    this.addEmptySubPeriods();\n  },\n  mounted: function() {\n    this.$refs.periods._computedStyle = window.getComputedStyle(this.$refs.periods);\n    this.$refs.periodScroll._computedStyle = window.getComputedStyle(this.$refs.periodScroll);\n    this.$watch(\"period\", this.onPeriodChanged);\n\n    this.$refs.periodScroll.addEventListener(\"scroll\", this.updateScrollArrows);\n    window.addEventListener(\"resize\", this.updateScrollArrows);\n    this.updateScrollArrows();\n  },\n  computed: {\n    // this determins which the last zoom level is before we go straight to showing snapshot\n    canZoom() {\n      return this.period.type < this.maxZoomLevel;\n    },\n    isTooltipPeriodDayOrHour() {\n      return this.tooltipPeriod.type >= PywbPeriod.Type.day;\n    },\n    iContainCurrentSnapshot() {\n      return this.currentSnapshot && this.period.contains(this.currentSnapshot);\n    }\n  },\n  updated() {\n    // do something on update\n  },\n  methods: {\n    containsCurrentSnapshot(period) {\n      return this.iContainCurrentSnapshot && period.contains(this.currentSnapshot);\n    },\n    addEmptySubPeriods() {\n      this.period.fillEmptyChildPeriods(true);\n    },\n    updateScrollArrows() {\n      this.period.scroll = this.$refs.periodScroll.scrollLeft;\n      const maxScroll = parseInt(this.$refs.periods._computedStyle.width) - parseInt(this.$refs.periodScroll._computedStyle.width);\n      this.isScrollZero = !this.period.scroll; // if 0, then true (we are at scroll zero)\n      this.isScrollMax = Math.abs(maxScroll - this.period.scroll) < 5;\n    },\n    restoreScroll() {\n      this.$refs.periodScroll.scrollLeft = this.period.scroll;\n    },\n    scrollNext: function () {\n      if (this.isScrollMax) {\n        if (this.nextPeriod) {\n          this.$emit(\"goto-period\", this.nextPeriod, true /* onlyZoomToPeriod */);\n        }\n      } else {\n        this.$refs.periodScroll.scrollLeft += 30;\n      }\n    },\n    scrollPrev: function () {\n      if (this.isScrollZero) {\n        if (this.previousPeriod) {\n          this.$emit(\"goto-period\", this.previousPeriod, true /* onlyZoomToPeriod */);\n        }\n      } else {\n        this.$refs.periodScroll.scrollLeft -= 30;\n      }\n    },\n    getTimeFormatted: function(date) {\n      return (date.hour < 13 ? date.hour : (date.hour % 12)) + \":\" + ((date.minute < 10 ? \"0\":\"\")+date.minute) + \" \" + (date.hour < 12 ? \"am\":\"pm\");\n    },\n    getHistoLineHeight: function(value) {\n      const percent = Math.ceil((value/this.period.maxGrandchildSnapshotCount) * 100);\n      return (percent ? (5 + Math.ceil(percent*.95)) : 0) + \"%\";\n      // return percent + '%';\n    },\n    changePeriod(period, $event) {\n      // if not empty\n      if (period.snapshotCount) {\n        let periodToChangeTo = null;\n        // if contains a single snapshot only, navigate to snapshot (load snapshot in FRAME, do not ZOOM IN)\n        if (period.snapshot) {\n          // if period is at level \"snapshot\" (no more children), send period, else send the child period, a reference to which is stored (by data/model layer) in the current period; App event needs a period to be passed (cannot pass in snapshot object itself)\n          if (period.type === PywbPeriod.Type.snapshot) {\n            periodToChangeTo = period;\n          } else if (period.snapshotPeriod) {\n            periodToChangeTo = period.snapshotPeriod;\n          }\n        } else {\n        // if contains mulitple snapshots,\n          // zoom if ZOOM level is day or less, OR if period contain TOO MANY (>10)\n          if (this.canZoom) {\n            periodToChangeTo = period;\n          }\n        }\n\n        // if we selected a period to go to, emit event\n        if (periodToChangeTo) {\n          this.$emit(\"goto-period\", periodToChangeTo);\n        }\n      }\n      $event.stopPropagation();\n      return false;\n    },\n    onPeriodChanged(newPeriod, oldPeriod) {\n      this.addEmptySubPeriods();\n      const previousPeriod = this.period.getPrevious();\n      const nextPeriod = this.period.getNext();\n      if (!this.stayWithinPeriod || this.stayWithinPeriod.contains(previousPeriod)) {\n        this.previousPeriod = previousPeriod;\n      }\n      if (!this.stayWithinPeriod || this.stayWithinPeriod.contains(nextPeriod)) {\n        this.nextPeriod = nextPeriod;\n      }\n\n      // detect if going up level of period (new period type should be in old period parents)\n      if (oldPeriod && oldPeriod.type - newPeriod.type > 0) {\n        let highlightPeriod = oldPeriod;\n        for (let i=oldPeriod.type - newPeriod.type; i > 1; i--) {\n          highlightPeriod = highlightPeriod.parent;\n        }\n        this.highlightPeriod = highlightPeriod;\n        setTimeout((function() {\n          this.highlightPeriod = null;\n        }).bind(this), 2000);\n      }\n      setTimeout((function() {\n        this.restoreScroll();\n        this.updateScrollArrows();\n      }).bind(this), 1);\n    },\n    setTooltipPeriod(period, event) {\n      if (!period || !period.snapshotCount) {\n        this.tooltipPeriod = null;\n        return;\n      }\n      this.tooltipPeriod = period;\n\n      this.$nextTick(function() {\n        const tooltipContentsEl = document.querySelector('.period-tooltip div');\n        if (!tooltipContentsEl) {\n          return;\n        }\n\n        const periodTooltipStyle = window.getComputedStyle(tooltipContentsEl);\n        const tooltipWidth = parseInt(periodTooltipStyle.width);\n        const tooltipHeight = parseInt(periodTooltipStyle.height);\n        const spacing = 10;\n        if (window.innerWidth < event.x + (spacing*2) + tooltipWidth) {\n          this.tooltipPeriodPos.x = event.x - (tooltipWidth + spacing);\n        } else {\n          this.tooltipPeriodPos.x = event.x + spacing;\n        }\n        this.tooltipPeriodPos.y = event.y - (spacing + tooltipHeight);\n      });\n      event.stopPropagation();\n      return false;\n    }\n  }\n};\n</script>\n\n\n<style>\n    .timeline {\n        position: relative;\n        display: flex;\n        width: auto;\n        height: 60px;\n        margin: 5px;\n        justify-content: left;\n    }\n\n    .timeline .id {\n        display: inline-block;\n        font-size: 30px;\n    }\n    .timeline .arrow {\n        display: inline-block;\n        width: 20px;\n        font-size: 20px; /* font-size = width of arrow, as it UTF char */\n        line-height: 60px;\n        vertical-align: top;\n        cursor: pointer;\n    }\n    .timeline .arrow.previous {\n    }\n    .timeline .arrow.next {\n    }\n    .timeline .arrow.disabled, .timeline .arrow.disabled:hover {\n        /*color: lightgray;*/\n        background-color: transparent;\n        /*cursor: not-allowed;*/\n        visibility: hidden;\n    }\n    .timeline .arrow:hover {\n        background-color: antiquewhite;\n        color: firebrick;\n    }\n\n    .timeline .scroll {\n        position: relative;\n        display: inline-block;\n        width: 100%; /* */\n        height: 100%;\n\n        /* maker scrollable horizontally */\n        overflow-x: scroll;\n        overflow-y: hidden;\n        white-space: nowrap;\n        scroll-behavior: smooth;\n\n        text-align: center;\n\n        transition: background-color 500ms ease-in;\n    }\n    /* hide scroll bar */\n    .timeline .scroll::-webkit-scrollbar {\n        display: none;\n    }\n    /* highlight the scroll period: usually triggered from root app */\n    .timeline .scroll.highlight {\n        background-color: #fff7ce;\n    }\n    .timeline .scroll .periods {\n        display: flex;\n        justify-content: space-between;\n        height: 100%;\n        width: 100%;\n        min-width: 600px;\n    }\n\n\n    .timeline .period {\n        flex-grow: 1;\n        position: relative;\n        display: inline-block;\n        height: 100%;\n        /* line-height: 80px; /* use to center middle vertically */\n        white-space: normal;\n        vertical-align: top;\n        text-align: center;\n        background-color: transparent;\n\n        transition: background-color 500ms ease-in-out;\n    }\n    /* 1st period period child el */\n    .timeline .period:nth-child(1) {\n        /*border-left: 1px solid white; !* has left border; all other periods have right border *!*/\n    }\n\n    .timeline .period:hover {\n        background-color: #eeeeee;\n    }\n    .timeline .period.contains-current-snapshot, .timeline .period.contains-current-snapshot:hover {\n        background-color: #f7def4;\n    }\n\n    /* empty period */\n    .timeline .period.empty {\n        color: #aaa;\n        /*background-color: transparent;*/\n    }\n    /* highlighted period */\n    .timeline .period.highlight {\n        background-color: cyan;\n    }\n\n    .timeline .period .inner {\n        display: block;\n        position: absolute;\n        bottom: 0;\n        left: 0;\n        width: 100%;\n        height: 20px;\n        background-color: white;\n        border-top: 1px solid gray;\n        white-space: nowrap;\n        cursor: zoom-in;\n    }\n    .timeline .period .inner.has-single-snapshot {\n      cursor: pointer;\n    }\n    .timeline .period.last-level .inner, .timeline .period.empty .inner {\n      cursor: default;\n    }\n\n    .timeline .period .label {\n      width: 100%;\n      font-weight: bold;\n      font-size: 14px;\n      transition: background-color 500ms ease-in;\n    }\n    .timeline .period:hover .label {\n      position: absolute;\n      z-index: 20;\n      background-color: lightgrey;\n    }\n\n    .timeline .period .histo {\n        display: flex;\n        position: absolute;\n        top: 1px;\n        left: 0;\n        width: 100%;\n        height: 39px;\n        align-items: flex-end;\n        justify-content: space-between;\n        text-align: left;\n    }\n\n    .timeline .period .histo .line {\n        position: relative;\n        flex-grow: 1;\n        display: inline-block;\n        background-color: #a6cdf5;\n        margin: 0;\n        padding: 0;\n        cursor: zoom-in;\n    }\n    .timeline .period .histo .line.has-single-snapshot {\n      cursor: pointer;\n    }\n\n    /* Last level period histogram spaces things evenly */\n    .timeline .period.last-level .histo {\n        justify-content: space-around;\n    }\n\n    /* Last level period histogram lines do not grow, but are fixed width/margin */\n    .timeline .period.last-level .histo .line {\n        flex-grow: unset;\n        width: 5px;\n        margin-left: 2px;\n    }\n\n        /* update line color on hover*/\n        .timeline .period .histo .line:hover {\n            background-color: #f5a6eb;\n        }\n\n        .timeline .period .histo .line.contains-current-snapshot {\n            background-color: red;\n        }\n\n        /* Period that contains ONE snapshot only will show snapshot info*/\n        .timeline .period-tooltip {\n            position: fixed;\n            z-index: 100;\n            /*left or right set programmatically*/\n            display: block;\n            background-color: white;\n            border: 1px solid gray;\n            padding: 2px;\n            white-space: nowrap; /*no wrapping allowed*/\n        }\n            /*show on hover*/\n            .timeline .period-tooltip.show {\n                display: block;\n            }\n\n</style>\n"]
+                "sourcesContent": ["<template>\n    <div class=\"timeline\">\n        <div class=\"period-tooltip\" v-show=\"tooltipPeriod\" :style=\"{left: tooltipPeriodPos.x+'px', top: tooltipPeriodPos.y+'px'}\">\n            <template v-if=\"tooltipPeriod\">\n              <div v-if=\"tooltipPeriod.snapshot\">\n                {{ $root._('View capture on {date}', {date: tooltipPeriod.snapshot.getTimeDateFormatted()}) }}\n              </div>\n              <div v-else-if=\"tooltipPeriod.snapshotPeriod\">\n                {{ $root._('View capture on {date}', {date: tooltipPeriod.snapshotPeriod.snapshot.getTimeDateFormatted()}) }}\n              </div>\n              <div v-else-if=\"tooltipPeriod.snapshotCount\">\n                {{ $root._(\n                  isTooltipPeriodDayOrHour ? '{capture_text} on {date}':'{capture_text} in {month}', // TODO: split translation into \"in {year}\" and \"in {month}\"\n                  { capture_text: $root._(tooltipPeriod.snapshotCount !== 1 ? '{count} captures' : '{count} capture', {count: tooltipPeriod.snapshotCount}), [isTooltipPeriodDayOrHour ? 'date':'month']: tooltipPeriod.getFullReadableId() } )\n                }}\n              </div>\n            </template>\n        </div>\n        <div v-html=\"'&#x25C0;'\"\n          class=\"arrow previous\"\n          :class=\"{disabled: isScrollZero && !previousPeriod}\"\n          @click=\"scrollPrev\"\n          @keyup.enter=\"scrollPrev\"\n          @dblclick.stop.prevent tabindex=\"0\"></div>\n        <div class=\"scroll\" ref=\"periodScroll\" :class=\"{highlight: highlight}\">\n            <div class=\"periods\" ref=\"periods\">\n                <div v-for=\"subPeriod in period.children\"\n                     :key=\"subPeriod.fullId\"\n                     class=\"period\"\n                     :class=\"{empty: !subPeriod.snapshotCount, highlight: highlightPeriod === subPeriod, 'last-level': !canZoom, 'contains-current-snapshot': containsCurrentSnapshot(subPeriod) }\"\n                >\n                    <div class=\"histo\">\n                        <div class=\"line\"\n                             v-for=\"histoPeriod in subPeriod.children\"\n                             :key=\"histoPeriod.fullId\"\n                             :style=\"{height: getHistoLineHeight(histoPeriod.snapshotCount)}\"\n                             :class=\"{'has-single-snapshot': histoPeriod.snapshotCount === 1, 'contains-current-snapshot': containsCurrentSnapshot(histoPeriod)}\"\n                             @click=\"changePeriod(histoPeriod, $event)\"\n                             @keyup.enter=\"changePeriod(histoPeriod, $event)\"\n                             @mouseover=\"setTooltipPeriod(histoPeriod, $event)\"\n                             @mouseout=\"setTooltipPeriod(null, $event)\"\n                             :tabindex=\"histoPeriod.snapshotCount > 0 ? 0 : -1\"\n                        >\n                        </div>\n                    </div>\n                    <div class=\"inner\"\n                         :class=\"{'has-single-snapshot': subPeriod.snapshotCount === 1}\"\n                         @click=\"changePeriod(subPeriod, $event)\"\n                         @keyup.enter=\"changePeriod(histoPeriod, $event)\"\n                         @mouseover=\"setTooltipPeriod(subPeriod, $event)\"\n                         @mouseout=\"setTooltipPeriod(null, $event)\"\n                    >\n                        <div class=\"label\">\n                          {{subPeriod.getReadableId()}}\n                        </div>\n                    </div>\n                </div>\n            </div>\n        </div>\n        <div\n          v-html=\"'&#x25B6;'\"\n          class=\"arrow next\"\n          :class=\"{disabled: isScrollMax && !nextPeriod}\"\n          @click=\"scrollNext\"\n          @keyup.enter=\"scrollNext\"\n          @dblclick.stop.prevent tabindex=\"0\"></div>\n    </div>\n</template>\n\n<script>\nimport { PywbPeriod } from \"../model.js\";\n\nexport default{\n  props: {\n    period: { required: true },\n    currentSnapshot: { required: false, default: null},\n    highlight: { required: false, default: false},\n    stayWithinPeriod: { required: false, default: false},\n    maxZoomLevel: { required: false, default: PywbPeriod.Type.snapshot}\n  },\n  data: function() {\n    return {\n      highlightPeriod: null,\n      previousPeriod: null,\n      nextPeriod: null,\n      isScrollZero: true,\n      isScrollMax: true,\n      tooltipPeriod: null,\n      tooltipPeriodPos: {x:0,y:0}\n    };\n  },\n  created: function() {\n    this.addEmptySubPeriods();\n  },\n  mounted: function() {\n    this.$refs.periods._computedStyle = window.getComputedStyle(this.$refs.periods);\n    this.$refs.periodScroll._computedStyle = window.getComputedStyle(this.$refs.periodScroll);\n    this.$watch(\"period\", this.onPeriodChanged);\n\n    this.$refs.periodScroll.addEventListener(\"scroll\", this.updateScrollArrows);\n    window.addEventListener(\"resize\", this.updateScrollArrows);\n    this.updateScrollArrows();\n  },\n  computed: {\n    // this determins which the last zoom level is before we go straight to showing snapshot\n    canZoom() {\n      return this.period.type < this.maxZoomLevel;\n    },\n    isTooltipPeriodDayOrHour() {\n      return this.tooltipPeriod.type >= PywbPeriod.Type.day;\n    },\n    iContainCurrentSnapshot() {\n      return this.currentSnapshot && this.period.contains(this.currentSnapshot);\n    }\n  },\n  updated() {\n    // do something on update\n  },\n  methods: {\n    containsCurrentSnapshot(period) {\n      return this.iContainCurrentSnapshot && period.contains(this.currentSnapshot);\n    },\n    addEmptySubPeriods() {\n      this.period.fillEmptyChildPeriods(true);\n    },\n    updateScrollArrows() {\n      this.period.scroll = this.$refs.periodScroll.scrollLeft;\n      const maxScroll = parseInt(this.$refs.periods._computedStyle.width) - parseInt(this.$refs.periodScroll._computedStyle.width);\n      this.isScrollZero = !this.period.scroll; // if 0, then true (we are at scroll zero)\n      this.isScrollMax = Math.abs(maxScroll - this.period.scroll) < 5;\n    },\n    restoreScroll() {\n      this.$refs.periodScroll.scrollLeft = this.period.scroll;\n    },\n    scrollNext: function () {\n      if (this.isScrollMax) {\n        if (this.nextPeriod) {\n          this.$emit(\"goto-period\", this.nextPeriod, true /* onlyZoomToPeriod */);\n        }\n      } else {\n        this.$refs.periodScroll.scrollLeft += 30;\n      }\n    },\n    scrollPrev: function () {\n      if (this.isScrollZero) {\n        if (this.previousPeriod) {\n          this.$emit(\"goto-period\", this.previousPeriod, true /* onlyZoomToPeriod */);\n        }\n      } else {\n        this.$refs.periodScroll.scrollLeft -= 30;\n      }\n    },\n    getTimeFormatted: function(date) {\n      return (date.hour < 13 ? date.hour : (date.hour % 12)) + \":\" + ((date.minute < 10 ? \"0\":\"\")+date.minute) + \" \" + (date.hour < 12 ? \"am\":\"pm\");\n    },\n    getHistoLineHeight: function(value) {\n      const percent = Math.ceil((value/this.period.maxGrandchildSnapshotCount) * 100);\n      return (percent ? (5 + Math.ceil(percent*.95)) : 0) + \"%\";\n      // return percent + '%';\n    },\n    changePeriod(period, $event) {\n      // if not empty\n      if (period.snapshotCount) {\n        let periodToChangeTo = null;\n        // if contains a single snapshot only, navigate to snapshot (load snapshot in FRAME, do not ZOOM IN)\n        if (period.snapshot) {\n          // if period is at level \"snapshot\" (no more children), send period, else send the child period, a reference to which is stored (by data/model layer) in the current period; App event needs a period to be passed (cannot pass in snapshot object itself)\n          if (period.type === PywbPeriod.Type.snapshot) {\n            periodToChangeTo = period;\n          } else if (period.snapshotPeriod) {\n            periodToChangeTo = period.snapshotPeriod;\n          }\n        } else {\n        // if contains mulitple snapshots,\n          // zoom if ZOOM level is day or less, OR if period contain TOO MANY (>10)\n          if (this.canZoom) {\n            periodToChangeTo = period;\n          }\n        }\n\n        // if we selected a period to go to, emit event\n        if (periodToChangeTo) {\n          this.$emit(\"goto-period\", periodToChangeTo);\n        }\n      }\n      $event.stopPropagation();\n      return false;\n    },\n    onPeriodChanged(newPeriod, oldPeriod) {\n      this.addEmptySubPeriods();\n      const previousPeriod = this.period.getPrevious();\n      const nextPeriod = this.period.getNext();\n      if (!this.stayWithinPeriod || this.stayWithinPeriod.contains(previousPeriod)) {\n        this.previousPeriod = previousPeriod;\n      }\n      if (!this.stayWithinPeriod || this.stayWithinPeriod.contains(nextPeriod)) {\n        this.nextPeriod = nextPeriod;\n      }\n\n      // detect if going up level of period (new period type should be in old period parents)\n      if (oldPeriod && oldPeriod.type - newPeriod.type > 0) {\n        let highlightPeriod = oldPeriod;\n        for (let i=oldPeriod.type - newPeriod.type; i > 1; i--) {\n          highlightPeriod = highlightPeriod.parent;\n        }\n        this.highlightPeriod = highlightPeriod;\n        setTimeout((function() {\n          this.highlightPeriod = null;\n        }).bind(this), 2000);\n      }\n      setTimeout((function() {\n        this.restoreScroll();\n        this.updateScrollArrows();\n      }).bind(this), 1);\n    },\n    setTooltipPeriod(period, event) {\n      if (!period || !period.snapshotCount) {\n        this.tooltipPeriod = null;\n        return;\n      }\n      this.tooltipPeriod = period;\n\n      this.$nextTick(function() {\n        const tooltipContentsEl = document.querySelector('.period-tooltip div');\n        if (!tooltipContentsEl) {\n          return;\n        }\n\n        const periodTooltipStyle = window.getComputedStyle(tooltipContentsEl);\n        const tooltipWidth = parseInt(periodTooltipStyle.width);\n        const tooltipHeight = parseInt(periodTooltipStyle.height);\n        const spacing = 10;\n        if (window.innerWidth < event.x + (spacing*2) + tooltipWidth) {\n          this.tooltipPeriodPos.x = event.x - (tooltipWidth + spacing);\n        } else {\n          this.tooltipPeriodPos.x = event.x + spacing;\n        }\n        this.tooltipPeriodPos.y = event.y - (spacing + tooltipHeight);\n      });\n      event.stopPropagation();\n      return false;\n    }\n  }\n};\n</script>\n\n\n<style>\n    .timeline {\n        position: relative;\n        display: flex;\n        width: auto;\n        height: 60px;\n        margin: 5px;\n        justify-content: left;\n    }\n\n    .timeline .id {\n        display: inline-block;\n        font-size: 30px;\n    }\n    .timeline .arrow {\n        display: inline-block;\n        width: 20px;\n        font-size: 20px; /* font-size = width of arrow, as it UTF char */\n        line-height: 60px;\n        vertical-align: top;\n        cursor: pointer;\n    }\n    .timeline .arrow.previous {\n    }\n    .timeline .arrow.next {\n    }\n    .timeline .arrow.disabled, .timeline .arrow.disabled:hover {\n        /*color: lightgray;*/\n        background-color: transparent;\n        /*cursor: not-allowed;*/\n        visibility: hidden;\n    }\n    .timeline .arrow:hover {\n        background-color: antiquewhite;\n        color: firebrick;\n    }\n\n    .timeline .scroll {\n        position: relative;\n        display: inline-block;\n        width: 100%; /* */\n        height: 100%;\n\n        /* maker scrollable horizontally */\n        overflow-x: scroll;\n        overflow-y: hidden;\n        white-space: nowrap;\n        scroll-behavior: smooth;\n\n        text-align: center;\n\n        transition: background-color 500ms ease-in;\n    }\n    /* hide scroll bar */\n    .timeline .scroll::-webkit-scrollbar {\n        display: none;\n    }\n    /* highlight the scroll period: usually triggered from root app */\n    .timeline .scroll.highlight {\n        background-color: #fff7ce;\n    }\n    .timeline .scroll .periods {\n        display: flex;\n        justify-content: space-between;\n        height: 100%;\n        width: 100%;\n        min-width: 600px;\n    }\n\n\n    .timeline .period {\n        flex-grow: 1;\n        position: relative;\n        display: inline-block;\n        height: 100%;\n        /* line-height: 80px; /* use to center middle vertically */\n        white-space: normal;\n        vertical-align: top;\n        text-align: center;\n        background-color: transparent;\n\n        transition: background-color 500ms ease-in-out;\n    }\n    /* 1st period period child el */\n    .timeline .period:nth-child(1) {\n        /*border-left: 1px solid white; !* has left border; all other periods have right border *!*/\n    }\n\n    .timeline .period:hover {\n        background-color: #eeeeee;\n    }\n    .timeline .period.contains-current-snapshot, .timeline .period.contains-current-snapshot:hover {\n        background-color: #f7def4;\n    }\n\n    /* empty period */\n    .timeline .period.empty {\n        color: #aaa;\n        /*background-color: transparent;*/\n    }\n    /* highlighted period */\n    .timeline .period.highlight {\n        background-color: cyan;\n    }\n\n    .timeline .period .inner {\n        display: block;\n        position: absolute;\n        bottom: 0;\n        left: 0;\n        width: 100%;\n        height: 20px;\n        background-color: white;\n        border-top: 1px solid gray;\n        white-space: nowrap;\n        cursor: zoom-in;\n    }\n    .timeline .period .inner.has-single-snapshot {\n      cursor: pointer;\n    }\n    .timeline .period.last-level .inner, .timeline .period.empty .inner {\n      cursor: default;\n    }\n\n    .timeline .period .label {\n      width: 100%;\n      font-weight: bold;\n      font-size: 14px;\n      transition: background-color 500ms ease-in;\n    }\n    .timeline .period:hover .label {\n      position: absolute;\n      z-index: 20;\n      background-color: lightgrey;\n    }\n\n    .timeline .period .histo {\n        display: flex;\n        position: absolute;\n        top: 1px;\n        left: 0;\n        width: 100%;\n        height: 39px;\n        align-items: flex-end;\n        justify-content: space-between;\n        text-align: left;\n    }\n\n    .timeline .period .histo .line {\n        position: relative;\n        flex-grow: 1;\n        display: inline-block;\n        background-color: #a6cdf5;\n        margin: 0;\n        padding: 0;\n        cursor: zoom-in;\n    }\n    .timeline .period .histo .line.has-single-snapshot {\n      cursor: pointer;\n    }\n\n    /* Last level period histogram spaces things evenly */\n    .timeline .period.last-level .histo {\n        justify-content: space-around;\n    }\n\n    /* Last level period histogram lines do not grow, but are fixed width/margin */\n    .timeline .period.last-level .histo .line {\n        flex-grow: unset;\n        width: 5px;\n        margin-left: 2px;\n    }\n\n        /* update line color on hover*/\n        .timeline .period .histo .line:hover {\n            background-color: #f5a6eb;\n        }\n\n        .timeline .period .histo .line.contains-current-snapshot {\n            background-color: red;\n        }\n\n        /* Period that contains ONE snapshot only will show snapshot info*/\n        .timeline .period-tooltip {\n            position: fixed;\n            z-index: 100;\n            /*left or right set programmatically*/\n            display: block;\n            background-color: white;\n            border: 1px solid gray;\n            padding: 2px;\n            white-space: nowrap; /*no wrapping allowed*/\n        }\n            /*show on hover*/\n            .timeline .period-tooltip.show {\n                display: block;\n            }\n\n</style>\n"]
             },
             media: undefined
         });
 
     };
     /* scoped */
     const __vue_scope_id__$6 = undefined;
@@ -1386,18 +1383,16 @@
                                             return null
                                         }
                                         return _vm.changePeriod(_vm.parents[0])
                                     }
                                 }
                             },
                             [
-                                _c("img", {
-                                    attrs: {
-                                        src: "/static/zoom-out-icon-333316.png"
-                                    }
+                                _c("i", {
+                                    staticClass: "fa fa-search-minus"
                                 }),
                                 _vm._v(
                                     " " +
                                     _vm._s(_vm.parents[0].getReadableId(true)) +
                                     "\n            "
                                 )
                             ]
@@ -1485,23 +1480,23 @@
     };
     var __vue_staticRenderFns__$5 = [];
     __vue_render__$5._withStripped = true;
 
     /* style */
     const __vue_inject_styles__$5 = function(inject) {
         if (!inject) return
-        inject("data-v-7ed1ae1d_0", {
+        inject("data-v-6060fb7e_0", {
             source: "\n.breadcrumbs {\n  text-align: center;\n}\n.breadcrumbs .item {\n    position: relative;\n    display: inline;\n    margin: 0 2px 0 0;\n    font-size: inherit;\n}\n.breadcrumbs .count {\n    /*vertical-align: middle;*/\n    font-size: inherit;\n}\n.breadcrumbs .item .goto {\n    display: inline-block;\n    margin: 1px;\n    padding: 1px;\n    cursor: zoom-out;\n    border-radius: 5px;\n    background-color: #eeeeee;\n}\n.breadcrumbs .item .goto:hover {\n    background-color: #a6cdf5;\n}\n.breadcrumbs .item .goto img {\n  height: 15px;\n}\n.breadcrumbs .item.snapshot {\n    display: block;\n}\n\n",
             map: {
                 "version": 3,
                 "sources": ["/Users/tessa/dev/pywb/pywb/vueui/src/components/TimelineBreadcrumbs.vue"],
                 "names": [],
                 "mappings": ";AA0DA;EACA,kBAAA;AACA;AACA;IACA,kBAAA;IACA,eAAA;IACA,iBAAA;IACA,kBAAA;AACA;AACA;IACA,0BAAA;IACA,kBAAA;AACA;AAEA;IACA,qBAAA;IACA,WAAA;IACA,YAAA;IACA,gBAAA;IACA,kBAAA;IACA,yBAAA;AACA;AACA;IACA,yBAAA;AACA;AACA;EACA,YAAA;AACA;AAEA;IACA,cAAA;AACA",
                 "file": "TimelineBreadcrumbs.vue",
-                "sourcesContent": ["<template>\n    <div class=\"breadcrumbs\">\n        <template v-if=\"parents.length\">\n            <span class=\"item\">\n                <span\n                    class=\"goto\"\n                    @click=\"changePeriod(parents[0])\"\n                    @keyup.enter=\"changePeriod(parents[0])\"\n                    :title=\"getPeriodZoomOutText(parents[0])\"\n                    tabindex=\"1\">\n                  <img src=\"/static/zoom-out-icon-333316.png\" /> {{parents[0].getReadableId(true)}}\n                </span>\n            </span>\n            &gt;\n            <span v-for=\"(parent,i) in parents\" :key=\"parent.id\" class=\"item\" v-if=\"i > 0\">\n                <span\n                    class=\"goto\"\n                    @click=\"changePeriod(parent)\"\n                    @keyup.enter=\"changePeriod(parent)\"\n                    :title=\"getPeriodZoomOutText(parent)\"\n                    tabindex=\"1\">\n                  {{parent.getReadableId(true)}}\n                </span>\n            </span>\n        </template>\n        <span class=\"item\">\n            <span class=\"current\">{{period.getReadableId(true)}}</span>\n            <span class=\"count\">({{ $root._(period.snapshotCount !== 1 ? '{count} captures':'{count} capture', {count: period.snapshotCount}) }})</span>\n        </span>\n    </div>\n</template>\n\n<script>\nexport default {\n  props: {\n    period: {\n      required: true\n    }\n  },\n  computed: {\n    parents: function() {\n      return this.period.getParents();\n    }\n  },\n  methods: {\n    getPeriodZoomOutText(period) {\n      return 'Zoom out to '+period.getReadableId(true)+ ' ('+period.snapshotCount+' captures)';\n    },\n    changePeriod(period) {\n      if (period.snapshotCount) {\n        this.$emit(\"goto-period\", period);\n      }\n    },\n  }\n};\n</script>\n\n<style>\n    .breadcrumbs {\n      text-align: center;\n    }\n    .breadcrumbs .item {\n        position: relative;\n        display: inline;\n        margin: 0 2px 0 0;\n        font-size: inherit;\n    }\n    .breadcrumbs .count {\n        /*vertical-align: middle;*/\n        font-size: inherit;\n    }\n\n    .breadcrumbs .item .goto {\n        display: inline-block;\n        margin: 1px;\n        padding: 1px;\n        cursor: zoom-out;\n        border-radius: 5px;\n        background-color: #eeeeee;\n     }\n    .breadcrumbs .item .goto:hover {\n        background-color: #a6cdf5;\n    }\n    .breadcrumbs .item .goto img {\n      height: 15px;\n    }\n\n    .breadcrumbs .item.snapshot {\n        display: block;\n    }\n\n</style>\n"]
+                "sourcesContent": ["<template>\n    <div class=\"breadcrumbs\">\n        <template v-if=\"parents.length\">\n            <span class=\"item\">\n                <span\n                    class=\"goto\"\n                    @click=\"changePeriod(parents[0])\"\n                    @keyup.enter=\"changePeriod(parents[0])\"\n                    :title=\"getPeriodZoomOutText(parents[0])\"\n                    tabindex=\"1\">\n                  <i class=\"fa fa-search-minus\"></i> {{parents[0].getReadableId(true)}}\n                </span>\n            </span>\n            &gt;\n            <span v-for=\"(parent,i) in parents\" :key=\"parent.id\" class=\"item\" v-if=\"i > 0\">\n                <span\n                    class=\"goto\"\n                    @click=\"changePeriod(parent)\"\n                    @keyup.enter=\"changePeriod(parent)\"\n                    :title=\"getPeriodZoomOutText(parent)\"\n                    tabindex=\"1\">\n                  {{parent.getReadableId(true)}}\n                </span>\n            </span>\n        </template>\n        <span class=\"item\">\n            <span class=\"current\">{{period.getReadableId(true)}}</span>\n            <span class=\"count\">({{ $root._(period.snapshotCount !== 1 ? '{count} captures':'{count} capture', {count: period.snapshotCount}) }})</span>\n        </span>\n    </div>\n</template>\n\n<script>\nexport default {\n  props: {\n    period: {\n      required: true\n    }\n  },\n  computed: {\n    parents: function() {\n      return this.period.getParents();\n    }\n  },\n  methods: {\n    getPeriodZoomOutText(period) {\n      return 'Zoom out to '+period.getReadableId(true)+ ' ('+period.snapshotCount+' captures)';\n    },\n    changePeriod(period) {\n      if (period.snapshotCount) {\n        this.$emit(\"goto-period\", period);\n      }\n    },\n  }\n};\n</script>\n\n<style>\n    .breadcrumbs {\n      text-align: center;\n    }\n    .breadcrumbs .item {\n        position: relative;\n        display: inline;\n        margin: 0 2px 0 0;\n        font-size: inherit;\n    }\n    .breadcrumbs .count {\n        /*vertical-align: middle;*/\n        font-size: inherit;\n    }\n\n    .breadcrumbs .item .goto {\n        display: inline-block;\n        margin: 1px;\n        padding: 1px;\n        cursor: zoom-out;\n        border-radius: 5px;\n        background-color: #eeeeee;\n     }\n    .breadcrumbs .item .goto:hover {\n        background-color: #a6cdf5;\n    }\n    .breadcrumbs .item .goto img {\n      height: 15px;\n    }\n\n    .breadcrumbs .item.snapshot {\n        display: block;\n    }\n\n</style>\n"]
             },
             media: undefined
         });
 
     };
     /* scoped */
     const __vue_scope_id__$5 = undefined;
@@ -2362,14 +2357,17 @@
                     '--navbar-background': `#${this.config.navbarBackground}`,
                     '--navbar-color': `#${this.config.navbarColor}`
                 }
             },
             lightButtons() {
                 return !!this.config.navbarLightButtons;
             },
+            printingEnabled() {
+                return !this.config.disablePrinting;
+            },
             previousSnapshot() {
                 if (!this.currentSnapshotIndex) {
                     return null;
                 }
                 if (this.currentSnapshotIndex > 0) {
                     return this.snapshots[this.currentSnapshotIndex - 1];
                 }
@@ -2452,14 +2450,22 @@
                     window.location.href = this.config.prefix + ts + (ts ? "/" : "") + newUrl;
                 }
             },
             toggleTimelineView() {
                 this.showTimelineView = !this.showTimelineView;
                 window.localStorage.setItem("showTimelineView", this.showTimelineView ? "1" : "0");
             },
+            hasReplayFrame() {
+                return !!window.frames.replay_iframe;
+            },
+            printReplayFrame() {
+                window.frames.replay_iframe.contentWindow.focus();
+                window.frames.replay_iframe.contentWindow.print();
+                return false;
+            },
             setData( /** @type {PywbData} data */ data) {
 
                 // data-set will usually happen at App INIT (from parent caller)
                 this.$set(this, "snapshots", data.snapshots);
                 this.$set(this, "currentPeriod", data.timeline);
 
                 // get last-saved current period from previous page/app refresh (if there was such)
@@ -2737,14 +2743,40 @@
                                                 },
                                                 [_c("i", {
                                                     staticClass: "far fa-chart-bar"
                                                 })]
                                             )
                                         ]),
                                         _vm._v(" "),
+                                        _c("li", {
+                                            staticClass: "nav-item"
+                                        }, [
+                                            _vm.printingEnabled && _vm.hasReplayFrame() ?
+                                            _c(
+                                                "button", {
+                                                    staticClass: "btn btn-sm",
+                                                    class: {
+                                                        "btn-outline-light": _vm.lightButtons,
+                                                        "btn-outline-dark": !_vm.lightButtons
+                                                    },
+                                                    attrs: {
+                                                        "aria-pressed": _vm.printReplayFrame,
+                                                        title: _vm._("Print")
+                                                    },
+                                                    on: {
+                                                        click: _vm.printReplayFrame
+                                                    }
+                                                },
+                                                [_c("i", {
+                                                    staticClass: "fas fa-print"
+                                                })]
+                                            ) :
+                                            _vm._e()
+                                        ]),
+                                        _vm._v(" "),
                                         _vm.localesAreSet ?
                                         _c("li", {
                                             staticClass: "nav-item dropdown"
                                         }, [
                                             _c(
                                                 "button", {
                                                     staticClass: "btn btn-sm dropdown-toggle",
@@ -2976,23 +3008,23 @@
         }
     ];
     __vue_render__._withStripped = true;
 
     /* style */
     const __vue_inject_styles__ = function(inject) {
         if (!inject) return
-        inject("data-v-74a508dc_0", {
+        inject("data-v-3784da0a_0", {
             source: "\nbody {\n  padding-top: 89px !important;\n}\n.app {\n  font-family: Calibri, Arial, sans-serif;\n  /*border-bottom: 1px solid lightcoral;*/\n  width: 100%;\n}\n.app.expanded {\n  /*height: 130px;*/\n  max-height: calc(100vh - 90px);\n  display: flex;\n  flex-direction: column;\n}\n.full-view {\n  /*position: fixed;*/\n  /*top: 150px;*/\n  left: 0;\n}\n.navbar {\n  background-color: var(--navbar-background);\n  color:  var(--navbar-color);\n}\n.top-navbar {\n  z-index: 90;\n  padding: 2px 16px 0 16px;\n}\n.top-navbar span.navbar-toggler-icon {\n  margin: .25rem !important;\n}\n#logo-img {\n  max-height: 40px;\n}\n.title-nav {\n  margin-top: 50px;\n  z-index: 80;\n}\n#secondNavbar {\n  height: 24px !important;\n}\n#navbarCollapse {\n  justify-content: right;\n}\n#navbarCollapse ul#toggles {\n  display: flex;\n  align-content: center;\n}\n#navbarCollapse:not(.show) ul#toggles li:not(:first-child) {\n  margin-left: .25rem;\n}\n#navbarCollapse.show {\n  padding-bottom: 1em;\n}\n#navbarCollapse.show ul#toggles li {\n  margin-top: 5px;\n}\n#navbarCollapse.show ul#toggles li {\n  margin-left: 0px;\n}\n.iframe iframe {\n  width: 100%;\n  height: 80vh;\n}\n#searchdiv {\n  height: 31px;\n}\n#theurl {\n  width: 250px;\n}\n@media (min-width: 576px) {\n#theurl {\n    width: 350px;\n}\n}\n@media (min-width: 768px) {\n#theurl {\n    width: 500px;\n}\n}\n@media (min-width: 992px) {\n#theurl {\n    width: 600px;\n}\n}\n@media (min-width: 1200px) {\n#theurl {\n    width: 900px;\n}\n}\n#toggles {\n  align-items: center;\n}\n.breadcrumb-row {\n  display: flex;\n  align-items: center;\n  justify-content: center;\n}\ndiv.timeline-wrap div.card {\n  margin-top: 55px;\n}\n#calendar-card {\n  overflow-y: auto;\n  max-height: 100%;\n}\ndiv.timeline-wrap div.card-body {\n  display: flex;\n  align-items: center;\n  justify-content: center;\n}\ndiv.timeline-wrap div.card-body div.row {\n  width: 100%;\n  align-items: center;\n  justify-content: center;\n}\n#calendar-card-body {\n  padding: 0;\n}\n.strong {\n  font-weight: bold;\n}\n.hidden {\n  color: var(--navbar-background);\n}\n",
             map: {
                 "version": 3,
                 "sources": ["/Users/tessa/dev/pywb/pywb/vueui/src/App.vue"],
                 "names": [],
-                "mappings": ";AAgXA;EACA,4BAAA;AACA;AACA;EACA,uCAAA;EACA,uCAAA;EACA,WAAA;AACA;AACA;EACA,iBAAA;EACA,8BAAA;EACA,aAAA;EACA,sBAAA;AACA;AACA;EACA,mBAAA;EACA,cAAA;EACA,OAAA;AACA;AACA;EACA,0CAAA;EACA,2BAAA;AACA;AACA;EACA,WAAA;EACA,wBAAA;AACA;AACA;EACA,yBAAA;AACA;AACA;EACA,gBAAA;AACA;AACA;EACA,gBAAA;EACA,WAAA;AACA;AACA;EACA,uBAAA;AACA;AACA;EACA,sBAAA;AACA;AACA;EACA,aAAA;EACA,qBAAA;AACA;AACA;EACA,mBAAA;AACA;AACA;EACA,mBAAA;AACA;AACA;EACA,eAAA;AACA;AACA;EACA,gBAAA;AACA;AACA;EACA,WAAA;EACA,YAAA;AACA;AACA;EACA,YAAA;AACA;AACA;EACA,YAAA;AACA;AACA;AACA;IACA,YAAA;AACA;AACA;AACA;AACA;IACA,YAAA;AACA;AACA;AACA;AACA;IACA,YAAA;AACA;AACA;AACA;AACA;IACA,YAAA;AACA;AACA;AACA;EACA,mBAAA;AACA;AACA;EACA,aAAA;EACA,mBAAA;EACA,uBAAA;AACA;AACA;EACA,gBAAA;AACA;AACA;EACA,gBAAA;EACA,gBAAA;AACA;AACA;EACA,aAAA;EACA,mBAAA;EACA,uBAAA;AACA;AACA;EACA,WAAA;EACA,mBAAA;EACA,uBAAA;AACA;AAEA;EACA,UAAA;AACA;AACA;EACA,iBAAA;AACA;AACA;EACA,+BAAA;AACA",
+                "mappings": ";AAsYA;EACA,4BAAA;AACA;AACA;EACA,uCAAA;EACA,uCAAA;EACA,WAAA;AACA;AACA;EACA,iBAAA;EACA,8BAAA;EACA,aAAA;EACA,sBAAA;AACA;AACA;EACA,mBAAA;EACA,cAAA;EACA,OAAA;AACA;AACA;EACA,0CAAA;EACA,2BAAA;AACA;AACA;EACA,WAAA;EACA,wBAAA;AACA;AACA;EACA,yBAAA;AACA;AACA;EACA,gBAAA;AACA;AACA;EACA,gBAAA;EACA,WAAA;AACA;AACA;EACA,uBAAA;AACA;AACA;EACA,sBAAA;AACA;AACA;EACA,aAAA;EACA,qBAAA;AACA;AACA;EACA,mBAAA;AACA;AACA;EACA,mBAAA;AACA;AACA;EACA,eAAA;AACA;AACA;EACA,gBAAA;AACA;AACA;EACA,WAAA;EACA,YAAA;AACA;AACA;EACA,YAAA;AACA;AACA;EACA,YAAA;AACA;AACA;AACA;IACA,YAAA;AACA;AACA;AACA;AACA;IACA,YAAA;AACA;AACA;AACA;AACA;IACA,YAAA;AACA;AACA;AACA;AACA;IACA,YAAA;AACA;AACA;AACA;EACA,mBAAA;AACA;AACA;EACA,aAAA;EACA,mBAAA;EACA,uBAAA;AACA;AACA;EACA,gBAAA;AACA;AACA;EACA,gBAAA;EACA,gBAAA;AACA;AACA;EACA,aAAA;EACA,mBAAA;EACA,uBAAA;AACA;AACA;EACA,WAAA;EACA,mBAAA;EACA,uBAAA;AACA;AAEA;EACA,UAAA;AACA;AACA;EACA,iBAAA;AACA;AACA;EACA,+BAAA;AACA",
                 "file": "App.vue",
-                "sourcesContent": ["<template>\n  <div class=\"app\" :class=\"{expanded: showTimelineView || showFullView }\" data-app=\"webrecorder-replay-app\">\n    <!-- Top navbar -->\n    <nav\n      class=\"navbar navbar-light navbar-expand-lg fixed-top top-navbar justify-content-center\"\n      :style=\"navbarStyle\">\n      <a class=\"navbar-brand flex-grow-1 my-1\" :href=\"config.logoHomeUrl\" v-if=\"config.logoHomeUrl\">\n        <img :src=\"config.logoImg\" id=\"logo-img\" alt=\"_('pywb logo')\">\n      </a>\n      <div class=\"navbar-brand flex-grow-1 my-1\" v-else>\n        <img :src=\"config.logoImg\" id=\"logo-img\" alt=\"_('pywb logo')\">\n      </div>\n      <div class=\"flex-grow-1 d-flex\" id=\"searchdiv\">\n        <form\n          class=\"form-inline my-2 my-md-0 mx-lg-auto\"\n          role=\"search\"\n          @submit=\"gotoUrl\">\n          <input\n            id=\"theurl\"\n            type=\"text\"\n            :value=\"config.url\"\n            height=\"31\"\n            aria-label=\"_('Search for archival capture of URL')\"\n            title=\"_('Search for archival capture of URL')\"></input>\n        </form>\n      </div>\n      <button\n        class=\"navbar-toggler btn btn-sm\"\n        id=\"collapse-button\"\n        type=\"button\"\n        data-toggle=\"collapse\"\n        data-target=\"#navbarCollapse\"\n        aria-controls=\"navbarCollapse\"\n        aria-expanded=\"false\"\n        aria-label=\"_('Toggle navigation')\">\n        <span class=\"navbar-toggler-icon\"></span>\n      </button>\n      <div class=\"collapse navbar-collapse ml-auto\" id=\"navbarCollapse\">\n        <ul class=\"navbar-nav ml-3\" id=\"toggles\">\n          <li class=\"nav-item\">\n            <button\n              class=\"btn btn-sm\"\n              :class=\"{active: showFullView, 'btn-outline-light': lightButtons, 'btn-outline-dark': !lightButtons}\"\n              :title=\"_('Previous capture')\"\n              v-if=\"previousSnapshot\"\n              @click=\"gotoPreviousSnapshot\">\n              <i class=\"fas fa-arrow-left\" :title=\"_('Previous capture')\"></i>\n            </button>\n          </li>\n          <li class=\"nav-item\">\n            <button\n              class=\"btn btn-sm\"\n              :class=\"{active: showFullView, 'btn-outline-light': lightButtons, 'btn-outline-dark': !lightButtons}\"\n              :title=\"_('Next capture')\"\n              v-if=\"nextSnapshot\"\n              @click=\"gotoNextSnapshot\">\n              <i class=\"fas fa-arrow-right\" :title=\"_('Next capture')\"></i>\n            </button>\n          </li>\n          <li class=\"nav-item active\">\n            <button\n              class=\"btn btn-sm\"\n              :class=\"{active: showFullView, 'btn-outline-light': lightButtons, 'btn-outline-dark': !lightButtons}\"\n              :aria-pressed=\"(showFullView ? true : false)\"\n              @click=\"showFullView = !showFullView\"\n              :title=\"(showFullView ? _('Hide calendar') : _('Show calendar'))\">\n              <i class=\"far fa-calendar-alt\"></i>\n            </button>\n          </li>\n          <li class=\"nav-item\">\n            <button\n              class=\"btn btn-sm\"\n              :class=\"{active: showTimelineView, 'btn-outline-light': lightButtons, 'btn-outline-dark': !lightButtons}\"\n              :aria-pressed=\"showTimelineView\"\n              @click=\"toggleTimelineView\"\n              :title=\"(showTimelineView ? _('Hide timeline') : _('Show timeline'))\">\n              <i class=\"far fa-chart-bar\"></i>\n            </button>\n          </li>\n          <li class=\"nav-item dropdown\" v-if=\"localesAreSet\">\n            <button\n              class=\"btn btn-sm dropdown-toggle\"\n              :class=\"{'btn-outline-light': lightButtons, 'btn-outline-dark': !lightButtons}\"\n              type=\"button\"\n              id=\"locale-dropdown\"\n              data-toggle=\"dropdown\"\n              aria-haspopup=\"true\"\n              aria-expanded=\"false\"\n              :title=\"_('Select language')\">\n              <i class=\"fas fa-globe-africa\" :title=\"_('Language')\"></i>\n            </button>\n            <div class=\"dropdown-menu dropdown-menu-right\" aria-labelledby=\"locale-dropdown\">\n              <a\n                class=\"dropdown-item\"\n                v-for=\"(locPath, key) in config.allLocales\"\n                :key=\"key\"\n                :href=\"locPath + (currentSnapshot ? currentSnapshot.id : '*') + '/' + config.url\">\n                {{ key }}\n              </a>\n            </div>\n          </li>\n        </ul>\n      </div>\n    </nav>\n\n    <!-- Capture title and date -->\n    <nav\n      class=\"navbar navbar-light justify-content-center title-nav fixed-top\"\n      id=\"second-navbar\"\n      :style=\"navbarStyle\">\n      <span class=\"hidden\" v-if=\"!currentSnapshot\">&nbsp;</span>\n      <span v-if=\"currentSnapshot\">\n        <span class=\"strong mr-1\">\n          {{_('Current Capture')}}: \n          <span class=\"ml-1\" v-if=\"config.title\">\n            {{ config.title }}\n          </span>\n        </span>\n        <span class=\"mr-1\" v-if=\"config.title\">|</span>\n        {{currentSnapshot.getTimeDateFormatted()}}\n      </span>\n    </nav>\n\n    <!-- Timeline -->\n    <div class=\"card border-top-0 border-left-0 border-right-0 timeline-wrap\">\n      <div class=\"card-body\" v-if=\"currentPeriod && showTimelineView\">\n        <div class=\"row\">\n          <div class=\"col col-12\">\n            <TimelineBreadcrumbs\n              :period=\"currentPeriod\"\n              @goto-period=\"gotoPeriod\"\n            ></TimelineBreadcrumbs>\n          </div>\n          <div class=\"col col-12 mt-2\">\n            <Timeline\n              :period=\"currentPeriod\"\n              :highlight=\"timelineHighlight\"\n              :current-snapshot=\"currentSnapshot\"\n              :max-zoom-level=\"maxTimelineZoomLevel\"\n              @goto-period=\"gotoPeriod\"\n            ></Timeline>\n          </div>\n        </div>\n      </div>    \n    </div>\n\n    <!-- Calendar -->\n    <div class=\"card\" id=\"calendar-card\" v-if=\"currentPeriod && showFullView && currentPeriod.children.length\">\n      <div class=\"card-body\" id=\"calendar-card-body\">\n        <CalendarYear\n          :period=\"currentPeriod\"\n          :current-snapshot=\"currentSnapshot\"\n           @goto-period=\"gotoPeriod\">\n        </CalendarYear>\n      </div>\n    </div>\n    \n  </div>\n</template>\n\n<script>\nimport Timeline from \"./components/Timeline.vue\";\nimport TimelineBreadcrumbs from \"./components/TimelineBreadcrumbs.vue\";\nimport CalendarYear from \"./components/CalendarYear.vue\";\n\nimport { PywbSnapshot, PywbPeriod } from \"./model.js\";\nimport {PywbI18N} from \"./i18n\";\n\nexport default {\n  name: \"PywbReplayApp\",\n  //el: '[data-app=\"webrecorder-replay-app\"]',\n  data: function() {\n    return {\n      snapshots: [],\n      currentPeriod: null,\n      currentSnapshot: null,\n      currentSnapshotIndex: null,\n      msgs: [],\n      showFullView: false,\n      showTimelineView: false,\n      maxTimelineZoomLevel: PywbPeriod.Type.day,\n      config: {\n        title: \"\",\n        initialView: {},\n        allLocales: {}\n      },\n      timelineHighlight: false,\n      locales: [],\n    };\n  },\n  components: {Timeline, TimelineBreadcrumbs, CalendarYear},\n  mounted: function() {\n    // add empty unload event listener to make this page bfcache ineligible.\n    // bfcache otherwises prevent the query template from reloading as expected\n    // when the user navigates there via browser back/forward buttons\n    addEventListener('unload', (event) => { });\n  },\n  updated: function() {\n    // set top frame title equal to value pulled from replay frame\n    document.title = this._(\"Archived Page: \") + this.config.title;\n  },\n  computed: {\n    sessionStorageUrlKey() {\n      // remove http(s), www and trailing slash\n      return 'zoom__' + this.config.url.replace(/^https?:\\/\\/(www\\.)?/, '').replace(/\\/$/, '');\n    },\n    localesAreSet() {\n      return Object.entries(this.config.allLocales).length > 0;\n    },\n    navbarStyle() {\n      return {\n        '--navbar-background': `#${this.config.navbarBackground}`,\n        '--navbar-color': `#${this.config.navbarColor}`\n      }\n    },\n    lightButtons() {\n      return !!this.config.navbarLightButtons;\n    },\n    previousSnapshot() {\n      if (!this.currentSnapshotIndex) {\n        return null;\n      }\n      if (this.currentSnapshotIndex > 0) {\n        return this.snapshots[this.currentSnapshotIndex - 1];\n      }\n      return null;\n    },\n    nextSnapshot() {\n      if (this.currentSnapshotIndex == null) {\n        return null;\n      }\n      if (\n        (this.currentSnapshotIndex >= 0)\n        && (this.currentSnapshotIndex !== this.snapshots.length - 1)) {\n        return this.snapshots[this.currentSnapshotIndex + 1];\n      }\n      return null;\n    }\n  },\n  methods: {\n    _(id, embeddedVariableStrings=null) {\n      return PywbI18N.instance.getText(id, embeddedVariableStrings);\n    },\n    gotoPeriod: function(newPeriod, onlyZoomToPeriod) {\n      if (this.timelineHighlight) {\n        setTimeout((() => {\n          this.timelineHighlight=false;\n        }).bind(this), 3000);\n      }\n      // only go to snapshot if caller did not request to zoom only\n      if (newPeriod.snapshot && !onlyZoomToPeriod) {\n        this.gotoSnapshot(newPeriod.snapshot, newPeriod, true /* reloadIFrame */);\n      } else {\n        // save current period (aka zoom)\n        // use sessionStorage (not localStorage), as we want this to be a very temporary memory for current page tab/window and no longer; NOTE: it serves when navigating from an \"*\" query to a specific capture and subsequent reloads\n        if (window.sessionStorage) {\n          window.sessionStorage.setItem(this.sessionStorageUrlKey, newPeriod.fullId);\n        }\n        // If new period goes beyond allowed max level\n        if (newPeriod.type > this.maxTimelineZoomLevel) {\n          this.currentPeriod = newPeriod.get(this.maxTimelineZoomLevel);\n        } else {\n          this.currentPeriod = newPeriod;\n        }\n      }\n    },\n    gotoSnapshot(snapshot, fromPeriod, reloadIFrame=false) {\n      this.currentSnapshot = snapshot;\n\n      const isCurrentSnapshot = (snapshotInArray) => snapshotInArray.id == snapshot.id && snapshotInArray.url == snapshot.url;\n      this.currentSnapshotIndex = this.snapshots.findIndex(isCurrentSnapshot);\n\n      // if the current period doesn't match the current snapshot, update it\n      if (!this.currentPeriod || (fromPeriod && !this.currentPeriod.contains(fromPeriod))) {\n        const fromPeriodAtMaxZoomLevel = fromPeriod.get(this.maxTimelineZoomLevel);\n        if (!this.currentPeriod || fromPeriodAtMaxZoomLevel !== this.currentPeriod) {\n          this.currentPeriod = fromPeriodAtMaxZoomLevel;\n        }\n      }\n\n      // update iframe only if the snapshot was selected from the calendar/timeline.\n      // if the change originated from a user clicking a link in the iframe, emitting\n      // snow-shapshot will only cause a flash of content\n      if (reloadIFrame !== false) {\n        this.$emit(\"show-snapshot\", snapshot);\n      }\n      this.initBannerState(true);\n    },\n    gotoPreviousSnapshot() {\n      let periodToChangeTo = this.currentPeriod.findByFullId(this.previousSnapshot.getFullId());\n      this.gotoPeriod(periodToChangeTo, false /* onlyZoomToPeriod */);\n    },\n    gotoNextSnapshot() {\n      let periodToChangeTo = this.currentPeriod.findByFullId(this.nextSnapshot.getFullId());\n      this.gotoPeriod(periodToChangeTo, false /* onlyZoomToPeriod */);\n    },\n    gotoUrl(event) {\n      event.preventDefault();\n      const newUrl = document.querySelector(\"#theurl\").value;\n      if (newUrl !== this.config.url) {\n        const ts = this.config.timestamp === undefined ? \"*\" : this.config.timestamp;\n        window.location.href = this.config.prefix + ts + (ts ? \"/\" : \"\") + newUrl;\n      }\n    },\n    toggleTimelineView() {\n      this.showTimelineView = !this.showTimelineView;\n      window.localStorage.setItem(\"showTimelineView\", this.showTimelineView ? \"1\" : \"0\");\n    },\n    setData(/** @type {PywbData} data */ data) {\n\n      // data-set will usually happen at App INIT (from parent caller)\n      this.$set(this, \"snapshots\", data.snapshots);\n      this.$set(this, \"currentPeriod\", data.timeline);\n\n      // get last-saved current period from previous page/app refresh (if there was such)\n      if (window.sessionStorage) {\n        const currentPeriodId = window.sessionStorage.getItem(this.sessionStorageUrlKey);\n        if (currentPeriodId) {\n          const newCurrentPeriodFromStorage = this.currentPeriod.findByFullId(currentPeriodId);\n          if (newCurrentPeriodFromStorage) {\n            this.currentPeriod = newCurrentPeriodFromStorage;\n          }\n        }\n      }\n\n      // signal app is DONE setting and rendering data; ON NEXT TICK\n      this.$nextTick(function isDone() {\n        this.$emit('data-set-and-render-completed');\n      }.bind(this));\n    },\n    setSnapshot(view) {\n      if (!this.currentPeriod) {\n        return false;\n      }\n\n      // turn off calendar (aka full) view\n      this.showFullView = false;\n\n      // convert to snapshot object to support proper rendering of time/date\n      const snapshot = new PywbSnapshot(view, 0);\n\n      this.config.url = view.url;\n\n      let periodToChangeTo = this.currentPeriod.findByFullId(snapshot.getFullId());\n      if (periodToChangeTo) {\n        this.gotoPeriod(periodToChangeTo, false /* onlyZoomToPeriod */);\n        return true;\n      }\n      return false;\n    },\n    initBannerState(isReplay) {\n      // if not replay, always show both\n      if (!isReplay) {\n        this.showFullView = true;\n        this.showTimelineView = true;\n      } else {\n        this.showFullView = false;\n        this.showTimelineView = window.localStorage.getItem(\"showTimelineView\") === \"1\";\n      }\n    },\n    updateTitle(title) {\n      this.config.title = title;\n    }\n  }\n};\n</script>\n\n<style>\n  body {\n    padding-top: 89px !important;\n  }\n  .app {\n    font-family: Calibri, Arial, sans-serif;\n    /*border-bottom: 1px solid lightcoral;*/\n    width: 100%;\n  }\n  .app.expanded {\n    /*height: 130px;*/\n    max-height: calc(100vh - 90px);\n    display: flex;\n    flex-direction: column;\n  }\n  .full-view {\n    /*position: fixed;*/\n    /*top: 150px;*/\n    left: 0;\n  }\n  .navbar {\n    background-color: var(--navbar-background);\n    color:  var(--navbar-color);\n  }\n  .top-navbar {\n    z-index: 90;\n    padding: 2px 16px 0 16px;\n  }\n  .top-navbar span.navbar-toggler-icon {\n    margin: .25rem !important;\n  }\n  #logo-img {\n    max-height: 40px;\n  }\n  .title-nav {\n    margin-top: 50px;\n    z-index: 80;\n  }\n  #secondNavbar {\n    height: 24px !important;\n  }\n  #navbarCollapse {\n    justify-content: right;\n  }\n  #navbarCollapse ul#toggles {\n    display: flex;\n    align-content: center;\n  }\n  #navbarCollapse:not(.show) ul#toggles li:not(:first-child) {\n    margin-left: .25rem;\n  }\n  #navbarCollapse.show {\n    padding-bottom: 1em;\n  }\n  #navbarCollapse.show ul#toggles li {\n    margin-top: 5px;\n  }\n  #navbarCollapse.show ul#toggles li {\n    margin-left: 0px;\n  }\n  .iframe iframe {\n    width: 100%;\n    height: 80vh;\n  }\n  #searchdiv {\n    height: 31px;\n  }\n  #theurl {\n    width: 250px;\n  }\n  @media (min-width: 576px) {\n    #theurl {\n      width: 350px;\n    }\n  }\n  @media (min-width: 768px) {\n    #theurl {\n      width: 500px;\n    }\n  }\n  @media (min-width: 992px) {\n    #theurl {\n      width: 600px;\n    }\n  }\n  @media (min-width: 1200px) {\n    #theurl {\n      width: 900px;\n    }\n  }\n  #toggles {\n    align-items: center;\n  }\n  .breadcrumb-row {\n    display: flex;\n    align-items: center;\n    justify-content: center;\n  }\n  div.timeline-wrap div.card {\n    margin-top: 55px;\n  }\n  #calendar-card {\n    overflow-y: auto;\n    max-height: 100%;\n  }\n  div.timeline-wrap div.card-body {\n    display: flex;\n    align-items: center;\n    justify-content: center;\n  }\n  div.timeline-wrap div.card-body div.row {\n    width: 100%;\n    align-items: center;\n    justify-content: center;\n  }\n\n  #calendar-card-body {\n    padding: 0;\n  }\n  .strong {\n    font-weight: bold;\n  }\n  .hidden {\n    color: var(--navbar-background);\n  }\n</style>\n"]
+                "sourcesContent": ["<template>\n  <div class=\"app\" :class=\"{expanded: showTimelineView || showFullView }\" data-app=\"webrecorder-replay-app\">\n    <!-- Top navbar -->\n    <nav\n      class=\"navbar navbar-light navbar-expand-lg fixed-top top-navbar justify-content-center\"\n      :style=\"navbarStyle\">\n      <a class=\"navbar-brand flex-grow-1 my-1\" :href=\"config.logoHomeUrl\" v-if=\"config.logoHomeUrl\">\n        <img :src=\"config.logoImg\" id=\"logo-img\" alt=\"_('pywb logo')\">\n      </a>\n      <div class=\"navbar-brand flex-grow-1 my-1\" v-else>\n        <img :src=\"config.logoImg\" id=\"logo-img\" alt=\"_('pywb logo')\">\n      </div>\n      <div class=\"flex-grow-1 d-flex\" id=\"searchdiv\">\n        <form\n          class=\"form-inline my-2 my-md-0 mx-lg-auto\"\n          role=\"search\"\n          @submit=\"gotoUrl\">\n          <input\n            id=\"theurl\"\n            type=\"text\"\n            :value=\"config.url\"\n            height=\"31\"\n            aria-label=\"_('Search for archival capture of URL')\"\n            title=\"_('Search for archival capture of URL')\"></input>\n        </form>\n      </div>\n      <button\n        class=\"navbar-toggler btn btn-sm\"\n        id=\"collapse-button\"\n        type=\"button\"\n        data-toggle=\"collapse\"\n        data-target=\"#navbarCollapse\"\n        aria-controls=\"navbarCollapse\"\n        aria-expanded=\"false\"\n        aria-label=\"_('Toggle navigation')\">\n        <span class=\"navbar-toggler-icon\"></span>\n      </button>\n      <div class=\"collapse navbar-collapse ml-auto\" id=\"navbarCollapse\">\n        <ul class=\"navbar-nav ml-3\" id=\"toggles\">\n          <li class=\"nav-item\">\n            <button\n              class=\"btn btn-sm\"\n              :class=\"{active: showFullView, 'btn-outline-light': lightButtons, 'btn-outline-dark': !lightButtons}\"\n              :title=\"_('Previous capture')\"\n              v-if=\"previousSnapshot\"\n              @click=\"gotoPreviousSnapshot\">\n              <i class=\"fas fa-arrow-left\" :title=\"_('Previous capture')\"></i>\n            </button>\n          </li>\n          <li class=\"nav-item\">\n            <button\n              class=\"btn btn-sm\"\n              :class=\"{active: showFullView, 'btn-outline-light': lightButtons, 'btn-outline-dark': !lightButtons}\"\n              :title=\"_('Next capture')\"\n              v-if=\"nextSnapshot\"\n              @click=\"gotoNextSnapshot\">\n              <i class=\"fas fa-arrow-right\" :title=\"_('Next capture')\"></i>\n            </button>\n          </li>\n          <li class=\"nav-item active\">\n            <button\n              class=\"btn btn-sm\"\n              :class=\"{active: showFullView, 'btn-outline-light': lightButtons, 'btn-outline-dark': !lightButtons}\"\n              :aria-pressed=\"(showFullView ? true : false)\"\n              @click=\"showFullView = !showFullView\"\n              :title=\"(showFullView ? _('Hide calendar') : _('Show calendar'))\">\n              <i class=\"far fa-calendar-alt\"></i>\n            </button>\n          </li>\n          <li class=\"nav-item\">\n            <button\n              class=\"btn btn-sm\"\n              :class=\"{active: showTimelineView, 'btn-outline-light': lightButtons, 'btn-outline-dark': !lightButtons}\"\n              :aria-pressed=\"showTimelineView\"\n              @click=\"toggleTimelineView\"\n              :title=\"(showTimelineView ? _('Hide timeline') : _('Show timeline'))\">\n              <i class=\"far fa-chart-bar\"></i>\n            </button>\n          </li>\n          <li class=\"nav-item\">\n            <button\n              class=\"btn btn-sm\"\n              :class=\"{'btn-outline-light': lightButtons, 'btn-outline-dark': !lightButtons}\"\n              :aria-pressed=\"printReplayFrame\"\n              @click=\"printReplayFrame\"\n              v-if=\"printingEnabled && hasReplayFrame()\"\n              :title=\"_('Print')\">\n              <i class=\"fas fa-print\"></i>\n            </button>\n          </li>\n          <li class=\"nav-item dropdown\" v-if=\"localesAreSet\">\n            <button\n              class=\"btn btn-sm dropdown-toggle\"\n              :class=\"{'btn-outline-light': lightButtons, 'btn-outline-dark': !lightButtons}\"\n              type=\"button\"\n              id=\"locale-dropdown\"\n              data-toggle=\"dropdown\"\n              aria-haspopup=\"true\"\n              aria-expanded=\"false\"\n              :title=\"_('Select language')\">\n              <i class=\"fas fa-globe-africa\" :title=\"_('Language')\"></i>\n            </button>\n            <div class=\"dropdown-menu dropdown-menu-right\" aria-labelledby=\"locale-dropdown\">\n              <a\n                class=\"dropdown-item\"\n                v-for=\"(locPath, key) in config.allLocales\"\n                :key=\"key\"\n                :href=\"locPath + (currentSnapshot ? currentSnapshot.id : '*') + '/' + config.url\">\n                {{ key }}\n              </a>\n            </div>\n          </li>\n        </ul>\n      </div>\n    </nav>\n\n    <!-- Capture title and date -->\n    <nav\n      class=\"navbar navbar-light justify-content-center title-nav fixed-top\"\n      id=\"second-navbar\"\n      :style=\"navbarStyle\">\n      <span class=\"hidden\" v-if=\"!currentSnapshot\">&nbsp;</span>\n      <span v-if=\"currentSnapshot\">\n        <span class=\"strong mr-1\">\n          {{_('Current Capture')}}: \n          <span class=\"ml-1\" v-if=\"config.title\">\n            {{ config.title }}\n          </span>\n        </span>\n        <span class=\"mr-1\" v-if=\"config.title\">|</span>\n        {{currentSnapshot.getTimeDateFormatted()}}\n      </span>\n    </nav>\n\n    <!-- Timeline -->\n    <div class=\"card border-top-0 border-left-0 border-right-0 timeline-wrap\">\n      <div class=\"card-body\" v-if=\"currentPeriod && showTimelineView\">\n        <div class=\"row\">\n          <div class=\"col col-12\">\n            <TimelineBreadcrumbs\n              :period=\"currentPeriod\"\n              @goto-period=\"gotoPeriod\"\n            ></TimelineBreadcrumbs>\n          </div>\n          <div class=\"col col-12 mt-2\">\n            <Timeline\n              :period=\"currentPeriod\"\n              :highlight=\"timelineHighlight\"\n              :current-snapshot=\"currentSnapshot\"\n              :max-zoom-level=\"maxTimelineZoomLevel\"\n              @goto-period=\"gotoPeriod\"\n            ></Timeline>\n          </div>\n        </div>\n      </div>    \n    </div>\n\n    <!-- Calendar -->\n    <div class=\"card\" id=\"calendar-card\" v-if=\"currentPeriod && showFullView && currentPeriod.children.length\">\n      <div class=\"card-body\" id=\"calendar-card-body\">\n        <CalendarYear\n          :period=\"currentPeriod\"\n          :current-snapshot=\"currentSnapshot\"\n           @goto-period=\"gotoPeriod\">\n        </CalendarYear>\n      </div>\n    </div>\n    \n  </div>\n</template>\n\n<script>\nimport Timeline from \"./components/Timeline.vue\";\nimport TimelineBreadcrumbs from \"./components/TimelineBreadcrumbs.vue\";\nimport CalendarYear from \"./components/CalendarYear.vue\";\n\nimport { PywbSnapshot, PywbPeriod } from \"./model.js\";\nimport {PywbI18N} from \"./i18n\";\n\nexport default {\n  name: \"PywbReplayApp\",\n  //el: '[data-app=\"webrecorder-replay-app\"]',\n  data: function() {\n    return {\n      snapshots: [],\n      currentPeriod: null,\n      currentSnapshot: null,\n      currentSnapshotIndex: null,\n      msgs: [],\n      showFullView: false,\n      showTimelineView: false,\n      maxTimelineZoomLevel: PywbPeriod.Type.day,\n      config: {\n        title: \"\",\n        initialView: {},\n        allLocales: {}\n      },\n      timelineHighlight: false,\n      locales: [],\n    };\n  },\n  components: {Timeline, TimelineBreadcrumbs, CalendarYear},\n  mounted: function() {\n    // add empty unload event listener to make this page bfcache ineligible.\n    // bfcache otherwises prevent the query template from reloading as expected\n    // when the user navigates there via browser back/forward buttons\n    addEventListener('unload', (event) => { });\n  },\n  updated: function() {\n    // set top frame title equal to value pulled from replay frame\n    document.title = this._(\"Archived Page: \") + this.config.title;\n  },\n  computed: {\n    sessionStorageUrlKey() {\n      // remove http(s), www and trailing slash\n      return 'zoom__' + this.config.url.replace(/^https?:\\/\\/(www\\.)?/, '').replace(/\\/$/, '');\n    },\n    localesAreSet() {\n      return Object.entries(this.config.allLocales).length > 0;\n    },\n    navbarStyle() {\n      return {\n        '--navbar-background': `#${this.config.navbarBackground}`,\n        '--navbar-color': `#${this.config.navbarColor}`\n      }\n    },\n    lightButtons() {\n      return !!this.config.navbarLightButtons;\n    },\n    printingEnabled() {\n      return !this.config.disablePrinting;\n    },\n    previousSnapshot() {\n      if (!this.currentSnapshotIndex) {\n        return null;\n      }\n      if (this.currentSnapshotIndex > 0) {\n        return this.snapshots[this.currentSnapshotIndex - 1];\n      }\n      return null;\n    },\n    nextSnapshot() {\n      if (this.currentSnapshotIndex == null) {\n        return null;\n      }\n      if (\n        (this.currentSnapshotIndex >= 0)\n        && (this.currentSnapshotIndex !== this.snapshots.length - 1)) {\n        return this.snapshots[this.currentSnapshotIndex + 1];\n      }\n      return null;\n    }\n  },\n  methods: {\n    _(id, embeddedVariableStrings=null) {\n      return PywbI18N.instance.getText(id, embeddedVariableStrings);\n    },\n    gotoPeriod: function(newPeriod, onlyZoomToPeriod) {\n      if (this.timelineHighlight) {\n        setTimeout((() => {\n          this.timelineHighlight=false;\n        }).bind(this), 3000);\n      }\n      // only go to snapshot if caller did not request to zoom only\n      if (newPeriod.snapshot && !onlyZoomToPeriod) {\n        this.gotoSnapshot(newPeriod.snapshot, newPeriod, true /* reloadIFrame */);\n      } else {\n        // save current period (aka zoom)\n        // use sessionStorage (not localStorage), as we want this to be a very temporary memory for current page tab/window and no longer; NOTE: it serves when navigating from an \"*\" query to a specific capture and subsequent reloads\n        if (window.sessionStorage) {\n          window.sessionStorage.setItem(this.sessionStorageUrlKey, newPeriod.fullId);\n        }\n        // If new period goes beyond allowed max level\n        if (newPeriod.type > this.maxTimelineZoomLevel) {\n          this.currentPeriod = newPeriod.get(this.maxTimelineZoomLevel);\n        } else {\n          this.currentPeriod = newPeriod;\n        }\n      }\n    },\n    gotoSnapshot(snapshot, fromPeriod, reloadIFrame=false) {\n      this.currentSnapshot = snapshot;\n\n      const isCurrentSnapshot = (snapshotInArray) => snapshotInArray.id == snapshot.id && snapshotInArray.url == snapshot.url;\n      this.currentSnapshotIndex = this.snapshots.findIndex(isCurrentSnapshot);\n\n      // if the current period doesn't match the current snapshot, update it\n      if (!this.currentPeriod || (fromPeriod && !this.currentPeriod.contains(fromPeriod))) {\n        const fromPeriodAtMaxZoomLevel = fromPeriod.get(this.maxTimelineZoomLevel);\n        if (!this.currentPeriod || fromPeriodAtMaxZoomLevel !== this.currentPeriod) {\n          this.currentPeriod = fromPeriodAtMaxZoomLevel;\n        }\n      }\n\n      // update iframe only if the snapshot was selected from the calendar/timeline.\n      // if the change originated from a user clicking a link in the iframe, emitting\n      // snow-shapshot will only cause a flash of content\n      if (reloadIFrame !== false) {\n        this.$emit(\"show-snapshot\", snapshot);\n      }\n      this.initBannerState(true);\n    },\n    gotoPreviousSnapshot() {\n      let periodToChangeTo = this.currentPeriod.findByFullId(this.previousSnapshot.getFullId());\n      this.gotoPeriod(periodToChangeTo, false /* onlyZoomToPeriod */);\n    },\n    gotoNextSnapshot() {\n      let periodToChangeTo = this.currentPeriod.findByFullId(this.nextSnapshot.getFullId());\n      this.gotoPeriod(periodToChangeTo, false /* onlyZoomToPeriod */);\n    },\n    gotoUrl(event) {\n      event.preventDefault();\n      const newUrl = document.querySelector(\"#theurl\").value;\n      if (newUrl !== this.config.url) {\n        const ts = this.config.timestamp === undefined ? \"*\" : this.config.timestamp;\n        window.location.href = this.config.prefix + ts + (ts ? \"/\" : \"\") + newUrl;\n      }\n    },\n    toggleTimelineView() {\n      this.showTimelineView = !this.showTimelineView;\n      window.localStorage.setItem(\"showTimelineView\", this.showTimelineView ? \"1\" : \"0\");\n    },\n    hasReplayFrame() {\n      return !! window.frames.replay_iframe;\n    },\n    printReplayFrame() {\n      window.frames.replay_iframe.contentWindow.focus();\n      window.frames.replay_iframe.contentWindow.print();\n      return false;\n    },\n    setData(/** @type {PywbData} data */ data) {\n\n      // data-set will usually happen at App INIT (from parent caller)\n      this.$set(this, \"snapshots\", data.snapshots);\n      this.$set(this, \"currentPeriod\", data.timeline);\n\n      // get last-saved current period from previous page/app refresh (if there was such)\n      if (window.sessionStorage) {\n        const currentPeriodId = window.sessionStorage.getItem(this.sessionStorageUrlKey);\n        if (currentPeriodId) {\n          const newCurrentPeriodFromStorage = this.currentPeriod.findByFullId(currentPeriodId);\n          if (newCurrentPeriodFromStorage) {\n            this.currentPeriod = newCurrentPeriodFromStorage;\n          }\n        }\n      }\n\n      // signal app is DONE setting and rendering data; ON NEXT TICK\n      this.$nextTick(function isDone() {\n        this.$emit('data-set-and-render-completed');\n      }.bind(this));\n    },\n    setSnapshot(view) {\n      if (!this.currentPeriod) {\n        return false;\n      }\n\n      // turn off calendar (aka full) view\n      this.showFullView = false;\n\n      // convert to snapshot object to support proper rendering of time/date\n      const snapshot = new PywbSnapshot(view, 0);\n\n      this.config.url = view.url;\n\n      let periodToChangeTo = this.currentPeriod.findByFullId(snapshot.getFullId());\n      if (periodToChangeTo) {\n        this.gotoPeriod(periodToChangeTo, false /* onlyZoomToPeriod */);\n        return true;\n      }\n      return false;\n    },\n    initBannerState(isReplay) {\n      // if not replay, always show both\n      if (!isReplay) {\n        this.showFullView = true;\n        this.showTimelineView = true;\n      } else {\n        this.showFullView = false;\n        this.showTimelineView = window.localStorage.getItem(\"showTimelineView\") === \"1\";\n      }\n    },\n    updateTitle(title) {\n      this.config.title = title;\n    }\n  }\n};\n</script>\n\n<style>\n  body {\n    padding-top: 89px !important;\n  }\n  .app {\n    font-family: Calibri, Arial, sans-serif;\n    /*border-bottom: 1px solid lightcoral;*/\n    width: 100%;\n  }\n  .app.expanded {\n    /*height: 130px;*/\n    max-height: calc(100vh - 90px);\n    display: flex;\n    flex-direction: column;\n  }\n  .full-view {\n    /*position: fixed;*/\n    /*top: 150px;*/\n    left: 0;\n  }\n  .navbar {\n    background-color: var(--navbar-background);\n    color:  var(--navbar-color);\n  }\n  .top-navbar {\n    z-index: 90;\n    padding: 2px 16px 0 16px;\n  }\n  .top-navbar span.navbar-toggler-icon {\n    margin: .25rem !important;\n  }\n  #logo-img {\n    max-height: 40px;\n  }\n  .title-nav {\n    margin-top: 50px;\n    z-index: 80;\n  }\n  #secondNavbar {\n    height: 24px !important;\n  }\n  #navbarCollapse {\n    justify-content: right;\n  }\n  #navbarCollapse ul#toggles {\n    display: flex;\n    align-content: center;\n  }\n  #navbarCollapse:not(.show) ul#toggles li:not(:first-child) {\n    margin-left: .25rem;\n  }\n  #navbarCollapse.show {\n    padding-bottom: 1em;\n  }\n  #navbarCollapse.show ul#toggles li {\n    margin-top: 5px;\n  }\n  #navbarCollapse.show ul#toggles li {\n    margin-left: 0px;\n  }\n  .iframe iframe {\n    width: 100%;\n    height: 80vh;\n  }\n  #searchdiv {\n    height: 31px;\n  }\n  #theurl {\n    width: 250px;\n  }\n  @media (min-width: 576px) {\n    #theurl {\n      width: 350px;\n    }\n  }\n  @media (min-width: 768px) {\n    #theurl {\n      width: 500px;\n    }\n  }\n  @media (min-width: 992px) {\n    #theurl {\n      width: 600px;\n    }\n  }\n  @media (min-width: 1200px) {\n    #theurl {\n      width: 900px;\n    }\n  }\n  #toggles {\n    align-items: center;\n  }\n  .breadcrumb-row {\n    display: flex;\n    align-items: center;\n    justify-content: center;\n  }\n  div.timeline-wrap div.card {\n    margin-top: 55px;\n  }\n  #calendar-card {\n    overflow-y: auto;\n    max-height: 100%;\n  }\n  div.timeline-wrap div.card-body {\n    display: flex;\n    align-items: center;\n    justify-content: center;\n  }\n  div.timeline-wrap div.card-body div.row {\n    width: 100%;\n    align-items: center;\n    justify-content: center;\n  }\n\n  #calendar-card-body {\n    padding: 0;\n  }\n  .strong {\n    font-weight: bold;\n  }\n  .hidden {\n    color: var(--navbar-background);\n  }\n</style>\n"]
             },
             media: undefined
         });
 
     };
     /* scoped */
     const __vue_scope_id__ = undefined;
@@ -15264,84 +15296,80 @@
             return container.innerHTML
         }
     }
 
     Vue.compile = compileToFunctions;
 
     // ===========================================================================
-    function main(staticPrefix, url, prefix, timestamp, logoUrl, navbarBackground, navbarColor, navbarLightButtons, locale, allLocales, i18nStrings, logoHomeUrl) {
+    function main(config, locale, i18nStrings) {
         PywbI18N.init(locale, i18nStrings);
-        new CDXLoader(staticPrefix, url, prefix, timestamp, logoUrl, navbarBackground, navbarColor, navbarLightButtons, allLocales, logoHomeUrl);
+        new CDXLoader(config);
     }
 
     // ===========================================================================
     class CDXLoader {
-        constructor(staticPrefix, url, prefix, timestamp, logoUrl, navbarBackground, navbarColor, navbarLightButtons, allLocales, logoHomeUrl) {
+        constructor(config) {
             this.loadingSpinner = null;
             this.loaded = false;
             this.opts = {};
-            this.prefix = prefix;
-            this.staticPrefix = staticPrefix;
-            this.logoUrl = logoUrl;
-            this.logoHomeUrl = logoHomeUrl;
-            this.navbarBackground = navbarBackground;
-            this.navbarColor = navbarColor;
-            this.navbarLightButtons = navbarLightButtons;
-            this.timestamp = timestamp;
+            this.url = config.url;
+            this.prefix = config.prefix;
+            this.staticPrefix = config.staticPrefix;
+            this.logoUrl = config.logoUrl;
+            this.logoHomeUrl = config.logoHomeUrl;
+            this.navbarBackground = config.navbarBackground;
+            this.navbarColor = config.navbarColor;
+            this.navbarLightButtons = config.navbarLightButtons;
+            this.disablePrinting = config.disablePrinting;
 
-            this.isReplay = (timestamp !== undefined);
+            this.timestamp = config.timestamp;
+
+            this.isReplay = (config.timestamp !== undefined);
 
             setTimeout(() => {
                 if (!this.loaded) {
                     this.loadingSpinner = new LoadingSpinner({
                         text: PywbI18N.instance?.getText('Loading...'),
-                        isSmall: !!timestamp
+                        isSmall: !!this.timestamp
                     }); // bootstrap loading-spinner EARLY ON
                     this.loadingSpinner.setOn();
                 }
             }, 500);
 
             if (this.isReplay) {
-                window.WBBanner = new VueBannerWrapper(this, url, timestamp);
+                window.WBBanner = new VueBannerWrapper(this, this.url, this.timestamp);
             }
 
             let queryURL;
+            let url;
 
             // query form *?=url...
             if (window.location.href.indexOf("*?") > 0) {
                 queryURL = window.location.href.replace("*?", "cdx?") + "&output=json";
                 url = new URL(queryURL).searchParams.get("url");
 
                 // otherwise, traditional calendar form /*/<url>
-            } else if (url) {
+            } else if (this.url) {
+                url = this.url;
                 const params = new URLSearchParams();
                 params.set("url", url);
                 params.set("output", "json");
-                queryURL = prefix + "cdx?" + params.toString();
+                queryURL = this.prefix + "cdx?" + params.toString();
 
                 // otherwise, an error since no URL
             } else {
                 throw new Error("No query URL specified");
             }
 
-            const logoImg = this.staticPrefix + "/" + (this.logoUrl ? this.logoUrl : "pywb-logo-sm.png");
+            config.logoImg = this.staticPrefix + "/" + (!!this.logoUrl ? this.logoUrl : "pywb-logo-sm.png");
 
-            this.app = this.initApp({
-                logoImg,
-                logoHomeUrl,
-                navbarBackground,
-                navbarColor,
-                navbarLightButtons,
-                url,
-                allLocales,
-                timestamp
-            });
+            this.app = this.initApp(config);
 
             this.loadCDX(queryURL).then((cdxList) => {
-                this.setAppData(cdxList, url, this.timestamp);
+                this.setAppData(cdxList, url, config.timestamp);
             });
         }
 
         initApp(config = {}) {
             const app = new Vue(__vue_component__);
 
             app.$set(app, "config", {
@@ -15518,8 +15546,8 @@
     Object.defineProperty(exports, '__esModule', {
         value: true
     });
 
     return exports;
 
 }({}));
```

### Comparing `pywb-2.7.4/pywb/static/wb_frame.js` & `pywb-2.8.0/pywb/static/wb_frame.js`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/static/wombat.js` & `pywb-2.8.0/pywb/static/wombat.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 /*
 Wombat.js client-side rewriting engine for web archive replay
-Copyright (C) 2014-2023 Webrecorder Software, Rhizome, and Contributors. Released under the GNU Affero General Public License.
+Copyright (C) 2014-2024 Webrecorder Software, Rhizome, and Contributors. Released under the GNU Affero General Public License.
 
 This file is part of wombat.js, see https://github.com/webrecorder/wombat.js for the full source
 Wombat.js is part of the Webrecorder project (https://github.com/webrecorder)
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU Affero General Public License as published
 by the Free Software Foundation, either version 3 of the License, or
@@ -101,15 +101,15 @@
                     value: function(prop) {
                         return this._orig_loc[prop]
                     }
                 },
                 orig_setter: {
                     enumerable: false,
                     value: function(prop, value) {
-                        this._orig_loc[prop] = value
+                        this._orig_loc[prop] != value && (this._orig_loc[prop] = value)
                     }
                 }
             }), wombat.initLocOverride(this, this.orig_setter, this.orig_getter), wombat.setLoc(this, orig_loc.href), orig_loc) this.hasOwnProperty(prop) || typeof orig_loc[prop] === "function" || (this[prop] = orig_loc[prop])
     }
 
     function AutoFetcher(wombat, config) {
         return this instanceof AutoFetcher ? void(this.elemSelector = "img[srcset], img[data-srcset], img[data-src], video[srcset], video[data-srcset], video[data-src], audio[srcset], audio[data-srcset], audio[data-src], picture > source[srcset], picture > source[data-srcset], picture > source[data-src], video > source[srcset], video > source[data-srcset], video > source[data-src], audio > source[srcset], audio > source[data-srcset], audio > source[data-src]", this.wombat = wombat, this.$wbwindow = wombat.$wbwindow, this.worker = null, autobind(this), this._initWorker(config)) : new AutoFetcher(wombat, config)
@@ -234,15 +234,15 @@
 
     function g(t, e) {
         return y(t, e).toString()
     }
 
     function Wombat($wbwindow, wbinfo) {
         if (!(this instanceof Wombat)) return new Wombat($wbwindow, wbinfo);
-        this.debug_rw = false, this.$wbwindow = $wbwindow, this.WBWindow = Window, this.origHost = $wbwindow.location.host, this.origHostname = $wbwindow.location.hostname, this.origProtocol = $wbwindow.location.protocol, this.HTTP_PREFIX = "http://", this.HTTPS_PREFIX = "https://", this.REL_PREFIX = "//", this.VALID_PREFIXES = [this.HTTP_PREFIX, this.HTTPS_PREFIX, this.REL_PREFIX], this.IGNORE_PREFIXES = ["#", "about:", "data:", "blob:", "mailto:", "javascript:", "{", "*"], "ignore_prefixes" in wbinfo && (this.IGNORE_PREFIXES = this.IGNORE_PREFIXES.concat(wbinfo.ignore_prefixes)), this.WB_CHECK_THIS_FUNC = "_____WB$wombat$check$this$function_____", this.WB_ASSIGN_FUNC = "_____WB$wombat$assign$function_____", this.wb_setAttribute = $wbwindow.Element.prototype.setAttribute, this.wb_getAttribute = $wbwindow.Element.prototype.getAttribute, this.wb_funToString = Function.prototype.toString, this.WBAutoFetchWorker = null, this.wbUseAFWorker = wbinfo.enable_auto_fetch && $wbwindow.Worker != null && wbinfo.is_live, this.wb_rel_prefix = "", this.wb_wombat_updating = false, this.message_listeners = new FuncMap, this.storage_listeners = new FuncMap, this.linkAsTypes = {
+        this.debug_rw = false, this.$wbwindow = $wbwindow, this.WBWindow = Window, this.URL = URL, this.origHost = $wbwindow.location.host, this.origHostname = $wbwindow.location.hostname, this.origProtocol = $wbwindow.location.protocol, this.HTTP_PREFIX = "http://", this.HTTPS_PREFIX = "https://", this.REL_PREFIX = "//", this.VALID_PREFIXES = [this.HTTP_PREFIX, this.HTTPS_PREFIX, this.REL_PREFIX], this.IGNORE_PREFIXES = ["#", "about:", "data:", "blob:", "mailto:", "javascript:", "{", "*"], "ignore_prefixes" in wbinfo && (this.IGNORE_PREFIXES = this.IGNORE_PREFIXES.concat(wbinfo.ignore_prefixes)), this.WB_CHECK_THIS_FUNC = "_____WB$wombat$check$this$function_____", this.WB_ASSIGN_FUNC = "_____WB$wombat$assign$function_____", this.wb_setAttribute = $wbwindow.Element.prototype.setAttribute, this.wb_getAttribute = $wbwindow.Element.prototype.getAttribute, this.wb_funToString = Function.prototype.toString, this.WBAutoFetchWorker = null, this.wbUseAFWorker = wbinfo.enable_auto_fetch && $wbwindow.Worker != null && wbinfo.is_live, this.wb_rel_prefix = "", this.wb_wombat_updating = false, this.message_listeners = new FuncMap, this.storage_listeners = new FuncMap, this.linkAsTypes = {
             script: "js_",
             worker: "js_",
             style: "cs_",
             image: "im_",
             document: "if_",
             fetch: "mp_",
             font: "oe_",
@@ -600,15 +600,16 @@
         return str.indexOf("[native code]") != -1 && (!(funToTest.__WB_is_native_func__ !== undefined) || !!funToTest.__WB_is_native_func__)
     }, Wombat.prototype.isString = function(arg) {
         return arg != null && Object.getPrototypeOf(arg) === String.prototype
     }, Wombat.prototype.blobUrlForIframe = function(iframe, string) {
         var blob = new Blob([string], {
                 type: "text/html"
             }),
-            url = URL.createObjectURL(blob);
+            url = this.URL.createObjectURL(blob),
+            URL = this.URL;
         iframe.__wb_blobSrc = url, iframe.addEventListener("load", function() {
             iframe.__wb_blobSrc && (URL.revokeObjectURL(iframe.__wb_blobSrc), iframe.__wb_blobSrc = null)
         }, {
             once: true
         }), iframe.__wb_origSrc = iframe.src;
         var blobIdUrl = url.slice(url.lastIndexOf("/") + 1) + "/" + this.wb_info.url;
         iframe.src = this.wb_info.prefix + this.wb_info.request_ts + "mp_/blob:" + blobIdUrl
@@ -718,20 +719,20 @@
         })
     }, Wombat.prototype.reconstructDocType = function(doctype) {
         return doctype == null ? "" : "<!doctype " + doctype.name + (doctype.publicId ? " PUBLIC \"" + doctype.publicId + "\"" : "") + (!doctype.publicId && doctype.systemId ? " SYSTEM" : "") + (doctype.systemId ? " \"" + doctype.systemId + "\"" : "") + ">"
     }, Wombat.prototype.getFinalUrl = function(useRel, mod, url) {
         var prefix = useRel ? this.wb_rel_prefix : this.wb_abs_prefix;
         return mod == null && (mod = this.wb_info.mod), this.wb_info.is_live || (prefix += this.wb_info.wombat_ts), prefix += mod, prefix[prefix.length - 1] !== "/" && (prefix += "/"), prefix + url
     }, Wombat.prototype.resolveRelUrl = function(url, doc) {
-        var docObj = doc || this.$wbwindow.document,
-            parser = this.makeParser(docObj.baseURI, docObj),
-            hash = parser.href.lastIndexOf("#"),
-            href = hash >= 0 ? parser.href.substring(0, hash) : parser.href,
-            lastslash = href.lastIndexOf("/");
-        return parser.href = lastslash >= 0 && lastslash !== href.length - 1 ? href.substring(0, lastslash + 1) + url : href + url, parser.href
+        function isValidBaseURI(doc) {
+            return !!(doc && doc.baseURI) && (doc.baseURI.startsWith(wombat.HTTPS_PREFIX) || doc.baseURI.startsWith(wombat.HTTP_PREFIX))
+        }
+        var wombat = this,
+            baseURI = null;
+        return baseURI = isValidBaseURI(doc) ? doc.baseURI : isValidBaseURI(this.$wbwindow.document) ? this.$wbwindow.document.baseURI : this.$wbwindow.__WB_replay_top.document.baseURI, new this.URL(url, baseURI).href
     }, Wombat.prototype.extractOriginalURL = function(rewrittenUrl) {
         if (!rewrittenUrl) return "";
         if (this.wb_is_proxy) return rewrittenUrl;
         var rwURLString = rewrittenUrl.toString(),
             url = rwURLString;
         if (this.startsWithOneOf(url, this.IGNORE_PREFIXES)) return url;
         if (url.startsWith(this.wb_info.static_prefix)) return url;
@@ -892,31 +893,30 @@
             return prop === "href" ? wombat.extractOriginalURL(curr_orig_href) : prop === "ancestorOrigins" ? [] : (this._orig_href !== curr_orig_href && wombat.setLoc(this, curr_orig_href), this["_" + prop])
         }
     }, Wombat.prototype.makeSetLocProp = function(prop, origSetter, origGetter) {
         var wombat = this;
         return function newSetLocProp(value) {
             if (this._no_rewrite) return origSetter.call(this, prop, value);
             if (this["_" + prop] !== value) {
-                if (this["_" + prop] = value, !this._parser) {
-                    var href = origGetter.call(this);
-                    this._parser = wombat.makeParser(href, this.ownerDocument)
-                }
-                var rel = false;
+                this["_" + prop] = value;
+                var href = origGetter.call(this),
+                    parser = wombat.makeParser(href, this.ownerDocument),
+                    rel = false;
                 if (prop === "href" && typeof value === "string")
-                    if (value && this._parser instanceof URL) try {
-                        value = new URL(value, this._parser).href
+                    if (value && parser instanceof wombat.URL) try {
+                        value = new wombat.URL(value, parser).href
                     } catch (e) {
                         console.warn("Error resolving URL", e)
-                    } else value && (value[0] === "." || value[0] === "#" ? value = wombat.resolveRelUrl(value, this.ownerDocument) : value[0] === "/" && (value.length > 1 && value[1] === "/" ? value = this._parser.protocol + value : (rel = true, value = WB_wombat_location.origin + value)));
+                    } else value && (value[0] === "." || value[0] === "#" ? value = wombat.resolveRelUrl(value, this.ownerDocument) : value[0] === "/" && (value.length > 1 && value[1] === "/" ? value = parser.protocol + value : (rel = true, value = WB_wombat_location.origin + value)));
                 try {
-                    this._parser[prop] = value
+                    parser[prop] = value
                 } catch (e) {
                     console.log("Error setting " + prop + " = " + value)
                 }
-                prop === "hash" ? (value = this._parser[prop], origSetter.call(this, "hash", value)) : (rel = rel || value === this._parser.pathname, value = wombat.rewriteUrl(this._parser.href, rel), origSetter.call(this, "href", value))
+                prop === "hash" ? (value = parser[prop], origSetter.call(this, "hash", value)) : (rel = rel || value === parser.pathname, value = wombat.rewriteUrl(parser.href, rel), origSetter.call(this, "href", value))
             }
         }
     }, Wombat.prototype.styleReplacer = function(match, n1, n2, n3, offset, string) {
         return n1 + this.rewriteUrl(n2) + n3
     }, Wombat.prototype.domConstructorErrorChecker = function(thisObj, what, args, numRequiredArgs) {
         var errorMsg, needArgs = typeof numRequiredArgs === "number" ? numRequiredArgs : 1;
         if (thisObj instanceof this.WBWindow ? errorMsg = "Failed to construct '" + what + "': Please use the 'new' operator, this DOM object constructor cannot be called as a function." : args && args.length < needArgs && (errorMsg = "Failed to construct '" + what + "': " + needArgs + " argument required, but only 0 present."), errorMsg) throw new TypeError(errorMsg)
@@ -928,15 +928,19 @@
             case Node.TEXT_NODE:
                 (fnThis.tagName === "STYLE" || newNode.parentNode && newNode.parentNode.tagName === "STYLE") && (newNode.textContent = this.rewriteStyle(newNode.textContent));
                 break;
             case Node.DOCUMENT_FRAGMENT_NODE:
                 this.recurseRewriteElem(newNode);
         }
         var created = originalFn.call(fnThis, newNode, oldNode);
-        return created && created.tagName === "IFRAME" && (created.allow = "autoplay 'self'; fullscreen 'self'", this.initIframeWombat(created)), created
+        if (created && created.tagName === "IFRAME") {
+            const currentAllow = created.allow ? `; ${created.allow}` : "";
+            created.allow = `autoplay 'self'; fullscreen 'self'${currentAllow}`, this.initIframeWombat(created)
+        }
+        return created
     }, Wombat.prototype.rewriteWSURL = function(originalURL) {
         if (!originalURL) return originalURL;
         var urltype_ = typeof originalURL,
             url = originalURL;
         if (urltype_ === "object") url = originalURL.toString();
         else if (urltype_ !== "string") return originalURL;
         if (!url) return url;
@@ -983,16 +987,16 @@
                     rebuild = false;
                 return path.indexOf(this.wb_rel_prefix) < 0 && url.indexOf("/static/") < 0 && (path = this.getFinalUrl(true, mod, WB_wombat_location.origin + "/" + path), rebuild = true), prefix !== curr_scheme && prefix !== this.REL_PREFIX && (rebuild = true), rebuild && (url = useRel ? "" : curr_scheme + orig_host, path && path[0] !== "/" && (url += "/"), url += path), url
             }
             return this.getFinalUrl(useRel, mod, url)
         }
         return prefix = this.startsWithOneOf(url, this.BAD_PREFIXES), prefix ? this.getFinalUrl(useRel, mod, this.extractOriginalURL(url)) : url
     }, Wombat.prototype.rewriteUrl = function(url, useRel, mod, doc) {
-        var rewritten = this.rewriteUrl_(url, useRel, mod, doc);
-        return this.debug_rw && (url === rewritten ? console.log("NOT REWRITTEN " + url) : console.log("REWRITE: " + url + " -> " + rewritten)), rewritten
+        var rewritten;
+        return rewritten = this.wb_info.rewrite_function ? this.wb_info.rewrite_function(url, useRel, mod, doc) : this.rewriteUrl_(url, useRel, mod, doc), this.debug_rw && (url === rewritten ? console.log("NOT REWRITTEN " + url) : console.log("REWRITE: " + url + " -> " + rewritten)), rewritten
     }, Wombat.prototype.performAttributeRewrite = function(elem, name, value, absUrlOnly) {
         switch (name) {
             case "innerHTML":
             case "outerHTML":
                 return this.rewriteHtml(value);
             case "filter":
                 return this.rewriteInlineStyle(value);
@@ -1035,15 +1039,15 @@
             new_value = "javascript:window.parent._wb_wombat.initNewWindowWombat(window);" + value.substr(11)
         }
         return new_value || (new_value = this.rewriteUrl(value, false, this.rwModForElement(elem, attrName))), new_value !== value && (this.wb_setAttribute.call(elem, attrName, new_value), true)
     }, Wombat.prototype.rewriteScript = function(elem) {
         if (elem.hasAttribute("src") || !elem.textContent || !this.$wbwindow.Proxy) return this.rewriteAttr(elem, "src");
         if (this.skipWrapScriptBasedOnType(elem.type)) return false;
         var text = elem.textContent.trim();
-        return !this.skipWrapScriptTextBasedOnText(text) && (elem.textContent = this.wrapScriptTextJsProxy(text), true)
+        return !this.skipWrapScriptTextBasedOnText(text) && (elem.textContent = this.wrapScriptTextJsProxy(text), this.wb_info.injectDocClose && elem.textContent.trim().length && (elem.textContent += ";document.close();"), true)
     }, Wombat.prototype.rewriteSVGElem = function(elem) {
         var changed = this.rewriteAttr(elem, "filter");
         return changed = this.rewriteAttr(elem, "style") || changed, changed = this.rewriteAttr(elem, "xlink:href") || changed, changed = this.rewriteAttr(elem, "href") || changed, changed = this.rewriteAttr(elem, "src") || changed, changed
     }, Wombat.prototype.rewriteElem = function(elem) {
         var changed = false;
         if (!elem) return changed;
         if (elem instanceof SVGElement) changed = this.rewriteSVGElem(elem);
@@ -1097,15 +1101,15 @@
             case "A":
                 if (changed = this.rewriteAttr(elem, "href") || changed, elem.hasAttribute("target")) {
                     var newTarget = this.rewriteAttrTarget(elem.target);
                     newTarget !== elem.target && (elem.target = newTarget, changed = true)
                 }
                 break;
             default: {
-                changed = this.rewriteAttr(elem, "src"), changed = this.rewriteAttr(elem, "srcset") || changed, changed = this.rewriteAttr(elem, "href") || changed, changed = this.rewriteAttr(elem, "style") || changed, changed = this.rewriteAttr(elem, "poster") || changed;
+                changed = this.rewriteAttr(elem, "src"), changed = this.rewriteAttr(elem, "srcset") || changed, changed = this.rewriteAttr(elem, "href") || changed, changed = this.rewriteAttr(elem, "style") || changed, changed = this.rewriteAttr(elem, "poster") || changed, changed = this.rewriteAttr(elem, "background") || changed;
                 break
             }
         }
         return elem.hasAttribute && elem.removeAttribute && (elem.hasAttribute("crossorigin") && (elem.removeAttribute("crossorigin"), changed = true), elem.hasAttribute("integrity") && (elem.removeAttribute("integrity"), changed = true)), changed
     }, Wombat.prototype.recurseRewriteElem = function(curr) {
         if (!this.nodeHasChildren(curr)) return false;
         for (var changed = false, rewriteQ = [curr.children || curr.childNodes]; rewriteQ.length > 0;)
@@ -1128,15 +1132,19 @@
         var template = inner_doc.head.children[0];
         if (template._no_rewrite = true, this.recurseRewriteElem(template.content)) {
             var new_html = template.innerHTML;
             if (checkEndTag) {
                 var first_elem = template.content.children && template.content.children[0];
                 if (first_elem) {
                     var end_tag = "</" + first_elem.tagName.toLowerCase() + ">";
-                    this.endsWith(new_html, end_tag) && !this.endsWith(rwString.toLowerCase(), end_tag) && (new_html = new_html.substring(0, new_html.length - end_tag.length))
+                    if (this.endsWith(new_html, end_tag) && !this.endsWith(rwString.toLowerCase(), end_tag)) new_html = new_html.substring(0, new_html.length - end_tag.length);
+                    else if (new_html.trimEnd().endsWith(end_tag) && !rwString.trimEnd().endsWith(end_tag)) {
+                        var lastInx = rwString.lastIndexOf(end_tag);
+                        lastInx > 0 && (new_html += rwString.slice(lastInx + end_tag.length))
+                    }
                 } else if (rwString[0] !== "<" || rwString[rwString.length - 1] !== ">") return this.write_buff += rwString, undefined
             }
             return new_html
         }
         return rwString
     }, Wombat.prototype.rewriteHtmlFull = function(string, checkEndTag) {
         var inner_doc = new DOMParser().parseFromString(string, "text/html");
@@ -1207,15 +1215,15 @@
                 ww_rw = this.wb_info.ww_rw_script || this.wb_info.static_prefix + "wombatWorkers.js",
                 rw = "(function() { self.importScripts('" + ww_rw + "'); new WBWombat({'prefix': '" + this.wb_abs_prefix + "', 'prefixMod': '" + this.wb_abs_prefix + "wkrf_/', 'originalURL': '" + originalURL + "'}); })();";
             workerCode = rw + workerCode
         }
         var blob = new Blob([workerCode], {
             type: "application/javascript"
         });
-        return URL.createObjectURL(blob)
+        return this.URL.createObjectURL(blob)
     }, Wombat.prototype.rewriteTextNodeFn = function(fnThis, originalFn, argsObj) {
         var args, deproxiedThis = this.proxyToObj(fnThis);
         if (argsObj.length > 0 && deproxiedThis.parentElement && deproxiedThis.parentElement.tagName === "STYLE") {
             args = new Array(argsObj.length);
             var dataIndex = argsObj.length - 1;
             dataIndex === 2 ? (args[0] = argsObj[0], args[1] = argsObj[1]) : dataIndex === 1 && (args[0] = argsObj[0]), args[dataIndex] = this.rewriteStyle(argsObj[dataIndex])
         } else args = argsObj;
@@ -1324,16 +1332,17 @@
     }, Wombat.prototype.overrideHistoryFunc = function(funcName) {
         if (!this.$wbwindow.history) return undefined;
         var orig_func = this.$wbwindow.history[funcName];
         if (!orig_func) return undefined;
         this.$wbwindow.history["_orig_" + funcName] = orig_func, this.$wbwindow.history.___wb_ownWindow = this.$wbwindow;
         var wombat = this,
             rewrittenFunc = function histNewFunc(stateObj, title, url) {
-                var rewritten_url, resolvedURL, historyWin = this.___wb_ownWindow || wombat.$wbwindow,
-                    wombatLocation = historyWin.WB_wombat_location;
+                var historyWin = this.___wb_ownWindow || wombat.$wbwindow;
+                url = wombat.extractOriginalURL(url);
+                var rewritten_url, resolvedURL, wombatLocation = historyWin.WB_wombat_location;
                 if (url) {
                     var parser = wombat._makeURLParser(url, historyWin.document);
                     if (resolvedURL = parser.href, rewritten_url = wombat.rewriteUrl(resolvedURL), resolvedURL !== wombatLocation.origin && wombatLocation.href !== "about:blank" && !wombat.startsWith(resolvedURL, wombatLocation.origin + "/")) throw new DOMException("Invalid history change: " + resolvedURL)
                 } else resolvedURL = wombatLocation.href;
                 orig_func.call(this, stateObj, title, rewritten_url);
                 var origTitle = historyWin.document.title;
                 wombat.WBAutoFetchWorker && historyWin.setTimeout(function() {
@@ -1413,15 +1422,15 @@
             orig_getter = this.getOrigGetter(obj, "dataset"),
             wombat = this,
             getter = function wrapDataSet() {
                 var dataset = orig_getter.call(this),
                     proxy = new Proxy(dataset, {
                         get(target, prop, receiver) {
                             var result = target[prop];
-                            return wombat.startsWithOneOf(result, wombat.wb_prefixes) ? wombat.extractOriginalURL(result) : result
+                            return typeof result === "string" && wombat.startsWithOneOf(result, wombat.wb_prefixes) ? wombat.extractOriginalURL(result) : result
                         }
                     });
                 return proxy
             };
         this.defProp(obj, "dataset", null, getter)
     }, Wombat.prototype.overrideStyleProxy = function(overrideProps) {
         var obj = this.$wbwindow.HTMLElement.prototype,
@@ -1799,20 +1808,38 @@
                 wombat = this;
             this.$wbwindow.Blob = function(Blob_) {
                 return function Blob(array, options) {
                     return options && (options.type === "application/xhtml+xml" || options.type === "text/html") && array.length === 1 && typeof array[0] === "string" && wombat.startsWith(array[0], "<!DOCTYPE html>") && (array[0] = wombat.rewriteHtml(array[0]), options.type = "text/html"), new Blob_(array, options)
                 }
             }(this.$wbwindow.Blob), this.$wbwindow.Blob.prototype = orig_blob.prototype
         }
+    }, Wombat.prototype.initIntersectionObsOverride = function() {
+        var orig_iobs = this.$wbwindow.IntersectionObserver,
+            wombat = this;
+        this.$wbwindow.IntersectionObserver = function(IObs) {
+            return function(callback, options) {
+                return options && options.root && (options.root = wombat.proxyToObj(options.root)), new IObs(callback, options)
+            }
+        }(this.$wbwindow.IntersectionObserver), this.$wbwindow.IntersectionObserver.prototype = orig_iobs.prototype, Object.defineProperty(this.$wbwindow.IntersectionObserver.prototype, "constructor", {
+            value: this.$wbwindow.IntersectionObserver
+        })
     }, Wombat.prototype.initWSOverride = function() {
         this.$wbwindow.WebSocket && this.$wbwindow.WebSocket.prototype && (this.$wbwindow.WebSocket = function(WebSocket_) {
             function WebSocket(url, protocols) {
-                this.addEventListener = function() {}, this.removeEventListener = function() {}, this.close = function() {}, this.send = function(data) {
+                function simOpen() {
+                    var ev = new CustomEvent("open");
+                    ws.onopen && ws.onopen(ev), ws.openCallbacks.forEach(callback => callback(ev))
+                }
+                this.openCallbacks = [], this.addEventListener = function(type, callback) {
+                    type === "open" && WebSocket.openCallbacks.push(callback)
+                }, this.removeEventListener = function() {}, this.close = function() {}, this.send = function(data) {
                     console.log("ws send", data)
-                }, this.protocol = protocols && protocols.length ? protocols[0] : "", this.url = url, this.readyState = 0
+                }, this.protocol = protocols && protocols.length ? protocols[0] : "", this.url = url, this.readyState = 1;
+                var ws = this;
+                setTimeout(simOpen, 500)
             }
             return WebSocket.CONNECTING = 0, WebSocket.OPEN = 1, WebSocket.CLOSING = 2, WebSocket.CLOSED = 3, WebSocket
         }(this.$wbwindow.WebSocket), Object.defineProperty(this.$wbwindow.WebSocket.prototype, "constructor", {
             value: this.$wbwindow.WebSocket
         }), addToStringTagToClass(this.$wbwindow.WebSocket, "WebSocket"))
     }, Wombat.prototype.initDocTitleOverride = function() {
         var orig_get_title = this.getOrigGetter(this.$wbwindow.document, "title"),
@@ -2097,15 +2124,15 @@
 
         function prepForWrite(args) {
             var string;
             return args.length === 0 ? "" : (string = args.length === 1 ? args[0] : Array.prototype.join.call(args, ""), string)
         }
 
         function docWrite(fnThis, originalFn, string) {
-            if (wombat.$wbwindow, isSWLoad()) return void(wombat._writeBuff += string);
+            if (wombat.$wbwindow, isSWLoad() || document.readyState === "loading" && wombat.wb_info.injectDocClose) return void(wombat._writeBuff += string);
             string = wombat.rewriteHtml(string, true);
             var thisObj = wombat.proxyToObj(fnThis),
                 res = originalFn.call(thisObj, string);
             return wombat.initNewWindowWombat(thisObj.defaultView), res
         }
         if (this.$wbwindow.DOMParser) {
             var DocumentProto = this.$wbwindow.Document.prototype,
@@ -2130,15 +2157,15 @@
                         res = orig_doc_open.call(thisObj, rwUrl, arguments[1], arguments[2]), wombat.initNewWindowWombat(res, arguments[0])
                     } else res = orig_doc_open.call(thisObj), isSWLoad() ? wombat._writeBuff = "" : wombat.initNewWindowWombat(thisObj.defaultView);
                     return res
                 };
             $wbDocument.open = new_open, DocumentProto.open = new_open;
             var originalClose = $wbDocument.close,
                 newClose = function close() {
-                    if (wombat._writeBuff) return wombat.blobUrlForIframe(wombat.$wbwindow.frameElement, wombat._writeBuff), void(wombat._writeBuff = "");
+                    if (wombat._writeBuff) return isSWLoad() ? wombat.blobUrlForIframe(wombat.$wbwindow.frameElement, wombat._writeBuff) : document.readyState === "loading" && orig_doc_write.call($wbDocument, wombat.rewriteHtml(wombat._writeBuff, true)), void(wombat._writeBuff = "");
                     var thisObj = wombat.proxyToObj(this);
                     return wombat.initNewWindowWombat(thisObj.defaultView), originalClose.__WB_orig_apply ? originalClose.__WB_orig_apply(thisObj, arguments) : originalClose.apply(thisObj, arguments)
                 };
             $wbDocument.close = newClose, DocumentProto.close = newClose;
             var oBodyGetter = this.getOrigGetter(DocumentProto, "body"),
                 oBodySetter = this.getOrigSetter(DocumentProto, "body");
             oBodyGetter && oBodySetter && this.defProp(DocumentProto, "body", function body(newBody) {
@@ -2204,15 +2231,15 @@
             }(oSharedWorker), this.$wbwindow.SharedWorker.prototype = oSharedWorker.prototype, Object.defineProperty(this.$wbwindow.SharedWorker.prototype, "constructor", {
                 value: this.$wbwindow.SharedWorker
             }), this.$wbwindow.SharedWorker.__wb_sharedWorker_overridden = true
         }
         if (this.$wbwindow.ServiceWorkerContainer && this.$wbwindow.ServiceWorkerContainer.prototype && this.$wbwindow.ServiceWorkerContainer.prototype.register) {
             var orig_register = this.$wbwindow.ServiceWorkerContainer.prototype.register;
             this.$wbwindow.ServiceWorkerContainer.prototype.register = function register(scriptURL, options) {
-                var newScriptURL = new URL(scriptURL, wombat.$wbwindow.document.baseURI).href,
+                var newScriptURL = new wombat.URL(scriptURL, wombat.$wbwindow.document.baseURI).href,
                     mod = wombat.getPageUnderModifier();
                 return options && options.scope ? options.scope = wombat.rewriteUrl(options.scope, false, mod) : options = {
                     scope: wombat.rewriteUrl("/", false, mod)
                 }, orig_register.call(this, wombat.rewriteUrl(newScriptURL, false, "sw_"), options)
             }
         }
         if (this.$wbwindow.Worklet && this.$wbwindow.Worklet.prototype && this.$wbwindow.Worklet.prototype.addModule && !this.$wbwindow.Worklet.__wb_workerlet_overridden) {
@@ -2274,15 +2301,15 @@
                     return thisObj && thisObj._WB_wombat_obj_proxy ? thisObj._WB_wombat_obj_proxy : thisObj
                 }
             })
         } catch (e) {}
     }, Wombat.prototype.initImportWrapperFunc = function(win) {
         var wombat = this;
         win.____wb_rewrite_import__ = function(base, url) {
-            return base && (url = new URL(url, base).href), import(wombat.rewriteUrl(url, false, "esm_"))
+            return base && (url = new wombat.URL(url, base).href), import(wombat.rewriteUrl(url, false, "esm_"))
         }
     }, Wombat.prototype.overrideGetOwnPropertyNames = function(win) {
         var orig_getOwnPropertyNames = win.Object.getOwnPropertyNames,
             removeProps = [this.WB_CHECK_THIS_FUNC, "WB_wombat_location", "__WB_pmw", "WB_wombat_top", "WB_wombat_eval", "WB_wombat_runEval"];
         try {
             win.Object.defineProperty(win.Object, "getOwnPropertyNames", {
                 value: function(object) {
@@ -2768,15 +2795,15 @@
             };
         this.defProp(this.$wbwindow.Object.prototype, "WB_wombat_runEval", setNoop, function() {
             return runEval
         }), this.defProp(this.$wbwindow.Object.prototype, "WB_wombat_runEval2", setNoop, function() {
             return runEval2
         })
     }, Wombat.prototype.wombatInit = function() {
-        this._internalInit(), this.initCookiePreset(), this.initHistoryOverrides(), this.overrideFunctionApply(this.$wbwindow), this.overrideFunctionBind(this.$wbwindow), this.initDocTitleOverride(), this.initHashChange(), this.wb_opts.skip_postmessage || (this.initPostMessageOverride(this.$wbwindow), this.initMessageEventOverride(this.$wbwindow)), this.initCheckThisFunc(this.$wbwindow), this.initImportWrapperFunc(this.$wbwindow), this.overrideGetOwnPropertyNames(this.$wbwindow), this.initUIEventsOverrides(), this.initDocWriteOpenCloseOverride(), this.initEvalOverride(), this.initHTTPOverrides(), this.initAudioOverride(), this.initFontFaceOverride(this.$wbwindow), this.initWorkerOverrides(), this.initTextNodeOverrides(), this.initCSSOMOverrides(), this.overrideHtmlAssign(this.$wbwindow.Element, "innerHTML", true), this.overrideHtmlAssign(this.$wbwindow.Element, "outerHTML", true), this.overrideHtmlAssignSrcDoc(this.$wbwindow.HTMLIFrameElement, "srcdoc", true), this.overrideHtmlAssign(this.$wbwindow.HTMLStyleElement, "textContent"), this.overrideShadowDom(), this.overridePropExtract(this.$wbwindow.Document.prototype, "URL"), this.overridePropExtract(this.$wbwindow.Document.prototype, "documentURI"), this.overridePropExtract(this.$wbwindow.Node.prototype, "baseURI"), this.overrideAttrProps(), this.overrideDataSet(), this.initInsertAdjacentElementHTMLOverrides(), this.overrideIframeContentAccess("contentWindow"), this.overrideIframeContentAccess("contentDocument"), this.overrideFuncArgProxyToObj(this.$wbwindow.MutationObserver, "observe"), this.overrideFuncArgProxyToObj(this.$wbwindow.Node, "compareDocumentPosition"), this.overrideFuncArgProxyToObj(this.$wbwindow.Node, "contains"), this.overrideFuncArgProxyToObj(this.$wbwindow.Document, "createTreeWalker"), this.overrideFuncArgProxyToObj(this.$wbwindow.Document, "evaluate", 1), this.overrideFuncArgProxyToObj(this.$wbwindow.XSLTProcessor, "transformToFragment", 1), this.overrideFuncThisProxyToObj(this.$wbwindow, "getComputedStyle", this.$wbwindow), this.overrideFuncThisProxyToObj(this.$wbwindow, "clearTimeout"), this.overrideFuncThisProxyToObj(this.$wbwindow, "clearInterval"), this.overrideFuncThisProxyToObj(this.$wbwindow.EventTarget.prototype, "dispatchEvent"), this.initTimeoutIntervalOverrides(), this.overrideFramesAccess(this.$wbwindow), this.overrideSWAccess(this.$wbwindow), this.initElementGetSetAttributeOverride(), this.initSvgImageOverrides(), this.initAttrOverrides(), this.initCookiesOverride(), this.initCreateElementNSFix(), this.wb_opts.skip_dom || this.initDomOverride(), this.initRegisterUnRegPHOverride(), this.initPresentationRequestOverride(), this.initBeaconOverride(), this.initMiscNavigatorOverrides(), this.initSeededRandom(this.wb_info.wombat_sec), this.initCryptoRandom(), this.initFixedRatio(this.wb_info.pixel_ratio || 1), this.initDateOverride(this.wb_info.wombat_sec), this.initBlobOverride(), this.initWSOverride(), this.initOpenOverride(), this.initDisableNotificationsGeoLocation(), this.initStorageOverride(), this.initCachesOverride(), this.initIndexedDBOverride(), this.initWindowObjProxy(this.$wbwindow), this.initDocumentObjProxy(this.$wbwindow.document);
+        this._internalInit(), this.initCookiePreset(), this.initHistoryOverrides(), this.overrideFunctionApply(this.$wbwindow), this.overrideFunctionBind(this.$wbwindow), this.initDocTitleOverride(), this.initHashChange(), this.wb_opts.skip_postmessage || (this.initPostMessageOverride(this.$wbwindow), this.initMessageEventOverride(this.$wbwindow)), this.initCheckThisFunc(this.$wbwindow), this.initImportWrapperFunc(this.$wbwindow), this.overrideGetOwnPropertyNames(this.$wbwindow), this.initUIEventsOverrides(), this.initDocWriteOpenCloseOverride(), this.initEvalOverride(), this.initHTTPOverrides(), this.initAudioOverride(), this.initFontFaceOverride(this.$wbwindow), this.initWorkerOverrides(), this.initTextNodeOverrides(), this.initCSSOMOverrides(), this.overrideHtmlAssign(this.$wbwindow.Element, "innerHTML", true), this.overrideHtmlAssign(this.$wbwindow.Element, "outerHTML", true), this.overrideHtmlAssignSrcDoc(this.$wbwindow.HTMLIFrameElement, "srcdoc", true), this.overrideHtmlAssign(this.$wbwindow.HTMLStyleElement, "textContent"), this.overrideShadowDom(), this.overridePropExtract(this.$wbwindow.Document.prototype, "URL"), this.overridePropExtract(this.$wbwindow.Document.prototype, "documentURI"), this.overridePropExtract(this.$wbwindow.Node.prototype, "baseURI"), this.overrideAttrProps(), this.overrideDataSet(), this.initInsertAdjacentElementHTMLOverrides(), this.overrideIframeContentAccess("contentWindow"), this.overrideIframeContentAccess("contentDocument"), this.initIntersectionObsOverride(), this.overrideFuncArgProxyToObj(this.$wbwindow.MutationObserver, "observe"), this.overrideFuncArgProxyToObj(this.$wbwindow.Node, "compareDocumentPosition"), this.overrideFuncArgProxyToObj(this.$wbwindow.Node, "contains"), this.overrideFuncArgProxyToObj(this.$wbwindow.Document, "createTreeWalker"), this.overrideFuncArgProxyToObj(this.$wbwindow.Document, "evaluate", 1), this.overrideFuncArgProxyToObj(this.$wbwindow.XSLTProcessor, "transformToFragment", 1), this.overrideFuncThisProxyToObj(this.$wbwindow, "getComputedStyle", this.$wbwindow), this.overrideFuncThisProxyToObj(this.$wbwindow, "clearTimeout"), this.overrideFuncThisProxyToObj(this.$wbwindow, "clearInterval"), this.overrideFuncThisProxyToObj(this.$wbwindow.EventTarget.prototype, "dispatchEvent"), this.initTimeoutIntervalOverrides(), this.overrideFramesAccess(this.$wbwindow), this.overrideSWAccess(this.$wbwindow), this.initElementGetSetAttributeOverride(), this.initSvgImageOverrides(), this.initAttrOverrides(), this.initCookiesOverride(), this.initCreateElementNSFix(), this.wb_opts.skip_dom || this.initDomOverride(), this.initRegisterUnRegPHOverride(), this.initPresentationRequestOverride(), this.initBeaconOverride(), this.initMiscNavigatorOverrides(), this.initSeededRandom(this.wb_info.wombat_sec), this.initCryptoRandom(), this.initFixedRatio(this.wb_info.pixel_ratio || 1), this.initDateOverride(this.wb_info.wombat_sec), this.initBlobOverride(), this.initWSOverride(), this.initOpenOverride(), this.initDisableNotificationsGeoLocation(), this.initStorageOverride(), this.initCachesOverride(), this.initIndexedDBOverride(), this.initWindowObjProxy(this.$wbwindow), this.initDocumentObjProxy(this.$wbwindow.document);
         var wombat = this;
         return {
             extract_orig: this.extractOriginalURL,
             rewrite_url: this.rewriteUrl,
             watch_elem: this.watchElem,
             init_new_window_wombat: this.initNewWindowWombat,
             init_paths: this.initPaths,
```

### Comparing `pywb-2.7.4/pywb/static/wombatProxyMode.js` & `pywb-2.8.0/pywb/static/wombatProxyMode.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 /*
 Wombat.js client-side rewriting engine for web archive replay
-Copyright (C) 2014-2023 Webrecorder Software, Rhizome, and Contributors. Released under the GNU Affero General Public License.
+Copyright (C) 2014-2024 Webrecorder Software, Rhizome, and Contributors. Released under the GNU Affero General Public License.
 
 This file is part of wombat.js, see https://github.com/webrecorder/wombat.js for the full source
 Wombat.js is part of the Webrecorder project (https://github.com/webrecorder)
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU Affero General Public License as published
 by the Free Software Foundation, either version 3 of the License, or
```

### Comparing `pywb-2.7.4/pywb/static/wombatWorkers.js` & `pywb-2.8.0/pywb/static/wombatWorkers.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 /*
 Wombat.js client-side rewriting engine for web archive replay
-Copyright (C) 2014-2023 Webrecorder Software, Rhizome, and Contributors. Released under the GNU Affero General Public License.
+Copyright (C) 2014-2024 Webrecorder Software, Rhizome, and Contributors. Released under the GNU Affero General Public License.
 
 This file is part of wombat.js, see https://github.com/webrecorder/wombat.js for the full source
 Wombat.js is part of the Webrecorder project (https://github.com/webrecorder)
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU Affero General Public License as published
 by the Free Software Foundation, either version 3 of the License, or
```

### Comparing `pywb-2.7.4/pywb/templates/banner.html` & `pywb-2.8.0/pywb/templates/banner.html`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/templates/base.html` & `pywb-2.8.0/pywb/templates/base.html`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/templates/error.html` & `pywb-2.8.0/pywb/templates/error.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% extends "base.html" %}
 {% block title %}{{ _('Pywb Error') }}{% endblock %}
 {% block body %}
 <div class="container text-danger error">
     <div class="row justify-content-center">
-        <h2 class="display-2">Pywb Error</h2>
+        <h2 class="display-2">{{ _('Pywb Error') }}</h2>
     </div>
     <div class="row">
         <div class="col-12 text-center">
         {% if err_status == 451 %}
             <p class="lead">{% trans %}Access Blocked to {{ err_msg }}{% endtrans %}</p>
 
         {% elif err_status == 404 and err_details == 'coll_not_found' %}
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {% extends "base.html" %} {% block title %}{{ _('Pywb Error') }}{% endblock %}
 {% block body %}
-********** PPyywwbb EErrrroorr **********
+********** {{{{ __((''PPyywwbb EErrrroorr'')) }}}} **********
 {% if err_status == 451 %}
 {% trans %}Access Blocked to {{ err_msg }}{% endtrans %}
 {% elif err_status == 404 and err_details == 'coll_not_found' %}
 {% trans %}Collection not found: {{{{ eerrrr__mmssgg }}}}{{%% eennddttrraannss %%}}
 _{_{_ ___(_'_S_e_e_ _l_i_s_t_ _o_f_ _v_a_l_i_d_ _c_o_l_l_e_c_t_i_o_n_s_'_)_ _}_}
 {% elif err_status == 404 and err_details == 'static_file_not_found' %}
 {% trans %}Static file not found: {{{{ eerrrr__mmssgg }}}}{{%% eennddttrraannss %%}}
```

### Comparing `pywb-2.7.4/pywb/templates/frame_insert.html` & `pywb-2.8.0/pywb/templates/frame_insert.html`

 * *Files 19% similar despite different names*

```diff
@@ -21,16 +21,29 @@
 {% include 'vue_loc.html' %}
 
 </head>
 <body style="margin: 0px; padding: 0px;">
 
 <div id="app" style="width: 100%; height: 200px"></div>
 <script>
-    VueUI.main("{{ static_prefix }}", "{{ url }}", "{{ wb_prefix }}", "{{ timestamp }}", "{{ ui.logo }}", "{{ ui.navbar_background_hex | default('f8f9fa') }}", "{{ ui.navbar_color_hex | default('212529') }}", "{{ ui.navbar_light_buttons }}", "{{ env.pywb_lang | default('en') }}",
-      allLocales, i18nStrings, "{{ ui.logo_home_url }}");
+  VueUI.main({
+      staticPrefix: "{{ static_prefix }}",
+      url: "{{ url }}",
+      prefix: "{{ wb_prefix }}",
+      timestamp: "{{ timestamp }}",
+      logoUrl: "{{ ui.logo }}",
+      navbarBackground: "{{ ui.navbar_background_hex | default('f8f9fa') }}",
+      navbarColor: "{{ ui.navbar_color_hex | default('212529') }}",
+      navbarLightButtons: "{{ ui.navbar_light_buttons }}",
+      logoHomeUrl: "{{ ui.logo_home_url }}",
+      disablePrinting: "{{ ui.disable_printing }}",
+      allLocales: allLocales
+    },
+    "{{ env.pywb_lang | default('en') }}",
+    i18nStrings);
 </script>
 
 <div id="wb_iframe_div">
 <iframe id="replay_iframe" frameborder="0" seamless="seamless" scrolling="yes" class="wb_iframe" allow="autoplay; fullscreen"></iframe>
 </div>
 <script>
   var cframe = new ContentFrame({"url": "{{ url }}" + window.location.hash,
```

### Comparing `pywb-2.7.4/pywb/templates/head_insert.html` & `pywb-2.8.0/pywb/templates/head_insert.html`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/templates/header.html` & `pywb-2.8.0/pywb/templates/header.html`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/templates/index.html` & `pywb-2.8.0/pywb/templates/index.html`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/templates/instructions.html` & `pywb-2.8.0/pywb/templates/instructions.html`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/templates/not_found.html` & `pywb-2.8.0/pywb/templates/not_found.html`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/templates/proxy_cert_download.html` & `pywb-2.8.0/pywb/templates/proxy_cert_download.html`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/templates/proxy_select.html` & `pywb-2.8.0/pywb/templates/proxy_select.html`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/templates/query.html` & `pywb-2.8.0/pywb/templates/query.html`

 * *Files 6% similar despite different names*

```diff
@@ -90,14 +90,27 @@
 </script>
 
 {% else %}
 
 <div id="app" style="width: 100%; height: 100%"></div>
 
 <script>
-  VueUI.main("{{ static_prefix }}", "{{ url }}", "{{ prefix }}", undefined, "{{ ui.logo }}", "{{ ui.navbar_background_hex | default('f8f9fa') }}", "{{ ui.navbar_color_hex | default('212529') }}", "{{ ui.navbar_light_buttons }}", "{{ env.pywb_lang | default('en') }}",
-      allLocales, i18nStrings, "{{ ui.logo_home_url }}");
+  VueUI.main({
+      staticPrefix: "{{ static_prefix }}",
+      url: "{{ url }}",
+      prefix: "{{ prefix }}",
+      timestamp: undefined,
+      logoUrl: "{{ ui.logo }}",
+      navbarBackground: "{{ ui.navbar_background_hex | default('f8f9fa') }}",
+      navbarColor: "{{ ui.navbar_color_hex | default('212529') }}",
+      navbarLightButtons: "{{ ui.navbar_light_buttons }}",
+      logoHomeUrl: "{{ ui.logo_home_url }}",
+      disablePrinting: "{{ ui.disable_printing }}",
+      allLocales: allLocales
+    },
+    "{{ env.pywb_lang | default('en') }}",
+    i18nStrings);
 </script>
 
 {% endif %}
 
 {% endblock %}
```

### Comparing `pywb-2.7.4/pywb/templates/search.html` & `pywb-2.8.0/pywb/templates/search.html`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/templates/vue_loc.html` & `pywb-2.8.0/pywb/templates/vue_loc.html`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         "All-time": "{{ _Q('All-time') }}",
         "Show timeline":"{{ _Q('Show timeline') }}",
         "Hide timeline":"{{ _Q('Hide timeline') }}",
         "Show calendar":"{{ _Q('Show calendar') }}",
         "Hide calendar":"{{ _Q('Hide calendar') }}",
         "Previous capture":"{{ _Q('Previous capture') }}",
         "Next capture":"{{ _Q('Next capture') }}",
+        "Print":"{{ _Q('Print') }}",
         "Select language":"{{ _Q('Select language') }}",
         "View capture on {date}":"{{ _Q('View capture on {date}') }}",
         "{count} capture":"{{ _Q('{count} capture') }}",
         "{count} captures":"{{ _Q('{count} captures') }}",
         "{capture_text} on {date}":"{{ _Q('{capture_text} on {date}') }}",
         "{capture_text} in {month}":"{{ _Q('{capture_text} in {month}') }}",
         "current":"{{ _Q('current') }}", // translators: current capture in list of captures
```

### Comparing `pywb-2.7.4/pywb/utils/README.md` & `pywb-2.8.0/pywb/utils/README.md`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/utils/binsearch.py` & `pywb-2.8.0/pywb/utils/binsearch.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,11 +146,11 @@
 
 
 #=================================================================
 def iter_exact(reader, key, token=b' '):
     """
     Create an iterator which iterates over lines where the first field matches
     the 'key', equivalent to token + sep prefix.
-    Default field termin_ator/seperator is ' '
+    Default field termin_ator/separator is ' '
     """
 
     return iter_prefix(reader, key + token)
```

### Comparing `pywb-2.7.4/pywb/utils/canonicalize.py` & `pywb-2.8.0/pywb/utils/canonicalize.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/utils/format.py` & `pywb-2.8.0/pywb/utils/format.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/utils/geventserver.py` & `pywb-2.8.0/pywb/utils/geventserver.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/utils/io.py` & `pywb-2.8.0/pywb/utils/io.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/utils/loaders.py` & `pywb-2.8.0/pywb/utils/loaders.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/utils/memento.py` & `pywb-2.8.0/pywb/utils/memento.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/utils/merge.py` & `pywb-2.8.0/pywb/utils/merge.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/utils/test/test_binsearch.py` & `pywb-2.8.0/pywb/utils/test/test_binsearch.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/utils/test/test_loaders.py` & `pywb-2.8.0/pywb/utils/test/test_loaders.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/utils/wbexception.py` & `pywb-2.8.0/pywb/utils/wbexception.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/vueui/src/cdx-simulator/README.md` & `pywb-2.8.0/pywb/vueui/src/cdx-simulator/README.md`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/access_checker.py` & `pywb-2.8.0/pywb/warcserver/access_checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,14 +256,18 @@
 
             if key_exact == acl_key:
                 acl_obj = CDXObject(acl)
 
             if key.startswith(acl_key):
                 acl_obj = CDXObject(acl)
 
+            # Check for "*," in ACL, which matches any URL
+            if acl_key == b"*,":
+                acl_obj = CDXObject(acl)
+
             if acl_obj:
                 user = acl_obj.get('user')
                 if user == acl_user:
                     return acl_obj
                 elif not user:
                     last_key = acl_key
                     last_obj = acl_obj
```

### Comparing `pywb-2.7.4/pywb/warcserver/amf.py` & `pywb-2.8.0/pywb/warcserver/amf.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/basewarcserver.py` & `pywb-2.8.0/pywb/warcserver/basewarcserver.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/handlers.py` & `pywb-2.8.0/pywb/warcserver/handlers.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/http.py` & `pywb-2.8.0/pywb/warcserver/http.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/index/aggregator.py` & `pywb-2.8.0/pywb/warcserver/index/aggregator.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/index/cdxobject.py` & `pywb-2.8.0/pywb/warcserver/index/cdxobject.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/index/cdxops.py` & `pywb-2.8.0/pywb/warcserver/index/cdxops.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/index/fuzzymatcher.py` & `pywb-2.8.0/pywb/warcserver/index/fuzzymatcher.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/index/indexsource.py` & `pywb-2.8.0/pywb/warcserver/index/indexsource.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/index/query.py` & `pywb-2.8.0/pywb/warcserver/index/query.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/index/test/test_cdxobject.py` & `pywb-2.8.0/pywb/warcserver/index/test/test_cdxobject.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/index/test/test_cdxops.py` & `pywb-2.8.0/pywb/warcserver/index/test/test_cdxops.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/index/test/test_dir_agg.py` & `pywb-2.8.0/pywb/warcserver/index/test/test_dir_agg.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/index/test/test_fuzzymatcher.py` & `pywb-2.8.0/pywb/warcserver/index/test/test_fuzzymatcher.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/index/test/test_indexsource.py` & `pywb-2.8.0/pywb/warcserver/index/test/test_indexsource.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/index/test/test_lazy_ops.py` & `pywb-2.8.0/pywb/warcserver/index/test/test_lazy_ops.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/index/test/test_memento_agg.py` & `pywb-2.8.0/pywb/warcserver/index/test/test_memento_agg.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/index/test/test_redis_agg.py` & `pywb-2.8.0/pywb/warcserver/index/test/test_redis_agg.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/index/test/test_timeouts.py` & `pywb-2.8.0/pywb/warcserver/index/test/test_timeouts.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/index/test/test_xmlquery_indexsource.py` & `pywb-2.8.0/pywb/warcserver/index/test/test_xmlquery_indexsource.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/index/test/test_zipnum.py` & `pywb-2.8.0/pywb/warcserver/index/test/test_zipnum.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/index/zipnum.py` & `pywb-2.8.0/pywb/warcserver/index/zipnum.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/inputrequest.py` & `pywb-2.8.0/pywb/warcserver/inputrequest.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/resource/blockrecordloader.py` & `pywb-2.8.0/pywb/warcserver/resource/blockrecordloader.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/resource/pathresolvers.py` & `pywb-2.8.0/pywb/warcserver/resource/pathresolvers.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/resource/resolvingloader.py` & `pywb-2.8.0/pywb/warcserver/resource/resolvingloader.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/resource/responseloader.py` & `pywb-2.8.0/pywb/warcserver/resource/responseloader.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/resource/test/test_loading.py` & `pywb-2.8.0/pywb/warcserver/resource/test/test_loading.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/resource/test/test_pathresolvers.py` & `pywb-2.8.0/pywb/warcserver/resource/test/test_pathresolvers.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/test/test_access.py` & `pywb-2.8.0/pywb/warcserver/test/test_access.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/test/test_amf.py` & `pywb-2.8.0/pywb/warcserver/test/test_amf.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/test/test_handlers.py` & `pywb-2.8.0/pywb/warcserver/test/test_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -381,16 +381,15 @@
         resp = self.testapp.get('/urlagnost/resource?url=http://example.com/&param.arg=foo')
 
         assert resp.status_int == 200
         assert resp.headers['Link'] == MementoUtils.make_link('http://test@example.com/', 'original')
         assert resp.headers['Warcserver-Source-Coll'] == 'url-agnost'
         assert resp.headers['Memento-Datetime'] == 'Mon, 29 Jul 2013 19:51:51 GMT'
 
-    #@pytest.mark.skipif(os.environ.get('CI') is not None, reason='Skip Test on CI')
-    @pytest.mark.skip("youtube-dl update needed")
+    @pytest.mark.skipif(os.environ.get('CI') is not None, reason='Skip Test on CI')
     def test_live_video_loader(self):
         pytest.importorskip('youtube_dl')
         params = {'url': 'http://www.youtube.com/v/BfBgWtAIbRc',
                   'content_type': 'application/vnd.youtube-dl_formats+json'
                  }
 
         resp = self.testapp.get('/live/resource', params=params)
@@ -401,16 +400,15 @@
 
         assert resp.headers['Link'] == MementoUtils.make_link('metadata://www.youtube.com/v/BfBgWtAIbRc', 'original')
         assert resp.headers['Memento-Datetime'] != ''
 
         assert b'WARC-Type: metadata' in resp.body
         assert b'Content-Type: application/vnd.youtube-dl_formats+json' in resp.body
 
-    #@pytest.mark.skipif(os.environ.get('CI') is not None, reason='Skip Test on CI')
-    @pytest.mark.skip("youtube-dl update needed")
+    @pytest.mark.skipif(os.environ.get('CI') is not None, reason='Skip Test on CI')
     def test_live_video_loader_post(self):
         pytest.importorskip('youtube_dl')
         req_data = """\
 GET /v/BfBgWtAIbRc HTTP/1.1
 accept-encoding: gzip, deflate
 accept: */*
 host: www.youtube.com\
```

### Comparing `pywb-2.7.4/pywb/warcserver/test/test_inputreq.py` & `pywb-2.8.0/pywb/warcserver/test/test_inputreq.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         start_response('200 OK', [('Content-Type', 'text/plain; charset=utf-8')])
         return [result]
 
 
 
 #=============================================================================
 class TestInputReq(object):
-    def setup(self):
+    def setup_method(self):
         self.app = InputReqApp()
         self.testapp = webtest.TestApp(self.app)
 
     def test_get_direct(self):
         res = self.testapp.get('/test/http://example.com/', headers={'Foo': 'Bar'})
         assert res.text == '\
 GET /test/http://example.com/ HTTP/1.0\r\n\
```

### Comparing `pywb-2.7.4/pywb/warcserver/test/test_upstream.py` & `pywb-2.8.0/pywb/warcserver/test/test_upstream.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from pywb.warcserver.upstreamindexsource import UpstreamMementoIndexSource, UpstreamAggIndexSource
 
 from .testutils import LiveServerTests, HttpBinLiveTests, BaseTestClass
 
 
 class TestUpstream(LiveServerTests, HttpBinLiveTests, BaseTestClass):
-    def setup(self):
+    def setup_method(self):
         app = BaseWarcServer()
 
         base_url = 'http://localhost:{0}'.format(self.server.port)
         app.add_route('/upstream',
             DefaultResourceHandler(SimpleAggregator(
                            {'upstream': UpstreamAggIndexSource(base_url + '/live')})
             )
```

### Comparing `pywb-2.7.4/pywb/warcserver/test/test_warcserver.py` & `pywb-2.8.0/pywb/warcserver/test/test_warcserver.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/test/test_warcserver_config.yaml` & `pywb-2.8.0/pywb/warcserver/test/test_warcserver_config.yaml`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/test/testutils.py` & `pywb-2.8.0/pywb/warcserver/test/testutils.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/upstreamindexsource.py` & `pywb-2.8.0/pywb/warcserver/upstreamindexsource.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb/warcserver/warcserver.py` & `pywb-2.8.0/pywb/warcserver/warcserver.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/pywb.egg-info/PKG-INFO` & `pywb-2.8.0/pywb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 Metadata-Version: 2.1
 Name: pywb
-Version: 2.7.4
+Version: 2.8.0
 Summary: Pywb Webrecorder web archive replay and capture tools
 Home-page: https://github.com/webrecorder/pywb
 Author: Ilya Kreymer
 Author-email: ikreymer@gmail.com
 License: GPL
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: Proxy Servers
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Server
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving
 Classifier: Topic :: System :: Archiving :: Backup
 Classifier: Topic :: Utilities
+Requires-Python: >=3.7,<3.12
 Provides-Extra: i18n
 License-File: LICENSE
 License-File: NOTICE
 
-Webrecorder pywb 2.7
+Webrecorder pywb 2.8
 ====================
 
 .. image:: https://raw.githubusercontent.com/webrecorder/pywb/main/pywb/static/pywb-logo.png
 
 .. image:: https://github.com/webrecorder/pywb/workflows/CI/badge.svg
       :target: https://github.com/webrecorder/pywb/actions
 .. image:: https://codecov.io/gh/webrecorder/pywb/branch/main/graph/badge.svg
@@ -93,27 +90,23 @@
 
 
 Installation for Deployment
 ---------------------------
 
 To install pywb for usage, you can use:
 
-```shell
-pip install pywb
-```
+``pip install pywb``
 
 Note: depending on your Python installation, you may have to use `pip3` instead of `pip`.
 
 
 Installation from local copy
 ----------------------------
 
-```shell
-git clone https://github.com/webrecorder/pywb
-```
+``git clone https://github.com/webrecorder/pywb``
 
 To install from a locally cloned copy, install with ``pip install -e .`` or ``python setup.py install``.
 
 To run tests, we recommend installing ``pip install tox tox-current-env`` and then running ``tox --current-env`` to test in your current Python environment.
 
 To Build docs locally, run:  ``cd docs; make html``. (The docs will be built in ``./_build/html/index.html``)
```

### Comparing `pywb-2.7.4/pywb.egg-info/SOURCES.txt` & `pywb-2.8.0/pywb.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -127,31 +127,28 @@
 pywb/rewrite/test/test_html_insert_rewriter.py
 pywb/rewrite/test/test_html_rewriter.py
 pywb/rewrite/test/test_jsonp_rewriter.py
 pywb/rewrite/test/test_regex_rewriters.py
 pywb/rewrite/test/test_url_rewriter.py
 pywb/rewrite/test/test_wburl.py
 pywb/static/autoFetchWorker.js
-pywb/static/calendar-icon.png
 pywb/static/calendar.svg
 pywb/static/pywb-logo-sm.png
 pywb/static/pywb-logo.png
 pywb/static/query.js
 pywb/static/queryWorker.js
 pywb/static/scroll-webkit.css
 pywb/static/search.js
-pywb/static/timeline-icon.png
 pywb/static/transclusions.js
 pywb/static/vidrw.js
 pywb/static/vue_banner.css
 pywb/static/wb_frame.js
 pywb/static/wombat.js
 pywb/static/wombatProxyMode.js
 pywb/static/wombatWorkers.js
-pywb/static/zoom-out-icon-333316.png
 pywb/static/css/base.css
 pywb/static/css/bootstrap.min.css
 pywb/static/css/font-awesome.min.css
 pywb/static/css/query.css
 pywb/static/flowplayer/flowplayer-3.2.18.swf
 pywb/static/flowplayer/flowplayer.audio-3.2.11.swf
 pywb/static/flowplayer/flowplayer.controls-3.2.16.swf
@@ -259,14 +256,15 @@
 pywb/warcserver/test/test_amf.py
 pywb/warcserver/test/test_handlers.py
 pywb/warcserver/test/test_inputreq.py
 pywb/warcserver/test/test_upstream.py
 pywb/warcserver/test/test_warcserver.py
 pywb/warcserver/test/test_warcserver_config.yaml
 pywb/warcserver/test/testutils.py
+sample_archive/access/allow_all.aclj
 sample_archive/access/allows.aclj
 sample_archive/access/blocks.aclj
 sample_archive/access/list1.aclj
 sample_archive/access/list2.aclj
 sample_archive/access/pywb.aclj
 sample_archive/access/single-line.aclj
 sample_archive/cdx/bad.cdx
@@ -277,14 +275,15 @@
 sample_archive/cdx/httpbin-resource.cdxj
 sample_archive/cdx/iana.cdx
 sample_archive/cdx/missing-status-text.cdxj
 sample_archive/cdx/post-test.cdx
 sample_archive/cdx/url-agnost-example.cdx
 sample_archive/cdxj/dupes.cdxj
 sample_archive/cdxj/example-no-digest.cdxj
+sample_archive/cdxj/example.cdx.gz
 sample_archive/cdxj/example.cdxj
 sample_archive/cdxj/example2.cdxj
 sample_archive/cdxj/iana.cdxj
 sample_archive/cdxj/post-test.cdxj
 sample_archive/cdxj/url-agnost-example.cdxj
 sample_archive/non-surt-cdx/example-non-surt.cdx
 sample_archive/text_content/link_headers.yaml
@@ -337,14 +336,15 @@
 tests/test_cert_req.py
 tests/test_cli.py
 tests/test_embargo.py
 tests/test_force_https.py
 tests/test_integration.py
 tests/test_live_rewriter.py
 tests/test_locales.py
+tests/test_manager.py
 tests/test_memento.py
 tests/test_prefer_header.py
 tests/test_prefixed_deploy.py
 tests/test_proxy.py
 tests/test_range.py
 tests/test_record_dedup.py
 tests/test_record_replay.py
```

### Comparing `pywb-2.7.4/sample_archive/access/pywb.aclj` & `pywb-2.8.0/sample_archive/access/pywb.aclj`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 org,iana)/exact/match/first/line/aclj### - {"access": "allow", "url": "https://www.iana.org/exact/match/first/line/aclj/"}
 org,iana)/about - {"access": "block"}
 org,iana)/about - {"access": "allow", "user": "staff"}
 org,iana)/_css/2013.1/fonts/opensans-semibold.ttf - {"access": "allow"}
 org,iana)/_css - {"access": "exclude"}
 org,iana)/### - {"access": "allow"}
 org,iana)/ - {"access": "exclude"}
+com,example)/?example=3 - {"access": "block", "user": "staff"}
+com,example)/?example=3 - {"access": "exclude", "user": "staff2"}
 org,example)/?example=1 - {"access": "block"}
 com,example)/?example=2 - {"access": "allow_ignore_embargo"}
 com,example)/?example=1 - {"access": "allow_ignore_embargo", "user": "staff2"}
 com,example)/?example=1 - {"access": "allow", "user": "staff"}
 com,example)/ - {"access": "allow"}
```

### Comparing `pywb-2.7.4/sample_archive/cdx/bad.cdx` & `pywb-2.8.0/sample_archive/cdx/bad.cdx`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/sample_archive/cdx/dupes.cdx` & `pywb-2.8.0/sample_archive/cdx/dupes.cdx`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/sample_archive/cdx/iana.cdx` & `pywb-2.8.0/sample_archive/cdx/iana.cdx`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/sample_archive/cdx/post-test.cdx` & `pywb-2.8.0/sample_archive/cdx/post-test.cdx`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/sample_archive/cdxj/dupes.cdxj` & `pywb-2.8.0/sample_archive/cdxj/dupes.cdxj`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/sample_archive/cdxj/example.cdxj` & `pywb-2.8.0/sample_archive/cdxj/example.cdxj`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/sample_archive/cdxj/iana.cdxj` & `pywb-2.8.0/sample_archive/cdxj/iana.cdxj`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/sample_archive/cdxj/post-test.cdxj` & `pywb-2.8.0/sample_archive/cdxj/post-test.cdxj`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/sample_archive/text_content/link_headers.yaml` & `pywb-2.8.0/sample_archive/text_content/link_headers.yaml`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/sample_archive/text_content/sample_dash.mpd` & `pywb-2.8.0/sample_archive/text_content/sample_dash.mpd`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/sample_archive/text_content/sample_hls.m3u8` & `pywb-2.8.0/sample_archive/text_content/sample_hls.m3u8`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/sample_archive/warcs/dupes.warc.gz` & `pywb-2.8.0/sample_archive/warcs/dupes.warc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/sample_archive/warcs/example-bad.warc.gz.bad` & `pywb-2.8.0/sample_archive/warcs/example-bad.warc.gz.bad`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/sample_archive/warcs/example-extra.warc` & `pywb-2.8.0/sample_archive/warcs/example-extra.warc`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/sample_archive/warcs/example-url-agnostic-orig.warc.gz` & `pywb-2.8.0/sample_archive/warcs/example-url-agnostic-orig.warc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/sample_archive/warcs/example-url-agnostic-revisit.warc.gz` & `pywb-2.8.0/sample_archive/warcs/example-url-agnostic-revisit.warc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/sample_archive/warcs/example-wget-1-14.warc.gz` & `pywb-2.8.0/sample_archive/warcs/example-wget-1-14.warc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/sample_archive/warcs/example-wpull.warc.gz` & `pywb-2.8.0/sample_archive/warcs/example-wpull.warc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/sample_archive/warcs/example.arc` & `pywb-2.8.0/sample_archive/warcs/example.arc`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/sample_archive/warcs/example.arc.gz` & `pywb-2.8.0/sample_archive/warcs/example.arc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/sample_archive/warcs/example.warc` & `pywb-2.8.0/sample_archive/warcs/example.warc`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/sample_archive/warcs/example.warc.gz` & `pywb-2.8.0/sample_archive/warcs/example.warc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/sample_archive/warcs/example2.warc.gz` & `pywb-2.8.0/sample_archive/warcs/example2.warc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/sample_archive/warcs/iana.warc.gz` & `pywb-2.8.0/sample_archive/warcs/iana.warc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/sample_archive/warcs/post-test.warc.gz` & `pywb-2.8.0/sample_archive/warcs/post-test.warc.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/sample_archive/zipcdx/zipnum-sample.cdx.gz` & `pywb-2.8.0/sample_archive/zipcdx/zipnum-sample.cdx.gz`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/sample_archive/zipcdx/zipnum-sample.idx` & `pywb-2.8.0/sample_archive/zipcdx/zipnum-sample.idx`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/setup.py` & `pywb-2.8.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,14 +109,15 @@
     install_requires=load_requirements('requirements.txt'),
     extras_require={
         "i18n":  [
             "babel",
             "translate_toolkit"
         ],
     },
+    python_requires='>=3.7,<3.12',
     tests_require=load_requirements("test_requirements.txt"),
     cmdclass={'test': PyTest},
     test_suite='',
     entry_points="""
         [console_scripts]
         pywb = pywb.apps.cli:wayback
         wayback = pywb.apps.cli:wayback
@@ -127,24 +128,20 @@
         warcserver = pywb.apps.cli:warcserver
         """,
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: Web Environment',
         'License :: OSI Approved :: GNU General Public License (GPL)',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Internet :: Proxy Servers',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Internet :: WWW/HTTP :: WSGI',
         'Topic :: Internet :: WWW/HTTP :: WSGI :: Application',
         'Topic :: Internet :: WWW/HTTP :: WSGI :: Middleware',
         'Topic :: Internet :: WWW/HTTP :: WSGI :: Server',
         'Topic :: Software Development :: Libraries :: Python Modules',
```

### Comparing `pywb-2.7.4/tests/base_config_test.py` & `pywb-2.8.0/tests/base_config_test.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests/config_test.yaml` & `pywb-2.8.0/tests/config_test.yaml`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests/config_test_access.yaml` & `pywb-2.8.0/tests/config_test_access.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -58,10 +58,17 @@
         embargo:
             older:
                 years: 1
 
         acl_paths:
             - ./sample_archive/access/pywb.aclj
 
+    pywb-wildcard-surt:
+        index_paths: ./sample_archive/cdx/
+        archive_paths: ./sample_archive/warcs/
+        default_access: block
+        acl_paths:
+            - ./sample_archive/access/allow_all.aclj
+
```

### Comparing `pywb-2.7.4/tests/i18n-data/l337/LC_MESSAGES/messages.po` & `pywb-2.8.0/tests/i18n-data/l337/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests/memento_fixture.py` & `pywb-2.8.0/tests/memento_fixture.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests/test_acl.py` & `pywb-2.8.0/tests/test_acl.py`

 * *Files 20% similar despite different names*

```diff
@@ -37,20 +37,31 @@
         assert len(resp.text.splitlines()) == 1
 
         resp = self.testapp.get('/pywb/mp_/http://www.iana.org/about/', status=451)
 
         assert 'Access Blocked' in resp.text
 
     def test_allow_via_acl_header(self):
-        resp = self.query('http://www.iana.org/about/')
-
+        resp = self.testapp.get('/pywb/cdx?url=http://www.iana.org/about/', headers={"X-Pywb-Acl-User": "staff"})
         assert len(resp.text.splitlines()) == 1
 
         resp = self.testapp.get('/pywb/mp_/http://www.iana.org/about/', headers={"X-Pywb-Acl-User": "staff"}, status=200)
 
+    def test_block_via_acl_header(self):
+        resp = self.testapp.get('/pywb/cdx?url=http://example.com/?example=3', headers={"X-Pywb-Acl-User": "staff"})
+        assert len(resp.text.splitlines()) > 0
+
+        resp = self.testapp.get('/pywb/mp_/http://example.com/?example=3', headers={"X-Pywb-Acl-User": "staff"}, status=451)
+
+    def test_exclude_via_acl_header(self):
+        resp = self.testapp.get('/pywb/cdx?url=http://example.com/?example=3', headers={"X-Pywb-Acl-User": "staff2"})
+        assert len(resp.text.splitlines()) == 0
+
+        resp = self.testapp.get('/pywb/mp_/http://example.com/?example=3', headers={"X-Pywb-Acl-User": "staff2"}, status=404)
+
     def test_allowed_more_specific(self):
         resp = self.query('http://www.iana.org/_css/2013.1/fonts/opensans-semibold.ttf')
 
         assert resp.status_code == 200
 
         assert len(resp.text.splitlines()) > 0
 
@@ -81,9 +92,13 @@
 
         assert len(resp.text.splitlines()) > 0
 
         resp = self.testapp.get('/pywb-acl-dir/mp_/http://httpbin.org/anything/resource.json')
 
         assert '"http://httpbin.org/anything/resource.json"' in resp.text
 
+    def test_allow_all_acl_user_specific(self):
+        resp = self.testapp.get('/pywb-wildcard-surt/mp_/http://example.com/', status=451)
 
+        assert 'Access Blocked' in resp.text
 
+        resp = self.testapp.get('/pywb-wildcard-surt/mp_/http://example.com/', headers={"X-Pywb-Acl-User": "staff"}, status=200)
```

### Comparing `pywb-2.7.4/tests/test_acl_manager.py` & `pywb-2.8.0/tests/test_acl_manager.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests/test_auto_colls.py` & `pywb-2.8.0/tests/test_auto_colls.py`

 * *Files 0% similar despite different names*

```diff
@@ -533,15 +533,15 @@
             main(['template', '--remove', 'query_html'])
 
         # already removed
         with raises(IOError):
             main(['template', 'foo', '--remove', 'query_html'])
 
     def test_err_no_such_coll(self):
-        """ Test error adding warc to non-existant collection
+        """ Test error adding warc to non-existent collection
         """
         warc1 = self._get_sample_warc('example.warc.gz')
 
         with raises(IOError):
             main(['add', 'bar', warc1])
 
     def test_err_wrong_warcs(self):
```

### Comparing `pywb-2.7.4/tests/test_cdx_server_app.py` & `pywb-2.8.0/tests/test_cdx_server_app.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests/test_cert_req.py` & `pywb-2.8.0/tests/test_cert_req.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests/test_cli.py` & `pywb-2.8.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests/test_embargo.py` & `pywb-2.8.0/tests/test_embargo.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,19 @@
         # ignore embargo
         resp = self.testapp.get('/pywb-embargo-acl/20140126201054mp_/http://example.com/?example=2', status=200)
 
 
     def test_embargo_ignore_acl_with_header_only(self):
         # ignore embargo with custom header only
         headers = {"X-Pywb-ACL-User": "staff2"}
-        resp = self.testapp.get('/pywb-embargo-acl/20140126201054mp_/http://example.com/?example=1', status=200, headers=headers)
 
+        resp = self.testapp.get('/pywb-embargo-acl/cdx?url=http://example.com/?example=1', headers=headers)
+        assert len(resp.text.splitlines()) > 0
+        resp = self.testapp.get('/pywb-embargo-acl/20140126201054mp_/http://example.com/?example=1', status=200, headers=headers)
+        resp = self.testapp.get('/pywb-embargo-acl/cdx?url=http://example.com/?example=1')
+        assert len(resp.text.splitlines()) == 0
         resp = self.testapp.get('/pywb-embargo-acl/20140126201054mp_/http://example.com/?example=1', status=404)
```

### Comparing `pywb-2.7.4/tests/test_force_https.py` & `pywb-2.8.0/tests/test_force_https.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,10 +52,10 @@
     def setup_class(cls):
         super(TestForceHttpsRoot, cls).setup_class('config_test_root_coll.yaml')
 
     def test_force_https_root_replay_1(self, fmod):
         resp = self.get('/20140128051539{0}/http://www.iana.org/domains/example', fmod,
                         headers={'X-Forwarded-Proto': 'https'})
 
-        assert resp.headers['Location'] == 'https://localhost:80/20140128051539{0}/http://www.iana.org/domains/reserved'.format(fmod)
+        assert resp.headers['Location'] == 'https://localhost:80/20140128051539{0}/http://www.iana.org/help/example-domains'.format(fmod)
```

### Comparing `pywb-2.7.4/tests/test_integration.py` & `pywb-2.8.0/tests/test_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,25 +396,25 @@
 
     def test_non_exact_replay_skip_self_redir_slash(self, fmod):
         uri = '/pywb/20140126200927{0}/http://www.iana.org/domains/root/db/'
         resp = self.get(uri, fmod)
         assert resp.status_int == 200
         assert resp.headers['Content-Location'].endswith('/pywb/20140126200928{0}/http://www.iana.org/domains/root/db'.format(fmod))
 
-    def test_not_existant_warc_other_capture(self, fmod):
+    def test_not_existent_warc_other_capture(self, fmod):
         resp = self.get('/pywb/20140703030321{0}/http://example.com/?example=2', fmod)
         assert resp.status_int == 200
         assert resp.headers['Content-Location'].endswith('/pywb/20140603030341{0}/http://example.com?example=2'.format(fmod))
 
     def test_missing_revisit_other_capture(self, fmod):
         resp = self.get('/pywb/20140603030351{0}/http://example.com/?example=2', fmod)
         assert resp.status_int == 200
         assert resp.headers['Content-Location'].endswith('/pywb/20140603030341{0}/http://example.com?example=2'.format(fmod))
 
-    def test_not_existant_warc_no_other(self, fmod):
+    def test_not_existent_warc_no_other(self, fmod):
         resp = self.get('/pywb/20140703030321{0}/http://example.com/?example=3', fmod, status=503)
         assert resp.status_int == 503
 
     def test_missing_revisit_no_other(self, fmod):
         resp = self.get('/pywb/20140603030351{0}/http://example.com/?example=3', fmod, status=503)
         assert resp.status_int == 503
```

### Comparing `pywb-2.7.4/tests/test_live_rewriter.py` & `pywb-2.8.0/tests/test_live_rewriter.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,33 +87,36 @@
         #assert '"http://httpbin.org/anything/abc##xyz"' in resp.text
         assert resp.status_int == 200
 
     def test_live_head(self, fmod_sl):
         resp = self.head('/live/{0}httpbin.org/get?foo=bar', fmod_sl)
         assert resp.status_int == 200
 
-    @pytest.mark.skipif(sys.version_info < (3,0), reason='does not respond in 2.7')
-    def test_live_bad_content_length(self, fmod_sl):
-        resp = self.get('/live/{0}httpbin.org/response-headers?content-length=149,149', fmod_sl, status=200)
-        assert resp.headers['Content-Length'] == '149'
-
-        resp = self.get('/live/{0}httpbin.org/response-headers?Content-Length=xyz', fmod_sl, status=200)
-        assert resp.headers['Content-Length'] == '90'
-
-    @pytest.mark.skipif(sys.version_info < (3,0), reason='does not respond in 2.7')
-    def test_live_bad_content_length_with_range(self, fmod_sl):
-        resp = self.get('/live/{0}httpbin.org/response-headers?content-length=149,149', fmod_sl,
-                        headers={'Range': 'bytes=0-'}, status=206)
-        assert resp.headers['Content-Length'] == '149'
-        assert resp.headers['Content-Range'] == 'bytes 0-148/149'
-
-        resp = self.get('/live/{0}httpbin.org/response-headers?Content-Length=xyz', fmod_sl,
-                        headers={'Range': 'bytes=0-'}, status=206)
-        assert resp.headers['Content-Length'] == '90'
-        assert resp.headers['Content-Range'] == 'bytes 0-89/90'
+    # Following tests are temporarily commented out because latest version of PSF httpbin
+    # now returns 400 if content-length header isn't parsable as an int
+
+    # @pytest.mark.skipif(sys.version_info < (3,0), reason='does not respond in 2.7')
+    # def test_live_bad_content_length(self, fmod_sl):
+    #     resp = self.get('/live/{0}httpbin.org/response-headers?content-length=149,149', fmod_sl, status=200)
+    #     assert resp.headers['Content-Length'] == '149'
+
+    #     resp = self.get('/live/{0}httpbin.org/response-headers?Content-Length=xyz', fmod_sl, status=200)
+    #     assert resp.headers['Content-Length'] == '90'
+
+    # @pytest.mark.skipif(sys.version_info < (3,0), reason='does not respond in 2.7')
+    # def test_live_bad_content_length_with_range(self, fmod_sl):
+    #     resp = self.get('/live/{0}httpbin.org/response-headers?content-length=149,149', fmod_sl,
+    #                     headers={'Range': 'bytes=0-'}, status=206)
+    #     assert resp.headers['Content-Length'] == '149'
+    #     assert resp.headers['Content-Range'] == 'bytes 0-148/149'
+
+    #     resp = self.get('/live/{0}httpbin.org/response-headers?Content-Length=xyz', fmod_sl,
+    #                     headers={'Range': 'bytes=0-'}, status=206)
+    #     assert resp.headers['Content-Length'] == '90'
+    #     assert resp.headers['Content-Range'] == 'bytes 0-89/90'
 
     def test_custom_unicode_header(self, fmod_sl):
         value = u'⛄'
         value = value.encode('utf-8')
         if six.PY3:
             value = value.decode('latin-1')
 
@@ -165,16 +168,15 @@
         assert resp.status_int == 400
 
     def test_live_invalid_2(self, fmod_sl):
         resp = self.get('/live/{0}@#$@#$', fmod_sl, status=307)
         resp = resp.follow(status=400)
         assert resp.status_int == 400
 
-    #@pytest.mark.skipif(os.environ.get('CI') is not None, reason='Skip Test on CI')
-    @pytest.mark.skip("youtube-dl update needed")
+    @pytest.mark.skipif(os.environ.get('CI') is not None, reason='Skip Test on CI')
     def test_live_video_info(self):
         pytest.importorskip('youtube_dl')
         resp = self.testapp.get('/live/vi_/https://www.youtube.com/watch?v=DjFZyFWSt1M')
         assert resp.status_int == 200
         assert resp.content_type == 'application/vnd.youtube-dl_formats+json', resp.content_type
 
     def test_deflate(self, fmod_sl):
```

### Comparing `pywb-2.7.4/tests/test_locales.py` & `pywb-2.8.0/tests/test_locales.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests/test_memento.py` & `pywb-2.8.0/tests/test_memento.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests/test_prefer_header.py` & `pywb-2.8.0/tests/test_prefer_header.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests/test_prefixed_deploy.py` & `pywb-2.8.0/tests/test_prefixed_deploy.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests/test_proxy.py` & `pywb-2.8.0/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests/test_range.py` & `pywb-2.8.0/tests/test_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         resp = self.get('/pywb/20140127171250{0}/http://example.com/', fmod, headers=headers)
 
         assert resp.status_int == 206
         assert resp.headers['Accept-Ranges'] == 'bytes'
         assert resp.headers['Content-Range'] == 'bytes 0-200/1270', resp.headers['Content-Range']
         assert resp.content_length == 201, resp.content_length
 
-        assert self.recorder_skip == '1'
+        assert self.recorder_skip == None
 
         assert 'wombat.js' not in resp.text
 
     def test_replay_range_start_end_2(self, fmod):
         headers = [('Range', 'bytes=10-200')]
         resp = self.get('/pywb/20140127171250{0}/http://example.com/', fmod, headers=headers)
```

### Comparing `pywb-2.7.4/tests/test_record_dedup.py` & `pywb-2.8.0/tests/test_record_dedup.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests/test_record_replay.py` & `pywb-2.8.0/tests/test_record_replay.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests/test_redirect_classic.py` & `pywb-2.8.0/tests/test_redirect_classic.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests/test_redirect_revisits.py` & `pywb-2.8.0/tests/test_redirect_revisits.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests/test_redirects.py` & `pywb-2.8.0/tests/test_redirects.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests/test_root_coll.py` & `pywb-2.8.0/tests/test_root_coll.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests/test_socks.py` & `pywb-2.8.0/tests/test_socks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from .base_config_test import BaseConfigTest, fmod_sl
 
-import sys
 import os
 import pytest
 
 
 # ============================================================================
-@pytest.mark.skipif(sys.version_info >= (3, 10), reason="need to reexamine on py3.10")
 class TestSOCKSProxy(BaseConfigTest):
     @classmethod
     def setup_class(cls):
         pytest.importorskip('socks')
         os.environ['SOCKS_HOST'] = 'localhost'
         os.environ['SOCKS_PORT'] = '0'
```

### Comparing `pywb-2.7.4/tests/test_zipnum_auto_dir.py` & `pywb-2.8.0/tests/test_zipnum_auto_dir.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests_disabled/fixture.py` & `pywb-2.8.0/tests_disabled/fixture.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests_disabled/live.py` & `pywb-2.8.0/tests_disabled/live.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests_disabled/perms_fixture.py` & `pywb-2.8.0/tests_disabled/perms_fixture.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests_disabled/server_mock.py` & `pywb-2.8.0/tests_disabled/server_mock.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests_disabled/server_thread.py` & `pywb-2.8.0/tests_disabled/server_thread.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests_disabled/test_cdxserver.py` & `pywb-2.8.0/tests_disabled/test_cdxserver.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests_disabled/test_config_memento.yaml` & `pywb-2.8.0/tests_disabled/test_config_memento.yaml`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests_disabled/test_config_proxy_https_cookie.yaml` & `pywb-2.8.0/tests_disabled/test_config_proxy_https_cookie.yaml`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests_disabled/test_live_proxy.py` & `pywb-2.8.0/tests_disabled/test_live_proxy.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests_disabled/test_memento.py` & `pywb-2.8.0/tests_disabled/test_memento.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests_disabled/test_perms.py` & `pywb-2.8.0/tests_disabled/test_perms.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests_disabled/test_perms_app.py` & `pywb-2.8.0/tests_disabled/test_perms_app.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests_disabled/test_proxy_http_auth.py` & `pywb-2.8.0/tests_disabled/test_proxy_http_auth.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests_disabled/test_proxy_http_cookie.py` & `pywb-2.8.0/tests_disabled/test_proxy_http_cookie.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests_disabled/test_proxy_http_ip.py` & `pywb-2.8.0/tests_disabled/test_proxy_http_ip.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests_disabled/test_proxy_http_ip_redis.py` & `pywb-2.8.0/tests_disabled/test_proxy_http_ip_redis.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests_disabled/test_proxy_http_no_banner.py` & `pywb-2.8.0/tests_disabled/test_proxy_http_no_banner.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests_disabled/test_proxy_https_cookie.py` & `pywb-2.8.0/tests_disabled/test_proxy_https_cookie.py`

 * *Files identical despite different names*

### Comparing `pywb-2.7.4/tests_disabled/test_rewrite_content.py` & `pywb-2.8.0/tests_disabled/test_rewrite_content.py`

 * *Files identical despite different names*
