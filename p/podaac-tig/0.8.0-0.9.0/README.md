# Comparing `tmp/podaac_tig-0.8.0.tar.gz` & `tmp/podaac_tig-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podaac_tig-0.8.0.tar", max compression
+gzip compressed data, was "podaac_tig-0.9.0.tar", max compression
```

## Comparing `podaac_tig-0.8.0.tar` & `podaac_tig-0.9.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-12-14 19:02:03.629961 podaac_tig-0.8.0/LICENSE
--rw-r--r--   0        0        0    12747 2023-12-14 19:02:03.629961 podaac_tig-0.8.0/README.md
--rw-r--r--   0        0        0        0 2023-12-14 19:02:03.633961 podaac_tig-0.8.0/podaac/__init__.py
--rw-r--r--   0        0        0        0 2023-12-14 19:02:03.633961 podaac_tig-0.8.0/podaac/lambda_handler/__init__.py
--rw-r--r--   0        0        0     1737 2023-12-14 19:02:03.633961 podaac_tig-0.8.0/podaac/lambda_handler/clean_lambda_handler.py
--rw-r--r--   0        0        0        0 2023-12-14 19:02:03.633961 podaac_tig-0.8.0/podaac/lambda_handler/cumulus_cli_handler/__init__.py
--rw-r--r--   0        0        0     2686 2023-12-14 19:02:03.633961 podaac_tig-0.8.0/podaac/lambda_handler/cumulus_cli_handler/handlers.py
--rw-r--r--   0        0        0    15196 2023-12-14 19:02:03.633961 podaac_tig-0.8.0/podaac/lambda_handler/lambda_handler.py
--rw-r--r--   0        0        0        0 2023-12-14 19:02:03.633961 podaac_tig-0.8.0/podaac/tig/__init__.py
--rw-r--r--   0        0        0      924 2023-12-14 19:02:03.633961 podaac_tig-0.8.0/podaac/tig/cli.py
--rw-r--r--   0        0        0     6416 2023-12-14 19:02:03.633961 podaac_tig-0.8.0/podaac/tig/generate_hitide_config.py
--rwxr-xr-x   0        0        0     3559 2023-12-14 19:02:03.633961 podaac_tig-0.8.0/podaac/tig/generate_thumbnails.sh
--rw-r--r--   0        0        0    31792 2023-12-14 19:02:03.633961 podaac_tig-0.8.0/podaac/tig/tig.py
--rw-r--r--   0        0        0     1131 2023-12-14 19:02:21.825830 podaac_tig-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    14244 1970-01-01 00:00:00.000000 podaac_tig-0.8.0/setup.py
--rw-r--r--   0        0        0    13810 1970-01-01 00:00:00.000000 podaac_tig-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-22 23:11:17.442528 podaac_tig-0.9.0/LICENSE
+-rw-r--r--   0        0        0    13158 2024-02-22 23:11:17.442528 podaac_tig-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2024-02-22 23:11:17.446528 podaac_tig-0.9.0/podaac/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-22 23:11:17.446528 podaac_tig-0.9.0/podaac/lambda_handler/__init__.py
+-rw-r--r--   0        0        0     1737 2024-02-22 23:11:17.446528 podaac_tig-0.9.0/podaac/lambda_handler/clean_lambda_handler.py
+-rw-r--r--   0        0        0        0 2024-02-22 23:11:17.446528 podaac_tig-0.9.0/podaac/lambda_handler/cumulus_cli_handler/__init__.py
+-rw-r--r--   0        0        0     2686 2024-02-22 23:11:17.446528 podaac_tig-0.9.0/podaac/lambda_handler/cumulus_cli_handler/handlers.py
+-rw-r--r--   0        0        0    15196 2024-02-22 23:11:17.446528 podaac_tig-0.9.0/podaac/lambda_handler/lambda_handler.py
+-rw-r--r--   0        0        0        0 2024-02-22 23:11:17.446528 podaac_tig-0.9.0/podaac/tig/__init__.py
+-rw-r--r--   0        0        0      924 2024-02-22 23:11:17.446528 podaac_tig-0.9.0/podaac/tig/cli.py
+-rw-r--r--   0        0        0     7138 2024-02-22 23:11:17.446528 podaac_tig-0.9.0/podaac/tig/generate_hitide_config.py
+-rwxr-xr-x   0        0        0     3559 2024-02-22 23:11:17.446528 podaac_tig-0.9.0/podaac/tig/generate_thumbnails.sh
+-rw-r--r--   0        0        0    35443 2024-02-22 23:11:17.446528 podaac_tig-0.9.0/podaac/tig/tig.py
+-rw-r--r--   0        0        0     1131 2024-02-22 23:11:34.194450 podaac_tig-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    14662 1970-01-01 00:00:00.000000 podaac_tig-0.9.0/setup.py
+-rw-r--r--   0        0        0    14220 1970-01-01 00:00:00.000000 podaac_tig-0.9.0/PKG-INFO
```

### Comparing `podaac_tig-0.8.0/LICENSE` & `podaac_tig-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `podaac_tig-0.8.0/README.md` & `podaac_tig-0.9.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -75,14 +75,22 @@
 datset-id: collection short name 
 include-image-variables: csv file of with image variable names and min max setting for each variable
 longitude: longitude variable include the group if they're in group defaults to longitude
 latitude: latitude variable include the group if they're in a group defaults to latitude
 time: time variable include the group if they're in a group defaults to time
 footprint_strategy: strategy to generate footprint will default to None options should be ["periodic", "linestring", "polar", "swot_linestring", "polarsides", "smap"]
 
+### CSV Columns
+
+variable: name of variable
+min: min value for variable
+max: max value for variable
+palette (optional): the palette to be used for the variable
+fill_missing (optional): if the generated images have missing pixel in images most likely resolution is to big, either lower resolution or we can fill in the pixels with surrounding pixel
+ppd (optional): resolution of the variable, must be an integer
 
 
 ## How to load and use tig module
 Project using tig can include/use the tig as following:
 ```shell script
     module "tig_module" {
       source = "https://cae-artifactory.jpl.nasa.gov/artifactory/general/gov/nasa/podaac/cumulus/tig-terraform/tig-terraform-0.3.0.zip"
```

### Comparing `podaac_tig-0.8.0/podaac/lambda_handler/clean_lambda_handler.py` & `podaac_tig-0.9.0/podaac/lambda_handler/clean_lambda_handler.py`

 * *Files identical despite different names*

### Comparing `podaac_tig-0.8.0/podaac/lambda_handler/cumulus_cli_handler/handlers.py` & `podaac_tig-0.9.0/podaac/lambda_handler/cumulus_cli_handler/handlers.py`

 * *Files identical despite different names*

### Comparing `podaac_tig-0.8.0/podaac/lambda_handler/lambda_handler.py` & `podaac_tig-0.9.0/podaac/lambda_handler/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `podaac_tig-0.8.0/podaac/tig/cli.py` & `podaac_tig-0.9.0/podaac/tig/cli.py`

 * *Files identical despite different names*

### Comparing `podaac_tig-0.8.0/podaac/tig/generate_hitide_config.py` & `podaac_tig-0.9.0/podaac/tig/generate_hitide_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -100,47 +100,65 @@
             'strategy': footprint_strategy,
             't': '0:0,0:*',
             's1': '0:*,0:0',
             'b': '*:*,0:*',
             's2': '0:*,*:*'
         }
 
-    vars_min_max = {}
+    vars_data = {}
     if include_image_variables:
-        vars_min_max = read_min_max_csv(include_image_variables)
+        vars_data = read_min_max_csv(include_image_variables)
 
     with nc.Dataset(granule, 'r') as dataset:  # pylint: disable=no-member
 
         data_var_names = get_variables_with_paths(dataset)
         dataset_config['variables'] = data_var_names
 
         try:
             for data_var in data_var_names:
-                if vars_min_max and data_var in vars_min_max:
+                if vars_data and data_var in vars_data:
                     variable = dataset[data_var]
 
                     units = variable.units if 'units' in variable.ncattrs() else ''
                     long_name = variable.long_name if 'long_name' in variable.ncattrs() else ''
 
-                    if data_var in vars_min_max:
-                        min_max = vars_min_max[data_var]
-                        min_val = float(min_max['min'])
-                        max_val = float(min_max['max'])
+                    palette = 'paletteMedspirationIndexed'
+                    fill_missing = False
+                    ppd = 16
+
+                    if data_var in vars_data:
+                        min_val = float(vars_data[data_var]['min'])
+                        max_val = float(vars_data[data_var]['max'])
+                        palette = vars_data[data_var].get('palette')
+                        fill_missing = vars_data[data_var].get('fill_missing', False)
+                        ppd = vars_data[data_var].get('ppd', 16)
                     else:
                         min_val = variable.valid_min if 'valid_min' in variable.ncattrs() else ''
                         max_val = variable.valid_max if 'valid_max' in variable.ncattrs() else ''
 
-                    dataset_config['imgVariables'].append({
+                    if not palette:
+                        palette = 'paletteMedspirationIndexed'
+
+                    dataset_dict = {
                         'id': data_var,
                         'title': long_name,
                         'units': units,
                         'min': min_val,
                         'max': max_val,
-                        'palette': 'paletteMedspirationIndexed'
-                    })
+                        'palette': palette
+                    }
+
+                    if fill_missing:
+                        fill_missing = fill_missing.lower().strip()
+                        dataset_dict['fill_missing'] = fill_missing == "true"
+
+                    if ppd != 16 and ppd.isdigit():
+                        dataset_dict['ppd'] = int(ppd)
+
+                    dataset_config['imgVariables'].append(dataset_dict)
 
         except Exception as ex:  # pylint: disable=broad-exception-caught
             print(f"Error: Failed on variable {data_var}, exception: " + str(ex))
 
     print(json.dumps(dataset_config, indent=4))
 
     # Specify the file path where you want to save the JSON data
```

### Comparing `podaac_tig-0.8.0/podaac/tig/generate_thumbnails.sh` & `podaac_tig-0.9.0/podaac/tig/generate_thumbnails.sh`

 * *Files identical despite different names*

### Comparing `podaac_tig-0.8.0/podaac/tig/tig.py` & `podaac_tig-0.9.0/podaac/tig/tig.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 ================
 tig.py
 ================
 
 Main module for the Tool for Image Generation (TIG)
 """
-# pylint: disable=invalid-name
+# pylint: disable=invalid-name, too-many-lines
 
 import os
 import logging
 import json
 import matplotlib.colors as col
 import matplotlib.cm as cm
 import matplotlib.pyplot as plt
@@ -205,18 +205,18 @@
         prev = None
         result = False
         for x_val in lons.flatten():
             if prev is None:
                 prev = x_val
                 continue
             if prev > 0 > x_val and prev - x_val > 200:
-                self.logger.debug("prev, x: %s, %s", prev, x_val)
+                self.logger.debug(f"prev, x: {prev}, {x_val}")
                 result = True
             elif x_val > 0 > prev and x_val - prev > 200:
-                self.logger.debug("prev, x: %s, %s", prev, x_val)
+                self.logger.debug(f"prev, x: {prev}, {x_val}")
                 result = True
         return result
 
     def crosses_antimeridian(self, lons):
         """
         Checks if an array of longitudinal values crosses the antimeridian
         Parameters
@@ -395,15 +395,15 @@
             The granule_id of the granule file
         Returns
         -------
         list
             List of output image file locations
         """
 
-        self.logger.info("\nProcessing %s", self.input_file)
+        self.logger.info(f"\nProcessing {self.input_file}")
         output_images = []
         if self.config.get('multi_lon_lat'):
             for group in self.config.get('multi_groups'):
                 output_images += self.generate_images_group(image_format, nearest, world_file, granule_id, group=group)
         else:
             output_images = self.generate_images_group(image_format, nearest, world_file, granule_id, group=None)
         return output_images
@@ -448,15 +448,19 @@
         if not self.crosses_antimeridian(lon_array):
             self.logger.debug("Region does not crosses 180/-180")
             region = (southern, northern, western, eastern)
         else:
             # Image spans antimeridian, wrap it.
             self.logger.debug("Region crosses 180/-180")
             region = (southern, northern, -180, 180)
-        self.logger.info("region: %s", str(region))
+
+        if self.config.get('global_grid', False):
+            region = (-90, 90, -180, 180)
+
+        self.logger.info(f"region: {region}")
         height_deg = region[1] - region[0]
         width_deg = region[3] - region[2]
         self.region = Region(region)
 
         output_dimensions = (int(height_deg * self.ppd), int(width_deg * self.ppd))
         (self.rows, self.cols) = output_dimensions
 
@@ -488,14 +492,96 @@
                                                       override_cols)
             if output_image_file is not None:
                 output_images.append({'image_file': output_image_file, 'variable': var['id'], 'group': group})
 
         self.logger.info("Finished processing variables")
         return output_images
 
+    def get_non_black_neighbor_value(self, img, x, y):
+        """
+        Get the value of a neighboring pixel that isn't black for a given pixel coordinate in an image array.
+
+        Parameters:
+        - img: NumPy array representing the image.
+        - x: Row coordinate of the pixel.
+        - y: Column coordinate of the pixel.
+
+        Returns:
+        - Value of a neighboring pixel that isn't black, or None if all neighbors are black.
+        """
+        height, width = img.shape[:2]
+
+        for i in range(-1, 2):
+            for j in range(-1, 2):
+                # Skip the central pixel itself
+                if i == 0 and j == 0:
+                    continue
+
+                # Calculate neighboring pixel coordinates
+                neighbor_x = x + i
+                neighbor_y = y + j
+
+                # Check if the neighbor is within the image bounds
+                if 0 <= neighbor_x < height and 0 <= neighbor_y < width:
+                    neighbor_value = img[neighbor_x, neighbor_y]
+
+                    # Check if the neighbor is not black (assuming black is 0)
+                    if not np.isnan(neighbor_value):
+                        return neighbor_value
+
+        # Return None if all neighbors are black
+        return None
+
+    def fill_swath_with_neighboring_pixel(self, output_array):
+        """
+        This method fills NaN values in the input image with RGB values from neighboring pixels.
+        The replacement values are chosen randomly from non-missing pixel portions of the image.
+        The probability of selecting a value is inversely proportional to the distance from the NaN position.
+
+        The function uses a helper function `non_nan_neighbors` to check if the neighboring values of a given
+        position are not NaN. It then retrieves x and y coordinates of NaN values with at least one non-NaN neighbor
+        and fills the NaN values in the copy with values from these neighbors.
+
+        Parameters:
+        - output_array (numpy.ndarray): Input image with missing data represented as NaN values.
+
+        Returns:
+        numpy.ndarray: (numpy.ndarray): Output image with missing values surrounded by data filled in.
+        """
+
+        def non_nan_neighbors(arr, x, y):
+            """
+            Check if there is at least one non-NaN neighbor for a given position.
+
+            Parameters:
+            - arr (numpy.ndarray): Input array.
+            - x (int): x-coordinate of the position.
+            - y (int): y-coordinate of the position.
+
+            Returns:
+            bool: True if there is at least one non-NaN neighbor, False otherwise.
+            """
+            neighbors = [
+                (x-1, y), (x+1, y),  # Left and right neighbors
+                (x, y-1), (x, y+1)   # Up and down neighbors
+            ]
+
+            return any(0 <= i < arr.shape[0] and 0 <= j < arr.shape[1] and not np.isnan(arr[i, j]) for i, j in neighbors)
+
+        # Get the indices of NaN values
+        img_with_neighbor_filled = output_array.copy()
+        x_swath, y_swath = zip(*[(x, y) for x, y in zip(*np.where(np.isnan(output_array))) if non_nan_neighbors(output_array, x, y)])
+
+        for index, (x, y) in enumerate(zip(x_swath, y_swath)):  # pylint: disable=unused-variable
+            value = self.get_non_black_neighbor_value(output_array, x, y)
+            if value is not None:
+                img_with_neighbor_filled[x, y] = value
+
+        return img_with_neighbor_filled
+
     def process_variable(self,
                          var,
                          lon_array,
                          lat_array,
                          alpha,
                          image_format='png',
                          nearest=False,
@@ -530,15 +616,15 @@
         -------
         list
             List of output image file locations
         """
 
         # Get variable name
         config_variable = var['id']
-        self.logger.info('variable: %s', config_variable)
+        self.logger.info(f'variable: {config_variable}')
 
         group, _, variable = config_variable.rpartition('/')
         if param_group:
             group = param_group
         local_dataset = xr.open_dataset(self.input_file, group=group, decode_times=False)
 
         # Get variable array and fill value
@@ -550,31 +636,27 @@
             # if no fill value get fill value from configuration if defined
             fill_value = var.get('fill_value')
             if fill_value is None:
                 raise KeyError(f'There is no fill value for variable {variable}') from KeyError
         local_dataset.close()
 
         # Get palette info
-        self.logger.info('palette: %s', var['palette'])
+        self.logger.info(f"palette: {var['palette']}")
         colormap = load_json_palette(self.palette_dir, var['palette'], alpha)
 
         # Set the output location
         group_string = group.strip('/').replace('/', '.').replace(" ", "_")
         file_name = '.'.join(x for x in [granule_id, group_string, variable, image_format] if x)
         output_location = "{}/{}".format(self.output_dir, file_name)
-        if not os.path.exists(self.output_dir):
-            os.makedirs(self.output_dir)
 
-        rows = self.rows
-        cols = self.cols
+        # Create the output directory if it doesn't exist
+        os.makedirs(self.output_dir, exist_ok=True)
 
-        if override_rows:
-            rows = override_rows
-        if override_cols:
-            cols = override_cols
+        rows = override_rows if override_rows else self.rows
+        cols = override_cols if override_cols else self.cols
 
         if var.get('is_swot_expert') and var.get('id') == "ssha_karin_2":
             lon_array, lat_array, var_array = self.get_swot_expert_data(group_string)
 
         try:
             # Generate an array to populate data for image output
             output_vals = self.generate_image_output(var_array,
@@ -583,34 +665,37 @@
                                                      fill_value,
                                                      rows,
                                                      cols,
                                                      nearest)
             output_vals[output_vals == fill_value] = np.nan
             out_array = np.flip(output_vals.flatten().reshape(rows, cols), 0)
 
+            if var.get('fill_missing'):
+                out_array = self.fill_swath_with_neighboring_pixel(out_array)
+
             # Color the image output array and save to a file
             plt.imsave(output_location,
                        out_array,
                        vmin=float(var['min']),
                        vmax=float(var['max']),
                        cmap=colormap,
                        format=image_format)
 
-            self.logger.info("Wrote %s", output_location)
+            self.logger.info(f"Wrote {output_location}")
 
             # Create world file if specified
             if world_file:
                 output_wld = output_location.replace(image_format, 'wld')
                 wld_string = create_world_file((self.region.max_lon-self.region.min_lon)/cols,
                                                (self.region.max_lat-self.region.min_lat)/rows,
                                                self.region.max_lat,
                                                self.region.min_lon)
                 with open(output_wld, 'w') as wld:
                     wld.write(wld_string)
-                self.logger.info("Wrote %s", output_wld)
+                self.logger.info(f"Wrote {output_wld}")
 
         except grids.GridDefinitionError:
             self.logger.warning("Could not grid variable %s", variable.split('/')[-1], exc_info=True)
             raise
         except (ValueError, IndexError):
             self.logger.warning("Could not image variable %s", variable.split('/')[-1], exc_info=True)
             raise
```

### Comparing `podaac_tig-0.8.0/pyproject.toml` & `podaac_tig-0.9.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "podaac-tig"
-version = "0.8.0"
+version = "0.9.0"
 description = "Tool for Image Generation (TIG)"
 authors = ["podaac-tva <podaac-tva@jpl.nasa.gov>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.jpl.nasa.gov/podaac/tig"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules"
@@ -12,32 +12,32 @@
 exclude = ['contrib', 'docs', 'tests']
 packages = [
     { include = "podaac" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.13"
-numpy = "^1.22.3"
-matplotlib = "^3.5.1"
-netCDF4 = "^1.5.8"
-xarray = "^2023.11.0"
-imageio = "^2.16.1"
+numpy = "^1.26.4"
+matplotlib = "^3.8.3"
+netCDF4 = "^1.6.5"
+xarray = "^2024.2.0"
+imageio = "^2.34.0"
 pygeogrids = "^0.5.0"
 cumulus-process = "^1.3.0"
-requests = "^2.27.1"
+requests = "^2.31.0"
 click = "^8.1.7"
-scipy = "^1.11.3"
+scipy = "^1.12.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.4.3"
-flake8 = "^6.1.0"
-pytest-cov = "^3.0.0"
-pylint = "^3.0.2"
-Sphinx = "^4.5.0"
-moto = "^4.2.5"
+pytest = "^8.0.1"
+flake8 = "^7.0.0"
+pytest-cov = "^4.1.0"
+pylint = "^3.0.3"
+Sphinx = "^7.2.6"
+moto = "^4.2.14"
 mock = "^5.1.0"
 
 [tool.poetry.scripts]
 tig = 'podaac.tig.cli:main'
 generate_hitide_config = 'podaac.tig.generate_hitide_config:generate_hitide_config_command'
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `podaac_tig-0.8.0/setup.py` & `podaac_tig-0.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,33 +9,33 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['click>=8.1.7,<9.0.0',
  'cumulus-process>=1.3.0,<2.0.0',
- 'imageio>=2.16.1,<3.0.0',
- 'matplotlib>=3.5.1,<4.0.0',
- 'netCDF4>=1.5.8,<2.0.0',
- 'numpy>=1.22.3,<2.0.0',
+ 'imageio>=2.34.0,<3.0.0',
+ 'matplotlib>=3.8.3,<4.0.0',
+ 'netCDF4>=1.6.5,<2.0.0',
+ 'numpy>=1.26.4,<2.0.0',
  'pygeogrids>=0.5.0,<0.6.0',
- 'requests>=2.27.1,<3.0.0',
- 'scipy>=1.11.3,<2.0.0',
- 'xarray>=2023.11.0,<2024.0.0']
+ 'requests>=2.31.0,<3.0.0',
+ 'scipy>=1.12.0,<2.0.0',
+ 'xarray>=2024.2.0,<2025.0.0']
 
 entry_points = \
 {'console_scripts': ['generate_hitide_config = '
                      'podaac.tig.generate_hitide_config:generate_hitide_config_command',
                      'tig = podaac.tig.cli:main']}
 
 setup_kwargs = {
     'name': 'podaac-tig',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Tool for Image Generation (TIG)',
-    'long_description': '# TIG - Tool for Image Generation\n\n# Table of contents\n\n- [Overview](#overview)\n- [Install poetry](#install-poetry-python-dependency-manager)\n- [Build](#build)\n- [How to load and use tig module](#how-to-load-and-use-tig-module)\n  - [tig Input](#tig-input)\n  - [tig Output](#tig-output)\n- [CLI Commands](#cli-commands)\n\n## Overview\n   tig is built to be used within Cumulus ecosystem.  It is depending on cumulus CMA ([Cumulus Documentation](https://nasa.github.io/cumulus)).\n   Please refer to the [Usage](#usage) section for inputs and outputs. TIG itself is a lambda function which runs on top of CMA as its lambda layer.\n\n## Install poetry (python dependency manager)\n   Install poetry following the directions here: https://python-poetry.org/docs/#installation\n\n   - Be sure to install poetry in an isolated environment from the rest of your system.\n   - Be sure to use with a python version less than 3.12\n\n## Build\n* Jenkins pipeline template is applied to this project.\n* development is based on poetry python environment.  \n  * poetry run pytest   // to run unit test\n  * poetry install      // to install all dependencies defined in toml file\n  * poetry shell        //to enter the poetry shell\n  * poetry build        // to build the wheel\n\n\nUnit Test can be run using the command\n```shell script\npoetry run pytest\n```\n\n## CLI Commands\n- [Generate Thumbnails](#generate-thumbnails)\n- [Generate Config File](#generate-config-file)\n- [Run Tig](#run-tig)\n\n### Generate Thumbnails\nUse cli helper script to generate thumbnails for each collection (NOTE: This automatically generates the config file and runs tig)\n```\nGo to dir `podaac/tig` and look at generate_thumbnails.sh script.  Follow directions at top to setup.\n```\n\n### Generate Config File\nUse cli to create a tig configuration for collections \n```\ngenerate_hitide_config --granule <granule_file> -dataset-id <collection short name> --include-image-variables <csv file image variables> --longitude <lon variable> --latitude <lat variable> --time <time variable> --footprint_strategy <footprint strategy>\n```\n\ngranule: a sample granule file to generate the configuration for\ndatset-id: collection short name \ninclude-image-variables: csv file of with image variable names and min max setting for each variable\nlongitude: longitude variable include the group if they\'re in group defaults to longitude\nlatitude: latitude variable include the group if they\'re in a group defaults to latitude\ntime: time variable include the group if they\'re in a group defaults to time\nfootprint_strategy: strategy to generate footprint will default to None options should be ["periodic", "linestring", "polar", "swot_linestring", "polarsides", "smap"]\n\n### Run Tig\nUse cli to test thumbnail image generation for a granule with configuration file and palettes\n\n```\ntig --input_file <granule> --output_dir <output_dir> --config_file <config_file> --palette_dir <palette_dir>\n```\n\nUse cli to create a tig configuration for collections \n```\ngenerate_hitide_config --granule <granule_file> -dataset-id <collection short name> --include-image-variables <csv file image variables> --longitude <lon variable> --latitude <lat variable> --time <time variable> --footprint_strategy <footprint strategy>\n```\n\ngranule: a sample granule file to generate the configuration for\ndatset-id: collection short name \ninclude-image-variables: csv file of with image variable names and min max setting for each variable\nlongitude: longitude variable include the group if they\'re in group defaults to longitude\nlatitude: latitude variable include the group if they\'re in a group defaults to latitude\ntime: time variable include the group if they\'re in a group defaults to time\nfootprint_strategy: strategy to generate footprint will default to None options should be ["periodic", "linestring", "polar", "swot_linestring", "polarsides", "smap"]\n\n\n\n## How to load and use tig module\nProject using tig can include/use the tig as following:\n```shell script\n    module "tig_module" {\n      source = "https://cae-artifactory.jpl.nasa.gov/artifactory/general/gov/nasa/podaac/cumulus/tig-terraform/tig-terraform-0.3.0.zip"\n      // Lambda variables\n      prefix = var.prefix\n      image = var.tig_image\n      role = module.cumulus.lambda_processing_role_arn\n      cmr_environment = var.cmr_environment\n      subnet_ids = var.subnet_ids\n      security_group_ids = [aws_security_group.no_ingress_all_egress.id]\n      task_logs_retention_in_days = var.task_logs_retention_in_days\n      config_url = "https://hitide.podaac.earthdatacloud.nasa.gov/dataset-configs"\n      palette_url = "https://hitide.podaac.earthdatacloud.nasa.gov/palettes"\n      memory_size = var.tig_memory_size\n}\n\n```\nand the module input variables explained as below.\n\n| field name | type | default | values | description\n| ---------- | ---- | ------- | ------ | -----------\n| prefix | string | (required) | | A prefix string of lambda function. Ex. prefix = "sample" , created lambda : sample-tig\n| region | string | (required) | | AWS region where tig lambda is running upon.  Ex. us-west-2\n| cmr_environment | string | (required) | | dev, sit, ops\n| config_bucket | string | (required) | | bucket where dataset config resides\n| config_dir | string | (required) | | directory where dataset config file resides. dataset-config file follows the collection_shortname.cfg pattern. Ex. MODIS_A-JPL-L2P-v2019.0.cfg\n| tig_output_bucket | string | (required) | | bucket where tig file is created and written\n| tig_output_dir | string | (required) | | output directory of created tig(fp) file. file will be created as s3://tig_output_bucket/tig_output_dir/collection_short_name/granule_id.png. ex. s3://my-cumulus-internaldataset-tig/ MODIS_A-JPL-L2P-v2019.0/20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0.png\n| lambda_role | string | (required) | | aws user role to run tig lambda\n| layers | list(string) | (required) | | list of layers\' arn where tig runs upon.\n| security_group_ids | list(string) | (required) | | security group ids\n| subnet_ids | list(string) | (required) | | subnet ids where tig runs within\n|config_url | string | | | the url of where to retrieve configurations\n|palette_url | string | | | the url of where to retrieve palettes\n\nECS input variables optional\n\n| field name | type | default | values | description\n| ---------- | ---- | ------- | ------ | -----------\n|tig_ecs | bool | false | | boolean to deploy ecs task\n|cluster_arn | string | | | cumulus cluster arn\n|desired_count | number | 1 | | number of ecs tig task to run\n|log_destination_arn | string | | | A shared AWS:Log:Destination that receives logs in log_groups\n|ecs_cpu | number | 700 | |cpu unit to allocate to a tig task\n|ecs_memory_reservation | number | 1024 | | memory unit to allocate to tig task\n\n\nFargate input variables optional\n\n| field name | type | default | values | description\n| ---------- | ---- | ------- | ------ | -----------\n|tig_fargate | bool | false | | boolean to deploy fargate task\n|fargate_memory | number | 2048 | | amount of memory to allocate for a single fargate task\n|fargate_cpu | number | 1024 | | amount of cpu to allocate for a single fargate task\n|fargate_desired_count | number | 1 | | desired count of how many fargate task\n|fargate_min_capacity | number | 1 | | minimum number of fargate task when scaling\n|fargate_max_capacity | number | 1 | | maximum number of fargate task when scaling\n|scale_dimensions | map(string) | null | | cloudwatch dimensions to scale on\n|scale_up_cooldown | number | 60 | | seconds before able to scaling up again\n|scale_down_cooldown | number | 120 | | seconds before able to scaling down again\n|comparison_operator_scale_up | string | GreaterThanOrEqualToThreshold | | The arithmetic operation to use when comparing the specified Statistic and Threshold\n|evaluation_periods_scale_up | number | 1 | | The number of periods over which data is compared to the specified threshold\n|metric_name_scale_up | string | CPUUtilization | | name of the metric\n|namespace_scale_up | string | AWS/ECS | | namespace for the alarm\'s associated metric\n|period_scale_up | number | 60 | | period in seconds over which the specified statistic is applied\n|statistic_scale_up | string | Average | | statistic to apply to the metric\n|threshold_scale_up | number | 50 | | threshold for statistic to compare against to trigger step\n|scale_up_step_adjustment | list | | | step adjustment to make when scaling up fargate\n|comparison_operator_scale_down | string \n|evaluation_periods_scale_down | number | 1 | | The number of periods over which data is compared to the specified threshold\n|metric_name_scale_down | string | CPUUtilization | | name of the metric\n|namespace_scale_down | string | AWS/ECS | | namespace for the alarm\'s associated metric\n|period_scale_down | number | 60 | | period in seconds over which the specified statistic is applied\n|statistic_scale_down | string | Average | | statistic to apply to the metric\n|threshold_scale_down | number | 50 | | threshold for statistic to compare against to trigger step\n|scale_down_step_adjustment | list | | | step adjustment to make when scaling down fargate\n|fargate_iam_role | string | | | iam arn role for fargate\n\nmodule output variables\n\n| field name | type | default | values | description\n| ---------- | ---- | ------- | ------ | -----------\n| tig_function_name | string | (required) | | The name of deployed tig lambda function\n| tig_task_arn | string | (required) | | tig lambda aws arn\n\n### tig Input\n   Cumulus message with granules payload.  Example below\n```json\n{\n  "granules": [\n    {\n      "files": [\n        {\n          "filename": "s3://bucket/file/with/checksum.dat",\n          "checksumType": "md5",\n          "checksum": "asdfdsa"\n        },\n        {\n          "filename": "s3://bucket/file/without/checksum.dat",\n        }\n      ]\n    }\n  ]\n}\n```\n\n### tig Output\n   * A tig file will be created under configured tig_output_bucket and tig-output-dir.  filename as granuleId.png. Ex. s3://my-cumulus-internaldataset-tig/ MODIS_A-JPL-L2P-v2019.0/20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0.png\n   * A file object will be appended to the files[] of processed granule. Example:\n```json\n{\n  "granules": [\n    {\n      "granuleId": "20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0",\n      "dataType": "MODIS_A-JPL-L2P-v2019.0",\n      "sync_granule_duration": 2603,\n      "files": [\n        {\n          "bucket": "my-protected",\n          "path": "MODIS_A-JPL-L2P-v2019.0/2020/001",\n          "filename": "s3://my-protected/MODIS_A-JPL-L2P-v2019.0/20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0.nc",\n          "size": 18232098,\n          "name": "20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0.nc",\n          "checksumType": "md5",\n          "checksum": "aa5204f125ae83847b3b80fa2e571b00",\n          "type": "data",\n          "url_path": "{cmrMetadata.CollectionReference.ShortName}",\n          "filepath": "MODIS_A-JPL-L2P-v2019.0/20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0.nc",\n          "duplicate_found": true\n        },\n        {\n          "bucket": "my-public",\n          "path": "MODIS_A-JPL-L2P-v2019.0/2020/001",\n          "filename": "s3://my-public/MODIS_A-JPL-L2P-v2019.0/20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0.nc.md5",\n          "size": 98,\n          "name": "20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0.nc.md5",\n          "type": "metadata",\n          "url_path": "{cmrMetadata.CollectionReference.ShortName}",\n          "filepath": "MODIS_A-JPL-L2P-v2019.0/20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0.nc.md5",\n          "duplicate_found": true\n        },\n        {\n          "bucket": "my-public",\n          "filename": "s3://my-public/MODIS_A-JPL-L2P-v2019.0/20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0.cmr.json",\n          "size": 1617,\n          "name": "20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0.cmr.json",\n          "type": "metadata",\n          "url_path": "{cmrMetadata.CollectionReference.ShortName}",\n          "filepath": "MODIS_A-JPL-L2P-v2019.0/20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0.cmr.json",\n          "etag": "\\"3e5b9259c5ee7eae5fe71467f151498b\\""\n        },\n        {\n          "bucket": "my-internal",\n          "filename": "s3://my-internal/dataset-tig/MODIS_A-JPL-L2P-v2019.0/20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0.png",\n          "filepath": "dataset-tig/MODIS_A-JPL-L2P-v2019.0/20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0.png",\n          "size": 452,\n          "name": "20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0.png",\n          "type": "metadata"\n        }\n      ],\n}\n',
+    'long_description': '# TIG - Tool for Image Generation\n\n# Table of contents\n\n- [Overview](#overview)\n- [Install poetry](#install-poetry-python-dependency-manager)\n- [Build](#build)\n- [How to load and use tig module](#how-to-load-and-use-tig-module)\n  - [tig Input](#tig-input)\n  - [tig Output](#tig-output)\n- [CLI Commands](#cli-commands)\n\n## Overview\n   tig is built to be used within Cumulus ecosystem.  It is depending on cumulus CMA ([Cumulus Documentation](https://nasa.github.io/cumulus)).\n   Please refer to the [Usage](#usage) section for inputs and outputs. TIG itself is a lambda function which runs on top of CMA as its lambda layer.\n\n## Install poetry (python dependency manager)\n   Install poetry following the directions here: https://python-poetry.org/docs/#installation\n\n   - Be sure to install poetry in an isolated environment from the rest of your system.\n   - Be sure to use with a python version less than 3.12\n\n## Build\n* Jenkins pipeline template is applied to this project.\n* development is based on poetry python environment.  \n  * poetry run pytest   // to run unit test\n  * poetry install      // to install all dependencies defined in toml file\n  * poetry shell        //to enter the poetry shell\n  * poetry build        // to build the wheel\n\n\nUnit Test can be run using the command\n```shell script\npoetry run pytest\n```\n\n## CLI Commands\n- [Generate Thumbnails](#generate-thumbnails)\n- [Generate Config File](#generate-config-file)\n- [Run Tig](#run-tig)\n\n### Generate Thumbnails\nUse cli helper script to generate thumbnails for each collection (NOTE: This automatically generates the config file and runs tig)\n```\nGo to dir `podaac/tig` and look at generate_thumbnails.sh script.  Follow directions at top to setup.\n```\n\n### Generate Config File\nUse cli to create a tig configuration for collections \n```\ngenerate_hitide_config --granule <granule_file> -dataset-id <collection short name> --include-image-variables <csv file image variables> --longitude <lon variable> --latitude <lat variable> --time <time variable> --footprint_strategy <footprint strategy>\n```\n\ngranule: a sample granule file to generate the configuration for\ndatset-id: collection short name \ninclude-image-variables: csv file of with image variable names and min max setting for each variable\nlongitude: longitude variable include the group if they\'re in group defaults to longitude\nlatitude: latitude variable include the group if they\'re in a group defaults to latitude\ntime: time variable include the group if they\'re in a group defaults to time\nfootprint_strategy: strategy to generate footprint will default to None options should be ["periodic", "linestring", "polar", "swot_linestring", "polarsides", "smap"]\n\n### Run Tig\nUse cli to test thumbnail image generation for a granule with configuration file and palettes\n\n```\ntig --input_file <granule> --output_dir <output_dir> --config_file <config_file> --palette_dir <palette_dir>\n```\n\nUse cli to create a tig configuration for collections \n```\ngenerate_hitide_config --granule <granule_file> -dataset-id <collection short name> --include-image-variables <csv file image variables> --longitude <lon variable> --latitude <lat variable> --time <time variable> --footprint_strategy <footprint strategy>\n```\n\ngranule: a sample granule file to generate the configuration for\ndatset-id: collection short name \ninclude-image-variables: csv file of with image variable names and min max setting for each variable\nlongitude: longitude variable include the group if they\'re in group defaults to longitude\nlatitude: latitude variable include the group if they\'re in a group defaults to latitude\ntime: time variable include the group if they\'re in a group defaults to time\nfootprint_strategy: strategy to generate footprint will default to None options should be ["periodic", "linestring", "polar", "swot_linestring", "polarsides", "smap"]\n\n### CSV Columns\n\nvariable: name of variable\nmin: min value for variable\nmax: max value for variable\npalette (optional): the palette to be used for the variable\nfill_missing (optional): if the generated images have missing pixel in images most likely resolution is to big, either lower resolution or we can fill in the pixels with surrounding pixel\nppd (optional): resolution of the variable, must be an integer\n\n\n## How to load and use tig module\nProject using tig can include/use the tig as following:\n```shell script\n    module "tig_module" {\n      source = "https://cae-artifactory.jpl.nasa.gov/artifactory/general/gov/nasa/podaac/cumulus/tig-terraform/tig-terraform-0.3.0.zip"\n      // Lambda variables\n      prefix = var.prefix\n      image = var.tig_image\n      role = module.cumulus.lambda_processing_role_arn\n      cmr_environment = var.cmr_environment\n      subnet_ids = var.subnet_ids\n      security_group_ids = [aws_security_group.no_ingress_all_egress.id]\n      task_logs_retention_in_days = var.task_logs_retention_in_days\n      config_url = "https://hitide.podaac.earthdatacloud.nasa.gov/dataset-configs"\n      palette_url = "https://hitide.podaac.earthdatacloud.nasa.gov/palettes"\n      memory_size = var.tig_memory_size\n}\n\n```\nand the module input variables explained as below.\n\n| field name | type | default | values | description\n| ---------- | ---- | ------- | ------ | -----------\n| prefix | string | (required) | | A prefix string of lambda function. Ex. prefix = "sample" , created lambda : sample-tig\n| region | string | (required) | | AWS region where tig lambda is running upon.  Ex. us-west-2\n| cmr_environment | string | (required) | | dev, sit, ops\n| config_bucket | string | (required) | | bucket where dataset config resides\n| config_dir | string | (required) | | directory where dataset config file resides. dataset-config file follows the collection_shortname.cfg pattern. Ex. MODIS_A-JPL-L2P-v2019.0.cfg\n| tig_output_bucket | string | (required) | | bucket where tig file is created and written\n| tig_output_dir | string | (required) | | output directory of created tig(fp) file. file will be created as s3://tig_output_bucket/tig_output_dir/collection_short_name/granule_id.png. ex. s3://my-cumulus-internaldataset-tig/ MODIS_A-JPL-L2P-v2019.0/20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0.png\n| lambda_role | string | (required) | | aws user role to run tig lambda\n| layers | list(string) | (required) | | list of layers\' arn where tig runs upon.\n| security_group_ids | list(string) | (required) | | security group ids\n| subnet_ids | list(string) | (required) | | subnet ids where tig runs within\n|config_url | string | | | the url of where to retrieve configurations\n|palette_url | string | | | the url of where to retrieve palettes\n\nECS input variables optional\n\n| field name | type | default | values | description\n| ---------- | ---- | ------- | ------ | -----------\n|tig_ecs | bool | false | | boolean to deploy ecs task\n|cluster_arn | string | | | cumulus cluster arn\n|desired_count | number | 1 | | number of ecs tig task to run\n|log_destination_arn | string | | | A shared AWS:Log:Destination that receives logs in log_groups\n|ecs_cpu | number | 700 | |cpu unit to allocate to a tig task\n|ecs_memory_reservation | number | 1024 | | memory unit to allocate to tig task\n\n\nFargate input variables optional\n\n| field name | type | default | values | description\n| ---------- | ---- | ------- | ------ | -----------\n|tig_fargate | bool | false | | boolean to deploy fargate task\n|fargate_memory | number | 2048 | | amount of memory to allocate for a single fargate task\n|fargate_cpu | number | 1024 | | amount of cpu to allocate for a single fargate task\n|fargate_desired_count | number | 1 | | desired count of how many fargate task\n|fargate_min_capacity | number | 1 | | minimum number of fargate task when scaling\n|fargate_max_capacity | number | 1 | | maximum number of fargate task when scaling\n|scale_dimensions | map(string) | null | | cloudwatch dimensions to scale on\n|scale_up_cooldown | number | 60 | | seconds before able to scaling up again\n|scale_down_cooldown | number | 120 | | seconds before able to scaling down again\n|comparison_operator_scale_up | string | GreaterThanOrEqualToThreshold | | The arithmetic operation to use when comparing the specified Statistic and Threshold\n|evaluation_periods_scale_up | number | 1 | | The number of periods over which data is compared to the specified threshold\n|metric_name_scale_up | string | CPUUtilization | | name of the metric\n|namespace_scale_up | string | AWS/ECS | | namespace for the alarm\'s associated metric\n|period_scale_up | number | 60 | | period in seconds over which the specified statistic is applied\n|statistic_scale_up | string | Average | | statistic to apply to the metric\n|threshold_scale_up | number | 50 | | threshold for statistic to compare against to trigger step\n|scale_up_step_adjustment | list | | | step adjustment to make when scaling up fargate\n|comparison_operator_scale_down | string \n|evaluation_periods_scale_down | number | 1 | | The number of periods over which data is compared to the specified threshold\n|metric_name_scale_down | string | CPUUtilization | | name of the metric\n|namespace_scale_down | string | AWS/ECS | | namespace for the alarm\'s associated metric\n|period_scale_down | number | 60 | | period in seconds over which the specified statistic is applied\n|statistic_scale_down | string | Average | | statistic to apply to the metric\n|threshold_scale_down | number | 50 | | threshold for statistic to compare against to trigger step\n|scale_down_step_adjustment | list | | | step adjustment to make when scaling down fargate\n|fargate_iam_role | string | | | iam arn role for fargate\n\nmodule output variables\n\n| field name | type | default | values | description\n| ---------- | ---- | ------- | ------ | -----------\n| tig_function_name | string | (required) | | The name of deployed tig lambda function\n| tig_task_arn | string | (required) | | tig lambda aws arn\n\n### tig Input\n   Cumulus message with granules payload.  Example below\n```json\n{\n  "granules": [\n    {\n      "files": [\n        {\n          "filename": "s3://bucket/file/with/checksum.dat",\n          "checksumType": "md5",\n          "checksum": "asdfdsa"\n        },\n        {\n          "filename": "s3://bucket/file/without/checksum.dat",\n        }\n      ]\n    }\n  ]\n}\n```\n\n### tig Output\n   * A tig file will be created under configured tig_output_bucket and tig-output-dir.  filename as granuleId.png. Ex. s3://my-cumulus-internaldataset-tig/ MODIS_A-JPL-L2P-v2019.0/20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0.png\n   * A file object will be appended to the files[] of processed granule. Example:\n```json\n{\n  "granules": [\n    {\n      "granuleId": "20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0",\n      "dataType": "MODIS_A-JPL-L2P-v2019.0",\n      "sync_granule_duration": 2603,\n      "files": [\n        {\n          "bucket": "my-protected",\n          "path": "MODIS_A-JPL-L2P-v2019.0/2020/001",\n          "filename": "s3://my-protected/MODIS_A-JPL-L2P-v2019.0/20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0.nc",\n          "size": 18232098,\n          "name": "20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0.nc",\n          "checksumType": "md5",\n          "checksum": "aa5204f125ae83847b3b80fa2e571b00",\n          "type": "data",\n          "url_path": "{cmrMetadata.CollectionReference.ShortName}",\n          "filepath": "MODIS_A-JPL-L2P-v2019.0/20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0.nc",\n          "duplicate_found": true\n        },\n        {\n          "bucket": "my-public",\n          "path": "MODIS_A-JPL-L2P-v2019.0/2020/001",\n          "filename": "s3://my-public/MODIS_A-JPL-L2P-v2019.0/20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0.nc.md5",\n          "size": 98,\n          "name": "20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0.nc.md5",\n          "type": "metadata",\n          "url_path": "{cmrMetadata.CollectionReference.ShortName}",\n          "filepath": "MODIS_A-JPL-L2P-v2019.0/20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0.nc.md5",\n          "duplicate_found": true\n        },\n        {\n          "bucket": "my-public",\n          "filename": "s3://my-public/MODIS_A-JPL-L2P-v2019.0/20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0.cmr.json",\n          "size": 1617,\n          "name": "20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0.cmr.json",\n          "type": "metadata",\n          "url_path": "{cmrMetadata.CollectionReference.ShortName}",\n          "filepath": "MODIS_A-JPL-L2P-v2019.0/20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0.cmr.json",\n          "etag": "\\"3e5b9259c5ee7eae5fe71467f151498b\\""\n        },\n        {\n          "bucket": "my-internal",\n          "filename": "s3://my-internal/dataset-tig/MODIS_A-JPL-L2P-v2019.0/20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0.png",\n          "filepath": "dataset-tig/MODIS_A-JPL-L2P-v2019.0/20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0.png",\n          "size": 452,\n          "name": "20200101000000-JPL-L2P_GHRSST-SSTskin-MODIS_A-D-v02.0-fv01.0.png",\n          "type": "metadata"\n        }\n      ],\n}\n',
     'author': 'podaac-tva',
     'author_email': 'podaac-tva@jpl.nasa.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.jpl.nasa.gov/podaac/tig',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `podaac_tig-0.8.0/PKG-INFO` & `podaac_tig-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: podaac-tig
-Version: 0.8.0
+Version: 0.9.0
 Summary: Tool for Image Generation (TIG)
 Home-page: https://github.jpl.nasa.gov/podaac/tig
 License: Apache-2.0
 Author: podaac-tva
 Author-email: podaac-tva@jpl.nasa.gov
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: cumulus-process (>=1.3.0,<2.0.0)
-Requires-Dist: imageio (>=2.16.1,<3.0.0)
-Requires-Dist: matplotlib (>=3.5.1,<4.0.0)
-Requires-Dist: netCDF4 (>=1.5.8,<2.0.0)
-Requires-Dist: numpy (>=1.22.3,<2.0.0)
+Requires-Dist: imageio (>=2.34.0,<3.0.0)
+Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
+Requires-Dist: netCDF4 (>=1.6.5,<2.0.0)
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pygeogrids (>=0.5.0,<0.6.0)
-Requires-Dist: requests (>=2.27.1,<3.0.0)
-Requires-Dist: scipy (>=1.11.3,<2.0.0)
-Requires-Dist: xarray (>=2023.11.0,<2024.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: scipy (>=1.12.0,<2.0.0)
+Requires-Dist: xarray (>=2024.2.0,<2025.0.0)
 Project-URL: Repository, https://github.jpl.nasa.gov/podaac/tig
 Description-Content-Type: text/markdown
 
 # TIG - Tool for Image Generation
 
 # Table of contents
 
@@ -102,14 +102,22 @@
 datset-id: collection short name 
 include-image-variables: csv file of with image variable names and min max setting for each variable
 longitude: longitude variable include the group if they're in group defaults to longitude
 latitude: latitude variable include the group if they're in a group defaults to latitude
 time: time variable include the group if they're in a group defaults to time
 footprint_strategy: strategy to generate footprint will default to None options should be ["periodic", "linestring", "polar", "swot_linestring", "polarsides", "smap"]
 
+### CSV Columns
+
+variable: name of variable
+min: min value for variable
+max: max value for variable
+palette (optional): the palette to be used for the variable
+fill_missing (optional): if the generated images have missing pixel in images most likely resolution is to big, either lower resolution or we can fill in the pixels with surrounding pixel
+ppd (optional): resolution of the variable, must be an integer
 
 
 ## How to load and use tig module
 Project using tig can include/use the tig as following:
 ```shell script
     module "tig_module" {
       source = "https://cae-artifactory.jpl.nasa.gov/artifactory/general/gov/nasa/podaac/cumulus/tig-terraform/tig-terraform-0.3.0.zip"
```

