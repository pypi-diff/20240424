# Comparing `tmp/seapopym-0.0.1.3.tar.gz` & `tmp/seapopym-0.0.1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seapopym-0.0.1.3.tar", max compression
+gzip compressed data, was "seapopym-0.0.1.3.1.tar", max compression
```

## Comparing `seapopym-0.0.1.3.tar` & `seapopym-0.0.1.3.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1070 2024-03-11 23:18:12.538968 seapopym-0.0.1.3/LICENSE
--rw-r--r--   0        0        0     1170 2024-04-08 23:04:02.855468 seapopym-0.0.1.3/README.md
--rw-r--r--   0        0        0     1240 2024-04-10 21:47:32.273762 seapopym-0.0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-02 02:55:48.497608 seapopym-0.0.1.3/seapopym/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 02:55:48.497704 seapopym-0.0.1.3/seapopym/configuration/__init__.py
--rw-r--r--   0        0        0     1110 2024-04-09 05:02:49.187954 seapopym-0.0.1.3/seapopym/configuration/base_configuration.py
--rw-r--r--   0        0        0        0 2024-04-02 02:55:48.497941 seapopym-0.0.1.3/seapopym/configuration/no_transport/__init__.py
--rw-r--r--   0        0        0     2144 2024-04-09 05:03:52.135501 seapopym-0.0.1.3/seapopym/configuration/no_transport/configuration.py
--rw-r--r--   0        0        0     7665 2024-04-08 02:54:52.889502 seapopym-0.0.1.3/seapopym/configuration/no_transport/configuration_to_dataset.py
--rw-r--r--   0        0        0     8718 2024-04-10 00:16:49.797960 seapopym-0.0.1.3/seapopym/configuration/no_transport/parameter.py
--rw-r--r--   0        0        0        0 2024-04-08 03:07:38.628025 seapopym-0.0.1.3/seapopym/configuration/parameters/__init__.py
--rw-r--r--   0        0        0     8303 2024-04-10 06:02:33.805896 seapopym-0.0.1.3/seapopym/configuration/parameters/parameter_environment.py
--rw-r--r--   0        0        0     6922 2024-04-10 06:03:03.659858 seapopym-0.0.1.3/seapopym/configuration/parameters/parameter_forcing.py
--rw-r--r--   0        0        0     5664 2024-04-02 02:55:48.499108 seapopym-0.0.1.3/seapopym/configuration/parameters/parameter_functional_group.py
--rw-r--r--   0        0        0        0 2024-04-02 02:55:48.499152 seapopym-0.0.1.3/seapopym/exception/__init__.py
--rw-r--r--   0        0        0     1981 2024-04-02 02:55:48.499367 seapopym-0.0.1.3/seapopym/exception/parameter_exception.py
--rw-r--r--   0        0        0        0 2024-04-02 02:55:48.499420 seapopym-0.0.1.3/seapopym/function/core/__init__.py
--rw-r--r--   0        0        0     3134 2024-04-10 05:43:21.984226 seapopym-0.0.1.3/seapopym/function/core/kernel.py
--rw-r--r--   0        0        0     7161 2024-04-08 03:07:38.628595 seapopym-0.0.1.3/seapopym/function/core/template.py
--rw-r--r--   0        0        0      556 2024-04-08 03:07:38.628847 seapopym-0.0.1.3/seapopym/function/generator/__init__.py
--rw-r--r--   0        0        0     3279 2024-04-08 23:41:33.783430 seapopym-0.0.1.3/seapopym/function/generator/apply_coefficient_to_primary_production.py
--rw-r--r--   0        0        0     2884 2024-04-08 23:42:36.914042 seapopym-0.0.1.3/seapopym/function/generator/average_temperature.py
--rw-r--r--   0        0        0        0 2024-04-02 02:55:48.500744 seapopym-0.0.1.3/seapopym/function/generator/biomass/__init__.py
--rw-r--r--   0        0        0     2266 2024-04-10 05:54:56.523895 seapopym-0.0.1.3/seapopym/function/generator/biomass/biomass.py
--rw-r--r--   0        0        0     1695 2024-04-02 02:55:48.501086 seapopym-0.0.1.3/seapopym/function/generator/biomass/compiled_functions.py
--rw-r--r--   0        0        0     6252 2024-04-08 03:07:38.629846 seapopym-0.0.1.3/seapopym/function/generator/cell_area.py
--rw-r--r--   0        0        0     5285 2024-04-09 05:17:25.721091 seapopym-0.0.1.3/seapopym/function/generator/day_length.py
--rw-r--r--   0        0        0     3729 2024-04-08 03:07:38.630168 seapopym-0.0.1.3/seapopym/function/generator/mask.py
--rw-r--r--   0        0        0     2280 2024-04-08 03:07:38.630364 seapopym-0.0.1.3/seapopym/function/generator/mask_temperature.py
--rw-r--r--   0        0        0     1766 2024-04-08 23:40:17.869043 seapopym-0.0.1.3/seapopym/function/generator/min_temperature.py
--rw-r--r--   0        0        0     2173 2024-04-08 03:07:38.630718 seapopym-0.0.1.3/seapopym/function/generator/mortality_field.py
--rw-r--r--   0        0        0        0 2024-04-02 02:55:48.502336 seapopym-0.0.1.3/seapopym/function/generator/production/__init__.py
--rw-r--r--   0        0        0     7571 2024-04-10 03:59:53.391409 seapopym-0.0.1.3/seapopym/function/generator/production/compiled_functions.py
--rw-r--r--   0        0        0     6580 2024-04-10 05:54:40.556574 seapopym-0.0.1.3/seapopym/function/generator/production/production.py
--rw-r--r--   0        0        0        0 2024-04-02 02:55:48.502858 seapopym-0.0.1.3/seapopym/logging/__init__.py
--rw-r--r--   0        0        0     2079 2024-04-02 02:55:48.503073 seapopym-0.0.1.3/seapopym/logging/custom_logger.py
--rw-r--r--   0        0        0        0 2024-04-02 02:55:48.503115 seapopym-0.0.1.3/seapopym/model/__init__.py
--rw-r--r--   0        0        0     1793 2024-04-08 03:07:38.631293 seapopym-0.0.1.3/seapopym/model/base_model.py
--rw-r--r--   0        0        0     4461 2024-04-10 21:46:19.171146 seapopym-0.0.1.3/seapopym/model/no_transport_model.py
--rw-r--r--   0        0        0        0 2024-04-08 03:07:38.631613 seapopym-0.0.1.3/seapopym/plotter/__init__.py
--rw-r--r--   0        0        0     1138 2024-04-08 03:07:38.631874 seapopym-0.0.1.3/seapopym/plotter/base_functions.py
--rw-r--r--   0        0        0        0 2024-04-02 02:55:48.503531 seapopym-0.0.1.3/seapopym/standard/__init__.py
--rw-r--r--   0        0        0     3707 2024-04-02 02:55:48.503717 seapopym-0.0.1.3/seapopym/standard/attributs.py
--rw-r--r--   0        0        0     2688 2024-04-02 02:55:48.503855 seapopym-0.0.1.3/seapopym/standard/coordinates.py
--rw-r--r--   0        0        0     3251 2024-04-08 03:07:38.632076 seapopym-0.0.1.3/seapopym/standard/labels.py
--rw-r--r--   0        0        0      880 2024-04-08 03:07:38.632268 seapopym-0.0.1.3/seapopym/standard/types.py
--rw-r--r--   0        0        0     2202 2024-04-02 02:55:48.504254 seapopym-0.0.1.3/seapopym/standard/units.py
--rw-r--r--   0        0        0        0 2024-04-04 23:35:32.426610 seapopym-0.0.1.3/seapopym/writer/__init__.py
--rw-r--r--   0        0        0     3666 2024-04-10 03:53:43.521606 seapopym-0.0.1.3/seapopym/writer/base_functions.py
--rw-r--r--   0        0        0     2456 1970-01-01 00:00:00.000000 seapopym-0.0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-11 23:18:12.538968 seapopym-0.0.1.3.1/LICENSE
+-rw-r--r--   0        0        0     1170 2024-04-08 23:04:02.855468 seapopym-0.0.1.3.1/README.md
+-rw-r--r--   0        0        0     1371 2024-04-24 03:16:41.855131 seapopym-0.0.1.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-02 02:55:48.497608 seapopym-0.0.1.3.1/seapopym/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 02:55:48.497704 seapopym-0.0.1.3.1/seapopym/configuration/__init__.py
+-rw-r--r--   0        0        0     1110 2024-04-09 05:02:49.187954 seapopym-0.0.1.3.1/seapopym/configuration/base_configuration.py
+-rw-r--r--   0        0        0        0 2024-04-02 02:55:48.497941 seapopym-0.0.1.3.1/seapopym/configuration/no_transport/__init__.py
+-rw-r--r--   0        0        0     2144 2024-04-09 05:03:52.135501 seapopym-0.0.1.3.1/seapopym/configuration/no_transport/configuration.py
+-rw-r--r--   0        0        0     7665 2024-04-08 02:54:52.889502 seapopym-0.0.1.3.1/seapopym/configuration/no_transport/configuration_to_dataset.py
+-rw-r--r--   0        0        0     8718 2024-04-10 00:16:49.797960 seapopym-0.0.1.3.1/seapopym/configuration/no_transport/parameter.py
+-rw-r--r--   0        0        0        0 2024-04-08 03:07:38.628025 seapopym-0.0.1.3.1/seapopym/configuration/parameters/__init__.py
+-rw-r--r--   0        0        0     8303 2024-04-10 06:02:33.805896 seapopym-0.0.1.3.1/seapopym/configuration/parameters/parameter_environment.py
+-rw-r--r--   0        0        0     6922 2024-04-10 06:03:03.659858 seapopym-0.0.1.3.1/seapopym/configuration/parameters/parameter_forcing.py
+-rw-r--r--   0        0        0     5664 2024-04-02 02:55:48.499108 seapopym-0.0.1.3.1/seapopym/configuration/parameters/parameter_functional_group.py
+-rw-r--r--   0        0        0        0 2024-04-02 02:55:48.499152 seapopym-0.0.1.3.1/seapopym/exception/__init__.py
+-rw-r--r--   0        0        0     1981 2024-04-02 02:55:48.499367 seapopym-0.0.1.3.1/seapopym/exception/parameter_exception.py
+-rw-r--r--   0        0        0        0 2024-04-02 02:55:48.499420 seapopym-0.0.1.3.1/seapopym/function/core/__init__.py
+-rw-r--r--   0        0        0     3134 2024-04-10 05:43:21.984226 seapopym-0.0.1.3.1/seapopym/function/core/kernel.py
+-rw-r--r--   0        0        0     7161 2024-04-08 03:07:38.628595 seapopym-0.0.1.3.1/seapopym/function/core/template.py
+-rw-r--r--   0        0        0      556 2024-04-08 03:07:38.628847 seapopym-0.0.1.3.1/seapopym/function/generator/__init__.py
+-rw-r--r--   0        0        0     3279 2024-04-08 23:41:33.783430 seapopym-0.0.1.3.1/seapopym/function/generator/apply_coefficient_to_primary_production.py
+-rw-r--r--   0        0        0     2884 2024-04-08 23:42:36.914042 seapopym-0.0.1.3.1/seapopym/function/generator/average_temperature.py
+-rw-r--r--   0        0        0        0 2024-04-02 02:55:48.500744 seapopym-0.0.1.3.1/seapopym/function/generator/biomass/__init__.py
+-rw-r--r--   0        0        0     2266 2024-04-10 05:54:56.523895 seapopym-0.0.1.3.1/seapopym/function/generator/biomass/biomass.py
+-rw-r--r--   0        0        0     1695 2024-04-02 02:55:48.501086 seapopym-0.0.1.3.1/seapopym/function/generator/biomass/compiled_functions.py
+-rw-r--r--   0        0        0     6252 2024-04-08 03:07:38.629846 seapopym-0.0.1.3.1/seapopym/function/generator/cell_area.py
+-rw-r--r--   0        0        0     5285 2024-04-09 05:17:25.721091 seapopym-0.0.1.3.1/seapopym/function/generator/day_length.py
+-rw-r--r--   0        0        0     3729 2024-04-08 03:07:38.630168 seapopym-0.0.1.3.1/seapopym/function/generator/mask.py
+-rw-r--r--   0        0        0     2280 2024-04-08 03:07:38.630364 seapopym-0.0.1.3.1/seapopym/function/generator/mask_temperature.py
+-rw-r--r--   0        0        0     1766 2024-04-08 23:40:17.869043 seapopym-0.0.1.3.1/seapopym/function/generator/min_temperature.py
+-rw-r--r--   0        0        0     2173 2024-04-08 03:07:38.630718 seapopym-0.0.1.3.1/seapopym/function/generator/mortality_field.py
+-rw-r--r--   0        0        0        0 2024-04-02 02:55:48.502336 seapopym-0.0.1.3.1/seapopym/function/generator/production/__init__.py
+-rw-r--r--   0        0        0     7571 2024-04-10 03:59:53.391409 seapopym-0.0.1.3.1/seapopym/function/generator/production/compiled_functions.py
+-rw-r--r--   0        0        0     6580 2024-04-10 05:54:40.556574 seapopym-0.0.1.3.1/seapopym/function/generator/production/production.py
+-rw-r--r--   0        0        0        0 2024-04-02 02:55:48.502858 seapopym-0.0.1.3.1/seapopym/logging/__init__.py
+-rw-r--r--   0        0        0     2079 2024-04-02 02:55:48.503073 seapopym-0.0.1.3.1/seapopym/logging/custom_logger.py
+-rw-r--r--   0        0        0        0 2024-04-02 02:55:48.503115 seapopym-0.0.1.3.1/seapopym/model/__init__.py
+-rw-r--r--   0        0        0     1793 2024-04-08 03:07:38.631293 seapopym-0.0.1.3.1/seapopym/model/base_model.py
+-rw-r--r--   0        0        0     4461 2024-04-10 21:46:19.171146 seapopym-0.0.1.3.1/seapopym/model/no_transport_model.py
+-rw-r--r--   0        0        0        0 2024-04-08 03:07:38.631613 seapopym-0.0.1.3.1/seapopym/plotter/__init__.py
+-rw-r--r--   0        0        0     1138 2024-04-08 03:07:38.631874 seapopym-0.0.1.3.1/seapopym/plotter/base_functions.py
+-rw-r--r--   0        0        0        0 2024-04-02 02:55:48.503531 seapopym-0.0.1.3.1/seapopym/standard/__init__.py
+-rw-r--r--   0        0        0     3707 2024-04-02 02:55:48.503717 seapopym-0.0.1.3.1/seapopym/standard/attributs.py
+-rw-r--r--   0        0        0     2688 2024-04-02 02:55:48.503855 seapopym-0.0.1.3.1/seapopym/standard/coordinates.py
+-rw-r--r--   0        0        0     3251 2024-04-08 03:07:38.632076 seapopym-0.0.1.3.1/seapopym/standard/labels.py
+-rw-r--r--   0        0        0      880 2024-04-08 03:07:38.632268 seapopym-0.0.1.3.1/seapopym/standard/types.py
+-rw-r--r--   0        0        0     2202 2024-04-02 02:55:48.504254 seapopym-0.0.1.3.1/seapopym/standard/units.py
+-rw-r--r--   0        0        0        0 2024-04-04 23:35:32.426610 seapopym-0.0.1.3.1/seapopym/writer/__init__.py
+-rw-r--r--   0        0        0     3666 2024-04-10 03:53:43.521606 seapopym-0.0.1.3.1/seapopym/writer/base_functions.py
+-rw-r--r--   0        0        0     2508 1970-01-01 00:00:00.000000 seapopym-0.0.1.3.1/PKG-INFO
```

### Comparing `seapopym-0.0.1.3/LICENSE` & `seapopym-0.0.1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/README.md` & `seapopym-0.0.1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/pyproject.toml` & `seapopym-0.0.1.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 [tool.poetry]
 name = "seapopym"
-version = "0.0.1.3"
+version = "0.0.1.3.1"
 description = "Seapodym is a Python package that provides models to simulate the dynamics of low and mid trophic level marine ecosystems."
 authors = ["Jules Lehodey <lehodey.jules+seapopym@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/Ash12H/Seapopym"
 documentation = "https://seapopym.readthedocs.io/en/latest/"
 classifiers = ["Topic :: Scientific/Engineering :: Oceanography"]
 
 [tool.poetry.urls]
 "Documentation" = "https://seapopym.readthedocs.io/en/latest/"
 "Bug Tracker" = "https://github.com/Ash12H/Seapopym/issues"
 
 [tool.poetry.dependencies]
-python = "^3.12"
+python = ">=3.12,<3.13"
 xarray = "^2024.2.0"
 netcdf4 = "^1.6.5"
 dask = "^2024.2.0"
 distributed = "^2024.2.0"
 bokeh = "^3.3.4"
 matplotlib = "^3.8.3"
 cf-xarray = "^0.9.0"
 pint = "^0.23"
 xgcm = "^0.8.1"
 pint-xarray = "^0.3"
 zarr = "^2.17.0"
 numba = "^0.59.0"
+copernicusmarine = "^1.1.1"
 
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.2.1"
 notebook = "^7.1.0"
 graphviz = "^0.20.1"
 pooch = "^1.8.1"
@@ -39,10 +40,15 @@
 
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^7.2.6"
 nbsphinx = "^0.9.3"
 sphinx-rtd-theme = "^2.0.0"
 
+
+[tool.poetry.group.cloud.dependencies]
+google-cloud-storage = "^2.16.0"
+gcsfs = "^2024.3.1"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `seapopym-0.0.1.3/seapopym/configuration/base_configuration.py` & `seapopym-0.0.1.3.1/seapopym/configuration/base_configuration.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/configuration/no_transport/configuration.py` & `seapopym-0.0.1.3.1/seapopym/configuration/no_transport/configuration.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/configuration/no_transport/configuration_to_dataset.py` & `seapopym-0.0.1.3.1/seapopym/configuration/no_transport/configuration_to_dataset.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/configuration/no_transport/parameter.py` & `seapopym-0.0.1.3.1/seapopym/configuration/no_transport/parameter.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/configuration/parameters/parameter_environment.py` & `seapopym-0.0.1.3.1/seapopym/configuration/parameters/parameter_environment.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/configuration/parameters/parameter_forcing.py` & `seapopym-0.0.1.3.1/seapopym/configuration/parameters/parameter_forcing.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/configuration/parameters/parameter_functional_group.py` & `seapopym-0.0.1.3.1/seapopym/configuration/parameters/parameter_functional_group.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/exception/parameter_exception.py` & `seapopym-0.0.1.3.1/seapopym/exception/parameter_exception.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/function/core/kernel.py` & `seapopym-0.0.1.3.1/seapopym/function/core/kernel.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/function/core/template.py` & `seapopym-0.0.1.3.1/seapopym/function/core/template.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/function/generator/__init__.py` & `seapopym-0.0.1.3.1/seapopym/function/generator/__init__.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/function/generator/apply_coefficient_to_primary_production.py` & `seapopym-0.0.1.3.1/seapopym/function/generator/apply_coefficient_to_primary_production.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/function/generator/average_temperature.py` & `seapopym-0.0.1.3.1/seapopym/function/generator/average_temperature.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/function/generator/biomass/biomass.py` & `seapopym-0.0.1.3.1/seapopym/function/generator/biomass/biomass.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/function/generator/biomass/compiled_functions.py` & `seapopym-0.0.1.3.1/seapopym/function/generator/biomass/compiled_functions.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/function/generator/cell_area.py` & `seapopym-0.0.1.3.1/seapopym/function/generator/cell_area.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/function/generator/day_length.py` & `seapopym-0.0.1.3.1/seapopym/function/generator/day_length.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/function/generator/mask.py` & `seapopym-0.0.1.3.1/seapopym/function/generator/mask.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/function/generator/mask_temperature.py` & `seapopym-0.0.1.3.1/seapopym/function/generator/mask_temperature.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/function/generator/min_temperature.py` & `seapopym-0.0.1.3.1/seapopym/function/generator/min_temperature.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/function/generator/mortality_field.py` & `seapopym-0.0.1.3.1/seapopym/function/generator/mortality_field.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/function/generator/production/compiled_functions.py` & `seapopym-0.0.1.3.1/seapopym/function/generator/production/compiled_functions.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/function/generator/production/production.py` & `seapopym-0.0.1.3.1/seapopym/function/generator/production/production.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/logging/custom_logger.py` & `seapopym-0.0.1.3.1/seapopym/logging/custom_logger.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/model/base_model.py` & `seapopym-0.0.1.3.1/seapopym/model/base_model.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/model/no_transport_model.py` & `seapopym-0.0.1.3.1/seapopym/model/no_transport_model.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/plotter/base_functions.py` & `seapopym-0.0.1.3.1/seapopym/plotter/base_functions.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/standard/attributs.py` & `seapopym-0.0.1.3.1/seapopym/standard/attributs.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/standard/coordinates.py` & `seapopym-0.0.1.3.1/seapopym/standard/coordinates.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/standard/labels.py` & `seapopym-0.0.1.3.1/seapopym/standard/labels.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/standard/types.py` & `seapopym-0.0.1.3.1/seapopym/standard/types.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/standard/units.py` & `seapopym-0.0.1.3.1/seapopym/standard/units.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/seapopym/writer/base_functions.py` & `seapopym-0.0.1.3.1/seapopym/writer/base_functions.py`

 * *Files identical despite different names*

### Comparing `seapopym-0.0.1.3/PKG-INFO` & `seapopym-0.0.1.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: seapopym
-Version: 0.0.1.3
+Version: 0.0.1.3.1
 Summary: Seapodym is a Python package that provides models to simulate the dynamics of low and mid trophic level marine ecosystems.
 Home-page: https://github.com/Ash12H/Seapopym
 License: MIT
 Author: Jules Lehodey
 Author-email: lehodey.jules+seapopym@gmail.com
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.12,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Oceanography
 Requires-Dist: bokeh (>=3.3.4,<4.0.0)
 Requires-Dist: cf-xarray (>=0.9.0,<0.10.0)
+Requires-Dist: copernicusmarine (>=1.1.1,<2.0.0)
 Requires-Dist: dask (>=2024.2.0,<2025.0.0)
 Requires-Dist: distributed (>=2024.2.0,<2025.0.0)
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
 Requires-Dist: netcdf4 (>=1.6.5,<2.0.0)
 Requires-Dist: numba (>=0.59.0,<0.60.0)
 Requires-Dist: pint (>=0.23,<0.24)
 Requires-Dist: pint-xarray (>=0.3,<0.4)
```

