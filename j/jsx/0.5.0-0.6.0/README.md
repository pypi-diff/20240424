# Comparing `tmp/jsx-0.5.0.tar.gz` & `tmp/jsx-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsx-0.5.0.tar", last modified: Sun Mar 10 16:20:43 2024, max compression
+gzip compressed data, was "jsx-0.6.0.tar", last modified: Tue Apr 23 23:01:21 2024, max compression
```

## Comparing `jsx-0.5.0.tar` & `jsx-0.6.0.tar`

### file list

```diff
@@ -1,112 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 16:20:43.644219 jsx-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-10 16:20:38.000000 jsx-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-03-10 16:20:43.644219 jsx-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-03-10 16:20:38.000000 jsx-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-10 16:20:38.000000 jsx-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-10 16:20:43.644219 jsx-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 16:20:43.624220 jsx-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 16:20:43.628219 jsx-0.5.0/src/jsx/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 16:20:43.628219 jsx-0.5.0/src/jsx/components/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/components/component.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 16:20:43.640219 jsx-0.5.0/src/jsx/html/
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/_auto_html.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/a.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/abbr.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/address.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/area.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/article.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/aside.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/b.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/base.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/blockquote.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/body.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/br.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/button.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/cite.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/code.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/col.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/div.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/element.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/em.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/embed.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/footer.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/form.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/fragment.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/h1.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/h2.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/h3.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/h4.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/h5.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/h6.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/head.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/header.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/hr.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/html.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/i.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/img.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/input.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/label.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/li.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/link.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/main.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/nav.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/ol.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/option.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/p.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/param.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/pre.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/script.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/section.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/select.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/small.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/source.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/span.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/strong.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/sub.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/sup.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/table.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/tbody.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/td.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/textarea.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/th.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/thead.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/time.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/title.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/tr.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/track.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/u.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/ul.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/html/wbr.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 16:20:43.640219 jsx-0.5.0/src/jsx/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/middlewares/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5924 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/middlewares/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/middlewares/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 16:20:43.644219 jsx-0.5.0/src/jsx/server/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/server/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/server/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/server/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/server/ws_router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 16:20:43.644219 jsx-0.5.0/src/jsx/styling/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/styling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/styling/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/styling/style.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-10 16:20:38.000000 jsx-0.5.0/src/jsx/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 16:20:43.644219 jsx-0.5.0/src/jsx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-03-10 16:20:43.000000 jsx-0.5.0/src/jsx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-03-10 16:20:43.000000 jsx-0.5.0/src/jsx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-10 16:20:43.000000 jsx-0.5.0/src/jsx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-10 16:20:43.000000 jsx-0.5.0/src/jsx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 16:20:43.644219 jsx-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-10 16:20:38.000000 jsx-0.5.0/tests/test_asgi_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-10 16:20:38.000000 jsx-0.5.0/tests/test_nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-03-10 16:20:38.000000 jsx-0.5.0/tests/test_rendering.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-10 16:20:38.000000 jsx-0.5.0/tests/test_wsgi_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:01:21.325303 jsx-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-23 23:01:16.000000 jsx-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-23 23:01:21.325303 jsx-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-23 23:01:16.000000 jsx-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:01:21.325303 jsx-0.6.0/jsx/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-23 23:01:16.000000 jsx-0.6.0/jsx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-23 23:01:16.000000 jsx-0.6.0/jsx/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-23 23:01:16.000000 jsx-0.6.0/jsx/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-23 23:01:16.000000 jsx-0.6.0/jsx/internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-23 23:01:16.000000 jsx-0.6.0/jsx/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:01:21.325303 jsx-0.6.0/jsx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-23 23:01:21.000000 jsx-0.6.0/jsx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-23 23:01:21.000000 jsx-0.6.0/jsx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 23:01:21.000000 jsx-0.6.0/jsx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-23 23:01:21.000000 jsx-0.6.0/jsx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-23 23:01:21.000000 jsx-0.6.0/jsx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-23 23:01:16.000000 jsx-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-23 23:01:16.000000 jsx-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 23:01:21.325303 jsx-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:01:21.325303 jsx-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-23 23:01:16.000000 jsx-0.6.0/tests/test_asgi_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-23 23:01:16.000000 jsx-0.6.0/tests/test_nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-04-23 23:01:16.000000 jsx-0.6.0/tests/test_rendering.py
```

### Comparing `jsx-0.5.0/LICENSE` & `jsx-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsx-0.5.0/PKG-INFO` & `jsx-0.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 Metadata-Version: 2.1
 Name: jsx
-Version: 0.5.0
+Version: 0.6.0
 Summary: A Python package for creating and manipulating HTML components. It is working similar to React.js, but in Python
 Author-email: Xpo Development <dev@xpo.dev>
 Project-URL: Homepage, https://github.com/xpodev/jsx
 Project-URL: Issues, https://github.com/xpodev/jsx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-socketio==5.11.1
+Requires-Dist: cssutils==2.9.0
 
 # Python JSX
 
-[![PyPI version](https://badge.fury.io/py/jsx.svg?)](https://pypi.org/project/jsx)
+[![PyPI version](https://badge.fury.io/py/jsx.svg)](https://pypi.org/project/jsx)
 
-![build](https://github.com/xpodev/pyrl/actions/workflows/python-publish.yml/badge.svg)
 ![test](https://github.com/xpodev/pyrl/actions/workflows/python-test.yml/badge.svg)
 
 JSX is a Python package for creating and manipulating HTML components. It is working similar to React.js, but in Python.
 
+## Installation
+```sh
+pip install jsx
+```
 
 ## Usage
 
 ```python
 from jsx import Div, H1, P, Component, Style
 
 class MyComponent(Component):
@@ -52,15 +57,15 @@
 def hello_world():
   return render(MyComponent())
 ```
 
 ### Server actions
 It's possible to pass a python function as component props.
 
-The current version works with `ASGIApp` and `WSGIApp`.
+The current version works with `ASGIApp`.
 ```python
 class Person(Component):
   def __init__(self, name: str, age: float):
     self.age = age
     self.name = name
 
   def render(self):
@@ -77,18 +82,18 @@
       Button(
         "Submit Age",
         type="submit"
       ),
       on_submit=self.save_age
     )
 
-  def set_age(self, event_data: JSXChangeEvent):
+  def set_age(self, event_data: ChangeEvent):
     self.age = event_data.value
 
-  def save_age(self, event_data: JSXSubmitEvent):
+  def save_age(self, event_data: SubmitEvent):
     user = get_user()
     user.age = self.age
     save(user)
 ```
 To call a function on the server include this script in your file
 ```html
 <script src="/socket.io/static/main.js"></script>
```

### Comparing `jsx-0.5.0/README.md` & `jsx-0.6.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # Python JSX
 
-[![PyPI version](https://badge.fury.io/py/jsx.svg?)](https://pypi.org/project/jsx)
+[![PyPI version](https://badge.fury.io/py/jsx.svg)](https://pypi.org/project/jsx)
 
-![build](https://github.com/xpodev/pyrl/actions/workflows/python-publish.yml/badge.svg)
 ![test](https://github.com/xpodev/pyrl/actions/workflows/python-test.yml/badge.svg)
 
 JSX is a Python package for creating and manipulating HTML components. It is working similar to React.js, but in Python.
 
+## Installation
+```sh
+pip install jsx
+```
 
 ## Usage
 
 ```python
 from jsx import Div, H1, P, Component, Style
 
 class MyComponent(Component):
@@ -38,15 +41,15 @@
 def hello_world():
   return render(MyComponent())
 ```
 
 ### Server actions
 It's possible to pass a python function as component props.
 
-The current version works with `ASGIApp` and `WSGIApp`.
+The current version works with `ASGIApp`.
 ```python
 class Person(Component):
   def __init__(self, name: str, age: float):
     self.age = age
     self.name = name
 
   def render(self):
@@ -63,18 +66,18 @@
       Button(
         "Submit Age",
         type="submit"
       ),
       on_submit=self.save_age
     )
 
-  def set_age(self, event_data: JSXChangeEvent):
+  def set_age(self, event_data: ChangeEvent):
     self.age = event_data.value
 
-  def save_age(self, event_data: JSXSubmitEvent):
+  def save_age(self, event_data: SubmitEvent):
     user = get_user()
     user.age = self.age
     save(user)
 ```
 To call a function on the server include this script in your file
 ```html
 <script src="/socket.io/static/main.js"></script>
@@ -97,8 +100,8 @@
 Actions use [socket.io](https://socket.io) to communicate between server and client.
 
 ## TODO
 - [ ] Add detailed documentation
 - [ ] Add more tests
 - [ ] Add support for http actions
 ## Contributing
-Feel free to open an issue or a pull request.
+Feel free to open an issue or a pull request.
```

### Comparing `jsx-0.5.0/pyproject.toml` & `jsx-0.6.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 [project]
 name = "jsx"
-version = "0.5.0"
+version = "0.6.0"
 authors = [
   { name="Xpo Development", email="dev@xpo.dev" },
 ]
 description = "A Python package for creating and manipulating HTML components. It is working similar to React.js, but in Python"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dynamic = ["dependencies"]
 
 [project.urls]
 Homepage = "https://github.com/xpodev/jsx"
-Issues = "https://github.com/xpodev/jsx/issues"
+Issues = "https://github.com/xpodev/jsx/issues"
+
+[tool.setuptools]
+packages = ["jsx"]
+
+[tool.setuptools.dynamic]
+dependencies = {file = ["requirements.txt"]}
```

### Comparing `jsx-0.5.0/src/jsx/html/element.py` & `jsx-0.6.0/jsx/element.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,55 @@
-from typing import TYPE_CHECKING
-from abc import abstractproperty
+from typing import TYPE_CHECKING, Iterable, TypeVar, Generic, Unpack
+from abc import abstractmethod
 
-from ..server.database import DB
+from .types import Primitive, Renderable
+
+from .server.database import DB
 
 if TYPE_CHECKING:
     from jsx.types import ChildrenType
 
 
-def class_name_mapper(class_name):
-    return {
-        "class": " ".join(
-            class_name.split() if isinstance(class_name, str) else class_name
-        )
-    }
+PropsType = TypeVar("PropsType")
+
+
+def _class_name_mapper(class_name):
+    if isinstance(class_name, list):
+        class_name = " ".join(class_name)
+
+    class_name = str(class_name)
+    return {"class": " ".join(class_name.split())}
 
 
-PROPS_MAP = {
-    "class_name": class_name_mapper,
+_PROPS_MAP = {
+    "class_name": _class_name_mapper,
     "html_for": "for",
 }
 
 
-class Element:
-    def __init__(self, *children: "ChildrenType", **kwargs):
-        self.children = children
+class Element(Generic[PropsType]):
+    def __init__(
+        self,
+        *args: "ChildrenType",
+        children: Iterable[Renderable | Primitive] = [],
+        **kwargs: Unpack[PropsType],
+    ):
+        self.children = list(args or children)
         self.props = kwargs
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def tag_name(self) -> str:
         pass
 
     inline = False
 
     def props_dict(self):
         props_copy = self.props.copy()
-        for key, value in PROPS_MAP.items():
+        for key, value in _PROPS_MAP.items():
             if key in props_copy:
                 if callable(value):
                     props_copy.update(value(props_copy.pop(key)))
                 else:
                     props_copy[value] = props_copy.pop(key)
 
         jsx_events = []
@@ -48,11 +59,15 @@
                 key = key.removeprefix("on_")
                 DB.add_element_event(self, key, value)
                 jsx_events.append(key)
             if value is None or value is False:
                 del props_copy[key]
 
         if len(jsx_events) > 0:
-            props_copy["jsx:id"] = DB.element_ids[self]
-            props_copy["jsx:events"] = ",".join(jsx_events)
+            props_copy["slarf:id"] = DB.element_ids[self]
+            props_copy["slarf:events"] = ",".join(jsx_events)
 
         return props_copy
+
+    def __call__(self, *children: "ChildrenType"):
+        self.children = children
+        return self
```

### Comparing `jsx-0.5.0/src/jsx/renderer.py` & `jsx-0.6.0/jsx/renderer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from html import escape
 from typing import TYPE_CHECKING, Any
 from uuid import uuid4 as uuid
 
 from .server.request import request as _request
-
 from .errors import RenderError
 from .components.component import Component
-from .html.element import Element
+from .element import Element
 
 if TYPE_CHECKING:
     from .types import Renderable, Primitive
 
 
 def render(element: "Renderable | Primitive", *, prettify=False, tab_indent=1) -> str:
     request = _request()
@@ -26,15 +25,15 @@
     if not isinstance(element, Element):
         return str(element) if element is not None else ""
 
     tag_name = getattr(element, "tag_name", None)
 
     props = {k: v for k, v in element.props_dict().items() if v not in [None, False]}
 
-    props_string = render_props(props, element)
+    props_string = render_props(props)
     open_tag = f"{tag_name} {props_string}".strip()
 
     if element.inline:
         if len(element.children) > 0:
             # Maybe this should be a warning instead of an error?
             raise RenderError("Inline components cannot have children")
         return f"<{open_tag}>"
@@ -74,33 +73,12 @@
                 element.children,
             )
         ),
         "props": element.props_dict(),
     }
 
 
-def render_props(props: dict[str, Any], element: Element) -> str:
-    DB = _db()
-
-    props_strings = []
-    for key, value in props.items():
-        if callable(value):
-            event = key.removeprefix("on_")
-            DB.add_element_event(element, event, value)
-        elif value is True:
-            props_strings.append(key)
-        else:
-            props_strings.append(f'{key}="{escape(str(value))}"')
-
-    if element in DB.element_ids:
-        subscriptable = DB.get_element(element)
-        props_strings.append(
-            f'jsx:id="{subscriptable.id}" jsx:events="{",".join(subscriptable.events)}"'
-        )
-
-    return " ".join(props_strings)
-
-
-def _db():
-    from .server.database import DB
-
-    return DB
+def render_props(props: dict[str, Any]) -> str:
+    return " ".join(
+        key if value is True else f'{key}="{escape(str(value))}"'
+        for key, value in props.items()
+    )
```

### Comparing `jsx-0.5.0/src/jsx.egg-info/PKG-INFO` & `jsx-0.6.0/jsx.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 Metadata-Version: 2.1
 Name: jsx
-Version: 0.5.0
+Version: 0.6.0
 Summary: A Python package for creating and manipulating HTML components. It is working similar to React.js, but in Python
 Author-email: Xpo Development <dev@xpo.dev>
 Project-URL: Homepage, https://github.com/xpodev/jsx
 Project-URL: Issues, https://github.com/xpodev/jsx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-socketio==5.11.1
+Requires-Dist: cssutils==2.9.0
 
 # Python JSX
 
-[![PyPI version](https://badge.fury.io/py/jsx.svg?)](https://pypi.org/project/jsx)
+[![PyPI version](https://badge.fury.io/py/jsx.svg)](https://pypi.org/project/jsx)
 
-![build](https://github.com/xpodev/pyrl/actions/workflows/python-publish.yml/badge.svg)
 ![test](https://github.com/xpodev/pyrl/actions/workflows/python-test.yml/badge.svg)
 
 JSX is a Python package for creating and manipulating HTML components. It is working similar to React.js, but in Python.
 
+## Installation
+```sh
+pip install jsx
+```
 
 ## Usage
 
 ```python
 from jsx import Div, H1, P, Component, Style
 
 class MyComponent(Component):
@@ -52,15 +57,15 @@
 def hello_world():
   return render(MyComponent())
 ```
 
 ### Server actions
 It's possible to pass a python function as component props.
 
-The current version works with `ASGIApp` and `WSGIApp`.
+The current version works with `ASGIApp`.
 ```python
 class Person(Component):
   def __init__(self, name: str, age: float):
     self.age = age
     self.name = name
 
   def render(self):
@@ -77,18 +82,18 @@
       Button(
         "Submit Age",
         type="submit"
       ),
       on_submit=self.save_age
     )
 
-  def set_age(self, event_data: JSXChangeEvent):
+  def set_age(self, event_data: ChangeEvent):
     self.age = event_data.value
 
-  def save_age(self, event_data: JSXSubmitEvent):
+  def save_age(self, event_data: SubmitEvent):
     user = get_user()
     user.age = self.age
     save(user)
 ```
 To call a function on the server include this script in your file
 ```html
 <script src="/socket.io/static/main.js"></script>
```

### Comparing `jsx-0.5.0/tests/test_rendering.py` & `jsx-0.6.0/tests/test_rendering.py`

 * *Files identical despite different names*

