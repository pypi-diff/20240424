# Comparing `tmp/axem_dem-0.4.0.tar.gz` & `tmp/axem_dem-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axem_dem-0.4.0.tar", max compression
+gzip compressed data, was "axem_dem-0.5.0.tar", max compression
```

## Comparing `axem_dem-0.4.0.tar` & `axem_dem-0.5.0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
--rw-r--r--   0        0        0    13291 2024-02-23 13:48:13.916078 axem_dem-0.4.0/LICENSE
--rw-r--r--   0        0        0     6008 2024-03-12 14:32:11.417948 axem_dem-0.4.0/README.md
--rw-r--r--   0        0        0       97 2024-02-23 13:48:13.916078 axem_dem-0.4.0/dem/__init__.py
--rw-r--r--   0        0        0     2330 2024-03-28 14:04:41.572070 axem_dem-0.4.0/dem/__main__.py
--rw-r--r--   0        0        0      745 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/cli/command/add_cat_cmd.py
--rw-r--r--   0        0        0      826 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/cli/command/add_host_cmd.py
--rw-r--r--   0        0        0      649 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/cli/command/add_reg_cmd.py
--rw-r--r--   0        0        0     1134 2024-03-28 14:04:41.572070 axem_dem-0.4.0/dem/cli/command/assign_cmd.py
--rw-r--r--   0        0        0     2219 2024-03-28 14:04:41.572070 axem_dem-0.4.0/dem/cli/command/clone_cmd.py
--rw-r--r--   0        0        0     1508 2024-03-28 14:04:41.572070 axem_dem-0.4.0/dem/cli/command/cp_cmd.py
--rw-r--r--   0        0        0     4709 2024-04-03 10:43:00.178425 axem_dem-0.4.0/dem/cli/command/create_cmd.py
--rw-r--r--   0        0        0      755 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/cli/command/del_cat_cmd.py
--rw-r--r--   0        0        0      647 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/cli/command/del_host_cmd.py
--rw-r--r--   0        0        0      706 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/cli/command/del_reg_cmd.py
--rw-r--r--   0        0        0     1158 2024-03-28 14:04:41.572070 axem_dem-0.4.0/dem/cli/command/delete_cmd.py
--rw-r--r--   0        0        0      909 2024-03-28 14:04:41.572070 axem_dem-0.4.0/dem/cli/command/export_cmd.py
--rw-r--r--   0        0        0     2002 2024-04-03 10:43:00.178425 axem_dem-0.4.0/dem/cli/command/info_cmd.py
--rw-r--r--   0        0        0     2048 2024-03-28 14:04:41.572070 axem_dem-0.4.0/dem/cli/command/init_cmd.py
--rw-r--r--   0        0        0     1173 2024-03-28 14:04:41.572070 axem_dem-0.4.0/dem/cli/command/install_cmd.py
--rw-r--r--   0        0        0      935 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/cli/command/list_cat_cmd.py
--rw-r--r--   0        0        0     5427 2024-03-28 14:04:41.572070 axem_dem-0.4.0/dem/cli/command/list_cmd.py
--rw-r--r--   0        0        0      972 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/cli/command/list_host_cmd.py
--rw-r--r--   0        0        0      636 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/cli/command/list_reg_cmd.py
--rw-r--r--   0        0        0     1431 2024-03-28 14:04:41.572070 axem_dem-0.4.0/dem/cli/command/load_cmd.py
--rw-r--r--   0        0        0     7181 2024-04-03 10:43:00.178425 axem_dem-0.4.0/dem/cli/command/modify_cmd.py
--rw-r--r--   0        0        0      545 2024-03-28 14:04:41.572070 axem_dem-0.4.0/dem/cli/command/rename_cmd.py
--rw-r--r--   0        0        0     2372 2024-03-28 14:04:41.572070 axem_dem-0.4.0/dem/cli/command/run_cmd.py
--rw-r--r--   0        0        0     1119 2024-03-28 14:04:41.572070 axem_dem-0.4.0/dem/cli/command/uninstall_cmd.py
--rw-r--r--   0        0        0      167 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/cli/console.py
--rw-r--r--   0        0        0    16397 2024-03-28 11:53:58.448947 axem_dem-0.4.0/dem/cli/main.py
--rw-r--r--   0        0        0      790 2024-04-03 10:43:00.178425 axem_dem-0.4.0/dem/cli/tui/printable_tool_image.py
--rw-r--r--   0        0        0    10200 2024-04-03 10:43:00.178425 axem_dem-0.4.0/dem/cli/tui/renderable/menu.py
--rw-r--r--   0        0        0     4411 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/cli/tui/tui_user_output.py
--rw-r--r--   0        0        0     5453 2024-04-03 17:47:34.676890 axem_dem-0.4.0/dem/cli/tui/window/dev_env_settings_window.py
--rw-r--r--   0        0        0     5263 2024-03-28 14:49:12.318896 axem_dem-0.4.0/dem/core/container_engine.py
--rw-r--r--   0        0        0      770 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/core/core.py
--rw-r--r--   0        0        0     4232 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/core/data_management.py
--rwxr-xr-x   0        0        0     3020 2024-03-28 11:53:58.448947 axem_dem-0.4.0/dem/core/dev_env.py
--rw-r--r--   0        0        0     4443 2024-03-25 12:12:59.178746 axem_dem-0.4.0/dem/core/dev_env_catalog.py
--rw-r--r--   0        0        0     1330 2024-03-28 11:53:58.448947 axem_dem-0.4.0/dem/core/exceptions.py
--rw-r--r--   0        0        0     2122 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/core/hosts.py
--rw-r--r--   0        0        0     9982 2024-03-28 11:53:58.452947 axem_dem-0.4.0/dem/core/platform.py
--rw-r--r--   0        0        0      129 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/core/properties.py
--rw-r--r--   0        0        0     9292 2024-03-29 10:43:36.316870 axem_dem-0.4.0/dem/core/registry.py
--rw-r--r--   0        0        0     3507 2024-03-28 11:53:58.452947 axem_dem-0.4.0/dem/core/tool_images.py
--rw-r--r--   0        0        0     2235 2024-02-23 13:48:13.920078 axem_dem-0.4.0/dem/core/user_output.py
--rw-r--r--   0        0        0     1812 2024-04-03 17:54:18.051991 axem_dem-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     7373 1970-01-01 00:00:00.000000 axem_dem-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    13291 2024-04-04 10:00:14.896884 axem_dem-0.5.0/LICENSE
+-rw-r--r--   0        0        0     6008 2024-04-04 10:00:14.900884 axem_dem-0.5.0/README.md
+-rw-r--r--   0        0        0       97 2024-04-04 10:00:14.900884 axem_dem-0.5.0/dem/__init__.py
+-rw-r--r--   0        0        0     2330 2024-04-04 10:00:14.900884 axem_dem-0.5.0/dem/__main__.py
+-rw-r--r--   0        0        0      745 2024-04-04 10:00:14.900884 axem_dem-0.5.0/dem/cli/command/add_cat_cmd.py
+-rw-r--r--   0        0        0      826 2024-04-04 10:00:14.900884 axem_dem-0.5.0/dem/cli/command/add_host_cmd.py
+-rw-r--r--   0        0        0      649 2024-04-04 10:00:14.900884 axem_dem-0.5.0/dem/cli/command/add_reg_cmd.py
+-rw-r--r--   0        0        0     1134 2024-04-23 08:46:41.499604 axem_dem-0.5.0/dem/cli/command/assign_cmd.py
+-rw-r--r--   0        0        0     2219 2024-04-23 08:46:41.499604 axem_dem-0.5.0/dem/cli/command/clone_cmd.py
+-rw-r--r--   0        0        0     1508 2024-04-23 08:46:41.499604 axem_dem-0.5.0/dem/cli/command/cp_cmd.py
+-rw-r--r--   0        0        0     4709 2024-04-23 08:46:41.503604 axem_dem-0.5.0/dem/cli/command/create_cmd.py
+-rw-r--r--   0        0        0      755 2024-04-04 10:00:14.900884 axem_dem-0.5.0/dem/cli/command/del_cat_cmd.py
+-rw-r--r--   0        0        0      647 2024-04-04 10:00:14.900884 axem_dem-0.5.0/dem/cli/command/del_host_cmd.py
+-rw-r--r--   0        0        0      706 2024-04-04 10:00:14.900884 axem_dem-0.5.0/dem/cli/command/del_reg_cmd.py
+-rw-r--r--   0        0        0     1158 2024-04-23 08:46:41.503604 axem_dem-0.5.0/dem/cli/command/delete_cmd.py
+-rw-r--r--   0        0        0      909 2024-04-04 10:00:14.900884 axem_dem-0.5.0/dem/cli/command/export_cmd.py
+-rw-r--r--   0        0        0     1911 2024-04-23 08:46:41.503604 axem_dem-0.5.0/dem/cli/command/import_cmd.py
+-rw-r--r--   0        0        0     6440 2024-04-23 08:46:41.503604 axem_dem-0.5.0/dem/cli/command/info_cmd.py
+-rw-r--r--   0        0        0     2048 2024-04-23 08:46:41.503604 axem_dem-0.5.0/dem/cli/command/init_cmd.py
+-rw-r--r--   0        0        0     1173 2024-04-04 10:00:14.900884 axem_dem-0.5.0/dem/cli/command/install_cmd.py
+-rw-r--r--   0        0        0      935 2024-04-04 10:00:14.900884 axem_dem-0.5.0/dem/cli/command/list_cat_cmd.py
+-rw-r--r--   0        0        0     4110 2024-04-23 08:46:41.503604 axem_dem-0.5.0/dem/cli/command/list_cmd.py
+-rw-r--r--   0        0        0      972 2024-04-04 10:00:14.900884 axem_dem-0.5.0/dem/cli/command/list_host_cmd.py
+-rw-r--r--   0        0        0      636 2024-04-04 10:00:14.904884 axem_dem-0.5.0/dem/cli/command/list_reg_cmd.py
+-rw-r--r--   0        0        0     5040 2024-04-16 08:55:39.456506 axem_dem-0.5.0/dem/cli/command/list_tools_cmd.py
+-rw-r--r--   0        0        0     7181 2024-04-23 08:46:41.503604 axem_dem-0.5.0/dem/cli/command/modify_cmd.py
+-rw-r--r--   0        0        0      545 2024-04-23 08:46:41.507604 axem_dem-0.5.0/dem/cli/command/rename_cmd.py
+-rw-r--r--   0        0        0     2372 2024-04-04 10:00:14.904884 axem_dem-0.5.0/dem/cli/command/run_cmd.py
+-rw-r--r--   0        0        0     1119 2024-04-04 10:00:14.904884 axem_dem-0.5.0/dem/cli/command/uninstall_cmd.py
+-rw-r--r--   0        0        0      167 2024-04-04 10:00:14.904884 axem_dem-0.5.0/dem/cli/console.py
+-rw-r--r--   0        0        0    17635 2024-04-23 08:46:41.507604 axem_dem-0.5.0/dem/cli/main.py
+-rw-r--r--   0        0        0      964 2024-04-12 07:23:41.038261 axem_dem-0.5.0/dem/cli/tui/printable_tool_image.py
+-rw-r--r--   0        0        0    10200 2024-04-04 10:00:14.904884 axem_dem-0.5.0/dem/cli/tui/renderable/menu.py
+-rw-r--r--   0        0        0     4411 2024-04-04 10:00:14.904884 axem_dem-0.5.0/dem/cli/tui/tui_user_output.py
+-rw-r--r--   0        0        0     5453 2024-04-04 10:00:14.904884 axem_dem-0.5.0/dem/cli/tui/window/dev_env_settings_window.py
+-rw-r--r--   0        0        0     5263 2024-04-04 10:00:14.904884 axem_dem-0.5.0/dem/core/container_engine.py
+-rw-r--r--   0        0        0      770 2024-04-04 10:00:14.904884 axem_dem-0.5.0/dem/core/core.py
+-rw-r--r--   0        0        0     4232 2024-04-04 10:00:14.904884 axem_dem-0.5.0/dem/core/data_management.py
+-rwxr-xr-x   0        0        0     4468 2024-04-16 08:55:39.456506 axem_dem-0.5.0/dem/core/dev_env.py
+-rw-r--r--   0        0        0     4443 2024-04-04 10:00:14.908884 axem_dem-0.5.0/dem/core/dev_env_catalog.py
+-rw-r--r--   0        0        0     1461 2024-04-12 07:23:41.038261 axem_dem-0.5.0/dem/core/exceptions.py
+-rw-r--r--   0        0        0     2122 2024-04-04 10:00:14.908884 axem_dem-0.5.0/dem/core/hosts.py
+-rw-r--r--   0        0        0    10273 2024-04-23 08:46:41.507604 axem_dem-0.5.0/dem/core/platform.py
+-rw-r--r--   0        0        0      129 2024-04-04 10:00:14.908884 axem_dem-0.5.0/dem/core/properties.py
+-rw-r--r--   0        0        0     9626 2024-04-12 07:23:41.042261 axem_dem-0.5.0/dem/core/registry.py
+-rw-r--r--   0        0        0     3795 2024-04-12 07:23:41.042261 axem_dem-0.5.0/dem/core/tool_images.py
+-rw-r--r--   0        0        0     2235 2024-04-04 10:00:14.908884 axem_dem-0.5.0/dem/core/user_output.py
+-rw-r--r--   0        0        0     1819 2024-04-24 10:29:35.511775 axem_dem-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7411 1970-01-01 00:00:00.000000 axem_dem-0.5.0/PKG-INFO
```

### Comparing `axem_dem-0.4.0/LICENSE` & `axem_dem-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/README.md` & `axem_dem-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/__main__.py` & `axem_dem-0.5.0/dem/__main__.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/cli/command/add_cat_cmd.py` & `axem_dem-0.5.0/dem/cli/command/add_cat_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/cli/command/add_host_cmd.py` & `axem_dem-0.5.0/dem/cli/command/add_host_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/cli/command/add_reg_cmd.py` & `axem_dem-0.5.0/dem/cli/command/add_reg_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/cli/command/assign_cmd.py` & `axem_dem-0.5.0/dem/cli/command/assign_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/cli/command/clone_cmd.py` & `axem_dem-0.5.0/dem/cli/command/clone_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/cli/command/cp_cmd.py` & `axem_dem-0.5.0/dem/cli/command/cp_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/cli/command/create_cmd.py` & `axem_dem-0.5.0/dem/cli/command/create_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/cli/command/del_cat_cmd.py` & `axem_dem-0.5.0/dem/cli/command/del_cat_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/cli/command/del_host_cmd.py` & `axem_dem-0.5.0/dem/cli/command/del_host_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/cli/command/del_reg_cmd.py` & `axem_dem-0.5.0/dem/cli/command/del_reg_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/cli/command/delete_cmd.py` & `axem_dem-0.5.0/dem/cli/command/delete_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/cli/command/export_cmd.py` & `axem_dem-0.5.0/dem/cli/command/export_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/cli/command/init_cmd.py` & `axem_dem-0.5.0/dem/cli/command/init_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/cli/command/install_cmd.py` & `axem_dem-0.5.0/dem/cli/command/install_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/cli/command/list_cat_cmd.py` & `axem_dem-0.5.0/dem/cli/command/list_cat_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/cli/command/list_host_cmd.py` & `axem_dem-0.5.0/dem/cli/command/list_host_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/cli/command/list_reg_cmd.py` & `axem_dem-0.5.0/dem/cli/command/list_reg_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/cli/command/modify_cmd.py` & `axem_dem-0.5.0/dem/cli/command/modify_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/cli/command/rename_cmd.py` & `axem_dem-0.5.0/dem/cli/command/rename_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/cli/command/run_cmd.py` & `axem_dem-0.5.0/dem/cli/command/run_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/cli/command/uninstall_cmd.py` & `axem_dem-0.5.0/dem/cli/command/uninstall_cmd.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/cli/main.py` & `axem_dem-0.5.0/dem/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 # dem/cli/main.py
 
 import typer, importlib.metadata
 from typing import Generator
 from typing_extensions import Annotated
 import os
 from dem import __command__, __app_name__
-from dem.cli.command import cp_cmd, info_cmd, list_cmd, create_cmd, modify_cmd, delete_cmd, \
-                            rename_cmd, run_cmd, export_cmd, load_cmd, clone_cmd, add_reg_cmd, \
+from dem.cli.command import cp_cmd, import_cmd, info_cmd, list_cmd, create_cmd, modify_cmd, delete_cmd, \
+                            rename_cmd, run_cmd, export_cmd, clone_cmd, add_reg_cmd, \
                             list_reg_cmd, del_reg_cmd, add_cat_cmd, list_cat_cmd, del_cat_cmd, \
                             add_host_cmd, uninstall_cmd, install_cmd, assign_cmd, init_cmd, \
-                            list_host_cmd, del_host_cmd
+                            list_host_cmd, del_host_cmd, list_tools_cmd
 from dem.cli.console import stdout
 from dem.core.platform import Platform
 from dem.core.exceptions import InternalError
 
 typer_cli: typer.Typer = typer.Typer(rich_markup_mode="rich")
 platform: Platform | None = None
 
@@ -72,47 +72,67 @@
     """
     if platform is not None:
         for host_config in platform.hosts.list_host_configs():
             if host_config["name"].startswith(incomplete) or (incomplete == ""):
                 yield host_config["name"]
 
 # DEM commands
-@typer_cli.command("list") # "list" is a Python keyword
-def list_(local: Annotated[bool, typer.Option(help="Scope is the local host.")] = False,
-          all: Annotated[bool, typer.Option(help="Scope is the catalogs.")] = False,
-          env: Annotated[bool, typer.Option(help="List the environments.")] = False,
-          tool: Annotated[bool, typer.Option(help="List the tool images.")] = False) -> None:
+@typer_cli.command("list", context_settings={"allow_extra_args": True}) # "list" is a Python keyword
+def list_(cat: Annotated[bool, typer.Option(help="List the Dev Envs available from the catalogs.",
+                                            show_default=False)] = False,
+          ctx: Annotated[typer.Context, typer.Option()] = None) -> None:
     """
-    List the Development Environments available locally or from the catalogs.
-    
-    The following option combinations are suppported:
+    List the Dev Envs.
 
-        --local --env -> List the local Development Environments.
+    By default the local Dev Envs will be listed.
+    
+    --cat: List the available Dev Envs from the catalogs. Specify the catalogs' name to list the Dev 
+    Envs from. More then one catalog can be specified. If no catalog is specified, all the available
+    catalogs will be used.
+    """
+    if platform and ctx:
+        list_cmd.execute(platform, cat, ctx.args)
+    else:
+        raise InternalError("Error: The platform hasn't been initialized properly!")
 
-        --all --env -> List the Development Environments available from the catalogs.
+@typer_cli.command(context_settings={"allow_extra_args": True})
+def list_tools(reg: Annotated[bool, typer.Option(help="List the available tools in the registries.",
+                                                  show_default=False)] = False,
+               ctx: Annotated[typer.Context, typer.Option()] = None) -> None:
+    """
+    List the available tools.
 
-        --local --tool -> List the local tool images.
+    By default the local tools will be listed.
 
-        --all --tool -> List the tool images available from the registries.
+    --reg: List the available tools in the registries. Specify the registry's name to list the tools
+    from. More then one registry can be specified. If no registry is specified, all the available
+    registries will be used.
     """
-    if platform:
-        list_cmd.execute(platform, local, all, env, tool)
+    if platform and ctx:
+        list_tools_cmd.execute(platform, reg, ctx.args)
     else:
         raise InternalError("Error: The platform hasn't been initialized properly!")
 
-@typer_cli.command()
+@typer_cli.command(context_settings={"allow_extra_args": True})
 def info(dev_env_name: Annotated[str, typer.Argument(help="Name of the Development Environment to get info about.",
-                                                     autocompletion=autocomplete_dev_env_name)]) -> None:
+                                                     autocompletion=autocomplete_dev_env_name)],
+         cat: Annotated[bool, typer.Option(help="Get the Dev Env from the catalogs")] = False,
+         ctx: Annotated[typer.Context, typer.Option()] = None) -> None:
     """
     Get information about the specified Development Environment available locally or in the catalogs.
 
+    --cat: DEM will search for the Dev Env in the catalogs and will print the details of the first
+    match. You can specifiy the catalogs' name to search in after this option. If no catalog is 
+    specified, all the available catalogs will be used. If the Dev Env is not found in the catalogs,
+    an error message will be printed.
+
     Note: Autocomplete only works with the locally avialable Dev Envs.
     """
-    if platform:
-        info_cmd.execute(platform, dev_env_name)
+    if platform and ctx:
+        info_cmd.execute(platform, dev_env_name, cat, ctx.args)
     else:
         raise InternalError("Error: The platform hasn't been initialized properly!")
 
 @typer_cli.command()
 def cp(dev_env_name: Annotated[str, typer.Argument(help="Name of the Development Environment to cp.",
                                                    autocompletion=autocomplete_dev_env_name)],
        new_dev_env_name: Annotated[str, typer.Argument(help="Name of the New Development Environment.")]) -> None:
@@ -142,21 +162,21 @@
     Export the Development Environment.
     """
     if platform:
         export_cmd.execute(platform, dev_env_name,path_to_export)
     else:
         raise InternalError("Error: The platform hasn't been initialized properly!")
 
-@typer_cli.command()
-def load(path_to_dev_env: Annotated[str, typer.Argument(help="Path to the Dev Env to import.")]) -> None:
+@typer_cli.command("import")
+def import_(path_to_dev_env: Annotated[str, typer.Argument(help="Path to the Dev Env to import.")]) -> None:
     """
     Import the Development Environment.
     """
     if platform:
-        load_cmd.execute(platform, path_to_dev_env)
+        import_cmd.execute(platform, path_to_dev_env)
     else:
         raise InternalError("Error: The platform hasn't been initialized properly!")
 
 @typer_cli.command()
 def clone(dev_env_name: Annotated[str, typer.Argument(help="Name of the Dev Env descriptor to clone.")]) -> None:
     """
     Copy the Dev Env's descriptor from the catalog to the local descriptor storage.
```

### Comparing `axem_dem-0.4.0/dem/cli/tui/renderable/menu.py` & `axem_dem-0.5.0/dem/cli/tui/renderable/menu.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/cli/tui/tui_user_output.py` & `axem_dem-0.5.0/dem/cli/tui/tui_user_output.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/cli/tui/window/dev_env_settings_window.py` & `axem_dem-0.5.0/dem/cli/tui/window/dev_env_settings_window.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/core/container_engine.py` & `axem_dem-0.5.0/dem/core/container_engine.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/core/core.py` & `axem_dem-0.5.0/dem/core/core.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/core/data_management.py` & `axem_dem-0.5.0/dem/core/data_management.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/core/dev_env_catalog.py` & `axem_dem-0.5.0/dem/core/dev_env_catalog.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/core/exceptions.py` & `axem_dem-0.5.0/dem/core/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,19 @@
     base_message = "Invalid file: "
 
     def __init__(self, message: str = "") -> None:
         super().__init__(self.base_message + message)
 
 class RegistryError(Exception):
     """Raised when the communication with registry fails."""
-    pass
+
+    base_message = "Registry error: "
+
+    def __init__(self, message: str) -> None:
+        super().__init__(self.base_message + message)
 
 class ToolImageError(Exception):
     """Raised when there is a problem with the tool image."""
     pass
 
 class ContainerEngineError(Exception):
     """Raised when there is a problem with the container engine."""
```

### Comparing `axem_dem-0.4.0/dem/core/hosts.py` & `axem_dem-0.5.0/dem/core/hosts.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/dem/core/platform.py` & `axem_dem-0.5.0/dem/core/platform.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,15 @@
 from dem.core.hosts import Hosts
 
 class Platform(Core):
     """ Representation of the Development Platform:
         - The available tool images.
         - The available Development Environments.
         - External resources.
-
-        Class variables:
-            local_only -- work with the local tool images only
     """
-    local_only = False
 
     def _dev_env_json_version_check(self, dev_env_json_major_version: int) -> None:
         """ Check that the json file is supported.
 
             The version is stored as a string in the X.Y format.
             Raises an DataStorageError exception, if the version is not supported.
         """
@@ -39,14 +35,20 @@
         """ Init the class."""
         self._dev_env_catalogs: DevEnvCatalogs | None = None
         self._tool_images = None
         self._container_engine = None
         self._registries = None
         self._hosts = None
 
+        # Set this to true in the platform instance to work with the local tool images only
+        self.local_only = False
+        # Set this to true in the platform instance so when first accessing the `tool_images` 
+        # instance variable, do not automatically update the tool images from the registries
+        self.disable_tool_update = False
+
     def load_dev_envs(self) -> None:
         """ Load the Development Environments from the dev_env.json file.
         
             The Dev Envs will only contain the descriptors and not the ToolImage instances.
         """
         self.dev_env_json = LocalDevEnvJSON()
         self.dev_env_json.update()
@@ -65,15 +67,16 @@
     def tool_images(self) -> ToolImages:
         """ The tool images.
 
             The ToolImages() gets instantiated only at the first access.
         """
         if self._tool_images is None:
             self._tool_images = ToolImages(self.container_engine, self.registries)
-            self._tool_images.update(local_only=self.local_only)
+            if not self.disable_tool_update:
+                self._tool_images.update(local_only=self.local_only)
         return self._tool_images
     
     @property
     def container_engine(self) -> ContainerEngine:
         """ The container engine.
 
             The ContainerEngine() gets instantiated only at the first access.
```

### Comparing `axem_dem-0.4.0/dem/core/registry.py` & `axem_dem-0.5.0/dem/core/registry.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Direct access to the registry over HTTP. or using the container engine."""
 # dem/core/registry.py
 
 from dem.core.core import Core
 from dem.core.container_engine import ContainerEngine
+from dem.core.exceptions import RegistryError
 import requests
 from typing import Generator
 from abc import ABC, abstractmethod
 
 class Registry(Core, ABC):
     """ Abstract base class for a registry."""
     def __init__(self, container_engine: ContainerEngine, registry_config: dict) -> None:
@@ -181,27 +182,32 @@
                 registry_config -- registry config
             """
         if DockerHub._docker_hub_domain in registry_config["url"]:
             self.registries.append(DockerHub(self._container_engine, registry_config))
         else:
             self.registries.append(DockerRegistry(self._container_engine, registry_config))
 
-    def list_repos(self) -> list[str]:
+    def list_repos(self, reg_selection: list[str]) -> list[str]:
         """ List the available repositories.
+
+            Args:
+                reg_selection -- the selected registries, empty list means all registries
         
             Return with the list of repositories.
         """
         repo_list: list[str] = []
 
         for registry in self.registries:
-            try:
-                repo_list.extend(registry.repos)
-            except Exception as e:
-                self.user_output.error(str(e))
-                self.user_output.error("[red]Error: The " + registry._registry_config["name"] + " registry is not available.[/]")
+            if not reg_selection or registry._registry_config["name"] in reg_selection:
+                try:
+                    repo_list.extend(registry.repos)
+                except Exception as e:
+                    self.user_output.error(str(e))
+                    self.user_output.error("[red]Error: The " + registry._registry_config["name"] + \
+                                           " registry is not available.[/]")
 
         return repo_list
 
     def add_registry(self, registry_config: dict) -> None:
         """ Add a new registry.
         
             Args:
```

### Comparing `axem_dem-0.4.0/dem/core/tool_images.py` & `axem_dem-0.5.0/dem/core/tool_images.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,14 +10,22 @@
         LOCAL_ONLY,
         REGISTRY_ONLY,
         LOCAL_AND_REGISTRY,
         NOT_AVAILABLE,
     ) = range(4)
 
     def __init__(self, name: str) -> None:
+        """ Init the class.
+        
+            Args:
+                name -- the name of the tool image
+                
+            Exceptions:
+                ToolImageError -- if the name is invalid
+        """
         self.name = name
         try:
             self.repository = self.name.split(":")[0]
             self.tag = self.name.split(":")[1]
         except IndexError:
             raise ToolImageError(f"Invalid tool image name: {name}")
         self.availability = self.NOT_AVAILABLE
@@ -34,29 +42,30 @@
                 registries -- registries
                 update_on_instantiation -- set to false for manual update
         """
         self.container_engine = container_engine
         self.registries = registries
         self.all_tool_images = {}
 
-    def update(self, local_only = False, registry_only = False) -> None:
+    def update(self, local_only: bool = False, registry_only: bool = False, 
+               reg_selection: list[str] = []) -> None:
         """ Update the list of available tools.
         
             Args:
                 local_only -- update the local tools only
                 registry_only -- update the registry tools only
         """
         registry_tool_image_names = []
         local_tool_image_names = []
 
         if not registry_only:
             local_tool_image_names = self.container_engine.get_local_tool_images()
 
         if not local_only:
-            registry_tool_image_names = self.registries.list_repos()
+            registry_tool_image_names = self.registries.list_repos(reg_selection)
 
         for tool_image_name in local_tool_image_names:
             tool_image = ToolImage(tool_image_name)
             if tool_image_name in registry_tool_image_names:
                 tool_image.availability = ToolImage.LOCAL_AND_REGISTRY
             else:
                 tool_image.availability = ToolImage.LOCAL_ONLY
```

### Comparing `axem_dem-0.4.0/dem/core/user_output.py` & `axem_dem-0.5.0/dem/core/user_output.py`

 * *Files identical despite different names*

### Comparing `axem_dem-0.4.0/pyproject.toml` & `axem_dem-0.5.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "axem-dem"
-version = "0.4.0"
+version = "0.5.0"
 description = "Manager for Containerized Development Environments"
 authors = ["Janos Murai <janos.murai@axemsolutions.io>"]
 license = "Eclipse Public License - v2.0"
 readme = "README.md"
 homepage = "https://axemsolutions.io/"
 documentation = "https://axemsolutions.io/dem_doc/"
 repository = "https://github.com/axem-solutions/dem"
@@ -24,34 +24,34 @@
 packages = [{include = "dem"}]
 
 [tool.poetry.scripts]
 dem = "dem.__main__:main"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-docker = "6.1.3"
-readchar = "4.0.5"
-requests = "2.31.0"
-rich = "13.4.2"
-typer = "0.9.0"
+docker = "^7.0.0"
+readchar = "^4.0.6"
+requests = "^2.31.0"
+rich = "^13.7.1"
+typer = "^0.12.2"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-mkdocs-material = "^9.1.7"
+mkdocs-material = "^9.5.17"
 mike = "^2.0.0"
 jinja2 = "^3.1.3"
 
 [tool.poetry.group.test]
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.3.1"
-mock = "^5.0.2"
-pytest-cov = "^4.1.0"
+pytest = "^8.1.1"
+mock = "^5.1.0"
+pytest-cov = "^5.0.0"
 
 [tool.coverage.report]
 # Regexes for lines to exclude from consideration
 exclude_also = [
     "if __name__ == .__main__.:",
 ]
```

### Comparing `axem_dem-0.4.0/PKG-INFO` & `axem_dem-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: axem-dem
-Version: 0.4.0
+Version: 0.5.0
 Summary: Manager for Containerized Development Environments
 Home-page: https://axemsolutions.io/
 License: Eclipse Public License - v2.0
 Keywords: iot,embedded,edge,development environment,tools,containers
 Author: Janos Murai
 Author-email: janos.murai@axemsolutions.io
 Requires-Python: >=3.10,<4.0
@@ -18,19 +18,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: Software Development :: Testing
-Requires-Dist: docker (==6.1.3)
-Requires-Dist: readchar (==4.0.5)
-Requires-Dist: requests (==2.31.0)
-Requires-Dist: rich (==13.4.2)
-Requires-Dist: typer (==0.9.0)
+Requires-Dist: docker (>=7.0.0,<8.0.0)
+Requires-Dist: readchar (>=4.0.6,<5.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
+Requires-Dist: typer (>=0.12.2,<0.13.0)
 Project-URL: Documentation, https://axemsolutions.io/dem_doc/
 Project-URL: Repository, https://github.com/axem-solutions/dem
 Description-Content-Type: text/markdown
 
 <div align="center">
     <picture>
         <source media="(prefers-color-scheme: dark)" srcset="docs/wp-content/dem_logo_dark.png">
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: axem-dem Version: 0.4.0 Summary: Manager for
+Metadata-Version: 2.1 Name: axem-dem Version: 0.5.0 Summary: Manager for
 Containerized Development Environments Home-page: https://axemsolutions.io/
 License: Eclipse Public License - v2.0 Keywords: iot,embedded,edge,development
 environment,tools,containers Author: Janos Murai Author-email:
 janos.murai@axemsolutions.io Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Environment :: Console Classifier:
 Intended Audience :: Developers Classifier: License :: Other/Proprietary
 License Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
 Software Development Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Compilers Classifier: Topic ::
 Software Development :: Debuggers Classifier: Topic :: Software Development ::
 Embedded Systems Classifier: Topic :: Software Development :: Testing Requires-
-Dist: docker (==6.1.3) Requires-Dist: readchar (==4.0.5) Requires-Dist:
-requests (==2.31.0) Requires-Dist: rich (==13.4.2) Requires-Dist: typer
-(==0.9.0) Project-URL: Documentation, https://axemsolutions.io/dem_doc/
-Project-URL: Repository, https://github.com/axem-solutions/dem Description-
-Content-Type: text/markdown
+Dist: docker (>=7.0.0,<8.0.0) Requires-Dist: readchar (>=4.0.6,<5.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-Dist: rich
+(>=13.7.1,<14.0.0) Requires-Dist: typer (>=0.12.2,<0.13.0) Project-URL:
+Documentation, https://axemsolutions.io/dem_doc/ Project-URL: Repository,
+https://github.com/axem-solutions/dem Description-Content-Type: text/markdown
                                   [DEM logo]
 
                     ************ DDeevveellooppmmeenntt EEnnvviirroonnmmeenntt MMaannaaggeerr
                                      ffoorr
                           EEmmbbeeddddeedd DDeevveellooppmmeenntt ************
        ******** MMaannaaggee yyoouurr iissoollaatteedd DDeevveellooppmmeenntt EEnnvviirroonnmmeennttss wwiitthh eeaassee ********
```

