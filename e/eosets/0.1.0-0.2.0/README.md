# Comparing `tmp/eosets-0.1.0.tar.gz` & `tmp/eosets-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eosets-0.1.0.tar", last modified: Wed Jul 19 09:41:29 2023, max compression
+gzip compressed data, was "eosets-0.2.0.tar", last modified: Wed Apr 24 13:17:47 2024, max compression
```

## Comparing `eosets-0.1.0.tar` & `eosets-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:41:29.784636 eosets-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-07-19 09:41:16.000000 eosets-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-19 09:41:16.000000 eosets-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-19 09:41:16.000000 eosets-0.1.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-19 09:41:29.784636 eosets-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-19 09:41:16.000000 eosets-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:41:29.780636 eosets-0.1.0/eosets/
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-19 09:41:17.000000 eosets-0.1.0/eosets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-19 09:41:17.000000 eosets-0.1.0/eosets/__meta__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-19 09:41:17.000000 eosets-0.1.0/eosets/env_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-19 09:41:17.000000 eosets-0.1.0/eosets/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17107 2023-07-19 09:41:17.000000 eosets-0.1.0/eosets/mosaic.py
--rw-r--r--   0 runner    (1001) docker     (123)    18277 2023-07-19 09:41:17.000000 eosets-0.1.0/eosets/pair.py
--rw-r--r--   0 runner    (1001) docker     (123)    16198 2023-07-19 09:41:17.000000 eosets-0.1.0/eosets/series.py
--rw-r--r--   0 runner    (1001) docker     (123)    13526 2023-07-19 09:41:17.000000 eosets-0.1.0/eosets/set.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-19 09:41:17.000000 eosets-0.1.0/eosets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:41:29.780636 eosets-0.1.0/eosets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-19 09:41:29.000000 eosets-0.1.0/eosets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-19 09:41:29.000000 eosets-0.1.0/eosets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 09:41:29.000000 eosets-0.1.0/eosets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-19 09:41:29.000000 eosets-0.1.0/eosets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-19 09:41:29.000000 eosets-0.1.0/eosets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-19 09:41:17.000000 eosets-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-19 09:41:29.784636 eosets-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-19 09:41:17.000000 eosets-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:17:47.578109 eosets-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10166 2024-04-24 13:17:39.000000 eosets-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-24 13:17:39.000000 eosets-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-24 13:17:39.000000 eosets-0.2.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-24 13:17:47.578109 eosets-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-24 13:17:39.000000 eosets-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:17:47.574109 eosets-0.2.0/eosets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-24 13:17:39.000000 eosets-0.2.0/eosets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-24 13:17:39.000000 eosets-0.2.0/eosets/__meta__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-24 13:17:39.000000 eosets-0.2.0/eosets/env_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-24 13:17:39.000000 eosets-0.2.0/eosets/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17577 2024-04-24 13:17:39.000000 eosets-0.2.0/eosets/mosaic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19829 2024-04-24 13:17:39.000000 eosets-0.2.0/eosets/pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16006 2024-04-24 13:17:39.000000 eosets-0.2.0/eosets/series.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13465 2024-04-24 13:17:39.000000 eosets-0.2.0/eosets/set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-24 13:17:39.000000 eosets-0.2.0/eosets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:17:47.578109 eosets-0.2.0/eosets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-24 13:17:47.000000 eosets-0.2.0/eosets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-24 13:17:47.000000 eosets-0.2.0/eosets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:17:47.000000 eosets-0.2.0/eosets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-24 13:17:47.000000 eosets-0.2.0/eosets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 13:17:47.000000 eosets-0.2.0/eosets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-24 13:17:39.000000 eosets-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-24 13:17:47.578109 eosets-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-24 13:17:39.000000 eosets-0.2.0/setup.py
```

### Comparing `eosets-0.1.0/LICENSE` & `eosets-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eosets-0.1.0/NOTICE` & `eosets-0.2.0/NOTICE`

 * *Files identical despite different names*

### Comparing `eosets-0.1.0/PKG-INFO` & `eosets-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eosets
-Version: 0.1.0
+Version: 0.2.0
 Summary: This library aims to simplify any process working with different sets of EO data handled by EOReader.
 Home-page: UNKNOWN
 Author: ICube-SERTIT
 Author-email: dev-sertit@unistra.fr
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/sertit/eosets/issues/
 Project-URL: Documentation, https://eosets.readthedocs.io/en/latest/
```

### Comparing `eosets-0.1.0/README.md` & `eosets-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `eosets-0.1.0/eosets/__init__.py` & `eosets-0.2.0/eosets/__init__.py`

 * *Files identical despite different names*

### Comparing `eosets-0.1.0/eosets/__meta__.py` & `eosets-0.2.0/eosets/__meta__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 **EOSets** library
 """
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 __title__ = "eosets"
 __description__ = "This library aims to simplify any process working with different sets of EO data handled by EOReader."
 __author__ = "ICube-SERTIT"
 __author_email__ = "dev-sertit@unistra.fr"
 __url__ = "https://github.com/sertit/eosets"
 __license__ = "Apache 2.0"
 __copyright__ = "Copyright 2023, SERTIT-ICube - France, https://sertit.unistra.fr/"
```

### Comparing `eosets-0.1.0/eosets/env_vars.py` & `eosets-0.2.0/eosets/env_vars.py`

 * *Files identical despite different names*

### Comparing `eosets-0.1.0/eosets/exceptions.py` & `eosets-0.2.0/eosets/exceptions.py`

 * *Files identical despite different names*

### Comparing `eosets-0.1.0/eosets/mosaic.py` & `eosets-0.2.0/eosets/mosaic.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,32 +17,31 @@
 """ Class implementing the mosaic object """
 import logging
 import os
 import shutil
 from collections import defaultdict
 from enum import unique
 from glob import glob
-from pathlib import Path
 from typing import Union
 
 import geopandas as gpd
 import xarray as xr
-from cloudpathlib import AnyPath, CloudPath
 from eoreader import cache, utils
 from eoreader.bands import BandNames, is_spectral_band, to_band, to_str
 from eoreader.products import Product
 from eoreader.reader import Reader
 from eoreader.utils import UINT16_NODATA
-from sertit import rasters
+from sertit import AnyPath, files, rasters
 from sertit.misc import ListEnum
+from sertit.types import AnyPathStrType
 
 from eosets import EOSETS_NAME
 from eosets.exceptions import IncompatibleProducts
 from eosets.set import GeometryCheck, Set
-from eosets.utils import AnyPathType
+from eosets.utils import AnyPathType, stack
 
 READER = Reader()
 
 LOGGER = logging.getLogger(EOSETS_NAME)
 
 
 @unique
@@ -124,23 +123,23 @@
                 prod.output = self._get_tmp_folder(writable=True)
             except FileNotFoundError:
                 # Never mind for non-existing files: they have already been copied :)
                 pass
 
     def _manage_prods(
         self,
-        paths: Union[list, str, Path, CloudPath],
+        paths: Union[list, AnyPathStrType],
         contiguity_check: GeometryCheck,
         **kwargs,
     ):
         """
         Manage products attributes and check the compatibility of the mosaic's components
 
         Args:
-            paths (Union[list, str, Path, CloudPath]): Paths of the mosaic
+            paths (Union[list, AnyPathStrType]): Paths of the mosaic
             contiguity_check (GeometryCheck): Method to check the contiguity of the mosaic
             **kwargs: Other arguments
 
         Raises:
             IncompatibleProducts: Incompatible products if not contiguous or not the same date
         """
         # Manage reference product
@@ -354,57 +353,67 @@
             for band in bands_to_load:
                 assert prod.has_band(
                     band
                 ), f"{prod.condensed_name} has not a {to_str(band)[0]} band."
 
         # Load and reorganize bands
         prod_band_paths = defaultdict(list)
-        for prod in self.get_prods():
-            prod: Product
-            LOGGER.debug(
-                f"*** Loading {to_str(bands_to_load)} for {prod.condensed_name} ***"
-            )
+        if bands_to_load:
+            for prod in self.get_prods():
+                prod: Product
+                LOGGER.debug(
+                    f"*** Loading {to_str(bands_to_load)} for {prod.condensed_name} ***"
+                )
 
-            # Load bands
-            prod.load(bands_to_load, pixel_size, **kwargs).keys()
+                # Load bands
+                prod.load(bands_to_load, pixel_size, **kwargs).keys()
 
-            # Store paths
-            for band in bands_to_load:
-                if is_spectral_band(band):
-                    band_path = prod.get_band_paths([band], pixel_size, **kwargs)[band]
-                else:
-                    # Use glob fct as _get_band_folder is a tmpDirectory
-                    band_path = glob(
-                        os.path.join(prod._get_band_folder(), f"*{to_str(band)[0]}*")
-                    )[0]
+                # Store paths
+                for band in bands_to_load:
+                    if is_spectral_band(band):
+                        band_path = prod.get_band_paths([band], pixel_size, **kwargs)[
+                            band
+                        ]
+                    else:
+                        # Use glob fct as _get_band_folder is a tmpDirectory
+                        band_path = glob(
+                            os.path.join(
+                                prod._get_band_folder(), f"*_{to_str(band)[0]}_*"
+                            )
+                        )[0]
 
-                prod_band_paths[band].append(str(band_path))
+                    prod_band_paths[band].append(str(band_path))
 
         # Merge
         merged_dict = {}
         for band in bands_path:
             output_path = bands_path[band]
             if not output_path.is_file():
                 LOGGER.debug(f"Merging bands {to_str(band)[0]}")
                 if self.mosaic_method == MosaicMethod.VRT:
                     prod_path = []
                     for path in prod_band_paths[band]:
                         out_path, exists = self._get_out_path(os.path.basename(path))
                         if not exists:
-                            shutil.move(path, out_path)
+                            if AnyPath(path).parent.is_relative_to(self.output):
+                                # If EOReader's band: move
+                                shutil.move(path, out_path)
+                            else:
+                                # If raw product's band: copy
+                                files.copy(path, out_path)
                         prod_path.append(out_path)
                 else:
                     prod_path = prod_band_paths[band]
 
                 # Don't pass kwargs here because of unwanted errors
                 merge_fct(prod_path, output_path)
 
             # Load in memory and update attribute
             merged_dict[band] = self._update_attrs(
-                rasters.read(output_path), bands, **kwargs
+                utils.read(output_path), bands, **kwargs
             )
 
         # Collocate VRTs
         LOGGER.debug("Collocating bands")
         merged_dict = self._collocate_bands(merged_dict)
 
         # Create a dataset (only after collocation)
@@ -452,25 +461,25 @@
         band_ds = self.load(bands, pixel_size=pixel_size, **kwargs)
 
         # Stack bands
         if save_as_int:
             nodata = kwargs.get("nodata", UINT16_NODATA)
         else:
             nodata = kwargs.get("nodata", self.nodata)
-        stack, dtype = utils.stack_dict(bands, band_ds, save_as_int, nodata, **kwargs)
+        stk, dtype = stack(bands, band_ds, save_as_int, nodata, **kwargs)
 
         # Update stack's attributes
-        stack = self._update_attrs(stack, bands, **kwargs)
+        stk = self._update_attrs(stk, bands, **kwargs)
 
         # Write on disk
         if stack_path:
             LOGGER.debug("Saving stack")
-            utils.write(stack, stack_path, dtype=dtype, **kwargs)
+            utils.write(stk, stack_path, dtype=dtype, **kwargs)
 
-        return stack
+        return stk
 
     def _collocate_bands(self, bands: dict, reference: xr.DataArray = None) -> dict:
         """
         Collocate all bands from a dict
 
         Args:
             bands (dict): Dict of bands to collocate if needed
```

### Comparing `eosets-0.1.0/eosets/series.py` & `eosets-0.2.0/eosets/series.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,33 +15,33 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """ Class implementing the series object """
 import logging
 import os
 from collections import defaultdict
 from enum import unique
-from pathlib import Path
 from typing import Union
 
 import geopandas as gpd
 import numpy as np
 import xarray as xr
-from cloudpathlib import AnyPath, CloudPath
 from eoreader import cache
 from eoreader.bands import BandNames, to_band, to_str
 from eoreader.reader import Reader
 from eoreader.utils import UINT16_NODATA
 from rasterio.enums import Resampling
+from sertit import AnyPath
 from sertit.misc import ListEnum
+from sertit.types import AnyPathStrType
 
 from eosets import EOSETS_NAME
 from eosets.exceptions import IncompatibleProducts
 from eosets.mosaic import Mosaic
 from eosets.set import GeometryCheck, Set
-from eosets.utils import AnyPathType, read, stack_dict, write
+from eosets.utils import AnyPathType, read, stack, write
 
 LOGGER = logging.getLogger(EOSETS_NAME)
 READER = Reader()
 
 
 @unique
 class Alignment(ListEnum):
@@ -76,38 +76,38 @@
 class Series(Set):
     """Class of series"""
 
     def __init__(
         self,
         paths: list,
         id: str = None,
-        output_path: Union[str, Path, CloudPath] = None,
+        output_path: Union[AnyPathStrType] = None,
         remove_tmp: bool = True,
         overlap_check: Union[GeometryCheck, str] = GeometryCheck.EXTENT,
         contiguity_check: Union[GeometryCheck, str] = GeometryCheck.EXTENT,
         alignement: Union[Alignment, str] = Alignment.FIRST,
         coregister: bool = False,
-        ruling_mosaic: Union[Mosaic, int, str] = None,
+        reference_mosaic: Union[Mosaic, int, str] = None,
         **kwargs,
     ):
         # Manage mosaics
         self.mosaics = None
-        """ Pivot mosaic (unique date and contiguous). The one on which the child will be aligned. """
+        """ Mosaics composing the series. """
 
         self.id = None
         """ ID of the series """
 
         self.alignment = Alignment.convert_from(alignement)[0]
         """ Series alignment (on first mosaic, on last mosaic, on a hypothetical mean product). """
 
         self.coregister = coregister
         """ Do we need to coregister the time series? """
 
-        self.ruling_mosaic = ruling_mosaic
-        """ Ruling mosaic """
+        self.reference_mosaic = reference_mosaic
+        """ Reference mosaic """
 
         self._unique_mosaic = len(paths) == 1
 
         contiguity_check = GeometryCheck.convert_from(contiguity_check)[0]
         overlap_check = GeometryCheck.convert_from(overlap_check)[0]
 
         # Init the base class
@@ -205,104 +205,104 @@
             else:
                 raise IncompatibleProducts(
                     "All mosaics of a series should have a different datetime! If not, please regroup them in a unique mosaic."
                 )
 
         # Check geometry
         if overlap_check != GeometryCheck.NONE:
-            ruling_geom: gpd.GeoDataFrame = getattr(
-                self.ruling_mosaic, str(overlap_check.value)
+            reference_geom: gpd.GeoDataFrame = getattr(
+                self.reference_mosaic, str(overlap_check.value)
             )()
             for mos in self.mosaics:
-                if mos.id != self.ruling_mosaic.id:
+                if mos.id != self.reference_mosaic.id:
                     mos_geom: gpd.GeoDataFrame = getattr(
                         mos, str(overlap_check.value)
                     )()
-                    if not ruling_geom.intersects(
-                        mos_geom.to_crs(self.ruling_mosaic.crs)
+                    if not reference_geom.intersects(
+                        mos_geom.to_crs(self.reference_mosaic.crs)
                     ).all():
                         raise IncompatibleProducts("All mosaics should overlap!")
 
         # Fill other attributes
         self.nof_prods = len(self.get_prods())
         self.id = "_".join(mos.id for mos in self.mosaics)
         self.full_name = "_".join(mos.full_name for mos in self.mosaics)
         self.condensed_name = self.full_name
         # TODO (how to name series ???)
 
     @property
-    def ruling_mosaic(self) -> Mosaic:
+    def reference_mosaic(self) -> Mosaic:
         """
-        Get the ruling mosaic of the series
+        Get the reference mosaic of the series
 
         Returns:
             Mosaic: Output path ofthe mosaic
         """
         if self.alignment in [Alignment.FIRST, Alignment.LAST]:
-            return self.mosaics[self._ruling_mosaic]
+            return self.mosaics[self._reference_mosaic]
         elif self.alignment == Alignment.MEAN:
             raise NotImplementedError
         elif self.alignment == Alignment.EXTERNAL:
-            return self._ruling_mosaic
+            return self._reference_mosaic
         elif self.alignment == Alignment.CUSTOM:
-            if isinstance(self._ruling_mosaic, int):
-                return self.mosaics[self._ruling_mosaic]
+            if isinstance(self._reference_mosaic, int):
+                return self.mosaics[self._reference_mosaic]
 
-    @ruling_mosaic.setter
-    def ruling_mosaic(self, mosaic: Union[Mosaic, int] = None):
+    @reference_mosaic.setter
+    def reference_mosaic(self, mosaic: Union[Mosaic, int] = None):
         if self.alignment == Alignment.FIRST:
-            self._ruling_mosaic = 0
+            self._reference_mosaic = 0
         elif self.alignment == Alignment.LAST:
-            self._ruling_mosaic = -1
+            self._reference_mosaic = -1
         elif self.alignment == Alignment.MEAN:
             raise NotImplementedError
         elif self.alignment == Alignment.EXTERNAL:
             assert mosaic is not None
-            self._ruling_mosaic = mosaic
+            self._reference_mosaic = mosaic
         elif self.alignment == Alignment.CUSTOM:
             assert isinstance(mosaic, (Mosaic, int))
             if isinstance(mosaic, int):
                 assert abs(mosaic) <= len(self.mosaics)
-            self._ruling_mosaic = mosaic
+            self._reference_mosaic = mosaic
 
     def read_mtd(self):
         """Read the pair's metadata, but not implemented for now."""
         # TODO: how ? Just return the fields that are shared between series' components ? Or create a XML from scratch ?
         raise NotImplementedError
 
     @cache
     def footprint(self) -> gpd.GeoDataFrame:
         """
-        Get the footprint of the series, i.e. the intersection between all mosaics in the ruling mosaic's CRS.
+        Get the footprint of the series, i.e. the intersection between all mosaics in the reference mosaic's CRS.
 
         Returns:
             gpd.GeoDataFrame: Footprint of the mosaic
         """
         footprint = None
         for mos in self.mosaics:
-            geom: gpd.GeoDataFrame = mos.footprint().to_crs(self.ruling_mosaic.crs)
+            geom: gpd.GeoDataFrame = mos.footprint().to_crs(self.reference_mosaic.crs)
             if footprint is None:
                 footprint = geom
             else:
                 footprint = footprint.overlay(geom, "intersection")
 
         return footprint
 
     @cache
     def extent(self) -> gpd.GeoDataFrame:
         """
-        Get the extent of the series, i.e. the intersection between all mosaics in the ruling mosaic's CRS.
+        Get the extent of the series, i.e. the intersection between all mosaics in the reference mosaic's CRS.
 
         Returns:
             gpd.GeoDataFrame: Extent of the mosaic
 
         """
         extent = None
         for mos in self.mosaics:
-            geom: gpd.GeoDataFrame = mos.footprint().to_crs(self.ruling_mosaic.crs)
+            geom: gpd.GeoDataFrame = mos.footprint().to_crs(self.reference_mosaic.crs)
             if extent is None:
                 extent = geom
             else:
                 extent = extent.overlay(geom, "intersection")
 
         return extent
 
@@ -327,59 +327,59 @@
             xr.Dataset: Wanted bands as xr.Datasets
         """
         bands = to_band(bands)
 
         # Load bands
         window = kwargs.pop("window", self.footprint())
 
-        # Load pivot bands
-        ruling_ds = self.ruling_mosaic.load(
+        # Load reference mosaic bands
+        reference_ds = self.reference_mosaic.load(
             bands, pixel_size=pixel_size, window=window, **kwargs
-        ).expand_dims({"time": [self.ruling_mosaic.datetime]}, axis=-1)
+        ).expand_dims({"time": [self.reference_mosaic.datetime]}, axis=-1)
 
         # Load mosaic bands
         arr_dict = defaultdict(list)
         for mos_id, mos in enumerate(self.mosaics):
             # Get mosaic datetime
             dt = mos.datetime
 
             # Manage if band to be loaded or already on memory
-            if mos.id != self.ruling_mosaic.id:
+            if mos.id != self.reference_mosaic.id:
                 # Load bands for new mosaic
                 mos_ds = mos.load(bands, pixel_size=pixel_size, window=window, **kwargs)
 
                 # Add the bands to the dataset
                 for band in bands:
                     mos_arr = mos_ds[band]
-                    ruling_arr = ruling_ds[band]
+                    reference_arr = reference_ds[band]
 
                     # To be sure, always collocate arrays, even if the size is the same
                     # Indeed, a small difference in the coordinates will lead to empy arrays
                     # So the bands MUST BE exactly aligned
                     mos_arr = (
                         mos_arr.rio.reproject_match(
-                            ruling_arr, resampling=resampling, **kwargs
+                            reference_arr, resampling=resampling, **kwargs
                         )
                         .expand_dims({"time": [dt]}, axis=-1)
                         .assign_coords({"time": [dt]})
                     )
 
                     # Save mosaics
                     arr_dict[band].append(mos_arr)
             else:
                 # We already have the bands in memory, just assign time to every arrays and save it
                 for band in bands:
-                    mos_arr = ruling_ds[band].assign_coords({"time": [dt]})
+                    mos_arr = reference_ds[band].assign_coords({"time": [dt]})
                     arr_dict[band].append(mos_arr)
 
         # Create empty dataset with correct coordinates
         series_ds = xr.Dataset(
             coords={
-                "x": ruling_ds.x,
-                "y": ruling_ds.y,
+                "x": reference_ds.x,
+                "y": reference_ds.y,
                 "band": np.arange(1, len(self.mosaics) + 1),  # One array per band
                 "time": [mos.datetime for mos in self.mosaics],
             }
         )
 
         # Make sure the dataset has the bands in the right order -> re-order the input dict
         series_ds = xr.merge([xr.merge(arr_dict[band]) for band in bands])
@@ -398,15 +398,15 @@
         **kwargs,
     ) -> xr.DataArray:
         """
         Stack bands and index of a series.
 
         Args:
             bands (list): Bands and index combination
-            pixel_size (float): Stack pixel size. . If not specified, use the product pixel size.
+            pixel_size (float): Stack pixel size. If not specified, use the product pixel size.
             stack_path (Union[str, AnyPathType]): Stack path
             save_as_int (bool): Convert stack to uint16 to save disk space (and therefore multiply the values by 10.000)
             **kwargs: Other arguments passed to :code:`load` or :code:`rioxarray.to_raster()` (such as :code:`compress`)
 
         Returns:
             xr.DataArray: Stack as a DataArray
         """
@@ -422,41 +422,37 @@
             else:
                 os.makedirs(str(stack_path.parent), exist_ok=True)
 
         # Load all bands
         band_ds = self.load(bands, pixel_size=pixel_size, **kwargs)
 
         # Rename bands and remove time variable
-        coords = {"x": band_ds.x, "y": band_ds.y, "band": 1}
-        stk_dict = {}
+        new_bands = []
         for band in bands:
             for idx, dt in enumerate(band_ds.time.values):
-                stk_dict[
+                new_bands.append(
                     f"{np.datetime_as_string(dt, unit='s')}_{to_str(band)[0]}"
-                ] = band_ds[band].sel(time=dt, drop=True)
-
-        # Create a dataset correctly formatted for stacking
-        stack_ds = xr.Dataset(stk_dict, coords=coords)
+                )
 
         # Stack bands
         if save_as_int:
             nodata = kwargs.get("nodata", UINT16_NODATA)
         else:
             nodata = kwargs.get("nodata", self.nodata)
-        stack, dtype = stack_dict(bands, stack_ds, save_as_int, nodata, **kwargs)
+        stk, dtype = stack(bands, band_ds, save_as_int, nodata, **kwargs)
 
         # Update stack's attributes
-        stack = self._update_attrs(stack, list(stk_dict.keys()), **kwargs)
+        stk = self._update_attrs(stk, new_bands, **kwargs)
 
         # Write on disk
         if stack_path:
             LOGGER.debug("Saving stack")
-            write(stack, stack_path, dtype=dtype, **kwargs)
+            write(stk, stack_path, dtype=dtype, **kwargs)
 
-        return stack
+        return stk
 
     def _update_attrs_constellation_specific(
         self, xarr: xr.DataArray, bands: list, **kwargs
     ) -> xr.DataArray:
         """
         Update attributes of the given array (constellation specific)
```

### Comparing `eosets-0.1.0/eosets/set.py` & `eosets-0.2.0/eosets/set.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,18 +21,17 @@
 import tempfile
 from abc import abstractmethod
 from enum import unique
 from typing import Any, Tuple, Union
 
 import geopandas as gpd
 import xarray as xr
-from cloudpathlib import AnyPath, CloudPath
 from eoreader.bands import BandNames, to_str
 from eoreader.products import Product
-from sertit import files
+from sertit import AnyPath, files, path
 from sertit.misc import ListEnum
 
 from eosets import EOSETS_NAME
 from eosets.env_vars import CI_EOSETS_BAND_FOLDER
 from eosets.utils import AnyPathType
 
 LOGGER = logging.getLogger(EOSETS_NAME)
@@ -178,15 +177,15 @@
         Output directory of the set
 
         Args:
             value (Union[str, AnyPathType]): Output path of the set
         """
         # Set the new output
         self._output = AnyPath(value)
-        if not isinstance(self._output, CloudPath):
+        if not path.is_cloud_path(self._output):
             self._output = self._output.resolve()
 
         # Create temporary process folder
         old_tmp_process = self._tmp_process
         self._set_tmp_process()
 
         # Update for every sets
@@ -281,20 +280,19 @@
             bool: True if this attribute is the same for all products constituting the mosaic.
         """
         ref_attr = getattr(self.get_first_prod(), attr)
 
         if self.nof_prods > 1:
             if callable(ref_attr):
                 is_homogeneous = all(
-                    ref_attr() == getattr(child, attr)()
-                    for child in self.get_prods()[1:]
+                    ref_attr() == getattr(sec, attr)() for sec in self.get_prods()[1:]
                 )
             else:
                 is_homogeneous = all(
-                    ref_attr == getattr(child, attr) for child in self.get_prods()[1:]
+                    ref_attr == getattr(sec, attr) for sec in self.get_prods()[1:]
                 )
         else:
             is_homogeneous = True
 
         return is_homogeneous
 
     def get_first_prod(self) -> Product:
@@ -436,15 +434,14 @@
         # Update stack's attributes
         if len(xds) > 0:
             xds = self._update_attrs(xds, bands, **kwargs)
 
         return xds
 
     def get_bands_to_load(self, bands, out_suffix="tif") -> (list, dict):
-
         # Get the bands to be loaded
         bands_path = {}
         bands_to_load = []
         for band in bands:
             band_path, exists = self._get_out_path(
                 f"{self.id}_{to_str(band)[0]}.{out_suffix}"
             )
```

### Comparing `eosets-0.1.0/eosets/utils.py` & `eosets-0.2.0/eosets/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,18 +11,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """ Utils file """
-from pathlib import Path
-from typing import Union
 
-from cloudpathlib import CloudPath
 from eoreader import utils
+from sertit import types
 
-AnyPathType = Union[CloudPath, Path]
+AnyPathType = types.AnyPathType
 
 read = utils.read
 write = utils.write
-stack_dict = utils.stack_dict
+stack = utils.stack_dict
```

### Comparing `eosets-0.1.0/eosets.egg-info/PKG-INFO` & `eosets-0.2.0/eosets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eosets
-Version: 0.1.0
+Version: 0.2.0
 Summary: This library aims to simplify any process working with different sets of EO data handled by EOReader.
 Home-page: UNKNOWN
 Author: ICube-SERTIT
 Author-email: dev-sertit@unistra.fr
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/sertit/eosets/issues/
 Project-URL: Documentation, https://eosets.readthedocs.io/en/latest/
```

### Comparing `eosets-0.1.0/setup.py` & `eosets-0.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,29 @@
-import os
-
 import setuptools
 
 from eosets.__meta__ import (
     __author__,
     __author_email__,
     __description__,
     __documentation__,
     __title__,
     __url__,
     __version__,
 )
 
-BASEDIR = os.path.dirname(os.path.abspath(os.path.realpath(__file__)))
-with open(os.path.join(BASEDIR, "README.md"), "r", encoding="utf8") as f:
-    readme = f.read()
+with open("README.md", "r") as fh:
+    long_description = fh.read()
 
 setuptools.setup(
     name=__title__,
     version=__version__,
     author=__author__,
     author_email=__author_email__,
     description=__description__,
-    long_description=readme,
+    long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=[
         "lxml",
         "h5netcdf",
         "scipy",
         "rasterio>=1.3.0",
@@ -36,16 +33,16 @@
         "spyndex>=0.3.0",
         "pyresample",
         "zarr",
         "rtree",
         "validators",
         "methodtools",
         "dicttoxml",
-        "eoreader>0.20.0",
-        "sertit[full]>=1.27.3",
+        "eoreader>=0.21.1",
+        "sertit[full]>=1.36.1",
     ],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "License :: OSI Approved :: Apache Software License",
```

