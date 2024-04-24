# Comparing `tmp/joker-clients-0.2.3.tar.gz` & `tmp/joker-clients-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joker-clients-0.2.3.tar", last modified: Fri Mar 22 08:24:21 2024, max compression
+gzip compressed data, was "joker-clients-0.2.4.tar", last modified: Wed Apr 24 01:01:04 2024, max compression
```

## Comparing `joker-clients-0.2.3.tar` & `joker-clients-0.2.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-03-22 08:24:21.133241 joker-clients-0.2.3/
--rw-r--r--   0 Hailong    (502) staff       (20)    35149 2022-11-02 01:25:38.000000 joker-clients-0.2.3/LICENSE
--rw-r--r--   0 Hailong    (502) staff       (20)       24 2022-11-02 01:25:38.000000 joker-clients-0.2.3/MANIFEST.in
--rw-r--r--   0 Hailong    (502) staff       (20)     1422 2024-03-22 08:24:21.132860 joker-clients-0.2.3/PKG-INFO
--rw-r--r--   0 Hailong    (502) staff       (20)      533 2022-11-02 08:02:40.000000 joker-clients-0.2.3/README.md
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-03-22 08:24:21.121444 joker-clients-0.2.3/joker/
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-03-22 08:24:21.128622 joker-clients-0.2.3/joker/clients/
--rw-r--r--   0 Hailong    (502) staff       (20)      333 2024-03-22 08:23:57.000000 joker-clients-0.2.3/joker/clients/__init__.py
--rw-r--r--   0 Hailong    (502) staff       (20)     2372 2024-03-22 07:54:34.000000 joker-clients-0.2.3/joker/clients/cas.py
--rw-r--r--   0 Hailong    (502) staff       (20)     3366 2024-03-22 07:54:34.000000 joker-clients-0.2.3/joker/clients/email.py
--rw-r--r--   0 Hailong    (502) staff       (20)      386 2024-03-22 07:54:34.000000 joker-clients-0.2.3/joker/clients/files.py
--rw-r--r--   0 Hailong    (502) staff       (20)     3044 2024-03-22 08:21:27.000000 joker-clients-0.2.3/joker/clients/http.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1316 2024-03-22 07:54:34.000000 joker-clients-0.2.3/joker/clients/monolog.py
--rw-r--r--   0 Hailong    (502) staff       (20)     4036 2024-03-22 07:54:34.000000 joker-clients-0.2.3/joker/clients/printable.py
--rw-r--r--   0 Hailong    (502) staff       (20)     3832 2024-03-22 07:54:34.000000 joker-clients-0.2.3/joker/clients/utils.py
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-03-22 08:24:21.132289 joker-clients-0.2.3/joker_clients.egg-info/
--rw-r--r--   0 Hailong    (502) staff       (20)     1422 2024-03-22 08:24:21.000000 joker-clients-0.2.3/joker_clients.egg-info/PKG-INFO
--rw-r--r--   0 Hailong    (502) staff       (20)      511 2024-03-22 08:24:21.000000 joker-clients-0.2.3/joker_clients.egg-info/SOURCES.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        1 2024-03-22 08:24:21.000000 joker-clients-0.2.3/joker_clients.egg-info/dependency_links.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        6 2024-03-22 08:24:21.000000 joker-clients-0.2.3/joker_clients.egg-info/namespace_packages.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        1 2023-07-25 09:13:10.000000 joker-clients-0.2.3/joker_clients.egg-info/not-zip-safe
--rw-r--r--   0 Hailong    (502) staff       (20)       52 2024-03-22 08:24:21.000000 joker-clients-0.2.3/joker_clients.egg-info/requires.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        6 2024-03-22 08:24:21.000000 joker-clients-0.2.3/joker_clients.egg-info/top_level.txt
--rw-r--r--   0 Hailong    (502) staff       (20)       51 2024-03-21 10:39:12.000000 joker-clients-0.2.3/requirements.txt
--rw-r--r--   0 Hailong    (502) staff       (20)       38 2024-03-22 08:24:21.133378 joker-clients-0.2.3/setup.cfg
--rw-r--r--   0 Hailong    (502) staff       (20)     2087 2024-03-22 08:23:35.000000 joker-clients-0.2.3/setup.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-24 01:01:04.795645 joker-clients-0.2.4/
+-rw-r--r--   0 Hailong    (502) staff       (20)    35149 2022-11-02 01:25:38.000000 joker-clients-0.2.4/LICENSE
+-rw-r--r--   0 Hailong    (502) staff       (20)       24 2022-11-02 01:25:38.000000 joker-clients-0.2.4/MANIFEST.in
+-rw-r--r--   0 Hailong    (502) staff       (20)     1422 2024-04-24 01:01:04.795366 joker-clients-0.2.4/PKG-INFO
+-rw-r--r--   0 Hailong    (502) staff       (20)      533 2022-11-02 08:02:40.000000 joker-clients-0.2.4/README.md
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-24 01:01:04.786518 joker-clients-0.2.4/joker/
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-24 01:01:04.792232 joker-clients-0.2.4/joker/clients/
+-rw-r--r--   0 Hailong    (502) staff       (20)      333 2024-04-24 01:00:09.000000 joker-clients-0.2.4/joker/clients/__init__.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     2372 2024-04-24 00:59:51.000000 joker-clients-0.2.4/joker/clients/cas.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     3366 2024-03-22 07:54:34.000000 joker-clients-0.2.4/joker/clients/email.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      386 2024-03-22 07:54:34.000000 joker-clients-0.2.4/joker/clients/files.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     3044 2024-03-22 08:21:27.000000 joker-clients-0.2.4/joker/clients/http.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1316 2024-03-22 07:54:34.000000 joker-clients-0.2.4/joker/clients/monolog.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     4058 2024-04-24 00:59:55.000000 joker-clients-0.2.4/joker/clients/printable.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     3832 2024-04-24 00:59:51.000000 joker-clients-0.2.4/joker/clients/utils.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2024-04-24 01:01:04.794911 joker-clients-0.2.4/joker_clients.egg-info/
+-rw-r--r--   0 Hailong    (502) staff       (20)     1422 2024-04-24 01:01:04.000000 joker-clients-0.2.4/joker_clients.egg-info/PKG-INFO
+-rw-r--r--   0 Hailong    (502) staff       (20)      511 2024-04-24 01:01:04.000000 joker-clients-0.2.4/joker_clients.egg-info/SOURCES.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        1 2024-04-24 01:01:04.000000 joker-clients-0.2.4/joker_clients.egg-info/dependency_links.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        6 2024-04-24 01:01:04.000000 joker-clients-0.2.4/joker_clients.egg-info/namespace_packages.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        1 2023-07-25 09:13:10.000000 joker-clients-0.2.4/joker_clients.egg-info/not-zip-safe
+-rw-r--r--   0 Hailong    (502) staff       (20)       52 2024-04-24 01:01:04.000000 joker-clients-0.2.4/joker_clients.egg-info/requires.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        6 2024-04-24 01:01:04.000000 joker-clients-0.2.4/joker_clients.egg-info/top_level.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)       51 2024-03-21 10:39:12.000000 joker-clients-0.2.4/requirements.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)       38 2024-04-24 01:01:04.795776 joker-clients-0.2.4/setup.cfg
+-rw-r--r--   0 Hailong    (502) staff       (20)     2087 2024-03-22 08:23:35.000000 joker-clients-0.2.4/setup.py
```

### Comparing `joker-clients-0.2.3/LICENSE` & `joker-clients-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `joker-clients-0.2.3/PKG-INFO` & `joker-clients-0.2.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joker-clients
-Version: 0.2.3
+Version: 0.2.4
 Summary: simple clients for simple and dedicated services
 Home-page: https://github.com/frozflame/joker-clients
 Author: frozflame
 Author-email: frozflame@outlook.com
 License: GNU General Public License (GPL)
 Keywords: joker
 Classifier: Programming Language :: Python
```

### Comparing `joker-clients-0.2.3/README.md` & `joker-clients-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `joker-clients-0.2.3/joker/clients/cas.py` & `joker-clients-0.2.4/joker/clients/cas.py`

 * *Files identical despite different names*

### Comparing `joker-clients-0.2.3/joker/clients/email.py` & `joker-clients-0.2.4/joker/clients/email.py`

 * *Files identical despite different names*

### Comparing `joker-clients-0.2.3/joker/clients/http.py` & `joker-clients-0.2.4/joker/clients/http.py`

 * *Files identical despite different names*

### Comparing `joker-clients-0.2.3/joker/clients/monolog.py` & `joker-clients-0.2.4/joker/clients/monolog.py`

 * *Files identical despite different names*

### Comparing `joker-clients-0.2.3/joker/clients/printable.py` & `joker-clients-0.2.4/joker/clients/printable.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         except KeyError:
             raise RuntimeError(f"failed to render {url!r}")
         return PrintableTask(self, tpl_path, ctxid)
 
     def _generate(self, tpl_path: str, data: dict) -> tuple[bytes, str]:
         url = urljoin(self.inner_url, tpl_path)
         _logger.info("initial url: %r", url)
-        resp = self._post_as_json(url, data)
+        resp = self._post_as_json(url, data, allow_redirects=True)
         _logger.info("redirected url: %r", resp.url)
         _logger.info(
             "content: %s bytes, %r",
             len(resp.content),
             resp.content[:100],
         )
         if not utils.check_pdf_validity(resp.content):
```

### Comparing `joker-clients-0.2.3/joker/clients/utils.py` & `joker-clients-0.2.4/joker/clients/utils.py`

 * *Files identical despite different names*

### Comparing `joker-clients-0.2.3/joker_clients.egg-info/PKG-INFO` & `joker-clients-0.2.4/joker_clients.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joker-clients
-Version: 0.2.3
+Version: 0.2.4
 Summary: simple clients for simple and dedicated services
 Home-page: https://github.com/frozflame/joker-clients
 Author: frozflame
 Author-email: frozflame@outlook.com
 License: GNU General Public License (GPL)
 Keywords: joker
 Classifier: Programming Language :: Python
```

### Comparing `joker-clients-0.2.3/setup.py` & `joker-clients-0.2.4/setup.py`

 * *Files identical despite different names*

