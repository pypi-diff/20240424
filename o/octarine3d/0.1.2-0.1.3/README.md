# Comparing `tmp/octarine3d-0.1.2.tar.gz` & `tmp/octarine3d-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octarine3d-0.1.2.tar", last modified: Tue Apr 16 14:00:37 2024, max compression
+gzip compressed data, was "octarine3d-0.1.3.tar", last modified: Wed Apr 24 10:07:23 2024, max compression
```

## Comparing `octarine3d-0.1.2.tar` & `octarine3d-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:00:37.594943 octarine3d-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-16 14:00:32.000000 octarine3d-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-16 14:00:37.594943 octarine3d-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-16 14:00:32.000000 octarine3d-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:00:37.590943 octarine3d-0.1.2/octarine/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-16 14:00:32.000000 octarine3d-0.1.2/octarine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-16 14:00:32.000000 octarine3d-0.1.2/octarine/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-16 14:00:32.000000 octarine3d-0.1.2/octarine/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14390 2024-04-16 14:00:32.000000 octarine3d-0.1.2/octarine/controls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-16 14:00:32.000000 octarine3d-0.1.2/octarine/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    10054 2024-04-16 14:00:32.000000 octarine3d-0.1.2/octarine/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-04-16 14:00:32.000000 octarine3d-0.1.2/octarine/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    41162 2024-04-16 14:00:32.000000 octarine3d-0.1.2/octarine/viewer.py
--rw-r--r--   0 runner    (1001) docker     (127)    20173 2024-04-16 14:00:32.000000 octarine3d-0.1.2/octarine/visuals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:00:37.590943 octarine3d-0.1.2/octarine3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-16 14:00:37.000000 octarine3d-0.1.2/octarine3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-16 14:00:37.000000 octarine3d-0.1.2/octarine3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:00:37.000000 octarine3d-0.1.2/octarine3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:00:37.000000 octarine3d-0.1.2/octarine3d.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-16 14:00:37.000000 octarine3d-0.1.2/octarine3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 14:00:37.000000 octarine3d-0.1.2/octarine3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-16 14:00:32.000000 octarine3d-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 14:00:37.594943 octarine3d-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-16 14:00:32.000000 octarine3d-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:07:23.577922 octarine3d-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-24 10:07:18.000000 octarine3d-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-04-24 10:07:23.577922 octarine3d-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-24 10:07:18.000000 octarine3d-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:07:23.573922 octarine3d-0.1.3/octarine/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-24 10:07:18.000000 octarine3d-0.1.3/octarine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 10:07:18.000000 octarine3d-0.1.3/octarine/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-24 10:07:18.000000 octarine3d-0.1.3/octarine/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14390 2024-04-24 10:07:18.000000 octarine3d-0.1.3/octarine/controls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-24 10:07:18.000000 octarine3d-0.1.3/octarine/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10054 2024-04-24 10:07:18.000000 octarine3d-0.1.3/octarine/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-24 10:07:18.000000 octarine3d-0.1.3/octarine/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-24 10:07:18.000000 octarine3d-0.1.3/octarine/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41852 2024-04-24 10:07:18.000000 octarine3d-0.1.3/octarine/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20188 2024-04-24 10:07:18.000000 octarine3d-0.1.3/octarine/visuals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:07:23.577922 octarine3d-0.1.3/octarine3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-04-24 10:07:23.000000 octarine3d-0.1.3/octarine3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-24 10:07:23.000000 octarine3d-0.1.3/octarine3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:07:23.000000 octarine3d-0.1.3/octarine3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:07:23.000000 octarine3d-0.1.3/octarine3d.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-24 10:07:23.000000 octarine3d-0.1.3/octarine3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 10:07:23.000000 octarine3d-0.1.3/octarine3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 10:07:18.000000 octarine3d-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 10:07:23.577922 octarine3d-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-24 10:07:18.000000 octarine3d-0.1.3/setup.py
```

### Comparing `octarine3d-0.1.2/LICENSE` & `octarine3d-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `octarine3d-0.1.2/PKG-INFO` & `octarine3d-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octarine3d
-Version: 0.1.2
+Version: 0.1.3
 Summary: WGPU-based 3d viewer
 Home-page: https://github.com/schlegelp/octarine
 Author: Philipp Schlegel
 Author-email: pms70@cam.ac.uk
 License: BSD-2-Clause
 Project-URL: Documentation, https://schlegelp.github.io/octarine/
 Project-URL: Source, https://github.com/schlegelp/octarine
@@ -19,15 +19,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pygfx>=0.2.0
 Requires-Dist: numpy
-Requires-Dist: pandas
 Requires-Dist: pypng
 Requires-Dist: six
 Requires-Dist: cmap
 Provides-Extra: all
 Requires-Dist: jupyter_rfb; extra == "all"
 Requires-Dist: PySide6; extra == "all"
 Requires-Dist: ipywidgets; extra == "all"
@@ -36,14 +35,15 @@
 Requires-Dist: mkdocs; extra == "docs"
 Requires-Dist: mkdocs-material[imaging]; extra == "docs"
 Requires-Dist: mkdocstrings-python; extra == "docs"
 Requires-Dist: mkdocs-minify-plugin; extra == "docs"
 Requires-Dist: mkdocs-literate-nav; extra == "docs"
 Requires-Dist: mkdocs-gen-files; extra == "docs"
 Requires-Dist: mkdocs-glightbox; extra == "docs"
+Requires-Dist: mkdocs-section-index; extra == "docs"
 
 ![octarine banner](https://schlegelp.github.io/octarine/_static/octarine_logo_banner.png)
 <p align="center">
 <i>
 Octarine is the eighth color of the Discworld's spectrum, which is described as the color of magic itself. Only wizards and cats can see it.
 </i>
 </p>
```

### Comparing `octarine3d-0.1.2/README.md` & `octarine3d-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `octarine3d-0.1.2/octarine/config.py` & `octarine3d-0.1.3/octarine/config.py`

 * *Files identical despite different names*

### Comparing `octarine3d-0.1.2/octarine/controls.py` & `octarine3d-0.1.3/octarine/controls.py`

 * *Files identical despite different names*

### Comparing `octarine3d-0.1.2/octarine/conversion.py` & `octarine3d-0.1.3/octarine/conversion.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,17 +48,18 @@
 
 def register_converter(t, converter, insert='first'):
     """Register a converter for a given data type.
 
     Parameters
     ----------
     t :         type | hashable | callable
-                Data type to register the converter for. If a function
+                Data type the converter is meant to convert. If a function
                 it is expected to take a single argument `x` and return
-                True if `x` can be converted using `converter`.
+                True if `x` can be converted using `converter` and False
+                if not.
     converter : callable
                 Function that converts `x` to pygfx visuals. Must accept
                 at least a single argument and return either a single
                 visual or a list thereof.
     insert :    "first" | "last"
                 Whether to insert the converter at the beginning or end
                 of the list of converters. This is important because when
```

### Comparing `octarine3d-0.1.2/octarine/jupyter.py` & `octarine3d-0.1.3/octarine/jupyter.py`

 * *Files identical despite different names*

### Comparing `octarine3d-0.1.2/octarine/utils.py` & `octarine3d-0.1.3/octarine/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import six
 
 import pygfx as gfx
 import numpy as np
-import pandas as pd
 
 from collections.abc import Iterable
 
 from . import config
 
 # Set up logging
 logger = config.get_logger(__name__)
@@ -42,47 +41,52 @@
     if include_geometries:
         visuals += [ob for ob in x if 'pygfx.geometries' in str(type(ob))]
 
     # Collect scatter points
     scatter = [ob for ob in x if isinstance(ob, np.ndarray) and (ob.ndim == 2) and (ob.shape[1] == 3)]
 
     # Collect dataframes with X/Y/Z coordinates
-    dataframes = [ob for ob in x if isinstance(ob, pd.DataFrame)]
+    dataframes = [ob for ob in x if _is_pandas_dataframe(ob)]
     if [d for d in dataframes if False in np.isin(['x', 'y', 'z'], d.columns)]:
         logger.warning('DataFrames must have x, y and z columns.')
     dataframes = [d for d in dataframes if all(np.isin(['x', 'y', 'z'], d.columns))]
     scatter += [d[['x', 'y', 'z']].values for d in dataframes]
 
     # Collect volumes
     volumes = [ob for ob in x if isinstance(ob, np.ndarray) and (ob.ndim == 3)]
 
     # Collect meshes
     meshes = [ob for ob in x if is_mesh_like(ob)]
 
-    # Collect dataframes with X/Y/Z coordinates
-    dataframes = [ob for ob in x if isinstance(ob, pd.DataFrame)]
-    if [d for d in dataframes if False in np.isin(['x', 'y', 'z'], d.columns)]:
-        logger.warning('DataFrames must have x, y and z columns.')
-    # Filter to and extract x/y/z coordinates
-    dataframes = [d for d in dataframes if False not in [c in d.columns for c in ['x', 'y', 'z']]]
-    dataframes = [d[['x', 'y', 'z']].values for d in dataframes]
-
     # Collect arrays
     arrays = [ob.copy() for ob in x if isinstance(ob, np.ndarray)]
     # Remove arrays with wrong dimensions
     if [ob for ob in arrays if ob.shape[1] != 3 and ob.shape[0] != 2]:
         logger.warning('Arrays need to be of shape (N, 3) for scatter or (2, N)'
                        ' for line plots.')
     arrays = [ob for ob in arrays if any(np.isin(ob.shape, [2, 3]))]
 
     points = dataframes + arrays
 
     return meshes, volumes, points, visuals
 
 
+def _is_pandas_dataframe(x):
+    """Check if object is a pandas DataFrame."""
+    # We're doing this without the use of isinstance() to avoid
+    # needing pandas as a dependency
+    if not hasattr(x, "__class__"):
+        return False
+    # Check if any of the parent classes is a pandas DataFrame
+    for b in x.__class__.__mro__:
+        if b.__module__.startswith("pandas") and b.__name__ == "DataFrame":
+            return True
+    return False
+
+
 def make_iterable(x, force_type = None):
     """Force input into a numpy array.
 
     For dicts, keys will be turned into array.
 
     Examples
     --------
@@ -114,15 +118,15 @@
     True
     >>> oc.utils.is_iterable('a')
     False
     >>> oc.utils.is_iterable({'a': 1})
     True
 
     """
-    if isinstance(x, Iterable) and not isinstance(x, (six.string_types, pd.DataFrame)):
+    if isinstance(x, Iterable) and not isinstance(x, six.string_types) and not _is_pandas_dataframe(x):
         return True
     else:
         return False
 
 
 def is_hashable(x) -> bool:
     """Check if object is hashable."""
```

### Comparing `octarine3d-0.1.2/octarine/viewer.py` & `octarine3d-0.1.3/octarine/viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,19 @@
     title :     str, optional
                 Title of the viewer window.
     max_fps :   int, optional
                 Maximum frames per second to render.
     size :      tuple, optional
                 Size of the viewer window.
     camera :    "ortho" | "perspective", optional
+                Type of camera to use. Defaults to "ortho". Note you can always
+                change the camera type by adjust the `Viewer.camera.fov` attribute
+                (0 = ortho, >0 = perspective).
+    control :   "trackball" | "panzoom" | "fly" | "orbit"
+                Controller type to use. Defaults to "trackball".
     show :      bool, optional
                 Whether to immediately show the viewer. Note that this has no
                 effect in Jupyter. There you will have to call ``.show()`` manually
                 on the last line of a cell for the viewer to appear.
     **kwargs
                 Keyword arguments are passed through to ``WgpuCanvas``.
 
@@ -85,14 +90,15 @@
 
     def __init__(
         self,
         offscreen=False,
         title="Octarine Viewer",
         max_fps=30,
         camera="ortho",
+        control="trackball",
         size=None,
         show=True,
         **kwargs,
     ):
         # Check if we're running in an IPython environment
         if utils._type_of_script() == "ipython":
             ip = get_ipython()  # noqa: F821
@@ -150,17 +156,24 @@
             self.camera = gfx.OrthographicCamera()
         elif camera == "perspective":
             self.camera = gfx.PerspectiveCamera()
         else:
             raise ValueError(f"Unknown camera type: {camera}")
 
         # Add controller
-        self.controller = gfx.TrackballController(
-            self.camera, register_events=self.renderer
-        )
+        controller = {
+            "trackball": gfx.TrackballController,
+            "panzoom": gfx.PanZoomController,
+            "fly": gfx.FlyController,
+            "orbit": gfx.OrbitController,
+        }.get(control, None)
+        if controller is None:
+            raise ValueError(f"Unknown controller type: {control}")
+
+        self.controller = controller(self.camera, register_events=self.renderer)
 
         # Stats
         self.stats = gfx.Stats(self.renderer)
         self._show_fps = False
 
         # Setup key events
         self.key_events = {}
@@ -781,15 +794,17 @@
         if color is None:
             color = self._next_color()
         if name is None:
             name = self._next_label("Scatter")
         elif not isinstance(name, str):
             name = str(name)
 
-        visual = points2gfx(points, color=color, size=size, size_space=size_space, marker=marker)
+        visual = points2gfx(
+            points, color=color, size=size, size_space=size_space, marker=marker
+        )
         visual._object_id = name if name else uuid.uuid4()
 
         self._add_to_scene(visual, center)
 
     def add_lines(
         self,
         lines,
@@ -856,31 +871,31 @@
         )
         visual._object_id = name if name else uuid.uuid4()
         self._add_to_scene(visual, center)
 
     def add_volume(
         self,
         volume,
-        dims,
+        spacing=(1, 1, 1),
         name=None,
         color=None,
         offset=(0, 0, 0),
         clim="data",
         interpolation="linear",
         hide_zero=True,
         center=True,
     ):
         """Add image volume to canvas.
 
         Parameters
         ----------
         volume :    (N, M, K) array
                     Volume to plot.
-        dims :      tuple
-                    Scale factors for the volume.
+        spacing :   tuple
+                    Spacing between voxels.
         name :      str, optional
                     Name for the visual.
         color :     color | list of colors | pygfx.Texture, optional
                     Colormap to render the volume. This can be:
                       - name of a colormap (e.g. "viridis" or "magma")
                       - a single color (name, hex, rgb, rgba)
                       - a list of colors
@@ -916,15 +931,15 @@
         if name is None:
             name = self._next_label("Volume")
         elif not isinstance(name, str):
             name = str(name)
 
         visual = volume2gfx(
             volume,
-            dims=dims,
+            spacing=spacing,
             offset=offset,
             color=color,
             clim=clim,
             interpolation=interpolation,
             hide_zero=hide_zero,
         )
         visual._object_id = name if name else uuid.uuid4()
```

### Comparing `octarine3d-0.1.2/octarine/visuals.py` & `octarine3d-0.1.3/octarine/visuals.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,29 +103,29 @@
 
     # Convert to vispy cmap
     return gfx.Texture(colormap_data, dim=1)
 
 
 def volume2gfx(
     vol,
-    dims,
     color,
+    spacing=(1, 1, 1),
     offset=(0, 0, 0),
     clim="auto",
     interpolation="linear",
     hide_zero=True,
 ):
     """Convert volume (i.e. 3d arrays) to pygfx visual.
 
     Parameters
     ----------
     vol :           np.ndarray
                     3D array representing the volume.
-    dims :          tuple
-                    Dimensions of the volume along the (x, y, z) axes.
+    spacing :       tuple
+                    Spacing between voxels in the volume.
     color :         color | list of colors | pygfx.Texture, optional
                     Colormap to render the volume. This can be:
                       - name of a colormap (e.g. "viridis" or "magma")
                       - a single color (name, hex, rgb, rgba)
                       - a list of colors
                       - a 1D pygfx.Texture
                     Note that single colors typically don't look good and
@@ -155,18 +155,18 @@
 
     """
     # TODOs:
     # - add support for other Volume materials (e.g. gfx.VolumeMipMaterial)
 
     assert isinstance(vol, np.ndarray), "Expected 3D numpy array."
     assert vol.ndim == 3, "Expected 3D numpy array."
-    assert isinstance(dims, (tuple, list, np.ndarray, int, float))
-    if isinstance(dims, (int, float)):
-        dims = [dims] * 3
-    assert len(dims) == 3, "Expected dimensions as tuple of length 3."
+    assert isinstance(spacing, (tuple, list, np.ndarray, int, float))
+    if isinstance(spacing, (int, float)):
+        spacing = [spacing] * 3
+    assert len(spacing) == 3, "Expected spacing as tuple of length 3."
 
     # Similar to vispy, pygfx seems to expect zyx coordinate space
     grid = vol.T
 
     # Convert to data type that pygfx can handle:
     # Convert non-native byte order to native; e.g. >u4 -> u4 = uint64
     if grid.dtype.byteorder in (">", "<"):
@@ -222,15 +222,15 @@
     # vis.material.map.update_range((0, 0, 0), vis.material.map.size)
 
     # Set scales and offset
     (
         vis.local.scale_x,
         vis.local.scale_y,
         vis.local.scale_z,
-    ) = dims
+    ) = spacing
     (vis.local.x, vis.local.y, vis.local.z) = offset
 
     # Add custom attributes
     vis._object_type = "volume"
     vis._object_id = uuid.uuid4()
 
     return vis
```

### Comparing `octarine3d-0.1.2/octarine3d.egg-info/PKG-INFO` & `octarine3d-0.1.3/octarine3d.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octarine3d
-Version: 0.1.2
+Version: 0.1.3
 Summary: WGPU-based 3d viewer
 Home-page: https://github.com/schlegelp/octarine
 Author: Philipp Schlegel
 Author-email: pms70@cam.ac.uk
 License: BSD-2-Clause
 Project-URL: Documentation, https://schlegelp.github.io/octarine/
 Project-URL: Source, https://github.com/schlegelp/octarine
@@ -19,15 +19,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pygfx>=0.2.0
 Requires-Dist: numpy
-Requires-Dist: pandas
 Requires-Dist: pypng
 Requires-Dist: six
 Requires-Dist: cmap
 Provides-Extra: all
 Requires-Dist: jupyter_rfb; extra == "all"
 Requires-Dist: PySide6; extra == "all"
 Requires-Dist: ipywidgets; extra == "all"
@@ -36,14 +35,15 @@
 Requires-Dist: mkdocs; extra == "docs"
 Requires-Dist: mkdocs-material[imaging]; extra == "docs"
 Requires-Dist: mkdocstrings-python; extra == "docs"
 Requires-Dist: mkdocs-minify-plugin; extra == "docs"
 Requires-Dist: mkdocs-literate-nav; extra == "docs"
 Requires-Dist: mkdocs-gen-files; extra == "docs"
 Requires-Dist: mkdocs-glightbox; extra == "docs"
+Requires-Dist: mkdocs-section-index; extra == "docs"
 
 ![octarine banner](https://schlegelp.github.io/octarine/_static/octarine_logo_banner.png)
 <p align="center">
 <i>
 Octarine is the eighth color of the Discworld's spectrum, which is described as the color of magic itself. Only wizards and cats can see it.
 </i>
 </p>
```

### Comparing `octarine3d-0.1.2/setup.py` & `octarine3d-0.1.3/setup.py`

 * *Files identical despite different names*

