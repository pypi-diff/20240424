# Comparing `tmp/ck_apstra_api-0.3.1.tar.gz` & `tmp/ck_apstra_api-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ck_apstra_api-0.3.1.tar", max compression
+gzip compressed data, was "ck_apstra_api-0.3.2.tar", max compression
```

## Comparing `ck_apstra_api-0.3.1.tar` & `ck_apstra_api-0.3.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2023-09-28 00:59:26.688335 ck_apstra_api-0.3.1/LICENSE
--rw-r--r--   0        0        0     1226 2023-11-24 23:30:58.367886 ck_apstra_api-0.3.1/README.md
--rw-r--r--   0        0        0     1159 2024-04-21 00:40:15.531353 ck_apstra_api-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-09-28 01:27:34.624568 ck_apstra_api-0.3.1/src/ck_apstra_api/__init__.py
--rwxr-xr-x   0        0        0    31684 2024-04-20 23:59:53.359425 ck_apstra_api-0.3.1/src/ck_apstra_api/apstra_blueprint.py
--rwxr-xr-x   0        0        0     8554 2024-03-11 19:18:58.683250 ck_apstra_api-0.3.1/src/ck_apstra_api/apstra_session.py
--rw-r--r--   0        0        0     9265 2023-11-29 15:30:29.638239 ck_apstra_api-0.3.1/src/ck_apstra_api/cli.py
--rw-r--r--   0        0        0    27801 2024-04-20 21:55:03.988787 ck_apstra_api-0.3.1/src/ck_apstra_api/generic_system.py
--rw-r--r--   0        0        0    11866 2023-10-23 01:37:34.339126 ck_apstra_api-0.3.1/src/ck_apstra_api/ip_endpoint.py
--rw-r--r--   0        0        0     2346 2023-11-17 18:23:57.618869 ck_apstra_api-0.3.1/src/ck_apstra_api/pull_device_configuration.py
--rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 ck_apstra_api-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-09-28 00:59:26.688335 ck_apstra_api-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1226 2023-11-24 23:30:58.367886 ck_apstra_api-0.3.2/README.md
+-rw-r--r--   0        0        0     1159 2024-04-23 22:16:41.771405 ck_apstra_api-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-09-28 01:27:34.624568 ck_apstra_api-0.3.2/src/ck_apstra_api/__init__.py
+-rwxr-xr-x   0        0        0    32668 2024-04-23 19:17:44.299909 ck_apstra_api-0.3.2/src/ck_apstra_api/apstra_blueprint.py
+-rwxr-xr-x   0        0        0     8468 2024-04-23 18:59:16.565550 ck_apstra_api-0.3.2/src/ck_apstra_api/apstra_session.py
+-rw-r--r--   0        0        0     9265 2023-11-29 15:30:29.638239 ck_apstra_api-0.3.2/src/ck_apstra_api/cli.py
+-rw-r--r--   0        0        0    25422 2024-04-23 21:12:17.400215 ck_apstra_api-0.3.2/src/ck_apstra_api/generic_system.py
+-rw-r--r--   0        0        0    11866 2023-10-23 01:37:34.339126 ck_apstra_api-0.3.2/src/ck_apstra_api/ip_endpoint.py
+-rw-r--r--   0        0        0     2346 2023-11-17 18:23:57.618869 ck_apstra_api-0.3.2/src/ck_apstra_api/pull_device_configuration.py
+-rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 ck_apstra_api-0.3.2/PKG-INFO
```

### Comparing `ck_apstra_api-0.3.1/LICENSE` & `ck_apstra_api-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ck_apstra_api-0.3.1/README.md` & `ck_apstra_api-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ck_apstra_api-0.3.1/pyproject.toml` & `ck_apstra_api-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ck-apstra-api"
-version = "0.3.1"
+version = "0.3.2"
 description = "An implementation to use Apstra API"
 authors = [ "Charlie Kim <ckim@juniper.net>" ]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "<3.13,>=3.11"
```

### Comparing `ck_apstra_api-0.3.1/src/ck_apstra_api/apstra_blueprint.py` & `ck_apstra_api-0.3.2/src/ck_apstra_api/apstra_blueprint.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,60 +274,72 @@
         """
         ct_list, error = self.query(ct_list_query)
         if len(ct_list) == 0:
             self.logger.debug(f"No CTs found for {ct_labels=}")
             return []
         return [x['ep']['id'] for x in ct_list]
     
-    def add_generic_system(self, generic_system_spec: dict) -> list:
+    def add_generic_system(self, generic_system_spec: dict) -> Tuple[Optional[List], Optional[str]]:
         """
         Add a generic system (and access switch pair) to the blueprint.
 
         Args:
             generic_system_spec: The specification of the generic system.
 
         Returns:
             The ID of the switch-system-link ids.
         """
         new_generic_system_label = generic_system_spec['new_systems'][0]['label']
         existing_system_query = f"node('system', label='{new_generic_system_label}', name='system')"
         existing_system, error = self.query(existing_system_query)
         if len(existing_system) > 0:
             # skipping if the system already exists
-            return []
+            # return []
+            return [], None
         url = f"{self.url_prefix}/switch-system-links"
         created_generic_system = self.session.session.post(url, json=generic_system_spec)
         if created_generic_system.status_code >= 400:
-            self.logger.error(f"System not created: {created_generic_system=}, {new_generic_system_label=}, {created_generic_system.text=}")
-            return []
+            # self.logger.error(f"System not created: {created_generic_system=}, {new_generic_system_label=}, {created_generic_system.text=}")
+            return [], f"System not created: {created_generic_system=}, {new_generic_system_label=}, {created_generic_system.text=}"
+        # which case?
         if created_generic_system is None or len(created_generic_system.json()) == 0 or 'ids' not in created_generic_system.json():
-            return []
-        return created_generic_system.json()['ids']
+            return [], None
+        return created_generic_system.json()['ids'], None
 
-    def get_transformation_id(self, system_label, intf_name, speed) -> int:
+    def get_transformation_id(self, system_label, intf_name, speed) -> Tuple[Optional[int], Optional[str]]:
         '''
         Get the transformation ID for the interface
 
         Args:
             system_label: The label of the system
             intf_name: The name of the interface
             speed: The speed of the interface in the format of '10G'
         '''
+        # the unit is in uppercase
+        speed = speed.upper()
         system_im, error = self.get_system_with_im(system_label)
-        device_profile = self.session.get_device_profile(system_im['im']['device_profile_id'])
-
+        if error:
+            return None, f"{system_label=} {intf_name=} {speed=}\n\tError get_system_with_im {error=}"
+        device_profile, error = self.session.get_device_profile(system_im['im']['device_profile_id'])
+        if error:
+            return None, f"{system_label=} {intf_name=} {speed=}\n\tError get_device_profile {error=}"
+        if 'ports' not in device_profile:
+            return None, f"{system_label=} {intf_name=} {speed=}\n\tError: no ports in device profile {device_profile=}"
         for port in device_profile['ports']:
+            if 'transformations' not in port:
+                return None, f"{system_label=} {intf_name=} {speed=}\n\tError: no transformations in port {port=}"         
             for transformation in port['transformations']:
                 # self.logger.debug(f"{transformation=}")
                 for intf in transformation['interfaces']:
                     # if intf['name'] == intf_name:
                     #     self.logger.debug(f"{intf=}")
                     if intf['name'] == intf_name and intf['speed']['unit'] == speed[-1:] and intf['speed']['value'] == int(speed[:-1]): 
                         # self.logger.warning(f"{intf_name=}, {intf=}")
-                        return transformation['transformation_id']
+                        return transformation['transformation_id'], None
+        return None, f"transformation not found for {system_label=} {intf_name=} {speed=}"
 
     def patch_leaf_server_link(self, link_spec: dict) -> None:
         """
         Patch a leaf-server link.
 
         Args:
             link_spec: The specification of the leaf-server link.
```

### Comparing `ck_apstra_api-0.3.1/src/ck_apstra_api/apstra_session.py` & `ck_apstra_api-0.3.2/src/ck_apstra_api/apstra_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 #!/usr/bin/env python3
+from functools import cache
+from typing import Optional, Tuple
 import requests
 import urllib3
 import logging
 import time
 from datetime import datetime
 
 
@@ -120,32 +122,32 @@
         Check if the Apstra controller is online.
 
         Returns:
             True if the Apstra controller is online, False otherwise.
         """
         return self.token is not None
 
-    def get_device_profile(self, device_profile_name: str = None) -> dict:
+
+    @cache
+    def get_device_profile(self, device_profile_name: str = None) -> Tuple[Optional[dict], Optional[str]]:
         """
         Get the device profile with the specified name.
 
         Args:
             name: The name of the device profile.
 
         Returns:
             The device profile, or None if the device profile does not exist.
         """
         if device_profile_name is None:
-            self.logger.warning("name is None")
-            return None
-        if device_profile_name not in self.device_profile_cache:
-            # url = f"{self.url_prefix}/device-profiles"
-            device_profiles = self.get_items('device-profiles')['items']
-            self.device_profile_cache[device_profile_name] = [x for x in device_profiles if x['id'] == device_profile_name][0]
-        return self.device_profile_cache[device_profile_name]
+            return None, f"Error: {device_profile_name=}"
+        device_profiles = self.get_items('device-profiles')['items']
+        the_device_profile = [x for x in device_profiles if x['id'] == device_profile_name][0]
+        return the_device_profile, None
+
 
     def get_logical_device(self, id: int) -> dict:
         """
         Get the logical device with the specified ID.
 
         Args:
             id: The ID of the logical device.
```

### Comparing `ck_apstra_api-0.3.1/src/ck_apstra_api/cli.py` & `ck_apstra_api-0.3.2/src/ck_apstra_api/cli.py`

 * *Files identical despite different names*

### Comparing `ck_apstra_api-0.3.1/src/ck_apstra_api/generic_system.py` & `ck_apstra_api-0.3.2/src/ck_apstra_api/generic_system.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,124 +1,19 @@
 
 import logging
 from math import isnan
 from pathlib import Path
-from pydantic import BaseModel, validator, StrictStr, field_validator, Field
 from typing import List, Optional, Any, Tuple, TypeVar, Annotated
 import os
 import uuid
 
 from ck_apstra_api.apstra_session import CkApstraSession
 from ck_apstra_api.apstra_blueprint import CkApstraBlueprint, CkEnum
 
-class GenericSystemModel(BaseModel):
-    """
-    The variables from the excel sheet generic_systems
-    """
-    blueprint: str
-    system_label: str
-    is_external: Optional[bool] = False
-    speed: str               # 10G 
-    lag_mode: Optional[str]  # mandatory in case of multiple interfaces
-    tags: List[str] = Field(default = [])  # deprecated
-    gs_tags: List[str] = Field(default = [])
-
-    label1: str
-    ifname1: str
-    gs_ifname1: Optional[str]
-    tags1: List[str] = Field(default = [])
-
-    label2: Optional[str]
-    ifname2: Optional[str]
-    gs_ifname2: Optional[str]
-    tags2: List[str] = Field(default = [])
-
-    label3: Optional[str]
-    ifname3: Optional[str]
-    gs_ifname3: Optional[str]
-    tags3: List[str] = Field(default = [])
-
-    label4: Optional[str]
-    ifname4: Optional[str]
-    gs_ifname4: Optional[str]
-    tags4: List[str] = Field(default = [])
-
-    untagged_vlan: Optional[int] = None
-    tagged_vlans: Optional[List[int]] = None
-    ct_names: Optional[List[str]] = None
-    comment: Optional[str] = None
-
-    # convert to string in case an int is given
-    @field_validator('gs_ifname1', 'gs_ifname2', 'gs_ifname3', 'gs_ifname4', mode='before')
-    @classmethod
-    def conver_to_string(cls, v):
-        if v is None:
-            return None
-        if isinstance(v, str):
-            return v
-        return str(v)
-
-    @field_validator('tagged_vlans', mode='before')
-    @classmethod
-    def convert_to_list_of_int(cls, v):
-        if v is None:
-            return None
-        if isinstance(v, int):
-            return [v]
-        return [ x.strip() for x in v.split(',')]
-
-    @field_validator('is_external', mode='before')
-    @classmethod
-    def convert_to_bool(cls, v):
-        if isinstance(v, str) and v == 'yes':
-            return True
-        return False
-
-    @field_validator('tags', 'gs_tags', 'tags1', 'tags2', 'tags3', 'tags4', 'ct_names', mode='before')
-    @classmethod
-    def convert_to_list_of_str(cls, v):
-        if v is None:
-            return []
-        return [ x.strip() for x in v.split(',')]
-
-generic_system_data = {} # { blueprint: { generic_system: {....}}}
-
-
-def process_row(row):
-    blueprint_label = row['blueprint']
-    blueprint_data = generic_system_data.setdefault(blueprint_label, {})
-    system_label = row['system_label']
-    system_data = blueprint_data.setdefault(system_label,[])
-    # logging.debug(f"{generic_system_data}")
-    pydantic_data = GenericSystemModel(**row)
-    system_data.append(pydantic_data.model_dump())
-    # logging.debug(f"{pydantic_data=}")
-
-
-def read_generic_systems(input_file_path_string: str = None, sheet_name: str = 'generic_systems'):
-    excel_file_sting = input_file_path_string or os.getenv('excel_input_file')
-    input_file_path = Path(excel_file_sting) 
-    df = pd.read_excel(input_file_path, sheet_name=sheet_name, header=[1])
-    df = df.replace({np.nan: None})
-
-    df.apply(process_row, axis=1)
-    return generic_system_data
-
-# @click.command(name='read-generic-systems')
-# def click_read_generic_systems():
-#     job_env = CkJobEnv()
-#     generic_systems = read_generic_systems(job_env.excel_input_file, 'generic_systems')
-#     for bp_label, bp_data in generic_systems.items():
-#         logging.debug(f"{bp_label=}")
-#         for gs_label, gs_links_list in bp_data.items():
-#             logging.debug(f"{gs_label=}")
-#             for link in gs_links_list:
-#                 logging.debug(f"{link=}")
 
-# def form_lacp(job_env: CkJobEnv, generic_system_label: str, generic_system_links_list: list):
 def form_lacp(apstra_bp, generic_system_label: str, generic_system_links_list: list):
     # bp = job_env.main_bp
     bp = apstra_bp
     bp_label = bp.label
     lag_spec = {
         'links': {
             # <link_node_id>: {
@@ -130,33 +25,34 @@
     link_id_num = 0
     for link in generic_system_links_list:
         lag_mode = link['lag_mode']
         if lag_mode is None:
             # logging.debug(f"Skipping: Generic system {generic_system_label} has no lag_mode")
             continue                
         if lag_mode not in [ 'lacp_active', 'lacp_passive']:
-            logging.warning(f"Skipping: Generic system {generic_system_label} has invalid lag_mode {lag_mode}")
+            logging.warning(f"form_lacp Skipping: Generic system {generic_system_label} has invalid lag_mode {lag_mode}")
             continue
         link_id_num += 1
         group_label = f"link{link_id_num}"
-        # iterate over the 4 member interfaces
+        # iterate over the 4 member interfaces and links list
         for member_number in range(4):
             member_number += 1
             sw_label = link[f"label{member_number}"] if f"label{member_number}" in link else link[f"switch{member_number}"]
             sw_ifname = link[f"ifname{member_number}"] if f"ifname{member_number}" in link else link[f"switch_intf{member_number}"]
             gs_ifname = link[f"gs_ifname{member_number}"] if f"gs_ifname{member_number}" in link else link[f"server_intf{member_number}"]
             # skip if now switch is defined
             if not sw_label or not sw_ifname:
                 continue
             if sw_ifname[:2] not in ['et', 'xe', 'ge']:
-                logging.warning(f"Skipping: Generic system {generic_system_label} has invalid interface name {sw_ifname}")
+                # TODO: should fail on input validation
+                logging.warning(f"form_lacp Skipping: Switch for {generic_system_label}, {sw_ifname[:2]} has invalid interface name {sw_ifname}:{sw_ifname}")
                 continue
             switch_link_nodes = bp.get_switch_interface_nodes([sw_label], sw_ifname)
             if switch_link_nodes is None or len(switch_link_nodes) == 0:
-                logging.warning(f"Skipping: Generic system {generic_system_label} has invalid interface {sw_label}:{sw_ifname}")
+                logging.warning(f"form_lacp Skipping: Generic system {generic_system_label} has invalid interface {sw_label}:{sw_ifname}")
                 continue
             link_node_id = switch_link_nodes[0][CkEnum.LINK]['id']
             sw_if_node_id = switch_link_nodes[0][CkEnum.MEMBER_INTERFACE]['id']
             gs_if_node_id = switch_link_nodes[0][CkEnum.GENERIC_SYSTEM_INTERFACE]['id']
             link_spec = {
                 'group_label': group_label,
                 'lag_mode': lag_mode,
@@ -178,14 +74,16 @@
 def add_tags(apstra_bp, generic_system_label: str, generic_system_links_list: list) -> Tuple[Optional[str], Optional[str]]:
     bp = apstra_bp
     link_id_num = 0
     generic_system_node, error = bp.get_system_node_from_label(generic_system_label)
     if error:
         logging.warning(f"add_tags skipping: {error}")
         return None, f"add_tags {generic_system_label} not found in blueprint {bp.label}"
+    if not generic_system_node:
+        return None, f"add_tags {generic_system_label} not found in blueprint {bp.label}"
     generic_system_id = generic_system_node['id']
     for link in generic_system_links_list:
         link_id_num += 1
         group_label = f"link{link_id_num}"
         gs_tags = link['gs_tags']
         if len(gs_tags) > 0:
             bp.post_tagging(generic_system_id, tags_to_add=gs_tags)            
@@ -210,15 +108,15 @@
                 continue
             link_node_id = switch_link_nodes[0][CkEnum.LINK]['id']
             # logging.debug(f"{member_tags=}")
             if len(member_tags) > 0:
                 logging.debug(f"{member_tags=}")
                 bp.post_tagging(link_node_id, tags_to_add=member_tags)
                 
-
+    return None, None
 
 # def rename_generic_system_intf(job_env: CkJobEnv, generic_system_label: str, generic_system_links_list: list):
 #     bp = job_env.main_bp
 def rename_generic_system_intf(apstra_bp, generic_system_label: str, generic_system_links_list: list):
     bp = apstra_bp
     bp_label = bp.label
     patch_cable_map_spec = {
@@ -399,15 +297,16 @@
     }
     # to form logical device
     speed_count = {}
     system_type = 'server'
 
     for link in gs_links_list:
     #     logging.debug(f"{link=}")
-        link_speed = link['speed']
+        # make sure upper case
+        link_speed = link['speed'].upper()
         system_type = 'external' if link['is_external'] else 'server'
         for link_id_num in range(1, 5):
             # link_id_num = link_number + 1
             switch_label = link[f"switch{link_id_num}"]
             this_ifname = link[f"switch_intf{link_id_num}"]
             # skip if data is missing
             if not switch_label:
@@ -418,19 +317,27 @@
                 return None, error_message
             logging.debug(f"{switch_label=}")
             switch_node, error = bp.get_system_node_from_label(switch_label)
             if error:
                 error_message = f"Error: generic system {gs_label} has absent switch {switch_label}\n\tFrom get_system_node_from_label {error}"
                 # logging.warning(f"add_single_generic_system {error_message}")
                 return None, error_message
+            if not switch_node:
+                return None, f"Error: {switch_label} not found in blueprint {bp.label}"
             switch_id = switch_node['id']
+            transformation_id, error = bp.get_transformation_id(switch_label, this_ifname , link_speed)
+            if error:
+                error_message = f"Error: generic system {gs_label} has absent transformation {switch_label}:{this_ifname}\n\tFrom get_transformation_id {error}"
+                logging.warning(f"add_single_generic_system {error_message}")
+                return None, error_message
             link_spec = {
                 'switch': {
                     'system_id': switch_id,
-                    'transformation_id': bp.get_transformation_id(link[f"switch{link_id_num}"], this_ifname , link_speed),
+                    # 'transformation_id': bp.get_transformation_id(link[f"switch{link_id_num}"], this_ifname , link_speed),
+                    'transformation_id': transformation_id,
                     'if_name': link[f"switch_intf{link_id_num}"],
                 },
                 'system': {
                     'system_id': None,
                 },
                 # 'lag_mode':link['lag_mode'],
                 'lag_mode': None,
@@ -492,16 +399,19 @@
         new_system['logical_device']['panels'][0]['port_groups'].append(port_group)
         display_name = f"{display_name}-{count}x{speed}"
     new_system['logical_device']['display_name'] = display_name
     new_system['logical_device']['id'] = display_name
     generic_system_spec['new_systems'].append(new_system)
     logging.debug(f"add_single_generic_system {generic_system_spec=}, {speed_count=}")
 
-    generic_system_created = bp.add_generic_system(generic_system_spec)
-    logging.info(f"add_single_generic_system {gs_label} created in blueprint {bp.label}")
+    generic_system_created, error = bp.add_generic_system(generic_system_spec)
+    if error:
+        error_message = f"Error: generic system {gs_label} not created\n\tFrom add_generic_system {error}"
+        # logging.warning(error_message)
+        return None, error_message
 
     return None, None
                                                                              
 
 def add_generic_system(apstra_session, generic_systems: dict) -> Tuple[Optional[str], Optional[str]]:
     """
     Add a single generic system to the Apstra server from the given generic systems data.
@@ -562,15 +472,19 @@
             if error:
                 logging.warning(f"add_generic_system Error for {gs_label=}:\n\tFrom add_single_generic_system: {error}")
                 # return None, f"add_generic_system {error}"
 
         ## form LACP in the BP iterating over the generic systems
         for gs_label, gs_links_list in bp_data.items():
             form_lacp(bp, gs_label, gs_links_list)
-            add_tags(bp, gs_label, gs_links_list)
+            _, error = add_tags(bp, gs_label, gs_links_list)
+            if error:
+                logging.warning(f"add_generic_system Error for {gs_label=}:\n\tFrom add_tags: {error}")
+                # return None, f"add_generic_system {error}"
+                continue
             rename_generic_system_intf(bp, gs_label, gs_links_list)
 
             # # update connectivity templates - this should be run after lag update
             # assign_connectivity_templates(job_env, gs_label, gs_links_list)
             assign_connectivity_templates(bp, gs_label, gs_links_list)
 
         return None, None
```

### Comparing `ck_apstra_api-0.3.1/src/ck_apstra_api/ip_endpoint.py` & `ck_apstra_api-0.3.2/src/ck_apstra_api/ip_endpoint.py`

 * *Files identical despite different names*

### Comparing `ck_apstra_api-0.3.1/src/ck_apstra_api/pull_device_configuration.py` & `ck_apstra_api-0.3.2/src/ck_apstra_api/pull_device_configuration.py`

 * *Files identical despite different names*

### Comparing `ck_apstra_api-0.3.1/PKG-INFO` & `ck_apstra_api-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ck-apstra-api
-Version: 0.3.1
+Version: 0.3.2
 Summary: An implementation to use Apstra API
 License: MIT
 Author: Charlie Kim
 Author-email: ckim@juniper.net
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

