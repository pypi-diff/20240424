# Comparing `tmp/apibook-0.1.0.tar.gz` & `tmp/apibook-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apibook-0.1.0.tar", last modified: Fri Apr 12 08:58:07 2024, max compression
+gzip compressed data, was "apibook-0.1.1.tar", last modified: Wed Apr 24 09:10:44 2024, max compression
```

## Comparing `apibook-0.1.0.tar` & `apibook-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2024-04-12 08:58:07.220234 apibook-0.1.0/LICENSE-MIT.txt
--rw-r--r--   0        0        0     1268 2024-04-12 08:58:07.220234 apibook-0.1.0/README.md
--rw-r--r--   0        0        0      612 2024-04-12 08:58:07.220234 apibook-0.1.0/apibook/__init__.py
--rw-r--r--   0        0        0     9555 2024-04-12 08:58:07.220234 apibook-0.1.0/apibook/_ast.py
--rw-r--r--   0        0        0     2601 2024-04-12 08:58:07.220234 apibook-0.1.0/apibook/cli.py
--rw-r--r--   0        0        0     9886 2024-04-12 08:58:07.220234 apibook-0.1.0/apibook/data.py
--rw-r--r--   0        0        0     5134 2024-04-12 08:58:07.220234 apibook-0.1.0/apibook/main.py
--rw-r--r--   0        0        0     1166 2024-04-12 08:58:07.320234 apibook-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3168 1970-01-01 00:00:00.000000 apibook-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-24 09:10:44.808088 apibook-0.1.1/LICENSE-MIT.txt
+-rw-r--r--   0        0        0     1268 2024-04-24 09:10:44.808088 apibook-0.1.1/README.md
+-rw-r--r--   0        0        0      612 2024-04-24 09:10:44.808088 apibook-0.1.1/apibook/__init__.py
+-rw-r--r--   0        0        0     9555 2024-04-24 09:10:44.808088 apibook-0.1.1/apibook/_ast.py
+-rw-r--r--   0        0        0     2601 2024-04-24 09:10:44.808088 apibook-0.1.1/apibook/cli.py
+-rw-r--r--   0        0        0    10192 2024-04-24 09:10:44.808088 apibook-0.1.1/apibook/data.py
+-rw-r--r--   0        0        0     5239 2024-04-24 09:10:44.808088 apibook-0.1.1/apibook/main.py
+-rw-r--r--   0        0        0     1166 2024-04-24 09:10:44.948088 apibook-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3168 1970-01-01 00:00:00.000000 apibook-0.1.1/PKG-INFO
```

### Comparing `apibook-0.1.0/LICENSE-MIT.txt` & `apibook-0.1.1/LICENSE-MIT.txt`

 * *Files identical despite different names*

### Comparing `apibook-0.1.0/README.md` & `apibook-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `apibook-0.1.0/apibook/__init__.py` & `apibook-0.1.1/apibook/__init__.py`

 * *Files identical despite different names*

### Comparing `apibook-0.1.0/apibook/_ast.py` & `apibook-0.1.1/apibook/_ast.py`

 * *Files identical despite different names*

### Comparing `apibook-0.1.0/apibook/cli.py` & `apibook-0.1.1/apibook/cli.py`

 * *Files identical despite different names*

### Comparing `apibook-0.1.0/apibook/data.py` & `apibook-0.1.1/apibook/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -267,37 +267,46 @@
             item: the item to resolve
 
         Returns:
             the module containing the item
             the item queried
         """
 
-        for import_ in self.imports:
-            if isinstance(import_, FromImport):
-                if item in import_.names:
-                    if import_.relative == 0:
-                        return import_.module, item
-
-                    # resolve relative imports.
-                    # If we are in foo.bar.baz and we import from .qux import item
-                    # we need to resolve to foo.bar.qux.item
-                    if import_.module is None:
-                        return self.name, item
+        for import_ in self.imports + self.classes + self.variables:
+            match import_:
+                case FromImport(module, names, relative):
+                    if item in names:
+                        if relative == 0:
+                            return module, item
+
+                        # resolve relative imports.
+                        # If we are in foo.bar.baz and we import from .qux import item
+                        # we need to resolve to foo.bar.qux.item
+                        if module is None:
+                            return self.name, item
+
+                        parts = self.name.split(".")
+                        parts = parts[:-relative]
+                        parts.append(module)
+
+                        return ".".join(parts), item
 
-                    parts = self.name.split(".")
-                    parts = parts[: -import_.relative]
-                    parts.append(import_.module)
+                case NakedImport(module):
+                    if item == module:
+                        return self.name, item
 
-                    return ".".join(parts), item
+                case Variable(name):
+                    if item == name:
+                        return self.name, item
 
-            elif isinstance(import_, NakedImport):
-                if item == import_.module:
-                    return item
+                case Class(name):
+                    if item == name:
+                        return self.name, name
 
-        logger.warning(f"Could not resolve import {item} from {self.name}")
+        logger.warning(f"Could not resolve import {item} from {self}")
         return None
 
     @property
     def _visible_functions(self):
         return [m for m in self.functions if not m.name.startswith("_")]
 
     @property
```

### Comparing `apibook-0.1.0/apibook/main.py` & `apibook-0.1.1/apibook/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,28 +42,31 @@
 
 def fixup_reexports(root_module: str, docs: dict[str, Module]):
     """Inlines items that are reexported from other modules via '__all__'
     lists."""
     for mod, content in docs.items():
         logger.info("Fixing up reexports for '%s'", mod)
         for alias in content.all_exports:
-            mod, item = content.resolve_import(alias)
+            module, item = content.resolve_import(alias)
 
-            if docs.get(f"{mod}.{item}"):
+            if module == mod:
+                continue  # Don't reexport from the same module
+
+            if docs.get(f"{module}.{item}"):
                 continue
 
-            for candidate in [mod, f"{mod}.__init__"]:
+            for candidate in [module, f"{module}.__init__"]:
                 source_doc = docs.get(candidate)
 
-                logger.info(f"Checking {candidate} for {item} - {source_doc}")
+                logger.info(f"Checking {candidate} for {item}")
 
                 if source_doc:
-                    print(f"Resolving {source_doc.name}.{item}")
+                    logger.info(f"Resolving {source_doc.name}.{item}")
                     found_item = source_doc.resolve_export(item)
-                    logger.info(f"For {mod}.{item} found {found_item}")
+                    logger.debug(f"For {mod}.{item} found {found_item}")
 
                     match found_item:
                         case Class(_, _, _, _):
                             content.classes.append(found_item)
                             break
                         case Method(_, _, _, _):
                             content.functions.append(found_item)
@@ -79,15 +82,15 @@
                             break
                         case None:
                             print(f"Could not find {mod}.{item}")
 
             else:
                 known_modules = "\t" + "\n\t".join(f'"{k}"' for k in docs.keys())
                 raise ValueError(
-                    f"Could not find module {mod} or {mod}.__init__ - known modules:\n{known_modules}"
+                    f"Could not find module {module} or {module}.__init__ - known modules:\n{known_modules}"
                 )
 
 
 def run(root_dir: str, output_dir: str, summary_output_template: str | None):
     """Run the docstring generator."""
     docs = {}
     for root, _, files in os.walk(root_dir):
```

### Comparing `apibook-0.1.0/pyproject.toml` & `apibook-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "apibook"
 description = "API documentation generator for MdBook"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     { name = "Tom Solberg", email = "me@sbg.dev" },
 ]
 dependencies = [
     "docstring_parser",
     "rich",
 ]
```

### Comparing `apibook-0.1.0/PKG-INFO` & `apibook-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apibook
-Version: 0.1.0
+Version: 0.1.1
 Summary: API documentation generator for MdBook
 Keywords: mdbook apidoc documentation markdown
 Author-Email: Tom Solberg <me@sbg.dev>
 License: MIT License
         
         Copyright (c) 2022 Tom Solberg
```

