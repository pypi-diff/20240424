# Comparing `tmp/django_mapengine-1.4.1.tar.gz` & `tmp/django_mapengine-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_mapengine-1.4.1.tar", max compression
+gzip compressed data, was "django_mapengine-1.5.0.tar", max compression
```

## Comparing `django_mapengine-1.4.1.tar` & `django_mapengine-1.5.0.tar`

### file list

```diff
@@ -1,33 +1,35 @@
--rw-r--r--   0        0        0     1069 2024-03-12 15:15:44.559160 django_mapengine-1.4.1/LICENSE
--rw-r--r--   0        0        0     3373 2024-03-26 11:51:33.500776 django_mapengine-1.4.1/README.md
--rw-r--r--   0        0        0       60 2024-04-08 11:21:46.580386 django_mapengine-1.4.1/django_mapengine/__init__.py
--rw-r--r--   0        0        0     3034 2024-03-20 07:51:08.767681 django_mapengine-1.4.1/django_mapengine/apps.py
--rw-r--r--   0        0        0     6738 2024-03-12 15:15:44.559160 django_mapengine-1.4.1/django_mapengine/choropleth.py
--rw-r--r--   0        0        0    43608 2024-03-12 15:15:44.559160 django_mapengine-1.4.1/django_mapengine/colorbrewer.py
--rw-r--r--   0        0        0     2230 2024-03-26 11:51:33.500776 django_mapengine-1.4.1/django_mapengine/distill.py
--rw-r--r--   0        0        0     9505 2024-03-19 13:21:41.778113 django_mapengine-1.4.1/django_mapengine/layers.py
--rw-r--r--   0        0        0      928 2024-03-14 11:59:59.035708 django_mapengine-1.4.1/django_mapengine/legend.py
--rw-r--r--   0        0        0     2516 2024-03-14 11:59:59.039708 django_mapengine-1.4.1/django_mapengine/mvt.py
--rw-r--r--   0        0        0     2161 2023-06-14 12:49:56.418190 django_mapengine-1.4.1/django_mapengine/popups.py
--rw-r--r--   0        0        0     3394 2024-03-14 11:45:38.891732 django_mapengine-1.4.1/django_mapengine/setup.py
--rw-r--r--   0        0        0     5543 2024-03-19 11:27:28.550114 django_mapengine-1.4.1/django_mapengine/sources.py
--rw-r--r--   0        0        0     1023 2023-06-14 12:49:56.422190 django_mapengine-1.4.1/django_mapengine/static/django_mapengine/js/basemaps.js
--rw-r--r--   0        0        0     3220 2024-02-02 13:11:04.816042 django_mapengine-1.4.1/django_mapengine/static/django_mapengine/js/choropleth.js
--rw-r--r--   0        0        0      455 2024-03-12 15:15:44.559160 django_mapengine-1.4.1/django_mapengine/static/django_mapengine/js/events.js
--rw-r--r--   0        0        0      605 2023-06-14 12:49:56.422190 django_mapengine-1.4.1/django_mapengine/static/django_mapengine/js/helper.js
--rw-r--r--   0        0        0     1128 2023-08-23 11:10:37.048313 django_mapengine-1.4.1/django_mapengine/static/django_mapengine/js/init.js
--rw-r--r--   0        0        0     2693 2024-03-26 11:51:33.500776 django_mapengine-1.4.1/django_mapengine/static/django_mapengine/js/layer.js
--rw-r--r--   0        0        0     3069 2023-07-13 09:07:49.785869 django_mapengine-1.4.1/django_mapengine/static/django_mapengine/js/legend.js
--rw-r--r--   0        0        0     2412 2024-03-07 12:05:14.127045 django_mapengine-1.4.1/django_mapengine/static/django_mapengine/js/map.js
--rw-r--r--   0        0        0     2804 2024-03-12 15:15:49.899159 django_mapengine-1.4.1/django_mapengine/static/django_mapengine/js/popup.js
--rw-r--r--   0        0        0     2558 2023-06-14 12:49:56.422190 django_mapengine-1.4.1/django_mapengine/static/django_mapengine/js/regions.js
--rw-r--r--   0        0        0      513 2023-06-14 12:49:56.422190 django_mapengine-1.4.1/django_mapengine/static/django_mapengine/js/store.js
--rw-r--r--   0        0        0      355 2023-06-14 12:49:56.422190 django_mapengine-1.4.1/django_mapengine/templates/django_mapengine/map.html
--rw-r--r--   0        0        0     1203 2023-06-14 12:49:56.422190 django_mapengine-1.4.1/django_mapengine/templates/django_mapengine/map_basemaps.html
--rw-r--r--   0        0        0      937 2024-03-07 12:05:14.131045 django_mapengine-1.4.1/django_mapengine/templates/django_mapengine/map_js.html
--rw-r--r--   0        0        0      419 2024-03-07 12:05:14.131045 django_mapengine-1.4.1/django_mapengine/templates/django_mapengine/map_json.html
--rw-r--r--   0        0        0     1968 2024-03-14 11:59:59.039708 django_mapengine-1.4.1/django_mapengine/urls.py
--rw-r--r--   0        0        0     1264 2023-06-14 12:49:56.422190 django_mapengine-1.4.1/django_mapengine/utils.py
--rw-r--r--   0        0        0     2549 2024-03-26 11:51:33.500776 django_mapengine-1.4.1/django_mapengine/views.py
--rw-r--r--   0        0        0     1767 2024-04-08 11:21:46.580386 django_mapengine-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     4254 1970-01-01 00:00:00.000000 django_mapengine-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-03-12 15:15:44.559160 django_mapengine-1.5.0/LICENSE
+-rw-r--r--   0        0        0     3373 2024-03-26 11:51:33.500776 django_mapengine-1.5.0/README.md
+-rw-r--r--   0        0        0       60 2024-04-24 10:17:38.710736 django_mapengine-1.5.0/django_mapengine/__init__.py
+-rw-r--r--   0        0        0     3312 2024-04-24 10:17:38.710736 django_mapengine-1.5.0/django_mapengine/apps.py
+-rw-r--r--   0        0        0     6738 2024-03-12 15:15:44.559160 django_mapengine-1.5.0/django_mapengine/choropleth.py
+-rw-r--r--   0        0        0    43608 2024-03-12 15:15:44.559160 django_mapengine-1.5.0/django_mapengine/colorbrewer.py
+-rw-r--r--   0        0        0     2230 2024-03-26 11:51:33.500776 django_mapengine-1.5.0/django_mapengine/distill.py
+-rw-r--r--   0        0        0    10173 2024-04-24 10:17:38.710736 django_mapengine-1.5.0/django_mapengine/layers.py
+-rw-r--r--   0        0        0      928 2024-03-14 11:59:59.035708 django_mapengine-1.5.0/django_mapengine/legend.py
+-rw-r--r--   0        0        0     2516 2024-03-14 11:59:59.039708 django_mapengine-1.5.0/django_mapengine/mvt.py
+-rw-r--r--   0        0        0     2161 2023-06-14 12:49:56.418190 django_mapengine-1.5.0/django_mapengine/popups.py
+-rw-r--r--   0        0        0     4014 2024-04-24 10:17:38.710736 django_mapengine-1.5.0/django_mapengine/setup.py
+-rw-r--r--   0        0        0     5664 2024-04-24 10:17:38.710736 django_mapengine-1.5.0/django_mapengine/sources.py
+-rw-r--r--   0        0        0    14131 2024-04-24 10:17:38.710736 django_mapengine-1.5.0/django_mapengine/static/django_mapengine/images/layer_ctrl_default.svg
+-rw-r--r--   0        0        0    10121 2024-04-24 10:17:38.710736 django_mapengine-1.5.0/django_mapengine/static/django_mapengine/images/layer_ctrl_satellite.svg
+-rw-r--r--   0        0        0     1262 2024-04-24 10:17:38.710736 django_mapengine-1.5.0/django_mapengine/static/django_mapengine/js/basemaps.js
+-rw-r--r--   0        0        0     3220 2024-02-02 13:11:04.816042 django_mapengine-1.5.0/django_mapengine/static/django_mapengine/js/choropleth.js
+-rw-r--r--   0        0        0      455 2024-03-12 15:15:44.559160 django_mapengine-1.5.0/django_mapengine/static/django_mapengine/js/events.js
+-rw-r--r--   0        0        0      605 2023-06-14 12:49:56.422190 django_mapengine-1.5.0/django_mapengine/static/django_mapengine/js/helper.js
+-rw-r--r--   0        0        0     1128 2023-08-23 11:10:37.048313 django_mapengine-1.5.0/django_mapengine/static/django_mapengine/js/init.js
+-rw-r--r--   0        0        0     3577 2024-04-24 10:17:38.710736 django_mapengine-1.5.0/django_mapengine/static/django_mapengine/js/layer.js
+-rw-r--r--   0        0        0     3069 2023-07-13 09:07:49.785869 django_mapengine-1.5.0/django_mapengine/static/django_mapengine/js/legend.js
+-rw-r--r--   0        0        0     1782 2024-04-24 10:17:38.710736 django_mapengine-1.5.0/django_mapengine/static/django_mapengine/js/map.js
+-rw-r--r--   0        0        0     2804 2024-03-12 15:15:49.899159 django_mapengine-1.5.0/django_mapengine/static/django_mapengine/js/popup.js
+-rw-r--r--   0        0        0     2558 2023-06-14 12:49:56.422190 django_mapengine-1.5.0/django_mapengine/static/django_mapengine/js/regions.js
+-rw-r--r--   0        0        0      513 2023-06-14 12:49:56.422190 django_mapengine-1.5.0/django_mapengine/static/django_mapengine/js/store.js
+-rw-r--r--   0        0        0      318 2024-04-24 10:17:38.710736 django_mapengine-1.5.0/django_mapengine/templates/django_mapengine/map.html
+-rw-r--r--   0        0        0     1227 2024-04-24 10:17:38.710736 django_mapengine-1.5.0/django_mapengine/templates/django_mapengine/map_basemaps.html
+-rw-r--r--   0        0        0      937 2024-03-07 12:05:14.131045 django_mapengine-1.5.0/django_mapengine/templates/django_mapengine/map_js.html
+-rw-r--r--   0        0        0      489 2024-04-24 10:17:38.710736 django_mapengine-1.5.0/django_mapengine/templates/django_mapengine/map_json.html
+-rw-r--r--   0        0        0     1968 2024-03-14 11:59:59.039708 django_mapengine-1.5.0/django_mapengine/urls.py
+-rw-r--r--   0        0        0     1264 2023-06-14 12:49:56.422190 django_mapengine-1.5.0/django_mapengine/utils.py
+-rw-r--r--   0        0        0     2692 2024-04-24 10:17:38.710736 django_mapengine-1.5.0/django_mapengine/views.py
+-rw-r--r--   0        0        0     1767 2024-04-24 10:17:38.710736 django_mapengine-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4254 1970-01-01 00:00:00.000000 django_mapengine-1.5.0/PKG-INFO
```

### Comparing `django_mapengine-1.4.1/LICENSE` & `django_mapengine-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.4.1/README.md` & `django_mapengine-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.4.1/django_mapengine/apps.py` & `django_mapengine-1.5.0/django_mapengine/apps.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pathlib
 from typing import Dict, List, Tuple
 
 import environ
 from appconf import AppConf
 from django.conf import settings
 
-from . import choropleth
+from . import choropleth, setup
 
 env = environ.Env()
 
 
 class MapEngineConf(AppConf):
     """Config for django-mapengine app"""
 
@@ -62,14 +62,23 @@
     if MAX_BOUNDS:
         SETUP["maxBounds"] = MAX_BOUNDS
 
     LAYER_SWITCH_CLASS = "layer__switch"
 
     # MVTS and CLUSTERS
 
+    BASEMAPS = [
+        setup.MaptilerBasemap(
+            "satellite",
+            source_id="satellite",
+            type="raster",
+            image="django_mapengine/images/layer_ctrl_satellite.svg",
+            description="Satellite basemap view",
+        )
+    ]
     API_MVTS = {}
     API_CLUSTERS = []
 
     # LAYERS
     LAYERS_AT_STARTUP: List[str] = []
 
     # IMAGES
```

### Comparing `django_mapengine-1.4.1/django_mapengine/choropleth.py` & `django_mapengine-1.5.0/django_mapengine/choropleth.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.4.1/django_mapengine/colorbrewer.py` & `django_mapengine-1.5.0/django_mapengine/colorbrewer.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.4.1/django_mapengine/distill.py` & `django_mapengine-1.5.0/django_mapengine/distill.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.4.1/django_mapengine/layers.py` & `django_mapengine-1.5.0/django_mapengine/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,35 @@
 if TYPE_CHECKING:
     from collections.abc import Iterable
 
     from django_mapengine import setup
 
 
 @dataclass
+class BasemapLayer:
+    """Default map layer used in maplibre."""
+
+    # pylint:disable=C0103
+    id: str  # noqa: A003
+    source: str
+    type: str  # noqa: A003
+
+    def get_layer(self):
+        """
+        Build dict from layer settings and style.
+
+        Returns
+        -------
+        dict
+            to be used as layer in maplibre.
+        """
+        return {"id": self.id, "source": self.source, "type": self.type}
+
+
+@dataclass
 class MapLayer:
     """Default map layer used in maplibre."""
 
     # pylint:disable=C0103
     id: str  # noqa: A003
     source: str
     style: dict
@@ -159,14 +180,20 @@
         yield MapLayer(
             id=f"{self.id}_cluster_count",
             source=self.source,
             style=get_layer_style(f"{self.id}_cluster_count"),
         )
 
 
+def get_basemap_layers() -> Iterable[BasemapLayer]:
+    """Return basemap layers"""
+    for basemap in settings.MAP_ENGINE_BASEMAPS:
+        yield BasemapLayer(id=basemap.layer_id, source=basemap.layer_id, type=basemap.type)
+
+
 def get_region_layers() -> Iterable[MapLayer]:
     """
     Return map layers for region-based models.
 
     Returns three layers:
     - one for drawing region outline,
     - one for drawing region area and
```

### Comparing `django_mapengine-1.4.1/django_mapengine/legend.py` & `django_mapengine-1.5.0/django_mapengine/legend.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.4.1/django_mapengine/mvt.py` & `django_mapengine-1.5.0/django_mapengine/mvt.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.4.1/django_mapengine/popups.py` & `django_mapengine-1.5.0/django_mapengine/popups.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.4.1/django_mapengine/setup.py` & `django_mapengine-1.5.0/django_mapengine/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,43 @@
 if TYPE_CHECKING:
     from django.db.models import Manager, Model
 
 Zoom = namedtuple("MinMax", ("min", "max"))
 
 
 @dataclass
+class MaptilerBasemap:
+    """
+    Base class for a basemap
+
+    This is used to:
+    - prepare basemap layers
+    - prepare basemap sources
+    """
+
+    layer_id: str
+    source_id: str
+    description: str
+    image: str
+    type: str = "vector"  # noqa: A003
+    format: str = "jpg"
+
+    def as_dict(self):
+        """Return maptilerBasemap as dict"""
+        return {
+            "layer_id": self.layer_id,
+            "source_id": self.source_id,
+            "description": self.description,
+            "image": self.image,
+            "type": self.type,
+            "format": self.format,
+        }
+
+
+@dataclass
 class ModelAPI:
     """
     Base class for API interface
 
     This is used to:
     - set up API point via URL
     - prepare map layers
@@ -41,14 +70,15 @@
         return apps.get_model(self.app_name, self.model_name)
 
 
 # pylint:disable=R0903
 @dataclass
 class ClusterAPI(ModelAPI):
     """Exists only to distinguish between "normal" and clustered API"""
+
     properties: list = field(default_factory=lambda: [])
 
 
 @dataclass
 class MVTAPI(ModelAPI):
     """API for MVT-based models, which are accessed via model manager"""
```

### Comparing `django_mapengine-1.4.1/django_mapengine/sources.py` & `django_mapengine-1.5.0/django_mapengine/sources.py`

 * *Files 4% similar despite different names*

```diff
@@ -150,40 +150,41 @@
     """
     for cluster in settings.MAP_ENGINE_API_CLUSTERS:
         yield ClusterMapSource(
             cluster.layer_id, type="geojson", url=urls.reverse_lazy(f"django_mapengine:{cluster.layer_id}_cluster")
         )
 
 
-def get_satellite_source() -> MapSource:
+def get_satellite_sources() -> Iterable[MapSource]:
     """
     Return source for satellite basemap
 
     Returns
     -------
     MapSource
         of satellite raster
     """
-    return MapSource(
-        "satellite",
-        type="raster",
-        tiles=[
-            "https://api.maptiler.com/tiles/satellite-v2/"
-            f"{{z}}/{{x}}/{{y}}.jpg?key={settings.MAP_ENGINE_TILING_SERVICE_TOKEN}",
-        ],
-    )
+    for basemap in settings.MAP_ENGINE_BASEMAPS:
+        yield MapSource(
+            basemap.layer_id,
+            type=basemap.type,
+            tiles=[
+                f"https://api.maptiler.com/maps/{basemap.source_id}/"
+                f"{{z}}/{{x}}/{{y}}.{basemap.format}?key={settings.MAP_ENGINE_TILING_SERVICE_TOKEN}",
+            ],
+        )
 
 
 def get_all_sources() -> List[MapSource]:
     """
     Return all map sources for regions, satellite, statics and clusters
 
     Returns
     -------
     List[MapSource]
         all map sources
     """
     sources = list(get_region_sources())
-    sources.append(get_satellite_source())
+    sources.extend(get_satellite_sources())
     sources.extend(get_static_sources())
     sources.extend(get_cluster_sources())
     return sources
```

### Comparing `django_mapengine-1.4.1/django_mapengine/static/django_mapengine/js/basemaps.js` & `django_mapengine-1.5.0/django_mapengine/static/django_mapengine/js/basemaps.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,38 +1,41 @@
-const basemaps = ["satellite"];
+const toggleBasemapButton = document.getElementById("basemaps-control");
+toggleBasemapButton.onclick = toggleBasemapControl;
+
+const basemapButtons = document.getElementById("basemaps").querySelectorAll("button");
+const basemaps = Array.from(basemapButtons).map(function(basemapButton) {
+    return basemapButton.id.slice("basemaps__".length);
+});
+
+for (const basemapButton of basemapButtons) {
+    let basemap_layer = basemapButton.id.slice("basemaps__".length);
+    basemapButton.addEventListener("click", () => {
+        toggleBasemap(basemap_layer);
+    });
+}
 
 function toggleBasemap(basemap) {
     map_store.cold.basemap = basemap;
 
-    if (basemap === null) {
-        map_store.cold.basemapFocusElement = "basemaps__default";
-    } else {
-        map_store.cold.basemapFocusElement = `basemaps__${basemap}`;
-    }
-
     const legend = document.getElementById("legend");
     for (const bm of basemaps) {
-        map.setLayoutProperty(bm, "visibility", "none");
+        if (bm !== "default") {
+            map.setLayoutProperty(bm, "visibility", "none");
+        }
     }
-    if (basemap !== null) {
+    if (basemap !== "default") {
         map.setLayoutProperty(basemap, "visibility", "visible");
     } else {
         legend.hidden = true;
-
     }
 }
 
-// Toggle basemaps control
-let toggleBasemapButton = document.getElementById("basemaps-control");
-
 function toggleBasemapControl() {
     const basemapControl = document.getElementById("basemaps");
 
     if (basemapControl.style.display !== "none") {
         basemapControl.style.display = "none";
     } else {
         basemapControl.style.display = "flex";
-        document.getElementById(map_store.cold.basemapFocusElement).focus();
+        document.getElementById(`basemaps__${map_store.cold.basemap}`).focus();
     }
-}
-
-toggleBasemapButton.onclick = toggleBasemapControl;
+}
```

### Comparing `django_mapengine-1.4.1/django_mapengine/static/django_mapengine/js/choropleth.js` & `django_mapengine-1.5.0/django_mapengine/static/django_mapengine/js/choropleth.js`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.4.1/django_mapengine/static/django_mapengine/js/helper.js` & `django_mapengine-1.5.0/django_mapengine/static/django_mapengine/js/helper.js`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.4.1/django_mapengine/static/django_mapengine/js/init.js` & `django_mapengine-1.5.0/django_mapengine/static/django_mapengine/js/init.js`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.4.1/django_mapengine/static/django_mapengine/js/legend.js` & `django_mapengine-1.5.0/django_mapengine/static/django_mapengine/js/legend.js`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.4.1/django_mapengine/static/django_mapengine/js/map.js` & `django_mapengine-1.5.0/django_mapengine/static/django_mapengine/js/map.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -1,37 +1,15 @@
 map.on("load", async function() {
     PubSub.publish(mapEvent.MAP_LOADED);
 });
 
 PubSub.subscribe(mapEvent.MAP_LOADED, add_sources);
-PubSub.subscribe(mapEvent.MAP_LOADED, add_satellite);
 PubSub.subscribe(mapEvent.MAP_LOADED, add_images);
 
 
-function add_satellite(msg) {
-    const layers = map.getStyle().layers;
-    // Find the index of the first symbol layer in the map style
-    let firstSymbolId;
-    for (let i = 0; i < layers.length; i++) {
-        if (layers[i].type === "symbol") {
-            firstSymbolId = layers[i].id;
-            break;
-        }
-    }
-    map.addLayer({
-            id: "satellite",
-            type: "raster",
-            source: "satellite"
-        },
-        firstSymbolId
-    );
-    map.setLayoutProperty("satellite", "visibility", "none");
-    return logMessage(msg);
-}
-
 function add_sources(msg) {
     const sources = JSON.parse(document.getElementById("mapengine_sources").textContent);
     for (const source in sources) {
         map.addSource(source, sources[source]);
     }
     PubSub.publish(mapEvent.MAP_SOURCES_LOADED);
     return logMessage(msg);
```

### Comparing `django_mapengine-1.4.1/django_mapengine/static/django_mapengine/js/popup.js` & `django_mapengine-1.5.0/django_mapengine/static/django_mapengine/js/popup.js`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.4.1/django_mapengine/static/django_mapengine/js/regions.js` & `django_mapengine-1.5.0/django_mapengine/static/django_mapengine/js/regions.js`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.4.1/django_mapengine/static/django_mapengine/js/store.js` & `django_mapengine-1.5.0/django_mapengine/static/django_mapengine/js/store.js`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.4.1/django_mapengine/templates/django_mapengine/map_basemaps.html` & `django_mapengine-1.5.0/django_mapengine/templates/django_mapengine/map_basemaps.html`

 * *Files 20% similar despite different names*

```diff
@@ -5,19 +5,21 @@
       <path d="m16.933 0-5.8208 3.175-5.2917-3.1497-5.8208 3.1497v13.758l5.8208-3.175 5.2917 3.175 5.8208-3.175v-13.758zm-11.642 1.617v11.112l-4.2333 2.3518v-11.112l4.2333-2.3518zm1.0583 0.023254 4.2333 2.5404v11.112l-4.2333-2.5404v-11.112zm9.525 0.47646v11.113l-4.2333 2.1167v-11.112l4.2333-2.1167z"/>
     </svg>
     <div class="layers-text">{% trans "maps"|title %}</div>
   </div>
 </button>
 <div id="basemaps" class="basemaps" style="display:none">
   <div class="basemaps__btn">
-    <button id="basemaps__default" class="btn" onclick="toggleBasemap(null);">
-      <img src="{% static 'images/layer_ctrl_default.svg' %}" alt="Default basemap view">
+    <button id="basemaps__default" class="btn">
+      <img src="{% static 'django_mapengine/images/layer_ctrl_default.svg' %}" alt="Default basemap view">
       <span>{% trans "default"|title %}</span>
     </button>
   </div>
-  <div class="basemaps__btn">
-    <button id="basemaps__satellite" class="btn" onclick="toggleBasemap('satellite');">
-      <img src="{% static 'images/layer_ctrl_satellite.svg' %}" alt="Satellite basemap view">
-      <span>{% trans "satellite"|title %}</span>
-    </button>
-  </div>
+  {% for basemap in mapengine_basemap_layers %}
+    <div class="basemaps__btn">
+      <button id="basemaps__{{ basemap.layer_id }}" class="btn">
+        <img src="{% static basemap.image %}" alt="{{ basemap.description }}">
+        <span>{% trans basemap.layer_id|title %}</span>
+      </button>
+    </div>
+  {% endfor %}
 </div>
```

### Comparing `django_mapengine-1.4.1/django_mapengine/templates/django_mapengine/map_js.html` & `django_mapengine-1.5.0/django_mapengine/templates/django_mapengine/map_js.html`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.4.1/django_mapengine/urls.py` & `django_mapengine-1.5.0/django_mapengine/urls.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.4.1/django_mapengine/utils.py` & `django_mapengine-1.5.0/django_mapengine/utils.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.4.1/django_mapengine/views.py` & `django_mapengine-1.5.0/django_mapengine/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,26 +42,28 @@
             **{
                 "mapengine_setup": settings.MAP_ENGINE_SETUP,
                 "mapengine_zoom_levels": settings.MAP_ENGINE_ZOOM_LEVELS,
                 # Sources need valid URL (containing host and port), thus they have to be defined using request:
                 "mapengine_sources": {
                     source.name: source.get_source(self.request) for source in sources.get_all_sources()
                 },
+                "mapengine_basemap_layers": [basemap.as_dict() for basemap in settings.MAP_ENGINE_BASEMAPS],
                 "mapengine_layers": [layer.get_layer() for layer in layers.get_all_layers()],
                 "mapengine_layers_at_startup": settings.MAP_ENGINE_LAYERS_AT_STARTUP + settings.MAP_ENGINE_REGIONS,
                 "mapengine_images": [image.as_dict() for image in settings.MAP_ENGINE_IMAGES],
             }
         )
         store = {
             "debugMode": settings.MAP_ENGINE_DEBUG,
             "popups": {popup.layer_id: popup.as_dict() for popup in settings.MAP_ENGINE_POPUPS},
             "regions": settings.MAP_ENGINE_REGIONS,
             "result_views": {},  # Placeholder for already downloaded results (used in results.js)
             "zoom_levels": settings.MAP_ENGINE_ZOOM_LEVELS,
             "cluster_layers": [cluster.layer_id for cluster in settings.MAP_ENGINE_API_CLUSTERS],
             "choropleths": {choropleth.name: choropleth.as_dict() for choropleth in settings.MAP_ENGINE_CHOROPLETHS},
             "layer_switch_class": settings.MAP_ENGINE_LAYER_SWITCH_CLASS,
+            "basemap": "default",
         }
 
         context["mapengine_store_cold_init"] = store
 
         return context
```

### Comparing `django_mapengine-1.4.1/pyproject.toml` & `django_mapengine-1.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-mapengine"
-version = "1.4.1"
+version = "1.5.0"
 description = "Map engine for maplibre in django"
 authors = ["Hendrik Huyskens <hendrik.huyskens@rl-institut.de>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `django_mapengine-1.4.1/PKG-INFO` & `django_mapengine-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mapengine
-Version: 1.4.1
+Version: 1.5.0
 Summary: Map engine for maplibre in django
 Author: Hendrik Huyskens
 Author-email: hendrik.huyskens@rl-institut.de
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-mapengine Version: 1.4.1 Summary: Map engine
+Metadata-Version: 2.1 Name: django-mapengine Version: 1.5.0 Summary: Map engine
 for maplibre in django Author: Hendrik Huyskens Author-email:
 hendrik.huyskens@rl-institut.de Requires-Python: >=3.9,<3.12 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Dist: django-appconf (>=1.0.5,<2.0.0) Requires-Dist: django-distill
```

