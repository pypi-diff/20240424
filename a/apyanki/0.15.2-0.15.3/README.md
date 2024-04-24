# Comparing `tmp/apyanki-0.15.2.tar.gz` & `tmp/apyanki-0.15.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apyanki-0.15.2.tar", max compression
+gzip compressed data, was "apyanki-0.15.3.tar", max compression
```

## Comparing `apyanki-0.15.2.tar` & `apyanki-0.15.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1075 2022-04-08 08:17:45.340180 apyanki-0.15.2/LICENSE.md
--rw-r--r--   0        0        0    11048 2024-04-11 20:43:59.140388 apyanki-0.15.2/README.md
--rw-r--r--   0        0        0     1561 2024-04-12 13:05:21.485214 apyanki-0.15.2/pyproject.toml
--rw-r--r--   0        0        0      362 2024-04-11 20:43:59.140388 apyanki-0.15.2/src/apyanki/__init__.py
--rw-r--r--   0        0        0    16898 2024-04-11 20:43:59.140388 apyanki-0.15.2/src/apyanki/anki.py
--rw-r--r--   0        0        0     1964 2024-04-11 20:43:59.140388 apyanki-0.15.2/src/apyanki/cards.py
--rw-r--r--   0        0        0    14640 2024-04-11 20:43:59.140388 apyanki-0.15.2/src/apyanki/cli.py
--rw-r--r--   0        0        0     2021 2024-04-11 20:43:59.140388 apyanki-0.15.2/src/apyanki/config.py
--rw-r--r--   0        0        0     1259 2024-04-11 20:43:59.140388 apyanki-0.15.2/src/apyanki/console.py
--rw-r--r--   0        0        0     9117 2024-04-11 20:43:59.143721 apyanki-0.15.2/src/apyanki/fields.py
--rw-r--r--   0        0        0    23307 2024-04-11 20:43:59.143721 apyanki-0.15.2/src/apyanki/note.py
--rw-r--r--   0        0        0     2987 2024-04-11 20:43:59.143721 apyanki-0.15.2/src/apyanki/utilities.py
--rw-r--r--   0        0        0    12110 1970-01-01 00:00:00.000000 apyanki-0.15.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-03 19:56:02.857177 apyanki-0.15.3/LICENSE.md
+-rw-r--r--   0        0        0    11250 2024-04-19 20:43:04.288990 apyanki-0.15.3/README.md
+-rw-r--r--   0        0        0     1561 2024-04-24 20:54:26.964655 apyanki-0.15.3/pyproject.toml
+-rw-r--r--   0        0        0      362 2024-04-11 17:02:39.255040 apyanki-0.15.3/src/apyanki/__init__.py
+-rw-r--r--   0        0        0    16917 2024-04-19 20:21:19.756773 apyanki-0.15.3/src/apyanki/anki.py
+-rw-r--r--   0        0        0     1964 2024-04-11 17:02:57.515160 apyanki-0.15.3/src/apyanki/cards.py
+-rw-r--r--   0        0        0    14640 2024-04-11 17:03:04.491873 apyanki-0.15.3/src/apyanki/cli.py
+-rw-r--r--   0        0        0     2064 2024-04-19 20:39:20.334116 apyanki-0.15.3/src/apyanki/config.py
+-rw-r--r--   0        0        0     1259 2024-03-22 19:17:12.627164 apyanki-0.15.3/src/apyanki/console.py
+-rw-r--r--   0        0        0     9169 2024-04-19 20:40:01.254397 apyanki-0.15.3/src/apyanki/fields.py
+-rw-r--r--   0        0        0    23307 2024-04-11 17:08:37.727403 apyanki-0.15.3/src/apyanki/note.py
+-rw-r--r--   0        0        0     2987 2024-04-11 17:11:39.668604 apyanki-0.15.3/src/apyanki/utilities.py
+-rw-r--r--   0        0        0    12312 1970-01-01 00:00:00.000000 apyanki-0.15.3/PKG-INFO
```

### Comparing `apyanki-0.15.2/LICENSE.md` & `apyanki-0.15.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.2/README.md` & `apyanki-0.15.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,17 @@
   '300']` which specifies the command and its options to use for the
   corresponding key (file extension).
 - `img_viewers_default`: Specify the default command to show an image. Must be
   provided as a list of the command and desired options, such as `['feh',
   '-d']`.
 - `markdown_models`: Specify a list of models for which `apy` will use
   a markdown converter.
+- `markdown_pygments_style`: Specify the code highlight scheme to use for
+  fenced code blocks in Markdown notes. See the [Pygments
+  documentation](https://pygments.org/docs/styles/) for more details.
 - `pngCommands`/`svgCommands`: Set LaTeX commands to generate PNG/SVG files.
   This is inspired by the [Edit LaTeX build
   process](https://ankiweb.net/shared/info/937148547) addon to Anki.
 - `presets`: Specify preset combination of model and tags for use with `apy
   add-single`.
 - `profile_name`: Specify which profile to load by default.
 - `query`: Specify default query for `apy list`, `apy review` and `apy tag`.
```

### Comparing `apyanki-0.15.2/pyproject.toml` & `apyanki-0.15.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apyanki"
-version = "0.15.2"
+version = "0.15.3"
 description = "CLI script for interacting with local Anki collection"
 authors = ["Karl Yngve Lervåg <karl.yngve@lervag.net>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `apyanki-0.15.2/src/apyanki/anki.py` & `apyanki-0.15.3/src/apyanki/anki.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import tempfile
 import time
 from types import TracebackType
 from typing import Any, Generator, Optional, Sequence, TYPE_CHECKING, Type
 
 from click import Abort
 from rich.progress import Progress, SpinnerColumn, TextColumn
+from rich.table import Table
 
 from apyanki import cards
 from apyanki.config import cfg
 from apyanki.console import console
 from apyanki.note import Note, NoteData, markdown_file_to_notes
 from apyanki.utilities import cd, choose, editor, suppress_stdout
 
@@ -330,22 +331,23 @@
 
         # Save changes
         self.col.models.update_dict(model)
         self.modified = True
 
     def list_tags(self) -> None:
         """List all tags"""
+        table = Table(show_edge=False, box=None, header_style="bold white")
+        table.add_column("tag", style="cyan")
+        table.add_column("notes", style="magenta", justify="right")
+
         tags = [(t, len(self.col.find_notes(f"tag:{t}"))) for t in self.col.tags.all()]
-        width = len(max(tags, key=lambda x: len(x[0]))[0]) + 2
-        filler = " " * (cfg["width"] - 2 * width - 8)
+        for tag, n in sorted(tags, key=lambda x: x[0]):
+            table.add_row(tag, str(n))
 
-        for (t1, n1), (t2, n2) in zip(
-            sorted(tags, key=lambda x: x[0]), sorted(tags, key=lambda x: x[1])
-        ):
-            console.print(f"{t1:{width}s}{n1:4d}{filler}{t2:{width}s}{n2:4d}")
+        console.print(table)
 
     def change_tags(self, query: str, tags: str, add: bool = True) -> None:
         """Add/Remove tags from notes that match query"""
         note_ids = self.col.find_notes(query)
         if add:
             self.col.tags.bulk_add(note_ids, tags)
         else:
```

### Comparing `apyanki-0.15.2/src/apyanki/cards.py` & `apyanki-0.15.3/src/apyanki/cards.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.2/src/apyanki/cli.py` & `apyanki-0.15.3/src/apyanki/cli.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.2/src/apyanki/config.py` & `apyanki-0.15.3/src/apyanki/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 CFG_DEFAULT_VALUES: dict[str, Any] = {
     "base_path": None,
     "img_viewers": {
         "svg": ["display", "-density", "300"],
     },
     "img_viewers_default": ["feh"],
     "markdown_models": ["Basic"],
+    "markdown_pygments_style": "friendly",
     "presets": {},
     "profile_name": None,
     "query": "tag:marked OR -flag:0",
     "review_show_cards": False,
 }
 
 # Ensure that cfg has required keys
```

### Comparing `apyanki-0.15.2/src/apyanki/console.py` & `apyanki-0.15.3/src/apyanki/console.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.2/src/apyanki/fields.py` & `apyanki-0.15.3/src/apyanki/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from markdown.extensions.abbr import AbbrExtension
 from markdown.extensions.codehilite import CodeHiliteExtension
 from markdown.extensions.def_list import DefListExtension
 from markdown.extensions.fenced_code import FencedCodeExtension
 from markdown.extensions.footnotes import FootnoteExtension
 from markdownify import markdownify as to_md
 
+from apyanki.config import cfg
+
 if TYPE_CHECKING:
     from anki.models import NotetypeDict
     from apyanki.anki import Anki
 
 
 warnings.filterwarnings("ignore", category=MarkupResemblesLocatorWarning)
 
@@ -239,15 +241,15 @@
         text,
         extensions=[
             "tables",
             AbbrExtension(),
             CodeHiliteExtension(
                 noclasses=True,
                 linenums=False,
-                pygments_style="friendly",
+                pygments_style=cfg["markdown_pygments_style"],
                 guess_lang=False,
             ),
             DefListExtension(),
             FencedCodeExtension(),
             FootnoteExtension(),
         ],
         output_format="html",
```

### Comparing `apyanki-0.15.2/src/apyanki/note.py` & `apyanki-0.15.3/src/apyanki/note.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.2/src/apyanki/utilities.py` & `apyanki-0.15.3/src/apyanki/utilities.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.2/PKG-INFO` & `apyanki-0.15.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apyanki
-Version: 0.15.2
+Version: 0.15.3
 Summary: CLI script for interacting with local Anki collection
 Home-page: https://github.com/lervag/apy
 Author: Karl Yngve Lervåg
 Author-email: karl.yngve@lervag.net
 Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
@@ -128,14 +128,17 @@
   '300']` which specifies the command and its options to use for the
   corresponding key (file extension).
 - `img_viewers_default`: Specify the default command to show an image. Must be
   provided as a list of the command and desired options, such as `['feh',
   '-d']`.
 - `markdown_models`: Specify a list of models for which `apy` will use
   a markdown converter.
+- `markdown_pygments_style`: Specify the code highlight scheme to use for
+  fenced code blocks in Markdown notes. See the [Pygments
+  documentation](https://pygments.org/docs/styles/) for more details.
 - `pngCommands`/`svgCommands`: Set LaTeX commands to generate PNG/SVG files.
   This is inspired by the [Edit LaTeX build
   process](https://ankiweb.net/shared/info/937148547) addon to Anki.
 - `presets`: Specify preset combination of model and tags for use with `apy
   add-single`.
 - `profile_name`: Specify which profile to load by default.
 - `query`: Specify default query for `apy list`, `apy review` and `apy tag`.
```

