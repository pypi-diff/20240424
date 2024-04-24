# Comparing `tmp/stac_geoparquet-0.5.0.tar.gz` & `tmp/stac_geoparquet-0.5.1.tar.gz`

## Comparing `stac_geoparquet-0.5.0.tar` & `stac_geoparquet-0.5.1.tar`

### file list

```diff
@@ -1,46 +1,50 @@
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/.dockerignore
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/Dockerfile
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/setup.cfg
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/.github/workflows/continuous-integration.yml
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0    11225 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/spec/stac-geoparquet-spec.md
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/stac_geoparquet/__init__.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/stac_geoparquet/_compat.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/stac_geoparquet/_version.py
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/stac_geoparquet/cli.py
--rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/stac_geoparquet/from_arrow.py
--rw-r--r--   0        0        0     4710 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/stac_geoparquet/pc_runner.py
--rw-r--r--   0        0        0    12213 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/stac_geoparquet/pgstac_reader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/stac_geoparquet/py.typed
--rw-r--r--   0        0        0     8159 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/stac_geoparquet/stac_geoparquet.py
--rw-r--r--   0        0        0    12547 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/stac_geoparquet/to_arrow.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/stac_geoparquet/to_parquet.py
--rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/stac_geoparquet/utils.py
--rw-r--r--   0        0        0     5315 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/tests/base_sentinel2_l2a.json
--rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/tests/record_sentinel2_l2a.json
--rw-r--r--   0        0        0    15533 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/tests/sentinel-2-item.json
--rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/tests/test_arrow.py
--rw-r--r--   0        0        0     7348 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/tests/test_pgstac_reader.py
--rw-r--r--   0        0        0    15912 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/tests/test_stac_geoparquet.py
--rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/tests/test_to_dict.py
--rw-r--r--   0        0        0    39820 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/tests/data/3dep-lidar-copc-pc.json
--rw-r--r--   0        0        0   108915 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/tests/data/3dep-lidar-dsm-pc.json
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/tests/data/README.md
--rw-r--r--   0        0        0    14694 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/tests/data/cop-dem-glo-30-pc.json
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/tests/data/download.py
--rw-r--r--   0        0        0    50278 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/tests/data/io-lulc-annual-v02-pc.json
--rw-r--r--   0        0        0    43358 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/tests/data/io-lulc-pc.json
--rw-r--r--   0        0        0    67977 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/tests/data/landsat-c2-l1-pc.json
--rw-r--r--   0        0        0   149737 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/tests/data/landsat-c2-l2-pc.json
--rw-r--r--   0        0        0    17990 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/tests/data/naip-pc.json
--rw-r--r--   0        0        0    31869 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/tests/data/naip.parquet
--rw-r--r--   0        0        0    32984 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/tests/data/planet-nicfi-analytic-pc.json
--rw-r--r--   0        0        0    30476 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/tests/data/sentinel-1-rtc-pc.json
--rw-r--r--   0        0        0    98846 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/tests/data/sentinel-2-l2a-pc.json
--rw-r--r--   0        0        0    43820 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/tests/data/us-census-pc.json
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/LICENSE
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/README.md
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/.dockerignore
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/Dockerfile
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/setup.cfg
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/.github/workflows/continuous-integration.yml
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0    11225 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/spec/stac-geoparquet-spec.md
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/stac_geoparquet/__init__.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/stac_geoparquet/_compat.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/stac_geoparquet/_version.py
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/stac_geoparquet/cli.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/stac_geoparquet/from_arrow.py
+-rw-r--r--   0        0        0     4710 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/stac_geoparquet/pc_runner.py
+-rw-r--r--   0        0        0    12213 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/stac_geoparquet/pgstac_reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/stac_geoparquet/py.typed
+-rw-r--r--   0        0        0     8159 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/stac_geoparquet/stac_geoparquet.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/stac_geoparquet/to_arrow.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/stac_geoparquet/to_parquet.py
+-rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/stac_geoparquet/utils.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/stac_geoparquet/arrow/__init__.py
+-rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/stac_geoparquet/arrow/_from_arrow.py
+-rw-r--r--   0        0        0    12549 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/stac_geoparquet/arrow/_to_arrow.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/stac_geoparquet/arrow/_to_parquet.py
+-rw-r--r--   0        0        0     5315 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/tests/base_sentinel2_l2a.json
+-rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/tests/record_sentinel2_l2a.json
+-rw-r--r--   0        0        0    15533 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/tests/sentinel-2-item.json
+-rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/tests/test_arrow.py
+-rw-r--r--   0        0        0     7348 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/tests/test_pgstac_reader.py
+-rw-r--r--   0        0        0    15912 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/tests/test_stac_geoparquet.py
+-rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/tests/test_to_dict.py
+-rw-r--r--   0        0        0    39820 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/tests/data/3dep-lidar-copc-pc.json
+-rw-r--r--   0        0        0   108915 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/tests/data/3dep-lidar-dsm-pc.json
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/tests/data/README.md
+-rw-r--r--   0        0        0    14694 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/tests/data/cop-dem-glo-30-pc.json
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/tests/data/download.py
+-rw-r--r--   0        0        0    50278 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/tests/data/io-lulc-annual-v02-pc.json
+-rw-r--r--   0        0        0    43358 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/tests/data/io-lulc-pc.json
+-rw-r--r--   0        0        0    67977 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/tests/data/landsat-c2-l1-pc.json
+-rw-r--r--   0        0        0   149737 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/tests/data/landsat-c2-l2-pc.json
+-rw-r--r--   0        0        0    17990 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/tests/data/naip-pc.json
+-rw-r--r--   0        0        0    31869 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/tests/data/naip.parquet
+-rw-r--r--   0        0        0    32984 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/tests/data/planet-nicfi-analytic-pc.json
+-rw-r--r--   0        0        0    30476 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/tests/data/sentinel-1-rtc-pc.json
+-rw-r--r--   0        0        0    98846 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/tests/data/sentinel-2-l2a-pc.json
+-rw-r--r--   0        0        0    43820 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/tests/data/us-census-pc.json
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/LICENSE
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/README.md
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 stac_geoparquet-0.5.1/PKG-INFO
```

### Comparing `stac_geoparquet-0.5.0/setup.cfg` & `stac_geoparquet-0.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/.github/workflows/continuous-integration.yml` & `stac_geoparquet-0.5.1/.github/workflows/continuous-integration.yml`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/.github/workflows/publish.yml` & `stac_geoparquet-0.5.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/spec/stac-geoparquet-spec.md` & `stac_geoparquet-0.5.1/spec/stac-geoparquet-spec.md`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/stac_geoparquet/cli.py` & `stac_geoparquet-0.5.1/stac_geoparquet/cli.py`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/stac_geoparquet/from_arrow.py` & `stac_geoparquet-0.5.1/stac_geoparquet/arrow/_from_arrow.py`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/stac_geoparquet/pc_runner.py` & `stac_geoparquet-0.5.1/stac_geoparquet/pc_runner.py`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/stac_geoparquet/pgstac_reader.py` & `stac_geoparquet-0.5.1/stac_geoparquet/pgstac_reader.py`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/stac_geoparquet/stac_geoparquet.py` & `stac_geoparquet-0.5.1/stac_geoparquet/stac_geoparquet.py`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/stac_geoparquet/to_arrow.py` & `stac_geoparquet-0.5.1/stac_geoparquet/arrow/_to_arrow.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,15 @@
 
         pyarrow_chunk = pa.array(parsed_chunk)
         chunks.append(pyarrow_chunk)
 
     return pa.chunked_array(chunks)
 
 
-def is_bbox_3d(bbox_col: pa.ChunkedArray) -> bool:
+def _is_bbox_3d(bbox_col: pa.ChunkedArray) -> bool:
     """Infer whether the bounding box column represents 2d or 3d bounding boxes."""
     offsets_set = set()
     for chunk in bbox_col.chunks:
         offsets = chunk.offsets.to_numpy()
         offsets_set.update(np.unique(offsets[1:] - offsets[:-1]))
 
     if len(offsets_set) > 1:
@@ -272,15 +272,15 @@
             possible to minimize file size.
 
     Returns:
         New table
     """
     bbox_col_idx = table.schema.get_field_index("bbox")
     bbox_col = table.column(bbox_col_idx)
-    bbox_3d = is_bbox_3d(bbox_col)
+    bbox_3d = _is_bbox_3d(bbox_col)
 
     new_chunks = []
     for chunk in bbox_col.chunks:
         assert (
             pa.types.is_list(chunk.type)
             or pa.types.is_large_list(chunk.type)
             or pa.types.is_fixed_size_list(chunk.type)
```

### Comparing `stac_geoparquet-0.5.0/stac_geoparquet/to_parquet.py` & `stac_geoparquet-0.5.1/stac_geoparquet/arrow/_to_parquet.py`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/stac_geoparquet/utils.py` & `stac_geoparquet-0.5.1/stac_geoparquet/utils.py`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/tests/base_sentinel2_l2a.json` & `stac_geoparquet-0.5.1/tests/base_sentinel2_l2a.json`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/tests/record_sentinel2_l2a.json` & `stac_geoparquet-0.5.1/tests/record_sentinel2_l2a.json`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/tests/sentinel-2-item.json` & `stac_geoparquet-0.5.1/tests/sentinel-2-item.json`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/tests/test_arrow.py` & `stac_geoparquet-0.5.1/tests/test_arrow.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 import math
 from pathlib import Path
 from typing import Any, Dict, Sequence, Union
 
 import pytest
 from ciso8601 import parse_rfc3339
 
-from stac_geoparquet.from_arrow import stac_table_to_items
-from stac_geoparquet.to_arrow import parse_stac_items_to_arrow
+from stac_geoparquet.arrow import parse_stac_items_to_arrow, stac_table_to_items
 
 HERE = Path(__file__).parent
 
 JsonValue = Union[list, tuple, int, float, dict, str, bool, None]
 
 
 def assert_json_value_equal(
@@ -205,7 +204,27 @@
         assert_json_value_equal(result, expected, precision=0.001)
 
     table = parse_stac_items_to_arrow(items, downcast=False)
     items_result = list(stac_table_to_items(table))
 
     for result, expected in zip(items_result, items):
         assert_json_value_equal(result, expected, precision=0)
+
+
+def test_to_arrow_deprecated():
+    with pytest.warns(FutureWarning):
+        import stac_geoparquet.to_arrow
+    stac_geoparquet.to_arrow.parse_stac_items_to_arrow
+
+
+def test_to_parquet_deprecated():
+    with pytest.warns(FutureWarning):
+        import stac_geoparquet.to_parquet
+
+    stac_geoparquet.to_parquet.to_parquet
+
+
+def test_from_arrow_deprecated():
+    with pytest.warns(FutureWarning):
+        import stac_geoparquet.from_arrow
+
+    stac_geoparquet.from_arrow.stac_table_to_items
```

### Comparing `stac_geoparquet-0.5.0/tests/test_pgstac_reader.py` & `stac_geoparquet-0.5.1/tests/test_pgstac_reader.py`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/tests/test_stac_geoparquet.py` & `stac_geoparquet-0.5.1/tests/test_stac_geoparquet.py`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/tests/test_to_dict.py` & `stac_geoparquet-0.5.1/tests/test_to_dict.py`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/tests/data/3dep-lidar-copc-pc.json` & `stac_geoparquet-0.5.1/tests/data/3dep-lidar-copc-pc.json`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/tests/data/3dep-lidar-dsm-pc.json` & `stac_geoparquet-0.5.1/tests/data/3dep-lidar-dsm-pc.json`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/tests/data/cop-dem-glo-30-pc.json` & `stac_geoparquet-0.5.1/tests/data/cop-dem-glo-30-pc.json`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/tests/data/download.py` & `stac_geoparquet-0.5.1/tests/data/download.py`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/tests/data/io-lulc-annual-v02-pc.json` & `stac_geoparquet-0.5.1/tests/data/io-lulc-annual-v02-pc.json`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/tests/data/io-lulc-pc.json` & `stac_geoparquet-0.5.1/tests/data/io-lulc-pc.json`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/tests/data/landsat-c2-l1-pc.json` & `stac_geoparquet-0.5.1/tests/data/landsat-c2-l1-pc.json`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/tests/data/landsat-c2-l2-pc.json` & `stac_geoparquet-0.5.1/tests/data/landsat-c2-l2-pc.json`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/tests/data/naip-pc.json` & `stac_geoparquet-0.5.1/tests/data/naip-pc.json`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/tests/data/naip.parquet` & `stac_geoparquet-0.5.1/tests/data/naip.parquet`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/tests/data/planet-nicfi-analytic-pc.json` & `stac_geoparquet-0.5.1/tests/data/planet-nicfi-analytic-pc.json`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/tests/data/sentinel-1-rtc-pc.json` & `stac_geoparquet-0.5.1/tests/data/sentinel-1-rtc-pc.json`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/tests/data/sentinel-2-l2a-pc.json` & `stac_geoparquet-0.5.1/tests/data/sentinel-2-l2a-pc.json`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/tests/data/us-census-pc.json` & `stac_geoparquet-0.5.1/tests/data/us-census-pc.json`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/LICENSE` & `stac_geoparquet-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/pyproject.toml` & `stac_geoparquet-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.5.0/PKG-INFO` & `stac_geoparquet-0.5.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: stac_geoparquet
-Version: 0.5.0
+Version: 0.5.1
 Dynamic: Summary
 Project-URL: Home, https://github.com/stac-utils/stac-geoparquet
 Author-email: Tom Augspurger <taugspurger@microsoft.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2022 Tom Augspurger
         
@@ -69,48 +69,36 @@
 
 ## Purpose
 
 This library helps convert [STAC Items](https://github.com/radiantearth/stac-spec/blob/master/overview.md#item-overview) to [GeoParquet](https://github.com/opengeospatial/geoparquet). While STAC Items are commonly distributed as individual JSON files on object storage or through a [STAC API](https://github.com/radiantearth/stac-api-spec), STAC GeoParquet allows users to access a large number of STAC items in bulk without making repeated HTTP requests.
 
 ## Usage
 
-`stac_geoparquet.to_dataframe` does it all. You give it a list of (STAC Item) dictionaries. It just converts them to a `geopandas.GeoDataFrame`, which can be written to parquet with `.to_parquet`.
-
-```python
->>> import requests
->>> import stac_geoparquet
->>> item = requests.get("https://planetarycomputer.microsoft.com/api/stac/v1/collections/naip/items/ia_m_4209150_sw_15_060_20190828_20191105").json()
->>> df = stac_geoparquet.to_geodataframe([item])
->>> df.to_parquet("naip.parquet")
-```
+Use `stac_geoparquet.to_arrow.stac_items_to_arrow` and
+`stac_geoparquet.from_arrow.stac_table_to_items` to convert between STAC items
+and Arrow tables. Arrow Tables of STAC items can be written to parquet with
+`stac_geoparquet.to_parquet.to_parquet`.
 
 Note that `stac_geoparquet` lifts the keys in the item `properties` up to the top level of the DataFrame, similar to `geopandas.GeoDataFrame.from_features`.
 
 ```python
->>> list(df.columns)
-['type',
- 'stac_version',
- 'stac_extensions',
- 'id',
- 'geometry',
- 'bbox',
- 'links',
- 'assets',
- 'collection',
- 'gsd',
- 'datetime',
- 'naip:year',
- 'proj:bbox',
- 'proj:epsg',
- 'naip:state',
- 'proj:shape',
- 'proj:transform']
+>>> import requests
+>>> import stac_geoparquet.arrow
+>>> import pyarrow.parquet
+
+>>> items = requests.get(
+...     "https://planetarycomputer.microsoft.com/api/stac/v1/collections/sentinel-2-l2a/items"
+... ).json()["features"]
+>>> table = stac_geoparquet.arrow.parse_stac_items_to_arrow(items)
+>>> stac_geoparquet.arrow.to_parquet(table, "items.parquet")
+>>> table2 = pyarrow.parquet.read_table("items.parquet")
+>>> items2 = list(stac_geoparquet.arrow.stac_table_to_items(table2))
 ```
 
-We also provide `stac_geoparquet.to_dict` and `stac_geoparquet.to_item_collection` helpers that can be used to convert from DataFrames back to the original STAC items.
+See the [specification](./spec/stac-geoparquet-spec.md) for details on the output stac-geoparquet dataset.
 
 ## pgstac integration
 
 `stac_geoparquet.pgstac_reader` has some helpers for working with items coming from a `pgstac.items` table. It takes care of
 
 - Rehydrating the dehydrated items
 - Partitioning by time
```

