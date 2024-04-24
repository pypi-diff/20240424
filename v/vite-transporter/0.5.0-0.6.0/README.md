# Comparing `tmp/vite_transporter-0.5.0.tar.gz` & `tmp/vite_transporter-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vite_transporter-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vite_transporter-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vite_transporter-0.5.0.tar` & `vite_transporter-0.6.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     5201 2024-04-17 20:37:21.973545 vite_transporter-0.5.0/.gitignore
--rw-r--r--   0        0        0     1083 2024-03-29 08:24:35.046180 vite_transporter-0.5.0/LICENSE
--rw-r--r--   0        0        0     4078 2024-04-23 17:38:10.489230 vite_transporter-0.5.0/README.md
--rw-r--r--   0        0        0      738 2024-04-21 15:32:14.759993 vite_transporter-0.5.0/app_flask_demo/__init__.py
--rw-r--r--   0        0        0      192 2024-04-17 19:56:25.368755 vite_transporter-0.5.0/app_flask_demo/templates/index.html
--rw-r--r--   0        0        0    39139 2024-04-23 17:26:19.313411 vite_transporter-0.5.0/app_flask_demo/vt/app_vite_demo/ili-85e34484.gif
--rw-r--r--   0        0        0    21365 2024-04-23 17:26:19.313250 vite_transporter-0.5.0/app_flask_demo/vt/app_vite_demo/index-45b871c7.js
--rw-r--r--   0        0        0    33644 2024-04-23 17:26:19.312967 vite_transporter-0.5.0/app_flask_demo/vt/app_vite_demo/index-cc24c663.css
--rw-r--r--   0        0        0      750 2024-04-21 15:32:40.857714 vite_transporter-0.5.0/app_quart_demo/__init__.py
--rw-r--r--   0        0        0      192 2024-04-17 19:56:29.985721 vite_transporter-0.5.0/app_quart_demo/templates/index.html
--rw-r--r--   0        0        0    39139 2024-04-17 19:55:40.663413 vite_transporter-0.5.0/app_quart_demo/vt/app_vite_demo/ili-85e34484.gif
--rw-r--r--   0        0        0    33329 2024-04-17 19:55:40.663791 vite_transporter-0.5.0/app_quart_demo/vt/app_vite_demo/index-621914e8.css
--rw-r--r--   0        0        0    20285 2024-04-17 19:55:40.663651 vite_transporter-0.5.0/app_quart_demo/vt/app_vite_demo/index-6e585489.js
--rw-r--r--   0        0        0     2250 2024-04-21 15:33:39.440720 vite_transporter-0.5.0/app_vite_demo/Index.jsx
--rw-r--r--   0        0        0      536 2024-04-12 20:35:46.642592 vite_transporter-0.5.0/app_vite_demo/__router__.jsx
--rw-r--r--   0        0        0    39139 2024-03-12 16:01:48.215679 vite_transporter-0.5.0/app_vite_demo/assets/ili.gif
--rw-r--r--   0        0        0      596 2024-04-21 15:30:17.354196 vite_transporter-0.5.0/app_vite_demo/index.css
--rw-r--r--   0        0        0      414 2024-04-17 19:46:30.300521 vite_transporter-0.5.0/app_vite_demo/index.html
--rw-r--r--   0        0        0   105659 2024-04-23 17:26:15.620700 vite_transporter-0.5.0/app_vite_demo/package-lock.json
--rw-r--r--   0        0        0      570 2024-04-12 14:55:15.273422 vite_transporter-0.5.0/app_vite_demo/package.json
--rw-r--r--   0        0        0       80 2024-02-23 14:52:24.766425 vite_transporter-0.5.0/app_vite_demo/postcss.config.js
--rw-r--r--   0        0        0      151 2024-03-31 09:45:49.055622 vite_transporter-0.5.0/app_vite_demo/tailwind.config.js
--rw-r--r--   0        0        0      440 2024-04-01 09:05:29.649936 vite_transporter-0.5.0/app_vite_demo/vite.config.js
--rw-r--r--   0        0        0     1262 2024-04-24 06:07:20.779037 vite_transporter-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       31 2024-04-17 20:14:50.246973 vite_transporter-0.5.0/requirements/demos.txt
--rw-r--r--   0        0        0       22 2024-04-17 20:14:46.286993 vite_transporter-0.5.0/requirements/development.txt
--rw-r--r--   0        0        0       34 2024-04-17 16:11:12.368549 vite_transporter-0.5.0/requirements/main.txt
--rw-r--r--   0        0        0     2079 2024-04-24 06:07:31.419104 vite_transporter-0.5.0/vite_transporter/__init__.py
--rw-r--r--   0        0        0      178 2024-04-23 08:21:21.096283 vite_transporter-0.5.0/vite_transporter/platform/__init__.py
--rw-r--r--   0        0        0     4721 2024-04-24 06:06:36.654452 vite_transporter-0.5.0/vite_transporter/platform/flask.py
--rw-r--r--   0        0        0     4785 2024-04-24 06:06:49.254712 vite_transporter-0.5.0/vite_transporter/platform/quart.py
--rw-r--r--   0        0        0    10208 2024-04-24 06:06:49.255249 vite_transporter-0.5.0/vite_transporter/utilities.py
--rw-r--r--   0        0        0     4760 1970-01-01 00:00:00.000000 vite_transporter-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     5201 2024-04-17 20:37:21.973545 vite_transporter-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1083 2024-03-29 08:24:35.046180 vite_transporter-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4078 2024-04-23 17:38:10.489230 vite_transporter-0.6.0/README.md
+-rw-r--r--   0        0        0      738 2024-04-21 15:32:14.759993 vite_transporter-0.6.0/app_flask_demo/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-17 19:56:25.368755 vite_transporter-0.6.0/app_flask_demo/templates/index.html
+-rw-r--r--   0        0        0    39139 2024-04-23 17:26:19.313411 vite_transporter-0.6.0/app_flask_demo/vt/app_vite_demo/ili-85e34484.gif
+-rw-r--r--   0        0        0    21365 2024-04-23 17:26:19.313250 vite_transporter-0.6.0/app_flask_demo/vt/app_vite_demo/index-45b871c7.js
+-rw-r--r--   0        0        0    33644 2024-04-23 17:26:19.312967 vite_transporter-0.6.0/app_flask_demo/vt/app_vite_demo/index-cc24c663.css
+-rw-r--r--   0        0        0      750 2024-04-21 15:32:40.857714 vite_transporter-0.6.0/app_quart_demo/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-17 19:56:29.985721 vite_transporter-0.6.0/app_quart_demo/templates/index.html
+-rw-r--r--   0        0        0    39139 2024-04-17 19:55:40.663413 vite_transporter-0.6.0/app_quart_demo/vt/app_vite_demo/ili-85e34484.gif
+-rw-r--r--   0        0        0    33329 2024-04-17 19:55:40.663791 vite_transporter-0.6.0/app_quart_demo/vt/app_vite_demo/index-621914e8.css
+-rw-r--r--   0        0        0    20285 2024-04-17 19:55:40.663651 vite_transporter-0.6.0/app_quart_demo/vt/app_vite_demo/index-6e585489.js
+-rw-r--r--   0        0        0     2250 2024-04-21 15:33:39.440720 vite_transporter-0.6.0/app_vite_demo/Index.jsx
+-rw-r--r--   0        0        0      536 2024-04-12 20:35:46.642592 vite_transporter-0.6.0/app_vite_demo/__router__.jsx
+-rw-r--r--   0        0        0    39139 2024-03-12 16:01:48.215679 vite_transporter-0.6.0/app_vite_demo/assets/ili.gif
+-rw-r--r--   0        0        0      596 2024-04-21 15:30:17.354196 vite_transporter-0.6.0/app_vite_demo/index.css
+-rw-r--r--   0        0        0      414 2024-04-17 19:46:30.300521 vite_transporter-0.6.0/app_vite_demo/index.html
+-rw-r--r--   0        0        0   105659 2024-04-23 17:26:15.620700 vite_transporter-0.6.0/app_vite_demo/package-lock.json
+-rw-r--r--   0        0        0      570 2024-04-12 14:55:15.273422 vite_transporter-0.6.0/app_vite_demo/package.json
+-rw-r--r--   0        0        0       80 2024-02-23 14:52:24.766425 vite_transporter-0.6.0/app_vite_demo/postcss.config.js
+-rw-r--r--   0        0        0      151 2024-03-31 09:45:49.055622 vite_transporter-0.6.0/app_vite_demo/tailwind.config.js
+-rw-r--r--   0        0        0      440 2024-04-01 09:05:29.649936 vite_transporter-0.6.0/app_vite_demo/vite.config.js
+-rw-r--r--   0        0        0     1262 2024-04-24 06:07:20.779037 vite_transporter-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       31 2024-04-17 20:14:50.246973 vite_transporter-0.6.0/requirements/demos.txt
+-rw-r--r--   0        0        0       22 2024-04-17 20:14:46.286993 vite_transporter-0.6.0/requirements/development.txt
+-rw-r--r--   0        0        0       34 2024-04-17 16:11:12.368549 vite_transporter-0.6.0/requirements/main.txt
+-rw-r--r--   0        0        0     2318 2024-04-24 06:25:18.906846 vite_transporter-0.6.0/vite_transporter/__init__.py
+-rw-r--r--   0        0        0      178 2024-04-23 08:21:21.096283 vite_transporter-0.6.0/vite_transporter/platform/__init__.py
+-rw-r--r--   0        0        0     4721 2024-04-24 06:06:36.654452 vite_transporter-0.6.0/vite_transporter/platform/flask.py
+-rw-r--r--   0        0        0     4785 2024-04-24 06:06:49.254712 vite_transporter-0.6.0/vite_transporter/platform/quart.py
+-rw-r--r--   0        0        0    10269 2024-04-24 06:25:00.144950 vite_transporter-0.6.0/vite_transporter/utilities.py
+-rw-r--r--   0        0        0     4760 1970-01-01 00:00:00.000000 vite_transporter-0.6.0/PKG-INFO
```

### Comparing `vite_transporter-0.5.0/.gitignore` & `vite_transporter-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.5.0/LICENSE` & `vite_transporter-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.5.0/README.md` & `vite_transporter-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.5.0/app_flask_demo/__init__.py` & `vite_transporter-0.6.0/app_flask_demo/__init__.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.5.0/app_flask_demo/vt/app_vite_demo/ili-85e34484.gif` & `vite_transporter-0.6.0/app_flask_demo/vt/app_vite_demo/ili-85e34484.gif`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.5.0/app_flask_demo/vt/app_vite_demo/index-45b871c7.js` & `vite_transporter-0.6.0/app_flask_demo/vt/app_vite_demo/index-45b871c7.js`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.5.0/app_flask_demo/vt/app_vite_demo/index-cc24c663.css` & `vite_transporter-0.6.0/app_flask_demo/vt/app_vite_demo/index-cc24c663.css`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.5.0/app_quart_demo/__init__.py` & `vite_transporter-0.6.0/app_quart_demo/__init__.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.5.0/app_quart_demo/vt/app_vite_demo/ili-85e34484.gif` & `vite_transporter-0.6.0/app_quart_demo/vt/app_vite_demo/ili-85e34484.gif`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.5.0/app_quart_demo/vt/app_vite_demo/index-621914e8.css` & `vite_transporter-0.6.0/app_quart_demo/vt/app_vite_demo/index-621914e8.css`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.5.0/app_quart_demo/vt/app_vite_demo/index-6e585489.js` & `vite_transporter-0.6.0/app_quart_demo/vt/app_vite_demo/index-6e585489.js`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.5.0/app_vite_demo/Index.jsx` & `vite_transporter-0.6.0/app_vite_demo/Index.jsx`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.5.0/app_vite_demo/__router__.jsx` & `vite_transporter-0.6.0/app_vite_demo/__router__.jsx`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.5.0/app_vite_demo/assets/ili.gif` & `vite_transporter-0.6.0/app_vite_demo/assets/ili.gif`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.5.0/app_vite_demo/index.css` & `vite_transporter-0.6.0/app_vite_demo/index.css`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.5.0/app_vite_demo/package-lock.json` & `vite_transporter-0.6.0/app_vite_demo/package-lock.json`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.5.0/app_vite_demo/package.json` & `vite_transporter-0.6.0/app_vite_demo/package.json`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.5.0/pyproject.toml` & `vite_transporter-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.5.0/vite_transporter/__init__.py` & `vite_transporter-0.6.0/vite_transporter/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,78 +1,80 @@
 import sys
 
 from .utilities import ArgumentParser as _ArgumentParser
 from .utilities import Colr as _Colr
 from .utilities import PyProjectConfig as _PyProjectConfig
 from .utilities import compiler
 
-__version__ = "0.5.0"
+__version__ = "0.6.0"
 
 
-def setup_subparsers(pars):
-    subparsers = pars.add_subparsers()
+def setup_subparsers(parser):
+    subparsers = parser.add_subparsers()
 
-    subparsers.add_parser("compile").set_defaults(compile=False).add_argument(
-        "-y", action="store_true"
-    )
-    subparsers.add_parser("list").set_defaults(list=False)
-    subparsers.add_parser("ls").set_defaults(list=False)
+    _compile = subparsers.add_parser("compile")
+    _compile.set_defaults(compile=False)
+    _compile.add_argument("-y", action="store_true")
+
+    _list = subparsers.add_parser("list")
+    _list.set_defaults(list=False)
+    _ls = subparsers.add_parser("ls")
+    _ls.set_defaults(ls=False)
 
 
-def load_vite_apps(pyproject):
-    for vite_app in pyproject.vite_apps:
-        pyproject.vite_apps.append(
+def load_vite_apps(pyproject_config):
+    vite_apps = []
+    for vite_app in pyproject_config.vite_apps:
+        vite_apps.append(
             {
                 "vite_app": vite_app,
-                "serve_app": pyproject.vt_config.get("serve_app"),
+                "serve_app": pyproject_config.vt_config.get("serve_app"),
             }
         )
+    return vite_apps
 
 
-def list_ls(pars):
+def list_ls(vite_apps_found):
     print("")
-    if not pars.vite_apps:
+    if not vite_apps_found:
         print(f" {_Colr.WARNING}No vite apps found in pyproject.toml{_Colr.END}")
     else:
-        for app in pars.vite_apps:
+        for app in vite_apps_found:
             print(
                 f"{_Colr.OKGREEN}{app.get('vite_app')}/dist/assets{_Colr.END} "
                 f"{_Colr.BOLD}=>{_Colr.END} "
                 f"{_Colr.OKGREEN}{app.get('serve_app')}/vt/{app.get('vite_app')}/{_Colr.END}"
             )
     print("")
     sys.exit(0)
 
 
-def compile_(pyproject, pars, args):
+def compile_(pyproject_config, vite_apps_found, parsed_args):
     compiler(
-        pyproject,
-        pars.vite_apps,
-        replace=True if hasattr(args, "y") and args.y else False,
+        pyproject_config,
+        vite_apps_found,
+        replace=True if hasattr(parsed_args, "y") and parsed_args.y else False,
     )
     sys.exit(0)
 
 
 def cli_entry():
-    pars = _ArgumentParser(prog="vtf", add_help=False)
-    pars.add_argument(
+    parser = _ArgumentParser(prog="vtf", add_help=False)
+    parser.add_argument(
         "--version", "-v", action="version", version=f"vite-to-flask {__version__}"
     )
-    pars.add_argument("--help", "-h", action="help")
-
-    setup_subparsers(pars)
-
-    with _PyProjectConfig() as pyproject:
-        pypro: _PyProjectConfig = pyproject
+    parser.add_argument("--help", "-h", action="help")
 
-        load_vite_apps(pypro)
+    setup_subparsers(parser)
 
-        args = pars.parse_args()
+    with _PyProjectConfig() as pyproject_config:
+        vite_apps_found = load_vite_apps(pyproject_config)
+        parsed_args = parser.parse_args()
 
-        if hasattr(args, "compile"):
-            compile_(pypro, pars, args)
+        if hasattr(parsed_args, "compile"):
+            compile_(pyproject_config, vite_apps_found, parsed_args)
 
-        if hasattr(args, "list") or hasattr(args, "ls"):
-            list_ls(pars)
+        if hasattr(parsed_args, "list") or hasattr(parsed_args, "ls"):
+            list_ls(vite_apps_found)
 
     # print help if no command is given
-    pars.print_help()
+    parser.print_help()
```

### Comparing `vite_transporter-0.5.0/vite_transporter/platform/flask.py` & `vite_transporter-0.6.0/vite_transporter/platform/flask.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.5.0/vite_transporter/platform/quart.py` & `vite_transporter-0.6.0/vite_transporter/platform/quart.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.5.0/vite_transporter/utilities.py` & `vite_transporter-0.6.0/vite_transporter/utilities.py`

 * *Files 9% similar despite different names*

```diff
@@ -107,19 +107,18 @@
     def __exit__(self, exc_type, exc_val, exc_tb):
         return None
 
     def run(self, command: str):
         subprocess.run([self.npm_binary, *shlex.split(command)], cwd=self.workdir)
 
 
-def compiler(pypro: PyProjectConfig, vite_apps: list[dict], replace: bool = False):
-    pc: PyProjectConfig = pypro
+def compiler(pyproject_config: PyProjectConfig, vite_apps_found: list[dict], replace: bool = False):
 
     print("Compiling Vite apps...")
-    vt_dir = pc.cwd / pc.serve_app / "vt"
+    vt_dir = pyproject_config.cwd / pyproject_config.serve_app / "vt"
 
     # Delete contents of vt_dir
     if vt_dir.exists():
         if not replace:
             prompt = input(
                 f"Continuing will replace the contents of \n\r"
                 f"{vt_dir} \n\r"
@@ -139,30 +138,30 @@
             print("Operation aborted.")
             sys.exit(0)
 
     else:
         vt_dir.mkdir()
 
     # Create directories for vite apps
-    for app in vite_apps:
-        va_path = pc.cwd / app.get("vite_app")
+    for app in vite_apps_found:
+        va_path = pyproject_config.cwd / app.get("vite_app")
         va_node_modules = va_path / "node_modules"
         va_dist = va_path / "dist"
         va_assets = va_dist / "assets"
 
         va_vt_path = vt_dir / app.get("vite_app")
 
         if not va_vt_path.exists():
             va_vt_path.mkdir()
 
         if not va_node_modules.exists():
-            with NPMCommander(va_path, pc.npm_exec) as npm:
+            with NPMCommander(va_path, pyproject_config.npm_exec) as npm:
                 npm.run("install")
 
-        with NPXCommander(va_path, pc.npx_exec) as npx:
+        with NPXCommander(va_path, pyproject_config.npx_exec) as npx:
             npx.run("vite build --mode production")
 
         for item in va_assets.iterdir():
             print(f"{Colr.OKGREEN}Copying {item.name} to {va_vt_path}{Colr.END}")
 
             if item.suffix == ".js":
                 with open(va_vt_path / item.name, "w") as f:
```

### Comparing `vite_transporter-0.5.0/PKG-INFO` & `vite_transporter-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vite-transporter
-Version: 0.5.0
+Version: 0.6.0
 Summary: Transport Vite apps.
 Author-email: David Carmichael <david@uilix.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

