# Comparing `tmp/tooldelta-0.5.8.tar.gz` & `tmp/tooldelta-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooldelta-0.5.8.tar", max compression
+gzip compressed data, was "tooldelta-0.5.9.tar", max compression
```

## Comparing `tooldelta-0.5.8.tar` & `tooldelta-0.5.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rwxr-xr-x   0        0        0     1497 2024-04-19 14:15:54.468505 tooldelta-0.5.8/LICENSE
--rwxr-xr-x   0        0        0     2504 2024-04-19 14:15:54.468505 tooldelta-0.5.8/README.md
--rwxr-xr-x   0        0        0      973 2024-04-19 14:16:02.764524 tooldelta-0.5.8/pyproject.toml
--rwxr-xr-x   0        0        0      360 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/__init__.py
--rw-r--r--   0        0        0     4979 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/auths.py
--rwxr-xr-x   0        0        0    19961 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/builtins.py
--rwxr-xr-x   0        0        0    12365 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/cfg.py
--rwxr-xr-x   0        0        0    10889 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/color_print.py
--rw-r--r--   0        0        0     1884 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/constants.py
--rw-r--r--   0        0        0     5870 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/fb_conn/fbconn.py
--rwxr-xr-x   0        0        0    30098 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/frame.py
--rwxr-xr-x   0        0        0     4644 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/game_texts.py
--rwxr-xr-x   0        0        0      476 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/get_tool_delta_version.py
--rwxr-xr-x   0        0        0    20525 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/launch_cli.py
--rwxr-xr-x   0        0        0     1276 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/launch_options.py
--rwxr-xr-x   0        0        0     2425 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/logger.py
--rw-r--r--   0        0        0    30151 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/neo_conn.py
--rwxr-xr-x   0        0        0     1292 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/packets.py
--rwxr-xr-x   0        0        0    15769 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/plugin_load/PluginGroup.py
--rwxr-xr-x   0        0        0     3118 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/plugin_load/__init__.py
--rwxr-xr-x   0        0        0     7341 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/plugin_load/classic_plugin/__init__.py
--rwxr-xr-x   0        0        0      450 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/plugin_load/funcs.py
--rwxr-xr-x   0        0        0     9975 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/plugin_load/injected_plugin/__init__.py
--rwxr-xr-x   0        0        0     9146 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/plugin_load/injected_plugin/movent.py
--rwxr-xr-x   0        0        0    16934 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/plugin_manager.py
--rwxr-xr-x   0        0        0    16769 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/plugin_market.py
--rw-r--r--   0        0        0     1774 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/starter.py
--rwxr-xr-x   0        0        0      808 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/sys_args.py
--rwxr-xr-x   0        0        0     9071 2024-04-19 14:15:54.472505 tooldelta-0.5.8/tooldelta/urlmethod.py
--rw-r--r--   0        0        0     3743 1970-01-01 00:00:00.000000 tooldelta-0.5.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1497 2024-04-20 14:07:12.823486 tooldelta-0.5.9/LICENSE
+-rwxr-xr-x   0        0        0     2504 2024-04-20 14:07:12.823486 tooldelta-0.5.9/README.md
+-rwxr-xr-x   0        0        0      973 2024-04-20 14:07:20.891478 tooldelta-0.5.9/pyproject.toml
+-rwxr-xr-x   0        0        0      360 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/__init__.py
+-rw-r--r--   0        0        0     4979 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/auths.py
+-rwxr-xr-x   0        0        0    19961 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/builtins.py
+-rwxr-xr-x   0        0        0    12372 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/cfg.py
+-rwxr-xr-x   0        0        0    10889 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/color_print.py
+-rw-r--r--   0        0        0     1884 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/constants.py
+-rw-r--r--   0        0        0     5870 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/fb_conn/fbconn.py
+-rwxr-xr-x   0        0        0    30106 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/frame.py
+-rwxr-xr-x   0        0        0     4644 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/game_texts.py
+-rwxr-xr-x   0        0        0      476 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/get_tool_delta_version.py
+-rwxr-xr-x   0        0        0    20525 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/launch_cli.py
+-rwxr-xr-x   0        0        0     1534 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/launch_options.py
+-rwxr-xr-x   0        0        0     2425 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/logger.py
+-rw-r--r--   0        0        0    30151 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/neo_conn.py
+-rwxr-xr-x   0        0        0     1292 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/packets.py
+-rwxr-xr-x   0        0        0    15769 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/plugin_load/PluginGroup.py
+-rwxr-xr-x   0        0        0     3118 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/plugin_load/__init__.py
+-rwxr-xr-x   0        0        0     7341 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/plugin_load/classic_plugin/__init__.py
+-rwxr-xr-x   0        0        0      450 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/plugin_load/funcs.py
+-rwxr-xr-x   0        0        0     9975 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/plugin_load/injected_plugin/__init__.py
+-rwxr-xr-x   0        0        0     9146 2024-04-20 14:07:12.827486 tooldelta-0.5.9/tooldelta/plugin_load/injected_plugin/movent.py
+-rwxr-xr-x   0        0        0    16934 2024-04-20 14:07:12.831486 tooldelta-0.5.9/tooldelta/plugin_manager.py
+-rwxr-xr-x   0        0        0    16769 2024-04-20 14:07:12.831486 tooldelta-0.5.9/tooldelta/plugin_market.py
+-rw-r--r--   0        0        0     1784 2024-04-20 14:07:12.831486 tooldelta-0.5.9/tooldelta/starter.py
+-rwxr-xr-x   0        0        0      808 2024-04-20 14:07:12.831486 tooldelta-0.5.9/tooldelta/sys_args.py
+-rwxr-xr-x   0        0        0     9071 2024-04-20 14:07:12.831486 tooldelta-0.5.9/tooldelta/urlmethod.py
+-rw-r--r--   0        0        0     3743 1970-01-01 00:00:00.000000 tooldelta-0.5.9/PKG-INFO
```

### Comparing `tooldelta-0.5.8/LICENSE` & `tooldelta-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.8/README.md` & `tooldelta-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.8/pyproject.toml` & `tooldelta-0.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Tooldelta"
-version = "0.5.8" # This field is automatically set to the value in the version file
+version = "0.5.9" # This field is automatically set to the value in the version file
 description = "Plugin Loader for NeteaseRentalServer on Panel"
 authors = ["SuperScript-PRC"]
 license = ""
 
 readme = "README.md"
 homepage = "https://github.com/SuperScript-PRC/ToolDelta"
 repository = "https://github.com/SuperScript-PRC/ToolDelta"
```

### Comparing `tooldelta-0.5.8/tooldelta/auths.py` & `tooldelta-0.5.9/tooldelta/auths.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.8/tooldelta/builtins.py` & `tooldelta-0.5.9/tooldelta/builtins.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.8/tooldelta/cfg.py` & `tooldelta-0.5.9/tooldelta/cfg.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
         return os.path.isfile(path if path.endswith(".json") else path + ".json")
 
     def getPluginConfigAndVersion(
         self,
         pluginName: str,
         standardType: dict,
         default: dict,
-        default_vers: tuple[int, int, int],
+        default_vers: tuple[int, int, int] | list,
     ) -> tuple[dict[str, Any], tuple[int, ...]]:
         """获取插件配置文件及版本
 
         Args:
             pluginName (str): 插件名
             standardType (dict): 标准类型
             default (dict): 默认配置
```

### Comparing `tooldelta-0.5.8/tooldelta/color_print.py` & `tooldelta-0.5.9/tooldelta/color_print.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.8/tooldelta/constants.py` & `tooldelta-0.5.9/tooldelta/constants.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.8/tooldelta/fb_conn/fbconn.py` & `tooldelta-0.5.9/tooldelta/fb_conn/fbconn.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.8/tooldelta/frame.py` & `tooldelta-0.5.9/tooldelta/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -550,19 +550,19 @@
         if is_skiped:
             return
         if pkt_type == PacketIDS.PlayerList:
             self.process_player_list(pkt, self.linked_frame.link_plugin_group)
         elif pkt_type == PacketIDS.Text:
             self.process_text_packet(pkt, self.linked_frame.link_plugin_group)
 
-    def process_player_list(self, pkt, plugin_group: "PluginGroup") -> None:
+    def process_player_list(self, pkt: dict, plugin_group: "PluginGroup") -> None:
         """处理玩家列表等数据包
 
         Args:
-            pkt (_type_): 数据包内容
+            pkt (dict): 数据包内容
             plugin_group (PluginGroup): 插件组对象
         """
         # 处理玩家进出事件
         res = self.launcher.get_players_and_uuids()
         if res:
             self.allplayers = list(res.keys())
             self.players_uuid.update(res)
@@ -573,15 +573,15 @@
                 Print.print_inf(f"§e{playername} 加入了游戏")
                 if playername not in self.allplayers and not res:
                     self.allplayers.append(playername)
                     return
                 plugin_group.execute_player_join(
                     playername, self.linked_frame.on_plugin_err
                 )
-                asyncio.run(execute_player_join(player))
+                asyncio.run(execute_player_join(playername))
             else:
                 playername = next(
                     (k for k, v in self.players_uuid.items()
                      if v == player["UUID"]),
                     None,
                 )
                 if playername is None:
```

### Comparing `tooldelta-0.5.8/tooldelta/game_texts.py` & `tooldelta-0.5.9/tooldelta/game_texts.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.8/tooldelta/launch_cli.py` & `tooldelta-0.5.9/tooldelta/launch_cli.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.8/tooldelta/launch_options.py` & `tooldelta-0.5.9/tooldelta/launch_options.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 "启动选项"
 import os
 import signal
+import traceback
 from .color_print import Print
 from .starter import start_tool_delta
 from .plugin_manager import plugin_manager
 from .plugin_market import market
 from .sys_args import sys_args_to_dict
 
 
@@ -14,28 +15,33 @@
 
 
 signal.signal(signal.SIGINT, signal_handler)
 
 
 def client_title() -> None:
     "选择启动模式"
-    launch_mode = sys_args_to_dict()
-    if launch_mode.get("l"):
-        if not isinstance(launch_mode["l"], str):
-            raise ValueError("启动模式参数不合法")
-        r = launch_mode["l"]
-    else:
-        Print.clean_print("§b请选择启动模式(使用启动参数 -l <启动模式> 可以跳过该页面):")
-        Print.clean_print("1 - 启动 ToolDelta")
-        Print.clean_print("2 - 打开 ToolDelta 插件管理器")
-        Print.clean_print("3 - 打开 ToolDelta 插件市场")
-        r = input("请选择:").strip()
-    match r:
-        case "1":
-            start_tool_delta()
-        case "2":
-            plugin_manager.manage_plugins()
-        case "3":
-            market.enter_plugin_market()
-        case _:
-            Print.clean_print("§c不合法的模式: " + r)
-    os._exit(0)
+    try:
+        launch_mode = sys_args_to_dict()
+        if launch_mode.get("l"):
+            if not isinstance(launch_mode["l"], str):
+                raise ValueError("启动模式参数不合法")
+            r = launch_mode["l"]
+        else:
+            Print.clean_print("§b请选择启动模式(使用启动参数 -l <启动模式> 可以跳过该页面):")
+            Print.clean_print("1 - 启动 ToolDelta")
+            Print.clean_print("2 - 打开 ToolDelta 插件管理器")
+            Print.clean_print("3 - 打开 ToolDelta 插件市场")
+            r = input("请选择:").strip()
+        match r:
+            case "1":
+                start_tool_delta()
+            case "2":
+                plugin_manager.manage_plugins()
+            case "3":
+                market.enter_plugin_market()
+            case _:
+                Print.clean_print("§c不合法的模式: " + r)
+        os._exit(0)
+    except EOFError:
+        pass
+    except Exception:
+        Print.print_err("ToolDelta 运行过程中出现问题: " + traceback.format_exc())
```

### Comparing `tooldelta-0.5.8/tooldelta/logger.py` & `tooldelta-0.5.9/tooldelta/logger.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.8/tooldelta/neo_conn.py` & `tooldelta-0.5.9/tooldelta/neo_conn.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.8/tooldelta/packets.py` & `tooldelta-0.5.9/tooldelta/packets.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.8/tooldelta/plugin_load/PluginGroup.py` & `tooldelta-0.5.9/tooldelta/plugin_load/PluginGroup.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.8/tooldelta/plugin_load/__init__.py` & `tooldelta-0.5.9/tooldelta/plugin_load/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.8/tooldelta/plugin_load/classic_plugin/__init__.py` & `tooldelta-0.5.9/tooldelta/plugin_load/classic_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.8/tooldelta/plugin_load/injected_plugin/__init__.py` & `tooldelta-0.5.9/tooldelta/plugin_load/injected_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.8/tooldelta/plugin_load/injected_plugin/movent.py` & `tooldelta-0.5.9/tooldelta/plugin_load/injected_plugin/movent.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.8/tooldelta/plugin_manager.py` & `tooldelta-0.5.9/tooldelta/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.8/tooldelta/plugin_market.py` & `tooldelta-0.5.9/tooldelta/plugin_market.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.8/tooldelta/starter.py` & `tooldelta-0.5.9/tooldelta/starter.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         movent.set_frame(frame)
         plugin_group.read_all_plugins()
         frame.plugin_load_finished(plugin_group)
         tmpjson_save_thread()
         frame.launcher.listen_launched(game_control.Inject)
         game_control.set_listen_packets()
         raise frame.launcher.launch()
-    except (KeyboardInterrupt, SystemExit):
+    except (KeyboardInterrupt, SystemExit, EOFError):
         pass
     except Exception:
         Print.print_err("ToolDelta 运行过程中出现问题: " + traceback.format_exc())
 
 
 def safe_jump(*, out_task: bool = True, exit_directly: bool = True) -> None:
     """安全退出
```

### Comparing `tooldelta-0.5.8/tooldelta/sys_args.py` & `tooldelta-0.5.9/tooldelta/sys_args.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.8/tooldelta/urlmethod.py` & `tooldelta-0.5.9/tooldelta/urlmethod.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.8/PKG-INFO` & `tooldelta-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Tooldelta
-Version: 0.5.8
+Version: 0.5.9
 Summary: Plugin Loader for NeteaseRentalServer on Panel
 Home-page: https://github.com/SuperScript-PRC/ToolDelta
 Author: SuperScript-PRC
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Tooldelta Version: 0.5.8 Summary: Plugin Loader for
+Metadata-Version: 2.1 Name: Tooldelta Version: 0.5.9 Summary: Plugin Loader for
 NeteaseRentalServer on Panel Home-page: https://github.com/SuperScript-PRC/
 ToolDelta Author: SuperScript-PRC Requires-Python: >=3.9,<3.13 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: aiohttp (>=3.9.3,<4.0.0) Requires-Dist: colorama
 (>=0.4.6,<0.5.0) Requires-Dist: flask (>=3.0.2,<4.0.0) Requires-Dist: mido
```

