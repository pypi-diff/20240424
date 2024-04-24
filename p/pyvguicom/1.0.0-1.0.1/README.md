# Comparing `tmp/pyvguicom-1.0.0.tar.gz` & `tmp/pyvguicom-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvguicom-1.0.0.tar", last modified: Wed Mar 13 17:24:15 2024, max compression
+gzip compressed data, was "pyvguicom-1.0.1.tar", last modified: Wed Apr 24 16:19:56 2024, max compression
```

## Comparing `pyvguicom-1.0.0.tar` & `pyvguicom-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-03-13 17:24:15.927513 pyvguicom-1.0.0/
--rw-r--r--   0 peterglen  (1000) users      (100)     2792 2024-03-13 17:24:15.927513 pyvguicom-1.0.0/PKG-INFO
--rw-rw-r--   0 peterglen  (1000) users      (100)     2377 2024-03-13 17:22:20.000000 pyvguicom-1.0.0/README.md
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-03-13 17:24:15.927513 pyvguicom-1.0.0/pyvguicom/
--rw-r--r--   0 peterglen  (1000) users      (100)        0 2023-09-14 20:07:28.000000 pyvguicom-1.0.0/pyvguicom/__init__.py
--rw-r--r--   0 peterglen  (1000) users      (100)     7530 2023-09-14 20:07:28.000000 pyvguicom-1.0.0/pyvguicom/browsewin.py
--rw-r--r--   0 peterglen  (1000) users      (100)    10064 2023-09-14 20:07:28.000000 pyvguicom-1.0.0/pyvguicom/htmledit.py
--rw-r--r--   0 peterglen  (1000) users      (100)    21912 2023-09-14 20:07:28.000000 pyvguicom-1.0.0/pyvguicom/pgbox.py
--rw-r--r--   0 peterglen  (1000) users      (100)     6700 2023-09-14 20:07:28.000000 pyvguicom-1.0.0/pyvguicom/pgbutt.py
--rw-r--r--   0 peterglen  (1000) users      (100)     4932 2023-09-14 20:07:28.000000 pyvguicom-1.0.0/pyvguicom/pgentry.py
--rw-r--r--   0 peterglen  (1000) users      (100)    40484 2023-09-14 20:07:28.000000 pyvguicom-1.0.0/pyvguicom/pggui.py
--rw-r--r--   0 peterglen  (1000) users      (100)    15446 2023-09-14 20:07:28.000000 pyvguicom-1.0.0/pyvguicom/pgsimp.py
--rw-r--r--   0 peterglen  (1000) users      (100)    29354 2023-09-14 20:07:28.000000 pyvguicom-1.0.0/pyvguicom/pgtextview.py
--rw-r--r--   0 peterglen  (1000) users      (100)    31741 2023-09-14 20:07:28.000000 pyvguicom-1.0.0/pyvguicom/pgutils.py
--rw-r--r--   0 peterglen  (1000) users      (100)    25820 2023-09-14 20:07:28.000000 pyvguicom-1.0.0/pyvguicom/pgwkit.py
--rw-r--r--   0 peterglen  (1000) users      (100)     1017 2023-09-14 20:07:28.000000 pyvguicom-1.0.0/pyvguicom/plug.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     9570 2024-03-13 16:30:39.000000 pyvguicom-1.0.0/pyvguicom/sutil.py
--rwxr-xr-x   0 peterglen  (1000) users      (100)     2800 2023-09-14 20:07:28.000000 pyvguicom-1.0.0/pyvguicom/testbutt.py
--rwxr-xr-x   0 peterglen  (1000) users      (100)     8947 2023-09-14 20:07:28.000000 pyvguicom-1.0.0/pyvguicom/testicons.py
--rwxr-xr-x   0 peterglen  (1000) users      (100)     3222 2023-09-14 20:07:28.000000 pyvguicom-1.0.0/pyvguicom/testnums.py
--rwxr-xr-x   0 peterglen  (1000) users      (100)     4058 2023-09-14 20:07:28.000000 pyvguicom-1.0.0/pyvguicom/testroot.py
--rwxr-xr-x   0 peterglen  (1000) users      (100)     2401 2023-09-14 20:07:28.000000 pyvguicom-1.0.0/pyvguicom/testsimple.py
--rwxr-xr-x   0 peterglen  (1000) users      (100)     7193 2023-09-14 20:07:28.000000 pyvguicom-1.0.0/pyvguicom/testtextv.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-03-13 17:24:15.927513 pyvguicom-1.0.0/pyvguicom.egg-info/
--rw-r--r--   0 peterglen  (1000) users      (100)     2792 2024-03-13 17:24:15.000000 pyvguicom-1.0.0/pyvguicom.egg-info/PKG-INFO
--rw-r--r--   0 peterglen  (1000) users      (100)      554 2024-03-13 17:24:15.000000 pyvguicom-1.0.0/pyvguicom.egg-info/SOURCES.txt
--rw-r--r--   0 peterglen  (1000) users      (100)        1 2024-03-13 17:24:15.000000 pyvguicom-1.0.0/pyvguicom.egg-info/dependency_links.txt
--rw-r--r--   0 peterglen  (1000) users      (100)       10 2024-03-13 17:24:15.000000 pyvguicom-1.0.0/pyvguicom.egg-info/top_level.txt
--rw-r--r--   0 peterglen  (1000) users      (100)       38 2024-03-13 17:24:15.927513 pyvguicom-1.0.0/setup.cfg
--rw-rw-r--   0 peterglen  (1000) users      (100)     1625 2024-03-13 17:23:14.000000 pyvguicom-1.0.0/setup.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-24 16:19:56.022504 pyvguicom-1.0.1/
+-rw-r--r--   0 peterglen  (1000) users      (100)     3109 2024-04-24 16:19:56.022504 pyvguicom-1.0.1/PKG-INFO
+-rw-rw-r--   0 peterglen  (1000) users      (100)     2377 2024-03-13 17:22:20.000000 pyvguicom-1.0.1/README.md
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-24 16:19:56.022504 pyvguicom-1.0.1/pyvguicom/
+-rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-24 07:51:41.000000 pyvguicom-1.0.1/pyvguicom/__init__.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     7530 2023-09-14 20:07:28.000000 pyvguicom-1.0.1/pyvguicom/browsewin.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     3693 2024-04-24 07:55:00.000000 pyvguicom-1.0.1/pyvguicom/custwidg.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    10064 2023-09-14 20:07:28.000000 pyvguicom-1.0.1/pyvguicom/htmledit.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    20271 2024-04-24 11:20:12.000000 pyvguicom-1.0.1/pyvguicom/pgbox.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     6723 2024-04-24 06:56:13.000000 pyvguicom-1.0.1/pyvguicom/pgbutt.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     7882 2024-04-24 11:13:26.000000 pyvguicom-1.0.1/pyvguicom/pgentry.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    43189 2024-04-24 13:33:48.000000 pyvguicom-1.0.1/pyvguicom/pggui.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    13185 2024-04-24 11:17:09.000000 pyvguicom-1.0.1/pyvguicom/pgsel.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     7628 2024-04-24 13:25:59.000000 pyvguicom-1.0.1/pyvguicom/pgsimp.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    29341 2024-04-24 07:00:30.000000 pyvguicom-1.0.1/pyvguicom/pgtextview.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    41430 2024-04-24 16:03:58.000000 pyvguicom-1.0.1/pyvguicom/pgutils.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    25820 2023-09-14 20:07:28.000000 pyvguicom-1.0.1/pyvguicom/pgwkit.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     1017 2023-09-14 20:07:28.000000 pyvguicom-1.0.1/pyvguicom/plug.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     2901 2024-04-24 11:14:35.000000 pyvguicom-1.0.1/pyvguicom/testbutt.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     1149 2024-04-24 07:56:07.000000 pyvguicom-1.0.1/pyvguicom/testcust.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     2658 2024-04-24 07:38:49.000000 pyvguicom-1.0.1/pyvguicom/testentry.py
+-rwxr-xr-x   0 peterglen  (1000) users      (100)     8947 2023-09-14 20:07:28.000000 pyvguicom-1.0.1/pyvguicom/testicons.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3018 2024-04-24 03:27:26.000000 pyvguicom-1.0.1/pyvguicom/testlettsel.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3213 2024-04-24 07:48:24.000000 pyvguicom-1.0.1/pyvguicom/testnums.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4082 2024-04-24 11:12:22.000000 pyvguicom-1.0.1/pyvguicom/testroot.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     2355 2024-04-24 11:18:03.000000 pyvguicom-1.0.1/pyvguicom/testsimple.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     7124 2024-04-24 07:02:31.000000 pyvguicom-1.0.1/pyvguicom/testtextv.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-24 16:19:56.022504 pyvguicom-1.0.1/pyvguicom.egg-info/
+-rw-r--r--   0 peterglen  (1000) users      (100)     3109 2024-04-24 16:19:56.000000 pyvguicom-1.0.1/pyvguicom.egg-info/PKG-INFO
+-rw-r--r--   0 peterglen  (1000) users      (100)      646 2024-04-24 16:19:56.000000 pyvguicom-1.0.1/pyvguicom.egg-info/SOURCES.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)        1 2024-04-24 16:19:56.000000 pyvguicom-1.0.1/pyvguicom.egg-info/dependency_links.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)       10 2024-04-24 16:19:56.000000 pyvguicom-1.0.1/pyvguicom.egg-info/top_level.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)       38 2024-04-24 16:19:56.022504 pyvguicom-1.0.1/setup.cfg
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1431 2024-04-24 16:19:44.000000 pyvguicom-1.0.1/setup.py
```

### Comparing `pyvguicom-1.0.0/PKG-INFO` & `pyvguicom-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 Metadata-Version: 2.1
 Name: pyvguicom
-Version: 1.0.0
+Version: 1.0.1
 Summary: High power secure server GUI utility helpers.
-Home-page: https://github.com/pglen/pyvserv
+Home-page: https://github.com/pglen/pyguicom.git
 Author: Peter Glen
 Author-email: peterglen99@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 6 - Mature
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: Python Software Foundation License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
 # pyvguicom  PyV GUI Common utilities
 
 ## Common GUI routines and classes
```

### Comparing `pyvguicom-1.0.0/README.md` & `pyvguicom-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.0.0/pyvguicom/browsewin.py` & `pyvguicom-1.0.1/pyvguicom/browsewin.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.0.0/pyvguicom/htmledit.py` & `pyvguicom-1.0.1/pyvguicom/htmledit.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.0.0/pyvguicom/pgbox.py` & `pyvguicom-1.0.1/pyvguicom/pgbox.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 #!/usr/bin/python
 
-from __future__ import absolute_import
-from __future__ import print_function
-
-import os, sys, getopt, signal, string, fnmatch, math
-import random, time, subprocess, traceback, glob
+import  sys
 
 import gi
 gi.require_version("Gtk", "3.0")
 gi.require_version('PangoCairo', '1.0')
 
 from gi.repository import Gtk
 from gi.repository import Gdk
-from gi.repository import GLib
 from gi.repository import GObject
 from gi.repository import Pango
 from gi.repository import PangoCairo
 
-import sutil
+import pgutils
 
-sys.path.append('..')
-import pycommon.pgutils
+'''  PgGui documentaation '''
 
+#sys.path.append('..')
+#import pycommon.pgutils
 
 box_testmode = False
 
 def str2rgb(col):
 
     #print("in", col)
     aa = int(col[1:3], base=16)
@@ -64,16 +60,17 @@
                     #self.height = bb
                     self.h = bb
                 else:
                     raise ValueError
                 idx += 1
         else:
             for aaa in rrr:
-                self.x = aaa[0]; self.y =  aaa[1]
-                self.w =  aaa[2];
+                self.x = aaa[0]
+                self.y =  aaa[1]
+                self.w =  aaa[2]
                 #self.width =  aaa[2];
                 self.h =  aaa[3]
                 #self.height =  aaa[3]
                 break
             pass
 
     # Make it smaller
@@ -133,55 +130,55 @@
 
         urx = self.x + self.w;      lry = self.y + self.h
         urx2 = rect2.x + rect2.w;   lry2 = rect2.y + rect2.h
         inter = 0
 
         # X intersect
         if rect2.x >= self.x and rect2.x <= urx:
-            inter += 1;
+            inter += 1
         # Y intersect
         if rect2.y >= self.y and rect2.y <= lry:
-            inter += 1;
+            inter += 1
 
         # X intersect rev
         if self.x >= rect2.x and self.x <= urx2:
-            inter += 1;
+            inter += 1
         # Y intersect rev
         if self.y >= rect2.y and self.y <= lry2:
-            inter += 1;
+            inter += 1
 
         #print("inter", inter, str(self), "->", str(rect2))
         return (inter >= 2, self.x)
 
     # I was too lazy to write it; Crappy Gdt rect kicked me to it
     def contain(self, rect2):
         #self.dump()
         #rect2.dump()
         inter = 0
         # X intersect
         if rect2.x >= self.x and rect2.x + rect2.w <= self.x + self.w:
-            inter += 1;
+            inter += 1
         # Y intersect
         if rect2.y >= self.y and rect2.y + rect2.h <= self.y + self.h:
-            inter += 1;
+            inter += 1
         #print("inter", inter)
         return (inter == 2, self.x)
 
     # Convert index to values
     def __getitem__(self, key):
         if key == 0:
             return self.x
         elif key == 1:
             return self.y
         elif key == 2:
             return self.w
         elif key == 3:
             return self.h
         else:
-            raise IndexError;
+            raise IndexError
 
     def dump(self):
         return (self.x, self.y, self.w, self.h)
 
     '''
     # This was killed in favour of self implemented Rectangle class
     def __getattr__(self, attr):
@@ -201,67 +198,14 @@
             super(Gdk.Rectangle, self).__setattr__(attr, val)
     '''
 
     def __str__(self):
         return "R: x=%d y=%d w=%d h=%d" % (self.x, self.y, self.w, self.h)
 
 # ------------------------------------------------------------------------
-# An N pixel horizontal spacer. Defaults to X pix
-
-class xSpacer(Gtk.HBox):
-
-    def __init__(self, sp = None):
-        GObject.GObject.__init__(self)
-        #self.pack_start()
-        if box_testmode:
-            col = pgutils.randcolstr(100, 200)
-            self.modify_bg(Gtk.StateType.NORMAL, Gdk.color_parse(col))
-        if sp == None:
-            sp = 6
-        self.set_size_request(sp, sp)
-
-# ------------------------------------------------------------------------
-# An N pixel spacer. Defaults to 1 char height / width
-
-class Spacer(Gtk.Label):
-
-    global box_testmode
-
-    def __init__(self, sp = 1, title=None, left=False, bottom=False, test=False):
-
-        GObject.GObject.__init__(self)
-
-        #sp *= 1000
-        #self.set_markup("<span  size=\"" + str(sp) + "\"> </span>")
-        #self.set_text(" " * sp)
-
-        if title:
-            self.set_text(title)
-        else:
-            self.set_text(" " * sp)
-
-        if left:
-            self.set_xalign(0)
-
-        if bottom:
-            self.set_yalign(1)
-
-        if test or box_testmode:
-            self.modify_bg(Gtk.StateType.NORMAL, Gdk.color_parse("#888888"))
-
-        #self.set_property("angle", 15)
-        #attr = self.get_property("attributes")
-        #attr2 = Pango.AttrList()
-        #print ("attr", dir(attr))
-        #attr.
-        #self.set_property("attributes", attr)
-        #self.set_property("label", "wtf")
-        #self.set_property("background-set", True)
-
-# ------------------------------------------------------------------------
 # This override covers / hides the complexity of the treeview and the
 # textlisbox did not have the needed detail
 
 class ListBox(Gtk.TreeView):
 
     def __init__(self, limit = -1, colname = ''):
 
@@ -317,65 +261,65 @@
 
     # Select Item. -1 for select none; Rase Valuerror for wrong index.
     def select(self, idx):
         ts = self.get_selection()
         if idx == -1:
             ts.unselect_all()
             return
-        iter = self.treestore.get_iter_first()
+        iterx = self.treestore.get_iter_first()
         for aa in range(idx):
-            iter = self.treestore.iter_next(iter)
-            if not iter:
+            iterx = self.treestore.iter_next(iter)
+            if not iterx:
                 break
-        if not iter:
+        if not iterx:
             pass
             #raise ValueError("Invalid selection index.")
-        ts.select_iter(iter)
+        ts.select_iter(iterx)
 
     # Return the number of list items
     def get_size(self):
         cnt = 0
-        iter = self.treestore.get_iter_first()
-        if not iter:
+        iterx = self.treestore.get_iter_first()
+        if not iterx:
             return cnt
         cnt = 1
         while True:
-            iter = self.treestore.iter_next(iter)
-            if not iter:
+            iterx = self.treestore.iter_next(iter)
+            if not iterx:
                 break
             cnt += 1
         return cnt
 
     def get_item(self, idx):
         cnt = 0; res = ""
-        iter = self.treestore.get_iter_first()
-        if not iter:
+        iterx = self.treestore.get_iter_first()
+        if not iterx:
             return ""
         cnt = 1
         while True:
-            iter = self.treestore.iter_next(iter)
-            if not iter:
+            iterx = self.treestore.iter_next(iter)
+            if not iterx:
                 break
             if cnt == idx:
-                res = self.treestore.get_value(iter, 0)
+                res = self.treestore.get_value(iterx, 0)
                 break
             cnt += 1
         return res
 
     def append(self, strx):
         if self.limit != -1:
             # count them
             cnt = self.get_size()
             #print("limiting cnt=", cnt, "limit=", self.limit)
             for aa in range(cnt - self.limit):
-                iter = self.treestore.get_iter_first()
-                if not iter:
+                iterx = self.treestore.get_iter_first()
+                if not iterx:
                     break
                 try:
-                    self.treestore.remove(iter)
+                    self.treestore.remove(iterx)
                 except:
                     print("except: treestore remove lim")
 
         last = self.treestore.append(None, [strx])
         self.set_cursor_on_cell(self.treestore.get_path(last), None, None, False)
 
     def get_text(self):
@@ -448,15 +392,15 @@
                 #print("Selected: name=%s" % (name))
 
             if self.callme:
                 try:
                     self.callme(name)
                 except:
                     print("Callback:", sys.exc_info())
-                    sutil.print_exception("callb")
+                    pgutils.print_exception("callb")
 
             else:
                 entry = combo.get_child()
                 name = entry.get_text()
                 #print("Entered: %s" % name)
 
         except:
@@ -481,47 +425,47 @@
 
     # --------------------------------------------------------------------
     def  sel_text(self, txt):
 
         #print("Sel combo text")
 
         model = self.get_model()
-        iter = model.get_iter_first()
-        if iter:
+        iterx = model.get_iter_first()
+        if iterx:
             cnt = 0
             while True:
 
-                #print("entry %d" % cnt, model[iter][0], txt)
-                if  model[iter][0] == txt:
-                    #print("Found %d" % cnt, model[iter][0])
-                    self.set_active_iter(iter)
+                #print("entry %d" % cnt, model[iterx][0], txt)
+                if  model[iterx][0] == txt:
+                    #print("Found %d" % cnt, model[iterx][0])
+                    self.set_active_iter(iterx)
                     break
 
-                iter = model.iter_next(iter)
-                if not iter:
+                iterx = model.iter_next(iterx)
+                if not iterx:
                     break
                 cnt += 1
 
     def     sel_first(self):
         model = self.get_model()
-        iter = model.get_iter_first()
-        self.set_active_iter(iter)
+        iterx = model.get_iter_first()
+        self.set_active_iter(iterx)
 
 # ------------------------------------------------------------------------
 # Gtk.TreeView simpler combo for color selection
 
 class   ColorRenderer(Gtk.CellRenderer):
 
     __gproperties__ = {
           'text' : (GObject.TYPE_STRING, 'text',
                     'string that represents the item',
-                    'hello', GObject.PARAM_READWRITE),
+                    'hello', GObject.ParamFlags.READWRITE),
           'bgcolor' : (GObject.TYPE_STRING, 'bgcolor',
                     'string that represents the RGB color',
-                    'white', GObject.PARAM_READWRITE),
+                    'white', GObject.ParamFlags.READWRITE),
           }
 
     def __init__(self):
         Gtk.CellRenderer.__init__(self)
         # Create placeholders
         self.text = "None"
         self.bgcolor = "None"
@@ -566,15 +510,15 @@
                 ddd.append(1)
             else:
                 ddd.append(0)
         ddd.append(1.)
         cr.set_source_rgba (*ddd)
 
         (pr, lr) = layout.get_extents()
-        xx = lr.width / Pango.SCALE; yy = lr.height / Pango.SCALE;
+        xx = lr.width / Pango.SCALE; yy = lr.height / Pango.SCALE
 
         cr.move_to((background_area.width - xx)/2, (background_area.height - yy)/2)
         PangoCairo.show_layout (cr, layout)
 
         cr.restore()
 
     def do_get_property(self, property):
@@ -616,18 +560,18 @@
         self.connect("changed", self.combo_changed)
         #self.connect("notify::popup-shown", self.combo_focus)
 
     def combo_focus(self, arg1, arg2):
         print("Focus", arg1, arg2)
 
     #def data_func(self, arg1, arg2, arg3, arg4):
-    '''def data_func(self, column, renderer, model, iter):
+    '''def data_func(self, column, renderer, model, iterx):
         #print("data_func called", arg1, arg2, arg3, arg4)
-        #print("data_func ", model, iter)
-        val = model.get_value(iter, 0)
+        #print("data_func ", model, iterx)
+        val = model.get_value(iterx, 0)
         #print("val", val)
         #renderer.set_property("cell-background", val)
         renderer.set_property("background", val)
         renderer.set_property("xpad", 0)
     '''
 
     def printdetails(self, arg, arg2, arg3):
@@ -681,34 +625,34 @@
 
     # --------------------------------------------------------------------
     def  sel_text(self, txt):
 
         #print("Sel combo text")
 
         model = self.get_model()
-        iter = model.get_iter_first()
-        if iter:
+        iterx = model.get_iter_first()
+        if iterx:
             cnt = 0
             while True:
 
-                #print("entry %d" % cnt, model[iter][0], txt)
-                if  model[iter][0] == txt:
-                    #print("Found %d" % cnt, model[iter][0])
-                    self.set_active_iter(iter)
+                #print("entry %d" % cnt, model[iterx][0], txt)
+                if  model[iterx][0] == txt:
+                    #print("Found %d" % cnt, model[iterx][0])
+                    self.set_active_iter(iterx)
                     break
 
-                iter = model.iter_next(iter)
-                if not iter:
+                iterx = model.iter_next(iterx)
+                if not iterx:
                     break
                 cnt += 1
 
     def     sel_first(self):
         model = self.get_model()
-        iter = model.get_iter_first()
-        self.set_active_iter(iter)
+        iterx = model.get_iter_first()
+        self.set_active_iter(iterx)
 
 
 # ------------------------------------------------------------------------
 # Added convenience methods
 
 class   xVBox(Gtk.VBox):
 
@@ -742,11 +686,8 @@
         self.pad = pad
 
     def pack(self, obj, expand = False, pad = 0):
         if pad == 0:
             pad = self.pad
         self.pack_start(obj, expand, expand, pad)
 
-
 # EOF
-
-
```

### Comparing `pyvguicom-1.0.0/pyvguicom/pgbutt.py` & `pyvguicom-1.0.1/pyvguicom/pgbutt.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from gi.repository import Pango
 from gi.repository import GObject
 
 gi.require_version('PangoCairo', '1.0')
 from gi.repository import PangoCairo
 
 import cairo
-from sutil import *
+from pgutils import *
 
 class smallbutt(Gtk.EventBox):
 
     __gsignals__ = {
     #"activate": (GObject.SIGNAL_RUN_FIRST, GObject.TYPE_NONE, () ),
     "pressed": (GObject.SIGNAL_RUN_FIRST, GObject.TYPE_NONE, () ),
     }
@@ -146,15 +146,16 @@
             self.mnem = False
 
         if self.omnem != self.mnem:
             self.omnem = self.mnem
             #print("changed to", self.mnem)
             self.queue_draw()
 
-        GLib.timeout_add(1000, self.stattime, self, 0)
+        #GLib.timeout_add(1000, self.stattime, self, 0)
+        return True
 
     def mactivate(self, *arg):
         #print("mactivate", arg)
         self.emit('pressed')
         return True
 
     def enter_label(self, arg, arg2):
```

### Comparing `pyvguicom-1.0.0/pyvguicom/pggui.py` & `pyvguicom-1.0.1/pyvguicom/pggui.py`

 * *Files 4% similar despite different names*

```diff
@@ -298,25 +298,32 @@
         #x = 0; y = 0; width = 10; height = 10
         #cr.save()
         #cr.translate(x + width / 2., y + height / 2.)
         #cr.scale(width / 2., height / 2.)
         #cr.restore()
 
         ccc = pgutils.str2float(self.color)
+
+        cr.set_source_rgba(ccc[0] * 0.5, ccc[1] * 0.5, ccc[2] * 0.5)
+        cr.arc(rect.width/2, rect.height/2, rect.width / 2. * .85, 0., 2 * math.pi)
+        cr.fill()
+
         cr.set_source_rgba(ccc[0] * 0.7, ccc[1] * 0.7, ccc[2] * 0.7)
         cr.arc(rect.width/2, rect.height/2., rect.width/2., 0., 2 * math.pi)
         cr.fill()
 
         cr.set_source_rgba(ccc[0], ccc[1], ccc[2])
-        cr.arc(rect.width/2, rect.height/2, rect.width / 2. * .8, 0., 2 * math.pi)
+        cr.arc(rect.width/2, rect.height/2, rect.width / 2. * .7, 0., 2 * math.pi)
         cr.fill()
 
         # Reflection on the r
-        cr.set_source_rgba(ccc[0], ccc[1] + 0.51, ccc[2])
-        cr.arc(rect.width/2+1, rect.height/2, rect.width / 2. * .2, 0., 2 * math.pi)
+        cdx = 0.2
+        colx = [ min(1, ccc[0] + cdx), min(1, ccc[1] + cdx), min(1, ccc[2] + cdx), ]
+        cr.set_source_rgba(*colx)
+        cr.arc(rect.width/2+1, rect.height/2, rect.width / 2. * .3, 0., 2 * math.pi)
         cr.fill()
 
 # ------------------------------------------------------------------------
 
 class MenuButt(Gtk.DrawingArea):
 
     def __init__(self, menarr, callb, tooltip = "Menu", size = 20, border = 2):
@@ -651,23 +658,68 @@
 
 def set_testmode(flag):
     global gui_testmode
     gui_testmode = flag
 
 # ------------------------------------------------------------------------
 # An N pixel horizontal spacer. Defaults to X pix  get_center
+#
+#def hspacer(hbox, xstr = "    ", expand = False):
+#    lab = Gtk.Label(label=xstr)
+#    hbox.pack_start(lab, expand, 0, 0)
+#
+#def vspacer(vbox, xstr = "     ", expand = False):
+#    lab = Gtk.Label(label=xstr)
+#    vbox.pack_start(lab, expand , 0, 0)
+#def vspacer(sp = 8):
+#    lab = Gtk.VBox()
+#    lab.set_size_request(sp, sp)
+#
+#    if gui_testmode:
+#        lab.override_background_color(
+#                    Gtk.StateFlags.NORMAL, Gdk.RGBA(1, .5, .5) )
+#    return lab
+
+# ------------------------------------------------------------------------
+# An N pixel spacer. Defaults to 1 char height / width
+
+class Spacer(Gtk.Label):
+
+    global box_testmode
+
+    def __init__(self, sp = 1, title=None, left=False, bottom=False, test=False):
+
+        GObject.GObject.__init__(self)
+
+        #sp *= 1000
+        #self.set_markup("<span  size=\"" + str(sp) + "\"> </span>")
+        #self.set_text(" " * sp)
+
+        if title:
+            self.set_text(title)
+        else:
+            self.set_text(" " * sp)
+
+        if left:
+            self.set_xalign(0)
+
+        if bottom:
+            self.set_yalign(1)
 
-def vspacer(sp = 8):
-    lab = Gtk.VBox()
-    lab.set_size_request(sp, sp)
-
-    if gui_testmode:
-        lab.override_background_color(
-                    Gtk.StateFlags.NORMAL, Gdk.RGBA(1, .5, .5) )
-    return lab
+        if test or box_testmode:
+            self.modify_bg(Gtk.StateType.NORMAL, Gdk.color_parse("#888888"))
+
+        #self.set_property("angle", 15)
+        #attr = self.get_property("attributes")
+        #attr2 = Pango.AttrList()
+        #print ("attr", dir(attr))
+        #attr.
+        #self.set_property("attributes", attr)
+        #self.set_property("label", "wtf")
+        #self.set_property("background-set", True)
 
 # ------------------------------------------------------------------------
 # An N pixel horizontal spacer. Defaults to X pix  get_center
 
 class xSpacer(Gtk.HBox):
 
     def __init__(self, sp = None):
@@ -676,14 +728,28 @@
         if gui_testmode:
             col = randcolstr(100, 200)
             self.modify_bg(Gtk.StateType.NORMAL, Gdk.color_parse(col))
         if sp == None:
             sp = 6
         self.set_size_request(sp, sp)
 
+# An N pixel vertical spacer. Defaults to X pix  get_center
+
+class ySpacer(Gtk.VBox):
+
+    def __init__(self, sp = None):
+        GObject.GObject.__init__(self)
+        #self.pack_start()
+        if gui_testmode:
+            col = randcolstr(100, 200)
+            self.modify_bg(Gtk.StateType.NORMAL, Gdk.color_parse(col))
+        if sp == None:
+            sp = 6
+        self.set_size_request(sp, sp)
+
 # ------------------------------------------------------------------------
 # An N pixel spacer. Defaults to 1 char height / width
 
 class Spacer(Gtk.Label):
 
     global gui_testmode
 
@@ -695,21 +761,18 @@
         #self.set_markup("<span  size=\"" + str(sp) + "\"> </span>")
         #self.set_text(" " * sp)
 
         if title:
             self.set_text(title)
         else:
             self.set_text(" " * sp)
-
         if left:
             self.set_xalign(0)
-
         if bottom:
             self.set_yalign(1)
-
         if test or gui_testmode:
             self.modify_bg(Gtk.StateType.NORMAL, Gdk.color_parse("#888888"))
 
         #self.set_property("angle", 15)
         #attr = self.get_property("attributes")
         #attr2 = Pango.AttrList()
         #print ("attr", dir(attr))
@@ -825,15 +888,14 @@
     def get_text(self):
         for aa in (self.buttons):
             if aa.get_active():
                 return aa.get_label()
         # Nothing selected ... empty str
         return ""
 
-
 # Bug fix in Gtk
 
 class   SeparatorMenuItem(Gtk.SeparatorMenuItem):
 
     def __init__(self):
         Gtk.SeparatorMenuItem.__init__(self);
         self.show()
@@ -1313,14 +1375,37 @@
 
     def clicked(self, arg1):
         pass
         #print("clicked", arg1)
         #if self.callme:
         #    self.callme(arg1)
 
+
+def message(msg):
+    dialog = Gtk.MessageDialog(None, Gtk.DialogFlags.DESTROY_WITH_PARENT,
+        Gtk.MessageType.INFO, Gtk.ButtonsType.CLOSE, text=msg)
+
+    #    'Action: "%s" of type "%s"' % (action.get_name(), type(action)))
+
+    # Close dialog on user response
+    dialog.connect ("response", lambda d, r: d.destroy())
+    return dialog.run()
+
+def yesno(msg):
+    dialog = Gtk.MessageDialog(None, Gtk.DialogFlags.DESTROY_WITH_PARENT,
+        Gtk.MessageType.INFO, Gtk.ButtonsType.YES_NO, text=msg)
+
+    #    'Action: "%s" of type "%s"' % (action.get_name(), type(action)))
+
+    # Close dialog on user response
+    #dialog.connect ("response", lambda d, r: d.destroy())
+    ret = dialog.run()
+    dialog.destroy()
+    return  ret
+
 # ------------------------------------------------------------------------
 # Highlite test items
 
 def set_gui_testmode(flag):
     global gui_testmode
     gui_testmode = flag
```

### Comparing `pyvguicom-1.0.0/pyvguicom/pgtextview.py` & `pyvguicom-1.0.1/pyvguicom/pgtextview.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from gi.repository import Gtk
 from gi.repository import Gdk
 from gi.repository import GLib
 from gi.repository import GObject
 from gi.repository import Pango
 
 import pgbox
-import sutil
 
 # Colors for editor selection. Use X11 color names.
 
 font_colors =   \
         (
             # Color name; RGBA for display
             ("Black",       "#000000ff"),  ("White",       "#ffffffff"),
```

### Comparing `pyvguicom-1.0.0/pyvguicom/pgutils.py` & `pyvguicom-1.0.1/pyvguicom/pgutils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,65 +1,50 @@
 #!/usr/bin/python
 
-from __future__ import absolute_import
-from __future__ import print_function
+# pylint: disable=C0103
+# pylint: disable=C0209
+# pylint: disable=C0321
 
-import os, sys, getopt, signal, string, fnmatch, math, warnings
-import random, time, subprocess, traceback, glob, stat
+import os, sys, getopt, string,  math, warnings
+import random, time, traceback, stat
+import platform
 
 if sys.version_info.major < 3:
     pass
 else:
     import inspect
     if inspect.isbuiltin(time.process_time):
         time.clock = time.process_time
 
+''' General utility fiunctions '''
+
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk
 from gi.repository import Gdk
-from gi.repository import GLib
 from gi.repository import GObject
-from gi.repository import Pango
 
 # Add the new line twice for more balaced string
 
 allcr =    " " + "\r" + "\n" + \
             "\r" + "\n"
 
                    #string.punctuation +
 
 allstr =    " " + \
             string.ascii_lowercase +  string.ascii_uppercase +  \
                 string.digits
 
 allasc =      string.ascii_lowercase +  string.ascii_uppercase +  \
                 string.digits + "_"
-
 alllett =      string.ascii_lowercase +  string.ascii_uppercase
-
-
 testmode = 0
 
 # -----------------------------------------------------------------------
 # Sleep just a little, but allow the system to breed
-#
-#def  usleep2(msec):
-#
-#    got_clock = time.clock() + float(msec) / 1000
-#    #print( got_clock)
-#    while True:
-#        if time.clock() > got_clock:
-#            break
-#        #print ("Sleeping")
-#        Gtk.main_iteration_do(False)
-#
-
-# -----------------------------------------------------------------------
-# Sleep just a little, but allow the system to breed
 
 def  usleep2(msec):
 
     if sys.version_info[0] < 3 or \
         (sys.version_info[0] == 3 and sys.version_info[1] < 3):
         timefunc = time.clock
     else:
@@ -74,91 +59,75 @@
         Gtk.main_iteration_do(False)
 
 # -----------------------------------------------------------------------
 # Pull up a message box
 
 def message2(strx, title = "Dialog", parent=None):
 
-        dialog = Gtk.MessageDialog()
-
-        # Close dialog on user response
-        dialog.add_button("Close", Gtk.ButtonsType.CLOSE)
-
-        if title:
-            dialog.set_title(title)
-
-        #box = dialog.get_content_area()
-        #box.add(Gtk.Label(strx))
-
-        dialog.set_markup(strx)
-
-        if parent:
-            dialog.set_transient_for(parent)
-
-        dialog.connect ("response", lambda d, r: d.destroy())
-        dialog.show_all()
-
+    dialog = Gtk.MessageDialog()
+    # Close dialog on user response
+    dialog.add_button("Close", Gtk.ButtonsType.CLOSE)
+    if title:
+        dialog.set_title(title)
+    #box = dialog.get_content_area()
+    #box.add(Gtk.Label(strx))
+    dialog.set_markup(strx)
+    if parent:
+        dialog.set_transient_for(parent)
+    dialog.connect ("response", lambda d, r: d.destroy())
+    dialog.show_all()
 
 def yes_no2(message, title = "Question", parent=None):
 
-        dialog = Gtk.MessageDialog()
-
-        if title:
-            dialog.set_title(title)
-
-        dialog.add_button("_Yes", Gtk.ResponseType.YES)
-        dialog.add_button("_No", Gtk.ResponseType.NO)
-
-        dialog.set_markup(message)
-
-        img = Gtk.Image.new_from_stock(Gtk.STOCK_DIALOG_QUESTION, Gtk.IconSize.DIALOG)
-        dialog.set_image(img)
-
-        if parent:
-            dialog.set_transient_for(parent)
-
-        dialog.connect("key-press-event", yn_key, 0)
-
-        #dialog.connect ("response", lambda d, r: d.destroy())
-
-        dialog.show_all()
-        response = dialog.run()
-        dialog.destroy()
+    dialog = Gtk.MessageDialog()
+    if title:
+        dialog.set_title(title)
+    dialog.add_button("_Yes", Gtk.ResponseType.YES)
+    dialog.add_button("_No", Gtk.ResponseType.NO)
+    dialog.set_markup(message)
+    img = Gtk.Image.new_from_stock(Gtk.STOCK_DIALOG_QUESTION, Gtk.IconSize.DIALOG)
+    dialog.set_image(img)
+    if parent:
+        dialog.set_transient_for(parent)
+    dialog.connect("key-press-event", yn_key, 0)
+    #dialog.connect ("response", lambda d, r: d.destroy())
+    dialog.show_all()
+    response = dialog.run()
+    dialog.destroy()
 
-        return response
+    return response
 
 # ------------------------------------------------------------------------
 # Do dialog
 
-def yes_no_cancel2(message, title = "Question", cancel = True, parent=None):
+def yes_no_cancel2(message, title = "Question", cancel = True):
 
     warnings.simplefilter("ignore")
 
     dialog = Gtk.Dialog(title,
                    None,
                    Gtk.DialogFlags.MODAL | Gtk.DialogFlags.DESTROY_WITH_PARENT)
 
     dialog.set_default_response(Gtk.ResponseType.YES)
     dialog.set_position(Gtk.WindowPosition.CENTER)
-    #dialog.set_transient_for(pedconfig.conf.pedwin.mywin)
 
     sp = "     "
-    label = Gtk.Label(message);
+    label = Gtk.Label(message)
     label2 = Gtk.Label(sp);      label3 = Gtk.Label(sp)
     label2a = Gtk.Label(sp);     label3a = Gtk.Label(sp)
 
-    hbox = Gtk.HBox() ;
+    hbox = Gtk.HBox()
 
-    hbox.pack_start(label2, 0, 0, 0);
-    hbox.pack_start(label, 1, 1, 0);
+    hbox.pack_start(label2, 0, 0, 0)
+    hbox.pack_start(label, 1, 1, 0)
     hbox.pack_start(label3, 0, 0, 0)
 
-    dialog.vbox.pack_start(label2a, 0, 0, 0);
+    dialog.vbox.pack_start(label2a, 0, 0, 0)
     dialog.vbox.pack_start(hbox, 0, 0, 0)
-    dialog.vbox.pack_start(label3a, 0, 0, 0);
+    dialog.vbox.pack_start(label3a, 0, 0, 0)
 
     dialog.add_button("_Yes", Gtk.ResponseType.YES)
     dialog.add_button("_No", Gtk.ResponseType.NO)
 
     if cancel:
         dialog.add_button("_Cancel", Gtk.ResponseType.CANCEL)
 
@@ -338,15 +307,15 @@
     return stry
 
 def clean_str2(strx):
     stry = ""
     skip = False
     for aa in range(len(strx)):
         if skip:
-            skip = False;
+            skip = False
             continue
         if strx[aa] == '\\' and strx[aa+1] == 'r':
             skip = True
         if strx[aa] == '\\' and strx[aa+1] == 'n':
             skip = True
         if strx[aa] == '\\' and strx[aa+1] == '0':
             skip = True
@@ -557,15 +526,15 @@
 
     while True:
         if pos >= lenx:
             break
 
         chh = strx[pos]
 
-        if(chh == '\\'):
+        if chh == '\\':
             #print "backslash", strx[pos:]
             pos2 = pos + 1; strx2 = ""
             while True:
                 if pos2 >= lenx:
                     # See if we accumulated anything
                     if strx2 != "":
                         xtab.append(oct2int(strx2))
@@ -656,66 +625,14 @@
     except:
         return False
 
     if stat.S_ISREG(ss[stat.ST_MODE]):
         return True
     return False
 
-
-'''
-# Append to log
-def logentry(kind, startt, fname):
-    logfname = "account.txt"
-    logfile = pedconfig.conf.log_dir + "/" + logfname
-    try:
-        fp = open(logfile, "a+")
-    except:
-        try:
-            fp = open(logfile, "w+")
-            fp.seek(0, os.SEEK_END);
-        except:
-            print("Cannot open/create log file", logfile)
-            return
-
-    log_clock = time.time()
-
-    print("Action:", "%s %s" % (kind, os.path.realpath(fname)), file=fp)
-    print("On:", time.ctime(log_clock), file=fp)
-    print("Delta:", "%.0f" % (log_clock - startt), file=fp)
-    print("Date:", "%.0f %s %s\n" % \
-                        (log_clock, os.path.basename(fname), kind.split()[0]), file=fp)
-    fp.close()
-
-# Append to timesheet
-def timesheet(kind, startt, endd):
-
-    logfname = "timesheet.txt"
-    logfile = pedconfig.conf.log_dir + "/" + logfname
-    try:
-        fp = open(logfile, "a+")
-    except:
-        try:
-            fp = open(logfile, "w+")
-            fp.seek(0, os.SEEK_END);
-        except:
-            print("Cannot open/create log file", logfile)
-            return
-
-    log_clock = time.time()
-
-    print("Action:", "%s" % (kind), file=fp)
-    print("On:", time.ctime(log_clock), file=fp)
-    if endd:
-        td = endd - startt
-        print("Time diff:", "%.0f %d:%d" % (td, td / 3600, (td % 3600) / 60), file=fp)
-
-    print(file=fp)
-    fp.close()
-'''
-
 def put_exception2_old(xstr):
 
     cumm = xstr + " "
     a,b,c = sys.exc_info()
     if a != None:
         cumm += str(a) + " " + str(b) + "\n"
         try:
@@ -752,15 +669,15 @@
     xlen = len(strx)
     while True:
         if idx >= xlen: break
         chh = strx[idx]
         if  chh == "\t":
             # Generate string
             spaces = tabstop - (cnt % tabstop)
-            ttt = "";
+            ttt = ""
             for aa in range(spaces):
                 ttt += " "
             res += ttt
             cnt += spaces
         else:
             cnt += 1
             res += chh
@@ -770,31 +687,29 @@
 # ------------------------------------------------------------------------
 # Get am pm version of a number
 
 def ampmstr(bb):
 
     dd = "AM"
     if bb == 12:
-       dd = "PM"
+        dd = "PM"
     elif bb > 12:
         bb -= 12
         dd = "PM"
-
     return "%02d %s" % (bb, dd)
 
-
 # It's totally optional to do this, you could just manually insert icons
 # and have them not be themeable, especially if you never expect people
 # to theme your app.
 
 def register_stock_icons():
     ''' This function registers our custom toolbar icons, so they
         can be themed.
     '''
-    items = [('demo-gtk-logo', '_GTK!', 0, 0, '')]
+    #items = [('demo-gtk-logo', '_GTK!', 0, 0, '')]
     # Register our stock items
     #Gtk.stock_add(items)
 
     # Add our custom icon factory to the list of defaults
     factory = Gtk.IconFactory()
     factory.add_default()
 
@@ -823,18 +738,14 @@
             transparent = xbuf.add_alpha(True, chr(255), chr(255),chr(255))
             icon_set = Gtk.IconSet(transparent)
             factory.add('demo-gtk-logo', icon_set)
 
         except GObject.GError as error:
             print('failed to load GTK logo for toolbar')
 
-
-if __name__ == '__main__':
-    print("This file was not meant to run directly")
-
 # ------------------------------------------------------------------------
 # Let the higher level deal with errors.
 
 def  readfile(strx, sep = None):
 
     text = []
 
@@ -871,16 +782,16 @@
 
     # Clean out spuriously occurring \r and \n
     # Example: ST Microelectronics Makefiles
 
     text = []
     for aa in text2:
         #print("'%s\n" % aa)
-        bb = aa.replace("\r", "");
-        cc = bb.replace("\n", "");
+        bb = aa.replace("\r", "")
+        cc = bb.replace("\n", "")
         text.append(cc)
     #text2 = []
 
     return text
 
 # ------------------------------------------------------------------------
 # Handle command line. Interpret optarray and decorate the class
@@ -947,27 +858,29 @@
                    Gtk.DialogFlags.MODAL | Gtk.DialogFlags.DESTROY_WITH_PARENT)
 
     dialog.set_default_response(Gtk.ResponseType.YES)
     dialog.set_position(Gtk.WindowPosition.CENTER)
     #dialog.set_transient_for(pedconfig.conf.pedwin.mywin)
 
     sp = "     "
-    label = Gtk.Label(message);
-    label2 = Gtk.Label(sp);      label3 = Gtk.Label(sp)
-    label2a = Gtk.Label(sp);     label3a = Gtk.Label(sp)
+    label = Gtk.Label(message)
+    label2 = Gtk.Label(sp)
+    label3 = Gtk.Label(sp)
+    label2a = Gtk.Label(sp)
+    label3a = Gtk.Label(sp)
 
-    hbox = Gtk.HBox() ;
+    hbox = Gtk.HBox()
 
-    hbox.pack_start(label2, 0, 0, 0);
-    hbox.pack_start(label, 1, 1, 0);
+    hbox.pack_start(label2, 0, 0, 0)
+    hbox.pack_start(label, 1, 1, 0)
     hbox.pack_start(label3, 0, 0, 0)
 
-    dialog.vbox.pack_start(label2a, 0, 0, 0);
+    dialog.vbox.pack_start(label2a, 0, 0, 0)
     dialog.vbox.pack_start(hbox, 0, 0, 0)
-    dialog.vbox.pack_start(label3a, 0, 0, 0);
+    dialog.vbox.pack_start(label3a, 0, 0, 0)
 
     dialog.add_button("_Yes", Gtk.ResponseType.YES)
     dialog.add_button("_No", Gtk.ResponseType.NO)
 
     if cancel:
         dialog.add_button("_Cancel", Gtk.ResponseType.CANCEL)
 
@@ -1001,25 +914,22 @@
         win.response(Gtk.ResponseType.NO)
 
     if cancel:
         if event.keyval == Gdk.KEY_c or \
             event.keyval == Gdk.KEY_C:
             win.response(Gtk.ResponseType.CANCEL)
 
-# ------------------------------------------------------------------------
-# Show About dialog:
-
-import platform
+def  about2(self2):
 
-def  about(self2):
+    ''' Show About dialog: '''
 
     dialog = Gtk.AboutDialog()
     dialog.set_name(pedconfig.conf.progname +  " - Python Editor ")
 
-    dialog.set_version(str(pedconfig.conf.version));
+    dialog.set_version(str(pedconfig.conf.version))
     gver = (Gtk.get_major_version(), \
                         Gtk.get_minor_version(), \
                             Gtk.get_micro_version())
 
     dialog.set_position(Gtk.WindowPosition.CENTER)
     dialog.set_transient_for(pedconfig.conf.pedwin.mywin)
 
@@ -1035,29 +945,29 @@
         "\nRunning PyGtk %d.%d.%d" % vvv +\
         "\non GTK %d.%d.%d\n" % gver +\
         "\nRunning Python %s" % platform.python_version() +\
         "\non %s %s\n" % (platform.system(), platform.release()) +\
         "\nPyedPro Build Date: %s\n" % pedconfig.conf.build_date +\
         "Exe Path:\n%s\n" % os.path.realpath(ddd)
 
-    dialog.set_comments(comm);
+    dialog.set_comments(comm)
     dialog.set_copyright(pedconfig.conf.progname + " Created by Peter Glen.\n"
                           "Project is in the Public Domain.")
     dialog.set_program_name(pedconfig.conf.progname)
     img_dir = os.path.join(os.path.dirname(__file__), 'images')
     #img_path = os.path.join(img_dir, 'gtk-logo-rgb.gif')
     img_path = os.path.join(img_dir, 'pyedpro.png')
 
     try:
         pixbuf = GdkPixbuf.Pixbuf.new_from_file(img_path)
         #print "loaded pixbuf"
         dialog.set_logo(pixbuf)
 
     except:
-        print("Cannot load logo for about dialog", img_path);
+        print("Cannot load logo for about dialog", img_path)
         print(sys.exc_info())
 
     #dialog.set_website("")
 
     ## Close dialog on user response
     dialog.connect ("response", lambda d, r: d.destroy())
     dialog.connect("key-press-event", about_key)
@@ -1070,15 +980,15 @@
         if event.keyval == Gdk.KEY_x or event.keyval == Gdk.KEY_X:
             if event.state & Gdk.ModifierType.MOD1_MASK:
                 win.destroy()
 
 # ------------------------------------------------------------------------
 # Show a regular message:
 
-def message(strx, title = None):
+def message3(strx, title = None):
 
     #print("called: message()", strx)
 
     icon = Gtk.STOCK_INFO
     dialog = Gtk.MessageDialog(buttons=Gtk.ButtonsType.CLOSE,
                                message_type=Gtk.MessageType.INFO)
 
@@ -1094,10 +1004,438 @@
     dialog.set_position(Gtk.WindowPosition.CENTER)
 
     # Close dialog on user response
     dialog.connect("response", lambda d, r: d.destroy())
     dialog.show()
     dialog.run()
 
-# EOF
+# -----------------------------------------------------------------------
+# Call func with all processes, func called with stat as its argument
+# Function may return True to stop iteration
+
+def withps(func, opt = None):
+
+    ret = False
+    dl = os.listdir("/proc")
+    for aa in dl:
+        fname = "/proc/" + aa + "/stat"
+        if os.path.isfile(fname):
+            ff = open(fname, "r").read().split()
+            ret = func(ff, opt)
+        if ret:
+            break
+    return ret
+
+# ------------------------------------------------------------------------
+# Find
+
+def find(self):
+
+    head = "Find in text"
+
+    dialog = Gtk.Dialog(head,
+                   None,
+                   Gtk.DIALOG_MODAL | Gtk.DIALOG_DESTROY_WITH_PARENT,
+                   (Gtk.STOCK_CANCEL, Gtk.RESPONSE_REJECT,
+                    Gtk.STOCK_OK, Gtk.RESPONSE_ACCEPT))
+    dialog.set_default_response(Gtk.RESPONSE_ACCEPT)
+
+    try:
+        dialog.set_icon_from_file("epub.png")
+    except:
+        print ("Cannot load find dialog icon", sys.exc_info())
+
+    self.dialog = dialog
+
+    label3 = Gtk.Label("   ");  label4 = Gtk.Label("   ")
+    label5 = Gtk.Label("   ");  label6 = Gtk.Label("   ")
+    label7 = Gtk.Label("   ");  label8 = Gtk.Label("   ")
+
+    warnings.simplefilter("ignore")
+    entry = Gtk.Entry()
+    warnings.simplefilter("default")
+    entry.set_text(self.oldfind)
+
+    entry.set_activates_default(True)
+
+    dialog.vbox.pack_start(label4)
+
+    hbox2 = Gtk.HBox()
+    hbox2.pack_start(label6, False)
+    hbox2.pack_start(entry)
+    hbox2.pack_start(label7, False)
+
+    dialog.vbox.pack_start(hbox2)
+
+    dialog.checkbox = Gtk.CheckButton("Search _Backwards")
+    dialog.checkbox2 = Gtk.CheckButton("Case In_sensitive")
+    dialog.vbox.pack_start(label5)
+
+    hbox = Gtk.HBox()
+    #hbox.pack_start(label1);  hbox.pack_start(dialog.checkbox)
+    #hbox.pack_start(label2);  hbox.pack_start(dialog.checkbox2)
+    hbox.pack_start(label3)
+    dialog.vbox.pack_start(hbox)
+    dialog.vbox.pack_start(label8)
+
+    label32 = Gtk.Label("   ")
+    hbox4 = Gtk.HBox()
+
+    hbox4.pack_start(label32)
+    dialog.vbox.pack_start(hbox4)
+
+    dialog.show_all()
+    response = dialog.run()
+    self.srctxt = entry.get_text()
+
+    dialog.destroy()
+
+    if response != Gtk.RESPONSE_ACCEPT:
+        return None
+
+    return self.srctxt, dialog.checkbox.get_active(), \
+                dialog.checkbox2.get_active()
+
+disp = Gdk.Display.get_default()
+scr = disp.get_default_screen()
+
+#print( "num_mon",  scr.get_n_monitors()    )
+#for aa in range(scr.get_n_monitors()):
+#    print( "mon", aa, scr.get_monitor_geometry(aa);)
+
+# ------------------------------------------------------------------------
+# Get current screen (monitor) width and height
+
+def get_screen_wh():
+
+    ptr = disp.get_pointer()
+    mon = scr.get_monitor_at_point(ptr[1], ptr[2])
+    geo = scr.get_monitor_geometry(mon)
+    www = geo.width; hhh = geo.height
+    if www == 0 or hhh == 0:
+        www = Gdk.get_screen_width()
+        hhh = Gdk.get_screen_height()
+    return www, hhh
+
+# ------------------------------------------------------------------------
+# Get current screen (monitor) upper left corner xx / yy
+
+def get_screen_xy():
+
+    ptr = disp.get_pointer()
+    mon = scr.get_monitor_at_point(ptr[1], ptr[2])
+    geo = scr.get_monitor_geometry(mon)
+    return geo.x, geo.y
+
+# ------------------------------------------------------------------------
+# Print( an exception as the system would print it)
+
+def print_exception(xstr):
+    cumm = xstr + " "
+    a,b,c = sys.exc_info()
+    if a != None:
+        cumm += str(a) + " " + str(b) + "\n"
+        try:
+            #cumm += str(traceback.format_tb(c, 10))
+            ttt = traceback.extract_tb(c)
+            for aa in ttt:
+                cumm += "File: " + os.path.basename(aa[0]) + \
+                        " Line: " + str(aa[1]) + "\n" +  \
+                    "   Context: " + aa[2] + " -> " + aa[3] + "\n"
+        except:
+            print("Could not print trace stack. ", sys.exc_info())
+    print( cumm)
 
 
+# ------------------------------------------------------------------------
+# Show a regular message:
+
+def message(strx, parent = None, title = None, icon = Gtk.MessageType.INFO):
+
+    dialog = Gtk.MessageDialog(parent, Gtk.DialogFlags.DESTROY_WITH_PARENT,
+        icon, Gtk.ButtonsType.CLOSE, strx)
+
+    dialog.set_modal(True)
+
+    if title:
+        dialog.set_title(title)
+    else:
+        dialog.set_title("DBGui Message")
+
+    # Close dialog on user response
+    dialog.connect("response", lambda d, r: d.destroy())
+    dialog.show()
+
+# -----------------------------------------------------------------------
+# Sleep just a little, but allow the system to breed
+
+def  usleep(msec):
+
+    if sys.version_info[0] < 3 or \
+        (sys.version_info[0] == 3 and sys.version_info[1] < 3):
+        timefunc = time.clock
+    else:
+        timefunc = time.process_time
+
+    got_clock = timefunc() + float(msec) / 1000
+    #print( got_clock)
+    while True:
+        if timefunc() > got_clock:
+            break
+        #print ("Sleeping")
+        Gtk.main_iteration_do(False)
+
+# ------------------------------------------------------------------------
+# Create temporary file, return name. Empty string ("") if error.
+
+def tmpname(indir, template):
+
+    fname = ""
+    if not os.access(indir, os.W_OK):
+        print( "Cannot access ", indir)
+        return fname
+
+    cnt = 1
+    while True:
+        tmp = indir + "/" + template + "_" + str(cnt)
+        if not os.access(tmp, os.R_OK):
+            fname = tmp
+            break
+        # Safety valve
+        if cnt > 10000:
+            break
+    return fname
+
+# ------------------------------------------------------------------------
+# Execute man loop
+
+def mainloop():
+    while True:
+        ev = Gdk.event_peek()
+        #print( ev)
+        if ev:
+            if ev.type == Gdk.EventType.DELETE:
+                break
+            if ev.type == Gdk.EventType.UNMAP:
+                break
+        if Gtk.main_iteration_do(True):
+            break
+
+class Unbuffered(object):
+    def __init__(self, stream):
+        self.stream = stream
+
+    def write(self, data):
+        self.stream.write(data)
+        self.stream.flush()
+
+    def writelines(self, datas):
+        self.stream.writelines(datas)
+        self.stream.flush()
+
+    def __getattr__(self, attr):
+        return getattr(self.stream, attr)
+
+# Time to str and str to time
+
+def time_n2s(ttt):
+    sss = time.ctime(ttt)
+    return sss
+
+def time_s2n(sss):
+    rrr = time.strptime(sss)
+    ttt = time.mktime(rrr)
+    return ttt
+
+def yes_no_cancel(title, message, cancel = True, parent = None):
+
+    #warnings.simplefilter("ignore")
+    dialog = Gtk.Dialog(title,
+                   None,
+                   Gtk.DialogFlags.MODAL | Gtk.DialogFlags.DESTROY_WITH_PARENT)
+
+
+    dialog.set_default_response(Gtk.ResponseType.YES)
+    dialog.set_position(Gtk.WindowPosition.CENTER)
+    dialog.set_transient_for(parent)
+
+    sp = "     "
+    label = Gtk.Label(message)
+    label2 = Gtk.Label(sp)
+    label3 = Gtk.Label(sp)
+    label2a = Gtk.Label(sp)
+    label3a = Gtk.Label(sp)
+
+    hbox = Gtk.HBox()
+
+    hbox.pack_start(label2, 0, 0, 0)
+    hbox.pack_start(label, 1, 1, 0)
+    hbox.pack_start(label3, 0, 0, 0)
+
+    dialog.vbox.pack_start(label2a, 0, 0, 0)
+    dialog.vbox.pack_start(hbox, 0, 0, 0)
+    dialog.vbox.pack_start(label3a, 0, 0, 0)
+
+    dialog.add_button("_Yes", Gtk.ResponseType.YES)
+    dialog.add_button("_No", Gtk.ResponseType.NO)
+
+    if cancel:
+        dialog.add_button("_Cancel", Gtk.ResponseType.CANCEL)
+
+    dialog.connect("key-press-event", yn_key, cancel)
+    #dialog.connect("key-release-event", yn_key, cancel)
+    #warnings.simplefilter("default")
+
+    dialog.show_all()
+    response = dialog.run()
+    # Convert all responses to cancel
+    if  response == Gtk.ResponseType.CANCEL or \
+        response == Gtk.ResponseType.REJECT or \
+        response == Gtk.ResponseType.CLOSE  or \
+        response == Gtk.ResponseType.DELETE_EVENT:
+        response = Gtk.ResponseType.CANCEL
+    dialog.destroy()
+
+    return  response
+
+def yn_key(win, event, cancel):
+    #print( event)
+    if event.keyval == Gdk.KEY_y or \
+        event.keyval == Gdk.KEY_Y:
+        win.response(Gtk.ResponseType.YES)
+
+    if event.keyval == Gdk.KEY_n or \
+        event.keyval == Gdk.KEY_N:
+        win.response(Gtk.ResponseType.NO)
+
+    if cancel:
+        if event.keyval == Gdk.KEY_c or \
+            event.keyval == Gdk.KEY_C:
+            win.response(Gtk.ResponseType.CANCEL)
+
+def opendialog(parent=None):
+
+    # We create an array, so it is passed around by reference
+    fname = [""]
+
+    def makefilter(mask, name):
+        filter =  Gtk.FileFilter.new()
+        filter.add_pattern(mask)
+        filter.set_name(name)
+        return filter
+
+    def done_open_fc(win, resp, fname):
+        #print "done_open_fc", win, resp
+        if resp == Gtk.ButtonsType.OK:
+            fname[0] = win.get_filename()
+            if not fname[0]:
+                #print "Must have filename"
+                pass
+            elif os.path.isdir(fname[0]):
+                os.chdir(fname[0])
+                win.set_current_folder(fname[0])
+                return
+            else:
+                #print("OFD", fname[0])
+                pass
+        win.destroy()
+
+    but =   "Cancel", Gtk.ButtonsType.CANCEL,\
+            "Open File", Gtk.ButtonsType.OK
+
+    fc = Gtk.FileChooserDialog("Open file", parent, \
+         Gtk.FileChooserAction.OPEN  \
+        , but)
+
+    filters = []
+    filters.append(makefilter("*.mup", "MarkUp files (*.py)"))
+    filters.append(makefilter("*.*", "All files (*.*)"))
+
+    if filters:
+        for aa in filters:
+            fc.add_filter(aa)
+
+    fc.set_default_response(Gtk.ButtonsType.OK)
+    fc.set_current_folder(os.getcwd())
+    fc.connect("response", done_open_fc, fname)
+    #fc.connect("current-folder-changed", self.folder_ch )
+    #fc.set_current_name(self.fname)
+    fc.run()
+    #print("OFD2", fname[0])
+    return fname[0]
+
+def savedialog(resp):
+
+    #print "File dialog"
+    fname = [""]   # So it is passed around as a reference
+
+    def makefilter(mask, name):
+        filterx =  Gtk.FileFilter.new()
+        filterx.add_pattern(mask)
+        filterx.set_name(name)
+        return filterx
+
+    def done_fc(win, resp, fname):
+        #print( "done_fc", win, resp)
+        if resp == Gtk.ResponseType.OK:
+            fname[0] = win.get_filename()
+            if not fname[0]:
+                print("Must have filename")
+            else:
+                pass
+        win.destroy()
+
+    but =   "Cancel", Gtk.ResponseType.CANCEL,   \
+                    "Save File", Gtk.ResponseType.OK
+    fc = Gtk.FileChooserDialog("Save file as ... ", None,
+            Gtk.FileChooserAction.SAVE, but)
+
+    #fc.set_do_overwrite_confirmation(True)
+
+    filters = []
+    filters.append(makefilter("*.mup", "MarkUp files (*.py)"))
+    filters.append(makefilter("*.*", "All files (*.*)"))
+
+    if filters:
+        for aa in filters:
+            fc.add_filter(aa)
+
+    fc.set_current_name(os.path.basename(fname[0]))
+    fc.set_current_folder(os.path.dirname(fname[0]))
+    fc.set_default_response(Gtk.ResponseType.OK)
+    fc.connect("response", done_fc, fname)
+    fc.run()
+    return fname[0]
+
+# ------------------------------------------------------------------------
+
+def leadspace(strx):
+
+    ''' Count lead spaces '''
+
+    cnt = 0
+    for aa in range(len(strx)):
+        bb = strx[aa]
+        if bb == " ":
+            cnt += 1
+        elif bb == "\t":
+            cnt += 1
+        elif bb == "\r":
+            cnt += 1
+        elif bb == "\n":
+            cnt += 1
+        else:
+            break
+    return cnt
+
+def wrapscroll(what):
+
+    scroll2 = Gtk.ScrolledWindow()
+    scroll2.add(what)
+    frame2 = Gtk.Frame()
+    frame2.add(scroll2)
+    return frame2
+
+if __name__ == '__main__':
+    print("This file was not meant to run directly")
+
+# EOF
```

### Comparing `pyvguicom-1.0.0/pyvguicom/pgwkit.py` & `pyvguicom-1.0.1/pyvguicom/pgwkit.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.0.0/pyvguicom/plug.py` & `pyvguicom-1.0.1/pyvguicom/plug.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.0.0/pyvguicom/testbutt.py` & `pyvguicom-1.0.1/pyvguicom/testbutt.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,69 +10,71 @@
 from gi.repository import GLib
 from gi.repository import GObject
 from gi.repository import Pango
 
 gi.require_version('WebKit2', '4.0')
 from gi.repository import WebKit2
 
-from pgbutt import *
-from pggui import *
+import pgbutt
+import pggui
 
 class testWin(Gtk.Window):
 
     def __init__(self, *args, **kwargs):
         super(testWin, self).__init__(*args, **kwargs)
 
         self.connect("destroy", Gtk.main_quit)
 
         vbox13 = Gtk.VBox()
 
-        vbox13.pack_start(vspacer(), 0, 0, 0)
-        vbox13.pack_start(Gtk.Label.new("Test smallbutt TEST implementation"), 1, 1, 0)
-        #vbox13.pack_start(vspacer(), 1, 1, 0)
+        vbox13.pack_start(pggui.ySpacer(), 0, 0, 0)
+        vbox13.pack_start(Gtk.Label.new("Smallbutt TEST implementation"), 1, 1, 0)
+        #vbox13.pack_start(pggui.ySpacer(), 1, 1, 0)
 
         hbox13 = Gtk.HBox()
-        hbox13.pack_start(vspacer(), 1, 1, 0)
-        butt3x = smallbutt(" _Find in Text ", self.findx, "")
+        hbox13.pack_start(pggui.ySpacer(), 1, 1, 0)
+        butt3x = pgbutt.smallbutt(" _Find in Text ", self.findx, "")
         hbox13.pack_start(butt3x, 0, 0, 0)
-        hbox13.pack_start(vspacer(), 0, 0, 0)
-        butt3z = smallbutt(" _Search All ", self.findx, "")
+        hbox13.pack_start(pggui.ySpacer(), 0, 0, 0)
+        butt3z = pgbutt.smallbutt(" _Search All ", self.findx, "")
         hbox13.pack_start(butt3z, 0, 0, 0)
-        hbox13.pack_start(vspacer(), 1, 1, 0)
+        hbox13.pack_start(pggui.ySpacer(), 1, 1, 0)
 
         hbox16 = Gtk.HBox()
-        hbox16.pack_start(vspacer(), 1, 1, 0)
-        butt3x = smallbutt("_Align in Text", self.findx, "")
+        hbox16.pack_start(pggui.ySpacer(), 1, 1, 0)
+        butt3x = pgbutt.smallbutt("_Align in Text", self.findx, "")
         hbox16.pack_start(butt3x, 0, 0, 0)
-        hbox16.pack_start(vspacer(), 0, 0, 0)
-        butt3z = smallbutt("_Delete All", self.delx, "")
+        hbox16.pack_start(pggui.ySpacer(), 0, 0, 0)
+        butt3z = pgbutt.smallbutt("_Delete All", self.delx, "")
         hbox16.pack_start(butt3z, 0, 0, 0)
-        hbox16.pack_start(vspacer(), 1, 1, 0)
+        hbox16.pack_start(pggui.ySpacer(), 1, 1, 0)
 
         hbox14 = Gtk.HBox()
-        hbox14.pack_start(vspacer(), 1, 1, 0)
-        butt3y = smallbutt("E_xit", self.exit_prog, "Exit program")
+        hbox14.pack_start(pggui.ySpacer(), 1, 1, 0)
+        butt3y = pgbutt.smallbutt("E_xit", self.exit_prog, "Exit program")
         hbox14.pack_start(butt3y, 0, 0, 0)
-        hbox14.pack_start(vspacer(), 1, 1, 0)
+        hbox14.pack_start(pggui.ySpacer(), 1, 1, 0)
 
         hbox15 = Gtk.HBox()
-        hbox15.pack_start(vspacer(), 1, 1, 0)
-        butt3z = Gtk.Button.new_with_mnemonic("Regular _Button")
+        hbox15.pack_start(pggui.ySpacer(), 1, 1, 0)
+        butt3z = Gtk.Button.new_with_mnemonic("Regular small _Button")
         butt3z.set_relief(Gtk.ReliefStyle.NONE)
         butt3z.connect("clicked", self.regbutt)
         hbox15.pack_start(butt3z, 0, 0, 0)
-        hbox15.pack_start(vspacer(), 1, 1, 0)
+        hbox15.pack_start(pggui.ySpacer(), 1, 1, 0)
+
 
         vbox13.pack_start(hbox13, 0, 0, 0)
         vbox13.pack_start(hbox16, 0, 0, 0)
-        #vbox13.pack_start(hbox15, 0, 0, 0)
         vbox13.pack_start(hbox14, 0, 0, 0)
-        vbox13.pack_start(vspacer(), 1, 1, 0)
+        vbox13.pack_start(hbox15, 0, 0, 0)
+
+        vbox13.pack_start(pggui.ySpacer(), 1, 1, 0)
 
-        self.set_size_request(300, 200)
+        self.set_size_request(400, 300)
         self.add(vbox13)
         self.show_all()
 
         # Gtk.Label
         #print("children", butt3x.get_children())
 
     def regbutt(self, arg):
```

### Comparing `pyvguicom-1.0.0/pyvguicom/testicons.py` & `pyvguicom-1.0.1/pyvguicom/testicons.py`

 * *Files identical despite different names*

### Comparing `pyvguicom-1.0.0/pyvguicom/testnums.py` & `pyvguicom-1.0.1/pyvguicom/testnums.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,41 +8,33 @@
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk
 from gi.repository import Gdk
 from gi.repository import GObject
 from gi.repository import GLib
 
-from pgsimp import *
+from pgsel import *
 from pgutils import *
 from pggui import *
 from pgbox import *
 
 #def OnExit(arg1, arg2):
 #    #print("Exiting", arg1, arg2)
 #    Gtk.main_quit()
 
 # ------------------------------------------------------------------------
 class testwin(Gtk.Window):
 
     def __init__(self):
         Gtk.Window.__init__(self)
-        self.set_default_size(1024, 768)
+        #self.set_default_size(1024, 768)
         #self.set_default_size(800, 600)
         self.set_position(Gtk.WindowPosition.CENTER)
         self.connect("unmap", Gtk.main_quit)
 
-def wrapscroll(what):
-
-    scroll2 = Gtk.ScrolledWindow()
-    scroll2.add(what)
-    frame2 = Gtk.Frame()
-    frame2.add(scroll2)
-    return frame2
-
 # ------------------------------------------------------------------------
 
 class pgtestwin(testwin):
 
     def __init__(self):
 
         testwin.__init__(self)
@@ -78,14 +70,18 @@
         hbox4.pack_start(self.ts4a, 0, 0, 2)
 
         vbox.pack_start(hbox3, 0, 0, 2)
         vbox.pack_start(hbox4, 0, 0, 2)
         vbox.pack_start(hbox, 1, 1, 2)
         vbox.pack_start(hbox5, 0, 0, 2)
 
+        butt = Gtk.Button.new_with_mnemonic("E_xit")
+        butt.connect("clicked", Gtk.main_quit)
+        vbox.pack_start(butt, 0, 0, 2)
+
         self.add(vbox)
         self.show_all()
 
     def  letterfilter(self, letter):
         #print("letterfilter", letter)
         self.label.set_text(letter)
 
@@ -106,15 +102,14 @@
 
     def change_ts4a(self, val):
         #print("change_ms2", val)
         self.label.set_text("M click: " + str(val))
         pass
 
 tw = pgtestwin()
-
 cnt = 0;
 
 def  handler_tick(ww):
 
     global cnt
     #print("handler_tick", ww)
```

### Comparing `pyvguicom-1.0.0/pyvguicom/testroot.py` & `pyvguicom-1.0.1/pyvguicom/testroot.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from gi.repository import GObject
 from gi.repository import Pango
 
 #gi.require_version('WebKit2', '4.0')
 #from gi.repository import WebKit2
 
 from pgbutt import *
-from pggui import *
+import pggui
 
 # Allow the core to search pydbase
 #fff = os.path.realpath(os.path.dirname(__file__) + os.sep + "../pydbase/")
 fff =  "../pydbase/"
 #print(fff)
 
 sys.path.append(fff)
@@ -96,33 +96,34 @@
     def __init__(self, *args, **kwargs):
         super(testWin, self).__init__(*args, **kwargs)
 
         self.connect("destroy", self.dest)
 
         vbox13 = Gtk.VBox()
 
-        #vbox13.pack_start(vspacer(), 0, 0, 0)
+        #vbox13.pack_start(pggui.ySpacer(), 0, 0, 0)
         vbox13.pack_start(Gtk.Label.new("  Test root entry window implementation  "), 1, 1, 0)
 
         #popup.set_titlebar(Gtk.Button())
         #popup.set_titlebar(hb)
 
         self.arr = []
         for aa in range(3):
             self.arr.append(PopWin())
-        vbox13.pack_start(vspacer(), 1, 1, 0)
+
+        vbox13.pack_start(pggui.ySpacer(), 1, 1, 0)
 
         hbox14 = Gtk.HBox()
-        hbox14.pack_start(vspacer(), 1, 1, 0)
+        hbox14.pack_start(pggui.ySpacer(), 1, 1, 0)
         butt3y = smallbutt("E_xit", self.exit_prog, "Exit program")
         hbox14.pack_start(butt3y, 0, 0, 0)
-        hbox14.pack_start(vspacer(), 1, 1, 0)
+        hbox14.pack_start(pggui.ySpacer(), 1, 1, 0)
 
         vbox13.pack_start(hbox14, 0, 0, 0)
-        vbox13.pack_start(vspacer(12), 0, 0, 0)
+        vbox13.pack_start(pggui.ySpacer(12), 0, 0, 0)
 
         self.set_size_request(300, 200)
         self.add(vbox13)
         self.show_all()
 
         for bb in self.arr:
             bb.post()
```

### Comparing `pyvguicom-1.0.0/pyvguicom/testsimple.py` & `pyvguicom-1.0.1/pyvguicom/testsimple.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 #!/usr/bin/env python
 
 from __future__ import print_function
 
 import os, sys, getopt, signal, select, string, time
 import struct, stat, base64, random, zlib
 
-from pgsimp import *
-from pgutils import *
+import gi
+gi.require_version("Gtk", "3.0")
+from gi.repository import Gtk
+from gi.repository import Gdk
+from gi.repository import GLib
+from gi.repository import GObject
+from gi.repository import Pango
 
-#def OnExit(arg1, arg2):
-#    #print("Exiting", arg1, arg2)
-#    Gtk.main_quit()
+import pgsimp
+import pgutils
 
 # ------------------------------------------------------------------------
 class testwin(Gtk.Window):
 
     def __init__(self):
         Gtk.Window.__init__(self)
-        self.set_default_size(1024, 768)
-        #self.set_default_size(800, 600)
+        #self.set_default_size(1024, 768)
+        self.set_default_size(800, 600)
         self.set_position(Gtk.WindowPosition.CENTER)
         self.connect("unmap", Gtk.main_quit)
 
-
-def wrapscroll(what):
-
-    scroll2 = Gtk.ScrolledWindow()
-    scroll2.add(what)
-    frame2 = Gtk.Frame()
-    frame2.add(scroll2)
-    return frame2
-
 # ------------------------------------------------------------------------
 
 class pgtestwin(testwin):
 
     def __init__(self):
 
         testwin.__init__(self)
@@ -44,46 +39,44 @@
         hbox5 = Gtk.HBox()
 
         self.label = Gtk.Label.new("Test strings here")
         hbox5.pack_start(self.label, 1, 1, 2)
 
         vbox  = Gtk.VBox()
 
-        self.treeview = SimpleTree(("Hour", "Subject", "Alarm", "Notes"))
-        frame2 = wrapscroll(self.treeview)
+        self.treeview = pgsimp.SimpleTree(("Hour", "Subject", "Alarm", "Notes"))
+        frame2 = pgutils.wrapscroll(self.treeview)
         hbox.pack_start(frame2, 1, 1, 2)
 
-        self.editor = SimpleEdit()
-        frame3 = wrapscroll(self.editor)
+        self.editor = pgsimp.SimpleEdit()
+        frame3 = pgutils.wrapscroll(self.editor)
         hbox.pack_start(frame3, 1, 1, 2)
 
-        self.selector = LetterNumberSel(self.letterfilter, "Mono 16")
-        hbox2.pack_start(self.selector , 1, 1, 2)
-
         vbox.pack_start(hbox3, 0, 0, 2)
         vbox.pack_start(hbox2, 0, 0, 2)
         vbox.pack_start(hbox4, 0, 0, 2)
         vbox.pack_start(hbox, 1, 1, 2)
         vbox.pack_start(hbox5, 0, 0, 2)
 
+        butt = Gtk.Button.new_with_mnemonic("E_xit")
+        butt.connect("clicked", Gtk.main_quit)
+        vbox.pack_start(butt, 0, 0, 2)
+
         self.add(vbox)
         self.show_all()
 
-    def  letterfilter(self, letter):
-        #print("letterfilter", letter)
-        self.label.set_text(letter)
-
 tw = pgtestwin()
 
 #print("test")
 
 def fillrand():
     aaa = []
     for aa in range(10):
-        aaa.append( (randstr(12), randstr(12), randstr(12), randstr(12)) )
+        aaa.append( (pgutils.randstr(12), pgutils.randstr(12),
+                        pgutils.randstr(12), pgutils.randstr(12)) )
     return aaa
 
 aaa = fillrand()
 tw.treeview.clear()
 for aa in aaa:
     try:
         tw.treeview.append(aa)
@@ -97,7 +90,8 @@
         tw.editor.append(str(aa) + "\n")
     except:
         print(sys.exc_info())
 
 
 Gtk.main()
 
+# EOF
```

### Comparing `pyvguicom-1.0.0/pyvguicom/testtextv.py` & `pyvguicom-1.0.1/pyvguicom/testtextv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,29 @@
 #!/usr/bin/env python
 
 '''
-
   This is a test application for driving the pgTextView control;
   It has load / save functionality.
-
 '''
-
 import os, sys, getopt, signal, random, time, warnings
 
-#from pgutil import  *
-#from pgui import  *
-
-import pgutils
-import pgtextview
-
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk
 from gi.repository import Gdk
 from gi.repository import GLib
 from gi.repository import GObject
 from gi.repository import Pango
 
-import pgbox
-import sutil
+import pgutils
+import pgtextview
 
 #deftext = "It puzzles me when I see a person lacking fundamentals is \
 #  able to amass a fortune to the tune of billions. What is even more \
-#puzziling is that they beleive their 'BS' and open flout all."
+#puzziling is that they beleive their own 'BS' and openly flout all."
 
 # The pango example text
 
 deftext = \
 '''
 Text sizes: <span size="xx-small">tiny</span> <span size="x-small">very small</span> <span size="small">small</span> <span size="medium">normal</span> <span size="large">large</span> <span size="x-large">very large</span> <span size="xx-large">huge</span>
 Text <span color="gray">c<span color="green">o</span>l<span color="tomato">o</span>rs</span> and <span background="pink">backgrounds</span>
```

### Comparing `pyvguicom-1.0.0/pyvguicom.egg-info/PKG-INFO` & `pyvguicom-1.0.1/pyvguicom.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 Metadata-Version: 2.1
 Name: pyvguicom
-Version: 1.0.0
+Version: 1.0.1
 Summary: High power secure server GUI utility helpers.
-Home-page: https://github.com/pglen/pyvserv
+Home-page: https://github.com/pglen/pyguicom.git
 Author: Peter Glen
 Author-email: peterglen99@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 6 - Mature
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: Python Software Foundation License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
 # pyvguicom  PyV GUI Common utilities
 
 ## Common GUI routines and classes
```

### Comparing `pyvguicom-1.0.0/pyvguicom.egg-info/SOURCES.txt` & `pyvguicom-1.0.1/pyvguicom.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 README.md
 setup.py
 pyvguicom/__init__.py
 pyvguicom/browsewin.py
+pyvguicom/custwidg.py
 pyvguicom/htmledit.py
 pyvguicom/pgbox.py
 pyvguicom/pgbutt.py
 pyvguicom/pgentry.py
 pyvguicom/pggui.py
+pyvguicom/pgsel.py
 pyvguicom/pgsimp.py
 pyvguicom/pgtextview.py
 pyvguicom/pgutils.py
 pyvguicom/pgwkit.py
 pyvguicom/plug.py
-pyvguicom/sutil.py
 pyvguicom/testbutt.py
+pyvguicom/testcust.py
+pyvguicom/testentry.py
 pyvguicom/testicons.py
+pyvguicom/testlettsel.py
 pyvguicom/testnums.py
 pyvguicom/testroot.py
 pyvguicom/testsimple.py
 pyvguicom/testtextv.py
 pyvguicom.egg-info/PKG-INFO
 pyvguicom.egg-info/SOURCES.txt
 pyvguicom.egg-info/dependency_links.txt
```

### Comparing `pyvguicom-1.0.0/setup.py` & `pyvguicom-1.0.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,47 +2,41 @@
 
 descx = '''
     These classes are for python PyGobject (Gtk) development. They are used in
     several projects. They act as a simplification front end for the PyGtk / PyGobject
     classes.
     '''
 
+includex = ["*", "pyvguicom"]
+
 classx = [
-          'Development Status :: Mature',
-          'Environment :: GUI',
+          'Development Status :: 6 - Mature',
           'Intended Audience :: End Users/Desktop',
           'Intended Audience :: Developers',
           'Intended Audience :: System Administrators',
           'License :: OSI Approved :: Python Software Foundation License',
           'Operating System :: Microsoft :: Windows',
           'Operating System :: POSIX',
           'Programming Language :: Python',
-          'Topic :: Editors',
-          'Topic :: Software Development :: Servers',
+          'Topic :: Software Development :: Libraries',
         ]
 
-includex = ["*", "pyvguicom"]
-
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyvguicom",
-    version="1.0.0",
+    version="1.0.1",
     author="Peter Glen",
     author_email="peterglen99@gmail.com",
     description="High power secure server GUI utility helpers.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/pglen/pyvserv",
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
+    url="https://github.com/pglen/pyguicom.git",
+    classifiers= classx,
     include_package_data=True,
     packages=setuptools.find_packages(include=includex),
     package_dir = {
                     'pyvguicom':           'pyvguicom',
                    },
     python_requires='>=3',
     entry_points={
```

