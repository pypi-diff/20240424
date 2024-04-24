# Comparing `tmp/plantuml-markdown-3.9.5.tar.gz` & `tmp/plantuml-markdown-3.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plantuml-markdown-3.9.5.tar", last modified: Mon Apr 22 18:15:29 2024, from Unix
+gzip compressed data, was "plantuml-markdown-3.9.6.tar", last modified: Wed Apr 24 06:01:26 2024, from Unix
```

## Comparing `plantuml-markdown-3.9.5.tar` & `plantuml-markdown-3.9.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 michele   (1000) michele   (1000)        0 2024-04-22 18:15:29.325034 plantuml-markdown-3.9.5/
--rw-rw-r--   0 michele   (1000) michele   (1000)     1299 2022-08-08 16:48:39.000000 plantuml-markdown-3.9.5/LICENSE
--rw-rw-r--   0 michele   (1000) michele   (1000)    17028 2024-04-22 18:15:29.325034 plantuml-markdown-3.9.5/PKG-INFO
--rw-rw-r--   0 michele   (1000) michele   (1000)    16250 2024-03-26 19:32:41.000000 plantuml-markdown-3.9.5/README.md
-drwxrwxr-x   0 michele   (1000) michele   (1000)        0 2024-04-22 18:15:29.325034 plantuml-markdown-3.9.5/plantuml_markdown/
--rw-rw-r--   0 michele   (1000) michele   (1000)      130 2024-03-26 19:32:41.000000 plantuml-markdown-3.9.5/plantuml_markdown/__init__.py
--rw-rw-r--   0 michele   (1000) michele   (1000)    31246 2024-04-22 18:14:45.000000 plantuml-markdown-3.9.5/plantuml_markdown/plantuml_markdown.py
-drwxrwxr-x   0 michele   (1000) michele   (1000)        0 2024-04-22 18:15:29.325034 plantuml-markdown-3.9.5/plantuml_markdown.egg-info/
--rw-rw-r--   0 michele   (1000) michele   (1000)    17028 2024-04-22 18:15:29.000000 plantuml-markdown-3.9.5/plantuml_markdown.egg-info/PKG-INFO
--rw-rw-r--   0 michele   (1000) michele   (1000)      423 2024-04-22 18:15:29.000000 plantuml-markdown-3.9.5/plantuml_markdown.egg-info/SOURCES.txt
--rw-rw-r--   0 michele   (1000) michele   (1000)        1 2024-04-22 18:15:29.000000 plantuml-markdown-3.9.5/plantuml_markdown.egg-info/dependency_links.txt
--rw-r--r--   0 michele   (1000) michele   (1000)       86 2024-04-22 18:15:29.000000 plantuml-markdown-3.9.5/plantuml_markdown.egg-info/entry_points.txt
--rw-rw-r--   0 michele   (1000) michele   (1000)       22 2024-04-22 18:15:29.000000 plantuml-markdown-3.9.5/plantuml_markdown.egg-info/requires.txt
--rw-rw-r--   0 michele   (1000) michele   (1000)       18 2024-04-22 18:15:29.000000 plantuml-markdown-3.9.5/plantuml_markdown.egg-info/top_level.txt
--rw-rw-r--   0 michele   (1000) michele   (1000)       38 2024-04-22 18:15:29.325034 plantuml-markdown-3.9.5/setup.cfg
--rw-rw-r--   0 michele   (1000) michele   (1000)     1486 2024-04-22 18:14:45.000000 plantuml-markdown-3.9.5/setup.py
-drwxrwxr-x   0 michele   (1000) michele   (1000)        0 2024-04-22 18:15:29.325034 plantuml-markdown-3.9.5/test/
--rw-rw-r--   0 michele   (1000) michele   (1000)    34104 2024-03-26 19:32:41.000000 plantuml-markdown-3.9.5/test/test_plantuml.py
--rw-rw-r--   0 michele   (1000) michele   (1000)     1931 2022-10-09 18:20:36.000000 plantuml-markdown-3.9.5/test/test_plantuml_fenced.py
--rw-rw-r--   0 michele   (1000) michele   (1000)      531 2022-10-16 11:00:27.000000 plantuml-markdown-3.9.5/test/test_plantuml_legacy.py
--rw-rw-r--   0 michele   (1000) michele   (1000)       22 2024-04-22 18:15:29.365034 plantuml-markdown-3.9.5/requirements.txt
+drwxrwxr-x   0 michele   (1000) michele   (1000)        0 2024-04-24 06:01:26.022096 plantuml-markdown-3.9.6/
+-rw-rw-r--   0 michele   (1000) michele   (1000)     1299 2022-08-08 16:48:39.000000 plantuml-markdown-3.9.6/LICENSE
+-rw-rw-r--   0 michele   (1000) michele   (1000)    17028 2024-04-24 06:01:26.022096 plantuml-markdown-3.9.6/PKG-INFO
+-rw-rw-r--   0 michele   (1000) michele   (1000)    16250 2024-03-26 19:32:41.000000 plantuml-markdown-3.9.6/README.md
+drwxrwxr-x   0 michele   (1000) michele   (1000)        0 2024-04-24 06:01:26.022096 plantuml-markdown-3.9.6/plantuml_markdown/
+-rw-rw-r--   0 michele   (1000) michele   (1000)      130 2024-03-26 19:32:41.000000 plantuml-markdown-3.9.6/plantuml_markdown/__init__.py
+-rw-rw-r--   0 michele   (1000) michele   (1000)    31301 2024-04-24 05:59:55.000000 plantuml-markdown-3.9.6/plantuml_markdown/plantuml_markdown.py
+drwxrwxr-x   0 michele   (1000) michele   (1000)        0 2024-04-24 06:01:26.022096 plantuml-markdown-3.9.6/plantuml_markdown.egg-info/
+-rw-rw-r--   0 michele   (1000) michele   (1000)    17028 2024-04-24 06:01:25.000000 plantuml-markdown-3.9.6/plantuml_markdown.egg-info/PKG-INFO
+-rw-rw-r--   0 michele   (1000) michele   (1000)      423 2024-04-24 06:01:25.000000 plantuml-markdown-3.9.6/plantuml_markdown.egg-info/SOURCES.txt
+-rw-rw-r--   0 michele   (1000) michele   (1000)        1 2024-04-24 06:01:25.000000 plantuml-markdown-3.9.6/plantuml_markdown.egg-info/dependency_links.txt
+-rw-r--r--   0 michele   (1000) michele   (1000)       86 2024-04-24 06:01:25.000000 plantuml-markdown-3.9.6/plantuml_markdown.egg-info/entry_points.txt
+-rw-rw-r--   0 michele   (1000) michele   (1000)       22 2024-04-24 06:01:25.000000 plantuml-markdown-3.9.6/plantuml_markdown.egg-info/requires.txt
+-rw-rw-r--   0 michele   (1000) michele   (1000)       18 2024-04-24 06:01:25.000000 plantuml-markdown-3.9.6/plantuml_markdown.egg-info/top_level.txt
+-rw-rw-r--   0 michele   (1000) michele   (1000)       38 2024-04-24 06:01:26.022096 plantuml-markdown-3.9.6/setup.cfg
+-rw-rw-r--   0 michele   (1000) michele   (1000)     1486 2024-04-24 05:59:55.000000 plantuml-markdown-3.9.6/setup.py
+drwxrwxr-x   0 michele   (1000) michele   (1000)        0 2024-04-24 06:01:26.022096 plantuml-markdown-3.9.6/test/
+-rw-rw-r--   0 michele   (1000) michele   (1000)    34839 2024-04-24 05:59:55.000000 plantuml-markdown-3.9.6/test/test_plantuml.py
+-rw-rw-r--   0 michele   (1000) michele   (1000)     1931 2022-10-09 18:20:36.000000 plantuml-markdown-3.9.6/test/test_plantuml_fenced.py
+-rw-rw-r--   0 michele   (1000) michele   (1000)      531 2022-10-16 11:00:27.000000 plantuml-markdown-3.9.6/test/test_plantuml_legacy.py
+-rw-rw-r--   0 michele   (1000) michele   (1000)       22 2024-04-24 06:01:26.062094 plantuml-markdown-3.9.6/requirements.txt
```

### Comparing `plantuml-markdown-3.9.5/LICENSE` & `plantuml-markdown-3.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `plantuml-markdown-3.9.5/PKG-INFO` & `plantuml-markdown-3.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plantuml-markdown
-Version: 3.9.5
+Version: 3.9.6
 Summary: A PlantUML plugin for Markdown
 Home-page: https://github.com/mikitex70/plantuml-markdown
 Author: Michele Tessaro
 Author-email: michele.tessaro.tex@gmail.com
 Keywords: Markdown,typesetting,include,plugin,extension
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `plantuml-markdown-3.9.5/README.md` & `plantuml-markdown-3.9.6/README.md`

 * *Files identical despite different names*

### Comparing `plantuml-markdown-3.9.5/plantuml_markdown/plantuml_markdown.py` & `plantuml-markdown-3.9.6/plantuml_markdown/plantuml_markdown.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,14 +334,15 @@
         return f'<div style="color: red">{msg}</div>'
 
     def _render_diagram(self, code: str, requested_format: str) -> Tuple[Optional[bytes], Optional[str]]:
         cached_diagram_file = None
         diagram = None
 
         if self._cachedir:
+            os.makedirs(self._cachedir, exist_ok=True)
             diagram_hash = "%08x" % (adler32(code.encode('UTF-8')) & 0xffffffff)
             cached_diagram_file = os.path.expanduser(
                     os.path.join(self._cachedir, diagram_hash + '.' + requested_format))
 
             if os.path.isfile(cached_diagram_file):
                 with open(cached_diagram_file, 'rb') as f:
                     diagram = f.read()
```

### Comparing `plantuml-markdown-3.9.5/plantuml_markdown.egg-info/PKG-INFO` & `plantuml-markdown-3.9.6/plantuml_markdown.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plantuml-markdown
-Version: 3.9.5
+Version: 3.9.6
 Summary: A PlantUML plugin for Markdown
 Home-page: https://github.com/mikitex70/plantuml-markdown
 Author: Michele Tessaro
 Author-email: michele.tessaro.tex@gmail.com
 Keywords: Markdown,typesetting,include,plugin,extension
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `plantuml-markdown-3.9.5/setup.py` & `plantuml-markdown-3.9.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     install_requirements = f.read().splitlines()
 
 with open(path.join(here, 'test-requirements.txt')) as f:
     test_requirements = f.read().splitlines()
 
 setuptools.setup(
     name="plantuml-markdown",
-    version="3.9.5",
+    version="3.9.6",
     author="Michele Tessaro",
     author_email="michele.tessaro.tex@gmail.com",
     description="A PlantUML plugin for Markdown",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=['Markdown', 'typesetting', 'include', 'plugin', 'extension'],
     url="https://github.com/mikitex70/plantuml-markdown",
```

### Comparing `plantuml-markdown-3.9.5/test/test_plantuml.py` & `plantuml-markdown-3.9.6/test/test_plantuml.py`

 * *Files 1% similar despite different names*

```diff
@@ -791,7 +791,24 @@
                                             'plantuml_markdown': {
                                                 'server': plantumlserver_mock.url,
                                             }
                                         })
             text = self.text_builder.diagram('A -> B').format('txt').build()
             self.assertEqual('<pre><code class="text">dummy</code></pre>',
                              self.md.convert(text))
+
+    def test_cachedir(self):
+        """
+        Verify that `cachedir` is created if it does not exist
+        """
+        temp_dir = tempfile.TemporaryDirectory()
+        cache_dir = os.path.join(temp_dir.name, 'cache', 'dir')
+        self.md = markdown.Markdown(extensions=['plantuml_markdown'],
+                                    extension_configs={
+                                        'plantuml_markdown': {
+                                            'cachedir': cache_dir,
+                                        }
+                                    })
+        text = self.text_builder.diagram("A --> B").build()
+        self.md.convert(text)
+        self.assertTrue(os.path.exists(cache_dir))
+        temp_dir.cleanup()
```

### Comparing `plantuml-markdown-3.9.5/test/test_plantuml_fenced.py` & `plantuml-markdown-3.9.6/test/test_plantuml_fenced.py`

 * *Files identical despite different names*

### Comparing `plantuml-markdown-3.9.5/test/test_plantuml_legacy.py` & `plantuml-markdown-3.9.6/test/test_plantuml_legacy.py`

 * *Files identical despite different names*

