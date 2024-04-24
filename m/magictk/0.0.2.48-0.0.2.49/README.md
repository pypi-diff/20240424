# Comparing `tmp/magictk-0.0.2.48.tar.gz` & `tmp/magictk-0.0.2.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magictk-0.0.2.48.tar", last modified: Mon Apr 22 04:03:59 2024, max compression
+gzip compressed data, was "magictk-0.0.2.49.tar", last modified: Tue Apr 23 14:33:19 2024, max compression
```

## Comparing `magictk-0.0.2.48.tar` & `magictk-0.0.2.49.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 04:03:59.855080 magictk-0.0.2.48/
--rw-r--r--   0 root         (0) root         (0)       47 2024-04-22 04:03:59.000000 magictk-0.0.2.48/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-22 04:03:59.855080 magictk-0.0.2.48/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1376 2024-04-22 04:03:59.000000 magictk-0.0.2.48/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 04:03:59.855080 magictk-0.0.2.48/magictk/
--rw-r--r--   0 root         (0) root         (0)      411 2024-04-22 04:03:59.000000 magictk-0.0.2.48/magictk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9695 2024-04-22 04:03:59.000000 magictk-0.0.2.48/magictk/_window_ctl.py
--rw-r--r--   0 root         (0) root         (0)    13250 2024-04-22 04:03:59.000000 magictk-0.0.2.48/magictk/_window_size.py
--rw-r--r--   0 root         (0) root         (0)     3253 2024-04-22 04:03:59.000000 magictk-0.0.2.48/magictk/basicwindow.py
--rw-r--r--   0 root         (0) root         (0)    13450 2024-04-22 04:03:59.000000 magictk-0.0.2.48/magictk/button.py
--rw-r--r--   0 root         (0) root         (0)    11146 2024-04-22 04:03:59.000000 magictk-0.0.2.48/magictk/checkbox.py
--rw-r--r--   0 root         (0) root         (0)     1919 2024-04-22 04:03:59.000000 magictk-0.0.2.48/magictk/color_tmpl.py
--rw-r--r--   0 root         (0) root         (0)    12042 2024-04-22 04:03:59.000000 magictk-0.0.2.48/magictk/entry.py
--rw-r--r--   0 root         (0) root         (0)      578 2024-04-22 04:03:59.000000 magictk-0.0.2.48/magictk/fontconfig.py
--rw-r--r--   0 root         (0) root         (0)     1493 2024-04-22 04:03:59.000000 magictk-0.0.2.48/magictk/frame.py
--rw-r--r--   0 root         (0) root         (0)    15906 2024-04-22 04:03:59.000000 magictk-0.0.2.48/magictk/icon.ico
--rw-r--r--   0 root         (0) root         (0)       70 2024-04-22 04:03:59.000000 magictk-0.0.2.48/magictk/mtk.py
--rw-r--r--   0 root         (0) root         (0)      720 2024-04-22 04:03:59.000000 magictk-0.0.2.48/magictk/photoload.py
--rw-r--r--   0 root         (0) root         (0)     5893 2024-04-22 04:03:59.000000 magictk-0.0.2.48/magictk/progressbar.py
--rw-r--r--   0 root         (0) root         (0)    22329 2024-04-22 04:03:59.000000 magictk-0.0.2.48/magictk/res.pickle
--rw-r--r--   0 root         (0) root         (0)     7112 2024-04-22 04:03:59.000000 magictk-0.0.2.48/magictk/scrollbar.py
--rw-r--r--   0 root         (0) root         (0)     6077 2024-04-22 04:03:59.000000 magictk-0.0.2.48/magictk/select.py
--rw-r--r--   0 root         (0) root         (0)    11076 2024-04-22 04:03:59.000000 magictk-0.0.2.48/magictk/submenu.py
--rw-r--r--   0 root         (0) root         (0)    10213 2024-04-22 04:03:59.000000 magictk-0.0.2.48/magictk/window.py
--rw-r--r--   0 root         (0) root         (0)     2647 2024-04-22 04:03:59.000000 magictk-0.0.2.48/magictk/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 04:03:59.855080 magictk-0.0.2.48/magictk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-22 04:03:59.000000 magictk-0.0.2.48/magictk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      592 2024-04-22 04:03:59.000000 magictk-0.0.2.48/magictk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 04:03:59.000000 magictk-0.0.2.48/magictk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-22 04:03:59.000000 magictk-0.0.2.48/magictk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-22 04:03:59.855080 magictk-0.0.2.48/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1127 2024-04-22 04:03:59.000000 magictk-0.0.2.48/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 14:33:19.956346 magictk-0.0.2.49/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-04-23 14:33:19.000000 magictk-0.0.2.49/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      595 2024-04-23 14:33:19.956346 magictk-0.0.2.49/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1376 2024-04-23 14:33:19.000000 magictk-0.0.2.49/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 14:33:19.956346 magictk-0.0.2.49/magictk/
+-rw-r--r--   0 root         (0) root         (0)      411 2024-04-23 14:33:19.000000 magictk-0.0.2.49/magictk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9695 2024-04-23 14:33:19.000000 magictk-0.0.2.49/magictk/_window_ctl.py
+-rw-r--r--   0 root         (0) root         (0)    13250 2024-04-23 14:33:19.000000 magictk-0.0.2.49/magictk/_window_size.py
+-rw-r--r--   0 root         (0) root         (0)     3253 2024-04-23 14:33:19.000000 magictk-0.0.2.49/magictk/basicwindow.py
+-rw-r--r--   0 root         (0) root         (0)    13450 2024-04-23 14:33:19.000000 magictk-0.0.2.49/magictk/button.py
+-rw-r--r--   0 root         (0) root         (0)    11146 2024-04-23 14:33:19.000000 magictk-0.0.2.49/magictk/checkbox.py
+-rw-r--r--   0 root         (0) root         (0)     1919 2024-04-23 14:33:19.000000 magictk-0.0.2.49/magictk/color_tmpl.py
+-rw-r--r--   0 root         (0) root         (0)    12042 2024-04-23 14:33:19.000000 magictk-0.0.2.49/magictk/entry.py
+-rw-r--r--   0 root         (0) root         (0)      578 2024-04-23 14:33:19.000000 magictk-0.0.2.49/magictk/fontconfig.py
+-rw-r--r--   0 root         (0) root         (0)     2547 2024-04-23 14:33:19.000000 magictk-0.0.2.49/magictk/frame.py
+-rw-r--r--   0 root         (0) root         (0)    15906 2024-04-23 14:33:19.000000 magictk-0.0.2.49/magictk/icon.ico
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-23 14:33:19.000000 magictk-0.0.2.49/magictk/mtk.py
+-rw-r--r--   0 root         (0) root         (0)      720 2024-04-23 14:33:19.000000 magictk-0.0.2.49/magictk/photoload.py
+-rw-r--r--   0 root         (0) root         (0)     5893 2024-04-23 14:33:19.000000 magictk-0.0.2.49/magictk/progressbar.py
+-rw-r--r--   0 root         (0) root         (0)    22329 2024-04-23 14:33:19.000000 magictk-0.0.2.49/magictk/res.pickle
+-rw-r--r--   0 root         (0) root         (0)     8106 2024-04-23 14:33:19.000000 magictk-0.0.2.49/magictk/scrollbar.py
+-rw-r--r--   0 root         (0) root         (0)     6077 2024-04-23 14:33:19.000000 magictk-0.0.2.49/magictk/select.py
+-rw-r--r--   0 root         (0) root         (0)    11076 2024-04-23 14:33:19.000000 magictk-0.0.2.49/magictk/submenu.py
+-rw-r--r--   0 root         (0) root         (0)    10213 2024-04-23 14:33:19.000000 magictk-0.0.2.49/magictk/window.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2024-04-23 14:33:19.000000 magictk-0.0.2.49/magictk/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 14:33:19.956346 magictk-0.0.2.49/magictk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      595 2024-04-23 14:33:19.000000 magictk-0.0.2.49/magictk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      592 2024-04-23 14:33:19.000000 magictk-0.0.2.49/magictk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 14:33:19.000000 magictk-0.0.2.49/magictk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-23 14:33:19.000000 magictk-0.0.2.49/magictk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 14:33:19.956346 magictk-0.0.2.49/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-04-23 14:33:19.000000 magictk-0.0.2.49/setup.py
```

### Comparing `magictk-0.0.2.48/PKG-INFO` & `magictk-0.0.2.49/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: magictk
-Version: 0.0.2.48
+Version: 0.0.2.49
 Summary: A tkinter weights looks like element-plus
 Home-page: http://git.hmtsai.cn/cxykevin/magictk.git
 Author: cxykevin|git.hmtsai.cn
 Author-email: cxykevin@yeah.net
 License: GPLv2
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `magictk-0.0.2.48/README.md` & `magictk-0.0.2.49/README.md`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.48/magictk/_window_ctl.py` & `magictk-0.0.2.49/magictk/_window_ctl.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.48/magictk/_window_size.py` & `magictk-0.0.2.49/magictk/_window_size.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.48/magictk/basicwindow.py` & `magictk-0.0.2.49/magictk/basicwindow.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.48/magictk/button.py` & `magictk-0.0.2.49/magictk/button.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.48/magictk/checkbox.py` & `magictk-0.0.2.49/magictk/checkbox.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.48/magictk/color_tmpl.py` & `magictk-0.0.2.49/magictk/color_tmpl.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.48/magictk/entry.py` & `magictk-0.0.2.49/magictk/entry.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.48/magictk/fontconfig.py` & `magictk-0.0.2.49/magictk/fontconfig.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.48/magictk/icon.ico` & `magictk-0.0.2.49/magictk/icon.ico`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.48/magictk/photoload.py` & `magictk-0.0.2.49/magictk/photoload.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.48/magictk/progressbar.py` & `magictk-0.0.2.49/magictk/progressbar.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.48/magictk/res.pickle` & `magictk-0.0.2.49/magictk/res.pickle`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.48/magictk/scrollbar.py` & `magictk-0.0.2.49/magictk/scrollbar.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,52 +11,61 @@
     progress = 0.0
     __progress_pixel = 0
     __move_progress_pixel = 0
     max_flash = 4
     scroll_y = 0
     y_size = 1.0
     bar_len = 100
+    _dis_event = False
 
     def cal_bar(self):
-        self.bar_len = max(self.h*self._r_maxh//self._r_allh, 20)
-        self.y_size = self._r_allh/(self.h-self.bar_len)
+        self.bar_len = self._r_maxh*self.h//self._r_allh
+        if (self.h-self.bar_len == 0):
+            self.y_size = 0
+        else:
+            self.bar_len = max(20, self.bar_len)
+            self.y_size = (self._r_allh-self._r_maxh)/(self.h-self.bar_len)
 
     def __draw_corner(self, r_x, r_y, x, y, colors="#000000", rid="", bgcolor=None, **kwargs):
         if bgcolor is None:
             bgcolor = self.color["border_light"]
         self.__fill_obj[rid] = []
         self.__fill_obj[rid+"_pos"] = []
         self.__fill_obj[rid+"_pos2"] = []
         self.border_info = json.loads(photoload.loadres("scrollbarborder"))
         y_n = 0
         for i in self.border_info:
             x_n = 0
             for j in i:
                 if (r_x == 0):
                     px = x+x_n+1
+                    zpx = x_n+1
                 else:
                     px = x+6-x_n
+                    zpx = 6-x_n
                 if (r_y == 0):
                     py = y+y_n+1
+                    zpy = y_n+1
                 else:
                     py = y+3-y_n-1
+                    zpy = 3-y_n-1
                 if (j < 0):
                     lcolor = -j
                 else:
                     lcolor = j
                 # if(lcolor==255):
                 #     continue
                 g_color = color_tmpl.mix_color(
                     bgcolor, colors, int((1-lcolor/255)*1000)/1000)
 
                 obj = self.canvas.create_rectangle(
                     px, py, px, py, width=0, fill=g_color)
 
                 self.__fill_obj[rid].append(obj)
-                self.__fill_obj[rid+"_pos"].append([px, py])
+                self.__fill_obj[rid+"_pos"].append([zpx, zpy])
                 self.__fill_obj[rid+"_pos2"].append([y_n, x_n])
 
                 x_n += 1
             y_n += 1
 
     def __init__(self, master=None, root_anim=None, w=None, h=8, colors="primary", color_list: dict = None, allh=100,
                  maxh=50, callback=lambda obj, val: None):
@@ -82,68 +91,84 @@
         self.__draw()
         self.bind_event()
         self.update_pos()
 
     def pack(self, *args, **kwargs):
         self.canvas.pack(*args, **kwargs)
 
+    def pack_forget(self, *args, **kwargs):
+        self.canvas.pack_forget(*args, **kwargs)
+
     def grid(self, *args, **kwargs):
         self.canvas.grid(*args, **kwargs)
 
+    def grid_forget(self, *args, **kwargs):
+        self.canvas.grid_forget(*args, **kwargs)
+
     def place(self, *args, **kwargs):
         self.canvas.place(*args, **kwargs)
 
+    def place_forget(self, *args, **kwargs):
+        self.canvas.place_forget(*args, **kwargs)
+
     def update_pos(self):
         for i in range(len(self.__fill_obj["upside"])):
             self.canvas.coords(
                 self.__fill_obj["upside"][i], int(self.__fill_obj["upside_pos"][i][0]), self.__fill_obj["upside_pos"][i][1]+self.scroll_y, int(self.__fill_obj["upside_pos"][i][0]), self.__fill_obj["upside_pos"][i][1]+self.scroll_y)
         self.canvas.coords(
             self.__fill_obj["fgbar"][0], 1, 4+self.scroll_y, self.w-1, self.scroll_y+self.bar_len-4+1)
         for i in range(len(self.__fill_obj["bottomside"])):
             self.canvas.coords(
-                self.__fill_obj["bottomside"][i], int(self.__fill_obj["bottomside_pos"][i][0]), self.__fill_obj["bottomside_pos"][i][1]+self.scroll_y, int(self.__fill_obj["bottomside_pos"][i][0]), self.__fill_obj["bottomside_pos"][i][1]+self.scroll_y)
+                self.__fill_obj["bottomside"][i], int(self.__fill_obj["bottomside_pos"][i][0]), self.__fill_obj["bottomside_pos"][i][1]+self.scroll_y+self.bar_len-5, int(self.__fill_obj["bottomside_pos"][i][0]), self.__fill_obj["bottomside_pos"][i][1]+self.scroll_y+self.bar_len-5)
 
     def bind_event(self):
-        def mouse_press(event: tkinter.Event):
-            if (event.y >= self.scroll_y and event.y <= self.scroll_y+self.bar_len):
-                pass
-            else:
+        def mouse_move(event: tkinter.Event):
+            if (not self._dis_event):
+                delta_y = event.y-self.scroll_y
                 self.scroll_y = min(self.h-self.bar_len,
-                                    max(0, event.y-self.bar_len//2))
-            self.move_start = event.y-self.scroll_y
-            for i in range(len(self.__fill_obj["upside"])):
-                self.canvas.itemconfig(
-                    self.__fill_obj["upside"][i], fill=color_tmpl.mix_color(
-                        self.color["background"], self.color["border_base"], int((1-self.border_info[self.__fill_obj["upside_pos2"][i][0]][self.__fill_obj["upside_pos2"][i][1]]/255)*1000)/1000))
-            self.canvas.itemconfig(
-                self.__fill_obj["fgbar"][0], fill=self.color["border_base"])
-            for i in range(len(self.__fill_obj["bottomside"])):
-                self.canvas.itemconfig(
-                    self.__fill_obj["bottomside"][i], fill=color_tmpl.mix_color(
-                        self.color["background"], self.color["border_base"], int((1-self.border_info[self.__fill_obj["bottomside_pos2"][i][0]][self.__fill_obj["bottomside_pos2"][i][1]]/255)*1000)/1000))
-            self.update_pos()
+                                    max(0, self.scroll_y+delta_y-self.move_start))
+                self.callback(self, self.get())
+                self.update_pos()
 
-        def mouse_move(event: tkinter.Event):
-            delta_y = event.y-self.scroll_y
-            self.scroll_y = min(self.h-self.bar_len,
-                                max(0, self.scroll_y+delta_y-self.move_start))
-            self.callback(self, self.get())
-            self.update_pos()
+        def mouse_press(event: tkinter.Event):
+            if (not self._dis_event):
+                flag = False
+                if (event.y >= self.scroll_y and event.y <= self.scroll_y+self.bar_len):
+                    pass
+                else:
+                    self.scroll_y = min(self.h-self.bar_len,
+                                        max(0, event.y-self.bar_len//2))
+                    flag = True
+                self.move_start = event.y-self.scroll_y
+                for i in range(len(self.__fill_obj["upside"])):
+                    self.canvas.itemconfig(
+                        self.__fill_obj["upside"][i], fill=color_tmpl.mix_color(
+                            self.color["background"], self.color["border_base"], int((1-self.border_info[self.__fill_obj["upside_pos2"][i][0]][self.__fill_obj["upside_pos2"][i][1]]/255)*1000)/1000))
+                self.canvas.itemconfig(
+                    self.__fill_obj["fgbar"][0], fill=self.color["border_base"])
+                for i in range(len(self.__fill_obj["bottomside"])):
+                    self.canvas.itemconfig(
+                        self.__fill_obj["bottomside"][i], fill=color_tmpl.mix_color(
+                            self.color["background"], self.color["border_base"], int((1-self.border_info[self.__fill_obj["bottomside_pos2"][i][0]][self.__fill_obj["bottomside_pos2"][i][1]]/255)*1000)/1000))
+                if (flag):
+                    self.update_pos()
+                    mouse_move(event)
 
         def mouse_release(event: tkinter.Event):
-            for i in range(len(self.__fill_obj["upside"])):
-                self.canvas.itemconfig(
-                    self.__fill_obj["upside"][i], fill=color_tmpl.mix_color(
-                        self.color["background"], self.color["border_light"], int((1-self.border_info[self.__fill_obj["upside_pos2"][i][0]][self.__fill_obj["upside_pos2"][i][1]]/255)*1000)/1000))
-            self.canvas.itemconfig(
-                self.__fill_obj["fgbar"][0], fill=self.color["border_light"])
-            for i in range(len(self.__fill_obj["bottomside"])):
+            if (not self._dis_event):
+                for i in range(len(self.__fill_obj["upside"])):
+                    self.canvas.itemconfig(
+                        self.__fill_obj["upside"][i], fill=color_tmpl.mix_color(
+                            self.color["background"], self.color["border_light"], int((1-self.border_info[self.__fill_obj["upside_pos2"][i][0]][self.__fill_obj["upside_pos2"][i][1]]/255)*1000)/1000))
                 self.canvas.itemconfig(
-                    self.__fill_obj["bottomside"][i], fill=color_tmpl.mix_color(
-                        self.color["background"], self.color["border_light"], int((1-self.border_info[self.__fill_obj["bottomside_pos2"][i][0]][self.__fill_obj["bottomside_pos2"][i][1]]/255)*1000)/1000))
+                    self.__fill_obj["fgbar"][0], fill=self.color["border_light"])
+                for i in range(len(self.__fill_obj["bottomside"])):
+                    self.canvas.itemconfig(
+                        self.__fill_obj["bottomside"][i], fill=color_tmpl.mix_color(
+                            self.color["background"], self.color["border_light"], int((1-self.border_info[self.__fill_obj["bottomside_pos2"][i][0]][self.__fill_obj["bottomside_pos2"][i][1]]/255)*1000)/1000))
 
         self.canvas.bind("<B1-Motion>", mouse_move)
         self.canvas.bind("<Button-1>", mouse_press)
         self.canvas.bind("<ButtonRelease-1>", mouse_release)
 
     def __draw(self):
         self.__draw_corner(0, 0, 0, self.scroll_y,
@@ -151,10 +176,10 @@
         self.__fill_obj["fgbar"] = [
             self.canvas.create_rectangle(1, 4+self.scroll_y, self.w-1, self.scroll_y+self.bar_len-4+1, width=0, fill=self.color["border_light"])]
         self.__draw_corner(0, 1, 0, self.scroll_y+self.bar_len-4+1,
                            self.color["border_light"], "bottomside", bgcolor=self.color["background"])
 
     def get(self):
         if (self.scroll_y+self.bar_len >= self.h):
-            return self._r_allh
+            return self._r_allh-self._r_maxh
         else:
             return int(min(self.scroll_y*self.y_size, self._r_allh))
```

### Comparing `magictk-0.0.2.48/magictk/select.py` & `magictk-0.0.2.49/magictk/select.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.48/magictk/submenu.py` & `magictk-0.0.2.49/magictk/submenu.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.48/magictk/window.py` & `magictk-0.0.2.49/magictk/window.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.48/magictk/workspace.py` & `magictk-0.0.2.49/magictk/workspace.py`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.48/magictk.egg-info/PKG-INFO` & `magictk-0.0.2.49/magictk.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: magictk
-Version: 0.0.2.48
+Version: 0.0.2.49
 Summary: A tkinter weights looks like element-plus
 Home-page: http://git.hmtsai.cn/cxykevin/magictk.git
 Author: cxykevin|git.hmtsai.cn
 Author-email: cxykevin@yeah.net
 License: GPLv2
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `magictk-0.0.2.48/magictk.egg-info/SOURCES.txt` & `magictk-0.0.2.49/magictk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magictk-0.0.2.48/setup.py` & `magictk-0.0.2.49/setup.py`

 * *Files identical despite different names*

