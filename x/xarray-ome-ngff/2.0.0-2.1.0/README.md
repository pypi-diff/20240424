# Comparing `tmp/xarray_ome_ngff-2.0.0.tar.gz` & `tmp/xarray_ome_ngff-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarray_ome_ngff-2.0.0.tar", max compression
+gzip compressed data, was "xarray_ome_ngff-2.1.0.tar", max compression
```

## Comparing `xarray_ome_ngff-2.0.0.tar` & `xarray_ome_ngff-2.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1511 2023-02-15 20:59:22.209367 xarray_ome_ngff-2.0.0/LICENSE.md
--rw-r--r--   0        0        0     4377 2024-03-31 21:14:43.152054 xarray_ome_ngff-2.0.0/README.md
--rw-r--r--   0        0        0      811 2024-03-31 21:15:35.288610 xarray_ome_ngff-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     5816 2024-03-31 21:14:43.154826 xarray_ome_ngff-2.0.0/src/xarray_ome_ngff/__init__.py
--rw-r--r--   0        0        0     3980 2024-03-31 21:14:43.155056 xarray_ome_ngff-2.0.0/src/xarray_ome_ngff/array_wrap.py
--rw-r--r--   0        0        0      355 2024-03-31 21:14:43.155330 xarray_ome_ngff-2.0.0/src/xarray_ome_ngff/core.py
--rw-r--r--   0        0        0        0 2023-03-22 18:23:46.045591 xarray_ome_ngff-2.0.0/src/xarray_ome_ngff/py.typed
--rw-r--r--   0        0        0        0 2023-03-10 21:37:50.406964 xarray_ome_ngff-2.0.0/src/xarray_ome_ngff/v04/__init__.py
--rw-r--r--   0        0        0    20151 2024-03-31 21:14:43.155694 xarray_ome_ngff-2.0.0/src/xarray_ome_ngff/v04/multiscale.py
--rw-r--r--   0        0        0     5110 1970-01-01 00:00:00.000000 xarray_ome_ngff-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1511 2024-01-01 11:59:38.523694 xarray_ome_ngff-2.1.0/LICENSE.md
+-rw-r--r--   0        0        0     4376 2024-04-03 14:55:35.758166 xarray_ome_ngff-2.1.0/README.md
+-rw-r--r--   0        0        0     1201 2024-04-23 14:33:59.828157 xarray_ome_ngff-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5838 2024-04-23 13:22:32.986586 xarray_ome_ngff-2.1.0/src/xarray_ome_ngff/__init__.py
+-rw-r--r--   0        0        0     4122 2024-04-23 13:44:31.635682 xarray_ome_ngff-2.1.0/src/xarray_ome_ngff/array_wrap.py
+-rw-r--r--   0        0        0      304 2024-04-23 09:58:43.154962 xarray_ome_ngff-2.1.0/src/xarray_ome_ngff/core.py
+-rw-r--r--   0        0        0        0 2024-01-01 11:59:38.527695 xarray_ome_ngff-2.1.0/src/xarray_ome_ngff/py.typed
+-rw-r--r--   0        0        0        0 2024-01-01 11:59:38.527695 xarray_ome_ngff-2.1.0/src/xarray_ome_ngff/v04/__init__.py
+-rw-r--r--   0        0        0    20892 2024-04-23 14:32:41.155614 xarray_ome_ngff-2.1.0/src/xarray_ome_ngff/v04/multiscale.py
+-rw-r--r--   0        0        0     5109 1970-01-01 00:00:00.000000 xarray_ome_ngff-2.1.0/PKG-INFO
```

### Comparing `xarray_ome_ngff-2.0.0/LICENSE.md` & `xarray_ome_ngff-2.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `xarray_ome_ngff-2.0.0/README.md` & `xarray_ome_ngff-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # xarray-ome-ngff
 
 Integrating [Xarray](https://docs.xarray.dev/en/stable/) with [OME-NGFF](https://ngff.openmicroscopy.org/).
 
 ## Help
-
-See [documentation](https://janeliscicomp.github.io/xarray-multiscale) for more details
+See [documentation](https://janeliascicomp.github.io/xarray-ome-ngff/) for more details
 
 ## Usage
 
 ### Read OME-NGFF data
 
 ```python
 import zarr
```

### Comparing `xarray_ome_ngff-2.0.0/src/xarray_ome_ngff/__init__.py` & `xarray_ome_ngff-2.1.0/src/xarray_ome_ngff/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 def create_multiscale_group(
     *,
     store: BaseStore,
     path: str,
     arrays: dict[str, DataArray],
     transform_precision: int | None = None,
     ngff_version: Literal["0.4"] = "0.4",
-):
+) -> MultiscaleGroupV04:
     """
     store: zarr.storage.BaseStore
         The storage backend for the Zarr hierarchy.
     path: str
         The path in the storage backend for the multiscale group.
     arrays: dict[str, DataArray]
         A mapping from strings to `xarray.DataArray`.
```

### Comparing `xarray_ome_ngff-2.0.0/src/xarray_ome_ngff/v04/multiscale.py` & `xarray_ome_ngff-2.1.0/src/xarray_ome_ngff/v04/multiscale.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
-from pydantic_ome_ngff.v04.multiscale import Group
-from typing import TYPE_CHECKING
+from pydantic_ome_ngff.v04.multiscale import Group as MultiscaleGroup
+from typing import TYPE_CHECKING, Literal
 
-from xarray_ome_ngff.array_wrap import ArrayWrapperSpec
-from xarray_ome_ngff.array_wrap import BaseArrayWrapper
+from xarray_ome_ngff.array_wrap import ArrayWrapperSpec, DaskArrayWrapper
 from xarray_ome_ngff.array_wrap import ZarrArrayWrapper
 from xarray_ome_ngff.array_wrap import parse_wrapper
 
 if TYPE_CHECKING:
     from typing import Any, Dict, Sequence
 
 import numpy as np
@@ -18,14 +17,16 @@
     VectorScale,
     VectorTranslation,
 )
 import warnings
 from xarray_ome_ngff.core import CoordinateAttrs, ureg
 import zarr
 from zarr.storage import BaseStore
+from numcodecs.abc import Codec
+from numcodecs import Zstd
 
 import os
 
 
 def multiscale_metadata(
     arrays: dict[str, DataArray],
     name: str | None = None,
@@ -102,15 +103,15 @@
         metadata=metadata,
     )
 
 
 def transforms_from_coords(
     coords: dict[str, DataArray],
     normalize_units: bool = True,
-    infer_axis_type=True,
+    infer_axis_type: bool = True,
     transform_precision: int | None = None,
 ) -> tuple[tuple[Axis, ...], tuple[VectorScale, VectorTranslation]]:
     """
     Generate Axes and CoordinateTransformations from the coordinates of an xarray.DataArray.
 
     Parameters
     ----------
@@ -139,17 +140,17 @@
     -------
     tuple[tuple[Axis, ...], tuple[VectorScale, VectorTranslation]]
         A tuple containing a tuple of `Axis` objects, one per dimension, and
         a tuple with a VectorScaleTransform a VectorTranslationTransform.
         Both transformations are are derived from the coordinates of the input array.
     """
 
-    translate = ()
-    scale = ()
-    axes = ()
+    translate: tuple[float, ...] = ()
+    scale: tuple[float, ...] = ()
+    axes: tuple[Axis, ...] = ()
 
     for dim, coord in coords.items():
         if ndim := len(coord.dims) != 1:
             msg = (
                 "Each coordinate must have one and only one dimension. "
                 f"Got a coordinate with {ndim}."
             )
@@ -171,122 +172,120 @@
         units = coord.attrs.get("units", None)
         if normalize_units and units is not None:
             units = ureg.get_name(units, case_sensitive=True)
         if (type := coord.attrs.get("type", None)) is None and infer_axis_type:
             unit_dimensionality = ureg.get_dimensionality(units)
             if len(unit_dimensionality) > 1:
                 msg = (
-                    f'Failed to infer the type of axis with unit = "{units}"',
+                    f'Failed to infer the type of axis with unit = "{units}"'
                     f'because it appears that unit "{units}" is a compound unit, '
                     'which cannot be mapped to a single axis type. "type" will be '
-                    'set to "None" for this axis.',
-                )
-                warnings.warn(
-                    RuntimeWarning,
+                    'set to "None" for this axis.'
                 )
+                warnings.warn(msg, category=RuntimeWarning)
             if "[length]" in unit_dimensionality:
                 type = "space"
             elif "[time]" in unit_dimensionality:
                 type = "time"
 
         axes += (
             Axis(
                 name=dim,
                 unit=units,
                 type=type,
             ),
         )
     if transform_precision is not None:
-        scale = np.round(scale, transform_precision)
-        translate = np.round(translate, transform_precision)
+        scale = tuple(np.round(scale, transform_precision).tolist())
+        translate = tuple(np.round(translate, transform_precision).tolist())
 
     transforms = (
         VectorScale(scale=scale),
         VectorTranslation(translation=translate),
     )
     return axes, transforms
 
 
 def coords_from_transforms(
+    *,
     axes: Sequence[Axis],
-    transforms: Sequence[tuple[VectorScale] | tuple[VectorScale, VectorTranslation]],
+    transforms: tuple[VectorScale, VectorTranslation],
     shape: tuple[int, ...],
-) -> tuple[DataArray]:
+) -> tuple[DataArray, ...]:
     """
     Given an output shape, convert a sequence of Axis objects and a corresponding
     sequence of coordinateTransform objects into xarray-compatible coordinates.
     """
 
     if len(axes) != len(shape):
         msg = (
             "Length of axes must match length of shape. "
             f"Got {len(axes)} axes but shape has {len(shape)} elements"
         )
         raise ValueError(msg)
 
     result = []
 
+    for tx in transforms:
+        if tx.type == "translation":
+            if len(tx.translation) != len(axes):
+                msg = (
+                    f"Translation parameter has length {len(tx.translation)}. "
+                    f"This does not match the number of axes {len(axes)}."
+                )
+                raise ValueError(msg)
+
+        elif tx.type == "scale":
+            if len(tx.scale) != len(axes):
+                msg = (
+                    f"Scale parameter has length {len(tx.scale)}. "
+                    f"This does not match the number of axes {len(axes)}."
+                )
+                raise ValueError(msg)
+        elif tx.type == "identity":
+            pass
+        else:
+            msg = (
+                f"Transform type {tx.type} not recognized. Must be one of scale, "
+                "translation, or identity"
+            )
+            raise ValueError(msg)
+
     for idx, axis in enumerate(axes):
         base_coord = np.arange(shape[idx], dtype="float")
         name = axis.name
         unit = axis.unit
         # apply transforms in order
         for tx in transforms:
-            if isinstance(getattr(tx, "path", None), str):
-                msg = (
-                    f"Problematic transform: {tx}. This library cannot handle "
-                    "transforms with paths. Resolve this path to a literal scale or "
-                    "translation"
-                )
-                raise ValueError(msg)
-
             if tx.type == "translation":
-                if len(tx.translation) != len(axes):
-                    msg = (
-                        f"Translation parameter has length {len(tx.translation)}. "
-                        f"This does not match the number of axes {len(axes)}."
-                    )
-                    raise ValueError(msg)
                 base_coord += tx.translation[idx]
             elif tx.type == "scale":
-                if len(tx.scale) != len(axes):
-                    msg = (
-                        f"Scale parameter has length {len(tx.scale)}. "
-                        f"This does not match the number of axes {len(axes)}."
-                    )
-                    raise ValueError(msg)
                 base_coord *= tx.scale[idx]
             elif tx.type == "identity":
                 pass
-            else:
-                msg = (
-                    f"Transform type {tx.type} not recognized. Must be one of scale, "
-                    "translation, or identity"
-                )
-                raise ValueError(msg)
 
         result.append(
             DataArray(
                 base_coord,
                 attrs=CoordinateAttrs(units=unit).model_dump(),
                 dims=(name,),
             )
         )
 
     return tuple(result)
 
 
-def fuse_coordinate_transforms(
+def normalize_transforms(
     base_transforms: (
         None | tuple[()] | tuple[VectorScale] | tuple[VectorScale, VectorTranslation]
     ),
     dset_transforms: tuple[VectorScale] | tuple[VectorScale, VectorTranslation],
 ) -> tuple[VectorScale, VectorTranslation]:
 
-    if base_transforms is None or base_transforms == ():
+    if base_transforms is None or len(base_transforms) == 0:
         out_scale = dset_transforms[0]
         if len(dset_transforms) == 1:
             out_trans = VectorTranslation(translation=(0,) * len(out_scale.scale))
         else:
             out_trans = dset_transforms[1]
     else:
         base_scale = base_transforms[0]
@@ -297,27 +296,38 @@
         if len(base_transforms) == 1:
             if len(dset_transforms) == 1:
                 out_trans = VectorTranslation(translation=(0,) * len(base_scale.scale))
             else:
                 out_trans = dset_transforms[1]
         else:
             base_trans = base_transforms[1]
-            dset_trans = dset_transforms[1]
+            if len(dset_transforms) == 2:
+                dset_trans = dset_transforms[1]
+            else:
+                dset_trans = VectorTranslation(
+                    translation=(0,) * len(base_trans.translation)
+                )
             out_trans = VectorTranslation(
                 translation=tuple(
-                    b + d for b, d in zip(base_trans.scale, dset_trans.scale)
+                    b + d
+                    for b, d in zip(base_trans.translation, dset_trans.translation)
                 )
             )
 
     return out_scale, out_trans
 
 
 def model_group(
-    *, arrays: dict[str, DataArray], transform_precision: int | None = None
-) -> Group:
+    *,
+    arrays: dict[str, DataArray],
+    transform_precision: int | None = None,
+    chunks: tuple[int, ...] | tuple[tuple[int, ...]] | Literal["auto"] = "auto",
+    compressor: Codec | None = Zstd(3),
+    fill_value: Any = 0,
+) -> MultiscaleGroup:
     """
     Create a model of an OME-NGFF multiscale group from a dict of `xarray.DataArray`.
     The dimensions / coordinates of the arrays will be used to infer OME-NGFF axis metadata, as well
     as the OME-NGFF coordinate transformation metadata (i.e., scaling and translation).
 
     Parameters
     ----------
@@ -336,38 +346,45 @@
                 transforms_from_coords(
                     a.coords, transform_precision=transform_precision
                 )
                 for a in arrays.values()
             )
         )
     )
-    # requires a fix upstream to make models hashable
-    # if len(set(axeses)) != 1:
-    #    raise ValueError(
-    #        f"Got {len(set(axeses))} unique axes from `arrays`",
-    #        "which suggests means that their dimensions and / or coordinates are incompatible.",
-    #    )
-
-    group = Group.from_arrays(
-        arrays=arrays.values(),
-        paths=arrays.keys(),
+
+    if len(set(axeses)) != 1:
+        msg = (
+            f"Got {len(set(axeses))} unique axes from `arrays` "
+            "which means that their dimensions and / or coordinates are incompatible."
+        )
+        raise ValueError(msg)
+
+    group = MultiscaleGroup.from_arrays(
+        arrays=tuple(arrays.values()),
+        paths=tuple(arrays.keys()),
         axes=axeses[0],
         scales=[tx[0].scale for tx in transformses],
         translations=[tx[1].translation for tx in transformses],
+        chunks=chunks,
+        compressor=compressor,
+        fill_value=fill_value,
     )
     return group
 
 
 def create_group(
     *,
     store: BaseStore,
     path: str,
     arrays: dict[str, DataArray],
     transform_precision: int | None = None,
-):
+    chunks: tuple[int, ...] | tuple[tuple[int, ...]] | Literal["auto"] = "auto",
+    compressor: Codec | None = Zstd(3),
+    fill_value: Any = 0,
+) -> zarr.Group:
     """
     Create Zarr group that complies with 0.4 of the OME-NGFF multiscale specification from a dict
     of `xarray.DataArray`.
 
     Parameters
     ----------
 
@@ -378,22 +395,30 @@
     transform_precision: int | None, default is None
         Whether, and how much, to round the transformations estimated from the coordinates.
         The default (`None`) results in no rounding; specifying an `int` x will round transforms to
         x decimal places using `numpy.round(transform, x)`.
 
     """
 
-    model = model_group(arrays=arrays, transform_precision=transform_precision)
+    model = model_group(
+        arrays=arrays,
+        transform_precision=transform_precision,
+        chunks=chunks,
+        compressor=compressor,
+        fill_value=fill_value,
+    )
     return model.to_zarr(store, path)
 
 
 def read_group(
     group: zarr.Group,
     *,
-    array_wrapper: BaseArrayWrapper | ArrayWrapperSpec = ZarrArrayWrapper(),
+    array_wrapper: (
+        ZarrArrayWrapper | DaskArrayWrapper | ArrayWrapperSpec
+    ) = ZarrArrayWrapper(),
     multiscales_index: int = 0,
 ) -> dict[str, DataArray]:
     """
     Create a dictionary of `xarray.DataArray` from a Zarr group that implements version 0.4 of the
     OME-NGFF multiscale image specification.
 
     The keys of the dictionary are the paths to the Zarr arrays. The values of the dictionary are
@@ -418,50 +443,54 @@
 
     Returns
     -------
     dict[str, DataArray]
     """
     result: dict[str, DataArray] = {}
     # parse the zarr group as a multiscale group
-    multiscale_group_parsed = Group.from_zarr(group)
+    multiscale_group_parsed = MultiscaleGroup.from_zarr(group)
     multi_meta = multiscale_group_parsed.attributes.multiscales[multiscales_index]
     multi_tx = multi_meta.coordinateTransformations
     wrapper_parsed = parse_wrapper(array_wrapper)
 
     for dset in multi_meta.datasets:
-        tx_fused = fuse_coordinate_transforms(multi_tx, dset.coordinateTransformations)
+        tx_fused = normalize_transforms(multi_tx, dset.coordinateTransformations)
         arr_z: zarr.Array = group[dset.path]
         arr_wrapped = wrapper_parsed.wrap(arr_z)
-        coords = coords_from_transforms(multi_meta.axes, tx_fused, arr_z.shape)
+        coords = coords_from_transforms(
+            axes=multi_meta.axes, transforms=tx_fused, shape=arr_z.shape
+        )
         arr_out = DataArray(data=arr_wrapped, coords=coords)
         result[dset.path] = arr_out
 
     return result
 
 
-def get_parent(node: zarr.Group | zarr.Array):
+def get_parent(node: zarr.Group | zarr.Array) -> zarr.Group:
     """
     Get the parent node of a Zarr array or group
     """
     if hasattr(node.store, "path"):
         store_path = node.store.path
         if node.path == "":
             new_full_path, new_node_path = os.path.split(os.path.split(store_path)[0])
         else:
             full_path, _ = os.path.split(os.path.join(store_path, node.path))
             new_full_path, new_node_path = os.path.split(full_path)
         return zarr.open_group(type(node.store)(new_full_path), path=new_node_path)
     else:
-        return zarr.open(store=node.store, path=os.path.split(node.path)[0])
+        return zarr.open_group(store=node.store, path=os.path.split(node.path)[0])
 
 
 def read_array(
     array: zarr.Array,
     *,
-    array_wrapper: BaseArrayWrapper | ArrayWrapperSpec = ZarrArrayWrapper(),
+    array_wrapper: (
+        ZarrArrayWrapper | DaskArrayWrapper | ArrayWrapperSpec
+    ) = ZarrArrayWrapper(),
 ) -> DataArray:
     """
     Read a single Zarr array as an `xarray.DataArray`, using version 0.4 OME-NGFF multiscale
     metadata.
 
     The information necessary for creating the coordinates of the `DataArray` are not stored
     in the attributes of the Zarr array given to this function. Instead, the coordinates must
@@ -470,15 +499,15 @@
     whether that metadata references the provided array. Once the correct multiscales metadata is
     found, the coordinates can be constructed correctly.
 
     Parameters
     ----------
     array: zarr.Array
         A Zarr array that is part of a version 0.4 OME-NGFF multiscale image.
-    array_wrapper: BaseArrayWrapper | ArrayWrapperSpec, default is ZarrArrayWrapper
+    array_wrapper: ZarrArrayWrapper | DaskArrayWrapper | ArrayWrapperSpec, default is ZarrArrayWrapper
         The array wrapper class to use when converting the Zarr array to an `xarray.DataArray`.
     Returns
     -------
     xarray.DataArray
     """
 
     if hasattr(array.store, "path"):
@@ -498,25 +527,25 @@
     for _ in range(num_parents):
         if hasattr(parent.store, "path"):
             parent_path = os.path.join(parent.store.path, parent.path)
         else:
             parent_path = parent.path
         array_path_rel = os.path.relpath(full_path, parent_path)
         try:
-            model = Group.from_zarr(parent)
+            model = MultiscaleGroup.from_zarr(parent)
             for multi in model.attributes.multiscales:
                 multi_tx = multi.coordinateTransformations
 
                 for dset in multi.datasets:
                     if dset.path == array_path_rel:
-                        tx_fused = fuse_coordinate_transforms(
+                        tx_fused = normalize_transforms(
                             multi_tx, dset.coordinateTransformations
                         )
                         coords = coords_from_transforms(
-                            multi.axes, tx_fused, array.shape
+                            axes=multi.axes, transforms=tx_fused, shape=array.shape
                         )
                         arr_wrapped = wrapper.wrap(array)
                         return DataArray(arr_wrapped, coords=coords)
         except ValueError:
             parent = get_parent(parent)
     raise FileNotFoundError(
         f"Could not find version 0.4 OME-NGFF multiscale metadata in any Zarr groups in the "
```

### Comparing `xarray_ome_ngff-2.0.0/PKG-INFO` & `xarray_ome_ngff-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarray-ome-ngff
-Version: 2.0.0
+Version: 2.1.0
 Summary: xarray and ome-ngff
 Author: Davis Vann Bennett
 Author-email: davis.v.bennett@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -19,16 +19,15 @@
 Description-Content-Type: text/markdown
 
 # xarray-ome-ngff
 
 Integrating [Xarray](https://docs.xarray.dev/en/stable/) with [OME-NGFF](https://ngff.openmicroscopy.org/).
 
 ## Help
-
-See [documentation](https://janeliscicomp.github.io/xarray-multiscale) for more details
+See [documentation](https://janeliascicomp.github.io/xarray-ome-ngff/) for more details
 
 ## Usage
 
 ### Read OME-NGFF data
 
 ```python
 import zarr
```

