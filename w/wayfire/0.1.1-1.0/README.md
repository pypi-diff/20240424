# Comparing `tmp/wayfire-0.1.1.tar.gz` & `tmp/wayfire-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wayfire-0.1.1.tar", last modified: Sat Mar 30 15:21:06 2024, max compression
+gzip compressed data, was "wayfire-1.0.tar", last modified: Wed Apr 24 15:41:29 2024, max compression
```

## Comparing `wayfire-0.1.1.tar` & `wayfire-1.0.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:21:06.507492 wayfire-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-03-30 15:21:06.507492 wayfire-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-03-30 15:21:02.000000 wayfire-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-30 15:21:02.000000 wayfire-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 15:21:06.507492 wayfire-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:21:06.507492 wayfire-0.1.1/wayfire/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 15:21:02.000000 wayfire-0.1.1/wayfire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54104 2024-03-30 15:21:02.000000 wayfire-0.1.1/wayfire/ipc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:21:06.507492 wayfire-0.1.1/wayfire/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-03-30 15:21:02.000000 wayfire-0.1.1/wayfire/tests/gtk4_window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 15:21:06.507492 wayfire-0.1.1/wayfire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-03-30 15:21:06.000000 wayfire-0.1.1/wayfire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-30 15:21:06.000000 wayfire-0.1.1/wayfire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 15:21:06.000000 wayfire-0.1.1/wayfire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-30 15:21:06.000000 wayfire-0.1.1/wayfire.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:41:29.374029 wayfire-1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-24 15:41:25.000000 wayfire-1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-24 15:41:29.370029 wayfire-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-24 15:41:25.000000 wayfire-1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-24 15:41:25.000000 wayfire-1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:41:29.374029 wayfire-1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:41:29.370029 wayfire-1.0/wayfire/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:41:25.000000 wayfire-1.0/wayfire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79702 2024-04-24 15:41:25.000000 wayfire-1.0/wayfire/ipc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:41:29.370029 wayfire-1.0/wayfire/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-24 15:41:25.000000 wayfire-1.0/wayfire/tests/gtk3_dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-24 15:41:25.000000 wayfire-1.0/wayfire/tests/gtk3_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-24 15:41:25.000000 wayfire-1.0/wayfire/tests/layershell.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-24 15:41:25.000000 wayfire-1.0/wayfire/tests/wayfire.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:41:29.370029 wayfire-1.0/wayfire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-24 15:41:29.000000 wayfire-1.0/wayfire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-24 15:41:29.000000 wayfire-1.0/wayfire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:41:29.000000 wayfire-1.0/wayfire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 15:41:29.000000 wayfire-1.0/wayfire.egg-info/top_level.txt
```

### Comparing `wayfire-0.1.1/PKG-INFO` & `wayfire-1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wayfire
-Version: 0.1.1
+Version: 1.0
 Summary: wayfire compositor library
 Author-email: Thiago <systemofdown@gmail.com>
 Project-URL: Homepage, https://github.com/killown/waypy
 Project-URL: Issues, https://github.com/killown/waypy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
```

### Comparing `wayfire-0.1.1/README.md` & `wayfire-1.0/README.md`

 * *Files identical despite different names*

### Comparing `wayfire-0.1.1/wayfire/ipc.py` & `wayfire-1.0/wayfire/ipc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,60 @@
 import socket
 import json as js
+import requests
 import os
-from subprocess import call
+from subprocess import call, Popen, check_output, run, PIPE
 from itertools import cycle
 import dbus
 import configparser
+from configparser import ConfigParser
 from itertools import filterfalse
 import time
-from random import randint, choice, random
+from random import randint, choice, random, sample
 import threading
+import psutil
+import pkg_resources
+
+from ctypes import CDLL
+
+CDLL("libgtk4-layer-shell.so")
+
+
+def check_geometry(x: int, y: int, width: int, height: int, obj) -> bool:
+    if (
+        obj["x"] == x
+        and obj["y"] == y
+        and obj["width"] == width
+        and obj["height"] == height
+    ):
+        return True
+    return False
+
+
+def extract_socket_name(file_path):
+    with open(file_path, "r") as file:
+        for line in file:
+            if "Using socket name" in line:
+                parts = line.split()
+                return parts[-1].strip()
+
+
+def find_wayland_display(pid):
+    try:
+        process = psutil.Process(pid)
+        for fd in process.open_files():
+            if "wayland-" in fd.path:
+                display = fd.path.split("-")[-1]
+                if "." in display:
+                    display = display.split(".")[0]
+                return f"wayland-{display}"
+    except (psutil.NoSuchProcess, psutil.AccessDenied):
+        pass
+
+    return None
 
 
 def get_msg_template(method: str, methods=None):
     plugin = None
     # just in case there is a unknow situation where the method has no plugin
     if "/" in method:
         plugin = method.split("/")[0]
@@ -44,38 +86,42 @@
     geometry["width"] = w
     geometry["height"] = h
     return geometry
 
 
 class WayfireSocket:
     def __init__(self, socket_name):
-        self.client = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
-
+        self.client = None
         # if socket_name is empity, we need a workaround to set it
         # that happens when the compositor has no views in the workspace
         # so WAYFIRE_SOCKET env is not set
         if socket_name is None:
             # the last item is the most recent socket file
             socket_list = sorted(
                 [
                     os.path.join("/tmp", i)
                     for i in os.listdir("/tmp")
                     if "wayfire-wayland" in i
                 ]
             )
             for sock in socket_list:
                 try:
-                    self.client.connect(sock)
+                    self.connect_client(sock)
                     break
                 except Exception as e:
                     print(e)
         else:
-            self.client.connect(socket_name)
-        # initialize it once for performance in some cases
-        self.methods = self.list_methods()
+            # initialize it once for performance in some cases
+            self.connect_client(socket_name)
+            self.methods = self.list_methods()
+            self.socket_name = socket_name
+
+    def connect_client(self, socket_name):
+        self.client = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
+        self.client.connect(socket_name)
 
     def read_exact(self, n):
         response = bytes()
         while n > 0:
             read_this_time = self.client.recv(n)
             if not read_this_time:
                 raise Exception("Failed to read anything from the socket!")
@@ -88,14 +134,183 @@
         rlen = int.from_bytes(self.read_exact(4), byteorder="little")
         response_message = self.read_exact(rlen)
         response = js.loads(response_message)
         if "error" in response:
             raise Exception(response["error"])
         return response
 
+    def create_wayland_output(self):
+        message = get_msg_template("stipc/create_wayland_output", self.methods)
+        self.send_json(message)
+
+    def create_headless_output(self, width, height):
+        message = get_msg_template("wayfire/create-headless-output")
+        message["data"]["width"] = width
+        message["data"]["height"] = height
+        return self.send_json(message)
+
+    def destroy_headless_output(self, output_name=None, output_id=None):
+        assert output_name is not None or output_id is not None
+        message = get_msg_template("wayfire/destroy-headless-output", self.methods)
+        if output_name is not None:
+            message["data"]["output"] = output_name
+        else:
+            message["data"]["output-id"] = output_id
+
+        return self.send_json(message)
+
+    def register_binding(
+        self,
+        binding: str,
+        call_method=None,
+        call_data=None,
+        command=None,
+        mode=None,
+        exec_always=False,
+    ):
+        message = get_msg_template("command/register-binding")
+        message["data"]["binding"] = binding
+        message["data"]["exec-always"] = exec_always
+        if mode and mode != "press" and mode != "normal":
+            message["data"]["mode"] = mode
+
+        if call_method is not None:
+            message["data"]["call-method"] = call_method
+        if call_data is not None:
+            message["data"]["call-data"] = call_data
+        if command is not None:
+            message["data"]["command"] = command
+
+        return self.send_json(message)
+
+    def unregister_binding(self, binding_id: int):
+        message = get_msg_template("command/unregister-binding")
+        message["data"]["binding-id"] = binding_id
+        return self.send_json(message)
+
+    def clear_bindings(self):
+        message = get_msg_template("command/clear-bindings")
+        return self.send_json(message)
+
+    def get_option_value(self, option):
+        message = get_msg_template("wayfire/get-config-option")
+        message["data"]["option"] = option
+        return self.send_json(message)
+
+    def set_option_values(self, options):
+        sanitized_options = {}
+        for key, value in options.items():
+            if "/" in key:
+                sanitized_options[key] = value
+            else:
+                for option_name, option_value in value.items():
+                    sanitized_options[key + "/" + option_name] = option_value
+
+        message = get_msg_template("wayfire/set-config-options")
+        print(js.dumps(sanitized_options, indent=4))
+        message["data"] = sanitized_options
+        return self.send_json(message)
+
+    def layout_views(self, layout):
+        views = self.list_views()
+        method = "stipc/layout_views"
+        message = get_msg_template(method, self.methods)
+        msg_layout = []
+
+        for ident in layout:
+            x, y, w, h = layout[ident][:4]
+            for v in views:
+                if v["app-id"] == ident or v["title"] == ident or v["id"] == ident:
+                    layout_for_view = {
+                        "id": v["id"],
+                        "x": x,
+                        "y": y,
+                        "width": w,
+                        "height": h,
+                    }
+                    if len(layout[ident]) == 5:
+                        layout_for_view["output"] = layout[ident][-1]
+                    msg_layout.append(layout_for_view)
+
+        message["data"]["views"] = msg_layout
+        return self.send_json(message)
+
+    def set_touch(self, id: int, x: int, y: int):
+        method = "stipc/touch"
+        message = get_msg_template(method, self.methods)
+        message["data"]["finger"] = id
+        message["data"]["x"] = x
+        message["data"]["y"] = y
+        return self.send_json(message)
+
+    def tablet_tool_proximity(self, x, y, prox_in):
+        method = "stipc/tablet/tool_proximity"
+        message = get_msg_template(method, self.methods)
+        message["data"]["x"] = x
+        message["data"]["y"] = y
+        message["data"]["proximity_in"] = prox_in
+        return self.send_json(message)
+
+    def tablet_tool_tip(self, x, y, state):
+        method = "stipc/tablet/tool_tip"
+        message = get_msg_template(method, self.methods)
+        message["data"]["x"] = x
+        message["data"]["y"] = y
+        message["data"]["state"] = state
+        return self.send_json(message)
+
+    def tablet_tool_axis(self, x, y, pressure):
+        method = "stipc/tablet/tool_axis"
+        message = get_msg_template(method, self.methods)
+        message["data"]["x"] = x
+        message["data"]["y"] = y
+        message["data"]["pressure"] = pressure
+        return self.send_json(message)
+
+    def tablet_tool_button(self, btn, state):
+        method = "stipc/tablet/tool_button"
+        message = get_msg_template(method, self.methods)
+        message["data"]["button"] = btn
+        message["data"]["state"] = state
+        return self.send_json(message)
+
+    def tablet_pad_button(self, btn, state):
+        method = "stipc/tablet/pad_button"
+        message = get_msg_template(method, self.methods)
+        message["data"]["button"] = btn
+        message["data"]["state"] = state
+        return self.send_json(message)
+
+    def release_touch(self, id: int):
+        method = "stipc/touch_release"
+        message = get_msg_template(method, self.methods)
+        message["data"]["finger"] = id
+        return self.send_json(message)
+
+    def destroy_wayland_output(self, output: str):
+        method = "stipc/destroy_wayland_output"
+        message = get_msg_template(method, self.methods)
+        message["data"]["output"] = output
+        return self.send_json(message)
+
+    def delay_next_tx(self):
+        method = "stipc/delay_next_tx"
+        message = get_msg_template(method, self.methods)
+        return self.send_json(message)
+
+    def xwayland_pid(self):
+        method = "stipc/get_xwayland_pid"
+        message = get_msg_template(method, self.methods)
+        return self.send_json(message)
+
+    def xwayland_display(self):
+        method = "stipc/get_xwayland_display"
+        message = get_msg_template(method, self.methods)
+        return self.send_json(message)
+
     def list_methods(self):
         query = get_msg_template("list-methods")
         response = self.send_json(query)
         data = js.dumps(response["methods"], indent=4)
         data = data.replace("'", '"')
         data_list = js.loads(data)
         return data_list
@@ -109,14 +324,23 @@
         self.client.send(header)
         self.client.send(data)
         return self.read_message()
 
     # this is not a socket IPC thing, but since the compositor developer won't implement
     # dpms for ipc, this tool just works fine
     # this was not intended to be here, but anyways, lets use it
+
+    def dpms_status(self):
+        status = check_output(["wlopm"]).decode().strip().split("\n")
+        dpms_status = {}
+        for line in status:
+            line = line.split()
+            dpms_status[line[0]] = line[1]
+        return dpms_status
+
     def dpms(self, state, output_name=None):
         if state == "off" and output_name is None:
             outputs = [output["name"] for output in self.list_outputs()]
             for output in outputs:
                 call("wlopm --off {}".format(output).split())
         if state == "on" and output_name is None:
             outputs = [output["name"] for output in self.list_outputs()]
@@ -295,28 +519,41 @@
     def run(self, cmd):
         message = get_msg_template("stipc/run", self.methods)
         if message is None:
             return
         message["data"]["cmd"] = cmd
         return self.send_json(message)
 
-    def press_key(self, key: str):
-        if key[:2] == "S-":
-            self.set_key_state("KEY_LEFTMETA", True)
-            self.set_key_state(key[2:], True)
-            self.set_key_state(key[2:], False)
-            self.set_key_state("KEY_LEFTMETA", False)
-        elif key[:2] == "C-":
-            self.set_key_state("KEY_LEFTCTRL", True)
-            self.set_key_state(key[2:], True)
-            self.set_key_state(key[2:], False)
-            self.set_key_state("KEY_LEFTCTRL", False)
-        else:
-            self.set_key_state(key, True)
-            self.set_key_state(key, False)
+    def press_key(self, keys: str, timeout=0):
+        modifiers = {
+            "A": "KEY_LEFTALT",
+            "S": "KEY_LEFTSHIFT",
+            "C": "KEY_LEFTCTRL",
+            "W": "KEY_LEFTMETA",
+        }
+        key_combinations = keys.split("-")
+
+        for modifier in key_combinations[:-1]:
+            if modifier in modifiers:
+                self.set_key_state(modifiers[modifier], True)
+
+        if timeout >= 1:
+            time.sleep(timeout / 1000)
+
+        actual_key = key_combinations[-1]
+        self.set_key_state(actual_key, True)
+
+        if timeout >= 1:
+            time.sleep(timeout / 1000)
+
+        self.set_key_state(actual_key, False)
+
+        for modifier in key_combinations[:-1]:
+            if modifier in modifiers:
+                self.set_key_state(modifiers[modifier], False)
 
     def toggle_showdesktop(self):
         message = get_msg_template("wm-actions/toggle_showdesktop", self.methods)
         if message is None:
             return
         return self.send_json(message)
 
@@ -381,14 +618,19 @@
         return True
 
     def list_outputs_ids(self):
         outputs = self.list_outputs()
         if outputs:
             return [i["id"] for i in outputs]
 
+    def list_outputs_names(self):
+        outputs = self.list_outputs()
+        if outputs:
+            return [i["name"] for i in outputs]
+
     def sum_geometry_resolution(self):
         outputs = sock.list_outputs()
         total_width = 0
         total_height = 0
         for output in outputs:
             total_width += output["geometry"]["width"]
             total_height += output["geometry"]["height"]
@@ -466,23 +708,27 @@
     def set_focus(self, view_id: int):
         message = get_msg_template("window-rules/focus-view")
         if message is None:
             return
         message["data"]["id"] = view_id
         return self.send_json(message)
 
+    def get_active_workspace(self):
+        data = self.get_active_workspace_info()
+        if data:
+            x = data["x"]
+            y = data["y"]
+            return {"x": x, "y": y}
+
     def go_workspace_set_focus(self, view_id):
-        focused_output = self.get_focused_output_id()
-        view_output_id = self.get_view_output_id(view_id)
-        # needed to change the workspace if not the focused output
-        if focused_output != view_output_id:
-            self.set_focus(view_id)
         workspace = self.get_view_workspace(view_id)
+        active_workspace = self.get_active_workspace()
         if workspace:
-            self.set_workspace(workspace)
+            if active_workspace != workspace:
+                self.set_workspace(workspace)
         self.set_focus(view_id)
 
     def get_focused_view(self):
         message = get_msg_template("window-rules/get-focused-view")
         if message is None:
             return
         return self.send_json(message)["info"]
@@ -495,14 +741,26 @@
         view = self.get_focused_view()
         if view is not None:
             view_id = self.get_focused_view()
             if view_id is not None:
                 view_id = view_id["id"]
                 return self.get_view_pid(view_id)
 
+    def has_ouput_fullscreen_view(self, output_id):
+        # any fullscreen doesn't matter from what workspace
+        list_views = self.list_views()
+        if not list_views:
+            return
+        if any(
+            True
+            for i in list_views
+            if i["fullscreen"] is True and i["output-id"] == output_id
+        ):
+            return True
+
     def is_focused_view_fullscreen(self):
         focused_view = self.get_focused_view()
         if focused_view is not None:
             return focused_view.get("fullscreen")
         return None
 
     def get_focused_view_role(self):
@@ -556,16 +814,20 @@
 
     def get_focused_view_app_id(self):
         return self.get_focused_view()["app-id"]
 
     def get_focused_output(self):
         message = get_msg_template("window-rules/get-focused-output")
         if message is None:
-            return
-        return self.send_json(message)["info"]
+            return None
+        message = self.send_json(message)
+        if "info" in message:
+            return message["info"]
+        else:
+            return message
 
     def coordinates_to_number(self, rows, cols, coordinates):
         row, col = coordinates
         if 0 <= row < rows and 0 <= col < cols:
             return row * cols + col + 1
         else:
             return None
@@ -601,14 +863,24 @@
 
     def get_focused_output_id(self):
         focused_output = self.get_focused_output()
         if focused_output is not None:
             return focused_output.get("id")
         return None
 
+    def get_output_id_by_name(self, output_name):
+        for output in self.list_outputs():
+            if output["name"] == output_name:
+                return output["id"]
+
+    def get_output_name_by_id(self, output_id):
+        for output in self.list_outputs():
+            if output["id"] == output_id:
+                return output["name"]
+
     def get_focused_output_geometry(self):
         focused_output = self.get_focused_output()
         if focused_output is not None:
             return focused_output.get("geometry")
         return None
 
     def get_focused_output_workarea(self):
@@ -802,14 +1074,20 @@
 
     def get_view_output_id(self, view_id):
         view = self.get_view(view_id)
         if view is not None:
             return view.get("output-id")
         return None
 
+    def get_view_output_name(self, view_id):
+        view = self.get_view(view_id)
+        if view is not None:
+            return view.get("output-name")
+        return None
+
     def is_view_fullscreen(self, view_id):
         view = self.get_view(view_id)
         if view is not None:
             return view.get("fullscreen")
         return None
 
     def is_view_focusable(self, view_id):
@@ -820,14 +1098,25 @@
 
     def get_view_geometry(self, view_id):
         view = self.get_view(view_id)
         if view is not None:
             return view.get("geometry")
         return None
 
+    def toggle_minimize_from_app_id(self, app_id):
+        list_views = sock.list_views()
+        if not list_views:
+            return
+        ids = [i["id"] for i in list_views if i["app-id"] == app_id]
+        for id in ids:
+            if sock.is_view_minimized(id):
+                sock.set_minimized(id, False)
+            else:
+                sock.set_minimized(id, True)
+
     def is_view_minimized(self, view_id):
         view = self.get_view(view_id)
         if view is not None:
             return view.get("minimized")
         return None
 
     def is_view_maximized(self, view_id):
@@ -910,14 +1199,22 @@
 
     def toggle_expo(self):
         message = get_msg_template("expo/toggle")
         if message is None:
             return
         self.send_json(message)
 
+    def find_view_by_pid(self, pid):
+        lviews = self.list_views()
+        if not lviews:
+            return
+        view = [view for view in lviews if view["pid"] == pid]
+        if view:
+            return view[0]
+
     def find_device_id(self, name_or_id_or_type):
         devices = self.list_input_devices()
         for dev in devices:
             if (
                 dev["name"] == name_or_id_or_type
                 or str(dev["id"]) == name_or_id_or_type
                 or dev["type"] == name_or_id_or_type
@@ -931,16 +1228,152 @@
         return msg
 
     def enable_input_device(self, args):
         device_id = self.find_device_id(args)
         msg = self.configure_input_device(device_id, True)
         return msg
 
+    def get_wayfire_ini_path(self):
+        wayfire_ini_path = os.getenv("WAYFIRE_CONFIG_FILE")
+        if wayfire_ini_path:
+            return wayfire_ini_path
+        else:
+            print("Error: WAYFIRE_CONFIG_FILE environment variable is not set.")
+            return None
+
+    def enable_plugin(self, plugin_name):
+        wayfire_ini_path = self.get_wayfire_ini_path()
+        if not wayfire_ini_path:
+            return
+
+        config = ConfigParser()
+        config.read(wayfire_ini_path)
+
+        if "core" not in config:
+            config["core"] = {}
+
+        plugins = config["core"].get("plugins", "").split()
+
+        if plugin_name in plugins:
+            print(f"Plugin '{plugin_name}' is already enabled in wayfire.ini.")
+            return
+
+        plugins.append(plugin_name)
+        config["core"]["plugins"] = " ".join(plugins)
+
+        with open(wayfire_ini_path, "w") as configfile:
+            config.write(configfile)
+
+        print(f"Plugin '{plugin_name}' enabled successfully in wayfire.ini.")
+
+    def disable_plugin(self, plugin_name):
+        wayfire_ini_path = self.get_wayfire_ini_path()
+        if not wayfire_ini_path:
+            return
+
+        config = ConfigParser()
+        config.read(wayfire_ini_path)
+
+        if "core" not in config:
+            print("Error: 'core' section not found in wayfire.ini.")
+            return
+
+        plugins = config["core"].get("plugins", "").split()
+
+        if plugin_name not in plugins:
+            print(f"Plugin '{plugin_name}' is not enabled in wayfire.ini.")
+            return
+
+        plugins.remove(plugin_name)
+        config["core"]["plugins"] = " ".join(plugins)
+
+        with open(wayfire_ini_path, "w") as configfile:
+            config.write(configfile)
+
+        print(f"Plugin '{plugin_name}' disabled successfully in wayfire.ini.")
+
+    def list_plugins(self):
+        official_url = "https://github.com/WayfireWM/wayfire/tree/master/metadata"
+        extra_url = (
+            "https://github.com/WayfireWM/wayfire-plugins-extra/tree/master/metadata"
+        )
+
+        official_response = requests.get(official_url)
+        extra_response = requests.get(extra_url)
+
+        if official_response.status_code != 200 or extra_response.status_code != 200:
+            print("Failed to fetch content from one or both repositories.")
+            return {}
+
+        official_html_content = official_response.text
+        extra_html_content = extra_response.text
+
+        official_start_index = official_html_content.find(
+            '<script type="application/json" data-target="react-app.embeddedData">'
+        )
+        extra_start_index = extra_html_content.find(
+            '<script type="application/json" data-target="react-app.embeddedData">'
+        )
+
+        official_end_index = official_html_content.find(
+            "</script>", official_start_index
+        )
+        extra_end_index = extra_html_content.find("</script>", extra_start_index)
+
+        official_json_data = official_html_content[
+            official_start_index
+            + len(
+                '<script type="application/json" data-target="react-app.embeddedData">'
+            ) : official_end_index
+        ]
+        extra_json_data = extra_html_content[
+            extra_start_index
+            + len(
+                '<script type="application/json" data-target="react-app.embeddedData">'
+            ) : extra_end_index
+        ]
+
+        official_data = js.loads(official_json_data)
+        extra_data = js.loads(extra_json_data)
+
+        official_plugin_names = [
+            item["name"][:-4]
+            for item in official_data["payload"]["tree"]["items"]
+            if item["contentType"] == "file" and item["name"].endswith(".xml")
+        ]
+        extra_plugin_names = [
+            item["name"][:-4]
+            for item in extra_data["payload"]["tree"]["items"]
+            if item["contentType"] == "file" and item["name"].endswith(".xml")
+        ]
+
+        return {
+            "official-plugins": official_plugin_names,
+            "extra-plugins": extra_plugin_names,
+        }
+
+    def list_enabled_plugins(self):
+        wayfire_ini_path = self.get_wayfire_ini_path()
+        if not wayfire_ini_path:
+            return []
+
+        config = ConfigParser()
+        config.read(wayfire_ini_path)
+
+        if "core" not in config:
+            print("Error: 'core' section not found in wayfire.ini.")
+            return []
+
+        plugins = config["core"].get("plugins", "").split()
+        return plugins
+
     def reload_plugins(self):
-        filename = os.path.expanduser(os.path.join("~", ".config", "wayfire.ini"))
+        filename = self.get_wayfire_ini_path()
+        if not filename:
+            return
 
         config = configparser.ConfigParser()
         config.read(filename)
 
         # Comment out the 'plugins' line
         config["core"]["plugins"] = "# " + config["core"]["plugins"]
 
@@ -956,27 +1389,16 @@
         )
 
         # Save the modified configuration back to the file
         with open(filename, "w") as configfile:
             config.write(configfile)
 
     def reload_plugin(self, plugin_name):
-        filename = os.path.expanduser(os.path.join("~", ".config", "wayfire.ini"))
-        config = configparser.ConfigParser()
-        config.read(filename)
-        if plugin_name in config["core"]["plugins"]:
-            plugins_list = config["core"]["plugins"].split()
-            plugins_list.remove(plugin_name)
-            config["core"]["plugins"] = " ".join(plugins_list)
-            with open(filename, "w") as configfile:
-                config.write(configfile)
-            plugins_list.append(plugin_name)
-            config["core"]["plugins"] = " ".join(plugins_list)
-            with open(filename, "w") as configfile:
-                config.write(configfile)
+        self.disable_plugin(plugin_name)
+        self.enable_plugin(plugin_name)
 
     def maximize(self, view_id):
         self.assign_slot(view_id, "slot_c")
 
     def maximize_all_views_from_active_workspace(self):
         for view_id in self.get_views_from_active_workspace():
             if not self.is_view_fullscreen(view_id):
@@ -1013,14 +1435,28 @@
         return not (
             view["x"] >= workspace_end_x
             or view["y"] > workspace_end_y
             or view["x"] + view["width"] <= workspace_start_x
             or view["y"] + view["height"] <= workspace_start_y
         )
 
+    def get_workspace_from_view(self, view_id):
+        ws_with_views = self.get_workspaces_with_views()
+        for ws in ws_with_views:
+            if ws["view-id"] == view_id:
+                return {"x": ws["x"], "y": ws["y"]}
+
+    def has_workspace_views(self, ws):
+        ws_with_views = self.get_workspaces_with_views()
+        for wwv in ws_with_views:
+            del wwv["view-id"]
+            if wwv == ws:
+                return True
+        return False
+
     def get_workspaces_with_views(self):
         focused_output = self.get_focused_output()
         monitor = focused_output["geometry"]
         ws_with_views = []
         views = self.focused_output_views()
         if views:
             for ws_x in range(focused_output["workspace"]["grid_width"]):
@@ -1320,52 +1756,240 @@
         if message is None:
             return
         message["data"]["x"] = x
         message["data"]["y"] = y
         message["data"]["output-id"] = output_id
         if view_id is not None:
             message["data"]["view-id"] = view_id
-        self.send_json(message)
-        return True
+        return self.send_json(message)
+
+    def find_view_middle_cursor_position(self, view_geometry, monitor_geometry):
+        # Calculate the middle position of the view
+        view_middle_x = view_geometry["x"] + view_geometry["width"] // 2
+        view_middle_y = view_geometry["y"] + view_geometry["height"] // 2
+
+        # Calculate the offset from the monitor's top-left corner
+        cursor_x = monitor_geometry["x"] + view_middle_x
+        cursor_y = monitor_geometry["y"] + view_middle_y
+
+        return cursor_x, cursor_y
+
+    def move_cursor_middle(self, view_id):
+        view = self.get_view(view_id)
+        output_id = view["output-id"]
+        view_geometry = view["geometry"]
+        output_geometry = self.query_output(output_id)["geometry"]
+        cursor_x, cursor_y = self.find_view_middle_cursor_position(
+            view_geometry, output_geometry
+        )
+        self.move_cursor(cursor_x, cursor_y)
+
+    def focus_next_view_from_active_workspace(self):
+        views = self.get_views_from_active_workspace()
+        if views:
+            self.go_workspace_set_focus(views[0])
 
     def configure_input_device(self, id, enabled: bool):
         message = get_msg_template("input/configure-device")
         if message is None:
             return
         message["data"]["id"] = id
         message["data"]["enabled"] = enabled
         return self.send_json(message)
 
+    def get_config_location_from_log(self, file_path):
+        with open(file_path, "r") as file:
+            for line in file:
+                if "Using config file:" in line:
+                    parts = line.split()
+                    return parts[-1].strip()
+
+    def start_nested_wayfire(self, wayfire_ini=None, cmd=None):
+        if wayfire_ini is None:
+            module_dir = pkg_resources.resource_filename(__name__, "")
+            wayfire_ini = os.path.join(module_dir, "tests/wayfire.ini")
+            print("Using config: {}".format(wayfire_ini))
+        logfile = "/tmp/wayfire-nested.log"
+        asan_options = "ASAN_OPTIONS=new_delete_type_mismatch=0:detect_leaks=0:detect_odr_violation=0"
+        sock.run(
+            "{0} wayfire -c {1} -d &>{2}".format(asan_options, wayfire_ini, logfile)
+        )["pid"]
+        time.sleep(1)
+        wayland_display = extract_socket_name(logfile)
+        if cmd is not None:
+            sock.run("WAYLAND_DISPLAY={0} {1}".format(wayland_display, cmd))
+        os.environ["WAYLAND_DISPLAY"] = wayland_display
+        self.socket_name = "/tmp/wayfire-{}.socket".format(wayland_display)
+        print(self.socket_name)
+        print(os.path.exists(self.socket_name))
+        self.connect_client(self.socket_name)
+        return wayland_display
+
+    def test_random_press_key_with_modifiers(self, num_combinations=1):
+        """
+        Randomly generates key combinations and calls press_key function.
+
+        Args:
+            sock: Instance of the class containing the press_key method.
+            num_combinations (int): Number of random key combinations to generate.
+
+        Returns:
+            None
+        """
+        keys = [
+            "KEY_CANCEL",
+            "KEY_HELP",
+            "KEY_BACK_SPACE",
+            "KEY_TAB",
+            "KEY_CLEAR",
+            "KEY_ENTER",
+            "KEY_SHIFT",
+            "KEY_CONTROL",
+            "KEY_ALT",
+            "KEY_PAUSE",
+            "KEY_CAPS_LOCK",
+            "KEY_ESCAPE",
+            "KEY_SPACE",
+            "KEY_PAGE_UP",
+            "KEY_PAGE_DOWN",
+            "KEY_END",
+            "KEY_HOME",
+            "KEY_ARROW_LEFT",
+            "KEY_ARROW_UP",
+            "KEY_ARROW_RIGHT",
+            "KEY_ARROW_DOWN",
+            "KEY_PRINT_SCREEN",
+            "KEY_INSERT",
+            "KEY_DELETE",
+            "KEY_0",
+            "KEY_1",
+            "KEY_2",
+            "KEY_3",
+            "KEY_4",
+            "KEY_5",
+            "KEY_6",
+            "KEY_7",
+            "KEY_8",
+            "KEY_9",
+            "KEY_SEMICOLON",
+            "KEY_EQUALS",
+            "KEY_A",
+            "KEY_B",
+            "KEY_C",
+            "KEY_D",
+            "KEY_E",
+            "KEY_F",
+            "KEY_G",
+            "KEY_H",
+            "KEY_I",
+            "KEY_J",
+            "KEY_K",
+            "KEY_L",
+            "KEY_M",
+            "KEY_N",
+            "KEY_O",
+            "KEY_P",
+            "KEY_Q",
+            "KEY_R",
+            "KEY_S",
+            "KEY_T",
+            "KEY_U",
+            "KEY_V",
+            "KEY_W",
+            "KEY_X",
+            "KEY_Y",
+            "KEY_Z",
+            "KEY_LEFT_WINDOW_KEY",
+            "KEY_RIGHT_WINDOW_KEY",
+            "KEY_SELECT_KEY",
+            "KEY_NUMPAD_0",
+            "KEY_NUMPAD_1",
+            "KEY_NUMPAD_2",
+            "KEY_NUMPAD_3",
+            "KEY_NUMPAD_4",
+            "KEY_NUMPAD_5",
+            "KEY_NUMPAD_6",
+            "KEY_NUMPAD_7",
+            "KEY_NUMPAD_8",
+            "KEY_NUMPAD_9",
+            "KEY_MULTIPLY",
+            "KEY_ADD",
+            "KEY_SEPARATOR",
+            "KEY_SUBTRACT",
+            "KEY_DECIMAL_POINT",
+            "KEY_DIVIDE",
+            "KEY_F1",
+            "KEY_F2",
+            "KEY_F3",
+            "KEY_F4",
+            "KEY_F5",
+            "KEY_F6",
+            "KEY_F7",
+            "KEY_F8",
+            "KEY_F9",
+            "KEY_F10",
+            "KEY_F11",
+            "KEY_F12",
+            "KEY_NUM_LOCK",
+            "KEY_SCROLL_LOCK",
+            "KEY_COMMA",
+            "KEY_PERIOD",
+            "KEY_SLASH",
+            "KEY_BACK_QUOTE",
+            "KEY_OPEN_BRACKET",
+            "KEY_BACK_SLASH",
+            "KEY_CLOSE_BRACKET",
+            "KEY_QUOTE",
+            "KEY_META",
+        ]
+
+        modifiers = ["A-", "S-", "C-"]
+
+        for _ in range(num_combinations):
+            modifier = choice(modifiers)
+            main_key = choice(keys)
+            key_combination = modifier + main_key
+            try:
+                self.press_key(key_combination)
+            except:
+                continue
+
     def test_random_set_view_position(self, view_id):
+        if view_id is None:
+            view_id = self.test_random_view_id()
         actions = [
             self.set_view_top_left,
             self.set_view_top_right,
             self.set_view_bottom_left,
             self.set_view_right,
             self.set_view_left,
             self.set_view_bottom,
             self.set_view_top,
             self.set_view_center,
             self.set_view_bottom_right,
         ]
         choice(actions)(view_id)
 
     def test_random_change_view_state(self, view_id):
+        if view_id is None:
+            view_id = self.test_random_view_id()
         actions = [
             lambda: self.maximize(view_id),
             lambda: self.set_fullscreen(view_id),
             lambda: self.set_minimized(view_id, True),
             lambda: self.set_minimized(view_id, False),
             lambda: self.set_sticky(view_id, choice([True, False])),
             lambda: self.send_to_back(view_id, choice([True, False])),
             lambda: self.set_view_alpha(view_id, random() * 1.0),
         ]
         choice(actions)()
 
     def test_random_list_info(self, view_id):
+        if view_id is None:
+            view_id = self.test_random_view_id()
         actions = [
             self.list_outputs,
             self.list_wsets,
             lambda: self.wset_info(view_id),
             lambda: self.get_view(view_id),
             lambda: self.get_view_info(view_id),
             lambda: self.get_view_alpha(view_id),
@@ -1373,44 +1997,70 @@
             self.get_workspaces_with_views,
             self.get_workspaces_without_views,
             self.get_views_from_active_workspace,
         ]
         choice(actions)()
 
     def test_set_view_position(self, view_id):
+        if view_id is None:
+            view_id = self.test_random_view_id()
         self.set_view_top_left(view_id)
         self.set_view_top_right(view_id)
         self.set_view_bottom_left(view_id)
         self.set_view_right(view_id)
         self.set_view_left(view_id)
         self.set_view_bottom(view_id)
         self.set_view_top(view_id)
         self.set_view_center(view_id)
         self.set_view_bottom_right(view_id)
         self.set_focus(view_id)
 
+    def test_random_view_id(self):
+        ids = self.list_ids()
+        if ids:
+            return choice(ids)
+
     def test_change_view_state(self, view_id):
-        self.maximize(view_id)
-        self.set_fullscreen(view_id)
-        self.set_minimized(view_id, True)
-        self.set_minimized(view_id, False)
-        self.set_sticky(view_id, choice([True, False]))
-        self.send_to_back(view_id, choice([True, False]))
-        self.set_view_alpha(view_id, random() * 1.0)
-        self.set_focus(view_id)
+        if view_id is None:
+            view_id = self.test_random_view_id()
+        actions = [
+            lambda: self.maximize(view_id),
+            lambda: self.set_fullscreen(view_id),
+            lambda: self.set_minimized(view_id, choice([True, False])),
+            lambda: self.set_sticky(view_id, choice([True, False])),
+            lambda: self.send_to_back(view_id, choice([True, False])),
+            lambda: self.set_view_alpha(view_id, random() * 1.0),
+        ]
+        choice(actions)()
 
     def test_move_cursor_and_click(self):
-        self.move_cursor(randint(100, 10000), randint(100, 10000))
-        self.click_button("BTN_LEFT", "press")
-        self.click_button("BTN_LEFT", "press")
+        sumgeo = self.sum_geometry_resolution()
+        self.move_cursor(randint(100, sumgeo[0]), randint(100, sumgeo[1]))
+        self.click_button("BTN_LEFT", "full")
+
+    def test_move_cursor_and_drag_drop(self):
+        sumgeo = self.sum_geometry_resolution()
+        random_iterations = randint(1, 8)
+
+        for _ in range(random_iterations):
+            self.click_and_drag(
+                "S-BTN_LEFT",
+                randint(1, sumgeo[0]),
+                randint(1, sumgeo[1]),
+                randint(1, sumgeo[0]),
+                randint(1, sumgeo[1]),
+                True,
+            )
 
     def test_list_info(self, view_id):
+        if view_id is None:
+            view_id = self.test_random_view_id()
         self.list_outputs()
         self.list_wsets()
-        self.wset_info(view_id)
+        # self.wset_info(view_id)
         self.get_view(view_id)
         self.get_view_info(view_id)
         self.get_view_alpha(view_id)
         self.list_input_devices()
         self.get_workspaces_with_views()
         self.get_workspaces_without_views()
         self.get_views_from_active_workspace()
@@ -1418,73 +2068,213 @@
 
     def test_cube_plugin(self):
         self.cube_activate()
         self.cube_rotate_left()
         self.cube_rotate_right()
         self.click_button("BTN_LEFT", "full")
 
-    def test_plugins(self):
-        functions = [
-            (self.scale_toggle, ()),
-            (self.toggle_expo, ()),
-            (self.toggle_showdesktop, ()),
-            (self.test_cube_plugin, ()),
-            # (self.reload_plugins, ()),
+    def test_toggle_switcher_view_plugin(self):
+        for _ in range(2):
+            self.press_key("A-KEY_TAB")
+
+    def test_toggle_tile_plugin(self):
+        self.press_key("W-KEY_T")
+
+    def test_auto_rotate_plugin(self):
+        keys_combinations = [
+            "C-W-KEY_UP",
+            "C-W-KEY_LEFT",
+            "C-W-KEY_RIGHT",
+            "C-W-KEY_DOWN",
         ]
-        random_function, args = choice(functions)
-        random_function(*args)
+
+        for _ in range(len(keys_combinations)):
+            key_combination = choice(keys_combinations)
+            self.press_key(key_combination)
+
+    def test_invert_plugin(self):
+        for _ in range(2):
+            self.press_key("A-KEY_I")
+
+    def test_magnifier_plugin(self):
+        for _ in range(2):
+            self.press_key("A-W-KEY_M")
+
+    def test_focus_change_plugin(self):
+        for _ in range(2):
+            self.press_key("S-W-KEY_UP")
+            self.press_key("S-W-KEY_DOWN")
+            self.press_key("S-W-KEY_LEFT")
+            self.press_key("S-W-KEY_RIGHT")
+
+    def test_output_switcher_plugin(self):
+        for _ in range(2):
+            self.press_key("A-KEY_O")
+            self.press_key("A-S-KEY_O")
+
+    def test_low_priority_plugins(self, plugin=None):
+        functions = {
+            "invert": (self.test_invert_plugin, ()),
+            "focus-change": (self.test_focus_change_plugin, ()),
+            "magnifier": (self.test_magnifier_plugin, ()),
+            "output-switcher": (self.test_output_switcher_plugin, ()),
+        }
+
+        if plugin is None:
+            random_function, args = choice(list(functions.values()))
+            random_function(*args)
+        elif plugin in functions:
+            random_function, args = functions[plugin]
+            random_function(*args)
+
+    def test_plugins(self, plugin=None):
+        functions = {
+            "expo": (self.toggle_expo, ()),
+            "scale": (self.scale_toggle, ()),
+            "showdesktop": (self.toggle_showdesktop, ()),
+            "cube": (self.test_cube_plugin, ()),
+            "switcherview": (self.test_toggle_switcher_view_plugin, ()),
+            "autorotate": (self.test_auto_rotate_plugin, ()),
+            "invert": (self.test_invert_plugin, ()),
+            "tile": (self.test_toggle_tile_plugin, ()),
+        }
+
+        if plugin is None:
+            random_function, args = choice(list(functions.values()))
+            random_function(*args)
+        elif plugin in functions:
+            random_function, args = functions[plugin]
+            random_function(*args)
+
+    def test_output(self):
+        current_outputs = self.list_outputs_ids()
+        if randint(1, 99) != 4:
+            return
+        self.create_wayland_output()
+        for output_id in self.list_outputs_ids():
+            if output_id in current_outputs:
+                continue
+            else:
+                name = self.query_output(output_id)["name"]
+                self.destroy_wayland_output(name)
 
     def test_turn_off_on_outputs(self):
         self.dpms("off")
         time.sleep(10)
         self.dpms("on")
 
-    def test_wayfire(self, number_of_views_to_open, max_tries=1, speed=0):
-        from wayfire.tests.gtk4_window import spam_new_views, open_new_view
+    def test_is_terminal_available(self, terminal):
+        try:
+            Popen(["which", terminal], stdout=PIPE, stderr=PIPE)
+            return True
+        except FileNotFoundError:
+            return False
 
-        list_views = self.list_views()
-        view_id = None
-        if list_views:
-            view_id = choice([i["id"] for i in list_views])
-        workspaces = self.total_workspaces()
+    def test_choose_terminal(self):
+        terminals = [
+            "xterm",
+            "alacritty",
+            "kitty",
+            "rxvt",
+            "rxvt-unicode",
+            "lxterminal",
+            "eterm",
+            "roxterm",
+            "mlterm",
+            "sakura",
+            "aterm",
+            "xfce4-terminal",
+            "mlterm",
+            "stterm",
+            "konsole",
+            "gnome-terminal",
+            "mate-terminal",
+            "terminology",
+            "terminator",
+            "tilda",
+            "tilix",
+            "alacritty",
+            "foot",
+            "cool-retro-term",
+            "deepin-terminal",
+            "rxvt-unicode-256color",
+            "pantheon-terminal",
+        ]
+        for terminal in terminals:
+            if self.test_is_terminal_available(terminal):
+                run(["killall", "-9", terminal])
+                return terminal
+        return None
+
+    def test_spam_terminals(self, number_of_views_to_open, wayland_display=None):
+        chosen_terminal = self.test_choose_terminal()
+        if chosen_terminal:
+            for _ in range(number_of_views_to_open):
+                if wayland_display is None:
+                    sock.run(chosen_terminal)
+                else:
+                    command = "export WAYLAND_DISPLAY={0} ; {1}".format(
+                        wayland_display, chosen_terminal
+                    )
+                    Popen(command, shell=True)
+
+    def test_spam_go_workspace_set_focus(self):
+        list_ids = self.list_ids()
+        num_items = randint(1, len(list_ids))
+        random_views = sample(list_ids, num_items)
+        for view_id in random_views:
+            self.go_workspace_set_focus(view_id)
+
+    def test_set_function_priority(self, functions):
+        priority = []
+        for _ in range(randint(1, 4)):
+            priority.append(choice(functions))
+        return priority
+
+    def random_delay_next_tx(self):
+        random_run = randint(1, 8)
+        if random_run > 4:
+            for _ in range(1, randint(2, 100)):
+                self.delay_next_tx()
+
+    def test_random_views(self, view_id):
+        functions = [
+            lambda: self.test_random_set_view_position(view_id),
+            lambda: self.test_random_change_view_state(view_id),
+            lambda: self.test_set_view_position(view_id),
+            lambda: self.test_change_view_state(view_id),
+        ]
+
+        choice(functions)()
+
+    def test_wayfire(
+        self, number_of_views_to_open, max_tries=1, speed=0, plugin=None, display=None
+    ):
+        from wayfire.tests.gtk3_window import spam_new_views
+        from wayfire.tests.gtk3_dialogs import spam_new_dialogs
+        from wayfire.tests.layershell import spam_new_layers
+
+        # Retrieve necessary data
+        view_id = self.test_random_view_id()
+        workspaces = (
+            [{"x": x, "y": y} for x, y in self.total_workspaces().values()]
+            if self.total_workspaces()
+            else []
+        )
         sumgeo = self.sum_geometry_resolution()
-        if workspaces:
-            workspaces = workspaces.values()
-            workspaces = [{"x": x, "y": y} for x, y in workspaces]
 
+        # Define functions to be executed
         functions = [
-            (self.go_next_workspace_with_views, ()),
-            (self.set_focused_view_to_workspace_without_views, ()),
-            # (self.test_move_cursor_and_click, ()),
-            (self.test_random_set_view_position, (view_id,)),
-            (self.test_random_change_view_state, (view_id,)),
-            (self.test_random_list_info, (view_id,)),
-            (self.test_set_view_position, (view_id)),
-            (self.test_list_info, (view_id)),
-            (self.test_change_view_state, (view_id)),
-            (self.test_plugins, ()),
-            (self.set_focus, (view_id,)),
-            (
-                self.click_and_drag,
-                (
-                    "S-BTN_LEFT",
-                    randint(1, sumgeo[0]),
-                    randint(1, sumgeo[1]),
-                    randint(1, sumgeo[0]),
-                    randint(1, sumgeo[1]),
-                    True,
-                ),
-            ),
-            (
-                # self.click_button,
-                # (
-                #    choice(["BTN_RIGHT", "BTN_LEFT"]),
-                #    "press",
-                # ),
-            ),
+            (self.go_workspace_set_focus, (view_id)),
+            (self.test_move_cursor_and_click, ()),
+            (self.test_plugins, (plugin,)),
+            (self.test_low_priority_plugins, (plugin,)),
+            (self.test_move_cursor_and_drag_drop, ()),
+            (self.test_output, ()),
+            (self.test_random_views, (view_id)),
             (
                 self.configure_view,
                 (
                     view_id,
                     randint(1, sumgeo[0]),
                     randint(0, sumgeo[1]),
                     randint(1, sumgeo[0]),
@@ -1494,67 +2284,73 @@
             (
                 self.set_workspace,
                 (choice(workspaces), view_id, choice(self.list_outputs_ids())),
             ),
         ]
 
         iterations = 0
-        dpms_allowed = 0
-        # lets keep those views open for some time
-        for i in range(number_of_views_to_open):
-            thread = threading.Thread(target=open_new_view, args=(1000000000))
-            thread.start()
 
-        # now spam views
+        self.test_spam_terminals(number_of_views_to_open, wayland_display=display)
+
+        # Start spamming views
         thread = threading.Thread(target=spam_new_views)
         thread.start()
 
-        results_file = "/tmp/test-wayfire.py"
-        if os.path.exists(results_file):
-            with open(results_file, "w"):
-                pass
-        # Write the necessary imports at the beginning of the file
-        with open(results_file, "a") as file:
-            file.write("import socket\n")
-            file.write("import json as js\n")
-            file.write("import os\n")
-            file.write("from subprocess import call\n")
-            file.write("from itertools import cycle\n")
-            file.write("from sys import argv\n")
-            file.write("import dbus\n")
-            file.write("import configparser\n")
-            file.write("from itertools import filterfalse\n")
-            file.write("import time\n")
-            file.write("from random import randint, choice, random\n")
-            file.write("import threading\n")
-            file.write("\n")
+        thread = threading.Thread(target=spam_new_dialogs)
+        thread.start()
+
+        # spam_new_layers_thread = threading.Thread(target=spam_new_layers)
+        # spam_new_layers_thread.start()
+
+        # FIXME: Implement this to not use keybinds in the terminal with script running
+        # first_view_focused = self.get_focused_view()
+
+        # Execute functions with specified priority
+        func_priority = self.test_set_function_priority(functions)
+        should_execute_function_priority = 0
+        should_change_function_priority = 0
 
         while iterations < max_tries:
             if speed != 0:
                 random_time = speed / randint(1, speed)
                 time.sleep(random_time / 1000)
+
             try:
-                # only run dpms two times
-                if dpms_allowed > max_tries / 2:
-                    thread_outputs = threading.Thread(
-                        target=self.test_turn_off_on_outputs
-                    )
-                    thread_outputs.start()
-                    dpms_allowed = 0
-                dpms_allowed += 1
-                random_function, args = choice(functions)
+                # Repeat certain functions every N iterations
+                if should_execute_function_priority > 20:
+                    for func, args in func_priority:
+                        for _ in range(4):
+                            result = func(*args)
+                            print(result)
+                    should_execute_function_priority = 0
+
+                should_execute_function_priority += 1
+
+                if should_change_function_priority > 40:
+                    func_priority = self.test_set_function_priority(functions)
+                    should_execute_function_priority = 0
 
-                # Write the function call with "sock." prefix to the file
-                with open(results_file, "a") as file:
-                    file.write(
-                        f"sock.{random_function.__name__}({', '.join(map(repr, args))})\n"
-                    )
+                should_change_function_priority += 1
+
+                random_function, args = choice(functions)
 
                 result = random_function(*args)
                 iterations += 1
                 print(result)
+                self.random_delay_next_tx()
+                if iterations + 1 == max_tries:
+                    # lets close the focused output in the last iteration
+                    # so it close while still there is actions going on
+                    try:
+                        output_id = self.get_focused_output_id()
+                        name = self.query_output(output_id)["name"]
+                        self.destroy_wayland_output(name)
+                    except Exception as e:
+                        print(e)
+
             except Exception as e:
+                func_priority = self.test_set_function_priority(functions)
                 print(e)
 
 
 addr = os.getenv("WAYFIRE_SOCKET")
 sock = WayfireSocket(addr)
```

### Comparing `wayfire-0.1.1/wayfire.egg-info/PKG-INFO` & `wayfire-1.0/wayfire.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wayfire
-Version: 0.1.1
+Version: 1.0
 Summary: wayfire compositor library
 Author-email: Thiago <systemofdown@gmail.com>
 Project-URL: Homepage, https://github.com/killown/waypy
 Project-URL: Issues, https://github.com/killown/waypy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
```

