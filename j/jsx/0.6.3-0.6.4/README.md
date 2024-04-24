# Comparing `tmp/jsx-0.6.3.tar.gz` & `tmp/jsx-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsx-0.6.3.tar", last modified: Tue Apr 23 23:21:50 2024, max compression
+gzip compressed data, was "jsx-0.6.4.tar", last modified: Wed Apr 24 00:28:11 2024, max compression
```

## Comparing `jsx-0.6.3.tar` & `jsx-0.6.4.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:50.918844 jsx-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-23 23:21:45.000000 jsx-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-23 23:21:50.918844 jsx-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-23 23:21:45.000000 jsx-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:50.902844 jsx-0.6.3/jsx/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:50.902844 jsx-0.6.3/jsx/components/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/components/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/components/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/element.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:50.914844 jsx-0.6.3/jsx/html/
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/_auto_html.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/a.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/abbr.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/address.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/area.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/article.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/aside.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/b.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/base.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/blockquote.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/body.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/br.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/button.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/cite.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/code.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/col.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/div.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/em.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/embed.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/footer.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/form.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/fragment.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/h1.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/h2.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/h3.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/h4.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/h5.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/h6.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/head.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/header.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/hr.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/html.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/i.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/img.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/input.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/label.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/li.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/link.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/main.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/nav.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/ol.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/option.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/p.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/param.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/pre.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/script.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/section.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/select.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/small.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/source.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/span.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/strong.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/sub.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/sup.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/table.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/tbody.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/td.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/textarea.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/th.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/thead.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/time.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/title.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/tr.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/track.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/u.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/ul.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/html/wbr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:50.914844 jsx-0.6.3/jsx/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/middlewares/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/middlewares/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:50.918844 jsx-0.6.3/jsx/server/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/server/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/server/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/server/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/server/ws_router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:50.918844 jsx-0.6.3/jsx/styling/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/styling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/styling/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/styling/css_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/styling/style.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:50.918844 jsx-0.6.3/jsx/types/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/types/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    10941 2024-04-23 23:21:45.000000 jsx-0.6.3/jsx/types/html.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:50.918844 jsx-0.6.3/jsx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-23 23:21:50.000000 jsx-0.6.3/jsx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-23 23:21:50.000000 jsx-0.6.3/jsx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 23:21:50.000000 jsx-0.6.3/jsx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-23 23:21:50.000000 jsx-0.6.3/jsx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-23 23:21:50.000000 jsx-0.6.3/jsx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-23 23:21:45.000000 jsx-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-23 23:21:45.000000 jsx-0.6.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 23:21:50.918844 jsx-0.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:21:50.918844 jsx-0.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-23 23:21:45.000000 jsx-0.6.3/tests/test_asgi_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-23 23:21:45.000000 jsx-0.6.3/tests/test_nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-04-23 23:21:45.000000 jsx-0.6.3/tests/test_rendering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:28:11.052363 jsx-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-24 00:28:04.000000 jsx-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-24 00:28:11.052363 jsx-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-24 00:28:04.000000 jsx-0.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:28:11.036363 jsx-0.6.4/jsx/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:28:11.036363 jsx-0.6.4/jsx/components/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/components/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:28:11.048363 jsx-0.6.4/jsx/html/
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/_auto_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/a.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/abbr.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/area.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/article.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/aside.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/b.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/blockquote.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/body.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/br.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/cite.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/col.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/div.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/em.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/footer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/fragment.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/h1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/h2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/h3.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/h4.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/h5.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/h6.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/head.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/hr.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/i.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/img.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/li.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/nav.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/ol.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/option.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/p.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/param.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/pre.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/section.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/small.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/span.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/strong.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/sup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/tbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/td.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/textarea.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/th.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/thead.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/title.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/tr.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/u.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/ul.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/html/wbr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:28:11.048363 jsx-0.6.4/jsx/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/middlewares/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/middlewares/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:28:11.048363 jsx-0.6.4/jsx/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/server/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/server/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/server/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/server/ws_router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:28:11.052363 jsx-0.6.4/jsx/styling/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/styling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/styling/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/styling/css_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/styling/style.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:28:11.052363 jsx-0.6.4/jsx/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/types/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10941 2024-04-24 00:28:04.000000 jsx-0.6.4/jsx/types/html.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:28:11.052363 jsx-0.6.4/jsx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-24 00:28:11.000000 jsx-0.6.4/jsx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-24 00:28:11.000000 jsx-0.6.4/jsx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 00:28:11.000000 jsx-0.6.4/jsx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-24 00:28:11.000000 jsx-0.6.4/jsx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-24 00:28:11.000000 jsx-0.6.4/jsx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-24 00:28:04.000000 jsx-0.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-24 00:28:04.000000 jsx-0.6.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 00:28:11.052363 jsx-0.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:28:11.052363 jsx-0.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-24 00:28:04.000000 jsx-0.6.4/tests/test_asgi_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-24 00:28:04.000000 jsx-0.6.4/tests/test_nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-04-24 00:28:04.000000 jsx-0.6.4/tests/test_rendering.py
```

### Comparing `jsx-0.6.3/LICENSE` & `jsx-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jsx-0.6.3/PKG-INFO` & `jsx-0.6.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsx
-Version: 0.6.3
+Version: 0.6.4
 Summary: A Python package for creating and manipulating HTML components. It is working similar to React.js, but in Python
 Author-email: Xpo Development <dev@xpo.dev>
 Project-URL: Homepage, https://github.com/xpodev/jsx
 Project-URL: Issues, https://github.com/xpodev/jsx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jsx-0.6.3/README.md` & `jsx-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `jsx-0.6.3/jsx/components/component.py` & `jsx-0.6.4/jsx/components/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     def __init_subclass__(cls) -> None:
         if cls.__init__ is ContainerComponent.__init__:
             return
         
         original_init = cls.__init__
 
         def __init__(self, *args, children=None, **kwargs):
+            children = getattr(self, "children", None) or children
             ContainerComponent.__init__(self, *(children or args))
             original_init(self, **kwargs)
         
         cls.__init__ = __init__
             
     def __call__(self, *children: "ChildrenType"):
         self.children = children
```

### Comparing `jsx-0.6.3/jsx/components/page.py` & `jsx-0.6.4/jsx/components/page.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import Literal, TypedDict
-from jsx import (
+from .base import (
     ContainerComponent,
+)
+from ..html import (
     Fragment,
     Html,
     Head,
     Title,
     Body,
     Meta,
 )
```

### Comparing `jsx-0.6.3/jsx/element.py` & `jsx-0.6.4/jsx/element.py`

 * *Files identical despite different names*

### Comparing `jsx-0.6.3/jsx/html/__init__.py` & `jsx-0.6.4/jsx/html/__init__.py`

 * *Files identical despite different names*

### Comparing `jsx-0.6.3/jsx/internal.py` & `jsx-0.6.4/jsx/internal.py`

 * *Files identical despite different names*

### Comparing `jsx-0.6.3/jsx/middlewares/asgi.py` & `jsx-0.6.4/jsx/middlewares/asgi.py`

 * *Files identical despite different names*

### Comparing `jsx-0.6.3/jsx/middlewares/base.py` & `jsx-0.6.4/jsx/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `jsx-0.6.3/jsx/renderer.py` & `jsx-0.6.4/jsx/renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from html import escape
 from typing import TYPE_CHECKING, Any
 from uuid import uuid4 as uuid
 
 from .server.request import request as _request
 from .errors import RenderError
-from .components.component import Component
+from .components.base import Component
 from .element import Element
 
 if TYPE_CHECKING:
     from .types import Renderable, Primitive
 
 
 def render(element: "Renderable | Primitive", *, prettify=False, tab_indent=1) -> str:
```

### Comparing `jsx-0.6.3/jsx/server/database.py` & `jsx-0.6.4/jsx/server/database.py`

 * *Files identical despite different names*

### Comparing `jsx-0.6.3/jsx/server/request.py` & `jsx-0.6.4/jsx/server/request.py`

 * *Files identical despite different names*

### Comparing `jsx-0.6.3/jsx/server/ws_router.py` & `jsx-0.6.4/jsx/server/ws_router.py`

 * *Files identical despite different names*

### Comparing `jsx-0.6.3/jsx/styling/color.py` & `jsx-0.6.4/jsx/styling/color.py`

 * *Files identical despite different names*

### Comparing `jsx-0.6.3/jsx/styling/css_modules.py` & `jsx-0.6.4/jsx/styling/css_modules.py`

 * *Files identical despite different names*

### Comparing `jsx-0.6.3/jsx/styling/style.py` & `jsx-0.6.4/jsx/styling/style.py`

 * *Files identical despite different names*

### Comparing `jsx-0.6.3/jsx/types/html.py` & `jsx-0.6.4/jsx/types/html.py`

 * *Files identical despite different names*

### Comparing `jsx-0.6.3/jsx.egg-info/PKG-INFO` & `jsx-0.6.4/jsx.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsx
-Version: 0.6.3
+Version: 0.6.4
 Summary: A Python package for creating and manipulating HTML components. It is working similar to React.js, but in Python
 Author-email: Xpo Development <dev@xpo.dev>
 Project-URL: Homepage, https://github.com/xpodev/jsx
 Project-URL: Issues, https://github.com/xpodev/jsx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jsx-0.6.3/jsx.egg-info/SOURCES.txt` & `jsx-0.6.4/jsx.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 jsx/renderer.py
 jsx.egg-info/PKG-INFO
 jsx.egg-info/SOURCES.txt
 jsx.egg-info/dependency_links.txt
 jsx.egg-info/requires.txt
 jsx.egg-info/top_level.txt
 jsx/components/__init__.py
-jsx/components/component.py
+jsx/components/base.py
 jsx/components/page.py
 jsx/html/__init__.py
 jsx/html/_auto_html.py
 jsx/html/a.py
 jsx/html/abbr.py
 jsx/html/address.py
 jsx/html/area.py
```

### Comparing `jsx-0.6.3/pyproject.toml` & `jsx-0.6.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jsx"
-version = "0.6.3"
+version = "0.6.4"
 authors = [
   { name="Xpo Development", email="dev@xpo.dev" },
 ]
 description = "A Python package for creating and manipulating HTML components. It is working similar to React.js, but in Python"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `jsx-0.6.3/tests/test_rendering.py` & `jsx-0.6.4/tests/test_rendering.py`

 * *Files identical despite different names*

