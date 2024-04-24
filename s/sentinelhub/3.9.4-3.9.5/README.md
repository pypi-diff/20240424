# Comparing `tmp/sentinelhub-3.9.4.tar.gz` & `tmp/sentinelhub-3.9.5.tar.gz`

## Comparing `sentinelhub-3.9.4.tar` & `sentinelhub-3.9.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0   768447 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/.utmzones.geojson
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/__init__.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/_version.py
--rw-r--r--   0        0        0    31885 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/areas.py
--rw-r--r--   0        0        0    12857 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/base.py
--rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/commands.py
--rw-r--r--   0        0        0    10166 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/config.py
--rw-r--r--   0        0        0    13528 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/constants.py
--rw-r--r--   0        0        0    24305 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/data_collections.py
--rw-r--r--   0        0        0    11310 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/data_collections_bands.py
--rw-r--r--   0        0        0     7572 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/data_utils.py
--rw-r--r--   0        0        0     6692 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/decoding.py
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/evalscript.py
--rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/exceptions.py
--rw-r--r--   0        0        0     8485 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/geo_utils.py
--rw-r--r--   0        0        0    23000 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/geometry.py
--rw-r--r--   0        0        0     5360 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/io_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/py.typed
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/testing_utils.py
--rw-r--r--   0        0        0     8029 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/time_utils.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/types.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/api/__init__.py
--rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/api/base.py
--rw-r--r--   0        0        0     9526 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/api/base_request.py
--rw-r--r--   0        0        0    12179 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/api/byoc.py
--rw-r--r--   0        0        0    13966 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/api/catalog.py
--rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/api/fis.py
--rw-r--r--   0        0        0    30244 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/api/ogc.py
--rw-r--r--   0        0        0     7706 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/api/opensearch.py
--rw-r--r--   0        0        0    13617 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/api/process.py
--rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/api/statistical.py
--rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/api/utils.py
--rw-r--r--   0        0        0     7604 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/api/wfs.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/api/batch/__init__.py
--rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/api/batch/base.py
--rw-r--r--   0        0        0    24249 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/api/batch/process.py
--rw-r--r--   0        0        0     8156 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/api/batch/statistical.py
--rw-r--r--   0        0        0    10767 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/api/batch/utils.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/aws/__init__.py
--rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/aws/batch.py
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/aws/client.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/aws/commands.py
--rw-r--r--   0        0        0     6428 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/aws/constants.py
--rw-r--r--   0        0        0    30230 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/aws/data.py
--rw-r--r--   0        0        0    18453 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/aws/data_safe.py
--rw-r--r--   0        0        0    10989 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/aws/request.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/download/__init__.py
--rw-r--r--   0        0        0    11587 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/download/client.py
--rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/download/handlers.py
--rw-r--r--   0        0        0    10054 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/download/models.py
--rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/download/rate_limit.py
--rw-r--r--   0        0        0     8799 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/download/sentinelhub_client.py
--rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/download/sentinelhub_statistical_client.py
--rw-r--r--   0        0        0    14615 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/download/session.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/geopedia/__init__.py
--rw-r--r--   0        0        0    16370 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/geopedia/core.py
--rw-r--r--   0        0        0     6618 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/sentinelhub/geopedia/request.py
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/LICENSE.md
--rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/README.md
--rw-r--r--   0        0        0     6614 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/pyproject.toml
--rw-r--r--   0        0        0    10197 2020-02-02 00:00:00.000000 sentinelhub-3.9.4/PKG-INFO
+-rw-r--r--   0        0        0   768447 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/.utmzones.geojson
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/__init__.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/_version.py
+-rw-r--r--   0        0        0    31885 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/areas.py
+-rw-r--r--   0        0        0    12857 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/base.py
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/commands.py
+-rw-r--r--   0        0        0    10166 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/config.py
+-rw-r--r--   0        0        0    13528 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/constants.py
+-rw-r--r--   0        0        0    24305 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/data_collections.py
+-rw-r--r--   0        0        0    11310 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/data_collections_bands.py
+-rw-r--r--   0        0        0     7572 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/data_utils.py
+-rw-r--r--   0        0        0     6692 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/decoding.py
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/evalscript.py
+-rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/exceptions.py
+-rw-r--r--   0        0        0     8485 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/geo_utils.py
+-rw-r--r--   0        0        0    23000 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/geometry.py
+-rw-r--r--   0        0        0     5360 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/io_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/py.typed
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/testing_utils.py
+-rw-r--r--   0        0        0     8029 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/time_utils.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/types.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/api/__init__.py
+-rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/api/base.py
+-rw-r--r--   0        0        0     9526 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/api/base_request.py
+-rw-r--r--   0        0        0    12179 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/api/byoc.py
+-rw-r--r--   0        0        0    13966 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/api/catalog.py
+-rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/api/fis.py
+-rw-r--r--   0        0        0    30244 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/api/ogc.py
+-rw-r--r--   0        0        0     7706 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/api/opensearch.py
+-rw-r--r--   0        0        0    13617 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/api/process.py
+-rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/api/statistical.py
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/api/utils.py
+-rw-r--r--   0        0        0     7604 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/api/wfs.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/api/batch/__init__.py
+-rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/api/batch/base.py
+-rw-r--r--   0        0        0    24249 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/api/batch/process.py
+-rw-r--r--   0        0        0     8156 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/api/batch/statistical.py
+-rw-r--r--   0        0        0    10767 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/api/batch/utils.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/aws/__init__.py
+-rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/aws/batch.py
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/aws/client.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/aws/commands.py
+-rw-r--r--   0        0        0     6428 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/aws/constants.py
+-rw-r--r--   0        0        0    30230 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/aws/data.py
+-rw-r--r--   0        0        0    18453 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/aws/data_safe.py
+-rw-r--r--   0        0        0    10989 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/aws/request.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/download/__init__.py
+-rw-r--r--   0        0        0    11587 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/download/client.py
+-rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/download/handlers.py
+-rw-r--r--   0        0        0    10054 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/download/models.py
+-rw-r--r--   0        0        0     5248 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/download/rate_limit.py
+-rw-r--r--   0        0        0     9131 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/download/sentinelhub_client.py
+-rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/download/sentinelhub_statistical_client.py
+-rw-r--r--   0        0        0    14615 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/download/session.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/geopedia/__init__.py
+-rw-r--r--   0        0        0    16370 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/geopedia/core.py
+-rw-r--r--   0        0        0     6618 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/sentinelhub/geopedia/request.py
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/LICENSE.md
+-rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/README.md
+-rw-r--r--   0        0        0     6621 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/pyproject.toml
+-rw-r--r--   0        0        0    10204 2020-02-02 00:00:00.000000 sentinelhub-3.9.5/PKG-INFO
```

### Comparing `sentinelhub-3.9.4/sentinelhub/.utmzones.geojson` & `sentinelhub-3.9.5/sentinelhub/.utmzones.geojson`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/__init__.py` & `sentinelhub-3.9.5/sentinelhub/__init__.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/areas.py` & `sentinelhub-3.9.5/sentinelhub/areas.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/base.py` & `sentinelhub-3.9.5/sentinelhub/base.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/commands.py` & `sentinelhub-3.9.5/sentinelhub/commands.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/config.py` & `sentinelhub-3.9.5/sentinelhub/config.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/constants.py` & `sentinelhub-3.9.5/sentinelhub/constants.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/data_collections.py` & `sentinelhub-3.9.5/sentinelhub/data_collections.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/data_collections_bands.py` & `sentinelhub-3.9.5/sentinelhub/data_collections_bands.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/data_utils.py` & `sentinelhub-3.9.5/sentinelhub/data_utils.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/decoding.py` & `sentinelhub-3.9.5/sentinelhub/decoding.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/evalscript.py` & `sentinelhub-3.9.5/sentinelhub/evalscript.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/exceptions.py` & `sentinelhub-3.9.5/sentinelhub/exceptions.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/geo_utils.py` & `sentinelhub-3.9.5/sentinelhub/geo_utils.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/geometry.py` & `sentinelhub-3.9.5/sentinelhub/geometry.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/io_utils.py` & `sentinelhub-3.9.5/sentinelhub/io_utils.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/testing_utils.py` & `sentinelhub-3.9.5/sentinelhub/testing_utils.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/time_utils.py` & `sentinelhub-3.9.5/sentinelhub/time_utils.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/api/__init__.py` & `sentinelhub-3.9.5/sentinelhub/api/__init__.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/api/base.py` & `sentinelhub-3.9.5/sentinelhub/api/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,26 +21,28 @@
 from ..types import JsonDict
 from .utils import datetime_config, remove_undefined
 
 
 class SentinelHubService(metaclass=ABCMeta):
     """A base class for classes interacting with different Sentinel Hub APIs"""
 
+    _DEFAULT_RETRY_TIME = 30
+
     def __init__(self, config: Optional[SHConfig] = None):
         """
         :param config: A configuration object with required parameters `sh_client_id`, `sh_client_secret`, and
             `sh_auth_base_url` which is used for authentication and `sh_base_url` which defines the service
             deployment that will be used.
         """
         self.config = config or SHConfig()
 
         base_url = self.config.sh_base_url.rstrip("/")
         self.service_url = self._get_service_url(base_url)
 
-        self.client = SentinelHubDownloadClient(config=self.config)
+        self.client = SentinelHubDownloadClient(config=self.config, default_retry_time=self._DEFAULT_RETRY_TIME)
 
     @staticmethod
     @abstractmethod
     def _get_service_url(base_url: str) -> str:
         """Provides the URL to a specific service"""
```

### Comparing `sentinelhub-3.9.4/sentinelhub/api/base_request.py` & `sentinelhub-3.9.5/sentinelhub/api/base_request.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/api/byoc.py` & `sentinelhub-3.9.5/sentinelhub/api/byoc.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/api/catalog.py` & `sentinelhub-3.9.5/sentinelhub/api/catalog.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/api/fis.py` & `sentinelhub-3.9.5/sentinelhub/api/fis.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/api/ogc.py` & `sentinelhub-3.9.5/sentinelhub/api/ogc.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/api/opensearch.py` & `sentinelhub-3.9.5/sentinelhub/api/opensearch.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/api/process.py` & `sentinelhub-3.9.5/sentinelhub/api/process.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/api/statistical.py` & `sentinelhub-3.9.5/sentinelhub/api/statistical.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/api/utils.py` & `sentinelhub-3.9.5/sentinelhub/api/utils.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/api/wfs.py` & `sentinelhub-3.9.5/sentinelhub/api/wfs.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/api/batch/base.py` & `sentinelhub-3.9.5/sentinelhub/api/batch/base.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/api/batch/process.py` & `sentinelhub-3.9.5/sentinelhub/api/batch/process.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/api/batch/statistical.py` & `sentinelhub-3.9.5/sentinelhub/api/batch/statistical.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/api/batch/utils.py` & `sentinelhub-3.9.5/sentinelhub/api/batch/utils.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/aws/batch.py` & `sentinelhub-3.9.5/sentinelhub/aws/batch.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/aws/client.py` & `sentinelhub-3.9.5/sentinelhub/aws/client.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/aws/commands.py` & `sentinelhub-3.9.5/sentinelhub/aws/commands.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/aws/constants.py` & `sentinelhub-3.9.5/sentinelhub/aws/constants.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/aws/data.py` & `sentinelhub-3.9.5/sentinelhub/aws/data.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/aws/data_safe.py` & `sentinelhub-3.9.5/sentinelhub/aws/data_safe.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/aws/request.py` & `sentinelhub-3.9.5/sentinelhub/aws/request.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/download/client.py` & `sentinelhub-3.9.5/sentinelhub/download/client.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/download/handlers.py` & `sentinelhub-3.9.5/sentinelhub/download/handlers.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/download/models.py` & `sentinelhub-3.9.5/sentinelhub/download/models.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/download/rate_limit.py` & `sentinelhub-3.9.5/sentinelhub/download/rate_limit.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,17 +46,22 @@
         wait_time = max(self.next_download_time - current_time, 0)
 
         if wait_time == 0:
             self.next_download_time = max(current_time + self.wait_time, self.next_download_time)
 
         return wait_time
 
-    def update(self, headers: dict) -> None:
-        """Update the next possible download time if the service has responded with the rate limit"""
-        retry_after: float = int(headers.get(self.RETRY_HEADER, 0))  # can be a string representation of a number
+    def update(self, headers: dict, *, default: float) -> None:
+        """Update the next possible download time if the service has responded with the rate limit.
+
+        :param headers: The headers that (may) contain information about waiting times.
+        :param default: The default waiting time (in milliseconds) when retrying after getting a
+            TOO_MANY_REQUESTS response without appropriate retry headers.
+        """
+        retry_after: float = int(headers.get(self.RETRY_HEADER, default))  # can be a string representation of a number
         retry_after = retry_after / 1000
 
         if retry_after:
             self.next_download_time = max(time.monotonic() + retry_after, self.next_download_time)
 
 
 class PolicyBucket:
```

### Comparing `sentinelhub-3.9.4/sentinelhub/download/sentinelhub_client.py` & `sentinelhub-3.9.5/sentinelhub/download/sentinelhub_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -30,29 +30,32 @@
 
 class SentinelHubDownloadClient(DownloadClient):
     """Download client specifically configured for download from Sentinel Hub service"""
 
     _CACHED_SESSIONS: ClassVar[dict[tuple[str, str], SentinelHubSession]] = {}
     _UNIVERSAL_CACHE_KEY = "universal-user", "default-url"
 
-    def __init__(self, *, session: SentinelHubSession | None = None, **kwargs: Any):
+    def __init__(self, *, session: SentinelHubSession | None = None, default_retry_time: float = 30, **kwargs: Any):
         """
         :param session: If a session object is provided here then this client instance will always use only the
             provided session. Otherwise, it will either use a cached session or create a new session and cache
             it.
+        :param default_retry_time: The default waiting time (in seconds) when retrying after getting a TOO_MANY_REQUESTS
+            response without appropriate retry headers.
         :param kwargs: Optional parameters from DownloadClient
         """
         super().__init__(**kwargs)
 
         if session is not None and not isinstance(session, SentinelHubSession):
             raise ValueError(
                 f"A session parameter has to be an instance of {SentinelHubSession.__name__} or None, but "
                 f"{session} was given"
             )
         self.session = session
+        self.default_retry_time = default_retry_time * 1000  # rescale to milliseconds
 
         self.rate_limit = SentinelHubRateLimit(num_processes=self.config.number_of_download_processes)
         self.lock: Lock | None = None
 
     def download(self, *args: Any, **kwargs: Any) -> Any:
         """The main download method
 
@@ -80,18 +83,17 @@
                     "Sending %s request to %s. Hash of sent request is %s",
                     request.request_type.value,
                     request.url,
                     request.get_hashed_name(),
                 )
                 response = self._do_download(request)
 
-                self._execute_thread_safe(self.rate_limit.update, response.headers)
-
                 if response.status_code == requests.status_codes.codes.TOO_MANY_REQUESTS:
                     warnings.warn("Download rate limit hit", category=SHRateLimitWarning)
+                    self._execute_thread_safe(self.rate_limit.update, response.headers, default=self.default_retry_time)
                     continue
 
                 response.raise_for_status()
 
                 LOGGER.debug("Successful %s request to %s", request.request_type.value, request.url)
                 return DownloadResponse.from_response(response, request)
```

### Comparing `sentinelhub-3.9.4/sentinelhub/download/sentinelhub_statistical_client.py` & `sentinelhub-3.9.5/sentinelhub/download/sentinelhub_statistical_client.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/download/session.py` & `sentinelhub-3.9.5/sentinelhub/download/session.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/geopedia/core.py` & `sentinelhub-3.9.5/sentinelhub/geopedia/core.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/sentinelhub/geopedia/request.py` & `sentinelhub-3.9.5/sentinelhub/geopedia/request.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/.gitignore` & `sentinelhub-3.9.5/.gitignore`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/LICENSE.md` & `sentinelhub-3.9.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/README.md` & `sentinelhub-3.9.5/README.md`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.4/pyproject.toml` & `sentinelhub-3.9.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     "requests>=2.27.0",
     "requests-oauthlib>=1.0.0",
     "shapely",
     "tifffile>=2020.9.30",
     "tomli",
     "tomli_w",
     "tqdm",
-    "typing-extensions",
+    "typing-extensions>=4.5.0",
     "utm",
 ]
 
 [project.optional-dependencies]
 docs = [
     "docutils",
     "ipython",
```

### Comparing `sentinelhub-3.9.4/PKG-INFO` & `sentinelhub-3.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentinelhub
-Version: 3.9.4
+Version: 3.9.5
 Summary: Python API for Sentinel Hub
 Project-URL: Homepage, https://github.com/sentinel-hub/sentinelhub-py
 Project-URL: Documentation, https://sentinelhub-py.readthedocs.io
 Project-URL: Issues, https://github.com/sentinel-hub/sentinelhub-py/issues
 Project-URL: Source, https://github.com/sentinel-hub/sentinelhub-py
 Project-URL: Forum, https://forum.sentinel-hub.com
 Author-email: Sinergise EO research team <eoresearch@sinergise.com>
@@ -58,15 +58,15 @@
 Requires-Dist: requests-oauthlib>=1.0.0
 Requires-Dist: requests>=2.27.0
 Requires-Dist: shapely
 Requires-Dist: tifffile>=2020.9.30
 Requires-Dist: tomli
 Requires-Dist: tomli-w
 Requires-Dist: tqdm
-Requires-Dist: typing-extensions
+Requires-Dist: typing-extensions>=4.5.0
 Requires-Dist: utm
 Provides-Extra: aws
 Requires-Dist: boto3; extra == 'aws'
 Requires-Dist: botocore; extra == 'aws'
 Provides-Extra: dev
 Requires-Dist: basemap; extra == 'dev'
 Requires-Dist: boto3-stubs>=1.20.0; extra == 'dev'
```

