# Comparing `tmp/markline-0.3.2.tar.gz` & `tmp/markline-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markline-0.3.2.tar", max compression
+gzip compressed data, was "markline-0.3.3.tar", max compression
```

## Comparing `markline-0.3.2.tar` & `markline-0.3.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1069 2023-08-05 08:51:19.846218 markline-0.3.2/LICENSE.md
--rw-r--r--   0        0        0     1458 2023-08-05 08:51:19.846218 markline-0.3.2/README.md
--rw-r--r--   0        0        0    28165 2023-08-05 08:51:19.850218 markline-0.3.2/markline/__init__.py
--rw-r--r--   0        0        0      604 2023-08-05 08:51:19.850218 markline-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2166 1970-01-01 00:00:00.000000 markline-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-24 07:27:12.066054 markline-0.3.3/LICENSE.md
+-rw-r--r--   0        0        0     1458 2024-04-24 07:27:12.066054 markline-0.3.3/README.md
+-rw-r--r--   0        0        0    28142 2024-04-24 07:27:12.066054 markline-0.3.3/markline/__init__.py
+-rw-r--r--   0        0        0      604 2024-04-24 07:27:12.066054 markline-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2217 1970-01-01 00:00:00.000000 markline-0.3.3/PKG-INFO
```

### Comparing `markline-0.3.2/LICENSE.md` & `markline-0.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `markline-0.3.2/README.md` & `markline-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `markline-0.3.2/markline/__init__.py` & `markline-0.3.3/markline/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -516,15 +516,15 @@
         For more information on Logseq block properties refer to the Logseq documentation.
         https://docs.logseq.com/#/page/term%2Fproperties
 
         Returns:
             properties (dict): Default properties to store.
         """
         return {
-            "headline": coalesce(self.meta.get("og:title"), self.original.title.string),
+            "title": self.meta.get("og:title"),
             "description": self.meta.get("og:description"),
             "publisher": self.meta.get("og:site_name"),
             "url": self.url,
         }
 
     def add_properties(self, properties: dict) -> None:
         """Add properties to the properties store.
@@ -722,15 +722,15 @@
         else:
             elems = [e.name for e in self.draft.find_all()]
             return dict(Counter(elems).most_common())
 
     def render(
         self,
         input_format: str = "html-native_divs-native_spans",
-        output_format: str = "gfm",
+        output_format: str = "gfm-raw_html",
         output_options: List[str] = ["--wrap=none"],
     ) -> str:
         """Render the draft HTML content to a Pandoc formatted output.
 
         The BeautifulSoup object is converted to an HTML string
         and passed to Pandoc.
 
@@ -738,15 +738,15 @@
         the Pandoc README: https://github.com/jgm/pandoc#pandoc
 
         Args:
             input_format (str, optional): A Pandoc supported format.
                 Defaults to "html-native_divs-native_spans". This is recommended to
                 preserve only the necessary HTML tags and attributes.
             output_format (str, optional): A Pandoc supported format.
-                Defaults to "gfm" or Github Flavored Markdown (GFM).
+                Defaults to "gfm-raw_html" or Github Flavored Markdown (GFM).
             output_options (List[str], optional): A list of Pandoc write options.
                 Defaults to ["--wrap=none"]. See available options:
                 https://pandoc.org/MANUAL.html#options
 
         Returns:
             str: Pandoc formatted output.
         """
```

### Comparing `markline-0.3.2/pyproject.toml` & `markline-0.3.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "markline"
-version = "0.3.2"
+version = "0.3.3"
 description = "Convert Markup to Markdown with a transformation pipeline."
 authors = ["Hugh Cameron <hescameron+githubprojects@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/hughcameron/markline"
 repository = "https://github.com/hughcameron/markline"
 readme = "README.md"
```

### Comparing `markline-0.3.2/PKG-INFO` & `markline-0.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: markline
-Version: 0.3.2
+Version: 0.3.3
 Summary: Convert Markup to Markdown with a transformation pipeline.
 Home-page: https://github.com/hughcameron/markline
 License: MIT
 Author: Hugh Cameron
 Author-email: hescameron+githubprojects@gmail.com
 Requires-Python: >=3.10.6,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: furl (>=2.1.3,<3.0.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: pypandoc (>=1.11,<2.0)
 Project-URL: Repository, https://github.com/hughcameron/markline
 Description-Content-Type: text/markdown
```

