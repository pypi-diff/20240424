# Comparing `tmp/clastic-23.1.0.tar.gz` & `tmp/clastic-24.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/clastic-23.1.0.tar", last modified: Mon Dec 18 01:06:15 2023, max compression
+gzip compressed data, was "clastic-24.0.0.tar", last modified: Wed Apr 24 04:50:58 2024, max compression
```

## Comparing `clastic-23.1.0.tar` & `clastic-24.0.0.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxr-x   0 mahmoud   (1000) mahmoud   (1000)        0 2023-12-18 01:06:15.000000 clastic-23.1.0/
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1502 2023-02-17 08:21:28.000000 clastic-23.1.0/LICENSE
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      148 2023-02-17 08:21:28.000000 clastic-23.1.0/MANIFEST.in
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1275 2023-12-18 01:06:15.000000 clastic-23.1.0/PKG-INFO
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)    31177 2023-02-17 08:21:28.000000 clastic-23.1.0/README.rst
-drwxrwxr-x   0 mahmoud   (1000) mahmoud   (1000)        0 2023-12-18 01:06:15.000000 clastic-23.1.0/clastic/
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1185 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/__init__.py
-drwxrwxr-x   0 mahmoud   (1000) mahmoud   (1000)        0 2023-12-18 01:06:15.000000 clastic-23.1.0/clastic/_clastic_assets/
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1292 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/_clastic_assets/common.css
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)    93064 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/_clastic_assets/jquery-1.10.1.min.js
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     7346 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/_clastic_assets/normalize.css
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)    15261 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/_contextual_errors.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      116 2023-12-18 00:47:29.000000 clastic-23.1.0/clastic/_version.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)    27636 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/_werkzeug_serving.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)    21394 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/application.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     2405 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/cline.py
-drwxrwxr-x   0 mahmoud   (1000) mahmoud   (1000)        0 2023-12-18 01:06:15.000000 clastic-23.1.0/clastic/contrib/
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)        0 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/contrib/__init__.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     5250 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/contrib/obj_browser.py
-drwxrwxr-x   0 mahmoud   (1000) mahmoud   (1000)        0 2023-12-18 01:06:15.000000 clastic-23.1.0/clastic/contrib/webtop/
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)        0 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/contrib/webtop/__init__.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      694 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/contrib/webtop/top.html
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     2937 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/contrib/webtop/top.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      778 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/decorators.py
-drwxrwxr-x   0 mahmoud   (1000) mahmoud   (1000)        0 2023-12-18 01:06:15.000000 clastic-23.1.0/clastic/docs/
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     9781 2023-10-17 16:32:29.000000 clastic-23.1.0/clastic/docs/routing.md
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)    26472 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/errors.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     6369 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/flaw.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)    16272 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/meta.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      903 2023-10-17 16:32:29.000000 clastic-23.1.0/clastic/meta_base.html
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     3557 2023-10-17 16:32:29.000000 clastic-23.1.0/clastic/meta_env_section.html
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      505 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/meta_host_section.html
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      742 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/meta_main_base.html
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      393 2023-10-17 16:32:29.000000 clastic-23.1.0/clastic/meta_mw_section.html
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      501 2023-10-17 16:32:29.000000 clastic-23.1.0/clastic/meta_proc_section.html
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1221 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/meta_pyvm_section.html
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      191 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/meta_resource_section.html
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      958 2023-10-17 16:32:29.000000 clastic-23.1.0/clastic/meta_route_section.html
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1253 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/meta_rusage_section.html
-drwxrwxr-x   0 mahmoud   (1000) mahmoud   (1000)        0 2023-12-18 01:06:15.000000 clastic-23.1.0/clastic/middleware/
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      460 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/middleware/__init__.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1258 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/middleware/client_cache.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1223 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/middleware/compress.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     3278 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/middleware/context.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     4665 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/middleware/cookie.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     7424 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/middleware/core.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1347 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/middleware/form.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1702 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/middleware/profile.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     5835 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/middleware/stats.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1630 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/middleware/url.py
-drwxrwxr-x   0 mahmoud   (1000) mahmoud   (1000)        0 2023-12-18 01:06:15.000000 clastic-23.1.0/clastic/render/
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      483 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/render/__init__.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     2077 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/render/ashes_templates.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     2085 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/render/chameleon_templates.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1784 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/render/mako_templates.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     6224 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/render/simple.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     4806 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/render/tabular.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)    25392 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/route.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     6676 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/server.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     5810 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/sinter.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     6285 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/static.py
-drwxrwxr-x   0 mahmoud   (1000) mahmoud   (1000)        0 2023-12-18 01:06:15.000000 clastic-23.1.0/clastic/tests/
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)        0 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/tests/__init__.py
-drwxrwxr-x   0 mahmoud   (1000) mahmoud   (1000)        0 2023-12-18 01:06:15.000000 clastic-23.1.0/clastic/tests/_ashes_tmpls/
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      251 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/tests/_ashes_tmpls/basic_template.html
-drwxrwxr-x   0 mahmoud   (1000) mahmoud   (1000)        0 2023-12-18 01:06:15.000000 clastic-23.1.0/clastic/tests/_chameleon_tmpls/
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      331 2023-12-17 21:13:46.000000 clastic-23.1.0/clastic/tests/_chameleon_tmpls/basic_template.pt
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)       59 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/tests/_chameleon_tmpls/broken_template_1.pt
-drwxrwxr-x   0 mahmoud   (1000) mahmoud   (1000)        0 2023-12-18 01:06:15.000000 clastic-23.1.0/clastic/tests/_mako_tmpls/
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      356 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/tests/_mako_tmpls/basic_template.html
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      102 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/tests/_mako_tmpls/broken_template_1.html
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     2146 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/tests/common.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     2754 2023-10-17 16:32:28.000000 clastic-23.1.0/clastic/tests/test_arg_resolve.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     2323 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/tests/test_ashes_render.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     3420 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/tests/test_basic.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     2060 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/tests/test_chameleon_render.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      329 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/tests/test_cline.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     3483 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/tests/test_context_proc.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1513 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/tests/test_cookie.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1499 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/tests/test_decorators.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     2294 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/tests/test_errors.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      416 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/tests/test_flaw.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1750 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/tests/test_http_routing.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     2008 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/tests/test_mako_render.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     3061 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/tests/test_meta.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     6338 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/tests/test_middleware.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      548 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/tests/test_obj_browser.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     4901 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/tests/test_render.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     2935 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/tests/test_render_error.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     6011 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/tests/test_routing.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      709 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/tests/test_serve.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1757 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/tests/test_static.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      841 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/tests/test_stats_mw.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      244 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/tests/test_webtop.py
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1357 2023-12-18 00:29:52.000000 clastic-23.1.0/clastic/utils.py
-drwxrwxr-x   0 mahmoud   (1000) mahmoud   (1000)        0 2023-12-18 01:06:15.000000 clastic-23.1.0/clastic.egg-info/
--rw-r--r--   0 mahmoud   (1000) mahmoud   (1000)     1275 2023-12-18 01:06:15.000000 clastic-23.1.0/clastic.egg-info/PKG-INFO
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     2594 2023-12-18 01:06:15.000000 clastic-23.1.0/clastic.egg-info/SOURCES.txt
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)        1 2023-12-18 01:06:15.000000 clastic-23.1.0/clastic.egg-info/dependency_links.txt
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)        1 2023-04-21 00:32:16.000000 clastic-23.1.0/clastic.egg-info/not-zip-safe
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)       83 2023-12-18 01:06:15.000000 clastic-23.1.0/clastic.egg-info/requires.txt
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)        8 2023-12-18 01:06:15.000000 clastic-23.1.0/clastic.egg-info/top_level.txt
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)       61 2023-12-18 01:06:15.000000 clastic-23.1.0/setup.cfg
--rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     2975 2023-12-18 00:44:21.000000 clastic-23.1.0/setup.py
+drwxrwxr-x   0 mahmoud   (1000) mahmoud   (1000)        0 2024-04-24 04:50:58.864790 clastic-24.0.0/
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1502 2023-02-17 08:21:28.000000 clastic-24.0.0/LICENSE
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      148 2023-02-17 08:21:28.000000 clastic-24.0.0/MANIFEST.in
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1275 2024-04-24 04:50:58.864790 clastic-24.0.0/PKG-INFO
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)    31174 2023-12-18 17:57:08.000000 clastic-24.0.0/README.rst
+drwxrwxr-x   0 mahmoud   (1000) mahmoud   (1000)        0 2024-04-24 04:50:58.860790 clastic-24.0.0/clastic/
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1185 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/__init__.py
+drwxrwxr-x   0 mahmoud   (1000) mahmoud   (1000)        0 2024-04-24 04:50:58.860790 clastic-24.0.0/clastic/_clastic_assets/
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1292 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/_clastic_assets/common.css
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)    93064 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/_clastic_assets/jquery-1.10.1.min.js
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     7346 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/_clastic_assets/normalize.css
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)    15261 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/_contextual_errors.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      116 2024-04-24 04:50:30.000000 clastic-24.0.0/clastic/_version.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)    27636 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/_werkzeug_serving.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)    21394 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/application.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     2405 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/cline.py
+drwxrwxr-x   0 mahmoud   (1000) mahmoud   (1000)        0 2024-04-24 04:50:58.860790 clastic-24.0.0/clastic/contrib/
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)        0 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/contrib/__init__.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     5250 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/contrib/obj_browser.py
+drwxrwxr-x   0 mahmoud   (1000) mahmoud   (1000)        0 2024-04-24 04:50:58.860790 clastic-24.0.0/clastic/contrib/webtop/
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)        0 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/contrib/webtop/__init__.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      694 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/contrib/webtop/top.html
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     2937 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/contrib/webtop/top.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      778 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/decorators.py
+drwxrwxr-x   0 mahmoud   (1000) mahmoud   (1000)        0 2024-04-24 04:50:58.860790 clastic-24.0.0/clastic/docs/
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     9781 2023-10-17 16:32:29.000000 clastic-24.0.0/clastic/docs/routing.md
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)    26472 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/errors.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     6369 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/flaw.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)    16367 2024-04-24 04:45:29.000000 clastic-24.0.0/clastic/meta.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      903 2023-10-17 16:32:29.000000 clastic-24.0.0/clastic/meta_base.html
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     3557 2023-10-17 16:32:29.000000 clastic-24.0.0/clastic/meta_env_section.html
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      505 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/meta_host_section.html
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      742 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/meta_main_base.html
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      393 2023-10-17 16:32:29.000000 clastic-24.0.0/clastic/meta_mw_section.html
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      501 2023-10-17 16:32:29.000000 clastic-24.0.0/clastic/meta_proc_section.html
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1221 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/meta_pyvm_section.html
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      191 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/meta_resource_section.html
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      958 2023-10-17 16:32:29.000000 clastic-24.0.0/clastic/meta_route_section.html
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1253 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/meta_rusage_section.html
+drwxrwxr-x   0 mahmoud   (1000) mahmoud   (1000)        0 2024-04-24 04:50:58.860790 clastic-24.0.0/clastic/middleware/
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      460 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/middleware/__init__.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1258 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/middleware/client_cache.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1223 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/middleware/compress.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     3278 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/middleware/context.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     4665 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/middleware/cookie.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     7424 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/middleware/core.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1347 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/middleware/form.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1702 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/middleware/profile.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     5835 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/middleware/stats.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1630 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/middleware/url.py
+drwxrwxr-x   0 mahmoud   (1000) mahmoud   (1000)        0 2024-04-24 04:50:58.864790 clastic-24.0.0/clastic/render/
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      483 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/render/__init__.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     2077 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/render/ashes_templates.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     2085 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/render/chameleon_templates.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1784 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/render/mako_templates.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     6224 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/render/simple.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     4806 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/render/tabular.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)    25392 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/route.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     6676 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/server.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     5810 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/sinter.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     6285 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/static.py
+drwxrwxr-x   0 mahmoud   (1000) mahmoud   (1000)        0 2024-04-24 04:50:58.864790 clastic-24.0.0/clastic/tests/
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)        0 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/tests/__init__.py
+drwxrwxr-x   0 mahmoud   (1000) mahmoud   (1000)        0 2024-04-24 04:50:58.864790 clastic-24.0.0/clastic/tests/_ashes_tmpls/
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      251 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/tests/_ashes_tmpls/basic_template.html
+drwxrwxr-x   0 mahmoud   (1000) mahmoud   (1000)        0 2024-04-24 04:50:58.864790 clastic-24.0.0/clastic/tests/_chameleon_tmpls/
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      331 2023-12-17 21:13:46.000000 clastic-24.0.0/clastic/tests/_chameleon_tmpls/basic_template.pt
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)       59 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/tests/_chameleon_tmpls/broken_template_1.pt
+drwxrwxr-x   0 mahmoud   (1000) mahmoud   (1000)        0 2024-04-24 04:50:58.864790 clastic-24.0.0/clastic/tests/_mako_tmpls/
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      356 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/tests/_mako_tmpls/basic_template.html
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      102 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/tests/_mako_tmpls/broken_template_1.html
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     2146 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/tests/common.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     2754 2023-10-17 16:32:28.000000 clastic-24.0.0/clastic/tests/test_arg_resolve.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     2323 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/tests/test_ashes_render.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     3420 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/tests/test_basic.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     2082 2024-04-24 02:04:01.000000 clastic-24.0.0/clastic/tests/test_chameleon_render.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      329 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/tests/test_cline.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     3483 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/tests/test_context_proc.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1513 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/tests/test_cookie.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1499 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/tests/test_decorators.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     2294 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/tests/test_errors.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      416 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/tests/test_flaw.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1750 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/tests/test_http_routing.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     2008 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/tests/test_mako_render.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     3252 2024-04-24 04:39:19.000000 clastic-24.0.0/clastic/tests/test_meta.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     6338 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/tests/test_middleware.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      548 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/tests/test_obj_browser.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     4901 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/tests/test_render.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     2935 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/tests/test_render_error.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     6011 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/tests/test_routing.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      709 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/tests/test_serve.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1757 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/tests/test_static.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      841 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/tests/test_stats_mw.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)      244 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/tests/test_webtop.py
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     1357 2023-12-18 00:29:52.000000 clastic-24.0.0/clastic/utils.py
+drwxrwxr-x   0 mahmoud   (1000) mahmoud   (1000)        0 2024-04-24 04:50:58.860790 clastic-24.0.0/clastic.egg-info/
+-rw-r--r--   0 mahmoud   (1000) mahmoud   (1000)     1275 2024-04-24 04:50:58.000000 clastic-24.0.0/clastic.egg-info/PKG-INFO
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     2594 2024-04-24 04:50:58.000000 clastic-24.0.0/clastic.egg-info/SOURCES.txt
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)        1 2024-04-24 04:50:58.000000 clastic-24.0.0/clastic.egg-info/dependency_links.txt
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)        1 2023-04-21 00:32:16.000000 clastic-24.0.0/clastic.egg-info/not-zip-safe
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)       83 2024-04-24 04:50:58.000000 clastic-24.0.0/clastic.egg-info/requires.txt
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)        8 2024-04-24 04:50:58.000000 clastic-24.0.0/clastic.egg-info/top_level.txt
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)       61 2024-04-24 04:50:58.864790 clastic-24.0.0/setup.cfg
+-rw-rw-r--   0 mahmoud   (1000) mahmoud   (1000)     2975 2024-04-24 02:04:01.000000 clastic-24.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `clastic-23.1.0/LICENSE` & `clastic-24.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/PKG-INFO` & `clastic-24.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: clastic
-Version: 23.1.0
+Version: 24.0.0
 Summary: A functional Python web framework that streamlines explicit development practices while eliminating global state.
 Home-page: https://github.com/mahmoud/clastic
 Author: Mahmoud Hashemi
 Author-email: mahmoud@hatnote.com
 License: BSD
 Description: Clastic is a functional Python web framework that streamlines
         explicit development practices while eliminating global state.
```

### Comparing `clastic-23.1.0/README.rst` & `clastic-24.0.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
    <a href="https://pypi.org/project/clastic/"><img src="https://img.shields.io/pypi/v/clastic.svg"></a>
    <a href="https://calver.org/"><img src="https://img.shields.io/badge/calver-YY.MINOR.MICRO-22bfda.svg"></a>
 
 A functional Python web framework that streamlines explicit
 development practices while eliminating global state.
 
-Clastic is pure-Python, tested on Python 2.7-3.7, and
+Clastic is pure-Python, tested on Python 3.7+, and
 `documented <https://python-clastic.readthedocs.io/>`_,
 with `tutorials <https://python-clastic.readthedocs.io/en/latest/tutorial.html>`_.
 
 .. contents::
    :depth: 2
    :backlinks: top
    :local:
```

### Comparing `clastic-23.1.0/clastic/__init__.py` & `clastic-24.0.0/clastic/__init__.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/_clastic_assets/common.css` & `clastic-24.0.0/clastic/_clastic_assets/common.css`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/_clastic_assets/jquery-1.10.1.min.js` & `clastic-24.0.0/clastic/_clastic_assets/jquery-1.10.1.min.js`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/_clastic_assets/normalize.css` & `clastic-24.0.0/clastic/_clastic_assets/normalize.css`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/_contextual_errors.py` & `clastic-24.0.0/clastic/_contextual_errors.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/_werkzeug_serving.py` & `clastic-24.0.0/clastic/_werkzeug_serving.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/application.py` & `clastic-24.0.0/clastic/application.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/cline.py` & `clastic-24.0.0/clastic/cline.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/contrib/obj_browser.py` & `clastic-24.0.0/clastic/contrib/obj_browser.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/contrib/webtop/top.html` & `clastic-24.0.0/clastic/contrib/webtop/top.html`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/contrib/webtop/top.py` & `clastic-24.0.0/clastic/contrib/webtop/top.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/decorators.py` & `clastic-24.0.0/clastic/decorators.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/docs/routing.md` & `clastic-24.0.0/clastic/docs/routing.md`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/errors.py` & `clastic-24.0.0/clastic/errors.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/flaw.py` & `clastic-24.0.0/clastic/flaw.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/meta.py` & `clastic-24.0.0/clastic/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,28 +91,28 @@
 
 
 def get_proc_info():
     ret = {}
     ret['pid'] = os.getpid()
     _user_t, _sys_t = os.times()[:2]
     ret['cpu_times'] = {'user_time': _user_t, 'sys_time': _sys_t}
-    ret['cwd'] = os.getcwdu()
+    ret['cwd'] = os.getcwd()
     ret['umask'] = os.umask(os.umask(2))  # have to set to get
     ret['umask_str'] = '{0:03o}'.format(ret['umask'])
 
     ret['owner'] = glom(globals(), Coalesce(T['getpass'].getuser(),
                                             T['os'].getuid()),
                         skip_exc=Exception)
 
     # use 0 to get current niceness, seems to return process group's nice level
     unix_only_vals = glom(os, {'ppid': T.getppid(),
                                'pgid': T.getpgrp(),
                                'niceness': T.nice(0)},
                           skip_exc=AttributeError)
-    ret.update(unix_only_vals)
+    ret.update(unix_only_vals or {})
 
     ret['rusage'] = get_rusage_dict()
     ret['rlimit'] = get_rlimit_dict()
     return ret
 
 
 # TODO: byte order, path, prefix
@@ -195,16 +195,19 @@
     ret['have_readline'] = HAVE_READLINE
 
     ret['active_thread_count'] = glom(sys, (T._current_frames(), len), skip_exc=Exception)
     ret['recursion_limit'] = sys.getrecursionlimit()
 
     ret['gc'] = glom(None, Call(get_gc_info), skip_exc=Exception)  # effectively try/except:pass
 
-    get_interval = getattr(sys, 'getswitchinterval', sys.getcheckinterval)
-    ret['check_interval'] = get_interval()
+    get_interval = getattr(sys, 'getswitchinterval', getattr(sys, 'getcheckinterval', None))
+    if get_interval:
+        ret['check_interval'] = get_interval()
+    else:
+        ret['check_interval'] = None
     return ret
 
 
 def get_gc_info():
     import gc
     ret = {}
     ret['is_enabled'] = gc.isenabled()
```

### Comparing `clastic-23.1.0/clastic/meta_base.html` & `clastic-24.0.0/clastic/meta_base.html`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/meta_env_section.html` & `clastic-24.0.0/clastic/meta_env_section.html`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/meta_main_base.html` & `clastic-24.0.0/clastic/meta_main_base.html`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/meta_pyvm_section.html` & `clastic-24.0.0/clastic/meta_pyvm_section.html`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/meta_route_section.html` & `clastic-24.0.0/clastic/meta_route_section.html`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/meta_rusage_section.html` & `clastic-24.0.0/clastic/meta_rusage_section.html`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/middleware/client_cache.py` & `clastic-24.0.0/clastic/middleware/client_cache.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/middleware/compress.py` & `clastic-24.0.0/clastic/middleware/compress.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/middleware/context.py` & `clastic-24.0.0/clastic/middleware/context.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/middleware/cookie.py` & `clastic-24.0.0/clastic/middleware/cookie.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/middleware/core.py` & `clastic-24.0.0/clastic/middleware/core.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/middleware/form.py` & `clastic-24.0.0/clastic/middleware/form.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/middleware/profile.py` & `clastic-24.0.0/clastic/middleware/profile.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/middleware/stats.py` & `clastic-24.0.0/clastic/middleware/stats.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/middleware/url.py` & `clastic-24.0.0/clastic/middleware/url.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/render/ashes_templates.py` & `clastic-24.0.0/clastic/render/ashes_templates.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/render/chameleon_templates.py` & `clastic-24.0.0/clastic/render/chameleon_templates.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/render/mako_templates.py` & `clastic-24.0.0/clastic/render/mako_templates.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/render/simple.py` & `clastic-24.0.0/clastic/render/simple.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/render/tabular.py` & `clastic-24.0.0/clastic/render/tabular.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/route.py` & `clastic-24.0.0/clastic/route.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/server.py` & `clastic-24.0.0/clastic/server.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/sinter.py` & `clastic-24.0.0/clastic/sinter.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/static.py` & `clastic-24.0.0/clastic/static.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/tests/common.py` & `clastic-24.0.0/clastic/tests/common.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/tests/test_arg_resolve.py` & `clastic-24.0.0/clastic/tests/test_arg_resolve.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/tests/test_ashes_render.py` & `clastic-24.0.0/clastic/tests/test_ashes_render.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/tests/test_basic.py` & `clastic-24.0.0/clastic/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/tests/test_chameleon_render.py` & `clastic-24.0.0/clastic/tests/test_chameleon_render.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,12 +54,12 @@
     tmpl = 'basic_template.pt'
     app = Application([('/', hello_world_ctx, tmpl),
                        ('/json/', hello_world_ctx, render_basic)],
                       render_factory=chameleon_render)
 
     c = app.get_local_client()
     resp = c.get('/')
-    assert resp.status_code == 200
+    assert resp.status_code == 200, resp.data
     assert b'clasty' in resp.data
 
     resp = c.get('/json/')
-    assert resp.status_code == 200
+    assert resp.status_code == 200, resp.data
```

### Comparing `clastic-23.1.0/clastic/tests/test_context_proc.py` & `clastic-24.0.0/clastic/tests/test_context_proc.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/tests/test_cookie.py` & `clastic-24.0.0/clastic/tests/test_cookie.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/tests/test_decorators.py` & `clastic-24.0.0/clastic/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/tests/test_errors.py` & `clastic-24.0.0/clastic/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/tests/test_http_routing.py` & `clastic-24.0.0/clastic/tests/test_http_routing.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/tests/test_mako_render.py` & `clastic-24.0.0/clastic/tests/test_mako_render.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/tests/test_meta.py` & `clastic-24.0.0/clastic/tests/test_meta.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,26 +55,29 @@
     cl = app.get_local_client()
     assert cl.get('/meta/').status_code == 200
     if IS_PYPY:
         return
 
     resp = cl.get('/meta/json/')
     assert resp.status_code == 200
+    resp_data = json.loads(resp.data)
 
-    endpoints = [r['endpoint'] for r in json.loads(resp.data)['app']['routes']]
+    endpoints = [r['endpoint'] for r in resp_data['app']['routes']]
     assert endpoints == [{'module_name': 'clastic.tests.test_meta', 'name': 'func_ep'},
                          {'module_name': 'clastic.tests.test_meta.CallableObj', 'name': 'ep_method'},
                          {'module_name': 'clastic.tests.test_meta', 'name': 'CallableObj'},
                          {'module_name': 'clastic.static.StaticFileRoute', 'name': 'get_file_response'},
                          {'module_name': 'clastic.meta.MetaApplication', 'name': 'get_main'},
                          {'module_name': 'clastic.static.StaticApplication',
                           'name': 'get_file_response'},
                          {'module_name': 'clastic.meta.MetaApplication', 'name': 'get_main'},
                          {'module_name': 'builtins', 'name': 'sum'}]
-
+    
+    for peripheral, info in resp_data.items():
+        assert 'exc_content' not in info, f'failed meta context for domain "{peripheral}": {info["exc_content"]}'
 
 def test_resource_redaction():
     app = Application(routes=[('/meta', MetaApplication())],
                       resources={'a_secret': 'vsecret', 'ok': 'bokay'})
 
     cl = app.get_local_client()
     resp = cl.get('/meta/')
```

### Comparing `clastic-23.1.0/clastic/tests/test_middleware.py` & `clastic-24.0.0/clastic/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/tests/test_obj_browser.py` & `clastic-24.0.0/clastic/tests/test_obj_browser.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/tests/test_render.py` & `clastic-24.0.0/clastic/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/tests/test_render_error.py` & `clastic-24.0.0/clastic/tests/test_render_error.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/tests/test_routing.py` & `clastic-24.0.0/clastic/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/tests/test_serve.py` & `clastic-24.0.0/clastic/tests/test_serve.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/tests/test_static.py` & `clastic-24.0.0/clastic/tests/test_static.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/tests/test_stats_mw.py` & `clastic-24.0.0/clastic/tests/test_stats_mw.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic/utils.py` & `clastic-24.0.0/clastic/utils.py`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/clastic.egg-info/PKG-INFO` & `clastic-24.0.0/clastic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: clastic
-Version: 23.1.0
+Version: 24.0.0
 Summary: A functional Python web framework that streamlines explicit development practices while eliminating global state.
 Home-page: https://github.com/mahmoud/clastic
 Author: Mahmoud Hashemi
 Author-email: mahmoud@hatnote.com
 License: BSD
 Description: Clastic is a functional Python web framework that streamlines
         explicit development practices while eliminating global state.
```

### Comparing `clastic-23.1.0/clastic.egg-info/SOURCES.txt` & `clastic-24.0.0/clastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clastic-23.1.0/setup.py` & `clastic-24.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
           'attrs',
           'boltons>=20.0.0', 
           'glom', 
           'secure-cookie==0.1.0,<=0.2.0'],
       license=__license__,
       platforms='any',
       tests_require=[
-          'chameleon==3.9.1',
+          'chameleon>=4.4.1',
           'Mako', 
           'pytest', 
           'psutil'],
       classifiers=[
           'Intended Audience :: Developers',
           'Development Status :: 5 - Production/Stable',
           'Topic :: Internet :: WWW/HTTP :: HTTP Servers',
```

