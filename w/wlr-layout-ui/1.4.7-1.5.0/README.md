# Comparing `tmp/wlr_layout_ui-1.4.7.tar.gz` & `tmp/wlr_layout_ui-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wlr_layout_ui-1.4.7.tar", max compression
+gzip compressed data, was "wlr_layout_ui-1.5.0.tar", max compression
```

## Comparing `wlr_layout_ui-1.4.7.tar` & `wlr_layout_ui-1.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1070 2024-04-08 16:08:47.075411 wlr_layout_ui-1.4.7/LICENSE
--rw-r--r--   0        0        0      558 2024-03-30 19:04:20.505512 wlr_layout_ui-1.4.7/README.md
--rw-r--r--   0        0        0      652 2024-04-12 17:31:06.974882 wlr_layout_ui-1.4.7/pyproject.toml
--rw-r--r--   0        0        0     2435 2024-02-19 21:26:30.823859 wlr_layout_ui-1.4.7/src/wlr_layout_ui/__init__.py
--rw-r--r--   0        0        0     4304 2023-12-20 15:42:38.511785 wlr_layout_ui-1.4.7/src/wlr_layout_ui/displaywidget.py
--rw-r--r--   0        0        0      387 2024-03-30 19:04:20.505512 wlr_layout_ui-1.4.7/src/wlr_layout_ui/factories.py
--rw-r--r--   0        0        0    21897 2024-04-01 15:30:20.126238 wlr_layout_ui-1.4.7/src/wlr_layout_ui/gui.py
--rw-r--r--   0        0        0      469 2023-10-24 21:30:47.569956 wlr_layout_ui-1.4.7/src/wlr_layout_ui/profiles.py
--rw-r--r--   0        0        0     5475 2024-04-08 16:08:47.075411 wlr_layout_ui-1.4.7/src/wlr_layout_ui/screens.py
--rw-r--r--   0        0        0      274 2024-04-08 23:21:29.224449 wlr_layout_ui-1.4.7/src/wlr_layout_ui/settings.py
--rw-r--r--   0        0        0     1706 2024-03-30 19:04:20.505512 wlr_layout_ui-1.4.7/src/wlr_layout_ui/shapes.py
--rw-r--r--   0        0        0     4496 2024-03-30 19:09:30.198398 wlr_layout_ui-1.4.7/src/wlr_layout_ui/utils.py
--rw-r--r--   0        0        0    12366 2024-03-30 19:04:20.505512 wlr_layout_ui-1.4.7/src/wlr_layout_ui/widgets.py
--rw-r--r--   0        0        0     1323 1970-01-01 00:00:00.000000 wlr_layout_ui-1.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-08 16:08:47.075411 wlr_layout_ui-1.5.0/LICENSE
+-rw-r--r--   0        0        0      558 2024-03-30 19:04:20.505512 wlr_layout_ui-1.5.0/README.md
+-rw-r--r--   0        0        0      652 2024-04-24 21:02:22.985325 wlr_layout_ui-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2435 2024-02-19 21:26:30.823859 wlr_layout_ui-1.5.0/src/wlr_layout_ui/__init__.py
+-rw-r--r--   0        0        0     4249 2024-04-24 19:45:02.396301 wlr_layout_ui-1.5.0/src/wlr_layout_ui/displaywidget.py
+-rw-r--r--   0        0        0      387 2024-03-30 19:04:20.505512 wlr_layout_ui-1.5.0/src/wlr_layout_ui/factories.py
+-rw-r--r--   0        0        0    23746 2024-04-24 21:01:33.060987 wlr_layout_ui-1.5.0/src/wlr_layout_ui/gui.py
+-rw-r--r--   0        0        0      469 2023-10-24 21:30:47.569956 wlr_layout_ui-1.5.0/src/wlr_layout_ui/profiles.py
+-rw-r--r--   0        0        0     5542 2024-04-24 19:21:05.917645 wlr_layout_ui-1.5.0/src/wlr_layout_ui/screens.py
+-rw-r--r--   0        0        0      274 2024-04-08 23:21:29.224449 wlr_layout_ui-1.5.0/src/wlr_layout_ui/settings.py
+-rw-r--r--   0        0        0     1706 2024-03-30 19:04:20.505512 wlr_layout_ui-1.5.0/src/wlr_layout_ui/shapes.py
+-rw-r--r--   0        0        0     4525 2024-04-24 20:29:33.972898 wlr_layout_ui-1.5.0/src/wlr_layout_ui/utils.py
+-rw-r--r--   0        0        0    12366 2024-03-30 19:04:20.505512 wlr_layout_ui-1.5.0/src/wlr_layout_ui/widgets.py
+-rw-r--r--   0        0        0     1323 1970-01-01 00:00:00.000000 wlr_layout_ui-1.5.0/PKG-INFO
```

### Comparing `wlr_layout_ui-1.4.7/LICENSE` & `wlr_layout_ui-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.4.7/README.md` & `wlr_layout_ui-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.4.7/pyproject.toml` & `wlr_layout_ui-1.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wlr-layout-ui"
-version = "1.4.7"
+version = "1.5.0"
 description = "A tiny GUI to configure screen layouts on wayland"
 authors = ["fdev31 <fdev31@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/fdev31/wlr-layout-ui"
 packages = [{include = "wlr_layout_ui", from = "src"}]
 license = "MIT"
```

### Comparing `wlr_layout_ui-1.4.7/src/wlr_layout_ui/__init__.py` & `wlr_layout_ui-1.5.0/src/wlr_layout_ui/__init__.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.4.7/src/wlr_layout_ui/displaywidget.py` & `wlr_layout_ui-1.5.0/src/wlr_layout_ui/displaywidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,29 +122,26 @@
             font_size=16,
             color=(240, 240, 240, 255),
         ).draw()
 
         # Second caption line
         if self.screen.active:
             assert self.screen.mode
-            label = "%dx%d" % (
-                self.screen.mode.width,
-                self.screen.mode.height,
-            )
+            label = f"{self.screen.mode.width}x{self.screen.mode.height}"
             Label(
                 label,
                 anchor_x="center",
                 anchor_y="center",
                 x=tx,
                 y=ty + 20,
                 color=txt_color,
                 bold=self.screen.active,
             ).draw()
             Label(
-                "%dHz" % self.screen.mode.freq,
+                f"{self.screen.mode.freq}Hz",
                 anchor_x="center",
                 anchor_y="center",
                 x=tx,
                 y=ty - 20,
                 color=txt_color,
                 bold=self.screen.active,
             ).draw()
```

### Comparing `wlr_layout_ui-1.4.7/src/wlr_layout_ui/gui.py` & `wlr_layout_ui-1.5.0/src/wlr_layout_ui/gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,27 @@
 from .utils import sorted_resolutions, sorted_frequencies, find_matching_mode
 from .utils import compute_bounding_box, trim_rects_flip_y, make_command, Rect
 from .profiles import save_profile, load_profiles
 from .screens import displayInfo, load
 
 hex_re = re.compile("^[0-9x]+$")
 
-CONFIRM_DELAY = 10
+CONFIRM_DELAY = 20
+
+
+def get_size(screen, scale=0):
+    "Get the size of the window based on the screen size and UI_RATIO"
+    if not scale:
+        scale = UI_RATIO
+    w, h = ((screen.mode.width / scale) / screen.scale), (
+        (screen.mode.height / scale) / screen.scale
+    )
+    if screen.transform in (1, 3, 5, 7):
+        return (h, w)
+    return (w, h)
 
 
 class UI(pyglet.window.Window):
     def __init__(self, width, height):
         super().__init__(width, height, PROG_NAME, resizable=True)
         self.selected_item = None
         self.scale_factor = 1
@@ -97,26 +109,43 @@
         self.freqs = Dropdown(
             ref_rect.copy(),
             label="Rate",
             options=[],
             onchange=self.action_update_mode,
             # invert=True,
         )
-        ref_rect.width //= 3
+        ref_rect.width //= 2
+        self.rotation = Dropdown(
+            ref_rect.copy(),
+            label="Rotation",
+            options=[
+                {"name": "0", "value": 0},
+                {"name": "90", "value": 1},
+                {"name": "180", "value": 2},
+                {"name": "270", "value": 3},
+                {"name": "flip", "value": 4},
+                {"name": "flip 90", "value": 5},
+                {"name": "flip 180", "value": 6},
+                {"name": "flip 270", "value": 7},
+            ],
+            onchange=self.action_update_rotation,
+            # invert=True,
+        )
+        ref_rect.width //= 2
         self.on_off_but = Button(
             ref_rect.copy(),
             label="On",
             toggled_label="Off",
             action=self.action_toggle_screen_power,
             style=Style(highlight=(200, 100, 150), color=(100, 200, 150)),
             togglable=True,
         )
 
         self.settings_box = HBox(
-            widgets=[self.resolutions, self.freqs, self.on_off_but]
+            widgets=[self.resolutions, self.freqs, self.rotation, self.on_off_but]
         )
         self.require_selected_item.add(self.settings_box)
         # }}}
 
         self._widgets: list[Widget] = [
             self.action_box,
             self.settings_box,
@@ -171,29 +200,42 @@
         for screen in sorted(displayInfo, key=lambda s: s.uid):
             # Get the position and mode width and height for this screen
             x, y = screen.position
 
             max_width = max(m.width for m in screen.available)
             max_height = max(m.height for m in screen.available)
 
+            is_rotated = screen.transform in (1, 3, 5, 7)
+
             if screen.mode:
-                h = int(screen.mode.height / UI_RATIO / screen.scale)
+
+                w, h = get_size(screen)
+                h = int(
+                    (screen.mode.height if is_rotated else screen.mode.height)
+                    / UI_RATIO
+                    / screen.scale
+                )
+                if is_rotated:
+                    y -= screen.mode.height - screen.mode.width
+
                 rect = Rect(
                     int(x / UI_RATIO),
                     -int(y / UI_RATIO) - h,
                     int((screen.mode.width / UI_RATIO) / screen.scale),
                     h,
                 )
             else:
                 rect = Rect(
                     int(x / UI_RATIO),
                     int(y / UI_RATIO),
                     int((max_width / UI_RATIO) / screen.scale),
                     int((max_height / UI_RATIO) / screen.scale),
                 )
+            if is_rotated:
+                rect.width, rect.height = rect.height, rect.width
             gs = GuiScreen(screen, rect)
             gs.genColor()
             gui_screens.append(gs)
 
         max_x = max(s.rect.right for s in gui_screens)
         min_x = min(s.rect.left for s in gui_screens)
         min_y = min(s.rect.top for s in gui_screens)
@@ -507,14 +549,15 @@
                     "active": gs.screen.active,
                     "width": gs.screen.mode.width,
                     "height": gs.screen.mode.height,
                     "freq": gs.screen.mode.freq,
                     "x": rect.x,
                     "y": rect.y,
                     "uid": gs.screen.uid,
+                    "transform": gs.screen.transform,
                 }
             )
         return ret
 
     def action_save_new_profile(self):
         assert self.text_input
         save_profile(self.text_input, self.get_profile_data())
@@ -541,23 +584,20 @@
                     return screen
 
         for screen_info in self.profile_list.get_value():
             # try to match screen info with current screens & update accordingly
             found = findScreen(screen_info["uid"])
             if found:
                 info = screen_info.copy()
-                rect = Rect(
-                    info["x"],
-                    -info["y"] - info["height"],
-                    info["width"],
-                    info["height"],
-                )
+                w, h = get_size(found.screen, scale=1)
+                rect = Rect(info["x"], -info["y"] - h, w, h)
                 srect = rect.scaled(1 / UI_RATIO)
                 info.pop("uid")
                 found.screen.active = info.pop("active")
+                found.screen.transform = info.get("transform", 0)
                 found.screen.mode = find_matching_mode(
                     found.screen.available,
                     (info["width"], info["height"]),
                     info["freq"],
                 )
                 found.target_rect = srect
         self.center_layout()
@@ -576,23 +616,32 @@
 
     def action_save_layout(self):
         cmd = make_command(
             [s.screen for s in self.gui_screens],
             [s.rect.scaled(UI_RATIO) for s in self.gui_screens],
             not LEGACY,
         )
+        print(cmd)
         if os.system(cmd):
             self.set_error("Failed applying the layout")
 
         self.confirmation_needed = time.time()
 
     def action_toggle_screen_power(self):
         if self.selected_item:
             self.selected_item.screen.active = not self.selected_item.screen.active
 
+    def action_update_rotation(self):
+        "Update the rotation of the selected screen"
+        assert self.selected_item
+        self.selected_item.screen.transform = self.rotation.get_value()
+        self.selected_item.target_rect.width, self.selected_item.target_rect.height = (
+            get_size(self.selected_item.screen)
+        )
+
     def action_update_screen_spec(self):
         self.action_update_frequencies(self.selected_item, self.resolutions.get_value())
         self.action_update_mode()
         self.center_layout()
 
     def action_update_mode(self):
         assert self.selected_item
@@ -617,10 +666,11 @@
             {"name": f"{r[0]} x {r[1]}", "value": r} for r in res
         ]
         i = -1
         for i, r in enumerate(res):
             if r[0] == cur_mode.width and r[1] == cur_mode.height:
                 break
         self.resolutions.selected_index = i
+        self.rotation.selected_index = screen.screen.transform
         self.action_update_frequencies(screen)
 
     # }}}
```

### Comparing `wlr_layout_ui-1.4.7/src/wlr_layout_ui/screens.py` & `wlr_layout_ui-1.5.0/src/wlr_layout_ui/screens.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     uid: str
     name: str
     active: bool = False
     position: Tuple[int, int] = (0, 0)
     mode: None | Mode = None
     scale: float = 1
     available: list[Mode] = field(default_factory=list)
+    transform: int = 0
 
     def __repr__(self):
         return "<Screen%s %s [%s]>" % ("*" if self.active else "", self.name, self.mode)
 
 
 displayInfo: list[Screen] = []
 
@@ -65,14 +66,15 @@
             uid=monitor["name"],
             name=monitor["description"],
             active=monitor["activeWorkspace"]["id"] >= 0,
             scale=monitor["scale"],
             position=(monitor["x"], monitor["y"]),
             available=modes,
             mode=modes[idx],
+            transform=monitor["transform"],
         )
         displayInfo.append(current_screen)
 
 
 def load():
 
     if displayInfo:
```

### Comparing `wlr_layout_ui-1.4.7/src/wlr_layout_ui/shapes.py` & `wlr_layout_ui-1.5.0/src/wlr_layout_ui/shapes.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.4.7/src/wlr_layout_ui/utils.py` & `wlr_layout_ui-1.5.0/src/wlr_layout_ui/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     command = ['hyprctl --batch "']
 
     for screen, rect in zip(screens, screens_rect):
         if not screen.active:
             command.append(f"keyword monitor {screen.uid},disable ;")
             continue
         command.append(
-            f"keyword monitor {screen.uid},{screen.mode},{int(rect.x)}x{int(rect.y)},{screen.scale} ;"
+            f"keyword monitor {screen.uid},{screen.mode},{int(rect.x)}x{int(rect.y)},{screen.scale},transform,{screen.transform} ;"
         )
 
     cmd = " ".join(command + ['"'])
     return cmd
 
 
 def make_command_legacy(screens, rects, wayland=False):
```

### Comparing `wlr_layout_ui-1.4.7/src/wlr_layout_ui/widgets.py` & `wlr_layout_ui-1.5.0/src/wlr_layout_ui/widgets.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.4.7/PKG-INFO` & `wlr_layout_ui-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wlr-layout-ui
-Version: 1.4.7
+Version: 1.5.0
 Summary: A tiny GUI to configure screen layouts on wayland
 Home-page: https://github.com/fdev31/wlr-layout-ui
 License: MIT
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

