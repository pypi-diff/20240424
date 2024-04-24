# Comparing `tmp/vite_transporter-0.4.2.tar.gz` & `tmp/vite_transporter-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vite_transporter-0.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vite_transporter-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vite_transporter-0.4.2.tar` & `vite_transporter-0.5.0.tar`

### file list

```diff
@@ -1,36 +1,33 @@
--rw-r--r--   0        0        0     5201 2024-04-17 20:37:21.973545 vite_transporter-0.4.2/.gitignore
--rw-r--r--   0        0        0     1083 2024-03-29 08:24:35.046180 vite_transporter-0.4.2/LICENSE
--rw-r--r--   0        0        0     4078 2024-04-23 17:38:10.489230 vite_transporter-0.4.2/README.md
--rw-r--r--   0        0        0      738 2024-04-21 15:32:14.759993 vite_transporter-0.4.2/app_flask_demo/__init__.py
--rw-r--r--   0        0        0      192 2024-04-17 19:56:25.368755 vite_transporter-0.4.2/app_flask_demo/templates/index.html
--rw-r--r--   0        0        0    39139 2024-04-23 17:26:19.313411 vite_transporter-0.4.2/app_flask_demo/vt/app_vite_demo/ili-85e34484.gif
--rw-r--r--   0        0        0    21365 2024-04-23 17:26:19.313250 vite_transporter-0.4.2/app_flask_demo/vt/app_vite_demo/index-45b871c7.js
--rw-r--r--   0        0        0    33644 2024-04-23 17:26:19.312967 vite_transporter-0.4.2/app_flask_demo/vt/app_vite_demo/index-cc24c663.css
--rw-r--r--   0        0        0      750 2024-04-21 15:32:40.857714 vite_transporter-0.4.2/app_quart_demo/__init__.py
--rw-r--r--   0        0        0      192 2024-04-17 19:56:29.985721 vite_transporter-0.4.2/app_quart_demo/templates/index.html
--rw-r--r--   0        0        0    39139 2024-04-17 19:55:40.663413 vite_transporter-0.4.2/app_quart_demo/vt/app_vite_demo/ili-85e34484.gif
--rw-r--r--   0        0        0    33329 2024-04-17 19:55:40.663791 vite_transporter-0.4.2/app_quart_demo/vt/app_vite_demo/index-621914e8.css
--rw-r--r--   0        0        0    20285 2024-04-17 19:55:40.663651 vite_transporter-0.4.2/app_quart_demo/vt/app_vite_demo/index-6e585489.js
--rw-r--r--   0        0        0     2250 2024-04-21 15:33:39.440720 vite_transporter-0.4.2/app_vite_demo/Index.jsx
--rw-r--r--   0        0        0      536 2024-04-12 20:35:46.642592 vite_transporter-0.4.2/app_vite_demo/__router__.jsx
--rw-r--r--   0        0        0    39139 2024-03-12 16:01:48.215679 vite_transporter-0.4.2/app_vite_demo/assets/ili.gif
--rw-r--r--   0        0        0      596 2024-04-21 15:30:17.354196 vite_transporter-0.4.2/app_vite_demo/index.css
--rw-r--r--   0        0        0      414 2024-04-17 19:46:30.300521 vite_transporter-0.4.2/app_vite_demo/index.html
--rw-r--r--   0        0        0   105659 2024-04-23 17:26:15.620700 vite_transporter-0.4.2/app_vite_demo/package-lock.json
--rw-r--r--   0        0        0      570 2024-04-12 14:55:15.273422 vite_transporter-0.4.2/app_vite_demo/package.json
--rw-r--r--   0        0        0       80 2024-02-23 14:52:24.766425 vite_transporter-0.4.2/app_vite_demo/postcss.config.js
--rw-r--r--   0        0        0      151 2024-03-31 09:45:49.055622 vite_transporter-0.4.2/app_vite_demo/tailwind.config.js
--rw-r--r--   0        0        0      440 2024-04-01 09:05:29.649936 vite_transporter-0.4.2/app_vite_demo/vite.config.js
--rw-r--r--   0        0        0     1257 2024-04-21 15:37:04.537415 vite_transporter-0.4.2/pyproject.toml
--rw-r--r--   0        0        0       31 2024-04-17 20:14:50.246973 vite_transporter-0.4.2/requirements/demos.txt
--rw-r--r--   0        0        0       22 2024-04-17 20:14:46.286993 vite_transporter-0.4.2/requirements/development.txt
--rw-r--r--   0        0        0       34 2024-04-17 16:11:12.368549 vite_transporter-0.4.2/requirements/main.txt
--rw-r--r--   0        0        0     2185 2024-04-23 17:38:19.453468 vite_transporter-0.4.2/vite_transporter/__init__.py
--rw-r--r--   0        0        0     2654 2024-04-21 13:26:49.370076 vite_transporter-0.4.2/vite_transporter/_headers.py
--rw-r--r--   0        0        0     4871 2024-04-03 07:34:32.709087 vite_transporter-0.4.2/vite_transporter/_html_tags.py
--rw-r--r--   0        0        0     4002 2024-04-17 20:42:01.707392 vite_transporter-0.4.2/vite_transporter/helpers.py
--rw-r--r--   0        0        0      909 2024-04-17 15:48:32.502792 vite_transporter-0.4.2/vite_transporter/parser.py
--rw-r--r--   0        0        0      178 2024-04-23 08:21:21.096283 vite_transporter-0.4.2/vite_transporter/platform/__init__.py
--rw-r--r--   0        0        0     4679 2024-04-23 08:25:01.100158 vite_transporter-0.4.2/vite_transporter/platform/flask.py
--rw-r--r--   0        0        0     4743 2024-04-23 08:25:01.103735 vite_transporter-0.4.2/vite_transporter/platform/quart.py
--rw-r--r--   0        0        0     4760 1970-01-01 00:00:00.000000 vite_transporter-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     5201 2024-04-17 20:37:21.973545 vite_transporter-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1083 2024-03-29 08:24:35.046180 vite_transporter-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4078 2024-04-23 17:38:10.489230 vite_transporter-0.5.0/README.md
+-rw-r--r--   0        0        0      738 2024-04-21 15:32:14.759993 vite_transporter-0.5.0/app_flask_demo/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-17 19:56:25.368755 vite_transporter-0.5.0/app_flask_demo/templates/index.html
+-rw-r--r--   0        0        0    39139 2024-04-23 17:26:19.313411 vite_transporter-0.5.0/app_flask_demo/vt/app_vite_demo/ili-85e34484.gif
+-rw-r--r--   0        0        0    21365 2024-04-23 17:26:19.313250 vite_transporter-0.5.0/app_flask_demo/vt/app_vite_demo/index-45b871c7.js
+-rw-r--r--   0        0        0    33644 2024-04-23 17:26:19.312967 vite_transporter-0.5.0/app_flask_demo/vt/app_vite_demo/index-cc24c663.css
+-rw-r--r--   0        0        0      750 2024-04-21 15:32:40.857714 vite_transporter-0.5.0/app_quart_demo/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-17 19:56:29.985721 vite_transporter-0.5.0/app_quart_demo/templates/index.html
+-rw-r--r--   0        0        0    39139 2024-04-17 19:55:40.663413 vite_transporter-0.5.0/app_quart_demo/vt/app_vite_demo/ili-85e34484.gif
+-rw-r--r--   0        0        0    33329 2024-04-17 19:55:40.663791 vite_transporter-0.5.0/app_quart_demo/vt/app_vite_demo/index-621914e8.css
+-rw-r--r--   0        0        0    20285 2024-04-17 19:55:40.663651 vite_transporter-0.5.0/app_quart_demo/vt/app_vite_demo/index-6e585489.js
+-rw-r--r--   0        0        0     2250 2024-04-21 15:33:39.440720 vite_transporter-0.5.0/app_vite_demo/Index.jsx
+-rw-r--r--   0        0        0      536 2024-04-12 20:35:46.642592 vite_transporter-0.5.0/app_vite_demo/__router__.jsx
+-rw-r--r--   0        0        0    39139 2024-03-12 16:01:48.215679 vite_transporter-0.5.0/app_vite_demo/assets/ili.gif
+-rw-r--r--   0        0        0      596 2024-04-21 15:30:17.354196 vite_transporter-0.5.0/app_vite_demo/index.css
+-rw-r--r--   0        0        0      414 2024-04-17 19:46:30.300521 vite_transporter-0.5.0/app_vite_demo/index.html
+-rw-r--r--   0        0        0   105659 2024-04-23 17:26:15.620700 vite_transporter-0.5.0/app_vite_demo/package-lock.json
+-rw-r--r--   0        0        0      570 2024-04-12 14:55:15.273422 vite_transporter-0.5.0/app_vite_demo/package.json
+-rw-r--r--   0        0        0       80 2024-02-23 14:52:24.766425 vite_transporter-0.5.0/app_vite_demo/postcss.config.js
+-rw-r--r--   0        0        0      151 2024-03-31 09:45:49.055622 vite_transporter-0.5.0/app_vite_demo/tailwind.config.js
+-rw-r--r--   0        0        0      440 2024-04-01 09:05:29.649936 vite_transporter-0.5.0/app_vite_demo/vite.config.js
+-rw-r--r--   0        0        0     1262 2024-04-24 06:07:20.779037 vite_transporter-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       31 2024-04-17 20:14:50.246973 vite_transporter-0.5.0/requirements/demos.txt
+-rw-r--r--   0        0        0       22 2024-04-17 20:14:46.286993 vite_transporter-0.5.0/requirements/development.txt
+-rw-r--r--   0        0        0       34 2024-04-17 16:11:12.368549 vite_transporter-0.5.0/requirements/main.txt
+-rw-r--r--   0        0        0     2079 2024-04-24 06:07:31.419104 vite_transporter-0.5.0/vite_transporter/__init__.py
+-rw-r--r--   0        0        0      178 2024-04-23 08:21:21.096283 vite_transporter-0.5.0/vite_transporter/platform/__init__.py
+-rw-r--r--   0        0        0     4721 2024-04-24 06:06:36.654452 vite_transporter-0.5.0/vite_transporter/platform/flask.py
+-rw-r--r--   0        0        0     4785 2024-04-24 06:06:49.254712 vite_transporter-0.5.0/vite_transporter/platform/quart.py
+-rw-r--r--   0        0        0    10208 2024-04-24 06:06:49.255249 vite_transporter-0.5.0/vite_transporter/utilities.py
+-rw-r--r--   0        0        0     4760 1970-01-01 00:00:00.000000 vite_transporter-0.5.0/PKG-INFO
```

### Comparing `vite_transporter-0.4.2/.gitignore` & `vite_transporter-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.2/LICENSE` & `vite_transporter-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.2/README.md` & `vite_transporter-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.2/app_flask_demo/__init__.py` & `vite_transporter-0.5.0/app_flask_demo/__init__.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.2/app_flask_demo/vt/app_vite_demo/ili-85e34484.gif` & `vite_transporter-0.5.0/app_flask_demo/vt/app_vite_demo/ili-85e34484.gif`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.2/app_flask_demo/vt/app_vite_demo/index-45b871c7.js` & `vite_transporter-0.5.0/app_flask_demo/vt/app_vite_demo/index-45b871c7.js`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.2/app_flask_demo/vt/app_vite_demo/index-cc24c663.css` & `vite_transporter-0.5.0/app_flask_demo/vt/app_vite_demo/index-cc24c663.css`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.2/app_quart_demo/__init__.py` & `vite_transporter-0.5.0/app_quart_demo/__init__.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.2/app_quart_demo/vt/app_vite_demo/ili-85e34484.gif` & `vite_transporter-0.5.0/app_quart_demo/vt/app_vite_demo/ili-85e34484.gif`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.2/app_quart_demo/vt/app_vite_demo/index-621914e8.css` & `vite_transporter-0.5.0/app_quart_demo/vt/app_vite_demo/index-621914e8.css`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.2/app_quart_demo/vt/app_vite_demo/index-6e585489.js` & `vite_transporter-0.5.0/app_quart_demo/vt/app_vite_demo/index-6e585489.js`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.2/app_vite_demo/Index.jsx` & `vite_transporter-0.5.0/app_vite_demo/Index.jsx`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.2/app_vite_demo/__router__.jsx` & `vite_transporter-0.5.0/app_vite_demo/__router__.jsx`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.2/app_vite_demo/assets/ili.gif` & `vite_transporter-0.5.0/app_vite_demo/assets/ili.gif`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.2/app_vite_demo/index.css` & `vite_transporter-0.5.0/app_vite_demo/index.css`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.2/app_vite_demo/package-lock.json` & `vite_transporter-0.5.0/app_vite_demo/package-lock.json`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.2/app_vite_demo/package.json` & `vite_transporter-0.5.0/app_vite_demo/package.json`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.2/pyproject.toml` & `vite_transporter-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 dynamic = ["version"]
 
 [project.optional-dependencies]
 flask = ["flask"]
 quart = ["quart"]
 
 [project.scripts]
-vt = "vite_transporter:_cli"
+vt = "vite_transporter:cli_entry"
 
 [tool.pyqwe]
 vite = "*(app_vite_demo):npx vite --host 127.0.0.1 --port 5003"
 flask = "*:flask --app app_flask_demo run --host 127.0.0.1 --port 5001 --debug"
 quart = "*:quart --app app_quart_demo run --host 127.0.0.1 --port 5002"
 install = "*:flit install --symlink"
 build = "*:flit build"
```

### Comparing `vite_transporter-0.4.2/vite_transporter/__init__.py` & `vite_transporter-0.5.0/vite_transporter/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,72 +1,78 @@
 import sys
 
-from .helpers import Colr as _Colr
-from .helpers import PyProjectConfig as _PyProjectConfig
-from .helpers import _compile
-from .parser import ArgumentParser as _ArgumentParser
+from .utilities import ArgumentParser as _ArgumentParser
+from .utilities import Colr as _Colr
+from .utilities import PyProjectConfig as _PyProjectConfig
+from .utilities import compiler
 
-__version__ = "0.4.2"
+__version__ = "0.5.0"
 
 
-def _cli():
+def setup_subparsers(pars):
+    subparsers = pars.add_subparsers()
+
+    subparsers.add_parser("compile").set_defaults(compile=False).add_argument(
+        "-y", action="store_true"
+    )
+    subparsers.add_parser("list").set_defaults(list=False)
+    subparsers.add_parser("ls").set_defaults(list=False)
+
+
+def load_vite_apps(pyproject):
+    for vite_app in pyproject.vite_apps:
+        pyproject.vite_apps.append(
+            {
+                "vite_app": vite_app,
+                "serve_app": pyproject.vt_config.get("serve_app"),
+            }
+        )
+
+
+def list_ls(pars):
+    print("")
+    if not pars.vite_apps:
+        print(f" {_Colr.WARNING}No vite apps found in pyproject.toml{_Colr.END}")
+    else:
+        for app in pars.vite_apps:
+            print(
+                f"{_Colr.OKGREEN}{app.get('vite_app')}/dist/assets{_Colr.END} "
+                f"{_Colr.BOLD}=>{_Colr.END} "
+                f"{_Colr.OKGREEN}{app.get('serve_app')}/vt/{app.get('vite_app')}/{_Colr.END}"
+            )
+    print("")
+    sys.exit(0)
+
+
+def compile_(pyproject, pars, args):
+    compiler(
+        pyproject,
+        pars.vite_apps,
+        replace=True if hasattr(args, "y") and args.y else False,
+    )
+    sys.exit(0)
+
+
+def cli_entry():
     pars = _ArgumentParser(prog="vtf", add_help=False)
     pars.add_argument(
         "--version", "-v", action="version", version=f"vite-to-flask {__version__}"
     )
     pars.add_argument("--help", "-h", action="help")
 
-    subparsers = pars.add_subparsers()
-
-    compile_parser = subparsers.add_parser("compile")
-    compile_parser.set_defaults(compile=False)
-    compile_parser.add_argument("-y", action="store_true")
-
-    list_parser = subparsers.add_parser("list")
-    list_parser.set_defaults(list=False)
-
-    ls_parser = subparsers.add_parser("ls")
-    ls_parser.set_defaults(list=False)
+    setup_subparsers(pars)
 
     with _PyProjectConfig() as pyproject:
         pypro: _PyProjectConfig = pyproject
 
-        for vite_app in pypro.vite_apps:
-            pars.vite_apps.append(
-                {
-                    "vite_app": vite_app,
-                    "serve_app": pypro.vt_config.get("serve_app"),
-                }
-            )
+        load_vite_apps(pypro)
 
         args = pars.parse_args()
 
         if hasattr(args, "compile"):
-            _compile(
-                pyproject,
-                pars.vite_apps,
-                replace=True if hasattr(args, "y") and args.y else False,
-            )
-
-            # exit after compiling
-            sys.exit(0)
+            compile_(pypro, pars, args)
 
         if hasattr(args, "list") or hasattr(args, "ls"):
-            print("")
-            if not pars.vite_apps:
-                print(
-                    f" {_Colr.WARNING}No vite apps found in pyproject.toml{_Colr.END}"
-                )
-            else:
-                for app in pars.vite_apps:
-                    print(
-                        f"{_Colr.OKGREEN}{app.get('vite_app')}/dist/assets{_Colr.END} "
-                        f"{_Colr.BOLD}=>{_Colr.END} "
-                        f"{_Colr.OKGREEN}{app.get('serve_app')}/vt/{app.get('vite_app')}/{_Colr.END}"
-                    )
-            print("")
-
-            # exit after listing
-            sys.exit(0)
+            list_ls(pars)
 
     # print help if no command is given
     pars.print_help()
```

### Comparing `vite_transporter-0.4.2/vite_transporter/platform/flask.py` & `vite_transporter-0.5.0/vite_transporter/platform/flask.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 if "flask" in sys.modules:
     from flask import Flask, url_for, send_from_directory
     from markupsafe import Markup
 else:
     raise ImportError("Flask is not installed.")
 
-from vite_transporter._html_tags import BodyContent, ScriptTag, LinkTag
-from vite_transporter.helpers import Colr
-from vite_transporter._headers import http_headers
+from vite_transporter.utilities import BodyContent, ScriptTag, LinkTag
+from vite_transporter.utilities import Colr
+from vite_transporter.utilities import http_headers
 
 
 class ViteTransporter:
     app: t.Optional[Flask]
     vt_root_path: Path
 
     cors_allowed_hosts: list = None
 
     def __init__(
-            self, app: t.Optional[Flask] = None, cors_allowed_hosts: t.Optional[list] = None
+        self, app: t.Optional[Flask] = None, cors_allowed_hosts: t.Optional[list] = None
     ) -> None:
         if app is not None:
             self.init_app(app, cors_allowed_hosts)
 
     def init_app(self, app: Flask, cors_allowed_hosts: t.Optional[list] = None) -> None:
         if app is None:
             raise ImportError("No app was passed in.")
@@ -97,32 +97,36 @@
                 return Markup("".join([tag.raw() for tag in tags]))
 
             return dict(vt_head=vt_head)
 
         @app.context_processor
         def vt_body_processor():
             def vt_body(
-                    root_id: str = "root",
-                    noscript_message: str = "You need to enable JavaScript to run this app.",
+                root_id: str = "root",
+                noscript_message: str = "You need to enable JavaScript to run this app.",
             ) -> t.Any:
                 return BodyContent(root_id, noscript_message)()
 
             return dict(vt_body=vt_body)
 
     @staticmethod
-    def _load_cors_headers(app: Flask, cors_allowed_hosts: t.Optional[list] = None) -> None:
+    def _load_cors_headers(
+        app: Flask, cors_allowed_hosts: t.Optional[list] = None
+    ) -> None:
         if cors_allowed_hosts:
             print(
                 f"\n\r{Colr.WARNING}{Colr.BOLD}vite-transporter is disabling CORS restrictions for:"
                 f"{Colr.END}{Colr.END}\n\r"
                 f"{Colr.OKCYAN}{', '.join(cors_allowed_hosts)}{Colr.END}\n\r"
             )
 
             @app.after_request
             def after_request(response):
-                response.headers["Access-Control-Allow-Origin"] = ", ".join(cors_allowed_hosts)
+                response.headers["Access-Control-Allow-Origin"] = ", ".join(
+                    cors_allowed_hosts
+                )
                 response.headers["Access-Control-Allow-Headers"] = ", ".join(
                     http_headers
                 )
                 response.headers["Access-Control-Allow-Methods"] = "*"
                 response.headers["Access-Control-Allow-Credentials"] = "true"
                 return response
```

### Comparing `vite_transporter-0.4.2/vite_transporter/platform/quart.py` & `vite_transporter-0.5.0/vite_transporter/platform/quart.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import sys
 import typing as t
 from pathlib import Path
 
-from vite_transporter.helpers import Colr
+from vite_transporter.utilities import Colr
 
 if "quart" in sys.modules:
     from markupsafe import Markup
     from quart import Quart, url_for, send_from_directory
 else:
     raise ImportError("Quart is not installed.")
 
-from vite_transporter._html_tags import BodyContent, ScriptTag, LinkTag
-from vite_transporter._headers import http_headers
+from vite_transporter.utilities import BodyContent, ScriptTag, LinkTag
+from vite_transporter.utilities import http_headers
 
 
 class ViteTransporter:
     app: t.Optional[Quart]
     vt_root_path: Path
 
     cors_allowed_hosts: list = None
 
     def __init__(
-            self, app: t.Optional[Quart] = None, cors_allowed_hosts: t.Optional[list] = None
+        self, app: t.Optional[Quart] = None, cors_allowed_hosts: t.Optional[list] = None
     ) -> None:
         if app is not None:
             self.init_app(app, cors_allowed_hosts)
 
     def init_app(self, app: Quart, cors_allowed_hosts: t.Optional[list] = None) -> None:
         if app is None:
             raise ImportError("No app was passed in.")
@@ -98,32 +98,36 @@
                 return Markup("".join([tag.raw() for tag in tags]))
 
             return dict(vt_head=vt_head)
 
         @app.context_processor
         async def vt_body_processor():
             def vt_body(
-                    root_id: str = "root",
-                    noscript_message: str = "You need to enable JavaScript to run this app.",
+                root_id: str = "root",
+                noscript_message: str = "You need to enable JavaScript to run this app.",
             ) -> t.Any:
                 return BodyContent(root_id, noscript_message)()
 
             return dict(vt_body=vt_body)
 
     @staticmethod
-    def _load_cors_headers(app: Quart, cors_allowed_hosts: t.Optional[list] = None) -> None:
+    def _load_cors_headers(
+        app: Quart, cors_allowed_hosts: t.Optional[list] = None
+    ) -> None:
         if cors_allowed_hosts:
             print(
                 f"\n\r{Colr.WARNING}{Colr.BOLD}vite-transporter is disabling CORS restrictions for:"
                 f"{Colr.END}{Colr.END}\n\r"
                 f"{Colr.OKCYAN}{', '.join(cors_allowed_hosts)}{Colr.END}\n\r"
             )
 
             @app.after_request
             async def after_request(response):
-                response.headers["Access-Control-Allow-Origin"] = ", ".join(cors_allowed_hosts)
+                response.headers["Access-Control-Allow-Origin"] = ", ".join(
+                    cors_allowed_hosts
+                )
                 response.headers["Access-Control-Allow-Headers"] = ", ".join(
                     http_headers
                 )
                 response.headers["Access-Control-Allow-Methods"] = "*"
                 response.headers["Access-Control-Allow-Credentials"] = "true"
                 return response
```

### Comparing `vite_transporter-0.4.2/PKG-INFO` & `vite_transporter-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vite-transporter
-Version: 0.4.2
+Version: 0.5.0
 Summary: Transport Vite apps.
 Author-email: David Carmichael <david@uilix.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

