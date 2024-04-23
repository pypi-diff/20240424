# Comparing `tmp/jsx-0.6.1.tar.gz` & `tmp/jsx-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsx-0.6.1.tar", last modified: Tue Apr 23 23:09:35 2024, max compression
+gzip compressed data, was "jsx-0.6.2.tar", last modified: Tue Apr 23 23:15:39 2024, max compression
```

## Comparing `jsx-0.6.1.tar` & `jsx-0.6.2.tar`

### file list

```diff
@@ -1,112 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:09:35.369462 jsx-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-23 23:09:28.000000 jsx-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-23 23:09:35.369462 jsx-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-23 23:09:28.000000 jsx-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:09:35.349461 jsx-0.6.1/jsx/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:09:35.349461 jsx-0.6.1/jsx/components/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/components/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/components/page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:09:35.365462 jsx-0.6.1/jsx/html/
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/_auto_html.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/a.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/abbr.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/address.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/area.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/article.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/aside.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/b.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/base.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/blockquote.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/body.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/br.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/button.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/cite.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/code.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/col.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/div.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/em.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/embed.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/footer.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/form.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/fragment.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/h1.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/h2.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/h3.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/h4.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/h5.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/h6.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/head.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/header.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/hr.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/html.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/i.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/img.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/input.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/label.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/li.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/link.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/main.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/nav.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/ol.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/option.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/p.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/param.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/pre.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/script.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/section.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/select.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/small.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/source.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/span.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/strong.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/sub.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/sup.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/table.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/tbody.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/td.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/textarea.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/th.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/thead.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/time.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/title.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/tr.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/track.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/u.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/ul.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/html/wbr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:09:35.369462 jsx-0.6.1/jsx/jsx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-23 23:09:35.000000 jsx-0.6.1/jsx/jsx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-23 23:09:35.000000 jsx-0.6.1/jsx/jsx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 23:09:35.000000 jsx-0.6.1/jsx/jsx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-23 23:09:35.000000 jsx-0.6.1/jsx/jsx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 23:09:35.000000 jsx-0.6.1/jsx/jsx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:09:35.365462 jsx-0.6.1/jsx/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/middlewares/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/middlewares/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:09:35.365462 jsx-0.6.1/jsx/server/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/server/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/server/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/server/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/server/ws_router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:09:35.365462 jsx-0.6.1/jsx/styling/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/styling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/styling/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/styling/css_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/styling/style.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:09:35.365462 jsx-0.6.1/jsx/types/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/types/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    10941 2024-04-23 23:09:28.000000 jsx-0.6.1/jsx/types/html.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-23 23:09:28.000000 jsx-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-23 23:09:28.000000 jsx-0.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 23:09:35.369462 jsx-0.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:09:35.369462 jsx-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-23 23:09:28.000000 jsx-0.6.1/tests/test_asgi_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-23 23:09:28.000000 jsx-0.6.1/tests/test_nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-04-23 23:09:28.000000 jsx-0.6.1/tests/test_rendering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:15:39.363992 jsx-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-23 23:15:31.000000 jsx-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-23 23:15:39.363992 jsx-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-23 23:15:31.000000 jsx-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:15:39.363992 jsx-0.6.2/jsx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-23 23:15:39.000000 jsx-0.6.2/jsx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-23 23:15:39.000000 jsx-0.6.2/jsx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 23:15:39.000000 jsx-0.6.2/jsx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-23 23:15:39.000000 jsx-0.6.2/jsx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-23 23:15:39.000000 jsx-0.6.2/jsx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-23 23:15:31.000000 jsx-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-23 23:15:31.000000 jsx-0.6.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 23:15:39.363992 jsx-0.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 23:15:39.363992 jsx-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-23 23:15:31.000000 jsx-0.6.2/tests/test_asgi_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-23 23:15:31.000000 jsx-0.6.2/tests/test_nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-04-23 23:15:31.000000 jsx-0.6.2/tests/test_rendering.py
```

### Comparing `jsx-0.6.1/LICENSE` & `jsx-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jsx-0.6.1/PKG-INFO` & `jsx-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsx
-Version: 0.6.1
+Version: 0.6.2
 Summary: A Python package for creating and manipulating HTML components. It is working similar to React.js, but in Python
 Author-email: Xpo Development <dev@xpo.dev>
 Project-URL: Homepage, https://github.com/xpodev/jsx
 Project-URL: Issues, https://github.com/xpodev/jsx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jsx-0.6.1/README.md` & `jsx-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `jsx-0.6.1/jsx/jsx.egg-info/PKG-INFO` & `jsx-0.6.2/jsx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsx
-Version: 0.6.1
+Version: 0.6.2
 Summary: A Python package for creating and manipulating HTML components. It is working similar to React.js, but in Python
 Author-email: Xpo Development <dev@xpo.dev>
 Project-URL: Homepage, https://github.com/xpodev/jsx
 Project-URL: Issues, https://github.com/xpodev/jsx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jsx-0.6.1/pyproject.toml` & `jsx-0.6.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jsx"
-version = "0.6.1"
+version = "0.6.2"
 authors = [
   { name="Xpo Development", email="dev@xpo.dev" },
 ]
 description = "A Python package for creating and manipulating HTML components. It is working similar to React.js, but in Python"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -14,12 +14,12 @@
 ]
 dynamic = ["dependencies"]
 
 [project.urls]
 Homepage = "https://github.com/xpodev/jsx"
 Issues = "https://github.com/xpodev/jsx/issues"
 
-[tool.setuptools.packages.find]
-where = ["jsx"]
+[tool.setuptools]
+py-modules = ["jsx"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
```

### Comparing `jsx-0.6.1/tests/test_rendering.py` & `jsx-0.6.2/tests/test_rendering.py`

 * *Files identical despite different names*

