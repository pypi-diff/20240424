# Comparing `tmp/tkeasygui-0.2.57.tar.gz` & `tmp/tkeasygui-0.2.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkeasygui-0.2.57.tar", last modified: Sun Apr 21 13:11:02 2024, max compression
+gzip compressed data, was "tkeasygui-0.2.63.tar", last modified: Wed Apr 24 11:55:38 2024, max compression
```

## Comparing `tkeasygui-0.2.57.tar` & `tkeasygui-0.2.63.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-21 13:11:02.331579 tkeasygui-0.2.57/
--rw-r--r--   0 kujirahand   (501) staff       (20)     1067 2024-03-15 10:03:04.000000 tkeasygui-0.2.57/LICENSE
--rw-r--r--   0 kujirahand   (501) staff       (20)     6828 2024-04-21 13:11:02.331341 tkeasygui-0.2.57/PKG-INFO
--rw-r--r--   0 kujirahand   (501) staff       (20)     4424 2024-04-21 07:45:22.000000 tkeasygui-0.2.57/README.md
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-21 13:11:02.329553 tkeasygui-0.2.57/TkEasyGUI/
--rw-r--r--   0 kujirahand   (501) staff       (20)      376 2024-04-20 12:19:46.000000 tkeasygui-0.2.57/TkEasyGUI/__init__.py
--rw-r--r--   0 kujirahand   (501) staff       (20)    27595 2024-04-21 12:07:15.000000 tkeasygui-0.2.57/TkEasyGUI/dialogs.py
--rw-r--r--   0 kujirahand   (501) staff       (20)     2016 2024-04-21 12:06:43.000000 tkeasygui-0.2.57/TkEasyGUI/locale_easy.py
--rw-r--r--   0 kujirahand   (501) staff       (20)     6538 2024-04-21 06:55:17.000000 tkeasygui-0.2.57/TkEasyGUI/utils.py
--rw-r--r--   0 kujirahand   (501) staff       (20)      168 2024-04-21 13:11:00.000000 tkeasygui-0.2.57/TkEasyGUI/version.py
--rw-r--r--   0 kujirahand   (501) staff       (20)   119550 2024-04-21 13:04:34.000000 tkeasygui-0.2.57/TkEasyGUI/widgets.py
-drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-21 13:11:02.331019 tkeasygui-0.2.57/TkEasyGUI.egg-info/
--rw-r--r--   0 kujirahand   (501) staff       (20)     6828 2024-04-21 13:11:02.000000 tkeasygui-0.2.57/TkEasyGUI.egg-info/PKG-INFO
--rw-r--r--   0 kujirahand   (501) staff       (20)      325 2024-04-21 13:11:02.000000 tkeasygui-0.2.57/TkEasyGUI.egg-info/SOURCES.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)        1 2024-04-21 13:11:02.000000 tkeasygui-0.2.57/TkEasyGUI.egg-info/dependency_links.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)       17 2024-04-21 13:11:02.000000 tkeasygui-0.2.57/TkEasyGUI.egg-info/requires.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)       10 2024-04-21 13:11:02.000000 tkeasygui-0.2.57/TkEasyGUI.egg-info/top_level.txt
--rw-r--r--   0 kujirahand   (501) staff       (20)     1301 2024-04-21 13:10:56.000000 tkeasygui-0.2.57/pyproject.toml
--rw-r--r--   0 kujirahand   (501) staff       (20)       38 2024-04-21 13:11:02.331627 tkeasygui-0.2.57/setup.cfg
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-24 11:55:38.458690 tkeasygui-0.2.63/
+-rw-r--r--   0 kujirahand   (501) staff       (20)     1067 2024-03-15 10:03:04.000000 tkeasygui-0.2.63/LICENSE
+-rw-r--r--   0 kujirahand   (501) staff       (20)     6747 2024-04-24 11:55:38.458466 tkeasygui-0.2.63/PKG-INFO
+-rw-r--r--   0 kujirahand   (501) staff       (20)     4343 2024-04-24 05:52:16.000000 tkeasygui-0.2.63/README.md
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-24 11:55:38.456990 tkeasygui-0.2.63/TkEasyGUI/
+-rw-r--r--   0 kujirahand   (501) staff       (20)      376 2024-04-20 12:19:46.000000 tkeasygui-0.2.63/TkEasyGUI/__init__.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)    27595 2024-04-21 12:07:15.000000 tkeasygui-0.2.63/TkEasyGUI/dialogs.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)     2545 2024-04-24 11:24:23.000000 tkeasygui-0.2.63/TkEasyGUI/locale_easy.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)     6538 2024-04-21 06:55:17.000000 tkeasygui-0.2.63/TkEasyGUI/utils.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)      168 2024-04-24 11:55:36.000000 tkeasygui-0.2.63/TkEasyGUI/version.py
+-rw-r--r--   0 kujirahand   (501) staff       (20)   120490 2024-04-24 10:39:53.000000 tkeasygui-0.2.63/TkEasyGUI/widgets.py
+drwxr-xr-x   0 kujirahand   (501) staff       (20)        0 2024-04-24 11:55:38.458162 tkeasygui-0.2.63/TkEasyGUI.egg-info/
+-rw-r--r--   0 kujirahand   (501) staff       (20)     6747 2024-04-24 11:55:38.000000 tkeasygui-0.2.63/TkEasyGUI.egg-info/PKG-INFO
+-rw-r--r--   0 kujirahand   (501) staff       (20)      325 2024-04-24 11:55:38.000000 tkeasygui-0.2.63/TkEasyGUI.egg-info/SOURCES.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)        1 2024-04-24 11:55:38.000000 tkeasygui-0.2.63/TkEasyGUI.egg-info/dependency_links.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)       17 2024-04-24 11:55:38.000000 tkeasygui-0.2.63/TkEasyGUI.egg-info/requires.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)       10 2024-04-24 11:55:38.000000 tkeasygui-0.2.63/TkEasyGUI.egg-info/top_level.txt
+-rw-r--r--   0 kujirahand   (501) staff       (20)     1301 2024-04-24 11:18:19.000000 tkeasygui-0.2.63/pyproject.toml
+-rw-r--r--   0 kujirahand   (501) staff       (20)       38 2024-04-24 11:55:38.458737 tkeasygui-0.2.63/setup.cfg
```

### Comparing `tkeasygui-0.2.57/LICENSE` & `tkeasygui-0.2.63/LICENSE`

 * *Files identical despite different names*

### Comparing `tkeasygui-0.2.57/PKG-INFO` & `tkeasygui-0.2.63/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TkEasyGUI
-Version: 0.2.57
+Version: 0.2.63
 Summary: TkEasyGUI is simple GUI Library for Python3 with Tkinter
 Author-email: kujirahand <web@kujirahand.com>
 Maintainer-email: kujirahand <web@kujirahand.com>
 License: MIT License
         
         Copyright (c) 2024 kujirahand
         
@@ -83,16 +83,16 @@
 
 ## How to use - popup dialogs
 
 Using TkEasyGUI is simple. If you only want to display a dialog, it requires just two lines of code.
 
 ```py
 import TkEasyGUI as eg
-eg.print("A joyful heart is good medicine.") # popup message
-eg.popup("A joyful heart is good medicine.") # same as eg.print function
+# Displays the message in a popup dialog.
+eg.print("A joyful heart is good medicine.")
 ```
 
 Ask the user for their name and display that name in the window.
 
 ```py
 import TkEasyGUI as eg
 name = eg.input("What is your name?")
@@ -102,38 +102,40 @@
 ### How to use - widgets
 
 To create a simple window with only labels and buttons, you would write as follows:
 
 ```py
 import TkEasyGUI as eg
 # define layout
-layout = [[eg.Text("Hello, World!")],
-          [eg.Button("Exit")]]
+layout = [
+    [eg.Text("Hello, World!")],
+    [eg.Button("OK")]
+]
 # create a window
-with eg.Window("test", layout) as window:
-    # event loop
-    for event, values in window.event_iter():
-        if event == "Exit":
-            eg.popup("Thank you.")
-            break
+window = eg.Window("Hello App", layout)
+# event loop
+for event, values in window.event_iter():
+    if event == "OK":
+        eg.print("Thank you.")
+        break
 ```
 
 You can describe it using an event model similar to the famous GUI library, PySimpleGUI.
 
 ```py
 import TkEasyGUI as eg
+
 # define layout
-layout = [[eg.Text("Hello, World!")],
-          [eg.Button("Exit")]]
+layout = [[eg.Text("Hello, World!")], [eg.Button("OK")]]
 # create a window
-window = eg.Window("test", layout)
+window = eg.Window("Hello App", layout)
 # event loop
 while True:
     event, values = window.read()
-    if event in ["Exit", eg.WINDOW_CLOSED]:
+    if event in ["OK", eg.WINDOW_CLOSED]:
         eg.popup("Thank you.")
         break
 # close window
 window.close()
 ```
 
 ## Samples
```

### Comparing `tkeasygui-0.2.57/README.md` & `tkeasygui-0.2.63/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 
 ## How to use - popup dialogs
 
 Using TkEasyGUI is simple. If you only want to display a dialog, it requires just two lines of code.
 
 ```py
 import TkEasyGUI as eg
-eg.print("A joyful heart is good medicine.") # popup message
-eg.popup("A joyful heart is good medicine.") # same as eg.print function
+# Displays the message in a popup dialog.
+eg.print("A joyful heart is good medicine.")
 ```
 
 Ask the user for their name and display that name in the window.
 
 ```py
 import TkEasyGUI as eg
 name = eg.input("What is your name?")
@@ -54,38 +54,40 @@
 ### How to use - widgets
 
 To create a simple window with only labels and buttons, you would write as follows:
 
 ```py
 import TkEasyGUI as eg
 # define layout
-layout = [[eg.Text("Hello, World!")],
-          [eg.Button("Exit")]]
+layout = [
+    [eg.Text("Hello, World!")],
+    [eg.Button("OK")]
+]
 # create a window
-with eg.Window("test", layout) as window:
-    # event loop
-    for event, values in window.event_iter():
-        if event == "Exit":
-            eg.popup("Thank you.")
-            break
+window = eg.Window("Hello App", layout)
+# event loop
+for event, values in window.event_iter():
+    if event == "OK":
+        eg.print("Thank you.")
+        break
 ```
 
 You can describe it using an event model similar to the famous GUI library, PySimpleGUI.
 
 ```py
 import TkEasyGUI as eg
+
 # define layout
-layout = [[eg.Text("Hello, World!")],
-          [eg.Button("Exit")]]
+layout = [[eg.Text("Hello, World!")], [eg.Button("OK")]]
 # create a window
-window = eg.Window("test", layout)
+window = eg.Window("Hello App", layout)
 # event loop
 while True:
     event, values = window.read()
-    if event in ["Exit", eg.WINDOW_CLOSED]:
+    if event in ["OK", eg.WINDOW_CLOSED]:
         eg.popup("Thank you.")
         break
 # close window
 window.close()
 ```
 
 ## Samples
```

### Comparing `tkeasygui-0.2.57/TkEasyGUI/dialogs.py` & `tkeasygui-0.2.63/TkEasyGUI/dialogs.py`

 * *Files identical despite different names*

### Comparing `tkeasygui-0.2.57/TkEasyGUI/locale_easy.py` & `tkeasygui-0.2.63/TkEasyGUI/locale_easy.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,40 +4,58 @@
 import locale
 from typing import Union
 
 _locale: str = ""
 # locale messages
 _locale_messages: dict[str, dict[str, str]] = {
     "ja": {
+        "__date_format__": "%Y-%m-%d",
         "OK": "OK",
         "Cancel": "キャンセル",
         "Yes": "はい",
         "No": "いいえ",
         "Close": "閉じる",
         "Information": "お知らせ",
         "Warning": "警告",
         "Error": "エラー",
         "Question": "質問",
         "Text Input": "テキスト入力",
         "Select date": "日付の選択",
-        "__date_format__": "%Y-%m-%d",
+        "Copy": "コピー",
+        "Paste": "貼り付け",
+        "Cut": "切り取り",
+        "File": "ファイル",
+        "Open": "開く",
+        "Save": "保存",
+        "Run": "実行",
+        "Quit": "終了",
+        "Thank you.": "ありがとうございます。",
     },
     "zh": {
+        "__date_format__": "%Y年%m月%d日",
         "OK": "好",
         "Cancel": "取消",
         "Yes": "是",
         "No": "不",
         "Close": "关闭",
         "Information": "信息",
         "Warning": "警告",
         "Error": "错误",
         "Question": "问题",
         "Text input": "文本输入",
         "Select date": "选择日期",
-        "__date_format__": "%Y年%m月%d日",
+        "Copy": "复制",
+        "Paste": "粘贴",
+        "Cut": "剪切",
+        "File": "文件",
+        "Open": "打开",
+        "Save": "保存",
+        "Run": "运行",
+        "Quit": "退出",
+        "Thank you.": "谢谢。",
     },
 }
 
 def get_locale() -> str:
     """get locale"""
     global _locale
     if _locale == "":
```

### Comparing `tkeasygui-0.2.57/TkEasyGUI/utils.py` & `tkeasygui-0.2.63/TkEasyGUI/utils.py`

 * *Files identical despite different names*

### Comparing `tkeasygui-0.2.57/TkEasyGUI/widgets.py` & `tkeasygui-0.2.63/TkEasyGUI/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,31 +73,34 @@
         super().__init__(self.message)
 
 class Window:
     """
     Main window object in TkEasyGUI
     """
     def __init__(
-                self,
-                title: str,
-                layout: list[list[Element]], # set elements layout
-                size: Union[tuple[str, int], None] = None, # window size
-                resizable:bool = False,
-                font: Union[FontType, None] = None,
-                modal: bool = False, # modal window
-                keep_on_top:bool = False, # keep on top
-                no_titlebar: bool = False, # hide titlebar
-                grab_anywhere: bool = False, # can move window by dragging anywhere
-                alpha_channel: float = 1.0, # window alpha channel
-                enable_key_events: bool = False, # enable keyboard events
-                return_keyboard_events: bool = False, # enable keyboard events (for compatibility)
-                location: Union[tuple[int, int], None] = None, # window location
-                center_window: bool = True, # move window to center
-                row_padding: int = 2, # row padding
-                **kw) -> None:
+        self,
+        title: str,
+        layout: list[list[Element]],  # set elements layout
+        size: Union[tuple[str, int], None] = None,  # window size
+        resizable: bool = False,
+        font: Union[FontType, None] = None,
+        modal: bool = False,  # modal window
+        keep_on_top: bool = False,  # keep on top
+        no_titlebar: bool = False,  # hide titlebar
+        grab_anywhere: bool = False,  # can move window by dragging anywhere
+        alpha_channel: float = 1.0,  # window alpha channel
+        enable_key_events: bool = False,  # enable keyboard events
+        return_keyboard_events: bool = False,  # enable keyboard events (for compatibility)
+        location: Union[tuple[int, int], None] = None,  # window location
+        center_window: bool = True,  # move window to center
+        row_padding: int = 2, # row padding
+        padding_x: int = 8, # x padding around the window
+        padding_y: int = 8, # y padding around the window 
+        **kw,
+    ) -> None:
         """Create a window with a layout of widgets."""
         self.modal: bool = modal
         # check active window
         active_win = utils._get_active_window()
         if active_win is None:
             active_win = get_root_window()
         self.window: tk.Toplevel = tk.Toplevel(master=active_win)
@@ -124,33 +127,34 @@
         self._mouse_x: Union[int, None] = None
         self._mouse_y: Union[int, None] = None
         self.alpha_channel: float = alpha_channel
         self.enable_key_events: bool = enable_key_events
         self.return_keyboard_events: bool = return_keyboard_events
         self.font_size_average: tuple[int, int] = (12, 10)
         self.row_padding: int = row_padding
+        self.center_window: bool = center_window
         # Frame
-        self.frame: ttk.Frame = ttk.Frame(self.window, padding=10)
-        self.frame.configure(style="TFrame")
+        self.frame: tk.Frame = tk.Frame(self.window)
+        # self.frame.configure(style="TFrame")
         # set window properties
         self.window.title(title)
         self.window.protocol("WM_DELETE_WINDOW", lambda : self._close_handler())
         self.size: Union[tuple[int, int], None] = size
         if size is not None:
             self.set_size(size)
         self.window.resizable(resizable, resizable)
         # create widgets
         self._create_widget(self.frame, layout)
         # pack frame
-        self.frame.pack(expand=True, fill="both")
+        self.frame.pack(expand=True, fill="both", padx=padding_x, pady=padding_y)
         self.frame.rowconfigure(0, weight=1)
         if keep_on_top:
             self.window.attributes("-topmost", True)
         if no_titlebar:
-            self.hide_titlebar(True)
+            self.window.after_idle(self.hide_titlebar, True)
         if grab_anywhere:
             self.set_grab_anywhere(True)
         if alpha_channel < 1.0:
             self.set_alpha_channel(alpha_channel)
         # font
         self._calc_font_size(font)
         # bind events
@@ -167,28 +171,31 @@
             self.window.attributes("-topmost", 1) # topmost
             # self.window.transient(parent)
             self.window.grab_set()
             self.window.focus_force()
         # push window
         self.parent_window: Union[Window, None] = _window_parent()
         _window_push(self)
+        # set show event
+        self.window.bind("<Map>", self._on_window_show)
         # position
         if location is not None:
             self.set_location(location)
         else:
             # could not get size with geometry() before window is shown
-            if center_window:
-                self.window.bind("<Map>", self._on_window_show)
+            # so, move window to center after window is shown `_on_window_show`
+            pass
 
     def _on_window_show(self, *event) -> None:
         """Handle window show event."""
-        if self.parent_window is None: # only this window
-            self.move_to_center()
-        else:
-            self.move_to_center(center_pos=self.parent_window.get_center_location())
+        if self.center_window:
+            if self.parent_window is None: # only this window
+                self.move_to_center()
+            else:
+                self.move_to_center(center_pos=self.parent_window.get_center_location())
 
     def set_location(self, xy: tuple[int, int]) -> None:
         """Set window location."""
         self.window.geometry(f"+{xy[0]}+{xy[1]}")
     
     def get_location(self) -> tuple[int, int]:
         """Get window location."""
@@ -242,19 +249,30 @@
         # prepare create
         for widgets in layout:
             for elem in widgets:
                 elem.prepare_create(self)
         # create widgets
         self.need_focus_widget: tk.Widget|None = None
         for row_no, widgets in enumerate(layout):
-            # frame_row = ttk.Frame(parent, padding=5, name=f"tkeasygui_frame_row_{row_no}")
-            frame_row = ttk.Frame(parent, padding=self.row_padding ,name=f"tkeasygui_frame_row_{row_no}")
+            bgcolor = None
+            if parent is not None:
+                bgcolor = parent.cget("background")
+            frame_prop = {
+                "name": f"tkeasygui_frame_row_{row_no}",
+                "background": bgcolor
+            }
+            frame_row = tk.Frame(parent, **frame_prop)
             # columns
             prev_element: Element|None = None
-            row_prop: dict[str, Any] = {"expand": False, "fill": "x", "side": valign}
+            row_pack_prop: dict[str, Any] = {
+                "expand": False,
+                "fill": "x",
+                "side": valign,
+                "pady": self.row_padding,
+            }
             # reversed?
             if align == "right":
                 widgets = reversed(widgets)
             for col_no, elemment in enumerate(widgets):
                 # create widget
                 elem: Element = elemment
                 # set window and parent
@@ -304,21 +322,21 @@
                 if isinstance(elem, Menu):
                     continue
                 # pack widget
                 fill_props = elem._get_pack_props(align, valign)
                 widget.pack(**fill_props)
                 # expand_y?
                 if elem.expand_y:
-                    row_prop["expand"] = True
-                    row_prop["fill"] = "both"
+                    row_pack_prop["expand"] = True
+                    row_pack_prop["fill"] = "both"
                 # pady
                 if elem.pady is not None:
-                    row_prop["pady"] = elem.pady
+                    row_pack_prop["pady"] = elem.pady
             # add row
-            frame_row.pack(**row_prop)
+            frame_row.pack(**row_pack_prop)
         # end of create
         if self.need_focus_widget is not None:
             self.need_focus_widget.focus_set()
 
     def _calc_font_size(self, font: FontType) -> None:
         """Calculate font size."""
         font_obj = tkinter_font.Font()
@@ -427,37 +445,41 @@
             # _event_hooks
             if key in self._event_hooks:
                 flag_stop = self._dispatch_event_hooks(key, values)
                 if flag_stop:
                     key = f"{key}-stopped" # change event name
                     values = self.get_values() # collect values again
             # If an event hidden from the user occurs, continue to use the mainloop.
-            if key.endswith("/hide"):
+            if isinstance(key, str) and key.endswith("/hide"):
                 continue # hide system events
             # return a event
             break
         return (key, values)
 
-    def event_iter(self, timeout: Union[int, None] = None, timeout_key: str=TIMEOUT_KEY) -> Any:
+    def event_iter(self, timeout: Union[int, None] = None, timeout_key: str=TIMEOUT_KEY, auto_close: bool=True) -> Any:
         """
         Return generator with event and values
         **Example**
         ```py
         import TkEasyGUI as eg
         # create a window
-        with eg.Window("test", layout=[[eg.Button("Hello")]]) as window:
-            # event loop
-            for event, values in window.event_iter():
-                if event == "Hello":
-                    eg.popup("Hello, World!")
+        window = eg.Window("test", layout=[[eg.Button("Hello")]])
+        # event loop
+        for event, values in window.event_iter():
+            if event == "Hello":
+                eg.popup("Hello, World!")
         ```
        """
+        # event loop
         while self.is_alive():
             event, values = self.read(timeout=timeout, timeout_key=timeout_key)
             yield (event, values)
+        # close window
+        if auto_close:
+            self.close()
     
     def _dispatch_event_hooks(self, key: str, values: dict[str, Any]) -> bool:
         """Dispatch event hooks."""
         # execute _event_hooks
         flag_stop = False
         if key in self._event_hooks:
             for handle in self._event_hooks[key]:
@@ -575,14 +597,18 @@
             self.window.overrideredirect(flag)
             self._no_titlebar = flag
         except Exception:
             pass
 
     def close(self) -> None:
         """Close the window."""
+        # already closed?
+        if not self.flag_alive:
+            return
+        # close window
         try:
             self.flag_alive = False
             _window_pop(self)
             self.window.destroy() # close window
             if _window_count() == 0:
                 self.window.quit() # quit app
         except Exception as e:
@@ -602,16 +628,20 @@
     
     def __getitem__(self, key: str) -> Any:
         """Get an element by its key."""
         return self.key_elements[key]
     
     def show(self) -> None:
         """ Show hidden window (hide -> show)"""
-        self.window.deiconify()
-    
+        # check status
+        if self.is_hidden:
+            self.un_hide()
+        if self.minimized:
+            self.normal()
+
     def refresh(self) -> "Window":
         """Refresh window"""
         try:
             self.window.update()
         except Exception:
             pass
         return self
@@ -1006,14 +1036,18 @@
         # get prev_widget
         return self.prev_element
 
     def __getattr__(self, name: str) -> Any:
         """Get unknown attribute."""
         # Method called when the attribute is not found in the object's instance dictionary
         if self.widget is not None:
+            # Widget
+            if name == "Widget": # for compatibility with PySimpleGUI
+                return self.widget
+            # prop
             if hasattr(self.widget, name):
                 return self.widget.__getattribute__(name)
         return self.__getitem__(name)
 
     def __getitem__(self, name: str) -> Any:
         """Get element property"""
         # For compatibility with PySImpleGUI
@@ -1027,61 +1061,63 @@
             if name in self.widget:
                 return self.widget[name]
         return None
 
 class Frame(Element):
     """Frame element."""
     def __init__(
-                self,
-                title: str,
-                layout: list[list[Element]],
-                key: str = "",
-                size: Union[tuple[int, int], None] = None,
-                relief: ReliefType="groove",
-                # text props
-                font: Union[FontType, None] = None, # font
-                color: Union[str, None] = None,
-                text_color: Union[str, None] = None,
-                background_color: Union[str, None] = None,
-                label_outside: bool=False,
-                vertical_alignment: TextVAlign="top", # vertical alignment
-                text_align: Union[TextAlign, None]="left", # text align
-                # pack props
-                expand_x: bool = False,
-                expand_y: bool = False,
-                pad: Union[PadType, None] = None,
-                # other
-                metadata: Union[dict[str, Any], None] = None,
-                use_ttk: bool=False,
-                **kw) -> None:
+        self,
+        title: str,
+        layout: list[list[Element]],
+        key: str = "",
+        size: Union[tuple[int, int], None] = None,
+        relief: ReliefType = "groove",
+        # text props
+        font: Union[FontType, None] = None,  # font
+        color: Union[str, None] = None,
+        text_color: Union[str, None] = None,
+        background_color: Union[str, None] = None,  # background_color
+        # pack props
+        label_outside: bool = False,
+        vertical_alignment: TextVAlign = "top",  # vertical alignment
+        text_align: Union[TextAlign, None] = "left",  # text align
+        # pack props
+        expand_x: bool = False,
+        expand_y: bool = False,
+        pad: Union[PadType, None] = None,
+        # other
+        metadata: Union[dict[str, Any], None] = None,
+        use_ttk: bool = False,
+        **kw,
+    ) -> None:
         style_name = "TLabelframe" if use_ttk else ""
         super().__init__("Frame", style_name, key, False, metadata, **kw)
         self.has_children = True
         self.layout = layout
         self.label_outside = label_outside
         self.props["text"] = title
         self.props["relief"] = relief
         self.text_align = text_align
         self.vertical_alignment = vertical_alignment
         self._set_text_props(color=color, text_color=text_color, background_color=background_color, font=font)
         self._set_pack_props(expand_x=expand_x, expand_y=expand_y, pad=pad)
         self.use_ttk: bool = use_ttk
-
         if size is not None:
             self.props["size"] = size
 
     def create(self, win: Window, parent: tk.Widget) -> tk.Widget:
         """Create a Frame widget."""
         if self.use_ttk:
             get_ttk_style().configure(self.style_name, labeloutside=self.label_outside)
             self.widget = ttk.LabelFrame(
                 parent,
                 style=self.style_name,
                 **self.props)
         else:
+            # dfault
             self.widget = tk.LabelFrame(parent, **self.props)
         return self.widget
 
     def get(self) -> Any:
         """Return Widget"""
         return self.widget
 
@@ -1323,15 +1359,15 @@
         tooltip: Union[str, None] = None,  # (TODO) tooltip
         button_color: Union[str, tuple[str, str], None] = None,
         # text props
         text_align: Union[TextAlign, None] = "left",  # text align
         font: Union[FontType, None] = None,  # font
         color: Union[str, None] = None,  # text color
         text_color: Union[str, None] = None,  # same as color
-        background_color: Union[str, None] = None,  # background color
+        background_color: Union[str, None] = None,  # background color (not supported on macOS)
         # pack props
         expand_x: bool = False,
         expand_y: bool = False,
         pad: Union[PadType, None] = None,
         # other
         use_ttk_buttons: bool = False,
         metadata: Union[dict[str, Any], None] = None,
@@ -2975,15 +3011,16 @@
         # popup
         result = dialogs.popup_color(
             title=self.title,
             default_color=self.default_color,
         )
         if (target is not None) and (result is not None) and (result != ""):
             target.update(result)
-            self.window._event_handler(self.key, {"event": result, "event_type": "change"})
+            if self.enable_events:
+                self.window._event_handler(self.key, {"event": result, "event_type": "change"})
         return result
 
 class ListBrowse(FileBrowse):
     """ListBrowse element."""
 
     def __init__(
         self,
@@ -3016,17 +3053,16 @@
             items=self.items,
             message=self.message,
             title=self.title,
             font=self.font,
         )
         if (target is not None) and (result is not None) and (result != ""):
             target.update(result)
-            self.window._event_handler(
-                self.key, {"event": result, "event_type": "change"}
-            )
+            if self.enable_events:
+                self.window._event_handler(self.key, {"event": result, "event_type": "change"})
         return result
 
 class MultilineBrowse(FileBrowse):
     """MultilineBrowse element."""
 
     def __init__(
         self,
@@ -3058,17 +3094,18 @@
             title=self.title,
             font=self.font,
         )
         if (target is not None) and (result is not None) and (result != ""):
             result = result.replace("\r", "")
             result = result.replace("\n", "\\n")
             target.update(result)
-            self.window._event_handler(
-                self.key, {"event": result, "event_type": "change"}
-            )
+            if self.enable_events:
+                self.window._event_handler(
+                    self.key, {"event": result, "event_type": "change"}
+                )
         return result
 
 
 def rgb(r: int, g: int, b: int) -> str:
     """Convert RGB to Hex"""
     r = r & 0xFF
     g = g & 0xFF
```

### Comparing `tkeasygui-0.2.57/TkEasyGUI.egg-info/PKG-INFO` & `tkeasygui-0.2.63/TkEasyGUI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TkEasyGUI
-Version: 0.2.57
+Version: 0.2.63
 Summary: TkEasyGUI is simple GUI Library for Python3 with Tkinter
 Author-email: kujirahand <web@kujirahand.com>
 Maintainer-email: kujirahand <web@kujirahand.com>
 License: MIT License
         
         Copyright (c) 2024 kujirahand
         
@@ -83,16 +83,16 @@
 
 ## How to use - popup dialogs
 
 Using TkEasyGUI is simple. If you only want to display a dialog, it requires just two lines of code.
 
 ```py
 import TkEasyGUI as eg
-eg.print("A joyful heart is good medicine.") # popup message
-eg.popup("A joyful heart is good medicine.") # same as eg.print function
+# Displays the message in a popup dialog.
+eg.print("A joyful heart is good medicine.")
 ```
 
 Ask the user for their name and display that name in the window.
 
 ```py
 import TkEasyGUI as eg
 name = eg.input("What is your name?")
@@ -102,38 +102,40 @@
 ### How to use - widgets
 
 To create a simple window with only labels and buttons, you would write as follows:
 
 ```py
 import TkEasyGUI as eg
 # define layout
-layout = [[eg.Text("Hello, World!")],
-          [eg.Button("Exit")]]
+layout = [
+    [eg.Text("Hello, World!")],
+    [eg.Button("OK")]
+]
 # create a window
-with eg.Window("test", layout) as window:
-    # event loop
-    for event, values in window.event_iter():
-        if event == "Exit":
-            eg.popup("Thank you.")
-            break
+window = eg.Window("Hello App", layout)
+# event loop
+for event, values in window.event_iter():
+    if event == "OK":
+        eg.print("Thank you.")
+        break
 ```
 
 You can describe it using an event model similar to the famous GUI library, PySimpleGUI.
 
 ```py
 import TkEasyGUI as eg
+
 # define layout
-layout = [[eg.Text("Hello, World!")],
-          [eg.Button("Exit")]]
+layout = [[eg.Text("Hello, World!")], [eg.Button("OK")]]
 # create a window
-window = eg.Window("test", layout)
+window = eg.Window("Hello App", layout)
 # event loop
 while True:
     event, values = window.read()
-    if event in ["Exit", eg.WINDOW_CLOSED]:
+    if event in ["OK", eg.WINDOW_CLOSED]:
         eg.popup("Thank you.")
         break
 # close window
 window.close()
 ```
 
 ## Samples
```

### Comparing `tkeasygui-0.2.57/pyproject.toml` & `tkeasygui-0.2.63/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TkEasyGUI"
-version = "0.2.57"
+version = "0.2.63"
 dependencies = [
   "Pillow",
   "pyperclip",
 ]
 requires-python = ">=3.9"
 authors = [
   { name="kujirahand", email="web@kujirahand.com" },
```

