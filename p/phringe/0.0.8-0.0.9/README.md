# Comparing `tmp/phringe-0.0.8.tar.gz` & `tmp/phringe-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phringe-0.0.8.tar", max compression
+gzip compressed data, was "phringe-0.0.9.tar", max compression
```

## Comparing `phringe-0.0.8.tar` & `phringe-0.0.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1072 2024-02-05 12:16:41.447059 phringe-0.0.8/LICENSE
--rw-r--r--   0        0        0       15 2024-02-21 08:55:27.312918 phringe-0.0.8/phringe/__init__.py
--rw-r--r--   0        0        0     1781 2024-02-27 08:06:49.907703 phringe-0.0.8/phringe/__main__.py
--rw-r--r--   0        0        0        0 2024-02-08 08:35:21.257604 phringe-0.0.8/phringe/core/__init__.py
--rw-r--r--   0        0        0        0 2024-02-08 08:35:21.273625 phringe-0.0.8/phringe/core/entities/__init__.py
--rw-r--r--   0        0        0      375 2024-02-08 09:22:44.811062 phringe-0.0.8/phringe/core/entities/base_component.py
--rw-r--r--   0        0        0     5401 2024-02-22 15:40:57.194481 phringe-0.0.8/phringe/core/entities/observation.py
--rw-r--r--   0        0        0        0 2024-02-08 08:35:21.273625 phringe-0.0.8/phringe/core/entities/observatory/__init__.py
--rw-r--r--   0        0        0     6930 2024-02-21 08:47:44.996860 phringe-0.0.8/phringe/core/entities/observatory/array_configuration.py
--rw-r--r--   0        0        0     5340 2024-02-08 09:08:54.823102 phringe-0.0.8/phringe/core/entities/observatory/beam_combination_scheme.py
--rw-r--r--   0        0        0    18069 2024-02-22 15:28:57.787162 phringe-0.0.8/phringe/core/entities/observatory/observatory.py
--rw-r--r--   0        0        0        0 2024-02-08 08:35:21.289407 phringe-0.0.8/phringe/core/entities/photon_sources/__init__.py
--rw-r--r--   0        0        0     3344 2024-02-26 12:28:15.271437 phringe-0.0.8/phringe/core/entities/photon_sources/base_photon_source.py
--rw-r--r--   0        0        0     5423 2024-02-26 12:28:15.276172 phringe-0.0.8/phringe/core/entities/photon_sources/exozodi.py
--rw-r--r--   0        0        0     4024 2024-02-26 12:35:39.120595 phringe-0.0.8/phringe/core/entities/photon_sources/local_zodi.py
--rw-r--r--   0        0        0    13870 2024-02-26 12:28:41.207998 phringe-0.0.8/phringe/core/entities/photon_sources/planet.py
--rw-r--r--   0        0        0     7170 2024-02-26 12:28:50.055568 phringe-0.0.8/phringe/core/entities/photon_sources/star.py
--rw-r--r--   0        0        0     5989 2024-02-27 08:32:05.732277 phringe-0.0.8/phringe/core/entities/scene.py
--rw-r--r--   0        0        0     5172 2024-02-23 08:35:18.865732 phringe-0.0.8/phringe/core/entities/settings.py
--rw-r--r--   0        0        0        0 2024-02-05 15:27:51.892809 phringe-0.0.8/phringe/core/processing/__init__.py
--rw-r--r--   0        0        0    19923 2024-02-26 12:21:22.198446 phringe-0.0.8/phringe/core/processing/data_generator.py
--rw-r--r--   0        0        0        0 2024-02-08 08:35:21.243748 phringe-0.0.8/phringe/io/__init__.py
--rw-r--r--   0        0        0      878 2024-02-26 12:34:13.955489 phringe-0.0.8/phringe/io/fits_writer.py
--rw-r--r--   0        0        0      623 2024-02-21 10:20:11.841601 phringe-0.0.8/phringe/io/txt_reader.py
--rw-r--r--   0        0        0     1344 2024-02-23 13:01:58.721175 phringe-0.0.8/phringe/io/utils.py
--rw-r--r--   0        0        0     1033 2024-02-08 09:36:48.784816 phringe-0.0.8/phringe/io/validators.py
--rw-r--r--   0        0        0      783 2024-02-20 15:46:59.570736 phringe-0.0.8/phringe/io/yaml_handler.py
--rw-r--r--   0        0        0     5679 2024-02-27 08:20:01.234252 phringe-0.0.8/phringe/phringe.py
--rw-r--r--   0        0        0        0 2024-02-14 13:23:10.827561 phringe-0.0.8/phringe/util/__init__.py
--rw-r--r--   0        0        0     1845 2024-02-14 13:23:10.827561 phringe-0.0.8/phringe/util/grid.py
--rw-r--r--   0        0        0      364 2024-02-21 15:47:23.439454 phringe-0.0.8/phringe/util/helpers.py
--rw-r--r--   0        0        0      609 2024-02-08 09:36:31.886993 phringe-0.0.8/phringe/util/matrix.py
--rw-r--r--   0        0        0     8978 2024-02-22 15:23:49.328550 phringe-0.0.8/phringe/util/noise_generator.py
--rw-r--r--   0        0        0     3104 2024-02-21 16:03:07.739057 phringe-0.0.8/phringe/util/spectrum.py
--rw-r--r--   0        0        0     1942 2024-02-27 08:37:25.042366 phringe-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3334 2024-02-21 08:57:12.437424 phringe-0.0.8/README.md
--rw-r--r--   0        0        0     4380 1970-01-01 00:00:00.000000 phringe-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-02-05 12:16:41.447059 phringe-0.0.9/LICENSE
+-rw-r--r--   0        0        0       15 2024-02-21 08:55:27.312918 phringe-0.0.9/phringe/__init__.py
+-rw-r--r--   0        0        0     1740 2024-03-01 11:33:01.890556 phringe-0.0.9/phringe/__main__.py
+-rw-r--r--   0        0        0        0 2024-02-08 08:35:21.257604 phringe-0.0.9/phringe/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-08 08:35:21.273625 phringe-0.0.9/phringe/core/entities/__init__.py
+-rw-r--r--   0        0        0      375 2024-02-08 09:22:44.811062 phringe-0.0.9/phringe/core/entities/base_component.py
+-rw-r--r--   0        0        0     5401 2024-02-22 15:40:57.194481 phringe-0.0.9/phringe/core/entities/observation.py
+-rw-r--r--   0        0        0        0 2024-02-08 08:35:21.273625 phringe-0.0.9/phringe/core/entities/observatory/__init__.py
+-rw-r--r--   0        0        0     7067 2024-02-27 12:57:18.149015 phringe-0.0.9/phringe/core/entities/observatory/array_configuration.py
+-rw-r--r--   0        0        0     5340 2024-02-08 09:08:54.823102 phringe-0.0.9/phringe/core/entities/observatory/beam_combination_scheme.py
+-rw-r--r--   0        0        0    18083 2024-02-27 13:05:32.881810 phringe-0.0.9/phringe/core/entities/observatory/observatory.py
+-rw-r--r--   0        0        0        0 2024-02-08 08:35:21.289407 phringe-0.0.9/phringe/core/entities/photon_sources/__init__.py
+-rw-r--r--   0        0        0     3344 2024-02-26 12:28:15.271437 phringe-0.0.9/phringe/core/entities/photon_sources/base_photon_source.py
+-rw-r--r--   0        0        0     5423 2024-02-26 12:28:15.276172 phringe-0.0.9/phringe/core/entities/photon_sources/exozodi.py
+-rw-r--r--   0        0        0     4024 2024-02-26 12:35:39.120595 phringe-0.0.9/phringe/core/entities/photon_sources/local_zodi.py
+-rw-r--r--   0        0        0    13870 2024-02-26 12:28:41.207998 phringe-0.0.9/phringe/core/entities/photon_sources/planet.py
+-rw-r--r--   0        0        0     7170 2024-02-26 12:28:50.055568 phringe-0.0.9/phringe/core/entities/photon_sources/star.py
+-rw-r--r--   0        0        0     5989 2024-02-27 08:32:05.732277 phringe-0.0.9/phringe/core/entities/scene.py
+-rw-r--r--   0        0        0     5172 2024-02-27 16:05:55.683735 phringe-0.0.9/phringe/core/entities/settings.py
+-rw-r--r--   0        0        0        0 2024-02-05 15:27:51.892809 phringe-0.0.9/phringe/core/processing/__init__.py
+-rw-r--r--   0        0        0    19923 2024-02-29 09:17:06.897063 phringe-0.0.9/phringe/core/processing/data_generator.py
+-rw-r--r--   0        0        0        0 2024-02-08 08:35:21.243748 phringe-0.0.9/phringe/io/__init__.py
+-rw-r--r--   0        0        0      878 2024-02-26 12:34:13.955489 phringe-0.0.9/phringe/io/fits_writer.py
+-rw-r--r--   0        0        0      623 2024-02-21 10:20:11.841601 phringe-0.0.9/phringe/io/txt_reader.py
+-rw-r--r--   0        0        0     1069 2024-02-29 14:06:19.678222 phringe-0.0.9/phringe/io/utils.py
+-rw-r--r--   0        0        0     1033 2024-02-08 09:36:48.784816 phringe-0.0.9/phringe/io/validators.py
+-rw-r--r--   0        0        0      783 2024-02-20 15:46:59.570736 phringe-0.0.9/phringe/io/yaml_handler.py
+-rw-r--r--   0        0        0     7525 2024-03-01 11:33:01.902680 phringe-0.0.9/phringe/phringe.py
+-rw-r--r--   0        0        0        0 2024-02-14 13:23:10.827561 phringe-0.0.9/phringe/util/__init__.py
+-rw-r--r--   0        0        0     1845 2024-02-14 13:23:10.827561 phringe-0.0.9/phringe/util/grid.py
+-rw-r--r--   0        0        0      364 2024-02-21 15:47:23.439454 phringe-0.0.9/phringe/util/helpers.py
+-rw-r--r--   0        0        0      609 2024-02-08 09:36:31.886993 phringe-0.0.9/phringe/util/matrix.py
+-rw-r--r--   0        0        0     8978 2024-02-22 15:23:49.328550 phringe-0.0.9/phringe/util/noise_generator.py
+-rw-r--r--   0        0        0     3104 2024-02-21 16:03:07.739057 phringe-0.0.9/phringe/util/spectrum.py
+-rw-r--r--   0        0        0     1942 2024-03-01 11:46:52.300562 phringe-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3334 2024-02-21 08:57:12.437424 phringe-0.0.9/README.md
+-rw-r--r--   0        0        0     4380 1970-01-01 00:00:00.000000 phringe-0.0.9/PKG-INFO
```

### Comparing `phringe-0.0.8/LICENSE` & `phringe-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `phringe-0.0.8/phringe/__main__.py` & `phringe-0.0.9/phringe/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,33 +34,33 @@
     type=click.Path(exists=True),
     help="Path to the output directory.",
     default=Path('.'),
     required=False
 )
 @click.option('--fits/--no-fits', default=True, help="Write data to FITS file.")
 @click.option('--copy/--no-copy', default=True, help="Write copy of input files to output directory.")
-@click.option('--stats/--no-stats', default=False,
-              help="Enable photon statistics by generate separate data sets for all sources.")
+@click.option('--sep/--no-sep', default=False,
+              help="Generate separate data for the individual sources.")
 def main(
         config: Path,
         exoplanetary_system: Path,
         spectrum_tuples=None,
         output_dir=Path('.'),
         fits=True,
         copy=True,
-        stats=False
+        sep=False
 ):
     """PHRINGE. synthetic PHotometRy data generator for nullING intErferometers.
 
     CONFIG: Path to the configuration file.
     EXOPLANETARY_SYSTEM: Path to the exoplanetary system file.
     """
     phringe = PHRINGE()
     phringe.run(
-        config_file_path_or_dict=config,
-        exoplanetary_system_file_path_or_dict=exoplanetary_system,
+        config_file_path=config,
+        exoplanetary_system_file_path=exoplanetary_system,
         spectrum_tuple=spectrum_tuples,
         output_dir=output_dir,
         write_fits=fits,
         create_copy=copy,
-        enable_stats=stats
+        generate_separate=sep
     )
```

### Comparing `phringe-0.0.8/phringe/core/entities/observation.py` & `phringe-0.0.9/phringe/core/entities/observation.py`

 * *Files identical despite different names*

### Comparing `phringe-0.0.8/phringe/core/entities/observatory/array_configuration.py` & `phringe-0.0.9/phringe/core/entities/observatory/array_configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,18 +20,18 @@
     EQUILATERAL_TRIANGLE_CIRCULAR_ROTATION = 'equilateral-triangle-circular-rotation'
     REGULAR_PENTAGON_CIRCULAR_ROTATION = 'regular-pentagon-circular-rotation'
 
 
 class ArrayConfiguration(ABC, BaseModel):
     """Class representation of a collector array configuration.
 
-    :param baseline_length: The length of the baseline
+    :param nulling_baseline_length: The length of the nulling baseline
     :param type: The type of the array configuration
     """
-    baseline_length: Any = None
+    nulling_baseline_length: Any = None
     type: Any = None
     collector_coordinates: Any = None
 
     @abstractmethod
     def get_collector_coordinates(
             self,
             time_steps: np.ndarray,
@@ -54,15 +54,15 @@
     type: Any = ArrayConfigurationEnum.EMMA_X_CIRCULAR_ROTATION
 
     def get_collector_coordinates(self,
                                   time_steps: np.ndarray,
                                   modulation_period: Quantity,
                                   baseline_ratio: int) -> Coordinates:
         rotation_matrix = get_2d_rotation_matrix(time_steps, modulation_period)
-        emma_x_static = self.baseline_length / 2 * np.array(
+        emma_x_static = self.nulling_baseline_length / 2 * np.array(
             [[baseline_ratio, baseline_ratio, -baseline_ratio, -baseline_ratio], [1, -1, -1, 1]])
         collector_positions = np.einsum('ijl,jk->ikl', rotation_matrix, emma_x_static)
         collector_coordinates = np.zeros(len(time_steps), dtype=object)
         for i in range(len(time_steps)):
             collector_coordinates[i] = Coordinates(collector_positions[0, :, i], collector_positions[1, :, i])
         return collector_coordinates
 
@@ -72,40 +72,41 @@
     """
     type: Any = ArrayConfigurationEnum.EMMA_X_DOUBLE_STRETCH
 
     def get_collector_coordinates(self,
                                   time_steps: np.ndarray,
                                   modulation_period: Quantity,
                                   baseline_ratio: int) -> np.ndarray:
-        emma_x_static = self.baseline_length / 2 * np.array(
+        emma_x_static = self.nulling_baseline_length / 2 * np.array(
             [[baseline_ratio, baseline_ratio, -baseline_ratio, -baseline_ratio], [1, -1, -1, 1]])
         # TODO: fix calculations
-        collector_positions = emma_x_static * (1 + (2 * self.baseline_length) / self.baseline_length * np.sin(
-            2 * np.pi * u.rad / modulation_period * time_steps))
+        collector_positions = emma_x_static * (
+                    1 + (2 * self.nulling_baseline_length) / self.nulling_baseline_length * np.sin(
+                2 * np.pi * u.rad / modulation_period * time_steps))
         return Coordinates(collector_positions[0], collector_positions[1])
 
 
 class EquilateralTriangleCircularRotation(ArrayConfiguration):
     """Class representation of an equilateral triangle configuration with circular rotation of the array.
     """
     type: Any = ArrayConfigurationEnum.EQUILATERAL_TRIANGLE_CIRCULAR_ROTATION
 
     def get_collector_coordinates(self,
                                   time_steps: np.ndarray,
                                   modulation_period: Quantity,
                                   baseline_ratio: int) -> np.ndarray:
-        height = np.sqrt(3) / 2 * self.baseline_length
+        height = np.sqrt(3) / 2 * self.nulling_baseline_length
         height_to_center = height / 3
         rotation_matrix = get_2d_rotation_matrix(time_steps, modulation_period)
 
         equilateral_triangle_static = np.array(
-            [[0, self.baseline_length.value / 2, -self.baseline_length.value / 2],
+            [[0, self.nulling_baseline_length.value / 2, -self.nulling_baseline_length.value / 2],
              [height.value - height_to_center.value, -height_to_center.value, -height_to_center.value]])
         collector_positions = np.einsum('ijl,jk->ikl', rotation_matrix,
-                                        equilateral_triangle_static) * self.baseline_length.unit
+                                        equilateral_triangle_static) * self.nulling_baseline_length.unit
         collector_coordinates = np.zeros(len(time_steps), dtype=object)
         for i in range(len(time_steps)):
             collector_coordinates[i] = Coordinates(collector_positions[0, :, i], collector_positions[1, :, i])
         return collector_coordinates
 
 
 class RegularPentagonCircularRotation(ArrayConfiguration):
@@ -115,34 +116,34 @@
 
     def _get_x_position(self, angle) -> astropy.units.Quantity:
         """Return the x position.
 
         :param angle: The angle at which the collector is located
         :return: The x position
         """
-        return 0.851 * self.baseline_length.value * np.cos(angle)
+        return 0.851 * self.nulling_baseline_length.value * np.cos(angle)
 
     def _get_y_position(self, angle) -> astropy.units.Quantity:
         """Return the y position.
 
         :param angle: The angle at which the collector is located
         :return: The y position
         """
-        return 0.851 * self.baseline_length.value * np.sin(angle)
+        return 0.851 * self.nulling_baseline_length.value * np.sin(angle)
 
     def get_collector_coordinates(self,
                                   time_steps: np.ndarray,
                                   modulation_period: Quantity,
                                   baseline_ratio: int) -> np.ndarray:
         angles = [0, 2 * np.pi / 5, 4 * np.pi / 5, 6 * np.pi / 5, 8 * np.pi / 5]
         rotation_matrix = get_2d_rotation_matrix(time_steps, modulation_period)
         pentagon_static = np.array([
             [self._get_x_position(angles[0]), self._get_x_position(angles[1]), self._get_x_position(angles[2]),
              self._get_x_position(angles[3]), self._get_x_position(angles[4])],
             [self._get_y_position(angles[0]), self._get_y_position(angles[1]), self._get_y_position(angles[2]),
              self._get_y_position(angles[3]), self._get_y_position(angles[4])]])
         collector_positions = np.einsum('ijl,jk->ikl', rotation_matrix,
-                                        pentagon_static) * self.baseline_length.unit
+                                        pentagon_static) * self.nulling_baseline_length.unit
         collector_coordinates = np.zeros(len(time_steps), dtype=object)
         for i in range(len(time_steps)):
             collector_coordinates[i] = Coordinates(collector_positions[0, :, i], collector_positions[1, :, i])
         return collector_coordinates
```

### Comparing `phringe-0.0.8/phringe/core/entities/observatory/beam_combination_scheme.py` & `phringe-0.0.9/phringe/core/entities/observatory/beam_combination_scheme.py`

 * *Files identical despite different names*

### Comparing `phringe-0.0.8/phringe/core/entities/observatory/observatory.py` & `phringe-0.0.9/phringe/core/entities/observatory/observatory.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,15 +235,15 @@
         :param optimized_differential_output: The optimized differential output index
         :param optimized_wavelength: The optimized wavelength
         :param optimized_angular_distance: The optimized angular distance
         :return: The optimal baseline
         """
         # TODO: Check all factors again
         factors = (1,)
-        match (self.array_configuration.type, self.beam_combination_scheme.type):
+        match (self.array_configuration.type.value, self.beam_combination_scheme.type):
 
             # 3 collector arrays
             case (ArrayConfigurationEnum.EQUILATERAL_TRIANGLE_CIRCULAR_ROTATION.value,
                   BeamCombinationSchemeEnum.KERNEL_3.value, ):
                 factors = (0.67,)
 
             # 4 collector arrays
@@ -344,15 +344,15 @@
             optimized_angular_distance=optimized_star_separation,
         ).to(u.m)
 
         if (
                 baseline_minimum.to(u.m).value <= optimal_baseline.value
                 and optimal_baseline.value <= baseline_maximum.to(u.m).value
         ):
-            self.array_configuration.baseline_length = optimal_baseline
+            self.array_configuration.nulling_baseline_length = optimal_baseline
         else:
             raise ValueError(
                 f"Optimal baseline of {optimal_baseline} is not within allowed ranges of baselines {self.array_configuration.baseline_minimum}-{self.array_configuration.baseline_maximum}"
             )
 
     def prepare(self, settings, observation, scene):
         """Prepare the observatory for the simulation.
```

### Comparing `phringe-0.0.8/phringe/core/entities/photon_sources/base_photon_source.py` & `phringe-0.0.9/phringe/core/entities/photon_sources/base_photon_source.py`

 * *Files identical despite different names*

### Comparing `phringe-0.0.8/phringe/core/entities/photon_sources/exozodi.py` & `phringe-0.0.9/phringe/core/entities/photon_sources/exozodi.py`

 * *Files identical despite different names*

### Comparing `phringe-0.0.8/phringe/core/entities/photon_sources/local_zodi.py` & `phringe-0.0.9/phringe/core/entities/photon_sources/local_zodi.py`

 * *Files identical despite different names*

### Comparing `phringe-0.0.8/phringe/core/entities/photon_sources/planet.py` & `phringe-0.0.9/phringe/core/entities/photon_sources/planet.py`

 * *Files identical despite different names*

### Comparing `phringe-0.0.8/phringe/core/entities/photon_sources/star.py` & `phringe-0.0.9/phringe/core/entities/photon_sources/star.py`

 * *Files identical despite different names*

### Comparing `phringe-0.0.8/phringe/core/entities/scene.py` & `phringe-0.0.9/phringe/core/entities/scene.py`

 * *Files identical despite different names*

### Comparing `phringe-0.0.8/phringe/core/entities/settings.py` & `phringe-0.0.9/phringe/core/entities/settings.py`

 * *Files identical despite different names*

### Comparing `phringe-0.0.8/phringe/core/processing/data_generator.py` & `phringe-0.0.9/phringe/core/processing/data_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
             settings.has_exozodi_leakage
         )
         self.star = scene.star
         self.simulation_time_step_duration = settings.simulation_time_step_duration.to(u.s).value
         self.simulation_time_steps = settings.simulation_time_steps.to(u.s).value
         self.unperturbed_instrument_throughput = observatory.unperturbed_instrument_throughput
         self.simulation_wavelength_steps = settings.simulation_wavelength_steps.to(u.m).value
-        self.simulation_wavelength_bin_widhts = settings.simulation_wavelength_bin_widths.to(u.m).value
+        self.simulation_wavelength_bin_widths = settings.simulation_wavelength_bin_widths.to(u.m).value
         self.differential_photon_counts = self._initialize_differential_photon_counts()
         self.binned_photon_counts = self._initialize_binned_photon_counts()
         self._remove_units_from_source_sky_coordinates()
         self._remove_units_from_source_sky_brightness_distribution()
         self._remove_units_from_collector_coordinates()
 
     def _apply_shot_noise(self, mean_photon_counts) -> int:
@@ -246,15 +246,15 @@
             source_sky_brightness_distribution = source.sky_brightness_distribution[index_time]
         else:
             source_sky_brightness_distribution = source.sky_brightness_distribution
 
         photon_counts = np.zeros(self.number_of_outputs)
         index_wavelength = int(np.where(self.simulation_wavelength_steps == wavelength)[0])
         normalization = self._calculate_normalization(source_sky_brightness_distribution, index_wavelength)
-        wavelength_bin_width = self.simulation_wavelength_bin_widhts[index_wavelength]
+        wavelength_bin_width = self.simulation_wavelength_bin_widths[index_wavelength]
 
         for index_ir, intensity_response in enumerate(intensity_response):
             mean_photon_counts = (
                     np.sum(intensity_response
                            * source_sky_brightness_distribution[index_wavelength]
                            * self.simulation_time_step_duration
                            * wavelength_bin_width)
```

### Comparing `phringe-0.0.8/phringe/io/fits_writer.py` & `phringe-0.0.9/phringe/io/fits_writer.py`

 * *Files identical despite different names*

### Comparing `phringe-0.0.8/phringe/io/txt_reader.py` & `phringe-0.0.9/phringe/io/txt_reader.py`

 * *Files identical despite different names*

### Comparing `phringe-0.0.8/phringe/io/utils.py` & `phringe-0.0.9/phringe/io/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 from pathlib import Path
-from typing import Union
 
 from phringe.io.txt_reader import TXTReader
 from phringe.io.yaml_handler import YAMLHandler
 from phringe.util.helpers import SpectrumContext
 
 
-def get_dict_from_path_or_dict(file_path_or_dict: Union[Path, dict]) -> dict:
-    """Read the dictionary from the path and return it or return the dictionary directly.
+def get_dict_from_path(file_path: Path) -> dict:
+    """Read the dictionary from the path and return it.
 
-    :param file_path_or_dict: The path to the file or the dictionary
+    :param file_path: The path to the file
     :return: The dictionary
     """
-    try:
-        config_file_path_or_dict = Path(file_path_or_dict)
-        config_dict = YAMLHandler().read(file_path_or_dict)
-    except TypeError:
-        config_dict = file_path_or_dict
-    return config_dict
+    dict = YAMLHandler().read(file_path)
+    return dict
 
 
 def get_spectra_from_path(spectrum_tuple: tuple[tuple[str, Path]]) -> list[SpectrumContext]:
     """Read the spectra from the paths and return a list of SpectrumContext objects.
 
     :param spectrum_tuple: List of tuples containing the planet name and the path to the corresponding spectrum text file
     :return: The spectra
```

### Comparing `phringe-0.0.8/phringe/io/validators.py` & `phringe-0.0.9/phringe/io/validators.py`

 * *Files identical despite different names*

### Comparing `phringe-0.0.8/phringe/io/yaml_handler.py` & `phringe-0.0.9/phringe/io/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `phringe-0.0.8/phringe/util/grid.py` & `phringe-0.0.9/phringe/util/grid.py`

 * *Files identical despite different names*

### Comparing `phringe-0.0.8/phringe/util/matrix.py` & `phringe-0.0.9/phringe/util/matrix.py`

 * *Files identical despite different names*

### Comparing `phringe-0.0.8/phringe/util/noise_generator.py` & `phringe-0.0.9/phringe/util/noise_generator.py`

 * *Files identical despite different names*

### Comparing `phringe-0.0.8/phringe/util/spectrum.py` & `phringe-0.0.9/phringe/util/spectrum.py`

 * *Files identical despite different names*

### Comparing `phringe-0.0.8/pyproject.toml` & `phringe-0.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "phringe"
-version = "0.0.8"
+version = "0.0.9"
 description = "PHRINGE"
 authors = ["Philipp A. Huber <huberph@phys.ethz.ch>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pahuber/phringe"
 repository = "https://github.com/pahuber/phringe"
 documentation = "https://phringe.readthedocs.io"
```

### Comparing `phringe-0.0.8/README.md` & `phringe-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `phringe-0.0.8/PKG-INFO` & `phringe-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phringe
-Version: 0.0.8
+Version: 0.0.9
 Summary: PHRINGE
 Home-page: https://github.com/pahuber/phringe
 License: MIT
 Author: Philipp A. Huber
 Author-email: huberph@phys.ethz.ch
 Requires-Python: >=3.9,<3.11
 Classifier: Development Status :: 4 - Beta
```

