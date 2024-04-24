# Comparing `tmp/planet-2.6.tar.gz` & `tmp/planet-2.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/planet-client-python/planet-client-python/dist/.tmp-r_wbbgm7/planet-2.6.tar", last modified: Wed Apr 24 17:24:15 2024, max compression
+gzip compressed data, was "/home/runner/work/planet-client-python/planet-client-python/dist/.tmp-qffvu8xp/planet-2.6.dev0.tar", last modified: Mon Apr  8 22:07:10 2024, max compression
```

## Comparing `planet-2.6.tar` & `planet-2.6.dev0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:24:15.000000 planet-2.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-04-24 17:23:57.000000 planet-2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-24 17:24:15.000000 planet-2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-24 17:23:57.000000 planet-2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:24:15.000000 planet-2.6/planet/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-24 17:23:57.000000 planet-2.6/planet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-24 17:23:57.000000 planet-2.6/planet/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-04-24 17:23:57.000000 planet-2.6/planet/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:24:15.000000 planet-2.6/planet/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 17:23:57.000000 planet-2.6/planet/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-24 17:23:57.000000 planet-2.6/planet/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-24 17:23:57.000000 planet-2.6/planet/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-24 17:23:57.000000 planet-2.6/planet/cli/cmds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-24 17:23:57.000000 planet-2.6/planet/cli/collect.py
--rw-r--r--   0 runner    (1001) docker     (127)    21836 2024-04-24 17:23:57.000000 planet-2.6/planet/cli/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-24 17:23:57.000000 planet-2.6/planet/cli/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-24 17:23:57.000000 planet-2.6/planet/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    11842 2024-04-24 17:23:57.000000 planet-2.6/planet/cli/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-24 17:23:57.000000 planet-2.6/planet/cli/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    15189 2024-04-24 17:23:57.000000 planet-2.6/planet/cli/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-24 17:23:57.000000 planet-2.6/planet/cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:24:15.000000 planet-2.6/planet/clients/
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-24 17:23:57.000000 planet-2.6/planet/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22413 2024-04-24 17:23:57.000000 planet-2.6/planet/clients/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-04-24 17:23:57.000000 planet-2.6/planet/clients/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-04-24 17:23:57.000000 planet-2.6/planet/clients/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-24 17:23:57.000000 planet-2.6/planet/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:24:15.000000 planet-2.6/planet/data/
--rw-r--r--   0 runner    (1001) docker     (127)    13778 2024-04-24 17:23:57.000000 planet-2.6/planet/data/Feature.json
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-24 17:23:57.000000 planet-2.6/planet/data/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    19154 2024-04-24 17:23:57.000000 planet-2.6/planet/data/orders_product_bundle_2023-02-24.json
--rw-r--r--   0 runner    (1001) docker     (127)    11237 2024-04-24 17:23:57.000000 planet-2.6/planet/data_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-24 17:23:57.000000 planet-2.6/planet/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-04-24 17:23:57.000000 planet-2.6/planet/geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)    16194 2024-04-24 17:23:57.000000 planet-2.6/planet/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-24 17:23:57.000000 planet-2.6/planet/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     9136 2024-04-24 17:23:57.000000 planet-2.6/planet/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    19195 2024-04-24 17:23:57.000000 planet-2.6/planet/order_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-04-24 17:23:57.000000 planet-2.6/planet/reporting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-04-24 17:23:57.000000 planet-2.6/planet/specs.py
--rw-r--r--   0 runner    (1001) docker     (127)    28569 2024-04-24 17:23:57.000000 planet-2.6/planet/subscription_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:24:15.000000 planet-2.6/planet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-24 17:24:15.000000 planet-2.6/planet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-24 17:24:15.000000 planet-2.6/planet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 17:24:15.000000 planet-2.6/planet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 17:24:15.000000 planet-2.6/planet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 17:24:15.000000 planet-2.6/planet.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-24 17:24:15.000000 planet-2.6/planet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 17:24:15.000000 planet-2.6/planet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-24 17:24:15.000000 planet-2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-24 17:23:57.000000 planet-2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:07:10.000000 planet-2.6.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-04-08 22:06:43.000000 planet-2.6.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-08 22:07:10.000000 planet-2.6.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-08 22:06:43.000000 planet-2.6.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/cmds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/collect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21836 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11842 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15160 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22413 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/clients/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/clients/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/clients/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    13778 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/data/Feature.json
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    19154 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/data/orders_product_bundle_2023-02-24.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11237 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/data_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16194 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9136 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19195 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/order_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/specs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28493 2024-04-08 22:06:43.000000 planet-2.6.dev0/planet/subscription_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 22:07:10.000000 planet-2.6.dev0/planet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-08 22:07:10.000000 planet-2.6.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-08 22:06:43.000000 planet-2.6.dev0/setup.py
```

### Comparing `planet-2.6/LICENSE` & `planet-2.6.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `planet-2.6/PKG-INFO` & `planet-2.6.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planet
-Version: 2.6
+Version: 2.6.dev0
 Summary: Planet SDK for Python
 Home-page: https://github.com/planetlabs/planet-client-python
 Author: Jennifer Reiber Kyle
 Maintainer: Planet Dev Rel Team
 Maintainer-email: developers@planet.com
 License: Apache 2.0
 Keywords: planet api sdk client
```

### Comparing `planet-2.6/README.md` & `planet-2.6.dev0/README.md`

 * *Files identical despite different names*

### Comparing `planet-2.6/planet/__init__.py` & `planet-2.6.dev0/planet/__init__.py`

 * *Files identical despite different names*

### Comparing `planet-2.6/planet/auth.py` & `planet-2.6.dev0/planet/auth.py`

 * *Files identical despite different names*

### Comparing `planet-2.6/planet/cli/auth.py` & `planet-2.6.dev0/planet/cli/auth.py`

 * *Files identical despite different names*

### Comparing `planet-2.6/planet/cli/cli.py` & `planet-2.6.dev0/planet/cli/cli.py`

 * *Files identical despite different names*

### Comparing `planet-2.6/planet/cli/cmds.py` & `planet-2.6.dev0/planet/cli/cmds.py`

 * *Files identical despite different names*

### Comparing `planet-2.6/planet/cli/collect.py` & `planet-2.6.dev0/planet/cli/collect.py`

 * *Files identical despite different names*

### Comparing `planet-2.6/planet/cli/data.py` & `planet-2.6.dev0/planet/cli/data.py`

 * *Files identical despite different names*

### Comparing `planet-2.6/planet/cli/io.py` & `planet-2.6.dev0/planet/cli/io.py`

 * *Files identical despite different names*

### Comparing `planet-2.6/planet/cli/options.py` & `planet-2.6.dev0/planet/cli/options.py`

 * *Files identical despite different names*

### Comparing `planet-2.6/planet/cli/orders.py` & `planet-2.6.dev0/planet/cli/orders.py`

 * *Files identical despite different names*

### Comparing `planet-2.6/planet/cli/subscriptions.py` & `planet-2.6.dev0/planet/cli/subscriptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -402,15 +402,14 @@
 @subscriptions.command()  # type: ignore
 @translate_exceptions
 @click.option(
     '--var-type',
     required=True,
     help='Planetary variable type.',
     type=click.Choice([
-        "analysis_ready_ps",
         "biomass_proxy",
         "land_surface_temperature",
         "soil_water_content",
         "vegetation_optical_depth",
         "forest_carbon_diligence_30m",
         "field_boundaries_sentinel_2_p1m"
     ]),
```

### Comparing `planet-2.6/planet/cli/types.py` & `planet-2.6.dev0/planet/cli/types.py`

 * *Files identical despite different names*

### Comparing `planet-2.6/planet/clients/__init__.py` & `planet-2.6.dev0/planet/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `planet-2.6/planet/clients/data.py` & `planet-2.6.dev0/planet/clients/data.py`

 * *Files identical despite different names*

### Comparing `planet-2.6/planet/clients/orders.py` & `planet-2.6.dev0/planet/clients/orders.py`

 * *Files identical despite different names*

### Comparing `planet-2.6/planet/clients/subscriptions.py` & `planet-2.6.dev0/planet/clients/subscriptions.py`

 * *Files identical despite different names*

### Comparing `planet-2.6/planet/constants.py` & `planet-2.6.dev0/planet/constants.py`

 * *Files identical despite different names*

### Comparing `planet-2.6/planet/data/Feature.json` & `planet-2.6.dev0/planet/data/Feature.json`

 * *Files identical despite different names*

### Comparing `planet-2.6/planet/data/README.md` & `planet-2.6.dev0/planet/data/README.md`

 * *Files identical despite different names*

### Comparing `planet-2.6/planet/data/orders_product_bundle_2023-02-24.json` & `planet-2.6.dev0/planet/data/orders_product_bundle_2023-02-24.json`

 * *Files identical despite different names*

### Comparing `planet-2.6/planet/data_filter.py` & `planet-2.6.dev0/planet/data_filter.py`

 * *Files identical despite different names*

### Comparing `planet-2.6/planet/exceptions.py` & `planet-2.6.dev0/planet/exceptions.py`

 * *Files identical despite different names*

### Comparing `planet-2.6/planet/geojson.py` & `planet-2.6.dev0/planet/geojson.py`

 * *Files identical despite different names*

### Comparing `planet-2.6/planet/http.py` & `planet-2.6.dev0/planet/http.py`

 * *Files identical despite different names*

### Comparing `planet-2.6/planet/io.py` & `planet-2.6.dev0/planet/io.py`

 * *Files identical despite different names*

### Comparing `planet-2.6/planet/models.py` & `planet-2.6.dev0/planet/models.py`

 * *Files identical despite different names*

### Comparing `planet-2.6/planet/order_request.py` & `planet-2.6.dev0/planet/order_request.py`

 * *Files identical despite different names*

### Comparing `planet-2.6/planet/reporting.py` & `planet-2.6.dev0/planet/reporting.py`

 * *Files identical despite different names*

### Comparing `planet-2.6/planet/specs.py` & `planet-2.6.dev0/planet/specs.py`

 * *Files identical despite different names*

### Comparing `planet-2.6/planet/subscription_request.py` & `planet-2.6.dev0/planet/subscription_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,16 +276,15 @@
     if time_range_type:
         parameters['time_range_type'] = time_range_type
 
     return {"type": "catalog", "parameters": parameters}
 
 
 def planetary_variable_source(
-    var_type: Literal["analysis_ready_ps",
-                      "biomass_proxy",
+    var_type: Literal["biomass_proxy",
                       "land_surface_temperature",
                       "soil_water_content",
                       "vegetation_optical_depth",
                       "forest_carbon_diligence_30m",
                       "field_boundaries_sentinel_2_p1m"],
     var_id: str,
     geometry: Mapping,
@@ -301,18 +300,17 @@
 
     The return value can be passed to
     [planet.subscription_request.build_request][].
 
     Note: this function does not validate variable types and ids.
 
     Parameters:
-        var_type: one of "analysis_ready_ps", "biomass_proxy",
-            "land_surface_temperature", "soil_water_content",
-            "vegetation_optical_depth", "forest_carbon_diligence_30m,
-            or field_boundaries_sentinel_2_p1m".
+        var_type: one of "biomass_proxy", "land_surface_temperature",
+            "soil_water_content", "vegetation_optical_depth",
+            "forest_carbon_diligence_30m, or field_boundaries_sentinel_2_p1m".
         var_id: a value such as "SWC-AMSR2-C_V1.0_100" for soil water
             content derived from AMSR2 C band.
         geometry: The area of interest of the subscription that will be
             used to determine matches.
         start_time: The start time of the subscription. This time can be
             in the past or future.
         end_time: The end time of the subscription. This time can be in
```

### Comparing `planet-2.6/planet.egg-info/PKG-INFO` & `planet-2.6.dev0/planet.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planet
-Version: 2.6
+Version: 2.6.dev0
 Summary: Planet SDK for Python
 Home-page: https://github.com/planetlabs/planet-client-python
 Author: Jennifer Reiber Kyle
 Maintainer: Planet Dev Rel Team
 Maintainer-email: developers@planet.com
 License: Apache 2.0
 Keywords: planet api sdk client
```

### Comparing `planet-2.6/planet.egg-info/SOURCES.txt` & `planet-2.6.dev0/planet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `planet-2.6/setup.py` & `planet-2.6.dev0/setup.py`

 * *Files identical despite different names*

