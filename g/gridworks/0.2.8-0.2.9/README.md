# Comparing `tmp/gridworks-0.2.8.tar.gz` & `tmp/gridworks-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks-0.2.8.tar", max compression
+gzip compressed data, was "gridworks-0.2.9.tar", max compression
```

## Comparing `gridworks-0.2.8.tar` & `gridworks-0.2.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1065 2023-08-03 16:39:47.639297 gridworks-0.2.8/LICENSE
--rw-r--r--   0        0        0     5584 2023-08-03 16:40:08.451467 gridworks-0.2.8/README.md
--rw-r--r--   0        0        0     2562 2023-08-03 16:40:08.451467 gridworks-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      249 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/__init__.py
--rw-r--r--   0        0        0      208 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/__main__.py
--rw-r--r--   0        0        0    51618 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/actor_base.py
--rw-r--r--   0        0        0    18028 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/algo_utils.py
--rw-r--r--   0        0        0    12872 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/api_utils.py
--rw-r--r--   0        0        0     2016 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/base_api_types.py
--rw-r--r--   0        0        0      251 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/conversion_factors.py
--rw-r--r--   0        0        0        0 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/data_classes/__init__.py
--rw-r--r--   0        0        0    23522 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/data_classes/base_g_node.py
--rw-r--r--   0        0        0     6726 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/data_classes/g_node.py
--rw-r--r--   0        0        0     6405 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/data_classes/g_node_instance.py
--rw-r--r--   0        0        0     5011 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/data_classes/g_node_strategy.py
--rw-r--r--   0        0        0      694 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/data_classes/gps_point.py
--rw-r--r--   0        0        0     2498 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/data_classes/market_type.py
--rw-r--r--   0        0        0     1214 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/data_classes/supervisor_container.py
--rw-r--r--   0        0        0      131 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/dev_utils/__init__.py
--rw-r--r--   0        0        0     3391 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/dev_utils/algo_setup.py
--rw-r--r--   0        0        0     1238 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/__init__.py
--rw-r--r--   0        0        0      673 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/algo_cert_type.py
--rw-r--r--   0        0        0      990 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/core_g_node_role.py
--rw-r--r--   0        0        0     2547 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/g_node_role.py
--rw-r--r--   0        0        0      992 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/g_node_status.py
--rw-r--r--   0        0        0      933 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/gni_status.py
--rw-r--r--   0        0        0      563 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/market_price_unit.py
--rw-r--r--   0        0        0      590 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/market_quantity_unit.py
--rw-r--r--   0        0        0     1394 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/market_type_name.py
--rw-r--r--   0        0        0     1326 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/message_category.py
--rw-r--r--   0        0        0     1189 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/message_category_symbol.py
--rw-r--r--   0        0        0      626 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/recognized_currency_unit.py
--rw-r--r--   0        0        0     2734 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/strategy_name.py
--rw-r--r--   0        0        0     1081 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/supervisor_container_status.py
--rw-r--r--   0        0        0      795 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/enums/universe_type.py
--rw-r--r--   0        0        0      336 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/errors.py
--rw-r--r--   0        0        0     8749 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/gw_config.py
--rw-r--r--   0        0        0     2813 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/message.py
--rw-r--r--   0        0        0    17029 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/property_format.py
--rw-r--r--   0        0        0        0 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/py.typed
--rw-r--r--   0        0        0     9199 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/rest_api.py
--rw-r--r--   0        0        0     1476 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/types/__init__.py
--rw-r--r--   0        0        0    20321 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/types/base_g_node_gt.py
--rw-r--r--   0        0        0    24525 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/types/g_node_gt.py
--rw-r--r--   0        0        0    15787 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/types/g_node_instance_gt.py
--rw-r--r--   0        0        0     6719 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/types/gw_cert_id.py
--rw-r--r--   0        0        0     3502 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/types/heartbeat_a.py
--rw-r--r--   0        0        0        0 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/types/old_versions/__init__.py
--rw-r--r--   0        0        0     1838 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/types/old_versions/heartbeat_a_001.py
--rw-r--r--   0        0        0     5581 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/types/ready.py
--rw-r--r--   0        0        0     8098 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/types/sim_timestep.py
--rw-r--r--   0        0        0     6096 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/types/super_starter.py
--rw-r--r--   0        0        0    12069 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/types/supervisor_container_gt.py
--rw-r--r--   0        0        0     5788 2023-08-03 16:39:47.723298 gridworks-0.2.8/src/gridworks/utils.py
--rw-r--r--   0        0        0      788 2023-08-03 16:39:47.727298 gridworks-0.2.8/src/gridworks_test/__init__.py
--rw-r--r--   0        0        0     6947 2023-08-03 16:39:47.727298 gridworks-0.2.8/src/gridworks_test/stub_actors.py
--rw-r--r--   0        0        0     4047 2023-08-03 16:39:47.727298 gridworks-0.2.8/src/gridworks_test/wait.py
--rw-r--r--   0        0        0     7036 1970-01-01 00:00:00.000000 gridworks-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-08-16 17:05:28.527175 gridworks-0.2.9/LICENSE
+-rw-r--r--   0        0        0     5584 2023-08-16 17:05:28.527175 gridworks-0.2.9/README.md
+-rw-r--r--   0        0        0     2562 2023-08-16 17:05:54.973752 gridworks-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      249 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/__init__.py
+-rw-r--r--   0        0        0      208 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/__main__.py
+-rw-r--r--   0        0        0    51618 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/actor_base.py
+-rw-r--r--   0        0        0    18028 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/algo_utils.py
+-rw-r--r--   0        0        0    12872 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/api_utils.py
+-rw-r--r--   0        0        0     2016 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/base_api_types.py
+-rw-r--r--   0        0        0      251 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/conversion_factors.py
+-rw-r--r--   0        0        0        0 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/data_classes/__init__.py
+-rw-r--r--   0        0        0    23522 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/data_classes/base_g_node.py
+-rw-r--r--   0        0        0     6726 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/data_classes/g_node.py
+-rw-r--r--   0        0        0     6405 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/data_classes/g_node_instance.py
+-rw-r--r--   0        0        0     5011 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/data_classes/g_node_strategy.py
+-rw-r--r--   0        0        0      694 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/data_classes/gps_point.py
+-rw-r--r--   0        0        0     2498 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/data_classes/market_type.py
+-rw-r--r--   0        0        0     1214 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/data_classes/supervisor_container.py
+-rw-r--r--   0        0        0      131 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/dev_utils/__init__.py
+-rw-r--r--   0        0        0     3391 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/dev_utils/algo_setup.py
+-rw-r--r--   0        0        0     1238 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/enums/__init__.py
+-rw-r--r--   0        0        0      673 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/enums/algo_cert_type.py
+-rw-r--r--   0        0        0      990 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/enums/core_g_node_role.py
+-rw-r--r--   0        0        0     2547 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/enums/g_node_role.py
+-rw-r--r--   0        0        0      992 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/enums/g_node_status.py
+-rw-r--r--   0        0        0      933 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/enums/gni_status.py
+-rw-r--r--   0        0        0      563 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/enums/market_price_unit.py
+-rw-r--r--   0        0        0      590 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/enums/market_quantity_unit.py
+-rw-r--r--   0        0        0     1394 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/enums/market_type_name.py
+-rw-r--r--   0        0        0     1326 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/enums/message_category.py
+-rw-r--r--   0        0        0     1189 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/enums/message_category_symbol.py
+-rw-r--r--   0        0        0      626 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/enums/recognized_currency_unit.py
+-rw-r--r--   0        0        0     2734 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/enums/strategy_name.py
+-rw-r--r--   0        0        0     1081 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/enums/supervisor_container_status.py
+-rw-r--r--   0        0        0      795 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/enums/universe_type.py
+-rw-r--r--   0        0        0      336 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/errors.py
+-rw-r--r--   0        0        0     8749 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/gw_config.py
+-rw-r--r--   0        0        0     2813 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/message.py
+-rw-r--r--   0        0        0    17029 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/property_format.py
+-rw-r--r--   0        0        0        0 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/py.typed
+-rw-r--r--   0        0        0     9199 2023-08-16 17:05:28.615184 gridworks-0.2.9/src/gridworks/rest_api.py
+-rw-r--r--   0        0        0     1476 2023-08-16 17:05:28.619185 gridworks-0.2.9/src/gridworks/types/__init__.py
+-rw-r--r--   0        0        0    20321 2023-08-16 17:05:28.619185 gridworks-0.2.9/src/gridworks/types/base_g_node_gt.py
+-rw-r--r--   0        0        0    24525 2023-08-16 17:05:28.619185 gridworks-0.2.9/src/gridworks/types/g_node_gt.py
+-rw-r--r--   0        0        0    15787 2023-08-16 17:05:28.619185 gridworks-0.2.9/src/gridworks/types/g_node_instance_gt.py
+-rw-r--r--   0        0        0     6719 2023-08-16 17:05:28.619185 gridworks-0.2.9/src/gridworks/types/gw_cert_id.py
+-rw-r--r--   0        0        0     3502 2023-08-16 17:05:28.619185 gridworks-0.2.9/src/gridworks/types/heartbeat_a.py
+-rw-r--r--   0        0        0        0 2023-08-16 17:05:28.619185 gridworks-0.2.9/src/gridworks/types/old_versions/__init__.py
+-rw-r--r--   0        0        0     1838 2023-08-16 17:05:28.619185 gridworks-0.2.9/src/gridworks/types/old_versions/heartbeat_a_001.py
+-rw-r--r--   0        0        0     5581 2023-08-16 17:05:28.619185 gridworks-0.2.9/src/gridworks/types/ready.py
+-rw-r--r--   0        0        0     8098 2023-08-16 17:05:28.619185 gridworks-0.2.9/src/gridworks/types/sim_timestep.py
+-rw-r--r--   0        0        0     6096 2023-08-16 17:05:28.619185 gridworks-0.2.9/src/gridworks/types/super_starter.py
+-rw-r--r--   0        0        0    12069 2023-08-16 17:05:28.619185 gridworks-0.2.9/src/gridworks/types/supervisor_container_gt.py
+-rw-r--r--   0        0        0     5788 2023-08-16 17:05:28.619185 gridworks-0.2.9/src/gridworks/utils.py
+-rw-r--r--   0        0        0      788 2023-08-16 17:05:28.619185 gridworks-0.2.9/src/gridworks_test/__init__.py
+-rw-r--r--   0        0        0     6947 2023-08-16 17:05:28.619185 gridworks-0.2.9/src/gridworks_test/stub_actors.py
+-rw-r--r--   0        0        0     4259 2023-08-16 17:05:54.973752 gridworks-0.2.9/src/gridworks_test/wait.py
+-rw-r--r--   0        0        0     7036 1970-01-01 00:00:00.000000 gridworks-0.2.9/PKG-INFO
```

### Comparing `gridworks-0.2.8/LICENSE` & `gridworks-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/README.md` & `gridworks-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/pyproject.toml` & `gridworks-0.2.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks"
-version = "0.2.8"
+version = "0.2.9"
 description = "Gridworks"
 authors = ["GridWorks <gridworks@gridworks-consulting.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks"
 repository = "https://github.com/thegridelectric/gridworks"
 documentation = "https://gridworks.readthedocs.io"
```

### Comparing `gridworks-0.2.8/src/gridworks/actor_base.py` & `gridworks-0.2.9/src/gridworks/actor_base.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/algo_utils.py` & `gridworks-0.2.9/src/gridworks/algo_utils.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/api_utils.py` & `gridworks-0.2.9/src/gridworks/api_utils.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/base_api_types.py` & `gridworks-0.2.9/src/gridworks/base_api_types.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/data_classes/base_g_node.py` & `gridworks-0.2.9/src/gridworks/data_classes/base_g_node.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/data_classes/g_node.py` & `gridworks-0.2.9/src/gridworks/data_classes/g_node.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/data_classes/g_node_instance.py` & `gridworks-0.2.9/src/gridworks/data_classes/g_node_instance.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/data_classes/g_node_strategy.py` & `gridworks-0.2.9/src/gridworks/data_classes/g_node_strategy.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/data_classes/gps_point.py` & `gridworks-0.2.9/src/gridworks/data_classes/gps_point.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/data_classes/market_type.py` & `gridworks-0.2.9/src/gridworks/data_classes/market_type.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/data_classes/supervisor_container.py` & `gridworks-0.2.9/src/gridworks/data_classes/supervisor_container.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/dev_utils/algo_setup.py` & `gridworks-0.2.9/src/gridworks/dev_utils/algo_setup.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/enums/__init__.py` & `gridworks-0.2.9/src/gridworks/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/enums/algo_cert_type.py` & `gridworks-0.2.9/src/gridworks/enums/algo_cert_type.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/enums/core_g_node_role.py` & `gridworks-0.2.9/src/gridworks/enums/core_g_node_role.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/enums/g_node_role.py` & `gridworks-0.2.9/src/gridworks/enums/g_node_role.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/enums/g_node_status.py` & `gridworks-0.2.9/src/gridworks/enums/g_node_status.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/enums/gni_status.py` & `gridworks-0.2.9/src/gridworks/enums/gni_status.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/enums/market_price_unit.py` & `gridworks-0.2.9/src/gridworks/enums/market_price_unit.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/enums/market_quantity_unit.py` & `gridworks-0.2.9/src/gridworks/enums/market_quantity_unit.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/enums/market_type_name.py` & `gridworks-0.2.9/src/gridworks/enums/market_type_name.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/enums/message_category.py` & `gridworks-0.2.9/src/gridworks/enums/message_category.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/enums/message_category_symbol.py` & `gridworks-0.2.9/src/gridworks/enums/message_category_symbol.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/enums/recognized_currency_unit.py` & `gridworks-0.2.9/src/gridworks/enums/recognized_currency_unit.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/enums/strategy_name.py` & `gridworks-0.2.9/src/gridworks/enums/strategy_name.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/enums/supervisor_container_status.py` & `gridworks-0.2.9/src/gridworks/enums/supervisor_container_status.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/enums/universe_type.py` & `gridworks-0.2.9/src/gridworks/enums/universe_type.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/gw_config.py` & `gridworks-0.2.9/src/gridworks/gw_config.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/message.py` & `gridworks-0.2.9/src/gridworks/message.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/property_format.py` & `gridworks-0.2.9/src/gridworks/property_format.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/rest_api.py` & `gridworks-0.2.9/src/gridworks/rest_api.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/types/__init__.py` & `gridworks-0.2.9/src/gridworks/types/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/types/base_g_node_gt.py` & `gridworks-0.2.9/src/gridworks/types/base_g_node_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/types/g_node_gt.py` & `gridworks-0.2.9/src/gridworks/types/g_node_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/types/g_node_instance_gt.py` & `gridworks-0.2.9/src/gridworks/types/g_node_instance_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/types/gw_cert_id.py` & `gridworks-0.2.9/src/gridworks/types/gw_cert_id.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/types/heartbeat_a.py` & `gridworks-0.2.9/src/gridworks/types/heartbeat_a.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/types/old_versions/heartbeat_a_001.py` & `gridworks-0.2.9/src/gridworks/types/old_versions/heartbeat_a_001.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/types/ready.py` & `gridworks-0.2.9/src/gridworks/types/ready.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/types/sim_timestep.py` & `gridworks-0.2.9/src/gridworks/types/sim_timestep.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/types/super_starter.py` & `gridworks-0.2.9/src/gridworks/types/super_starter.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/types/supervisor_container_gt.py` & `gridworks-0.2.9/src/gridworks/types/supervisor_container_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks/utils.py` & `gridworks-0.2.9/src/gridworks/utils.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks_test/__init__.py` & `gridworks-0.2.9/src/gridworks_test/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks_test/stub_actors.py` & `gridworks-0.2.9/src/gridworks_test/stub_actors.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.8/src/gridworks_test/wait.py` & `gridworks-0.2.9/src/gridworks_test/wait.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,34 +67,41 @@
     f_is_async = inspect.iscoroutinefunction(f)
     result = False
     if now >= until:
         if f_is_async:
             result = await f()
         else:
             result = f()
-    while now < until and result is False:
+    while now < until and not result:
         if f_is_async:
             result = await f()
         else:
             result = f()
-        if result is False:
+        if not result:
             now = time.time()
             if now < until:
                 await asyncio.sleep(min(retry_duration, until - now))
                 now = time.time()
-    if result is True:
+                # oops! we overslept
+                if now >= until:
+                    if f_is_async:
+                        result = await f()
+                    else:
+                        result = f()
+    if result:
         return True
     else:
         caller = getframeinfo(stack()[1][0])
         format_dict = dict(
             tag=tag,
             file=Path(caller.filename).name,
             line=caller.lineno,
             seconds=time.time() - start,
             f=f,
+            p=f(),
             err_str=err_str_f_(),
         )
         err_str = err_format.format(**format_dict)
         if error_dict is not None:
             error_dict.update(
                 format_dict,
                 err_str=err_str,
```

### Comparing `gridworks-0.2.8/PKG-INFO` & `gridworks-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridworks
-Version: 0.2.8
+Version: 0.2.9
 Summary: Gridworks
 Home-page: https://github.com/thegridelectric/gridworks
 License: MIT
 Author: GridWorks
 Author-email: gridworks@gridworks-consulting.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

