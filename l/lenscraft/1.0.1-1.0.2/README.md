# Comparing `tmp/lenscraft-1.0.1.tar.gz` & `tmp/lenscraft-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lenscraft-1.0.1.tar", last modified: Tue Apr 23 19:10:46 2024, max compression
+gzip compressed data, was "lenscraft-1.0.2.tar", last modified: Wed Apr 24 19:09:38 2024, max compression
```

## Comparing `lenscraft-1.0.1.tar` & `lenscraft-1.0.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 19:10:46.226827 lenscraft-1.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     3947 2024-04-23 18:41:25.000000 lenscraft-1.0.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      503 2024-04-23 19:08:22.000000 lenscraft-1.0.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1672 2024-04-23 18:41:25.000000 lenscraft-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1285 2024-04-23 19:10:46.226827 lenscraft-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      569 2024-04-23 18:41:25.000000 lenscraft-1.0.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)   388581 2024-04-23 18:41:25.000000 lenscraft-1.0.1/ScreenShot1.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 19:10:46.222826 lenscraft-1.0.1/images/
--rw-rw-rw-   0 root         (0) root         (0)   776666 2024-04-23 18:41:25.000000 lenscraft-1.0.1/images/0.9858_1.1766.png
--rw-rw-rw-   0 root         (0) root         (0)   192094 2024-04-23 18:41:25.000000 lenscraft-1.0.1/images/334.png
--rw-rw-rw-   0 root         (0) root         (0)  4916278 2024-04-23 18:41:25.000000 lenscraft-1.0.1/images/Ring_9_9.png
--rw-rw-rw-   0 root         (0) root         (0)    15666 2024-04-23 18:41:25.000000 lenscraft-1.0.1/images/mask.png
--rw-rw-rw-   0 root         (0) root         (0)   755205 2024-04-23 18:41:25.000000 lenscraft-1.0.1/images/spacer_top__13.png
--rw-rw-rw-   0 root         (0) root         (0)   609893 2024-04-23 18:41:25.000000 lenscraft-1.0.1/images/spacer_top__14.png
--rw-rw-rw-   0 root         (0) root         (0)   750759 2024-04-23 18:41:25.000000 lenscraft-1.0.1/images/spacer_top__3.png
--rw-rw-rw-   0 root         (0) root         (0)   916168 2024-04-23 18:41:25.000000 lenscraft-1.0.1/images/spacer_top__9.png
--rw-rw-rw-   0 root         (0) root         (0)      918 2024-04-23 19:08:22.000000 lenscraft-1.0.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-04-23 18:41:25.000000 lenscraft-1.0.1/requirments.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 19:10:46.226827 lenscraft-1.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 19:10:46.214826 lenscraft-1.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 19:10:46.222826 lenscraft-1.0.1/src/lenscraft/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 18:41:25.000000 lenscraft-1.0.1/src/lenscraft/__init__.py
--rw-r--r--   0 root         (0) root         (0)      411 2024-04-23 19:10:46.000000 lenscraft-1.0.1/src/lenscraft/_version.py
--rw-rw-rw-   0 root         (0) root         (0)       81 2024-04-23 18:41:25.000000 lenscraft-1.0.1/src/lenscraft/app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 19:10:46.226827 lenscraft-1.0.1/src/lenscraft/assets/
--rw-rw-rw-   0 root         (0) root         (0)      923 2024-04-23 18:41:25.000000 lenscraft-1.0.1/src/lenscraft/assets/CornerTemplate.png
--rw-rw-rw-   0 root         (0) root         (0)       65 2024-04-23 18:41:25.000000 lenscraft-1.0.1/src/lenscraft/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 19:10:46.226827 lenscraft-1.0.1/src/lenscraft/editor/
--rw-rw-rw-   0 root         (0) root         (0)     5370 2024-04-23 18:41:25.000000 lenscraft-1.0.1/src/lenscraft/editor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7721 2024-04-23 18:41:25.000000 lenscraft-1.0.1/src/lenscraft/gabor.py
--rw-rw-rw-   0 root         (0) root         (0)     5774 2024-04-23 18:41:25.000000 lenscraft-1.0.1/src/lenscraft/image.py
--rw-rw-rw-   0 root         (0) root         (0)    17849 2024-04-23 18:41:25.000000 lenscraft-1.0.1/src/lenscraft/nodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 19:10:46.226827 lenscraft-1.0.1/src/lenscraft/texture/
--rw-rw-rw-   0 root         (0) root         (0)      637 2024-04-23 18:41:25.000000 lenscraft-1.0.1/src/lenscraft/texture/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2682 2024-04-23 18:41:25.000000 lenscraft-1.0.1/src/lenscraft/texture/classify.py
--rw-rw-rw-   0 root         (0) root         (0)    13815 2024-04-23 18:41:25.000000 lenscraft-1.0.1/src/lenscraft/texture/tool.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2024-04-23 18:41:25.000000 lenscraft-1.0.1/src/lenscraft/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 19:10:46.226827 lenscraft-1.0.1/src/lenscraft.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1285 2024-04-23 19:10:46.000000 lenscraft-1.0.1/src/lenscraft.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      867 2024-04-23 19:10:46.000000 lenscraft-1.0.1/src/lenscraft.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 19:10:46.000000 lenscraft-1.0.1/src/lenscraft.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2024-04-23 19:10:46.000000 lenscraft-1.0.1/src/lenscraft.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      126 2024-04-23 19:10:46.000000 lenscraft-1.0.1/src/lenscraft.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-23 19:10:46.000000 lenscraft-1.0.1/src/lenscraft.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 19:10:46.226827 lenscraft-1.0.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 18:41:25.000000 lenscraft-1.0.1/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:09:38.389312 lenscraft-1.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)     3947 2024-04-23 18:41:25.000000 lenscraft-1.0.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      503 2024-04-23 19:08:22.000000 lenscraft-1.0.2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1672 2024-04-23 18:41:25.000000 lenscraft-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1300 2024-04-24 19:09:38.389312 lenscraft-1.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      584 2024-04-23 19:24:28.000000 lenscraft-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:09:38.377311 lenscraft-1.0.2/images/
+-rw-rw-rw-   0 root         (0) root         (0)   776666 2024-04-23 18:41:25.000000 lenscraft-1.0.2/images/0.9858_1.1766.png
+-rw-rw-rw-   0 root         (0) root         (0)   192094 2024-04-23 18:41:25.000000 lenscraft-1.0.2/images/334.png
+-rw-rw-rw-   0 root         (0) root         (0)  4916278 2024-04-23 18:41:25.000000 lenscraft-1.0.2/images/Ring_9_9.png
+-rw-rw-rw-   0 root         (0) root         (0)    15666 2024-04-23 18:41:25.000000 lenscraft-1.0.2/images/mask.png
+-rw-rw-rw-   0 root         (0) root         (0)   755205 2024-04-23 18:41:25.000000 lenscraft-1.0.2/images/spacer_top__13.png
+-rw-rw-rw-   0 root         (0) root         (0)   609893 2024-04-23 18:41:25.000000 lenscraft-1.0.2/images/spacer_top__14.png
+-rw-rw-rw-   0 root         (0) root         (0)   750759 2024-04-23 18:41:25.000000 lenscraft-1.0.2/images/spacer_top__3.png
+-rw-rw-rw-   0 root         (0) root         (0)   916168 2024-04-23 18:41:25.000000 lenscraft-1.0.2/images/spacer_top__9.png
+-rw-rw-rw-   0 root         (0) root         (0)      918 2024-04-23 19:08:22.000000 lenscraft-1.0.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-04-23 18:41:25.000000 lenscraft-1.0.2/requirments.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 19:09:38.389312 lenscraft-1.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:09:38.333308 lenscraft-1.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:09:38.381311 lenscraft-1.0.2/src/lenscraft/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 18:41:25.000000 lenscraft-1.0.2/src/lenscraft/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-04-24 19:00:28.000000 lenscraft-1.0.2/src/lenscraft/__main__.py
+-rw-r--r--   0 root         (0) root         (0)      411 2024-04-24 19:09:38.000000 lenscraft-1.0.2/src/lenscraft/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       81 2024-04-23 18:41:25.000000 lenscraft-1.0.2/src/lenscraft/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:09:38.385311 lenscraft-1.0.2/src/lenscraft/assets/
+-rw-rw-rw-   0 root         (0) root         (0)      923 2024-04-23 18:41:25.000000 lenscraft-1.0.2/src/lenscraft/assets/CornerTemplate.png
+-rw-rw-rw-   0 root         (0) root         (0)       65 2024-04-23 18:41:25.000000 lenscraft-1.0.2/src/lenscraft/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:09:38.385311 lenscraft-1.0.2/src/lenscraft/editor/
+-rw-rw-rw-   0 root         (0) root         (0)     5370 2024-04-23 18:41:25.000000 lenscraft-1.0.2/src/lenscraft/editor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7721 2024-04-23 18:41:25.000000 lenscraft-1.0.2/src/lenscraft/gabor.py
+-rw-rw-rw-   0 root         (0) root         (0)     5774 2024-04-23 18:41:25.000000 lenscraft-1.0.2/src/lenscraft/image.py
+-rw-rw-rw-   0 root         (0) root         (0)    17849 2024-04-23 18:41:25.000000 lenscraft-1.0.2/src/lenscraft/nodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:09:38.389312 lenscraft-1.0.2/src/lenscraft/texture/
+-rw-rw-rw-   0 root         (0) root         (0)      637 2024-04-23 18:41:25.000000 lenscraft-1.0.2/src/lenscraft/texture/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2682 2024-04-23 18:41:25.000000 lenscraft-1.0.2/src/lenscraft/texture/classify.py
+-rw-rw-rw-   0 root         (0) root         (0)    13972 2024-04-24 19:00:28.000000 lenscraft-1.0.2/src/lenscraft/texture/tool.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2024-04-23 18:41:25.000000 lenscraft-1.0.2/src/lenscraft/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:09:38.389312 lenscraft-1.0.2/src/lenscraft.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1300 2024-04-24 19:09:38.000000 lenscraft-1.0.2/src/lenscraft.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      877 2024-04-24 19:09:38.000000 lenscraft-1.0.2/src/lenscraft.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 19:09:38.000000 lenscraft-1.0.2/src/lenscraft.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2024-04-24 19:09:38.000000 lenscraft-1.0.2/src/lenscraft.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      126 2024-04-24 19:09:38.000000 lenscraft-1.0.2/src/lenscraft.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-24 19:09:38.000000 lenscraft-1.0.2/src/lenscraft.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 19:09:38.389312 lenscraft-1.0.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 18:41:25.000000 lenscraft-1.0.2/tests/__init__.py
```

### Comparing `lenscraft-1.0.1/.gitignore` & `lenscraft-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.1/LICENSE` & `lenscraft-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.1/PKG-INFO` & `lenscraft-1.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lenscraft
-Version: 1.0.1
+Version: 1.0.2
 Summary: Application to quickly build machine vision pipelines with little or no code
 Author-email: Gudjon Einar Magnusson <gmagnusson@fraunhofer.org>
 Project-URL: Homepage, https://cma.fraunhofer.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -39,15 +39,15 @@
 
 
 ## How to Use
 
 1. Add images you want to work with
 2. Build vision pipeline using the Node Editor
 
-![image](/ScreenShot1.png)
+![image](https://i.imgur.com/ELtun4k.png)
 
 ## Developer?
 
 1. Clone the repository
 2. Install the package in edit mode
 
 ```
```

### Comparing `lenscraft-1.0.1/README.md` & `lenscraft-1.0.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 ## How to Use
 
 1. Add images you want to work with
 2. Build vision pipeline using the Node Editor
 
-![image](/ScreenShot1.png)
+![image](https://i.imgur.com/ELtun4k.png)
 
 ## Developer?
 
 1. Clone the repository
 2. Install the package in edit mode
 
 ```
```

### Comparing `lenscraft-1.0.1/images/0.9858_1.1766.png` & `lenscraft-1.0.2/images/0.9858_1.1766.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.1/images/334.png` & `lenscraft-1.0.2/images/334.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.1/images/Ring_9_9.png` & `lenscraft-1.0.2/images/Ring_9_9.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.1/images/mask.png` & `lenscraft-1.0.2/images/mask.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.1/images/spacer_top__13.png` & `lenscraft-1.0.2/images/spacer_top__13.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.1/images/spacer_top__14.png` & `lenscraft-1.0.2/images/spacer_top__14.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.1/images/spacer_top__3.png` & `lenscraft-1.0.2/images/spacer_top__3.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.1/images/spacer_top__9.png` & `lenscraft-1.0.2/images/spacer_top__9.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.1/pyproject.toml` & `lenscraft-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.1/src/lenscraft/assets/CornerTemplate.png` & `lenscraft-1.0.2/src/lenscraft/assets/CornerTemplate.png`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.1/src/lenscraft/editor/__init__.py` & `lenscraft-1.0.2/src/lenscraft/editor/__init__.py`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.1/src/lenscraft/gabor.py` & `lenscraft-1.0.2/src/lenscraft/gabor.py`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.1/src/lenscraft/image.py` & `lenscraft-1.0.2/src/lenscraft/image.py`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.1/src/lenscraft/nodes.py` & `lenscraft-1.0.2/src/lenscraft/nodes.py`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.1/src/lenscraft/texture/__init__.py` & `lenscraft-1.0.2/src/lenscraft/texture/__init__.py`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.1/src/lenscraft/texture/classify.py` & `lenscraft-1.0.2/src/lenscraft/texture/classify.py`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.1/src/lenscraft/texture/tool.py` & `lenscraft-1.0.2/src/lenscraft/texture/tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,18 +129,21 @@
 
                 (w, h) = image.fit(width=600)
                 with dpg.drawlist(width=w, height=h) as canvas:
                     image.draw_image(width=w)
                 self._tabs[tab] = ImageTab(tab, image, canvas)
 
     def _on_mouse_click(self):
-        current_tab = self.current_tab().tab_id
+        if not dpg.is_item_visible(self.id):
+            return
+        
+        current_tab = self.current_tab()
         if not current_tab:
             return
-        canvas = self._tabs[current_tab].canvas_id
+        canvas = self._tabs[current_tab.tab_id].canvas_id
         if not dpg.is_item_hovered(canvas):
             return
 
         current_border = self.current_border()
         if current_border is None:
             self.start_new_border()
         else:
@@ -188,15 +191,18 @@
         canvas = self.current_tab().canvas_id
         start = self.mouse_image_coordinates()
         print("Start:", start)
         new_line = TextureBorder(self.current_tab(), start)
         self.borders.append(new_line)
         self._update_border_list()
 
-    def current_tab(self) -> ImageTab:
+    def current_tab(self) -> Optional[ImageTab]:
+        if self._current_tab_id is None:
+            return None
+        
         return self._tabs[self._current_tab_id]
 
     def current_canvas(self):
         return self.current_tab().canvas_id
 
     def _update_border_list(self):
         # Clear the list
```

### Comparing `lenscraft-1.0.1/src/lenscraft/utils.py` & `lenscraft-1.0.2/src/lenscraft/utils.py`

 * *Files identical despite different names*

### Comparing `lenscraft-1.0.1/src/lenscraft.egg-info/PKG-INFO` & `lenscraft-1.0.2/src/lenscraft.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lenscraft
-Version: 1.0.1
+Version: 1.0.2
 Summary: Application to quickly build machine vision pipelines with little or no code
 Author-email: Gudjon Einar Magnusson <gmagnusson@fraunhofer.org>
 Project-URL: Homepage, https://cma.fraunhofer.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -39,15 +39,15 @@
 
 
 ## How to Use
 
 1. Add images you want to work with
 2. Build vision pipeline using the Node Editor
 
-![image](/ScreenShot1.png)
+![image](https://i.imgur.com/ELtun4k.png)
 
 ## Developer?
 
 1. Clone the repository
 2. Install the package in edit mode
 
 ```
```

### Comparing `lenscraft-1.0.1/src/lenscraft.egg-info/SOURCES.txt` & `lenscraft-1.0.2/src/lenscraft.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 .gitignore
 .gitlab-ci.yml
 LICENSE
 README.md
-ScreenShot1.png
 pyproject.toml
 requirments.txt
 images/0.9858_1.1766.png
 images/334.png
 images/Ring_9_9.png
 images/mask.png
 images/spacer_top__13.png
 images/spacer_top__14.png
 images/spacer_top__3.png
 images/spacer_top__9.png
 src/lenscraft/__init__.py
+src/lenscraft/__main__.py
 src/lenscraft/_version.py
 src/lenscraft/app.py
 src/lenscraft/cli.py
 src/lenscraft/gabor.py
 src/lenscraft/image.py
 src/lenscraft/nodes.py
 src/lenscraft/utils.py
```

