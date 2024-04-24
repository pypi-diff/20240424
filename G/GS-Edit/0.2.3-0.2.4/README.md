# Comparing `tmp/gs_edit-0.2.3.tar.gz` & `tmp/gs_edit-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gs_edit-0.2.3.tar", last modified: Mon Apr 22 04:40:30 2024, max compression
+gzip compressed data, was "gs_edit-0.2.4.tar", last modified: Wed Apr 24 05:21:32 2024, max compression
```

## Comparing `gs_edit-0.2.3.tar` & `gs_edit-0.2.4.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 04:40:29.880000 gs_edit-0.2.3/
--rw-rw-rw-   0        0        0     1066 2024-02-12 21:48:00.000000 gs_edit-0.2.3/LICENSE
--rw-rw-rw-   0        0        0      112 2024-04-22 04:40:00.000000 gs_edit-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1738 2024-04-22 04:40:32.000000 gs_edit-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1318 2024-04-04 04:14:34.000000 gs_edit-0.2.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-22 04:40:32.000000 gs_edit-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      771 2024-04-22 04:23:26.000000 gs_edit-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 04:40:29.880000 gs_edit-0.2.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-22 04:40:29.890000 gs_edit-0.2.3/src/GS_Edit.egg-info/
--rw-rw-rw-   0        0        0     1738 2024-04-22 04:40:30.000000 gs_edit-0.2.3/src/GS_Edit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1135 2024-04-22 04:40:30.000000 gs_edit-0.2.3/src/GS_Edit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 04:40:30.000000 gs_edit-0.2.3/src/GS_Edit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-04-22 04:40:30.000000 gs_edit-0.2.3/src/GS_Edit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2024-04-22 04:40:30.000000 gs_edit-0.2.3/src/GS_Edit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-22 04:40:30.000000 gs_edit-0.2.3/src/GS_Edit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-22 04:40:29.890000 gs_edit-0.2.3/src/gsedit/
--rw-rw-rw-   0        0        0        0 2024-04-22 02:06:00.000000 gs_edit-0.2.3/src/gsedit/__init__.py
--rw-rw-rw-   0        0        0      382 2024-04-22 02:45:16.000000 gs_edit-0.2.3/src/gsedit/cli.py
--rw-rw-rw-   0        0        0      958 2024-03-26 00:10:36.000000 gs_edit-0.2.3/src/gsedit/code_completer.py
-drwxrwxrwx   0        0        0        0 2024-04-22 04:40:29.900000 gs_edit-0.2.3/src/gsedit/css/
--rw-rw-rw-   0        0        0      369 2024-04-19 04:20:18.000000 gs_edit-0.2.3/src/gsedit/css/cssEditor.qss
--rw-rw-rw-   0        0        0       59 2024-03-26 00:10:44.000000 gs_edit-0.2.3/src/gsedit/css/grep.qss
--rw-rw-rw-   0        0        0      544 2024-04-12 01:05:14.000000 gs_edit-0.2.3/src/gsedit/css/integratedTerminal.qss
--rw-rw-rw-   0        0        0       51 2024-04-19 04:17:04.000000 gs_edit-0.2.3/src/gsedit/css/mainBody.qss
--rw-rw-rw-   0        0        0      276 2024-04-19 17:13:16.000000 gs_edit-0.2.3/src/gsedit/css/menuBar.qss
--rw-rw-rw-   0        0        0       43 2024-03-25 04:28:56.000000 gs_edit-0.2.3/src/gsedit/css/sidebar.qss
--rw-rw-rw-   0        0        0       94 2024-04-19 19:39:08.000000 gs_edit-0.2.3/src/gsedit/css/statusBar.qss
--rw-rw-rw-   0        0        0     2874 2024-04-19 04:14:20.000000 gs_edit-0.2.3/src/gsedit/css/style.qss
--rw-rw-rw-   0        0        0      450 2024-04-22 02:58:04.000000 gs_edit-0.2.3/src/gsedit/css/tabBar.qss
--rw-rw-rw-   0        0        0      165 2024-03-26 00:10:46.000000 gs_edit-0.2.3/src/gsedit/css/tools.qss
--rw-rw-rw-   0        0        0     8520 2024-04-22 03:00:52.000000 gs_edit-0.2.3/src/gsedit/css_editor.py
--rw-rw-rw-   0        0        0     8720 2024-04-22 02:33:12.000000 gs_edit-0.2.3/src/gsedit/file_explorer.py
--rw-rw-rw-   0        0        0     4445 2024-04-22 02:47:20.000000 gs_edit-0.2.3/src/gsedit/grep.py
--rw-rw-rw-   0        0        0     3381 2024-04-22 02:35:40.000000 gs_edit-0.2.3/src/gsedit/grepgine.py
--rw-rw-rw-   0        0        0     1477 2024-03-21 05:28:34.000000 gs_edit-0.2.3/src/gsedit/gsconfig.py
-drwxrwxrwx   0        0        0        0 2024-04-22 04:40:29.900000 gs_edit-0.2.3/src/gsedit/images/
--rw-rw-rw-   0        0        0     1240 2024-02-22 23:10:24.000000 gs_edit-0.2.3/src/gsedit/images/close.svg
--rw-rw-rw-   0        0        0     1087 2024-02-22 19:27:58.000000 gs_edit-0.2.3/src/gsedit/images/folder.svg
--rw-rw-rw-   0        0        0     1918 2024-02-29 06:36:00.000000 gs_edit-0.2.3/src/gsedit/images/grep.svg
--rw-rw-rw-   0        0        0  2514652 2024-03-24 21:36:04.000000 gs_edit-0.2.3/src/gsedit/images/icon.png
--rw-rw-rw-   0        0        0     4388 2024-04-22 02:51:32.000000 gs_edit-0.2.3/src/gsedit/integrated_terminal.py
--rw-rw-rw-   0        0        0    19217 2024-04-22 02:35:24.000000 gs_edit-0.2.3/src/gsedit/language_lexer.py
--rw-rw-rw-   0        0        0     3017 2024-04-22 02:43:30.000000 gs_edit-0.2.3/src/gsedit/main.py
--rw-rw-rw-   0        0        0     1955 2024-04-22 02:47:40.000000 gs_edit-0.2.3/src/gsedit/main_body.py
--rw-rw-rw-   0        0        0    14413 2024-04-22 02:47:58.000000 gs_edit-0.2.3/src/gsedit/menu_bar.py
--rw-rw-rw-   0        0        0      882 2024-04-22 02:53:56.000000 gs_edit-0.2.3/src/gsedit/popup.py
--rw-rw-rw-   0        0        0    11554 2024-03-26 00:10:42.000000 gs_edit-0.2.3/src/gsedit/res_src.py
--rw-rw-rw-   0        0        0     3237 2024-04-22 02:49:22.000000 gs_edit-0.2.3/src/gsedit/sidebar.py
--rw-rw-rw-   0        0        0      700 2024-04-22 02:45:14.000000 gs_edit-0.2.3/src/gsedit/status_bar.py
--rw-rw-rw-   0        0        0     1599 2024-04-22 02:58:22.000000 gs_edit-0.2.3/src/gsedit/tab_bar.py
--rw-rw-rw-   0        0        0     6945 2024-04-22 02:50:02.000000 gs_edit-0.2.3/src/gsedit/text_editor.py
--rw-rw-rw-   0        0        0     2524 2024-04-22 02:50:20.000000 gs_edit-0.2.3/src/gsedit/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-22 04:40:29.910000 gs_edit-0.2.3/src/tests/
--rw-rw-rw-   0        0        0        0 2024-04-22 02:04:38.000000 gs_edit-0.2.3/src/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 05:21:32.300000 gs_edit-0.2.4/
+-rw-rw-rw-   0        0        0     1066 2024-02-12 21:48:00.000000 gs_edit-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0      151 2024-04-22 18:02:04.000000 gs_edit-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1738 2024-04-24 05:21:34.000000 gs_edit-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1318 2024-04-04 04:14:34.000000 gs_edit-0.2.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-24 05:21:34.000000 gs_edit-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      787 2024-04-23 18:26:06.000000 gs_edit-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 05:21:32.310000 gs_edit-0.2.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-24 05:21:32.310000 gs_edit-0.2.4/src/GS_Edit.egg-info/
+-rw-rw-rw-   0        0        0     1738 2024-04-24 05:21:34.000000 gs_edit-0.2.4/src/GS_Edit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1167 2024-04-24 05:21:34.000000 gs_edit-0.2.4/src/GS_Edit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 05:21:34.000000 gs_edit-0.2.4/src/GS_Edit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-24 05:21:34.000000 gs_edit-0.2.4/src/GS_Edit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2024-04-24 05:21:34.000000 gs_edit-0.2.4/src/GS_Edit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-24 05:21:34.000000 gs_edit-0.2.4/src/GS_Edit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 05:21:32.320000 gs_edit-0.2.4/src/gsedit/
+-rw-rw-rw-   0        0        0        0 2024-04-22 02:06:00.000000 gs_edit-0.2.4/src/gsedit/__init__.py
+-rw-rw-rw-   0        0        0      614 2024-04-23 18:26:06.000000 gs_edit-0.2.4/src/gsedit/cli.py
+-rw-rw-rw-   0        0        0      958 2024-03-26 00:10:36.000000 gs_edit-0.2.4/src/gsedit/code_completer.py
+drwxrwxrwx   0        0        0        0 2024-04-24 05:21:32.320000 gs_edit-0.2.4/src/gsedit/css/
+-rw-rw-rw-   0        0        0      369 2024-04-19 04:20:18.000000 gs_edit-0.2.4/src/gsedit/css/cssEditor.qss
+-rw-rw-rw-   0        0        0      208 2024-04-24 03:57:16.000000 gs_edit-0.2.4/src/gsedit/css/grep.qss
+-rw-rw-rw-   0        0        0      544 2024-04-12 01:05:14.000000 gs_edit-0.2.4/src/gsedit/css/integratedTerminal.qss
+-rw-rw-rw-   0        0        0       46 2024-04-24 02:18:48.000000 gs_edit-0.2.4/src/gsedit/css/mainBody.qss
+-rw-rw-rw-   0        0        0      459 2024-04-24 04:13:14.000000 gs_edit-0.2.4/src/gsedit/css/menuBar.qss
+-rw-rw-rw-   0        0        0      251 2024-04-24 04:06:14.000000 gs_edit-0.2.4/src/gsedit/css/sidebar.qss
+-rw-rw-rw-   0        0        0      232 2024-04-24 04:03:04.000000 gs_edit-0.2.4/src/gsedit/css/statusBar.qss
+-rw-rw-rw-   0        0        0     2943 2024-04-24 03:58:20.000000 gs_edit-0.2.4/src/gsedit/css/style.qss
+-rw-rw-rw-   0        0        0      450 2024-04-22 02:58:04.000000 gs_edit-0.2.4/src/gsedit/css/tabBar.qss
+-rw-rw-rw-   0        0        0      140 2024-04-24 03:57:38.000000 gs_edit-0.2.4/src/gsedit/css/tools.qss
+-rw-rw-rw-   0        0        0     8520 2024-04-22 03:00:52.000000 gs_edit-0.2.4/src/gsedit/css_editor.py
+-rw-rw-rw-   0        0        0     8968 2024-04-23 18:26:06.000000 gs_edit-0.2.4/src/gsedit/file_explorer.py
+-rw-rw-rw-   0        0        0     4587 2024-04-24 03:56:58.000000 gs_edit-0.2.4/src/gsedit/grep.py
+-rw-rw-rw-   0        0        0     3395 2024-04-22 23:35:32.000000 gs_edit-0.2.4/src/gsedit/grepgine.py
+-rw-rw-rw-   0        0        0     1900 2024-04-23 18:26:06.000000 gs_edit-0.2.4/src/gsedit/gsconfig.py
+drwxrwxrwx   0        0        0        0 2024-04-24 05:21:32.330000 gs_edit-0.2.4/src/gsedit/images/
+-rw-rw-rw-   0        0        0     1240 2024-02-22 23:10:24.000000 gs_edit-0.2.4/src/gsedit/images/close.svg
+-rw-rw-rw-   0        0        0     1087 2024-02-22 19:27:58.000000 gs_edit-0.2.4/src/gsedit/images/folder.svg
+-rw-rw-rw-   0        0        0     1918 2024-02-29 06:36:00.000000 gs_edit-0.2.4/src/gsedit/images/grep.svg
+-rw-rw-rw-   0        0        0  2514652 2024-03-24 21:36:04.000000 gs_edit-0.2.4/src/gsedit/images/icon.png
+-rw-rw-rw-   0        0        0      168 2024-02-26 00:10:40.000000 gs_edit-0.2.4/src/gsedit/images/resources.qrc
+-rw-rw-rw-   0        0        0     4388 2024-04-22 02:51:32.000000 gs_edit-0.2.4/src/gsedit/integrated_terminal.py
+-rw-rw-rw-   0        0        0    22083 2024-04-23 18:26:06.000000 gs_edit-0.2.4/src/gsedit/language_lexer.py
+-rw-rw-rw-   0        0        0     3135 2024-04-24 03:58:28.000000 gs_edit-0.2.4/src/gsedit/main.py
+-rw-rw-rw-   0        0        0     2031 2024-04-24 02:17:58.000000 gs_edit-0.2.4/src/gsedit/main_body.py
+-rw-rw-rw-   0        0        0    14632 2024-04-23 22:22:26.000000 gs_edit-0.2.4/src/gsedit/menu_bar.py
+-rw-rw-rw-   0        0        0      882 2024-04-22 02:53:56.000000 gs_edit-0.2.4/src/gsedit/popup.py
+-rw-rw-rw-   0        0        0    11554 2024-03-26 00:10:42.000000 gs_edit-0.2.4/src/gsedit/res_src.py
+-rw-rw-rw-   0        0        0     4374 2024-04-24 03:45:04.000000 gs_edit-0.2.4/src/gsedit/sidebar.py
+-rw-rw-rw-   0        0        0      700 2024-04-22 02:45:14.000000 gs_edit-0.2.4/src/gsedit/status_bar.py
+-rw-rw-rw-   0        0        0     1599 2024-04-22 02:58:22.000000 gs_edit-0.2.4/src/gsedit/tab_bar.py
+-rw-rw-rw-   0        0        0     7292 2024-04-23 22:24:56.000000 gs_edit-0.2.4/src/gsedit/text_editor.py
+-rw-rw-rw-   0        0        0     2524 2024-04-23 19:53:56.000000 gs_edit-0.2.4/src/gsedit/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-24 05:21:32.330000 gs_edit-0.2.4/src/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-22 02:04:38.000000 gs_edit-0.2.4/src/tests/__init__.py
```

### Comparing `gs_edit-0.2.3/LICENSE` & `gs_edit-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.3/PKG-INFO` & `gs_edit-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GS-Edit
-Version: 0.2.3
+Version: 0.2.4
 Summary: The Best Code Editor - GS
 Home-page: https://github.com/james-kaddissi/gs_edit
 Author: James Kaddissi
 Author-email: jameskaddissi@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gs_edit-0.2.3/README.md` & `gs_edit-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.3/setup.py` & `gs_edit-0.2.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='GS-Edit', 
-    version='0.2.3',
+    version='0.2.4',
     description='The Best Code Editor - GS',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',  
     author='James Kaddissi',
     author_email='jameskaddissi@gmail.com',
     url='https://github.com/james-kaddissi/gs_edit',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     package_data={
-        'gsedit': ['css/*.qss', 'images/*.png', 'images/*.svg'],
+        'gsedit': ['css/*.qss', 'images/*.png', 'images/*.svg', 'images/*.qrc'],
     },
     install_requires=[
         'PyQt5',  
         'QScintilla',
         'jedi'
     ],
     entry_points={
```

### Comparing `gs_edit-0.2.3/src/GS_Edit.egg-info/PKG-INFO` & `gs_edit-0.2.4/src/GS_Edit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GS-Edit
-Version: 0.2.3
+Version: 0.2.4
 Summary: The Best Code Editor - GS
 Home-page: https://github.com/james-kaddissi/gs_edit
 Author: James Kaddissi
 Author-email: jameskaddissi@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gs_edit-0.2.3/src/GS_Edit.egg-info/SOURCES.txt` & `gs_edit-0.2.4/src/GS_Edit.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -38,8 +38,9 @@
 src/gsedit/css/style.qss
 src/gsedit/css/tabBar.qss
 src/gsedit/css/tools.qss
 src/gsedit/images/close.svg
 src/gsedit/images/folder.svg
 src/gsedit/images/grep.svg
 src/gsedit/images/icon.png
+src/gsedit/images/resources.qrc
 src/tests/__init__.py
```

### Comparing `gs_edit-0.2.3/src/gsedit/code_completer.py` & `gs_edit-0.2.4/src/gsedit/code_completer.py`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.3/src/gsedit/css/integratedTerminal.qss` & `gs_edit-0.2.4/src/gsedit/css/integratedTerminal.qss`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.3/src/gsedit/css/style.qss` & `gs_edit-0.2.4/src/gsedit/css/style.qss`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 QMainWindow {
-    background-color: #0C0C1A;
-    color: #bebebe
+    background-color: red;
+    color: #bebebe;
+    padding: 0px;
+    margin: 0px;
 }
 
 QSplitter {
     background-color: #32303d;
+    padding: 0px;
+    margin: 0px;
 }
 
 QSplitter::handle {
-    background-color: #c678dd;
+    background-color: black;
 }
 
 QScrollBar:vertical {
     border: none;
     width: 12px;
     margin: 15px 0 15px 0;
     background-color: #2e2e2e;
```

### Comparing `gs_edit-0.2.3/src/gsedit/css_editor.py` & `gs_edit-0.2.4/src/gsedit/css_editor.py`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.3/src/gsedit/file_explorer.py` & `gs_edit-0.2.4/src/gsedit/file_explorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,21 @@
         self.itemDelegate().closeEditor.connect(self.close_editor)
 
     def set_no_root(self):
         # Clear the root path
         self.file_system_model.setRootPath("No Folder Opened")
         self.setRootIndex(QModelIndex()) 
         self.setEnabled(False) 
+    
+    def open_file_in_tab(self, file_path):
+        editor = TextEditor()
+        with open(file_path, 'r', encoding='utf-8') as file:
+            editor.setText(file.read())
+        self.tab.addTab(editor, os.path.basename(file_path))
+
 
     def set_root_path(self, path):
         self.file_system_model.setRootPath(path)
         self.setRootIndex(self.file_system_model.index(path))
         self.setEnabled(True)  
 
     def enable_explorer(self):
```

### Comparing `gs_edit-0.2.3/src/gsedit/grep.py` & `gs_edit-0.2.4/src/gsedit/grep.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,61 +49,60 @@
             self.setStyleSheet(style_file.read())
 
 class GrepResult(QListWidget):
     def __init__(self, window) -> None:
         super(GrepResult, self).__init__()
         self.window = window
         self.initialize_results()
+        self.refresh_style()
+
+    def refresh_style(self):
+        base_path = os.path.dirname(__file__) 
+        style_sheet_path = os.path.join(base_path, 'css', 'grep.qss')
+        with open(style_sheet_path, "r") as style_file:
+            self.setStyleSheet(style_file.read())
 
     def initialize_results(self):
         self.setFont(QFont("Fixedsys", 14))
-        self.setStyleSheet("""
-            QListWidget {
-                background-color: #0C0C1A;
-                border-radius: 5px;
-                border: 1px solid #CDCDCD;
-                padding: 5px;
-                color: #CDCDCD;
-            }
-        """)
         self.itemClicked.connect(self.grep_view_clicked)
 
     def grep_view_clicked(self, content):
         self.add_tab(self.window, Path(content.path))
         editor = self.window.tab.currentWidget()
         editor.setCursorPosition(content.ln, content.endln)
         editor.setFocus()
 
     def finish_grep(self, content):
         self.clear()
         for i in content:
             self.addItem(i)
 
-    def text_editor(self, path=None, pyf=None, cf=None, jsonf=None, rustf=None, cppf=None) -> QsciScintilla:
-        editor = TextEditor(self.window, path=path, pyf=pyf, cf=cf, jsonf=jsonf, rustf=rustf, cppf=cppf)
+    def text_editor(self, path=None, pyf=None, cf=None, jsonf=None, rustf=None, cppf=None, jsf=None) -> QsciScintilla:
+        editor = TextEditor(self.window, path=path, pyf=pyf, cf=cf, jsonf=jsonf, rustf=rustf, cppf=cppf, jsf=jsf)
         return editor
 
     def valid_file_check(self, path):
         with open(path, 'rb') as f:
             return b'\0' in f.read(1024)
 
     def add_tab(self, window, path: Path, is_new_file=False):
         if not is_new_file and self.valid_file_check(path):
             window.statusBar().set_timed_message("Cannot open this file type", 2000)
             return
         if path.is_dir():
             return
 
         editor = self.text_editor(
-            path, 
-            path.suffix in gsconfig.get_consideration("python"), 
-            path.suffix in gsconfig.get_consideration("c"), 
-            path.suffix in gsconfig.get_consideration("json"),
-            path.suffix in gsconfig.get_consideration("rust"), 
-            path.suffix in gsconfig.get_consideration("cpp")
+            path,
+            path.suffix in gsedit.gsconfig.get_consideration("python"), 
+            path.suffix in gsedit.gsconfig.get_consideration("c"), 
+            path.suffix in gsedit.gsconfig.get_consideration("json"),
+            path.suffix in gsedit.gsconfig.get_consideration("rust"), 
+            path.suffix in gsedit.gsconfig.get_consideration("cpp"),
+            path.suffix in gsedit.gsconfig.get_consideration("javascript")
         )
         if is_new_file:
             window.tab.addTab(editor, "untitled")
             window.setWindowTitle("untitled - " + window.app_title)
             window.statusBar().set_timed_message("untitled created", 2000)
             window.tab.setCurrentIndex(window.tab.count() - 1)
             window.current_file = None
```

### Comparing `gs_edit-0.2.3/src/gsedit/grepgine.py` & `gs_edit-0.2.4/src/gsedit/grepgine.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,19 +76,19 @@
                                         path,
                                         j,
                                         l.end(),
                                         k[l.start():].strip()[:200]
                                     )
                                     self.content.append(prep)
                         except re.error as err:
-                            if gsconfig.get_config("debugMode"):
+                            if gsedit.gsconfig.get_config("debugMode"):
                                 print(err)
                             
                 except:
-                    if gsconfig.get_config("debugMode"):
+                    if gsedit.gsconfig.get_config("debugMode"):
                         print(err)
                     continue
         self.final_result.emit(self.content)
 
     def activate(self):
         self.grep()
```

### Comparing `gs_edit-0.2.3/src/gsedit/gsconfig.py` & `gs_edit-0.2.4/src/gsedit/gsconfig.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import json
+import os
 
-config_path = 'gsconfig.json'
+base_path = os.path.dirname(__file__)
+config_path = os.path.join(base_path, 'gsconfig.json')
 
 def get_config(name):
     try:
         with open(config_path, 'r') as file:
             config = json.load(file)
 
         return config[name]
@@ -41,8 +43,18 @@
         with open(config_path, 'r') as file:
             config = json.load(file)
 
         return config["language-considerations"][name]
 
     except FileNotFoundError:
         print("Config file not found, please ensure the config_path is correct and points to a proper config json.")
+        return None
+    
+def get_preference(category, pref):
+    try:
+        with open(config_path, 'r') as file:
+            config = json.load(file)
+
+        return config[category][pref]
+    except FileNotFoundError:
+        print("Config file not found, please ensure the config_path is correct and points to a proper config json.")
         return None
```

### Comparing `gs_edit-0.2.3/src/gsedit/images/close.svg` & `gs_edit-0.2.4/src/gsedit/images/close.svg`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.3/src/gsedit/images/folder.svg` & `gs_edit-0.2.4/src/gsedit/images/folder.svg`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.3/src/gsedit/images/grep.svg` & `gs_edit-0.2.4/src/gsedit/images/grep.svg`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.3/src/gsedit/images/icon.png` & `gs_edit-0.2.4/src/gsedit/images/icon.png`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.3/src/gsedit/integrated_terminal.py` & `gs_edit-0.2.4/src/gsedit/integrated_terminal.py`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.3/src/gsedit/language_lexer.py` & `gs_edit-0.2.4/src/gsedit/language_lexer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import builtins
 import keyword
 import re
 import types
 import json
+import os
 
 from PyQt5.Qsci import *
 from PyQt5.QtCore import *
 from PyQt5.QtGui import *
 from PyQt5.QtWidgets import *
 
 import gsedit.gsconfig
@@ -82,15 +83,17 @@
             "demiBold": QFont.DemiBold,
             "bold": QFont.Bold,
             "extraBold": QFont.ExtraBold,
             "black": QFont.Black
         }
 
     def _generateTheme(self):
-        with open(self.path, "r") as file:
+        base_path = os.path.dirname(__file__)
+        config_path = os.path.join(base_path, 'active-theme.json')
+        with open(config_path, "r") as file:
             self.theme = json.load(file)
 
         syntax_rules = self.theme["active-theme"]["syntax-rules"]
 
         for i in syntax_rules:
             item = list(i.keys())[0]
 
@@ -474,14 +477,81 @@
             elif token.isdigit():
                 self.setStyling(token_length, self.CONSTANTS)
             elif token in self.saved_names:
                 self.setStyling(token_length, self.FUNCTIONS)
             else:
                 self.setStyling(token_length, self.DEFAULT)
 
+class JavaScriptLexer(GSLexer):
+    def __init__(self, editor):
+        super(JavaScriptLexer, self).__init__("JavaScript", editor)
+        self.generateKeywords([
+            "break", "case", "catch", "class", "const", "continue", "debugger", "default", "delete",
+            "do", "else", "export", "extends", "finally", "for", "function", "if", "import",
+            "in", "instanceof", "let", "new", "return", "super", "switch", "this", "throw",
+            "try", "typeof", "var", "void", "while", "with", "yield", "async", "await"
+        ])
+        self.generateSavedNames([
+            "Array", "Date", "eval", "function", "hasOwnProperty", "Infinity", "isNaN", "isFinite", 
+            "Number", "Object", "parseFloat", "parseInt", "String", "Boolean", "RegExp", "Error",
+            "console", "window", "document"
+        ])
+
+    def styleText(self, start, end):
+        self.startStyling(start)
+
+        text = self.editor.text()[start:end]
+        self.get_token(text)
+
+        is_string = False
+        is_comment = False
+
+        while True:
+            curr_token = self.get_next_token()
+            if curr_token is None:
+                break
+            token, token_length = curr_token
+
+            if is_comment:
+                self.setStyling(token_length, self.COMMENTS)
+                if token.startswith("*/") or token == "\n":
+                    is_comment = False
+                continue
+
+            if is_string:
+                self.setStyling(token_length, self.STRING)
+                if token in ['"', "'"]:
+                    is_string = False
+                continue
+
+            if token in self.keywords:
+                self.setStyling(token_length, self.KEYWORD)
+            elif token.startswith("/*"):
+                self.setStyling(token_length, self.COMMENTS)
+                is_comment = True
+            elif token == "//":
+                self.setStyling(token_length, self.COMMENTS)
+                self.skip_to_end_of_line()
+            elif token in ['"', "'"]:
+                self.setStyling(token_length, self.STRING)
+                is_string = True
+            elif token.isdigit():
+                self.setStyling(token_length, self.CONSTANTS)
+            elif token in self.saved_names:
+                self.setStyling(token_length, self.FUNCTIONS)
+            else:
+                self.setStyling(token_length, self.DEFAULT)
+
+    def skip_to_end_of_line(self):
+        text = self.editor.text()
+        pos = self.currentPosition
+        while pos < len(text) and text[pos] != '\n':
+            pos += 1
+        self.setStyling(pos - self.currentPosition, self.COMMENTS)
+        self.currentPosition = pos
 
 
 class JSONLexer(GSLexer):
     def __init__(self, editor):
         super(JSONLexer, self).__init__("JSON", editor)
         self.generateSavedNames([
             "true",
```

### Comparing `gs_edit-0.2.3/src/gsedit/main.py` & `gs_edit-0.2.4/src/gsedit/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         super(QMainWindow, self).__init__()
         self.app_title = "GS-Edit"
         self.app_icon = QIcon("./src/gsedit/images/icon.png")
         self.setWindowIcon(self.app_icon)
         self.app_version = "0.1.0"
         self.initialize_window()
         self.current_file = None
-        self.current_tool = "folder"
+        self.current_tool = None
         self.css_editor = CSSEditor(self)
 
     def initialize_window(self):
         # window configuration
         self.setWindowTitle(self.app_title)
         self.resize(1400, 1000)
         base_path = os.path.dirname(__file__)
@@ -58,21 +58,24 @@
         top_menu_bar = MenuBar(self, self.bar, self.file_explorer_frame.file_explorer)
         self.setMenuBar(top_menu_bar)
 
     def configure_body(self):
         # main body
         self.sidebar = Sidebar(self)
         self.horizontal_split = QSplitter(Qt.Horizontal)
+        self.horizontal_split.setHandleWidth(2)
         self.tab = TabBar(self, self.bar)
         self.grep_frame = GrepFrame(self)
         self.file_explorer_frame = FileExplorerFrame(self)
         self.horizontal_split.addWidget(self.file_explorer_frame)
         self.horizontal_split.addWidget(self.tab)
         self.main_body_frame = MainBodyFrame(self)
         self.setCentralWidget(self.main_body_frame)
+        self.file_explorer_frame.hide()
+        self.grep_frame.hide()
 
     def toggle_terminal(self):
         if self.main_body_frame.terminal_widget.isVisible():
             self.main_body_frame.terminal_widget.hide()
         else:
             self.main_body_frame.terminal_widget.show()
```

### Comparing `gs_edit-0.2.3/src/gsedit/main_body.py` & `gs_edit-0.2.4/src/gsedit/main_body.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,35 +7,37 @@
 from gsedit.integrated_terminal import IntegratedTerminal
 
 import os
 
 class MainBodyFrame(QFrame):
     def __init__(self, window) -> None:
         super(MainBodyFrame, self).__init__()
-        self.refresh_style()
         self.window = window
         self.initialize_frame()
         self.set_layout()
+        self.refresh_style()
 
     def refresh_style(self):
         base_path = os.path.dirname(__file__) 
         style_sheet_path = os.path.join(base_path, 'css', 'mainBody.qss')
         with open(style_sheet_path, "r") as style_file:
             self.setStyleSheet(style_file.read())
 
     def initialize_frame(self):
         self.setFrameShape(QFrame.NoFrame)
         self.setFrameShadow(QFrame.Plain)
         self.setLineWidth(0)
         self.setMidLineWidth(0)
-        self.setContentsMargins(0, 0, 0, 0,)
+        self.setContentsMargins(0, 0, 0, 0)
         self.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
     
     def set_layout(self):
         layout = QVBoxLayout(self)
+        layout.setContentsMargins(0, 0, 0, 0)
+        layout.setSpacing(0)
         self.vertical_split = QSplitter(Qt.Vertical)  # This splitter will manage the main content and the terminal
         
         self.editor_area = QWidget()  # Container for the main editor layout
         editor_layout = QHBoxLayout(self.editor_area)
         editor_layout.setContentsMargins(0, 0, 0, 0)
         editor_layout.setSpacing(0)
         editor_layout.addWidget(self.window.sidebar)
```

### Comparing `gs_edit-0.2.3/src/gsedit/menu_bar.py` & `gs_edit-0.2.4/src/gsedit/menu_bar.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,32 +209,38 @@
         self.edit_style_option()
     def edit_style_option(self):
         edit_css = QAction("Edit Styles", self)
         edit_css.triggered.connect(self.edit_style_command)
         self.style_menu.addAction(edit_css)
 
     def new_file_command(self):
-        self.window.add_tab(Path("untitled"), is_new_file=True)
+        self.window.grep_frame.grep_view.add_tab(self.window, Path("untitled"), is_new_file=True)
     def new_folder_command(self):
         folder_path = Path(self.file_explorer.file_system_model.rootPath()) / 'new folder'
         x = 1
         while folder_path.exists():
             folder_path = Path(folder_path.parent / f"new folder{x}")
             x += 1
         i = self.file_explorer.file_system_model.mkdir(self.file_explorer.rootIndex(), folder_path.name)
         self.file_explorer.edit(i)
     def new_project_command(self):
         self.status_bar.set_timed_message("Project functionality to be added...", 3000)
     def open_file_command(self):
-        new_file, _ = QFileDialog.getOpenFileName(self.window, "Pick A File", "", "All Files [*];;Python Files [*.py]")
-        if new_file == '':
+        file_name, filter_type = QFileDialog.getOpenFileName(
+            self.window, 
+            "Pick A File", 
+            "", 
+            "All Files (*);;Python Files (*.py);;JavaScript Files (*.js)"
+        )
+
+        if file_name:  # Check if a file was actually selected
+            path = Path(file_name)
+            self.window.grep_frame.grep_view.add_tab(self.window, path, False)
+        else:
             self.status_bar.set_timed_message("Open cancelled.", 2000)
-            return
-        path = Path(new_file)
-        self.window.add_tab(path)
     def open_folder_command(self):
         new_folder = QFileDialog.getExistingDirectory(self.window, "Pick A Folder", "")
         if new_folder:
             # Set the root path of the file explorer to the new folder and re-enable it
             self.file_explorer.set_root_path(new_folder)
             self.status_bar.set_timed_message(f"Changed folder to {new_folder}", 2000)
         else:
```

### Comparing `gs_edit-0.2.3/src/gsedit/popup.py` & `gs_edit-0.2.4/src/gsedit/popup.py`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.3/src/gsedit/res_src.py` & `gs_edit-0.2.4/src/gsedit/res_src.py`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.3/src/gsedit/sidebar.py` & `gs_edit-0.2.4/src/gsedit/tools.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,87 +1,62 @@
 from PyQt5.QtWidgets import *
 from PyQt5 import *
 from PyQt5.Qsci import *
 from PyQt5.QtGui import *
 from PyQt5.QtCore import *
-
 import os
 
-class Sidebar(QFrame):
-    def __init__(self, window) -> None:
-        super(Sidebar, self).__init__()
-        self.window = window
-        self.initialize_sidebar()
+from gsedit.file_explorer import FileExplorer, FileExplorerLayout
+from gsedit.grep import GrepLayout, Searchbar, GrepToggle, GrepResult
+from gsedit.grepgine import Grepgine
+
+class GeneralToolFrame(QFrame):
+    def __init__(self) -> None:
+        super(GeneralToolFrame, self).__init__()
+        self.initialize_frame(200, 400)
         self.refresh_style()
     
-    def initialize_sidebar(self):
-        self.setFrameShape(QFrame.StyledPanel)
+    def initialize_frame(self, minimum, maximum) -> QFrame:
+        self.setMaximumWidth(maximum)
+        self.setMinimumWidth(minimum)
+        self.setFrameShape(QFrame.NoFrame)
         self.setFrameShadow(QFrame.Plain)
-        self.setLayout(SidebarLayout(self.window))
+        self.setContentsMargins(0, 0, 0, 0)
 
     def refresh_style(self):
-        base_path = os.path.dirname(__file__)  
-        style_sheet_path = os.path.join(base_path, 'css', 'sidebar.qss')
+        base_path = os.path.dirname(__file__) 
+        style_sheet_path = os.path.join(base_path, 'css', 'tools.qss')
         with open(style_sheet_path, "r") as style_file:
-            self.setStyleSheet(style_file.read()) #collin smith
+            self.setStyleSheet(style_file.read())
 
-class SidebarLayout(QVBoxLayout):
+class FileExplorerFrame(GeneralToolFrame):
     def __init__(self, window) -> None:
-        super(SidebarLayout, self).__init__()
+        super(FileExplorerFrame, self).__init__()
         self.window = window
-        self.initialize_layout()
-        self.initialize_icons()
-    
-    def initialize_layout(self):
-        self.setContentsMargins(5, 10, 5, 0)
-        self.setSpacing(0)
-        self.setAlignment(Qt.AlignTop | Qt.AlignCenter)
-    
-    def initialize_icons(self):
-        folder_icon = self.tool_bar_icon("./src/gsedit/images/folder.svg",  "folder")
-        self.addWidget(folder_icon)
-        grep_icon = self.tool_bar_icon("./src/gsedit/images/grep.svg", "grep")
-        self.addWidget(grep_icon)
-
-    def tool_bar_icon(self, path, id):
-        label = ToolLabel(path, id, self.window)
-        return label
-
-class ToolLabel(QLabel):
-    def __init__(self, path, id, window) -> None:
-        super(ToolLabel, self).__init__()
-        self.path = path
-        self.id = id
+        self.file_explorer_layout = FileExplorerLayout()
+        self.file_explorer = FileExplorer(tab=self.window.tab, add_tab=self.window.grep_frame.grep_view.add_tab, window=self.window)
+        self.file_explorer_layout.addWidget(self.file_explorer)
+        self.setLayout(self.file_explorer_layout)
+
+class GrepFrame(GeneralToolFrame):
+    def __init__(self, window) -> None:
+        super(GrepFrame, self).__init__()
         self.window = window
-        self.initialize_label()
+        grep_layout = GrepLayout()
+        grep_result = Searchbar(self.window)
+        self.grep_box = GrepToggle(self.window)
+        self.grepgine = Grepgine()
+        self.grep_view = GrepResult(self.window)
+        self.grepgine.final_result.connect(self.grep_view.finish_grep)
+        grep_result.textChanged.connect(
+            lambda x: self.grepgine.modify(
+                x,
+                self.window.file_explorer_frame.file_explorer.file_system_model.rootDirectory().absolutePath(),
+                self.grep_box.isChecked()
+            )
+        )
+        grep_layout.addWidget(self.grep_box)
+        grep_layout.addWidget(grep_result)
+        grep_layout.addSpacerItem(QSpacerItem(4, 4, QSizePolicy.Minimum, QSizePolicy.Minimum))
+        grep_layout.addWidget(self.grep_view)
 
-    def initialize_label(self):
-        self.setPixmap(QPixmap(self.path).scaled(QSize(35, 35)))
-        self.setAlignment(Qt.AlignmentFlag.AlignTop)
-        self.setFont(self.window.window_font)
-        if(self.id == "folder"):
-            self.mousePressEvent = lambda e: self.toolbar_toggle(self.id)
-        elif(self.id == "grep"):
-            self.mousePressEvent = lambda e: self.toolbar_toggle(self.id)
-        self.enterEvent = self.change_cursor("pointer")
-        self.leaveEvent = self.change_cursor("arrow")
-    def change_cursor(self, name):
-        if name == "pointer":
-            self.window.setCursor(Qt.PointingHandCursor)
-        elif name == "arrow":
-            self.window.setCursor(Qt.ArrowCursor)
-    
-    def toolbar_toggle(self, tool):
-        if tool == "folder":
-            if self.window.current_tool != "folder":
-                self.window.horizontal_split.insertWidget(0, self.window.file_explorer_frame)
-        elif tool == "grep":
-            if self.window.current_tool != "grep":
-                self.window.horizontal_split.insertWidget(0, self.window.grep_frame)
-
-        if self.window.current_tool == tool:
-            temp_frame = self.window.horizontal_split.widget(0)
-            if temp_frame.isHidden():
-                temp_frame.show()
-            else:
-                temp_frame.hide()
-        self.window.current_tool = tool
+        self.setLayout(grep_layout)
```

### Comparing `gs_edit-0.2.3/src/gsedit/status_bar.py` & `gs_edit-0.2.4/src/gsedit/status_bar.py`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.3/src/gsedit/tab_bar.py` & `gs_edit-0.2.4/src/gsedit/tab_bar.py`

 * *Files identical despite different names*

### Comparing `gs_edit-0.2.3/src/gsedit/text_editor.py` & `gs_edit-0.2.4/src/gsedit/text_editor.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,32 +9,33 @@
 import pkgutil
 import keyword
 
 import gsedit.gsconfig
 
 from pathlib import Path
 
-from gsedit.language_lexer import PythonLexer, CLexer, JSONLexer, RustLexer, CppLexer
+from gsedit.language_lexer import JavaScriptLexer, PythonLexer, CLexer, JSONLexer, RustLexer, CppLexer
 from gsedit.code_completer import Completer
 
 
 if TYPE_CHECKING:
     from gsedit.main import MainWindow # prevents circular imports
 
 class TextEditor(QsciScintilla):
-    def __init__(self, window, parent = None, path = None, pyf=None, cf=None, jsonf=None, rustf=None, cppf=None):
+    def __init__(self, window, parent = None, path = None, pyf=None, cf=None, jsonf=None, rustf=None, cppf=None, jsf=None):
         super(TextEditor, self).__init__(parent)
         self.window = window
         self.path = path
         self.abs_path = self.path.absolute()
         self.pyf = pyf
         self.cf = cf
         self.jsonf = jsonf
         self.rustf = rustf
         self.cppf = cppf
+        self.jsf = jsf
         self.setUtf8(True)
 
         self.window_font = QFont("Fire Code")
         self.window_font.setPointSize(12)
 
         self.setFont(self.window_font)
         
@@ -94,21 +95,27 @@
             self.setLexer(self.lexer)
         elif self.cppf:
             self.lexer = CppLexer(self)
             self.lexer.setDefaultFont(self.window_font)
             self.api = QsciAPIs(self.lexer)
             self.code_completer = Completer(self.abs_path, self.api)
             self.setLexer(self.lexer)
+        elif self.jsf:
+            self.lexer = JavaScriptLexer(self)
+            self.lexer.setDefaultFont(self.window_font)
+            self.api = QsciAPIs(self.lexer)
+            self.code_completer = Completer(self.abs_path, self.api)
+            self.setLexer(self.lexer)
         else:
-            self.setPaper(QColor(gsconfig.get_color("primary-background")))
-            self.setColor(QColor(gsconfig.get_color("primary-text")))
+            self.setPaper(QColor(gsedit.gsconfig.get_color("primary-background")))
+            self.setColor(QColor(gsedit.gsconfig.get_color("primary-text")))
 
 
         self.setMarginType(0, QsciScintilla.NumberMargin)
-        self.setMarginWidth(0, "0000")
+        self.setMarginWidth(0, "000")
         self.setMarginsForegroundColor(QColor("white"))
         self.setMarginsBackgroundColor((QColor("#0C0C1A")))
         self.setMarginsFont(self.window_font)
     
     @property
     def unsaved_changes(self):
         return self._unsaved_changes
```

