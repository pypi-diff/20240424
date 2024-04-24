# Comparing `tmp/tldraw-2.0.8.tar.gz` & `tmp/tldraw-2.0.9.tar.gz`

## Comparing `tldraw-2.0.8.tar` & `tldraw-2.0.9.tar`

### file list

```diff
@@ -1,29 +1,27 @@
--rw-r--r--   0        0        0     7290 2020-02-02 00:00:00.000000 tldraw-2.0.8/src/tldraw/__init__.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 tldraw-2.0.8/src/tldraw/prompt.py
--rw-r--r--   0        0        0    61221 2020-02-02 00:00:00.000000 tldraw-2.0.8/src/tldraw/static/coordinates.css
--rw-r--r--   0        0        0  1044419 2020-02-02 00:00:00.000000 tldraw-2.0.8/src/tldraw/static/coordinates.js
--rw-r--r--   0        0        0    61328 2020-02-02 00:00:00.000000 tldraw-2.0.8/src/tldraw/static/get_stroke.css
--rw-r--r--   0        0        0  1044173 2020-02-02 00:00:00.000000 tldraw-2.0.8/src/tldraw/static/get_stroke.js
--rw-r--r--   0        0        0    61221 2020-02-02 00:00:00.000000 tldraw-2.0.8/src/tldraw/static/image.css
--rw-r--r--   0        0        0  1044206 2020-02-02 00:00:00.000000 tldraw-2.0.8/src/tldraw/static/image.js
--rw-r--r--   0        0        0    61221 2020-02-02 00:00:00.000000 tldraw-2.0.8/src/tldraw/static/image_and_array.css
--rw-r--r--   0        0        0  1044657 2020-02-02 00:00:00.000000 tldraw-2.0.8/src/tldraw/static/image_and_array.js
--rw-r--r--   0        0        0    61380 2020-02-02 00:00:00.000000 tldraw-2.0.8/src/tldraw/static/makereal.css
--rw-r--r--   0        0        0  1045350 2020-02-02 00:00:00.000000 tldraw-2.0.8/src/tldraw/static/makereal.js
--rw-r--r--   0        0        0   221839 2020-02-02 00:00:00.000000 tldraw-2.0.8/src/tldraw/static/makestatic_markdown.css
--rw-r--r--   0        0        0  7162659 2020-02-02 00:00:00.000000 tldraw-2.0.8/src/tldraw/static/makestatic_markdown.js
--rw-r--r--   0        0        0    61221 2020-02-02 00:00:00.000000 tldraw-2.0.8/src/tldraw/static/makestatic_png.css
--rw-r--r--   0        0        0  1045125 2020-02-02 00:00:00.000000 tldraw-2.0.8/src/tldraw/static/makestatic_png.js
--rw-r--r--   0        0        0    61221 2020-02-02 00:00:00.000000 tldraw-2.0.8/src/tldraw/static/makestatic_svg.css
--rw-r--r--   0        0        0  1044892 2020-02-02 00:00:00.000000 tldraw-2.0.8/src/tldraw/static/makestatic_svg.js
--rw-r--r--   0        0        0    61221 2020-02-02 00:00:00.000000 tldraw-2.0.8/src/tldraw/static/makestatic_tldraw.css
--rw-r--r--   0        0        0  1045523 2020-02-02 00:00:00.000000 tldraw-2.0.8/src/tldraw/static/makestatic_tldraw.js
--rw-r--r--   0        0        0    61380 2020-02-02 00:00:00.000000 tldraw-2.0.8/src/tldraw/static/makestatic_to_markdown.css
--rw-r--r--   0        0        0  1045261 2020-02-02 00:00:00.000000 tldraw-2.0.8/src/tldraw/static/makestatic_to_markdown.js
--rw-r--r--   0        0        0    61328 2020-02-02 00:00:00.000000 tldraw-2.0.8/src/tldraw/static/minimal.css
--rw-r--r--   0        0        0  1044144 2020-02-02 00:00:00.000000 tldraw-2.0.8/src/tldraw/static/minimal.js
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 tldraw-2.0.8/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 tldraw-2.0.8/LICENSE
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 tldraw-2.0.8/README.md
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 tldraw-2.0.8/pyproject.toml
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 tldraw-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0     7290 2020-02-02 00:00:00.000000 tldraw-2.0.9/src/tldraw/__init__.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 tldraw-2.0.9/src/tldraw/prompt.py
+-rw-r--r--   0        0        0    61221 2020-02-02 00:00:00.000000 tldraw-2.0.9/src/tldraw/static/coordinates.css
+-rw-r--r--   0        0        0  1044419 2020-02-02 00:00:00.000000 tldraw-2.0.9/src/tldraw/static/coordinates.js
+-rw-r--r--   0        0        0    61328 2020-02-02 00:00:00.000000 tldraw-2.0.9/src/tldraw/static/get_stroke.css
+-rw-r--r--   0        0        0  1044173 2020-02-02 00:00:00.000000 tldraw-2.0.9/src/tldraw/static/get_stroke.js
+-rw-r--r--   0        0        0    61221 2020-02-02 00:00:00.000000 tldraw-2.0.9/src/tldraw/static/image.css
+-rw-r--r--   0        0        0  1044206 2020-02-02 00:00:00.000000 tldraw-2.0.9/src/tldraw/static/image.js
+-rw-r--r--   0        0        0    61221 2020-02-02 00:00:00.000000 tldraw-2.0.9/src/tldraw/static/image_and_array.css
+-rw-r--r--   0        0        0  1044657 2020-02-02 00:00:00.000000 tldraw-2.0.9/src/tldraw/static/image_and_array.js
+-rw-r--r--   0        0        0    61380 2020-02-02 00:00:00.000000 tldraw-2.0.9/src/tldraw/static/makereal.css
+-rw-r--r--   0        0        0  1045350 2020-02-02 00:00:00.000000 tldraw-2.0.9/src/tldraw/static/makereal.js
+-rw-r--r--   0        0        0    61221 2020-02-02 00:00:00.000000 tldraw-2.0.9/src/tldraw/static/makestatic_png.css
+-rw-r--r--   0        0        0  1045125 2020-02-02 00:00:00.000000 tldraw-2.0.9/src/tldraw/static/makestatic_png.js
+-rw-r--r--   0        0        0    61221 2020-02-02 00:00:00.000000 tldraw-2.0.9/src/tldraw/static/makestatic_svg.css
+-rw-r--r--   0        0        0  1044892 2020-02-02 00:00:00.000000 tldraw-2.0.9/src/tldraw/static/makestatic_svg.js
+-rw-r--r--   0        0        0    61221 2020-02-02 00:00:00.000000 tldraw-2.0.9/src/tldraw/static/makestatic_tldraw.css
+-rw-r--r--   0        0        0  1045523 2020-02-02 00:00:00.000000 tldraw-2.0.9/src/tldraw/static/makestatic_tldraw.js
+-rw-r--r--   0        0        0    61380 2020-02-02 00:00:00.000000 tldraw-2.0.9/src/tldraw/static/makestatic_to_markdown.css
+-rw-r--r--   0        0        0  1045261 2020-02-02 00:00:00.000000 tldraw-2.0.9/src/tldraw/static/makestatic_to_markdown.js
+-rw-r--r--   0        0        0    61328 2020-02-02 00:00:00.000000 tldraw-2.0.9/src/tldraw/static/minimal.css
+-rw-r--r--   0        0        0  1044144 2020-02-02 00:00:00.000000 tldraw-2.0.9/src/tldraw/static/minimal.js
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 tldraw-2.0.9/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 tldraw-2.0.9/LICENSE
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 tldraw-2.0.9/README.md
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 tldraw-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 tldraw-2.0.9/PKG-INFO
```

### Comparing `tldraw-2.0.8/src/tldraw/__init__.py` & `tldraw-2.0.9/src/tldraw/__init__.py`

 * *Files identical despite different names*

### Comparing `tldraw-2.0.8/src/tldraw/prompt.py` & `tldraw-2.0.9/src/tldraw/prompt.py`

 * *Files identical despite different names*

### Comparing `tldraw-2.0.8/src/tldraw/static/coordinates.css` & `tldraw-2.0.9/src/tldraw/static/coordinates.css`

 * *Files identical despite different names*

### Comparing `tldraw-2.0.8/src/tldraw/static/coordinates.js` & `tldraw-2.0.9/src/tldraw/static/coordinates.js`

 * *Files identical despite different names*

### Comparing `tldraw-2.0.8/src/tldraw/static/get_stroke.css` & `tldraw-2.0.9/src/tldraw/static/get_stroke.css`

 * *Files identical despite different names*

### Comparing `tldraw-2.0.8/src/tldraw/static/get_stroke.js` & `tldraw-2.0.9/src/tldraw/static/get_stroke.js`

 * *Files identical despite different names*

### Comparing `tldraw-2.0.8/src/tldraw/static/image.css` & `tldraw-2.0.9/src/tldraw/static/image.css`

 * *Files identical despite different names*

### Comparing `tldraw-2.0.8/src/tldraw/static/image.js` & `tldraw-2.0.9/src/tldraw/static/image.js`

 * *Files identical despite different names*

### Comparing `tldraw-2.0.8/src/tldraw/static/image_and_array.css` & `tldraw-2.0.9/src/tldraw/static/image_and_array.css`

 * *Files identical despite different names*

### Comparing `tldraw-2.0.8/src/tldraw/static/image_and_array.js` & `tldraw-2.0.9/src/tldraw/static/image_and_array.js`

 * *Files identical despite different names*

### Comparing `tldraw-2.0.8/src/tldraw/static/makereal.css` & `tldraw-2.0.9/src/tldraw/static/makereal.css`

 * *Files identical despite different names*

### Comparing `tldraw-2.0.8/src/tldraw/static/makereal.js` & `tldraw-2.0.9/src/tldraw/static/makereal.js`

 * *Files identical despite different names*

### Comparing `tldraw-2.0.8/src/tldraw/static/makestatic_png.css` & `tldraw-2.0.9/src/tldraw/static/makestatic_png.css`

 * *Files identical despite different names*

### Comparing `tldraw-2.0.8/src/tldraw/static/makestatic_png.js` & `tldraw-2.0.9/src/tldraw/static/makestatic_png.js`

 * *Files identical despite different names*

### Comparing `tldraw-2.0.8/src/tldraw/static/makestatic_svg.css` & `tldraw-2.0.9/src/tldraw/static/makestatic_svg.css`

 * *Files identical despite different names*

### Comparing `tldraw-2.0.8/src/tldraw/static/makestatic_svg.js` & `tldraw-2.0.9/src/tldraw/static/makestatic_svg.js`

 * *Files identical despite different names*

### Comparing `tldraw-2.0.8/src/tldraw/static/makestatic_tldraw.css` & `tldraw-2.0.9/src/tldraw/static/makestatic_tldraw.css`

 * *Files identical despite different names*

### Comparing `tldraw-2.0.8/src/tldraw/static/makestatic_tldraw.js` & `tldraw-2.0.9/src/tldraw/static/makestatic_tldraw.js`

 * *Files identical despite different names*

### Comparing `tldraw-2.0.8/src/tldraw/static/makestatic_to_markdown.css` & `tldraw-2.0.9/src/tldraw/static/makestatic_to_markdown.css`

 * *Files identical despite different names*

### Comparing `tldraw-2.0.8/src/tldraw/static/makestatic_to_markdown.js` & `tldraw-2.0.9/src/tldraw/static/makestatic_to_markdown.js`

 * *Files identical despite different names*

### Comparing `tldraw-2.0.8/src/tldraw/static/minimal.css` & `tldraw-2.0.9/src/tldraw/static/minimal.css`

 * *Files identical despite different names*

### Comparing `tldraw-2.0.8/src/tldraw/static/minimal.js` & `tldraw-2.0.9/src/tldraw/static/minimal.js`

 * *Files identical despite different names*

### Comparing `tldraw-2.0.8/LICENSE` & `tldraw-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tldraw-2.0.8/README.md` & `tldraw-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `tldraw-2.0.8/pyproject.toml` & `tldraw-2.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tldraw"
-version = "2.0.8"
+version = "2.0.9"
 dependencies = ["anywidget", "ipylab", "requests", "ipykernel"]
 description = "Tldraw for Jupyter"
 license = "MIT"
 readme = "README.md"
 [project.optional-dependencies]
 dev = ["watchfiles", "jupyterlab"]
```

### Comparing `tldraw-2.0.8/PKG-INFO` & `tldraw-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: tldraw
-Version: 2.0.8
+Version: 2.0.9
 Summary: Tldraw for Jupyter
 License-Expression: MIT
 License-File: LICENSE
 Requires-Dist: anywidget
 Requires-Dist: ipykernel
 Requires-Dist: ipylab
 Requires-Dist: requests
```

